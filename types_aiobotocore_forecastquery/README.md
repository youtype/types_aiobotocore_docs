<a id="type-annotations-for-aiobotocore-forecastqueryservice-module"></a>

# Type annotations for aiobotocore ForecastQueryService module

> [Index](..) > ForecastQueryService

Auto-generated documentation for
[ForecastQueryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
type annotations stubs module
[types-aiobotocore-forecastquery](https://pypi.org/project/types-aiobotocore-forecastquery/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[forecastquery]'

# Lite version does not provide session.create_client overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[forecastquery]'

# standalone installation
pip install types-aiobotocore-forecastquery
```

- [Type annotations for aiobotocore ForecastQueryService module](#type-annotations-for-aiobotocore-forecastqueryservice-module)
  - [ForecastQueryServiceClient](#forecastqueryserviceclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="forecastqueryserviceclient"></a>

## ForecastQueryServiceClient

Type annotations for `session.create_client("forecastquery")` as
[ForecastQueryServiceClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_forecastquery.client import ForecastQueryServiceClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [query_forecast](./client.md#query_forecast)

<a id="exceptions"></a>

### Exceptions

ForecastQueryServiceClient [exceptions](./client.md#exceptions)

- ClientError
- InvalidInputException
- InvalidNextTokenException
- LimitExceededException
- ResourceInUseException
- ResourceNotFoundException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_forecastquery.literals import ServiceName, ...
```

- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_forecastquery.type_defs import DataPointTypeDef, ...
```

- [DataPointTypeDef](./type_defs.md#datapointtypedef)
- [ForecastTypeDef](./type_defs.md#forecasttypedef)
- [QueryForecastRequestRequestTypeDef](./type_defs.md#queryforecastrequestrequesttypedef)
- [QueryForecastResponseTypeDef](./type_defs.md#queryforecastresponsetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
