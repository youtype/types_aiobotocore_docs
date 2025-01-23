# CloudTrail module

> [Index](../README.md) > CloudTrail


!!! note ""

    Auto-generated documentation for [CloudTrail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#cloudtrail)
    type annotations stubs module [types-aiobotocore-cloudtrail](https://pypi.org/project/types-aiobotocore-cloudtrail/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudTrail` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CloudTrail` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cloudtrail]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cloudtrail]'

# standalone installation
python -m pip install types-aiobotocore-cloudtrail
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cloudtrail
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudTrailClient

Type annotations and code completion for  `#!python session.create_client("cloudtrail")` as [CloudTrailClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client)

```python
# CloudTrailClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail.client import CloudTrailClient


session = get_session()
async with session.create_client("cloudtrail") as client:
    client: CloudTrailClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("cloudtrail").get_paginator("...")`.

```python
# ListImportFailuresPaginator usage example

from types_aiobotocore_cloudtrail.paginator import ListImportFailuresPaginator

def get_list_import_failures_paginator() -> ListImportFailuresPaginator:
    return client.get_paginator("list_import_failures"))
```

- [ListImportFailuresPaginator](./paginators.md#listimportfailurespaginator)
- [ListImportsPaginator](./paginators.md#listimportspaginator)
- [ListPublicKeysPaginator](./paginators.md#listpublickeyspaginator)
- [ListTagsPaginator](./paginators.md#listtagspaginator)
- [ListTrailsPaginator](./paginators.md#listtrailspaginator)
- [LookupEventsPaginator](./paginators.md#lookupeventspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BillingModeType usage example

from types_aiobotocore_cloudtrail.literals import BillingModeType

def get_value() -> BillingModeType:
    return "EXTENDABLE_RETENTION_PRICING"
```

- [BillingModeType](./literals.md#billingmodetype)
- [DashboardStatusType](./literals.md#dashboardstatustype)
- [DashboardTypeType](./literals.md#dashboardtypetype)
- [DeliveryStatusType](./literals.md#deliverystatustype)
- [DestinationTypeType](./literals.md#destinationtypetype)
- [EventCategoryType](./literals.md#eventcategorytype)
- [EventDataStoreStatusType](./literals.md#eventdatastorestatustype)
- [FederationStatusType](./literals.md#federationstatustype)
- [ImportFailureStatusType](./literals.md#importfailurestatustype)
- [ImportStatusType](./literals.md#importstatustype)
- [InsightTypeType](./literals.md#insighttypetype)
- [InsightsMetricDataTypeType](./literals.md#insightsmetricdatatypetype)
- [ListImportFailuresPaginatorName](./literals.md#listimportfailurespaginatorname)
- [ListImportsPaginatorName](./literals.md#listimportspaginatorname)
- [ListPublicKeysPaginatorName](./literals.md#listpublickeyspaginatorname)
- [ListTagsPaginatorName](./literals.md#listtagspaginatorname)
- [ListTrailsPaginatorName](./literals.md#listtrailspaginatorname)
- [LookupAttributeKeyType](./literals.md#lookupattributekeytype)
- [LookupEventsPaginatorName](./literals.md#lookupeventspaginatorname)
- [QueryStatusType](./literals.md#querystatustype)
- [ReadWriteTypeType](./literals.md#readwritetypetype)
- [RefreshScheduleFrequencyUnitType](./literals.md#refreshschedulefrequencyunittype)
- [RefreshScheduleStatusType](./literals.md#refreshschedulestatustype)
- [CloudTrailServiceName](./literals.md#cloudtrailservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TagTypeDef](./type_defs.md#tagtypedef)
- [AdvancedFieldSelectorOutputTypeDef](./type_defs.md#advancedfieldselectoroutputtypedef)
- [AdvancedFieldSelectorTypeDef](./type_defs.md#advancedfieldselectortypedef)
- [CancelQueryRequestRequestTypeDef](./type_defs.md#cancelqueryrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ChannelTypeDef](./type_defs.md#channeltypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [RequestWidgetTypeDef](./type_defs.md#requestwidgettypedef)
- [WidgetTypeDef](./type_defs.md#widgettypedef)
- [DashboardDetailTypeDef](./type_defs.md#dashboarddetailtypedef)
- [DataResourceOutputTypeDef](./type_defs.md#dataresourceoutputtypedef)
- [DataResourceTypeDef](./type_defs.md#dataresourcetypedef)
- [DeleteChannelRequestRequestTypeDef](./type_defs.md#deletechannelrequestrequesttypedef)
- [DeleteDashboardRequestRequestTypeDef](./type_defs.md#deletedashboardrequestrequesttypedef)
- [DeleteEventDataStoreRequestRequestTypeDef](./type_defs.md#deleteeventdatastorerequestrequesttypedef)
- [DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef)
- [DeleteTrailRequestRequestTypeDef](./type_defs.md#deletetrailrequestrequesttypedef)
- [DeregisterOrganizationDelegatedAdminRequestRequestTypeDef](./type_defs.md#deregisterorganizationdelegatedadminrequestrequesttypedef)
- [DescribeQueryRequestRequestTypeDef](./type_defs.md#describequeryrequestrequesttypedef)
- [QueryStatisticsForDescribeQueryTypeDef](./type_defs.md#querystatisticsfordescribequerytypedef)
- [DescribeTrailsRequestRequestTypeDef](./type_defs.md#describetrailsrequestrequesttypedef)
- [TrailTypeDef](./type_defs.md#trailtypedef)
- [DisableFederationRequestRequestTypeDef](./type_defs.md#disablefederationrequestrequesttypedef)
- [EnableFederationRequestRequestTypeDef](./type_defs.md#enablefederationrequestrequesttypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [GenerateQueryRequestRequestTypeDef](./type_defs.md#generatequeryrequestrequesttypedef)
- [GetChannelRequestRequestTypeDef](./type_defs.md#getchannelrequestrequesttypedef)
- [IngestionStatusTypeDef](./type_defs.md#ingestionstatustypedef)
- [GetDashboardRequestRequestTypeDef](./type_defs.md#getdashboardrequestrequesttypedef)
- [GetEventDataStoreRequestRequestTypeDef](./type_defs.md#geteventdatastorerequestrequesttypedef)
- [PartitionKeyTypeDef](./type_defs.md#partitionkeytypedef)
- [GetEventSelectorsRequestRequestTypeDef](./type_defs.md#geteventselectorsrequestrequesttypedef)
- [GetImportRequestRequestTypeDef](./type_defs.md#getimportrequestrequesttypedef)
- [ImportStatisticsTypeDef](./type_defs.md#importstatisticstypedef)
- [GetInsightSelectorsRequestRequestTypeDef](./type_defs.md#getinsightselectorsrequestrequesttypedef)
- [InsightSelectorTypeDef](./type_defs.md#insightselectortypedef)
- [GetQueryResultsRequestRequestTypeDef](./type_defs.md#getqueryresultsrequestrequesttypedef)
- [QueryStatisticsTypeDef](./type_defs.md#querystatisticstypedef)
- [GetResourcePolicyRequestRequestTypeDef](./type_defs.md#getresourcepolicyrequestrequesttypedef)
- [GetTrailRequestRequestTypeDef](./type_defs.md#gettrailrequestrequesttypedef)
- [GetTrailStatusRequestRequestTypeDef](./type_defs.md#gettrailstatusrequestrequesttypedef)
- [ImportFailureListItemTypeDef](./type_defs.md#importfailurelistitemtypedef)
- [S3ImportSourceTypeDef](./type_defs.md#s3importsourcetypedef)
- [ImportsListItemTypeDef](./type_defs.md#importslistitemtypedef)
- [ListChannelsRequestRequestTypeDef](./type_defs.md#listchannelsrequestrequesttypedef)
- [ListDashboardsRequestRequestTypeDef](./type_defs.md#listdashboardsrequestrequesttypedef)
- [ListEventDataStoresRequestRequestTypeDef](./type_defs.md#listeventdatastoresrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListImportFailuresRequestRequestTypeDef](./type_defs.md#listimportfailuresrequestrequesttypedef)
- [ListImportsRequestRequestTypeDef](./type_defs.md#listimportsrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [PublicKeyTypeDef](./type_defs.md#publickeytypedef)
- [QueryTypeDef](./type_defs.md#querytypedef)
- [ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef)
- [ListTrailsRequestRequestTypeDef](./type_defs.md#listtrailsrequestrequesttypedef)
- [TrailInfoTypeDef](./type_defs.md#trailinfotypedef)
- [LookupAttributeTypeDef](./type_defs.md#lookupattributetypedef)
- [PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef)
- [RefreshScheduleFrequencyTypeDef](./type_defs.md#refreshschedulefrequencytypedef)
- [RegisterOrganizationDelegatedAdminRequestRequestTypeDef](./type_defs.md#registerorganizationdelegatedadminrequestrequesttypedef)
- [RestoreEventDataStoreRequestRequestTypeDef](./type_defs.md#restoreeventdatastorerequestrequesttypedef)
- [StartDashboardRefreshRequestRequestTypeDef](./type_defs.md#startdashboardrefreshrequestrequesttypedef)
- [StartEventDataStoreIngestionRequestRequestTypeDef](./type_defs.md#starteventdatastoreingestionrequestrequesttypedef)
- [StartLoggingRequestRequestTypeDef](./type_defs.md#startloggingrequestrequesttypedef)
- [StartQueryRequestRequestTypeDef](./type_defs.md#startqueryrequestrequesttypedef)
- [StopEventDataStoreIngestionRequestRequestTypeDef](./type_defs.md#stopeventdatastoreingestionrequestrequesttypedef)
- [StopImportRequestRequestTypeDef](./type_defs.md#stopimportrequestrequesttypedef)
- [StopLoggingRequestRequestTypeDef](./type_defs.md#stoploggingrequestrequesttypedef)
- [UpdateTrailRequestRequestTypeDef](./type_defs.md#updatetrailrequestrequesttypedef)
- [AddTagsRequestRequestTypeDef](./type_defs.md#addtagsrequestrequesttypedef)
- [CreateTrailRequestRequestTypeDef](./type_defs.md#createtrailrequestrequesttypedef)
- [RemoveTagsRequestRequestTypeDef](./type_defs.md#removetagsrequestrequesttypedef)
- [ResourceTagTypeDef](./type_defs.md#resourcetagtypedef)
- [AdvancedEventSelectorOutputTypeDef](./type_defs.md#advancedeventselectoroutputtypedef)
- [AdvancedFieldSelectorUnionTypeDef](./type_defs.md#advancedfieldselectoruniontypedef)
- [CancelQueryResponseTypeDef](./type_defs.md#cancelqueryresponsetypedef)
- [CreateTrailResponseTypeDef](./type_defs.md#createtrailresponsetypedef)
- [DisableFederationResponseTypeDef](./type_defs.md#disablefederationresponsetypedef)
- [EnableFederationResponseTypeDef](./type_defs.md#enablefederationresponsetypedef)
- [GenerateQueryResponseTypeDef](./type_defs.md#generatequeryresponsetypedef)
- [GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef)
- [GetTrailStatusResponseTypeDef](./type_defs.md#gettrailstatusresponsetypedef)
- [ListInsightsMetricDataResponseTypeDef](./type_defs.md#listinsightsmetricdataresponsetypedef)
- [PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef)
- [StartDashboardRefreshResponseTypeDef](./type_defs.md#startdashboardrefreshresponsetypedef)
- [StartQueryResponseTypeDef](./type_defs.md#startqueryresponsetypedef)
- [UpdateTrailResponseTypeDef](./type_defs.md#updatetrailresponsetypedef)
- [ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)
- [CreateChannelRequestRequestTypeDef](./type_defs.md#createchannelrequestrequesttypedef)
- [CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef)
- [UpdateChannelRequestRequestTypeDef](./type_defs.md#updatechannelrequestrequesttypedef)
- [UpdateChannelResponseTypeDef](./type_defs.md#updatechannelresponsetypedef)
- [ListDashboardsResponseTypeDef](./type_defs.md#listdashboardsresponsetypedef)
- [EventSelectorOutputTypeDef](./type_defs.md#eventselectoroutputtypedef)
- [DataResourceUnionTypeDef](./type_defs.md#dataresourceuniontypedef)
- [DescribeQueryResponseTypeDef](./type_defs.md#describequeryresponsetypedef)
- [DescribeTrailsResponseTypeDef](./type_defs.md#describetrailsresponsetypedef)
- [GetTrailResponseTypeDef](./type_defs.md#gettrailresponsetypedef)
- [EventTypeDef](./type_defs.md#eventtypedef)
- [GetInsightSelectorsResponseTypeDef](./type_defs.md#getinsightselectorsresponsetypedef)
- [PutInsightSelectorsRequestRequestTypeDef](./type_defs.md#putinsightselectorsrequestrequesttypedef)
- [PutInsightSelectorsResponseTypeDef](./type_defs.md#putinsightselectorsresponsetypedef)
- [GetQueryResultsResponseTypeDef](./type_defs.md#getqueryresultsresponsetypedef)
- [ListImportFailuresResponseTypeDef](./type_defs.md#listimportfailuresresponsetypedef)
- [ImportSourceTypeDef](./type_defs.md#importsourcetypedef)
- [ListImportsResponseTypeDef](./type_defs.md#listimportsresponsetypedef)
- [ListImportFailuresRequestPaginateTypeDef](./type_defs.md#listimportfailuresrequestpaginatetypedef)
- [ListImportsRequestPaginateTypeDef](./type_defs.md#listimportsrequestpaginatetypedef)
- [ListTagsRequestPaginateTypeDef](./type_defs.md#listtagsrequestpaginatetypedef)
- [ListTrailsRequestPaginateTypeDef](./type_defs.md#listtrailsrequestpaginatetypedef)
- [ListInsightsMetricDataRequestRequestTypeDef](./type_defs.md#listinsightsmetricdatarequestrequesttypedef)
- [ListPublicKeysRequestPaginateTypeDef](./type_defs.md#listpublickeysrequestpaginatetypedef)
- [ListPublicKeysRequestRequestTypeDef](./type_defs.md#listpublickeysrequestrequesttypedef)
- [ListQueriesRequestRequestTypeDef](./type_defs.md#listqueriesrequestrequesttypedef)
- [ListPublicKeysResponseTypeDef](./type_defs.md#listpublickeysresponsetypedef)
- [ListQueriesResponseTypeDef](./type_defs.md#listqueriesresponsetypedef)
- [ListTrailsResponseTypeDef](./type_defs.md#listtrailsresponsetypedef)
- [LookupEventsRequestPaginateTypeDef](./type_defs.md#lookupeventsrequestpaginatetypedef)
- [LookupEventsRequestRequestTypeDef](./type_defs.md#lookupeventsrequestrequesttypedef)
- [RefreshScheduleTypeDef](./type_defs.md#refreshscheduletypedef)
- [ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef)
- [CreateEventDataStoreResponseTypeDef](./type_defs.md#createeventdatastoreresponsetypedef)
- [EventDataStoreTypeDef](./type_defs.md#eventdatastoretypedef)
- [GetEventDataStoreResponseTypeDef](./type_defs.md#geteventdatastoreresponsetypedef)
- [RestoreEventDataStoreResponseTypeDef](./type_defs.md#restoreeventdatastoreresponsetypedef)
- [SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef)
- [UpdateEventDataStoreResponseTypeDef](./type_defs.md#updateeventdatastoreresponsetypedef)
- [AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef)
- [GetEventSelectorsResponseTypeDef](./type_defs.md#geteventselectorsresponsetypedef)
- [PutEventSelectorsResponseTypeDef](./type_defs.md#puteventselectorsresponsetypedef)
- [EventSelectorTypeDef](./type_defs.md#eventselectortypedef)
- [LookupEventsResponseTypeDef](./type_defs.md#lookupeventsresponsetypedef)
- [GetImportResponseTypeDef](./type_defs.md#getimportresponsetypedef)
- [StartImportRequestRequestTypeDef](./type_defs.md#startimportrequestrequesttypedef)
- [StartImportResponseTypeDef](./type_defs.md#startimportresponsetypedef)
- [StopImportResponseTypeDef](./type_defs.md#stopimportresponsetypedef)
- [CreateDashboardRequestRequestTypeDef](./type_defs.md#createdashboardrequestrequesttypedef)
- [CreateDashboardResponseTypeDef](./type_defs.md#createdashboardresponsetypedef)
- [GetDashboardResponseTypeDef](./type_defs.md#getdashboardresponsetypedef)
- [UpdateDashboardRequestRequestTypeDef](./type_defs.md#updatedashboardrequestrequesttypedef)
- [UpdateDashboardResponseTypeDef](./type_defs.md#updatedashboardresponsetypedef)
- [ListEventDataStoresResponseTypeDef](./type_defs.md#listeventdatastoresresponsetypedef)
- [GetChannelResponseTypeDef](./type_defs.md#getchannelresponsetypedef)
- [AdvancedEventSelectorUnionTypeDef](./type_defs.md#advancedeventselectoruniontypedef)
- [UpdateEventDataStoreRequestRequestTypeDef](./type_defs.md#updateeventdatastorerequestrequesttypedef)
- [EventSelectorUnionTypeDef](./type_defs.md#eventselectoruniontypedef)
- [CreateEventDataStoreRequestRequestTypeDef](./type_defs.md#createeventdatastorerequestrequesttypedef)
- [PutEventSelectorsRequestRequestTypeDef](./type_defs.md#puteventselectorsrequestrequesttypedef)

