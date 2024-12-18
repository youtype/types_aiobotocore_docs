# SignerClient

> [Index](../README.md) > [Signer](./README.md) > SignerClient

!!! note ""

    Auto-generated documentation for [Signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
    type annotations stubs module [types-aiobotocore-signer](https://pypi.org/project/types-aiobotocore-signer/).

## SignerClient

Type annotations and code completion for `#!python session.create_client("signer")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client)

```python
# SignerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_signer.client import SignerClient

session = get_session()
async with session.create_client("signer") as client:
    client: SignerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("signer").exceptions` structure.

```python
# SignerClient.exceptions usage example

async with session.create_client("signer") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.InternalServiceErrorException,
        client.NotFoundException,
        client.ResourceNotFoundException,
        client.ServiceLimitExceededException,
        client.ThrottlingException,
        client.TooManyRequestsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# SignerClient usage type checking example

from types_aiobotocore_signer.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("signer").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("signer").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/generate_presigned_url.html)

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



Type annotations and code completion for `#!python session.create_client("signer").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### add\_profile\_permission

Adds cross-account permissions to a signing profile.

Type annotations and code completion for `#!python session.create_client("signer").add_profile_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/add_profile_permission.html)

```python
# add_profile_permission method definition

await def add_profile_permission(
    self,
    *,
    profileName: str,
    action: str,
    principal: str,
    statementId: str,
    profileVersion: str = ...,
    revisionId: str = ...,
) -> AddProfilePermissionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AddProfilePermissionResponseTypeDef](./type_defs.md#addprofilepermissionresponsetypedef) 


```python
# add_profile_permission method usage example with argument unpacking

kwargs: AddProfilePermissionRequestRequestTypeDef = {  # (1)
    "profileName": ...,
    "action": ...,
    "principal": ...,
    "statementId": ...,
}

parent.add_profile_permission(**kwargs)
```

1. See [:material-code-braces: AddProfilePermissionRequestRequestTypeDef](./type_defs.md#addprofilepermissionrequestrequesttypedef) 

### cancel\_signing\_profile

Changes the state of an <code>ACTIVE</code> signing profile to
<code>CANCELED</code>.

Type annotations and code completion for `#!python session.create_client("signer").cancel_signing_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/cancel_signing_profile.html)

```python
# cancel_signing_profile method definition

await def cancel_signing_profile(
    self,
    *,
    profileName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# cancel_signing_profile method usage example with argument unpacking

kwargs: CancelSigningProfileRequestRequestTypeDef = {  # (1)
    "profileName": ...,
}

parent.cancel_signing_profile(**kwargs)
```

1. See [:material-code-braces: CancelSigningProfileRequestRequestTypeDef](./type_defs.md#cancelsigningprofilerequestrequesttypedef) 

### describe\_signing\_job

Returns information about a specific code signing job.

Type annotations and code completion for `#!python session.create_client("signer").describe_signing_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/describe_signing_job.html)

```python
# describe_signing_job method definition

await def describe_signing_job(
    self,
    *,
    jobId: str,
) -> DescribeSigningJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSigningJobResponseTypeDef](./type_defs.md#describesigningjobresponsetypedef) 


```python
# describe_signing_job method usage example with argument unpacking

kwargs: DescribeSigningJobRequestRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.describe_signing_job(**kwargs)
```

1. See [:material-code-braces: DescribeSigningJobRequestRequestTypeDef](./type_defs.md#describesigningjobrequestrequesttypedef) 

### get\_revocation\_status

Retrieves the revocation status of one or more of the signing profile, signing
job, and signing certificate.

Type annotations and code completion for `#!python session.create_client("signer").get_revocation_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/get_revocation_status.html)

```python
# get_revocation_status method definition

await def get_revocation_status(
    self,
    *,
    signatureTimestamp: TimestampTypeDef,
    platformId: str,
    profileVersionArn: str,
    jobArn: str,
    certificateHashes: Sequence[str],
) -> GetRevocationStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRevocationStatusResponseTypeDef](./type_defs.md#getrevocationstatusresponsetypedef) 


```python
# get_revocation_status method usage example with argument unpacking

kwargs: GetRevocationStatusRequestRequestTypeDef = {  # (1)
    "signatureTimestamp": ...,
    "platformId": ...,
    "profileVersionArn": ...,
    "jobArn": ...,
    "certificateHashes": ...,
}

parent.get_revocation_status(**kwargs)
```

1. See [:material-code-braces: GetRevocationStatusRequestRequestTypeDef](./type_defs.md#getrevocationstatusrequestrequesttypedef) 

### get\_signing\_platform

Returns information on a specific signing platform.

Type annotations and code completion for `#!python session.create_client("signer").get_signing_platform` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/get_signing_platform.html)

```python
# get_signing_platform method definition

await def get_signing_platform(
    self,
    *,
    platformId: str,
) -> GetSigningPlatformResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSigningPlatformResponseTypeDef](./type_defs.md#getsigningplatformresponsetypedef) 


```python
# get_signing_platform method usage example with argument unpacking

kwargs: GetSigningPlatformRequestRequestTypeDef = {  # (1)
    "platformId": ...,
}

parent.get_signing_platform(**kwargs)
```

1. See [:material-code-braces: GetSigningPlatformRequestRequestTypeDef](./type_defs.md#getsigningplatformrequestrequesttypedef) 

### get\_signing\_profile

Returns information on a specific signing profile.

Type annotations and code completion for `#!python session.create_client("signer").get_signing_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/get_signing_profile.html)

```python
# get_signing_profile method definition

await def get_signing_profile(
    self,
    *,
    profileName: str,
    profileOwner: str = ...,
) -> GetSigningProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSigningProfileResponseTypeDef](./type_defs.md#getsigningprofileresponsetypedef) 


```python
# get_signing_profile method usage example with argument unpacking

kwargs: GetSigningProfileRequestRequestTypeDef = {  # (1)
    "profileName": ...,
}

parent.get_signing_profile(**kwargs)
```

1. See [:material-code-braces: GetSigningProfileRequestRequestTypeDef](./type_defs.md#getsigningprofilerequestrequesttypedef) 

### list\_profile\_permissions

Lists the cross-account permissions associated with a signing profile.

Type annotations and code completion for `#!python session.create_client("signer").list_profile_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/list_profile_permissions.html)

```python
# list_profile_permissions method definition

await def list_profile_permissions(
    self,
    *,
    profileName: str,
    nextToken: str = ...,
) -> ListProfilePermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProfilePermissionsResponseTypeDef](./type_defs.md#listprofilepermissionsresponsetypedef) 


```python
# list_profile_permissions method usage example with argument unpacking

kwargs: ListProfilePermissionsRequestRequestTypeDef = {  # (1)
    "profileName": ...,
}

parent.list_profile_permissions(**kwargs)
```

1. See [:material-code-braces: ListProfilePermissionsRequestRequestTypeDef](./type_defs.md#listprofilepermissionsrequestrequesttypedef) 

### list\_signing\_jobs

Lists all your signing jobs.

Type annotations and code completion for `#!python session.create_client("signer").list_signing_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/list_signing_jobs.html)

```python
# list_signing_jobs method definition

await def list_signing_jobs(
    self,
    *,
    status: SigningStatusType = ...,  # (1)
    platformId: str = ...,
    requestedBy: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    isRevoked: bool = ...,
    signatureExpiresBefore: TimestampTypeDef = ...,
    signatureExpiresAfter: TimestampTypeDef = ...,
    jobInvoker: str = ...,
) -> ListSigningJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SigningStatusType](./literals.md#signingstatustype) 
2. See [:material-code-braces: ListSigningJobsResponseTypeDef](./type_defs.md#listsigningjobsresponsetypedef) 


```python
# list_signing_jobs method usage example with argument unpacking

kwargs: ListSigningJobsRequestRequestTypeDef = {  # (1)
    "status": ...,
}

parent.list_signing_jobs(**kwargs)
```

1. See [:material-code-braces: ListSigningJobsRequestRequestTypeDef](./type_defs.md#listsigningjobsrequestrequesttypedef) 

### list\_signing\_platforms

Lists all signing platforms available in AWS Signer that match the request
parameters.

Type annotations and code completion for `#!python session.create_client("signer").list_signing_platforms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/list_signing_platforms.html)

```python
# list_signing_platforms method definition

await def list_signing_platforms(
    self,
    *,
    category: str = ...,
    partner: str = ...,
    target: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSigningPlatformsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSigningPlatformsResponseTypeDef](./type_defs.md#listsigningplatformsresponsetypedef) 


```python
# list_signing_platforms method usage example with argument unpacking

kwargs: ListSigningPlatformsRequestRequestTypeDef = {  # (1)
    "category": ...,
}

parent.list_signing_platforms(**kwargs)
```

1. See [:material-code-braces: ListSigningPlatformsRequestRequestTypeDef](./type_defs.md#listsigningplatformsrequestrequesttypedef) 

### list\_signing\_profiles

Lists all available signing profiles in your AWS account.

Type annotations and code completion for `#!python session.create_client("signer").list_signing_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/list_signing_profiles.html)

```python
# list_signing_profiles method definition

await def list_signing_profiles(
    self,
    *,
    includeCanceled: bool = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    platformId: str = ...,
    statuses: Sequence[SigningProfileStatusType] = ...,  # (1)
) -> ListSigningProfilesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SigningProfileStatusType](./literals.md#signingprofilestatustype) 
2. See [:material-code-braces: ListSigningProfilesResponseTypeDef](./type_defs.md#listsigningprofilesresponsetypedef) 


```python
# list_signing_profiles method usage example with argument unpacking

kwargs: ListSigningProfilesRequestRequestTypeDef = {  # (1)
    "includeCanceled": ...,
}

parent.list_signing_profiles(**kwargs)
```

1. See [:material-code-braces: ListSigningProfilesRequestRequestTypeDef](./type_defs.md#listsigningprofilesrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of the tags associated with a signing profile resource.

Type annotations and code completion for `#!python session.create_client("signer").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/list_tags_for_resource.html)

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

### put\_signing\_profile

Creates a signing profile.

Type annotations and code completion for `#!python session.create_client("signer").put_signing_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/put_signing_profile.html)

```python
# put_signing_profile method definition

await def put_signing_profile(
    self,
    *,
    profileName: str,
    platformId: str,
    signingMaterial: SigningMaterialTypeDef = ...,  # (1)
    signatureValidityPeriod: SignatureValidityPeriodTypeDef = ...,  # (2)
    overrides: SigningPlatformOverridesTypeDef = ...,  # (3)
    signingParameters: Mapping[str, str] = ...,
    tags: Mapping[str, str] = ...,
) -> PutSigningProfileResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: SigningMaterialTypeDef](./type_defs.md#signingmaterialtypedef) 
2. See [:material-code-braces: SignatureValidityPeriodTypeDef](./type_defs.md#signaturevalidityperiodtypedef) 
3. See [:material-code-braces: SigningPlatformOverridesTypeDef](./type_defs.md#signingplatformoverridestypedef) 
4. See [:material-code-braces: PutSigningProfileResponseTypeDef](./type_defs.md#putsigningprofileresponsetypedef) 


```python
# put_signing_profile method usage example with argument unpacking

kwargs: PutSigningProfileRequestRequestTypeDef = {  # (1)
    "profileName": ...,
    "platformId": ...,
}

parent.put_signing_profile(**kwargs)
```

1. See [:material-code-braces: PutSigningProfileRequestRequestTypeDef](./type_defs.md#putsigningprofilerequestrequesttypedef) 

### remove\_profile\_permission

Removes cross-account permissions from a signing profile.

Type annotations and code completion for `#!python session.create_client("signer").remove_profile_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/remove_profile_permission.html)

```python
# remove_profile_permission method definition

await def remove_profile_permission(
    self,
    *,
    profileName: str,
    revisionId: str,
    statementId: str,
) -> RemoveProfilePermissionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RemoveProfilePermissionResponseTypeDef](./type_defs.md#removeprofilepermissionresponsetypedef) 


```python
# remove_profile_permission method usage example with argument unpacking

kwargs: RemoveProfilePermissionRequestRequestTypeDef = {  # (1)
    "profileName": ...,
    "revisionId": ...,
    "statementId": ...,
}

parent.remove_profile_permission(**kwargs)
```

1. See [:material-code-braces: RemoveProfilePermissionRequestRequestTypeDef](./type_defs.md#removeprofilepermissionrequestrequesttypedef) 

### revoke\_signature

Changes the state of a signing job to REVOKED.

Type annotations and code completion for `#!python session.create_client("signer").revoke_signature` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/revoke_signature.html)

```python
# revoke_signature method definition

await def revoke_signature(
    self,
    *,
    jobId: str,
    reason: str,
    jobOwner: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# revoke_signature method usage example with argument unpacking

kwargs: RevokeSignatureRequestRequestTypeDef = {  # (1)
    "jobId": ...,
    "reason": ...,
}

parent.revoke_signature(**kwargs)
```

1. See [:material-code-braces: RevokeSignatureRequestRequestTypeDef](./type_defs.md#revokesignaturerequestrequesttypedef) 

### revoke\_signing\_profile

Changes the state of a signing profile to REVOKED.

Type annotations and code completion for `#!python session.create_client("signer").revoke_signing_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/revoke_signing_profile.html)

```python
# revoke_signing_profile method definition

await def revoke_signing_profile(
    self,
    *,
    profileName: str,
    profileVersion: str,
    reason: str,
    effectiveTime: TimestampTypeDef,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# revoke_signing_profile method usage example with argument unpacking

kwargs: RevokeSigningProfileRequestRequestTypeDef = {  # (1)
    "profileName": ...,
    "profileVersion": ...,
    "reason": ...,
    "effectiveTime": ...,
}

parent.revoke_signing_profile(**kwargs)
```

1. See [:material-code-braces: RevokeSigningProfileRequestRequestTypeDef](./type_defs.md#revokesigningprofilerequestrequesttypedef) 

### sign\_payload

Signs a binary payload and returns a signature envelope.

Type annotations and code completion for `#!python session.create_client("signer").sign_payload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/sign_payload.html)

```python
# sign_payload method definition

await def sign_payload(
    self,
    *,
    profileName: str,
    payload: BlobTypeDef,
    payloadFormat: str,
    profileOwner: str = ...,
) -> SignPayloadResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SignPayloadResponseTypeDef](./type_defs.md#signpayloadresponsetypedef) 


```python
# sign_payload method usage example with argument unpacking

kwargs: SignPayloadRequestRequestTypeDef = {  # (1)
    "profileName": ...,
    "payload": ...,
    "payloadFormat": ...,
}

parent.sign_payload(**kwargs)
```

1. See [:material-code-braces: SignPayloadRequestRequestTypeDef](./type_defs.md#signpayloadrequestrequesttypedef) 

### start\_signing\_job

Initiates a signing job to be performed on the code provided.

Type annotations and code completion for `#!python session.create_client("signer").start_signing_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/start_signing_job.html)

```python
# start_signing_job method definition

await def start_signing_job(
    self,
    *,
    source: SourceTypeDef,  # (1)
    destination: DestinationTypeDef,  # (2)
    profileName: str,
    clientRequestToken: str,
    profileOwner: str = ...,
) -> StartSigningJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
3. See [:material-code-braces: StartSigningJobResponseTypeDef](./type_defs.md#startsigningjobresponsetypedef) 


```python
# start_signing_job method usage example with argument unpacking

kwargs: StartSigningJobRequestRequestTypeDef = {  # (1)
    "source": ...,
    "destination": ...,
    "profileName": ...,
    "clientRequestToken": ...,
}

parent.start_signing_job(**kwargs)
```

1. See [:material-code-braces: StartSigningJobRequestRequestTypeDef](./type_defs.md#startsigningjobrequestrequesttypedef) 

### tag\_resource

Adds one or more tags to a signing profile.

Type annotations and code completion for `#!python session.create_client("signer").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/tag_resource.html)

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

Removes one or more tags from a signing profile.

Type annotations and code completion for `#!python session.create_client("signer").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/client/untag_resource.html)

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

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("signer").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "SignerClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("signer").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client)

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

Type annotations and code completion for `#!python session.create_client("signer").get_paginator` method with overloads.

- `client.get_paginator("list_signing_jobs")` -> [ListSigningJobsPaginator](./paginators.md#listsigningjobspaginator)
- `client.get_paginator("list_signing_platforms")` -> [ListSigningPlatformsPaginator](./paginators.md#listsigningplatformspaginator)
- `client.get_paginator("list_signing_profiles")` -> [ListSigningProfilesPaginator](./paginators.md#listsigningprofilespaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("signer").get_waiter` method with overloads.

- `client.get_waiter("successful_signing_job")` -> [SuccessfulSigningJobWaiter](./waiters.md#successfulsigningjobwaiter)

