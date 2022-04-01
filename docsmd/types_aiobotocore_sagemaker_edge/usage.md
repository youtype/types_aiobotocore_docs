# Examples

> [Index](../README.md) > [SagemakerEdgeManager](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SagemakerEdgeManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
    type annotations stubs module [types-aiobotocore-sagemaker-edge](https://pypi.org/project/types-aiobotocore-sagemaker-edge/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sagemaker-edge]` package installed.

Write your `SagemakerEdgeManager` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("sagemaker-edge") as client:  # (1)
        result = await client.get_device_registration()  # (2)
    ```

    1. client: [SagemakerEdgeManagerClient](./client.md)
    2. result: [:material-code-braces: GetDeviceRegistrationResultTypeDef](./type_defs.md#getdeviceregistrationresulttypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[sagemaker-edge]`
or a standalone `types_aiobotocore_sagemaker_edge` package, you have to explicitly specify
`client: SagemakerEdgeManagerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_sagemaker_edge.client import SagemakerEdgeManagerClient
    from types_aiobotocore_sagemaker_edge.type_defs import GetDeviceRegistrationResultTypeDef
    from types_aiobotocore_sagemaker_edge.type_defs import GetDeviceRegistrationRequestRequestTypeDef


    session = get_session()

    async with session.create_client("sagemaker-edge") as client:
        client: SagemakerEdgeManagerClient
        kwargs: GetDeviceRegistrationRequestRequestTypeDef = {...}
        result: GetDeviceRegistrationResultTypeDef = await client.get_device_registration(**kwargs)
    ```




