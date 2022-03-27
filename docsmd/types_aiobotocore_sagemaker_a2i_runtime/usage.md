# Examples

> [Index](../README.md) > [AugmentedAIRuntime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AugmentedAIRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
    type annotations stubs module [types-aiobotocore-sagemaker-a2i-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sagemaker-a2i-runtime]` package installed.

Write your `AugmentedAIRuntime` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("sagemaker-a2i-runtime") as client:  # (1)
        result = await client.describe_human_loop()  # (2)
    ```

    1. client: [AugmentedAIRuntimeClient](./client.md)
    2. result: [:material-code-braces: DescribeHumanLoopResponseTypeDef](./type_defs.md#describehumanloopresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("sagemaker-a2i-runtime") as client:  # (1)
        paginator = client.get_paginator("list_human_loops")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [AugmentedAIRuntimeClient](./client.md)
    2. paginator: [ListHumanLoopsPaginator](./paginators.md#listhumanloopspaginator)
    3. item: [:material-code-braces: ListHumanLoopsResponseTypeDef](./type_defs.md#listhumanloopsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[sagemaker-a2i-runtime]`
or a standalone `types_aiobotocore_sagemaker_a2i_runtime` package, you have to explicitly specify
`client: AugmentedAIRuntimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_sagemaker_a2i_runtime.client import AugmentedAIRuntimeClient
    from types_aiobotocore_sagemaker_a2i_runtime.type_defs import DescribeHumanLoopResponseTypeDef
    from types_aiobotocore_sagemaker_a2i_runtime.type_defs import DescribeHumanLoopRequestRequestTypeDef


    session = get_session()

    async with session.create_client("sagemaker-a2i-runtime") as client:
        client: AugmentedAIRuntimeClient
        kwargs: DescribeHumanLoopRequestRequestTypeDef = {...}
        result: DescribeHumanLoopResponseTypeDef = await client.describe_human_loop(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_sagemaker_a2i_runtime.client import AugmentedAIRuntimeClient
    from types_aiobotocore_sagemaker_a2i_runtime.paginator import ListHumanLoopsPaginator
    from types_aiobotocore_sagemaker_a2i_runtime.type_defs import ListHumanLoopsResponseTypeDef


    session = get_session()

    async with session.create_client("sagemaker-a2i-runtime") as client:
        client: AugmentedAIRuntimeClient
        paginator: ListHumanLoopsPaginator = client.get_paginator("list_human_loops")
        async for item in paginator.paginate(...):
            item: ListHumanLoopsResponseTypeDef
            print(item)
    ```


