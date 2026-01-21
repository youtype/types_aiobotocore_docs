# Paginators

> [Index](../README.md) > [CodeBuild](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeBuild](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#codebuild)
    type annotations stubs module [types-aiobotocore-codebuild](https://pypi.org/project/types-aiobotocore-codebuild/).

## DescribeCodeCoveragesPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("describe_code_coverages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/DescribeCodeCoverages.html#CodeBuild.Paginator.DescribeCodeCoverages)

```python
# DescribeCodeCoveragesPaginator usage example

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
3. item: `AioPageIterator[DescribeCodeCoveragesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeCodeCoveragesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    reportArn: str,
    sortOrder: SortOrderTypeType = ...,  # (1)
    sortBy: ReportCodeCoverageSortByTypeType = ...,  # (2)
    minLineCoveragePercentage: float = ...,
    maxLineCoveragePercentage: float = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[DescribeCodeCoveragesOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
2. See [:material-code-brackets: ReportCodeCoverageSortByTypeType](./literals.md#reportcodecoveragesortbytypetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[DescribeCodeCoveragesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCodeCoveragesInputPaginateTypeDef = {  # (1)
    "reportArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCodeCoveragesInputPaginateTypeDef](./type_defs.md#describecodecoveragesinputpaginatetypedef)
## DescribeTestCasesPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("describe_test_cases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/DescribeTestCases.html#CodeBuild.Paginator.DescribeTestCases)

```python
# DescribeTestCasesPaginator usage example

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
3. item: `AioPageIterator[DescribeTestCasesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTestCasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    reportArn: str,
    filter: TestCaseFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTestCasesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TestCaseFilterTypeDef](./type_defs.md#testcasefiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTestCasesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTestCasesInputPaginateTypeDef = {  # (1)
    "reportArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTestCasesInputPaginateTypeDef](./type_defs.md#describetestcasesinputpaginatetypedef)
## ListBuildBatchesForProjectPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_build_batches_for_project")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/ListBuildBatchesForProject.html#CodeBuild.Paginator.ListBuildBatchesForProject)

```python
# ListBuildBatchesForProjectPaginator usage example

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
3. item: `AioPageIterator[ListBuildBatchesForProjectOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBuildBatchesForProjectPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    projectName: str = ...,
    filter: BuildBatchFilterTypeDef = ...,  # (1)
    sortOrder: SortOrderTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListBuildBatchesForProjectOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: BuildBatchFilterTypeDef](./type_defs.md#buildbatchfiltertypedef)
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListBuildBatchesForProjectOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBuildBatchesForProjectInputPaginateTypeDef = {  # (1)
    "projectName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBuildBatchesForProjectInputPaginateTypeDef](./type_defs.md#listbuildbatchesforprojectinputpaginatetypedef)
## ListBuildBatchesPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_build_batches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/ListBuildBatches.html#CodeBuild.Paginator.ListBuildBatches)

```python
# ListBuildBatchesPaginator usage example

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
3. item: `AioPageIterator[ListBuildBatchesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBuildBatchesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filter: BuildBatchFilterTypeDef = ...,  # (1)
    sortOrder: SortOrderTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListBuildBatchesOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: BuildBatchFilterTypeDef](./type_defs.md#buildbatchfiltertypedef)
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListBuildBatchesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBuildBatchesInputPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBuildBatchesInputPaginateTypeDef](./type_defs.md#listbuildbatchesinputpaginatetypedef)
## ListBuildsForProjectPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_builds_for_project")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/ListBuildsForProject.html#CodeBuild.Paginator.ListBuildsForProject)

```python
# ListBuildsForProjectPaginator usage example

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
3. item: `AioPageIterator[ListBuildsForProjectOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBuildsForProjectPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    projectName: str,
    sortOrder: SortOrderTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListBuildsForProjectOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListBuildsForProjectOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBuildsForProjectInputPaginateTypeDef = {  # (1)
    "projectName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBuildsForProjectInputPaginateTypeDef](./type_defs.md#listbuildsforprojectinputpaginatetypedef)
## ListBuildsPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_builds")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/ListBuilds.html#CodeBuild.Paginator.ListBuilds)

```python
# ListBuildsPaginator usage example

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
3. item: `AioPageIterator[ListBuildsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBuildsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sortOrder: SortOrderTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListBuildsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListBuildsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBuildsInputPaginateTypeDef = {  # (1)
    "sortOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBuildsInputPaginateTypeDef](./type_defs.md#listbuildsinputpaginatetypedef)
## ListCommandExecutionsForSandboxPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_command_executions_for_sandbox")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/ListCommandExecutionsForSandbox.html#CodeBuild.Paginator.ListCommandExecutionsForSandbox)

```python
# ListCommandExecutionsForSandboxPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListCommandExecutionsForSandboxPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: ListCommandExecutionsForSandboxPaginator = client.get_paginator("list_command_executions_for_sandbox")  # (2)
    async for item in paginator.paginate(...):
        item: ListCommandExecutionsForSandboxOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [ListCommandExecutionsForSandboxPaginator](./paginators.md#listcommandexecutionsforsandboxpaginator)
3. item: `AioPageIterator[ListCommandExecutionsForSandboxOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCommandExecutionsForSandboxPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sandboxId: str,
    sortOrder: SortOrderTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListCommandExecutionsForSandboxOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListCommandExecutionsForSandboxOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCommandExecutionsForSandboxInputPaginateTypeDef = {  # (1)
    "sandboxId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCommandExecutionsForSandboxInputPaginateTypeDef](./type_defs.md#listcommandexecutionsforsandboxinputpaginatetypedef)
## ListProjectsPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/ListProjects.html#CodeBuild.Paginator.ListProjects)

```python
# ListProjectsPaginator usage example

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
3. item: `AioPageIterator[ListProjectsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sortBy: ProjectSortByTypeType = ...,  # (1)
    sortOrder: SortOrderTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListProjectsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ProjectSortByTypeType](./literals.md#projectsortbytypetype)
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListProjectsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProjectsInputPaginateTypeDef = {  # (1)
    "sortBy": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsInputPaginateTypeDef](./type_defs.md#listprojectsinputpaginatetypedef)
## ListReportGroupsPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_report_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/ListReportGroups.html#CodeBuild.Paginator.ListReportGroups)

```python
# ListReportGroupsPaginator usage example

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
3. item: `AioPageIterator[ListReportGroupsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListReportGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sortOrder: SortOrderTypeType = ...,  # (1)
    sortBy: ReportGroupSortByTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListReportGroupsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
2. See [:material-code-brackets: ReportGroupSortByTypeType](./literals.md#reportgroupsortbytypetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListReportGroupsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListReportGroupsInputPaginateTypeDef = {  # (1)
    "sortOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReportGroupsInputPaginateTypeDef](./type_defs.md#listreportgroupsinputpaginatetypedef)
## ListReportsForReportGroupPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_reports_for_report_group")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/ListReportsForReportGroup.html#CodeBuild.Paginator.ListReportsForReportGroup)

```python
# ListReportsForReportGroupPaginator usage example

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
3. item: `AioPageIterator[ListReportsForReportGroupOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListReportsForReportGroupPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    reportGroupArn: str,
    sortOrder: SortOrderTypeType = ...,  # (1)
    filter: ReportFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListReportsForReportGroupOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
2. See [:material-code-braces: ReportFilterTypeDef](./type_defs.md#reportfiltertypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListReportsForReportGroupOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListReportsForReportGroupInputPaginateTypeDef = {  # (1)
    "reportGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReportsForReportGroupInputPaginateTypeDef](./type_defs.md#listreportsforreportgroupinputpaginatetypedef)
## ListReportsPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_reports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/ListReports.html#CodeBuild.Paginator.ListReports)

```python
# ListReportsPaginator usage example

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
3. item: `AioPageIterator[ListReportsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListReportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sortOrder: SortOrderTypeType = ...,  # (1)
    filter: ReportFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListReportsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
2. See [:material-code-braces: ReportFilterTypeDef](./type_defs.md#reportfiltertypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListReportsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListReportsInputPaginateTypeDef = {  # (1)
    "sortOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReportsInputPaginateTypeDef](./type_defs.md#listreportsinputpaginatetypedef)
## ListSandboxesForProjectPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_sandboxes_for_project")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/ListSandboxesForProject.html#CodeBuild.Paginator.ListSandboxesForProject)

```python
# ListSandboxesForProjectPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListSandboxesForProjectPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: ListSandboxesForProjectPaginator = client.get_paginator("list_sandboxes_for_project")  # (2)
    async for item in paginator.paginate(...):
        item: ListSandboxesForProjectOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [ListSandboxesForProjectPaginator](./paginators.md#listsandboxesforprojectpaginator)
3. item: `AioPageIterator[ListSandboxesForProjectOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSandboxesForProjectPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    projectName: str,
    sortOrder: SortOrderTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListSandboxesForProjectOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListSandboxesForProjectOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSandboxesForProjectInputPaginateTypeDef = {  # (1)
    "projectName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSandboxesForProjectInputPaginateTypeDef](./type_defs.md#listsandboxesforprojectinputpaginatetypedef)
## ListSandboxesPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_sandboxes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/ListSandboxes.html#CodeBuild.Paginator.ListSandboxes)

```python
# ListSandboxesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codebuild.paginator import ListSandboxesPaginator

session = get_session()
async with session.create_client("codebuild") as client:  # (1)
    paginator: ListSandboxesPaginator = client.get_paginator("list_sandboxes")  # (2)
    async for item in paginator.paginate(...):
        item: ListSandboxesOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [ListSandboxesPaginator](./paginators.md#listsandboxespaginator)
3. item: `AioPageIterator[ListSandboxesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSandboxesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sortOrder: SortOrderTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListSandboxesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListSandboxesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSandboxesInputPaginateTypeDef = {  # (1)
    "sortOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSandboxesInputPaginateTypeDef](./type_defs.md#listsandboxesinputpaginatetypedef)
## ListSharedProjectsPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_shared_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/ListSharedProjects.html#CodeBuild.Paginator.ListSharedProjects)

```python
# ListSharedProjectsPaginator usage example

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
3. item: `AioPageIterator[ListSharedProjectsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSharedProjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sortBy: SharedResourceSortByTypeType = ...,  # (1)
    sortOrder: SortOrderTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListSharedProjectsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SharedResourceSortByTypeType](./literals.md#sharedresourcesortbytypetype)
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListSharedProjectsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSharedProjectsInputPaginateTypeDef = {  # (1)
    "sortBy": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSharedProjectsInputPaginateTypeDef](./type_defs.md#listsharedprojectsinputpaginatetypedef)
## ListSharedReportGroupsPaginator

Type annotations and code completion for `#!python session.create_client("codebuild").get_paginator("list_shared_report_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild/paginator/ListSharedReportGroups.html#CodeBuild.Paginator.ListSharedReportGroups)

```python
# ListSharedReportGroupsPaginator usage example

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
3. item: `AioPageIterator[ListSharedReportGroupsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSharedReportGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sortOrder: SortOrderTypeType = ...,  # (1)
    sortBy: SharedResourceSortByTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListSharedReportGroupsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype)
2. See [:material-code-brackets: SharedResourceSortByTypeType](./literals.md#sharedresourcesortbytypetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListSharedReportGroupsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSharedReportGroupsInputPaginateTypeDef = {  # (1)
    "sortOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSharedReportGroupsInputPaginateTypeDef](./type_defs.md#listsharedreportgroupsinputpaginatetypedef)
