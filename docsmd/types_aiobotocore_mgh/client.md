# MigrationHubClient

> [Index](../README.md) > [MigrationHub](./README.md) > MigrationHubClient

!!! note ""

    Auto-generated documentation for [MigrationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
    type annotations stubs module [types-aiobotocore-mgh](https://pypi.org/project/types-aiobotocore-mgh/).

## MigrationHubClient

Type annotations and code completion for `#!python session.create_client("mgh")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client)

```python
MigrationHubClient usage example

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
MigrationHubClient.exceptions usage example

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
MigrationHubClient usage type checking example

from types_aiobotocore_mgh.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_created\_artifact

Associates a created artifact of an AWS cloud resource, the target receiving the
migration, with the migration task performed by a migration tool.

Type annotations and code completion for `#!python session.create_client("mgh").associate_created_artifact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.associate_created_artifact)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.associate_discovered_resource)

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

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("mgh").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("mgh").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_progress\_update\_stream

Creates a progress update stream which is an AWS resource used for access
control as well as a namespace for migration task names that is implicitly
linked to your AWS account.

Type annotations and code completion for `#!python session.create_client("mgh").create_progress_update_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.create_progress_update_stream)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.delete_progress_update_stream)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.describe_application_state)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.describe_migration_task)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.disassociate_created_artifact)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.disassociate_discovered_resource)

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

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("mgh").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.generate_presigned_url)

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


### import\_migration\_task

Registers a new migration task which represents a server, database, etc., being
migrated to AWS by a migration tool.

Type annotations and code completion for `#!python session.create_client("mgh").import_migration_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.import_migration_task)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.list_application_states)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.list_created_artifacts)

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

Lists discovered resources associated with the given `MigrationTask`.

Type annotations and code completion for `#!python session.create_client("mgh").list_discovered_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.list_discovered_resources)

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

### list\_migration\_tasks

Lists all, or filtered by resource name, migration tasks associated with the
user account making this call.

Type annotations and code completion for `#!python session.create_client("mgh").list_migration_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.list_migration_tasks)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.list_progress_update_streams)

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

### notify\_application\_state

Sets the migration state of an application.

Type annotations and code completion for `#!python session.create_client("mgh").notify_application_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.notify_application_state)

```python
# notify_application_state method definition

await def notify_application_state(
    self,
    *,
    ApplicationId: str,
    Status: ApplicationStatusType,  # (1)
    UpdateDateTime: Union[datetime, str] = ...,
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.notify_migration_task_state)

```python
# notify_migration_task_state method definition

await def notify_migration_task_state(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    Task: TaskTypeDef,  # (1)
    UpdateDateTime: Union[datetime, str],
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.put_resource_attributes)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> MigrationHubClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("mgh").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator` method with overloads.

- `client.get_paginator("list_application_states")` -> [ListApplicationStatesPaginator](./paginators.md#listapplicationstatespaginator)
- `client.get_paginator("list_created_artifacts")` -> [ListCreatedArtifactsPaginator](./paginators.md#listcreatedartifactspaginator)
- `client.get_paginator("list_discovered_resources")` -> [ListDiscoveredResourcesPaginator](./paginators.md#listdiscoveredresourcespaginator)
- `client.get_paginator("list_migration_tasks")` -> [ListMigrationTasksPaginator](./paginators.md#listmigrationtaskspaginator)
- `client.get_paginator("list_progress_update_streams")` -> [ListProgressUpdateStreamsPaginator](./paginators.md#listprogressupdatestreamspaginator)



