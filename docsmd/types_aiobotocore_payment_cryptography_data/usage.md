# Examples

> [Index](../README.md) > [PaymentCryptographyDataPlane](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PaymentCryptographyDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#paymentcryptographydataplane)
    type annotations stubs module [types-aiobotocore-payment-cryptography-data](https://pypi.org/project/types-aiobotocore-payment-cryptography-data/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[payment-cryptography-data]` package installed.

Write your `PaymentCryptographyDataPlane` code as usual,
type checking and code completion should work out of the box.



```python
# PaymentCryptographyDataPlaneClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("payment-cryptography-data") as client:  # (1)
    result = await client.decrypt_data()  # (2)
```

1. client: [PaymentCryptographyDataPlaneClient](./client.md)
2. result: [:material-code-braces: DecryptDataOutputTypeDef](./type_defs.md#decryptdataoutputtypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[payment-cryptography-data]`
or a standalone `types_aiobotocore_payment_cryptography_data` package, you have to explicitly specify
`client: PaymentCryptographyDataPlaneClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PaymentCryptographyDataPlaneClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_payment_cryptography_data.client import PaymentCryptographyDataPlaneClient
from types_aiobotocore_payment_cryptography_data.type_defs import DecryptDataOutputTypeDef
from types_aiobotocore_payment_cryptography_data.type_defs import DecryptDataInputTypeDef


session = get_session()

async with session.create_client("payment-cryptography-data") as client:
    client: PaymentCryptographyDataPlaneClient
    kwargs: DecryptDataInputTypeDef = {...}
    result: DecryptDataOutputTypeDef = await client.decrypt_data(**kwargs)
```




