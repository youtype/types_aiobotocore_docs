# Paginators

> [Index](../README.md) > [CodePipeline](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodePipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#codepipeline)
    type annotations stubs module [types-aiobotocore-codepipeline](https://pypi.org/project/types-aiobotocore-codepipeline/).

## ListActionExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("codepipeline").get_paginator("list_action_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline/paginator/ListActionExecutions.html#CodePipeline.Paginator.ListActionExecutions)

```python
# ListActionExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListActionExecutionsPaginator

session = get_session()
async with session.create_client("codepipeline") as client:  # (1)
    paginator: ListActionExecutionsPaginator = client.get_paginator("list_action_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListActionExecutionsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodePipelineClient](./client.md)
2. paginator: [ListActionExecutionsPaginator](./paginators.md#listactionexecutionspaginator)
3. item: `AioPageIterator[ListActionExecutionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListActionExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    pipelineName: str,
    filter: ActionExecutionFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListActionExecutionsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ActionExecutionFilterTypeDef](./type_defs.md#actionexecutionfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListActionExecutionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListActionExecutionsInputPaginateTypeDef = {  # (1)
    "pipelineName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListActionExecutionsInputPaginateTypeDef](./type_defs.md#listactionexecutionsinputpaginatetypedef)
## ListActionTypesPaginator

Type annotations and code completion for `#!python session.create_client("codepipeline").get_paginator("list_action_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline/paginator/ListActionTypes.html#CodePipeline.Paginator.ListActionTypes)

```python
# ListActionTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListActionTypesPaginator

session = get_session()
async with session.create_client("codepipeline") as client:  # (1)
    paginator: ListActionTypesPaginator = client.get_paginator("list_action_types")  # (2)
    async for item in paginator.paginate(...):
        item: ListActionTypesOutputTypeDef
        print(item)  # (3)
```

1. client: [CodePipelineClient](./client.md)
2. paginator: [ListActionTypesPaginator](./paginators.md#listactiontypespaginator)
3. item: `AioPageIterator[ListActionTypesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListActionTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    actionOwnerFilter: ActionOwnerType = ...,  # (1)
    regionFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListActionTypesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ActionOwnerType](./literals.md#actionownertype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListActionTypesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListActionTypesInputPaginateTypeDef = {  # (1)
    "actionOwnerFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListActionTypesInputPaginateTypeDef](./type_defs.md#listactiontypesinputpaginatetypedef)
## ListDeployActionExecutionTargetsPaginator

Type annotations and code completion for `#!python session.create_client("codepipeline").get_paginator("list_deploy_action_execution_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline/paginator/ListDeployActionExecutionTargets.html#CodePipeline.Paginator.ListDeployActionExecutionTargets)

```python
# ListDeployActionExecutionTargetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListDeployActionExecutionTargetsPaginator

session = get_session()
async with session.create_client("codepipeline") as client:  # (1)
    paginator: ListDeployActionExecutionTargetsPaginator = client.get_paginator("list_deploy_action_execution_targets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeployActionExecutionTargetsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodePipelineClient](./client.md)
2. paginator: [ListDeployActionExecutionTargetsPaginator](./paginators.md#listdeployactionexecutiontargetspaginator)
3. item: `AioPageIterator[ListDeployActionExecutionTargetsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDeployActionExecutionTargetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    actionExecutionId: str,
    pipelineName: str = ...,
    filters: Sequence[TargetFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDeployActionExecutionTargetsOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[TargetFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDeployActionExecutionTargetsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDeployActionExecutionTargetsInputPaginateTypeDef = {  # (1)
    "actionExecutionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeployActionExecutionTargetsInputPaginateTypeDef](./type_defs.md#listdeployactionexecutiontargetsinputpaginatetypedef)
## ListPipelineExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("codepipeline").get_paginator("list_pipeline_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline/paginator/ListPipelineExecutions.html#CodePipeline.Paginator.ListPipelineExecutions)

```python
# ListPipelineExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListPipelineExecutionsPaginator

session = get_session()
async with session.create_client("codepipeline") as client:  # (1)
    paginator: ListPipelineExecutionsPaginator = client.get_paginator("list_pipeline_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPipelineExecutionsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodePipelineClient](./client.md)
2. paginator: [ListPipelineExecutionsPaginator](./paginators.md#listpipelineexecutionspaginator)
3. item: `AioPageIterator[ListPipelineExecutionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPipelineExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    pipelineName: str,
    filter: PipelineExecutionFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListPipelineExecutionsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: PipelineExecutionFilterTypeDef](./type_defs.md#pipelineexecutionfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListPipelineExecutionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPipelineExecutionsInputPaginateTypeDef = {  # (1)
    "pipelineName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPipelineExecutionsInputPaginateTypeDef](./type_defs.md#listpipelineexecutionsinputpaginatetypedef)
## ListPipelinesPaginator

Type annotations and code completion for `#!python session.create_client("codepipeline").get_paginator("list_pipelines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline/paginator/ListPipelines.html#CodePipeline.Paginator.ListPipelines)

```python
# ListPipelinesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListPipelinesPaginator

session = get_session()
async with session.create_client("codepipeline") as client:  # (1)
    paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")  # (2)
    async for item in paginator.paginate(...):
        item: ListPipelinesOutputTypeDef
        print(item)  # (3)
```

1. client: [CodePipelineClient](./client.md)
2. paginator: [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
3. item: `AioPageIterator[ListPipelinesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPipelinesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPipelinesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPipelinesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPipelinesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPipelinesInputPaginateTypeDef](./type_defs.md#listpipelinesinputpaginatetypedef)
## ListRuleExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("codepipeline").get_paginator("list_rule_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline/paginator/ListRuleExecutions.html#CodePipeline.Paginator.ListRuleExecutions)

```python
# ListRuleExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListRuleExecutionsPaginator

session = get_session()
async with session.create_client("codepipeline") as client:  # (1)
    paginator: ListRuleExecutionsPaginator = client.get_paginator("list_rule_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListRuleExecutionsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodePipelineClient](./client.md)
2. paginator: [ListRuleExecutionsPaginator](./paginators.md#listruleexecutionspaginator)
3. item: `AioPageIterator[ListRuleExecutionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRuleExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    pipelineName: str,
    filter: RuleExecutionFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListRuleExecutionsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: RuleExecutionFilterTypeDef](./type_defs.md#ruleexecutionfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListRuleExecutionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRuleExecutionsInputPaginateTypeDef = {  # (1)
    "pipelineName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRuleExecutionsInputPaginateTypeDef](./type_defs.md#listruleexecutionsinputpaginatetypedef)
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("codepipeline").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline/paginator/ListTagsForResource.html#CodePipeline.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("codepipeline") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceOutputTypeDef
        print(item)  # (3)
```

1. client: [CodePipelineClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: `AioPageIterator[ListTagsForResourceOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTagsForResourceOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTagsForResourceOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceInputPaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputPaginateTypeDef](./type_defs.md#listtagsforresourceinputpaginatetypedef)
## ListWebhooksPaginator

Type annotations and code completion for `#!python session.create_client("codepipeline").get_paginator("list_webhooks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline/paginator/ListWebhooks.html#CodePipeline.Paginator.ListWebhooks)

```python
# ListWebhooksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListWebhooksPaginator

session = get_session()
async with session.create_client("codepipeline") as client:  # (1)
    paginator: ListWebhooksPaginator = client.get_paginator("list_webhooks")  # (2)
    async for item in paginator.paginate(...):
        item: ListWebhooksOutputTypeDef
        print(item)  # (3)
```

1. client: [CodePipelineClient](./client.md)
2. paginator: [ListWebhooksPaginator](./paginators.md#listwebhookspaginator)
3. item: `AioPageIterator[ListWebhooksOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWebhooksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListWebhooksOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListWebhooksOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWebhooksInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWebhooksInputPaginateTypeDef](./type_defs.md#listwebhooksinputpaginatetypedef)
