# Paginators

> [Index](../README.md) > [QBusiness](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [QBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#qbusiness)
    type annotations stubs module [types-aiobotocore-qbusiness](https://pypi.org/project/types-aiobotocore-qbusiness/).

## GetChatControlsConfigurationPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("get_chat_controls_configuration")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/GetChatControlsConfiguration.html#QBusiness.Paginator.GetChatControlsConfiguration)

```python
# GetChatControlsConfigurationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import GetChatControlsConfigurationPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: GetChatControlsConfigurationPaginator = client.get_paginator("get_chat_controls_configuration")  # (2)
    async for item in paginator.paginate(...):
        item: GetChatControlsConfigurationResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [GetChatControlsConfigurationPaginator](./paginators.md#getchatcontrolsconfigurationpaginator)
3. item: [:material-code-braces: GetChatControlsConfigurationResponseTypeDef](./type_defs.md#getchatcontrolsconfigurationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetChatControlsConfigurationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetChatControlsConfigurationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetChatControlsConfigurationResponseTypeDef](./type_defs.md#getchatcontrolsconfigurationresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetChatControlsConfigurationRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetChatControlsConfigurationRequestPaginateTypeDef](./type_defs.md#getchatcontrolsconfigurationrequestpaginatetypedef) 
## ListApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListApplications.html#QBusiness.Paginator.ListApplications)

```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListApplicationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestPaginateTypeDef](./type_defs.md#listapplicationsrequestpaginatetypedef) 
## ListAttachmentsPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_attachments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListAttachments.html#QBusiness.Paginator.ListAttachments)

```python
# ListAttachmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListAttachmentsPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListAttachmentsPaginator = client.get_paginator("list_attachments")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttachmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListAttachmentsPaginator](./paginators.md#listattachmentspaginator)
3. item: [:material-code-braces: ListAttachmentsResponseTypeDef](./type_defs.md#listattachmentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAttachmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    conversationId: str = ...,
    userId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAttachmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAttachmentsResponseTypeDef](./type_defs.md#listattachmentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAttachmentsRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttachmentsRequestPaginateTypeDef](./type_defs.md#listattachmentsrequestpaginatetypedef) 
## ListConversationsPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_conversations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListConversations.html#QBusiness.Paginator.ListConversations)

```python
# ListConversationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListConversationsPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListConversationsPaginator = client.get_paginator("list_conversations")  # (2)
    async for item in paginator.paginate(...):
        item: ListConversationsResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListConversationsPaginator](./paginators.md#listconversationspaginator)
3. item: [:material-code-braces: ListConversationsResponseTypeDef](./type_defs.md#listconversationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConversationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    userId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConversationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConversationsResponseTypeDef](./type_defs.md#listconversationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConversationsRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConversationsRequestPaginateTypeDef](./type_defs.md#listconversationsrequestpaginatetypedef) 
## ListDataAccessorsPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_data_accessors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListDataAccessors.html#QBusiness.Paginator.ListDataAccessors)

```python
# ListDataAccessorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListDataAccessorsPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListDataAccessorsPaginator = client.get_paginator("list_data_accessors")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataAccessorsResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListDataAccessorsPaginator](./paginators.md#listdataaccessorspaginator)
3. item: [:material-code-braces: ListDataAccessorsResponseTypeDef](./type_defs.md#listdataaccessorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataAccessorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDataAccessorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataAccessorsResponseTypeDef](./type_defs.md#listdataaccessorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataAccessorsRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataAccessorsRequestPaginateTypeDef](./type_defs.md#listdataaccessorsrequestpaginatetypedef) 
## ListDataSourceSyncJobsPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_data_source_sync_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListDataSourceSyncJobs.html#QBusiness.Paginator.ListDataSourceSyncJobs)

```python
# ListDataSourceSyncJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListDataSourceSyncJobsPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListDataSourceSyncJobsPaginator = client.get_paginator("list_data_source_sync_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSourceSyncJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListDataSourceSyncJobsPaginator](./paginators.md#listdatasourcesyncjobspaginator)
3. item: [:material-code-braces: ListDataSourceSyncJobsResponseTypeDef](./type_defs.md#listdatasourcesyncjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataSourceSyncJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    dataSourceId: str,
    applicationId: str,
    indexId: str,
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
    statusFilter: DataSourceSyncJobStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDataSourceSyncJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DataSourceSyncJobStatusType](./literals.md#datasourcesyncjobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDataSourceSyncJobsResponseTypeDef](./type_defs.md#listdatasourcesyncjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSourceSyncJobsRequestPaginateTypeDef = {  # (1)
    "dataSourceId": ...,
    "applicationId": ...,
    "indexId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSourceSyncJobsRequestPaginateTypeDef](./type_defs.md#listdatasourcesyncjobsrequestpaginatetypedef) 
## ListDataSourcesPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_data_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListDataSources.html#QBusiness.Paginator.ListDataSources)

```python
# ListDataSourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListDataSourcesPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListDataSourcesPaginator = client.get_paginator("list_data_sources")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
3. item: [:material-code-braces: ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataSourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    indexId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDataSourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSourcesRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesRequestPaginateTypeDef](./type_defs.md#listdatasourcesrequestpaginatetypedef) 
## ListDocumentsPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_documents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListDocuments.html#QBusiness.Paginator.ListDocuments)

```python
# ListDocumentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListDocumentsPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListDocumentsPaginator = client.get_paginator("list_documents")  # (2)
    async for item in paginator.paginate(...):
        item: ListDocumentsResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListDocumentsPaginator](./paginators.md#listdocumentspaginator)
3. item: [:material-code-braces: ListDocumentsResponseTypeDef](./type_defs.md#listdocumentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDocumentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    indexId: str,
    dataSourceIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDocumentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDocumentsResponseTypeDef](./type_defs.md#listdocumentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDocumentsRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDocumentsRequestPaginateTypeDef](./type_defs.md#listdocumentsrequestpaginatetypedef) 
## ListGroupsPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListGroups.html#QBusiness.Paginator.ListGroups)

```python
# ListGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListGroupsPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListGroupsPaginator](./paginators.md#listgroupspaginator)
3. item: [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    indexId: str,
    updatedEarlierThan: TimestampTypeDef,
    dataSourceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupsRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
    "updatedEarlierThan": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestPaginateTypeDef](./type_defs.md#listgroupsrequestpaginatetypedef) 
## ListIndicesPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_indices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListIndices.html#QBusiness.Paginator.ListIndices)

```python
# ListIndicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListIndicesPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListIndicesPaginator = client.get_paginator("list_indices")  # (2)
    async for item in paginator.paginate(...):
        item: ListIndicesResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListIndicesPaginator](./paginators.md#listindicespaginator)
3. item: [:material-code-braces: ListIndicesResponseTypeDef](./type_defs.md#listindicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIndicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListIndicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIndicesResponseTypeDef](./type_defs.md#listindicesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIndicesRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIndicesRequestPaginateTypeDef](./type_defs.md#listindicesrequestpaginatetypedef) 
## ListMessagesPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_messages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListMessages.html#QBusiness.Paginator.ListMessages)

```python
# ListMessagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListMessagesPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListMessagesPaginator = client.get_paginator("list_messages")  # (2)
    async for item in paginator.paginate(...):
        item: ListMessagesResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListMessagesPaginator](./paginators.md#listmessagespaginator)
3. item: [:material-code-braces: ListMessagesResponseTypeDef](./type_defs.md#listmessagesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMessagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    conversationId: str,
    applicationId: str,
    userId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMessagesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMessagesResponseTypeDef](./type_defs.md#listmessagesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMessagesRequestPaginateTypeDef = {  # (1)
    "conversationId": ...,
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMessagesRequestPaginateTypeDef](./type_defs.md#listmessagesrequestpaginatetypedef) 
## ListPluginActionsPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_plugin_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListPluginActions.html#QBusiness.Paginator.ListPluginActions)

```python
# ListPluginActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListPluginActionsPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListPluginActionsPaginator = client.get_paginator("list_plugin_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPluginActionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListPluginActionsPaginator](./paginators.md#listpluginactionspaginator)
3. item: [:material-code-braces: ListPluginActionsResponseTypeDef](./type_defs.md#listpluginactionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPluginActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    pluginId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPluginActionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPluginActionsResponseTypeDef](./type_defs.md#listpluginactionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPluginActionsRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
    "pluginId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPluginActionsRequestPaginateTypeDef](./type_defs.md#listpluginactionsrequestpaginatetypedef) 
## ListPluginTypeActionsPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_plugin_type_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListPluginTypeActions.html#QBusiness.Paginator.ListPluginTypeActions)

```python
# ListPluginTypeActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListPluginTypeActionsPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListPluginTypeActionsPaginator = client.get_paginator("list_plugin_type_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPluginTypeActionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListPluginTypeActionsPaginator](./paginators.md#listplugintypeactionspaginator)
3. item: [:material-code-braces: ListPluginTypeActionsResponseTypeDef](./type_defs.md#listplugintypeactionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPluginTypeActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    pluginType: PluginTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListPluginTypeActionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PluginTypeType](./literals.md#plugintypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPluginTypeActionsResponseTypeDef](./type_defs.md#listplugintypeactionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPluginTypeActionsRequestPaginateTypeDef = {  # (1)
    "pluginType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPluginTypeActionsRequestPaginateTypeDef](./type_defs.md#listplugintypeactionsrequestpaginatetypedef) 
## ListPluginTypeMetadataPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_plugin_type_metadata")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListPluginTypeMetadata.html#QBusiness.Paginator.ListPluginTypeMetadata)

```python
# ListPluginTypeMetadataPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListPluginTypeMetadataPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListPluginTypeMetadataPaginator = client.get_paginator("list_plugin_type_metadata")  # (2)
    async for item in paginator.paginate(...):
        item: ListPluginTypeMetadataResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListPluginTypeMetadataPaginator](./paginators.md#listplugintypemetadatapaginator)
3. item: [:material-code-braces: ListPluginTypeMetadataResponseTypeDef](./type_defs.md#listplugintypemetadataresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPluginTypeMetadataPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPluginTypeMetadataResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPluginTypeMetadataResponseTypeDef](./type_defs.md#listplugintypemetadataresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPluginTypeMetadataRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPluginTypeMetadataRequestPaginateTypeDef](./type_defs.md#listplugintypemetadatarequestpaginatetypedef) 
## ListPluginsPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_plugins")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListPlugins.html#QBusiness.Paginator.ListPlugins)

```python
# ListPluginsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListPluginsPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListPluginsPaginator = client.get_paginator("list_plugins")  # (2)
    async for item in paginator.paginate(...):
        item: ListPluginsResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListPluginsPaginator](./paginators.md#listpluginspaginator)
3. item: [:material-code-braces: ListPluginsResponseTypeDef](./type_defs.md#listpluginsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPluginsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPluginsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPluginsResponseTypeDef](./type_defs.md#listpluginsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPluginsRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPluginsRequestPaginateTypeDef](./type_defs.md#listpluginsrequestpaginatetypedef) 
## ListRetrieversPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_retrievers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListRetrievers.html#QBusiness.Paginator.ListRetrievers)

```python
# ListRetrieversPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListRetrieversPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListRetrieversPaginator = client.get_paginator("list_retrievers")  # (2)
    async for item in paginator.paginate(...):
        item: ListRetrieversResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListRetrieversPaginator](./paginators.md#listretrieverspaginator)
3. item: [:material-code-braces: ListRetrieversResponseTypeDef](./type_defs.md#listretrieversresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRetrieversPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRetrieversResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRetrieversResponseTypeDef](./type_defs.md#listretrieversresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRetrieversRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRetrieversRequestPaginateTypeDef](./type_defs.md#listretrieversrequestpaginatetypedef) 
## ListSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListSubscriptions.html#QBusiness.Paginator.ListSubscriptions)

```python
# ListSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListSubscriptionsPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListSubscriptionsPaginator](./paginators.md#listsubscriptionspaginator)
3. item: [:material-code-braces: ListSubscriptionsResponseTypeDef](./type_defs.md#listsubscriptionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSubscriptionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubscriptionsResponseTypeDef](./type_defs.md#listsubscriptionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSubscriptionsRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionsRequestPaginateTypeDef](./type_defs.md#listsubscriptionsrequestpaginatetypedef) 
## ListWebExperiencesPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("list_web_experiences")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/ListWebExperiences.html#QBusiness.Paginator.ListWebExperiences)

```python
# ListWebExperiencesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import ListWebExperiencesPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: ListWebExperiencesPaginator = client.get_paginator("list_web_experiences")  # (2)
    async for item in paginator.paginate(...):
        item: ListWebExperiencesResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [ListWebExperiencesPaginator](./paginators.md#listwebexperiencespaginator)
3. item: [:material-code-braces: ListWebExperiencesResponseTypeDef](./type_defs.md#listwebexperiencesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWebExperiencesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWebExperiencesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWebExperiencesResponseTypeDef](./type_defs.md#listwebexperiencesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWebExperiencesRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWebExperiencesRequestPaginateTypeDef](./type_defs.md#listwebexperiencesrequestpaginatetypedef) 
## SearchRelevantContentPaginator

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator("search_relevant_content")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/paginator/SearchRelevantContent.html#QBusiness.Paginator.SearchRelevantContent)

```python
# SearchRelevantContentPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.paginator import SearchRelevantContentPaginator

session = get_session()
async with session.create_client("qbusiness") as client:  # (1)
    paginator: SearchRelevantContentPaginator = client.get_paginator("search_relevant_content")  # (2)
    async for item in paginator.paginate(...):
        item: SearchRelevantContentResponseTypeDef
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [SearchRelevantContentPaginator](./paginators.md#searchrelevantcontentpaginator)
3. item: [:material-code-braces: SearchRelevantContentResponseTypeDef](./type_defs.md#searchrelevantcontentresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchRelevantContentPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    queryText: str,
    contentSource: ContentSourceTypeDef,  # (1)
    attributeFilter: AttributeFilterPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[SearchRelevantContentResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ContentSourceTypeDef](./type_defs.md#contentsourcetypedef) 
2. See [:material-code-braces: AttributeFilterPaginatorTypeDef](./type_defs.md#attributefilterpaginatortypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: SearchRelevantContentResponseTypeDef](./type_defs.md#searchrelevantcontentresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchRelevantContentRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
    "queryText": ...,
    "contentSource": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchRelevantContentRequestPaginateTypeDef](./type_defs.md#searchrelevantcontentrequestpaginatetypedef) 
