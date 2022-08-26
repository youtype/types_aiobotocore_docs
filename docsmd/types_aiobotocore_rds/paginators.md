# Paginators

> [Index](../README.md) > [RDS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [RDS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
    type annotations stubs module [types-aiobotocore-rds](https://pypi.org/project/types-aiobotocore-rds/).

## DescribeCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeCertificates)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    CertificateIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[CertificateMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: CertificateMessageTypeDef](./type_defs.md#certificatemessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = {  # (1)
    "CertificateIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef](./type_defs.md#describecertificatesmessagedescribecertificatespaginatetypedef) 
## DescribeDBClusterBacktracksPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_cluster_backtracks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterBacktracks)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBClusterIdentifier: str,
    BacktrackIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBClusterBacktrackMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterBacktrackMessageTypeDef](./type_defs.md#dbclusterbacktrackmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef](./type_defs.md#describedbclusterbacktracksmessagedescribedbclusterbacktrackspaginatetypedef) 
## DescribeDBClusterEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_cluster_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterEndpoints)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBClusterIdentifier: str = ...,
    DBClusterEndpointIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBClusterEndpointMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterEndpointMessageTypeDef](./type_defs.md#dbclusterendpointmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef](./type_defs.md#describedbclusterendpointsmessagedescribedbclusterendpointspaginatetypedef) 
## DescribeDBClusterParameterGroupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_cluster_parameter_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterParameterGroups)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBClusterParameterGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBClusterParameterGroupsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterParameterGroupsMessageTypeDef](./type_defs.md#dbclusterparametergroupsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = {  # (1)
    "DBClusterParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef](./type_defs.md#describedbclusterparametergroupsmessagedescribedbclusterparametergroupspaginatetypedef) 
## DescribeDBClusterParametersPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_cluster_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterParameters)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBClusterParameterGroupName: str,
    Source: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBClusterParameterGroupDetailsTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterParameterGroupDetailsTypeDef](./type_defs.md#dbclusterparametergroupdetailstypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = {  # (1)
    "DBClusterParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef](./type_defs.md#describedbclusterparametersmessagedescribedbclusterparameterspaginatetypedef) 
## DescribeDBClusterSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_cluster_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterSnapshots)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBClusterIdentifier: str = ...,
    DBClusterSnapshotIdentifier: str = ...,
    SnapshotType: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IncludeShared: bool = ...,
    IncludePublic: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBClusterSnapshotMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterSnapshotMessageTypeDef](./type_defs.md#dbclustersnapshotmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef](./type_defs.md#describedbclustersnapshotsmessagedescribedbclustersnapshotspaginatetypedef) 
## DescribeDBClustersPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusters)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBClusterIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IncludeShared: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBClusterMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterMessageTypeDef](./type_defs.md#dbclustermessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef](./type_defs.md#describedbclustersmessagedescribedbclusterspaginatetypedef) 
## DescribeDBEngineVersionsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_engine_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBEngineVersions)

```python title="Usage example"
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

```python title="Method definition"
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
) -> AsyncIterator[DBEngineVersionMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBEngineVersionMessageTypeDef](./type_defs.md#dbengineversionmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = {  # (1)
    "Engine": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef](./type_defs.md#describedbengineversionsmessagedescribedbengineversionspaginatetypedef) 
## DescribeDBInstanceAutomatedBackupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_instance_automated_backups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBInstanceAutomatedBackups)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DbiResourceId: str = ...,
    DBInstanceIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DBInstanceAutomatedBackupsArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBInstanceAutomatedBackupMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBInstanceAutomatedBackupMessageTypeDef](./type_defs.md#dbinstanceautomatedbackupmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBInstanceAutomatedBackupsMessageDescribeDBInstanceAutomatedBackupsPaginateTypeDef = {  # (1)
    "DbiResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBInstanceAutomatedBackupsMessageDescribeDBInstanceAutomatedBackupsPaginateTypeDef](./type_defs.md#describedbinstanceautomatedbackupsmessagedescribedbinstanceautomatedbackupspaginatetypedef) 
## DescribeDBInstancesPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBInstances)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBInstanceMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBInstanceMessageTypeDef](./type_defs.md#dbinstancemessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef](./type_defs.md#describedbinstancesmessagedescribedbinstancespaginatetypedef) 
## DescribeDBLogFilesPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_log_files")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBLogFiles)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBInstanceIdentifier: str,
    FilenameContains: str = ...,
    FileLastWritten: int = ...,
    FileSize: int = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeDBLogFilesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDBLogFilesResponseTypeDef](./type_defs.md#describedblogfilesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef](./type_defs.md#describedblogfilesmessagedescribedblogfilespaginatetypedef) 
## DescribeDBParameterGroupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_parameter_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBParameterGroups)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBParameterGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBParameterGroupsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBParameterGroupsMessageTypeDef](./type_defs.md#dbparametergroupsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = {  # (1)
    "DBParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef](./type_defs.md#describedbparametergroupsmessagedescribedbparametergroupspaginatetypedef) 
## DescribeDBParametersPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBParameters)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBParameterGroupName: str,
    Source: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBParameterGroupDetailsTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBParameterGroupDetailsTypeDef](./type_defs.md#dbparametergroupdetailstypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = {  # (1)
    "DBParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef](./type_defs.md#describedbparametersmessagedescribedbparameterspaginatetypedef) 
## DescribeDBProxiesPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_proxies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBProxies)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBProxyName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeDBProxiesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDBProxiesResponseTypeDef](./type_defs.md#describedbproxiesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBProxiesRequestDescribeDBProxiesPaginateTypeDef = {  # (1)
    "DBProxyName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBProxiesRequestDescribeDBProxiesPaginateTypeDef](./type_defs.md#describedbproxiesrequestdescribedbproxiespaginatetypedef) 
## DescribeDBProxyEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_proxy_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBProxyEndpoints)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBProxyName: str = ...,
    DBProxyEndpointName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeDBProxyEndpointsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDBProxyEndpointsResponseTypeDef](./type_defs.md#describedbproxyendpointsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBProxyEndpointsRequestDescribeDBProxyEndpointsPaginateTypeDef = {  # (1)
    "DBProxyName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBProxyEndpointsRequestDescribeDBProxyEndpointsPaginateTypeDef](./type_defs.md#describedbproxyendpointsrequestdescribedbproxyendpointspaginatetypedef) 
## DescribeDBProxyTargetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_proxy_target_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBProxyTargetGroups)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBProxyName: str,
    TargetGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeDBProxyTargetGroupsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDBProxyTargetGroupsResponseTypeDef](./type_defs.md#describedbproxytargetgroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef = {  # (1)
    "DBProxyName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef](./type_defs.md#describedbproxytargetgroupsrequestdescribedbproxytargetgroupspaginatetypedef) 
## DescribeDBProxyTargetsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_proxy_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBProxyTargets)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBProxyName: str,
    TargetGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeDBProxyTargetsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDBProxyTargetsResponseTypeDef](./type_defs.md#describedbproxytargetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef = {  # (1)
    "DBProxyName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef](./type_defs.md#describedbproxytargetsrequestdescribedbproxytargetspaginatetypedef) 
## DescribeDBSecurityGroupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_security_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBSecurityGroups)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBSecurityGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBSecurityGroupMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBSecurityGroupMessageTypeDef](./type_defs.md#dbsecuritygroupmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBSecurityGroupsMessageDescribeDBSecurityGroupsPaginateTypeDef = {  # (1)
    "DBSecurityGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBSecurityGroupsMessageDescribeDBSecurityGroupsPaginateTypeDef](./type_defs.md#describedbsecuritygroupsmessagedescribedbsecuritygroupspaginatetypedef) 
## DescribeDBSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBSnapshots)

```python title="Usage example"
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

```python title="Method definition"
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
) -> AsyncIterator[DBSnapshotMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBSnapshotMessageTypeDef](./type_defs.md#dbsnapshotmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBSnapshotsMessageDescribeDBSnapshotsPaginateTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBSnapshotsMessageDescribeDBSnapshotsPaginateTypeDef](./type_defs.md#describedbsnapshotsmessagedescribedbsnapshotspaginatetypedef) 
## DescribeDBSubnetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_db_subnet_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBSubnetGroups)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBSubnetGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBSubnetGroupMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBSubnetGroupMessageTypeDef](./type_defs.md#dbsubnetgroupmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = {  # (1)
    "DBSubnetGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef](./type_defs.md#describedbsubnetgroupsmessagedescribedbsubnetgroupspaginatetypedef) 
## DescribeEngineDefaultClusterParametersPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_engine_default_cluster_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEngineDefaultClusterParameters)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBParameterGroupFamily: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEngineDefaultClusterParametersResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEngineDefaultClusterParametersResultTypeDef](./type_defs.md#describeenginedefaultclusterparametersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef = {  # (1)
    "DBParameterGroupFamily": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef](./type_defs.md#describeenginedefaultclusterparametersmessagedescribeenginedefaultclusterparameterspaginatetypedef) 
## DescribeEngineDefaultParametersPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_engine_default_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEngineDefaultParameters)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBParameterGroupFamily: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEngineDefaultParametersResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEngineDefaultParametersResultTypeDef](./type_defs.md#describeenginedefaultparametersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = {  # (1)
    "DBParameterGroupFamily": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef](./type_defs.md#describeenginedefaultparametersmessagedescribeenginedefaultparameterspaginatetypedef) 
## DescribeEventSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_event_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEventSubscriptions)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    SubscriptionName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: EventSubscriptionsMessageTypeDef](./type_defs.md#eventsubscriptionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = {  # (1)
    "SubscriptionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef](./type_defs.md#describeeventsubscriptionsmessagedescribeeventsubscriptionspaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEvents)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    SourceIdentifier: str = ...,
    SourceType: SourceTypeType = ...,  # (1)
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    Duration: int = ...,
    EventCategories: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[EventsMessageTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: EventsMessageTypeDef](./type_defs.md#eventsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventsMessageDescribeEventsPaginateTypeDef = {  # (1)
    "SourceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsMessageDescribeEventsPaginateTypeDef](./type_defs.md#describeeventsmessagedescribeeventspaginatetypedef) 
## DescribeExportTasksPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_export_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeExportTasks)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    ExportTaskIdentifier: str = ...,
    SourceArn: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ExportTasksMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ExportTasksMessageTypeDef](./type_defs.md#exporttasksmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeExportTasksMessageDescribeExportTasksPaginateTypeDef = {  # (1)
    "ExportTaskIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeExportTasksMessageDescribeExportTasksPaginateTypeDef](./type_defs.md#describeexporttasksmessagedescribeexporttaskspaginatetypedef) 
## DescribeGlobalClustersPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_global_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeGlobalClusters)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalClusterIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GlobalClustersMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GlobalClustersMessageTypeDef](./type_defs.md#globalclustersmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = {  # (1)
    "GlobalClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef](./type_defs.md#describeglobalclustersmessagedescribeglobalclusterspaginatetypedef) 
## DescribeOptionGroupOptionsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_option_group_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeOptionGroupOptions)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    EngineName: str,
    MajorEngineVersion: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[OptionGroupOptionsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: OptionGroupOptionsMessageTypeDef](./type_defs.md#optiongroupoptionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef = {  # (1)
    "EngineName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef](./type_defs.md#describeoptiongroupoptionsmessagedescribeoptiongroupoptionspaginatetypedef) 
## DescribeOptionGroupsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_option_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeOptionGroups)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    OptionGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    EngineName: str = ...,
    MajorEngineVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[OptionGroupsTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: OptionGroupsTypeDef](./type_defs.md#optiongroupstypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeOptionGroupsMessageDescribeOptionGroupsPaginateTypeDef = {  # (1)
    "OptionGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOptionGroupsMessageDescribeOptionGroupsPaginateTypeDef](./type_defs.md#describeoptiongroupsmessagedescribeoptiongroupspaginatetypedef) 
## DescribeOrderableDBInstanceOptionsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_orderable_db_instance_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeOrderableDBInstanceOptions)

```python title="Usage example"
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

```python title="Method definition"
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
) -> AsyncIterator[OrderableDBInstanceOptionsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: OrderableDBInstanceOptionsMessageTypeDef](./type_defs.md#orderabledbinstanceoptionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = {  # (1)
    "Engine": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef](./type_defs.md#describeorderabledbinstanceoptionsmessagedescribeorderabledbinstanceoptionspaginatetypedef) 
## DescribePendingMaintenanceActionsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_pending_maintenance_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribePendingMaintenanceActions)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[PendingMaintenanceActionsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: PendingMaintenanceActionsMessageTypeDef](./type_defs.md#pendingmaintenanceactionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = {  # (1)
    "ResourceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef](./type_defs.md#describependingmaintenanceactionsmessagedescribependingmaintenanceactionspaginatetypedef) 
## DescribeReservedDBInstancesPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_reserved_db_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeReservedDBInstances)

```python title="Usage example"
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

```python title="Method definition"
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
) -> AsyncIterator[ReservedDBInstanceMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ReservedDBInstanceMessageTypeDef](./type_defs.md#reserveddbinstancemessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReservedDBInstancesMessageDescribeReservedDBInstancesPaginateTypeDef = {  # (1)
    "ReservedDBInstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedDBInstancesMessageDescribeReservedDBInstancesPaginateTypeDef](./type_defs.md#describereserveddbinstancesmessagedescribereserveddbinstancespaginatetypedef) 
## DescribeReservedDBInstancesOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_reserved_db_instances_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeReservedDBInstancesOfferings)

```python title="Usage example"
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

```python title="Method definition"
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
) -> AsyncIterator[ReservedDBInstancesOfferingMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ReservedDBInstancesOfferingMessageTypeDef](./type_defs.md#reserveddbinstancesofferingmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReservedDBInstancesOfferingsMessageDescribeReservedDBInstancesOfferingsPaginateTypeDef = {  # (1)
    "ReservedDBInstancesOfferingId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedDBInstancesOfferingsMessageDescribeReservedDBInstancesOfferingsPaginateTypeDef](./type_defs.md#describereserveddbinstancesofferingsmessagedescribereserveddbinstancesofferingspaginatetypedef) 
## DescribeSourceRegionsPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("describe_source_regions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeSourceRegions)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    RegionName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SourceRegionMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SourceRegionMessageTypeDef](./type_defs.md#sourceregionmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSourceRegionsMessageDescribeSourceRegionsPaginateTypeDef = {  # (1)
    "RegionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSourceRegionsMessageDescribeSourceRegionsPaginateTypeDef](./type_defs.md#describesourceregionsmessagedescribesourceregionspaginatetypedef) 
## DownloadDBLogFilePortionPaginator

Type annotations and code completion for `#!python session.create_client("rds").get_paginator("download_db_log_file_portion")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DownloadDBLogFilePortion)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DBInstanceIdentifier: str,
    LogFileName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DownloadDBLogFilePortionDetailsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DownloadDBLogFilePortionDetailsTypeDef](./type_defs.md#downloaddblogfileportiondetailstypedef) 


```python title="Usage example with kwargs"
kwargs: DownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
    "LogFileName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef](./type_defs.md#downloaddblogfileportionmessagedownloaddblogfileportionpaginatetypedef) 
