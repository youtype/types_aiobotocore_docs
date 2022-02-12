<a id="paginators-for-aiobotocore-iotthingsgraph-module"></a>

# Paginators for aiobotocore IoTThingsGraph module

> [Index](..) > [IoTThingsGraph](.) > Paginators

Auto-generated documentation for
[IoTThingsGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
type annotations stubs module
[types-aiobotocore-iotthingsgraph](https://pypi.org/project/types-aiobotocore-iotthingsgraph/).

- [Paginators for aiobotocore IoTThingsGraph module](#paginators-for-aiobotocore-iotthingsgraph-module)
  - [GetFlowTemplateRevisionsPaginator](#getflowtemplaterevisionspaginator)
  - [GetSystemTemplateRevisionsPaginator](#getsystemtemplaterevisionspaginator)
  - [ListFlowExecutionMessagesPaginator](#listflowexecutionmessagespaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)
  - [SearchEntitiesPaginator](#searchentitiespaginator)
  - [SearchFlowExecutionsPaginator](#searchflowexecutionspaginator)
  - [SearchFlowTemplatesPaginator](#searchflowtemplatespaginator)
  - [SearchSystemInstancesPaginator](#searchsysteminstancespaginator)
  - [SearchSystemTemplatesPaginator](#searchsystemtemplatespaginator)
  - [SearchThingsPaginator](#searchthingspaginator)

<a id="getflowtemplaterevisionspaginator"></a>

## GetFlowTemplateRevisionsPaginator

Type annotations for
`session.create_client("iotthingsgraph").get_paginator("get_flow_template_revisions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import GetFlowTemplateRevisionsPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:
    client: IoTThingsGraphClient
    paginator: GetFlowTemplateRevisionsPaginator = client.get_paginator("get_flow_template_revisions")
```

Boto3 documentation:
[IoTThingsGraph.Paginator.GetFlowTemplateRevisions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions)

Arguments for `GetFlowTemplateRevisionsPaginator.paginate` method:

- `id`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetFlowTemplateRevisionsPaginator.paginate` returns
`AsyncIterable`\[[GetFlowTemplateRevisionsResponseTypeDef](./type_defs.md#getflowtemplaterevisionsresponsetypedef)\].

<a id="getsystemtemplaterevisionspaginator"></a>

## GetSystemTemplateRevisionsPaginator

Type annotations for
`session.create_client("iotthingsgraph").get_paginator("get_system_template_revisions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import GetSystemTemplateRevisionsPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:
    client: IoTThingsGraphClient
    paginator: GetSystemTemplateRevisionsPaginator = client.get_paginator("get_system_template_revisions")
```

Boto3 documentation:
[IoTThingsGraph.Paginator.GetSystemTemplateRevisions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions)

Arguments for `GetSystemTemplateRevisionsPaginator.paginate` method:

- `id`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetSystemTemplateRevisionsPaginator.paginate` returns
`AsyncIterable`\[[GetSystemTemplateRevisionsResponseTypeDef](./type_defs.md#getsystemtemplaterevisionsresponsetypedef)\].

<a id="listflowexecutionmessagespaginator"></a>

## ListFlowExecutionMessagesPaginator

Type annotations for
`session.create_client("iotthingsgraph").get_paginator("list_flow_execution_messages")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import ListFlowExecutionMessagesPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:
    client: IoTThingsGraphClient
    paginator: ListFlowExecutionMessagesPaginator = client.get_paginator("list_flow_execution_messages")
```

Boto3 documentation:
[IoTThingsGraph.Paginator.ListFlowExecutionMessages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages)

Arguments for `ListFlowExecutionMessagesPaginator.paginate` method:

- `flowExecutionId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFlowExecutionMessagesPaginator.paginate` returns
`AsyncIterable`\[[ListFlowExecutionMessagesResponseTypeDef](./type_defs.md#listflowexecutionmessagesresponsetypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("iotthingsgraph").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:
    client: IoTThingsGraphClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[IoTThingsGraph.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `resourceArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`AsyncIterable`\[[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)\].

<a id="searchentitiespaginator"></a>

## SearchEntitiesPaginator

Type annotations for
`session.create_client("iotthingsgraph").get_paginator("search_entities")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import SearchEntitiesPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:
    client: IoTThingsGraphClient
    paginator: SearchEntitiesPaginator = client.get_paginator("search_entities")
```

Boto3 documentation:
[IoTThingsGraph.Paginator.SearchEntities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchEntities)

Arguments for `SearchEntitiesPaginator.paginate` method:

- `entityTypes`: `Sequence`\[[EntityTypeType](./literals.md#entitytypetype)\]
  *(required)*
- `filters`:
  `Sequence`\[[EntityFilterTypeDef](./type_defs.md#entityfiltertypedef)\]
- `namespaceVersion`: `int`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchEntitiesPaginator.paginate` returns
`AsyncIterable`\[[SearchEntitiesResponseTypeDef](./type_defs.md#searchentitiesresponsetypedef)\].

<a id="searchflowexecutionspaginator"></a>

## SearchFlowExecutionsPaginator

Type annotations for
`session.create_client("iotthingsgraph").get_paginator("search_flow_executions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import SearchFlowExecutionsPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:
    client: IoTThingsGraphClient
    paginator: SearchFlowExecutionsPaginator = client.get_paginator("search_flow_executions")
```

Boto3 documentation:
[IoTThingsGraph.Paginator.SearchFlowExecutions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowExecutions)

Arguments for `SearchFlowExecutionsPaginator.paginate` method:

- `systemInstanceId`: `str` *(required)*
- `flowExecutionId`: `str`
- `startTime`: `Union`\[`datetime`, `str`\]
- `endTime`: `Union`\[`datetime`, `str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchFlowExecutionsPaginator.paginate` returns
`AsyncIterable`\[[SearchFlowExecutionsResponseTypeDef](./type_defs.md#searchflowexecutionsresponsetypedef)\].

<a id="searchflowtemplatespaginator"></a>

## SearchFlowTemplatesPaginator

Type annotations for
`session.create_client("iotthingsgraph").get_paginator("search_flow_templates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import SearchFlowTemplatesPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:
    client: IoTThingsGraphClient
    paginator: SearchFlowTemplatesPaginator = client.get_paginator("search_flow_templates")
```

Boto3 documentation:
[IoTThingsGraph.Paginator.SearchFlowTemplates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowTemplates)

Arguments for `SearchFlowTemplatesPaginator.paginate` method:

- `filters`:
  `Sequence`\[[FlowTemplateFilterTypeDef](./type_defs.md#flowtemplatefiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchFlowTemplatesPaginator.paginate` returns
`AsyncIterable`\[[SearchFlowTemplatesResponseTypeDef](./type_defs.md#searchflowtemplatesresponsetypedef)\].

<a id="searchsysteminstancespaginator"></a>

## SearchSystemInstancesPaginator

Type annotations for
`session.create_client("iotthingsgraph").get_paginator("search_system_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import SearchSystemInstancesPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:
    client: IoTThingsGraphClient
    paginator: SearchSystemInstancesPaginator = client.get_paginator("search_system_instances")
```

Boto3 documentation:
[IoTThingsGraph.Paginator.SearchSystemInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemInstances)

Arguments for `SearchSystemInstancesPaginator.paginate` method:

- `filters`:
  `Sequence`\[[SystemInstanceFilterTypeDef](./type_defs.md#systeminstancefiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchSystemInstancesPaginator.paginate` returns
`AsyncIterable`\[[SearchSystemInstancesResponseTypeDef](./type_defs.md#searchsysteminstancesresponsetypedef)\].

<a id="searchsystemtemplatespaginator"></a>

## SearchSystemTemplatesPaginator

Type annotations for
`session.create_client("iotthingsgraph").get_paginator("search_system_templates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import SearchSystemTemplatesPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:
    client: IoTThingsGraphClient
    paginator: SearchSystemTemplatesPaginator = client.get_paginator("search_system_templates")
```

Boto3 documentation:
[IoTThingsGraph.Paginator.SearchSystemTemplates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemTemplates)

Arguments for `SearchSystemTemplatesPaginator.paginate` method:

- `filters`:
  `Sequence`\[[SystemTemplateFilterTypeDef](./type_defs.md#systemtemplatefiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchSystemTemplatesPaginator.paginate` returns
`AsyncIterable`\[[SearchSystemTemplatesResponseTypeDef](./type_defs.md#searchsystemtemplatesresponsetypedef)\].

<a id="searchthingspaginator"></a>

## SearchThingsPaginator

Type annotations for
`session.create_client("iotthingsgraph").get_paginator("search_things")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.paginator import SearchThingsPaginator

session = get_session()
async with session.create_client("iotthingsgraph") as client:
    client: IoTThingsGraphClient
    paginator: SearchThingsPaginator = client.get_paginator("search_things")
```

Boto3 documentation:
[IoTThingsGraph.Paginator.SearchThings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchThings)

Arguments for `SearchThingsPaginator.paginate` method:

- `entityId`: `str` *(required)*
- `namespaceVersion`: `int`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchThingsPaginator.paginate` returns
`AsyncIterable`\[[SearchThingsResponseTypeDef](./type_defs.md#searchthingsresponsetypedef)\].
