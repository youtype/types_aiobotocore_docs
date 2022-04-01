# Examples

> [Index](../README.md) > [ComputeOptimizer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ComputeOptimizer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
    type annotations stubs module [types-aiobotocore-compute-optimizer](https://pypi.org/project/types-aiobotocore-compute-optimizer/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[compute-optimizer]` package installed.

Write your `ComputeOptimizer` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("compute-optimizer") as client:  # (1)
        result = await client.describe_recommendation_export_jobs()  # (2)
    ```

    1. client: [ComputeOptimizerClient](./client.md)
    2. result: [:material-code-braces: DescribeRecommendationExportJobsResponseTypeDef](./type_defs.md#describerecommendationexportjobsresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[compute-optimizer]`
or a standalone `types_aiobotocore_compute_optimizer` package, you have to explicitly specify
`client: ComputeOptimizerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_compute_optimizer.client import ComputeOptimizerClient
    from types_aiobotocore_compute_optimizer.type_defs import DescribeRecommendationExportJobsResponseTypeDef
    from types_aiobotocore_compute_optimizer.type_defs import DescribeRecommendationExportJobsRequestRequestTypeDef


    session = get_session()

    async with session.create_client("compute-optimizer") as client:
        client: ComputeOptimizerClient
        kwargs: DescribeRecommendationExportJobsRequestRequestTypeDef = {...}
        result: DescribeRecommendationExportJobsResponseTypeDef = await client.describe_recommendation_export_jobs(**kwargs)
    ```




