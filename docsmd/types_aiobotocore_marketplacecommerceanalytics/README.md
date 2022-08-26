# MarketplaceCommerceAnalytics module

> [Index](../README.md) > MarketplaceCommerceAnalytics


!!! note ""

    Auto-generated documentation for [MarketplaceCommerceAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
    type annotations stubs module [types-aiobotocore-marketplacecommerceanalytics](https://pypi.org/project/types-aiobotocore-marketplacecommerceanalytics/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `MarketplaceCommerceAnalytics` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[marketplacecommerceanalytics]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[marketplacecommerceanalytics]'


# standalone installation
python -m pip install types-aiobotocore-marketplacecommerceanalytics
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-marketplacecommerceanalytics
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MarketplaceCommerceAnalyticsClient

Type annotations and code completion for  `#!python session.create_client("marketplacecommerceanalytics")` as [MarketplaceCommerceAnalyticsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_marketplacecommerceanalytics.client import MarketplaceCommerceAnalyticsClient


session = get_session()
async with session.create_client("marketplacecommerceanalytics") as client:
    client: MarketplaceCommerceAnalyticsClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_marketplacecommerceanalytics.literals import DataSetTypeType

def get_value() -> DataSetTypeType:
    return "customer_profile_by_geography"
```

- [DataSetTypeType](./literals.md#datasettypetype)
- [SupportDataSetTypeType](./literals.md#supportdatasettypetype)
- [MarketplaceCommerceAnalyticsServiceName](./literals.md#marketplacecommerceanalyticsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_marketplacecommerceanalytics.type_defs import GenerateDataSetRequestRequestTypeDef

def get_value() -> GenerateDataSetRequestRequestTypeDef:
    return {
        "dataSetType": ...,
        "dataSetPublicationDate": ...,
        "roleNameArn": ...,
        "destinationS3BucketName": ...,
        "snsTopicArn": ...,
    }
```

- [GenerateDataSetRequestRequestTypeDef](./type_defs.md#generatedatasetrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [StartSupportDataExportRequestRequestTypeDef](./type_defs.md#startsupportdataexportrequestrequesttypedef)
- [GenerateDataSetResultTypeDef](./type_defs.md#generatedatasetresulttypedef)
- [StartSupportDataExportResultTypeDef](./type_defs.md#startsupportdataexportresulttypedef)

