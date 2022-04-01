# Paginators

> [Index](../README.md) > [MTurk](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MTurk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
    type annotations stubs module [types-aiobotocore-mturk](https://pypi.org/project/types-aiobotocore-mturk/).

## ListAssignmentsForHITPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_assignments_for_hit")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListAssignmentsForHITPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListAssignmentsForHITPaginator = client.get_paginator("list_assignments_for_hit")
```


### paginate

Type annotations and code completion for `#!python ListAssignmentsForHITPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    HITId: str,
    AssignmentStatuses: Sequence[AssignmentStatusType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAssignmentsForHITResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssignmentsForHITResponseTypeDef](./type_defs.md#listassignmentsforhitresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = {  # (1)
    "HITId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef](./type_defs.md#listassignmentsforhitrequestlistassignmentsforhitpaginatetypedef) 
## ListBonusPaymentsPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_bonus_payments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListBonusPaymentsPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListBonusPaymentsPaginator = client.get_paginator("list_bonus_payments")
```


### paginate

Type annotations and code completion for `#!python ListBonusPaymentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    HITId: str = ...,
    AssignmentId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBonusPaymentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBonusPaymentsResponseTypeDef](./type_defs.md#listbonuspaymentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef = {  # (1)
    "HITId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef](./type_defs.md#listbonuspaymentsrequestlistbonuspaymentspaginatetypedef) 
## ListHITsPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_hits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListHITsPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListHITsPaginator = client.get_paginator("list_hits")
```


### paginate

Type annotations and code completion for `#!python ListHITsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListHITsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHITsResponseTypeDef](./type_defs.md#listhitsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListHITsRequestListHITsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHITsRequestListHITsPaginateTypeDef](./type_defs.md#listhitsrequestlisthitspaginatetypedef) 
## ListHITsForQualificationTypePaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_hits_for_qualification_type")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListHITsForQualificationTypePaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListHITsForQualificationTypePaginator = client.get_paginator("list_hits_for_qualification_type")
```


### paginate

Type annotations and code completion for `#!python ListHITsForQualificationTypePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    QualificationTypeId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListHITsForQualificationTypeResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHITsForQualificationTypeResponseTypeDef](./type_defs.md#listhitsforqualificationtyperesponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = {  # (1)
    "QualificationTypeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef](./type_defs.md#listhitsforqualificationtyperequestlisthitsforqualificationtypepaginatetypedef) 
## ListQualificationRequestsPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_qualification_requests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListQualificationRequestsPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListQualificationRequestsPaginator = client.get_paginator("list_qualification_requests")
```


### paginate

Type annotations and code completion for `#!python ListQualificationRequestsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    QualificationTypeId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListQualificationRequestsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListQualificationRequestsResponseTypeDef](./type_defs.md#listqualificationrequestsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef = {  # (1)
    "QualificationTypeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef](./type_defs.md#listqualificationrequestsrequestlistqualificationrequestspaginatetypedef) 
## ListQualificationTypesPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_qualification_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListQualificationTypesPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListQualificationTypesPaginator = client.get_paginator("list_qualification_types")
```


### paginate

Type annotations and code completion for `#!python ListQualificationTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    MustBeRequestable: bool,
    Query: str = ...,
    MustBeOwnedByCaller: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListQualificationTypesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListQualificationTypesResponseTypeDef](./type_defs.md#listqualificationtypesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListQualificationTypesRequestListQualificationTypesPaginateTypeDef = {  # (1)
    "MustBeRequestable": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQualificationTypesRequestListQualificationTypesPaginateTypeDef](./type_defs.md#listqualificationtypesrequestlistqualificationtypespaginatetypedef) 
## ListReviewableHITsPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_reviewable_hits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListReviewableHITsPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListReviewableHITsPaginator = client.get_paginator("list_reviewable_hits")
```


### paginate

Type annotations and code completion for `#!python ListReviewableHITsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    HITTypeId: str = ...,
    Status: ReviewableHITStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListReviewableHITsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ReviewableHITStatusType](./literals.md#reviewablehitstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListReviewableHITsResponseTypeDef](./type_defs.md#listreviewablehitsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListReviewableHITsRequestListReviewableHITsPaginateTypeDef = {  # (1)
    "HITTypeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReviewableHITsRequestListReviewableHITsPaginateTypeDef](./type_defs.md#listreviewablehitsrequestlistreviewablehitspaginatetypedef) 
## ListWorkerBlocksPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_worker_blocks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListWorkerBlocksPaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListWorkerBlocksPaginator = client.get_paginator("list_worker_blocks")
```


### paginate

Type annotations and code completion for `#!python ListWorkerBlocksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListWorkerBlocksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkerBlocksResponseTypeDef](./type_defs.md#listworkerblocksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef](./type_defs.md#listworkerblocksrequestlistworkerblockspaginatetypedef) 
## ListWorkersWithQualificationTypePaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_workers_with_qualification_type")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListWorkersWithQualificationTypePaginator

session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
    paginator: ListWorkersWithQualificationTypePaginator = client.get_paginator("list_workers_with_qualification_type")
```


### paginate

Type annotations and code completion for `#!python ListWorkersWithQualificationTypePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    QualificationTypeId: str,
    Status: QualificationStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListWorkersWithQualificationTypeResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: QualificationStatusType](./literals.md#qualificationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListWorkersWithQualificationTypeResponseTypeDef](./type_defs.md#listworkerswithqualificationtyperesponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = {  # (1)
    "QualificationTypeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef](./type_defs.md#listworkerswithqualificationtyperequestlistworkerswithqualificationtypepaginatetypedef) 
