<a id="paginators-for-aiobotocore-augmentedairuntime-module"></a>

# Paginators for aiobotocore AugmentedAIRuntime module

> [Index](..) > [AugmentedAIRuntime](.) > Paginators

Auto-generated documentation for
[AugmentedAIRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
type annotations stubs module
[types-aiobotocore-sagemaker-a2i-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime/).

- [Paginators for aiobotocore AugmentedAIRuntime module](#paginators-for-aiobotocore-augmentedairuntime-module)
  - [ListHumanLoopsPaginator](#listhumanloopspaginator)

<a id="listhumanloopspaginator"></a>

## ListHumanLoopsPaginator

Type annotations for
`session.create_client("sagemaker-a2i-runtime").get_paginator("list_human_loops")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_a2i_runtime.paginator import ListHumanLoopsPaginator

session = get_session()
async with session.create_client("sagemaker-a2i-runtime") as client:
    client: AugmentedAIRuntimeClient
    paginator: ListHumanLoopsPaginator = client.get_paginator("list_human_loops")
```

Boto3 documentation:
[AugmentedAIRuntime.Paginator.ListHumanLoops](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Paginator.ListHumanLoops)

Arguments for `ListHumanLoopsPaginator.paginate` method:

- `FlowDefinitionArn`: `str` *(required)*
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListHumanLoopsPaginator.paginate` returns
`_PageIterator`\[[ListHumanLoopsResponseTypeDef](./type_defs.md#listhumanloopsresponsetypedef)\].
