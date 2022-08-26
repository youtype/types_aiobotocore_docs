# Paginators

> [Index](../README.md) > [MainframeModernization](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MainframeModernization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
    type annotations stubs module [types-aiobotocore-m2](https://pypi.org/project/types-aiobotocore-m2/).

## ListApplicationVersionsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_application_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplicationVersions)

```python title="Usage example"
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
3. item: [:material-code-braces: ListApplicationVersionsResponseTypeDef](./type_defs.md#listapplicationversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApplicationVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationVersionsResponseTypeDef](./type_defs.md#listapplicationversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef](./type_defs.md#listapplicationversionsrequestlistapplicationversionspaginatetypedef) 
## ListApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplications)

```python title="Usage example"
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
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    environmentId: str = ...,
    names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApplicationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListApplicationsRequestListApplicationsPaginateTypeDef = {  # (1)
    "environmentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestListApplicationsPaginateTypeDef](./type_defs.md#listapplicationsrequestlistapplicationspaginatetypedef) 
## ListBatchJobDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_batch_job_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobDefinitions)

```python title="Usage example"
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
3. item: [:material-code-braces: ListBatchJobDefinitionsResponseTypeDef](./type_defs.md#listbatchjobdefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBatchJobDefinitionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    applicationId: str,
    prefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBatchJobDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBatchJobDefinitionsResponseTypeDef](./type_defs.md#listbatchjobdefinitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef](./type_defs.md#listbatchjobdefinitionsrequestlistbatchjobdefinitionspaginatetypedef) 
## ListBatchJobExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_batch_job_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobExecutions)

```python title="Usage example"
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
3. item: [:material-code-braces: ListBatchJobExecutionsResponseTypeDef](./type_defs.md#listbatchjobexecutionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBatchJobExecutionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    applicationId: str,
    executionIds: Sequence[str] = ...,
    jobName: str = ...,
    startedAfter: Union[datetime, str] = ...,
    startedBefore: Union[datetime, str] = ...,
    status: BatchJobExecutionStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListBatchJobExecutionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: BatchJobExecutionStatusType](./literals.md#batchjobexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListBatchJobExecutionsResponseTypeDef](./type_defs.md#listbatchjobexecutionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef](./type_defs.md#listbatchjobexecutionsrequestlistbatchjobexecutionspaginatetypedef) 
## ListDataSetImportHistoryPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_data_set_import_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSetImportHistory)

```python title="Usage example"
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
3. item: [:material-code-braces: ListDataSetImportHistoryResponseTypeDef](./type_defs.md#listdatasetimporthistoryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataSetImportHistoryPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDataSetImportHistoryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataSetImportHistoryResponseTypeDef](./type_defs.md#listdatasetimporthistoryresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef](./type_defs.md#listdatasetimporthistoryrequestlistdatasetimporthistorypaginatetypedef) 
## ListDataSetsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_data_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSets)

```python title="Usage example"
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
3. item: [:material-code-braces: ListDataSetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    applicationId: str,
    prefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDataSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataSetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDataSetsRequestListDataSetsPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSetsRequestListDataSetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef) 
## ListDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDeployments)

```python title="Usage example"
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
3. item: [:material-code-braces: ListDeploymentsResponseTypeDef](./type_defs.md#listdeploymentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDeploymentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    applicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDeploymentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeploymentsResponseTypeDef](./type_defs.md#listdeploymentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeploymentsRequestListDeploymentsPaginateTypeDef = {  # (1)
    "applicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsRequestListDeploymentsPaginateTypeDef](./type_defs.md#listdeploymentsrequestlistdeploymentspaginatetypedef) 
## ListEngineVersionsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_engine_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEngineVersions)

```python title="Usage example"
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
3. item: [:material-code-braces: ListEngineVersionsResponseTypeDef](./type_defs.md#listengineversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEngineVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    engineType: EngineTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListEngineVersionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEngineVersionsResponseTypeDef](./type_defs.md#listengineversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = {  # (1)
    "engineType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEngineVersionsRequestListEngineVersionsPaginateTypeDef](./type_defs.md#listengineversionsrequestlistengineversionspaginatetypedef) 
## ListEnvironmentsPaginator

Type annotations and code completion for `#!python session.create_client("m2").get_paginator("list_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEnvironments)

```python title="Usage example"
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
3. item: [:material-code-braces: ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEnvironmentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    engineType: EngineTypeType = ...,  # (1)
    names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListEnvironmentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = {  # (1)
    "engineType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsRequestListEnvironmentsPaginateTypeDef](./type_defs.md#listenvironmentsrequestlistenvironmentspaginatetypedef) 
