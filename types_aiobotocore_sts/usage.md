<a id="examples-for-aiobotocore-sts-module"></a>

# Examples for aiobotocore STS module

> [Index](../README.md) > [STS](./README.md) > Examples

- [Examples for aiobotocore STS module](#examples-for-aiobotocore-sts-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sts]` package installed.

Write your `STS` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type STSClient
# and provides type checking and code completion
async with session.create_client("sts") as client:
    
    # result has type AssumeRoleResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.assume_role()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sts]` or a standalone `types_aiobotocore_sts`
package, you have to explicitly specify `client: STSClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sts.client import STSClient
from types_aiobotocore_sts.type_defs import AssumeRoleResponseTypeDef






session = get_session()

async with session.create_client("sts") as client:
    client: STSClient

    
    result: AssumeRoleResponseTypeDef = client.assume_role()
    

    

    
```
