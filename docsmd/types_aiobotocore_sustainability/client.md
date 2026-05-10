# SustainabilityClient

> [Index](../README.md) > [Sustainability](./README.md) > SustainabilityClient

!!! note ""

    Auto-generated documentation for [Sustainability](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability.html#sustainability)
    type annotations stubs module [types-aiobotocore-sustainability](https://pypi.org/project/types-aiobotocore-sustainability/).

## SustainabilityClient

Type annotations and code completion for `#!python session.create_client("sustainability")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability.html#Sustainability.Client)

```python
# SustainabilityClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_sustainability.client import SustainabilityClient

session = get_session()
async with session.create_client("sustainability") as client:
    client: SustainabilityClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("sustainability").exceptions` structure.

```python
# SustainabilityClient.exceptions usage example

async with session.create_client("sustainability") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalServerException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# SustainabilityClient usage type checking example

from types_aiobotocore_sustainability.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("sustainability").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("sustainability").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_estimated\_carbon\_emissions

Returns estimated carbon emission values based on customer grouping and
filtering parameters.

Type annotations and code completion for `#!python session.create_client("sustainability").get_estimated_carbon_emissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability/client/get_estimated_carbon_emissions.html)

```python
# get_estimated_carbon_emissions method definition

await def get_estimated_carbon_emissions(
    self,
    *,
    TimePeriod: TimePeriodUnionTypeDef,  # (1)
    GroupBy: Sequence[DimensionType] = ...,  # (2)
    FilterBy: FilterExpressionTypeDef = ...,  # (3)
    EmissionsTypes: Sequence[EmissionsTypeType] = ...,  # (4)
    Granularity: TimeGranularityType = ...,  # (5)
    GranularityConfiguration: GranularityConfigurationTypeDef = ...,  # (6)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetEstimatedCarbonEmissionsResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: TimePeriodUnionTypeDef](#timeperioduniontypedef)
2. See `Sequence[DimensionType]`
3. See [:material-code-braces: FilterExpressionTypeDef](./type_defs.md#filterexpressiontypedef)
4. See `Sequence[EmissionsTypeType]`
5. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype)
6. See [:material-code-braces: GranularityConfigurationTypeDef](./type_defs.md#granularityconfigurationtypedef)
7. See [:material-code-braces: GetEstimatedCarbonEmissionsResponseTypeDef](./type_defs.md#getestimatedcarbonemissionsresponsetypedef)


```python
# get_estimated_carbon_emissions method usage example with argument unpacking

kwargs: GetEstimatedCarbonEmissionsRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_estimated_carbon_emissions(**kwargs)
```

1. See [:material-code-braces: GetEstimatedCarbonEmissionsRequestTypeDef](./type_defs.md#getestimatedcarbonemissionsrequesttypedef)

### get\_estimated\_carbon\_emissions\_dimension\_values

Returns the possible dimension values available for a customer's account.

Type annotations and code completion for `#!python session.create_client("sustainability").get_estimated_carbon_emissions_dimension_values` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability/client/get_estimated_carbon_emissions_dimension_values.html)

```python
# get_estimated_carbon_emissions_dimension_values method definition

await def get_estimated_carbon_emissions_dimension_values(
    self,
    *,
    TimePeriod: TimePeriodUnionTypeDef,  # (1)
    Dimensions: Sequence[DimensionType],  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetEstimatedCarbonEmissionsDimensionValuesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TimePeriodUnionTypeDef](#timeperioduniontypedef)
2. See `Sequence[DimensionType]`
3. See [:material-code-braces: GetEstimatedCarbonEmissionsDimensionValuesResponseTypeDef](./type_defs.md#getestimatedcarbonemissionsdimensionvaluesresponsetypedef)


```python
# get_estimated_carbon_emissions_dimension_values method usage example with argument unpacking

kwargs: GetEstimatedCarbonEmissionsDimensionValuesRequestTypeDef = {  # (1)
    "TimePeriod": ...,
    "Dimensions": ...,
}

parent.get_estimated_carbon_emissions_dimension_values(**kwargs)
```

1. See [:material-code-braces: GetEstimatedCarbonEmissionsDimensionValuesRequestTypeDef](./type_defs.md#getestimatedcarbonemissionsdimensionvaluesrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("sustainability").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability.html#Sustainability.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("sustainability").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability.html#Sustainability.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("sustainability").get_paginator` method with overloads.

- `client.get_paginator("get_estimated_carbon_emissions_dimension_values")` -> [GetEstimatedCarbonEmissionsDimensionValuesPaginator](./paginators.md#getestimatedcarbonemissionsdimensionvaluespaginator)
- `client.get_paginator("get_estimated_carbon_emissions")` -> [GetEstimatedCarbonEmissionsPaginator](./paginators.md#getestimatedcarbonemissionspaginator)



