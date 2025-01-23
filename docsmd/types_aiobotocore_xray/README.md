# XRay module

> [Index](../README.md) > XRay


!!! note ""

    Auto-generated documentation for [XRay](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#xray)
    type annotations stubs module [types-aiobotocore-xray](https://pypi.org/project/types-aiobotocore-xray/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `XRay` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `XRay` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[xray]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[xray]'

# standalone installation
python -m pip install types-aiobotocore-xray
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-xray
```

## Usage

Code samples can be found in [Examples](./usage.md).

## XRayClient

Type annotations and code completion for  `#!python session.create_client("xray")` as [XRayClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# XRayClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_xray.client import XRayClient


session = get_session()
async with session.create_client("xray") as client:
    client: XRayClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("xray").get_paginator("...")`.

```python
# BatchGetTracesPaginator usage example

from types_aiobotocore_xray.paginator import BatchGetTracesPaginator

def get_batch_get_traces_paginator() -> BatchGetTracesPaginator:
    return client.get_paginator("batch_get_traces"))
```

- [BatchGetTracesPaginator](./paginators.md#batchgettracespaginator)
- [GetGroupsPaginator](./paginators.md#getgroupspaginator)
- [GetSamplingRulesPaginator](./paginators.md#getsamplingrulespaginator)
- [GetSamplingStatisticSummariesPaginator](./paginators.md#getsamplingstatisticsummariespaginator)
- [GetServiceGraphPaginator](./paginators.md#getservicegraphpaginator)
- [GetTimeSeriesServiceStatisticsPaginator](./paginators.md#gettimeseriesservicestatisticspaginator)
- [GetTraceGraphPaginator](./paginators.md#gettracegraphpaginator)
- [GetTraceSummariesPaginator](./paginators.md#gettracesummariespaginator)
- [ListResourcePoliciesPaginator](./paginators.md#listresourcepoliciespaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BatchGetTracesPaginatorName usage example

from types_aiobotocore_xray.literals import BatchGetTracesPaginatorName

def get_value() -> BatchGetTracesPaginatorName:
    return "batch_get_traces"
```

- [BatchGetTracesPaginatorName](./literals.md#batchgettracespaginatorname)
- [EncryptionStatusType](./literals.md#encryptionstatustype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [GetGroupsPaginatorName](./literals.md#getgroupspaginatorname)
- [GetSamplingRulesPaginatorName](./literals.md#getsamplingrulespaginatorname)
- [GetSamplingStatisticSummariesPaginatorName](./literals.md#getsamplingstatisticsummariespaginatorname)
- [GetServiceGraphPaginatorName](./literals.md#getservicegraphpaginatorname)
- [GetTimeSeriesServiceStatisticsPaginatorName](./literals.md#gettimeseriesservicestatisticspaginatorname)
- [GetTraceGraphPaginatorName](./literals.md#gettracegraphpaginatorname)
- [GetTraceSummariesPaginatorName](./literals.md#gettracesummariespaginatorname)
- [InsightCategoryType](./literals.md#insightcategorytype)
- [InsightStateType](./literals.md#insightstatetype)
- [ListResourcePoliciesPaginatorName](./literals.md#listresourcepoliciespaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [RetrievalStatusType](./literals.md#retrievalstatustype)
- [SamplingStrategyNameType](./literals.md#samplingstrategynametype)
- [TimeRangeTypeType](./literals.md#timerangetypetype)
- [TraceFormatTypeType](./literals.md#traceformattypetype)
- [TraceSegmentDestinationStatusType](./literals.md#tracesegmentdestinationstatustype)
- [TraceSegmentDestinationType](./literals.md#tracesegmentdestinationtype)
- [XRayServiceName](./literals.md#xrayservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AliasTypeDef](./type_defs.md#aliastypedef)
- [AnnotationValueTypeDef](./type_defs.md#annotationvaluetypedef)
- [ServiceIdTypeDef](./type_defs.md#serviceidtypedef)
- [AvailabilityZoneDetailTypeDef](./type_defs.md#availabilityzonedetailtypedef)
- [BackendConnectionErrorsTypeDef](./type_defs.md#backendconnectionerrorstypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [BatchGetTracesRequestRequestTypeDef](./type_defs.md#batchgettracesrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CancelTraceRetrievalRequestRequestTypeDef](./type_defs.md#canceltraceretrievalrequestrequesttypedef)
- [InsightsConfigurationTypeDef](./type_defs.md#insightsconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [SamplingRuleTypeDef](./type_defs.md#samplingruletypedef)
- [DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef)
- [DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef)
- [DeleteSamplingRuleRequestRequestTypeDef](./type_defs.md#deletesamplingrulerequestrequesttypedef)
- [ErrorStatisticsTypeDef](./type_defs.md#errorstatisticstypedef)
- [FaultStatisticsTypeDef](./type_defs.md#faultstatisticstypedef)
- [HistogramEntryTypeDef](./type_defs.md#histogramentrytypedef)
- [EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef)
- [RootCauseExceptionTypeDef](./type_defs.md#rootcauseexceptiontypedef)
- [ForecastStatisticsTypeDef](./type_defs.md#forecaststatisticstypedef)
- [GetGroupRequestRequestTypeDef](./type_defs.md#getgrouprequestrequesttypedef)
- [GetGroupsRequestRequestTypeDef](./type_defs.md#getgroupsrequestrequesttypedef)
- [GetIndexingRulesRequestRequestTypeDef](./type_defs.md#getindexingrulesrequestrequesttypedef)
- [GetInsightEventsRequestRequestTypeDef](./type_defs.md#getinsighteventsrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [GetInsightRequestRequestTypeDef](./type_defs.md#getinsightrequestrequesttypedef)
- [GetRetrievedTracesGraphRequestRequestTypeDef](./type_defs.md#getretrievedtracesgraphrequestrequesttypedef)
- [GetSamplingRulesRequestRequestTypeDef](./type_defs.md#getsamplingrulesrequestrequesttypedef)
- [GetSamplingStatisticSummariesRequestRequestTypeDef](./type_defs.md#getsamplingstatisticsummariesrequestrequesttypedef)
- [SamplingStatisticSummaryTypeDef](./type_defs.md#samplingstatisticsummarytypedef)
- [SamplingTargetDocumentTypeDef](./type_defs.md#samplingtargetdocumenttypedef)
- [UnprocessedStatisticsTypeDef](./type_defs.md#unprocessedstatisticstypedef)
- [GetTraceGraphRequestRequestTypeDef](./type_defs.md#gettracegraphrequestrequesttypedef)
- [SamplingStrategyTypeDef](./type_defs.md#samplingstrategytypedef)
- [GraphLinkTypeDef](./type_defs.md#graphlinktypedef)
- [HttpTypeDef](./type_defs.md#httptypedef)
- [ProbabilisticRuleValueTypeDef](./type_defs.md#probabilisticrulevaluetypedef)
- [ProbabilisticRuleValueUpdateTypeDef](./type_defs.md#probabilisticrulevalueupdatetypedef)
- [RequestImpactStatisticsTypeDef](./type_defs.md#requestimpactstatisticstypedef)
- [InsightImpactGraphEdgeTypeDef](./type_defs.md#insightimpactgraphedgetypedef)
- [InstanceIdDetailTypeDef](./type_defs.md#instanceiddetailtypedef)
- [ListResourcePoliciesRequestRequestTypeDef](./type_defs.md#listresourcepoliciesrequestrequesttypedef)
- [ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef)
- [ListRetrievedTracesRequestRequestTypeDef](./type_defs.md#listretrievedtracesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [PutEncryptionConfigRequestRequestTypeDef](./type_defs.md#putencryptionconfigrequestrequesttypedef)
- [PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef)
- [PutTraceSegmentsRequestRequestTypeDef](./type_defs.md#puttracesegmentsrequestrequesttypedef)
- [UnprocessedTraceSegmentTypeDef](./type_defs.md#unprocessedtracesegmenttypedef)
- [ResourceARNDetailTypeDef](./type_defs.md#resourcearndetailtypedef)
- [ResponseTimeRootCauseEntityTypeDef](./type_defs.md#responsetimerootcauseentitytypedef)
- [SpanTypeDef](./type_defs.md#spantypedef)
- [SamplingRuleOutputTypeDef](./type_defs.md#samplingruleoutputtypedef)
- [SamplingRuleUpdateTypeDef](./type_defs.md#samplingruleupdatetypedef)
- [SegmentTypeDef](./type_defs.md#segmenttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateTraceSegmentDestinationRequestRequestTypeDef](./type_defs.md#updatetracesegmentdestinationrequestrequesttypedef)
- [AnomalousServiceTypeDef](./type_defs.md#anomalousservicetypedef)
- [TraceUserTypeDef](./type_defs.md#traceusertypedef)
- [ValueWithServiceIdsTypeDef](./type_defs.md#valuewithserviceidstypedef)
- [BatchGetTracesRequestPaginateTypeDef](./type_defs.md#batchgettracesrequestpaginatetypedef)
- [GetGroupsRequestPaginateTypeDef](./type_defs.md#getgroupsrequestpaginatetypedef)
- [GetSamplingRulesRequestPaginateTypeDef](./type_defs.md#getsamplingrulesrequestpaginatetypedef)
- [GetSamplingStatisticSummariesRequestPaginateTypeDef](./type_defs.md#getsamplingstatisticsummariesrequestpaginatetypedef)
- [GetTraceGraphRequestPaginateTypeDef](./type_defs.md#gettracegraphrequestpaginatetypedef)
- [ListResourcePoliciesRequestPaginateTypeDef](./type_defs.md#listresourcepoliciesrequestpaginatetypedef)
- [ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef)
- [GetTraceSegmentDestinationResultTypeDef](./type_defs.md#gettracesegmentdestinationresulttypedef)
- [StartTraceRetrievalResultTypeDef](./type_defs.md#starttraceretrievalresulttypedef)
- [UpdateTraceSegmentDestinationResultTypeDef](./type_defs.md#updatetracesegmentdestinationresulttypedef)
- [GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef)
- [GroupTypeDef](./type_defs.md#grouptypedef)
- [UpdateGroupRequestRequestTypeDef](./type_defs.md#updategrouprequestrequesttypedef)
- [CreateGroupRequestRequestTypeDef](./type_defs.md#creategrouprequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateSamplingRuleRequestRequestTypeDef](./type_defs.md#createsamplingrulerequestrequesttypedef)
- [EdgeStatisticsTypeDef](./type_defs.md#edgestatisticstypedef)
- [ServiceStatisticsTypeDef](./type_defs.md#servicestatisticstypedef)
- [GetEncryptionConfigResultTypeDef](./type_defs.md#getencryptionconfigresulttypedef)
- [PutEncryptionConfigResultTypeDef](./type_defs.md#putencryptionconfigresulttypedef)
- [ErrorRootCauseEntityTypeDef](./type_defs.md#errorrootcauseentitytypedef)
- [FaultRootCauseEntityTypeDef](./type_defs.md#faultrootcauseentitytypedef)
- [GetInsightImpactGraphRequestRequestTypeDef](./type_defs.md#getinsightimpactgraphrequestrequesttypedef)
- [GetInsightSummariesRequestRequestTypeDef](./type_defs.md#getinsightsummariesrequestrequesttypedef)
- [GetServiceGraphRequestPaginateTypeDef](./type_defs.md#getservicegraphrequestpaginatetypedef)
- [GetServiceGraphRequestRequestTypeDef](./type_defs.md#getservicegraphrequestrequesttypedef)
- [GetTimeSeriesServiceStatisticsRequestPaginateTypeDef](./type_defs.md#gettimeseriesservicestatisticsrequestpaginatetypedef)
- [GetTimeSeriesServiceStatisticsRequestRequestTypeDef](./type_defs.md#gettimeseriesservicestatisticsrequestrequesttypedef)
- [SamplingStatisticsDocumentTypeDef](./type_defs.md#samplingstatisticsdocumenttypedef)
- [StartTraceRetrievalRequestRequestTypeDef](./type_defs.md#starttraceretrievalrequestrequesttypedef)
- [TelemetryRecordTypeDef](./type_defs.md#telemetryrecordtypedef)
- [GetSamplingStatisticSummariesResultTypeDef](./type_defs.md#getsamplingstatisticsummariesresulttypedef)
- [GetSamplingTargetsResultTypeDef](./type_defs.md#getsamplingtargetsresulttypedef)
- [GetTraceSummariesRequestPaginateTypeDef](./type_defs.md#gettracesummariesrequestpaginatetypedef)
- [GetTraceSummariesRequestRequestTypeDef](./type_defs.md#gettracesummariesrequestrequesttypedef)
- [IndexingRuleValueTypeDef](./type_defs.md#indexingrulevaluetypedef)
- [IndexingRuleValueUpdateTypeDef](./type_defs.md#indexingrulevalueupdatetypedef)
- [InsightImpactGraphServiceTypeDef](./type_defs.md#insightimpactgraphservicetypedef)
- [ListResourcePoliciesResultTypeDef](./type_defs.md#listresourcepoliciesresulttypedef)
- [PutResourcePolicyResultTypeDef](./type_defs.md#putresourcepolicyresulttypedef)
- [PutTraceSegmentsResultTypeDef](./type_defs.md#puttracesegmentsresulttypedef)
- [ResponseTimeRootCauseServiceTypeDef](./type_defs.md#responsetimerootcauseservicetypedef)
- [RetrievedTraceTypeDef](./type_defs.md#retrievedtracetypedef)
- [SamplingRuleRecordTypeDef](./type_defs.md#samplingrulerecordtypedef)
- [UpdateSamplingRuleRequestRequestTypeDef](./type_defs.md#updatesamplingrulerequestrequesttypedef)
- [TraceTypeDef](./type_defs.md#tracetypedef)
- [InsightEventTypeDef](./type_defs.md#insighteventtypedef)
- [InsightSummaryTypeDef](./type_defs.md#insightsummarytypedef)
- [InsightTypeDef](./type_defs.md#insighttypedef)
- [GetGroupsResultTypeDef](./type_defs.md#getgroupsresulttypedef)
- [CreateGroupResultTypeDef](./type_defs.md#creategroupresulttypedef)
- [GetGroupResultTypeDef](./type_defs.md#getgroupresulttypedef)
- [UpdateGroupResultTypeDef](./type_defs.md#updategroupresulttypedef)
- [EdgeTypeDef](./type_defs.md#edgetypedef)
- [TimeSeriesServiceStatisticsTypeDef](./type_defs.md#timeseriesservicestatisticstypedef)
- [ErrorRootCauseServiceTypeDef](./type_defs.md#errorrootcauseservicetypedef)
- [FaultRootCauseServiceTypeDef](./type_defs.md#faultrootcauseservicetypedef)
- [GetSamplingTargetsRequestRequestTypeDef](./type_defs.md#getsamplingtargetsrequestrequesttypedef)
- [PutTelemetryRecordsRequestRequestTypeDef](./type_defs.md#puttelemetryrecordsrequestrequesttypedef)
- [IndexingRuleTypeDef](./type_defs.md#indexingruletypedef)
- [UpdateIndexingRuleRequestRequestTypeDef](./type_defs.md#updateindexingrulerequestrequesttypedef)
- [GetInsightImpactGraphResultTypeDef](./type_defs.md#getinsightimpactgraphresulttypedef)
- [ResponseTimeRootCauseTypeDef](./type_defs.md#responsetimerootcausetypedef)
- [ListRetrievedTracesResultTypeDef](./type_defs.md#listretrievedtracesresulttypedef)
- [CreateSamplingRuleResultTypeDef](./type_defs.md#createsamplingruleresulttypedef)
- [DeleteSamplingRuleResultTypeDef](./type_defs.md#deletesamplingruleresulttypedef)
- [GetSamplingRulesResultTypeDef](./type_defs.md#getsamplingrulesresulttypedef)
- [UpdateSamplingRuleResultTypeDef](./type_defs.md#updatesamplingruleresulttypedef)
- [BatchGetTracesResultTypeDef](./type_defs.md#batchgettracesresulttypedef)
- [GetInsightEventsResultTypeDef](./type_defs.md#getinsighteventsresulttypedef)
- [GetInsightSummariesResultTypeDef](./type_defs.md#getinsightsummariesresulttypedef)
- [GetInsightResultTypeDef](./type_defs.md#getinsightresulttypedef)
- [ServiceTypeDef](./type_defs.md#servicetypedef)
- [GetTimeSeriesServiceStatisticsResultTypeDef](./type_defs.md#gettimeseriesservicestatisticsresulttypedef)
- [ErrorRootCauseTypeDef](./type_defs.md#errorrootcausetypedef)
- [FaultRootCauseTypeDef](./type_defs.md#faultrootcausetypedef)
- [GetIndexingRulesResultTypeDef](./type_defs.md#getindexingrulesresulttypedef)
- [UpdateIndexingRuleResultTypeDef](./type_defs.md#updateindexingruleresulttypedef)
- [GetServiceGraphResultTypeDef](./type_defs.md#getservicegraphresulttypedef)
- [GetTraceGraphResultTypeDef](./type_defs.md#gettracegraphresulttypedef)
- [RetrievedServiceTypeDef](./type_defs.md#retrievedservicetypedef)
- [TraceSummaryTypeDef](./type_defs.md#tracesummarytypedef)
- [GetRetrievedTracesGraphResultTypeDef](./type_defs.md#getretrievedtracesgraphresulttypedef)
- [GetTraceSummariesResultTypeDef](./type_defs.md#gettracesummariesresulttypedef)

