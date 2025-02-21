# Examples

> [Index](../README.md) > [Invoicing](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Invoicing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing.html#invoicing)
    type annotations stubs module [types-aiobotocore-invoicing](https://pypi.org/project/types-aiobotocore-invoicing/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[invoicing]` package installed.

Write your `Invoicing` code as usual,
type checking and code completion should work out of the box.



```python
# InvoicingClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("invoicing") as client:  # (1)
    result = await client.batch_get_invoice_profile()  # (2)
```

1. client: [InvoicingClient](./client.md)
2. result: [:material-code-braces: BatchGetInvoiceProfileResponseTypeDef](./type_defs.md#batchgetinvoiceprofileresponsetypedef) 



```python
# ListInvoiceUnitsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("invoicing") as client:  # (1)
    paginator = client.get_paginator("list_invoice_units")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [InvoicingClient](./client.md)
2. paginator: [ListInvoiceUnitsPaginator](./paginators.md#listinvoiceunitspaginator)
3. item: [:material-code-braces: ListInvoiceUnitsResponseTypeDef](./type_defs.md#listinvoiceunitsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[invoicing]`
or a standalone `types_aiobotocore_invoicing` package, you have to explicitly specify
`client: InvoicingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# InvoicingClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_invoicing.client import InvoicingClient
from types_aiobotocore_invoicing.type_defs import BatchGetInvoiceProfileResponseTypeDef
from types_aiobotocore_invoicing.type_defs import BatchGetInvoiceProfileRequestTypeDef


session = get_session()

async with session.create_client("invoicing") as client:
    client: InvoicingClient
    kwargs: BatchGetInvoiceProfileRequestTypeDef = {...}
    result: BatchGetInvoiceProfileResponseTypeDef = await client.batch_get_invoice_profile(**kwargs)
```



```python
# ListInvoiceUnitsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_invoicing.client import InvoicingClient
from types_aiobotocore_invoicing.paginator import ListInvoiceUnitsPaginator
from types_aiobotocore_invoicing.type_defs import ListInvoiceUnitsResponseTypeDef


session = get_session()

async with session.create_client("invoicing") as client:
    client: InvoicingClient
    paginator: ListInvoiceUnitsPaginator = client.get_paginator("list_invoice_units")
    async for item in paginator.paginate(...):
        item: ListInvoiceUnitsResponseTypeDef
        print(item)
```


