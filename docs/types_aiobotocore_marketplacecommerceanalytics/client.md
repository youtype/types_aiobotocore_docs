<a id="marketplacecommerceanalyticsclient-for-aiobotocore-marketplacecommerceanalytics-module"></a>

# MarketplaceCommerceAnalyticsClient for aiobotocore MarketplaceCommerceAnalytics module

> [Index](../README.md) > [MarketplaceCommerceAnalytics](./README.md) >
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
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="marketplacecommerceanalyticsclient"></a>

## MarketplaceCommerceAnalyticsClient

Type annotations for `session.create_client("marketplacecommerceanalytics")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_marketplacecommerceanalytics.client import MarketplaceCommerceAnalyticsClient

session = get_session()
async with session.create_client("marketplacecommerceanalytics") as client:
    client: MarketplaceCommerceAnalyticsClient
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
`session.create_client("marketplacecommerceanalytics").exceptions` method.

Boto3 documentation:
[MarketplaceCommerceAnalytics.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`session.create_client("marketplacecommerceanalytics").can_paginate` method.

Boto3 documentation:
[MarketplaceCommerceAnalytics.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="generate\_data\_set"></a>

### generate_data_set

Given a data set type and data set publication date, asynchronously publishes
the requested data set to the specified S3 bucket and notifies the specified
SNS topic once the data is available.

Type annotations for
`session.create_client("marketplacecommerceanalytics").generate_data_set`
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

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("marketplacecommerceanalytics").generate_presigned_url`
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

<a id="start\_support\_data\_export"></a>

### start_support_data_export

Given a data set type and a from date, asynchronously publishes the requested
customer support data to the specified S3 bucket and notifies the specified SNS
topic once the data is available.

Type annotations for
`session.create_client("marketplacecommerceanalytics").start_support_data_export`
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

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for
`session.create_client("marketplacecommerceanalytics").__aenter__` method.

Boto3 documentation:
[MarketplaceCommerceAnalytics.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[MarketplaceCommerceAnalyticsClient](#marketplacecommerceanalyticsclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for
`session.create_client("marketplacecommerceanalytics").__aexit__` method.

Boto3 documentation:
[MarketplaceCommerceAnalytics.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
