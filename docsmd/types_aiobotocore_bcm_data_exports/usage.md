# Examples

> [Index](../README.md) > [BillingandCostManagementDataExports](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BillingandCostManagementDataExports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#billingandcostmanagementdataexports)
    type annotations stubs module [types-aiobotocore-bcm-data-exports](https://pypi.org/project/types-aiobotocore-bcm-data-exports/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[bcm-data-exports]` package installed.

Write your `BillingandCostManagementDataExports` code as usual,
type checking and code completion should work out of the box.



```python
# BillingandCostManagementDataExportsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bcm-data-exports") as client:  # (1)
    result = await client.create_export()  # (2)
```

1. client: [BillingandCostManagementDataExportsClient](./client.md)
2. result: [:material-code-braces: CreateExportResponseTypeDef](./type_defs.md#createexportresponsetypedef) 



```python
# ListExecutionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bcm-data-exports") as client:  # (1)
    paginator = client.get_paginator("list_executions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BillingandCostManagementDataExportsClient](./client.md)
2. paginator: [ListExecutionsPaginator](./paginators.md#listexecutionspaginator)
3. item: [:material-code-braces: ListExecutionsResponseTypeDef](./type_defs.md#listexecutionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[bcm-data-exports]`
or a standalone `types_aiobotocore_bcm_data_exports` package, you have to explicitly specify
`client: BillingandCostManagementDataExportsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# BillingandCostManagementDataExportsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bcm_data_exports.client import BillingandCostManagementDataExportsClient
from types_aiobotocore_bcm_data_exports.type_defs import CreateExportResponseTypeDef
from types_aiobotocore_bcm_data_exports.type_defs import CreateExportRequestTypeDef


session = get_session()

async with session.create_client("bcm-data-exports") as client:
    client: BillingandCostManagementDataExportsClient
    kwargs: CreateExportRequestTypeDef = {...}
    result: CreateExportResponseTypeDef = await client.create_export(**kwargs)
```



```python
# ListExecutionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bcm_data_exports.client import BillingandCostManagementDataExportsClient
from types_aiobotocore_bcm_data_exports.paginator import ListExecutionsPaginator
from types_aiobotocore_bcm_data_exports.type_defs import ListExecutionsResponseTypeDef


session = get_session()

async with session.create_client("bcm-data-exports") as client:
    client: BillingandCostManagementDataExportsClient
    paginator: ListExecutionsPaginator = client.get_paginator("list_executions")
    async for item in paginator.paginate(...):
        item: ListExecutionsResponseTypeDef
        print(item)
```


