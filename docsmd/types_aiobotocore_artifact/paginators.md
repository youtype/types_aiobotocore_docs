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
3. item: `AioPageIterator[ListCustomerAgreementsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCustomerAgreementsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCustomerAgreementsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCustomerAgreementsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomerAgreementsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomerAgreementsRequestPaginateTypeDef](./type_defs.md#listcustomeragreementsrequestpaginatetypedef)
## ListReportVersionsPaginator

Type annotations and code completion for `#!python session.create_client("artifact").get_paginator("list_report_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact/paginator/ListReportVersions.html#Artifact.Paginator.ListReportVersions)

```python
# ListReportVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_artifact.paginator import ListReportVersionsPaginator

session = get_session()
async with session.create_client("artifact") as client:  # (1)
    paginator: ListReportVersionsPaginator = client.get_paginator("list_report_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListReportVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ArtifactClient](./client.md)
2. paginator: [ListReportVersionsPaginator](./paginators.md#listreportversionspaginator)
3. item: `AioPageIterator[ListReportVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListReportVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    reportId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListReportVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListReportVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListReportVersionsRequestPaginateTypeDef = {  # (1)
    "reportId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReportVersionsRequestPaginateTypeDef](./type_defs.md#listreportversionsrequestpaginatetypedef)
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
3. item: `AioPageIterator[ListReportsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListReportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListReportsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListReportsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListReportsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReportsRequestPaginateTypeDef](./type_defs.md#listreportsrequestpaginatetypedef)
