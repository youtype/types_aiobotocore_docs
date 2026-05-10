# Type definitions

> [Index](../README.md) > [ElementalInference](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ElementalInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference.html#elementalinference)
    type annotations stubs module [types-aiobotocore-elementalinference](https://pypi.org/project/types-aiobotocore-elementalinference/).

## OutputConfigUnionTypeDef

```python
# OutputConfigUnionTypeDef Union usage example

from types_aiobotocore_elementalinference.type_defs import OutputConfigUnionTypeDef


def get_value() -> OutputConfigUnionTypeDef:
    return ...


# OutputConfigUnionTypeDef definition

OutputConfigUnionTypeDef = Union[
    OutputConfigTypeDef,  # (1)
    OutputConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef)
2. See [:material-code-braces: OutputConfigOutputTypeDef](./type_defs.md#outputconfigoutputtypedef)



## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```


## ClippingConfigTypeDef

```python
# ClippingConfigTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import ClippingConfigTypeDef


def get_value() -> ClippingConfigTypeDef:
    return {
        "callbackMetadata": ...,
    }


# ClippingConfigTypeDef definition

class ClippingConfigTypeDef(TypedDict):
    callbackMetadata: NotRequired[str],
```


## FeedAssociationTypeDef

```python
# FeedAssociationTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import FeedAssociationTypeDef


def get_value() -> FeedAssociationTypeDef:
    return {
        "associatedResourceName": ...,
    }


# FeedAssociationTypeDef definition

class FeedAssociationTypeDef(TypedDict):
    associatedResourceName: str,
```


## DeleteFeedRequestTypeDef

```python
# DeleteFeedRequestTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import DeleteFeedRequestTypeDef


def get_value() -> DeleteFeedRequestTypeDef:
    return {
        "id": ...,
    }


# DeleteFeedRequestTypeDef definition

class DeleteFeedRequestTypeDef(TypedDict):
    id: str,
```


## DisassociateFeedRequestTypeDef

```python
# DisassociateFeedRequestTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import DisassociateFeedRequestTypeDef


def get_value() -> DisassociateFeedRequestTypeDef:
    return {
        "id": ...,
    }


# DisassociateFeedRequestTypeDef definition

class DisassociateFeedRequestTypeDef(TypedDict):
    id: str,
    associatedResourceName: str,
    dryRun: NotRequired[bool],
```


## GetFeedRequestTypeDef

```python
# GetFeedRequestTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import GetFeedRequestTypeDef


def get_value() -> GetFeedRequestTypeDef:
    return {
        "id": ...,
    }


# GetFeedRequestTypeDef definition

class GetFeedRequestTypeDef(TypedDict):
    id: str,
```


## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```


## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import PaginatorConfigTypeDef


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


## ListFeedsRequestTypeDef

```python
# ListFeedsRequestTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import ListFeedsRequestTypeDef


def get_value() -> ListFeedsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListFeedsRequestTypeDef definition

class ListFeedsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```


## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```


## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```


## AssociateFeedResponseTypeDef

```python
# AssociateFeedResponseTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import AssociateFeedResponseTypeDef


def get_value() -> AssociateFeedResponseTypeDef:
    return {
        "arn": ...,
    }


# AssociateFeedResponseTypeDef definition

class AssociateFeedResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteFeedResponseTypeDef

```python
# DeleteFeedResponseTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import DeleteFeedResponseTypeDef


def get_value() -> DeleteFeedResponseTypeDef:
    return {
        "arn": ...,
    }


# DeleteFeedResponseTypeDef definition

class DeleteFeedResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    status: FeedStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FeedStatusType](./literals.md#feedstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DisassociateFeedResponseTypeDef

```python
# DisassociateFeedResponseTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import DisassociateFeedResponseTypeDef


def get_value() -> DisassociateFeedResponseTypeDef:
    return {
        "arn": ...,
    }


# DisassociateFeedResponseTypeDef definition

class DisassociateFeedResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## OutputConfigOutputTypeDef

```python
# OutputConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import OutputConfigOutputTypeDef


def get_value() -> OutputConfigOutputTypeDef:
    return {
        "cropping": ...,
    }


# OutputConfigOutputTypeDef definition

class OutputConfigOutputTypeDef(TypedDict):
    cropping: NotRequired[dict[str, Any]],
    clipping: NotRequired[ClippingConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ClippingConfigTypeDef](./type_defs.md#clippingconfigtypedef)

## OutputConfigTypeDef

```python
# OutputConfigTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import OutputConfigTypeDef


def get_value() -> OutputConfigTypeDef:
    return {
        "cropping": ...,
    }


# OutputConfigTypeDef definition

class OutputConfigTypeDef(TypedDict):
    cropping: NotRequired[Mapping[str, Any]],
    clipping: NotRequired[ClippingConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ClippingConfigTypeDef](./type_defs.md#clippingconfigtypedef)

## FeedSummaryTypeDef

```python
# FeedSummaryTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import FeedSummaryTypeDef


def get_value() -> FeedSummaryTypeDef:
    return {
        "arn": ...,
    }


# FeedSummaryTypeDef definition

class FeedSummaryTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    status: FeedStatusType,  # (2)
    association: NotRequired[FeedAssociationTypeDef],  # (1)
```

1. See [:material-code-braces: FeedAssociationTypeDef](./type_defs.md#feedassociationtypedef)
2. See [:material-code-brackets: FeedStatusType](./literals.md#feedstatustype)

## GetFeedRequestWaitTypeDef

```python
# GetFeedRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import GetFeedRequestWaitTypeDef


def get_value() -> GetFeedRequestWaitTypeDef:
    return {
        "id": ...,
    }


# GetFeedRequestWaitTypeDef definition

class GetFeedRequestWaitTypeDef(TypedDict):
    id: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

## ListFeedsRequestPaginateTypeDef

```python
# ListFeedsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import ListFeedsRequestPaginateTypeDef


def get_value() -> ListFeedsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListFeedsRequestPaginateTypeDef definition

class ListFeedsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## GetOutputTypeDef

```python
# GetOutputTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import GetOutputTypeDef


def get_value() -> GetOutputTypeDef:
    return {
        "name": ...,
    }


# GetOutputTypeDef definition

class GetOutputTypeDef(TypedDict):
    name: str,
    outputConfig: OutputConfigOutputTypeDef,  # (1)
    status: OutputStatusType,  # (2)
    description: NotRequired[str],
    fromAssociation: NotRequired[bool],
```

1. See [:material-code-braces: OutputConfigOutputTypeDef](./type_defs.md#outputconfigoutputtypedef)
2. See [:material-code-brackets: OutputStatusType](./literals.md#outputstatustype)

## ListFeedsResponseTypeDef

```python
# ListFeedsResponseTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import ListFeedsResponseTypeDef


def get_value() -> ListFeedsResponseTypeDef:
    return {
        "feeds": ...,
    }


# ListFeedsResponseTypeDef definition

class ListFeedsResponseTypeDef(TypedDict):
    feeds: list[FeedSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[FeedSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateFeedResponseTypeDef

```python
# CreateFeedResponseTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import CreateFeedResponseTypeDef


def get_value() -> CreateFeedResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateFeedResponseTypeDef definition

class CreateFeedResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    id: str,
    dataEndpoints: list[str],
    outputs: list[GetOutputTypeDef],  # (1)
    status: FeedStatusType,  # (2)
    association: FeedAssociationTypeDef,  # (3)
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See `list[GetOutputTypeDef]`
2. See [:material-code-brackets: FeedStatusType](./literals.md#feedstatustype)
3. See [:material-code-braces: FeedAssociationTypeDef](./type_defs.md#feedassociationtypedef)
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetFeedResponseTypeDef

```python
# GetFeedResponseTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import GetFeedResponseTypeDef


def get_value() -> GetFeedResponseTypeDef:
    return {
        "arn": ...,
    }


# GetFeedResponseTypeDef definition

class GetFeedResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    id: str,
    dataEndpoints: list[str],
    outputs: list[GetOutputTypeDef],  # (1)
    status: FeedStatusType,  # (2)
    association: FeedAssociationTypeDef,  # (3)
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See `list[GetOutputTypeDef]`
2. See [:material-code-brackets: FeedStatusType](./literals.md#feedstatustype)
3. See [:material-code-braces: FeedAssociationTypeDef](./type_defs.md#feedassociationtypedef)
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateFeedResponseTypeDef

```python
# UpdateFeedResponseTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import UpdateFeedResponseTypeDef


def get_value() -> UpdateFeedResponseTypeDef:
    return {
        "arn": ...,
    }


# UpdateFeedResponseTypeDef definition

class UpdateFeedResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    id: str,
    dataEndpoints: list[str],
    outputs: list[GetOutputTypeDef],  # (1)
    status: FeedStatusType,  # (2)
    association: FeedAssociationTypeDef,  # (3)
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See `list[GetOutputTypeDef]`
2. See [:material-code-brackets: FeedStatusType](./literals.md#feedstatustype)
3. See [:material-code-braces: FeedAssociationTypeDef](./type_defs.md#feedassociationtypedef)
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateOutputTypeDef

```python
# CreateOutputTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import CreateOutputTypeDef


def get_value() -> CreateOutputTypeDef:
    return {
        "name": ...,
    }


# CreateOutputTypeDef definition

class CreateOutputTypeDef(TypedDict):
    name: str,
    outputConfig: OutputConfigUnionTypeDef,  # (1)
    status: OutputStatusType,  # (2)
    description: NotRequired[str],
```

1. See [:material-code-braces: OutputConfigUnionTypeDef](#outputconfiguniontypedef)
2. See [:material-code-brackets: OutputStatusType](./literals.md#outputstatustype)

## UpdateOutputTypeDef

```python
# UpdateOutputTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import UpdateOutputTypeDef


def get_value() -> UpdateOutputTypeDef:
    return {
        "name": ...,
    }


# UpdateOutputTypeDef definition

class UpdateOutputTypeDef(TypedDict):
    name: str,
    outputConfig: OutputConfigUnionTypeDef,  # (1)
    status: OutputStatusType,  # (2)
    description: NotRequired[str],
    fromAssociation: NotRequired[bool],
```

1. See [:material-code-braces: OutputConfigUnionTypeDef](#outputconfiguniontypedef)
2. See [:material-code-brackets: OutputStatusType](./literals.md#outputstatustype)

## AssociateFeedRequestTypeDef

```python
# AssociateFeedRequestTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import AssociateFeedRequestTypeDef


def get_value() -> AssociateFeedRequestTypeDef:
    return {
        "id": ...,
    }


# AssociateFeedRequestTypeDef definition

class AssociateFeedRequestTypeDef(TypedDict):
    id: str,
    associatedResourceName: str,
    outputs: Sequence[CreateOutputTypeDef],  # (1)
    dryRun: NotRequired[bool],
```

1. See `Sequence[CreateOutputTypeDef]`

## CreateFeedRequestTypeDef

```python
# CreateFeedRequestTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import CreateFeedRequestTypeDef


def get_value() -> CreateFeedRequestTypeDef:
    return {
        "name": ...,
    }


# CreateFeedRequestTypeDef definition

class CreateFeedRequestTypeDef(TypedDict):
    name: str,
    outputs: Sequence[CreateOutputTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See `Sequence[CreateOutputTypeDef]`

## UpdateFeedRequestTypeDef

```python
# UpdateFeedRequestTypeDef TypedDict usage example

from types_aiobotocore_elementalinference.type_defs import UpdateFeedRequestTypeDef


def get_value() -> UpdateFeedRequestTypeDef:
    return {
        "name": ...,
    }


# UpdateFeedRequestTypeDef definition

class UpdateFeedRequestTypeDef(TypedDict):
    name: str,
    id: str,
    outputs: Sequence[UpdateOutputTypeDef],  # (1)
```

1. See `Sequence[UpdateOutputTypeDef]`

