# Examples

> [Index](../README.md) > [IoTWireless](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTWireless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#iotwireless)
    type annotations stubs module [types-aiobotocore-iotwireless](https://pypi.org/project/types-aiobotocore-iotwireless/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iotwireless]` package installed.

Write your `IoTWireless` code as usual,
type checking and code completion should work out of the box.



```python
# IoTWirelessClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iotwireless") as client:  # (1)
    result = await client.associate_aws_account_with_partner_account()  # (2)
```

1. client: [IoTWirelessClient](./client.md)
2. result: [:material-code-braces: AssociateAwsAccountWithPartnerAccountResponseTypeDef](./type_defs.md#associateawsaccountwithpartneraccountresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[iotwireless]`
or a standalone `types_aiobotocore_iotwireless` package, you have to explicitly specify
`client: IoTWirelessClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IoTWirelessClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iotwireless.client import IoTWirelessClient
from types_aiobotocore_iotwireless.type_defs import AssociateAwsAccountWithPartnerAccountResponseTypeDef
from types_aiobotocore_iotwireless.type_defs import AssociateAwsAccountWithPartnerAccountRequestTypeDef


session = get_session()

async with session.create_client("iotwireless") as client:
    client: IoTWirelessClient
    kwargs: AssociateAwsAccountWithPartnerAccountRequestTypeDef = {...}
    result: AssociateAwsAccountWithPartnerAccountResponseTypeDef = await client.associate_aws_account_with_partner_account(**kwargs)
```




