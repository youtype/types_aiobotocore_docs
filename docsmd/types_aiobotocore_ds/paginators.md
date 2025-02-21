# Paginators

> [Index](../README.md) > [DirectoryService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DirectoryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#directoryservice)
    type annotations stubs module [types-aiobotocore-ds](https://pypi.org/project/types-aiobotocore-ds/).

## DescribeClientAuthenticationSettingsPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_client_authentication_settings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/DescribeClientAuthenticationSettings.html#DirectoryService.Paginator.DescribeClientAuthenticationSettings)

```python
# DescribeClientAuthenticationSettingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeClientAuthenticationSettingsPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeClientAuthenticationSettingsPaginator = client.get_paginator("describe_client_authentication_settings")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeClientAuthenticationSettingsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeClientAuthenticationSettingsPaginator](./paginators.md#describeclientauthenticationsettingspaginator)
3. item: [:material-code-braces: DescribeClientAuthenticationSettingsResultTypeDef](./type_defs.md#describeclientauthenticationsettingsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClientAuthenticationSettingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    Type: ClientAuthenticationTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeClientAuthenticationSettingsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ClientAuthenticationTypeType](./literals.md#clientauthenticationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeClientAuthenticationSettingsResultTypeDef](./type_defs.md#describeclientauthenticationsettingsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClientAuthenticationSettingsRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClientAuthenticationSettingsRequestPaginateTypeDef](./type_defs.md#describeclientauthenticationsettingsrequestpaginatetypedef) 
## DescribeDirectoriesPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_directories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/DescribeDirectories.html#DirectoryService.Paginator.DescribeDirectories)

```python
# DescribeDirectoriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeDirectoriesPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeDirectoriesPaginator = client.get_paginator("describe_directories")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDirectoriesResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeDirectoriesPaginator](./paginators.md#describedirectoriespaginator)
3. item: [:material-code-braces: DescribeDirectoriesResultTypeDef](./type_defs.md#describedirectoriesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDirectoriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeDirectoriesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDirectoriesResultTypeDef](./type_defs.md#describedirectoriesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDirectoriesRequestPaginateTypeDef = {  # (1)
    "DirectoryIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDirectoriesRequestPaginateTypeDef](./type_defs.md#describedirectoriesrequestpaginatetypedef) 
## DescribeDomainControllersPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_domain_controllers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/DescribeDomainControllers.html#DirectoryService.Paginator.DescribeDomainControllers)

```python
# DescribeDomainControllersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeDomainControllersPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeDomainControllersPaginator = client.get_paginator("describe_domain_controllers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDomainControllersResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeDomainControllersPaginator](./paginators.md#describedomaincontrollerspaginator)
3. item: [:material-code-braces: DescribeDomainControllersResultTypeDef](./type_defs.md#describedomaincontrollersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDomainControllersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    DomainControllerIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeDomainControllersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDomainControllersResultTypeDef](./type_defs.md#describedomaincontrollersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDomainControllersRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDomainControllersRequestPaginateTypeDef](./type_defs.md#describedomaincontrollersrequestpaginatetypedef) 
## DescribeLDAPSSettingsPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_ldaps_settings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/DescribeLDAPSSettings.html#DirectoryService.Paginator.DescribeLDAPSSettings)

```python
# DescribeLDAPSSettingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeLDAPSSettingsPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeLDAPSSettingsPaginator = client.get_paginator("describe_ldaps_settings")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLDAPSSettingsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeLDAPSSettingsPaginator](./paginators.md#describeldapssettingspaginator)
3. item: [:material-code-braces: DescribeLDAPSSettingsResultTypeDef](./type_defs.md#describeldapssettingsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLDAPSSettingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    Type: LDAPSTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeLDAPSSettingsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LDAPSTypeType](./literals.md#ldapstypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeLDAPSSettingsResultTypeDef](./type_defs.md#describeldapssettingsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLDAPSSettingsRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLDAPSSettingsRequestPaginateTypeDef](./type_defs.md#describeldapssettingsrequestpaginatetypedef) 
## DescribeRegionsPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_regions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/DescribeRegions.html#DirectoryService.Paginator.DescribeRegions)

```python
# DescribeRegionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeRegionsPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeRegionsPaginator = client.get_paginator("describe_regions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRegionsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeRegionsPaginator](./paginators.md#describeregionspaginator)
3. item: [:material-code-braces: DescribeRegionsResultTypeDef](./type_defs.md#describeregionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRegionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    RegionName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeRegionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRegionsResultTypeDef](./type_defs.md#describeregionsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegionsRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegionsRequestPaginateTypeDef](./type_defs.md#describeregionsrequestpaginatetypedef) 
## DescribeSharedDirectoriesPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_shared_directories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/DescribeSharedDirectories.html#DirectoryService.Paginator.DescribeSharedDirectories)

```python
# DescribeSharedDirectoriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeSharedDirectoriesPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeSharedDirectoriesPaginator = client.get_paginator("describe_shared_directories")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSharedDirectoriesResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeSharedDirectoriesPaginator](./paginators.md#describeshareddirectoriespaginator)
3. item: [:material-code-braces: DescribeSharedDirectoriesResultTypeDef](./type_defs.md#describeshareddirectoriesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSharedDirectoriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OwnerDirectoryId: str,
    SharedDirectoryIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeSharedDirectoriesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSharedDirectoriesResultTypeDef](./type_defs.md#describeshareddirectoriesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSharedDirectoriesRequestPaginateTypeDef = {  # (1)
    "OwnerDirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSharedDirectoriesRequestPaginateTypeDef](./type_defs.md#describeshareddirectoriesrequestpaginatetypedef) 
## DescribeSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/DescribeSnapshots.html#DirectoryService.Paginator.DescribeSnapshots)

```python
# DescribeSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeSnapshotsPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeSnapshotsPaginator = client.get_paginator("describe_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSnapshotsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeSnapshotsPaginator](./paginators.md#describesnapshotspaginator)
3. item: [:material-code-braces: DescribeSnapshotsResultTypeDef](./type_defs.md#describesnapshotsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str = ...,
    SnapshotIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeSnapshotsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSnapshotsResultTypeDef](./type_defs.md#describesnapshotsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSnapshotsRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotsRequestPaginateTypeDef](./type_defs.md#describesnapshotsrequestpaginatetypedef) 
## DescribeTrustsPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_trusts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/DescribeTrusts.html#DirectoryService.Paginator.DescribeTrusts)

```python
# DescribeTrustsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeTrustsPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeTrustsPaginator = client.get_paginator("describe_trusts")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTrustsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeTrustsPaginator](./paginators.md#describetrustspaginator)
3. item: [:material-code-braces: DescribeTrustsResultTypeDef](./type_defs.md#describetrustsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTrustsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str = ...,
    TrustIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeTrustsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeTrustsResultTypeDef](./type_defs.md#describetrustsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTrustsRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTrustsRequestPaginateTypeDef](./type_defs.md#describetrustsrequestpaginatetypedef) 
## DescribeUpdateDirectoryPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_update_directory")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/DescribeUpdateDirectory.html#DirectoryService.Paginator.DescribeUpdateDirectory)

```python
# DescribeUpdateDirectoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeUpdateDirectoryPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeUpdateDirectoryPaginator = client.get_paginator("describe_update_directory")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeUpdateDirectoryResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeUpdateDirectoryPaginator](./paginators.md#describeupdatedirectorypaginator)
3. item: [:material-code-braces: DescribeUpdateDirectoryResultTypeDef](./type_defs.md#describeupdatedirectoryresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeUpdateDirectoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    UpdateType: UpdateTypeType,  # (1)
    RegionName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeUpdateDirectoryResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: UpdateTypeType](./literals.md#updatetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeUpdateDirectoryResultTypeDef](./type_defs.md#describeupdatedirectoryresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeUpdateDirectoryRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
    "UpdateType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeUpdateDirectoryRequestPaginateTypeDef](./type_defs.md#describeupdatedirectoryrequestpaginatetypedef) 
## ListCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("list_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/ListCertificates.html#DirectoryService.Paginator.ListCertificates)

```python
# ListCertificatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import ListCertificatesPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: ListCertificatesPaginator = client.get_paginator("list_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: ListCertificatesResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)
3. item: [:material-code-braces: ListCertificatesResultTypeDef](./type_defs.md#listcertificatesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListCertificatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCertificatesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCertificatesResultTypeDef](./type_defs.md#listcertificatesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCertificatesRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCertificatesRequestPaginateTypeDef](./type_defs.md#listcertificatesrequestpaginatetypedef) 
## ListIpRoutesPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("list_ip_routes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/ListIpRoutes.html#DirectoryService.Paginator.ListIpRoutes)

```python
# ListIpRoutesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import ListIpRoutesPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: ListIpRoutesPaginator = client.get_paginator("list_ip_routes")  # (2)
    async for item in paginator.paginate(...):
        item: ListIpRoutesResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [ListIpRoutesPaginator](./paginators.md#listiproutespaginator)
3. item: [:material-code-braces: ListIpRoutesResultTypeDef](./type_defs.md#listiproutesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListIpRoutesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListIpRoutesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIpRoutesResultTypeDef](./type_defs.md#listiproutesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIpRoutesRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIpRoutesRequestPaginateTypeDef](./type_defs.md#listiproutesrequestpaginatetypedef) 
## ListLogSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("list_log_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/ListLogSubscriptions.html#DirectoryService.Paginator.ListLogSubscriptions)

```python
# ListLogSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import ListLogSubscriptionsPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: ListLogSubscriptionsPaginator = client.get_paginator("list_log_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListLogSubscriptionsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [ListLogSubscriptionsPaginator](./paginators.md#listlogsubscriptionspaginator)
3. item: [:material-code-braces: ListLogSubscriptionsResultTypeDef](./type_defs.md#listlogsubscriptionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListLogSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListLogSubscriptionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLogSubscriptionsResultTypeDef](./type_defs.md#listlogsubscriptionsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLogSubscriptionsRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLogSubscriptionsRequestPaginateTypeDef](./type_defs.md#listlogsubscriptionsrequestpaginatetypedef) 
## ListSchemaExtensionsPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("list_schema_extensions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/ListSchemaExtensions.html#DirectoryService.Paginator.ListSchemaExtensions)

```python
# ListSchemaExtensionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import ListSchemaExtensionsPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: ListSchemaExtensionsPaginator = client.get_paginator("list_schema_extensions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemaExtensionsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [ListSchemaExtensionsPaginator](./paginators.md#listschemaextensionspaginator)
3. item: [:material-code-braces: ListSchemaExtensionsResultTypeDef](./type_defs.md#listschemaextensionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListSchemaExtensionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSchemaExtensionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchemaExtensionsResultTypeDef](./type_defs.md#listschemaextensionsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSchemaExtensionsRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemaExtensionsRequestPaginateTypeDef](./type_defs.md#listschemaextensionsrequestpaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds/paginator/ListTagsForResource.html#DirectoryService.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTagsForResourceResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestPaginateTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef) 
