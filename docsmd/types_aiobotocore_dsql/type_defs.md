# Type definitions

> [Index](../README.md) > [AuroraDSQL](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AuroraDSQL](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql.html#auroradsql)
    type annotations stubs module [types-aiobotocore-dsql](https://pypi.org/project/types-aiobotocore-dsql/).



## ClusterSummaryTypeDef

```python
# ClusterSummaryTypeDef definition

class ClusterSummaryTypeDef(TypedDict):
    identifier: str,
    arn: str,
```

## CreateClusterInputRequestTypeDef

```python
# CreateClusterInputRequestTypeDef definition

class CreateClusterInputRequestTypeDef(TypedDict):
    deletionProtectionEnabled: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
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

## LinkedClusterPropertiesTypeDef

```python
# LinkedClusterPropertiesTypeDef definition

class LinkedClusterPropertiesTypeDef(TypedDict):
    deletionProtectionEnabled: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
```

## DeleteClusterInputRequestTypeDef

```python
# DeleteClusterInputRequestTypeDef definition

class DeleteClusterInputRequestTypeDef(TypedDict):
    identifier: str,
    clientToken: NotRequired[str],
```

## DeleteMultiRegionClustersInputRequestTypeDef

```python
# DeleteMultiRegionClustersInputRequestTypeDef definition

class DeleteMultiRegionClustersInputRequestTypeDef(TypedDict):
    linkedClusterArns: Sequence[str],
    clientToken: NotRequired[str],
```

## GetClusterInputRequestTypeDef

```python
# GetClusterInputRequestTypeDef definition

class GetClusterInputRequestTypeDef(TypedDict):
    identifier: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListClustersInputRequestTypeDef

```python
# ListClustersInputRequestTypeDef definition

class ListClustersInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateClusterInputRequestTypeDef

```python
# UpdateClusterInputRequestTypeDef definition

class UpdateClusterInputRequestTypeDef(TypedDict):
    identifier: str,
    deletionProtectionEnabled: NotRequired[bool],
    clientToken: NotRequired[str],
```

## CreateClusterOutputTypeDef

```python
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
# CreateMultiRegionClustersOutputTypeDef definition

class CreateMultiRegionClustersOutputTypeDef(TypedDict):
    linkedClusterArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteClusterOutputTypeDef

```python
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
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetClusterOutputTypeDef

```python
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
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterOutputTypeDef

```python
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
## CreateMultiRegionClustersInputRequestTypeDef

```python
# CreateMultiRegionClustersInputRequestTypeDef definition

class CreateMultiRegionClustersInputRequestTypeDef(TypedDict):
    linkedRegionList: Sequence[str],
    witnessRegion: str,
    clusterProperties: NotRequired[Mapping[str, LinkedClusterPropertiesTypeDef]],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: LinkedClusterPropertiesTypeDef](./type_defs.md#linkedclusterpropertiestypedef) 
## GetClusterInputWaitTypeDef

```python
# GetClusterInputWaitTypeDef definition

class GetClusterInputWaitTypeDef(TypedDict):
    identifier: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## ListClustersInputPaginateTypeDef

```python
# ListClustersInputPaginateTypeDef definition

class ListClustersInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
