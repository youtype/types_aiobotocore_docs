# Type definitions

> [Index](../README.md) > [MarketplaceMetering](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MarketplaceMetering](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#marketplacemetering)
    type annotations stubs module [types-aiobotocore-meteringmarketplace](https://pypi.org/project/types-aiobotocore-meteringmarketplace/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## UsageAllocationUnionTypeDef

```python
# UsageAllocationUnionTypeDef definition

UsageAllocationUnionTypeDef = Union[
    UsageAllocationTypeDef,  # (1)
    UsageAllocationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: UsageAllocationTypeDef](./type_defs.md#usageallocationtypedef) 
2. See [:material-code-braces: UsageAllocationOutputTypeDef](./type_defs.md#usageallocationoutputtypedef) 

## UsageRecordUnionTypeDef

```python
# UsageRecordUnionTypeDef definition

UsageRecordUnionTypeDef = Union[
    UsageRecordTypeDef,  # (1)
    UsageRecordOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: UsageRecordTypeDef](./type_defs.md#usagerecordtypedef) 
2. See [:material-code-braces: UsageRecordOutputTypeDef](./type_defs.md#usagerecordoutputtypedef) 



## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
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
## UsageAllocationOutputTypeDef

```python
# UsageAllocationOutputTypeDef definition

class UsageAllocationOutputTypeDef(TypedDict):
    AllocatedUsageQuantity: int,
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UsageAllocationTypeDef

```python
# UsageAllocationTypeDef definition

class UsageAllocationTypeDef(TypedDict):
    AllocatedUsageQuantity: int,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UsageRecordOutputTypeDef

```python
# UsageRecordOutputTypeDef definition

class UsageRecordOutputTypeDef(TypedDict):
    Timestamp: datetime,
    CustomerIdentifier: str,
    Dimension: str,
    Quantity: NotRequired[int],
    UsageAllocations: NotRequired[List[UsageAllocationOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: UsageAllocationOutputTypeDef](./type_defs.md#usageallocationoutputtypedef) 
## UsageRecordResultTypeDef

```python
# UsageRecordResultTypeDef definition

class UsageRecordResultTypeDef(TypedDict):
    UsageRecord: NotRequired[UsageRecordOutputTypeDef],  # (1)
    MeteringRecordId: NotRequired[str],
    Status: NotRequired[UsageRecordResultStatusType],  # (2)
```

1. See [:material-code-braces: UsageRecordOutputTypeDef](./type_defs.md#usagerecordoutputtypedef) 
2. See [:material-code-brackets: UsageRecordResultStatusType](./literals.md#usagerecordresultstatustype) 
## MeterUsageRequestRequestTypeDef

```python
# MeterUsageRequestRequestTypeDef definition

class MeterUsageRequestRequestTypeDef(TypedDict):
    ProductCode: str,
    Timestamp: TimestampTypeDef,
    UsageDimension: str,
    UsageQuantity: NotRequired[int],
    DryRun: NotRequired[bool],
    UsageAllocations: NotRequired[Sequence[UsageAllocationUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: UsageAllocationTypeDef](./type_defs.md#usageallocationtypedef) [:material-code-braces: UsageAllocationOutputTypeDef](./type_defs.md#usageallocationoutputtypedef) 
## UsageRecordTypeDef

```python
# UsageRecordTypeDef definition

class UsageRecordTypeDef(TypedDict):
    Timestamp: TimestampTypeDef,
    CustomerIdentifier: str,
    Dimension: str,
    Quantity: NotRequired[int],
    UsageAllocations: NotRequired[Sequence[UsageAllocationUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: UsageAllocationTypeDef](./type_defs.md#usageallocationtypedef) [:material-code-braces: UsageAllocationOutputTypeDef](./type_defs.md#usageallocationoutputtypedef) 
## BatchMeterUsageResultTypeDef

```python
# BatchMeterUsageResultTypeDef definition

class BatchMeterUsageResultTypeDef(TypedDict):
    Results: List[UsageRecordResultTypeDef],  # (1)
    UnprocessedRecords: List[UsageRecordOutputTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: UsageRecordResultTypeDef](./type_defs.md#usagerecordresulttypedef) 
2. See [:material-code-braces: UsageRecordOutputTypeDef](./type_defs.md#usagerecordoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchMeterUsageRequestRequestTypeDef

```python
# BatchMeterUsageRequestRequestTypeDef definition

class BatchMeterUsageRequestRequestTypeDef(TypedDict):
    UsageRecords: Sequence[UsageRecordUnionTypeDef],  # (1)
    ProductCode: str,
```

1. See [:material-code-braces: UsageRecordTypeDef](./type_defs.md#usagerecordtypedef) [:material-code-braces: UsageRecordOutputTypeDef](./type_defs.md#usagerecordoutputtypedef) 
