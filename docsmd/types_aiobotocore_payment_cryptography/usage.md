# Examples

> [Index](../README.md) > [PaymentCryptographyControlPlane](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PaymentCryptographyControlPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#paymentcryptographycontrolplane)
    type annotations stubs module [types-aiobotocore-payment-cryptography](https://pypi.org/project/types-aiobotocore-payment-cryptography/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[payment-cryptography]` package installed.

Write your `PaymentCryptographyControlPlane` code as usual,
type checking and code completion should work out of the box.



```python
# PaymentCryptographyControlPlaneClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("payment-cryptography") as client:  # (1)
    result = await client.create_alias()  # (2)
```

1. client: [PaymentCryptographyControlPlaneClient](./client.md)
2. result: [:material-code-braces: CreateAliasOutputTypeDef](./type_defs.md#createaliasoutputtypedef) 



```python
# ListAliasesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("payment-cryptography") as client:  # (1)
    paginator = client.get_paginator("list_aliases")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PaymentCryptographyControlPlaneClient](./client.md)
2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
3. item: [:material-code-braces: ListAliasesOutputTypeDef](./type_defs.md#listaliasesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[payment-cryptography]`
or a standalone `types_aiobotocore_payment_cryptography` package, you have to explicitly specify
`client: PaymentCryptographyControlPlaneClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PaymentCryptographyControlPlaneClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_payment_cryptography.client import PaymentCryptographyControlPlaneClient
from types_aiobotocore_payment_cryptography.type_defs import CreateAliasOutputTypeDef
from types_aiobotocore_payment_cryptography.type_defs import CreateAliasInputTypeDef


session = get_session()

async with session.create_client("payment-cryptography") as client:
    client: PaymentCryptographyControlPlaneClient
    kwargs: CreateAliasInputTypeDef = {...}
    result: CreateAliasOutputTypeDef = await client.create_alias(**kwargs)
```



```python
# ListAliasesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_payment_cryptography.client import PaymentCryptographyControlPlaneClient
from types_aiobotocore_payment_cryptography.paginator import ListAliasesPaginator
from types_aiobotocore_payment_cryptography.type_defs import ListAliasesOutputTypeDef


session = get_session()

async with session.create_client("payment-cryptography") as client:
    client: PaymentCryptographyControlPlaneClient
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
    async for item in paginator.paginate(...):
        item: ListAliasesOutputTypeDef
        print(item)
```


