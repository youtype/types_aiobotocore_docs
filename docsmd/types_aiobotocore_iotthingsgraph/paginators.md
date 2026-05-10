# Paginators

> [Index](../README.md) > [IoTThingsGraph](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoTThingsGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#iotthingsgraph)
    type annotations stubs module [types-aiobotocore-iotthingsgraph](https://pypi.org/project/types-aiobotocore-iotthingsgraph/).

## GetFlowTemplateRevisionsPaginator

Type annotations and code completion for `#!python session.create_client("iotthingsgraph").get_paginator("get_flow_template_revisions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph/paginator/GetFlowTemplateRevisions.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions)

```python
# GetFlowTemplateRevisionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import GetFlowTemplateRevisionsPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:  # (1)
    paginator: GetFlowTemplateRevisionsPaginator = client.get_paginator("get_flow_template_revisions")  # (2)
    async for item in paginator.paginate(...):
        item: GetFlowTemplateRevisionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [GetFlowTemplateRevisionsPaginator](./paginators.md#getflowtemplaterevisionspaginator)
3. item: `AioPageIterator[GetFlowTemplateRevisionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetFlowTemplateRevisionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    id: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetFlowTemplateRevisionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetFlowTemplateRevisionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetFlowTemplateRevisionsRequestPaginateTypeDef = {  # (1)
    "id": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetFlowTemplateRevisionsRequestPaginateTypeDef](./type_defs.md#getflowtemplaterevisionsrequestpaginatetypedef)
## GetSystemTemplateRevisionsPaginator

Type annotations and code completion for `#!python session.create_client("iotthingsgraph").get_paginator("get_system_template_revisions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph/paginator/GetSystemTemplateRevisions.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions)

```python
# GetSystemTemplateRevisionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import GetSystemTemplateRevisionsPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:  # (1)
    paginator: GetSystemTemplateRevisionsPaginator = client.get_paginator("get_system_template_revisions")  # (2)
    async for item in paginator.paginate(...):
        item: GetSystemTemplateRevisionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [GetSystemTemplateRevisionsPaginator](./paginators.md#getsystemtemplaterevisionspaginator)
3. item: `AioPageIterator[GetSystemTemplateRevisionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetSystemTemplateRevisionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    id: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetSystemTemplateRevisionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetSystemTemplateRevisionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetSystemTemplateRevisionsRequestPaginateTypeDef = {  # (1)
    "id": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSystemTemplateRevisionsRequestPaginateTypeDef](./type_defs.md#getsystemtemplaterevisionsrequestpaginatetypedef)
## ListFlowExecutionMessagesPaginator

Type annotations and code completion for `#!python session.create_client("iotthingsgraph").get_paginator("list_flow_execution_messages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph/paginator/ListFlowExecutionMessages.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages)

```python
# ListFlowExecutionMessagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import ListFlowExecutionMessagesPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:  # (1)
    paginator: ListFlowExecutionMessagesPaginator = client.get_paginator("list_flow_execution_messages")  # (2)
    async for item in paginator.paginate(...):
        item: ListFlowExecutionMessagesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [ListFlowExecutionMessagesPaginator](./paginators.md#listflowexecutionmessagespaginator)
3. item: `AioPageIterator[ListFlowExecutionMessagesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFlowExecutionMessagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    flowExecutionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFlowExecutionMessagesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFlowExecutionMessagesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFlowExecutionMessagesRequestPaginateTypeDef = {  # (1)
    "flowExecutionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowExecutionMessagesRequestPaginateTypeDef](./type_defs.md#listflowexecutionmessagesrequestpaginatetypedef)
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("iotthingsgraph").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph/paginator/ListTagsForResource.html#IoTThingsGraph.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: `AioPageIterator[ListTagsForResourceResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTagsForResourceResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestPaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef)
## SearchEntitiesPaginator

Type annotations and code completion for `#!python session.create_client("iotthingsgraph").get_paginator("search_entities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph/paginator/SearchEntities.html#IoTThingsGraph.Paginator.SearchEntities)

```python
# SearchEntitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import SearchEntitiesPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:  # (1)
    paginator: SearchEntitiesPaginator = client.get_paginator("search_entities")  # (2)
    async for item in paginator.paginate(...):
        item: SearchEntitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [SearchEntitiesPaginator](./paginators.md#searchentitiespaginator)
3. item: `AioPageIterator[SearchEntitiesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchEntitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    entityTypes: Sequence[EntityTypeType],  # (1)
    filters: Sequence[EntityFilterTypeDef] = ...,  # (2)
    namespaceVersion: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchEntitiesResponseTypeDef]:  # (4)
    ...
```

1. See `Sequence[EntityTypeType]`
2. See `Sequence[EntityFilterTypeDef]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchEntitiesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchEntitiesRequestPaginateTypeDef = {  # (1)
    "entityTypes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchEntitiesRequestPaginateTypeDef](./type_defs.md#searchentitiesrequestpaginatetypedef)
## SearchFlowExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("iotthingsgraph").get_paginator("search_flow_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph/paginator/SearchFlowExecutions.html#IoTThingsGraph.Paginator.SearchFlowExecutions)

```python
# SearchFlowExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import SearchFlowExecutionsPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:  # (1)
    paginator: SearchFlowExecutionsPaginator = client.get_paginator("search_flow_executions")  # (2)
    async for item in paginator.paginate(...):
        item: SearchFlowExecutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [SearchFlowExecutionsPaginator](./paginators.md#searchflowexecutionspaginator)
3. item: `AioPageIterator[SearchFlowExecutionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchFlowExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    systemInstanceId: str,
    flowExecutionId: str = ...,
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[SearchFlowExecutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[SearchFlowExecutionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchFlowExecutionsRequestPaginateTypeDef = {  # (1)
    "systemInstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchFlowExecutionsRequestPaginateTypeDef](./type_defs.md#searchflowexecutionsrequestpaginatetypedef)
## SearchFlowTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("iotthingsgraph").get_paginator("search_flow_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph/paginator/SearchFlowTemplates.html#IoTThingsGraph.Paginator.SearchFlowTemplates)

```python
# SearchFlowTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import SearchFlowTemplatesPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:  # (1)
    paginator: SearchFlowTemplatesPaginator = client.get_paginator("search_flow_templates")  # (2)
    async for item in paginator.paginate(...):
        item: SearchFlowTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [SearchFlowTemplatesPaginator](./paginators.md#searchflowtemplatespaginator)
3. item: `AioPageIterator[SearchFlowTemplatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchFlowTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[FlowTemplateFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchFlowTemplatesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[FlowTemplateFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchFlowTemplatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchFlowTemplatesRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchFlowTemplatesRequestPaginateTypeDef](./type_defs.md#searchflowtemplatesrequestpaginatetypedef)
## SearchSystemInstancesPaginator

Type annotations and code completion for `#!python session.create_client("iotthingsgraph").get_paginator("search_system_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph/paginator/SearchSystemInstances.html#IoTThingsGraph.Paginator.SearchSystemInstances)

```python
# SearchSystemInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import SearchSystemInstancesPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:  # (1)
    paginator: SearchSystemInstancesPaginator = client.get_paginator("search_system_instances")  # (2)
    async for item in paginator.paginate(...):
        item: SearchSystemInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [SearchSystemInstancesPaginator](./paginators.md#searchsysteminstancespaginator)
3. item: `AioPageIterator[SearchSystemInstancesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchSystemInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[SystemInstanceFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchSystemInstancesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[SystemInstanceFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchSystemInstancesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchSystemInstancesRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchSystemInstancesRequestPaginateTypeDef](./type_defs.md#searchsysteminstancesrequestpaginatetypedef)
## SearchSystemTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("iotthingsgraph").get_paginator("search_system_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph/paginator/SearchSystemTemplates.html#IoTThingsGraph.Paginator.SearchSystemTemplates)

```python
# SearchSystemTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import SearchSystemTemplatesPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:  # (1)
    paginator: SearchSystemTemplatesPaginator = client.get_paginator("search_system_templates")  # (2)
    async for item in paginator.paginate(...):
        item: SearchSystemTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [SearchSystemTemplatesPaginator](./paginators.md#searchsystemtemplatespaginator)
3. item: `AioPageIterator[SearchSystemTemplatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchSystemTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[SystemTemplateFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchSystemTemplatesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[SystemTemplateFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchSystemTemplatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchSystemTemplatesRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchSystemTemplatesRequestPaginateTypeDef](./type_defs.md#searchsystemtemplatesrequestpaginatetypedef)
## SearchThingsPaginator

Type annotations and code completion for `#!python session.create_client("iotthingsgraph").get_paginator("search_things")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph/paginator/SearchThings.html#IoTThingsGraph.Paginator.SearchThings)

```python
# SearchThingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import SearchThingsPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:  # (1)
    paginator: SearchThingsPaginator = client.get_paginator("search_things")  # (2)
    async for item in paginator.paginate(...):
        item: SearchThingsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [SearchThingsPaginator](./paginators.md#searchthingspaginator)
3. item: `AioPageIterator[SearchThingsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchThingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    entityId: str,
    namespaceVersion: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[SearchThingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[SearchThingsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchThingsRequestPaginateTypeDef = {  # (1)
    "entityId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchThingsRequestPaginateTypeDef](./type_defs.md#searchthingsrequestpaginatetypedef)
