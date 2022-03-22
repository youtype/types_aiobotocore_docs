<a id="examples-for-aiobotocore-ec2-module"></a>

# Examples for aiobotocore EC2 module

> [Index](../README.md) > [EC2](./README.md) > Examples

- [Examples for aiobotocore EC2 module](#examples-for-aiobotocore-ec2-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[ec2]` package installed.

Write your `EC2` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type EC2Client
# and provides type checking and code completion
async with session.create_client("ec2") as client:
    
    # result has type AcceptReservedInstancesExchangeQuoteResultTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_reserved_instances_exchange_quote()
    

    
    # paginator has type DescribeAddressesAttributePaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_addresses_attribute")
    async for item in paginator.paginate(...):
        # item has type DescribeAddressesAttributeResultTypeDef
        print(item)
    

    
    # waiter has type BundleTaskCompleteWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("bundle_task_complete")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[ec2]` or a standalone `types_aiobotocore_ec2`
package, you have to explicitly specify `client: EC2Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_ec2.client import EC2Client
from types_aiobotocore_ec2.type_defs import AcceptReservedInstancesExchangeQuoteResultTypeDef
from types_aiobotocore_ec2.paginator import DescribeAddressesAttributePaginator
from types_aiobotocore_ec2.waiter import BundleTaskCompleteWaiter
from types_aiobotocore_ec2.literals import PaginatorName
from types_aiobotocore_ec2.literals import WaiterName


session = get_session()

async with session.create_client("ec2") as client:
    client: EC2Client

    
    result: AcceptReservedInstancesExchangeQuoteResultTypeDef = client.accept_reserved_instances_exchange_quote()
    

    
    paginator_name: PaginatorName = "describe_addresses_attribute"
    paginator: DescribeAddressesAttributePaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeAddressesAttributeResultTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "bundle_task_complete"
    waiter: BundleTaskCompleteWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
