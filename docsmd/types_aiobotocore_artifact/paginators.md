# Paginators

> [Index](../README.md) > [Artifact](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
    type annotations stubs module [types-aiobotocore-artifact](https://pypi.org/project/types-aiobotocore-artifact/).

## ListReportsPaginator

Type annotations and code completion for `#!python session.create_client("artifact").get_paginator("list_reports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Paginator.ListReports)

```python
# ListReportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_artifact.paginator import ListReportsPaginator

session = get_session()
async with session.create_client("artifact") as client:  # (1)
    paginator: ListReportsPaginator = client.get_paginator("list_reports")  # (2)
    async for item in paginator.paginate(...):
        item: ListReportsResponseTypeDef
        print(item)  # (3)
```

1. client: [ArtifactClient](./client.md)
2. paginator: [ListReportsPaginator](./paginators.md#listreportspaginator)
3. item: [:material-code-braces: ListReportsResponseTypeDef](./type_defs.md#listreportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListReportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListReportsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListReportsResponseTypeDef](./type_defs.md#listreportsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListReportsRequestListReportsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReportsRequestListReportsPaginateTypeDef](./type_defs.md#listreportsrequestlistreportspaginatetypedef) 
