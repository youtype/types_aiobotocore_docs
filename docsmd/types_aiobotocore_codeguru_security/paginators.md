# Paginators

> [Index](../README.md) > [CodeGuruSecurity](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeGuruSecurity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
    type annotations stubs module [types-aiobotocore-codeguru-security](https://pypi.org/project/types-aiobotocore-codeguru-security/).

## GetFindingsPaginator

Type annotations and code completion for `#!python session.create_client("codeguru-security").get_paginator("get_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.GetFindings)

```python
# GetFindingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codeguru_security.paginator import GetFindingsPaginator

session = get_session()
async with session.create_client("codeguru-security") as client:  # (1)
    paginator: GetFindingsPaginator = client.get_paginator("get_findings")  # (2)
    async for item in paginator.paginate(...):
        item: GetFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeGuruSecurityClient](./client.md)
2. paginator: [GetFindingsPaginator](./paginators.md#getfindingspaginator)
3. item: [:material-code-braces: GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetFindingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    scanName: str,
    status: StatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetFindingsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetFindingsRequestGetFindingsPaginateTypeDef = {  # (1)
    "scanName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetFindingsRequestGetFindingsPaginateTypeDef](./type_defs.md#getfindingsrequestgetfindingspaginatetypedef) 
## ListFindingsMetricsPaginator

Type annotations and code completion for `#!python session.create_client("codeguru-security").get_paginator("list_findings_metrics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics)

```python
# ListFindingsMetricsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codeguru_security.paginator import ListFindingsMetricsPaginator

session = get_session()
async with session.create_client("codeguru-security") as client:  # (1)
    paginator: ListFindingsMetricsPaginator = client.get_paginator("list_findings_metrics")  # (2)
    async for item in paginator.paginate(...):
        item: ListFindingsMetricsResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeGuruSecurityClient](./client.md)
2. paginator: [ListFindingsMetricsPaginator](./paginators.md#listfindingsmetricspaginator)
3. item: [:material-code-braces: ListFindingsMetricsResponseTypeDef](./type_defs.md#listfindingsmetricsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFindingsMetricsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    endDate: Union[datetime, str],
    startDate: Union[datetime, str],
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFindingsMetricsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFindingsMetricsResponseTypeDef](./type_defs.md#listfindingsmetricsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = {  # (1)
    "endDate": ...,
    "startDate": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef](./type_defs.md#listfindingsmetricsrequestlistfindingsmetricspaginatetypedef) 
## ListScansPaginator

Type annotations and code completion for `#!python session.create_client("codeguru-security").get_paginator("list_scans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListScans)

```python
# ListScansPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codeguru_security.paginator import ListScansPaginator

session = get_session()
async with session.create_client("codeguru-security") as client:  # (1)
    paginator: ListScansPaginator = client.get_paginator("list_scans")  # (2)
    async for item in paginator.paginate(...):
        item: ListScansResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeGuruSecurityClient](./client.md)
2. paginator: [ListScansPaginator](./paginators.md#listscanspaginator)
3. item: [:material-code-braces: ListScansResponseTypeDef](./type_defs.md#listscansresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListScansPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListScansResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListScansResponseTypeDef](./type_defs.md#listscansresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListScansRequestListScansPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListScansRequestListScansPaginateTypeDef](./type_defs.md#listscansrequestlistscanspaginatetypedef) 
