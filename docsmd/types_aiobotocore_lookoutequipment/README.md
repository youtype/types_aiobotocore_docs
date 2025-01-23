# LookoutEquipment module

> [Index](../README.md) > LookoutEquipment


!!! note ""

    Auto-generated documentation for [LookoutEquipment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#lookoutequipment)
    type annotations stubs module [types-aiobotocore-lookoutequipment](https://pypi.org/project/types-aiobotocore-lookoutequipment/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `LookoutEquipment` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `LookoutEquipment` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[lookoutequipment]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[lookoutequipment]'

# standalone installation
python -m pip install types-aiobotocore-lookoutequipment
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-lookoutequipment
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LookoutEquipmentClient

Type annotations and code completion for  `#!python session.create_client("lookoutequipment")` as [LookoutEquipmentClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client)

```python
# LookoutEquipmentClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_lookoutequipment.client import LookoutEquipmentClient


session = get_session()
async with session.create_client("lookoutequipment") as client:
    client: LookoutEquipmentClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AutoPromotionResultType usage example

from types_aiobotocore_lookoutequipment.literals import AutoPromotionResultType

def get_value() -> AutoPromotionResultType:
    return "MODEL_NOT_PROMOTED"
```

- [AutoPromotionResultType](./literals.md#autopromotionresulttype)
- [DataUploadFrequencyType](./literals.md#datauploadfrequencytype)
- [DatasetStatusType](./literals.md#datasetstatustype)
- [InferenceDataImportStrategyType](./literals.md#inferencedataimportstrategytype)
- [InferenceExecutionStatusType](./literals.md#inferenceexecutionstatustype)
- [InferenceSchedulerStatusType](./literals.md#inferenceschedulerstatustype)
- [IngestionJobStatusType](./literals.md#ingestionjobstatustype)
- [LabelRatingType](./literals.md#labelratingtype)
- [LatestInferenceResultType](./literals.md#latestinferenceresulttype)
- [ModelPromoteModeType](./literals.md#modelpromotemodetype)
- [ModelQualityType](./literals.md#modelqualitytype)
- [ModelStatusType](./literals.md#modelstatustype)
- [ModelVersionSourceTypeType](./literals.md#modelversionsourcetypetype)
- [ModelVersionStatusType](./literals.md#modelversionstatustype)
- [MonotonicityType](./literals.md#monotonicitytype)
- [RetrainingSchedulerStatusType](./literals.md#retrainingschedulerstatustype)
- [StatisticalIssueStatusType](./literals.md#statisticalissuestatustype)
- [TargetSamplingRateType](./literals.md#targetsamplingratetype)
- [LookoutEquipmentServiceName](./literals.md#lookoutequipmentservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CategoricalValuesTypeDef](./type_defs.md#categoricalvaluestypedef)
- [CountPercentTypeDef](./type_defs.md#countpercenttypedef)
- [DatasetSchemaTypeDef](./type_defs.md#datasetschematypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [DataPreProcessingConfigurationTypeDef](./type_defs.md#datapreprocessingconfigurationtypedef)
- [DuplicateTimestampsTypeDef](./type_defs.md#duplicatetimestampstypedef)
- [InvalidSensorDataTypeDef](./type_defs.md#invalidsensordatatypedef)
- [MissingSensorDataTypeDef](./type_defs.md#missingsensordatatypedef)
- [UnsupportedTimestampsTypeDef](./type_defs.md#unsupportedtimestampstypedef)
- [DatasetSummaryTypeDef](./type_defs.md#datasetsummarytypedef)
- [DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef)
- [DeleteInferenceSchedulerRequestRequestTypeDef](./type_defs.md#deleteinferenceschedulerrequestrequesttypedef)
- [DeleteLabelGroupRequestRequestTypeDef](./type_defs.md#deletelabelgrouprequestrequesttypedef)
- [DeleteLabelRequestRequestTypeDef](./type_defs.md#deletelabelrequestrequesttypedef)
- [DeleteModelRequestRequestTypeDef](./type_defs.md#deletemodelrequestrequesttypedef)
- [DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef)
- [DeleteRetrainingSchedulerRequestRequestTypeDef](./type_defs.md#deleteretrainingschedulerrequestrequesttypedef)
- [DescribeDataIngestionJobRequestRequestTypeDef](./type_defs.md#describedataingestionjobrequestrequesttypedef)
- [DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef)
- [DescribeInferenceSchedulerRequestRequestTypeDef](./type_defs.md#describeinferenceschedulerrequestrequesttypedef)
- [DescribeLabelGroupRequestRequestTypeDef](./type_defs.md#describelabelgrouprequestrequesttypedef)
- [DescribeLabelRequestRequestTypeDef](./type_defs.md#describelabelrequestrequesttypedef)
- [DescribeModelRequestRequestTypeDef](./type_defs.md#describemodelrequestrequesttypedef)
- [DescribeModelVersionRequestRequestTypeDef](./type_defs.md#describemodelversionrequestrequesttypedef)
- [S3ObjectTypeDef](./type_defs.md#s3objecttypedef)
- [DescribeResourcePolicyRequestRequestTypeDef](./type_defs.md#describeresourcepolicyrequestrequesttypedef)
- [DescribeRetrainingSchedulerRequestRequestTypeDef](./type_defs.md#describeretrainingschedulerrequestrequesttypedef)
- [InferenceEventSummaryTypeDef](./type_defs.md#inferenceeventsummarytypedef)
- [InferenceInputNameConfigurationTypeDef](./type_defs.md#inferenceinputnameconfigurationtypedef)
- [InferenceS3InputConfigurationTypeDef](./type_defs.md#inferences3inputconfigurationtypedef)
- [InferenceS3OutputConfigurationTypeDef](./type_defs.md#inferences3outputconfigurationtypedef)
- [InferenceSchedulerSummaryTypeDef](./type_defs.md#inferenceschedulersummarytypedef)
- [IngestionS3InputConfigurationTypeDef](./type_defs.md#ingestions3inputconfigurationtypedef)
- [MissingCompleteSensorDataTypeDef](./type_defs.md#missingcompletesensordatatypedef)
- [SensorsWithShortDateRangeTypeDef](./type_defs.md#sensorswithshortdaterangetypedef)
- [LabelGroupSummaryTypeDef](./type_defs.md#labelgroupsummarytypedef)
- [LabelSummaryTypeDef](./type_defs.md#labelsummarytypedef)
- [LabelsS3InputConfigurationTypeDef](./type_defs.md#labelss3inputconfigurationtypedef)
- [LargeTimestampGapsTypeDef](./type_defs.md#largetimestampgapstypedef)
- [ListDataIngestionJobsRequestRequestTypeDef](./type_defs.md#listdataingestionjobsrequestrequesttypedef)
- [ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef)
- [ListInferenceSchedulersRequestRequestTypeDef](./type_defs.md#listinferenceschedulersrequestrequesttypedef)
- [ListLabelGroupsRequestRequestTypeDef](./type_defs.md#listlabelgroupsrequestrequesttypedef)
- [ModelVersionSummaryTypeDef](./type_defs.md#modelversionsummarytypedef)
- [ListModelsRequestRequestTypeDef](./type_defs.md#listmodelsrequestrequesttypedef)
- [ListRetrainingSchedulersRequestRequestTypeDef](./type_defs.md#listretrainingschedulersrequestrequesttypedef)
- [RetrainingSchedulerSummaryTypeDef](./type_defs.md#retrainingschedulersummarytypedef)
- [ListSensorStatisticsRequestRequestTypeDef](./type_defs.md#listsensorstatisticsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ModelDiagnosticsS3OutputConfigurationTypeDef](./type_defs.md#modeldiagnosticss3outputconfigurationtypedef)
- [MonotonicValuesTypeDef](./type_defs.md#monotonicvaluestypedef)
- [MultipleOperatingModesTypeDef](./type_defs.md#multipleoperatingmodestypedef)
- [PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef)
- [StartInferenceSchedulerRequestRequestTypeDef](./type_defs.md#startinferenceschedulerrequestrequesttypedef)
- [StartRetrainingSchedulerRequestRequestTypeDef](./type_defs.md#startretrainingschedulerrequestrequesttypedef)
- [StopInferenceSchedulerRequestRequestTypeDef](./type_defs.md#stopinferenceschedulerrequestrequesttypedef)
- [StopRetrainingSchedulerRequestRequestTypeDef](./type_defs.md#stopretrainingschedulerrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateActiveModelVersionRequestRequestTypeDef](./type_defs.md#updateactivemodelversionrequestrequesttypedef)
- [UpdateLabelGroupRequestRequestTypeDef](./type_defs.md#updatelabelgrouprequestrequesttypedef)
- [CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef)
- [CreateLabelGroupRequestRequestTypeDef](./type_defs.md#createlabelgrouprequestrequesttypedef)
- [ImportDatasetRequestRequestTypeDef](./type_defs.md#importdatasetrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef)
- [CreateInferenceSchedulerResponseTypeDef](./type_defs.md#createinferenceschedulerresponsetypedef)
- [CreateLabelGroupResponseTypeDef](./type_defs.md#createlabelgroupresponsetypedef)
- [CreateLabelResponseTypeDef](./type_defs.md#createlabelresponsetypedef)
- [CreateModelResponseTypeDef](./type_defs.md#createmodelresponsetypedef)
- [CreateRetrainingSchedulerResponseTypeDef](./type_defs.md#createretrainingschedulerresponsetypedef)
- [DescribeLabelGroupResponseTypeDef](./type_defs.md#describelabelgroupresponsetypedef)
- [DescribeLabelResponseTypeDef](./type_defs.md#describelabelresponsetypedef)
- [DescribeResourcePolicyResponseTypeDef](./type_defs.md#describeresourcepolicyresponsetypedef)
- [DescribeRetrainingSchedulerResponseTypeDef](./type_defs.md#describeretrainingschedulerresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ImportDatasetResponseTypeDef](./type_defs.md#importdatasetresponsetypedef)
- [ImportModelVersionResponseTypeDef](./type_defs.md#importmodelversionresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef)
- [StartDataIngestionJobResponseTypeDef](./type_defs.md#startdataingestionjobresponsetypedef)
- [StartInferenceSchedulerResponseTypeDef](./type_defs.md#startinferenceschedulerresponsetypedef)
- [StartRetrainingSchedulerResponseTypeDef](./type_defs.md#startretrainingschedulerresponsetypedef)
- [StopInferenceSchedulerResponseTypeDef](./type_defs.md#stopinferenceschedulerresponsetypedef)
- [StopRetrainingSchedulerResponseTypeDef](./type_defs.md#stopretrainingschedulerresponsetypedef)
- [UpdateActiveModelVersionResponseTypeDef](./type_defs.md#updateactivemodelversionresponsetypedef)
- [CreateLabelRequestRequestTypeDef](./type_defs.md#createlabelrequestrequesttypedef)
- [CreateRetrainingSchedulerRequestRequestTypeDef](./type_defs.md#createretrainingschedulerrequestrequesttypedef)
- [ListInferenceEventsRequestRequestTypeDef](./type_defs.md#listinferenceeventsrequestrequesttypedef)
- [ListInferenceExecutionsRequestRequestTypeDef](./type_defs.md#listinferenceexecutionsrequestrequesttypedef)
- [ListLabelsRequestRequestTypeDef](./type_defs.md#listlabelsrequestrequesttypedef)
- [ListModelVersionsRequestRequestTypeDef](./type_defs.md#listmodelversionsrequestrequesttypedef)
- [UpdateRetrainingSchedulerRequestRequestTypeDef](./type_defs.md#updateretrainingschedulerrequestrequesttypedef)
- [ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)
- [IngestedFilesSummaryTypeDef](./type_defs.md#ingestedfilessummarytypedef)
- [ListInferenceEventsResponseTypeDef](./type_defs.md#listinferenceeventsresponsetypedef)
- [InferenceInputConfigurationTypeDef](./type_defs.md#inferenceinputconfigurationtypedef)
- [InferenceOutputConfigurationTypeDef](./type_defs.md#inferenceoutputconfigurationtypedef)
- [ListInferenceSchedulersResponseTypeDef](./type_defs.md#listinferenceschedulersresponsetypedef)
- [IngestionInputConfigurationTypeDef](./type_defs.md#ingestioninputconfigurationtypedef)
- [InsufficientSensorDataTypeDef](./type_defs.md#insufficientsensordatatypedef)
- [ListLabelGroupsResponseTypeDef](./type_defs.md#listlabelgroupsresponsetypedef)
- [ListLabelsResponseTypeDef](./type_defs.md#listlabelsresponsetypedef)
- [LabelsInputConfigurationTypeDef](./type_defs.md#labelsinputconfigurationtypedef)
- [ListModelVersionsResponseTypeDef](./type_defs.md#listmodelversionsresponsetypedef)
- [ListRetrainingSchedulersResponseTypeDef](./type_defs.md#listretrainingschedulersresponsetypedef)
- [ModelDiagnosticsOutputConfigurationTypeDef](./type_defs.md#modeldiagnosticsoutputconfigurationtypedef)
- [SensorStatisticsSummaryTypeDef](./type_defs.md#sensorstatisticssummarytypedef)
- [CreateInferenceSchedulerRequestRequestTypeDef](./type_defs.md#createinferenceschedulerrequestrequesttypedef)
- [DescribeInferenceSchedulerResponseTypeDef](./type_defs.md#describeinferenceschedulerresponsetypedef)
- [InferenceExecutionSummaryTypeDef](./type_defs.md#inferenceexecutionsummarytypedef)
- [UpdateInferenceSchedulerRequestRequestTypeDef](./type_defs.md#updateinferenceschedulerrequestrequesttypedef)
- [DataIngestionJobSummaryTypeDef](./type_defs.md#dataingestionjobsummarytypedef)
- [StartDataIngestionJobRequestRequestTypeDef](./type_defs.md#startdataingestionjobrequestrequesttypedef)
- [DataQualitySummaryTypeDef](./type_defs.md#dataqualitysummarytypedef)
- [ImportModelVersionRequestRequestTypeDef](./type_defs.md#importmodelversionrequestrequesttypedef)
- [CreateModelRequestRequestTypeDef](./type_defs.md#createmodelrequestrequesttypedef)
- [DescribeModelResponseTypeDef](./type_defs.md#describemodelresponsetypedef)
- [DescribeModelVersionResponseTypeDef](./type_defs.md#describemodelversionresponsetypedef)
- [ModelSummaryTypeDef](./type_defs.md#modelsummarytypedef)
- [UpdateModelRequestRequestTypeDef](./type_defs.md#updatemodelrequestrequesttypedef)
- [ListSensorStatisticsResponseTypeDef](./type_defs.md#listsensorstatisticsresponsetypedef)
- [ListInferenceExecutionsResponseTypeDef](./type_defs.md#listinferenceexecutionsresponsetypedef)
- [ListDataIngestionJobsResponseTypeDef](./type_defs.md#listdataingestionjobsresponsetypedef)
- [DescribeDataIngestionJobResponseTypeDef](./type_defs.md#describedataingestionjobresponsetypedef)
- [DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef)
- [ListModelsResponseTypeDef](./type_defs.md#listmodelsresponsetypedef)

