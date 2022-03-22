<a id="examples-for-aiobotocore-ssm-module"></a>

# Examples for aiobotocore SSM module

> [Index](../README.md) > [SSM](./README.md) > Examples

- [Examples for aiobotocore SSM module](#examples-for-aiobotocore-ssm-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[ssm]` package installed.

Write your `SSM` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SSMClient
# and provides type checking and code completion
async with session.create_client("ssm") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_tags_to_resource()
    

    
    # paginator has type DescribeActivationsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_activations")
    async for item in paginator.paginate(...):
        # item has type DescribeActivationsResultTypeDef
        print(item)
    

    
    # waiter has type CommandExecutedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("command_executed")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[ssm]` or a standalone `types_aiobotocore_ssm`
package, you have to explicitly specify `client: SSMClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_ssm.client import SSMClient
from types_aiobotocore_ssm.type_defs import Dict[str, Any]
from types_aiobotocore_ssm.paginator import DescribeActivationsPaginator
from types_aiobotocore_ssm.waiter import CommandExecutedWaiter
from types_aiobotocore_ssm.literals import PaginatorName
from types_aiobotocore_ssm.literals import WaiterName


session = get_session()

async with session.create_client("ssm") as client:
    client: SSMClient

    
    result: Dict[str, Any] = client.add_tags_to_resource()
    

    
    paginator_name: PaginatorName = "describe_activations"
    paginator: DescribeActivationsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeActivationsResultTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "command_executed"
    waiter: CommandExecutedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
