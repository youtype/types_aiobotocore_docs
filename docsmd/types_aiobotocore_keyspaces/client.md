# KeyspacesClient

> [Index](../README.md) > [Keyspaces](./README.md) > KeyspacesClient

!!! note ""

    Auto-generated documentation for [Keyspaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#keyspaces)
    type annotations stubs module [types-aiobotocore-keyspaces](https://pypi.org/project/types-aiobotocore-keyspaces/).

## KeyspacesClient

Type annotations and code completion for `#!python session.create_client("keyspaces")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client)

```python
# KeyspacesClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_keyspaces.client import KeyspacesClient

session = get_session()
async with session.create_client("keyspaces") as client:
    client: KeyspacesClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("keyspaces").exceptions` structure.

```python
# KeyspacesClient.exceptions usage example

async with session.create_client("keyspaces") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# KeyspacesClient usage type checking example

from types_aiobotocore_keyspaces.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("keyspaces").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("keyspaces").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/generate_presigned_url.html)

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


### create\_keyspace

The <code>CreateKeyspace</code> operation adds a new keyspace to your account.

Type annotations and code completion for `#!python session.create_client("keyspaces").create_keyspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/create_keyspace.html)

```python
# create_keyspace method definition

await def create_keyspace(
    self,
    *,
    keyspaceName: str,
    tags: Sequence[TagTypeDef] = ...,  # (1)
    replicationSpecification: ReplicationSpecificationTypeDef = ...,  # (2)
) -> CreateKeyspaceResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ReplicationSpecificationTypeDef](./type_defs.md#replicationspecificationtypedef) 
3. See [:material-code-braces: CreateKeyspaceResponseTypeDef](./type_defs.md#createkeyspaceresponsetypedef) 


```python
# create_keyspace method usage example with argument unpacking

kwargs: CreateKeyspaceRequestTypeDef = {  # (1)
    "keyspaceName": ...,
}

parent.create_keyspace(**kwargs)
```

1. See [:material-code-braces: CreateKeyspaceRequestTypeDef](./type_defs.md#createkeyspacerequesttypedef) 

### create\_table

The <code>CreateTable</code> operation adds a new table to the specified
keyspace.

Type annotations and code completion for `#!python session.create_client("keyspaces").create_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/create_table.html)

```python
# create_table method definition

await def create_table(
    self,
    *,
    keyspaceName: str,
    tableName: str,
    schemaDefinition: SchemaDefinitionUnionTypeDef,  # (1)
    comment: CommentTypeDef = ...,  # (2)
    capacitySpecification: CapacitySpecificationTypeDef = ...,  # (3)
    encryptionSpecification: EncryptionSpecificationTypeDef = ...,  # (4)
    pointInTimeRecovery: PointInTimeRecoveryTypeDef = ...,  # (5)
    ttl: TimeToLiveTypeDef = ...,  # (6)
    defaultTimeToLive: int = ...,
    tags: Sequence[TagTypeDef] = ...,  # (7)
    clientSideTimestamps: ClientSideTimestampsTypeDef = ...,  # (8)
    autoScalingSpecification: AutoScalingSpecificationTypeDef = ...,  # (9)
    replicaSpecifications: Sequence[ReplicaSpecificationTypeDef] = ...,  # (10)
) -> CreateTableResponseTypeDef:  # (11)
    ...
```

1. See [:material-code-braces: SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef) [:material-code-braces: SchemaDefinitionOutputTypeDef](./type_defs.md#schemadefinitionoutputtypedef) 
2. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
3. See [:material-code-braces: CapacitySpecificationTypeDef](./type_defs.md#capacityspecificationtypedef) 
4. See [:material-code-braces: EncryptionSpecificationTypeDef](./type_defs.md#encryptionspecificationtypedef) 
5. See [:material-code-braces: PointInTimeRecoveryTypeDef](./type_defs.md#pointintimerecoverytypedef) 
6. See [:material-code-braces: TimeToLiveTypeDef](./type_defs.md#timetolivetypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: ClientSideTimestampsTypeDef](./type_defs.md#clientsidetimestampstypedef) 
9. See [:material-code-braces: AutoScalingSpecificationTypeDef](./type_defs.md#autoscalingspecificationtypedef) 
10. See [:material-code-braces: ReplicaSpecificationTypeDef](./type_defs.md#replicaspecificationtypedef) 
11. See [:material-code-braces: CreateTableResponseTypeDef](./type_defs.md#createtableresponsetypedef) 


```python
# create_table method usage example with argument unpacking

kwargs: CreateTableRequestTypeDef = {  # (1)
    "keyspaceName": ...,
    "tableName": ...,
    "schemaDefinition": ...,
}

parent.create_table(**kwargs)
```

1. See [:material-code-braces: CreateTableRequestTypeDef](./type_defs.md#createtablerequesttypedef) 

### create\_type

The <code>CreateType</code> operation creates a new user-defined type in the
specified keyspace.

Type annotations and code completion for `#!python session.create_client("keyspaces").create_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/create_type.html)

```python
# create_type method definition

await def create_type(
    self,
    *,
    keyspaceName: str,
    typeName: str,
    fieldDefinitions: Sequence[FieldDefinitionTypeDef],  # (1)
) -> CreateTypeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FieldDefinitionTypeDef](./type_defs.md#fielddefinitiontypedef) 
2. See [:material-code-braces: CreateTypeResponseTypeDef](./type_defs.md#createtyperesponsetypedef) 


```python
# create_type method usage example with argument unpacking

kwargs: CreateTypeRequestTypeDef = {  # (1)
    "keyspaceName": ...,
    "typeName": ...,
    "fieldDefinitions": ...,
}

parent.create_type(**kwargs)
```

1. See [:material-code-braces: CreateTypeRequestTypeDef](./type_defs.md#createtyperequesttypedef) 

### delete\_keyspace

The <code>DeleteKeyspace</code> operation deletes a keyspace and all of its
tables.

Type annotations and code completion for `#!python session.create_client("keyspaces").delete_keyspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/delete_keyspace.html)

```python
# delete_keyspace method definition

await def delete_keyspace(
    self,
    *,
    keyspaceName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_keyspace method usage example with argument unpacking

kwargs: DeleteKeyspaceRequestTypeDef = {  # (1)
    "keyspaceName": ...,
}

parent.delete_keyspace(**kwargs)
```

1. See [:material-code-braces: DeleteKeyspaceRequestTypeDef](./type_defs.md#deletekeyspacerequesttypedef) 

### delete\_table

The <code>DeleteTable</code> operation deletes a table and all of its data.

Type annotations and code completion for `#!python session.create_client("keyspaces").delete_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/delete_table.html)

```python
# delete_table method definition

await def delete_table(
    self,
    *,
    keyspaceName: str,
    tableName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_table method usage example with argument unpacking

kwargs: DeleteTableRequestTypeDef = {  # (1)
    "keyspaceName": ...,
    "tableName": ...,
}

parent.delete_table(**kwargs)
```

1. See [:material-code-braces: DeleteTableRequestTypeDef](./type_defs.md#deletetablerequesttypedef) 

### delete\_type

The <code>DeleteType</code> operation deletes a user-defined type (UDT).

Type annotations and code completion for `#!python session.create_client("keyspaces").delete_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/delete_type.html)

```python
# delete_type method definition

await def delete_type(
    self,
    *,
    keyspaceName: str,
    typeName: str,
) -> DeleteTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTypeResponseTypeDef](./type_defs.md#deletetyperesponsetypedef) 


```python
# delete_type method usage example with argument unpacking

kwargs: DeleteTypeRequestTypeDef = {  # (1)
    "keyspaceName": ...,
    "typeName": ...,
}

parent.delete_type(**kwargs)
```

1. See [:material-code-braces: DeleteTypeRequestTypeDef](./type_defs.md#deletetyperequesttypedef) 

### get\_keyspace

Returns the name of the specified keyspace, the Amazon Resource Name (ARN), the
replication strategy, the Amazon Web Services Regions of a multi-Region
keyspace, and the status of newly added Regions after an
<code>UpdateKeyspace</code> operation.

Type annotations and code completion for `#!python session.create_client("keyspaces").get_keyspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/get_keyspace.html)

```python
# get_keyspace method definition

await def get_keyspace(
    self,
    *,
    keyspaceName: str,
) -> GetKeyspaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKeyspaceResponseTypeDef](./type_defs.md#getkeyspaceresponsetypedef) 


```python
# get_keyspace method usage example with argument unpacking

kwargs: GetKeyspaceRequestTypeDef = {  # (1)
    "keyspaceName": ...,
}

parent.get_keyspace(**kwargs)
```

1. See [:material-code-braces: GetKeyspaceRequestTypeDef](./type_defs.md#getkeyspacerequesttypedef) 

### get\_table

Returns information about the table, including the table's name and current
status, the keyspace name, configuration settings, and metadata.

Type annotations and code completion for `#!python session.create_client("keyspaces").get_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/get_table.html)

```python
# get_table method definition

await def get_table(
    self,
    *,
    keyspaceName: str,
    tableName: str,
) -> GetTableResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableResponseTypeDef](./type_defs.md#gettableresponsetypedef) 


```python
# get_table method usage example with argument unpacking

kwargs: GetTableRequestTypeDef = {  # (1)
    "keyspaceName": ...,
    "tableName": ...,
}

parent.get_table(**kwargs)
```

1. See [:material-code-braces: GetTableRequestTypeDef](./type_defs.md#gettablerequesttypedef) 

### get\_table\_auto\_scaling\_settings

Returns auto scaling related settings of the specified table in JSON format.

Type annotations and code completion for `#!python session.create_client("keyspaces").get_table_auto_scaling_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/get_table_auto_scaling_settings.html)

```python
# get_table_auto_scaling_settings method definition

await def get_table_auto_scaling_settings(
    self,
    *,
    keyspaceName: str,
    tableName: str,
) -> GetTableAutoScalingSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableAutoScalingSettingsResponseTypeDef](./type_defs.md#gettableautoscalingsettingsresponsetypedef) 


```python
# get_table_auto_scaling_settings method usage example with argument unpacking

kwargs: GetTableAutoScalingSettingsRequestTypeDef = {  # (1)
    "keyspaceName": ...,
    "tableName": ...,
}

parent.get_table_auto_scaling_settings(**kwargs)
```

1. See [:material-code-braces: GetTableAutoScalingSettingsRequestTypeDef](./type_defs.md#gettableautoscalingsettingsrequesttypedef) 

### get\_type

The <code>GetType</code> operation returns information about the type, for
example the field definitions, the timestamp when the type was last modified,
the level of nesting, the status, and details about if the type is used in
other types and tables.

Type annotations and code completion for `#!python session.create_client("keyspaces").get_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/get_type.html)

```python
# get_type method definition

await def get_type(
    self,
    *,
    keyspaceName: str,
    typeName: str,
) -> GetTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTypeResponseTypeDef](./type_defs.md#gettyperesponsetypedef) 


```python
# get_type method usage example with argument unpacking

kwargs: GetTypeRequestTypeDef = {  # (1)
    "keyspaceName": ...,
    "typeName": ...,
}

parent.get_type(**kwargs)
```

1. See [:material-code-braces: GetTypeRequestTypeDef](./type_defs.md#gettyperequesttypedef) 

### list\_keyspaces

The <code>ListKeyspaces</code> operation returns a list of keyspaces.

Type annotations and code completion for `#!python session.create_client("keyspaces").list_keyspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/list_keyspaces.html)

```python
# list_keyspaces method definition

await def list_keyspaces(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListKeyspacesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKeyspacesResponseTypeDef](./type_defs.md#listkeyspacesresponsetypedef) 


```python
# list_keyspaces method usage example with argument unpacking

kwargs: ListKeyspacesRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_keyspaces(**kwargs)
```

1. See [:material-code-braces: ListKeyspacesRequestTypeDef](./type_defs.md#listkeyspacesrequesttypedef) 

### list\_tables

The <code>ListTables</code> operation returns a list of tables for a specified
keyspace.

Type annotations and code completion for `#!python session.create_client("keyspaces").list_tables` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/list_tables.html)

```python
# list_tables method definition

await def list_tables(
    self,
    *,
    keyspaceName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTablesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef) 


```python
# list_tables method usage example with argument unpacking

kwargs: ListTablesRequestTypeDef = {  # (1)
    "keyspaceName": ...,
}

parent.list_tables(**kwargs)
```

1. See [:material-code-braces: ListTablesRequestTypeDef](./type_defs.md#listtablesrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of all tags associated with the specified Amazon Keyspaces
resource.

Type annotations and code completion for `#!python session.create_client("keyspaces").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
    nextToken: str = ...,
    maxResults: int = ...,
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

### list\_types

The <code>ListTypes</code> operation returns a list of types for a specified
keyspace.

Type annotations and code completion for `#!python session.create_client("keyspaces").list_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/list_types.html)

```python
# list_types method definition

await def list_types(
    self,
    *,
    keyspaceName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTypesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTypesResponseTypeDef](./type_defs.md#listtypesresponsetypedef) 


```python
# list_types method usage example with argument unpacking

kwargs: ListTypesRequestTypeDef = {  # (1)
    "keyspaceName": ...,
}

parent.list_types(**kwargs)
```

1. See [:material-code-braces: ListTypesRequestTypeDef](./type_defs.md#listtypesrequesttypedef) 

### restore\_table

Restores the table to the specified point in time within the
<code>earliest_restorable_timestamp</code> and the current time.

Type annotations and code completion for `#!python session.create_client("keyspaces").restore_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/restore_table.html)

```python
# restore_table method definition

await def restore_table(
    self,
    *,
    sourceKeyspaceName: str,
    sourceTableName: str,
    targetKeyspaceName: str,
    targetTableName: str,
    restoreTimestamp: TimestampTypeDef = ...,
    capacitySpecificationOverride: CapacitySpecificationTypeDef = ...,  # (1)
    encryptionSpecificationOverride: EncryptionSpecificationTypeDef = ...,  # (2)
    pointInTimeRecoveryOverride: PointInTimeRecoveryTypeDef = ...,  # (3)
    tagsOverride: Sequence[TagTypeDef] = ...,  # (4)
    autoScalingSpecification: AutoScalingSpecificationTypeDef = ...,  # (5)
    replicaSpecifications: Sequence[ReplicaSpecificationTypeDef] = ...,  # (6)
) -> RestoreTableResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: CapacitySpecificationTypeDef](./type_defs.md#capacityspecificationtypedef) 
2. See [:material-code-braces: EncryptionSpecificationTypeDef](./type_defs.md#encryptionspecificationtypedef) 
3. See [:material-code-braces: PointInTimeRecoveryTypeDef](./type_defs.md#pointintimerecoverytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: AutoScalingSpecificationTypeDef](./type_defs.md#autoscalingspecificationtypedef) 
6. See [:material-code-braces: ReplicaSpecificationTypeDef](./type_defs.md#replicaspecificationtypedef) 
7. See [:material-code-braces: RestoreTableResponseTypeDef](./type_defs.md#restoretableresponsetypedef) 


```python
# restore_table method usage example with argument unpacking

kwargs: RestoreTableRequestTypeDef = {  # (1)
    "sourceKeyspaceName": ...,
    "sourceTableName": ...,
    "targetKeyspaceName": ...,
    "targetTableName": ...,
}

parent.restore_table(**kwargs)
```

1. See [:material-code-braces: RestoreTableRequestTypeDef](./type_defs.md#restoretablerequesttypedef) 

### tag\_resource

Associates a set of tags with a Amazon Keyspaces resource.

Type annotations and code completion for `#!python session.create_client("keyspaces").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/tag_resource.html)

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

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes the association of tags from a Amazon Keyspaces resource.

Type annotations and code completion for `#!python session.create_client("keyspaces").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_keyspace

Adds a new Amazon Web Services Region to the keyspace.

Type annotations and code completion for `#!python session.create_client("keyspaces").update_keyspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/update_keyspace.html)

```python
# update_keyspace method definition

await def update_keyspace(
    self,
    *,
    keyspaceName: str,
    replicationSpecification: ReplicationSpecificationTypeDef,  # (1)
    clientSideTimestamps: ClientSideTimestampsTypeDef = ...,  # (2)
) -> UpdateKeyspaceResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ReplicationSpecificationTypeDef](./type_defs.md#replicationspecificationtypedef) 
2. See [:material-code-braces: ClientSideTimestampsTypeDef](./type_defs.md#clientsidetimestampstypedef) 
3. See [:material-code-braces: UpdateKeyspaceResponseTypeDef](./type_defs.md#updatekeyspaceresponsetypedef) 


```python
# update_keyspace method usage example with argument unpacking

kwargs: UpdateKeyspaceRequestTypeDef = {  # (1)
    "keyspaceName": ...,
    "replicationSpecification": ...,
}

parent.update_keyspace(**kwargs)
```

1. See [:material-code-braces: UpdateKeyspaceRequestTypeDef](./type_defs.md#updatekeyspacerequesttypedef) 

### update\_table

Adds new columns to the table or updates one of the table's settings, for
example capacity mode, auto scaling, encryption, point-in-time recovery, or ttl
settings.

Type annotations and code completion for `#!python session.create_client("keyspaces").update_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces/client/update_table.html)

```python
# update_table method definition

await def update_table(
    self,
    *,
    keyspaceName: str,
    tableName: str,
    addColumns: Sequence[ColumnDefinitionTypeDef] = ...,  # (1)
    capacitySpecification: CapacitySpecificationTypeDef = ...,  # (2)
    encryptionSpecification: EncryptionSpecificationTypeDef = ...,  # (3)
    pointInTimeRecovery: PointInTimeRecoveryTypeDef = ...,  # (4)
    ttl: TimeToLiveTypeDef = ...,  # (5)
    defaultTimeToLive: int = ...,
    clientSideTimestamps: ClientSideTimestampsTypeDef = ...,  # (6)
    autoScalingSpecification: AutoScalingSpecificationTypeDef = ...,  # (7)
    replicaSpecifications: Sequence[ReplicaSpecificationTypeDef] = ...,  # (8)
) -> UpdateTableResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: ColumnDefinitionTypeDef](./type_defs.md#columndefinitiontypedef) 
2. See [:material-code-braces: CapacitySpecificationTypeDef](./type_defs.md#capacityspecificationtypedef) 
3. See [:material-code-braces: EncryptionSpecificationTypeDef](./type_defs.md#encryptionspecificationtypedef) 
4. See [:material-code-braces: PointInTimeRecoveryTypeDef](./type_defs.md#pointintimerecoverytypedef) 
5. See [:material-code-braces: TimeToLiveTypeDef](./type_defs.md#timetolivetypedef) 
6. See [:material-code-braces: ClientSideTimestampsTypeDef](./type_defs.md#clientsidetimestampstypedef) 
7. See [:material-code-braces: AutoScalingSpecificationTypeDef](./type_defs.md#autoscalingspecificationtypedef) 
8. See [:material-code-braces: ReplicaSpecificationTypeDef](./type_defs.md#replicaspecificationtypedef) 
9. See [:material-code-braces: UpdateTableResponseTypeDef](./type_defs.md#updatetableresponsetypedef) 


```python
# update_table method usage example with argument unpacking

kwargs: UpdateTableRequestTypeDef = {  # (1)
    "keyspaceName": ...,
    "tableName": ...,
}

parent.update_table(**kwargs)
```

1. See [:material-code-braces: UpdateTableRequestTypeDef](./type_defs.md#updatetablerequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("keyspaces").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("keyspaces").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client)

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

Type annotations and code completion for `#!python session.create_client("keyspaces").get_paginator` method with overloads.

- `client.get_paginator("list_keyspaces")` -> [ListKeyspacesPaginator](./paginators.md#listkeyspacespaginator)
- `client.get_paginator("list_tables")` -> [ListTablesPaginator](./paginators.md#listtablespaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- `client.get_paginator("list_types")` -> [ListTypesPaginator](./paginators.md#listtypespaginator)



