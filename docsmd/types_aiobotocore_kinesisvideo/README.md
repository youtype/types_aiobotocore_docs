# KinesisVideo module

> [Index](../README.md) > KinesisVideo


!!! note ""

    Auto-generated documentation for [KinesisVideo](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#kinesisvideo)
    type annotations stubs module [types-aiobotocore-kinesisvideo](https://pypi.org/project/types-aiobotocore-kinesisvideo/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
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
- [CreateStreamInputTypeDef](./type_defs.md#createstreaminputtypedef)
- [DeleteEdgeConfigurationInputTypeDef](./type_defs.md#deleteedgeconfigurationinputtypedef)
- [DeleteSignalingChannelInputTypeDef](./type_defs.md#deletesignalingchannelinputtypedef)
- [DeleteStreamInputTypeDef](./type_defs.md#deletestreaminputtypedef)
- [LocalSizeConfigTypeDef](./type_defs.md#localsizeconfigtypedef)
- [DescribeEdgeConfigurationInputTypeDef](./type_defs.md#describeedgeconfigurationinputtypedef)
- [DescribeImageGenerationConfigurationInputTypeDef](./type_defs.md#describeimagegenerationconfigurationinputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeMappedResourceConfigurationInputTypeDef](./type_defs.md#describemappedresourceconfigurationinputtypedef)
- [MappedResourceConfigurationListItemTypeDef](./type_defs.md#mappedresourceconfigurationlistitemtypedef)
- [DescribeMediaStorageConfigurationInputTypeDef](./type_defs.md#describemediastorageconfigurationinputtypedef)
- [MediaStorageConfigurationTypeDef](./type_defs.md#mediastorageconfigurationtypedef)
- [DescribeNotificationConfigurationInputTypeDef](./type_defs.md#describenotificationconfigurationinputtypedef)
- [DescribeSignalingChannelInputTypeDef](./type_defs.md#describesignalingchannelinputtypedef)
- [DescribeStreamInputTypeDef](./type_defs.md#describestreaminputtypedef)
- [StreamInfoTypeDef](./type_defs.md#streaminfotypedef)
- [LastRecorderStatusTypeDef](./type_defs.md#lastrecorderstatustypedef)
- [LastUploaderStatusTypeDef](./type_defs.md#lastuploaderstatustypedef)
- [GetDataEndpointInputTypeDef](./type_defs.md#getdataendpointinputtypedef)
- [SingleMasterChannelEndpointConfigurationTypeDef](./type_defs.md#singlemasterchannelendpointconfigurationtypedef)
- [ResourceEndpointListItemTypeDef](./type_defs.md#resourceendpointlistitemtypedef)
- [ImageGenerationDestinationConfigTypeDef](./type_defs.md#imagegenerationdestinationconfigtypedef)
- [ListEdgeAgentConfigurationsInputTypeDef](./type_defs.md#listedgeagentconfigurationsinputtypedef)
- [StreamNameConditionTypeDef](./type_defs.md#streamnameconditiontypedef)
- [ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)
- [ListTagsForStreamInputTypeDef](./type_defs.md#listtagsforstreaminputtypedef)
- [MediaSourceConfigTypeDef](./type_defs.md#mediasourceconfigtypedef)
- [NotificationDestinationConfigTypeDef](./type_defs.md#notificationdestinationconfigtypedef)
- [ScheduleConfigTypeDef](./type_defs.md#scheduleconfigtypedef)
- [TagStreamInputTypeDef](./type_defs.md#tagstreaminputtypedef)
- [UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)
- [UntagStreamInputTypeDef](./type_defs.md#untagstreaminputtypedef)
- [UpdateDataRetentionInputTypeDef](./type_defs.md#updatedataretentioninputtypedef)
- [UpdateStreamInputTypeDef](./type_defs.md#updatestreaminputtypedef)
- [ChannelInfoTypeDef](./type_defs.md#channelinfotypedef)
- [UpdateSignalingChannelInputTypeDef](./type_defs.md#updatesignalingchannelinputtypedef)
- [ListSignalingChannelsInputTypeDef](./type_defs.md#listsignalingchannelsinputtypedef)
- [CreateSignalingChannelInputTypeDef](./type_defs.md#createsignalingchannelinputtypedef)
- [TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)
- [CreateSignalingChannelOutputTypeDef](./type_defs.md#createsignalingchanneloutputtypedef)
- [CreateStreamOutputTypeDef](./type_defs.md#createstreamoutputtypedef)
- [GetDataEndpointOutputTypeDef](./type_defs.md#getdataendpointoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [ListTagsForStreamOutputTypeDef](./type_defs.md#listtagsforstreamoutputtypedef)
- [DeletionConfigTypeDef](./type_defs.md#deletionconfigtypedef)
- [DescribeMappedResourceConfigurationInputPaginateTypeDef](./type_defs.md#describemappedresourceconfigurationinputpaginatetypedef)
- [ListEdgeAgentConfigurationsInputPaginateTypeDef](./type_defs.md#listedgeagentconfigurationsinputpaginatetypedef)
- [ListSignalingChannelsInputPaginateTypeDef](./type_defs.md#listsignalingchannelsinputpaginatetypedef)
- [DescribeMappedResourceConfigurationOutputTypeDef](./type_defs.md#describemappedresourceconfigurationoutputtypedef)
- [DescribeMediaStorageConfigurationOutputTypeDef](./type_defs.md#describemediastorageconfigurationoutputtypedef)
- [UpdateMediaStorageConfigurationInputTypeDef](./type_defs.md#updatemediastorageconfigurationinputtypedef)
- [DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef)
- [ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef)
- [EdgeAgentStatusTypeDef](./type_defs.md#edgeagentstatustypedef)
- [GetSignalingChannelEndpointInputTypeDef](./type_defs.md#getsignalingchannelendpointinputtypedef)
- [GetSignalingChannelEndpointOutputTypeDef](./type_defs.md#getsignalingchannelendpointoutputtypedef)
- [ImageGenerationConfigurationOutputTypeDef](./type_defs.md#imagegenerationconfigurationoutputtypedef)
- [ImageGenerationConfigurationTypeDef](./type_defs.md#imagegenerationconfigurationtypedef)
- [ListStreamsInputPaginateTypeDef](./type_defs.md#liststreamsinputpaginatetypedef)
- [ListStreamsInputTypeDef](./type_defs.md#liststreamsinputtypedef)
- [NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef)
- [RecorderConfigTypeDef](./type_defs.md#recorderconfigtypedef)
- [UploaderConfigTypeDef](./type_defs.md#uploaderconfigtypedef)
- [DescribeSignalingChannelOutputTypeDef](./type_defs.md#describesignalingchanneloutputtypedef)
- [ListSignalingChannelsOutputTypeDef](./type_defs.md#listsignalingchannelsoutputtypedef)
- [DescribeImageGenerationConfigurationOutputTypeDef](./type_defs.md#describeimagegenerationconfigurationoutputtypedef)
- [ImageGenerationConfigurationUnionTypeDef](./type_defs.md#imagegenerationconfigurationuniontypedef)
- [DescribeNotificationConfigurationOutputTypeDef](./type_defs.md#describenotificationconfigurationoutputtypedef)
- [UpdateNotificationConfigurationInputTypeDef](./type_defs.md#updatenotificationconfigurationinputtypedef)
- [EdgeConfigTypeDef](./type_defs.md#edgeconfigtypedef)
- [UpdateImageGenerationConfigurationInputTypeDef](./type_defs.md#updateimagegenerationconfigurationinputtypedef)
- [DescribeEdgeConfigurationOutputTypeDef](./type_defs.md#describeedgeconfigurationoutputtypedef)
- [ListEdgeAgentConfigurationsEdgeConfigTypeDef](./type_defs.md#listedgeagentconfigurationsedgeconfigtypedef)
- [StartEdgeConfigurationUpdateInputTypeDef](./type_defs.md#startedgeconfigurationupdateinputtypedef)
- [StartEdgeConfigurationUpdateOutputTypeDef](./type_defs.md#startedgeconfigurationupdateoutputtypedef)
- [ListEdgeAgentConfigurationsOutputTypeDef](./type_defs.md#listedgeagentconfigurationsoutputtypedef)

