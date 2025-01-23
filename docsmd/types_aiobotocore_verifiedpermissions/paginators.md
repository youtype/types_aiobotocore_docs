# Paginators

> [Index](../README.md) > [VerifiedPermissions](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [VerifiedPermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#verifiedpermissions)
    type annotations stubs module [types-aiobotocore-verifiedpermissions](https://pypi.org/project/types-aiobotocore-verifiedpermissions/).

## ListIdentitySourcesPaginator

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").get_paginator("list_identity_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/paginator/ListIdentitySources.html#VerifiedPermissions.Paginator.ListIdentitySources)

```python
# ListIdentitySourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_verifiedpermissions.paginator import ListIdentitySourcesPaginator

session = get_session()
async with session.create_client("verifiedpermissions") as client:  # (1)
    paginator: ListIdentitySourcesPaginator = client.get_paginator("list_identity_sources")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdentitySourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [VerifiedPermissionsClient](./client.md)
2. paginator: [ListIdentitySourcesPaginator](./paginators.md#listidentitysourcespaginator)
3. item: [:material-code-braces: ListIdentitySourcesOutputTypeDef](./type_defs.md#listidentitysourcesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListIdentitySourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    policyStoreId: str,
    filters: Sequence[IdentitySourceFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListIdentitySourcesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: IdentitySourceFilterTypeDef](./type_defs.md#identitysourcefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListIdentitySourcesOutputTypeDef](./type_defs.md#listidentitysourcesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIdentitySourcesInputPaginateTypeDef = {  # (1)
    "policyStoreId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdentitySourcesInputPaginateTypeDef](./type_defs.md#listidentitysourcesinputpaginatetypedef) 
## ListPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").get_paginator("list_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/paginator/ListPolicies.html#VerifiedPermissions.Paginator.ListPolicies)

```python
# ListPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_verifiedpermissions.paginator import ListPoliciesPaginator

session = get_session()
async with session.create_client("verifiedpermissions") as client:  # (1)
    paginator: ListPoliciesPaginator = client.get_paginator("list_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListPoliciesOutputTypeDef
        print(item)  # (3)
```

1. client: [VerifiedPermissionsClient](./client.md)
2. paginator: [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
3. item: [:material-code-braces: ListPoliciesOutputTypeDef](./type_defs.md#listpoliciesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    policyStoreId: str,
    filter: PolicyFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListPoliciesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: PolicyFilterTypeDef](./type_defs.md#policyfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPoliciesOutputTypeDef](./type_defs.md#listpoliciesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPoliciesInputPaginateTypeDef = {  # (1)
    "policyStoreId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoliciesInputPaginateTypeDef](./type_defs.md#listpoliciesinputpaginatetypedef) 
## ListPolicyStoresPaginator

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").get_paginator("list_policy_stores")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/paginator/ListPolicyStores.html#VerifiedPermissions.Paginator.ListPolicyStores)

```python
# ListPolicyStoresPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_verifiedpermissions.paginator import ListPolicyStoresPaginator

session = get_session()
async with session.create_client("verifiedpermissions") as client:  # (1)
    paginator: ListPolicyStoresPaginator = client.get_paginator("list_policy_stores")  # (2)
    async for item in paginator.paginate(...):
        item: ListPolicyStoresOutputTypeDef
        print(item)  # (3)
```

1. client: [VerifiedPermissionsClient](./client.md)
2. paginator: [ListPolicyStoresPaginator](./paginators.md#listpolicystorespaginator)
3. item: [:material-code-braces: ListPolicyStoresOutputTypeDef](./type_defs.md#listpolicystoresoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListPolicyStoresPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPolicyStoresOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPolicyStoresOutputTypeDef](./type_defs.md#listpolicystoresoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPolicyStoresInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPolicyStoresInputPaginateTypeDef](./type_defs.md#listpolicystoresinputpaginatetypedef) 
## ListPolicyTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").get_paginator("list_policy_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/paginator/ListPolicyTemplates.html#VerifiedPermissions.Paginator.ListPolicyTemplates)

```python
# ListPolicyTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_verifiedpermissions.paginator import ListPolicyTemplatesPaginator

session = get_session()
async with session.create_client("verifiedpermissions") as client:  # (1)
    paginator: ListPolicyTemplatesPaginator = client.get_paginator("list_policy_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListPolicyTemplatesOutputTypeDef
        print(item)  # (3)
```

1. client: [VerifiedPermissionsClient](./client.md)
2. paginator: [ListPolicyTemplatesPaginator](./paginators.md#listpolicytemplatespaginator)
3. item: [:material-code-braces: ListPolicyTemplatesOutputTypeDef](./type_defs.md#listpolicytemplatesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListPolicyTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    policyStoreId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPolicyTemplatesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPolicyTemplatesOutputTypeDef](./type_defs.md#listpolicytemplatesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPolicyTemplatesInputPaginateTypeDef = {  # (1)
    "policyStoreId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPolicyTemplatesInputPaginateTypeDef](./type_defs.md#listpolicytemplatesinputpaginatetypedef) 
