<a id="paginators-for-aiobotocore-support-module"></a>

# Paginators for aiobotocore Support module

> [Index](../README.md) > [Support](./README.md) > Paginators

Auto-generated documentation for
[Support](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
type annotations stubs module
[types-aiobotocore-support](https://pypi.org/project/types-aiobotocore-support/).

- [Paginators for aiobotocore Support module](#paginators-for-aiobotocore-support-module)
  - [DescribeCasesPaginator](#describecasespaginator)
  - [DescribeCommunicationsPaginator](#describecommunicationspaginator)

<a id="describecasespaginator"></a>

## DescribeCasesPaginator

Type annotations for
`session.create_client("support").get_paginator("describe_cases")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_support.paginator import DescribeCasesPaginator

session = get_session()
async with session.create_client("support") as client:
    client: SupportClient
    paginator: DescribeCasesPaginator = client.get_paginator("describe_cases")
```

Boto3 documentation:
[Support.Paginator.DescribeCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCases)

Arguments for `DescribeCasesPaginator.paginate` method:

- `caseIdList`: `Sequence`\[`str`\]
- `displayId`: `str`
- `afterTime`: `str`
- `beforeTime`: `str`
- `includeResolvedCases`: `bool`
- `language`: `str`
- `includeCommunications`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeCasesPaginator.paginate` returns
`AsyncIterator`\[[DescribeCasesResponseTypeDef](./type_defs.md#describecasesresponsetypedef)\].

<a id="describecommunicationspaginator"></a>

## DescribeCommunicationsPaginator

Type annotations for
`session.create_client("support").get_paginator("describe_communications")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_support.paginator import DescribeCommunicationsPaginator

session = get_session()
async with session.create_client("support") as client:
    client: SupportClient
    paginator: DescribeCommunicationsPaginator = client.get_paginator("describe_communications")
```

Boto3 documentation:
[Support.Paginator.DescribeCommunications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCommunications)

Arguments for `DescribeCommunicationsPaginator.paginate` method:

- `caseId`: `str` *(required)*
- `beforeTime`: `str`
- `afterTime`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeCommunicationsPaginator.paginate` returns
`AsyncIterator`\[[DescribeCommunicationsResponseTypeDef](./type_defs.md#describecommunicationsresponsetypedef)\].
