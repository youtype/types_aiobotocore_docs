<a id="ecrpublicclient-for-aiobotocore-ecrpublic-module"></a>

# ECRPublicClient for aiobotocore ECRPublic module

> [Index](..) > [ECRPublic](.) > ECRPublicClient

Auto-generated documentation for
[ECRPublic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
type annotations stubs module
[types-aiobotocore-ecr-public](https://pypi.org/project/types-aiobotocore-ecr-public/).

- [ECRPublicClient for aiobotocore ECRPublic module](#ecrpublicclient-for-aiobotocore-ecrpublic-module)
  - [ECRPublicClient](#ecrpublicclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [batch_check_layer_availability](#batch_check_layer_availability)
    - [batch_delete_image](#batch_delete_image)
    - [can_paginate](#can_paginate)
    - [complete_layer_upload](#complete_layer_upload)
    - [create_repository](#create_repository)
    - [delete_repository](#delete_repository)
    - [delete_repository_policy](#delete_repository_policy)
    - [describe_image_tags](#describe_image_tags)
    - [describe_images](#describe_images)
    - [describe_registries](#describe_registries)
    - [describe_repositories](#describe_repositories)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_authorization_token](#get_authorization_token)
    - [get_registry_catalog_data](#get_registry_catalog_data)
    - [get_repository_catalog_data](#get_repository_catalog_data)
    - [get_repository_policy](#get_repository_policy)
    - [initiate_layer_upload](#initiate_layer_upload)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [put_image](#put_image)
    - [put_registry_catalog_data](#put_registry_catalog_data)
    - [put_repository_catalog_data](#put_repository_catalog_data)
    - [set_repository_policy](#set_repository_policy)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [upload_layer_part](#upload_layer_part)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="ecrpublicclient"></a>

## ECRPublicClient

Type annotations for `session.create_client("ecr-public")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_ecr_public.client import ECRPublicClient

session = get_session()
async with session.create_client("ecr-public") as client:
    client: ECRPublicClient
```

Boto3 documentation:
[ECRPublic.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_ecr_public.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.EmptyUploadException`
- `Exceptions.ImageAlreadyExistsException`
- `Exceptions.ImageDigestDoesNotMatchException`
- `Exceptions.ImageNotFoundException`
- `Exceptions.ImageTagAlreadyExistsException`
- `Exceptions.InvalidLayerException`
- `Exceptions.InvalidLayerPartException`
- `Exceptions.InvalidParameterException`
- `Exceptions.InvalidTagParameterException`
- `Exceptions.LayerAlreadyExistsException`
- `Exceptions.LayerPartTooSmallException`
- `Exceptions.LayersNotFoundException`
- `Exceptions.LimitExceededException`
- `Exceptions.ReferencedImagesNotFoundException`
- `Exceptions.RegistryNotFoundException`
- `Exceptions.RepositoryAlreadyExistsException`
- `Exceptions.RepositoryNotEmptyException`
- `Exceptions.RepositoryNotFoundException`
- `Exceptions.RepositoryPolicyNotFoundException`
- `Exceptions.ServerException`
- `Exceptions.TooManyTagsException`
- `Exceptions.UnsupportedCommandException`
- `Exceptions.UploadNotFoundException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ECRPublicClient exceptions.

Type annotations for `session.create_client("ecr-public").exceptions` method.

Boto3 documentation:
[ECRPublic.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="batch_check_layer_availability"></a>

### batch_check_layer_availability

Checks the availability of one or more image layers within a repository in a
public registry.

Type annotations for
`session.create_client("ecr-public").batch_check_layer_availability` method.

Boto3 documentation:
[ECRPublic.Client.batch_check_layer_availability](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.batch_check_layer_availability)

Asynchronous method. Use `await batch_check_layer_availability(...)` for a
synchronous call.

Arguments mapping described in
[BatchCheckLayerAvailabilityRequestRequestTypeDef](./type_defs.md#batchchecklayeravailabilityrequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `layerDigests`: `Sequence`\[`str`\] *(required)*
- `registryId`: `str`

Returns a `Coroutine` for
[BatchCheckLayerAvailabilityResponseTypeDef](./type_defs.md#batchchecklayeravailabilityresponsetypedef).

<a id="batch_delete_image"></a>

### batch_delete_image

Deletes a list of specified images within a repository in a public registry.

Type annotations for `session.create_client("ecr-public").batch_delete_image`
method.

Boto3 documentation:
[ECRPublic.Client.batch_delete_image](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.batch_delete_image)

Asynchronous method. Use `await batch_delete_image(...)` for a synchronous
call.

Arguments mapping described in
[BatchDeleteImageRequestRequestTypeDef](./type_defs.md#batchdeleteimagerequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `imageIds`:
  `Sequence`\[[ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef)\]
  *(required)*
- `registryId`: `str`

Returns a `Coroutine` for
[BatchDeleteImageResponseTypeDef](./type_defs.md#batchdeleteimageresponsetypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("ecr-public").can_paginate` method.

Boto3 documentation:
[ECRPublic.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="complete_layer_upload"></a>

### complete_layer_upload

Informs Amazon ECR that the image layer upload has completed for a specified
public registry, repository name, and upload ID.

Type annotations for
`session.create_client("ecr-public").complete_layer_upload` method.

Boto3 documentation:
[ECRPublic.Client.complete_layer_upload](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.complete_layer_upload)

Asynchronous method. Use `await complete_layer_upload(...)` for a synchronous
call.

Arguments mapping described in
[CompleteLayerUploadRequestRequestTypeDef](./type_defs.md#completelayeruploadrequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `uploadId`: `str` *(required)*
- `layerDigests`: `Sequence`\[`str`\] *(required)*
- `registryId`: `str`

Returns a `Coroutine` for
[CompleteLayerUploadResponseTypeDef](./type_defs.md#completelayeruploadresponsetypedef).

<a id="create_repository"></a>

### create_repository

Creates a repository in a public registry.

Type annotations for `session.create_client("ecr-public").create_repository`
method.

Boto3 documentation:
[ECRPublic.Client.create_repository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.create_repository)

Asynchronous method. Use `await create_repository(...)` for a synchronous call.

Arguments mapping described in
[CreateRepositoryRequestRequestTypeDef](./type_defs.md#createrepositoryrequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `catalogData`:
  [RepositoryCatalogDataInputTypeDef](./type_defs.md#repositorycatalogdatainputtypedef)
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateRepositoryResponseTypeDef](./type_defs.md#createrepositoryresponsetypedef).

<a id="delete_repository"></a>

### delete_repository

Deletes a repository in a public registry.

Type annotations for `session.create_client("ecr-public").delete_repository`
method.

Boto3 documentation:
[ECRPublic.Client.delete_repository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.delete_repository)

Asynchronous method. Use `await delete_repository(...)` for a synchronous call.

Arguments mapping described in
[DeleteRepositoryRequestRequestTypeDef](./type_defs.md#deleterepositoryrequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`
- `force`: `bool`

Returns a `Coroutine` for
[DeleteRepositoryResponseTypeDef](./type_defs.md#deleterepositoryresponsetypedef).

<a id="delete_repository_policy"></a>

### delete_repository_policy

Deletes the repository policy associated with the specified repository.

Type annotations for
`session.create_client("ecr-public").delete_repository_policy` method.

Boto3 documentation:
[ECRPublic.Client.delete_repository_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.delete_repository_policy)

Asynchronous method. Use `await delete_repository_policy(...)` for a
synchronous call.

Arguments mapping described in
[DeleteRepositoryPolicyRequestRequestTypeDef](./type_defs.md#deleterepositorypolicyrequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`

Returns a `Coroutine` for
[DeleteRepositoryPolicyResponseTypeDef](./type_defs.md#deleterepositorypolicyresponsetypedef).

<a id="describe_image_tags"></a>

### describe_image_tags

Returns the image tag details for a repository in a public registry.

Type annotations for `session.create_client("ecr-public").describe_image_tags`
method.

Boto3 documentation:
[ECRPublic.Client.describe_image_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.describe_image_tags)

Asynchronous method. Use `await describe_image_tags(...)` for a synchronous
call.

Arguments mapping described in
[DescribeImageTagsRequestRequestTypeDef](./type_defs.md#describeimagetagsrequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[DescribeImageTagsResponseTypeDef](./type_defs.md#describeimagetagsresponsetypedef).

<a id="describe_images"></a>

### describe_images

Returns metadata about the images in a repository in a public registry.

Type annotations for `session.create_client("ecr-public").describe_images`
method.

Boto3 documentation:
[ECRPublic.Client.describe_images](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.describe_images)

Asynchronous method. Use `await describe_images(...)` for a synchronous call.

Arguments mapping described in
[DescribeImagesRequestRequestTypeDef](./type_defs.md#describeimagesrequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`
- `imageIds`:
  `Sequence`\[[ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef)\]
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[DescribeImagesResponseTypeDef](./type_defs.md#describeimagesresponsetypedef).

<a id="describe_registries"></a>

### describe_registries

Returns details for a public registry.

Type annotations for `session.create_client("ecr-public").describe_registries`
method.

Boto3 documentation:
[ECRPublic.Client.describe_registries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.describe_registries)

Asynchronous method. Use `await describe_registries(...)` for a synchronous
call.

Arguments mapping described in
[DescribeRegistriesRequestRequestTypeDef](./type_defs.md#describeregistriesrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[DescribeRegistriesResponseTypeDef](./type_defs.md#describeregistriesresponsetypedef).

<a id="describe_repositories"></a>

### describe_repositories

Describes repositories in a public registry.

Type annotations for
`session.create_client("ecr-public").describe_repositories` method.

Boto3 documentation:
[ECRPublic.Client.describe_repositories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.describe_repositories)

Asynchronous method. Use `await describe_repositories(...)` for a synchronous
call.

Arguments mapping described in
[DescribeRepositoriesRequestRequestTypeDef](./type_defs.md#describerepositoriesrequestrequesttypedef).

Keyword-only arguments:

- `registryId`: `str`
- `repositoryNames`: `Sequence`\[`str`\]
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[DescribeRepositoriesResponseTypeDef](./type_defs.md#describerepositoriesresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("ecr-public").generate_presigned_url` method.

Boto3 documentation:
[ECRPublic.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_authorization_token"></a>

### get_authorization_token

Retrieves an authorization token.

Type annotations for
`session.create_client("ecr-public").get_authorization_token` method.

Boto3 documentation:
[ECRPublic.Client.get_authorization_token](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.get_authorization_token)

Asynchronous method. Use `await get_authorization_token(...)` for a synchronous
call.

Returns a `Coroutine` for
[GetAuthorizationTokenResponseTypeDef](./type_defs.md#getauthorizationtokenresponsetypedef).

<a id="get_registry_catalog_data"></a>

### get_registry_catalog_data

Retrieves catalog metadata for a public registry.

Type annotations for
`session.create_client("ecr-public").get_registry_catalog_data` method.

Boto3 documentation:
[ECRPublic.Client.get_registry_catalog_data](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.get_registry_catalog_data)

Asynchronous method. Use `await get_registry_catalog_data(...)` for a
synchronous call.

Returns a `Coroutine` for
[GetRegistryCatalogDataResponseTypeDef](./type_defs.md#getregistrycatalogdataresponsetypedef).

<a id="get_repository_catalog_data"></a>

### get_repository_catalog_data

Retrieve catalog metadata for a repository in a public registry.

Type annotations for
`session.create_client("ecr-public").get_repository_catalog_data` method.

Boto3 documentation:
[ECRPublic.Client.get_repository_catalog_data](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.get_repository_catalog_data)

Asynchronous method. Use `await get_repository_catalog_data(...)` for a
synchronous call.

Arguments mapping described in
[GetRepositoryCatalogDataRequestRequestTypeDef](./type_defs.md#getrepositorycatalogdatarequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`

Returns a `Coroutine` for
[GetRepositoryCatalogDataResponseTypeDef](./type_defs.md#getrepositorycatalogdataresponsetypedef).

<a id="get_repository_policy"></a>

### get_repository_policy

Retrieves the repository policy for the specified repository.

Type annotations for
`session.create_client("ecr-public").get_repository_policy` method.

Boto3 documentation:
[ECRPublic.Client.get_repository_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.get_repository_policy)

Asynchronous method. Use `await get_repository_policy(...)` for a synchronous
call.

Arguments mapping described in
[GetRepositoryPolicyRequestRequestTypeDef](./type_defs.md#getrepositorypolicyrequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`

Returns a `Coroutine` for
[GetRepositoryPolicyResponseTypeDef](./type_defs.md#getrepositorypolicyresponsetypedef).

<a id="initiate_layer_upload"></a>

### initiate_layer_upload

Notifies Amazon ECR that you intend to upload an image layer.

Type annotations for
`session.create_client("ecr-public").initiate_layer_upload` method.

Boto3 documentation:
[ECRPublic.Client.initiate_layer_upload](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.initiate_layer_upload)

Asynchronous method. Use `await initiate_layer_upload(...)` for a synchronous
call.

Arguments mapping described in
[InitiateLayerUploadRequestRequestTypeDef](./type_defs.md#initiatelayeruploadrequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`

Returns a `Coroutine` for
[InitiateLayerUploadResponseTypeDef](./type_defs.md#initiatelayeruploadresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

List the tags for an Amazon ECR Public resource.

Type annotations for
`session.create_client("ecr-public").list_tags_for_resource` method.

Boto3 documentation:
[ECRPublic.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="put_image"></a>

### put_image

Creates or updates the image manifest and tags associated with an image.

Type annotations for `session.create_client("ecr-public").put_image` method.

Boto3 documentation:
[ECRPublic.Client.put_image](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.put_image)

Asynchronous method. Use `await put_image(...)` for a synchronous call.

Arguments mapping described in
[PutImageRequestRequestTypeDef](./type_defs.md#putimagerequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `imageManifest`: `str` *(required)*
- `registryId`: `str`
- `imageManifestMediaType`: `str`
- `imageTag`: `str`
- `imageDigest`: `str`

Returns a `Coroutine` for
[PutImageResponseTypeDef](./type_defs.md#putimageresponsetypedef).

<a id="put_registry_catalog_data"></a>

### put_registry_catalog_data

Create or updates the catalog data for a public registry.

Type annotations for
`session.create_client("ecr-public").put_registry_catalog_data` method.

Boto3 documentation:
[ECRPublic.Client.put_registry_catalog_data](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.put_registry_catalog_data)

Asynchronous method. Use `await put_registry_catalog_data(...)` for a
synchronous call.

Arguments mapping described in
[PutRegistryCatalogDataRequestRequestTypeDef](./type_defs.md#putregistrycatalogdatarequestrequesttypedef).

Keyword-only arguments:

- `displayName`: `str`

Returns a `Coroutine` for
[PutRegistryCatalogDataResponseTypeDef](./type_defs.md#putregistrycatalogdataresponsetypedef).

<a id="put_repository_catalog_data"></a>

### put_repository_catalog_data

Creates or updates the catalog data for a repository in a public registry.

Type annotations for
`session.create_client("ecr-public").put_repository_catalog_data` method.

Boto3 documentation:
[ECRPublic.Client.put_repository_catalog_data](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.put_repository_catalog_data)

Asynchronous method. Use `await put_repository_catalog_data(...)` for a
synchronous call.

Arguments mapping described in
[PutRepositoryCatalogDataRequestRequestTypeDef](./type_defs.md#putrepositorycatalogdatarequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `catalogData`:
  [RepositoryCatalogDataInputTypeDef](./type_defs.md#repositorycatalogdatainputtypedef)
  *(required)*
- `registryId`: `str`

Returns a `Coroutine` for
[PutRepositoryCatalogDataResponseTypeDef](./type_defs.md#putrepositorycatalogdataresponsetypedef).

<a id="set_repository_policy"></a>

### set_repository_policy

Applies a repository policy to the specified public repository to control
access permissions.

Type annotations for
`session.create_client("ecr-public").set_repository_policy` method.

Boto3 documentation:
[ECRPublic.Client.set_repository_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.set_repository_policy)

Asynchronous method. Use `await set_repository_policy(...)` for a synchronous
call.

Arguments mapping described in
[SetRepositoryPolicyRequestRequestTypeDef](./type_defs.md#setrepositorypolicyrequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `policyText`: `str` *(required)*
- `registryId`: `str`
- `force`: `bool`

Returns a `Coroutine` for
[SetRepositoryPolicyResponseTypeDef](./type_defs.md#setrepositorypolicyresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Associates the specified tags to a resource with the specified `resourceArn`.

Type annotations for `session.create_client("ecr-public").tag_resource` method.

Boto3 documentation:
[ECRPublic.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Deletes specified tags from a resource.

Type annotations for `session.create_client("ecr-public").untag_resource`
method.

Boto3 documentation:
[ECRPublic.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="upload_layer_part"></a>

### upload_layer_part

Uploads an image layer part to Amazon ECR.

Type annotations for `session.create_client("ecr-public").upload_layer_part`
method.

Boto3 documentation:
[ECRPublic.Client.upload_layer_part](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.upload_layer_part)

Asynchronous method. Use `await upload_layer_part(...)` for a synchronous call.

Arguments mapping described in
[UploadLayerPartRequestRequestTypeDef](./type_defs.md#uploadlayerpartrequestrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `uploadId`: `str` *(required)*
- `partFirstByte`: `int` *(required)*
- `partLastByte`: `int` *(required)*
- `layerPartBlob`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]
  *(required)*
- `registryId`: `str`

Returns a `Coroutine` for
[UploadLayerPartResponseTypeDef](./type_defs.md#uploadlayerpartresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("ecr-public").__aenter__` method.

Boto3 documentation:
[ECRPublic.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [ECRPublicClient](#ecrpublicclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("ecr-public").__aexit__` method.

Boto3 documentation:
[ECRPublic.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("ecr-public").get_paginator` method
with overloads.

- `client.get_paginator("describe_image_tags")` ->
  [DescribeImageTagsPaginator](./paginators.md#describeimagetagspaginator)
- `client.get_paginator("describe_images")` ->
  [DescribeImagesPaginator](./paginators.md#describeimagespaginator)
- `client.get_paginator("describe_registries")` ->
  [DescribeRegistriesPaginator](./paginators.md#describeregistriespaginator)
- `client.get_paginator("describe_repositories")` ->
  [DescribeRepositoriesPaginator](./paginators.md#describerepositoriespaginator)
