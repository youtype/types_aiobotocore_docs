# Paginators

> [Index](../README.md) > [TaxSettings](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [TaxSettings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#taxsettings)
    type annotations stubs module [types-aiobotocore-taxsettings](https://pypi.org/project/types-aiobotocore-taxsettings/).

## ListSupplementalTaxRegistrationsPaginator

Type annotations and code completion for `#!python session.create_client("taxsettings").get_paginator("list_supplemental_tax_registrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/paginator/ListSupplementalTaxRegistrations.html#TaxSettings.Paginator.ListSupplementalTaxRegistrations)

```python
# ListSupplementalTaxRegistrationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_taxsettings.paginator import ListSupplementalTaxRegistrationsPaginator

session = get_session()
async with session.create_client("taxsettings") as client:  # (1)
    paginator: ListSupplementalTaxRegistrationsPaginator = client.get_paginator("list_supplemental_tax_registrations")  # (2)
    async for item in paginator.paginate(...):
        item: ListSupplementalTaxRegistrationsResponseTypeDef
        print(item)  # (3)
```

1. client: [TaxSettingsClient](./client.md)
2. paginator: [ListSupplementalTaxRegistrationsPaginator](./paginators.md#listsupplementaltaxregistrationspaginator)
3. item: [:material-code-braces: ListSupplementalTaxRegistrationsResponseTypeDef](./type_defs.md#listsupplementaltaxregistrationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSupplementalTaxRegistrationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSupplementalTaxRegistrationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSupplementalTaxRegistrationsResponseTypeDef](./type_defs.md#listsupplementaltaxregistrationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSupplementalTaxRegistrationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSupplementalTaxRegistrationsRequestPaginateTypeDef](./type_defs.md#listsupplementaltaxregistrationsrequestpaginatetypedef) 
## ListTaxExemptionsPaginator

Type annotations and code completion for `#!python session.create_client("taxsettings").get_paginator("list_tax_exemptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/paginator/ListTaxExemptions.html#TaxSettings.Paginator.ListTaxExemptions)

```python
# ListTaxExemptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_taxsettings.paginator import ListTaxExemptionsPaginator

session = get_session()
async with session.create_client("taxsettings") as client:  # (1)
    paginator: ListTaxExemptionsPaginator = client.get_paginator("list_tax_exemptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListTaxExemptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [TaxSettingsClient](./client.md)
2. paginator: [ListTaxExemptionsPaginator](./paginators.md#listtaxexemptionspaginator)
3. item: [:material-code-braces: ListTaxExemptionsResponseTypeDef](./type_defs.md#listtaxexemptionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTaxExemptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTaxExemptionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTaxExemptionsResponseTypeDef](./type_defs.md#listtaxexemptionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTaxExemptionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTaxExemptionsRequestPaginateTypeDef](./type_defs.md#listtaxexemptionsrequestpaginatetypedef) 
## ListTaxRegistrationsPaginator

Type annotations and code completion for `#!python session.create_client("taxsettings").get_paginator("list_tax_registrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/paginator/ListTaxRegistrations.html#TaxSettings.Paginator.ListTaxRegistrations)

```python
# ListTaxRegistrationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_taxsettings.paginator import ListTaxRegistrationsPaginator

session = get_session()
async with session.create_client("taxsettings") as client:  # (1)
    paginator: ListTaxRegistrationsPaginator = client.get_paginator("list_tax_registrations")  # (2)
    async for item in paginator.paginate(...):
        item: ListTaxRegistrationsResponseTypeDef
        print(item)  # (3)
```

1. client: [TaxSettingsClient](./client.md)
2. paginator: [ListTaxRegistrationsPaginator](./paginators.md#listtaxregistrationspaginator)
3. item: [:material-code-braces: ListTaxRegistrationsResponseTypeDef](./type_defs.md#listtaxregistrationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTaxRegistrationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTaxRegistrationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTaxRegistrationsResponseTypeDef](./type_defs.md#listtaxregistrationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTaxRegistrationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTaxRegistrationsRequestPaginateTypeDef](./type_defs.md#listtaxregistrationsrequestpaginatetypedef) 
