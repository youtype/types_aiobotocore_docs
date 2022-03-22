<a id="examples-for-aiobotocore-configservice-module"></a>

# Examples for aiobotocore ConfigService module

> [Index](../README.md) > [ConfigService](./README.md) > Examples

- [Examples for aiobotocore ConfigService module](#examples-for-aiobotocore-configservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[config]` package installed.

Write your `ConfigService` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ConfigServiceClient
# and provides type checking and code completion
async with session.create_client("config") as client:
    
    # result has type BatchGetAggregateResourceConfigResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_get_aggregate_resource_config()
    

    
    # paginator has type DescribeAggregateComplianceByConfigRulesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_aggregate_compliance_by_config_rules")
    async for item in paginator.paginate(...):
        # item has type DescribeAggregateComplianceByConfigRulesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[config]` or a standalone
`types_aiobotocore_config` package, you have to explicitly specify
`client: ConfigServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_config.client import ConfigServiceClient
from types_aiobotocore_config.type_defs import BatchGetAggregateResourceConfigResponseTypeDef
from types_aiobotocore_config.paginator import DescribeAggregateComplianceByConfigRulesPaginator

from types_aiobotocore_config.literals import PaginatorName



session = get_session()

async with session.create_client("config") as client:
    client: ConfigServiceClient

    
    result: BatchGetAggregateResourceConfigResponseTypeDef = client.batch_get_aggregate_resource_config()
    

    
    paginator_name: PaginatorName = "describe_aggregate_compliance_by_config_rules"
    paginator: DescribeAggregateComplianceByConfigRulesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeAggregateComplianceByConfigRulesResponseTypeDef
        print(item)
    

    
```
