# MgnClient

> [Index](../README.md) > [Mgn](./README.md) > MgnClient

!!! note ""

    Auto-generated documentation for [Mgn](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
    type annotations stubs module [types-aiobotocore-mgn](https://pypi.org/project/types-aiobotocore-mgn/).

## MgnClient

Type annotations and code completion for `#!python session.create_client("mgn")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#Mgn.Client)

```python
# MgnClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_mgn.client import MgnClient

session = get_session()
async with session.create_client("mgn") as client:
    client: MgnClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("mgn").exceptions` structure.

```python
# MgnClient.exceptions usage example

async with session.create_client("mgn") as client:
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
# MgnClient usage type checking example

from types_aiobotocore_mgn.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("mgn").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("mgn").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/generate_presigned_url.html)

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


### close



Type annotations and code completion for `#!python session.create_client("mgn").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### archive\_application

Archive application.

Type annotations and code completion for `#!python session.create_client("mgn").archive_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/archive_application.html)

```python
# archive_application method definition

await def archive_application(
    self,
    *,
    applicationID: str,
    accountID: str = ...,
) -> ApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef) 


```python
# archive_application method usage example with argument unpacking

kwargs: ArchiveApplicationRequestRequestTypeDef = {  # (1)
    "applicationID": ...,
}

parent.archive_application(**kwargs)
```

1. See [:material-code-braces: ArchiveApplicationRequestRequestTypeDef](./type_defs.md#archiveapplicationrequestrequesttypedef) 

### archive\_wave

Archive wave.

Type annotations and code completion for `#!python session.create_client("mgn").archive_wave` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/archive_wave.html)

```python
# archive_wave method definition

await def archive_wave(
    self,
    *,
    waveID: str,
    accountID: str = ...,
) -> WaveResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: WaveResponseTypeDef](./type_defs.md#waveresponsetypedef) 


```python
# archive_wave method usage example with argument unpacking

kwargs: ArchiveWaveRequestRequestTypeDef = {  # (1)
    "waveID": ...,
}

parent.archive_wave(**kwargs)
```

1. See [:material-code-braces: ArchiveWaveRequestRequestTypeDef](./type_defs.md#archivewaverequestrequesttypedef) 

### associate\_applications

Associate applications to wave.

Type annotations and code completion for `#!python session.create_client("mgn").associate_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/associate_applications.html)

```python
# associate_applications method definition

await def associate_applications(
    self,
    *,
    applicationIDs: Sequence[str],
    waveID: str,
    accountID: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# associate_applications method usage example with argument unpacking

kwargs: AssociateApplicationsRequestRequestTypeDef = {  # (1)
    "applicationIDs": ...,
    "waveID": ...,
}

parent.associate_applications(**kwargs)
```

1. See [:material-code-braces: AssociateApplicationsRequestRequestTypeDef](./type_defs.md#associateapplicationsrequestrequesttypedef) 

### associate\_source\_servers

Associate source servers to application.

Type annotations and code completion for `#!python session.create_client("mgn").associate_source_servers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/associate_source_servers.html)

```python
# associate_source_servers method definition

await def associate_source_servers(
    self,
    *,
    applicationID: str,
    sourceServerIDs: Sequence[str],
    accountID: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# associate_source_servers method usage example with argument unpacking

kwargs: AssociateSourceServersRequestRequestTypeDef = {  # (1)
    "applicationID": ...,
    "sourceServerIDs": ...,
}

parent.associate_source_servers(**kwargs)
```

1. See [:material-code-braces: AssociateSourceServersRequestRequestTypeDef](./type_defs.md#associatesourceserversrequestrequesttypedef) 

### change\_server\_life\_cycle\_state

Allows the user to set the SourceServer.LifeCycle.state property for specific
Source Server IDs to one of the following: READY_FOR_TEST or READY_FOR_CUTOVER.

Type annotations and code completion for `#!python session.create_client("mgn").change_server_life_cycle_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/change_server_life_cycle_state.html)

```python
# change_server_life_cycle_state method definition

await def change_server_life_cycle_state(
    self,
    *,
    lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,  # (1)
    sourceServerID: str,
    accountID: str = ...,
) -> SourceServerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef](./type_defs.md#changeserverlifecyclestatesourceserverlifecycletypedef) 
2. See [:material-code-braces: SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef) 


```python
# change_server_life_cycle_state method usage example with argument unpacking

kwargs: ChangeServerLifeCycleStateRequestRequestTypeDef = {  # (1)
    "lifeCycle": ...,
    "sourceServerID": ...,
}

parent.change_server_life_cycle_state(**kwargs)
```

1. See [:material-code-braces: ChangeServerLifeCycleStateRequestRequestTypeDef](./type_defs.md#changeserverlifecyclestaterequestrequesttypedef) 

### create\_application

Create application.

Type annotations and code completion for `#!python session.create_client("mgn").create_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/create_application.html)

```python
# create_application method definition

await def create_application(
    self,
    *,
    name: str,
    accountID: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> ApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef) 


```python
# create_application method usage example with argument unpacking

kwargs: CreateApplicationRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_application(**kwargs)
```

1. See [:material-code-braces: CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef) 

### create\_connector

Create Connector.

Type annotations and code completion for `#!python session.create_client("mgn").create_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/create_connector.html)

```python
# create_connector method definition

await def create_connector(
    self,
    *,
    name: str,
    ssmInstanceID: str,
    ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> ConnectorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConnectorSsmCommandConfigTypeDef](./type_defs.md#connectorssmcommandconfigtypedef) 
2. See [:material-code-braces: ConnectorResponseTypeDef](./type_defs.md#connectorresponsetypedef) 


```python
# create_connector method usage example with argument unpacking

kwargs: CreateConnectorRequestRequestTypeDef = {  # (1)
    "name": ...,
    "ssmInstanceID": ...,
}

parent.create_connector(**kwargs)
```

1. See [:material-code-braces: CreateConnectorRequestRequestTypeDef](./type_defs.md#createconnectorrequestrequesttypedef) 

### create\_launch\_configuration\_template

Creates a new Launch Configuration Template.

Type annotations and code completion for `#!python session.create_client("mgn").create_launch_configuration_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/create_launch_configuration_template.html)

```python
# create_launch_configuration_template method definition

await def create_launch_configuration_template(
    self,
    *,
    associatePublicIpAddress: bool = ...,
    bootMode: BootModeType = ...,  # (1)
    copyPrivateIp: bool = ...,
    copyTags: bool = ...,
    enableMapAutoTagging: bool = ...,
    largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,  # (2)
    launchDisposition: LaunchDispositionType = ...,  # (3)
    licensing: LicensingTypeDef = ...,  # (4)
    mapAutoTaggingMpeID: str = ...,
    postLaunchActions: PostLaunchActionsTypeDef = ...,  # (5)
    smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,  # (2)
    smallVolumeMaxSize: int = ...,
    tags: Mapping[str, str] = ...,
    targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,  # (7)
) -> LaunchConfigurationTemplateResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype) 
2. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
3. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
4. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
5. See [:material-code-braces: PostLaunchActionsTypeDef](./type_defs.md#postlaunchactionstypedef) 
6. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
7. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
8. See [:material-code-braces: LaunchConfigurationTemplateResponseTypeDef](./type_defs.md#launchconfigurationtemplateresponsetypedef) 


```python
# create_launch_configuration_template method usage example with argument unpacking

kwargs: CreateLaunchConfigurationTemplateRequestRequestTypeDef = {  # (1)
    "associatePublicIpAddress": ...,
}

parent.create_launch_configuration_template(**kwargs)
```

1. See [:material-code-braces: CreateLaunchConfigurationTemplateRequestRequestTypeDef](./type_defs.md#createlaunchconfigurationtemplaterequestrequesttypedef) 

### create\_replication\_configuration\_template

Creates a new ReplicationConfigurationTemplate.

Type annotations and code completion for `#!python session.create_client("mgn").create_replication_configuration_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/create_replication_configuration_template.html)

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
    replicationServerInstanceType: str,
    replicationServersSecurityGroupsIDs: Sequence[str],
    stagingAreaSubnetId: str,
    stagingAreaTags: Mapping[str, str],
    useDedicatedReplicationServer: bool,
    ebsEncryptionKeyArn: str = ...,
    tags: Mapping[str, str] = ...,
    useFipsEndpoint: bool = ...,
) -> ReplicationConfigurationTemplateResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: ReplicationConfigurationTemplateResponseTypeDef](./type_defs.md#replicationconfigurationtemplateresponsetypedef) 


```python
# create_replication_configuration_template method usage example with argument unpacking

kwargs: CreateReplicationConfigurationTemplateRequestRequestTypeDef = {  # (1)
    "associateDefaultSecurityGroup": ...,
    "bandwidthThrottling": ...,
    "createPublicIP": ...,
    "dataPlaneRouting": ...,
    "defaultLargeStagingDiskType": ...,
    "ebsEncryption": ...,
    "replicationServerInstanceType": ...,
    "replicationServersSecurityGroupsIDs": ...,
    "stagingAreaSubnetId": ...,
    "stagingAreaTags": ...,
    "useDedicatedReplicationServer": ...,
}

parent.create_replication_configuration_template(**kwargs)
```

1. See [:material-code-braces: CreateReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#createreplicationconfigurationtemplaterequestrequesttypedef) 

### create\_wave

Create wave.

Type annotations and code completion for `#!python session.create_client("mgn").create_wave` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/create_wave.html)

```python
# create_wave method definition

await def create_wave(
    self,
    *,
    name: str,
    accountID: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> WaveResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: WaveResponseTypeDef](./type_defs.md#waveresponsetypedef) 


```python
# create_wave method usage example with argument unpacking

kwargs: CreateWaveRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_wave(**kwargs)
```

1. See [:material-code-braces: CreateWaveRequestRequestTypeDef](./type_defs.md#createwaverequestrequesttypedef) 

### delete\_application

Delete application.

Type annotations and code completion for `#!python session.create_client("mgn").delete_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/delete_application.html)

```python
# delete_application method definition

await def delete_application(
    self,
    *,
    applicationID: str,
    accountID: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_application method usage example with argument unpacking

kwargs: DeleteApplicationRequestRequestTypeDef = {  # (1)
    "applicationID": ...,
}

parent.delete_application(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef) 

### delete\_connector

Delete Connector.

Type annotations and code completion for `#!python session.create_client("mgn").delete_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/delete_connector.html)

```python
# delete_connector method definition

await def delete_connector(
    self,
    *,
    connectorID: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_connector method usage example with argument unpacking

kwargs: DeleteConnectorRequestRequestTypeDef = {  # (1)
    "connectorID": ...,
}

parent.delete_connector(**kwargs)
```

1. See [:material-code-braces: DeleteConnectorRequestRequestTypeDef](./type_defs.md#deleteconnectorrequestrequesttypedef) 

### delete\_job

Deletes a single Job by ID.

Type annotations and code completion for `#!python session.create_client("mgn").delete_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/delete_job.html)

```python
# delete_job method definition

await def delete_job(
    self,
    *,
    jobID: str,
    accountID: str = ...,
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

Type annotations and code completion for `#!python session.create_client("mgn").delete_launch_configuration_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/delete_launch_configuration_template.html)

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

### delete\_replication\_configuration\_template

Deletes a single Replication Configuration Template by ID.

Type annotations and code completion for `#!python session.create_client("mgn").delete_replication_configuration_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/delete_replication_configuration_template.html)

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

### delete\_source\_server

Deletes a single source server by ID.

Type annotations and code completion for `#!python session.create_client("mgn").delete_source_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/delete_source_server.html)

```python
# delete_source_server method definition

await def delete_source_server(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
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

### delete\_vcenter\_client

Deletes a given vCenter client by ID.

Type annotations and code completion for `#!python session.create_client("mgn").delete_vcenter_client` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/delete_vcenter_client.html)

```python
# delete_vcenter_client method definition

await def delete_vcenter_client(
    self,
    *,
    vcenterClientID: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_vcenter_client method usage example with argument unpacking

kwargs: DeleteVcenterClientRequestRequestTypeDef = {  # (1)
    "vcenterClientID": ...,
}

parent.delete_vcenter_client(**kwargs)
```

1. See [:material-code-braces: DeleteVcenterClientRequestRequestTypeDef](./type_defs.md#deletevcenterclientrequestrequesttypedef) 

### delete\_wave

Delete wave.

Type annotations and code completion for `#!python session.create_client("mgn").delete_wave` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/delete_wave.html)

```python
# delete_wave method definition

await def delete_wave(
    self,
    *,
    waveID: str,
    accountID: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_wave method usage example with argument unpacking

kwargs: DeleteWaveRequestRequestTypeDef = {  # (1)
    "waveID": ...,
}

parent.delete_wave(**kwargs)
```

1. See [:material-code-braces: DeleteWaveRequestRequestTypeDef](./type_defs.md#deletewaverequestrequesttypedef) 

### describe\_job\_log\_items

Retrieves detailed job log items with paging.

Type annotations and code completion for `#!python session.create_client("mgn").describe_job_log_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/describe_job_log_items.html)

```python
# describe_job_log_items method definition

await def describe_job_log_items(
    self,
    *,
    jobID: str,
    accountID: str = ...,
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

Type annotations and code completion for `#!python session.create_client("mgn").describe_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/describe_jobs.html)

```python
# describe_jobs method definition

await def describe_jobs(
    self,
    *,
    accountID: str = ...,
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
    "accountID": ...,
}

parent.describe_jobs(**kwargs)
```

1. See [:material-code-braces: DescribeJobsRequestRequestTypeDef](./type_defs.md#describejobsrequestrequesttypedef) 

### describe\_launch\_configuration\_templates

Lists all Launch Configuration Templates, filtered by Launch Configuration
Template IDs.

Type annotations and code completion for `#!python session.create_client("mgn").describe_launch_configuration_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/describe_launch_configuration_templates.html)

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

### describe\_replication\_configuration\_templates

Lists all ReplicationConfigurationTemplates, filtered by Source Server IDs.

Type annotations and code completion for `#!python session.create_client("mgn").describe_replication_configuration_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/describe_replication_configuration_templates.html)

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

### describe\_source\_servers

Retrieves all SourceServers or multiple SourceServers by ID.

Type annotations and code completion for `#!python session.create_client("mgn").describe_source_servers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/describe_source_servers.html)

```python
# describe_source_servers method definition

await def describe_source_servers(
    self,
    *,
    accountID: str = ...,
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
    "accountID": ...,
}

parent.describe_source_servers(**kwargs)
```

1. See [:material-code-braces: DescribeSourceServersRequestRequestTypeDef](./type_defs.md#describesourceserversrequestrequesttypedef) 

### describe\_vcenter\_clients

Returns a list of the installed vCenter clients.

Type annotations and code completion for `#!python session.create_client("mgn").describe_vcenter_clients` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/describe_vcenter_clients.html)

```python
# describe_vcenter_clients method definition

await def describe_vcenter_clients(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeVcenterClientsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVcenterClientsResponseTypeDef](./type_defs.md#describevcenterclientsresponsetypedef) 


```python
# describe_vcenter_clients method usage example with argument unpacking

kwargs: DescribeVcenterClientsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.describe_vcenter_clients(**kwargs)
```

1. See [:material-code-braces: DescribeVcenterClientsRequestRequestTypeDef](./type_defs.md#describevcenterclientsrequestrequesttypedef) 

### disassociate\_applications

Disassociate applications from wave.

Type annotations and code completion for `#!python session.create_client("mgn").disassociate_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/disassociate_applications.html)

```python
# disassociate_applications method definition

await def disassociate_applications(
    self,
    *,
    applicationIDs: Sequence[str],
    waveID: str,
    accountID: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_applications method usage example with argument unpacking

kwargs: DisassociateApplicationsRequestRequestTypeDef = {  # (1)
    "applicationIDs": ...,
    "waveID": ...,
}

parent.disassociate_applications(**kwargs)
```

1. See [:material-code-braces: DisassociateApplicationsRequestRequestTypeDef](./type_defs.md#disassociateapplicationsrequestrequesttypedef) 

### disassociate\_source\_servers

Disassociate source servers from application.

Type annotations and code completion for `#!python session.create_client("mgn").disassociate_source_servers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/disassociate_source_servers.html)

```python
# disassociate_source_servers method definition

await def disassociate_source_servers(
    self,
    *,
    applicationID: str,
    sourceServerIDs: Sequence[str],
    accountID: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_source_servers method usage example with argument unpacking

kwargs: DisassociateSourceServersRequestRequestTypeDef = {  # (1)
    "applicationID": ...,
    "sourceServerIDs": ...,
}

parent.disassociate_source_servers(**kwargs)
```

1. See [:material-code-braces: DisassociateSourceServersRequestRequestTypeDef](./type_defs.md#disassociatesourceserversrequestrequesttypedef) 

### disconnect\_from\_service

Disconnects specific Source Servers from Application Migration Service.

Type annotations and code completion for `#!python session.create_client("mgn").disconnect_from_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/disconnect_from_service.html)

```python
# disconnect_from_service method definition

await def disconnect_from_service(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
) -> SourceServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef) 


```python
# disconnect_from_service method usage example with argument unpacking

kwargs: DisconnectFromServiceRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.disconnect_from_service(**kwargs)
```

1. See [:material-code-braces: DisconnectFromServiceRequestRequestTypeDef](./type_defs.md#disconnectfromservicerequestrequesttypedef) 

### finalize\_cutover

Finalizes the cutover immediately for specific Source Servers.

Type annotations and code completion for `#!python session.create_client("mgn").finalize_cutover` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/finalize_cutover.html)

```python
# finalize_cutover method definition

await def finalize_cutover(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
) -> SourceServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef) 


```python
# finalize_cutover method usage example with argument unpacking

kwargs: FinalizeCutoverRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.finalize_cutover(**kwargs)
```

1. See [:material-code-braces: FinalizeCutoverRequestRequestTypeDef](./type_defs.md#finalizecutoverrequestrequesttypedef) 

### get\_launch\_configuration

Lists all LaunchConfigurations available, filtered by Source Server IDs.

Type annotations and code completion for `#!python session.create_client("mgn").get_launch_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/get_launch_configuration.html)

```python
# get_launch_configuration method definition

await def get_launch_configuration(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
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

Lists all ReplicationConfigurations, filtered by Source Server ID.

Type annotations and code completion for `#!python session.create_client("mgn").get_replication_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/get_replication_configuration.html)

```python
# get_replication_configuration method definition

await def get_replication_configuration(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
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

Initialize Application Migration Service.

Type annotations and code completion for `#!python session.create_client("mgn").initialize_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/initialize_service.html)

```python
# initialize_service method definition

await def initialize_service(
    self,
) -> Dict[str, Any]:
    ...
```


### list\_applications

Retrieves all applications or multiple applications by ID.

Type annotations and code completion for `#!python session.create_client("mgn").list_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/list_applications.html)

```python
# list_applications method definition

await def list_applications(
    self,
    *,
    accountID: str = ...,
    filters: ListApplicationsRequestFiltersTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListApplicationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListApplicationsRequestFiltersTypeDef](./type_defs.md#listapplicationsrequestfilterstypedef) 
2. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python
# list_applications method usage example with argument unpacking

kwargs: ListApplicationsRequestRequestTypeDef = {  # (1)
    "accountID": ...,
}

parent.list_applications(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef) 

### list\_connectors

List Connectors.

Type annotations and code completion for `#!python session.create_client("mgn").list_connectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/list_connectors.html)

```python
# list_connectors method definition

await def list_connectors(
    self,
    *,
    filters: ListConnectorsRequestFiltersTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListConnectorsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListConnectorsRequestFiltersTypeDef](./type_defs.md#listconnectorsrequestfilterstypedef) 
2. See [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


```python
# list_connectors method usage example with argument unpacking

kwargs: ListConnectorsRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_connectors(**kwargs)
```

1. See [:material-code-braces: ListConnectorsRequestRequestTypeDef](./type_defs.md#listconnectorsrequestrequesttypedef) 

### list\_export\_errors

List export errors.

Type annotations and code completion for `#!python session.create_client("mgn").list_export_errors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/list_export_errors.html)

```python
# list_export_errors method definition

await def list_export_errors(
    self,
    *,
    exportID: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListExportErrorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListExportErrorsResponseTypeDef](./type_defs.md#listexporterrorsresponsetypedef) 


```python
# list_export_errors method usage example with argument unpacking

kwargs: ListExportErrorsRequestRequestTypeDef = {  # (1)
    "exportID": ...,
}

parent.list_export_errors(**kwargs)
```

1. See [:material-code-braces: ListExportErrorsRequestRequestTypeDef](./type_defs.md#listexporterrorsrequestrequesttypedef) 

### list\_exports

List exports.

Type annotations and code completion for `#!python session.create_client("mgn").list_exports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/list_exports.html)

```python
# list_exports method definition

await def list_exports(
    self,
    *,
    filters: ListExportsRequestFiltersTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListExportsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListExportsRequestFiltersTypeDef](./type_defs.md#listexportsrequestfilterstypedef) 
2. See [:material-code-braces: ListExportsResponseTypeDef](./type_defs.md#listexportsresponsetypedef) 


```python
# list_exports method usage example with argument unpacking

kwargs: ListExportsRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_exports(**kwargs)
```

1. See [:material-code-braces: ListExportsRequestRequestTypeDef](./type_defs.md#listexportsrequestrequesttypedef) 

### list\_import\_errors

List import errors.

Type annotations and code completion for `#!python session.create_client("mgn").list_import_errors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/list_import_errors.html)

```python
# list_import_errors method definition

await def list_import_errors(
    self,
    *,
    importID: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListImportErrorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListImportErrorsResponseTypeDef](./type_defs.md#listimporterrorsresponsetypedef) 


```python
# list_import_errors method usage example with argument unpacking

kwargs: ListImportErrorsRequestRequestTypeDef = {  # (1)
    "importID": ...,
}

parent.list_import_errors(**kwargs)
```

1. See [:material-code-braces: ListImportErrorsRequestRequestTypeDef](./type_defs.md#listimporterrorsrequestrequesttypedef) 

### list\_imports

List imports.

Type annotations and code completion for `#!python session.create_client("mgn").list_imports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/list_imports.html)

```python
# list_imports method definition

await def list_imports(
    self,
    *,
    filters: ListImportsRequestFiltersTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListImportsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListImportsRequestFiltersTypeDef](./type_defs.md#listimportsrequestfilterstypedef) 
2. See [:material-code-braces: ListImportsResponseTypeDef](./type_defs.md#listimportsresponsetypedef) 


```python
# list_imports method usage example with argument unpacking

kwargs: ListImportsRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_imports(**kwargs)
```

1. See [:material-code-braces: ListImportsRequestRequestTypeDef](./type_defs.md#listimportsrequestrequesttypedef) 

### list\_managed\_accounts

List Managed Accounts.

Type annotations and code completion for `#!python session.create_client("mgn").list_managed_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/list_managed_accounts.html)

```python
# list_managed_accounts method definition

await def list_managed_accounts(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListManagedAccountsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListManagedAccountsResponseTypeDef](./type_defs.md#listmanagedaccountsresponsetypedef) 


```python
# list_managed_accounts method usage example with argument unpacking

kwargs: ListManagedAccountsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_managed_accounts(**kwargs)
```

1. See [:material-code-braces: ListManagedAccountsRequestRequestTypeDef](./type_defs.md#listmanagedaccountsrequestrequesttypedef) 

### list\_source\_server\_actions

List source server post migration custom actions.

Type annotations and code completion for `#!python session.create_client("mgn").list_source_server_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/list_source_server_actions.html)

```python
# list_source_server_actions method definition

await def list_source_server_actions(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
    filters: SourceServerActionsRequestFiltersTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSourceServerActionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SourceServerActionsRequestFiltersTypeDef](./type_defs.md#sourceserveractionsrequestfilterstypedef) 
2. See [:material-code-braces: ListSourceServerActionsResponseTypeDef](./type_defs.md#listsourceserveractionsresponsetypedef) 


```python
# list_source_server_actions method usage example with argument unpacking

kwargs: ListSourceServerActionsRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.list_source_server_actions(**kwargs)
```

1. See [:material-code-braces: ListSourceServerActionsRequestRequestTypeDef](./type_defs.md#listsourceserveractionsrequestrequesttypedef) 

### list\_tags\_for\_resource

List all tags for your Application Migration Service resources.

Type annotations and code completion for `#!python session.create_client("mgn").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/list_tags_for_resource.html)

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

### list\_template\_actions

List template post migration custom actions.

Type annotations and code completion for `#!python session.create_client("mgn").list_template_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/list_template_actions.html)

```python
# list_template_actions method definition

await def list_template_actions(
    self,
    *,
    launchConfigurationTemplateID: str,
    filters: TemplateActionsRequestFiltersTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTemplateActionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TemplateActionsRequestFiltersTypeDef](./type_defs.md#templateactionsrequestfilterstypedef) 
2. See [:material-code-braces: ListTemplateActionsResponseTypeDef](./type_defs.md#listtemplateactionsresponsetypedef) 


```python
# list_template_actions method usage example with argument unpacking

kwargs: ListTemplateActionsRequestRequestTypeDef = {  # (1)
    "launchConfigurationTemplateID": ...,
}

parent.list_template_actions(**kwargs)
```

1. See [:material-code-braces: ListTemplateActionsRequestRequestTypeDef](./type_defs.md#listtemplateactionsrequestrequesttypedef) 

### list\_waves

Retrieves all waves or multiple waves by ID.

Type annotations and code completion for `#!python session.create_client("mgn").list_waves` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/list_waves.html)

```python
# list_waves method definition

await def list_waves(
    self,
    *,
    accountID: str = ...,
    filters: ListWavesRequestFiltersTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWavesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListWavesRequestFiltersTypeDef](./type_defs.md#listwavesrequestfilterstypedef) 
2. See [:material-code-braces: ListWavesResponseTypeDef](./type_defs.md#listwavesresponsetypedef) 


```python
# list_waves method usage example with argument unpacking

kwargs: ListWavesRequestRequestTypeDef = {  # (1)
    "accountID": ...,
}

parent.list_waves(**kwargs)
```

1. See [:material-code-braces: ListWavesRequestRequestTypeDef](./type_defs.md#listwavesrequestrequesttypedef) 

### mark\_as\_archived

Archives specific Source Servers by setting the SourceServer.isArchived
property to true for specified SourceServers by ID.

Type annotations and code completion for `#!python session.create_client("mgn").mark_as_archived` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/mark_as_archived.html)

```python
# mark_as_archived method definition

await def mark_as_archived(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
) -> SourceServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef) 


```python
# mark_as_archived method usage example with argument unpacking

kwargs: MarkAsArchivedRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.mark_as_archived(**kwargs)
```

1. See [:material-code-braces: MarkAsArchivedRequestRequestTypeDef](./type_defs.md#markasarchivedrequestrequesttypedef) 

### pause\_replication

Pause Replication.

Type annotations and code completion for `#!python session.create_client("mgn").pause_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/pause_replication.html)

```python
# pause_replication method definition

await def pause_replication(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
) -> SourceServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef) 


```python
# pause_replication method usage example with argument unpacking

kwargs: PauseReplicationRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.pause_replication(**kwargs)
```

1. See [:material-code-braces: PauseReplicationRequestRequestTypeDef](./type_defs.md#pausereplicationrequestrequesttypedef) 

### put\_source\_server\_action

Put source server post migration custom action.

Type annotations and code completion for `#!python session.create_client("mgn").put_source_server_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/put_source_server_action.html)

```python
# put_source_server_action method definition

await def put_source_server_action(
    self,
    *,
    actionID: str,
    actionName: str,
    documentIdentifier: str,
    order: int,
    sourceServerID: str,
    accountID: str = ...,
    active: bool = ...,
    category: ActionCategoryType = ...,  # (1)
    description: str = ...,
    documentVersion: str = ...,
    externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,  # (2)
    mustSucceedForCutover: bool = ...,
    parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,  # (3)
    timeoutSeconds: int = ...,
) -> SourceServerActionDocumentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype) 
2. See [:material-code-braces: SsmExternalParameterTypeDef](./type_defs.md#ssmexternalparametertypedef) 
3. See [:material-code-braces: SsmParameterStoreParameterTypeDef](./type_defs.md#ssmparameterstoreparametertypedef) 
4. See [:material-code-braces: SourceServerActionDocumentResponseTypeDef](./type_defs.md#sourceserveractiondocumentresponsetypedef) 


```python
# put_source_server_action method usage example with argument unpacking

kwargs: PutSourceServerActionRequestRequestTypeDef = {  # (1)
    "actionID": ...,
    "actionName": ...,
    "documentIdentifier": ...,
    "order": ...,
    "sourceServerID": ...,
}

parent.put_source_server_action(**kwargs)
```

1. See [:material-code-braces: PutSourceServerActionRequestRequestTypeDef](./type_defs.md#putsourceserveractionrequestrequesttypedef) 

### put\_template\_action

Put template post migration custom action.

Type annotations and code completion for `#!python session.create_client("mgn").put_template_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/put_template_action.html)

```python
# put_template_action method definition

await def put_template_action(
    self,
    *,
    actionID: str,
    actionName: str,
    documentIdentifier: str,
    launchConfigurationTemplateID: str,
    order: int,
    active: bool = ...,
    category: ActionCategoryType = ...,  # (1)
    description: str = ...,
    documentVersion: str = ...,
    externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,  # (2)
    mustSucceedForCutover: bool = ...,
    operatingSystem: str = ...,
    parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,  # (3)
    timeoutSeconds: int = ...,
) -> TemplateActionDocumentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype) 
2. See [:material-code-braces: SsmExternalParameterTypeDef](./type_defs.md#ssmexternalparametertypedef) 
3. See [:material-code-braces: SsmParameterStoreParameterTypeDef](./type_defs.md#ssmparameterstoreparametertypedef) 
4. See [:material-code-braces: TemplateActionDocumentResponseTypeDef](./type_defs.md#templateactiondocumentresponsetypedef) 


```python
# put_template_action method usage example with argument unpacking

kwargs: PutTemplateActionRequestRequestTypeDef = {  # (1)
    "actionID": ...,
    "actionName": ...,
    "documentIdentifier": ...,
    "launchConfigurationTemplateID": ...,
    "order": ...,
}

parent.put_template_action(**kwargs)
```

1. See [:material-code-braces: PutTemplateActionRequestRequestTypeDef](./type_defs.md#puttemplateactionrequestrequesttypedef) 

### remove\_source\_server\_action

Remove source server post migration custom action.

Type annotations and code completion for `#!python session.create_client("mgn").remove_source_server_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/remove_source_server_action.html)

```python
# remove_source_server_action method definition

await def remove_source_server_action(
    self,
    *,
    actionID: str,
    sourceServerID: str,
    accountID: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# remove_source_server_action method usage example with argument unpacking

kwargs: RemoveSourceServerActionRequestRequestTypeDef = {  # (1)
    "actionID": ...,
    "sourceServerID": ...,
}

parent.remove_source_server_action(**kwargs)
```

1. See [:material-code-braces: RemoveSourceServerActionRequestRequestTypeDef](./type_defs.md#removesourceserveractionrequestrequesttypedef) 

### remove\_template\_action

Remove template post migration custom action.

Type annotations and code completion for `#!python session.create_client("mgn").remove_template_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/remove_template_action.html)

```python
# remove_template_action method definition

await def remove_template_action(
    self,
    *,
    actionID: str,
    launchConfigurationTemplateID: str,
) -> Dict[str, Any]:
    ...
```



```python
# remove_template_action method usage example with argument unpacking

kwargs: RemoveTemplateActionRequestRequestTypeDef = {  # (1)
    "actionID": ...,
    "launchConfigurationTemplateID": ...,
}

parent.remove_template_action(**kwargs)
```

1. See [:material-code-braces: RemoveTemplateActionRequestRequestTypeDef](./type_defs.md#removetemplateactionrequestrequesttypedef) 

### resume\_replication

Resume Replication.

Type annotations and code completion for `#!python session.create_client("mgn").resume_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/resume_replication.html)

```python
# resume_replication method definition

await def resume_replication(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
) -> SourceServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef) 


```python
# resume_replication method usage example with argument unpacking

kwargs: ResumeReplicationRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.resume_replication(**kwargs)
```

1. See [:material-code-braces: ResumeReplicationRequestRequestTypeDef](./type_defs.md#resumereplicationrequestrequesttypedef) 

### retry\_data\_replication

Causes the data replication initiation sequence to begin immediately upon next
Handshake for specified SourceServer IDs, regardless of when the previous
initiation started.

Type annotations and code completion for `#!python session.create_client("mgn").retry_data_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/retry_data_replication.html)

```python
# retry_data_replication method definition

await def retry_data_replication(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
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

### start\_cutover

Launches a Cutover Instance for specific Source Servers.

Type annotations and code completion for `#!python session.create_client("mgn").start_cutover` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/start_cutover.html)

```python
# start_cutover method definition

await def start_cutover(
    self,
    *,
    sourceServerIDs: Sequence[str],
    accountID: str = ...,
    tags: Mapping[str, str] = ...,
) -> StartCutoverResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartCutoverResponseTypeDef](./type_defs.md#startcutoverresponsetypedef) 


```python
# start_cutover method usage example with argument unpacking

kwargs: StartCutoverRequestRequestTypeDef = {  # (1)
    "sourceServerIDs": ...,
}

parent.start_cutover(**kwargs)
```

1. See [:material-code-braces: StartCutoverRequestRequestTypeDef](./type_defs.md#startcutoverrequestrequesttypedef) 

### start\_export

Start export.

Type annotations and code completion for `#!python session.create_client("mgn").start_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/start_export.html)

```python
# start_export method definition

await def start_export(
    self,
    *,
    s3Bucket: str,
    s3Key: str,
    s3BucketOwner: str = ...,
) -> StartExportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartExportResponseTypeDef](./type_defs.md#startexportresponsetypedef) 


```python
# start_export method usage example with argument unpacking

kwargs: StartExportRequestRequestTypeDef = {  # (1)
    "s3Bucket": ...,
    "s3Key": ...,
}

parent.start_export(**kwargs)
```

1. See [:material-code-braces: StartExportRequestRequestTypeDef](./type_defs.md#startexportrequestrequesttypedef) 

### start\_import

Start import.

Type annotations and code completion for `#!python session.create_client("mgn").start_import` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/start_import.html)

```python
# start_import method definition

await def start_import(
    self,
    *,
    s3BucketSource: S3BucketSourceTypeDef,  # (1)
    clientToken: str = ...,
) -> StartImportResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: S3BucketSourceTypeDef](./type_defs.md#s3bucketsourcetypedef) 
2. See [:material-code-braces: StartImportResponseTypeDef](./type_defs.md#startimportresponsetypedef) 


```python
# start_import method usage example with argument unpacking

kwargs: StartImportRequestRequestTypeDef = {  # (1)
    "s3BucketSource": ...,
}

parent.start_import(**kwargs)
```

1. See [:material-code-braces: StartImportRequestRequestTypeDef](./type_defs.md#startimportrequestrequesttypedef) 

### start\_replication

Starts replication for SNAPSHOT_SHIPPING agents.

Type annotations and code completion for `#!python session.create_client("mgn").start_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/start_replication.html)

```python
# start_replication method definition

await def start_replication(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
) -> SourceServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef) 


```python
# start_replication method usage example with argument unpacking

kwargs: StartReplicationRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.start_replication(**kwargs)
```

1. See [:material-code-braces: StartReplicationRequestRequestTypeDef](./type_defs.md#startreplicationrequestrequesttypedef) 

### start\_test

Launches a Test Instance for specific Source Servers.

Type annotations and code completion for `#!python session.create_client("mgn").start_test` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/start_test.html)

```python
# start_test method definition

await def start_test(
    self,
    *,
    sourceServerIDs: Sequence[str],
    accountID: str = ...,
    tags: Mapping[str, str] = ...,
) -> StartTestResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartTestResponseTypeDef](./type_defs.md#starttestresponsetypedef) 


```python
# start_test method usage example with argument unpacking

kwargs: StartTestRequestRequestTypeDef = {  # (1)
    "sourceServerIDs": ...,
}

parent.start_test(**kwargs)
```

1. See [:material-code-braces: StartTestRequestRequestTypeDef](./type_defs.md#starttestrequestrequesttypedef) 

### stop\_replication

Stop Replication.

Type annotations and code completion for `#!python session.create_client("mgn").stop_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/stop_replication.html)

```python
# stop_replication method definition

await def stop_replication(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
) -> SourceServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef) 


```python
# stop_replication method usage example with argument unpacking

kwargs: StopReplicationRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.stop_replication(**kwargs)
```

1. See [:material-code-braces: StopReplicationRequestRequestTypeDef](./type_defs.md#stopreplicationrequestrequesttypedef) 

### tag\_resource

Adds or overwrites only the specified tags for the specified Application
Migration Service resource or resources.

Type annotations and code completion for `#!python session.create_client("mgn").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/tag_resource.html)

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

### terminate\_target\_instances

Starts a job that terminates specific launched EC2 Test and Cutover instances.

Type annotations and code completion for `#!python session.create_client("mgn").terminate_target_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/terminate_target_instances.html)

```python
# terminate_target_instances method definition

await def terminate_target_instances(
    self,
    *,
    sourceServerIDs: Sequence[str],
    accountID: str = ...,
    tags: Mapping[str, str] = ...,
) -> TerminateTargetInstancesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TerminateTargetInstancesResponseTypeDef](./type_defs.md#terminatetargetinstancesresponsetypedef) 


```python
# terminate_target_instances method usage example with argument unpacking

kwargs: TerminateTargetInstancesRequestRequestTypeDef = {  # (1)
    "sourceServerIDs": ...,
}

parent.terminate_target_instances(**kwargs)
```

1. See [:material-code-braces: TerminateTargetInstancesRequestRequestTypeDef](./type_defs.md#terminatetargetinstancesrequestrequesttypedef) 

### unarchive\_application

Unarchive application.

Type annotations and code completion for `#!python session.create_client("mgn").unarchive_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/unarchive_application.html)

```python
# unarchive_application method definition

await def unarchive_application(
    self,
    *,
    applicationID: str,
    accountID: str = ...,
) -> ApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef) 


```python
# unarchive_application method usage example with argument unpacking

kwargs: UnarchiveApplicationRequestRequestTypeDef = {  # (1)
    "applicationID": ...,
}

parent.unarchive_application(**kwargs)
```

1. See [:material-code-braces: UnarchiveApplicationRequestRequestTypeDef](./type_defs.md#unarchiveapplicationrequestrequesttypedef) 

### unarchive\_wave

Unarchive wave.

Type annotations and code completion for `#!python session.create_client("mgn").unarchive_wave` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/unarchive_wave.html)

```python
# unarchive_wave method definition

await def unarchive_wave(
    self,
    *,
    waveID: str,
    accountID: str = ...,
) -> WaveResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: WaveResponseTypeDef](./type_defs.md#waveresponsetypedef) 


```python
# unarchive_wave method usage example with argument unpacking

kwargs: UnarchiveWaveRequestRequestTypeDef = {  # (1)
    "waveID": ...,
}

parent.unarchive_wave(**kwargs)
```

1. See [:material-code-braces: UnarchiveWaveRequestRequestTypeDef](./type_defs.md#unarchivewaverequestrequesttypedef) 

### untag\_resource

Deletes the specified set of tags from the specified set of Application
Migration Service resources.

Type annotations and code completion for `#!python session.create_client("mgn").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/untag_resource.html)

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

### update\_application

Update application.

Type annotations and code completion for `#!python session.create_client("mgn").update_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/update_application.html)

```python
# update_application method definition

await def update_application(
    self,
    *,
    applicationID: str,
    accountID: str = ...,
    description: str = ...,
    name: str = ...,
) -> ApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef) 


```python
# update_application method usage example with argument unpacking

kwargs: UpdateApplicationRequestRequestTypeDef = {  # (1)
    "applicationID": ...,
}

parent.update_application(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef) 

### update\_connector

Update Connector.

Type annotations and code completion for `#!python session.create_client("mgn").update_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/update_connector.html)

```python
# update_connector method definition

await def update_connector(
    self,
    *,
    connectorID: str,
    name: str = ...,
    ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...,  # (1)
) -> ConnectorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConnectorSsmCommandConfigTypeDef](./type_defs.md#connectorssmcommandconfigtypedef) 
2. See [:material-code-braces: ConnectorResponseTypeDef](./type_defs.md#connectorresponsetypedef) 


```python
# update_connector method usage example with argument unpacking

kwargs: UpdateConnectorRequestRequestTypeDef = {  # (1)
    "connectorID": ...,
}

parent.update_connector(**kwargs)
```

1. See [:material-code-braces: UpdateConnectorRequestRequestTypeDef](./type_defs.md#updateconnectorrequestrequesttypedef) 

### update\_launch\_configuration

Updates multiple LaunchConfigurations by Source Server ID.

Type annotations and code completion for `#!python session.create_client("mgn").update_launch_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/update_launch_configuration.html)

```python
# update_launch_configuration method definition

await def update_launch_configuration(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
    bootMode: BootModeType = ...,  # (1)
    copyPrivateIp: bool = ...,
    copyTags: bool = ...,
    enableMapAutoTagging: bool = ...,
    launchDisposition: LaunchDispositionType = ...,  # (2)
    licensing: LicensingTypeDef = ...,  # (3)
    mapAutoTaggingMpeID: str = ...,
    name: str = ...,
    postLaunchActions: PostLaunchActionsTypeDef = ...,  # (4)
    targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,  # (5)
) -> LaunchConfigurationTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype) 
2. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
3. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
4. See [:material-code-braces: PostLaunchActionsTypeDef](./type_defs.md#postlaunchactionstypedef) 
5. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
6. See [:material-code-braces: LaunchConfigurationTypeDef](./type_defs.md#launchconfigurationtypedef) 


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

Type annotations and code completion for `#!python session.create_client("mgn").update_launch_configuration_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/update_launch_configuration_template.html)

```python
# update_launch_configuration_template method definition

await def update_launch_configuration_template(
    self,
    *,
    launchConfigurationTemplateID: str,
    associatePublicIpAddress: bool = ...,
    bootMode: BootModeType = ...,  # (1)
    copyPrivateIp: bool = ...,
    copyTags: bool = ...,
    enableMapAutoTagging: bool = ...,
    largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,  # (2)
    launchDisposition: LaunchDispositionType = ...,  # (3)
    licensing: LicensingTypeDef = ...,  # (4)
    mapAutoTaggingMpeID: str = ...,
    postLaunchActions: PostLaunchActionsTypeDef = ...,  # (5)
    smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,  # (2)
    smallVolumeMaxSize: int = ...,
    targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,  # (7)
) -> LaunchConfigurationTemplateResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype) 
2. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
3. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
4. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
5. See [:material-code-braces: PostLaunchActionsTypeDef](./type_defs.md#postlaunchactionstypedef) 
6. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
7. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
8. See [:material-code-braces: LaunchConfigurationTemplateResponseTypeDef](./type_defs.md#launchconfigurationtemplateresponsetypedef) 


```python
# update_launch_configuration_template method usage example with argument unpacking

kwargs: UpdateLaunchConfigurationTemplateRequestRequestTypeDef = {  # (1)
    "launchConfigurationTemplateID": ...,
}

parent.update_launch_configuration_template(**kwargs)
```

1. See [:material-code-braces: UpdateLaunchConfigurationTemplateRequestRequestTypeDef](./type_defs.md#updatelaunchconfigurationtemplaterequestrequesttypedef) 

### update\_replication\_configuration

Allows you to update multiple ReplicationConfigurations by Source Server ID.

Type annotations and code completion for `#!python session.create_client("mgn").update_replication_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/update_replication_configuration.html)

```python
# update_replication_configuration method definition

await def update_replication_configuration(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
    associateDefaultSecurityGroup: bool = ...,
    bandwidthThrottling: int = ...,
    createPublicIP: bool = ...,
    dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType = ...,  # (1)
    defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,  # (2)
    ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,  # (3)
    ebsEncryptionKeyArn: str = ...,
    name: str = ...,
    replicatedDisks: Sequence[ReplicationConfigurationReplicatedDiskTypeDef] = ...,  # (4)
    replicationServerInstanceType: str = ...,
    replicationServersSecurityGroupsIDs: Sequence[str] = ...,
    stagingAreaSubnetId: str = ...,
    stagingAreaTags: Mapping[str, str] = ...,
    useDedicatedReplicationServer: bool = ...,
    useFipsEndpoint: bool = ...,
) -> ReplicationConfigurationTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: ReplicationConfigurationReplicatedDiskTypeDef](./type_defs.md#replicationconfigurationreplicateddisktypedef) 
5. See [:material-code-braces: ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef) 


```python
# update_replication_configuration method usage example with argument unpacking

kwargs: UpdateReplicationConfigurationRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.update_replication_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateReplicationConfigurationRequestRequestTypeDef](./type_defs.md#updatereplicationconfigurationrequestrequesttypedef) 

### update\_replication\_configuration\_template

Updates multiple ReplicationConfigurationTemplates by ID.

Type annotations and code completion for `#!python session.create_client("mgn").update_replication_configuration_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/update_replication_configuration_template.html)

```python
# update_replication_configuration_template method definition

await def update_replication_configuration_template(
    self,
    *,
    replicationConfigurationTemplateID: str,
    arn: str = ...,
    associateDefaultSecurityGroup: bool = ...,
    bandwidthThrottling: int = ...,
    createPublicIP: bool = ...,
    dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType = ...,  # (1)
    defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,  # (2)
    ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,  # (3)
    ebsEncryptionKeyArn: str = ...,
    replicationServerInstanceType: str = ...,
    replicationServersSecurityGroupsIDs: Sequence[str] = ...,
    stagingAreaSubnetId: str = ...,
    stagingAreaTags: Mapping[str, str] = ...,
    useDedicatedReplicationServer: bool = ...,
    useFipsEndpoint: bool = ...,
) -> ReplicationConfigurationTemplateResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: ReplicationConfigurationTemplateResponseTypeDef](./type_defs.md#replicationconfigurationtemplateresponsetypedef) 


```python
# update_replication_configuration_template method usage example with argument unpacking

kwargs: UpdateReplicationConfigurationTemplateRequestRequestTypeDef = {  # (1)
    "replicationConfigurationTemplateID": ...,
}

parent.update_replication_configuration_template(**kwargs)
```

1. See [:material-code-braces: UpdateReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#updatereplicationconfigurationtemplaterequestrequesttypedef) 

### update\_source\_server

Update Source Server.

Type annotations and code completion for `#!python session.create_client("mgn").update_source_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/update_source_server.html)

```python
# update_source_server method definition

await def update_source_server(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
    connectorAction: SourceServerConnectorActionTypeDef = ...,  # (1)
) -> SourceServerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SourceServerConnectorActionTypeDef](./type_defs.md#sourceserverconnectoractiontypedef) 
2. See [:material-code-braces: SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef) 


```python
# update_source_server method usage example with argument unpacking

kwargs: UpdateSourceServerRequestRequestTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.update_source_server(**kwargs)
```

1. See [:material-code-braces: UpdateSourceServerRequestRequestTypeDef](./type_defs.md#updatesourceserverrequestrequesttypedef) 

### update\_source\_server\_replication\_type

Allows you to change between the AGENT_BASED replication type and the
SNAPSHOT_SHIPPING replication type.

Type annotations and code completion for `#!python session.create_client("mgn").update_source_server_replication_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/update_source_server_replication_type.html)

```python
# update_source_server_replication_type method definition

await def update_source_server_replication_type(
    self,
    *,
    replicationType: ReplicationTypeType,  # (1)
    sourceServerID: str,
    accountID: str = ...,
) -> SourceServerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ReplicationTypeType](./literals.md#replicationtypetype) 
2. See [:material-code-braces: SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef) 


```python
# update_source_server_replication_type method usage example with argument unpacking

kwargs: UpdateSourceServerReplicationTypeRequestRequestTypeDef = {  # (1)
    "replicationType": ...,
    "sourceServerID": ...,
}

parent.update_source_server_replication_type(**kwargs)
```

1. See [:material-code-braces: UpdateSourceServerReplicationTypeRequestRequestTypeDef](./type_defs.md#updatesourceserverreplicationtyperequestrequesttypedef) 

### update\_wave

Update wave.

Type annotations and code completion for `#!python session.create_client("mgn").update_wave` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/client/update_wave.html)

```python
# update_wave method definition

await def update_wave(
    self,
    *,
    waveID: str,
    accountID: str = ...,
    description: str = ...,
    name: str = ...,
) -> WaveResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: WaveResponseTypeDef](./type_defs.md#waveresponsetypedef) 


```python
# update_wave method usage example with argument unpacking

kwargs: UpdateWaveRequestRequestTypeDef = {  # (1)
    "waveID": ...,
}

parent.update_wave(**kwargs)
```

1. See [:material-code-braces: UpdateWaveRequestRequestTypeDef](./type_defs.md#updatewaverequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("mgn").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#Mgn.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "MgnClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("mgn").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#Mgn.Client)

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

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator` method with overloads.

- `client.get_paginator("describe_job_log_items")` -> [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
- `client.get_paginator("describe_jobs")` -> [DescribeJobsPaginator](./paginators.md#describejobspaginator)
- `client.get_paginator("describe_launch_configuration_templates")` -> [DescribeLaunchConfigurationTemplatesPaginator](./paginators.md#describelaunchconfigurationtemplatespaginator)
- `client.get_paginator("describe_replication_configuration_templates")` -> [DescribeReplicationConfigurationTemplatesPaginator](./paginators.md#describereplicationconfigurationtemplatespaginator)
- `client.get_paginator("describe_source_servers")` -> [DescribeSourceServersPaginator](./paginators.md#describesourceserverspaginator)
- `client.get_paginator("describe_vcenter_clients")` -> [DescribeVcenterClientsPaginator](./paginators.md#describevcenterclientspaginator)
- `client.get_paginator("list_applications")` -> [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- `client.get_paginator("list_connectors")` -> [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
- `client.get_paginator("list_export_errors")` -> [ListExportErrorsPaginator](./paginators.md#listexporterrorspaginator)
- `client.get_paginator("list_exports")` -> [ListExportsPaginator](./paginators.md#listexportspaginator)
- `client.get_paginator("list_import_errors")` -> [ListImportErrorsPaginator](./paginators.md#listimporterrorspaginator)
- `client.get_paginator("list_imports")` -> [ListImportsPaginator](./paginators.md#listimportspaginator)
- `client.get_paginator("list_managed_accounts")` -> [ListManagedAccountsPaginator](./paginators.md#listmanagedaccountspaginator)
- `client.get_paginator("list_source_server_actions")` -> [ListSourceServerActionsPaginator](./paginators.md#listsourceserveractionspaginator)
- `client.get_paginator("list_template_actions")` -> [ListTemplateActionsPaginator](./paginators.md#listtemplateactionspaginator)
- `client.get_paginator("list_waves")` -> [ListWavesPaginator](./paginators.md#listwavespaginator)



