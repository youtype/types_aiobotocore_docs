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
3. item: [:material-code-braces: ListBlueprintsResponseTypeDef](./type_defs.md#listblueprintsresponsetypedef) 


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
) -> AioPageIterator[ListBlueprintsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-brackets: BlueprintStageFilterType](./literals.md#blueprintstagefiltertype) 
3. See [:material-code-braces: DataAutomationProjectFilterTypeDef](./type_defs.md#dataautomationprojectfiltertypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListBlueprintsResponseTypeDef](./type_defs.md#listblueprintsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBlueprintsRequestPaginateTypeDef = {  # (1)
    "blueprintArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBlueprintsRequestPaginateTypeDef](./type_defs.md#listblueprintsrequestpaginatetypedef) 
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
3. item: [:material-code-braces: ListDataAutomationProjectsResponseTypeDef](./type_defs.md#listdataautomationprojectsresponsetypedef) 


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
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListDataAutomationProjectsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: DataAutomationProjectStageFilterType](./literals.md#dataautomationprojectstagefiltertype) 
2. See [:material-code-braces: BlueprintFilterTypeDef](./type_defs.md#blueprintfiltertypedef) 
3. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListDataAutomationProjectsResponseTypeDef](./type_defs.md#listdataautomationprojectsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataAutomationProjectsRequestPaginateTypeDef = {  # (1)
    "projectStageFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataAutomationProjectsRequestPaginateTypeDef](./type_defs.md#listdataautomationprojectsrequestpaginatetypedef) 
