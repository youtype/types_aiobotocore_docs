# Paginators

> [Index](../README.md) > [MainframeModernization](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MainframeModernization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#mainframemodernization)
    type annotations stubs module [types-aiobotocore-m2](https://pypi.org/project/types-aiobotocore-m2/).

## ListApplicationVersionsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_application_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2/paginator/ListApplicationVersions.html#MainframeModernization.Paginator.ListApplicationVersions)

```python
# ListApplicationVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_m2.paginator import ListApplicationVersionsPaginator

session = get_session()
async with session.create_client("m2") as client:  # (1)
    paginator: ListApplicationVersionsPaginator = client.get_paginator("list_application_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationClient](./client.md)
2. paginator: [ListApplicationVersionsPaginator](./paginators.md#listapplicationversionspaginator)
3. item: `AioPageIterator[ListApplicationVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListApplicationVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListApplicationVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListApplicationVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationVersionsRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationVersionsRequestPaginateTypeDef](./type_defs.md#listapplicationversionsrequestpaginatetypedef)
## ListApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2/paginator/ListApplications.html#MainframeModernization.Paginator.ListApplications)

```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_m2.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("m2") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: `AioPageIterator[ListApplicationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    environmentId: str = ...,
    names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListApplicationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListApplicationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationsRequestPaginateTypeDef = {  # (1)
    "environmentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestPaginateTypeDef](./type_defs.md#listapplicationsrequestpaginatetypedef)
## ListBatchJobDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_batch_job_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2/paginator/ListBatchJobDefinitions.html#MainframeModernization.Paginator.ListBatchJobDefinitions)

```python
# ListBatchJobDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_m2.paginator import ListBatchJobDefinitionsPaginator

session = get_session()
async with session.create_client("m2") as client:  # (1)
    paginator: ListBatchJobDefinitionsPaginator = client.get_paginator("list_batch_job_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListBatchJobDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationClient](./client.md)
2. paginator: [ListBatchJobDefinitionsPaginator](./paginators.md#listbatchjobdefinitionspaginator)
3. item: `AioPageIterator[ListBatchJobDefinitionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBatchJobDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    prefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBatchJobDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBatchJobDefinitionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBatchJobDefinitionsRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBatchJobDefinitionsRequestPaginateTypeDef](./type_defs.md#listbatchjobdefinitionsrequestpaginatetypedef)
## ListBatchJobExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_batch_job_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2/paginator/ListBatchJobExecutions.html#MainframeModernization.Paginator.ListBatchJobExecutions)

```python
# ListBatchJobExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_m2.paginator import ListBatchJobExecutionsPaginator

session = get_session()
async with session.create_client("m2") as client:  # (1)
    paginator: ListBatchJobExecutionsPaginator = client.get_paginator("list_batch_job_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListBatchJobExecutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationClient](./client.md)
2. paginator: [ListBatchJobExecutionsPaginator](./paginators.md#listbatchjobexecutionspaginator)
3. item: `AioPageIterator[ListBatchJobExecutionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBatchJobExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    executionIds: Sequence[str] = ...,
    jobName: str = ...,
    startedAfter: TimestampTypeDef = ...,
    startedBefore: TimestampTypeDef = ...,
    status: BatchJobExecutionStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListBatchJobExecutionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: BatchJobExecutionStatusType](./literals.md#batchjobexecutionstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListBatchJobExecutionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBatchJobExecutionsRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBatchJobExecutionsRequestPaginateTypeDef](./type_defs.md#listbatchjobexecutionsrequestpaginatetypedef)
## ListDataSetExportHistoryPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_data_set_export_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2/paginator/ListDataSetExportHistory.html#MainframeModernization.Paginator.ListDataSetExportHistory)

```python
# ListDataSetExportHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_m2.paginator import ListDataSetExportHistoryPaginator

session = get_session()
async with session.create_client("m2") as client:  # (1)
    paginator: ListDataSetExportHistoryPaginator = client.get_paginator("list_data_set_export_history")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSetExportHistoryResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationClient](./client.md)
2. paginator: [ListDataSetExportHistoryPaginator](./paginators.md#listdatasetexporthistorypaginator)
3. item: `AioPageIterator[ListDataSetExportHistoryResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataSetExportHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDataSetExportHistoryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataSetExportHistoryResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSetExportHistoryRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSetExportHistoryRequestPaginateTypeDef](./type_defs.md#listdatasetexporthistoryrequestpaginatetypedef)
## ListDataSetImportHistoryPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_data_set_import_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2/paginator/ListDataSetImportHistory.html#MainframeModernization.Paginator.ListDataSetImportHistory)

```python
# ListDataSetImportHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_m2.paginator import ListDataSetImportHistoryPaginator

session = get_session()
async with session.create_client("m2") as client:  # (1)
    paginator: ListDataSetImportHistoryPaginator = client.get_paginator("list_data_set_import_history")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSetImportHistoryResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationClient](./client.md)
2. paginator: [ListDataSetImportHistoryPaginator](./paginators.md#listdatasetimporthistorypaginator)
3. item: `AioPageIterator[ListDataSetImportHistoryResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataSetImportHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDataSetImportHistoryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataSetImportHistoryResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSetImportHistoryRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSetImportHistoryRequestPaginateTypeDef](./type_defs.md#listdatasetimporthistoryrequestpaginatetypedef)
## ListDataSetsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_data_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2/paginator/ListDataSets.html#MainframeModernization.Paginator.ListDataSets)

```python
# ListDataSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_m2.paginator import ListDataSetsPaginator

session = get_session()
async with session.create_client("m2") as client:  # (1)
    paginator: ListDataSetsPaginator = client.get_paginator("list_data_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationClient](./client.md)
2. paginator: [ListDataSetsPaginator](./paginators.md#listdatasetspaginator)
3. item: `AioPageIterator[ListDataSetsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    nameFilter: str = ...,
    prefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDataSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataSetsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSetsRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSetsRequestPaginateTypeDef](./type_defs.md#listdatasetsrequestpaginatetypedef)
## ListDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2/paginator/ListDeployments.html#MainframeModernization.Paginator.ListDeployments)

```python
# ListDeploymentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_m2.paginator import ListDeploymentsPaginator

session = get_session()
async with session.create_client("m2") as client:  # (1)
    paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentsResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationClient](./client.md)
2. paginator: [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
3. item: `AioPageIterator[ListDeploymentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDeploymentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDeploymentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDeploymentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDeploymentsRequestPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsRequestPaginateTypeDef](./type_defs.md#listdeploymentsrequestpaginatetypedef)
## ListEngineVersionsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_engine_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2/paginator/ListEngineVersions.html#MainframeModernization.Paginator.ListEngineVersions)

```python
# ListEngineVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_m2.paginator import ListEngineVersionsPaginator

session = get_session()
async with session.create_client("m2") as client:  # (1)
    paginator: ListEngineVersionsPaginator = client.get_paginator("list_engine_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListEngineVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationClient](./client.md)
2. paginator: [ListEngineVersionsPaginator](./paginators.md#listengineversionspaginator)
3. item: `AioPageIterator[ListEngineVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEngineVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    engineType: EngineTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListEngineVersionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListEngineVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEngineVersionsRequestPaginateTypeDef = {  # (1)
    "engineType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEngineVersionsRequestPaginateTypeDef](./type_defs.md#listengineversionsrequestpaginatetypedef)
## ListEnvironmentsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2/paginator/ListEnvironments.html#MainframeModernization.Paginator.ListEnvironments)

```python
# ListEnvironmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_m2.paginator import ListEnvironmentsPaginator

session = get_session()
async with session.create_client("m2") as client:  # (1)
    paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [MainframeModernizationClient](./client.md)
2. paginator: [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
3. item: `AioPageIterator[ListEnvironmentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEnvironmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    engineType: EngineTypeType = ...,  # (1)
    names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListEnvironmentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListEnvironmentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEnvironmentsRequestPaginateTypeDef = {  # (1)
    "engineType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsRequestPaginateTypeDef](./type_defs.md#listenvironmentsrequestpaginatetypedef)
