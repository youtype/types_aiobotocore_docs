# Paginators

> [Index](../README.md) > [MainframeModernizationApplicationTesting](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MainframeModernizationApplicationTesting](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest.html#mainframemodernizationapplicationtesting)
    type annotations stubs module [types-aiobotocore-apptest](https://pypi.org/project/types-aiobotocore-apptest/).

## ListTestCasesPaginator

Type annotations and code completion for `#!python session.create_client("apptest").get_paginator("list_test_cases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/paginator/ListTestCases.html#MainframeModernizationApplicationTesting.Paginator.ListTestCases)

```python
# ListTestCasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apptest.paginator import ListTestCasesPaginator

session = get_session()
async with session.create_client("apptest") as client:  # (1)
    paginator: ListTestCasesPaginator = client.get_paginator("list_test_cases")  # (2)
    async for item in paginator.paginate(...):
        item: ListTestCasesResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationApplicationTestingClient](./client.md)
2. paginator: [ListTestCasesPaginator](./paginators.md#listtestcasespaginator)
3. item: `AioPageIterator[ListTestCasesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTestCasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    testCaseIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTestCasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTestCasesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTestCasesRequestPaginateTypeDef = {  # (1)
    "testCaseIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTestCasesRequestPaginateTypeDef](./type_defs.md#listtestcasesrequestpaginatetypedef)
## ListTestConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("apptest").get_paginator("list_test_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/paginator/ListTestConfigurations.html#MainframeModernizationApplicationTesting.Paginator.ListTestConfigurations)

```python
# ListTestConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apptest.paginator import ListTestConfigurationsPaginator

session = get_session()
async with session.create_client("apptest") as client:  # (1)
    paginator: ListTestConfigurationsPaginator = client.get_paginator("list_test_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListTestConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationApplicationTestingClient](./client.md)
2. paginator: [ListTestConfigurationsPaginator](./paginators.md#listtestconfigurationspaginator)
3. item: `AioPageIterator[ListTestConfigurationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTestConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    testConfigurationIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTestConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTestConfigurationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTestConfigurationsRequestPaginateTypeDef = {  # (1)
    "testConfigurationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTestConfigurationsRequestPaginateTypeDef](./type_defs.md#listtestconfigurationsrequestpaginatetypedef)
## ListTestRunStepsPaginator

Type annotations and code completion for `#!python session.create_client("apptest").get_paginator("list_test_run_steps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/paginator/ListTestRunSteps.html#MainframeModernizationApplicationTesting.Paginator.ListTestRunSteps)

```python
# ListTestRunStepsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apptest.paginator import ListTestRunStepsPaginator

session = get_session()
async with session.create_client("apptest") as client:  # (1)
    paginator: ListTestRunStepsPaginator = client.get_paginator("list_test_run_steps")  # (2)
    async for item in paginator.paginate(...):
        item: ListTestRunStepsResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationApplicationTestingClient](./client.md)
2. paginator: [ListTestRunStepsPaginator](./paginators.md#listtestrunstepspaginator)
3. item: `AioPageIterator[ListTestRunStepsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTestRunStepsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    testRunId: str,
    testCaseId: str = ...,
    testSuiteId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTestRunStepsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTestRunStepsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTestRunStepsRequestPaginateTypeDef = {  # (1)
    "testRunId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTestRunStepsRequestPaginateTypeDef](./type_defs.md#listtestrunstepsrequestpaginatetypedef)
## ListTestRunTestCasesPaginator

Type annotations and code completion for `#!python session.create_client("apptest").get_paginator("list_test_run_test_cases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/paginator/ListTestRunTestCases.html#MainframeModernizationApplicationTesting.Paginator.ListTestRunTestCases)

```python
# ListTestRunTestCasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apptest.paginator import ListTestRunTestCasesPaginator

session = get_session()
async with session.create_client("apptest") as client:  # (1)
    paginator: ListTestRunTestCasesPaginator = client.get_paginator("list_test_run_test_cases")  # (2)
    async for item in paginator.paginate(...):
        item: ListTestRunTestCasesResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationApplicationTestingClient](./client.md)
2. paginator: [ListTestRunTestCasesPaginator](./paginators.md#listtestruntestcasespaginator)
3. item: `AioPageIterator[ListTestRunTestCasesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTestRunTestCasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    testRunId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTestRunTestCasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTestRunTestCasesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTestRunTestCasesRequestPaginateTypeDef = {  # (1)
    "testRunId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTestRunTestCasesRequestPaginateTypeDef](./type_defs.md#listtestruntestcasesrequestpaginatetypedef)
## ListTestRunsPaginator

Type annotations and code completion for `#!python session.create_client("apptest").get_paginator("list_test_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/paginator/ListTestRuns.html#MainframeModernizationApplicationTesting.Paginator.ListTestRuns)

```python
# ListTestRunsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apptest.paginator import ListTestRunsPaginator

session = get_session()
async with session.create_client("apptest") as client:  # (1)
    paginator: ListTestRunsPaginator = client.get_paginator("list_test_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListTestRunsResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationApplicationTestingClient](./client.md)
2. paginator: [ListTestRunsPaginator](./paginators.md#listtestrunspaginator)
3. item: `AioPageIterator[ListTestRunsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTestRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    testSuiteId: str = ...,
    testRunIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTestRunsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTestRunsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTestRunsRequestPaginateTypeDef = {  # (1)
    "testSuiteId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTestRunsRequestPaginateTypeDef](./type_defs.md#listtestrunsrequestpaginatetypedef)
## ListTestSuitesPaginator

Type annotations and code completion for `#!python session.create_client("apptest").get_paginator("list_test_suites")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/paginator/ListTestSuites.html#MainframeModernizationApplicationTesting.Paginator.ListTestSuites)

```python
# ListTestSuitesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apptest.paginator import ListTestSuitesPaginator

session = get_session()
async with session.create_client("apptest") as client:  # (1)
    paginator: ListTestSuitesPaginator = client.get_paginator("list_test_suites")  # (2)
    async for item in paginator.paginate(...):
        item: ListTestSuitesResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationApplicationTestingClient](./client.md)
2. paginator: [ListTestSuitesPaginator](./paginators.md#listtestsuitespaginator)
3. item: `AioPageIterator[ListTestSuitesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTestSuitesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    testSuiteIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTestSuitesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTestSuitesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTestSuitesRequestPaginateTypeDef = {  # (1)
    "testSuiteIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTestSuitesRequestPaginateTypeDef](./type_defs.md#listtestsuitesrequestpaginatetypedef)
