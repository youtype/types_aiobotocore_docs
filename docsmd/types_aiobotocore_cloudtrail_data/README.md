# CloudTrailDataService module

> [Index](../README.md) > CloudTrailDataService


!!! note ""

    Auto-generated documentation for [CloudTrailDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#cloudtraildataservice)
    type annotations stubs module [types-aiobotocore-cloudtrail-data](https://pypi.org/project/types-aiobotocore-cloudtrail-data/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudTrailDataService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CloudTrailDataService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cloudtrail-data]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cloudtrail-data]'

# standalone installation
python -m pip install types-aiobotocore-cloudtrail-data
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cloudtrail-data
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudTrailDataServiceClient

Type annotations and code completion for  `#!python session.create_client("cloudtrail-data")` as [CloudTrailDataServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService.Client)

```python
# CloudTrailDataServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail_data.client import CloudTrailDataServiceClient


session = get_session()
async with session.create_client("cloudtrail-data") as client:
    client: CloudTrailDataServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CloudTrailDataServiceServiceName usage example

from types_aiobotocore_cloudtrail_data.literals import CloudTrailDataServiceServiceName

def get_value() -> CloudTrailDataServiceServiceName:
    return "cloudtrail-data"
```

- [CloudTrailDataServiceServiceName](./literals.md#cloudtraildataserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AuditEventResultEntryTypeDef](./type_defs.md#auditeventresultentrytypedef)
- [AuditEventTypeDef](./type_defs.md#auditeventtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ResultErrorEntryTypeDef](./type_defs.md#resulterrorentrytypedef)
- [PutAuditEventsRequestTypeDef](./type_defs.md#putauditeventsrequesttypedef)
- [PutAuditEventsResponseTypeDef](./type_defs.md#putauditeventsresponsetypedef)

