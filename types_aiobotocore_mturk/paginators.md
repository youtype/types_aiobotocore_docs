<a id="paginators-for-aiobotocore-mturk-module"></a>

# Paginators for aiobotocore MTurk module

> [Index](..) > [MTurk](.) > Paginators

Auto-generated documentation for
[MTurk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
type annotations stubs module
[types-aiobotocore-mturk](https://pypi.org/project/types-aiobotocore-mturk/).

- [Paginators for aiobotocore MTurk module](#paginators-for-aiobotocore-mturk-module)
  - [ListAssignmentsForHITPaginator](#listassignmentsforhitpaginator)
  - [ListBonusPaymentsPaginator](#listbonuspaymentspaginator)
  - [ListHITsPaginator](#listhitspaginator)
  - [ListHITsForQualificationTypePaginator](#listhitsforqualificationtypepaginator)
  - [ListQualificationRequestsPaginator](#listqualificationrequestspaginator)
  - [ListQualificationTypesPaginator](#listqualificationtypespaginator)
  - [ListReviewableHITsPaginator](#listreviewablehitspaginator)
  - [ListWorkerBlocksPaginator](#listworkerblockspaginator)
  - [ListWorkersWithQualificationTypePaginator](#listworkerswithqualificationtypepaginator)

<a id="listassignmentsforhitpaginator"></a>

## ListAssignmentsForHITPaginator

Type annotations for
`session.create_client("mturk").get_paginator("list_assignments_for_hit")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListAssignmentsForHITPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListAssignmentsForHITPaginator = client.get_paginator("list_assignments_for_hit")
```

Boto3 documentation:
[MTurk.Paginator.ListAssignmentsForHIT](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT)

Arguments for `ListAssignmentsForHITPaginator.paginate` method:

- `HITId`: `str` *(required)*
- `AssignmentStatuses`:
  `Sequence`\[[AssignmentStatusType](./literals.md#assignmentstatustype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAssignmentsForHITPaginator.paginate` returns
`_PageIterator`\[[ListAssignmentsForHITResponseTypeDef](./type_defs.md#listassignmentsforhitresponsetypedef)\].

<a id="listbonuspaymentspaginator"></a>

## ListBonusPaymentsPaginator

Type annotations for
`session.create_client("mturk").get_paginator("list_bonus_payments")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListBonusPaymentsPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListBonusPaymentsPaginator = client.get_paginator("list_bonus_payments")
```

Boto3 documentation:
[MTurk.Paginator.ListBonusPayments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments)

Arguments for `ListBonusPaymentsPaginator.paginate` method:

- `HITId`: `str`
- `AssignmentId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBonusPaymentsPaginator.paginate` returns
`_PageIterator`\[[ListBonusPaymentsResponseTypeDef](./type_defs.md#listbonuspaymentsresponsetypedef)\].

<a id="listhitspaginator"></a>

## ListHITsPaginator

Type annotations for
`session.create_client("mturk").get_paginator("list_hits")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListHITsPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListHITsPaginator = client.get_paginator("list_hits")
```

Boto3 documentation:
[MTurk.Paginator.ListHITs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs)

Arguments for `ListHITsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListHITsPaginator.paginate` returns
`_PageIterator`\[[ListHITsResponseTypeDef](./type_defs.md#listhitsresponsetypedef)\].

<a id="listhitsforqualificationtypepaginator"></a>

## ListHITsForQualificationTypePaginator

Type annotations for
`session.create_client("mturk").get_paginator("list_hits_for_qualification_type")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListHITsForQualificationTypePaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListHITsForQualificationTypePaginator = client.get_paginator("list_hits_for_qualification_type")
```

Boto3 documentation:
[MTurk.Paginator.ListHITsForQualificationType](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType)

Arguments for `ListHITsForQualificationTypePaginator.paginate` method:

- `QualificationTypeId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListHITsForQualificationTypePaginator.paginate` returns
`_PageIterator`\[[ListHITsForQualificationTypeResponseTypeDef](./type_defs.md#listhitsforqualificationtyperesponsetypedef)\].

<a id="listqualificationrequestspaginator"></a>

## ListQualificationRequestsPaginator

Type annotations for
`session.create_client("mturk").get_paginator("list_qualification_requests")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListQualificationRequestsPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListQualificationRequestsPaginator = client.get_paginator("list_qualification_requests")
```

Boto3 documentation:
[MTurk.Paginator.ListQualificationRequests](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests)

Arguments for `ListQualificationRequestsPaginator.paginate` method:

- `QualificationTypeId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListQualificationRequestsPaginator.paginate` returns
`_PageIterator`\[[ListQualificationRequestsResponseTypeDef](./type_defs.md#listqualificationrequestsresponsetypedef)\].

<a id="listqualificationtypespaginator"></a>

## ListQualificationTypesPaginator

Type annotations for
`session.create_client("mturk").get_paginator("list_qualification_types")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListQualificationTypesPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListQualificationTypesPaginator = client.get_paginator("list_qualification_types")
```

Boto3 documentation:
[MTurk.Paginator.ListQualificationTypes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes)

Arguments for `ListQualificationTypesPaginator.paginate` method:

- `MustBeRequestable`: `bool` *(required)*
- `Query`: `str`
- `MustBeOwnedByCaller`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListQualificationTypesPaginator.paginate` returns
`_PageIterator`\[[ListQualificationTypesResponseTypeDef](./type_defs.md#listqualificationtypesresponsetypedef)\].

<a id="listreviewablehitspaginator"></a>

## ListReviewableHITsPaginator

Type annotations for
`session.create_client("mturk").get_paginator("list_reviewable_hits")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListReviewableHITsPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListReviewableHITsPaginator = client.get_paginator("list_reviewable_hits")
```

Boto3 documentation:
[MTurk.Paginator.ListReviewableHITs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs)

Arguments for `ListReviewableHITsPaginator.paginate` method:

- `HITTypeId`: `str`
- `Status`: [ReviewableHITStatusType](./literals.md#reviewablehitstatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListReviewableHITsPaginator.paginate` returns
`_PageIterator`\[[ListReviewableHITsResponseTypeDef](./type_defs.md#listreviewablehitsresponsetypedef)\].

<a id="listworkerblockspaginator"></a>

## ListWorkerBlocksPaginator

Type annotations for
`session.create_client("mturk").get_paginator("list_worker_blocks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListWorkerBlocksPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListWorkerBlocksPaginator = client.get_paginator("list_worker_blocks")
```

Boto3 documentation:
[MTurk.Paginator.ListWorkerBlocks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks)

Arguments for `ListWorkerBlocksPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListWorkerBlocksPaginator.paginate` returns
`_PageIterator`\[[ListWorkerBlocksResponseTypeDef](./type_defs.md#listworkerblocksresponsetypedef)\].

<a id="listworkerswithqualificationtypepaginator"></a>

## ListWorkersWithQualificationTypePaginator

Type annotations for
`session.create_client("mturk").get_paginator("list_workers_with_qualification_type")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListWorkersWithQualificationTypePaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListWorkersWithQualificationTypePaginator = client.get_paginator("list_workers_with_qualification_type")
```

Boto3 documentation:
[MTurk.Paginator.ListWorkersWithQualificationType](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType)

Arguments for `ListWorkersWithQualificationTypePaginator.paginate` method:

- `QualificationTypeId`: `str` *(required)*
- `Status`: [QualificationStatusType](./literals.md#qualificationstatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListWorkersWithQualificationTypePaginator.paginate` returns
`_PageIterator`\[[ListWorkersWithQualificationTypeResponseTypeDef](./type_defs.md#listworkerswithqualificationtyperesponsetypedef)\].
