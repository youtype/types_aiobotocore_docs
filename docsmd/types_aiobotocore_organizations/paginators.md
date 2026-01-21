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
3. item: `AioPageIterator[ListAWSServiceAccessForOrganizationResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAWSServiceAccessForOrganizationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAWSServiceAccessForOrganizationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAWSServiceAccessForOrganizationResponseTypeDef]`


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
3. item: `AioPageIterator[ListAccountsForParentResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAccountsForParentPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ParentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAccountsForParentResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAccountsForParentResponseTypeDef]`


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
3. item: `AioPageIterator[ListAccountsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAccountsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountsRequestPaginateTypeDef](./type_defs.md#listaccountsrequestpaginatetypedef)
## ListAccountsWithInvalidEffectivePolicyPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_accounts_with_invalid_effective_policy")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListAccountsWithInvalidEffectivePolicy.html#Organizations.Paginator.ListAccountsWithInvalidEffectivePolicy)

```python
# ListAccountsWithInvalidEffectivePolicyPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListAccountsWithInvalidEffectivePolicyPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListAccountsWithInvalidEffectivePolicyPaginator = client.get_paginator("list_accounts_with_invalid_effective_policy")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountsWithInvalidEffectivePolicyResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListAccountsWithInvalidEffectivePolicyPaginator](./paginators.md#listaccountswithinvalideffectivepolicypaginator)
3. item: `AioPageIterator[ListAccountsWithInvalidEffectivePolicyResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAccountsWithInvalidEffectivePolicyPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PolicyType: EffectivePolicyTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAccountsWithInvalidEffectivePolicyResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EffectivePolicyTypeType](./literals.md#effectivepolicytypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAccountsWithInvalidEffectivePolicyResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountsWithInvalidEffectivePolicyRequestPaginateTypeDef = {  # (1)
    "PolicyType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountsWithInvalidEffectivePolicyRequestPaginateTypeDef](./type_defs.md#listaccountswithinvalideffectivepolicyrequestpaginatetypedef)
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
3. item: `AioPageIterator[ListChildrenResponseTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListChildrenResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ChildTypeType](./literals.md#childtypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListChildrenResponseTypeDef]`


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
3. item: `AioPageIterator[ListCreateAccountStatusResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCreateAccountStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    States: Sequence[CreateAccountStateType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListCreateAccountStatusResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[CreateAccountStateType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListCreateAccountStatusResponseTypeDef]`


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
3. item: `AioPageIterator[ListDelegatedAdministratorsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDelegatedAdministratorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServicePrincipal: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDelegatedAdministratorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDelegatedAdministratorsResponseTypeDef]`


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
3. item: `AioPageIterator[ListDelegatedServicesForAccountResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDelegatedServicesForAccountPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDelegatedServicesForAccountResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDelegatedServicesForAccountResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDelegatedServicesForAccountRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDelegatedServicesForAccountRequestPaginateTypeDef](./type_defs.md#listdelegatedservicesforaccountrequestpaginatetypedef)
## ListEffectivePolicyValidationErrorsPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_effective_policy_validation_errors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations/paginator/ListEffectivePolicyValidationErrors.html#Organizations.Paginator.ListEffectivePolicyValidationErrors)

```python
# ListEffectivePolicyValidationErrorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListEffectivePolicyValidationErrorsPaginator

session = get_session()
async with session.create_client("organizations") as client:  # (1)
    paginator: ListEffectivePolicyValidationErrorsPaginator = client.get_paginator("list_effective_policy_validation_errors")  # (2)
    async for item in paginator.paginate(...):
        item: ListEffectivePolicyValidationErrorsResponseTypeDef
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListEffectivePolicyValidationErrorsPaginator](./paginators.md#listeffectivepolicyvalidationerrorspaginator)
3. item: `AioPageIterator[ListEffectivePolicyValidationErrorsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEffectivePolicyValidationErrorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    PolicyType: EffectivePolicyTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListEffectivePolicyValidationErrorsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EffectivePolicyTypeType](./literals.md#effectivepolicytypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListEffectivePolicyValidationErrorsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEffectivePolicyValidationErrorsRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
    "PolicyType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEffectivePolicyValidationErrorsRequestPaginateTypeDef](./type_defs.md#listeffectivepolicyvalidationerrorsrequestpaginatetypedef)
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
3. item: `AioPageIterator[ListHandshakesForAccountResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python ListHandshakesForAccountPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: HandshakeFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListHandshakesForAccountResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: HandshakeFilterTypeDef](./type_defs.md#handshakefiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListHandshakesForAccountResponsePaginatorTypeDef]`


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
3. item: `AioPageIterator[ListHandshakesForOrganizationResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python ListHandshakesForOrganizationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: HandshakeFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListHandshakesForOrganizationResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: HandshakeFilterTypeDef](./type_defs.md#handshakefiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListHandshakesForOrganizationResponsePaginatorTypeDef]`


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
3. item: `AioPageIterator[ListOrganizationalUnitsForParentResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOrganizationalUnitsForParentPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ParentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOrganizationalUnitsForParentResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOrganizationalUnitsForParentResponseTypeDef]`


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
3. item: `AioPageIterator[ListParentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListParentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChildId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListParentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListParentsResponseTypeDef]`


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
3. item: `AioPageIterator[ListPoliciesForTargetResponseTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListPoliciesForTargetResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListPoliciesForTargetResponseTypeDef]`


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
3. item: `AioPageIterator[ListPoliciesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: PolicyTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListPoliciesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListPoliciesResponseTypeDef]`


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
3. item: `AioPageIterator[ListRootsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRootsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRootsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRootsResponseTypeDef]`


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
3. item: `AioPageIterator[ListTagsForResourceResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTagsForResourceResponseTypeDef]`


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
3. item: `AioPageIterator[ListTargetsForPolicyResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTargetsForPolicyPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PolicyId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTargetsForPolicyResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTargetsForPolicyResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTargetsForPolicyRequestPaginateTypeDef = {  # (1)
    "PolicyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTargetsForPolicyRequestPaginateTypeDef](./type_defs.md#listtargetsforpolicyrequestpaginatetypedef)
