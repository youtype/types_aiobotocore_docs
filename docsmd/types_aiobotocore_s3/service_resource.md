# S3ServiceResource

> [Index](../README.md) > [S3](./README.md) > S3ServiceResource

!!! note ""

    Auto-generated documentation for [S3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#s3)
    type annotations stubs module [types-aiobotocore-s3](https://pypi.org/project/types-aiobotocore-s3/).

## S3ServiceResource

Type annotations and code completion for `#!python session.resource("s3")`, included resources and collections.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/index.html)

```python
# S3ServiceResource usage example

from types_aiobotocore_s3.service_resource import S3ServiceResource

def get_s3_resource() -> S3ServiceResource:
    return session.resource("s3")
```


## Attributes


- `meta`: `S3ResourceMeta`

- `buckets`: `ServiceResourceBucketsCollection`




## Collections

### ServiceResourceBucketsCollection

Provides access to [Bucket](#bucket) resource.

Type annotations and code completion for `#!python session.resource("s3").buckets` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/buckets.html#S3.ServiceResource.buckets)

```python
# ServiceResourceBucketsCollection usage example

from types_aiobotocore_s3.service_resource import ServiceResourceBucketsCollection

def get_collection() -> ServiceResourceBucketsCollection:
    return session.resource("s3").buckets
```



## Methods

### S3ServiceResource.get\_available\_subresources method

Returns a list of all the available sub-resources for this resource.

Type annotations and code completion for `#!python session.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


### S3ServiceResource.create\_bucket method

This action creates an Amazon S3 bucket.

Type annotations and code completion for `#!python session.resource("s3").create_bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/create_bucket.html)

```python
# create_bucket method definition

await def create_bucket(
    self,
    *,
    Bucket: str,
    ACL: BucketCannedACLType = ...,  # (1)
    CreateBucketConfiguration: CreateBucketConfigurationTypeDef = ...,  # (2)
    GrantFullControl: str = ...,
    GrantRead: str = ...,
    GrantReadACP: str = ...,
    GrantWrite: str = ...,
    GrantWriteACP: str = ...,
    ObjectLockEnabledForBucket: bool = ...,
    ObjectOwnership: ObjectOwnershipType = ...,  # (3)
) -> _Bucket:
    ...
```

1. See [:material-code-brackets: BucketCannedACLType](./literals.md#bucketcannedacltype) 
2. See [:material-code-braces: CreateBucketConfigurationTypeDef](./type_defs.md#createbucketconfigurationtypedef) 
3. See [:material-code-brackets: ObjectOwnershipType](./literals.md#objectownershiptype) 


```python
# create_bucket method usage example with argument unpacking

kwargs: CreateBucketRequestServiceResourceCreateBucketTypeDef = {  # (1)
    "Bucket": ...,
}

parent.create_bucket(**kwargs)
```

1. See [:material-code-braces: CreateBucketRequestServiceResourceCreateBucketTypeDef](./type_defs.md#createbucketrequestserviceresourcecreatebuckettypedef) 

### S3ServiceResource.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python session.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
    name: str,
) -> _Bucket:
    ...
```


### S3ServiceResource.BucketAcl method

Creates a BucketAcl resource.

Type annotations and code completion for `#!python session.resource("s3").BucketAcl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/BucketAcl.html)

```python
# BucketAcl method definition

await def BucketAcl(
    self,
    bucket_name: str,
) -> _BucketAcl:
    ...
```


### S3ServiceResource.BucketCors method

Creates a BucketCors resource.

Type annotations and code completion for `#!python session.resource("s3").BucketCors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/BucketCors.html)

```python
# BucketCors method definition

await def BucketCors(
    self,
    bucket_name: str,
) -> _BucketCors:
    ...
```


### S3ServiceResource.BucketLifecycle method

Creates a BucketLifecycle resource.

Type annotations and code completion for `#!python session.resource("s3").BucketLifecycle` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/BucketLifecycle.html)

```python
# BucketLifecycle method definition

await def BucketLifecycle(
    self,
    bucket_name: str,
) -> _BucketLifecycle:
    ...
```


### S3ServiceResource.BucketLifecycleConfiguration method

Creates a BucketLifecycleConfiguration resource.

Type annotations and code completion for `#!python session.resource("s3").BucketLifecycleConfiguration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/BucketLifecycleConfiguration.html)

```python
# BucketLifecycleConfiguration method definition

await def BucketLifecycleConfiguration(
    self,
    bucket_name: str,
) -> _BucketLifecycleConfiguration:
    ...
```


### S3ServiceResource.BucketLogging method

Creates a BucketLogging resource.

Type annotations and code completion for `#!python session.resource("s3").BucketLogging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/BucketLogging.html)

```python
# BucketLogging method definition

await def BucketLogging(
    self,
    bucket_name: str,
) -> _BucketLogging:
    ...
```


### S3ServiceResource.BucketNotification method

Creates a BucketNotification resource.

Type annotations and code completion for `#!python session.resource("s3").BucketNotification` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/BucketNotification.html)

```python
# BucketNotification method definition

await def BucketNotification(
    self,
    bucket_name: str,
) -> _BucketNotification:
    ...
```


### S3ServiceResource.BucketPolicy method

Creates a BucketPolicy resource.

Type annotations and code completion for `#!python session.resource("s3").BucketPolicy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/BucketPolicy.html)

```python
# BucketPolicy method definition

await def BucketPolicy(
    self,
    bucket_name: str,
) -> _BucketPolicy:
    ...
```


### S3ServiceResource.BucketRequestPayment method

Creates a BucketRequestPayment resource.

Type annotations and code completion for `#!python session.resource("s3").BucketRequestPayment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/BucketRequestPayment.html)

```python
# BucketRequestPayment method definition

await def BucketRequestPayment(
    self,
    bucket_name: str,
) -> _BucketRequestPayment:
    ...
```


### S3ServiceResource.BucketTagging method

Creates a BucketTagging resource.

Type annotations and code completion for `#!python session.resource("s3").BucketTagging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/BucketTagging.html)

```python
# BucketTagging method definition

await def BucketTagging(
    self,
    bucket_name: str,
) -> _BucketTagging:
    ...
```


### S3ServiceResource.BucketVersioning method

Creates a BucketVersioning resource.

Type annotations and code completion for `#!python session.resource("s3").BucketVersioning` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/BucketVersioning.html)

```python
# BucketVersioning method definition

await def BucketVersioning(
    self,
    bucket_name: str,
) -> _BucketVersioning:
    ...
```


### S3ServiceResource.BucketWebsite method

Creates a BucketWebsite resource.

Type annotations and code completion for `#!python session.resource("s3").BucketWebsite` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/BucketWebsite.html)

```python
# BucketWebsite method definition

await def BucketWebsite(
    self,
    bucket_name: str,
) -> _BucketWebsite:
    ...
```


### S3ServiceResource.MultipartUpload method

Creates a MultipartUpload resource.

Type annotations and code completion for `#!python session.resource("s3").MultipartUpload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/MultipartUpload.html)

```python
# MultipartUpload method definition

await def MultipartUpload(
    self,
    bucket_name: str,
    object_key: str,
    id: str,
) -> _MultipartUpload:
    ...
```


### S3ServiceResource.MultipartUploadPart method

Creates a MultipartUploadPart resource.

Type annotations and code completion for `#!python session.resource("s3").MultipartUploadPart` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/MultipartUploadPart.html)

```python
# MultipartUploadPart method definition

await def MultipartUploadPart(
    self,
    bucket_name: str,
    object_key: str,
    multipart_upload_id: str,
    part_number: int,
) -> _MultipartUploadPart:
    ...
```


### S3ServiceResource.Object method

Creates a Object resource.

Type annotations and code completion for `#!python session.resource("s3").Object` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/Object.html)

```python
# Object method definition

await def Object(
    self,
    bucket_name: str,
    key: str,
) -> _Object:
    ...
```


### S3ServiceResource.ObjectAcl method

Creates a ObjectAcl resource.

Type annotations and code completion for `#!python session.resource("s3").ObjectAcl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/ObjectAcl.html)

```python
# ObjectAcl method definition

await def ObjectAcl(
    self,
    bucket_name: str,
    object_key: str,
) -> _ObjectAcl:
    ...
```


### S3ServiceResource.ObjectSummary method

Creates a ObjectSummary resource.

Type annotations and code completion for `#!python session.resource("s3").ObjectSummary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/ObjectSummary.html)

```python
# ObjectSummary method definition

await def ObjectSummary(
    self,
    bucket_name: str,
    key: str,
) -> _ObjectSummary:
    ...
```


### S3ServiceResource.ObjectVersion method

Creates a ObjectVersion resource.

Type annotations and code completion for `#!python session.resource("s3").ObjectVersion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/service-resource/ObjectVersion.html)

```python
# ObjectVersion method definition

await def ObjectVersion(
    self,
    bucket_name: str,
    object_key: str,
    id: str,
) -> _ObjectVersion:
    ...
```




## Bucket

Type annotations and code completion for `#!python session.resource("s3").Bucket` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/index.html#S3.Bucket)

```python
# Bucket usage example

from types_aiobotocore_s3.service_resource import Bucket

def get_resource() -> Bucket:
    return session.resource("s3").Bucket(...)
```


### Bucket attributes


- `name`: `str`
- `multipart_uploads`: `BucketMultipartUploadsCollection`
- `object_versions`: `BucketObjectVersionsCollection`
- `objects`: `BucketObjectsCollection`
- `creation_date`: `Awaitable`[`datetime`]
- `bucket_region`: `Awaitable`[`str`]
- `meta`: `S3ResourceMeta`



### Bucket collections


#### Bucket.multipart_uploads

Provides access to [MultipartUpload](#multipartupload) resource.

Type annotations and code completion for `#!python session.resource("s3").Bucket(...).multipart_uploads` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/multipart_uploads.html#S3.Bucket.multipart_uploads)

```python
# BucketMultipartUploadsCollection usage example

from types_aiobotocore_s3.service_resource import BucketMultipartUploadsCollection

def get_collection() -> BucketMultipartUploadsCollection:
    resource = session.resource("s3").Bucket(...)
    return resource.multipart_uploads
```

#### Bucket.object_versions

Provides access to [ObjectVersion](#objectversion) resource.

Type annotations and code completion for `#!python session.resource("s3").Bucket(...).object_versions` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/object_versions.html#S3.Bucket.object_versions)

```python
# BucketObjectVersionsCollection usage example

from types_aiobotocore_s3.service_resource import BucketObjectVersionsCollection

def get_collection() -> BucketObjectVersionsCollection:
    resource = session.resource("s3").Bucket(...)
    return resource.object_versions
```

#### Bucket.objects

Provides access to [ObjectSummary](#objectsummary) resource.

Type annotations and code completion for `#!python session.resource("s3").Bucket(...).objects` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/objects.html#S3.Bucket.objects)

```python
# BucketObjectsCollection usage example

from types_aiobotocore_s3.service_resource import BucketObjectsCollection

def get_collection() -> BucketObjectsCollection:
    resource = session.resource("s3").Bucket(...)
    return resource.objects
```




### Bucket methods


#### Bucket.get\_available\_subresources method

Returns a list of all the available sub-resources for this Bucket.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Bucket.create method

This action creates an Amazon S3 bucket.

Type annotations and code completion for `#!python aiobotocore.resource("s3").create` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/create.html)

```python
# create method definition

await def create(
    self,
    *,
    ACL: BucketCannedACLType = ...,  # (1)
    CreateBucketConfiguration: CreateBucketConfigurationTypeDef = ...,  # (2)
    GrantFullControl: str = ...,
    GrantRead: str = ...,
    GrantReadACP: str = ...,
    GrantWrite: str = ...,
    GrantWriteACP: str = ...,
    ObjectLockEnabledForBucket: bool = ...,
    ObjectOwnership: ObjectOwnershipType = ...,  # (3)
) -> CreateBucketOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: BucketCannedACLType](./literals.md#bucketcannedacltype) 
2. See [:material-code-braces: CreateBucketConfigurationTypeDef](./type_defs.md#createbucketconfigurationtypedef) 
3. See [:material-code-brackets: ObjectOwnershipType](./literals.md#objectownershiptype) 
4. See [:material-code-braces: CreateBucketOutputTypeDef](./type_defs.md#createbucketoutputtypedef) 


```python
# create method usage example with argument unpacking

kwargs: CreateBucketRequestBucketCreateTypeDef = {  # (1)
    "ACL": ...,
}

parent.create(**kwargs)
```

1. See [:material-code-braces: CreateBucketRequestBucketCreateTypeDef](./type_defs.md#createbucketrequestbucketcreatetypedef) 

#### Bucket.delete method

Deletes the S3 bucket.

Type annotations and code completion for `#!python aiobotocore.resource("s3").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/delete.html)

```python
# delete method definition

await def delete(
    self,
    *,
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```



```python
# delete method usage example with argument unpacking

kwargs: DeleteBucketRequestBucketDeleteTypeDef = {  # (1)
    "ExpectedBucketOwner": ...,
}

parent.delete(**kwargs)
```

1. See [:material-code-braces: DeleteBucketRequestBucketDeleteTypeDef](./type_defs.md#deletebucketrequestbucketdeletetypedef) 

#### Bucket.delete\_objects method

This operation enables you to delete multiple objects from a bucket using a
single HTTP request.

Type annotations and code completion for `#!python aiobotocore.resource("s3").delete_objects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/delete_objects.html)

```python
# delete_objects method definition

await def delete_objects(
    self,
    *,
    Delete: DeleteTypeDef,  # (1)
    MFA: str = ...,
    RequestPayer: RequestPayerType = ...,  # (2)
    BypassGovernanceRetention: bool = ...,
    ExpectedBucketOwner: str = ...,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (3)
) -> DeleteObjectsOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DeleteTypeDef](./type_defs.md#deletetypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
4. See [:material-code-braces: DeleteObjectsOutputTypeDef](./type_defs.md#deleteobjectsoutputtypedef) 


```python
# delete_objects method usage example with argument unpacking

kwargs: DeleteObjectsRequestBucketDeleteObjectsTypeDef = {  # (1)
    "Delete": ...,
}

parent.delete_objects(**kwargs)
```

1. See [:material-code-braces: DeleteObjectsRequestBucketDeleteObjectsTypeDef](./type_defs.md#deleteobjectsrequestbucketdeleteobjectstypedef) 

#### Bucket.put\_object method

Adds an object to a bucket.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put_object` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/put_object.html)

```python
# put_object method definition

await def put_object(
    self,
    *,
    Key: str,
    ACL: ObjectCannedACLType = ...,  # (1)
    Body: BlobTypeDef = ...,
    CacheControl: str = ...,
    ContentDisposition: str = ...,
    ContentEncoding: str = ...,
    ContentLanguage: str = ...,
    ContentLength: int = ...,
    ContentMD5: str = ...,
    ContentType: str = ...,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (2)
    ChecksumCRC32: str = ...,
    ChecksumCRC32C: str = ...,
    ChecksumCRC64NVME: str = ...,
    ChecksumSHA1: str = ...,
    ChecksumSHA256: str = ...,
    Expires: TimestampTypeDef = ...,
    IfMatch: str = ...,
    IfNoneMatch: str = ...,
    GrantFullControl: str = ...,
    GrantRead: str = ...,
    GrantReadACP: str = ...,
    GrantWriteACP: str = ...,
    WriteOffsetBytes: int = ...,
    Metadata: Mapping[str, str] = ...,
    ServerSideEncryption: ServerSideEncryptionType = ...,  # (3)
    StorageClass: StorageClassType = ...,  # (4)
    WebsiteRedirectLocation: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    SSEKMSKeyId: str = ...,
    SSEKMSEncryptionContext: str = ...,
    BucketKeyEnabled: bool = ...,
    RequestPayer: RequestPayerType = ...,  # (5)
    Tagging: str = ...,
    ObjectLockMode: ObjectLockModeType = ...,  # (6)
    ObjectLockRetainUntilDate: TimestampTypeDef = ...,
    ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,  # (7)
    ExpectedBucketOwner: str = ...,
) -> _Object:
    ...
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
3. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
4. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
5. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
6. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
7. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 


```python
# put_object method usage example with argument unpacking

kwargs: PutObjectRequestBucketPutObjectTypeDef = {  # (1)
    "Key": ...,
}

parent.put_object(**kwargs)
```

1. See [:material-code-braces: PutObjectRequestBucketPutObjectTypeDef](./type_defs.md#putobjectrequestbucketputobjecttypedef) 

#### Bucket.wait\_until\_exists method

Waits until Bucket is exists.

Type annotations and code completion for `#!python aiobotocore.resource("s3").wait_until_exists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/wait_until_exists.html)

```python
# wait_until_exists method definition

await def wait_until_exists(
    self,
) -> None:
    ...
```


#### Bucket.wait\_until\_not\_exists method

Waits until Bucket is not_exists.

Type annotations and code completion for `#!python aiobotocore.resource("s3").wait_until_not_exists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/wait_until_not_exists.html)

```python
# wait_until_not_exists method definition

await def wait_until_not_exists(
    self,
) -> None:
    ...
```


#### Bucket.Acl method

Creates a BucketAcl resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/Acl.html)

```python
# Acl method definition

await def Acl(
    self,
) -> _BucketAcl:
    ...
```


#### Bucket.Cors method

Creates a BucketCors resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Cors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/Cors.html)

```python
# Cors method definition

await def Cors(
    self,
) -> _BucketCors:
    ...
```


#### Bucket.Lifecycle method

Creates a BucketLifecycle resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Lifecycle` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/Lifecycle.html)

```python
# Lifecycle method definition

await def Lifecycle(
    self,
) -> _BucketLifecycle:
    ...
```


#### Bucket.LifecycleConfiguration method

Creates a BucketLifecycleConfiguration resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").LifecycleConfiguration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/LifecycleConfiguration.html)

```python
# LifecycleConfiguration method definition

await def LifecycleConfiguration(
    self,
) -> _BucketLifecycleConfiguration:
    ...
```


#### Bucket.Logging method

Creates a BucketLogging resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Logging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/Logging.html)

```python
# Logging method definition

await def Logging(
    self,
) -> _BucketLogging:
    ...
```


#### Bucket.Notification method

Creates a BucketNotification resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Notification` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/Notification.html)

```python
# Notification method definition

await def Notification(
    self,
) -> _BucketNotification:
    ...
```


#### Bucket.Object method

Creates a Object resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Object` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/Object.html)

```python
# Object method definition

await def Object(
    self,
    key: str,
) -> _Object:
    ...
```


#### Bucket.Policy method

Creates a BucketPolicy resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/Policy.html)

```python
# Policy method definition

await def Policy(
    self,
) -> _BucketPolicy:
    ...
```


#### Bucket.RequestPayment method

Creates a BucketRequestPayment resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").RequestPayment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/RequestPayment.html)

```python
# RequestPayment method definition

await def RequestPayment(
    self,
) -> _BucketRequestPayment:
    ...
```


#### Bucket.Tagging method

Creates a BucketTagging resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Tagging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/Tagging.html)

```python
# Tagging method definition

await def Tagging(
    self,
) -> _BucketTagging:
    ...
```


#### Bucket.Versioning method

Creates a BucketVersioning resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Versioning` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/Versioning.html)

```python
# Versioning method definition

await def Versioning(
    self,
) -> _BucketVersioning:
    ...
```


#### Bucket.Website method

Creates a BucketWebsite resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Website` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/Website.html)

```python
# Website method definition

await def Website(
    self,
) -> _BucketWebsite:
    ...
```


#### Bucket.load method

Calls s3.Client.list_buckets() to update the attributes of the Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Bucket.copy method

Copy an object from one S3 location to another.

Type annotations and code completion for `#!python aiobotocore.resource("s3").copy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/copy.html)

```python
# copy method definition

await def copy(
    self,
    CopySource: CopySourceTypeDef,  # (1)
    Key: str,
    ExtraArgs: Union[Dict[str, Any], None] = ...,
    Callback: Union[Callable[..., Any], None] = ...,
    SourceClient: Union[AioBaseClient, None] = ...,
    Config: Union[TransferConfig, None] = ...,
) -> None:
    ...
```

1. See [:material-code-braces: CopySourceTypeDef](./type_defs.md#copysourcetypedef) 


```python
# copy method usage example with argument unpacking

kwargs: BucketCopyRequestTypeDef = {  # (1)
    "CopySource": ...,
    "Key": ...,
}

parent.copy(**kwargs)
```

1. See [:material-code-braces: BucketCopyRequestTypeDef](./type_defs.md#bucketcopyrequesttypedef) 

#### Bucket.download\_file method

Download an object from S3 to a file.

Type annotations and code completion for `#!python aiobotocore.resource("s3").download_file` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/download_file.html)

```python
# download_file method definition

await def download_file(
    self,
    Key: str,
    Filename: str,
    ExtraArgs: Union[Dict[str, Any], None] = ...,
    Callback: Union[Callable[..., Any], None] = ...,
    Config: Union[TransferConfig, None] = ...,
) -> None:
    ...
```



```python
# download_file method usage example with argument unpacking

kwargs: BucketDownloadFileRequestTypeDef = {  # (1)
    "Key": ...,
    "Filename": ...,
}

parent.download_file(**kwargs)
```

1. See [:material-code-braces: BucketDownloadFileRequestTypeDef](./type_defs.md#bucketdownloadfilerequesttypedef) 

#### Bucket.download\_fileobj method

Download an object from S3 to a file-like object.

Type annotations and code completion for `#!python aiobotocore.resource("s3").download_fileobj` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/download_fileobj.html)

```python
# download_fileobj method definition

await def download_fileobj(
    self,
    Key: str,
    Fileobj: FileobjTypeDef,
    ExtraArgs: Union[Dict[str, Any], None] = ...,
    Callback: Union[Callable[..., Any], None] = ...,
    Config: Union[TransferConfig, None] = ...,
) -> None:
    ...
```



```python
# download_fileobj method usage example with argument unpacking

kwargs: BucketDownloadFileobjRequestTypeDef = {  # (1)
    "Key": ...,
    "Fileobj": ...,
}

parent.download_fileobj(**kwargs)
```

1. See [:material-code-braces: BucketDownloadFileobjRequestTypeDef](./type_defs.md#bucketdownloadfileobjrequesttypedef) 

#### Bucket.upload\_file method

Upload a file to S3.

Type annotations and code completion for `#!python aiobotocore.resource("s3").upload_file` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/upload_file.html)

```python
# upload_file method definition

await def upload_file(
    self,
    Filename: str,
    Key: str,
    ExtraArgs: Union[Dict[str, Any], None] = ...,
    Callback: Union[Callable[..., Any], None] = ...,
    Config: Union[TransferConfig, None] = ...,
) -> None:
    ...
```



```python
# upload_file method usage example with argument unpacking

kwargs: BucketUploadFileRequestTypeDef = {  # (1)
    "Filename": ...,
    "Key": ...,
}

parent.upload_file(**kwargs)
```

1. See [:material-code-braces: BucketUploadFileRequestTypeDef](./type_defs.md#bucketuploadfilerequesttypedef) 

#### Bucket.upload\_fileobj method

Upload a file-like object to S3.

Type annotations and code completion for `#!python aiobotocore.resource("s3").upload_fileobj` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucket/upload_fileobj.html)

```python
# upload_fileobj method definition

await def upload_fileobj(
    self,
    Fileobj: FileobjTypeDef,
    Key: str,
    ExtraArgs: Union[Dict[str, Any], None] = ...,
    Callback: Union[Callable[..., Any], None] = ...,
    Config: Union[TransferConfig, None] = ...,
) -> None:
    ...
```



```python
# upload_fileobj method usage example with argument unpacking

kwargs: BucketUploadFileobjRequestTypeDef = {  # (1)
    "Fileobj": ...,
    "Key": ...,
}

parent.upload_fileobj(**kwargs)
```

1. See [:material-code-braces: BucketUploadFileobjRequestTypeDef](./type_defs.md#bucketuploadfileobjrequesttypedef) 




## BucketAcl

Type annotations and code completion for `#!python session.resource("s3").BucketAcl` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketacl/index.html#S3.BucketAcl)

```python
# BucketAcl usage example

from types_aiobotocore_s3.service_resource import BucketAcl

def get_resource() -> BucketAcl:
    return session.resource("s3").BucketAcl(...)
```


### BucketAcl attributes


- `bucket_name`: `str`
- `owner`: `Awaitable`[[OwnerTypeDef](./type_defs.md#ownertypedef)]
- `grants`: `Awaitable`[`List`[[GrantTypeDef](./type_defs.md#granttypedef)]]
- `meta`: `S3ResourceMeta`





### BucketAcl methods


#### BucketAcl.get\_available\_subresources method

Returns a list of all the available sub-resources for this BucketAcl.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketacl/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### BucketAcl.put method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketacl/put.html)

```python
# put method definition

await def put(
    self,
    *,
    ACL: BucketCannedACLType = ...,  # (1)
    AccessControlPolicy: AccessControlPolicyTypeDef = ...,  # (2)
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (3)
    GrantFullControl: str = ...,
    GrantRead: str = ...,
    GrantReadACP: str = ...,
    GrantWrite: str = ...,
    GrantWriteACP: str = ...,
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```

1. See [:material-code-brackets: BucketCannedACLType](./literals.md#bucketcannedacltype) 
2. See [:material-code-braces: AccessControlPolicyTypeDef](./type_defs.md#accesscontrolpolicytypedef) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 


```python
# put method usage example with argument unpacking

kwargs: PutBucketAclRequestBucketAclPutTypeDef = {  # (1)
    "ACL": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutBucketAclRequestBucketAclPutTypeDef](./type_defs.md#putbucketaclrequestbucketaclputtypedef) 

#### BucketAcl.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketacl/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
) -> _Bucket:
    ...
```


#### BucketAcl.load method



Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketacl/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### BucketAcl.reload method



Type annotations and code completion for `#!python aiobotocore.resource("s3").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketacl/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## BucketCors

Type annotations and code completion for `#!python session.resource("s3").BucketCors` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketcors/index.html#S3.BucketCors)

```python
# BucketCors usage example

from types_aiobotocore_s3.service_resource import BucketCors

def get_resource() -> BucketCors:
    return session.resource("s3").BucketCors(...)
```


### BucketCors attributes


- `bucket_name`: `str`
- `cors_rules`: `Awaitable`[`List`[[CORSRuleOutputTypeDef](./type_defs.md#corsruleoutputtypedef)]]
- `meta`: `S3ResourceMeta`





### BucketCors methods


#### BucketCors.get\_available\_subresources method

Returns a list of all the available sub-resources for this BucketCors.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketcors/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### BucketCors.delete method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketcors/delete.html)

```python
# delete method definition

await def delete(
    self,
    *,
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```



```python
# delete method usage example with argument unpacking

kwargs: DeleteBucketCorsRequestBucketCorsDeleteTypeDef = {  # (1)
    "ExpectedBucketOwner": ...,
}

parent.delete(**kwargs)
```

1. See [:material-code-braces: DeleteBucketCorsRequestBucketCorsDeleteTypeDef](./type_defs.md#deletebucketcorsrequestbucketcorsdeletetypedef) 

#### BucketCors.put method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketcors/put.html)

```python
# put method definition

await def put(
    self,
    *,
    CORSConfiguration: CORSConfigurationTypeDef,  # (1)
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (2)
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```

1. See [:material-code-braces: CORSConfigurationTypeDef](./type_defs.md#corsconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 


```python
# put method usage example with argument unpacking

kwargs: PutBucketCorsRequestBucketCorsPutTypeDef = {  # (1)
    "CORSConfiguration": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutBucketCorsRequestBucketCorsPutTypeDef](./type_defs.md#putbucketcorsrequestbucketcorsputtypedef) 

#### BucketCors.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketcors/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
) -> _Bucket:
    ...
```


#### BucketCors.load method



Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketcors/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### BucketCors.reload method



Type annotations and code completion for `#!python aiobotocore.resource("s3").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketcors/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## BucketLifecycle

Type annotations and code completion for `#!python session.resource("s3").BucketLifecycle` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycle/index.html#S3.BucketLifecycle)

```python
# BucketLifecycle usage example

from types_aiobotocore_s3.service_resource import BucketLifecycle

def get_resource() -> BucketLifecycle:
    return session.resource("s3").BucketLifecycle(...)
```


### BucketLifecycle attributes


- `bucket_name`: `str`
- `rules`: `Awaitable`[`List`[[RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef)]]
- `meta`: `S3ResourceMeta`





### BucketLifecycle methods


#### BucketLifecycle.get\_available\_subresources method

Returns a list of all the available sub-resources for this BucketLifecycle.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycle/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### BucketLifecycle.delete method

Deletes the lifecycle configuration from the specified bucket.

Type annotations and code completion for `#!python aiobotocore.resource("s3").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycle/delete.html)

```python
# delete method definition

await def delete(
    self,
    *,
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```



```python
# delete method usage example with argument unpacking

kwargs: DeleteBucketLifecycleRequestBucketLifecycleDeleteTypeDef = {  # (1)
    "ExpectedBucketOwner": ...,
}

parent.delete(**kwargs)
```

1. See [:material-code-braces: DeleteBucketLifecycleRequestBucketLifecycleDeleteTypeDef](./type_defs.md#deletebucketlifecyclerequestbucketlifecycledeletetypedef) 

#### BucketLifecycle.put method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycle/put.html)

```python
# put method definition

await def put(
    self,
    *,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (1)
    LifecycleConfiguration: LifecycleConfigurationTypeDef = ...,  # (2)
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-braces: LifecycleConfigurationTypeDef](./type_defs.md#lifecycleconfigurationtypedef) 


```python
# put method usage example with argument unpacking

kwargs: PutBucketLifecycleRequestBucketLifecyclePutTypeDef = {  # (1)
    "ChecksumAlgorithm": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutBucketLifecycleRequestBucketLifecyclePutTypeDef](./type_defs.md#putbucketlifecyclerequestbucketlifecycleputtypedef) 

#### BucketLifecycle.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycle/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
) -> _Bucket:
    ...
```


#### BucketLifecycle.load method



Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycle/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### BucketLifecycle.reload method



Type annotations and code completion for `#!python aiobotocore.resource("s3").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycle/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## BucketLifecycleConfiguration

Type annotations and code completion for `#!python session.resource("s3").BucketLifecycleConfiguration` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycleconfiguration/index.html#S3.BucketLifecycleConfiguration)

```python
# BucketLifecycleConfiguration usage example

from types_aiobotocore_s3.service_resource import BucketLifecycleConfiguration

def get_resource() -> BucketLifecycleConfiguration:
    return session.resource("s3").BucketLifecycleConfiguration(...)
```


### BucketLifecycleConfiguration attributes


- `bucket_name`: `str`
- `rules`: `Awaitable`[`List`[[LifecycleRuleOutputTypeDef](./type_defs.md#lifecycleruleoutputtypedef)]]
- `transition_default_minimum_object_size`: `Awaitable`[[TransitionDefaultMinimumObjectSizeType](./literals.md#transitiondefaultminimumobjectsizetype)]
- `meta`: `S3ResourceMeta`





### BucketLifecycleConfiguration methods


#### BucketLifecycleConfiguration.get\_available\_subresources method

Returns a list of all the available sub-resources for this
BucketLifecycleConfiguration.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycleconfiguration/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### BucketLifecycleConfiguration.delete method

Deletes the lifecycle configuration from the specified bucket.

Type annotations and code completion for `#!python aiobotocore.resource("s3").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycleconfiguration/delete.html)

```python
# delete method definition

await def delete(
    self,
    *,
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```



```python
# delete method usage example with argument unpacking

kwargs: DeleteBucketLifecycleRequestBucketLifecycleConfigurationDeleteTypeDef = {  # (1)
    "ExpectedBucketOwner": ...,
}

parent.delete(**kwargs)
```

1. See [:material-code-braces: DeleteBucketLifecycleRequestBucketLifecycleConfigurationDeleteTypeDef](./type_defs.md#deletebucketlifecyclerequestbucketlifecycleconfigurationdeletetypedef) 

#### BucketLifecycleConfiguration.put method

Creates a new lifecycle configuration for the bucket or replaces an existing
lifecycle configuration.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycleconfiguration/put.html)

```python
# put method definition

await def put(
    self,
    *,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (1)
    LifecycleConfiguration: BucketLifecycleConfigurationTypeDef = ...,  # (2)
    ExpectedBucketOwner: str = ...,
    TransitionDefaultMinimumObjectSize: TransitionDefaultMinimumObjectSizeType = ...,  # (3)
) -> PutBucketLifecycleConfigurationOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-braces: BucketLifecycleConfigurationTypeDef](./type_defs.md#bucketlifecycleconfigurationtypedef) 
3. See [:material-code-brackets: TransitionDefaultMinimumObjectSizeType](./literals.md#transitiondefaultminimumobjectsizetype) 
4. See [:material-code-braces: PutBucketLifecycleConfigurationOutputTypeDef](./type_defs.md#putbucketlifecycleconfigurationoutputtypedef) 


```python
# put method usage example with argument unpacking

kwargs: PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef = {  # (1)
    "ChecksumAlgorithm": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef](./type_defs.md#putbucketlifecycleconfigurationrequestbucketlifecycleconfigurationputtypedef) 

#### BucketLifecycleConfiguration.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycleconfiguration/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
) -> _Bucket:
    ...
```


#### BucketLifecycleConfiguration.load method



Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycleconfiguration/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### BucketLifecycleConfiguration.reload method



Type annotations and code completion for `#!python aiobotocore.resource("s3").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlifecycleconfiguration/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## BucketLogging

Type annotations and code completion for `#!python session.resource("s3").BucketLogging` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlogging/index.html#S3.BucketLogging)

```python
# BucketLogging usage example

from types_aiobotocore_s3.service_resource import BucketLogging

def get_resource() -> BucketLogging:
    return session.resource("s3").BucketLogging(...)
```


### BucketLogging attributes


- `bucket_name`: `str`
- `logging_enabled`: `Awaitable`[[LoggingEnabledOutputTypeDef](./type_defs.md#loggingenabledoutputtypedef)]
- `meta`: `S3ResourceMeta`





### BucketLogging methods


#### BucketLogging.get\_available\_subresources method

Returns a list of all the available sub-resources for this BucketLogging.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlogging/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### BucketLogging.put method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlogging/put.html)

```python
# put method definition

await def put(
    self,
    *,
    BucketLoggingStatus: BucketLoggingStatusTypeDef,  # (1)
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (2)
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```

1. See [:material-code-braces: BucketLoggingStatusTypeDef](./type_defs.md#bucketloggingstatustypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 


```python
# put method usage example with argument unpacking

kwargs: PutBucketLoggingRequestBucketLoggingPutTypeDef = {  # (1)
    "BucketLoggingStatus": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutBucketLoggingRequestBucketLoggingPutTypeDef](./type_defs.md#putbucketloggingrequestbucketloggingputtypedef) 

#### BucketLogging.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlogging/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
) -> _Bucket:
    ...
```


#### BucketLogging.load method



Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlogging/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### BucketLogging.reload method



Type annotations and code completion for `#!python aiobotocore.resource("s3").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketlogging/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## BucketNotification

Type annotations and code completion for `#!python session.resource("s3").BucketNotification` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketnotification/index.html#S3.BucketNotification)

```python
# BucketNotification usage example

from types_aiobotocore_s3.service_resource import BucketNotification

def get_resource() -> BucketNotification:
    return session.resource("s3").BucketNotification(...)
```


### BucketNotification attributes


- `bucket_name`: `str`
- `topic_configurations`: `Awaitable`[`List`[[TopicConfigurationOutputTypeDef](./type_defs.md#topicconfigurationoutputtypedef)]]
- `queue_configurations`: `Awaitable`[`List`[[QueueConfigurationOutputTypeDef](./type_defs.md#queueconfigurationoutputtypedef)]]
- `lambda_function_configurations`: `Awaitable`[`List`[[LambdaFunctionConfigurationOutputTypeDef](./type_defs.md#lambdafunctionconfigurationoutputtypedef)]]
- `event_bridge_configuration`: `Awaitable`[`Dict`[`str`, `Any`]]
- `meta`: `S3ResourceMeta`





### BucketNotification methods


#### BucketNotification.get\_available\_subresources method

Returns a list of all the available sub-resources for this BucketNotification.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketnotification/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### BucketNotification.put method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketnotification/put.html)

```python
# put method definition

await def put(
    self,
    *,
    NotificationConfiguration: NotificationConfigurationTypeDef,  # (1)
    ExpectedBucketOwner: str = ...,
    SkipDestinationValidation: bool = ...,
) -> None:
    ...
```

1. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 


```python
# put method usage example with argument unpacking

kwargs: PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef = {  # (1)
    "NotificationConfiguration": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef](./type_defs.md#putbucketnotificationconfigurationrequestbucketnotificationputtypedef) 

#### BucketNotification.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketnotification/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
) -> _Bucket:
    ...
```


#### BucketNotification.load method



Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketnotification/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### BucketNotification.reload method



Type annotations and code completion for `#!python aiobotocore.resource("s3").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketnotification/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## BucketPolicy

Type annotations and code completion for `#!python session.resource("s3").BucketPolicy` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketpolicy/index.html#S3.BucketPolicy)

```python
# BucketPolicy usage example

from types_aiobotocore_s3.service_resource import BucketPolicy

def get_resource() -> BucketPolicy:
    return session.resource("s3").BucketPolicy(...)
```


### BucketPolicy attributes


- `bucket_name`: `str`
- `policy`: `Awaitable`[`str`]
- `meta`: `S3ResourceMeta`





### BucketPolicy methods


#### BucketPolicy.get\_available\_subresources method

Returns a list of all the available sub-resources for this BucketPolicy.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketpolicy/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### BucketPolicy.delete method

Deletes the policy of a specified bucket.

Type annotations and code completion for `#!python aiobotocore.resource("s3").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketpolicy/delete.html)

```python
# delete method definition

await def delete(
    self,
    *,
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```



```python
# delete method usage example with argument unpacking

kwargs: DeleteBucketPolicyRequestBucketPolicyDeleteTypeDef = {  # (1)
    "ExpectedBucketOwner": ...,
}

parent.delete(**kwargs)
```

1. See [:material-code-braces: DeleteBucketPolicyRequestBucketPolicyDeleteTypeDef](./type_defs.md#deletebucketpolicyrequestbucketpolicydeletetypedef) 

#### BucketPolicy.put method

Applies an Amazon S3 bucket policy to an Amazon S3 bucket.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketpolicy/put.html)

```python
# put method definition

await def put(
    self,
    *,
    Policy: str,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (1)
    ConfirmRemoveSelfBucketAccess: bool = ...,
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 


```python
# put method usage example with argument unpacking

kwargs: PutBucketPolicyRequestBucketPolicyPutTypeDef = {  # (1)
    "Policy": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutBucketPolicyRequestBucketPolicyPutTypeDef](./type_defs.md#putbucketpolicyrequestbucketpolicyputtypedef) 

#### BucketPolicy.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketpolicy/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
) -> _Bucket:
    ...
```


#### BucketPolicy.load method



Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketpolicy/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### BucketPolicy.reload method



Type annotations and code completion for `#!python aiobotocore.resource("s3").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketpolicy/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## BucketRequestPayment

Type annotations and code completion for `#!python session.resource("s3").BucketRequestPayment` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketrequestpayment/index.html#S3.BucketRequestPayment)

```python
# BucketRequestPayment usage example

from types_aiobotocore_s3.service_resource import BucketRequestPayment

def get_resource() -> BucketRequestPayment:
    return session.resource("s3").BucketRequestPayment(...)
```


### BucketRequestPayment attributes


- `bucket_name`: `str`
- `payer`: `Awaitable`[[PayerType](./literals.md#payertype)]
- `meta`: `S3ResourceMeta`





### BucketRequestPayment methods


#### BucketRequestPayment.get\_available\_subresources method

Returns a list of all the available sub-resources for this BucketRequestPayment.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketrequestpayment/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### BucketRequestPayment.put method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketrequestpayment/put.html)

```python
# put method definition

await def put(
    self,
    *,
    RequestPaymentConfiguration: RequestPaymentConfigurationTypeDef,  # (1)
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (2)
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```

1. See [:material-code-braces: RequestPaymentConfigurationTypeDef](./type_defs.md#requestpaymentconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 


```python
# put method usage example with argument unpacking

kwargs: PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef = {  # (1)
    "RequestPaymentConfiguration": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef](./type_defs.md#putbucketrequestpaymentrequestbucketrequestpaymentputtypedef) 

#### BucketRequestPayment.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketrequestpayment/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
) -> _Bucket:
    ...
```


#### BucketRequestPayment.load method



Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketrequestpayment/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### BucketRequestPayment.reload method



Type annotations and code completion for `#!python aiobotocore.resource("s3").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketrequestpayment/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## BucketTagging

Type annotations and code completion for `#!python session.resource("s3").BucketTagging` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/buckettagging/index.html#S3.BucketTagging)

```python
# BucketTagging usage example

from types_aiobotocore_s3.service_resource import BucketTagging

def get_resource() -> BucketTagging:
    return session.resource("s3").BucketTagging(...)
```


### BucketTagging attributes


- `bucket_name`: `str`
- `tag_set`: `Awaitable`[`List`[[TagTypeDef](./type_defs.md#tagtypedef)]]
- `meta`: `S3ResourceMeta`





### BucketTagging methods


#### BucketTagging.get\_available\_subresources method

Returns a list of all the available sub-resources for this BucketTagging.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/buckettagging/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### BucketTagging.delete method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/buckettagging/delete.html)

```python
# delete method definition

await def delete(
    self,
    *,
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```



```python
# delete method usage example with argument unpacking

kwargs: DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef = {  # (1)
    "ExpectedBucketOwner": ...,
}

parent.delete(**kwargs)
```

1. See [:material-code-braces: DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef](./type_defs.md#deletebuckettaggingrequestbuckettaggingdeletetypedef) 

#### BucketTagging.put method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/buckettagging/put.html)

```python
# put method definition

await def put(
    self,
    *,
    Tagging: TaggingTypeDef,  # (1)
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (2)
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```

1. See [:material-code-braces: TaggingTypeDef](./type_defs.md#taggingtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 


```python
# put method usage example with argument unpacking

kwargs: PutBucketTaggingRequestBucketTaggingPutTypeDef = {  # (1)
    "Tagging": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutBucketTaggingRequestBucketTaggingPutTypeDef](./type_defs.md#putbuckettaggingrequestbuckettaggingputtypedef) 

#### BucketTagging.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/buckettagging/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
) -> _Bucket:
    ...
```


#### BucketTagging.load method



Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/buckettagging/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### BucketTagging.reload method



Type annotations and code completion for `#!python aiobotocore.resource("s3").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/buckettagging/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## BucketVersioning

Type annotations and code completion for `#!python session.resource("s3").BucketVersioning` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketversioning/index.html#S3.BucketVersioning)

```python
# BucketVersioning usage example

from types_aiobotocore_s3.service_resource import BucketVersioning

def get_resource() -> BucketVersioning:
    return session.resource("s3").BucketVersioning(...)
```


### BucketVersioning attributes


- `bucket_name`: `str`
- `status`: `Awaitable`[[BucketVersioningStatusType](./literals.md#bucketversioningstatustype)]
- `mfa_delete`: `Awaitable`[[MFADeleteStatusType](./literals.md#mfadeletestatustype)]
- `meta`: `S3ResourceMeta`





### BucketVersioning methods


#### BucketVersioning.get\_available\_subresources method

Returns a list of all the available sub-resources for this BucketVersioning.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketversioning/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### BucketVersioning.enable method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").enable` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketversioning/enable.html)

```python
# enable method definition

await def enable(
    self,
    *,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (1)
    MFA: str = ...,
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 


```python
# enable method usage example with argument unpacking

kwargs: PutBucketVersioningRequestBucketVersioningEnableTypeDef = {  # (1)
    "ChecksumAlgorithm": ...,
}

parent.enable(**kwargs)
```

1. See [:material-code-braces: PutBucketVersioningRequestBucketVersioningEnableTypeDef](./type_defs.md#putbucketversioningrequestbucketversioningenabletypedef) 

#### BucketVersioning.put method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketversioning/put.html)

```python
# put method definition

await def put(
    self,
    *,
    VersioningConfiguration: VersioningConfigurationTypeDef,  # (1)
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (2)
    MFA: str = ...,
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```

1. See [:material-code-braces: VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 


```python
# put method usage example with argument unpacking

kwargs: PutBucketVersioningRequestBucketVersioningPutTypeDef = {  # (1)
    "VersioningConfiguration": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutBucketVersioningRequestBucketVersioningPutTypeDef](./type_defs.md#putbucketversioningrequestbucketversioningputtypedef) 

#### BucketVersioning.suspend method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").suspend` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketversioning/suspend.html)

```python
# suspend method definition

await def suspend(
    self,
    *,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (1)
    MFA: str = ...,
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 


```python
# suspend method usage example with argument unpacking

kwargs: PutBucketVersioningRequestBucketVersioningSuspendTypeDef = {  # (1)
    "ChecksumAlgorithm": ...,
}

parent.suspend(**kwargs)
```

1. See [:material-code-braces: PutBucketVersioningRequestBucketVersioningSuspendTypeDef](./type_defs.md#putbucketversioningrequestbucketversioningsuspendtypedef) 

#### BucketVersioning.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketversioning/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
) -> _Bucket:
    ...
```


#### BucketVersioning.load method



Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketversioning/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### BucketVersioning.reload method



Type annotations and code completion for `#!python aiobotocore.resource("s3").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketversioning/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## BucketWebsite

Type annotations and code completion for `#!python session.resource("s3").BucketWebsite` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketwebsite/index.html#S3.BucketWebsite)

```python
# BucketWebsite usage example

from types_aiobotocore_s3.service_resource import BucketWebsite

def get_resource() -> BucketWebsite:
    return session.resource("s3").BucketWebsite(...)
```


### BucketWebsite attributes


- `bucket_name`: `str`
- `redirect_all_requests_to`: `Awaitable`[[RedirectAllRequestsToTypeDef](./type_defs.md#redirectallrequeststotypedef)]
- `index_document`: `Awaitable`[[IndexDocumentTypeDef](./type_defs.md#indexdocumenttypedef)]
- `error_document`: `Awaitable`[[ErrorDocumentTypeDef](./type_defs.md#errordocumenttypedef)]
- `routing_rules`: `Awaitable`[`List`[[RoutingRuleTypeDef](./type_defs.md#routingruletypedef)]]
- `meta`: `S3ResourceMeta`





### BucketWebsite methods


#### BucketWebsite.get\_available\_subresources method

Returns a list of all the available sub-resources for this BucketWebsite.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketwebsite/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### BucketWebsite.delete method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketwebsite/delete.html)

```python
# delete method definition

await def delete(
    self,
    *,
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```



```python
# delete method usage example with argument unpacking

kwargs: DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef = {  # (1)
    "ExpectedBucketOwner": ...,
}

parent.delete(**kwargs)
```

1. See [:material-code-braces: DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef](./type_defs.md#deletebucketwebsiterequestbucketwebsitedeletetypedef) 

#### BucketWebsite.put method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketwebsite/put.html)

```python
# put method definition

await def put(
    self,
    *,
    WebsiteConfiguration: WebsiteConfigurationTypeDef,  # (1)
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (2)
    ExpectedBucketOwner: str = ...,
) -> None:
    ...
```

1. See [:material-code-braces: WebsiteConfigurationTypeDef](./type_defs.md#websiteconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 


```python
# put method usage example with argument unpacking

kwargs: PutBucketWebsiteRequestBucketWebsitePutTypeDef = {  # (1)
    "WebsiteConfiguration": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutBucketWebsiteRequestBucketWebsitePutTypeDef](./type_defs.md#putbucketwebsiterequestbucketwebsiteputtypedef) 

#### BucketWebsite.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketwebsite/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
) -> _Bucket:
    ...
```


#### BucketWebsite.load method



Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketwebsite/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### BucketWebsite.reload method



Type annotations and code completion for `#!python aiobotocore.resource("s3").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/bucketwebsite/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## MultipartUpload

Type annotations and code completion for `#!python session.resource("s3").MultipartUpload` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/multipartupload/index.html#S3.MultipartUpload)

```python
# MultipartUpload usage example

from types_aiobotocore_s3.service_resource import MultipartUpload

def get_resource() -> MultipartUpload:
    return session.resource("s3").MultipartUpload(...)
```


### MultipartUpload attributes


- `bucket_name`: `str`
- `object_key`: `str`
- `id`: `str`
- `parts`: `MultipartUploadPartsCollection`
- `upload_id`: `Awaitable`[`str`]
- `key`: `Awaitable`[`str`]
- `initiated`: `Awaitable`[`datetime`]
- `storage_class`: `Awaitable`[[StorageClassType](./literals.md#storageclasstype)]
- `owner`: `Awaitable`[[OwnerTypeDef](./type_defs.md#ownertypedef)]
- `initiator`: `Awaitable`[[InitiatorTypeDef](./type_defs.md#initiatortypedef)]
- `checksum_algorithm`: `Awaitable`[[ChecksumAlgorithmType](./literals.md#checksumalgorithmtype)]
- `checksum_type`: `Awaitable`[[ChecksumTypeType](./literals.md#checksumtypetype)]
- `meta`: `S3ResourceMeta`



### MultipartUpload collections


#### MultipartUpload.parts

Provides access to [MultipartUploadPart](#multipartuploadpart) resource.

Type annotations and code completion for `#!python session.resource("s3").MultipartUpload(...).parts` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/multipartupload/parts.html#S3.MultipartUpload.parts)

```python
# MultipartUploadPartsCollection usage example

from types_aiobotocore_s3.service_resource import MultipartUploadPartsCollection

def get_collection() -> MultipartUploadPartsCollection:
    resource = session.resource("s3").MultipartUpload(...)
    return resource.parts
```




### MultipartUpload methods


#### MultipartUpload.get\_available\_subresources method

Returns a list of all the available sub-resources for this MultipartUpload.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/multipartupload/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### MultipartUpload.abort method

This operation aborts a multipart upload.

Type annotations and code completion for `#!python aiobotocore.resource("s3").abort` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/multipartupload/abort.html)

```python
# abort method definition

await def abort(
    self,
    *,
    RequestPayer: RequestPayerType = ...,  # (1)
    ExpectedBucketOwner: str = ...,
    IfMatchInitiatedTime: TimestampTypeDef = ...,
) -> AbortMultipartUploadOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-braces: AbortMultipartUploadOutputTypeDef](./type_defs.md#abortmultipartuploadoutputtypedef) 


```python
# abort method usage example with argument unpacking

kwargs: AbortMultipartUploadRequestMultipartUploadAbortTypeDef = {  # (1)
    "RequestPayer": ...,
}

parent.abort(**kwargs)
```

1. See [:material-code-braces: AbortMultipartUploadRequestMultipartUploadAbortTypeDef](./type_defs.md#abortmultipartuploadrequestmultipartuploadaborttypedef) 

#### MultipartUpload.complete method

Completes a multipart upload by assembling previously uploaded parts.

Type annotations and code completion for `#!python aiobotocore.resource("s3").complete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/multipartupload/complete.html)

```python
# complete method definition

await def complete(
    self,
    *,
    MultipartUpload: CompletedMultipartUploadTypeDef = ...,  # (1)
    ChecksumCRC32: str = ...,
    ChecksumCRC32C: str = ...,
    ChecksumCRC64NVME: str = ...,
    ChecksumSHA1: str = ...,
    ChecksumSHA256: str = ...,
    ChecksumType: ChecksumTypeType = ...,  # (2)
    MpuObjectSize: int = ...,
    RequestPayer: RequestPayerType = ...,  # (3)
    ExpectedBucketOwner: str = ...,
    IfMatch: str = ...,
    IfNoneMatch: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
) -> _Object:
    ...
```

1. See [:material-code-braces: CompletedMultipartUploadTypeDef](./type_defs.md#completedmultipartuploadtypedef) 
2. See [:material-code-brackets: ChecksumTypeType](./literals.md#checksumtypetype) 
3. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 


```python
# complete method usage example with argument unpacking

kwargs: CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef = {  # (1)
    "MultipartUpload": ...,
}

parent.complete(**kwargs)
```

1. See [:material-code-braces: CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef](./type_defs.md#completemultipartuploadrequestmultipartuploadcompletetypedef) 

#### MultipartUpload.Object method

Creates a Object resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Object` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/multipartupload/Object.html)

```python
# Object method definition

await def Object(
    self,
) -> _Object:
    ...
```


#### MultipartUpload.Part method

Creates a MultipartUploadPart resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Part` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/multipartupload/Part.html)

```python
# Part method definition

await def Part(
    self,
    part_number: int,
) -> _MultipartUploadPart:
    ...
```





## MultipartUploadPart

Type annotations and code completion for `#!python session.resource("s3").MultipartUploadPart` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/multipartuploadpart/index.html#S3.MultipartUploadPart)

```python
# MultipartUploadPart usage example

from types_aiobotocore_s3.service_resource import MultipartUploadPart

def get_resource() -> MultipartUploadPart:
    return session.resource("s3").MultipartUploadPart(...)
```


### MultipartUploadPart attributes


- `bucket_name`: `str`
- `object_key`: `str`
- `multipart_upload_id`: `str`
- `part_number`: `int`
- `last_modified`: `Awaitable`[`datetime`]
- `e_tag`: `Awaitable`[`str`]
- `size`: `Awaitable`[`int`]
- `checksum_crc32`: `Awaitable`[`str`]
- `checksum_crc32_c`: `Awaitable`[`str`]
- `checksum_crc64_nvme`: `Awaitable`[`str`]
- `checksum_sha1`: `Awaitable`[`str`]
- `checksum_sha256`: `Awaitable`[`str`]
- `meta`: `S3ResourceMeta`





### MultipartUploadPart methods


#### MultipartUploadPart.get\_available\_subresources method

Returns a list of all the available sub-resources for this MultipartUploadPart.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/multipartuploadpart/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### MultipartUploadPart.copy\_from method

Uploads a part by copying data from an existing object as data source.

Type annotations and code completion for `#!python aiobotocore.resource("s3").copy_from` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/multipartuploadpart/copy_from.html)

```python
# copy_from method definition

await def copy_from(
    self,
    *,
    CopySource: CopySourceOrStrTypeDef,  # (1)
    CopySourceIfMatch: str = ...,
    CopySourceIfModifiedSince: TimestampTypeDef = ...,
    CopySourceIfNoneMatch: str = ...,
    CopySourceIfUnmodifiedSince: TimestampTypeDef = ...,
    CopySourceRange: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    CopySourceSSECustomerAlgorithm: str = ...,
    CopySourceSSECustomerKey: Union[str, bytes] = ...,
    RequestPayer: RequestPayerType = ...,  # (2)
    ExpectedBucketOwner: str = ...,
    ExpectedSourceBucketOwner: str = ...,
) -> UploadPartCopyOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: CopySourceTypeDef](./type_defs.md#copysourcetypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-braces: UploadPartCopyOutputTypeDef](./type_defs.md#uploadpartcopyoutputtypedef) 


```python
# copy_from method usage example with argument unpacking

kwargs: UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef = {  # (1)
    "CopySource": ...,
}

parent.copy_from(**kwargs)
```

1. See [:material-code-braces: UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef](./type_defs.md#uploadpartcopyrequestmultipartuploadpartcopyfromtypedef) 

#### MultipartUploadPart.upload method

Uploads a part in a multipart upload.

Type annotations and code completion for `#!python aiobotocore.resource("s3").upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/multipartuploadpart/upload.html)

```python
# upload method definition

await def upload(
    self,
    *,
    Body: BlobTypeDef = ...,
    ContentLength: int = ...,
    ContentMD5: str = ...,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (1)
    ChecksumCRC32: str = ...,
    ChecksumCRC32C: str = ...,
    ChecksumCRC64NVME: str = ...,
    ChecksumSHA1: str = ...,
    ChecksumSHA256: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    RequestPayer: RequestPayerType = ...,  # (2)
    ExpectedBucketOwner: str = ...,
) -> UploadPartOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-braces: UploadPartOutputTypeDef](./type_defs.md#uploadpartoutputtypedef) 


```python
# upload method usage example with argument unpacking

kwargs: UploadPartRequestMultipartUploadPartUploadTypeDef = {  # (1)
    "Body": ...,
}

parent.upload(**kwargs)
```

1. See [:material-code-braces: UploadPartRequestMultipartUploadPartUploadTypeDef](./type_defs.md#uploadpartrequestmultipartuploadpartuploadtypedef) 

#### MultipartUploadPart.MultipartUpload method

Creates a MultipartUpload resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").MultipartUpload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/multipartuploadpart/MultipartUpload.html)

```python
# MultipartUpload method definition

await def MultipartUpload(
    self,
) -> _MultipartUpload:
    ...
```





## Object

Type annotations and code completion for `#!python session.resource("s3").Object` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/index.html#S3.Object)

```python
# Object usage example

from types_aiobotocore_s3.service_resource import Object

def get_resource() -> Object:
    return session.resource("s3").Object(...)
```


### Object attributes


- `bucket_name`: `str`
- `key`: `str`
- `delete_marker`: `Awaitable`[`bool`]
- `accept_ranges`: `Awaitable`[`str`]
- `expiration`: `Awaitable`[`str`]
- `restore`: `Awaitable`[`str`]
- `archive_status`: `Awaitable`[[ArchiveStatusType](./literals.md#archivestatustype)]
- `last_modified`: `Awaitable`[`datetime`]
- `content_length`: `Awaitable`[`int`]
- `checksum_crc32`: `Awaitable`[`str`]
- `checksum_crc32_c`: `Awaitable`[`str`]
- `checksum_crc64_nvme`: `Awaitable`[`str`]
- `checksum_sha1`: `Awaitable`[`str`]
- `checksum_sha256`: `Awaitable`[`str`]
- `checksum_type`: `Awaitable`[[ChecksumTypeType](./literals.md#checksumtypetype)]
- `e_tag`: `Awaitable`[`str`]
- `missing_meta`: `Awaitable`[`int`]
- `version_id`: `Awaitable`[`str`]
- `cache_control`: `Awaitable`[`str`]
- `content_disposition`: `Awaitable`[`str`]
- `content_encoding`: `Awaitable`[`str`]
- `content_language`: `Awaitable`[`str`]
- `content_type`: `Awaitable`[`str`]
- `content_range`: `Awaitable`[`str`]
- `expires`: `Awaitable`[`datetime`]
- `website_redirect_location`: `Awaitable`[`str`]
- `server_side_encryption`: `Awaitable`[[ServerSideEncryptionType](./literals.md#serversideencryptiontype)]
- `metadata`: `Awaitable`[`Dict`[`str`, `str`]]
- `sse_customer_algorithm`: `Awaitable`[`str`]
- `sse_customer_key_md5`: `Awaitable`[`str`]
- `ssekms_key_id`: `Awaitable`[`str`]
- `bucket_key_enabled`: `Awaitable`[`bool`]
- `storage_class`: `Awaitable`[[StorageClassType](./literals.md#storageclasstype)]
- `request_charged`: `Awaitable`[`Literal['requester']` (see [RequestChargedType](./literals.md#requestchargedtype))]
- `replication_status`: `Awaitable`[[ReplicationStatusType](./literals.md#replicationstatustype)]
- `parts_count`: `Awaitable`[`int`]
- `object_lock_mode`: `Awaitable`[[ObjectLockModeType](./literals.md#objectlockmodetype)]
- `object_lock_retain_until_date`: `Awaitable`[`datetime`]
- `object_lock_legal_hold_status`: `Awaitable`[[ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype)]
- `meta`: `S3ResourceMeta`





### Object methods


#### Object.get\_available\_subresources method

Returns a list of all the available sub-resources for this Object.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Object.copy\_from method

Creates a copy of an object that is already stored in Amazon S3.

Type annotations and code completion for `#!python aiobotocore.resource("s3").copy_from` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/copy_from.html)

```python
# copy_from method definition

await def copy_from(
    self,
    *,
    CopySource: CopySourceOrStrTypeDef,  # (1)
    ACL: ObjectCannedACLType = ...,  # (2)
    CacheControl: str = ...,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (3)
    ContentDisposition: str = ...,
    ContentEncoding: str = ...,
    ContentLanguage: str = ...,
    ContentType: str = ...,
    CopySourceIfMatch: str = ...,
    CopySourceIfModifiedSince: TimestampTypeDef = ...,
    CopySourceIfNoneMatch: str = ...,
    CopySourceIfUnmodifiedSince: TimestampTypeDef = ...,
    Expires: TimestampTypeDef = ...,
    GrantFullControl: str = ...,
    GrantRead: str = ...,
    GrantReadACP: str = ...,
    GrantWriteACP: str = ...,
    Metadata: Mapping[str, str] = ...,
    MetadataDirective: MetadataDirectiveType = ...,  # (4)
    TaggingDirective: TaggingDirectiveType = ...,  # (5)
    ServerSideEncryption: ServerSideEncryptionType = ...,  # (6)
    StorageClass: StorageClassType = ...,  # (7)
    WebsiteRedirectLocation: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    SSEKMSKeyId: str = ...,
    SSEKMSEncryptionContext: str = ...,
    BucketKeyEnabled: bool = ...,
    CopySourceSSECustomerAlgorithm: str = ...,
    CopySourceSSECustomerKey: Union[str, bytes] = ...,
    RequestPayer: RequestPayerType = ...,  # (8)
    Tagging: str = ...,
    ObjectLockMode: ObjectLockModeType = ...,  # (9)
    ObjectLockRetainUntilDate: TimestampTypeDef = ...,
    ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,  # (10)
    ExpectedBucketOwner: str = ...,
    ExpectedSourceBucketOwner: str = ...,
) -> CopyObjectOutputTypeDef:  # (11)
    ...
```

1. See [:material-code-braces: CopySourceTypeDef](./type_defs.md#copysourcetypedef) 
2. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
4. See [:material-code-brackets: MetadataDirectiveType](./literals.md#metadatadirectivetype) 
5. See [:material-code-brackets: TaggingDirectiveType](./literals.md#taggingdirectivetype) 
6. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
7. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
8. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
9. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
10. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
11. See [:material-code-braces: CopyObjectOutputTypeDef](./type_defs.md#copyobjectoutputtypedef) 


```python
# copy_from method usage example with argument unpacking

kwargs: CopyObjectRequestObjectCopyFromTypeDef = {  # (1)
    "CopySource": ...,
}

parent.copy_from(**kwargs)
```

1. See [:material-code-braces: CopyObjectRequestObjectCopyFromTypeDef](./type_defs.md#copyobjectrequestobjectcopyfromtypedef) 

#### Object.delete method

Removes an object from a bucket.

Type annotations and code completion for `#!python aiobotocore.resource("s3").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/delete.html)

```python
# delete method definition

await def delete(
    self,
    *,
    MFA: str = ...,
    VersionId: str = ...,
    RequestPayer: RequestPayerType = ...,  # (1)
    BypassGovernanceRetention: bool = ...,
    ExpectedBucketOwner: str = ...,
    IfMatch: str = ...,
    IfMatchLastModifiedTime: TimestampTypeDef = ...,
    IfMatchSize: int = ...,
) -> DeleteObjectOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-braces: DeleteObjectOutputTypeDef](./type_defs.md#deleteobjectoutputtypedef) 


```python
# delete method usage example with argument unpacking

kwargs: DeleteObjectRequestObjectDeleteTypeDef = {  # (1)
    "MFA": ...,
}

parent.delete(**kwargs)
```

1. See [:material-code-braces: DeleteObjectRequestObjectDeleteTypeDef](./type_defs.md#deleteobjectrequestobjectdeletetypedef) 

#### Object.get method

Retrieves an object from Amazon S3.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/get.html)

```python
# get method definition

await def get(
    self,
    *,
    IfMatch: str = ...,
    IfModifiedSince: TimestampTypeDef = ...,
    IfNoneMatch: str = ...,
    IfUnmodifiedSince: TimestampTypeDef = ...,
    Range: str = ...,
    ResponseCacheControl: str = ...,
    ResponseContentDisposition: str = ...,
    ResponseContentEncoding: str = ...,
    ResponseContentLanguage: str = ...,
    ResponseContentType: str = ...,
    ResponseExpires: TimestampTypeDef = ...,
    VersionId: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    RequestPayer: RequestPayerType = ...,  # (1)
    PartNumber: int = ...,
    ExpectedBucketOwner: str = ...,
    ChecksumMode: ChecksumModeType = ...,  # (2)
) -> GetObjectOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-brackets: ChecksumModeType](./literals.md#checksummodetype) 
3. See [:material-code-braces: GetObjectOutputTypeDef](./type_defs.md#getobjectoutputtypedef) 


```python
# get method usage example with argument unpacking

kwargs: GetObjectRequestObjectGetTypeDef = {  # (1)
    "IfMatch": ...,
}

parent.get(**kwargs)
```

1. See [:material-code-braces: GetObjectRequestObjectGetTypeDef](./type_defs.md#getobjectrequestobjectgettypedef) 

#### Object.initiate\_multipart\_upload method

This action initiates a multipart upload and returns an upload ID.

Type annotations and code completion for `#!python aiobotocore.resource("s3").initiate_multipart_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/initiate_multipart_upload.html)

```python
# initiate_multipart_upload method definition

await def initiate_multipart_upload(
    self,
    *,
    ACL: ObjectCannedACLType = ...,  # (1)
    CacheControl: str = ...,
    ContentDisposition: str = ...,
    ContentEncoding: str = ...,
    ContentLanguage: str = ...,
    ContentType: str = ...,
    Expires: TimestampTypeDef = ...,
    GrantFullControl: str = ...,
    GrantRead: str = ...,
    GrantReadACP: str = ...,
    GrantWriteACP: str = ...,
    Metadata: Mapping[str, str] = ...,
    ServerSideEncryption: ServerSideEncryptionType = ...,  # (2)
    StorageClass: StorageClassType = ...,  # (3)
    WebsiteRedirectLocation: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    SSEKMSKeyId: str = ...,
    SSEKMSEncryptionContext: str = ...,
    BucketKeyEnabled: bool = ...,
    RequestPayer: RequestPayerType = ...,  # (4)
    Tagging: str = ...,
    ObjectLockMode: ObjectLockModeType = ...,  # (5)
    ObjectLockRetainUntilDate: TimestampTypeDef = ...,
    ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,  # (6)
    ExpectedBucketOwner: str = ...,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (7)
    ChecksumType: ChecksumTypeType = ...,  # (8)
) -> _MultipartUpload:
    ...
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
3. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
4. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
5. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
6. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
7. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
8. See [:material-code-brackets: ChecksumTypeType](./literals.md#checksumtypetype) 


```python
# initiate_multipart_upload method usage example with argument unpacking

kwargs: CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef = {  # (1)
    "ACL": ...,
}

parent.initiate_multipart_upload(**kwargs)
```

1. See [:material-code-braces: CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef](./type_defs.md#createmultipartuploadrequestobjectinitiatemultipartuploadtypedef) 

#### Object.put method

Adds an object to a bucket.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/put.html)

```python
# put method definition

await def put(
    self,
    *,
    ACL: ObjectCannedACLType = ...,  # (1)
    Body: BlobTypeDef = ...,
    CacheControl: str = ...,
    ContentDisposition: str = ...,
    ContentEncoding: str = ...,
    ContentLanguage: str = ...,
    ContentLength: int = ...,
    ContentMD5: str = ...,
    ContentType: str = ...,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (2)
    ChecksumCRC32: str = ...,
    ChecksumCRC32C: str = ...,
    ChecksumCRC64NVME: str = ...,
    ChecksumSHA1: str = ...,
    ChecksumSHA256: str = ...,
    Expires: TimestampTypeDef = ...,
    IfMatch: str = ...,
    IfNoneMatch: str = ...,
    GrantFullControl: str = ...,
    GrantRead: str = ...,
    GrantReadACP: str = ...,
    GrantWriteACP: str = ...,
    WriteOffsetBytes: int = ...,
    Metadata: Mapping[str, str] = ...,
    ServerSideEncryption: ServerSideEncryptionType = ...,  # (3)
    StorageClass: StorageClassType = ...,  # (4)
    WebsiteRedirectLocation: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    SSEKMSKeyId: str = ...,
    SSEKMSEncryptionContext: str = ...,
    BucketKeyEnabled: bool = ...,
    RequestPayer: RequestPayerType = ...,  # (5)
    Tagging: str = ...,
    ObjectLockMode: ObjectLockModeType = ...,  # (6)
    ObjectLockRetainUntilDate: TimestampTypeDef = ...,
    ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,  # (7)
    ExpectedBucketOwner: str = ...,
) -> PutObjectOutputTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
3. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
4. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
5. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
6. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
7. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
8. See [:material-code-braces: PutObjectOutputTypeDef](./type_defs.md#putobjectoutputtypedef) 


```python
# put method usage example with argument unpacking

kwargs: PutObjectRequestObjectPutTypeDef = {  # (1)
    "ACL": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutObjectRequestObjectPutTypeDef](./type_defs.md#putobjectrequestobjectputtypedef) 

#### Object.restore\_object method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").restore_object` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/restore_object.html)

```python
# restore_object method definition

await def restore_object(
    self,
    *,
    VersionId: str = ...,
    RestoreRequest: RestoreRequestTypeDef = ...,  # (1)
    RequestPayer: RequestPayerType = ...,  # (2)
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (3)
    ExpectedBucketOwner: str = ...,
) -> RestoreObjectOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RestoreRequestTypeDef](./type_defs.md#restorerequesttypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
4. See [:material-code-braces: RestoreObjectOutputTypeDef](./type_defs.md#restoreobjectoutputtypedef) 


```python
# restore_object method usage example with argument unpacking

kwargs: RestoreObjectRequestObjectRestoreObjectTypeDef = {  # (1)
    "VersionId": ...,
}

parent.restore_object(**kwargs)
```

1. See [:material-code-braces: RestoreObjectRequestObjectRestoreObjectTypeDef](./type_defs.md#restoreobjectrequestobjectrestoreobjecttypedef) 

#### Object.wait\_until\_exists method

Waits until Object is exists.

Type annotations and code completion for `#!python aiobotocore.resource("s3").wait_until_exists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/wait_until_exists.html)

```python
# wait_until_exists method definition

await def wait_until_exists(
    self,
) -> None:
    ...
```


#### Object.wait\_until\_not\_exists method

Waits until Object is not_exists.

Type annotations and code completion for `#!python aiobotocore.resource("s3").wait_until_not_exists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/wait_until_not_exists.html)

```python
# wait_until_not_exists method definition

await def wait_until_not_exists(
    self,
) -> None:
    ...
```


#### Object.Acl method

Creates a ObjectAcl resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/Acl.html)

```python
# Acl method definition

await def Acl(
    self,
) -> _ObjectAcl:
    ...
```


#### Object.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
) -> _Bucket:
    ...
```


#### Object.MultipartUpload method

Creates a MultipartUpload resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").MultipartUpload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/MultipartUpload.html)

```python
# MultipartUpload method definition

await def MultipartUpload(
    self,
    id: str,
) -> _MultipartUpload:
    ...
```


#### Object.Version method

Creates a ObjectVersion resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/Version.html)

```python
# Version method definition

await def Version(
    self,
    id: str,
) -> _ObjectVersion:
    ...
```


#### Object.copy method

Copy an object from one S3 location to another.

Type annotations and code completion for `#!python aiobotocore.resource("s3").copy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/copy.html)

```python
# copy method definition

await def copy(
    self,
    CopySource: CopySourceTypeDef,  # (1)
    ExtraArgs: Union[Dict[str, Any], None] = ...,
    Callback: Union[Callable[..., Any], None] = ...,
    SourceClient: Union[AioBaseClient, None] = ...,
    Config: Union[TransferConfig, None] = ...,
) -> None:
    ...
```

1. See [:material-code-braces: CopySourceTypeDef](./type_defs.md#copysourcetypedef) 


```python
# copy method usage example with argument unpacking

kwargs: ObjectCopyRequestTypeDef = {  # (1)
    "CopySource": ...,
}

parent.copy(**kwargs)
```

1. See [:material-code-braces: ObjectCopyRequestTypeDef](./type_defs.md#objectcopyrequesttypedef) 

#### Object.download\_file method

Download an object from S3 to a file.

Type annotations and code completion for `#!python aiobotocore.resource("s3").download_file` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/download_file.html)

```python
# download_file method definition

await def download_file(
    self,
    Filename: str,
    ExtraArgs: Union[Dict[str, Any], None] = ...,
    Callback: Union[Callable[..., Any], None] = ...,
    Config: Union[TransferConfig, None] = ...,
) -> None:
    ...
```



```python
# download_file method usage example with argument unpacking

kwargs: ObjectDownloadFileRequestTypeDef = {  # (1)
    "Filename": ...,
}

parent.download_file(**kwargs)
```

1. See [:material-code-braces: ObjectDownloadFileRequestTypeDef](./type_defs.md#objectdownloadfilerequesttypedef) 

#### Object.download\_fileobj method

Download an object from S3 to a file-like object.

Type annotations and code completion for `#!python aiobotocore.resource("s3").download_fileobj` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/download_fileobj.html)

```python
# download_fileobj method definition

await def download_fileobj(
    self,
    Fileobj: FileobjTypeDef,
    ExtraArgs: Union[Dict[str, Any], None] = ...,
    Callback: Union[Callable[..., Any], None] = ...,
    Config: Union[TransferConfig, None] = ...,
) -> None:
    ...
```



```python
# download_fileobj method usage example with argument unpacking

kwargs: ObjectDownloadFileobjRequestTypeDef = {  # (1)
    "Fileobj": ...,
}

parent.download_fileobj(**kwargs)
```

1. See [:material-code-braces: ObjectDownloadFileobjRequestTypeDef](./type_defs.md#objectdownloadfileobjrequesttypedef) 

#### Object.upload\_file method

Upload a file to S3.

Type annotations and code completion for `#!python aiobotocore.resource("s3").upload_file` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/upload_file.html)

```python
# upload_file method definition

await def upload_file(
    self,
    Filename: str,
    ExtraArgs: Union[Dict[str, Any], None] = ...,
    Callback: Union[Callable[..., Any], None] = ...,
    Config: Union[TransferConfig, None] = ...,
) -> None:
    ...
```



```python
# upload_file method usage example with argument unpacking

kwargs: ObjectUploadFileRequestTypeDef = {  # (1)
    "Filename": ...,
}

parent.upload_file(**kwargs)
```

1. See [:material-code-braces: ObjectUploadFileRequestTypeDef](./type_defs.md#objectuploadfilerequesttypedef) 

#### Object.upload\_fileobj method

Upload a file-like object to S3.

Type annotations and code completion for `#!python aiobotocore.resource("s3").upload_fileobj` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/upload_fileobj.html)

```python
# upload_fileobj method definition

await def upload_fileobj(
    self,
    Fileobj: FileobjTypeDef,
    ExtraArgs: Union[Dict[str, Any], None] = ...,
    Callback: Union[Callable[..., Any], None] = ...,
    Config: Union[TransferConfig, None] = ...,
) -> None:
    ...
```



```python
# upload_fileobj method usage example with argument unpacking

kwargs: ObjectUploadFileobjRequestTypeDef = {  # (1)
    "Fileobj": ...,
}

parent.upload_fileobj(**kwargs)
```

1. See [:material-code-braces: ObjectUploadFileobjRequestTypeDef](./type_defs.md#objectuploadfileobjrequesttypedef) 

#### Object.load method



Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Object.reload method



Type annotations and code completion for `#!python aiobotocore.resource("s3").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/object/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## ObjectAcl

Type annotations and code completion for `#!python session.resource("s3").ObjectAcl` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectacl/index.html#S3.ObjectAcl)

```python
# ObjectAcl usage example

from types_aiobotocore_s3.service_resource import ObjectAcl

def get_resource() -> ObjectAcl:
    return session.resource("s3").ObjectAcl(...)
```


### ObjectAcl attributes


- `bucket_name`: `str`
- `object_key`: `str`
- `owner`: `Awaitable`[[OwnerTypeDef](./type_defs.md#ownertypedef)]
- `grants`: `Awaitable`[`List`[[GrantTypeDef](./type_defs.md#granttypedef)]]
- `request_charged`: `Awaitable`[`Literal['requester']` (see [RequestChargedType](./literals.md#requestchargedtype))]
- `meta`: `S3ResourceMeta`





### ObjectAcl methods


#### ObjectAcl.get\_available\_subresources method

Returns a list of all the available sub-resources for this ObjectAcl.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectacl/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### ObjectAcl.put method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectacl/put.html)

```python
# put method definition

await def put(
    self,
    *,
    ACL: ObjectCannedACLType = ...,  # (1)
    AccessControlPolicy: AccessControlPolicyTypeDef = ...,  # (2)
    ContentMD5: str = ...,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (3)
    GrantFullControl: str = ...,
    GrantRead: str = ...,
    GrantReadACP: str = ...,
    GrantWrite: str = ...,
    GrantWriteACP: str = ...,
    RequestPayer: RequestPayerType = ...,  # (4)
    VersionId: str = ...,
    ExpectedBucketOwner: str = ...,
) -> PutObjectAclOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-braces: AccessControlPolicyTypeDef](./type_defs.md#accesscontrolpolicytypedef) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
4. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
5. See [:material-code-braces: PutObjectAclOutputTypeDef](./type_defs.md#putobjectacloutputtypedef) 


```python
# put method usage example with argument unpacking

kwargs: PutObjectAclRequestObjectAclPutTypeDef = {  # (1)
    "ACL": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutObjectAclRequestObjectAclPutTypeDef](./type_defs.md#putobjectaclrequestobjectaclputtypedef) 

#### ObjectAcl.Object method

Creates a Object resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Object` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectacl/Object.html)

```python
# Object method definition

await def Object(
    self,
) -> _Object:
    ...
```


#### ObjectAcl.load method



Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectacl/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### ObjectAcl.reload method



Type annotations and code completion for `#!python aiobotocore.resource("s3").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectacl/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## ObjectSummary

Type annotations and code completion for `#!python session.resource("s3").ObjectSummary` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/index.html#S3.ObjectSummary)

```python
# ObjectSummary usage example

from types_aiobotocore_s3.service_resource import ObjectSummary

def get_resource() -> ObjectSummary:
    return session.resource("s3").ObjectSummary(...)
```


### ObjectSummary attributes


- `bucket_name`: `str`
- `key`: `str`
- `last_modified`: `Awaitable`[`datetime`]
- `e_tag`: `Awaitable`[`str`]
- `checksum_algorithm`: `Awaitable`[`List`[[ChecksumAlgorithmType](./literals.md#checksumalgorithmtype)]]
- `checksum_type`: `Awaitable`[[ChecksumTypeType](./literals.md#checksumtypetype)]
- `size`: `Awaitable`[`int`]
- `storage_class`: `Awaitable`[[ObjectStorageClassType](./literals.md#objectstorageclasstype)]
- `owner`: `Awaitable`[[OwnerTypeDef](./type_defs.md#ownertypedef)]
- `restore_status`: `Awaitable`[[RestoreStatusTypeDef](./type_defs.md#restorestatustypedef)]
- `meta`: `S3ResourceMeta`





### ObjectSummary methods


#### ObjectSummary.get\_available\_subresources method

Returns a list of all the available sub-resources for this ObjectSummary.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### ObjectSummary.copy\_from method

Creates a copy of an object that is already stored in Amazon S3.

Type annotations and code completion for `#!python aiobotocore.resource("s3").copy_from` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/copy_from.html)

```python
# copy_from method definition

await def copy_from(
    self,
    *,
    CopySource: CopySourceOrStrTypeDef,  # (1)
    ACL: ObjectCannedACLType = ...,  # (2)
    CacheControl: str = ...,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (3)
    ContentDisposition: str = ...,
    ContentEncoding: str = ...,
    ContentLanguage: str = ...,
    ContentType: str = ...,
    CopySourceIfMatch: str = ...,
    CopySourceIfModifiedSince: TimestampTypeDef = ...,
    CopySourceIfNoneMatch: str = ...,
    CopySourceIfUnmodifiedSince: TimestampTypeDef = ...,
    Expires: TimestampTypeDef = ...,
    GrantFullControl: str = ...,
    GrantRead: str = ...,
    GrantReadACP: str = ...,
    GrantWriteACP: str = ...,
    Metadata: Mapping[str, str] = ...,
    MetadataDirective: MetadataDirectiveType = ...,  # (4)
    TaggingDirective: TaggingDirectiveType = ...,  # (5)
    ServerSideEncryption: ServerSideEncryptionType = ...,  # (6)
    StorageClass: StorageClassType = ...,  # (7)
    WebsiteRedirectLocation: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    SSEKMSKeyId: str = ...,
    SSEKMSEncryptionContext: str = ...,
    BucketKeyEnabled: bool = ...,
    CopySourceSSECustomerAlgorithm: str = ...,
    CopySourceSSECustomerKey: Union[str, bytes] = ...,
    RequestPayer: RequestPayerType = ...,  # (8)
    Tagging: str = ...,
    ObjectLockMode: ObjectLockModeType = ...,  # (9)
    ObjectLockRetainUntilDate: TimestampTypeDef = ...,
    ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,  # (10)
    ExpectedBucketOwner: str = ...,
    ExpectedSourceBucketOwner: str = ...,
) -> CopyObjectOutputTypeDef:  # (11)
    ...
```

1. See [:material-code-braces: CopySourceTypeDef](./type_defs.md#copysourcetypedef) 
2. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
4. See [:material-code-brackets: MetadataDirectiveType](./literals.md#metadatadirectivetype) 
5. See [:material-code-brackets: TaggingDirectiveType](./literals.md#taggingdirectivetype) 
6. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
7. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
8. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
9. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
10. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
11. See [:material-code-braces: CopyObjectOutputTypeDef](./type_defs.md#copyobjectoutputtypedef) 


```python
# copy_from method usage example with argument unpacking

kwargs: CopyObjectRequestObjectSummaryCopyFromTypeDef = {  # (1)
    "CopySource": ...,
}

parent.copy_from(**kwargs)
```

1. See [:material-code-braces: CopyObjectRequestObjectSummaryCopyFromTypeDef](./type_defs.md#copyobjectrequestobjectsummarycopyfromtypedef) 

#### ObjectSummary.delete method

Removes an object from a bucket.

Type annotations and code completion for `#!python aiobotocore.resource("s3").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/delete.html)

```python
# delete method definition

await def delete(
    self,
    *,
    MFA: str = ...,
    VersionId: str = ...,
    RequestPayer: RequestPayerType = ...,  # (1)
    BypassGovernanceRetention: bool = ...,
    ExpectedBucketOwner: str = ...,
    IfMatch: str = ...,
    IfMatchLastModifiedTime: TimestampTypeDef = ...,
    IfMatchSize: int = ...,
) -> DeleteObjectOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-braces: DeleteObjectOutputTypeDef](./type_defs.md#deleteobjectoutputtypedef) 


```python
# delete method usage example with argument unpacking

kwargs: DeleteObjectRequestObjectSummaryDeleteTypeDef = {  # (1)
    "MFA": ...,
}

parent.delete(**kwargs)
```

1. See [:material-code-braces: DeleteObjectRequestObjectSummaryDeleteTypeDef](./type_defs.md#deleteobjectrequestobjectsummarydeletetypedef) 

#### ObjectSummary.get method

Retrieves an object from Amazon S3.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/get.html)

```python
# get method definition

await def get(
    self,
    *,
    IfMatch: str = ...,
    IfModifiedSince: TimestampTypeDef = ...,
    IfNoneMatch: str = ...,
    IfUnmodifiedSince: TimestampTypeDef = ...,
    Range: str = ...,
    ResponseCacheControl: str = ...,
    ResponseContentDisposition: str = ...,
    ResponseContentEncoding: str = ...,
    ResponseContentLanguage: str = ...,
    ResponseContentType: str = ...,
    ResponseExpires: TimestampTypeDef = ...,
    VersionId: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    RequestPayer: RequestPayerType = ...,  # (1)
    PartNumber: int = ...,
    ExpectedBucketOwner: str = ...,
    ChecksumMode: ChecksumModeType = ...,  # (2)
) -> GetObjectOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-brackets: ChecksumModeType](./literals.md#checksummodetype) 
3. See [:material-code-braces: GetObjectOutputTypeDef](./type_defs.md#getobjectoutputtypedef) 


```python
# get method usage example with argument unpacking

kwargs: GetObjectRequestObjectSummaryGetTypeDef = {  # (1)
    "IfMatch": ...,
}

parent.get(**kwargs)
```

1. See [:material-code-braces: GetObjectRequestObjectSummaryGetTypeDef](./type_defs.md#getobjectrequestobjectsummarygettypedef) 

#### ObjectSummary.initiate\_multipart\_upload method

This action initiates a multipart upload and returns an upload ID.

Type annotations and code completion for `#!python aiobotocore.resource("s3").initiate_multipart_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/initiate_multipart_upload.html)

```python
# initiate_multipart_upload method definition

await def initiate_multipart_upload(
    self,
    *,
    ACL: ObjectCannedACLType = ...,  # (1)
    CacheControl: str = ...,
    ContentDisposition: str = ...,
    ContentEncoding: str = ...,
    ContentLanguage: str = ...,
    ContentType: str = ...,
    Expires: TimestampTypeDef = ...,
    GrantFullControl: str = ...,
    GrantRead: str = ...,
    GrantReadACP: str = ...,
    GrantWriteACP: str = ...,
    Metadata: Mapping[str, str] = ...,
    ServerSideEncryption: ServerSideEncryptionType = ...,  # (2)
    StorageClass: StorageClassType = ...,  # (3)
    WebsiteRedirectLocation: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    SSEKMSKeyId: str = ...,
    SSEKMSEncryptionContext: str = ...,
    BucketKeyEnabled: bool = ...,
    RequestPayer: RequestPayerType = ...,  # (4)
    Tagging: str = ...,
    ObjectLockMode: ObjectLockModeType = ...,  # (5)
    ObjectLockRetainUntilDate: TimestampTypeDef = ...,
    ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,  # (6)
    ExpectedBucketOwner: str = ...,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (7)
    ChecksumType: ChecksumTypeType = ...,  # (8)
) -> _MultipartUpload:
    ...
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
3. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
4. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
5. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
6. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
7. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
8. See [:material-code-brackets: ChecksumTypeType](./literals.md#checksumtypetype) 


```python
# initiate_multipart_upload method usage example with argument unpacking

kwargs: CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef = {  # (1)
    "ACL": ...,
}

parent.initiate_multipart_upload(**kwargs)
```

1. See [:material-code-braces: CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef](./type_defs.md#createmultipartuploadrequestobjectsummaryinitiatemultipartuploadtypedef) 

#### ObjectSummary.put method

Adds an object to a bucket.

Type annotations and code completion for `#!python aiobotocore.resource("s3").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/put.html)

```python
# put method definition

await def put(
    self,
    *,
    ACL: ObjectCannedACLType = ...,  # (1)
    Body: BlobTypeDef = ...,
    CacheControl: str = ...,
    ContentDisposition: str = ...,
    ContentEncoding: str = ...,
    ContentLanguage: str = ...,
    ContentLength: int = ...,
    ContentMD5: str = ...,
    ContentType: str = ...,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (2)
    ChecksumCRC32: str = ...,
    ChecksumCRC32C: str = ...,
    ChecksumCRC64NVME: str = ...,
    ChecksumSHA1: str = ...,
    ChecksumSHA256: str = ...,
    Expires: TimestampTypeDef = ...,
    IfMatch: str = ...,
    IfNoneMatch: str = ...,
    GrantFullControl: str = ...,
    GrantRead: str = ...,
    GrantReadACP: str = ...,
    GrantWriteACP: str = ...,
    WriteOffsetBytes: int = ...,
    Metadata: Mapping[str, str] = ...,
    ServerSideEncryption: ServerSideEncryptionType = ...,  # (3)
    StorageClass: StorageClassType = ...,  # (4)
    WebsiteRedirectLocation: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    SSEKMSKeyId: str = ...,
    SSEKMSEncryptionContext: str = ...,
    BucketKeyEnabled: bool = ...,
    RequestPayer: RequestPayerType = ...,  # (5)
    Tagging: str = ...,
    ObjectLockMode: ObjectLockModeType = ...,  # (6)
    ObjectLockRetainUntilDate: TimestampTypeDef = ...,
    ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,  # (7)
    ExpectedBucketOwner: str = ...,
) -> PutObjectOutputTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
3. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
4. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
5. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
6. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
7. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
8. See [:material-code-braces: PutObjectOutputTypeDef](./type_defs.md#putobjectoutputtypedef) 


```python
# put method usage example with argument unpacking

kwargs: PutObjectRequestObjectSummaryPutTypeDef = {  # (1)
    "ACL": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutObjectRequestObjectSummaryPutTypeDef](./type_defs.md#putobjectrequestobjectsummaryputtypedef) 

#### ObjectSummary.restore\_object method

This operation is not supported for directory buckets.

Type annotations and code completion for `#!python aiobotocore.resource("s3").restore_object` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/restore_object.html)

```python
# restore_object method definition

await def restore_object(
    self,
    *,
    VersionId: str = ...,
    RestoreRequest: RestoreRequestTypeDef = ...,  # (1)
    RequestPayer: RequestPayerType = ...,  # (2)
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (3)
    ExpectedBucketOwner: str = ...,
) -> RestoreObjectOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RestoreRequestTypeDef](./type_defs.md#restorerequesttypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
4. See [:material-code-braces: RestoreObjectOutputTypeDef](./type_defs.md#restoreobjectoutputtypedef) 


```python
# restore_object method usage example with argument unpacking

kwargs: RestoreObjectRequestObjectSummaryRestoreObjectTypeDef = {  # (1)
    "VersionId": ...,
}

parent.restore_object(**kwargs)
```

1. See [:material-code-braces: RestoreObjectRequestObjectSummaryRestoreObjectTypeDef](./type_defs.md#restoreobjectrequestobjectsummaryrestoreobjecttypedef) 

#### ObjectSummary.wait\_until\_exists method

Waits until ObjectSummary is exists.

Type annotations and code completion for `#!python aiobotocore.resource("s3").wait_until_exists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/wait_until_exists.html)

```python
# wait_until_exists method definition

await def wait_until_exists(
    self,
) -> None:
    ...
```


#### ObjectSummary.wait\_until\_not\_exists method

Waits until ObjectSummary is not_exists.

Type annotations and code completion for `#!python aiobotocore.resource("s3").wait_until_not_exists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/wait_until_not_exists.html)

```python
# wait_until_not_exists method definition

await def wait_until_not_exists(
    self,
) -> None:
    ...
```


#### ObjectSummary.Acl method

Creates a ObjectAcl resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/Acl.html)

```python
# Acl method definition

await def Acl(
    self,
) -> _ObjectAcl:
    ...
```


#### ObjectSummary.Bucket method

Creates a Bucket resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/Bucket.html)

```python
# Bucket method definition

await def Bucket(
    self,
) -> _Bucket:
    ...
```


#### ObjectSummary.MultipartUpload method

Creates a MultipartUpload resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").MultipartUpload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/MultipartUpload.html)

```python
# MultipartUpload method definition

await def MultipartUpload(
    self,
    id: str,
) -> _MultipartUpload:
    ...
```


#### ObjectSummary.Object method

Creates a Object resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Object` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/Object.html)

```python
# Object method definition

await def Object(
    self,
) -> _Object:
    ...
```


#### ObjectSummary.Version method

Creates a ObjectVersion resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/Version.html)

```python
# Version method definition

await def Version(
    self,
    id: str,
) -> _ObjectVersion:
    ...
```


#### ObjectSummary.load method

Calls s3.Client.head_object to update the attributes of the ObjectSummary
resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectsummary/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```





## ObjectVersion

Type annotations and code completion for `#!python session.resource("s3").ObjectVersion` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectversion/index.html#S3.ObjectVersion)

```python
# ObjectVersion usage example

from types_aiobotocore_s3.service_resource import ObjectVersion

def get_resource() -> ObjectVersion:
    return session.resource("s3").ObjectVersion(...)
```


### ObjectVersion attributes


- `bucket_name`: `str`
- `object_key`: `str`
- `id`: `str`
- `e_tag`: `Awaitable`[`str`]
- `checksum_algorithm`: `Awaitable`[`List`[[ChecksumAlgorithmType](./literals.md#checksumalgorithmtype)]]
- `checksum_type`: `Awaitable`[[ChecksumTypeType](./literals.md#checksumtypetype)]
- `size`: `Awaitable`[`int`]
- `storage_class`: `Awaitable`[`Literal['STANDARD']` (see [ObjectVersionStorageClassType](./literals.md#objectversionstorageclasstype))]
- `key`: `Awaitable`[`str`]
- `version_id`: `Awaitable`[`str`]
- `is_latest`: `Awaitable`[`bool`]
- `last_modified`: `Awaitable`[`datetime`]
- `owner`: `Awaitable`[[OwnerTypeDef](./type_defs.md#ownertypedef)]
- `restore_status`: `Awaitable`[[RestoreStatusTypeDef](./type_defs.md#restorestatustypedef)]
- `meta`: `S3ResourceMeta`





### ObjectVersion methods


#### ObjectVersion.get\_available\_subresources method

Returns a list of all the available sub-resources for this ObjectVersion.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectversion/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### ObjectVersion.delete method

Removes an object from a bucket.

Type annotations and code completion for `#!python aiobotocore.resource("s3").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectversion/delete.html)

```python
# delete method definition

await def delete(
    self,
    *,
    MFA: str = ...,
    RequestPayer: RequestPayerType = ...,  # (1)
    BypassGovernanceRetention: bool = ...,
    ExpectedBucketOwner: str = ...,
    IfMatch: str = ...,
    IfMatchLastModifiedTime: TimestampTypeDef = ...,
    IfMatchSize: int = ...,
) -> DeleteObjectOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-braces: DeleteObjectOutputTypeDef](./type_defs.md#deleteobjectoutputtypedef) 


```python
# delete method usage example with argument unpacking

kwargs: DeleteObjectRequestObjectVersionDeleteTypeDef = {  # (1)
    "MFA": ...,
}

parent.delete(**kwargs)
```

1. See [:material-code-braces: DeleteObjectRequestObjectVersionDeleteTypeDef](./type_defs.md#deleteobjectrequestobjectversiondeletetypedef) 

#### ObjectVersion.get method

Retrieves an object from Amazon S3.

Type annotations and code completion for `#!python aiobotocore.resource("s3").get` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectversion/get.html)

```python
# get method definition

await def get(
    self,
    *,
    IfMatch: str = ...,
    IfModifiedSince: TimestampTypeDef = ...,
    IfNoneMatch: str = ...,
    IfUnmodifiedSince: TimestampTypeDef = ...,
    Range: str = ...,
    ResponseCacheControl: str = ...,
    ResponseContentDisposition: str = ...,
    ResponseContentEncoding: str = ...,
    ResponseContentLanguage: str = ...,
    ResponseContentType: str = ...,
    ResponseExpires: TimestampTypeDef = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    RequestPayer: RequestPayerType = ...,  # (1)
    PartNumber: int = ...,
    ExpectedBucketOwner: str = ...,
    ChecksumMode: ChecksumModeType = ...,  # (2)
) -> GetObjectOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-brackets: ChecksumModeType](./literals.md#checksummodetype) 
3. See [:material-code-braces: GetObjectOutputTypeDef](./type_defs.md#getobjectoutputtypedef) 


```python
# get method usage example with argument unpacking

kwargs: GetObjectRequestObjectVersionGetTypeDef = {  # (1)
    "IfMatch": ...,
}

parent.get(**kwargs)
```

1. See [:material-code-braces: GetObjectRequestObjectVersionGetTypeDef](./type_defs.md#getobjectrequestobjectversiongettypedef) 

#### ObjectVersion.head method

The <code>HEAD</code> operation retrieves metadata from an object without
returning the object itself.

Type annotations and code completion for `#!python aiobotocore.resource("s3").head` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectversion/head.html)

```python
# head method definition

await def head(
    self,
    *,
    IfMatch: str = ...,
    IfModifiedSince: TimestampTypeDef = ...,
    IfNoneMatch: str = ...,
    IfUnmodifiedSince: TimestampTypeDef = ...,
    Range: str = ...,
    ResponseCacheControl: str = ...,
    ResponseContentDisposition: str = ...,
    ResponseContentEncoding: str = ...,
    ResponseContentLanguage: str = ...,
    ResponseContentType: str = ...,
    ResponseExpires: TimestampTypeDef = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    RequestPayer: RequestPayerType = ...,  # (1)
    PartNumber: int = ...,
    ExpectedBucketOwner: str = ...,
    ChecksumMode: ChecksumModeType = ...,  # (2)
) -> HeadObjectOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-brackets: ChecksumModeType](./literals.md#checksummodetype) 
3. See [:material-code-braces: HeadObjectOutputTypeDef](./type_defs.md#headobjectoutputtypedef) 


```python
# head method usage example with argument unpacking

kwargs: HeadObjectRequestObjectVersionHeadTypeDef = {  # (1)
    "IfMatch": ...,
}

parent.head(**kwargs)
```

1. See [:material-code-braces: HeadObjectRequestObjectVersionHeadTypeDef](./type_defs.md#headobjectrequestobjectversionheadtypedef) 

#### ObjectVersion.Object method

Creates a Object resource.

Type annotations and code completion for `#!python aiobotocore.resource("s3").Object` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/objectversion/Object.html)

```python
# Object method definition

await def Object(
    self,
) -> _Object:
    ...
```




