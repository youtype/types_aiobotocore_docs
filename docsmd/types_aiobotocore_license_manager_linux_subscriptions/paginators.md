# Paginators

> [Index](../README.md) > [LicenseManagerLinuxSubscriptions](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [LicenseManagerLinuxSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-linux-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-linux-subscriptions/).

## ListLinuxSubscriptionInstancesPaginator

Type annotations and code completion for `#!python session.create_client("license-manager-linux-subscriptions").get_paginator("list_linux_subscription_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Paginator.ListLinuxSubscriptionInstances)

```python
# ListLinuxSubscriptionInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager_linux_subscriptions.paginator import ListLinuxSubscriptionInstancesPaginator

session = get_session()
async with session.create_client("license-manager-linux-subscriptions") as client:  # (1)
    paginator: ListLinuxSubscriptionInstancesPaginator = client.get_paginator("list_linux_subscription_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListLinuxSubscriptionInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [LicenseManagerLinuxSubscriptionsClient](./client.md)
2. paginator: [ListLinuxSubscriptionInstancesPaginator](./paginators.md#listlinuxsubscriptioninstancespaginator)
3. item: [:material-code-braces: ListLinuxSubscriptionInstancesResponseTypeDef](./type_defs.md#listlinuxsubscriptioninstancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLinuxSubscriptionInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListLinuxSubscriptionInstancesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListLinuxSubscriptionInstancesResponseTypeDef](./type_defs.md#listlinuxsubscriptioninstancesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef](./type_defs.md#listlinuxsubscriptioninstancesrequestlistlinuxsubscriptioninstancespaginatetypedef) 
## ListLinuxSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("license-manager-linux-subscriptions").get_paginator("list_linux_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Paginator.ListLinuxSubscriptions)

```python
# ListLinuxSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager_linux_subscriptions.paginator import ListLinuxSubscriptionsPaginator

session = get_session()
async with session.create_client("license-manager-linux-subscriptions") as client:  # (1)
    paginator: ListLinuxSubscriptionsPaginator = client.get_paginator("list_linux_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListLinuxSubscriptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [LicenseManagerLinuxSubscriptionsClient](./client.md)
2. paginator: [ListLinuxSubscriptionsPaginator](./paginators.md#listlinuxsubscriptionspaginator)
3. item: [:material-code-braces: ListLinuxSubscriptionsResponseTypeDef](./type_defs.md#listlinuxsubscriptionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLinuxSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListLinuxSubscriptionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListLinuxSubscriptionsResponseTypeDef](./type_defs.md#listlinuxsubscriptionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef](./type_defs.md#listlinuxsubscriptionsrequestlistlinuxsubscriptionspaginatetypedef) 
