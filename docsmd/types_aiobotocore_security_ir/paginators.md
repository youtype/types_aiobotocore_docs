# Paginators

> [Index](../README.md) > [SecurityIncidentResponse](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SecurityIncidentResponse](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#securityincidentresponse)
    type annotations stubs module [types-aiobotocore-security-ir](https://pypi.org/project/types-aiobotocore-security-ir/).

## ListCaseEditsPaginator

Type annotations and code completion for `#!python session.create_client("security-ir").get_paginator("list_case_edits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir/paginator/ListCaseEdits.html#SecurityIncidentResponse.Paginator.ListCaseEdits)

```python
# ListCaseEditsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_security_ir.paginator import ListCaseEditsPaginator

session = get_session()
async with session.create_client("security-ir") as client:  # (1)
    paginator: ListCaseEditsPaginator = client.get_paginator("list_case_edits")  # (2)
    async for item in paginator.paginate(...):
        item: ListCaseEditsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityIncidentResponseClient](./client.md)
2. paginator: [ListCaseEditsPaginator](./paginators.md#listcaseeditspaginator)
3. item: [:material-code-braces: ListCaseEditsResponseTypeDef](./type_defs.md#listcaseeditsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCaseEditsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    caseId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCaseEditsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCaseEditsResponseTypeDef](./type_defs.md#listcaseeditsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCaseEditsRequestListCaseEditsPaginateTypeDef = {  # (1)
    "caseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCaseEditsRequestListCaseEditsPaginateTypeDef](./type_defs.md#listcaseeditsrequestlistcaseeditspaginatetypedef) 
## ListCasesPaginator

Type annotations and code completion for `#!python session.create_client("security-ir").get_paginator("list_cases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir/paginator/ListCases.html#SecurityIncidentResponse.Paginator.ListCases)

```python
# ListCasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_security_ir.paginator import ListCasesPaginator

session = get_session()
async with session.create_client("security-ir") as client:  # (1)
    paginator: ListCasesPaginator = client.get_paginator("list_cases")  # (2)
    async for item in paginator.paginate(...):
        item: ListCasesResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityIncidentResponseClient](./client.md)
2. paginator: [ListCasesPaginator](./paginators.md#listcasespaginator)
3. item: [:material-code-braces: ListCasesResponseTypeDef](./type_defs.md#listcasesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCasesResponseTypeDef](./type_defs.md#listcasesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCasesRequestListCasesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCasesRequestListCasesPaginateTypeDef](./type_defs.md#listcasesrequestlistcasespaginatetypedef) 
## ListCommentsPaginator

Type annotations and code completion for `#!python session.create_client("security-ir").get_paginator("list_comments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir/paginator/ListComments.html#SecurityIncidentResponse.Paginator.ListComments)

```python
# ListCommentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_security_ir.paginator import ListCommentsPaginator

session = get_session()
async with session.create_client("security-ir") as client:  # (1)
    paginator: ListCommentsPaginator = client.get_paginator("list_comments")  # (2)
    async for item in paginator.paginate(...):
        item: ListCommentsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityIncidentResponseClient](./client.md)
2. paginator: [ListCommentsPaginator](./paginators.md#listcommentspaginator)
3. item: [:material-code-braces: ListCommentsResponseTypeDef](./type_defs.md#listcommentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCommentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    caseId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCommentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCommentsResponseTypeDef](./type_defs.md#listcommentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCommentsRequestListCommentsPaginateTypeDef = {  # (1)
    "caseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCommentsRequestListCommentsPaginateTypeDef](./type_defs.md#listcommentsrequestlistcommentspaginatetypedef) 
## ListMembershipsPaginator

Type annotations and code completion for `#!python session.create_client("security-ir").get_paginator("list_memberships")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir/paginator/ListMemberships.html#SecurityIncidentResponse.Paginator.ListMemberships)

```python
# ListMembershipsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_security_ir.paginator import ListMembershipsPaginator

session = get_session()
async with session.create_client("security-ir") as client:  # (1)
    paginator: ListMembershipsPaginator = client.get_paginator("list_memberships")  # (2)
    async for item in paginator.paginate(...):
        item: ListMembershipsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityIncidentResponseClient](./client.md)
2. paginator: [ListMembershipsPaginator](./paginators.md#listmembershipspaginator)
3. item: [:material-code-braces: ListMembershipsResponseTypeDef](./type_defs.md#listmembershipsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMembershipsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMembershipsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMembershipsResponseTypeDef](./type_defs.md#listmembershipsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMembershipsRequestListMembershipsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMembershipsRequestListMembershipsPaginateTypeDef](./type_defs.md#listmembershipsrequestlistmembershipspaginatetypedef) 
