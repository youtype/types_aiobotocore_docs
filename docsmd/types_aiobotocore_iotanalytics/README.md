# IoTAnalytics module

> [Index](../README.md) > IoTAnalytics


!!! note ""

    Auto-generated documentation for [IoTAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#iotanalytics)
    type annotations stubs module [types-aiobotocore-iotanalytics](https://pypi.org/project/types-aiobotocore-iotanalytics/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `IoTAnalytics` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `IoTAnalytics` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iotanalytics]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iotanalytics]'

# standalone installation
python -m pip install types-aiobotocore-iotanalytics
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iotanalytics
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTAnalyticsClient

Type annotations and code completion for  `#!python session.create_client("iotanalytics")` as [IoTAnalyticsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client)

```python
# IoTAnalyticsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.client import IoTAnalyticsClient


session = get_session()
async with session.create_client("iotanalytics") as client:
    client: IoTAnalyticsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("iotanalytics").get_paginator("...")`.

```python
# ListChannelsPaginator usage example

from types_aiobotocore_iotanalytics.paginator import ListChannelsPaginator

def get_list_channels_paginator() -> ListChannelsPaginator:
    return client.get_paginator("list_channels"))
```

- [ListChannelsPaginator](./paginators.md#listchannelspaginator)
- [ListDatasetContentsPaginator](./paginators.md#listdatasetcontentspaginator)
- [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
- [ListDatastoresPaginator](./paginators.md#listdatastorespaginator)
- [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ChannelStatusType usage example

from types_aiobotocore_iotanalytics.literals import ChannelStatusType

def get_value() -> ChannelStatusType:
    return "ACTIVE"
```

- [ChannelStatusType](./literals.md#channelstatustype)
- [ComputeTypeType](./literals.md#computetypetype)
- [DatasetActionTypeType](./literals.md#datasetactiontypetype)
- [DatasetContentStateType](./literals.md#datasetcontentstatetype)
- [DatasetStatusType](./literals.md#datasetstatustype)
- [DatastoreStatusType](./literals.md#datastorestatustype)
- [FileFormatTypeType](./literals.md#fileformattypetype)
- [ListChannelsPaginatorName](./literals.md#listchannelspaginatorname)
- [ListDatasetContentsPaginatorName](./literals.md#listdatasetcontentspaginatorname)
- [ListDatasetsPaginatorName](./literals.md#listdatasetspaginatorname)
- [ListDatastoresPaginatorName](./literals.md#listdatastorespaginatorname)
- [ListPipelinesPaginatorName](./literals.md#listpipelinespaginatorname)
- [LoggingLevelType](./literals.md#loggingleveltype)
- [ReprocessingStatusType](./literals.md#reprocessingstatustype)
- [IoTAnalyticsServiceName](./literals.md#iotanalyticsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AddAttributesActivityOutputTypeDef](./type_defs.md#addattributesactivityoutputtypedef)
- [AddAttributesActivityTypeDef](./type_defs.md#addattributesactivitytypedef)
- [BatchPutMessageErrorEntryTypeDef](./type_defs.md#batchputmessageerrorentrytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CancelPipelineReprocessingRequestTypeDef](./type_defs.md#cancelpipelinereprocessingrequesttypedef)
- [ChannelActivityTypeDef](./type_defs.md#channelactivitytypedef)
- [ChannelMessagesTypeDef](./type_defs.md#channelmessagestypedef)
- [EstimatedResourceSizeTypeDef](./type_defs.md#estimatedresourcesizetypedef)
- [CustomerManagedChannelS3StorageTypeDef](./type_defs.md#customermanagedchannels3storagetypedef)
- [CustomerManagedChannelS3StorageSummaryTypeDef](./type_defs.md#customermanagedchannels3storagesummarytypedef)
- [RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef)
- [ColumnTypeDef](./type_defs.md#columntypedef)
- [ResourceConfigurationTypeDef](./type_defs.md#resourceconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CreateDatasetContentRequestTypeDef](./type_defs.md#createdatasetcontentrequesttypedef)
- [VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef)
- [CustomerManagedDatastoreS3StorageSummaryTypeDef](./type_defs.md#customermanageddatastores3storagesummarytypedef)
- [CustomerManagedDatastoreS3StorageTypeDef](./type_defs.md#customermanageddatastores3storagetypedef)
- [DatasetActionSummaryTypeDef](./type_defs.md#datasetactionsummarytypedef)
- [IotEventsDestinationConfigurationTypeDef](./type_defs.md#ioteventsdestinationconfigurationtypedef)
- [DatasetContentStatusTypeDef](./type_defs.md#datasetcontentstatustypedef)
- [DatasetContentVersionValueTypeDef](./type_defs.md#datasetcontentversionvaluetypedef)
- [DatasetEntryTypeDef](./type_defs.md#datasetentrytypedef)
- [ScheduleTypeDef](./type_defs.md#scheduletypedef)
- [TriggeringDatasetTypeDef](./type_defs.md#triggeringdatasettypedef)
- [DatastoreActivityTypeDef](./type_defs.md#datastoreactivitytypedef)
- [IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef](./type_defs.md#iotsitewisecustomermanageddatastores3storagesummarytypedef)
- [IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef](./type_defs.md#iotsitewisecustomermanageddatastores3storagetypedef)
- [PartitionTypeDef](./type_defs.md#partitiontypedef)
- [TimestampPartitionTypeDef](./type_defs.md#timestamppartitiontypedef)
- [DeleteChannelRequestTypeDef](./type_defs.md#deletechannelrequesttypedef)
- [DeleteDatasetContentRequestTypeDef](./type_defs.md#deletedatasetcontentrequesttypedef)
- [DeleteDatasetRequestTypeDef](./type_defs.md#deletedatasetrequesttypedef)
- [DeleteDatastoreRequestTypeDef](./type_defs.md#deletedatastorerequesttypedef)
- [DeletePipelineRequestTypeDef](./type_defs.md#deletepipelinerequesttypedef)
- [DeltaTimeSessionWindowConfigurationTypeDef](./type_defs.md#deltatimesessionwindowconfigurationtypedef)
- [DeltaTimeTypeDef](./type_defs.md#deltatimetypedef)
- [DescribeChannelRequestTypeDef](./type_defs.md#describechannelrequesttypedef)
- [DescribeDatasetRequestTypeDef](./type_defs.md#describedatasetrequesttypedef)
- [DescribeDatastoreRequestTypeDef](./type_defs.md#describedatastorerequesttypedef)
- [LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef)
- [DescribePipelineRequestTypeDef](./type_defs.md#describepipelinerequesttypedef)
- [DeviceRegistryEnrichActivityTypeDef](./type_defs.md#deviceregistryenrichactivitytypedef)
- [DeviceShadowEnrichActivityTypeDef](./type_defs.md#deviceshadowenrichactivitytypedef)
- [FilterActivityTypeDef](./type_defs.md#filteractivitytypedef)
- [GetDatasetContentRequestTypeDef](./type_defs.md#getdatasetcontentrequesttypedef)
- [GlueConfigurationTypeDef](./type_defs.md#glueconfigurationtypedef)
- [LambdaActivityTypeDef](./type_defs.md#lambdaactivitytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListChannelsRequestTypeDef](./type_defs.md#listchannelsrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListDatasetsRequestTypeDef](./type_defs.md#listdatasetsrequesttypedef)
- [ListDatastoresRequestTypeDef](./type_defs.md#listdatastoresrequesttypedef)
- [ListPipelinesRequestTypeDef](./type_defs.md#listpipelinesrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [MathActivityTypeDef](./type_defs.md#mathactivitytypedef)
- [OutputFileUriValueTypeDef](./type_defs.md#outputfileurivaluetypedef)
- [RemoveAttributesActivityOutputTypeDef](./type_defs.md#removeattributesactivityoutputtypedef)
- [SelectAttributesActivityOutputTypeDef](./type_defs.md#selectattributesactivityoutputtypedef)
- [ReprocessingSummaryTypeDef](./type_defs.md#reprocessingsummarytypedef)
- [RemoveAttributesActivityTypeDef](./type_defs.md#removeattributesactivitytypedef)
- [SelectAttributesActivityTypeDef](./type_defs.md#selectattributesactivitytypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [AddAttributesActivityUnionTypeDef](./type_defs.md#addattributesactivityuniontypedef)
- [BatchPutMessageResponseTypeDef](./type_defs.md#batchputmessageresponsetypedef)
- [CreateDatasetContentResponseTypeDef](./type_defs.md#createdatasetcontentresponsetypedef)
- [CreatePipelineResponseTypeDef](./type_defs.md#createpipelineresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [RunPipelineActivityResponseTypeDef](./type_defs.md#runpipelineactivityresponsetypedef)
- [SampleChannelDataResponseTypeDef](./type_defs.md#samplechanneldataresponsetypedef)
- [StartPipelineReprocessingResponseTypeDef](./type_defs.md#startpipelinereprocessingresponsetypedef)
- [MessageTypeDef](./type_defs.md#messagetypedef)
- [ChannelStatisticsTypeDef](./type_defs.md#channelstatisticstypedef)
- [DatastoreStatisticsTypeDef](./type_defs.md#datastorestatisticstypedef)
- [ChannelStorageOutputTypeDef](./type_defs.md#channelstorageoutputtypedef)
- [ChannelStorageTypeDef](./type_defs.md#channelstoragetypedef)
- [ChannelStorageSummaryTypeDef](./type_defs.md#channelstoragesummarytypedef)
- [CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef)
- [CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef)
- [CreateDatastoreResponseTypeDef](./type_defs.md#createdatastoreresponsetypedef)
- [SchemaDefinitionOutputTypeDef](./type_defs.md#schemadefinitionoutputtypedef)
- [SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [DatasetContentSummaryTypeDef](./type_defs.md#datasetcontentsummarytypedef)
- [GetDatasetContentResponseTypeDef](./type_defs.md#getdatasetcontentresponsetypedef)
- [DatasetTriggerTypeDef](./type_defs.md#datasettriggertypedef)
- [DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef](./type_defs.md#datastoreiotsitewisemultilayerstoragesummarytypedef)
- [DatastoreIotSiteWiseMultiLayerStorageTypeDef](./type_defs.md#datastoreiotsitewisemultilayerstoragetypedef)
- [DatastorePartitionTypeDef](./type_defs.md#datastorepartitiontypedef)
- [LateDataRuleConfigurationTypeDef](./type_defs.md#latedataruleconfigurationtypedef)
- [QueryFilterTypeDef](./type_defs.md#queryfiltertypedef)
- [DescribeLoggingOptionsResponseTypeDef](./type_defs.md#describeloggingoptionsresponsetypedef)
- [PutLoggingOptionsRequestTypeDef](./type_defs.md#putloggingoptionsrequesttypedef)
- [S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef)
- [ListChannelsRequestPaginateTypeDef](./type_defs.md#listchannelsrequestpaginatetypedef)
- [ListDatasetsRequestPaginateTypeDef](./type_defs.md#listdatasetsrequestpaginatetypedef)
- [ListDatastoresRequestPaginateTypeDef](./type_defs.md#listdatastoresrequestpaginatetypedef)
- [ListPipelinesRequestPaginateTypeDef](./type_defs.md#listpipelinesrequestpaginatetypedef)
- [ListDatasetContentsRequestPaginateTypeDef](./type_defs.md#listdatasetcontentsrequestpaginatetypedef)
- [ListDatasetContentsRequestTypeDef](./type_defs.md#listdatasetcontentsrequesttypedef)
- [SampleChannelDataRequestTypeDef](./type_defs.md#samplechanneldatarequesttypedef)
- [StartPipelineReprocessingRequestTypeDef](./type_defs.md#startpipelinereprocessingrequesttypedef)
- [VariableTypeDef](./type_defs.md#variabletypedef)
- [PipelineActivityOutputTypeDef](./type_defs.md#pipelineactivityoutputtypedef)
- [PipelineSummaryTypeDef](./type_defs.md#pipelinesummarytypedef)
- [RemoveAttributesActivityUnionTypeDef](./type_defs.md#removeattributesactivityuniontypedef)
- [SelectAttributesActivityUnionTypeDef](./type_defs.md#selectattributesactivityuniontypedef)
- [BatchPutMessageRequestTypeDef](./type_defs.md#batchputmessagerequesttypedef)
- [ChannelTypeDef](./type_defs.md#channeltypedef)
- [ChannelStorageUnionTypeDef](./type_defs.md#channelstorageuniontypedef)
- [ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef)
- [ParquetConfigurationOutputTypeDef](./type_defs.md#parquetconfigurationoutputtypedef)
- [ParquetConfigurationTypeDef](./type_defs.md#parquetconfigurationtypedef)
- [ListDatasetContentsResponseTypeDef](./type_defs.md#listdatasetcontentsresponsetypedef)
- [DatasetSummaryTypeDef](./type_defs.md#datasetsummarytypedef)
- [DatastoreStorageSummaryTypeDef](./type_defs.md#datastorestoragesummarytypedef)
- [DatastoreStorageOutputTypeDef](./type_defs.md#datastorestorageoutputtypedef)
- [DatastoreStorageTypeDef](./type_defs.md#datastorestoragetypedef)
- [DatastorePartitionsOutputTypeDef](./type_defs.md#datastorepartitionsoutputtypedef)
- [DatastorePartitionsTypeDef](./type_defs.md#datastorepartitionstypedef)
- [LateDataRuleTypeDef](./type_defs.md#latedataruletypedef)
- [SqlQueryDatasetActionOutputTypeDef](./type_defs.md#sqlquerydatasetactionoutputtypedef)
- [SqlQueryDatasetActionTypeDef](./type_defs.md#sqlquerydatasetactiontypedef)
- [DatasetContentDeliveryDestinationTypeDef](./type_defs.md#datasetcontentdeliverydestinationtypedef)
- [ContainerDatasetActionOutputTypeDef](./type_defs.md#containerdatasetactionoutputtypedef)
- [ContainerDatasetActionTypeDef](./type_defs.md#containerdatasetactiontypedef)
- [PipelineTypeDef](./type_defs.md#pipelinetypedef)
- [ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef)
- [PipelineActivityTypeDef](./type_defs.md#pipelineactivitytypedef)
- [DescribeChannelResponseTypeDef](./type_defs.md#describechannelresponsetypedef)
- [CreateChannelRequestTypeDef](./type_defs.md#createchannelrequesttypedef)
- [UpdateChannelRequestTypeDef](./type_defs.md#updatechannelrequesttypedef)
- [ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)
- [FileFormatConfigurationOutputTypeDef](./type_defs.md#fileformatconfigurationoutputtypedef)
- [FileFormatConfigurationTypeDef](./type_defs.md#fileformatconfigurationtypedef)
- [ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)
- [DatastoreStorageUnionTypeDef](./type_defs.md#datastorestorageuniontypedef)
- [DatastoreSummaryTypeDef](./type_defs.md#datastoresummarytypedef)
- [DatastorePartitionsUnionTypeDef](./type_defs.md#datastorepartitionsuniontypedef)
- [SqlQueryDatasetActionUnionTypeDef](./type_defs.md#sqlquerydatasetactionuniontypedef)
- [DatasetContentDeliveryRuleTypeDef](./type_defs.md#datasetcontentdeliveryruletypedef)
- [DatasetActionOutputTypeDef](./type_defs.md#datasetactionoutputtypedef)
- [ContainerDatasetActionUnionTypeDef](./type_defs.md#containerdatasetactionuniontypedef)
- [DescribePipelineResponseTypeDef](./type_defs.md#describepipelineresponsetypedef)
- [PipelineActivityUnionTypeDef](./type_defs.md#pipelineactivityuniontypedef)
- [DatastoreTypeDef](./type_defs.md#datastoretypedef)
- [FileFormatConfigurationUnionTypeDef](./type_defs.md#fileformatconfigurationuniontypedef)
- [ListDatastoresResponseTypeDef](./type_defs.md#listdatastoresresponsetypedef)
- [DatasetTypeDef](./type_defs.md#datasettypedef)
- [DatasetActionTypeDef](./type_defs.md#datasetactiontypedef)
- [CreatePipelineRequestTypeDef](./type_defs.md#createpipelinerequesttypedef)
- [RunPipelineActivityRequestTypeDef](./type_defs.md#runpipelineactivityrequesttypedef)
- [UpdatePipelineRequestTypeDef](./type_defs.md#updatepipelinerequesttypedef)
- [DescribeDatastoreResponseTypeDef](./type_defs.md#describedatastoreresponsetypedef)
- [CreateDatastoreRequestTypeDef](./type_defs.md#createdatastorerequesttypedef)
- [UpdateDatastoreRequestTypeDef](./type_defs.md#updatedatastorerequesttypedef)
- [DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef)
- [DatasetActionUnionTypeDef](./type_defs.md#datasetactionuniontypedef)
- [CreateDatasetRequestTypeDef](./type_defs.md#createdatasetrequesttypedef)
- [UpdateDatasetRequestTypeDef](./type_defs.md#updatedatasetrequesttypedef)

