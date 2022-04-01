# Examples

> [Index](../README.md) > [EC2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EC2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
    type annotations stubs module [types-aiobotocore-ec2](https://pypi.org/project/types-aiobotocore-ec2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ec2]` package installed.

Write your `EC2` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("ec2") as client:  # (1)
        result = await client.accept_reserved_instances_exchange_quote()  # (2)
    ```

    1. client: [EC2Client](./client.md)
    2. result: [:material-code-braces: AcceptReservedInstancesExchangeQuoteResultTypeDef](./type_defs.md#acceptreservedinstancesexchangequoteresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("ec2") as client:  # (1)
        paginator = client.get_paginator("describe_addresses_attribute")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [EC2Client](./client.md)
    2. paginator: [DescribeAddressesAttributePaginator](./paginators.md#describeaddressesattributepaginator)
    3. item: [:material-code-braces: DescribeAddressesAttributeResultTypeDef](./type_defs.md#describeaddressesattributeresulttypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
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


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_ec2.client import EC2Client
    from types_aiobotocore_ec2.type_defs import AcceptReservedInstancesExchangeQuoteResultTypeDef
    from types_aiobotocore_ec2.type_defs import AcceptReservedInstancesExchangeQuoteRequestRequestTypeDef


    session = get_session()

    async with session.create_client("ec2") as client:
        client: EC2Client
        kwargs: AcceptReservedInstancesExchangeQuoteRequestRequestTypeDef = {...}
        result: AcceptReservedInstancesExchangeQuoteResultTypeDef = await client.accept_reserved_instances_exchange_quote(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_ec2.client import EC2Client
    from types_aiobotocore_ec2.paginator import DescribeAddressesAttributePaginator
    from types_aiobotocore_ec2.type_defs import DescribeAddressesAttributeResultTypeDef


    session = get_session()

    async with session.create_client("ec2") as client:
        client: EC2Client
        paginator: DescribeAddressesAttributePaginator = client.get_paginator("describe_addresses_attribute")
        async for item in paginator.paginate(...):
            item: DescribeAddressesAttributeResultTypeDef
            print(item)
    ```



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_ec2.client import EC2Client
    from types_aiobotocore_ec2.waiter import BundleTaskCompleteWaiter


    session = get_session()

    async with session.create_client("ec2") as client:
        client: EC2Client
        waiter: BundleTaskCompleteWaiter = client.get_waiter("bundle_task_complete")
        await waiter.wait()
    ```
