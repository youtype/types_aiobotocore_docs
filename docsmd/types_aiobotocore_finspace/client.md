# finspaceClient

> [Index](../README.md) > [finspace](./README.md) > finspaceClient

!!! note ""

    Auto-generated documentation for [finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
    type annotations stubs module [types-aiobotocore-finspace](https://pypi.org/project/types-aiobotocore-finspace/).

## finspaceClient

Type annotations and code completion for `#!python session.create_client("finspace")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client)

```python
finspaceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_finspace.client import finspaceClient

session = get_session()
async with session.create_client("finspace") as client:
    client: finspaceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("finspace").exceptions` structure.

```python
finspaceClient.exceptions usage example

async with session.create_client("finspace") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.InvalidRequestException,
        client.LimitExceededException,
        client.ResourceAlreadyExistsException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
finspaceClient usage type checking example

from types_aiobotocore_finspace.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("finspace").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("finspace").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_environment

Create a new FinSpace environment.

Type annotations and code completion for `#!python session.create_client("finspace").create_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_environment)

```python
# create_environment method definition

await def create_environment(
    self,
    *,
    name: str,
    description: str = ...,
    kmsKeyId: str = ...,
    tags: Mapping[str, str] = ...,
    federationMode: FederationModeType = ...,  # (1)
    federationParameters: FederationParametersTypeDef = ...,  # (2)
    superuserParameters: SuperuserParametersTypeDef = ...,  # (3)
    dataBundles: Sequence[str] = ...,
) -> CreateEnvironmentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: FederationModeType](./literals.md#federationmodetype) 
2. See [:material-code-braces: FederationParametersTypeDef](./type_defs.md#federationparameterstypedef) 
3. See [:material-code-braces: SuperuserParametersTypeDef](./type_defs.md#superuserparameterstypedef) 
4. See [:material-code-braces: CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef) 


```python
# create_environment method usage example with argument unpacking

kwargs: CreateEnvironmentRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_environment(**kwargs)
```

1. See [:material-code-braces: CreateEnvironmentRequestRequestTypeDef](./type_defs.md#createenvironmentrequestrequesttypedef) 

### create\_kx\_changeset

Creates a changeset for a kdb database.

Type annotations and code completion for `#!python session.create_client("finspace").create_kx_changeset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_changeset)

```python
# create_kx_changeset method definition

await def create_kx_changeset(
    self,
    *,
    environmentId: str,
    databaseName: str,
    changeRequests: Sequence[ChangeRequestTypeDef],  # (1)
    clientToken: str,
) -> CreateKxChangesetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ChangeRequestTypeDef](./type_defs.md#changerequesttypedef) 
2. See [:material-code-braces: CreateKxChangesetResponseTypeDef](./type_defs.md#createkxchangesetresponsetypedef) 


```python
# create_kx_changeset method usage example with argument unpacking

kwargs: CreateKxChangesetRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "databaseName": ...,
    "changeRequests": ...,
    "clientToken": ...,
}

parent.create_kx_changeset(**kwargs)
```

1. See [:material-code-braces: CreateKxChangesetRequestRequestTypeDef](./type_defs.md#createkxchangesetrequestrequesttypedef) 

### create\_kx\_cluster

Creates a new kdb cluster.

Type annotations and code completion for `#!python session.create_client("finspace").create_kx_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_cluster)

```python
# create_kx_cluster method definition

await def create_kx_cluster(
    self,
    *,
    environmentId: str,
    clusterName: str,
    clusterType: KxClusterTypeType,  # (1)
    capacityConfiguration: CapacityConfigurationTypeDef,  # (2)
    releaseLabel: str,
    azMode: KxAzModeType,  # (3)
    clientToken: str = ...,
    databases: Sequence[KxDatabaseConfigurationTypeDef] = ...,  # (4)
    cacheStorageConfigurations: Sequence[KxCacheStorageConfigurationTypeDef] = ...,  # (5)
    autoScalingConfiguration: AutoScalingConfigurationTypeDef = ...,  # (6)
    clusterDescription: str = ...,
    vpcConfiguration: VpcConfigurationTypeDef = ...,  # (7)
    initializationScript: str = ...,
    commandLineArguments: Sequence[KxCommandLineArgumentTypeDef] = ...,  # (8)
    code: CodeConfigurationTypeDef = ...,  # (9)
    executionRole: str = ...,
    savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef = ...,  # (10)
    availabilityZoneId: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateKxClusterResponseTypeDef:  # (11)
    ...
```

1. See [:material-code-brackets: KxClusterTypeType](./literals.md#kxclustertypetype) 
2. See [:material-code-braces: CapacityConfigurationTypeDef](./type_defs.md#capacityconfigurationtypedef) 
3. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
4. See [:material-code-braces: KxDatabaseConfigurationTypeDef](./type_defs.md#kxdatabaseconfigurationtypedef) 
5. See [:material-code-braces: KxCacheStorageConfigurationTypeDef](./type_defs.md#kxcachestorageconfigurationtypedef) 
6. See [:material-code-braces: AutoScalingConfigurationTypeDef](./type_defs.md#autoscalingconfigurationtypedef) 
7. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
8. See [:material-code-braces: KxCommandLineArgumentTypeDef](./type_defs.md#kxcommandlineargumenttypedef) 
9. See [:material-code-braces: CodeConfigurationTypeDef](./type_defs.md#codeconfigurationtypedef) 
10. See [:material-code-braces: KxSavedownStorageConfigurationTypeDef](./type_defs.md#kxsavedownstorageconfigurationtypedef) 
11. See [:material-code-braces: CreateKxClusterResponseTypeDef](./type_defs.md#createkxclusterresponsetypedef) 


```python
# create_kx_cluster method usage example with argument unpacking

kwargs: CreateKxClusterRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "clusterName": ...,
    "clusterType": ...,
    "capacityConfiguration": ...,
    "releaseLabel": ...,
    "azMode": ...,
}

parent.create_kx_cluster(**kwargs)
```

1. See [:material-code-braces: CreateKxClusterRequestRequestTypeDef](./type_defs.md#createkxclusterrequestrequesttypedef) 

### create\_kx\_database

Creates a new kdb database in the environment.

Type annotations and code completion for `#!python session.create_client("finspace").create_kx_database` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_database)

```python
# create_kx_database method definition

await def create_kx_database(
    self,
    *,
    environmentId: str,
    databaseName: str,
    clientToken: str,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateKxDatabaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateKxDatabaseResponseTypeDef](./type_defs.md#createkxdatabaseresponsetypedef) 


```python
# create_kx_database method usage example with argument unpacking

kwargs: CreateKxDatabaseRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "databaseName": ...,
    "clientToken": ...,
}

parent.create_kx_database(**kwargs)
```

1. See [:material-code-braces: CreateKxDatabaseRequestRequestTypeDef](./type_defs.md#createkxdatabaserequestrequesttypedef) 

### create\_kx\_environment

Creates a managed kdb environment for the account.

Type annotations and code completion for `#!python session.create_client("finspace").create_kx_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_environment)

```python
# create_kx_environment method definition

await def create_kx_environment(
    self,
    *,
    name: str,
    kmsKeyId: str,
    description: str = ...,
    tags: Mapping[str, str] = ...,
    clientToken: str = ...,
) -> CreateKxEnvironmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateKxEnvironmentResponseTypeDef](./type_defs.md#createkxenvironmentresponsetypedef) 


```python
# create_kx_environment method usage example with argument unpacking

kwargs: CreateKxEnvironmentRequestRequestTypeDef = {  # (1)
    "name": ...,
    "kmsKeyId": ...,
}

parent.create_kx_environment(**kwargs)
```

1. See [:material-code-braces: CreateKxEnvironmentRequestRequestTypeDef](./type_defs.md#createkxenvironmentrequestrequesttypedef) 

### create\_kx\_user

Creates a user in FinSpace kdb environment with an associated IAM role.

Type annotations and code completion for `#!python session.create_client("finspace").create_kx_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_user)

```python
# create_kx_user method definition

await def create_kx_user(
    self,
    *,
    environmentId: str,
    userName: str,
    iamRole: str,
    tags: Mapping[str, str] = ...,
    clientToken: str = ...,
) -> CreateKxUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateKxUserResponseTypeDef](./type_defs.md#createkxuserresponsetypedef) 


```python
# create_kx_user method usage example with argument unpacking

kwargs: CreateKxUserRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "userName": ...,
    "iamRole": ...,
}

parent.create_kx_user(**kwargs)
```

1. See [:material-code-braces: CreateKxUserRequestRequestTypeDef](./type_defs.md#createkxuserrequestrequesttypedef) 

### delete\_environment

Delete an FinSpace environment.

Type annotations and code completion for `#!python session.create_client("finspace").delete_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_environment)

```python
# delete_environment method definition

await def delete_environment(
    self,
    *,
    environmentId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_environment method usage example with argument unpacking

kwargs: DeleteEnvironmentRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.delete_environment(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentRequestRequestTypeDef](./type_defs.md#deleteenvironmentrequestrequesttypedef) 

### delete\_kx\_cluster

Deletes a kdb cluster.

Type annotations and code completion for `#!python session.create_client("finspace").delete_kx_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_kx_cluster)

```python
# delete_kx_cluster method definition

await def delete_kx_cluster(
    self,
    *,
    environmentId: str,
    clusterName: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_kx_cluster method usage example with argument unpacking

kwargs: DeleteKxClusterRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "clusterName": ...,
}

parent.delete_kx_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteKxClusterRequestRequestTypeDef](./type_defs.md#deletekxclusterrequestrequesttypedef) 

### delete\_kx\_database

Deletes the specified database and all of its associated data.

Type annotations and code completion for `#!python session.create_client("finspace").delete_kx_database` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_kx_database)

```python
# delete_kx_database method definition

await def delete_kx_database(
    self,
    *,
    environmentId: str,
    databaseName: str,
    clientToken: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_kx_database method usage example with argument unpacking

kwargs: DeleteKxDatabaseRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "databaseName": ...,
    "clientToken": ...,
}

parent.delete_kx_database(**kwargs)
```

1. See [:material-code-braces: DeleteKxDatabaseRequestRequestTypeDef](./type_defs.md#deletekxdatabaserequestrequesttypedef) 

### delete\_kx\_environment

Deletes the kdb environment.

Type annotations and code completion for `#!python session.create_client("finspace").delete_kx_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_kx_environment)

```python
# delete_kx_environment method definition

await def delete_kx_environment(
    self,
    *,
    environmentId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_kx_environment method usage example with argument unpacking

kwargs: DeleteKxEnvironmentRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.delete_kx_environment(**kwargs)
```

1. See [:material-code-braces: DeleteKxEnvironmentRequestRequestTypeDef](./type_defs.md#deletekxenvironmentrequestrequesttypedef) 

### delete\_kx\_user

Deletes a user in the specified kdb environment.

Type annotations and code completion for `#!python session.create_client("finspace").delete_kx_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_kx_user)

```python
# delete_kx_user method definition

await def delete_kx_user(
    self,
    *,
    userName: str,
    environmentId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_kx_user method usage example with argument unpacking

kwargs: DeleteKxUserRequestRequestTypeDef = {  # (1)
    "userName": ...,
    "environmentId": ...,
}

parent.delete_kx_user(**kwargs)
```

1. See [:material-code-braces: DeleteKxUserRequestRequestTypeDef](./type_defs.md#deletekxuserrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("finspace").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.generate_presigned_url)

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


### get\_environment

Returns the FinSpace environment object.

Type annotations and code completion for `#!python session.create_client("finspace").get_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_environment)

```python
# get_environment method definition

await def get_environment(
    self,
    *,
    environmentId: str,
) -> GetEnvironmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnvironmentResponseTypeDef](./type_defs.md#getenvironmentresponsetypedef) 


```python
# get_environment method usage example with argument unpacking

kwargs: GetEnvironmentRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.get_environment(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentRequestRequestTypeDef](./type_defs.md#getenvironmentrequestrequesttypedef) 

### get\_kx\_changeset

Returns information about a kdb changeset.

Type annotations and code completion for `#!python session.create_client("finspace").get_kx_changeset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_changeset)

```python
# get_kx_changeset method definition

await def get_kx_changeset(
    self,
    *,
    environmentId: str,
    databaseName: str,
    changesetId: str,
) -> GetKxChangesetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKxChangesetResponseTypeDef](./type_defs.md#getkxchangesetresponsetypedef) 


```python
# get_kx_changeset method usage example with argument unpacking

kwargs: GetKxChangesetRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "databaseName": ...,
    "changesetId": ...,
}

parent.get_kx_changeset(**kwargs)
```

1. See [:material-code-braces: GetKxChangesetRequestRequestTypeDef](./type_defs.md#getkxchangesetrequestrequesttypedef) 

### get\_kx\_cluster

Retrieves information about a kdb cluster.

Type annotations and code completion for `#!python session.create_client("finspace").get_kx_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_cluster)

```python
# get_kx_cluster method definition

await def get_kx_cluster(
    self,
    *,
    environmentId: str,
    clusterName: str,
) -> GetKxClusterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKxClusterResponseTypeDef](./type_defs.md#getkxclusterresponsetypedef) 


```python
# get_kx_cluster method usage example with argument unpacking

kwargs: GetKxClusterRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "clusterName": ...,
}

parent.get_kx_cluster(**kwargs)
```

1. See [:material-code-braces: GetKxClusterRequestRequestTypeDef](./type_defs.md#getkxclusterrequestrequesttypedef) 

### get\_kx\_connection\_string

Retrieves a connection string for a user to connect to a kdb cluster.

Type annotations and code completion for `#!python session.create_client("finspace").get_kx_connection_string` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_connection_string)

```python
# get_kx_connection_string method definition

await def get_kx_connection_string(
    self,
    *,
    userArn: str,
    environmentId: str,
    clusterName: str,
) -> GetKxConnectionStringResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKxConnectionStringResponseTypeDef](./type_defs.md#getkxconnectionstringresponsetypedef) 


```python
# get_kx_connection_string method usage example with argument unpacking

kwargs: GetKxConnectionStringRequestRequestTypeDef = {  # (1)
    "userArn": ...,
    "environmentId": ...,
    "clusterName": ...,
}

parent.get_kx_connection_string(**kwargs)
```

1. See [:material-code-braces: GetKxConnectionStringRequestRequestTypeDef](./type_defs.md#getkxconnectionstringrequestrequesttypedef) 

### get\_kx\_database

Returns database information for the specified environment ID.

Type annotations and code completion for `#!python session.create_client("finspace").get_kx_database` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_database)

```python
# get_kx_database method definition

await def get_kx_database(
    self,
    *,
    environmentId: str,
    databaseName: str,
) -> GetKxDatabaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKxDatabaseResponseTypeDef](./type_defs.md#getkxdatabaseresponsetypedef) 


```python
# get_kx_database method usage example with argument unpacking

kwargs: GetKxDatabaseRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "databaseName": ...,
}

parent.get_kx_database(**kwargs)
```

1. See [:material-code-braces: GetKxDatabaseRequestRequestTypeDef](./type_defs.md#getkxdatabaserequestrequesttypedef) 

### get\_kx\_environment

Retrieves all the information for the specified kdb environment.

Type annotations and code completion for `#!python session.create_client("finspace").get_kx_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_environment)

```python
# get_kx_environment method definition

await def get_kx_environment(
    self,
    *,
    environmentId: str,
) -> GetKxEnvironmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKxEnvironmentResponseTypeDef](./type_defs.md#getkxenvironmentresponsetypedef) 


```python
# get_kx_environment method usage example with argument unpacking

kwargs: GetKxEnvironmentRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.get_kx_environment(**kwargs)
```

1. See [:material-code-braces: GetKxEnvironmentRequestRequestTypeDef](./type_defs.md#getkxenvironmentrequestrequesttypedef) 

### get\_kx\_user

Retrieves information about the specified kdb user.

Type annotations and code completion for `#!python session.create_client("finspace").get_kx_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_user)

```python
# get_kx_user method definition

await def get_kx_user(
    self,
    *,
    userName: str,
    environmentId: str,
) -> GetKxUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKxUserResponseTypeDef](./type_defs.md#getkxuserresponsetypedef) 


```python
# get_kx_user method usage example with argument unpacking

kwargs: GetKxUserRequestRequestTypeDef = {  # (1)
    "userName": ...,
    "environmentId": ...,
}

parent.get_kx_user(**kwargs)
```

1. See [:material-code-braces: GetKxUserRequestRequestTypeDef](./type_defs.md#getkxuserrequestrequesttypedef) 

### list\_environments

A list of all of your FinSpace environments.

Type annotations and code completion for `#!python session.create_client("finspace").list_environments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_environments)

```python
# list_environments method definition

await def list_environments(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListEnvironmentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef) 


```python
# list_environments method usage example with argument unpacking

kwargs: ListEnvironmentsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_environments(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsRequestRequestTypeDef](./type_defs.md#listenvironmentsrequestrequesttypedef) 

### list\_kx\_changesets

Returns a list of all the changesets for a database.

Type annotations and code completion for `#!python session.create_client("finspace").list_kx_changesets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_changesets)

```python
# list_kx_changesets method definition

await def list_kx_changesets(
    self,
    *,
    environmentId: str,
    databaseName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListKxChangesetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKxChangesetsResponseTypeDef](./type_defs.md#listkxchangesetsresponsetypedef) 


```python
# list_kx_changesets method usage example with argument unpacking

kwargs: ListKxChangesetsRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "databaseName": ...,
}

parent.list_kx_changesets(**kwargs)
```

1. See [:material-code-braces: ListKxChangesetsRequestRequestTypeDef](./type_defs.md#listkxchangesetsrequestrequesttypedef) 

### list\_kx\_cluster\_nodes

Lists all the nodes in a kdb cluster.

Type annotations and code completion for `#!python session.create_client("finspace").list_kx_cluster_nodes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_cluster_nodes)

```python
# list_kx_cluster_nodes method definition

await def list_kx_cluster_nodes(
    self,
    *,
    environmentId: str,
    clusterName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListKxClusterNodesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKxClusterNodesResponseTypeDef](./type_defs.md#listkxclusternodesresponsetypedef) 


```python
# list_kx_cluster_nodes method usage example with argument unpacking

kwargs: ListKxClusterNodesRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "clusterName": ...,
}

parent.list_kx_cluster_nodes(**kwargs)
```

1. See [:material-code-braces: ListKxClusterNodesRequestRequestTypeDef](./type_defs.md#listkxclusternodesrequestrequesttypedef) 

### list\_kx\_clusters

Returns a list of clusters.

Type annotations and code completion for `#!python session.create_client("finspace").list_kx_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_clusters)

```python
# list_kx_clusters method definition

await def list_kx_clusters(
    self,
    *,
    environmentId: str,
    clusterType: KxClusterTypeType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListKxClustersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: KxClusterTypeType](./literals.md#kxclustertypetype) 
2. See [:material-code-braces: ListKxClustersResponseTypeDef](./type_defs.md#listkxclustersresponsetypedef) 


```python
# list_kx_clusters method usage example with argument unpacking

kwargs: ListKxClustersRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.list_kx_clusters(**kwargs)
```

1. See [:material-code-braces: ListKxClustersRequestRequestTypeDef](./type_defs.md#listkxclustersrequestrequesttypedef) 

### list\_kx\_databases

Returns a list of all the databases in the kdb environment.

Type annotations and code completion for `#!python session.create_client("finspace").list_kx_databases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_databases)

```python
# list_kx_databases method definition

await def list_kx_databases(
    self,
    *,
    environmentId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListKxDatabasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKxDatabasesResponseTypeDef](./type_defs.md#listkxdatabasesresponsetypedef) 


```python
# list_kx_databases method usage example with argument unpacking

kwargs: ListKxDatabasesRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.list_kx_databases(**kwargs)
```

1. See [:material-code-braces: ListKxDatabasesRequestRequestTypeDef](./type_defs.md#listkxdatabasesrequestrequesttypedef) 

### list\_kx\_environments

Returns a list of kdb environments created in an account.

Type annotations and code completion for `#!python session.create_client("finspace").list_kx_environments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_environments)

```python
# list_kx_environments method definition

await def list_kx_environments(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListKxEnvironmentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKxEnvironmentsResponseTypeDef](./type_defs.md#listkxenvironmentsresponsetypedef) 


```python
# list_kx_environments method usage example with argument unpacking

kwargs: ListKxEnvironmentsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_kx_environments(**kwargs)
```

1. See [:material-code-braces: ListKxEnvironmentsRequestRequestTypeDef](./type_defs.md#listkxenvironmentsrequestrequesttypedef) 

### list\_kx\_users

Lists all the users in a kdb environment.

Type annotations and code completion for `#!python session.create_client("finspace").list_kx_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_users)

```python
# list_kx_users method definition

await def list_kx_users(
    self,
    *,
    environmentId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListKxUsersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKxUsersResponseTypeDef](./type_defs.md#listkxusersresponsetypedef) 


```python
# list_kx_users method usage example with argument unpacking

kwargs: ListKxUsersRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.list_kx_users(**kwargs)
```

1. See [:material-code-braces: ListKxUsersRequestRequestTypeDef](./type_defs.md#listkxusersrequestrequesttypedef) 

### list\_tags\_for\_resource

A list of all tags for a resource.

Type annotations and code completion for `#!python session.create_client("finspace").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_tags_for_resource)

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

### tag\_resource

Adds metadata tags to a FinSpace resource.

Type annotations and code completion for `#!python session.create_client("finspace").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes metadata tags from a FinSpace resource.

Type annotations and code completion for `#!python session.create_client("finspace").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_environment

Update your FinSpace environment.

Type annotations and code completion for `#!python session.create_client("finspace").update_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_environment)

```python
# update_environment method definition

await def update_environment(
    self,
    *,
    environmentId: str,
    name: str = ...,
    description: str = ...,
    federationMode: FederationModeType = ...,  # (1)
    federationParameters: FederationParametersTypeDef = ...,  # (2)
) -> UpdateEnvironmentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: FederationModeType](./literals.md#federationmodetype) 
2. See [:material-code-braces: FederationParametersTypeDef](./type_defs.md#federationparameterstypedef) 
3. See [:material-code-braces: UpdateEnvironmentResponseTypeDef](./type_defs.md#updateenvironmentresponsetypedef) 


```python
# update_environment method usage example with argument unpacking

kwargs: UpdateEnvironmentRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.update_environment(**kwargs)
```

1. See [:material-code-braces: UpdateEnvironmentRequestRequestTypeDef](./type_defs.md#updateenvironmentrequestrequesttypedef) 

### update\_kx\_cluster\_databases

Updates the databases mounted on a kdb cluster, which includes the `changesetId`
and all the dbPaths to be cached.

Type annotations and code completion for `#!python session.create_client("finspace").update_kx_cluster_databases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_cluster_databases)

```python
# update_kx_cluster_databases method definition

await def update_kx_cluster_databases(
    self,
    *,
    environmentId: str,
    clusterName: str,
    databases: Sequence[KxDatabaseConfigurationTypeDef],  # (1)
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: KxDatabaseConfigurationTypeDef](./type_defs.md#kxdatabaseconfigurationtypedef) 


```python
# update_kx_cluster_databases method usage example with argument unpacking

kwargs: UpdateKxClusterDatabasesRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "clusterName": ...,
    "databases": ...,
}

parent.update_kx_cluster_databases(**kwargs)
```

1. See [:material-code-braces: UpdateKxClusterDatabasesRequestRequestTypeDef](./type_defs.md#updatekxclusterdatabasesrequestrequesttypedef) 

### update\_kx\_database

Updates information for the given kdb database.

Type annotations and code completion for `#!python session.create_client("finspace").update_kx_database` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_database)

```python
# update_kx_database method definition

await def update_kx_database(
    self,
    *,
    environmentId: str,
    databaseName: str,
    clientToken: str,
    description: str = ...,
) -> UpdateKxDatabaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateKxDatabaseResponseTypeDef](./type_defs.md#updatekxdatabaseresponsetypedef) 


```python
# update_kx_database method usage example with argument unpacking

kwargs: UpdateKxDatabaseRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "databaseName": ...,
    "clientToken": ...,
}

parent.update_kx_database(**kwargs)
```

1. See [:material-code-braces: UpdateKxDatabaseRequestRequestTypeDef](./type_defs.md#updatekxdatabaserequestrequesttypedef) 

### update\_kx\_environment

Updates information for the given kdb environment.

Type annotations and code completion for `#!python session.create_client("finspace").update_kx_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_environment)

```python
# update_kx_environment method definition

await def update_kx_environment(
    self,
    *,
    environmentId: str,
    name: str = ...,
    description: str = ...,
    clientToken: str = ...,
) -> UpdateKxEnvironmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateKxEnvironmentResponseTypeDef](./type_defs.md#updatekxenvironmentresponsetypedef) 


```python
# update_kx_environment method usage example with argument unpacking

kwargs: UpdateKxEnvironmentRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.update_kx_environment(**kwargs)
```

1. See [:material-code-braces: UpdateKxEnvironmentRequestRequestTypeDef](./type_defs.md#updatekxenvironmentrequestrequesttypedef) 

### update\_kx\_environment\_network

Updates environment network to connect to your internal network by using a
transit gateway.

Type annotations and code completion for `#!python session.create_client("finspace").update_kx_environment_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_environment_network)

```python
# update_kx_environment_network method definition

await def update_kx_environment_network(
    self,
    *,
    environmentId: str,
    transitGatewayConfiguration: TransitGatewayConfigurationTypeDef = ...,  # (1)
    customDNSConfiguration: Sequence[CustomDNSServerTypeDef] = ...,  # (2)
    clientToken: str = ...,
) -> UpdateKxEnvironmentNetworkResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TransitGatewayConfigurationTypeDef](./type_defs.md#transitgatewayconfigurationtypedef) 
2. See [:material-code-braces: CustomDNSServerTypeDef](./type_defs.md#customdnsservertypedef) 
3. See [:material-code-braces: UpdateKxEnvironmentNetworkResponseTypeDef](./type_defs.md#updatekxenvironmentnetworkresponsetypedef) 


```python
# update_kx_environment_network method usage example with argument unpacking

kwargs: UpdateKxEnvironmentNetworkRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.update_kx_environment_network(**kwargs)
```

1. See [:material-code-braces: UpdateKxEnvironmentNetworkRequestRequestTypeDef](./type_defs.md#updatekxenvironmentnetworkrequestrequesttypedef) 

### update\_kx\_user

Updates the user details.

Type annotations and code completion for `#!python session.create_client("finspace").update_kx_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_user)

```python
# update_kx_user method definition

await def update_kx_user(
    self,
    *,
    environmentId: str,
    userName: str,
    iamRole: str,
    clientToken: str = ...,
) -> UpdateKxUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateKxUserResponseTypeDef](./type_defs.md#updatekxuserresponsetypedef) 


```python
# update_kx_user method usage example with argument unpacking

kwargs: UpdateKxUserRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
    "userName": ...,
    "iamRole": ...,
}

parent.update_kx_user(**kwargs)
```

1. See [:material-code-braces: UpdateKxUserRequestRequestTypeDef](./type_defs.md#updatekxuserrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("finspace").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> finspaceClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("finspace").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("finspace").get_paginator` method with overloads.

- `client.get_paginator("list_kx_environments")` -> [ListKxEnvironmentsPaginator](./paginators.md#listkxenvironmentspaginator)



