# Examples

> [Index](../README.md) > [IAM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
    type annotations stubs module [types-aiobotocore-iam](https://pypi.org/project/types-aiobotocore-iam/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iam]` package installed.

Write your `IAM` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("iam") as client:  # (1)
        result = await client.create_access_key()  # (2)
    ```

    1. client: [IAMClient](./client.md)
    2. result: [:material-code-braces: CreateAccessKeyResponseTypeDef](./type_defs.md#createaccesskeyresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("iam") as client:  # (1)
        paginator = client.get_paginator("get_account_authorization_details")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [IAMClient](./client.md)
    2. paginator: [GetAccountAuthorizationDetailsPaginator](./paginators.md#getaccountauthorizationdetailspaginator)
    3. item: [:material-code-braces: GetAccountAuthorizationDetailsResponseTypeDef](./type_defs.md#getaccountauthorizationdetailsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("iam") as client:  # (1)
        waiter = client.get_waiter("instance_profile_exists")  # (2)
        await waiter.wait()
    ```

    1. client: [IAMClient](./client.md)
    2. waiter: [InstanceProfileExistsWaiter](./waiters.md#instanceprofileexistswaiter)


### Explicit type annotations

With `types-aiobotocore-lite[iam]`
or a standalone `types_aiobotocore_iam` package, you have to explicitly specify
`client: IAMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_iam.client import IAMClient
    from types_aiobotocore_iam.type_defs import CreateAccessKeyResponseTypeDef
    from types_aiobotocore_iam.type_defs import CreateAccessKeyRequestRequestTypeDef


    session = get_session()

    async with session.create_client("iam") as client:
        client: IAMClient
        kwargs: CreateAccessKeyRequestRequestTypeDef = {...}
        result: CreateAccessKeyResponseTypeDef = await client.create_access_key(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_iam.client import IAMClient
    from types_aiobotocore_iam.paginator import GetAccountAuthorizationDetailsPaginator
    from types_aiobotocore_iam.type_defs import GetAccountAuthorizationDetailsResponseTypeDef


    session = get_session()

    async with session.create_client("iam") as client:
        client: IAMClient
        paginator: GetAccountAuthorizationDetailsPaginator = client.get_paginator("get_account_authorization_details")
        async for item in paginator.paginate(...):
            item: GetAccountAuthorizationDetailsResponseTypeDef
            print(item)
    ```



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_iam.client import IAMClient
    from types_aiobotocore_iam.waiter import InstanceProfileExistsWaiter


    session = get_session()

    async with session.create_client("iam") as client:
        client: IAMClient
        waiter: InstanceProfileExistsWaiter = client.get_waiter("instance_profile_exists")
        await waiter.wait()
    ```
