# Paginators

> [Index](../README.md) > [CodeBuild](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeBuild](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
    type annotations stubs module [types-aiobotocore-codebuild](https://pypi.org/project/types-aiobotocore-codebuild/).

## DescribeCodeCoveragesPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("describe_code_coverages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeCodeCoverages)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import DescribeCodeCoveragesPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: DescribeCodeCoveragesPaginator = client.get_paginator("describe_code_coverages")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCodeCoveragesOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [DescribeCodeCoveragesPaginator](./paginators.md#describecodecoveragespaginator)
3. item: [:material-code-braces: DescribeCodeCoveragesOutputTypeDef](./type_defs.md#describecodecoveragesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCodeCoveragesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    reportArn: str,
    sortOrder: SortOrderTypeType = ...,  # (1)
    sortBy: ReportCodeCoverageSortByTypeType = ...,  # (2)
    minLineCoveragePercentage: float = ...,
    maxLineCoveragePercentage: float = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeCodeCoveragesOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-brackets: ReportCodeCoverageSortByTypeType](./literals.md#reportcodecoveragesortbytypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeCodeCoveragesOutputTypeDef](./type_defs.md#describecodecoveragesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = {  # (1)
    "reportArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef](./type_defs.md#describecodecoveragesinputdescribecodecoveragespaginatetypedef) 
## DescribeTestCasesPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("describe_test_cases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeTestCases)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import DescribeTestCasesPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: DescribeTestCasesPaginator = client.get_paginator("describe_test_cases")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTestCasesOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [DescribeTestCasesPaginator](./paginators.md#describetestcasespaginator)
3. item: [:material-code-braces: DescribeTestCasesOutputTypeDef](./type_defs.md#describetestcasesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTestCasesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    reportArn: str,
    filter: TestCaseFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTestCasesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TestCaseFilterTypeDef](./type_defs.md#testcasefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTestCasesOutputTypeDef](./type_defs.md#describetestcasesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTestCasesInputDescribeTestCasesPaginateTypeDef = {  # (1)
    "reportArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTestCasesInputDescribeTestCasesPaginateTypeDef](./type_defs.md#describetestcasesinputdescribetestcasespaginatetypedef) 
## ListBuildBatchesPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_build_batches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatches)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListBuildBatchesPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: ListBuildBatchesPaginator = client.get_paginator("list_build_batches")  # (2)
    async for item in paginator.paginate(...):
        item: ListBuildBatchesOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [ListBuildBatchesPaginator](./paginators.md#listbuildbatchespaginator)
3. item: [:material-code-braces: ListBuildBatchesOutputTypeDef](./type_defs.md#listbuildbatchesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBuildBatchesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filter: BuildBatchFilterTypeDef = ...,  # (1)
    sortOrder: SortOrderTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListBuildBatchesOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: BuildBatchFilterTypeDef](./type_defs.md#buildbatchfiltertypedef) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListBuildBatchesOutputTypeDef](./type_defs.md#listbuildbatchesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListBuildBatchesInputListBuildBatchesPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBuildBatchesInputListBuildBatchesPaginateTypeDef](./type_defs.md#listbuildbatchesinputlistbuildbatchespaginatetypedef) 
## ListBuildBatchesForProjectPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_build_batches_for_project")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatchesForProject)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListBuildBatchesForProjectPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: ListBuildBatchesForProjectPaginator = client.get_paginator("list_build_batches_for_project")  # (2)
    async for item in paginator.paginate(...):
        item: ListBuildBatchesForProjectOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [ListBuildBatchesForProjectPaginator](./paginators.md#listbuildbatchesforprojectpaginator)
3. item: [:material-code-braces: ListBuildBatchesForProjectOutputTypeDef](./type_defs.md#listbuildbatchesforprojectoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBuildBatchesForProjectPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    projectName: str = ...,
    filter: BuildBatchFilterTypeDef = ...,  # (1)
    sortOrder: SortOrderTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListBuildBatchesForProjectOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: BuildBatchFilterTypeDef](./type_defs.md#buildbatchfiltertypedef) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListBuildBatchesForProjectOutputTypeDef](./type_defs.md#listbuildbatchesforprojectoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = {  # (1)
    "projectName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef](./type_defs.md#listbuildbatchesforprojectinputlistbuildbatchesforprojectpaginatetypedef) 
## ListBuildsPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_builds")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListBuildsPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: ListBuildsPaginator = client.get_paginator("list_builds")  # (2)
    async for item in paginator.paginate(...):
        item: ListBuildsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [ListBuildsPaginator](./paginators.md#listbuildspaginator)
3. item: [:material-code-braces: ListBuildsOutputTypeDef](./type_defs.md#listbuildsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBuildsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    sortOrder: SortOrderTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListBuildsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListBuildsOutputTypeDef](./type_defs.md#listbuildsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListBuildsInputListBuildsPaginateTypeDef = {  # (1)
    "sortOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBuildsInputListBuildsPaginateTypeDef](./type_defs.md#listbuildsinputlistbuildspaginatetypedef) 
## ListBuildsForProjectPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_builds_for_project")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildsForProject)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListBuildsForProjectPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: ListBuildsForProjectPaginator = client.get_paginator("list_builds_for_project")  # (2)
    async for item in paginator.paginate(...):
        item: ListBuildsForProjectOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [ListBuildsForProjectPaginator](./paginators.md#listbuildsforprojectpaginator)
3. item: [:material-code-braces: ListBuildsForProjectOutputTypeDef](./type_defs.md#listbuildsforprojectoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBuildsForProjectPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    projectName: str,
    sortOrder: SortOrderTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListBuildsForProjectOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListBuildsForProjectOutputTypeDef](./type_defs.md#listbuildsforprojectoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = {  # (1)
    "projectName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef](./type_defs.md#listbuildsforprojectinputlistbuildsforprojectpaginatetypedef) 
## ListProjectsPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListProjects)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: [:material-code-braces: ListProjectsOutputTypeDef](./type_defs.md#listprojectsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    sortBy: ProjectSortByTypeType = ...,  # (1)
    sortOrder: SortOrderTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListProjectsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ProjectSortByTypeType](./literals.md#projectsortbytypetype) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListProjectsOutputTypeDef](./type_defs.md#listprojectsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListProjectsInputListProjectsPaginateTypeDef = {  # (1)
    "sortBy": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsInputListProjectsPaginateTypeDef](./type_defs.md#listprojectsinputlistprojectspaginatetypedef) 
## ListReportGroupsPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_report_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListReportGroupsPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: ListReportGroupsPaginator = client.get_paginator("list_report_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListReportGroupsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [ListReportGroupsPaginator](./paginators.md#listreportgroupspaginator)
3. item: [:material-code-braces: ListReportGroupsOutputTypeDef](./type_defs.md#listreportgroupsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListReportGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    sortOrder: SortOrderTypeType = ...,  # (1)
    sortBy: ReportGroupSortByTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListReportGroupsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-brackets: ReportGroupSortByTypeType](./literals.md#reportgroupsortbytypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListReportGroupsOutputTypeDef](./type_defs.md#listreportgroupsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListReportGroupsInputListReportGroupsPaginateTypeDef = {  # (1)
    "sortOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReportGroupsInputListReportGroupsPaginateTypeDef](./type_defs.md#listreportgroupsinputlistreportgroupspaginatetypedef) 
## ListReportsPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_reports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReports)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListReportsPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: ListReportsPaginator = client.get_paginator("list_reports")  # (2)
    async for item in paginator.paginate(...):
        item: ListReportsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [ListReportsPaginator](./paginators.md#listreportspaginator)
3. item: [:material-code-braces: ListReportsOutputTypeDef](./type_defs.md#listreportsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListReportsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    sortOrder: SortOrderTypeType = ...,  # (1)
    filter: ReportFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListReportsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-braces: ReportFilterTypeDef](./type_defs.md#reportfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListReportsOutputTypeDef](./type_defs.md#listreportsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListReportsInputListReportsPaginateTypeDef = {  # (1)
    "sortOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReportsInputListReportsPaginateTypeDef](./type_defs.md#listreportsinputlistreportspaginatetypedef) 
## ListReportsForReportGroupPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_reports_for_report_group")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportsForReportGroup)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListReportsForReportGroupPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: ListReportsForReportGroupPaginator = client.get_paginator("list_reports_for_report_group")  # (2)
    async for item in paginator.paginate(...):
        item: ListReportsForReportGroupOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [ListReportsForReportGroupPaginator](./paginators.md#listreportsforreportgrouppaginator)
3. item: [:material-code-braces: ListReportsForReportGroupOutputTypeDef](./type_defs.md#listreportsforreportgroupoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListReportsForReportGroupPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    reportGroupArn: str,
    sortOrder: SortOrderTypeType = ...,  # (1)
    filter: ReportFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListReportsForReportGroupOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-braces: ReportFilterTypeDef](./type_defs.md#reportfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListReportsForReportGroupOutputTypeDef](./type_defs.md#listreportsforreportgroupoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef = {  # (1)
    "reportGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef](./type_defs.md#listreportsforreportgroupinputlistreportsforreportgrouppaginatetypedef) 
## ListSharedProjectsPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_shared_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedProjects)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListSharedProjectsPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: ListSharedProjectsPaginator = client.get_paginator("list_shared_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListSharedProjectsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [ListSharedProjectsPaginator](./paginators.md#listsharedprojectspaginator)
3. item: [:material-code-braces: ListSharedProjectsOutputTypeDef](./type_defs.md#listsharedprojectsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSharedProjectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    sortBy: SharedResourceSortByTypeType = ...,  # (1)
    sortOrder: SortOrderTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListSharedProjectsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SharedResourceSortByTypeType](./literals.md#sharedresourcesortbytypetype) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListSharedProjectsOutputTypeDef](./type_defs.md#listsharedprojectsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListSharedProjectsInputListSharedProjectsPaginateTypeDef = {  # (1)
    "sortBy": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSharedProjectsInputListSharedProjectsPaginateTypeDef](./type_defs.md#listsharedprojectsinputlistsharedprojectspaginatetypedef) 
## ListSharedReportGroupsPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_shared_report_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedReportGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListSharedReportGroupsPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: ListSharedReportGroupsPaginator = client.get_paginator("list_shared_report_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListSharedReportGroupsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [ListSharedReportGroupsPaginator](./paginators.md#listsharedreportgroupspaginator)
3. item: [:material-code-braces: ListSharedReportGroupsOutputTypeDef](./type_defs.md#listsharedreportgroupsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSharedReportGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    sortOrder: SortOrderTypeType = ...,  # (1)
    sortBy: SharedResourceSortByTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListSharedReportGroupsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-brackets: SharedResourceSortByTypeType](./literals.md#sharedresourcesortbytypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListSharedReportGroupsOutputTypeDef](./type_defs.md#listsharedreportgroupsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef = {  # (1)
    "sortOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef](./type_defs.md#listsharedreportgroupsinputlistsharedreportgroupspaginatetypedef) 
