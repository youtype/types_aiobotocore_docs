# FraudDetector module

> [Index](../README.md) > FraudDetector


!!! note ""

    Auto-generated documentation for [FraudDetector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#frauddetector)
    type annotations stubs module [types-aiobotocore-frauddetector](https://pypi.org/project/types-aiobotocore-frauddetector/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `FraudDetector` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `FraudDetector` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[frauddetector]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[frauddetector]'

# standalone installation
python -m pip install types-aiobotocore-frauddetector
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-frauddetector
```

## Usage

Code samples can be found in [Examples](./usage.md).

## FraudDetectorClient

Type annotations and code completion for  `#!python session.create_client("frauddetector")` as [FraudDetectorClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client)

```python
# FraudDetectorClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_frauddetector.client import FraudDetectorClient


session = get_session()
async with session.create_client("frauddetector") as client:
    client: FraudDetectorClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AsyncJobStatusType usage example

from types_aiobotocore_frauddetector.literals import AsyncJobStatusType

def get_value() -> AsyncJobStatusType:
    return "CANCELED"
```

- [AsyncJobStatusType](./literals.md#asyncjobstatustype)
- [DataSourceType](./literals.md#datasourcetype)
- [DataTypeType](./literals.md#datatypetype)
- [DetectorVersionStatusType](./literals.md#detectorversionstatustype)
- [EventIngestionType](./literals.md#eventingestiontype)
- [LanguageType](./literals.md#languagetype)
- [ListUpdateModeType](./literals.md#listupdatemodetype)
- [ModelEndpointStatusType](./literals.md#modelendpointstatustype)
- [ModelInputDataFormatType](./literals.md#modelinputdataformattype)
- [ModelOutputDataFormatType](./literals.md#modeloutputdataformattype)
- [ModelSourceType](./literals.md#modelsourcetype)
- [ModelTypeEnumType](./literals.md#modeltypeenumtype)
- [ModelVersionStatusType](./literals.md#modelversionstatustype)
- [RuleExecutionModeType](./literals.md#ruleexecutionmodetype)
- [TrainingDataSourceEnumType](./literals.md#trainingdatasourceenumtype)
- [UnlabeledEventsTreatmentType](./literals.md#unlabeledeventstreatmenttype)
- [FraudDetectorServiceName](./literals.md#frauddetectorservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ATIMetricDataPointTypeDef](./type_defs.md#atimetricdatapointtypedef)
- [ATIModelPerformanceTypeDef](./type_defs.md#atimodelperformancetypedef)
- [AggregatedLogOddsMetricTypeDef](./type_defs.md#aggregatedlogoddsmetrictypedef)
- [AggregatedVariablesImpactExplanationTypeDef](./type_defs.md#aggregatedvariablesimpactexplanationtypedef)
- [AllowDenyListTypeDef](./type_defs.md#allowdenylisttypedef)
- [BatchCreateVariableErrorTypeDef](./type_defs.md#batchcreatevariableerrortypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [VariableEntryTypeDef](./type_defs.md#variableentrytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchGetVariableErrorTypeDef](./type_defs.md#batchgetvariableerrortypedef)
- [BatchGetVariableRequestRequestTypeDef](./type_defs.md#batchgetvariablerequestrequesttypedef)
- [VariableTypeDef](./type_defs.md#variabletypedef)
- [BatchImportTypeDef](./type_defs.md#batchimporttypedef)
- [BatchPredictionTypeDef](./type_defs.md#batchpredictiontypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CancelBatchImportJobRequestRequestTypeDef](./type_defs.md#cancelbatchimportjobrequestrequesttypedef)
- [CancelBatchPredictionJobRequestRequestTypeDef](./type_defs.md#cancelbatchpredictionjobrequestrequesttypedef)
- [ModelVersionTypeDef](./type_defs.md#modelversiontypedef)
- [RuleTypeDef](./type_defs.md#ruletypedef)
- [ExternalEventsDetailTypeDef](./type_defs.md#externaleventsdetailtypedef)
- [FieldValidationMessageTypeDef](./type_defs.md#fieldvalidationmessagetypedef)
- [FileValidationMessageTypeDef](./type_defs.md#filevalidationmessagetypedef)
- [DeleteBatchImportJobRequestRequestTypeDef](./type_defs.md#deletebatchimportjobrequestrequesttypedef)
- [DeleteBatchPredictionJobRequestRequestTypeDef](./type_defs.md#deletebatchpredictionjobrequestrequesttypedef)
- [DeleteDetectorRequestRequestTypeDef](./type_defs.md#deletedetectorrequestrequesttypedef)
- [DeleteDetectorVersionRequestRequestTypeDef](./type_defs.md#deletedetectorversionrequestrequesttypedef)
- [DeleteEntityTypeRequestRequestTypeDef](./type_defs.md#deleteentitytyperequestrequesttypedef)
- [DeleteEventRequestRequestTypeDef](./type_defs.md#deleteeventrequestrequesttypedef)
- [DeleteEventTypeRequestRequestTypeDef](./type_defs.md#deleteeventtyperequestrequesttypedef)
- [DeleteEventsByEventTypeRequestRequestTypeDef](./type_defs.md#deleteeventsbyeventtyperequestrequesttypedef)
- [DeleteExternalModelRequestRequestTypeDef](./type_defs.md#deleteexternalmodelrequestrequesttypedef)
- [DeleteLabelRequestRequestTypeDef](./type_defs.md#deletelabelrequestrequesttypedef)
- [DeleteListRequestRequestTypeDef](./type_defs.md#deletelistrequestrequesttypedef)
- [DeleteModelRequestRequestTypeDef](./type_defs.md#deletemodelrequestrequesttypedef)
- [DeleteModelVersionRequestRequestTypeDef](./type_defs.md#deletemodelversionrequestrequesttypedef)
- [DeleteOutcomeRequestRequestTypeDef](./type_defs.md#deleteoutcomerequestrequesttypedef)
- [DeleteVariableRequestRequestTypeDef](./type_defs.md#deletevariablerequestrequesttypedef)
- [DescribeDetectorRequestRequestTypeDef](./type_defs.md#describedetectorrequestrequesttypedef)
- [DetectorVersionSummaryTypeDef](./type_defs.md#detectorversionsummarytypedef)
- [DescribeModelVersionsRequestRequestTypeDef](./type_defs.md#describemodelversionsrequestrequesttypedef)
- [DetectorTypeDef](./type_defs.md#detectortypedef)
- [EntityTypeDef](./type_defs.md#entitytypedef)
- [EntityTypeTypeDef](./type_defs.md#entitytypetypedef)
- [EvaluatedExternalModelTypeDef](./type_defs.md#evaluatedexternalmodeltypedef)
- [EvaluatedRuleTypeDef](./type_defs.md#evaluatedruletypedef)
- [EventOrchestrationTypeDef](./type_defs.md#eventorchestrationtypedef)
- [EventPredictionSummaryTypeDef](./type_defs.md#eventpredictionsummarytypedef)
- [IngestedEventStatisticsTypeDef](./type_defs.md#ingestedeventstatisticstypedef)
- [EventVariableSummaryTypeDef](./type_defs.md#eventvariablesummarytypedef)
- [ExternalModelSummaryTypeDef](./type_defs.md#externalmodelsummarytypedef)
- [ModelInputConfigurationTypeDef](./type_defs.md#modelinputconfigurationtypedef)
- [ModelOutputConfigurationOutputTypeDef](./type_defs.md#modeloutputconfigurationoutputtypedef)
- [FilterConditionTypeDef](./type_defs.md#filterconditiontypedef)
- [GetBatchImportJobsRequestRequestTypeDef](./type_defs.md#getbatchimportjobsrequestrequesttypedef)
- [GetBatchPredictionJobsRequestRequestTypeDef](./type_defs.md#getbatchpredictionjobsrequestrequesttypedef)
- [GetDeleteEventsByEventTypeStatusRequestRequestTypeDef](./type_defs.md#getdeleteeventsbyeventtypestatusrequestrequesttypedef)
- [GetDetectorVersionRequestRequestTypeDef](./type_defs.md#getdetectorversionrequestrequesttypedef)
- [GetDetectorsRequestRequestTypeDef](./type_defs.md#getdetectorsrequestrequesttypedef)
- [GetEntityTypesRequestRequestTypeDef](./type_defs.md#getentitytypesrequestrequesttypedef)
- [GetEventPredictionMetadataRequestRequestTypeDef](./type_defs.md#geteventpredictionmetadatarequestrequesttypedef)
- [RuleResultTypeDef](./type_defs.md#ruleresulttypedef)
- [GetEventRequestRequestTypeDef](./type_defs.md#geteventrequestrequesttypedef)
- [GetEventTypesRequestRequestTypeDef](./type_defs.md#geteventtypesrequestrequesttypedef)
- [GetExternalModelsRequestRequestTypeDef](./type_defs.md#getexternalmodelsrequestrequesttypedef)
- [KMSKeyTypeDef](./type_defs.md#kmskeytypedef)
- [GetLabelsRequestRequestTypeDef](./type_defs.md#getlabelsrequestrequesttypedef)
- [LabelTypeDef](./type_defs.md#labeltypedef)
- [GetListElementsRequestRequestTypeDef](./type_defs.md#getlistelementsrequestrequesttypedef)
- [GetListsMetadataRequestRequestTypeDef](./type_defs.md#getlistsmetadatarequestrequesttypedef)
- [GetModelVersionRequestRequestTypeDef](./type_defs.md#getmodelversionrequestrequesttypedef)
- [GetModelsRequestRequestTypeDef](./type_defs.md#getmodelsrequestrequesttypedef)
- [ModelTypeDef](./type_defs.md#modeltypedef)
- [GetOutcomesRequestRequestTypeDef](./type_defs.md#getoutcomesrequestrequesttypedef)
- [OutcomeTypeDef](./type_defs.md#outcometypedef)
- [GetRulesRequestRequestTypeDef](./type_defs.md#getrulesrequestrequesttypedef)
- [RuleDetailTypeDef](./type_defs.md#ruledetailtypedef)
- [GetVariablesRequestRequestTypeDef](./type_defs.md#getvariablesrequestrequesttypedef)
- [IngestedEventsTimeWindowTypeDef](./type_defs.md#ingestedeventstimewindowtypedef)
- [LabelSchemaOutputTypeDef](./type_defs.md#labelschemaoutputtypedef)
- [LabelSchemaTypeDef](./type_defs.md#labelschematypedef)
- [PredictionTimeRangeTypeDef](./type_defs.md#predictiontimerangetypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [LogOddsMetricTypeDef](./type_defs.md#logoddsmetrictypedef)
- [MetricDataPointTypeDef](./type_defs.md#metricdatapointtypedef)
- [ModelOutputConfigurationTypeDef](./type_defs.md#modeloutputconfigurationtypedef)
- [OFIMetricDataPointTypeDef](./type_defs.md#ofimetricdatapointtypedef)
- [UncertaintyRangeTypeDef](./type_defs.md#uncertaintyrangetypedef)
- [VariableImpactExplanationTypeDef](./type_defs.md#variableimpactexplanationtypedef)
- [PutKMSEncryptionKeyRequestRequestTypeDef](./type_defs.md#putkmsencryptionkeyrequestrequesttypedef)
- [TFIMetricDataPointTypeDef](./type_defs.md#tfimetricdatapointtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDetectorVersionMetadataRequestRequestTypeDef](./type_defs.md#updatedetectorversionmetadatarequestrequesttypedef)
- [UpdateDetectorVersionStatusRequestRequestTypeDef](./type_defs.md#updatedetectorversionstatusrequestrequesttypedef)
- [UpdateEventLabelRequestRequestTypeDef](./type_defs.md#updateeventlabelrequestrequesttypedef)
- [UpdateListRequestRequestTypeDef](./type_defs.md#updatelistrequestrequesttypedef)
- [UpdateModelRequestRequestTypeDef](./type_defs.md#updatemodelrequestrequesttypedef)
- [UpdateModelVersionStatusRequestRequestTypeDef](./type_defs.md#updatemodelversionstatusrequestrequesttypedef)
- [UpdateVariableRequestRequestTypeDef](./type_defs.md#updatevariablerequestrequesttypedef)
- [ATITrainingMetricsValueTypeDef](./type_defs.md#atitrainingmetricsvaluetypedef)
- [AggregatedVariablesImportanceMetricsTypeDef](./type_defs.md#aggregatedvariablesimportancemetricstypedef)
- [CreateBatchImportJobRequestRequestTypeDef](./type_defs.md#createbatchimportjobrequestrequesttypedef)
- [CreateBatchPredictionJobRequestRequestTypeDef](./type_defs.md#createbatchpredictionjobrequestrequesttypedef)
- [CreateListRequestRequestTypeDef](./type_defs.md#createlistrequestrequesttypedef)
- [CreateModelRequestRequestTypeDef](./type_defs.md#createmodelrequestrequesttypedef)
- [CreateRuleRequestRequestTypeDef](./type_defs.md#createrulerequestrequesttypedef)
- [CreateVariableRequestRequestTypeDef](./type_defs.md#createvariablerequestrequesttypedef)
- [PutDetectorRequestRequestTypeDef](./type_defs.md#putdetectorrequestrequesttypedef)
- [PutEntityTypeRequestRequestTypeDef](./type_defs.md#putentitytyperequestrequesttypedef)
- [PutLabelRequestRequestTypeDef](./type_defs.md#putlabelrequestrequesttypedef)
- [PutOutcomeRequestRequestTypeDef](./type_defs.md#putoutcomerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [BatchCreateVariableRequestRequestTypeDef](./type_defs.md#batchcreatevariablerequestrequesttypedef)
- [BatchCreateVariableResultTypeDef](./type_defs.md#batchcreatevariableresulttypedef)
- [CreateDetectorVersionResultTypeDef](./type_defs.md#createdetectorversionresulttypedef)
- [CreateModelVersionResultTypeDef](./type_defs.md#createmodelversionresulttypedef)
- [DeleteEventsByEventTypeResultTypeDef](./type_defs.md#deleteeventsbyeventtyperesulttypedef)
- [GetDeleteEventsByEventTypeStatusResultTypeDef](./type_defs.md#getdeleteeventsbyeventtypestatusresulttypedef)
- [GetListElementsResultTypeDef](./type_defs.md#getlistelementsresulttypedef)
- [GetListsMetadataResultTypeDef](./type_defs.md#getlistsmetadataresulttypedef)
- [ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef)
- [UpdateModelVersionResultTypeDef](./type_defs.md#updatemodelversionresulttypedef)
- [BatchGetVariableResultTypeDef](./type_defs.md#batchgetvariableresulttypedef)
- [GetVariablesResultTypeDef](./type_defs.md#getvariablesresulttypedef)
- [GetBatchImportJobsResultTypeDef](./type_defs.md#getbatchimportjobsresulttypedef)
- [GetBatchPredictionJobsResultTypeDef](./type_defs.md#getbatchpredictionjobsresulttypedef)
- [ModelEndpointDataBlobTypeDef](./type_defs.md#modelendpointdatablobtypedef)
- [ModelScoresTypeDef](./type_defs.md#modelscorestypedef)
- [CreateDetectorVersionRequestRequestTypeDef](./type_defs.md#createdetectorversionrequestrequesttypedef)
- [CreateRuleResultTypeDef](./type_defs.md#createruleresulttypedef)
- [DeleteRuleRequestRequestTypeDef](./type_defs.md#deleterulerequestrequesttypedef)
- [GetDetectorVersionResultTypeDef](./type_defs.md#getdetectorversionresulttypedef)
- [UpdateDetectorVersionRequestRequestTypeDef](./type_defs.md#updatedetectorversionrequestrequesttypedef)
- [UpdateRuleMetadataRequestRequestTypeDef](./type_defs.md#updaterulemetadatarequestrequesttypedef)
- [UpdateRuleVersionRequestRequestTypeDef](./type_defs.md#updateruleversionrequestrequesttypedef)
- [UpdateRuleVersionResultTypeDef](./type_defs.md#updateruleversionresulttypedef)
- [DataValidationMetricsTypeDef](./type_defs.md#datavalidationmetricstypedef)
- [DescribeDetectorResultTypeDef](./type_defs.md#describedetectorresulttypedef)
- [GetDetectorsResultTypeDef](./type_defs.md#getdetectorsresulttypedef)
- [EventTypeDef](./type_defs.md#eventtypedef)
- [SendEventRequestRequestTypeDef](./type_defs.md#sendeventrequestrequesttypedef)
- [GetEntityTypesResultTypeDef](./type_defs.md#getentitytypesresulttypedef)
- [PutEventTypeRequestRequestTypeDef](./type_defs.md#puteventtyperequestrequesttypedef)
- [ListEventPredictionsResultTypeDef](./type_defs.md#listeventpredictionsresulttypedef)
- [EventTypeTypeDef](./type_defs.md#eventtypetypedef)
- [ExternalModelOutputsTypeDef](./type_defs.md#externalmodeloutputstypedef)
- [ExternalModelTypeDef](./type_defs.md#externalmodeltypedef)
- [GetKMSEncryptionKeyResultTypeDef](./type_defs.md#getkmsencryptionkeyresulttypedef)
- [GetLabelsResultTypeDef](./type_defs.md#getlabelsresulttypedef)
- [GetModelsResultTypeDef](./type_defs.md#getmodelsresulttypedef)
- [GetOutcomesResultTypeDef](./type_defs.md#getoutcomesresulttypedef)
- [GetRulesResultTypeDef](./type_defs.md#getrulesresulttypedef)
- [IngestedEventsDetailTypeDef](./type_defs.md#ingestedeventsdetailtypedef)
- [TrainingDataSchemaOutputTypeDef](./type_defs.md#trainingdataschemaoutputtypedef)
- [LabelSchemaUnionTypeDef](./type_defs.md#labelschemauniontypedef)
- [ListEventPredictionsRequestRequestTypeDef](./type_defs.md#listeventpredictionsrequestrequesttypedef)
- [VariableImportanceMetricsTypeDef](./type_defs.md#variableimportancemetricstypedef)
- [TrainingMetricsTypeDef](./type_defs.md#trainingmetricstypedef)
- [PutExternalModelRequestRequestTypeDef](./type_defs.md#putexternalmodelrequestrequesttypedef)
- [OFIModelPerformanceTypeDef](./type_defs.md#ofimodelperformancetypedef)
- [TFIModelPerformanceTypeDef](./type_defs.md#tfimodelperformancetypedef)
- [PredictionExplanationsTypeDef](./type_defs.md#predictionexplanationstypedef)
- [GetEventPredictionRequestRequestTypeDef](./type_defs.md#geteventpredictionrequestrequesttypedef)
- [GetEventResultTypeDef](./type_defs.md#geteventresulttypedef)
- [GetEventTypesResultTypeDef](./type_defs.md#geteventtypesresulttypedef)
- [GetEventPredictionResultTypeDef](./type_defs.md#geteventpredictionresulttypedef)
- [GetExternalModelsResultTypeDef](./type_defs.md#getexternalmodelsresulttypedef)
- [UpdateModelVersionRequestRequestTypeDef](./type_defs.md#updatemodelversionrequestrequesttypedef)
- [GetModelVersionResultTypeDef](./type_defs.md#getmodelversionresulttypedef)
- [TrainingDataSchemaTypeDef](./type_defs.md#trainingdataschematypedef)
- [TrainingResultTypeDef](./type_defs.md#trainingresulttypedef)
- [OFITrainingMetricsValueTypeDef](./type_defs.md#ofitrainingmetricsvaluetypedef)
- [TFITrainingMetricsValueTypeDef](./type_defs.md#tfitrainingmetricsvaluetypedef)
- [ModelVersionEvaluationTypeDef](./type_defs.md#modelversionevaluationtypedef)
- [CreateModelVersionRequestRequestTypeDef](./type_defs.md#createmodelversionrequestrequesttypedef)
- [TrainingMetricsV2TypeDef](./type_defs.md#trainingmetricsv2typedef)
- [EvaluatedModelVersionTypeDef](./type_defs.md#evaluatedmodelversiontypedef)
- [TrainingResultV2TypeDef](./type_defs.md#trainingresultv2typedef)
- [GetEventPredictionMetadataResultTypeDef](./type_defs.md#geteventpredictionmetadataresulttypedef)
- [ModelVersionDetailTypeDef](./type_defs.md#modelversiondetailtypedef)
- [DescribeModelVersionsResultTypeDef](./type_defs.md#describemodelversionsresulttypedef)

