# drsClient

> [Index](../README.md) > [drs](./README.md) > drsClient

!!! note ""

    Auto-generated documentation for [drs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
    type annotations stubs module [types-aiobotocore-drs](https://pypi.org/project/types-aiobotocore-drs/).

## drsClient

Type annotations and code completion for `#!python session.create_client("drs")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client)

```python
drsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_drs.client import drsClient

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("drs").exceptions` structure.

```python
drsClient.exceptions usage example

async with session.create_client("drs") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.UninitializedAccountException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
drsClient usage type checking example

from types_aiobotocore_drs.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_source\_network\_stack

Associate a Source Network to an existing CloudFormation Stack and modify launch
templates to use this network.

Type annotations and code completion for `#!python session.create_client("drs").associate_source_network_stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.associate_source_network_stack)

```python
# associate_source_network_stack method definition

await def associate_source_network_stack(
    self,
    *,
    cfnStackName: str,
    sourceNetworkID: str,
) -> AssociateSourceNetworkStackResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateSourceNetworkStackResponseTypeDef](./type_defs.md#associatesourcenetworkstackresponsetypedef) 


```python
# associate_source_network_stack method usage example with argument unpacking

kwargs: AssociateSourceNetworkStackRequestRequestTypeDef = {  # (1)
    "cfnStackName": ...,
    "sourceNetworkID": ...,
}

parent.associate_source_network_stack(**kwargs)
```

1. See [:material-code-braces: AssociateSourceNetworkStackRequestRequestTypeDef](./type_defs.md#associatesourcenetworkstackrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("drs").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("drs").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_extended\_source\_server

Create an extended source server in the target Account based on the source
server in staging account.

Type annotations and code completion for `#!python session.create_client("drs").create_extended_source_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_extended_source_server)

```python
# create_extended_source_server method definition

await def create_extended_source_server(
    self,
    *,
    sourceServerArn: str,
    tags: Mapping[str, str] = ...,
) -> CreateExtendedSourceServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateExtendedSourceServerResponseTypeDef](./type_defs.md#createextendedsourceserverresponsetypedef) 


```python
# create_extended_source_server method usage example with argument unpacking

kwargs: CreateExtendedSourceServerRequestRequestTypeDef = {  # (1)
    "sourceServerArn": ...,
}

parent.create_extended_source_server(**kwargs)
```

1. See [:material-code-braces: CreateExtendedSourceServerRequestRequestTypeDef](./type_defs.md#createextendedsourceserverrequestrequesttypedef) 

### create\_launch\_configuration\_template

Creates a new Launch Configuration Template.

Type annotations and code completion for `#!python session.create_client("drs").create_launch_configuration_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_launch_configuration_template)

```python
# create_launch_configuration_template method definition

await def create_launch_configuration_template(
    self,
    *,
    copyPrivateIp: bool = ...,
    copyTags: bool = ...,
    exportBucketArn: str = ...,
    launchDisposition: LaunchDispositionType = ...,  # (1)
    licensing: LicensingTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
    targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,  # (3)
) -> CreateLaunchConfigurationTemplateResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
2. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
3. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
4. See [:material-code-braces: CreateLaunchConfigurationTemplateResponseTypeDef](./type_defs.md#createlaunchconfigurationtemplateresponsetypedef) 


```python
# create_launch_configuration_template method usage example with argument unpacking

kwargs: CreateLaunchConfigurationTemplateRequestRequestTypeDef = {  # (1)
    "copyPrivateIp": ...,
}

parent.create_launch_configuration_template(**kwargs)
```

1. See [:material-code-braces: CreateLaunchConfigurationTemplateRequestRequestTypeDef](./type_defs.md#createlaunchconfigurationtemplaterequestrequesttypedef) 

### create\_replication\_configuration\_template

Creates a new ReplicationConfigurationTemplate.

Type annotations and code completion for `#!python session.create_client("drs").create_replication_configuration_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_replication_configuration_template)

```python
# create_replication_configuration_template method definition

await def create_replication_configuration_template(
    self,
    *,
    associateDefaultSecurityGroup: bool,
    bandwidthThrottling: int,
    createPublicIP: bool,
    dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType,  # (1)
    defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType,  # (2)
    ebsEncryption: ReplicationConfigurationEbsEncryptionType,  # (3)
    pitPolicy: Sequence[PITPolicyRuleTypeDef],  # (4)
    replicationServerInstanceType: str,
    replicationServersSecurityGroupsIDs: Sequence[str],
    stagingAreaSubnetId: str,
    stagingAreaTags: Mapping[str, str],
    useDedicatedReplicationServer: bool,
    autoReplicateNewDisks: bool = ...,
    ebsEncryptionKeyArn: str = ...,
    tags: Mapping[str, str] = ...,
) -> ReplicationConfigurationTemplateResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: PITPolicyRuleTypeDef](./type_defs.md#pitpolicyruletypedef) 
5. See [:material-code-braces: ReplicationConfigurationTemplateResponseTypeDef](./type_defs.md#replicationconfigurationtemplateresponsetypedef) 


```python
# create_replication_configuration_template method usage example with argument unpacking

kwargs: CreateReplicationConfigurationTemplateRequestRequestTypeDef = {  # (1)
    "associateDefaultSecurityGroup": ...,
    "bandwidthThrottling": ...,
    "createPublicIP": ...,
    "dataPlaneRouting": ...,
    "defaultLargeStagingDiskType": ...,
    "ebsEncryption": ...,
    "pitPolicy": ...,
    "replicationServerInstanceType": ...,
    "replicationServersSecurityGroupsIDs": ...,
    "stagingAreaSubnetId": ...,
    "stagingAreaTags": ...,
    "useDedicatedReplicationServer": ...,
}

parent.create_replication_configuration_template(**kwargs)
```

1. See [:material-code-braces: CreateReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#createreplicationconfigurationtemplaterequestrequesttypedef) 

### create\_source\_network

Create a new Source Network resource for a provided VPC ID.

Type annotations and code completion for `#!python session.create_client("drs").create_source_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_source_network)

```python
# create_source_network method definition

await def create_source_network(
    self,
    *,
    originAccountID: str,
    originRegion: str,
    vpcID: str,
    tags: Mapping[str, str] = ...,
) -> CreateSourceNetworkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSourceNetworkResponseTypeDef](./type_defs.md#createsourcenetworkresponsetypedef) 


```python
# create_source_network method usage example with argument unpacking

kwargs: CreateSourceNetworkRequestRequestTypeDef = {  # (1)
    "originAccountID": ...,
    "originRegion": ...,
    "vpcID": ...,
}

parent.create_source_network(**kwargs)
```

1. See [:material-code-braces: CreateSourceNetworkRequestRequestTypeDef](./type_defs.md#createsourcenetworkrequestrequesttypedef) 

### delete\_job

Deletes a single Job by ID.

Type annotations and code completion for `#!python session.create_client("drs").delete_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_job)

```python
# delete_job method definition

await def delete_job(
    self,
    *,
    jobID: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_job method usage example with argument unpacking

kwargs: DeleteJobRequestRequestTypeDef = {  # (1)
    "jobID": ...,
}

parent.delete_job(**kwargs)
```

1. See [:material-code-braces: DeleteJobRequestRequestTypeDef](./type_defs.md#deletejobrequestrequesttypedef) 

### delete\_launch\_configuration\_template

Deletes a single Launch Configuration Template by ID.

Type annotations and code completion for `#!python session.create_client("drs").delete_launch_configuration_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_launch_configuration_template)

```python
# delete_launch_configuration_template method definition

await def delete_launch_configuration_template(
    self,
    *,
    launchConfigurationTemplateID: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_launch_configuration_template method usage example with argument unpacking

kwargs: DeleteLaunchConfigurationTemplateRequestRequestTypeDef = {  # (1)
    "launchConfigurationTemplateID": ...,
}

parent.delete_launch_configuration_template(**kwargs)
```

1. See [:material-code-braces: DeleteLaunchConfigurationTemplateRequestRequestTypeDef](./type_defs.md#deletelaunchconfigurationtemplaterequestrequesttypedef) 

### delete\_recovery\_instance

Deletes a single Recovery Instance by ID.

Type annotations and code completion for `#!python session.create_client("drs").delete_recovery_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_recovery_instance)

```python
# delete_recovery_instance method definition

await def delete_recovery_instance(
    self,
    *,
    recoveryInstanceID: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_recovery_instance method usage example with argument unpacking

kwargs: DeleteRecoveryInstanceRequestRequestTypeDef = {  # (1)
    "recoveryInstanceID": ...,
}

parent.delete_recovery_instance(**kwargs)
```

1. See [:material-code-braces: DeleteRecoveryInstanceRequestRequestTypeDef](./type_defs.md#deleterecoveryinstancerequestrequesttypedef) 

### delete\_replication\_configuration\_template

Deletes a single Replication Configuration Template by ID See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/drs-2020-02-26/DeleteReplicationConfigurationTemplate).

Type annotations and code completion for `#!python session.create_client("drs").delete_replication_configuration_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_replication_configuration_template)

```python
# delete_replication_configuration_template method definition

await def delete_replication_configuration_template(
    self,
    *,
    replicationConfigurationTemplateID: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_replication_configuration_template method usage example with argument unpacking

kwargs: DeleteReplicationConfigurationTemplateRequestRequestTypeDef = {  # (1)
    "replicationConfigurationTemplateID": ...,
}

parent.delete_replication_configuration_template(**kwargs)
```

1. See [:material-code-braces: DeleteReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#deletereplicationconfigurationtemplaterequestrequesttypedef) 

### delete\_source\_network

Delete Source Network resource.

Type annotations and code completion for `#!python session.create_client("drs").delete_source_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_source_network)

```python
# delete_source_network method definition

await def delete_source_network(
    self,
    *,
    sourceNetworkID: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_source_network method usage example with argument unpacking

kwargs: DeleteSourceNetworkRequestRequestTypeDef = {  # (1)
    "sourceNetworkID": ...,
}

parent.delete_source_network(**kwargs)
```

1. See [:material-code-braces: DeleteSourceNetworkRequestRequestTypeDef](./type_defs.md#deletesourcenetworkrequestrequesttypedef) 

### delete\_source\_server

Deletes a single Source Server by ID.

Type annotations and code completion for `#!python session.create_client("drs").delete_source_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_source_server)

```python
# delete_source_server method definition

await def delete_source_server(
    self,
    *,
    sourceServerID: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_source_server method usage example with argument unpacking

kwargs: DeleteSourceServerRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.delete_source_server(**kwargs)
```

1. See [:material-code-braces: DeleteSourceServerRequestRequestTypeDef](./type_defs.md#deletesourceserverrequestrequesttypedef) 

### describe\_job\_log\_items

Retrieves a detailed Job log with pagination.

Type annotations and code completion for `#!python session.create_client("drs").describe_job_log_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_job_log_items)

```python
# describe_job_log_items method definition

await def describe_job_log_items(
    self,
    *,
    jobID: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeJobLogItemsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef) 


```python
# describe_job_log_items method usage example with argument unpacking

kwargs: DescribeJobLogItemsRequestRequestTypeDef = {  # (1)
    "jobID": ...,
}

parent.describe_job_log_items(**kwargs)
```

1. See [:material-code-braces: DescribeJobLogItemsRequestRequestTypeDef](./type_defs.md#describejoblogitemsrequestrequesttypedef) 

### describe\_jobs

Returns a list of Jobs.

Type annotations and code completion for `#!python session.create_client("drs").describe_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_jobs)

```python
# describe_jobs method definition

await def describe_jobs(
    self,
    *,
    filters: DescribeJobsRequestFiltersTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef) 
2. See [:material-code-braces: DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef) 


```python
# describe_jobs method usage example with argument unpacking

kwargs: DescribeJobsRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.describe_jobs(**kwargs)
```

1. See [:material-code-braces: DescribeJobsRequestRequestTypeDef](./type_defs.md#describejobsrequestrequesttypedef) 

### describe\_launch\_configuration\_templates

Lists all Launch Configuration Templates, filtered by Launch Configuration
Template IDs See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/drs-2020-02-26/DescribeLaunchConfigurationTemplates).

Type annotations and code completion for `#!python session.create_client("drs").describe_launch_configuration_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_launch_configuration_templates)

```python
# describe_launch_configuration_templates method definition

await def describe_launch_configuration_templates(
    self,
    *,
    launchConfigurationTemplateIDs: Sequence[str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeLaunchConfigurationTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLaunchConfigurationTemplatesResponseTypeDef](./type_defs.md#describelaunchconfigurationtemplatesresponsetypedef) 


```python
# describe_launch_configuration_templates method usage example with argument unpacking

kwargs: DescribeLaunchConfigurationTemplatesRequestRequestTypeDef = {  # (1)
    "launchConfigurationTemplateIDs": ...,
}

parent.describe_launch_configuration_templates(**kwargs)
```

1. See [:material-code-braces: DescribeLaunchConfigurationTemplatesRequestRequestTypeDef](./type_defs.md#describelaunchconfigurationtemplatesrequestrequesttypedef) 

### describe\_recovery\_instances

Lists all Recovery Instances or multiple Recovery Instances by ID.

Type annotations and code completion for `#!python session.create_client("drs").describe_recovery_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_recovery_instances)

```python
# describe_recovery_instances method definition

await def describe_recovery_instances(
    self,
    *,
    filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeRecoveryInstancesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DescribeRecoveryInstancesRequestFiltersTypeDef](./type_defs.md#describerecoveryinstancesrequestfilterstypedef) 
2. See [:material-code-braces: DescribeRecoveryInstancesResponseTypeDef](./type_defs.md#describerecoveryinstancesresponsetypedef) 


```python
# describe_recovery_instances method usage example with argument unpacking

kwargs: DescribeRecoveryInstancesRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.describe_recovery_instances(**kwargs)
```

1. See [:material-code-braces: DescribeRecoveryInstancesRequestRequestTypeDef](./type_defs.md#describerecoveryinstancesrequestrequesttypedef) 

### describe\_recovery\_snapshots

Lists all Recovery Snapshots for a single Source Server.

Type annotations and code completion for `#!python session.create_client("drs").describe_recovery_snapshots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_recovery_snapshots)

```python
# describe_recovery_snapshots method definition

await def describe_recovery_snapshots(
    self,
    *,
    sourceServerID: str,
    filters: DescribeRecoverySnapshotsRequestFiltersTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    order: RecoverySnapshotsOrderType = ...,  # (2)
) -> DescribeRecoverySnapshotsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DescribeRecoverySnapshotsRequestFiltersTypeDef](./type_defs.md#describerecoverysnapshotsrequestfilterstypedef) 
2. See [:material-code-brackets: RecoverySnapshotsOrderType](./literals.md#recoverysnapshotsordertype) 
3. See [:material-code-braces: DescribeRecoverySnapshotsResponseTypeDef](./type_defs.md#describerecoverysnapshotsresponsetypedef) 


```python
# describe_recovery_snapshots method usage example with argument unpacking

kwargs: DescribeRecoverySnapshotsRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.describe_recovery_snapshots(**kwargs)
```

1. See [:material-code-braces: DescribeRecoverySnapshotsRequestRequestTypeDef](./type_defs.md#describerecoverysnapshotsrequestrequesttypedef) 

### describe\_replication\_configuration\_templates

Lists all ReplicationConfigurationTemplates, filtered by Source Server IDs.

Type annotations and code completion for `#!python session.create_client("drs").describe_replication_configuration_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_replication_configuration_templates)

```python
# describe_replication_configuration_templates method definition

await def describe_replication_configuration_templates(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    replicationConfigurationTemplateIDs: Sequence[str] = ...,
) -> DescribeReplicationConfigurationTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef) 


```python
# describe_replication_configuration_templates method usage example with argument unpacking

kwargs: DescribeReplicationConfigurationTemplatesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.describe_replication_configuration_templates(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationConfigurationTemplatesRequestRequestTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequestrequesttypedef) 

### describe\_source\_networks

Lists all Source Networks or multiple Source Networks filtered by ID.

Type annotations and code completion for `#!python session.create_client("drs").describe_source_networks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_source_networks)

```python
# describe_source_networks method definition

await def describe_source_networks(
    self,
    *,
    filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeSourceNetworksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DescribeSourceNetworksRequestFiltersTypeDef](./type_defs.md#describesourcenetworksrequestfilterstypedef) 
2. See [:material-code-braces: DescribeSourceNetworksResponseTypeDef](./type_defs.md#describesourcenetworksresponsetypedef) 


```python
# describe_source_networks method usage example with argument unpacking

kwargs: DescribeSourceNetworksRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.describe_source_networks(**kwargs)
```

1. See [:material-code-braces: DescribeSourceNetworksRequestRequestTypeDef](./type_defs.md#describesourcenetworksrequestrequesttypedef) 

### describe\_source\_servers

Lists all Source Servers or multiple Source Servers filtered by ID.

Type annotations and code completion for `#!python session.create_client("drs").describe_source_servers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_source_servers)

```python
# describe_source_servers method definition

await def describe_source_servers(
    self,
    *,
    filters: DescribeSourceServersRequestFiltersTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeSourceServersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef) 
2. See [:material-code-braces: DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef) 


```python
# describe_source_servers method usage example with argument unpacking

kwargs: DescribeSourceServersRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.describe_source_servers(**kwargs)
```

1. See [:material-code-braces: DescribeSourceServersRequestRequestTypeDef](./type_defs.md#describesourceserversrequestrequesttypedef) 

### disconnect\_recovery\_instance

Disconnect a Recovery Instance from Elastic Disaster Recovery.

Type annotations and code completion for `#!python session.create_client("drs").disconnect_recovery_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.disconnect_recovery_instance)

```python
# disconnect_recovery_instance method definition

await def disconnect_recovery_instance(
    self,
    *,
    recoveryInstanceID: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disconnect_recovery_instance method usage example with argument unpacking

kwargs: DisconnectRecoveryInstanceRequestRequestTypeDef = {  # (1)
    "recoveryInstanceID": ...,
}

parent.disconnect_recovery_instance(**kwargs)
```

1. See [:material-code-braces: DisconnectRecoveryInstanceRequestRequestTypeDef](./type_defs.md#disconnectrecoveryinstancerequestrequesttypedef) 

### disconnect\_source\_server

Disconnects a specific Source Server from Elastic Disaster Recovery.

Type annotations and code completion for `#!python session.create_client("drs").disconnect_source_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.disconnect_source_server)

```python
# disconnect_source_server method definition

await def disconnect_source_server(
    self,
    *,
    sourceServerID: str,
) -> SourceServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef) 


```python
# disconnect_source_server method usage example with argument unpacking

kwargs: DisconnectSourceServerRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.disconnect_source_server(**kwargs)
```

1. See [:material-code-braces: DisconnectSourceServerRequestRequestTypeDef](./type_defs.md#disconnectsourceserverrequestrequesttypedef) 

### export\_source\_network\_cfn\_template

Export the Source Network CloudFormation template to an S3 bucket.

Type annotations and code completion for `#!python session.create_client("drs").export_source_network_cfn_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.export_source_network_cfn_template)

```python
# export_source_network_cfn_template method definition

await def export_source_network_cfn_template(
    self,
    *,
    sourceNetworkID: str,
) -> ExportSourceNetworkCfnTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExportSourceNetworkCfnTemplateResponseTypeDef](./type_defs.md#exportsourcenetworkcfntemplateresponsetypedef) 


```python
# export_source_network_cfn_template method usage example with argument unpacking

kwargs: ExportSourceNetworkCfnTemplateRequestRequestTypeDef = {  # (1)
    "sourceNetworkID": ...,
}

parent.export_source_network_cfn_template(**kwargs)
```

1. See [:material-code-braces: ExportSourceNetworkCfnTemplateRequestRequestTypeDef](./type_defs.md#exportsourcenetworkcfntemplaterequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("drs").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_failback\_replication\_configuration

Lists all Failback ReplicationConfigurations, filtered by Recovery Instance ID.

Type annotations and code completion for `#!python session.create_client("drs").get_failback_replication_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_failback_replication_configuration)

```python
# get_failback_replication_configuration method definition

await def get_failback_replication_configuration(
    self,
    *,
    recoveryInstanceID: str,
) -> GetFailbackReplicationConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFailbackReplicationConfigurationResponseTypeDef](./type_defs.md#getfailbackreplicationconfigurationresponsetypedef) 


```python
# get_failback_replication_configuration method usage example with argument unpacking

kwargs: GetFailbackReplicationConfigurationRequestRequestTypeDef = {  # (1)
    "recoveryInstanceID": ...,
}

parent.get_failback_replication_configuration(**kwargs)
```

1. See [:material-code-braces: GetFailbackReplicationConfigurationRequestRequestTypeDef](./type_defs.md#getfailbackreplicationconfigurationrequestrequesttypedef) 

### get\_launch\_configuration

Gets a LaunchConfiguration, filtered by Source Server IDs.

Type annotations and code completion for `#!python session.create_client("drs").get_launch_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_launch_configuration)

```python
# get_launch_configuration method definition

await def get_launch_configuration(
    self,
    *,
    sourceServerID: str,
) -> LaunchConfigurationTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: LaunchConfigurationTypeDef](./type_defs.md#launchconfigurationtypedef) 


```python
# get_launch_configuration method usage example with argument unpacking

kwargs: GetLaunchConfigurationRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.get_launch_configuration(**kwargs)
```

1. See [:material-code-braces: GetLaunchConfigurationRequestRequestTypeDef](./type_defs.md#getlaunchconfigurationrequestrequesttypedef) 

### get\_replication\_configuration

Gets a ReplicationConfiguration, filtered by Source Server ID.

Type annotations and code completion for `#!python session.create_client("drs").get_replication_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_replication_configuration)

```python
# get_replication_configuration method definition

await def get_replication_configuration(
    self,
    *,
    sourceServerID: str,
) -> ReplicationConfigurationTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef) 


```python
# get_replication_configuration method usage example with argument unpacking

kwargs: GetReplicationConfigurationRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.get_replication_configuration(**kwargs)
```

1. See [:material-code-braces: GetReplicationConfigurationRequestRequestTypeDef](./type_defs.md#getreplicationconfigurationrequestrequesttypedef) 

### initialize\_service

Initialize Elastic Disaster Recovery.

Type annotations and code completion for `#!python session.create_client("drs").initialize_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.initialize_service)

```python
# initialize_service method definition

await def initialize_service(
    self,
) -> Dict[str, Any]:
    ...
```


### list\_extensible\_source\_servers

Returns a list of source servers on a staging account that are extensible, which
means that: a.

Type annotations and code completion for `#!python session.create_client("drs").list_extensible_source_servers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.list_extensible_source_servers)

```python
# list_extensible_source_servers method definition

await def list_extensible_source_servers(
    self,
    *,
    stagingAccountID: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListExtensibleSourceServersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListExtensibleSourceServersResponseTypeDef](./type_defs.md#listextensiblesourceserversresponsetypedef) 


```python
# list_extensible_source_servers method usage example with argument unpacking

kwargs: ListExtensibleSourceServersRequestRequestTypeDef = {  # (1)
    "stagingAccountID": ...,
}

parent.list_extensible_source_servers(**kwargs)
```

1. See [:material-code-braces: ListExtensibleSourceServersRequestRequestTypeDef](./type_defs.md#listextensiblesourceserversrequestrequesttypedef) 

### list\_staging\_accounts

Returns an array of staging accounts for existing extended source servers.

Type annotations and code completion for `#!python session.create_client("drs").list_staging_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.list_staging_accounts)

```python
# list_staging_accounts method definition

await def list_staging_accounts(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListStagingAccountsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStagingAccountsResponseTypeDef](./type_defs.md#liststagingaccountsresponsetypedef) 


```python
# list_staging_accounts method usage example with argument unpacking

kwargs: ListStagingAccountsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_staging_accounts(**kwargs)
```

1. See [:material-code-braces: ListStagingAccountsRequestRequestTypeDef](./type_defs.md#liststagingaccountsrequestrequesttypedef) 

### list\_tags\_for\_resource

List all tags for your Elastic Disaster Recovery resources.

Type annotations and code completion for `#!python session.create_client("drs").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### retry\_data\_replication

WARNING: RetryDataReplication is deprecated.

Type annotations and code completion for `#!python session.create_client("drs").retry_data_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.retry_data_replication)

```python
# retry_data_replication method definition

await def retry_data_replication(
    self,
    *,
    sourceServerID: str,
) -> SourceServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef) 


```python
# retry_data_replication method usage example with argument unpacking

kwargs: RetryDataReplicationRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.retry_data_replication(**kwargs)
```

1. See [:material-code-braces: RetryDataReplicationRequestRequestTypeDef](./type_defs.md#retrydatareplicationrequestrequesttypedef) 

### reverse\_replication

Start replication to origin / target region - applies only to protected
instances that originated in EC2.

Type annotations and code completion for `#!python session.create_client("drs").reverse_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.reverse_replication)

```python
# reverse_replication method definition

await def reverse_replication(
    self,
    *,
    recoveryInstanceID: str,
) -> ReverseReplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ReverseReplicationResponseTypeDef](./type_defs.md#reversereplicationresponsetypedef) 


```python
# reverse_replication method usage example with argument unpacking

kwargs: ReverseReplicationRequestRequestTypeDef = {  # (1)
    "recoveryInstanceID": ...,
}

parent.reverse_replication(**kwargs)
```

1. See [:material-code-braces: ReverseReplicationRequestRequestTypeDef](./type_defs.md#reversereplicationrequestrequesttypedef) 

### start\_failback\_launch

Initiates a Job for launching the machine that is being failed back to from the
specified Recovery Instance.

Type annotations and code completion for `#!python session.create_client("drs").start_failback_launch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_failback_launch)

```python
# start_failback_launch method definition

await def start_failback_launch(
    self,
    *,
    recoveryInstanceIDs: Sequence[str],
    tags: Mapping[str, str] = ...,
) -> StartFailbackLaunchResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartFailbackLaunchResponseTypeDef](./type_defs.md#startfailbacklaunchresponsetypedef) 


```python
# start_failback_launch method usage example with argument unpacking

kwargs: StartFailbackLaunchRequestRequestTypeDef = {  # (1)
    "recoveryInstanceIDs": ...,
}

parent.start_failback_launch(**kwargs)
```

1. See [:material-code-braces: StartFailbackLaunchRequestRequestTypeDef](./type_defs.md#startfailbacklaunchrequestrequesttypedef) 

### start\_recovery

Launches Recovery Instances for the specified Source Servers.

Type annotations and code completion for `#!python session.create_client("drs").start_recovery` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_recovery)

```python
# start_recovery method definition

await def start_recovery(
    self,
    *,
    sourceServers: Sequence[StartRecoveryRequestSourceServerTypeDef],  # (1)
    isDrill: bool = ...,
    tags: Mapping[str, str] = ...,
) -> StartRecoveryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StartRecoveryRequestSourceServerTypeDef](./type_defs.md#startrecoveryrequestsourceservertypedef) 
2. See [:material-code-braces: StartRecoveryResponseTypeDef](./type_defs.md#startrecoveryresponsetypedef) 


```python
# start_recovery method usage example with argument unpacking

kwargs: StartRecoveryRequestRequestTypeDef = {  # (1)
    "sourceServers": ...,
}

parent.start_recovery(**kwargs)
```

1. See [:material-code-braces: StartRecoveryRequestRequestTypeDef](./type_defs.md#startrecoveryrequestrequesttypedef) 

### start\_replication

Starts replication for a stopped Source Server.

Type annotations and code completion for `#!python session.create_client("drs").start_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_replication)

```python
# start_replication method definition

await def start_replication(
    self,
    *,
    sourceServerID: str,
) -> StartReplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartReplicationResponseTypeDef](./type_defs.md#startreplicationresponsetypedef) 


```python
# start_replication method usage example with argument unpacking

kwargs: StartReplicationRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.start_replication(**kwargs)
```

1. See [:material-code-braces: StartReplicationRequestRequestTypeDef](./type_defs.md#startreplicationrequestrequesttypedef) 

### start\_source\_network\_recovery

Deploy VPC for the specified Source Network and modify launch templates to use
this network.

Type annotations and code completion for `#!python session.create_client("drs").start_source_network_recovery` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_source_network_recovery)

```python
# start_source_network_recovery method definition

await def start_source_network_recovery(
    self,
    *,
    sourceNetworks: Sequence[StartSourceNetworkRecoveryRequestNetworkEntryTypeDef],  # (1)
    deployAsNew: bool = ...,
    tags: Mapping[str, str] = ...,
) -> StartSourceNetworkRecoveryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StartSourceNetworkRecoveryRequestNetworkEntryTypeDef](./type_defs.md#startsourcenetworkrecoveryrequestnetworkentrytypedef) 
2. See [:material-code-braces: StartSourceNetworkRecoveryResponseTypeDef](./type_defs.md#startsourcenetworkrecoveryresponsetypedef) 


```python
# start_source_network_recovery method usage example with argument unpacking

kwargs: StartSourceNetworkRecoveryRequestRequestTypeDef = {  # (1)
    "sourceNetworks": ...,
}

parent.start_source_network_recovery(**kwargs)
```

1. See [:material-code-braces: StartSourceNetworkRecoveryRequestRequestTypeDef](./type_defs.md#startsourcenetworkrecoveryrequestrequesttypedef) 

### start\_source\_network\_replication

Starts replication for a Source Network.

Type annotations and code completion for `#!python session.create_client("drs").start_source_network_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_source_network_replication)

```python
# start_source_network_replication method definition

await def start_source_network_replication(
    self,
    *,
    sourceNetworkID: str,
) -> StartSourceNetworkReplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartSourceNetworkReplicationResponseTypeDef](./type_defs.md#startsourcenetworkreplicationresponsetypedef) 


```python
# start_source_network_replication method usage example with argument unpacking

kwargs: StartSourceNetworkReplicationRequestRequestTypeDef = {  # (1)
    "sourceNetworkID": ...,
}

parent.start_source_network_replication(**kwargs)
```

1. See [:material-code-braces: StartSourceNetworkReplicationRequestRequestTypeDef](./type_defs.md#startsourcenetworkreplicationrequestrequesttypedef) 

### stop\_failback

Stops the failback process for a specified Recovery Instance.

Type annotations and code completion for `#!python session.create_client("drs").stop_failback` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.stop_failback)

```python
# stop_failback method definition

await def stop_failback(
    self,
    *,
    recoveryInstanceID: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_failback method usage example with argument unpacking

kwargs: StopFailbackRequestRequestTypeDef = {  # (1)
    "recoveryInstanceID": ...,
}

parent.stop_failback(**kwargs)
```

1. See [:material-code-braces: StopFailbackRequestRequestTypeDef](./type_defs.md#stopfailbackrequestrequesttypedef) 

### stop\_replication

Stops replication for a Source Server.

Type annotations and code completion for `#!python session.create_client("drs").stop_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.stop_replication)

```python
# stop_replication method definition

await def stop_replication(
    self,
    *,
    sourceServerID: str,
) -> StopReplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopReplicationResponseTypeDef](./type_defs.md#stopreplicationresponsetypedef) 


```python
# stop_replication method usage example with argument unpacking

kwargs: StopReplicationRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.stop_replication(**kwargs)
```

1. See [:material-code-braces: StopReplicationRequestRequestTypeDef](./type_defs.md#stopreplicationrequestrequesttypedef) 

### stop\_source\_network\_replication

Stops replication for a Source Network.

Type annotations and code completion for `#!python session.create_client("drs").stop_source_network_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.stop_source_network_replication)

```python
# stop_source_network_replication method definition

await def stop_source_network_replication(
    self,
    *,
    sourceNetworkID: str,
) -> StopSourceNetworkReplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopSourceNetworkReplicationResponseTypeDef](./type_defs.md#stopsourcenetworkreplicationresponsetypedef) 


```python
# stop_source_network_replication method usage example with argument unpacking

kwargs: StopSourceNetworkReplicationRequestRequestTypeDef = {  # (1)
    "sourceNetworkID": ...,
}

parent.stop_source_network_replication(**kwargs)
```

1. See [:material-code-braces: StopSourceNetworkReplicationRequestRequestTypeDef](./type_defs.md#stopsourcenetworkreplicationrequestrequesttypedef) 

### tag\_resource

Adds or overwrites only the specified tags for the specified Elastic Disaster
Recovery resource or resources.

Type annotations and code completion for `#!python session.create_client("drs").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### terminate\_recovery\_instances

Initiates a Job for terminating the EC2 resources associated with the specified
Recovery Instances, and then will delete the Recovery Instances from the Elastic
Disaster Recovery service.

Type annotations and code completion for `#!python session.create_client("drs").terminate_recovery_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.terminate_recovery_instances)

```python
# terminate_recovery_instances method definition

await def terminate_recovery_instances(
    self,
    *,
    recoveryInstanceIDs: Sequence[str],
) -> TerminateRecoveryInstancesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TerminateRecoveryInstancesResponseTypeDef](./type_defs.md#terminaterecoveryinstancesresponsetypedef) 


```python
# terminate_recovery_instances method usage example with argument unpacking

kwargs: TerminateRecoveryInstancesRequestRequestTypeDef = {  # (1)
    "recoveryInstanceIDs": ...,
}

parent.terminate_recovery_instances(**kwargs)
```

1. See [:material-code-braces: TerminateRecoveryInstancesRequestRequestTypeDef](./type_defs.md#terminaterecoveryinstancesrequestrequesttypedef) 

### untag\_resource

Deletes the specified set of tags from the specified set of Elastic Disaster
Recovery resources.

Type annotations and code completion for `#!python session.create_client("drs").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_failback\_replication\_configuration

Allows you to update the failback replication configuration of a Recovery
Instance by ID.

Type annotations and code completion for `#!python session.create_client("drs").update_failback_replication_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_failback_replication_configuration)

```python
# update_failback_replication_configuration method definition

await def update_failback_replication_configuration(
    self,
    *,
    recoveryInstanceID: str,
    bandwidthThrottling: int = ...,
    name: str = ...,
    usePrivateIP: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_failback_replication_configuration method usage example with argument unpacking

kwargs: UpdateFailbackReplicationConfigurationRequestRequestTypeDef = {  # (1)
    "recoveryInstanceID": ...,
}

parent.update_failback_replication_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateFailbackReplicationConfigurationRequestRequestTypeDef](./type_defs.md#updatefailbackreplicationconfigurationrequestrequesttypedef) 

### update\_launch\_configuration

Updates a LaunchConfiguration by Source Server ID.

Type annotations and code completion for `#!python session.create_client("drs").update_launch_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_launch_configuration)

```python
# update_launch_configuration method definition

await def update_launch_configuration(
    self,
    *,
    sourceServerID: str,
    copyPrivateIp: bool = ...,
    copyTags: bool = ...,
    launchDisposition: LaunchDispositionType = ...,  # (1)
    licensing: LicensingTypeDef = ...,  # (2)
    name: str = ...,
    targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,  # (3)
) -> LaunchConfigurationTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
2. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
3. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
4. See [:material-code-braces: LaunchConfigurationTypeDef](./type_defs.md#launchconfigurationtypedef) 


```python
# update_launch_configuration method usage example with argument unpacking

kwargs: UpdateLaunchConfigurationRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.update_launch_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateLaunchConfigurationRequestRequestTypeDef](./type_defs.md#updatelaunchconfigurationrequestrequesttypedef) 

### update\_launch\_configuration\_template

Updates an existing Launch Configuration Template by ID.

Type annotations and code completion for `#!python session.create_client("drs").update_launch_configuration_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_launch_configuration_template)

```python
# update_launch_configuration_template method definition

await def update_launch_configuration_template(
    self,
    *,
    launchConfigurationTemplateID: str,
    copyPrivateIp: bool = ...,
    copyTags: bool = ...,
    exportBucketArn: str = ...,
    launchDisposition: LaunchDispositionType = ...,  # (1)
    licensing: LicensingTypeDef = ...,  # (2)
    targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,  # (3)
) -> UpdateLaunchConfigurationTemplateResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
2. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
3. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
4. See [:material-code-braces: UpdateLaunchConfigurationTemplateResponseTypeDef](./type_defs.md#updatelaunchconfigurationtemplateresponsetypedef) 


```python
# update_launch_configuration_template method usage example with argument unpacking

kwargs: UpdateLaunchConfigurationTemplateRequestRequestTypeDef = {  # (1)
    "launchConfigurationTemplateID": ...,
}

parent.update_launch_configuration_template(**kwargs)
```

1. See [:material-code-braces: UpdateLaunchConfigurationTemplateRequestRequestTypeDef](./type_defs.md#updatelaunchconfigurationtemplaterequestrequesttypedef) 

### update\_replication\_configuration

Allows you to update a ReplicationConfiguration by Source Server ID.

Type annotations and code completion for `#!python session.create_client("drs").update_replication_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_replication_configuration)

```python
# update_replication_configuration method definition

await def update_replication_configuration(
    self,
    *,
    sourceServerID: str,
    associateDefaultSecurityGroup: bool = ...,
    autoReplicateNewDisks: bool = ...,
    bandwidthThrottling: int = ...,
    createPublicIP: bool = ...,
    dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType = ...,  # (1)
    defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,  # (2)
    ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,  # (3)
    ebsEncryptionKeyArn: str = ...,
    name: str = ...,
    pitPolicy: Sequence[PITPolicyRuleTypeDef] = ...,  # (4)
    replicatedDisks: Sequence[ReplicationConfigurationReplicatedDiskTypeDef] = ...,  # (5)
    replicationServerInstanceType: str = ...,
    replicationServersSecurityGroupsIDs: Sequence[str] = ...,
    stagingAreaSubnetId: str = ...,
    stagingAreaTags: Mapping[str, str] = ...,
    useDedicatedReplicationServer: bool = ...,
) -> ReplicationConfigurationTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: PITPolicyRuleTypeDef](./type_defs.md#pitpolicyruletypedef) 
5. See [:material-code-braces: ReplicationConfigurationReplicatedDiskTypeDef](./type_defs.md#replicationconfigurationreplicateddisktypedef) 
6. See [:material-code-braces: ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef) 


```python
# update_replication_configuration method usage example with argument unpacking

kwargs: UpdateReplicationConfigurationRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.update_replication_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateReplicationConfigurationRequestRequestTypeDef](./type_defs.md#updatereplicationconfigurationrequestrequesttypedef) 

### update\_replication\_configuration\_template

Updates a ReplicationConfigurationTemplate by ID.

Type annotations and code completion for `#!python session.create_client("drs").update_replication_configuration_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_replication_configuration_template)

```python
# update_replication_configuration_template method definition

await def update_replication_configuration_template(
    self,
    *,
    replicationConfigurationTemplateID: str,
    arn: str = ...,
    associateDefaultSecurityGroup: bool = ...,
    autoReplicateNewDisks: bool = ...,
    bandwidthThrottling: int = ...,
    createPublicIP: bool = ...,
    dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType = ...,  # (1)
    defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,  # (2)
    ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,  # (3)
    ebsEncryptionKeyArn: str = ...,
    pitPolicy: Sequence[PITPolicyRuleTypeDef] = ...,  # (4)
    replicationServerInstanceType: str = ...,
    replicationServersSecurityGroupsIDs: Sequence[str] = ...,
    stagingAreaSubnetId: str = ...,
    stagingAreaTags: Mapping[str, str] = ...,
    useDedicatedReplicationServer: bool = ...,
) -> ReplicationConfigurationTemplateResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: PITPolicyRuleTypeDef](./type_defs.md#pitpolicyruletypedef) 
5. See [:material-code-braces: ReplicationConfigurationTemplateResponseTypeDef](./type_defs.md#replicationconfigurationtemplateresponsetypedef) 


```python
# update_replication_configuration_template method usage example with argument unpacking

kwargs: UpdateReplicationConfigurationTemplateRequestRequestTypeDef = {  # (1)
    "replicationConfigurationTemplateID": ...,
}

parent.update_replication_configuration_template(**kwargs)
```

1. See [:material-code-braces: UpdateReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#updatereplicationconfigurationtemplaterequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("drs").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> drsClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("drs").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator` method with overloads.

- `client.get_paginator("describe_job_log_items")` -> [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
- `client.get_paginator("describe_jobs")` -> [DescribeJobsPaginator](./paginators.md#describejobspaginator)
- `client.get_paginator("describe_launch_configuration_templates")` -> [DescribeLaunchConfigurationTemplatesPaginator](./paginators.md#describelaunchconfigurationtemplatespaginator)
- `client.get_paginator("describe_recovery_instances")` -> [DescribeRecoveryInstancesPaginator](./paginators.md#describerecoveryinstancespaginator)
- `client.get_paginator("describe_recovery_snapshots")` -> [DescribeRecoverySnapshotsPaginator](./paginators.md#describerecoverysnapshotspaginator)
- `client.get_paginator("describe_replication_configuration_templates")` -> [DescribeReplicationConfigurationTemplatesPaginator](./paginators.md#describereplicationconfigurationtemplatespaginator)
- `client.get_paginator("describe_source_networks")` -> [DescribeSourceNetworksPaginator](./paginators.md#describesourcenetworkspaginator)
- `client.get_paginator("describe_source_servers")` -> [DescribeSourceServersPaginator](./paginators.md#describesourceserverspaginator)
- `client.get_paginator("list_extensible_source_servers")` -> [ListExtensibleSourceServersPaginator](./paginators.md#listextensiblesourceserverspaginator)
- `client.get_paginator("list_staging_accounts")` -> [ListStagingAccountsPaginator](./paginators.md#liststagingaccountspaginator)



