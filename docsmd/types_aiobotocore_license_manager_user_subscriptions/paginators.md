# Paginators

> [Index](../README.md) > [LicenseManagerUserSubscriptions](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [LicenseManagerUserSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#licensemanagerusersubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-user-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions/).

## ListIdentityProvidersPaginator

Type annotations and code completion for `#!python session.create_client("license-manager-user-subscriptions").get_paginator("list_identity_providers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions/paginator/ListIdentityProviders.html#LicenseManagerUserSubscriptions.Paginator.ListIdentityProviders)

```python
# ListIdentityProvidersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager_user_subscriptions.paginator import ListIdentityProvidersPaginator

session = get_session()
async with session.create_client("license-manager-user-subscriptions") as client:  # (1)
    paginator: ListIdentityProvidersPaginator = client.get_paginator("list_identity_providers")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdentityProvidersResponseTypeDef
        print(item)  # (3)
```

1. client: [LicenseManagerUserSubscriptionsClient](./client.md)
2. paginator: [ListIdentityProvidersPaginator](./paginators.md#listidentityproviderspaginator)
3. item: [:material-code-braces: ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIdentityProvidersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListIdentityProvidersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIdentityProvidersRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdentityProvidersRequestPaginateTypeDef](./type_defs.md#listidentityprovidersrequestpaginatetypedef) 
## ListInstancesPaginator

Type annotations and code completion for `#!python session.create_client("license-manager-user-subscriptions").get_paginator("list_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions/paginator/ListInstances.html#LicenseManagerUserSubscriptions.Paginator.ListInstances)

```python
# ListInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager_user_subscriptions.paginator import ListInstancesPaginator

session = get_session()
async with session.create_client("license-manager-user-subscriptions") as client:  # (1)
    paginator: ListInstancesPaginator = client.get_paginator("list_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [LicenseManagerUserSubscriptionsClient](./client.md)
2. paginator: [ListInstancesPaginator](./paginators.md#listinstancespaginator)
3. item: [:material-code-braces: ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListInstancesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInstancesRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstancesRequestPaginateTypeDef](./type_defs.md#listinstancesrequestpaginatetypedef) 
## ListLicenseServerEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("license-manager-user-subscriptions").get_paginator("list_license_server_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions/paginator/ListLicenseServerEndpoints.html#LicenseManagerUserSubscriptions.Paginator.ListLicenseServerEndpoints)

```python
# ListLicenseServerEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager_user_subscriptions.paginator import ListLicenseServerEndpointsPaginator

session = get_session()
async with session.create_client("license-manager-user-subscriptions") as client:  # (1)
    paginator: ListLicenseServerEndpointsPaginator = client.get_paginator("list_license_server_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListLicenseServerEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [LicenseManagerUserSubscriptionsClient](./client.md)
2. paginator: [ListLicenseServerEndpointsPaginator](./paginators.md#listlicenseserverendpointspaginator)
3. item: [:material-code-braces: ListLicenseServerEndpointsResponseTypeDef](./type_defs.md#listlicenseserverendpointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLicenseServerEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListLicenseServerEndpointsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListLicenseServerEndpointsResponseTypeDef](./type_defs.md#listlicenseserverendpointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLicenseServerEndpointsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLicenseServerEndpointsRequestPaginateTypeDef](./type_defs.md#listlicenseserverendpointsrequestpaginatetypedef) 
## ListProductSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("license-manager-user-subscriptions").get_paginator("list_product_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions/paginator/ListProductSubscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListProductSubscriptions)

```python
# ListProductSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager_user_subscriptions.paginator import ListProductSubscriptionsPaginator

session = get_session()
async with session.create_client("license-manager-user-subscriptions") as client:  # (1)
    paginator: ListProductSubscriptionsPaginator = client.get_paginator("list_product_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListProductSubscriptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [LicenseManagerUserSubscriptionsClient](./client.md)
2. paginator: [ListProductSubscriptionsPaginator](./paginators.md#listproductsubscriptionspaginator)
3. item: [:material-code-braces: ListProductSubscriptionsResponseTypeDef](./type_defs.md#listproductsubscriptionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProductSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IdentityProvider: IdentityProviderUnionTypeDef,  # (1)
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    Product: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListProductSubscriptionsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListProductSubscriptionsResponseTypeDef](./type_defs.md#listproductsubscriptionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProductSubscriptionsRequestPaginateTypeDef = {  # (1)
    "IdentityProvider": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProductSubscriptionsRequestPaginateTypeDef](./type_defs.md#listproductsubscriptionsrequestpaginatetypedef) 
## ListUserAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("license-manager-user-subscriptions").get_paginator("list_user_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions/paginator/ListUserAssociations.html#LicenseManagerUserSubscriptions.Paginator.ListUserAssociations)

```python
# ListUserAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager_user_subscriptions.paginator import ListUserAssociationsPaginator

session = get_session()
async with session.create_client("license-manager-user-subscriptions") as client:  # (1)
    paginator: ListUserAssociationsPaginator = client.get_paginator("list_user_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [LicenseManagerUserSubscriptionsClient](./client.md)
2. paginator: [ListUserAssociationsPaginator](./paginators.md#listuserassociationspaginator)
3. item: [:material-code-braces: ListUserAssociationsResponseTypeDef](./type_defs.md#listuserassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUserAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IdentityProvider: IdentityProviderUnionTypeDef,  # (1)
    InstanceId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListUserAssociationsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListUserAssociationsResponseTypeDef](./type_defs.md#listuserassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUserAssociationsRequestPaginateTypeDef = {  # (1)
    "IdentityProvider": ...,
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserAssociationsRequestPaginateTypeDef](./type_defs.md#listuserassociationsrequestpaginatetypedef) 
