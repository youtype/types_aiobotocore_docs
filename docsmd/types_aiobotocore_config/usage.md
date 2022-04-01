# Examples

> [Index](../README.md) > [ConfigService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ConfigService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
    type annotations stubs module [types-aiobotocore-config](https://pypi.org/project/types-aiobotocore-config/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[config]` package installed.

Write your `ConfigService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("config") as client:  # (1)
        result = await client.batch_get_aggregate_resource_config()  # (2)
    ```

    1. client: [ConfigServiceClient](./client.md)
    2. result: [:material-code-braces: BatchGetAggregateResourceConfigResponseTypeDef](./type_defs.md#batchgetaggregateresourceconfigresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("config") as client:  # (1)
        paginator = client.get_paginator("describe_aggregate_compliance_by_config_rules")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ConfigServiceClient](./client.md)
    2. paginator: [DescribeAggregateComplianceByConfigRulesPaginator](./paginators.md#describeaggregatecompliancebyconfigrulespaginator)
    3. item: [:material-code-braces: DescribeAggregateComplianceByConfigRulesResponseTypeDef](./type_defs.md#describeaggregatecompliancebyconfigrulesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[config]`
or a standalone `types_aiobotocore_config` package, you have to explicitly specify
`client: ConfigServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_config.client import ConfigServiceClient
    from types_aiobotocore_config.type_defs import BatchGetAggregateResourceConfigResponseTypeDef
    from types_aiobotocore_config.type_defs import BatchGetAggregateResourceConfigRequestRequestTypeDef


    session = get_session()

    async with session.create_client("config") as client:
        client: ConfigServiceClient
        kwargs: BatchGetAggregateResourceConfigRequestRequestTypeDef = {...}
        result: BatchGetAggregateResourceConfigResponseTypeDef = await client.batch_get_aggregate_resource_config(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_config.client import ConfigServiceClient
    from types_aiobotocore_config.paginator import DescribeAggregateComplianceByConfigRulesPaginator
    from types_aiobotocore_config.type_defs import DescribeAggregateComplianceByConfigRulesResponseTypeDef


    session = get_session()

    async with session.create_client("config") as client:
        client: ConfigServiceClient
        paginator: DescribeAggregateComplianceByConfigRulesPaginator = client.get_paginator("describe_aggregate_compliance_by_config_rules")
        async for item in paginator.paginate(...):
            item: DescribeAggregateComplianceByConfigRulesResponseTypeDef
            print(item)
    ```


