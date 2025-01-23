# Paginators

> [Index](../README.md) > [RedshiftServerless](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [RedshiftServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#redshiftserverless)
    type annotations stubs module [types-aiobotocore-redshift-serverless](https://pypi.org/project/types-aiobotocore-redshift-serverless/).

## ListCustomDomainAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_custom_domain_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless/paginator/ListCustomDomainAssociations.html#RedshiftServerless.Paginator.ListCustomDomainAssociations)

```python
# ListCustomDomainAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_serverless.paginator import ListCustomDomainAssociationsPaginator

session = get_session()
async with session.create_client("redshift-serverless") as client:  # (1)
    paginator: ListCustomDomainAssociationsPaginator = client.get_paginator("list_custom_domain_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomDomainAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftServerlessClient](./client.md)
2. paginator: [ListCustomDomainAssociationsPaginator](./paginators.md#listcustomdomainassociationspaginator)
3. item: [:material-code-braces: ListCustomDomainAssociationsResponseTypeDef](./type_defs.md#listcustomdomainassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomDomainAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    customDomainCertificateArn: str = ...,
    customDomainName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCustomDomainAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomDomainAssociationsResponseTypeDef](./type_defs.md#listcustomdomainassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomDomainAssociationsRequestPaginateTypeDef = {  # (1)
    "customDomainCertificateArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomDomainAssociationsRequestPaginateTypeDef](./type_defs.md#listcustomdomainassociationsrequestpaginatetypedef) 
## ListEndpointAccessPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_endpoint_access")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless/paginator/ListEndpointAccess.html#RedshiftServerless.Paginator.ListEndpointAccess)

```python
# ListEndpointAccessPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_serverless.paginator import ListEndpointAccessPaginator

session = get_session()
async with session.create_client("redshift-serverless") as client:  # (1)
    paginator: ListEndpointAccessPaginator = client.get_paginator("list_endpoint_access")  # (2)
    async for item in paginator.paginate(...):
        item: ListEndpointAccessResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftServerlessClient](./client.md)
2. paginator: [ListEndpointAccessPaginator](./paginators.md#listendpointaccesspaginator)
3. item: [:material-code-braces: ListEndpointAccessResponseTypeDef](./type_defs.md#listendpointaccessresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEndpointAccessPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ownerAccount: str = ...,
    vpcId: str = ...,
    workgroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEndpointAccessResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEndpointAccessResponseTypeDef](./type_defs.md#listendpointaccessresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEndpointAccessRequestPaginateTypeDef = {  # (1)
    "ownerAccount": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEndpointAccessRequestPaginateTypeDef](./type_defs.md#listendpointaccessrequestpaginatetypedef) 
## ListManagedWorkgroupsPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_managed_workgroups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless/paginator/ListManagedWorkgroups.html#RedshiftServerless.Paginator.ListManagedWorkgroups)

```python
# ListManagedWorkgroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_serverless.paginator import ListManagedWorkgroupsPaginator

session = get_session()
async with session.create_client("redshift-serverless") as client:  # (1)
    paginator: ListManagedWorkgroupsPaginator = client.get_paginator("list_managed_workgroups")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedWorkgroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftServerlessClient](./client.md)
2. paginator: [ListManagedWorkgroupsPaginator](./paginators.md#listmanagedworkgroupspaginator)
3. item: [:material-code-braces: ListManagedWorkgroupsResponseTypeDef](./type_defs.md#listmanagedworkgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListManagedWorkgroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sourceArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListManagedWorkgroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListManagedWorkgroupsResponseTypeDef](./type_defs.md#listmanagedworkgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedWorkgroupsRequestPaginateTypeDef = {  # (1)
    "sourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedWorkgroupsRequestPaginateTypeDef](./type_defs.md#listmanagedworkgroupsrequestpaginatetypedef) 
## ListNamespacesPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_namespaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless/paginator/ListNamespaces.html#RedshiftServerless.Paginator.ListNamespaces)

```python
# ListNamespacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_serverless.paginator import ListNamespacesPaginator

session = get_session()
async with session.create_client("redshift-serverless") as client:  # (1)
    paginator: ListNamespacesPaginator = client.get_paginator("list_namespaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListNamespacesResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftServerlessClient](./client.md)
2. paginator: [ListNamespacesPaginator](./paginators.md#listnamespacespaginator)
3. item: [:material-code-braces: ListNamespacesResponseTypeDef](./type_defs.md#listnamespacesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListNamespacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListNamespacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListNamespacesResponseTypeDef](./type_defs.md#listnamespacesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListNamespacesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNamespacesRequestPaginateTypeDef](./type_defs.md#listnamespacesrequestpaginatetypedef) 
## ListRecoveryPointsPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_recovery_points")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless/paginator/ListRecoveryPoints.html#RedshiftServerless.Paginator.ListRecoveryPoints)

```python
# ListRecoveryPointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_serverless.paginator import ListRecoveryPointsPaginator

session = get_session()
async with session.create_client("redshift-serverless") as client:  # (1)
    paginator: ListRecoveryPointsPaginator = client.get_paginator("list_recovery_points")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecoveryPointsResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftServerlessClient](./client.md)
2. paginator: [ListRecoveryPointsPaginator](./paginators.md#listrecoverypointspaginator)
3. item: [:material-code-braces: ListRecoveryPointsResponseTypeDef](./type_defs.md#listrecoverypointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRecoveryPointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    endTime: TimestampTypeDef = ...,
    namespaceArn: str = ...,
    namespaceName: str = ...,
    startTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRecoveryPointsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecoveryPointsResponseTypeDef](./type_defs.md#listrecoverypointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRecoveryPointsRequestPaginateTypeDef = {  # (1)
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecoveryPointsRequestPaginateTypeDef](./type_defs.md#listrecoverypointsrequestpaginatetypedef) 
## ListScheduledActionsPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_scheduled_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless/paginator/ListScheduledActions.html#RedshiftServerless.Paginator.ListScheduledActions)

```python
# ListScheduledActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_serverless.paginator import ListScheduledActionsPaginator

session = get_session()
async with session.create_client("redshift-serverless") as client:  # (1)
    paginator: ListScheduledActionsPaginator = client.get_paginator("list_scheduled_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListScheduledActionsResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftServerlessClient](./client.md)
2. paginator: [ListScheduledActionsPaginator](./paginators.md#listscheduledactionspaginator)
3. item: [:material-code-braces: ListScheduledActionsResponseTypeDef](./type_defs.md#listscheduledactionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListScheduledActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    namespaceName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListScheduledActionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListScheduledActionsResponseTypeDef](./type_defs.md#listscheduledactionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListScheduledActionsRequestPaginateTypeDef = {  # (1)
    "namespaceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListScheduledActionsRequestPaginateTypeDef](./type_defs.md#listscheduledactionsrequestpaginatetypedef) 
## ListSnapshotCopyConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_snapshot_copy_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless/paginator/ListSnapshotCopyConfigurations.html#RedshiftServerless.Paginator.ListSnapshotCopyConfigurations)

```python
# ListSnapshotCopyConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_serverless.paginator import ListSnapshotCopyConfigurationsPaginator

session = get_session()
async with session.create_client("redshift-serverless") as client:  # (1)
    paginator: ListSnapshotCopyConfigurationsPaginator = client.get_paginator("list_snapshot_copy_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListSnapshotCopyConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftServerlessClient](./client.md)
2. paginator: [ListSnapshotCopyConfigurationsPaginator](./paginators.md#listsnapshotcopyconfigurationspaginator)
3. item: [:material-code-braces: ListSnapshotCopyConfigurationsResponseTypeDef](./type_defs.md#listsnapshotcopyconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSnapshotCopyConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    namespaceName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSnapshotCopyConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSnapshotCopyConfigurationsResponseTypeDef](./type_defs.md#listsnapshotcopyconfigurationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSnapshotCopyConfigurationsRequestPaginateTypeDef = {  # (1)
    "namespaceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSnapshotCopyConfigurationsRequestPaginateTypeDef](./type_defs.md#listsnapshotcopyconfigurationsrequestpaginatetypedef) 
## ListSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless/paginator/ListSnapshots.html#RedshiftServerless.Paginator.ListSnapshots)

```python
# ListSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_serverless.paginator import ListSnapshotsPaginator

session = get_session()
async with session.create_client("redshift-serverless") as client:  # (1)
    paginator: ListSnapshotsPaginator = client.get_paginator("list_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: ListSnapshotsResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftServerlessClient](./client.md)
2. paginator: [ListSnapshotsPaginator](./paginators.md#listsnapshotspaginator)
3. item: [:material-code-braces: ListSnapshotsResponseTypeDef](./type_defs.md#listsnapshotsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    endTime: TimestampTypeDef = ...,
    namespaceArn: str = ...,
    namespaceName: str = ...,
    ownerAccount: str = ...,
    startTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSnapshotsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSnapshotsResponseTypeDef](./type_defs.md#listsnapshotsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSnapshotsRequestPaginateTypeDef = {  # (1)
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSnapshotsRequestPaginateTypeDef](./type_defs.md#listsnapshotsrequestpaginatetypedef) 
## ListTableRestoreStatusPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_table_restore_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless/paginator/ListTableRestoreStatus.html#RedshiftServerless.Paginator.ListTableRestoreStatus)

```python
# ListTableRestoreStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_serverless.paginator import ListTableRestoreStatusPaginator

session = get_session()
async with session.create_client("redshift-serverless") as client:  # (1)
    paginator: ListTableRestoreStatusPaginator = client.get_paginator("list_table_restore_status")  # (2)
    async for item in paginator.paginate(...):
        item: ListTableRestoreStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftServerlessClient](./client.md)
2. paginator: [ListTableRestoreStatusPaginator](./paginators.md#listtablerestorestatuspaginator)
3. item: [:material-code-braces: ListTableRestoreStatusResponseTypeDef](./type_defs.md#listtablerestorestatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTableRestoreStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    namespaceName: str = ...,
    workgroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTableRestoreStatusResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTableRestoreStatusResponseTypeDef](./type_defs.md#listtablerestorestatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTableRestoreStatusRequestPaginateTypeDef = {  # (1)
    "namespaceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTableRestoreStatusRequestPaginateTypeDef](./type_defs.md#listtablerestorestatusrequestpaginatetypedef) 
## ListUsageLimitsPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_usage_limits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless/paginator/ListUsageLimits.html#RedshiftServerless.Paginator.ListUsageLimits)

```python
# ListUsageLimitsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_serverless.paginator import ListUsageLimitsPaginator

session = get_session()
async with session.create_client("redshift-serverless") as client:  # (1)
    paginator: ListUsageLimitsPaginator = client.get_paginator("list_usage_limits")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsageLimitsResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftServerlessClient](./client.md)
2. paginator: [ListUsageLimitsPaginator](./paginators.md#listusagelimitspaginator)
3. item: [:material-code-braces: ListUsageLimitsResponseTypeDef](./type_defs.md#listusagelimitsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsageLimitsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceArn: str = ...,
    usageType: UsageLimitUsageTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListUsageLimitsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: UsageLimitUsageTypeType](./literals.md#usagelimitusagetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListUsageLimitsResponseTypeDef](./type_defs.md#listusagelimitsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUsageLimitsRequestPaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsageLimitsRequestPaginateTypeDef](./type_defs.md#listusagelimitsrequestpaginatetypedef) 
## ListWorkgroupsPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_workgroups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless/paginator/ListWorkgroups.html#RedshiftServerless.Paginator.ListWorkgroups)

```python
# ListWorkgroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_serverless.paginator import ListWorkgroupsPaginator

session = get_session()
async with session.create_client("redshift-serverless") as client:  # (1)
    paginator: ListWorkgroupsPaginator = client.get_paginator("list_workgroups")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkgroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftServerlessClient](./client.md)
2. paginator: [ListWorkgroupsPaginator](./paginators.md#listworkgroupspaginator)
3. item: [:material-code-braces: ListWorkgroupsResponseTypeDef](./type_defs.md#listworkgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkgroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ownerAccount: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWorkgroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkgroupsResponseTypeDef](./type_defs.md#listworkgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkgroupsRequestPaginateTypeDef = {  # (1)
    "ownerAccount": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkgroupsRequestPaginateTypeDef](./type_defs.md#listworkgroupsrequestpaginatetypedef) 
