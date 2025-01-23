# TimestreamQuery module

> [Index](../README.md) > TimestreamQuery


!!! note ""

    Auto-generated documentation for [TimestreamQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#timestreamquery)
    type annotations stubs module [types-aiobotocore-timestream-query](https://pypi.org/project/types-aiobotocore-timestream-query/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `TimestreamQuery` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `TimestreamQuery` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[timestream-query]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[timestream-query]'

# standalone installation
python -m pip install types-aiobotocore-timestream-query
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-timestream-query
```

## Usage

Code samples can be found in [Examples](./usage.md).

## TimestreamQueryClient

Type annotations and code completion for  `#!python session.create_client("timestream-query")` as [TimestreamQueryClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# TimestreamQueryClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_timestream_query.client import TimestreamQueryClient


session = get_session()
async with session.create_client("timestream-query") as client:
    client: TimestreamQueryClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("timestream-query").get_paginator("...")`.

```python
# ListScheduledQueriesPaginator usage example

from types_aiobotocore_timestream_query.paginator import ListScheduledQueriesPaginator

def get_list_scheduled_queries_paginator() -> ListScheduledQueriesPaginator:
    return client.get_paginator("list_scheduled_queries"))
```

- [ListScheduledQueriesPaginator](./paginators.md#listscheduledqueriespaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- [QueryPaginator](./paginators.md#querypaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ComputeModeType usage example

from types_aiobotocore_timestream_query.literals import ComputeModeType

def get_value() -> ComputeModeType:
    return "ON_DEMAND"
```

- [ComputeModeType](./literals.md#computemodetype)
- [DimensionValueTypeType](./literals.md#dimensionvaluetypetype)
- [LastUpdateStatusType](./literals.md#lastupdatestatustype)
- [ListScheduledQueriesPaginatorName](./literals.md#listscheduledqueriespaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [MeasureValueTypeType](./literals.md#measurevaluetypetype)
- [QueryInsightsModeType](./literals.md#queryinsightsmodetype)
- [QueryPaginatorName](./literals.md#querypaginatorname)
- [QueryPricingModelType](./literals.md#querypricingmodeltype)
- [S3EncryptionOptionType](./literals.md#s3encryptionoptiontype)
- [ScalarMeasureValueTypeType](./literals.md#scalarmeasurevaluetypetype)
- [ScalarTypeType](./literals.md#scalartypetype)
- [ScheduledQueryInsightsModeType](./literals.md#scheduledqueryinsightsmodetype)
- [ScheduledQueryRunStatusType](./literals.md#scheduledqueryrunstatustype)
- [ScheduledQueryStateType](./literals.md#scheduledquerystatetype)
- [TimestreamQueryServiceName](./literals.md#timestreamqueryservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [SnsConfigurationTypeDef](./type_defs.md#snsconfigurationtypedef)
- [CancelQueryRequestRequestTypeDef](./type_defs.md#cancelqueryrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TypePaginatorTypeDef](./type_defs.md#typepaginatortypedef)
- [ColumnInfoTypeDef](./type_defs.md#columninfotypedef)
- [ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [TimeSeriesDataPointPaginatorTypeDef](./type_defs.md#timeseriesdatapointpaginatortypedef)
- [TimeSeriesDataPointTypeDef](./type_defs.md#timeseriesdatapointtypedef)
- [DeleteScheduledQueryRequestRequestTypeDef](./type_defs.md#deletescheduledqueryrequestrequesttypedef)
- [EndpointTypeDef](./type_defs.md#endpointtypedef)
- [DescribeScheduledQueryRequestRequestTypeDef](./type_defs.md#describescheduledqueryrequestrequesttypedef)
- [DimensionMappingTypeDef](./type_defs.md#dimensionmappingtypedef)
- [S3ConfigurationTypeDef](./type_defs.md#s3configurationtypedef)
- [S3ReportLocationTypeDef](./type_defs.md#s3reportlocationtypedef)
- [ScheduledQueryInsightsTypeDef](./type_defs.md#scheduledqueryinsightstypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ExecutionStatsTypeDef](./type_defs.md#executionstatstypedef)
- [LastUpdateTypeDef](./type_defs.md#lastupdatetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListScheduledQueriesRequestRequestTypeDef](./type_defs.md#listscheduledqueriesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [MultiMeasureAttributeMappingTypeDef](./type_defs.md#multimeasureattributemappingtypedef)
- [PrepareQueryRequestRequestTypeDef](./type_defs.md#preparequeryrequestrequesttypedef)
- [QueryInsightsTypeDef](./type_defs.md#queryinsightstypedef)
- [QueryStatusTypeDef](./type_defs.md#querystatustypedef)
- [QuerySpatialCoverageMaxTypeDef](./type_defs.md#queryspatialcoveragemaxtypedef)
- [QueryTemporalRangeMaxTypeDef](./type_defs.md#querytemporalrangemaxtypedef)
- [TimestreamDestinationTypeDef](./type_defs.md#timestreamdestinationtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateScheduledQueryRequestRequestTypeDef](./type_defs.md#updatescheduledqueryrequestrequesttypedef)
- [AccountSettingsNotificationConfigurationTypeDef](./type_defs.md#accountsettingsnotificationconfigurationtypedef)
- [NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef)
- [CancelQueryResponseTypeDef](./type_defs.md#cancelqueryresponsetypedef)
- [CreateScheduledQueryResponseTypeDef](./type_defs.md#createscheduledqueryresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ColumnInfoPaginatorTypeDef](./type_defs.md#columninfopaginatortypedef)
- [TypeTypeDef](./type_defs.md#typetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [DatumPaginatorTypeDef](./type_defs.md#datumpaginatortypedef)
- [DatumTypeDef](./type_defs.md#datumtypedef)
- [DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef)
- [ErrorReportConfigurationTypeDef](./type_defs.md#errorreportconfigurationtypedef)
- [ErrorReportLocationTypeDef](./type_defs.md#errorreportlocationtypedef)
- [ExecuteScheduledQueryRequestRequestTypeDef](./type_defs.md#executescheduledqueryrequestrequesttypedef)
- [ListScheduledQueriesRequestPaginateTypeDef](./type_defs.md#listscheduledqueriesrequestpaginatetypedef)
- [ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef)
- [MixedMeasureMappingOutputTypeDef](./type_defs.md#mixedmeasuremappingoutputtypedef)
- [MixedMeasureMappingTypeDef](./type_defs.md#mixedmeasuremappingtypedef)
- [MultiMeasureMappingsOutputTypeDef](./type_defs.md#multimeasuremappingsoutputtypedef)
- [MultiMeasureMappingsTypeDef](./type_defs.md#multimeasuremappingstypedef)
- [QueryRequestPaginateTypeDef](./type_defs.md#queryrequestpaginatetypedef)
- [QueryRequestRequestTypeDef](./type_defs.md#queryrequestrequesttypedef)
- [QuerySpatialCoverageTypeDef](./type_defs.md#queryspatialcoveragetypedef)
- [QueryTemporalRangeTypeDef](./type_defs.md#querytemporalrangetypedef)
- [TargetDestinationTypeDef](./type_defs.md#targetdestinationtypedef)
- [ProvisionedCapacityRequestTypeDef](./type_defs.md#provisionedcapacityrequesttypedef)
- [ProvisionedCapacityResponseTypeDef](./type_defs.md#provisionedcapacityresponsetypedef)
- [ParameterMappingTypeDef](./type_defs.md#parametermappingtypedef)
- [SelectColumnTypeDef](./type_defs.md#selectcolumntypedef)
- [RowPaginatorTypeDef](./type_defs.md#rowpaginatortypedef)
- [RowTypeDef](./type_defs.md#rowtypedef)
- [MixedMeasureMappingUnionTypeDef](./type_defs.md#mixedmeasuremappinguniontypedef)
- [TimestreamConfigurationOutputTypeDef](./type_defs.md#timestreamconfigurationoutputtypedef)
- [MultiMeasureMappingsUnionTypeDef](./type_defs.md#multimeasuremappingsuniontypedef)
- [QueryInsightsResponseTypeDef](./type_defs.md#queryinsightsresponsetypedef)
- [ScheduledQueryInsightsResponseTypeDef](./type_defs.md#scheduledqueryinsightsresponsetypedef)
- [ScheduledQueryTypeDef](./type_defs.md#scheduledquerytypedef)
- [QueryComputeRequestTypeDef](./type_defs.md#querycomputerequesttypedef)
- [QueryComputeResponseTypeDef](./type_defs.md#querycomputeresponsetypedef)
- [PrepareQueryResponseTypeDef](./type_defs.md#preparequeryresponsetypedef)
- [TargetConfigurationOutputTypeDef](./type_defs.md#targetconfigurationoutputtypedef)
- [TimestreamConfigurationTypeDef](./type_defs.md#timestreamconfigurationtypedef)
- [QueryResponsePaginatorTypeDef](./type_defs.md#queryresponsepaginatortypedef)
- [QueryResponseTypeDef](./type_defs.md#queryresponsetypedef)
- [ScheduledQueryRunSummaryTypeDef](./type_defs.md#scheduledqueryrunsummarytypedef)
- [ListScheduledQueriesResponseTypeDef](./type_defs.md#listscheduledqueriesresponsetypedef)
- [UpdateAccountSettingsRequestRequestTypeDef](./type_defs.md#updateaccountsettingsrequestrequesttypedef)
- [DescribeAccountSettingsResponseTypeDef](./type_defs.md#describeaccountsettingsresponsetypedef)
- [UpdateAccountSettingsResponseTypeDef](./type_defs.md#updateaccountsettingsresponsetypedef)
- [TimestreamConfigurationUnionTypeDef](./type_defs.md#timestreamconfigurationuniontypedef)
- [ScheduledQueryDescriptionTypeDef](./type_defs.md#scheduledquerydescriptiontypedef)
- [TargetConfigurationTypeDef](./type_defs.md#targetconfigurationtypedef)
- [DescribeScheduledQueryResponseTypeDef](./type_defs.md#describescheduledqueryresponsetypedef)
- [CreateScheduledQueryRequestRequestTypeDef](./type_defs.md#createscheduledqueryrequestrequesttypedef)

