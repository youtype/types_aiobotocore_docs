# MarketplaceMeteringClient

> [Index](../README.md) > [MarketplaceMetering](./README.md) > MarketplaceMeteringClient

!!! note ""

    Auto-generated documentation for [MarketplaceMetering](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#marketplacemetering)
    type annotations stubs module [types-aiobotocore-meteringmarketplace](https://pypi.org/project/types-aiobotocore-meteringmarketplace/).

## MarketplaceMeteringClient

Type annotations and code completion for `#!python session.create_client("meteringmarketplace")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client)

```python
# MarketplaceMeteringClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_meteringmarketplace.client import MarketplaceMeteringClient

session = get_session()
async with session.create_client("meteringmarketplace") as client:
    client: MarketplaceMeteringClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("meteringmarketplace").exceptions` structure.

```python
# MarketplaceMeteringClient.exceptions usage example

async with session.create_client("meteringmarketplace") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.CustomerNotEntitledException,
        client.DisabledApiException,
        client.DuplicateRequestException,
        client.ExpiredTokenException,
        client.InternalServiceErrorException,
        client.InvalidCustomerIdentifierException,
        client.InvalidEndpointRegionException,
        client.InvalidProductCodeException,
        client.InvalidPublicKeyVersionException,
        client.InvalidRegionException,
        client.InvalidTagException,
        client.InvalidTokenException,
        client.InvalidUsageAllocationsException,
        client.InvalidUsageDimensionException,
        client.PlatformNotSupportedException,
        client.ThrottlingException,
        client.TimestampOutOfBoundsException,
    ) as e:
        print(e)
```

```python
# MarketplaceMeteringClient usage type checking example

from types_aiobotocore_meteringmarketplace.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("meteringmarketplace").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("meteringmarketplace").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace/client/generate_presigned_url.html)

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


### batch\_meter\_usage

<code>BatchMeterUsage</code> is called from a SaaS application listed on AWS
Marketplace to post metering records for a set of customers.

Type annotations and code completion for `#!python session.create_client("meteringmarketplace").batch_meter_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace/client/batch_meter_usage.html)

```python
# batch_meter_usage method definition

await def batch_meter_usage(
    self,
    *,
    UsageRecords: Sequence[UsageRecordUnionTypeDef],  # (1)
    ProductCode: str,
) -> BatchMeterUsageResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UsageRecordTypeDef](./type_defs.md#usagerecordtypedef) [:material-code-braces: UsageRecordOutputTypeDef](./type_defs.md#usagerecordoutputtypedef) 
2. See [:material-code-braces: BatchMeterUsageResultTypeDef](./type_defs.md#batchmeterusageresulttypedef) 


```python
# batch_meter_usage method usage example with argument unpacking

kwargs: BatchMeterUsageRequestTypeDef = {  # (1)
    "UsageRecords": ...,
    "ProductCode": ...,
}

parent.batch_meter_usage(**kwargs)
```

1. See [:material-code-braces: BatchMeterUsageRequestTypeDef](./type_defs.md#batchmeterusagerequesttypedef) 

### meter\_usage

API to emit metering records.

Type annotations and code completion for `#!python session.create_client("meteringmarketplace").meter_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace/client/meter_usage.html)

```python
# meter_usage method definition

await def meter_usage(
    self,
    *,
    ProductCode: str,
    Timestamp: TimestampTypeDef,
    UsageDimension: str,
    UsageQuantity: int = ...,
    DryRun: bool = ...,
    UsageAllocations: Sequence[UsageAllocationUnionTypeDef] = ...,  # (1)
) -> MeterUsageResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UsageAllocationTypeDef](./type_defs.md#usageallocationtypedef) [:material-code-braces: UsageAllocationOutputTypeDef](./type_defs.md#usageallocationoutputtypedef) 
2. See [:material-code-braces: MeterUsageResultTypeDef](./type_defs.md#meterusageresulttypedef) 


```python
# meter_usage method usage example with argument unpacking

kwargs: MeterUsageRequestTypeDef = {  # (1)
    "ProductCode": ...,
    "Timestamp": ...,
    "UsageDimension": ...,
}

parent.meter_usage(**kwargs)
```

1. See [:material-code-braces: MeterUsageRequestTypeDef](./type_defs.md#meterusagerequesttypedef) 

### register\_usage

Paid container software products sold through AWS Marketplace must integrate
with the AWS Marketplace Metering Service and call the
<code>RegisterUsage</code> operation for software entitlement and metering.

Type annotations and code completion for `#!python session.create_client("meteringmarketplace").register_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace/client/register_usage.html)

```python
# register_usage method definition

await def register_usage(
    self,
    *,
    ProductCode: str,
    PublicKeyVersion: int,
    Nonce: str = ...,
) -> RegisterUsageResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterUsageResultTypeDef](./type_defs.md#registerusageresulttypedef) 


```python
# register_usage method usage example with argument unpacking

kwargs: RegisterUsageRequestTypeDef = {  # (1)
    "ProductCode": ...,
    "PublicKeyVersion": ...,
}

parent.register_usage(**kwargs)
```

1. See [:material-code-braces: RegisterUsageRequestTypeDef](./type_defs.md#registerusagerequesttypedef) 

### resolve\_customer

<code>ResolveCustomer</code> is called by a SaaS application during the
registration process.

Type annotations and code completion for `#!python session.create_client("meteringmarketplace").resolve_customer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace/client/resolve_customer.html)

```python
# resolve_customer method definition

await def resolve_customer(
    self,
    *,
    RegistrationToken: str,
) -> ResolveCustomerResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResolveCustomerResultTypeDef](./type_defs.md#resolvecustomerresulttypedef) 


```python
# resolve_customer method usage example with argument unpacking

kwargs: ResolveCustomerRequestTypeDef = {  # (1)
    "RegistrationToken": ...,
}

parent.resolve_customer(**kwargs)
```

1. See [:material-code-braces: ResolveCustomerRequestTypeDef](./type_defs.md#resolvecustomerrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("meteringmarketplace").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("meteringmarketplace").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```





