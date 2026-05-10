# Examples

> [Index](../README.md) > [Sustainability](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Sustainability](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability.html#sustainability)
    type annotations stubs module [types-aiobotocore-sustainability](https://pypi.org/project/types-aiobotocore-sustainability/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sustainability]` package installed.

Write your `Sustainability` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SustainabilityClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sustainability") as client:  # (1)
    result = await client.get_estimated_carbon_emissions()  # (2)
```

1. client: [SustainabilityClient](./client.md)
2. result: [:material-code-braces: GetEstimatedCarbonEmissionsResponseTypeDef](./type_defs.md#getestimatedcarbonemissionsresponsetypedef)



#### Paginator usage example

```python
# GetEstimatedCarbonEmissionsDimensionValuesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sustainability") as client:  # (1)
    paginator = client.get_paginator("get_estimated_carbon_emissions_dimension_values")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SustainabilityClient](./client.md)
2. paginator: [GetEstimatedCarbonEmissionsDimensionValuesPaginator](./paginators.md#getestimatedcarbonemissionsdimensionvaluespaginator)
3. item: [:material-code-braces: GetEstimatedCarbonEmissionsDimensionValuesResponseTypeDef](./type_defs.md#getestimatedcarbonemissionsdimensionvaluesresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[sustainability]`
or a standalone `types_aiobotocore_sustainability` package, you have to explicitly specify
`client: SustainabilityClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SustainabilityClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sustainability.client import SustainabilityClient
from types_aiobotocore_sustainability.type_defs import GetEstimatedCarbonEmissionsResponseTypeDef
from types_aiobotocore_sustainability.type_defs import GetEstimatedCarbonEmissionsRequestTypeDef


session = get_session()

async with session.create_client("sustainability") as client:
    client: SustainabilityClient
    kwargs: GetEstimatedCarbonEmissionsRequestTypeDef = {...}
    result: GetEstimatedCarbonEmissionsResponseTypeDef = await client.get_estimated_carbon_emissions(**kwargs)
```



#### Paginator usage example

```python
# GetEstimatedCarbonEmissionsDimensionValuesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sustainability.client import SustainabilityClient
from types_aiobotocore_sustainability.paginator import GetEstimatedCarbonEmissionsDimensionValuesPaginator
from types_aiobotocore_sustainability.type_defs import GetEstimatedCarbonEmissionsDimensionValuesResponseTypeDef


session = get_session()

async with session.create_client("sustainability") as client:
    client: SustainabilityClient
    paginator: GetEstimatedCarbonEmissionsDimensionValuesPaginator = client.get_paginator("get_estimated_carbon_emissions_dimension_values")
    async for item in paginator.paginate(...):
        item: GetEstimatedCarbonEmissionsDimensionValuesResponseTypeDef
        print(item)
```


