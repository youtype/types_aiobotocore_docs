# ForecastQueryService module

> [Index](../README.md) > ForecastQueryService


!!! note ""

    Auto-generated documentation for [ForecastQueryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#forecastqueryservice)
    type annotations stubs module [types-aiobotocore-forecastquery](https://pypi.org/project/types-aiobotocore-forecastquery/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ForecastQueryService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ForecastQueryService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[forecastquery]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[forecastquery]'

# standalone installation
python -m pip install types-aiobotocore-forecastquery
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-forecastquery
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ForecastQueryServiceClient

Type annotations and code completion for  `#!python session.create_client("forecastquery")` as [ForecastQueryServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client)

```python
# ForecastQueryServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecastquery.client import ForecastQueryServiceClient


session = get_session()
async with session.create_client("forecastquery") as client:
    client: ForecastQueryServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ForecastQueryServiceServiceName usage example

from types_aiobotocore_forecastquery.literals import ForecastQueryServiceServiceName

def get_value() -> ForecastQueryServiceServiceName:
    return "forecastquery"
```

- [ForecastQueryServiceServiceName](./literals.md#forecastqueryserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [DataPointTypeDef](./type_defs.md#datapointtypedef)
- [QueryForecastRequestTypeDef](./type_defs.md#queryforecastrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [QueryWhatIfForecastRequestTypeDef](./type_defs.md#querywhatifforecastrequesttypedef)
- [ForecastTypeDef](./type_defs.md#forecasttypedef)
- [QueryForecastResponseTypeDef](./type_defs.md#queryforecastresponsetypedef)
- [QueryWhatIfForecastResponseTypeDef](./type_defs.md#querywhatifforecastresponsetypedef)

