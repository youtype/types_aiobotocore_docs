# MarketplaceMeteringClient

> [Index](../README.md) > [MarketplaceMetering](./README.md) > MarketplaceMeteringClient

!!! note ""

    Auto-generated documentation for [MarketplaceMetering](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
    type annotations stubs module [types-aiobotocore-meteringmarketplace](https://pypi.org/project/types-aiobotocore-meteringmarketplace/).

## MarketplaceMeteringClient

Type annotations and code completion for `#!python session.create_client("meteringmarketplace")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_meteringmarketplace.client import MarketplaceMeteringClient

session = get_session()
async with session.create_client("meteringmarketplace") as client:
    client: MarketplaceMeteringClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("meteringmarketplace").exceptions` structure.

```python title="Usage example"
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

```python title="Type checking example"
from types_aiobotocore_meteringmarketplace.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### batch\_meter\_usage

`BatchMeterUsage` is called from a SaaS application listed on AWS Marketplace to
post metering records for a set of customers.

Type annotations and code completion for `#!python session.create_client("meteringmarketplace").batch_meter_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.batch_meter_usage)

```python title="Method definition"
await def batch_meter_usage(
    self,
    *,
    UsageRecords: Sequence[UsageRecordTypeDef],  # (1)
    ProductCode: str,
) -> BatchMeterUsageResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UsageRecordTypeDef](./type_defs.md#usagerecordtypedef) 
2. See [:material-code-braces: BatchMeterUsageResultTypeDef](./type_defs.md#batchmeterusageresulttypedef) 


```python title="Usage example with kwargs"
kwargs: BatchMeterUsageRequestRequestTypeDef = {  # (1)
    "UsageRecords": ...,
    "ProductCode": ...,
}

parent.batch_meter_usage(**kwargs)
```

1. See [:material-code-braces: BatchMeterUsageRequestRequestTypeDef](./type_defs.md#batchmeterusagerequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("meteringmarketplace").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("meteringmarketplace").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("meteringmarketplace").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### meter\_usage

API to emit metering records.

Type annotations and code completion for `#!python session.create_client("meteringmarketplace").meter_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.meter_usage)

```python title="Method definition"
await def meter_usage(
    self,
    *,
    ProductCode: str,
    Timestamp: Union[datetime, str],
    UsageDimension: str,
    UsageQuantity: int = ...,
    DryRun: bool = ...,
    UsageAllocations: Sequence[UsageAllocationTypeDef] = ...,  # (1)
) -> MeterUsageResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UsageAllocationTypeDef](./type_defs.md#usageallocationtypedef) 
2. See [:material-code-braces: MeterUsageResultTypeDef](./type_defs.md#meterusageresulttypedef) 


```python title="Usage example with kwargs"
kwargs: MeterUsageRequestRequestTypeDef = {  # (1)
    "ProductCode": ...,
    "Timestamp": ...,
    "UsageDimension": ...,
}

parent.meter_usage(**kwargs)
```

1. See [:material-code-braces: MeterUsageRequestRequestTypeDef](./type_defs.md#meterusagerequestrequesttypedef) 

### register\_usage

Paid container software products sold through AWS Marketplace must integrate
with the AWS Marketplace Metering Service and call the `RegisterUsage` operation
for software entitlement and metering.

Type annotations and code completion for `#!python session.create_client("meteringmarketplace").register_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.register_usage)

```python title="Method definition"
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


```python title="Usage example with kwargs"
kwargs: RegisterUsageRequestRequestTypeDef = {  # (1)
    "ProductCode": ...,
    "PublicKeyVersion": ...,
}

parent.register_usage(**kwargs)
```

1. See [:material-code-braces: RegisterUsageRequestRequestTypeDef](./type_defs.md#registerusagerequestrequesttypedef) 

### resolve\_customer

`ResolveCustomer` is called by a SaaS application during the registration
process.

Type annotations and code completion for `#!python session.create_client("meteringmarketplace").resolve_customer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.resolve_customer)

```python title="Method definition"
await def resolve_customer(
    self,
    *,
    RegistrationToken: str,
) -> ResolveCustomerResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResolveCustomerResultTypeDef](./type_defs.md#resolvecustomerresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ResolveCustomerRequestRequestTypeDef = {  # (1)
    "RegistrationToken": ...,
}

parent.resolve_customer(**kwargs)
```

1. See [:material-code-braces: ResolveCustomerRequestRequestTypeDef](./type_defs.md#resolvecustomerrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("meteringmarketplace").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> MarketplaceMeteringClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("meteringmarketplace").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





