# CloudWatchEvidently module

> [Index](../README.md) > CloudWatchEvidently


!!! note ""

    Auto-generated documentation for [CloudWatchEvidently](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#cloudwatchevidently)
    type annotations stubs module [types-aiobotocore-evidently](https://pypi.org/project/types-aiobotocore-evidently/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudWatchEvidently` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CloudWatchEvidently` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[evidently]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[evidently]'

# standalone installation
python -m pip install types-aiobotocore-evidently
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-evidently
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudWatchEvidentlyClient

Type annotations and code completion for  `#!python session.create_client("evidently")` as [CloudWatchEvidentlyClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client)

```python
# CloudWatchEvidentlyClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_evidently.client import CloudWatchEvidentlyClient


session = get_session()
async with session.create_client("evidently") as client:
    client: CloudWatchEvidentlyClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("evidently").get_paginator("...")`.

```python
# ListExperimentsPaginator usage example

from types_aiobotocore_evidently.paginator import ListExperimentsPaginator

def get_list_experiments_paginator() -> ListExperimentsPaginator:
    return client.get_paginator("list_experiments"))
```

- [ListExperimentsPaginator](./paginators.md#listexperimentspaginator)
- [ListFeaturesPaginator](./paginators.md#listfeaturespaginator)
- [ListLaunchesPaginator](./paginators.md#listlaunchespaginator)
- [ListProjectsPaginator](./paginators.md#listprojectspaginator)
- [ListSegmentReferencesPaginator](./paginators.md#listsegmentreferencespaginator)
- [ListSegmentsPaginator](./paginators.md#listsegmentspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ChangeDirectionEnumType usage example

from types_aiobotocore_evidently.literals import ChangeDirectionEnumType

def get_value() -> ChangeDirectionEnumType:
    return "DECREASE"
```

- [ChangeDirectionEnumType](./literals.md#changedirectionenumtype)
- [EventTypeType](./literals.md#eventtypetype)
- [ExperimentBaseStatType](./literals.md#experimentbasestattype)
- [ExperimentReportNameType](./literals.md#experimentreportnametype)
- [ExperimentResultRequestTypeType](./literals.md#experimentresultrequesttypetype)
- [ExperimentResultResponseTypeType](./literals.md#experimentresultresponsetypetype)
- [ExperimentStatusType](./literals.md#experimentstatustype)
- [ExperimentStopDesiredStateType](./literals.md#experimentstopdesiredstatetype)
- [ExperimentTypeType](./literals.md#experimenttypetype)
- [FeatureEvaluationStrategyType](./literals.md#featureevaluationstrategytype)
- [FeatureStatusType](./literals.md#featurestatustype)
- [LaunchStatusType](./literals.md#launchstatustype)
- [LaunchStopDesiredStateType](./literals.md#launchstopdesiredstatetype)
- [LaunchTypeType](./literals.md#launchtypetype)
- [ListExperimentsPaginatorName](./literals.md#listexperimentspaginatorname)
- [ListFeaturesPaginatorName](./literals.md#listfeaturespaginatorname)
- [ListLaunchesPaginatorName](./literals.md#listlaunchespaginatorname)
- [ListProjectsPaginatorName](./literals.md#listprojectspaginatorname)
- [ListSegmentReferencesPaginatorName](./literals.md#listsegmentreferencespaginatorname)
- [ListSegmentsPaginatorName](./literals.md#listsegmentspaginatorname)
- [ProjectStatusType](./literals.md#projectstatustype)
- [SegmentReferenceResourceTypeType](./literals.md#segmentreferenceresourcetypetype)
- [VariationValueTypeType](./literals.md#variationvaluetypetype)
- [CloudWatchEvidentlyServiceName](./literals.md#cloudwatchevidentlyservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [EvaluationRequestTypeDef](./type_defs.md#evaluationrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CloudWatchLogsDestinationConfigTypeDef](./type_defs.md#cloudwatchlogsdestinationconfigtypedef)
- [CloudWatchLogsDestinationTypeDef](./type_defs.md#cloudwatchlogsdestinationtypedef)
- [OnlineAbConfigTypeDef](./type_defs.md#onlineabconfigtypedef)
- [TreatmentConfigTypeDef](./type_defs.md#treatmentconfigtypedef)
- [LaunchGroupConfigTypeDef](./type_defs.md#launchgroupconfigtypedef)
- [ProjectAppConfigResourceConfigTypeDef](./type_defs.md#projectappconfigresourceconfigtypedef)
- [CreateSegmentRequestTypeDef](./type_defs.md#createsegmentrequesttypedef)
- [SegmentTypeDef](./type_defs.md#segmenttypedef)
- [DeleteExperimentRequestTypeDef](./type_defs.md#deleteexperimentrequesttypedef)
- [DeleteFeatureRequestTypeDef](./type_defs.md#deletefeaturerequesttypedef)
- [DeleteLaunchRequestTypeDef](./type_defs.md#deletelaunchrequesttypedef)
- [DeleteProjectRequestTypeDef](./type_defs.md#deleteprojectrequesttypedef)
- [DeleteSegmentRequestTypeDef](./type_defs.md#deletesegmentrequesttypedef)
- [EvaluateFeatureRequestTypeDef](./type_defs.md#evaluatefeaturerequesttypedef)
- [VariableValueTypeDef](./type_defs.md#variablevaluetypedef)
- [EvaluationRuleTypeDef](./type_defs.md#evaluationruletypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ExperimentExecutionTypeDef](./type_defs.md#experimentexecutiontypedef)
- [ExperimentReportTypeDef](./type_defs.md#experimentreporttypedef)
- [ExperimentResultsDataTypeDef](./type_defs.md#experimentresultsdatatypedef)
- [ExperimentScheduleTypeDef](./type_defs.md#experimentscheduletypedef)
- [OnlineAbDefinitionTypeDef](./type_defs.md#onlineabdefinitiontypedef)
- [TreatmentTypeDef](./type_defs.md#treatmenttypedef)
- [GetExperimentRequestTypeDef](./type_defs.md#getexperimentrequesttypedef)
- [GetFeatureRequestTypeDef](./type_defs.md#getfeaturerequesttypedef)
- [GetLaunchRequestTypeDef](./type_defs.md#getlaunchrequesttypedef)
- [GetProjectRequestTypeDef](./type_defs.md#getprojectrequesttypedef)
- [GetSegmentRequestTypeDef](./type_defs.md#getsegmentrequesttypedef)
- [LaunchExecutionTypeDef](./type_defs.md#launchexecutiontypedef)
- [LaunchGroupTypeDef](./type_defs.md#launchgrouptypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListExperimentsRequestTypeDef](./type_defs.md#listexperimentsrequesttypedef)
- [ListFeaturesRequestTypeDef](./type_defs.md#listfeaturesrequesttypedef)
- [ListLaunchesRequestTypeDef](./type_defs.md#listlaunchesrequesttypedef)
- [ListProjectsRequestTypeDef](./type_defs.md#listprojectsrequesttypedef)
- [ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef)
- [ListSegmentReferencesRequestTypeDef](./type_defs.md#listsegmentreferencesrequesttypedef)
- [RefResourceTypeDef](./type_defs.md#refresourcetypedef)
- [ListSegmentsRequestTypeDef](./type_defs.md#listsegmentsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [MetricDefinitionConfigTypeDef](./type_defs.md#metricdefinitionconfigtypedef)
- [MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef)
- [ProjectAppConfigResourceTypeDef](./type_defs.md#projectappconfigresourcetypedef)
- [S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef)
- [S3DestinationTypeDef](./type_defs.md#s3destinationtypedef)
- [PutProjectEventsResultEntryTypeDef](./type_defs.md#putprojecteventsresultentrytypedef)
- [SegmentOverrideOutputTypeDef](./type_defs.md#segmentoverrideoutputtypedef)
- [SegmentOverrideTypeDef](./type_defs.md#segmentoverridetypedef)
- [StartLaunchRequestTypeDef](./type_defs.md#startlaunchrequesttypedef)
- [StopExperimentRequestTypeDef](./type_defs.md#stopexperimentrequesttypedef)
- [StopLaunchRequestTypeDef](./type_defs.md#stoplaunchrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [TestSegmentPatternRequestTypeDef](./type_defs.md#testsegmentpatternrequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [BatchEvaluateFeatureRequestTypeDef](./type_defs.md#batchevaluatefeaturerequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartExperimentResponseTypeDef](./type_defs.md#startexperimentresponsetypedef)
- [StopExperimentResponseTypeDef](./type_defs.md#stopexperimentresponsetypedef)
- [StopLaunchResponseTypeDef](./type_defs.md#stoplaunchresponsetypedef)
- [TestSegmentPatternResponseTypeDef](./type_defs.md#testsegmentpatternresponsetypedef)
- [UpdateProjectRequestTypeDef](./type_defs.md#updateprojectrequesttypedef)
- [CreateSegmentResponseTypeDef](./type_defs.md#createsegmentresponsetypedef)
- [GetSegmentResponseTypeDef](./type_defs.md#getsegmentresponsetypedef)
- [ListSegmentsResponseTypeDef](./type_defs.md#listsegmentsresponsetypedef)
- [EvaluateFeatureResponseTypeDef](./type_defs.md#evaluatefeatureresponsetypedef)
- [EvaluationResultTypeDef](./type_defs.md#evaluationresulttypedef)
- [VariationConfigTypeDef](./type_defs.md#variationconfigtypedef)
- [VariationTypeDef](./type_defs.md#variationtypedef)
- [FeatureSummaryTypeDef](./type_defs.md#featuresummarytypedef)
- [EventTypeDef](./type_defs.md#eventtypedef)
- [GetExperimentResultsRequestTypeDef](./type_defs.md#getexperimentresultsrequesttypedef)
- [StartExperimentRequestTypeDef](./type_defs.md#startexperimentrequesttypedef)
- [GetExperimentResultsResponseTypeDef](./type_defs.md#getexperimentresultsresponsetypedef)
- [ListExperimentsRequestPaginateTypeDef](./type_defs.md#listexperimentsrequestpaginatetypedef)
- [ListFeaturesRequestPaginateTypeDef](./type_defs.md#listfeaturesrequestpaginatetypedef)
- [ListLaunchesRequestPaginateTypeDef](./type_defs.md#listlaunchesrequestpaginatetypedef)
- [ListProjectsRequestPaginateTypeDef](./type_defs.md#listprojectsrequestpaginatetypedef)
- [ListSegmentReferencesRequestPaginateTypeDef](./type_defs.md#listsegmentreferencesrequestpaginatetypedef)
- [ListSegmentsRequestPaginateTypeDef](./type_defs.md#listsegmentsrequestpaginatetypedef)
- [ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef)
- [ListSegmentReferencesResponseTypeDef](./type_defs.md#listsegmentreferencesresponsetypedef)
- [MetricGoalConfigTypeDef](./type_defs.md#metricgoalconfigtypedef)
- [MetricMonitorConfigTypeDef](./type_defs.md#metricmonitorconfigtypedef)
- [MetricGoalTypeDef](./type_defs.md#metricgoaltypedef)
- [MetricMonitorTypeDef](./type_defs.md#metricmonitortypedef)
- [ProjectDataDeliveryConfigTypeDef](./type_defs.md#projectdatadeliveryconfigtypedef)
- [UpdateProjectDataDeliveryRequestTypeDef](./type_defs.md#updateprojectdatadeliveryrequesttypedef)
- [ProjectDataDeliveryTypeDef](./type_defs.md#projectdatadeliverytypedef)
- [PutProjectEventsResponseTypeDef](./type_defs.md#putprojecteventsresponsetypedef)
- [ScheduledSplitTypeDef](./type_defs.md#scheduledsplittypedef)
- [SegmentOverrideUnionTypeDef](./type_defs.md#segmentoverrideuniontypedef)
- [BatchEvaluateFeatureResponseTypeDef](./type_defs.md#batchevaluatefeatureresponsetypedef)
- [CreateFeatureRequestTypeDef](./type_defs.md#createfeaturerequesttypedef)
- [UpdateFeatureRequestTypeDef](./type_defs.md#updatefeaturerequesttypedef)
- [FeatureTypeDef](./type_defs.md#featuretypedef)
- [ListFeaturesResponseTypeDef](./type_defs.md#listfeaturesresponsetypedef)
- [PutProjectEventsRequestTypeDef](./type_defs.md#putprojecteventsrequesttypedef)
- [CreateExperimentRequestTypeDef](./type_defs.md#createexperimentrequesttypedef)
- [UpdateExperimentRequestTypeDef](./type_defs.md#updateexperimentrequesttypedef)
- [ExperimentTypeDef](./type_defs.md#experimenttypedef)
- [CreateProjectRequestTypeDef](./type_defs.md#createprojectrequesttypedef)
- [ProjectTypeDef](./type_defs.md#projecttypedef)
- [ScheduledSplitsLaunchDefinitionTypeDef](./type_defs.md#scheduledsplitslaunchdefinitiontypedef)
- [ScheduledSplitConfigTypeDef](./type_defs.md#scheduledsplitconfigtypedef)
- [CreateFeatureResponseTypeDef](./type_defs.md#createfeatureresponsetypedef)
- [GetFeatureResponseTypeDef](./type_defs.md#getfeatureresponsetypedef)
- [UpdateFeatureResponseTypeDef](./type_defs.md#updatefeatureresponsetypedef)
- [CreateExperimentResponseTypeDef](./type_defs.md#createexperimentresponsetypedef)
- [GetExperimentResponseTypeDef](./type_defs.md#getexperimentresponsetypedef)
- [ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef)
- [UpdateExperimentResponseTypeDef](./type_defs.md#updateexperimentresponsetypedef)
- [CreateProjectResponseTypeDef](./type_defs.md#createprojectresponsetypedef)
- [GetProjectResponseTypeDef](./type_defs.md#getprojectresponsetypedef)
- [UpdateProjectDataDeliveryResponseTypeDef](./type_defs.md#updateprojectdatadeliveryresponsetypedef)
- [UpdateProjectResponseTypeDef](./type_defs.md#updateprojectresponsetypedef)
- [LaunchTypeDef](./type_defs.md#launchtypedef)
- [ScheduledSplitsLaunchConfigTypeDef](./type_defs.md#scheduledsplitslaunchconfigtypedef)
- [CreateLaunchResponseTypeDef](./type_defs.md#createlaunchresponsetypedef)
- [GetLaunchResponseTypeDef](./type_defs.md#getlaunchresponsetypedef)
- [ListLaunchesResponseTypeDef](./type_defs.md#listlaunchesresponsetypedef)
- [StartLaunchResponseTypeDef](./type_defs.md#startlaunchresponsetypedef)
- [UpdateLaunchResponseTypeDef](./type_defs.md#updatelaunchresponsetypedef)
- [CreateLaunchRequestTypeDef](./type_defs.md#createlaunchrequesttypedef)
- [UpdateLaunchRequestTypeDef](./type_defs.md#updatelaunchrequesttypedef)

