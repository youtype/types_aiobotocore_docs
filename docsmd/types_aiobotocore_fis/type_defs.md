# Type definitions

> [Index](../README.md) > [FIS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [FIS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#fis)
    type annotations stubs module [types-aiobotocore-fis](https://pypi.org/project/types-aiobotocore-fis/).



## ActionParameterTypeDef

```python
# ActionParameterTypeDef definition

class ActionParameterTypeDef(TypedDict):
    description: NotRequired[str],
    required: NotRequired[bool],
```

## ActionTargetTypeDef

```python
# ActionTargetTypeDef definition

class ActionTargetTypeDef(TypedDict):
    resourceType: NotRequired[str],
```

## CreateExperimentTemplateActionInputTypeDef

```python
# CreateExperimentTemplateActionInputTypeDef definition

class CreateExperimentTemplateActionInputTypeDef(TypedDict):
    actionId: str,
    description: NotRequired[str],
    parameters: NotRequired[Mapping[str, str]],
    targets: NotRequired[Mapping[str, str]],
    startAfter: NotRequired[Sequence[str]],
```

## CreateExperimentTemplateExperimentOptionsInputTypeDef

```python
# CreateExperimentTemplateExperimentOptionsInputTypeDef definition

class CreateExperimentTemplateExperimentOptionsInputTypeDef(TypedDict):
    accountTargeting: NotRequired[AccountTargetingType],  # (1)
    emptyTargetResolutionMode: NotRequired[EmptyTargetResolutionModeType],  # (2)
```

1. See [:material-code-brackets: AccountTargetingType](./literals.md#accounttargetingtype) 
2. See [:material-code-brackets: EmptyTargetResolutionModeType](./literals.md#emptytargetresolutionmodetype) 
## ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef

```python
# ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef definition

class ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef(TypedDict):
    logGroupArn: str,
```

## ExperimentTemplateS3LogConfigurationInputTypeDef

```python
# ExperimentTemplateS3LogConfigurationInputTypeDef definition

class ExperimentTemplateS3LogConfigurationInputTypeDef(TypedDict):
    bucketName: str,
    prefix: NotRequired[str],
```

## CreateExperimentTemplateStopConditionInputTypeDef

```python
# CreateExperimentTemplateStopConditionInputTypeDef definition

class CreateExperimentTemplateStopConditionInputTypeDef(TypedDict):
    source: str,
    value: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## ExperimentTemplateTargetInputFilterTypeDef

```python
# ExperimentTemplateTargetInputFilterTypeDef definition

class ExperimentTemplateTargetInputFilterTypeDef(TypedDict):
    path: str,
    values: Sequence[str],
```

## CreateTargetAccountConfigurationRequestRequestTypeDef

```python
# CreateTargetAccountConfigurationRequestRequestTypeDef definition

class CreateTargetAccountConfigurationRequestRequestTypeDef(TypedDict):
    experimentTemplateId: str,
    accountId: str,
    roleArn: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

## TargetAccountConfigurationTypeDef

```python
# TargetAccountConfigurationTypeDef definition

class TargetAccountConfigurationTypeDef(TypedDict):
    roleArn: NotRequired[str],
    accountId: NotRequired[str],
    description: NotRequired[str],
```

## DeleteExperimentTemplateRequestRequestTypeDef

```python
# DeleteExperimentTemplateRequestRequestTypeDef definition

class DeleteExperimentTemplateRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteTargetAccountConfigurationRequestRequestTypeDef

```python
# DeleteTargetAccountConfigurationRequestRequestTypeDef definition

class DeleteTargetAccountConfigurationRequestRequestTypeDef(TypedDict):
    experimentTemplateId: str,
    accountId: str,
```

## ExperimentActionStateTypeDef

```python
# ExperimentActionStateTypeDef definition

class ExperimentActionStateTypeDef(TypedDict):
    status: NotRequired[ExperimentActionStatusType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: ExperimentActionStatusType](./literals.md#experimentactionstatustype) 
## ExperimentCloudWatchLogsLogConfigurationTypeDef

```python
# ExperimentCloudWatchLogsLogConfigurationTypeDef definition

class ExperimentCloudWatchLogsLogConfigurationTypeDef(TypedDict):
    logGroupArn: NotRequired[str],
```

## ExperimentErrorTypeDef

```python
# ExperimentErrorTypeDef definition

class ExperimentErrorTypeDef(TypedDict):
    accountId: NotRequired[str],
    code: NotRequired[str],
    location: NotRequired[str],
```

## ExperimentS3LogConfigurationTypeDef

```python
# ExperimentS3LogConfigurationTypeDef definition

class ExperimentS3LogConfigurationTypeDef(TypedDict):
    bucketName: NotRequired[str],
    prefix: NotRequired[str],
```

## ExperimentOptionsTypeDef

```python
# ExperimentOptionsTypeDef definition

class ExperimentOptionsTypeDef(TypedDict):
    accountTargeting: NotRequired[AccountTargetingType],  # (1)
    emptyTargetResolutionMode: NotRequired[EmptyTargetResolutionModeType],  # (2)
    actionsMode: NotRequired[ActionsModeType],  # (3)
```

1. See [:material-code-brackets: AccountTargetingType](./literals.md#accounttargetingtype) 
2. See [:material-code-brackets: EmptyTargetResolutionModeType](./literals.md#emptytargetresolutionmodetype) 
3. See [:material-code-brackets: ActionsModeType](./literals.md#actionsmodetype) 
## ExperimentReportConfigurationCloudWatchDashboardTypeDef

```python
# ExperimentReportConfigurationCloudWatchDashboardTypeDef definition

class ExperimentReportConfigurationCloudWatchDashboardTypeDef(TypedDict):
    dashboardIdentifier: NotRequired[str],
```

## ExperimentReportConfigurationOutputsS3ConfigurationTypeDef

```python
# ExperimentReportConfigurationOutputsS3ConfigurationTypeDef definition

class ExperimentReportConfigurationOutputsS3ConfigurationTypeDef(TypedDict):
    bucketName: NotRequired[str],
    prefix: NotRequired[str],
```

## ExperimentReportErrorTypeDef

```python
# ExperimentReportErrorTypeDef definition

class ExperimentReportErrorTypeDef(TypedDict):
    code: NotRequired[str],
```

## ExperimentReportS3ReportTypeDef

```python
# ExperimentReportS3ReportTypeDef definition

class ExperimentReportS3ReportTypeDef(TypedDict):
    arn: NotRequired[str],
    reportType: NotRequired[str],
```

## ExperimentStopConditionTypeDef

```python
# ExperimentStopConditionTypeDef definition

class ExperimentStopConditionTypeDef(TypedDict):
    source: NotRequired[str],
    value: NotRequired[str],
```

## ExperimentTargetAccountConfigurationSummaryTypeDef

```python
# ExperimentTargetAccountConfigurationSummaryTypeDef definition

class ExperimentTargetAccountConfigurationSummaryTypeDef(TypedDict):
    roleArn: NotRequired[str],
    accountId: NotRequired[str],
    description: NotRequired[str],
```

## ExperimentTargetAccountConfigurationTypeDef

```python
# ExperimentTargetAccountConfigurationTypeDef definition

class ExperimentTargetAccountConfigurationTypeDef(TypedDict):
    roleArn: NotRequired[str],
    accountId: NotRequired[str],
    description: NotRequired[str],
```

## ExperimentTargetFilterTypeDef

```python
# ExperimentTargetFilterTypeDef definition

class ExperimentTargetFilterTypeDef(TypedDict):
    path: NotRequired[str],
    values: NotRequired[List[str]],
```

## ExperimentTemplateActionTypeDef

```python
# ExperimentTemplateActionTypeDef definition

class ExperimentTemplateActionTypeDef(TypedDict):
    actionId: NotRequired[str],
    description: NotRequired[str],
    parameters: NotRequired[Dict[str, str]],
    targets: NotRequired[Dict[str, str]],
    startAfter: NotRequired[List[str]],
```

## ExperimentTemplateCloudWatchLogsLogConfigurationTypeDef

```python
# ExperimentTemplateCloudWatchLogsLogConfigurationTypeDef definition

class ExperimentTemplateCloudWatchLogsLogConfigurationTypeDef(TypedDict):
    logGroupArn: NotRequired[str],
```

## ExperimentTemplateExperimentOptionsTypeDef

```python
# ExperimentTemplateExperimentOptionsTypeDef definition

class ExperimentTemplateExperimentOptionsTypeDef(TypedDict):
    accountTargeting: NotRequired[AccountTargetingType],  # (1)
    emptyTargetResolutionMode: NotRequired[EmptyTargetResolutionModeType],  # (2)
```

1. See [:material-code-brackets: AccountTargetingType](./literals.md#accounttargetingtype) 
2. See [:material-code-brackets: EmptyTargetResolutionModeType](./literals.md#emptytargetresolutionmodetype) 
## ExperimentTemplateS3LogConfigurationTypeDef

```python
# ExperimentTemplateS3LogConfigurationTypeDef definition

class ExperimentTemplateS3LogConfigurationTypeDef(TypedDict):
    bucketName: NotRequired[str],
    prefix: NotRequired[str],
```

## ExperimentTemplateReportConfigurationCloudWatchDashboardTypeDef

```python
# ExperimentTemplateReportConfigurationCloudWatchDashboardTypeDef definition

class ExperimentTemplateReportConfigurationCloudWatchDashboardTypeDef(TypedDict):
    dashboardIdentifier: NotRequired[str],
```

## ReportConfigurationCloudWatchDashboardInputTypeDef

```python
# ReportConfigurationCloudWatchDashboardInputTypeDef definition

class ReportConfigurationCloudWatchDashboardInputTypeDef(TypedDict):
    dashboardIdentifier: NotRequired[str],
```

## ReportConfigurationS3OutputInputTypeDef

```python
# ReportConfigurationS3OutputInputTypeDef definition

class ReportConfigurationS3OutputInputTypeDef(TypedDict):
    bucketName: NotRequired[str],
    prefix: NotRequired[str],
```

## ReportConfigurationS3OutputTypeDef

```python
# ReportConfigurationS3OutputTypeDef definition

class ReportConfigurationS3OutputTypeDef(TypedDict):
    bucketName: NotRequired[str],
    prefix: NotRequired[str],
```

## ExperimentTemplateStopConditionTypeDef

```python
# ExperimentTemplateStopConditionTypeDef definition

class ExperimentTemplateStopConditionTypeDef(TypedDict):
    source: NotRequired[str],
    value: NotRequired[str],
```

## ExperimentTemplateSummaryTypeDef

```python
# ExperimentTemplateSummaryTypeDef definition

class ExperimentTemplateSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    description: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
```

## ExperimentTemplateTargetFilterTypeDef

```python
# ExperimentTemplateTargetFilterTypeDef definition

class ExperimentTemplateTargetFilterTypeDef(TypedDict):
    path: NotRequired[str],
    values: NotRequired[List[str]],
```

## GetActionRequestRequestTypeDef

```python
# GetActionRequestRequestTypeDef definition

class GetActionRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetExperimentRequestRequestTypeDef

```python
# GetExperimentRequestRequestTypeDef definition

class GetExperimentRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetExperimentTargetAccountConfigurationRequestRequestTypeDef

```python
# GetExperimentTargetAccountConfigurationRequestRequestTypeDef definition

class GetExperimentTargetAccountConfigurationRequestRequestTypeDef(TypedDict):
    experimentId: str,
    accountId: str,
```

## GetExperimentTemplateRequestRequestTypeDef

```python
# GetExperimentTemplateRequestRequestTypeDef definition

class GetExperimentTemplateRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetSafetyLeverRequestRequestTypeDef

```python
# GetSafetyLeverRequestRequestTypeDef definition

class GetSafetyLeverRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetTargetAccountConfigurationRequestRequestTypeDef

```python
# GetTargetAccountConfigurationRequestRequestTypeDef definition

class GetTargetAccountConfigurationRequestRequestTypeDef(TypedDict):
    experimentTemplateId: str,
    accountId: str,
```

## GetTargetResourceTypeRequestRequestTypeDef

```python
# GetTargetResourceTypeRequestRequestTypeDef definition

class GetTargetResourceTypeRequestRequestTypeDef(TypedDict):
    resourceType: str,
```

## ListActionsRequestRequestTypeDef

```python
# ListActionsRequestRequestTypeDef definition

class ListActionsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListExperimentResolvedTargetsRequestRequestTypeDef

```python
# ListExperimentResolvedTargetsRequestRequestTypeDef definition

class ListExperimentResolvedTargetsRequestRequestTypeDef(TypedDict):
    experimentId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    targetName: NotRequired[str],
```

## ResolvedTargetTypeDef

```python
# ResolvedTargetTypeDef definition

class ResolvedTargetTypeDef(TypedDict):
    resourceType: NotRequired[str],
    targetName: NotRequired[str],
    targetInformation: NotRequired[Dict[str, str]],
```

## ListExperimentTargetAccountConfigurationsRequestRequestTypeDef

```python
# ListExperimentTargetAccountConfigurationsRequestRequestTypeDef definition

class ListExperimentTargetAccountConfigurationsRequestRequestTypeDef(TypedDict):
    experimentId: str,
    nextToken: NotRequired[str],
```

## ListExperimentTemplatesRequestRequestTypeDef

```python
# ListExperimentTemplatesRequestRequestTypeDef definition

class ListExperimentTemplatesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListExperimentsRequestRequestTypeDef

```python
# ListExperimentsRequestRequestTypeDef definition

class ListExperimentsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    experimentTemplateId: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTargetAccountConfigurationsRequestRequestTypeDef

```python
# ListTargetAccountConfigurationsRequestRequestTypeDef definition

class ListTargetAccountConfigurationsRequestRequestTypeDef(TypedDict):
    experimentTemplateId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## TargetAccountConfigurationSummaryTypeDef

```python
# TargetAccountConfigurationSummaryTypeDef definition

class TargetAccountConfigurationSummaryTypeDef(TypedDict):
    roleArn: NotRequired[str],
    accountId: NotRequired[str],
    description: NotRequired[str],
```

## ListTargetResourceTypesRequestRequestTypeDef

```python
# ListTargetResourceTypesRequestRequestTypeDef definition

class ListTargetResourceTypesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## TargetResourceTypeSummaryTypeDef

```python
# TargetResourceTypeSummaryTypeDef definition

class TargetResourceTypeSummaryTypeDef(TypedDict):
    resourceType: NotRequired[str],
    description: NotRequired[str],
```

## SafetyLeverStateTypeDef

```python
# SafetyLeverStateTypeDef definition

class SafetyLeverStateTypeDef(TypedDict):
    status: NotRequired[SafetyLeverStatusType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: SafetyLeverStatusType](./literals.md#safetyleverstatustype) 
## StartExperimentExperimentOptionsInputTypeDef

```python
# StartExperimentExperimentOptionsInputTypeDef definition

class StartExperimentExperimentOptionsInputTypeDef(TypedDict):
    actionsMode: NotRequired[ActionsModeType],  # (1)
```

1. See [:material-code-brackets: ActionsModeType](./literals.md#actionsmodetype) 
## StopExperimentRequestRequestTypeDef

```python
# StopExperimentRequestRequestTypeDef definition

class StopExperimentRequestRequestTypeDef(TypedDict):
    id: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TargetResourceTypeParameterTypeDef

```python
# TargetResourceTypeParameterTypeDef definition

class TargetResourceTypeParameterTypeDef(TypedDict):
    description: NotRequired[str],
    required: NotRequired[bool],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: NotRequired[Sequence[str]],
```

## UpdateExperimentTemplateActionInputItemTypeDef

```python
# UpdateExperimentTemplateActionInputItemTypeDef definition

class UpdateExperimentTemplateActionInputItemTypeDef(TypedDict):
    actionId: NotRequired[str],
    description: NotRequired[str],
    parameters: NotRequired[Mapping[str, str]],
    targets: NotRequired[Mapping[str, str]],
    startAfter: NotRequired[Sequence[str]],
```

## UpdateExperimentTemplateExperimentOptionsInputTypeDef

```python
# UpdateExperimentTemplateExperimentOptionsInputTypeDef definition

class UpdateExperimentTemplateExperimentOptionsInputTypeDef(TypedDict):
    emptyTargetResolutionMode: NotRequired[EmptyTargetResolutionModeType],  # (1)
```

1. See [:material-code-brackets: EmptyTargetResolutionModeType](./literals.md#emptytargetresolutionmodetype) 
## UpdateExperimentTemplateStopConditionInputTypeDef

```python
# UpdateExperimentTemplateStopConditionInputTypeDef definition

class UpdateExperimentTemplateStopConditionInputTypeDef(TypedDict):
    source: str,
    value: NotRequired[str],
```

## UpdateSafetyLeverStateInputTypeDef

```python
# UpdateSafetyLeverStateInputTypeDef definition

class UpdateSafetyLeverStateInputTypeDef(TypedDict):
    status: SafetyLeverStatusInputType,  # (1)
    reason: str,
```

1. See [:material-code-brackets: SafetyLeverStatusInputType](./literals.md#safetyleverstatusinputtype) 
## UpdateTargetAccountConfigurationRequestRequestTypeDef

```python
# UpdateTargetAccountConfigurationRequestRequestTypeDef definition

class UpdateTargetAccountConfigurationRequestRequestTypeDef(TypedDict):
    experimentTemplateId: str,
    accountId: str,
    roleArn: NotRequired[str],
    description: NotRequired[str],
```

## ActionSummaryTypeDef

```python
# ActionSummaryTypeDef definition

class ActionSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    description: NotRequired[str],
    targets: NotRequired[Dict[str, ActionTargetTypeDef]],  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    description: NotRequired[str],
    parameters: NotRequired[Dict[str, ActionParameterTypeDef]],  # (1)
    targets: NotRequired[Dict[str, ActionTargetTypeDef]],  # (2)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ActionParameterTypeDef](./type_defs.md#actionparametertypedef) 
2. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
## CreateExperimentTemplateLogConfigurationInputTypeDef

```python
# CreateExperimentTemplateLogConfigurationInputTypeDef definition

class CreateExperimentTemplateLogConfigurationInputTypeDef(TypedDict):
    logSchemaVersion: int,
    cloudWatchLogsConfiguration: NotRequired[ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef],  # (1)
    s3Configuration: NotRequired[ExperimentTemplateS3LogConfigurationInputTypeDef],  # (2)
```

1. See [:material-code-braces: ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef](./type_defs.md#experimenttemplatecloudwatchlogslogconfigurationinputtypedef) 
2. See [:material-code-braces: ExperimentTemplateS3LogConfigurationInputTypeDef](./type_defs.md#experimenttemplates3logconfigurationinputtypedef) 
## UpdateExperimentTemplateLogConfigurationInputTypeDef

```python
# UpdateExperimentTemplateLogConfigurationInputTypeDef definition

class UpdateExperimentTemplateLogConfigurationInputTypeDef(TypedDict):
    cloudWatchLogsConfiguration: NotRequired[ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef],  # (1)
    s3Configuration: NotRequired[ExperimentTemplateS3LogConfigurationInputTypeDef],  # (2)
    logSchemaVersion: NotRequired[int],
```

1. See [:material-code-braces: ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef](./type_defs.md#experimenttemplatecloudwatchlogslogconfigurationinputtypedef) 
2. See [:material-code-braces: ExperimentTemplateS3LogConfigurationInputTypeDef](./type_defs.md#experimenttemplates3logconfigurationinputtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExperimentTemplateTargetInputTypeDef

```python
# CreateExperimentTemplateTargetInputTypeDef definition

class CreateExperimentTemplateTargetInputTypeDef(TypedDict):
    resourceType: str,
    selectionMode: str,
    resourceArns: NotRequired[Sequence[str]],
    resourceTags: NotRequired[Mapping[str, str]],
    filters: NotRequired[Sequence[ExperimentTemplateTargetInputFilterTypeDef]],  # (1)
    parameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ExperimentTemplateTargetInputFilterTypeDef](./type_defs.md#experimenttemplatetargetinputfiltertypedef) 
## UpdateExperimentTemplateTargetInputTypeDef

```python
# UpdateExperimentTemplateTargetInputTypeDef definition

class UpdateExperimentTemplateTargetInputTypeDef(TypedDict):
    resourceType: str,
    selectionMode: str,
    resourceArns: NotRequired[Sequence[str]],
    resourceTags: NotRequired[Mapping[str, str]],
    filters: NotRequired[Sequence[ExperimentTemplateTargetInputFilterTypeDef]],  # (1)
    parameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ExperimentTemplateTargetInputFilterTypeDef](./type_defs.md#experimenttemplatetargetinputfiltertypedef) 
## CreateTargetAccountConfigurationResponseTypeDef

```python
# CreateTargetAccountConfigurationResponseTypeDef definition

class CreateTargetAccountConfigurationResponseTypeDef(TypedDict):
    targetAccountConfiguration: TargetAccountConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetAccountConfigurationTypeDef](./type_defs.md#targetaccountconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTargetAccountConfigurationResponseTypeDef

```python
# DeleteTargetAccountConfigurationResponseTypeDef definition

class DeleteTargetAccountConfigurationResponseTypeDef(TypedDict):
    targetAccountConfiguration: TargetAccountConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetAccountConfigurationTypeDef](./type_defs.md#targetaccountconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTargetAccountConfigurationResponseTypeDef

```python
# GetTargetAccountConfigurationResponseTypeDef definition

class GetTargetAccountConfigurationResponseTypeDef(TypedDict):
    targetAccountConfiguration: TargetAccountConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetAccountConfigurationTypeDef](./type_defs.md#targetaccountconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTargetAccountConfigurationResponseTypeDef

```python
# UpdateTargetAccountConfigurationResponseTypeDef definition

class UpdateTargetAccountConfigurationResponseTypeDef(TypedDict):
    targetAccountConfiguration: TargetAccountConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetAccountConfigurationTypeDef](./type_defs.md#targetaccountconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExperimentActionTypeDef

```python
# ExperimentActionTypeDef definition

class ExperimentActionTypeDef(TypedDict):
    actionId: NotRequired[str],
    description: NotRequired[str],
    parameters: NotRequired[Dict[str, str]],
    targets: NotRequired[Dict[str, str]],
    startAfter: NotRequired[List[str]],
    state: NotRequired[ExperimentActionStateTypeDef],  # (1)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

1. See [:material-code-braces: ExperimentActionStateTypeDef](./type_defs.md#experimentactionstatetypedef) 
## ExperimentStateTypeDef

```python
# ExperimentStateTypeDef definition

class ExperimentStateTypeDef(TypedDict):
    status: NotRequired[ExperimentStatusType],  # (1)
    reason: NotRequired[str],
    error: NotRequired[ExperimentErrorTypeDef],  # (2)
```

1. See [:material-code-brackets: ExperimentStatusType](./literals.md#experimentstatustype) 
2. See [:material-code-braces: ExperimentErrorTypeDef](./type_defs.md#experimenterrortypedef) 
## ExperimentLogConfigurationTypeDef

```python
# ExperimentLogConfigurationTypeDef definition

class ExperimentLogConfigurationTypeDef(TypedDict):
    cloudWatchLogsConfiguration: NotRequired[ExperimentCloudWatchLogsLogConfigurationTypeDef],  # (1)
    s3Configuration: NotRequired[ExperimentS3LogConfigurationTypeDef],  # (2)
    logSchemaVersion: NotRequired[int],
```

1. See [:material-code-braces: ExperimentCloudWatchLogsLogConfigurationTypeDef](./type_defs.md#experimentcloudwatchlogslogconfigurationtypedef) 
2. See [:material-code-braces: ExperimentS3LogConfigurationTypeDef](./type_defs.md#experiments3logconfigurationtypedef) 
## ExperimentReportConfigurationDataSourcesTypeDef

```python
# ExperimentReportConfigurationDataSourcesTypeDef definition

class ExperimentReportConfigurationDataSourcesTypeDef(TypedDict):
    cloudWatchDashboards: NotRequired[List[ExperimentReportConfigurationCloudWatchDashboardTypeDef]],  # (1)
```

1. See [:material-code-braces: ExperimentReportConfigurationCloudWatchDashboardTypeDef](./type_defs.md#experimentreportconfigurationcloudwatchdashboardtypedef) 
## ExperimentReportConfigurationOutputsTypeDef

```python
# ExperimentReportConfigurationOutputsTypeDef definition

class ExperimentReportConfigurationOutputsTypeDef(TypedDict):
    s3Configuration: NotRequired[ExperimentReportConfigurationOutputsS3ConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ExperimentReportConfigurationOutputsS3ConfigurationTypeDef](./type_defs.md#experimentreportconfigurationoutputss3configurationtypedef) 
## ExperimentReportStateTypeDef

```python
# ExperimentReportStateTypeDef definition

class ExperimentReportStateTypeDef(TypedDict):
    status: NotRequired[ExperimentReportStatusType],  # (1)
    reason: NotRequired[str],
    error: NotRequired[ExperimentReportErrorTypeDef],  # (2)
```

1. See [:material-code-brackets: ExperimentReportStatusType](./literals.md#experimentreportstatustype) 
2. See [:material-code-braces: ExperimentReportErrorTypeDef](./type_defs.md#experimentreporterrortypedef) 
## ListExperimentTargetAccountConfigurationsResponseTypeDef

```python
# ListExperimentTargetAccountConfigurationsResponseTypeDef definition

class ListExperimentTargetAccountConfigurationsResponseTypeDef(TypedDict):
    targetAccountConfigurations: List[ExperimentTargetAccountConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExperimentTargetAccountConfigurationSummaryTypeDef](./type_defs.md#experimenttargetaccountconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExperimentTargetAccountConfigurationResponseTypeDef

```python
# GetExperimentTargetAccountConfigurationResponseTypeDef definition

class GetExperimentTargetAccountConfigurationResponseTypeDef(TypedDict):
    targetAccountConfiguration: ExperimentTargetAccountConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTargetAccountConfigurationTypeDef](./type_defs.md#experimenttargetaccountconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExperimentTargetTypeDef

```python
# ExperimentTargetTypeDef definition

class ExperimentTargetTypeDef(TypedDict):
    resourceType: NotRequired[str],
    resourceArns: NotRequired[List[str]],
    resourceTags: NotRequired[Dict[str, str]],
    filters: NotRequired[List[ExperimentTargetFilterTypeDef]],  # (1)
    selectionMode: NotRequired[str],
    parameters: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ExperimentTargetFilterTypeDef](./type_defs.md#experimenttargetfiltertypedef) 
## ExperimentTemplateLogConfigurationTypeDef

```python
# ExperimentTemplateLogConfigurationTypeDef definition

class ExperimentTemplateLogConfigurationTypeDef(TypedDict):
    cloudWatchLogsConfiguration: NotRequired[ExperimentTemplateCloudWatchLogsLogConfigurationTypeDef],  # (1)
    s3Configuration: NotRequired[ExperimentTemplateS3LogConfigurationTypeDef],  # (2)
    logSchemaVersion: NotRequired[int],
```

1. See [:material-code-braces: ExperimentTemplateCloudWatchLogsLogConfigurationTypeDef](./type_defs.md#experimenttemplatecloudwatchlogslogconfigurationtypedef) 
2. See [:material-code-braces: ExperimentTemplateS3LogConfigurationTypeDef](./type_defs.md#experimenttemplates3logconfigurationtypedef) 
## ExperimentTemplateReportConfigurationDataSourcesTypeDef

```python
# ExperimentTemplateReportConfigurationDataSourcesTypeDef definition

class ExperimentTemplateReportConfigurationDataSourcesTypeDef(TypedDict):
    cloudWatchDashboards: NotRequired[List[ExperimentTemplateReportConfigurationCloudWatchDashboardTypeDef]],  # (1)
```

1. See [:material-code-braces: ExperimentTemplateReportConfigurationCloudWatchDashboardTypeDef](./type_defs.md#experimenttemplatereportconfigurationcloudwatchdashboardtypedef) 
## ExperimentTemplateReportConfigurationDataSourcesInputTypeDef

```python
# ExperimentTemplateReportConfigurationDataSourcesInputTypeDef definition

class ExperimentTemplateReportConfigurationDataSourcesInputTypeDef(TypedDict):
    cloudWatchDashboards: NotRequired[Sequence[ReportConfigurationCloudWatchDashboardInputTypeDef]],  # (1)
```

1. See [:material-code-braces: ReportConfigurationCloudWatchDashboardInputTypeDef](./type_defs.md#reportconfigurationcloudwatchdashboardinputtypedef) 
## ExperimentTemplateReportConfigurationOutputsInputTypeDef

```python
# ExperimentTemplateReportConfigurationOutputsInputTypeDef definition

class ExperimentTemplateReportConfigurationOutputsInputTypeDef(TypedDict):
    s3Configuration: NotRequired[ReportConfigurationS3OutputInputTypeDef],  # (1)
```

1. See [:material-code-braces: ReportConfigurationS3OutputInputTypeDef](./type_defs.md#reportconfigurations3outputinputtypedef) 
## ExperimentTemplateReportConfigurationOutputsTypeDef

```python
# ExperimentTemplateReportConfigurationOutputsTypeDef definition

class ExperimentTemplateReportConfigurationOutputsTypeDef(TypedDict):
    s3Configuration: NotRequired[ReportConfigurationS3OutputTypeDef],  # (1)
```

1. See [:material-code-braces: ReportConfigurationS3OutputTypeDef](./type_defs.md#reportconfigurations3outputtypedef) 
## ListExperimentTemplatesResponseTypeDef

```python
# ListExperimentTemplatesResponseTypeDef definition

class ListExperimentTemplatesResponseTypeDef(TypedDict):
    experimentTemplates: List[ExperimentTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExperimentTemplateSummaryTypeDef](./type_defs.md#experimenttemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExperimentTemplateTargetTypeDef

```python
# ExperimentTemplateTargetTypeDef definition

class ExperimentTemplateTargetTypeDef(TypedDict):
    resourceType: NotRequired[str],
    resourceArns: NotRequired[List[str]],
    resourceTags: NotRequired[Dict[str, str]],
    filters: NotRequired[List[ExperimentTemplateTargetFilterTypeDef]],  # (1)
    selectionMode: NotRequired[str],
    parameters: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ExperimentTemplateTargetFilterTypeDef](./type_defs.md#experimenttemplatetargetfiltertypedef) 
## ListExperimentResolvedTargetsResponseTypeDef

```python
# ListExperimentResolvedTargetsResponseTypeDef definition

class ListExperimentResolvedTargetsResponseTypeDef(TypedDict):
    resolvedTargets: List[ResolvedTargetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResolvedTargetTypeDef](./type_defs.md#resolvedtargettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTargetAccountConfigurationsResponseTypeDef

```python
# ListTargetAccountConfigurationsResponseTypeDef definition

class ListTargetAccountConfigurationsResponseTypeDef(TypedDict):
    targetAccountConfigurations: List[TargetAccountConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TargetAccountConfigurationSummaryTypeDef](./type_defs.md#targetaccountconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTargetResourceTypesResponseTypeDef

```python
# ListTargetResourceTypesResponseTypeDef definition

class ListTargetResourceTypesResponseTypeDef(TypedDict):
    targetResourceTypes: List[TargetResourceTypeSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TargetResourceTypeSummaryTypeDef](./type_defs.md#targetresourcetypesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SafetyLeverTypeDef

```python
# SafetyLeverTypeDef definition

class SafetyLeverTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    state: NotRequired[SafetyLeverStateTypeDef],  # (1)
```

1. See [:material-code-braces: SafetyLeverStateTypeDef](./type_defs.md#safetyleverstatetypedef) 
## StartExperimentRequestRequestTypeDef

```python
# StartExperimentRequestRequestTypeDef definition

class StartExperimentRequestRequestTypeDef(TypedDict):
    clientToken: str,
    experimentTemplateId: str,
    experimentOptions: NotRequired[StartExperimentExperimentOptionsInputTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: StartExperimentExperimentOptionsInputTypeDef](./type_defs.md#startexperimentexperimentoptionsinputtypedef) 
## TargetResourceTypeTypeDef

```python
# TargetResourceTypeTypeDef definition

class TargetResourceTypeTypeDef(TypedDict):
    resourceType: NotRequired[str],
    description: NotRequired[str],
    parameters: NotRequired[Dict[str, TargetResourceTypeParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: TargetResourceTypeParameterTypeDef](./type_defs.md#targetresourcetypeparametertypedef) 
## UpdateSafetyLeverStateRequestRequestTypeDef

```python
# UpdateSafetyLeverStateRequestRequestTypeDef definition

class UpdateSafetyLeverStateRequestRequestTypeDef(TypedDict):
    id: str,
    state: UpdateSafetyLeverStateInputTypeDef,  # (1)
```

1. See [:material-code-braces: UpdateSafetyLeverStateInputTypeDef](./type_defs.md#updatesafetyleverstateinputtypedef) 
## ListActionsResponseTypeDef

```python
# ListActionsResponseTypeDef definition

class ListActionsResponseTypeDef(TypedDict):
    actions: List[ActionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ActionSummaryTypeDef](./type_defs.md#actionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetActionResponseTypeDef

```python
# GetActionResponseTypeDef definition

class GetActionResponseTypeDef(TypedDict):
    action: ActionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExperimentSummaryTypeDef

```python
# ExperimentSummaryTypeDef definition

class ExperimentSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    experimentTemplateId: NotRequired[str],
    state: NotRequired[ExperimentStateTypeDef],  # (1)
    creationTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
    experimentOptions: NotRequired[ExperimentOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: ExperimentStateTypeDef](./type_defs.md#experimentstatetypedef) 
2. See [:material-code-braces: ExperimentOptionsTypeDef](./type_defs.md#experimentoptionstypedef) 
## ExperimentReportConfigurationTypeDef

```python
# ExperimentReportConfigurationTypeDef definition

class ExperimentReportConfigurationTypeDef(TypedDict):
    outputs: NotRequired[ExperimentReportConfigurationOutputsTypeDef],  # (1)
    dataSources: NotRequired[ExperimentReportConfigurationDataSourcesTypeDef],  # (2)
    preExperimentDuration: NotRequired[str],
    postExperimentDuration: NotRequired[str],
```

1. See [:material-code-braces: ExperimentReportConfigurationOutputsTypeDef](./type_defs.md#experimentreportconfigurationoutputstypedef) 
2. See [:material-code-braces: ExperimentReportConfigurationDataSourcesTypeDef](./type_defs.md#experimentreportconfigurationdatasourcestypedef) 
## ExperimentReportTypeDef

```python
# ExperimentReportTypeDef definition

class ExperimentReportTypeDef(TypedDict):
    state: NotRequired[ExperimentReportStateTypeDef],  # (1)
    s3Reports: NotRequired[List[ExperimentReportS3ReportTypeDef]],  # (2)
```

1. See [:material-code-braces: ExperimentReportStateTypeDef](./type_defs.md#experimentreportstatetypedef) 
2. See [:material-code-braces: ExperimentReportS3ReportTypeDef](./type_defs.md#experimentreports3reporttypedef) 
## CreateExperimentTemplateReportConfigurationInputTypeDef

```python
# CreateExperimentTemplateReportConfigurationInputTypeDef definition

class CreateExperimentTemplateReportConfigurationInputTypeDef(TypedDict):
    outputs: NotRequired[ExperimentTemplateReportConfigurationOutputsInputTypeDef],  # (1)
    dataSources: NotRequired[ExperimentTemplateReportConfigurationDataSourcesInputTypeDef],  # (2)
    preExperimentDuration: NotRequired[str],
    postExperimentDuration: NotRequired[str],
```

1. See [:material-code-braces: ExperimentTemplateReportConfigurationOutputsInputTypeDef](./type_defs.md#experimenttemplatereportconfigurationoutputsinputtypedef) 
2. See [:material-code-braces: ExperimentTemplateReportConfigurationDataSourcesInputTypeDef](./type_defs.md#experimenttemplatereportconfigurationdatasourcesinputtypedef) 
## UpdateExperimentTemplateReportConfigurationInputTypeDef

```python
# UpdateExperimentTemplateReportConfigurationInputTypeDef definition

class UpdateExperimentTemplateReportConfigurationInputTypeDef(TypedDict):
    outputs: NotRequired[ExperimentTemplateReportConfigurationOutputsInputTypeDef],  # (1)
    dataSources: NotRequired[ExperimentTemplateReportConfigurationDataSourcesInputTypeDef],  # (2)
    preExperimentDuration: NotRequired[str],
    postExperimentDuration: NotRequired[str],
```

1. See [:material-code-braces: ExperimentTemplateReportConfigurationOutputsInputTypeDef](./type_defs.md#experimenttemplatereportconfigurationoutputsinputtypedef) 
2. See [:material-code-braces: ExperimentTemplateReportConfigurationDataSourcesInputTypeDef](./type_defs.md#experimenttemplatereportconfigurationdatasourcesinputtypedef) 
## ExperimentTemplateReportConfigurationTypeDef

```python
# ExperimentTemplateReportConfigurationTypeDef definition

class ExperimentTemplateReportConfigurationTypeDef(TypedDict):
    outputs: NotRequired[ExperimentTemplateReportConfigurationOutputsTypeDef],  # (1)
    dataSources: NotRequired[ExperimentTemplateReportConfigurationDataSourcesTypeDef],  # (2)
    preExperimentDuration: NotRequired[str],
    postExperimentDuration: NotRequired[str],
```

1. See [:material-code-braces: ExperimentTemplateReportConfigurationOutputsTypeDef](./type_defs.md#experimenttemplatereportconfigurationoutputstypedef) 
2. See [:material-code-braces: ExperimentTemplateReportConfigurationDataSourcesTypeDef](./type_defs.md#experimenttemplatereportconfigurationdatasourcestypedef) 
## GetSafetyLeverResponseTypeDef

```python
# GetSafetyLeverResponseTypeDef definition

class GetSafetyLeverResponseTypeDef(TypedDict):
    safetyLever: SafetyLeverTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SafetyLeverTypeDef](./type_defs.md#safetylevertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSafetyLeverStateResponseTypeDef

```python
# UpdateSafetyLeverStateResponseTypeDef definition

class UpdateSafetyLeverStateResponseTypeDef(TypedDict):
    safetyLever: SafetyLeverTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SafetyLeverTypeDef](./type_defs.md#safetylevertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTargetResourceTypeResponseTypeDef

```python
# GetTargetResourceTypeResponseTypeDef definition

class GetTargetResourceTypeResponseTypeDef(TypedDict):
    targetResourceType: TargetResourceTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetResourceTypeTypeDef](./type_defs.md#targetresourcetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExperimentsResponseTypeDef

```python
# ListExperimentsResponseTypeDef definition

class ListExperimentsResponseTypeDef(TypedDict):
    experiments: List[ExperimentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExperimentSummaryTypeDef](./type_defs.md#experimentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExperimentTypeDef

```python
# ExperimentTypeDef definition

class ExperimentTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    experimentTemplateId: NotRequired[str],
    roleArn: NotRequired[str],
    state: NotRequired[ExperimentStateTypeDef],  # (1)
    targets: NotRequired[Dict[str, ExperimentTargetTypeDef]],  # (2)
    actions: NotRequired[Dict[str, ExperimentActionTypeDef]],  # (3)
    stopConditions: NotRequired[List[ExperimentStopConditionTypeDef]],  # (4)
    creationTime: NotRequired[datetime],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
    logConfiguration: NotRequired[ExperimentLogConfigurationTypeDef],  # (5)
    experimentOptions: NotRequired[ExperimentOptionsTypeDef],  # (6)
    targetAccountConfigurationsCount: NotRequired[int],
    experimentReportConfiguration: NotRequired[ExperimentReportConfigurationTypeDef],  # (7)
    experimentReport: NotRequired[ExperimentReportTypeDef],  # (8)
```

1. See [:material-code-braces: ExperimentStateTypeDef](./type_defs.md#experimentstatetypedef) 
2. See [:material-code-braces: ExperimentTargetTypeDef](./type_defs.md#experimenttargettypedef) 
3. See [:material-code-braces: ExperimentActionTypeDef](./type_defs.md#experimentactiontypedef) 
4. See [:material-code-braces: ExperimentStopConditionTypeDef](./type_defs.md#experimentstopconditiontypedef) 
5. See [:material-code-braces: ExperimentLogConfigurationTypeDef](./type_defs.md#experimentlogconfigurationtypedef) 
6. See [:material-code-braces: ExperimentOptionsTypeDef](./type_defs.md#experimentoptionstypedef) 
7. See [:material-code-braces: ExperimentReportConfigurationTypeDef](./type_defs.md#experimentreportconfigurationtypedef) 
8. See [:material-code-braces: ExperimentReportTypeDef](./type_defs.md#experimentreporttypedef) 
## CreateExperimentTemplateRequestRequestTypeDef

```python
# CreateExperimentTemplateRequestRequestTypeDef definition

class CreateExperimentTemplateRequestRequestTypeDef(TypedDict):
    clientToken: str,
    description: str,
    stopConditions: Sequence[CreateExperimentTemplateStopConditionInputTypeDef],  # (1)
    actions: Mapping[str, CreateExperimentTemplateActionInputTypeDef],  # (2)
    roleArn: str,
    targets: NotRequired[Mapping[str, CreateExperimentTemplateTargetInputTypeDef]],  # (3)
    tags: NotRequired[Mapping[str, str]],
    logConfiguration: NotRequired[CreateExperimentTemplateLogConfigurationInputTypeDef],  # (4)
    experimentOptions: NotRequired[CreateExperimentTemplateExperimentOptionsInputTypeDef],  # (5)
    experimentReportConfiguration: NotRequired[CreateExperimentTemplateReportConfigurationInputTypeDef],  # (6)
```

1. See [:material-code-braces: CreateExperimentTemplateStopConditionInputTypeDef](./type_defs.md#createexperimenttemplatestopconditioninputtypedef) 
2. See [:material-code-braces: CreateExperimentTemplateActionInputTypeDef](./type_defs.md#createexperimenttemplateactioninputtypedef) 
3. See [:material-code-braces: CreateExperimentTemplateTargetInputTypeDef](./type_defs.md#createexperimenttemplatetargetinputtypedef) 
4. See [:material-code-braces: CreateExperimentTemplateLogConfigurationInputTypeDef](./type_defs.md#createexperimenttemplatelogconfigurationinputtypedef) 
5. See [:material-code-braces: CreateExperimentTemplateExperimentOptionsInputTypeDef](./type_defs.md#createexperimenttemplateexperimentoptionsinputtypedef) 
6. See [:material-code-braces: CreateExperimentTemplateReportConfigurationInputTypeDef](./type_defs.md#createexperimenttemplatereportconfigurationinputtypedef) 
## UpdateExperimentTemplateRequestRequestTypeDef

```python
# UpdateExperimentTemplateRequestRequestTypeDef definition

class UpdateExperimentTemplateRequestRequestTypeDef(TypedDict):
    id: str,
    description: NotRequired[str],
    stopConditions: NotRequired[Sequence[UpdateExperimentTemplateStopConditionInputTypeDef]],  # (1)
    targets: NotRequired[Mapping[str, UpdateExperimentTemplateTargetInputTypeDef]],  # (2)
    actions: NotRequired[Mapping[str, UpdateExperimentTemplateActionInputItemTypeDef]],  # (3)
    roleArn: NotRequired[str],
    logConfiguration: NotRequired[UpdateExperimentTemplateLogConfigurationInputTypeDef],  # (4)
    experimentOptions: NotRequired[UpdateExperimentTemplateExperimentOptionsInputTypeDef],  # (5)
    experimentReportConfiguration: NotRequired[UpdateExperimentTemplateReportConfigurationInputTypeDef],  # (6)
```

1. See [:material-code-braces: UpdateExperimentTemplateStopConditionInputTypeDef](./type_defs.md#updateexperimenttemplatestopconditioninputtypedef) 
2. See [:material-code-braces: UpdateExperimentTemplateTargetInputTypeDef](./type_defs.md#updateexperimenttemplatetargetinputtypedef) 
3. See [:material-code-braces: UpdateExperimentTemplateActionInputItemTypeDef](./type_defs.md#updateexperimenttemplateactioninputitemtypedef) 
4. See [:material-code-braces: UpdateExperimentTemplateLogConfigurationInputTypeDef](./type_defs.md#updateexperimenttemplatelogconfigurationinputtypedef) 
5. See [:material-code-braces: UpdateExperimentTemplateExperimentOptionsInputTypeDef](./type_defs.md#updateexperimenttemplateexperimentoptionsinputtypedef) 
6. See [:material-code-braces: UpdateExperimentTemplateReportConfigurationInputTypeDef](./type_defs.md#updateexperimenttemplatereportconfigurationinputtypedef) 
## ExperimentTemplateTypeDef

```python
# ExperimentTemplateTypeDef definition

class ExperimentTemplateTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    description: NotRequired[str],
    targets: NotRequired[Dict[str, ExperimentTemplateTargetTypeDef]],  # (1)
    actions: NotRequired[Dict[str, ExperimentTemplateActionTypeDef]],  # (2)
    stopConditions: NotRequired[List[ExperimentTemplateStopConditionTypeDef]],  # (3)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    roleArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    logConfiguration: NotRequired[ExperimentTemplateLogConfigurationTypeDef],  # (4)
    experimentOptions: NotRequired[ExperimentTemplateExperimentOptionsTypeDef],  # (5)
    targetAccountConfigurationsCount: NotRequired[int],
    experimentReportConfiguration: NotRequired[ExperimentTemplateReportConfigurationTypeDef],  # (6)
```

1. See [:material-code-braces: ExperimentTemplateTargetTypeDef](./type_defs.md#experimenttemplatetargettypedef) 
2. See [:material-code-braces: ExperimentTemplateActionTypeDef](./type_defs.md#experimenttemplateactiontypedef) 
3. See [:material-code-braces: ExperimentTemplateStopConditionTypeDef](./type_defs.md#experimenttemplatestopconditiontypedef) 
4. See [:material-code-braces: ExperimentTemplateLogConfigurationTypeDef](./type_defs.md#experimenttemplatelogconfigurationtypedef) 
5. See [:material-code-braces: ExperimentTemplateExperimentOptionsTypeDef](./type_defs.md#experimenttemplateexperimentoptionstypedef) 
6. See [:material-code-braces: ExperimentTemplateReportConfigurationTypeDef](./type_defs.md#experimenttemplatereportconfigurationtypedef) 
## GetExperimentResponseTypeDef

```python
# GetExperimentResponseTypeDef definition

class GetExperimentResponseTypeDef(TypedDict):
    experiment: ExperimentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartExperimentResponseTypeDef

```python
# StartExperimentResponseTypeDef definition

class StartExperimentResponseTypeDef(TypedDict):
    experiment: ExperimentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopExperimentResponseTypeDef

```python
# StopExperimentResponseTypeDef definition

class StopExperimentResponseTypeDef(TypedDict):
    experiment: ExperimentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExperimentTemplateResponseTypeDef

```python
# CreateExperimentTemplateResponseTypeDef definition

class CreateExperimentTemplateResponseTypeDef(TypedDict):
    experimentTemplate: ExperimentTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTemplateTypeDef](./type_defs.md#experimenttemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteExperimentTemplateResponseTypeDef

```python
# DeleteExperimentTemplateResponseTypeDef definition

class DeleteExperimentTemplateResponseTypeDef(TypedDict):
    experimentTemplate: ExperimentTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTemplateTypeDef](./type_defs.md#experimenttemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExperimentTemplateResponseTypeDef

```python
# GetExperimentTemplateResponseTypeDef definition

class GetExperimentTemplateResponseTypeDef(TypedDict):
    experimentTemplate: ExperimentTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTemplateTypeDef](./type_defs.md#experimenttemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateExperimentTemplateResponseTypeDef

```python
# UpdateExperimentTemplateResponseTypeDef definition

class UpdateExperimentTemplateResponseTypeDef(TypedDict):
    experimentTemplate: ExperimentTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTemplateTypeDef](./type_defs.md#experimenttemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
