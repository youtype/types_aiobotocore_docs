# Paginators

> [Index](../README.md) > [Honeycode](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Honeycode](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
    type annotations stubs module [types-aiobotocore-honeycode](https://pypi.org/project/types-aiobotocore-honeycode/).

## ListTableColumnsPaginator

Type annotations and code completion for `#!python session.create_client("honeycode").get_paginator("list_table_columns")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableColumns)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_honeycode.paginator import ListTableColumnsPaginator

session = get_session()
async with session.create_client("honeycode") as client:  # (1)
    paginator: ListTableColumnsPaginator = client.get_paginator("list_table_columns")  # (2)
    async for item in paginator.paginate(...):
        item: ListTableColumnsResultTypeDef
        print(item)  # (3)
```

1. client: [HoneycodeClient](./client.md)
2. paginator: [ListTableColumnsPaginator](./paginators.md#listtablecolumnspaginator)
3. item: [:material-code-braces: ListTableColumnsResultTypeDef](./type_defs.md#listtablecolumnsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListTableColumnsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    workbookId: str,
    tableId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTableColumnsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTableColumnsResultTypeDef](./type_defs.md#listtablecolumnsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListTableColumnsRequestListTableColumnsPaginateTypeDef = {  # (1)
    "workbookId": ...,
    "tableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTableColumnsRequestListTableColumnsPaginateTypeDef](./type_defs.md#listtablecolumnsrequestlisttablecolumnspaginatetypedef) 
## ListTableRowsPaginator

Type annotations and code completion for `#!python session.create_client("honeycode").get_paginator("list_table_rows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableRows)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_honeycode.paginator import ListTableRowsPaginator

session = get_session()
async with session.create_client("honeycode") as client:  # (1)
    paginator: ListTableRowsPaginator = client.get_paginator("list_table_rows")  # (2)
    async for item in paginator.paginate(...):
        item: ListTableRowsResultTypeDef
        print(item)  # (3)
```

1. client: [HoneycodeClient](./client.md)
2. paginator: [ListTableRowsPaginator](./paginators.md#listtablerowspaginator)
3. item: [:material-code-braces: ListTableRowsResultTypeDef](./type_defs.md#listtablerowsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListTableRowsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    workbookId: str,
    tableId: str,
    rowIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTableRowsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTableRowsResultTypeDef](./type_defs.md#listtablerowsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListTableRowsRequestListTableRowsPaginateTypeDef = {  # (1)
    "workbookId": ...,
    "tableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTableRowsRequestListTableRowsPaginateTypeDef](./type_defs.md#listtablerowsrequestlisttablerowspaginatetypedef) 
## ListTablesPaginator

Type annotations and code completion for `#!python session.create_client("honeycode").get_paginator("list_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTables)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_honeycode.paginator import ListTablesPaginator

session = get_session()
async with session.create_client("honeycode") as client:  # (1)
    paginator: ListTablesPaginator = client.get_paginator("list_tables")  # (2)
    async for item in paginator.paginate(...):
        item: ListTablesResultTypeDef
        print(item)  # (3)
```

1. client: [HoneycodeClient](./client.md)
2. paginator: [ListTablesPaginator](./paginators.md#listtablespaginator)
3. item: [:material-code-braces: ListTablesResultTypeDef](./type_defs.md#listtablesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListTablesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    workbookId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTablesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTablesResultTypeDef](./type_defs.md#listtablesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListTablesRequestListTablesPaginateTypeDef = {  # (1)
    "workbookId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTablesRequestListTablesPaginateTypeDef](./type_defs.md#listtablesrequestlisttablespaginatetypedef) 
## QueryTableRowsPaginator

Type annotations and code completion for `#!python session.create_client("honeycode").get_paginator("query_table_rows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.QueryTableRows)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_honeycode.paginator import QueryTableRowsPaginator

session = get_session()
async with session.create_client("honeycode") as client:  # (1)
    paginator: QueryTableRowsPaginator = client.get_paginator("query_table_rows")  # (2)
    async for item in paginator.paginate(...):
        item: QueryTableRowsResultTypeDef
        print(item)  # (3)
```

1. client: [HoneycodeClient](./client.md)
2. paginator: [QueryTableRowsPaginator](./paginators.md#querytablerowspaginator)
3. item: [:material-code-braces: QueryTableRowsResultTypeDef](./type_defs.md#querytablerowsresulttypedef) 


### paginate

Type annotations and code completion for `#!python QueryTableRowsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    workbookId: str,
    tableId: str,
    filterFormula: FilterTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[QueryTableRowsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: QueryTableRowsResultTypeDef](./type_defs.md#querytablerowsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: QueryTableRowsRequestQueryTableRowsPaginateTypeDef = {  # (1)
    "workbookId": ...,
    "tableId": ...,
    "filterFormula": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: QueryTableRowsRequestQueryTableRowsPaginateTypeDef](./type_defs.md#querytablerowsrequestquerytablerowspaginatetypedef) 
