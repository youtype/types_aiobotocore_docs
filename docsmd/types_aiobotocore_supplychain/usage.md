# Examples

> [Index](../README.md) > [SupplyChain](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SupplyChain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#supplychain)
    type annotations stubs module [types-aiobotocore-supplychain](https://pypi.org/project/types-aiobotocore-supplychain/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[supplychain]` package installed.

Write your `SupplyChain` code as usual,
type checking and code completion should work out of the box.



```python
# SupplyChainClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("supplychain") as client:  # (1)
    result = await client.create_bill_of_materials_import_job()  # (2)
```

1. client: [SupplyChainClient](./client.md)
2. result: [:material-code-braces: CreateBillOfMaterialsImportJobResponseTypeDef](./type_defs.md#createbillofmaterialsimportjobresponsetypedef) 



```python
# ListDataIntegrationFlowsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("supplychain") as client:  # (1)
    paginator = client.get_paginator("list_data_integration_flows")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SupplyChainClient](./client.md)
2. paginator: [ListDataIntegrationFlowsPaginator](./paginators.md#listdataintegrationflowspaginator)
3. item: [:material-code-braces: ListDataIntegrationFlowsResponseTypeDef](./type_defs.md#listdataintegrationflowsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[supplychain]`
or a standalone `types_aiobotocore_supplychain` package, you have to explicitly specify
`client: SupplyChainClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SupplyChainClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_supplychain.client import SupplyChainClient
from types_aiobotocore_supplychain.type_defs import CreateBillOfMaterialsImportJobResponseTypeDef
from types_aiobotocore_supplychain.type_defs import CreateBillOfMaterialsImportJobRequestTypeDef


session = get_session()

async with session.create_client("supplychain") as client:
    client: SupplyChainClient
    kwargs: CreateBillOfMaterialsImportJobRequestTypeDef = {...}
    result: CreateBillOfMaterialsImportJobResponseTypeDef = await client.create_bill_of_materials_import_job(**kwargs)
```



```python
# ListDataIntegrationFlowsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_supplychain.client import SupplyChainClient
from types_aiobotocore_supplychain.paginator import ListDataIntegrationFlowsPaginator
from types_aiobotocore_supplychain.type_defs import ListDataIntegrationFlowsResponseTypeDef


session = get_session()

async with session.create_client("supplychain") as client:
    client: SupplyChainClient
    paginator: ListDataIntegrationFlowsPaginator = client.get_paginator("list_data_integration_flows")
    async for item in paginator.paginate(...):
        item: ListDataIntegrationFlowsResponseTypeDef
        print(item)
```


