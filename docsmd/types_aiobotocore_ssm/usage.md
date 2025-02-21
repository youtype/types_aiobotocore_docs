# Examples

> [Index](../README.md) > [SSM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#ssm)
    type annotations stubs module [types-aiobotocore-ssm](https://pypi.org/project/types-aiobotocore-ssm/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ssm]` package installed.

Write your `SSM` code as usual,
type checking and code completion should work out of the box.



```python
# SSMClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ssm") as client:  # (1)
    result = await client.associate_ops_item_related_item()  # (2)
```

1. client: [SSMClient](./client.md)
2. result: [:material-code-braces: AssociateOpsItemRelatedItemResponseTypeDef](./type_defs.md#associateopsitemrelateditemresponsetypedef) 



```python
# DescribeActivationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ssm") as client:  # (1)
    paginator = client.get_paginator("describe_activations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SSMClient](./client.md)
2. paginator: [DescribeActivationsPaginator](./paginators.md#describeactivationspaginator)
3. item: [:material-code-braces: DescribeActivationsResultTypeDef](./type_defs.md#describeactivationsresulttypedef) 



```python
# CommandExecutedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ssm") as client:  # (1)
    waiter = client.get_waiter("command_executed")  # (2)
    await waiter.wait()
```

1. client: [SSMClient](./client.md)
2. waiter: [CommandExecutedWaiter](./waiters.md#commandexecutedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[ssm]`
or a standalone `types_aiobotocore_ssm` package, you have to explicitly specify
`client: SSMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SSMClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ssm.client import SSMClient
from types_aiobotocore_ssm.type_defs import AssociateOpsItemRelatedItemResponseTypeDef
from types_aiobotocore_ssm.type_defs import AssociateOpsItemRelatedItemRequestTypeDef


session = get_session()

async with session.create_client("ssm") as client:
    client: SSMClient
    kwargs: AssociateOpsItemRelatedItemRequestTypeDef = {...}
    result: AssociateOpsItemRelatedItemResponseTypeDef = await client.associate_ops_item_related_item(**kwargs)
```



```python
# DescribeActivationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ssm.client import SSMClient
from types_aiobotocore_ssm.paginator import DescribeActivationsPaginator
from types_aiobotocore_ssm.type_defs import DescribeActivationsResultTypeDef


session = get_session()

async with session.create_client("ssm") as client:
    client: SSMClient
    paginator: DescribeActivationsPaginator = client.get_paginator("describe_activations")
    async for item in paginator.paginate(...):
        item: DescribeActivationsResultTypeDef
        print(item)
```



```python
# CommandExecutedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ssm.client import SSMClient
from types_aiobotocore_ssm.waiter import CommandExecutedWaiter


session = get_session()

async with session.create_client("ssm") as client:
    client: SSMClient
    waiter: CommandExecutedWaiter = client.get_waiter("command_executed")
    await waiter.wait()
```
