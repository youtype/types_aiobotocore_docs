<a id="mediapackageclient-for-aiobotocore-mediapackage-module"></a>

# MediaPackageClient for aiobotocore MediaPackage module

> [Index](..) > [MediaPackage](.) > MediaPackageClient

Auto-generated documentation for
[MediaPackage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
type annotations stubs module
[types-aiobotocore-mediapackage](https://pypi.org/project/types-aiobotocore-mediapackage/).

- [MediaPackageClient for aiobotocore MediaPackage module](#mediapackageclient-for-aiobotocore-mediapackage-module)
  - [MediaPackageClient](#mediapackageclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [configure_logs](#configure_logs)
    - [create_channel](#create_channel)
    - [create_harvest_job](#create_harvest_job)
    - [create_origin_endpoint](#create_origin_endpoint)
    - [delete_channel](#delete_channel)
    - [delete_origin_endpoint](#delete_origin_endpoint)
    - [describe_channel](#describe_channel)
    - [describe_harvest_job](#describe_harvest_job)
    - [describe_origin_endpoint](#describe_origin_endpoint)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_channels](#list_channels)
    - [list_harvest_jobs](#list_harvest_jobs)
    - [list_origin_endpoints](#list_origin_endpoints)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [rotate_channel_credentials](#rotate_channel_credentials)
    - [rotate_ingest_endpoint_credentials](#rotate_ingest_endpoint_credentials)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_channel](#update_channel)
    - [update_origin_endpoint](#update_origin_endpoint)
    - [get_paginator](#get_paginator)

<a id="mediapackageclient"></a>

## MediaPackageClient

Type annotations for `aiobotocore.create_client("mediapackage")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_mediapackage.client import MediaPackageClient

def get_mediapackage_client() -> MediaPackageClient:
    return Session().client("mediapackage")
```

Boto3 documentation:
[MediaPackage.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_mediapackage.client import Exceptions

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

MediaPackageClient exceptions.

Type annotations for `aiobotocore.create_client("mediapackage").exceptions`
method.

Boto3 documentation:
[MediaPackage.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("mediapackage").can_paginate`
method.

Boto3 documentation:
[MediaPackage.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="configure_logs"></a>

### configure_logs

Changes the Channel's properities to configure log subscription See also:
[AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediapackage-2017-10-12/ConfigureLogs).

Type annotations for `aiobotocore.create_client("mediapackage").configure_logs`
method.

Boto3 documentation:
[MediaPackage.Client.configure_logs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.configure_logs)

Asynchronous method. Use `await configure_logs(...)` for a synchronous call.

Arguments mapping described in
[ConfigureLogsRequestRequestTypeDef](./type_defs.md#configurelogsrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `EgressAccessLogs`:
  [EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef)
- `IngressAccessLogs`:
  [IngressAccessLogsTypeDef](./type_defs.md#ingressaccesslogstypedef)

Returns a `Coroutine` for
[ConfigureLogsResponseTypeDef](./type_defs.md#configurelogsresponsetypedef).

<a id="create_channel"></a>

### create_channel

Creates a new Channel.

Type annotations for `aiobotocore.create_client("mediapackage").create_channel`
method.

Boto3 documentation:
[MediaPackage.Client.create_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.create_channel)

Asynchronous method. Use `await create_channel(...)` for a synchronous call.

Arguments mapping described in
[CreateChannelRequestRequestTypeDef](./type_defs.md#createchannelrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Description`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef).

<a id="create_harvest_job"></a>

### create_harvest_job

Creates a new HarvestJob record.

Type annotations for
`aiobotocore.create_client("mediapackage").create_harvest_job` method.

Boto3 documentation:
[MediaPackage.Client.create_harvest_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.create_harvest_job)

Asynchronous method. Use `await create_harvest_job(...)` for a synchronous
call.

Arguments mapping described in
[CreateHarvestJobRequestRequestTypeDef](./type_defs.md#createharvestjobrequestrequesttypedef).

Keyword-only arguments:

- `EndTime`: `str` *(required)*
- `Id`: `str` *(required)*
- `OriginEndpointId`: `str` *(required)*
- `S3Destination`: [S3DestinationTypeDef](./type_defs.md#s3destinationtypedef)
  *(required)*
- `StartTime`: `str` *(required)*

Returns a `Coroutine` for
[CreateHarvestJobResponseTypeDef](./type_defs.md#createharvestjobresponsetypedef).

<a id="create_origin_endpoint"></a>

### create_origin_endpoint

Creates a new OriginEndpoint record.

Type annotations for
`aiobotocore.create_client("mediapackage").create_origin_endpoint` method.

Boto3 documentation:
[MediaPackage.Client.create_origin_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.create_origin_endpoint)

Asynchronous method. Use `await create_origin_endpoint(...)` for a synchronous
call.

Arguments mapping described in
[CreateOriginEndpointRequestRequestTypeDef](./type_defs.md#createoriginendpointrequestrequesttypedef).

Keyword-only arguments:

- `ChannelId`: `str` *(required)*
- `Id`: `str` *(required)*
- `Authorization`: [AuthorizationTypeDef](./type_defs.md#authorizationtypedef)
- `CmafPackage`:
  [CmafPackageCreateOrUpdateParametersTypeDef](./type_defs.md#cmafpackagecreateorupdateparameterstypedef)
- `DashPackage`: [DashPackageTypeDef](./type_defs.md#dashpackagetypedef)
- `Description`: `str`
- `HlsPackage`: [HlsPackageTypeDef](./type_defs.md#hlspackagetypedef)
- `ManifestName`: `str`
- `MssPackage`: [MssPackageTypeDef](./type_defs.md#msspackagetypedef)
- `Origination`: [OriginationType](./literals.md#originationtype)
- `StartoverWindowSeconds`: `int`
- `Tags`: `Mapping`\[`str`, `str`\]
- `TimeDelaySeconds`: `int`
- `Whitelist`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[CreateOriginEndpointResponseTypeDef](./type_defs.md#createoriginendpointresponsetypedef).

<a id="delete_channel"></a>

### delete_channel

Deletes an existing Channel.

Type annotations for `aiobotocore.create_client("mediapackage").delete_channel`
method.

Boto3 documentation:
[MediaPackage.Client.delete_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.delete_channel)

Asynchronous method. Use `await delete_channel(...)` for a synchronous call.

Arguments mapping described in
[DeleteChannelRequestRequestTypeDef](./type_defs.md#deletechannelrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_origin_endpoint"></a>

### delete_origin_endpoint

Deletes an existing OriginEndpoint.

Type annotations for
`aiobotocore.create_client("mediapackage").delete_origin_endpoint` method.

Boto3 documentation:
[MediaPackage.Client.delete_origin_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.delete_origin_endpoint)

Asynchronous method. Use `await delete_origin_endpoint(...)` for a synchronous
call.

Arguments mapping described in
[DeleteOriginEndpointRequestRequestTypeDef](./type_defs.md#deleteoriginendpointrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_channel"></a>

### describe_channel

Gets details about a Channel.

Type annotations for
`aiobotocore.create_client("mediapackage").describe_channel` method.

Boto3 documentation:
[MediaPackage.Client.describe_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.describe_channel)

Asynchronous method. Use `await describe_channel(...)` for a synchronous call.

Arguments mapping described in
[DescribeChannelRequestRequestTypeDef](./type_defs.md#describechannelrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[DescribeChannelResponseTypeDef](./type_defs.md#describechannelresponsetypedef).

<a id="describe_harvest_job"></a>

### describe_harvest_job

Gets details about an existing HarvestJob.

Type annotations for
`aiobotocore.create_client("mediapackage").describe_harvest_job` method.

Boto3 documentation:
[MediaPackage.Client.describe_harvest_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.describe_harvest_job)

Asynchronous method. Use `await describe_harvest_job(...)` for a synchronous
call.

Arguments mapping described in
[DescribeHarvestJobRequestRequestTypeDef](./type_defs.md#describeharvestjobrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[DescribeHarvestJobResponseTypeDef](./type_defs.md#describeharvestjobresponsetypedef).

<a id="describe_origin_endpoint"></a>

### describe_origin_endpoint

Gets details about an existing OriginEndpoint.

Type annotations for
`aiobotocore.create_client("mediapackage").describe_origin_endpoint` method.

Boto3 documentation:
[MediaPackage.Client.describe_origin_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.describe_origin_endpoint)

Asynchronous method. Use `await describe_origin_endpoint(...)` for a
synchronous call.

Arguments mapping described in
[DescribeOriginEndpointRequestRequestTypeDef](./type_defs.md#describeoriginendpointrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[DescribeOriginEndpointResponseTypeDef](./type_defs.md#describeoriginendpointresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("mediapackage").generate_presigned_url` method.

Boto3 documentation:
[MediaPackage.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_channels"></a>

### list_channels

Returns a collection of Channels.

Type annotations for `aiobotocore.create_client("mediapackage").list_channels`
method.

Boto3 documentation:
[MediaPackage.Client.list_channels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.list_channels)

Asynchronous method. Use `await list_channels(...)` for a synchronous call.

Arguments mapping described in
[ListChannelsRequestRequestTypeDef](./type_defs.md#listchannelsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef).

<a id="list_harvest_jobs"></a>

### list_harvest_jobs

Returns a collection of HarvestJob records.

Type annotations for
`aiobotocore.create_client("mediapackage").list_harvest_jobs` method.

Boto3 documentation:
[MediaPackage.Client.list_harvest_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.list_harvest_jobs)

Asynchronous method. Use `await list_harvest_jobs(...)` for a synchronous call.

Arguments mapping described in
[ListHarvestJobsRequestRequestTypeDef](./type_defs.md#listharvestjobsrequestrequesttypedef).

Keyword-only arguments:

- `IncludeChannelId`: `str`
- `IncludeStatus`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListHarvestJobsResponseTypeDef](./type_defs.md#listharvestjobsresponsetypedef).

<a id="list_origin_endpoints"></a>

### list_origin_endpoints

Returns a collection of OriginEndpoint records.

Type annotations for
`aiobotocore.create_client("mediapackage").list_origin_endpoints` method.

Boto3 documentation:
[MediaPackage.Client.list_origin_endpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.list_origin_endpoints)

Asynchronous method. Use `await list_origin_endpoints(...)` for a synchronous
call.

Arguments mapping described in
[ListOriginEndpointsRequestRequestTypeDef](./type_defs.md#listoriginendpointsrequestrequesttypedef).

Keyword-only arguments:

- `ChannelId`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListOriginEndpointsResponseTypeDef](./type_defs.md#listoriginendpointsresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

See also:
[AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediapackage-2017-10-12/ListTagsForResource).

Type annotations for
`aiobotocore.create_client("mediapackage").list_tags_for_resource` method.

Boto3 documentation:
[MediaPackage.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="rotate_channel_credentials"></a>

### rotate_channel_credentials

Changes the Channel's first IngestEndpoint's username and password.

Type annotations for
`aiobotocore.create_client("mediapackage").rotate_channel_credentials` method.

Boto3 documentation:
[MediaPackage.Client.rotate_channel_credentials](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.rotate_channel_credentials)

Asynchronous method. Use `await rotate_channel_credentials(...)` for a
synchronous call.

Arguments mapping described in
[RotateChannelCredentialsRequestRequestTypeDef](./type_defs.md#rotatechannelcredentialsrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[RotateChannelCredentialsResponseTypeDef](./type_defs.md#rotatechannelcredentialsresponsetypedef).

<a id="rotate_ingest_endpoint_credentials"></a>

### rotate_ingest_endpoint_credentials

Rotate the IngestEndpoint's username and password, as specified by the
IngestEndpoint's id.

Type annotations for
`aiobotocore.create_client("mediapackage").rotate_ingest_endpoint_credentials`
method.

Boto3 documentation:
[MediaPackage.Client.rotate_ingest_endpoint_credentials](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.rotate_ingest_endpoint_credentials)

Asynchronous method. Use `await rotate_ingest_endpoint_credentials(...)` for a
synchronous call.

Arguments mapping described in
[RotateIngestEndpointCredentialsRequestRequestTypeDef](./type_defs.md#rotateingestendpointcredentialsrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `IngestEndpointId`: `str` *(required)*

Returns a `Coroutine` for
[RotateIngestEndpointCredentialsResponseTypeDef](./type_defs.md#rotateingestendpointcredentialsresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

See also:
[AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediapackage-2017-10-12/TagResource).

Type annotations for `aiobotocore.create_client("mediapackage").tag_resource`
method.

Boto3 documentation:
[MediaPackage.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

<a id="untag_resource"></a>

### untag_resource

See also:
[AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediapackage-2017-10-12/UntagResource).

Type annotations for `aiobotocore.create_client("mediapackage").untag_resource`
method.

Boto3 documentation:
[MediaPackage.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

<a id="update_channel"></a>

### update_channel

Updates an existing Channel.

Type annotations for `aiobotocore.create_client("mediapackage").update_channel`
method.

Boto3 documentation:
[MediaPackage.Client.update_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.update_channel)

Asynchronous method. Use `await update_channel(...)` for a synchronous call.

Arguments mapping described in
[UpdateChannelRequestRequestTypeDef](./type_defs.md#updatechannelrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Description`: `str`

Returns a `Coroutine` for
[UpdateChannelResponseTypeDef](./type_defs.md#updatechannelresponsetypedef).

<a id="update_origin_endpoint"></a>

### update_origin_endpoint

Updates an existing OriginEndpoint.

Type annotations for
`aiobotocore.create_client("mediapackage").update_origin_endpoint` method.

Boto3 documentation:
[MediaPackage.Client.update_origin_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.update_origin_endpoint)

Asynchronous method. Use `await update_origin_endpoint(...)` for a synchronous
call.

Arguments mapping described in
[UpdateOriginEndpointRequestRequestTypeDef](./type_defs.md#updateoriginendpointrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Authorization`: [AuthorizationTypeDef](./type_defs.md#authorizationtypedef)
- `CmafPackage`:
  [CmafPackageCreateOrUpdateParametersTypeDef](./type_defs.md#cmafpackagecreateorupdateparameterstypedef)
- `DashPackage`: [DashPackageTypeDef](./type_defs.md#dashpackagetypedef)
- `Description`: `str`
- `HlsPackage`: [HlsPackageTypeDef](./type_defs.md#hlspackagetypedef)
- `ManifestName`: `str`
- `MssPackage`: [MssPackageTypeDef](./type_defs.md#msspackagetypedef)
- `Origination`: [OriginationType](./literals.md#originationtype)
- `StartoverWindowSeconds`: `int`
- `TimeDelaySeconds`: `int`
- `Whitelist`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[UpdateOriginEndpointResponseTypeDef](./type_defs.md#updateoriginendpointresponsetypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("mediapackage").get_paginator`
method with overloads.

- `client.get_paginator("list_channels")` ->
  [ListChannelsPaginator](./paginators.md#listchannelspaginator)
- `client.get_paginator("list_harvest_jobs")` ->
  [ListHarvestJobsPaginator](./paginators.md#listharvestjobspaginator)
- `client.get_paginator("list_origin_endpoints")` ->
  [ListOriginEndpointsPaginator](./paginators.md#listoriginendpointspaginator)
