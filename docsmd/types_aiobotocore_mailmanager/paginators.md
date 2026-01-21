# Paginators

> [Index](../README.md) > [MailManager](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MailManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager.html#mailmanager)
    type annotations stubs module [types-aiobotocore-mailmanager](https://pypi.org/project/types-aiobotocore-mailmanager/).

## ListAddonInstancesPaginator

Type annotations and code completion for `#!python session.create_client("mailmanager").get_paginator("list_addon_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/paginator/ListAddonInstances.html#MailManager.Paginator.ListAddonInstances)

```python
# ListAddonInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.paginator import ListAddonInstancesPaginator

session = get_session()
async with session.create_client("mailmanager") as client:  # (1)
    paginator: ListAddonInstancesPaginator = client.get_paginator("list_addon_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListAddonInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListAddonInstancesPaginator](./paginators.md#listaddoninstancespaginator)
3. item: `AioPageIterator[ListAddonInstancesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAddonInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAddonInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAddonInstancesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAddonInstancesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAddonInstancesRequestPaginateTypeDef](./type_defs.md#listaddoninstancesrequestpaginatetypedef)
## ListAddonSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("mailmanager").get_paginator("list_addon_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/paginator/ListAddonSubscriptions.html#MailManager.Paginator.ListAddonSubscriptions)

```python
# ListAddonSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.paginator import ListAddonSubscriptionsPaginator

session = get_session()
async with session.create_client("mailmanager") as client:  # (1)
    paginator: ListAddonSubscriptionsPaginator = client.get_paginator("list_addon_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListAddonSubscriptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListAddonSubscriptionsPaginator](./paginators.md#listaddonsubscriptionspaginator)
3. item: `AioPageIterator[ListAddonSubscriptionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAddonSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAddonSubscriptionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAddonSubscriptionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAddonSubscriptionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAddonSubscriptionsRequestPaginateTypeDef](./type_defs.md#listaddonsubscriptionsrequestpaginatetypedef)
## ListAddressListImportJobsPaginator

Type annotations and code completion for `#!python session.create_client("mailmanager").get_paginator("list_address_list_import_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/paginator/ListAddressListImportJobs.html#MailManager.Paginator.ListAddressListImportJobs)

```python
# ListAddressListImportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.paginator import ListAddressListImportJobsPaginator

session = get_session()
async with session.create_client("mailmanager") as client:  # (1)
    paginator: ListAddressListImportJobsPaginator = client.get_paginator("list_address_list_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListAddressListImportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListAddressListImportJobsPaginator](./paginators.md#listaddresslistimportjobspaginator)
3. item: `AioPageIterator[ListAddressListImportJobsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAddressListImportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AddressListId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAddressListImportJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAddressListImportJobsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAddressListImportJobsRequestPaginateTypeDef = {  # (1)
    "AddressListId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAddressListImportJobsRequestPaginateTypeDef](./type_defs.md#listaddresslistimportjobsrequestpaginatetypedef)
## ListAddressListsPaginator

Type annotations and code completion for `#!python session.create_client("mailmanager").get_paginator("list_address_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/paginator/ListAddressLists.html#MailManager.Paginator.ListAddressLists)

```python
# ListAddressListsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.paginator import ListAddressListsPaginator

session = get_session()
async with session.create_client("mailmanager") as client:  # (1)
    paginator: ListAddressListsPaginator = client.get_paginator("list_address_lists")  # (2)
    async for item in paginator.paginate(...):
        item: ListAddressListsResponseTypeDef
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListAddressListsPaginator](./paginators.md#listaddresslistspaginator)
3. item: `AioPageIterator[ListAddressListsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAddressListsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAddressListsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAddressListsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAddressListsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAddressListsRequestPaginateTypeDef](./type_defs.md#listaddresslistsrequestpaginatetypedef)
## ListArchiveExportsPaginator

Type annotations and code completion for `#!python session.create_client("mailmanager").get_paginator("list_archive_exports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/paginator/ListArchiveExports.html#MailManager.Paginator.ListArchiveExports)

```python
# ListArchiveExportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.paginator import ListArchiveExportsPaginator

session = get_session()
async with session.create_client("mailmanager") as client:  # (1)
    paginator: ListArchiveExportsPaginator = client.get_paginator("list_archive_exports")  # (2)
    async for item in paginator.paginate(...):
        item: ListArchiveExportsResponseTypeDef
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListArchiveExportsPaginator](./paginators.md#listarchiveexportspaginator)
3. item: `AioPageIterator[ListArchiveExportsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListArchiveExportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ArchiveId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListArchiveExportsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListArchiveExportsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListArchiveExportsRequestPaginateTypeDef = {  # (1)
    "ArchiveId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListArchiveExportsRequestPaginateTypeDef](./type_defs.md#listarchiveexportsrequestpaginatetypedef)
## ListArchiveSearchesPaginator

Type annotations and code completion for `#!python session.create_client("mailmanager").get_paginator("list_archive_searches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/paginator/ListArchiveSearches.html#MailManager.Paginator.ListArchiveSearches)

```python
# ListArchiveSearchesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.paginator import ListArchiveSearchesPaginator

session = get_session()
async with session.create_client("mailmanager") as client:  # (1)
    paginator: ListArchiveSearchesPaginator = client.get_paginator("list_archive_searches")  # (2)
    async for item in paginator.paginate(...):
        item: ListArchiveSearchesResponseTypeDef
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListArchiveSearchesPaginator](./paginators.md#listarchivesearchespaginator)
3. item: `AioPageIterator[ListArchiveSearchesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListArchiveSearchesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ArchiveId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListArchiveSearchesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListArchiveSearchesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListArchiveSearchesRequestPaginateTypeDef = {  # (1)
    "ArchiveId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListArchiveSearchesRequestPaginateTypeDef](./type_defs.md#listarchivesearchesrequestpaginatetypedef)
## ListArchivesPaginator

Type annotations and code completion for `#!python session.create_client("mailmanager").get_paginator("list_archives")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/paginator/ListArchives.html#MailManager.Paginator.ListArchives)

```python
# ListArchivesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.paginator import ListArchivesPaginator

session = get_session()
async with session.create_client("mailmanager") as client:  # (1)
    paginator: ListArchivesPaginator = client.get_paginator("list_archives")  # (2)
    async for item in paginator.paginate(...):
        item: ListArchivesResponseTypeDef
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListArchivesPaginator](./paginators.md#listarchivespaginator)
3. item: `AioPageIterator[ListArchivesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListArchivesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListArchivesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListArchivesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListArchivesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListArchivesRequestPaginateTypeDef](./type_defs.md#listarchivesrequestpaginatetypedef)
## ListIngressPointsPaginator

Type annotations and code completion for `#!python session.create_client("mailmanager").get_paginator("list_ingress_points")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/paginator/ListIngressPoints.html#MailManager.Paginator.ListIngressPoints)

```python
# ListIngressPointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.paginator import ListIngressPointsPaginator

session = get_session()
async with session.create_client("mailmanager") as client:  # (1)
    paginator: ListIngressPointsPaginator = client.get_paginator("list_ingress_points")  # (2)
    async for item in paginator.paginate(...):
        item: ListIngressPointsResponseTypeDef
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListIngressPointsPaginator](./paginators.md#listingresspointspaginator)
3. item: `AioPageIterator[ListIngressPointsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIngressPointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListIngressPointsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListIngressPointsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIngressPointsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIngressPointsRequestPaginateTypeDef](./type_defs.md#listingresspointsrequestpaginatetypedef)
## ListMembersOfAddressListPaginator

Type annotations and code completion for `#!python session.create_client("mailmanager").get_paginator("list_members_of_address_list")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/paginator/ListMembersOfAddressList.html#MailManager.Paginator.ListMembersOfAddressList)

```python
# ListMembersOfAddressListPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.paginator import ListMembersOfAddressListPaginator

session = get_session()
async with session.create_client("mailmanager") as client:  # (1)
    paginator: ListMembersOfAddressListPaginator = client.get_paginator("list_members_of_address_list")  # (2)
    async for item in paginator.paginate(...):
        item: ListMembersOfAddressListResponseTypeDef
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListMembersOfAddressListPaginator](./paginators.md#listmembersofaddresslistpaginator)
3. item: `AioPageIterator[ListMembersOfAddressListResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMembersOfAddressListPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AddressListId: str,
    Filter: AddressFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListMembersOfAddressListResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AddressFilterTypeDef](./type_defs.md#addressfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListMembersOfAddressListResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMembersOfAddressListRequestPaginateTypeDef = {  # (1)
    "AddressListId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMembersOfAddressListRequestPaginateTypeDef](./type_defs.md#listmembersofaddresslistrequestpaginatetypedef)
## ListRelaysPaginator

Type annotations and code completion for `#!python session.create_client("mailmanager").get_paginator("list_relays")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/paginator/ListRelays.html#MailManager.Paginator.ListRelays)

```python
# ListRelaysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.paginator import ListRelaysPaginator

session = get_session()
async with session.create_client("mailmanager") as client:  # (1)
    paginator: ListRelaysPaginator = client.get_paginator("list_relays")  # (2)
    async for item in paginator.paginate(...):
        item: ListRelaysResponseTypeDef
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListRelaysPaginator](./paginators.md#listrelayspaginator)
3. item: `AioPageIterator[ListRelaysResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRelaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRelaysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRelaysResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRelaysRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRelaysRequestPaginateTypeDef](./type_defs.md#listrelaysrequestpaginatetypedef)
## ListRuleSetsPaginator

Type annotations and code completion for `#!python session.create_client("mailmanager").get_paginator("list_rule_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/paginator/ListRuleSets.html#MailManager.Paginator.ListRuleSets)

```python
# ListRuleSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.paginator import ListRuleSetsPaginator

session = get_session()
async with session.create_client("mailmanager") as client:  # (1)
    paginator: ListRuleSetsPaginator = client.get_paginator("list_rule_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListRuleSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListRuleSetsPaginator](./paginators.md#listrulesetspaginator)
3. item: `AioPageIterator[ListRuleSetsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRuleSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRuleSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRuleSetsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRuleSetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRuleSetsRequestPaginateTypeDef](./type_defs.md#listrulesetsrequestpaginatetypedef)
## ListTrafficPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("mailmanager").get_paginator("list_traffic_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/paginator/ListTrafficPolicies.html#MailManager.Paginator.ListTrafficPolicies)

```python
# ListTrafficPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.paginator import ListTrafficPoliciesPaginator

session = get_session()
async with session.create_client("mailmanager") as client:  # (1)
    paginator: ListTrafficPoliciesPaginator = client.get_paginator("list_traffic_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListTrafficPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListTrafficPoliciesPaginator](./paginators.md#listtrafficpoliciespaginator)
3. item: `AioPageIterator[ListTrafficPoliciesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTrafficPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTrafficPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTrafficPoliciesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTrafficPoliciesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrafficPoliciesRequestPaginateTypeDef](./type_defs.md#listtrafficpoliciesrequestpaginatetypedef)
