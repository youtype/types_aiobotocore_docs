# IoTTwinMakerClient

> [Index](../README.md) > [IoTTwinMaker](./README.md) > IoTTwinMakerClient

!!! note ""

    Auto-generated documentation for [IoTTwinMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#iottwinmaker)
    type annotations stubs module [types-aiobotocore-iottwinmaker](https://pypi.org/project/types-aiobotocore-iottwinmaker/).

## IoTTwinMakerClient

Type annotations and code completion for `#!python session.create_client("iottwinmaker")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client)

```python
# IoTTwinMakerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_iottwinmaker.client import IoTTwinMakerClient

session = get_session()
async with session.create_client("iottwinmaker") as client:
    client: IoTTwinMakerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("iottwinmaker").exceptions` structure.

```python
# IoTTwinMakerClient.exceptions usage example

async with session.create_client("iottwinmaker") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.ConnectorFailureException,
        client.ConnectorTimeoutException,
        client.InternalServerException,
        client.QueryTimeoutException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.TooManyTagsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# IoTTwinMakerClient usage type checking example

from types_aiobotocore_iottwinmaker.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("iottwinmaker").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("iottwinmaker").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/generate_presigned_url.html)

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



Type annotations and code completion for `#!python session.create_client("iottwinmaker").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### batch\_put\_property\_values

Sets values for multiple time series properties.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").batch_put_property_values` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/batch_put_property_values.html)

```python
# batch_put_property_values method definition

await def batch_put_property_values(
    self,
    *,
    workspaceId: str,
    entries: Sequence[PropertyValueEntryUnionTypeDef],  # (1)
) -> BatchPutPropertyValuesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PropertyValueEntryTypeDef](./type_defs.md#propertyvalueentrytypedef) [:material-code-braces: PropertyValueEntryOutputTypeDef](./type_defs.md#propertyvalueentryoutputtypedef) 
2. See [:material-code-braces: BatchPutPropertyValuesResponseTypeDef](./type_defs.md#batchputpropertyvaluesresponsetypedef) 


```python
# batch_put_property_values method usage example with argument unpacking

kwargs: BatchPutPropertyValuesRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "entries": ...,
}

parent.batch_put_property_values(**kwargs)
```

1. See [:material-code-braces: BatchPutPropertyValuesRequestRequestTypeDef](./type_defs.md#batchputpropertyvaluesrequestrequesttypedef) 

### cancel\_metadata\_transfer\_job

Cancels the metadata transfer job.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").cancel_metadata_transfer_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/cancel_metadata_transfer_job.html)

```python
# cancel_metadata_transfer_job method definition

await def cancel_metadata_transfer_job(
    self,
    *,
    metadataTransferJobId: str,
) -> CancelMetadataTransferJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelMetadataTransferJobResponseTypeDef](./type_defs.md#cancelmetadatatransferjobresponsetypedef) 


```python
# cancel_metadata_transfer_job method usage example with argument unpacking

kwargs: CancelMetadataTransferJobRequestRequestTypeDef = {  # (1)
    "metadataTransferJobId": ...,
}

parent.cancel_metadata_transfer_job(**kwargs)
```

1. See [:material-code-braces: CancelMetadataTransferJobRequestRequestTypeDef](./type_defs.md#cancelmetadatatransferjobrequestrequesttypedef) 

### create\_component\_type

Creates a component type.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").create_component_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/create_component_type.html)

```python
# create_component_type method definition

await def create_component_type(
    self,
    *,
    workspaceId: str,
    componentTypeId: str,
    isSingleton: bool = ...,
    description: str = ...,
    propertyDefinitions: Mapping[str, PropertyDefinitionRequestTypeDef] = ...,  # (1)
    extendsFrom: Sequence[str] = ...,
    functions: Mapping[str, FunctionRequestTypeDef] = ...,  # (2)
    tags: Mapping[str, str] = ...,
    propertyGroups: Mapping[str, PropertyGroupRequestTypeDef] = ...,  # (3)
    componentTypeName: str = ...,
    compositeComponentTypes: Mapping[str, CompositeComponentTypeRequestTypeDef] = ...,  # (4)
) -> CreateComponentTypeResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: PropertyDefinitionRequestTypeDef](./type_defs.md#propertydefinitionrequesttypedef) 
2. See [:material-code-braces: FunctionRequestTypeDef](./type_defs.md#functionrequesttypedef) 
3. See [:material-code-braces: PropertyGroupRequestTypeDef](./type_defs.md#propertygrouprequesttypedef) 
4. See [:material-code-braces: CompositeComponentTypeRequestTypeDef](./type_defs.md#compositecomponenttyperequesttypedef) 
5. See [:material-code-braces: CreateComponentTypeResponseTypeDef](./type_defs.md#createcomponenttyperesponsetypedef) 


```python
# create_component_type method usage example with argument unpacking

kwargs: CreateComponentTypeRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "componentTypeId": ...,
}

parent.create_component_type(**kwargs)
```

1. See [:material-code-braces: CreateComponentTypeRequestRequestTypeDef](./type_defs.md#createcomponenttyperequestrequesttypedef) 

### create\_entity

Creates an entity.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").create_entity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/create_entity.html)

```python
# create_entity method definition

await def create_entity(
    self,
    *,
    workspaceId: str,
    entityName: str,
    entityId: str = ...,
    description: str = ...,
    components: Mapping[str, ComponentRequestTypeDef] = ...,  # (1)
    compositeComponents: Mapping[str, CompositeComponentRequestTypeDef] = ...,  # (2)
    parentEntityId: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateEntityResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ComponentRequestTypeDef](./type_defs.md#componentrequesttypedef) 
2. See [:material-code-braces: CompositeComponentRequestTypeDef](./type_defs.md#compositecomponentrequesttypedef) 
3. See [:material-code-braces: CreateEntityResponseTypeDef](./type_defs.md#createentityresponsetypedef) 


```python
# create_entity method usage example with argument unpacking

kwargs: CreateEntityRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "entityName": ...,
}

parent.create_entity(**kwargs)
```

1. See [:material-code-braces: CreateEntityRequestRequestTypeDef](./type_defs.md#createentityrequestrequesttypedef) 

### create\_metadata\_transfer\_job

Creates a new metadata transfer job.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").create_metadata_transfer_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/create_metadata_transfer_job.html)

```python
# create_metadata_transfer_job method definition

await def create_metadata_transfer_job(
    self,
    *,
    sources: Sequence[SourceConfigurationUnionTypeDef],  # (1)
    destination: DestinationConfigurationTypeDef,  # (2)
    metadataTransferJobId: str = ...,
    description: str = ...,
) -> CreateMetadataTransferJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef) [:material-code-braces: SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef) 
2. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
3. See [:material-code-braces: CreateMetadataTransferJobResponseTypeDef](./type_defs.md#createmetadatatransferjobresponsetypedef) 


```python
# create_metadata_transfer_job method usage example with argument unpacking

kwargs: CreateMetadataTransferJobRequestRequestTypeDef = {  # (1)
    "sources": ...,
    "destination": ...,
}

parent.create_metadata_transfer_job(**kwargs)
```

1. See [:material-code-braces: CreateMetadataTransferJobRequestRequestTypeDef](./type_defs.md#createmetadatatransferjobrequestrequesttypedef) 

### create\_scene

Creates a scene.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").create_scene` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/create_scene.html)

```python
# create_scene method definition

await def create_scene(
    self,
    *,
    workspaceId: str,
    sceneId: str,
    contentLocation: str,
    description: str = ...,
    capabilities: Sequence[str] = ...,
    tags: Mapping[str, str] = ...,
    sceneMetadata: Mapping[str, str] = ...,
) -> CreateSceneResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSceneResponseTypeDef](./type_defs.md#createsceneresponsetypedef) 


```python
# create_scene method usage example with argument unpacking

kwargs: CreateSceneRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "sceneId": ...,
    "contentLocation": ...,
}

parent.create_scene(**kwargs)
```

1. See [:material-code-braces: CreateSceneRequestRequestTypeDef](./type_defs.md#createscenerequestrequesttypedef) 

### create\_sync\_job

This action creates a SyncJob.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").create_sync_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/create_sync_job.html)

```python
# create_sync_job method definition

await def create_sync_job(
    self,
    *,
    workspaceId: str,
    syncSource: str,
    syncRole: str,
    tags: Mapping[str, str] = ...,
) -> CreateSyncJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSyncJobResponseTypeDef](./type_defs.md#createsyncjobresponsetypedef) 


```python
# create_sync_job method usage example with argument unpacking

kwargs: CreateSyncJobRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "syncSource": ...,
    "syncRole": ...,
}

parent.create_sync_job(**kwargs)
```

1. See [:material-code-braces: CreateSyncJobRequestRequestTypeDef](./type_defs.md#createsyncjobrequestrequesttypedef) 

### create\_workspace

Creates a workplace.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").create_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/create_workspace.html)

```python
# create_workspace method definition

await def create_workspace(
    self,
    *,
    workspaceId: str,
    description: str = ...,
    s3Location: str = ...,
    role: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateWorkspaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateWorkspaceResponseTypeDef](./type_defs.md#createworkspaceresponsetypedef) 


```python
# create_workspace method usage example with argument unpacking

kwargs: CreateWorkspaceRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.create_workspace(**kwargs)
```

1. See [:material-code-braces: CreateWorkspaceRequestRequestTypeDef](./type_defs.md#createworkspacerequestrequesttypedef) 

### delete\_component\_type

Deletes a component type.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").delete_component_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/delete_component_type.html)

```python
# delete_component_type method definition

await def delete_component_type(
    self,
    *,
    workspaceId: str,
    componentTypeId: str,
) -> DeleteComponentTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteComponentTypeResponseTypeDef](./type_defs.md#deletecomponenttyperesponsetypedef) 


```python
# delete_component_type method usage example with argument unpacking

kwargs: DeleteComponentTypeRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "componentTypeId": ...,
}

parent.delete_component_type(**kwargs)
```

1. See [:material-code-braces: DeleteComponentTypeRequestRequestTypeDef](./type_defs.md#deletecomponenttyperequestrequesttypedef) 

### delete\_entity

Deletes an entity.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").delete_entity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/delete_entity.html)

```python
# delete_entity method definition

await def delete_entity(
    self,
    *,
    workspaceId: str,
    entityId: str,
    isRecursive: bool = ...,
) -> DeleteEntityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteEntityResponseTypeDef](./type_defs.md#deleteentityresponsetypedef) 


```python
# delete_entity method usage example with argument unpacking

kwargs: DeleteEntityRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "entityId": ...,
}

parent.delete_entity(**kwargs)
```

1. See [:material-code-braces: DeleteEntityRequestRequestTypeDef](./type_defs.md#deleteentityrequestrequesttypedef) 

### delete\_scene

Deletes a scene.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").delete_scene` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/delete_scene.html)

```python
# delete_scene method definition

await def delete_scene(
    self,
    *,
    workspaceId: str,
    sceneId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_scene method usage example with argument unpacking

kwargs: DeleteSceneRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "sceneId": ...,
}

parent.delete_scene(**kwargs)
```

1. See [:material-code-braces: DeleteSceneRequestRequestTypeDef](./type_defs.md#deletescenerequestrequesttypedef) 

### delete\_sync\_job

Delete the SyncJob.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").delete_sync_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/delete_sync_job.html)

```python
# delete_sync_job method definition

await def delete_sync_job(
    self,
    *,
    workspaceId: str,
    syncSource: str,
) -> DeleteSyncJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSyncJobResponseTypeDef](./type_defs.md#deletesyncjobresponsetypedef) 


```python
# delete_sync_job method usage example with argument unpacking

kwargs: DeleteSyncJobRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "syncSource": ...,
}

parent.delete_sync_job(**kwargs)
```

1. See [:material-code-braces: DeleteSyncJobRequestRequestTypeDef](./type_defs.md#deletesyncjobrequestrequesttypedef) 

### delete\_workspace

Deletes a workspace.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").delete_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/delete_workspace.html)

```python
# delete_workspace method definition

await def delete_workspace(
    self,
    *,
    workspaceId: str,
) -> DeleteWorkspaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteWorkspaceResponseTypeDef](./type_defs.md#deleteworkspaceresponsetypedef) 


```python
# delete_workspace method usage example with argument unpacking

kwargs: DeleteWorkspaceRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.delete_workspace(**kwargs)
```

1. See [:material-code-braces: DeleteWorkspaceRequestRequestTypeDef](./type_defs.md#deleteworkspacerequestrequesttypedef) 

### execute\_query

Run queries to access information from your knowledge graph of entities within
individual workspaces.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").execute_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/execute_query.html)

```python
# execute_query method definition

await def execute_query(
    self,
    *,
    workspaceId: str,
    queryStatement: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ExecuteQueryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExecuteQueryResponseTypeDef](./type_defs.md#executequeryresponsetypedef) 


```python
# execute_query method usage example with argument unpacking

kwargs: ExecuteQueryRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "queryStatement": ...,
}

parent.execute_query(**kwargs)
```

1. See [:material-code-braces: ExecuteQueryRequestRequestTypeDef](./type_defs.md#executequeryrequestrequesttypedef) 

### get\_component\_type

Retrieves information about a component type.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").get_component_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/get_component_type.html)

```python
# get_component_type method definition

await def get_component_type(
    self,
    *,
    workspaceId: str,
    componentTypeId: str,
) -> GetComponentTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetComponentTypeResponseTypeDef](./type_defs.md#getcomponenttyperesponsetypedef) 


```python
# get_component_type method usage example with argument unpacking

kwargs: GetComponentTypeRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "componentTypeId": ...,
}

parent.get_component_type(**kwargs)
```

1. See [:material-code-braces: GetComponentTypeRequestRequestTypeDef](./type_defs.md#getcomponenttyperequestrequesttypedef) 

### get\_entity

Retrieves information about an entity.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").get_entity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/get_entity.html)

```python
# get_entity method definition

await def get_entity(
    self,
    *,
    workspaceId: str,
    entityId: str,
) -> GetEntityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEntityResponseTypeDef](./type_defs.md#getentityresponsetypedef) 


```python
# get_entity method usage example with argument unpacking

kwargs: GetEntityRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "entityId": ...,
}

parent.get_entity(**kwargs)
```

1. See [:material-code-braces: GetEntityRequestRequestTypeDef](./type_defs.md#getentityrequestrequesttypedef) 

### get\_metadata\_transfer\_job

Gets a nmetadata transfer job.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").get_metadata_transfer_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/get_metadata_transfer_job.html)

```python
# get_metadata_transfer_job method definition

await def get_metadata_transfer_job(
    self,
    *,
    metadataTransferJobId: str,
) -> GetMetadataTransferJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMetadataTransferJobResponseTypeDef](./type_defs.md#getmetadatatransferjobresponsetypedef) 


```python
# get_metadata_transfer_job method usage example with argument unpacking

kwargs: GetMetadataTransferJobRequestRequestTypeDef = {  # (1)
    "metadataTransferJobId": ...,
}

parent.get_metadata_transfer_job(**kwargs)
```

1. See [:material-code-braces: GetMetadataTransferJobRequestRequestTypeDef](./type_defs.md#getmetadatatransferjobrequestrequesttypedef) 

### get\_pricing\_plan

Gets the pricing plan.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").get_pricing_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/get_pricing_plan.html)

```python
# get_pricing_plan method definition

await def get_pricing_plan(
    self,
) -> GetPricingPlanResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPricingPlanResponseTypeDef](./type_defs.md#getpricingplanresponsetypedef) 

### get\_property\_value

Gets the property values for a component, component type, entity, or workspace.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").get_property_value` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/get_property_value.html)

```python
# get_property_value method definition

await def get_property_value(
    self,
    *,
    selectedProperties: Sequence[str],
    workspaceId: str,
    componentName: str = ...,
    componentPath: str = ...,
    componentTypeId: str = ...,
    entityId: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    propertyGroupName: str = ...,
    tabularConditions: TabularConditionsTypeDef = ...,  # (1)
) -> GetPropertyValueResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TabularConditionsTypeDef](./type_defs.md#tabularconditionstypedef) 
2. See [:material-code-braces: GetPropertyValueResponseTypeDef](./type_defs.md#getpropertyvalueresponsetypedef) 


```python
# get_property_value method usage example with argument unpacking

kwargs: GetPropertyValueRequestRequestTypeDef = {  # (1)
    "selectedProperties": ...,
    "workspaceId": ...,
}

parent.get_property_value(**kwargs)
```

1. See [:material-code-braces: GetPropertyValueRequestRequestTypeDef](./type_defs.md#getpropertyvaluerequestrequesttypedef) 

### get\_property\_value\_history

Retrieves information about the history of a time series property value for a
component, component type, entity, or workspace.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").get_property_value_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/get_property_value_history.html)

```python
# get_property_value_history method definition

await def get_property_value_history(
    self,
    *,
    workspaceId: str,
    selectedProperties: Sequence[str],
    entityId: str = ...,
    componentName: str = ...,
    componentPath: str = ...,
    componentTypeId: str = ...,
    propertyFilters: Sequence[PropertyFilterTypeDef] = ...,  # (1)
    startDateTime: TimestampTypeDef = ...,
    endDateTime: TimestampTypeDef = ...,
    interpolation: InterpolationParametersTypeDef = ...,  # (2)
    nextToken: str = ...,
    maxResults: int = ...,
    orderByTime: OrderByTimeType = ...,  # (3)
    startTime: str = ...,
    endTime: str = ...,
) -> GetPropertyValueHistoryResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: PropertyFilterTypeDef](./type_defs.md#propertyfiltertypedef) 
2. See [:material-code-braces: InterpolationParametersTypeDef](./type_defs.md#interpolationparameterstypedef) 
3. See [:material-code-brackets: OrderByTimeType](./literals.md#orderbytimetype) 
4. See [:material-code-braces: GetPropertyValueHistoryResponseTypeDef](./type_defs.md#getpropertyvaluehistoryresponsetypedef) 


```python
# get_property_value_history method usage example with argument unpacking

kwargs: GetPropertyValueHistoryRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "selectedProperties": ...,
}

parent.get_property_value_history(**kwargs)
```

1. See [:material-code-braces: GetPropertyValueHistoryRequestRequestTypeDef](./type_defs.md#getpropertyvaluehistoryrequestrequesttypedef) 

### get\_scene

Retrieves information about a scene.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").get_scene` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/get_scene.html)

```python
# get_scene method definition

await def get_scene(
    self,
    *,
    workspaceId: str,
    sceneId: str,
) -> GetSceneResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSceneResponseTypeDef](./type_defs.md#getsceneresponsetypedef) 


```python
# get_scene method usage example with argument unpacking

kwargs: GetSceneRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "sceneId": ...,
}

parent.get_scene(**kwargs)
```

1. See [:material-code-braces: GetSceneRequestRequestTypeDef](./type_defs.md#getscenerequestrequesttypedef) 

### get\_sync\_job

Gets the SyncJob.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").get_sync_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/get_sync_job.html)

```python
# get_sync_job method definition

await def get_sync_job(
    self,
    *,
    syncSource: str,
    workspaceId: str = ...,
) -> GetSyncJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSyncJobResponseTypeDef](./type_defs.md#getsyncjobresponsetypedef) 


```python
# get_sync_job method usage example with argument unpacking

kwargs: GetSyncJobRequestRequestTypeDef = {  # (1)
    "syncSource": ...,
}

parent.get_sync_job(**kwargs)
```

1. See [:material-code-braces: GetSyncJobRequestRequestTypeDef](./type_defs.md#getsyncjobrequestrequesttypedef) 

### get\_workspace

Retrieves information about a workspace.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").get_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/get_workspace.html)

```python
# get_workspace method definition

await def get_workspace(
    self,
    *,
    workspaceId: str,
) -> GetWorkspaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkspaceResponseTypeDef](./type_defs.md#getworkspaceresponsetypedef) 


```python
# get_workspace method usage example with argument unpacking

kwargs: GetWorkspaceRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.get_workspace(**kwargs)
```

1. See [:material-code-braces: GetWorkspaceRequestRequestTypeDef](./type_defs.md#getworkspacerequestrequesttypedef) 

### list\_component\_types

Lists all component types in a workspace.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").list_component_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/list_component_types.html)

```python
# list_component_types method definition

await def list_component_types(
    self,
    *,
    workspaceId: str,
    filters: Sequence[ListComponentTypesFilterTypeDef] = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListComponentTypesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListComponentTypesFilterTypeDef](./type_defs.md#listcomponenttypesfiltertypedef) 
2. See [:material-code-braces: ListComponentTypesResponseTypeDef](./type_defs.md#listcomponenttypesresponsetypedef) 


```python
# list_component_types method usage example with argument unpacking

kwargs: ListComponentTypesRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.list_component_types(**kwargs)
```

1. See [:material-code-braces: ListComponentTypesRequestRequestTypeDef](./type_defs.md#listcomponenttypesrequestrequesttypedef) 

### list\_components

This API lists the components of an entity.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").list_components` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/list_components.html)

```python
# list_components method definition

await def list_components(
    self,
    *,
    workspaceId: str,
    entityId: str,
    componentPath: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListComponentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


```python
# list_components method usage example with argument unpacking

kwargs: ListComponentsRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "entityId": ...,
}

parent.list_components(**kwargs)
```

1. See [:material-code-braces: ListComponentsRequestRequestTypeDef](./type_defs.md#listcomponentsrequestrequesttypedef) 

### list\_entities

Lists all entities in a workspace.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").list_entities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/list_entities.html)

```python
# list_entities method definition

await def list_entities(
    self,
    *,
    workspaceId: str,
    filters: Sequence[ListEntitiesFilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListEntitiesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListEntitiesFilterTypeDef](./type_defs.md#listentitiesfiltertypedef) 
2. See [:material-code-braces: ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef) 


```python
# list_entities method usage example with argument unpacking

kwargs: ListEntitiesRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.list_entities(**kwargs)
```

1. See [:material-code-braces: ListEntitiesRequestRequestTypeDef](./type_defs.md#listentitiesrequestrequesttypedef) 

### list\_metadata\_transfer\_jobs

Lists the metadata transfer jobs.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").list_metadata_transfer_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/list_metadata_transfer_jobs.html)

```python
# list_metadata_transfer_jobs method definition

await def list_metadata_transfer_jobs(
    self,
    *,
    sourceType: SourceTypeType,  # (1)
    destinationType: DestinationTypeType,  # (2)
    filters: Sequence[ListMetadataTransferJobsFilterTypeDef] = ...,  # (3)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListMetadataTransferJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-brackets: DestinationTypeType](./literals.md#destinationtypetype) 
3. See [:material-code-braces: ListMetadataTransferJobsFilterTypeDef](./type_defs.md#listmetadatatransferjobsfiltertypedef) 
4. See [:material-code-braces: ListMetadataTransferJobsResponseTypeDef](./type_defs.md#listmetadatatransferjobsresponsetypedef) 


```python
# list_metadata_transfer_jobs method usage example with argument unpacking

kwargs: ListMetadataTransferJobsRequestRequestTypeDef = {  # (1)
    "sourceType": ...,
    "destinationType": ...,
}

parent.list_metadata_transfer_jobs(**kwargs)
```

1. See [:material-code-braces: ListMetadataTransferJobsRequestRequestTypeDef](./type_defs.md#listmetadatatransferjobsrequestrequesttypedef) 

### list\_properties

This API lists the properties of a component.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").list_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/list_properties.html)

```python
# list_properties method definition

await def list_properties(
    self,
    *,
    workspaceId: str,
    entityId: str,
    componentName: str = ...,
    componentPath: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListPropertiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPropertiesResponseTypeDef](./type_defs.md#listpropertiesresponsetypedef) 


```python
# list_properties method usage example with argument unpacking

kwargs: ListPropertiesRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "entityId": ...,
}

parent.list_properties(**kwargs)
```

1. See [:material-code-braces: ListPropertiesRequestRequestTypeDef](./type_defs.md#listpropertiesrequestrequesttypedef) 

### list\_scenes

Lists all scenes in a workspace.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").list_scenes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/list_scenes.html)

```python
# list_scenes method definition

await def list_scenes(
    self,
    *,
    workspaceId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListScenesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListScenesResponseTypeDef](./type_defs.md#listscenesresponsetypedef) 


```python
# list_scenes method usage example with argument unpacking

kwargs: ListScenesRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.list_scenes(**kwargs)
```

1. See [:material-code-braces: ListScenesRequestRequestTypeDef](./type_defs.md#listscenesrequestrequesttypedef) 

### list\_sync\_jobs

List all SyncJobs.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").list_sync_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/list_sync_jobs.html)

```python
# list_sync_jobs method definition

await def list_sync_jobs(
    self,
    *,
    workspaceId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSyncJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSyncJobsResponseTypeDef](./type_defs.md#listsyncjobsresponsetypedef) 


```python
# list_sync_jobs method usage example with argument unpacking

kwargs: ListSyncJobsRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.list_sync_jobs(**kwargs)
```

1. See [:material-code-braces: ListSyncJobsRequestRequestTypeDef](./type_defs.md#listsyncjobsrequestrequesttypedef) 

### list\_sync\_resources

Lists the sync resources.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").list_sync_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/list_sync_resources.html)

```python
# list_sync_resources method definition

await def list_sync_resources(
    self,
    *,
    workspaceId: str,
    syncSource: str,
    filters: Sequence[SyncResourceFilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSyncResourcesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SyncResourceFilterTypeDef](./type_defs.md#syncresourcefiltertypedef) 
2. See [:material-code-braces: ListSyncResourcesResponseTypeDef](./type_defs.md#listsyncresourcesresponsetypedef) 


```python
# list_sync_resources method usage example with argument unpacking

kwargs: ListSyncResourcesRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "syncSource": ...,
}

parent.list_sync_resources(**kwargs)
```

1. See [:material-code-braces: ListSyncResourcesRequestRequestTypeDef](./type_defs.md#listsyncresourcesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists all tags associated with a resource.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceARN: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_workspaces

Retrieves information about workspaces in the current account.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").list_workspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/list_workspaces.html)

```python
# list_workspaces method definition

await def list_workspaces(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkspacesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef) 


```python
# list_workspaces method usage example with argument unpacking

kwargs: ListWorkspacesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_workspaces(**kwargs)
```

1. See [:material-code-braces: ListWorkspacesRequestRequestTypeDef](./type_defs.md#listworkspacesrequestrequesttypedef) 

### tag\_resource

Adds tags to a resource.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceARN: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from a resource.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceARN: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_component\_type

Updates information in a component type.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").update_component_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/update_component_type.html)

```python
# update_component_type method definition

await def update_component_type(
    self,
    *,
    workspaceId: str,
    componentTypeId: str,
    isSingleton: bool = ...,
    description: str = ...,
    propertyDefinitions: Mapping[str, PropertyDefinitionRequestTypeDef] = ...,  # (1)
    extendsFrom: Sequence[str] = ...,
    functions: Mapping[str, FunctionRequestTypeDef] = ...,  # (2)
    propertyGroups: Mapping[str, PropertyGroupRequestTypeDef] = ...,  # (3)
    componentTypeName: str = ...,
    compositeComponentTypes: Mapping[str, CompositeComponentTypeRequestTypeDef] = ...,  # (4)
) -> UpdateComponentTypeResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: PropertyDefinitionRequestTypeDef](./type_defs.md#propertydefinitionrequesttypedef) 
2. See [:material-code-braces: FunctionRequestTypeDef](./type_defs.md#functionrequesttypedef) 
3. See [:material-code-braces: PropertyGroupRequestTypeDef](./type_defs.md#propertygrouprequesttypedef) 
4. See [:material-code-braces: CompositeComponentTypeRequestTypeDef](./type_defs.md#compositecomponenttyperequesttypedef) 
5. See [:material-code-braces: UpdateComponentTypeResponseTypeDef](./type_defs.md#updatecomponenttyperesponsetypedef) 


```python
# update_component_type method usage example with argument unpacking

kwargs: UpdateComponentTypeRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "componentTypeId": ...,
}

parent.update_component_type(**kwargs)
```

1. See [:material-code-braces: UpdateComponentTypeRequestRequestTypeDef](./type_defs.md#updatecomponenttyperequestrequesttypedef) 

### update\_entity

Updates an entity.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").update_entity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/update_entity.html)

```python
# update_entity method definition

await def update_entity(
    self,
    *,
    workspaceId: str,
    entityId: str,
    entityName: str = ...,
    description: str = ...,
    componentUpdates: Mapping[str, ComponentUpdateRequestTypeDef] = ...,  # (1)
    compositeComponentUpdates: Mapping[str, CompositeComponentUpdateRequestTypeDef] = ...,  # (2)
    parentEntityUpdate: ParentEntityUpdateRequestTypeDef = ...,  # (3)
) -> UpdateEntityResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ComponentUpdateRequestTypeDef](./type_defs.md#componentupdaterequesttypedef) 
2. See [:material-code-braces: CompositeComponentUpdateRequestTypeDef](./type_defs.md#compositecomponentupdaterequesttypedef) 
3. See [:material-code-braces: ParentEntityUpdateRequestTypeDef](./type_defs.md#parententityupdaterequesttypedef) 
4. See [:material-code-braces: UpdateEntityResponseTypeDef](./type_defs.md#updateentityresponsetypedef) 


```python
# update_entity method usage example with argument unpacking

kwargs: UpdateEntityRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "entityId": ...,
}

parent.update_entity(**kwargs)
```

1. See [:material-code-braces: UpdateEntityRequestRequestTypeDef](./type_defs.md#updateentityrequestrequesttypedef) 

### update\_pricing\_plan

Update the pricing plan.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").update_pricing_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/update_pricing_plan.html)

```python
# update_pricing_plan method definition

await def update_pricing_plan(
    self,
    *,
    pricingMode: PricingModeType,  # (1)
    bundleNames: Sequence[str] = ...,
) -> UpdatePricingPlanResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PricingModeType](./literals.md#pricingmodetype) 
2. See [:material-code-braces: UpdatePricingPlanResponseTypeDef](./type_defs.md#updatepricingplanresponsetypedef) 


```python
# update_pricing_plan method usage example with argument unpacking

kwargs: UpdatePricingPlanRequestRequestTypeDef = {  # (1)
    "pricingMode": ...,
}

parent.update_pricing_plan(**kwargs)
```

1. See [:material-code-braces: UpdatePricingPlanRequestRequestTypeDef](./type_defs.md#updatepricingplanrequestrequesttypedef) 

### update\_scene

Updates a scene.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").update_scene` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/update_scene.html)

```python
# update_scene method definition

await def update_scene(
    self,
    *,
    workspaceId: str,
    sceneId: str,
    contentLocation: str = ...,
    description: str = ...,
    capabilities: Sequence[str] = ...,
    sceneMetadata: Mapping[str, str] = ...,
) -> UpdateSceneResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateSceneResponseTypeDef](./type_defs.md#updatesceneresponsetypedef) 


```python
# update_scene method usage example with argument unpacking

kwargs: UpdateSceneRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
    "sceneId": ...,
}

parent.update_scene(**kwargs)
```

1. See [:material-code-braces: UpdateSceneRequestRequestTypeDef](./type_defs.md#updatescenerequestrequesttypedef) 

### update\_workspace

Updates a workspace.

Type annotations and code completion for `#!python session.create_client("iottwinmaker").update_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker/client/update_workspace.html)

```python
# update_workspace method definition

await def update_workspace(
    self,
    *,
    workspaceId: str,
    description: str = ...,
    role: str = ...,
    s3Location: str = ...,
) -> UpdateWorkspaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateWorkspaceResponseTypeDef](./type_defs.md#updateworkspaceresponsetypedef) 


```python
# update_workspace method usage example with argument unpacking

kwargs: UpdateWorkspaceRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.update_workspace(**kwargs)
```

1. See [:material-code-braces: UpdateWorkspaceRequestRequestTypeDef](./type_defs.md#updateworkspacerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("iottwinmaker").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "IoTTwinMakerClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("iottwinmaker").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client)

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





