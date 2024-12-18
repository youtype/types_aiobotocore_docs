# CodeConnectionsClient

> [Index](../README.md) > [CodeConnections](./README.md) > CodeConnectionsClient

!!! note ""

    Auto-generated documentation for [CodeConnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections.html#codeconnections)
    type annotations stubs module [types-aiobotocore-codeconnections](https://pypi.org/project/types-aiobotocore-codeconnections/).

## CodeConnectionsClient

Type annotations and code completion for `#!python session.create_client("codeconnections")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections.html#CodeConnections.Client)

```python
# CodeConnectionsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_codeconnections.client import CodeConnectionsClient

session = get_session()
async with session.create_client("codeconnections") as client:
    client: CodeConnectionsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("codeconnections").exceptions` structure.

```python
# CodeConnectionsClient.exceptions usage example

async with session.create_client("codeconnections") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConcurrentModificationException,
        client.ConditionalCheckFailedException,
        client.ConflictException,
        client.InternalServerException,
        client.InvalidInputException,
        client.LimitExceededException,
        client.ResourceAlreadyExistsException,
        client.ResourceNotFoundException,
        client.ResourceUnavailableException,
        client.RetryLatestCommitFailedException,
        client.SyncBlockerDoesNotExistException,
        client.SyncConfigurationStillExistsException,
        client.ThrottlingException,
        client.UnsupportedOperationException,
        client.UnsupportedProviderTypeException,
        client.UpdateOutOfSyncException,
    ) as e:
        print(e)
```

```python
# CodeConnectionsClient usage type checking example

from types_aiobotocore_codeconnections.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("codeconnections").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("codeconnections").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/generate_presigned_url.html)

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



Type annotations and code completion for `#!python session.create_client("codeconnections").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_connection

Creates a connection that can then be given to other Amazon Web Services
services like CodePipeline so that it can access third-party code repositories.

Type annotations and code completion for `#!python session.create_client("codeconnections").create_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/create_connection.html)

```python
# create_connection method definition

await def create_connection(
    self,
    *,
    ConnectionName: str,
    ProviderType: ProviderTypeType = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    HostArn: str = ...,
) -> CreateConnectionOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateConnectionOutputTypeDef](./type_defs.md#createconnectionoutputtypedef) 


```python
# create_connection method usage example with argument unpacking

kwargs: CreateConnectionInputRequestTypeDef = {  # (1)
    "ConnectionName": ...,
}

parent.create_connection(**kwargs)
```

1. See [:material-code-braces: CreateConnectionInputRequestTypeDef](./type_defs.md#createconnectioninputrequesttypedef) 

### create\_host

Creates a resource that represents the infrastructure where a third-party
provider is installed.

Type annotations and code completion for `#!python session.create_client("codeconnections").create_host` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/create_host.html)

```python
# create_host method definition

await def create_host(
    self,
    *,
    Name: str,
    ProviderType: ProviderTypeType,  # (1)
    ProviderEndpoint: str,
    VpcConfiguration: VpcConfigurationTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateHostOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateHostOutputTypeDef](./type_defs.md#createhostoutputtypedef) 


```python
# create_host method usage example with argument unpacking

kwargs: CreateHostInputRequestTypeDef = {  # (1)
    "Name": ...,
    "ProviderType": ...,
    "ProviderEndpoint": ...,
}

parent.create_host(**kwargs)
```

1. See [:material-code-braces: CreateHostInputRequestTypeDef](./type_defs.md#createhostinputrequesttypedef) 

### create\_repository\_link

Creates a link to a specified external Git repository.

Type annotations and code completion for `#!python session.create_client("codeconnections").create_repository_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/create_repository_link.html)

```python
# create_repository_link method definition

await def create_repository_link(
    self,
    *,
    ConnectionArn: str,
    OwnerId: str,
    RepositoryName: str,
    EncryptionKeyArn: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateRepositoryLinkOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateRepositoryLinkOutputTypeDef](./type_defs.md#createrepositorylinkoutputtypedef) 


```python
# create_repository_link method usage example with argument unpacking

kwargs: CreateRepositoryLinkInputRequestTypeDef = {  # (1)
    "ConnectionArn": ...,
    "OwnerId": ...,
    "RepositoryName": ...,
}

parent.create_repository_link(**kwargs)
```

1. See [:material-code-braces: CreateRepositoryLinkInputRequestTypeDef](./type_defs.md#createrepositorylinkinputrequesttypedef) 

### create\_sync\_configuration

Creates a sync configuration which allows Amazon Web Services to sync content
from a Git repository to update a specified Amazon Web Services resource.

Type annotations and code completion for `#!python session.create_client("codeconnections").create_sync_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/create_sync_configuration.html)

```python
# create_sync_configuration method definition

await def create_sync_configuration(
    self,
    *,
    Branch: str,
    ConfigFile: str,
    RepositoryLinkId: str,
    ResourceName: str,
    RoleArn: str,
    SyncType: SyncConfigurationTypeType,  # (1)
    PublishDeploymentStatus: PublishDeploymentStatusType = ...,  # (2)
    TriggerResourceUpdateOn: TriggerResourceUpdateOnType = ...,  # (3)
    PullRequestComment: PullRequestCommentType = ...,  # (4)
) -> CreateSyncConfigurationOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: SyncConfigurationTypeType](./literals.md#syncconfigurationtypetype) 
2. See [:material-code-brackets: PublishDeploymentStatusType](./literals.md#publishdeploymentstatustype) 
3. See [:material-code-brackets: TriggerResourceUpdateOnType](./literals.md#triggerresourceupdateontype) 
4. See [:material-code-brackets: PullRequestCommentType](./literals.md#pullrequestcommenttype) 
5. See [:material-code-braces: CreateSyncConfigurationOutputTypeDef](./type_defs.md#createsyncconfigurationoutputtypedef) 


```python
# create_sync_configuration method usage example with argument unpacking

kwargs: CreateSyncConfigurationInputRequestTypeDef = {  # (1)
    "Branch": ...,
    "ConfigFile": ...,
    "RepositoryLinkId": ...,
    "ResourceName": ...,
    "RoleArn": ...,
    "SyncType": ...,
}

parent.create_sync_configuration(**kwargs)
```

1. See [:material-code-braces: CreateSyncConfigurationInputRequestTypeDef](./type_defs.md#createsyncconfigurationinputrequesttypedef) 

### delete\_connection

The connection to be deleted.

Type annotations and code completion for `#!python session.create_client("codeconnections").delete_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/delete_connection.html)

```python
# delete_connection method definition

await def delete_connection(
    self,
    *,
    ConnectionArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_connection method usage example with argument unpacking

kwargs: DeleteConnectionInputRequestTypeDef = {  # (1)
    "ConnectionArn": ...,
}

parent.delete_connection(**kwargs)
```

1. See [:material-code-braces: DeleteConnectionInputRequestTypeDef](./type_defs.md#deleteconnectioninputrequesttypedef) 

### delete\_host

The host to be deleted.

Type annotations and code completion for `#!python session.create_client("codeconnections").delete_host` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/delete_host.html)

```python
# delete_host method definition

await def delete_host(
    self,
    *,
    HostArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_host method usage example with argument unpacking

kwargs: DeleteHostInputRequestTypeDef = {  # (1)
    "HostArn": ...,
}

parent.delete_host(**kwargs)
```

1. See [:material-code-braces: DeleteHostInputRequestTypeDef](./type_defs.md#deletehostinputrequesttypedef) 

### delete\_repository\_link

Deletes the association between your connection and a specified external Git
repository.

Type annotations and code completion for `#!python session.create_client("codeconnections").delete_repository_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/delete_repository_link.html)

```python
# delete_repository_link method definition

await def delete_repository_link(
    self,
    *,
    RepositoryLinkId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_repository_link method usage example with argument unpacking

kwargs: DeleteRepositoryLinkInputRequestTypeDef = {  # (1)
    "RepositoryLinkId": ...,
}

parent.delete_repository_link(**kwargs)
```

1. See [:material-code-braces: DeleteRepositoryLinkInputRequestTypeDef](./type_defs.md#deleterepositorylinkinputrequesttypedef) 

### delete\_sync\_configuration

Deletes the sync configuration for a specified repository and connection.

Type annotations and code completion for `#!python session.create_client("codeconnections").delete_sync_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/delete_sync_configuration.html)

```python
# delete_sync_configuration method definition

await def delete_sync_configuration(
    self,
    *,
    SyncType: SyncConfigurationTypeType,  # (1)
    ResourceName: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: SyncConfigurationTypeType](./literals.md#syncconfigurationtypetype) 


```python
# delete_sync_configuration method usage example with argument unpacking

kwargs: DeleteSyncConfigurationInputRequestTypeDef = {  # (1)
    "SyncType": ...,
    "ResourceName": ...,
}

parent.delete_sync_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteSyncConfigurationInputRequestTypeDef](./type_defs.md#deletesyncconfigurationinputrequesttypedef) 

### get\_connection

Returns the connection ARN and details such as status, owner, and provider type.

Type annotations and code completion for `#!python session.create_client("codeconnections").get_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/get_connection.html)

```python
# get_connection method definition

await def get_connection(
    self,
    *,
    ConnectionArn: str,
) -> GetConnectionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConnectionOutputTypeDef](./type_defs.md#getconnectionoutputtypedef) 


```python
# get_connection method usage example with argument unpacking

kwargs: GetConnectionInputRequestTypeDef = {  # (1)
    "ConnectionArn": ...,
}

parent.get_connection(**kwargs)
```

1. See [:material-code-braces: GetConnectionInputRequestTypeDef](./type_defs.md#getconnectioninputrequesttypedef) 

### get\_host

Returns the host ARN and details such as status, provider type, endpoint, and,
if applicable, the VPC configuration.

Type annotations and code completion for `#!python session.create_client("codeconnections").get_host` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/get_host.html)

```python
# get_host method definition

await def get_host(
    self,
    *,
    HostArn: str,
) -> GetHostOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetHostOutputTypeDef](./type_defs.md#gethostoutputtypedef) 


```python
# get_host method usage example with argument unpacking

kwargs: GetHostInputRequestTypeDef = {  # (1)
    "HostArn": ...,
}

parent.get_host(**kwargs)
```

1. See [:material-code-braces: GetHostInputRequestTypeDef](./type_defs.md#gethostinputrequesttypedef) 

### get\_repository\_link

Returns details about a repository link.

Type annotations and code completion for `#!python session.create_client("codeconnections").get_repository_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/get_repository_link.html)

```python
# get_repository_link method definition

await def get_repository_link(
    self,
    *,
    RepositoryLinkId: str,
) -> GetRepositoryLinkOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRepositoryLinkOutputTypeDef](./type_defs.md#getrepositorylinkoutputtypedef) 


```python
# get_repository_link method usage example with argument unpacking

kwargs: GetRepositoryLinkInputRequestTypeDef = {  # (1)
    "RepositoryLinkId": ...,
}

parent.get_repository_link(**kwargs)
```

1. See [:material-code-braces: GetRepositoryLinkInputRequestTypeDef](./type_defs.md#getrepositorylinkinputrequesttypedef) 

### get\_repository\_sync\_status

Returns details about the sync status for a repository.

Type annotations and code completion for `#!python session.create_client("codeconnections").get_repository_sync_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/get_repository_sync_status.html)

```python
# get_repository_sync_status method definition

await def get_repository_sync_status(
    self,
    *,
    Branch: str,
    RepositoryLinkId: str,
    SyncType: SyncConfigurationTypeType,  # (1)
) -> GetRepositorySyncStatusOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SyncConfigurationTypeType](./literals.md#syncconfigurationtypetype) 
2. See [:material-code-braces: GetRepositorySyncStatusOutputTypeDef](./type_defs.md#getrepositorysyncstatusoutputtypedef) 


```python
# get_repository_sync_status method usage example with argument unpacking

kwargs: GetRepositorySyncStatusInputRequestTypeDef = {  # (1)
    "Branch": ...,
    "RepositoryLinkId": ...,
    "SyncType": ...,
}

parent.get_repository_sync_status(**kwargs)
```

1. See [:material-code-braces: GetRepositorySyncStatusInputRequestTypeDef](./type_defs.md#getrepositorysyncstatusinputrequesttypedef) 

### get\_resource\_sync\_status

Returns the status of the sync with the Git repository for a specific Amazon
Web Services resource.

Type annotations and code completion for `#!python session.create_client("codeconnections").get_resource_sync_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/get_resource_sync_status.html)

```python
# get_resource_sync_status method definition

await def get_resource_sync_status(
    self,
    *,
    ResourceName: str,
    SyncType: SyncConfigurationTypeType,  # (1)
) -> GetResourceSyncStatusOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SyncConfigurationTypeType](./literals.md#syncconfigurationtypetype) 
2. See [:material-code-braces: GetResourceSyncStatusOutputTypeDef](./type_defs.md#getresourcesyncstatusoutputtypedef) 


```python
# get_resource_sync_status method usage example with argument unpacking

kwargs: GetResourceSyncStatusInputRequestTypeDef = {  # (1)
    "ResourceName": ...,
    "SyncType": ...,
}

parent.get_resource_sync_status(**kwargs)
```

1. See [:material-code-braces: GetResourceSyncStatusInputRequestTypeDef](./type_defs.md#getresourcesyncstatusinputrequesttypedef) 

### get\_sync\_blocker\_summary

Returns a list of the most recent sync blockers.

Type annotations and code completion for `#!python session.create_client("codeconnections").get_sync_blocker_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/get_sync_blocker_summary.html)

```python
# get_sync_blocker_summary method definition

await def get_sync_blocker_summary(
    self,
    *,
    SyncType: SyncConfigurationTypeType,  # (1)
    ResourceName: str,
) -> GetSyncBlockerSummaryOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SyncConfigurationTypeType](./literals.md#syncconfigurationtypetype) 
2. See [:material-code-braces: GetSyncBlockerSummaryOutputTypeDef](./type_defs.md#getsyncblockersummaryoutputtypedef) 


```python
# get_sync_blocker_summary method usage example with argument unpacking

kwargs: GetSyncBlockerSummaryInputRequestTypeDef = {  # (1)
    "SyncType": ...,
    "ResourceName": ...,
}

parent.get_sync_blocker_summary(**kwargs)
```

1. See [:material-code-braces: GetSyncBlockerSummaryInputRequestTypeDef](./type_defs.md#getsyncblockersummaryinputrequesttypedef) 

### get\_sync\_configuration

Returns details about a sync configuration, including the sync type and
resource name.

Type annotations and code completion for `#!python session.create_client("codeconnections").get_sync_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/get_sync_configuration.html)

```python
# get_sync_configuration method definition

await def get_sync_configuration(
    self,
    *,
    SyncType: SyncConfigurationTypeType,  # (1)
    ResourceName: str,
) -> GetSyncConfigurationOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SyncConfigurationTypeType](./literals.md#syncconfigurationtypetype) 
2. See [:material-code-braces: GetSyncConfigurationOutputTypeDef](./type_defs.md#getsyncconfigurationoutputtypedef) 


```python
# get_sync_configuration method usage example with argument unpacking

kwargs: GetSyncConfigurationInputRequestTypeDef = {  # (1)
    "SyncType": ...,
    "ResourceName": ...,
}

parent.get_sync_configuration(**kwargs)
```

1. See [:material-code-braces: GetSyncConfigurationInputRequestTypeDef](./type_defs.md#getsyncconfigurationinputrequesttypedef) 

### list\_connections

Lists the connections associated with your account.

Type annotations and code completion for `#!python session.create_client("codeconnections").list_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/list_connections.html)

```python
# list_connections method definition

await def list_connections(
    self,
    *,
    ProviderTypeFilter: ProviderTypeType = ...,  # (1)
    HostArnFilter: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListConnectionsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-braces: ListConnectionsOutputTypeDef](./type_defs.md#listconnectionsoutputtypedef) 


```python
# list_connections method usage example with argument unpacking

kwargs: ListConnectionsInputRequestTypeDef = {  # (1)
    "ProviderTypeFilter": ...,
}

parent.list_connections(**kwargs)
```

1. See [:material-code-braces: ListConnectionsInputRequestTypeDef](./type_defs.md#listconnectionsinputrequesttypedef) 

### list\_hosts

Lists the hosts associated with your account.

Type annotations and code completion for `#!python session.create_client("codeconnections").list_hosts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/list_hosts.html)

```python
# list_hosts method definition

await def list_hosts(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListHostsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListHostsOutputTypeDef](./type_defs.md#listhostsoutputtypedef) 


```python
# list_hosts method usage example with argument unpacking

kwargs: ListHostsInputRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_hosts(**kwargs)
```

1. See [:material-code-braces: ListHostsInputRequestTypeDef](./type_defs.md#listhostsinputrequesttypedef) 

### list\_repository\_links

Lists the repository links created for connections in your account.

Type annotations and code completion for `#!python session.create_client("codeconnections").list_repository_links` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/list_repository_links.html)

```python
# list_repository_links method definition

await def list_repository_links(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListRepositoryLinksOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRepositoryLinksOutputTypeDef](./type_defs.md#listrepositorylinksoutputtypedef) 


```python
# list_repository_links method usage example with argument unpacking

kwargs: ListRepositoryLinksInputRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_repository_links(**kwargs)
```

1. See [:material-code-braces: ListRepositoryLinksInputRequestTypeDef](./type_defs.md#listrepositorylinksinputrequesttypedef) 

### list\_repository\_sync\_definitions

Lists the repository sync definitions for repository links in your account.

Type annotations and code completion for `#!python session.create_client("codeconnections").list_repository_sync_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/list_repository_sync_definitions.html)

```python
# list_repository_sync_definitions method definition

await def list_repository_sync_definitions(
    self,
    *,
    RepositoryLinkId: str,
    SyncType: SyncConfigurationTypeType,  # (1)
) -> ListRepositorySyncDefinitionsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SyncConfigurationTypeType](./literals.md#syncconfigurationtypetype) 
2. See [:material-code-braces: ListRepositorySyncDefinitionsOutputTypeDef](./type_defs.md#listrepositorysyncdefinitionsoutputtypedef) 


```python
# list_repository_sync_definitions method usage example with argument unpacking

kwargs: ListRepositorySyncDefinitionsInputRequestTypeDef = {  # (1)
    "RepositoryLinkId": ...,
    "SyncType": ...,
}

parent.list_repository_sync_definitions(**kwargs)
```

1. See [:material-code-braces: ListRepositorySyncDefinitionsInputRequestTypeDef](./type_defs.md#listrepositorysyncdefinitionsinputrequesttypedef) 

### list\_sync\_configurations

Returns a list of sync configurations for a specified repository.

Type annotations and code completion for `#!python session.create_client("codeconnections").list_sync_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/list_sync_configurations.html)

```python
# list_sync_configurations method definition

await def list_sync_configurations(
    self,
    *,
    RepositoryLinkId: str,
    SyncType: SyncConfigurationTypeType,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListSyncConfigurationsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SyncConfigurationTypeType](./literals.md#syncconfigurationtypetype) 
2. See [:material-code-braces: ListSyncConfigurationsOutputTypeDef](./type_defs.md#listsyncconfigurationsoutputtypedef) 


```python
# list_sync_configurations method usage example with argument unpacking

kwargs: ListSyncConfigurationsInputRequestTypeDef = {  # (1)
    "RepositoryLinkId": ...,
    "SyncType": ...,
}

parent.list_sync_configurations(**kwargs)
```

1. See [:material-code-braces: ListSyncConfigurationsInputRequestTypeDef](./type_defs.md#listsyncconfigurationsinputrequesttypedef) 

### list\_tags\_for\_resource

Gets the set of key-value pairs (metadata) that are used to manage the resource.

Type annotations and code completion for `#!python session.create_client("codeconnections").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### tag\_resource

Adds to or modifies the tags of the given resource.

Type annotations and code completion for `#!python session.create_client("codeconnections").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Removes tags from an Amazon Web Services resource.

Type annotations and code completion for `#!python session.create_client("codeconnections").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_host

Updates a specified host with the provided configurations.

Type annotations and code completion for `#!python session.create_client("codeconnections").update_host` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/update_host.html)

```python
# update_host method definition

await def update_host(
    self,
    *,
    HostArn: str,
    ProviderEndpoint: str = ...,
    VpcConfiguration: VpcConfigurationTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 


```python
# update_host method usage example with argument unpacking

kwargs: UpdateHostInputRequestTypeDef = {  # (1)
    "HostArn": ...,
}

parent.update_host(**kwargs)
```

1. See [:material-code-braces: UpdateHostInputRequestTypeDef](./type_defs.md#updatehostinputrequesttypedef) 

### update\_repository\_link

Updates the association between your connection and a specified external Git
repository.

Type annotations and code completion for `#!python session.create_client("codeconnections").update_repository_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/update_repository_link.html)

```python
# update_repository_link method definition

await def update_repository_link(
    self,
    *,
    RepositoryLinkId: str,
    ConnectionArn: str = ...,
    EncryptionKeyArn: str = ...,
) -> UpdateRepositoryLinkOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateRepositoryLinkOutputTypeDef](./type_defs.md#updaterepositorylinkoutputtypedef) 


```python
# update_repository_link method usage example with argument unpacking

kwargs: UpdateRepositoryLinkInputRequestTypeDef = {  # (1)
    "RepositoryLinkId": ...,
}

parent.update_repository_link(**kwargs)
```

1. See [:material-code-braces: UpdateRepositoryLinkInputRequestTypeDef](./type_defs.md#updaterepositorylinkinputrequesttypedef) 

### update\_sync\_blocker

Allows you to update the status of a sync blocker, resolving the blocker and
allowing syncing to continue.

Type annotations and code completion for `#!python session.create_client("codeconnections").update_sync_blocker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/update_sync_blocker.html)

```python
# update_sync_blocker method definition

await def update_sync_blocker(
    self,
    *,
    Id: str,
    SyncType: SyncConfigurationTypeType,  # (1)
    ResourceName: str,
    ResolvedReason: str,
) -> UpdateSyncBlockerOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SyncConfigurationTypeType](./literals.md#syncconfigurationtypetype) 
2. See [:material-code-braces: UpdateSyncBlockerOutputTypeDef](./type_defs.md#updatesyncblockeroutputtypedef) 


```python
# update_sync_blocker method usage example with argument unpacking

kwargs: UpdateSyncBlockerInputRequestTypeDef = {  # (1)
    "Id": ...,
    "SyncType": ...,
    "ResourceName": ...,
    "ResolvedReason": ...,
}

parent.update_sync_blocker(**kwargs)
```

1. See [:material-code-braces: UpdateSyncBlockerInputRequestTypeDef](./type_defs.md#updatesyncblockerinputrequesttypedef) 

### update\_sync\_configuration

Updates the sync configuration for your connection and a specified external Git
repository.

Type annotations and code completion for `#!python session.create_client("codeconnections").update_sync_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections/client/update_sync_configuration.html)

```python
# update_sync_configuration method definition

await def update_sync_configuration(
    self,
    *,
    ResourceName: str,
    SyncType: SyncConfigurationTypeType,  # (1)
    Branch: str = ...,
    ConfigFile: str = ...,
    RepositoryLinkId: str = ...,
    RoleArn: str = ...,
    PublishDeploymentStatus: PublishDeploymentStatusType = ...,  # (2)
    TriggerResourceUpdateOn: TriggerResourceUpdateOnType = ...,  # (3)
    PullRequestComment: PullRequestCommentType = ...,  # (4)
) -> UpdateSyncConfigurationOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: SyncConfigurationTypeType](./literals.md#syncconfigurationtypetype) 
2. See [:material-code-brackets: PublishDeploymentStatusType](./literals.md#publishdeploymentstatustype) 
3. See [:material-code-brackets: TriggerResourceUpdateOnType](./literals.md#triggerresourceupdateontype) 
4. See [:material-code-brackets: PullRequestCommentType](./literals.md#pullrequestcommenttype) 
5. See [:material-code-braces: UpdateSyncConfigurationOutputTypeDef](./type_defs.md#updatesyncconfigurationoutputtypedef) 


```python
# update_sync_configuration method usage example with argument unpacking

kwargs: UpdateSyncConfigurationInputRequestTypeDef = {  # (1)
    "ResourceName": ...,
    "SyncType": ...,
}

parent.update_sync_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateSyncConfigurationInputRequestTypeDef](./type_defs.md#updatesyncconfigurationinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("codeconnections").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections.html#CodeConnections.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "CodeConnectionsClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("codeconnections").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections.html#CodeConnections.Client)

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





