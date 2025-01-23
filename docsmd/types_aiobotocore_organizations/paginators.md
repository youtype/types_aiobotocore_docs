# Paginators

> [Index](../README.md) > [Organizations](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Organizations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#organizations)
    type annotations stubs module [types-aiobotocore-organizations](https://pypi.org/project/types-aiobotocore-organizations/).

## ListAWSServiceAccessForOrganizationPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_aws_service_access_for_organization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListAWSServiceAccessForOrganization.html#Organizations.Paginator.ListAWSServiceAccessForOrganization)

```python
# ListAWSServiceAccessForOrganizationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListAWSServiceAccessForOrganizationPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListAWSServiceAccessForOrganizationPaginator = client.get_paginator("list_aws_service_access_for_organization")  # (2)
    async for item in paginator.paginate(...):
        item: ListAWSServiceAccessForOrganizationResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListAWSServiceAccessForOrganizationPaginator](./paginators.md#listawsserviceaccessfororganizationpaginator)
3. item: [:material-code-braces: ListAWSServiceAccessForOrganizationResponseTypeDef](./type_defs.md#listawsserviceaccessfororganizationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAWSServiceAccessForOrganizationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAWSServiceAccessForOrganizationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAWSServiceAccessForOrganizationResponseTypeDef](./type_defs.md#listawsserviceaccessfororganizationresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAWSServiceAccessForOrganizationRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAWSServiceAccessForOrganizationRequestPaginateTypeDef](./type_defs.md#listawsserviceaccessfororganizationrequestpaginatetypedef) 
## ListAccountsForParentPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_accounts_for_parent")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListAccountsForParent.html#Organizations.Paginator.ListAccountsForParent)

```python
# ListAccountsForParentPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListAccountsForParentPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListAccountsForParentPaginator = client.get_paginator("list_accounts_for_parent")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountsForParentResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListAccountsForParentPaginator](./paginators.md#listaccountsforparentpaginator)
3. item: [:material-code-braces: ListAccountsForParentResponseTypeDef](./type_defs.md#listaccountsforparentresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccountsForParentPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ParentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAccountsForParentResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccountsForParentResponseTypeDef](./type_defs.md#listaccountsforparentresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountsForParentRequestPaginateTypeDef = {  # (1)
    "ParentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountsForParentRequestPaginateTypeDef](./type_defs.md#listaccountsforparentrequestpaginatetypedef) 
## ListAccountsPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListAccounts.html#Organizations.Paginator.ListAccounts)

```python
# ListAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListAccountsPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListAccountsPaginator = client.get_paginator("list_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListAccountsPaginator](./paginators.md#listaccountspaginator)
3. item: [:material-code-braces: ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountsRequestPaginateTypeDef](./type_defs.md#listaccountsrequestpaginatetypedef) 
## ListChildrenPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_children")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListChildren.html#Organizations.Paginator.ListChildren)

```python
# ListChildrenPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListChildrenPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListChildrenPaginator = client.get_paginator("list_children")  # (2)
    async for item in paginator.paginate(...):
        item: ListChildrenResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListChildrenPaginator](./paginators.md#listchildrenpaginator)
3. item: [:material-code-braces: ListChildrenResponseTypeDef](./type_defs.md#listchildrenresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChildrenPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ParentId: str,
    ChildType: ChildTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListChildrenResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ChildTypeType](./literals.md#childtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListChildrenResponseTypeDef](./type_defs.md#listchildrenresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListChildrenRequestPaginateTypeDef = {  # (1)
    "ParentId": ...,
    "ChildType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChildrenRequestPaginateTypeDef](./type_defs.md#listchildrenrequestpaginatetypedef) 
## ListCreateAccountStatusPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_create_account_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListCreateAccountStatus.html#Organizations.Paginator.ListCreateAccountStatus)

```python
# ListCreateAccountStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListCreateAccountStatusPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListCreateAccountStatusPaginator = client.get_paginator("list_create_account_status")  # (2)
    async for item in paginator.paginate(...):
        item: ListCreateAccountStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListCreateAccountStatusPaginator](./paginators.md#listcreateaccountstatuspaginator)
3. item: [:material-code-braces: ListCreateAccountStatusResponseTypeDef](./type_defs.md#listcreateaccountstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCreateAccountStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    States: Sequence[CreateAccountStateType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListCreateAccountStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: CreateAccountStateType](./literals.md#createaccountstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListCreateAccountStatusResponseTypeDef](./type_defs.md#listcreateaccountstatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCreateAccountStatusRequestPaginateTypeDef = {  # (1)
    "States": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCreateAccountStatusRequestPaginateTypeDef](./type_defs.md#listcreateaccountstatusrequestpaginatetypedef) 
## ListDelegatedAdministratorsPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_delegated_administrators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListDelegatedAdministrators.html#Organizations.Paginator.ListDelegatedAdministrators)

```python
# ListDelegatedAdministratorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListDelegatedAdministratorsPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListDelegatedAdministratorsPaginator = client.get_paginator("list_delegated_administrators")  # (2)
    async for item in paginator.paginate(...):
        item: ListDelegatedAdministratorsResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListDelegatedAdministratorsPaginator](./paginators.md#listdelegatedadministratorspaginator)
3. item: [:material-code-braces: ListDelegatedAdministratorsResponseTypeDef](./type_defs.md#listdelegatedadministratorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDelegatedAdministratorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServicePrincipal: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDelegatedAdministratorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDelegatedAdministratorsResponseTypeDef](./type_defs.md#listdelegatedadministratorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDelegatedAdministratorsRequestPaginateTypeDef = {  # (1)
    "ServicePrincipal": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDelegatedAdministratorsRequestPaginateTypeDef](./type_defs.md#listdelegatedadministratorsrequestpaginatetypedef) 
## ListDelegatedServicesForAccountPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_delegated_services_for_account")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListDelegatedServicesForAccount.html#Organizations.Paginator.ListDelegatedServicesForAccount)

```python
# ListDelegatedServicesForAccountPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListDelegatedServicesForAccountPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListDelegatedServicesForAccountPaginator = client.get_paginator("list_delegated_services_for_account")  # (2)
    async for item in paginator.paginate(...):
        item: ListDelegatedServicesForAccountResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListDelegatedServicesForAccountPaginator](./paginators.md#listdelegatedservicesforaccountpaginator)
3. item: [:material-code-braces: ListDelegatedServicesForAccountResponseTypeDef](./type_defs.md#listdelegatedservicesforaccountresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDelegatedServicesForAccountPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDelegatedServicesForAccountResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDelegatedServicesForAccountResponseTypeDef](./type_defs.md#listdelegatedservicesforaccountresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDelegatedServicesForAccountRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDelegatedServicesForAccountRequestPaginateTypeDef](./type_defs.md#listdelegatedservicesforaccountrequestpaginatetypedef) 
## ListHandshakesForAccountPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_handshakes_for_account")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListHandshakesForAccount.html#Organizations.Paginator.ListHandshakesForAccount)

```python
# ListHandshakesForAccountPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListHandshakesForAccountPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListHandshakesForAccountPaginator = client.get_paginator("list_handshakes_for_account")  # (2)
    async for item in paginator.paginate(...):
        item: ListHandshakesForAccountResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListHandshakesForAccountPaginator](./paginators.md#listhandshakesforaccountpaginator)
3. item: [:material-code-braces: ListHandshakesForAccountResponsePaginatorTypeDef](./type_defs.md#listhandshakesforaccountresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListHandshakesForAccountPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: HandshakeFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListHandshakesForAccountResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: HandshakeFilterTypeDef](./type_defs.md#handshakefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListHandshakesForAccountResponsePaginatorTypeDef](./type_defs.md#listhandshakesforaccountresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListHandshakesForAccountRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHandshakesForAccountRequestPaginateTypeDef](./type_defs.md#listhandshakesforaccountrequestpaginatetypedef) 
## ListHandshakesForOrganizationPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_handshakes_for_organization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListHandshakesForOrganization.html#Organizations.Paginator.ListHandshakesForOrganization)

```python
# ListHandshakesForOrganizationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListHandshakesForOrganizationPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListHandshakesForOrganizationPaginator = client.get_paginator("list_handshakes_for_organization")  # (2)
    async for item in paginator.paginate(...):
        item: ListHandshakesForOrganizationResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListHandshakesForOrganizationPaginator](./paginators.md#listhandshakesfororganizationpaginator)
3. item: [:material-code-braces: ListHandshakesForOrganizationResponsePaginatorTypeDef](./type_defs.md#listhandshakesfororganizationresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListHandshakesForOrganizationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: HandshakeFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListHandshakesForOrganizationResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: HandshakeFilterTypeDef](./type_defs.md#handshakefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListHandshakesForOrganizationResponsePaginatorTypeDef](./type_defs.md#listhandshakesfororganizationresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListHandshakesForOrganizationRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHandshakesForOrganizationRequestPaginateTypeDef](./type_defs.md#listhandshakesfororganizationrequestpaginatetypedef) 
## ListOrganizationalUnitsForParentPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_organizational_units_for_parent")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListOrganizationalUnitsForParent.html#Organizations.Paginator.ListOrganizationalUnitsForParent)

```python
# ListOrganizationalUnitsForParentPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListOrganizationalUnitsForParentPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListOrganizationalUnitsForParentPaginator = client.get_paginator("list_organizational_units_for_parent")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrganizationalUnitsForParentResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListOrganizationalUnitsForParentPaginator](./paginators.md#listorganizationalunitsforparentpaginator)
3. item: [:material-code-braces: ListOrganizationalUnitsForParentResponseTypeDef](./type_defs.md#listorganizationalunitsforparentresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOrganizationalUnitsForParentPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ParentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListOrganizationalUnitsForParentResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOrganizationalUnitsForParentResponseTypeDef](./type_defs.md#listorganizationalunitsforparentresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOrganizationalUnitsForParentRequestPaginateTypeDef = {  # (1)
    "ParentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationalUnitsForParentRequestPaginateTypeDef](./type_defs.md#listorganizationalunitsforparentrequestpaginatetypedef) 
## ListParentsPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_parents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListParents.html#Organizations.Paginator.ListParents)

```python
# ListParentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListParentsPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListParentsPaginator = client.get_paginator("list_parents")  # (2)
    async for item in paginator.paginate(...):
        item: ListParentsResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListParentsPaginator](./paginators.md#listparentspaginator)
3. item: [:material-code-braces: ListParentsResponseTypeDef](./type_defs.md#listparentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListParentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChildId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListParentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListParentsResponseTypeDef](./type_defs.md#listparentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListParentsRequestPaginateTypeDef = {  # (1)
    "ChildId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListParentsRequestPaginateTypeDef](./type_defs.md#listparentsrequestpaginatetypedef) 
## ListPoliciesForTargetPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_policies_for_target")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListPoliciesForTarget.html#Organizations.Paginator.ListPoliciesForTarget)

```python
# ListPoliciesForTargetPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListPoliciesForTargetPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListPoliciesForTargetPaginator = client.get_paginator("list_policies_for_target")  # (2)
    async for item in paginator.paginate(...):
        item: ListPoliciesForTargetResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListPoliciesForTargetPaginator](./paginators.md#listpoliciesfortargetpaginator)
3. item: [:material-code-braces: ListPoliciesForTargetResponseTypeDef](./type_defs.md#listpoliciesfortargetresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPoliciesForTargetPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TargetId: str,
    Filter: PolicyTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListPoliciesForTargetResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPoliciesForTargetResponseTypeDef](./type_defs.md#listpoliciesfortargetresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPoliciesForTargetRequestPaginateTypeDef = {  # (1)
    "TargetId": ...,
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoliciesForTargetRequestPaginateTypeDef](./type_defs.md#listpoliciesfortargetrequestpaginatetypedef) 
## ListPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListPolicies.html#Organizations.Paginator.ListPolicies)

```python
# ListPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListPoliciesPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListPoliciesPaginator = client.get_paginator("list_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
3. item: [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: PolicyTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListPoliciesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPoliciesRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoliciesRequestPaginateTypeDef](./type_defs.md#listpoliciesrequestpaginatetypedef) 
## ListRootsPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_roots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListRoots.html#Organizations.Paginator.ListRoots)

```python
# ListRootsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListRootsPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListRootsPaginator = client.get_paginator("list_roots")  # (2)
    async for item in paginator.paginate(...):
        item: ListRootsResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListRootsPaginator](./paginators.md#listrootspaginator)
3. item: [:material-code-braces: ListRootsResponseTypeDef](./type_defs.md#listrootsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRootsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRootsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRootsResponseTypeDef](./type_defs.md#listrootsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRootsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRootsRequestPaginateTypeDef](./type_defs.md#listrootsrequestpaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListTagsForResource.html#Organizations.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestPaginateTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef) 
## ListTargetsForPolicyPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_targets_for_policy")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListTargetsForPolicy.html#Organizations.Paginator.ListTargetsForPolicy)

```python
# ListTargetsForPolicyPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListTargetsForPolicyPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListTargetsForPolicyPaginator = client.get_paginator("list_targets_for_policy")  # (2)
    async for item in paginator.paginate(...):
        item: ListTargetsForPolicyResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListTargetsForPolicyPaginator](./paginators.md#listtargetsforpolicypaginator)
3. item: [:material-code-braces: ListTargetsForPolicyResponseTypeDef](./type_defs.md#listtargetsforpolicyresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTargetsForPolicyPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PolicyId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTargetsForPolicyResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTargetsForPolicyResponseTypeDef](./type_defs.md#listtargetsforpolicyresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTargetsForPolicyRequestPaginateTypeDef = {  # (1)
    "PolicyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTargetsForPolicyRequestPaginateTypeDef](./type_defs.md#listtargetsforpolicyrequestpaginatetypedef) 
