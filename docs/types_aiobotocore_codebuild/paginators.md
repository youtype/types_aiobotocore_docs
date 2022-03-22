<a id="paginators-for-aiobotocore-codebuild-module"></a>

# Paginators for aiobotocore CodeBuild module

> [Index](../README.md) > [CodeBuild](./README.md) > Paginators

Auto-generated documentation for
[CodeBuild](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
type annotations stubs module
[types-aiobotocore-codebuild](https://pypi.org/project/types-aiobotocore-codebuild/).

- [Paginators for aiobotocore CodeBuild module](#paginators-for-aiobotocore-codebuild-module)
  - [DescribeCodeCoveragesPaginator](#describecodecoveragespaginator)
  - [DescribeTestCasesPaginator](#describetestcasespaginator)
  - [ListBuildBatchesPaginator](#listbuildbatchespaginator)
  - [ListBuildBatchesForProjectPaginator](#listbuildbatchesforprojectpaginator)
  - [ListBuildsPaginator](#listbuildspaginator)
  - [ListBuildsForProjectPaginator](#listbuildsforprojectpaginator)
  - [ListProjectsPaginator](#listprojectspaginator)
  - [ListReportGroupsPaginator](#listreportgroupspaginator)
  - [ListReportsPaginator](#listreportspaginator)
  - [ListReportsForReportGroupPaginator](#listreportsforreportgrouppaginator)
  - [ListSharedProjectsPaginator](#listsharedprojectspaginator)
  - [ListSharedReportGroupsPaginator](#listsharedreportgroupspaginator)

<a id="describecodecoveragespaginator"></a>

## DescribeCodeCoveragesPaginator

Type annotations for
`session.create_client("codebuild").get_paginator("describe_code_coverages")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import DescribeCodeCoveragesPaginator

session = get_session()
async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    paginator: DescribeCodeCoveragesPaginator = client.get_paginator("describe_code_coverages")
```

Boto3 documentation:
[CodeBuild.Paginator.DescribeCodeCoverages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeCodeCoverages)

Arguments for `DescribeCodeCoveragesPaginator.paginate` method:

- `reportArn`: `str` *(required)*
- `sortOrder`: [SortOrderTypeType](./literals.md#sortordertypetype)
- `sortBy`:
  [ReportCodeCoverageSortByTypeType](./literals.md#reportcodecoveragesortbytypetype)
- `minLineCoveragePercentage`: `float`
- `maxLineCoveragePercentage`: `float`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeCodeCoveragesPaginator.paginate` returns
`AsyncIterator`\[[DescribeCodeCoveragesOutputTypeDef](./type_defs.md#describecodecoveragesoutputtypedef)\].

<a id="describetestcasespaginator"></a>

## DescribeTestCasesPaginator

Type annotations for
`session.create_client("codebuild").get_paginator("describe_test_cases")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import DescribeTestCasesPaginator

session = get_session()
async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    paginator: DescribeTestCasesPaginator = client.get_paginator("describe_test_cases")
```

Boto3 documentation:
[CodeBuild.Paginator.DescribeTestCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeTestCases)

Arguments for `DescribeTestCasesPaginator.paginate` method:

- `reportArn`: `str` *(required)*
- `filter`: [TestCaseFilterTypeDef](./type_defs.md#testcasefiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeTestCasesPaginator.paginate` returns
`AsyncIterator`\[[DescribeTestCasesOutputTypeDef](./type_defs.md#describetestcasesoutputtypedef)\].

<a id="listbuildbatchespaginator"></a>

## ListBuildBatchesPaginator

Type annotations for
`session.create_client("codebuild").get_paginator("list_build_batches")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListBuildBatchesPaginator

session = get_session()
async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    paginator: ListBuildBatchesPaginator = client.get_paginator("list_build_batches")
```

Boto3 documentation:
[CodeBuild.Paginator.ListBuildBatches](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatches)

Arguments for `ListBuildBatchesPaginator.paginate` method:

- `filter`: [BuildBatchFilterTypeDef](./type_defs.md#buildbatchfiltertypedef)
- `sortOrder`: [SortOrderTypeType](./literals.md#sortordertypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBuildBatchesPaginator.paginate` returns
`AsyncIterator`\[[ListBuildBatchesOutputTypeDef](./type_defs.md#listbuildbatchesoutputtypedef)\].

<a id="listbuildbatchesforprojectpaginator"></a>

## ListBuildBatchesForProjectPaginator

Type annotations for
`session.create_client("codebuild").get_paginator("list_build_batches_for_project")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListBuildBatchesForProjectPaginator

session = get_session()
async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    paginator: ListBuildBatchesForProjectPaginator = client.get_paginator("list_build_batches_for_project")
```

Boto3 documentation:
[CodeBuild.Paginator.ListBuildBatchesForProject](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatchesForProject)

Arguments for `ListBuildBatchesForProjectPaginator.paginate` method:

- `projectName`: `str`
- `filter`: [BuildBatchFilterTypeDef](./type_defs.md#buildbatchfiltertypedef)
- `sortOrder`: [SortOrderTypeType](./literals.md#sortordertypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBuildBatchesForProjectPaginator.paginate` returns
`AsyncIterator`\[[ListBuildBatchesForProjectOutputTypeDef](./type_defs.md#listbuildbatchesforprojectoutputtypedef)\].

<a id="listbuildspaginator"></a>

## ListBuildsPaginator

Type annotations for
`session.create_client("codebuild").get_paginator("list_builds")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListBuildsPaginator

session = get_session()
async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    paginator: ListBuildsPaginator = client.get_paginator("list_builds")
```

Boto3 documentation:
[CodeBuild.Paginator.ListBuilds](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds)

Arguments for `ListBuildsPaginator.paginate` method:

- `sortOrder`: [SortOrderTypeType](./literals.md#sortordertypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBuildsPaginator.paginate` returns
`AsyncIterator`\[[ListBuildsOutputTypeDef](./type_defs.md#listbuildsoutputtypedef)\].

<a id="listbuildsforprojectpaginator"></a>

## ListBuildsForProjectPaginator

Type annotations for
`session.create_client("codebuild").get_paginator("list_builds_for_project")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListBuildsForProjectPaginator

session = get_session()
async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    paginator: ListBuildsForProjectPaginator = client.get_paginator("list_builds_for_project")
```

Boto3 documentation:
[CodeBuild.Paginator.ListBuildsForProject](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildsForProject)

Arguments for `ListBuildsForProjectPaginator.paginate` method:

- `projectName`: `str` *(required)*
- `sortOrder`: [SortOrderTypeType](./literals.md#sortordertypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBuildsForProjectPaginator.paginate` returns
`AsyncIterator`\[[ListBuildsForProjectOutputTypeDef](./type_defs.md#listbuildsforprojectoutputtypedef)\].

<a id="listprojectspaginator"></a>

## ListProjectsPaginator

Type annotations for
`session.create_client("codebuild").get_paginator("list_projects")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")
```

Boto3 documentation:
[CodeBuild.Paginator.ListProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListProjects)

Arguments for `ListProjectsPaginator.paginate` method:

- `sortBy`: [ProjectSortByTypeType](./literals.md#projectsortbytypetype)
- `sortOrder`: [SortOrderTypeType](./literals.md#sortordertypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListProjectsPaginator.paginate` returns
`AsyncIterator`\[[ListProjectsOutputTypeDef](./type_defs.md#listprojectsoutputtypedef)\].

<a id="listreportgroupspaginator"></a>

## ListReportGroupsPaginator

Type annotations for
`session.create_client("codebuild").get_paginator("list_report_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListReportGroupsPaginator

session = get_session()
async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    paginator: ListReportGroupsPaginator = client.get_paginator("list_report_groups")
```

Boto3 documentation:
[CodeBuild.Paginator.ListReportGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportGroups)

Arguments for `ListReportGroupsPaginator.paginate` method:

- `sortOrder`: [SortOrderTypeType](./literals.md#sortordertypetype)
- `sortBy`:
  [ReportGroupSortByTypeType](./literals.md#reportgroupsortbytypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListReportGroupsPaginator.paginate` returns
`AsyncIterator`\[[ListReportGroupsOutputTypeDef](./type_defs.md#listreportgroupsoutputtypedef)\].

<a id="listreportspaginator"></a>

## ListReportsPaginator

Type annotations for
`session.create_client("codebuild").get_paginator("list_reports")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListReportsPaginator

session = get_session()
async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    paginator: ListReportsPaginator = client.get_paginator("list_reports")
```

Boto3 documentation:
[CodeBuild.Paginator.ListReports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReports)

Arguments for `ListReportsPaginator.paginate` method:

- `sortOrder`: [SortOrderTypeType](./literals.md#sortordertypetype)
- `filter`: [ReportFilterTypeDef](./type_defs.md#reportfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListReportsPaginator.paginate` returns
`AsyncIterator`\[[ListReportsOutputTypeDef](./type_defs.md#listreportsoutputtypedef)\].

<a id="listreportsforreportgrouppaginator"></a>

## ListReportsForReportGroupPaginator

Type annotations for
`session.create_client("codebuild").get_paginator("list_reports_for_report_group")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListReportsForReportGroupPaginator

session = get_session()
async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    paginator: ListReportsForReportGroupPaginator = client.get_paginator("list_reports_for_report_group")
```

Boto3 documentation:
[CodeBuild.Paginator.ListReportsForReportGroup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportsForReportGroup)

Arguments for `ListReportsForReportGroupPaginator.paginate` method:

- `reportGroupArn`: `str` *(required)*
- `sortOrder`: [SortOrderTypeType](./literals.md#sortordertypetype)
- `filter`: [ReportFilterTypeDef](./type_defs.md#reportfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListReportsForReportGroupPaginator.paginate` returns
`AsyncIterator`\[[ListReportsForReportGroupOutputTypeDef](./type_defs.md#listreportsforreportgroupoutputtypedef)\].

<a id="listsharedprojectspaginator"></a>

## ListSharedProjectsPaginator

Type annotations for
`session.create_client("codebuild").get_paginator("list_shared_projects")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListSharedProjectsPaginator

session = get_session()
async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    paginator: ListSharedProjectsPaginator = client.get_paginator("list_shared_projects")
```

Boto3 documentation:
[CodeBuild.Paginator.ListSharedProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedProjects)

Arguments for `ListSharedProjectsPaginator.paginate` method:

- `sortBy`:
  [SharedResourceSortByTypeType](./literals.md#sharedresourcesortbytypetype)
- `sortOrder`: [SortOrderTypeType](./literals.md#sortordertypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSharedProjectsPaginator.paginate` returns
`AsyncIterator`\[[ListSharedProjectsOutputTypeDef](./type_defs.md#listsharedprojectsoutputtypedef)\].

<a id="listsharedreportgroupspaginator"></a>

## ListSharedReportGroupsPaginator

Type annotations for
`session.create_client("codebuild").get_paginator("list_shared_report_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListSharedReportGroupsPaginator

session = get_session()
async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    paginator: ListSharedReportGroupsPaginator = client.get_paginator("list_shared_report_groups")
```

Boto3 documentation:
[CodeBuild.Paginator.ListSharedReportGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedReportGroups)

Arguments for `ListSharedReportGroupsPaginator.paginate` method:

- `sortOrder`: [SortOrderTypeType](./literals.md#sortordertypetype)
- `sortBy`:
  [SharedResourceSortByTypeType](./literals.md#sharedresourcesortbytypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSharedReportGroupsPaginator.paginate` returns
`AsyncIterator`\[[ListSharedReportGroupsOutputTypeDef](./type_defs.md#listsharedreportgroupsoutputtypedef)\].
