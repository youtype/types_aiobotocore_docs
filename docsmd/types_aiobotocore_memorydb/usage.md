# Examples

> [Index](../README.md) > [MemoryDB](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MemoryDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
    type annotations stubs module [types-aiobotocore-memorydb](https://pypi.org/project/types-aiobotocore-memorydb/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[memorydb]` package installed.

Write your `MemoryDB` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("memorydb") as client:  # (1)
        result = await client.batch_update_cluster()  # (2)
    ```

    1. client: [MemoryDBClient](./client.md)
    2. result: [:material-code-braces: BatchUpdateClusterResponseTypeDef](./type_defs.md#batchupdateclusterresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[memorydb]`
or a standalone `types_aiobotocore_memorydb` package, you have to explicitly specify
`client: MemoryDBClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_memorydb.client import MemoryDBClient
    from types_aiobotocore_memorydb.type_defs import BatchUpdateClusterResponseTypeDef
    from types_aiobotocore_memorydb.type_defs import BatchUpdateClusterRequestRequestTypeDef


    session = get_session()

    async with session.create_client("memorydb") as client:
        client: MemoryDBClient
        kwargs: BatchUpdateClusterRequestRequestTypeDef = {...}
        result: BatchUpdateClusterResponseTypeDef = await client.batch_update_cluster(**kwargs)
    ```




