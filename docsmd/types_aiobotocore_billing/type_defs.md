# Type definitions

> [Index](../README.md) > [Billing](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Billing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#billing)
    type annotations stubs module [types-aiobotocore-billing](https://pypi.org/project/types-aiobotocore-billing/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## DimensionValuesUnionTypeDef

```python
# DimensionValuesUnionTypeDef definition

DimensionValuesUnionTypeDef = Union[
    DimensionValuesTypeDef,  # (1)
    DimensionValuesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DimensionValuesTypeDef](./type_defs.md#dimensionvaluestypedef) 
2. See [:material-code-braces: DimensionValuesOutputTypeDef](./type_defs.md#dimensionvaluesoutputtypedef) 

## TagValuesUnionTypeDef

```python
# TagValuesUnionTypeDef definition

TagValuesUnionTypeDef = Union[
    TagValuesTypeDef,  # (1)
    TagValuesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TagValuesTypeDef](./type_defs.md#tagvaluestypedef) 
2. See [:material-code-braces: TagValuesOutputTypeDef](./type_defs.md#tagvaluesoutputtypedef) 



## BillingViewListElementTypeDef

```python
# BillingViewListElementTypeDef definition

class BillingViewListElementTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    ownerAccountId: NotRequired[str],
    billingViewType: NotRequired[BillingViewTypeType],  # (1)
```

1. See [:material-code-brackets: BillingViewTypeType](./literals.md#billingviewtypetype) 
## ResourceTagTypeDef

```python
# ResourceTagTypeDef definition

class ResourceTagTypeDef(TypedDict):
    key: str,
    value: NotRequired[str],
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

## DeleteBillingViewRequestRequestTypeDef

```python
# DeleteBillingViewRequestRequestTypeDef definition

class DeleteBillingViewRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DimensionValuesOutputTypeDef

```python
# DimensionValuesOutputTypeDef definition

class DimensionValuesOutputTypeDef(TypedDict):
    key: DimensionType,  # (1)
    values: List[str],
```

1. See [:material-code-brackets: DimensionType](./literals.md#dimensiontype) 
## DimensionValuesTypeDef

```python
# DimensionValuesTypeDef definition

class DimensionValuesTypeDef(TypedDict):
    key: DimensionType,  # (1)
    values: Sequence[str],
```

1. See [:material-code-brackets: DimensionType](./literals.md#dimensiontype) 
## TagValuesOutputTypeDef

```python
# TagValuesOutputTypeDef definition

class TagValuesOutputTypeDef(TypedDict):
    key: str,
    values: List[str],
```

## GetBillingViewRequestRequestTypeDef

```python
# GetBillingViewRequestRequestTypeDef definition

class GetBillingViewRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetResourcePolicyRequestRequestTypeDef

```python
# GetResourcePolicyRequestRequestTypeDef definition

class GetResourcePolicyRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListSourceViewsForBillingViewRequestRequestTypeDef

```python
# ListSourceViewsForBillingViewRequestRequestTypeDef definition

class ListSourceViewsForBillingViewRequestRequestTypeDef(TypedDict):
    arn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TagValuesTypeDef

```python
# TagValuesTypeDef definition

class TagValuesTypeDef(TypedDict):
    key: str,
    values: Sequence[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    resourceTagKeys: Sequence[str],
```

## ActiveTimeRangeTypeDef

```python
# ActiveTimeRangeTypeDef definition

class ActiveTimeRangeTypeDef(TypedDict):
    activeAfterInclusive: TimestampTypeDef,
    activeBeforeInclusive: TimestampTypeDef,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    resourceTags: Sequence[ResourceTagTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## CreateBillingViewResponseTypeDef

```python
# CreateBillingViewResponseTypeDef definition

class CreateBillingViewResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBillingViewResponseTypeDef

```python
# DeleteBillingViewResponseTypeDef definition

class DeleteBillingViewResponseTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResponseTypeDef

```python
# GetResourcePolicyResponseTypeDef definition

class GetResourcePolicyResponseTypeDef(TypedDict):
    resourceArn: str,
    policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillingViewsResponseTypeDef

```python
# ListBillingViewsResponseTypeDef definition

class ListBillingViewsResponseTypeDef(TypedDict):
    billingViews: List[BillingViewListElementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BillingViewListElementTypeDef](./type_defs.md#billingviewlistelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSourceViewsForBillingViewResponseTypeDef

```python
# ListSourceViewsForBillingViewResponseTypeDef definition

class ListSourceViewsForBillingViewResponseTypeDef(TypedDict):
    sourceViews: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    resourceTags: List[ResourceTagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBillingViewResponseTypeDef

```python
# UpdateBillingViewResponseTypeDef definition

class UpdateBillingViewResponseTypeDef(TypedDict):
    arn: str,
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExpressionOutputTypeDef

```python
# ExpressionOutputTypeDef definition

class ExpressionOutputTypeDef(TypedDict):
    dimensions: NotRequired[DimensionValuesOutputTypeDef],  # (1)
    tags: NotRequired[TagValuesOutputTypeDef],  # (2)
```

1. See [:material-code-braces: DimensionValuesOutputTypeDef](./type_defs.md#dimensionvaluesoutputtypedef) 
2. See [:material-code-braces: TagValuesOutputTypeDef](./type_defs.md#tagvaluesoutputtypedef) 
## ListSourceViewsForBillingViewRequestPaginateTypeDef

```python
# ListSourceViewsForBillingViewRequestPaginateTypeDef definition

class ListSourceViewsForBillingViewRequestPaginateTypeDef(TypedDict):
    arn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillingViewsRequestPaginateTypeDef

```python
# ListBillingViewsRequestPaginateTypeDef definition

class ListBillingViewsRequestPaginateTypeDef(TypedDict):
    activeTimeRange: NotRequired[ActiveTimeRangeTypeDef],  # (1)
    arns: NotRequired[Sequence[str]],
    billingViewTypes: NotRequired[Sequence[BillingViewTypeType]],  # (2)
    ownerAccountId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ActiveTimeRangeTypeDef](./type_defs.md#activetimerangetypedef) 
2. See [:material-code-brackets: BillingViewTypeType](./literals.md#billingviewtypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillingViewsRequestRequestTypeDef

```python
# ListBillingViewsRequestRequestTypeDef definition

class ListBillingViewsRequestRequestTypeDef(TypedDict):
    activeTimeRange: NotRequired[ActiveTimeRangeTypeDef],  # (1)
    arns: NotRequired[Sequence[str]],
    billingViewTypes: NotRequired[Sequence[BillingViewTypeType]],  # (2)
    ownerAccountId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ActiveTimeRangeTypeDef](./type_defs.md#activetimerangetypedef) 
2. See [:material-code-brackets: BillingViewTypeType](./literals.md#billingviewtypetype) 
## BillingViewElementTypeDef

```python
# BillingViewElementTypeDef definition

class BillingViewElementTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    billingViewType: NotRequired[BillingViewTypeType],  # (1)
    ownerAccountId: NotRequired[str],
    dataFilterExpression: NotRequired[ExpressionOutputTypeDef],  # (2)
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: BillingViewTypeType](./literals.md#billingviewtypetype) 
2. See [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
## ExpressionTypeDef

```python
# ExpressionTypeDef definition

class ExpressionTypeDef(TypedDict):
    dimensions: NotRequired[DimensionValuesUnionTypeDef],  # (1)
    tags: NotRequired[TagValuesUnionTypeDef],  # (2)
```

1. See [:material-code-braces: DimensionValuesTypeDef](./type_defs.md#dimensionvaluestypedef) [:material-code-braces: DimensionValuesOutputTypeDef](./type_defs.md#dimensionvaluesoutputtypedef) 
2. See [:material-code-braces: TagValuesTypeDef](./type_defs.md#tagvaluestypedef) [:material-code-braces: TagValuesOutputTypeDef](./type_defs.md#tagvaluesoutputtypedef) 
## GetBillingViewResponseTypeDef

```python
# GetBillingViewResponseTypeDef definition

class GetBillingViewResponseTypeDef(TypedDict):
    billingView: BillingViewElementTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BillingViewElementTypeDef](./type_defs.md#billingviewelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBillingViewRequestRequestTypeDef

```python
# CreateBillingViewRequestRequestTypeDef definition

class CreateBillingViewRequestRequestTypeDef(TypedDict):
    name: str,
    sourceViews: Sequence[str],
    description: NotRequired[str],
    dataFilterExpression: NotRequired[ExpressionTypeDef],  # (1)
    clientToken: NotRequired[str],
    resourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (2)
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## UpdateBillingViewRequestRequestTypeDef

```python
# UpdateBillingViewRequestRequestTypeDef definition

class UpdateBillingViewRequestRequestTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    description: NotRequired[str],
    dataFilterExpression: NotRequired[ExpressionTypeDef],  # (1)
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
