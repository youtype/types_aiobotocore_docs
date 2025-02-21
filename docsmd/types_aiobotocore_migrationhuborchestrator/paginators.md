# Paginators

> [Index](../README.md) > [MigrationHubOrchestrator](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MigrationHubOrchestrator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#migrationhuborchestrator)
    type annotations stubs module [types-aiobotocore-migrationhuborchestrator](https://pypi.org/project/types-aiobotocore-migrationhuborchestrator/).

## ListPluginsPaginator

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_paginator("list_plugins")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator/paginator/ListPlugins.html#MigrationHubOrchestrator.Paginator.ListPlugins)

```python
# ListPluginsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhuborchestrator.paginator import ListPluginsPaginator

session = get_session()
async with session.create_client("migrationhuborchestrator") as client:  # (1)
    paginator: ListPluginsPaginator = client.get_paginator("list_plugins")  # (2)
    async for item in paginator.paginate(...):
        item: ListPluginsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubOrchestratorClient](./client.md)
2. paginator: [ListPluginsPaginator](./paginators.md#listpluginspaginator)
3. item: [:material-code-braces: ListPluginsResponseTypeDef](./type_defs.md#listpluginsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPluginsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPluginsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPluginsResponseTypeDef](./type_defs.md#listpluginsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPluginsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPluginsRequestPaginateTypeDef](./type_defs.md#listpluginsrequestpaginatetypedef) 
## ListTemplateStepGroupsPaginator

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_paginator("list_template_step_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator/paginator/ListTemplateStepGroups.html#MigrationHubOrchestrator.Paginator.ListTemplateStepGroups)

```python
# ListTemplateStepGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhuborchestrator.paginator import ListTemplateStepGroupsPaginator

session = get_session()
async with session.create_client("migrationhuborchestrator") as client:  # (1)
    paginator: ListTemplateStepGroupsPaginator = client.get_paginator("list_template_step_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListTemplateStepGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubOrchestratorClient](./client.md)
2. paginator: [ListTemplateStepGroupsPaginator](./paginators.md#listtemplatestepgroupspaginator)
3. item: [:material-code-braces: ListTemplateStepGroupsResponseTypeDef](./type_defs.md#listtemplatestepgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTemplateStepGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    templateId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTemplateStepGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTemplateStepGroupsResponseTypeDef](./type_defs.md#listtemplatestepgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTemplateStepGroupsRequestPaginateTypeDef = {  # (1)
    "templateId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTemplateStepGroupsRequestPaginateTypeDef](./type_defs.md#listtemplatestepgroupsrequestpaginatetypedef) 
## ListTemplateStepsPaginator

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_paginator("list_template_steps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator/paginator/ListTemplateSteps.html#MigrationHubOrchestrator.Paginator.ListTemplateSteps)

```python
# ListTemplateStepsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhuborchestrator.paginator import ListTemplateStepsPaginator

session = get_session()
async with session.create_client("migrationhuborchestrator") as client:  # (1)
    paginator: ListTemplateStepsPaginator = client.get_paginator("list_template_steps")  # (2)
    async for item in paginator.paginate(...):
        item: ListTemplateStepsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubOrchestratorClient](./client.md)
2. paginator: [ListTemplateStepsPaginator](./paginators.md#listtemplatestepspaginator)
3. item: [:material-code-braces: ListTemplateStepsResponseTypeDef](./type_defs.md#listtemplatestepsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTemplateStepsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    templateId: str,
    stepGroupId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTemplateStepsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTemplateStepsResponseTypeDef](./type_defs.md#listtemplatestepsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTemplateStepsRequestPaginateTypeDef = {  # (1)
    "templateId": ...,
    "stepGroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTemplateStepsRequestPaginateTypeDef](./type_defs.md#listtemplatestepsrequestpaginatetypedef) 
## ListTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_paginator("list_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator/paginator/ListTemplates.html#MigrationHubOrchestrator.Paginator.ListTemplates)

```python
# ListTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhuborchestrator.paginator import ListTemplatesPaginator

session = get_session()
async with session.create_client("migrationhuborchestrator") as client:  # (1)
    paginator: ListTemplatesPaginator = client.get_paginator("list_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListMigrationWorkflowTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubOrchestratorClient](./client.md)
2. paginator: [ListTemplatesPaginator](./paginators.md#listtemplatespaginator)
3. item: [:material-code-braces: ListMigrationWorkflowTemplatesResponseTypeDef](./type_defs.md#listmigrationworkflowtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    name: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMigrationWorkflowTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMigrationWorkflowTemplatesResponseTypeDef](./type_defs.md#listmigrationworkflowtemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMigrationWorkflowTemplatesRequestPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMigrationWorkflowTemplatesRequestPaginateTypeDef](./type_defs.md#listmigrationworkflowtemplatesrequestpaginatetypedef) 
## ListWorkflowStepGroupsPaginator

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_paginator("list_workflow_step_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator/paginator/ListWorkflowStepGroups.html#MigrationHubOrchestrator.Paginator.ListWorkflowStepGroups)

```python
# ListWorkflowStepGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhuborchestrator.paginator import ListWorkflowStepGroupsPaginator

session = get_session()
async with session.create_client("migrationhuborchestrator") as client:  # (1)
    paginator: ListWorkflowStepGroupsPaginator = client.get_paginator("list_workflow_step_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkflowStepGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubOrchestratorClient](./client.md)
2. paginator: [ListWorkflowStepGroupsPaginator](./paginators.md#listworkflowstepgroupspaginator)
3. item: [:material-code-braces: ListWorkflowStepGroupsResponseTypeDef](./type_defs.md#listworkflowstepgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkflowStepGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workflowId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWorkflowStepGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkflowStepGroupsResponseTypeDef](./type_defs.md#listworkflowstepgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowStepGroupsRequestPaginateTypeDef = {  # (1)
    "workflowId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowStepGroupsRequestPaginateTypeDef](./type_defs.md#listworkflowstepgroupsrequestpaginatetypedef) 
## ListWorkflowStepsPaginator

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_paginator("list_workflow_steps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator/paginator/ListWorkflowSteps.html#MigrationHubOrchestrator.Paginator.ListWorkflowSteps)

```python
# ListWorkflowStepsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhuborchestrator.paginator import ListWorkflowStepsPaginator

session = get_session()
async with session.create_client("migrationhuborchestrator") as client:  # (1)
    paginator: ListWorkflowStepsPaginator = client.get_paginator("list_workflow_steps")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkflowStepsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubOrchestratorClient](./client.md)
2. paginator: [ListWorkflowStepsPaginator](./paginators.md#listworkflowstepspaginator)
3. item: [:material-code-braces: ListWorkflowStepsResponseTypeDef](./type_defs.md#listworkflowstepsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkflowStepsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workflowId: str,
    stepGroupId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWorkflowStepsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkflowStepsResponseTypeDef](./type_defs.md#listworkflowstepsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowStepsRequestPaginateTypeDef = {  # (1)
    "workflowId": ...,
    "stepGroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowStepsRequestPaginateTypeDef](./type_defs.md#listworkflowstepsrequestpaginatetypedef) 
## ListWorkflowsPaginator

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_paginator("list_workflows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator/paginator/ListWorkflows.html#MigrationHubOrchestrator.Paginator.ListWorkflows)

```python
# ListWorkflowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhuborchestrator.paginator import ListWorkflowsPaginator

session = get_session()
async with session.create_client("migrationhuborchestrator") as client:  # (1)
    paginator: ListWorkflowsPaginator = client.get_paginator("list_workflows")  # (2)
    async for item in paginator.paginate(...):
        item: ListMigrationWorkflowsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubOrchestratorClient](./client.md)
2. paginator: [ListWorkflowsPaginator](./paginators.md#listworkflowspaginator)
3. item: [:material-code-braces: ListMigrationWorkflowsResponseTypeDef](./type_defs.md#listmigrationworkflowsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkflowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    templateId: str = ...,
    adsApplicationConfigurationName: str = ...,
    status: MigrationWorkflowStatusEnumType = ...,  # (1)
    name: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListMigrationWorkflowsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: MigrationWorkflowStatusEnumType](./literals.md#migrationworkflowstatusenumtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListMigrationWorkflowsResponseTypeDef](./type_defs.md#listmigrationworkflowsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMigrationWorkflowsRequestPaginateTypeDef = {  # (1)
    "templateId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMigrationWorkflowsRequestPaginateTypeDef](./type_defs.md#listmigrationworkflowsrequestpaginatetypedef) 
