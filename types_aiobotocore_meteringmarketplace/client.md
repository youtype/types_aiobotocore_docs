<a id="marketplacemeteringclient-for-aiobotocore-marketplacemetering-module"></a>

# MarketplaceMeteringClient for aiobotocore MarketplaceMetering module

> [Index](..) > [MarketplaceMetering](.) > MarketplaceMeteringClient

Auto-generated documentation for
[MarketplaceMetering](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
type annotations stubs module
[types-aiobotocore-meteringmarketplace](https://pypi.org/project/types-aiobotocore-meteringmarketplace/).

- [MarketplaceMeteringClient for aiobotocore MarketplaceMetering module](#marketplacemeteringclient-for-aiobotocore-marketplacemetering-module)
  - [MarketplaceMeteringClient](#marketplacemeteringclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [batch_meter_usage](#batch_meter_usage)
    - [can_paginate](#can_paginate)
    - [generate_presigned_url](#generate_presigned_url)
    - [meter_usage](#meter_usage)
    - [register_usage](#register_usage)
    - [resolve_customer](#resolve_customer)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)

<a id="marketplacemeteringclient"></a>

## MarketplaceMeteringClient

Type annotations for `session.create_client("meteringmarketplace")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_meteringmarketplace.client import MarketplaceMeteringClient

session = get_session()
async with session.create_client("meteringmarketplace") as client:
    client: MarketplaceMeteringClient
```

Boto3 documentation:
[MarketplaceMetering.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_meteringmarketplace.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.CustomerNotEntitledException`
- `Exceptions.DisabledApiException`
- `Exceptions.DuplicateRequestException`
- `Exceptions.ExpiredTokenException`
- `Exceptions.InternalServiceErrorException`
- `Exceptions.InvalidCustomerIdentifierException`
- `Exceptions.InvalidEndpointRegionException`
- `Exceptions.InvalidProductCodeException`
- `Exceptions.InvalidPublicKeyVersionException`
- `Exceptions.InvalidRegionException`
- `Exceptions.InvalidTagException`
- `Exceptions.InvalidTokenException`
- `Exceptions.InvalidUsageAllocationsException`
- `Exceptions.InvalidUsageDimensionException`
- `Exceptions.PlatformNotSupportedException`
- `Exceptions.ThrottlingException`
- `Exceptions.TimestampOutOfBoundsException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

MarketplaceMeteringClient exceptions.

Type annotations for `session.create_client("meteringmarketplace").exceptions`
method.

Boto3 documentation:
[MarketplaceMetering.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="batch_meter_usage"></a>

### batch_meter_usage

BatchMeterUsage is called from a SaaS application listed on the AWS Marketplace
to post metering records for a set of customers.

Type annotations for
`session.create_client("meteringmarketplace").batch_meter_usage` method.

Boto3 documentation:
[MarketplaceMetering.Client.batch_meter_usage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.batch_meter_usage)

Asynchronous method. Use `await batch_meter_usage(...)` for a synchronous call.

Arguments mapping described in
[BatchMeterUsageRequestRequestTypeDef](./type_defs.md#batchmeterusagerequestrequesttypedef).

Keyword-only arguments:

- `UsageRecords`:
  `Sequence`\[[UsageRecordTypeDef](./type_defs.md#usagerecordtypedef)\]
  *(required)*
- `ProductCode`: `str` *(required)*

Returns a `Coroutine` for
[BatchMeterUsageResultTypeDef](./type_defs.md#batchmeterusageresulttypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`session.create_client("meteringmarketplace").can_paginate` method.

Boto3 documentation:
[MarketplaceMetering.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("meteringmarketplace").generate_presigned_url` method.

Boto3 documentation:
[MarketplaceMetering.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="meter_usage"></a>

### meter_usage

API to emit metering records.

Type annotations for `session.create_client("meteringmarketplace").meter_usage`
method.

Boto3 documentation:
[MarketplaceMetering.Client.meter_usage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.meter_usage)

Asynchronous method. Use `await meter_usage(...)` for a synchronous call.

Arguments mapping described in
[MeterUsageRequestRequestTypeDef](./type_defs.md#meterusagerequestrequesttypedef).

Keyword-only arguments:

- `ProductCode`: `str` *(required)*
- `Timestamp`: `Union`\[`datetime`, `str`\] *(required)*
- `UsageDimension`: `str` *(required)*
- `UsageQuantity`: `int`
- `DryRun`: `bool`
- `UsageAllocations`:
  `Sequence`\[[UsageAllocationTypeDef](./type_defs.md#usageallocationtypedef)\]

Returns a `Coroutine` for
[MeterUsageResultTypeDef](./type_defs.md#meterusageresulttypedef).

<a id="register_usage"></a>

### register_usage

Paid container software products sold through AWS Marketplace must integrate
with the AWS Marketplace Metering Service and call the RegisterUsage operation
for software entitlement and metering.

Type annotations for
`session.create_client("meteringmarketplace").register_usage` method.

Boto3 documentation:
[MarketplaceMetering.Client.register_usage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.register_usage)

Asynchronous method. Use `await register_usage(...)` for a synchronous call.

Arguments mapping described in
[RegisterUsageRequestRequestTypeDef](./type_defs.md#registerusagerequestrequesttypedef).

Keyword-only arguments:

- `ProductCode`: `str` *(required)*
- `PublicKeyVersion`: `int` *(required)*
- `Nonce`: `str`

Returns a `Coroutine` for
[RegisterUsageResultTypeDef](./type_defs.md#registerusageresulttypedef).

<a id="resolve_customer"></a>

### resolve_customer

ResolveCustomer is called by a SaaS application during the registration
process.

Type annotations for
`session.create_client("meteringmarketplace").resolve_customer` method.

Boto3 documentation:
[MarketplaceMetering.Client.resolve_customer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.resolve_customer)

Asynchronous method. Use `await resolve_customer(...)` for a synchronous call.

Arguments mapping described in
[ResolveCustomerRequestRequestTypeDef](./type_defs.md#resolvecustomerrequestrequesttypedef).

Keyword-only arguments:

- `RegistrationToken`: `str` *(required)*

Returns a `Coroutine` for
[ResolveCustomerResultTypeDef](./type_defs.md#resolvecustomerresulttypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("meteringmarketplace").__aenter__`
method.

Boto3 documentation:
[MarketplaceMetering.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[MarketplaceMeteringClient](#marketplacemeteringclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("meteringmarketplace").__aexit__`
method.

Boto3 documentation:
[MarketplaceMetering.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
