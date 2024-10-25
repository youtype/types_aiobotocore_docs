# CloudWatchLogs module

> [Index](../README.md) > CloudWatchLogs


!!! note ""

    Auto-generated documentation for [CloudWatchLogs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
    type annotations stubs module [types-aiobotocore-logs](https://pypi.org/project/types-aiobotocore-logs/).

## How to install



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
- [InheritedPropertyType](./literals.md#inheritedpropertytype)
- [ListAnomaliesPaginatorName](./literals.md#listanomaliespaginatorname)
- [ListLogAnomalyDetectorsPaginatorName](./literals.md#listloganomalydetectorspaginatorname)
- [LogGroupClassType](./literals.md#loggroupclasstype)
- [OrderByType](./literals.md#orderbytype)
- [OutputFormatType](./literals.md#outputformattype)
- [PolicyTypeType](./literals.md#policytypetype)
- [QueryStatusType](./literals.md#querystatustype)
- [ScopeType](./literals.md#scopetype)
- [StandardUnitType](./literals.md#standardunittype)
- [StateType](./literals.md#statetype)
- [SuppressionStateType](./literals.md#suppressionstatetype)
- [SuppressionTypeType](./literals.md#suppressiontypetype)
- [SuppressionUnitType](./literals.md#suppressionunittype)
- [CloudWatchLogsServiceName](./literals.md#cloudwatchlogsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountPolicyTypeDef](./type_defs.md#accountpolicytypedef)
- [AnomalyDetectorTypeDef](./type_defs.md#anomalydetectortypedef)
- [LogEventTypeDef](./type_defs.md#logeventtypedef)
- [PatternTokenTypeDef](./type_defs.md#patterntokentypedef)
- [AssociateKmsKeyRequestRequestTypeDef](./type_defs.md#associatekmskeyrequestrequesttypedef)
- [CancelExportTaskRequestRequestTypeDef](./type_defs.md#cancelexporttaskrequestrequesttypedef)
- [S3DeliveryConfigurationTypeDef](./type_defs.md#s3deliveryconfigurationtypedef)
- [RecordFieldTypeDef](./type_defs.md#recordfieldtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateExportTaskRequestRequestTypeDef](./type_defs.md#createexporttaskrequestrequesttypedef)
- [CreateLogAnomalyDetectorRequestRequestTypeDef](./type_defs.md#createloganomalydetectorrequestrequesttypedef)
- [CreateLogGroupRequestRequestTypeDef](./type_defs.md#createloggrouprequestrequesttypedef)
- [CreateLogStreamRequestRequestTypeDef](./type_defs.md#createlogstreamrequestrequesttypedef)
- [DeleteAccountPolicyRequestRequestTypeDef](./type_defs.md#deleteaccountpolicyrequestrequesttypedef)
- [DeleteDataProtectionPolicyRequestRequestTypeDef](./type_defs.md#deletedataprotectionpolicyrequestrequesttypedef)
- [DeleteDeliveryDestinationPolicyRequestRequestTypeDef](./type_defs.md#deletedeliverydestinationpolicyrequestrequesttypedef)
- [DeleteDeliveryDestinationRequestRequestTypeDef](./type_defs.md#deletedeliverydestinationrequestrequesttypedef)
- [DeleteDeliveryRequestRequestTypeDef](./type_defs.md#deletedeliveryrequestrequesttypedef)
- [DeleteDeliverySourceRequestRequestTypeDef](./type_defs.md#deletedeliverysourcerequestrequesttypedef)
- [DeleteDestinationRequestRequestTypeDef](./type_defs.md#deletedestinationrequestrequesttypedef)
- [DeleteLogAnomalyDetectorRequestRequestTypeDef](./type_defs.md#deleteloganomalydetectorrequestrequesttypedef)
- [DeleteLogGroupRequestRequestTypeDef](./type_defs.md#deleteloggrouprequestrequesttypedef)
- [DeleteLogStreamRequestRequestTypeDef](./type_defs.md#deletelogstreamrequestrequesttypedef)
- [DeleteMetricFilterRequestRequestTypeDef](./type_defs.md#deletemetricfilterrequestrequesttypedef)
- [DeleteQueryDefinitionRequestRequestTypeDef](./type_defs.md#deletequerydefinitionrequestrequesttypedef)
- [DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef)
- [DeleteRetentionPolicyRequestRequestTypeDef](./type_defs.md#deleteretentionpolicyrequestrequesttypedef)
- [DeleteSubscriptionFilterRequestRequestTypeDef](./type_defs.md#deletesubscriptionfilterrequestrequesttypedef)
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
- [GetLogAnomalyDetectorRequestRequestTypeDef](./type_defs.md#getloganomalydetectorrequestrequesttypedef)
- [GetLogEventsRequestRequestTypeDef](./type_defs.md#getlogeventsrequestrequesttypedef)
- [OutputLogEventTypeDef](./type_defs.md#outputlogeventtypedef)
- [GetLogGroupFieldsRequestRequestTypeDef](./type_defs.md#getloggroupfieldsrequestrequesttypedef)
- [LogGroupFieldTypeDef](./type_defs.md#loggroupfieldtypedef)
- [GetLogRecordRequestRequestTypeDef](./type_defs.md#getlogrecordrequestrequesttypedef)
- [GetQueryResultsRequestRequestTypeDef](./type_defs.md#getqueryresultsrequestrequesttypedef)
- [QueryStatisticsTypeDef](./type_defs.md#querystatisticstypedef)
- [ResultFieldTypeDef](./type_defs.md#resultfieldtypedef)
- [InputLogEventTypeDef](./type_defs.md#inputlogeventtypedef)
- [ListAnomaliesRequestRequestTypeDef](./type_defs.md#listanomaliesrequestrequesttypedef)
- [ListLogAnomalyDetectorsRequestRequestTypeDef](./type_defs.md#listloganomalydetectorsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTagsLogGroupRequestRequestTypeDef](./type_defs.md#listtagsloggrouprequestrequesttypedef)
- [LiveTailSessionLogEventTypeDef](./type_defs.md#livetailsessionlogeventtypedef)
- [LiveTailSessionMetadataTypeDef](./type_defs.md#livetailsessionmetadatatypedef)
- [LiveTailSessionStartTypeDef](./type_defs.md#livetailsessionstarttypedef)
- [MetricFilterMatchRecordTypeDef](./type_defs.md#metricfiltermatchrecordtypedef)
- [MetricTransformationOutputTypeDef](./type_defs.md#metrictransformationoutputtypedef)
- [MetricTransformationTypeDef](./type_defs.md#metrictransformationtypedef)
- [PutAccountPolicyRequestRequestTypeDef](./type_defs.md#putaccountpolicyrequestrequesttypedef)
- [PutDataProtectionPolicyRequestRequestTypeDef](./type_defs.md#putdataprotectionpolicyrequestrequesttypedef)
- [PutDeliveryDestinationPolicyRequestRequestTypeDef](./type_defs.md#putdeliverydestinationpolicyrequestrequesttypedef)
- [PutDeliverySourceRequestRequestTypeDef](./type_defs.md#putdeliverysourcerequestrequesttypedef)
- [PutDestinationPolicyRequestRequestTypeDef](./type_defs.md#putdestinationpolicyrequestrequesttypedef)
- [PutDestinationRequestRequestTypeDef](./type_defs.md#putdestinationrequestrequesttypedef)
- [RejectedEntityInfoTypeDef](./type_defs.md#rejectedentityinfotypedef)
- [RejectedLogEventsInfoTypeDef](./type_defs.md#rejectedlogeventsinfotypedef)
- [PutQueryDefinitionRequestRequestTypeDef](./type_defs.md#putquerydefinitionrequestrequesttypedef)
- [PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef)
- [PutRetentionPolicyRequestRequestTypeDef](./type_defs.md#putretentionpolicyrequestrequesttypedef)
- [PutSubscriptionFilterRequestRequestTypeDef](./type_defs.md#putsubscriptionfilterrequestrequesttypedef)
- [SessionStreamingExceptionTypeDef](./type_defs.md#sessionstreamingexceptiontypedef)
- [SessionTimeoutExceptionTypeDef](./type_defs.md#sessiontimeoutexceptiontypedef)
- [StartLiveTailRequestRequestTypeDef](./type_defs.md#startlivetailrequestrequesttypedef)
- [StartQueryRequestRequestTypeDef](./type_defs.md#startqueryrequestrequesttypedef)
- [StopQueryRequestRequestTypeDef](./type_defs.md#stopqueryrequestrequesttypedef)
- [SuppressionPeriodTypeDef](./type_defs.md#suppressionperiodtypedef)
- [TagLogGroupRequestRequestTypeDef](./type_defs.md#tagloggrouprequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TestMetricFilterRequestRequestTypeDef](./type_defs.md#testmetricfilterrequestrequesttypedef)
- [UntagLogGroupRequestRequestTypeDef](./type_defs.md#untagloggrouprequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateLogAnomalyDetectorRequestRequestTypeDef](./type_defs.md#updateloganomalydetectorrequestrequesttypedef)
- [AnomalyTypeDef](./type_defs.md#anomalytypedef)
- [ConfigurationTemplateDeliveryConfigValuesTypeDef](./type_defs.md#configurationtemplatedeliveryconfigvaluestypedef)
- [CreateDeliveryRequestRequestTypeDef](./type_defs.md#createdeliveryrequestrequesttypedef)
- [DeliveryTypeDef](./type_defs.md#deliverytypedef)
- [UpdateDeliveryConfigurationRequestRequestTypeDef](./type_defs.md#updatedeliveryconfigurationrequestrequesttypedef)
- [CreateExportTaskResponseTypeDef](./type_defs.md#createexporttaskresponsetypedef)
- [CreateLogAnomalyDetectorResponseTypeDef](./type_defs.md#createloganomalydetectorresponsetypedef)
- [DeleteQueryDefinitionResponseTypeDef](./type_defs.md#deletequerydefinitionresponsetypedef)
- [DescribeAccountPoliciesResponseTypeDef](./type_defs.md#describeaccountpoliciesresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetDataProtectionPolicyResponseTypeDef](./type_defs.md#getdataprotectionpolicyresponsetypedef)
- [GetLogAnomalyDetectorResponseTypeDef](./type_defs.md#getloganomalydetectorresponsetypedef)
- [GetLogRecordResponseTypeDef](./type_defs.md#getlogrecordresponsetypedef)
- [ListLogAnomalyDetectorsResponseTypeDef](./type_defs.md#listloganomalydetectorsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListTagsLogGroupResponseTypeDef](./type_defs.md#listtagsloggroupresponsetypedef)
- [PutAccountPolicyResponseTypeDef](./type_defs.md#putaccountpolicyresponsetypedef)
- [PutDataProtectionPolicyResponseTypeDef](./type_defs.md#putdataprotectionpolicyresponsetypedef)
- [PutQueryDefinitionResponseTypeDef](./type_defs.md#putquerydefinitionresponsetypedef)
- [StartQueryResponseTypeDef](./type_defs.md#startqueryresponsetypedef)
- [StopQueryResponseTypeDef](./type_defs.md#stopqueryresponsetypedef)
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
- [DescribeDestinationsResponseTypeDef](./type_defs.md#describedestinationsresponsetypedef)
- [PutDestinationResponseTypeDef](./type_defs.md#putdestinationresponsetypedef)
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
- [LiveTailSessionUpdateTypeDef](./type_defs.md#livetailsessionupdatetypedef)
- [TestMetricFilterResponseTypeDef](./type_defs.md#testmetricfilterresponsetypedef)
- [MetricFilterTypeDef](./type_defs.md#metricfiltertypedef)
- [MetricTransformationUnionTypeDef](./type_defs.md#metrictransformationuniontypedef)
- [PutLogEventsResponseTypeDef](./type_defs.md#putlogeventsresponsetypedef)
- [UpdateAnomalyRequestRequestTypeDef](./type_defs.md#updateanomalyrequestrequesttypedef)
- [ListAnomaliesResponseTypeDef](./type_defs.md#listanomaliesresponsetypedef)
- [ConfigurationTemplateTypeDef](./type_defs.md#configurationtemplatetypedef)
- [CreateDeliveryResponseTypeDef](./type_defs.md#createdeliveryresponsetypedef)
- [DescribeDeliveriesResponseTypeDef](./type_defs.md#describedeliveriesresponsetypedef)
- [GetDeliveryResponseTypeDef](./type_defs.md#getdeliveryresponsetypedef)
- [DescribeDeliveryDestinationsResponseTypeDef](./type_defs.md#describedeliverydestinationsresponsetypedef)
- [GetDeliveryDestinationResponseTypeDef](./type_defs.md#getdeliverydestinationresponsetypedef)
- [PutDeliveryDestinationResponseTypeDef](./type_defs.md#putdeliverydestinationresponsetypedef)
- [DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef)
- [StartLiveTailResponseStreamTypeDef](./type_defs.md#startlivetailresponsestreamtypedef)
- [DescribeMetricFiltersResponseTypeDef](./type_defs.md#describemetricfiltersresponsetypedef)
- [PutMetricFilterRequestRequestTypeDef](./type_defs.md#putmetricfilterrequestrequesttypedef)
- [DescribeConfigurationTemplatesResponseTypeDef](./type_defs.md#describeconfigurationtemplatesresponsetypedef)
- [StartLiveTailResponseTypeDef](./type_defs.md#startlivetailresponsetypedef)

