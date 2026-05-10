# Paginators

> [Index](../README.md) > [Sustainability](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Sustainability](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability.html#sustainability)
    type annotations stubs module [types-aiobotocore-sustainability](https://pypi.org/project/types-aiobotocore-sustainability/).

## GetEstimatedCarbonEmissionsDimensionValuesPaginator

Type annotations and code completion for `#!python session.create_client("sustainability").get_paginator("get_estimated_carbon_emissions_dimension_values")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability/paginator/GetEstimatedCarbonEmissionsDimensionValues.html#Sustainability.Paginator.GetEstimatedCarbonEmissionsDimensionValues)

```python
# GetEstimatedCarbonEmissionsDimensionValuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sustainability.paginator import GetEstimatedCarbonEmissionsDimensionValuesPaginator

session = get_session()
async with session.create_client("sustainability") as client:  # (1)
    paginator: GetEstimatedCarbonEmissionsDimensionValuesPaginator = client.get_paginator("get_estimated_carbon_emissions_dimension_values")  # (2)
    async for item in paginator.paginate(...):
        item: GetEstimatedCarbonEmissionsDimensionValuesResponseTypeDef
        print(item)  # (3)
```

1. client: [SustainabilityClient](./client.md)
2. paginator: [GetEstimatedCarbonEmissionsDimensionValuesPaginator](./paginators.md#getestimatedcarbonemissionsdimensionvaluespaginator)
3. item: `AioPageIterator[GetEstimatedCarbonEmissionsDimensionValuesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetEstimatedCarbonEmissionsDimensionValuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TimePeriod: TimePeriodUnionTypeDef,  # (1)
    Dimensions: Sequence[DimensionType],  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[GetEstimatedCarbonEmissionsDimensionValuesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: TimePeriodUnionTypeDef](#timeperioduniontypedef)
2. See `Sequence[DimensionType]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[GetEstimatedCarbonEmissionsDimensionValuesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetEstimatedCarbonEmissionsDimensionValuesRequestPaginateTypeDef = {  # (1)
    "TimePeriod": ...,
    "Dimensions": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetEstimatedCarbonEmissionsDimensionValuesRequestPaginateTypeDef](./type_defs.md#getestimatedcarbonemissionsdimensionvaluesrequestpaginatetypedef)
## GetEstimatedCarbonEmissionsPaginator

Type annotations and code completion for `#!python session.create_client("sustainability").get_paginator("get_estimated_carbon_emissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability/paginator/GetEstimatedCarbonEmissions.html#Sustainability.Paginator.GetEstimatedCarbonEmissions)

```python
# GetEstimatedCarbonEmissionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sustainability.paginator import GetEstimatedCarbonEmissionsPaginator

session = get_session()
async with session.create_client("sustainability") as client:  # (1)
    paginator: GetEstimatedCarbonEmissionsPaginator = client.get_paginator("get_estimated_carbon_emissions")  # (2)
    async for item in paginator.paginate(...):
        item: GetEstimatedCarbonEmissionsResponseTypeDef
        print(item)  # (3)
```

1. client: [SustainabilityClient](./client.md)
2. paginator: [GetEstimatedCarbonEmissionsPaginator](./paginators.md#getestimatedcarbonemissionspaginator)
3. item: `AioPageIterator[GetEstimatedCarbonEmissionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetEstimatedCarbonEmissionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TimePeriod: TimePeriodUnionTypeDef,  # (1)
    GroupBy: Sequence[DimensionType] = ...,  # (2)
    FilterBy: FilterExpressionTypeDef = ...,  # (3)
    EmissionsTypes: Sequence[EmissionsTypeType] = ...,  # (4)
    Granularity: TimeGranularityType = ...,  # (5)
    GranularityConfiguration: GranularityConfigurationTypeDef = ...,  # (6)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (7)
) -> aiobotocore.paginate.AioPageIterator[GetEstimatedCarbonEmissionsResponseTypeDef]:  # (8)
    ...
```

1. See [:material-code-braces: TimePeriodUnionTypeDef](#timeperioduniontypedef)
2. See `Sequence[DimensionType]`
3. See [:material-code-braces: FilterExpressionTypeDef](./type_defs.md#filterexpressiontypedef)
4. See `Sequence[EmissionsTypeType]`
5. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype)
6. See [:material-code-braces: GranularityConfigurationTypeDef](./type_defs.md#granularityconfigurationtypedef)
7. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
8. See `AioPageIterator[GetEstimatedCarbonEmissionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetEstimatedCarbonEmissionsRequestPaginateTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetEstimatedCarbonEmissionsRequestPaginateTypeDef](./type_defs.md#getestimatedcarbonemissionsrequestpaginatetypedef)
