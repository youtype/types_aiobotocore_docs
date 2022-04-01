# Examples

> [Index](../README.md) > [Macie](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Macie](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
    type annotations stubs module [types-aiobotocore-macie](https://pypi.org/project/types-aiobotocore-macie/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[macie]` package installed.

Write your `Macie` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("macie") as client:  # (1)
        result = await client.associate_s3_resources()  # (2)
    ```

    1. client: [MacieClient](./client.md)
    2. result: [:material-code-braces: AssociateS3ResourcesResultTypeDef](./type_defs.md#associates3resourcesresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("macie") as client:  # (1)
        paginator = client.get_paginator("list_member_accounts")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MacieClient](./client.md)
    2. paginator: [ListMemberAccountsPaginator](./paginators.md#listmemberaccountspaginator)
    3. item: [:material-code-braces: ListMemberAccountsResultTypeDef](./type_defs.md#listmemberaccountsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[macie]`
or a standalone `types_aiobotocore_macie` package, you have to explicitly specify
`client: MacieClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_macie.client import MacieClient
    from types_aiobotocore_macie.type_defs import AssociateS3ResourcesResultTypeDef
    from types_aiobotocore_macie.type_defs import AssociateS3ResourcesRequestRequestTypeDef


    session = get_session()

    async with session.create_client("macie") as client:
        client: MacieClient
        kwargs: AssociateS3ResourcesRequestRequestTypeDef = {...}
        result: AssociateS3ResourcesResultTypeDef = await client.associate_s3_resources(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_macie.client import MacieClient
    from types_aiobotocore_macie.paginator import ListMemberAccountsPaginator
    from types_aiobotocore_macie.type_defs import ListMemberAccountsResultTypeDef


    session = get_session()

    async with session.create_client("macie") as client:
        client: MacieClient
        paginator: ListMemberAccountsPaginator = client.get_paginator("list_member_accounts")
        async for item in paginator.paginate(...):
            item: ListMemberAccountsResultTypeDef
            print(item)
    ```


