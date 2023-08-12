# AppFabricClient

> [Index](../README.md) > [AppFabric](./README.md) > AppFabricClient

!!! note ""

    Auto-generated documentation for [AppFabric](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
    type annotations stubs module [types-aiobotocore-appfabric](https://pypi.org/project/types-aiobotocore-appfabric/).

## AppFabricClient

Type annotations and code completion for `#!python session.create_client("appfabric")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client)

```python
AppFabricClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_appfabric.client import AppFabricClient

session = get_session()
async with session.create_client("appfabric") as client:
    client: AppFabricClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("appfabric").exceptions` structure.

```python
AppFabricClient.exceptions usage example

async with session.create_client("appfabric") as client:
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
        client.ValidationException,
    ) as e:
        print(e)
```

```python
AppFabricClient usage type checking example

from types_aiobotocore_appfabric.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### batch\_get\_user\_access\_tasks

Gets user access details in a batch request.

Type annotations and code completion for `#!python session.create_client("appfabric").batch_get_user_access_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.batch_get_user_access_tasks)

```python
# batch_get_user_access_tasks method definition

await def batch_get_user_access_tasks(
    self,
    *,
    appBundleIdentifier: str,
    taskIdList: Sequence[str],
) -> BatchGetUserAccessTasksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetUserAccessTasksResponseTypeDef](./type_defs.md#batchgetuseraccesstasksresponsetypedef) 


```python
# batch_get_user_access_tasks method usage example with argument unpacking

kwargs: BatchGetUserAccessTasksRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "taskIdList": ...,
}

parent.batch_get_user_access_tasks(**kwargs)
```

1. See [:material-code-braces: BatchGetUserAccessTasksRequestRequestTypeDef](./type_defs.md#batchgetuseraccesstasksrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("appfabric").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("appfabric").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### connect\_app\_authorization

Establishes a connection between Amazon Web Services AppFabric and an
application, which allows AppFabric to call the APIs of the application.

Type annotations and code completion for `#!python session.create_client("appfabric").connect_app_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.connect_app_authorization)

```python
# connect_app_authorization method definition

await def connect_app_authorization(
    self,
    *,
    appBundleIdentifier: str,
    appAuthorizationIdentifier: str,
    authRequest: AuthRequestTypeDef = ...,  # (1)
) -> ConnectAppAuthorizationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AuthRequestTypeDef](./type_defs.md#authrequesttypedef) 
2. See [:material-code-braces: ConnectAppAuthorizationResponseTypeDef](./type_defs.md#connectappauthorizationresponsetypedef) 


```python
# connect_app_authorization method usage example with argument unpacking

kwargs: ConnectAppAuthorizationRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "appAuthorizationIdentifier": ...,
}

parent.connect_app_authorization(**kwargs)
```

1. See [:material-code-braces: ConnectAppAuthorizationRequestRequestTypeDef](./type_defs.md#connectappauthorizationrequestrequesttypedef) 

### create\_app\_authorization

Creates an app authorization within an app bundle, which allows AppFabric to
connect to an application.

Type annotations and code completion for `#!python session.create_client("appfabric").create_app_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.create_app_authorization)

```python
# create_app_authorization method definition

await def create_app_authorization(
    self,
    *,
    appBundleIdentifier: str,
    app: str,
    credential: CredentialTypeDef,  # (1)
    tenant: TenantTypeDef,  # (2)
    authType: AuthTypeType,  # (3)
    clientToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateAppAuthorizationResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: CredentialTypeDef](./type_defs.md#credentialtypedef) 
2. See [:material-code-braces: TenantTypeDef](./type_defs.md#tenanttypedef) 
3. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateAppAuthorizationResponseTypeDef](./type_defs.md#createappauthorizationresponsetypedef) 


```python
# create_app_authorization method usage example with argument unpacking

kwargs: CreateAppAuthorizationRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "app": ...,
    "credential": ...,
    "tenant": ...,
    "authType": ...,
}

parent.create_app_authorization(**kwargs)
```

1. See [:material-code-braces: CreateAppAuthorizationRequestRequestTypeDef](./type_defs.md#createappauthorizationrequestrequesttypedef) 

### create\_app\_bundle

Creates an app bundle to collect data from an application using AppFabric.

Type annotations and code completion for `#!python session.create_client("appfabric").create_app_bundle` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.create_app_bundle)

```python
# create_app_bundle method definition

await def create_app_bundle(
    self,
    *,
    clientToken: str = ...,
    customerManagedKeyIdentifier: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateAppBundleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateAppBundleResponseTypeDef](./type_defs.md#createappbundleresponsetypedef) 


```python
# create_app_bundle method usage example with argument unpacking

kwargs: CreateAppBundleRequestRequestTypeDef = {  # (1)
    "clientToken": ...,
}

parent.create_app_bundle(**kwargs)
```

1. See [:material-code-braces: CreateAppBundleRequestRequestTypeDef](./type_defs.md#createappbundlerequestrequesttypedef) 

### create\_ingestion

Creates a data ingestion for an application.

Type annotations and code completion for `#!python session.create_client("appfabric").create_ingestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.create_ingestion)

```python
# create_ingestion method definition

await def create_ingestion(
    self,
    *,
    appBundleIdentifier: str,
    app: str,
    tenantId: str,
    ingestionType: IngestionTypeType,  # (1)
    clientToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateIngestionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: IngestionTypeType](./literals.md#ingestiontypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateIngestionResponseTypeDef](./type_defs.md#createingestionresponsetypedef) 


```python
# create_ingestion method usage example with argument unpacking

kwargs: CreateIngestionRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "app": ...,
    "tenantId": ...,
    "ingestionType": ...,
}

parent.create_ingestion(**kwargs)
```

1. See [:material-code-braces: CreateIngestionRequestRequestTypeDef](./type_defs.md#createingestionrequestrequesttypedef) 

### create\_ingestion\_destination

Creates an ingestion destination, which specifies how an application's ingested
data is processed by Amazon Web Services AppFabric and where it's delivered.

Type annotations and code completion for `#!python session.create_client("appfabric").create_ingestion_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.create_ingestion_destination)

```python
# create_ingestion_destination method definition

await def create_ingestion_destination(
    self,
    *,
    appBundleIdentifier: str,
    ingestionIdentifier: str,
    processingConfiguration: ProcessingConfigurationTypeDef,  # (1)
    destinationConfiguration: DestinationConfigurationTypeDef,  # (2)
    clientToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateIngestionDestinationResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) 
2. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateIngestionDestinationResponseTypeDef](./type_defs.md#createingestiondestinationresponsetypedef) 


```python
# create_ingestion_destination method usage example with argument unpacking

kwargs: CreateIngestionDestinationRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "ingestionIdentifier": ...,
    "processingConfiguration": ...,
    "destinationConfiguration": ...,
}

parent.create_ingestion_destination(**kwargs)
```

1. See [:material-code-braces: CreateIngestionDestinationRequestRequestTypeDef](./type_defs.md#createingestiondestinationrequestrequesttypedef) 

### delete\_app\_authorization

Deletes an app authorization.

Type annotations and code completion for `#!python session.create_client("appfabric").delete_app_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.delete_app_authorization)

```python
# delete_app_authorization method definition

await def delete_app_authorization(
    self,
    *,
    appBundleIdentifier: str,
    appAuthorizationIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_app_authorization method usage example with argument unpacking

kwargs: DeleteAppAuthorizationRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "appAuthorizationIdentifier": ...,
}

parent.delete_app_authorization(**kwargs)
```

1. See [:material-code-braces: DeleteAppAuthorizationRequestRequestTypeDef](./type_defs.md#deleteappauthorizationrequestrequesttypedef) 

### delete\_app\_bundle

Deletes an app bundle.

Type annotations and code completion for `#!python session.create_client("appfabric").delete_app_bundle` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.delete_app_bundle)

```python
# delete_app_bundle method definition

await def delete_app_bundle(
    self,
    *,
    appBundleIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_app_bundle method usage example with argument unpacking

kwargs: DeleteAppBundleRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
}

parent.delete_app_bundle(**kwargs)
```

1. See [:material-code-braces: DeleteAppBundleRequestRequestTypeDef](./type_defs.md#deleteappbundlerequestrequesttypedef) 

### delete\_ingestion

Deletes an ingestion.

Type annotations and code completion for `#!python session.create_client("appfabric").delete_ingestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.delete_ingestion)

```python
# delete_ingestion method definition

await def delete_ingestion(
    self,
    *,
    appBundleIdentifier: str,
    ingestionIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ingestion method usage example with argument unpacking

kwargs: DeleteIngestionRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "ingestionIdentifier": ...,
}

parent.delete_ingestion(**kwargs)
```

1. See [:material-code-braces: DeleteIngestionRequestRequestTypeDef](./type_defs.md#deleteingestionrequestrequesttypedef) 

### delete\_ingestion\_destination

Deletes an ingestion destination.

Type annotations and code completion for `#!python session.create_client("appfabric").delete_ingestion_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.delete_ingestion_destination)

```python
# delete_ingestion_destination method definition

await def delete_ingestion_destination(
    self,
    *,
    appBundleIdentifier: str,
    ingestionIdentifier: str,
    ingestionDestinationIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ingestion_destination method usage example with argument unpacking

kwargs: DeleteIngestionDestinationRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "ingestionIdentifier": ...,
    "ingestionDestinationIdentifier": ...,
}

parent.delete_ingestion_destination(**kwargs)
```

1. See [:material-code-braces: DeleteIngestionDestinationRequestRequestTypeDef](./type_defs.md#deleteingestiondestinationrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("appfabric").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.generate_presigned_url)

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


### get\_app\_authorization

Returns information about an app authorization.

Type annotations and code completion for `#!python session.create_client("appfabric").get_app_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.get_app_authorization)

```python
# get_app_authorization method definition

await def get_app_authorization(
    self,
    *,
    appBundleIdentifier: str,
    appAuthorizationIdentifier: str,
) -> GetAppAuthorizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAppAuthorizationResponseTypeDef](./type_defs.md#getappauthorizationresponsetypedef) 


```python
# get_app_authorization method usage example with argument unpacking

kwargs: GetAppAuthorizationRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "appAuthorizationIdentifier": ...,
}

parent.get_app_authorization(**kwargs)
```

1. See [:material-code-braces: GetAppAuthorizationRequestRequestTypeDef](./type_defs.md#getappauthorizationrequestrequesttypedef) 

### get\_app\_bundle

Returns information about an app bundle.

Type annotations and code completion for `#!python session.create_client("appfabric").get_app_bundle` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.get_app_bundle)

```python
# get_app_bundle method definition

await def get_app_bundle(
    self,
    *,
    appBundleIdentifier: str,
) -> GetAppBundleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAppBundleResponseTypeDef](./type_defs.md#getappbundleresponsetypedef) 


```python
# get_app_bundle method usage example with argument unpacking

kwargs: GetAppBundleRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
}

parent.get_app_bundle(**kwargs)
```

1. See [:material-code-braces: GetAppBundleRequestRequestTypeDef](./type_defs.md#getappbundlerequestrequesttypedef) 

### get\_ingestion

Returns information about an ingestion.

Type annotations and code completion for `#!python session.create_client("appfabric").get_ingestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.get_ingestion)

```python
# get_ingestion method definition

await def get_ingestion(
    self,
    *,
    appBundleIdentifier: str,
    ingestionIdentifier: str,
) -> GetIngestionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIngestionResponseTypeDef](./type_defs.md#getingestionresponsetypedef) 


```python
# get_ingestion method usage example with argument unpacking

kwargs: GetIngestionRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "ingestionIdentifier": ...,
}

parent.get_ingestion(**kwargs)
```

1. See [:material-code-braces: GetIngestionRequestRequestTypeDef](./type_defs.md#getingestionrequestrequesttypedef) 

### get\_ingestion\_destination

Returns information about an ingestion destination.

Type annotations and code completion for `#!python session.create_client("appfabric").get_ingestion_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.get_ingestion_destination)

```python
# get_ingestion_destination method definition

await def get_ingestion_destination(
    self,
    *,
    appBundleIdentifier: str,
    ingestionIdentifier: str,
    ingestionDestinationIdentifier: str,
) -> GetIngestionDestinationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIngestionDestinationResponseTypeDef](./type_defs.md#getingestiondestinationresponsetypedef) 


```python
# get_ingestion_destination method usage example with argument unpacking

kwargs: GetIngestionDestinationRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "ingestionIdentifier": ...,
    "ingestionDestinationIdentifier": ...,
}

parent.get_ingestion_destination(**kwargs)
```

1. See [:material-code-braces: GetIngestionDestinationRequestRequestTypeDef](./type_defs.md#getingestiondestinationrequestrequesttypedef) 

### list\_app\_authorizations

Returns a list of all app authorizations configured for an app bundle.

Type annotations and code completion for `#!python session.create_client("appfabric").list_app_authorizations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.list_app_authorizations)

```python
# list_app_authorizations method definition

await def list_app_authorizations(
    self,
    *,
    appBundleIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAppAuthorizationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppAuthorizationsResponseTypeDef](./type_defs.md#listappauthorizationsresponsetypedef) 


```python
# list_app_authorizations method usage example with argument unpacking

kwargs: ListAppAuthorizationsRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
}

parent.list_app_authorizations(**kwargs)
```

1. See [:material-code-braces: ListAppAuthorizationsRequestRequestTypeDef](./type_defs.md#listappauthorizationsrequestrequesttypedef) 

### list\_app\_bundles

Returns a list of app bundles.

Type annotations and code completion for `#!python session.create_client("appfabric").list_app_bundles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.list_app_bundles)

```python
# list_app_bundles method definition

await def list_app_bundles(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAppBundlesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppBundlesResponseTypeDef](./type_defs.md#listappbundlesresponsetypedef) 


```python
# list_app_bundles method usage example with argument unpacking

kwargs: ListAppBundlesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_app_bundles(**kwargs)
```

1. See [:material-code-braces: ListAppBundlesRequestRequestTypeDef](./type_defs.md#listappbundlesrequestrequesttypedef) 

### list\_ingestion\_destinations

Returns a list of all ingestion destinations configured for an ingestion.

Type annotations and code completion for `#!python session.create_client("appfabric").list_ingestion_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.list_ingestion_destinations)

```python
# list_ingestion_destinations method definition

await def list_ingestion_destinations(
    self,
    *,
    appBundleIdentifier: str,
    ingestionIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListIngestionDestinationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIngestionDestinationsResponseTypeDef](./type_defs.md#listingestiondestinationsresponsetypedef) 


```python
# list_ingestion_destinations method usage example with argument unpacking

kwargs: ListIngestionDestinationsRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "ingestionIdentifier": ...,
}

parent.list_ingestion_destinations(**kwargs)
```

1. See [:material-code-braces: ListIngestionDestinationsRequestRequestTypeDef](./type_defs.md#listingestiondestinationsrequestrequesttypedef) 

### list\_ingestions

Returns a list of all ingestions configured for an app bundle.

Type annotations and code completion for `#!python session.create_client("appfabric").list_ingestions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.list_ingestions)

```python
# list_ingestions method definition

await def list_ingestions(
    self,
    *,
    appBundleIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListIngestionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIngestionsResponseTypeDef](./type_defs.md#listingestionsresponsetypedef) 


```python
# list_ingestions method usage example with argument unpacking

kwargs: ListIngestionsRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
}

parent.list_ingestions(**kwargs)
```

1. See [:material-code-braces: ListIngestionsRequestRequestTypeDef](./type_defs.md#listingestionsrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags for a resource.

Type annotations and code completion for `#!python session.create_client("appfabric").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.list_tags_for_resource)

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

### start\_ingestion

Starts (enables) an ingestion, which collects data from an application.

Type annotations and code completion for `#!python session.create_client("appfabric").start_ingestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.start_ingestion)

```python
# start_ingestion method definition

await def start_ingestion(
    self,
    *,
    ingestionIdentifier: str,
    appBundleIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# start_ingestion method usage example with argument unpacking

kwargs: StartIngestionRequestRequestTypeDef = {  # (1)
    "ingestionIdentifier": ...,
    "appBundleIdentifier": ...,
}

parent.start_ingestion(**kwargs)
```

1. See [:material-code-braces: StartIngestionRequestRequestTypeDef](./type_defs.md#startingestionrequestrequesttypedef) 

### start\_user\_access\_tasks

Starts the tasks to search user access status for a specific email address.

Type annotations and code completion for `#!python session.create_client("appfabric").start_user_access_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.start_user_access_tasks)

```python
# start_user_access_tasks method definition

await def start_user_access_tasks(
    self,
    *,
    appBundleIdentifier: str,
    email: str,
) -> StartUserAccessTasksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartUserAccessTasksResponseTypeDef](./type_defs.md#startuseraccesstasksresponsetypedef) 


```python
# start_user_access_tasks method usage example with argument unpacking

kwargs: StartUserAccessTasksRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "email": ...,
}

parent.start_user_access_tasks(**kwargs)
```

1. See [:material-code-braces: StartUserAccessTasksRequestRequestTypeDef](./type_defs.md#startuseraccesstasksrequestrequesttypedef) 

### stop\_ingestion

Stops (disables) an ingestion.

Type annotations and code completion for `#!python session.create_client("appfabric").stop_ingestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.stop_ingestion)

```python
# stop_ingestion method definition

await def stop_ingestion(
    self,
    *,
    ingestionIdentifier: str,
    appBundleIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_ingestion method usage example with argument unpacking

kwargs: StopIngestionRequestRequestTypeDef = {  # (1)
    "ingestionIdentifier": ...,
    "appBundleIdentifier": ...,
}

parent.stop_ingestion(**kwargs)
```

1. See [:material-code-braces: StopIngestionRequestRequestTypeDef](./type_defs.md#stopingestionrequestrequesttypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified resource.

Type annotations and code completion for `#!python session.create_client("appfabric").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


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

Removes a tag or tags from a resource.

Type annotations and code completion for `#!python session.create_client("appfabric").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.untag_resource)

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

### update\_app\_authorization

Updates an app authorization within an app bundle, which allows AppFabric to
connect to an application.

Type annotations and code completion for `#!python session.create_client("appfabric").update_app_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.update_app_authorization)

```python
# update_app_authorization method definition

await def update_app_authorization(
    self,
    *,
    appBundleIdentifier: str,
    appAuthorizationIdentifier: str,
    credential: CredentialTypeDef = ...,  # (1)
    tenant: TenantTypeDef = ...,  # (2)
) -> UpdateAppAuthorizationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: CredentialTypeDef](./type_defs.md#credentialtypedef) 
2. See [:material-code-braces: TenantTypeDef](./type_defs.md#tenanttypedef) 
3. See [:material-code-braces: UpdateAppAuthorizationResponseTypeDef](./type_defs.md#updateappauthorizationresponsetypedef) 


```python
# update_app_authorization method usage example with argument unpacking

kwargs: UpdateAppAuthorizationRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "appAuthorizationIdentifier": ...,
}

parent.update_app_authorization(**kwargs)
```

1. See [:material-code-braces: UpdateAppAuthorizationRequestRequestTypeDef](./type_defs.md#updateappauthorizationrequestrequesttypedef) 

### update\_ingestion\_destination

Updates an ingestion destination, which specifies how an application's ingested
data is processed by Amazon Web Services AppFabric and where it's delivered.

Type annotations and code completion for `#!python session.create_client("appfabric").update_ingestion_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.update_ingestion_destination)

```python
# update_ingestion_destination method definition

await def update_ingestion_destination(
    self,
    *,
    appBundleIdentifier: str,
    ingestionIdentifier: str,
    ingestionDestinationIdentifier: str,
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
) -> UpdateIngestionDestinationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-braces: UpdateIngestionDestinationResponseTypeDef](./type_defs.md#updateingestiondestinationresponsetypedef) 


```python
# update_ingestion_destination method usage example with argument unpacking

kwargs: UpdateIngestionDestinationRequestRequestTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "ingestionIdentifier": ...,
    "ingestionDestinationIdentifier": ...,
    "destinationConfiguration": ...,
}

parent.update_ingestion_destination(**kwargs)
```

1. See [:material-code-braces: UpdateIngestionDestinationRequestRequestTypeDef](./type_defs.md#updateingestiondestinationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("appfabric").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> AppFabricClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("appfabric").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("appfabric").get_paginator` method with overloads.

- `client.get_paginator("list_app_authorizations")` -> [ListAppAuthorizationsPaginator](./paginators.md#listappauthorizationspaginator)
- `client.get_paginator("list_app_bundles")` -> [ListAppBundlesPaginator](./paginators.md#listappbundlespaginator)
- `client.get_paginator("list_ingestion_destinations")` -> [ListIngestionDestinationsPaginator](./paginators.md#listingestiondestinationspaginator)
- `client.get_paginator("list_ingestions")` -> [ListIngestionsPaginator](./paginators.md#listingestionspaginator)



