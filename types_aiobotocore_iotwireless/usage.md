<a id="examples-for-aiobotocore-iotwireless-module"></a>

# Examples for aiobotocore IoTWireless module

> [Index](../README.md) > [IoTWireless](./README.md) > Examples

- [Examples for aiobotocore IoTWireless module](#examples-for-aiobotocore-iotwireless-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iotwireless]` package installed.

Write your `IoTWireless` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoTWirelessClient
# and provides type checking and code completion
async with session.create_client("iotwireless") as client:
    
    # result has type AssociateAwsAccountWithPartnerAccountResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_aws_account_with_partner_account()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iotwireless]` or a standalone
`types_aiobotocore_iotwireless` package, you have to explicitly specify
`client: IoTWirelessClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotwireless.client import IoTWirelessClient
from types_aiobotocore_iotwireless.type_defs import AssociateAwsAccountWithPartnerAccountResponseTypeDef






session = get_session()

async with session.create_client("iotwireless") as client:
    client: IoTWirelessClient

    
    result: AssociateAwsAccountWithPartnerAccountResponseTypeDef = client.associate_aws_account_with_partner_account()
    

    

    
```
