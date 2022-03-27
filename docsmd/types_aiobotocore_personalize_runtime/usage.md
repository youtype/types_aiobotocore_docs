# Examples

> [Index](../README.md) > [PersonalizeRuntime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PersonalizeRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
    type annotations stubs module [types-aiobotocore-personalize-runtime](https://pypi.org/project/types-aiobotocore-personalize-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[personalize-runtime]` package installed.

Write your `PersonalizeRuntime` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("personalize-runtime") as client:  # (1)
        result = await client.get_personalized_ranking()  # (2)
    ```

    1. client: [PersonalizeRuntimeClient](./client.md)
    2. result: [:material-code-braces: GetPersonalizedRankingResponseTypeDef](./type_defs.md#getpersonalizedrankingresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[personalize-runtime]`
or a standalone `types_aiobotocore_personalize_runtime` package, you have to explicitly specify
`client: PersonalizeRuntimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_personalize_runtime.client import PersonalizeRuntimeClient
    from types_aiobotocore_personalize_runtime.type_defs import GetPersonalizedRankingResponseTypeDef
    from types_aiobotocore_personalize_runtime.type_defs import GetPersonalizedRankingRequestRequestTypeDef


    session = get_session()

    async with session.create_client("personalize-runtime") as client:
        client: PersonalizeRuntimeClient
        kwargs: GetPersonalizedRankingRequestRequestTypeDef = {...}
        result: GetPersonalizedRankingResponseTypeDef = await client.get_personalized_ranking(**kwargs)
    ```




