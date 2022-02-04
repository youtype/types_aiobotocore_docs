<a id="type-annotations-for-aiobotocore-marketplacecommerceanalytics-module"></a>

# Type annotations for aiobotocore MarketplaceCommerceAnalytics module

> [Index](..) > MarketplaceCommerceAnalytics

Auto-generated documentation for
[MarketplaceCommerceAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
type annotations stubs module
[types-aiobotocore-marketplacecommerceanalytics](https://pypi.org/project/types-aiobotocore-marketplacecommerceanalytics/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[marketplacecommerceanalytics]'

# install as a standalone
pip install types-aiobotocore-marketplacecommerceanalytics
```

- [Type annotations for aiobotocore MarketplaceCommerceAnalytics module](#type-annotations-for-aiobotocore-marketplacecommerceanalytics-module)
  - [MarketplaceCommerceAnalyticsClient](#marketplacecommerceanalyticsclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="marketplacecommerceanalyticsclient"></a>

## MarketplaceCommerceAnalyticsClient

Type annotations for
`aiobotocore.create_client("marketplacecommerceanalytics")` as
[MarketplaceCommerceAnalyticsClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_marketplacecommerceanalytics.client import MarketplaceCommerceAnalyticsClient
```

<a id="methods"></a>

### Methods

- [can_paginate](./client.md#can_paginate)
- [exceptions](./client.md#exceptions)
- [generate_data_set](./client.md#generate_data_set)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [start_support_data_export](./client.md#start_support_data_export)

<a id="exceptions"></a>

### Exceptions

MarketplaceCommerceAnalyticsClient [exceptions](./client.md#exceptions)

- ClientError
- MarketplaceCommerceAnalyticsException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_marketplacecommerceanalytics.literals import DataSetTypeType, ...
```

- [DataSetTypeType](./literals.md#datasettypetype)
- [SupportDataSetTypeType](./literals.md#supportdatasettypetype)
- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_marketplacecommerceanalytics.type_defs import GenerateDataSetRequestRequestTypeDef, ...
```

- [GenerateDataSetRequestRequestTypeDef](./type_defs.md#generatedatasetrequestrequesttypedef)
- [GenerateDataSetResultTypeDef](./type_defs.md#generatedatasetresulttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [StartSupportDataExportRequestRequestTypeDef](./type_defs.md#startsupportdataexportrequestrequesttypedef)
- [StartSupportDataExportResultTypeDef](./type_defs.md#startsupportdataexportresulttypedef)
