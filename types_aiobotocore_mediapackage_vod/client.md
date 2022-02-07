<a id="mediapackagevodclient-for-aiobotocore-mediapackagevod-module"></a>

# MediaPackageVodClient for aiobotocore MediaPackageVod module

> [Index](..) > [MediaPackageVod](.) > MediaPackageVodClient

Auto-generated documentation for
[MediaPackageVod](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
type annotations stubs module
[types-aiobotocore-mediapackage-vod](https://pypi.org/project/types-aiobotocore-mediapackage-vod/).

- [MediaPackageVodClient for aiobotocore MediaPackageVod module](#mediapackagevodclient-for-aiobotocore-mediapackagevod-module)
  - [MediaPackageVodClient](#mediapackagevodclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [configure_logs](#configure_logs)
    - [create_asset](#create_asset)
    - [create_packaging_configuration](#create_packaging_configuration)
    - [create_packaging_group](#create_packaging_group)
    - [delete_asset](#delete_asset)
    - [delete_packaging_configuration](#delete_packaging_configuration)
    - [delete_packaging_group](#delete_packaging_group)
    - [describe_asset](#describe_asset)
    - [describe_packaging_configuration](#describe_packaging_configuration)
    - [describe_packaging_group](#describe_packaging_group)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_assets](#list_assets)
    - [list_packaging_configurations](#list_packaging_configurations)
    - [list_packaging_groups](#list_packaging_groups)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_packaging_group](#update_packaging_group)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="mediapackagevodclient"></a>

## MediaPackageVodClient

Type annotations for `session.create_client("mediapackage-vod")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_mediapackage_vod.client import MediaPackageVodClient

session = get_session()
async with session.create_client("mediapackage-vod") as client:
    client: MediaPackageVodClient
```

Boto3 documentation:
[MediaPackageVod.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_mediapackage_vod.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ForbiddenException`
- `Exceptions.InternalServerErrorException`
- `Exceptions.NotFoundException`
- `Exceptions.ServiceUnavailableException`
- `Exceptions.TooManyRequestsException`
- `Exceptions.UnprocessableEntityException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

MediaPackageVodClient exceptions.

Type annotations for `session.create_client("mediapackage-vod").exceptions`
method.

Boto3 documentation:
[MediaPackageVod.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("mediapackage-vod").can_paginate`
method.

Boto3 documentation:
[MediaPackageVod.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="configure_logs"></a>

### configure_logs

Changes the packaging group's properities to configure log subscription See
also: \[AWS API
Documentation\](https://docs.aws.amazon.com/goto/WebAPI/mediapackage-
vod-2018-11-07/ConfigureLogs).

Type annotations for `session.create_client("mediapackage-vod").configure_logs`
method.

Boto3 documentation:
[MediaPackageVod.Client.configure_logs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.configure_logs)

Asynchronous method. Use `await configure_logs(...)` for a synchronous call.

Arguments mapping described in
[ConfigureLogsRequestRequestTypeDef](./type_defs.md#configurelogsrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `EgressAccessLogs`:
  [EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef)

Returns a `Coroutine` for
[ConfigureLogsResponseTypeDef](./type_defs.md#configurelogsresponsetypedef).

<a id="create_asset"></a>

### create_asset

Creates a new MediaPackage VOD Asset resource.

Type annotations for `session.create_client("mediapackage-vod").create_asset`
method.

Boto3 documentation:
[MediaPackageVod.Client.create_asset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_asset)

Asynchronous method. Use `await create_asset(...)` for a synchronous call.

Arguments mapping described in
[CreateAssetRequestRequestTypeDef](./type_defs.md#createassetrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `PackagingGroupId`: `str` *(required)*
- `SourceArn`: `str` *(required)*
- `SourceRoleArn`: `str` *(required)*
- `ResourceId`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateAssetResponseTypeDef](./type_defs.md#createassetresponsetypedef).

<a id="create_packaging_configuration"></a>

### create_packaging_configuration

Creates a new MediaPackage VOD PackagingConfiguration resource.

Type annotations for
`session.create_client("mediapackage-vod").create_packaging_configuration`
method.

Boto3 documentation:
[MediaPackageVod.Client.create_packaging_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_packaging_configuration)

Asynchronous method. Use `await create_packaging_configuration(...)` for a
synchronous call.

Arguments mapping described in
[CreatePackagingConfigurationRequestRequestTypeDef](./type_defs.md#createpackagingconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `PackagingGroupId`: `str` *(required)*
- `CmafPackage`: [CmafPackageTypeDef](./type_defs.md#cmafpackagetypedef)
- `DashPackage`: [DashPackageTypeDef](./type_defs.md#dashpackagetypedef)
- `HlsPackage`: [HlsPackageTypeDef](./type_defs.md#hlspackagetypedef)
- `MssPackage`: [MssPackageTypeDef](./type_defs.md#msspackagetypedef)
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreatePackagingConfigurationResponseTypeDef](./type_defs.md#createpackagingconfigurationresponsetypedef).

<a id="create_packaging_group"></a>

### create_packaging_group

Creates a new MediaPackage VOD PackagingGroup resource.

Type annotations for
`session.create_client("mediapackage-vod").create_packaging_group` method.

Boto3 documentation:
[MediaPackageVod.Client.create_packaging_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_packaging_group)

Asynchronous method. Use `await create_packaging_group(...)` for a synchronous
call.

Arguments mapping described in
[CreatePackagingGroupRequestRequestTypeDef](./type_defs.md#createpackaginggrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Authorization`: [AuthorizationTypeDef](./type_defs.md#authorizationtypedef)
- `EgressAccessLogs`:
  [EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef)
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreatePackagingGroupResponseTypeDef](./type_defs.md#createpackaginggroupresponsetypedef).

<a id="delete_asset"></a>

### delete_asset

Deletes an existing MediaPackage VOD Asset resource.

Type annotations for `session.create_client("mediapackage-vod").delete_asset`
method.

Boto3 documentation:
[MediaPackageVod.Client.delete_asset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.delete_asset)

Asynchronous method. Use `await delete_asset(...)` for a synchronous call.

Arguments mapping described in
[DeleteAssetRequestRequestTypeDef](./type_defs.md#deleteassetrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_packaging_configuration"></a>

### delete_packaging_configuration

Deletes a MediaPackage VOD PackagingConfiguration resource.

Type annotations for
`session.create_client("mediapackage-vod").delete_packaging_configuration`
method.

Boto3 documentation:
[MediaPackageVod.Client.delete_packaging_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.delete_packaging_configuration)

Asynchronous method. Use `await delete_packaging_configuration(...)` for a
synchronous call.

Arguments mapping described in
[DeletePackagingConfigurationRequestRequestTypeDef](./type_defs.md#deletepackagingconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_packaging_group"></a>

### delete_packaging_group

Deletes a MediaPackage VOD PackagingGroup resource.

Type annotations for
`session.create_client("mediapackage-vod").delete_packaging_group` method.

Boto3 documentation:
[MediaPackageVod.Client.delete_packaging_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.delete_packaging_group)

Asynchronous method. Use `await delete_packaging_group(...)` for a synchronous
call.

Arguments mapping described in
[DeletePackagingGroupRequestRequestTypeDef](./type_defs.md#deletepackaginggrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_asset"></a>

### describe_asset

Returns a description of a MediaPackage VOD Asset resource.

Type annotations for `session.create_client("mediapackage-vod").describe_asset`
method.

Boto3 documentation:
[MediaPackageVod.Client.describe_asset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.describe_asset)

Asynchronous method. Use `await describe_asset(...)` for a synchronous call.

Arguments mapping described in
[DescribeAssetRequestRequestTypeDef](./type_defs.md#describeassetrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAssetResponseTypeDef](./type_defs.md#describeassetresponsetypedef).

<a id="describe_packaging_configuration"></a>

### describe_packaging_configuration

Returns a description of a MediaPackage VOD PackagingConfiguration resource.

Type annotations for
`session.create_client("mediapackage-vod").describe_packaging_configuration`
method.

Boto3 documentation:
[MediaPackageVod.Client.describe_packaging_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.describe_packaging_configuration)

Asynchronous method. Use `await describe_packaging_configuration(...)` for a
synchronous call.

Arguments mapping described in
[DescribePackagingConfigurationRequestRequestTypeDef](./type_defs.md#describepackagingconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[DescribePackagingConfigurationResponseTypeDef](./type_defs.md#describepackagingconfigurationresponsetypedef).

<a id="describe_packaging_group"></a>

### describe_packaging_group

Returns a description of a MediaPackage VOD PackagingGroup resource.

Type annotations for
`session.create_client("mediapackage-vod").describe_packaging_group` method.

Boto3 documentation:
[MediaPackageVod.Client.describe_packaging_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.describe_packaging_group)

Asynchronous method. Use `await describe_packaging_group(...)` for a
synchronous call.

Arguments mapping described in
[DescribePackagingGroupRequestRequestTypeDef](./type_defs.md#describepackaginggrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[DescribePackagingGroupResponseTypeDef](./type_defs.md#describepackaginggroupresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("mediapackage-vod").generate_presigned_url` method.

Boto3 documentation:
[MediaPackageVod.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_assets"></a>

### list_assets

Returns a collection of MediaPackage VOD Asset resources.

Type annotations for `session.create_client("mediapackage-vod").list_assets`
method.

Boto3 documentation:
[MediaPackageVod.Client.list_assets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.list_assets)

Asynchronous method. Use `await list_assets(...)` for a synchronous call.

Arguments mapping described in
[ListAssetsRequestRequestTypeDef](./type_defs.md#listassetsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`
- `PackagingGroupId`: `str`

Returns a `Coroutine` for
[ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef).

<a id="list_packaging_configurations"></a>

### list_packaging_configurations

Returns a collection of MediaPackage VOD PackagingConfiguration resources.

Type annotations for
`session.create_client("mediapackage-vod").list_packaging_configurations`
method.

Boto3 documentation:
[MediaPackageVod.Client.list_packaging_configurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.list_packaging_configurations)

Asynchronous method. Use `await list_packaging_configurations(...)` for a
synchronous call.

Arguments mapping described in
[ListPackagingConfigurationsRequestRequestTypeDef](./type_defs.md#listpackagingconfigurationsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`
- `PackagingGroupId`: `str`

Returns a `Coroutine` for
[ListPackagingConfigurationsResponseTypeDef](./type_defs.md#listpackagingconfigurationsresponsetypedef).

<a id="list_packaging_groups"></a>

### list_packaging_groups

Returns a collection of MediaPackage VOD PackagingGroup resources.

Type annotations for
`session.create_client("mediapackage-vod").list_packaging_groups` method.

Boto3 documentation:
[MediaPackageVod.Client.list_packaging_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.list_packaging_groups)

Asynchronous method. Use `await list_packaging_groups(...)` for a synchronous
call.

Arguments mapping described in
[ListPackagingGroupsRequestRequestTypeDef](./type_defs.md#listpackaginggroupsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListPackagingGroupsResponseTypeDef](./type_defs.md#listpackaginggroupsresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Returns a list of the tags assigned to the specified resource.

Type annotations for
`session.create_client("mediapackage-vod").list_tags_for_resource` method.

Boto3 documentation:
[MediaPackageVod.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Adds tags to the specified resource.

Type annotations for `session.create_client("mediapackage-vod").tag_resource`
method.

Boto3 documentation:
[MediaPackageVod.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

<a id="untag_resource"></a>

### untag_resource

Removes tags from the specified resource.

Type annotations for `session.create_client("mediapackage-vod").untag_resource`
method.

Boto3 documentation:
[MediaPackageVod.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

<a id="update_packaging_group"></a>

### update_packaging_group

Updates a specific packaging group.

Type annotations for
`session.create_client("mediapackage-vod").update_packaging_group` method.

Boto3 documentation:
[MediaPackageVod.Client.update_packaging_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.update_packaging_group)

Asynchronous method. Use `await update_packaging_group(...)` for a synchronous
call.

Arguments mapping described in
[UpdatePackagingGroupRequestRequestTypeDef](./type_defs.md#updatepackaginggrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Authorization`: [AuthorizationTypeDef](./type_defs.md#authorizationtypedef)

Returns a `Coroutine` for
[UpdatePackagingGroupResponseTypeDef](./type_defs.md#updatepackaginggroupresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("mediapackage-vod").__aenter__`
method.

Boto3 documentation:
[MediaPackageVod.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [MediaPackageVodClient](#mediapackagevodclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("mediapackage-vod").__aexit__`
method.

Boto3 documentation:
[MediaPackageVod.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("mediapackage-vod").get_paginator`
method with overloads.

- `client.get_paginator("list_assets")` ->
  [ListAssetsPaginator](./paginators.md#listassetspaginator)
- `client.get_paginator("list_packaging_configurations")` ->
  [ListPackagingConfigurationsPaginator](./paginators.md#listpackagingconfigurationspaginator)
- `client.get_paginator("list_packaging_groups")` ->
  [ListPackagingGroupsPaginator](./paginators.md#listpackaginggroupspaginator)
