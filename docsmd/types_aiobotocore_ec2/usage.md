# Examples

> [Index](../README.md) > [EC2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EC2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#ec2)
    type annotations stubs module [types-aiobotocore-ec2](https://pypi.org/project/types-aiobotocore-ec2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ec2]` package installed.

Write your `EC2` code as usual,
type checking and code completion should work out of the box.



```python
# EC2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ec2") as client:  # (1)
    result = await client.accept_address_transfer()  # (2)
```

1. client: [EC2Client](./client.md)
2. result: [:material-code-braces: AcceptAddressTransferResultTypeDef](./type_defs.md#acceptaddresstransferresulttypedef) 



```python
# DescribeAddressTransfersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ec2") as client:  # (1)
    paginator = client.get_paginator("describe_address_transfers")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeAddressTransfersPaginator](./paginators.md#describeaddresstransferspaginator)
3. item: [:material-code-braces: DescribeAddressTransfersResultTypeDef](./type_defs.md#describeaddresstransfersresulttypedef) 



```python
# BundleTaskCompleteWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ec2") as client:  # (1)
    waiter = client.get_waiter("bundle_task_complete")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [BundleTaskCompleteWaiter](./waiters.md#bundletaskcompletewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[ec2]`
or a standalone `types_aiobotocore_ec2` package, you have to explicitly specify
`client: EC2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# EC2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ec2.client import EC2Client
from types_aiobotocore_ec2.type_defs import AcceptAddressTransferResultTypeDef
from types_aiobotocore_ec2.type_defs import AcceptAddressTransferRequestTypeDef


session = get_session()

async with session.create_client("ec2") as client:
    client: EC2Client
    kwargs: AcceptAddressTransferRequestTypeDef = {...}
    result: AcceptAddressTransferResultTypeDef = await client.accept_address_transfer(**kwargs)
```



```python
# DescribeAddressTransfersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ec2.client import EC2Client
from types_aiobotocore_ec2.paginator import DescribeAddressTransfersPaginator
from types_aiobotocore_ec2.type_defs import DescribeAddressTransfersResultTypeDef


session = get_session()

async with session.create_client("ec2") as client:
    client: EC2Client
    paginator: DescribeAddressTransfersPaginator = client.get_paginator("describe_address_transfers")
    async for item in paginator.paginate(...):
        item: DescribeAddressTransfersResultTypeDef
        print(item)
```



```python
# BundleTaskCompleteWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ec2.client import EC2Client
from types_aiobotocore_ec2.waiter import BundleTaskCompleteWaiter


session = get_session()

async with session.create_client("ec2") as client:
    client: EC2Client
    waiter: BundleTaskCompleteWaiter = client.get_waiter("bundle_task_complete")
    await waiter.wait()
```
