# Examples

> [Index](../README.md) > [IoT](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoT](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
    type annotations stubs module [types-aiobotocore-iot](https://pypi.org/project/types-aiobotocore-iot/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iot]` package installed.

Write your `IoT` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("iot") as client:  # (1)
        result = await client.associate_targets_with_job()  # (2)
    ```

    1. client: [IoTClient](./client.md)
    2. result: [:material-code-braces: AssociateTargetsWithJobResponseTypeDef](./type_defs.md#associatetargetswithjobresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("iot") as client:  # (1)
        paginator = client.get_paginator("get_behavior_model_training_summaries")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [IoTClient](./client.md)
    2. paginator: [GetBehaviorModelTrainingSummariesPaginator](./paginators.md#getbehaviormodeltrainingsummariespaginator)
    3. item: [:material-code-braces: GetBehaviorModelTrainingSummariesResponseTypeDef](./type_defs.md#getbehaviormodeltrainingsummariesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[iot]`
or a standalone `types_aiobotocore_iot` package, you have to explicitly specify
`client: IoTClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_iot.client import IoTClient
    from types_aiobotocore_iot.type_defs import AssociateTargetsWithJobResponseTypeDef
    from types_aiobotocore_iot.type_defs import AssociateTargetsWithJobRequestRequestTypeDef


    session = get_session()

    async with session.create_client("iot") as client:
        client: IoTClient
        kwargs: AssociateTargetsWithJobRequestRequestTypeDef = {...}
        result: AssociateTargetsWithJobResponseTypeDef = await client.associate_targets_with_job(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_iot.client import IoTClient
    from types_aiobotocore_iot.paginator import GetBehaviorModelTrainingSummariesPaginator
    from types_aiobotocore_iot.type_defs import GetBehaviorModelTrainingSummariesResponseTypeDef


    session = get_session()

    async with session.create_client("iot") as client:
        client: IoTClient
        paginator: GetBehaviorModelTrainingSummariesPaginator = client.get_paginator("get_behavior_model_training_summaries")
        async for item in paginator.paginate(...):
            item: GetBehaviorModelTrainingSummariesResponseTypeDef
            print(item)
    ```


