# CloudWatchLogs module

> [Index](../README.md) > CloudWatchLogs


!!! note ""

    Auto-generated documentation for [CloudWatchLogs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#cloudwatchlogs)
    type annotations stubs module [types-aiobotocore-logs](https://pypi.org/project/types-aiobotocore-logs/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudWatchLogs` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CloudWatchLogs` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[logs]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[logs]'

# standalone installation
python -m pip install types-aiobotocore-logs
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-logs
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudWatchLogsClient

Type annotations and code completion for  `#!python session.create_client("logs")` as [CloudWatchLogsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client)

```python
# CloudWatchLogsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.client import CloudWatchLogsClient


session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("logs").get_paginator("...")`.

```python
# DescribeConfigurationTemplatesPaginator usage example

from types_aiobotocore_logs.paginator import DescribeConfigurationTemplatesPaginator

def get_describe_configuration_templates_paginator() -> DescribeConfigurationTemplatesPaginator:
    return client.get_paginator("describe_configuration_templates"))
```

- [DescribeConfigurationTemplatesPaginator](./paginators.md#describeconfigurationtemplatespaginator)
- [DescribeDeliveriesPaginator](./paginators.md#describedeliveriespaginator)
- [DescribeDeliveryDestinationsPaginator](./paginators.md#describedeliverydestinationspaginator)
- [DescribeDeliverySourcesPaginator](./paginators.md#describedeliverysourcespaginator)
- [DescribeDestinationsPaginator](./paginators.md#describedestinationspaginator)
- [DescribeExportTasksPaginator](./paginators.md#describeexporttaskspaginator)
- [DescribeLogGroupsPaginator](./paginators.md#describeloggroupspaginator)
- [DescribeLogStreamsPaginator](./paginators.md#describelogstreamspaginator)
- [DescribeMetricFiltersPaginator](./paginators.md#describemetricfilterspaginator)
- [DescribeQueriesPaginator](./paginators.md#describequeriespaginator)
- [DescribeResourcePoliciesPaginator](./paginators.md#describeresourcepoliciespaginator)
- [DescribeSubscriptionFiltersPaginator](./paginators.md#describesubscriptionfilterspaginator)
- [FilterLogEventsPaginator](./paginators.md#filterlogeventspaginator)
- [ListAnomaliesPaginator](./paginators.md#listanomaliespaginator)
- [ListLogAnomalyDetectorsPaginator](./paginators.md#listloganomalydetectorspaginator)
- [ListLogGroupsForQueryPaginator](./paginators.md#listloggroupsforquerypaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AnomalyDetectorStatusType usage example

from types_aiobotocore_logs.literals import AnomalyDetectorStatusType

def get_value() -> AnomalyDetectorStatusType:
    return "ANALYZING"
```

- [AnomalyDetectorStatusType](./literals.md#anomalydetectorstatustype)
- [DataProtectionStatusType](./literals.md#dataprotectionstatustype)
- [DeliveryDestinationTypeType](./literals.md#deliverydestinationtypetype)
- [DescribeConfigurationTemplatesPaginatorName](./literals.md#describeconfigurationtemplatespaginatorname)
- [DescribeDeliveriesPaginatorName](./literals.md#describedeliveriespaginatorname)
- [DescribeDeliveryDestinationsPaginatorName](./literals.md#describedeliverydestinationspaginatorname)
- [DescribeDeliverySourcesPaginatorName](./literals.md#describedeliverysourcespaginatorname)
- [DescribeDestinationsPaginatorName](./literals.md#describedestinationspaginatorname)
- [DescribeExportTasksPaginatorName](./literals.md#describeexporttaskspaginatorname)
- [DescribeLogGroupsPaginatorName](./literals.md#describeloggroupspaginatorname)
- [DescribeLogStreamsPaginatorName](./literals.md#describelogstreamspaginatorname)
- [DescribeMetricFiltersPaginatorName](./literals.md#describemetricfilterspaginatorname)
- [DescribeQueriesPaginatorName](./literals.md#describequeriespaginatorname)
- [DescribeResourcePoliciesPaginatorName](./literals.md#describeresourcepoliciespaginatorname)
- [DescribeSubscriptionFiltersPaginatorName](./literals.md#describesubscriptionfilterspaginatorname)
- [DistributionType](./literals.md#distributiontype)
- [EntityRejectionErrorTypeType](./literals.md#entityrejectionerrortypetype)
- [EvaluationFrequencyType](./literals.md#evaluationfrequencytype)
- [ExportTaskStatusCodeType](./literals.md#exporttaskstatuscodetype)
- [FilterLogEventsPaginatorName](./literals.md#filterlogeventspaginatorname)
- [FlattenedElementType](./literals.md#flattenedelementtype)
- [IndexSourceType](./literals.md#indexsourcetype)
- [InheritedPropertyType](./literals.md#inheritedpropertytype)
- [IntegrationStatusType](./literals.md#integrationstatustype)
- [IntegrationTypeType](./literals.md#integrationtypetype)
- [ListAnomaliesPaginatorName](./literals.md#listanomaliespaginatorname)
- [ListLogAnomalyDetectorsPaginatorName](./literals.md#listloganomalydetectorspaginatorname)
- [ListLogGroupsForQueryPaginatorName](./literals.md#listloggroupsforquerypaginatorname)
- [LogGroupClassType](./literals.md#loggroupclasstype)
- [OpenSearchResourceStatusTypeType](./literals.md#opensearchresourcestatustypetype)
- [OrderByType](./literals.md#orderbytype)
- [OutputFormatType](./literals.md#outputformattype)
- [PolicyTypeType](./literals.md#policytypetype)
- [QueryLanguageType](./literals.md#querylanguagetype)
- [QueryStatusType](./literals.md#querystatustype)
- [ScopeType](./literals.md#scopetype)
- [StandardUnitType](./literals.md#standardunittype)
- [StateType](./literals.md#statetype)
- [SuppressionStateType](./literals.md#suppressionstatetype)
- [SuppressionTypeType](./literals.md#suppressiontypetype)
- [SuppressionUnitType](./literals.md#suppressionunittype)
- [TypeType](./literals.md#typetype)
- [CloudWatchLogsServiceName](./literals.md#cloudwatchlogsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountPolicyTypeDef](./type_defs.md#accountpolicytypedef)
- [AddKeyEntryTypeDef](./type_defs.md#addkeyentrytypedef)
- [AnomalyDetectorTypeDef](./type_defs.md#anomalydetectortypedef)
- [LogEventTypeDef](./type_defs.md#logeventtypedef)
- [PatternTokenTypeDef](./type_defs.md#patterntokentypedef)
- [AssociateKmsKeyRequestRequestTypeDef](./type_defs.md#associatekmskeyrequestrequesttypedef)
- [CSVOutputTypeDef](./type_defs.md#csvoutputtypedef)
- [CSVTypeDef](./type_defs.md#csvtypedef)
- [CancelExportTaskRequestRequestTypeDef](./type_defs.md#cancelexporttaskrequestrequesttypedef)
- [S3DeliveryConfigurationTypeDef](./type_defs.md#s3deliveryconfigurationtypedef)
- [RecordFieldTypeDef](./type_defs.md#recordfieldtypedef)
- [CopyValueEntryTypeDef](./type_defs.md#copyvalueentrytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateExportTaskRequestRequestTypeDef](./type_defs.md#createexporttaskrequestrequesttypedef)
- [CreateLogAnomalyDetectorRequestRequestTypeDef](./type_defs.md#createloganomalydetectorrequestrequesttypedef)
- [CreateLogGroupRequestRequestTypeDef](./type_defs.md#createloggrouprequestrequesttypedef)
- [CreateLogStreamRequestRequestTypeDef](./type_defs.md#createlogstreamrequestrequesttypedef)
- [DateTimeConverterOutputTypeDef](./type_defs.md#datetimeconverteroutputtypedef)
- [DateTimeConverterTypeDef](./type_defs.md#datetimeconvertertypedef)
- [DeleteAccountPolicyRequestRequestTypeDef](./type_defs.md#deleteaccountpolicyrequestrequesttypedef)
- [DeleteDataProtectionPolicyRequestRequestTypeDef](./type_defs.md#deletedataprotectionpolicyrequestrequesttypedef)
- [DeleteDeliveryDestinationPolicyRequestRequestTypeDef](./type_defs.md#deletedeliverydestinationpolicyrequestrequesttypedef)
- [DeleteDeliveryDestinationRequestRequestTypeDef](./type_defs.md#deletedeliverydestinationrequestrequesttypedef)
- [DeleteDeliveryRequestRequestTypeDef](./type_defs.md#deletedeliveryrequestrequesttypedef)
- [DeleteDeliverySourceRequestRequestTypeDef](./type_defs.md#deletedeliverysourcerequestrequesttypedef)
- [DeleteDestinationRequestRequestTypeDef](./type_defs.md#deletedestinationrequestrequesttypedef)
- [DeleteIndexPolicyRequestRequestTypeDef](./type_defs.md#deleteindexpolicyrequestrequesttypedef)
- [DeleteIntegrationRequestRequestTypeDef](./type_defs.md#deleteintegrationrequestrequesttypedef)
- [DeleteKeysOutputTypeDef](./type_defs.md#deletekeysoutputtypedef)
- [DeleteKeysTypeDef](./type_defs.md#deletekeystypedef)
- [DeleteLogAnomalyDetectorRequestRequestTypeDef](./type_defs.md#deleteloganomalydetectorrequestrequesttypedef)
- [DeleteLogGroupRequestRequestTypeDef](./type_defs.md#deleteloggrouprequestrequesttypedef)
- [DeleteLogStreamRequestRequestTypeDef](./type_defs.md#deletelogstreamrequestrequesttypedef)
- [DeleteMetricFilterRequestRequestTypeDef](./type_defs.md#deletemetricfilterrequestrequesttypedef)
- [DeleteQueryDefinitionRequestRequestTypeDef](./type_defs.md#deletequerydefinitionrequestrequesttypedef)
- [DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef)
- [DeleteRetentionPolicyRequestRequestTypeDef](./type_defs.md#deleteretentionpolicyrequestrequesttypedef)
- [DeleteSubscriptionFilterRequestRequestTypeDef](./type_defs.md#deletesubscriptionfilterrequestrequesttypedef)
- [DeleteTransformerRequestRequestTypeDef](./type_defs.md#deletetransformerrequestrequesttypedef)
- [DeliveryDestinationConfigurationTypeDef](./type_defs.md#deliverydestinationconfigurationtypedef)
- [DeliverySourceTypeDef](./type_defs.md#deliverysourcetypedef)
- [DescribeAccountPoliciesRequestRequestTypeDef](./type_defs.md#describeaccountpoliciesrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeConfigurationTemplatesRequestRequestTypeDef](./type_defs.md#describeconfigurationtemplatesrequestrequesttypedef)
- [DescribeDeliveriesRequestRequestTypeDef](./type_defs.md#describedeliveriesrequestrequesttypedef)
- [DescribeDeliveryDestinationsRequestRequestTypeDef](./type_defs.md#describedeliverydestinationsrequestrequesttypedef)
- [DescribeDeliverySourcesRequestRequestTypeDef](./type_defs.md#describedeliverysourcesrequestrequesttypedef)
- [DescribeDestinationsRequestRequestTypeDef](./type_defs.md#describedestinationsrequestrequesttypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [DescribeExportTasksRequestRequestTypeDef](./type_defs.md#describeexporttasksrequestrequesttypedef)
- [DescribeFieldIndexesRequestRequestTypeDef](./type_defs.md#describefieldindexesrequestrequesttypedef)
- [FieldIndexTypeDef](./type_defs.md#fieldindextypedef)
- [DescribeIndexPoliciesRequestRequestTypeDef](./type_defs.md#describeindexpoliciesrequestrequesttypedef)
- [IndexPolicyTypeDef](./type_defs.md#indexpolicytypedef)
- [DescribeLogGroupsRequestRequestTypeDef](./type_defs.md#describeloggroupsrequestrequesttypedef)
- [LogGroupTypeDef](./type_defs.md#loggrouptypedef)
- [DescribeLogStreamsRequestRequestTypeDef](./type_defs.md#describelogstreamsrequestrequesttypedef)
- [LogStreamTypeDef](./type_defs.md#logstreamtypedef)
- [DescribeMetricFiltersRequestRequestTypeDef](./type_defs.md#describemetricfiltersrequestrequesttypedef)
- [DescribeQueriesRequestRequestTypeDef](./type_defs.md#describequeriesrequestrequesttypedef)
- [QueryInfoTypeDef](./type_defs.md#queryinfotypedef)
- [DescribeQueryDefinitionsRequestRequestTypeDef](./type_defs.md#describequerydefinitionsrequestrequesttypedef)
- [QueryDefinitionTypeDef](./type_defs.md#querydefinitiontypedef)
- [DescribeResourcePoliciesRequestRequestTypeDef](./type_defs.md#describeresourcepoliciesrequestrequesttypedef)
- [ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef)
- [DescribeSubscriptionFiltersRequestRequestTypeDef](./type_defs.md#describesubscriptionfiltersrequestrequesttypedef)
- [SubscriptionFilterTypeDef](./type_defs.md#subscriptionfiltertypedef)
- [DisassociateKmsKeyRequestRequestTypeDef](./type_defs.md#disassociatekmskeyrequestrequesttypedef)
- [EntityTypeDef](./type_defs.md#entitytypedef)
- [ExportTaskExecutionInfoTypeDef](./type_defs.md#exporttaskexecutioninfotypedef)
- [ExportTaskStatusTypeDef](./type_defs.md#exporttaskstatustypedef)
- [FilterLogEventsRequestRequestTypeDef](./type_defs.md#filterlogeventsrequestrequesttypedef)
- [FilteredLogEventTypeDef](./type_defs.md#filteredlogeventtypedef)
- [SearchedLogStreamTypeDef](./type_defs.md#searchedlogstreamtypedef)
- [GetDataProtectionPolicyRequestRequestTypeDef](./type_defs.md#getdataprotectionpolicyrequestrequesttypedef)
- [GetDeliveryDestinationPolicyRequestRequestTypeDef](./type_defs.md#getdeliverydestinationpolicyrequestrequesttypedef)
- [PolicyTypeDef](./type_defs.md#policytypedef)
- [GetDeliveryDestinationRequestRequestTypeDef](./type_defs.md#getdeliverydestinationrequestrequesttypedef)
- [GetDeliveryRequestRequestTypeDef](./type_defs.md#getdeliveryrequestrequesttypedef)
- [GetDeliverySourceRequestRequestTypeDef](./type_defs.md#getdeliverysourcerequestrequesttypedef)
- [GetIntegrationRequestRequestTypeDef](./type_defs.md#getintegrationrequestrequesttypedef)
- [GetLogAnomalyDetectorRequestRequestTypeDef](./type_defs.md#getloganomalydetectorrequestrequesttypedef)
- [GetLogEventsRequestRequestTypeDef](./type_defs.md#getlogeventsrequestrequesttypedef)
- [OutputLogEventTypeDef](./type_defs.md#outputlogeventtypedef)
- [GetLogGroupFieldsRequestRequestTypeDef](./type_defs.md#getloggroupfieldsrequestrequesttypedef)
- [LogGroupFieldTypeDef](./type_defs.md#loggroupfieldtypedef)
- [GetLogRecordRequestRequestTypeDef](./type_defs.md#getlogrecordrequestrequesttypedef)
- [GetQueryResultsRequestRequestTypeDef](./type_defs.md#getqueryresultsrequestrequesttypedef)
- [QueryStatisticsTypeDef](./type_defs.md#querystatisticstypedef)
- [ResultFieldTypeDef](./type_defs.md#resultfieldtypedef)
- [GetTransformerRequestRequestTypeDef](./type_defs.md#gettransformerrequestrequesttypedef)
- [GrokTypeDef](./type_defs.md#groktypedef)
- [InputLogEventTypeDef](./type_defs.md#inputlogeventtypedef)
- [IntegrationSummaryTypeDef](./type_defs.md#integrationsummarytypedef)
- [ListAnomaliesRequestRequestTypeDef](./type_defs.md#listanomaliesrequestrequesttypedef)
- [ListIntegrationsRequestRequestTypeDef](./type_defs.md#listintegrationsrequestrequesttypedef)
- [ListLogAnomalyDetectorsRequestRequestTypeDef](./type_defs.md#listloganomalydetectorsrequestrequesttypedef)
- [ListLogGroupsForQueryRequestRequestTypeDef](./type_defs.md#listloggroupsforqueryrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTagsLogGroupRequestRequestTypeDef](./type_defs.md#listtagsloggrouprequestrequesttypedef)
- [ListToMapTypeDef](./type_defs.md#listtomaptypedef)
- [LiveTailSessionLogEventTypeDef](./type_defs.md#livetailsessionlogeventtypedef)
- [LiveTailSessionMetadataTypeDef](./type_defs.md#livetailsessionmetadatatypedef)
- [LiveTailSessionStartTypeDef](./type_defs.md#livetailsessionstarttypedef)
- [LowerCaseStringOutputTypeDef](./type_defs.md#lowercasestringoutputtypedef)
- [LowerCaseStringTypeDef](./type_defs.md#lowercasestringtypedef)
- [MetricFilterMatchRecordTypeDef](./type_defs.md#metricfiltermatchrecordtypedef)
- [MetricTransformationOutputTypeDef](./type_defs.md#metrictransformationoutputtypedef)
- [MetricTransformationTypeDef](./type_defs.md#metrictransformationtypedef)
- [MoveKeyEntryTypeDef](./type_defs.md#movekeyentrytypedef)
- [OpenSearchResourceStatusTypeDef](./type_defs.md#opensearchresourcestatustypedef)
- [OpenSearchResourceConfigTypeDef](./type_defs.md#opensearchresourceconfigtypedef)
- [ParseCloudfrontTypeDef](./type_defs.md#parsecloudfronttypedef)
- [ParseJSONTypeDef](./type_defs.md#parsejsontypedef)
- [ParseKeyValueTypeDef](./type_defs.md#parsekeyvaluetypedef)
- [ParsePostgresTypeDef](./type_defs.md#parsepostgrestypedef)
- [ParseRoute53TypeDef](./type_defs.md#parseroute53typedef)
- [ParseVPCTypeDef](./type_defs.md#parsevpctypedef)
- [ParseWAFTypeDef](./type_defs.md#parsewaftypedef)
- [TrimStringOutputTypeDef](./type_defs.md#trimstringoutputtypedef)
- [UpperCaseStringOutputTypeDef](./type_defs.md#uppercasestringoutputtypedef)
- [PutAccountPolicyRequestRequestTypeDef](./type_defs.md#putaccountpolicyrequestrequesttypedef)
- [PutDataProtectionPolicyRequestRequestTypeDef](./type_defs.md#putdataprotectionpolicyrequestrequesttypedef)
- [PutDeliveryDestinationPolicyRequestRequestTypeDef](./type_defs.md#putdeliverydestinationpolicyrequestrequesttypedef)
- [PutDeliverySourceRequestRequestTypeDef](./type_defs.md#putdeliverysourcerequestrequesttypedef)
- [PutDestinationPolicyRequestRequestTypeDef](./type_defs.md#putdestinationpolicyrequestrequesttypedef)
- [PutDestinationRequestRequestTypeDef](./type_defs.md#putdestinationrequestrequesttypedef)
- [PutIndexPolicyRequestRequestTypeDef](./type_defs.md#putindexpolicyrequestrequesttypedef)
- [RejectedEntityInfoTypeDef](./type_defs.md#rejectedentityinfotypedef)
- [RejectedLogEventsInfoTypeDef](./type_defs.md#rejectedlogeventsinfotypedef)
- [PutQueryDefinitionRequestRequestTypeDef](./type_defs.md#putquerydefinitionrequestrequesttypedef)
- [PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef)
- [PutRetentionPolicyRequestRequestTypeDef](./type_defs.md#putretentionpolicyrequestrequesttypedef)
- [PutSubscriptionFilterRequestRequestTypeDef](./type_defs.md#putsubscriptionfilterrequestrequesttypedef)
- [RenameKeyEntryTypeDef](./type_defs.md#renamekeyentrytypedef)
- [SessionStreamingExceptionTypeDef](./type_defs.md#sessionstreamingexceptiontypedef)
- [SessionTimeoutExceptionTypeDef](./type_defs.md#sessiontimeoutexceptiontypedef)
- [SplitStringEntryTypeDef](./type_defs.md#splitstringentrytypedef)
- [StartLiveTailRequestRequestTypeDef](./type_defs.md#startlivetailrequestrequesttypedef)
- [StartQueryRequestRequestTypeDef](./type_defs.md#startqueryrequestrequesttypedef)
- [StopQueryRequestRequestTypeDef](./type_defs.md#stopqueryrequestrequesttypedef)
- [SubstituteStringEntryTypeDef](./type_defs.md#substitutestringentrytypedef)
- [SuppressionPeriodTypeDef](./type_defs.md#suppressionperiodtypedef)
- [TagLogGroupRequestRequestTypeDef](./type_defs.md#tagloggrouprequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TestMetricFilterRequestRequestTypeDef](./type_defs.md#testmetricfilterrequestrequesttypedef)
- [TransformedLogRecordTypeDef](./type_defs.md#transformedlogrecordtypedef)
- [TrimStringTypeDef](./type_defs.md#trimstringtypedef)
- [TypeConverterEntryTypeDef](./type_defs.md#typeconverterentrytypedef)
- [UntagLogGroupRequestRequestTypeDef](./type_defs.md#untagloggrouprequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateLogAnomalyDetectorRequestRequestTypeDef](./type_defs.md#updateloganomalydetectorrequestrequesttypedef)
- [UpperCaseStringTypeDef](./type_defs.md#uppercasestringtypedef)
- [AddKeysOutputTypeDef](./type_defs.md#addkeysoutputtypedef)
- [AddKeysTypeDef](./type_defs.md#addkeystypedef)
- [AnomalyTypeDef](./type_defs.md#anomalytypedef)
- [CSVUnionTypeDef](./type_defs.md#csvuniontypedef)
- [ConfigurationTemplateDeliveryConfigValuesTypeDef](./type_defs.md#configurationtemplatedeliveryconfigvaluestypedef)
- [CreateDeliveryRequestRequestTypeDef](./type_defs.md#createdeliveryrequestrequesttypedef)
- [DeliveryTypeDef](./type_defs.md#deliverytypedef)
- [UpdateDeliveryConfigurationRequestRequestTypeDef](./type_defs.md#updatedeliveryconfigurationrequestrequesttypedef)
- [CopyValueOutputTypeDef](./type_defs.md#copyvalueoutputtypedef)
- [CopyValueTypeDef](./type_defs.md#copyvaluetypedef)
- [CreateExportTaskResponseTypeDef](./type_defs.md#createexporttaskresponsetypedef)
- [CreateLogAnomalyDetectorResponseTypeDef](./type_defs.md#createloganomalydetectorresponsetypedef)
- [DeleteQueryDefinitionResponseTypeDef](./type_defs.md#deletequerydefinitionresponsetypedef)
- [DescribeAccountPoliciesResponseTypeDef](./type_defs.md#describeaccountpoliciesresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetDataProtectionPolicyResponseTypeDef](./type_defs.md#getdataprotectionpolicyresponsetypedef)
- [GetLogAnomalyDetectorResponseTypeDef](./type_defs.md#getloganomalydetectorresponsetypedef)
- [GetLogRecordResponseTypeDef](./type_defs.md#getlogrecordresponsetypedef)
- [ListLogAnomalyDetectorsResponseTypeDef](./type_defs.md#listloganomalydetectorsresponsetypedef)
- [ListLogGroupsForQueryResponseTypeDef](./type_defs.md#listloggroupsforqueryresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListTagsLogGroupResponseTypeDef](./type_defs.md#listtagsloggroupresponsetypedef)
- [PutAccountPolicyResponseTypeDef](./type_defs.md#putaccountpolicyresponsetypedef)
- [PutDataProtectionPolicyResponseTypeDef](./type_defs.md#putdataprotectionpolicyresponsetypedef)
- [PutIntegrationResponseTypeDef](./type_defs.md#putintegrationresponsetypedef)
- [PutQueryDefinitionResponseTypeDef](./type_defs.md#putquerydefinitionresponsetypedef)
- [StartQueryResponseTypeDef](./type_defs.md#startqueryresponsetypedef)
- [StopQueryResponseTypeDef](./type_defs.md#stopqueryresponsetypedef)
- [DateTimeConverterUnionTypeDef](./type_defs.md#datetimeconverteruniontypedef)
- [DeleteKeysUnionTypeDef](./type_defs.md#deletekeysuniontypedef)
- [DeliveryDestinationTypeDef](./type_defs.md#deliverydestinationtypedef)
- [PutDeliveryDestinationRequestRequestTypeDef](./type_defs.md#putdeliverydestinationrequestrequesttypedef)
- [DescribeDeliverySourcesResponseTypeDef](./type_defs.md#describedeliverysourcesresponsetypedef)
- [GetDeliverySourceResponseTypeDef](./type_defs.md#getdeliverysourceresponsetypedef)
- [PutDeliverySourceResponseTypeDef](./type_defs.md#putdeliverysourceresponsetypedef)
- [DescribeConfigurationTemplatesRequestDescribeConfigurationTemplatesPaginateTypeDef](./type_defs.md#describeconfigurationtemplatesrequestdescribeconfigurationtemplatespaginatetypedef)
- [DescribeDeliveriesRequestDescribeDeliveriesPaginateTypeDef](./type_defs.md#describedeliveriesrequestdescribedeliveriespaginatetypedef)
- [DescribeDeliveryDestinationsRequestDescribeDeliveryDestinationsPaginateTypeDef](./type_defs.md#describedeliverydestinationsrequestdescribedeliverydestinationspaginatetypedef)
- [DescribeDeliverySourcesRequestDescribeDeliverySourcesPaginateTypeDef](./type_defs.md#describedeliverysourcesrequestdescribedeliverysourcespaginatetypedef)
- [DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef](./type_defs.md#describedestinationsrequestdescribedestinationspaginatetypedef)
- [DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef](./type_defs.md#describeexporttasksrequestdescribeexporttaskspaginatetypedef)
- [DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef](./type_defs.md#describeloggroupsrequestdescribeloggroupspaginatetypedef)
- [DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef](./type_defs.md#describelogstreamsrequestdescribelogstreamspaginatetypedef)
- [DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef](./type_defs.md#describemetricfiltersrequestdescribemetricfilterspaginatetypedef)
- [DescribeQueriesRequestDescribeQueriesPaginateTypeDef](./type_defs.md#describequeriesrequestdescribequeriespaginatetypedef)
- [DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef](./type_defs.md#describeresourcepoliciesrequestdescriberesourcepoliciespaginatetypedef)
- [DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef](./type_defs.md#describesubscriptionfiltersrequestdescribesubscriptionfilterspaginatetypedef)
- [FilterLogEventsRequestFilterLogEventsPaginateTypeDef](./type_defs.md#filterlogeventsrequestfilterlogeventspaginatetypedef)
- [ListAnomaliesRequestListAnomaliesPaginateTypeDef](./type_defs.md#listanomaliesrequestlistanomaliespaginatetypedef)
- [ListLogAnomalyDetectorsRequestListLogAnomalyDetectorsPaginateTypeDef](./type_defs.md#listloganomalydetectorsrequestlistloganomalydetectorspaginatetypedef)
- [ListLogGroupsForQueryRequestListLogGroupsForQueryPaginateTypeDef](./type_defs.md#listloggroupsforqueryrequestlistloggroupsforquerypaginatetypedef)
- [DescribeDestinationsResponseTypeDef](./type_defs.md#describedestinationsresponsetypedef)
- [PutDestinationResponseTypeDef](./type_defs.md#putdestinationresponsetypedef)
- [DescribeFieldIndexesResponseTypeDef](./type_defs.md#describefieldindexesresponsetypedef)
- [DescribeIndexPoliciesResponseTypeDef](./type_defs.md#describeindexpoliciesresponsetypedef)
- [PutIndexPolicyResponseTypeDef](./type_defs.md#putindexpolicyresponsetypedef)
- [DescribeLogGroupsResponseTypeDef](./type_defs.md#describeloggroupsresponsetypedef)
- [DescribeLogStreamsResponseTypeDef](./type_defs.md#describelogstreamsresponsetypedef)
- [DescribeQueriesResponseTypeDef](./type_defs.md#describequeriesresponsetypedef)
- [DescribeQueryDefinitionsResponseTypeDef](./type_defs.md#describequerydefinitionsresponsetypedef)
- [DescribeResourcePoliciesResponseTypeDef](./type_defs.md#describeresourcepoliciesresponsetypedef)
- [PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef)
- [DescribeSubscriptionFiltersResponseTypeDef](./type_defs.md#describesubscriptionfiltersresponsetypedef)
- [ExportTaskTypeDef](./type_defs.md#exporttasktypedef)
- [FilterLogEventsResponseTypeDef](./type_defs.md#filterlogeventsresponsetypedef)
- [GetDeliveryDestinationPolicyResponseTypeDef](./type_defs.md#getdeliverydestinationpolicyresponsetypedef)
- [PutDeliveryDestinationPolicyResponseTypeDef](./type_defs.md#putdeliverydestinationpolicyresponsetypedef)
- [GetLogEventsResponseTypeDef](./type_defs.md#getlogeventsresponsetypedef)
- [GetLogGroupFieldsResponseTypeDef](./type_defs.md#getloggroupfieldsresponsetypedef)
- [GetQueryResultsResponseTypeDef](./type_defs.md#getqueryresultsresponsetypedef)
- [PutLogEventsRequestRequestTypeDef](./type_defs.md#putlogeventsrequestrequesttypedef)
- [ListIntegrationsResponseTypeDef](./type_defs.md#listintegrationsresponsetypedef)
- [LiveTailSessionUpdateTypeDef](./type_defs.md#livetailsessionupdatetypedef)
- [LowerCaseStringUnionTypeDef](./type_defs.md#lowercasestringuniontypedef)
- [TestMetricFilterResponseTypeDef](./type_defs.md#testmetricfilterresponsetypedef)
- [MetricFilterTypeDef](./type_defs.md#metricfiltertypedef)
- [MetricTransformationUnionTypeDef](./type_defs.md#metrictransformationuniontypedef)
- [MoveKeysOutputTypeDef](./type_defs.md#movekeysoutputtypedef)
- [MoveKeysTypeDef](./type_defs.md#movekeystypedef)
- [OpenSearchApplicationTypeDef](./type_defs.md#opensearchapplicationtypedef)
- [OpenSearchCollectionTypeDef](./type_defs.md#opensearchcollectiontypedef)
- [OpenSearchDataAccessPolicyTypeDef](./type_defs.md#opensearchdataaccesspolicytypedef)
- [OpenSearchDataSourceTypeDef](./type_defs.md#opensearchdatasourcetypedef)
- [OpenSearchEncryptionPolicyTypeDef](./type_defs.md#opensearchencryptionpolicytypedef)
- [OpenSearchLifecyclePolicyTypeDef](./type_defs.md#opensearchlifecyclepolicytypedef)
- [OpenSearchNetworkPolicyTypeDef](./type_defs.md#opensearchnetworkpolicytypedef)
- [OpenSearchWorkspaceTypeDef](./type_defs.md#opensearchworkspacetypedef)
- [ResourceConfigTypeDef](./type_defs.md#resourceconfigtypedef)
- [PutLogEventsResponseTypeDef](./type_defs.md#putlogeventsresponsetypedef)
- [RenameKeysOutputTypeDef](./type_defs.md#renamekeysoutputtypedef)
- [RenameKeysTypeDef](./type_defs.md#renamekeystypedef)
- [SplitStringOutputTypeDef](./type_defs.md#splitstringoutputtypedef)
- [SplitStringTypeDef](./type_defs.md#splitstringtypedef)
- [SubstituteStringOutputTypeDef](./type_defs.md#substitutestringoutputtypedef)
- [SubstituteStringTypeDef](./type_defs.md#substitutestringtypedef)
- [UpdateAnomalyRequestRequestTypeDef](./type_defs.md#updateanomalyrequestrequesttypedef)
- [TestTransformerResponseTypeDef](./type_defs.md#testtransformerresponsetypedef)
- [TrimStringUnionTypeDef](./type_defs.md#trimstringuniontypedef)
- [TypeConverterOutputTypeDef](./type_defs.md#typeconverteroutputtypedef)
- [TypeConverterTypeDef](./type_defs.md#typeconvertertypedef)
- [UpperCaseStringUnionTypeDef](./type_defs.md#uppercasestringuniontypedef)
- [AddKeysUnionTypeDef](./type_defs.md#addkeysuniontypedef)
- [ListAnomaliesResponseTypeDef](./type_defs.md#listanomaliesresponsetypedef)
- [ConfigurationTemplateTypeDef](./type_defs.md#configurationtemplatetypedef)
- [CreateDeliveryResponseTypeDef](./type_defs.md#createdeliveryresponsetypedef)
- [DescribeDeliveriesResponseTypeDef](./type_defs.md#describedeliveriesresponsetypedef)
- [GetDeliveryResponseTypeDef](./type_defs.md#getdeliveryresponsetypedef)
- [CopyValueUnionTypeDef](./type_defs.md#copyvalueuniontypedef)
- [DescribeDeliveryDestinationsResponseTypeDef](./type_defs.md#describedeliverydestinationsresponsetypedef)
- [GetDeliveryDestinationResponseTypeDef](./type_defs.md#getdeliverydestinationresponsetypedef)
- [PutDeliveryDestinationResponseTypeDef](./type_defs.md#putdeliverydestinationresponsetypedef)
- [DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef)
- [StartLiveTailResponseStreamTypeDef](./type_defs.md#startlivetailresponsestreamtypedef)
- [DescribeMetricFiltersResponseTypeDef](./type_defs.md#describemetricfiltersresponsetypedef)
- [PutMetricFilterRequestRequestTypeDef](./type_defs.md#putmetricfilterrequestrequesttypedef)
- [MoveKeysUnionTypeDef](./type_defs.md#movekeysuniontypedef)
- [OpenSearchIntegrationDetailsTypeDef](./type_defs.md#opensearchintegrationdetailstypedef)
- [PutIntegrationRequestRequestTypeDef](./type_defs.md#putintegrationrequestrequesttypedef)
- [RenameKeysUnionTypeDef](./type_defs.md#renamekeysuniontypedef)
- [SplitStringUnionTypeDef](./type_defs.md#splitstringuniontypedef)
- [SubstituteStringUnionTypeDef](./type_defs.md#substitutestringuniontypedef)
- [ProcessorOutputTypeDef](./type_defs.md#processoroutputtypedef)
- [TypeConverterUnionTypeDef](./type_defs.md#typeconverteruniontypedef)
- [DescribeConfigurationTemplatesResponseTypeDef](./type_defs.md#describeconfigurationtemplatesresponsetypedef)
- [StartLiveTailResponseTypeDef](./type_defs.md#startlivetailresponsetypedef)
- [IntegrationDetailsTypeDef](./type_defs.md#integrationdetailstypedef)
- [GetTransformerResponseTypeDef](./type_defs.md#gettransformerresponsetypedef)
- [ProcessorTypeDef](./type_defs.md#processortypedef)
- [GetIntegrationResponseTypeDef](./type_defs.md#getintegrationresponsetypedef)
- [ProcessorUnionTypeDef](./type_defs.md#processoruniontypedef)
- [TestTransformerRequestRequestTypeDef](./type_defs.md#testtransformerrequestrequesttypedef)
- [PutTransformerRequestRequestTypeDef](./type_defs.md#puttransformerrequestrequesttypedef)

