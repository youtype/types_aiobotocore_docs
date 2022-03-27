# Examples

> [Index](../README.md) > [SESV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SESV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
    type annotations stubs module [types-aiobotocore-sesv2](https://pypi.org/project/types-aiobotocore-sesv2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sesv2]` package installed.

Write your `SESV2` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("sesv2") as client:  # (1)
        result = await client.create_deliverability_test_report()  # (2)
    ```

    1. client: [SESV2Client](./client.md)
    2. result: [:material-code-braces: CreateDeliverabilityTestReportResponseTypeDef](./type_defs.md#createdeliverabilitytestreportresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[sesv2]`
or a standalone `types_aiobotocore_sesv2` package, you have to explicitly specify
`client: SESV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_sesv2.client import SESV2Client
    from types_aiobotocore_sesv2.type_defs import CreateDeliverabilityTestReportResponseTypeDef
    from types_aiobotocore_sesv2.type_defs import CreateDeliverabilityTestReportRequestRequestTypeDef


    session = get_session()

    async with session.create_client("sesv2") as client:
        client: SESV2Client
        kwargs: CreateDeliverabilityTestReportRequestRequestTypeDef = {...}
        result: CreateDeliverabilityTestReportResponseTypeDef = await client.create_deliverability_test_report(**kwargs)
    ```




