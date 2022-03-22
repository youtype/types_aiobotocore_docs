<a id="examples-for-aiobotocore-customerprofiles-module"></a>

# Examples for aiobotocore CustomerProfiles module

> [Index](../README.md) > [CustomerProfiles](./README.md) > Examples

- [Examples for aiobotocore CustomerProfiles module](#examples-for-aiobotocore-customerprofiles-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[customer-profiles]` package installed.

Write your `CustomerProfiles` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CustomerProfilesClient
# and provides type checking and code completion
async with session.create_client("customer-profiles") as client:
    
    # result has type AddProfileKeyResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_profile_key()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[customer-profiles]` or a standalone
`types_aiobotocore_customer_profiles` package, you have to explicitly specify
`client: CustomerProfilesClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.client import CustomerProfilesClient
from types_aiobotocore_customer_profiles.type_defs import AddProfileKeyResponseTypeDef






session = get_session()

async with session.create_client("customer-profiles") as client:
    client: CustomerProfilesClient

    
    result: AddProfileKeyResponseTypeDef = client.add_profile_key()
    

    

    
```
