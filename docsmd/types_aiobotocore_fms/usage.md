# Examples

> [Index](../README.md) > [FMS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [FMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
    type annotations stubs module [types-aiobotocore-fms](https://pypi.org/project/types-aiobotocore-fms/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[fms]` package installed.

Write your `FMS` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("fms") as client:  # (1)
        result = await client.associate_third_party_firewall()  # (2)
    ```

    1. client: [FMSClient](./client.md)
    2. result: [:material-code-braces: AssociateThirdPartyFirewallResponseTypeDef](./type_defs.md#associatethirdpartyfirewallresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("fms") as client:  # (1)
        paginator = client.get_paginator("list_apps_lists")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [FMSClient](./client.md)
    2. paginator: [ListAppsListsPaginator](./paginators.md#listappslistspaginator)
    3. item: [:material-code-braces: ListAppsListsResponseTypeDef](./type_defs.md#listappslistsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[fms]`
or a standalone `types_aiobotocore_fms` package, you have to explicitly specify
`client: FMSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_fms.client import FMSClient
    from types_aiobotocore_fms.type_defs import AssociateThirdPartyFirewallResponseTypeDef
    from types_aiobotocore_fms.type_defs import AssociateThirdPartyFirewallRequestRequestTypeDef


    session = get_session()

    async with session.create_client("fms") as client:
        client: FMSClient
        kwargs: AssociateThirdPartyFirewallRequestRequestTypeDef = {...}
        result: AssociateThirdPartyFirewallResponseTypeDef = await client.associate_third_party_firewall(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_fms.client import FMSClient
    from types_aiobotocore_fms.paginator import ListAppsListsPaginator
    from types_aiobotocore_fms.type_defs import ListAppsListsResponseTypeDef


    session = get_session()

    async with session.create_client("fms") as client:
        client: FMSClient
        paginator: ListAppsListsPaginator = client.get_paginator("list_apps_lists")
        async for item in paginator.paginate(...):
            item: ListAppsListsResponseTypeDef
            print(item)
    ```


