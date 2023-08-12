# AppflowClient

> [Index](../README.md) > [Appflow](./README.md) > AppflowClient

!!! note ""

    Auto-generated documentation for [Appflow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
    type annotations stubs module [types-aiobotocore-appflow](https://pypi.org/project/types-aiobotocore-appflow/).

## AppflowClient

Type annotations and code completion for `#!python session.create_client("appflow")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client)

```python
AppflowClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_appflow.client import AppflowClient

session = get_session()
async with session.create_client("appflow") as client:
    client: AppflowClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("appflow").exceptions` structure.

```python
AppflowClient.exceptions usage example

async with session.create_client("appflow") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.ConnectorAuthenticationException,
        client.ConnectorServerException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.UnsupportedOperationException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
AppflowClient usage type checking example

from types_aiobotocore_appflow.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("appflow").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_flow\_executions

Cancels active runs for a flow.

Type annotations and code completion for `#!python session.create_client("appflow").cancel_flow_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.cancel_flow_executions)

```python
# cancel_flow_executions method definition

await def cancel_flow_executions(
    self,
    *,
    flowName: str,
    executionIds: Sequence[str] = ...,
) -> CancelFlowExecutionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelFlowExecutionsResponseTypeDef](./type_defs.md#cancelflowexecutionsresponsetypedef) 


```python
# cancel_flow_executions method usage example with argument unpacking

kwargs: CancelFlowExecutionsRequestRequestTypeDef = {  # (1)
    "flowName": ...,
}

parent.cancel_flow_executions(**kwargs)
```

1. See [:material-code-braces: CancelFlowExecutionsRequestRequestTypeDef](./type_defs.md#cancelflowexecutionsrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("appflow").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_connector\_profile

Creates a new connector profile associated with your Amazon Web Services
account.

Type annotations and code completion for `#!python session.create_client("appflow").create_connector_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_connector_profile)

```python
# create_connector_profile method definition

await def create_connector_profile(
    self,
    *,
    connectorProfileName: str,
    connectorType: ConnectorTypeType,  # (1)
    connectionMode: ConnectionModeType,  # (2)
    connectorProfileConfig: ConnectorProfileConfigTypeDef,  # (3)
    kmsArn: str = ...,
    connectorLabel: str = ...,
    clientToken: str = ...,
) -> CreateConnectorProfileResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ConnectorTypeType](./literals.md#connectortypetype) 
2. See [:material-code-brackets: ConnectionModeType](./literals.md#connectionmodetype) 
3. See [:material-code-braces: ConnectorProfileConfigTypeDef](./type_defs.md#connectorprofileconfigtypedef) 
4. See [:material-code-braces: CreateConnectorProfileResponseTypeDef](./type_defs.md#createconnectorprofileresponsetypedef) 


```python
# create_connector_profile method usage example with argument unpacking

kwargs: CreateConnectorProfileRequestRequestTypeDef = {  # (1)
    "connectorProfileName": ...,
    "connectorType": ...,
    "connectionMode": ...,
    "connectorProfileConfig": ...,
}

parent.create_connector_profile(**kwargs)
```

1. See [:material-code-braces: CreateConnectorProfileRequestRequestTypeDef](./type_defs.md#createconnectorprofilerequestrequesttypedef) 

### create\_flow

Enables your application to create a new flow using Amazon AppFlow.

Type annotations and code completion for `#!python session.create_client("appflow").create_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_flow)

```python
# create_flow method definition

await def create_flow(
    self,
    *,
    flowName: str,
    triggerConfig: TriggerConfigTypeDef,  # (1)
    sourceFlowConfig: SourceFlowConfigTypeDef,  # (2)
    destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],  # (3)
    tasks: Sequence[TaskTypeDef],  # (4)
    description: str = ...,
    kmsArn: str = ...,
    tags: Mapping[str, str] = ...,
    metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,  # (5)
    clientToken: str = ...,
) -> CreateFlowResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: TriggerConfigTypeDef](./type_defs.md#triggerconfigtypedef) 
2. See [:material-code-braces: SourceFlowConfigTypeDef](./type_defs.md#sourceflowconfigtypedef) 
3. See [:material-code-braces: DestinationFlowConfigTypeDef](./type_defs.md#destinationflowconfigtypedef) 
4. See [:material-code-braces: TaskTypeDef](./type_defs.md#tasktypedef) 
5. See [:material-code-braces: MetadataCatalogConfigTypeDef](./type_defs.md#metadatacatalogconfigtypedef) 
6. See [:material-code-braces: CreateFlowResponseTypeDef](./type_defs.md#createflowresponsetypedef) 


```python
# create_flow method usage example with argument unpacking

kwargs: CreateFlowRequestRequestTypeDef = {  # (1)
    "flowName": ...,
    "triggerConfig": ...,
    "sourceFlowConfig": ...,
    "destinationFlowConfigList": ...,
    "tasks": ...,
}

parent.create_flow(**kwargs)
```

1. See [:material-code-braces: CreateFlowRequestRequestTypeDef](./type_defs.md#createflowrequestrequesttypedef) 

### delete\_connector\_profile

Enables you to delete an existing connector profile.

Type annotations and code completion for `#!python session.create_client("appflow").delete_connector_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_connector_profile)

```python
# delete_connector_profile method definition

await def delete_connector_profile(
    self,
    *,
    connectorProfileName: str,
    forceDelete: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_connector_profile method usage example with argument unpacking

kwargs: DeleteConnectorProfileRequestRequestTypeDef = {  # (1)
    "connectorProfileName": ...,
}

parent.delete_connector_profile(**kwargs)
```

1. See [:material-code-braces: DeleteConnectorProfileRequestRequestTypeDef](./type_defs.md#deleteconnectorprofilerequestrequesttypedef) 

### delete\_flow

Enables your application to delete an existing flow.

Type annotations and code completion for `#!python session.create_client("appflow").delete_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_flow)

```python
# delete_flow method definition

await def delete_flow(
    self,
    *,
    flowName: str,
    forceDelete: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_flow method usage example with argument unpacking

kwargs: DeleteFlowRequestRequestTypeDef = {  # (1)
    "flowName": ...,
}

parent.delete_flow(**kwargs)
```

1. See [:material-code-braces: DeleteFlowRequestRequestTypeDef](./type_defs.md#deleteflowrequestrequesttypedef) 

### describe\_connector

Describes the given custom connector registered in your Amazon Web Services
account.

Type annotations and code completion for `#!python session.create_client("appflow").describe_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector)

```python
# describe_connector method definition

await def describe_connector(
    self,
    *,
    connectorType: ConnectorTypeType,  # (1)
    connectorLabel: str = ...,
) -> DescribeConnectorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConnectorTypeType](./literals.md#connectortypetype) 
2. See [:material-code-braces: DescribeConnectorResponseTypeDef](./type_defs.md#describeconnectorresponsetypedef) 


```python
# describe_connector method usage example with argument unpacking

kwargs: DescribeConnectorRequestRequestTypeDef = {  # (1)
    "connectorType": ...,
}

parent.describe_connector(**kwargs)
```

1. See [:material-code-braces: DescribeConnectorRequestRequestTypeDef](./type_defs.md#describeconnectorrequestrequesttypedef) 

### describe\_connector\_entity

Provides details regarding the entity used with the connector, with a
description of the data model for each field in that entity.

Type annotations and code completion for `#!python session.create_client("appflow").describe_connector_entity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_entity)

```python
# describe_connector_entity method definition

await def describe_connector_entity(
    self,
    *,
    connectorEntityName: str,
    connectorType: ConnectorTypeType = ...,  # (1)
    connectorProfileName: str = ...,
    apiVersion: str = ...,
) -> DescribeConnectorEntityResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConnectorTypeType](./literals.md#connectortypetype) 
2. See [:material-code-braces: DescribeConnectorEntityResponseTypeDef](./type_defs.md#describeconnectorentityresponsetypedef) 


```python
# describe_connector_entity method usage example with argument unpacking

kwargs: DescribeConnectorEntityRequestRequestTypeDef = {  # (1)
    "connectorEntityName": ...,
}

parent.describe_connector_entity(**kwargs)
```

1. See [:material-code-braces: DescribeConnectorEntityRequestRequestTypeDef](./type_defs.md#describeconnectorentityrequestrequesttypedef) 

### describe\_connector\_profiles

Returns a list of `connector-profile` details matching the provided `connector-
profile` names and `connector-types`.

Type annotations and code completion for `#!python session.create_client("appflow").describe_connector_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_profiles)

```python
# describe_connector_profiles method definition

await def describe_connector_profiles(
    self,
    *,
    connectorProfileNames: Sequence[str] = ...,
    connectorType: ConnectorTypeType = ...,  # (1)
    connectorLabel: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeConnectorProfilesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConnectorTypeType](./literals.md#connectortypetype) 
2. See [:material-code-braces: DescribeConnectorProfilesResponseTypeDef](./type_defs.md#describeconnectorprofilesresponsetypedef) 


```python
# describe_connector_profiles method usage example with argument unpacking

kwargs: DescribeConnectorProfilesRequestRequestTypeDef = {  # (1)
    "connectorProfileNames": ...,
}

parent.describe_connector_profiles(**kwargs)
```

1. See [:material-code-braces: DescribeConnectorProfilesRequestRequestTypeDef](./type_defs.md#describeconnectorprofilesrequestrequesttypedef) 

### describe\_connectors

Describes the connectors vended by Amazon AppFlow for specified connector types.

Type annotations and code completion for `#!python session.create_client("appflow").describe_connectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connectors)

```python
# describe_connectors method definition

await def describe_connectors(
    self,
    *,
    connectorTypes: Sequence[ConnectorTypeType] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeConnectorsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConnectorTypeType](./literals.md#connectortypetype) 
2. See [:material-code-braces: DescribeConnectorsResponseTypeDef](./type_defs.md#describeconnectorsresponsetypedef) 


```python
# describe_connectors method usage example with argument unpacking

kwargs: DescribeConnectorsRequestRequestTypeDef = {  # (1)
    "connectorTypes": ...,
}

parent.describe_connectors(**kwargs)
```

1. See [:material-code-braces: DescribeConnectorsRequestRequestTypeDef](./type_defs.md#describeconnectorsrequestrequesttypedef) 

### describe\_flow

Provides a description of the specified flow.

Type annotations and code completion for `#!python session.create_client("appflow").describe_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow)

```python
# describe_flow method definition

await def describe_flow(
    self,
    *,
    flowName: str,
) -> DescribeFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFlowResponseTypeDef](./type_defs.md#describeflowresponsetypedef) 


```python
# describe_flow method usage example with argument unpacking

kwargs: DescribeFlowRequestRequestTypeDef = {  # (1)
    "flowName": ...,
}

parent.describe_flow(**kwargs)
```

1. See [:material-code-braces: DescribeFlowRequestRequestTypeDef](./type_defs.md#describeflowrequestrequesttypedef) 

### describe\_flow\_execution\_records

Fetches the execution history of the flow.

Type annotations and code completion for `#!python session.create_client("appflow").describe_flow_execution_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow_execution_records)

```python
# describe_flow_execution_records method definition

await def describe_flow_execution_records(
    self,
    *,
    flowName: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeFlowExecutionRecordsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFlowExecutionRecordsResponseTypeDef](./type_defs.md#describeflowexecutionrecordsresponsetypedef) 


```python
# describe_flow_execution_records method usage example with argument unpacking

kwargs: DescribeFlowExecutionRecordsRequestRequestTypeDef = {  # (1)
    "flowName": ...,
}

parent.describe_flow_execution_records(**kwargs)
```

1. See [:material-code-braces: DescribeFlowExecutionRecordsRequestRequestTypeDef](./type_defs.md#describeflowexecutionrecordsrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("appflow").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.generate_presigned_url)

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


### list\_connector\_entities

Returns the list of available connector entities supported by Amazon AppFlow.

Type annotations and code completion for `#!python session.create_client("appflow").list_connector_entities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connector_entities)

```python
# list_connector_entities method definition

await def list_connector_entities(
    self,
    *,
    connectorProfileName: str = ...,
    connectorType: ConnectorTypeType = ...,  # (1)
    entitiesPath: str = ...,
    apiVersion: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListConnectorEntitiesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConnectorTypeType](./literals.md#connectortypetype) 
2. See [:material-code-braces: ListConnectorEntitiesResponseTypeDef](./type_defs.md#listconnectorentitiesresponsetypedef) 


```python
# list_connector_entities method usage example with argument unpacking

kwargs: ListConnectorEntitiesRequestRequestTypeDef = {  # (1)
    "connectorProfileName": ...,
}

parent.list_connector_entities(**kwargs)
```

1. See [:material-code-braces: ListConnectorEntitiesRequestRequestTypeDef](./type_defs.md#listconnectorentitiesrequestrequesttypedef) 

### list\_connectors

Returns the list of all registered custom connectors in your Amazon Web Services
account.

Type annotations and code completion for `#!python session.create_client("appflow").list_connectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connectors)

```python
# list_connectors method definition

await def list_connectors(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListConnectorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


```python
# list_connectors method usage example with argument unpacking

kwargs: ListConnectorsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_connectors(**kwargs)
```

1. See [:material-code-braces: ListConnectorsRequestRequestTypeDef](./type_defs.md#listconnectorsrequestrequesttypedef) 

### list\_flows

Lists all of the flows associated with your account.

Type annotations and code completion for `#!python session.create_client("appflow").list_flows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_flows)

```python
# list_flows method definition

await def list_flows(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListFlowsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFlowsResponseTypeDef](./type_defs.md#listflowsresponsetypedef) 


```python
# list_flows method usage example with argument unpacking

kwargs: ListFlowsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_flows(**kwargs)
```

1. See [:material-code-braces: ListFlowsRequestRequestTypeDef](./type_defs.md#listflowsrequestrequesttypedef) 

### list\_tags\_for\_resource

Retrieves the tags that are associated with a specified flow.

Type annotations and code completion for `#!python session.create_client("appflow").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_tags_for_resource)

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

### register\_connector

Registers a new custom connector with your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("appflow").register_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.register_connector)

```python
# register_connector method definition

await def register_connector(
    self,
    *,
    connectorLabel: str = ...,
    description: str = ...,
    connectorProvisioningType: ConnectorProvisioningTypeType = ...,  # (1)
    connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,  # (2)
    clientToken: str = ...,
) -> RegisterConnectorResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ConnectorProvisioningTypeType](./literals.md#connectorprovisioningtypetype) 
2. See [:material-code-braces: ConnectorProvisioningConfigTypeDef](./type_defs.md#connectorprovisioningconfigtypedef) 
3. See [:material-code-braces: RegisterConnectorResponseTypeDef](./type_defs.md#registerconnectorresponsetypedef) 


```python
# register_connector method usage example with argument unpacking

kwargs: RegisterConnectorRequestRequestTypeDef = {  # (1)
    "connectorLabel": ...,
}

parent.register_connector(**kwargs)
```

1. See [:material-code-braces: RegisterConnectorRequestRequestTypeDef](./type_defs.md#registerconnectorrequestrequesttypedef) 

### reset\_connector\_metadata\_cache

Resets metadata about your connector entities that Amazon AppFlow stored in its
cache.

Type annotations and code completion for `#!python session.create_client("appflow").reset_connector_metadata_cache` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.reset_connector_metadata_cache)

```python
# reset_connector_metadata_cache method definition

await def reset_connector_metadata_cache(
    self,
    *,
    connectorProfileName: str = ...,
    connectorType: ConnectorTypeType = ...,  # (1)
    connectorEntityName: str = ...,
    entitiesPath: str = ...,
    apiVersion: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ConnectorTypeType](./literals.md#connectortypetype) 


```python
# reset_connector_metadata_cache method usage example with argument unpacking

kwargs: ResetConnectorMetadataCacheRequestRequestTypeDef = {  # (1)
    "connectorProfileName": ...,
}

parent.reset_connector_metadata_cache(**kwargs)
```

1. See [:material-code-braces: ResetConnectorMetadataCacheRequestRequestTypeDef](./type_defs.md#resetconnectormetadatacacherequestrequesttypedef) 

### start\_flow

Activates an existing flow.

Type annotations and code completion for `#!python session.create_client("appflow").start_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.start_flow)

```python
# start_flow method definition

await def start_flow(
    self,
    *,
    flowName: str,
    clientToken: str = ...,
) -> StartFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartFlowResponseTypeDef](./type_defs.md#startflowresponsetypedef) 


```python
# start_flow method usage example with argument unpacking

kwargs: StartFlowRequestRequestTypeDef = {  # (1)
    "flowName": ...,
}

parent.start_flow(**kwargs)
```

1. See [:material-code-braces: StartFlowRequestRequestTypeDef](./type_defs.md#startflowrequestrequesttypedef) 

### stop\_flow

Deactivates the existing flow.

Type annotations and code completion for `#!python session.create_client("appflow").stop_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.stop_flow)

```python
# stop_flow method definition

await def stop_flow(
    self,
    *,
    flowName: str,
) -> StopFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopFlowResponseTypeDef](./type_defs.md#stopflowresponsetypedef) 


```python
# stop_flow method usage example with argument unpacking

kwargs: StopFlowRequestRequestTypeDef = {  # (1)
    "flowName": ...,
}

parent.stop_flow(**kwargs)
```

1. See [:material-code-braces: StopFlowRequestRequestTypeDef](./type_defs.md#stopflowrequestrequesttypedef) 

### tag\_resource

Applies a tag to the specified flow.

Type annotations and code completion for `#!python session.create_client("appflow").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.tag_resource)

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

### unregister\_connector

Unregisters the custom connector registered in your account that matches the
connector label provided in the request.

Type annotations and code completion for `#!python session.create_client("appflow").unregister_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.unregister_connector)

```python
# unregister_connector method definition

await def unregister_connector(
    self,
    *,
    connectorLabel: str,
    forceDelete: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# unregister_connector method usage example with argument unpacking

kwargs: UnregisterConnectorRequestRequestTypeDef = {  # (1)
    "connectorLabel": ...,
}

parent.unregister_connector(**kwargs)
```

1. See [:material-code-braces: UnregisterConnectorRequestRequestTypeDef](./type_defs.md#unregisterconnectorrequestrequesttypedef) 

### untag\_resource

Removes a tag from the specified flow.

Type annotations and code completion for `#!python session.create_client("appflow").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.untag_resource)

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

### update\_connector\_profile

Updates a given connector profile associated with your account.

Type annotations and code completion for `#!python session.create_client("appflow").update_connector_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_profile)

```python
# update_connector_profile method definition

await def update_connector_profile(
    self,
    *,
    connectorProfileName: str,
    connectionMode: ConnectionModeType,  # (1)
    connectorProfileConfig: ConnectorProfileConfigTypeDef,  # (2)
    clientToken: str = ...,
) -> UpdateConnectorProfileResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ConnectionModeType](./literals.md#connectionmodetype) 
2. See [:material-code-braces: ConnectorProfileConfigTypeDef](./type_defs.md#connectorprofileconfigtypedef) 
3. See [:material-code-braces: UpdateConnectorProfileResponseTypeDef](./type_defs.md#updateconnectorprofileresponsetypedef) 


```python
# update_connector_profile method usage example with argument unpacking

kwargs: UpdateConnectorProfileRequestRequestTypeDef = {  # (1)
    "connectorProfileName": ...,
    "connectionMode": ...,
    "connectorProfileConfig": ...,
}

parent.update_connector_profile(**kwargs)
```

1. See [:material-code-braces: UpdateConnectorProfileRequestRequestTypeDef](./type_defs.md#updateconnectorprofilerequestrequesttypedef) 

### update\_connector\_registration

Updates a custom connector that you've previously registered.

Type annotations and code completion for `#!python session.create_client("appflow").update_connector_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_registration)

```python
# update_connector_registration method definition

await def update_connector_registration(
    self,
    *,
    connectorLabel: str,
    description: str = ...,
    connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,  # (1)
    clientToken: str = ...,
) -> UpdateConnectorRegistrationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConnectorProvisioningConfigTypeDef](./type_defs.md#connectorprovisioningconfigtypedef) 
2. See [:material-code-braces: UpdateConnectorRegistrationResponseTypeDef](./type_defs.md#updateconnectorregistrationresponsetypedef) 


```python
# update_connector_registration method usage example with argument unpacking

kwargs: UpdateConnectorRegistrationRequestRequestTypeDef = {  # (1)
    "connectorLabel": ...,
}

parent.update_connector_registration(**kwargs)
```

1. See [:material-code-braces: UpdateConnectorRegistrationRequestRequestTypeDef](./type_defs.md#updateconnectorregistrationrequestrequesttypedef) 

### update\_flow

Updates an existing flow.

Type annotations and code completion for `#!python session.create_client("appflow").update_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_flow)

```python
# update_flow method definition

await def update_flow(
    self,
    *,
    flowName: str,
    triggerConfig: TriggerConfigTypeDef,  # (1)
    sourceFlowConfig: SourceFlowConfigTypeDef,  # (2)
    destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],  # (3)
    tasks: Sequence[TaskTypeDef],  # (4)
    description: str = ...,
    metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,  # (5)
    clientToken: str = ...,
) -> UpdateFlowResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: TriggerConfigTypeDef](./type_defs.md#triggerconfigtypedef) 
2. See [:material-code-braces: SourceFlowConfigTypeDef](./type_defs.md#sourceflowconfigtypedef) 
3. See [:material-code-braces: DestinationFlowConfigTypeDef](./type_defs.md#destinationflowconfigtypedef) 
4. See [:material-code-braces: TaskTypeDef](./type_defs.md#tasktypedef) 
5. See [:material-code-braces: MetadataCatalogConfigTypeDef](./type_defs.md#metadatacatalogconfigtypedef) 
6. See [:material-code-braces: UpdateFlowResponseTypeDef](./type_defs.md#updateflowresponsetypedef) 


```python
# update_flow method usage example with argument unpacking

kwargs: UpdateFlowRequestRequestTypeDef = {  # (1)
    "flowName": ...,
    "triggerConfig": ...,
    "sourceFlowConfig": ...,
    "destinationFlowConfigList": ...,
    "tasks": ...,
}

parent.update_flow(**kwargs)
```

1. See [:material-code-braces: UpdateFlowRequestRequestTypeDef](./type_defs.md#updateflowrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("appflow").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> AppflowClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("appflow").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.__aexit__)

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





