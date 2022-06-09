# Examples

> [Index](../README.md) > [CloudWatchLogs](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchLogs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
    type annotations stubs module [types-aiobotocore-logs](https://pypi.org/project/types-aiobotocore-logs/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[logs]` package installed.

Write your `CloudWatchLogs` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("logs") as client:  # (1)
        result = await client.associate_kms_key()  # (2)
    ```

    1. client: [CloudWatchLogsClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("logs") as client:  # (1)
        paginator = client.get_paginator("describe_destinations")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CloudWatchLogsClient](./client.md)
    2. paginator: [DescribeDestinationsPaginator](./paginators.md#describedestinationspaginator)
    3. item: [:material-code-braces: DescribeDestinationsResponseTypeDef](./type_defs.md#describedestinationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[logs]`
or a standalone `types_aiobotocore_logs` package, you have to explicitly specify
`client: CloudWatchLogsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_logs.client import CloudWatchLogsClient
    from types_aiobotocore_logs.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_logs.type_defs import AssociateKmsKeyRequestRequestTypeDef


    session = get_session()

    async with session.create_client("logs") as client:
        client: CloudWatchLogsClient
        kwargs: AssociateKmsKeyRequestRequestTypeDef = {...}
        result: EmptyResponseMetadataTypeDef = await client.associate_kms_key(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_logs.client import CloudWatchLogsClient
    from types_aiobotocore_logs.paginator import DescribeDestinationsPaginator
    from types_aiobotocore_logs.type_defs import DescribeDestinationsResponseTypeDef


    session = get_session()

    async with session.create_client("logs") as client:
        client: CloudWatchLogsClient
        paginator: DescribeDestinationsPaginator = client.get_paginator("describe_destinations")
        async for item in paginator.paginate(...):
            item: DescribeDestinationsResponseTypeDef
            print(item)
    ```


