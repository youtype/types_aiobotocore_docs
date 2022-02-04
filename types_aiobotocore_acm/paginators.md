<a id="paginators-for-aiobotocore-acm-module"></a>

# Paginators for aiobotocore ACM module

> [Index](..) > [ACM](.) > Paginators

Auto-generated documentation for
[ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
type annotations stubs module
[types-aiobotocore-acm](https://pypi.org/project/types-aiobotocore-acm/).

- [Paginators for aiobotocore ACM module](#paginators-for-aiobotocore-acm-module)
  - [ListCertificatesPaginator](#listcertificatespaginator)

<a id="listcertificatespaginator"></a>

## ListCertificatesPaginator

Type annotations for
`aiobotocore.create_client("acm").get_paginator("list_certificates")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_acm.paginator import ListCertificatesPaginator

def get_list_certificates_paginator() -> ListCertificatesPaginator:
    return Session().create_client("acm").get_paginator("list_certificates")
```

Boto3 documentation:
[ACM.Paginator.ListCertificates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Paginator.ListCertificates)

Arguments for `ListCertificatesPaginator.paginate` method:

- `CertificateStatuses`:
  `Sequence`\[[CertificateStatusType](./literals.md#certificatestatustype)\]
- `Includes`: [FiltersTypeDef](./type_defs.md#filterstypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCertificatesPaginator.paginate` returns
`_PageIterator`\[[ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef)\].
