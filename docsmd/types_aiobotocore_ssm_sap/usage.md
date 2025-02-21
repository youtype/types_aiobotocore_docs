# Examples

> [Index](../README.md) > [SsmSap](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SsmSap](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#ssmsap)
    type annotations stubs module [types-aiobotocore-ssm-sap](https://pypi.org/project/types-aiobotocore-ssm-sap/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ssm-sap]` package installed.

Write your `SsmSap` code as usual,
type checking and code completion should work out of the box.



```python
# SsmSapClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ssm-sap") as client:  # (1)
    result = await client.delete_resource_permission()  # (2)
```

1. client: [SsmSapClient](./client.md)
2. result: [:material-code-braces: DeleteResourcePermissionOutputTypeDef](./type_defs.md#deleteresourcepermissionoutputtypedef) 



```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ssm-sap") as client:  # (1)
    paginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SsmSapClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsOutputTypeDef](./type_defs.md#listapplicationsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[ssm-sap]`
or a standalone `types_aiobotocore_ssm_sap` package, you have to explicitly specify
`client: SsmSapClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SsmSapClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ssm_sap.client import SsmSapClient
from types_aiobotocore_ssm_sap.type_defs import DeleteResourcePermissionOutputTypeDef
from types_aiobotocore_ssm_sap.type_defs import DeleteResourcePermissionInputTypeDef


session = get_session()

async with session.create_client("ssm-sap") as client:
    client: SsmSapClient
    kwargs: DeleteResourcePermissionInputTypeDef = {...}
    result: DeleteResourcePermissionOutputTypeDef = await client.delete_resource_permission(**kwargs)
```



```python
# ListApplicationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ssm_sap.client import SsmSapClient
from types_aiobotocore_ssm_sap.paginator import ListApplicationsPaginator
from types_aiobotocore_ssm_sap.type_defs import ListApplicationsOutputTypeDef


session = get_session()

async with session.create_client("ssm-sap") as client:
    client: SsmSapClient
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
    async for item in paginator.paginate(...):
        item: ListApplicationsOutputTypeDef
        print(item)
```


