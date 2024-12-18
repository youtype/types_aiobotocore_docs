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
3. item: [:material-code-braces: ListAddonInstancesResponseTypeDef](./type_defs.md#listaddoninstancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAddonInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAddonInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAddonInstancesResponseTypeDef](./type_defs.md#listaddoninstancesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAddonInstancesRequestListAddonInstancesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAddonInstancesRequestListAddonInstancesPaginateTypeDef](./type_defs.md#listaddoninstancesrequestlistaddoninstancespaginatetypedef) 
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
3. item: [:material-code-braces: ListAddonSubscriptionsResponseTypeDef](./type_defs.md#listaddonsubscriptionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAddonSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAddonSubscriptionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAddonSubscriptionsResponseTypeDef](./type_defs.md#listaddonsubscriptionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAddonSubscriptionsRequestListAddonSubscriptionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAddonSubscriptionsRequestListAddonSubscriptionsPaginateTypeDef](./type_defs.md#listaddonsubscriptionsrequestlistaddonsubscriptionspaginatetypedef) 
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
3. item: [:material-code-braces: ListArchiveExportsResponseTypeDef](./type_defs.md#listarchiveexportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListArchiveExportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ArchiveId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListArchiveExportsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListArchiveExportsResponseTypeDef](./type_defs.md#listarchiveexportsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListArchiveExportsRequestListArchiveExportsPaginateTypeDef = {  # (1)
    "ArchiveId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListArchiveExportsRequestListArchiveExportsPaginateTypeDef](./type_defs.md#listarchiveexportsrequestlistarchiveexportspaginatetypedef) 
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
3. item: [:material-code-braces: ListArchiveSearchesResponseTypeDef](./type_defs.md#listarchivesearchesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListArchiveSearchesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ArchiveId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListArchiveSearchesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListArchiveSearchesResponseTypeDef](./type_defs.md#listarchivesearchesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListArchiveSearchesRequestListArchiveSearchesPaginateTypeDef = {  # (1)
    "ArchiveId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListArchiveSearchesRequestListArchiveSearchesPaginateTypeDef](./type_defs.md#listarchivesearchesrequestlistarchivesearchespaginatetypedef) 
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
3. item: [:material-code-braces: ListArchivesResponseTypeDef](./type_defs.md#listarchivesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListArchivesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListArchivesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListArchivesResponseTypeDef](./type_defs.md#listarchivesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListArchivesRequestListArchivesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListArchivesRequestListArchivesPaginateTypeDef](./type_defs.md#listarchivesrequestlistarchivespaginatetypedef) 
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
3. item: [:material-code-braces: ListIngressPointsResponseTypeDef](./type_defs.md#listingresspointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIngressPointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListIngressPointsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIngressPointsResponseTypeDef](./type_defs.md#listingresspointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIngressPointsRequestListIngressPointsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIngressPointsRequestListIngressPointsPaginateTypeDef](./type_defs.md#listingresspointsrequestlistingresspointspaginatetypedef) 
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
3. item: [:material-code-braces: ListRelaysResponseTypeDef](./type_defs.md#listrelaysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRelaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRelaysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRelaysResponseTypeDef](./type_defs.md#listrelaysresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRelaysRequestListRelaysPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRelaysRequestListRelaysPaginateTypeDef](./type_defs.md#listrelaysrequestlistrelayspaginatetypedef) 
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
3. item: [:material-code-braces: ListRuleSetsResponseTypeDef](./type_defs.md#listrulesetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRuleSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRuleSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRuleSetsResponseTypeDef](./type_defs.md#listrulesetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRuleSetsRequestListRuleSetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRuleSetsRequestListRuleSetsPaginateTypeDef](./type_defs.md#listrulesetsrequestlistrulesetspaginatetypedef) 
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
3. item: [:material-code-braces: ListTrafficPoliciesResponseTypeDef](./type_defs.md#listtrafficpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTrafficPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTrafficPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTrafficPoliciesResponseTypeDef](./type_defs.md#listtrafficpoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTrafficPoliciesRequestListTrafficPoliciesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrafficPoliciesRequestListTrafficPoliciesPaginateTypeDef](./type_defs.md#listtrafficpoliciesrequestlisttrafficpoliciespaginatetypedef) 
