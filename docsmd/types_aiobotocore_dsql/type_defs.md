# Type definitions

> [Index](../README.md) > [AuroraDSQL](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AuroraDSQL](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql.html#auroradsql)
    type annotations stubs module [types-aiobotocore-dsql](https://pypi.org/project/types-aiobotocore-dsql/).



## ClusterSummaryTypeDef

```python
# ClusterSummaryTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ClusterSummaryTypeDef


def get_value() -> ClusterSummaryTypeDef:
    return {
        "identifier": ...,
    }


# ClusterSummaryTypeDef definition

class ClusterSummaryTypeDef(TypedDict):
    identifier: str,
    arn: str,
```

## CreateClusterInputTypeDef

```python
# CreateClusterInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import CreateClusterInputTypeDef


def get_value() -> CreateClusterInputTypeDef:
    return {
        "deletionProtectionEnabled": ...,
    }


# CreateClusterInputTypeDef definition

class CreateClusterInputTypeDef(TypedDict):
    deletionProtectionEnabled: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ResponseMetadataTypeDef


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

## LinkedClusterPropertiesTypeDef

```python
# LinkedClusterPropertiesTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import LinkedClusterPropertiesTypeDef


def get_value() -> LinkedClusterPropertiesTypeDef:
    return {
        "deletionProtectionEnabled": ...,
    }


# LinkedClusterPropertiesTypeDef definition

class LinkedClusterPropertiesTypeDef(TypedDict):
    deletionProtectionEnabled: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
```

## DeleteClusterInputTypeDef

```python
# DeleteClusterInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import DeleteClusterInputTypeDef


def get_value() -> DeleteClusterInputTypeDef:
    return {
        "identifier": ...,
    }


# DeleteClusterInputTypeDef definition

class DeleteClusterInputTypeDef(TypedDict):
    identifier: str,
    clientToken: NotRequired[str],
```

## DeleteMultiRegionClustersInputTypeDef

```python
# DeleteMultiRegionClustersInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import DeleteMultiRegionClustersInputTypeDef


def get_value() -> DeleteMultiRegionClustersInputTypeDef:
    return {
        "linkedClusterArns": ...,
    }


# DeleteMultiRegionClustersInputTypeDef definition

class DeleteMultiRegionClustersInputTypeDef(TypedDict):
    linkedClusterArns: Sequence[str],
    clientToken: NotRequired[str],
```

## GetClusterInputTypeDef

```python
# GetClusterInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import GetClusterInputTypeDef


def get_value() -> GetClusterInputTypeDef:
    return {
        "identifier": ...,
    }


# GetClusterInputTypeDef definition

class GetClusterInputTypeDef(TypedDict):
    identifier: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import WaiterConfigTypeDef


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

from types_aiobotocore_dsql.type_defs import PaginatorConfigTypeDef


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

## ListClustersInputTypeDef

```python
# ListClustersInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ListClustersInputTypeDef


def get_value() -> ListClustersInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListClustersInputTypeDef definition

class ListClustersInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceInputTypeDef

```python
# ListTagsForResourceInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ListTagsForResourceInputTypeDef


def get_value() -> ListTagsForResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceInputTypeDef definition

class ListTagsForResourceInputTypeDef(TypedDict):
    resourceArn: str,
```

## TagResourceInputTypeDef

```python
# TagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import TagResourceInputTypeDef


def get_value() -> TagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceInputTypeDef definition

class TagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputTypeDef

```python
# UntagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import UntagResourceInputTypeDef


def get_value() -> UntagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceInputTypeDef definition

class UntagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateClusterInputTypeDef

```python
# UpdateClusterInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import UpdateClusterInputTypeDef


def get_value() -> UpdateClusterInputTypeDef:
    return {
        "identifier": ...,
    }


# UpdateClusterInputTypeDef definition

class UpdateClusterInputTypeDef(TypedDict):
    identifier: str,
    deletionProtectionEnabled: NotRequired[bool],
    clientToken: NotRequired[str],
```

## CreateClusterOutputTypeDef

```python
# CreateClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import CreateClusterOutputTypeDef


def get_value() -> CreateClusterOutputTypeDef:
    return {
        "identifier": ...,
    }


# CreateClusterOutputTypeDef definition

class CreateClusterOutputTypeDef(TypedDict):
    identifier: str,
    arn: str,
    status: ClusterStatusType,  # (1)
    creationTime: datetime,
    deletionProtectionEnabled: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMultiRegionClustersOutputTypeDef

```python
# CreateMultiRegionClustersOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import CreateMultiRegionClustersOutputTypeDef


def get_value() -> CreateMultiRegionClustersOutputTypeDef:
    return {
        "linkedClusterArns": ...,
    }


# CreateMultiRegionClustersOutputTypeDef definition

class CreateMultiRegionClustersOutputTypeDef(TypedDict):
    linkedClusterArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteClusterOutputTypeDef

```python
# DeleteClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import DeleteClusterOutputTypeDef


def get_value() -> DeleteClusterOutputTypeDef:
    return {
        "identifier": ...,
    }


# DeleteClusterOutputTypeDef definition

class DeleteClusterOutputTypeDef(TypedDict):
    identifier: str,
    arn: str,
    status: ClusterStatusType,  # (1)
    creationTime: datetime,
    deletionProtectionEnabled: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetClusterOutputTypeDef

```python
# GetClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import GetClusterOutputTypeDef


def get_value() -> GetClusterOutputTypeDef:
    return {
        "identifier": ...,
    }


# GetClusterOutputTypeDef definition

class GetClusterOutputTypeDef(TypedDict):
    identifier: str,
    arn: str,
    status: ClusterStatusType,  # (1)
    creationTime: datetime,
    deletionProtectionEnabled: bool,
    witnessRegion: str,
    linkedClusterArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersOutputTypeDef

```python
# ListClustersOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ListClustersOutputTypeDef


def get_value() -> ListClustersOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListClustersOutputTypeDef definition

class ListClustersOutputTypeDef(TypedDict):
    clusters: List[ClusterSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ClusterSummaryTypeDef](./type_defs.md#clustersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ListTagsForResourceOutputTypeDef


def get_value() -> ListTagsForResourceOutputTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterOutputTypeDef

```python
# UpdateClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import UpdateClusterOutputTypeDef


def get_value() -> UpdateClusterOutputTypeDef:
    return {
        "identifier": ...,
    }


# UpdateClusterOutputTypeDef definition

class UpdateClusterOutputTypeDef(TypedDict):
    identifier: str,
    arn: str,
    status: ClusterStatusType,  # (1)
    creationTime: datetime,
    deletionProtectionEnabled: bool,
    witnessRegion: str,
    linkedClusterArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMultiRegionClustersInputTypeDef

```python
# CreateMultiRegionClustersInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import CreateMultiRegionClustersInputTypeDef


def get_value() -> CreateMultiRegionClustersInputTypeDef:
    return {
        "linkedRegionList": ...,
    }


# CreateMultiRegionClustersInputTypeDef definition

class CreateMultiRegionClustersInputTypeDef(TypedDict):
    linkedRegionList: Sequence[str],
    witnessRegion: str,
    clusterProperties: NotRequired[Mapping[str, LinkedClusterPropertiesTypeDef]],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: LinkedClusterPropertiesTypeDef](./type_defs.md#linkedclusterpropertiestypedef) 
## GetClusterInputWaitExtraTypeDef

```python
# GetClusterInputWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import GetClusterInputWaitExtraTypeDef


def get_value() -> GetClusterInputWaitExtraTypeDef:
    return {
        "identifier": ...,
    }


# GetClusterInputWaitExtraTypeDef definition

class GetClusterInputWaitExtraTypeDef(TypedDict):
    identifier: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetClusterInputWaitTypeDef

```python
# GetClusterInputWaitTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import GetClusterInputWaitTypeDef


def get_value() -> GetClusterInputWaitTypeDef:
    return {
        "identifier": ...,
    }


# GetClusterInputWaitTypeDef definition

class GetClusterInputWaitTypeDef(TypedDict):
    identifier: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## ListClustersInputPaginateTypeDef

```python
# ListClustersInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ListClustersInputPaginateTypeDef


def get_value() -> ListClustersInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListClustersInputPaginateTypeDef definition

class ListClustersInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
