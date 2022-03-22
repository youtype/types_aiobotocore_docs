<a id="examples-for-aiobotocore-rekognition-module"></a>

# Examples for aiobotocore Rekognition module

> [Index](../README.md) > [Rekognition](./README.md) > Examples

- [Examples for aiobotocore Rekognition module](#examples-for-aiobotocore-rekognition-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[rekognition]` package installed.

Write your `Rekognition` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type RekognitionClient
# and provides type checking and code completion
async with session.create_client("rekognition") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeProjectVersionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_project_versions")
    async for item in paginator.paginate(...):
        # item has type DescribeProjectVersionsResponseTypeDef
        print(item)
    

    
    # waiter has type ProjectVersionRunningWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("project_version_running")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[rekognition]` or a standalone
`types_aiobotocore_rekognition` package, you have to explicitly specify
`client: RekognitionClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_rekognition.client import RekognitionClient
from types_aiobotocore_rekognition.type_defs import bool
from types_aiobotocore_rekognition.paginator import DescribeProjectVersionsPaginator
from types_aiobotocore_rekognition.waiter import ProjectVersionRunningWaiter
from types_aiobotocore_rekognition.literals import PaginatorName
from types_aiobotocore_rekognition.literals import WaiterName


session = get_session()

async with session.create_client("rekognition") as client:
    client: RekognitionClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_project_versions"
    paginator: DescribeProjectVersionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeProjectVersionsResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "project_version_running"
    waiter: ProjectVersionRunningWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
