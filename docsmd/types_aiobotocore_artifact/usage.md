# Examples

> [Index](../README.md) > [Artifact](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
    type annotations stubs module [types-aiobotocore-artifact](https://pypi.org/project/types-aiobotocore-artifact/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[artifact]` package installed.

Write your `Artifact` code as usual,
type checking and code completion should work out of the box.



```python
# ArtifactClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("artifact") as client:  # (1)
    result = await client.get_report()  # (2)
```

1. client: [ArtifactClient](./client.md)
2. result: [:material-code-braces: GetReportResponseTypeDef](./type_defs.md#getreportresponsetypedef) 



```python
# ListReportsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("artifact") as client:  # (1)
    paginator = client.get_paginator("list_reports")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ArtifactClient](./client.md)
2. paginator: [ListReportsPaginator](./paginators.md#listreportspaginator)
3. item: [:material-code-braces: ListReportsResponseTypeDef](./type_defs.md#listreportsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[artifact]`
or a standalone `types_aiobotocore_artifact` package, you have to explicitly specify
`client: ArtifactClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ArtifactClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_artifact.client import ArtifactClient
from types_aiobotocore_artifact.type_defs import GetReportResponseTypeDef
from types_aiobotocore_artifact.type_defs import GetReportRequestRequestTypeDef


session = get_session()

async with session.create_client("artifact") as client:
    client: ArtifactClient
    kwargs: GetReportRequestRequestTypeDef = {...}
    result: GetReportResponseTypeDef = await client.get_report(**kwargs)
```



```python
# ListReportsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_artifact.client import ArtifactClient
from types_aiobotocore_artifact.paginator import ListReportsPaginator
from types_aiobotocore_artifact.type_defs import ListReportsResponseTypeDef


session = get_session()

async with session.create_client("artifact") as client:
    client: ArtifactClient
    paginator: ListReportsPaginator = client.get_paginator("list_reports")
    async for item in paginator.paginate(...):
        item: ListReportsResponseTypeDef
        print(item)
```


