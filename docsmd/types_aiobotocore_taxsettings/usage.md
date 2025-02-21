# Examples

> [Index](../README.md) > [TaxSettings](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [TaxSettings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#taxsettings)
    type annotations stubs module [types-aiobotocore-taxsettings](https://pypi.org/project/types-aiobotocore-taxsettings/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[taxsettings]` package installed.

Write your `TaxSettings` code as usual,
type checking and code completion should work out of the box.



```python
# TaxSettingsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("taxsettings") as client:  # (1)
    result = await client.batch_delete_tax_registration()  # (2)
```

1. client: [TaxSettingsClient](./client.md)
2. result: [:material-code-braces: BatchDeleteTaxRegistrationResponseTypeDef](./type_defs.md#batchdeletetaxregistrationresponsetypedef) 



```python
# ListSupplementalTaxRegistrationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("taxsettings") as client:  # (1)
    paginator = client.get_paginator("list_supplemental_tax_registrations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [TaxSettingsClient](./client.md)
2. paginator: [ListSupplementalTaxRegistrationsPaginator](./paginators.md#listsupplementaltaxregistrationspaginator)
3. item: [:material-code-braces: ListSupplementalTaxRegistrationsResponseTypeDef](./type_defs.md#listsupplementaltaxregistrationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[taxsettings]`
or a standalone `types_aiobotocore_taxsettings` package, you have to explicitly specify
`client: TaxSettingsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# TaxSettingsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_taxsettings.client import TaxSettingsClient
from types_aiobotocore_taxsettings.type_defs import BatchDeleteTaxRegistrationResponseTypeDef
from types_aiobotocore_taxsettings.type_defs import BatchDeleteTaxRegistrationRequestTypeDef


session = get_session()

async with session.create_client("taxsettings") as client:
    client: TaxSettingsClient
    kwargs: BatchDeleteTaxRegistrationRequestTypeDef = {...}
    result: BatchDeleteTaxRegistrationResponseTypeDef = await client.batch_delete_tax_registration(**kwargs)
```



```python
# ListSupplementalTaxRegistrationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_taxsettings.client import TaxSettingsClient
from types_aiobotocore_taxsettings.paginator import ListSupplementalTaxRegistrationsPaginator
from types_aiobotocore_taxsettings.type_defs import ListSupplementalTaxRegistrationsResponseTypeDef


session = get_session()

async with session.create_client("taxsettings") as client:
    client: TaxSettingsClient
    paginator: ListSupplementalTaxRegistrationsPaginator = client.get_paginator("list_supplemental_tax_registrations")
    async for item in paginator.paginate(...):
        item: ListSupplementalTaxRegistrationsResponseTypeDef
        print(item)
```


