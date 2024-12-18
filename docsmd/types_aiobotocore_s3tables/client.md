# S3TablesClient

> [Index](../README.md) > [S3Tables](./README.md) > S3TablesClient

!!! note ""

    Auto-generated documentation for [S3Tables](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables.html#s3tables)
    type annotations stubs module [types-aiobotocore-s3tables](https://pypi.org/project/types-aiobotocore-s3tables/).

## S3TablesClient

Type annotations and code completion for `#!python session.create_client("s3tables")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables.html#S3Tables.Client)

```python
# S3TablesClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_s3tables.client import S3TablesClient

session = get_session()
async with session.create_client("s3tables") as client:
    client: S3TablesClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("s3tables").exceptions` structure.

```python
# S3TablesClient.exceptions usage example

async with session.create_client("s3tables") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.ForbiddenException,
        client.InternalServerErrorException,
        client.NotFoundException,
        client.TooManyRequestsException,
    ) as e:
        print(e)
```

```python
# S3TablesClient usage type checking example

from types_aiobotocore_s3tables.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("s3tables").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("s3tables").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/generate_presigned_url.html)

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



Type annotations and code completion for `#!python session.create_client("s3tables").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_namespace

Creates a namespace.

Type annotations and code completion for `#!python session.create_client("s3tables").create_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/create_namespace.html)

```python
# create_namespace method definition

await def create_namespace(
    self,
    *,
    tableBucketARN: str,
    namespace: Sequence[str],
) -> CreateNamespaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateNamespaceResponseTypeDef](./type_defs.md#createnamespaceresponsetypedef) 


```python
# create_namespace method usage example with argument unpacking

kwargs: CreateNamespaceRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
}

parent.create_namespace(**kwargs)
```

1. See [:material-code-braces: CreateNamespaceRequestRequestTypeDef](./type_defs.md#createnamespacerequestrequesttypedef) 

### create\_table

Creates a new table associated with the given namespace in a table bucket.

Type annotations and code completion for `#!python session.create_client("s3tables").create_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/create_table.html)

```python
# create_table method definition

await def create_table(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
    name: str,
    format: OpenTableFormatType,  # (1)
) -> CreateTableResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OpenTableFormatType](./literals.md#opentableformattype) 
2. See [:material-code-braces: CreateTableResponseTypeDef](./type_defs.md#createtableresponsetypedef) 


```python
# create_table method usage example with argument unpacking

kwargs: CreateTableRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
    "name": ...,
    "format": ...,
}

parent.create_table(**kwargs)
```

1. See [:material-code-braces: CreateTableRequestRequestTypeDef](./type_defs.md#createtablerequestrequesttypedef) 

### create\_table\_bucket

Creates a table bucket.

Type annotations and code completion for `#!python session.create_client("s3tables").create_table_bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/create_table_bucket.html)

```python
# create_table_bucket method definition

await def create_table_bucket(
    self,
    *,
    name: str,
) -> CreateTableBucketResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateTableBucketResponseTypeDef](./type_defs.md#createtablebucketresponsetypedef) 


```python
# create_table_bucket method usage example with argument unpacking

kwargs: CreateTableBucketRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_table_bucket(**kwargs)
```

1. See [:material-code-braces: CreateTableBucketRequestRequestTypeDef](./type_defs.md#createtablebucketrequestrequesttypedef) 

### delete\_namespace

Deletes a namespace.

Type annotations and code completion for `#!python session.create_client("s3tables").delete_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/delete_namespace.html)

```python
# delete_namespace method definition

await def delete_namespace(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_namespace method usage example with argument unpacking

kwargs: DeleteNamespaceRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
}

parent.delete_namespace(**kwargs)
```

1. See [:material-code-braces: DeleteNamespaceRequestRequestTypeDef](./type_defs.md#deletenamespacerequestrequesttypedef) 

### delete\_table

Deletes a table.

Type annotations and code completion for `#!python session.create_client("s3tables").delete_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/delete_table.html)

```python
# delete_table method definition

await def delete_table(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
    name: str,
    versionToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_table method usage example with argument unpacking

kwargs: DeleteTableRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
    "name": ...,
}

parent.delete_table(**kwargs)
```

1. See [:material-code-braces: DeleteTableRequestRequestTypeDef](./type_defs.md#deletetablerequestrequesttypedef) 

### delete\_table\_bucket

Deletes a table bucket.

Type annotations and code completion for `#!python session.create_client("s3tables").delete_table_bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/delete_table_bucket.html)

```python
# delete_table_bucket method definition

await def delete_table_bucket(
    self,
    *,
    tableBucketARN: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_table_bucket method usage example with argument unpacking

kwargs: DeleteTableBucketRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
}

parent.delete_table_bucket(**kwargs)
```

1. See [:material-code-braces: DeleteTableBucketRequestRequestTypeDef](./type_defs.md#deletetablebucketrequestrequesttypedef) 

### delete\_table\_bucket\_policy

Deletes a table bucket policy.

Type annotations and code completion for `#!python session.create_client("s3tables").delete_table_bucket_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/delete_table_bucket_policy.html)

```python
# delete_table_bucket_policy method definition

await def delete_table_bucket_policy(
    self,
    *,
    tableBucketARN: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_table_bucket_policy method usage example with argument unpacking

kwargs: DeleteTableBucketPolicyRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
}

parent.delete_table_bucket_policy(**kwargs)
```

1. See [:material-code-braces: DeleteTableBucketPolicyRequestRequestTypeDef](./type_defs.md#deletetablebucketpolicyrequestrequesttypedef) 

### delete\_table\_policy

Deletes a table policy.

Type annotations and code completion for `#!python session.create_client("s3tables").delete_table_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/delete_table_policy.html)

```python
# delete_table_policy method definition

await def delete_table_policy(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
    name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_table_policy method usage example with argument unpacking

kwargs: DeleteTablePolicyRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
    "name": ...,
}

parent.delete_table_policy(**kwargs)
```

1. See [:material-code-braces: DeleteTablePolicyRequestRequestTypeDef](./type_defs.md#deletetablepolicyrequestrequesttypedef) 

### get\_namespace

Gets details about a namespace.

Type annotations and code completion for `#!python session.create_client("s3tables").get_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/get_namespace.html)

```python
# get_namespace method definition

await def get_namespace(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
) -> GetNamespaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetNamespaceResponseTypeDef](./type_defs.md#getnamespaceresponsetypedef) 


```python
# get_namespace method usage example with argument unpacking

kwargs: GetNamespaceRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
}

parent.get_namespace(**kwargs)
```

1. See [:material-code-braces: GetNamespaceRequestRequestTypeDef](./type_defs.md#getnamespacerequestrequesttypedef) 

### get\_table

Gets details about a table.

Type annotations and code completion for `#!python session.create_client("s3tables").get_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/get_table.html)

```python
# get_table method definition

await def get_table(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
    name: str,
) -> GetTableResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableResponseTypeDef](./type_defs.md#gettableresponsetypedef) 


```python
# get_table method usage example with argument unpacking

kwargs: GetTableRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
    "name": ...,
}

parent.get_table(**kwargs)
```

1. See [:material-code-braces: GetTableRequestRequestTypeDef](./type_defs.md#gettablerequestrequesttypedef) 

### get\_table\_bucket

Gets details on a table bucket.

Type annotations and code completion for `#!python session.create_client("s3tables").get_table_bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/get_table_bucket.html)

```python
# get_table_bucket method definition

await def get_table_bucket(
    self,
    *,
    tableBucketARN: str,
) -> GetTableBucketResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableBucketResponseTypeDef](./type_defs.md#gettablebucketresponsetypedef) 


```python
# get_table_bucket method usage example with argument unpacking

kwargs: GetTableBucketRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
}

parent.get_table_bucket(**kwargs)
```

1. See [:material-code-braces: GetTableBucketRequestRequestTypeDef](./type_defs.md#gettablebucketrequestrequesttypedef) 

### get\_table\_bucket\_maintenance\_configuration

Gets details about a maintenance configuration for a given table bucket.

Type annotations and code completion for `#!python session.create_client("s3tables").get_table_bucket_maintenance_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/get_table_bucket_maintenance_configuration.html)

```python
# get_table_bucket_maintenance_configuration method definition

await def get_table_bucket_maintenance_configuration(
    self,
    *,
    tableBucketARN: str,
) -> GetTableBucketMaintenanceConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableBucketMaintenanceConfigurationResponseTypeDef](./type_defs.md#gettablebucketmaintenanceconfigurationresponsetypedef) 


```python
# get_table_bucket_maintenance_configuration method usage example with argument unpacking

kwargs: GetTableBucketMaintenanceConfigurationRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
}

parent.get_table_bucket_maintenance_configuration(**kwargs)
```

1. See [:material-code-braces: GetTableBucketMaintenanceConfigurationRequestRequestTypeDef](./type_defs.md#gettablebucketmaintenanceconfigurationrequestrequesttypedef) 

### get\_table\_bucket\_policy

Gets details about a table bucket policy.

Type annotations and code completion for `#!python session.create_client("s3tables").get_table_bucket_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/get_table_bucket_policy.html)

```python
# get_table_bucket_policy method definition

await def get_table_bucket_policy(
    self,
    *,
    tableBucketARN: str,
) -> GetTableBucketPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableBucketPolicyResponseTypeDef](./type_defs.md#gettablebucketpolicyresponsetypedef) 


```python
# get_table_bucket_policy method usage example with argument unpacking

kwargs: GetTableBucketPolicyRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
}

parent.get_table_bucket_policy(**kwargs)
```

1. See [:material-code-braces: GetTableBucketPolicyRequestRequestTypeDef](./type_defs.md#gettablebucketpolicyrequestrequesttypedef) 

### get\_table\_maintenance\_configuration

Gets details about the maintenance configuration of a table.

Type annotations and code completion for `#!python session.create_client("s3tables").get_table_maintenance_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/get_table_maintenance_configuration.html)

```python
# get_table_maintenance_configuration method definition

await def get_table_maintenance_configuration(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
    name: str,
) -> GetTableMaintenanceConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableMaintenanceConfigurationResponseTypeDef](./type_defs.md#gettablemaintenanceconfigurationresponsetypedef) 


```python
# get_table_maintenance_configuration method usage example with argument unpacking

kwargs: GetTableMaintenanceConfigurationRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
    "name": ...,
}

parent.get_table_maintenance_configuration(**kwargs)
```

1. See [:material-code-braces: GetTableMaintenanceConfigurationRequestRequestTypeDef](./type_defs.md#gettablemaintenanceconfigurationrequestrequesttypedef) 

### get\_table\_maintenance\_job\_status

Gets the status of a maintenance job for a table.

Type annotations and code completion for `#!python session.create_client("s3tables").get_table_maintenance_job_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/get_table_maintenance_job_status.html)

```python
# get_table_maintenance_job_status method definition

await def get_table_maintenance_job_status(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
    name: str,
) -> GetTableMaintenanceJobStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableMaintenanceJobStatusResponseTypeDef](./type_defs.md#gettablemaintenancejobstatusresponsetypedef) 


```python
# get_table_maintenance_job_status method usage example with argument unpacking

kwargs: GetTableMaintenanceJobStatusRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
    "name": ...,
}

parent.get_table_maintenance_job_status(**kwargs)
```

1. See [:material-code-braces: GetTableMaintenanceJobStatusRequestRequestTypeDef](./type_defs.md#gettablemaintenancejobstatusrequestrequesttypedef) 

### get\_table\_metadata\_location

Gets the location of the table metadata.

Type annotations and code completion for `#!python session.create_client("s3tables").get_table_metadata_location` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/get_table_metadata_location.html)

```python
# get_table_metadata_location method definition

await def get_table_metadata_location(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
    name: str,
) -> GetTableMetadataLocationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableMetadataLocationResponseTypeDef](./type_defs.md#gettablemetadatalocationresponsetypedef) 


```python
# get_table_metadata_location method usage example with argument unpacking

kwargs: GetTableMetadataLocationRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
    "name": ...,
}

parent.get_table_metadata_location(**kwargs)
```

1. See [:material-code-braces: GetTableMetadataLocationRequestRequestTypeDef](./type_defs.md#gettablemetadatalocationrequestrequesttypedef) 

### get\_table\_policy

Gets details about a table policy.

Type annotations and code completion for `#!python session.create_client("s3tables").get_table_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/get_table_policy.html)

```python
# get_table_policy method definition

await def get_table_policy(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
    name: str,
) -> GetTablePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTablePolicyResponseTypeDef](./type_defs.md#gettablepolicyresponsetypedef) 


```python
# get_table_policy method usage example with argument unpacking

kwargs: GetTablePolicyRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
    "name": ...,
}

parent.get_table_policy(**kwargs)
```

1. See [:material-code-braces: GetTablePolicyRequestRequestTypeDef](./type_defs.md#gettablepolicyrequestrequesttypedef) 

### list\_namespaces

Lists the namespaces within a table bucket.

Type annotations and code completion for `#!python session.create_client("s3tables").list_namespaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/list_namespaces.html)

```python
# list_namespaces method definition

await def list_namespaces(
    self,
    *,
    tableBucketARN: str,
    prefix: str = ...,
    continuationToken: str = ...,
    maxNamespaces: int = ...,
) -> ListNamespacesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListNamespacesResponseTypeDef](./type_defs.md#listnamespacesresponsetypedef) 


```python
# list_namespaces method usage example with argument unpacking

kwargs: ListNamespacesRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
}

parent.list_namespaces(**kwargs)
```

1. See [:material-code-braces: ListNamespacesRequestRequestTypeDef](./type_defs.md#listnamespacesrequestrequesttypedef) 

### list\_table\_buckets

Lists table buckets for your account.

Type annotations and code completion for `#!python session.create_client("s3tables").list_table_buckets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/list_table_buckets.html)

```python
# list_table_buckets method definition

await def list_table_buckets(
    self,
    *,
    prefix: str = ...,
    continuationToken: str = ...,
    maxBuckets: int = ...,
) -> ListTableBucketsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTableBucketsResponseTypeDef](./type_defs.md#listtablebucketsresponsetypedef) 


```python
# list_table_buckets method usage example with argument unpacking

kwargs: ListTableBucketsRequestRequestTypeDef = {  # (1)
    "prefix": ...,
}

parent.list_table_buckets(**kwargs)
```

1. See [:material-code-braces: ListTableBucketsRequestRequestTypeDef](./type_defs.md#listtablebucketsrequestrequesttypedef) 

### list\_tables

List tables in the given table bucket.

Type annotations and code completion for `#!python session.create_client("s3tables").list_tables` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/list_tables.html)

```python
# list_tables method definition

await def list_tables(
    self,
    *,
    tableBucketARN: str,
    namespace: str = ...,
    prefix: str = ...,
    continuationToken: str = ...,
    maxTables: int = ...,
) -> ListTablesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef) 


```python
# list_tables method usage example with argument unpacking

kwargs: ListTablesRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
}

parent.list_tables(**kwargs)
```

1. See [:material-code-braces: ListTablesRequestRequestTypeDef](./type_defs.md#listtablesrequestrequesttypedef) 

### put\_table\_bucket\_maintenance\_configuration

Creates a new maintenance configuration or replaces an existing maintenance
configuration for a table bucket.

Type annotations and code completion for `#!python session.create_client("s3tables").put_table_bucket_maintenance_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/put_table_bucket_maintenance_configuration.html)

```python
# put_table_bucket_maintenance_configuration method definition

await def put_table_bucket_maintenance_configuration(
    self,
    *,
    tableBucketARN: str,
    type: TableBucketMaintenanceTypeType,  # (1)
    value: TableBucketMaintenanceConfigurationValueTypeDef,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TableBucketMaintenanceTypeType](./literals.md#tablebucketmaintenancetypetype) 
2. See [:material-code-braces: TableBucketMaintenanceConfigurationValueTypeDef](./type_defs.md#tablebucketmaintenanceconfigurationvaluetypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_table_bucket_maintenance_configuration method usage example with argument unpacking

kwargs: PutTableBucketMaintenanceConfigurationRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "type": ...,
    "value": ...,
}

parent.put_table_bucket_maintenance_configuration(**kwargs)
```

1. See [:material-code-braces: PutTableBucketMaintenanceConfigurationRequestRequestTypeDef](./type_defs.md#puttablebucketmaintenanceconfigurationrequestrequesttypedef) 

### put\_table\_bucket\_policy

Creates a new maintenance configuration or replaces an existing table bucket
policy for a table bucket.

Type annotations and code completion for `#!python session.create_client("s3tables").put_table_bucket_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/put_table_bucket_policy.html)

```python
# put_table_bucket_policy method definition

await def put_table_bucket_policy(
    self,
    *,
    tableBucketARN: str,
    resourcePolicy: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_table_bucket_policy method usage example with argument unpacking

kwargs: PutTableBucketPolicyRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "resourcePolicy": ...,
}

parent.put_table_bucket_policy(**kwargs)
```

1. See [:material-code-braces: PutTableBucketPolicyRequestRequestTypeDef](./type_defs.md#puttablebucketpolicyrequestrequesttypedef) 

### put\_table\_maintenance\_configuration

Creates a new maintenance configuration or replaces an existing maintenance
configuration for a table.

Type annotations and code completion for `#!python session.create_client("s3tables").put_table_maintenance_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/put_table_maintenance_configuration.html)

```python
# put_table_maintenance_configuration method definition

await def put_table_maintenance_configuration(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
    name: str,
    type: TableMaintenanceTypeType,  # (1)
    value: TableMaintenanceConfigurationValueTypeDef,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TableMaintenanceTypeType](./literals.md#tablemaintenancetypetype) 
2. See [:material-code-braces: TableMaintenanceConfigurationValueTypeDef](./type_defs.md#tablemaintenanceconfigurationvaluetypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_table_maintenance_configuration method usage example with argument unpacking

kwargs: PutTableMaintenanceConfigurationRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
    "name": ...,
    "type": ...,
    "value": ...,
}

parent.put_table_maintenance_configuration(**kwargs)
```

1. See [:material-code-braces: PutTableMaintenanceConfigurationRequestRequestTypeDef](./type_defs.md#puttablemaintenanceconfigurationrequestrequesttypedef) 

### put\_table\_policy

Creates a new maintenance configuration or replaces an existing table policy
for a table.

Type annotations and code completion for `#!python session.create_client("s3tables").put_table_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/put_table_policy.html)

```python
# put_table_policy method definition

await def put_table_policy(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
    name: str,
    resourcePolicy: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_table_policy method usage example with argument unpacking

kwargs: PutTablePolicyRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
    "name": ...,
    "resourcePolicy": ...,
}

parent.put_table_policy(**kwargs)
```

1. See [:material-code-braces: PutTablePolicyRequestRequestTypeDef](./type_defs.md#puttablepolicyrequestrequesttypedef) 

### rename\_table

Renames a table or a namespace.

Type annotations and code completion for `#!python session.create_client("s3tables").rename_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/rename_table.html)

```python
# rename_table method definition

await def rename_table(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
    name: str,
    newNamespaceName: str = ...,
    newName: str = ...,
    versionToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# rename_table method usage example with argument unpacking

kwargs: RenameTableRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
    "name": ...,
}

parent.rename_table(**kwargs)
```

1. See [:material-code-braces: RenameTableRequestRequestTypeDef](./type_defs.md#renametablerequestrequesttypedef) 

### update\_table\_metadata\_location

Updates the metadata location for a table.

Type annotations and code completion for `#!python session.create_client("s3tables").update_table_metadata_location` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/client/update_table_metadata_location.html)

```python
# update_table_metadata_location method definition

await def update_table_metadata_location(
    self,
    *,
    tableBucketARN: str,
    namespace: str,
    name: str,
    versionToken: str,
    metadataLocation: str,
) -> UpdateTableMetadataLocationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateTableMetadataLocationResponseTypeDef](./type_defs.md#updatetablemetadatalocationresponsetypedef) 


```python
# update_table_metadata_location method usage example with argument unpacking

kwargs: UpdateTableMetadataLocationRequestRequestTypeDef = {  # (1)
    "tableBucketARN": ...,
    "namespace": ...,
    "name": ...,
    "versionToken": ...,
    "metadataLocation": ...,
}

parent.update_table_metadata_location(**kwargs)
```

1. See [:material-code-braces: UpdateTableMetadataLocationRequestRequestTypeDef](./type_defs.md#updatetablemetadatalocationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("s3tables").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables.html#S3Tables.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "S3TablesClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("s3tables").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables.html#S3Tables.Client)

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

Type annotations and code completion for `#!python session.create_client("s3tables").get_paginator` method with overloads.

- `client.get_paginator("list_namespaces")` -> [ListNamespacesPaginator](./paginators.md#listnamespacespaginator)
- `client.get_paginator("list_table_buckets")` -> [ListTableBucketsPaginator](./paginators.md#listtablebucketspaginator)
- `client.get_paginator("list_tables")` -> [ListTablesPaginator](./paginators.md#listtablespaginator)



