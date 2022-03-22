<a id="examples-for-aiobotocore-iotthingsgraph-module"></a>

# Examples for aiobotocore IoTThingsGraph module

> [Index](../README.md) > [IoTThingsGraph](./README.md) > Examples

- [Examples for aiobotocore IoTThingsGraph module](#examples-for-aiobotocore-iotthingsgraph-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iotthingsgraph]` package installed.

Write your `IoTThingsGraph` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoTThingsGraphClient
# and provides type checking and code completion
async with session.create_client("iotthingsgraph") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_entity_to_thing()
    

    
    # paginator has type GetFlowTemplateRevisionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_flow_template_revisions")
    async for item in paginator.paginate(...):
        # item has type GetFlowTemplateRevisionsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iotthingsgraph]` or a standalone
`types_aiobotocore_iotthingsgraph` package, you have to explicitly specify
`client: IoTThingsGraphClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.client import IoTThingsGraphClient
from types_aiobotocore_iotthingsgraph.type_defs import Dict[str, Any]
from types_aiobotocore_iotthingsgraph.paginator import GetFlowTemplateRevisionsPaginator

from types_aiobotocore_iotthingsgraph.literals import PaginatorName



session = get_session()

async with session.create_client("iotthingsgraph") as client:
    client: IoTThingsGraphClient

    
    result: Dict[str, Any] = client.associate_entity_to_thing()
    

    
    paginator_name: PaginatorName = "get_flow_template_revisions"
    paginator: GetFlowTemplateRevisionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetFlowTemplateRevisionsResponseTypeDef
        print(item)
    

    
```
