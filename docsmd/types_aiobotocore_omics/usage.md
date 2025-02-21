# Examples

> [Index](../README.md) > [Omics](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Omics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#omics)
    type annotations stubs module [types-aiobotocore-omics](https://pypi.org/project/types-aiobotocore-omics/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[omics]` package installed.

Write your `Omics` code as usual,
type checking and code completion should work out of the box.



```python
# OmicsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("omics") as client:  # (1)
    result = await client.accept_share()  # (2)
```

1. client: [OmicsClient](./client.md)
2. result: [:material-code-braces: AcceptShareResponseTypeDef](./type_defs.md#acceptshareresponsetypedef) 



```python
# ListAnnotationImportJobsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("omics") as client:  # (1)
    paginator = client.get_paginator("list_annotation_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [OmicsClient](./client.md)
2. paginator: [ListAnnotationImportJobsPaginator](./paginators.md#listannotationimportjobspaginator)
3. item: [:material-code-braces: ListAnnotationImportJobsResponseTypeDef](./type_defs.md#listannotationimportjobsresponsetypedef) 



```python
# AnnotationImportJobCreatedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("omics") as client:  # (1)
    waiter = client.get_waiter("annotation_import_job_created")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [AnnotationImportJobCreatedWaiter](./waiters.md#annotationimportjobcreatedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[omics]`
or a standalone `types_aiobotocore_omics` package, you have to explicitly specify
`client: OmicsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# OmicsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_omics.client import OmicsClient
from types_aiobotocore_omics.type_defs import AcceptShareResponseTypeDef
from types_aiobotocore_omics.type_defs import AcceptShareRequestTypeDef


session = get_session()

async with session.create_client("omics") as client:
    client: OmicsClient
    kwargs: AcceptShareRequestTypeDef = {...}
    result: AcceptShareResponseTypeDef = await client.accept_share(**kwargs)
```



```python
# ListAnnotationImportJobsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_omics.client import OmicsClient
from types_aiobotocore_omics.paginator import ListAnnotationImportJobsPaginator
from types_aiobotocore_omics.type_defs import ListAnnotationImportJobsResponseTypeDef


session = get_session()

async with session.create_client("omics") as client:
    client: OmicsClient
    paginator: ListAnnotationImportJobsPaginator = client.get_paginator("list_annotation_import_jobs")
    async for item in paginator.paginate(...):
        item: ListAnnotationImportJobsResponseTypeDef
        print(item)
```



```python
# AnnotationImportJobCreatedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_omics.client import OmicsClient
from types_aiobotocore_omics.waiter import AnnotationImportJobCreatedWaiter


session = get_session()

async with session.create_client("omics") as client:
    client: OmicsClient
    waiter: AnnotationImportJobCreatedWaiter = client.get_waiter("annotation_import_job_created")
    await waiter.wait()
```
