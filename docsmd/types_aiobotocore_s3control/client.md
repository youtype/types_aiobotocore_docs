# S3ControlClient

> [Index](../README.md) > [S3Control](./README.md) > S3ControlClient

!!! note ""

    Auto-generated documentation for [S3Control](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
    type annotations stubs module [types-aiobotocore-s3control](https://pypi.org/project/types-aiobotocore-s3control/).

## S3ControlClient

Type annotations and code completion for `#!python session.create_client("s3control")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client)

```python
# S3ControlClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_s3control.client import S3ControlClient

session = get_session()
async with session.create_client("s3control") as client:
    client: S3ControlClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("s3control").exceptions` structure.

```python
# S3ControlClient.exceptions usage example

async with session.create_client("s3control") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.BucketAlreadyExists,
        client.BucketAlreadyOwnedByYou,
        client.ClientError,
        client.IdempotencyException,
        client.InternalServiceException,
        client.InvalidNextTokenException,
        client.InvalidRequestException,
        client.JobStatusException,
        client.NoSuchPublicAccessBlockConfiguration,
        client.NotFoundException,
        client.TooManyRequestsException,
        client.TooManyTagsException,
    ) as e:
        print(e)
```

```python
# S3ControlClient usage type checking example

from types_aiobotocore_s3control.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### associate\_access\_grants\_identity\_center

Associate your S3 Access Grants instance with an Amazon Web Services IAM
Identity Center
instance.

Type annotations and code completion for `#!python session.create_client("s3control").associate_access_grants_identity_center` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.associate_access_grants_identity_center)

```python
# associate_access_grants_identity_center method definition

await def associate_access_grants_identity_center(
    self,
    *,
    AccountId: str,
    IdentityCenterArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_access_grants_identity_center method usage example with argument unpacking

kwargs: AssociateAccessGrantsIdentityCenterRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "IdentityCenterArn": ...,
}

parent.associate_access_grants_identity_center(**kwargs)
```

1. See [:material-code-braces: AssociateAccessGrantsIdentityCenterRequestRequestTypeDef](./type_defs.md#associateaccessgrantsidentitycenterrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("s3control").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("s3control").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_access\_grant

Creates an access grant that gives a grantee access to your S3 data.

Type annotations and code completion for `#!python session.create_client("s3control").create_access_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_grant)

```python
# create_access_grant method definition

await def create_access_grant(
    self,
    *,
    AccountId: str,
    AccessGrantsLocationId: str,
    Grantee: GranteeTypeDef,  # (1)
    Permission: PermissionType,  # (2)
    AccessGrantsLocationConfiguration: AccessGrantsLocationConfigurationTypeDef = ...,  # (3)
    ApplicationArn: str = ...,
    S3PrefixType: S3PrefixTypeType = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> CreateAccessGrantResultTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: GranteeTypeDef](./type_defs.md#granteetypedef) 
2. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
3. See [:material-code-braces: AccessGrantsLocationConfigurationTypeDef](./type_defs.md#accessgrantslocationconfigurationtypedef) 
4. See [:material-code-brackets: S3PrefixTypeType](./literals.md#s3prefixtypetype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CreateAccessGrantResultTypeDef](./type_defs.md#createaccessgrantresulttypedef) 


```python
# create_access_grant method usage example with argument unpacking

kwargs: CreateAccessGrantRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "AccessGrantsLocationId": ...,
    "Grantee": ...,
    "Permission": ...,
}

parent.create_access_grant(**kwargs)
```

1. See [:material-code-braces: CreateAccessGrantRequestRequestTypeDef](./type_defs.md#createaccessgrantrequestrequesttypedef) 

### create\_access\_grants\_instance

Creates an S3 Access Grants instance, which serves as a logical grouping for
access
grants.

Type annotations and code completion for `#!python session.create_client("s3control").create_access_grants_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_grants_instance)

```python
# create_access_grants_instance method definition

await def create_access_grants_instance(
    self,
    *,
    AccountId: str,
    IdentityCenterArn: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateAccessGrantsInstanceResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateAccessGrantsInstanceResultTypeDef](./type_defs.md#createaccessgrantsinstanceresulttypedef) 


```python
# create_access_grants_instance method usage example with argument unpacking

kwargs: CreateAccessGrantsInstanceRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.create_access_grants_instance(**kwargs)
```

1. See [:material-code-braces: CreateAccessGrantsInstanceRequestRequestTypeDef](./type_defs.md#createaccessgrantsinstancerequestrequesttypedef) 

### create\_access\_grants\_location

The S3 data location that you would like to register in your S3 Access Grants
instance.

Type annotations and code completion for `#!python session.create_client("s3control").create_access_grants_location` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_grants_location)

```python
# create_access_grants_location method definition

await def create_access_grants_location(
    self,
    *,
    AccountId: str,
    LocationScope: str,
    IAMRoleArn: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateAccessGrantsLocationResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateAccessGrantsLocationResultTypeDef](./type_defs.md#createaccessgrantslocationresulttypedef) 


```python
# create_access_grants_location method usage example with argument unpacking

kwargs: CreateAccessGrantsLocationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "LocationScope": ...,
    "IAMRoleArn": ...,
}

parent.create_access_grants_location(**kwargs)
```

1. See [:material-code-braces: CreateAccessGrantsLocationRequestRequestTypeDef](./type_defs.md#createaccessgrantslocationrequestrequesttypedef) 

### create\_access\_point

.

Type annotations and code completion for `#!python session.create_client("s3control").create_access_point` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point)

```python
# create_access_point method definition

await def create_access_point(
    self,
    *,
    AccountId: str,
    Name: str,
    Bucket: str,
    VpcConfiguration: VpcConfigurationTypeDef = ...,  # (1)
    PublicAccessBlockConfiguration: PublicAccessBlockConfigurationTypeDef = ...,  # (2)
    BucketAccountId: str = ...,
) -> CreateAccessPointResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
2. See [:material-code-braces: PublicAccessBlockConfigurationTypeDef](./type_defs.md#publicaccessblockconfigurationtypedef) 
3. See [:material-code-braces: CreateAccessPointResultTypeDef](./type_defs.md#createaccesspointresulttypedef) 


```python
# create_access_point method usage example with argument unpacking

kwargs: CreateAccessPointRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
    "Bucket": ...,
}

parent.create_access_point(**kwargs)
```

1. See [:material-code-braces: CreateAccessPointRequestRequestTypeDef](./type_defs.md#createaccesspointrequestrequesttypedef) 

### create\_access\_point\_for\_object\_lambda

.

Type annotations and code completion for `#!python session.create_client("s3control").create_access_point_for_object_lambda` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point_for_object_lambda)

```python
# create_access_point_for_object_lambda method definition

await def create_access_point_for_object_lambda(
    self,
    *,
    AccountId: str,
    Name: str,
    Configuration: ObjectLambdaConfigurationTypeDef,  # (1)
) -> CreateAccessPointForObjectLambdaResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ObjectLambdaConfigurationTypeDef](./type_defs.md#objectlambdaconfigurationtypedef) 
2. See [:material-code-braces: CreateAccessPointForObjectLambdaResultTypeDef](./type_defs.md#createaccesspointforobjectlambdaresulttypedef) 


```python
# create_access_point_for_object_lambda method usage example with argument unpacking

kwargs: CreateAccessPointForObjectLambdaRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
    "Configuration": ...,
}

parent.create_access_point_for_object_lambda(**kwargs)
```

1. See [:material-code-braces: CreateAccessPointForObjectLambdaRequestRequestTypeDef](./type_defs.md#createaccesspointforobjectlambdarequestrequesttypedef) 

### create\_bucket

.

Type annotations and code completion for `#!python session.create_client("s3control").create_bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_bucket)

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
    OutpostId: str = ...,
) -> CreateBucketResultTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: BucketCannedACLType](./literals.md#bucketcannedacltype) 
2. See [:material-code-braces: CreateBucketConfigurationTypeDef](./type_defs.md#createbucketconfigurationtypedef) 
3. See [:material-code-braces: CreateBucketResultTypeDef](./type_defs.md#createbucketresulttypedef) 


```python
# create_bucket method usage example with argument unpacking

kwargs: CreateBucketRequestRequestTypeDef = {  # (1)
    "Bucket": ...,
}

parent.create_bucket(**kwargs)
```

1. See [:material-code-braces: CreateBucketRequestRequestTypeDef](./type_defs.md#createbucketrequestrequesttypedef) 

### create\_job

This operation creates an S3 Batch Operations job.

Type annotations and code completion for `#!python session.create_client("s3control").create_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_job)

```python
# create_job method definition

await def create_job(
    self,
    *,
    AccountId: str,
    Operation: JobOperationTypeDef,  # (1)
    Report: JobReportTypeDef,  # (2)
    ClientRequestToken: str,
    Priority: int,
    RoleArn: str,
    ConfirmationRequired: bool = ...,
    Manifest: JobManifestTypeDef = ...,  # (3)
    Description: str = ...,
    Tags: Sequence[S3TagTypeDef] = ...,  # (4)
    ManifestGenerator: JobManifestGeneratorTypeDef = ...,  # (5)
) -> CreateJobResultTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: JobOperationTypeDef](./type_defs.md#joboperationtypedef) 
2. See [:material-code-braces: JobReportTypeDef](./type_defs.md#jobreporttypedef) 
3. See [:material-code-braces: JobManifestTypeDef](./type_defs.md#jobmanifesttypedef) 
4. See [:material-code-braces: S3TagTypeDef](./type_defs.md#s3tagtypedef) 
5. See [:material-code-braces: JobManifestGeneratorTypeDef](./type_defs.md#jobmanifestgeneratortypedef) 
6. See [:material-code-braces: CreateJobResultTypeDef](./type_defs.md#createjobresulttypedef) 


```python
# create_job method usage example with argument unpacking

kwargs: CreateJobRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Operation": ...,
    "Report": ...,
    "ClientRequestToken": ...,
    "Priority": ...,
    "RoleArn": ...,
}

parent.create_job(**kwargs)
```

1. See [:material-code-braces: CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef) 

### create\_multi\_region\_access\_point

.

Type annotations and code completion for `#!python session.create_client("s3control").create_multi_region_access_point` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_multi_region_access_point)

```python
# create_multi_region_access_point method definition

await def create_multi_region_access_point(
    self,
    *,
    AccountId: str,
    ClientToken: str,
    Details: CreateMultiRegionAccessPointInputTypeDef,  # (1)
) -> CreateMultiRegionAccessPointResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CreateMultiRegionAccessPointInputTypeDef](./type_defs.md#createmultiregionaccesspointinputtypedef) 
2. See [:material-code-braces: CreateMultiRegionAccessPointResultTypeDef](./type_defs.md#createmultiregionaccesspointresulttypedef) 


```python
# create_multi_region_access_point method usage example with argument unpacking

kwargs: CreateMultiRegionAccessPointRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "ClientToken": ...,
    "Details": ...,
}

parent.create_multi_region_access_point(**kwargs)
```

1. See [:material-code-braces: CreateMultiRegionAccessPointRequestRequestTypeDef](./type_defs.md#createmultiregionaccesspointrequestrequesttypedef) 

### create\_storage\_lens\_group

Creates a new S3 Storage Lens group and associates it with the specified Amazon
Web Services account
ID.

Type annotations and code completion for `#!python session.create_client("s3control").create_storage_lens_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_storage_lens_group)

```python
# create_storage_lens_group method definition

await def create_storage_lens_group(
    self,
    *,
    AccountId: str,
    StorageLensGroup: StorageLensGroupTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: StorageLensGroupTypeDef](./type_defs.md#storagelensgrouptypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_storage_lens_group method usage example with argument unpacking

kwargs: CreateStorageLensGroupRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "StorageLensGroup": ...,
}

parent.create_storage_lens_group(**kwargs)
```

1. See [:material-code-braces: CreateStorageLensGroupRequestRequestTypeDef](./type_defs.md#createstoragelensgrouprequestrequesttypedef) 

### delete\_access\_grant

Deletes the access grant from the S3 Access Grants instance.

Type annotations and code completion for `#!python session.create_client("s3control").delete_access_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_grant)

```python
# delete_access_grant method definition

await def delete_access_grant(
    self,
    *,
    AccountId: str,
    AccessGrantId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_access_grant method usage example with argument unpacking

kwargs: DeleteAccessGrantRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "AccessGrantId": ...,
}

parent.delete_access_grant(**kwargs)
```

1. See [:material-code-braces: DeleteAccessGrantRequestRequestTypeDef](./type_defs.md#deleteaccessgrantrequestrequesttypedef) 

### delete\_access\_grants\_instance

Deletes your S3 Access Grants instance.

Type annotations and code completion for `#!python session.create_client("s3control").delete_access_grants_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_grants_instance)

```python
# delete_access_grants_instance method definition

await def delete_access_grants_instance(
    self,
    *,
    AccountId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_access_grants_instance method usage example with argument unpacking

kwargs: DeleteAccessGrantsInstanceRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.delete_access_grants_instance(**kwargs)
```

1. See [:material-code-braces: DeleteAccessGrantsInstanceRequestRequestTypeDef](./type_defs.md#deleteaccessgrantsinstancerequestrequesttypedef) 

### delete\_access\_grants\_instance\_resource\_policy

Deletes the resource policy of the S3 Access Grants instance.

Type annotations and code completion for `#!python session.create_client("s3control").delete_access_grants_instance_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_grants_instance_resource_policy)

```python
# delete_access_grants_instance_resource_policy method definition

await def delete_access_grants_instance_resource_policy(
    self,
    *,
    AccountId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_access_grants_instance_resource_policy method usage example with argument unpacking

kwargs: DeleteAccessGrantsInstanceResourcePolicyRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.delete_access_grants_instance_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteAccessGrantsInstanceResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteaccessgrantsinstanceresourcepolicyrequestrequesttypedef) 

### delete\_access\_grants\_location

Deregisters a location from your S3 Access Grants instance.

Type annotations and code completion for `#!python session.create_client("s3control").delete_access_grants_location` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_grants_location)

```python
# delete_access_grants_location method definition

await def delete_access_grants_location(
    self,
    *,
    AccountId: str,
    AccessGrantsLocationId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_access_grants_location method usage example with argument unpacking

kwargs: DeleteAccessGrantsLocationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "AccessGrantsLocationId": ...,
}

parent.delete_access_grants_location(**kwargs)
```

1. See [:material-code-braces: DeleteAccessGrantsLocationRequestRequestTypeDef](./type_defs.md#deleteaccessgrantslocationrequestrequesttypedef) 

### delete\_access\_point

.

Type annotations and code completion for `#!python session.create_client("s3control").delete_access_point` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_point)

```python
# delete_access_point method definition

await def delete_access_point(
    self,
    *,
    AccountId: str,
    Name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_access_point method usage example with argument unpacking

kwargs: DeleteAccessPointRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.delete_access_point(**kwargs)
```

1. See [:material-code-braces: DeleteAccessPointRequestRequestTypeDef](./type_defs.md#deleteaccesspointrequestrequesttypedef) 

### delete\_access\_point\_for\_object\_lambda

.

Type annotations and code completion for `#!python session.create_client("s3control").delete_access_point_for_object_lambda` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_point_for_object_lambda)

```python
# delete_access_point_for_object_lambda method definition

await def delete_access_point_for_object_lambda(
    self,
    *,
    AccountId: str,
    Name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_access_point_for_object_lambda method usage example with argument unpacking

kwargs: DeleteAccessPointForObjectLambdaRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.delete_access_point_for_object_lambda(**kwargs)
```

1. See [:material-code-braces: DeleteAccessPointForObjectLambdaRequestRequestTypeDef](./type_defs.md#deleteaccesspointforobjectlambdarequestrequesttypedef) 

### delete\_access\_point\_policy

.

Type annotations and code completion for `#!python session.create_client("s3control").delete_access_point_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_point_policy)

```python
# delete_access_point_policy method definition

await def delete_access_point_policy(
    self,
    *,
    AccountId: str,
    Name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_access_point_policy method usage example with argument unpacking

kwargs: DeleteAccessPointPolicyRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.delete_access_point_policy(**kwargs)
```

1. See [:material-code-braces: DeleteAccessPointPolicyRequestRequestTypeDef](./type_defs.md#deleteaccesspointpolicyrequestrequesttypedef) 

### delete\_access\_point\_policy\_for\_object\_lambda

.

Type annotations and code completion for `#!python session.create_client("s3control").delete_access_point_policy_for_object_lambda` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_point_policy_for_object_lambda)

```python
# delete_access_point_policy_for_object_lambda method definition

await def delete_access_point_policy_for_object_lambda(
    self,
    *,
    AccountId: str,
    Name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_access_point_policy_for_object_lambda method usage example with argument unpacking

kwargs: DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.delete_access_point_policy_for_object_lambda(**kwargs)
```

1. See [:material-code-braces: DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef](./type_defs.md#deleteaccesspointpolicyforobjectlambdarequestrequesttypedef) 

### delete\_bucket

.

Type annotations and code completion for `#!python session.create_client("s3control").delete_bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket)

```python
# delete_bucket method definition

await def delete_bucket(
    self,
    *,
    AccountId: str,
    Bucket: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_bucket method usage example with argument unpacking

kwargs: DeleteBucketRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
}

parent.delete_bucket(**kwargs)
```

1. See [:material-code-braces: DeleteBucketRequestRequestTypeDef](./type_defs.md#deletebucketrequestrequesttypedef) 

### delete\_bucket\_lifecycle\_configuration

.

Type annotations and code completion for `#!python session.create_client("s3control").delete_bucket_lifecycle_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket_lifecycle_configuration)

```python
# delete_bucket_lifecycle_configuration method definition

await def delete_bucket_lifecycle_configuration(
    self,
    *,
    AccountId: str,
    Bucket: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_bucket_lifecycle_configuration method usage example with argument unpacking

kwargs: DeleteBucketLifecycleConfigurationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
}

parent.delete_bucket_lifecycle_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteBucketLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#deletebucketlifecycleconfigurationrequestrequesttypedef) 

### delete\_bucket\_policy

.

Type annotations and code completion for `#!python session.create_client("s3control").delete_bucket_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket_policy)

```python
# delete_bucket_policy method definition

await def delete_bucket_policy(
    self,
    *,
    AccountId: str,
    Bucket: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_bucket_policy method usage example with argument unpacking

kwargs: DeleteBucketPolicyRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
}

parent.delete_bucket_policy(**kwargs)
```

1. See [:material-code-braces: DeleteBucketPolicyRequestRequestTypeDef](./type_defs.md#deletebucketpolicyrequestrequesttypedef) 

### delete\_bucket\_replication

.

Type annotations and code completion for `#!python session.create_client("s3control").delete_bucket_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket_replication)

```python
# delete_bucket_replication method definition

await def delete_bucket_replication(
    self,
    *,
    AccountId: str,
    Bucket: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_bucket_replication method usage example with argument unpacking

kwargs: DeleteBucketReplicationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
}

parent.delete_bucket_replication(**kwargs)
```

1. See [:material-code-braces: DeleteBucketReplicationRequestRequestTypeDef](./type_defs.md#deletebucketreplicationrequestrequesttypedef) 

### delete\_bucket\_tagging

.

Type annotations and code completion for `#!python session.create_client("s3control").delete_bucket_tagging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket_tagging)

```python
# delete_bucket_tagging method definition

await def delete_bucket_tagging(
    self,
    *,
    AccountId: str,
    Bucket: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_bucket_tagging method usage example with argument unpacking

kwargs: DeleteBucketTaggingRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
}

parent.delete_bucket_tagging(**kwargs)
```

1. See [:material-code-braces: DeleteBucketTaggingRequestRequestTypeDef](./type_defs.md#deletebuckettaggingrequestrequesttypedef) 

### delete\_job\_tagging

Removes the entire tag set from the specified S3 Batch Operations job.

Type annotations and code completion for `#!python session.create_client("s3control").delete_job_tagging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_job_tagging)

```python
# delete_job_tagging method definition

await def delete_job_tagging(
    self,
    *,
    AccountId: str,
    JobId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_job_tagging method usage example with argument unpacking

kwargs: DeleteJobTaggingRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "JobId": ...,
}

parent.delete_job_tagging(**kwargs)
```

1. See [:material-code-braces: DeleteJobTaggingRequestRequestTypeDef](./type_defs.md#deletejobtaggingrequestrequesttypedef) 

### delete\_multi\_region\_access\_point

.

Type annotations and code completion for `#!python session.create_client("s3control").delete_multi_region_access_point` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_multi_region_access_point)

```python
# delete_multi_region_access_point method definition

await def delete_multi_region_access_point(
    self,
    *,
    AccountId: str,
    ClientToken: str,
    Details: DeleteMultiRegionAccessPointInputTypeDef,  # (1)
) -> DeleteMultiRegionAccessPointResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeleteMultiRegionAccessPointInputTypeDef](./type_defs.md#deletemultiregionaccesspointinputtypedef) 
2. See [:material-code-braces: DeleteMultiRegionAccessPointResultTypeDef](./type_defs.md#deletemultiregionaccesspointresulttypedef) 


```python
# delete_multi_region_access_point method usage example with argument unpacking

kwargs: DeleteMultiRegionAccessPointRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "ClientToken": ...,
    "Details": ...,
}

parent.delete_multi_region_access_point(**kwargs)
```

1. See [:material-code-braces: DeleteMultiRegionAccessPointRequestRequestTypeDef](./type_defs.md#deletemultiregionaccesspointrequestrequesttypedef) 

### delete\_public\_access\_block

.

Type annotations and code completion for `#!python session.create_client("s3control").delete_public_access_block` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_public_access_block)

```python
# delete_public_access_block method definition

await def delete_public_access_block(
    self,
    *,
    AccountId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_public_access_block method usage example with argument unpacking

kwargs: DeletePublicAccessBlockRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.delete_public_access_block(**kwargs)
```

1. See [:material-code-braces: DeletePublicAccessBlockRequestRequestTypeDef](./type_defs.md#deletepublicaccessblockrequestrequesttypedef) 

### delete\_storage\_lens\_configuration

.

Type annotations and code completion for `#!python session.create_client("s3control").delete_storage_lens_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_storage_lens_configuration)

```python
# delete_storage_lens_configuration method definition

await def delete_storage_lens_configuration(
    self,
    *,
    ConfigId: str,
    AccountId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_storage_lens_configuration method usage example with argument unpacking

kwargs: DeleteStorageLensConfigurationRequestRequestTypeDef = {  # (1)
    "ConfigId": ...,
    "AccountId": ...,
}

parent.delete_storage_lens_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteStorageLensConfigurationRequestRequestTypeDef](./type_defs.md#deletestoragelensconfigurationrequestrequesttypedef) 

### delete\_storage\_lens\_configuration\_tagging

.

Type annotations and code completion for `#!python session.create_client("s3control").delete_storage_lens_configuration_tagging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_storage_lens_configuration_tagging)

```python
# delete_storage_lens_configuration_tagging method definition

await def delete_storage_lens_configuration_tagging(
    self,
    *,
    ConfigId: str,
    AccountId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_storage_lens_configuration_tagging method usage example with argument unpacking

kwargs: DeleteStorageLensConfigurationTaggingRequestRequestTypeDef = {  # (1)
    "ConfigId": ...,
    "AccountId": ...,
}

parent.delete_storage_lens_configuration_tagging(**kwargs)
```

1. See [:material-code-braces: DeleteStorageLensConfigurationTaggingRequestRequestTypeDef](./type_defs.md#deletestoragelensconfigurationtaggingrequestrequesttypedef) 

### delete\_storage\_lens\_group

Deletes an existing S3 Storage Lens group.

Type annotations and code completion for `#!python session.create_client("s3control").delete_storage_lens_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_storage_lens_group)

```python
# delete_storage_lens_group method definition

await def delete_storage_lens_group(
    self,
    *,
    Name: str,
    AccountId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_storage_lens_group method usage example with argument unpacking

kwargs: DeleteStorageLensGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "AccountId": ...,
}

parent.delete_storage_lens_group(**kwargs)
```

1. See [:material-code-braces: DeleteStorageLensGroupRequestRequestTypeDef](./type_defs.md#deletestoragelensgrouprequestrequesttypedef) 

### describe\_job

Retrieves the configuration parameters and status for a Batch Operations job.

Type annotations and code completion for `#!python session.create_client("s3control").describe_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.describe_job)

```python
# describe_job method definition

await def describe_job(
    self,
    *,
    AccountId: str,
    JobId: str,
) -> DescribeJobResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeJobResultTypeDef](./type_defs.md#describejobresulttypedef) 


```python
# describe_job method usage example with argument unpacking

kwargs: DescribeJobRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "JobId": ...,
}

parent.describe_job(**kwargs)
```

1. See [:material-code-braces: DescribeJobRequestRequestTypeDef](./type_defs.md#describejobrequestrequesttypedef) 

### describe\_multi\_region\_access\_point\_operation

.

Type annotations and code completion for `#!python session.create_client("s3control").describe_multi_region_access_point_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.describe_multi_region_access_point_operation)

```python
# describe_multi_region_access_point_operation method definition

await def describe_multi_region_access_point_operation(
    self,
    *,
    AccountId: str,
    RequestTokenARN: str,
) -> DescribeMultiRegionAccessPointOperationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMultiRegionAccessPointOperationResultTypeDef](./type_defs.md#describemultiregionaccesspointoperationresulttypedef) 


```python
# describe_multi_region_access_point_operation method usage example with argument unpacking

kwargs: DescribeMultiRegionAccessPointOperationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "RequestTokenARN": ...,
}

parent.describe_multi_region_access_point_operation(**kwargs)
```

1. See [:material-code-braces: DescribeMultiRegionAccessPointOperationRequestRequestTypeDef](./type_defs.md#describemultiregionaccesspointoperationrequestrequesttypedef) 

### dissociate\_access\_grants\_identity\_center

Dissociates the Amazon Web Services IAM Identity Center instance from the S3
Access Grants
instance.

Type annotations and code completion for `#!python session.create_client("s3control").dissociate_access_grants_identity_center` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.dissociate_access_grants_identity_center)

```python
# dissociate_access_grants_identity_center method definition

await def dissociate_access_grants_identity_center(
    self,
    *,
    AccountId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# dissociate_access_grants_identity_center method usage example with argument unpacking

kwargs: DissociateAccessGrantsIdentityCenterRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.dissociate_access_grants_identity_center(**kwargs)
```

1. See [:material-code-braces: DissociateAccessGrantsIdentityCenterRequestRequestTypeDef](./type_defs.md#dissociateaccessgrantsidentitycenterrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("s3control").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.generate_presigned_url)

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


### get\_access\_grant

Get the details of an access grant from your S3 Access Grants instance.

Type annotations and code completion for `#!python session.create_client("s3control").get_access_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_grant)

```python
# get_access_grant method definition

await def get_access_grant(
    self,
    *,
    AccountId: str,
    AccessGrantId: str,
) -> GetAccessGrantResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessGrantResultTypeDef](./type_defs.md#getaccessgrantresulttypedef) 


```python
# get_access_grant method usage example with argument unpacking

kwargs: GetAccessGrantRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "AccessGrantId": ...,
}

parent.get_access_grant(**kwargs)
```

1. See [:material-code-braces: GetAccessGrantRequestRequestTypeDef](./type_defs.md#getaccessgrantrequestrequesttypedef) 

### get\_access\_grants\_instance

Retrieves the S3 Access Grants instance for a Region in your account.

Type annotations and code completion for `#!python session.create_client("s3control").get_access_grants_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_grants_instance)

```python
# get_access_grants_instance method definition

await def get_access_grants_instance(
    self,
    *,
    AccountId: str,
) -> GetAccessGrantsInstanceResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessGrantsInstanceResultTypeDef](./type_defs.md#getaccessgrantsinstanceresulttypedef) 


```python
# get_access_grants_instance method usage example with argument unpacking

kwargs: GetAccessGrantsInstanceRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.get_access_grants_instance(**kwargs)
```

1. See [:material-code-braces: GetAccessGrantsInstanceRequestRequestTypeDef](./type_defs.md#getaccessgrantsinstancerequestrequesttypedef) 

### get\_access\_grants\_instance\_for\_prefix

Retrieve the S3 Access Grants instance that contains a particular prefix.

Type annotations and code completion for `#!python session.create_client("s3control").get_access_grants_instance_for_prefix` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_grants_instance_for_prefix)

```python
# get_access_grants_instance_for_prefix method definition

await def get_access_grants_instance_for_prefix(
    self,
    *,
    AccountId: str,
    S3Prefix: str,
) -> GetAccessGrantsInstanceForPrefixResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessGrantsInstanceForPrefixResultTypeDef](./type_defs.md#getaccessgrantsinstanceforprefixresulttypedef) 


```python
# get_access_grants_instance_for_prefix method usage example with argument unpacking

kwargs: GetAccessGrantsInstanceForPrefixRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "S3Prefix": ...,
}

parent.get_access_grants_instance_for_prefix(**kwargs)
```

1. See [:material-code-braces: GetAccessGrantsInstanceForPrefixRequestRequestTypeDef](./type_defs.md#getaccessgrantsinstanceforprefixrequestrequesttypedef) 

### get\_access\_grants\_instance\_resource\_policy

Returns the resource policy of the S3 Access Grants instance.

Type annotations and code completion for `#!python session.create_client("s3control").get_access_grants_instance_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_grants_instance_resource_policy)

```python
# get_access_grants_instance_resource_policy method definition

await def get_access_grants_instance_resource_policy(
    self,
    *,
    AccountId: str,
) -> GetAccessGrantsInstanceResourcePolicyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessGrantsInstanceResourcePolicyResultTypeDef](./type_defs.md#getaccessgrantsinstanceresourcepolicyresulttypedef) 


```python
# get_access_grants_instance_resource_policy method usage example with argument unpacking

kwargs: GetAccessGrantsInstanceResourcePolicyRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.get_access_grants_instance_resource_policy(**kwargs)
```

1. See [:material-code-braces: GetAccessGrantsInstanceResourcePolicyRequestRequestTypeDef](./type_defs.md#getaccessgrantsinstanceresourcepolicyrequestrequesttypedef) 

### get\_access\_grants\_location

Retrieves the details of a particular location registered in your S3 Access
Grants
instance.

Type annotations and code completion for `#!python session.create_client("s3control").get_access_grants_location` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_grants_location)

```python
# get_access_grants_location method definition

await def get_access_grants_location(
    self,
    *,
    AccountId: str,
    AccessGrantsLocationId: str,
) -> GetAccessGrantsLocationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessGrantsLocationResultTypeDef](./type_defs.md#getaccessgrantslocationresulttypedef) 


```python
# get_access_grants_location method usage example with argument unpacking

kwargs: GetAccessGrantsLocationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "AccessGrantsLocationId": ...,
}

parent.get_access_grants_location(**kwargs)
```

1. See [:material-code-braces: GetAccessGrantsLocationRequestRequestTypeDef](./type_defs.md#getaccessgrantslocationrequestrequesttypedef) 

### get\_access\_point

.

Type annotations and code completion for `#!python session.create_client("s3control").get_access_point` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point)

```python
# get_access_point method definition

await def get_access_point(
    self,
    *,
    AccountId: str,
    Name: str,
) -> GetAccessPointResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessPointResultTypeDef](./type_defs.md#getaccesspointresulttypedef) 


```python
# get_access_point method usage example with argument unpacking

kwargs: GetAccessPointRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.get_access_point(**kwargs)
```

1. See [:material-code-braces: GetAccessPointRequestRequestTypeDef](./type_defs.md#getaccesspointrequestrequesttypedef) 

### get\_access\_point\_configuration\_for\_object\_lambda

.

Type annotations and code completion for `#!python session.create_client("s3control").get_access_point_configuration_for_object_lambda` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_configuration_for_object_lambda)

```python
# get_access_point_configuration_for_object_lambda method definition

await def get_access_point_configuration_for_object_lambda(
    self,
    *,
    AccountId: str,
    Name: str,
) -> GetAccessPointConfigurationForObjectLambdaResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessPointConfigurationForObjectLambdaResultTypeDef](./type_defs.md#getaccesspointconfigurationforobjectlambdaresulttypedef) 


```python
# get_access_point_configuration_for_object_lambda method usage example with argument unpacking

kwargs: GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.get_access_point_configuration_for_object_lambda(**kwargs)
```

1. See [:material-code-braces: GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef](./type_defs.md#getaccesspointconfigurationforobjectlambdarequestrequesttypedef) 

### get\_access\_point\_for\_object\_lambda

.

Type annotations and code completion for `#!python session.create_client("s3control").get_access_point_for_object_lambda` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_for_object_lambda)

```python
# get_access_point_for_object_lambda method definition

await def get_access_point_for_object_lambda(
    self,
    *,
    AccountId: str,
    Name: str,
) -> GetAccessPointForObjectLambdaResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessPointForObjectLambdaResultTypeDef](./type_defs.md#getaccesspointforobjectlambdaresulttypedef) 


```python
# get_access_point_for_object_lambda method usage example with argument unpacking

kwargs: GetAccessPointForObjectLambdaRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.get_access_point_for_object_lambda(**kwargs)
```

1. See [:material-code-braces: GetAccessPointForObjectLambdaRequestRequestTypeDef](./type_defs.md#getaccesspointforobjectlambdarequestrequesttypedef) 

### get\_access\_point\_policy

.

Type annotations and code completion for `#!python session.create_client("s3control").get_access_point_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy)

```python
# get_access_point_policy method definition

await def get_access_point_policy(
    self,
    *,
    AccountId: str,
    Name: str,
) -> GetAccessPointPolicyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessPointPolicyResultTypeDef](./type_defs.md#getaccesspointpolicyresulttypedef) 


```python
# get_access_point_policy method usage example with argument unpacking

kwargs: GetAccessPointPolicyRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.get_access_point_policy(**kwargs)
```

1. See [:material-code-braces: GetAccessPointPolicyRequestRequestTypeDef](./type_defs.md#getaccesspointpolicyrequestrequesttypedef) 

### get\_access\_point\_policy\_for\_object\_lambda

.

Type annotations and code completion for `#!python session.create_client("s3control").get_access_point_policy_for_object_lambda` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy_for_object_lambda)

```python
# get_access_point_policy_for_object_lambda method definition

await def get_access_point_policy_for_object_lambda(
    self,
    *,
    AccountId: str,
    Name: str,
) -> GetAccessPointPolicyForObjectLambdaResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessPointPolicyForObjectLambdaResultTypeDef](./type_defs.md#getaccesspointpolicyforobjectlambdaresulttypedef) 


```python
# get_access_point_policy_for_object_lambda method usage example with argument unpacking

kwargs: GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.get_access_point_policy_for_object_lambda(**kwargs)
```

1. See [:material-code-braces: GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef](./type_defs.md#getaccesspointpolicyforobjectlambdarequestrequesttypedef) 

### get\_access\_point\_policy\_status

.

Type annotations and code completion for `#!python session.create_client("s3control").get_access_point_policy_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy_status)

```python
# get_access_point_policy_status method definition

await def get_access_point_policy_status(
    self,
    *,
    AccountId: str,
    Name: str,
) -> GetAccessPointPolicyStatusResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessPointPolicyStatusResultTypeDef](./type_defs.md#getaccesspointpolicystatusresulttypedef) 


```python
# get_access_point_policy_status method usage example with argument unpacking

kwargs: GetAccessPointPolicyStatusRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.get_access_point_policy_status(**kwargs)
```

1. See [:material-code-braces: GetAccessPointPolicyStatusRequestRequestTypeDef](./type_defs.md#getaccesspointpolicystatusrequestrequesttypedef) 

### get\_access\_point\_policy\_status\_for\_object\_lambda

.

Type annotations and code completion for `#!python session.create_client("s3control").get_access_point_policy_status_for_object_lambda` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy_status_for_object_lambda)

```python
# get_access_point_policy_status_for_object_lambda method definition

await def get_access_point_policy_status_for_object_lambda(
    self,
    *,
    AccountId: str,
    Name: str,
) -> GetAccessPointPolicyStatusForObjectLambdaResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessPointPolicyStatusForObjectLambdaResultTypeDef](./type_defs.md#getaccesspointpolicystatusforobjectlambdaresulttypedef) 


```python
# get_access_point_policy_status_for_object_lambda method usage example with argument unpacking

kwargs: GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.get_access_point_policy_status_for_object_lambda(**kwargs)
```

1. See [:material-code-braces: GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef](./type_defs.md#getaccesspointpolicystatusforobjectlambdarequestrequesttypedef) 

### get\_bucket

Gets an Amazon S3 on Outposts bucket.

Type annotations and code completion for `#!python session.create_client("s3control").get_bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket)

```python
# get_bucket method definition

await def get_bucket(
    self,
    *,
    AccountId: str,
    Bucket: str,
) -> GetBucketResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBucketResultTypeDef](./type_defs.md#getbucketresulttypedef) 


```python
# get_bucket method usage example with argument unpacking

kwargs: GetBucketRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
}

parent.get_bucket(**kwargs)
```

1. See [:material-code-braces: GetBucketRequestRequestTypeDef](./type_defs.md#getbucketrequestrequesttypedef) 

### get\_bucket\_lifecycle\_configuration

.

Type annotations and code completion for `#!python session.create_client("s3control").get_bucket_lifecycle_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_lifecycle_configuration)

```python
# get_bucket_lifecycle_configuration method definition

await def get_bucket_lifecycle_configuration(
    self,
    *,
    AccountId: str,
    Bucket: str,
) -> GetBucketLifecycleConfigurationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBucketLifecycleConfigurationResultTypeDef](./type_defs.md#getbucketlifecycleconfigurationresulttypedef) 


```python
# get_bucket_lifecycle_configuration method usage example with argument unpacking

kwargs: GetBucketLifecycleConfigurationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
}

parent.get_bucket_lifecycle_configuration(**kwargs)
```

1. See [:material-code-braces: GetBucketLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#getbucketlifecycleconfigurationrequestrequesttypedef) 

### get\_bucket\_policy

.

Type annotations and code completion for `#!python session.create_client("s3control").get_bucket_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_policy)

```python
# get_bucket_policy method definition

await def get_bucket_policy(
    self,
    *,
    AccountId: str,
    Bucket: str,
) -> GetBucketPolicyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBucketPolicyResultTypeDef](./type_defs.md#getbucketpolicyresulttypedef) 


```python
# get_bucket_policy method usage example with argument unpacking

kwargs: GetBucketPolicyRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
}

parent.get_bucket_policy(**kwargs)
```

1. See [:material-code-braces: GetBucketPolicyRequestRequestTypeDef](./type_defs.md#getbucketpolicyrequestrequesttypedef) 

### get\_bucket\_replication

.

Type annotations and code completion for `#!python session.create_client("s3control").get_bucket_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_replication)

```python
# get_bucket_replication method definition

await def get_bucket_replication(
    self,
    *,
    AccountId: str,
    Bucket: str,
) -> GetBucketReplicationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBucketReplicationResultTypeDef](./type_defs.md#getbucketreplicationresulttypedef) 


```python
# get_bucket_replication method usage example with argument unpacking

kwargs: GetBucketReplicationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
}

parent.get_bucket_replication(**kwargs)
```

1. See [:material-code-braces: GetBucketReplicationRequestRequestTypeDef](./type_defs.md#getbucketreplicationrequestrequesttypedef) 

### get\_bucket\_tagging

.

Type annotations and code completion for `#!python session.create_client("s3control").get_bucket_tagging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_tagging)

```python
# get_bucket_tagging method definition

await def get_bucket_tagging(
    self,
    *,
    AccountId: str,
    Bucket: str,
) -> GetBucketTaggingResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBucketTaggingResultTypeDef](./type_defs.md#getbuckettaggingresulttypedef) 


```python
# get_bucket_tagging method usage example with argument unpacking

kwargs: GetBucketTaggingRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
}

parent.get_bucket_tagging(**kwargs)
```

1. See [:material-code-braces: GetBucketTaggingRequestRequestTypeDef](./type_defs.md#getbuckettaggingrequestrequesttypedef) 

### get\_bucket\_versioning

.

Type annotations and code completion for `#!python session.create_client("s3control").get_bucket_versioning` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_versioning)

```python
# get_bucket_versioning method definition

await def get_bucket_versioning(
    self,
    *,
    AccountId: str,
    Bucket: str,
) -> GetBucketVersioningResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBucketVersioningResultTypeDef](./type_defs.md#getbucketversioningresulttypedef) 


```python
# get_bucket_versioning method usage example with argument unpacking

kwargs: GetBucketVersioningRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
}

parent.get_bucket_versioning(**kwargs)
```

1. See [:material-code-braces: GetBucketVersioningRequestRequestTypeDef](./type_defs.md#getbucketversioningrequestrequesttypedef) 

### get\_data\_access

Returns a temporary access credential from S3 Access Grants to the grantee or
client
application.

Type annotations and code completion for `#!python session.create_client("s3control").get_data_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_data_access)

```python
# get_data_access method definition

await def get_data_access(
    self,
    *,
    AccountId: str,
    Target: str,
    Permission: PermissionType,  # (1)
    DurationSeconds: int = ...,
    Privilege: PrivilegeType = ...,  # (2)
    TargetType: S3PrefixTypeType = ...,  # (3)
) -> GetDataAccessResultTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
2. See [:material-code-brackets: PrivilegeType](./literals.md#privilegetype) 
3. See [:material-code-brackets: S3PrefixTypeType](./literals.md#s3prefixtypetype) 
4. See [:material-code-braces: GetDataAccessResultTypeDef](./type_defs.md#getdataaccessresulttypedef) 


```python
# get_data_access method usage example with argument unpacking

kwargs: GetDataAccessRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Target": ...,
    "Permission": ...,
}

parent.get_data_access(**kwargs)
```

1. See [:material-code-braces: GetDataAccessRequestRequestTypeDef](./type_defs.md#getdataaccessrequestrequesttypedef) 

### get\_job\_tagging

Returns the tags on an S3 Batch Operations job.

Type annotations and code completion for `#!python session.create_client("s3control").get_job_tagging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_job_tagging)

```python
# get_job_tagging method definition

await def get_job_tagging(
    self,
    *,
    AccountId: str,
    JobId: str,
) -> GetJobTaggingResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobTaggingResultTypeDef](./type_defs.md#getjobtaggingresulttypedef) 


```python
# get_job_tagging method usage example with argument unpacking

kwargs: GetJobTaggingRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "JobId": ...,
}

parent.get_job_tagging(**kwargs)
```

1. See [:material-code-braces: GetJobTaggingRequestRequestTypeDef](./type_defs.md#getjobtaggingrequestrequesttypedef) 

### get\_multi\_region\_access\_point

.

Type annotations and code completion for `#!python session.create_client("s3control").get_multi_region_access_point` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_multi_region_access_point)

```python
# get_multi_region_access_point method definition

await def get_multi_region_access_point(
    self,
    *,
    AccountId: str,
    Name: str,
) -> GetMultiRegionAccessPointResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMultiRegionAccessPointResultTypeDef](./type_defs.md#getmultiregionaccesspointresulttypedef) 


```python
# get_multi_region_access_point method usage example with argument unpacking

kwargs: GetMultiRegionAccessPointRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.get_multi_region_access_point(**kwargs)
```

1. See [:material-code-braces: GetMultiRegionAccessPointRequestRequestTypeDef](./type_defs.md#getmultiregionaccesspointrequestrequesttypedef) 

### get\_multi\_region\_access\_point\_policy

.

Type annotations and code completion for `#!python session.create_client("s3control").get_multi_region_access_point_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_multi_region_access_point_policy)

```python
# get_multi_region_access_point_policy method definition

await def get_multi_region_access_point_policy(
    self,
    *,
    AccountId: str,
    Name: str,
) -> GetMultiRegionAccessPointPolicyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMultiRegionAccessPointPolicyResultTypeDef](./type_defs.md#getmultiregionaccesspointpolicyresulttypedef) 


```python
# get_multi_region_access_point_policy method usage example with argument unpacking

kwargs: GetMultiRegionAccessPointPolicyRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.get_multi_region_access_point_policy(**kwargs)
```

1. See [:material-code-braces: GetMultiRegionAccessPointPolicyRequestRequestTypeDef](./type_defs.md#getmultiregionaccesspointpolicyrequestrequesttypedef) 

### get\_multi\_region\_access\_point\_policy\_status

.

Type annotations and code completion for `#!python session.create_client("s3control").get_multi_region_access_point_policy_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_multi_region_access_point_policy_status)

```python
# get_multi_region_access_point_policy_status method definition

await def get_multi_region_access_point_policy_status(
    self,
    *,
    AccountId: str,
    Name: str,
) -> GetMultiRegionAccessPointPolicyStatusResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMultiRegionAccessPointPolicyStatusResultTypeDef](./type_defs.md#getmultiregionaccesspointpolicystatusresulttypedef) 


```python
# get_multi_region_access_point_policy_status method usage example with argument unpacking

kwargs: GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.get_multi_region_access_point_policy_status(**kwargs)
```

1. See [:material-code-braces: GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef](./type_defs.md#getmultiregionaccesspointpolicystatusrequestrequesttypedef) 

### get\_multi\_region\_access\_point\_routes

.

Type annotations and code completion for `#!python session.create_client("s3control").get_multi_region_access_point_routes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_multi_region_access_point_routes)

```python
# get_multi_region_access_point_routes method definition

await def get_multi_region_access_point_routes(
    self,
    *,
    AccountId: str,
    Mrap: str,
) -> GetMultiRegionAccessPointRoutesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMultiRegionAccessPointRoutesResultTypeDef](./type_defs.md#getmultiregionaccesspointroutesresulttypedef) 


```python
# get_multi_region_access_point_routes method usage example with argument unpacking

kwargs: GetMultiRegionAccessPointRoutesRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Mrap": ...,
}

parent.get_multi_region_access_point_routes(**kwargs)
```

1. See [:material-code-braces: GetMultiRegionAccessPointRoutesRequestRequestTypeDef](./type_defs.md#getmultiregionaccesspointroutesrequestrequesttypedef) 

### get\_public\_access\_block

.

Type annotations and code completion for `#!python session.create_client("s3control").get_public_access_block` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_public_access_block)

```python
# get_public_access_block method definition

await def get_public_access_block(
    self,
    *,
    AccountId: str,
) -> GetPublicAccessBlockOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPublicAccessBlockOutputTypeDef](./type_defs.md#getpublicaccessblockoutputtypedef) 


```python
# get_public_access_block method usage example with argument unpacking

kwargs: GetPublicAccessBlockRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.get_public_access_block(**kwargs)
```

1. See [:material-code-braces: GetPublicAccessBlockRequestRequestTypeDef](./type_defs.md#getpublicaccessblockrequestrequesttypedef) 

### get\_storage\_lens\_configuration

.

Type annotations and code completion for `#!python session.create_client("s3control").get_storage_lens_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_storage_lens_configuration)

```python
# get_storage_lens_configuration method definition

await def get_storage_lens_configuration(
    self,
    *,
    ConfigId: str,
    AccountId: str,
) -> GetStorageLensConfigurationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStorageLensConfigurationResultTypeDef](./type_defs.md#getstoragelensconfigurationresulttypedef) 


```python
# get_storage_lens_configuration method usage example with argument unpacking

kwargs: GetStorageLensConfigurationRequestRequestTypeDef = {  # (1)
    "ConfigId": ...,
    "AccountId": ...,
}

parent.get_storage_lens_configuration(**kwargs)
```

1. See [:material-code-braces: GetStorageLensConfigurationRequestRequestTypeDef](./type_defs.md#getstoragelensconfigurationrequestrequesttypedef) 

### get\_storage\_lens\_configuration\_tagging

.

Type annotations and code completion for `#!python session.create_client("s3control").get_storage_lens_configuration_tagging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_storage_lens_configuration_tagging)

```python
# get_storage_lens_configuration_tagging method definition

await def get_storage_lens_configuration_tagging(
    self,
    *,
    ConfigId: str,
    AccountId: str,
) -> GetStorageLensConfigurationTaggingResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStorageLensConfigurationTaggingResultTypeDef](./type_defs.md#getstoragelensconfigurationtaggingresulttypedef) 


```python
# get_storage_lens_configuration_tagging method usage example with argument unpacking

kwargs: GetStorageLensConfigurationTaggingRequestRequestTypeDef = {  # (1)
    "ConfigId": ...,
    "AccountId": ...,
}

parent.get_storage_lens_configuration_tagging(**kwargs)
```

1. See [:material-code-braces: GetStorageLensConfigurationTaggingRequestRequestTypeDef](./type_defs.md#getstoragelensconfigurationtaggingrequestrequesttypedef) 

### get\_storage\_lens\_group

Retrieves the Storage Lens group configuration details.

Type annotations and code completion for `#!python session.create_client("s3control").get_storage_lens_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_storage_lens_group)

```python
# get_storage_lens_group method definition

await def get_storage_lens_group(
    self,
    *,
    Name: str,
    AccountId: str,
) -> GetStorageLensGroupResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStorageLensGroupResultTypeDef](./type_defs.md#getstoragelensgroupresulttypedef) 


```python
# get_storage_lens_group method usage example with argument unpacking

kwargs: GetStorageLensGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "AccountId": ...,
}

parent.get_storage_lens_group(**kwargs)
```

1. See [:material-code-braces: GetStorageLensGroupRequestRequestTypeDef](./type_defs.md#getstoragelensgrouprequestrequesttypedef) 

### list\_access\_grants

Returns the list of access grants in your S3 Access Grants instance.

Type annotations and code completion for `#!python session.create_client("s3control").list_access_grants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_access_grants)

```python
# list_access_grants method definition

await def list_access_grants(
    self,
    *,
    AccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    GranteeType: GranteeTypeType = ...,  # (1)
    GranteeIdentifier: str = ...,
    Permission: PermissionType = ...,  # (2)
    GrantScope: str = ...,
    ApplicationArn: str = ...,
) -> ListAccessGrantsResultTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: GranteeTypeType](./literals.md#granteetypetype) 
2. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
3. See [:material-code-braces: ListAccessGrantsResultTypeDef](./type_defs.md#listaccessgrantsresulttypedef) 


```python
# list_access_grants method usage example with argument unpacking

kwargs: ListAccessGrantsRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_access_grants(**kwargs)
```

1. See [:material-code-braces: ListAccessGrantsRequestRequestTypeDef](./type_defs.md#listaccessgrantsrequestrequesttypedef) 

### list\_access\_grants\_instances

Returns a list of S3 Access Grants instances.

Type annotations and code completion for `#!python session.create_client("s3control").list_access_grants_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_access_grants_instances)

```python
# list_access_grants_instances method definition

await def list_access_grants_instances(
    self,
    *,
    AccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAccessGrantsInstancesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccessGrantsInstancesResultTypeDef](./type_defs.md#listaccessgrantsinstancesresulttypedef) 


```python
# list_access_grants_instances method usage example with argument unpacking

kwargs: ListAccessGrantsInstancesRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_access_grants_instances(**kwargs)
```

1. See [:material-code-braces: ListAccessGrantsInstancesRequestRequestTypeDef](./type_defs.md#listaccessgrantsinstancesrequestrequesttypedef) 

### list\_access\_grants\_locations

Returns a list of the locations registered in your S3 Access Grants instance.

Type annotations and code completion for `#!python session.create_client("s3control").list_access_grants_locations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_access_grants_locations)

```python
# list_access_grants_locations method definition

await def list_access_grants_locations(
    self,
    *,
    AccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    LocationScope: str = ...,
) -> ListAccessGrantsLocationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccessGrantsLocationsResultTypeDef](./type_defs.md#listaccessgrantslocationsresulttypedef) 


```python
# list_access_grants_locations method usage example with argument unpacking

kwargs: ListAccessGrantsLocationsRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_access_grants_locations(**kwargs)
```

1. See [:material-code-braces: ListAccessGrantsLocationsRequestRequestTypeDef](./type_defs.md#listaccessgrantslocationsrequestrequesttypedef) 

### list\_access\_points

.

Type annotations and code completion for `#!python session.create_client("s3control").list_access_points` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_access_points)

```python
# list_access_points method definition

await def list_access_points(
    self,
    *,
    AccountId: str,
    Bucket: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAccessPointsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccessPointsResultTypeDef](./type_defs.md#listaccesspointsresulttypedef) 


```python
# list_access_points method usage example with argument unpacking

kwargs: ListAccessPointsRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_access_points(**kwargs)
```

1. See [:material-code-braces: ListAccessPointsRequestRequestTypeDef](./type_defs.md#listaccesspointsrequestrequesttypedef) 

### list\_access\_points\_for\_object\_lambda

.

Type annotations and code completion for `#!python session.create_client("s3control").list_access_points_for_object_lambda` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_access_points_for_object_lambda)

```python
# list_access_points_for_object_lambda method definition

await def list_access_points_for_object_lambda(
    self,
    *,
    AccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAccessPointsForObjectLambdaResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccessPointsForObjectLambdaResultTypeDef](./type_defs.md#listaccesspointsforobjectlambdaresulttypedef) 


```python
# list_access_points_for_object_lambda method usage example with argument unpacking

kwargs: ListAccessPointsForObjectLambdaRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_access_points_for_object_lambda(**kwargs)
```

1. See [:material-code-braces: ListAccessPointsForObjectLambdaRequestRequestTypeDef](./type_defs.md#listaccesspointsforobjectlambdarequestrequesttypedef) 

### list\_caller\_access\_grants

Returns a list of the access grants that were given to the caller using S3
Access Grants and that allow the caller to access the S3 data of the Amazon Web
Services account specified in the
request.

Type annotations and code completion for `#!python session.create_client("s3control").list_caller_access_grants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_caller_access_grants)

```python
# list_caller_access_grants method definition

await def list_caller_access_grants(
    self,
    *,
    AccountId: str,
    GrantScope: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    AllowedByApplication: bool = ...,
) -> ListCallerAccessGrantsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCallerAccessGrantsResultTypeDef](./type_defs.md#listcalleraccessgrantsresulttypedef) 


```python
# list_caller_access_grants method usage example with argument unpacking

kwargs: ListCallerAccessGrantsRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_caller_access_grants(**kwargs)
```

1. See [:material-code-braces: ListCallerAccessGrantsRequestRequestTypeDef](./type_defs.md#listcalleraccessgrantsrequestrequesttypedef) 

### list\_jobs

Lists current S3 Batch Operations jobs as well as the jobs that have ended
within the last 90 days for the Amazon Web Services account making the
request.

Type annotations and code completion for `#!python session.create_client("s3control").list_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_jobs)

```python
# list_jobs method definition

await def list_jobs(
    self,
    *,
    AccountId: str,
    JobStatuses: Sequence[JobStatusType] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListJobsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef) 


```python
# list_jobs method usage example with argument unpacking

kwargs: ListJobsRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_jobs(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef) 

### list\_multi\_region\_access\_points

.

Type annotations and code completion for `#!python session.create_client("s3control").list_multi_region_access_points` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_multi_region_access_points)

```python
# list_multi_region_access_points method definition

await def list_multi_region_access_points(
    self,
    *,
    AccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMultiRegionAccessPointsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMultiRegionAccessPointsResultTypeDef](./type_defs.md#listmultiregionaccesspointsresulttypedef) 


```python
# list_multi_region_access_points method usage example with argument unpacking

kwargs: ListMultiRegionAccessPointsRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_multi_region_access_points(**kwargs)
```

1. See [:material-code-braces: ListMultiRegionAccessPointsRequestRequestTypeDef](./type_defs.md#listmultiregionaccesspointsrequestrequesttypedef) 

### list\_regional\_buckets

.

Type annotations and code completion for `#!python session.create_client("s3control").list_regional_buckets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_regional_buckets)

```python
# list_regional_buckets method definition

await def list_regional_buckets(
    self,
    *,
    AccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    OutpostId: str = ...,
) -> ListRegionalBucketsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRegionalBucketsResultTypeDef](./type_defs.md#listregionalbucketsresulttypedef) 


```python
# list_regional_buckets method usage example with argument unpacking

kwargs: ListRegionalBucketsRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_regional_buckets(**kwargs)
```

1. See [:material-code-braces: ListRegionalBucketsRequestRequestTypeDef](./type_defs.md#listregionalbucketsrequestrequesttypedef) 

### list\_storage\_lens\_configurations

.

Type annotations and code completion for `#!python session.create_client("s3control").list_storage_lens_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_storage_lens_configurations)

```python
# list_storage_lens_configurations method definition

await def list_storage_lens_configurations(
    self,
    *,
    AccountId: str,
    NextToken: str = ...,
) -> ListStorageLensConfigurationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStorageLensConfigurationsResultTypeDef](./type_defs.md#liststoragelensconfigurationsresulttypedef) 


```python
# list_storage_lens_configurations method usage example with argument unpacking

kwargs: ListStorageLensConfigurationsRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_storage_lens_configurations(**kwargs)
```

1. See [:material-code-braces: ListStorageLensConfigurationsRequestRequestTypeDef](./type_defs.md#liststoragelensconfigurationsrequestrequesttypedef) 

### list\_storage\_lens\_groups

Lists all the Storage Lens groups in the specified home Region.

Type annotations and code completion for `#!python session.create_client("s3control").list_storage_lens_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_storage_lens_groups)

```python
# list_storage_lens_groups method definition

await def list_storage_lens_groups(
    self,
    *,
    AccountId: str,
    NextToken: str = ...,
) -> ListStorageLensGroupsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStorageLensGroupsResultTypeDef](./type_defs.md#liststoragelensgroupsresulttypedef) 


```python
# list_storage_lens_groups method usage example with argument unpacking

kwargs: ListStorageLensGroupsRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_storage_lens_groups(**kwargs)
```

1. See [:material-code-braces: ListStorageLensGroupsRequestRequestTypeDef](./type_defs.md#liststoragelensgroupsrequestrequesttypedef) 

### list\_tags\_for\_resource

This operation allows you to list all the Amazon Web Services resource tags for
a specified
resource.

Type annotations and code completion for `#!python session.create_client("s3control").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    AccountId: str,
    ResourceArn: str,
) -> ListTagsForResourceResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_access\_grants\_instance\_resource\_policy

Updates the resource policy of the S3 Access Grants instance.

Type annotations and code completion for `#!python session.create_client("s3control").put_access_grants_instance_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_grants_instance_resource_policy)

```python
# put_access_grants_instance_resource_policy method definition

await def put_access_grants_instance_resource_policy(
    self,
    *,
    AccountId: str,
    Policy: str,
    Organization: str = ...,
) -> PutAccessGrantsInstanceResourcePolicyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutAccessGrantsInstanceResourcePolicyResultTypeDef](./type_defs.md#putaccessgrantsinstanceresourcepolicyresulttypedef) 


```python
# put_access_grants_instance_resource_policy method usage example with argument unpacking

kwargs: PutAccessGrantsInstanceResourcePolicyRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Policy": ...,
}

parent.put_access_grants_instance_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutAccessGrantsInstanceResourcePolicyRequestRequestTypeDef](./type_defs.md#putaccessgrantsinstanceresourcepolicyrequestrequesttypedef) 

### put\_access\_point\_configuration\_for\_object\_lambda

.

Type annotations and code completion for `#!python session.create_client("s3control").put_access_point_configuration_for_object_lambda` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_point_configuration_for_object_lambda)

```python
# put_access_point_configuration_for_object_lambda method definition

await def put_access_point_configuration_for_object_lambda(
    self,
    *,
    AccountId: str,
    Name: str,
    Configuration: ObjectLambdaConfigurationTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ObjectLambdaConfigurationTypeDef](./type_defs.md#objectlambdaconfigurationtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_access_point_configuration_for_object_lambda method usage example with argument unpacking

kwargs: PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
    "Configuration": ...,
}

parent.put_access_point_configuration_for_object_lambda(**kwargs)
```

1. See [:material-code-braces: PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef](./type_defs.md#putaccesspointconfigurationforobjectlambdarequestrequesttypedef) 

### put\_access\_point\_policy

.

Type annotations and code completion for `#!python session.create_client("s3control").put_access_point_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_point_policy)

```python
# put_access_point_policy method definition

await def put_access_point_policy(
    self,
    *,
    AccountId: str,
    Name: str,
    Policy: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_access_point_policy method usage example with argument unpacking

kwargs: PutAccessPointPolicyRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
    "Policy": ...,
}

parent.put_access_point_policy(**kwargs)
```

1. See [:material-code-braces: PutAccessPointPolicyRequestRequestTypeDef](./type_defs.md#putaccesspointpolicyrequestrequesttypedef) 

### put\_access\_point\_policy\_for\_object\_lambda

.

Type annotations and code completion for `#!python session.create_client("s3control").put_access_point_policy_for_object_lambda` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_point_policy_for_object_lambda)

```python
# put_access_point_policy_for_object_lambda method definition

await def put_access_point_policy_for_object_lambda(
    self,
    *,
    AccountId: str,
    Name: str,
    Policy: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_access_point_policy_for_object_lambda method usage example with argument unpacking

kwargs: PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
    "Policy": ...,
}

parent.put_access_point_policy_for_object_lambda(**kwargs)
```

1. See [:material-code-braces: PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef](./type_defs.md#putaccesspointpolicyforobjectlambdarequestrequesttypedef) 

### put\_bucket\_lifecycle\_configuration

.

Type annotations and code completion for `#!python session.create_client("s3control").put_bucket_lifecycle_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_lifecycle_configuration)

```python
# put_bucket_lifecycle_configuration method definition

await def put_bucket_lifecycle_configuration(
    self,
    *,
    AccountId: str,
    Bucket: str,
    LifecycleConfiguration: LifecycleConfigurationTypeDef = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LifecycleConfigurationTypeDef](./type_defs.md#lifecycleconfigurationtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_bucket_lifecycle_configuration method usage example with argument unpacking

kwargs: PutBucketLifecycleConfigurationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
}

parent.put_bucket_lifecycle_configuration(**kwargs)
```

1. See [:material-code-braces: PutBucketLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#putbucketlifecycleconfigurationrequestrequesttypedef) 

### put\_bucket\_policy

.

Type annotations and code completion for `#!python session.create_client("s3control").put_bucket_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_policy)

```python
# put_bucket_policy method definition

await def put_bucket_policy(
    self,
    *,
    AccountId: str,
    Bucket: str,
    Policy: str,
    ConfirmRemoveSelfBucketAccess: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_bucket_policy method usage example with argument unpacking

kwargs: PutBucketPolicyRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
    "Policy": ...,
}

parent.put_bucket_policy(**kwargs)
```

1. See [:material-code-braces: PutBucketPolicyRequestRequestTypeDef](./type_defs.md#putbucketpolicyrequestrequesttypedef) 

### put\_bucket\_replication

.

Type annotations and code completion for `#!python session.create_client("s3control").put_bucket_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_replication)

```python
# put_bucket_replication method definition

await def put_bucket_replication(
    self,
    *,
    AccountId: str,
    Bucket: str,
    ReplicationConfiguration: ReplicationConfigurationTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_bucket_replication method usage example with argument unpacking

kwargs: PutBucketReplicationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
    "ReplicationConfiguration": ...,
}

parent.put_bucket_replication(**kwargs)
```

1. See [:material-code-braces: PutBucketReplicationRequestRequestTypeDef](./type_defs.md#putbucketreplicationrequestrequesttypedef) 

### put\_bucket\_tagging

.

Type annotations and code completion for `#!python session.create_client("s3control").put_bucket_tagging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_tagging)

```python
# put_bucket_tagging method definition

await def put_bucket_tagging(
    self,
    *,
    AccountId: str,
    Bucket: str,
    Tagging: TaggingTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TaggingTypeDef](./type_defs.md#taggingtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_bucket_tagging method usage example with argument unpacking

kwargs: PutBucketTaggingRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
    "Tagging": ...,
}

parent.put_bucket_tagging(**kwargs)
```

1. See [:material-code-braces: PutBucketTaggingRequestRequestTypeDef](./type_defs.md#putbuckettaggingrequestrequesttypedef) 

### put\_bucket\_versioning

.

Type annotations and code completion for `#!python session.create_client("s3control").put_bucket_versioning` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_versioning)

```python
# put_bucket_versioning method definition

await def put_bucket_versioning(
    self,
    *,
    AccountId: str,
    Bucket: str,
    VersioningConfiguration: VersioningConfigurationTypeDef,  # (1)
    MFA: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_bucket_versioning method usage example with argument unpacking

kwargs: PutBucketVersioningRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Bucket": ...,
    "VersioningConfiguration": ...,
}

parent.put_bucket_versioning(**kwargs)
```

1. See [:material-code-braces: PutBucketVersioningRequestRequestTypeDef](./type_defs.md#putbucketversioningrequestrequesttypedef) 

### put\_job\_tagging

Sets the supplied tag-set on an S3 Batch Operations job.

Type annotations and code completion for `#!python session.create_client("s3control").put_job_tagging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_job_tagging)

```python
# put_job_tagging method definition

await def put_job_tagging(
    self,
    *,
    AccountId: str,
    JobId: str,
    Tags: Sequence[S3TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: S3TagTypeDef](./type_defs.md#s3tagtypedef) 


```python
# put_job_tagging method usage example with argument unpacking

kwargs: PutJobTaggingRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "JobId": ...,
    "Tags": ...,
}

parent.put_job_tagging(**kwargs)
```

1. See [:material-code-braces: PutJobTaggingRequestRequestTypeDef](./type_defs.md#putjobtaggingrequestrequesttypedef) 

### put\_multi\_region\_access\_point\_policy

.

Type annotations and code completion for `#!python session.create_client("s3control").put_multi_region_access_point_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_multi_region_access_point_policy)

```python
# put_multi_region_access_point_policy method definition

await def put_multi_region_access_point_policy(
    self,
    *,
    AccountId: str,
    ClientToken: str,
    Details: PutMultiRegionAccessPointPolicyInputTypeDef,  # (1)
) -> PutMultiRegionAccessPointPolicyResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PutMultiRegionAccessPointPolicyInputTypeDef](./type_defs.md#putmultiregionaccesspointpolicyinputtypedef) 
2. See [:material-code-braces: PutMultiRegionAccessPointPolicyResultTypeDef](./type_defs.md#putmultiregionaccesspointpolicyresulttypedef) 


```python
# put_multi_region_access_point_policy method usage example with argument unpacking

kwargs: PutMultiRegionAccessPointPolicyRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "ClientToken": ...,
    "Details": ...,
}

parent.put_multi_region_access_point_policy(**kwargs)
```

1. See [:material-code-braces: PutMultiRegionAccessPointPolicyRequestRequestTypeDef](./type_defs.md#putmultiregionaccesspointpolicyrequestrequesttypedef) 

### put\_public\_access\_block

.

Type annotations and code completion for `#!python session.create_client("s3control").put_public_access_block` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_public_access_block)

```python
# put_public_access_block method definition

await def put_public_access_block(
    self,
    *,
    PublicAccessBlockConfiguration: PublicAccessBlockConfigurationTypeDef,  # (1)
    AccountId: str,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PublicAccessBlockConfigurationTypeDef](./type_defs.md#publicaccessblockconfigurationtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_public_access_block method usage example with argument unpacking

kwargs: PutPublicAccessBlockRequestRequestTypeDef = {  # (1)
    "PublicAccessBlockConfiguration": ...,
    "AccountId": ...,
}

parent.put_public_access_block(**kwargs)
```

1. See [:material-code-braces: PutPublicAccessBlockRequestRequestTypeDef](./type_defs.md#putpublicaccessblockrequestrequesttypedef) 

### put\_storage\_lens\_configuration

.

Type annotations and code completion for `#!python session.create_client("s3control").put_storage_lens_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_storage_lens_configuration)

```python
# put_storage_lens_configuration method definition

await def put_storage_lens_configuration(
    self,
    *,
    ConfigId: str,
    AccountId: str,
    StorageLensConfiguration: StorageLensConfigurationTypeDef,  # (1)
    Tags: Sequence[StorageLensTagTypeDef] = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: StorageLensConfigurationTypeDef](./type_defs.md#storagelensconfigurationtypedef) 
2. See [:material-code-braces: StorageLensTagTypeDef](./type_defs.md#storagelenstagtypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_storage_lens_configuration method usage example with argument unpacking

kwargs: PutStorageLensConfigurationRequestRequestTypeDef = {  # (1)
    "ConfigId": ...,
    "AccountId": ...,
    "StorageLensConfiguration": ...,
}

parent.put_storage_lens_configuration(**kwargs)
```

1. See [:material-code-braces: PutStorageLensConfigurationRequestRequestTypeDef](./type_defs.md#putstoragelensconfigurationrequestrequesttypedef) 

### put\_storage\_lens\_configuration\_tagging

.

Type annotations and code completion for `#!python session.create_client("s3control").put_storage_lens_configuration_tagging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_storage_lens_configuration_tagging)

```python
# put_storage_lens_configuration_tagging method definition

await def put_storage_lens_configuration_tagging(
    self,
    *,
    ConfigId: str,
    AccountId: str,
    Tags: Sequence[StorageLensTagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: StorageLensTagTypeDef](./type_defs.md#storagelenstagtypedef) 


```python
# put_storage_lens_configuration_tagging method usage example with argument unpacking

kwargs: PutStorageLensConfigurationTaggingRequestRequestTypeDef = {  # (1)
    "ConfigId": ...,
    "AccountId": ...,
    "Tags": ...,
}

parent.put_storage_lens_configuration_tagging(**kwargs)
```

1. See [:material-code-braces: PutStorageLensConfigurationTaggingRequestRequestTypeDef](./type_defs.md#putstoragelensconfigurationtaggingrequestrequesttypedef) 

### submit\_multi\_region\_access\_point\_routes

.

Type annotations and code completion for `#!python session.create_client("s3control").submit_multi_region_access_point_routes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.submit_multi_region_access_point_routes)

```python
# submit_multi_region_access_point_routes method definition

await def submit_multi_region_access_point_routes(
    self,
    *,
    AccountId: str,
    Mrap: str,
    RouteUpdates: Sequence[MultiRegionAccessPointRouteTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: MultiRegionAccessPointRouteTypeDef](./type_defs.md#multiregionaccesspointroutetypedef) 


```python
# submit_multi_region_access_point_routes method usage example with argument unpacking

kwargs: SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Mrap": ...,
    "RouteUpdates": ...,
}

parent.submit_multi_region_access_point_routes(**kwargs)
```

1. See [:material-code-braces: SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef](./type_defs.md#submitmultiregionaccesspointroutesrequestrequesttypedef) 

### tag\_resource

Creates a new Amazon Web Services resource tag or updates an existing resource
tag.

Type annotations and code completion for `#!python session.create_client("s3control").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    AccountId: str,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

This operation removes the specified Amazon Web Services resource tags from an
S3
resource.

Type annotations and code completion for `#!python session.create_client("s3control").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    AccountId: str,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_access\_grants\_location

Updates the IAM role of a registered location in your S3 Access Grants instance.

Type annotations and code completion for `#!python session.create_client("s3control").update_access_grants_location` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.update_access_grants_location)

```python
# update_access_grants_location method definition

await def update_access_grants_location(
    self,
    *,
    AccountId: str,
    AccessGrantsLocationId: str,
    IAMRoleArn: str,
) -> UpdateAccessGrantsLocationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAccessGrantsLocationResultTypeDef](./type_defs.md#updateaccessgrantslocationresulttypedef) 


```python
# update_access_grants_location method usage example with argument unpacking

kwargs: UpdateAccessGrantsLocationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "AccessGrantsLocationId": ...,
    "IAMRoleArn": ...,
}

parent.update_access_grants_location(**kwargs)
```

1. See [:material-code-braces: UpdateAccessGrantsLocationRequestRequestTypeDef](./type_defs.md#updateaccessgrantslocationrequestrequesttypedef) 

### update\_job\_priority

Updates an existing S3 Batch Operations job's priority.

Type annotations and code completion for `#!python session.create_client("s3control").update_job_priority` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.update_job_priority)

```python
# update_job_priority method definition

await def update_job_priority(
    self,
    *,
    AccountId: str,
    JobId: str,
    Priority: int,
) -> UpdateJobPriorityResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateJobPriorityResultTypeDef](./type_defs.md#updatejobpriorityresulttypedef) 


```python
# update_job_priority method usage example with argument unpacking

kwargs: UpdateJobPriorityRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "JobId": ...,
    "Priority": ...,
}

parent.update_job_priority(**kwargs)
```

1. See [:material-code-braces: UpdateJobPriorityRequestRequestTypeDef](./type_defs.md#updatejobpriorityrequestrequesttypedef) 

### update\_job\_status

Updates the status for the specified job.

Type annotations and code completion for `#!python session.create_client("s3control").update_job_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.update_job_status)

```python
# update_job_status method definition

await def update_job_status(
    self,
    *,
    AccountId: str,
    JobId: str,
    RequestedJobStatus: RequestedJobStatusType,  # (1)
    StatusUpdateReason: str = ...,
) -> UpdateJobStatusResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RequestedJobStatusType](./literals.md#requestedjobstatustype) 
2. See [:material-code-braces: UpdateJobStatusResultTypeDef](./type_defs.md#updatejobstatusresulttypedef) 


```python
# update_job_status method usage example with argument unpacking

kwargs: UpdateJobStatusRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "JobId": ...,
    "RequestedJobStatus": ...,
}

parent.update_job_status(**kwargs)
```

1. See [:material-code-braces: UpdateJobStatusRequestRequestTypeDef](./type_defs.md#updatejobstatusrequestrequesttypedef) 

### update\_storage\_lens\_group

Updates the existing Storage Lens group.

Type annotations and code completion for `#!python session.create_client("s3control").update_storage_lens_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.update_storage_lens_group)

```python
# update_storage_lens_group method definition

await def update_storage_lens_group(
    self,
    *,
    Name: str,
    AccountId: str,
    StorageLensGroup: StorageLensGroupTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StorageLensGroupTypeDef](./type_defs.md#storagelensgrouptypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_storage_lens_group method usage example with argument unpacking

kwargs: UpdateStorageLensGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "AccountId": ...,
    "StorageLensGroup": ...,
}

parent.update_storage_lens_group(**kwargs)
```

1. See [:material-code-braces: UpdateStorageLensGroupRequestRequestTypeDef](./type_defs.md#updatestoragelensgrouprequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("s3control").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "S3ControlClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("s3control").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("s3control").get_paginator` method with overloads.

- `client.get_paginator("list_access_points_for_object_lambda")` -> [ListAccessPointsForObjectLambdaPaginator](./paginators.md#listaccesspointsforobjectlambdapaginator)
- `client.get_paginator("list_caller_access_grants")` -> [ListCallerAccessGrantsPaginator](./paginators.md#listcalleraccessgrantspaginator)



