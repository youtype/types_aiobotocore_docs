# AppIntegrationsServiceClient

> [Index](../README.md) > [AppIntegrationsService](./README.md) > AppIntegrationsServiceClient

!!! note ""

    Auto-generated documentation for [AppIntegrationsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#appintegrationsservice)
    type annotations stubs module [types-aiobotocore-appintegrations](https://pypi.org/project/types-aiobotocore-appintegrations/).

## AppIntegrationsServiceClient

Type annotations and code completion for `#!python session.create_client("appintegrations")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client)

```python
# AppIntegrationsServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_appintegrations.client import AppIntegrationsServiceClient

session = get_session()
async with session.create_client("appintegrations") as client:
    client: AppIntegrationsServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("appintegrations").exceptions` structure.

```python
# AppIntegrationsServiceClient.exceptions usage example

async with session.create_client("appintegrations") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.DuplicateResourceException,
        client.InternalServiceError,
        client.InvalidRequestException,
        client.ResourceNotFoundException,
        client.ResourceQuotaExceededException,
        client.ThrottlingException,
        client.UnsupportedOperationException,
    ) as e:
        print(e)
```

```python
# AppIntegrationsServiceClient usage type checking example

from types_aiobotocore_appintegrations.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("appintegrations").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("appintegrations").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/generate_presigned_url.html)

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


### create\_application

Creates and persists an Application resource.

Type annotations and code completion for `#!python session.create_client("appintegrations").create_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/create_application.html)

```python
# create_application method definition

await def create_application(
    self,
    *,
    Name: str,
    Namespace: str,
    ApplicationSourceConfig: ApplicationSourceConfigUnionTypeDef,  # (1)
    Description: str = ...,
    Subscriptions: Sequence[SubscriptionTypeDef] = ...,  # (2)
    Publications: Sequence[PublicationTypeDef] = ...,  # (3)
    ClientToken: str = ...,
    Tags: Mapping[str, str] = ...,
    Permissions: Sequence[str] = ...,
) -> CreateApplicationResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ApplicationSourceConfigTypeDef](./type_defs.md#applicationsourceconfigtypedef) [:material-code-braces: ApplicationSourceConfigOutputTypeDef](./type_defs.md#applicationsourceconfigoutputtypedef) 
2. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
3. See [:material-code-braces: PublicationTypeDef](./type_defs.md#publicationtypedef) 
4. See [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 


```python
# create_application method usage example with argument unpacking

kwargs: CreateApplicationRequestTypeDef = {  # (1)
    "Name": ...,
    "Namespace": ...,
    "ApplicationSourceConfig": ...,
}

parent.create_application(**kwargs)
```

1. See [:material-code-braces: CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef) 

### create\_data\_integration

Creates and persists a DataIntegration resource.

Type annotations and code completion for `#!python session.create_client("appintegrations").create_data_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/create_data_integration.html)

```python
# create_data_integration method definition

await def create_data_integration(
    self,
    *,
    Name: str,
    KmsKey: str,
    Description: str = ...,
    SourceURI: str = ...,
    ScheduleConfig: ScheduleConfigurationTypeDef = ...,  # (1)
    Tags: Mapping[str, str] = ...,
    ClientToken: str = ...,
    FileConfiguration: FileConfigurationUnionTypeDef = ...,  # (2)
    ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...,
) -> CreateDataIntegrationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
2. See [:material-code-braces: FileConfigurationTypeDef](./type_defs.md#fileconfigurationtypedef) [:material-code-braces: FileConfigurationOutputTypeDef](./type_defs.md#fileconfigurationoutputtypedef) 
3. See [:material-code-braces: CreateDataIntegrationResponseTypeDef](./type_defs.md#createdataintegrationresponsetypedef) 


```python
# create_data_integration method usage example with argument unpacking

kwargs: CreateDataIntegrationRequestTypeDef = {  # (1)
    "Name": ...,
    "KmsKey": ...,
}

parent.create_data_integration(**kwargs)
```

1. See [:material-code-braces: CreateDataIntegrationRequestTypeDef](./type_defs.md#createdataintegrationrequesttypedef) 

### create\_data\_integration\_association

Creates and persists a DataIntegrationAssociation resource.

Type annotations and code completion for `#!python session.create_client("appintegrations").create_data_integration_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/create_data_integration_association.html)

```python
# create_data_integration_association method definition

await def create_data_integration_association(
    self,
    *,
    DataIntegrationIdentifier: str,
    ClientId: str = ...,
    ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...,
    DestinationURI: str = ...,
    ClientAssociationMetadata: Mapping[str, str] = ...,
    ClientToken: str = ...,
    ExecutionConfiguration: ExecutionConfigurationTypeDef = ...,  # (1)
) -> CreateDataIntegrationAssociationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ExecutionConfigurationTypeDef](./type_defs.md#executionconfigurationtypedef) 
2. See [:material-code-braces: CreateDataIntegrationAssociationResponseTypeDef](./type_defs.md#createdataintegrationassociationresponsetypedef) 


```python
# create_data_integration_association method usage example with argument unpacking

kwargs: CreateDataIntegrationAssociationRequestTypeDef = {  # (1)
    "DataIntegrationIdentifier": ...,
}

parent.create_data_integration_association(**kwargs)
```

1. See [:material-code-braces: CreateDataIntegrationAssociationRequestTypeDef](./type_defs.md#createdataintegrationassociationrequesttypedef) 

### create\_event\_integration

Creates an EventIntegration, given a specified name, description, and a
reference to an Amazon EventBridge bus in your account and a partner event
source that pushes events to that bus.

Type annotations and code completion for `#!python session.create_client("appintegrations").create_event_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/create_event_integration.html)

```python
# create_event_integration method definition

await def create_event_integration(
    self,
    *,
    Name: str,
    EventFilter: EventFilterTypeDef,  # (1)
    EventBridgeBus: str,
    Description: str = ...,
    ClientToken: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateEventIntegrationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
2. See [:material-code-braces: CreateEventIntegrationResponseTypeDef](./type_defs.md#createeventintegrationresponsetypedef) 


```python
# create_event_integration method usage example with argument unpacking

kwargs: CreateEventIntegrationRequestTypeDef = {  # (1)
    "Name": ...,
    "EventFilter": ...,
    "EventBridgeBus": ...,
}

parent.create_event_integration(**kwargs)
```

1. See [:material-code-braces: CreateEventIntegrationRequestTypeDef](./type_defs.md#createeventintegrationrequesttypedef) 

### delete\_application

Deletes the Application.

Type annotations and code completion for `#!python session.create_client("appintegrations").delete_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/delete_application.html)

```python
# delete_application method definition

await def delete_application(
    self,
    *,
    Arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_application method usage example with argument unpacking

kwargs: DeleteApplicationRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.delete_application(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationRequestTypeDef](./type_defs.md#deleteapplicationrequesttypedef) 

### delete\_data\_integration

Deletes the DataIntegration.

Type annotations and code completion for `#!python session.create_client("appintegrations").delete_data_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/delete_data_integration.html)

```python
# delete_data_integration method definition

await def delete_data_integration(
    self,
    *,
    DataIntegrationIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_data_integration method usage example with argument unpacking

kwargs: DeleteDataIntegrationRequestTypeDef = {  # (1)
    "DataIntegrationIdentifier": ...,
}

parent.delete_data_integration(**kwargs)
```

1. See [:material-code-braces: DeleteDataIntegrationRequestTypeDef](./type_defs.md#deletedataintegrationrequesttypedef) 

### delete\_event\_integration

Deletes the specified existing event integration.

Type annotations and code completion for `#!python session.create_client("appintegrations").delete_event_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/delete_event_integration.html)

```python
# delete_event_integration method definition

await def delete_event_integration(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_event_integration method usage example with argument unpacking

kwargs: DeleteEventIntegrationRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_event_integration(**kwargs)
```

1. See [:material-code-braces: DeleteEventIntegrationRequestTypeDef](./type_defs.md#deleteeventintegrationrequesttypedef) 

### get\_application

Get an Application resource.

Type annotations and code completion for `#!python session.create_client("appintegrations").get_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/get_application.html)

```python
# get_application method definition

await def get_application(
    self,
    *,
    Arn: str,
) -> GetApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApplicationResponseTypeDef](./type_defs.md#getapplicationresponsetypedef) 


```python
# get_application method usage example with argument unpacking

kwargs: GetApplicationRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.get_application(**kwargs)
```

1. See [:material-code-braces: GetApplicationRequestTypeDef](./type_defs.md#getapplicationrequesttypedef) 

### get\_data\_integration

Returns information about the DataIntegration.

Type annotations and code completion for `#!python session.create_client("appintegrations").get_data_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/get_data_integration.html)

```python
# get_data_integration method definition

await def get_data_integration(
    self,
    *,
    Identifier: str,
) -> GetDataIntegrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataIntegrationResponseTypeDef](./type_defs.md#getdataintegrationresponsetypedef) 


```python
# get_data_integration method usage example with argument unpacking

kwargs: GetDataIntegrationRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.get_data_integration(**kwargs)
```

1. See [:material-code-braces: GetDataIntegrationRequestTypeDef](./type_defs.md#getdataintegrationrequesttypedef) 

### get\_event\_integration

Returns information about the event integration.

Type annotations and code completion for `#!python session.create_client("appintegrations").get_event_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/get_event_integration.html)

```python
# get_event_integration method definition

await def get_event_integration(
    self,
    *,
    Name: str,
) -> GetEventIntegrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEventIntegrationResponseTypeDef](./type_defs.md#geteventintegrationresponsetypedef) 


```python
# get_event_integration method usage example with argument unpacking

kwargs: GetEventIntegrationRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_event_integration(**kwargs)
```

1. See [:material-code-braces: GetEventIntegrationRequestTypeDef](./type_defs.md#geteventintegrationrequesttypedef) 

### list\_application\_associations

Returns a paginated list of application associations for an application.

Type annotations and code completion for `#!python session.create_client("appintegrations").list_application_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/list_application_associations.html)

```python
# list_application_associations method definition

await def list_application_associations(
    self,
    *,
    ApplicationId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListApplicationAssociationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationAssociationsResponseTypeDef](./type_defs.md#listapplicationassociationsresponsetypedef) 


```python
# list_application_associations method usage example with argument unpacking

kwargs: ListApplicationAssociationsRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.list_application_associations(**kwargs)
```

1. See [:material-code-braces: ListApplicationAssociationsRequestTypeDef](./type_defs.md#listapplicationassociationsrequesttypedef) 

### list\_applications

Lists applications in the account.

Type annotations and code completion for `#!python session.create_client("appintegrations").list_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/list_applications.html)

```python
# list_applications method definition

await def list_applications(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListApplicationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python
# list_applications method usage example with argument unpacking

kwargs: ListApplicationsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_applications(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestTypeDef](./type_defs.md#listapplicationsrequesttypedef) 

### list\_data\_integration\_associations

Returns a paginated list of DataIntegration associations in the account.

Type annotations and code completion for `#!python session.create_client("appintegrations").list_data_integration_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/list_data_integration_associations.html)

```python
# list_data_integration_associations method definition

await def list_data_integration_associations(
    self,
    *,
    DataIntegrationIdentifier: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDataIntegrationAssociationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataIntegrationAssociationsResponseTypeDef](./type_defs.md#listdataintegrationassociationsresponsetypedef) 


```python
# list_data_integration_associations method usage example with argument unpacking

kwargs: ListDataIntegrationAssociationsRequestTypeDef = {  # (1)
    "DataIntegrationIdentifier": ...,
}

parent.list_data_integration_associations(**kwargs)
```

1. See [:material-code-braces: ListDataIntegrationAssociationsRequestTypeDef](./type_defs.md#listdataintegrationassociationsrequesttypedef) 

### list\_data\_integrations

Returns a paginated list of DataIntegrations in the account.

Type annotations and code completion for `#!python session.create_client("appintegrations").list_data_integrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/list_data_integrations.html)

```python
# list_data_integrations method definition

await def list_data_integrations(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDataIntegrationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataIntegrationsResponseTypeDef](./type_defs.md#listdataintegrationsresponsetypedef) 


```python
# list_data_integrations method usage example with argument unpacking

kwargs: ListDataIntegrationsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_data_integrations(**kwargs)
```

1. See [:material-code-braces: ListDataIntegrationsRequestTypeDef](./type_defs.md#listdataintegrationsrequesttypedef) 

### list\_event\_integration\_associations

Returns a paginated list of event integration associations in the account.

Type annotations and code completion for `#!python session.create_client("appintegrations").list_event_integration_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/list_event_integration_associations.html)

```python
# list_event_integration_associations method definition

await def list_event_integration_associations(
    self,
    *,
    EventIntegrationName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEventIntegrationAssociationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEventIntegrationAssociationsResponseTypeDef](./type_defs.md#listeventintegrationassociationsresponsetypedef) 


```python
# list_event_integration_associations method usage example with argument unpacking

kwargs: ListEventIntegrationAssociationsRequestTypeDef = {  # (1)
    "EventIntegrationName": ...,
}

parent.list_event_integration_associations(**kwargs)
```

1. See [:material-code-braces: ListEventIntegrationAssociationsRequestTypeDef](./type_defs.md#listeventintegrationassociationsrequesttypedef) 

### list\_event\_integrations

Returns a paginated list of event integrations in the account.

Type annotations and code completion for `#!python session.create_client("appintegrations").list_event_integrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/list_event_integrations.html)

```python
# list_event_integrations method definition

await def list_event_integrations(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEventIntegrationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEventIntegrationsResponseTypeDef](./type_defs.md#listeventintegrationsresponsetypedef) 


```python
# list_event_integrations method usage example with argument unpacking

kwargs: ListEventIntegrationsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_event_integrations(**kwargs)
```

1. See [:material-code-braces: ListEventIntegrationsRequestTypeDef](./type_defs.md#listeventintegrationsrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("appintegrations").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/list_tags_for_resource.html)

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

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### tag\_resource

Adds the specified tags to the specified resource.

Type annotations and code completion for `#!python session.create_client("appintegrations").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/tag_resource.html)

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

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes the specified tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("appintegrations").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/untag_resource.html)

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

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_application

Updates and persists an Application resource.

Type annotations and code completion for `#!python session.create_client("appintegrations").update_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/update_application.html)

```python
# update_application method definition

await def update_application(
    self,
    *,
    Arn: str,
    Name: str = ...,
    Description: str = ...,
    ApplicationSourceConfig: ApplicationSourceConfigUnionTypeDef = ...,  # (1)
    Subscriptions: Sequence[SubscriptionTypeDef] = ...,  # (2)
    Publications: Sequence[PublicationTypeDef] = ...,  # (3)
    Permissions: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ApplicationSourceConfigTypeDef](./type_defs.md#applicationsourceconfigtypedef) [:material-code-braces: ApplicationSourceConfigOutputTypeDef](./type_defs.md#applicationsourceconfigoutputtypedef) 
2. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
3. See [:material-code-braces: PublicationTypeDef](./type_defs.md#publicationtypedef) 


```python
# update_application method usage example with argument unpacking

kwargs: UpdateApplicationRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.update_application(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationRequestTypeDef](./type_defs.md#updateapplicationrequesttypedef) 

### update\_data\_integration

Updates the description of a DataIntegration.

Type annotations and code completion for `#!python session.create_client("appintegrations").update_data_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/update_data_integration.html)

```python
# update_data_integration method definition

await def update_data_integration(
    self,
    *,
    Identifier: str,
    Name: str = ...,
    Description: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_data_integration method usage example with argument unpacking

kwargs: UpdateDataIntegrationRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.update_data_integration(**kwargs)
```

1. See [:material-code-braces: UpdateDataIntegrationRequestTypeDef](./type_defs.md#updatedataintegrationrequesttypedef) 

### update\_data\_integration\_association

Updates and persists a DataIntegrationAssociation resource.

Type annotations and code completion for `#!python session.create_client("appintegrations").update_data_integration_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/update_data_integration_association.html)

```python
# update_data_integration_association method definition

await def update_data_integration_association(
    self,
    *,
    DataIntegrationIdentifier: str,
    DataIntegrationAssociationIdentifier: str,
    ExecutionConfiguration: ExecutionConfigurationTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ExecutionConfigurationTypeDef](./type_defs.md#executionconfigurationtypedef) 


```python
# update_data_integration_association method usage example with argument unpacking

kwargs: UpdateDataIntegrationAssociationRequestTypeDef = {  # (1)
    "DataIntegrationIdentifier": ...,
    "DataIntegrationAssociationIdentifier": ...,
    "ExecutionConfiguration": ...,
}

parent.update_data_integration_association(**kwargs)
```

1. See [:material-code-braces: UpdateDataIntegrationAssociationRequestTypeDef](./type_defs.md#updatedataintegrationassociationrequesttypedef) 

### update\_event\_integration

Updates the description of an event integration.

Type annotations and code completion for `#!python session.create_client("appintegrations").update_event_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/client/update_event_integration.html)

```python
# update_event_integration method definition

await def update_event_integration(
    self,
    *,
    Name: str,
    Description: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_event_integration method usage example with argument unpacking

kwargs: UpdateEventIntegrationRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_event_integration(**kwargs)
```

1. See [:material-code-braces: UpdateEventIntegrationRequestTypeDef](./type_defs.md#updateeventintegrationrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("appintegrations").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("appintegrations").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client)

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

Type annotations and code completion for `#!python session.create_client("appintegrations").get_paginator` method with overloads.

- `client.get_paginator("list_application_associations")` -> [ListApplicationAssociationsPaginator](./paginators.md#listapplicationassociationspaginator)
- `client.get_paginator("list_applications")` -> [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- `client.get_paginator("list_data_integration_associations")` -> [ListDataIntegrationAssociationsPaginator](./paginators.md#listdataintegrationassociationspaginator)
- `client.get_paginator("list_data_integrations")` -> [ListDataIntegrationsPaginator](./paginators.md#listdataintegrationspaginator)
- `client.get_paginator("list_event_integration_associations")` -> [ListEventIntegrationAssociationsPaginator](./paginators.md#listeventintegrationassociationspaginator)
- `client.get_paginator("list_event_integrations")` -> [ListEventIntegrationsPaginator](./paginators.md#listeventintegrationspaginator)



