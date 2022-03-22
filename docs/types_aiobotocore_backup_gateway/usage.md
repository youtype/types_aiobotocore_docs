<a id="examples-for-aiobotocore-backupgateway-module"></a>

# Examples for aiobotocore BackupGateway module

> [Index](../README.md) > [BackupGateway](./README.md) > Examples

- [Examples for aiobotocore BackupGateway module](#examples-for-aiobotocore-backupgateway-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[backup-gateway]` package installed.

Write your `BackupGateway` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type BackupGatewayClient
# and provides type checking and code completion
async with session.create_client("backup-gateway") as client:
    
    # result has type AssociateGatewayToServerOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_gateway_to_server()
    

    
    # paginator has type ListGatewaysPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_gateways")
    async for item in paginator.paginate(...):
        # item has type ListGatewaysOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[backup-gateway]` or a standalone
`types_aiobotocore_backup_gateway` package, you have to explicitly specify
`client: BackupGatewayClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_backup_gateway.client import BackupGatewayClient
from types_aiobotocore_backup_gateway.type_defs import AssociateGatewayToServerOutputTypeDef
from types_aiobotocore_backup_gateway.paginator import ListGatewaysPaginator

from types_aiobotocore_backup_gateway.literals import PaginatorName



session = get_session()

async with session.create_client("backup-gateway") as client:
    client: BackupGatewayClient

    
    result: AssociateGatewayToServerOutputTypeDef = client.associate_gateway_to_server()
    

    
    paginator_name: PaginatorName = "list_gateways"
    paginator: ListGatewaysPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListGatewaysOutputTypeDef
        print(item)
    

    
```
