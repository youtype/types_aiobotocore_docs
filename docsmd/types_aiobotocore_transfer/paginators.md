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
async with session.create_client("transfer") as client:  # (1)
    paginator: ListAccessesPaginator = client.get_paginator("list_accesses")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessesResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListAccessesPaginator](./paginators.md#listaccessespaginator)
3. item: [:material-code-braces: ListAccessesResponseTypeDef](./type_defs.md#listaccessesresponsetypedef) 


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
## ListAgreementsPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_agreements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAgreements)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListAgreementsPaginator

session = get_session()
async with session.create_client("transfer") as client:  # (1)
    paginator: ListAgreementsPaginator = client.get_paginator("list_agreements")  # (2)
    async for item in paginator.paginate(...):
        item: ListAgreementsResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListAgreementsPaginator](./paginators.md#listagreementspaginator)
3. item: [:material-code-braces: ListAgreementsResponseTypeDef](./type_defs.md#listagreementsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAgreementsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ServerId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAgreementsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAgreementsResponseTypeDef](./type_defs.md#listagreementsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAgreementsRequestListAgreementsPaginateTypeDef = {  # (1)
    "ServerId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAgreementsRequestListAgreementsPaginateTypeDef](./type_defs.md#listagreementsrequestlistagreementspaginatetypedef) 
## ListCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListCertificates)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListCertificatesPaginator

session = get_session()
async with session.create_client("transfer") as client:  # (1)
    paginator: ListCertificatesPaginator = client.get_paginator("list_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: ListCertificatesResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)
3. item: [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCertificatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCertificatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCertificatesRequestListCertificatesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCertificatesRequestListCertificatesPaginateTypeDef](./type_defs.md#listcertificatesrequestlistcertificatespaginatetypedef) 
## ListConnectorsPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_connectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListConnectors)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListConnectorsPaginator

session = get_session()
async with session.create_client("transfer") as client:  # (1)
    paginator: ListConnectorsPaginator = client.get_paginator("list_connectors")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectorsResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
3. item: [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConnectorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListConnectorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListConnectorsRequestListConnectorsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectorsRequestListConnectorsPaginateTypeDef](./type_defs.md#listconnectorsrequestlistconnectorspaginatetypedef) 
## ListExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListExecutions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListExecutionsPaginator

session = get_session()
async with session.create_client("transfer") as client:  # (1)
    paginator: ListExecutionsPaginator = client.get_paginator("list_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListExecutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListExecutionsPaginator](./paginators.md#listexecutionspaginator)
3. item: [:material-code-braces: ListExecutionsResponseTypeDef](./type_defs.md#listexecutionsresponsetypedef) 


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
## ListProfilesPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListProfiles)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListProfilesPaginator

session = get_session()
async with session.create_client("transfer") as client:  # (1)
    paginator: ListProfilesPaginator = client.get_paginator("list_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListProfilesPaginator](./paginators.md#listprofilespaginator)
3. item: [:material-code-braces: ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProfilesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ProfileType: ProfileTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListProfilesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ProfileTypeType](./literals.md#profiletypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListProfilesRequestListProfilesPaginateTypeDef = {  # (1)
    "ProfileType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProfilesRequestListProfilesPaginateTypeDef](./type_defs.md#listprofilesrequestlistprofilespaginatetypedef) 
## ListSecurityPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_security_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListSecurityPolicies)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListSecurityPoliciesPaginator

session = get_session()
async with session.create_client("transfer") as client:  # (1)
    paginator: ListSecurityPoliciesPaginator = client.get_paginator("list_security_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListSecurityPoliciesPaginator](./paginators.md#listsecuritypoliciespaginator)
3. item: [:material-code-braces: ListSecurityPoliciesResponseTypeDef](./type_defs.md#listsecuritypoliciesresponsetypedef) 


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
async with session.create_client("transfer") as client:  # (1)
    paginator: ListServersPaginator = client.get_paginator("list_servers")  # (2)
    async for item in paginator.paginate(...):
        item: ListServersResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListServersPaginator](./paginators.md#listserverspaginator)
3. item: [:material-code-braces: ListServersResponseTypeDef](./type_defs.md#listserversresponsetypedef) 


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
async with session.create_client("transfer") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


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
async with session.create_client("transfer") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


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
async with session.create_client("transfer") as client:  # (1)
    paginator: ListWorkflowsPaginator = client.get_paginator("list_workflows")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkflowsResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListWorkflowsPaginator](./paginators.md#listworkflowspaginator)
3. item: [:material-code-braces: ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef) 


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
