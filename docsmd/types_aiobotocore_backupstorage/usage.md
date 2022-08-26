# Examples

> [Index](../README.md) > [BackupStorage](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BackupStorage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
    type annotations stubs module [types-aiobotocore-backupstorage](https://pypi.org/project/types-aiobotocore-backupstorage/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[backupstorage]` package installed.

Write your `BackupStorage` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("backupstorage") as client:  # (1)
        result = await client.delete_object()  # (2)
    ```

    1. client: [BackupStorageClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[backupstorage]`
or a standalone `types_aiobotocore_backupstorage` package, you have to explicitly specify
`client: BackupStorageClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_backupstorage.client import BackupStorageClient
    from types_aiobotocore_backupstorage.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_backupstorage.type_defs import DeleteObjectInputRequestTypeDef


    session = get_session()

    async with session.create_client("backupstorage") as client:
        client: BackupStorageClient
        kwargs: DeleteObjectInputRequestTypeDef = {...}
        result: EmptyResponseMetadataTypeDef = await client.delete_object(**kwargs)
    ```




