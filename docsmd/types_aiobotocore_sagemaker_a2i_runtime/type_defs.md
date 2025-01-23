# Type definitions

> [Index](../README.md) > [AugmentedAIRuntime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AugmentedAIRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#augmentedairuntime)
    type annotations stubs module [types-aiobotocore-sagemaker-a2i-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## DeleteHumanLoopRequestRequestTypeDef

```python
# DeleteHumanLoopRequestRequestTypeDef definition

class DeleteHumanLoopRequestRequestTypeDef(TypedDict):
    HumanLoopName: str,
```

## DescribeHumanLoopRequestRequestTypeDef

```python
# DescribeHumanLoopRequestRequestTypeDef definition

class DescribeHumanLoopRequestRequestTypeDef(TypedDict):
    HumanLoopName: str,
```

## HumanLoopOutputTypeDef

```python
# HumanLoopOutputTypeDef definition

class HumanLoopOutputTypeDef(TypedDict):
    OutputS3Uri: str,
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

## HumanLoopDataAttributesTypeDef

```python
# HumanLoopDataAttributesTypeDef definition

class HumanLoopDataAttributesTypeDef(TypedDict):
    ContentClassifiers: Sequence[ContentClassifierType],  # (1)
```

1. See [:material-code-brackets: ContentClassifierType](./literals.md#contentclassifiertype) 
## HumanLoopInputTypeDef

```python
# HumanLoopInputTypeDef definition

class HumanLoopInputTypeDef(TypedDict):
    InputContent: str,
```

## HumanLoopSummaryTypeDef

```python
# HumanLoopSummaryTypeDef definition

class HumanLoopSummaryTypeDef(TypedDict):
    HumanLoopName: NotRequired[str],
    HumanLoopStatus: NotRequired[HumanLoopStatusType],  # (1)
    CreationTime: NotRequired[datetime],
    FailureReason: NotRequired[str],
    FlowDefinitionArn: NotRequired[str],
```

1. See [:material-code-brackets: HumanLoopStatusType](./literals.md#humanloopstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## StopHumanLoopRequestRequestTypeDef

```python
# StopHumanLoopRequestRequestTypeDef definition

class StopHumanLoopRequestRequestTypeDef(TypedDict):
    HumanLoopName: str,
```

## DescribeHumanLoopResponseTypeDef

```python
# DescribeHumanLoopResponseTypeDef definition

class DescribeHumanLoopResponseTypeDef(TypedDict):
    CreationTime: datetime,
    FailureReason: str,
    FailureCode: str,
    HumanLoopStatus: HumanLoopStatusType,  # (1)
    HumanLoopName: str,
    HumanLoopArn: str,
    FlowDefinitionArn: str,
    HumanLoopOutput: HumanLoopOutputTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: HumanLoopStatusType](./literals.md#humanloopstatustype) 
2. See [:material-code-braces: HumanLoopOutputTypeDef](./type_defs.md#humanloopoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartHumanLoopResponseTypeDef

```python
# StartHumanLoopResponseTypeDef definition

class StartHumanLoopResponseTypeDef(TypedDict):
    HumanLoopArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartHumanLoopRequestRequestTypeDef

```python
# StartHumanLoopRequestRequestTypeDef definition

class StartHumanLoopRequestRequestTypeDef(TypedDict):
    HumanLoopName: str,
    FlowDefinitionArn: str,
    HumanLoopInput: HumanLoopInputTypeDef,  # (1)
    DataAttributes: NotRequired[HumanLoopDataAttributesTypeDef],  # (2)
```

1. See [:material-code-braces: HumanLoopInputTypeDef](./type_defs.md#humanloopinputtypedef) 
2. See [:material-code-braces: HumanLoopDataAttributesTypeDef](./type_defs.md#humanloopdataattributestypedef) 
## ListHumanLoopsResponseTypeDef

```python
# ListHumanLoopsResponseTypeDef definition

class ListHumanLoopsResponseTypeDef(TypedDict):
    HumanLoopSummaries: List[HumanLoopSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HumanLoopSummaryTypeDef](./type_defs.md#humanloopsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHumanLoopsRequestPaginateTypeDef

```python
# ListHumanLoopsRequestPaginateTypeDef definition

class ListHumanLoopsRequestPaginateTypeDef(TypedDict):
    FlowDefinitionArn: str,
    CreationTimeAfter: NotRequired[TimestampTypeDef],
    CreationTimeBefore: NotRequired[TimestampTypeDef],
    SortOrder: NotRequired[SortOrderType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHumanLoopsRequestRequestTypeDef

```python
# ListHumanLoopsRequestRequestTypeDef definition

class ListHumanLoopsRequestRequestTypeDef(TypedDict):
    FlowDefinitionArn: str,
    CreationTimeAfter: NotRequired[TimestampTypeDef],
    CreationTimeBefore: NotRequired[TimestampTypeDef],
    SortOrder: NotRequired[SortOrderType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
