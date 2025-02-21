# Examples

> [Index](../README.md) > [QuickSight](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [QuickSight](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#quicksight)
    type annotations stubs module [types-aiobotocore-quicksight](https://pypi.org/project/types-aiobotocore-quicksight/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[quicksight]` package installed.

Write your `QuickSight` code as usual,
type checking and code completion should work out of the box.



```python
# QuickSightClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("quicksight") as client:  # (1)
    result = await client.batch_create_topic_reviewed_answer()  # (2)
```

1. client: [QuickSightClient](./client.md)
2. result: [:material-code-braces: BatchCreateTopicReviewedAnswerResponseTypeDef](./type_defs.md#batchcreatetopicreviewedanswerresponsetypedef) 



```python
# DescribeFolderPermissionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("quicksight") as client:  # (1)
    paginator = client.get_paginator("describe_folder_permissions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [DescribeFolderPermissionsPaginator](./paginators.md#describefolderpermissionspaginator)
3. item: [:material-code-braces: DescribeFolderPermissionsResponseTypeDef](./type_defs.md#describefolderpermissionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[quicksight]`
or a standalone `types_aiobotocore_quicksight` package, you have to explicitly specify
`client: QuickSightClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# QuickSightClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.client import QuickSightClient
from types_aiobotocore_quicksight.type_defs import BatchCreateTopicReviewedAnswerResponseTypeDef
from types_aiobotocore_quicksight.type_defs import BatchCreateTopicReviewedAnswerRequestTypeDef


session = get_session()

async with session.create_client("quicksight") as client:
    client: QuickSightClient
    kwargs: BatchCreateTopicReviewedAnswerRequestTypeDef = {...}
    result: BatchCreateTopicReviewedAnswerResponseTypeDef = await client.batch_create_topic_reviewed_answer(**kwargs)
```



```python
# DescribeFolderPermissionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.client import QuickSightClient
from types_aiobotocore_quicksight.paginator import DescribeFolderPermissionsPaginator
from types_aiobotocore_quicksight.type_defs import DescribeFolderPermissionsResponseTypeDef


session = get_session()

async with session.create_client("quicksight") as client:
    client: QuickSightClient
    paginator: DescribeFolderPermissionsPaginator = client.get_paginator("describe_folder_permissions")
    async for item in paginator.paginate(...):
        item: DescribeFolderPermissionsResponseTypeDef
        print(item)
```


