# Paginators

> [Index](../README.md) > [Transfer](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Transfer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
    type annotations stubs module [types-aiobotocore-transfer](https://pypi.org/project/types-aiobotocore-transfer/).

## ListAccessesPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_accesses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAccesses)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListAccessesPaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListAccessesPaginator = client.get_paginator("list_accesses")
```


### paginate

Type annotations and code completion for `#!python ListAccessesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ServerId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccessesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccessesResponseTypeDef](./type_defs.md#listaccessesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAccessesRequestListAccessesPaginateTypeDef = {  # (1)
    "ServerId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessesRequestListAccessesPaginateTypeDef](./type_defs.md#listaccessesrequestlistaccessespaginatetypedef) 
## ListExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListExecutions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListExecutionsPaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListExecutionsPaginator = client.get_paginator("list_executions")
```


### paginate

Type annotations and code completion for `#!python ListExecutionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    WorkflowId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListExecutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListExecutionsResponseTypeDef](./type_defs.md#listexecutionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListExecutionsRequestListExecutionsPaginateTypeDef = {  # (1)
    "WorkflowId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExecutionsRequestListExecutionsPaginateTypeDef](./type_defs.md#listexecutionsrequestlistexecutionspaginatetypedef) 
## ListSecurityPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_security_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListSecurityPolicies)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListSecurityPoliciesPaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListSecurityPoliciesPaginator = client.get_paginator("list_security_policies")
```


### paginate

Type annotations and code completion for `#!python ListSecurityPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSecurityPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSecurityPoliciesResponseTypeDef](./type_defs.md#listsecuritypoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef](./type_defs.md#listsecuritypoliciesrequestlistsecuritypoliciespaginatetypedef) 
## ListServersPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListServers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListServersPaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListServersPaginator = client.get_paginator("list_servers")
```


### paginate

Type annotations and code completion for `#!python ListServersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListServersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListServersResponseTypeDef](./type_defs.md#listserversresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListServersRequestListServersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServersRequestListServersPaginateTypeDef](./type_defs.md#listserversrequestlistserverspaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListTagsForResource)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef = {  # (1)
    "Arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourcerequestlisttagsforresourcepaginatetypedef) 
## ListUsersPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListUsers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListUsersPaginator = client.get_paginator("list_users")
```


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ServerId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUsersRequestListUsersPaginateTypeDef = {  # (1)
    "ServerId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestListUsersPaginateTypeDef](./type_defs.md#listusersrequestlistuserspaginatetypedef) 
## ListWorkflowsPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_workflows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListWorkflows)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListWorkflowsPaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListWorkflowsPaginator = client.get_paginator("list_workflows")
```


### paginate

Type annotations and code completion for `#!python ListWorkflowsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListWorkflowsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListWorkflowsRequestListWorkflowsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowsRequestListWorkflowsPaginateTypeDef](./type_defs.md#listworkflowsrequestlistworkflowspaginatetypedef) 
