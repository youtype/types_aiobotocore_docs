<a id="typed-dictionaries-for-aiobotocore-mobile-module"></a>

# Typed dictionaries for aiobotocore Mobile module

> [Index](..) > [Mobile](.) > Typed dictionaries

Auto-generated documentation for
[Mobile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
type annotations stubs module
[types-aiobotocore-mobile](https://pypi.org/project/types-aiobotocore-mobile/).

- [Typed dictionaries for aiobotocore Mobile module](#typed-dictionaries-for-aiobotocore-mobile-module)
  - [BundleDetailsTypeDef](#bundledetailstypedef)
  - [CreateProjectRequestRequestTypeDef](#createprojectrequestrequesttypedef)
  - [CreateProjectResultTypeDef](#createprojectresulttypedef)
  - [DeleteProjectRequestRequestTypeDef](#deleteprojectrequestrequesttypedef)
  - [DeleteProjectResultTypeDef](#deleteprojectresulttypedef)
  - [DescribeBundleRequestRequestTypeDef](#describebundlerequestrequesttypedef)
  - [DescribeBundleResultTypeDef](#describebundleresulttypedef)
  - [DescribeProjectRequestRequestTypeDef](#describeprojectrequestrequesttypedef)
  - [DescribeProjectResultTypeDef](#describeprojectresulttypedef)
  - [ExportBundleRequestRequestTypeDef](#exportbundlerequestrequesttypedef)
  - [ExportBundleResultTypeDef](#exportbundleresulttypedef)
  - [ExportProjectRequestRequestTypeDef](#exportprojectrequestrequesttypedef)
  - [ExportProjectResultTypeDef](#exportprojectresulttypedef)
  - [ListBundlesRequestRequestTypeDef](#listbundlesrequestrequesttypedef)
  - [ListBundlesResultTypeDef](#listbundlesresulttypedef)
  - [ListProjectsRequestRequestTypeDef](#listprojectsrequestrequesttypedef)
  - [ListProjectsResultTypeDef](#listprojectsresulttypedef)
  - [PaginatorConfigTypeDef](#paginatorconfigtypedef)
  - [ProjectDetailsTypeDef](#projectdetailstypedef)
  - [ProjectSummaryTypeDef](#projectsummarytypedef)
  - [ResourceTypeDef](#resourcetypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [UpdateProjectRequestRequestTypeDef](#updateprojectrequestrequesttypedef)
  - [UpdateProjectResultTypeDef](#updateprojectresulttypedef)

<a id="bundledetailstypedef"></a>

## BundleDetailsTypeDef

```python
from types_aiobotocore_mobile.type_defs import BundleDetailsTypeDef
```

Optional fields:

- `bundleId`: `str`
- `title`: `str`
- `version`: `str`
- `description`: `str`
- `iconUrl`: `str`
- `availablePlatforms`: `List`\[[PlatformType](./literals.md#platformtype)\]

<a id="createprojectrequestrequesttypedef"></a>

## CreateProjectRequestRequestTypeDef

```python
from types_aiobotocore_mobile.type_defs import CreateProjectRequestRequestTypeDef
```

Optional fields:

- `name`: `str`
- `region`: `str`
- `contents`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]
- `snapshotId`: `str`

<a id="createprojectresulttypedef"></a>

## CreateProjectResultTypeDef

```python
from types_aiobotocore_mobile.type_defs import CreateProjectResultTypeDef
```

Required fields:

- `details`: [ProjectDetailsTypeDef](./type_defs.md#projectdetailstypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deleteprojectrequestrequesttypedef"></a>

## DeleteProjectRequestRequestTypeDef

```python
from types_aiobotocore_mobile.type_defs import DeleteProjectRequestRequestTypeDef
```

Required fields:

- `projectId`: `str`

<a id="deleteprojectresulttypedef"></a>

## DeleteProjectResultTypeDef

```python
from types_aiobotocore_mobile.type_defs import DeleteProjectResultTypeDef
```

Required fields:

- `deletedResources`:
  `List`\[[ResourceTypeDef](./type_defs.md#resourcetypedef)\]
- `orphanedResources`:
  `List`\[[ResourceTypeDef](./type_defs.md#resourcetypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describebundlerequestrequesttypedef"></a>

## DescribeBundleRequestRequestTypeDef

```python
from types_aiobotocore_mobile.type_defs import DescribeBundleRequestRequestTypeDef
```

Required fields:

- `bundleId`: `str`

<a id="describebundleresulttypedef"></a>

## DescribeBundleResultTypeDef

```python
from types_aiobotocore_mobile.type_defs import DescribeBundleResultTypeDef
```

Required fields:

- `details`: [BundleDetailsTypeDef](./type_defs.md#bundledetailstypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describeprojectrequestrequesttypedef"></a>

## DescribeProjectRequestRequestTypeDef

```python
from types_aiobotocore_mobile.type_defs import DescribeProjectRequestRequestTypeDef
```

Required fields:

- `projectId`: `str`

Optional fields:

- `syncFromResources`: `bool`

<a id="describeprojectresulttypedef"></a>

## DescribeProjectResultTypeDef

```python
from types_aiobotocore_mobile.type_defs import DescribeProjectResultTypeDef
```

Required fields:

- `details`: [ProjectDetailsTypeDef](./type_defs.md#projectdetailstypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="exportbundlerequestrequesttypedef"></a>

## ExportBundleRequestRequestTypeDef

```python
from types_aiobotocore_mobile.type_defs import ExportBundleRequestRequestTypeDef
```

Required fields:

- `bundleId`: `str`

Optional fields:

- `projectId`: `str`
- `platform`: [PlatformType](./literals.md#platformtype)

<a id="exportbundleresulttypedef"></a>

## ExportBundleResultTypeDef

```python
from types_aiobotocore_mobile.type_defs import ExportBundleResultTypeDef
```

Required fields:

- `downloadUrl`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="exportprojectrequestrequesttypedef"></a>

## ExportProjectRequestRequestTypeDef

```python
from types_aiobotocore_mobile.type_defs import ExportProjectRequestRequestTypeDef
```

Required fields:

- `projectId`: `str`

<a id="exportprojectresulttypedef"></a>

## ExportProjectResultTypeDef

```python
from types_aiobotocore_mobile.type_defs import ExportProjectResultTypeDef
```

Required fields:

- `downloadUrl`: `str`
- `shareUrl`: `str`
- `snapshotId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listbundlesrequestrequesttypedef"></a>

## ListBundlesRequestRequestTypeDef

```python
from types_aiobotocore_mobile.type_defs import ListBundlesRequestRequestTypeDef
```

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="listbundlesresulttypedef"></a>

## ListBundlesResultTypeDef

```python
from types_aiobotocore_mobile.type_defs import ListBundlesResultTypeDef
```

Required fields:

- `bundleList`:
  `List`\[[BundleDetailsTypeDef](./type_defs.md#bundledetailstypedef)\]
- `nextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listprojectsrequestrequesttypedef"></a>

## ListProjectsRequestRequestTypeDef

```python
from types_aiobotocore_mobile.type_defs import ListProjectsRequestRequestTypeDef
```

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="listprojectsresulttypedef"></a>

## ListProjectsResultTypeDef

```python
from types_aiobotocore_mobile.type_defs import ListProjectsResultTypeDef
```

Required fields:

- `projects`:
  `List`\[[ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef)\]
- `nextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="paginatorconfigtypedef"></a>

## PaginatorConfigTypeDef

```python
from types_aiobotocore_mobile.type_defs import PaginatorConfigTypeDef
```

Optional fields:

- `MaxItems`: `int`
- `PageSize`: `int`
- `StartingToken`: `str`

<a id="projectdetailstypedef"></a>

## ProjectDetailsTypeDef

```python
from types_aiobotocore_mobile.type_defs import ProjectDetailsTypeDef
```

Optional fields:

- `name`: `str`
- `projectId`: `str`
- `region`: `str`
- `state`: [ProjectStateType](./literals.md#projectstatetype)
- `createdDate`: `datetime`
- `lastUpdatedDate`: `datetime`
- `consoleUrl`: `str`
- `resources`: `List`\[[ResourceTypeDef](./type_defs.md#resourcetypedef)\]

<a id="projectsummarytypedef"></a>

## ProjectSummaryTypeDef

```python
from types_aiobotocore_mobile.type_defs import ProjectSummaryTypeDef
```

Optional fields:

- `name`: `str`
- `projectId`: `str`

<a id="resourcetypedef"></a>

## ResourceTypeDef

```python
from types_aiobotocore_mobile.type_defs import ResourceTypeDef
```

Optional fields:

- `type`: `str`
- `name`: `str`
- `arn`: `str`
- `feature`: `str`
- `attributes`: `Dict`\[`str`, `str`\]

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_mobile.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="updateprojectrequestrequesttypedef"></a>

## UpdateProjectRequestRequestTypeDef

```python
from types_aiobotocore_mobile.type_defs import UpdateProjectRequestRequestTypeDef
```

Required fields:

- `projectId`: `str`

Optional fields:

- `contents`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]

<a id="updateprojectresulttypedef"></a>

## UpdateProjectResultTypeDef

```python
from types_aiobotocore_mobile.type_defs import UpdateProjectResultTypeDef
```

Required fields:

- `details`: [ProjectDetailsTypeDef](./type_defs.md#projectdetailstypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
