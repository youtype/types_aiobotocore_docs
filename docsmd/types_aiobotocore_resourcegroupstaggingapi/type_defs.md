# Type definitions

> [Index](../README.md) > [ResourceGroupsTaggingAPI](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ResourceGroupsTaggingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#resourcegroupstaggingapi)
    type annotations stubs module [types-aiobotocore-resourcegroupstaggingapi](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi/).



## ComplianceDetailsTypeDef

```python
# ComplianceDetailsTypeDef definition

class ComplianceDetailsTypeDef(TypedDict):
    NoncompliantKeys: NotRequired[List[str]],
    KeysWithNoncompliantValues: NotRequired[List[str]],
    ComplianceStatus: NotRequired[bool],
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

## FailureInfoTypeDef

```python
# FailureInfoTypeDef definition

class FailureInfoTypeDef(TypedDict):
    StatusCode: NotRequired[int],
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetComplianceSummaryInputRequestTypeDef

```python
# GetComplianceSummaryInputRequestTypeDef definition

class GetComplianceSummaryInputRequestTypeDef(TypedDict):
    TargetIdFilters: NotRequired[Sequence[str]],
    RegionFilters: NotRequired[Sequence[str]],
    ResourceTypeFilters: NotRequired[Sequence[str]],
    TagKeyFilters: NotRequired[Sequence[str]],
    GroupBy: NotRequired[Sequence[GroupByAttributeType]],  # (1)
    MaxResults: NotRequired[int],
    PaginationToken: NotRequired[str],
```

1. See [:material-code-brackets: GroupByAttributeType](./literals.md#groupbyattributetype) 
## SummaryTypeDef

```python
# SummaryTypeDef definition

class SummaryTypeDef(TypedDict):
    LastUpdated: NotRequired[str],
    TargetId: NotRequired[str],
    TargetIdType: NotRequired[TargetIdTypeType],  # (1)
    Region: NotRequired[str],
    ResourceType: NotRequired[str],
    NonCompliantResources: NotRequired[int],
```

1. See [:material-code-brackets: TargetIdTypeType](./literals.md#targetidtypetype) 
## TagFilterTypeDef

```python
# TagFilterTypeDef definition

class TagFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## GetTagKeysInputRequestTypeDef

```python
# GetTagKeysInputRequestTypeDef definition

class GetTagKeysInputRequestTypeDef(TypedDict):
    PaginationToken: NotRequired[str],
```

## GetTagValuesInputRequestTypeDef

```python
# GetTagValuesInputRequestTypeDef definition

class GetTagValuesInputRequestTypeDef(TypedDict):
    Key: str,
    PaginationToken: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## StartReportCreationInputRequestTypeDef

```python
# StartReportCreationInputRequestTypeDef definition

class StartReportCreationInputRequestTypeDef(TypedDict):
    S3Bucket: str,
```

## TagResourcesInputRequestTypeDef

```python
# TagResourcesInputRequestTypeDef definition

class TagResourcesInputRequestTypeDef(TypedDict):
    ResourceARNList: Sequence[str],
    Tags: Mapping[str, str],
```

## UntagResourcesInputRequestTypeDef

```python
# UntagResourcesInputRequestTypeDef definition

class UntagResourcesInputRequestTypeDef(TypedDict):
    ResourceARNList: Sequence[str],
    TagKeys: Sequence[str],
```

## DescribeReportCreationOutputTypeDef

```python
# DescribeReportCreationOutputTypeDef definition

class DescribeReportCreationOutputTypeDef(TypedDict):
    Status: str,
    S3Location: str,
    ErrorMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTagKeysOutputTypeDef

```python
# GetTagKeysOutputTypeDef definition

class GetTagKeysOutputTypeDef(TypedDict):
    PaginationToken: str,
    TagKeys: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTagValuesOutputTypeDef

```python
# GetTagValuesOutputTypeDef definition

class GetTagValuesOutputTypeDef(TypedDict):
    PaginationToken: str,
    TagValues: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourcesOutputTypeDef

```python
# TagResourcesOutputTypeDef definition

class TagResourcesOutputTypeDef(TypedDict):
    FailedResourcesMap: Dict[str, FailureInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailureInfoTypeDef](./type_defs.md#failureinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UntagResourcesOutputTypeDef

```python
# UntagResourcesOutputTypeDef definition

class UntagResourcesOutputTypeDef(TypedDict):
    FailedResourcesMap: Dict[str, FailureInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailureInfoTypeDef](./type_defs.md#failureinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComplianceSummaryInputPaginateTypeDef

```python
# GetComplianceSummaryInputPaginateTypeDef definition

class GetComplianceSummaryInputPaginateTypeDef(TypedDict):
    TargetIdFilters: NotRequired[Sequence[str]],
    RegionFilters: NotRequired[Sequence[str]],
    ResourceTypeFilters: NotRequired[Sequence[str]],
    TagKeyFilters: NotRequired[Sequence[str]],
    GroupBy: NotRequired[Sequence[GroupByAttributeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: GroupByAttributeType](./literals.md#groupbyattributetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTagKeysInputPaginateTypeDef

```python
# GetTagKeysInputPaginateTypeDef definition

class GetTagKeysInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTagValuesInputPaginateTypeDef

```python
# GetTagValuesInputPaginateTypeDef definition

class GetTagValuesInputPaginateTypeDef(TypedDict):
    Key: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetComplianceSummaryOutputTypeDef

```python
# GetComplianceSummaryOutputTypeDef definition

class GetComplianceSummaryOutputTypeDef(TypedDict):
    SummaryList: List[SummaryTypeDef],  # (1)
    PaginationToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SummaryTypeDef](./type_defs.md#summarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcesInputPaginateTypeDef

```python
# GetResourcesInputPaginateTypeDef definition

class GetResourcesInputPaginateTypeDef(TypedDict):
    TagFilters: NotRequired[Sequence[TagFilterTypeDef]],  # (1)
    TagsPerPage: NotRequired[int],
    ResourceTypeFilters: NotRequired[Sequence[str]],
    IncludeComplianceDetails: NotRequired[bool],
    ExcludeCompliantResources: NotRequired[bool],
    ResourceARNList: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetResourcesInputRequestTypeDef

```python
# GetResourcesInputRequestTypeDef definition

class GetResourcesInputRequestTypeDef(TypedDict):
    PaginationToken: NotRequired[str],
    TagFilters: NotRequired[Sequence[TagFilterTypeDef]],  # (1)
    ResourcesPerPage: NotRequired[int],
    TagsPerPage: NotRequired[int],
    ResourceTypeFilters: NotRequired[Sequence[str]],
    IncludeComplianceDetails: NotRequired[bool],
    ExcludeCompliantResources: NotRequired[bool],
    ResourceARNList: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
## ResourceTagMappingTypeDef

```python
# ResourceTagMappingTypeDef definition

class ResourceTagMappingTypeDef(TypedDict):
    ResourceARN: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
    ComplianceDetails: NotRequired[ComplianceDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ComplianceDetailsTypeDef](./type_defs.md#compliancedetailstypedef) 
## GetResourcesOutputTypeDef

```python
# GetResourcesOutputTypeDef definition

class GetResourcesOutputTypeDef(TypedDict):
    PaginationToken: str,
    ResourceTagMappingList: List[ResourceTagMappingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTagMappingTypeDef](./type_defs.md#resourcetagmappingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
