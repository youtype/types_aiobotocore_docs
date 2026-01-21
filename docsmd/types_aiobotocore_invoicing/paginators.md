# Paginators

> [Index](../README.md) > [Invoicing](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Invoicing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing.html#invoicing)
    type annotations stubs module [types-aiobotocore-invoicing](https://pypi.org/project/types-aiobotocore-invoicing/).

## ListInvoiceSummariesPaginator

Type annotations and code completion for `#!python session.create_client("invoicing").get_paginator("list_invoice_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/paginator/ListInvoiceSummaries.html#Invoicing.Paginator.ListInvoiceSummaries)

```python
# ListInvoiceSummariesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_invoicing.paginator import ListInvoiceSummariesPaginator

session = get_session()
async with session.create_client("invoicing") as client:  # (1)
    paginator: ListInvoiceSummariesPaginator = client.get_paginator("list_invoice_summaries")  # (2)
    async for item in paginator.paginate(...):
        item: ListInvoiceSummariesResponseTypeDef
        print(item)  # (3)
```

1. client: [InvoicingClient](./client.md)
2. paginator: [ListInvoiceSummariesPaginator](./paginators.md#listinvoicesummariespaginator)
3. item: `AioPageIterator[ListInvoiceSummariesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListInvoiceSummariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Selector: InvoiceSummariesSelectorTypeDef,  # (1)
    Filter: InvoiceSummariesFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListInvoiceSummariesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: InvoiceSummariesSelectorTypeDef](./type_defs.md#invoicesummariesselectortypedef)
2. See [:material-code-braces: InvoiceSummariesFilterTypeDef](./type_defs.md#invoicesummariesfiltertypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListInvoiceSummariesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListInvoiceSummariesRequestPaginateTypeDef = {  # (1)
    "Selector": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInvoiceSummariesRequestPaginateTypeDef](./type_defs.md#listinvoicesummariesrequestpaginatetypedef)
## ListInvoiceUnitsPaginator

Type annotations and code completion for `#!python session.create_client("invoicing").get_paginator("list_invoice_units")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/paginator/ListInvoiceUnits.html#Invoicing.Paginator.ListInvoiceUnits)

```python
# ListInvoiceUnitsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_invoicing.paginator import ListInvoiceUnitsPaginator

session = get_session()
async with session.create_client("invoicing") as client:  # (1)
    paginator: ListInvoiceUnitsPaginator = client.get_paginator("list_invoice_units")  # (2)
    async for item in paginator.paginate(...):
        item: ListInvoiceUnitsResponseTypeDef
        print(item)  # (3)
```

1. client: [InvoicingClient](./client.md)
2. paginator: [ListInvoiceUnitsPaginator](./paginators.md#listinvoiceunitspaginator)
3. item: `AioPageIterator[ListInvoiceUnitsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListInvoiceUnitsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: FiltersTypeDef = ...,  # (1)
    AsOf: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListInvoiceUnitsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListInvoiceUnitsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListInvoiceUnitsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInvoiceUnitsRequestPaginateTypeDef](./type_defs.md#listinvoiceunitsrequestpaginatetypedef)
## ListProcurementPortalPreferencesPaginator

Type annotations and code completion for `#!python session.create_client("invoicing").get_paginator("list_procurement_portal_preferences")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/paginator/ListProcurementPortalPreferences.html#Invoicing.Paginator.ListProcurementPortalPreferences)

```python
# ListProcurementPortalPreferencesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_invoicing.paginator import ListProcurementPortalPreferencesPaginator

session = get_session()
async with session.create_client("invoicing") as client:  # (1)
    paginator: ListProcurementPortalPreferencesPaginator = client.get_paginator("list_procurement_portal_preferences")  # (2)
    async for item in paginator.paginate(...):
        item: ListProcurementPortalPreferencesResponseTypeDef
        print(item)  # (3)
```

1. client: [InvoicingClient](./client.md)
2. paginator: [ListProcurementPortalPreferencesPaginator](./paginators.md#listprocurementportalpreferencespaginator)
3. item: `AioPageIterator[ListProcurementPortalPreferencesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProcurementPortalPreferencesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProcurementPortalPreferencesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProcurementPortalPreferencesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProcurementPortalPreferencesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProcurementPortalPreferencesRequestPaginateTypeDef](./type_defs.md#listprocurementportalpreferencesrequestpaginatetypedef)
