# ChatbotClient

> [Index](../README.md) > [Chatbot](./README.md) > ChatbotClient

!!! note ""

    Auto-generated documentation for [Chatbot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
    type annotations stubs module [types-aiobotocore-chatbot](https://pypi.org/project/types-aiobotocore-chatbot/).

## ChatbotClient

Type annotations and code completion for `#!python session.create_client("chatbot")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client)

```python
# ChatbotClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_chatbot.client import ChatbotClient

session = get_session()
async with session.create_client("chatbot") as client:
    client: ChatbotClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("chatbot").exceptions` structure.

```python
# ChatbotClient.exceptions usage example

async with session.create_client("chatbot") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConflictException,
        client.CreateChimeWebhookConfigurationException,
        client.CreateSlackChannelConfigurationException,
        client.CreateTeamsChannelConfigurationException,
        client.DeleteChimeWebhookConfigurationException,
        client.DeleteMicrosoftTeamsUserIdentityException,
        client.DeleteSlackChannelConfigurationException,
        client.DeleteSlackUserIdentityException,
        client.DeleteSlackWorkspaceAuthorizationFault,
        client.DeleteTeamsChannelConfigurationException,
        client.DeleteTeamsConfiguredTeamException,
        client.DescribeChimeWebhookConfigurationsException,
        client.DescribeSlackChannelConfigurationsException,
        client.DescribeSlackUserIdentitiesException,
        client.DescribeSlackWorkspacesException,
        client.GetAccountPreferencesException,
        client.GetTeamsChannelConfigurationException,
        client.InternalServiceError,
        client.InvalidParameterException,
        client.InvalidRequestException,
        client.LimitExceededException,
        client.ListMicrosoftTeamsConfiguredTeamsException,
        client.ListMicrosoftTeamsUserIdentitiesException,
        client.ListTeamsChannelConfigurationsException,
        client.ResourceNotFoundException,
        client.ServiceUnavailableException,
        client.TooManyTagsException,
        client.UpdateAccountPreferencesException,
        client.UpdateChimeWebhookConfigurationException,
        client.UpdateSlackChannelConfigurationException,
        client.UpdateTeamsChannelConfigurationException,
    ) as e:
        print(e)
```

```python
# ChatbotClient usage type checking example

from types_aiobotocore_chatbot.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("chatbot").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("chatbot").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_chime\_webhook\_configuration

Creates an AWS Chatbot configuration for Amazon Chime.

Type annotations and code completion for `#!python session.create_client("chatbot").create_chime_webhook_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_chime_webhook_configuration)

```python
# create_chime_webhook_configuration method definition

await def create_chime_webhook_configuration(
    self,
    *,
    WebhookDescription: str,
    WebhookUrl: str,
    SnsTopicArns: Sequence[str],
    IamRoleArn: str,
    ConfigurationName: str,
    LoggingLevel: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateChimeWebhookConfigurationResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateChimeWebhookConfigurationResultTypeDef](./type_defs.md#createchimewebhookconfigurationresulttypedef) 


```python
# create_chime_webhook_configuration method usage example with argument unpacking

kwargs: CreateChimeWebhookConfigurationRequestRequestTypeDef = {  # (1)
    "WebhookDescription": ...,
    "WebhookUrl": ...,
    "SnsTopicArns": ...,
    "IamRoleArn": ...,
    "ConfigurationName": ...,
}

parent.create_chime_webhook_configuration(**kwargs)
```

1. See [:material-code-braces: CreateChimeWebhookConfigurationRequestRequestTypeDef](./type_defs.md#createchimewebhookconfigurationrequestrequesttypedef) 

### create\_microsoft\_teams\_channel\_configuration

Creates an AWS Chatbot configuration for Microsoft Teams.

Type annotations and code completion for `#!python session.create_client("chatbot").create_microsoft_teams_channel_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_microsoft_teams_channel_configuration)

```python
# create_microsoft_teams_channel_configuration method definition

await def create_microsoft_teams_channel_configuration(
    self,
    *,
    ChannelId: str,
    TeamId: str,
    TenantId: str,
    IamRoleArn: str,
    ConfigurationName: str,
    ChannelName: str = ...,
    TeamName: str = ...,
    SnsTopicArns: Sequence[str] = ...,
    LoggingLevel: str = ...,
    GuardrailPolicyArns: Sequence[str] = ...,
    UserAuthorizationRequired: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateTeamsChannelConfigurationResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateTeamsChannelConfigurationResultTypeDef](./type_defs.md#createteamschannelconfigurationresulttypedef) 


```python
# create_microsoft_teams_channel_configuration method usage example with argument unpacking

kwargs: CreateTeamsChannelConfigurationRequestRequestTypeDef = {  # (1)
    "ChannelId": ...,
    "TeamId": ...,
    "TenantId": ...,
    "IamRoleArn": ...,
    "ConfigurationName": ...,
}

parent.create_microsoft_teams_channel_configuration(**kwargs)
```

1. See [:material-code-braces: CreateTeamsChannelConfigurationRequestRequestTypeDef](./type_defs.md#createteamschannelconfigurationrequestrequesttypedef) 

### create\_slack\_channel\_configuration

Creates an AWS Chatbot confugration for Slack.

Type annotations and code completion for `#!python session.create_client("chatbot").create_slack_channel_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_slack_channel_configuration)

```python
# create_slack_channel_configuration method definition

await def create_slack_channel_configuration(
    self,
    *,
    SlackTeamId: str,
    SlackChannelId: str,
    IamRoleArn: str,
    ConfigurationName: str,
    SlackChannelName: str = ...,
    SnsTopicArns: Sequence[str] = ...,
    LoggingLevel: str = ...,
    GuardrailPolicyArns: Sequence[str] = ...,
    UserAuthorizationRequired: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateSlackChannelConfigurationResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateSlackChannelConfigurationResultTypeDef](./type_defs.md#createslackchannelconfigurationresulttypedef) 


```python
# create_slack_channel_configuration method usage example with argument unpacking

kwargs: CreateSlackChannelConfigurationRequestRequestTypeDef = {  # (1)
    "SlackTeamId": ...,
    "SlackChannelId": ...,
    "IamRoleArn": ...,
    "ConfigurationName": ...,
}

parent.create_slack_channel_configuration(**kwargs)
```

1. See [:material-code-braces: CreateSlackChannelConfigurationRequestRequestTypeDef](./type_defs.md#createslackchannelconfigurationrequestrequesttypedef) 

### delete\_chime\_webhook\_configuration

Deletes a Amazon Chime webhook configuration for AWS Chatbot.

Type annotations and code completion for `#!python session.create_client("chatbot").delete_chime_webhook_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_chime_webhook_configuration)

```python
# delete_chime_webhook_configuration method definition

await def delete_chime_webhook_configuration(
    self,
    *,
    ChatConfigurationArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_chime_webhook_configuration method usage example with argument unpacking

kwargs: DeleteChimeWebhookConfigurationRequestRequestTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
}

parent.delete_chime_webhook_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteChimeWebhookConfigurationRequestRequestTypeDef](./type_defs.md#deletechimewebhookconfigurationrequestrequesttypedef) 

### delete\_microsoft\_teams\_channel\_configuration

Deletes a Microsoft Teams channel configuration for AWS Chatbot See also: [AWS
API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteMicrosoftTeamsChannelConfiguration).

Type annotations and code completion for `#!python session.create_client("chatbot").delete_microsoft_teams_channel_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_channel_configuration)

```python
# delete_microsoft_teams_channel_configuration method definition

await def delete_microsoft_teams_channel_configuration(
    self,
    *,
    ChatConfigurationArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_microsoft_teams_channel_configuration method usage example with argument unpacking

kwargs: DeleteTeamsChannelConfigurationRequestRequestTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
}

parent.delete_microsoft_teams_channel_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteTeamsChannelConfigurationRequestRequestTypeDef](./type_defs.md#deleteteamschannelconfigurationrequestrequesttypedef) 

### delete\_microsoft\_teams\_configured\_team

Deletes the Microsoft Teams team authorization allowing for channels to be
configured in that Microsoft Teams
team.

Type annotations and code completion for `#!python session.create_client("chatbot").delete_microsoft_teams_configured_team` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_configured_team)

```python
# delete_microsoft_teams_configured_team method definition

await def delete_microsoft_teams_configured_team(
    self,
    *,
    TeamId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_microsoft_teams_configured_team method usage example with argument unpacking

kwargs: DeleteTeamsConfiguredTeamRequestRequestTypeDef = {  # (1)
    "TeamId": ...,
}

parent.delete_microsoft_teams_configured_team(**kwargs)
```

1. See [:material-code-braces: DeleteTeamsConfiguredTeamRequestRequestTypeDef](./type_defs.md#deleteteamsconfiguredteamrequestrequesttypedef) 

### delete\_microsoft\_teams\_user\_identity

Identifes a user level permission for a channel configuration.

Type annotations and code completion for `#!python session.create_client("chatbot").delete_microsoft_teams_user_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_user_identity)

```python
# delete_microsoft_teams_user_identity method definition

await def delete_microsoft_teams_user_identity(
    self,
    *,
    ChatConfigurationArn: str,
    UserId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_microsoft_teams_user_identity method usage example with argument unpacking

kwargs: DeleteMicrosoftTeamsUserIdentityRequestRequestTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
    "UserId": ...,
}

parent.delete_microsoft_teams_user_identity(**kwargs)
```

1. See [:material-code-braces: DeleteMicrosoftTeamsUserIdentityRequestRequestTypeDef](./type_defs.md#deletemicrosoftteamsuseridentityrequestrequesttypedef) 

### delete\_slack\_channel\_configuration

Deletes a Slack channel configuration for AWS Chatbot See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteSlackChannelConfiguration).

Type annotations and code completion for `#!python session.create_client("chatbot").delete_slack_channel_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_channel_configuration)

```python
# delete_slack_channel_configuration method definition

await def delete_slack_channel_configuration(
    self,
    *,
    ChatConfigurationArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_slack_channel_configuration method usage example with argument unpacking

kwargs: DeleteSlackChannelConfigurationRequestRequestTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
}

parent.delete_slack_channel_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteSlackChannelConfigurationRequestRequestTypeDef](./type_defs.md#deleteslackchannelconfigurationrequestrequesttypedef) 

### delete\_slack\_user\_identity

Deletes a user level permission for a Slack channel configuration.

Type annotations and code completion for `#!python session.create_client("chatbot").delete_slack_user_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_user_identity)

```python
# delete_slack_user_identity method definition

await def delete_slack_user_identity(
    self,
    *,
    ChatConfigurationArn: str,
    SlackTeamId: str,
    SlackUserId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_slack_user_identity method usage example with argument unpacking

kwargs: DeleteSlackUserIdentityRequestRequestTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
    "SlackTeamId": ...,
    "SlackUserId": ...,
}

parent.delete_slack_user_identity(**kwargs)
```

1. See [:material-code-braces: DeleteSlackUserIdentityRequestRequestTypeDef](./type_defs.md#deleteslackuseridentityrequestrequesttypedef) 

### delete\_slack\_workspace\_authorization

Deletes the Slack workspace authorization that allows channels to be configured
in that
workspace.

Type annotations and code completion for `#!python session.create_client("chatbot").delete_slack_workspace_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_workspace_authorization)

```python
# delete_slack_workspace_authorization method definition

await def delete_slack_workspace_authorization(
    self,
    *,
    SlackTeamId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_slack_workspace_authorization method usage example with argument unpacking

kwargs: DeleteSlackWorkspaceAuthorizationRequestRequestTypeDef = {  # (1)
    "SlackTeamId": ...,
}

parent.delete_slack_workspace_authorization(**kwargs)
```

1. See [:material-code-braces: DeleteSlackWorkspaceAuthorizationRequestRequestTypeDef](./type_defs.md#deleteslackworkspaceauthorizationrequestrequesttypedef) 

### describe\_chime\_webhook\_configurations

Lists Amazon Chime webhook configurations optionally filtered by
ChatConfigurationArn See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeChimeWebhookConfigurations).

Type annotations and code completion for `#!python session.create_client("chatbot").describe_chime_webhook_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_chime_webhook_configurations)

```python
# describe_chime_webhook_configurations method definition

await def describe_chime_webhook_configurations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    ChatConfigurationArn: str = ...,
) -> DescribeChimeWebhookConfigurationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChimeWebhookConfigurationsResultTypeDef](./type_defs.md#describechimewebhookconfigurationsresulttypedef) 


```python
# describe_chime_webhook_configurations method usage example with argument unpacking

kwargs: DescribeChimeWebhookConfigurationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.describe_chime_webhook_configurations(**kwargs)
```

1. See [:material-code-braces: DescribeChimeWebhookConfigurationsRequestRequestTypeDef](./type_defs.md#describechimewebhookconfigurationsrequestrequesttypedef) 

### describe\_slack\_channel\_configurations

Lists Slack channel configurations optionally filtered by ChatConfigurationArn
See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeSlackChannelConfigurations).

Type annotations and code completion for `#!python session.create_client("chatbot").describe_slack_channel_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_channel_configurations)

```python
# describe_slack_channel_configurations method definition

await def describe_slack_channel_configurations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    ChatConfigurationArn: str = ...,
) -> DescribeSlackChannelConfigurationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSlackChannelConfigurationsResultTypeDef](./type_defs.md#describeslackchannelconfigurationsresulttypedef) 


```python
# describe_slack_channel_configurations method usage example with argument unpacking

kwargs: DescribeSlackChannelConfigurationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.describe_slack_channel_configurations(**kwargs)
```

1. See [:material-code-braces: DescribeSlackChannelConfigurationsRequestRequestTypeDef](./type_defs.md#describeslackchannelconfigurationsrequestrequesttypedef) 

### describe\_slack\_user\_identities

Lists all Slack user identities with a mapped role.

Type annotations and code completion for `#!python session.create_client("chatbot").describe_slack_user_identities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_user_identities)

```python
# describe_slack_user_identities method definition

await def describe_slack_user_identities(
    self,
    *,
    ChatConfigurationArn: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeSlackUserIdentitiesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSlackUserIdentitiesResultTypeDef](./type_defs.md#describeslackuseridentitiesresulttypedef) 


```python
# describe_slack_user_identities method usage example with argument unpacking

kwargs: DescribeSlackUserIdentitiesRequestRequestTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
}

parent.describe_slack_user_identities(**kwargs)
```

1. See [:material-code-braces: DescribeSlackUserIdentitiesRequestRequestTypeDef](./type_defs.md#describeslackuseridentitiesrequestrequesttypedef) 

### describe\_slack\_workspaces

List all authorized Slack workspaces connected to the AWS Account onboarded
with AWS
Chatbot.

Type annotations and code completion for `#!python session.create_client("chatbot").describe_slack_workspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_workspaces)

```python
# describe_slack_workspaces method definition

await def describe_slack_workspaces(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeSlackWorkspacesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSlackWorkspacesResultTypeDef](./type_defs.md#describeslackworkspacesresulttypedef) 


```python
# describe_slack_workspaces method usage example with argument unpacking

kwargs: DescribeSlackWorkspacesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.describe_slack_workspaces(**kwargs)
```

1. See [:material-code-braces: DescribeSlackWorkspacesRequestRequestTypeDef](./type_defs.md#describeslackworkspacesrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("chatbot").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_account\_preferences

Returns AWS Chatbot account preferences.

Type annotations and code completion for `#!python session.create_client("chatbot").get_account_preferences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.get_account_preferences)

```python
# get_account_preferences method definition

await def get_account_preferences(
    self,
) -> GetAccountPreferencesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountPreferencesResultTypeDef](./type_defs.md#getaccountpreferencesresulttypedef) 

### get\_microsoft\_teams\_channel\_configuration

Returns a Microsoft Teams channel configuration in an AWS account.

Type annotations and code completion for `#!python session.create_client("chatbot").get_microsoft_teams_channel_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.get_microsoft_teams_channel_configuration)

```python
# get_microsoft_teams_channel_configuration method definition

await def get_microsoft_teams_channel_configuration(
    self,
    *,
    ChatConfigurationArn: str,
) -> GetTeamsChannelConfigurationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTeamsChannelConfigurationResultTypeDef](./type_defs.md#getteamschannelconfigurationresulttypedef) 


```python
# get_microsoft_teams_channel_configuration method usage example with argument unpacking

kwargs: GetTeamsChannelConfigurationRequestRequestTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
}

parent.get_microsoft_teams_channel_configuration(**kwargs)
```

1. See [:material-code-braces: GetTeamsChannelConfigurationRequestRequestTypeDef](./type_defs.md#getteamschannelconfigurationrequestrequesttypedef) 

### list\_microsoft\_teams\_channel\_configurations

Lists all AWS Chatbot Microsoft Teams channel configurations in an AWS account.

Type annotations and code completion for `#!python session.create_client("chatbot").list_microsoft_teams_channel_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_channel_configurations)

```python
# list_microsoft_teams_channel_configurations method definition

await def list_microsoft_teams_channel_configurations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    TeamId: str = ...,
) -> ListTeamsChannelConfigurationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTeamsChannelConfigurationsResultTypeDef](./type_defs.md#listteamschannelconfigurationsresulttypedef) 


```python
# list_microsoft_teams_channel_configurations method usage example with argument unpacking

kwargs: ListTeamsChannelConfigurationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_microsoft_teams_channel_configurations(**kwargs)
```

1. See [:material-code-braces: ListTeamsChannelConfigurationsRequestRequestTypeDef](./type_defs.md#listteamschannelconfigurationsrequestrequesttypedef) 

### list\_microsoft\_teams\_configured\_teams

Lists all authorized Microsoft Teams for an AWS Account See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/ListMicrosoftTeamsConfiguredTeams).

Type annotations and code completion for `#!python session.create_client("chatbot").list_microsoft_teams_configured_teams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_configured_teams)

```python
# list_microsoft_teams_configured_teams method definition

await def list_microsoft_teams_configured_teams(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListMicrosoftTeamsConfiguredTeamsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMicrosoftTeamsConfiguredTeamsResultTypeDef](./type_defs.md#listmicrosoftteamsconfiguredteamsresulttypedef) 


```python
# list_microsoft_teams_configured_teams method usage example with argument unpacking

kwargs: ListMicrosoftTeamsConfiguredTeamsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_microsoft_teams_configured_teams(**kwargs)
```

1. See [:material-code-braces: ListMicrosoftTeamsConfiguredTeamsRequestRequestTypeDef](./type_defs.md#listmicrosoftteamsconfiguredteamsrequestrequesttypedef) 

### list\_microsoft\_teams\_user\_identities

A list all Microsoft Teams user identities with a mapped role.

Type annotations and code completion for `#!python session.create_client("chatbot").list_microsoft_teams_user_identities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_user_identities)

```python
# list_microsoft_teams_user_identities method definition

await def list_microsoft_teams_user_identities(
    self,
    *,
    ChatConfigurationArn: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMicrosoftTeamsUserIdentitiesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMicrosoftTeamsUserIdentitiesResultTypeDef](./type_defs.md#listmicrosoftteamsuseridentitiesresulttypedef) 


```python
# list_microsoft_teams_user_identities method usage example with argument unpacking

kwargs: ListMicrosoftTeamsUserIdentitiesRequestRequestTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
}

parent.list_microsoft_teams_user_identities(**kwargs)
```

1. See [:material-code-braces: ListMicrosoftTeamsUserIdentitiesRequestRequestTypeDef](./type_defs.md#listmicrosoftteamsuseridentitiesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists all of the tags associated with the Amazon Resource Name (ARN) that you
specify.

Type annotations and code completion for `#!python session.create_client("chatbot").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### tag\_resource

Attaches a key-value pair to a resource, as identified by its Amazon Resource
Name
(ARN).

Type annotations and code completion for `#!python session.create_client("chatbot").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Detaches a key-value pair from a resource, as identified by its Amazon Resource
Name
(ARN).

Type annotations and code completion for `#!python session.create_client("chatbot").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_account\_preferences

Updates AWS Chatbot account preferences.

Type annotations and code completion for `#!python session.create_client("chatbot").update_account_preferences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_account_preferences)

```python
# update_account_preferences method definition

await def update_account_preferences(
    self,
    *,
    UserAuthorizationRequired: bool = ...,
    TrainingDataCollectionEnabled: bool = ...,
) -> UpdateAccountPreferencesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAccountPreferencesResultTypeDef](./type_defs.md#updateaccountpreferencesresulttypedef) 


```python
# update_account_preferences method usage example with argument unpacking

kwargs: UpdateAccountPreferencesRequestRequestTypeDef = {  # (1)
    "UserAuthorizationRequired": ...,
}

parent.update_account_preferences(**kwargs)
```

1. See [:material-code-braces: UpdateAccountPreferencesRequestRequestTypeDef](./type_defs.md#updateaccountpreferencesrequestrequesttypedef) 

### update\_chime\_webhook\_configuration

Updates a Amazon Chime webhook configuration.

Type annotations and code completion for `#!python session.create_client("chatbot").update_chime_webhook_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_chime_webhook_configuration)

```python
# update_chime_webhook_configuration method definition

await def update_chime_webhook_configuration(
    self,
    *,
    ChatConfigurationArn: str,
    WebhookDescription: str = ...,
    WebhookUrl: str = ...,
    SnsTopicArns: Sequence[str] = ...,
    IamRoleArn: str = ...,
    LoggingLevel: str = ...,
) -> UpdateChimeWebhookConfigurationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateChimeWebhookConfigurationResultTypeDef](./type_defs.md#updatechimewebhookconfigurationresulttypedef) 


```python
# update_chime_webhook_configuration method usage example with argument unpacking

kwargs: UpdateChimeWebhookConfigurationRequestRequestTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
}

parent.update_chime_webhook_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateChimeWebhookConfigurationRequestRequestTypeDef](./type_defs.md#updatechimewebhookconfigurationrequestrequesttypedef) 

### update\_microsoft\_teams\_channel\_configuration

Updates an Microsoft Teams channel configuration.

Type annotations and code completion for `#!python session.create_client("chatbot").update_microsoft_teams_channel_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_microsoft_teams_channel_configuration)

```python
# update_microsoft_teams_channel_configuration method definition

await def update_microsoft_teams_channel_configuration(
    self,
    *,
    ChatConfigurationArn: str,
    ChannelId: str,
    ChannelName: str = ...,
    SnsTopicArns: Sequence[str] = ...,
    IamRoleArn: str = ...,
    LoggingLevel: str = ...,
    GuardrailPolicyArns: Sequence[str] = ...,
    UserAuthorizationRequired: bool = ...,
) -> UpdateTeamsChannelConfigurationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateTeamsChannelConfigurationResultTypeDef](./type_defs.md#updateteamschannelconfigurationresulttypedef) 


```python
# update_microsoft_teams_channel_configuration method usage example with argument unpacking

kwargs: UpdateTeamsChannelConfigurationRequestRequestTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
    "ChannelId": ...,
}

parent.update_microsoft_teams_channel_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateTeamsChannelConfigurationRequestRequestTypeDef](./type_defs.md#updateteamschannelconfigurationrequestrequesttypedef) 

### update\_slack\_channel\_configuration

Updates a Slack channel configuration.

Type annotations and code completion for `#!python session.create_client("chatbot").update_slack_channel_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_slack_channel_configuration)

```python
# update_slack_channel_configuration method definition

await def update_slack_channel_configuration(
    self,
    *,
    ChatConfigurationArn: str,
    SlackChannelId: str,
    SlackChannelName: str = ...,
    SnsTopicArns: Sequence[str] = ...,
    IamRoleArn: str = ...,
    LoggingLevel: str = ...,
    GuardrailPolicyArns: Sequence[str] = ...,
    UserAuthorizationRequired: bool = ...,
) -> UpdateSlackChannelConfigurationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateSlackChannelConfigurationResultTypeDef](./type_defs.md#updateslackchannelconfigurationresulttypedef) 


```python
# update_slack_channel_configuration method usage example with argument unpacking

kwargs: UpdateSlackChannelConfigurationRequestRequestTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
    "SlackChannelId": ...,
}

parent.update_slack_channel_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateSlackChannelConfigurationRequestRequestTypeDef](./type_defs.md#updateslackchannelconfigurationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("chatbot").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "ChatbotClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("chatbot").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("chatbot").get_paginator` method with overloads.

- `client.get_paginator("describe_chime_webhook_configurations")` -> [DescribeChimeWebhookConfigurationsPaginator](./paginators.md#describechimewebhookconfigurationspaginator)
- `client.get_paginator("describe_slack_channel_configurations")` -> [DescribeSlackChannelConfigurationsPaginator](./paginators.md#describeslackchannelconfigurationspaginator)
- `client.get_paginator("describe_slack_user_identities")` -> [DescribeSlackUserIdentitiesPaginator](./paginators.md#describeslackuseridentitiespaginator)
- `client.get_paginator("describe_slack_workspaces")` -> [DescribeSlackWorkspacesPaginator](./paginators.md#describeslackworkspacespaginator)
- `client.get_paginator("list_microsoft_teams_channel_configurations")` -> [ListMicrosoftTeamsChannelConfigurationsPaginator](./paginators.md#listmicrosoftteamschannelconfigurationspaginator)
- `client.get_paginator("list_microsoft_teams_configured_teams")` -> [ListMicrosoftTeamsConfiguredTeamsPaginator](./paginators.md#listmicrosoftteamsconfiguredteamspaginator)
- `client.get_paginator("list_microsoft_teams_user_identities")` -> [ListMicrosoftTeamsUserIdentitiesPaginator](./paginators.md#listmicrosoftteamsuseridentitiespaginator)



