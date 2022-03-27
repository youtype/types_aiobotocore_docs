# Examples

> [Index](../README.md) > [CustomerProfiles](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CustomerProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
    type annotations stubs module [types-aiobotocore-customer-profiles](https://pypi.org/project/types-aiobotocore-customer-profiles/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[customer-profiles]` package installed.

Write your `CustomerProfiles` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("customer-profiles") as client:  # (1)
        result = await client.add_profile_key()  # (2)
    ```

    1. client: [CustomerProfilesClient](./client.md)
    2. result: [:material-code-braces: AddProfileKeyResponseTypeDef](./type_defs.md#addprofilekeyresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[customer-profiles]`
or a standalone `types_aiobotocore_customer_profiles` package, you have to explicitly specify
`client: CustomerProfilesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_customer_profiles.client import CustomerProfilesClient
    from types_aiobotocore_customer_profiles.type_defs import AddProfileKeyResponseTypeDef
    from types_aiobotocore_customer_profiles.type_defs import AddProfileKeyRequestRequestTypeDef


    session = get_session()

    async with session.create_client("customer-profiles") as client:
        client: CustomerProfilesClient
        kwargs: AddProfileKeyRequestRequestTypeDef = {...}
        result: AddProfileKeyResponseTypeDef = await client.add_profile_key(**kwargs)
    ```




