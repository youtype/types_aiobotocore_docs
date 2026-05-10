# Paginators

> [Index](../README.md) > [DataAutomationforBedrock](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DataAutomationforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation.html#dataautomationforbedrock)
    type annotations stubs module [types-aiobotocore-bedrock-data-automation](https://pypi.org/project/types-aiobotocore-bedrock-data-automation/).

## ListBlueprintsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").get_paginator("list_blueprints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/paginator/ListBlueprints.html#DataAutomationforBedrock.Paginator.ListBlueprints)

```python
# ListBlueprintsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_data_automation.paginator import ListBlueprintsPaginator

session = get_session()
async with session.create_client("bedrock-data-automation") as client:  # (1)
    paginator: ListBlueprintsPaginator = client.get_paginator("list_blueprints")  # (2)
    async for item in paginator.paginate(...):
        item: ListBlueprintsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataAutomationforBedrockClient](./client.md)
2. paginator: [ListBlueprintsPaginator](./paginators.md#listblueprintspaginator)
3. item: `AioPageIterator[ListBlueprintsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBlueprintsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    blueprintArn: str = ...,
    resourceOwner: ResourceOwnerType = ...,  # (1)
    blueprintStageFilter: BlueprintStageFilterType = ...,  # (2)
    projectFilter: DataAutomationProjectFilterTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListBlueprintsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype)
2. See [:material-code-brackets: BlueprintStageFilterType](./literals.md#blueprintstagefiltertype)
3. See [:material-code-braces: DataAutomationProjectFilterTypeDef](./type_defs.md#dataautomationprojectfiltertypedef)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListBlueprintsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBlueprintsRequestPaginateTypeDef = {  # (1)
    "blueprintArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBlueprintsRequestPaginateTypeDef](./type_defs.md#listblueprintsrequestpaginatetypedef)
## ListDataAutomationLibrariesPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").get_paginator("list_data_automation_libraries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/paginator/ListDataAutomationLibraries.html#DataAutomationforBedrock.Paginator.ListDataAutomationLibraries)

```python
# ListDataAutomationLibrariesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_data_automation.paginator import ListDataAutomationLibrariesPaginator

session = get_session()
async with session.create_client("bedrock-data-automation") as client:  # (1)
    paginator: ListDataAutomationLibrariesPaginator = client.get_paginator("list_data_automation_libraries")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataAutomationLibrariesResponseTypeDef
        print(item)  # (3)
```

1. client: [DataAutomationforBedrockClient](./client.md)
2. paginator: [ListDataAutomationLibrariesPaginator](./paginators.md#listdataautomationlibrariespaginator)
3. item: `AioPageIterator[ListDataAutomationLibrariesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataAutomationLibrariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    projectFilter: DataAutomationProjectFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDataAutomationLibrariesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DataAutomationProjectFilterTypeDef](./type_defs.md#dataautomationprojectfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDataAutomationLibrariesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataAutomationLibrariesRequestPaginateTypeDef = {  # (1)
    "projectFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataAutomationLibrariesRequestPaginateTypeDef](./type_defs.md#listdataautomationlibrariesrequestpaginatetypedef)
## ListDataAutomationLibraryEntitiesPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").get_paginator("list_data_automation_library_entities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/paginator/ListDataAutomationLibraryEntities.html#DataAutomationforBedrock.Paginator.ListDataAutomationLibraryEntities)

```python
# ListDataAutomationLibraryEntitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_data_automation.paginator import ListDataAutomationLibraryEntitiesPaginator

session = get_session()
async with session.create_client("bedrock-data-automation") as client:  # (1)
    paginator: ListDataAutomationLibraryEntitiesPaginator = client.get_paginator("list_data_automation_library_entities")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataAutomationLibraryEntitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [DataAutomationforBedrockClient](./client.md)
2. paginator: [ListDataAutomationLibraryEntitiesPaginator](./paginators.md#listdataautomationlibraryentitiespaginator)
3. item: `AioPageIterator[ListDataAutomationLibraryEntitiesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataAutomationLibraryEntitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    libraryArn: str,
    entityType: EntityTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDataAutomationLibraryEntitiesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDataAutomationLibraryEntitiesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataAutomationLibraryEntitiesRequestPaginateTypeDef = {  # (1)
    "libraryArn": ...,
    "entityType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataAutomationLibraryEntitiesRequestPaginateTypeDef](./type_defs.md#listdataautomationlibraryentitiesrequestpaginatetypedef)
## ListDataAutomationLibraryIngestionJobsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").get_paginator("list_data_automation_library_ingestion_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/paginator/ListDataAutomationLibraryIngestionJobs.html#DataAutomationforBedrock.Paginator.ListDataAutomationLibraryIngestionJobs)

```python
# ListDataAutomationLibraryIngestionJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_data_automation.paginator import ListDataAutomationLibraryIngestionJobsPaginator

session = get_session()
async with session.create_client("bedrock-data-automation") as client:  # (1)
    paginator: ListDataAutomationLibraryIngestionJobsPaginator = client.get_paginator("list_data_automation_library_ingestion_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataAutomationLibraryIngestionJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataAutomationforBedrockClient](./client.md)
2. paginator: [ListDataAutomationLibraryIngestionJobsPaginator](./paginators.md#listdataautomationlibraryingestionjobspaginator)
3. item: `AioPageIterator[ListDataAutomationLibraryIngestionJobsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataAutomationLibraryIngestionJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    libraryArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDataAutomationLibraryIngestionJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataAutomationLibraryIngestionJobsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataAutomationLibraryIngestionJobsRequestPaginateTypeDef = {  # (1)
    "libraryArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataAutomationLibraryIngestionJobsRequestPaginateTypeDef](./type_defs.md#listdataautomationlibraryingestionjobsrequestpaginatetypedef)
## ListDataAutomationProjectsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").get_paginator("list_data_automation_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/paginator/ListDataAutomationProjects.html#DataAutomationforBedrock.Paginator.ListDataAutomationProjects)

```python
# ListDataAutomationProjectsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_data_automation.paginator import ListDataAutomationProjectsPaginator

session = get_session()
async with session.create_client("bedrock-data-automation") as client:  # (1)
    paginator: ListDataAutomationProjectsPaginator = client.get_paginator("list_data_automation_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataAutomationProjectsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataAutomationforBedrockClient](./client.md)
2. paginator: [ListDataAutomationProjectsPaginator](./paginators.md#listdataautomationprojectspaginator)
3. item: `AioPageIterator[ListDataAutomationProjectsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataAutomationProjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    projectStageFilter: DataAutomationProjectStageFilterType = ...,  # (1)
    blueprintFilter: BlueprintFilterTypeDef = ...,  # (2)
    resourceOwner: ResourceOwnerType = ...,  # (3)
    libraryFilter: DataAutomationLibraryFilterTypeDef = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> aiobotocore.paginate.AioPageIterator[ListDataAutomationProjectsResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: DataAutomationProjectStageFilterType](./literals.md#dataautomationprojectstagefiltertype)
2. See [:material-code-braces: BlueprintFilterTypeDef](./type_defs.md#blueprintfiltertypedef)
3. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype)
4. See [:material-code-braces: DataAutomationLibraryFilterTypeDef](./type_defs.md#dataautomationlibraryfiltertypedef)
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
6. See `AioPageIterator[ListDataAutomationProjectsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataAutomationProjectsRequestPaginateTypeDef = {  # (1)
    "projectStageFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataAutomationProjectsRequestPaginateTypeDef](./type_defs.md#listdataautomationprojectsrequestpaginatetypedef)
