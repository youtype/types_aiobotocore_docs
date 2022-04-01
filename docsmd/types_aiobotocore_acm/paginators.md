# Paginators

> [Index](../README.md) > [ACM](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
    type annotations stubs module [types-aiobotocore-acm](https://pypi.org/project/types-aiobotocore-acm/).

## ListCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("acm").get_paginator("list_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Paginator.ListCertificates)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_acm.paginator import ListCertificatesPaginator

session = get_session()
async with session.create_client("acm") as client:
    client: ACMClient
    paginator: ListCertificatesPaginator = client.get_paginator("list_certificates")
```


### paginate

Type annotations and code completion for `#!python ListCertificatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CertificateStatuses: Sequence[CertificateStatusType] = ...,  # (1)
    Includes: FiltersTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListCertificatesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
2. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCertificatesRequestListCertificatesPaginateTypeDef = {  # (1)
    "CertificateStatuses": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCertificatesRequestListCertificatesPaginateTypeDef](./type_defs.md#listcertificatesrequestlistcertificatespaginatetypedef) 
