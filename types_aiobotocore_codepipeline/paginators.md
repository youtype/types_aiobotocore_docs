<a id="paginators-for-aiobotocore-codepipeline-module"></a>

# Paginators for aiobotocore CodePipeline module

> [Index](..) > [CodePipeline](.) > Paginators

Auto-generated documentation for
[CodePipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
type annotations stubs module
[types-aiobotocore-codepipeline](https://pypi.org/project/types-aiobotocore-codepipeline/).

- [Paginators for aiobotocore CodePipeline module](#paginators-for-aiobotocore-codepipeline-module)
  - [ListActionExecutionsPaginator](#listactionexecutionspaginator)
  - [ListActionTypesPaginator](#listactiontypespaginator)
  - [ListPipelineExecutionsPaginator](#listpipelineexecutionspaginator)
  - [ListPipelinesPaginator](#listpipelinespaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)
  - [ListWebhooksPaginator](#listwebhookspaginator)

<a id="listactionexecutionspaginator"></a>

## ListActionExecutionsPaginator

Type annotations for
`session.create_client("codepipeline").get_paginator("list_action_executions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListActionExecutionsPaginator

session = get_session()
async with session.create_client("codepipeline") as client:
    client: CodePipelineClient
    paginator: ListActionExecutionsPaginator = client.get_paginator("list_action_executions")
```

Boto3 documentation:
[CodePipeline.Paginator.ListActionExecutions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionExecutions)

Arguments for `ListActionExecutionsPaginator.paginate` method:

- `pipelineName`: `str` *(required)*
- `filter`:
  [ActionExecutionFilterTypeDef](./type_defs.md#actionexecutionfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListActionExecutionsPaginator.paginate` returns
`_PageIterator`\[[ListActionExecutionsOutputTypeDef](./type_defs.md#listactionexecutionsoutputtypedef)\].

<a id="listactiontypespaginator"></a>

## ListActionTypesPaginator

Type annotations for
`session.create_client("codepipeline").get_paginator("list_action_types")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListActionTypesPaginator

session = get_session()
async with session.create_client("codepipeline") as client:
    client: CodePipelineClient
    paginator: ListActionTypesPaginator = client.get_paginator("list_action_types")
```

Boto3 documentation:
[CodePipeline.Paginator.ListActionTypes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionTypes)

Arguments for `ListActionTypesPaginator.paginate` method:

- `actionOwnerFilter`: [ActionOwnerType](./literals.md#actionownertype)
- `regionFilter`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListActionTypesPaginator.paginate` returns
`_PageIterator`\[[ListActionTypesOutputTypeDef](./type_defs.md#listactiontypesoutputtypedef)\].

<a id="listpipelineexecutionspaginator"></a>

## ListPipelineExecutionsPaginator

Type annotations for
`session.create_client("codepipeline").get_paginator("list_pipeline_executions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListPipelineExecutionsPaginator

session = get_session()
async with session.create_client("codepipeline") as client:
    client: CodePipelineClient
    paginator: ListPipelineExecutionsPaginator = client.get_paginator("list_pipeline_executions")
```

Boto3 documentation:
[CodePipeline.Paginator.ListPipelineExecutions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions)

Arguments for `ListPipelineExecutionsPaginator.paginate` method:

- `pipelineName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPipelineExecutionsPaginator.paginate` returns
`_PageIterator`\[[ListPipelineExecutionsOutputTypeDef](./type_defs.md#listpipelineexecutionsoutputtypedef)\].

<a id="listpipelinespaginator"></a>

## ListPipelinesPaginator

Type annotations for
`session.create_client("codepipeline").get_paginator("list_pipelines")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListPipelinesPaginator

session = get_session()
async with session.create_client("codepipeline") as client:
    client: CodePipelineClient
    paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")
```

Boto3 documentation:
[CodePipeline.Paginator.ListPipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelines)

Arguments for `ListPipelinesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPipelinesPaginator.paginate` returns
`_PageIterator`\[[ListPipelinesOutputTypeDef](./type_defs.md#listpipelinesoutputtypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("codepipeline").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("codepipeline") as client:
    client: CodePipelineClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[CodePipeline.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `resourceArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`_PageIterator`\[[ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)\].

<a id="listwebhookspaginator"></a>

## ListWebhooksPaginator

Type annotations for
`session.create_client("codepipeline").get_paginator("list_webhooks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.paginator import ListWebhooksPaginator

session = get_session()
async with session.create_client("codepipeline") as client:
    client: CodePipelineClient
    paginator: ListWebhooksPaginator = client.get_paginator("list_webhooks")
```

Boto3 documentation:
[CodePipeline.Paginator.ListWebhooks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListWebhooks)

Arguments for `ListWebhooksPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListWebhooksPaginator.paginate` returns
`_PageIterator`\[[ListWebhooksOutputTypeDef](./type_defs.md#listwebhooksoutputtypedef)\].
