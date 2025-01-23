# Type definitions

> [Index](../README.md) > [GlueDataBrew](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [GlueDataBrew](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#gluedatabrew)
    type annotations stubs module [types-aiobotocore-databrew](https://pypi.org/project/types-aiobotocore-databrew/).

## AllowedStatisticsUnionTypeDef

```python
# AllowedStatisticsUnionTypeDef definition

AllowedStatisticsUnionTypeDef = Union[
    AllowedStatisticsTypeDef,  # (1)
    AllowedStatisticsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AllowedStatisticsTypeDef](./type_defs.md#allowedstatisticstypedef) 
2. See [:material-code-braces: AllowedStatisticsOutputTypeDef](./type_defs.md#allowedstatisticsoutputtypedef) 

## ExcelOptionsUnionTypeDef

```python
# ExcelOptionsUnionTypeDef definition

ExcelOptionsUnionTypeDef = Union[
    ExcelOptionsTypeDef,  # (1)
    ExcelOptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ExcelOptionsTypeDef](./type_defs.md#exceloptionstypedef) 
2. See [:material-code-braces: ExcelOptionsOutputTypeDef](./type_defs.md#exceloptionsoutputtypedef) 

## FilterExpressionUnionTypeDef

```python
# FilterExpressionUnionTypeDef definition

FilterExpressionUnionTypeDef = Union[
    FilterExpressionTypeDef,  # (1)
    FilterExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FilterExpressionTypeDef](./type_defs.md#filterexpressiontypedef) 
2. See [:material-code-braces: FilterExpressionOutputTypeDef](./type_defs.md#filterexpressionoutputtypedef) 

## RecipeActionUnionTypeDef

```python
# RecipeActionUnionTypeDef definition

RecipeActionUnionTypeDef = Union[
    RecipeActionTypeDef,  # (1)
    RecipeActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RecipeActionTypeDef](./type_defs.md#recipeactiontypedef) 
2. See [:material-code-braces: RecipeActionOutputTypeDef](./type_defs.md#recipeactionoutputtypedef) 

## StatisticOverrideUnionTypeDef

```python
# StatisticOverrideUnionTypeDef definition

StatisticOverrideUnionTypeDef = Union[
    StatisticOverrideTypeDef,  # (1)
    StatisticOverrideOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StatisticOverrideTypeDef](./type_defs.md#statisticoverridetypedef) 
2. See [:material-code-braces: StatisticOverrideOutputTypeDef](./type_defs.md#statisticoverrideoutputtypedef) 

## RuleUnionTypeDef

```python
# RuleUnionTypeDef definition

RuleUnionTypeDef = Union[
    RuleTypeDef,  # (1)
    RuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 

## EntityDetectorConfigurationUnionTypeDef

```python
# EntityDetectorConfigurationUnionTypeDef definition

EntityDetectorConfigurationUnionTypeDef = Union[
    EntityDetectorConfigurationTypeDef,  # (1)
    EntityDetectorConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EntityDetectorConfigurationTypeDef](./type_defs.md#entitydetectorconfigurationtypedef) 
2. See [:material-code-braces: EntityDetectorConfigurationOutputTypeDef](./type_defs.md#entitydetectorconfigurationoutputtypedef) 

## UnionTypeDef

```python
# UnionTypeDef definition

UnionTypeDef = Union[
    OutputTypeDef,  # (1)
    ExtraOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
2. See [:material-code-braces: ExtraOutputTypeDef](./type_defs.md#extraoutputtypedef) 

## DatasetParameterUnionTypeDef

```python
# DatasetParameterUnionTypeDef definition

DatasetParameterUnionTypeDef = Union[
    DatasetParameterTypeDef,  # (1)
    DatasetParameterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DatasetParameterTypeDef](./type_defs.md#datasetparametertypedef) 
2. See [:material-code-braces: DatasetParameterOutputTypeDef](./type_defs.md#datasetparameteroutputtypedef) 

## RecipeStepUnionTypeDef

```python
# RecipeStepUnionTypeDef definition

RecipeStepUnionTypeDef = Union[
    RecipeStepTypeDef,  # (1)
    RecipeStepOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RecipeStepTypeDef](./type_defs.md#recipesteptypedef) 
2. See [:material-code-braces: RecipeStepOutputTypeDef](./type_defs.md#recipestepoutputtypedef) 

## StatisticsConfigurationUnionTypeDef

```python
# StatisticsConfigurationUnionTypeDef definition

StatisticsConfigurationUnionTypeDef = Union[
    StatisticsConfigurationTypeDef,  # (1)
    StatisticsConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StatisticsConfigurationTypeDef](./type_defs.md#statisticsconfigurationtypedef) 
2. See [:material-code-braces: StatisticsConfigurationOutputTypeDef](./type_defs.md#statisticsconfigurationoutputtypedef) 

## ColumnStatisticsConfigurationUnionTypeDef

```python
# ColumnStatisticsConfigurationUnionTypeDef definition

ColumnStatisticsConfigurationUnionTypeDef = Union[
    ColumnStatisticsConfigurationTypeDef,  # (1)
    ColumnStatisticsConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ColumnStatisticsConfigurationTypeDef](./type_defs.md#columnstatisticsconfigurationtypedef) 
2. See [:material-code-braces: ColumnStatisticsConfigurationOutputTypeDef](./type_defs.md#columnstatisticsconfigurationoutputtypedef) 



## AllowedStatisticsOutputTypeDef

```python
# AllowedStatisticsOutputTypeDef definition

class AllowedStatisticsOutputTypeDef(TypedDict):
    Statistics: List[str],
```

## AllowedStatisticsTypeDef

```python
# AllowedStatisticsTypeDef definition

class AllowedStatisticsTypeDef(TypedDict):
    Statistics: Sequence[str],
```

## BatchDeleteRecipeVersionRequestRequestTypeDef

```python
# BatchDeleteRecipeVersionRequestRequestTypeDef definition

class BatchDeleteRecipeVersionRequestRequestTypeDef(TypedDict):
    Name: str,
    RecipeVersions: Sequence[str],
```

## RecipeVersionErrorDetailTypeDef

```python
# RecipeVersionErrorDetailTypeDef definition

class RecipeVersionErrorDetailTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
    RecipeVersion: NotRequired[str],
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

## ColumnSelectorTypeDef

```python
# ColumnSelectorTypeDef definition

class ColumnSelectorTypeDef(TypedDict):
    Regex: NotRequired[str],
    Name: NotRequired[str],
```

## ConditionExpressionTypeDef

```python
# ConditionExpressionTypeDef definition

class ConditionExpressionTypeDef(TypedDict):
    Condition: str,
    TargetColumn: str,
    Value: NotRequired[str],
```

## JobSampleTypeDef

```python
# JobSampleTypeDef definition

class JobSampleTypeDef(TypedDict):
    Mode: NotRequired[SampleModeType],  # (1)
    Size: NotRequired[int],
```

1. See [:material-code-brackets: SampleModeType](./literals.md#samplemodetype) 
## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    Bucket: str,
    Key: NotRequired[str],
    BucketOwner: NotRequired[str],
```

## ValidationConfigurationTypeDef

```python
# ValidationConfigurationTypeDef definition

class ValidationConfigurationTypeDef(TypedDict):
    RulesetArn: str,
    ValidationMode: NotRequired[ValidationModeType],  # (1)
```

1. See [:material-code-brackets: ValidationModeType](./literals.md#validationmodetype) 
## SampleTypeDef

```python
# SampleTypeDef definition

class SampleTypeDef(TypedDict):
    Type: SampleTypeType,  # (1)
    Size: NotRequired[int],
```

1. See [:material-code-brackets: SampleTypeType](./literals.md#sampletypetype) 
## RecipeReferenceTypeDef

```python
# RecipeReferenceTypeDef definition

class RecipeReferenceTypeDef(TypedDict):
    Name: str,
    RecipeVersion: NotRequired[str],
```

## CreateScheduleRequestRequestTypeDef

```python
# CreateScheduleRequestRequestTypeDef definition

class CreateScheduleRequestRequestTypeDef(TypedDict):
    CronExpression: str,
    Name: str,
    JobNames: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
```

## CsvOptionsTypeDef

```python
# CsvOptionsTypeDef definition

class CsvOptionsTypeDef(TypedDict):
    Delimiter: NotRequired[str],
    HeaderRow: NotRequired[bool],
```

## CsvOutputOptionsTypeDef

```python
# CsvOutputOptionsTypeDef definition

class CsvOutputOptionsTypeDef(TypedDict):
    Delimiter: NotRequired[str],
```

## DatetimeOptionsTypeDef

```python
# DatetimeOptionsTypeDef definition

class DatetimeOptionsTypeDef(TypedDict):
    Format: str,
    TimezoneOffset: NotRequired[str],
    LocaleCode: NotRequired[str],
```

## FilterExpressionOutputTypeDef

```python
# FilterExpressionOutputTypeDef definition

class FilterExpressionOutputTypeDef(TypedDict):
    Expression: str,
    ValuesMap: Dict[str, str],
```

## DeleteDatasetRequestRequestTypeDef

```python
# DeleteDatasetRequestRequestTypeDef definition

class DeleteDatasetRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteJobRequestRequestTypeDef

```python
# DeleteJobRequestRequestTypeDef definition

class DeleteJobRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteProjectRequestRequestTypeDef

```python
# DeleteProjectRequestRequestTypeDef definition

class DeleteProjectRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteRecipeVersionRequestRequestTypeDef

```python
# DeleteRecipeVersionRequestRequestTypeDef definition

class DeleteRecipeVersionRequestRequestTypeDef(TypedDict):
    Name: str,
    RecipeVersion: str,
```

## DeleteRulesetRequestRequestTypeDef

```python
# DeleteRulesetRequestRequestTypeDef definition

class DeleteRulesetRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteScheduleRequestRequestTypeDef

```python
# DeleteScheduleRequestRequestTypeDef definition

class DeleteScheduleRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DescribeDatasetRequestRequestTypeDef

```python
# DescribeDatasetRequestRequestTypeDef definition

class DescribeDatasetRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DescribeJobRequestRequestTypeDef

```python
# DescribeJobRequestRequestTypeDef definition

class DescribeJobRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DescribeJobRunRequestRequestTypeDef

```python
# DescribeJobRunRequestRequestTypeDef definition

class DescribeJobRunRequestRequestTypeDef(TypedDict):
    Name: str,
    RunId: str,
```

## DescribeProjectRequestRequestTypeDef

```python
# DescribeProjectRequestRequestTypeDef definition

class DescribeProjectRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DescribeRecipeRequestRequestTypeDef

```python
# DescribeRecipeRequestRequestTypeDef definition

class DescribeRecipeRequestRequestTypeDef(TypedDict):
    Name: str,
    RecipeVersion: NotRequired[str],
```

## DescribeRulesetRequestRequestTypeDef

```python
# DescribeRulesetRequestRequestTypeDef definition

class DescribeRulesetRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DescribeScheduleRequestRequestTypeDef

```python
# DescribeScheduleRequestRequestTypeDef definition

class DescribeScheduleRequestRequestTypeDef(TypedDict):
    Name: str,
```

## ExcelOptionsOutputTypeDef

```python
# ExcelOptionsOutputTypeDef definition

class ExcelOptionsOutputTypeDef(TypedDict):
    SheetNames: NotRequired[List[str]],
    SheetIndexes: NotRequired[List[int]],
    HeaderRow: NotRequired[bool],
```

## ExcelOptionsTypeDef

```python
# ExcelOptionsTypeDef definition

class ExcelOptionsTypeDef(TypedDict):
    SheetNames: NotRequired[Sequence[str]],
    SheetIndexes: NotRequired[Sequence[int]],
    HeaderRow: NotRequired[bool],
```

## FilesLimitTypeDef

```python
# FilesLimitTypeDef definition

class FilesLimitTypeDef(TypedDict):
    MaxFiles: int,
    OrderedBy: NotRequired[OrderedByType],  # (1)
    Order: NotRequired[OrderType],  # (2)
```

1. See [:material-code-brackets: OrderedByType](./literals.md#orderedbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## FilterExpressionTypeDef

```python
# FilterExpressionTypeDef definition

class FilterExpressionTypeDef(TypedDict):
    Expression: str,
    ValuesMap: Mapping[str, str],
```

## JsonOptionsTypeDef

```python
# JsonOptionsTypeDef definition

class JsonOptionsTypeDef(TypedDict):
    MultiLine: NotRequired[bool],
```

## MetadataTypeDef

```python
# MetadataTypeDef definition

class MetadataTypeDef(TypedDict):
    SourceArn: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDatasetsRequestRequestTypeDef

```python
# ListDatasetsRequestRequestTypeDef definition

class ListDatasetsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListJobRunsRequestRequestTypeDef

```python
# ListJobRunsRequestRequestTypeDef definition

class ListJobRunsRequestRequestTypeDef(TypedDict):
    Name: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListJobsRequestRequestTypeDef

```python
# ListJobsRequestRequestTypeDef definition

class ListJobsRequestRequestTypeDef(TypedDict):
    DatasetName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ProjectName: NotRequired[str],
```

## ListProjectsRequestRequestTypeDef

```python
# ListProjectsRequestRequestTypeDef definition

class ListProjectsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListRecipeVersionsRequestRequestTypeDef

```python
# ListRecipeVersionsRequestRequestTypeDef definition

class ListRecipeVersionsRequestRequestTypeDef(TypedDict):
    Name: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListRecipesRequestRequestTypeDef

```python
# ListRecipesRequestRequestTypeDef definition

class ListRecipesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    RecipeVersion: NotRequired[str],
```

## ListRulesetsRequestRequestTypeDef

```python
# ListRulesetsRequestRequestTypeDef definition

class ListRulesetsRequestRequestTypeDef(TypedDict):
    TargetArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## RulesetItemTypeDef

```python
# RulesetItemTypeDef definition

class RulesetItemTypeDef(TypedDict):
    Name: str,
    TargetArn: str,
    AccountId: NotRequired[str],
    CreatedBy: NotRequired[str],
    CreateDate: NotRequired[datetime],
    Description: NotRequired[str],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    ResourceArn: NotRequired[str],
    RuleCount: NotRequired[int],
    Tags: NotRequired[Dict[str, str]],
```

## ListSchedulesRequestRequestTypeDef

```python
# ListSchedulesRequestRequestTypeDef definition

class ListSchedulesRequestRequestTypeDef(TypedDict):
    JobName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ScheduleTypeDef

```python
# ScheduleTypeDef definition

class ScheduleTypeDef(TypedDict):
    Name: str,
    AccountId: NotRequired[str],
    CreatedBy: NotRequired[str],
    CreateDate: NotRequired[datetime],
    JobNames: NotRequired[List[str]],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    ResourceArn: NotRequired[str],
    CronExpression: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## PublishRecipeRequestRequestTypeDef

```python
# PublishRecipeRequestRequestTypeDef definition

class PublishRecipeRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
```

## RecipeActionOutputTypeDef

```python
# RecipeActionOutputTypeDef definition

class RecipeActionOutputTypeDef(TypedDict):
    Operation: str,
    Parameters: NotRequired[Dict[str, str]],
```

## RecipeActionTypeDef

```python
# RecipeActionTypeDef definition

class RecipeActionTypeDef(TypedDict):
    Operation: str,
    Parameters: NotRequired[Mapping[str, str]],
```

## ThresholdTypeDef

```python
# ThresholdTypeDef definition

class ThresholdTypeDef(TypedDict):
    Value: float,
    Type: NotRequired[ThresholdTypeType],  # (1)
    Unit: NotRequired[ThresholdUnitType],  # (2)
```

1. See [:material-code-brackets: ThresholdTypeType](./literals.md#thresholdtypetype) 
2. See [:material-code-brackets: ThresholdUnitType](./literals.md#thresholdunittype) 
## ViewFrameTypeDef

```python
# ViewFrameTypeDef definition

class ViewFrameTypeDef(TypedDict):
    StartColumnIndex: int,
    ColumnRange: NotRequired[int],
    HiddenColumns: NotRequired[Sequence[str]],
    StartRowIndex: NotRequired[int],
    RowRange: NotRequired[int],
    Analytics: NotRequired[AnalyticsModeType],  # (1)
```

1. See [:material-code-brackets: AnalyticsModeType](./literals.md#analyticsmodetype) 
## StartJobRunRequestRequestTypeDef

```python
# StartJobRunRequestRequestTypeDef definition

class StartJobRunRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StartProjectSessionRequestRequestTypeDef

```python
# StartProjectSessionRequestRequestTypeDef definition

class StartProjectSessionRequestRequestTypeDef(TypedDict):
    Name: str,
    AssumeControl: NotRequired[bool],
```

## StatisticOverrideOutputTypeDef

```python
# StatisticOverrideOutputTypeDef definition

class StatisticOverrideOutputTypeDef(TypedDict):
    Statistic: str,
    Parameters: Dict[str, str],
```

## StatisticOverrideTypeDef

```python
# StatisticOverrideTypeDef definition

class StatisticOverrideTypeDef(TypedDict):
    Statistic: str,
    Parameters: Mapping[str, str],
```

## StopJobRunRequestRequestTypeDef

```python
# StopJobRunRequestRequestTypeDef definition

class StopJobRunRequestRequestTypeDef(TypedDict):
    Name: str,
    RunId: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateScheduleRequestRequestTypeDef

```python
# UpdateScheduleRequestRequestTypeDef definition

class UpdateScheduleRequestRequestTypeDef(TypedDict):
    CronExpression: str,
    Name: str,
    JobNames: NotRequired[Sequence[str]],
```

## EntityDetectorConfigurationOutputTypeDef

```python
# EntityDetectorConfigurationOutputTypeDef definition

class EntityDetectorConfigurationOutputTypeDef(TypedDict):
    EntityTypes: List[str],
    AllowedStatistics: NotRequired[List[AllowedStatisticsOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: AllowedStatisticsOutputTypeDef](./type_defs.md#allowedstatisticsoutputtypedef) 
## BatchDeleteRecipeVersionResponseTypeDef

```python
# BatchDeleteRecipeVersionResponseTypeDef definition

class BatchDeleteRecipeVersionResponseTypeDef(TypedDict):
    Name: str,
    Errors: List[RecipeVersionErrorDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecipeVersionErrorDetailTypeDef](./type_defs.md#recipeversionerrordetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatasetResponseTypeDef

```python
# CreateDatasetResponseTypeDef definition

class CreateDatasetResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProfileJobResponseTypeDef

```python
# CreateProfileJobResponseTypeDef definition

class CreateProfileJobResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectResponseTypeDef

```python
# CreateProjectResponseTypeDef definition

class CreateProjectResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRecipeJobResponseTypeDef

```python
# CreateRecipeJobResponseTypeDef definition

class CreateRecipeJobResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRecipeResponseTypeDef

```python
# CreateRecipeResponseTypeDef definition

class CreateRecipeResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRulesetResponseTypeDef

```python
# CreateRulesetResponseTypeDef definition

class CreateRulesetResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateScheduleResponseTypeDef

```python
# CreateScheduleResponseTypeDef definition

class CreateScheduleResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDatasetResponseTypeDef

```python
# DeleteDatasetResponseTypeDef definition

class DeleteDatasetResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteJobResponseTypeDef

```python
# DeleteJobResponseTypeDef definition

class DeleteJobResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProjectResponseTypeDef

```python
# DeleteProjectResponseTypeDef definition

class DeleteProjectResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRecipeVersionResponseTypeDef

```python
# DeleteRecipeVersionResponseTypeDef definition

class DeleteRecipeVersionResponseTypeDef(TypedDict):
    Name: str,
    RecipeVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRulesetResponseTypeDef

```python
# DeleteRulesetResponseTypeDef definition

class DeleteRulesetResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteScheduleResponseTypeDef

```python
# DeleteScheduleResponseTypeDef definition

class DeleteScheduleResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScheduleResponseTypeDef

```python
# DescribeScheduleResponseTypeDef definition

class DescribeScheduleResponseTypeDef(TypedDict):
    CreateDate: datetime,
    CreatedBy: str,
    JobNames: List[str],
    LastModifiedBy: str,
    LastModifiedDate: datetime,
    ResourceArn: str,
    CronExpression: str,
    Tags: Dict[str, str],
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PublishRecipeResponseTypeDef

```python
# PublishRecipeResponseTypeDef definition

class PublishRecipeResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendProjectSessionActionResponseTypeDef

```python
# SendProjectSessionActionResponseTypeDef definition

class SendProjectSessionActionResponseTypeDef(TypedDict):
    Result: str,
    Name: str,
    ActionId: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartJobRunResponseTypeDef

```python
# StartJobRunResponseTypeDef definition

class StartJobRunResponseTypeDef(TypedDict):
    RunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartProjectSessionResponseTypeDef

```python
# StartProjectSessionResponseTypeDef definition

class StartProjectSessionResponseTypeDef(TypedDict):
    Name: str,
    ClientSessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopJobRunResponseTypeDef

```python
# StopJobRunResponseTypeDef definition

class StopJobRunResponseTypeDef(TypedDict):
    RunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDatasetResponseTypeDef

```python
# UpdateDatasetResponseTypeDef definition

class UpdateDatasetResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProfileJobResponseTypeDef

```python
# UpdateProfileJobResponseTypeDef definition

class UpdateProfileJobResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectResponseTypeDef

```python
# UpdateProjectResponseTypeDef definition

class UpdateProjectResponseTypeDef(TypedDict):
    LastModifiedDate: datetime,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRecipeJobResponseTypeDef

```python
# UpdateRecipeJobResponseTypeDef definition

class UpdateRecipeJobResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRecipeResponseTypeDef

```python
# UpdateRecipeResponseTypeDef definition

class UpdateRecipeResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRulesetResponseTypeDef

```python
# UpdateRulesetResponseTypeDef definition

class UpdateRulesetResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateScheduleResponseTypeDef

```python
# UpdateScheduleResponseTypeDef definition

class UpdateScheduleResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataCatalogInputDefinitionTypeDef

```python
# DataCatalogInputDefinitionTypeDef definition

class DataCatalogInputDefinitionTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    TempDirectory: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## DatabaseInputDefinitionTypeDef

```python
# DatabaseInputDefinitionTypeDef definition

class DatabaseInputDefinitionTypeDef(TypedDict):
    GlueConnectionName: str,
    DatabaseTableName: NotRequired[str],
    TempDirectory: NotRequired[S3LocationTypeDef],  # (1)
    QueryString: NotRequired[str],
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## DatabaseTableOutputOptionsTypeDef

```python
# DatabaseTableOutputOptionsTypeDef definition

class DatabaseTableOutputOptionsTypeDef(TypedDict):
    TableName: str,
    TempDirectory: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## S3TableOutputOptionsTypeDef

```python
# S3TableOutputOptionsTypeDef definition

class S3TableOutputOptionsTypeDef(TypedDict):
    Location: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## CreateProjectRequestRequestTypeDef

```python
# CreateProjectRequestRequestTypeDef definition

class CreateProjectRequestRequestTypeDef(TypedDict):
    DatasetName: str,
    Name: str,
    RecipeName: str,
    RoleArn: str,
    Sample: NotRequired[SampleTypeDef],  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SampleTypeDef](./type_defs.md#sampletypedef) 
## DescribeProjectResponseTypeDef

```python
# DescribeProjectResponseTypeDef definition

class DescribeProjectResponseTypeDef(TypedDict):
    CreateDate: datetime,
    CreatedBy: str,
    DatasetName: str,
    LastModifiedDate: datetime,
    LastModifiedBy: str,
    Name: str,
    RecipeName: str,
    ResourceArn: str,
    Sample: SampleTypeDef,  # (1)
    RoleArn: str,
    Tags: Dict[str, str],
    SessionStatus: SessionStatusType,  # (2)
    OpenedBy: str,
    OpenDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SampleTypeDef](./type_defs.md#sampletypedef) 
2. See [:material-code-brackets: SessionStatusType](./literals.md#sessionstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProjectTypeDef

```python
# ProjectTypeDef definition

class ProjectTypeDef(TypedDict):
    Name: str,
    RecipeName: str,
    AccountId: NotRequired[str],
    CreateDate: NotRequired[datetime],
    CreatedBy: NotRequired[str],
    DatasetName: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    LastModifiedBy: NotRequired[str],
    ResourceArn: NotRequired[str],
    Sample: NotRequired[SampleTypeDef],  # (1)
    Tags: NotRequired[Dict[str, str]],
    RoleArn: NotRequired[str],
    OpenedBy: NotRequired[str],
    OpenDate: NotRequired[datetime],
```

1. See [:material-code-braces: SampleTypeDef](./type_defs.md#sampletypedef) 
## UpdateProjectRequestRequestTypeDef

```python
# UpdateProjectRequestRequestTypeDef definition

class UpdateProjectRequestRequestTypeDef(TypedDict):
    RoleArn: str,
    Name: str,
    Sample: NotRequired[SampleTypeDef],  # (1)
```

1. See [:material-code-braces: SampleTypeDef](./type_defs.md#sampletypedef) 
## OutputFormatOptionsTypeDef

```python
# OutputFormatOptionsTypeDef definition

class OutputFormatOptionsTypeDef(TypedDict):
    Csv: NotRequired[CsvOutputOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: CsvOutputOptionsTypeDef](./type_defs.md#csvoutputoptionstypedef) 
## DatasetParameterOutputTypeDef

```python
# DatasetParameterOutputTypeDef definition

class DatasetParameterOutputTypeDef(TypedDict):
    Name: str,
    Type: ParameterTypeType,  # (1)
    DatetimeOptions: NotRequired[DatetimeOptionsTypeDef],  # (2)
    CreateColumn: NotRequired[bool],
    Filter: NotRequired[FilterExpressionOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
2. See [:material-code-braces: DatetimeOptionsTypeDef](./type_defs.md#datetimeoptionstypedef) 
3. See [:material-code-braces: FilterExpressionOutputTypeDef](./type_defs.md#filterexpressionoutputtypedef) 
## FormatOptionsOutputTypeDef

```python
# FormatOptionsOutputTypeDef definition

class FormatOptionsOutputTypeDef(TypedDict):
    Json: NotRequired[JsonOptionsTypeDef],  # (1)
    Excel: NotRequired[ExcelOptionsOutputTypeDef],  # (2)
    Csv: NotRequired[CsvOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: JsonOptionsTypeDef](./type_defs.md#jsonoptionstypedef) 
2. See [:material-code-braces: ExcelOptionsOutputTypeDef](./type_defs.md#exceloptionsoutputtypedef) 
3. See [:material-code-braces: CsvOptionsTypeDef](./type_defs.md#csvoptionstypedef) 
## ListDatasetsRequestPaginateTypeDef

```python
# ListDatasetsRequestPaginateTypeDef definition

class ListDatasetsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobRunsRequestPaginateTypeDef

```python
# ListJobRunsRequestPaginateTypeDef definition

class ListJobRunsRequestPaginateTypeDef(TypedDict):
    Name: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsRequestPaginateTypeDef

```python
# ListJobsRequestPaginateTypeDef definition

class ListJobsRequestPaginateTypeDef(TypedDict):
    DatasetName: NotRequired[str],
    ProjectName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsRequestPaginateTypeDef

```python
# ListProjectsRequestPaginateTypeDef definition

class ListProjectsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecipeVersionsRequestPaginateTypeDef

```python
# ListRecipeVersionsRequestPaginateTypeDef definition

class ListRecipeVersionsRequestPaginateTypeDef(TypedDict):
    Name: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecipesRequestPaginateTypeDef

```python
# ListRecipesRequestPaginateTypeDef definition

class ListRecipesRequestPaginateTypeDef(TypedDict):
    RecipeVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRulesetsRequestPaginateTypeDef

```python
# ListRulesetsRequestPaginateTypeDef definition

class ListRulesetsRequestPaginateTypeDef(TypedDict):
    TargetArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchedulesRequestPaginateTypeDef

```python
# ListSchedulesRequestPaginateTypeDef definition

class ListSchedulesRequestPaginateTypeDef(TypedDict):
    JobName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRulesetsResponseTypeDef

```python
# ListRulesetsResponseTypeDef definition

class ListRulesetsResponseTypeDef(TypedDict):
    Rulesets: List[RulesetItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RulesetItemTypeDef](./type_defs.md#rulesetitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSchedulesResponseTypeDef

```python
# ListSchedulesResponseTypeDef definition

class ListSchedulesResponseTypeDef(TypedDict):
    Schedules: List[ScheduleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecipeStepOutputTypeDef

```python
# RecipeStepOutputTypeDef definition

class RecipeStepOutputTypeDef(TypedDict):
    Action: RecipeActionOutputTypeDef,  # (1)
    ConditionExpressions: NotRequired[List[ConditionExpressionTypeDef]],  # (2)
```

1. See [:material-code-braces: RecipeActionOutputTypeDef](./type_defs.md#recipeactionoutputtypedef) 
2. See [:material-code-braces: ConditionExpressionTypeDef](./type_defs.md#conditionexpressiontypedef) 
## RuleOutputTypeDef

```python
# RuleOutputTypeDef definition

class RuleOutputTypeDef(TypedDict):
    Name: str,
    CheckExpression: str,
    Disabled: NotRequired[bool],
    SubstitutionMap: NotRequired[Dict[str, str]],
    Threshold: NotRequired[ThresholdTypeDef],  # (1)
    ColumnSelectors: NotRequired[List[ColumnSelectorTypeDef]],  # (2)
```

1. See [:material-code-braces: ThresholdTypeDef](./type_defs.md#thresholdtypedef) 
2. See [:material-code-braces: ColumnSelectorTypeDef](./type_defs.md#columnselectortypedef) 
## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    Name: str,
    CheckExpression: str,
    Disabled: NotRequired[bool],
    SubstitutionMap: NotRequired[Mapping[str, str]],
    Threshold: NotRequired[ThresholdTypeDef],  # (1)
    ColumnSelectors: NotRequired[Sequence[ColumnSelectorTypeDef]],  # (2)
```

1. See [:material-code-braces: ThresholdTypeDef](./type_defs.md#thresholdtypedef) 
2. See [:material-code-braces: ColumnSelectorTypeDef](./type_defs.md#columnselectortypedef) 
## StatisticsConfigurationOutputTypeDef

```python
# StatisticsConfigurationOutputTypeDef definition

class StatisticsConfigurationOutputTypeDef(TypedDict):
    IncludedStatistics: NotRequired[List[str]],
    Overrides: NotRequired[List[StatisticOverrideOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: StatisticOverrideOutputTypeDef](./type_defs.md#statisticoverrideoutputtypedef) 
## EntityDetectorConfigurationTypeDef

```python
# EntityDetectorConfigurationTypeDef definition

class EntityDetectorConfigurationTypeDef(TypedDict):
    EntityTypes: Sequence[str],
    AllowedStatistics: NotRequired[Sequence[AllowedStatisticsUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: AllowedStatisticsTypeDef](./type_defs.md#allowedstatisticstypedef) [:material-code-braces: AllowedStatisticsOutputTypeDef](./type_defs.md#allowedstatisticsoutputtypedef) 
## InputTypeDef

```python
# InputTypeDef definition

class InputTypeDef(TypedDict):
    S3InputDefinition: NotRequired[S3LocationTypeDef],  # (1)
    DataCatalogInputDefinition: NotRequired[DataCatalogInputDefinitionTypeDef],  # (2)
    DatabaseInputDefinition: NotRequired[DatabaseInputDefinitionTypeDef],  # (3)
    Metadata: NotRequired[MetadataTypeDef],  # (4)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: DataCatalogInputDefinitionTypeDef](./type_defs.md#datacataloginputdefinitiontypedef) 
3. See [:material-code-braces: DatabaseInputDefinitionTypeDef](./type_defs.md#databaseinputdefinitiontypedef) 
4. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
## DatabaseOutputTypeDef

```python
# DatabaseOutputTypeDef definition

class DatabaseOutputTypeDef(TypedDict):
    GlueConnectionName: str,
    DatabaseOptions: DatabaseTableOutputOptionsTypeDef,  # (1)
    DatabaseOutputMode: NotRequired[DatabaseOutputModeType],  # (2)
```

1. See [:material-code-braces: DatabaseTableOutputOptionsTypeDef](./type_defs.md#databasetableoutputoptionstypedef) 
2. See [:material-code-brackets: DatabaseOutputModeType](./literals.md#databaseoutputmodetype) 
## DataCatalogOutputTypeDef

```python
# DataCatalogOutputTypeDef definition

class DataCatalogOutputTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    S3Options: NotRequired[S3TableOutputOptionsTypeDef],  # (1)
    DatabaseOptions: NotRequired[DatabaseTableOutputOptionsTypeDef],  # (2)
    Overwrite: NotRequired[bool],
```

1. See [:material-code-braces: S3TableOutputOptionsTypeDef](./type_defs.md#s3tableoutputoptionstypedef) 
2. See [:material-code-braces: DatabaseTableOutputOptionsTypeDef](./type_defs.md#databasetableoutputoptionstypedef) 
## ListProjectsResponseTypeDef

```python
# ListProjectsResponseTypeDef definition

class ListProjectsResponseTypeDef(TypedDict):
    Projects: List[ProjectTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExtraOutputTypeDef

```python
# ExtraOutputTypeDef definition

class ExtraOutputTypeDef(TypedDict):
    Location: S3LocationTypeDef,  # (3)
    CompressionFormat: NotRequired[CompressionFormatType],  # (1)
    Format: NotRequired[OutputFormatType],  # (2)
    PartitionColumns: NotRequired[List[str]],
    Overwrite: NotRequired[bool],
    FormatOptions: NotRequired[OutputFormatOptionsTypeDef],  # (4)
    MaxOutputFiles: NotRequired[int],
```

1. See [:material-code-brackets: CompressionFormatType](./literals.md#compressionformattype) 
2. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: OutputFormatOptionsTypeDef](./type_defs.md#outputformatoptionstypedef) 
## OutputTypeDef

```python
# OutputTypeDef definition

class OutputTypeDef(TypedDict):
    Location: S3LocationTypeDef,  # (3)
    CompressionFormat: NotRequired[CompressionFormatType],  # (1)
    Format: NotRequired[OutputFormatType],  # (2)
    PartitionColumns: NotRequired[Sequence[str]],
    Overwrite: NotRequired[bool],
    FormatOptions: NotRequired[OutputFormatOptionsTypeDef],  # (4)
    MaxOutputFiles: NotRequired[int],
```

1. See [:material-code-brackets: CompressionFormatType](./literals.md#compressionformattype) 
2. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: OutputFormatOptionsTypeDef](./type_defs.md#outputformatoptionstypedef) 
## PathOptionsOutputTypeDef

```python
# PathOptionsOutputTypeDef definition

class PathOptionsOutputTypeDef(TypedDict):
    LastModifiedDateCondition: NotRequired[FilterExpressionOutputTypeDef],  # (1)
    FilesLimit: NotRequired[FilesLimitTypeDef],  # (2)
    Parameters: NotRequired[Dict[str, DatasetParameterOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: FilterExpressionOutputTypeDef](./type_defs.md#filterexpressionoutputtypedef) 
2. See [:material-code-braces: FilesLimitTypeDef](./type_defs.md#fileslimittypedef) 
3. See [:material-code-braces: DatasetParameterOutputTypeDef](./type_defs.md#datasetparameteroutputtypedef) 
## FormatOptionsTypeDef

```python
# FormatOptionsTypeDef definition

class FormatOptionsTypeDef(TypedDict):
    Json: NotRequired[JsonOptionsTypeDef],  # (1)
    Excel: NotRequired[ExcelOptionsUnionTypeDef],  # (2)
    Csv: NotRequired[CsvOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: JsonOptionsTypeDef](./type_defs.md#jsonoptionstypedef) 
2. See [:material-code-braces: ExcelOptionsTypeDef](./type_defs.md#exceloptionstypedef) [:material-code-braces: ExcelOptionsOutputTypeDef](./type_defs.md#exceloptionsoutputtypedef) 
3. See [:material-code-braces: CsvOptionsTypeDef](./type_defs.md#csvoptionstypedef) 
## DatasetParameterTypeDef

```python
# DatasetParameterTypeDef definition

class DatasetParameterTypeDef(TypedDict):
    Name: str,
    Type: ParameterTypeType,  # (1)
    DatetimeOptions: NotRequired[DatetimeOptionsTypeDef],  # (2)
    CreateColumn: NotRequired[bool],
    Filter: NotRequired[FilterExpressionUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
2. See [:material-code-braces: DatetimeOptionsTypeDef](./type_defs.md#datetimeoptionstypedef) 
3. See [:material-code-braces: FilterExpressionTypeDef](./type_defs.md#filterexpressiontypedef) [:material-code-braces: FilterExpressionOutputTypeDef](./type_defs.md#filterexpressionoutputtypedef) 
## DescribeRecipeResponseTypeDef

```python
# DescribeRecipeResponseTypeDef definition

class DescribeRecipeResponseTypeDef(TypedDict):
    CreatedBy: str,
    CreateDate: datetime,
    LastModifiedBy: str,
    LastModifiedDate: datetime,
    ProjectName: str,
    PublishedBy: str,
    PublishedDate: datetime,
    Description: str,
    Name: str,
    Steps: List[RecipeStepOutputTypeDef],  # (1)
    Tags: Dict[str, str],
    ResourceArn: str,
    RecipeVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecipeStepOutputTypeDef](./type_defs.md#recipestepoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecipeTypeDef

```python
# RecipeTypeDef definition

class RecipeTypeDef(TypedDict):
    Name: str,
    CreatedBy: NotRequired[str],
    CreateDate: NotRequired[datetime],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    ProjectName: NotRequired[str],
    PublishedBy: NotRequired[str],
    PublishedDate: NotRequired[datetime],
    Description: NotRequired[str],
    ResourceArn: NotRequired[str],
    Steps: NotRequired[List[RecipeStepOutputTypeDef]],  # (1)
    Tags: NotRequired[Dict[str, str]],
    RecipeVersion: NotRequired[str],
```

1. See [:material-code-braces: RecipeStepOutputTypeDef](./type_defs.md#recipestepoutputtypedef) 
## RecipeStepTypeDef

```python
# RecipeStepTypeDef definition

class RecipeStepTypeDef(TypedDict):
    Action: RecipeActionUnionTypeDef,  # (1)
    ConditionExpressions: NotRequired[Sequence[ConditionExpressionTypeDef]],  # (2)
```

1. See [:material-code-braces: RecipeActionTypeDef](./type_defs.md#recipeactiontypedef) [:material-code-braces: RecipeActionOutputTypeDef](./type_defs.md#recipeactionoutputtypedef) 
2. See [:material-code-braces: ConditionExpressionTypeDef](./type_defs.md#conditionexpressiontypedef) 
## DescribeRulesetResponseTypeDef

```python
# DescribeRulesetResponseTypeDef definition

class DescribeRulesetResponseTypeDef(TypedDict):
    Name: str,
    Description: str,
    TargetArn: str,
    Rules: List[RuleOutputTypeDef],  # (1)
    CreateDate: datetime,
    CreatedBy: str,
    LastModifiedBy: str,
    LastModifiedDate: datetime,
    ResourceArn: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRulesetRequestRequestTypeDef

```python
# UpdateRulesetRequestRequestTypeDef definition

class UpdateRulesetRequestRequestTypeDef(TypedDict):
    Name: str,
    Rules: Sequence[RuleTypeDef],  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
## ColumnStatisticsConfigurationOutputTypeDef

```python
# ColumnStatisticsConfigurationOutputTypeDef definition

class ColumnStatisticsConfigurationOutputTypeDef(TypedDict):
    Statistics: StatisticsConfigurationOutputTypeDef,  # (2)
    Selectors: NotRequired[List[ColumnSelectorTypeDef]],  # (1)
```

1. See [:material-code-braces: ColumnSelectorTypeDef](./type_defs.md#columnselectortypedef) 
2. See [:material-code-braces: StatisticsConfigurationOutputTypeDef](./type_defs.md#statisticsconfigurationoutputtypedef) 
## StatisticsConfigurationTypeDef

```python
# StatisticsConfigurationTypeDef definition

class StatisticsConfigurationTypeDef(TypedDict):
    IncludedStatistics: NotRequired[Sequence[str]],
    Overrides: NotRequired[Sequence[StatisticOverrideUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: StatisticOverrideTypeDef](./type_defs.md#statisticoverridetypedef) [:material-code-braces: StatisticOverrideOutputTypeDef](./type_defs.md#statisticoverrideoutputtypedef) 
## JobRunTypeDef

```python
# JobRunTypeDef definition

class JobRunTypeDef(TypedDict):
    Attempt: NotRequired[int],
    CompletedOn: NotRequired[datetime],
    DatasetName: NotRequired[str],
    ErrorMessage: NotRequired[str],
    ExecutionTime: NotRequired[int],
    JobName: NotRequired[str],
    RunId: NotRequired[str],
    State: NotRequired[JobRunStateType],  # (1)
    LogSubscription: NotRequired[LogSubscriptionType],  # (2)
    LogGroupName: NotRequired[str],
    Outputs: NotRequired[List[ExtraOutputTypeDef]],  # (3)
    DataCatalogOutputs: NotRequired[List[DataCatalogOutputTypeDef]],  # (4)
    DatabaseOutputs: NotRequired[List[DatabaseOutputTypeDef]],  # (5)
    RecipeReference: NotRequired[RecipeReferenceTypeDef],  # (6)
    StartedBy: NotRequired[str],
    StartedOn: NotRequired[datetime],
    JobSample: NotRequired[JobSampleTypeDef],  # (7)
    ValidationConfigurations: NotRequired[List[ValidationConfigurationTypeDef]],  # (8)
```

1. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
2. See [:material-code-brackets: LogSubscriptionType](./literals.md#logsubscriptiontype) 
3. See [:material-code-braces: ExtraOutputTypeDef](./type_defs.md#extraoutputtypedef) 
4. See [:material-code-braces: DataCatalogOutputTypeDef](./type_defs.md#datacatalogoutputtypedef) 
5. See [:material-code-braces: DatabaseOutputTypeDef](./type_defs.md#databaseoutputtypedef) 
6. See [:material-code-braces: RecipeReferenceTypeDef](./type_defs.md#recipereferencetypedef) 
7. See [:material-code-braces: JobSampleTypeDef](./type_defs.md#jobsampletypedef) 
8. See [:material-code-braces: ValidationConfigurationTypeDef](./type_defs.md#validationconfigurationtypedef) 
## JobTypeDef

```python
# JobTypeDef definition

class JobTypeDef(TypedDict):
    Name: str,
    AccountId: NotRequired[str],
    CreatedBy: NotRequired[str],
    CreateDate: NotRequired[datetime],
    DatasetName: NotRequired[str],
    EncryptionKeyArn: NotRequired[str],
    EncryptionMode: NotRequired[EncryptionModeType],  # (1)
    Type: NotRequired[JobTypeType],  # (2)
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    LogSubscription: NotRequired[LogSubscriptionType],  # (3)
    MaxCapacity: NotRequired[int],
    MaxRetries: NotRequired[int],
    Outputs: NotRequired[List[ExtraOutputTypeDef]],  # (4)
    DataCatalogOutputs: NotRequired[List[DataCatalogOutputTypeDef]],  # (5)
    DatabaseOutputs: NotRequired[List[DatabaseOutputTypeDef]],  # (6)
    ProjectName: NotRequired[str],
    RecipeReference: NotRequired[RecipeReferenceTypeDef],  # (7)
    ResourceArn: NotRequired[str],
    RoleArn: NotRequired[str],
    Timeout: NotRequired[int],
    Tags: NotRequired[Dict[str, str]],
    JobSample: NotRequired[JobSampleTypeDef],  # (8)
    ValidationConfigurations: NotRequired[List[ValidationConfigurationTypeDef]],  # (9)
```

1. See [:material-code-brackets: EncryptionModeType](./literals.md#encryptionmodetype) 
2. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
3. See [:material-code-brackets: LogSubscriptionType](./literals.md#logsubscriptiontype) 
4. See [:material-code-braces: ExtraOutputTypeDef](./type_defs.md#extraoutputtypedef) 
5. See [:material-code-braces: DataCatalogOutputTypeDef](./type_defs.md#datacatalogoutputtypedef) 
6. See [:material-code-braces: DatabaseOutputTypeDef](./type_defs.md#databaseoutputtypedef) 
7. See [:material-code-braces: RecipeReferenceTypeDef](./type_defs.md#recipereferencetypedef) 
8. See [:material-code-braces: JobSampleTypeDef](./type_defs.md#jobsampletypedef) 
9. See [:material-code-braces: ValidationConfigurationTypeDef](./type_defs.md#validationconfigurationtypedef) 
## UpdateRecipeJobRequestRequestTypeDef

```python
# UpdateRecipeJobRequestRequestTypeDef definition

class UpdateRecipeJobRequestRequestTypeDef(TypedDict):
    Name: str,
    RoleArn: str,
    EncryptionKeyArn: NotRequired[str],
    EncryptionMode: NotRequired[EncryptionModeType],  # (1)
    LogSubscription: NotRequired[LogSubscriptionType],  # (2)
    MaxCapacity: NotRequired[int],
    MaxRetries: NotRequired[int],
    Outputs: NotRequired[Sequence[OutputTypeDef]],  # (3)
    DataCatalogOutputs: NotRequired[Sequence[DataCatalogOutputTypeDef]],  # (4)
    DatabaseOutputs: NotRequired[Sequence[DatabaseOutputTypeDef]],  # (5)
    Timeout: NotRequired[int],
```

1. See [:material-code-brackets: EncryptionModeType](./literals.md#encryptionmodetype) 
2. See [:material-code-brackets: LogSubscriptionType](./literals.md#logsubscriptiontype) 
3. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
4. See [:material-code-braces: DataCatalogOutputTypeDef](./type_defs.md#datacatalogoutputtypedef) 
5. See [:material-code-braces: DatabaseOutputTypeDef](./type_defs.md#databaseoutputtypedef) 
## DatasetTypeDef

```python
# DatasetTypeDef definition

class DatasetTypeDef(TypedDict):
    Name: str,
    Input: InputTypeDef,  # (3)
    AccountId: NotRequired[str],
    CreatedBy: NotRequired[str],
    CreateDate: NotRequired[datetime],
    Format: NotRequired[InputFormatType],  # (1)
    FormatOptions: NotRequired[FormatOptionsOutputTypeDef],  # (2)
    LastModifiedDate: NotRequired[datetime],
    LastModifiedBy: NotRequired[str],
    Source: NotRequired[SourceType],  # (4)
    PathOptions: NotRequired[PathOptionsOutputTypeDef],  # (5)
    Tags: NotRequired[Dict[str, str]],
    ResourceArn: NotRequired[str],
```

1. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
2. See [:material-code-braces: FormatOptionsOutputTypeDef](./type_defs.md#formatoptionsoutputtypedef) 
3. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
4. See [:material-code-brackets: SourceType](./literals.md#sourcetype) 
5. See [:material-code-braces: PathOptionsOutputTypeDef](./type_defs.md#pathoptionsoutputtypedef) 
## DescribeDatasetResponseTypeDef

```python
# DescribeDatasetResponseTypeDef definition

class DescribeDatasetResponseTypeDef(TypedDict):
    CreatedBy: str,
    CreateDate: datetime,
    Name: str,
    Format: InputFormatType,  # (1)
    FormatOptions: FormatOptionsOutputTypeDef,  # (2)
    Input: InputTypeDef,  # (3)
    LastModifiedDate: datetime,
    LastModifiedBy: str,
    Source: SourceType,  # (4)
    PathOptions: PathOptionsOutputTypeDef,  # (5)
    Tags: Dict[str, str],
    ResourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
2. See [:material-code-braces: FormatOptionsOutputTypeDef](./type_defs.md#formatoptionsoutputtypedef) 
3. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
4. See [:material-code-brackets: SourceType](./literals.md#sourcetype) 
5. See [:material-code-braces: PathOptionsOutputTypeDef](./type_defs.md#pathoptionsoutputtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecipeVersionsResponseTypeDef

```python
# ListRecipeVersionsResponseTypeDef definition

class ListRecipeVersionsResponseTypeDef(TypedDict):
    Recipes: List[RecipeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RecipeTypeDef](./type_defs.md#recipetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecipesResponseTypeDef

```python
# ListRecipesResponseTypeDef definition

class ListRecipesResponseTypeDef(TypedDict):
    Recipes: List[RecipeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RecipeTypeDef](./type_defs.md#recipetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendProjectSessionActionRequestRequestTypeDef

```python
# SendProjectSessionActionRequestRequestTypeDef definition

class SendProjectSessionActionRequestRequestTypeDef(TypedDict):
    Name: str,
    Preview: NotRequired[bool],
    RecipeStep: NotRequired[RecipeStepTypeDef],  # (1)
    StepIndex: NotRequired[int],
    ClientSessionId: NotRequired[str],
    ViewFrame: NotRequired[ViewFrameTypeDef],  # (2)
```

1. See [:material-code-braces: RecipeStepTypeDef](./type_defs.md#recipesteptypedef) 
2. See [:material-code-braces: ViewFrameTypeDef](./type_defs.md#viewframetypedef) 
## UpdateRecipeRequestRequestTypeDef

```python
# UpdateRecipeRequestRequestTypeDef definition

class UpdateRecipeRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    Steps: NotRequired[Sequence[RecipeStepTypeDef]],  # (1)
```

1. See [:material-code-braces: RecipeStepTypeDef](./type_defs.md#recipesteptypedef) 
## CreateRulesetRequestRequestTypeDef

```python
# CreateRulesetRequestRequestTypeDef definition

class CreateRulesetRequestRequestTypeDef(TypedDict):
    Name: str,
    TargetArn: str,
    Rules: Sequence[RuleUnionTypeDef],  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
## ProfileConfigurationOutputTypeDef

```python
# ProfileConfigurationOutputTypeDef definition

class ProfileConfigurationOutputTypeDef(TypedDict):
    DatasetStatisticsConfiguration: NotRequired[StatisticsConfigurationOutputTypeDef],  # (1)
    ProfileColumns: NotRequired[List[ColumnSelectorTypeDef]],  # (2)
    ColumnStatisticsConfigurations: NotRequired[List[ColumnStatisticsConfigurationOutputTypeDef]],  # (3)
    EntityDetectorConfiguration: NotRequired[EntityDetectorConfigurationOutputTypeDef],  # (4)
```

1. See [:material-code-braces: StatisticsConfigurationOutputTypeDef](./type_defs.md#statisticsconfigurationoutputtypedef) 
2. See [:material-code-braces: ColumnSelectorTypeDef](./type_defs.md#columnselectortypedef) 
3. See [:material-code-braces: ColumnStatisticsConfigurationOutputTypeDef](./type_defs.md#columnstatisticsconfigurationoutputtypedef) 
4. See [:material-code-braces: EntityDetectorConfigurationOutputTypeDef](./type_defs.md#entitydetectorconfigurationoutputtypedef) 
## ListJobRunsResponseTypeDef

```python
# ListJobRunsResponseTypeDef definition

class ListJobRunsResponseTypeDef(TypedDict):
    JobRuns: List[JobRunTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JobRunTypeDef](./type_defs.md#jobruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobsResponseTypeDef

```python
# ListJobsResponseTypeDef definition

class ListJobsResponseTypeDef(TypedDict):
    Jobs: List[JobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRecipeJobRequestRequestTypeDef

```python
# CreateRecipeJobRequestRequestTypeDef definition

class CreateRecipeJobRequestRequestTypeDef(TypedDict):
    Name: str,
    RoleArn: str,
    DatasetName: NotRequired[str],
    EncryptionKeyArn: NotRequired[str],
    EncryptionMode: NotRequired[EncryptionModeType],  # (1)
    LogSubscription: NotRequired[LogSubscriptionType],  # (2)
    MaxCapacity: NotRequired[int],
    MaxRetries: NotRequired[int],
    Outputs: NotRequired[Sequence[UnionTypeDef]],  # (3)
    DataCatalogOutputs: NotRequired[Sequence[DataCatalogOutputTypeDef]],  # (4)
    DatabaseOutputs: NotRequired[Sequence[DatabaseOutputTypeDef]],  # (5)
    ProjectName: NotRequired[str],
    RecipeReference: NotRequired[RecipeReferenceTypeDef],  # (6)
    Tags: NotRequired[Mapping[str, str]],
    Timeout: NotRequired[int],
```

1. See [:material-code-brackets: EncryptionModeType](./literals.md#encryptionmodetype) 
2. See [:material-code-brackets: LogSubscriptionType](./literals.md#logsubscriptiontype) 
3. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) [:material-code-braces: ExtraOutputTypeDef](./type_defs.md#extraoutputtypedef) 
4. See [:material-code-braces: DataCatalogOutputTypeDef](./type_defs.md#datacatalogoutputtypedef) 
5. See [:material-code-braces: DatabaseOutputTypeDef](./type_defs.md#databaseoutputtypedef) 
6. See [:material-code-braces: RecipeReferenceTypeDef](./type_defs.md#recipereferencetypedef) 
## ListDatasetsResponseTypeDef

```python
# ListDatasetsResponseTypeDef definition

class ListDatasetsResponseTypeDef(TypedDict):
    Datasets: List[DatasetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PathOptionsTypeDef

```python
# PathOptionsTypeDef definition

class PathOptionsTypeDef(TypedDict):
    LastModifiedDateCondition: NotRequired[FilterExpressionUnionTypeDef],  # (1)
    FilesLimit: NotRequired[FilesLimitTypeDef],  # (2)
    Parameters: NotRequired[Mapping[str, DatasetParameterUnionTypeDef]],  # (3)
```

1. See [:material-code-braces: FilterExpressionTypeDef](./type_defs.md#filterexpressiontypedef) [:material-code-braces: FilterExpressionOutputTypeDef](./type_defs.md#filterexpressionoutputtypedef) 
2. See [:material-code-braces: FilesLimitTypeDef](./type_defs.md#fileslimittypedef) 
3. See [:material-code-braces: DatasetParameterTypeDef](./type_defs.md#datasetparametertypedef) [:material-code-braces: DatasetParameterOutputTypeDef](./type_defs.md#datasetparameteroutputtypedef) 
## CreateRecipeRequestRequestTypeDef

```python
# CreateRecipeRequestRequestTypeDef definition

class CreateRecipeRequestRequestTypeDef(TypedDict):
    Name: str,
    Steps: Sequence[RecipeStepUnionTypeDef],  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: RecipeStepTypeDef](./type_defs.md#recipesteptypedef) [:material-code-braces: RecipeStepOutputTypeDef](./type_defs.md#recipestepoutputtypedef) 
## DescribeJobResponseTypeDef

```python
# DescribeJobResponseTypeDef definition

class DescribeJobResponseTypeDef(TypedDict):
    CreateDate: datetime,
    CreatedBy: str,
    DatasetName: str,
    EncryptionKeyArn: str,
    EncryptionMode: EncryptionModeType,  # (1)
    Name: str,
    Type: JobTypeType,  # (2)
    LastModifiedBy: str,
    LastModifiedDate: datetime,
    LogSubscription: LogSubscriptionType,  # (3)
    MaxCapacity: int,
    MaxRetries: int,
    Outputs: List[ExtraOutputTypeDef],  # (4)
    DataCatalogOutputs: List[DataCatalogOutputTypeDef],  # (5)
    DatabaseOutputs: List[DatabaseOutputTypeDef],  # (6)
    ProjectName: str,
    ProfileConfiguration: ProfileConfigurationOutputTypeDef,  # (7)
    ValidationConfigurations: List[ValidationConfigurationTypeDef],  # (8)
    RecipeReference: RecipeReferenceTypeDef,  # (9)
    ResourceArn: str,
    RoleArn: str,
    Tags: Dict[str, str],
    Timeout: int,
    JobSample: JobSampleTypeDef,  # (10)
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-brackets: EncryptionModeType](./literals.md#encryptionmodetype) 
2. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
3. See [:material-code-brackets: LogSubscriptionType](./literals.md#logsubscriptiontype) 
4. See [:material-code-braces: ExtraOutputTypeDef](./type_defs.md#extraoutputtypedef) 
5. See [:material-code-braces: DataCatalogOutputTypeDef](./type_defs.md#datacatalogoutputtypedef) 
6. See [:material-code-braces: DatabaseOutputTypeDef](./type_defs.md#databaseoutputtypedef) 
7. See [:material-code-braces: ProfileConfigurationOutputTypeDef](./type_defs.md#profileconfigurationoutputtypedef) 
8. See [:material-code-braces: ValidationConfigurationTypeDef](./type_defs.md#validationconfigurationtypedef) 
9. See [:material-code-braces: RecipeReferenceTypeDef](./type_defs.md#recipereferencetypedef) 
10. See [:material-code-braces: JobSampleTypeDef](./type_defs.md#jobsampletypedef) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeJobRunResponseTypeDef

```python
# DescribeJobRunResponseTypeDef definition

class DescribeJobRunResponseTypeDef(TypedDict):
    Attempt: int,
    CompletedOn: datetime,
    DatasetName: str,
    ErrorMessage: str,
    ExecutionTime: int,
    JobName: str,
    ProfileConfiguration: ProfileConfigurationOutputTypeDef,  # (1)
    ValidationConfigurations: List[ValidationConfigurationTypeDef],  # (2)
    RunId: str,
    State: JobRunStateType,  # (3)
    LogSubscription: LogSubscriptionType,  # (4)
    LogGroupName: str,
    Outputs: List[ExtraOutputTypeDef],  # (5)
    DataCatalogOutputs: List[DataCatalogOutputTypeDef],  # (6)
    DatabaseOutputs: List[DatabaseOutputTypeDef],  # (7)
    RecipeReference: RecipeReferenceTypeDef,  # (8)
    StartedBy: str,
    StartedOn: datetime,
    JobSample: JobSampleTypeDef,  # (9)
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-braces: ProfileConfigurationOutputTypeDef](./type_defs.md#profileconfigurationoutputtypedef) 
2. See [:material-code-braces: ValidationConfigurationTypeDef](./type_defs.md#validationconfigurationtypedef) 
3. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
4. See [:material-code-brackets: LogSubscriptionType](./literals.md#logsubscriptiontype) 
5. See [:material-code-braces: ExtraOutputTypeDef](./type_defs.md#extraoutputtypedef) 
6. See [:material-code-braces: DataCatalogOutputTypeDef](./type_defs.md#datacatalogoutputtypedef) 
7. See [:material-code-braces: DatabaseOutputTypeDef](./type_defs.md#databaseoutputtypedef) 
8. See [:material-code-braces: RecipeReferenceTypeDef](./type_defs.md#recipereferencetypedef) 
9. See [:material-code-braces: JobSampleTypeDef](./type_defs.md#jobsampletypedef) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ColumnStatisticsConfigurationTypeDef

```python
# ColumnStatisticsConfigurationTypeDef definition

class ColumnStatisticsConfigurationTypeDef(TypedDict):
    Statistics: StatisticsConfigurationUnionTypeDef,  # (2)
    Selectors: NotRequired[Sequence[ColumnSelectorTypeDef]],  # (1)
```

1. See [:material-code-braces: ColumnSelectorTypeDef](./type_defs.md#columnselectortypedef) 
2. See [:material-code-braces: StatisticsConfigurationTypeDef](./type_defs.md#statisticsconfigurationtypedef) [:material-code-braces: StatisticsConfigurationOutputTypeDef](./type_defs.md#statisticsconfigurationoutputtypedef) 
## CreateDatasetRequestRequestTypeDef

```python
# CreateDatasetRequestRequestTypeDef definition

class CreateDatasetRequestRequestTypeDef(TypedDict):
    Name: str,
    Input: InputTypeDef,  # (1)
    Format: NotRequired[InputFormatType],  # (2)
    FormatOptions: NotRequired[FormatOptionsTypeDef],  # (3)
    PathOptions: NotRequired[PathOptionsTypeDef],  # (4)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
2. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
3. See [:material-code-braces: FormatOptionsTypeDef](./type_defs.md#formatoptionstypedef) 
4. See [:material-code-braces: PathOptionsTypeDef](./type_defs.md#pathoptionstypedef) 
## UpdateDatasetRequestRequestTypeDef

```python
# UpdateDatasetRequestRequestTypeDef definition

class UpdateDatasetRequestRequestTypeDef(TypedDict):
    Name: str,
    Input: InputTypeDef,  # (1)
    Format: NotRequired[InputFormatType],  # (2)
    FormatOptions: NotRequired[FormatOptionsTypeDef],  # (3)
    PathOptions: NotRequired[PathOptionsTypeDef],  # (4)
```

1. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
2. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
3. See [:material-code-braces: FormatOptionsTypeDef](./type_defs.md#formatoptionstypedef) 
4. See [:material-code-braces: PathOptionsTypeDef](./type_defs.md#pathoptionstypedef) 
## ProfileConfigurationTypeDef

```python
# ProfileConfigurationTypeDef definition

class ProfileConfigurationTypeDef(TypedDict):
    DatasetStatisticsConfiguration: NotRequired[StatisticsConfigurationUnionTypeDef],  # (1)
    ProfileColumns: NotRequired[Sequence[ColumnSelectorTypeDef]],  # (2)
    ColumnStatisticsConfigurations: NotRequired[Sequence[ColumnStatisticsConfigurationUnionTypeDef]],  # (3)
    EntityDetectorConfiguration: NotRequired[EntityDetectorConfigurationUnionTypeDef],  # (4)
```

1. See [:material-code-braces: StatisticsConfigurationTypeDef](./type_defs.md#statisticsconfigurationtypedef) [:material-code-braces: StatisticsConfigurationOutputTypeDef](./type_defs.md#statisticsconfigurationoutputtypedef) 
2. See [:material-code-braces: ColumnSelectorTypeDef](./type_defs.md#columnselectortypedef) 
3. See [:material-code-braces: ColumnStatisticsConfigurationTypeDef](./type_defs.md#columnstatisticsconfigurationtypedef) [:material-code-braces: ColumnStatisticsConfigurationOutputTypeDef](./type_defs.md#columnstatisticsconfigurationoutputtypedef) 
4. See [:material-code-braces: EntityDetectorConfigurationTypeDef](./type_defs.md#entitydetectorconfigurationtypedef) [:material-code-braces: EntityDetectorConfigurationOutputTypeDef](./type_defs.md#entitydetectorconfigurationoutputtypedef) 
## CreateProfileJobRequestRequestTypeDef

```python
# CreateProfileJobRequestRequestTypeDef definition

class CreateProfileJobRequestRequestTypeDef(TypedDict):
    DatasetName: str,
    Name: str,
    OutputLocation: S3LocationTypeDef,  # (1)
    RoleArn: str,
    EncryptionKeyArn: NotRequired[str],
    EncryptionMode: NotRequired[EncryptionModeType],  # (2)
    LogSubscription: NotRequired[LogSubscriptionType],  # (3)
    MaxCapacity: NotRequired[int],
    MaxRetries: NotRequired[int],
    Configuration: NotRequired[ProfileConfigurationTypeDef],  # (4)
    ValidationConfigurations: NotRequired[Sequence[ValidationConfigurationTypeDef]],  # (5)
    Tags: NotRequired[Mapping[str, str]],
    Timeout: NotRequired[int],
    JobSample: NotRequired[JobSampleTypeDef],  # (6)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-brackets: EncryptionModeType](./literals.md#encryptionmodetype) 
3. See [:material-code-brackets: LogSubscriptionType](./literals.md#logsubscriptiontype) 
4. See [:material-code-braces: ProfileConfigurationTypeDef](./type_defs.md#profileconfigurationtypedef) 
5. See [:material-code-braces: ValidationConfigurationTypeDef](./type_defs.md#validationconfigurationtypedef) 
6. See [:material-code-braces: JobSampleTypeDef](./type_defs.md#jobsampletypedef) 
## UpdateProfileJobRequestRequestTypeDef

```python
# UpdateProfileJobRequestRequestTypeDef definition

class UpdateProfileJobRequestRequestTypeDef(TypedDict):
    Name: str,
    OutputLocation: S3LocationTypeDef,  # (1)
    RoleArn: str,
    Configuration: NotRequired[ProfileConfigurationTypeDef],  # (2)
    EncryptionKeyArn: NotRequired[str],
    EncryptionMode: NotRequired[EncryptionModeType],  # (3)
    LogSubscription: NotRequired[LogSubscriptionType],  # (4)
    MaxCapacity: NotRequired[int],
    MaxRetries: NotRequired[int],
    ValidationConfigurations: NotRequired[Sequence[ValidationConfigurationTypeDef]],  # (5)
    Timeout: NotRequired[int],
    JobSample: NotRequired[JobSampleTypeDef],  # (6)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: ProfileConfigurationTypeDef](./type_defs.md#profileconfigurationtypedef) 
3. See [:material-code-brackets: EncryptionModeType](./literals.md#encryptionmodetype) 
4. See [:material-code-brackets: LogSubscriptionType](./literals.md#logsubscriptiontype) 
5. See [:material-code-braces: ValidationConfigurationTypeDef](./type_defs.md#validationconfigurationtypedef) 
6. See [:material-code-braces: JobSampleTypeDef](./type_defs.md#jobsampletypedef) 
