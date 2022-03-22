<a id="examples-for-aiobotocore-ssooidc-module"></a>

# Examples for aiobotocore SSOOIDC module

> [Index](../README.md) > [SSOOIDC](./README.md) > Examples

- [Examples for aiobotocore SSOOIDC module](#examples-for-aiobotocore-ssooidc-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sso-oidc]` package installed.

Write your `SSOOIDC` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SSOOIDCClient
# and provides type checking and code completion
async with session.create_client("sso-oidc") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sso-oidc]` or a standalone
`types_aiobotocore_sso_oidc` package, you have to explicitly specify
`client: SSOOIDCClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sso_oidc.client import SSOOIDCClient
from types_aiobotocore_sso_oidc.type_defs import bool






session = get_session()

async with session.create_client("sso-oidc") as client:
    client: SSOOIDCClient

    
    result: bool = client.can_paginate()
    

    

    
```
