# Type definitions

> [Index](../README.md) > [MainframeModernizationApplicationTesting](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MainframeModernizationApplicationTesting](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest.html#mainframemodernizationapplicationtesting)
    type annotations stubs module [types-aiobotocore-apptest](https://pypi.org/project/types-aiobotocore-apptest/).

## BatchUnionTypeDef

```python
# BatchUnionTypeDef definition

BatchUnionTypeDef = Union[
    BatchTypeDef,  # (1)
    BatchOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BatchTypeDef](./type_defs.md#batchtypedef) 
2. See [:material-code-braces: BatchOutputTypeDef](./type_defs.md#batchoutputtypedef) 

## CloudFormationUnionTypeDef

```python
# CloudFormationUnionTypeDef definition

CloudFormationUnionTypeDef = Union[
    CloudFormationTypeDef,  # (1)
    CloudFormationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CloudFormationTypeDef](./type_defs.md#cloudformationtypedef) 
2. See [:material-code-braces: CloudFormationOutputTypeDef](./type_defs.md#cloudformationoutputtypedef) 

## TN3270UnionTypeDef

```python
# TN3270UnionTypeDef definition

TN3270UnionTypeDef = Union[
    TN3270TypeDef,  # (1)
    TN3270OutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TN3270TypeDef](./type_defs.md#tn3270typedef) 
2. See [:material-code-braces: TN3270OutputTypeDef](./type_defs.md#tn3270outputtypedef) 

## ResourceTypeUnionTypeDef

```python
# ResourceTypeUnionTypeDef definition

ResourceTypeUnionTypeDef = Union[
    ResourceTypeTypeDef,  # (1)
    ResourceTypeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResourceTypeTypeDef](./type_defs.md#resourcetypetypedef) 
2. See [:material-code-braces: ResourceTypeOutputTypeDef](./type_defs.md#resourcetypeoutputtypedef) 

## FileMetadataUnionTypeDef

```python
# FileMetadataUnionTypeDef definition

FileMetadataUnionTypeDef = Union[
    FileMetadataTypeDef,  # (1)
    FileMetadataOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FileMetadataTypeDef](./type_defs.md#filemetadatatypedef) 
2. See [:material-code-braces: FileMetadataOutputTypeDef](./type_defs.md#filemetadataoutputtypedef) 

## MainframeActionTypeUnionTypeDef

```python
# MainframeActionTypeUnionTypeDef definition

MainframeActionTypeUnionTypeDef = Union[
    MainframeActionTypeTypeDef,  # (1)
    MainframeActionTypeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MainframeActionTypeTypeDef](./type_defs.md#mainframeactiontypetypedef) 
2. See [:material-code-braces: MainframeActionTypeOutputTypeDef](./type_defs.md#mainframeactiontypeoutputtypedef) 

## ResourceUnionTypeDef

```python
# ResourceUnionTypeDef definition

ResourceUnionTypeDef = Union[
    ResourceTypeDef,  # (1)
    ResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 

## InputFileUnionTypeDef

```python
# InputFileUnionTypeDef definition

InputFileUnionTypeDef = Union[
    InputFileTypeDef,  # (1)
    InputFileOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InputFileTypeDef](./type_defs.md#inputfiletypedef) 
2. See [:material-code-braces: InputFileOutputTypeDef](./type_defs.md#inputfileoutputtypedef) 

## MainframeActionUnionTypeDef

```python
# MainframeActionUnionTypeDef definition

MainframeActionUnionTypeDef = Union[
    MainframeActionTypeDef,  # (1)
    MainframeActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MainframeActionTypeDef](./type_defs.md#mainframeactiontypedef) 
2. See [:material-code-braces: MainframeActionOutputTypeDef](./type_defs.md#mainframeactionoutputtypedef) 

## InputUnionTypeDef

```python
# InputUnionTypeDef definition

InputUnionTypeDef = Union[
    InputTypeDef,  # (1)
    InputOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
2. See [:material-code-braces: InputOutputTypeDef](./type_defs.md#inputoutputtypedef) 

## CompareActionUnionTypeDef

```python
# CompareActionUnionTypeDef definition

CompareActionUnionTypeDef = Union[
    CompareActionTypeDef,  # (1)
    CompareActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CompareActionTypeDef](./type_defs.md#compareactiontypedef) 
2. See [:material-code-braces: CompareActionOutputTypeDef](./type_defs.md#compareactionoutputtypedef) 

## StepActionUnionTypeDef

```python
# StepActionUnionTypeDef definition

StepActionUnionTypeDef = Union[
    StepActionTypeDef,  # (1)
    StepActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StepActionTypeDef](./type_defs.md#stepactiontypedef) 
2. See [:material-code-braces: StepActionOutputTypeDef](./type_defs.md#stepactionoutputtypedef) 

## StepUnionTypeDef

```python
# StepUnionTypeDef definition

StepUnionTypeDef = Union[
    StepTypeDef,  # (1)
    StepOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
2. See [:material-code-braces: StepOutputTypeDef](./type_defs.md#stepoutputtypedef) 



## BatchOutputTypeDef

```python
# BatchOutputTypeDef definition

class BatchOutputTypeDef(TypedDict):
    batchJobName: str,
    batchJobParameters: NotRequired[Dict[str, str]],
    exportDataSetNames: NotRequired[List[str]],
```

## MainframeActionPropertiesTypeDef

```python
# MainframeActionPropertiesTypeDef definition

class MainframeActionPropertiesTypeDef(TypedDict):
    dmsTaskArn: NotRequired[str],
```

## DataSetTypeDef

```python
# DataSetTypeDef definition

class DataSetTypeDef(TypedDict):
    type: DataSetTypeType,  # (1)
    name: str,
    ccsid: str,
    format: FormatType,  # (2)
    length: int,
```

1. See [:material-code-brackets: DataSetTypeType](./literals.md#datasettypetype) 
2. See [:material-code-brackets: FormatType](./literals.md#formattype) 
## BatchTypeDef

```python
# BatchTypeDef definition

class BatchTypeDef(TypedDict):
    batchJobName: str,
    batchJobParameters: NotRequired[Mapping[str, str]],
    exportDataSetNames: NotRequired[Sequence[str]],
```

## CloudFormationActionTypeDef

```python
# CloudFormationActionTypeDef definition

class CloudFormationActionTypeDef(TypedDict):
    resource: str,
    actionType: NotRequired[CloudFormationActionTypeType],  # (1)
```

1. See [:material-code-brackets: CloudFormationActionTypeType](./literals.md#cloudformationactiontypetype) 
## CloudFormationOutputTypeDef

```python
# CloudFormationOutputTypeDef definition

class CloudFormationOutputTypeDef(TypedDict):
    templateLocation: str,
    parameters: NotRequired[Dict[str, str]],
```

## CloudFormationTypeDef

```python
# CloudFormationTypeDef definition

class CloudFormationTypeDef(TypedDict):
    templateLocation: str,
    parameters: NotRequired[Mapping[str, str]],
```

## CompareDataSetsStepOutputTypeDef

```python
# CompareDataSetsStepOutputTypeDef definition

class CompareDataSetsStepOutputTypeDef(TypedDict):
    comparisonOutputLocation: str,
    comparisonStatus: ComparisonStatusEnumType,  # (1)
```

1. See [:material-code-brackets: ComparisonStatusEnumType](./literals.md#comparisonstatusenumtype) 
## SourceDatabaseMetadataTypeDef

```python
# SourceDatabaseMetadataTypeDef definition

class SourceDatabaseMetadataTypeDef(TypedDict):
    type: SourceDatabaseType,  # (1)
    captureTool: CaptureToolType,  # (2)
```

1. See [:material-code-brackets: SourceDatabaseType](./literals.md#sourcedatabasetype) 
2. See [:material-code-brackets: CaptureToolType](./literals.md#capturetooltype) 
## TargetDatabaseMetadataTypeDef

```python
# TargetDatabaseMetadataTypeDef definition

class TargetDatabaseMetadataTypeDef(TypedDict):
    type: TargetDatabaseType,  # (1)
    captureTool: CaptureToolType,  # (2)
```

1. See [:material-code-brackets: TargetDatabaseType](./literals.md#targetdatabasetype) 
2. See [:material-code-brackets: CaptureToolType](./literals.md#capturetooltype) 
## CompareDatabaseCDCStepOutputTypeDef

```python
# CompareDatabaseCDCStepOutputTypeDef definition

class CompareDatabaseCDCStepOutputTypeDef(TypedDict):
    comparisonOutputLocation: str,
    comparisonStatus: ComparisonStatusEnumType,  # (1)
```

1. See [:material-code-brackets: ComparisonStatusEnumType](./literals.md#comparisonstatusenumtype) 
## CreateCloudFormationStepInputTypeDef

```python
# CreateCloudFormationStepInputTypeDef definition

class CreateCloudFormationStepInputTypeDef(TypedDict):
    templateLocation: str,
    parameters: NotRequired[Dict[str, str]],
```

## CreateCloudFormationStepOutputTypeDef

```python
# CreateCloudFormationStepOutputTypeDef definition

class CreateCloudFormationStepOutputTypeDef(TypedDict):
    stackId: str,
    exports: NotRequired[Dict[str, str]],
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

## ServiceSettingsTypeDef

```python
# ServiceSettingsTypeDef definition

class ServiceSettingsTypeDef(TypedDict):
    kmsKeyId: NotRequired[str],
```

## TestCasesTypeDef

```python
# TestCasesTypeDef definition

class TestCasesTypeDef(TypedDict):
    sequential: NotRequired[Sequence[str]],
```

## DeleteCloudFormationStepInputTypeDef

```python
# DeleteCloudFormationStepInputTypeDef definition

class DeleteCloudFormationStepInputTypeDef(TypedDict):
    stackId: str,
```

## DeleteTestCaseRequestRequestTypeDef

```python
# DeleteTestCaseRequestRequestTypeDef definition

class DeleteTestCaseRequestRequestTypeDef(TypedDict):
    testCaseId: str,
```

## DeleteTestConfigurationRequestRequestTypeDef

```python
# DeleteTestConfigurationRequestRequestTypeDef definition

class DeleteTestConfigurationRequestRequestTypeDef(TypedDict):
    testConfigurationId: str,
```

## DeleteTestRunRequestRequestTypeDef

```python
# DeleteTestRunRequestRequestTypeDef definition

class DeleteTestRunRequestRequestTypeDef(TypedDict):
    testRunId: str,
```

## DeleteTestSuiteRequestRequestTypeDef

```python
# DeleteTestSuiteRequestRequestTypeDef definition

class DeleteTestSuiteRequestRequestTypeDef(TypedDict):
    testSuiteId: str,
```

## GetTestCaseRequestRequestTypeDef

```python
# GetTestCaseRequestRequestTypeDef definition

class GetTestCaseRequestRequestTypeDef(TypedDict):
    testCaseId: str,
    testCaseVersion: NotRequired[int],
```

## TestCaseLatestVersionTypeDef

```python
# TestCaseLatestVersionTypeDef definition

class TestCaseLatestVersionTypeDef(TypedDict):
    version: int,
    status: TestCaseLifecycleType,  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: TestCaseLifecycleType](./literals.md#testcaselifecycletype) 
## GetTestConfigurationRequestRequestTypeDef

```python
# GetTestConfigurationRequestRequestTypeDef definition

class GetTestConfigurationRequestRequestTypeDef(TypedDict):
    testConfigurationId: str,
    testConfigurationVersion: NotRequired[int],
```

## TestConfigurationLatestVersionTypeDef

```python
# TestConfigurationLatestVersionTypeDef definition

class TestConfigurationLatestVersionTypeDef(TypedDict):
    version: int,
    status: TestConfigurationLifecycleType,  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: TestConfigurationLifecycleType](./literals.md#testconfigurationlifecycletype) 
## GetTestRunStepRequestRequestTypeDef

```python
# GetTestRunStepRequestRequestTypeDef definition

class GetTestRunStepRequestRequestTypeDef(TypedDict):
    testRunId: str,
    stepName: str,
    testCaseId: NotRequired[str],
    testSuiteId: NotRequired[str],
```

## GetTestSuiteRequestRequestTypeDef

```python
# GetTestSuiteRequestRequestTypeDef definition

class GetTestSuiteRequestRequestTypeDef(TypedDict):
    testSuiteId: str,
    testSuiteVersion: NotRequired[int],
```

## TestCasesOutputTypeDef

```python
# TestCasesOutputTypeDef definition

class TestCasesOutputTypeDef(TypedDict):
    sequential: NotRequired[List[str]],
```

## TestSuiteLatestVersionTypeDef

```python
# TestSuiteLatestVersionTypeDef definition

class TestSuiteLatestVersionTypeDef(TypedDict):
    version: int,
    status: TestSuiteLifecycleType,  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: TestSuiteLifecycleType](./literals.md#testsuitelifecycletype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListTestCasesRequestRequestTypeDef

```python
# ListTestCasesRequestRequestTypeDef definition

class ListTestCasesRequestRequestTypeDef(TypedDict):
    testCaseIds: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TestCaseSummaryTypeDef

```python
# TestCaseSummaryTypeDef definition

class TestCaseSummaryTypeDef(TypedDict):
    testCaseId: str,
    testCaseArn: str,
    name: str,
    latestVersion: int,
    status: TestCaseLifecycleType,  # (1)
    creationTime: datetime,
    lastUpdateTime: datetime,
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: TestCaseLifecycleType](./literals.md#testcaselifecycletype) 
## ListTestConfigurationsRequestRequestTypeDef

```python
# ListTestConfigurationsRequestRequestTypeDef definition

class ListTestConfigurationsRequestRequestTypeDef(TypedDict):
    testConfigurationIds: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TestConfigurationSummaryTypeDef

```python
# TestConfigurationSummaryTypeDef definition

class TestConfigurationSummaryTypeDef(TypedDict):
    testConfigurationId: str,
    name: str,
    latestVersion: int,
    testConfigurationArn: str,
    status: TestConfigurationLifecycleType,  # (1)
    creationTime: datetime,
    lastUpdateTime: datetime,
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: TestConfigurationLifecycleType](./literals.md#testconfigurationlifecycletype) 
## ListTestRunStepsRequestRequestTypeDef

```python
# ListTestRunStepsRequestRequestTypeDef definition

class ListTestRunStepsRequestRequestTypeDef(TypedDict):
    testRunId: str,
    testCaseId: NotRequired[str],
    testSuiteId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TestRunStepSummaryTypeDef

```python
# TestRunStepSummaryTypeDef definition

class TestRunStepSummaryTypeDef(TypedDict):
    stepName: str,
    testRunId: str,
    status: StepRunStatusType,  # (1)
    runStartTime: datetime,
    testCaseId: NotRequired[str],
    testCaseVersion: NotRequired[int],
    testSuiteId: NotRequired[str],
    testSuiteVersion: NotRequired[int],
    beforeStep: NotRequired[bool],
    afterStep: NotRequired[bool],
    statusReason: NotRequired[str],
    runEndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: StepRunStatusType](./literals.md#steprunstatustype) 
## ListTestRunTestCasesRequestRequestTypeDef

```python
# ListTestRunTestCasesRequestRequestTypeDef definition

class ListTestRunTestCasesRequestRequestTypeDef(TypedDict):
    testRunId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TestCaseRunSummaryTypeDef

```python
# TestCaseRunSummaryTypeDef definition

class TestCaseRunSummaryTypeDef(TypedDict):
    testCaseId: str,
    testCaseVersion: int,
    testRunId: str,
    status: TestCaseRunStatusType,  # (1)
    runStartTime: datetime,
    statusReason: NotRequired[str],
    runEndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: TestCaseRunStatusType](./literals.md#testcaserunstatustype) 
## ListTestRunsRequestRequestTypeDef

```python
# ListTestRunsRequestRequestTypeDef definition

class ListTestRunsRequestRequestTypeDef(TypedDict):
    testSuiteId: NotRequired[str],
    testRunIds: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TestRunSummaryTypeDef

```python
# TestRunSummaryTypeDef definition

class TestRunSummaryTypeDef(TypedDict):
    testRunId: str,
    testRunArn: str,
    testSuiteId: str,
    testSuiteVersion: int,
    status: TestRunStatusType,  # (1)
    runStartTime: datetime,
    testConfigurationId: NotRequired[str],
    testConfigurationVersion: NotRequired[int],
    statusReason: NotRequired[str],
    runEndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: TestRunStatusType](./literals.md#testrunstatustype) 
## ListTestSuitesRequestRequestTypeDef

```python
# ListTestSuitesRequestRequestTypeDef definition

class ListTestSuitesRequestRequestTypeDef(TypedDict):
    testSuiteIds: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TestSuiteSummaryTypeDef

```python
# TestSuiteSummaryTypeDef definition

class TestSuiteSummaryTypeDef(TypedDict):
    testSuiteId: str,
    name: str,
    latestVersion: int,
    testSuiteArn: str,
    status: TestSuiteLifecycleType,  # (1)
    creationTime: datetime,
    lastUpdateTime: datetime,
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: TestSuiteLifecycleType](./literals.md#testsuitelifecycletype) 
## M2ManagedActionPropertiesTypeDef

```python
# M2ManagedActionPropertiesTypeDef definition

class M2ManagedActionPropertiesTypeDef(TypedDict):
    forceStop: NotRequired[bool],
    importDataSetLocation: NotRequired[str],
```

## M2ManagedApplicationStepOutputTypeDef

```python
# M2ManagedApplicationStepOutputTypeDef definition

class M2ManagedApplicationStepOutputTypeDef(TypedDict):
    importDataSetSummary: NotRequired[Dict[str, str]],
```

## M2ManagedApplicationSummaryTypeDef

```python
# M2ManagedApplicationSummaryTypeDef definition

class M2ManagedApplicationSummaryTypeDef(TypedDict):
    applicationId: str,
    runtime: M2ManagedRuntimeType,  # (1)
    listenerPort: NotRequired[int],
```

1. See [:material-code-brackets: M2ManagedRuntimeType](./literals.md#m2managedruntimetype) 
## M2ManagedApplicationTypeDef

```python
# M2ManagedApplicationTypeDef definition

class M2ManagedApplicationTypeDef(TypedDict):
    applicationId: str,
    runtime: M2ManagedRuntimeType,  # (1)
    vpcEndpointServiceName: NotRequired[str],
    listenerPort: NotRequired[str],
```

1. See [:material-code-brackets: M2ManagedRuntimeType](./literals.md#m2managedruntimetype) 
## M2NonManagedApplicationActionTypeDef

```python
# M2NonManagedApplicationActionTypeDef definition

class M2NonManagedApplicationActionTypeDef(TypedDict):
    resource: str,
    actionType: M2NonManagedActionTypeType,  # (1)
```

1. See [:material-code-brackets: M2NonManagedActionTypeType](./literals.md#m2nonmanagedactiontypetype) 
## M2NonManagedApplicationStepInputTypeDef

```python
# M2NonManagedApplicationStepInputTypeDef definition

class M2NonManagedApplicationStepInputTypeDef(TypedDict):
    vpcEndpointServiceName: str,
    listenerPort: int,
    runtime: M2NonManagedRuntimeType,  # (1)
    actionType: M2NonManagedActionTypeType,  # (2)
    webAppName: NotRequired[str],
```

1. See [:material-code-brackets: M2NonManagedRuntimeType](./literals.md#m2nonmanagedruntimetype) 
2. See [:material-code-brackets: M2NonManagedActionTypeType](./literals.md#m2nonmanagedactiontypetype) 
## M2NonManagedApplicationSummaryTypeDef

```python
# M2NonManagedApplicationSummaryTypeDef definition

class M2NonManagedApplicationSummaryTypeDef(TypedDict):
    vpcEndpointServiceName: str,
    listenerPort: int,
    runtime: M2NonManagedRuntimeType,  # (1)
    webAppName: NotRequired[str],
```

1. See [:material-code-brackets: M2NonManagedRuntimeType](./literals.md#m2nonmanagedruntimetype) 
## M2NonManagedApplicationTypeDef

```python
# M2NonManagedApplicationTypeDef definition

class M2NonManagedApplicationTypeDef(TypedDict):
    vpcEndpointServiceName: str,
    listenerPort: str,
    runtime: M2NonManagedRuntimeType,  # (1)
    webAppName: NotRequired[str],
```

1. See [:material-code-brackets: M2NonManagedRuntimeType](./literals.md#m2nonmanagedruntimetype) 
## OutputFileTypeDef

```python
# OutputFileTypeDef definition

class OutputFileTypeDef(TypedDict):
    fileLocation: NotRequired[str],
```

## ScriptSummaryTypeDef

```python
# ScriptSummaryTypeDef definition

class ScriptSummaryTypeDef(TypedDict):
    scriptLocation: str,
    type: ScriptTypeType,  # (1)
```

1. See [:material-code-brackets: ScriptTypeType](./literals.md#scripttypetype) 
## ScriptTypeDef

```python
# ScriptTypeDef definition

class ScriptTypeDef(TypedDict):
    scriptLocation: str,
    type: ScriptTypeType,  # (1)
```

1. See [:material-code-brackets: ScriptTypeType](./literals.md#scripttypetype) 
## StartTestRunRequestRequestTypeDef

```python
# StartTestRunRequestRequestTypeDef definition

class StartTestRunRequestRequestTypeDef(TypedDict):
    testSuiteId: str,
    testConfigurationId: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## BatchStepOutputTypeDef

```python
# BatchStepOutputTypeDef definition

class BatchStepOutputTypeDef(TypedDict):
    dataSetExportLocation: NotRequired[str],
    dmsOutputLocation: NotRequired[str],
    dataSetDetails: NotRequired[List[DataSetTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSetTypeDef](./type_defs.md#datasettypedef) 
## CompareDataSetsStepInputTypeDef

```python
# CompareDataSetsStepInputTypeDef definition

class CompareDataSetsStepInputTypeDef(TypedDict):
    sourceLocation: str,
    targetLocation: str,
    sourceDataSets: List[DataSetTypeDef],  # (1)
    targetDataSets: List[DataSetTypeDef],  # (1)
```

1. See [:material-code-braces: DataSetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: DataSetTypeDef](./type_defs.md#datasettypedef) 
## TN3270StepOutputTypeDef

```python
# TN3270StepOutputTypeDef definition

class TN3270StepOutputTypeDef(TypedDict):
    scriptOutputLocation: str,
    dataSetExportLocation: NotRequired[str],
    dmsOutputLocation: NotRequired[str],
    dataSetDetails: NotRequired[List[DataSetTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSetTypeDef](./type_defs.md#datasettypedef) 
## CompareDatabaseCDCStepInputTypeDef

```python
# CompareDatabaseCDCStepInputTypeDef definition

class CompareDatabaseCDCStepInputTypeDef(TypedDict):
    sourceLocation: str,
    targetLocation: str,
    sourceMetadata: SourceDatabaseMetadataTypeDef,  # (1)
    targetMetadata: TargetDatabaseMetadataTypeDef,  # (2)
    outputLocation: NotRequired[str],
```

1. See [:material-code-braces: SourceDatabaseMetadataTypeDef](./type_defs.md#sourcedatabasemetadatatypedef) 
2. See [:material-code-braces: TargetDatabaseMetadataTypeDef](./type_defs.md#targetdatabasemetadatatypedef) 
## DatabaseCDCTypeDef

```python
# DatabaseCDCTypeDef definition

class DatabaseCDCTypeDef(TypedDict):
    sourceMetadata: SourceDatabaseMetadataTypeDef,  # (1)
    targetMetadata: TargetDatabaseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceDatabaseMetadataTypeDef](./type_defs.md#sourcedatabasemetadatatypedef) 
2. See [:material-code-braces: TargetDatabaseMetadataTypeDef](./type_defs.md#targetdatabasemetadatatypedef) 
## CreateCloudFormationSummaryTypeDef

```python
# CreateCloudFormationSummaryTypeDef definition

class CreateCloudFormationSummaryTypeDef(TypedDict):
    stepInput: CreateCloudFormationStepInputTypeDef,  # (1)
    stepOutput: NotRequired[CreateCloudFormationStepOutputTypeDef],  # (2)
```

1. See [:material-code-braces: CreateCloudFormationStepInputTypeDef](./type_defs.md#createcloudformationstepinputtypedef) 
2. See [:material-code-braces: CreateCloudFormationStepOutputTypeDef](./type_defs.md#createcloudformationstepoutputtypedef) 
## CreateTestCaseResponseTypeDef

```python
# CreateTestCaseResponseTypeDef definition

class CreateTestCaseResponseTypeDef(TypedDict):
    testCaseId: str,
    testCaseVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTestConfigurationResponseTypeDef

```python
# CreateTestConfigurationResponseTypeDef definition

class CreateTestConfigurationResponseTypeDef(TypedDict):
    testConfigurationId: str,
    testConfigurationVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTestSuiteResponseTypeDef

```python
# CreateTestSuiteResponseTypeDef definition

class CreateTestSuiteResponseTypeDef(TypedDict):
    testSuiteId: str,
    testSuiteVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTestRunResponseTypeDef

```python
# StartTestRunResponseTypeDef definition

class StartTestRunResponseTypeDef(TypedDict):
    testRunId: str,
    testRunStatus: TestRunStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TestRunStatusType](./literals.md#testrunstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTestCaseResponseTypeDef

```python
# UpdateTestCaseResponseTypeDef definition

class UpdateTestCaseResponseTypeDef(TypedDict):
    testCaseId: str,
    testCaseVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTestConfigurationResponseTypeDef

```python
# UpdateTestConfigurationResponseTypeDef definition

class UpdateTestConfigurationResponseTypeDef(TypedDict):
    testConfigurationId: str,
    testConfigurationVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTestSuiteResponseTypeDef

```python
# UpdateTestSuiteResponseTypeDef definition

class UpdateTestSuiteResponseTypeDef(TypedDict):
    testSuiteId: str,
    testSuiteVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCloudFormationSummaryTypeDef

```python
# DeleteCloudFormationSummaryTypeDef definition

class DeleteCloudFormationSummaryTypeDef(TypedDict):
    stepInput: DeleteCloudFormationStepInputTypeDef,  # (1)
    stepOutput: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: DeleteCloudFormationStepInputTypeDef](./type_defs.md#deletecloudformationstepinputtypedef) 
## ListTestCasesRequestPaginateTypeDef

```python
# ListTestCasesRequestPaginateTypeDef definition

class ListTestCasesRequestPaginateTypeDef(TypedDict):
    testCaseIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTestConfigurationsRequestPaginateTypeDef

```python
# ListTestConfigurationsRequestPaginateTypeDef definition

class ListTestConfigurationsRequestPaginateTypeDef(TypedDict):
    testConfigurationIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTestRunStepsRequestPaginateTypeDef

```python
# ListTestRunStepsRequestPaginateTypeDef definition

class ListTestRunStepsRequestPaginateTypeDef(TypedDict):
    testRunId: str,
    testCaseId: NotRequired[str],
    testSuiteId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTestRunTestCasesRequestPaginateTypeDef

```python
# ListTestRunTestCasesRequestPaginateTypeDef definition

class ListTestRunTestCasesRequestPaginateTypeDef(TypedDict):
    testRunId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTestRunsRequestPaginateTypeDef

```python
# ListTestRunsRequestPaginateTypeDef definition

class ListTestRunsRequestPaginateTypeDef(TypedDict):
    testSuiteId: NotRequired[str],
    testRunIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTestSuitesRequestPaginateTypeDef

```python
# ListTestSuitesRequestPaginateTypeDef definition

class ListTestSuitesRequestPaginateTypeDef(TypedDict):
    testSuiteIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTestCasesResponseTypeDef

```python
# ListTestCasesResponseTypeDef definition

class ListTestCasesResponseTypeDef(TypedDict):
    testCases: List[TestCaseSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestCaseSummaryTypeDef](./type_defs.md#testcasesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTestConfigurationsResponseTypeDef

```python
# ListTestConfigurationsResponseTypeDef definition

class ListTestConfigurationsResponseTypeDef(TypedDict):
    testConfigurations: List[TestConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestConfigurationSummaryTypeDef](./type_defs.md#testconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTestRunStepsResponseTypeDef

```python
# ListTestRunStepsResponseTypeDef definition

class ListTestRunStepsResponseTypeDef(TypedDict):
    testRunSteps: List[TestRunStepSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestRunStepSummaryTypeDef](./type_defs.md#testrunstepsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTestRunTestCasesResponseTypeDef

```python
# ListTestRunTestCasesResponseTypeDef definition

class ListTestRunTestCasesResponseTypeDef(TypedDict):
    testRunTestCases: List[TestCaseRunSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestCaseRunSummaryTypeDef](./type_defs.md#testcaserunsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTestRunsResponseTypeDef

```python
# ListTestRunsResponseTypeDef definition

class ListTestRunsResponseTypeDef(TypedDict):
    testRuns: List[TestRunSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestRunSummaryTypeDef](./type_defs.md#testrunsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTestSuitesResponseTypeDef

```python
# ListTestSuitesResponseTypeDef definition

class ListTestSuitesResponseTypeDef(TypedDict):
    testSuites: List[TestSuiteSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestSuiteSummaryTypeDef](./type_defs.md#testsuitesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## M2ManagedApplicationActionTypeDef

```python
# M2ManagedApplicationActionTypeDef definition

class M2ManagedApplicationActionTypeDef(TypedDict):
    resource: str,
    actionType: M2ManagedActionTypeType,  # (1)
    properties: NotRequired[M2ManagedActionPropertiesTypeDef],  # (2)
```

1. See [:material-code-brackets: M2ManagedActionTypeType](./literals.md#m2managedactiontypetype) 
2. See [:material-code-braces: M2ManagedActionPropertiesTypeDef](./type_defs.md#m2managedactionpropertiestypedef) 
## M2ManagedApplicationStepInputTypeDef

```python
# M2ManagedApplicationStepInputTypeDef definition

class M2ManagedApplicationStepInputTypeDef(TypedDict):
    applicationId: str,
    runtime: str,
    actionType: M2ManagedActionTypeType,  # (1)
    vpcEndpointServiceName: NotRequired[str],
    listenerPort: NotRequired[int],
    properties: NotRequired[M2ManagedActionPropertiesTypeDef],  # (2)
```

1. See [:material-code-brackets: M2ManagedActionTypeType](./literals.md#m2managedactiontypetype) 
2. See [:material-code-braces: M2ManagedActionPropertiesTypeDef](./type_defs.md#m2managedactionpropertiestypedef) 
## M2NonManagedApplicationStepSummaryTypeDef

```python
# M2NonManagedApplicationStepSummaryTypeDef definition

class M2NonManagedApplicationStepSummaryTypeDef(TypedDict):
    stepInput: M2NonManagedApplicationStepInputTypeDef,  # (1)
    stepOutput: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: M2NonManagedApplicationStepInputTypeDef](./type_defs.md#m2nonmanagedapplicationstepinputtypedef) 
## MainframeResourceSummaryTypeDef

```python
# MainframeResourceSummaryTypeDef definition

class MainframeResourceSummaryTypeDef(TypedDict):
    m2ManagedApplication: NotRequired[M2ManagedApplicationSummaryTypeDef],  # (1)
    m2NonManagedApplication: NotRequired[M2NonManagedApplicationSummaryTypeDef],  # (2)
```

1. See [:material-code-braces: M2ManagedApplicationSummaryTypeDef](./type_defs.md#m2managedapplicationsummarytypedef) 
2. See [:material-code-braces: M2NonManagedApplicationSummaryTypeDef](./type_defs.md#m2nonmanagedapplicationsummarytypedef) 
## ResourceTypeOutputTypeDef

```python
# ResourceTypeOutputTypeDef definition

class ResourceTypeOutputTypeDef(TypedDict):
    cloudFormation: NotRequired[CloudFormationOutputTypeDef],  # (1)
    m2ManagedApplication: NotRequired[M2ManagedApplicationTypeDef],  # (2)
    m2NonManagedApplication: NotRequired[M2NonManagedApplicationTypeDef],  # (3)
```

1. See [:material-code-braces: CloudFormationOutputTypeDef](./type_defs.md#cloudformationoutputtypedef) 
2. See [:material-code-braces: M2ManagedApplicationTypeDef](./type_defs.md#m2managedapplicationtypedef) 
3. See [:material-code-braces: M2NonManagedApplicationTypeDef](./type_defs.md#m2nonmanagedapplicationtypedef) 
## OutputTypeDef

```python
# OutputTypeDef definition

class OutputTypeDef(TypedDict):
    file: NotRequired[OutputFileTypeDef],  # (1)
```

1. See [:material-code-braces: OutputFileTypeDef](./type_defs.md#outputfiletypedef) 
## TN3270OutputTypeDef

```python
# TN3270OutputTypeDef definition

class TN3270OutputTypeDef(TypedDict):
    script: ScriptTypeDef,  # (1)
    exportDataSetNames: NotRequired[List[str]],
```

1. See [:material-code-braces: ScriptTypeDef](./type_defs.md#scripttypedef) 
## TN3270TypeDef

```python
# TN3270TypeDef definition

class TN3270TypeDef(TypedDict):
    script: ScriptTypeDef,  # (1)
    exportDataSetNames: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ScriptTypeDef](./type_defs.md#scripttypedef) 
## CompareDataSetsSummaryTypeDef

```python
# CompareDataSetsSummaryTypeDef definition

class CompareDataSetsSummaryTypeDef(TypedDict):
    stepInput: CompareDataSetsStepInputTypeDef,  # (1)
    stepOutput: NotRequired[CompareDataSetsStepOutputTypeDef],  # (2)
```

1. See [:material-code-braces: CompareDataSetsStepInputTypeDef](./type_defs.md#comparedatasetsstepinputtypedef) 
2. See [:material-code-braces: CompareDataSetsStepOutputTypeDef](./type_defs.md#comparedatasetsstepoutputtypedef) 
## ResourceTypeTypeDef

```python
# ResourceTypeTypeDef definition

class ResourceTypeTypeDef(TypedDict):
    cloudFormation: NotRequired[CloudFormationUnionTypeDef],  # (1)
    m2ManagedApplication: NotRequired[M2ManagedApplicationTypeDef],  # (2)
    m2NonManagedApplication: NotRequired[M2NonManagedApplicationTypeDef],  # (3)
```

1. See [:material-code-braces: CloudFormationTypeDef](./type_defs.md#cloudformationtypedef) [:material-code-braces: CloudFormationOutputTypeDef](./type_defs.md#cloudformationoutputtypedef) 
2. See [:material-code-braces: M2ManagedApplicationTypeDef](./type_defs.md#m2managedapplicationtypedef) 
3. See [:material-code-braces: M2NonManagedApplicationTypeDef](./type_defs.md#m2nonmanagedapplicationtypedef) 
## CompareDatabaseCDCSummaryTypeDef

```python
# CompareDatabaseCDCSummaryTypeDef definition

class CompareDatabaseCDCSummaryTypeDef(TypedDict):
    stepInput: CompareDatabaseCDCStepInputTypeDef,  # (1)
    stepOutput: NotRequired[CompareDatabaseCDCStepOutputTypeDef],  # (2)
```

1. See [:material-code-braces: CompareDatabaseCDCStepInputTypeDef](./type_defs.md#comparedatabasecdcstepinputtypedef) 
2. See [:material-code-braces: CompareDatabaseCDCStepOutputTypeDef](./type_defs.md#comparedatabasecdcstepoutputtypedef) 
## FileMetadataOutputTypeDef

```python
# FileMetadataOutputTypeDef definition

class FileMetadataOutputTypeDef(TypedDict):
    dataSets: NotRequired[List[DataSetTypeDef]],  # (1)
    databaseCDC: NotRequired[DatabaseCDCTypeDef],  # (2)
```

1. See [:material-code-braces: DataSetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: DatabaseCDCTypeDef](./type_defs.md#databasecdctypedef) 
## FileMetadataTypeDef

```python
# FileMetadataTypeDef definition

class FileMetadataTypeDef(TypedDict):
    dataSets: NotRequired[Sequence[DataSetTypeDef]],  # (1)
    databaseCDC: NotRequired[DatabaseCDCTypeDef],  # (2)
```

1. See [:material-code-braces: DataSetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: DatabaseCDCTypeDef](./type_defs.md#databasecdctypedef) 
## CloudFormationStepSummaryTypeDef

```python
# CloudFormationStepSummaryTypeDef definition

class CloudFormationStepSummaryTypeDef(TypedDict):
    createCloudformation: NotRequired[CreateCloudFormationSummaryTypeDef],  # (1)
    deleteCloudformation: NotRequired[DeleteCloudFormationSummaryTypeDef],  # (2)
```

1. See [:material-code-braces: CreateCloudFormationSummaryTypeDef](./type_defs.md#createcloudformationsummarytypedef) 
2. See [:material-code-braces: DeleteCloudFormationSummaryTypeDef](./type_defs.md#deletecloudformationsummarytypedef) 
## ResourceActionTypeDef

```python
# ResourceActionTypeDef definition

class ResourceActionTypeDef(TypedDict):
    m2ManagedApplicationAction: NotRequired[M2ManagedApplicationActionTypeDef],  # (1)
    m2NonManagedApplicationAction: NotRequired[M2NonManagedApplicationActionTypeDef],  # (2)
    cloudFormationAction: NotRequired[CloudFormationActionTypeDef],  # (3)
```

1. See [:material-code-braces: M2ManagedApplicationActionTypeDef](./type_defs.md#m2managedapplicationactiontypedef) 
2. See [:material-code-braces: M2NonManagedApplicationActionTypeDef](./type_defs.md#m2nonmanagedapplicationactiontypedef) 
3. See [:material-code-braces: CloudFormationActionTypeDef](./type_defs.md#cloudformationactiontypedef) 
## M2ManagedApplicationStepSummaryTypeDef

```python
# M2ManagedApplicationStepSummaryTypeDef definition

class M2ManagedApplicationStepSummaryTypeDef(TypedDict):
    stepInput: M2ManagedApplicationStepInputTypeDef,  # (1)
    stepOutput: NotRequired[M2ManagedApplicationStepOutputTypeDef],  # (2)
```

1. See [:material-code-braces: M2ManagedApplicationStepInputTypeDef](./type_defs.md#m2managedapplicationstepinputtypedef) 
2. See [:material-code-braces: M2ManagedApplicationStepOutputTypeDef](./type_defs.md#m2managedapplicationstepoutputtypedef) 
## BatchStepInputTypeDef

```python
# BatchStepInputTypeDef definition

class BatchStepInputTypeDef(TypedDict):
    resource: MainframeResourceSummaryTypeDef,  # (1)
    batchJobName: str,
    batchJobParameters: NotRequired[Dict[str, str]],
    exportDataSetNames: NotRequired[List[str]],
    properties: NotRequired[MainframeActionPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: MainframeResourceSummaryTypeDef](./type_defs.md#mainframeresourcesummarytypedef) 
2. See [:material-code-braces: MainframeActionPropertiesTypeDef](./type_defs.md#mainframeactionpropertiestypedef) 
## TN3270StepInputTypeDef

```python
# TN3270StepInputTypeDef definition

class TN3270StepInputTypeDef(TypedDict):
    resource: MainframeResourceSummaryTypeDef,  # (1)
    script: ScriptSummaryTypeDef,  # (2)
    exportDataSetNames: NotRequired[List[str]],
    properties: NotRequired[MainframeActionPropertiesTypeDef],  # (3)
```

1. See [:material-code-braces: MainframeResourceSummaryTypeDef](./type_defs.md#mainframeresourcesummarytypedef) 
2. See [:material-code-braces: ScriptSummaryTypeDef](./type_defs.md#scriptsummarytypedef) 
3. See [:material-code-braces: MainframeActionPropertiesTypeDef](./type_defs.md#mainframeactionpropertiestypedef) 
## ResourceOutputTypeDef

```python
# ResourceOutputTypeDef definition

class ResourceOutputTypeDef(TypedDict):
    name: str,
    type: ResourceTypeOutputTypeDef,  # (1)
```

1. See [:material-code-braces: ResourceTypeOutputTypeDef](./type_defs.md#resourcetypeoutputtypedef) 
## MainframeActionTypeOutputTypeDef

```python
# MainframeActionTypeOutputTypeDef definition

class MainframeActionTypeOutputTypeDef(TypedDict):
    batch: NotRequired[BatchOutputTypeDef],  # (1)
    tn3270: NotRequired[TN3270OutputTypeDef],  # (2)
```

1. See [:material-code-braces: BatchOutputTypeDef](./type_defs.md#batchoutputtypedef) 
2. See [:material-code-braces: TN3270OutputTypeDef](./type_defs.md#tn3270outputtypedef) 
## CompareFileTypeTypeDef

```python
# CompareFileTypeTypeDef definition

class CompareFileTypeTypeDef(TypedDict):
    datasets: NotRequired[CompareDataSetsSummaryTypeDef],  # (1)
    databaseCDC: NotRequired[CompareDatabaseCDCSummaryTypeDef],  # (2)
```

1. See [:material-code-braces: CompareDataSetsSummaryTypeDef](./type_defs.md#comparedatasetssummarytypedef) 
2. See [:material-code-braces: CompareDatabaseCDCSummaryTypeDef](./type_defs.md#comparedatabasecdcsummarytypedef) 
## InputFileOutputTypeDef

```python
# InputFileOutputTypeDef definition

class InputFileOutputTypeDef(TypedDict):
    sourceLocation: str,
    targetLocation: str,
    fileMetadata: FileMetadataOutputTypeDef,  # (1)
```

1. See [:material-code-braces: FileMetadataOutputTypeDef](./type_defs.md#filemetadataoutputtypedef) 
## ResourceActionSummaryTypeDef

```python
# ResourceActionSummaryTypeDef definition

class ResourceActionSummaryTypeDef(TypedDict):
    cloudFormation: NotRequired[CloudFormationStepSummaryTypeDef],  # (1)
    m2ManagedApplication: NotRequired[M2ManagedApplicationStepSummaryTypeDef],  # (2)
    m2NonManagedApplication: NotRequired[M2NonManagedApplicationStepSummaryTypeDef],  # (3)
```

1. See [:material-code-braces: CloudFormationStepSummaryTypeDef](./type_defs.md#cloudformationstepsummarytypedef) 
2. See [:material-code-braces: M2ManagedApplicationStepSummaryTypeDef](./type_defs.md#m2managedapplicationstepsummarytypedef) 
3. See [:material-code-braces: M2NonManagedApplicationStepSummaryTypeDef](./type_defs.md#m2nonmanagedapplicationstepsummarytypedef) 
## BatchSummaryTypeDef

```python
# BatchSummaryTypeDef definition

class BatchSummaryTypeDef(TypedDict):
    stepInput: BatchStepInputTypeDef,  # (1)
    stepOutput: NotRequired[BatchStepOutputTypeDef],  # (2)
```

1. See [:material-code-braces: BatchStepInputTypeDef](./type_defs.md#batchstepinputtypedef) 
2. See [:material-code-braces: BatchStepOutputTypeDef](./type_defs.md#batchstepoutputtypedef) 
## TN3270SummaryTypeDef

```python
# TN3270SummaryTypeDef definition

class TN3270SummaryTypeDef(TypedDict):
    stepInput: TN3270StepInputTypeDef,  # (1)
    stepOutput: NotRequired[TN3270StepOutputTypeDef],  # (2)
```

1. See [:material-code-braces: TN3270StepInputTypeDef](./type_defs.md#tn3270stepinputtypedef) 
2. See [:material-code-braces: TN3270StepOutputTypeDef](./type_defs.md#tn3270stepoutputtypedef) 
## GetTestConfigurationResponseTypeDef

```python
# GetTestConfigurationResponseTypeDef definition

class GetTestConfigurationResponseTypeDef(TypedDict):
    testConfigurationId: str,
    name: str,
    testConfigurationArn: str,
    latestVersion: TestConfigurationLatestVersionTypeDef,  # (1)
    testConfigurationVersion: int,
    status: TestConfigurationLifecycleType,  # (2)
    statusReason: str,
    creationTime: datetime,
    lastUpdateTime: datetime,
    description: str,
    resources: List[ResourceOutputTypeDef],  # (3)
    properties: Dict[str, str],
    tags: Dict[str, str],
    serviceSettings: ServiceSettingsTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: TestConfigurationLatestVersionTypeDef](./type_defs.md#testconfigurationlatestversiontypedef) 
2. See [:material-code-brackets: TestConfigurationLifecycleType](./literals.md#testconfigurationlifecycletype) 
3. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
4. See [:material-code-braces: ServiceSettingsTypeDef](./type_defs.md#servicesettingstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MainframeActionOutputTypeDef

```python
# MainframeActionOutputTypeDef definition

class MainframeActionOutputTypeDef(TypedDict):
    resource: str,
    actionType: MainframeActionTypeOutputTypeDef,  # (1)
    properties: NotRequired[MainframeActionPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: MainframeActionTypeOutputTypeDef](./type_defs.md#mainframeactiontypeoutputtypedef) 
2. See [:material-code-braces: MainframeActionPropertiesTypeDef](./type_defs.md#mainframeactionpropertiestypedef) 
## MainframeActionTypeTypeDef

```python
# MainframeActionTypeTypeDef definition

class MainframeActionTypeTypeDef(TypedDict):
    batch: NotRequired[BatchUnionTypeDef],  # (1)
    tn3270: NotRequired[TN3270UnionTypeDef],  # (2)
```

1. See [:material-code-braces: BatchTypeDef](./type_defs.md#batchtypedef) [:material-code-braces: BatchOutputTypeDef](./type_defs.md#batchoutputtypedef) 
2. See [:material-code-braces: TN3270TypeDef](./type_defs.md#tn3270typedef) [:material-code-braces: TN3270OutputTypeDef](./type_defs.md#tn3270outputtypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    name: str,
    type: ResourceTypeUnionTypeDef,  # (1)
```

1. See [:material-code-braces: ResourceTypeTypeDef](./type_defs.md#resourcetypetypedef) [:material-code-braces: ResourceTypeOutputTypeDef](./type_defs.md#resourcetypeoutputtypedef) 
## FileTypeDef

```python
# FileTypeDef definition

class FileTypeDef(TypedDict):
    fileType: NotRequired[CompareFileTypeTypeDef],  # (1)
```

1. See [:material-code-braces: CompareFileTypeTypeDef](./type_defs.md#comparefiletypetypedef) 
## InputOutputTypeDef

```python
# InputOutputTypeDef definition

class InputOutputTypeDef(TypedDict):
    file: NotRequired[InputFileOutputTypeDef],  # (1)
```

1. See [:material-code-braces: InputFileOutputTypeDef](./type_defs.md#inputfileoutputtypedef) 
## InputFileTypeDef

```python
# InputFileTypeDef definition

class InputFileTypeDef(TypedDict):
    sourceLocation: str,
    targetLocation: str,
    fileMetadata: FileMetadataUnionTypeDef,  # (1)
```

1. See [:material-code-braces: FileMetadataTypeDef](./type_defs.md#filemetadatatypedef) [:material-code-braces: FileMetadataOutputTypeDef](./type_defs.md#filemetadataoutputtypedef) 
## MainframeActionSummaryTypeDef

```python
# MainframeActionSummaryTypeDef definition

class MainframeActionSummaryTypeDef(TypedDict):
    batch: NotRequired[BatchSummaryTypeDef],  # (1)
    tn3270: NotRequired[TN3270SummaryTypeDef],  # (2)
```

1. See [:material-code-braces: BatchSummaryTypeDef](./type_defs.md#batchsummarytypedef) 
2. See [:material-code-braces: TN3270SummaryTypeDef](./type_defs.md#tn3270summarytypedef) 
## UpdateTestConfigurationRequestRequestTypeDef

```python
# UpdateTestConfigurationRequestRequestTypeDef definition

class UpdateTestConfigurationRequestRequestTypeDef(TypedDict):
    testConfigurationId: str,
    description: NotRequired[str],
    resources: NotRequired[Sequence[ResourceTypeDef]],  # (1)
    properties: NotRequired[Mapping[str, str]],
    serviceSettings: NotRequired[ServiceSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ServiceSettingsTypeDef](./type_defs.md#servicesettingstypedef) 
## CompareActionSummaryTypeDef

```python
# CompareActionSummaryTypeDef definition

class CompareActionSummaryTypeDef(TypedDict):
    type: FileTypeDef,  # (1)
```

1. See [:material-code-braces: FileTypeDef](./type_defs.md#filetypedef) 
## CompareActionOutputTypeDef

```python
# CompareActionOutputTypeDef definition

class CompareActionOutputTypeDef(TypedDict):
    input: InputOutputTypeDef,  # (1)
    output: NotRequired[OutputTypeDef],  # (2)
```

1. See [:material-code-braces: InputOutputTypeDef](./type_defs.md#inputoutputtypedef) 
2. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
## MainframeActionTypeDef

```python
# MainframeActionTypeDef definition

class MainframeActionTypeDef(TypedDict):
    resource: str,
    actionType: MainframeActionTypeUnionTypeDef,  # (1)
    properties: NotRequired[MainframeActionPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: MainframeActionTypeTypeDef](./type_defs.md#mainframeactiontypetypedef) [:material-code-braces: MainframeActionTypeOutputTypeDef](./type_defs.md#mainframeactiontypeoutputtypedef) 
2. See [:material-code-braces: MainframeActionPropertiesTypeDef](./type_defs.md#mainframeactionpropertiestypedef) 
## CreateTestConfigurationRequestRequestTypeDef

```python
# CreateTestConfigurationRequestRequestTypeDef definition

class CreateTestConfigurationRequestRequestTypeDef(TypedDict):
    name: str,
    resources: Sequence[ResourceUnionTypeDef],  # (1)
    description: NotRequired[str],
    properties: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    serviceSettings: NotRequired[ServiceSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
2. See [:material-code-braces: ServiceSettingsTypeDef](./type_defs.md#servicesettingstypedef) 
## StepRunSummaryTypeDef

```python
# StepRunSummaryTypeDef definition

class StepRunSummaryTypeDef(TypedDict):
    mainframeAction: NotRequired[MainframeActionSummaryTypeDef],  # (1)
    compareAction: NotRequired[CompareActionSummaryTypeDef],  # (2)
    resourceAction: NotRequired[ResourceActionSummaryTypeDef],  # (3)
```

1. See [:material-code-braces: MainframeActionSummaryTypeDef](./type_defs.md#mainframeactionsummarytypedef) 
2. See [:material-code-braces: CompareActionSummaryTypeDef](./type_defs.md#compareactionsummarytypedef) 
3. See [:material-code-braces: ResourceActionSummaryTypeDef](./type_defs.md#resourceactionsummarytypedef) 
## StepActionOutputTypeDef

```python
# StepActionOutputTypeDef definition

class StepActionOutputTypeDef(TypedDict):
    resourceAction: NotRequired[ResourceActionTypeDef],  # (1)
    mainframeAction: NotRequired[MainframeActionOutputTypeDef],  # (2)
    compareAction: NotRequired[CompareActionOutputTypeDef],  # (3)
```

1. See [:material-code-braces: ResourceActionTypeDef](./type_defs.md#resourceactiontypedef) 
2. See [:material-code-braces: MainframeActionOutputTypeDef](./type_defs.md#mainframeactionoutputtypedef) 
3. See [:material-code-braces: CompareActionOutputTypeDef](./type_defs.md#compareactionoutputtypedef) 
## InputTypeDef

```python
# InputTypeDef definition

class InputTypeDef(TypedDict):
    file: NotRequired[InputFileUnionTypeDef],  # (1)
```

1. See [:material-code-braces: InputFileTypeDef](./type_defs.md#inputfiletypedef) [:material-code-braces: InputFileOutputTypeDef](./type_defs.md#inputfileoutputtypedef) 
## GetTestRunStepResponseTypeDef

```python
# GetTestRunStepResponseTypeDef definition

class GetTestRunStepResponseTypeDef(TypedDict):
    stepName: str,
    testRunId: str,
    testCaseId: str,
    testCaseVersion: int,
    testSuiteId: str,
    testSuiteVersion: int,
    beforeStep: bool,
    afterStep: bool,
    status: StepRunStatusType,  # (1)
    statusReason: str,
    runStartTime: datetime,
    runEndTime: datetime,
    stepRunSummary: StepRunSummaryTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: StepRunStatusType](./literals.md#steprunstatustype) 
2. See [:material-code-braces: StepRunSummaryTypeDef](./type_defs.md#steprunsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StepOutputTypeDef

```python
# StepOutputTypeDef definition

class StepOutputTypeDef(TypedDict):
    name: str,
    action: StepActionOutputTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: StepActionOutputTypeDef](./type_defs.md#stepactionoutputtypedef) 
## GetTestCaseResponseTypeDef

```python
# GetTestCaseResponseTypeDef definition

class GetTestCaseResponseTypeDef(TypedDict):
    testCaseId: str,
    testCaseArn: str,
    name: str,
    description: str,
    latestVersion: TestCaseLatestVersionTypeDef,  # (1)
    testCaseVersion: int,
    status: TestCaseLifecycleType,  # (2)
    statusReason: str,
    creationTime: datetime,
    lastUpdateTime: datetime,
    steps: List[StepOutputTypeDef],  # (3)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TestCaseLatestVersionTypeDef](./type_defs.md#testcaselatestversiontypedef) 
2. See [:material-code-brackets: TestCaseLifecycleType](./literals.md#testcaselifecycletype) 
3. See [:material-code-braces: StepOutputTypeDef](./type_defs.md#stepoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTestSuiteResponseTypeDef

```python
# GetTestSuiteResponseTypeDef definition

class GetTestSuiteResponseTypeDef(TypedDict):
    testSuiteId: str,
    name: str,
    latestVersion: TestSuiteLatestVersionTypeDef,  # (1)
    testSuiteVersion: int,
    status: TestSuiteLifecycleType,  # (2)
    statusReason: str,
    testSuiteArn: str,
    creationTime: datetime,
    lastUpdateTime: datetime,
    description: str,
    beforeSteps: List[StepOutputTypeDef],  # (3)
    afterSteps: List[StepOutputTypeDef],  # (3)
    testCases: TestCasesOutputTypeDef,  # (5)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: TestSuiteLatestVersionTypeDef](./type_defs.md#testsuitelatestversiontypedef) 
2. See [:material-code-brackets: TestSuiteLifecycleType](./literals.md#testsuitelifecycletype) 
3. See [:material-code-braces: StepOutputTypeDef](./type_defs.md#stepoutputtypedef) 
4. See [:material-code-braces: StepOutputTypeDef](./type_defs.md#stepoutputtypedef) 
5. See [:material-code-braces: TestCasesOutputTypeDef](./type_defs.md#testcasesoutputtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CompareActionTypeDef

```python
# CompareActionTypeDef definition

class CompareActionTypeDef(TypedDict):
    input: InputUnionTypeDef,  # (1)
    output: NotRequired[OutputTypeDef],  # (2)
```

1. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) [:material-code-braces: InputOutputTypeDef](./type_defs.md#inputoutputtypedef) 
2. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
## StepActionTypeDef

```python
# StepActionTypeDef definition

class StepActionTypeDef(TypedDict):
    resourceAction: NotRequired[ResourceActionTypeDef],  # (1)
    mainframeAction: NotRequired[MainframeActionUnionTypeDef],  # (2)
    compareAction: NotRequired[CompareActionUnionTypeDef],  # (3)
```

1. See [:material-code-braces: ResourceActionTypeDef](./type_defs.md#resourceactiontypedef) 
2. See [:material-code-braces: MainframeActionTypeDef](./type_defs.md#mainframeactiontypedef) [:material-code-braces: MainframeActionOutputTypeDef](./type_defs.md#mainframeactionoutputtypedef) 
3. See [:material-code-braces: CompareActionTypeDef](./type_defs.md#compareactiontypedef) [:material-code-braces: CompareActionOutputTypeDef](./type_defs.md#compareactionoutputtypedef) 
## StepTypeDef

```python
# StepTypeDef definition

class StepTypeDef(TypedDict):
    name: str,
    action: StepActionUnionTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: StepActionTypeDef](./type_defs.md#stepactiontypedef) [:material-code-braces: StepActionOutputTypeDef](./type_defs.md#stepactionoutputtypedef) 
## CreateTestSuiteRequestRequestTypeDef

```python
# CreateTestSuiteRequestRequestTypeDef definition

class CreateTestSuiteRequestRequestTypeDef(TypedDict):
    name: str,
    testCases: TestCasesTypeDef,  # (1)
    description: NotRequired[str],
    beforeSteps: NotRequired[Sequence[StepTypeDef]],  # (2)
    afterSteps: NotRequired[Sequence[StepTypeDef]],  # (2)
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: TestCasesTypeDef](./type_defs.md#testcasestypedef) 
2. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
3. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
## UpdateTestCaseRequestRequestTypeDef

```python
# UpdateTestCaseRequestRequestTypeDef definition

class UpdateTestCaseRequestRequestTypeDef(TypedDict):
    testCaseId: str,
    description: NotRequired[str],
    steps: NotRequired[Sequence[StepTypeDef]],  # (1)
```

1. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
## UpdateTestSuiteRequestRequestTypeDef

```python
# UpdateTestSuiteRequestRequestTypeDef definition

class UpdateTestSuiteRequestRequestTypeDef(TypedDict):
    testSuiteId: str,
    description: NotRequired[str],
    beforeSteps: NotRequired[Sequence[StepTypeDef]],  # (1)
    afterSteps: NotRequired[Sequence[StepTypeDef]],  # (1)
    testCases: NotRequired[TestCasesTypeDef],  # (3)
```

1. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
2. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
3. See [:material-code-braces: TestCasesTypeDef](./type_defs.md#testcasestypedef) 
## CreateTestCaseRequestRequestTypeDef

```python
# CreateTestCaseRequestRequestTypeDef definition

class CreateTestCaseRequestRequestTypeDef(TypedDict):
    name: str,
    steps: Sequence[StepUnionTypeDef],  # (1)
    description: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) [:material-code-braces: StepOutputTypeDef](./type_defs.md#stepoutputtypedef) 
