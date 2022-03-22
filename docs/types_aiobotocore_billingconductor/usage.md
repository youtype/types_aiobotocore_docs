<a id="examples-for-aiobotocore-billingconductor-module"></a>

# Examples for aiobotocore BillingConductor module

> [Index](../README.md) > [BillingConductor](./README.md) > Examples

- [Examples for aiobotocore BillingConductor module](#examples-for-aiobotocore-billingconductor-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[billingconductor]` package installed.

Write your `BillingConductor` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type BillingConductorClient
# and provides type checking and code completion
async with session.create_client("billingconductor") as client:
    
    # result has type AssociateAccountsOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_accounts()
    

    
    # paginator has type ListAccountAssociationsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_account_associations")
    async for item in paginator.paginate(...):
        # item has type ListAccountAssociationsOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[billingconductor]` or a standalone
`types_aiobotocore_billingconductor` package, you have to explicitly specify
`client: BillingConductorClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_billingconductor.client import BillingConductorClient
from types_aiobotocore_billingconductor.type_defs import AssociateAccountsOutputTypeDef
from types_aiobotocore_billingconductor.paginator import ListAccountAssociationsPaginator

from types_aiobotocore_billingconductor.literals import PaginatorName



session = get_session()

async with session.create_client("billingconductor") as client:
    client: BillingConductorClient

    
    result: AssociateAccountsOutputTypeDef = client.associate_accounts()
    

    
    paginator_name: PaginatorName = "list_account_associations"
    paginator: ListAccountAssociationsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAccountAssociationsOutputTypeDef
        print(item)
    

    
```
