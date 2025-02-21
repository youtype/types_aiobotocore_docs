# Paginators

> [Index](../README.md) > [MTurk](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MTurk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#mturk)
    type annotations stubs module [types-aiobotocore-mturk](https://pypi.org/project/types-aiobotocore-mturk/).

## ListAssignmentsForHITPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_assignments_for_hit")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk/paginator/ListAssignmentsForHIT.html#MTurk.Paginator.ListAssignmentsForHIT)

```python
# ListAssignmentsForHITPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListAssignmentsForHITPaginator

session = get_session()
async with session.create_client("mturk") as client:  # (1)
    paginator: ListAssignmentsForHITPaginator = client.get_paginator("list_assignments_for_hit")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssignmentsForHITResponseTypeDef
        print(item)  # (3)
```

1. client: [MTurkClient](./client.md)
2. paginator: [ListAssignmentsForHITPaginator](./paginators.md#listassignmentsforhitpaginator)
3. item: [:material-code-braces: ListAssignmentsForHITResponseTypeDef](./type_defs.md#listassignmentsforhitresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssignmentsForHITPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    HITId: str,
    AssignmentStatuses: Sequence[AssignmentStatusType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssignmentsForHITResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssignmentsForHITResponseTypeDef](./type_defs.md#listassignmentsforhitresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssignmentsForHITRequestPaginateTypeDef = {  # (1)
    "HITId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssignmentsForHITRequestPaginateTypeDef](./type_defs.md#listassignmentsforhitrequestpaginatetypedef) 
## ListBonusPaymentsPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_bonus_payments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk/paginator/ListBonusPayments.html#MTurk.Paginator.ListBonusPayments)

```python
# ListBonusPaymentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListBonusPaymentsPaginator

session = get_session()
async with session.create_client("mturk") as client:  # (1)
    paginator: ListBonusPaymentsPaginator = client.get_paginator("list_bonus_payments")  # (2)
    async for item in paginator.paginate(...):
        item: ListBonusPaymentsResponseTypeDef
        print(item)  # (3)
```

1. client: [MTurkClient](./client.md)
2. paginator: [ListBonusPaymentsPaginator](./paginators.md#listbonuspaymentspaginator)
3. item: [:material-code-braces: ListBonusPaymentsResponseTypeDef](./type_defs.md#listbonuspaymentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBonusPaymentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    HITId: str = ...,
    AssignmentId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListBonusPaymentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBonusPaymentsResponseTypeDef](./type_defs.md#listbonuspaymentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBonusPaymentsRequestPaginateTypeDef = {  # (1)
    "HITId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBonusPaymentsRequestPaginateTypeDef](./type_defs.md#listbonuspaymentsrequestpaginatetypedef) 
## ListHITsForQualificationTypePaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_hits_for_qualification_type")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk/paginator/ListHITsForQualificationType.html#MTurk.Paginator.ListHITsForQualificationType)

```python
# ListHITsForQualificationTypePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListHITsForQualificationTypePaginator

session = get_session()
async with session.create_client("mturk") as client:  # (1)
    paginator: ListHITsForQualificationTypePaginator = client.get_paginator("list_hits_for_qualification_type")  # (2)
    async for item in paginator.paginate(...):
        item: ListHITsForQualificationTypeResponseTypeDef
        print(item)  # (3)
```

1. client: [MTurkClient](./client.md)
2. paginator: [ListHITsForQualificationTypePaginator](./paginators.md#listhitsforqualificationtypepaginator)
3. item: [:material-code-braces: ListHITsForQualificationTypeResponseTypeDef](./type_defs.md#listhitsforqualificationtyperesponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListHITsForQualificationTypePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    QualificationTypeId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListHITsForQualificationTypeResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHITsForQualificationTypeResponseTypeDef](./type_defs.md#listhitsforqualificationtyperesponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListHITsForQualificationTypeRequestPaginateTypeDef = {  # (1)
    "QualificationTypeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHITsForQualificationTypeRequestPaginateTypeDef](./type_defs.md#listhitsforqualificationtyperequestpaginatetypedef) 
## ListHITsPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_hits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk/paginator/ListHITs.html#MTurk.Paginator.ListHITs)

```python
# ListHITsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListHITsPaginator

session = get_session()
async with session.create_client("mturk") as client:  # (1)
    paginator: ListHITsPaginator = client.get_paginator("list_hits")  # (2)
    async for item in paginator.paginate(...):
        item: ListHITsResponseTypeDef
        print(item)  # (3)
```

1. client: [MTurkClient](./client.md)
2. paginator: [ListHITsPaginator](./paginators.md#listhitspaginator)
3. item: [:material-code-braces: ListHITsResponseTypeDef](./type_defs.md#listhitsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListHITsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListHITsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHITsResponseTypeDef](./type_defs.md#listhitsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListHITsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHITsRequestPaginateTypeDef](./type_defs.md#listhitsrequestpaginatetypedef) 
## ListQualificationRequestsPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_qualification_requests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk/paginator/ListQualificationRequests.html#MTurk.Paginator.ListQualificationRequests)

```python
# ListQualificationRequestsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListQualificationRequestsPaginator

session = get_session()
async with session.create_client("mturk") as client:  # (1)
    paginator: ListQualificationRequestsPaginator = client.get_paginator("list_qualification_requests")  # (2)
    async for item in paginator.paginate(...):
        item: ListQualificationRequestsResponseTypeDef
        print(item)  # (3)
```

1. client: [MTurkClient](./client.md)
2. paginator: [ListQualificationRequestsPaginator](./paginators.md#listqualificationrequestspaginator)
3. item: [:material-code-braces: ListQualificationRequestsResponseTypeDef](./type_defs.md#listqualificationrequestsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListQualificationRequestsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    QualificationTypeId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListQualificationRequestsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListQualificationRequestsResponseTypeDef](./type_defs.md#listqualificationrequestsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListQualificationRequestsRequestPaginateTypeDef = {  # (1)
    "QualificationTypeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQualificationRequestsRequestPaginateTypeDef](./type_defs.md#listqualificationrequestsrequestpaginatetypedef) 
## ListQualificationTypesPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_qualification_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk/paginator/ListQualificationTypes.html#MTurk.Paginator.ListQualificationTypes)

```python
# ListQualificationTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListQualificationTypesPaginator

session = get_session()
async with session.create_client("mturk") as client:  # (1)
    paginator: ListQualificationTypesPaginator = client.get_paginator("list_qualification_types")  # (2)
    async for item in paginator.paginate(...):
        item: ListQualificationTypesResponseTypeDef
        print(item)  # (3)
```

1. client: [MTurkClient](./client.md)
2. paginator: [ListQualificationTypesPaginator](./paginators.md#listqualificationtypespaginator)
3. item: [:material-code-braces: ListQualificationTypesResponseTypeDef](./type_defs.md#listqualificationtypesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListQualificationTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    MustBeRequestable: bool,
    Query: str = ...,
    MustBeOwnedByCaller: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListQualificationTypesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListQualificationTypesResponseTypeDef](./type_defs.md#listqualificationtypesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListQualificationTypesRequestPaginateTypeDef = {  # (1)
    "MustBeRequestable": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQualificationTypesRequestPaginateTypeDef](./type_defs.md#listqualificationtypesrequestpaginatetypedef) 
## ListReviewableHITsPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_reviewable_hits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk/paginator/ListReviewableHITs.html#MTurk.Paginator.ListReviewableHITs)

```python
# ListReviewableHITsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListReviewableHITsPaginator

session = get_session()
async with session.create_client("mturk") as client:  # (1)
    paginator: ListReviewableHITsPaginator = client.get_paginator("list_reviewable_hits")  # (2)
    async for item in paginator.paginate(...):
        item: ListReviewableHITsResponseTypeDef
        print(item)  # (3)
```

1. client: [MTurkClient](./client.md)
2. paginator: [ListReviewableHITsPaginator](./paginators.md#listreviewablehitspaginator)
3. item: [:material-code-braces: ListReviewableHITsResponseTypeDef](./type_defs.md#listreviewablehitsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListReviewableHITsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    HITTypeId: str = ...,
    Status: ReviewableHITStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListReviewableHITsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ReviewableHITStatusType](./literals.md#reviewablehitstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListReviewableHITsResponseTypeDef](./type_defs.md#listreviewablehitsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListReviewableHITsRequestPaginateTypeDef = {  # (1)
    "HITTypeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReviewableHITsRequestPaginateTypeDef](./type_defs.md#listreviewablehitsrequestpaginatetypedef) 
## ListWorkerBlocksPaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_worker_blocks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk/paginator/ListWorkerBlocks.html#MTurk.Paginator.ListWorkerBlocks)

```python
# ListWorkerBlocksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListWorkerBlocksPaginator

session = get_session()
async with session.create_client("mturk") as client:  # (1)
    paginator: ListWorkerBlocksPaginator = client.get_paginator("list_worker_blocks")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkerBlocksResponseTypeDef
        print(item)  # (3)
```

1. client: [MTurkClient](./client.md)
2. paginator: [ListWorkerBlocksPaginator](./paginators.md#listworkerblockspaginator)
3. item: [:material-code-braces: ListWorkerBlocksResponseTypeDef](./type_defs.md#listworkerblocksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkerBlocksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWorkerBlocksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkerBlocksResponseTypeDef](./type_defs.md#listworkerblocksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkerBlocksRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkerBlocksRequestPaginateTypeDef](./type_defs.md#listworkerblocksrequestpaginatetypedef) 
## ListWorkersWithQualificationTypePaginator

Type annotations and code completion for `#!python session.create_client("mturk").get_paginator("list_workers_with_qualification_type")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk/paginator/ListWorkersWithQualificationType.html#MTurk.Paginator.ListWorkersWithQualificationType)

```python
# ListWorkersWithQualificationTypePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mturk.paginator import ListWorkersWithQualificationTypePaginator

session = get_session()
async with session.create_client("mturk") as client:  # (1)
    paginator: ListWorkersWithQualificationTypePaginator = client.get_paginator("list_workers_with_qualification_type")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkersWithQualificationTypeResponseTypeDef
        print(item)  # (3)
```

1. client: [MTurkClient](./client.md)
2. paginator: [ListWorkersWithQualificationTypePaginator](./paginators.md#listworkerswithqualificationtypepaginator)
3. item: [:material-code-braces: ListWorkersWithQualificationTypeResponseTypeDef](./type_defs.md#listworkerswithqualificationtyperesponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkersWithQualificationTypePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    QualificationTypeId: str,
    Status: QualificationStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListWorkersWithQualificationTypeResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: QualificationStatusType](./literals.md#qualificationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListWorkersWithQualificationTypeResponseTypeDef](./type_defs.md#listworkerswithqualificationtyperesponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkersWithQualificationTypeRequestPaginateTypeDef = {  # (1)
    "QualificationTypeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkersWithQualificationTypeRequestPaginateTypeDef](./type_defs.md#listworkerswithqualificationtyperequestpaginatetypedef) 
