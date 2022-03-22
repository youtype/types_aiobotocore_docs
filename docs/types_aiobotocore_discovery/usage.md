<a id="examples-for-aiobotocore-applicationdiscoveryservice-module"></a>

# Examples for aiobotocore ApplicationDiscoveryService module

> [Index](../README.md) > [ApplicationDiscoveryService](./README.md) > Examples

- [Examples for aiobotocore ApplicationDiscoveryService module](#examples-for-aiobotocore-applicationdiscoveryservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[discovery]` package installed.

Write your `ApplicationDiscoveryService` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ApplicationDiscoveryServiceClient
# and provides type checking and code completion
async with session.create_client("discovery") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_configuration_items_to_application()
    

    
    # paginator has type DescribeAgentsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_agents")
    async for item in paginator.paginate(...):
        # item has type DescribeAgentsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[discovery]` or a standalone
`types_aiobotocore_discovery` package, you have to explicitly specify
`client: ApplicationDiscoveryServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_discovery.client import ApplicationDiscoveryServiceClient
from types_aiobotocore_discovery.type_defs import Dict[str, Any]
from types_aiobotocore_discovery.paginator import DescribeAgentsPaginator

from types_aiobotocore_discovery.literals import PaginatorName



session = get_session()

async with session.create_client("discovery") as client:
    client: ApplicationDiscoveryServiceClient

    
    result: Dict[str, Any] = client.associate_configuration_items_to_application()
    

    
    paginator_name: PaginatorName = "describe_agents"
    paginator: DescribeAgentsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeAgentsResponseTypeDef
        print(item)
    

    
```
