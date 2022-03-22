<a id="examples-for-aiobotocore-cloudformation-module"></a>

# Examples for aiobotocore CloudFormation module

> [Index](../README.md) > [CloudFormation](./README.md) > Examples

- [Examples for aiobotocore CloudFormation module](#examples-for-aiobotocore-cloudformation-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cloudformation]` package installed.

Write your `CloudFormation` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CloudFormationClient
# and provides type checking and code completion
async with session.create_client("cloudformation") as client:
    
    # result has type ActivateTypeOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.activate_type()
    

    
    # paginator has type DescribeAccountLimitsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_account_limits")
    async for item in paginator.paginate(...):
        # item has type DescribeAccountLimitsOutputTypeDef
        print(item)
    

    
    # waiter has type ChangeSetCreateCompleteWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("change_set_create_complete")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cloudformation]` or a standalone
`types_aiobotocore_cloudformation` package, you have to explicitly specify
`client: CloudFormationClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.client import CloudFormationClient
from types_aiobotocore_cloudformation.type_defs import ActivateTypeOutputTypeDef
from types_aiobotocore_cloudformation.paginator import DescribeAccountLimitsPaginator
from types_aiobotocore_cloudformation.waiter import ChangeSetCreateCompleteWaiter
from types_aiobotocore_cloudformation.literals import PaginatorName
from types_aiobotocore_cloudformation.literals import WaiterName


session = get_session()

async with session.create_client("cloudformation") as client:
    client: CloudFormationClient

    
    result: ActivateTypeOutputTypeDef = client.activate_type()
    

    
    paginator_name: PaginatorName = "describe_account_limits"
    paginator: DescribeAccountLimitsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeAccountLimitsOutputTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "change_set_create_complete"
    waiter: ChangeSetCreateCompleteWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
