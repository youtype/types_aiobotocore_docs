# S3VectorsClient

> [Index](../README.md) > [S3Vectors](./README.md) > S3VectorsClient

!!! note ""

    Auto-generated documentation for [S3Vectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors.html#s3vectors)
    type annotations stubs module [types-aiobotocore-s3vectors](https://pypi.org/project/types-aiobotocore-s3vectors/).

## S3VectorsClient

Type annotations and code completion for `#!python session.create_client("s3vectors")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors.html#S3Vectors.Client)

```python
# S3VectorsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_s3vectors.client import S3VectorsClient

session = get_session()
async with session.create_client("s3vectors") as client:
    client: S3VectorsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("s3vectors").exceptions` structure.

```python
# S3VectorsClient.exceptions usage example

async with session.create_client("s3vectors") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.KmsDisabledException,
        client.KmsInvalidKeyUsageException,
        client.KmsInvalidStateException,
        client.KmsNotFoundException,
        client.NotFoundException,
        client.ServiceQuotaExceededException,
        client.ServiceUnavailableException,
        client.TooManyRequestsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# S3VectorsClient usage type checking example

from types_aiobotocore_s3vectors.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("s3vectors").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("s3vectors").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/generate_presigned_url.html)

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


### create\_index

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").create_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/create_index.html)

```python
# create_index method definition

await def create_index(
    self,
    *,
    indexName: str,
    dataType: DataTypeType,  # (1)
    dimension: int,
    distanceMetric: DistanceMetricType,  # (2)
    vectorBucketName: str = ...,
    vectorBucketArn: str = ...,
    metadataConfiguration: MetadataConfigurationUnionTypeDef = ...,  # (3)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: DataTypeType](./literals.md#datatypetype)
2. See [:material-code-brackets: DistanceMetricType](./literals.md#distancemetrictype)
3. See [:material-code-braces: MetadataConfigurationUnionTypeDef](#metadataconfigurationuniontypedef)


```python
# create_index method usage example with argument unpacking

kwargs: CreateIndexInputTypeDef = {  # (1)
    "indexName": ...,
    "dataType": ...,
    "dimension": ...,
    "distanceMetric": ...,
}

parent.create_index(**kwargs)
```

1. See [:material-code-braces: CreateIndexInputTypeDef](./type_defs.md#createindexinputtypedef)

### create\_vector\_bucket

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").create_vector_bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/create_vector_bucket.html)

```python
# create_vector_bucket method definition

await def create_vector_bucket(
    self,
    *,
    vectorBucketName: str,
    encryptionConfiguration: EncryptionConfigurationTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)


```python
# create_vector_bucket method usage example with argument unpacking

kwargs: CreateVectorBucketInputTypeDef = {  # (1)
    "vectorBucketName": ...,
}

parent.create_vector_bucket(**kwargs)
```

1. See [:material-code-braces: CreateVectorBucketInputTypeDef](./type_defs.md#createvectorbucketinputtypedef)

### delete\_index

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").delete_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/delete_index.html)

```python
# delete_index method definition

await def delete_index(
    self,
    *,
    vectorBucketName: str = ...,
    indexName: str = ...,
    indexArn: str = ...,
) -> Dict[str, Any]:
    ...
```

```python
# delete_index method usage example with argument unpacking

kwargs: DeleteIndexInputTypeDef = {  # (1)
    "vectorBucketName": ...,
}

parent.delete_index(**kwargs)
```

1. See [:material-code-braces: DeleteIndexInputTypeDef](./type_defs.md#deleteindexinputtypedef)

### delete\_vector\_bucket

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").delete_vector_bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/delete_vector_bucket.html)

```python
# delete_vector_bucket method definition

await def delete_vector_bucket(
    self,
    *,
    vectorBucketName: str = ...,
    vectorBucketArn: str = ...,
) -> Dict[str, Any]:
    ...
```

```python
# delete_vector_bucket method usage example with argument unpacking

kwargs: DeleteVectorBucketInputTypeDef = {  # (1)
    "vectorBucketName": ...,
}

parent.delete_vector_bucket(**kwargs)
```

1. See [:material-code-braces: DeleteVectorBucketInputTypeDef](./type_defs.md#deletevectorbucketinputtypedef)

### delete\_vector\_bucket\_policy

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").delete_vector_bucket_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/delete_vector_bucket_policy.html)

```python
# delete_vector_bucket_policy method definition

await def delete_vector_bucket_policy(
    self,
    *,
    vectorBucketName: str = ...,
    vectorBucketArn: str = ...,
) -> Dict[str, Any]:
    ...
```

```python
# delete_vector_bucket_policy method usage example with argument unpacking

kwargs: DeleteVectorBucketPolicyInputTypeDef = {  # (1)
    "vectorBucketName": ...,
}

parent.delete_vector_bucket_policy(**kwargs)
```

1. See [:material-code-braces: DeleteVectorBucketPolicyInputTypeDef](./type_defs.md#deletevectorbucketpolicyinputtypedef)

### delete\_vectors

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").delete_vectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/delete_vectors.html)

```python
# delete_vectors method definition

await def delete_vectors(
    self,
    *,
    keys: Sequence[str],
    vectorBucketName: str = ...,
    indexName: str = ...,
    indexArn: str = ...,
) -> Dict[str, Any]:
    ...
```

```python
# delete_vectors method usage example with argument unpacking

kwargs: DeleteVectorsInputTypeDef = {  # (1)
    "keys": ...,
}

parent.delete_vectors(**kwargs)
```

1. See [:material-code-braces: DeleteVectorsInputTypeDef](./type_defs.md#deletevectorsinputtypedef)

### get\_index

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").get_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/get_index.html)

```python
# get_index method definition

await def get_index(
    self,
    *,
    vectorBucketName: str = ...,
    indexName: str = ...,
    indexArn: str = ...,
) -> GetIndexOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIndexOutputTypeDef](./type_defs.md#getindexoutputtypedef)


```python
# get_index method usage example with argument unpacking

kwargs: GetIndexInputTypeDef = {  # (1)
    "vectorBucketName": ...,
}

parent.get_index(**kwargs)
```

1. See [:material-code-braces: GetIndexInputTypeDef](./type_defs.md#getindexinputtypedef)

### get\_vector\_bucket

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").get_vector_bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/get_vector_bucket.html)

```python
# get_vector_bucket method definition

await def get_vector_bucket(
    self,
    *,
    vectorBucketName: str = ...,
    vectorBucketArn: str = ...,
) -> GetVectorBucketOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVectorBucketOutputTypeDef](./type_defs.md#getvectorbucketoutputtypedef)


```python
# get_vector_bucket method usage example with argument unpacking

kwargs: GetVectorBucketInputTypeDef = {  # (1)
    "vectorBucketName": ...,
}

parent.get_vector_bucket(**kwargs)
```

1. See [:material-code-braces: GetVectorBucketInputTypeDef](./type_defs.md#getvectorbucketinputtypedef)

### get\_vector\_bucket\_policy

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").get_vector_bucket_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/get_vector_bucket_policy.html)

```python
# get_vector_bucket_policy method definition

await def get_vector_bucket_policy(
    self,
    *,
    vectorBucketName: str = ...,
    vectorBucketArn: str = ...,
) -> GetVectorBucketPolicyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVectorBucketPolicyOutputTypeDef](./type_defs.md#getvectorbucketpolicyoutputtypedef)


```python
# get_vector_bucket_policy method usage example with argument unpacking

kwargs: GetVectorBucketPolicyInputTypeDef = {  # (1)
    "vectorBucketName": ...,
}

parent.get_vector_bucket_policy(**kwargs)
```

1. See [:material-code-braces: GetVectorBucketPolicyInputTypeDef](./type_defs.md#getvectorbucketpolicyinputtypedef)

### get\_vectors

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").get_vectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/get_vectors.html)

```python
# get_vectors method definition

await def get_vectors(
    self,
    *,
    keys: Sequence[str],
    vectorBucketName: str = ...,
    indexName: str = ...,
    indexArn: str = ...,
    returnData: bool = ...,
    returnMetadata: bool = ...,
) -> GetVectorsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVectorsOutputTypeDef](./type_defs.md#getvectorsoutputtypedef)


```python
# get_vectors method usage example with argument unpacking

kwargs: GetVectorsInputTypeDef = {  # (1)
    "keys": ...,
}

parent.get_vectors(**kwargs)
```

1. See [:material-code-braces: GetVectorsInputTypeDef](./type_defs.md#getvectorsinputtypedef)

### list\_indexes

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").list_indexes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/list_indexes.html)

```python
# list_indexes method definition

await def list_indexes(
    self,
    *,
    vectorBucketName: str = ...,
    vectorBucketArn: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    prefix: str = ...,
) -> ListIndexesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIndexesOutputTypeDef](./type_defs.md#listindexesoutputtypedef)


```python
# list_indexes method usage example with argument unpacking

kwargs: ListIndexesInputTypeDef = {  # (1)
    "vectorBucketName": ...,
}

parent.list_indexes(**kwargs)
```

1. See [:material-code-braces: ListIndexesInputTypeDef](./type_defs.md#listindexesinputtypedef)

### list\_vector\_buckets

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").list_vector_buckets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/list_vector_buckets.html)

```python
# list_vector_buckets method definition

await def list_vector_buckets(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    prefix: str = ...,
) -> ListVectorBucketsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVectorBucketsOutputTypeDef](./type_defs.md#listvectorbucketsoutputtypedef)


```python
# list_vector_buckets method usage example with argument unpacking

kwargs: ListVectorBucketsInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_vector_buckets(**kwargs)
```

1. See [:material-code-braces: ListVectorBucketsInputTypeDef](./type_defs.md#listvectorbucketsinputtypedef)

### list\_vectors

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").list_vectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/list_vectors.html)

```python
# list_vectors method definition

await def list_vectors(
    self,
    *,
    vectorBucketName: str = ...,
    indexName: str = ...,
    indexArn: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    segmentCount: int = ...,
    segmentIndex: int = ...,
    returnData: bool = ...,
    returnMetadata: bool = ...,
) -> ListVectorsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVectorsOutputTypeDef](./type_defs.md#listvectorsoutputtypedef)


```python
# list_vectors method usage example with argument unpacking

kwargs: ListVectorsInputTypeDef = {  # (1)
    "vectorBucketName": ...,
}

parent.list_vectors(**kwargs)
```

1. See [:material-code-braces: ListVectorsInputTypeDef](./type_defs.md#listvectorsinputtypedef)

### put\_vector\_bucket\_policy

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").put_vector_bucket_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/put_vector_bucket_policy.html)

```python
# put_vector_bucket_policy method definition

await def put_vector_bucket_policy(
    self,
    *,
    policy: str,
    vectorBucketName: str = ...,
    vectorBucketArn: str = ...,
) -> Dict[str, Any]:
    ...
```

```python
# put_vector_bucket_policy method usage example with argument unpacking

kwargs: PutVectorBucketPolicyInputTypeDef = {  # (1)
    "policy": ...,
}

parent.put_vector_bucket_policy(**kwargs)
```

1. See [:material-code-braces: PutVectorBucketPolicyInputTypeDef](./type_defs.md#putvectorbucketpolicyinputtypedef)

### put\_vectors

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").put_vectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/put_vectors.html)

```python
# put_vectors method definition

await def put_vectors(
    self,
    *,
    vectors: Sequence[PutInputVectorTypeDef],  # (1)
    vectorBucketName: str = ...,
    indexName: str = ...,
    indexArn: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See `Sequence[PutInputVectorTypeDef]`


```python
# put_vectors method usage example with argument unpacking

kwargs: PutVectorsInputTypeDef = {  # (1)
    "vectors": ...,
}

parent.put_vectors(**kwargs)
```

1. See [:material-code-braces: PutVectorsInputTypeDef](./type_defs.md#putvectorsinputtypedef)

### query\_vectors

<note> <p>Amazon S3 Vectors is in preview release for Amazon S3 and is subject
to change.

Type annotations and code completion for `#!python session.create_client("s3vectors").query_vectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/client/query_vectors.html)

```python
# query_vectors method definition

await def query_vectors(
    self,
    *,
    topK: int,
    queryVector: VectorDataUnionTypeDef,  # (1)
    vectorBucketName: str = ...,
    indexName: str = ...,
    indexArn: str = ...,
    filter: Mapping[str, Any] = ...,
    returnMetadata: bool = ...,
    returnDistance: bool = ...,
) -> QueryVectorsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VectorDataUnionTypeDef](#vectordatauniontypedef)
2. See [:material-code-braces: QueryVectorsOutputTypeDef](./type_defs.md#queryvectorsoutputtypedef)


```python
# query_vectors method usage example with argument unpacking

kwargs: QueryVectorsInputTypeDef = {  # (1)
    "topK": ...,
    "queryVector": ...,
}

parent.query_vectors(**kwargs)
```

1. See [:material-code-braces: QueryVectorsInputTypeDef](./type_defs.md#queryvectorsinputtypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("s3vectors").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors.html#S3Vectors.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("s3vectors").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors.html#S3Vectors.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("s3vectors").get_paginator` method with overloads.

- `client.get_paginator("list_indexes")` -> [ListIndexesPaginator](./paginators.md#listindexespaginator)
- `client.get_paginator("list_vector_buckets")` -> [ListVectorBucketsPaginator](./paginators.md#listvectorbucketspaginator)
- `client.get_paginator("list_vectors")` -> [ListVectorsPaginator](./paginators.md#listvectorspaginator)



