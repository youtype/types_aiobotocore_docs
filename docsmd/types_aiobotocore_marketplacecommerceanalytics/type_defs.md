# Type definitions

> [Index](../README.md) > [MarketplaceCommerceAnalytics](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MarketplaceCommerceAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#marketplacecommerceanalytics)
    type annotations stubs module [types-aiobotocore-marketplacecommerceanalytics](https://pypi.org/project/types-aiobotocore-marketplacecommerceanalytics/).

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
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## GenerateDataSetRequestRequestTypeDef

```python
# GenerateDataSetRequestRequestTypeDef definition

class GenerateDataSetRequestRequestTypeDef(TypedDict):
    dataSetType: DataSetTypeType,  # (1)
    dataSetPublicationDate: TimestampTypeDef,
    roleNameArn: str,
    destinationS3BucketName: str,
    snsTopicArn: str,
    destinationS3Prefix: NotRequired[str],
    customerDefinedValues: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DataSetTypeType](./literals.md#datasettypetype) 
## StartSupportDataExportRequestRequestTypeDef

```python
# StartSupportDataExportRequestRequestTypeDef definition

class StartSupportDataExportRequestRequestTypeDef(TypedDict):
    dataSetType: SupportDataSetTypeType,  # (1)
    fromDate: TimestampTypeDef,
    roleNameArn: str,
    destinationS3BucketName: str,
    snsTopicArn: str,
    destinationS3Prefix: NotRequired[str],
    customerDefinedValues: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: SupportDataSetTypeType](./literals.md#supportdatasettypetype) 
## GenerateDataSetResultTypeDef

```python
# GenerateDataSetResultTypeDef definition

class GenerateDataSetResultTypeDef(TypedDict):
    dataSetRequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSupportDataExportResultTypeDef

```python
# StartSupportDataExportResultTypeDef definition

class StartSupportDataExportResultTypeDef(TypedDict):
    dataSetRequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
