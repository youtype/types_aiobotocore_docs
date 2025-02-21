# Type definitions

> [Index](../README.md) > [Billing](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Billing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#billing)
    type annotations stubs module [types-aiobotocore-billing](https://pypi.org/project/types-aiobotocore-billing/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_billing.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ExpressionUnionTypeDef

```python
# ExpressionUnionTypeDef Union usage example

from types_aiobotocore_billing.type_defs import ExpressionUnionTypeDef


def get_value() -> ExpressionUnionTypeDef:
    return ...


# ExpressionUnionTypeDef definition

ExpressionUnionTypeDef = Union[
    ExpressionTypeDef,  # (1)
    ExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
2. See [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 



## BillingViewListElementTypeDef

```python
# BillingViewListElementTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import BillingViewListElementTypeDef


def get_value() -> BillingViewListElementTypeDef:
    return {
        "arn": ...,
    }


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
# ResourceTagTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import ResourceTagTypeDef


def get_value() -> ResourceTagTypeDef:
    return {
        "key": ...,
    }


# ResourceTagTypeDef definition

class ResourceTagTypeDef(TypedDict):
    key: str,
    value: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## DeleteBillingViewRequestTypeDef

```python
# DeleteBillingViewRequestTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import DeleteBillingViewRequestTypeDef


def get_value() -> DeleteBillingViewRequestTypeDef:
    return {
        "arn": ...,
    }


# DeleteBillingViewRequestTypeDef definition

class DeleteBillingViewRequestTypeDef(TypedDict):
    arn: str,
```

## DimensionValuesOutputTypeDef

```python
# DimensionValuesOutputTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import DimensionValuesOutputTypeDef


def get_value() -> DimensionValuesOutputTypeDef:
    return {
        "key": ...,
    }


# DimensionValuesOutputTypeDef definition

class DimensionValuesOutputTypeDef(TypedDict):
    key: DimensionType,  # (1)
    values: List[str],
```

1. See [:material-code-brackets: DimensionType](./literals.md#dimensiontype) 
## DimensionValuesTypeDef

```python
# DimensionValuesTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import DimensionValuesTypeDef


def get_value() -> DimensionValuesTypeDef:
    return {
        "key": ...,
    }


# DimensionValuesTypeDef definition

class DimensionValuesTypeDef(TypedDict):
    key: DimensionType,  # (1)
    values: Sequence[str],
```

1. See [:material-code-brackets: DimensionType](./literals.md#dimensiontype) 
## TagValuesOutputTypeDef

```python
# TagValuesOutputTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import TagValuesOutputTypeDef


def get_value() -> TagValuesOutputTypeDef:
    return {
        "key": ...,
    }


# TagValuesOutputTypeDef definition

class TagValuesOutputTypeDef(TypedDict):
    key: str,
    values: List[str],
```

## TagValuesTypeDef

```python
# TagValuesTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import TagValuesTypeDef


def get_value() -> TagValuesTypeDef:
    return {
        "key": ...,
    }


# TagValuesTypeDef definition

class TagValuesTypeDef(TypedDict):
    key: str,
    values: Sequence[str],
```

## GetBillingViewRequestTypeDef

```python
# GetBillingViewRequestTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import GetBillingViewRequestTypeDef


def get_value() -> GetBillingViewRequestTypeDef:
    return {
        "arn": ...,
    }


# GetBillingViewRequestTypeDef definition

class GetBillingViewRequestTypeDef(TypedDict):
    arn: str,
```

## GetResourcePolicyRequestTypeDef

```python
# GetResourcePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import GetResourcePolicyRequestTypeDef


def get_value() -> GetResourcePolicyRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# GetResourcePolicyRequestTypeDef definition

class GetResourcePolicyRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListSourceViewsForBillingViewRequestTypeDef

```python
# ListSourceViewsForBillingViewRequestTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import ListSourceViewsForBillingViewRequestTypeDef


def get_value() -> ListSourceViewsForBillingViewRequestTypeDef:
    return {
        "arn": ...,
    }


# ListSourceViewsForBillingViewRequestTypeDef definition

class ListSourceViewsForBillingViewRequestTypeDef(TypedDict):
    arn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    resourceTagKeys: Sequence[str],
```

## ActiveTimeRangeTypeDef

```python
# ActiveTimeRangeTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import ActiveTimeRangeTypeDef


def get_value() -> ActiveTimeRangeTypeDef:
    return {
        "activeAfterInclusive": ...,
    }


# ActiveTimeRangeTypeDef definition

class ActiveTimeRangeTypeDef(TypedDict):
    activeAfterInclusive: TimestampTypeDef,
    activeBeforeInclusive: TimestampTypeDef,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    resourceTags: Sequence[ResourceTagTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## CreateBillingViewResponseTypeDef

```python
# CreateBillingViewResponseTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import CreateBillingViewResponseTypeDef


def get_value() -> CreateBillingViewResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateBillingViewResponseTypeDef definition

class CreateBillingViewResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBillingViewResponseTypeDef

```python
# DeleteBillingViewResponseTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import DeleteBillingViewResponseTypeDef


def get_value() -> DeleteBillingViewResponseTypeDef:
    return {
        "arn": ...,
    }


# DeleteBillingViewResponseTypeDef definition

class DeleteBillingViewResponseTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResponseTypeDef

```python
# GetResourcePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import GetResourcePolicyResponseTypeDef


def get_value() -> GetResourcePolicyResponseTypeDef:
    return {
        "resourceArn": ...,
    }


# GetResourcePolicyResponseTypeDef definition

class GetResourcePolicyResponseTypeDef(TypedDict):
    resourceArn: str,
    policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillingViewsResponseTypeDef

```python
# ListBillingViewsResponseTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import ListBillingViewsResponseTypeDef


def get_value() -> ListBillingViewsResponseTypeDef:
    return {
        "billingViews": ...,
    }


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
# ListSourceViewsForBillingViewResponseTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import ListSourceViewsForBillingViewResponseTypeDef


def get_value() -> ListSourceViewsForBillingViewResponseTypeDef:
    return {
        "sourceViews": ...,
    }


# ListSourceViewsForBillingViewResponseTypeDef definition

class ListSourceViewsForBillingViewResponseTypeDef(TypedDict):
    sourceViews: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "resourceTags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    resourceTags: List[ResourceTagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBillingViewResponseTypeDef

```python
# UpdateBillingViewResponseTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import UpdateBillingViewResponseTypeDef


def get_value() -> UpdateBillingViewResponseTypeDef:
    return {
        "arn": ...,
    }


# UpdateBillingViewResponseTypeDef definition

class UpdateBillingViewResponseTypeDef(TypedDict):
    arn: str,
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExpressionOutputTypeDef

```python
# ExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import ExpressionOutputTypeDef


def get_value() -> ExpressionOutputTypeDef:
    return {
        "dimensions": ...,
    }


# ExpressionOutputTypeDef definition

class ExpressionOutputTypeDef(TypedDict):
    dimensions: NotRequired[DimensionValuesOutputTypeDef],  # (1)
    tags: NotRequired[TagValuesOutputTypeDef],  # (2)
```

1. See [:material-code-braces: DimensionValuesOutputTypeDef](./type_defs.md#dimensionvaluesoutputtypedef) 
2. See [:material-code-braces: TagValuesOutputTypeDef](./type_defs.md#tagvaluesoutputtypedef) 
## ExpressionTypeDef

```python
# ExpressionTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import ExpressionTypeDef


def get_value() -> ExpressionTypeDef:
    return {
        "dimensions": ...,
    }


# ExpressionTypeDef definition

class ExpressionTypeDef(TypedDict):
    dimensions: NotRequired[DimensionValuesTypeDef],  # (1)
    tags: NotRequired[TagValuesTypeDef],  # (2)
```

1. See [:material-code-braces: DimensionValuesTypeDef](./type_defs.md#dimensionvaluestypedef) 
2. See [:material-code-braces: TagValuesTypeDef](./type_defs.md#tagvaluestypedef) 
## ListSourceViewsForBillingViewRequestPaginateTypeDef

```python
# ListSourceViewsForBillingViewRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import ListSourceViewsForBillingViewRequestPaginateTypeDef


def get_value() -> ListSourceViewsForBillingViewRequestPaginateTypeDef:
    return {
        "arn": ...,
    }


# ListSourceViewsForBillingViewRequestPaginateTypeDef definition

class ListSourceViewsForBillingViewRequestPaginateTypeDef(TypedDict):
    arn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillingViewsRequestPaginateTypeDef

```python
# ListBillingViewsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import ListBillingViewsRequestPaginateTypeDef


def get_value() -> ListBillingViewsRequestPaginateTypeDef:
    return {
        "activeTimeRange": ...,
    }


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
## ListBillingViewsRequestTypeDef

```python
# ListBillingViewsRequestTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import ListBillingViewsRequestTypeDef


def get_value() -> ListBillingViewsRequestTypeDef:
    return {
        "activeTimeRange": ...,
    }


# ListBillingViewsRequestTypeDef definition

class ListBillingViewsRequestTypeDef(TypedDict):
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
# BillingViewElementTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import BillingViewElementTypeDef


def get_value() -> BillingViewElementTypeDef:
    return {
        "arn": ...,
    }


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
## GetBillingViewResponseTypeDef

```python
# GetBillingViewResponseTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import GetBillingViewResponseTypeDef


def get_value() -> GetBillingViewResponseTypeDef:
    return {
        "billingView": ...,
    }


# GetBillingViewResponseTypeDef definition

class GetBillingViewResponseTypeDef(TypedDict):
    billingView: BillingViewElementTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BillingViewElementTypeDef](./type_defs.md#billingviewelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBillingViewRequestTypeDef

```python
# CreateBillingViewRequestTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import CreateBillingViewRequestTypeDef


def get_value() -> CreateBillingViewRequestTypeDef:
    return {
        "name": ...,
    }


# CreateBillingViewRequestTypeDef definition

class CreateBillingViewRequestTypeDef(TypedDict):
    name: str,
    sourceViews: Sequence[str],
    description: NotRequired[str],
    dataFilterExpression: NotRequired[ExpressionUnionTypeDef],  # (1)
    clientToken: NotRequired[str],
    resourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (2)
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## UpdateBillingViewRequestTypeDef

```python
# UpdateBillingViewRequestTypeDef TypedDict usage example

from types_aiobotocore_billing.type_defs import UpdateBillingViewRequestTypeDef


def get_value() -> UpdateBillingViewRequestTypeDef:
    return {
        "arn": ...,
    }


# UpdateBillingViewRequestTypeDef definition

class UpdateBillingViewRequestTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    description: NotRequired[str],
    dataFilterExpression: NotRequired[ExpressionUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
