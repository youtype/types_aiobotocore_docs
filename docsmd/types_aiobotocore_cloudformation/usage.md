# Examples

> [Index](../README.md) > [CloudFormation](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#cloudformation)
    type annotations stubs module [types-aiobotocore-cloudformation](https://pypi.org/project/types-aiobotocore-cloudformation/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cloudformation]` package installed.

Write your `CloudFormation` code as usual,
type checking and code completion should work out of the box.



```python
# CloudFormationClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudformation") as client:  # (1)
    result = await client.activate_type()  # (2)
```

1. client: [CloudFormationClient](./client.md)
2. result: [:material-code-braces: ActivateTypeOutputTypeDef](./type_defs.md#activatetypeoutputtypedef) 



```python
# DescribeAccountLimitsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudformation") as client:  # (1)
    paginator = client.get_paginator("describe_account_limits")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
3. item: [:material-code-braces: DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef) 



```python
# ChangeSetCreateCompleteWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudformation") as client:  # (1)
    waiter = client.get_waiter("change_set_create_complete")  # (2)
    await waiter.wait()
```

1. client: [CloudFormationClient](./client.md)
2. waiter: [ChangeSetCreateCompleteWaiter](./waiters.md#changesetcreatecompletewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[cloudformation]`
or a standalone `types_aiobotocore_cloudformation` package, you have to explicitly specify
`client: CloudFormationClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudFormationClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.client import CloudFormationClient
from types_aiobotocore_cloudformation.type_defs import ActivateTypeOutputTypeDef
from types_aiobotocore_cloudformation.type_defs import ActivateTypeInputTypeDef


session = get_session()

async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    kwargs: ActivateTypeInputTypeDef = {...}
    result: ActivateTypeOutputTypeDef = await client.activate_type(**kwargs)
```



```python
# DescribeAccountLimitsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.client import CloudFormationClient
from types_aiobotocore_cloudformation.paginator import DescribeAccountLimitsPaginator
from types_aiobotocore_cloudformation.type_defs import DescribeAccountLimitsOutputTypeDef


session = get_session()

async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")
    async for item in paginator.paginate(...):
        item: DescribeAccountLimitsOutputTypeDef
        print(item)
```



```python
# ChangeSetCreateCompleteWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.client import CloudFormationClient
from types_aiobotocore_cloudformation.waiter import ChangeSetCreateCompleteWaiter


session = get_session()

async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    waiter: ChangeSetCreateCompleteWaiter = client.get_waiter("change_set_create_complete")
    await waiter.wait()
```
