<a id="marketplacecommerceanalyticsclient-for-aiobotocore-marketplacecommerceanalytics-module"></a>

# MarketplaceCommerceAnalyticsClient for aiobotocore MarketplaceCommerceAnalytics module

> [Index](..) > [MarketplaceCommerceAnalytics](.) >
> MarketplaceCommerceAnalyticsClient

Auto-generated documentation for
[MarketplaceCommerceAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
type annotations stubs module
[types-aiobotocore-marketplacecommerceanalytics](https://pypi.org/project/types-aiobotocore-marketplacecommerceanalytics/).

- [MarketplaceCommerceAnalyticsClient for aiobotocore MarketplaceCommerceAnalytics module](#marketplacecommerceanalyticsclient-for-aiobotocore-marketplacecommerceanalytics-module)
  - [MarketplaceCommerceAnalyticsClient](#marketplacecommerceanalyticsclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [generate_data_set](#generate_data_set)
    - [generate_presigned_url](#generate_presigned_url)
    - [start_support_data_export](#start_support_data_export)

<a id="marketplacecommerceanalyticsclient"></a>

## MarketplaceCommerceAnalyticsClient

Type annotations for
`aiobotocore.create_client("marketplacecommerceanalytics")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_marketplacecommerceanalytics.client import MarketplaceCommerceAnalyticsClient

def get_marketplacecommerceanalytics_client() -> MarketplaceCommerceAnalyticsClient:
    return Session().client("marketplacecommerceanalytics")
```

Boto3 documentation:
[MarketplaceCommerceAnalytics.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_marketplacecommerceanalytics.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.MarketplaceCommerceAnalyticsException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

MarketplaceCommerceAnalyticsClient exceptions.

Type annotations for
`aiobotocore.create_client("marketplacecommerceanalytics").exceptions` method.

Boto3 documentation:
[MarketplaceCommerceAnalytics.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`aiobotocore.create_client("marketplacecommerceanalytics").can_paginate`
method.

Boto3 documentation:
[MarketplaceCommerceAnalytics.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="generate_data_set"></a>

### generate_data_set

Given a data set type and data set publication date, asynchronously publishes
the requested data set to the specified S3 bucket and notifies the specified
SNS topic once the data is available.

Type annotations for
`aiobotocore.create_client("marketplacecommerceanalytics").generate_data_set`
method.

Boto3 documentation:
[MarketplaceCommerceAnalytics.Client.generate_data_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client.generate_data_set)

Asynchronous method. Use `await generate_data_set(...)` for a synchronous call.

Arguments mapping described in
[GenerateDataSetRequestRequestTypeDef](./type_defs.md#generatedatasetrequestrequesttypedef).

Keyword-only arguments:

- `dataSetType`: [DataSetTypeType](./literals.md#datasettypetype) *(required)*
- `dataSetPublicationDate`: `Union`\[`datetime`, `str`\] *(required)*
- `roleNameArn`: `str` *(required)*
- `destinationS3BucketName`: `str` *(required)*
- `snsTopicArn`: `str` *(required)*
- `destinationS3Prefix`: `str`
- `customerDefinedValues`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[GenerateDataSetResultTypeDef](./type_defs.md#generatedatasetresulttypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("marketplacecommerceanalytics").generate_presigned_url`
method.

Boto3 documentation:
[MarketplaceCommerceAnalytics.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="start_support_data_export"></a>

### start_support_data_export

Given a data set type and a from date, asynchronously publishes the requested
customer support data to the specified S3 bucket and notifies the specified SNS
topic once the data is available.

Type annotations for
`aiobotocore.create_client("marketplacecommerceanalytics").start_support_data_export`
method.

Boto3 documentation:
[MarketplaceCommerceAnalytics.Client.start_support_data_export](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client.start_support_data_export)

Asynchronous method. Use `await start_support_data_export(...)` for a
synchronous call.

Arguments mapping described in
[StartSupportDataExportRequestRequestTypeDef](./type_defs.md#startsupportdataexportrequestrequesttypedef).

Keyword-only arguments:

- `dataSetType`: [SupportDataSetTypeType](./literals.md#supportdatasettypetype)
  *(required)*
- `fromDate`: `Union`\[`datetime`, `str`\] *(required)*
- `roleNameArn`: `str` *(required)*
- `destinationS3BucketName`: `str` *(required)*
- `snsTopicArn`: `str` *(required)*
- `destinationS3Prefix`: `str`
- `customerDefinedValues`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[StartSupportDataExportResultTypeDef](./type_defs.md#startsupportdataexportresulttypedef).
