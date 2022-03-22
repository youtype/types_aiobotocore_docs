<a id="examples-for-aiobotocore-sns-module"></a>

# Examples for aiobotocore SNS module

> [Index](../README.md) > [SNS](./README.md) > Examples

- [Examples for aiobotocore SNS module](#examples-for-aiobotocore-sns-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sns]` package installed.

Write your `SNS` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SNSClient
# and provides type checking and code completion
async with session.create_client("sns") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_permission()
    

    
    # paginator has type ListEndpointsByPlatformApplicationPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_endpoints_by_platform_application")
    async for item in paginator.paginate(...):
        # item has type ListEndpointsByPlatformApplicationResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sns]` or a standalone `types_aiobotocore_sns`
package, you have to explicitly specify `client: SNSClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sns.client import SNSClient
from types_aiobotocore_sns.type_defs import None
from types_aiobotocore_sns.paginator import ListEndpointsByPlatformApplicationPaginator

from types_aiobotocore_sns.literals import PaginatorName



session = get_session()

async with session.create_client("sns") as client:
    client: SNSClient

    
    result: None = client.add_permission()
    

    
    paginator_name: PaginatorName = "list_endpoints_by_platform_application"
    paginator: ListEndpointsByPlatformApplicationPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListEndpointsByPlatformApplicationResponseTypeDef
        print(item)
    

    
```
