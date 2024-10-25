# Type definitions

> [Index](../README.md) > [Chatbot](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Chatbot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
    type annotations stubs module [types-aiobotocore-chatbot](https://pypi.org/project/types-aiobotocore-chatbot/).



## AccountPreferencesTypeDef

```python
# AccountPreferencesTypeDef definition

class AccountPreferencesTypeDef(TypedDict):
    UserAuthorizationRequired: NotRequired[bool],
    TrainingDataCollectionEnabled: NotRequired[bool],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    TagKey: str,
    TagValue: str,
```

## ConfiguredTeamTypeDef

```python
# ConfiguredTeamTypeDef definition

class ConfiguredTeamTypeDef(TypedDict):
    TenantId: str,
    TeamId: str,
    TeamName: NotRequired[str],
    State: NotRequired[str],
    StateReason: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## DeleteChimeWebhookConfigurationRequestRequestTypeDef

```python
# DeleteChimeWebhookConfigurationRequestRequestTypeDef definition

class DeleteChimeWebhookConfigurationRequestRequestTypeDef(TypedDict):
    ChatConfigurationArn: str,
```

## DeleteMicrosoftTeamsUserIdentityRequestRequestTypeDef

```python
# DeleteMicrosoftTeamsUserIdentityRequestRequestTypeDef definition

class DeleteMicrosoftTeamsUserIdentityRequestRequestTypeDef(TypedDict):
    ChatConfigurationArn: str,
    UserId: str,
```

## DeleteSlackChannelConfigurationRequestRequestTypeDef

```python
# DeleteSlackChannelConfigurationRequestRequestTypeDef definition

class DeleteSlackChannelConfigurationRequestRequestTypeDef(TypedDict):
    ChatConfigurationArn: str,
```

## DeleteSlackUserIdentityRequestRequestTypeDef

```python
# DeleteSlackUserIdentityRequestRequestTypeDef definition

class DeleteSlackUserIdentityRequestRequestTypeDef(TypedDict):
    ChatConfigurationArn: str,
    SlackTeamId: str,
    SlackUserId: str,
```

## DeleteSlackWorkspaceAuthorizationRequestRequestTypeDef

```python
# DeleteSlackWorkspaceAuthorizationRequestRequestTypeDef definition

class DeleteSlackWorkspaceAuthorizationRequestRequestTypeDef(TypedDict):
    SlackTeamId: str,
```

## DeleteTeamsChannelConfigurationRequestRequestTypeDef

```python
# DeleteTeamsChannelConfigurationRequestRequestTypeDef definition

class DeleteTeamsChannelConfigurationRequestRequestTypeDef(TypedDict):
    ChatConfigurationArn: str,
```

## DeleteTeamsConfiguredTeamRequestRequestTypeDef

```python
# DeleteTeamsConfiguredTeamRequestRequestTypeDef definition

class DeleteTeamsConfiguredTeamRequestRequestTypeDef(TypedDict):
    TeamId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeChimeWebhookConfigurationsRequestRequestTypeDef

```python
# DescribeChimeWebhookConfigurationsRequestRequestTypeDef definition

class DescribeChimeWebhookConfigurationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChatConfigurationArn: NotRequired[str],
```

## DescribeSlackChannelConfigurationsRequestRequestTypeDef

```python
# DescribeSlackChannelConfigurationsRequestRequestTypeDef definition

class DescribeSlackChannelConfigurationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChatConfigurationArn: NotRequired[str],
```

## DescribeSlackUserIdentitiesRequestRequestTypeDef

```python
# DescribeSlackUserIdentitiesRequestRequestTypeDef definition

class DescribeSlackUserIdentitiesRequestRequestTypeDef(TypedDict):
    ChatConfigurationArn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SlackUserIdentityTypeDef

```python
# SlackUserIdentityTypeDef definition

class SlackUserIdentityTypeDef(TypedDict):
    IamRoleArn: str,
    ChatConfigurationArn: str,
    SlackTeamId: str,
    SlackUserId: str,
    AwsUserIdentity: NotRequired[str],
```

## DescribeSlackWorkspacesRequestRequestTypeDef

```python
# DescribeSlackWorkspacesRequestRequestTypeDef definition

class DescribeSlackWorkspacesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## SlackWorkspaceTypeDef

```python
# SlackWorkspaceTypeDef definition

class SlackWorkspaceTypeDef(TypedDict):
    SlackTeamId: str,
    SlackTeamName: str,
    State: NotRequired[str],
    StateReason: NotRequired[str],
```

## GetTeamsChannelConfigurationRequestRequestTypeDef

```python
# GetTeamsChannelConfigurationRequestRequestTypeDef definition

class GetTeamsChannelConfigurationRequestRequestTypeDef(TypedDict):
    ChatConfigurationArn: str,
```

## ListMicrosoftTeamsConfiguredTeamsRequestRequestTypeDef

```python
# ListMicrosoftTeamsConfiguredTeamsRequestRequestTypeDef definition

class ListMicrosoftTeamsConfiguredTeamsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListMicrosoftTeamsUserIdentitiesRequestRequestTypeDef

```python
# ListMicrosoftTeamsUserIdentitiesRequestRequestTypeDef definition

class ListMicrosoftTeamsUserIdentitiesRequestRequestTypeDef(TypedDict):
    ChatConfigurationArn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## TeamsUserIdentityTypeDef

```python
# TeamsUserIdentityTypeDef definition

class TeamsUserIdentityTypeDef(TypedDict):
    IamRoleArn: str,
    ChatConfigurationArn: str,
    TeamId: str,
    UserId: NotRequired[str],
    AwsUserIdentity: NotRequired[str],
    TeamsChannelId: NotRequired[str],
    TeamsTenantId: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## ListTeamsChannelConfigurationsRequestRequestTypeDef

```python
# ListTeamsChannelConfigurationsRequestRequestTypeDef definition

class ListTeamsChannelConfigurationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    TeamId: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateAccountPreferencesRequestRequestTypeDef

```python
# UpdateAccountPreferencesRequestRequestTypeDef definition

class UpdateAccountPreferencesRequestRequestTypeDef(TypedDict):
    UserAuthorizationRequired: NotRequired[bool],
    TrainingDataCollectionEnabled: NotRequired[bool],
```

## UpdateChimeWebhookConfigurationRequestRequestTypeDef

```python
# UpdateChimeWebhookConfigurationRequestRequestTypeDef definition

class UpdateChimeWebhookConfigurationRequestRequestTypeDef(TypedDict):
    ChatConfigurationArn: str,
    WebhookDescription: NotRequired[str],
    WebhookUrl: NotRequired[str],
    SnsTopicArns: NotRequired[Sequence[str]],
    IamRoleArn: NotRequired[str],
    LoggingLevel: NotRequired[str],
```

## UpdateSlackChannelConfigurationRequestRequestTypeDef

```python
# UpdateSlackChannelConfigurationRequestRequestTypeDef definition

class UpdateSlackChannelConfigurationRequestRequestTypeDef(TypedDict):
    ChatConfigurationArn: str,
    SlackChannelId: str,
    SlackChannelName: NotRequired[str],
    SnsTopicArns: NotRequired[Sequence[str]],
    IamRoleArn: NotRequired[str],
    LoggingLevel: NotRequired[str],
    GuardrailPolicyArns: NotRequired[Sequence[str]],
    UserAuthorizationRequired: NotRequired[bool],
```

## UpdateTeamsChannelConfigurationRequestRequestTypeDef

```python
# UpdateTeamsChannelConfigurationRequestRequestTypeDef definition

class UpdateTeamsChannelConfigurationRequestRequestTypeDef(TypedDict):
    ChatConfigurationArn: str,
    ChannelId: str,
    ChannelName: NotRequired[str],
    SnsTopicArns: NotRequired[Sequence[str]],
    IamRoleArn: NotRequired[str],
    LoggingLevel: NotRequired[str],
    GuardrailPolicyArns: NotRequired[Sequence[str]],
    UserAuthorizationRequired: NotRequired[bool],
```

## ChimeWebhookConfigurationTypeDef

```python
# ChimeWebhookConfigurationTypeDef definition

class ChimeWebhookConfigurationTypeDef(TypedDict):
    WebhookDescription: str,
    ChatConfigurationArn: str,
    IamRoleArn: str,
    SnsTopicArns: List[str],
    ConfigurationName: NotRequired[str],
    LoggingLevel: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
    State: NotRequired[str],
    StateReason: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateChimeWebhookConfigurationRequestRequestTypeDef

```python
# CreateChimeWebhookConfigurationRequestRequestTypeDef definition

class CreateChimeWebhookConfigurationRequestRequestTypeDef(TypedDict):
    WebhookDescription: str,
    WebhookUrl: str,
    SnsTopicArns: Sequence[str],
    IamRoleArn: str,
    ConfigurationName: str,
    LoggingLevel: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSlackChannelConfigurationRequestRequestTypeDef

```python
# CreateSlackChannelConfigurationRequestRequestTypeDef definition

class CreateSlackChannelConfigurationRequestRequestTypeDef(TypedDict):
    SlackTeamId: str,
    SlackChannelId: str,
    IamRoleArn: str,
    ConfigurationName: str,
    SlackChannelName: NotRequired[str],
    SnsTopicArns: NotRequired[Sequence[str]],
    LoggingLevel: NotRequired[str],
    GuardrailPolicyArns: NotRequired[Sequence[str]],
    UserAuthorizationRequired: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateTeamsChannelConfigurationRequestRequestTypeDef

```python
# CreateTeamsChannelConfigurationRequestRequestTypeDef definition

class CreateTeamsChannelConfigurationRequestRequestTypeDef(TypedDict):
    ChannelId: str,
    TeamId: str,
    TenantId: str,
    IamRoleArn: str,
    ConfigurationName: str,
    ChannelName: NotRequired[str],
    TeamName: NotRequired[str],
    SnsTopicArns: NotRequired[Sequence[str]],
    LoggingLevel: NotRequired[str],
    GuardrailPolicyArns: NotRequired[Sequence[str]],
    UserAuthorizationRequired: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## SlackChannelConfigurationTypeDef

```python
# SlackChannelConfigurationTypeDef definition

class SlackChannelConfigurationTypeDef(TypedDict):
    SlackTeamName: str,
    SlackTeamId: str,
    SlackChannelId: str,
    SlackChannelName: str,
    ChatConfigurationArn: str,
    IamRoleArn: str,
    SnsTopicArns: List[str],
    ConfigurationName: NotRequired[str],
    LoggingLevel: NotRequired[str],
    GuardrailPolicyArns: NotRequired[List[str]],
    UserAuthorizationRequired: NotRequired[bool],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
    State: NotRequired[str],
    StateReason: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TeamsChannelConfigurationTypeDef

```python
# TeamsChannelConfigurationTypeDef definition

class TeamsChannelConfigurationTypeDef(TypedDict):
    ChannelId: str,
    TeamId: str,
    TenantId: str,
    ChatConfigurationArn: str,
    IamRoleArn: str,
    SnsTopicArns: List[str],
    ChannelName: NotRequired[str],
    TeamName: NotRequired[str],
    ConfigurationName: NotRequired[str],
    LoggingLevel: NotRequired[str],
    GuardrailPolicyArns: NotRequired[List[str]],
    UserAuthorizationRequired: NotRequired[bool],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
    State: NotRequired[str],
    StateReason: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetAccountPreferencesResultTypeDef

```python
# GetAccountPreferencesResultTypeDef definition

class GetAccountPreferencesResultTypeDef(TypedDict):
    AccountPreferences: AccountPreferencesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountPreferencesTypeDef](./type_defs.md#accountpreferencestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMicrosoftTeamsConfiguredTeamsResultTypeDef

```python
# ListMicrosoftTeamsConfiguredTeamsResultTypeDef definition

class ListMicrosoftTeamsConfiguredTeamsResultTypeDef(TypedDict):
    ConfiguredTeams: List[ConfiguredTeamTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfiguredTeamTypeDef](./type_defs.md#configuredteamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountPreferencesResultTypeDef

```python
# UpdateAccountPreferencesResultTypeDef definition

class UpdateAccountPreferencesResultTypeDef(TypedDict):
    AccountPreferences: AccountPreferencesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountPreferencesTypeDef](./type_defs.md#accountpreferencestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChimeWebhookConfigurationsRequestDescribeChimeWebhookConfigurationsPaginateTypeDef

```python
# DescribeChimeWebhookConfigurationsRequestDescribeChimeWebhookConfigurationsPaginateTypeDef definition

class DescribeChimeWebhookConfigurationsRequestDescribeChimeWebhookConfigurationsPaginateTypeDef(TypedDict):
    ChatConfigurationArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSlackChannelConfigurationsRequestDescribeSlackChannelConfigurationsPaginateTypeDef

```python
# DescribeSlackChannelConfigurationsRequestDescribeSlackChannelConfigurationsPaginateTypeDef definition

class DescribeSlackChannelConfigurationsRequestDescribeSlackChannelConfigurationsPaginateTypeDef(TypedDict):
    ChatConfigurationArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSlackUserIdentitiesRequestDescribeSlackUserIdentitiesPaginateTypeDef

```python
# DescribeSlackUserIdentitiesRequestDescribeSlackUserIdentitiesPaginateTypeDef definition

class DescribeSlackUserIdentitiesRequestDescribeSlackUserIdentitiesPaginateTypeDef(TypedDict):
    ChatConfigurationArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSlackWorkspacesRequestDescribeSlackWorkspacesPaginateTypeDef

```python
# DescribeSlackWorkspacesRequestDescribeSlackWorkspacesPaginateTypeDef definition

class DescribeSlackWorkspacesRequestDescribeSlackWorkspacesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMicrosoftTeamsConfiguredTeamsRequestListMicrosoftTeamsConfiguredTeamsPaginateTypeDef

```python
# ListMicrosoftTeamsConfiguredTeamsRequestListMicrosoftTeamsConfiguredTeamsPaginateTypeDef definition

class ListMicrosoftTeamsConfiguredTeamsRequestListMicrosoftTeamsConfiguredTeamsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMicrosoftTeamsUserIdentitiesRequestListMicrosoftTeamsUserIdentitiesPaginateTypeDef

```python
# ListMicrosoftTeamsUserIdentitiesRequestListMicrosoftTeamsUserIdentitiesPaginateTypeDef definition

class ListMicrosoftTeamsUserIdentitiesRequestListMicrosoftTeamsUserIdentitiesPaginateTypeDef(TypedDict):
    ChatConfigurationArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTeamsChannelConfigurationsRequestListMicrosoftTeamsChannelConfigurationsPaginateTypeDef

```python
# ListTeamsChannelConfigurationsRequestListMicrosoftTeamsChannelConfigurationsPaginateTypeDef definition

class ListTeamsChannelConfigurationsRequestListMicrosoftTeamsChannelConfigurationsPaginateTypeDef(TypedDict):
    TeamId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSlackUserIdentitiesResultTypeDef

```python
# DescribeSlackUserIdentitiesResultTypeDef definition

class DescribeSlackUserIdentitiesResultTypeDef(TypedDict):
    SlackUserIdentities: List[SlackUserIdentityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SlackUserIdentityTypeDef](./type_defs.md#slackuseridentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSlackWorkspacesResultTypeDef

```python
# DescribeSlackWorkspacesResultTypeDef definition

class DescribeSlackWorkspacesResultTypeDef(TypedDict):
    SlackWorkspaces: List[SlackWorkspaceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SlackWorkspaceTypeDef](./type_defs.md#slackworkspacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMicrosoftTeamsUserIdentitiesResultTypeDef

```python
# ListMicrosoftTeamsUserIdentitiesResultTypeDef definition

class ListMicrosoftTeamsUserIdentitiesResultTypeDef(TypedDict):
    TeamsUserIdentities: List[TeamsUserIdentityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TeamsUserIdentityTypeDef](./type_defs.md#teamsuseridentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChimeWebhookConfigurationResultTypeDef

```python
# CreateChimeWebhookConfigurationResultTypeDef definition

class CreateChimeWebhookConfigurationResultTypeDef(TypedDict):
    WebhookConfiguration: ChimeWebhookConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChimeWebhookConfigurationTypeDef](./type_defs.md#chimewebhookconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChimeWebhookConfigurationsResultTypeDef

```python
# DescribeChimeWebhookConfigurationsResultTypeDef definition

class DescribeChimeWebhookConfigurationsResultTypeDef(TypedDict):
    WebhookConfigurations: List[ChimeWebhookConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChimeWebhookConfigurationTypeDef](./type_defs.md#chimewebhookconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChimeWebhookConfigurationResultTypeDef

```python
# UpdateChimeWebhookConfigurationResultTypeDef definition

class UpdateChimeWebhookConfigurationResultTypeDef(TypedDict):
    WebhookConfiguration: ChimeWebhookConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChimeWebhookConfigurationTypeDef](./type_defs.md#chimewebhookconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSlackChannelConfigurationResultTypeDef

```python
# CreateSlackChannelConfigurationResultTypeDef definition

class CreateSlackChannelConfigurationResultTypeDef(TypedDict):
    ChannelConfiguration: SlackChannelConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SlackChannelConfigurationTypeDef](./type_defs.md#slackchannelconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSlackChannelConfigurationsResultTypeDef

```python
# DescribeSlackChannelConfigurationsResultTypeDef definition

class DescribeSlackChannelConfigurationsResultTypeDef(TypedDict):
    SlackChannelConfigurations: List[SlackChannelConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SlackChannelConfigurationTypeDef](./type_defs.md#slackchannelconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSlackChannelConfigurationResultTypeDef

```python
# UpdateSlackChannelConfigurationResultTypeDef definition

class UpdateSlackChannelConfigurationResultTypeDef(TypedDict):
    ChannelConfiguration: SlackChannelConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SlackChannelConfigurationTypeDef](./type_defs.md#slackchannelconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTeamsChannelConfigurationResultTypeDef

```python
# CreateTeamsChannelConfigurationResultTypeDef definition

class CreateTeamsChannelConfigurationResultTypeDef(TypedDict):
    ChannelConfiguration: TeamsChannelConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TeamsChannelConfigurationTypeDef](./type_defs.md#teamschannelconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTeamsChannelConfigurationResultTypeDef

```python
# GetTeamsChannelConfigurationResultTypeDef definition

class GetTeamsChannelConfigurationResultTypeDef(TypedDict):
    ChannelConfiguration: TeamsChannelConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TeamsChannelConfigurationTypeDef](./type_defs.md#teamschannelconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTeamsChannelConfigurationsResultTypeDef

```python
# ListTeamsChannelConfigurationsResultTypeDef definition

class ListTeamsChannelConfigurationsResultTypeDef(TypedDict):
    TeamChannelConfigurations: List[TeamsChannelConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TeamsChannelConfigurationTypeDef](./type_defs.md#teamschannelconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTeamsChannelConfigurationResultTypeDef

```python
# UpdateTeamsChannelConfigurationResultTypeDef definition

class UpdateTeamsChannelConfigurationResultTypeDef(TypedDict):
    ChannelConfiguration: TeamsChannelConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TeamsChannelConfigurationTypeDef](./type_defs.md#teamschannelconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
