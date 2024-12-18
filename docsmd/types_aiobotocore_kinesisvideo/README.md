# KinesisVideo module

> [Index](../README.md) > KinesisVideo


!!! note ""

    Auto-generated documentation for [KinesisVideo](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#kinesisvideo)
    type annotations stubs module [types-aiobotocore-kinesisvideo](https://pypi.org/project/types-aiobotocore-kinesisvideo/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `KinesisVideo` service.
1. Use provided commands to install generated packages.



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

```python
# KinesisVideoClient usage example

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

```python
# DescribeMappedResourceConfigurationPaginator usage example

from types_aiobotocore_kinesisvideo.paginator import DescribeMappedResourceConfigurationPaginator

def get_describe_mapped_resource_configuration_paginator() -> DescribeMappedResourceConfigurationPaginator:
    return client.get_paginator("describe_mapped_resource_configuration"))
```

- [DescribeMappedResourceConfigurationPaginator](./paginators.md#describemappedresourceconfigurationpaginator)
- [ListEdgeAgentConfigurationsPaginator](./paginators.md#listedgeagentconfigurationspaginator)
- [ListSignalingChannelsPaginator](./paginators.md#listsignalingchannelspaginator)
- [ListStreamsPaginator](./paginators.md#liststreamspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# APINameType usage example

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
- [DescribeMappedResourceConfigurationPaginatorName](./literals.md#describemappedresourceconfigurationpaginatorname)
- [FormatConfigKeyType](./literals.md#formatconfigkeytype)
- [FormatType](./literals.md#formattype)
- [ImageSelectorTypeType](./literals.md#imageselectortypetype)
- [ListEdgeAgentConfigurationsPaginatorName](./literals.md#listedgeagentconfigurationspaginatorname)
- [ListSignalingChannelsPaginatorName](./literals.md#listsignalingchannelspaginatorname)
- [ListStreamsPaginatorName](./literals.md#liststreamspaginatorname)
- [MediaStorageConfigurationStatusType](./literals.md#mediastorageconfigurationstatustype)
- [MediaUriTypeType](./literals.md#mediauritypetype)
- [RecorderStatusType](./literals.md#recorderstatustype)
- [StatusType](./literals.md#statustype)
- [StrategyOnFullSizeType](./literals.md#strategyonfullsizetype)
- [SyncStatusType](./literals.md#syncstatustype)
- [UpdateDataRetentionOperationType](./literals.md#updatedataretentionoperationtype)
- [UploaderStatusType](./literals.md#uploaderstatustype)
- [KinesisVideoServiceName](./literals.md#kinesisvideoservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [SingleMasterConfigurationTypeDef](./type_defs.md#singlemasterconfigurationtypedef)
- [ChannelNameConditionTypeDef](./type_defs.md#channelnameconditiontypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateStreamInputRequestTypeDef](./type_defs.md#createstreaminputrequesttypedef)
- [DeleteEdgeConfigurationInputRequestTypeDef](./type_defs.md#deleteedgeconfigurationinputrequesttypedef)
- [DeleteSignalingChannelInputRequestTypeDef](./type_defs.md#deletesignalingchannelinputrequesttypedef)
- [DeleteStreamInputRequestTypeDef](./type_defs.md#deletestreaminputrequesttypedef)
- [LocalSizeConfigTypeDef](./type_defs.md#localsizeconfigtypedef)
- [DescribeEdgeConfigurationInputRequestTypeDef](./type_defs.md#describeedgeconfigurationinputrequesttypedef)
- [DescribeImageGenerationConfigurationInputRequestTypeDef](./type_defs.md#describeimagegenerationconfigurationinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeMappedResourceConfigurationInputRequestTypeDef](./type_defs.md#describemappedresourceconfigurationinputrequesttypedef)
- [MappedResourceConfigurationListItemTypeDef](./type_defs.md#mappedresourceconfigurationlistitemtypedef)
- [DescribeMediaStorageConfigurationInputRequestTypeDef](./type_defs.md#describemediastorageconfigurationinputrequesttypedef)
- [MediaStorageConfigurationTypeDef](./type_defs.md#mediastorageconfigurationtypedef)
- [DescribeNotificationConfigurationInputRequestTypeDef](./type_defs.md#describenotificationconfigurationinputrequesttypedef)
- [DescribeSignalingChannelInputRequestTypeDef](./type_defs.md#describesignalingchannelinputrequesttypedef)
- [DescribeStreamInputRequestTypeDef](./type_defs.md#describestreaminputrequesttypedef)
- [StreamInfoTypeDef](./type_defs.md#streaminfotypedef)
- [LastRecorderStatusTypeDef](./type_defs.md#lastrecorderstatustypedef)
- [LastUploaderStatusTypeDef](./type_defs.md#lastuploaderstatustypedef)
- [GetDataEndpointInputRequestTypeDef](./type_defs.md#getdataendpointinputrequesttypedef)
- [SingleMasterChannelEndpointConfigurationTypeDef](./type_defs.md#singlemasterchannelendpointconfigurationtypedef)
- [ResourceEndpointListItemTypeDef](./type_defs.md#resourceendpointlistitemtypedef)
- [ImageGenerationDestinationConfigTypeDef](./type_defs.md#imagegenerationdestinationconfigtypedef)
- [ListEdgeAgentConfigurationsInputRequestTypeDef](./type_defs.md#listedgeagentconfigurationsinputrequesttypedef)
- [StreamNameConditionTypeDef](./type_defs.md#streamnameconditiontypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ListTagsForStreamInputRequestTypeDef](./type_defs.md#listtagsforstreaminputrequesttypedef)
- [MediaSourceConfigTypeDef](./type_defs.md#mediasourceconfigtypedef)
- [NotificationDestinationConfigTypeDef](./type_defs.md#notificationdestinationconfigtypedef)
- [ScheduleConfigTypeDef](./type_defs.md#scheduleconfigtypedef)
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
- [DeletionConfigTypeDef](./type_defs.md#deletionconfigtypedef)
- [DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef](./type_defs.md#describemappedresourceconfigurationinputdescribemappedresourceconfigurationpaginatetypedef)
- [ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef](./type_defs.md#listedgeagentconfigurationsinputlistedgeagentconfigurationspaginatetypedef)
- [ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef](./type_defs.md#listsignalingchannelsinputlistsignalingchannelspaginatetypedef)
- [DescribeMappedResourceConfigurationOutputTypeDef](./type_defs.md#describemappedresourceconfigurationoutputtypedef)
- [DescribeMediaStorageConfigurationOutputTypeDef](./type_defs.md#describemediastorageconfigurationoutputtypedef)
- [UpdateMediaStorageConfigurationInputRequestTypeDef](./type_defs.md#updatemediastorageconfigurationinputrequesttypedef)
- [DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef)
- [ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef)
- [EdgeAgentStatusTypeDef](./type_defs.md#edgeagentstatustypedef)
- [GetSignalingChannelEndpointInputRequestTypeDef](./type_defs.md#getsignalingchannelendpointinputrequesttypedef)
- [GetSignalingChannelEndpointOutputTypeDef](./type_defs.md#getsignalingchannelendpointoutputtypedef)
- [ImageGenerationConfigurationOutputTypeDef](./type_defs.md#imagegenerationconfigurationoutputtypedef)
- [ImageGenerationConfigurationTypeDef](./type_defs.md#imagegenerationconfigurationtypedef)
- [ListStreamsInputListStreamsPaginateTypeDef](./type_defs.md#liststreamsinputliststreamspaginatetypedef)
- [ListStreamsInputRequestTypeDef](./type_defs.md#liststreamsinputrequesttypedef)
- [NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef)
- [RecorderConfigTypeDef](./type_defs.md#recorderconfigtypedef)
- [UploaderConfigTypeDef](./type_defs.md#uploaderconfigtypedef)
- [DescribeSignalingChannelOutputTypeDef](./type_defs.md#describesignalingchanneloutputtypedef)
- [ListSignalingChannelsOutputTypeDef](./type_defs.md#listsignalingchannelsoutputtypedef)
- [DescribeImageGenerationConfigurationOutputTypeDef](./type_defs.md#describeimagegenerationconfigurationoutputtypedef)
- [UpdateImageGenerationConfigurationInputRequestTypeDef](./type_defs.md#updateimagegenerationconfigurationinputrequesttypedef)
- [DescribeNotificationConfigurationOutputTypeDef](./type_defs.md#describenotificationconfigurationoutputtypedef)
- [UpdateNotificationConfigurationInputRequestTypeDef](./type_defs.md#updatenotificationconfigurationinputrequesttypedef)
- [EdgeConfigTypeDef](./type_defs.md#edgeconfigtypedef)
- [DescribeEdgeConfigurationOutputTypeDef](./type_defs.md#describeedgeconfigurationoutputtypedef)
- [ListEdgeAgentConfigurationsEdgeConfigTypeDef](./type_defs.md#listedgeagentconfigurationsedgeconfigtypedef)
- [StartEdgeConfigurationUpdateInputRequestTypeDef](./type_defs.md#startedgeconfigurationupdateinputrequesttypedef)
- [StartEdgeConfigurationUpdateOutputTypeDef](./type_defs.md#startedgeconfigurationupdateoutputtypedef)
- [ListEdgeAgentConfigurationsOutputTypeDef](./type_defs.md#listedgeagentconfigurationsoutputtypedef)

