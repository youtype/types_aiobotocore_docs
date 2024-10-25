# TimestreamInfluxDBClient

> [Index](../README.md) > [TimestreamInfluxDB](./README.md) > TimestreamInfluxDBClient

!!! note ""

    Auto-generated documentation for [TimestreamInfluxDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB)
    type annotations stubs module [types-aiobotocore-timestream-influxdb](https://pypi.org/project/types-aiobotocore-timestream-influxdb/).

## TimestreamInfluxDBClient

Type annotations and code completion for `#!python session.create_client("timestream-influxdb")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client)

```python
# TimestreamInfluxDBClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_timestream_influxdb.client import TimestreamInfluxDBClient

session = get_session()
async with session.create_client("timestream-influxdb") as client:
    client: TimestreamInfluxDBClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("timestream-influxdb").exceptions` structure.

```python
# TimestreamInfluxDBClient.exceptions usage example

async with session.create_client("timestream-influxdb") as client:
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
# TimestreamInfluxDBClient usage type checking example

from types_aiobotocore_timestream_influxdb.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_db\_instance

Creates a new Timestream for InfluxDB DB instance.

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").create_db_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.create_db_instance)

```python
# create_db_instance method definition

await def create_db_instance(
    self,
    *,
    name: str,
    password: str,
    dbInstanceType: DbInstanceTypeType,  # (1)
    vpcSubnetIds: Sequence[str],
    vpcSecurityGroupIds: Sequence[str],
    allocatedStorage: int,
    username: str = ...,
    organization: str = ...,
    bucket: str = ...,
    publiclyAccessible: bool = ...,
    dbStorageType: DbStorageTypeType = ...,  # (2)
    dbParameterGroupIdentifier: str = ...,
    deploymentType: DeploymentTypeType = ...,  # (3)
    logDeliveryConfiguration: LogDeliveryConfigurationTypeDef = ...,  # (4)
    tags: Mapping[str, str] = ...,
    port: int = ...,
) -> CreateDbInstanceOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
2. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
3. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
4. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
5. See [:material-code-braces: CreateDbInstanceOutputTypeDef](./type_defs.md#createdbinstanceoutputtypedef) 


```python
# create_db_instance method usage example with argument unpacking

kwargs: CreateDbInstanceInputRequestTypeDef = {  # (1)
    "name": ...,
    "password": ...,
    "dbInstanceType": ...,
    "vpcSubnetIds": ...,
    "vpcSecurityGroupIds": ...,
    "allocatedStorage": ...,
}

parent.create_db_instance(**kwargs)
```

1. See [:material-code-braces: CreateDbInstanceInputRequestTypeDef](./type_defs.md#createdbinstanceinputrequesttypedef) 

### create\_db\_parameter\_group

Creates a new Timestream for InfluxDB DB parameter group to associate with DB
instances.

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").create_db_parameter_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.create_db_parameter_group)

```python
# create_db_parameter_group method definition

await def create_db_parameter_group(
    self,
    *,
    name: str,
    description: str = ...,
    parameters: ParametersTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateDbParameterGroupOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
2. See [:material-code-braces: CreateDbParameterGroupOutputTypeDef](./type_defs.md#createdbparametergroupoutputtypedef) 


```python
# create_db_parameter_group method usage example with argument unpacking

kwargs: CreateDbParameterGroupInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_db_parameter_group(**kwargs)
```

1. See [:material-code-braces: CreateDbParameterGroupInputRequestTypeDef](./type_defs.md#createdbparametergroupinputrequesttypedef) 

### delete\_db\_instance

Deletes a Timestream for InfluxDB DB instance.

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").delete_db_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.delete_db_instance)

```python
# delete_db_instance method definition

await def delete_db_instance(
    self,
    *,
    identifier: str,
) -> DeleteDbInstanceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDbInstanceOutputTypeDef](./type_defs.md#deletedbinstanceoutputtypedef) 


```python
# delete_db_instance method usage example with argument unpacking

kwargs: DeleteDbInstanceInputRequestTypeDef = {  # (1)
    "identifier": ...,
}

parent.delete_db_instance(**kwargs)
```

1. See [:material-code-braces: DeleteDbInstanceInputRequestTypeDef](./type_defs.md#deletedbinstanceinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.generate_presigned_url)

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


### get\_db\_instance

Returns a Timestream for InfluxDB DB instance.

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").get_db_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.get_db_instance)

```python
# get_db_instance method definition

await def get_db_instance(
    self,
    *,
    identifier: str,
) -> GetDbInstanceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDbInstanceOutputTypeDef](./type_defs.md#getdbinstanceoutputtypedef) 


```python
# get_db_instance method usage example with argument unpacking

kwargs: GetDbInstanceInputRequestTypeDef = {  # (1)
    "identifier": ...,
}

parent.get_db_instance(**kwargs)
```

1. See [:material-code-braces: GetDbInstanceInputRequestTypeDef](./type_defs.md#getdbinstanceinputrequesttypedef) 

### get\_db\_parameter\_group

Returns a Timestream for InfluxDB DB parameter group.

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").get_db_parameter_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.get_db_parameter_group)

```python
# get_db_parameter_group method definition

await def get_db_parameter_group(
    self,
    *,
    identifier: str,
) -> GetDbParameterGroupOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDbParameterGroupOutputTypeDef](./type_defs.md#getdbparametergroupoutputtypedef) 


```python
# get_db_parameter_group method usage example with argument unpacking

kwargs: GetDbParameterGroupInputRequestTypeDef = {  # (1)
    "identifier": ...,
}

parent.get_db_parameter_group(**kwargs)
```

1. See [:material-code-braces: GetDbParameterGroupInputRequestTypeDef](./type_defs.md#getdbparametergroupinputrequesttypedef) 

### list\_db\_instances

Returns a list of Timestream for InfluxDB DB instances.

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").list_db_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.list_db_instances)

```python
# list_db_instances method definition

await def list_db_instances(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDbInstancesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDbInstancesOutputTypeDef](./type_defs.md#listdbinstancesoutputtypedef) 


```python
# list_db_instances method usage example with argument unpacking

kwargs: ListDbInstancesInputRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_db_instances(**kwargs)
```

1. See [:material-code-braces: ListDbInstancesInputRequestTypeDef](./type_defs.md#listdbinstancesinputrequesttypedef) 

### list\_db\_parameter\_groups

Returns a list of Timestream for InfluxDB DB parameter groups.

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").list_db_parameter_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.list_db_parameter_groups)

```python
# list_db_parameter_groups method definition

await def list_db_parameter_groups(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDbParameterGroupsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDbParameterGroupsOutputTypeDef](./type_defs.md#listdbparametergroupsoutputtypedef) 


```python
# list_db_parameter_groups method usage example with argument unpacking

kwargs: ListDbParameterGroupsInputRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_db_parameter_groups(**kwargs)
```

1. See [:material-code-braces: ListDbParameterGroupsInputRequestTypeDef](./type_defs.md#listdbparametergroupsinputrequesttypedef) 

### list\_tags\_for\_resource

A list of tags applied to the resource.

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.list_tags_for_resource)

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

Tags are composed of a Key/Value pairs.

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


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

Removes the tag from the specified resource.

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_db\_instance

Updates a Timestream for InfluxDB DB instance.

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").update_db_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.update_db_instance)

```python
# update_db_instance method definition

await def update_db_instance(
    self,
    *,
    identifier: str,
    logDeliveryConfiguration: LogDeliveryConfigurationTypeDef = ...,  # (1)
    dbParameterGroupIdentifier: str = ...,
    port: int = ...,
    dbInstanceType: DbInstanceTypeType = ...,  # (2)
    deploymentType: DeploymentTypeType = ...,  # (3)
) -> UpdateDbInstanceOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
2. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
3. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
4. See [:material-code-braces: UpdateDbInstanceOutputTypeDef](./type_defs.md#updatedbinstanceoutputtypedef) 


```python
# update_db_instance method usage example with argument unpacking

kwargs: UpdateDbInstanceInputRequestTypeDef = {  # (1)
    "identifier": ...,
}

parent.update_db_instance(**kwargs)
```

1. See [:material-code-braces: UpdateDbInstanceInputRequestTypeDef](./type_defs.md#updatedbinstanceinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("timestream-influxdb").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "TimestreamInfluxDBClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("timestream-influxdb").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").get_paginator` method with overloads.

- `client.get_paginator("list_db_instances")` -> [ListDbInstancesPaginator](./paginators.md#listdbinstancespaginator)
- `client.get_paginator("list_db_parameter_groups")` -> [ListDbParameterGroupsPaginator](./paginators.md#listdbparametergroupspaginator)



