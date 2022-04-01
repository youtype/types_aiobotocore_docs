# Examples

> [Index](../README.md) > [SageMaker](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SageMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
    type annotations stubs module [types-aiobotocore-sagemaker](https://pypi.org/project/types-aiobotocore-sagemaker/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sagemaker]` package installed.

Write your `SageMaker` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("sagemaker") as client:  # (1)
        result = await client.add_association()  # (2)
    ```

    1. client: [SageMakerClient](./client.md)
    2. result: [:material-code-braces: AddAssociationResponseTypeDef](./type_defs.md#addassociationresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("sagemaker") as client:  # (1)
        paginator = client.get_paginator("list_actions")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [SageMakerClient](./client.md)
    2. paginator: [ListActionsPaginator](./paginators.md#listactionspaginator)
    3. item: [:material-code-braces: ListActionsResponseTypeDef](./type_defs.md#listactionsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("sagemaker") as client:  # (1)
        waiter = client.get_waiter("endpoint_deleted")  # (2)
        await waiter.wait()
    ```

    1. client: [SageMakerClient](./client.md)
    2. waiter: [EndpointDeletedWaiter](./waiters.md#endpointdeletedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[sagemaker]`
or a standalone `types_aiobotocore_sagemaker` package, you have to explicitly specify
`client: SageMakerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_sagemaker.client import SageMakerClient
    from types_aiobotocore_sagemaker.type_defs import AddAssociationResponseTypeDef
    from types_aiobotocore_sagemaker.type_defs import AddAssociationRequestRequestTypeDef


    session = get_session()

    async with session.create_client("sagemaker") as client:
        client: SageMakerClient
        kwargs: AddAssociationRequestRequestTypeDef = {...}
        result: AddAssociationResponseTypeDef = await client.add_association(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_sagemaker.client import SageMakerClient
    from types_aiobotocore_sagemaker.paginator import ListActionsPaginator
    from types_aiobotocore_sagemaker.type_defs import ListActionsResponseTypeDef


    session = get_session()

    async with session.create_client("sagemaker") as client:
        client: SageMakerClient
        paginator: ListActionsPaginator = client.get_paginator("list_actions")
        async for item in paginator.paginate(...):
            item: ListActionsResponseTypeDef
            print(item)
    ```



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_sagemaker.client import SageMakerClient
    from types_aiobotocore_sagemaker.waiter import EndpointDeletedWaiter


    session = get_session()

    async with session.create_client("sagemaker") as client:
        client: SageMakerClient
        waiter: EndpointDeletedWaiter = client.get_waiter("endpoint_deleted")
        await waiter.wait()
    ```
