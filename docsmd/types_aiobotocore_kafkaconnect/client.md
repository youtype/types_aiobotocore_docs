# KafkaConnectClient

> [Index](../README.md) > [KafkaConnect](./README.md) > KafkaConnectClient

!!! note ""

    Auto-generated documentation for [KafkaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#kafkaconnect)
    type annotations stubs module [types-aiobotocore-kafkaconnect](https://pypi.org/project/types-aiobotocore-kafkaconnect/).

## KafkaConnectClient

Type annotations and code completion for `#!python session.create_client("kafkaconnect")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Client)

```python
# KafkaConnectClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_kafkaconnect.client import KafkaConnectClient

session = get_session()
async with session.create_client("kafkaconnect") as client:
    client: KafkaConnectClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("kafkaconnect").exceptions` structure.

```python
# KafkaConnectClient.exceptions usage example

async with session.create_client("kafkaconnect") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.ForbiddenException,
        client.InternalServerErrorException,
        client.NotFoundException,
        client.ServiceUnavailableException,
        client.TooManyRequestsException,
        client.UnauthorizedException,
    ) as e:
        print(e)
```

```python
# KafkaConnectClient usage type checking example

from types_aiobotocore_kafkaconnect.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("kafkaconnect").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("kafkaconnect").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/generate_presigned_url.html)

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



Type annotations and code completion for `#!python session.create_client("kafkaconnect").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_connector

Creates a connector using the specified properties.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").create_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/create_connector.html)

```python
# create_connector method definition

await def create_connector(
    self,
    *,
    capacity: CapacityTypeDef,  # (1)
    connectorConfiguration: Mapping[str, str],
    connectorName: str,
    kafkaCluster: KafkaClusterTypeDef,  # (2)
    kafkaClusterClientAuthentication: KafkaClusterClientAuthenticationTypeDef,  # (3)
    kafkaClusterEncryptionInTransit: KafkaClusterEncryptionInTransitTypeDef,  # (4)
    kafkaConnectVersion: str,
    plugins: Sequence[PluginTypeDef],  # (5)
    serviceExecutionRoleArn: str,
    connectorDescription: str = ...,
    logDelivery: LogDeliveryTypeDef = ...,  # (6)
    tags: Mapping[str, str] = ...,
    workerConfiguration: WorkerConfigurationTypeDef = ...,  # (7)
) -> CreateConnectorResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
2. See [:material-code-braces: KafkaClusterTypeDef](./type_defs.md#kafkaclustertypedef) 
3. See [:material-code-braces: KafkaClusterClientAuthenticationTypeDef](./type_defs.md#kafkaclusterclientauthenticationtypedef) 
4. See [:material-code-braces: KafkaClusterEncryptionInTransitTypeDef](./type_defs.md#kafkaclusterencryptionintransittypedef) 
5. See [:material-code-braces: PluginTypeDef](./type_defs.md#plugintypedef) 
6. See [:material-code-braces: LogDeliveryTypeDef](./type_defs.md#logdeliverytypedef) 
7. See [:material-code-braces: WorkerConfigurationTypeDef](./type_defs.md#workerconfigurationtypedef) 
8. See [:material-code-braces: CreateConnectorResponseTypeDef](./type_defs.md#createconnectorresponsetypedef) 


```python
# create_connector method usage example with argument unpacking

kwargs: CreateConnectorRequestRequestTypeDef = {  # (1)
    "capacity": ...,
    "connectorConfiguration": ...,
    "connectorName": ...,
    "kafkaCluster": ...,
    "kafkaClusterClientAuthentication": ...,
    "kafkaClusterEncryptionInTransit": ...,
    "kafkaConnectVersion": ...,
    "plugins": ...,
    "serviceExecutionRoleArn": ...,
}

parent.create_connector(**kwargs)
```

1. See [:material-code-braces: CreateConnectorRequestRequestTypeDef](./type_defs.md#createconnectorrequestrequesttypedef) 

### create\_custom\_plugin

Creates a custom plugin using the specified properties.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").create_custom_plugin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/create_custom_plugin.html)

```python
# create_custom_plugin method definition

await def create_custom_plugin(
    self,
    *,
    contentType: CustomPluginContentTypeType,  # (1)
    location: CustomPluginLocationTypeDef,  # (2)
    name: str,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateCustomPluginResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CustomPluginContentTypeType](./literals.md#customplugincontenttypetype) 
2. See [:material-code-braces: CustomPluginLocationTypeDef](./type_defs.md#custompluginlocationtypedef) 
3. See [:material-code-braces: CreateCustomPluginResponseTypeDef](./type_defs.md#createcustompluginresponsetypedef) 


```python
# create_custom_plugin method usage example with argument unpacking

kwargs: CreateCustomPluginRequestRequestTypeDef = {  # (1)
    "contentType": ...,
    "location": ...,
    "name": ...,
}

parent.create_custom_plugin(**kwargs)
```

1. See [:material-code-braces: CreateCustomPluginRequestRequestTypeDef](./type_defs.md#createcustompluginrequestrequesttypedef) 

### create\_worker\_configuration

Creates a worker configuration using the specified properties.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").create_worker_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/create_worker_configuration.html)

```python
# create_worker_configuration method definition

await def create_worker_configuration(
    self,
    *,
    name: str,
    propertiesFileContent: str,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateWorkerConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateWorkerConfigurationResponseTypeDef](./type_defs.md#createworkerconfigurationresponsetypedef) 


```python
# create_worker_configuration method usage example with argument unpacking

kwargs: CreateWorkerConfigurationRequestRequestTypeDef = {  # (1)
    "name": ...,
    "propertiesFileContent": ...,
}

parent.create_worker_configuration(**kwargs)
```

1. See [:material-code-braces: CreateWorkerConfigurationRequestRequestTypeDef](./type_defs.md#createworkerconfigurationrequestrequesttypedef) 

### delete\_connector

Deletes the specified connector.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").delete_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/delete_connector.html)

```python
# delete_connector method definition

await def delete_connector(
    self,
    *,
    connectorArn: str,
    currentVersion: str = ...,
) -> DeleteConnectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteConnectorResponseTypeDef](./type_defs.md#deleteconnectorresponsetypedef) 


```python
# delete_connector method usage example with argument unpacking

kwargs: DeleteConnectorRequestRequestTypeDef = {  # (1)
    "connectorArn": ...,
}

parent.delete_connector(**kwargs)
```

1. See [:material-code-braces: DeleteConnectorRequestRequestTypeDef](./type_defs.md#deleteconnectorrequestrequesttypedef) 

### delete\_custom\_plugin

Deletes a custom plugin.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").delete_custom_plugin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/delete_custom_plugin.html)

```python
# delete_custom_plugin method definition

await def delete_custom_plugin(
    self,
    *,
    customPluginArn: str,
) -> DeleteCustomPluginResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteCustomPluginResponseTypeDef](./type_defs.md#deletecustompluginresponsetypedef) 


```python
# delete_custom_plugin method usage example with argument unpacking

kwargs: DeleteCustomPluginRequestRequestTypeDef = {  # (1)
    "customPluginArn": ...,
}

parent.delete_custom_plugin(**kwargs)
```

1. See [:material-code-braces: DeleteCustomPluginRequestRequestTypeDef](./type_defs.md#deletecustompluginrequestrequesttypedef) 

### delete\_worker\_configuration

Deletes the specified worker configuration.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").delete_worker_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/delete_worker_configuration.html)

```python
# delete_worker_configuration method definition

await def delete_worker_configuration(
    self,
    *,
    workerConfigurationArn: str,
) -> DeleteWorkerConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteWorkerConfigurationResponseTypeDef](./type_defs.md#deleteworkerconfigurationresponsetypedef) 


```python
# delete_worker_configuration method usage example with argument unpacking

kwargs: DeleteWorkerConfigurationRequestRequestTypeDef = {  # (1)
    "workerConfigurationArn": ...,
}

parent.delete_worker_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteWorkerConfigurationRequestRequestTypeDef](./type_defs.md#deleteworkerconfigurationrequestrequesttypedef) 

### describe\_connector

Returns summary information about the connector.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").describe_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/describe_connector.html)

```python
# describe_connector method definition

await def describe_connector(
    self,
    *,
    connectorArn: str,
) -> DescribeConnectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConnectorResponseTypeDef](./type_defs.md#describeconnectorresponsetypedef) 


```python
# describe_connector method usage example with argument unpacking

kwargs: DescribeConnectorRequestRequestTypeDef = {  # (1)
    "connectorArn": ...,
}

parent.describe_connector(**kwargs)
```

1. See [:material-code-braces: DescribeConnectorRequestRequestTypeDef](./type_defs.md#describeconnectorrequestrequesttypedef) 

### describe\_custom\_plugin

A summary description of the custom plugin.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").describe_custom_plugin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/describe_custom_plugin.html)

```python
# describe_custom_plugin method definition

await def describe_custom_plugin(
    self,
    *,
    customPluginArn: str,
) -> DescribeCustomPluginResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCustomPluginResponseTypeDef](./type_defs.md#describecustompluginresponsetypedef) 


```python
# describe_custom_plugin method usage example with argument unpacking

kwargs: DescribeCustomPluginRequestRequestTypeDef = {  # (1)
    "customPluginArn": ...,
}

parent.describe_custom_plugin(**kwargs)
```

1. See [:material-code-braces: DescribeCustomPluginRequestRequestTypeDef](./type_defs.md#describecustompluginrequestrequesttypedef) 

### describe\_worker\_configuration

Returns information about a worker configuration.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").describe_worker_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/describe_worker_configuration.html)

```python
# describe_worker_configuration method definition

await def describe_worker_configuration(
    self,
    *,
    workerConfigurationArn: str,
) -> DescribeWorkerConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkerConfigurationResponseTypeDef](./type_defs.md#describeworkerconfigurationresponsetypedef) 


```python
# describe_worker_configuration method usage example with argument unpacking

kwargs: DescribeWorkerConfigurationRequestRequestTypeDef = {  # (1)
    "workerConfigurationArn": ...,
}

parent.describe_worker_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeWorkerConfigurationRequestRequestTypeDef](./type_defs.md#describeworkerconfigurationrequestrequesttypedef) 

### list\_connectors

Returns a list of all the connectors in this account and Region.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").list_connectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/list_connectors.html)

```python
# list_connectors method definition

await def list_connectors(
    self,
    *,
    connectorNamePrefix: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListConnectorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


```python
# list_connectors method usage example with argument unpacking

kwargs: ListConnectorsRequestRequestTypeDef = {  # (1)
    "connectorNamePrefix": ...,
}

parent.list_connectors(**kwargs)
```

1. See [:material-code-braces: ListConnectorsRequestRequestTypeDef](./type_defs.md#listconnectorsrequestrequesttypedef) 

### list\_custom\_plugins

Returns a list of all of the custom plugins in this account and Region.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").list_custom_plugins` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/list_custom_plugins.html)

```python
# list_custom_plugins method definition

await def list_custom_plugins(
    self,
    *,
    maxResults: int = ...,
    namePrefix: str = ...,
    nextToken: str = ...,
) -> ListCustomPluginsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCustomPluginsResponseTypeDef](./type_defs.md#listcustompluginsresponsetypedef) 


```python
# list_custom_plugins method usage example with argument unpacking

kwargs: ListCustomPluginsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_custom_plugins(**kwargs)
```

1. See [:material-code-braces: ListCustomPluginsRequestRequestTypeDef](./type_defs.md#listcustompluginsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists all the tags attached to the specified resource.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/list_tags_for_resource.html)

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

### list\_worker\_configurations

Returns a list of all of the worker configurations in this account and Region.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").list_worker_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/list_worker_configurations.html)

```python
# list_worker_configurations method definition

await def list_worker_configurations(
    self,
    *,
    maxResults: int = ...,
    namePrefix: str = ...,
    nextToken: str = ...,
) -> ListWorkerConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkerConfigurationsResponseTypeDef](./type_defs.md#listworkerconfigurationsresponsetypedef) 


```python
# list_worker_configurations method usage example with argument unpacking

kwargs: ListWorkerConfigurationsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_worker_configurations(**kwargs)
```

1. See [:material-code-braces: ListWorkerConfigurationsRequestRequestTypeDef](./type_defs.md#listworkerconfigurationsrequestrequesttypedef) 

### tag\_resource

Attaches tags to the specified resource.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/tag_resource.html)

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

Removes tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/untag_resource.html)

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

### update\_connector

Updates the specified connector.

Type annotations and code completion for `#!python session.create_client("kafkaconnect").update_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/client/update_connector.html)

```python
# update_connector method definition

await def update_connector(
    self,
    *,
    capacity: CapacityUpdateTypeDef,  # (1)
    connectorArn: str,
    currentVersion: str,
) -> UpdateConnectorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CapacityUpdateTypeDef](./type_defs.md#capacityupdatetypedef) 
2. See [:material-code-braces: UpdateConnectorResponseTypeDef](./type_defs.md#updateconnectorresponsetypedef) 


```python
# update_connector method usage example with argument unpacking

kwargs: UpdateConnectorRequestRequestTypeDef = {  # (1)
    "capacity": ...,
    "connectorArn": ...,
    "currentVersion": ...,
}

parent.update_connector(**kwargs)
```

1. See [:material-code-braces: UpdateConnectorRequestRequestTypeDef](./type_defs.md#updateconnectorrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("kafkaconnect").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "KafkaConnectClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("kafkaconnect").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Client)

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

Type annotations and code completion for `#!python session.create_client("kafkaconnect").get_paginator` method with overloads.

- `client.get_paginator("list_connectors")` -> [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
- `client.get_paginator("list_custom_plugins")` -> [ListCustomPluginsPaginator](./paginators.md#listcustompluginspaginator)
- `client.get_paginator("list_worker_configurations")` -> [ListWorkerConfigurationsPaginator](./paginators.md#listworkerconfigurationspaginator)



