# Examples

> [Index](../README.md) > [ResilienceHub](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ResilienceHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
    type annotations stubs module [types-aiobotocore-resiliencehub](https://pypi.org/project/types-aiobotocore-resiliencehub/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[resiliencehub]` package installed.

Write your `ResilienceHub` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("resiliencehub") as client:  # (1)
        result = await client.add_draft_app_version_resource_mappings()  # (2)
    ```

    1. client: [ResilienceHubClient](./client.md)
    2. result: [:material-code-braces: AddDraftAppVersionResourceMappingsResponseTypeDef](./type_defs.md#adddraftappversionresourcemappingsresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[resiliencehub]`
or a standalone `types_aiobotocore_resiliencehub` package, you have to explicitly specify
`client: ResilienceHubClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_resiliencehub.client import ResilienceHubClient
    from types_aiobotocore_resiliencehub.type_defs import AddDraftAppVersionResourceMappingsResponseTypeDef
    from types_aiobotocore_resiliencehub.type_defs import AddDraftAppVersionResourceMappingsRequestRequestTypeDef


    session = get_session()

    async with session.create_client("resiliencehub") as client:
        client: ResilienceHubClient
        kwargs: AddDraftAppVersionResourceMappingsRequestRequestTypeDef = {...}
        result: AddDraftAppVersionResourceMappingsResponseTypeDef = await client.add_draft_app_version_resource_mappings(**kwargs)
    ```




