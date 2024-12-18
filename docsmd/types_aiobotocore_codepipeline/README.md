# CodePipeline module

> [Index](../README.md) > CodePipeline


!!! note ""

    Auto-generated documentation for [CodePipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#codepipeline)
    type annotations stubs module [types-aiobotocore-codepipeline](https://pypi.org/project/types-aiobotocore-codepipeline/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CodePipeline` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CodePipeline` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[codepipeline]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[codepipeline]'

# standalone installation
python -m pip install types-aiobotocore-codepipeline
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-codepipeline
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CodePipelineClient

Type annotations and code completion for  `#!python session.create_client("codepipeline")` as [CodePipelineClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client)

```python
# CodePipelineClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.client import CodePipelineClient


session = get_session()
async with session.create_client("codepipeline") as client:
    client: CodePipelineClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("codepipeline").get_paginator("...")`.

```python
# ListActionExecutionsPaginator usage example

from types_aiobotocore_codepipeline.paginator import ListActionExecutionsPaginator

def get_list_action_executions_paginator() -> ListActionExecutionsPaginator:
    return client.get_paginator("list_action_executions"))
```

- [ListActionExecutionsPaginator](./paginators.md#listactionexecutionspaginator)
- [ListActionTypesPaginator](./paginators.md#listactiontypespaginator)
- [ListPipelineExecutionsPaginator](./paginators.md#listpipelineexecutionspaginator)
- [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
- [ListRuleExecutionsPaginator](./paginators.md#listruleexecutionspaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- [ListWebhooksPaginator](./paginators.md#listwebhookspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionCategoryType usage example

from types_aiobotocore_codepipeline.literals import ActionCategoryType

def get_value() -> ActionCategoryType:
    return "Approval"
```

- [ActionCategoryType](./literals.md#actioncategorytype)
- [ActionConfigurationPropertyTypeType](./literals.md#actionconfigurationpropertytypetype)
- [ActionExecutionStatusType](./literals.md#actionexecutionstatustype)
- [ActionOwnerType](./literals.md#actionownertype)
- [ApprovalStatusType](./literals.md#approvalstatustype)
- [ArtifactLocationTypeType](./literals.md#artifactlocationtypetype)
- [ArtifactStoreTypeType](./literals.md#artifactstoretypetype)
- [BlockerTypeType](./literals.md#blockertypetype)
- [ConditionExecutionStatusType](./literals.md#conditionexecutionstatustype)
- [ConditionTypeType](./literals.md#conditiontypetype)
- [EncryptionKeyTypeType](./literals.md#encryptionkeytypetype)
- [ExecutionModeType](./literals.md#executionmodetype)
- [ExecutionTypeType](./literals.md#executiontypetype)
- [ExecutorTypeType](./literals.md#executortypetype)
- [FailureTypeType](./literals.md#failuretypetype)
- [GitPullRequestEventTypeType](./literals.md#gitpullrequesteventtypetype)
- [JobStatusType](./literals.md#jobstatustype)
- [ListActionExecutionsPaginatorName](./literals.md#listactionexecutionspaginatorname)
- [ListActionTypesPaginatorName](./literals.md#listactiontypespaginatorname)
- [ListPipelineExecutionsPaginatorName](./literals.md#listpipelineexecutionspaginatorname)
- [ListPipelinesPaginatorName](./literals.md#listpipelinespaginatorname)
- [ListRuleExecutionsPaginatorName](./literals.md#listruleexecutionspaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [ListWebhooksPaginatorName](./literals.md#listwebhookspaginatorname)
- [PipelineExecutionStatusType](./literals.md#pipelineexecutionstatustype)
- [PipelineTriggerProviderTypeType](./literals.md#pipelinetriggerprovidertypetype)
- [PipelineTypeType](./literals.md#pipelinetypetype)
- [ResultType](./literals.md#resulttype)
- [RetryTriggerType](./literals.md#retrytriggertype)
- [RuleCategoryType](./literals.md#rulecategorytype)
- [RuleConfigurationPropertyTypeType](./literals.md#ruleconfigurationpropertytypetype)
- [RuleExecutionStatusType](./literals.md#ruleexecutionstatustype)
- [RuleOwnerType](./literals.md#ruleownertype)
- [SourceRevisionTypeType](./literals.md#sourcerevisiontypetype)
- [StageExecutionStatusType](./literals.md#stageexecutionstatustype)
- [StageRetryModeType](./literals.md#stageretrymodetype)
- [StageTransitionTypeType](./literals.md#stagetransitiontypetype)
- [StartTimeRangeType](./literals.md#starttimerangetype)
- [TriggerTypeType](./literals.md#triggertypetype)
- [WebhookAuthenticationTypeType](./literals.md#webhookauthenticationtypetype)
- [CodePipelineServiceName](./literals.md#codepipelineservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AWSSessionCredentialsTypeDef](./type_defs.md#awssessioncredentialstypedef)
- [AcknowledgeJobInputRequestTypeDef](./type_defs.md#acknowledgejobinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AcknowledgeThirdPartyJobInputRequestTypeDef](./type_defs.md#acknowledgethirdpartyjobinputrequesttypedef)
- [ActionConfigurationPropertyTypeDef](./type_defs.md#actionconfigurationpropertytypedef)
- [ActionConfigurationTypeDef](./type_defs.md#actionconfigurationtypedef)
- [ActionContextTypeDef](./type_defs.md#actioncontexttypedef)
- [ActionTypeIdTypeDef](./type_defs.md#actiontypeidtypedef)
- [InputArtifactTypeDef](./type_defs.md#inputartifacttypedef)
- [OutputArtifactOutputTypeDef](./type_defs.md#outputartifactoutputtypedef)
- [LatestInPipelineExecutionFilterTypeDef](./type_defs.md#latestinpipelineexecutionfiltertypedef)
- [ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef)
- [ActionRevisionOutputTypeDef](./type_defs.md#actionrevisionoutputtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ActionTypeArtifactDetailsTypeDef](./type_defs.md#actiontypeartifactdetailstypedef)
- [ActionTypeIdentifierTypeDef](./type_defs.md#actiontypeidentifiertypedef)
- [ActionTypePermissionsOutputTypeDef](./type_defs.md#actiontypepermissionsoutputtypedef)
- [ActionTypePropertyTypeDef](./type_defs.md#actiontypepropertytypedef)
- [ActionTypeUrlsTypeDef](./type_defs.md#actiontypeurlstypedef)
- [ActionTypePermissionsTypeDef](./type_defs.md#actiontypepermissionstypedef)
- [ActionTypeSettingsTypeDef](./type_defs.md#actiontypesettingstypedef)
- [ArtifactDetailsTypeDef](./type_defs.md#artifactdetailstypedef)
- [ApprovalResultTypeDef](./type_defs.md#approvalresulttypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [S3ArtifactLocationTypeDef](./type_defs.md#s3artifactlocationtypedef)
- [ArtifactRevisionTypeDef](./type_defs.md#artifactrevisiontypedef)
- [EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef)
- [BlockerDeclarationTypeDef](./type_defs.md#blockerdeclarationtypedef)
- [ConditionExecutionTypeDef](./type_defs.md#conditionexecutiontypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DeleteCustomActionTypeInputRequestTypeDef](./type_defs.md#deletecustomactiontypeinputrequesttypedef)
- [DeletePipelineInputRequestTypeDef](./type_defs.md#deletepipelineinputrequesttypedef)
- [DeleteWebhookInputRequestTypeDef](./type_defs.md#deletewebhookinputrequesttypedef)
- [DeregisterWebhookWithThirdPartyInputRequestTypeDef](./type_defs.md#deregisterwebhookwiththirdpartyinputrequesttypedef)
- [DisableStageTransitionInputRequestTypeDef](./type_defs.md#disablestagetransitioninputrequesttypedef)
- [EnableStageTransitionInputRequestTypeDef](./type_defs.md#enablestagetransitioninputrequesttypedef)
- [ExecutionDetailsTypeDef](./type_defs.md#executiondetailstypedef)
- [ExecutionTriggerTypeDef](./type_defs.md#executiontriggertypedef)
- [JobWorkerExecutorConfigurationOutputTypeDef](./type_defs.md#jobworkerexecutorconfigurationoutputtypedef)
- [LambdaExecutorConfigurationTypeDef](./type_defs.md#lambdaexecutorconfigurationtypedef)
- [RetryConfigurationTypeDef](./type_defs.md#retryconfigurationtypedef)
- [FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef)
- [GetActionTypeInputRequestTypeDef](./type_defs.md#getactiontypeinputrequesttypedef)
- [GetJobDetailsInputRequestTypeDef](./type_defs.md#getjobdetailsinputrequesttypedef)
- [GetPipelineExecutionInputRequestTypeDef](./type_defs.md#getpipelineexecutioninputrequesttypedef)
- [GetPipelineInputRequestTypeDef](./type_defs.md#getpipelineinputrequesttypedef)
- [PipelineMetadataTypeDef](./type_defs.md#pipelinemetadatatypedef)
- [GetPipelineStateInputRequestTypeDef](./type_defs.md#getpipelinestateinputrequesttypedef)
- [GetThirdPartyJobDetailsInputRequestTypeDef](./type_defs.md#getthirdpartyjobdetailsinputrequesttypedef)
- [GitBranchFilterCriteriaOutputTypeDef](./type_defs.md#gitbranchfiltercriteriaoutputtypedef)
- [GitBranchFilterCriteriaTypeDef](./type_defs.md#gitbranchfiltercriteriatypedef)
- [GitFilePathFilterCriteriaOutputTypeDef](./type_defs.md#gitfilepathfiltercriteriaoutputtypedef)
- [GitFilePathFilterCriteriaTypeDef](./type_defs.md#gitfilepathfiltercriteriatypedef)
- [GitTagFilterCriteriaOutputTypeDef](./type_defs.md#gittagfiltercriteriaoutputtypedef)
- [GitTagFilterCriteriaTypeDef](./type_defs.md#gittagfiltercriteriatypedef)
- [JobWorkerExecutorConfigurationTypeDef](./type_defs.md#jobworkerexecutorconfigurationtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListActionTypesInputRequestTypeDef](./type_defs.md#listactiontypesinputrequesttypedef)
- [ListPipelinesInputRequestTypeDef](./type_defs.md#listpipelinesinputrequesttypedef)
- [PipelineSummaryTypeDef](./type_defs.md#pipelinesummarytypedef)
- [ListRuleTypesInputRequestTypeDef](./type_defs.md#listruletypesinputrequesttypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ListWebhooksInputRequestTypeDef](./type_defs.md#listwebhooksinputrequesttypedef)
- [OutputArtifactTypeDef](./type_defs.md#outputartifacttypedef)
- [OverrideStageConditionInputRequestTypeDef](./type_defs.md#overridestageconditioninputrequesttypedef)
- [StageContextTypeDef](./type_defs.md#stagecontexttypedef)
- [PipelineVariableDeclarationTypeDef](./type_defs.md#pipelinevariabledeclarationtypedef)
- [SucceededInStageFilterTypeDef](./type_defs.md#succeededinstagefiltertypedef)
- [PipelineRollbackMetadataTypeDef](./type_defs.md#pipelinerollbackmetadatatypedef)
- [SourceRevisionTypeDef](./type_defs.md#sourcerevisiontypedef)
- [StopExecutionTriggerTypeDef](./type_defs.md#stopexecutiontriggertypedef)
- [ResolvedPipelineVariableTypeDef](./type_defs.md#resolvedpipelinevariabletypedef)
- [PipelineVariableTypeDef](./type_defs.md#pipelinevariabletypedef)
- [ThirdPartyJobTypeDef](./type_defs.md#thirdpartyjobtypedef)
- [RegisterWebhookWithThirdPartyInputRequestTypeDef](./type_defs.md#registerwebhookwiththirdpartyinputrequesttypedef)
- [RetryStageExecutionInputRequestTypeDef](./type_defs.md#retrystageexecutioninputrequesttypedef)
- [RetryStageMetadataTypeDef](./type_defs.md#retrystagemetadatatypedef)
- [RollbackStageInputRequestTypeDef](./type_defs.md#rollbackstageinputrequesttypedef)
- [RuleConfigurationPropertyTypeDef](./type_defs.md#ruleconfigurationpropertytypedef)
- [RuleTypeIdTypeDef](./type_defs.md#ruletypeidtypedef)
- [RuleRevisionTypeDef](./type_defs.md#rulerevisiontypedef)
- [RuleTypeSettingsTypeDef](./type_defs.md#ruletypesettingstypedef)
- [SourceRevisionOverrideTypeDef](./type_defs.md#sourcerevisionoverridetypedef)
- [StageConditionsExecutionTypeDef](./type_defs.md#stageconditionsexecutiontypedef)
- [StageExecutionTypeDef](./type_defs.md#stageexecutiontypedef)
- [TransitionStateTypeDef](./type_defs.md#transitionstatetypedef)
- [StopPipelineExecutionInputRequestTypeDef](./type_defs.md#stoppipelineexecutioninputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [WebhookAuthConfigurationTypeDef](./type_defs.md#webhookauthconfigurationtypedef)
- [WebhookFilterRuleTypeDef](./type_defs.md#webhookfilterruletypedef)
- [AcknowledgeJobOutputTypeDef](./type_defs.md#acknowledgejoboutputtypedef)
- [AcknowledgeThirdPartyJobOutputTypeDef](./type_defs.md#acknowledgethirdpartyjoboutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [PutActionRevisionOutputTypeDef](./type_defs.md#putactionrevisionoutputtypedef)
- [PutApprovalResultOutputTypeDef](./type_defs.md#putapprovalresultoutputtypedef)
- [RetryStageExecutionOutputTypeDef](./type_defs.md#retrystageexecutionoutputtypedef)
- [RollbackStageOutputTypeDef](./type_defs.md#rollbackstageoutputtypedef)
- [StartPipelineExecutionOutputTypeDef](./type_defs.md#startpipelineexecutionoutputtypedef)
- [StopPipelineExecutionOutputTypeDef](./type_defs.md#stoppipelineexecutionoutputtypedef)
- [PollForJobsInputRequestTypeDef](./type_defs.md#pollforjobsinputrequesttypedef)
- [PollForThirdPartyJobsInputRequestTypeDef](./type_defs.md#pollforthirdpartyjobsinputrequesttypedef)
- [ActionDeclarationOutputTypeDef](./type_defs.md#actiondeclarationoutputtypedef)
- [ActionExecutionFilterTypeDef](./type_defs.md#actionexecutionfiltertypedef)
- [RuleExecutionFilterTypeDef](./type_defs.md#ruleexecutionfiltertypedef)
- [ActionExecutionResultTypeDef](./type_defs.md#actionexecutionresulttypedef)
- [ActionExecutionTypeDef](./type_defs.md#actionexecutiontypedef)
- [RuleExecutionResultTypeDef](./type_defs.md#ruleexecutionresulttypedef)
- [RuleExecutionTypeDef](./type_defs.md#ruleexecutiontypedef)
- [ActionRevisionTypeDef](./type_defs.md#actionrevisiontypedef)
- [CurrentRevisionTypeDef](./type_defs.md#currentrevisiontypedef)
- [ActionTypePermissionsUnionTypeDef](./type_defs.md#actiontypepermissionsuniontypedef)
- [ActionTypeTypeDef](./type_defs.md#actiontypetypedef)
- [PutApprovalResultInputRequestTypeDef](./type_defs.md#putapprovalresultinputrequesttypedef)
- [ArtifactDetailTypeDef](./type_defs.md#artifactdetailtypedef)
- [ArtifactLocationTypeDef](./type_defs.md#artifactlocationtypedef)
- [ArtifactStoreTypeDef](./type_defs.md#artifactstoretypedef)
- [CreateCustomActionTypeInputRequestTypeDef](./type_defs.md#createcustomactiontypeinputrequesttypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [ExecutorConfigurationOutputTypeDef](./type_defs.md#executorconfigurationoutputtypedef)
- [PutJobFailureResultInputRequestTypeDef](./type_defs.md#putjobfailureresultinputrequesttypedef)
- [PutThirdPartyJobFailureResultInputRequestTypeDef](./type_defs.md#putthirdpartyjobfailureresultinputrequesttypedef)
- [GitBranchFilterCriteriaUnionTypeDef](./type_defs.md#gitbranchfiltercriteriauniontypedef)
- [GitPullRequestFilterOutputTypeDef](./type_defs.md#gitpullrequestfilteroutputtypedef)
- [GitFilePathFilterCriteriaUnionTypeDef](./type_defs.md#gitfilepathfiltercriteriauniontypedef)
- [GitPushFilterOutputTypeDef](./type_defs.md#gitpushfilteroutputtypedef)
- [GitTagFilterCriteriaUnionTypeDef](./type_defs.md#gittagfiltercriteriauniontypedef)
- [JobWorkerExecutorConfigurationUnionTypeDef](./type_defs.md#jobworkerexecutorconfigurationuniontypedef)
- [ListActionTypesInputListActionTypesPaginateTypeDef](./type_defs.md#listactiontypesinputlistactiontypespaginatetypedef)
- [ListPipelinesInputListPipelinesPaginateTypeDef](./type_defs.md#listpipelinesinputlistpipelinespaginatetypedef)
- [ListTagsForResourceInputListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourceinputlisttagsforresourcepaginatetypedef)
- [ListWebhooksInputListWebhooksPaginateTypeDef](./type_defs.md#listwebhooksinputlistwebhookspaginatetypedef)
- [ListPipelinesOutputTypeDef](./type_defs.md#listpipelinesoutputtypedef)
- [OutputArtifactUnionTypeDef](./type_defs.md#outputartifactuniontypedef)
- [PipelineContextTypeDef](./type_defs.md#pipelinecontexttypedef)
- [PipelineExecutionFilterTypeDef](./type_defs.md#pipelineexecutionfiltertypedef)
- [PipelineExecutionSummaryTypeDef](./type_defs.md#pipelineexecutionsummarytypedef)
- [PipelineExecutionTypeDef](./type_defs.md#pipelineexecutiontypedef)
- [PollForThirdPartyJobsOutputTypeDef](./type_defs.md#pollforthirdpartyjobsoutputtypedef)
- [RuleDeclarationOutputTypeDef](./type_defs.md#ruledeclarationoutputtypedef)
- [RuleDeclarationTypeDef](./type_defs.md#ruledeclarationtypedef)
- [RuleTypeTypeDef](./type_defs.md#ruletypetypedef)
- [StartPipelineExecutionInputRequestTypeDef](./type_defs.md#startpipelineexecutioninputrequesttypedef)
- [WebhookDefinitionOutputTypeDef](./type_defs.md#webhookdefinitionoutputtypedef)
- [WebhookDefinitionTypeDef](./type_defs.md#webhookdefinitiontypedef)
- [ListActionExecutionsInputListActionExecutionsPaginateTypeDef](./type_defs.md#listactionexecutionsinputlistactionexecutionspaginatetypedef)
- [ListActionExecutionsInputRequestTypeDef](./type_defs.md#listactionexecutionsinputrequesttypedef)
- [ListRuleExecutionsInputListRuleExecutionsPaginateTypeDef](./type_defs.md#listruleexecutionsinputlistruleexecutionspaginatetypedef)
- [ListRuleExecutionsInputRequestTypeDef](./type_defs.md#listruleexecutionsinputrequesttypedef)
- [ActionStateTypeDef](./type_defs.md#actionstatetypedef)
- [RuleExecutionOutputTypeDef](./type_defs.md#ruleexecutionoutputtypedef)
- [RuleStateTypeDef](./type_defs.md#rulestatetypedef)
- [PutActionRevisionInputRequestTypeDef](./type_defs.md#putactionrevisioninputrequesttypedef)
- [PutJobSuccessResultInputRequestTypeDef](./type_defs.md#putjobsuccessresultinputrequesttypedef)
- [PutThirdPartyJobSuccessResultInputRequestTypeDef](./type_defs.md#putthirdpartyjobsuccessresultinputrequesttypedef)
- [CreateCustomActionTypeOutputTypeDef](./type_defs.md#createcustomactiontypeoutputtypedef)
- [ListActionTypesOutputTypeDef](./type_defs.md#listactiontypesoutputtypedef)
- [ActionExecutionInputTypeDef](./type_defs.md#actionexecutioninputtypedef)
- [ActionExecutionOutputTypeDef](./type_defs.md#actionexecutionoutputtypedef)
- [RuleExecutionInputTypeDef](./type_defs.md#ruleexecutioninputtypedef)
- [ArtifactTypeDef](./type_defs.md#artifacttypedef)
- [ActionTypeExecutorOutputTypeDef](./type_defs.md#actiontypeexecutoroutputtypedef)
- [GitPullRequestFilterTypeDef](./type_defs.md#gitpullrequestfiltertypedef)
- [GitConfigurationOutputTypeDef](./type_defs.md#gitconfigurationoutputtypedef)
- [GitPushFilterTypeDef](./type_defs.md#gitpushfiltertypedef)
- [ExecutorConfigurationTypeDef](./type_defs.md#executorconfigurationtypedef)
- [ActionDeclarationTypeDef](./type_defs.md#actiondeclarationtypedef)
- [ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef](./type_defs.md#listpipelineexecutionsinputlistpipelineexecutionspaginatetypedef)
- [ListPipelineExecutionsInputRequestTypeDef](./type_defs.md#listpipelineexecutionsinputrequesttypedef)
- [ListPipelineExecutionsOutputTypeDef](./type_defs.md#listpipelineexecutionsoutputtypedef)
- [GetPipelineExecutionOutputTypeDef](./type_defs.md#getpipelineexecutionoutputtypedef)
- [ConditionOutputTypeDef](./type_defs.md#conditionoutputtypedef)
- [RuleDeclarationUnionTypeDef](./type_defs.md#ruledeclarationuniontypedef)
- [ListRuleTypesOutputTypeDef](./type_defs.md#listruletypesoutputtypedef)
- [ListWebhookItemTypeDef](./type_defs.md#listwebhookitemtypedef)
- [PutWebhookInputRequestTypeDef](./type_defs.md#putwebhookinputrequesttypedef)
- [ConditionStateTypeDef](./type_defs.md#conditionstatetypedef)
- [ActionExecutionDetailTypeDef](./type_defs.md#actionexecutiondetailtypedef)
- [RuleExecutionDetailTypeDef](./type_defs.md#ruleexecutiondetailtypedef)
- [JobDataTypeDef](./type_defs.md#jobdatatypedef)
- [ThirdPartyJobDataTypeDef](./type_defs.md#thirdpartyjobdatatypedef)
- [ActionTypeDeclarationOutputTypeDef](./type_defs.md#actiontypedeclarationoutputtypedef)
- [GitPullRequestFilterUnionTypeDef](./type_defs.md#gitpullrequestfilteruniontypedef)
- [PipelineTriggerDeclarationOutputTypeDef](./type_defs.md#pipelinetriggerdeclarationoutputtypedef)
- [GitPushFilterUnionTypeDef](./type_defs.md#gitpushfilteruniontypedef)
- [ExecutorConfigurationUnionTypeDef](./type_defs.md#executorconfigurationuniontypedef)
- [ActionDeclarationUnionTypeDef](./type_defs.md#actiondeclarationuniontypedef)
- [BeforeEntryConditionsOutputTypeDef](./type_defs.md#beforeentryconditionsoutputtypedef)
- [FailureConditionsOutputTypeDef](./type_defs.md#failureconditionsoutputtypedef)
- [SuccessConditionsOutputTypeDef](./type_defs.md#successconditionsoutputtypedef)
- [ConditionTypeDef](./type_defs.md#conditiontypedef)
- [ListWebhooksOutputTypeDef](./type_defs.md#listwebhooksoutputtypedef)
- [PutWebhookOutputTypeDef](./type_defs.md#putwebhookoutputtypedef)
- [StageConditionStateTypeDef](./type_defs.md#stageconditionstatetypedef)
- [ListActionExecutionsOutputTypeDef](./type_defs.md#listactionexecutionsoutputtypedef)
- [ListRuleExecutionsOutputTypeDef](./type_defs.md#listruleexecutionsoutputtypedef)
- [JobDetailsTypeDef](./type_defs.md#jobdetailstypedef)
- [JobTypeDef](./type_defs.md#jobtypedef)
- [ThirdPartyJobDetailsTypeDef](./type_defs.md#thirdpartyjobdetailstypedef)
- [GetActionTypeOutputTypeDef](./type_defs.md#getactiontypeoutputtypedef)
- [GitConfigurationTypeDef](./type_defs.md#gitconfigurationtypedef)
- [ActionTypeExecutorTypeDef](./type_defs.md#actiontypeexecutortypedef)
- [StageDeclarationOutputTypeDef](./type_defs.md#stagedeclarationoutputtypedef)
- [BeforeEntryConditionsTypeDef](./type_defs.md#beforeentryconditionstypedef)
- [ConditionUnionTypeDef](./type_defs.md#conditionuniontypedef)
- [SuccessConditionsTypeDef](./type_defs.md#successconditionstypedef)
- [StageStateTypeDef](./type_defs.md#stagestatetypedef)
- [GetJobDetailsOutputTypeDef](./type_defs.md#getjobdetailsoutputtypedef)
- [PollForJobsOutputTypeDef](./type_defs.md#pollforjobsoutputtypedef)
- [GetThirdPartyJobDetailsOutputTypeDef](./type_defs.md#getthirdpartyjobdetailsoutputtypedef)
- [GitConfigurationUnionTypeDef](./type_defs.md#gitconfigurationuniontypedef)
- [ActionTypeExecutorUnionTypeDef](./type_defs.md#actiontypeexecutoruniontypedef)
- [PipelineDeclarationOutputTypeDef](./type_defs.md#pipelinedeclarationoutputtypedef)
- [BeforeEntryConditionsUnionTypeDef](./type_defs.md#beforeentryconditionsuniontypedef)
- [FailureConditionsTypeDef](./type_defs.md#failureconditionstypedef)
- [SuccessConditionsUnionTypeDef](./type_defs.md#successconditionsuniontypedef)
- [GetPipelineStateOutputTypeDef](./type_defs.md#getpipelinestateoutputtypedef)
- [PipelineTriggerDeclarationTypeDef](./type_defs.md#pipelinetriggerdeclarationtypedef)
- [ActionTypeDeclarationTypeDef](./type_defs.md#actiontypedeclarationtypedef)
- [CreatePipelineOutputTypeDef](./type_defs.md#createpipelineoutputtypedef)
- [GetPipelineOutputTypeDef](./type_defs.md#getpipelineoutputtypedef)
- [UpdatePipelineOutputTypeDef](./type_defs.md#updatepipelineoutputtypedef)
- [FailureConditionsUnionTypeDef](./type_defs.md#failureconditionsuniontypedef)
- [PipelineTriggerDeclarationUnionTypeDef](./type_defs.md#pipelinetriggerdeclarationuniontypedef)
- [UpdateActionTypeInputRequestTypeDef](./type_defs.md#updateactiontypeinputrequesttypedef)
- [StageDeclarationTypeDef](./type_defs.md#stagedeclarationtypedef)
- [StageDeclarationUnionTypeDef](./type_defs.md#stagedeclarationuniontypedef)
- [PipelineDeclarationTypeDef](./type_defs.md#pipelinedeclarationtypedef)
- [CreatePipelineInputRequestTypeDef](./type_defs.md#createpipelineinputrequesttypedef)
- [UpdatePipelineInputRequestTypeDef](./type_defs.md#updatepipelineinputrequesttypedef)

