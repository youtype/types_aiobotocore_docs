# mediapackagev2Client

> [Index](../README.md) > [mediapackagev2](./README.md) > mediapackagev2Client

!!! note ""

    Auto-generated documentation for [mediapackagev2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
    type annotations stubs module [types-aiobotocore-mediapackagev2](https://pypi.org/project/types-aiobotocore-mediapackagev2/).

## mediapackagev2Client

Type annotations and code completion for `#!python session.create_client("mediapackagev2")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client)

```python
mediapackagev2Client usage example

from aiobotocore.session import get_session
from types_aiobotocore_mediapackagev2.client import mediapackagev2Client

session = get_session()
async with session.create_client("mediapackagev2") as client:
    client: mediapackagev2Client
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("mediapackagev2").exceptions` structure.

```python
mediapackagev2Client.exceptions usage example

async with session.create_client("mediapackagev2") as client:
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
mediapackagev2Client usage type checking example

from types_aiobotocore_mediapackagev2.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("mediapackagev2").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_channel

Create a channel to start receiving content streams.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").create_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.create_channel)

```python
# create_channel method definition

await def create_channel(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    ClientToken: str = ...,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef) 


```python
# create_channel method usage example with argument unpacking

kwargs: CreateChannelRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.create_channel(**kwargs)
```

1. See [:material-code-braces: CreateChannelRequestRequestTypeDef](./type_defs.md#createchannelrequestrequesttypedef) 

### create\_channel\_group

Create a channel group to group your channels and origin endpoints.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").create_channel_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.create_channel_group)

```python
# create_channel_group method definition

await def create_channel_group(
    self,
    *,
    ChannelGroupName: str,
    ClientToken: str = ...,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateChannelGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateChannelGroupResponseTypeDef](./type_defs.md#createchannelgroupresponsetypedef) 


```python
# create_channel_group method usage example with argument unpacking

kwargs: CreateChannelGroupRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
}

parent.create_channel_group(**kwargs)
```

1. See [:material-code-braces: CreateChannelGroupRequestRequestTypeDef](./type_defs.md#createchannelgrouprequestrequesttypedef) 

### create\_origin\_endpoint

The endpoint is attached to a channel, and represents the output of the live
content.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").create_origin_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.create_origin_endpoint)

```python
# create_origin_endpoint method definition

await def create_origin_endpoint(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    ContainerType: ContainerTypeType,  # (1)
    Segment: SegmentTypeDef = ...,  # (2)
    ClientToken: str = ...,
    Description: str = ...,
    StartoverWindowSeconds: int = ...,
    HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,  # (3)
    LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,  # (4)
    Tags: Mapping[str, str] = ...,
) -> CreateOriginEndpointResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
3. See [:material-code-braces: CreateHlsManifestConfigurationTypeDef](./type_defs.md#createhlsmanifestconfigurationtypedef) 
4. See [:material-code-braces: CreateLowLatencyHlsManifestConfigurationTypeDef](./type_defs.md#createlowlatencyhlsmanifestconfigurationtypedef) 
5. See [:material-code-braces: CreateOriginEndpointResponseTypeDef](./type_defs.md#createoriginendpointresponsetypedef) 


```python
# create_origin_endpoint method usage example with argument unpacking

kwargs: CreateOriginEndpointRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
    "ContainerType": ...,
}

parent.create_origin_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateOriginEndpointRequestRequestTypeDef](./type_defs.md#createoriginendpointrequestrequesttypedef) 

### delete\_channel

Delete a channel to stop AWS Elemental MediaPackage from receiving further
content.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").delete_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.delete_channel)

```python
# delete_channel method definition

await def delete_channel(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_channel method usage example with argument unpacking

kwargs: DeleteChannelRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.delete_channel(**kwargs)
```

1. See [:material-code-braces: DeleteChannelRequestRequestTypeDef](./type_defs.md#deletechannelrequestrequesttypedef) 

### delete\_channel\_group

Delete a channel group.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").delete_channel_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.delete_channel_group)

```python
# delete_channel_group method definition

await def delete_channel_group(
    self,
    *,
    ChannelGroupName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_channel_group method usage example with argument unpacking

kwargs: DeleteChannelGroupRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
}

parent.delete_channel_group(**kwargs)
```

1. See [:material-code-braces: DeleteChannelGroupRequestRequestTypeDef](./type_defs.md#deletechannelgrouprequestrequesttypedef) 

### delete\_channel\_policy

Delete a channel policy.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").delete_channel_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.delete_channel_policy)

```python
# delete_channel_policy method definition

await def delete_channel_policy(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_channel_policy method usage example with argument unpacking

kwargs: DeleteChannelPolicyRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.delete_channel_policy(**kwargs)
```

1. See [:material-code-braces: DeleteChannelPolicyRequestRequestTypeDef](./type_defs.md#deletechannelpolicyrequestrequesttypedef) 

### delete\_origin\_endpoint

Origin endpoints can serve content until they're deleted.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").delete_origin_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.delete_origin_endpoint)

```python
# delete_origin_endpoint method definition

await def delete_origin_endpoint(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_origin_endpoint method usage example with argument unpacking

kwargs: DeleteOriginEndpointRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
}

parent.delete_origin_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteOriginEndpointRequestRequestTypeDef](./type_defs.md#deleteoriginendpointrequestrequesttypedef) 

### delete\_origin\_endpoint\_policy

Delete an origin endpoint policy.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").delete_origin_endpoint_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.delete_origin_endpoint_policy)

```python
# delete_origin_endpoint_policy method definition

await def delete_origin_endpoint_policy(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_origin_endpoint_policy method usage example with argument unpacking

kwargs: DeleteOriginEndpointPolicyRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
}

parent.delete_origin_endpoint_policy(**kwargs)
```

1. See [:material-code-braces: DeleteOriginEndpointPolicyRequestRequestTypeDef](./type_defs.md#deleteoriginendpointpolicyrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.generate_presigned_url)

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


### get\_channel

Retrieves the specified channel that's configured in AWS Elemental MediaPackage,
including the origin endpoints that are associated with it.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.get_channel)

```python
# get_channel method definition

await def get_channel(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
) -> GetChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChannelResponseTypeDef](./type_defs.md#getchannelresponsetypedef) 


```python
# get_channel method usage example with argument unpacking

kwargs: GetChannelRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.get_channel(**kwargs)
```

1. See [:material-code-braces: GetChannelRequestRequestTypeDef](./type_defs.md#getchannelrequestrequesttypedef) 

### get\_channel\_group

Retrieves the specified channel group that's configured in AWS Elemental
MediaPackage, including the channels and origin endpoints that are associated
with it.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_channel_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.get_channel_group)

```python
# get_channel_group method definition

await def get_channel_group(
    self,
    *,
    ChannelGroupName: str,
) -> GetChannelGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChannelGroupResponseTypeDef](./type_defs.md#getchannelgroupresponsetypedef) 


```python
# get_channel_group method usage example with argument unpacking

kwargs: GetChannelGroupRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
}

parent.get_channel_group(**kwargs)
```

1. See [:material-code-braces: GetChannelGroupRequestRequestTypeDef](./type_defs.md#getchannelgrouprequestrequesttypedef) 

### get\_channel\_policy

Retrieves the specified channel policy that's configured in AWS Elemental
MediaPackage.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_channel_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.get_channel_policy)

```python
# get_channel_policy method definition

await def get_channel_policy(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
) -> GetChannelPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChannelPolicyResponseTypeDef](./type_defs.md#getchannelpolicyresponsetypedef) 


```python
# get_channel_policy method usage example with argument unpacking

kwargs: GetChannelPolicyRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.get_channel_policy(**kwargs)
```

1. See [:material-code-braces: GetChannelPolicyRequestRequestTypeDef](./type_defs.md#getchannelpolicyrequestrequesttypedef) 

### get\_origin\_endpoint

Retrieves the specified origin endpoint that's configured in AWS Elemental
MediaPackage to obtain its playback URL and to view the packaging settings that
it's currently using.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_origin_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.get_origin_endpoint)

```python
# get_origin_endpoint method definition

await def get_origin_endpoint(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
) -> GetOriginEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOriginEndpointResponseTypeDef](./type_defs.md#getoriginendpointresponsetypedef) 


```python
# get_origin_endpoint method usage example with argument unpacking

kwargs: GetOriginEndpointRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
}

parent.get_origin_endpoint(**kwargs)
```

1. See [:material-code-braces: GetOriginEndpointRequestRequestTypeDef](./type_defs.md#getoriginendpointrequestrequesttypedef) 

### get\_origin\_endpoint\_policy

Retrieves the specified origin endpoint policy that's configured in AWS
Elemental MediaPackage.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_origin_endpoint_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.get_origin_endpoint_policy)

```python
# get_origin_endpoint_policy method definition

await def get_origin_endpoint_policy(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
) -> GetOriginEndpointPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOriginEndpointPolicyResponseTypeDef](./type_defs.md#getoriginendpointpolicyresponsetypedef) 


```python
# get_origin_endpoint_policy method usage example with argument unpacking

kwargs: GetOriginEndpointPolicyRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
}

parent.get_origin_endpoint_policy(**kwargs)
```

1. See [:material-code-braces: GetOriginEndpointPolicyRequestRequestTypeDef](./type_defs.md#getoriginendpointpolicyrequestrequesttypedef) 

### list\_channel\_groups

Retrieves all channel groups that are configured in AWS Elemental MediaPackage,
including the channels and origin endpoints that are associated with it.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").list_channel_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.list_channel_groups)

```python
# list_channel_groups method definition

await def list_channel_groups(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListChannelGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelGroupsResponseTypeDef](./type_defs.md#listchannelgroupsresponsetypedef) 


```python
# list_channel_groups method usage example with argument unpacking

kwargs: ListChannelGroupsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_channel_groups(**kwargs)
```

1. See [:material-code-braces: ListChannelGroupsRequestRequestTypeDef](./type_defs.md#listchannelgroupsrequestrequesttypedef) 

### list\_channels

Retrieves all channels in a specific channel group that are configured in AWS
Elemental MediaPackage, including the origin endpoints that are associated with
it.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").list_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.list_channels)

```python
# list_channels method definition

await def list_channels(
    self,
    *,
    ChannelGroupName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListChannelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python
# list_channels method usage example with argument unpacking

kwargs: ListChannelsRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
}

parent.list_channels(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestRequestTypeDef](./type_defs.md#listchannelsrequestrequesttypedef) 

### list\_origin\_endpoints

Retrieves all origin endpoints in a specific channel that are configured in AWS
Elemental MediaPackage.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").list_origin_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.list_origin_endpoints)

```python
# list_origin_endpoints method definition

await def list_origin_endpoints(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListOriginEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOriginEndpointsResponseTypeDef](./type_defs.md#listoriginendpointsresponsetypedef) 


```python
# list_origin_endpoints method usage example with argument unpacking

kwargs: ListOriginEndpointsRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.list_origin_endpoints(**kwargs)
```

1. See [:material-code-braces: ListOriginEndpointsRequestRequestTypeDef](./type_defs.md#listoriginendpointsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags assigned to a resource.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_channel\_policy

Attaches an IAM policy to the specified channel.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").put_channel_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.put_channel_policy)

```python
# put_channel_policy method definition

await def put_channel_policy(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    Policy: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_channel_policy method usage example with argument unpacking

kwargs: PutChannelPolicyRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "Policy": ...,
}

parent.put_channel_policy(**kwargs)
```

1. See [:material-code-braces: PutChannelPolicyRequestRequestTypeDef](./type_defs.md#putchannelpolicyrequestrequesttypedef) 

### put\_origin\_endpoint\_policy

Attaches an IAM policy to the specified origin endpoint.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").put_origin_endpoint_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.put_origin_endpoint_policy)

```python
# put_origin_endpoint_policy method definition

await def put_origin_endpoint_policy(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    Policy: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_origin_endpoint_policy method usage example with argument unpacking

kwargs: PutOriginEndpointPolicyRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
    "Policy": ...,
}

parent.put_origin_endpoint_policy(**kwargs)
```

1. See [:material-code-braces: PutOriginEndpointPolicyRequestRequestTypeDef](./type_defs.md#putoriginendpointpolicyrequestrequesttypedef) 

### tag\_resource

Assigns one of more tags (key-value pairs) to the specified MediaPackage
resource.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes one or more tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_channel

Update the specified channel.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").update_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.update_channel)

```python
# update_channel method definition

await def update_channel(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    Description: str = ...,
) -> UpdateChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateChannelResponseTypeDef](./type_defs.md#updatechannelresponsetypedef) 


```python
# update_channel method usage example with argument unpacking

kwargs: UpdateChannelRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.update_channel(**kwargs)
```

1. See [:material-code-braces: UpdateChannelRequestRequestTypeDef](./type_defs.md#updatechannelrequestrequesttypedef) 

### update\_channel\_group

Update the specified channel group.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").update_channel_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.update_channel_group)

```python
# update_channel_group method definition

await def update_channel_group(
    self,
    *,
    ChannelGroupName: str,
    Description: str = ...,
) -> UpdateChannelGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateChannelGroupResponseTypeDef](./type_defs.md#updatechannelgroupresponsetypedef) 


```python
# update_channel_group method usage example with argument unpacking

kwargs: UpdateChannelGroupRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
}

parent.update_channel_group(**kwargs)
```

1. See [:material-code-braces: UpdateChannelGroupRequestRequestTypeDef](./type_defs.md#updatechannelgrouprequestrequesttypedef) 

### update\_origin\_endpoint

Update the specified origin endpoint.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").update_origin_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.update_origin_endpoint)

```python
# update_origin_endpoint method definition

await def update_origin_endpoint(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    ContainerType: ContainerTypeType,  # (1)
    Segment: SegmentTypeDef = ...,  # (2)
    Description: str = ...,
    StartoverWindowSeconds: int = ...,
    HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,  # (3)
    LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,  # (4)
) -> UpdateOriginEndpointResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
3. See [:material-code-braces: CreateHlsManifestConfigurationTypeDef](./type_defs.md#createhlsmanifestconfigurationtypedef) 
4. See [:material-code-braces: CreateLowLatencyHlsManifestConfigurationTypeDef](./type_defs.md#createlowlatencyhlsmanifestconfigurationtypedef) 
5. See [:material-code-braces: UpdateOriginEndpointResponseTypeDef](./type_defs.md#updateoriginendpointresponsetypedef) 


```python
# update_origin_endpoint method usage example with argument unpacking

kwargs: UpdateOriginEndpointRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
    "ContainerType": ...,
}

parent.update_origin_endpoint(**kwargs)
```

1. See [:material-code-braces: UpdateOriginEndpointRequestRequestTypeDef](./type_defs.md#updateoriginendpointrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("mediapackagev2").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> mediapackagev2Client:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("mediapackagev2").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_paginator` method with overloads.

- `client.get_paginator("list_channel_groups")` -> [ListChannelGroupsPaginator](./paginators.md#listchannelgroupspaginator)
- `client.get_paginator("list_channels")` -> [ListChannelsPaginator](./paginators.md#listchannelspaginator)
- `client.get_paginator("list_origin_endpoints")` -> [ListOriginEndpointsPaginator](./paginators.md#listoriginendpointspaginator)



