# Type definitions

> [Index](../README.md) > [MarketplaceMetering](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MarketplaceMetering](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
    type annotations stubs module [types-aiobotocore-meteringmarketplace](https://pypi.org/project/types-aiobotocore-meteringmarketplace/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## RegisterUsageRequestRequestTypeDef

```python
# RegisterUsageRequestRequestTypeDef definition

class RegisterUsageRequestRequestTypeDef(TypedDict):
    ProductCode: str,
    PublicKeyVersion: int,
    Nonce: NotRequired[str],
```

## ResolveCustomerRequestRequestTypeDef

```python
# ResolveCustomerRequestRequestTypeDef definition

class ResolveCustomerRequestRequestTypeDef(TypedDict):
    RegistrationToken: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## MeterUsageResultTypeDef

```python
# MeterUsageResultTypeDef definition

class MeterUsageResultTypeDef(TypedDict):
    MeteringRecordId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterUsageResultTypeDef

```python
# RegisterUsageResultTypeDef definition

class RegisterUsageResultTypeDef(TypedDict):
    PublicKeyRotationTimestamp: datetime,
    Signature: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResolveCustomerResultTypeDef

```python
# ResolveCustomerResultTypeDef definition

class ResolveCustomerResultTypeDef(TypedDict):
    CustomerIdentifier: str,
    ProductCode: str,
    CustomerAWSAccountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UsageAllocationTypeDef

```python
# UsageAllocationTypeDef definition

class UsageAllocationTypeDef(TypedDict):
    AllocatedUsageQuantity: int,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## MeterUsageRequestRequestTypeDef

```python
# MeterUsageRequestRequestTypeDef definition

class MeterUsageRequestRequestTypeDef(TypedDict):
    ProductCode: str,
    Timestamp: Union[datetime, str],
    UsageDimension: str,
    UsageQuantity: NotRequired[int],
    DryRun: NotRequired[bool],
    UsageAllocations: NotRequired[Sequence[UsageAllocationTypeDef]],  # (1)
```

1. See [:material-code-braces: UsageAllocationTypeDef](./type_defs.md#usageallocationtypedef) 
## UsageRecordTypeDef

```python
# UsageRecordTypeDef definition

class UsageRecordTypeDef(TypedDict):
    Timestamp: Union[datetime, str],
    CustomerIdentifier: str,
    Dimension: str,
    Quantity: NotRequired[int],
    UsageAllocations: NotRequired[Sequence[UsageAllocationTypeDef]],  # (1)
```

1. See [:material-code-braces: UsageAllocationTypeDef](./type_defs.md#usageallocationtypedef) 
## BatchMeterUsageRequestRequestTypeDef

```python
# BatchMeterUsageRequestRequestTypeDef definition

class BatchMeterUsageRequestRequestTypeDef(TypedDict):
    UsageRecords: Sequence[UsageRecordTypeDef],  # (1)
    ProductCode: str,
```

1. See [:material-code-braces: UsageRecordTypeDef](./type_defs.md#usagerecordtypedef) 
## UsageRecordResultTypeDef

```python
# UsageRecordResultTypeDef definition

class UsageRecordResultTypeDef(TypedDict):
    UsageRecord: NotRequired[UsageRecordTypeDef],  # (1)
    MeteringRecordId: NotRequired[str],
    Status: NotRequired[UsageRecordResultStatusType],  # (2)
```

1. See [:material-code-braces: UsageRecordTypeDef](./type_defs.md#usagerecordtypedef) 
2. See [:material-code-brackets: UsageRecordResultStatusType](./literals.md#usagerecordresultstatustype) 
## BatchMeterUsageResultTypeDef

```python
# BatchMeterUsageResultTypeDef definition

class BatchMeterUsageResultTypeDef(TypedDict):
    Results: List[UsageRecordResultTypeDef],  # (1)
    UnprocessedRecords: List[UsageRecordTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: UsageRecordResultTypeDef](./type_defs.md#usagerecordresulttypedef) 
2. See [:material-code-braces: UsageRecordTypeDef](./type_defs.md#usagerecordtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
