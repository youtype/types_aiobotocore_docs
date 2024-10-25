# Type definitions

> [Index](../README.md) > [SupportApp](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SupportApp](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
    type annotations stubs module [types-aiobotocore-support-app](https://pypi.org/project/types-aiobotocore-support-app/).



## CreateSlackChannelConfigurationRequestRequestTypeDef

```python
# CreateSlackChannelConfigurationRequestRequestTypeDef definition

class CreateSlackChannelConfigurationRequestRequestTypeDef(TypedDict):
    channelId: str,
    channelRoleArn: str,
    notifyOnCaseSeverity: NotificationSeverityLevelType,  # (1)
    teamId: str,
    channelName: NotRequired[str],
    notifyOnAddCorrespondenceToCase: NotRequired[bool],
    notifyOnCreateOrReopenCase: NotRequired[bool],
    notifyOnResolveCase: NotRequired[bool],
```

1. See [:material-code-brackets: NotificationSeverityLevelType](./literals.md#notificationseverityleveltype) 
## DeleteSlackChannelConfigurationRequestRequestTypeDef

```python
# DeleteSlackChannelConfigurationRequestRequestTypeDef definition

class DeleteSlackChannelConfigurationRequestRequestTypeDef(TypedDict):
    channelId: str,
    teamId: str,
```

## DeleteSlackWorkspaceConfigurationRequestRequestTypeDef

```python
# DeleteSlackWorkspaceConfigurationRequestRequestTypeDef definition

class DeleteSlackWorkspaceConfigurationRequestRequestTypeDef(TypedDict):
    teamId: str,
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

## ListSlackChannelConfigurationsRequestRequestTypeDef

```python
# ListSlackChannelConfigurationsRequestRequestTypeDef definition

class ListSlackChannelConfigurationsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
```

## SlackChannelConfigurationTypeDef

```python
# SlackChannelConfigurationTypeDef definition

class SlackChannelConfigurationTypeDef(TypedDict):
    channelId: str,
    teamId: str,
    channelName: NotRequired[str],
    channelRoleArn: NotRequired[str],
    notifyOnAddCorrespondenceToCase: NotRequired[bool],
    notifyOnCaseSeverity: NotRequired[NotificationSeverityLevelType],  # (1)
    notifyOnCreateOrReopenCase: NotRequired[bool],
    notifyOnResolveCase: NotRequired[bool],
```

1. See [:material-code-brackets: NotificationSeverityLevelType](./literals.md#notificationseverityleveltype) 
## ListSlackWorkspaceConfigurationsRequestRequestTypeDef

```python
# ListSlackWorkspaceConfigurationsRequestRequestTypeDef definition

class ListSlackWorkspaceConfigurationsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
```

## SlackWorkspaceConfigurationTypeDef

```python
# SlackWorkspaceConfigurationTypeDef definition

class SlackWorkspaceConfigurationTypeDef(TypedDict):
    teamId: str,
    allowOrganizationMemberAccount: NotRequired[bool],
    teamName: NotRequired[str],
```

## PutAccountAliasRequestRequestTypeDef

```python
# PutAccountAliasRequestRequestTypeDef definition

class PutAccountAliasRequestRequestTypeDef(TypedDict):
    accountAlias: str,
```

## RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef

```python
# RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef definition

class RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef(TypedDict):
    teamId: str,
```

## UpdateSlackChannelConfigurationRequestRequestTypeDef

```python
# UpdateSlackChannelConfigurationRequestRequestTypeDef definition

class UpdateSlackChannelConfigurationRequestRequestTypeDef(TypedDict):
    channelId: str,
    teamId: str,
    channelName: NotRequired[str],
    channelRoleArn: NotRequired[str],
    notifyOnAddCorrespondenceToCase: NotRequired[bool],
    notifyOnCaseSeverity: NotRequired[NotificationSeverityLevelType],  # (1)
    notifyOnCreateOrReopenCase: NotRequired[bool],
    notifyOnResolveCase: NotRequired[bool],
```

1. See [:material-code-brackets: NotificationSeverityLevelType](./literals.md#notificationseverityleveltype) 
## GetAccountAliasResultTypeDef

```python
# GetAccountAliasResultTypeDef definition

class GetAccountAliasResultTypeDef(TypedDict):
    accountAlias: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterSlackWorkspaceForOrganizationResultTypeDef

```python
# RegisterSlackWorkspaceForOrganizationResultTypeDef definition

class RegisterSlackWorkspaceForOrganizationResultTypeDef(TypedDict):
    accountType: AccountTypeType,  # (1)
    teamId: str,
    teamName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AccountTypeType](./literals.md#accounttypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSlackChannelConfigurationResultTypeDef

```python
# UpdateSlackChannelConfigurationResultTypeDef definition

class UpdateSlackChannelConfigurationResultTypeDef(TypedDict):
    channelId: str,
    channelName: str,
    channelRoleArn: str,
    notifyOnAddCorrespondenceToCase: bool,
    notifyOnCaseSeverity: NotificationSeverityLevelType,  # (1)
    notifyOnCreateOrReopenCase: bool,
    notifyOnResolveCase: bool,
    teamId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: NotificationSeverityLevelType](./literals.md#notificationseverityleveltype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSlackChannelConfigurationsResultTypeDef

```python
# ListSlackChannelConfigurationsResultTypeDef definition

class ListSlackChannelConfigurationsResultTypeDef(TypedDict):
    slackChannelConfigurations: List[SlackChannelConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SlackChannelConfigurationTypeDef](./type_defs.md#slackchannelconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSlackWorkspaceConfigurationsResultTypeDef

```python
# ListSlackWorkspaceConfigurationsResultTypeDef definition

class ListSlackWorkspaceConfigurationsResultTypeDef(TypedDict):
    slackWorkspaceConfigurations: List[SlackWorkspaceConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SlackWorkspaceConfigurationTypeDef](./type_defs.md#slackworkspaceconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
