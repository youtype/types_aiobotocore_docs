# Paginators

> [Index](../README.md) > [RedshiftServerless](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [RedshiftServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
    type annotations stubs module [types-aiobotocore-redshift-serverless](https://pypi.org/project/types-aiobotocore-redshift-serverless/).

## ListEndpointAccessPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_endpoint_access")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListEndpointAccess)

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
    vpcId: str = ...,
    workgroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEndpointAccessResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEndpointAccessResponseTypeDef](./type_defs.md#listendpointaccessresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEndpointAccessRequestListEndpointAccessPaginateTypeDef = {  # (1)
    "vpcId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEndpointAccessRequestListEndpointAccessPaginateTypeDef](./type_defs.md#listendpointaccessrequestlistendpointaccesspaginatetypedef) 
## ListNamespacesPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_namespaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListNamespaces)

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
) -> AsyncIterator[ListNamespacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListNamespacesResponseTypeDef](./type_defs.md#listnamespacesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListNamespacesRequestListNamespacesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNamespacesRequestListNamespacesPaginateTypeDef](./type_defs.md#listnamespacesrequestlistnamespacespaginatetypedef) 
## ListRecoveryPointsPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_recovery_points")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints)

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
    endTime: Union[datetime, str] = ...,
    namespaceArn: str = ...,
    namespaceName: str = ...,
    startTime: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRecoveryPointsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecoveryPointsResponseTypeDef](./type_defs.md#listrecoverypointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = {  # (1)
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef](./type_defs.md#listrecoverypointsrequestlistrecoverypointspaginatetypedef) 
## ListSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots)

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
    endTime: Union[datetime, str] = ...,
    namespaceArn: str = ...,
    namespaceName: str = ...,
    ownerAccount: str = ...,
    startTime: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSnapshotsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSnapshotsResponseTypeDef](./type_defs.md#listsnapshotsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSnapshotsRequestListSnapshotsPaginateTypeDef = {  # (1)
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSnapshotsRequestListSnapshotsPaginateTypeDef](./type_defs.md#listsnapshotsrequestlistsnapshotspaginatetypedef) 
## ListTableRestoreStatusPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_table_restore_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListTableRestoreStatus)

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
) -> AsyncIterator[ListTableRestoreStatusResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTableRestoreStatusResponseTypeDef](./type_defs.md#listtablerestorestatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = {  # (1)
    "namespaceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef](./type_defs.md#listtablerestorestatusrequestlisttablerestorestatuspaginatetypedef) 
## ListUsageLimitsPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_usage_limits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListUsageLimits)

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
) -> AsyncIterator[ListUsageLimitsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: UsageLimitUsageTypeType](./literals.md#usagelimitusagetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListUsageLimitsResponseTypeDef](./type_defs.md#listusagelimitsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsageLimitsRequestListUsageLimitsPaginateTypeDef](./type_defs.md#listusagelimitsrequestlistusagelimitspaginatetypedef) 
## ListWorkgroupsPaginator

Type annotations and code completion for `#!python session.create_client("redshift-serverless").get_paginator("list_workgroups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListWorkgroups)

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
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListWorkgroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkgroupsResponseTypeDef](./type_defs.md#listworkgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkgroupsRequestListWorkgroupsPaginateTypeDef](./type_defs.md#listworkgroupsrequestlistworkgroupspaginatetypedef) 
