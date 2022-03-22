<a id="examples-for-aiobotocore-cloudsearchdomain-module"></a>

# Examples for aiobotocore CloudSearchDomain module

> [Index](../README.md) > [CloudSearchDomain](./README.md) > Examples

- [Examples for aiobotocore CloudSearchDomain module](#examples-for-aiobotocore-cloudsearchdomain-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cloudsearchdomain]` package installed.

Write your `CloudSearchDomain` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CloudSearchDomainClient
# and provides type checking and code completion
async with session.create_client("cloudsearchdomain") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cloudsearchdomain]` or a standalone
`types_aiobotocore_cloudsearchdomain` package, you have to explicitly specify
`client: CloudSearchDomainClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudsearchdomain.client import CloudSearchDomainClient
from types_aiobotocore_cloudsearchdomain.type_defs import bool






session = get_session()

async with session.create_client("cloudsearchdomain") as client:
    client: CloudSearchDomainClient

    
    result: bool = client.can_paginate()
    

    

    
```
