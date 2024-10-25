# SchemasClient

> [Index](../README.md) > [Schemas](./README.md) > SchemasClient

!!! note ""

    Auto-generated documentation for [Schemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
    type annotations stubs module [types-aiobotocore-schemas](https://pypi.org/project/types-aiobotocore-schemas/).

## SchemasClient

Type annotations and code completion for `#!python session.create_client("schemas")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client)

```python
# SchemasClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_schemas.client import SchemasClient

session = get_session()
async with session.create_client("schemas") as client:
    client: SchemasClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("schemas").exceptions` structure.

```python
# SchemasClient.exceptions usage example

async with session.create_client("schemas") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.ForbiddenException,
        client.GoneException,
        client.InternalServerErrorException,
        client.NotFoundException,
        client.PreconditionFailedException,
        client.ServiceUnavailableException,
        client.TooManyRequestsException,
        client.UnauthorizedException,
    ) as e:
        print(e)
```

```python
# SchemasClient usage type checking example

from types_aiobotocore_schemas.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("schemas").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("schemas").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_discoverer

Creates a discoverer.

Type annotations and code completion for `#!python session.create_client("schemas").create_discoverer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.create_discoverer)

```python
# create_discoverer method definition

await def create_discoverer(
    self,
    *,
    SourceArn: str,
    Description: str = ...,
    CrossAccount: bool = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateDiscovererResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateDiscovererResponseTypeDef](./type_defs.md#creatediscovererresponsetypedef) 


```python
# create_discoverer method usage example with argument unpacking

kwargs: CreateDiscovererRequestRequestTypeDef = {  # (1)
    "SourceArn": ...,
}

parent.create_discoverer(**kwargs)
```

1. See [:material-code-braces: CreateDiscovererRequestRequestTypeDef](./type_defs.md#creatediscovererrequestrequesttypedef) 

### create\_registry

Creates a registry.

Type annotations and code completion for `#!python session.create_client("schemas").create_registry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.create_registry)

```python
# create_registry method definition

await def create_registry(
    self,
    *,
    RegistryName: str,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateRegistryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateRegistryResponseTypeDef](./type_defs.md#createregistryresponsetypedef) 


```python
# create_registry method usage example with argument unpacking

kwargs: CreateRegistryRequestRequestTypeDef = {  # (1)
    "RegistryName": ...,
}

parent.create_registry(**kwargs)
```

1. See [:material-code-braces: CreateRegistryRequestRequestTypeDef](./type_defs.md#createregistryrequestrequesttypedef) 

### create\_schema

Creates a schema definition.

Type annotations and code completion for `#!python session.create_client("schemas").create_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.create_schema)

```python
# create_schema method definition

await def create_schema(
    self,
    *,
    Content: str,
    RegistryName: str,
    SchemaName: str,
    Type: TypeType,  # (1)
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateSchemaResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-braces: CreateSchemaResponseTypeDef](./type_defs.md#createschemaresponsetypedef) 


```python
# create_schema method usage example with argument unpacking

kwargs: CreateSchemaRequestRequestTypeDef = {  # (1)
    "Content": ...,
    "RegistryName": ...,
    "SchemaName": ...,
    "Type": ...,
}

parent.create_schema(**kwargs)
```

1. See [:material-code-braces: CreateSchemaRequestRequestTypeDef](./type_defs.md#createschemarequestrequesttypedef) 

### delete\_discoverer

Deletes a discoverer.

Type annotations and code completion for `#!python session.create_client("schemas").delete_discoverer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.delete_discoverer)

```python
# delete_discoverer method definition

await def delete_discoverer(
    self,
    *,
    DiscovererId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_discoverer method usage example with argument unpacking

kwargs: DeleteDiscovererRequestRequestTypeDef = {  # (1)
    "DiscovererId": ...,
}

parent.delete_discoverer(**kwargs)
```

1. See [:material-code-braces: DeleteDiscovererRequestRequestTypeDef](./type_defs.md#deletediscovererrequestrequesttypedef) 

### delete\_registry

Deletes a Registry.

Type annotations and code completion for `#!python session.create_client("schemas").delete_registry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.delete_registry)

```python
# delete_registry method definition

await def delete_registry(
    self,
    *,
    RegistryName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_registry method usage example with argument unpacking

kwargs: DeleteRegistryRequestRequestTypeDef = {  # (1)
    "RegistryName": ...,
}

parent.delete_registry(**kwargs)
```

1. See [:material-code-braces: DeleteRegistryRequestRequestTypeDef](./type_defs.md#deleteregistryrequestrequesttypedef) 

### delete\_resource\_policy

Delete the resource-based policy attached to the specified registry.

Type annotations and code completion for `#!python session.create_client("schemas").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.delete_resource_policy)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    RegistryName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyRequestRequestTypeDef = {  # (1)
    "RegistryName": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef) 

### delete\_schema

Delete a schema definition.

Type annotations and code completion for `#!python session.create_client("schemas").delete_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.delete_schema)

```python
# delete_schema method definition

await def delete_schema(
    self,
    *,
    RegistryName: str,
    SchemaName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_schema method usage example with argument unpacking

kwargs: DeleteSchemaRequestRequestTypeDef = {  # (1)
    "RegistryName": ...,
    "SchemaName": ...,
}

parent.delete_schema(**kwargs)
```

1. See [:material-code-braces: DeleteSchemaRequestRequestTypeDef](./type_defs.md#deleteschemarequestrequesttypedef) 

### delete\_schema\_version

Delete the schema version definition See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/schemas-2019-12-02/DeleteSchemaVersion).

Type annotations and code completion for `#!python session.create_client("schemas").delete_schema_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.delete_schema_version)

```python
# delete_schema_version method definition

await def delete_schema_version(
    self,
    *,
    RegistryName: str,
    SchemaName: str,
    SchemaVersion: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_schema_version method usage example with argument unpacking

kwargs: DeleteSchemaVersionRequestRequestTypeDef = {  # (1)
    "RegistryName": ...,
    "SchemaName": ...,
    "SchemaVersion": ...,
}

parent.delete_schema_version(**kwargs)
```

1. See [:material-code-braces: DeleteSchemaVersionRequestRequestTypeDef](./type_defs.md#deleteschemaversionrequestrequesttypedef) 

### describe\_code\_binding

Describe the code binding URI.

Type annotations and code completion for `#!python session.create_client("schemas").describe_code_binding` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.describe_code_binding)

```python
# describe_code_binding method definition

await def describe_code_binding(
    self,
    *,
    Language: str,
    RegistryName: str,
    SchemaName: str,
    SchemaVersion: str = ...,
) -> DescribeCodeBindingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCodeBindingResponseTypeDef](./type_defs.md#describecodebindingresponsetypedef) 


```python
# describe_code_binding method usage example with argument unpacking

kwargs: DescribeCodeBindingRequestRequestTypeDef = {  # (1)
    "Language": ...,
    "RegistryName": ...,
    "SchemaName": ...,
}

parent.describe_code_binding(**kwargs)
```

1. See [:material-code-braces: DescribeCodeBindingRequestRequestTypeDef](./type_defs.md#describecodebindingrequestrequesttypedef) 

### describe\_discoverer

Describes the discoverer.

Type annotations and code completion for `#!python session.create_client("schemas").describe_discoverer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.describe_discoverer)

```python
# describe_discoverer method definition

await def describe_discoverer(
    self,
    *,
    DiscovererId: str,
) -> DescribeDiscovererResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDiscovererResponseTypeDef](./type_defs.md#describediscovererresponsetypedef) 


```python
# describe_discoverer method usage example with argument unpacking

kwargs: DescribeDiscovererRequestRequestTypeDef = {  # (1)
    "DiscovererId": ...,
}

parent.describe_discoverer(**kwargs)
```

1. See [:material-code-braces: DescribeDiscovererRequestRequestTypeDef](./type_defs.md#describediscovererrequestrequesttypedef) 

### describe\_registry

Describes the registry.

Type annotations and code completion for `#!python session.create_client("schemas").describe_registry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.describe_registry)

```python
# describe_registry method definition

await def describe_registry(
    self,
    *,
    RegistryName: str,
) -> DescribeRegistryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRegistryResponseTypeDef](./type_defs.md#describeregistryresponsetypedef) 


```python
# describe_registry method usage example with argument unpacking

kwargs: DescribeRegistryRequestRequestTypeDef = {  # (1)
    "RegistryName": ...,
}

parent.describe_registry(**kwargs)
```

1. See [:material-code-braces: DescribeRegistryRequestRequestTypeDef](./type_defs.md#describeregistryrequestrequesttypedef) 

### describe\_schema

Retrieve the schema definition.

Type annotations and code completion for `#!python session.create_client("schemas").describe_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.describe_schema)

```python
# describe_schema method definition

await def describe_schema(
    self,
    *,
    RegistryName: str,
    SchemaName: str,
    SchemaVersion: str = ...,
) -> DescribeSchemaResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSchemaResponseTypeDef](./type_defs.md#describeschemaresponsetypedef) 


```python
# describe_schema method usage example with argument unpacking

kwargs: DescribeSchemaRequestRequestTypeDef = {  # (1)
    "RegistryName": ...,
    "SchemaName": ...,
}

parent.describe_schema(**kwargs)
```

1. See [:material-code-braces: DescribeSchemaRequestRequestTypeDef](./type_defs.md#describeschemarequestrequesttypedef) 

### export\_schema

See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/schemas-2019-12-02/ExportSchema).

Type annotations and code completion for `#!python session.create_client("schemas").export_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.export_schema)

```python
# export_schema method definition

await def export_schema(
    self,
    *,
    RegistryName: str,
    SchemaName: str,
    Type: str,
    SchemaVersion: str = ...,
) -> ExportSchemaResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExportSchemaResponseTypeDef](./type_defs.md#exportschemaresponsetypedef) 


```python
# export_schema method usage example with argument unpacking

kwargs: ExportSchemaRequestRequestTypeDef = {  # (1)
    "RegistryName": ...,
    "SchemaName": ...,
    "Type": ...,
}

parent.export_schema(**kwargs)
```

1. See [:material-code-braces: ExportSchemaRequestRequestTypeDef](./type_defs.md#exportschemarequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("schemas").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.generate_presigned_url)

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


### get\_code\_binding\_source

Get the code binding source URI.

Type annotations and code completion for `#!python session.create_client("schemas").get_code_binding_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.get_code_binding_source)

```python
# get_code_binding_source method definition

await def get_code_binding_source(
    self,
    *,
    Language: str,
    RegistryName: str,
    SchemaName: str,
    SchemaVersion: str = ...,
) -> GetCodeBindingSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCodeBindingSourceResponseTypeDef](./type_defs.md#getcodebindingsourceresponsetypedef) 


```python
# get_code_binding_source method usage example with argument unpacking

kwargs: GetCodeBindingSourceRequestRequestTypeDef = {  # (1)
    "Language": ...,
    "RegistryName": ...,
    "SchemaName": ...,
}

parent.get_code_binding_source(**kwargs)
```

1. See [:material-code-braces: GetCodeBindingSourceRequestRequestTypeDef](./type_defs.md#getcodebindingsourcerequestrequesttypedef) 

### get\_discovered\_schema

Get the discovered schema that was generated based on sampled events.

Type annotations and code completion for `#!python session.create_client("schemas").get_discovered_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.get_discovered_schema)

```python
# get_discovered_schema method definition

await def get_discovered_schema(
    self,
    *,
    Events: Sequence[str],
    Type: TypeType,  # (1)
) -> GetDiscoveredSchemaResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-braces: GetDiscoveredSchemaResponseTypeDef](./type_defs.md#getdiscoveredschemaresponsetypedef) 


```python
# get_discovered_schema method usage example with argument unpacking

kwargs: GetDiscoveredSchemaRequestRequestTypeDef = {  # (1)
    "Events": ...,
    "Type": ...,
}

parent.get_discovered_schema(**kwargs)
```

1. See [:material-code-braces: GetDiscoveredSchemaRequestRequestTypeDef](./type_defs.md#getdiscoveredschemarequestrequesttypedef) 

### get\_resource\_policy

Retrieves the resource-based policy attached to a given registry.

Type annotations and code completion for `#!python session.create_client("schemas").get_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.get_resource_policy)

```python
# get_resource_policy method definition

await def get_resource_policy(
    self,
    *,
    RegistryName: str = ...,
) -> GetResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef) 


```python
# get_resource_policy method usage example with argument unpacking

kwargs: GetResourcePolicyRequestRequestTypeDef = {  # (1)
    "RegistryName": ...,
}

parent.get_resource_policy(**kwargs)
```

1. See [:material-code-braces: GetResourcePolicyRequestRequestTypeDef](./type_defs.md#getresourcepolicyrequestrequesttypedef) 

### list\_discoverers

List the discoverers.

Type annotations and code completion for `#!python session.create_client("schemas").list_discoverers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.list_discoverers)

```python
# list_discoverers method definition

await def list_discoverers(
    self,
    *,
    DiscovererIdPrefix: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
    SourceArnPrefix: str = ...,
) -> ListDiscoverersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDiscoverersResponseTypeDef](./type_defs.md#listdiscoverersresponsetypedef) 


```python
# list_discoverers method usage example with argument unpacking

kwargs: ListDiscoverersRequestRequestTypeDef = {  # (1)
    "DiscovererIdPrefix": ...,
}

parent.list_discoverers(**kwargs)
```

1. See [:material-code-braces: ListDiscoverersRequestRequestTypeDef](./type_defs.md#listdiscoverersrequestrequesttypedef) 

### list\_registries

List the registries.

Type annotations and code completion for `#!python session.create_client("schemas").list_registries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.list_registries)

```python
# list_registries method definition

await def list_registries(
    self,
    *,
    Limit: int = ...,
    NextToken: str = ...,
    RegistryNamePrefix: str = ...,
    Scope: str = ...,
) -> ListRegistriesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRegistriesResponseTypeDef](./type_defs.md#listregistriesresponsetypedef) 


```python
# list_registries method usage example with argument unpacking

kwargs: ListRegistriesRequestRequestTypeDef = {  # (1)
    "Limit": ...,
}

parent.list_registries(**kwargs)
```

1. See [:material-code-braces: ListRegistriesRequestRequestTypeDef](./type_defs.md#listregistriesrequestrequesttypedef) 

### list\_schema\_versions

Provides a list of the schema versions and related information.

Type annotations and code completion for `#!python session.create_client("schemas").list_schema_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.list_schema_versions)

```python
# list_schema_versions method definition

await def list_schema_versions(
    self,
    *,
    RegistryName: str,
    SchemaName: str,
    Limit: int = ...,
    NextToken: str = ...,
) -> ListSchemaVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSchemaVersionsResponseTypeDef](./type_defs.md#listschemaversionsresponsetypedef) 


```python
# list_schema_versions method usage example with argument unpacking

kwargs: ListSchemaVersionsRequestRequestTypeDef = {  # (1)
    "RegistryName": ...,
    "SchemaName": ...,
}

parent.list_schema_versions(**kwargs)
```

1. See [:material-code-braces: ListSchemaVersionsRequestRequestTypeDef](./type_defs.md#listschemaversionsrequestrequesttypedef) 

### list\_schemas

List the schemas.

Type annotations and code completion for `#!python session.create_client("schemas").list_schemas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.list_schemas)

```python
# list_schemas method definition

await def list_schemas(
    self,
    *,
    RegistryName: str,
    Limit: int = ...,
    NextToken: str = ...,
    SchemaNamePrefix: str = ...,
) -> ListSchemasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


```python
# list_schemas method usage example with argument unpacking

kwargs: ListSchemasRequestRequestTypeDef = {  # (1)
    "RegistryName": ...,
}

parent.list_schemas(**kwargs)
```

1. See [:material-code-braces: ListSchemasRequestRequestTypeDef](./type_defs.md#listschemasrequestrequesttypedef) 

### list\_tags\_for\_resource

Get tags for resource.

Type annotations and code completion for `#!python session.create_client("schemas").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_code\_binding

Put code binding URI See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/schemas-2019-12-02/PutCodeBinding).

Type annotations and code completion for `#!python session.create_client("schemas").put_code_binding` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.put_code_binding)

```python
# put_code_binding method definition

await def put_code_binding(
    self,
    *,
    Language: str,
    RegistryName: str,
    SchemaName: str,
    SchemaVersion: str = ...,
) -> PutCodeBindingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutCodeBindingResponseTypeDef](./type_defs.md#putcodebindingresponsetypedef) 


```python
# put_code_binding method usage example with argument unpacking

kwargs: PutCodeBindingRequestRequestTypeDef = {  # (1)
    "Language": ...,
    "RegistryName": ...,
    "SchemaName": ...,
}

parent.put_code_binding(**kwargs)
```

1. See [:material-code-braces: PutCodeBindingRequestRequestTypeDef](./type_defs.md#putcodebindingrequestrequesttypedef) 

### put\_resource\_policy

The name of the policy.

Type annotations and code completion for `#!python session.create_client("schemas").put_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.put_resource_policy)

```python
# put_resource_policy method definition

await def put_resource_policy(
    self,
    *,
    Policy: str,
    RegistryName: str = ...,
    RevisionId: str = ...,
) -> PutResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef) 


```python
# put_resource_policy method usage example with argument unpacking

kwargs: PutResourcePolicyRequestRequestTypeDef = {  # (1)
    "Policy": ...,
}

parent.put_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef) 

### search\_schemas

Search the schemas See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/schemas-2019-12-02/SearchSchemas).

Type annotations and code completion for `#!python session.create_client("schemas").search_schemas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.search_schemas)

```python
# search_schemas method definition

await def search_schemas(
    self,
    *,
    Keywords: str,
    RegistryName: str,
    Limit: int = ...,
    NextToken: str = ...,
) -> SearchSchemasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SearchSchemasResponseTypeDef](./type_defs.md#searchschemasresponsetypedef) 


```python
# search_schemas method usage example with argument unpacking

kwargs: SearchSchemasRequestRequestTypeDef = {  # (1)
    "Keywords": ...,
    "RegistryName": ...,
}

parent.search_schemas(**kwargs)
```

1. See [:material-code-braces: SearchSchemasRequestRequestTypeDef](./type_defs.md#searchschemasrequestrequesttypedef) 

### start\_discoverer

Starts the discoverer See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/schemas-2019-12-02/StartDiscoverer).

Type annotations and code completion for `#!python session.create_client("schemas").start_discoverer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.start_discoverer)

```python
# start_discoverer method definition

await def start_discoverer(
    self,
    *,
    DiscovererId: str,
) -> StartDiscovererResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartDiscovererResponseTypeDef](./type_defs.md#startdiscovererresponsetypedef) 


```python
# start_discoverer method usage example with argument unpacking

kwargs: StartDiscovererRequestRequestTypeDef = {  # (1)
    "DiscovererId": ...,
}

parent.start_discoverer(**kwargs)
```

1. See [:material-code-braces: StartDiscovererRequestRequestTypeDef](./type_defs.md#startdiscovererrequestrequesttypedef) 

### stop\_discoverer

Stops the discoverer See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/schemas-2019-12-02/StopDiscoverer).

Type annotations and code completion for `#!python session.create_client("schemas").stop_discoverer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.stop_discoverer)

```python
# stop_discoverer method definition

await def stop_discoverer(
    self,
    *,
    DiscovererId: str,
) -> StopDiscovererResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopDiscovererResponseTypeDef](./type_defs.md#stopdiscovererresponsetypedef) 


```python
# stop_discoverer method usage example with argument unpacking

kwargs: StopDiscovererRequestRequestTypeDef = {  # (1)
    "DiscovererId": ...,
}

parent.stop_discoverer(**kwargs)
```

1. See [:material-code-braces: StopDiscovererRequestRequestTypeDef](./type_defs.md#stopdiscovererrequestrequesttypedef) 

### tag\_resource

Add tags to a resource.

Type annotations and code completion for `#!python session.create_client("schemas").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from a resource.

Type annotations and code completion for `#!python session.create_client("schemas").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_discoverer

Updates the discoverer See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/schemas-2019-12-02/UpdateDiscoverer).

Type annotations and code completion for `#!python session.create_client("schemas").update_discoverer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.update_discoverer)

```python
# update_discoverer method definition

await def update_discoverer(
    self,
    *,
    DiscovererId: str,
    Description: str = ...,
    CrossAccount: bool = ...,
) -> UpdateDiscovererResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDiscovererResponseTypeDef](./type_defs.md#updatediscovererresponsetypedef) 


```python
# update_discoverer method usage example with argument unpacking

kwargs: UpdateDiscovererRequestRequestTypeDef = {  # (1)
    "DiscovererId": ...,
}

parent.update_discoverer(**kwargs)
```

1. See [:material-code-braces: UpdateDiscovererRequestRequestTypeDef](./type_defs.md#updatediscovererrequestrequesttypedef) 

### update\_registry

Updates a registry.

Type annotations and code completion for `#!python session.create_client("schemas").update_registry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.update_registry)

```python
# update_registry method definition

await def update_registry(
    self,
    *,
    RegistryName: str,
    Description: str = ...,
) -> UpdateRegistryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateRegistryResponseTypeDef](./type_defs.md#updateregistryresponsetypedef) 


```python
# update_registry method usage example with argument unpacking

kwargs: UpdateRegistryRequestRequestTypeDef = {  # (1)
    "RegistryName": ...,
}

parent.update_registry(**kwargs)
```

1. See [:material-code-braces: UpdateRegistryRequestRequestTypeDef](./type_defs.md#updateregistryrequestrequesttypedef) 

### update\_schema

Updates the schema definition .

Type annotations and code completion for `#!python session.create_client("schemas").update_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.update_schema)

```python
# update_schema method definition

await def update_schema(
    self,
    *,
    RegistryName: str,
    SchemaName: str,
    ClientTokenId: str = ...,
    Content: str = ...,
    Description: str = ...,
    Type: TypeType = ...,  # (1)
) -> UpdateSchemaResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-braces: UpdateSchemaResponseTypeDef](./type_defs.md#updateschemaresponsetypedef) 


```python
# update_schema method usage example with argument unpacking

kwargs: UpdateSchemaRequestRequestTypeDef = {  # (1)
    "RegistryName": ...,
    "SchemaName": ...,
}

parent.update_schema(**kwargs)
```

1. See [:material-code-braces: UpdateSchemaRequestRequestTypeDef](./type_defs.md#updateschemarequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("schemas").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "SchemasClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("schemas").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("schemas").get_paginator` method with overloads.

- `client.get_paginator("list_discoverers")` -> [ListDiscoverersPaginator](./paginators.md#listdiscovererspaginator)
- `client.get_paginator("list_registries")` -> [ListRegistriesPaginator](./paginators.md#listregistriespaginator)
- `client.get_paginator("list_schema_versions")` -> [ListSchemaVersionsPaginator](./paginators.md#listschemaversionspaginator)
- `client.get_paginator("list_schemas")` -> [ListSchemasPaginator](./paginators.md#listschemaspaginator)
- `client.get_paginator("search_schemas")` -> [SearchSchemasPaginator](./paginators.md#searchschemaspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("schemas").get_waiter` method with overloads.

- `client.get_waiter("code_binding_exists")` -> [CodeBindingExistsWaiter](./waiters.md#codebindingexistswaiter)

