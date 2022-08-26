# KinesisVideo module

> [Index](../README.md) > KinesisVideo


!!! note ""

    Auto-generated documentation for [KinesisVideo](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
    type annotations stubs module [types-aiobotocore-kinesisvideo](https://pypi.org/project/types-aiobotocore-kinesisvideo/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `KinesisVideo` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[kinesisvideo]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[kinesisvideo]'


# standalone installation
python -m pip install types-aiobotocore-kinesisvideo
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-kinesisvideo
```

## Usage

Code samples can be found in [Examples](./usage.md).

## KinesisVideoClient

Type annotations and code completion for  `#!python session.create_client("kinesisvideo")` as [KinesisVideoClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_kinesisvideo.client import KinesisVideoClient


session = get_session()
async with session.create_client("kinesisvideo") as client:
    client: KinesisVideoClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("kinesisvideo").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_kinesisvideo.paginator import ListSignalingChannelsPaginator

def get_list_signaling_channels_paginator() -> ListSignalingChannelsPaginator:
    return client.get_paginator("list_signaling_channels"))
```

- [ListSignalingChannelsPaginator](./paginators.md#listsignalingchannelspaginator)
- [ListStreamsPaginator](./paginators.md#liststreamspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_kinesisvideo.literals import APINameType

def get_value() -> APINameType:
    return "GET_CLIP"
```

- [APINameType](./literals.md#apinametype)
- [ChannelProtocolType](./literals.md#channelprotocoltype)
- [ChannelRoleType](./literals.md#channelroletype)
- [ChannelTypeType](./literals.md#channeltypetype)
- [ComparisonOperatorType](./literals.md#comparisonoperatortype)
- [ConfigurationStatusType](./literals.md#configurationstatustype)
- [FormatConfigKeyType](./literals.md#formatconfigkeytype)
- [FormatType](./literals.md#formattype)
- [ImageSelectorTypeType](./literals.md#imageselectortypetype)
- [ListSignalingChannelsPaginatorName](./literals.md#listsignalingchannelspaginatorname)
- [ListStreamsPaginatorName](./literals.md#liststreamspaginatorname)
- [StatusType](./literals.md#statustype)
- [UpdateDataRetentionOperationType](./literals.md#updatedataretentionoperationtype)
- [KinesisVideoServiceName](./literals.md#kinesisvideoservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef

def get_value() -> SingleMasterConfigurationTypeDef:
    return {
        "MessageTtlSeconds": ...,
    }
```

- [SingleMasterConfigurationTypeDef](./type_defs.md#singlemasterconfigurationtypedef)
- [ChannelNameConditionTypeDef](./type_defs.md#channelnameconditiontypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateStreamInputRequestTypeDef](./type_defs.md#createstreaminputrequesttypedef)
- [DeleteSignalingChannelInputRequestTypeDef](./type_defs.md#deletesignalingchannelinputrequesttypedef)
- [DeleteStreamInputRequestTypeDef](./type_defs.md#deletestreaminputrequesttypedef)
- [DescribeImageGenerationConfigurationInputRequestTypeDef](./type_defs.md#describeimagegenerationconfigurationinputrequesttypedef)
- [DescribeNotificationConfigurationInputRequestTypeDef](./type_defs.md#describenotificationconfigurationinputrequesttypedef)
- [DescribeSignalingChannelInputRequestTypeDef](./type_defs.md#describesignalingchannelinputrequesttypedef)
- [DescribeStreamInputRequestTypeDef](./type_defs.md#describestreaminputrequesttypedef)
- [StreamInfoTypeDef](./type_defs.md#streaminfotypedef)
- [GetDataEndpointInputRequestTypeDef](./type_defs.md#getdataendpointinputrequesttypedef)
- [SingleMasterChannelEndpointConfigurationTypeDef](./type_defs.md#singlemasterchannelendpointconfigurationtypedef)
- [ResourceEndpointListItemTypeDef](./type_defs.md#resourceendpointlistitemtypedef)
- [ImageGenerationDestinationConfigTypeDef](./type_defs.md#imagegenerationdestinationconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [StreamNameConditionTypeDef](./type_defs.md#streamnameconditiontypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ListTagsForStreamInputRequestTypeDef](./type_defs.md#listtagsforstreaminputrequesttypedef)
- [NotificationDestinationConfigTypeDef](./type_defs.md#notificationdestinationconfigtypedef)
- [TagStreamInputRequestTypeDef](./type_defs.md#tagstreaminputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UntagStreamInputRequestTypeDef](./type_defs.md#untagstreaminputrequesttypedef)
- [UpdateDataRetentionInputRequestTypeDef](./type_defs.md#updatedataretentioninputrequesttypedef)
- [UpdateStreamInputRequestTypeDef](./type_defs.md#updatestreaminputrequesttypedef)
- [ChannelInfoTypeDef](./type_defs.md#channelinfotypedef)
- [UpdateSignalingChannelInputRequestTypeDef](./type_defs.md#updatesignalingchannelinputrequesttypedef)
- [ListSignalingChannelsInputRequestTypeDef](./type_defs.md#listsignalingchannelsinputrequesttypedef)
- [CreateSignalingChannelInputRequestTypeDef](./type_defs.md#createsignalingchannelinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [CreateSignalingChannelOutputTypeDef](./type_defs.md#createsignalingchanneloutputtypedef)
- [CreateStreamOutputTypeDef](./type_defs.md#createstreamoutputtypedef)
- [GetDataEndpointOutputTypeDef](./type_defs.md#getdataendpointoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [ListTagsForStreamOutputTypeDef](./type_defs.md#listtagsforstreamoutputtypedef)
- [DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef)
- [ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef)
- [GetSignalingChannelEndpointInputRequestTypeDef](./type_defs.md#getsignalingchannelendpointinputrequesttypedef)
- [GetSignalingChannelEndpointOutputTypeDef](./type_defs.md#getsignalingchannelendpointoutputtypedef)
- [ImageGenerationConfigurationTypeDef](./type_defs.md#imagegenerationconfigurationtypedef)
- [ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef](./type_defs.md#listsignalingchannelsinputlistsignalingchannelspaginatetypedef)
- [ListStreamsInputListStreamsPaginateTypeDef](./type_defs.md#liststreamsinputliststreamspaginatetypedef)
- [ListStreamsInputRequestTypeDef](./type_defs.md#liststreamsinputrequesttypedef)
- [NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef)
- [DescribeSignalingChannelOutputTypeDef](./type_defs.md#describesignalingchanneloutputtypedef)
- [ListSignalingChannelsOutputTypeDef](./type_defs.md#listsignalingchannelsoutputtypedef)
- [DescribeImageGenerationConfigurationOutputTypeDef](./type_defs.md#describeimagegenerationconfigurationoutputtypedef)
- [UpdateImageGenerationConfigurationInputRequestTypeDef](./type_defs.md#updateimagegenerationconfigurationinputrequesttypedef)
- [DescribeNotificationConfigurationOutputTypeDef](./type_defs.md#describenotificationconfigurationoutputtypedef)
- [UpdateNotificationConfigurationInputRequestTypeDef](./type_defs.md#updatenotificationconfigurationinputrequesttypedef)

