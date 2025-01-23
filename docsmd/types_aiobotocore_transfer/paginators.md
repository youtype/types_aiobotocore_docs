# Paginators

> [Index](../README.md) > [Transfer](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Transfer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#transfer)
    type annotations stubs module [types-aiobotocore-transfer](https://pypi.org/project/types-aiobotocore-transfer/).

## ListAccessesPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_accesses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer/paginator/ListAccesses.html#Transfer.Paginator.ListAccesses)

```python
# ListAccessesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    ServerId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAccessesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccessesResponseTypeDef](./type_defs.md#listaccessesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccessesRequestPaginateTypeDef = {  # (1)
    "ServerId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessesRequestPaginateTypeDef](./type_defs.md#listaccessesrequestpaginatetypedef) 
## ListAgreementsPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_agreements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer/paginator/ListAgreements.html#Transfer.Paginator.ListAgreements)

```python
# ListAgreementsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    ServerId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAgreementsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAgreementsResponseTypeDef](./type_defs.md#listagreementsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAgreementsRequestPaginateTypeDef = {  # (1)
    "ServerId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAgreementsRequestPaginateTypeDef](./type_defs.md#listagreementsrequestpaginatetypedef) 
## ListCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer/paginator/ListCertificates.html#Transfer.Paginator.ListCertificates)

```python
# ListCertificatesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCertificatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCertificatesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCertificatesRequestPaginateTypeDef](./type_defs.md#listcertificatesrequestpaginatetypedef) 
## ListConnectorsPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_connectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer/paginator/ListConnectors.html#Transfer.Paginator.ListConnectors)

```python
# ListConnectorsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConnectorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConnectorsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectorsRequestPaginateTypeDef](./type_defs.md#listconnectorsrequestpaginatetypedef) 
## ListExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer/paginator/ListExecutions.html#Transfer.Paginator.ListExecutions)

```python
# ListExecutionsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    WorkflowId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListExecutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListExecutionsResponseTypeDef](./type_defs.md#listexecutionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListExecutionsRequestPaginateTypeDef = {  # (1)
    "WorkflowId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExecutionsRequestPaginateTypeDef](./type_defs.md#listexecutionsrequestpaginatetypedef) 
## ListFileTransferResultsPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_file_transfer_results")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer/paginator/ListFileTransferResults.html#Transfer.Paginator.ListFileTransferResults)

```python
# ListFileTransferResultsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListFileTransferResultsPaginator

session = get_session()
async with session.create_client("transfer") as client:  # (1)
    paginator: ListFileTransferResultsPaginator = client.get_paginator("list_file_transfer_results")  # (2)
    async for item in paginator.paginate(...):
        item: ListFileTransferResultsResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListFileTransferResultsPaginator](./paginators.md#listfiletransferresultspaginator)
3. item: [:material-code-braces: ListFileTransferResultsResponseTypeDef](./type_defs.md#listfiletransferresultsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFileTransferResultsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConnectorId: str,
    TransferId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFileTransferResultsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFileTransferResultsResponseTypeDef](./type_defs.md#listfiletransferresultsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFileTransferResultsRequestPaginateTypeDef = {  # (1)
    "ConnectorId": ...,
    "TransferId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFileTransferResultsRequestPaginateTypeDef](./type_defs.md#listfiletransferresultsrequestpaginatetypedef) 
## ListProfilesPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer/paginator/ListProfiles.html#Transfer.Paginator.ListProfiles)

```python
# ListProfilesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    ProfileType: ProfileTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListProfilesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ProfileTypeType](./literals.md#profiletypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProfilesRequestPaginateTypeDef = {  # (1)
    "ProfileType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProfilesRequestPaginateTypeDef](./type_defs.md#listprofilesrequestpaginatetypedef) 
## ListSecurityPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_security_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer/paginator/ListSecurityPolicies.html#Transfer.Paginator.ListSecurityPolicies)

```python
# ListSecurityPoliciesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSecurityPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSecurityPoliciesResponseTypeDef](./type_defs.md#listsecuritypoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSecurityPoliciesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityPoliciesRequestPaginateTypeDef](./type_defs.md#listsecuritypoliciesrequestpaginatetypedef) 
## ListServersPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer/paginator/ListServers.html#Transfer.Paginator.ListServers)

```python
# ListServersPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListServersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListServersResponseTypeDef](./type_defs.md#listserversresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListServersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServersRequestPaginateTypeDef](./type_defs.md#listserversrequestpaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer/paginator/ListTagsForResource.html#Transfer.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    Arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestPaginateTypeDef = {  # (1)
    "Arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef) 
## ListUsersPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer/paginator/ListUsers.html#Transfer.Paginator.ListUsers)

```python
# ListUsersPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    ServerId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUsersRequestPaginateTypeDef = {  # (1)
    "ServerId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestPaginateTypeDef](./type_defs.md#listusersrequestpaginatetypedef) 
## ListWebAppsPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_web_apps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer/paginator/ListWebApps.html#Transfer.Paginator.ListWebApps)

```python
# ListWebAppsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListWebAppsPaginator

session = get_session()
async with session.create_client("transfer") as client:  # (1)
    paginator: ListWebAppsPaginator = client.get_paginator("list_web_apps")  # (2)
    async for item in paginator.paginate(...):
        item: ListWebAppsResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListWebAppsPaginator](./paginators.md#listwebappspaginator)
3. item: [:material-code-braces: ListWebAppsResponseTypeDef](./type_defs.md#listwebappsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWebAppsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWebAppsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWebAppsResponseTypeDef](./type_defs.md#listwebappsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWebAppsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWebAppsRequestPaginateTypeDef](./type_defs.md#listwebappsrequestpaginatetypedef) 
## ListWorkflowsPaginator

Type annotations and code completion for `#!python session.create_client("transfer").get_paginator("list_workflows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer/paginator/ListWorkflows.html#Transfer.Paginator.ListWorkflows)

```python
# ListWorkflowsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWorkflowsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowsRequestPaginateTypeDef](./type_defs.md#listworkflowsrequestpaginatetypedef) 
