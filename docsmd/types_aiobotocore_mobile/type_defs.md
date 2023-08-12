# Type definitions

> [Index](../README.md) > [Mobile](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Mobile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
    type annotations stubs module [types-aiobotocore-mobile](https://pypi.org/project/types-aiobotocore-mobile/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## BundleDetailsTypeDef

```python
# BundleDetailsTypeDef definition

class BundleDetailsTypeDef(TypedDict):
    bundleId: NotRequired[str],
    title: NotRequired[str],
    version: NotRequired[str],
    description: NotRequired[str],
    iconUrl: NotRequired[str],
    availablePlatforms: NotRequired[List[PlatformType]],  # (1)
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
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

## DeleteProjectRequestRequestTypeDef

```python
# DeleteProjectRequestRequestTypeDef definition

class DeleteProjectRequestRequestTypeDef(TypedDict):
    projectId: str,
```

## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    type: NotRequired[str],
    name: NotRequired[str],
    arn: NotRequired[str],
    feature: NotRequired[str],
    attributes: NotRequired[Dict[str, str]],
```

## DescribeBundleRequestRequestTypeDef

```python
# DescribeBundleRequestRequestTypeDef definition

class DescribeBundleRequestRequestTypeDef(TypedDict):
    bundleId: str,
```

## DescribeProjectRequestRequestTypeDef

```python
# DescribeProjectRequestRequestTypeDef definition

class DescribeProjectRequestRequestTypeDef(TypedDict):
    projectId: str,
    syncFromResources: NotRequired[bool],
```

## ExportBundleRequestRequestTypeDef

```python
# ExportBundleRequestRequestTypeDef definition

class ExportBundleRequestRequestTypeDef(TypedDict):
    bundleId: str,
    projectId: NotRequired[str],
    platform: NotRequired[PlatformType],  # (1)
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
## ExportProjectRequestRequestTypeDef

```python
# ExportProjectRequestRequestTypeDef definition

class ExportProjectRequestRequestTypeDef(TypedDict):
    projectId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListBundlesRequestRequestTypeDef

```python
# ListBundlesRequestRequestTypeDef definition

class ListBundlesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListProjectsRequestRequestTypeDef

```python
# ListProjectsRequestRequestTypeDef definition

class ListProjectsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ProjectSummaryTypeDef

```python
# ProjectSummaryTypeDef definition

class ProjectSummaryTypeDef(TypedDict):
    name: NotRequired[str],
    projectId: NotRequired[str],
```

## CreateProjectRequestRequestTypeDef

```python
# CreateProjectRequestRequestTypeDef definition

class CreateProjectRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    region: NotRequired[str],
    contents: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    snapshotId: NotRequired[str],
```

## UpdateProjectRequestRequestTypeDef

```python
# UpdateProjectRequestRequestTypeDef definition

class UpdateProjectRequestRequestTypeDef(TypedDict):
    projectId: str,
    contents: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
```

## DescribeBundleResultTypeDef

```python
# DescribeBundleResultTypeDef definition

class DescribeBundleResultTypeDef(TypedDict):
    details: BundleDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BundleDetailsTypeDef](./type_defs.md#bundledetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportBundleResultTypeDef

```python
# ExportBundleResultTypeDef definition

class ExportBundleResultTypeDef(TypedDict):
    downloadUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportProjectResultTypeDef

```python
# ExportProjectResultTypeDef definition

class ExportProjectResultTypeDef(TypedDict):
    downloadUrl: str,
    shareUrl: str,
    snapshotId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBundlesResultTypeDef

```python
# ListBundlesResultTypeDef definition

class ListBundlesResultTypeDef(TypedDict):
    bundleList: List[BundleDetailsTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BundleDetailsTypeDef](./type_defs.md#bundledetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProjectResultTypeDef

```python
# DeleteProjectResultTypeDef definition

class DeleteProjectResultTypeDef(TypedDict):
    deletedResources: List[ResourceTypeDef],  # (1)
    orphanedResources: List[ResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProjectDetailsTypeDef

```python
# ProjectDetailsTypeDef definition

class ProjectDetailsTypeDef(TypedDict):
    name: NotRequired[str],
    projectId: NotRequired[str],
    region: NotRequired[str],
    state: NotRequired[ProjectStateType],  # (1)
    createdDate: NotRequired[datetime],
    lastUpdatedDate: NotRequired[datetime],
    consoleUrl: NotRequired[str],
    resources: NotRequired[List[ResourceTypeDef]],  # (2)
```

1. See [:material-code-brackets: ProjectStateType](./literals.md#projectstatetype) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
## ListBundlesRequestListBundlesPaginateTypeDef

```python
# ListBundlesRequestListBundlesPaginateTypeDef definition

class ListBundlesRequestListBundlesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsRequestListProjectsPaginateTypeDef

```python
# ListProjectsRequestListProjectsPaginateTypeDef definition

class ListProjectsRequestListProjectsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsResultTypeDef

```python
# ListProjectsResultTypeDef definition

class ListProjectsResultTypeDef(TypedDict):
    projects: List[ProjectSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectResultTypeDef

```python
# CreateProjectResultTypeDef definition

class CreateProjectResultTypeDef(TypedDict):
    details: ProjectDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectDetailsTypeDef](./type_defs.md#projectdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProjectResultTypeDef

```python
# DescribeProjectResultTypeDef definition

class DescribeProjectResultTypeDef(TypedDict):
    details: ProjectDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectDetailsTypeDef](./type_defs.md#projectdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectResultTypeDef

```python
# UpdateProjectResultTypeDef definition

class UpdateProjectResultTypeDef(TypedDict):
    details: ProjectDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectDetailsTypeDef](./type_defs.md#projectdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
