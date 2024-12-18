# DevOpsGuru module

> [Index](../README.md) > DevOpsGuru


!!! note ""

    Auto-generated documentation for [DevOpsGuru](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#devopsguru)
    type annotations stubs module [types-aiobotocore-devops-guru](https://pypi.org/project/types-aiobotocore-devops-guru/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `DevOpsGuru` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `DevOpsGuru` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[devops-guru]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[devops-guru]'

# standalone installation
python -m pip install types-aiobotocore-devops-guru
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-devops-guru
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DevOpsGuruClient

Type annotations and code completion for  `#!python session.create_client("devops-guru")` as [DevOpsGuruClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client)

```python
# DevOpsGuruClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.client import DevOpsGuruClient


session = get_session()
async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("devops-guru").get_paginator("...")`.

```python
# DescribeOrganizationResourceCollectionHealthPaginator usage example

from types_aiobotocore_devops_guru.paginator import DescribeOrganizationResourceCollectionHealthPaginator

def get_describe_organization_resource_collection_health_paginator() -> DescribeOrganizationResourceCollectionHealthPaginator:
    return client.get_paginator("describe_organization_resource_collection_health"))
```

- [DescribeOrganizationResourceCollectionHealthPaginator](./paginators.md#describeorganizationresourcecollectionhealthpaginator)
- [DescribeResourceCollectionHealthPaginator](./paginators.md#describeresourcecollectionhealthpaginator)
- [GetCostEstimationPaginator](./paginators.md#getcostestimationpaginator)
- [GetResourceCollectionPaginator](./paginators.md#getresourcecollectionpaginator)
- [ListAnomaliesForInsightPaginator](./paginators.md#listanomaliesforinsightpaginator)
- [ListAnomalousLogGroupsPaginator](./paginators.md#listanomalousloggroupspaginator)
- [ListEventsPaginator](./paginators.md#listeventspaginator)
- [ListInsightsPaginator](./paginators.md#listinsightspaginator)
- [ListMonitoredResourcesPaginator](./paginators.md#listmonitoredresourcespaginator)
- [ListNotificationChannelsPaginator](./paginators.md#listnotificationchannelspaginator)
- [ListOrganizationInsightsPaginator](./paginators.md#listorganizationinsightspaginator)
- [ListRecommendationsPaginator](./paginators.md#listrecommendationspaginator)
- [SearchInsightsPaginator](./paginators.md#searchinsightspaginator)
- [SearchOrganizationInsightsPaginator](./paginators.md#searchorganizationinsightspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AnomalySeverityType usage example

from types_aiobotocore_devops_guru.literals import AnomalySeverityType

def get_value() -> AnomalySeverityType:
    return "HIGH"
```

- [AnomalySeverityType](./literals.md#anomalyseveritytype)
- [AnomalyStatusType](./literals.md#anomalystatustype)
- [AnomalyTypeType](./literals.md#anomalytypetype)
- [CloudWatchMetricDataStatusCodeType](./literals.md#cloudwatchmetricdatastatuscodetype)
- [CloudWatchMetricsStatType](./literals.md#cloudwatchmetricsstattype)
- [CostEstimationServiceResourceStateType](./literals.md#costestimationserviceresourcestatetype)
- [CostEstimationStatusType](./literals.md#costestimationstatustype)
- [DescribeOrganizationResourceCollectionHealthPaginatorName](./literals.md#describeorganizationresourcecollectionhealthpaginatorname)
- [DescribeResourceCollectionHealthPaginatorName](./literals.md#describeresourcecollectionhealthpaginatorname)
- [EventClassType](./literals.md#eventclasstype)
- [EventDataSourceType](./literals.md#eventdatasourcetype)
- [EventSourceOptInStatusType](./literals.md#eventsourceoptinstatustype)
- [GetCostEstimationPaginatorName](./literals.md#getcostestimationpaginatorname)
- [GetResourceCollectionPaginatorName](./literals.md#getresourcecollectionpaginatorname)
- [InsightFeedbackOptionType](./literals.md#insightfeedbackoptiontype)
- [InsightSeverityType](./literals.md#insightseveritytype)
- [InsightStatusType](./literals.md#insightstatustype)
- [InsightTypeType](./literals.md#insighttypetype)
- [ListAnomaliesForInsightPaginatorName](./literals.md#listanomaliesforinsightpaginatorname)
- [ListAnomalousLogGroupsPaginatorName](./literals.md#listanomalousloggroupspaginatorname)
- [ListEventsPaginatorName](./literals.md#listeventspaginatorname)
- [ListInsightsPaginatorName](./literals.md#listinsightspaginatorname)
- [ListMonitoredResourcesPaginatorName](./literals.md#listmonitoredresourcespaginatorname)
- [ListNotificationChannelsPaginatorName](./literals.md#listnotificationchannelspaginatorname)
- [ListOrganizationInsightsPaginatorName](./literals.md#listorganizationinsightspaginatorname)
- [ListRecommendationsPaginatorName](./literals.md#listrecommendationspaginatorname)
- [LocaleType](./literals.md#localetype)
- [LogAnomalyTypeType](./literals.md#loganomalytypetype)
- [NotificationMessageTypeType](./literals.md#notificationmessagetypetype)
- [OptInStatusType](./literals.md#optinstatustype)
- [OrganizationResourceCollectionTypeType](./literals.md#organizationresourcecollectiontypetype)
- [ResourceCollectionTypeType](./literals.md#resourcecollectiontypetype)
- [ResourcePermissionType](./literals.md#resourcepermissiontype)
- [ResourceTypeFilterType](./literals.md#resourcetypefiltertype)
- [SearchInsightsPaginatorName](./literals.md#searchinsightspaginatorname)
- [SearchOrganizationInsightsPaginatorName](./literals.md#searchorganizationinsightspaginatorname)
- [ServerSideEncryptionTypeType](./literals.md#serversideencryptiontypetype)
- [ServiceNameType](./literals.md#servicenametype)
- [UpdateResourceCollectionActionType](./literals.md#updateresourcecollectionactiontype)
- [DevOpsGuruServiceName](./literals.md#devopsguruservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountInsightHealthTypeDef](./type_defs.md#accountinsighthealthtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AmazonCodeGuruProfilerIntegrationTypeDef](./type_defs.md#amazoncodeguruprofilerintegrationtypedef)
- [AnomalyReportedTimeRangeTypeDef](./type_defs.md#anomalyreportedtimerangetypedef)
- [AnomalyResourceTypeDef](./type_defs.md#anomalyresourcetypedef)
- [AnomalySourceMetadataTypeDef](./type_defs.md#anomalysourcemetadatatypedef)
- [AnomalyTimeRangeTypeDef](./type_defs.md#anomalytimerangetypedef)
- [CloudFormationCollectionFilterTypeDef](./type_defs.md#cloudformationcollectionfiltertypedef)
- [CloudFormationCollectionOutputTypeDef](./type_defs.md#cloudformationcollectionoutputtypedef)
- [CloudFormationCollectionTypeDef](./type_defs.md#cloudformationcollectiontypedef)
- [CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef](./type_defs.md#cloudformationcostestimationresourcecollectionfilteroutputtypedef)
- [CloudFormationCostEstimationResourceCollectionFilterTypeDef](./type_defs.md#cloudformationcostestimationresourcecollectionfiltertypedef)
- [InsightHealthTypeDef](./type_defs.md#insighthealthtypedef)
- [TimestampMetricValuePairTypeDef](./type_defs.md#timestampmetricvaluepairtypedef)
- [CloudWatchMetricsDimensionTypeDef](./type_defs.md#cloudwatchmetricsdimensiontypedef)
- [TagCostEstimationResourceCollectionFilterOutputTypeDef](./type_defs.md#tagcostestimationresourcecollectionfilteroutputtypedef)
- [CostEstimationTimeRangeTypeDef](./type_defs.md#costestimationtimerangetypedef)
- [DeleteInsightRequestRequestTypeDef](./type_defs.md#deleteinsightrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [DescribeAnomalyRequestRequestTypeDef](./type_defs.md#describeanomalyrequestrequesttypedef)
- [DescribeFeedbackRequestRequestTypeDef](./type_defs.md#describefeedbackrequestrequesttypedef)
- [InsightFeedbackTypeDef](./type_defs.md#insightfeedbacktypedef)
- [DescribeInsightRequestRequestTypeDef](./type_defs.md#describeinsightrequestrequesttypedef)
- [DescribeOrganizationHealthRequestRequestTypeDef](./type_defs.md#describeorganizationhealthrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef](./type_defs.md#describeorganizationresourcecollectionhealthrequestrequesttypedef)
- [DescribeResourceCollectionHealthRequestRequestTypeDef](./type_defs.md#describeresourcecollectionhealthrequestrequesttypedef)
- [EventResourceTypeDef](./type_defs.md#eventresourcetypedef)
- [GetCostEstimationRequestRequestTypeDef](./type_defs.md#getcostestimationrequestrequesttypedef)
- [ServiceResourceCostTypeDef](./type_defs.md#serviceresourcecosttypedef)
- [GetResourceCollectionRequestRequestTypeDef](./type_defs.md#getresourcecollectionrequestrequesttypedef)
- [InsightTimeRangeTypeDef](./type_defs.md#insighttimerangetypedef)
- [KMSServerSideEncryptionIntegrationConfigTypeDef](./type_defs.md#kmsserversideencryptionintegrationconfigtypedef)
- [KMSServerSideEncryptionIntegrationTypeDef](./type_defs.md#kmsserversideencryptionintegrationtypedef)
- [ServiceCollectionTypeDef](./type_defs.md#servicecollectiontypedef)
- [ListAnomalousLogGroupsRequestRequestTypeDef](./type_defs.md#listanomalousloggroupsrequestrequesttypedef)
- [ListInsightsOngoingStatusFilterTypeDef](./type_defs.md#listinsightsongoingstatusfiltertypedef)
- [ListMonitoredResourcesFiltersTypeDef](./type_defs.md#listmonitoredresourcesfilterstypedef)
- [ListNotificationChannelsRequestRequestTypeDef](./type_defs.md#listnotificationchannelsrequestrequesttypedef)
- [ListRecommendationsRequestRequestTypeDef](./type_defs.md#listrecommendationsrequestrequesttypedef)
- [LogAnomalyClassTypeDef](./type_defs.md#loganomalyclasstypedef)
- [LogsAnomalyDetectionIntegrationConfigTypeDef](./type_defs.md#logsanomalydetectionintegrationconfigtypedef)
- [LogsAnomalyDetectionIntegrationTypeDef](./type_defs.md#logsanomalydetectionintegrationtypedef)
- [NotificationFilterConfigOutputTypeDef](./type_defs.md#notificationfilterconfigoutputtypedef)
- [SnsChannelConfigTypeDef](./type_defs.md#snschannelconfigtypedef)
- [NotificationFilterConfigTypeDef](./type_defs.md#notificationfilterconfigtypedef)
- [OpsCenterIntegrationConfigTypeDef](./type_defs.md#opscenterintegrationconfigtypedef)
- [OpsCenterIntegrationTypeDef](./type_defs.md#opscenterintegrationtypedef)
- [PerformanceInsightsMetricDimensionGroupTypeDef](./type_defs.md#performanceinsightsmetricdimensiongrouptypedef)
- [PerformanceInsightsStatTypeDef](./type_defs.md#performanceinsightsstattypedef)
- [PerformanceInsightsReferenceScalarTypeDef](./type_defs.md#performanceinsightsreferencescalartypedef)
- [PredictionTimeRangeTypeDef](./type_defs.md#predictiontimerangetypedef)
- [ServiceCollectionOutputTypeDef](./type_defs.md#servicecollectionoutputtypedef)
- [RecommendationRelatedAnomalyResourceTypeDef](./type_defs.md#recommendationrelatedanomalyresourcetypedef)
- [RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef](./type_defs.md#recommendationrelatedcloudwatchmetricssourcedetailtypedef)
- [RecommendationRelatedEventResourceTypeDef](./type_defs.md#recommendationrelatedeventresourcetypedef)
- [RemoveNotificationChannelRequestRequestTypeDef](./type_defs.md#removenotificationchannelrequestrequesttypedef)
- [TagCollectionFilterTypeDef](./type_defs.md#tagcollectionfiltertypedef)
- [TagCollectionOutputTypeDef](./type_defs.md#tagcollectionoutputtypedef)
- [TagCollectionTypeDef](./type_defs.md#tagcollectiontypedef)
- [ServiceInsightHealthTypeDef](./type_defs.md#serviceinsighthealthtypedef)
- [TagCostEstimationResourceCollectionFilterTypeDef](./type_defs.md#tagcostestimationresourcecollectionfiltertypedef)
- [UpdateCloudFormationCollectionFilterTypeDef](./type_defs.md#updatecloudformationcollectionfiltertypedef)
- [UpdateTagCollectionFilterTypeDef](./type_defs.md#updatetagcollectionfiltertypedef)
- [AccountHealthTypeDef](./type_defs.md#accounthealthtypedef)
- [AddNotificationChannelResponseTypeDef](./type_defs.md#addnotificationchannelresponsetypedef)
- [DescribeAccountHealthResponseTypeDef](./type_defs.md#describeaccounthealthresponsetypedef)
- [DescribeAccountOverviewResponseTypeDef](./type_defs.md#describeaccountoverviewresponsetypedef)
- [DescribeOrganizationHealthResponseTypeDef](./type_defs.md#describeorganizationhealthresponsetypedef)
- [DescribeOrganizationOverviewResponseTypeDef](./type_defs.md#describeorganizationoverviewresponsetypedef)
- [EventSourcesConfigTypeDef](./type_defs.md#eventsourcesconfigtypedef)
- [CloudFormationCostEstimationResourceCollectionFilterUnionTypeDef](./type_defs.md#cloudformationcostestimationresourcecollectionfilteruniontypedef)
- [CloudFormationHealthTypeDef](./type_defs.md#cloudformationhealthtypedef)
- [TagHealthTypeDef](./type_defs.md#taghealthtypedef)
- [CloudWatchMetricsDataSummaryTypeDef](./type_defs.md#cloudwatchmetricsdatasummarytypedef)
- [CostEstimationResourceCollectionFilterOutputTypeDef](./type_defs.md#costestimationresourcecollectionfilteroutputtypedef)
- [DescribeAccountOverviewRequestRequestTypeDef](./type_defs.md#describeaccountoverviewrequestrequesttypedef)
- [DescribeOrganizationOverviewRequestRequestTypeDef](./type_defs.md#describeorganizationoverviewrequestrequesttypedef)
- [EndTimeRangeTypeDef](./type_defs.md#endtimerangetypedef)
- [EventTimeRangeTypeDef](./type_defs.md#eventtimerangetypedef)
- [StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef)
- [DescribeFeedbackResponseTypeDef](./type_defs.md#describefeedbackresponsetypedef)
- [PutFeedbackRequestRequestTypeDef](./type_defs.md#putfeedbackrequestrequesttypedef)
- [DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef](./type_defs.md#describeorganizationresourcecollectionhealthrequestdescribeorganizationresourcecollectionhealthpaginatetypedef)
- [DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef](./type_defs.md#describeresourcecollectionhealthrequestdescriberesourcecollectionhealthpaginatetypedef)
- [GetCostEstimationRequestGetCostEstimationPaginateTypeDef](./type_defs.md#getcostestimationrequestgetcostestimationpaginatetypedef)
- [GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef](./type_defs.md#getresourcecollectionrequestgetresourcecollectionpaginatetypedef)
- [ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef](./type_defs.md#listanomalousloggroupsrequestlistanomalousloggroupspaginatetypedef)
- [ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef](./type_defs.md#listnotificationchannelsrequestlistnotificationchannelspaginatetypedef)
- [ListRecommendationsRequestListRecommendationsPaginateTypeDef](./type_defs.md#listrecommendationsrequestlistrecommendationspaginatetypedef)
- [ListAnomaliesForInsightFiltersTypeDef](./type_defs.md#listanomaliesforinsightfilterstypedef)
- [ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef](./type_defs.md#listmonitoredresourcesrequestlistmonitoredresourcespaginatetypedef)
- [ListMonitoredResourcesRequestRequestTypeDef](./type_defs.md#listmonitoredresourcesrequestrequesttypedef)
- [LogAnomalyShowcaseTypeDef](./type_defs.md#loganomalyshowcasetypedef)
- [NotificationChannelConfigOutputTypeDef](./type_defs.md#notificationchannelconfigoutputtypedef)
- [NotificationFilterConfigUnionTypeDef](./type_defs.md#notificationfilterconfiguniontypedef)
- [UpdateServiceIntegrationConfigTypeDef](./type_defs.md#updateserviceintegrationconfigtypedef)
- [ServiceIntegrationConfigTypeDef](./type_defs.md#serviceintegrationconfigtypedef)
- [PerformanceInsightsMetricQueryTypeDef](./type_defs.md#performanceinsightsmetricquerytypedef)
- [ServiceCollectionUnionTypeDef](./type_defs.md#servicecollectionuniontypedef)
- [RecommendationRelatedAnomalySourceDetailTypeDef](./type_defs.md#recommendationrelatedanomalysourcedetailtypedef)
- [RecommendationRelatedEventTypeDef](./type_defs.md#recommendationrelatedeventtypedef)
- [ResourceCollectionFilterTypeDef](./type_defs.md#resourcecollectionfiltertypedef)
- [ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef)
- [ResourceCollectionTypeDef](./type_defs.md#resourcecollectiontypedef)
- [ServiceHealthTypeDef](./type_defs.md#servicehealthtypedef)
- [TagCostEstimationResourceCollectionFilterUnionTypeDef](./type_defs.md#tagcostestimationresourcecollectionfilteruniontypedef)
- [UpdateResourceCollectionFilterTypeDef](./type_defs.md#updateresourcecollectionfiltertypedef)
- [DescribeEventSourcesConfigResponseTypeDef](./type_defs.md#describeeventsourcesconfigresponsetypedef)
- [UpdateEventSourcesConfigRequestRequestTypeDef](./type_defs.md#updateeventsourcesconfigrequestrequesttypedef)
- [CloudWatchMetricsDetailTypeDef](./type_defs.md#cloudwatchmetricsdetailtypedef)
- [GetCostEstimationResponseTypeDef](./type_defs.md#getcostestimationresponsetypedef)
- [ListInsightsClosedStatusFilterTypeDef](./type_defs.md#listinsightsclosedstatusfiltertypedef)
- [ListInsightsAnyStatusFilterTypeDef](./type_defs.md#listinsightsanystatusfiltertypedef)
- [ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef](./type_defs.md#listanomaliesforinsightrequestlistanomaliesforinsightpaginatetypedef)
- [ListAnomaliesForInsightRequestRequestTypeDef](./type_defs.md#listanomaliesforinsightrequestrequesttypedef)
- [AnomalousLogGroupTypeDef](./type_defs.md#anomalousloggrouptypedef)
- [NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef)
- [NotificationChannelConfigTypeDef](./type_defs.md#notificationchannelconfigtypedef)
- [UpdateServiceIntegrationRequestRequestTypeDef](./type_defs.md#updateserviceintegrationrequestrequesttypedef)
- [DescribeServiceIntegrationResponseTypeDef](./type_defs.md#describeserviceintegrationresponsetypedef)
- [PerformanceInsightsReferenceMetricTypeDef](./type_defs.md#performanceinsightsreferencemetrictypedef)
- [RecommendationRelatedAnomalyTypeDef](./type_defs.md#recommendationrelatedanomalytypedef)
- [GetResourceCollectionResponseTypeDef](./type_defs.md#getresourcecollectionresponsetypedef)
- [EventTypeDef](./type_defs.md#eventtypedef)
- [MonitoredResourceIdentifierTypeDef](./type_defs.md#monitoredresourceidentifiertypedef)
- [ProactiveInsightSummaryTypeDef](./type_defs.md#proactiveinsightsummarytypedef)
- [ProactiveInsightTypeDef](./type_defs.md#proactiveinsighttypedef)
- [ProactiveOrganizationInsightSummaryTypeDef](./type_defs.md#proactiveorganizationinsightsummarytypedef)
- [ReactiveInsightSummaryTypeDef](./type_defs.md#reactiveinsightsummarytypedef)
- [ReactiveInsightTypeDef](./type_defs.md#reactiveinsighttypedef)
- [ReactiveOrganizationInsightSummaryTypeDef](./type_defs.md#reactiveorganizationinsightsummarytypedef)
- [ListEventsFiltersTypeDef](./type_defs.md#listeventsfilterstypedef)
- [ResourceCollectionUnionTypeDef](./type_defs.md#resourcecollectionuniontypedef)
- [DescribeOrganizationResourceCollectionHealthResponseTypeDef](./type_defs.md#describeorganizationresourcecollectionhealthresponsetypedef)
- [DescribeResourceCollectionHealthResponseTypeDef](./type_defs.md#describeresourcecollectionhealthresponsetypedef)
- [CostEstimationResourceCollectionFilterTypeDef](./type_defs.md#costestimationresourcecollectionfiltertypedef)
- [UpdateResourceCollectionRequestRequestTypeDef](./type_defs.md#updateresourcecollectionrequestrequesttypedef)
- [ListInsightsStatusFilterTypeDef](./type_defs.md#listinsightsstatusfiltertypedef)
- [ListAnomalousLogGroupsResponseTypeDef](./type_defs.md#listanomalousloggroupsresponsetypedef)
- [ListNotificationChannelsResponseTypeDef](./type_defs.md#listnotificationchannelsresponsetypedef)
- [AddNotificationChannelRequestRequestTypeDef](./type_defs.md#addnotificationchannelrequestrequesttypedef)
- [PerformanceInsightsReferenceComparisonValuesTypeDef](./type_defs.md#performanceinsightsreferencecomparisonvaluestypedef)
- [RecommendationTypeDef](./type_defs.md#recommendationtypedef)
- [ListEventsResponseTypeDef](./type_defs.md#listeventsresponsetypedef)
- [ListMonitoredResourcesResponseTypeDef](./type_defs.md#listmonitoredresourcesresponsetypedef)
- [ListInsightsResponseTypeDef](./type_defs.md#listinsightsresponsetypedef)
- [SearchInsightsResponseTypeDef](./type_defs.md#searchinsightsresponsetypedef)
- [SearchOrganizationInsightsResponseTypeDef](./type_defs.md#searchorganizationinsightsresponsetypedef)
- [DescribeInsightResponseTypeDef](./type_defs.md#describeinsightresponsetypedef)
- [ListOrganizationInsightsResponseTypeDef](./type_defs.md#listorganizationinsightsresponsetypedef)
- [ListEventsRequestListEventsPaginateTypeDef](./type_defs.md#listeventsrequestlisteventspaginatetypedef)
- [ListEventsRequestRequestTypeDef](./type_defs.md#listeventsrequestrequesttypedef)
- [SearchInsightsFiltersTypeDef](./type_defs.md#searchinsightsfilterstypedef)
- [SearchOrganizationInsightsFiltersTypeDef](./type_defs.md#searchorganizationinsightsfilterstypedef)
- [StartCostEstimationRequestRequestTypeDef](./type_defs.md#startcostestimationrequestrequesttypedef)
- [ListInsightsRequestListInsightsPaginateTypeDef](./type_defs.md#listinsightsrequestlistinsightspaginatetypedef)
- [ListInsightsRequestRequestTypeDef](./type_defs.md#listinsightsrequestrequesttypedef)
- [ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef](./type_defs.md#listorganizationinsightsrequestlistorganizationinsightspaginatetypedef)
- [ListOrganizationInsightsRequestRequestTypeDef](./type_defs.md#listorganizationinsightsrequestrequesttypedef)
- [PerformanceInsightsReferenceDataTypeDef](./type_defs.md#performanceinsightsreferencedatatypedef)
- [ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef)
- [SearchInsightsRequestRequestTypeDef](./type_defs.md#searchinsightsrequestrequesttypedef)
- [SearchInsightsRequestSearchInsightsPaginateTypeDef](./type_defs.md#searchinsightsrequestsearchinsightspaginatetypedef)
- [SearchOrganizationInsightsRequestRequestTypeDef](./type_defs.md#searchorganizationinsightsrequestrequesttypedef)
- [SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef](./type_defs.md#searchorganizationinsightsrequestsearchorganizationinsightspaginatetypedef)
- [PerformanceInsightsMetricsDetailTypeDef](./type_defs.md#performanceinsightsmetricsdetailtypedef)
- [AnomalySourceDetailsTypeDef](./type_defs.md#anomalysourcedetailstypedef)
- [ProactiveAnomalySummaryTypeDef](./type_defs.md#proactiveanomalysummarytypedef)
- [ProactiveAnomalyTypeDef](./type_defs.md#proactiveanomalytypedef)
- [ReactiveAnomalySummaryTypeDef](./type_defs.md#reactiveanomalysummarytypedef)
- [ReactiveAnomalyTypeDef](./type_defs.md#reactiveanomalytypedef)
- [ListAnomaliesForInsightResponseTypeDef](./type_defs.md#listanomaliesforinsightresponsetypedef)
- [DescribeAnomalyResponseTypeDef](./type_defs.md#describeanomalyresponsetypedef)

