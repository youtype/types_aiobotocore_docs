# Paginators

> [Index](../README.md) > [Artifact](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#artifact)
    type annotations stubs module [types-aiobotocore-artifact](https://pypi.org/project/types-aiobotocore-artifact/).

## ListCustomerAgreementsPaginator

Type annotations and code completion for `#!python session.create_client("artifact").get_paginator("list_customer_agreements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact/paginator/ListCustomerAgreements.html#Artifact.Paginator.ListCustomerAgreements)

```python
# ListCustomerAgreementsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_artifact.paginator import ListCustomerAgreementsPaginator

session = get_session()
async with session.create_client("artifact") as client:  # (1)
    paginator: ListCustomerAgreementsPaginator = client.get_paginator("list_customer_agreements")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomerAgreementsResponseTypeDef
        print(item)  # (3)
```

1. client: [ArtifactClient](./client.md)
2. paginator: [ListCustomerAgreementsPaginator](./paginators.md#listcustomeragreementspaginator)
3. item: [:material-code-braces: ListCustomerAgreementsResponseTypeDef](./type_defs.md#listcustomeragreementsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomerAgreementsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCustomerAgreementsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomerAgreementsResponseTypeDef](./type_defs.md#listcustomeragreementsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomerAgreementsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomerAgreementsRequestPaginateTypeDef](./type_defs.md#listcustomeragreementsrequestpaginatetypedef) 
## ListReportsPaginator

Type annotations and code completion for `#!python session.create_client("artifact").get_paginator("list_reports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact/paginator/ListReports.html#Artifact.Paginator.ListReports)

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
) -> AioPageIterator[ListReportsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListReportsResponseTypeDef](./type_defs.md#listreportsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListReportsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReportsRequestPaginateTypeDef](./type_defs.md#listreportsrequestpaginatetypedef) 
