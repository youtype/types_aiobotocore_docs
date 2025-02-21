# Paginators

> [Index](../README.md) > [Redshift](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Redshift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#redshift)
    type annotations stubs module [types-aiobotocore-redshift](https://pypi.org/project/types-aiobotocore-redshift/).

## DescribeClusterDbRevisionsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_cluster_db_revisions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeClusterDbRevisions.html#Redshift.Paginator.DescribeClusterDbRevisions)

```python
# DescribeClusterDbRevisionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeClusterDbRevisionsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeClusterDbRevisionsPaginator = client.get_paginator("describe_cluster_db_revisions")  # (2)
    async for item in paginator.paginate(...):
        item: ClusterDbRevisionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterDbRevisionsPaginator](./paginators.md#describeclusterdbrevisionspaginator)
3. item: [:material-code-braces: ClusterDbRevisionsMessageTypeDef](./type_defs.md#clusterdbrevisionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterDbRevisionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ClusterDbRevisionsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClusterDbRevisionsMessageTypeDef](./type_defs.md#clusterdbrevisionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClusterDbRevisionsMessagePaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterDbRevisionsMessagePaginateTypeDef](./type_defs.md#describeclusterdbrevisionsmessagepaginatetypedef) 
## DescribeClusterParameterGroupsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_cluster_parameter_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeClusterParameterGroups.html#Redshift.Paginator.DescribeClusterParameterGroups)

```python
# DescribeClusterParameterGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeClusterParameterGroupsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeClusterParameterGroupsPaginator = client.get_paginator("describe_cluster_parameter_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ClusterParameterGroupsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterParameterGroupsPaginator](./paginators.md#describeclusterparametergroupspaginator)
3. item: [:material-code-braces: ClusterParameterGroupsMessageTypeDef](./type_defs.md#clusterparametergroupsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterParameterGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ParameterGroupName: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ClusterParameterGroupsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClusterParameterGroupsMessageTypeDef](./type_defs.md#clusterparametergroupsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClusterParameterGroupsMessagePaginateTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterParameterGroupsMessagePaginateTypeDef](./type_defs.md#describeclusterparametergroupsmessagepaginatetypedef) 
## DescribeClusterParametersPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_cluster_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeClusterParameters.html#Redshift.Paginator.DescribeClusterParameters)

```python
# DescribeClusterParametersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeClusterParametersPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeClusterParametersPaginator = client.get_paginator("describe_cluster_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: ClusterParameterGroupDetailsTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterParametersPaginator](./paginators.md#describeclusterparameterspaginator)
3. item: [:material-code-braces: ClusterParameterGroupDetailsTypeDef](./type_defs.md#clusterparametergroupdetailstypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterParametersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ParameterGroupName: str,
    Source: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ClusterParameterGroupDetailsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClusterParameterGroupDetailsTypeDef](./type_defs.md#clusterparametergroupdetailstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClusterParametersMessagePaginateTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterParametersMessagePaginateTypeDef](./type_defs.md#describeclusterparametersmessagepaginatetypedef) 
## DescribeClusterSecurityGroupsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_cluster_security_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeClusterSecurityGroups.html#Redshift.Paginator.DescribeClusterSecurityGroups)

```python
# DescribeClusterSecurityGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeClusterSecurityGroupsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeClusterSecurityGroupsPaginator = client.get_paginator("describe_cluster_security_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ClusterSecurityGroupMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterSecurityGroupsPaginator](./paginators.md#describeclustersecuritygroupspaginator)
3. item: [:material-code-braces: ClusterSecurityGroupMessageTypeDef](./type_defs.md#clustersecuritygroupmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterSecurityGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterSecurityGroupName: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ClusterSecurityGroupMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClusterSecurityGroupMessageTypeDef](./type_defs.md#clustersecuritygroupmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClusterSecurityGroupsMessagePaginateTypeDef = {  # (1)
    "ClusterSecurityGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterSecurityGroupsMessagePaginateTypeDef](./type_defs.md#describeclustersecuritygroupsmessagepaginatetypedef) 
## DescribeClusterSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_cluster_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeClusterSnapshots.html#Redshift.Paginator.DescribeClusterSnapshots)

```python
# DescribeClusterSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeClusterSnapshotsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeClusterSnapshotsPaginator = client.get_paginator("describe_cluster_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: SnapshotMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterSnapshotsPaginator](./paginators.md#describeclustersnapshotspaginator)
3. item: [:material-code-braces: SnapshotMessageTypeDef](./type_defs.md#snapshotmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    SnapshotIdentifier: str = ...,
    SnapshotArn: str = ...,
    SnapshotType: str = ...,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    OwnerAccount: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    ClusterExists: bool = ...,
    SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[SnapshotMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SnapshotSortingEntityTypeDef](./type_defs.md#snapshotsortingentitytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SnapshotMessageTypeDef](./type_defs.md#snapshotmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClusterSnapshotsMessagePaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterSnapshotsMessagePaginateTypeDef](./type_defs.md#describeclustersnapshotsmessagepaginatetypedef) 
## DescribeClusterSubnetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_cluster_subnet_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeClusterSubnetGroups.html#Redshift.Paginator.DescribeClusterSubnetGroups)

```python
# DescribeClusterSubnetGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeClusterSubnetGroupsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeClusterSubnetGroupsPaginator = client.get_paginator("describe_cluster_subnet_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ClusterSubnetGroupMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterSubnetGroupsPaginator](./paginators.md#describeclustersubnetgroupspaginator)
3. item: [:material-code-braces: ClusterSubnetGroupMessageTypeDef](./type_defs.md#clustersubnetgroupmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterSubnetGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterSubnetGroupName: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ClusterSubnetGroupMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClusterSubnetGroupMessageTypeDef](./type_defs.md#clustersubnetgroupmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClusterSubnetGroupsMessagePaginateTypeDef = {  # (1)
    "ClusterSubnetGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterSubnetGroupsMessagePaginateTypeDef](./type_defs.md#describeclustersubnetgroupsmessagepaginatetypedef) 
## DescribeClusterTracksPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_cluster_tracks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeClusterTracks.html#Redshift.Paginator.DescribeClusterTracks)

```python
# DescribeClusterTracksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeClusterTracksPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeClusterTracksPaginator = client.get_paginator("describe_cluster_tracks")  # (2)
    async for item in paginator.paginate(...):
        item: TrackListMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterTracksPaginator](./paginators.md#describeclustertrackspaginator)
3. item: [:material-code-braces: TrackListMessageTypeDef](./type_defs.md#tracklistmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterTracksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    MaintenanceTrackName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[TrackListMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: TrackListMessageTypeDef](./type_defs.md#tracklistmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClusterTracksMessagePaginateTypeDef = {  # (1)
    "MaintenanceTrackName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterTracksMessagePaginateTypeDef](./type_defs.md#describeclustertracksmessagepaginatetypedef) 
## DescribeClusterVersionsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_cluster_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeClusterVersions.html#Redshift.Paginator.DescribeClusterVersions)

```python
# DescribeClusterVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeClusterVersionsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeClusterVersionsPaginator = client.get_paginator("describe_cluster_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ClusterVersionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterVersionsPaginator](./paginators.md#describeclusterversionspaginator)
3. item: [:material-code-braces: ClusterVersionsMessageTypeDef](./type_defs.md#clusterversionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterVersion: str = ...,
    ClusterParameterGroupFamily: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ClusterVersionsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClusterVersionsMessageTypeDef](./type_defs.md#clusterversionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClusterVersionsMessagePaginateTypeDef = {  # (1)
    "ClusterVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterVersionsMessagePaginateTypeDef](./type_defs.md#describeclusterversionsmessagepaginatetypedef) 
## DescribeClustersPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeClusters.html#Redshift.Paginator.DescribeClusters)

```python
# DescribeClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeClustersPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ClustersMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClustersPaginator](./paginators.md#describeclusterspaginator)
3. item: [:material-code-braces: ClustersMessageTypeDef](./type_defs.md#clustersmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ClustersMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClustersMessageTypeDef](./type_defs.md#clustersmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClustersMessagePaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClustersMessagePaginateTypeDef](./type_defs.md#describeclustersmessagepaginatetypedef) 
## DescribeCustomDomainAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_custom_domain_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeCustomDomainAssociations.html#Redshift.Paginator.DescribeCustomDomainAssociations)

```python
# DescribeCustomDomainAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeCustomDomainAssociationsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeCustomDomainAssociationsPaginator = client.get_paginator("describe_custom_domain_associations")  # (2)
    async for item in paginator.paginate(...):
        item: CustomDomainAssociationsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeCustomDomainAssociationsPaginator](./paginators.md#describecustomdomainassociationspaginator)
3. item: [:material-code-braces: CustomDomainAssociationsMessageTypeDef](./type_defs.md#customdomainassociationsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCustomDomainAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CustomDomainName: str = ...,
    CustomDomainCertificateArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[CustomDomainAssociationsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: CustomDomainAssociationsMessageTypeDef](./type_defs.md#customdomainassociationsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCustomDomainAssociationsMessagePaginateTypeDef = {  # (1)
    "CustomDomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCustomDomainAssociationsMessagePaginateTypeDef](./type_defs.md#describecustomdomainassociationsmessagepaginatetypedef) 
## DescribeDataSharesForConsumerPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_data_shares_for_consumer")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeDataSharesForConsumer.html#Redshift.Paginator.DescribeDataSharesForConsumer)

```python
# DescribeDataSharesForConsumerPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeDataSharesForConsumerPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeDataSharesForConsumerPaginator = client.get_paginator("describe_data_shares_for_consumer")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDataSharesForConsumerResultTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeDataSharesForConsumerPaginator](./paginators.md#describedatasharesforconsumerpaginator)
3. item: [:material-code-braces: DescribeDataSharesForConsumerResultTypeDef](./type_defs.md#describedatasharesforconsumerresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDataSharesForConsumerPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConsumerArn: str = ...,
    Status: DataShareStatusForConsumerType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeDataSharesForConsumerResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DataShareStatusForConsumerType](./literals.md#datasharestatusforconsumertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDataSharesForConsumerResultTypeDef](./type_defs.md#describedatasharesforconsumerresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDataSharesForConsumerMessagePaginateTypeDef = {  # (1)
    "ConsumerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDataSharesForConsumerMessagePaginateTypeDef](./type_defs.md#describedatasharesforconsumermessagepaginatetypedef) 
## DescribeDataSharesForProducerPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_data_shares_for_producer")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeDataSharesForProducer.html#Redshift.Paginator.DescribeDataSharesForProducer)

```python
# DescribeDataSharesForProducerPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeDataSharesForProducerPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeDataSharesForProducerPaginator = client.get_paginator("describe_data_shares_for_producer")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDataSharesForProducerResultTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeDataSharesForProducerPaginator](./paginators.md#describedatasharesforproducerpaginator)
3. item: [:material-code-braces: DescribeDataSharesForProducerResultTypeDef](./type_defs.md#describedatasharesforproducerresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDataSharesForProducerPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProducerArn: str = ...,
    Status: DataShareStatusForProducerType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeDataSharesForProducerResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DataShareStatusForProducerType](./literals.md#datasharestatusforproducertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDataSharesForProducerResultTypeDef](./type_defs.md#describedatasharesforproducerresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDataSharesForProducerMessagePaginateTypeDef = {  # (1)
    "ProducerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDataSharesForProducerMessagePaginateTypeDef](./type_defs.md#describedatasharesforproducermessagepaginatetypedef) 
## DescribeDataSharesPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_data_shares")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeDataShares.html#Redshift.Paginator.DescribeDataShares)

```python
# DescribeDataSharesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeDataSharesPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeDataSharesPaginator = client.get_paginator("describe_data_shares")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDataSharesResultTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeDataSharesPaginator](./paginators.md#describedatasharespaginator)
3. item: [:material-code-braces: DescribeDataSharesResultTypeDef](./type_defs.md#describedatasharesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDataSharesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DataShareArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeDataSharesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDataSharesResultTypeDef](./type_defs.md#describedatasharesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDataSharesMessagePaginateTypeDef = {  # (1)
    "DataShareArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDataSharesMessagePaginateTypeDef](./type_defs.md#describedatasharesmessagepaginatetypedef) 
## DescribeDefaultClusterParametersPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_default_cluster_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeDefaultClusterParameters.html#Redshift.Paginator.DescribeDefaultClusterParameters)

```python
# DescribeDefaultClusterParametersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeDefaultClusterParametersPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeDefaultClusterParametersPaginator = client.get_paginator("describe_default_cluster_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDefaultClusterParametersResultTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeDefaultClusterParametersPaginator](./paginators.md#describedefaultclusterparameterspaginator)
3. item: [:material-code-braces: DescribeDefaultClusterParametersResultTypeDef](./type_defs.md#describedefaultclusterparametersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDefaultClusterParametersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ParameterGroupFamily: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeDefaultClusterParametersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDefaultClusterParametersResultTypeDef](./type_defs.md#describedefaultclusterparametersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDefaultClusterParametersMessagePaginateTypeDef = {  # (1)
    "ParameterGroupFamily": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDefaultClusterParametersMessagePaginateTypeDef](./type_defs.md#describedefaultclusterparametersmessagepaginatetypedef) 
## DescribeEndpointAccessPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_endpoint_access")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeEndpointAccess.html#Redshift.Paginator.DescribeEndpointAccess)

```python
# DescribeEndpointAccessPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeEndpointAccessPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeEndpointAccessPaginator = client.get_paginator("describe_endpoint_access")  # (2)
    async for item in paginator.paginate(...):
        item: EndpointAccessListTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeEndpointAccessPaginator](./paginators.md#describeendpointaccesspaginator)
3. item: [:material-code-braces: EndpointAccessListTypeDef](./type_defs.md#endpointaccesslisttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEndpointAccessPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    ResourceOwner: str = ...,
    EndpointName: str = ...,
    VpcId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[EndpointAccessListTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: EndpointAccessListTypeDef](./type_defs.md#endpointaccesslisttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEndpointAccessMessagePaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointAccessMessagePaginateTypeDef](./type_defs.md#describeendpointaccessmessagepaginatetypedef) 
## DescribeEndpointAuthorizationPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_endpoint_authorization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeEndpointAuthorization.html#Redshift.Paginator.DescribeEndpointAuthorization)

```python
# DescribeEndpointAuthorizationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeEndpointAuthorizationPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeEndpointAuthorizationPaginator = client.get_paginator("describe_endpoint_authorization")  # (2)
    async for item in paginator.paginate(...):
        item: EndpointAuthorizationListTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeEndpointAuthorizationPaginator](./paginators.md#describeendpointauthorizationpaginator)
3. item: [:material-code-braces: EndpointAuthorizationListTypeDef](./type_defs.md#endpointauthorizationlisttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEndpointAuthorizationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    Account: str = ...,
    Grantee: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[EndpointAuthorizationListTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: EndpointAuthorizationListTypeDef](./type_defs.md#endpointauthorizationlisttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEndpointAuthorizationMessagePaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointAuthorizationMessagePaginateTypeDef](./type_defs.md#describeendpointauthorizationmessagepaginatetypedef) 
## DescribeEventSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_event_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeEventSubscriptions.html#Redshift.Paginator.DescribeEventSubscriptions)

```python
# DescribeEventSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeEventSubscriptionsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: EventSubscriptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
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
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[EventSubscriptionsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: EventSubscriptionsMessageTypeDef](./type_defs.md#eventsubscriptionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEventSubscriptionsMessagePaginateTypeDef = {  # (1)
    "SubscriptionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventSubscriptionsMessagePaginateTypeDef](./type_defs.md#describeeventsubscriptionsmessagepaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeEvents.html#Redshift.Paginator.DescribeEvents)

```python
# DescribeEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")  # (2)
    async for item in paginator.paginate(...):
        item: EventsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
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
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[EventsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: EventsMessageTypeDef](./type_defs.md#eventsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEventsMessagePaginateTypeDef = {  # (1)
    "SourceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsMessagePaginateTypeDef](./type_defs.md#describeeventsmessagepaginatetypedef) 
## DescribeHsmClientCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_hsm_client_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeHsmClientCertificates.html#Redshift.Paginator.DescribeHsmClientCertificates)

```python
# DescribeHsmClientCertificatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeHsmClientCertificatesPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeHsmClientCertificatesPaginator = client.get_paginator("describe_hsm_client_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: HsmClientCertificateMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeHsmClientCertificatesPaginator](./paginators.md#describehsmclientcertificatespaginator)
3. item: [:material-code-braces: HsmClientCertificateMessageTypeDef](./type_defs.md#hsmclientcertificatemessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeHsmClientCertificatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    HsmClientCertificateIdentifier: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[HsmClientCertificateMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: HsmClientCertificateMessageTypeDef](./type_defs.md#hsmclientcertificatemessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeHsmClientCertificatesMessagePaginateTypeDef = {  # (1)
    "HsmClientCertificateIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeHsmClientCertificatesMessagePaginateTypeDef](./type_defs.md#describehsmclientcertificatesmessagepaginatetypedef) 
## DescribeHsmConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_hsm_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeHsmConfigurations.html#Redshift.Paginator.DescribeHsmConfigurations)

```python
# DescribeHsmConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeHsmConfigurationsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeHsmConfigurationsPaginator = client.get_paginator("describe_hsm_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: HsmConfigurationMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeHsmConfigurationsPaginator](./paginators.md#describehsmconfigurationspaginator)
3. item: [:material-code-braces: HsmConfigurationMessageTypeDef](./type_defs.md#hsmconfigurationmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeHsmConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    HsmConfigurationIdentifier: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[HsmConfigurationMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: HsmConfigurationMessageTypeDef](./type_defs.md#hsmconfigurationmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeHsmConfigurationsMessagePaginateTypeDef = {  # (1)
    "HsmConfigurationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeHsmConfigurationsMessagePaginateTypeDef](./type_defs.md#describehsmconfigurationsmessagepaginatetypedef) 
## DescribeInboundIntegrationsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_inbound_integrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeInboundIntegrations.html#Redshift.Paginator.DescribeInboundIntegrations)

```python
# DescribeInboundIntegrationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeInboundIntegrationsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeInboundIntegrationsPaginator = client.get_paginator("describe_inbound_integrations")  # (2)
    async for item in paginator.paginate(...):
        item: InboundIntegrationsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeInboundIntegrationsPaginator](./paginators.md#describeinboundintegrationspaginator)
3. item: [:material-code-braces: InboundIntegrationsMessageTypeDef](./type_defs.md#inboundintegrationsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeInboundIntegrationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IntegrationArn: str = ...,
    TargetArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[InboundIntegrationsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: InboundIntegrationsMessageTypeDef](./type_defs.md#inboundintegrationsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeInboundIntegrationsMessagePaginateTypeDef = {  # (1)
    "IntegrationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInboundIntegrationsMessagePaginateTypeDef](./type_defs.md#describeinboundintegrationsmessagepaginatetypedef) 
## DescribeIntegrationsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_integrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeIntegrations.html#Redshift.Paginator.DescribeIntegrations)

```python
# DescribeIntegrationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeIntegrationsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeIntegrationsPaginator = client.get_paginator("describe_integrations")  # (2)
    async for item in paginator.paginate(...):
        item: IntegrationsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeIntegrationsPaginator](./paginators.md#describeintegrationspaginator)
3. item: [:material-code-braces: IntegrationsMessageTypeDef](./type_defs.md#integrationsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeIntegrationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IntegrationArn: str = ...,
    Filters: Sequence[DescribeIntegrationsFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[IntegrationsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DescribeIntegrationsFilterTypeDef](./type_defs.md#describeintegrationsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: IntegrationsMessageTypeDef](./type_defs.md#integrationsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeIntegrationsMessagePaginateTypeDef = {  # (1)
    "IntegrationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIntegrationsMessagePaginateTypeDef](./type_defs.md#describeintegrationsmessagepaginatetypedef) 
## DescribeNodeConfigurationOptionsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_node_configuration_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeNodeConfigurationOptions.html#Redshift.Paginator.DescribeNodeConfigurationOptions)

```python
# DescribeNodeConfigurationOptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeNodeConfigurationOptionsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeNodeConfigurationOptionsPaginator = client.get_paginator("describe_node_configuration_options")  # (2)
    async for item in paginator.paginate(...):
        item: NodeConfigurationOptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeNodeConfigurationOptionsPaginator](./paginators.md#describenodeconfigurationoptionspaginator)
3. item: [:material-code-braces: NodeConfigurationOptionsMessageTypeDef](./type_defs.md#nodeconfigurationoptionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeNodeConfigurationOptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ActionType: ActionTypeType,  # (1)
    ClusterIdentifier: str = ...,
    SnapshotIdentifier: str = ...,
    SnapshotArn: str = ...,
    OwnerAccount: str = ...,
    Filters: Sequence[NodeConfigurationOptionsFilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[NodeConfigurationOptionsMessageTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-braces: NodeConfigurationOptionsFilterTypeDef](./type_defs.md#nodeconfigurationoptionsfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: NodeConfigurationOptionsMessageTypeDef](./type_defs.md#nodeconfigurationoptionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeNodeConfigurationOptionsMessagePaginateTypeDef = {  # (1)
    "ActionType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNodeConfigurationOptionsMessagePaginateTypeDef](./type_defs.md#describenodeconfigurationoptionsmessagepaginatetypedef) 
## DescribeOrderableClusterOptionsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_orderable_cluster_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeOrderableClusterOptions.html#Redshift.Paginator.DescribeOrderableClusterOptions)

```python
# DescribeOrderableClusterOptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeOrderableClusterOptionsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeOrderableClusterOptionsPaginator = client.get_paginator("describe_orderable_cluster_options")  # (2)
    async for item in paginator.paginate(...):
        item: OrderableClusterOptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeOrderableClusterOptionsPaginator](./paginators.md#describeorderableclusteroptionspaginator)
3. item: [:material-code-braces: OrderableClusterOptionsMessageTypeDef](./type_defs.md#orderableclusteroptionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrderableClusterOptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterVersion: str = ...,
    NodeType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[OrderableClusterOptionsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: OrderableClusterOptionsMessageTypeDef](./type_defs.md#orderableclusteroptionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeOrderableClusterOptionsMessagePaginateTypeDef = {  # (1)
    "ClusterVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrderableClusterOptionsMessagePaginateTypeDef](./type_defs.md#describeorderableclusteroptionsmessagepaginatetypedef) 
## DescribeRedshiftIdcApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_redshift_idc_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeRedshiftIdcApplications.html#Redshift.Paginator.DescribeRedshiftIdcApplications)

```python
# DescribeRedshiftIdcApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeRedshiftIdcApplicationsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeRedshiftIdcApplicationsPaginator = client.get_paginator("describe_redshift_idc_applications")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRedshiftIdcApplicationsResultTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeRedshiftIdcApplicationsPaginator](./paginators.md#describeredshiftidcapplicationspaginator)
3. item: [:material-code-braces: DescribeRedshiftIdcApplicationsResultTypeDef](./type_defs.md#describeredshiftidcapplicationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRedshiftIdcApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RedshiftIdcApplicationArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeRedshiftIdcApplicationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRedshiftIdcApplicationsResultTypeDef](./type_defs.md#describeredshiftidcapplicationsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRedshiftIdcApplicationsMessagePaginateTypeDef = {  # (1)
    "RedshiftIdcApplicationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRedshiftIdcApplicationsMessagePaginateTypeDef](./type_defs.md#describeredshiftidcapplicationsmessagepaginatetypedef) 
## DescribeReservedNodeExchangeStatusPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_reserved_node_exchange_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeReservedNodeExchangeStatus.html#Redshift.Paginator.DescribeReservedNodeExchangeStatus)

```python
# DescribeReservedNodeExchangeStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeReservedNodeExchangeStatusPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeReservedNodeExchangeStatusPaginator = client.get_paginator("describe_reserved_node_exchange_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReservedNodeExchangeStatusOutputMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeReservedNodeExchangeStatusPaginator](./paginators.md#describereservednodeexchangestatuspaginator)
3. item: [:material-code-braces: DescribeReservedNodeExchangeStatusOutputMessageTypeDef](./type_defs.md#describereservednodeexchangestatusoutputmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedNodeExchangeStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReservedNodeId: str = ...,
    ReservedNodeExchangeRequestId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeReservedNodeExchangeStatusOutputMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReservedNodeExchangeStatusOutputMessageTypeDef](./type_defs.md#describereservednodeexchangestatusoutputmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReservedNodeExchangeStatusInputMessagePaginateTypeDef = {  # (1)
    "ReservedNodeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedNodeExchangeStatusInputMessagePaginateTypeDef](./type_defs.md#describereservednodeexchangestatusinputmessagepaginatetypedef) 
## DescribeReservedNodeOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_reserved_node_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeReservedNodeOfferings.html#Redshift.Paginator.DescribeReservedNodeOfferings)

```python
# DescribeReservedNodeOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeReservedNodeOfferingsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeReservedNodeOfferingsPaginator = client.get_paginator("describe_reserved_node_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: ReservedNodeOfferingsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeReservedNodeOfferingsPaginator](./paginators.md#describereservednodeofferingspaginator)
3. item: [:material-code-braces: ReservedNodeOfferingsMessageTypeDef](./type_defs.md#reservednodeofferingsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedNodeOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReservedNodeOfferingId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ReservedNodeOfferingsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ReservedNodeOfferingsMessageTypeDef](./type_defs.md#reservednodeofferingsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReservedNodeOfferingsMessagePaginateTypeDef = {  # (1)
    "ReservedNodeOfferingId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedNodeOfferingsMessagePaginateTypeDef](./type_defs.md#describereservednodeofferingsmessagepaginatetypedef) 
## DescribeReservedNodesPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_reserved_nodes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeReservedNodes.html#Redshift.Paginator.DescribeReservedNodes)

```python
# DescribeReservedNodesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeReservedNodesPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeReservedNodesPaginator = client.get_paginator("describe_reserved_nodes")  # (2)
    async for item in paginator.paginate(...):
        item: ReservedNodesMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeReservedNodesPaginator](./paginators.md#describereservednodespaginator)
3. item: [:material-code-braces: ReservedNodesMessageTypeDef](./type_defs.md#reservednodesmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedNodesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReservedNodeId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ReservedNodesMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ReservedNodesMessageTypeDef](./type_defs.md#reservednodesmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReservedNodesMessagePaginateTypeDef = {  # (1)
    "ReservedNodeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedNodesMessagePaginateTypeDef](./type_defs.md#describereservednodesmessagepaginatetypedef) 
## DescribeScheduledActionsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_scheduled_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeScheduledActions.html#Redshift.Paginator.DescribeScheduledActions)

```python
# DescribeScheduledActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeScheduledActionsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ScheduledActionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeScheduledActionsPaginator](./paginators.md#describescheduledactionspaginator)
3. item: [:material-code-braces: ScheduledActionsMessageTypeDef](./type_defs.md#scheduledactionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeScheduledActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ScheduledActionName: str = ...,
    TargetActionType: ScheduledActionTypeValuesType = ...,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    Active: bool = ...,
    Filters: Sequence[ScheduledActionFilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ScheduledActionsMessageTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ScheduledActionTypeValuesType](./literals.md#scheduledactiontypevaluestype) 
2. See [:material-code-braces: ScheduledActionFilterTypeDef](./type_defs.md#scheduledactionfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ScheduledActionsMessageTypeDef](./type_defs.md#scheduledactionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeScheduledActionsMessagePaginateTypeDef = {  # (1)
    "ScheduledActionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScheduledActionsMessagePaginateTypeDef](./type_defs.md#describescheduledactionsmessagepaginatetypedef) 
## DescribeSnapshotCopyGrantsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_snapshot_copy_grants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeSnapshotCopyGrants.html#Redshift.Paginator.DescribeSnapshotCopyGrants)

```python
# DescribeSnapshotCopyGrantsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeSnapshotCopyGrantsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeSnapshotCopyGrantsPaginator = client.get_paginator("describe_snapshot_copy_grants")  # (2)
    async for item in paginator.paginate(...):
        item: SnapshotCopyGrantMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeSnapshotCopyGrantsPaginator](./paginators.md#describesnapshotcopygrantspaginator)
3. item: [:material-code-braces: SnapshotCopyGrantMessageTypeDef](./type_defs.md#snapshotcopygrantmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSnapshotCopyGrantsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SnapshotCopyGrantName: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[SnapshotCopyGrantMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SnapshotCopyGrantMessageTypeDef](./type_defs.md#snapshotcopygrantmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSnapshotCopyGrantsMessagePaginateTypeDef = {  # (1)
    "SnapshotCopyGrantName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotCopyGrantsMessagePaginateTypeDef](./type_defs.md#describesnapshotcopygrantsmessagepaginatetypedef) 
## DescribeSnapshotSchedulesPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_snapshot_schedules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeSnapshotSchedules.html#Redshift.Paginator.DescribeSnapshotSchedules)

```python
# DescribeSnapshotSchedulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeSnapshotSchedulesPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeSnapshotSchedulesPaginator = client.get_paginator("describe_snapshot_schedules")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSnapshotSchedulesOutputMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeSnapshotSchedulesPaginator](./paginators.md#describesnapshotschedulespaginator)
3. item: [:material-code-braces: DescribeSnapshotSchedulesOutputMessageTypeDef](./type_defs.md#describesnapshotschedulesoutputmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSnapshotSchedulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    ScheduleIdentifier: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeSnapshotSchedulesOutputMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSnapshotSchedulesOutputMessageTypeDef](./type_defs.md#describesnapshotschedulesoutputmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSnapshotSchedulesMessagePaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotSchedulesMessagePaginateTypeDef](./type_defs.md#describesnapshotschedulesmessagepaginatetypedef) 
## DescribeTableRestoreStatusPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_table_restore_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeTableRestoreStatus.html#Redshift.Paginator.DescribeTableRestoreStatus)

```python
# DescribeTableRestoreStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeTableRestoreStatusPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeTableRestoreStatusPaginator = client.get_paginator("describe_table_restore_status")  # (2)
    async for item in paginator.paginate(...):
        item: TableRestoreStatusMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeTableRestoreStatusPaginator](./paginators.md#describetablerestorestatuspaginator)
3. item: [:material-code-braces: TableRestoreStatusMessageTypeDef](./type_defs.md#tablerestorestatusmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTableRestoreStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    TableRestoreRequestId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[TableRestoreStatusMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: TableRestoreStatusMessageTypeDef](./type_defs.md#tablerestorestatusmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTableRestoreStatusMessagePaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTableRestoreStatusMessagePaginateTypeDef](./type_defs.md#describetablerestorestatusmessagepaginatetypedef) 
## DescribeTagsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeTags.html#Redshift.Paginator.DescribeTags)

```python
# DescribeTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeTagsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")  # (2)
    async for item in paginator.paginate(...):
        item: TaggedResourceListMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeTagsPaginator](./paginators.md#describetagspaginator)
3. item: [:material-code-braces: TaggedResourceListMessageTypeDef](./type_defs.md#taggedresourcelistmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceName: str = ...,
    ResourceType: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[TaggedResourceListMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: TaggedResourceListMessageTypeDef](./type_defs.md#taggedresourcelistmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTagsMessagePaginateTypeDef = {  # (1)
    "ResourceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTagsMessagePaginateTypeDef](./type_defs.md#describetagsmessagepaginatetypedef) 
## DescribeUsageLimitsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("describe_usage_limits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/DescribeUsageLimits.html#Redshift.Paginator.DescribeUsageLimits)

```python
# DescribeUsageLimitsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import DescribeUsageLimitsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: DescribeUsageLimitsPaginator = client.get_paginator("describe_usage_limits")  # (2)
    async for item in paginator.paginate(...):
        item: UsageLimitListTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeUsageLimitsPaginator](./paginators.md#describeusagelimitspaginator)
3. item: [:material-code-braces: UsageLimitListTypeDef](./type_defs.md#usagelimitlisttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeUsageLimitsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UsageLimitId: str = ...,
    ClusterIdentifier: str = ...,
    FeatureType: UsageLimitFeatureTypeType = ...,  # (1)
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[UsageLimitListTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: UsageLimitFeatureTypeType](./literals.md#usagelimitfeaturetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: UsageLimitListTypeDef](./type_defs.md#usagelimitlisttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeUsageLimitsMessagePaginateTypeDef = {  # (1)
    "UsageLimitId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeUsageLimitsMessagePaginateTypeDef](./type_defs.md#describeusagelimitsmessagepaginatetypedef) 
## GetReservedNodeExchangeConfigurationOptionsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("get_reserved_node_exchange_configuration_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/GetReservedNodeExchangeConfigurationOptions.html#Redshift.Paginator.GetReservedNodeExchangeConfigurationOptions)

```python
# GetReservedNodeExchangeConfigurationOptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import GetReservedNodeExchangeConfigurationOptionsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: GetReservedNodeExchangeConfigurationOptionsPaginator = client.get_paginator("get_reserved_node_exchange_configuration_options")  # (2)
    async for item in paginator.paginate(...):
        item: GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [GetReservedNodeExchangeConfigurationOptionsPaginator](./paginators.md#getreservednodeexchangeconfigurationoptionspaginator)
3. item: [:material-code-braces: GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef](./type_defs.md#getreservednodeexchangeconfigurationoptionsoutputmessagetypedef) 


### paginate

Type annotations and code completion for `#!python GetReservedNodeExchangeConfigurationOptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ActionType: ReservedNodeExchangeActionTypeType,  # (1)
    ClusterIdentifier: str = ...,
    SnapshotIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ReservedNodeExchangeActionTypeType](./literals.md#reservednodeexchangeactiontypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef](./type_defs.md#getreservednodeexchangeconfigurationoptionsoutputmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetReservedNodeExchangeConfigurationOptionsInputMessagePaginateTypeDef = {  # (1)
    "ActionType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetReservedNodeExchangeConfigurationOptionsInputMessagePaginateTypeDef](./type_defs.md#getreservednodeexchangeconfigurationoptionsinputmessagepaginatetypedef) 
## GetReservedNodeExchangeOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("get_reserved_node_exchange_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/GetReservedNodeExchangeOfferings.html#Redshift.Paginator.GetReservedNodeExchangeOfferings)

```python
# GetReservedNodeExchangeOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import GetReservedNodeExchangeOfferingsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: GetReservedNodeExchangeOfferingsPaginator = client.get_paginator("get_reserved_node_exchange_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: GetReservedNodeExchangeOfferingsOutputMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [GetReservedNodeExchangeOfferingsPaginator](./paginators.md#getreservednodeexchangeofferingspaginator)
3. item: [:material-code-braces: GetReservedNodeExchangeOfferingsOutputMessageTypeDef](./type_defs.md#getreservednodeexchangeofferingsoutputmessagetypedef) 


### paginate

Type annotations and code completion for `#!python GetReservedNodeExchangeOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReservedNodeId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetReservedNodeExchangeOfferingsOutputMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetReservedNodeExchangeOfferingsOutputMessageTypeDef](./type_defs.md#getreservednodeexchangeofferingsoutputmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetReservedNodeExchangeOfferingsInputMessagePaginateTypeDef = {  # (1)
    "ReservedNodeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetReservedNodeExchangeOfferingsInputMessagePaginateTypeDef](./type_defs.md#getreservednodeexchangeofferingsinputmessagepaginatetypedef) 
## ListRecommendationsPaginator

Type annotations and code completion for `#!python session.create_client("redshift").get_paginator("list_recommendations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift/paginator/ListRecommendations.html#Redshift.Paginator.ListRecommendations)

```python
# ListRecommendationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift.paginator import ListRecommendationsPaginator

session = get_session()
async with session.create_client("redshift") as client:  # (1)
    paginator: ListRecommendationsPaginator = client.get_paginator("list_recommendations")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommendationsResultTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [ListRecommendationsPaginator](./paginators.md#listrecommendationspaginator)
3. item: [:material-code-braces: ListRecommendationsResultTypeDef](./type_defs.md#listrecommendationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListRecommendationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    NamespaceArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRecommendationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecommendationsResultTypeDef](./type_defs.md#listrecommendationsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRecommendationsMessagePaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendationsMessagePaginateTypeDef](./type_defs.md#listrecommendationsmessagepaginatetypedef) 
