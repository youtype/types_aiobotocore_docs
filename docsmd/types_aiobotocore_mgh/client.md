# MigrationHubClient

> [Index](../README.md) > [MigrationHub](./README.md) > MigrationHubClient

!!! note ""

    Auto-generated documentation for [MigrationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#migrationhub)
    type annotations stubs module [types-aiobotocore-mgh](https://pypi.org/project/types-aiobotocore-mgh/).

## MigrationHubClient

Type annotations and code completion for `#!python session.create_client("mgh")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client)

```python
# MigrationHubClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_mgh.client import MigrationHubClient

session = get_session()
async with session.create_client("mgh") as client:
    client: MigrationHubClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("mgh").exceptions` structure.

```python
# MigrationHubClient.exceptions usage example

async with session.create_client("mgh") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.DryRunOperation,
        client.HomeRegionNotSetException,
        client.InternalServerError,
        client.InvalidInputException,
        client.PolicyErrorException,
        client.ResourceNotFoundException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
        client.UnauthorizedOperation,
    ) as e:
        print(e)
```

```python
# MigrationHubClient usage type checking example

from types_aiobotocore_mgh.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("mgh").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("mgh").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/generate_presigned_url.html)

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


### associate\_created\_artifact

Associates a created artifact of an AWS cloud resource, the target receiving
the migration, with the migration task performed by a migration tool.

Type annotations and code completion for `#!python session.create_client("mgh").associate_created_artifact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/associate_created_artifact.html)

```python
# associate_created_artifact method definition

await def associate_created_artifact(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    CreatedArtifact: CreatedArtifactTypeDef,  # (1)
    DryRun: bool = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: CreatedArtifactTypeDef](./type_defs.md#createdartifacttypedef) 


```python
# associate_created_artifact method usage example with argument unpacking

kwargs: AssociateCreatedArtifactRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
    "CreatedArtifact": ...,
}

parent.associate_created_artifact(**kwargs)
```

1. See [:material-code-braces: AssociateCreatedArtifactRequestRequestTypeDef](./type_defs.md#associatecreatedartifactrequestrequesttypedef) 

### associate\_discovered\_resource

Associates a discovered resource ID from Application Discovery Service with a
migration task.

Type annotations and code completion for `#!python session.create_client("mgh").associate_discovered_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/associate_discovered_resource.html)

```python
# associate_discovered_resource method definition

await def associate_discovered_resource(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    DiscoveredResource: DiscoveredResourceTypeDef,  # (1)
    DryRun: bool = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: DiscoveredResourceTypeDef](./type_defs.md#discoveredresourcetypedef) 


```python
# associate_discovered_resource method usage example with argument unpacking

kwargs: AssociateDiscoveredResourceRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
    "DiscoveredResource": ...,
}

parent.associate_discovered_resource(**kwargs)
```

1. See [:material-code-braces: AssociateDiscoveredResourceRequestRequestTypeDef](./type_defs.md#associatediscoveredresourcerequestrequesttypedef) 

### associate\_source\_resource

Associates a source resource with a migration task.

Type annotations and code completion for `#!python session.create_client("mgh").associate_source_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/associate_source_resource.html)

```python
# associate_source_resource method definition

await def associate_source_resource(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    SourceResource: SourceResourceTypeDef,  # (1)
    DryRun: bool = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: SourceResourceTypeDef](./type_defs.md#sourceresourcetypedef) 


```python
# associate_source_resource method usage example with argument unpacking

kwargs: AssociateSourceResourceRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
    "SourceResource": ...,
}

parent.associate_source_resource(**kwargs)
```

1. See [:material-code-braces: AssociateSourceResourceRequestRequestTypeDef](./type_defs.md#associatesourceresourcerequestrequesttypedef) 

### create\_progress\_update\_stream

Creates a progress update stream which is an AWS resource used for access
control as well as a namespace for migration task names that is implicitly
linked to your AWS account.

Type annotations and code completion for `#!python session.create_client("mgh").create_progress_update_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/create_progress_update_stream.html)

```python
# create_progress_update_stream method definition

await def create_progress_update_stream(
    self,
    *,
    ProgressUpdateStreamName: str,
    DryRun: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# create_progress_update_stream method usage example with argument unpacking

kwargs: CreateProgressUpdateStreamRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStreamName": ...,
}

parent.create_progress_update_stream(**kwargs)
```

1. See [:material-code-braces: CreateProgressUpdateStreamRequestRequestTypeDef](./type_defs.md#createprogressupdatestreamrequestrequesttypedef) 

### delete\_progress\_update\_stream

Deletes a progress update stream, including all of its tasks, which was
previously created as an AWS resource used for access control.

Type annotations and code completion for `#!python session.create_client("mgh").delete_progress_update_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/delete_progress_update_stream.html)

```python
# delete_progress_update_stream method definition

await def delete_progress_update_stream(
    self,
    *,
    ProgressUpdateStreamName: str,
    DryRun: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_progress_update_stream method usage example with argument unpacking

kwargs: DeleteProgressUpdateStreamRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStreamName": ...,
}

parent.delete_progress_update_stream(**kwargs)
```

1. See [:material-code-braces: DeleteProgressUpdateStreamRequestRequestTypeDef](./type_defs.md#deleteprogressupdatestreamrequestrequesttypedef) 

### describe\_application\_state

Gets the migration status of an application.

Type annotations and code completion for `#!python session.create_client("mgh").describe_application_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/describe_application_state.html)

```python
# describe_application_state method definition

await def describe_application_state(
    self,
    *,
    ApplicationId: str,
) -> DescribeApplicationStateResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeApplicationStateResultTypeDef](./type_defs.md#describeapplicationstateresulttypedef) 


```python
# describe_application_state method usage example with argument unpacking

kwargs: DescribeApplicationStateRequestRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.describe_application_state(**kwargs)
```

1. See [:material-code-braces: DescribeApplicationStateRequestRequestTypeDef](./type_defs.md#describeapplicationstaterequestrequesttypedef) 

### describe\_migration\_task

Retrieves a list of all attributes associated with a specific migration task.

Type annotations and code completion for `#!python session.create_client("mgh").describe_migration_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/describe_migration_task.html)

```python
# describe_migration_task method definition

await def describe_migration_task(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
) -> DescribeMigrationTaskResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMigrationTaskResultTypeDef](./type_defs.md#describemigrationtaskresulttypedef) 


```python
# describe_migration_task method usage example with argument unpacking

kwargs: DescribeMigrationTaskRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
}

parent.describe_migration_task(**kwargs)
```

1. See [:material-code-braces: DescribeMigrationTaskRequestRequestTypeDef](./type_defs.md#describemigrationtaskrequestrequesttypedef) 

### disassociate\_created\_artifact

Disassociates a created artifact of an AWS resource with a migration task
performed by a migration tool that was previously associated.

Type annotations and code completion for `#!python session.create_client("mgh").disassociate_created_artifact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/disassociate_created_artifact.html)

```python
# disassociate_created_artifact method definition

await def disassociate_created_artifact(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    CreatedArtifactName: str,
    DryRun: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_created_artifact method usage example with argument unpacking

kwargs: DisassociateCreatedArtifactRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
    "CreatedArtifactName": ...,
}

parent.disassociate_created_artifact(**kwargs)
```

1. See [:material-code-braces: DisassociateCreatedArtifactRequestRequestTypeDef](./type_defs.md#disassociatecreatedartifactrequestrequesttypedef) 

### disassociate\_discovered\_resource

Disassociate an Application Discovery Service discovered resource from a
migration task.

Type annotations and code completion for `#!python session.create_client("mgh").disassociate_discovered_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/disassociate_discovered_resource.html)

```python
# disassociate_discovered_resource method definition

await def disassociate_discovered_resource(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    ConfigurationId: str,
    DryRun: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_discovered_resource method usage example with argument unpacking

kwargs: DisassociateDiscoveredResourceRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
    "ConfigurationId": ...,
}

parent.disassociate_discovered_resource(**kwargs)
```

1. See [:material-code-braces: DisassociateDiscoveredResourceRequestRequestTypeDef](./type_defs.md#disassociatediscoveredresourcerequestrequesttypedef) 

### disassociate\_source\_resource

Removes the association between a source resource and a migration task.

Type annotations and code completion for `#!python session.create_client("mgh").disassociate_source_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/disassociate_source_resource.html)

```python
# disassociate_source_resource method definition

await def disassociate_source_resource(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    SourceResourceName: str,
    DryRun: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_source_resource method usage example with argument unpacking

kwargs: DisassociateSourceResourceRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
    "SourceResourceName": ...,
}

parent.disassociate_source_resource(**kwargs)
```

1. See [:material-code-braces: DisassociateSourceResourceRequestRequestTypeDef](./type_defs.md#disassociatesourceresourcerequestrequesttypedef) 

### import\_migration\_task

Registers a new migration task which represents a server, database, etc., being
migrated to AWS by a migration tool.

Type annotations and code completion for `#!python session.create_client("mgh").import_migration_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/import_migration_task.html)

```python
# import_migration_task method definition

await def import_migration_task(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    DryRun: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# import_migration_task method usage example with argument unpacking

kwargs: ImportMigrationTaskRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
}

parent.import_migration_task(**kwargs)
```

1. See [:material-code-braces: ImportMigrationTaskRequestRequestTypeDef](./type_defs.md#importmigrationtaskrequestrequesttypedef) 

### list\_application\_states

Lists all the migration statuses for your applications.

Type annotations and code completion for `#!python session.create_client("mgh").list_application_states` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/list_application_states.html)

```python
# list_application_states method definition

await def list_application_states(
    self,
    *,
    ApplicationIds: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListApplicationStatesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationStatesResultTypeDef](./type_defs.md#listapplicationstatesresulttypedef) 


```python
# list_application_states method usage example with argument unpacking

kwargs: ListApplicationStatesRequestRequestTypeDef = {  # (1)
    "ApplicationIds": ...,
}

parent.list_application_states(**kwargs)
```

1. See [:material-code-braces: ListApplicationStatesRequestRequestTypeDef](./type_defs.md#listapplicationstatesrequestrequesttypedef) 

### list\_created\_artifacts

Lists the created artifacts attached to a given migration task in an update
stream.

Type annotations and code completion for `#!python session.create_client("mgh").list_created_artifacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/list_created_artifacts.html)

```python
# list_created_artifacts method definition

await def list_created_artifacts(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListCreatedArtifactsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCreatedArtifactsResultTypeDef](./type_defs.md#listcreatedartifactsresulttypedef) 


```python
# list_created_artifacts method usage example with argument unpacking

kwargs: ListCreatedArtifactsRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
}

parent.list_created_artifacts(**kwargs)
```

1. See [:material-code-braces: ListCreatedArtifactsRequestRequestTypeDef](./type_defs.md#listcreatedartifactsrequestrequesttypedef) 

### list\_discovered\_resources

Lists discovered resources associated with the given <code>MigrationTask</code>.

Type annotations and code completion for `#!python session.create_client("mgh").list_discovered_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/list_discovered_resources.html)

```python
# list_discovered_resources method definition

await def list_discovered_resources(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDiscoveredResourcesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDiscoveredResourcesResultTypeDef](./type_defs.md#listdiscoveredresourcesresulttypedef) 


```python
# list_discovered_resources method usage example with argument unpacking

kwargs: ListDiscoveredResourcesRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
}

parent.list_discovered_resources(**kwargs)
```

1. See [:material-code-braces: ListDiscoveredResourcesRequestRequestTypeDef](./type_defs.md#listdiscoveredresourcesrequestrequesttypedef) 

### list\_migration\_task\_updates

This is a paginated API that returns all the migration-task states for the
specified <code>MigrationTaskName</code> and <code>ProgressUpdateStream</code>.

Type annotations and code completion for `#!python session.create_client("mgh").list_migration_task_updates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/list_migration_task_updates.html)

```python
# list_migration_task_updates method definition

await def list_migration_task_updates(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMigrationTaskUpdatesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMigrationTaskUpdatesResultTypeDef](./type_defs.md#listmigrationtaskupdatesresulttypedef) 


```python
# list_migration_task_updates method usage example with argument unpacking

kwargs: ListMigrationTaskUpdatesRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
}

parent.list_migration_task_updates(**kwargs)
```

1. See [:material-code-braces: ListMigrationTaskUpdatesRequestRequestTypeDef](./type_defs.md#listmigrationtaskupdatesrequestrequesttypedef) 

### list\_migration\_tasks

Lists all, or filtered by resource name, migration tasks associated with the
user account making this call.

Type annotations and code completion for `#!python session.create_client("mgh").list_migration_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/list_migration_tasks.html)

```python
# list_migration_tasks method definition

await def list_migration_tasks(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    ResourceName: str = ...,
) -> ListMigrationTasksResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMigrationTasksResultTypeDef](./type_defs.md#listmigrationtasksresulttypedef) 


```python
# list_migration_tasks method usage example with argument unpacking

kwargs: ListMigrationTasksRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_migration_tasks(**kwargs)
```

1. See [:material-code-braces: ListMigrationTasksRequestRequestTypeDef](./type_defs.md#listmigrationtasksrequestrequesttypedef) 

### list\_progress\_update\_streams

Lists progress update streams associated with the user account making this call.

Type annotations and code completion for `#!python session.create_client("mgh").list_progress_update_streams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/list_progress_update_streams.html)

```python
# list_progress_update_streams method definition

await def list_progress_update_streams(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListProgressUpdateStreamsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProgressUpdateStreamsResultTypeDef](./type_defs.md#listprogressupdatestreamsresulttypedef) 


```python
# list_progress_update_streams method usage example with argument unpacking

kwargs: ListProgressUpdateStreamsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_progress_update_streams(**kwargs)
```

1. See [:material-code-braces: ListProgressUpdateStreamsRequestRequestTypeDef](./type_defs.md#listprogressupdatestreamsrequestrequesttypedef) 

### list\_source\_resources

Lists all the source resource that are associated with the specified
<code>MigrationTaskName</code> and <code>ProgressUpdateStream</code>.

Type annotations and code completion for `#!python session.create_client("mgh").list_source_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/list_source_resources.html)

```python
# list_source_resources method definition

await def list_source_resources(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListSourceResourcesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSourceResourcesResultTypeDef](./type_defs.md#listsourceresourcesresulttypedef) 


```python
# list_source_resources method usage example with argument unpacking

kwargs: ListSourceResourcesRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
}

parent.list_source_resources(**kwargs)
```

1. See [:material-code-braces: ListSourceResourcesRequestRequestTypeDef](./type_defs.md#listsourceresourcesrequestrequesttypedef) 

### notify\_application\_state

Sets the migration state of an application.

Type annotations and code completion for `#!python session.create_client("mgh").notify_application_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/notify_application_state.html)

```python
# notify_application_state method definition

await def notify_application_state(
    self,
    *,
    ApplicationId: str,
    Status: ApplicationStatusType,  # (1)
    UpdateDateTime: TimestampTypeDef = ...,
    DryRun: bool = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 


```python
# notify_application_state method usage example with argument unpacking

kwargs: NotifyApplicationStateRequestRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "Status": ...,
}

parent.notify_application_state(**kwargs)
```

1. See [:material-code-braces: NotifyApplicationStateRequestRequestTypeDef](./type_defs.md#notifyapplicationstaterequestrequesttypedef) 

### notify\_migration\_task\_state

Notifies Migration Hub of the current status, progress, or other detail
regarding a migration task.

Type annotations and code completion for `#!python session.create_client("mgh").notify_migration_task_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/notify_migration_task_state.html)

```python
# notify_migration_task_state method definition

await def notify_migration_task_state(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    Task: TaskTypeDef,  # (1)
    UpdateDateTime: TimestampTypeDef,
    NextUpdateSeconds: int,
    DryRun: bool = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TaskTypeDef](./type_defs.md#tasktypedef) 


```python
# notify_migration_task_state method usage example with argument unpacking

kwargs: NotifyMigrationTaskStateRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
    "Task": ...,
    "UpdateDateTime": ...,
    "NextUpdateSeconds": ...,
}

parent.notify_migration_task_state(**kwargs)
```

1. See [:material-code-braces: NotifyMigrationTaskStateRequestRequestTypeDef](./type_defs.md#notifymigrationtaskstaterequestrequesttypedef) 

### put\_resource\_attributes

Provides identifying details of the resource being migrated so that it can be
associated in the Application Discovery Service repository.

Type annotations and code completion for `#!python session.create_client("mgh").put_resource_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/client/put_resource_attributes.html)

```python
# put_resource_attributes method definition

await def put_resource_attributes(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    ResourceAttributeList: Sequence[ResourceAttributeTypeDef],  # (1)
    DryRun: bool = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ResourceAttributeTypeDef](./type_defs.md#resourceattributetypedef) 


```python
# put_resource_attributes method usage example with argument unpacking

kwargs: PutResourceAttributesRequestRequestTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
    "ResourceAttributeList": ...,
}

parent.put_resource_attributes(**kwargs)
```

1. See [:material-code-braces: PutResourceAttributesRequestRequestTypeDef](./type_defs.md#putresourceattributesrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("mgh").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("mgh").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator` method with overloads.

- `client.get_paginator("list_application_states")` -> [ListApplicationStatesPaginator](./paginators.md#listapplicationstatespaginator)
- `client.get_paginator("list_created_artifacts")` -> [ListCreatedArtifactsPaginator](./paginators.md#listcreatedartifactspaginator)
- `client.get_paginator("list_discovered_resources")` -> [ListDiscoveredResourcesPaginator](./paginators.md#listdiscoveredresourcespaginator)
- `client.get_paginator("list_migration_task_updates")` -> [ListMigrationTaskUpdatesPaginator](./paginators.md#listmigrationtaskupdatespaginator)
- `client.get_paginator("list_migration_tasks")` -> [ListMigrationTasksPaginator](./paginators.md#listmigrationtaskspaginator)
- `client.get_paginator("list_progress_update_streams")` -> [ListProgressUpdateStreamsPaginator](./paginators.md#listprogressupdatestreamspaginator)
- `client.get_paginator("list_source_resources")` -> [ListSourceResourcesPaginator](./paginators.md#listsourceresourcespaginator)



