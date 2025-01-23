# Paginators

> [Index](../README.md) > [RDS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [RDS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#rds)
    type annotations stubs module [types-aiobotocore-rds](https://pypi.org/project/types-aiobotocore-rds/).

## DescribeBlueGreenDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_blue_green_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeBlueGreenDeployments.html#RDS.Paginator.DescribeBlueGreenDeployments)

```python
# DescribeBlueGreenDeploymentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeBlueGreenDeploymentsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeBlueGreenDeploymentsPaginator = client.get_paginator("describe_blue_green_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBlueGreenDeploymentsResponseTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeBlueGreenDeploymentsPaginator](./paginators.md#describebluegreendeploymentspaginator)
3. item: [:material-code-braces: DescribeBlueGreenDeploymentsResponseTypeDef](./type_defs.md#describebluegreendeploymentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeBlueGreenDeploymentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    BlueGreenDeploymentIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeBlueGreenDeploymentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeBlueGreenDeploymentsResponseTypeDef](./type_defs.md#describebluegreendeploymentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeBlueGreenDeploymentsRequestPaginateTypeDef = {  # (1)
    "BlueGreenDeploymentIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBlueGreenDeploymentsRequestPaginateTypeDef](./type_defs.md#describebluegreendeploymentsrequestpaginatetypedef) 
## DescribeCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeCertificates.html#RDS.Paginator.DescribeCertificates)

```python
# DescribeCertificatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeCertificatesPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeCertificatesPaginator = client.get_paginator("describe_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: CertificateMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeCertificatesPaginator](./paginators.md#describecertificatespaginator)
3. item: [:material-code-braces: CertificateMessageTypeDef](./type_defs.md#certificatemessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCertificatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CertificateIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[CertificateMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: CertificateMessageTypeDef](./type_defs.md#certificatemessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCertificatesMessagePaginateTypeDef = {  # (1)
    "CertificateIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCertificatesMessagePaginateTypeDef](./type_defs.md#describecertificatesmessagepaginatetypedef) 
## DescribeDBClusterAutomatedBackupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_cluster_automated_backups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBClusterAutomatedBackups.html#RDS.Paginator.DescribeDBClusterAutomatedBackups)

```python
# DescribeDBClusterAutomatedBackupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBClusterAutomatedBackupsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBClusterAutomatedBackupsPaginator = client.get_paginator("describe_db_cluster_automated_backups")  # (2)
    async for item in paginator.paginate(...):
        item: DBClusterAutomatedBackupMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBClusterAutomatedBackupsPaginator](./paginators.md#describedbclusterautomatedbackupspaginator)
3. item: [:material-code-braces: DBClusterAutomatedBackupMessageTypeDef](./type_defs.md#dbclusterautomatedbackupmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBClusterAutomatedBackupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DbClusterResourceId: str = ...,
    DBClusterIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBClusterAutomatedBackupMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterAutomatedBackupMessageTypeDef](./type_defs.md#dbclusterautomatedbackupmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBClusterAutomatedBackupsMessagePaginateTypeDef = {  # (1)
    "DbClusterResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterAutomatedBackupsMessagePaginateTypeDef](./type_defs.md#describedbclusterautomatedbackupsmessagepaginatetypedef) 
## DescribeDBClusterBacktracksPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_cluster_backtracks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBClusterBacktracks.html#RDS.Paginator.DescribeDBClusterBacktracks)

```python
# DescribeDBClusterBacktracksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBClusterBacktracksPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBClusterBacktracksPaginator = client.get_paginator("describe_db_cluster_backtracks")  # (2)
    async for item in paginator.paginate(...):
        item: DBClusterBacktrackMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBClusterBacktracksPaginator](./paginators.md#describedbclusterbacktrackspaginator)
3. item: [:material-code-braces: DBClusterBacktrackMessageTypeDef](./type_defs.md#dbclusterbacktrackmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBClusterBacktracksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBClusterIdentifier: str,
    BacktrackIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBClusterBacktrackMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterBacktrackMessageTypeDef](./type_defs.md#dbclusterbacktrackmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBClusterBacktracksMessagePaginateTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterBacktracksMessagePaginateTypeDef](./type_defs.md#describedbclusterbacktracksmessagepaginatetypedef) 
## DescribeDBClusterEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_cluster_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBClusterEndpoints.html#RDS.Paginator.DescribeDBClusterEndpoints)

```python
# DescribeDBClusterEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBClusterEndpointsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBClusterEndpointsPaginator = client.get_paginator("describe_db_cluster_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: DBClusterEndpointMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBClusterEndpointsPaginator](./paginators.md#describedbclusterendpointspaginator)
3. item: [:material-code-braces: DBClusterEndpointMessageTypeDef](./type_defs.md#dbclusterendpointmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBClusterEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBClusterIdentifier: str = ...,
    DBClusterEndpointIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBClusterEndpointMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterEndpointMessageTypeDef](./type_defs.md#dbclusterendpointmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBClusterEndpointsMessagePaginateTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterEndpointsMessagePaginateTypeDef](./type_defs.md#describedbclusterendpointsmessagepaginatetypedef) 
## DescribeDBClusterParameterGroupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_cluster_parameter_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBClusterParameterGroups.html#RDS.Paginator.DescribeDBClusterParameterGroups)

```python
# DescribeDBClusterParameterGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBClusterParameterGroupsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBClusterParameterGroupsPaginator = client.get_paginator("describe_db_cluster_parameter_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DBClusterParameterGroupsMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBClusterParameterGroupsPaginator](./paginators.md#describedbclusterparametergroupspaginator)
3. item: [:material-code-braces: DBClusterParameterGroupsMessageTypeDef](./type_defs.md#dbclusterparametergroupsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBClusterParameterGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBClusterParameterGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBClusterParameterGroupsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterParameterGroupsMessageTypeDef](./type_defs.md#dbclusterparametergroupsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBClusterParameterGroupsMessagePaginateTypeDef = {  # (1)
    "DBClusterParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterParameterGroupsMessagePaginateTypeDef](./type_defs.md#describedbclusterparametergroupsmessagepaginatetypedef) 
## DescribeDBClusterParametersPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_cluster_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBClusterParameters.html#RDS.Paginator.DescribeDBClusterParameters)

```python
# DescribeDBClusterParametersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBClusterParametersPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBClusterParametersPaginator = client.get_paginator("describe_db_cluster_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: DBClusterParameterGroupDetailsTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBClusterParametersPaginator](./paginators.md#describedbclusterparameterspaginator)
3. item: [:material-code-braces: DBClusterParameterGroupDetailsTypeDef](./type_defs.md#dbclusterparametergroupdetailstypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBClusterParametersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBClusterParameterGroupName: str,
    Source: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBClusterParameterGroupDetailsTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterParameterGroupDetailsTypeDef](./type_defs.md#dbclusterparametergroupdetailstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBClusterParametersMessagePaginateTypeDef = {  # (1)
    "DBClusterParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterParametersMessagePaginateTypeDef](./type_defs.md#describedbclusterparametersmessagepaginatetypedef) 
## DescribeDBClusterSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_cluster_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBClusterSnapshots.html#RDS.Paginator.DescribeDBClusterSnapshots)

```python
# DescribeDBClusterSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBClusterSnapshotsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBClusterSnapshotsPaginator = client.get_paginator("describe_db_cluster_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: DBClusterSnapshotMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBClusterSnapshotsPaginator](./paginators.md#describedbclustersnapshotspaginator)
3. item: [:material-code-braces: DBClusterSnapshotMessageTypeDef](./type_defs.md#dbclustersnapshotmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBClusterSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBClusterIdentifier: str = ...,
    DBClusterSnapshotIdentifier: str = ...,
    SnapshotType: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IncludeShared: bool = ...,
    IncludePublic: bool = ...,
    DbClusterResourceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBClusterSnapshotMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterSnapshotMessageTypeDef](./type_defs.md#dbclustersnapshotmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBClusterSnapshotsMessagePaginateTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterSnapshotsMessagePaginateTypeDef](./type_defs.md#describedbclustersnapshotsmessagepaginatetypedef) 
## DescribeDBClustersPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBClusters.html#RDS.Paginator.DescribeDBClusters)

```python
# DescribeDBClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBClustersPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBClustersPaginator = client.get_paginator("describe_db_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: DBClusterMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBClustersPaginator](./paginators.md#describedbclusterspaginator)
3. item: [:material-code-braces: DBClusterMessageTypeDef](./type_defs.md#dbclustermessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBClusterIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IncludeShared: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBClusterMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterMessageTypeDef](./type_defs.md#dbclustermessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBClustersMessagePaginateTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClustersMessagePaginateTypeDef](./type_defs.md#describedbclustersmessagepaginatetypedef) 
## DescribeDBEngineVersionsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_engine_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBEngineVersions.html#RDS.Paginator.DescribeDBEngineVersions)

```python
# DescribeDBEngineVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBEngineVersionsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBEngineVersionsPaginator = client.get_paginator("describe_db_engine_versions")  # (2)
    async for item in paginator.paginate(...):
        item: DBEngineVersionMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBEngineVersionsPaginator](./paginators.md#describedbengineversionspaginator)
3. item: [:material-code-braces: DBEngineVersionMessageTypeDef](./type_defs.md#dbengineversionmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBEngineVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Engine: str = ...,
    EngineVersion: str = ...,
    DBParameterGroupFamily: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DefaultOnly: bool = ...,
    ListSupportedCharacterSets: bool = ...,
    ListSupportedTimezones: bool = ...,
    IncludeAll: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBEngineVersionMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBEngineVersionMessageTypeDef](./type_defs.md#dbengineversionmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBEngineVersionsMessagePaginateTypeDef = {  # (1)
    "Engine": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBEngineVersionsMessagePaginateTypeDef](./type_defs.md#describedbengineversionsmessagepaginatetypedef) 
## DescribeDBInstanceAutomatedBackupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_instance_automated_backups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBInstanceAutomatedBackups.html#RDS.Paginator.DescribeDBInstanceAutomatedBackups)

```python
# DescribeDBInstanceAutomatedBackupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBInstanceAutomatedBackupsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBInstanceAutomatedBackupsPaginator = client.get_paginator("describe_db_instance_automated_backups")  # (2)
    async for item in paginator.paginate(...):
        item: DBInstanceAutomatedBackupMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBInstanceAutomatedBackupsPaginator](./paginators.md#describedbinstanceautomatedbackupspaginator)
3. item: [:material-code-braces: DBInstanceAutomatedBackupMessageTypeDef](./type_defs.md#dbinstanceautomatedbackupmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBInstanceAutomatedBackupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DbiResourceId: str = ...,
    DBInstanceIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DBInstanceAutomatedBackupsArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBInstanceAutomatedBackupMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBInstanceAutomatedBackupMessageTypeDef](./type_defs.md#dbinstanceautomatedbackupmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBInstanceAutomatedBackupsMessagePaginateTypeDef = {  # (1)
    "DbiResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBInstanceAutomatedBackupsMessagePaginateTypeDef](./type_defs.md#describedbinstanceautomatedbackupsmessagepaginatetypedef) 
## DescribeDBInstancesPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBInstances.html#RDS.Paginator.DescribeDBInstances)

```python
# DescribeDBInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBInstancesPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBInstancesPaginator = client.get_paginator("describe_db_instances")  # (2)
    async for item in paginator.paginate(...):
        item: DBInstanceMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBInstancesPaginator](./paginators.md#describedbinstancespaginator)
3. item: [:material-code-braces: DBInstanceMessageTypeDef](./type_defs.md#dbinstancemessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBInstanceMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBInstanceMessageTypeDef](./type_defs.md#dbinstancemessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBInstancesMessagePaginateTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBInstancesMessagePaginateTypeDef](./type_defs.md#describedbinstancesmessagepaginatetypedef) 
## DescribeDBLogFilesPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_log_files")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBLogFiles.html#RDS.Paginator.DescribeDBLogFiles)

```python
# DescribeDBLogFilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBLogFilesPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBLogFilesPaginator = client.get_paginator("describe_db_log_files")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDBLogFilesResponseTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBLogFilesPaginator](./paginators.md#describedblogfilespaginator)
3. item: [:material-code-braces: DescribeDBLogFilesResponseTypeDef](./type_defs.md#describedblogfilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBLogFilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBInstanceIdentifier: str,
    FilenameContains: str = ...,
    FileLastWritten: int = ...,
    FileSize: int = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeDBLogFilesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDBLogFilesResponseTypeDef](./type_defs.md#describedblogfilesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBLogFilesMessagePaginateTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBLogFilesMessagePaginateTypeDef](./type_defs.md#describedblogfilesmessagepaginatetypedef) 
## DescribeDBParameterGroupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_parameter_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBParameterGroups.html#RDS.Paginator.DescribeDBParameterGroups)

```python
# DescribeDBParameterGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBParameterGroupsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBParameterGroupsPaginator = client.get_paginator("describe_db_parameter_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DBParameterGroupsMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBParameterGroupsPaginator](./paginators.md#describedbparametergroupspaginator)
3. item: [:material-code-braces: DBParameterGroupsMessageTypeDef](./type_defs.md#dbparametergroupsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBParameterGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBParameterGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBParameterGroupsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBParameterGroupsMessageTypeDef](./type_defs.md#dbparametergroupsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBParameterGroupsMessagePaginateTypeDef = {  # (1)
    "DBParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBParameterGroupsMessagePaginateTypeDef](./type_defs.md#describedbparametergroupsmessagepaginatetypedef) 
## DescribeDBParametersPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBParameters.html#RDS.Paginator.DescribeDBParameters)

```python
# DescribeDBParametersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBParametersPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBParametersPaginator = client.get_paginator("describe_db_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: DBParameterGroupDetailsTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBParametersPaginator](./paginators.md#describedbparameterspaginator)
3. item: [:material-code-braces: DBParameterGroupDetailsTypeDef](./type_defs.md#dbparametergroupdetailstypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBParametersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBParameterGroupName: str,
    Source: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBParameterGroupDetailsTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBParameterGroupDetailsTypeDef](./type_defs.md#dbparametergroupdetailstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBParametersMessagePaginateTypeDef = {  # (1)
    "DBParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBParametersMessagePaginateTypeDef](./type_defs.md#describedbparametersmessagepaginatetypedef) 
## DescribeDBProxiesPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_proxies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBProxies.html#RDS.Paginator.DescribeDBProxies)

```python
# DescribeDBProxiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBProxiesPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBProxiesPaginator = client.get_paginator("describe_db_proxies")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDBProxiesResponseTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBProxiesPaginator](./paginators.md#describedbproxiespaginator)
3. item: [:material-code-braces: DescribeDBProxiesResponseTypeDef](./type_defs.md#describedbproxiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBProxiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBProxyName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeDBProxiesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDBProxiesResponseTypeDef](./type_defs.md#describedbproxiesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBProxiesRequestPaginateTypeDef = {  # (1)
    "DBProxyName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBProxiesRequestPaginateTypeDef](./type_defs.md#describedbproxiesrequestpaginatetypedef) 
## DescribeDBProxyEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_proxy_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBProxyEndpoints.html#RDS.Paginator.DescribeDBProxyEndpoints)

```python
# DescribeDBProxyEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBProxyEndpointsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBProxyEndpointsPaginator = client.get_paginator("describe_db_proxy_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDBProxyEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBProxyEndpointsPaginator](./paginators.md#describedbproxyendpointspaginator)
3. item: [:material-code-braces: DescribeDBProxyEndpointsResponseTypeDef](./type_defs.md#describedbproxyendpointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBProxyEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBProxyName: str = ...,
    DBProxyEndpointName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeDBProxyEndpointsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDBProxyEndpointsResponseTypeDef](./type_defs.md#describedbproxyendpointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBProxyEndpointsRequestPaginateTypeDef = {  # (1)
    "DBProxyName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBProxyEndpointsRequestPaginateTypeDef](./type_defs.md#describedbproxyendpointsrequestpaginatetypedef) 
## DescribeDBProxyTargetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_proxy_target_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBProxyTargetGroups.html#RDS.Paginator.DescribeDBProxyTargetGroups)

```python
# DescribeDBProxyTargetGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBProxyTargetGroupsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBProxyTargetGroupsPaginator = client.get_paginator("describe_db_proxy_target_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDBProxyTargetGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBProxyTargetGroupsPaginator](./paginators.md#describedbproxytargetgroupspaginator)
3. item: [:material-code-braces: DescribeDBProxyTargetGroupsResponseTypeDef](./type_defs.md#describedbproxytargetgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBProxyTargetGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBProxyName: str,
    TargetGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeDBProxyTargetGroupsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDBProxyTargetGroupsResponseTypeDef](./type_defs.md#describedbproxytargetgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBProxyTargetGroupsRequestPaginateTypeDef = {  # (1)
    "DBProxyName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBProxyTargetGroupsRequestPaginateTypeDef](./type_defs.md#describedbproxytargetgroupsrequestpaginatetypedef) 
## DescribeDBProxyTargetsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_proxy_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBProxyTargets.html#RDS.Paginator.DescribeDBProxyTargets)

```python
# DescribeDBProxyTargetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBProxyTargetsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBProxyTargetsPaginator = client.get_paginator("describe_db_proxy_targets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDBProxyTargetsResponseTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBProxyTargetsPaginator](./paginators.md#describedbproxytargetspaginator)
3. item: [:material-code-braces: DescribeDBProxyTargetsResponseTypeDef](./type_defs.md#describedbproxytargetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBProxyTargetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBProxyName: str,
    TargetGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeDBProxyTargetsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDBProxyTargetsResponseTypeDef](./type_defs.md#describedbproxytargetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBProxyTargetsRequestPaginateTypeDef = {  # (1)
    "DBProxyName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBProxyTargetsRequestPaginateTypeDef](./type_defs.md#describedbproxytargetsrequestpaginatetypedef) 
## DescribeDBRecommendationsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_recommendations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBRecommendations.html#RDS.Paginator.DescribeDBRecommendations)

```python
# DescribeDBRecommendationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBRecommendationsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBRecommendationsPaginator = client.get_paginator("describe_db_recommendations")  # (2)
    async for item in paginator.paginate(...):
        item: DBRecommendationsMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBRecommendationsPaginator](./paginators.md#describedbrecommendationspaginator)
3. item: [:material-code-braces: DBRecommendationsMessageTypeDef](./type_defs.md#dbrecommendationsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBRecommendationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LastUpdatedAfter: TimestampTypeDef = ...,
    LastUpdatedBefore: TimestampTypeDef = ...,
    Locale: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBRecommendationsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBRecommendationsMessageTypeDef](./type_defs.md#dbrecommendationsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBRecommendationsMessagePaginateTypeDef = {  # (1)
    "LastUpdatedAfter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBRecommendationsMessagePaginateTypeDef](./type_defs.md#describedbrecommendationsmessagepaginatetypedef) 
## DescribeDBSecurityGroupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_security_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBSecurityGroups.html#RDS.Paginator.DescribeDBSecurityGroups)

```python
# DescribeDBSecurityGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBSecurityGroupsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBSecurityGroupsPaginator = client.get_paginator("describe_db_security_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DBSecurityGroupMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBSecurityGroupsPaginator](./paginators.md#describedbsecuritygroupspaginator)
3. item: [:material-code-braces: DBSecurityGroupMessageTypeDef](./type_defs.md#dbsecuritygroupmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBSecurityGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBSecurityGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBSecurityGroupMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBSecurityGroupMessageTypeDef](./type_defs.md#dbsecuritygroupmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBSecurityGroupsMessagePaginateTypeDef = {  # (1)
    "DBSecurityGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBSecurityGroupsMessagePaginateTypeDef](./type_defs.md#describedbsecuritygroupsmessagepaginatetypedef) 
## DescribeDBSnapshotTenantDatabasesPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_snapshot_tenant_databases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBSnapshotTenantDatabases.html#RDS.Paginator.DescribeDBSnapshotTenantDatabases)

```python
# DescribeDBSnapshotTenantDatabasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBSnapshotTenantDatabasesPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBSnapshotTenantDatabasesPaginator = client.get_paginator("describe_db_snapshot_tenant_databases")  # (2)
    async for item in paginator.paginate(...):
        item: DBSnapshotTenantDatabasesMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBSnapshotTenantDatabasesPaginator](./paginators.md#describedbsnapshottenantdatabasespaginator)
3. item: [:material-code-braces: DBSnapshotTenantDatabasesMessageTypeDef](./type_defs.md#dbsnapshottenantdatabasesmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBSnapshotTenantDatabasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    DBSnapshotIdentifier: str = ...,
    SnapshotType: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DbiResourceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBSnapshotTenantDatabasesMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBSnapshotTenantDatabasesMessageTypeDef](./type_defs.md#dbsnapshottenantdatabasesmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBSnapshotTenantDatabasesMessagePaginateTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBSnapshotTenantDatabasesMessagePaginateTypeDef](./type_defs.md#describedbsnapshottenantdatabasesmessagepaginatetypedef) 
## DescribeDBSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBSnapshots.html#RDS.Paginator.DescribeDBSnapshots)

```python
# DescribeDBSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBSnapshotsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBSnapshotsPaginator = client.get_paginator("describe_db_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: DBSnapshotMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBSnapshotsPaginator](./paginators.md#describedbsnapshotspaginator)
3. item: [:material-code-braces: DBSnapshotMessageTypeDef](./type_defs.md#dbsnapshotmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    DBSnapshotIdentifier: str = ...,
    SnapshotType: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IncludeShared: bool = ...,
    IncludePublic: bool = ...,
    DbiResourceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBSnapshotMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBSnapshotMessageTypeDef](./type_defs.md#dbsnapshotmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBSnapshotsMessagePaginateTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBSnapshotsMessagePaginateTypeDef](./type_defs.md#describedbsnapshotsmessagepaginatetypedef) 
## DescribeDBSubnetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_subnet_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeDBSubnetGroups.html#RDS.Paginator.DescribeDBSubnetGroups)

```python
# DescribeDBSubnetGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeDBSubnetGroupsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeDBSubnetGroupsPaginator = client.get_paginator("describe_db_subnet_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DBSubnetGroupMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeDBSubnetGroupsPaginator](./paginators.md#describedbsubnetgroupspaginator)
3. item: [:material-code-braces: DBSubnetGroupMessageTypeDef](./type_defs.md#dbsubnetgroupmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBSubnetGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBSubnetGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DBSubnetGroupMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBSubnetGroupMessageTypeDef](./type_defs.md#dbsubnetgroupmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDBSubnetGroupsMessagePaginateTypeDef = {  # (1)
    "DBSubnetGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBSubnetGroupsMessagePaginateTypeDef](./type_defs.md#describedbsubnetgroupsmessagepaginatetypedef) 
## DescribeEngineDefaultClusterParametersPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_engine_default_cluster_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeEngineDefaultClusterParameters.html#RDS.Paginator.DescribeEngineDefaultClusterParameters)

```python
# DescribeEngineDefaultClusterParametersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeEngineDefaultClusterParametersPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeEngineDefaultClusterParametersPaginator = client.get_paginator("describe_engine_default_cluster_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEngineDefaultClusterParametersResultTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeEngineDefaultClusterParametersPaginator](./paginators.md#describeenginedefaultclusterparameterspaginator)
3. item: [:material-code-braces: DescribeEngineDefaultClusterParametersResultTypeDef](./type_defs.md#describeenginedefaultclusterparametersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEngineDefaultClusterParametersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBParameterGroupFamily: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeEngineDefaultClusterParametersResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEngineDefaultClusterParametersResultTypeDef](./type_defs.md#describeenginedefaultclusterparametersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEngineDefaultClusterParametersMessagePaginateTypeDef = {  # (1)
    "DBParameterGroupFamily": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEngineDefaultClusterParametersMessagePaginateTypeDef](./type_defs.md#describeenginedefaultclusterparametersmessagepaginatetypedef) 
## DescribeEngineDefaultParametersPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_engine_default_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeEngineDefaultParameters.html#RDS.Paginator.DescribeEngineDefaultParameters)

```python
# DescribeEngineDefaultParametersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeEngineDefaultParametersPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeEngineDefaultParametersPaginator = client.get_paginator("describe_engine_default_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEngineDefaultParametersResultTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeEngineDefaultParametersPaginator](./paginators.md#describeenginedefaultparameterspaginator)
3. item: [:material-code-braces: DescribeEngineDefaultParametersResultTypeDef](./type_defs.md#describeenginedefaultparametersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEngineDefaultParametersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBParameterGroupFamily: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeEngineDefaultParametersResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEngineDefaultParametersResultTypeDef](./type_defs.md#describeenginedefaultparametersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEngineDefaultParametersMessagePaginateTypeDef = {  # (1)
    "DBParameterGroupFamily": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEngineDefaultParametersMessagePaginateTypeDef](./type_defs.md#describeenginedefaultparametersmessagepaginatetypedef) 
## DescribeEventSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_event_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeEventSubscriptions.html#RDS.Paginator.DescribeEventSubscriptions)

```python
# DescribeEventSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeEventSubscriptionsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: EventSubscriptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeEventSubscriptionsPaginator](./paginators.md#describeeventsubscriptionspaginator)
3. item: [:material-code-braces: EventSubscriptionsMessageTypeDef](./type_defs.md#eventsubscriptionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SubscriptionName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[EventSubscriptionsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: EventSubscriptionsMessageTypeDef](./type_defs.md#eventsubscriptionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEventSubscriptionsMessagePaginateTypeDef = {  # (1)
    "SubscriptionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventSubscriptionsMessagePaginateTypeDef](./type_defs.md#describeeventsubscriptionsmessagepaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeEvents.html#RDS.Paginator.DescribeEvents)

```python
# DescribeEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")  # (2)
    async for item in paginator.paginate(...):
        item: EventsMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
3. item: [:material-code-braces: EventsMessageTypeDef](./type_defs.md#eventsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SourceIdentifier: str = ...,
    SourceType: SourceTypeType = ...,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    Duration: int = ...,
    EventCategories: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[EventsMessageTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: EventsMessageTypeDef](./type_defs.md#eventsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEventsMessagePaginateTypeDef = {  # (1)
    "SourceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsMessagePaginateTypeDef](./type_defs.md#describeeventsmessagepaginatetypedef) 
## DescribeExportTasksPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_export_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeExportTasks.html#RDS.Paginator.DescribeExportTasks)

```python
# DescribeExportTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeExportTasksPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeExportTasksPaginator = client.get_paginator("describe_export_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ExportTasksMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeExportTasksPaginator](./paginators.md#describeexporttaskspaginator)
3. item: [:material-code-braces: ExportTasksMessageTypeDef](./type_defs.md#exporttasksmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeExportTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ExportTaskIdentifier: str = ...,
    SourceArn: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SourceType: ExportSourceTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ExportTasksMessageTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: ExportSourceTypeType](./literals.md#exportsourcetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ExportTasksMessageTypeDef](./type_defs.md#exporttasksmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeExportTasksMessagePaginateTypeDef = {  # (1)
    "ExportTaskIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeExportTasksMessagePaginateTypeDef](./type_defs.md#describeexporttasksmessagepaginatetypedef) 
## DescribeGlobalClustersPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_global_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeGlobalClusters.html#RDS.Paginator.DescribeGlobalClusters)

```python
# DescribeGlobalClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeGlobalClustersPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeGlobalClustersPaginator = client.get_paginator("describe_global_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: GlobalClustersMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeGlobalClustersPaginator](./paginators.md#describeglobalclusterspaginator)
3. item: [:material-code-braces: GlobalClustersMessageTypeDef](./type_defs.md#globalclustersmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeGlobalClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GlobalClusterIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GlobalClustersMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GlobalClustersMessageTypeDef](./type_defs.md#globalclustersmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeGlobalClustersMessagePaginateTypeDef = {  # (1)
    "GlobalClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeGlobalClustersMessagePaginateTypeDef](./type_defs.md#describeglobalclustersmessagepaginatetypedef) 
## DescribeIntegrationsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_integrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeIntegrations.html#RDS.Paginator.DescribeIntegrations)

```python
# DescribeIntegrationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeIntegrationsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeIntegrationsPaginator = client.get_paginator("describe_integrations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeIntegrationsResponseTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeIntegrationsPaginator](./paginators.md#describeintegrationspaginator)
3. item: [:material-code-braces: DescribeIntegrationsResponseTypeDef](./type_defs.md#describeintegrationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeIntegrationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IntegrationIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeIntegrationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeIntegrationsResponseTypeDef](./type_defs.md#describeintegrationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeIntegrationsMessagePaginateTypeDef = {  # (1)
    "IntegrationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIntegrationsMessagePaginateTypeDef](./type_defs.md#describeintegrationsmessagepaginatetypedef) 
## DescribeOptionGroupOptionsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_option_group_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeOptionGroupOptions.html#RDS.Paginator.DescribeOptionGroupOptions)

```python
# DescribeOptionGroupOptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeOptionGroupOptionsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeOptionGroupOptionsPaginator = client.get_paginator("describe_option_group_options")  # (2)
    async for item in paginator.paginate(...):
        item: OptionGroupOptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeOptionGroupOptionsPaginator](./paginators.md#describeoptiongroupoptionspaginator)
3. item: [:material-code-braces: OptionGroupOptionsMessageTypeDef](./type_defs.md#optiongroupoptionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOptionGroupOptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    EngineName: str,
    MajorEngineVersion: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[OptionGroupOptionsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: OptionGroupOptionsMessageTypeDef](./type_defs.md#optiongroupoptionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeOptionGroupOptionsMessagePaginateTypeDef = {  # (1)
    "EngineName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOptionGroupOptionsMessagePaginateTypeDef](./type_defs.md#describeoptiongroupoptionsmessagepaginatetypedef) 
## DescribeOptionGroupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_option_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeOptionGroups.html#RDS.Paginator.DescribeOptionGroups)

```python
# DescribeOptionGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeOptionGroupsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeOptionGroupsPaginator = client.get_paginator("describe_option_groups")  # (2)
    async for item in paginator.paginate(...):
        item: OptionGroupsTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeOptionGroupsPaginator](./paginators.md#describeoptiongroupspaginator)
3. item: [:material-code-braces: OptionGroupsTypeDef](./type_defs.md#optiongroupstypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOptionGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OptionGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    EngineName: str = ...,
    MajorEngineVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[OptionGroupsTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: OptionGroupsTypeDef](./type_defs.md#optiongroupstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeOptionGroupsMessagePaginateTypeDef = {  # (1)
    "OptionGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOptionGroupsMessagePaginateTypeDef](./type_defs.md#describeoptiongroupsmessagepaginatetypedef) 
## DescribeOrderableDBInstanceOptionsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_orderable_db_instance_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeOrderableDBInstanceOptions.html#RDS.Paginator.DescribeOrderableDBInstanceOptions)

```python
# DescribeOrderableDBInstanceOptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeOrderableDBInstanceOptionsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeOrderableDBInstanceOptionsPaginator = client.get_paginator("describe_orderable_db_instance_options")  # (2)
    async for item in paginator.paginate(...):
        item: OrderableDBInstanceOptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeOrderableDBInstanceOptionsPaginator](./paginators.md#describeorderabledbinstanceoptionspaginator)
3. item: [:material-code-braces: OrderableDBInstanceOptionsMessageTypeDef](./type_defs.md#orderabledbinstanceoptionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrderableDBInstanceOptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Engine: str,
    EngineVersion: str = ...,
    DBInstanceClass: str = ...,
    LicenseModel: str = ...,
    AvailabilityZoneGroup: str = ...,
    Vpc: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[OrderableDBInstanceOptionsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: OrderableDBInstanceOptionsMessageTypeDef](./type_defs.md#orderabledbinstanceoptionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeOrderableDBInstanceOptionsMessagePaginateTypeDef = {  # (1)
    "Engine": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrderableDBInstanceOptionsMessagePaginateTypeDef](./type_defs.md#describeorderabledbinstanceoptionsmessagepaginatetypedef) 
## DescribePendingMaintenanceActionsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_pending_maintenance_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribePendingMaintenanceActions.html#RDS.Paginator.DescribePendingMaintenanceActions)

```python
# DescribePendingMaintenanceActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribePendingMaintenanceActionsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribePendingMaintenanceActionsPaginator = client.get_paginator("describe_pending_maintenance_actions")  # (2)
    async for item in paginator.paginate(...):
        item: PendingMaintenanceActionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribePendingMaintenanceActionsPaginator](./paginators.md#describependingmaintenanceactionspaginator)
3. item: [:material-code-braces: PendingMaintenanceActionsMessageTypeDef](./type_defs.md#pendingmaintenanceactionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribePendingMaintenanceActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[PendingMaintenanceActionsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: PendingMaintenanceActionsMessageTypeDef](./type_defs.md#pendingmaintenanceactionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribePendingMaintenanceActionsMessagePaginateTypeDef = {  # (1)
    "ResourceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePendingMaintenanceActionsMessagePaginateTypeDef](./type_defs.md#describependingmaintenanceactionsmessagepaginatetypedef) 
## DescribeReservedDBInstancesOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_reserved_db_instances_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeReservedDBInstancesOfferings.html#RDS.Paginator.DescribeReservedDBInstancesOfferings)

```python
# DescribeReservedDBInstancesOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeReservedDBInstancesOfferingsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeReservedDBInstancesOfferingsPaginator = client.get_paginator("describe_reserved_db_instances_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: ReservedDBInstancesOfferingMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeReservedDBInstancesOfferingsPaginator](./paginators.md#describereserveddbinstancesofferingspaginator)
3. item: [:material-code-braces: ReservedDBInstancesOfferingMessageTypeDef](./type_defs.md#reserveddbinstancesofferingmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedDBInstancesOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReservedDBInstancesOfferingId: str = ...,
    DBInstanceClass: str = ...,
    Duration: str = ...,
    ProductDescription: str = ...,
    OfferingType: str = ...,
    MultiAZ: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ReservedDBInstancesOfferingMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ReservedDBInstancesOfferingMessageTypeDef](./type_defs.md#reserveddbinstancesofferingmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReservedDBInstancesOfferingsMessagePaginateTypeDef = {  # (1)
    "ReservedDBInstancesOfferingId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedDBInstancesOfferingsMessagePaginateTypeDef](./type_defs.md#describereserveddbinstancesofferingsmessagepaginatetypedef) 
## DescribeReservedDBInstancesPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_reserved_db_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeReservedDBInstances.html#RDS.Paginator.DescribeReservedDBInstances)

```python
# DescribeReservedDBInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeReservedDBInstancesPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeReservedDBInstancesPaginator = client.get_paginator("describe_reserved_db_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ReservedDBInstanceMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeReservedDBInstancesPaginator](./paginators.md#describereserveddbinstancespaginator)
3. item: [:material-code-braces: ReservedDBInstanceMessageTypeDef](./type_defs.md#reserveddbinstancemessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedDBInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReservedDBInstanceId: str = ...,
    ReservedDBInstancesOfferingId: str = ...,
    DBInstanceClass: str = ...,
    Duration: str = ...,
    ProductDescription: str = ...,
    OfferingType: str = ...,
    MultiAZ: bool = ...,
    LeaseId: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ReservedDBInstanceMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ReservedDBInstanceMessageTypeDef](./type_defs.md#reserveddbinstancemessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReservedDBInstancesMessagePaginateTypeDef = {  # (1)
    "ReservedDBInstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedDBInstancesMessagePaginateTypeDef](./type_defs.md#describereserveddbinstancesmessagepaginatetypedef) 
## DescribeSourceRegionsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_source_regions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeSourceRegions.html#RDS.Paginator.DescribeSourceRegions)

```python
# DescribeSourceRegionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeSourceRegionsPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeSourceRegionsPaginator = client.get_paginator("describe_source_regions")  # (2)
    async for item in paginator.paginate(...):
        item: SourceRegionMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeSourceRegionsPaginator](./paginators.md#describesourceregionspaginator)
3. item: [:material-code-braces: SourceRegionMessageTypeDef](./type_defs.md#sourceregionmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSourceRegionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RegionName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[SourceRegionMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SourceRegionMessageTypeDef](./type_defs.md#sourceregionmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSourceRegionsMessagePaginateTypeDef = {  # (1)
    "RegionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSourceRegionsMessagePaginateTypeDef](./type_defs.md#describesourceregionsmessagepaginatetypedef) 
## DescribeTenantDatabasesPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_tenant_databases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DescribeTenantDatabases.html#RDS.Paginator.DescribeTenantDatabases)

```python
# DescribeTenantDatabasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DescribeTenantDatabasesPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DescribeTenantDatabasesPaginator = client.get_paginator("describe_tenant_databases")  # (2)
    async for item in paginator.paginate(...):
        item: TenantDatabasesMessageTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeTenantDatabasesPaginator](./paginators.md#describetenantdatabasespaginator)
3. item: [:material-code-braces: TenantDatabasesMessageTypeDef](./type_defs.md#tenantdatabasesmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTenantDatabasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    TenantDBName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[TenantDatabasesMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: TenantDatabasesMessageTypeDef](./type_defs.md#tenantdatabasesmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTenantDatabasesMessagePaginateTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTenantDatabasesMessagePaginateTypeDef](./type_defs.md#describetenantdatabasesmessagepaginatetypedef) 
## DownloadDBLogFilePortionPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("download_db_log_file_portion")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/paginator/DownloadDBLogFilePortion.html#RDS.Paginator.DownloadDBLogFilePortion)

```python
# DownloadDBLogFilePortionPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rds.paginator import DownloadDBLogFilePortionPaginator

session = get_session()
async with session.create_client("rds") as client:  # (1)
    paginator: DownloadDBLogFilePortionPaginator = client.get_paginator("download_db_log_file_portion")  # (2)
    async for item in paginator.paginate(...):
        item: DownloadDBLogFilePortionDetailsTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DownloadDBLogFilePortionPaginator](./paginators.md#downloaddblogfileportionpaginator)
3. item: [:material-code-braces: DownloadDBLogFilePortionDetailsTypeDef](./type_defs.md#downloaddblogfileportiondetailstypedef) 


### paginate

Type annotations and code completion for `#!python DownloadDBLogFilePortionPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DBInstanceIdentifier: str,
    LogFileName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DownloadDBLogFilePortionDetailsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DownloadDBLogFilePortionDetailsTypeDef](./type_defs.md#downloaddblogfileportiondetailstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DownloadDBLogFilePortionMessagePaginateTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
    "LogFileName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DownloadDBLogFilePortionMessagePaginateTypeDef](./type_defs.md#downloaddblogfileportionmessagepaginatetypedef) 
