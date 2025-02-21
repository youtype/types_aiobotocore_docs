# Examples

> [Index](../README.md) > [IoTThingsGraph](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTThingsGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#iotthingsgraph)
    type annotations stubs module [types-aiobotocore-iotthingsgraph](https://pypi.org/project/types-aiobotocore-iotthingsgraph/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iotthingsgraph]` package installed.

Write your `IoTThingsGraph` code as usual,
type checking and code completion should work out of the box.



```python
# IoTThingsGraphClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iotthingsgraph") as client:  # (1)
    result = await client.create_flow_template()  # (2)
```

1. client: [IoTThingsGraphClient](./client.md)
2. result: [:material-code-braces: CreateFlowTemplateResponseTypeDef](./type_defs.md#createflowtemplateresponsetypedef) 



```python
# GetFlowTemplateRevisionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iotthingsgraph") as client:  # (1)
    paginator = client.get_paginator("get_flow_template_revisions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [GetFlowTemplateRevisionsPaginator](./paginators.md#getflowtemplaterevisionspaginator)
3. item: [:material-code-braces: GetFlowTemplateRevisionsResponseTypeDef](./type_defs.md#getflowtemplaterevisionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[iotthingsgraph]`
or a standalone `types_aiobotocore_iotthingsgraph` package, you have to explicitly specify
`client: IoTThingsGraphClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IoTThingsGraphClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.client import IoTThingsGraphClient
from types_aiobotocore_iotthingsgraph.type_defs import CreateFlowTemplateResponseTypeDef
from types_aiobotocore_iotthingsgraph.type_defs import CreateFlowTemplateRequestTypeDef


session = get_session()

async with session.create_client("iotthingsgraph") as client:
    client: IoTThingsGraphClient
    kwargs: CreateFlowTemplateRequestTypeDef = {...}
    result: CreateFlowTemplateResponseTypeDef = await client.create_flow_template(**kwargs)
```



```python
# GetFlowTemplateRevisionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iotthingsgraph.client import IoTThingsGraphClient
from types_aiobotocore_iotthingsgraph.paginator import GetFlowTemplateRevisionsPaginator
from types_aiobotocore_iotthingsgraph.type_defs import GetFlowTemplateRevisionsResponseTypeDef


session = get_session()

async with session.create_client("iotthingsgraph") as client:
    client: IoTThingsGraphClient
    paginator: GetFlowTemplateRevisionsPaginator = client.get_paginator("get_flow_template_revisions")
    async for item in paginator.paginate(...):
        item: GetFlowTemplateRevisionsResponseTypeDef
        print(item)
```


