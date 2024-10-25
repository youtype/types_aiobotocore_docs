# SFN module

> [Index](../README.md) > SFN


!!! note ""

    Auto-generated documentation for [SFN](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
    type annotations stubs module [types-aiobotocore-stepfunctions](https://pypi.org/project/types-aiobotocore-stepfunctions/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `SFN` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[stepfunctions]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[stepfunctions]'


# standalone installation
python -m pip install types-aiobotocore-stepfunctions
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-stepfunctions
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SFNClient

Type annotations and code completion for  `#!python session.create_client("stepfunctions")` as [SFNClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client)

```python
# SFNClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_stepfunctions.client import SFNClient


session = get_session()
async with session.create_client("stepfunctions") as client:
    client: SFNClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("stepfunctions").get_paginator("...")`.

```python
# GetExecutionHistoryPaginator usage example

from types_aiobotocore_stepfunctions.paginator import GetExecutionHistoryPaginator

def get_get_execution_history_paginator() -> GetExecutionHistoryPaginator:
    return client.get_paginator("get_execution_history"))
```

- [GetExecutionHistoryPaginator](./paginators.md#getexecutionhistorypaginator)
- [ListActivitiesPaginator](./paginators.md#listactivitiespaginator)
- [ListExecutionsPaginator](./paginators.md#listexecutionspaginator)
- [ListMapRunsPaginator](./paginators.md#listmaprunspaginator)
- [ListStateMachinesPaginator](./paginators.md#liststatemachinespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# EncryptionTypeType usage example

from types_aiobotocore_stepfunctions.literals import EncryptionTypeType

def get_value() -> EncryptionTypeType:
    return "AWS_OWNED_KEY"
```

- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [ExecutionRedriveFilterType](./literals.md#executionredrivefiltertype)
- [ExecutionRedriveStatusType](./literals.md#executionredrivestatustype)
- [ExecutionStatusType](./literals.md#executionstatustype)
- [GetExecutionHistoryPaginatorName](./literals.md#getexecutionhistorypaginatorname)
- [HistoryEventTypeType](./literals.md#historyeventtypetype)
- [IncludedDataType](./literals.md#includeddatatype)
- [InspectionLevelType](./literals.md#inspectionleveltype)
- [ListActivitiesPaginatorName](./literals.md#listactivitiespaginatorname)
- [ListExecutionsPaginatorName](./literals.md#listexecutionspaginatorname)
- [ListMapRunsPaginatorName](./literals.md#listmaprunspaginatorname)
- [ListStateMachinesPaginatorName](./literals.md#liststatemachinespaginatorname)
- [LogLevelType](./literals.md#logleveltype)
- [MapRunStatusType](./literals.md#maprunstatustype)
- [StateMachineStatusType](./literals.md#statemachinestatustype)
- [StateMachineTypeType](./literals.md#statemachinetypetype)
- [SyncExecutionStatusType](./literals.md#syncexecutionstatustype)
- [TestExecutionStatusType](./literals.md#testexecutionstatustype)
- [ValidateStateMachineDefinitionResultCodeType](./literals.md#validatestatemachinedefinitionresultcodetype)
- [ValidateStateMachineDefinitionSeverityType](./literals.md#validatestatemachinedefinitionseveritytype)
- [SFNServiceName](./literals.md#sfnservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActivityFailedEventDetailsTypeDef](./type_defs.md#activityfailedeventdetailstypedef)
- [ActivityListItemTypeDef](./type_defs.md#activitylistitemtypedef)
- [ActivityScheduleFailedEventDetailsTypeDef](./type_defs.md#activityschedulefailedeventdetailstypedef)
- [HistoryEventExecutionDataDetailsTypeDef](./type_defs.md#historyeventexecutiondatadetailstypedef)
- [ActivityStartedEventDetailsTypeDef](./type_defs.md#activitystartedeventdetailstypedef)
- [ActivityTimedOutEventDetailsTypeDef](./type_defs.md#activitytimedouteventdetailstypedef)
- [BillingDetailsTypeDef](./type_defs.md#billingdetailstypedef)
- [CloudWatchEventsExecutionDataDetailsTypeDef](./type_defs.md#cloudwatcheventsexecutiondatadetailstypedef)
- [CloudWatchLogsLogGroupTypeDef](./type_defs.md#cloudwatchlogsloggrouptypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [RoutingConfigurationListItemTypeDef](./type_defs.md#routingconfigurationlistitemtypedef)
- [TracingConfigurationTypeDef](./type_defs.md#tracingconfigurationtypedef)
- [DeleteActivityInputRequestTypeDef](./type_defs.md#deleteactivityinputrequesttypedef)
- [DeleteStateMachineAliasInputRequestTypeDef](./type_defs.md#deletestatemachinealiasinputrequesttypedef)
- [DeleteStateMachineInputRequestTypeDef](./type_defs.md#deletestatemachineinputrequesttypedef)
- [DeleteStateMachineVersionInputRequestTypeDef](./type_defs.md#deletestatemachineversioninputrequesttypedef)
- [DescribeActivityInputRequestTypeDef](./type_defs.md#describeactivityinputrequesttypedef)
- [DescribeExecutionInputRequestTypeDef](./type_defs.md#describeexecutioninputrequesttypedef)
- [DescribeMapRunInputRequestTypeDef](./type_defs.md#describemapruninputrequesttypedef)
- [MapRunExecutionCountsTypeDef](./type_defs.md#maprunexecutioncountstypedef)
- [MapRunItemCountsTypeDef](./type_defs.md#maprunitemcountstypedef)
- [DescribeStateMachineAliasInputRequestTypeDef](./type_defs.md#describestatemachinealiasinputrequesttypedef)
- [DescribeStateMachineForExecutionInputRequestTypeDef](./type_defs.md#describestatemachineforexecutioninputrequesttypedef)
- [DescribeStateMachineInputRequestTypeDef](./type_defs.md#describestatemachineinputrequesttypedef)
- [ExecutionAbortedEventDetailsTypeDef](./type_defs.md#executionabortedeventdetailstypedef)
- [ExecutionFailedEventDetailsTypeDef](./type_defs.md#executionfailedeventdetailstypedef)
- [ExecutionListItemTypeDef](./type_defs.md#executionlistitemtypedef)
- [ExecutionRedrivenEventDetailsTypeDef](./type_defs.md#executionredriveneventdetailstypedef)
- [ExecutionTimedOutEventDetailsTypeDef](./type_defs.md#executiontimedouteventdetailstypedef)
- [GetActivityTaskInputRequestTypeDef](./type_defs.md#getactivitytaskinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetExecutionHistoryInputRequestTypeDef](./type_defs.md#getexecutionhistoryinputrequesttypedef)
- [LambdaFunctionFailedEventDetailsTypeDef](./type_defs.md#lambdafunctionfailedeventdetailstypedef)
- [LambdaFunctionScheduleFailedEventDetailsTypeDef](./type_defs.md#lambdafunctionschedulefailedeventdetailstypedef)
- [LambdaFunctionStartFailedEventDetailsTypeDef](./type_defs.md#lambdafunctionstartfailedeventdetailstypedef)
- [LambdaFunctionTimedOutEventDetailsTypeDef](./type_defs.md#lambdafunctiontimedouteventdetailstypedef)
- [MapIterationEventDetailsTypeDef](./type_defs.md#mapiterationeventdetailstypedef)
- [MapRunFailedEventDetailsTypeDef](./type_defs.md#maprunfailedeventdetailstypedef)
- [MapRunRedrivenEventDetailsTypeDef](./type_defs.md#maprunredriveneventdetailstypedef)
- [MapRunStartedEventDetailsTypeDef](./type_defs.md#maprunstartedeventdetailstypedef)
- [MapStateStartedEventDetailsTypeDef](./type_defs.md#mapstatestartedeventdetailstypedef)
- [TaskFailedEventDetailsTypeDef](./type_defs.md#taskfailedeventdetailstypedef)
- [TaskStartFailedEventDetailsTypeDef](./type_defs.md#taskstartfailedeventdetailstypedef)
- [TaskStartedEventDetailsTypeDef](./type_defs.md#taskstartedeventdetailstypedef)
- [TaskSubmitFailedEventDetailsTypeDef](./type_defs.md#tasksubmitfailedeventdetailstypedef)
- [TaskTimedOutEventDetailsTypeDef](./type_defs.md#tasktimedouteventdetailstypedef)
- [InspectionDataRequestTypeDef](./type_defs.md#inspectiondatarequesttypedef)
- [InspectionDataResponseTypeDef](./type_defs.md#inspectiondataresponsetypedef)
- [TaskCredentialsTypeDef](./type_defs.md#taskcredentialstypedef)
- [ListActivitiesInputRequestTypeDef](./type_defs.md#listactivitiesinputrequesttypedef)
- [ListExecutionsInputRequestTypeDef](./type_defs.md#listexecutionsinputrequesttypedef)
- [ListMapRunsInputRequestTypeDef](./type_defs.md#listmaprunsinputrequesttypedef)
- [MapRunListItemTypeDef](./type_defs.md#maprunlistitemtypedef)
- [ListStateMachineAliasesInputRequestTypeDef](./type_defs.md#liststatemachinealiasesinputrequesttypedef)
- [StateMachineAliasListItemTypeDef](./type_defs.md#statemachinealiaslistitemtypedef)
- [ListStateMachineVersionsInputRequestTypeDef](./type_defs.md#liststatemachineversionsinputrequesttypedef)
- [StateMachineVersionListItemTypeDef](./type_defs.md#statemachineversionlistitemtypedef)
- [ListStateMachinesInputRequestTypeDef](./type_defs.md#liststatemachinesinputrequesttypedef)
- [StateMachineListItemTypeDef](./type_defs.md#statemachinelistitemtypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [PublishStateMachineVersionInputRequestTypeDef](./type_defs.md#publishstatemachineversioninputrequesttypedef)
- [RedriveExecutionInputRequestTypeDef](./type_defs.md#redriveexecutioninputrequesttypedef)
- [SendTaskFailureInputRequestTypeDef](./type_defs.md#sendtaskfailureinputrequesttypedef)
- [SendTaskHeartbeatInputRequestTypeDef](./type_defs.md#sendtaskheartbeatinputrequesttypedef)
- [SendTaskSuccessInputRequestTypeDef](./type_defs.md#sendtasksuccessinputrequesttypedef)
- [StartExecutionInputRequestTypeDef](./type_defs.md#startexecutioninputrequesttypedef)
- [StartSyncExecutionInputRequestTypeDef](./type_defs.md#startsyncexecutioninputrequesttypedef)
- [StopExecutionInputRequestTypeDef](./type_defs.md#stopexecutioninputrequesttypedef)
- [TestStateInputRequestTypeDef](./type_defs.md#teststateinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateMapRunInputRequestTypeDef](./type_defs.md#updatemapruninputrequesttypedef)
- [ValidateStateMachineDefinitionDiagnosticTypeDef](./type_defs.md#validatestatemachinedefinitiondiagnostictypedef)
- [ValidateStateMachineDefinitionInputRequestTypeDef](./type_defs.md#validatestatemachinedefinitioninputrequesttypedef)
- [ActivityScheduledEventDetailsTypeDef](./type_defs.md#activityscheduledeventdetailstypedef)
- [ActivitySucceededEventDetailsTypeDef](./type_defs.md#activitysucceededeventdetailstypedef)
- [ExecutionStartedEventDetailsTypeDef](./type_defs.md#executionstartedeventdetailstypedef)
- [ExecutionSucceededEventDetailsTypeDef](./type_defs.md#executionsucceededeventdetailstypedef)
- [LambdaFunctionSucceededEventDetailsTypeDef](./type_defs.md#lambdafunctionsucceededeventdetailstypedef)
- [StateEnteredEventDetailsTypeDef](./type_defs.md#stateenteredeventdetailstypedef)
- [StateExitedEventDetailsTypeDef](./type_defs.md#stateexitedeventdetailstypedef)
- [TaskSubmittedEventDetailsTypeDef](./type_defs.md#tasksubmittedeventdetailstypedef)
- [TaskSucceededEventDetailsTypeDef](./type_defs.md#tasksucceededeventdetailstypedef)
- [LogDestinationTypeDef](./type_defs.md#logdestinationtypedef)
- [CreateActivityInputRequestTypeDef](./type_defs.md#createactivityinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [CreateActivityOutputTypeDef](./type_defs.md#createactivityoutputtypedef)
- [CreateStateMachineAliasOutputTypeDef](./type_defs.md#createstatemachinealiasoutputtypedef)
- [CreateStateMachineOutputTypeDef](./type_defs.md#createstatemachineoutputtypedef)
- [DescribeActivityOutputTypeDef](./type_defs.md#describeactivityoutputtypedef)
- [DescribeExecutionOutputTypeDef](./type_defs.md#describeexecutionoutputtypedef)
- [GetActivityTaskOutputTypeDef](./type_defs.md#getactivitytaskoutputtypedef)
- [ListActivitiesOutputTypeDef](./type_defs.md#listactivitiesoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [PublishStateMachineVersionOutputTypeDef](./type_defs.md#publishstatemachineversionoutputtypedef)
- [RedriveExecutionOutputTypeDef](./type_defs.md#redriveexecutionoutputtypedef)
- [StartExecutionOutputTypeDef](./type_defs.md#startexecutionoutputtypedef)
- [StartSyncExecutionOutputTypeDef](./type_defs.md#startsyncexecutionoutputtypedef)
- [StopExecutionOutputTypeDef](./type_defs.md#stopexecutionoutputtypedef)
- [UpdateStateMachineAliasOutputTypeDef](./type_defs.md#updatestatemachinealiasoutputtypedef)
- [UpdateStateMachineOutputTypeDef](./type_defs.md#updatestatemachineoutputtypedef)
- [CreateStateMachineAliasInputRequestTypeDef](./type_defs.md#createstatemachinealiasinputrequesttypedef)
- [DescribeStateMachineAliasOutputTypeDef](./type_defs.md#describestatemachinealiasoutputtypedef)
- [UpdateStateMachineAliasInputRequestTypeDef](./type_defs.md#updatestatemachinealiasinputrequesttypedef)
- [DescribeMapRunOutputTypeDef](./type_defs.md#describemaprunoutputtypedef)
- [ListExecutionsOutputTypeDef](./type_defs.md#listexecutionsoutputtypedef)
- [GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef](./type_defs.md#getexecutionhistoryinputgetexecutionhistorypaginatetypedef)
- [ListActivitiesInputListActivitiesPaginateTypeDef](./type_defs.md#listactivitiesinputlistactivitiespaginatetypedef)
- [ListExecutionsInputListExecutionsPaginateTypeDef](./type_defs.md#listexecutionsinputlistexecutionspaginatetypedef)
- [ListMapRunsInputListMapRunsPaginateTypeDef](./type_defs.md#listmaprunsinputlistmaprunspaginatetypedef)
- [ListStateMachinesInputListStateMachinesPaginateTypeDef](./type_defs.md#liststatemachinesinputliststatemachinespaginatetypedef)
- [InspectionDataTypeDef](./type_defs.md#inspectiondatatypedef)
- [LambdaFunctionScheduledEventDetailsTypeDef](./type_defs.md#lambdafunctionscheduledeventdetailstypedef)
- [TaskScheduledEventDetailsTypeDef](./type_defs.md#taskscheduledeventdetailstypedef)
- [ListMapRunsOutputTypeDef](./type_defs.md#listmaprunsoutputtypedef)
- [ListStateMachineAliasesOutputTypeDef](./type_defs.md#liststatemachinealiasesoutputtypedef)
- [ListStateMachineVersionsOutputTypeDef](./type_defs.md#liststatemachineversionsoutputtypedef)
- [ListStateMachinesOutputTypeDef](./type_defs.md#liststatemachinesoutputtypedef)
- [ValidateStateMachineDefinitionOutputTypeDef](./type_defs.md#validatestatemachinedefinitionoutputtypedef)
- [LoggingConfigurationOutputTypeDef](./type_defs.md#loggingconfigurationoutputtypedef)
- [LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef)
- [TestStateOutputTypeDef](./type_defs.md#teststateoutputtypedef)
- [HistoryEventTypeDef](./type_defs.md#historyeventtypedef)
- [DescribeStateMachineForExecutionOutputTypeDef](./type_defs.md#describestatemachineforexecutionoutputtypedef)
- [DescribeStateMachineOutputTypeDef](./type_defs.md#describestatemachineoutputtypedef)
- [CreateStateMachineInputRequestTypeDef](./type_defs.md#createstatemachineinputrequesttypedef)
- [UpdateStateMachineInputRequestTypeDef](./type_defs.md#updatestatemachineinputrequesttypedef)
- [GetExecutionHistoryOutputTypeDef](./type_defs.md#getexecutionhistoryoutputtypedef)

