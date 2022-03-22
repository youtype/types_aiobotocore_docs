<a id="examples-for-aiobotocore-elastictranscoder-module"></a>

# Examples for aiobotocore ElasticTranscoder module

> [Index](../README.md) > [ElasticTranscoder](./README.md) > Examples

- [Examples for aiobotocore ElasticTranscoder module](#examples-for-aiobotocore-elastictranscoder-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[elastictranscoder]` package installed.

Write your `ElasticTranscoder` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ElasticTranscoderClient
# and provides type checking and code completion
async with session.create_client("elastictranscoder") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListJobsByPipelinePaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_jobs_by_pipeline")
    async for item in paginator.paginate(...):
        # item has type ListJobsByPipelineResponseTypeDef
        print(item)
    

    
    # waiter has type JobCompleteWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("job_complete")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[elastictranscoder]` or a standalone
`types_aiobotocore_elastictranscoder` package, you have to explicitly specify
`client: ElasticTranscoderClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.client import ElasticTranscoderClient
from types_aiobotocore_elastictranscoder.type_defs import bool
from types_aiobotocore_elastictranscoder.paginator import ListJobsByPipelinePaginator
from types_aiobotocore_elastictranscoder.waiter import JobCompleteWaiter
from types_aiobotocore_elastictranscoder.literals import PaginatorName
from types_aiobotocore_elastictranscoder.literals import WaiterName


session = get_session()

async with session.create_client("elastictranscoder") as client:
    client: ElasticTranscoderClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_jobs_by_pipeline"
    paginator: ListJobsByPipelinePaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListJobsByPipelineResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "job_complete"
    waiter: JobCompleteWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
