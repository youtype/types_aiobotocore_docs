# Paginators

> [Index](../README.md) > [Chatbot](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Chatbot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot)
    type annotations stubs module [types-aiobotocore-chatbot](https://pypi.org/project/types-aiobotocore-chatbot/).

## DescribeChimeWebhookConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("chatbot").get_paginator("describe_chime_webhook_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot/paginator/DescribeChimeWebhookConfigurations.html#Chatbot.Paginator.DescribeChimeWebhookConfigurations)

```python
# DescribeChimeWebhookConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_chatbot.paginator import DescribeChimeWebhookConfigurationsPaginator

session = get_session()
async with session.create_client("chatbot") as client:  # (1)
    paginator: DescribeChimeWebhookConfigurationsPaginator = client.get_paginator("describe_chime_webhook_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeChimeWebhookConfigurationsResultTypeDef
        print(item)  # (3)
```

1. client: [ChatbotClient](./client.md)
2. paginator: [DescribeChimeWebhookConfigurationsPaginator](./paginators.md#describechimewebhookconfigurationspaginator)
3. item: [:material-code-braces: DescribeChimeWebhookConfigurationsResultTypeDef](./type_defs.md#describechimewebhookconfigurationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeChimeWebhookConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChatConfigurationArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeChimeWebhookConfigurationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeChimeWebhookConfigurationsResultTypeDef](./type_defs.md#describechimewebhookconfigurationsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeChimeWebhookConfigurationsRequestPaginateTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeChimeWebhookConfigurationsRequestPaginateTypeDef](./type_defs.md#describechimewebhookconfigurationsrequestpaginatetypedef) 
## DescribeSlackChannelConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("chatbot").get_paginator("describe_slack_channel_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot/paginator/DescribeSlackChannelConfigurations.html#Chatbot.Paginator.DescribeSlackChannelConfigurations)

```python
# DescribeSlackChannelConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_chatbot.paginator import DescribeSlackChannelConfigurationsPaginator

session = get_session()
async with session.create_client("chatbot") as client:  # (1)
    paginator: DescribeSlackChannelConfigurationsPaginator = client.get_paginator("describe_slack_channel_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSlackChannelConfigurationsResultTypeDef
        print(item)  # (3)
```

1. client: [ChatbotClient](./client.md)
2. paginator: [DescribeSlackChannelConfigurationsPaginator](./paginators.md#describeslackchannelconfigurationspaginator)
3. item: [:material-code-braces: DescribeSlackChannelConfigurationsResultTypeDef](./type_defs.md#describeslackchannelconfigurationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSlackChannelConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChatConfigurationArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeSlackChannelConfigurationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSlackChannelConfigurationsResultTypeDef](./type_defs.md#describeslackchannelconfigurationsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSlackChannelConfigurationsRequestPaginateTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSlackChannelConfigurationsRequestPaginateTypeDef](./type_defs.md#describeslackchannelconfigurationsrequestpaginatetypedef) 
## DescribeSlackUserIdentitiesPaginator

Type annotations and code completion for `#!python session.create_client("chatbot").get_paginator("describe_slack_user_identities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot/paginator/DescribeSlackUserIdentities.html#Chatbot.Paginator.DescribeSlackUserIdentities)

```python
# DescribeSlackUserIdentitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_chatbot.paginator import DescribeSlackUserIdentitiesPaginator

session = get_session()
async with session.create_client("chatbot") as client:  # (1)
    paginator: DescribeSlackUserIdentitiesPaginator = client.get_paginator("describe_slack_user_identities")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSlackUserIdentitiesResultTypeDef
        print(item)  # (3)
```

1. client: [ChatbotClient](./client.md)
2. paginator: [DescribeSlackUserIdentitiesPaginator](./paginators.md#describeslackuseridentitiespaginator)
3. item: [:material-code-braces: DescribeSlackUserIdentitiesResultTypeDef](./type_defs.md#describeslackuseridentitiesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSlackUserIdentitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChatConfigurationArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeSlackUserIdentitiesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSlackUserIdentitiesResultTypeDef](./type_defs.md#describeslackuseridentitiesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSlackUserIdentitiesRequestPaginateTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSlackUserIdentitiesRequestPaginateTypeDef](./type_defs.md#describeslackuseridentitiesrequestpaginatetypedef) 
## DescribeSlackWorkspacesPaginator

Type annotations and code completion for `#!python session.create_client("chatbot").get_paginator("describe_slack_workspaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot/paginator/DescribeSlackWorkspaces.html#Chatbot.Paginator.DescribeSlackWorkspaces)

```python
# DescribeSlackWorkspacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_chatbot.paginator import DescribeSlackWorkspacesPaginator

session = get_session()
async with session.create_client("chatbot") as client:  # (1)
    paginator: DescribeSlackWorkspacesPaginator = client.get_paginator("describe_slack_workspaces")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSlackWorkspacesResultTypeDef
        print(item)  # (3)
```

1. client: [ChatbotClient](./client.md)
2. paginator: [DescribeSlackWorkspacesPaginator](./paginators.md#describeslackworkspacespaginator)
3. item: [:material-code-braces: DescribeSlackWorkspacesResultTypeDef](./type_defs.md#describeslackworkspacesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSlackWorkspacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeSlackWorkspacesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSlackWorkspacesResultTypeDef](./type_defs.md#describeslackworkspacesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSlackWorkspacesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSlackWorkspacesRequestPaginateTypeDef](./type_defs.md#describeslackworkspacesrequestpaginatetypedef) 
## ListAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("chatbot").get_paginator("list_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot/paginator/ListAssociations.html#Chatbot.Paginator.ListAssociations)

```python
# ListAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_chatbot.paginator import ListAssociationsPaginator

session = get_session()
async with session.create_client("chatbot") as client:  # (1)
    paginator: ListAssociationsPaginator = client.get_paginator("list_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [ChatbotClient](./client.md)
2. paginator: [ListAssociationsPaginator](./paginators.md#listassociationspaginator)
3. item: [:material-code-braces: ListAssociationsResultTypeDef](./type_defs.md#listassociationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChatConfiguration: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAssociationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssociationsResultTypeDef](./type_defs.md#listassociationsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssociationsRequestPaginateTypeDef = {  # (1)
    "ChatConfiguration": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociationsRequestPaginateTypeDef](./type_defs.md#listassociationsrequestpaginatetypedef) 
## ListCustomActionsPaginator

Type annotations and code completion for `#!python session.create_client("chatbot").get_paginator("list_custom_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot/paginator/ListCustomActions.html#Chatbot.Paginator.ListCustomActions)

```python
# ListCustomActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_chatbot.paginator import ListCustomActionsPaginator

session = get_session()
async with session.create_client("chatbot") as client:  # (1)
    paginator: ListCustomActionsPaginator = client.get_paginator("list_custom_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomActionsResultTypeDef
        print(item)  # (3)
```

1. client: [ChatbotClient](./client.md)
2. paginator: [ListCustomActionsPaginator](./paginators.md#listcustomactionspaginator)
3. item: [:material-code-braces: ListCustomActionsResultTypeDef](./type_defs.md#listcustomactionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCustomActionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomActionsResultTypeDef](./type_defs.md#listcustomactionsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomActionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomActionsRequestPaginateTypeDef](./type_defs.md#listcustomactionsrequestpaginatetypedef) 
## ListMicrosoftTeamsChannelConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("chatbot").get_paginator("list_microsoft_teams_channel_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot/paginator/ListMicrosoftTeamsChannelConfigurations.html#Chatbot.Paginator.ListMicrosoftTeamsChannelConfigurations)

```python
# ListMicrosoftTeamsChannelConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_chatbot.paginator import ListMicrosoftTeamsChannelConfigurationsPaginator

session = get_session()
async with session.create_client("chatbot") as client:  # (1)
    paginator: ListMicrosoftTeamsChannelConfigurationsPaginator = client.get_paginator("list_microsoft_teams_channel_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListTeamsChannelConfigurationsResultTypeDef
        print(item)  # (3)
```

1. client: [ChatbotClient](./client.md)
2. paginator: [ListMicrosoftTeamsChannelConfigurationsPaginator](./paginators.md#listmicrosoftteamschannelconfigurationspaginator)
3. item: [:material-code-braces: ListTeamsChannelConfigurationsResultTypeDef](./type_defs.md#listteamschannelconfigurationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListMicrosoftTeamsChannelConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TeamId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTeamsChannelConfigurationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTeamsChannelConfigurationsResultTypeDef](./type_defs.md#listteamschannelconfigurationsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTeamsChannelConfigurationsRequestPaginateTypeDef = {  # (1)
    "TeamId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTeamsChannelConfigurationsRequestPaginateTypeDef](./type_defs.md#listteamschannelconfigurationsrequestpaginatetypedef) 
## ListMicrosoftTeamsConfiguredTeamsPaginator

Type annotations and code completion for `#!python session.create_client("chatbot").get_paginator("list_microsoft_teams_configured_teams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot/paginator/ListMicrosoftTeamsConfiguredTeams.html#Chatbot.Paginator.ListMicrosoftTeamsConfiguredTeams)

```python
# ListMicrosoftTeamsConfiguredTeamsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_chatbot.paginator import ListMicrosoftTeamsConfiguredTeamsPaginator

session = get_session()
async with session.create_client("chatbot") as client:  # (1)
    paginator: ListMicrosoftTeamsConfiguredTeamsPaginator = client.get_paginator("list_microsoft_teams_configured_teams")  # (2)
    async for item in paginator.paginate(...):
        item: ListMicrosoftTeamsConfiguredTeamsResultTypeDef
        print(item)  # (3)
```

1. client: [ChatbotClient](./client.md)
2. paginator: [ListMicrosoftTeamsConfiguredTeamsPaginator](./paginators.md#listmicrosoftteamsconfiguredteamspaginator)
3. item: [:material-code-braces: ListMicrosoftTeamsConfiguredTeamsResultTypeDef](./type_defs.md#listmicrosoftteamsconfiguredteamsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListMicrosoftTeamsConfiguredTeamsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMicrosoftTeamsConfiguredTeamsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMicrosoftTeamsConfiguredTeamsResultTypeDef](./type_defs.md#listmicrosoftteamsconfiguredteamsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMicrosoftTeamsConfiguredTeamsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMicrosoftTeamsConfiguredTeamsRequestPaginateTypeDef](./type_defs.md#listmicrosoftteamsconfiguredteamsrequestpaginatetypedef) 
## ListMicrosoftTeamsUserIdentitiesPaginator

Type annotations and code completion for `#!python session.create_client("chatbot").get_paginator("list_microsoft_teams_user_identities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot/paginator/ListMicrosoftTeamsUserIdentities.html#Chatbot.Paginator.ListMicrosoftTeamsUserIdentities)

```python
# ListMicrosoftTeamsUserIdentitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_chatbot.paginator import ListMicrosoftTeamsUserIdentitiesPaginator

session = get_session()
async with session.create_client("chatbot") as client:  # (1)
    paginator: ListMicrosoftTeamsUserIdentitiesPaginator = client.get_paginator("list_microsoft_teams_user_identities")  # (2)
    async for item in paginator.paginate(...):
        item: ListMicrosoftTeamsUserIdentitiesResultTypeDef
        print(item)  # (3)
```

1. client: [ChatbotClient](./client.md)
2. paginator: [ListMicrosoftTeamsUserIdentitiesPaginator](./paginators.md#listmicrosoftteamsuseridentitiespaginator)
3. item: [:material-code-braces: ListMicrosoftTeamsUserIdentitiesResultTypeDef](./type_defs.md#listmicrosoftteamsuseridentitiesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListMicrosoftTeamsUserIdentitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChatConfigurationArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMicrosoftTeamsUserIdentitiesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMicrosoftTeamsUserIdentitiesResultTypeDef](./type_defs.md#listmicrosoftteamsuseridentitiesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMicrosoftTeamsUserIdentitiesRequestPaginateTypeDef = {  # (1)
    "ChatConfigurationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMicrosoftTeamsUserIdentitiesRequestPaginateTypeDef](./type_defs.md#listmicrosoftteamsuseridentitiesrequestpaginatetypedef) 
