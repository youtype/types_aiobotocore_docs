# Paginators

> [Index](../README.md) > [IAM](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
    type annotations stubs module [types-aiobotocore-iam](https://pypi.org/project/types-aiobotocore-iam/).

## GetAccountAuthorizationDetailsPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("get_account_authorization_details")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetAccountAuthorizationDetails)

```python
# GetAccountAuthorizationDetailsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import GetAccountAuthorizationDetailsPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: GetAccountAuthorizationDetailsPaginator = client.get_paginator("get_account_authorization_details")  # (2)
    async for item in paginator.paginate(...):
        item: GetAccountAuthorizationDetailsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [GetAccountAuthorizationDetailsPaginator](./paginators.md#getaccountauthorizationdetailspaginator)
3. item: [:material-code-braces: GetAccountAuthorizationDetailsResponseTypeDef](./type_defs.md#getaccountauthorizationdetailsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetAccountAuthorizationDetailsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: Sequence[EntityTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetAccountAuthorizationDetailsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetAccountAuthorizationDetailsResponseTypeDef](./type_defs.md#getaccountauthorizationdetailsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef](./type_defs.md#getaccountauthorizationdetailsrequestgetaccountauthorizationdetailspaginatetypedef) 
## GetGroupPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("get_group")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup)

```python
# GetGroupPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import GetGroupPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: GetGroupPaginator = client.get_paginator("get_group")  # (2)
    async for item in paginator.paginate(...):
        item: GetGroupResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [GetGroupPaginator](./paginators.md#getgrouppaginator)
3. item: [:material-code-braces: GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetGroupPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GroupName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetGroupResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetGroupRequestGetGroupPaginateTypeDef = {  # (1)
    "GroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetGroupRequestGetGroupPaginateTypeDef](./type_defs.md#getgrouprequestgetgrouppaginatetypedef) 
## ListAccessKeysPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_access_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys)

```python
# ListAccessKeysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListAccessKeysPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListAccessKeysPaginator = client.get_paginator("list_access_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListAccessKeysPaginator](./paginators.md#listaccesskeyspaginator)
3. item: [:material-code-braces: ListAccessKeysResponseTypeDef](./type_defs.md#listaccesskeysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccessKeysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccessKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccessKeysResponseTypeDef](./type_defs.md#listaccesskeysresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccessKeysRequestListAccessKeysPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessKeysRequestListAccessKeysPaginateTypeDef](./type_defs.md#listaccesskeysrequestlistaccesskeyspaginatetypedef) 
## ListAccountAliasesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_account_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases)

```python
# ListAccountAliasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListAccountAliasesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListAccountAliasesPaginator = client.get_paginator("list_account_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountAliasesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListAccountAliasesPaginator](./paginators.md#listaccountaliasespaginator)
3. item: [:material-code-braces: ListAccountAliasesResponseTypeDef](./type_defs.md#listaccountaliasesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccountAliasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccountAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccountAliasesResponseTypeDef](./type_defs.md#listaccountaliasesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountAliasesRequestListAccountAliasesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountAliasesRequestListAccountAliasesPaginateTypeDef](./type_defs.md#listaccountaliasesrequestlistaccountaliasespaginatetypedef) 
## ListAttachedGroupPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_attached_group_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedGroupPolicies)

```python
# ListAttachedGroupPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListAttachedGroupPoliciesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListAttachedGroupPoliciesPaginator = client.get_paginator("list_attached_group_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttachedGroupPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListAttachedGroupPoliciesPaginator](./paginators.md#listattachedgrouppoliciespaginator)
3. item: [:material-code-braces: ListAttachedGroupPoliciesResponseTypeDef](./type_defs.md#listattachedgrouppoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAttachedGroupPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GroupName: str,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAttachedGroupPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAttachedGroupPoliciesResponseTypeDef](./type_defs.md#listattachedgrouppoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef = {  # (1)
    "GroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef](./type_defs.md#listattachedgrouppoliciesrequestlistattachedgrouppoliciespaginatetypedef) 
## ListAttachedRolePoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_attached_role_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedRolePolicies)

```python
# ListAttachedRolePoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListAttachedRolePoliciesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListAttachedRolePoliciesPaginator = client.get_paginator("list_attached_role_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttachedRolePoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListAttachedRolePoliciesPaginator](./paginators.md#listattachedrolepoliciespaginator)
3. item: [:material-code-braces: ListAttachedRolePoliciesResponseTypeDef](./type_defs.md#listattachedrolepoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAttachedRolePoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RoleName: str,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAttachedRolePoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAttachedRolePoliciesResponseTypeDef](./type_defs.md#listattachedrolepoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef = {  # (1)
    "RoleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef](./type_defs.md#listattachedrolepoliciesrequestlistattachedrolepoliciespaginatetypedef) 
## ListAttachedUserPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_attached_user_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedUserPolicies)

```python
# ListAttachedUserPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListAttachedUserPoliciesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListAttachedUserPoliciesPaginator = client.get_paginator("list_attached_user_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttachedUserPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListAttachedUserPoliciesPaginator](./paginators.md#listattacheduserpoliciespaginator)
3. item: [:material-code-braces: ListAttachedUserPoliciesResponseTypeDef](./type_defs.md#listattacheduserpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAttachedUserPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserName: str,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAttachedUserPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAttachedUserPoliciesResponseTypeDef](./type_defs.md#listattacheduserpoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef](./type_defs.md#listattacheduserpoliciesrequestlistattacheduserpoliciespaginatetypedef) 
## ListEntitiesForPolicyPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_entities_for_policy")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListEntitiesForPolicy)

```python
# ListEntitiesForPolicyPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListEntitiesForPolicyPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListEntitiesForPolicyPaginator = client.get_paginator("list_entities_for_policy")  # (2)
    async for item in paginator.paginate(...):
        item: ListEntitiesForPolicyResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListEntitiesForPolicyPaginator](./paginators.md#listentitiesforpolicypaginator)
3. item: [:material-code-braces: ListEntitiesForPolicyResponseTypeDef](./type_defs.md#listentitiesforpolicyresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEntitiesForPolicyPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PolicyArn: str,
    EntityFilter: EntityTypeType = ...,  # (1)
    PathPrefix: str = ...,
    PolicyUsageFilter: PolicyUsageTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListEntitiesForPolicyResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-brackets: PolicyUsageTypeType](./literals.md#policyusagetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListEntitiesForPolicyResponseTypeDef](./type_defs.md#listentitiesforpolicyresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef](./type_defs.md#listentitiesforpolicyrequestlistentitiesforpolicypaginatetypedef) 
## ListGroupPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_group_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies)

```python
# ListGroupPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListGroupPoliciesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListGroupPoliciesPaginator = client.get_paginator("list_group_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListGroupPoliciesPaginator](./paginators.md#listgrouppoliciespaginator)
3. item: [:material-code-braces: ListGroupPoliciesResponseTypeDef](./type_defs.md#listgrouppoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GroupName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGroupPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupPoliciesResponseTypeDef](./type_defs.md#listgrouppoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = {  # (1)
    "GroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef](./type_defs.md#listgrouppoliciesrequestlistgrouppoliciespaginatetypedef) 
## ListGroupsPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups)

```python
# ListGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListGroupsPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListGroupsPaginator](./paginators.md#listgroupspaginator)
3. item: [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupsRequestListGroupsPaginateTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestListGroupsPaginateTypeDef](./type_defs.md#listgroupsrequestlistgroupspaginatetypedef) 
## ListGroupsForUserPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_groups_for_user")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser)

```python
# ListGroupsForUserPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListGroupsForUserPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListGroupsForUserPaginator = client.get_paginator("list_groups_for_user")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsForUserResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListGroupsForUserPaginator](./paginators.md#listgroupsforuserpaginator)
3. item: [:material-code-braces: ListGroupsForUserResponseTypeDef](./type_defs.md#listgroupsforuserresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsForUserPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGroupsForUserResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupsForUserResponseTypeDef](./type_defs.md#listgroupsforuserresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupsForUserRequestListGroupsForUserPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsForUserRequestListGroupsForUserPaginateTypeDef](./type_defs.md#listgroupsforuserrequestlistgroupsforuserpaginatetypedef) 
## ListInstanceProfileTagsPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_instance_profile_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfileTags)

```python
# ListInstanceProfileTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListInstanceProfileTagsPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListInstanceProfileTagsPaginator = client.get_paginator("list_instance_profile_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceProfileTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListInstanceProfileTagsPaginator](./paginators.md#listinstanceprofiletagspaginator)
3. item: [:material-code-braces: ListInstanceProfileTagsResponseTypeDef](./type_defs.md#listinstanceprofiletagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInstanceProfileTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceProfileName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInstanceProfileTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstanceProfileTagsResponseTypeDef](./type_defs.md#listinstanceprofiletagsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef = {  # (1)
    "InstanceProfileName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef](./type_defs.md#listinstanceprofiletagsrequestlistinstanceprofiletagspaginatetypedef) 
## ListInstanceProfilesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_instance_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles)

```python
# ListInstanceProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListInstanceProfilesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListInstanceProfilesPaginator = client.get_paginator("list_instance_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListInstanceProfilesPaginator](./paginators.md#listinstanceprofilespaginator)
3. item: [:material-code-braces: ListInstanceProfilesResponseTypeDef](./type_defs.md#listinstanceprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInstanceProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInstanceProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstanceProfilesResponseTypeDef](./type_defs.md#listinstanceprofilesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef](./type_defs.md#listinstanceprofilesrequestlistinstanceprofilespaginatetypedef) 
## ListInstanceProfilesForRolePaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_instance_profiles_for_role")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole)

```python
# ListInstanceProfilesForRolePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListInstanceProfilesForRolePaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListInstanceProfilesForRolePaginator = client.get_paginator("list_instance_profiles_for_role")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceProfilesForRoleResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListInstanceProfilesForRolePaginator](./paginators.md#listinstanceprofilesforrolepaginator)
3. item: [:material-code-braces: ListInstanceProfilesForRoleResponseTypeDef](./type_defs.md#listinstanceprofilesforroleresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInstanceProfilesForRolePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RoleName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInstanceProfilesForRoleResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstanceProfilesForRoleResponseTypeDef](./type_defs.md#listinstanceprofilesforroleresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef = {  # (1)
    "RoleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef](./type_defs.md#listinstanceprofilesforrolerequestlistinstanceprofilesforrolepaginatetypedef) 
## ListMFADeviceTagsPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_mfa_device_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADeviceTags)

```python
# ListMFADeviceTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListMFADeviceTagsPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListMFADeviceTagsPaginator = client.get_paginator("list_mfa_device_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListMFADeviceTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListMFADeviceTagsPaginator](./paginators.md#listmfadevicetagspaginator)
3. item: [:material-code-braces: ListMFADeviceTagsResponseTypeDef](./type_defs.md#listmfadevicetagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMFADeviceTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SerialNumber: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMFADeviceTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMFADeviceTagsResponseTypeDef](./type_defs.md#listmfadevicetagsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef = {  # (1)
    "SerialNumber": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef](./type_defs.md#listmfadevicetagsrequestlistmfadevicetagspaginatetypedef) 
## ListMFADevicesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_mfa_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices)

```python
# ListMFADevicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListMFADevicesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListMFADevicesPaginator = client.get_paginator("list_mfa_devices")  # (2)
    async for item in paginator.paginate(...):
        item: ListMFADevicesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListMFADevicesPaginator](./paginators.md#listmfadevicespaginator)
3. item: [:material-code-braces: ListMFADevicesResponseTypeDef](./type_defs.md#listmfadevicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMFADevicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMFADevicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMFADevicesResponseTypeDef](./type_defs.md#listmfadevicesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMFADevicesRequestListMFADevicesPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMFADevicesRequestListMFADevicesPaginateTypeDef](./type_defs.md#listmfadevicesrequestlistmfadevicespaginatetypedef) 
## ListOpenIDConnectProviderTagsPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_open_id_connect_provider_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListOpenIDConnectProviderTags)

```python
# ListOpenIDConnectProviderTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListOpenIDConnectProviderTagsPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListOpenIDConnectProviderTagsPaginator = client.get_paginator("list_open_id_connect_provider_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListOpenIDConnectProviderTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListOpenIDConnectProviderTagsPaginator](./paginators.md#listopenidconnectprovidertagspaginator)
3. item: [:material-code-braces: ListOpenIDConnectProviderTagsResponseTypeDef](./type_defs.md#listopenidconnectprovidertagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOpenIDConnectProviderTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OpenIDConnectProviderArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOpenIDConnectProviderTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOpenIDConnectProviderTagsResponseTypeDef](./type_defs.md#listopenidconnectprovidertagsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef = {  # (1)
    "OpenIDConnectProviderArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef](./type_defs.md#listopenidconnectprovidertagsrequestlistopenidconnectprovidertagspaginatetypedef) 
## ListPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicies)

```python
# ListPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListPoliciesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListPoliciesPaginator = client.get_paginator("list_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
3. item: [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Scope: policyScopeTypeType = ...,  # (1)
    OnlyAttached: bool = ...,
    PathPrefix: str = ...,
    PolicyUsageFilter: PolicyUsageTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListPoliciesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: policyScopeTypeType](./literals.md#policyscopetypetype) 
2. See [:material-code-brackets: PolicyUsageTypeType](./literals.md#policyusagetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPoliciesRequestListPoliciesPaginateTypeDef = {  # (1)
    "Scope": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoliciesRequestListPoliciesPaginateTypeDef](./type_defs.md#listpoliciesrequestlistpoliciespaginatetypedef) 
## ListPolicyTagsPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_policy_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyTags)

```python
# ListPolicyTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListPolicyTagsPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListPolicyTagsPaginator = client.get_paginator("list_policy_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListPolicyTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListPolicyTagsPaginator](./paginators.md#listpolicytagspaginator)
3. item: [:material-code-braces: ListPolicyTagsResponseTypeDef](./type_defs.md#listpolicytagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPolicyTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PolicyArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPolicyTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPolicyTagsResponseTypeDef](./type_defs.md#listpolicytagsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPolicyTagsRequestListPolicyTagsPaginateTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPolicyTagsRequestListPolicyTagsPaginateTypeDef](./type_defs.md#listpolicytagsrequestlistpolicytagspaginatetypedef) 
## ListPolicyVersionsPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_policy_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions)

```python
# ListPolicyVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListPolicyVersionsPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListPolicyVersionsPaginator = client.get_paginator("list_policy_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPolicyVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListPolicyVersionsPaginator](./paginators.md#listpolicyversionspaginator)
3. item: [:material-code-braces: ListPolicyVersionsResponseTypeDef](./type_defs.md#listpolicyversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPolicyVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PolicyArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPolicyVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPolicyVersionsResponseTypeDef](./type_defs.md#listpolicyversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef](./type_defs.md#listpolicyversionsrequestlistpolicyversionspaginatetypedef) 
## ListRolePoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_role_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies)

```python
# ListRolePoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListRolePoliciesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListRolePoliciesPaginator = client.get_paginator("list_role_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListRolePoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListRolePoliciesPaginator](./paginators.md#listrolepoliciespaginator)
3. item: [:material-code-braces: ListRolePoliciesResponseTypeDef](./type_defs.md#listrolepoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRolePoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RoleName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRolePoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRolePoliciesResponseTypeDef](./type_defs.md#listrolepoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRolePoliciesRequestListRolePoliciesPaginateTypeDef = {  # (1)
    "RoleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRolePoliciesRequestListRolePoliciesPaginateTypeDef](./type_defs.md#listrolepoliciesrequestlistrolepoliciespaginatetypedef) 
## ListRoleTagsPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_role_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoleTags)

```python
# ListRoleTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListRoleTagsPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListRoleTagsPaginator = client.get_paginator("list_role_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoleTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListRoleTagsPaginator](./paginators.md#listroletagspaginator)
3. item: [:material-code-braces: ListRoleTagsResponseTypeDef](./type_defs.md#listroletagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRoleTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RoleName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRoleTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRoleTagsResponseTypeDef](./type_defs.md#listroletagsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRoleTagsRequestListRoleTagsPaginateTypeDef = {  # (1)
    "RoleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoleTagsRequestListRoleTagsPaginateTypeDef](./type_defs.md#listroletagsrequestlistroletagspaginatetypedef) 
## ListRolesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_roles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles)

```python
# ListRolesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListRolesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListRolesPaginator = client.get_paginator("list_roles")  # (2)
    async for item in paginator.paginate(...):
        item: ListRolesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListRolesPaginator](./paginators.md#listrolespaginator)
3. item: [:material-code-braces: ListRolesResponseTypeDef](./type_defs.md#listrolesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRolesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRolesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRolesResponseTypeDef](./type_defs.md#listrolesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRolesRequestListRolesPaginateTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRolesRequestListRolesPaginateTypeDef](./type_defs.md#listrolesrequestlistrolespaginatetypedef) 
## ListSAMLProviderTagsPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_saml_provider_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSAMLProviderTags)

```python
# ListSAMLProviderTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListSAMLProviderTagsPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListSAMLProviderTagsPaginator = client.get_paginator("list_saml_provider_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListSAMLProviderTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListSAMLProviderTagsPaginator](./paginators.md#listsamlprovidertagspaginator)
3. item: [:material-code-braces: ListSAMLProviderTagsResponseTypeDef](./type_defs.md#listsamlprovidertagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSAMLProviderTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SAMLProviderArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSAMLProviderTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSAMLProviderTagsResponseTypeDef](./type_defs.md#listsamlprovidertagsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef = {  # (1)
    "SAMLProviderArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef](./type_defs.md#listsamlprovidertagsrequestlistsamlprovidertagspaginatetypedef) 
## ListSSHPublicKeysPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_ssh_public_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys)

```python
# ListSSHPublicKeysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListSSHPublicKeysPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListSSHPublicKeysPaginator = client.get_paginator("list_ssh_public_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListSSHPublicKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListSSHPublicKeysPaginator](./paginators.md#listsshpublickeyspaginator)
3. item: [:material-code-braces: ListSSHPublicKeysResponseTypeDef](./type_defs.md#listsshpublickeysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSSHPublicKeysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSSHPublicKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSSHPublicKeysResponseTypeDef](./type_defs.md#listsshpublickeysresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef](./type_defs.md#listsshpublickeysrequestlistsshpublickeyspaginatetypedef) 
## ListServerCertificateTagsPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_server_certificate_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificateTags)

```python
# ListServerCertificateTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListServerCertificateTagsPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListServerCertificateTagsPaginator = client.get_paginator("list_server_certificate_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListServerCertificateTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListServerCertificateTagsPaginator](./paginators.md#listservercertificatetagspaginator)
3. item: [:material-code-braces: ListServerCertificateTagsResponseTypeDef](./type_defs.md#listservercertificatetagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListServerCertificateTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServerCertificateName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListServerCertificateTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListServerCertificateTagsResponseTypeDef](./type_defs.md#listservercertificatetagsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef = {  # (1)
    "ServerCertificateName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef](./type_defs.md#listservercertificatetagsrequestlistservercertificatetagspaginatetypedef) 
## ListServerCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_server_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates)

```python
# ListServerCertificatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListServerCertificatesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListServerCertificatesPaginator = client.get_paginator("list_server_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: ListServerCertificatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListServerCertificatesPaginator](./paginators.md#listservercertificatespaginator)
3. item: [:material-code-braces: ListServerCertificatesResponseTypeDef](./type_defs.md#listservercertificatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListServerCertificatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListServerCertificatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListServerCertificatesResponseTypeDef](./type_defs.md#listservercertificatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListServerCertificatesRequestListServerCertificatesPaginateTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServerCertificatesRequestListServerCertificatesPaginateTypeDef](./type_defs.md#listservercertificatesrequestlistservercertificatespaginatetypedef) 
## ListSigningCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_signing_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates)

```python
# ListSigningCertificatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListSigningCertificatesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListSigningCertificatesPaginator = client.get_paginator("list_signing_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: ListSigningCertificatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListSigningCertificatesPaginator](./paginators.md#listsigningcertificatespaginator)
3. item: [:material-code-braces: ListSigningCertificatesResponseTypeDef](./type_defs.md#listsigningcertificatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSigningCertificatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSigningCertificatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSigningCertificatesResponseTypeDef](./type_defs.md#listsigningcertificatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef](./type_defs.md#listsigningcertificatesrequestlistsigningcertificatespaginatetypedef) 
## ListUserPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_user_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies)

```python
# ListUserPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListUserPoliciesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListUserPoliciesPaginator = client.get_paginator("list_user_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListUserPoliciesPaginator](./paginators.md#listuserpoliciespaginator)
3. item: [:material-code-braces: ListUserPoliciesResponseTypeDef](./type_defs.md#listuserpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUserPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUserPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUserPoliciesResponseTypeDef](./type_defs.md#listuserpoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUserPoliciesRequestListUserPoliciesPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserPoliciesRequestListUserPoliciesPaginateTypeDef](./type_defs.md#listuserpoliciesrequestlistuserpoliciespaginatetypedef) 
## ListUserTagsPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_user_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags)

```python
# ListUserTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListUserTagsPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListUserTagsPaginator = client.get_paginator("list_user_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListUserTagsPaginator](./paginators.md#listusertagspaginator)
3. item: [:material-code-braces: ListUserTagsResponseTypeDef](./type_defs.md#listusertagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUserTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUserTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUserTagsResponseTypeDef](./type_defs.md#listusertagsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUserTagsRequestListUserTagsPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserTagsRequestListUserTagsPaginateTypeDef](./type_defs.md#listusertagsrequestlistusertagspaginatetypedef) 
## ListUsersPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers)

```python
# ListUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUsersRequestListUsersPaginateTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestListUsersPaginateTypeDef](./type_defs.md#listusersrequestlistuserspaginatetypedef) 
## ListVirtualMFADevicesPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("list_virtual_mfa_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListVirtualMFADevices)

```python
# ListVirtualMFADevicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import ListVirtualMFADevicesPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: ListVirtualMFADevicesPaginator = client.get_paginator("list_virtual_mfa_devices")  # (2)
    async for item in paginator.paginate(...):
        item: ListVirtualMFADevicesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListVirtualMFADevicesPaginator](./paginators.md#listvirtualmfadevicespaginator)
3. item: [:material-code-braces: ListVirtualMFADevicesResponseTypeDef](./type_defs.md#listvirtualmfadevicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListVirtualMFADevicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AssignmentStatus: assignmentStatusTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListVirtualMFADevicesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: assignmentStatusTypeType](./literals.md#assignmentstatustypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListVirtualMFADevicesResponseTypeDef](./type_defs.md#listvirtualmfadevicesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef = {  # (1)
    "AssignmentStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef](./type_defs.md#listvirtualmfadevicesrequestlistvirtualmfadevicespaginatetypedef) 
## SimulateCustomPolicyPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("simulate_custom_policy")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulateCustomPolicy)

```python
# SimulateCustomPolicyPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import SimulateCustomPolicyPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: SimulateCustomPolicyPaginator = client.get_paginator("simulate_custom_policy")  # (2)
    async for item in paginator.paginate(...):
        item: SimulatePolicyResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [SimulateCustomPolicyPaginator](./paginators.md#simulatecustompolicypaginator)
3. item: [:material-code-braces: SimulatePolicyResponseTypeDef](./type_defs.md#simulatepolicyresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SimulateCustomPolicyPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PolicyInputList: Sequence[str],
    ActionNames: Sequence[str],
    PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
    ResourceArns: Sequence[str] = ...,
    ResourcePolicy: str = ...,
    ResourceOwner: str = ...,
    CallerArn: str = ...,
    ContextEntries: Sequence[ContextEntryTypeDef] = ...,  # (1)
    ResourceHandlingOption: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SimulatePolicyResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ContextEntryTypeDef](./type_defs.md#contextentrytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SimulatePolicyResponseTypeDef](./type_defs.md#simulatepolicyresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef = {  # (1)
    "PolicyInputList": ...,
    "ActionNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef](./type_defs.md#simulatecustompolicyrequestsimulatecustompolicypaginatetypedef) 
## SimulatePrincipalPolicyPaginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator("simulate_principal_policy")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulatePrincipalPolicy)

```python
# SimulatePrincipalPolicyPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.paginator import SimulatePrincipalPolicyPaginator

session = get_session()
async with session.create_client("iam") as client:  # (1)
    paginator: SimulatePrincipalPolicyPaginator = client.get_paginator("simulate_principal_policy")  # (2)
    async for item in paginator.paginate(...):
        item: SimulatePolicyResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [SimulatePrincipalPolicyPaginator](./paginators.md#simulateprincipalpolicypaginator)
3. item: [:material-code-braces: SimulatePolicyResponseTypeDef](./type_defs.md#simulatepolicyresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SimulatePrincipalPolicyPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PolicySourceArn: str,
    ActionNames: Sequence[str],
    PolicyInputList: Sequence[str] = ...,
    PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
    ResourceArns: Sequence[str] = ...,
    ResourcePolicy: str = ...,
    ResourceOwner: str = ...,
    CallerArn: str = ...,
    ContextEntries: Sequence[ContextEntryTypeDef] = ...,  # (1)
    ResourceHandlingOption: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SimulatePolicyResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ContextEntryTypeDef](./type_defs.md#contextentrytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SimulatePolicyResponseTypeDef](./type_defs.md#simulatepolicyresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef = {  # (1)
    "PolicySourceArn": ...,
    "ActionNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef](./type_defs.md#simulateprincipalpolicyrequestsimulateprincipalpolicypaginatetypedef) 
