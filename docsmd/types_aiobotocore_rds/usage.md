# Examples

> [Index](../README.md) > [RDS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RDS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
    type annotations stubs module [types-aiobotocore-rds](https://pypi.org/project/types-aiobotocore-rds/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[rds]` package installed.

Write your `RDS` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("rds") as client:  # (1)
        result = await client.add_source_identifier_to_subscription()  # (2)
    ```

    1. client: [RDSClient](./client.md)
    2. result: [:material-code-braces: AddSourceIdentifierToSubscriptionResultTypeDef](./type_defs.md#addsourceidentifiertosubscriptionresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("rds") as client:  # (1)
        paginator = client.get_paginator("describe_certificates")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [RDSClient](./client.md)
    2. paginator: [DescribeCertificatesPaginator](./paginators.md#describecertificatespaginator)
    3. item: [:material-code-braces: CertificateMessageTypeDef](./type_defs.md#certificatemessagetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("rds") as client:  # (1)
        waiter = client.get_waiter("db_cluster_snapshot_available")  # (2)
        await waiter.wait()
    ```

    1. client: [RDSClient](./client.md)
    2. waiter: [DBClusterSnapshotAvailableWaiter](./waiters.md#dbclustersnapshotavailablewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[rds]`
or a standalone `types_aiobotocore_rds` package, you have to explicitly specify
`client: RDSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_rds.client import RDSClient
    from types_aiobotocore_rds.type_defs import AddSourceIdentifierToSubscriptionResultTypeDef
    from types_aiobotocore_rds.type_defs import AddSourceIdentifierToSubscriptionMessageRequestTypeDef


    session = get_session()

    async with session.create_client("rds") as client:
        client: RDSClient
        kwargs: AddSourceIdentifierToSubscriptionMessageRequestTypeDef = {...}
        result: AddSourceIdentifierToSubscriptionResultTypeDef = await client.add_source_identifier_to_subscription(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_rds.client import RDSClient
    from types_aiobotocore_rds.paginator import DescribeCertificatesPaginator
    from types_aiobotocore_rds.type_defs import CertificateMessageTypeDef


    session = get_session()

    async with session.create_client("rds") as client:
        client: RDSClient
        paginator: DescribeCertificatesPaginator = client.get_paginator("describe_certificates")
        async for item in paginator.paginate(...):
            item: CertificateMessageTypeDef
            print(item)
    ```



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_rds.client import RDSClient
    from types_aiobotocore_rds.waiter import DBClusterSnapshotAvailableWaiter


    session = get_session()

    async with session.create_client("rds") as client:
        client: RDSClient
        waiter: DBClusterSnapshotAvailableWaiter = client.get_waiter("db_cluster_snapshot_available")
        await waiter.wait()
    ```
