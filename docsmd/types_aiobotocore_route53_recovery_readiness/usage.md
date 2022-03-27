# Examples

> [Index](../README.md) > [Route53RecoveryReadiness](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Route53RecoveryReadiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
    type annotations stubs module [types-aiobotocore-route53-recovery-readiness](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[route53-recovery-readiness]` package installed.

Write your `Route53RecoveryReadiness` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("route53-recovery-readiness") as client:  # (1)
        result = await client.create_cell()  # (2)
    ```

    1. client: [Route53RecoveryReadinessClient](./client.md)
    2. result: [:material-code-braces: CreateCellResponseTypeDef](./type_defs.md#createcellresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("route53-recovery-readiness") as client:  # (1)
        paginator = client.get_paginator("get_cell_readiness_summary")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [Route53RecoveryReadinessClient](./client.md)
    2. paginator: [GetCellReadinessSummaryPaginator](./paginators.md#getcellreadinesssummarypaginator)
    3. item: [:material-code-braces: GetCellReadinessSummaryResponseTypeDef](./type_defs.md#getcellreadinesssummaryresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[route53-recovery-readiness]`
or a standalone `types_aiobotocore_route53_recovery_readiness` package, you have to explicitly specify
`client: Route53RecoveryReadinessClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_route53_recovery_readiness.client import Route53RecoveryReadinessClient
    from types_aiobotocore_route53_recovery_readiness.type_defs import CreateCellResponseTypeDef
    from types_aiobotocore_route53_recovery_readiness.type_defs import CreateCellRequestRequestTypeDef


    session = get_session()

    async with session.create_client("route53-recovery-readiness") as client:
        client: Route53RecoveryReadinessClient
        kwargs: CreateCellRequestRequestTypeDef = {...}
        result: CreateCellResponseTypeDef = await client.create_cell(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_route53_recovery_readiness.client import Route53RecoveryReadinessClient
    from types_aiobotocore_route53_recovery_readiness.paginator import GetCellReadinessSummaryPaginator
    from types_aiobotocore_route53_recovery_readiness.type_defs import GetCellReadinessSummaryResponseTypeDef


    session = get_session()

    async with session.create_client("route53-recovery-readiness") as client:
        client: Route53RecoveryReadinessClient
        paginator: GetCellReadinessSummaryPaginator = client.get_paginator("get_cell_readiness_summary")
        async for item in paginator.paginate(...):
            item: GetCellReadinessSummaryResponseTypeDef
            print(item)
    ```


