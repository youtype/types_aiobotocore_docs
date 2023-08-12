# Type definitions

> [Index](../README.md) > [QuickSight](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [QuickSight](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
    type annotations stubs module [types-aiobotocore-quicksight](https://pypi.org/project/types-aiobotocore-quicksight/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AccountCustomizationTypeDef

```python
# AccountCustomizationTypeDef definition

class AccountCustomizationTypeDef(TypedDict):
    DefaultTheme: NotRequired[str],
    DefaultEmailCustomizationTemplate: NotRequired[str],
```

## AccountInfoTypeDef

```python
# AccountInfoTypeDef definition

class AccountInfoTypeDef(TypedDict):
    AccountName: NotRequired[str],
    Edition: NotRequired[EditionType],  # (1)
    NotificationEmail: NotRequired[str],
    AuthenticationType: NotRequired[str],
    AccountSubscriptionStatus: NotRequired[str],
    IAMIdentityCenterInstanceArn: NotRequired[str],
```

1. See [:material-code-brackets: EditionType](./literals.md#editiontype) 
## AccountSettingsTypeDef

```python
# AccountSettingsTypeDef definition

class AccountSettingsTypeDef(TypedDict):
    AccountName: NotRequired[str],
    Edition: NotRequired[EditionType],  # (1)
    DefaultNamespace: NotRequired[str],
    NotificationEmail: NotRequired[str],
    PublicSharingEnabled: NotRequired[bool],
    TerminationProtectionEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: EditionType](./literals.md#editiontype) 
## ActiveIAMPolicyAssignmentTypeDef

```python
# ActiveIAMPolicyAssignmentTypeDef definition

class ActiveIAMPolicyAssignmentTypeDef(TypedDict):
    AssignmentName: NotRequired[str],
    PolicyArn: NotRequired[str],
```

## AdHocFilteringOptionTypeDef

```python
# AdHocFilteringOptionTypeDef definition

class AdHocFilteringOptionTypeDef(TypedDict):
    AvailabilityStatus: NotRequired[DashboardBehaviorType],  # (1)
```

1. See [:material-code-brackets: DashboardBehaviorType](./literals.md#dashboardbehaviortype) 
## AttributeAggregationFunctionTypeDef

```python
# AttributeAggregationFunctionTypeDef definition

class AttributeAggregationFunctionTypeDef(TypedDict):
    SimpleAttributeAggregation: NotRequired[SimpleAttributeAggregationFunctionType],  # (1)
    ValueForMultipleValues: NotRequired[str],
```

1. See [:material-code-brackets: SimpleAttributeAggregationFunctionType](./literals.md#simpleattributeaggregationfunctiontype) 
## ColumnIdentifierTypeDef

```python
# ColumnIdentifierTypeDef definition

class ColumnIdentifierTypeDef(TypedDict):
    DataSetIdentifier: str,
    ColumnName: str,
```

## AmazonElasticsearchParametersTypeDef

```python
# AmazonElasticsearchParametersTypeDef definition

class AmazonElasticsearchParametersTypeDef(TypedDict):
    Domain: str,
```

## AmazonOpenSearchParametersTypeDef

```python
# AmazonOpenSearchParametersTypeDef definition

class AmazonOpenSearchParametersTypeDef(TypedDict):
    Domain: str,
```

## CalculatedFieldTypeDef

```python
# CalculatedFieldTypeDef definition

class CalculatedFieldTypeDef(TypedDict):
    DataSetIdentifier: str,
    Name: str,
    Expression: str,
```

## DataSetIdentifierDeclarationTypeDef

```python
# DataSetIdentifierDeclarationTypeDef definition

class DataSetIdentifierDeclarationTypeDef(TypedDict):
    Identifier: str,
    DataSetArn: str,
```

## EntityTypeDef

```python
# EntityTypeDef definition

class EntityTypeDef(TypedDict):
    Path: NotRequired[str],
```

## AnalysisSearchFilterTypeDef

```python
# AnalysisSearchFilterTypeDef definition

class AnalysisSearchFilterTypeDef(TypedDict):
    Operator: NotRequired[FilterOperatorType],  # (1)
    Name: NotRequired[AnalysisFilterAttributeType],  # (2)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: FilterOperatorType](./literals.md#filteroperatortype) 
2. See [:material-code-brackets: AnalysisFilterAttributeType](./literals.md#analysisfilterattributetype) 
## DataSetReferenceTypeDef

```python
# DataSetReferenceTypeDef definition

class DataSetReferenceTypeDef(TypedDict):
    DataSetPlaceholder: str,
    DataSetArn: str,
```

## AnalysisSummaryTypeDef

```python
# AnalysisSummaryTypeDef definition

class AnalysisSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    AnalysisId: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[ResourceStatusType],  # (1)
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
## SheetTypeDef

```python
# SheetTypeDef definition

class SheetTypeDef(TypedDict):
    SheetId: NotRequired[str],
    Name: NotRequired[str],
```

## AnchorDateConfigurationTypeDef

```python
# AnchorDateConfigurationTypeDef definition

class AnchorDateConfigurationTypeDef(TypedDict):
    AnchorOption: NotRequired[AnchorOptionType],  # (1)
    ParameterName: NotRequired[str],
```

1. See [:material-code-brackets: AnchorOptionType](./literals.md#anchoroptiontype) 
## AnonymousUserDashboardEmbeddingConfigurationTypeDef

```python
# AnonymousUserDashboardEmbeddingConfigurationTypeDef definition

class AnonymousUserDashboardEmbeddingConfigurationTypeDef(TypedDict):
    InitialDashboardId: str,
```

## DashboardVisualIdTypeDef

```python
# DashboardVisualIdTypeDef definition

class DashboardVisualIdTypeDef(TypedDict):
    DashboardId: str,
    SheetId: str,
    VisualId: str,
```

## AnonymousUserQSearchBarEmbeddingConfigurationTypeDef

```python
# AnonymousUserQSearchBarEmbeddingConfigurationTypeDef definition

class AnonymousUserQSearchBarEmbeddingConfigurationTypeDef(TypedDict):
    InitialTopicId: str,
```

## ArcAxisDisplayRangeTypeDef

```python
# ArcAxisDisplayRangeTypeDef definition

class ArcAxisDisplayRangeTypeDef(TypedDict):
    Min: NotRequired[float],
    Max: NotRequired[float],
```

## ArcConfigurationTypeDef

```python
# ArcConfigurationTypeDef definition

class ArcConfigurationTypeDef(TypedDict):
    ArcAngle: NotRequired[float],
    ArcThickness: NotRequired[ArcThicknessOptionsType],  # (1)
```

1. See [:material-code-brackets: ArcThicknessOptionsType](./literals.md#arcthicknessoptionstype) 
## ArcOptionsTypeDef

```python
# ArcOptionsTypeDef definition

class ArcOptionsTypeDef(TypedDict):
    ArcThickness: NotRequired[ArcThicknessType],  # (1)
```

1. See [:material-code-brackets: ArcThicknessType](./literals.md#arcthicknesstype) 
## AssetBundleExportJobAnalysisOverridePropertiesTypeDef

```python
# AssetBundleExportJobAnalysisOverridePropertiesTypeDef definition

class AssetBundleExportJobAnalysisOverridePropertiesTypeDef(TypedDict):
    Properties: List[AssetBundleExportJobAnalysisPropertyToOverrideType],  # (1)
    Arn: NotRequired[str],
```

1. See [:material-code-brackets: AssetBundleExportJobAnalysisPropertyToOverrideType](./literals.md#assetbundleexportjobanalysispropertytooverridetype) 
## AssetBundleExportJobDashboardOverridePropertiesTypeDef

```python
# AssetBundleExportJobDashboardOverridePropertiesTypeDef definition

class AssetBundleExportJobDashboardOverridePropertiesTypeDef(TypedDict):
    Properties: List[AssetBundleExportJobDashboardPropertyToOverrideType],  # (1)
    Arn: NotRequired[str],
```

1. See [:material-code-brackets: AssetBundleExportJobDashboardPropertyToOverrideType](./literals.md#assetbundleexportjobdashboardpropertytooverridetype) 
## AssetBundleExportJobDataSetOverridePropertiesTypeDef

```python
# AssetBundleExportJobDataSetOverridePropertiesTypeDef definition

class AssetBundleExportJobDataSetOverridePropertiesTypeDef(TypedDict):
    Properties: List[AssetBundleExportJobDataSetPropertyToOverrideType],  # (1)
    Arn: NotRequired[str],
```

1. See [:material-code-brackets: AssetBundleExportJobDataSetPropertyToOverrideType](./literals.md#assetbundleexportjobdatasetpropertytooverridetype) 
## AssetBundleExportJobDataSourceOverridePropertiesTypeDef

```python
# AssetBundleExportJobDataSourceOverridePropertiesTypeDef definition

class AssetBundleExportJobDataSourceOverridePropertiesTypeDef(TypedDict):
    Properties: List[AssetBundleExportJobDataSourcePropertyToOverrideType],  # (1)
    Arn: NotRequired[str],
```

1. See [:material-code-brackets: AssetBundleExportJobDataSourcePropertyToOverrideType](./literals.md#assetbundleexportjobdatasourcepropertytooverridetype) 
## AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef

```python
# AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef definition

class AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef(TypedDict):
    Properties: List[AssetBundleExportJobRefreshSchedulePropertyToOverrideType],  # (1)
    Arn: NotRequired[str],
```

1. See [:material-code-brackets: AssetBundleExportJobRefreshSchedulePropertyToOverrideType](./literals.md#assetbundleexportjobrefreshschedulepropertytooverridetype) 
## AssetBundleExportJobResourceIdOverrideConfigurationTypeDef

```python
# AssetBundleExportJobResourceIdOverrideConfigurationTypeDef definition

class AssetBundleExportJobResourceIdOverrideConfigurationTypeDef(TypedDict):
    PrefixForAllResources: NotRequired[bool],
```

## AssetBundleExportJobThemeOverridePropertiesTypeDef

```python
# AssetBundleExportJobThemeOverridePropertiesTypeDef definition

class AssetBundleExportJobThemeOverridePropertiesTypeDef(TypedDict):
    Properties: List[AssetBundleExportJobThemePropertyToOverrideType],  # (1)
    Arn: NotRequired[str],
```

1. See [:material-code-brackets: AssetBundleExportJobThemePropertyToOverrideType](./literals.md#assetbundleexportjobthemepropertytooverridetype) 
## AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef

```python
# AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef definition

class AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef(TypedDict):
    Properties: List[AssetBundleExportJobVPCConnectionPropertyToOverrideType],  # (1)
    Arn: NotRequired[str],
```

1. See [:material-code-brackets: AssetBundleExportJobVPCConnectionPropertyToOverrideType](./literals.md#assetbundleexportjobvpcconnectionpropertytooverridetype) 
## AssetBundleExportJobErrorTypeDef

```python
# AssetBundleExportJobErrorTypeDef definition

class AssetBundleExportJobErrorTypeDef(TypedDict):
    Arn: NotRequired[str],
    Type: NotRequired[str],
    Message: NotRequired[str],
```

## AssetBundleExportJobSummaryTypeDef

```python
# AssetBundleExportJobSummaryTypeDef definition

class AssetBundleExportJobSummaryTypeDef(TypedDict):
    JobStatus: NotRequired[AssetBundleExportJobStatusType],  # (1)
    Arn: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    AssetBundleExportJobId: NotRequired[str],
    IncludeAllDependencies: NotRequired[bool],
    ExportFormat: NotRequired[AssetBundleExportFormatType],  # (2)
```

1. See [:material-code-brackets: AssetBundleExportJobStatusType](./literals.md#assetbundleexportjobstatustype) 
2. See [:material-code-brackets: AssetBundleExportFormatType](./literals.md#assetbundleexportformattype) 
## AssetBundleImportJobAnalysisOverrideParametersTypeDef

```python
# AssetBundleImportJobAnalysisOverrideParametersTypeDef definition

class AssetBundleImportJobAnalysisOverrideParametersTypeDef(TypedDict):
    AnalysisId: str,
    Name: NotRequired[str],
```

## AssetBundleImportJobDashboardOverrideParametersTypeDef

```python
# AssetBundleImportJobDashboardOverrideParametersTypeDef definition

class AssetBundleImportJobDashboardOverrideParametersTypeDef(TypedDict):
    DashboardId: str,
    Name: NotRequired[str],
```

## AssetBundleImportJobDataSetOverrideParametersTypeDef

```python
# AssetBundleImportJobDataSetOverrideParametersTypeDef definition

class AssetBundleImportJobDataSetOverrideParametersTypeDef(TypedDict):
    DataSetId: str,
    Name: NotRequired[str],
```

## AssetBundleImportJobDataSourceCredentialPairTypeDef

```python
# AssetBundleImportJobDataSourceCredentialPairTypeDef definition

class AssetBundleImportJobDataSourceCredentialPairTypeDef(TypedDict):
    Username: str,
    Password: str,
```

## SslPropertiesTypeDef

```python
# SslPropertiesTypeDef definition

class SslPropertiesTypeDef(TypedDict):
    DisableSsl: NotRequired[bool],
```

## VpcConnectionPropertiesTypeDef

```python
# VpcConnectionPropertiesTypeDef definition

class VpcConnectionPropertiesTypeDef(TypedDict):
    VpcConnectionArn: str,
```

## AssetBundleImportJobErrorTypeDef

```python
# AssetBundleImportJobErrorTypeDef definition

class AssetBundleImportJobErrorTypeDef(TypedDict):
    Arn: NotRequired[str],
    Type: NotRequired[str],
    Message: NotRequired[str],
```

## AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef

```python
# AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef definition

class AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef(TypedDict):
    DataSetId: str,
    ScheduleId: str,
    StartAfterDateTime: NotRequired[datetime],
```

## AssetBundleImportJobResourceIdOverrideConfigurationTypeDef

```python
# AssetBundleImportJobResourceIdOverrideConfigurationTypeDef definition

class AssetBundleImportJobResourceIdOverrideConfigurationTypeDef(TypedDict):
    PrefixForAllResources: NotRequired[str],
```

## AssetBundleImportJobThemeOverrideParametersTypeDef

```python
# AssetBundleImportJobThemeOverrideParametersTypeDef definition

class AssetBundleImportJobThemeOverrideParametersTypeDef(TypedDict):
    ThemeId: str,
    Name: NotRequired[str],
```

## AssetBundleImportJobVPCConnectionOverrideParametersTypeDef

```python
# AssetBundleImportJobVPCConnectionOverrideParametersTypeDef definition

class AssetBundleImportJobVPCConnectionOverrideParametersTypeDef(TypedDict):
    VPCConnectionId: str,
    Name: NotRequired[str],
    SubnetIds: NotRequired[List[str]],
    SecurityGroupIds: NotRequired[List[str]],
    DnsResolvers: NotRequired[List[str]],
    RoleArn: NotRequired[str],
```

## AssetBundleImportJobSummaryTypeDef

```python
# AssetBundleImportJobSummaryTypeDef definition

class AssetBundleImportJobSummaryTypeDef(TypedDict):
    JobStatus: NotRequired[AssetBundleImportJobStatusType],  # (1)
    Arn: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    AssetBundleImportJobId: NotRequired[str],
    FailureAction: NotRequired[AssetBundleImportFailureActionType],  # (2)
```

1. See [:material-code-brackets: AssetBundleImportJobStatusType](./literals.md#assetbundleimportjobstatustype) 
2. See [:material-code-brackets: AssetBundleImportFailureActionType](./literals.md#assetbundleimportfailureactiontype) 
## AssetBundleImportSourceDescriptionTypeDef

```python
# AssetBundleImportSourceDescriptionTypeDef definition

class AssetBundleImportSourceDescriptionTypeDef(TypedDict):
    Body: NotRequired[str],
    S3Uri: NotRequired[str],
```

## AthenaParametersTypeDef

```python
# AthenaParametersTypeDef definition

class AthenaParametersTypeDef(TypedDict):
    WorkGroup: NotRequired[str],
    RoleArn: NotRequired[str],
```

## AuroraParametersTypeDef

```python
# AuroraParametersTypeDef definition

class AuroraParametersTypeDef(TypedDict):
    Host: str,
    Port: int,
    Database: str,
```

## AuroraPostgreSqlParametersTypeDef

```python
# AuroraPostgreSqlParametersTypeDef definition

class AuroraPostgreSqlParametersTypeDef(TypedDict):
    Host: str,
    Port: int,
    Database: str,
```

## AwsIotAnalyticsParametersTypeDef

```python
# AwsIotAnalyticsParametersTypeDef definition

class AwsIotAnalyticsParametersTypeDef(TypedDict):
    DataSetName: str,
```

## DateAxisOptionsTypeDef

```python
# DateAxisOptionsTypeDef definition

class DateAxisOptionsTypeDef(TypedDict):
    MissingDateVisibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## AxisDisplayMinMaxRangeTypeDef

```python
# AxisDisplayMinMaxRangeTypeDef definition

class AxisDisplayMinMaxRangeTypeDef(TypedDict):
    Minimum: NotRequired[float],
    Maximum: NotRequired[float],
```

## AxisLinearScaleTypeDef

```python
# AxisLinearScaleTypeDef definition

class AxisLinearScaleTypeDef(TypedDict):
    StepCount: NotRequired[int],
    StepSize: NotRequired[float],
```

## AxisLogarithmicScaleTypeDef

```python
# AxisLogarithmicScaleTypeDef definition

class AxisLogarithmicScaleTypeDef(TypedDict):
    Base: NotRequired[float],
```

## ItemsLimitConfigurationTypeDef

```python
# ItemsLimitConfigurationTypeDef definition

class ItemsLimitConfigurationTypeDef(TypedDict):
    ItemsLimit: NotRequired[int],
    OtherCategories: NotRequired[OtherCategoriesType],  # (1)
```

1. See [:material-code-brackets: OtherCategoriesType](./literals.md#othercategoriestype) 
## BinCountOptionsTypeDef

```python
# BinCountOptionsTypeDef definition

class BinCountOptionsTypeDef(TypedDict):
    Value: NotRequired[int],
```

## BinWidthOptionsTypeDef

```python
# BinWidthOptionsTypeDef definition

class BinWidthOptionsTypeDef(TypedDict):
    Value: NotRequired[float],
    BinCountLimit: NotRequired[int],
```

## BookmarksConfigurationsTypeDef

```python
# BookmarksConfigurationsTypeDef definition

class BookmarksConfigurationsTypeDef(TypedDict):
    Enabled: bool,
```

## BorderStyleTypeDef

```python
# BorderStyleTypeDef definition

class BorderStyleTypeDef(TypedDict):
    Show: NotRequired[bool],
```

## BoxPlotStyleOptionsTypeDef

```python
# BoxPlotStyleOptionsTypeDef definition

class BoxPlotStyleOptionsTypeDef(TypedDict):
    FillStyle: NotRequired[BoxPlotFillStyleType],  # (1)
```

1. See [:material-code-brackets: BoxPlotFillStyleType](./literals.md#boxplotfillstyletype) 
## PaginationConfigurationTypeDef

```python
# PaginationConfigurationTypeDef definition

class PaginationConfigurationTypeDef(TypedDict):
    PageSize: int,
    PageNumber: int,
```

## CalculatedColumnTypeDef

```python
# CalculatedColumnTypeDef definition

class CalculatedColumnTypeDef(TypedDict):
    ColumnName: str,
    ColumnId: str,
    Expression: str,
```

## CalculatedMeasureFieldTypeDef

```python
# CalculatedMeasureFieldTypeDef definition

class CalculatedMeasureFieldTypeDef(TypedDict):
    FieldId: str,
    Expression: str,
```

## CancelIngestionRequestRequestTypeDef

```python
# CancelIngestionRequestRequestTypeDef definition

class CancelIngestionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSetId: str,
    IngestionId: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## CastColumnTypeOperationTypeDef

```python
# CastColumnTypeOperationTypeDef definition

class CastColumnTypeOperationTypeDef(TypedDict):
    ColumnName: str,
    NewColumnType: ColumnDataTypeType,  # (1)
    Format: NotRequired[str],
```

1. See [:material-code-brackets: ColumnDataTypeType](./literals.md#columndatatypetype) 
## CustomFilterConfigurationTypeDef

```python
# CustomFilterConfigurationTypeDef definition

class CustomFilterConfigurationTypeDef(TypedDict):
    MatchOperator: CategoryFilterMatchOperatorType,  # (1)
    NullOption: FilterNullOptionType,  # (3)
    CategoryValue: NotRequired[str],
    SelectAllOptions: NotRequired[CategoryFilterSelectAllOptionsType],  # (2)
    ParameterName: NotRequired[str],
```

1. See [:material-code-brackets: CategoryFilterMatchOperatorType](./literals.md#categoryfiltermatchoperatortype) 
2. See [:material-code-brackets: CategoryFilterSelectAllOptionsType](./literals.md#categoryfilterselectalloptionstype) 
3. See [:material-code-brackets: FilterNullOptionType](./literals.md#filternulloptiontype) 
## CustomFilterListConfigurationTypeDef

```python
# CustomFilterListConfigurationTypeDef definition

class CustomFilterListConfigurationTypeDef(TypedDict):
    MatchOperator: CategoryFilterMatchOperatorType,  # (1)
    NullOption: FilterNullOptionType,  # (3)
    CategoryValues: NotRequired[Sequence[str]],
    SelectAllOptions: NotRequired[CategoryFilterSelectAllOptionsType],  # (2)
```

1. See [:material-code-brackets: CategoryFilterMatchOperatorType](./literals.md#categoryfiltermatchoperatortype) 
2. See [:material-code-brackets: CategoryFilterSelectAllOptionsType](./literals.md#categoryfilterselectalloptionstype) 
3. See [:material-code-brackets: FilterNullOptionType](./literals.md#filternulloptiontype) 
## FilterListConfigurationTypeDef

```python
# FilterListConfigurationTypeDef definition

class FilterListConfigurationTypeDef(TypedDict):
    MatchOperator: CategoryFilterMatchOperatorType,  # (1)
    CategoryValues: NotRequired[Sequence[str]],
    SelectAllOptions: NotRequired[CategoryFilterSelectAllOptionsType],  # (2)
```

1. See [:material-code-brackets: CategoryFilterMatchOperatorType](./literals.md#categoryfiltermatchoperatortype) 
2. See [:material-code-brackets: CategoryFilterSelectAllOptionsType](./literals.md#categoryfilterselectalloptionstype) 
## CellValueSynonymTypeDef

```python
# CellValueSynonymTypeDef definition

class CellValueSynonymTypeDef(TypedDict):
    CellValue: NotRequired[str],
    Synonyms: NotRequired[Sequence[str]],
```

## SimpleClusterMarkerTypeDef

```python
# SimpleClusterMarkerTypeDef definition

class SimpleClusterMarkerTypeDef(TypedDict):
    Color: NotRequired[str],
```

## CollectiveConstantTypeDef

```python
# CollectiveConstantTypeDef definition

class CollectiveConstantTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
```

## DataColorTypeDef

```python
# DataColorTypeDef definition

class DataColorTypeDef(TypedDict):
    Color: NotRequired[str],
    DataValue: NotRequired[float],
```

## CustomColorTypeDef

```python
# CustomColorTypeDef definition

class CustomColorTypeDef(TypedDict):
    Color: str,
    FieldValue: NotRequired[str],
    SpecialValue: NotRequired[SpecialValueType],  # (1)
```

1. See [:material-code-brackets: SpecialValueType](./literals.md#specialvaluetype) 
## ColumnDescriptionTypeDef

```python
# ColumnDescriptionTypeDef definition

class ColumnDescriptionTypeDef(TypedDict):
    Text: NotRequired[str],
```

## ColumnGroupColumnSchemaTypeDef

```python
# ColumnGroupColumnSchemaTypeDef definition

class ColumnGroupColumnSchemaTypeDef(TypedDict):
    Name: NotRequired[str],
```

## GeoSpatialColumnGroupTypeDef

```python
# GeoSpatialColumnGroupTypeDef definition

class GeoSpatialColumnGroupTypeDef(TypedDict):
    Name: str,
    Columns: Sequence[str],
    CountryCode: NotRequired[GeoSpatialCountryCodeType],  # (1)
```

1. See [:material-code-brackets: GeoSpatialCountryCodeType](./literals.md#geospatialcountrycodetype) 
## ColumnLevelPermissionRuleTypeDef

```python
# ColumnLevelPermissionRuleTypeDef definition

class ColumnLevelPermissionRuleTypeDef(TypedDict):
    Principals: NotRequired[Sequence[str]],
    ColumnNames: NotRequired[Sequence[str]],
```

## ColumnSchemaTypeDef

```python
# ColumnSchemaTypeDef definition

class ColumnSchemaTypeDef(TypedDict):
    Name: NotRequired[str],
    DataType: NotRequired[str],
    GeographicRole: NotRequired[str],
```

## ComparativeOrderTypeDef

```python
# ComparativeOrderTypeDef definition

class ComparativeOrderTypeDef(TypedDict):
    UseOrdering: NotRequired[ColumnOrderingTypeType],  # (1)
    SpecifedOrder: NotRequired[Sequence[str]],
    TreatUndefinedSpecifiedValues: NotRequired[UndefinedSpecifiedValueTypeType],  # (2)
```

1. See [:material-code-brackets: ColumnOrderingTypeType](./literals.md#columnorderingtypetype) 
2. See [:material-code-brackets: UndefinedSpecifiedValueTypeType](./literals.md#undefinedspecifiedvaluetypetype) 
## ConditionalFormattingSolidColorTypeDef

```python
# ConditionalFormattingSolidColorTypeDef definition

class ConditionalFormattingSolidColorTypeDef(TypedDict):
    Expression: str,
    Color: NotRequired[str],
```

## ConditionalFormattingCustomIconOptionsTypeDef

```python
# ConditionalFormattingCustomIconOptionsTypeDef definition

class ConditionalFormattingCustomIconOptionsTypeDef(TypedDict):
    Icon: NotRequired[IconType],  # (1)
    UnicodeIcon: NotRequired[str],
```

1. See [:material-code-brackets: IconType](./literals.md#icontype) 
## ConditionalFormattingIconDisplayConfigurationTypeDef

```python
# ConditionalFormattingIconDisplayConfigurationTypeDef definition

class ConditionalFormattingIconDisplayConfigurationTypeDef(TypedDict):
    IconDisplayOption: NotRequired[ConditionalFormattingIconDisplayOptionType],  # (1)
```

1. See [:material-code-brackets: ConditionalFormattingIconDisplayOptionType](./literals.md#conditionalformattingicondisplayoptiontype) 
## ConditionalFormattingIconSetTypeDef

```python
# ConditionalFormattingIconSetTypeDef definition

class ConditionalFormattingIconSetTypeDef(TypedDict):
    Expression: str,
    IconSetType: NotRequired[ConditionalFormattingIconSetTypeType],  # (1)
```

1. See [:material-code-brackets: ConditionalFormattingIconSetTypeType](./literals.md#conditionalformattingiconsettypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateAccountSubscriptionRequestRequestTypeDef

```python
# CreateAccountSubscriptionRequestRequestTypeDef definition

class CreateAccountSubscriptionRequestRequestTypeDef(TypedDict):
    Edition: EditionType,  # (1)
    AuthenticationMethod: AuthenticationMethodOptionType,  # (2)
    AwsAccountId: str,
    AccountName: str,
    NotificationEmail: str,
    ActiveDirectoryName: NotRequired[str],
    Realm: NotRequired[str],
    DirectoryId: NotRequired[str],
    AdminGroup: NotRequired[Sequence[str]],
    AuthorGroup: NotRequired[Sequence[str]],
    ReaderGroup: NotRequired[Sequence[str]],
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    EmailAddress: NotRequired[str],
    ContactNumber: NotRequired[str],
```

1. See [:material-code-brackets: EditionType](./literals.md#editiontype) 
2. See [:material-code-brackets: AuthenticationMethodOptionType](./literals.md#authenticationmethodoptiontype) 
## SignupResponseTypeDef

```python
# SignupResponseTypeDef definition

class SignupResponseTypeDef(TypedDict):
    IAMUser: NotRequired[bool],
    userLoginName: NotRequired[str],
    accountName: NotRequired[str],
    directoryType: NotRequired[str],
```

## ResourcePermissionTypeDef

```python
# ResourcePermissionTypeDef definition

class ResourcePermissionTypeDef(TypedDict):
    Principal: str,
    Actions: Sequence[str],
```

## DataSetUsageConfigurationTypeDef

```python
# DataSetUsageConfigurationTypeDef definition

class DataSetUsageConfigurationTypeDef(TypedDict):
    DisableUseAsDirectQuerySource: NotRequired[bool],
    DisableUseAsImportedSource: NotRequired[bool],
```

## FieldFolderTypeDef

```python
# FieldFolderTypeDef definition

class FieldFolderTypeDef(TypedDict):
    description: NotRequired[str],
    columns: NotRequired[Sequence[str]],
```

## RowLevelPermissionDataSetTypeDef

```python
# RowLevelPermissionDataSetTypeDef definition

class RowLevelPermissionDataSetTypeDef(TypedDict):
    Arn: str,
    PermissionPolicy: RowLevelPermissionPolicyType,  # (1)
    Namespace: NotRequired[str],
    FormatVersion: NotRequired[RowLevelPermissionFormatVersionType],  # (2)
    Status: NotRequired[StatusType],  # (3)
```

1. See [:material-code-brackets: RowLevelPermissionPolicyType](./literals.md#rowlevelpermissionpolicytype) 
2. See [:material-code-brackets: RowLevelPermissionFormatVersionType](./literals.md#rowlevelpermissionformatversiontype) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## CreateFolderMembershipRequestRequestTypeDef

```python
# CreateFolderMembershipRequestRequestTypeDef definition

class CreateFolderMembershipRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    FolderId: str,
    MemberId: str,
    MemberType: MemberTypeType,  # (1)
```

1. See [:material-code-brackets: MemberTypeType](./literals.md#membertypetype) 
## FolderMemberTypeDef

```python
# FolderMemberTypeDef definition

class FolderMemberTypeDef(TypedDict):
    MemberId: NotRequired[str],
    MemberType: NotRequired[MemberTypeType],  # (1)
```

1. See [:material-code-brackets: MemberTypeType](./literals.md#membertypetype) 
## CreateGroupMembershipRequestRequestTypeDef

```python
# CreateGroupMembershipRequestRequestTypeDef definition

class CreateGroupMembershipRequestRequestTypeDef(TypedDict):
    MemberName: str,
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
```

## GroupMemberTypeDef

```python
# GroupMemberTypeDef definition

class GroupMemberTypeDef(TypedDict):
    Arn: NotRequired[str],
    MemberName: NotRequired[str],
```

## CreateGroupRequestRequestTypeDef

```python
# CreateGroupRequestRequestTypeDef definition

class CreateGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
    Description: NotRequired[str],
```

## GroupTypeDef

```python
# GroupTypeDef definition

class GroupTypeDef(TypedDict):
    Arn: NotRequired[str],
    GroupName: NotRequired[str],
    Description: NotRequired[str],
    PrincipalId: NotRequired[str],
```

## CreateIAMPolicyAssignmentRequestRequestTypeDef

```python
# CreateIAMPolicyAssignmentRequestRequestTypeDef definition

class CreateIAMPolicyAssignmentRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AssignmentName: str,
    AssignmentStatus: AssignmentStatusType,  # (1)
    Namespace: str,
    PolicyArn: NotRequired[str],
    Identities: NotRequired[Mapping[str, Sequence[str]]],
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
## CreateIngestionRequestRequestTypeDef

```python
# CreateIngestionRequestRequestTypeDef definition

class CreateIngestionRequestRequestTypeDef(TypedDict):
    DataSetId: str,
    IngestionId: str,
    AwsAccountId: str,
    IngestionType: NotRequired[IngestionTypeType],  # (1)
```

1. See [:material-code-brackets: IngestionTypeType](./literals.md#ingestiontypetype) 
## CreateTemplateAliasRequestRequestTypeDef

```python
# CreateTemplateAliasRequestRequestTypeDef definition

class CreateTemplateAliasRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    AliasName: str,
    TemplateVersionNumber: int,
```

## TemplateAliasTypeDef

```python
# TemplateAliasTypeDef definition

class TemplateAliasTypeDef(TypedDict):
    AliasName: NotRequired[str],
    Arn: NotRequired[str],
    TemplateVersionNumber: NotRequired[int],
```

## CreateThemeAliasRequestRequestTypeDef

```python
# CreateThemeAliasRequestRequestTypeDef definition

class CreateThemeAliasRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    ThemeId: str,
    AliasName: str,
    ThemeVersionNumber: int,
```

## ThemeAliasTypeDef

```python
# ThemeAliasTypeDef definition

class ThemeAliasTypeDef(TypedDict):
    Arn: NotRequired[str],
    AliasName: NotRequired[str],
    ThemeVersionNumber: NotRequired[int],
```

## DecimalPlacesConfigurationTypeDef

```python
# DecimalPlacesConfigurationTypeDef definition

class DecimalPlacesConfigurationTypeDef(TypedDict):
    DecimalPlaces: int,
```

## NegativeValueConfigurationTypeDef

```python
# NegativeValueConfigurationTypeDef definition

class NegativeValueConfigurationTypeDef(TypedDict):
    DisplayMode: NegativeValueDisplayModeType,  # (1)
```

1. See [:material-code-brackets: NegativeValueDisplayModeType](./literals.md#negativevaluedisplaymodetype) 
## NullValueFormatConfigurationTypeDef

```python
# NullValueFormatConfigurationTypeDef definition

class NullValueFormatConfigurationTypeDef(TypedDict):
    NullString: str,
```

## LocalNavigationConfigurationTypeDef

```python
# LocalNavigationConfigurationTypeDef definition

class LocalNavigationConfigurationTypeDef(TypedDict):
    TargetSheetId: str,
```

## CustomActionURLOperationTypeDef

```python
# CustomActionURLOperationTypeDef definition

class CustomActionURLOperationTypeDef(TypedDict):
    URLTemplate: str,
    URLTarget: URLTargetConfigurationType,  # (1)
```

1. See [:material-code-brackets: URLTargetConfigurationType](./literals.md#urltargetconfigurationtype) 
## CustomContentConfigurationTypeDef

```python
# CustomContentConfigurationTypeDef definition

class CustomContentConfigurationTypeDef(TypedDict):
    ContentUrl: NotRequired[str],
    ContentType: NotRequired[CustomContentTypeType],  # (1)
    ImageScaling: NotRequired[CustomContentImageScalingConfigurationType],  # (2)
```

1. See [:material-code-brackets: CustomContentTypeType](./literals.md#customcontenttypetype) 
2. See [:material-code-brackets: CustomContentImageScalingConfigurationType](./literals.md#customcontentimagescalingconfigurationtype) 
## CustomNarrativeOptionsTypeDef

```python
# CustomNarrativeOptionsTypeDef definition

class CustomNarrativeOptionsTypeDef(TypedDict):
    Narrative: str,
```

## InputColumnTypeDef

```python
# InputColumnTypeDef definition

class InputColumnTypeDef(TypedDict):
    Name: str,
    Type: InputColumnDataTypeType,  # (1)
```

1. See [:material-code-brackets: InputColumnDataTypeType](./literals.md#inputcolumndatatypetype) 
## DataPointDrillUpDownOptionTypeDef

```python
# DataPointDrillUpDownOptionTypeDef definition

class DataPointDrillUpDownOptionTypeDef(TypedDict):
    AvailabilityStatus: NotRequired[DashboardBehaviorType],  # (1)
```

1. See [:material-code-brackets: DashboardBehaviorType](./literals.md#dashboardbehaviortype) 
## DataPointMenuLabelOptionTypeDef

```python
# DataPointMenuLabelOptionTypeDef definition

class DataPointMenuLabelOptionTypeDef(TypedDict):
    AvailabilityStatus: NotRequired[DashboardBehaviorType],  # (1)
```

1. See [:material-code-brackets: DashboardBehaviorType](./literals.md#dashboardbehaviortype) 
## DataPointTooltipOptionTypeDef

```python
# DataPointTooltipOptionTypeDef definition

class DataPointTooltipOptionTypeDef(TypedDict):
    AvailabilityStatus: NotRequired[DashboardBehaviorType],  # (1)
```

1. See [:material-code-brackets: DashboardBehaviorType](./literals.md#dashboardbehaviortype) 
## ExportToCSVOptionTypeDef

```python
# ExportToCSVOptionTypeDef definition

class ExportToCSVOptionTypeDef(TypedDict):
    AvailabilityStatus: NotRequired[DashboardBehaviorType],  # (1)
```

1. See [:material-code-brackets: DashboardBehaviorType](./literals.md#dashboardbehaviortype) 
## ExportWithHiddenFieldsOptionTypeDef

```python
# ExportWithHiddenFieldsOptionTypeDef definition

class ExportWithHiddenFieldsOptionTypeDef(TypedDict):
    AvailabilityStatus: NotRequired[DashboardBehaviorType],  # (1)
```

1. See [:material-code-brackets: DashboardBehaviorType](./literals.md#dashboardbehaviortype) 
## SheetControlsOptionTypeDef

```python
# SheetControlsOptionTypeDef definition

class SheetControlsOptionTypeDef(TypedDict):
    VisibilityState: NotRequired[DashboardUIStateType],  # (1)
```

1. See [:material-code-brackets: DashboardUIStateType](./literals.md#dashboarduistatetype) 
## SheetLayoutElementMaximizationOptionTypeDef

```python
# SheetLayoutElementMaximizationOptionTypeDef definition

class SheetLayoutElementMaximizationOptionTypeDef(TypedDict):
    AvailabilityStatus: NotRequired[DashboardBehaviorType],  # (1)
```

1. See [:material-code-brackets: DashboardBehaviorType](./literals.md#dashboardbehaviortype) 
## VisualAxisSortOptionTypeDef

```python
# VisualAxisSortOptionTypeDef definition

class VisualAxisSortOptionTypeDef(TypedDict):
    AvailabilityStatus: NotRequired[DashboardBehaviorType],  # (1)
```

1. See [:material-code-brackets: DashboardBehaviorType](./literals.md#dashboardbehaviortype) 
## VisualMenuOptionTypeDef

```python
# VisualMenuOptionTypeDef definition

class VisualMenuOptionTypeDef(TypedDict):
    AvailabilityStatus: NotRequired[DashboardBehaviorType],  # (1)
```

1. See [:material-code-brackets: DashboardBehaviorType](./literals.md#dashboardbehaviortype) 
## DashboardSearchFilterTypeDef

```python
# DashboardSearchFilterTypeDef definition

class DashboardSearchFilterTypeDef(TypedDict):
    Operator: FilterOperatorType,  # (1)
    Name: NotRequired[DashboardFilterAttributeType],  # (2)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: FilterOperatorType](./literals.md#filteroperatortype) 
2. See [:material-code-brackets: DashboardFilterAttributeType](./literals.md#dashboardfilterattributetype) 
## DashboardSummaryTypeDef

```python
# DashboardSummaryTypeDef definition

class DashboardSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    DashboardId: NotRequired[str],
    Name: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    PublishedVersionNumber: NotRequired[int],
    LastPublishedTime: NotRequired[datetime],
```

## DashboardVersionSummaryTypeDef

```python
# DashboardVersionSummaryTypeDef definition

class DashboardVersionSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    VersionNumber: NotRequired[int],
    Status: NotRequired[ResourceStatusType],  # (1)
    SourceEntityArn: NotRequired[str],
    Description: NotRequired[str],
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
## ExportHiddenFieldsOptionTypeDef

```python
# ExportHiddenFieldsOptionTypeDef definition

class ExportHiddenFieldsOptionTypeDef(TypedDict):
    AvailabilityStatus: NotRequired[DashboardBehaviorType],  # (1)
```

1. See [:material-code-brackets: DashboardBehaviorType](./literals.md#dashboardbehaviortype) 
## DataAggregationTypeDef

```python
# DataAggregationTypeDef definition

class DataAggregationTypeDef(TypedDict):
    DatasetRowDateGranularity: NotRequired[TopicTimeGranularityType],  # (1)
    DefaultDateColumnName: NotRequired[str],
```

1. See [:material-code-brackets: TopicTimeGranularityType](./literals.md#topictimegranularitytype) 
## DataBarsOptionsTypeDef

```python
# DataBarsOptionsTypeDef definition

class DataBarsOptionsTypeDef(TypedDict):
    FieldId: str,
    PositiveColor: NotRequired[str],
    NegativeColor: NotRequired[str],
```

## DataColorPaletteTypeDef

```python
# DataColorPaletteTypeDef definition

class DataColorPaletteTypeDef(TypedDict):
    Colors: NotRequired[Sequence[str]],
    MinMaxGradient: NotRequired[Sequence[str]],
    EmptyFillColor: NotRequired[str],
```

## DataPathLabelTypeTypeDef

```python
# DataPathLabelTypeTypeDef definition

class DataPathLabelTypeTypeDef(TypedDict):
    FieldId: NotRequired[str],
    FieldValue: NotRequired[str],
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## FieldLabelTypeTypeDef

```python
# FieldLabelTypeTypeDef definition

class FieldLabelTypeTypeDef(TypedDict):
    FieldId: NotRequired[str],
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## MaximumLabelTypeTypeDef

```python
# MaximumLabelTypeTypeDef definition

class MaximumLabelTypeTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## MinimumLabelTypeTypeDef

```python
# MinimumLabelTypeTypeDef definition

class MinimumLabelTypeTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## RangeEndsLabelTypeTypeDef

```python
# RangeEndsLabelTypeTypeDef definition

class RangeEndsLabelTypeTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## DataPathValueTypeDef

```python
# DataPathValueTypeDef definition

class DataPathValueTypeDef(TypedDict):
    FieldId: str,
    FieldValue: str,
```

## DataSetSearchFilterTypeDef

```python
# DataSetSearchFilterTypeDef definition

class DataSetSearchFilterTypeDef(TypedDict):
    Operator: FilterOperatorType,  # (1)
    Name: DataSetFilterAttributeType,  # (2)
    Value: str,
```

1. See [:material-code-brackets: FilterOperatorType](./literals.md#filteroperatortype) 
2. See [:material-code-brackets: DataSetFilterAttributeType](./literals.md#datasetfilterattributetype) 
## OutputColumnTypeDef

```python
# OutputColumnTypeDef definition

class OutputColumnTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    Type: NotRequired[ColumnDataTypeType],  # (1)
```

1. See [:material-code-brackets: ColumnDataTypeType](./literals.md#columndatatypetype) 
## DataSourceErrorInfoTypeDef

```python
# DataSourceErrorInfoTypeDef definition

class DataSourceErrorInfoTypeDef(TypedDict):
    Type: NotRequired[DataSourceErrorInfoTypeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceErrorInfoTypeType](./literals.md#datasourceerrorinfotypetype) 
## DatabricksParametersTypeDef

```python
# DatabricksParametersTypeDef definition

class DatabricksParametersTypeDef(TypedDict):
    Host: str,
    Port: int,
    SqlEndpointPath: str,
```

## ExasolParametersTypeDef

```python
# ExasolParametersTypeDef definition

class ExasolParametersTypeDef(TypedDict):
    Host: str,
    Port: int,
```

## JiraParametersTypeDef

```python
# JiraParametersTypeDef definition

class JiraParametersTypeDef(TypedDict):
    SiteBaseUrl: str,
```

## MariaDbParametersTypeDef

```python
# MariaDbParametersTypeDef definition

class MariaDbParametersTypeDef(TypedDict):
    Host: str,
    Port: int,
    Database: str,
```

## MySqlParametersTypeDef

```python
# MySqlParametersTypeDef definition

class MySqlParametersTypeDef(TypedDict):
    Host: str,
    Port: int,
    Database: str,
```

## OracleParametersTypeDef

```python
# OracleParametersTypeDef definition

class OracleParametersTypeDef(TypedDict):
    Host: str,
    Port: int,
    Database: str,
```

## PostgreSqlParametersTypeDef

```python
# PostgreSqlParametersTypeDef definition

class PostgreSqlParametersTypeDef(TypedDict):
    Host: str,
    Port: int,
    Database: str,
```

## PrestoParametersTypeDef

```python
# PrestoParametersTypeDef definition

class PrestoParametersTypeDef(TypedDict):
    Host: str,
    Port: int,
    Catalog: str,
```

## RdsParametersTypeDef

```python
# RdsParametersTypeDef definition

class RdsParametersTypeDef(TypedDict):
    InstanceId: str,
    Database: str,
```

## RedshiftParametersTypeDef

```python
# RedshiftParametersTypeDef definition

class RedshiftParametersTypeDef(TypedDict):
    Database: str,
    Host: NotRequired[str],
    Port: NotRequired[int],
    ClusterId: NotRequired[str],
```

## ServiceNowParametersTypeDef

```python
# ServiceNowParametersTypeDef definition

class ServiceNowParametersTypeDef(TypedDict):
    SiteBaseUrl: str,
```

## SnowflakeParametersTypeDef

```python
# SnowflakeParametersTypeDef definition

class SnowflakeParametersTypeDef(TypedDict):
    Host: str,
    Database: str,
    Warehouse: str,
```

## SparkParametersTypeDef

```python
# SparkParametersTypeDef definition

class SparkParametersTypeDef(TypedDict):
    Host: str,
    Port: int,
```

## SqlServerParametersTypeDef

```python
# SqlServerParametersTypeDef definition

class SqlServerParametersTypeDef(TypedDict):
    Host: str,
    Port: int,
    Database: str,
```

## TeradataParametersTypeDef

```python
# TeradataParametersTypeDef definition

class TeradataParametersTypeDef(TypedDict):
    Host: str,
    Port: int,
    Database: str,
```

## TwitterParametersTypeDef

```python
# TwitterParametersTypeDef definition

class TwitterParametersTypeDef(TypedDict):
    Query: str,
    MaxRows: int,
```

## DataSourceSearchFilterTypeDef

```python
# DataSourceSearchFilterTypeDef definition

class DataSourceSearchFilterTypeDef(TypedDict):
    Operator: FilterOperatorType,  # (1)
    Name: DataSourceFilterAttributeType,  # (2)
    Value: str,
```

1. See [:material-code-brackets: FilterOperatorType](./literals.md#filteroperatortype) 
2. See [:material-code-brackets: DataSourceFilterAttributeType](./literals.md#datasourcefilterattributetype) 
## DataSourceSummaryTypeDef

```python
# DataSourceSummaryTypeDef definition

class DataSourceSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    DataSourceId: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[DataSourceTypeType],  # (1)
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
## RollingDateConfigurationTypeDef

```python
# RollingDateConfigurationTypeDef definition

class RollingDateConfigurationTypeDef(TypedDict):
    Expression: str,
    DataSetIdentifier: NotRequired[str],
```

## MappedDataSetParameterTypeDef

```python
# MappedDataSetParameterTypeDef definition

class MappedDataSetParameterTypeDef(TypedDict):
    DataSetIdentifier: str,
    DataSetParameterName: str,
```

## SheetControlInfoIconLabelOptionsTypeDef

```python
# SheetControlInfoIconLabelOptionsTypeDef definition

class SheetControlInfoIconLabelOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    InfoIconText: NotRequired[str],
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## DecimalDatasetParameterDefaultValuesTypeDef

```python
# DecimalDatasetParameterDefaultValuesTypeDef definition

class DecimalDatasetParameterDefaultValuesTypeDef(TypedDict):
    StaticValues: NotRequired[Sequence[float]],
```

## DecimalValueWhenUnsetConfigurationTypeDef

```python
# DecimalValueWhenUnsetConfigurationTypeDef definition

class DecimalValueWhenUnsetConfigurationTypeDef(TypedDict):
    ValueWhenUnsetOption: NotRequired[ValueWhenUnsetOptionType],  # (1)
    CustomValue: NotRequired[float],
```

1. See [:material-code-brackets: ValueWhenUnsetOptionType](./literals.md#valuewhenunsetoptiontype) 
## DecimalParameterTypeDef

```python
# DecimalParameterTypeDef definition

class DecimalParameterTypeDef(TypedDict):
    Name: str,
    Values: Sequence[float],
```

## DeleteAccountCustomizationRequestRequestTypeDef

```python
# DeleteAccountCustomizationRequestRequestTypeDef definition

class DeleteAccountCustomizationRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: NotRequired[str],
```

## DeleteAccountSubscriptionRequestRequestTypeDef

```python
# DeleteAccountSubscriptionRequestRequestTypeDef definition

class DeleteAccountSubscriptionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
```

## DeleteAnalysisRequestRequestTypeDef

```python
# DeleteAnalysisRequestRequestTypeDef definition

class DeleteAnalysisRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AnalysisId: str,
    RecoveryWindowInDays: NotRequired[int],
    ForceDeleteWithoutRecovery: NotRequired[bool],
```

## DeleteDashboardRequestRequestTypeDef

```python
# DeleteDashboardRequestRequestTypeDef definition

class DeleteDashboardRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    VersionNumber: NotRequired[int],
```

## DeleteDataSetRefreshPropertiesRequestRequestTypeDef

```python
# DeleteDataSetRefreshPropertiesRequestRequestTypeDef definition

class DeleteDataSetRefreshPropertiesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSetId: str,
```

## DeleteDataSetRequestRequestTypeDef

```python
# DeleteDataSetRequestRequestTypeDef definition

class DeleteDataSetRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSetId: str,
```

## DeleteDataSourceRequestRequestTypeDef

```python
# DeleteDataSourceRequestRequestTypeDef definition

class DeleteDataSourceRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSourceId: str,
```

## DeleteFolderMembershipRequestRequestTypeDef

```python
# DeleteFolderMembershipRequestRequestTypeDef definition

class DeleteFolderMembershipRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    FolderId: str,
    MemberId: str,
    MemberType: MemberTypeType,  # (1)
```

1. See [:material-code-brackets: MemberTypeType](./literals.md#membertypetype) 
## DeleteFolderRequestRequestTypeDef

```python
# DeleteFolderRequestRequestTypeDef definition

class DeleteFolderRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    FolderId: str,
```

## DeleteGroupMembershipRequestRequestTypeDef

```python
# DeleteGroupMembershipRequestRequestTypeDef definition

class DeleteGroupMembershipRequestRequestTypeDef(TypedDict):
    MemberName: str,
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
```

## DeleteGroupRequestRequestTypeDef

```python
# DeleteGroupRequestRequestTypeDef definition

class DeleteGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
```

## DeleteIAMPolicyAssignmentRequestRequestTypeDef

```python
# DeleteIAMPolicyAssignmentRequestRequestTypeDef definition

class DeleteIAMPolicyAssignmentRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AssignmentName: str,
    Namespace: str,
```

## DeleteNamespaceRequestRequestTypeDef

```python
# DeleteNamespaceRequestRequestTypeDef definition

class DeleteNamespaceRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: str,
```

## DeleteRefreshScheduleRequestRequestTypeDef

```python
# DeleteRefreshScheduleRequestRequestTypeDef definition

class DeleteRefreshScheduleRequestRequestTypeDef(TypedDict):
    DataSetId: str,
    AwsAccountId: str,
    ScheduleId: str,
```

## DeleteTemplateAliasRequestRequestTypeDef

```python
# DeleteTemplateAliasRequestRequestTypeDef definition

class DeleteTemplateAliasRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    AliasName: str,
```

## DeleteTemplateRequestRequestTypeDef

```python
# DeleteTemplateRequestRequestTypeDef definition

class DeleteTemplateRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    VersionNumber: NotRequired[int],
```

## DeleteThemeAliasRequestRequestTypeDef

```python
# DeleteThemeAliasRequestRequestTypeDef definition

class DeleteThemeAliasRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    ThemeId: str,
    AliasName: str,
```

## DeleteThemeRequestRequestTypeDef

```python
# DeleteThemeRequestRequestTypeDef definition

class DeleteThemeRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    ThemeId: str,
    VersionNumber: NotRequired[int],
```

## DeleteTopicRefreshScheduleRequestRequestTypeDef

```python
# DeleteTopicRefreshScheduleRequestRequestTypeDef definition

class DeleteTopicRefreshScheduleRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TopicId: str,
    DatasetId: str,
```

## DeleteTopicRequestRequestTypeDef

```python
# DeleteTopicRequestRequestTypeDef definition

class DeleteTopicRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TopicId: str,
```

## DeleteUserByPrincipalIdRequestRequestTypeDef

```python
# DeleteUserByPrincipalIdRequestRequestTypeDef definition

class DeleteUserByPrincipalIdRequestRequestTypeDef(TypedDict):
    PrincipalId: str,
    AwsAccountId: str,
    Namespace: str,
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    AwsAccountId: str,
    Namespace: str,
```

## DeleteVPCConnectionRequestRequestTypeDef

```python
# DeleteVPCConnectionRequestRequestTypeDef definition

class DeleteVPCConnectionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    VPCConnectionId: str,
```

## DescribeAccountCustomizationRequestRequestTypeDef

```python
# DescribeAccountCustomizationRequestRequestTypeDef definition

class DescribeAccountCustomizationRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: NotRequired[str],
    Resolved: NotRequired[bool],
```

## DescribeAccountSettingsRequestRequestTypeDef

```python
# DescribeAccountSettingsRequestRequestTypeDef definition

class DescribeAccountSettingsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
```

## DescribeAccountSubscriptionRequestRequestTypeDef

```python
# DescribeAccountSubscriptionRequestRequestTypeDef definition

class DescribeAccountSubscriptionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
```

## DescribeAnalysisDefinitionRequestRequestTypeDef

```python
# DescribeAnalysisDefinitionRequestRequestTypeDef definition

class DescribeAnalysisDefinitionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AnalysisId: str,
```

## DescribeAnalysisPermissionsRequestRequestTypeDef

```python
# DescribeAnalysisPermissionsRequestRequestTypeDef definition

class DescribeAnalysisPermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AnalysisId: str,
```

## DescribeAnalysisRequestRequestTypeDef

```python
# DescribeAnalysisRequestRequestTypeDef definition

class DescribeAnalysisRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AnalysisId: str,
```

## DescribeAssetBundleExportJobRequestRequestTypeDef

```python
# DescribeAssetBundleExportJobRequestRequestTypeDef definition

class DescribeAssetBundleExportJobRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AssetBundleExportJobId: str,
```

## DescribeAssetBundleImportJobRequestRequestTypeDef

```python
# DescribeAssetBundleImportJobRequestRequestTypeDef definition

class DescribeAssetBundleImportJobRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AssetBundleImportJobId: str,
```

## DescribeDashboardDefinitionRequestRequestTypeDef

```python
# DescribeDashboardDefinitionRequestRequestTypeDef definition

class DescribeDashboardDefinitionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    VersionNumber: NotRequired[int],
    AliasName: NotRequired[str],
```

## DescribeDashboardPermissionsRequestRequestTypeDef

```python
# DescribeDashboardPermissionsRequestRequestTypeDef definition

class DescribeDashboardPermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
```

## DescribeDashboardRequestRequestTypeDef

```python
# DescribeDashboardRequestRequestTypeDef definition

class DescribeDashboardRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    VersionNumber: NotRequired[int],
    AliasName: NotRequired[str],
```

## DescribeDashboardSnapshotJobRequestRequestTypeDef

```python
# DescribeDashboardSnapshotJobRequestRequestTypeDef definition

class DescribeDashboardSnapshotJobRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    SnapshotJobId: str,
```

## DescribeDashboardSnapshotJobResultRequestRequestTypeDef

```python
# DescribeDashboardSnapshotJobResultRequestRequestTypeDef definition

class DescribeDashboardSnapshotJobResultRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    SnapshotJobId: str,
```

## SnapshotJobErrorInfoTypeDef

```python
# SnapshotJobErrorInfoTypeDef definition

class SnapshotJobErrorInfoTypeDef(TypedDict):
    ErrorMessage: NotRequired[str],
    ErrorType: NotRequired[str],
```

## DescribeDataSetPermissionsRequestRequestTypeDef

```python
# DescribeDataSetPermissionsRequestRequestTypeDef definition

class DescribeDataSetPermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSetId: str,
```

## DescribeDataSetRefreshPropertiesRequestRequestTypeDef

```python
# DescribeDataSetRefreshPropertiesRequestRequestTypeDef definition

class DescribeDataSetRefreshPropertiesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSetId: str,
```

## DescribeDataSetRequestRequestTypeDef

```python
# DescribeDataSetRequestRequestTypeDef definition

class DescribeDataSetRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSetId: str,
```

## DescribeDataSourcePermissionsRequestRequestTypeDef

```python
# DescribeDataSourcePermissionsRequestRequestTypeDef definition

class DescribeDataSourcePermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSourceId: str,
```

## DescribeDataSourceRequestRequestTypeDef

```python
# DescribeDataSourceRequestRequestTypeDef definition

class DescribeDataSourceRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSourceId: str,
```

## DescribeFolderPermissionsRequestRequestTypeDef

```python
# DescribeFolderPermissionsRequestRequestTypeDef definition

class DescribeFolderPermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    FolderId: str,
```

## DescribeFolderRequestRequestTypeDef

```python
# DescribeFolderRequestRequestTypeDef definition

class DescribeFolderRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    FolderId: str,
```

## DescribeFolderResolvedPermissionsRequestRequestTypeDef

```python
# DescribeFolderResolvedPermissionsRequestRequestTypeDef definition

class DescribeFolderResolvedPermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    FolderId: str,
```

## FolderTypeDef

```python
# FolderTypeDef definition

class FolderTypeDef(TypedDict):
    FolderId: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    FolderType: NotRequired[FolderTypeType],  # (1)
    FolderPath: NotRequired[List[str]],
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: FolderTypeType](./literals.md#foldertypetype) 
## DescribeGroupMembershipRequestRequestTypeDef

```python
# DescribeGroupMembershipRequestRequestTypeDef definition

class DescribeGroupMembershipRequestRequestTypeDef(TypedDict):
    MemberName: str,
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
```

## DescribeGroupRequestRequestTypeDef

```python
# DescribeGroupRequestRequestTypeDef definition

class DescribeGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
```

## DescribeIAMPolicyAssignmentRequestRequestTypeDef

```python
# DescribeIAMPolicyAssignmentRequestRequestTypeDef definition

class DescribeIAMPolicyAssignmentRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AssignmentName: str,
    Namespace: str,
```

## IAMPolicyAssignmentTypeDef

```python
# IAMPolicyAssignmentTypeDef definition

class IAMPolicyAssignmentTypeDef(TypedDict):
    AwsAccountId: NotRequired[str],
    AssignmentId: NotRequired[str],
    AssignmentName: NotRequired[str],
    PolicyArn: NotRequired[str],
    Identities: NotRequired[Dict[str, List[str]]],
    AssignmentStatus: NotRequired[AssignmentStatusType],  # (1)
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
## DescribeIngestionRequestRequestTypeDef

```python
# DescribeIngestionRequestRequestTypeDef definition

class DescribeIngestionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSetId: str,
    IngestionId: str,
```

## DescribeIpRestrictionRequestRequestTypeDef

```python
# DescribeIpRestrictionRequestRequestTypeDef definition

class DescribeIpRestrictionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
```

## DescribeNamespaceRequestRequestTypeDef

```python
# DescribeNamespaceRequestRequestTypeDef definition

class DescribeNamespaceRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: str,
```

## DescribeRefreshScheduleRequestRequestTypeDef

```python
# DescribeRefreshScheduleRequestRequestTypeDef definition

class DescribeRefreshScheduleRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSetId: str,
    ScheduleId: str,
```

## DescribeTemplateAliasRequestRequestTypeDef

```python
# DescribeTemplateAliasRequestRequestTypeDef definition

class DescribeTemplateAliasRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    AliasName: str,
```

## DescribeTemplateDefinitionRequestRequestTypeDef

```python
# DescribeTemplateDefinitionRequestRequestTypeDef definition

class DescribeTemplateDefinitionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    VersionNumber: NotRequired[int],
    AliasName: NotRequired[str],
```

## DescribeTemplatePermissionsRequestRequestTypeDef

```python
# DescribeTemplatePermissionsRequestRequestTypeDef definition

class DescribeTemplatePermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
```

## DescribeTemplateRequestRequestTypeDef

```python
# DescribeTemplateRequestRequestTypeDef definition

class DescribeTemplateRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    VersionNumber: NotRequired[int],
    AliasName: NotRequired[str],
```

## DescribeThemeAliasRequestRequestTypeDef

```python
# DescribeThemeAliasRequestRequestTypeDef definition

class DescribeThemeAliasRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    ThemeId: str,
    AliasName: str,
```

## DescribeThemePermissionsRequestRequestTypeDef

```python
# DescribeThemePermissionsRequestRequestTypeDef definition

class DescribeThemePermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    ThemeId: str,
```

## DescribeThemeRequestRequestTypeDef

```python
# DescribeThemeRequestRequestTypeDef definition

class DescribeThemeRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    ThemeId: str,
    VersionNumber: NotRequired[int],
    AliasName: NotRequired[str],
```

## DescribeTopicPermissionsRequestRequestTypeDef

```python
# DescribeTopicPermissionsRequestRequestTypeDef definition

class DescribeTopicPermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TopicId: str,
```

## DescribeTopicRefreshRequestRequestTypeDef

```python
# DescribeTopicRefreshRequestRequestTypeDef definition

class DescribeTopicRefreshRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TopicId: str,
    RefreshId: str,
```

## TopicRefreshDetailsTypeDef

```python
# TopicRefreshDetailsTypeDef definition

class TopicRefreshDetailsTypeDef(TypedDict):
    RefreshArn: NotRequired[str],
    RefreshId: NotRequired[str],
    RefreshStatus: NotRequired[TopicRefreshStatusType],  # (1)
```

1. See [:material-code-brackets: TopicRefreshStatusType](./literals.md#topicrefreshstatustype) 
## DescribeTopicRefreshScheduleRequestRequestTypeDef

```python
# DescribeTopicRefreshScheduleRequestRequestTypeDef definition

class DescribeTopicRefreshScheduleRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TopicId: str,
    DatasetId: str,
```

## DescribeTopicRequestRequestTypeDef

```python
# DescribeTopicRequestRequestTypeDef definition

class DescribeTopicRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TopicId: str,
```

## DescribeUserRequestRequestTypeDef

```python
# DescribeUserRequestRequestTypeDef definition

class DescribeUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    AwsAccountId: str,
    Namespace: str,
```

## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    Arn: NotRequired[str],
    UserName: NotRequired[str],
    Email: NotRequired[str],
    Role: NotRequired[UserRoleType],  # (1)
    IdentityType: NotRequired[IdentityTypeType],  # (2)
    Active: NotRequired[bool],
    PrincipalId: NotRequired[str],
    CustomPermissionsName: NotRequired[str],
    ExternalLoginFederationProviderType: NotRequired[str],
    ExternalLoginFederationProviderUrl: NotRequired[str],
    ExternalLoginId: NotRequired[str],
```

1. See [:material-code-brackets: UserRoleType](./literals.md#userroletype) 
2. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## DescribeVPCConnectionRequestRequestTypeDef

```python
# DescribeVPCConnectionRequestRequestTypeDef definition

class DescribeVPCConnectionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    VPCConnectionId: str,
```

## NegativeFormatTypeDef

```python
# NegativeFormatTypeDef definition

class NegativeFormatTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Suffix: NotRequired[str],
```

## DonutCenterOptionsTypeDef

```python
# DonutCenterOptionsTypeDef definition

class DonutCenterOptionsTypeDef(TypedDict):
    LabelVisibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## ListControlSelectAllOptionsTypeDef

```python
# ListControlSelectAllOptionsTypeDef definition

class ListControlSelectAllOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## ErrorInfoTypeDef

```python
# ErrorInfoTypeDef definition

class ErrorInfoTypeDef(TypedDict):
    Type: NotRequired[IngestionErrorTypeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: IngestionErrorTypeType](./literals.md#ingestionerrortypetype) 
## ExcludePeriodConfigurationTypeDef

```python
# ExcludePeriodConfigurationTypeDef definition

class ExcludePeriodConfigurationTypeDef(TypedDict):
    Amount: int,
    Granularity: TimeGranularityType,  # (1)
    Status: NotRequired[WidgetStatusType],  # (2)
```

1. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype) 
2. See [:material-code-brackets: WidgetStatusType](./literals.md#widgetstatustype) 
## FieldSortTypeDef

```python
# FieldSortTypeDef definition

class FieldSortTypeDef(TypedDict):
    FieldId: str,
    Direction: SortDirectionType,  # (1)
```

1. See [:material-code-brackets: SortDirectionType](./literals.md#sortdirectiontype) 
## FieldTooltipItemTypeDef

```python
# FieldTooltipItemTypeDef definition

class FieldTooltipItemTypeDef(TypedDict):
    FieldId: str,
    Label: NotRequired[str],
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## GeospatialMapStyleOptionsTypeDef

```python
# GeospatialMapStyleOptionsTypeDef definition

class GeospatialMapStyleOptionsTypeDef(TypedDict):
    BaseMapStyle: NotRequired[BaseMapStyleTypeType],  # (1)
```

1. See [:material-code-brackets: BaseMapStyleTypeType](./literals.md#basemapstyletypetype) 
## FilterSelectableValuesTypeDef

```python
# FilterSelectableValuesTypeDef definition

class FilterSelectableValuesTypeDef(TypedDict):
    Values: NotRequired[Sequence[str]],
```

## SameSheetTargetVisualConfigurationTypeDef

```python
# SameSheetTargetVisualConfigurationTypeDef definition

class SameSheetTargetVisualConfigurationTypeDef(TypedDict):
    TargetVisuals: NotRequired[Sequence[str]],
    TargetVisualOptions: NotRequired[TargetVisualOptionsType],  # (1)
```

1. See [:material-code-brackets: TargetVisualOptionsType](./literals.md#targetvisualoptionstype) 
## FilterOperationTypeDef

```python
# FilterOperationTypeDef definition

class FilterOperationTypeDef(TypedDict):
    ConditionExpression: str,
```

## FolderSearchFilterTypeDef

```python
# FolderSearchFilterTypeDef definition

class FolderSearchFilterTypeDef(TypedDict):
    Operator: NotRequired[FilterOperatorType],  # (1)
    Name: NotRequired[FolderFilterAttributeType],  # (2)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: FilterOperatorType](./literals.md#filteroperatortype) 
2. See [:material-code-brackets: FolderFilterAttributeType](./literals.md#folderfilterattributetype) 
## FolderSummaryTypeDef

```python
# FolderSummaryTypeDef definition

class FolderSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    FolderId: NotRequired[str],
    Name: NotRequired[str],
    FolderType: NotRequired[FolderTypeType],  # (1)
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: FolderTypeType](./literals.md#foldertypetype) 
## FontSizeTypeDef

```python
# FontSizeTypeDef definition

class FontSizeTypeDef(TypedDict):
    Relative: NotRequired[RelativeFontSizeType],  # (1)
```

1. See [:material-code-brackets: RelativeFontSizeType](./literals.md#relativefontsizetype) 
## FontWeightTypeDef

```python
# FontWeightTypeDef definition

class FontWeightTypeDef(TypedDict):
    Name: NotRequired[FontWeightNameType],  # (1)
```

1. See [:material-code-brackets: FontWeightNameType](./literals.md#fontweightnametype) 
## FontTypeDef

```python
# FontTypeDef definition

class FontTypeDef(TypedDict):
    FontFamily: NotRequired[str],
```

## TimeBasedForecastPropertiesTypeDef

```python
# TimeBasedForecastPropertiesTypeDef definition

class TimeBasedForecastPropertiesTypeDef(TypedDict):
    PeriodsForward: NotRequired[int],
    PeriodsBackward: NotRequired[int],
    UpperBoundary: NotRequired[float],
    LowerBoundary: NotRequired[float],
    PredictionInterval: NotRequired[int],
    Seasonality: NotRequired[int],
```

## FreeFormLayoutScreenCanvasSizeOptionsTypeDef

```python
# FreeFormLayoutScreenCanvasSizeOptionsTypeDef definition

class FreeFormLayoutScreenCanvasSizeOptionsTypeDef(TypedDict):
    OptimizedViewPortWidth: str,
```

## FreeFormLayoutElementBackgroundStyleTypeDef

```python
# FreeFormLayoutElementBackgroundStyleTypeDef definition

class FreeFormLayoutElementBackgroundStyleTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    Color: NotRequired[str],
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## FreeFormLayoutElementBorderStyleTypeDef

```python
# FreeFormLayoutElementBorderStyleTypeDef definition

class FreeFormLayoutElementBorderStyleTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    Color: NotRequired[str],
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## LoadingAnimationTypeDef

```python
# LoadingAnimationTypeDef definition

class LoadingAnimationTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## SessionTagTypeDef

```python
# SessionTagTypeDef definition

class SessionTagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## GeospatialCoordinateBoundsTypeDef

```python
# GeospatialCoordinateBoundsTypeDef definition

class GeospatialCoordinateBoundsTypeDef(TypedDict):
    North: float,
    South: float,
    West: float,
    East: float,
```

## GeospatialHeatmapDataColorTypeDef

```python
# GeospatialHeatmapDataColorTypeDef definition

class GeospatialHeatmapDataColorTypeDef(TypedDict):
    Color: str,
```

## GetDashboardEmbedUrlRequestRequestTypeDef

```python
# GetDashboardEmbedUrlRequestRequestTypeDef definition

class GetDashboardEmbedUrlRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    IdentityType: EmbeddingIdentityTypeType,  # (1)
    SessionLifetimeInMinutes: NotRequired[int],
    UndoRedoDisabled: NotRequired[bool],
    ResetDisabled: NotRequired[bool],
    StatePersistenceEnabled: NotRequired[bool],
    UserArn: NotRequired[str],
    Namespace: NotRequired[str],
    AdditionalDashboardIds: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: EmbeddingIdentityTypeType](./literals.md#embeddingidentitytypetype) 
## GetSessionEmbedUrlRequestRequestTypeDef

```python
# GetSessionEmbedUrlRequestRequestTypeDef definition

class GetSessionEmbedUrlRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    EntryPoint: NotRequired[str],
    SessionLifetimeInMinutes: NotRequired[int],
    UserArn: NotRequired[str],
```

## TableBorderOptionsTypeDef

```python
# TableBorderOptionsTypeDef definition

class TableBorderOptionsTypeDef(TypedDict):
    Color: NotRequired[str],
    Thickness: NotRequired[int],
    Style: NotRequired[TableBorderStyleType],  # (1)
```

1. See [:material-code-brackets: TableBorderStyleType](./literals.md#tableborderstyletype) 
## GradientStopTypeDef

```python
# GradientStopTypeDef definition

class GradientStopTypeDef(TypedDict):
    GradientOffset: float,
    DataValue: NotRequired[float],
    Color: NotRequired[str],
```

## GridLayoutScreenCanvasSizeOptionsTypeDef

```python
# GridLayoutScreenCanvasSizeOptionsTypeDef definition

class GridLayoutScreenCanvasSizeOptionsTypeDef(TypedDict):
    ResizeOption: ResizeOptionType,  # (1)
    OptimizedViewPortWidth: NotRequired[str],
```

1. See [:material-code-brackets: ResizeOptionType](./literals.md#resizeoptiontype) 
## GridLayoutElementTypeDef

```python
# GridLayoutElementTypeDef definition

class GridLayoutElementTypeDef(TypedDict):
    ElementId: str,
    ElementType: LayoutElementTypeType,  # (1)
    ColumnSpan: int,
    RowSpan: int,
    ColumnIndex: NotRequired[int],
    RowIndex: NotRequired[int],
```

1. See [:material-code-brackets: LayoutElementTypeType](./literals.md#layoutelementtypetype) 
## GroupSearchFilterTypeDef

```python
# GroupSearchFilterTypeDef definition

class GroupSearchFilterTypeDef(TypedDict):
    Operator: GroupFilterOperatorType,  # (1)
    Name: GroupFilterAttributeType,  # (2)
    Value: str,
```

1. See [:material-code-brackets: GroupFilterOperatorType](./literals.md#groupfilteroperatortype) 
2. See [:material-code-brackets: GroupFilterAttributeType](./literals.md#groupfilterattributetype) 
## GutterStyleTypeDef

```python
# GutterStyleTypeDef definition

class GutterStyleTypeDef(TypedDict):
    Show: NotRequired[bool],
```

## IAMPolicyAssignmentSummaryTypeDef

```python
# IAMPolicyAssignmentSummaryTypeDef definition

class IAMPolicyAssignmentSummaryTypeDef(TypedDict):
    AssignmentName: NotRequired[str],
    AssignmentStatus: NotRequired[AssignmentStatusType],  # (1)
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
## LookbackWindowTypeDef

```python
# LookbackWindowTypeDef definition

class LookbackWindowTypeDef(TypedDict):
    ColumnName: str,
    Size: int,
    SizeUnit: LookbackWindowSizeUnitType,  # (1)
```

1. See [:material-code-brackets: LookbackWindowSizeUnitType](./literals.md#lookbackwindowsizeunittype) 
## QueueInfoTypeDef

```python
# QueueInfoTypeDef definition

class QueueInfoTypeDef(TypedDict):
    WaitingOnIngestion: str,
    QueuedIngestion: str,
```

## RowInfoTypeDef

```python
# RowInfoTypeDef definition

class RowInfoTypeDef(TypedDict):
    RowsIngested: NotRequired[int],
    RowsDropped: NotRequired[int],
    TotalRowsInDataset: NotRequired[int],
```

## IntegerDatasetParameterDefaultValuesTypeDef

```python
# IntegerDatasetParameterDefaultValuesTypeDef definition

class IntegerDatasetParameterDefaultValuesTypeDef(TypedDict):
    StaticValues: NotRequired[Sequence[int]],
```

## IntegerValueWhenUnsetConfigurationTypeDef

```python
# IntegerValueWhenUnsetConfigurationTypeDef definition

class IntegerValueWhenUnsetConfigurationTypeDef(TypedDict):
    ValueWhenUnsetOption: NotRequired[ValueWhenUnsetOptionType],  # (1)
    CustomValue: NotRequired[int],
```

1. See [:material-code-brackets: ValueWhenUnsetOptionType](./literals.md#valuewhenunsetoptiontype) 
## IntegerParameterTypeDef

```python
# IntegerParameterTypeDef definition

class IntegerParameterTypeDef(TypedDict):
    Name: str,
    Values: Sequence[int],
```

## JoinKeyPropertiesTypeDef

```python
# JoinKeyPropertiesTypeDef definition

class JoinKeyPropertiesTypeDef(TypedDict):
    UniqueKey: NotRequired[bool],
```

## ProgressBarOptionsTypeDef

```python
# ProgressBarOptionsTypeDef definition

class ProgressBarOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## SecondaryValueOptionsTypeDef

```python
# SecondaryValueOptionsTypeDef definition

class SecondaryValueOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## TrendArrowOptionsTypeDef

```python
# TrendArrowOptionsTypeDef definition

class TrendArrowOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## LineChartLineStyleSettingsTypeDef

```python
# LineChartLineStyleSettingsTypeDef definition

class LineChartLineStyleSettingsTypeDef(TypedDict):
    LineVisibility: NotRequired[VisibilityType],  # (1)
    LineInterpolation: NotRequired[LineInterpolationType],  # (2)
    LineStyle: NotRequired[LineChartLineStyleType],  # (3)
    LineWidth: NotRequired[str],
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-brackets: LineInterpolationType](./literals.md#lineinterpolationtype) 
3. See [:material-code-brackets: LineChartLineStyleType](./literals.md#linechartlinestyletype) 
## LineChartMarkerStyleSettingsTypeDef

```python
# LineChartMarkerStyleSettingsTypeDef definition

class LineChartMarkerStyleSettingsTypeDef(TypedDict):
    MarkerVisibility: NotRequired[VisibilityType],  # (1)
    MarkerShape: NotRequired[LineChartMarkerShapeType],  # (2)
    MarkerSize: NotRequired[str],
    MarkerColor: NotRequired[str],
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-brackets: LineChartMarkerShapeType](./literals.md#linechartmarkershapetype) 
## MissingDataConfigurationTypeDef

```python
# MissingDataConfigurationTypeDef definition

class MissingDataConfigurationTypeDef(TypedDict):
    TreatmentOption: NotRequired[MissingDataTreatmentOptionType],  # (1)
```

1. See [:material-code-brackets: MissingDataTreatmentOptionType](./literals.md#missingdatatreatmentoptiontype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAnalysesRequestRequestTypeDef

```python
# ListAnalysesRequestRequestTypeDef definition

class ListAnalysesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListAssetBundleExportJobsRequestRequestTypeDef

```python
# ListAssetBundleExportJobsRequestRequestTypeDef definition

class ListAssetBundleExportJobsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListAssetBundleImportJobsRequestRequestTypeDef

```python
# ListAssetBundleImportJobsRequestRequestTypeDef definition

class ListAssetBundleImportJobsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListControlSearchOptionsTypeDef

```python
# ListControlSearchOptionsTypeDef definition

class ListControlSearchOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## ListDashboardVersionsRequestRequestTypeDef

```python
# ListDashboardVersionsRequestRequestTypeDef definition

class ListDashboardVersionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDashboardsRequestRequestTypeDef

```python
# ListDashboardsRequestRequestTypeDef definition

class ListDashboardsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDataSetsRequestRequestTypeDef

```python
# ListDataSetsRequestRequestTypeDef definition

class ListDataSetsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDataSourcesRequestRequestTypeDef

```python
# ListDataSourcesRequestRequestTypeDef definition

class ListDataSourcesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListFolderMembersRequestRequestTypeDef

```python
# ListFolderMembersRequestRequestTypeDef definition

class ListFolderMembersRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    FolderId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MemberIdArnPairTypeDef

```python
# MemberIdArnPairTypeDef definition

class MemberIdArnPairTypeDef(TypedDict):
    MemberId: NotRequired[str],
    MemberArn: NotRequired[str],
```

## ListFoldersRequestRequestTypeDef

```python
# ListFoldersRequestRequestTypeDef definition

class ListFoldersRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListGroupMembershipsRequestRequestTypeDef

```python
# ListGroupMembershipsRequestRequestTypeDef definition

class ListGroupMembershipsRequestRequestTypeDef(TypedDict):
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListGroupsRequestRequestTypeDef

```python
# ListGroupsRequestRequestTypeDef definition

class ListGroupsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListIAMPolicyAssignmentsForUserRequestRequestTypeDef

```python
# ListIAMPolicyAssignmentsForUserRequestRequestTypeDef definition

class ListIAMPolicyAssignmentsForUserRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    UserName: str,
    Namespace: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListIAMPolicyAssignmentsRequestRequestTypeDef

```python
# ListIAMPolicyAssignmentsRequestRequestTypeDef definition

class ListIAMPolicyAssignmentsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: str,
    AssignmentStatus: NotRequired[AssignmentStatusType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
## ListIngestionsRequestRequestTypeDef

```python
# ListIngestionsRequestRequestTypeDef definition

class ListIngestionsRequestRequestTypeDef(TypedDict):
    DataSetId: str,
    AwsAccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListNamespacesRequestRequestTypeDef

```python
# ListNamespacesRequestRequestTypeDef definition

class ListNamespacesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListRefreshSchedulesRequestRequestTypeDef

```python
# ListRefreshSchedulesRequestRequestTypeDef definition

class ListRefreshSchedulesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSetId: str,
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListTemplateAliasesRequestRequestTypeDef

```python
# ListTemplateAliasesRequestRequestTypeDef definition

class ListTemplateAliasesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTemplateVersionsRequestRequestTypeDef

```python
# ListTemplateVersionsRequestRequestTypeDef definition

class ListTemplateVersionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## TemplateVersionSummaryTypeDef

```python
# TemplateVersionSummaryTypeDef definition

class TemplateVersionSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    VersionNumber: NotRequired[int],
    CreatedTime: NotRequired[datetime],
    Status: NotRequired[ResourceStatusType],  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
## ListTemplatesRequestRequestTypeDef

```python
# ListTemplatesRequestRequestTypeDef definition

class ListTemplatesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## TemplateSummaryTypeDef

```python
# TemplateSummaryTypeDef definition

class TemplateSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    TemplateId: NotRequired[str],
    Name: NotRequired[str],
    LatestVersionNumber: NotRequired[int],
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

## ListThemeAliasesRequestRequestTypeDef

```python
# ListThemeAliasesRequestRequestTypeDef definition

class ListThemeAliasesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    ThemeId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListThemeVersionsRequestRequestTypeDef

```python
# ListThemeVersionsRequestRequestTypeDef definition

class ListThemeVersionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    ThemeId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ThemeVersionSummaryTypeDef

```python
# ThemeVersionSummaryTypeDef definition

class ThemeVersionSummaryTypeDef(TypedDict):
    VersionNumber: NotRequired[int],
    Arn: NotRequired[str],
    Description: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    Status: NotRequired[ResourceStatusType],  # (1)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
## ListThemesRequestRequestTypeDef

```python
# ListThemesRequestRequestTypeDef definition

class ListThemesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Type: NotRequired[ThemeTypeType],  # (1)
```

1. See [:material-code-brackets: ThemeTypeType](./literals.md#themetypetype) 
## ThemeSummaryTypeDef

```python
# ThemeSummaryTypeDef definition

class ThemeSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    ThemeId: NotRequired[str],
    LatestVersionNumber: NotRequired[int],
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

## ListTopicRefreshSchedulesRequestRequestTypeDef

```python
# ListTopicRefreshSchedulesRequestRequestTypeDef definition

class ListTopicRefreshSchedulesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TopicId: str,
```

## ListTopicsRequestRequestTypeDef

```python
# ListTopicsRequestRequestTypeDef definition

class ListTopicsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## TopicSummaryTypeDef

```python
# TopicSummaryTypeDef definition

class TopicSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    TopicId: NotRequired[str],
    Name: NotRequired[str],
```

## ListUserGroupsRequestRequestTypeDef

```python
# ListUserGroupsRequestRequestTypeDef definition

class ListUserGroupsRequestRequestTypeDef(TypedDict):
    UserName: str,
    AwsAccountId: str,
    Namespace: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListUsersRequestRequestTypeDef

```python
# ListUsersRequestRequestTypeDef definition

class ListUsersRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListVPCConnectionsRequestRequestTypeDef

```python
# ListVPCConnectionsRequestRequestTypeDef definition

class ListVPCConnectionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## LongFormatTextTypeDef

```python
# LongFormatTextTypeDef definition

class LongFormatTextTypeDef(TypedDict):
    PlainText: NotRequired[str],
    RichText: NotRequired[str],
```

## ManifestFileLocationTypeDef

```python
# ManifestFileLocationTypeDef definition

class ManifestFileLocationTypeDef(TypedDict):
    Bucket: str,
    Key: str,
```

## MarginStyleTypeDef

```python
# MarginStyleTypeDef definition

class MarginStyleTypeDef(TypedDict):
    Show: NotRequired[bool],
```

## NamedEntityDefinitionMetricTypeDef

```python
# NamedEntityDefinitionMetricTypeDef definition

class NamedEntityDefinitionMetricTypeDef(TypedDict):
    Aggregation: NotRequired[NamedEntityAggTypeType],  # (1)
    AggregationFunctionParameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: NamedEntityAggTypeType](./literals.md#namedentityaggtypetype) 
## NamespaceErrorTypeDef

```python
# NamespaceErrorTypeDef definition

class NamespaceErrorTypeDef(TypedDict):
    Type: NotRequired[NamespaceErrorTypeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: NamespaceErrorTypeType](./literals.md#namespaceerrortypetype) 
## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    SubnetId: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    ErrorMessage: NotRequired[str],
    Status: NotRequired[NetworkInterfaceStatusType],  # (1)
    NetworkInterfaceId: NotRequired[str],
```

1. See [:material-code-brackets: NetworkInterfaceStatusType](./literals.md#networkinterfacestatustype) 
## NumericRangeFilterValueTypeDef

```python
# NumericRangeFilterValueTypeDef definition

class NumericRangeFilterValueTypeDef(TypedDict):
    StaticValue: NotRequired[float],
    Parameter: NotRequired[str],
```

## ThousandSeparatorOptionsTypeDef

```python
# ThousandSeparatorOptionsTypeDef definition

class ThousandSeparatorOptionsTypeDef(TypedDict):
    Symbol: NotRequired[NumericSeparatorSymbolType],  # (1)
    Visibility: NotRequired[VisibilityType],  # (2)
```

1. See [:material-code-brackets: NumericSeparatorSymbolType](./literals.md#numericseparatorsymboltype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## PercentileAggregationTypeDef

```python
# PercentileAggregationTypeDef definition

class PercentileAggregationTypeDef(TypedDict):
    PercentileValue: NotRequired[float],
```

## StringParameterTypeDef

```python
# StringParameterTypeDef definition

class StringParameterTypeDef(TypedDict):
    Name: str,
    Values: Sequence[str],
```

## PercentVisibleRangeTypeDef

```python
# PercentVisibleRangeTypeDef definition

class PercentVisibleRangeTypeDef(TypedDict):
    From: NotRequired[float],
    To: NotRequired[float],
```

## PivotTableConditionalFormattingScopeTypeDef

```python
# PivotTableConditionalFormattingScopeTypeDef definition

class PivotTableConditionalFormattingScopeTypeDef(TypedDict):
    Role: NotRequired[PivotTableConditionalFormattingScopeRoleType],  # (1)
```

1. See [:material-code-brackets: PivotTableConditionalFormattingScopeRoleType](./literals.md#pivottableconditionalformattingscoperoletype) 
## PivotTablePaginatedReportOptionsTypeDef

```python
# PivotTablePaginatedReportOptionsTypeDef definition

class PivotTablePaginatedReportOptionsTypeDef(TypedDict):
    VerticalOverflowVisibility: NotRequired[VisibilityType],  # (1)
    OverflowColumnHeaderVisibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## PivotTableFieldOptionTypeDef

```python
# PivotTableFieldOptionTypeDef definition

class PivotTableFieldOptionTypeDef(TypedDict):
    FieldId: str,
    CustomLabel: NotRequired[str],
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## PivotTableFieldSubtotalOptionsTypeDef

```python
# PivotTableFieldSubtotalOptionsTypeDef definition

class PivotTableFieldSubtotalOptionsTypeDef(TypedDict):
    FieldId: NotRequired[str],
```

## PivotTableRowsLabelOptionsTypeDef

```python
# PivotTableRowsLabelOptionsTypeDef definition

class PivotTableRowsLabelOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    CustomLabel: NotRequired[str],
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## RowAlternateColorOptionsTypeDef

```python
# RowAlternateColorOptionsTypeDef definition

class RowAlternateColorOptionsTypeDef(TypedDict):
    Status: NotRequired[WidgetStatusType],  # (1)
    RowAlternateColors: NotRequired[Sequence[str]],
    UsePrimaryBackgroundColor: NotRequired[WidgetStatusType],  # (1)
```

1. See [:material-code-brackets: WidgetStatusType](./literals.md#widgetstatustype) 
2. See [:material-code-brackets: WidgetStatusType](./literals.md#widgetstatustype) 
## ProjectOperationTypeDef

```python
# ProjectOperationTypeDef definition

class ProjectOperationTypeDef(TypedDict):
    ProjectedColumns: Sequence[str],
```

## RadarChartAreaStyleSettingsTypeDef

```python
# RadarChartAreaStyleSettingsTypeDef definition

class RadarChartAreaStyleSettingsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## RangeConstantTypeDef

```python
# RangeConstantTypeDef definition

class RangeConstantTypeDef(TypedDict):
    Minimum: NotRequired[str],
    Maximum: NotRequired[str],
```

## ReferenceLineCustomLabelConfigurationTypeDef

```python
# ReferenceLineCustomLabelConfigurationTypeDef definition

class ReferenceLineCustomLabelConfigurationTypeDef(TypedDict):
    CustomLabel: str,
```

## ReferenceLineStaticDataConfigurationTypeDef

```python
# ReferenceLineStaticDataConfigurationTypeDef definition

class ReferenceLineStaticDataConfigurationTypeDef(TypedDict):
    Value: float,
```

## ReferenceLineStyleConfigurationTypeDef

```python
# ReferenceLineStyleConfigurationTypeDef definition

class ReferenceLineStyleConfigurationTypeDef(TypedDict):
    Pattern: NotRequired[ReferenceLinePatternTypeType],  # (1)
    Color: NotRequired[str],
```

1. See [:material-code-brackets: ReferenceLinePatternTypeType](./literals.md#referencelinepatterntypetype) 
## ScheduleRefreshOnEntityTypeDef

```python
# ScheduleRefreshOnEntityTypeDef definition

class ScheduleRefreshOnEntityTypeDef(TypedDict):
    DayOfWeek: NotRequired[DayOfWeekType],  # (1)
    DayOfMonth: NotRequired[str],
```

1. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) 
## RegisterUserRequestRequestTypeDef

```python
# RegisterUserRequestRequestTypeDef definition

class RegisterUserRequestRequestTypeDef(TypedDict):
    IdentityType: IdentityTypeType,  # (1)
    Email: str,
    UserRole: UserRoleType,  # (2)
    AwsAccountId: str,
    Namespace: str,
    IamArn: NotRequired[str],
    SessionName: NotRequired[str],
    UserName: NotRequired[str],
    CustomPermissionsName: NotRequired[str],
    ExternalLoginFederationProviderType: NotRequired[str],
    CustomFederationProviderUrl: NotRequired[str],
    ExternalLoginId: NotRequired[str],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-brackets: UserRoleType](./literals.md#userroletype) 
## StatePersistenceConfigurationsTypeDef

```python
# StatePersistenceConfigurationsTypeDef definition

class StatePersistenceConfigurationsTypeDef(TypedDict):
    Enabled: bool,
```

## RegisteredUserQSearchBarEmbeddingConfigurationTypeDef

```python
# RegisteredUserQSearchBarEmbeddingConfigurationTypeDef definition

class RegisteredUserQSearchBarEmbeddingConfigurationTypeDef(TypedDict):
    InitialTopicId: NotRequired[str],
```

## RenameColumnOperationTypeDef

```python
# RenameColumnOperationTypeDef definition

class RenameColumnOperationTypeDef(TypedDict):
    ColumnName: str,
    NewColumnName: str,
```

## RestoreAnalysisRequestRequestTypeDef

```python
# RestoreAnalysisRequestRequestTypeDef definition

class RestoreAnalysisRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AnalysisId: str,
```

## RowLevelPermissionTagRuleTypeDef

```python
# RowLevelPermissionTagRuleTypeDef definition

class RowLevelPermissionTagRuleTypeDef(TypedDict):
    TagKey: str,
    ColumnName: str,
    TagMultiValueDelimiter: NotRequired[str],
    MatchAllValue: NotRequired[str],
```

## S3BucketConfigurationTypeDef

```python
# S3BucketConfigurationTypeDef definition

class S3BucketConfigurationTypeDef(TypedDict):
    BucketName: str,
    BucketPrefix: str,
    BucketRegion: str,
```

## UploadSettingsTypeDef

```python
# UploadSettingsTypeDef definition

class UploadSettingsTypeDef(TypedDict):
    Format: NotRequired[FileFormatType],  # (1)
    StartFromRow: NotRequired[int],
    ContainsHeader: NotRequired[bool],
    TextQualifier: NotRequired[TextQualifierType],  # (2)
    Delimiter: NotRequired[str],
```

1. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
2. See [:material-code-brackets: TextQualifierType](./literals.md#textqualifiertype) 
## SectionAfterPageBreakTypeDef

```python
# SectionAfterPageBreakTypeDef definition

class SectionAfterPageBreakTypeDef(TypedDict):
    Status: NotRequired[SectionPageBreakStatusType],  # (1)
```

1. See [:material-code-brackets: SectionPageBreakStatusType](./literals.md#sectionpagebreakstatustype) 
## SpacingTypeDef

```python
# SpacingTypeDef definition

class SpacingTypeDef(TypedDict):
    Top: NotRequired[str],
    Bottom: NotRequired[str],
    Left: NotRequired[str],
    Right: NotRequired[str],
```

## SheetVisualScopingConfigurationTypeDef

```python
# SheetVisualScopingConfigurationTypeDef definition

class SheetVisualScopingConfigurationTypeDef(TypedDict):
    SheetId: str,
    Scope: FilterVisualScopeType,  # (1)
    VisualIds: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: FilterVisualScopeType](./literals.md#filtervisualscopetype) 
## SemanticEntityTypeTypeDef

```python
# SemanticEntityTypeTypeDef definition

class SemanticEntityTypeTypeDef(TypedDict):
    TypeName: NotRequired[str],
    SubTypeName: NotRequired[str],
    TypeParameters: NotRequired[Mapping[str, str]],
```

## SemanticTypeTypeDef

```python
# SemanticTypeTypeDef definition

class SemanticTypeTypeDef(TypedDict):
    TypeName: NotRequired[str],
    SubTypeName: NotRequired[str],
    TypeParameters: NotRequired[Mapping[str, str]],
    TruthyCellValue: NotRequired[str],
    TruthyCellValueSynonyms: NotRequired[Sequence[str]],
    FalseyCellValue: NotRequired[str],
    FalseyCellValueSynonyms: NotRequired[Sequence[str]],
```

## SheetTextBoxTypeDef

```python
# SheetTextBoxTypeDef definition

class SheetTextBoxTypeDef(TypedDict):
    SheetTextBoxId: str,
    Content: NotRequired[str],
```

## SheetElementConfigurationOverridesTypeDef

```python
# SheetElementConfigurationOverridesTypeDef definition

class SheetElementConfigurationOverridesTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## ShortFormatTextTypeDef

```python
# ShortFormatTextTypeDef definition

class ShortFormatTextTypeDef(TypedDict):
    PlainText: NotRequired[str],
    RichText: NotRequired[str],
```

## SmallMultiplesAxisPropertiesTypeDef

```python
# SmallMultiplesAxisPropertiesTypeDef definition

class SmallMultiplesAxisPropertiesTypeDef(TypedDict):
    Scale: NotRequired[SmallMultiplesAxisScaleType],  # (1)
    Placement: NotRequired[SmallMultiplesAxisPlacementType],  # (2)
```

1. See [:material-code-brackets: SmallMultiplesAxisScaleType](./literals.md#smallmultiplesaxisscaletype) 
2. See [:material-code-brackets: SmallMultiplesAxisPlacementType](./literals.md#smallmultiplesaxisplacementtype) 
## SnapshotAnonymousUserRedactedTypeDef

```python
# SnapshotAnonymousUserRedactedTypeDef definition

class SnapshotAnonymousUserRedactedTypeDef(TypedDict):
    RowLevelPermissionTagKeys: NotRequired[List[str]],
```

## SnapshotFileSheetSelectionTypeDef

```python
# SnapshotFileSheetSelectionTypeDef definition

class SnapshotFileSheetSelectionTypeDef(TypedDict):
    SheetId: str,
    SelectionScope: SnapshotFileSheetSelectionScopeType,  # (1)
    VisualIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: SnapshotFileSheetSelectionScopeType](./literals.md#snapshotfilesheetselectionscopetype) 
## SnapshotJobResultErrorInfoTypeDef

```python
# SnapshotJobResultErrorInfoTypeDef definition

class SnapshotJobResultErrorInfoTypeDef(TypedDict):
    ErrorMessage: NotRequired[str],
    ErrorType: NotRequired[str],
```

## StringDatasetParameterDefaultValuesTypeDef

```python
# StringDatasetParameterDefaultValuesTypeDef definition

class StringDatasetParameterDefaultValuesTypeDef(TypedDict):
    StaticValues: NotRequired[Sequence[str]],
```

## StringValueWhenUnsetConfigurationTypeDef

```python
# StringValueWhenUnsetConfigurationTypeDef definition

class StringValueWhenUnsetConfigurationTypeDef(TypedDict):
    ValueWhenUnsetOption: NotRequired[ValueWhenUnsetOptionType],  # (1)
    CustomValue: NotRequired[str],
```

1. See [:material-code-brackets: ValueWhenUnsetOptionType](./literals.md#valuewhenunsetoptiontype) 
## TableStyleTargetTypeDef

```python
# TableStyleTargetTypeDef definition

class TableStyleTargetTypeDef(TypedDict):
    CellType: StyledCellTypeType,  # (1)
```

1. See [:material-code-brackets: StyledCellTypeType](./literals.md#styledcelltypetype) 
## TableCellImageSizingConfigurationTypeDef

```python
# TableCellImageSizingConfigurationTypeDef definition

class TableCellImageSizingConfigurationTypeDef(TypedDict):
    TableCellImageScalingConfiguration: NotRequired[TableCellImageScalingConfigurationType],  # (1)
```

1. See [:material-code-brackets: TableCellImageScalingConfigurationType](./literals.md#tablecellimagescalingconfigurationtype) 
## TablePaginatedReportOptionsTypeDef

```python
# TablePaginatedReportOptionsTypeDef definition

class TablePaginatedReportOptionsTypeDef(TypedDict):
    VerticalOverflowVisibility: NotRequired[VisibilityType],  # (1)
    OverflowColumnHeaderVisibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## TableFieldCustomIconContentTypeDef

```python
# TableFieldCustomIconContentTypeDef definition

class TableFieldCustomIconContentTypeDef(TypedDict):
    Icon: NotRequired[TableFieldIconSetTypeType],  # (1)
```

1. See [:material-code-brackets: TableFieldIconSetTypeType](./literals.md#tablefieldiconsettypetype) 
## TemplateSourceTemplateTypeDef

```python
# TemplateSourceTemplateTypeDef definition

class TemplateSourceTemplateTypeDef(TypedDict):
    Arn: str,
```

## TextControlPlaceholderOptionsTypeDef

```python
# TextControlPlaceholderOptionsTypeDef definition

class TextControlPlaceholderOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## UIColorPaletteTypeDef

```python
# UIColorPaletteTypeDef definition

class UIColorPaletteTypeDef(TypedDict):
    PrimaryForeground: NotRequired[str],
    PrimaryBackground: NotRequired[str],
    SecondaryForeground: NotRequired[str],
    SecondaryBackground: NotRequired[str],
    Accent: NotRequired[str],
    AccentForeground: NotRequired[str],
    Danger: NotRequired[str],
    DangerForeground: NotRequired[str],
    Warning: NotRequired[str],
    WarningForeground: NotRequired[str],
    Success: NotRequired[str],
    SuccessForeground: NotRequired[str],
    Dimension: NotRequired[str],
    DimensionForeground: NotRequired[str],
    Measure: NotRequired[str],
    MeasureForeground: NotRequired[str],
```

## ThemeErrorTypeDef

```python
# ThemeErrorTypeDef definition

class ThemeErrorTypeDef(TypedDict):
    Type: NotRequired[ThemeErrorTypeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: ThemeErrorTypeType](./literals.md#themeerrortypetype) 
## TopicSingularFilterConstantTypeDef

```python
# TopicSingularFilterConstantTypeDef definition

class TopicSingularFilterConstantTypeDef(TypedDict):
    ConstantType: NotRequired[ConstantTypeType],  # (1)
    SingularConstant: NotRequired[str],
```

1. See [:material-code-brackets: ConstantTypeType](./literals.md#constanttypetype) 
## UntagColumnOperationTypeDef

```python
# UntagColumnOperationTypeDef definition

class UntagColumnOperationTypeDef(TypedDict):
    ColumnName: str,
    TagNames: Sequence[ColumnTagNameType],  # (1)
```

1. See [:material-code-brackets: ColumnTagNameType](./literals.md#columntagnametype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateAccountSettingsRequestRequestTypeDef

```python
# UpdateAccountSettingsRequestRequestTypeDef definition

class UpdateAccountSettingsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DefaultNamespace: str,
    NotificationEmail: NotRequired[str],
    TerminationProtectionEnabled: NotRequired[bool],
```

## UpdateDashboardPublishedVersionRequestRequestTypeDef

```python
# UpdateDashboardPublishedVersionRequestRequestTypeDef definition

class UpdateDashboardPublishedVersionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    VersionNumber: int,
```

## UpdateFolderRequestRequestTypeDef

```python
# UpdateFolderRequestRequestTypeDef definition

class UpdateFolderRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    FolderId: str,
    Name: str,
```

## UpdateGroupRequestRequestTypeDef

```python
# UpdateGroupRequestRequestTypeDef definition

class UpdateGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
    Description: NotRequired[str],
```

## UpdateIAMPolicyAssignmentRequestRequestTypeDef

```python
# UpdateIAMPolicyAssignmentRequestRequestTypeDef definition

class UpdateIAMPolicyAssignmentRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AssignmentName: str,
    Namespace: str,
    AssignmentStatus: NotRequired[AssignmentStatusType],  # (1)
    PolicyArn: NotRequired[str],
    Identities: NotRequired[Mapping[str, Sequence[str]]],
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
## UpdateIpRestrictionRequestRequestTypeDef

```python
# UpdateIpRestrictionRequestRequestTypeDef definition

class UpdateIpRestrictionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    IpRestrictionRuleMap: NotRequired[Mapping[str, str]],
    Enabled: NotRequired[bool],
```

## UpdatePublicSharingSettingsRequestRequestTypeDef

```python
# UpdatePublicSharingSettingsRequestRequestTypeDef definition

class UpdatePublicSharingSettingsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    PublicSharingEnabled: NotRequired[bool],
```

## UpdateTemplateAliasRequestRequestTypeDef

```python
# UpdateTemplateAliasRequestRequestTypeDef definition

class UpdateTemplateAliasRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    AliasName: str,
    TemplateVersionNumber: int,
```

## UpdateThemeAliasRequestRequestTypeDef

```python
# UpdateThemeAliasRequestRequestTypeDef definition

class UpdateThemeAliasRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    ThemeId: str,
    AliasName: str,
    ThemeVersionNumber: int,
```

## UpdateUserRequestRequestTypeDef

```python
# UpdateUserRequestRequestTypeDef definition

class UpdateUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    AwsAccountId: str,
    Namespace: str,
    Email: str,
    Role: UserRoleType,  # (1)
    CustomPermissionsName: NotRequired[str],
    UnapplyCustomPermissions: NotRequired[bool],
    ExternalLoginFederationProviderType: NotRequired[str],
    CustomFederationProviderUrl: NotRequired[str],
    ExternalLoginId: NotRequired[str],
```

1. See [:material-code-brackets: UserRoleType](./literals.md#userroletype) 
## UpdateVPCConnectionRequestRequestTypeDef

```python
# UpdateVPCConnectionRequestRequestTypeDef definition

class UpdateVPCConnectionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    VPCConnectionId: str,
    Name: str,
    SubnetIds: Sequence[str],
    SecurityGroupIds: Sequence[str],
    RoleArn: str,
    DnsResolvers: NotRequired[Sequence[str]],
```

## WaterfallChartOptionsTypeDef

```python
# WaterfallChartOptionsTypeDef definition

class WaterfallChartOptionsTypeDef(TypedDict):
    TotalBarLabel: NotRequired[str],
```

## WordCloudOptionsTypeDef

```python
# WordCloudOptionsTypeDef definition

class WordCloudOptionsTypeDef(TypedDict):
    WordOrientation: NotRequired[WordCloudWordOrientationType],  # (1)
    WordScaling: NotRequired[WordCloudWordScalingType],  # (2)
    CloudLayout: NotRequired[WordCloudCloudLayoutType],  # (3)
    WordCasing: NotRequired[WordCloudWordCasingType],  # (4)
    WordPadding: NotRequired[WordCloudWordPaddingType],  # (5)
    MaximumStringLength: NotRequired[int],
```

1. See [:material-code-brackets: WordCloudWordOrientationType](./literals.md#wordcloudwordorientationtype) 
2. See [:material-code-brackets: WordCloudWordScalingType](./literals.md#wordcloudwordscalingtype) 
3. See [:material-code-brackets: WordCloudCloudLayoutType](./literals.md#wordcloudcloudlayouttype) 
4. See [:material-code-brackets: WordCloudWordCasingType](./literals.md#wordcloudwordcasingtype) 
5. See [:material-code-brackets: WordCloudWordPaddingType](./literals.md#wordcloudwordpaddingtype) 
## UpdateAccountCustomizationRequestRequestTypeDef

```python
# UpdateAccountCustomizationRequestRequestTypeDef definition

class UpdateAccountCustomizationRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AccountCustomization: AccountCustomizationTypeDef,  # (1)
    Namespace: NotRequired[str],
```

1. See [:material-code-braces: AccountCustomizationTypeDef](./type_defs.md#accountcustomizationtypedef) 
## AxisLabelReferenceOptionsTypeDef

```python
# AxisLabelReferenceOptionsTypeDef definition

class AxisLabelReferenceOptionsTypeDef(TypedDict):
    FieldId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
## CascadingControlSourceTypeDef

```python
# CascadingControlSourceTypeDef definition

class CascadingControlSourceTypeDef(TypedDict):
    SourceSheetControlId: NotRequired[str],
    ColumnToMatch: NotRequired[ColumnIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
## CategoryDrillDownFilterTypeDef

```python
# CategoryDrillDownFilterTypeDef definition

class CategoryDrillDownFilterTypeDef(TypedDict):
    Column: ColumnIdentifierTypeDef,  # (1)
    CategoryValues: Sequence[str],
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
## ContributionAnalysisDefaultTypeDef

```python
# ContributionAnalysisDefaultTypeDef definition

class ContributionAnalysisDefaultTypeDef(TypedDict):
    MeasureFieldId: str,
    ContributorDimensions: Sequence[ColumnIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
## DynamicDefaultValueTypeDef

```python
# DynamicDefaultValueTypeDef definition

class DynamicDefaultValueTypeDef(TypedDict):
    DefaultValueColumn: ColumnIdentifierTypeDef,  # (1)
    UserNameColumn: NotRequired[ColumnIdentifierTypeDef],  # (1)
    GroupNameColumn: NotRequired[ColumnIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
3. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
## FilterOperationSelectedFieldsConfigurationTypeDef

```python
# FilterOperationSelectedFieldsConfigurationTypeDef definition

class FilterOperationSelectedFieldsConfigurationTypeDef(TypedDict):
    SelectedFields: NotRequired[Sequence[str]],
    SelectedFieldOptions: NotRequired[SelectedFieldOptionsType],  # (1)
    SelectedColumns: NotRequired[Sequence[ColumnIdentifierTypeDef]],  # (2)
```

1. See [:material-code-brackets: SelectedFieldOptionsType](./literals.md#selectedfieldoptionstype) 
2. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
## NumericEqualityDrillDownFilterTypeDef

```python
# NumericEqualityDrillDownFilterTypeDef definition

class NumericEqualityDrillDownFilterTypeDef(TypedDict):
    Column: ColumnIdentifierTypeDef,  # (1)
    Value: float,
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
## ParameterSelectableValuesTypeDef

```python
# ParameterSelectableValuesTypeDef definition

class ParameterSelectableValuesTypeDef(TypedDict):
    Values: NotRequired[Sequence[str]],
    LinkToDataSetColumn: NotRequired[ColumnIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
## AnalysisErrorTypeDef

```python
# AnalysisErrorTypeDef definition

class AnalysisErrorTypeDef(TypedDict):
    Type: NotRequired[AnalysisErrorTypeType],  # (1)
    Message: NotRequired[str],
    ViolatedEntities: NotRequired[List[EntityTypeDef]],  # (2)
```

1. See [:material-code-brackets: AnalysisErrorTypeType](./literals.md#analysiserrortypetype) 
2. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
## DashboardErrorTypeDef

```python
# DashboardErrorTypeDef definition

class DashboardErrorTypeDef(TypedDict):
    Type: NotRequired[DashboardErrorTypeType],  # (1)
    Message: NotRequired[str],
    ViolatedEntities: NotRequired[List[EntityTypeDef]],  # (2)
```

1. See [:material-code-brackets: DashboardErrorTypeType](./literals.md#dashboarderrortypetype) 
2. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
## TemplateErrorTypeDef

```python
# TemplateErrorTypeDef definition

class TemplateErrorTypeDef(TypedDict):
    Type: NotRequired[TemplateErrorTypeType],  # (1)
    Message: NotRequired[str],
    ViolatedEntities: NotRequired[List[EntityTypeDef]],  # (2)
```

1. See [:material-code-brackets: TemplateErrorTypeType](./literals.md#templateerrortypetype) 
2. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
## SearchAnalysesRequestRequestTypeDef

```python
# SearchAnalysesRequestRequestTypeDef definition

class SearchAnalysesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Filters: Sequence[AnalysisSearchFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: AnalysisSearchFilterTypeDef](./type_defs.md#analysissearchfiltertypedef) 
## AnalysisSourceTemplateTypeDef

```python
# AnalysisSourceTemplateTypeDef definition

class AnalysisSourceTemplateTypeDef(TypedDict):
    DataSetReferences: Sequence[DataSetReferenceTypeDef],  # (1)
    Arn: str,
```

1. See [:material-code-braces: DataSetReferenceTypeDef](./type_defs.md#datasetreferencetypedef) 
## DashboardSourceTemplateTypeDef

```python
# DashboardSourceTemplateTypeDef definition

class DashboardSourceTemplateTypeDef(TypedDict):
    DataSetReferences: Sequence[DataSetReferenceTypeDef],  # (1)
    Arn: str,
```

1. See [:material-code-braces: DataSetReferenceTypeDef](./type_defs.md#datasetreferencetypedef) 
## TemplateSourceAnalysisTypeDef

```python
# TemplateSourceAnalysisTypeDef definition

class TemplateSourceAnalysisTypeDef(TypedDict):
    Arn: str,
    DataSetReferences: Sequence[DataSetReferenceTypeDef],  # (1)
```

1. See [:material-code-braces: DataSetReferenceTypeDef](./type_defs.md#datasetreferencetypedef) 
## AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef

```python
# AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef definition

class AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef(TypedDict):
    InitialDashboardVisualId: DashboardVisualIdTypeDef,  # (1)
```

1. See [:material-code-braces: DashboardVisualIdTypeDef](./type_defs.md#dashboardvisualidtypedef) 
## RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef

```python
# RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef definition

class RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef(TypedDict):
    InitialDashboardVisualId: DashboardVisualIdTypeDef,  # (1)
```

1. See [:material-code-braces: DashboardVisualIdTypeDef](./type_defs.md#dashboardvisualidtypedef) 
## ArcAxisConfigurationTypeDef

```python
# ArcAxisConfigurationTypeDef definition

class ArcAxisConfigurationTypeDef(TypedDict):
    Range: NotRequired[ArcAxisDisplayRangeTypeDef],  # (1)
    ReserveRange: NotRequired[int],
```

1. See [:material-code-braces: ArcAxisDisplayRangeTypeDef](./type_defs.md#arcaxisdisplayrangetypedef) 
## AssetBundleCloudFormationOverridePropertyConfigurationTypeDef

```python
# AssetBundleCloudFormationOverridePropertyConfigurationTypeDef definition

class AssetBundleCloudFormationOverridePropertyConfigurationTypeDef(TypedDict):
    ResourceIdOverrideConfiguration: NotRequired[AssetBundleExportJobResourceIdOverrideConfigurationTypeDef],  # (1)
    VPCConnections: NotRequired[List[AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef]],  # (2)
    RefreshSchedules: NotRequired[List[AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef]],  # (3)
    DataSources: NotRequired[List[AssetBundleExportJobDataSourceOverridePropertiesTypeDef]],  # (4)
    DataSets: NotRequired[List[AssetBundleExportJobDataSetOverridePropertiesTypeDef]],  # (5)
    Themes: NotRequired[List[AssetBundleExportJobThemeOverridePropertiesTypeDef]],  # (6)
    Analyses: NotRequired[List[AssetBundleExportJobAnalysisOverridePropertiesTypeDef]],  # (7)
    Dashboards: NotRequired[List[AssetBundleExportJobDashboardOverridePropertiesTypeDef]],  # (8)
```

1. See [:material-code-braces: AssetBundleExportJobResourceIdOverrideConfigurationTypeDef](./type_defs.md#assetbundleexportjobresourceidoverrideconfigurationtypedef) 
2. See [:material-code-braces: AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef](./type_defs.md#assetbundleexportjobvpcconnectionoverridepropertiestypedef) 
3. See [:material-code-braces: AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef](./type_defs.md#assetbundleexportjobrefreshscheduleoverridepropertiestypedef) 
4. See [:material-code-braces: AssetBundleExportJobDataSourceOverridePropertiesTypeDef](./type_defs.md#assetbundleexportjobdatasourceoverridepropertiestypedef) 
5. See [:material-code-braces: AssetBundleExportJobDataSetOverridePropertiesTypeDef](./type_defs.md#assetbundleexportjobdatasetoverridepropertiestypedef) 
6. See [:material-code-braces: AssetBundleExportJobThemeOverridePropertiesTypeDef](./type_defs.md#assetbundleexportjobthemeoverridepropertiestypedef) 
7. See [:material-code-braces: AssetBundleExportJobAnalysisOverridePropertiesTypeDef](./type_defs.md#assetbundleexportjobanalysisoverridepropertiestypedef) 
8. See [:material-code-braces: AssetBundleExportJobDashboardOverridePropertiesTypeDef](./type_defs.md#assetbundleexportjobdashboardoverridepropertiestypedef) 
## AssetBundleImportJobDataSourceCredentialsTypeDef

```python
# AssetBundleImportJobDataSourceCredentialsTypeDef definition

class AssetBundleImportJobDataSourceCredentialsTypeDef(TypedDict):
    CredentialPair: NotRequired[AssetBundleImportJobDataSourceCredentialPairTypeDef],  # (1)
    SecretArn: NotRequired[str],
```

1. See [:material-code-braces: AssetBundleImportJobDataSourceCredentialPairTypeDef](./type_defs.md#assetbundleimportjobdatasourcecredentialpairtypedef) 
## AssetBundleImportSourceTypeDef

```python
# AssetBundleImportSourceTypeDef definition

class AssetBundleImportSourceTypeDef(TypedDict):
    Body: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    S3Uri: NotRequired[str],
```

## AxisDisplayRangeTypeDef

```python
# AxisDisplayRangeTypeDef definition

class AxisDisplayRangeTypeDef(TypedDict):
    MinMax: NotRequired[AxisDisplayMinMaxRangeTypeDef],  # (1)
    DataDriven: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: AxisDisplayMinMaxRangeTypeDef](./type_defs.md#axisdisplayminmaxrangetypedef) 
## AxisScaleTypeDef

```python
# AxisScaleTypeDef definition

class AxisScaleTypeDef(TypedDict):
    Linear: NotRequired[AxisLinearScaleTypeDef],  # (1)
    Logarithmic: NotRequired[AxisLogarithmicScaleTypeDef],  # (2)
```

1. See [:material-code-braces: AxisLinearScaleTypeDef](./type_defs.md#axislinearscaletypedef) 
2. See [:material-code-braces: AxisLogarithmicScaleTypeDef](./type_defs.md#axislogarithmicscaletypedef) 
## HistogramBinOptionsTypeDef

```python
# HistogramBinOptionsTypeDef definition

class HistogramBinOptionsTypeDef(TypedDict):
    SelectedBinType: NotRequired[HistogramBinTypeType],  # (1)
    BinCount: NotRequired[BinCountOptionsTypeDef],  # (2)
    BinWidth: NotRequired[BinWidthOptionsTypeDef],  # (3)
    StartValue: NotRequired[float],
```

1. See [:material-code-brackets: HistogramBinTypeType](./literals.md#histogrambintypetype) 
2. See [:material-code-braces: BinCountOptionsTypeDef](./type_defs.md#bincountoptionstypedef) 
3. See [:material-code-braces: BinWidthOptionsTypeDef](./type_defs.md#binwidthoptionstypedef) 
## TileStyleTypeDef

```python
# TileStyleTypeDef definition

class TileStyleTypeDef(TypedDict):
    Border: NotRequired[BorderStyleTypeDef],  # (1)
```

1. See [:material-code-braces: BorderStyleTypeDef](./type_defs.md#borderstyletypedef) 
## BoxPlotOptionsTypeDef

```python
# BoxPlotOptionsTypeDef definition

class BoxPlotOptionsTypeDef(TypedDict):
    StyleOptions: NotRequired[BoxPlotStyleOptionsTypeDef],  # (1)
    OutlierVisibility: NotRequired[VisibilityType],  # (2)
    AllDataPointsVisibility: NotRequired[VisibilityType],  # (2)
```

1. See [:material-code-braces: BoxPlotStyleOptionsTypeDef](./type_defs.md#boxplotstyleoptionstypedef) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
3. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## CreateColumnsOperationTypeDef

```python
# CreateColumnsOperationTypeDef definition

class CreateColumnsOperationTypeDef(TypedDict):
    Columns: Sequence[CalculatedColumnTypeDef],  # (1)
```

1. See [:material-code-braces: CalculatedColumnTypeDef](./type_defs.md#calculatedcolumntypedef) 
## CancelIngestionResponseTypeDef

```python
# CancelIngestionResponseTypeDef definition

class CancelIngestionResponseTypeDef(TypedDict):
    Arn: str,
    IngestionId: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAccountCustomizationResponseTypeDef

```python
# CreateAccountCustomizationResponseTypeDef definition

class CreateAccountCustomizationResponseTypeDef(TypedDict):
    Arn: str,
    AwsAccountId: str,
    Namespace: str,
    AccountCustomization: AccountCustomizationTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountCustomizationTypeDef](./type_defs.md#accountcustomizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAnalysisResponseTypeDef

```python
# CreateAnalysisResponseTypeDef definition

class CreateAnalysisResponseTypeDef(TypedDict):
    Arn: str,
    AnalysisId: str,
    CreationStatus: ResourceStatusType,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDashboardResponseTypeDef

```python
# CreateDashboardResponseTypeDef definition

class CreateDashboardResponseTypeDef(TypedDict):
    Arn: str,
    VersionArn: str,
    DashboardId: str,
    CreationStatus: ResourceStatusType,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataSetResponseTypeDef

```python
# CreateDataSetResponseTypeDef definition

class CreateDataSetResponseTypeDef(TypedDict):
    Arn: str,
    DataSetId: str,
    IngestionArn: str,
    IngestionId: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataSourceResponseTypeDef

```python
# CreateDataSourceResponseTypeDef definition

class CreateDataSourceResponseTypeDef(TypedDict):
    Arn: str,
    DataSourceId: str,
    CreationStatus: ResourceStatusType,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFolderResponseTypeDef

```python
# CreateFolderResponseTypeDef definition

class CreateFolderResponseTypeDef(TypedDict):
    Status: int,
    Arn: str,
    FolderId: str,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIAMPolicyAssignmentResponseTypeDef

```python
# CreateIAMPolicyAssignmentResponseTypeDef definition

class CreateIAMPolicyAssignmentResponseTypeDef(TypedDict):
    AssignmentName: str,
    AssignmentId: str,
    AssignmentStatus: AssignmentStatusType,  # (1)
    PolicyArn: str,
    Identities: Dict[str, List[str]],
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIngestionResponseTypeDef

```python
# CreateIngestionResponseTypeDef definition

class CreateIngestionResponseTypeDef(TypedDict):
    Arn: str,
    IngestionId: str,
    IngestionStatus: IngestionStatusType,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: IngestionStatusType](./literals.md#ingestionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNamespaceResponseTypeDef

```python
# CreateNamespaceResponseTypeDef definition

class CreateNamespaceResponseTypeDef(TypedDict):
    Arn: str,
    Name: str,
    CapacityRegion: str,
    CreationStatus: NamespaceStatusType,  # (1)
    IdentityStore: IdentityStoreType,  # (2)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: NamespaceStatusType](./literals.md#namespacestatustype) 
2. See [:material-code-brackets: IdentityStoreType](./literals.md#identitystoretype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRefreshScheduleResponseTypeDef

```python
# CreateRefreshScheduleResponseTypeDef definition

class CreateRefreshScheduleResponseTypeDef(TypedDict):
    Status: int,
    RequestId: str,
    ScheduleId: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTemplateResponseTypeDef

```python
# CreateTemplateResponseTypeDef definition

class CreateTemplateResponseTypeDef(TypedDict):
    Arn: str,
    VersionArn: str,
    TemplateId: str,
    CreationStatus: ResourceStatusType,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateThemeResponseTypeDef

```python
# CreateThemeResponseTypeDef definition

class CreateThemeResponseTypeDef(TypedDict):
    Arn: str,
    VersionArn: str,
    ThemeId: str,
    CreationStatus: ResourceStatusType,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTopicRefreshScheduleResponseTypeDef

```python
# CreateTopicRefreshScheduleResponseTypeDef definition

class CreateTopicRefreshScheduleResponseTypeDef(TypedDict):
    TopicId: str,
    TopicArn: str,
    DatasetArn: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTopicResponseTypeDef

```python
# CreateTopicResponseTypeDef definition

class CreateTopicResponseTypeDef(TypedDict):
    Arn: str,
    TopicId: str,
    RefreshArn: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVPCConnectionResponseTypeDef

```python
# CreateVPCConnectionResponseTypeDef definition

class CreateVPCConnectionResponseTypeDef(TypedDict):
    Arn: str,
    VPCConnectionId: str,
    CreationStatus: VPCConnectionResourceStatusType,  # (1)
    AvailabilityStatus: VPCConnectionAvailabilityStatusType,  # (2)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VPCConnectionResourceStatusType](./literals.md#vpcconnectionresourcestatustype) 
2. See [:material-code-brackets: VPCConnectionAvailabilityStatusType](./literals.md#vpcconnectionavailabilitystatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAccountCustomizationResponseTypeDef

```python
# DeleteAccountCustomizationResponseTypeDef definition

class DeleteAccountCustomizationResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAccountSubscriptionResponseTypeDef

```python
# DeleteAccountSubscriptionResponseTypeDef definition

class DeleteAccountSubscriptionResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAnalysisResponseTypeDef

```python
# DeleteAnalysisResponseTypeDef definition

class DeleteAnalysisResponseTypeDef(TypedDict):
    Status: int,
    Arn: str,
    AnalysisId: str,
    DeletionTime: datetime,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDashboardResponseTypeDef

```python
# DeleteDashboardResponseTypeDef definition

class DeleteDashboardResponseTypeDef(TypedDict):
    Status: int,
    Arn: str,
    DashboardId: str,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataSetRefreshPropertiesResponseTypeDef

```python
# DeleteDataSetRefreshPropertiesResponseTypeDef definition

class DeleteDataSetRefreshPropertiesResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataSetResponseTypeDef

```python
# DeleteDataSetResponseTypeDef definition

class DeleteDataSetResponseTypeDef(TypedDict):
    Arn: str,
    DataSetId: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataSourceResponseTypeDef

```python
# DeleteDataSourceResponseTypeDef definition

class DeleteDataSourceResponseTypeDef(TypedDict):
    Arn: str,
    DataSourceId: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFolderMembershipResponseTypeDef

```python
# DeleteFolderMembershipResponseTypeDef definition

class DeleteFolderMembershipResponseTypeDef(TypedDict):
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFolderResponseTypeDef

```python
# DeleteFolderResponseTypeDef definition

class DeleteFolderResponseTypeDef(TypedDict):
    Status: int,
    Arn: str,
    FolderId: str,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGroupMembershipResponseTypeDef

```python
# DeleteGroupMembershipResponseTypeDef definition

class DeleteGroupMembershipResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGroupResponseTypeDef

```python
# DeleteGroupResponseTypeDef definition

class DeleteGroupResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteIAMPolicyAssignmentResponseTypeDef

```python
# DeleteIAMPolicyAssignmentResponseTypeDef definition

class DeleteIAMPolicyAssignmentResponseTypeDef(TypedDict):
    AssignmentName: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteNamespaceResponseTypeDef

```python
# DeleteNamespaceResponseTypeDef definition

class DeleteNamespaceResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRefreshScheduleResponseTypeDef

```python
# DeleteRefreshScheduleResponseTypeDef definition

class DeleteRefreshScheduleResponseTypeDef(TypedDict):
    Status: int,
    RequestId: str,
    ScheduleId: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTemplateAliasResponseTypeDef

```python
# DeleteTemplateAliasResponseTypeDef definition

class DeleteTemplateAliasResponseTypeDef(TypedDict):
    Status: int,
    TemplateId: str,
    AliasName: str,
    Arn: str,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTemplateResponseTypeDef

```python
# DeleteTemplateResponseTypeDef definition

class DeleteTemplateResponseTypeDef(TypedDict):
    RequestId: str,
    Arn: str,
    TemplateId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteThemeAliasResponseTypeDef

```python
# DeleteThemeAliasResponseTypeDef definition

class DeleteThemeAliasResponseTypeDef(TypedDict):
    AliasName: str,
    Arn: str,
    RequestId: str,
    Status: int,
    ThemeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteThemeResponseTypeDef

```python
# DeleteThemeResponseTypeDef definition

class DeleteThemeResponseTypeDef(TypedDict):
    Arn: str,
    RequestId: str,
    Status: int,
    ThemeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTopicRefreshScheduleResponseTypeDef

```python
# DeleteTopicRefreshScheduleResponseTypeDef definition

class DeleteTopicRefreshScheduleResponseTypeDef(TypedDict):
    TopicId: str,
    TopicArn: str,
    DatasetArn: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTopicResponseTypeDef

```python
# DeleteTopicResponseTypeDef definition

class DeleteTopicResponseTypeDef(TypedDict):
    Arn: str,
    TopicId: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteUserByPrincipalIdResponseTypeDef

```python
# DeleteUserByPrincipalIdResponseTypeDef definition

class DeleteUserByPrincipalIdResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteUserResponseTypeDef

```python
# DeleteUserResponseTypeDef definition

class DeleteUserResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVPCConnectionResponseTypeDef

```python
# DeleteVPCConnectionResponseTypeDef definition

class DeleteVPCConnectionResponseTypeDef(TypedDict):
    Arn: str,
    VPCConnectionId: str,
    DeletionStatus: VPCConnectionResourceStatusType,  # (1)
    AvailabilityStatus: VPCConnectionAvailabilityStatusType,  # (2)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VPCConnectionResourceStatusType](./literals.md#vpcconnectionresourcestatustype) 
2. See [:material-code-brackets: VPCConnectionAvailabilityStatusType](./literals.md#vpcconnectionavailabilitystatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountCustomizationResponseTypeDef

```python
# DescribeAccountCustomizationResponseTypeDef definition

class DescribeAccountCustomizationResponseTypeDef(TypedDict):
    Arn: str,
    AwsAccountId: str,
    Namespace: str,
    AccountCustomization: AccountCustomizationTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountCustomizationTypeDef](./type_defs.md#accountcustomizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountSettingsResponseTypeDef

```python
# DescribeAccountSettingsResponseTypeDef definition

class DescribeAccountSettingsResponseTypeDef(TypedDict):
    AccountSettings: AccountSettingsTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountSubscriptionResponseTypeDef

```python
# DescribeAccountSubscriptionResponseTypeDef definition

class DescribeAccountSubscriptionResponseTypeDef(TypedDict):
    AccountInfo: AccountInfoTypeDef,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountInfoTypeDef](./type_defs.md#accountinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeIpRestrictionResponseTypeDef

```python
# DescribeIpRestrictionResponseTypeDef definition

class DescribeIpRestrictionResponseTypeDef(TypedDict):
    AwsAccountId: str,
    IpRestrictionRuleMap: Dict[str, str],
    Enabled: bool,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateEmbedUrlForAnonymousUserResponseTypeDef

```python
# GenerateEmbedUrlForAnonymousUserResponseTypeDef definition

class GenerateEmbedUrlForAnonymousUserResponseTypeDef(TypedDict):
    EmbedUrl: str,
    Status: int,
    RequestId: str,
    AnonymousUserArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateEmbedUrlForRegisteredUserResponseTypeDef

```python
# GenerateEmbedUrlForRegisteredUserResponseTypeDef definition

class GenerateEmbedUrlForRegisteredUserResponseTypeDef(TypedDict):
    EmbedUrl: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDashboardEmbedUrlResponseTypeDef

```python
# GetDashboardEmbedUrlResponseTypeDef definition

class GetDashboardEmbedUrlResponseTypeDef(TypedDict):
    EmbedUrl: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSessionEmbedUrlResponseTypeDef

```python
# GetSessionEmbedUrlResponseTypeDef definition

class GetSessionEmbedUrlResponseTypeDef(TypedDict):
    EmbedUrl: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAnalysesResponseTypeDef

```python
# ListAnalysesResponseTypeDef definition

class ListAnalysesResponseTypeDef(TypedDict):
    AnalysisSummaryList: List[AnalysisSummaryTypeDef],  # (1)
    NextToken: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisSummaryTypeDef](./type_defs.md#analysissummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssetBundleExportJobsResponseTypeDef

```python
# ListAssetBundleExportJobsResponseTypeDef definition

class ListAssetBundleExportJobsResponseTypeDef(TypedDict):
    AssetBundleExportJobSummaryList: List[AssetBundleExportJobSummaryTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetBundleExportJobSummaryTypeDef](./type_defs.md#assetbundleexportjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssetBundleImportJobsResponseTypeDef

```python
# ListAssetBundleImportJobsResponseTypeDef definition

class ListAssetBundleImportJobsResponseTypeDef(TypedDict):
    AssetBundleImportJobSummaryList: List[AssetBundleImportJobSummaryTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetBundleImportJobSummaryTypeDef](./type_defs.md#assetbundleimportjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIAMPolicyAssignmentsForUserResponseTypeDef

```python
# ListIAMPolicyAssignmentsForUserResponseTypeDef definition

class ListIAMPolicyAssignmentsForUserResponseTypeDef(TypedDict):
    ActiveAssignments: List[ActiveIAMPolicyAssignmentTypeDef],  # (1)
    RequestId: str,
    NextToken: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActiveIAMPolicyAssignmentTypeDef](./type_defs.md#activeiampolicyassignmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDataSetRefreshPropertiesResponseTypeDef

```python
# PutDataSetRefreshPropertiesResponseTypeDef definition

class PutDataSetRefreshPropertiesResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreAnalysisResponseTypeDef

```python
# RestoreAnalysisResponseTypeDef definition

class RestoreAnalysisResponseTypeDef(TypedDict):
    Status: int,
    Arn: str,
    AnalysisId: str,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchAnalysesResponseTypeDef

```python
# SearchAnalysesResponseTypeDef definition

class SearchAnalysesResponseTypeDef(TypedDict):
    AnalysisSummaryList: List[AnalysisSummaryTypeDef],  # (1)
    NextToken: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisSummaryTypeDef](./type_defs.md#analysissummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAssetBundleExportJobResponseTypeDef

```python
# StartAssetBundleExportJobResponseTypeDef definition

class StartAssetBundleExportJobResponseTypeDef(TypedDict):
    Arn: str,
    AssetBundleExportJobId: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAssetBundleImportJobResponseTypeDef

```python
# StartAssetBundleImportJobResponseTypeDef definition

class StartAssetBundleImportJobResponseTypeDef(TypedDict):
    Arn: str,
    AssetBundleImportJobId: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDashboardSnapshotJobResponseTypeDef

```python
# StartDashboardSnapshotJobResponseTypeDef definition

class StartDashboardSnapshotJobResponseTypeDef(TypedDict):
    Arn: str,
    SnapshotJobId: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceResponseTypeDef

```python
# TagResourceResponseTypeDef definition

class TagResourceResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UntagResourceResponseTypeDef

```python
# UntagResourceResponseTypeDef definition

class UntagResourceResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountCustomizationResponseTypeDef

```python
# UpdateAccountCustomizationResponseTypeDef definition

class UpdateAccountCustomizationResponseTypeDef(TypedDict):
    Arn: str,
    AwsAccountId: str,
    Namespace: str,
    AccountCustomization: AccountCustomizationTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountCustomizationTypeDef](./type_defs.md#accountcustomizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountSettingsResponseTypeDef

```python
# UpdateAccountSettingsResponseTypeDef definition

class UpdateAccountSettingsResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAnalysisResponseTypeDef

```python
# UpdateAnalysisResponseTypeDef definition

class UpdateAnalysisResponseTypeDef(TypedDict):
    Arn: str,
    AnalysisId: str,
    UpdateStatus: ResourceStatusType,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDashboardPublishedVersionResponseTypeDef

```python
# UpdateDashboardPublishedVersionResponseTypeDef definition

class UpdateDashboardPublishedVersionResponseTypeDef(TypedDict):
    DashboardId: str,
    DashboardArn: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDashboardResponseTypeDef

```python
# UpdateDashboardResponseTypeDef definition

class UpdateDashboardResponseTypeDef(TypedDict):
    Arn: str,
    VersionArn: str,
    DashboardId: str,
    CreationStatus: ResourceStatusType,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataSetPermissionsResponseTypeDef

```python
# UpdateDataSetPermissionsResponseTypeDef definition

class UpdateDataSetPermissionsResponseTypeDef(TypedDict):
    DataSetArn: str,
    DataSetId: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataSetResponseTypeDef

```python
# UpdateDataSetResponseTypeDef definition

class UpdateDataSetResponseTypeDef(TypedDict):
    Arn: str,
    DataSetId: str,
    IngestionArn: str,
    IngestionId: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataSourcePermissionsResponseTypeDef

```python
# UpdateDataSourcePermissionsResponseTypeDef definition

class UpdateDataSourcePermissionsResponseTypeDef(TypedDict):
    DataSourceArn: str,
    DataSourceId: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataSourceResponseTypeDef

```python
# UpdateDataSourceResponseTypeDef definition

class UpdateDataSourceResponseTypeDef(TypedDict):
    Arn: str,
    DataSourceId: str,
    UpdateStatus: ResourceStatusType,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFolderResponseTypeDef

```python
# UpdateFolderResponseTypeDef definition

class UpdateFolderResponseTypeDef(TypedDict):
    Status: int,
    Arn: str,
    FolderId: str,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIAMPolicyAssignmentResponseTypeDef

```python
# UpdateIAMPolicyAssignmentResponseTypeDef definition

class UpdateIAMPolicyAssignmentResponseTypeDef(TypedDict):
    AssignmentName: str,
    AssignmentId: str,
    PolicyArn: str,
    Identities: Dict[str, List[str]],
    AssignmentStatus: AssignmentStatusType,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIpRestrictionResponseTypeDef

```python
# UpdateIpRestrictionResponseTypeDef definition

class UpdateIpRestrictionResponseTypeDef(TypedDict):
    AwsAccountId: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePublicSharingSettingsResponseTypeDef

```python
# UpdatePublicSharingSettingsResponseTypeDef definition

class UpdatePublicSharingSettingsResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRefreshScheduleResponseTypeDef

```python
# UpdateRefreshScheduleResponseTypeDef definition

class UpdateRefreshScheduleResponseTypeDef(TypedDict):
    Status: int,
    RequestId: str,
    ScheduleId: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTemplateResponseTypeDef

```python
# UpdateTemplateResponseTypeDef definition

class UpdateTemplateResponseTypeDef(TypedDict):
    TemplateId: str,
    Arn: str,
    VersionArn: str,
    CreationStatus: ResourceStatusType,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateThemeResponseTypeDef

```python
# UpdateThemeResponseTypeDef definition

class UpdateThemeResponseTypeDef(TypedDict):
    ThemeId: str,
    Arn: str,
    VersionArn: str,
    CreationStatus: ResourceStatusType,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTopicRefreshScheduleResponseTypeDef

```python
# UpdateTopicRefreshScheduleResponseTypeDef definition

class UpdateTopicRefreshScheduleResponseTypeDef(TypedDict):
    TopicId: str,
    TopicArn: str,
    DatasetArn: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTopicResponseTypeDef

```python
# UpdateTopicResponseTypeDef definition

class UpdateTopicResponseTypeDef(TypedDict):
    TopicId: str,
    Arn: str,
    RefreshArn: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVPCConnectionResponseTypeDef

```python
# UpdateVPCConnectionResponseTypeDef definition

class UpdateVPCConnectionResponseTypeDef(TypedDict):
    Arn: str,
    VPCConnectionId: str,
    UpdateStatus: VPCConnectionResourceStatusType,  # (1)
    AvailabilityStatus: VPCConnectionAvailabilityStatusType,  # (2)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VPCConnectionResourceStatusType](./literals.md#vpcconnectionresourcestatustype) 
2. See [:material-code-brackets: VPCConnectionAvailabilityStatusType](./literals.md#vpcconnectionavailabilitystatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CategoryFilterConfigurationTypeDef

```python
# CategoryFilterConfigurationTypeDef definition

class CategoryFilterConfigurationTypeDef(TypedDict):
    FilterListConfiguration: NotRequired[FilterListConfigurationTypeDef],  # (1)
    CustomFilterListConfiguration: NotRequired[CustomFilterListConfigurationTypeDef],  # (2)
    CustomFilterConfiguration: NotRequired[CustomFilterConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: FilterListConfigurationTypeDef](./type_defs.md#filterlistconfigurationtypedef) 
2. See [:material-code-braces: CustomFilterListConfigurationTypeDef](./type_defs.md#customfilterlistconfigurationtypedef) 
3. See [:material-code-braces: CustomFilterConfigurationTypeDef](./type_defs.md#customfilterconfigurationtypedef) 
## ClusterMarkerTypeDef

```python
# ClusterMarkerTypeDef definition

class ClusterMarkerTypeDef(TypedDict):
    SimpleClusterMarker: NotRequired[SimpleClusterMarkerTypeDef],  # (1)
```

1. See [:material-code-braces: SimpleClusterMarkerTypeDef](./type_defs.md#simpleclustermarkertypedef) 
## TopicCategoryFilterConstantTypeDef

```python
# TopicCategoryFilterConstantTypeDef definition

class TopicCategoryFilterConstantTypeDef(TypedDict):
    ConstantType: NotRequired[ConstantTypeType],  # (1)
    SingularConstant: NotRequired[str],
    CollectiveConstant: NotRequired[CollectiveConstantTypeDef],  # (2)
```

1. See [:material-code-brackets: ConstantTypeType](./literals.md#constanttypetype) 
2. See [:material-code-braces: CollectiveConstantTypeDef](./type_defs.md#collectiveconstanttypedef) 
## ColorScaleTypeDef

```python
# ColorScaleTypeDef definition

class ColorScaleTypeDef(TypedDict):
    Colors: Sequence[DataColorTypeDef],  # (1)
    ColorFillType: ColorFillTypeType,  # (2)
    NullValueColor: NotRequired[DataColorTypeDef],  # (3)
```

1. See [:material-code-braces: DataColorTypeDef](./type_defs.md#datacolortypedef) 
2. See [:material-code-brackets: ColorFillTypeType](./literals.md#colorfilltypetype) 
3. See [:material-code-braces: DataColorTypeDef](./type_defs.md#datacolortypedef) 
## ColorsConfigurationTypeDef

```python
# ColorsConfigurationTypeDef definition

class ColorsConfigurationTypeDef(TypedDict):
    CustomColors: NotRequired[Sequence[CustomColorTypeDef]],  # (1)
```

1. See [:material-code-braces: CustomColorTypeDef](./type_defs.md#customcolortypedef) 
## ColumnTagTypeDef

```python
# ColumnTagTypeDef definition

class ColumnTagTypeDef(TypedDict):
    ColumnGeographicRole: NotRequired[GeoSpatialDataRoleType],  # (1)
    ColumnDescription: NotRequired[ColumnDescriptionTypeDef],  # (2)
```

1. See [:material-code-brackets: GeoSpatialDataRoleType](./literals.md#geospatialdataroletype) 
2. See [:material-code-braces: ColumnDescriptionTypeDef](./type_defs.md#columndescriptiontypedef) 
## ColumnGroupSchemaTypeDef

```python
# ColumnGroupSchemaTypeDef definition

class ColumnGroupSchemaTypeDef(TypedDict):
    Name: NotRequired[str],
    ColumnGroupColumnSchemaList: NotRequired[Sequence[ColumnGroupColumnSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: ColumnGroupColumnSchemaTypeDef](./type_defs.md#columngroupcolumnschematypedef) 
## ColumnGroupTypeDef

```python
# ColumnGroupTypeDef definition

class ColumnGroupTypeDef(TypedDict):
    GeoSpatialColumnGroup: NotRequired[GeoSpatialColumnGroupTypeDef],  # (1)
```

1. See [:material-code-braces: GeoSpatialColumnGroupTypeDef](./type_defs.md#geospatialcolumngrouptypedef) 
## DataSetSchemaTypeDef

```python
# DataSetSchemaTypeDef definition

class DataSetSchemaTypeDef(TypedDict):
    ColumnSchemaList: NotRequired[Sequence[ColumnSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: ColumnSchemaTypeDef](./type_defs.md#columnschematypedef) 
## ConditionalFormattingCustomIconConditionTypeDef

```python
# ConditionalFormattingCustomIconConditionTypeDef definition

class ConditionalFormattingCustomIconConditionTypeDef(TypedDict):
    Expression: str,
    IconOptions: ConditionalFormattingCustomIconOptionsTypeDef,  # (1)
    Color: NotRequired[str],
    DisplayConfiguration: NotRequired[ConditionalFormattingIconDisplayConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ConditionalFormattingCustomIconOptionsTypeDef](./type_defs.md#conditionalformattingcustomiconoptionstypedef) 
2. See [:material-code-braces: ConditionalFormattingIconDisplayConfigurationTypeDef](./type_defs.md#conditionalformattingicondisplayconfigurationtypedef) 
## CreateAccountCustomizationRequestRequestTypeDef

```python
# CreateAccountCustomizationRequestRequestTypeDef definition

class CreateAccountCustomizationRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AccountCustomization: AccountCustomizationTypeDef,  # (1)
    Namespace: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: AccountCustomizationTypeDef](./type_defs.md#accountcustomizationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateNamespaceRequestRequestTypeDef

```python
# CreateNamespaceRequestRequestTypeDef definition

class CreateNamespaceRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: str,
    IdentityStore: IdentityStoreType,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: IdentityStoreType](./literals.md#identitystoretype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateVPCConnectionRequestRequestTypeDef

```python
# CreateVPCConnectionRequestRequestTypeDef definition

class CreateVPCConnectionRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    VPCConnectionId: str,
    Name: str,
    SubnetIds: Sequence[str],
    SecurityGroupIds: Sequence[str],
    RoleArn: str,
    DnsResolvers: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAccountSubscriptionResponseTypeDef

```python
# CreateAccountSubscriptionResponseTypeDef definition

class CreateAccountSubscriptionResponseTypeDef(TypedDict):
    SignupResponse: SignupResponseTypeDef,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SignupResponseTypeDef](./type_defs.md#signupresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFolderRequestRequestTypeDef

```python
# CreateFolderRequestRequestTypeDef definition

class CreateFolderRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    FolderId: str,
    Name: NotRequired[str],
    FolderType: NotRequired[FolderTypeType],  # (1)
    ParentFolderArn: NotRequired[str],
    Permissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: FolderTypeType](./literals.md#foldertypetype) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeAnalysisPermissionsResponseTypeDef

```python
# DescribeAnalysisPermissionsResponseTypeDef definition

class DescribeAnalysisPermissionsResponseTypeDef(TypedDict):
    AnalysisId: str,
    AnalysisArn: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDataSetPermissionsResponseTypeDef

```python
# DescribeDataSetPermissionsResponseTypeDef definition

class DescribeDataSetPermissionsResponseTypeDef(TypedDict):
    DataSetArn: str,
    DataSetId: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDataSourcePermissionsResponseTypeDef

```python
# DescribeDataSourcePermissionsResponseTypeDef definition

class DescribeDataSourcePermissionsResponseTypeDef(TypedDict):
    DataSourceArn: str,
    DataSourceId: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFolderPermissionsResponseTypeDef

```python
# DescribeFolderPermissionsResponseTypeDef definition

class DescribeFolderPermissionsResponseTypeDef(TypedDict):
    Status: int,
    FolderId: str,
    Arn: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFolderResolvedPermissionsResponseTypeDef

```python
# DescribeFolderResolvedPermissionsResponseTypeDef definition

class DescribeFolderResolvedPermissionsResponseTypeDef(TypedDict):
    Status: int,
    FolderId: str,
    Arn: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTemplatePermissionsResponseTypeDef

```python
# DescribeTemplatePermissionsResponseTypeDef definition

class DescribeTemplatePermissionsResponseTypeDef(TypedDict):
    TemplateId: str,
    TemplateArn: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeThemePermissionsResponseTypeDef

```python
# DescribeThemePermissionsResponseTypeDef definition

class DescribeThemePermissionsResponseTypeDef(TypedDict):
    ThemeId: str,
    ThemeArn: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTopicPermissionsResponseTypeDef

```python
# DescribeTopicPermissionsResponseTypeDef definition

class DescribeTopicPermissionsResponseTypeDef(TypedDict):
    TopicId: str,
    TopicArn: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LinkSharingConfigurationTypeDef

```python
# LinkSharingConfigurationTypeDef definition

class LinkSharingConfigurationTypeDef(TypedDict):
    Permissions: NotRequired[List[ResourcePermissionTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
## UpdateAnalysisPermissionsRequestRequestTypeDef

```python
# UpdateAnalysisPermissionsRequestRequestTypeDef definition

class UpdateAnalysisPermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AnalysisId: str,
    GrantPermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
    RevokePermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
## UpdateAnalysisPermissionsResponseTypeDef

```python
# UpdateAnalysisPermissionsResponseTypeDef definition

class UpdateAnalysisPermissionsResponseTypeDef(TypedDict):
    AnalysisArn: str,
    AnalysisId: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDashboardPermissionsRequestRequestTypeDef

```python
# UpdateDashboardPermissionsRequestRequestTypeDef definition

class UpdateDashboardPermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    GrantPermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
    RevokePermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
    GrantLinkPermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
    RevokeLinkPermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
4. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
## UpdateDataSetPermissionsRequestRequestTypeDef

```python
# UpdateDataSetPermissionsRequestRequestTypeDef definition

class UpdateDataSetPermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSetId: str,
    GrantPermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
    RevokePermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
## UpdateDataSourcePermissionsRequestRequestTypeDef

```python
# UpdateDataSourcePermissionsRequestRequestTypeDef definition

class UpdateDataSourcePermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSourceId: str,
    GrantPermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
    RevokePermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
## UpdateFolderPermissionsRequestRequestTypeDef

```python
# UpdateFolderPermissionsRequestRequestTypeDef definition

class UpdateFolderPermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    FolderId: str,
    GrantPermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
    RevokePermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
## UpdateFolderPermissionsResponseTypeDef

```python
# UpdateFolderPermissionsResponseTypeDef definition

class UpdateFolderPermissionsResponseTypeDef(TypedDict):
    Status: int,
    Arn: str,
    FolderId: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTemplatePermissionsRequestRequestTypeDef

```python
# UpdateTemplatePermissionsRequestRequestTypeDef definition

class UpdateTemplatePermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    GrantPermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
    RevokePermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
## UpdateTemplatePermissionsResponseTypeDef

```python
# UpdateTemplatePermissionsResponseTypeDef definition

class UpdateTemplatePermissionsResponseTypeDef(TypedDict):
    TemplateId: str,
    TemplateArn: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateThemePermissionsRequestRequestTypeDef

```python
# UpdateThemePermissionsRequestRequestTypeDef definition

class UpdateThemePermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    ThemeId: str,
    GrantPermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
    RevokePermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
## UpdateThemePermissionsResponseTypeDef

```python
# UpdateThemePermissionsResponseTypeDef definition

class UpdateThemePermissionsResponseTypeDef(TypedDict):
    ThemeId: str,
    ThemeArn: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTopicPermissionsRequestRequestTypeDef

```python
# UpdateTopicPermissionsRequestRequestTypeDef definition

class UpdateTopicPermissionsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TopicId: str,
    GrantPermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
    RevokePermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
## UpdateTopicPermissionsResponseTypeDef

```python
# UpdateTopicPermissionsResponseTypeDef definition

class UpdateTopicPermissionsResponseTypeDef(TypedDict):
    TopicId: str,
    TopicArn: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSetSummaryTypeDef

```python
# DataSetSummaryTypeDef definition

class DataSetSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    DataSetId: NotRequired[str],
    Name: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    ImportMode: NotRequired[DataSetImportModeType],  # (1)
    RowLevelPermissionDataSet: NotRequired[RowLevelPermissionDataSetTypeDef],  # (2)
    RowLevelPermissionTagConfigurationApplied: NotRequired[bool],
    ColumnLevelPermissionRulesApplied: NotRequired[bool],
```

1. See [:material-code-brackets: DataSetImportModeType](./literals.md#datasetimportmodetype) 
2. See [:material-code-braces: RowLevelPermissionDataSetTypeDef](./type_defs.md#rowlevelpermissiondatasettypedef) 
## CreateFolderMembershipResponseTypeDef

```python
# CreateFolderMembershipResponseTypeDef definition

class CreateFolderMembershipResponseTypeDef(TypedDict):
    Status: int,
    FolderMember: FolderMemberTypeDef,  # (1)
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FolderMemberTypeDef](./type_defs.md#foldermembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupMembershipResponseTypeDef

```python
# CreateGroupMembershipResponseTypeDef definition

class CreateGroupMembershipResponseTypeDef(TypedDict):
    GroupMember: GroupMemberTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupMemberTypeDef](./type_defs.md#groupmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGroupMembershipResponseTypeDef

```python
# DescribeGroupMembershipResponseTypeDef definition

class DescribeGroupMembershipResponseTypeDef(TypedDict):
    GroupMember: GroupMemberTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupMemberTypeDef](./type_defs.md#groupmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupMembershipsResponseTypeDef

```python
# ListGroupMembershipsResponseTypeDef definition

class ListGroupMembershipsResponseTypeDef(TypedDict):
    GroupMemberList: List[GroupMemberTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupMemberTypeDef](./type_defs.md#groupmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupResponseTypeDef

```python
# CreateGroupResponseTypeDef definition

class CreateGroupResponseTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGroupResponseTypeDef

```python
# DescribeGroupResponseTypeDef definition

class DescribeGroupResponseTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupsResponseTypeDef

```python
# ListGroupsResponseTypeDef definition

class ListGroupsResponseTypeDef(TypedDict):
    GroupList: List[GroupTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUserGroupsResponseTypeDef

```python
# ListUserGroupsResponseTypeDef definition

class ListUserGroupsResponseTypeDef(TypedDict):
    GroupList: List[GroupTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchGroupsResponseTypeDef

```python
# SearchGroupsResponseTypeDef definition

class SearchGroupsResponseTypeDef(TypedDict):
    GroupList: List[GroupTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGroupResponseTypeDef

```python
# UpdateGroupResponseTypeDef definition

class UpdateGroupResponseTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTemplateAliasResponseTypeDef

```python
# CreateTemplateAliasResponseTypeDef definition

class CreateTemplateAliasResponseTypeDef(TypedDict):
    TemplateAlias: TemplateAliasTypeDef,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateAliasTypeDef](./type_defs.md#templatealiastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTemplateAliasResponseTypeDef

```python
# DescribeTemplateAliasResponseTypeDef definition

class DescribeTemplateAliasResponseTypeDef(TypedDict):
    TemplateAlias: TemplateAliasTypeDef,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateAliasTypeDef](./type_defs.md#templatealiastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTemplateAliasesResponseTypeDef

```python
# ListTemplateAliasesResponseTypeDef definition

class ListTemplateAliasesResponseTypeDef(TypedDict):
    TemplateAliasList: List[TemplateAliasTypeDef],  # (1)
    Status: int,
    RequestId: str,
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateAliasTypeDef](./type_defs.md#templatealiastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTemplateAliasResponseTypeDef

```python
# UpdateTemplateAliasResponseTypeDef definition

class UpdateTemplateAliasResponseTypeDef(TypedDict):
    TemplateAlias: TemplateAliasTypeDef,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateAliasTypeDef](./type_defs.md#templatealiastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateThemeAliasResponseTypeDef

```python
# CreateThemeAliasResponseTypeDef definition

class CreateThemeAliasResponseTypeDef(TypedDict):
    ThemeAlias: ThemeAliasTypeDef,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeAliasTypeDef](./type_defs.md#themealiastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeThemeAliasResponseTypeDef

```python
# DescribeThemeAliasResponseTypeDef definition

class DescribeThemeAliasResponseTypeDef(TypedDict):
    ThemeAlias: ThemeAliasTypeDef,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeAliasTypeDef](./type_defs.md#themealiastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThemeAliasesResponseTypeDef

```python
# ListThemeAliasesResponseTypeDef definition

class ListThemeAliasesResponseTypeDef(TypedDict):
    ThemeAliasList: List[ThemeAliasTypeDef],  # (1)
    Status: int,
    RequestId: str,
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeAliasTypeDef](./type_defs.md#themealiastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateThemeAliasResponseTypeDef

```python
# UpdateThemeAliasResponseTypeDef definition

class UpdateThemeAliasResponseTypeDef(TypedDict):
    ThemeAlias: ThemeAliasTypeDef,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeAliasTypeDef](./type_defs.md#themealiastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomActionNavigationOperationTypeDef

```python
# CustomActionNavigationOperationTypeDef definition

class CustomActionNavigationOperationTypeDef(TypedDict):
    LocalNavigationConfiguration: NotRequired[LocalNavigationConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: LocalNavigationConfigurationTypeDef](./type_defs.md#localnavigationconfigurationtypedef) 
## CustomParameterValuesTypeDef

```python
# CustomParameterValuesTypeDef definition

class CustomParameterValuesTypeDef(TypedDict):
    StringValues: NotRequired[Sequence[str]],
    IntegerValues: NotRequired[Sequence[int]],
    DecimalValues: NotRequired[Sequence[float]],
    DateTimeValues: NotRequired[Sequence[Union[datetime, str]]],
```

## DateTimeDatasetParameterDefaultValuesTypeDef

```python
# DateTimeDatasetParameterDefaultValuesTypeDef definition

class DateTimeDatasetParameterDefaultValuesTypeDef(TypedDict):
    StaticValues: NotRequired[Sequence[Union[datetime, str]]],
```

## DateTimeParameterTypeDef

```python
# DateTimeParameterTypeDef definition

class DateTimeParameterTypeDef(TypedDict):
    Name: str,
    Values: Sequence[Union[datetime, str]],
```

## DateTimeValueWhenUnsetConfigurationTypeDef

```python
# DateTimeValueWhenUnsetConfigurationTypeDef definition

class DateTimeValueWhenUnsetConfigurationTypeDef(TypedDict):
    ValueWhenUnsetOption: NotRequired[ValueWhenUnsetOptionType],  # (1)
    CustomValue: NotRequired[Union[datetime, str]],
```

1. See [:material-code-brackets: ValueWhenUnsetOptionType](./literals.md#valuewhenunsetoptiontype) 
## NewDefaultValuesTypeDef

```python
# NewDefaultValuesTypeDef definition

class NewDefaultValuesTypeDef(TypedDict):
    StringStaticValues: NotRequired[Sequence[str]],
    DecimalStaticValues: NotRequired[Sequence[float]],
    DateTimeStaticValues: NotRequired[Sequence[Union[datetime, str]]],
    IntegerStaticValues: NotRequired[Sequence[int]],
```

## TimeEqualityFilterTypeDef

```python
# TimeEqualityFilterTypeDef definition

class TimeEqualityFilterTypeDef(TypedDict):
    FilterId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    Value: NotRequired[Union[datetime, str]],
    ParameterName: NotRequired[str],
    TimeGranularity: NotRequired[TimeGranularityType],  # (2)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype) 
## TimeRangeDrillDownFilterTypeDef

```python
# TimeRangeDrillDownFilterTypeDef definition

class TimeRangeDrillDownFilterTypeDef(TypedDict):
    Column: ColumnIdentifierTypeDef,  # (1)
    RangeMinimum: Union[datetime, str],
    RangeMaximum: Union[datetime, str],
    TimeGranularity: TimeGranularityType,  # (2)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype) 
## TopicRefreshScheduleTypeDef

```python
# TopicRefreshScheduleTypeDef definition

class TopicRefreshScheduleTypeDef(TypedDict):
    IsEnabled: bool,
    BasedOnSpiceSchedule: bool,
    StartingAt: NotRequired[Union[datetime, str]],
    Timezone: NotRequired[str],
    RepeatAt: NotRequired[str],
    TopicScheduleType: NotRequired[TopicScheduleTypeType],  # (1)
```

1. See [:material-code-brackets: TopicScheduleTypeType](./literals.md#topicscheduletypetype) 
## WhatIfPointScenarioTypeDef

```python
# WhatIfPointScenarioTypeDef definition

class WhatIfPointScenarioTypeDef(TypedDict):
    Date: Union[datetime, str],
    Value: float,
```

## WhatIfRangeScenarioTypeDef

```python
# WhatIfRangeScenarioTypeDef definition

class WhatIfRangeScenarioTypeDef(TypedDict):
    StartDate: Union[datetime, str],
    EndDate: Union[datetime, str],
    Value: float,
```

## CustomSqlTypeDef

```python
# CustomSqlTypeDef definition

class CustomSqlTypeDef(TypedDict):
    DataSourceArn: str,
    Name: str,
    SqlQuery: str,
    Columns: NotRequired[Sequence[InputColumnTypeDef]],  # (1)
```

1. See [:material-code-braces: InputColumnTypeDef](./type_defs.md#inputcolumntypedef) 
## RelationalTableTypeDef

```python
# RelationalTableTypeDef definition

class RelationalTableTypeDef(TypedDict):
    DataSourceArn: str,
    Name: str,
    InputColumns: Sequence[InputColumnTypeDef],  # (1)
    Catalog: NotRequired[str],
    Schema: NotRequired[str],
```

1. See [:material-code-braces: InputColumnTypeDef](./type_defs.md#inputcolumntypedef) 
## SearchDashboardsRequestRequestTypeDef

```python
# SearchDashboardsRequestRequestTypeDef definition

class SearchDashboardsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Filters: Sequence[DashboardSearchFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DashboardSearchFilterTypeDef](./type_defs.md#dashboardsearchfiltertypedef) 
## ListDashboardsResponseTypeDef

```python
# ListDashboardsResponseTypeDef definition

class ListDashboardsResponseTypeDef(TypedDict):
    DashboardSummaryList: List[DashboardSummaryTypeDef],  # (1)
    NextToken: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DashboardSummaryTypeDef](./type_defs.md#dashboardsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchDashboardsResponseTypeDef

```python
# SearchDashboardsResponseTypeDef definition

class SearchDashboardsResponseTypeDef(TypedDict):
    DashboardSummaryList: List[DashboardSummaryTypeDef],  # (1)
    NextToken: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DashboardSummaryTypeDef](./type_defs.md#dashboardsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDashboardVersionsResponseTypeDef

```python
# ListDashboardVersionsResponseTypeDef definition

class ListDashboardVersionsResponseTypeDef(TypedDict):
    DashboardVersionSummaryList: List[DashboardVersionSummaryTypeDef],  # (1)
    NextToken: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DashboardVersionSummaryTypeDef](./type_defs.md#dashboardversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DashboardVisualPublishOptionsTypeDef

```python
# DashboardVisualPublishOptionsTypeDef definition

class DashboardVisualPublishOptionsTypeDef(TypedDict):
    ExportHiddenFieldsOption: NotRequired[ExportHiddenFieldsOptionTypeDef],  # (1)
```

1. See [:material-code-braces: ExportHiddenFieldsOptionTypeDef](./type_defs.md#exporthiddenfieldsoptiontypedef) 
## TableInlineVisualizationTypeDef

```python
# TableInlineVisualizationTypeDef definition

class TableInlineVisualizationTypeDef(TypedDict):
    DataBars: NotRequired[DataBarsOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: DataBarsOptionsTypeDef](./type_defs.md#databarsoptionstypedef) 
## DataLabelTypeTypeDef

```python
# DataLabelTypeTypeDef definition

class DataLabelTypeTypeDef(TypedDict):
    FieldLabelType: NotRequired[FieldLabelTypeTypeDef],  # (1)
    DataPathLabelType: NotRequired[DataPathLabelTypeTypeDef],  # (2)
    RangeEndsLabelType: NotRequired[RangeEndsLabelTypeTypeDef],  # (3)
    MinimumLabelType: NotRequired[MinimumLabelTypeTypeDef],  # (4)
    MaximumLabelType: NotRequired[MaximumLabelTypeTypeDef],  # (5)
```

1. See [:material-code-braces: FieldLabelTypeTypeDef](./type_defs.md#fieldlabeltypetypedef) 
2. See [:material-code-braces: DataPathLabelTypeTypeDef](./type_defs.md#datapathlabeltypetypedef) 
3. See [:material-code-braces: RangeEndsLabelTypeTypeDef](./type_defs.md#rangeendslabeltypetypedef) 
4. See [:material-code-braces: MinimumLabelTypeTypeDef](./type_defs.md#minimumlabeltypetypedef) 
5. See [:material-code-braces: MaximumLabelTypeTypeDef](./type_defs.md#maximumlabeltypetypedef) 
## DataPathColorTypeDef

```python
# DataPathColorTypeDef definition

class DataPathColorTypeDef(TypedDict):
    Element: DataPathValueTypeDef,  # (1)
    Color: str,
    TimeGranularity: NotRequired[TimeGranularityType],  # (2)
```

1. See [:material-code-braces: DataPathValueTypeDef](./type_defs.md#datapathvaluetypedef) 
2. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype) 
## DataPathSortTypeDef

```python
# DataPathSortTypeDef definition

class DataPathSortTypeDef(TypedDict):
    Direction: SortDirectionType,  # (1)
    SortPaths: Sequence[DataPathValueTypeDef],  # (2)
```

1. See [:material-code-brackets: SortDirectionType](./literals.md#sortdirectiontype) 
2. See [:material-code-braces: DataPathValueTypeDef](./type_defs.md#datapathvaluetypedef) 
## PivotTableDataPathOptionTypeDef

```python
# PivotTableDataPathOptionTypeDef definition

class PivotTableDataPathOptionTypeDef(TypedDict):
    DataPathList: Sequence[DataPathValueTypeDef],  # (1)
    Width: NotRequired[str],
```

1. See [:material-code-braces: DataPathValueTypeDef](./type_defs.md#datapathvaluetypedef) 
## PivotTableFieldCollapseStateTargetTypeDef

```python
# PivotTableFieldCollapseStateTargetTypeDef definition

class PivotTableFieldCollapseStateTargetTypeDef(TypedDict):
    FieldId: NotRequired[str],
    FieldDataPathValues: NotRequired[Sequence[DataPathValueTypeDef]],  # (1)
```

1. See [:material-code-braces: DataPathValueTypeDef](./type_defs.md#datapathvaluetypedef) 
## SearchDataSetsRequestRequestTypeDef

```python
# SearchDataSetsRequestRequestTypeDef definition

class SearchDataSetsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Filters: Sequence[DataSetSearchFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DataSetSearchFilterTypeDef](./type_defs.md#datasetsearchfiltertypedef) 
## SearchDataSourcesRequestRequestTypeDef

```python
# SearchDataSourcesRequestRequestTypeDef definition

class SearchDataSourcesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Filters: Sequence[DataSourceSearchFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DataSourceSearchFilterTypeDef](./type_defs.md#datasourcesearchfiltertypedef) 
## SearchDataSourcesResponseTypeDef

```python
# SearchDataSourcesResponseTypeDef definition

class SearchDataSourcesResponseTypeDef(TypedDict):
    DataSourceSummaries: List[DataSourceSummaryTypeDef],  # (1)
    NextToken: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceSummaryTypeDef](./type_defs.md#datasourcesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TimeRangeFilterValueTypeDef

```python
# TimeRangeFilterValueTypeDef definition

class TimeRangeFilterValueTypeDef(TypedDict):
    StaticValue: NotRequired[Union[datetime, str]],
    RollingDate: NotRequired[RollingDateConfigurationTypeDef],  # (1)
    Parameter: NotRequired[str],
```

1. See [:material-code-braces: RollingDateConfigurationTypeDef](./type_defs.md#rollingdateconfigurationtypedef) 
## DecimalDatasetParameterTypeDef

```python
# DecimalDatasetParameterTypeDef definition

class DecimalDatasetParameterTypeDef(TypedDict):
    Id: str,
    Name: str,
    ValueType: DatasetParameterValueTypeType,  # (1)
    DefaultValues: NotRequired[DecimalDatasetParameterDefaultValuesTypeDef],  # (2)
```

1. See [:material-code-brackets: DatasetParameterValueTypeType](./literals.md#datasetparametervaluetypetype) 
2. See [:material-code-braces: DecimalDatasetParameterDefaultValuesTypeDef](./type_defs.md#decimaldatasetparameterdefaultvaluestypedef) 
## DescribeFolderResponseTypeDef

```python
# DescribeFolderResponseTypeDef definition

class DescribeFolderResponseTypeDef(TypedDict):
    Status: int,
    Folder: FolderTypeDef,  # (1)
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FolderTypeDef](./type_defs.md#foldertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeIAMPolicyAssignmentResponseTypeDef

```python
# DescribeIAMPolicyAssignmentResponseTypeDef definition

class DescribeIAMPolicyAssignmentResponseTypeDef(TypedDict):
    IAMPolicyAssignment: IAMPolicyAssignmentTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IAMPolicyAssignmentTypeDef](./type_defs.md#iampolicyassignmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTopicRefreshResponseTypeDef

```python
# DescribeTopicRefreshResponseTypeDef definition

class DescribeTopicRefreshResponseTypeDef(TypedDict):
    RefreshDetails: TopicRefreshDetailsTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TopicRefreshDetailsTypeDef](./type_defs.md#topicrefreshdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserResponseTypeDef

```python
# DescribeUserResponseTypeDef definition

class DescribeUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersResponseTypeDef

```python
# ListUsersResponseTypeDef definition

class ListUsersResponseTypeDef(TypedDict):
    UserList: List[UserTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterUserResponseTypeDef

```python
# RegisterUserResponseTypeDef definition

class RegisterUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    UserInvitationUrl: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserResponseTypeDef

```python
# UpdateUserResponseTypeDef definition

class UpdateUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisplayFormatOptionsTypeDef

```python
# DisplayFormatOptionsTypeDef definition

class DisplayFormatOptionsTypeDef(TypedDict):
    UseBlankCellFormat: NotRequired[bool],
    BlankCellFormat: NotRequired[str],
    DateFormat: NotRequired[str],
    DecimalSeparator: NotRequired[TopicNumericSeparatorSymbolType],  # (1)
    GroupingSeparator: NotRequired[str],
    UseGrouping: NotRequired[bool],
    FractionDigits: NotRequired[int],
    Prefix: NotRequired[str],
    Suffix: NotRequired[str],
    UnitScaler: NotRequired[NumberScaleType],  # (2)
    NegativeFormat: NotRequired[NegativeFormatTypeDef],  # (3)
    CurrencySymbol: NotRequired[str],
```

1. See [:material-code-brackets: TopicNumericSeparatorSymbolType](./literals.md#topicnumericseparatorsymboltype) 
2. See [:material-code-brackets: NumberScaleType](./literals.md#numberscaletype) 
3. See [:material-code-braces: NegativeFormatTypeDef](./type_defs.md#negativeformattypedef) 
## DonutOptionsTypeDef

```python
# DonutOptionsTypeDef definition

class DonutOptionsTypeDef(TypedDict):
    ArcOptions: NotRequired[ArcOptionsTypeDef],  # (1)
    DonutCenterOptions: NotRequired[DonutCenterOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: ArcOptionsTypeDef](./type_defs.md#arcoptionstypedef) 
2. See [:material-code-braces: DonutCenterOptionsTypeDef](./type_defs.md#donutcenteroptionstypedef) 
## RelativeDatesFilterTypeDef

```python
# RelativeDatesFilterTypeDef definition

class RelativeDatesFilterTypeDef(TypedDict):
    FilterId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    AnchorDateConfiguration: AnchorDateConfigurationTypeDef,  # (2)
    TimeGranularity: TimeGranularityType,  # (3)
    RelativeDateType: RelativeDateTypeType,  # (5)
    NullOption: FilterNullOptionType,  # (6)
    MinimumGranularity: NotRequired[TimeGranularityType],  # (3)
    RelativeDateValue: NotRequired[int],
    ParameterName: NotRequired[str],
    ExcludePeriodConfiguration: NotRequired[ExcludePeriodConfigurationTypeDef],  # (7)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: AnchorDateConfigurationTypeDef](./type_defs.md#anchordateconfigurationtypedef) 
3. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype) 
4. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype) 
5. See [:material-code-brackets: RelativeDateTypeType](./literals.md#relativedatetypetype) 
6. See [:material-code-brackets: FilterNullOptionType](./literals.md#filternulloptiontype) 
7. See [:material-code-braces: ExcludePeriodConfigurationTypeDef](./type_defs.md#excludeperiodconfigurationtypedef) 
## FilterOperationTargetVisualsConfigurationTypeDef

```python
# FilterOperationTargetVisualsConfigurationTypeDef definition

class FilterOperationTargetVisualsConfigurationTypeDef(TypedDict):
    SameSheetTargetVisualConfiguration: NotRequired[SameSheetTargetVisualConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SameSheetTargetVisualConfigurationTypeDef](./type_defs.md#samesheettargetvisualconfigurationtypedef) 
## SearchFoldersRequestRequestTypeDef

```python
# SearchFoldersRequestRequestTypeDef definition

class SearchFoldersRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Filters: Sequence[FolderSearchFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FolderSearchFilterTypeDef](./type_defs.md#foldersearchfiltertypedef) 
## ListFoldersResponseTypeDef

```python
# ListFoldersResponseTypeDef definition

class ListFoldersResponseTypeDef(TypedDict):
    Status: int,
    FolderSummaryList: List[FolderSummaryTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FolderSummaryTypeDef](./type_defs.md#foldersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchFoldersResponseTypeDef

```python
# SearchFoldersResponseTypeDef definition

class SearchFoldersResponseTypeDef(TypedDict):
    Status: int,
    FolderSummaryList: List[FolderSummaryTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FolderSummaryTypeDef](./type_defs.md#foldersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FontConfigurationTypeDef

```python
# FontConfigurationTypeDef definition

class FontConfigurationTypeDef(TypedDict):
    FontSize: NotRequired[FontSizeTypeDef],  # (1)
    FontDecoration: NotRequired[FontDecorationType],  # (2)
    FontColor: NotRequired[str],
    FontWeight: NotRequired[FontWeightTypeDef],  # (3)
    FontStyle: NotRequired[FontStyleType],  # (4)
```

1. See [:material-code-braces: FontSizeTypeDef](./type_defs.md#fontsizetypedef) 
2. See [:material-code-brackets: FontDecorationType](./literals.md#fontdecorationtype) 
3. See [:material-code-braces: FontWeightTypeDef](./type_defs.md#fontweighttypedef) 
4. See [:material-code-brackets: FontStyleType](./literals.md#fontstyletype) 
## TypographyTypeDef

```python
# TypographyTypeDef definition

class TypographyTypeDef(TypedDict):
    FontFamilies: NotRequired[Sequence[FontTypeDef]],  # (1)
```

1. See [:material-code-braces: FontTypeDef](./type_defs.md#fonttypedef) 
## FreeFormLayoutCanvasSizeOptionsTypeDef

```python
# FreeFormLayoutCanvasSizeOptionsTypeDef definition

class FreeFormLayoutCanvasSizeOptionsTypeDef(TypedDict):
    ScreenCanvasSizeOptions: NotRequired[FreeFormLayoutScreenCanvasSizeOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: FreeFormLayoutScreenCanvasSizeOptionsTypeDef](./type_defs.md#freeformlayoutscreencanvassizeoptionstypedef) 
## SnapshotAnonymousUserTypeDef

```python
# SnapshotAnonymousUserTypeDef definition

class SnapshotAnonymousUserTypeDef(TypedDict):
    RowLevelPermissionTags: NotRequired[Sequence[SessionTagTypeDef]],  # (1)
```

1. See [:material-code-braces: SessionTagTypeDef](./type_defs.md#sessiontagtypedef) 
## GeospatialWindowOptionsTypeDef

```python
# GeospatialWindowOptionsTypeDef definition

class GeospatialWindowOptionsTypeDef(TypedDict):
    Bounds: NotRequired[GeospatialCoordinateBoundsTypeDef],  # (1)
    MapZoomMode: NotRequired[MapZoomModeType],  # (2)
```

1. See [:material-code-braces: GeospatialCoordinateBoundsTypeDef](./type_defs.md#geospatialcoordinateboundstypedef) 
2. See [:material-code-brackets: MapZoomModeType](./literals.md#mapzoommodetype) 
## GeospatialHeatmapColorScaleTypeDef

```python
# GeospatialHeatmapColorScaleTypeDef definition

class GeospatialHeatmapColorScaleTypeDef(TypedDict):
    Colors: NotRequired[Sequence[GeospatialHeatmapDataColorTypeDef]],  # (1)
```

1. See [:material-code-braces: GeospatialHeatmapDataColorTypeDef](./type_defs.md#geospatialheatmapdatacolortypedef) 
## TableSideBorderOptionsTypeDef

```python
# TableSideBorderOptionsTypeDef definition

class TableSideBorderOptionsTypeDef(TypedDict):
    InnerVertical: NotRequired[TableBorderOptionsTypeDef],  # (1)
    InnerHorizontal: NotRequired[TableBorderOptionsTypeDef],  # (1)
    Left: NotRequired[TableBorderOptionsTypeDef],  # (1)
    Right: NotRequired[TableBorderOptionsTypeDef],  # (1)
    Top: NotRequired[TableBorderOptionsTypeDef],  # (1)
    Bottom: NotRequired[TableBorderOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: TableBorderOptionsTypeDef](./type_defs.md#tableborderoptionstypedef) 
2. See [:material-code-braces: TableBorderOptionsTypeDef](./type_defs.md#tableborderoptionstypedef) 
3. See [:material-code-braces: TableBorderOptionsTypeDef](./type_defs.md#tableborderoptionstypedef) 
4. See [:material-code-braces: TableBorderOptionsTypeDef](./type_defs.md#tableborderoptionstypedef) 
5. See [:material-code-braces: TableBorderOptionsTypeDef](./type_defs.md#tableborderoptionstypedef) 
6. See [:material-code-braces: TableBorderOptionsTypeDef](./type_defs.md#tableborderoptionstypedef) 
## GradientColorTypeDef

```python
# GradientColorTypeDef definition

class GradientColorTypeDef(TypedDict):
    Stops: NotRequired[Sequence[GradientStopTypeDef]],  # (1)
```

1. See [:material-code-braces: GradientStopTypeDef](./type_defs.md#gradientstoptypedef) 
## GridLayoutCanvasSizeOptionsTypeDef

```python
# GridLayoutCanvasSizeOptionsTypeDef definition

class GridLayoutCanvasSizeOptionsTypeDef(TypedDict):
    ScreenCanvasSizeOptions: NotRequired[GridLayoutScreenCanvasSizeOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: GridLayoutScreenCanvasSizeOptionsTypeDef](./type_defs.md#gridlayoutscreencanvassizeoptionstypedef) 
## SearchGroupsRequestRequestTypeDef

```python
# SearchGroupsRequestRequestTypeDef definition

class SearchGroupsRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: str,
    Filters: Sequence[GroupSearchFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: GroupSearchFilterTypeDef](./type_defs.md#groupsearchfiltertypedef) 
## ListIAMPolicyAssignmentsResponseTypeDef

```python
# ListIAMPolicyAssignmentsResponseTypeDef definition

class ListIAMPolicyAssignmentsResponseTypeDef(TypedDict):
    IAMPolicyAssignments: List[IAMPolicyAssignmentSummaryTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IAMPolicyAssignmentSummaryTypeDef](./type_defs.md#iampolicyassignmentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IncrementalRefreshTypeDef

```python
# IncrementalRefreshTypeDef definition

class IncrementalRefreshTypeDef(TypedDict):
    LookbackWindow: LookbackWindowTypeDef,  # (1)
```

1. See [:material-code-braces: LookbackWindowTypeDef](./type_defs.md#lookbackwindowtypedef) 
## IngestionTypeDef

```python
# IngestionTypeDef definition

class IngestionTypeDef(TypedDict):
    Arn: str,
    IngestionStatus: IngestionStatusType,  # (1)
    CreatedTime: datetime,
    IngestionId: NotRequired[str],
    ErrorInfo: NotRequired[ErrorInfoTypeDef],  # (2)
    RowInfo: NotRequired[RowInfoTypeDef],  # (3)
    QueueInfo: NotRequired[QueueInfoTypeDef],  # (4)
    IngestionTimeInSeconds: NotRequired[int],
    IngestionSizeInBytes: NotRequired[int],
    RequestSource: NotRequired[IngestionRequestSourceType],  # (5)
    RequestType: NotRequired[IngestionRequestTypeType],  # (6)
```

1. See [:material-code-brackets: IngestionStatusType](./literals.md#ingestionstatustype) 
2. See [:material-code-braces: ErrorInfoTypeDef](./type_defs.md#errorinfotypedef) 
3. See [:material-code-braces: RowInfoTypeDef](./type_defs.md#rowinfotypedef) 
4. See [:material-code-braces: QueueInfoTypeDef](./type_defs.md#queueinfotypedef) 
5. See [:material-code-brackets: IngestionRequestSourceType](./literals.md#ingestionrequestsourcetype) 
6. See [:material-code-brackets: IngestionRequestTypeType](./literals.md#ingestionrequesttypetype) 
## IntegerDatasetParameterTypeDef

```python
# IntegerDatasetParameterTypeDef definition

class IntegerDatasetParameterTypeDef(TypedDict):
    Id: str,
    Name: str,
    ValueType: DatasetParameterValueTypeType,  # (1)
    DefaultValues: NotRequired[IntegerDatasetParameterDefaultValuesTypeDef],  # (2)
```

1. See [:material-code-brackets: DatasetParameterValueTypeType](./literals.md#datasetparametervaluetypetype) 
2. See [:material-code-braces: IntegerDatasetParameterDefaultValuesTypeDef](./type_defs.md#integerdatasetparameterdefaultvaluestypedef) 
## JoinInstructionTypeDef

```python
# JoinInstructionTypeDef definition

class JoinInstructionTypeDef(TypedDict):
    LeftOperand: str,
    RightOperand: str,
    Type: JoinTypeType,  # (3)
    OnClause: str,
    LeftJoinKeyProperties: NotRequired[JoinKeyPropertiesTypeDef],  # (1)
    RightJoinKeyProperties: NotRequired[JoinKeyPropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: JoinKeyPropertiesTypeDef](./type_defs.md#joinkeypropertiestypedef) 
2. See [:material-code-braces: JoinKeyPropertiesTypeDef](./type_defs.md#joinkeypropertiestypedef) 
3. See [:material-code-brackets: JoinTypeType](./literals.md#jointypetype) 
## LineChartDefaultSeriesSettingsTypeDef

```python
# LineChartDefaultSeriesSettingsTypeDef definition

class LineChartDefaultSeriesSettingsTypeDef(TypedDict):
    AxisBinding: NotRequired[AxisBindingType],  # (1)
    LineStyleSettings: NotRequired[LineChartLineStyleSettingsTypeDef],  # (2)
    MarkerStyleSettings: NotRequired[LineChartMarkerStyleSettingsTypeDef],  # (3)
```

1. See [:material-code-brackets: AxisBindingType](./literals.md#axisbindingtype) 
2. See [:material-code-braces: LineChartLineStyleSettingsTypeDef](./type_defs.md#linechartlinestylesettingstypedef) 
3. See [:material-code-braces: LineChartMarkerStyleSettingsTypeDef](./type_defs.md#linechartmarkerstylesettingstypedef) 
## LineChartSeriesSettingsTypeDef

```python
# LineChartSeriesSettingsTypeDef definition

class LineChartSeriesSettingsTypeDef(TypedDict):
    LineStyleSettings: NotRequired[LineChartLineStyleSettingsTypeDef],  # (1)
    MarkerStyleSettings: NotRequired[LineChartMarkerStyleSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: LineChartLineStyleSettingsTypeDef](./type_defs.md#linechartlinestylesettingstypedef) 
2. See [:material-code-braces: LineChartMarkerStyleSettingsTypeDef](./type_defs.md#linechartmarkerstylesettingstypedef) 
## ListAnalysesRequestListAnalysesPaginateTypeDef

```python
# ListAnalysesRequestListAnalysesPaginateTypeDef definition

class ListAnalysesRequestListAnalysesPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetBundleExportJobsRequestListAssetBundleExportJobsPaginateTypeDef

```python
# ListAssetBundleExportJobsRequestListAssetBundleExportJobsPaginateTypeDef definition

class ListAssetBundleExportJobsRequestListAssetBundleExportJobsPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetBundleImportJobsRequestListAssetBundleImportJobsPaginateTypeDef

```python
# ListAssetBundleImportJobsRequestListAssetBundleImportJobsPaginateTypeDef definition

class ListAssetBundleImportJobsRequestListAssetBundleImportJobsPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDashboardVersionsRequestListDashboardVersionsPaginateTypeDef

```python
# ListDashboardVersionsRequestListDashboardVersionsPaginateTypeDef definition

class ListDashboardVersionsRequestListDashboardVersionsPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDashboardsRequestListDashboardsPaginateTypeDef

```python
# ListDashboardsRequestListDashboardsPaginateTypeDef definition

class ListDashboardsRequestListDashboardsPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSetsRequestListDataSetsPaginateTypeDef

```python
# ListDataSetsRequestListDataSetsPaginateTypeDef definition

class ListDataSetsRequestListDataSetsPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSourcesRequestListDataSourcesPaginateTypeDef

```python
# ListDataSourcesRequestListDataSourcesPaginateTypeDef definition

class ListDataSourcesRequestListDataSourcesPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef

```python
# ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef definition

class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(TypedDict):
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupsRequestListGroupsPaginateTypeDef

```python
# ListGroupsRequestListGroupsPaginateTypeDef definition

class ListGroupsRequestListGroupsPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIAMPolicyAssignmentsForUserRequestListIAMPolicyAssignmentsForUserPaginateTypeDef

```python
# ListIAMPolicyAssignmentsForUserRequestListIAMPolicyAssignmentsForUserPaginateTypeDef definition

class ListIAMPolicyAssignmentsForUserRequestListIAMPolicyAssignmentsForUserPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    UserName: str,
    Namespace: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIAMPolicyAssignmentsRequestListIAMPolicyAssignmentsPaginateTypeDef

```python
# ListIAMPolicyAssignmentsRequestListIAMPolicyAssignmentsPaginateTypeDef definition

class ListIAMPolicyAssignmentsRequestListIAMPolicyAssignmentsPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: str,
    AssignmentStatus: NotRequired[AssignmentStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIngestionsRequestListIngestionsPaginateTypeDef

```python
# ListIngestionsRequestListIngestionsPaginateTypeDef definition

class ListIngestionsRequestListIngestionsPaginateTypeDef(TypedDict):
    DataSetId: str,
    AwsAccountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNamespacesRequestListNamespacesPaginateTypeDef

```python
# ListNamespacesRequestListNamespacesPaginateTypeDef definition

class ListNamespacesRequestListNamespacesPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTemplateAliasesRequestListTemplateAliasesPaginateTypeDef

```python
# ListTemplateAliasesRequestListTemplateAliasesPaginateTypeDef definition

class ListTemplateAliasesRequestListTemplateAliasesPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTemplateVersionsRequestListTemplateVersionsPaginateTypeDef

```python
# ListTemplateVersionsRequestListTemplateVersionsPaginateTypeDef definition

class ListTemplateVersionsRequestListTemplateVersionsPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTemplatesRequestListTemplatesPaginateTypeDef

```python
# ListTemplatesRequestListTemplatesPaginateTypeDef definition

class ListTemplatesRequestListTemplatesPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThemeVersionsRequestListThemeVersionsPaginateTypeDef

```python
# ListThemeVersionsRequestListThemeVersionsPaginateTypeDef definition

class ListThemeVersionsRequestListThemeVersionsPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    ThemeId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThemesRequestListThemesPaginateTypeDef

```python
# ListThemesRequestListThemesPaginateTypeDef definition

class ListThemesRequestListThemesPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    Type: NotRequired[ThemeTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ThemeTypeType](./literals.md#themetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUserGroupsRequestListUserGroupsPaginateTypeDef

```python
# ListUserGroupsRequestListUserGroupsPaginateTypeDef definition

class ListUserGroupsRequestListUserGroupsPaginateTypeDef(TypedDict):
    UserName: str,
    AwsAccountId: str,
    Namespace: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsersRequestListUsersPaginateTypeDef

```python
# ListUsersRequestListUsersPaginateTypeDef definition

class ListUsersRequestListUsersPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchAnalysesRequestSearchAnalysesPaginateTypeDef

```python
# SearchAnalysesRequestSearchAnalysesPaginateTypeDef definition

class SearchAnalysesRequestSearchAnalysesPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    Filters: Sequence[AnalysisSearchFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AnalysisSearchFilterTypeDef](./type_defs.md#analysissearchfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchDashboardsRequestSearchDashboardsPaginateTypeDef

```python
# SearchDashboardsRequestSearchDashboardsPaginateTypeDef definition

class SearchDashboardsRequestSearchDashboardsPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    Filters: Sequence[DashboardSearchFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DashboardSearchFilterTypeDef](./type_defs.md#dashboardsearchfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchDataSetsRequestSearchDataSetsPaginateTypeDef

```python
# SearchDataSetsRequestSearchDataSetsPaginateTypeDef definition

class SearchDataSetsRequestSearchDataSetsPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    Filters: Sequence[DataSetSearchFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DataSetSearchFilterTypeDef](./type_defs.md#datasetsearchfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchDataSourcesRequestSearchDataSourcesPaginateTypeDef

```python
# SearchDataSourcesRequestSearchDataSourcesPaginateTypeDef definition

class SearchDataSourcesRequestSearchDataSourcesPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    Filters: Sequence[DataSourceSearchFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DataSourceSearchFilterTypeDef](./type_defs.md#datasourcesearchfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchGroupsRequestSearchGroupsPaginateTypeDef

```python
# SearchGroupsRequestSearchGroupsPaginateTypeDef definition

class SearchGroupsRequestSearchGroupsPaginateTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: str,
    Filters: Sequence[GroupSearchFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: GroupSearchFilterTypeDef](./type_defs.md#groupsearchfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFolderMembersResponseTypeDef

```python
# ListFolderMembersResponseTypeDef definition

class ListFolderMembersResponseTypeDef(TypedDict):
    Status: int,
    FolderMemberList: List[MemberIdArnPairTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberIdArnPairTypeDef](./type_defs.md#memberidarnpairtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTemplateVersionsResponseTypeDef

```python
# ListTemplateVersionsResponseTypeDef definition

class ListTemplateVersionsResponseTypeDef(TypedDict):
    TemplateVersionSummaryList: List[TemplateVersionSummaryTypeDef],  # (1)
    NextToken: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateVersionSummaryTypeDef](./type_defs.md#templateversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTemplatesResponseTypeDef

```python
# ListTemplatesResponseTypeDef definition

class ListTemplatesResponseTypeDef(TypedDict):
    TemplateSummaryList: List[TemplateSummaryTypeDef],  # (1)
    NextToken: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateSummaryTypeDef](./type_defs.md#templatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThemeVersionsResponseTypeDef

```python
# ListThemeVersionsResponseTypeDef definition

class ListThemeVersionsResponseTypeDef(TypedDict):
    ThemeVersionSummaryList: List[ThemeVersionSummaryTypeDef],  # (1)
    NextToken: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeVersionSummaryTypeDef](./type_defs.md#themeversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThemesResponseTypeDef

```python
# ListThemesResponseTypeDef definition

class ListThemesResponseTypeDef(TypedDict):
    ThemeSummaryList: List[ThemeSummaryTypeDef],  # (1)
    NextToken: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeSummaryTypeDef](./type_defs.md#themesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTopicsResponseTypeDef

```python
# ListTopicsResponseTypeDef definition

class ListTopicsResponseTypeDef(TypedDict):
    TopicsSummaries: List[TopicSummaryTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TopicSummaryTypeDef](./type_defs.md#topicsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VisualSubtitleLabelOptionsTypeDef

```python
# VisualSubtitleLabelOptionsTypeDef definition

class VisualSubtitleLabelOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    FormatText: NotRequired[LongFormatTextTypeDef],  # (2)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-braces: LongFormatTextTypeDef](./type_defs.md#longformattexttypedef) 
## S3ParametersTypeDef

```python
# S3ParametersTypeDef definition

class S3ParametersTypeDef(TypedDict):
    ManifestFileLocation: ManifestFileLocationTypeDef,  # (1)
    RoleArn: NotRequired[str],
```

1. See [:material-code-braces: ManifestFileLocationTypeDef](./type_defs.md#manifestfilelocationtypedef) 
## TileLayoutStyleTypeDef

```python
# TileLayoutStyleTypeDef definition

class TileLayoutStyleTypeDef(TypedDict):
    Gutter: NotRequired[GutterStyleTypeDef],  # (1)
    Margin: NotRequired[MarginStyleTypeDef],  # (2)
```

1. See [:material-code-braces: GutterStyleTypeDef](./type_defs.md#gutterstyletypedef) 
2. See [:material-code-braces: MarginStyleTypeDef](./type_defs.md#marginstyletypedef) 
## NamedEntityDefinitionTypeDef

```python
# NamedEntityDefinitionTypeDef definition

class NamedEntityDefinitionTypeDef(TypedDict):
    FieldName: NotRequired[str],
    PropertyName: NotRequired[str],
    PropertyRole: NotRequired[PropertyRoleType],  # (1)
    PropertyUsage: NotRequired[PropertyUsageType],  # (2)
    Metric: NotRequired[NamedEntityDefinitionMetricTypeDef],  # (3)
```

1. See [:material-code-brackets: PropertyRoleType](./literals.md#propertyroletype) 
2. See [:material-code-brackets: PropertyUsageType](./literals.md#propertyusagetype) 
3. See [:material-code-braces: NamedEntityDefinitionMetricTypeDef](./type_defs.md#namedentitydefinitionmetrictypedef) 
## NamespaceInfoV2TypeDef

```python
# NamespaceInfoV2TypeDef definition

class NamespaceInfoV2TypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
    CapacityRegion: NotRequired[str],
    CreationStatus: NotRequired[NamespaceStatusType],  # (1)
    IdentityStore: NotRequired[IdentityStoreType],  # (2)
    NamespaceError: NotRequired[NamespaceErrorTypeDef],  # (3)
```

1. See [:material-code-brackets: NamespaceStatusType](./literals.md#namespacestatustype) 
2. See [:material-code-brackets: IdentityStoreType](./literals.md#identitystoretype) 
3. See [:material-code-braces: NamespaceErrorTypeDef](./type_defs.md#namespaceerrortypedef) 
## VPCConnectionSummaryTypeDef

```python
# VPCConnectionSummaryTypeDef definition

class VPCConnectionSummaryTypeDef(TypedDict):
    VPCConnectionId: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    VPCId: NotRequired[str],
    SecurityGroupIds: NotRequired[List[str]],
    DnsResolvers: NotRequired[List[str]],
    Status: NotRequired[VPCConnectionResourceStatusType],  # (1)
    AvailabilityStatus: NotRequired[VPCConnectionAvailabilityStatusType],  # (2)
    NetworkInterfaces: NotRequired[List[NetworkInterfaceTypeDef]],  # (3)
    RoleArn: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: VPCConnectionResourceStatusType](./literals.md#vpcconnectionresourcestatustype) 
2. See [:material-code-brackets: VPCConnectionAvailabilityStatusType](./literals.md#vpcconnectionavailabilitystatustype) 
3. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
## VPCConnectionTypeDef

```python
# VPCConnectionTypeDef definition

class VPCConnectionTypeDef(TypedDict):
    VPCConnectionId: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    VPCId: NotRequired[str],
    SecurityGroupIds: NotRequired[List[str]],
    DnsResolvers: NotRequired[List[str]],
    Status: NotRequired[VPCConnectionResourceStatusType],  # (1)
    AvailabilityStatus: NotRequired[VPCConnectionAvailabilityStatusType],  # (2)
    NetworkInterfaces: NotRequired[List[NetworkInterfaceTypeDef]],  # (3)
    RoleArn: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: VPCConnectionResourceStatusType](./literals.md#vpcconnectionresourcestatustype) 
2. See [:material-code-brackets: VPCConnectionAvailabilityStatusType](./literals.md#vpcconnectionavailabilitystatustype) 
3. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
## NumericSeparatorConfigurationTypeDef

```python
# NumericSeparatorConfigurationTypeDef definition

class NumericSeparatorConfigurationTypeDef(TypedDict):
    DecimalSeparator: NotRequired[NumericSeparatorSymbolType],  # (1)
    ThousandsSeparator: NotRequired[ThousandSeparatorOptionsTypeDef],  # (2)
```

1. See [:material-code-brackets: NumericSeparatorSymbolType](./literals.md#numericseparatorsymboltype) 
2. See [:material-code-braces: ThousandSeparatorOptionsTypeDef](./type_defs.md#thousandseparatoroptionstypedef) 
## NumericalAggregationFunctionTypeDef

```python
# NumericalAggregationFunctionTypeDef definition

class NumericalAggregationFunctionTypeDef(TypedDict):
    SimpleNumericalAggregation: NotRequired[SimpleNumericalAggregationFunctionType],  # (1)
    PercentileAggregation: NotRequired[PercentileAggregationTypeDef],  # (2)
```

1. See [:material-code-brackets: SimpleNumericalAggregationFunctionType](./literals.md#simplenumericalaggregationfunctiontype) 
2. See [:material-code-braces: PercentileAggregationTypeDef](./type_defs.md#percentileaggregationtypedef) 
## VisibleRangeOptionsTypeDef

```python
# VisibleRangeOptionsTypeDef definition

class VisibleRangeOptionsTypeDef(TypedDict):
    PercentRange: NotRequired[PercentVisibleRangeTypeDef],  # (1)
```

1. See [:material-code-braces: PercentVisibleRangeTypeDef](./type_defs.md#percentvisiblerangetypedef) 
## RadarChartSeriesSettingsTypeDef

```python
# RadarChartSeriesSettingsTypeDef definition

class RadarChartSeriesSettingsTypeDef(TypedDict):
    AreaStyleSettings: NotRequired[RadarChartAreaStyleSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: RadarChartAreaStyleSettingsTypeDef](./type_defs.md#radarchartareastylesettingstypedef) 
## TopicRangeFilterConstantTypeDef

```python
# TopicRangeFilterConstantTypeDef definition

class TopicRangeFilterConstantTypeDef(TypedDict):
    ConstantType: NotRequired[ConstantTypeType],  # (1)
    RangeConstant: NotRequired[RangeConstantTypeDef],  # (2)
```

1. See [:material-code-brackets: ConstantTypeType](./literals.md#constanttypetype) 
2. See [:material-code-braces: RangeConstantTypeDef](./type_defs.md#rangeconstanttypedef) 
## RefreshFrequencyTypeDef

```python
# RefreshFrequencyTypeDef definition

class RefreshFrequencyTypeDef(TypedDict):
    Interval: RefreshIntervalType,  # (1)
    RefreshOnDay: NotRequired[ScheduleRefreshOnEntityTypeDef],  # (2)
    Timezone: NotRequired[str],
    TimeOfTheDay: NotRequired[str],
```

1. See [:material-code-brackets: RefreshIntervalType](./literals.md#refreshintervaltype) 
2. See [:material-code-braces: ScheduleRefreshOnEntityTypeDef](./type_defs.md#schedulerefreshonentitytypedef) 
## RegisteredUserConsoleFeatureConfigurationsTypeDef

```python
# RegisteredUserConsoleFeatureConfigurationsTypeDef definition

class RegisteredUserConsoleFeatureConfigurationsTypeDef(TypedDict):
    StatePersistence: NotRequired[StatePersistenceConfigurationsTypeDef],  # (1)
```

1. See [:material-code-braces: StatePersistenceConfigurationsTypeDef](./type_defs.md#statepersistenceconfigurationstypedef) 
## RegisteredUserDashboardFeatureConfigurationsTypeDef

```python
# RegisteredUserDashboardFeatureConfigurationsTypeDef definition

class RegisteredUserDashboardFeatureConfigurationsTypeDef(TypedDict):
    StatePersistence: NotRequired[StatePersistenceConfigurationsTypeDef],  # (1)
    Bookmarks: NotRequired[BookmarksConfigurationsTypeDef],  # (2)
```

1. See [:material-code-braces: StatePersistenceConfigurationsTypeDef](./type_defs.md#statepersistenceconfigurationstypedef) 
2. See [:material-code-braces: BookmarksConfigurationsTypeDef](./type_defs.md#bookmarksconfigurationstypedef) 
## RowLevelPermissionTagConfigurationTypeDef

```python
# RowLevelPermissionTagConfigurationTypeDef definition

class RowLevelPermissionTagConfigurationTypeDef(TypedDict):
    TagRules: Sequence[RowLevelPermissionTagRuleTypeDef],  # (2)
    Status: NotRequired[StatusType],  # (1)
    TagRuleConfigurations: NotRequired[Sequence[Sequence[str]]],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: RowLevelPermissionTagRuleTypeDef](./type_defs.md#rowlevelpermissiontagruletypedef) 
## SnapshotS3DestinationConfigurationTypeDef

```python
# SnapshotS3DestinationConfigurationTypeDef definition

class SnapshotS3DestinationConfigurationTypeDef(TypedDict):
    BucketConfiguration: NotRequired[S3BucketConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: S3BucketConfigurationTypeDef](./type_defs.md#s3bucketconfigurationtypedef) 
## S3SourceTypeDef

```python
# S3SourceTypeDef definition

class S3SourceTypeDef(TypedDict):
    DataSourceArn: str,
    InputColumns: Sequence[InputColumnTypeDef],  # (2)
    UploadSettings: NotRequired[UploadSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: UploadSettingsTypeDef](./type_defs.md#uploadsettingstypedef) 
2. See [:material-code-braces: InputColumnTypeDef](./type_defs.md#inputcolumntypedef) 
## SectionPageBreakConfigurationTypeDef

```python
# SectionPageBreakConfigurationTypeDef definition

class SectionPageBreakConfigurationTypeDef(TypedDict):
    After: NotRequired[SectionAfterPageBreakTypeDef],  # (1)
```

1. See [:material-code-braces: SectionAfterPageBreakTypeDef](./type_defs.md#sectionafterpagebreaktypedef) 
## SectionBasedLayoutPaperCanvasSizeOptionsTypeDef

```python
# SectionBasedLayoutPaperCanvasSizeOptionsTypeDef definition

class SectionBasedLayoutPaperCanvasSizeOptionsTypeDef(TypedDict):
    PaperSize: NotRequired[PaperSizeType],  # (1)
    PaperOrientation: NotRequired[PaperOrientationType],  # (2)
    PaperMargin: NotRequired[SpacingTypeDef],  # (3)
```

1. See [:material-code-brackets: PaperSizeType](./literals.md#papersizetype) 
2. See [:material-code-brackets: PaperOrientationType](./literals.md#paperorientationtype) 
3. See [:material-code-braces: SpacingTypeDef](./type_defs.md#spacingtypedef) 
## SectionStyleTypeDef

```python
# SectionStyleTypeDef definition

class SectionStyleTypeDef(TypedDict):
    Height: NotRequired[str],
    Padding: NotRequired[SpacingTypeDef],  # (1)
```

1. See [:material-code-braces: SpacingTypeDef](./type_defs.md#spacingtypedef) 
## SelectedSheetsFilterScopeConfigurationTypeDef

```python
# SelectedSheetsFilterScopeConfigurationTypeDef definition

class SelectedSheetsFilterScopeConfigurationTypeDef(TypedDict):
    SheetVisualScopingConfigurations: NotRequired[Sequence[SheetVisualScopingConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: SheetVisualScopingConfigurationTypeDef](./type_defs.md#sheetvisualscopingconfigurationtypedef) 
## SheetElementRenderingRuleTypeDef

```python
# SheetElementRenderingRuleTypeDef definition

class SheetElementRenderingRuleTypeDef(TypedDict):
    Expression: str,
    ConfigurationOverrides: SheetElementConfigurationOverridesTypeDef,  # (1)
```

1. See [:material-code-braces: SheetElementConfigurationOverridesTypeDef](./type_defs.md#sheetelementconfigurationoverridestypedef) 
## VisualTitleLabelOptionsTypeDef

```python
# VisualTitleLabelOptionsTypeDef definition

class VisualTitleLabelOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    FormatText: NotRequired[ShortFormatTextTypeDef],  # (2)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-braces: ShortFormatTextTypeDef](./type_defs.md#shortformattexttypedef) 
## SnapshotUserConfigurationRedactedTypeDef

```python
# SnapshotUserConfigurationRedactedTypeDef definition

class SnapshotUserConfigurationRedactedTypeDef(TypedDict):
    AnonymousUsers: NotRequired[List[SnapshotAnonymousUserRedactedTypeDef]],  # (1)
```

1. See [:material-code-braces: SnapshotAnonymousUserRedactedTypeDef](./type_defs.md#snapshotanonymoususerredactedtypedef) 
## SnapshotFileTypeDef

```python
# SnapshotFileTypeDef definition

class SnapshotFileTypeDef(TypedDict):
    SheetSelections: List[SnapshotFileSheetSelectionTypeDef],  # (1)
    FormatType: SnapshotFileFormatTypeType,  # (2)
```

1. See [:material-code-braces: SnapshotFileSheetSelectionTypeDef](./type_defs.md#snapshotfilesheetselectiontypedef) 
2. See [:material-code-brackets: SnapshotFileFormatTypeType](./literals.md#snapshotfileformattypetype) 
## StringDatasetParameterTypeDef

```python
# StringDatasetParameterTypeDef definition

class StringDatasetParameterTypeDef(TypedDict):
    Id: str,
    Name: str,
    ValueType: DatasetParameterValueTypeType,  # (1)
    DefaultValues: NotRequired[StringDatasetParameterDefaultValuesTypeDef],  # (2)
```

1. See [:material-code-brackets: DatasetParameterValueTypeType](./literals.md#datasetparametervaluetypetype) 
2. See [:material-code-braces: StringDatasetParameterDefaultValuesTypeDef](./type_defs.md#stringdatasetparameterdefaultvaluestypedef) 
## TableFieldImageConfigurationTypeDef

```python
# TableFieldImageConfigurationTypeDef definition

class TableFieldImageConfigurationTypeDef(TypedDict):
    SizingOptions: NotRequired[TableCellImageSizingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: TableCellImageSizingConfigurationTypeDef](./type_defs.md#tablecellimagesizingconfigurationtypedef) 
## TopicNumericEqualityFilterTypeDef

```python
# TopicNumericEqualityFilterTypeDef definition

class TopicNumericEqualityFilterTypeDef(TypedDict):
    Constant: NotRequired[TopicSingularFilterConstantTypeDef],  # (1)
    Aggregation: NotRequired[NamedFilterAggTypeType],  # (2)
```

1. See [:material-code-braces: TopicSingularFilterConstantTypeDef](./type_defs.md#topicsingularfilterconstanttypedef) 
2. See [:material-code-brackets: NamedFilterAggTypeType](./literals.md#namedfilteraggtypetype) 
## TopicRelativeDateFilterTypeDef

```python
# TopicRelativeDateFilterTypeDef definition

class TopicRelativeDateFilterTypeDef(TypedDict):
    TimeGranularity: NotRequired[TopicTimeGranularityType],  # (1)
    RelativeDateFilterFunction: NotRequired[TopicRelativeDateFilterFunctionType],  # (2)
    Constant: NotRequired[TopicSingularFilterConstantTypeDef],  # (3)
```

1. See [:material-code-brackets: TopicTimeGranularityType](./literals.md#topictimegranularitytype) 
2. See [:material-code-brackets: TopicRelativeDateFilterFunctionType](./literals.md#topicrelativedatefilterfunctiontype) 
3. See [:material-code-braces: TopicSingularFilterConstantTypeDef](./type_defs.md#topicsingularfilterconstanttypedef) 
## CascadingControlConfigurationTypeDef

```python
# CascadingControlConfigurationTypeDef definition

class CascadingControlConfigurationTypeDef(TypedDict):
    SourceControls: NotRequired[Sequence[CascadingControlSourceTypeDef]],  # (1)
```

1. See [:material-code-braces: CascadingControlSourceTypeDef](./type_defs.md#cascadingcontrolsourcetypedef) 
## DateTimeDefaultValuesTypeDef

```python
# DateTimeDefaultValuesTypeDef definition

class DateTimeDefaultValuesTypeDef(TypedDict):
    DynamicValue: NotRequired[DynamicDefaultValueTypeDef],  # (1)
    StaticValues: NotRequired[Sequence[Union[datetime, str]]],
    RollingDate: NotRequired[RollingDateConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: DynamicDefaultValueTypeDef](./type_defs.md#dynamicdefaultvaluetypedef) 
2. See [:material-code-braces: RollingDateConfigurationTypeDef](./type_defs.md#rollingdateconfigurationtypedef) 
## DecimalDefaultValuesTypeDef

```python
# DecimalDefaultValuesTypeDef definition

class DecimalDefaultValuesTypeDef(TypedDict):
    DynamicValue: NotRequired[DynamicDefaultValueTypeDef],  # (1)
    StaticValues: NotRequired[Sequence[float]],
```

1. See [:material-code-braces: DynamicDefaultValueTypeDef](./type_defs.md#dynamicdefaultvaluetypedef) 
## IntegerDefaultValuesTypeDef

```python
# IntegerDefaultValuesTypeDef definition

class IntegerDefaultValuesTypeDef(TypedDict):
    DynamicValue: NotRequired[DynamicDefaultValueTypeDef],  # (1)
    StaticValues: NotRequired[Sequence[int]],
```

1. See [:material-code-braces: DynamicDefaultValueTypeDef](./type_defs.md#dynamicdefaultvaluetypedef) 
## StringDefaultValuesTypeDef

```python
# StringDefaultValuesTypeDef definition

class StringDefaultValuesTypeDef(TypedDict):
    DynamicValue: NotRequired[DynamicDefaultValueTypeDef],  # (1)
    StaticValues: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: DynamicDefaultValueTypeDef](./type_defs.md#dynamicdefaultvaluetypedef) 
## AnalysisTypeDef

```python
# AnalysisTypeDef definition

class AnalysisTypeDef(TypedDict):
    AnalysisId: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[ResourceStatusType],  # (1)
    Errors: NotRequired[List[AnalysisErrorTypeDef]],  # (2)
    DataSetArns: NotRequired[List[str]],
    ThemeArn: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    Sheets: NotRequired[List[SheetTypeDef]],  # (3)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-braces: AnalysisErrorTypeDef](./type_defs.md#analysiserrortypedef) 
3. See [:material-code-braces: SheetTypeDef](./type_defs.md#sheettypedef) 
## DashboardVersionTypeDef

```python
# DashboardVersionTypeDef definition

class DashboardVersionTypeDef(TypedDict):
    CreatedTime: NotRequired[datetime],
    Errors: NotRequired[List[DashboardErrorTypeDef]],  # (1)
    VersionNumber: NotRequired[int],
    Status: NotRequired[ResourceStatusType],  # (2)
    Arn: NotRequired[str],
    SourceEntityArn: NotRequired[str],
    DataSetArns: NotRequired[List[str]],
    Description: NotRequired[str],
    ThemeArn: NotRequired[str],
    Sheets: NotRequired[List[SheetTypeDef]],  # (3)
```

1. See [:material-code-braces: DashboardErrorTypeDef](./type_defs.md#dashboarderrortypedef) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
3. See [:material-code-braces: SheetTypeDef](./type_defs.md#sheettypedef) 
## AnalysisSourceEntityTypeDef

```python
# AnalysisSourceEntityTypeDef definition

class AnalysisSourceEntityTypeDef(TypedDict):
    SourceTemplate: NotRequired[AnalysisSourceTemplateTypeDef],  # (1)
```

1. See [:material-code-braces: AnalysisSourceTemplateTypeDef](./type_defs.md#analysissourcetemplatetypedef) 
## DashboardSourceEntityTypeDef

```python
# DashboardSourceEntityTypeDef definition

class DashboardSourceEntityTypeDef(TypedDict):
    SourceTemplate: NotRequired[DashboardSourceTemplateTypeDef],  # (1)
```

1. See [:material-code-braces: DashboardSourceTemplateTypeDef](./type_defs.md#dashboardsourcetemplatetypedef) 
## TemplateSourceEntityTypeDef

```python
# TemplateSourceEntityTypeDef definition

class TemplateSourceEntityTypeDef(TypedDict):
    SourceAnalysis: NotRequired[TemplateSourceAnalysisTypeDef],  # (1)
    SourceTemplate: NotRequired[TemplateSourceTemplateTypeDef],  # (2)
```

1. See [:material-code-braces: TemplateSourceAnalysisTypeDef](./type_defs.md#templatesourceanalysistypedef) 
2. See [:material-code-braces: TemplateSourceTemplateTypeDef](./type_defs.md#templatesourcetemplatetypedef) 
## AnonymousUserEmbeddingExperienceConfigurationTypeDef

```python
# AnonymousUserEmbeddingExperienceConfigurationTypeDef definition

class AnonymousUserEmbeddingExperienceConfigurationTypeDef(TypedDict):
    Dashboard: NotRequired[AnonymousUserDashboardEmbeddingConfigurationTypeDef],  # (1)
    DashboardVisual: NotRequired[AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef],  # (2)
    QSearchBar: NotRequired[AnonymousUserQSearchBarEmbeddingConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: AnonymousUserDashboardEmbeddingConfigurationTypeDef](./type_defs.md#anonymoususerdashboardembeddingconfigurationtypedef) 
2. See [:material-code-braces: AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef](./type_defs.md#anonymoususerdashboardvisualembeddingconfigurationtypedef) 
3. See [:material-code-braces: AnonymousUserQSearchBarEmbeddingConfigurationTypeDef](./type_defs.md#anonymoususerqsearchbarembeddingconfigurationtypedef) 
## DescribeAssetBundleExportJobResponseTypeDef

```python
# DescribeAssetBundleExportJobResponseTypeDef definition

class DescribeAssetBundleExportJobResponseTypeDef(TypedDict):
    JobStatus: AssetBundleExportJobStatusType,  # (1)
    DownloadUrl: str,
    Errors: List[AssetBundleExportJobErrorTypeDef],  # (2)
    Arn: str,
    CreatedTime: datetime,
    AssetBundleExportJobId: str,
    AwsAccountId: str,
    ResourceArns: List[str],
    IncludeAllDependencies: bool,
    ExportFormat: AssetBundleExportFormatType,  # (3)
    CloudFormationOverridePropertyConfiguration: AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,  # (4)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: AssetBundleExportJobStatusType](./literals.md#assetbundleexportjobstatustype) 
2. See [:material-code-braces: AssetBundleExportJobErrorTypeDef](./type_defs.md#assetbundleexportjoberrortypedef) 
3. See [:material-code-brackets: AssetBundleExportFormatType](./literals.md#assetbundleexportformattype) 
4. See [:material-code-braces: AssetBundleCloudFormationOverridePropertyConfigurationTypeDef](./type_defs.md#assetbundlecloudformationoverridepropertyconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAssetBundleExportJobRequestRequestTypeDef

```python
# StartAssetBundleExportJobRequestRequestTypeDef definition

class StartAssetBundleExportJobRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AssetBundleExportJobId: str,
    ResourceArns: Sequence[str],
    ExportFormat: AssetBundleExportFormatType,  # (1)
    IncludeAllDependencies: NotRequired[bool],
    CloudFormationOverridePropertyConfiguration: NotRequired[AssetBundleCloudFormationOverridePropertyConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: AssetBundleExportFormatType](./literals.md#assetbundleexportformattype) 
2. See [:material-code-braces: AssetBundleCloudFormationOverridePropertyConfigurationTypeDef](./type_defs.md#assetbundlecloudformationoverridepropertyconfigurationtypedef) 
## NumericAxisOptionsTypeDef

```python
# NumericAxisOptionsTypeDef definition

class NumericAxisOptionsTypeDef(TypedDict):
    Scale: NotRequired[AxisScaleTypeDef],  # (1)
    Range: NotRequired[AxisDisplayRangeTypeDef],  # (2)
```

1. See [:material-code-braces: AxisScaleTypeDef](./type_defs.md#axisscaletypedef) 
2. See [:material-code-braces: AxisDisplayRangeTypeDef](./type_defs.md#axisdisplayrangetypedef) 
## CategoryFilterTypeDef

```python
# CategoryFilterTypeDef definition

class CategoryFilterTypeDef(TypedDict):
    FilterId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    Configuration: CategoryFilterConfigurationTypeDef,  # (2)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: CategoryFilterConfigurationTypeDef](./type_defs.md#categoryfilterconfigurationtypedef) 
## ClusterMarkerConfigurationTypeDef

```python
# ClusterMarkerConfigurationTypeDef definition

class ClusterMarkerConfigurationTypeDef(TypedDict):
    ClusterMarker: NotRequired[ClusterMarkerTypeDef],  # (1)
```

1. See [:material-code-braces: ClusterMarkerTypeDef](./type_defs.md#clustermarkertypedef) 
## TopicCategoryFilterTypeDef

```python
# TopicCategoryFilterTypeDef definition

class TopicCategoryFilterTypeDef(TypedDict):
    CategoryFilterFunction: NotRequired[CategoryFilterFunctionType],  # (1)
    CategoryFilterType: NotRequired[CategoryFilterTypeType],  # (2)
    Constant: NotRequired[TopicCategoryFilterConstantTypeDef],  # (3)
    Inverse: NotRequired[bool],
```

1. See [:material-code-brackets: CategoryFilterFunctionType](./literals.md#categoryfilterfunctiontype) 
2. See [:material-code-brackets: CategoryFilterTypeType](./literals.md#categoryfiltertypetype) 
3. See [:material-code-braces: TopicCategoryFilterConstantTypeDef](./type_defs.md#topiccategoryfilterconstanttypedef) 
## TagColumnOperationTypeDef

```python
# TagColumnOperationTypeDef definition

class TagColumnOperationTypeDef(TypedDict):
    ColumnName: str,
    Tags: Sequence[ColumnTagTypeDef],  # (1)
```

1. See [:material-code-braces: ColumnTagTypeDef](./type_defs.md#columntagtypedef) 
## DataSetConfigurationTypeDef

```python
# DataSetConfigurationTypeDef definition

class DataSetConfigurationTypeDef(TypedDict):
    Placeholder: NotRequired[str],
    DataSetSchema: NotRequired[DataSetSchemaTypeDef],  # (1)
    ColumnGroupSchemaList: NotRequired[Sequence[ColumnGroupSchemaTypeDef]],  # (2)
```

1. See [:material-code-braces: DataSetSchemaTypeDef](./type_defs.md#datasetschematypedef) 
2. See [:material-code-braces: ColumnGroupSchemaTypeDef](./type_defs.md#columngroupschematypedef) 
## ConditionalFormattingIconTypeDef

```python
# ConditionalFormattingIconTypeDef definition

class ConditionalFormattingIconTypeDef(TypedDict):
    IconSet: NotRequired[ConditionalFormattingIconSetTypeDef],  # (1)
    CustomCondition: NotRequired[ConditionalFormattingCustomIconConditionTypeDef],  # (2)
```

1. See [:material-code-braces: ConditionalFormattingIconSetTypeDef](./type_defs.md#conditionalformattingiconsettypedef) 
2. See [:material-code-braces: ConditionalFormattingCustomIconConditionTypeDef](./type_defs.md#conditionalformattingcustomiconconditiontypedef) 
## DescribeDashboardPermissionsResponseTypeDef

```python
# DescribeDashboardPermissionsResponseTypeDef definition

class DescribeDashboardPermissionsResponseTypeDef(TypedDict):
    DashboardId: str,
    DashboardArn: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    Status: int,
    RequestId: str,
    LinkSharingConfiguration: LinkSharingConfigurationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: LinkSharingConfigurationTypeDef](./type_defs.md#linksharingconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDashboardPermissionsResponseTypeDef

```python
# UpdateDashboardPermissionsResponseTypeDef definition

class UpdateDashboardPermissionsResponseTypeDef(TypedDict):
    DashboardArn: str,
    DashboardId: str,
    Permissions: List[ResourcePermissionTypeDef],  # (1)
    RequestId: str,
    Status: int,
    LinkSharingConfiguration: LinkSharingConfigurationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: LinkSharingConfigurationTypeDef](./type_defs.md#linksharingconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataSetsResponseTypeDef

```python
# ListDataSetsResponseTypeDef definition

class ListDataSetsResponseTypeDef(TypedDict):
    DataSetSummaries: List[DataSetSummaryTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSetSummaryTypeDef](./type_defs.md#datasetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchDataSetsResponseTypeDef

```python
# SearchDataSetsResponseTypeDef definition

class SearchDataSetsResponseTypeDef(TypedDict):
    DataSetSummaries: List[DataSetSummaryTypeDef],  # (1)
    NextToken: str,
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSetSummaryTypeDef](./type_defs.md#datasetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomValuesConfigurationTypeDef

```python
# CustomValuesConfigurationTypeDef definition

class CustomValuesConfigurationTypeDef(TypedDict):
    CustomValues: CustomParameterValuesTypeDef,  # (1)
    IncludeNullValue: NotRequired[bool],
```

1. See [:material-code-braces: CustomParameterValuesTypeDef](./type_defs.md#customparametervaluestypedef) 
## DateTimeDatasetParameterTypeDef

```python
# DateTimeDatasetParameterTypeDef definition

class DateTimeDatasetParameterTypeDef(TypedDict):
    Id: str,
    Name: str,
    ValueType: DatasetParameterValueTypeType,  # (1)
    TimeGranularity: NotRequired[TimeGranularityType],  # (2)
    DefaultValues: NotRequired[DateTimeDatasetParameterDefaultValuesTypeDef],  # (3)
```

1. See [:material-code-brackets: DatasetParameterValueTypeType](./literals.md#datasetparametervaluetypetype) 
2. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype) 
3. See [:material-code-braces: DateTimeDatasetParameterDefaultValuesTypeDef](./type_defs.md#datetimedatasetparameterdefaultvaluestypedef) 
## ParametersTypeDef

```python
# ParametersTypeDef definition

class ParametersTypeDef(TypedDict):
    StringParameters: NotRequired[Sequence[StringParameterTypeDef]],  # (1)
    IntegerParameters: NotRequired[Sequence[IntegerParameterTypeDef]],  # (2)
    DecimalParameters: NotRequired[Sequence[DecimalParameterTypeDef]],  # (3)
    DateTimeParameters: NotRequired[Sequence[DateTimeParameterTypeDef]],  # (4)
```

1. See [:material-code-braces: StringParameterTypeDef](./type_defs.md#stringparametertypedef) 
2. See [:material-code-braces: IntegerParameterTypeDef](./type_defs.md#integerparametertypedef) 
3. See [:material-code-braces: DecimalParameterTypeDef](./type_defs.md#decimalparametertypedef) 
4. See [:material-code-braces: DateTimeParameterTypeDef](./type_defs.md#datetimeparametertypedef) 
## OverrideDatasetParameterOperationTypeDef

```python
# OverrideDatasetParameterOperationTypeDef definition

class OverrideDatasetParameterOperationTypeDef(TypedDict):
    ParameterName: str,
    NewParameterName: NotRequired[str],
    NewDefaultValues: NotRequired[NewDefaultValuesTypeDef],  # (1)
```

1. See [:material-code-braces: NewDefaultValuesTypeDef](./type_defs.md#newdefaultvaluestypedef) 
## DrillDownFilterTypeDef

```python
# DrillDownFilterTypeDef definition

class DrillDownFilterTypeDef(TypedDict):
    NumericEqualityFilter: NotRequired[NumericEqualityDrillDownFilterTypeDef],  # (1)
    CategoryFilter: NotRequired[CategoryDrillDownFilterTypeDef],  # (2)
    TimeRangeFilter: NotRequired[TimeRangeDrillDownFilterTypeDef],  # (3)
```

1. See [:material-code-braces: NumericEqualityDrillDownFilterTypeDef](./type_defs.md#numericequalitydrilldownfiltertypedef) 
2. See [:material-code-braces: CategoryDrillDownFilterTypeDef](./type_defs.md#categorydrilldownfiltertypedef) 
3. See [:material-code-braces: TimeRangeDrillDownFilterTypeDef](./type_defs.md#timerangedrilldownfiltertypedef) 
## CreateTopicRefreshScheduleRequestRequestTypeDef

```python
# CreateTopicRefreshScheduleRequestRequestTypeDef definition

class CreateTopicRefreshScheduleRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TopicId: str,
    DatasetArn: str,
    RefreshSchedule: TopicRefreshScheduleTypeDef,  # (1)
    DatasetName: NotRequired[str],
```

1. See [:material-code-braces: TopicRefreshScheduleTypeDef](./type_defs.md#topicrefreshscheduletypedef) 
## DescribeTopicRefreshScheduleResponseTypeDef

```python
# DescribeTopicRefreshScheduleResponseTypeDef definition

class DescribeTopicRefreshScheduleResponseTypeDef(TypedDict):
    TopicId: str,
    TopicArn: str,
    DatasetArn: str,
    RefreshSchedule: TopicRefreshScheduleTypeDef,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TopicRefreshScheduleTypeDef](./type_defs.md#topicrefreshscheduletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TopicRefreshScheduleSummaryTypeDef

```python
# TopicRefreshScheduleSummaryTypeDef definition

class TopicRefreshScheduleSummaryTypeDef(TypedDict):
    DatasetId: NotRequired[str],
    DatasetArn: NotRequired[str],
    DatasetName: NotRequired[str],
    RefreshSchedule: NotRequired[TopicRefreshScheduleTypeDef],  # (1)
```

1. See [:material-code-braces: TopicRefreshScheduleTypeDef](./type_defs.md#topicrefreshscheduletypedef) 
## UpdateTopicRefreshScheduleRequestRequestTypeDef

```python
# UpdateTopicRefreshScheduleRequestRequestTypeDef definition

class UpdateTopicRefreshScheduleRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TopicId: str,
    DatasetId: str,
    RefreshSchedule: TopicRefreshScheduleTypeDef,  # (1)
```

1. See [:material-code-braces: TopicRefreshScheduleTypeDef](./type_defs.md#topicrefreshscheduletypedef) 
## ForecastScenarioTypeDef

```python
# ForecastScenarioTypeDef definition

class ForecastScenarioTypeDef(TypedDict):
    WhatIfPointScenario: NotRequired[WhatIfPointScenarioTypeDef],  # (1)
    WhatIfRangeScenario: NotRequired[WhatIfRangeScenarioTypeDef],  # (2)
```

1. See [:material-code-braces: WhatIfPointScenarioTypeDef](./type_defs.md#whatifpointscenariotypedef) 
2. See [:material-code-braces: WhatIfRangeScenarioTypeDef](./type_defs.md#whatifrangescenariotypedef) 
## DashboardPublishOptionsTypeDef

```python
# DashboardPublishOptionsTypeDef definition

class DashboardPublishOptionsTypeDef(TypedDict):
    AdHocFilteringOption: NotRequired[AdHocFilteringOptionTypeDef],  # (1)
    ExportToCSVOption: NotRequired[ExportToCSVOptionTypeDef],  # (2)
    SheetControlsOption: NotRequired[SheetControlsOptionTypeDef],  # (3)
    VisualPublishOptions: NotRequired[DashboardVisualPublishOptionsTypeDef],  # (4)
    SheetLayoutElementMaximizationOption: NotRequired[SheetLayoutElementMaximizationOptionTypeDef],  # (5)
    VisualMenuOption: NotRequired[VisualMenuOptionTypeDef],  # (6)
    VisualAxisSortOption: NotRequired[VisualAxisSortOptionTypeDef],  # (7)
    ExportWithHiddenFieldsOption: NotRequired[ExportWithHiddenFieldsOptionTypeDef],  # (8)
    DataPointDrillUpDownOption: NotRequired[DataPointDrillUpDownOptionTypeDef],  # (9)
    DataPointMenuLabelOption: NotRequired[DataPointMenuLabelOptionTypeDef],  # (10)
    DataPointTooltipOption: NotRequired[DataPointTooltipOptionTypeDef],  # (11)
```

1. See [:material-code-braces: AdHocFilteringOptionTypeDef](./type_defs.md#adhocfilteringoptiontypedef) 
2. See [:material-code-braces: ExportToCSVOptionTypeDef](./type_defs.md#exporttocsvoptiontypedef) 
3. See [:material-code-braces: SheetControlsOptionTypeDef](./type_defs.md#sheetcontrolsoptiontypedef) 
4. See [:material-code-braces: DashboardVisualPublishOptionsTypeDef](./type_defs.md#dashboardvisualpublishoptionstypedef) 
5. See [:material-code-braces: SheetLayoutElementMaximizationOptionTypeDef](./type_defs.md#sheetlayoutelementmaximizationoptiontypedef) 
6. See [:material-code-braces: VisualMenuOptionTypeDef](./type_defs.md#visualmenuoptiontypedef) 
7. See [:material-code-braces: VisualAxisSortOptionTypeDef](./type_defs.md#visualaxissortoptiontypedef) 
8. See [:material-code-braces: ExportWithHiddenFieldsOptionTypeDef](./type_defs.md#exportwithhiddenfieldsoptiontypedef) 
9. See [:material-code-braces: DataPointDrillUpDownOptionTypeDef](./type_defs.md#datapointdrillupdownoptiontypedef) 
10. See [:material-code-braces: DataPointMenuLabelOptionTypeDef](./type_defs.md#datapointmenulabeloptiontypedef) 
11. See [:material-code-braces: DataPointTooltipOptionTypeDef](./type_defs.md#datapointtooltipoptiontypedef) 
## VisualPaletteTypeDef

```python
# VisualPaletteTypeDef definition

class VisualPaletteTypeDef(TypedDict):
    ChartColor: NotRequired[str],
    ColorMap: NotRequired[Sequence[DataPathColorTypeDef]],  # (1)
```

1. See [:material-code-braces: DataPathColorTypeDef](./type_defs.md#datapathcolortypedef) 
## PivotTableFieldCollapseStateOptionTypeDef

```python
# PivotTableFieldCollapseStateOptionTypeDef definition

class PivotTableFieldCollapseStateOptionTypeDef(TypedDict):
    Target: PivotTableFieldCollapseStateTargetTypeDef,  # (1)
    State: NotRequired[PivotTableFieldCollapseStateType],  # (2)
```

1. See [:material-code-braces: PivotTableFieldCollapseStateTargetTypeDef](./type_defs.md#pivottablefieldcollapsestatetargettypedef) 
2. See [:material-code-brackets: PivotTableFieldCollapseStateType](./literals.md#pivottablefieldcollapsestatetype) 
## TimeRangeFilterTypeDef

```python
# TimeRangeFilterTypeDef definition

class TimeRangeFilterTypeDef(TypedDict):
    FilterId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    NullOption: FilterNullOptionType,  # (4)
    IncludeMinimum: NotRequired[bool],
    IncludeMaximum: NotRequired[bool],
    RangeMinimumValue: NotRequired[TimeRangeFilterValueTypeDef],  # (2)
    RangeMaximumValue: NotRequired[TimeRangeFilterValueTypeDef],  # (2)
    ExcludePeriodConfiguration: NotRequired[ExcludePeriodConfigurationTypeDef],  # (5)
    TimeGranularity: NotRequired[TimeGranularityType],  # (6)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: TimeRangeFilterValueTypeDef](./type_defs.md#timerangefiltervaluetypedef) 
3. See [:material-code-braces: TimeRangeFilterValueTypeDef](./type_defs.md#timerangefiltervaluetypedef) 
4. See [:material-code-brackets: FilterNullOptionType](./literals.md#filternulloptiontype) 
5. See [:material-code-braces: ExcludePeriodConfigurationTypeDef](./type_defs.md#excludeperiodconfigurationtypedef) 
6. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype) 
## DefaultFormattingTypeDef

```python
# DefaultFormattingTypeDef definition

class DefaultFormattingTypeDef(TypedDict):
    DisplayFormat: NotRequired[DisplayFormatType],  # (1)
    DisplayFormatOptions: NotRequired[DisplayFormatOptionsTypeDef],  # (2)
```

1. See [:material-code-brackets: DisplayFormatType](./literals.md#displayformattype) 
2. See [:material-code-braces: DisplayFormatOptionsTypeDef](./type_defs.md#displayformatoptionstypedef) 
## CustomActionFilterOperationTypeDef

```python
# CustomActionFilterOperationTypeDef definition

class CustomActionFilterOperationTypeDef(TypedDict):
    SelectedFieldsConfiguration: FilterOperationSelectedFieldsConfigurationTypeDef,  # (1)
    TargetVisualsConfiguration: FilterOperationTargetVisualsConfigurationTypeDef,  # (2)
```

1. See [:material-code-braces: FilterOperationSelectedFieldsConfigurationTypeDef](./type_defs.md#filteroperationselectedfieldsconfigurationtypedef) 
2. See [:material-code-braces: FilterOperationTargetVisualsConfigurationTypeDef](./type_defs.md#filteroperationtargetvisualsconfigurationtypedef) 
## AxisLabelOptionsTypeDef

```python
# AxisLabelOptionsTypeDef definition

class AxisLabelOptionsTypeDef(TypedDict):
    FontConfiguration: NotRequired[FontConfigurationTypeDef],  # (1)
    CustomLabel: NotRequired[str],
    ApplyTo: NotRequired[AxisLabelReferenceOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: FontConfigurationTypeDef](./type_defs.md#fontconfigurationtypedef) 
2. See [:material-code-braces: AxisLabelReferenceOptionsTypeDef](./type_defs.md#axislabelreferenceoptionstypedef) 
## DataLabelOptionsTypeDef

```python
# DataLabelOptionsTypeDef definition

class DataLabelOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    CategoryLabelVisibility: NotRequired[VisibilityType],  # (1)
    MeasureLabelVisibility: NotRequired[VisibilityType],  # (1)
    DataLabelTypes: NotRequired[Sequence[DataLabelTypeTypeDef]],  # (4)
    Position: NotRequired[DataLabelPositionType],  # (5)
    LabelContent: NotRequired[DataLabelContentType],  # (6)
    LabelFontConfiguration: NotRequired[FontConfigurationTypeDef],  # (7)
    LabelColor: NotRequired[str],
    Overlap: NotRequired[DataLabelOverlapType],  # (8)
    TotalsVisibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
3. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
4. See [:material-code-braces: DataLabelTypeTypeDef](./type_defs.md#datalabeltypetypedef) 
5. See [:material-code-brackets: DataLabelPositionType](./literals.md#datalabelpositiontype) 
6. See [:material-code-brackets: DataLabelContentType](./literals.md#datalabelcontenttype) 
7. See [:material-code-braces: FontConfigurationTypeDef](./type_defs.md#fontconfigurationtypedef) 
8. See [:material-code-brackets: DataLabelOverlapType](./literals.md#datalabeloverlaptype) 
9. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## FunnelChartDataLabelOptionsTypeDef

```python
# FunnelChartDataLabelOptionsTypeDef definition

class FunnelChartDataLabelOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    CategoryLabelVisibility: NotRequired[VisibilityType],  # (1)
    MeasureLabelVisibility: NotRequired[VisibilityType],  # (1)
    Position: NotRequired[DataLabelPositionType],  # (4)
    LabelFontConfiguration: NotRequired[FontConfigurationTypeDef],  # (5)
    LabelColor: NotRequired[str],
    MeasureDataLabelStyle: NotRequired[FunnelChartMeasureDataLabelStyleType],  # (6)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
3. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
4. See [:material-code-brackets: DataLabelPositionType](./literals.md#datalabelpositiontype) 
5. See [:material-code-braces: FontConfigurationTypeDef](./type_defs.md#fontconfigurationtypedef) 
6. See [:material-code-brackets: FunnelChartMeasureDataLabelStyleType](./literals.md#funnelchartmeasuredatalabelstyletype) 
## LabelOptionsTypeDef

```python
# LabelOptionsTypeDef definition

class LabelOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    FontConfiguration: NotRequired[FontConfigurationTypeDef],  # (2)
    CustomLabel: NotRequired[str],
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-braces: FontConfigurationTypeDef](./type_defs.md#fontconfigurationtypedef) 
## PanelTitleOptionsTypeDef

```python
# PanelTitleOptionsTypeDef definition

class PanelTitleOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    FontConfiguration: NotRequired[FontConfigurationTypeDef],  # (2)
    HorizontalTextAlignment: NotRequired[HorizontalTextAlignmentType],  # (3)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-braces: FontConfigurationTypeDef](./type_defs.md#fontconfigurationtypedef) 
3. See [:material-code-brackets: HorizontalTextAlignmentType](./literals.md#horizontaltextalignmenttype) 
## TableFieldCustomTextContentTypeDef

```python
# TableFieldCustomTextContentTypeDef definition

class TableFieldCustomTextContentTypeDef(TypedDict):
    FontConfiguration: FontConfigurationTypeDef,  # (1)
    Value: NotRequired[str],
```

1. See [:material-code-braces: FontConfigurationTypeDef](./type_defs.md#fontconfigurationtypedef) 
## DefaultFreeFormLayoutConfigurationTypeDef

```python
# DefaultFreeFormLayoutConfigurationTypeDef definition

class DefaultFreeFormLayoutConfigurationTypeDef(TypedDict):
    CanvasSizeOptions: FreeFormLayoutCanvasSizeOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: FreeFormLayoutCanvasSizeOptionsTypeDef](./type_defs.md#freeformlayoutcanvassizeoptionstypedef) 
## SnapshotUserConfigurationTypeDef

```python
# SnapshotUserConfigurationTypeDef definition

class SnapshotUserConfigurationTypeDef(TypedDict):
    AnonymousUsers: NotRequired[Sequence[SnapshotAnonymousUserTypeDef]],  # (1)
```

1. See [:material-code-braces: SnapshotAnonymousUserTypeDef](./type_defs.md#snapshotanonymoususertypedef) 
## GeospatialHeatmapConfigurationTypeDef

```python
# GeospatialHeatmapConfigurationTypeDef definition

class GeospatialHeatmapConfigurationTypeDef(TypedDict):
    HeatmapColor: NotRequired[GeospatialHeatmapColorScaleTypeDef],  # (1)
```

1. See [:material-code-braces: GeospatialHeatmapColorScaleTypeDef](./type_defs.md#geospatialheatmapcolorscaletypedef) 
## GlobalTableBorderOptionsTypeDef

```python
# GlobalTableBorderOptionsTypeDef definition

class GlobalTableBorderOptionsTypeDef(TypedDict):
    UniformBorder: NotRequired[TableBorderOptionsTypeDef],  # (1)
    SideSpecificBorder: NotRequired[TableSideBorderOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: TableBorderOptionsTypeDef](./type_defs.md#tableborderoptionstypedef) 
2. See [:material-code-braces: TableSideBorderOptionsTypeDef](./type_defs.md#tablesideborderoptionstypedef) 
## ConditionalFormattingGradientColorTypeDef

```python
# ConditionalFormattingGradientColorTypeDef definition

class ConditionalFormattingGradientColorTypeDef(TypedDict):
    Expression: str,
    Color: GradientColorTypeDef,  # (1)
```

1. See [:material-code-braces: GradientColorTypeDef](./type_defs.md#gradientcolortypedef) 
## DefaultGridLayoutConfigurationTypeDef

```python
# DefaultGridLayoutConfigurationTypeDef definition

class DefaultGridLayoutConfigurationTypeDef(TypedDict):
    CanvasSizeOptions: GridLayoutCanvasSizeOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: GridLayoutCanvasSizeOptionsTypeDef](./type_defs.md#gridlayoutcanvassizeoptionstypedef) 
## GridLayoutConfigurationTypeDef

```python
# GridLayoutConfigurationTypeDef definition

class GridLayoutConfigurationTypeDef(TypedDict):
    Elements: Sequence[GridLayoutElementTypeDef],  # (1)
    CanvasSizeOptions: NotRequired[GridLayoutCanvasSizeOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: GridLayoutElementTypeDef](./type_defs.md#gridlayoutelementtypedef) 
2. See [:material-code-braces: GridLayoutCanvasSizeOptionsTypeDef](./type_defs.md#gridlayoutcanvassizeoptionstypedef) 
## RefreshConfigurationTypeDef

```python
# RefreshConfigurationTypeDef definition

class RefreshConfigurationTypeDef(TypedDict):
    IncrementalRefresh: IncrementalRefreshTypeDef,  # (1)
```

1. See [:material-code-braces: IncrementalRefreshTypeDef](./type_defs.md#incrementalrefreshtypedef) 
## DescribeIngestionResponseTypeDef

```python
# DescribeIngestionResponseTypeDef definition

class DescribeIngestionResponseTypeDef(TypedDict):
    Ingestion: IngestionTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionTypeDef](./type_defs.md#ingestiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIngestionsResponseTypeDef

```python
# ListIngestionsResponseTypeDef definition

class ListIngestionsResponseTypeDef(TypedDict):
    Ingestions: List[IngestionTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionTypeDef](./type_defs.md#ingestiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LogicalTableSourceTypeDef

```python
# LogicalTableSourceTypeDef definition

class LogicalTableSourceTypeDef(TypedDict):
    JoinInstruction: NotRequired[JoinInstructionTypeDef],  # (1)
    PhysicalTableId: NotRequired[str],
    DataSetArn: NotRequired[str],
```

1. See [:material-code-braces: JoinInstructionTypeDef](./type_defs.md#joininstructiontypedef) 
## DataFieldSeriesItemTypeDef

```python
# DataFieldSeriesItemTypeDef definition

class DataFieldSeriesItemTypeDef(TypedDict):
    FieldId: str,
    AxisBinding: AxisBindingType,  # (1)
    FieldValue: NotRequired[str],
    Settings: NotRequired[LineChartSeriesSettingsTypeDef],  # (2)
```

1. See [:material-code-brackets: AxisBindingType](./literals.md#axisbindingtype) 
2. See [:material-code-braces: LineChartSeriesSettingsTypeDef](./type_defs.md#linechartseriessettingstypedef) 
## FieldSeriesItemTypeDef

```python
# FieldSeriesItemTypeDef definition

class FieldSeriesItemTypeDef(TypedDict):
    FieldId: str,
    AxisBinding: AxisBindingType,  # (1)
    Settings: NotRequired[LineChartSeriesSettingsTypeDef],  # (2)
```

1. See [:material-code-brackets: AxisBindingType](./literals.md#axisbindingtype) 
2. See [:material-code-braces: LineChartSeriesSettingsTypeDef](./type_defs.md#linechartseriessettingstypedef) 
## DataSourceParametersTypeDef

```python
# DataSourceParametersTypeDef definition

class DataSourceParametersTypeDef(TypedDict):
    AmazonElasticsearchParameters: NotRequired[AmazonElasticsearchParametersTypeDef],  # (1)
    AthenaParameters: NotRequired[AthenaParametersTypeDef],  # (2)
    AuroraParameters: NotRequired[AuroraParametersTypeDef],  # (3)
    AuroraPostgreSqlParameters: NotRequired[AuroraPostgreSqlParametersTypeDef],  # (4)
    AwsIotAnalyticsParameters: NotRequired[AwsIotAnalyticsParametersTypeDef],  # (5)
    JiraParameters: NotRequired[JiraParametersTypeDef],  # (6)
    MariaDbParameters: NotRequired[MariaDbParametersTypeDef],  # (7)
    MySqlParameters: NotRequired[MySqlParametersTypeDef],  # (8)
    OracleParameters: NotRequired[OracleParametersTypeDef],  # (9)
    PostgreSqlParameters: NotRequired[PostgreSqlParametersTypeDef],  # (10)
    PrestoParameters: NotRequired[PrestoParametersTypeDef],  # (11)
    RdsParameters: NotRequired[RdsParametersTypeDef],  # (12)
    RedshiftParameters: NotRequired[RedshiftParametersTypeDef],  # (13)
    S3Parameters: NotRequired[S3ParametersTypeDef],  # (14)
    ServiceNowParameters: NotRequired[ServiceNowParametersTypeDef],  # (15)
    SnowflakeParameters: NotRequired[SnowflakeParametersTypeDef],  # (16)
    SparkParameters: NotRequired[SparkParametersTypeDef],  # (17)
    SqlServerParameters: NotRequired[SqlServerParametersTypeDef],  # (18)
    TeradataParameters: NotRequired[TeradataParametersTypeDef],  # (19)
    TwitterParameters: NotRequired[TwitterParametersTypeDef],  # (20)
    AmazonOpenSearchParameters: NotRequired[AmazonOpenSearchParametersTypeDef],  # (21)
    ExasolParameters: NotRequired[ExasolParametersTypeDef],  # (22)
    DatabricksParameters: NotRequired[DatabricksParametersTypeDef],  # (23)
```

1. See [:material-code-braces: AmazonElasticsearchParametersTypeDef](./type_defs.md#amazonelasticsearchparameterstypedef) 
2. See [:material-code-braces: AthenaParametersTypeDef](./type_defs.md#athenaparameterstypedef) 
3. See [:material-code-braces: AuroraParametersTypeDef](./type_defs.md#auroraparameterstypedef) 
4. See [:material-code-braces: AuroraPostgreSqlParametersTypeDef](./type_defs.md#aurorapostgresqlparameterstypedef) 
5. See [:material-code-braces: AwsIotAnalyticsParametersTypeDef](./type_defs.md#awsiotanalyticsparameterstypedef) 
6. See [:material-code-braces: JiraParametersTypeDef](./type_defs.md#jiraparameterstypedef) 
7. See [:material-code-braces: MariaDbParametersTypeDef](./type_defs.md#mariadbparameterstypedef) 
8. See [:material-code-braces: MySqlParametersTypeDef](./type_defs.md#mysqlparameterstypedef) 
9. See [:material-code-braces: OracleParametersTypeDef](./type_defs.md#oracleparameterstypedef) 
10. See [:material-code-braces: PostgreSqlParametersTypeDef](./type_defs.md#postgresqlparameterstypedef) 
11. See [:material-code-braces: PrestoParametersTypeDef](./type_defs.md#prestoparameterstypedef) 
12. See [:material-code-braces: RdsParametersTypeDef](./type_defs.md#rdsparameterstypedef) 
13. See [:material-code-braces: RedshiftParametersTypeDef](./type_defs.md#redshiftparameterstypedef) 
14. See [:material-code-braces: S3ParametersTypeDef](./type_defs.md#s3parameterstypedef) 
15. See [:material-code-braces: ServiceNowParametersTypeDef](./type_defs.md#servicenowparameterstypedef) 
16. See [:material-code-braces: SnowflakeParametersTypeDef](./type_defs.md#snowflakeparameterstypedef) 
17. See [:material-code-braces: SparkParametersTypeDef](./type_defs.md#sparkparameterstypedef) 
18. See [:material-code-braces: SqlServerParametersTypeDef](./type_defs.md#sqlserverparameterstypedef) 
19. See [:material-code-braces: TeradataParametersTypeDef](./type_defs.md#teradataparameterstypedef) 
20. See [:material-code-braces: TwitterParametersTypeDef](./type_defs.md#twitterparameterstypedef) 
21. See [:material-code-braces: AmazonOpenSearchParametersTypeDef](./type_defs.md#amazonopensearchparameterstypedef) 
22. See [:material-code-braces: ExasolParametersTypeDef](./type_defs.md#exasolparameterstypedef) 
23. See [:material-code-braces: DatabricksParametersTypeDef](./type_defs.md#databricksparameterstypedef) 
## SheetStyleTypeDef

```python
# SheetStyleTypeDef definition

class SheetStyleTypeDef(TypedDict):
    Tile: NotRequired[TileStyleTypeDef],  # (1)
    TileLayout: NotRequired[TileLayoutStyleTypeDef],  # (2)
```

1. See [:material-code-braces: TileStyleTypeDef](./type_defs.md#tilestyletypedef) 
2. See [:material-code-braces: TileLayoutStyleTypeDef](./type_defs.md#tilelayoutstyletypedef) 
## TopicNamedEntityTypeDef

```python
# TopicNamedEntityTypeDef definition

class TopicNamedEntityTypeDef(TypedDict):
    EntityName: str,
    EntityDescription: NotRequired[str],
    EntitySynonyms: NotRequired[Sequence[str]],
    SemanticEntityType: NotRequired[SemanticEntityTypeTypeDef],  # (1)
    Definition: NotRequired[Sequence[NamedEntityDefinitionTypeDef]],  # (2)
```

1. See [:material-code-braces: SemanticEntityTypeTypeDef](./type_defs.md#semanticentitytypetypedef) 
2. See [:material-code-braces: NamedEntityDefinitionTypeDef](./type_defs.md#namedentitydefinitiontypedef) 
## DescribeNamespaceResponseTypeDef

```python
# DescribeNamespaceResponseTypeDef definition

class DescribeNamespaceResponseTypeDef(TypedDict):
    Namespace: NamespaceInfoV2TypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NamespaceInfoV2TypeDef](./type_defs.md#namespaceinfov2typedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNamespacesResponseTypeDef

```python
# ListNamespacesResponseTypeDef definition

class ListNamespacesResponseTypeDef(TypedDict):
    Namespaces: List[NamespaceInfoV2TypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NamespaceInfoV2TypeDef](./type_defs.md#namespaceinfov2typedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVPCConnectionsResponseTypeDef

```python
# ListVPCConnectionsResponseTypeDef definition

class ListVPCConnectionsResponseTypeDef(TypedDict):
    VPCConnectionSummaries: List[VPCConnectionSummaryTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VPCConnectionSummaryTypeDef](./type_defs.md#vpcconnectionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVPCConnectionResponseTypeDef

```python
# DescribeVPCConnectionResponseTypeDef definition

class DescribeVPCConnectionResponseTypeDef(TypedDict):
    VPCConnection: VPCConnectionTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VPCConnectionTypeDef](./type_defs.md#vpcconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CurrencyDisplayFormatConfigurationTypeDef

```python
# CurrencyDisplayFormatConfigurationTypeDef definition

class CurrencyDisplayFormatConfigurationTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Suffix: NotRequired[str],
    SeparatorConfiguration: NotRequired[NumericSeparatorConfigurationTypeDef],  # (1)
    Symbol: NotRequired[str],
    DecimalPlacesConfiguration: NotRequired[DecimalPlacesConfigurationTypeDef],  # (2)
    NumberScale: NotRequired[NumberScaleType],  # (3)
    NegativeValueConfiguration: NotRequired[NegativeValueConfigurationTypeDef],  # (4)
    NullValueFormatConfiguration: NotRequired[NullValueFormatConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: NumericSeparatorConfigurationTypeDef](./type_defs.md#numericseparatorconfigurationtypedef) 
2. See [:material-code-braces: DecimalPlacesConfigurationTypeDef](./type_defs.md#decimalplacesconfigurationtypedef) 
3. See [:material-code-brackets: NumberScaleType](./literals.md#numberscaletype) 
4. See [:material-code-braces: NegativeValueConfigurationTypeDef](./type_defs.md#negativevalueconfigurationtypedef) 
5. See [:material-code-braces: NullValueFormatConfigurationTypeDef](./type_defs.md#nullvalueformatconfigurationtypedef) 
## NumberDisplayFormatConfigurationTypeDef

```python
# NumberDisplayFormatConfigurationTypeDef definition

class NumberDisplayFormatConfigurationTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Suffix: NotRequired[str],
    SeparatorConfiguration: NotRequired[NumericSeparatorConfigurationTypeDef],  # (1)
    DecimalPlacesConfiguration: NotRequired[DecimalPlacesConfigurationTypeDef],  # (2)
    NumberScale: NotRequired[NumberScaleType],  # (3)
    NegativeValueConfiguration: NotRequired[NegativeValueConfigurationTypeDef],  # (4)
    NullValueFormatConfiguration: NotRequired[NullValueFormatConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: NumericSeparatorConfigurationTypeDef](./type_defs.md#numericseparatorconfigurationtypedef) 
2. See [:material-code-braces: DecimalPlacesConfigurationTypeDef](./type_defs.md#decimalplacesconfigurationtypedef) 
3. See [:material-code-brackets: NumberScaleType](./literals.md#numberscaletype) 
4. See [:material-code-braces: NegativeValueConfigurationTypeDef](./type_defs.md#negativevalueconfigurationtypedef) 
5. See [:material-code-braces: NullValueFormatConfigurationTypeDef](./type_defs.md#nullvalueformatconfigurationtypedef) 
## PercentageDisplayFormatConfigurationTypeDef

```python
# PercentageDisplayFormatConfigurationTypeDef definition

class PercentageDisplayFormatConfigurationTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Suffix: NotRequired[str],
    SeparatorConfiguration: NotRequired[NumericSeparatorConfigurationTypeDef],  # (1)
    DecimalPlacesConfiguration: NotRequired[DecimalPlacesConfigurationTypeDef],  # (2)
    NegativeValueConfiguration: NotRequired[NegativeValueConfigurationTypeDef],  # (3)
    NullValueFormatConfiguration: NotRequired[NullValueFormatConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: NumericSeparatorConfigurationTypeDef](./type_defs.md#numericseparatorconfigurationtypedef) 
2. See [:material-code-braces: DecimalPlacesConfigurationTypeDef](./type_defs.md#decimalplacesconfigurationtypedef) 
3. See [:material-code-braces: NegativeValueConfigurationTypeDef](./type_defs.md#negativevalueconfigurationtypedef) 
4. See [:material-code-braces: NullValueFormatConfigurationTypeDef](./type_defs.md#nullvalueformatconfigurationtypedef) 
## AggregationFunctionTypeDef

```python
# AggregationFunctionTypeDef definition

class AggregationFunctionTypeDef(TypedDict):
    NumericalAggregationFunction: NotRequired[NumericalAggregationFunctionTypeDef],  # (1)
    CategoricalAggregationFunction: NotRequired[CategoricalAggregationFunctionType],  # (2)
    DateAggregationFunction: NotRequired[DateAggregationFunctionType],  # (3)
    AttributeAggregationFunction: NotRequired[AttributeAggregationFunctionTypeDef],  # (4)
```

1. See [:material-code-braces: NumericalAggregationFunctionTypeDef](./type_defs.md#numericalaggregationfunctiontypedef) 
2. See [:material-code-brackets: CategoricalAggregationFunctionType](./literals.md#categoricalaggregationfunctiontype) 
3. See [:material-code-brackets: DateAggregationFunctionType](./literals.md#dateaggregationfunctiontype) 
4. See [:material-code-braces: AttributeAggregationFunctionTypeDef](./type_defs.md#attributeaggregationfunctiontypedef) 
## ScrollBarOptionsTypeDef

```python
# ScrollBarOptionsTypeDef definition

class ScrollBarOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    VisibleRange: NotRequired[VisibleRangeOptionsTypeDef],  # (2)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-braces: VisibleRangeOptionsTypeDef](./type_defs.md#visiblerangeoptionstypedef) 
## TopicDateRangeFilterTypeDef

```python
# TopicDateRangeFilterTypeDef definition

class TopicDateRangeFilterTypeDef(TypedDict):
    Inclusive: NotRequired[bool],
    Constant: NotRequired[TopicRangeFilterConstantTypeDef],  # (1)
```

1. See [:material-code-braces: TopicRangeFilterConstantTypeDef](./type_defs.md#topicrangefilterconstanttypedef) 
## TopicNumericRangeFilterTypeDef

```python
# TopicNumericRangeFilterTypeDef definition

class TopicNumericRangeFilterTypeDef(TypedDict):
    Inclusive: NotRequired[bool],
    Constant: NotRequired[TopicRangeFilterConstantTypeDef],  # (1)
    Aggregation: NotRequired[NamedFilterAggTypeType],  # (2)
```

1. See [:material-code-braces: TopicRangeFilterConstantTypeDef](./type_defs.md#topicrangefilterconstanttypedef) 
2. See [:material-code-brackets: NamedFilterAggTypeType](./literals.md#namedfilteraggtypetype) 
## RefreshScheduleTypeDef

```python
# RefreshScheduleTypeDef definition

class RefreshScheduleTypeDef(TypedDict):
    ScheduleId: str,
    ScheduleFrequency: RefreshFrequencyTypeDef,  # (1)
    RefreshType: IngestionTypeType,  # (2)
    StartAfterDateTime: NotRequired[Union[datetime, str]],
    Arn: NotRequired[str],
```

1. See [:material-code-braces: RefreshFrequencyTypeDef](./type_defs.md#refreshfrequencytypedef) 
2. See [:material-code-brackets: IngestionTypeType](./literals.md#ingestiontypetype) 
## RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef

```python
# RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef definition

class RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef(TypedDict):
    InitialPath: NotRequired[str],
    FeatureConfigurations: NotRequired[RegisteredUserConsoleFeatureConfigurationsTypeDef],  # (1)
```

1. See [:material-code-braces: RegisteredUserConsoleFeatureConfigurationsTypeDef](./type_defs.md#registereduserconsolefeatureconfigurationstypedef) 
## RegisteredUserDashboardEmbeddingConfigurationTypeDef

```python
# RegisteredUserDashboardEmbeddingConfigurationTypeDef definition

class RegisteredUserDashboardEmbeddingConfigurationTypeDef(TypedDict):
    InitialDashboardId: str,
    FeatureConfigurations: NotRequired[RegisteredUserDashboardFeatureConfigurationsTypeDef],  # (1)
```

1. See [:material-code-braces: RegisteredUserDashboardFeatureConfigurationsTypeDef](./type_defs.md#registereduserdashboardfeatureconfigurationstypedef) 
## SnapshotDestinationConfigurationTypeDef

```python
# SnapshotDestinationConfigurationTypeDef definition

class SnapshotDestinationConfigurationTypeDef(TypedDict):
    S3Destinations: NotRequired[List[SnapshotS3DestinationConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: SnapshotS3DestinationConfigurationTypeDef](./type_defs.md#snapshots3destinationconfigurationtypedef) 
## SnapshotJobS3ResultTypeDef

```python
# SnapshotJobS3ResultTypeDef definition

class SnapshotJobS3ResultTypeDef(TypedDict):
    S3DestinationConfiguration: NotRequired[SnapshotS3DestinationConfigurationTypeDef],  # (1)
    S3Uri: NotRequired[str],
    ErrorInfo: NotRequired[List[SnapshotJobResultErrorInfoTypeDef]],  # (2)
```

1. See [:material-code-braces: SnapshotS3DestinationConfigurationTypeDef](./type_defs.md#snapshots3destinationconfigurationtypedef) 
2. See [:material-code-braces: SnapshotJobResultErrorInfoTypeDef](./type_defs.md#snapshotjobresulterrorinfotypedef) 
## PhysicalTableTypeDef

```python
# PhysicalTableTypeDef definition

class PhysicalTableTypeDef(TypedDict):
    RelationalTable: NotRequired[RelationalTableTypeDef],  # (1)
    CustomSql: NotRequired[CustomSqlTypeDef],  # (2)
    S3Source: NotRequired[S3SourceTypeDef],  # (3)
```

1. See [:material-code-braces: RelationalTableTypeDef](./type_defs.md#relationaltabletypedef) 
2. See [:material-code-braces: CustomSqlTypeDef](./type_defs.md#customsqltypedef) 
3. See [:material-code-braces: S3SourceTypeDef](./type_defs.md#s3sourcetypedef) 
## SectionBasedLayoutCanvasSizeOptionsTypeDef

```python
# SectionBasedLayoutCanvasSizeOptionsTypeDef definition

class SectionBasedLayoutCanvasSizeOptionsTypeDef(TypedDict):
    PaperCanvasSizeOptions: NotRequired[SectionBasedLayoutPaperCanvasSizeOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: SectionBasedLayoutPaperCanvasSizeOptionsTypeDef](./type_defs.md#sectionbasedlayoutpapercanvassizeoptionstypedef) 
## FilterScopeConfigurationTypeDef

```python
# FilterScopeConfigurationTypeDef definition

class FilterScopeConfigurationTypeDef(TypedDict):
    SelectedSheets: NotRequired[SelectedSheetsFilterScopeConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SelectedSheetsFilterScopeConfigurationTypeDef](./type_defs.md#selectedsheetsfilterscopeconfigurationtypedef) 
## FreeFormLayoutElementTypeDef

```python
# FreeFormLayoutElementTypeDef definition

class FreeFormLayoutElementTypeDef(TypedDict):
    ElementId: str,
    ElementType: LayoutElementTypeType,  # (1)
    XAxisLocation: str,
    YAxisLocation: str,
    Width: str,
    Height: str,
    Visibility: NotRequired[VisibilityType],  # (2)
    RenderingRules: NotRequired[Sequence[SheetElementRenderingRuleTypeDef]],  # (3)
    BorderStyle: NotRequired[FreeFormLayoutElementBorderStyleTypeDef],  # (4)
    SelectedBorderStyle: NotRequired[FreeFormLayoutElementBorderStyleTypeDef],  # (4)
    BackgroundStyle: NotRequired[FreeFormLayoutElementBackgroundStyleTypeDef],  # (6)
    LoadingAnimation: NotRequired[LoadingAnimationTypeDef],  # (7)
```

1. See [:material-code-brackets: LayoutElementTypeType](./literals.md#layoutelementtypetype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
3. See [:material-code-braces: SheetElementRenderingRuleTypeDef](./type_defs.md#sheetelementrenderingruletypedef) 
4. See [:material-code-braces: FreeFormLayoutElementBorderStyleTypeDef](./type_defs.md#freeformlayoutelementborderstyletypedef) 
5. See [:material-code-braces: FreeFormLayoutElementBorderStyleTypeDef](./type_defs.md#freeformlayoutelementborderstyletypedef) 
6. See [:material-code-braces: FreeFormLayoutElementBackgroundStyleTypeDef](./type_defs.md#freeformlayoutelementbackgroundstyletypedef) 
7. See [:material-code-braces: LoadingAnimationTypeDef](./type_defs.md#loadinganimationtypedef) 
## SnapshotFileGroupTypeDef

```python
# SnapshotFileGroupTypeDef definition

class SnapshotFileGroupTypeDef(TypedDict):
    Files: NotRequired[List[SnapshotFileTypeDef]],  # (1)
```

1. See [:material-code-braces: SnapshotFileTypeDef](./type_defs.md#snapshotfiletypedef) 
## DateTimeParameterDeclarationTypeDef

```python
# DateTimeParameterDeclarationTypeDef definition

class DateTimeParameterDeclarationTypeDef(TypedDict):
    Name: str,
    DefaultValues: NotRequired[DateTimeDefaultValuesTypeDef],  # (1)
    TimeGranularity: NotRequired[TimeGranularityType],  # (2)
    ValueWhenUnset: NotRequired[DateTimeValueWhenUnsetConfigurationTypeDef],  # (3)
    MappedDataSetParameters: NotRequired[Sequence[MappedDataSetParameterTypeDef]],  # (4)
```

1. See [:material-code-braces: DateTimeDefaultValuesTypeDef](./type_defs.md#datetimedefaultvaluestypedef) 
2. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype) 
3. See [:material-code-braces: DateTimeValueWhenUnsetConfigurationTypeDef](./type_defs.md#datetimevaluewhenunsetconfigurationtypedef) 
4. See [:material-code-braces: MappedDataSetParameterTypeDef](./type_defs.md#mappeddatasetparametertypedef) 
## DecimalParameterDeclarationTypeDef

```python
# DecimalParameterDeclarationTypeDef definition

class DecimalParameterDeclarationTypeDef(TypedDict):
    ParameterValueType: ParameterValueTypeType,  # (1)
    Name: str,
    DefaultValues: NotRequired[DecimalDefaultValuesTypeDef],  # (2)
    ValueWhenUnset: NotRequired[DecimalValueWhenUnsetConfigurationTypeDef],  # (3)
    MappedDataSetParameters: NotRequired[Sequence[MappedDataSetParameterTypeDef]],  # (4)
```

1. See [:material-code-brackets: ParameterValueTypeType](./literals.md#parametervaluetypetype) 
2. See [:material-code-braces: DecimalDefaultValuesTypeDef](./type_defs.md#decimaldefaultvaluestypedef) 
3. See [:material-code-braces: DecimalValueWhenUnsetConfigurationTypeDef](./type_defs.md#decimalvaluewhenunsetconfigurationtypedef) 
4. See [:material-code-braces: MappedDataSetParameterTypeDef](./type_defs.md#mappeddatasetparametertypedef) 
## IntegerParameterDeclarationTypeDef

```python
# IntegerParameterDeclarationTypeDef definition

class IntegerParameterDeclarationTypeDef(TypedDict):
    ParameterValueType: ParameterValueTypeType,  # (1)
    Name: str,
    DefaultValues: NotRequired[IntegerDefaultValuesTypeDef],  # (2)
    ValueWhenUnset: NotRequired[IntegerValueWhenUnsetConfigurationTypeDef],  # (3)
    MappedDataSetParameters: NotRequired[Sequence[MappedDataSetParameterTypeDef]],  # (4)
```

1. See [:material-code-brackets: ParameterValueTypeType](./literals.md#parametervaluetypetype) 
2. See [:material-code-braces: IntegerDefaultValuesTypeDef](./type_defs.md#integerdefaultvaluestypedef) 
3. See [:material-code-braces: IntegerValueWhenUnsetConfigurationTypeDef](./type_defs.md#integervaluewhenunsetconfigurationtypedef) 
4. See [:material-code-braces: MappedDataSetParameterTypeDef](./type_defs.md#mappeddatasetparametertypedef) 
## StringParameterDeclarationTypeDef

```python
# StringParameterDeclarationTypeDef definition

class StringParameterDeclarationTypeDef(TypedDict):
    ParameterValueType: ParameterValueTypeType,  # (1)
    Name: str,
    DefaultValues: NotRequired[StringDefaultValuesTypeDef],  # (2)
    ValueWhenUnset: NotRequired[StringValueWhenUnsetConfigurationTypeDef],  # (3)
    MappedDataSetParameters: NotRequired[Sequence[MappedDataSetParameterTypeDef]],  # (4)
```

1. See [:material-code-brackets: ParameterValueTypeType](./literals.md#parametervaluetypetype) 
2. See [:material-code-braces: StringDefaultValuesTypeDef](./type_defs.md#stringdefaultvaluestypedef) 
3. See [:material-code-braces: StringValueWhenUnsetConfigurationTypeDef](./type_defs.md#stringvaluewhenunsetconfigurationtypedef) 
4. See [:material-code-braces: MappedDataSetParameterTypeDef](./type_defs.md#mappeddatasetparametertypedef) 
## DescribeAnalysisResponseTypeDef

```python
# DescribeAnalysisResponseTypeDef definition

class DescribeAnalysisResponseTypeDef(TypedDict):
    Analysis: AnalysisTypeDef,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisTypeDef](./type_defs.md#analysistypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DashboardTypeDef

```python
# DashboardTypeDef definition

class DashboardTypeDef(TypedDict):
    DashboardId: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Version: NotRequired[DashboardVersionTypeDef],  # (1)
    CreatedTime: NotRequired[datetime],
    LastPublishedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-braces: DashboardVersionTypeDef](./type_defs.md#dashboardversiontypedef) 
## GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef

```python
# GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef definition

class GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    Namespace: str,
    AuthorizedResourceArns: Sequence[str],
    ExperienceConfiguration: AnonymousUserEmbeddingExperienceConfigurationTypeDef,  # (1)
    SessionLifetimeInMinutes: NotRequired[int],
    SessionTags: NotRequired[Sequence[SessionTagTypeDef]],  # (2)
    AllowedDomains: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: AnonymousUserEmbeddingExperienceConfigurationTypeDef](./type_defs.md#anonymoususerembeddingexperienceconfigurationtypedef) 
2. See [:material-code-braces: SessionTagTypeDef](./type_defs.md#sessiontagtypedef) 
## AxisDataOptionsTypeDef

```python
# AxisDataOptionsTypeDef definition

class AxisDataOptionsTypeDef(TypedDict):
    NumericAxisOptions: NotRequired[NumericAxisOptionsTypeDef],  # (1)
    DateAxisOptions: NotRequired[DateAxisOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: NumericAxisOptionsTypeDef](./type_defs.md#numericaxisoptionstypedef) 
2. See [:material-code-braces: DateAxisOptionsTypeDef](./type_defs.md#dateaxisoptionstypedef) 
## TemplateVersionTypeDef

```python
# TemplateVersionTypeDef definition

class TemplateVersionTypeDef(TypedDict):
    CreatedTime: NotRequired[datetime],
    Errors: NotRequired[List[TemplateErrorTypeDef]],  # (1)
    VersionNumber: NotRequired[int],
    Status: NotRequired[ResourceStatusType],  # (2)
    DataSetConfigurations: NotRequired[List[DataSetConfigurationTypeDef]],  # (3)
    Description: NotRequired[str],
    SourceEntityArn: NotRequired[str],
    ThemeArn: NotRequired[str],
    Sheets: NotRequired[List[SheetTypeDef]],  # (4)
```

1. See [:material-code-braces: TemplateErrorTypeDef](./type_defs.md#templateerrortypedef) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
3. See [:material-code-braces: DataSetConfigurationTypeDef](./type_defs.md#datasetconfigurationtypedef) 
4. See [:material-code-braces: SheetTypeDef](./type_defs.md#sheettypedef) 
## DestinationParameterValueConfigurationTypeDef

```python
# DestinationParameterValueConfigurationTypeDef definition

class DestinationParameterValueConfigurationTypeDef(TypedDict):
    CustomValuesConfiguration: NotRequired[CustomValuesConfigurationTypeDef],  # (1)
    SelectAllValueOptions: NotRequired[SelectAllValueOptionsType],  # (2)
    SourceParameterName: NotRequired[str],
    SourceField: NotRequired[str],
    SourceColumn: NotRequired[ColumnIdentifierTypeDef],  # (3)
```

1. See [:material-code-braces: CustomValuesConfigurationTypeDef](./type_defs.md#customvaluesconfigurationtypedef) 
2. See [:material-code-brackets: SelectAllValueOptionsType](./literals.md#selectallvalueoptionstype) 
3. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
## DatasetParameterTypeDef

```python
# DatasetParameterTypeDef definition

class DatasetParameterTypeDef(TypedDict):
    StringDatasetParameter: NotRequired[StringDatasetParameterTypeDef],  # (1)
    DecimalDatasetParameter: NotRequired[DecimalDatasetParameterTypeDef],  # (2)
    IntegerDatasetParameter: NotRequired[IntegerDatasetParameterTypeDef],  # (3)
    DateTimeDatasetParameter: NotRequired[DateTimeDatasetParameterTypeDef],  # (4)
```

1. See [:material-code-braces: StringDatasetParameterTypeDef](./type_defs.md#stringdatasetparametertypedef) 
2. See [:material-code-braces: DecimalDatasetParameterTypeDef](./type_defs.md#decimaldatasetparametertypedef) 
3. See [:material-code-braces: IntegerDatasetParameterTypeDef](./type_defs.md#integerdatasetparametertypedef) 
4. See [:material-code-braces: DateTimeDatasetParameterTypeDef](./type_defs.md#datetimedatasetparametertypedef) 
## TransformOperationTypeDef

```python
# TransformOperationTypeDef definition

class TransformOperationTypeDef(TypedDict):
    ProjectOperation: NotRequired[ProjectOperationTypeDef],  # (1)
    FilterOperation: NotRequired[FilterOperationTypeDef],  # (2)
    CreateColumnsOperation: NotRequired[CreateColumnsOperationTypeDef],  # (3)
    RenameColumnOperation: NotRequired[RenameColumnOperationTypeDef],  # (4)
    CastColumnTypeOperation: NotRequired[CastColumnTypeOperationTypeDef],  # (5)
    TagColumnOperation: NotRequired[TagColumnOperationTypeDef],  # (6)
    UntagColumnOperation: NotRequired[UntagColumnOperationTypeDef],  # (7)
    OverrideDatasetParameterOperation: NotRequired[OverrideDatasetParameterOperationTypeDef],  # (8)
```

1. See [:material-code-braces: ProjectOperationTypeDef](./type_defs.md#projectoperationtypedef) 
2. See [:material-code-braces: FilterOperationTypeDef](./type_defs.md#filteroperationtypedef) 
3. See [:material-code-braces: CreateColumnsOperationTypeDef](./type_defs.md#createcolumnsoperationtypedef) 
4. See [:material-code-braces: RenameColumnOperationTypeDef](./type_defs.md#renamecolumnoperationtypedef) 
5. See [:material-code-braces: CastColumnTypeOperationTypeDef](./type_defs.md#castcolumntypeoperationtypedef) 
6. See [:material-code-braces: TagColumnOperationTypeDef](./type_defs.md#tagcolumnoperationtypedef) 
7. See [:material-code-braces: UntagColumnOperationTypeDef](./type_defs.md#untagcolumnoperationtypedef) 
8. See [:material-code-braces: OverrideDatasetParameterOperationTypeDef](./type_defs.md#overridedatasetparameteroperationtypedef) 
## DateTimeHierarchyTypeDef

```python
# DateTimeHierarchyTypeDef definition

class DateTimeHierarchyTypeDef(TypedDict):
    HierarchyId: str,
    DrillDownFilters: NotRequired[Sequence[DrillDownFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: DrillDownFilterTypeDef](./type_defs.md#drilldownfiltertypedef) 
## ExplicitHierarchyTypeDef

```python
# ExplicitHierarchyTypeDef definition

class ExplicitHierarchyTypeDef(TypedDict):
    HierarchyId: str,
    Columns: Sequence[ColumnIdentifierTypeDef],  # (1)
    DrillDownFilters: NotRequired[Sequence[DrillDownFilterTypeDef]],  # (2)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: DrillDownFilterTypeDef](./type_defs.md#drilldownfiltertypedef) 
## PredefinedHierarchyTypeDef

```python
# PredefinedHierarchyTypeDef definition

class PredefinedHierarchyTypeDef(TypedDict):
    HierarchyId: str,
    Columns: Sequence[ColumnIdentifierTypeDef],  # (1)
    DrillDownFilters: NotRequired[Sequence[DrillDownFilterTypeDef]],  # (2)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: DrillDownFilterTypeDef](./type_defs.md#drilldownfiltertypedef) 
## ListTopicRefreshSchedulesResponseTypeDef

```python
# ListTopicRefreshSchedulesResponseTypeDef definition

class ListTopicRefreshSchedulesResponseTypeDef(TypedDict):
    TopicId: str,
    TopicArn: str,
    RefreshSchedules: List[TopicRefreshScheduleSummaryTypeDef],  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TopicRefreshScheduleSummaryTypeDef](./type_defs.md#topicrefreshschedulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ForecastConfigurationTypeDef

```python
# ForecastConfigurationTypeDef definition

class ForecastConfigurationTypeDef(TypedDict):
    ForecastProperties: NotRequired[TimeBasedForecastPropertiesTypeDef],  # (1)
    Scenario: NotRequired[ForecastScenarioTypeDef],  # (2)
```

1. See [:material-code-braces: TimeBasedForecastPropertiesTypeDef](./type_defs.md#timebasedforecastpropertiestypedef) 
2. See [:material-code-braces: ForecastScenarioTypeDef](./type_defs.md#forecastscenariotypedef) 
## PivotTableFieldOptionsTypeDef

```python
# PivotTableFieldOptionsTypeDef definition

class PivotTableFieldOptionsTypeDef(TypedDict):
    SelectedFieldOptions: NotRequired[Sequence[PivotTableFieldOptionTypeDef]],  # (1)
    DataPathOptions: NotRequired[Sequence[PivotTableDataPathOptionTypeDef]],  # (2)
    CollapseStateOptions: NotRequired[Sequence[PivotTableFieldCollapseStateOptionTypeDef]],  # (3)
```

1. See [:material-code-braces: PivotTableFieldOptionTypeDef](./type_defs.md#pivottablefieldoptiontypedef) 
2. See [:material-code-braces: PivotTableDataPathOptionTypeDef](./type_defs.md#pivottabledatapathoptiontypedef) 
3. See [:material-code-braces: PivotTableFieldCollapseStateOptionTypeDef](./type_defs.md#pivottablefieldcollapsestateoptiontypedef) 
## TopicCalculatedFieldTypeDef

```python
# TopicCalculatedFieldTypeDef definition

class TopicCalculatedFieldTypeDef(TypedDict):
    CalculatedFieldName: str,
    Expression: str,
    CalculatedFieldDescription: NotRequired[str],
    CalculatedFieldSynonyms: NotRequired[Sequence[str]],
    IsIncludedInTopic: NotRequired[bool],
    DisableIndexing: NotRequired[bool],
    ColumnDataRole: NotRequired[ColumnDataRoleType],  # (1)
    TimeGranularity: NotRequired[TopicTimeGranularityType],  # (2)
    DefaultFormatting: NotRequired[DefaultFormattingTypeDef],  # (3)
    Aggregation: NotRequired[DefaultAggregationType],  # (4)
    ComparativeOrder: NotRequired[ComparativeOrderTypeDef],  # (5)
    SemanticType: NotRequired[SemanticTypeTypeDef],  # (6)
    AllowedAggregations: NotRequired[Sequence[AuthorSpecifiedAggregationType]],  # (7)
    NotAllowedAggregations: NotRequired[Sequence[AuthorSpecifiedAggregationType]],  # (7)
    NeverAggregateInFilter: NotRequired[bool],
    CellValueSynonyms: NotRequired[Sequence[CellValueSynonymTypeDef]],  # (9)
    NonAdditive: NotRequired[bool],
```

1. See [:material-code-brackets: ColumnDataRoleType](./literals.md#columndataroletype) 
2. See [:material-code-brackets: TopicTimeGranularityType](./literals.md#topictimegranularitytype) 
3. See [:material-code-braces: DefaultFormattingTypeDef](./type_defs.md#defaultformattingtypedef) 
4. See [:material-code-brackets: DefaultAggregationType](./literals.md#defaultaggregationtype) 
5. See [:material-code-braces: ComparativeOrderTypeDef](./type_defs.md#comparativeordertypedef) 
6. See [:material-code-braces: SemanticTypeTypeDef](./type_defs.md#semantictypetypedef) 
7. See [:material-code-brackets: AuthorSpecifiedAggregationType](./literals.md#authorspecifiedaggregationtype) 
8. See [:material-code-brackets: AuthorSpecifiedAggregationType](./literals.md#authorspecifiedaggregationtype) 
9. See [:material-code-braces: CellValueSynonymTypeDef](./type_defs.md#cellvaluesynonymtypedef) 
## TopicColumnTypeDef

```python
# TopicColumnTypeDef definition

class TopicColumnTypeDef(TypedDict):
    ColumnName: str,
    ColumnFriendlyName: NotRequired[str],
    ColumnDescription: NotRequired[str],
    ColumnSynonyms: NotRequired[Sequence[str]],
    ColumnDataRole: NotRequired[ColumnDataRoleType],  # (1)
    Aggregation: NotRequired[DefaultAggregationType],  # (2)
    IsIncludedInTopic: NotRequired[bool],
    DisableIndexing: NotRequired[bool],
    ComparativeOrder: NotRequired[ComparativeOrderTypeDef],  # (3)
    SemanticType: NotRequired[SemanticTypeTypeDef],  # (4)
    TimeGranularity: NotRequired[TopicTimeGranularityType],  # (5)
    AllowedAggregations: NotRequired[Sequence[AuthorSpecifiedAggregationType]],  # (6)
    NotAllowedAggregations: NotRequired[Sequence[AuthorSpecifiedAggregationType]],  # (6)
    DefaultFormatting: NotRequired[DefaultFormattingTypeDef],  # (8)
    NeverAggregateInFilter: NotRequired[bool],
    CellValueSynonyms: NotRequired[Sequence[CellValueSynonymTypeDef]],  # (9)
    NonAdditive: NotRequired[bool],
```

1. See [:material-code-brackets: ColumnDataRoleType](./literals.md#columndataroletype) 
2. See [:material-code-brackets: DefaultAggregationType](./literals.md#defaultaggregationtype) 
3. See [:material-code-braces: ComparativeOrderTypeDef](./type_defs.md#comparativeordertypedef) 
4. See [:material-code-braces: SemanticTypeTypeDef](./type_defs.md#semantictypetypedef) 
5. See [:material-code-brackets: TopicTimeGranularityType](./literals.md#topictimegranularitytype) 
6. See [:material-code-brackets: AuthorSpecifiedAggregationType](./literals.md#authorspecifiedaggregationtype) 
7. See [:material-code-brackets: AuthorSpecifiedAggregationType](./literals.md#authorspecifiedaggregationtype) 
8. See [:material-code-braces: DefaultFormattingTypeDef](./type_defs.md#defaultformattingtypedef) 
9. See [:material-code-braces: CellValueSynonymTypeDef](./type_defs.md#cellvaluesynonymtypedef) 
## ChartAxisLabelOptionsTypeDef

```python
# ChartAxisLabelOptionsTypeDef definition

class ChartAxisLabelOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    SortIconVisibility: NotRequired[VisibilityType],  # (1)
    AxisLabelOptions: NotRequired[Sequence[AxisLabelOptionsTypeDef]],  # (3)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
3. See [:material-code-braces: AxisLabelOptionsTypeDef](./type_defs.md#axislabeloptionstypedef) 
## AxisTickLabelOptionsTypeDef

```python
# AxisTickLabelOptionsTypeDef definition

class AxisTickLabelOptionsTypeDef(TypedDict):
    LabelOptions: NotRequired[LabelOptionsTypeDef],  # (1)
    RotationAngle: NotRequired[float],
```

1. See [:material-code-braces: LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef) 
## DateTimePickerControlDisplayOptionsTypeDef

```python
# DateTimePickerControlDisplayOptionsTypeDef definition

class DateTimePickerControlDisplayOptionsTypeDef(TypedDict):
    TitleOptions: NotRequired[LabelOptionsTypeDef],  # (1)
    DateTimeFormat: NotRequired[str],
    InfoIconLabelOptions: NotRequired[SheetControlInfoIconLabelOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef) 
2. See [:material-code-braces: SheetControlInfoIconLabelOptionsTypeDef](./type_defs.md#sheetcontrolinfoiconlabeloptionstypedef) 
## DropDownControlDisplayOptionsTypeDef

```python
# DropDownControlDisplayOptionsTypeDef definition

class DropDownControlDisplayOptionsTypeDef(TypedDict):
    SelectAllOptions: NotRequired[ListControlSelectAllOptionsTypeDef],  # (1)
    TitleOptions: NotRequired[LabelOptionsTypeDef],  # (2)
    InfoIconLabelOptions: NotRequired[SheetControlInfoIconLabelOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: ListControlSelectAllOptionsTypeDef](./type_defs.md#listcontrolselectalloptionstypedef) 
2. See [:material-code-braces: LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef) 
3. See [:material-code-braces: SheetControlInfoIconLabelOptionsTypeDef](./type_defs.md#sheetcontrolinfoiconlabeloptionstypedef) 
## LegendOptionsTypeDef

```python
# LegendOptionsTypeDef definition

class LegendOptionsTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    Title: NotRequired[LabelOptionsTypeDef],  # (2)
    Position: NotRequired[LegendPositionType],  # (3)
    Width: NotRequired[str],
    Height: NotRequired[str],
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-braces: LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef) 
3. See [:material-code-brackets: LegendPositionType](./literals.md#legendpositiontype) 
## ListControlDisplayOptionsTypeDef

```python
# ListControlDisplayOptionsTypeDef definition

class ListControlDisplayOptionsTypeDef(TypedDict):
    SearchOptions: NotRequired[ListControlSearchOptionsTypeDef],  # (1)
    SelectAllOptions: NotRequired[ListControlSelectAllOptionsTypeDef],  # (2)
    TitleOptions: NotRequired[LabelOptionsTypeDef],  # (3)
    InfoIconLabelOptions: NotRequired[SheetControlInfoIconLabelOptionsTypeDef],  # (4)
```

1. See [:material-code-braces: ListControlSearchOptionsTypeDef](./type_defs.md#listcontrolsearchoptionstypedef) 
2. See [:material-code-braces: ListControlSelectAllOptionsTypeDef](./type_defs.md#listcontrolselectalloptionstypedef) 
3. See [:material-code-braces: LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef) 
4. See [:material-code-braces: SheetControlInfoIconLabelOptionsTypeDef](./type_defs.md#sheetcontrolinfoiconlabeloptionstypedef) 
## RelativeDateTimeControlDisplayOptionsTypeDef

```python
# RelativeDateTimeControlDisplayOptionsTypeDef definition

class RelativeDateTimeControlDisplayOptionsTypeDef(TypedDict):
    TitleOptions: NotRequired[LabelOptionsTypeDef],  # (1)
    DateTimeFormat: NotRequired[str],
    InfoIconLabelOptions: NotRequired[SheetControlInfoIconLabelOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef) 
2. See [:material-code-braces: SheetControlInfoIconLabelOptionsTypeDef](./type_defs.md#sheetcontrolinfoiconlabeloptionstypedef) 
## SliderControlDisplayOptionsTypeDef

```python
# SliderControlDisplayOptionsTypeDef definition

class SliderControlDisplayOptionsTypeDef(TypedDict):
    TitleOptions: NotRequired[LabelOptionsTypeDef],  # (1)
    InfoIconLabelOptions: NotRequired[SheetControlInfoIconLabelOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef) 
2. See [:material-code-braces: SheetControlInfoIconLabelOptionsTypeDef](./type_defs.md#sheetcontrolinfoiconlabeloptionstypedef) 
## TextAreaControlDisplayOptionsTypeDef

```python
# TextAreaControlDisplayOptionsTypeDef definition

class TextAreaControlDisplayOptionsTypeDef(TypedDict):
    TitleOptions: NotRequired[LabelOptionsTypeDef],  # (1)
    PlaceholderOptions: NotRequired[TextControlPlaceholderOptionsTypeDef],  # (2)
    InfoIconLabelOptions: NotRequired[SheetControlInfoIconLabelOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef) 
2. See [:material-code-braces: TextControlPlaceholderOptionsTypeDef](./type_defs.md#textcontrolplaceholderoptionstypedef) 
3. See [:material-code-braces: SheetControlInfoIconLabelOptionsTypeDef](./type_defs.md#sheetcontrolinfoiconlabeloptionstypedef) 
## TextFieldControlDisplayOptionsTypeDef

```python
# TextFieldControlDisplayOptionsTypeDef definition

class TextFieldControlDisplayOptionsTypeDef(TypedDict):
    TitleOptions: NotRequired[LabelOptionsTypeDef],  # (1)
    PlaceholderOptions: NotRequired[TextControlPlaceholderOptionsTypeDef],  # (2)
    InfoIconLabelOptions: NotRequired[SheetControlInfoIconLabelOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef) 
2. See [:material-code-braces: TextControlPlaceholderOptionsTypeDef](./type_defs.md#textcontrolplaceholderoptionstypedef) 
3. See [:material-code-braces: SheetControlInfoIconLabelOptionsTypeDef](./type_defs.md#sheetcontrolinfoiconlabeloptionstypedef) 
## PanelConfigurationTypeDef

```python
# PanelConfigurationTypeDef definition

class PanelConfigurationTypeDef(TypedDict):
    Title: NotRequired[PanelTitleOptionsTypeDef],  # (1)
    BorderVisibility: NotRequired[VisibilityType],  # (2)
    BorderThickness: NotRequired[str],
    BorderStyle: NotRequired[PanelBorderStyleType],  # (3)
    BorderColor: NotRequired[str],
    GutterVisibility: NotRequired[VisibilityType],  # (2)
    GutterSpacing: NotRequired[str],
    BackgroundVisibility: NotRequired[VisibilityType],  # (2)
    BackgroundColor: NotRequired[str],
```

1. See [:material-code-braces: PanelTitleOptionsTypeDef](./type_defs.md#paneltitleoptionstypedef) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
3. See [:material-code-brackets: PanelBorderStyleType](./literals.md#panelborderstyletype) 
4. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
5. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## TableFieldLinkContentConfigurationTypeDef

```python
# TableFieldLinkContentConfigurationTypeDef definition

class TableFieldLinkContentConfigurationTypeDef(TypedDict):
    CustomTextContent: NotRequired[TableFieldCustomTextContentTypeDef],  # (1)
    CustomIconContent: NotRequired[TableFieldCustomIconContentTypeDef],  # (2)
```

1. See [:material-code-braces: TableFieldCustomTextContentTypeDef](./type_defs.md#tablefieldcustomtextcontenttypedef) 
2. See [:material-code-braces: TableFieldCustomIconContentTypeDef](./type_defs.md#tablefieldcustomiconcontenttypedef) 
## GeospatialPointStyleOptionsTypeDef

```python
# GeospatialPointStyleOptionsTypeDef definition

class GeospatialPointStyleOptionsTypeDef(TypedDict):
    SelectedPointStyle: NotRequired[GeospatialSelectedPointStyleType],  # (1)
    ClusterMarkerConfiguration: NotRequired[ClusterMarkerConfigurationTypeDef],  # (2)
    HeatmapConfiguration: NotRequired[GeospatialHeatmapConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: GeospatialSelectedPointStyleType](./literals.md#geospatialselectedpointstyletype) 
2. See [:material-code-braces: ClusterMarkerConfigurationTypeDef](./type_defs.md#clustermarkerconfigurationtypedef) 
3. See [:material-code-braces: GeospatialHeatmapConfigurationTypeDef](./type_defs.md#geospatialheatmapconfigurationtypedef) 
## TableCellStyleTypeDef

```python
# TableCellStyleTypeDef definition

class TableCellStyleTypeDef(TypedDict):
    Visibility: NotRequired[VisibilityType],  # (1)
    FontConfiguration: NotRequired[FontConfigurationTypeDef],  # (2)
    TextWrap: NotRequired[TextWrapType],  # (3)
    HorizontalTextAlignment: NotRequired[HorizontalTextAlignmentType],  # (4)
    VerticalTextAlignment: NotRequired[VerticalTextAlignmentType],  # (5)
    BackgroundColor: NotRequired[str],
    Height: NotRequired[int],
    Border: NotRequired[GlobalTableBorderOptionsTypeDef],  # (6)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-braces: FontConfigurationTypeDef](./type_defs.md#fontconfigurationtypedef) 
3. See [:material-code-brackets: TextWrapType](./literals.md#textwraptype) 
4. See [:material-code-brackets: HorizontalTextAlignmentType](./literals.md#horizontaltextalignmenttype) 
5. See [:material-code-brackets: VerticalTextAlignmentType](./literals.md#verticaltextalignmenttype) 
6. See [:material-code-braces: GlobalTableBorderOptionsTypeDef](./type_defs.md#globaltableborderoptionstypedef) 
## ConditionalFormattingColorTypeDef

```python
# ConditionalFormattingColorTypeDef definition

class ConditionalFormattingColorTypeDef(TypedDict):
    Solid: NotRequired[ConditionalFormattingSolidColorTypeDef],  # (1)
    Gradient: NotRequired[ConditionalFormattingGradientColorTypeDef],  # (2)
```

1. See [:material-code-braces: ConditionalFormattingSolidColorTypeDef](./type_defs.md#conditionalformattingsolidcolortypedef) 
2. See [:material-code-braces: ConditionalFormattingGradientColorTypeDef](./type_defs.md#conditionalformattinggradientcolortypedef) 
## DefaultInteractiveLayoutConfigurationTypeDef

```python
# DefaultInteractiveLayoutConfigurationTypeDef definition

class DefaultInteractiveLayoutConfigurationTypeDef(TypedDict):
    Grid: NotRequired[DefaultGridLayoutConfigurationTypeDef],  # (1)
    FreeForm: NotRequired[DefaultFreeFormLayoutConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: DefaultGridLayoutConfigurationTypeDef](./type_defs.md#defaultgridlayoutconfigurationtypedef) 
2. See [:material-code-braces: DefaultFreeFormLayoutConfigurationTypeDef](./type_defs.md#defaultfreeformlayoutconfigurationtypedef) 
## SheetControlLayoutConfigurationTypeDef

```python
# SheetControlLayoutConfigurationTypeDef definition

class SheetControlLayoutConfigurationTypeDef(TypedDict):
    GridLayout: NotRequired[GridLayoutConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: GridLayoutConfigurationTypeDef](./type_defs.md#gridlayoutconfigurationtypedef) 
## DataSetRefreshPropertiesTypeDef

```python
# DataSetRefreshPropertiesTypeDef definition

class DataSetRefreshPropertiesTypeDef(TypedDict):
    RefreshConfiguration: RefreshConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: RefreshConfigurationTypeDef](./type_defs.md#refreshconfigurationtypedef) 
## SeriesItemTypeDef

```python
# SeriesItemTypeDef definition

class SeriesItemTypeDef(TypedDict):
    FieldSeriesItem: NotRequired[FieldSeriesItemTypeDef],  # (1)
    DataFieldSeriesItem: NotRequired[DataFieldSeriesItemTypeDef],  # (2)
```

1. See [:material-code-braces: FieldSeriesItemTypeDef](./type_defs.md#fieldseriesitemtypedef) 
2. See [:material-code-braces: DataFieldSeriesItemTypeDef](./type_defs.md#datafieldseriesitemtypedef) 
## AssetBundleImportJobDataSourceOverrideParametersTypeDef

```python
# AssetBundleImportJobDataSourceOverrideParametersTypeDef definition

class AssetBundleImportJobDataSourceOverrideParametersTypeDef(TypedDict):
    DataSourceId: str,
    Name: NotRequired[str],
    DataSourceParameters: NotRequired[DataSourceParametersTypeDef],  # (1)
    VpcConnectionProperties: NotRequired[VpcConnectionPropertiesTypeDef],  # (2)
    SslProperties: NotRequired[SslPropertiesTypeDef],  # (3)
    Credentials: NotRequired[AssetBundleImportJobDataSourceCredentialsTypeDef],  # (4)
```

1. See [:material-code-braces: DataSourceParametersTypeDef](./type_defs.md#datasourceparameterstypedef) 
2. See [:material-code-braces: VpcConnectionPropertiesTypeDef](./type_defs.md#vpcconnectionpropertiestypedef) 
3. See [:material-code-braces: SslPropertiesTypeDef](./type_defs.md#sslpropertiestypedef) 
4. See [:material-code-braces: AssetBundleImportJobDataSourceCredentialsTypeDef](./type_defs.md#assetbundleimportjobdatasourcecredentialstypedef) 
## CredentialPairTypeDef

```python
# CredentialPairTypeDef definition

class CredentialPairTypeDef(TypedDict):
    Username: str,
    Password: str,
    AlternateDataSourceParameters: NotRequired[Sequence[DataSourceParametersTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceParametersTypeDef](./type_defs.md#datasourceparameterstypedef) 
## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    Arn: NotRequired[str],
    DataSourceId: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[DataSourceTypeType],  # (1)
    Status: NotRequired[ResourceStatusType],  # (2)
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    DataSourceParameters: NotRequired[DataSourceParametersTypeDef],  # (3)
    AlternateDataSourceParameters: NotRequired[List[DataSourceParametersTypeDef]],  # (4)
    VpcConnectionProperties: NotRequired[VpcConnectionPropertiesTypeDef],  # (5)
    SslProperties: NotRequired[SslPropertiesTypeDef],  # (6)
    ErrorInfo: NotRequired[DataSourceErrorInfoTypeDef],  # (7)
    SecretArn: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
3. See [:material-code-braces: DataSourceParametersTypeDef](./type_defs.md#datasourceparameterstypedef) 
4. See [:material-code-braces: DataSourceParametersTypeDef](./type_defs.md#datasourceparameterstypedef) 
5. See [:material-code-braces: VpcConnectionPropertiesTypeDef](./type_defs.md#vpcconnectionpropertiestypedef) 
6. See [:material-code-braces: SslPropertiesTypeDef](./type_defs.md#sslpropertiestypedef) 
7. See [:material-code-braces: DataSourceErrorInfoTypeDef](./type_defs.md#datasourceerrorinfotypedef) 
## ThemeConfigurationTypeDef

```python
# ThemeConfigurationTypeDef definition

class ThemeConfigurationTypeDef(TypedDict):
    DataColorPalette: NotRequired[DataColorPaletteTypeDef],  # (1)
    UIColorPalette: NotRequired[UIColorPaletteTypeDef],  # (2)
    Sheet: NotRequired[SheetStyleTypeDef],  # (3)
    Typography: NotRequired[TypographyTypeDef],  # (4)
```

1. See [:material-code-braces: DataColorPaletteTypeDef](./type_defs.md#datacolorpalettetypedef) 
2. See [:material-code-braces: UIColorPaletteTypeDef](./type_defs.md#uicolorpalettetypedef) 
3. See [:material-code-braces: SheetStyleTypeDef](./type_defs.md#sheetstyletypedef) 
4. See [:material-code-braces: TypographyTypeDef](./type_defs.md#typographytypedef) 
## ComparisonFormatConfigurationTypeDef

```python
# ComparisonFormatConfigurationTypeDef definition

class ComparisonFormatConfigurationTypeDef(TypedDict):
    NumberDisplayFormatConfiguration: NotRequired[NumberDisplayFormatConfigurationTypeDef],  # (1)
    PercentageDisplayFormatConfiguration: NotRequired[PercentageDisplayFormatConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: NumberDisplayFormatConfigurationTypeDef](./type_defs.md#numberdisplayformatconfigurationtypedef) 
2. See [:material-code-braces: PercentageDisplayFormatConfigurationTypeDef](./type_defs.md#percentagedisplayformatconfigurationtypedef) 
## NumericFormatConfigurationTypeDef

```python
# NumericFormatConfigurationTypeDef definition

class NumericFormatConfigurationTypeDef(TypedDict):
    NumberDisplayFormatConfiguration: NotRequired[NumberDisplayFormatConfigurationTypeDef],  # (1)
    CurrencyDisplayFormatConfiguration: NotRequired[CurrencyDisplayFormatConfigurationTypeDef],  # (2)
    PercentageDisplayFormatConfiguration: NotRequired[PercentageDisplayFormatConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: NumberDisplayFormatConfigurationTypeDef](./type_defs.md#numberdisplayformatconfigurationtypedef) 
2. See [:material-code-braces: CurrencyDisplayFormatConfigurationTypeDef](./type_defs.md#currencydisplayformatconfigurationtypedef) 
3. See [:material-code-braces: PercentageDisplayFormatConfigurationTypeDef](./type_defs.md#percentagedisplayformatconfigurationtypedef) 
## AggregationSortConfigurationTypeDef

```python
# AggregationSortConfigurationTypeDef definition

class AggregationSortConfigurationTypeDef(TypedDict):
    Column: ColumnIdentifierTypeDef,  # (1)
    SortDirection: SortDirectionType,  # (2)
    AggregationFunction: NotRequired[AggregationFunctionTypeDef],  # (3)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-brackets: SortDirectionType](./literals.md#sortdirectiontype) 
3. See [:material-code-braces: AggregationFunctionTypeDef](./type_defs.md#aggregationfunctiontypedef) 
## ColumnSortTypeDef

```python
# ColumnSortTypeDef definition

class ColumnSortTypeDef(TypedDict):
    SortBy: ColumnIdentifierTypeDef,  # (1)
    Direction: SortDirectionType,  # (2)
    AggregationFunction: NotRequired[AggregationFunctionTypeDef],  # (3)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-brackets: SortDirectionType](./literals.md#sortdirectiontype) 
3. See [:material-code-braces: AggregationFunctionTypeDef](./type_defs.md#aggregationfunctiontypedef) 
## ColumnTooltipItemTypeDef

```python
# ColumnTooltipItemTypeDef definition

class ColumnTooltipItemTypeDef(TypedDict):
    Column: ColumnIdentifierTypeDef,  # (1)
    Label: NotRequired[str],
    Visibility: NotRequired[VisibilityType],  # (2)
    Aggregation: NotRequired[AggregationFunctionTypeDef],  # (3)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
3. See [:material-code-braces: AggregationFunctionTypeDef](./type_defs.md#aggregationfunctiontypedef) 
## NumericEqualityFilterTypeDef

```python
# NumericEqualityFilterTypeDef definition

class NumericEqualityFilterTypeDef(TypedDict):
    FilterId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    MatchOperator: NumericEqualityMatchOperatorType,  # (3)
    NullOption: FilterNullOptionType,  # (5)
    Value: NotRequired[float],
    SelectAllOptions: NotRequired[NumericFilterSelectAllOptionsType],  # (2)
    AggregationFunction: NotRequired[AggregationFunctionTypeDef],  # (4)
    ParameterName: NotRequired[str],
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-brackets: NumericFilterSelectAllOptionsType](./literals.md#numericfilterselectalloptionstype) 
3. See [:material-code-brackets: NumericEqualityMatchOperatorType](./literals.md#numericequalitymatchoperatortype) 
4. See [:material-code-braces: AggregationFunctionTypeDef](./type_defs.md#aggregationfunctiontypedef) 
5. See [:material-code-brackets: FilterNullOptionType](./literals.md#filternulloptiontype) 
## NumericRangeFilterTypeDef

```python
# NumericRangeFilterTypeDef definition

class NumericRangeFilterTypeDef(TypedDict):
    FilterId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    NullOption: FilterNullOptionType,  # (6)
    IncludeMinimum: NotRequired[bool],
    IncludeMaximum: NotRequired[bool],
    RangeMinimum: NotRequired[NumericRangeFilterValueTypeDef],  # (2)
    RangeMaximum: NotRequired[NumericRangeFilterValueTypeDef],  # (2)
    SelectAllOptions: NotRequired[NumericFilterSelectAllOptionsType],  # (4)
    AggregationFunction: NotRequired[AggregationFunctionTypeDef],  # (5)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: NumericRangeFilterValueTypeDef](./type_defs.md#numericrangefiltervaluetypedef) 
3. See [:material-code-braces: NumericRangeFilterValueTypeDef](./type_defs.md#numericrangefiltervaluetypedef) 
4. See [:material-code-brackets: NumericFilterSelectAllOptionsType](./literals.md#numericfilterselectalloptionstype) 
5. See [:material-code-braces: AggregationFunctionTypeDef](./type_defs.md#aggregationfunctiontypedef) 
6. See [:material-code-brackets: FilterNullOptionType](./literals.md#filternulloptiontype) 
## ReferenceLineDynamicDataConfigurationTypeDef

```python
# ReferenceLineDynamicDataConfigurationTypeDef definition

class ReferenceLineDynamicDataConfigurationTypeDef(TypedDict):
    Column: ColumnIdentifierTypeDef,  # (1)
    Calculation: NumericalAggregationFunctionTypeDef,  # (3)
    MeasureAggregationFunction: NotRequired[AggregationFunctionTypeDef],  # (2)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: AggregationFunctionTypeDef](./type_defs.md#aggregationfunctiontypedef) 
3. See [:material-code-braces: NumericalAggregationFunctionTypeDef](./type_defs.md#numericalaggregationfunctiontypedef) 
## TopicFilterTypeDef

```python
# TopicFilterTypeDef definition

class TopicFilterTypeDef(TypedDict):
    FilterName: str,
    OperandFieldName: str,
    FilterDescription: NotRequired[str],
    FilterClass: NotRequired[FilterClassType],  # (1)
    FilterSynonyms: NotRequired[Sequence[str]],
    FilterType: NotRequired[NamedFilterTypeType],  # (2)
    CategoryFilter: NotRequired[TopicCategoryFilterTypeDef],  # (3)
    NumericEqualityFilter: NotRequired[TopicNumericEqualityFilterTypeDef],  # (4)
    NumericRangeFilter: NotRequired[TopicNumericRangeFilterTypeDef],  # (5)
    DateRangeFilter: NotRequired[TopicDateRangeFilterTypeDef],  # (6)
    RelativeDateFilter: NotRequired[TopicRelativeDateFilterTypeDef],  # (7)
```

1. See [:material-code-brackets: FilterClassType](./literals.md#filterclasstype) 
2. See [:material-code-brackets: NamedFilterTypeType](./literals.md#namedfiltertypetype) 
3. See [:material-code-braces: TopicCategoryFilterTypeDef](./type_defs.md#topiccategoryfiltertypedef) 
4. See [:material-code-braces: TopicNumericEqualityFilterTypeDef](./type_defs.md#topicnumericequalityfiltertypedef) 
5. See [:material-code-braces: TopicNumericRangeFilterTypeDef](./type_defs.md#topicnumericrangefiltertypedef) 
6. See [:material-code-braces: TopicDateRangeFilterTypeDef](./type_defs.md#topicdaterangefiltertypedef) 
7. See [:material-code-braces: TopicRelativeDateFilterTypeDef](./type_defs.md#topicrelativedatefiltertypedef) 
## CreateRefreshScheduleRequestRequestTypeDef

```python
# CreateRefreshScheduleRequestRequestTypeDef definition

class CreateRefreshScheduleRequestRequestTypeDef(TypedDict):
    DataSetId: str,
    AwsAccountId: str,
    Schedule: RefreshScheduleTypeDef,  # (1)
```

1. See [:material-code-braces: RefreshScheduleTypeDef](./type_defs.md#refreshscheduletypedef) 
## DescribeRefreshScheduleResponseTypeDef

```python
# DescribeRefreshScheduleResponseTypeDef definition

class DescribeRefreshScheduleResponseTypeDef(TypedDict):
    RefreshSchedule: RefreshScheduleTypeDef,  # (1)
    Status: int,
    RequestId: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RefreshScheduleTypeDef](./type_defs.md#refreshscheduletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRefreshSchedulesResponseTypeDef

```python
# ListRefreshSchedulesResponseTypeDef definition

class ListRefreshSchedulesResponseTypeDef(TypedDict):
    RefreshSchedules: List[RefreshScheduleTypeDef],  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RefreshScheduleTypeDef](./type_defs.md#refreshscheduletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRefreshScheduleRequestRequestTypeDef

```python
# UpdateRefreshScheduleRequestRequestTypeDef definition

class UpdateRefreshScheduleRequestRequestTypeDef(TypedDict):
    DataSetId: str,
    AwsAccountId: str,
    Schedule: RefreshScheduleTypeDef,  # (1)
```

1. See [:material-code-braces: RefreshScheduleTypeDef](./type_defs.md#refreshscheduletypedef) 
## RegisteredUserEmbeddingExperienceConfigurationTypeDef

```python
# RegisteredUserEmbeddingExperienceConfigurationTypeDef definition

class RegisteredUserEmbeddingExperienceConfigurationTypeDef(TypedDict):
    Dashboard: NotRequired[RegisteredUserDashboardEmbeddingConfigurationTypeDef],  # (1)
    QuickSightConsole: NotRequired[RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef],  # (2)
    QSearchBar: NotRequired[RegisteredUserQSearchBarEmbeddingConfigurationTypeDef],  # (3)
    DashboardVisual: NotRequired[RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: RegisteredUserDashboardEmbeddingConfigurationTypeDef](./type_defs.md#registereduserdashboardembeddingconfigurationtypedef) 
2. See [:material-code-braces: RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef](./type_defs.md#registereduserquicksightconsoleembeddingconfigurationtypedef) 
3. See [:material-code-braces: RegisteredUserQSearchBarEmbeddingConfigurationTypeDef](./type_defs.md#registereduserqsearchbarembeddingconfigurationtypedef) 
4. See [:material-code-braces: RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef](./type_defs.md#registereduserdashboardvisualembeddingconfigurationtypedef) 
## SnapshotJobResultFileGroupTypeDef

```python
# SnapshotJobResultFileGroupTypeDef definition

class SnapshotJobResultFileGroupTypeDef(TypedDict):
    Files: NotRequired[List[SnapshotFileTypeDef]],  # (1)
    S3Results: NotRequired[List[SnapshotJobS3ResultTypeDef]],  # (2)
```

1. See [:material-code-braces: SnapshotFileTypeDef](./type_defs.md#snapshotfiletypedef) 
2. See [:material-code-braces: SnapshotJobS3ResultTypeDef](./type_defs.md#snapshotjobs3resulttypedef) 
## DefaultSectionBasedLayoutConfigurationTypeDef

```python
# DefaultSectionBasedLayoutConfigurationTypeDef definition

class DefaultSectionBasedLayoutConfigurationTypeDef(TypedDict):
    CanvasSizeOptions: SectionBasedLayoutCanvasSizeOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: SectionBasedLayoutCanvasSizeOptionsTypeDef](./type_defs.md#sectionbasedlayoutcanvassizeoptionstypedef) 
## FreeFormLayoutConfigurationTypeDef

```python
# FreeFormLayoutConfigurationTypeDef definition

class FreeFormLayoutConfigurationTypeDef(TypedDict):
    Elements: Sequence[FreeFormLayoutElementTypeDef],  # (1)
    CanvasSizeOptions: NotRequired[FreeFormLayoutCanvasSizeOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: FreeFormLayoutElementTypeDef](./type_defs.md#freeformlayoutelementtypedef) 
2. See [:material-code-braces: FreeFormLayoutCanvasSizeOptionsTypeDef](./type_defs.md#freeformlayoutcanvassizeoptionstypedef) 
## FreeFormSectionLayoutConfigurationTypeDef

```python
# FreeFormSectionLayoutConfigurationTypeDef definition

class FreeFormSectionLayoutConfigurationTypeDef(TypedDict):
    Elements: Sequence[FreeFormLayoutElementTypeDef],  # (1)
```

1. See [:material-code-braces: FreeFormLayoutElementTypeDef](./type_defs.md#freeformlayoutelementtypedef) 
## SnapshotConfigurationTypeDef

```python
# SnapshotConfigurationTypeDef definition

class SnapshotConfigurationTypeDef(TypedDict):
    FileGroups: List[SnapshotFileGroupTypeDef],  # (1)
    DestinationConfiguration: NotRequired[SnapshotDestinationConfigurationTypeDef],  # (2)
    Parameters: NotRequired[ParametersTypeDef],  # (3)
```

1. See [:material-code-braces: SnapshotFileGroupTypeDef](./type_defs.md#snapshotfilegrouptypedef) 
2. See [:material-code-braces: SnapshotDestinationConfigurationTypeDef](./type_defs.md#snapshotdestinationconfigurationtypedef) 
3. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
## ParameterDeclarationTypeDef

```python
# ParameterDeclarationTypeDef definition

class ParameterDeclarationTypeDef(TypedDict):
    StringParameterDeclaration: NotRequired[StringParameterDeclarationTypeDef],  # (1)
    DecimalParameterDeclaration: NotRequired[DecimalParameterDeclarationTypeDef],  # (2)
    IntegerParameterDeclaration: NotRequired[IntegerParameterDeclarationTypeDef],  # (3)
    DateTimeParameterDeclaration: NotRequired[DateTimeParameterDeclarationTypeDef],  # (4)
```

1. See [:material-code-braces: StringParameterDeclarationTypeDef](./type_defs.md#stringparameterdeclarationtypedef) 
2. See [:material-code-braces: DecimalParameterDeclarationTypeDef](./type_defs.md#decimalparameterdeclarationtypedef) 
3. See [:material-code-braces: IntegerParameterDeclarationTypeDef](./type_defs.md#integerparameterdeclarationtypedef) 
4. See [:material-code-braces: DateTimeParameterDeclarationTypeDef](./type_defs.md#datetimeparameterdeclarationtypedef) 
## DescribeDashboardResponseTypeDef

```python
# DescribeDashboardResponseTypeDef definition

class DescribeDashboardResponseTypeDef(TypedDict):
    Dashboard: DashboardTypeDef,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DashboardTypeDef](./type_defs.md#dashboardtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TemplateTypeDef

```python
# TemplateTypeDef definition

class TemplateTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Version: NotRequired[TemplateVersionTypeDef],  # (1)
    TemplateId: NotRequired[str],
    LastUpdatedTime: NotRequired[datetime],
    CreatedTime: NotRequired[datetime],
```

1. See [:material-code-braces: TemplateVersionTypeDef](./type_defs.md#templateversiontypedef) 
## SetParameterValueConfigurationTypeDef

```python
# SetParameterValueConfigurationTypeDef definition

class SetParameterValueConfigurationTypeDef(TypedDict):
    DestinationParameterName: str,
    Value: DestinationParameterValueConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: DestinationParameterValueConfigurationTypeDef](./type_defs.md#destinationparametervalueconfigurationtypedef) 
## LogicalTableTypeDef

```python
# LogicalTableTypeDef definition

class LogicalTableTypeDef(TypedDict):
    Alias: str,
    Source: LogicalTableSourceTypeDef,  # (2)
    DataTransforms: NotRequired[Sequence[TransformOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: TransformOperationTypeDef](./type_defs.md#transformoperationtypedef) 
2. See [:material-code-braces: LogicalTableSourceTypeDef](./type_defs.md#logicaltablesourcetypedef) 
## ColumnHierarchyTypeDef

```python
# ColumnHierarchyTypeDef definition

class ColumnHierarchyTypeDef(TypedDict):
    ExplicitHierarchy: NotRequired[ExplicitHierarchyTypeDef],  # (1)
    DateTimeHierarchy: NotRequired[DateTimeHierarchyTypeDef],  # (2)
    PredefinedHierarchy: NotRequired[PredefinedHierarchyTypeDef],  # (3)
```

1. See [:material-code-braces: ExplicitHierarchyTypeDef](./type_defs.md#explicithierarchytypedef) 
2. See [:material-code-braces: DateTimeHierarchyTypeDef](./type_defs.md#datetimehierarchytypedef) 
3. See [:material-code-braces: PredefinedHierarchyTypeDef](./type_defs.md#predefinedhierarchytypedef) 
## AxisDisplayOptionsTypeDef

```python
# AxisDisplayOptionsTypeDef definition

class AxisDisplayOptionsTypeDef(TypedDict):
    TickLabelOptions: NotRequired[AxisTickLabelOptionsTypeDef],  # (1)
    AxisLineVisibility: NotRequired[VisibilityType],  # (2)
    GridLineVisibility: NotRequired[VisibilityType],  # (2)
    DataOptions: NotRequired[AxisDataOptionsTypeDef],  # (4)
    ScrollbarOptions: NotRequired[ScrollBarOptionsTypeDef],  # (5)
    AxisOffset: NotRequired[str],
```

1. See [:material-code-braces: AxisTickLabelOptionsTypeDef](./type_defs.md#axisticklabeloptionstypedef) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
3. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
4. See [:material-code-braces: AxisDataOptionsTypeDef](./type_defs.md#axisdataoptionstypedef) 
5. See [:material-code-braces: ScrollBarOptionsTypeDef](./type_defs.md#scrollbaroptionstypedef) 
## FilterDateTimePickerControlTypeDef

```python
# FilterDateTimePickerControlTypeDef definition

class FilterDateTimePickerControlTypeDef(TypedDict):
    FilterControlId: str,
    Title: str,
    SourceFilterId: str,
    DisplayOptions: NotRequired[DateTimePickerControlDisplayOptionsTypeDef],  # (1)
    Type: NotRequired[SheetControlDateTimePickerTypeType],  # (2)
```

1. See [:material-code-braces: DateTimePickerControlDisplayOptionsTypeDef](./type_defs.md#datetimepickercontroldisplayoptionstypedef) 
2. See [:material-code-brackets: SheetControlDateTimePickerTypeType](./literals.md#sheetcontroldatetimepickertypetype) 
## ParameterDateTimePickerControlTypeDef

```python
# ParameterDateTimePickerControlTypeDef definition

class ParameterDateTimePickerControlTypeDef(TypedDict):
    ParameterControlId: str,
    Title: str,
    SourceParameterName: str,
    DisplayOptions: NotRequired[DateTimePickerControlDisplayOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: DateTimePickerControlDisplayOptionsTypeDef](./type_defs.md#datetimepickercontroldisplayoptionstypedef) 
## FilterDropDownControlTypeDef

```python
# FilterDropDownControlTypeDef definition

class FilterDropDownControlTypeDef(TypedDict):
    FilterControlId: str,
    Title: str,
    SourceFilterId: str,
    DisplayOptions: NotRequired[DropDownControlDisplayOptionsTypeDef],  # (1)
    Type: NotRequired[SheetControlListTypeType],  # (2)
    SelectableValues: NotRequired[FilterSelectableValuesTypeDef],  # (3)
    CascadingControlConfiguration: NotRequired[CascadingControlConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: DropDownControlDisplayOptionsTypeDef](./type_defs.md#dropdowncontroldisplayoptionstypedef) 
2. See [:material-code-brackets: SheetControlListTypeType](./literals.md#sheetcontrollisttypetype) 
3. See [:material-code-braces: FilterSelectableValuesTypeDef](./type_defs.md#filterselectablevaluestypedef) 
4. See [:material-code-braces: CascadingControlConfigurationTypeDef](./type_defs.md#cascadingcontrolconfigurationtypedef) 
## ParameterDropDownControlTypeDef

```python
# ParameterDropDownControlTypeDef definition

class ParameterDropDownControlTypeDef(TypedDict):
    ParameterControlId: str,
    Title: str,
    SourceParameterName: str,
    DisplayOptions: NotRequired[DropDownControlDisplayOptionsTypeDef],  # (1)
    Type: NotRequired[SheetControlListTypeType],  # (2)
    SelectableValues: NotRequired[ParameterSelectableValuesTypeDef],  # (3)
    CascadingControlConfiguration: NotRequired[CascadingControlConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: DropDownControlDisplayOptionsTypeDef](./type_defs.md#dropdowncontroldisplayoptionstypedef) 
2. See [:material-code-brackets: SheetControlListTypeType](./literals.md#sheetcontrollisttypetype) 
3. See [:material-code-braces: ParameterSelectableValuesTypeDef](./type_defs.md#parameterselectablevaluestypedef) 
4. See [:material-code-braces: CascadingControlConfigurationTypeDef](./type_defs.md#cascadingcontrolconfigurationtypedef) 
## FilterListControlTypeDef

```python
# FilterListControlTypeDef definition

class FilterListControlTypeDef(TypedDict):
    FilterControlId: str,
    Title: str,
    SourceFilterId: str,
    DisplayOptions: NotRequired[ListControlDisplayOptionsTypeDef],  # (1)
    Type: NotRequired[SheetControlListTypeType],  # (2)
    SelectableValues: NotRequired[FilterSelectableValuesTypeDef],  # (3)
    CascadingControlConfiguration: NotRequired[CascadingControlConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: ListControlDisplayOptionsTypeDef](./type_defs.md#listcontroldisplayoptionstypedef) 
2. See [:material-code-brackets: SheetControlListTypeType](./literals.md#sheetcontrollisttypetype) 
3. See [:material-code-braces: FilterSelectableValuesTypeDef](./type_defs.md#filterselectablevaluestypedef) 
4. See [:material-code-braces: CascadingControlConfigurationTypeDef](./type_defs.md#cascadingcontrolconfigurationtypedef) 
## ParameterListControlTypeDef

```python
# ParameterListControlTypeDef definition

class ParameterListControlTypeDef(TypedDict):
    ParameterControlId: str,
    Title: str,
    SourceParameterName: str,
    DisplayOptions: NotRequired[ListControlDisplayOptionsTypeDef],  # (1)
    Type: NotRequired[SheetControlListTypeType],  # (2)
    SelectableValues: NotRequired[ParameterSelectableValuesTypeDef],  # (3)
    CascadingControlConfiguration: NotRequired[CascadingControlConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: ListControlDisplayOptionsTypeDef](./type_defs.md#listcontroldisplayoptionstypedef) 
2. See [:material-code-brackets: SheetControlListTypeType](./literals.md#sheetcontrollisttypetype) 
3. See [:material-code-braces: ParameterSelectableValuesTypeDef](./type_defs.md#parameterselectablevaluestypedef) 
4. See [:material-code-braces: CascadingControlConfigurationTypeDef](./type_defs.md#cascadingcontrolconfigurationtypedef) 
## FilterRelativeDateTimeControlTypeDef

```python
# FilterRelativeDateTimeControlTypeDef definition

class FilterRelativeDateTimeControlTypeDef(TypedDict):
    FilterControlId: str,
    Title: str,
    SourceFilterId: str,
    DisplayOptions: NotRequired[RelativeDateTimeControlDisplayOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: RelativeDateTimeControlDisplayOptionsTypeDef](./type_defs.md#relativedatetimecontroldisplayoptionstypedef) 
## FilterSliderControlTypeDef

```python
# FilterSliderControlTypeDef definition

class FilterSliderControlTypeDef(TypedDict):
    FilterControlId: str,
    Title: str,
    SourceFilterId: str,
    MaximumValue: float,
    MinimumValue: float,
    StepSize: float,
    DisplayOptions: NotRequired[SliderControlDisplayOptionsTypeDef],  # (1)
    Type: NotRequired[SheetControlSliderTypeType],  # (2)
```

1. See [:material-code-braces: SliderControlDisplayOptionsTypeDef](./type_defs.md#slidercontroldisplayoptionstypedef) 
2. See [:material-code-brackets: SheetControlSliderTypeType](./literals.md#sheetcontrolslidertypetype) 
## ParameterSliderControlTypeDef

```python
# ParameterSliderControlTypeDef definition

class ParameterSliderControlTypeDef(TypedDict):
    ParameterControlId: str,
    Title: str,
    SourceParameterName: str,
    MaximumValue: float,
    MinimumValue: float,
    StepSize: float,
    DisplayOptions: NotRequired[SliderControlDisplayOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: SliderControlDisplayOptionsTypeDef](./type_defs.md#slidercontroldisplayoptionstypedef) 
## FilterTextAreaControlTypeDef

```python
# FilterTextAreaControlTypeDef definition

class FilterTextAreaControlTypeDef(TypedDict):
    FilterControlId: str,
    Title: str,
    SourceFilterId: str,
    Delimiter: NotRequired[str],
    DisplayOptions: NotRequired[TextAreaControlDisplayOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: TextAreaControlDisplayOptionsTypeDef](./type_defs.md#textareacontroldisplayoptionstypedef) 
## ParameterTextAreaControlTypeDef

```python
# ParameterTextAreaControlTypeDef definition

class ParameterTextAreaControlTypeDef(TypedDict):
    ParameterControlId: str,
    Title: str,
    SourceParameterName: str,
    Delimiter: NotRequired[str],
    DisplayOptions: NotRequired[TextAreaControlDisplayOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: TextAreaControlDisplayOptionsTypeDef](./type_defs.md#textareacontroldisplayoptionstypedef) 
## FilterTextFieldControlTypeDef

```python
# FilterTextFieldControlTypeDef definition

class FilterTextFieldControlTypeDef(TypedDict):
    FilterControlId: str,
    Title: str,
    SourceFilterId: str,
    DisplayOptions: NotRequired[TextFieldControlDisplayOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: TextFieldControlDisplayOptionsTypeDef](./type_defs.md#textfieldcontroldisplayoptionstypedef) 
## ParameterTextFieldControlTypeDef

```python
# ParameterTextFieldControlTypeDef definition

class ParameterTextFieldControlTypeDef(TypedDict):
    ParameterControlId: str,
    Title: str,
    SourceParameterName: str,
    DisplayOptions: NotRequired[TextFieldControlDisplayOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: TextFieldControlDisplayOptionsTypeDef](./type_defs.md#textfieldcontroldisplayoptionstypedef) 
## SmallMultiplesOptionsTypeDef

```python
# SmallMultiplesOptionsTypeDef definition

class SmallMultiplesOptionsTypeDef(TypedDict):
    MaxVisibleRows: NotRequired[int],
    MaxVisibleColumns: NotRequired[int],
    PanelConfiguration: NotRequired[PanelConfigurationTypeDef],  # (1)
    XAxis: NotRequired[SmallMultiplesAxisPropertiesTypeDef],  # (2)
    YAxis: NotRequired[SmallMultiplesAxisPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: PanelConfigurationTypeDef](./type_defs.md#panelconfigurationtypedef) 
2. See [:material-code-braces: SmallMultiplesAxisPropertiesTypeDef](./type_defs.md#smallmultiplesaxispropertiestypedef) 
3. See [:material-code-braces: SmallMultiplesAxisPropertiesTypeDef](./type_defs.md#smallmultiplesaxispropertiestypedef) 
## TableFieldLinkConfigurationTypeDef

```python
# TableFieldLinkConfigurationTypeDef definition

class TableFieldLinkConfigurationTypeDef(TypedDict):
    Target: URLTargetConfigurationType,  # (1)
    Content: TableFieldLinkContentConfigurationTypeDef,  # (2)
```

1. See [:material-code-brackets: URLTargetConfigurationType](./literals.md#urltargetconfigurationtype) 
2. See [:material-code-braces: TableFieldLinkContentConfigurationTypeDef](./type_defs.md#tablefieldlinkcontentconfigurationtypedef) 
## PivotTableOptionsTypeDef

```python
# PivotTableOptionsTypeDef definition

class PivotTableOptionsTypeDef(TypedDict):
    MetricPlacement: NotRequired[PivotTableMetricPlacementType],  # (1)
    SingleMetricVisibility: NotRequired[VisibilityType],  # (2)
    ColumnNamesVisibility: NotRequired[VisibilityType],  # (2)
    ToggleButtonsVisibility: NotRequired[VisibilityType],  # (2)
    ColumnHeaderStyle: NotRequired[TableCellStyleTypeDef],  # (5)
    RowHeaderStyle: NotRequired[TableCellStyleTypeDef],  # (5)
    CellStyle: NotRequired[TableCellStyleTypeDef],  # (5)
    RowFieldNamesStyle: NotRequired[TableCellStyleTypeDef],  # (5)
    RowAlternateColorOptions: NotRequired[RowAlternateColorOptionsTypeDef],  # (9)
    CollapsedRowDimensionsVisibility: NotRequired[VisibilityType],  # (2)
    RowsLayout: NotRequired[PivotTableRowsLayoutType],  # (11)
    RowsLabelOptions: NotRequired[PivotTableRowsLabelOptionsTypeDef],  # (12)
    DefaultCellWidth: NotRequired[str],
```

1. See [:material-code-brackets: PivotTableMetricPlacementType](./literals.md#pivottablemetricplacementtype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
3. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
4. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
5. See [:material-code-braces: TableCellStyleTypeDef](./type_defs.md#tablecellstyletypedef) 
6. See [:material-code-braces: TableCellStyleTypeDef](./type_defs.md#tablecellstyletypedef) 
7. See [:material-code-braces: TableCellStyleTypeDef](./type_defs.md#tablecellstyletypedef) 
8. See [:material-code-braces: TableCellStyleTypeDef](./type_defs.md#tablecellstyletypedef) 
9. See [:material-code-braces: RowAlternateColorOptionsTypeDef](./type_defs.md#rowalternatecoloroptionstypedef) 
10. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
11. See [:material-code-brackets: PivotTableRowsLayoutType](./literals.md#pivottablerowslayouttype) 
12. See [:material-code-braces: PivotTableRowsLabelOptionsTypeDef](./type_defs.md#pivottablerowslabeloptionstypedef) 
## PivotTotalOptionsTypeDef

```python
# PivotTotalOptionsTypeDef definition

class PivotTotalOptionsTypeDef(TypedDict):
    TotalsVisibility: NotRequired[VisibilityType],  # (1)
    Placement: NotRequired[TableTotalsPlacementType],  # (2)
    ScrollStatus: NotRequired[TableTotalsScrollStatusType],  # (3)
    CustomLabel: NotRequired[str],
    TotalCellStyle: NotRequired[TableCellStyleTypeDef],  # (4)
    ValueCellStyle: NotRequired[TableCellStyleTypeDef],  # (4)
    MetricHeaderCellStyle: NotRequired[TableCellStyleTypeDef],  # (4)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-brackets: TableTotalsPlacementType](./literals.md#tabletotalsplacementtype) 
3. See [:material-code-brackets: TableTotalsScrollStatusType](./literals.md#tabletotalsscrollstatustype) 
4. See [:material-code-braces: TableCellStyleTypeDef](./type_defs.md#tablecellstyletypedef) 
5. See [:material-code-braces: TableCellStyleTypeDef](./type_defs.md#tablecellstyletypedef) 
6. See [:material-code-braces: TableCellStyleTypeDef](./type_defs.md#tablecellstyletypedef) 
## SubtotalOptionsTypeDef

```python
# SubtotalOptionsTypeDef definition

class SubtotalOptionsTypeDef(TypedDict):
    TotalsVisibility: NotRequired[VisibilityType],  # (1)
    CustomLabel: NotRequired[str],
    FieldLevel: NotRequired[PivotTableSubtotalLevelType],  # (2)
    FieldLevelOptions: NotRequired[Sequence[PivotTableFieldSubtotalOptionsTypeDef]],  # (3)
    TotalCellStyle: NotRequired[TableCellStyleTypeDef],  # (4)
    ValueCellStyle: NotRequired[TableCellStyleTypeDef],  # (4)
    MetricHeaderCellStyle: NotRequired[TableCellStyleTypeDef],  # (4)
    StyleTargets: NotRequired[Sequence[TableStyleTargetTypeDef]],  # (7)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-brackets: PivotTableSubtotalLevelType](./literals.md#pivottablesubtotalleveltype) 
3. See [:material-code-braces: PivotTableFieldSubtotalOptionsTypeDef](./type_defs.md#pivottablefieldsubtotaloptionstypedef) 
4. See [:material-code-braces: TableCellStyleTypeDef](./type_defs.md#tablecellstyletypedef) 
5. See [:material-code-braces: TableCellStyleTypeDef](./type_defs.md#tablecellstyletypedef) 
6. See [:material-code-braces: TableCellStyleTypeDef](./type_defs.md#tablecellstyletypedef) 
7. See [:material-code-braces: TableStyleTargetTypeDef](./type_defs.md#tablestyletargettypedef) 
## TableOptionsTypeDef

```python
# TableOptionsTypeDef definition

class TableOptionsTypeDef(TypedDict):
    Orientation: NotRequired[TableOrientationType],  # (1)
    HeaderStyle: NotRequired[TableCellStyleTypeDef],  # (2)
    CellStyle: NotRequired[TableCellStyleTypeDef],  # (2)
    RowAlternateColorOptions: NotRequired[RowAlternateColorOptionsTypeDef],  # (4)
```

1. See [:material-code-brackets: TableOrientationType](./literals.md#tableorientationtype) 
2. See [:material-code-braces: TableCellStyleTypeDef](./type_defs.md#tablecellstyletypedef) 
3. See [:material-code-braces: TableCellStyleTypeDef](./type_defs.md#tablecellstyletypedef) 
4. See [:material-code-braces: RowAlternateColorOptionsTypeDef](./type_defs.md#rowalternatecoloroptionstypedef) 
## TotalOptionsTypeDef

```python
# TotalOptionsTypeDef definition

class TotalOptionsTypeDef(TypedDict):
    TotalsVisibility: NotRequired[VisibilityType],  # (1)
    Placement: NotRequired[TableTotalsPlacementType],  # (2)
    ScrollStatus: NotRequired[TableTotalsScrollStatusType],  # (3)
    CustomLabel: NotRequired[str],
    TotalCellStyle: NotRequired[TableCellStyleTypeDef],  # (4)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-brackets: TableTotalsPlacementType](./literals.md#tabletotalsplacementtype) 
3. See [:material-code-brackets: TableTotalsScrollStatusType](./literals.md#tabletotalsscrollstatustype) 
4. See [:material-code-braces: TableCellStyleTypeDef](./type_defs.md#tablecellstyletypedef) 
## GaugeChartArcConditionalFormattingTypeDef

```python
# GaugeChartArcConditionalFormattingTypeDef definition

class GaugeChartArcConditionalFormattingTypeDef(TypedDict):
    ForegroundColor: NotRequired[ConditionalFormattingColorTypeDef],  # (1)
```

1. See [:material-code-braces: ConditionalFormattingColorTypeDef](./type_defs.md#conditionalformattingcolortypedef) 
## GaugeChartPrimaryValueConditionalFormattingTypeDef

```python
# GaugeChartPrimaryValueConditionalFormattingTypeDef definition

class GaugeChartPrimaryValueConditionalFormattingTypeDef(TypedDict):
    TextColor: NotRequired[ConditionalFormattingColorTypeDef],  # (1)
    Icon: NotRequired[ConditionalFormattingIconTypeDef],  # (2)
```

1. See [:material-code-braces: ConditionalFormattingColorTypeDef](./type_defs.md#conditionalformattingcolortypedef) 
2. See [:material-code-braces: ConditionalFormattingIconTypeDef](./type_defs.md#conditionalformattingicontypedef) 
## KPIPrimaryValueConditionalFormattingTypeDef

```python
# KPIPrimaryValueConditionalFormattingTypeDef definition

class KPIPrimaryValueConditionalFormattingTypeDef(TypedDict):
    TextColor: NotRequired[ConditionalFormattingColorTypeDef],  # (1)
    Icon: NotRequired[ConditionalFormattingIconTypeDef],  # (2)
```

1. See [:material-code-braces: ConditionalFormattingColorTypeDef](./type_defs.md#conditionalformattingcolortypedef) 
2. See [:material-code-braces: ConditionalFormattingIconTypeDef](./type_defs.md#conditionalformattingicontypedef) 
## KPIProgressBarConditionalFormattingTypeDef

```python
# KPIProgressBarConditionalFormattingTypeDef definition

class KPIProgressBarConditionalFormattingTypeDef(TypedDict):
    ForegroundColor: NotRequired[ConditionalFormattingColorTypeDef],  # (1)
```

1. See [:material-code-braces: ConditionalFormattingColorTypeDef](./type_defs.md#conditionalformattingcolortypedef) 
## ShapeConditionalFormatTypeDef

```python
# ShapeConditionalFormatTypeDef definition

class ShapeConditionalFormatTypeDef(TypedDict):
    BackgroundColor: ConditionalFormattingColorTypeDef,  # (1)
```

1. See [:material-code-braces: ConditionalFormattingColorTypeDef](./type_defs.md#conditionalformattingcolortypedef) 
## TableRowConditionalFormattingTypeDef

```python
# TableRowConditionalFormattingTypeDef definition

class TableRowConditionalFormattingTypeDef(TypedDict):
    BackgroundColor: NotRequired[ConditionalFormattingColorTypeDef],  # (1)
    TextColor: NotRequired[ConditionalFormattingColorTypeDef],  # (1)
```

1. See [:material-code-braces: ConditionalFormattingColorTypeDef](./type_defs.md#conditionalformattingcolortypedef) 
2. See [:material-code-braces: ConditionalFormattingColorTypeDef](./type_defs.md#conditionalformattingcolortypedef) 
## TextConditionalFormatTypeDef

```python
# TextConditionalFormatTypeDef definition

class TextConditionalFormatTypeDef(TypedDict):
    BackgroundColor: NotRequired[ConditionalFormattingColorTypeDef],  # (1)
    TextColor: NotRequired[ConditionalFormattingColorTypeDef],  # (1)
    Icon: NotRequired[ConditionalFormattingIconTypeDef],  # (3)
```

1. See [:material-code-braces: ConditionalFormattingColorTypeDef](./type_defs.md#conditionalformattingcolortypedef) 
2. See [:material-code-braces: ConditionalFormattingColorTypeDef](./type_defs.md#conditionalformattingcolortypedef) 
3. See [:material-code-braces: ConditionalFormattingIconTypeDef](./type_defs.md#conditionalformattingicontypedef) 
## SheetControlLayoutTypeDef

```python
# SheetControlLayoutTypeDef definition

class SheetControlLayoutTypeDef(TypedDict):
    Configuration: SheetControlLayoutConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: SheetControlLayoutConfigurationTypeDef](./type_defs.md#sheetcontrollayoutconfigurationtypedef) 
## DescribeDataSetRefreshPropertiesResponseTypeDef

```python
# DescribeDataSetRefreshPropertiesResponseTypeDef definition

class DescribeDataSetRefreshPropertiesResponseTypeDef(TypedDict):
    RequestId: str,
    Status: int,
    DataSetRefreshProperties: DataSetRefreshPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSetRefreshPropertiesTypeDef](./type_defs.md#datasetrefreshpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDataSetRefreshPropertiesRequestRequestTypeDef

```python
# PutDataSetRefreshPropertiesRequestRequestTypeDef definition

class PutDataSetRefreshPropertiesRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSetId: str,
    DataSetRefreshProperties: DataSetRefreshPropertiesTypeDef,  # (1)
```

1. See [:material-code-braces: DataSetRefreshPropertiesTypeDef](./type_defs.md#datasetrefreshpropertiestypedef) 
## AssetBundleImportJobOverrideParametersTypeDef

```python
# AssetBundleImportJobOverrideParametersTypeDef definition

class AssetBundleImportJobOverrideParametersTypeDef(TypedDict):
    ResourceIdOverrideConfiguration: NotRequired[AssetBundleImportJobResourceIdOverrideConfigurationTypeDef],  # (1)
    VPCConnections: NotRequired[List[AssetBundleImportJobVPCConnectionOverrideParametersTypeDef]],  # (2)
    RefreshSchedules: NotRequired[List[AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef]],  # (3)
    DataSources: NotRequired[List[AssetBundleImportJobDataSourceOverrideParametersTypeDef]],  # (4)
    DataSets: NotRequired[List[AssetBundleImportJobDataSetOverrideParametersTypeDef]],  # (5)
    Themes: NotRequired[List[AssetBundleImportJobThemeOverrideParametersTypeDef]],  # (6)
    Analyses: NotRequired[List[AssetBundleImportJobAnalysisOverrideParametersTypeDef]],  # (7)
    Dashboards: NotRequired[List[AssetBundleImportJobDashboardOverrideParametersTypeDef]],  # (8)
```

1. See [:material-code-braces: AssetBundleImportJobResourceIdOverrideConfigurationTypeDef](./type_defs.md#assetbundleimportjobresourceidoverrideconfigurationtypedef) 
2. See [:material-code-braces: AssetBundleImportJobVPCConnectionOverrideParametersTypeDef](./type_defs.md#assetbundleimportjobvpcconnectionoverrideparameterstypedef) 
3. See [:material-code-braces: AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef](./type_defs.md#assetbundleimportjobrefreshscheduleoverrideparameterstypedef) 
4. See [:material-code-braces: AssetBundleImportJobDataSourceOverrideParametersTypeDef](./type_defs.md#assetbundleimportjobdatasourceoverrideparameterstypedef) 
5. See [:material-code-braces: AssetBundleImportJobDataSetOverrideParametersTypeDef](./type_defs.md#assetbundleimportjobdatasetoverrideparameterstypedef) 
6. See [:material-code-braces: AssetBundleImportJobThemeOverrideParametersTypeDef](./type_defs.md#assetbundleimportjobthemeoverrideparameterstypedef) 
7. See [:material-code-braces: AssetBundleImportJobAnalysisOverrideParametersTypeDef](./type_defs.md#assetbundleimportjobanalysisoverrideparameterstypedef) 
8. See [:material-code-braces: AssetBundleImportJobDashboardOverrideParametersTypeDef](./type_defs.md#assetbundleimportjobdashboardoverrideparameterstypedef) 
## DataSourceCredentialsTypeDef

```python
# DataSourceCredentialsTypeDef definition

class DataSourceCredentialsTypeDef(TypedDict):
    CredentialPair: NotRequired[CredentialPairTypeDef],  # (1)
    CopySourceArn: NotRequired[str],
    SecretArn: NotRequired[str],
```

1. See [:material-code-braces: CredentialPairTypeDef](./type_defs.md#credentialpairtypedef) 
## DescribeDataSourceResponseTypeDef

```python
# DescribeDataSourceResponseTypeDef definition

class DescribeDataSourceResponseTypeDef(TypedDict):
    DataSource: DataSourceTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataSourcesResponseTypeDef

```python
# ListDataSourcesResponseTypeDef definition

class ListDataSourcesResponseTypeDef(TypedDict):
    DataSources: List[DataSourceTypeDef],  # (1)
    NextToken: str,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateThemeRequestRequestTypeDef

```python
# CreateThemeRequestRequestTypeDef definition

class CreateThemeRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    ThemeId: str,
    Name: str,
    BaseThemeId: str,
    Configuration: ThemeConfigurationTypeDef,  # (1)
    VersionDescription: NotRequired[str],
    Permissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: ThemeConfigurationTypeDef](./type_defs.md#themeconfigurationtypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ThemeVersionTypeDef

```python
# ThemeVersionTypeDef definition

class ThemeVersionTypeDef(TypedDict):
    VersionNumber: NotRequired[int],
    Arn: NotRequired[str],
    Description: NotRequired[str],
    BaseThemeId: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    Configuration: NotRequired[ThemeConfigurationTypeDef],  # (1)
    Errors: NotRequired[List[ThemeErrorTypeDef]],  # (2)
    Status: NotRequired[ResourceStatusType],  # (3)
```

1. See [:material-code-braces: ThemeConfigurationTypeDef](./type_defs.md#themeconfigurationtypedef) 
2. See [:material-code-braces: ThemeErrorTypeDef](./type_defs.md#themeerrortypedef) 
3. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
## UpdateThemeRequestRequestTypeDef

```python
# UpdateThemeRequestRequestTypeDef definition

class UpdateThemeRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    ThemeId: str,
    BaseThemeId: str,
    Name: NotRequired[str],
    VersionDescription: NotRequired[str],
    Configuration: NotRequired[ThemeConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ThemeConfigurationTypeDef](./type_defs.md#themeconfigurationtypedef) 
## ComparisonConfigurationTypeDef

```python
# ComparisonConfigurationTypeDef definition

class ComparisonConfigurationTypeDef(TypedDict):
    ComparisonMethod: NotRequired[ComparisonMethodType],  # (1)
    ComparisonFormat: NotRequired[ComparisonFormatConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: ComparisonMethodType](./literals.md#comparisonmethodtype) 
2. See [:material-code-braces: ComparisonFormatConfigurationTypeDef](./type_defs.md#comparisonformatconfigurationtypedef) 
## DateTimeFormatConfigurationTypeDef

```python
# DateTimeFormatConfigurationTypeDef definition

class DateTimeFormatConfigurationTypeDef(TypedDict):
    DateTimeFormat: NotRequired[str],
    NullValueFormatConfiguration: NotRequired[NullValueFormatConfigurationTypeDef],  # (1)
    NumericFormatConfiguration: NotRequired[NumericFormatConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: NullValueFormatConfigurationTypeDef](./type_defs.md#nullvalueformatconfigurationtypedef) 
2. See [:material-code-braces: NumericFormatConfigurationTypeDef](./type_defs.md#numericformatconfigurationtypedef) 
## NumberFormatConfigurationTypeDef

```python
# NumberFormatConfigurationTypeDef definition

class NumberFormatConfigurationTypeDef(TypedDict):
    FormatConfiguration: NotRequired[NumericFormatConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: NumericFormatConfigurationTypeDef](./type_defs.md#numericformatconfigurationtypedef) 
## ReferenceLineValueLabelConfigurationTypeDef

```python
# ReferenceLineValueLabelConfigurationTypeDef definition

class ReferenceLineValueLabelConfigurationTypeDef(TypedDict):
    RelativePosition: NotRequired[ReferenceLineValueLabelRelativePositionType],  # (1)
    FormatConfiguration: NotRequired[NumericFormatConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: ReferenceLineValueLabelRelativePositionType](./literals.md#referencelinevaluelabelrelativepositiontype) 
2. See [:material-code-braces: NumericFormatConfigurationTypeDef](./type_defs.md#numericformatconfigurationtypedef) 
## StringFormatConfigurationTypeDef

```python
# StringFormatConfigurationTypeDef definition

class StringFormatConfigurationTypeDef(TypedDict):
    NullValueFormatConfiguration: NotRequired[NullValueFormatConfigurationTypeDef],  # (1)
    NumericFormatConfiguration: NotRequired[NumericFormatConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: NullValueFormatConfigurationTypeDef](./type_defs.md#nullvalueformatconfigurationtypedef) 
2. See [:material-code-braces: NumericFormatConfigurationTypeDef](./type_defs.md#numericformatconfigurationtypedef) 
## TopBottomFilterTypeDef

```python
# TopBottomFilterTypeDef definition

class TopBottomFilterTypeDef(TypedDict):
    FilterId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    AggregationSortConfigurations: Sequence[AggregationSortConfigurationTypeDef],  # (2)
    Limit: NotRequired[int],
    TimeGranularity: NotRequired[TimeGranularityType],  # (3)
    ParameterName: NotRequired[str],
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: AggregationSortConfigurationTypeDef](./type_defs.md#aggregationsortconfigurationtypedef) 
3. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype) 
## FieldSortOptionsTypeDef

```python
# FieldSortOptionsTypeDef definition

class FieldSortOptionsTypeDef(TypedDict):
    FieldSort: NotRequired[FieldSortTypeDef],  # (1)
    ColumnSort: NotRequired[ColumnSortTypeDef],  # (2)
```

1. See [:material-code-braces: FieldSortTypeDef](./type_defs.md#fieldsorttypedef) 
2. See [:material-code-braces: ColumnSortTypeDef](./type_defs.md#columnsorttypedef) 
## PivotTableSortByTypeDef

```python
# PivotTableSortByTypeDef definition

class PivotTableSortByTypeDef(TypedDict):
    Field: NotRequired[FieldSortTypeDef],  # (1)
    Column: NotRequired[ColumnSortTypeDef],  # (2)
    DataPath: NotRequired[DataPathSortTypeDef],  # (3)
```

1. See [:material-code-braces: FieldSortTypeDef](./type_defs.md#fieldsorttypedef) 
2. See [:material-code-braces: ColumnSortTypeDef](./type_defs.md#columnsorttypedef) 
3. See [:material-code-braces: DataPathSortTypeDef](./type_defs.md#datapathsorttypedef) 
## TooltipItemTypeDef

```python
# TooltipItemTypeDef definition

class TooltipItemTypeDef(TypedDict):
    FieldTooltipItem: NotRequired[FieldTooltipItemTypeDef],  # (1)
    ColumnTooltipItem: NotRequired[ColumnTooltipItemTypeDef],  # (2)
```

1. See [:material-code-braces: FieldTooltipItemTypeDef](./type_defs.md#fieldtooltipitemtypedef) 
2. See [:material-code-braces: ColumnTooltipItemTypeDef](./type_defs.md#columntooltipitemtypedef) 
## ReferenceLineDataConfigurationTypeDef

```python
# ReferenceLineDataConfigurationTypeDef definition

class ReferenceLineDataConfigurationTypeDef(TypedDict):
    StaticConfiguration: NotRequired[ReferenceLineStaticDataConfigurationTypeDef],  # (1)
    DynamicConfiguration: NotRequired[ReferenceLineDynamicDataConfigurationTypeDef],  # (2)
    AxisBinding: NotRequired[AxisBindingType],  # (3)
```

1. See [:material-code-braces: ReferenceLineStaticDataConfigurationTypeDef](./type_defs.md#referencelinestaticdataconfigurationtypedef) 
2. See [:material-code-braces: ReferenceLineDynamicDataConfigurationTypeDef](./type_defs.md#referencelinedynamicdataconfigurationtypedef) 
3. See [:material-code-brackets: AxisBindingType](./literals.md#axisbindingtype) 
## DatasetMetadataTypeDef

```python
# DatasetMetadataTypeDef definition

class DatasetMetadataTypeDef(TypedDict):
    DatasetArn: str,
    DatasetName: NotRequired[str],
    DatasetDescription: NotRequired[str],
    DataAggregation: NotRequired[DataAggregationTypeDef],  # (1)
    Filters: NotRequired[Sequence[TopicFilterTypeDef]],  # (2)
    Columns: NotRequired[Sequence[TopicColumnTypeDef]],  # (3)
    CalculatedFields: NotRequired[Sequence[TopicCalculatedFieldTypeDef]],  # (4)
    NamedEntities: NotRequired[Sequence[TopicNamedEntityTypeDef]],  # (5)
```

1. See [:material-code-braces: DataAggregationTypeDef](./type_defs.md#dataaggregationtypedef) 
2. See [:material-code-braces: TopicFilterTypeDef](./type_defs.md#topicfiltertypedef) 
3. See [:material-code-braces: TopicColumnTypeDef](./type_defs.md#topiccolumntypedef) 
4. See [:material-code-braces: TopicCalculatedFieldTypeDef](./type_defs.md#topiccalculatedfieldtypedef) 
5. See [:material-code-braces: TopicNamedEntityTypeDef](./type_defs.md#topicnamedentitytypedef) 
## GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef

```python
# GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef definition

class GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    UserArn: str,
    ExperienceConfiguration: RegisteredUserEmbeddingExperienceConfigurationTypeDef,  # (1)
    SessionLifetimeInMinutes: NotRequired[int],
    AllowedDomains: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: RegisteredUserEmbeddingExperienceConfigurationTypeDef](./type_defs.md#registereduserembeddingexperienceconfigurationtypedef) 
## AnonymousUserSnapshotJobResultTypeDef

```python
# AnonymousUserSnapshotJobResultTypeDef definition

class AnonymousUserSnapshotJobResultTypeDef(TypedDict):
    FileGroups: NotRequired[List[SnapshotJobResultFileGroupTypeDef]],  # (1)
```

1. See [:material-code-braces: SnapshotJobResultFileGroupTypeDef](./type_defs.md#snapshotjobresultfilegrouptypedef) 
## DefaultPaginatedLayoutConfigurationTypeDef

```python
# DefaultPaginatedLayoutConfigurationTypeDef definition

class DefaultPaginatedLayoutConfigurationTypeDef(TypedDict):
    SectionBased: NotRequired[DefaultSectionBasedLayoutConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: DefaultSectionBasedLayoutConfigurationTypeDef](./type_defs.md#defaultsectionbasedlayoutconfigurationtypedef) 
## SectionLayoutConfigurationTypeDef

```python
# SectionLayoutConfigurationTypeDef definition

class SectionLayoutConfigurationTypeDef(TypedDict):
    FreeFormLayout: FreeFormSectionLayoutConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: FreeFormSectionLayoutConfigurationTypeDef](./type_defs.md#freeformsectionlayoutconfigurationtypedef) 
## DescribeDashboardSnapshotJobResponseTypeDef

```python
# DescribeDashboardSnapshotJobResponseTypeDef definition

class DescribeDashboardSnapshotJobResponseTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    SnapshotJobId: str,
    UserConfiguration: SnapshotUserConfigurationRedactedTypeDef,  # (1)
    SnapshotConfiguration: SnapshotConfigurationTypeDef,  # (2)
    Arn: str,
    JobStatus: SnapshotJobStatusType,  # (3)
    CreatedTime: datetime,
    LastUpdatedTime: datetime,
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: SnapshotUserConfigurationRedactedTypeDef](./type_defs.md#snapshotuserconfigurationredactedtypedef) 
2. See [:material-code-braces: SnapshotConfigurationTypeDef](./type_defs.md#snapshotconfigurationtypedef) 
3. See [:material-code-brackets: SnapshotJobStatusType](./literals.md#snapshotjobstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDashboardSnapshotJobRequestRequestTypeDef

```python
# StartDashboardSnapshotJobRequestRequestTypeDef definition

class StartDashboardSnapshotJobRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    SnapshotJobId: str,
    UserConfiguration: SnapshotUserConfigurationTypeDef,  # (1)
    SnapshotConfiguration: SnapshotConfigurationTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotUserConfigurationTypeDef](./type_defs.md#snapshotuserconfigurationtypedef) 
2. See [:material-code-braces: SnapshotConfigurationTypeDef](./type_defs.md#snapshotconfigurationtypedef) 
## DescribeTemplateResponseTypeDef

```python
# DescribeTemplateResponseTypeDef definition

class DescribeTemplateResponseTypeDef(TypedDict):
    Template: TemplateTypeDef,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomActionSetParametersOperationTypeDef

```python
# CustomActionSetParametersOperationTypeDef definition

class CustomActionSetParametersOperationTypeDef(TypedDict):
    ParameterValueConfigurations: Sequence[SetParameterValueConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SetParameterValueConfigurationTypeDef](./type_defs.md#setparametervalueconfigurationtypedef) 
## CreateDataSetRequestRequestTypeDef

```python
# CreateDataSetRequestRequestTypeDef definition

class CreateDataSetRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSetId: str,
    Name: str,
    PhysicalTableMap: Mapping[str, PhysicalTableTypeDef],  # (1)
    ImportMode: DataSetImportModeType,  # (2)
    LogicalTableMap: NotRequired[Mapping[str, LogicalTableTypeDef]],  # (3)
    ColumnGroups: NotRequired[Sequence[ColumnGroupTypeDef]],  # (4)
    FieldFolders: NotRequired[Mapping[str, FieldFolderTypeDef]],  # (5)
    Permissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (6)
    RowLevelPermissionDataSet: NotRequired[RowLevelPermissionDataSetTypeDef],  # (7)
    RowLevelPermissionTagConfiguration: NotRequired[RowLevelPermissionTagConfigurationTypeDef],  # (8)
    ColumnLevelPermissionRules: NotRequired[Sequence[ColumnLevelPermissionRuleTypeDef]],  # (9)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (10)
    DataSetUsageConfiguration: NotRequired[DataSetUsageConfigurationTypeDef],  # (11)
    DatasetParameters: NotRequired[Sequence[DatasetParameterTypeDef]],  # (12)
```

1. See [:material-code-braces: PhysicalTableTypeDef](./type_defs.md#physicaltabletypedef) 
2. See [:material-code-brackets: DataSetImportModeType](./literals.md#datasetimportmodetype) 
3. See [:material-code-braces: LogicalTableTypeDef](./type_defs.md#logicaltabletypedef) 
4. See [:material-code-braces: ColumnGroupTypeDef](./type_defs.md#columngrouptypedef) 
5. See [:material-code-braces: FieldFolderTypeDef](./type_defs.md#fieldfoldertypedef) 
6. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
7. See [:material-code-braces: RowLevelPermissionDataSetTypeDef](./type_defs.md#rowlevelpermissiondatasettypedef) 
8. See [:material-code-braces: RowLevelPermissionTagConfigurationTypeDef](./type_defs.md#rowlevelpermissiontagconfigurationtypedef) 
9. See [:material-code-braces: ColumnLevelPermissionRuleTypeDef](./type_defs.md#columnlevelpermissionruletypedef) 
10. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
11. See [:material-code-braces: DataSetUsageConfigurationTypeDef](./type_defs.md#datasetusageconfigurationtypedef) 
12. See [:material-code-braces: DatasetParameterTypeDef](./type_defs.md#datasetparametertypedef) 
## DataSetTypeDef

```python
# DataSetTypeDef definition

class DataSetTypeDef(TypedDict):
    Arn: NotRequired[str],
    DataSetId: NotRequired[str],
    Name: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    PhysicalTableMap: NotRequired[Dict[str, PhysicalTableTypeDef]],  # (1)
    LogicalTableMap: NotRequired[Dict[str, LogicalTableTypeDef]],  # (2)
    OutputColumns: NotRequired[List[OutputColumnTypeDef]],  # (3)
    ImportMode: NotRequired[DataSetImportModeType],  # (4)
    ConsumedSpiceCapacityInBytes: NotRequired[int],
    ColumnGroups: NotRequired[List[ColumnGroupTypeDef]],  # (5)
    FieldFolders: NotRequired[Dict[str, FieldFolderTypeDef]],  # (6)
    RowLevelPermissionDataSet: NotRequired[RowLevelPermissionDataSetTypeDef],  # (7)
    RowLevelPermissionTagConfiguration: NotRequired[RowLevelPermissionTagConfigurationTypeDef],  # (8)
    ColumnLevelPermissionRules: NotRequired[List[ColumnLevelPermissionRuleTypeDef]],  # (9)
    DataSetUsageConfiguration: NotRequired[DataSetUsageConfigurationTypeDef],  # (10)
    DatasetParameters: NotRequired[List[DatasetParameterTypeDef]],  # (11)
```

1. See [:material-code-braces: PhysicalTableTypeDef](./type_defs.md#physicaltabletypedef) 
2. See [:material-code-braces: LogicalTableTypeDef](./type_defs.md#logicaltabletypedef) 
3. See [:material-code-braces: OutputColumnTypeDef](./type_defs.md#outputcolumntypedef) 
4. See [:material-code-brackets: DataSetImportModeType](./literals.md#datasetimportmodetype) 
5. See [:material-code-braces: ColumnGroupTypeDef](./type_defs.md#columngrouptypedef) 
6. See [:material-code-braces: FieldFolderTypeDef](./type_defs.md#fieldfoldertypedef) 
7. See [:material-code-braces: RowLevelPermissionDataSetTypeDef](./type_defs.md#rowlevelpermissiondatasettypedef) 
8. See [:material-code-braces: RowLevelPermissionTagConfigurationTypeDef](./type_defs.md#rowlevelpermissiontagconfigurationtypedef) 
9. See [:material-code-braces: ColumnLevelPermissionRuleTypeDef](./type_defs.md#columnlevelpermissionruletypedef) 
10. See [:material-code-braces: DataSetUsageConfigurationTypeDef](./type_defs.md#datasetusageconfigurationtypedef) 
11. See [:material-code-braces: DatasetParameterTypeDef](./type_defs.md#datasetparametertypedef) 
## UpdateDataSetRequestRequestTypeDef

```python
# UpdateDataSetRequestRequestTypeDef definition

class UpdateDataSetRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSetId: str,
    Name: str,
    PhysicalTableMap: Mapping[str, PhysicalTableTypeDef],  # (1)
    ImportMode: DataSetImportModeType,  # (2)
    LogicalTableMap: NotRequired[Mapping[str, LogicalTableTypeDef]],  # (3)
    ColumnGroups: NotRequired[Sequence[ColumnGroupTypeDef]],  # (4)
    FieldFolders: NotRequired[Mapping[str, FieldFolderTypeDef]],  # (5)
    RowLevelPermissionDataSet: NotRequired[RowLevelPermissionDataSetTypeDef],  # (6)
    RowLevelPermissionTagConfiguration: NotRequired[RowLevelPermissionTagConfigurationTypeDef],  # (7)
    ColumnLevelPermissionRules: NotRequired[Sequence[ColumnLevelPermissionRuleTypeDef]],  # (8)
    DataSetUsageConfiguration: NotRequired[DataSetUsageConfigurationTypeDef],  # (9)
    DatasetParameters: NotRequired[Sequence[DatasetParameterTypeDef]],  # (10)
```

1. See [:material-code-braces: PhysicalTableTypeDef](./type_defs.md#physicaltabletypedef) 
2. See [:material-code-brackets: DataSetImportModeType](./literals.md#datasetimportmodetype) 
3. See [:material-code-braces: LogicalTableTypeDef](./type_defs.md#logicaltabletypedef) 
4. See [:material-code-braces: ColumnGroupTypeDef](./type_defs.md#columngrouptypedef) 
5. See [:material-code-braces: FieldFolderTypeDef](./type_defs.md#fieldfoldertypedef) 
6. See [:material-code-braces: RowLevelPermissionDataSetTypeDef](./type_defs.md#rowlevelpermissiondatasettypedef) 
7. See [:material-code-braces: RowLevelPermissionTagConfigurationTypeDef](./type_defs.md#rowlevelpermissiontagconfigurationtypedef) 
8. See [:material-code-braces: ColumnLevelPermissionRuleTypeDef](./type_defs.md#columnlevelpermissionruletypedef) 
9. See [:material-code-braces: DataSetUsageConfigurationTypeDef](./type_defs.md#datasetusageconfigurationtypedef) 
10. See [:material-code-braces: DatasetParameterTypeDef](./type_defs.md#datasetparametertypedef) 
## LineSeriesAxisDisplayOptionsTypeDef

```python
# LineSeriesAxisDisplayOptionsTypeDef definition

class LineSeriesAxisDisplayOptionsTypeDef(TypedDict):
    AxisOptions: NotRequired[AxisDisplayOptionsTypeDef],  # (1)
    MissingDataConfigurations: NotRequired[Sequence[MissingDataConfigurationTypeDef]],  # (2)
```

1. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
2. See [:material-code-braces: MissingDataConfigurationTypeDef](./type_defs.md#missingdataconfigurationtypedef) 
## FilterControlTypeDef

```python
# FilterControlTypeDef definition

class FilterControlTypeDef(TypedDict):
    DateTimePicker: NotRequired[FilterDateTimePickerControlTypeDef],  # (1)
    List: NotRequired[FilterListControlTypeDef],  # (2)
    Dropdown: NotRequired[FilterDropDownControlTypeDef],  # (3)
    TextField: NotRequired[FilterTextFieldControlTypeDef],  # (4)
    TextArea: NotRequired[FilterTextAreaControlTypeDef],  # (5)
    Slider: NotRequired[FilterSliderControlTypeDef],  # (6)
    RelativeDateTime: NotRequired[FilterRelativeDateTimeControlTypeDef],  # (7)
```

1. See [:material-code-braces: FilterDateTimePickerControlTypeDef](./type_defs.md#filterdatetimepickercontroltypedef) 
2. See [:material-code-braces: FilterListControlTypeDef](./type_defs.md#filterlistcontroltypedef) 
3. See [:material-code-braces: FilterDropDownControlTypeDef](./type_defs.md#filterdropdowncontroltypedef) 
4. See [:material-code-braces: FilterTextFieldControlTypeDef](./type_defs.md#filtertextfieldcontroltypedef) 
5. See [:material-code-braces: FilterTextAreaControlTypeDef](./type_defs.md#filtertextareacontroltypedef) 
6. See [:material-code-braces: FilterSliderControlTypeDef](./type_defs.md#filterslidercontroltypedef) 
7. See [:material-code-braces: FilterRelativeDateTimeControlTypeDef](./type_defs.md#filterrelativedatetimecontroltypedef) 
## ParameterControlTypeDef

```python
# ParameterControlTypeDef definition

class ParameterControlTypeDef(TypedDict):
    DateTimePicker: NotRequired[ParameterDateTimePickerControlTypeDef],  # (1)
    List: NotRequired[ParameterListControlTypeDef],  # (2)
    Dropdown: NotRequired[ParameterDropDownControlTypeDef],  # (3)
    TextField: NotRequired[ParameterTextFieldControlTypeDef],  # (4)
    TextArea: NotRequired[ParameterTextAreaControlTypeDef],  # (5)
    Slider: NotRequired[ParameterSliderControlTypeDef],  # (6)
```

1. See [:material-code-braces: ParameterDateTimePickerControlTypeDef](./type_defs.md#parameterdatetimepickercontroltypedef) 
2. See [:material-code-braces: ParameterListControlTypeDef](./type_defs.md#parameterlistcontroltypedef) 
3. See [:material-code-braces: ParameterDropDownControlTypeDef](./type_defs.md#parameterdropdowncontroltypedef) 
4. See [:material-code-braces: ParameterTextFieldControlTypeDef](./type_defs.md#parametertextfieldcontroltypedef) 
5. See [:material-code-braces: ParameterTextAreaControlTypeDef](./type_defs.md#parametertextareacontroltypedef) 
6. See [:material-code-braces: ParameterSliderControlTypeDef](./type_defs.md#parameterslidercontroltypedef) 
## TableFieldURLConfigurationTypeDef

```python
# TableFieldURLConfigurationTypeDef definition

class TableFieldURLConfigurationTypeDef(TypedDict):
    LinkConfiguration: NotRequired[TableFieldLinkConfigurationTypeDef],  # (1)
    ImageConfiguration: NotRequired[TableFieldImageConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: TableFieldLinkConfigurationTypeDef](./type_defs.md#tablefieldlinkconfigurationtypedef) 
2. See [:material-code-braces: TableFieldImageConfigurationTypeDef](./type_defs.md#tablefieldimageconfigurationtypedef) 
## PivotTableTotalOptionsTypeDef

```python
# PivotTableTotalOptionsTypeDef definition

class PivotTableTotalOptionsTypeDef(TypedDict):
    RowSubtotalOptions: NotRequired[SubtotalOptionsTypeDef],  # (1)
    ColumnSubtotalOptions: NotRequired[SubtotalOptionsTypeDef],  # (1)
    RowTotalOptions: NotRequired[PivotTotalOptionsTypeDef],  # (3)
    ColumnTotalOptions: NotRequired[PivotTotalOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: SubtotalOptionsTypeDef](./type_defs.md#subtotaloptionstypedef) 
2. See [:material-code-braces: SubtotalOptionsTypeDef](./type_defs.md#subtotaloptionstypedef) 
3. See [:material-code-braces: PivotTotalOptionsTypeDef](./type_defs.md#pivottotaloptionstypedef) 
4. See [:material-code-braces: PivotTotalOptionsTypeDef](./type_defs.md#pivottotaloptionstypedef) 
## GaugeChartConditionalFormattingOptionTypeDef

```python
# GaugeChartConditionalFormattingOptionTypeDef definition

class GaugeChartConditionalFormattingOptionTypeDef(TypedDict):
    PrimaryValue: NotRequired[GaugeChartPrimaryValueConditionalFormattingTypeDef],  # (1)
    Arc: NotRequired[GaugeChartArcConditionalFormattingTypeDef],  # (2)
```

1. See [:material-code-braces: GaugeChartPrimaryValueConditionalFormattingTypeDef](./type_defs.md#gaugechartprimaryvalueconditionalformattingtypedef) 
2. See [:material-code-braces: GaugeChartArcConditionalFormattingTypeDef](./type_defs.md#gaugechartarcconditionalformattingtypedef) 
## KPIConditionalFormattingOptionTypeDef

```python
# KPIConditionalFormattingOptionTypeDef definition

class KPIConditionalFormattingOptionTypeDef(TypedDict):
    PrimaryValue: NotRequired[KPIPrimaryValueConditionalFormattingTypeDef],  # (1)
    ProgressBar: NotRequired[KPIProgressBarConditionalFormattingTypeDef],  # (2)
```

1. See [:material-code-braces: KPIPrimaryValueConditionalFormattingTypeDef](./type_defs.md#kpiprimaryvalueconditionalformattingtypedef) 
2. See [:material-code-braces: KPIProgressBarConditionalFormattingTypeDef](./type_defs.md#kpiprogressbarconditionalformattingtypedef) 
## FilledMapShapeConditionalFormattingTypeDef

```python
# FilledMapShapeConditionalFormattingTypeDef definition

class FilledMapShapeConditionalFormattingTypeDef(TypedDict):
    FieldId: str,
    Format: NotRequired[ShapeConditionalFormatTypeDef],  # (1)
```

1. See [:material-code-braces: ShapeConditionalFormatTypeDef](./type_defs.md#shapeconditionalformattypedef) 
## PivotTableCellConditionalFormattingTypeDef

```python
# PivotTableCellConditionalFormattingTypeDef definition

class PivotTableCellConditionalFormattingTypeDef(TypedDict):
    FieldId: str,
    TextFormat: NotRequired[TextConditionalFormatTypeDef],  # (1)
    Scope: NotRequired[PivotTableConditionalFormattingScopeTypeDef],  # (2)
    Scopes: NotRequired[Sequence[PivotTableConditionalFormattingScopeTypeDef]],  # (3)
```

1. See [:material-code-braces: TextConditionalFormatTypeDef](./type_defs.md#textconditionalformattypedef) 
2. See [:material-code-braces: PivotTableConditionalFormattingScopeTypeDef](./type_defs.md#pivottableconditionalformattingscopetypedef) 
3. See [:material-code-braces: PivotTableConditionalFormattingScopeTypeDef](./type_defs.md#pivottableconditionalformattingscopetypedef) 
## TableCellConditionalFormattingTypeDef

```python
# TableCellConditionalFormattingTypeDef definition

class TableCellConditionalFormattingTypeDef(TypedDict):
    FieldId: str,
    TextFormat: NotRequired[TextConditionalFormatTypeDef],  # (1)
```

1. See [:material-code-braces: TextConditionalFormatTypeDef](./type_defs.md#textconditionalformattypedef) 
## DescribeAssetBundleImportJobResponseTypeDef

```python
# DescribeAssetBundleImportJobResponseTypeDef definition

class DescribeAssetBundleImportJobResponseTypeDef(TypedDict):
    JobStatus: AssetBundleImportJobStatusType,  # (1)
    Errors: List[AssetBundleImportJobErrorTypeDef],  # (2)
    RollbackErrors: List[AssetBundleImportJobErrorTypeDef],  # (2)
    Arn: str,
    CreatedTime: datetime,
    AssetBundleImportJobId: str,
    AwsAccountId: str,
    AssetBundleImportSource: AssetBundleImportSourceDescriptionTypeDef,  # (4)
    OverrideParameters: AssetBundleImportJobOverrideParametersTypeDef,  # (5)
    FailureAction: AssetBundleImportFailureActionType,  # (6)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: AssetBundleImportJobStatusType](./literals.md#assetbundleimportjobstatustype) 
2. See [:material-code-braces: AssetBundleImportJobErrorTypeDef](./type_defs.md#assetbundleimportjoberrortypedef) 
3. See [:material-code-braces: AssetBundleImportJobErrorTypeDef](./type_defs.md#assetbundleimportjoberrortypedef) 
4. See [:material-code-braces: AssetBundleImportSourceDescriptionTypeDef](./type_defs.md#assetbundleimportsourcedescriptiontypedef) 
5. See [:material-code-braces: AssetBundleImportJobOverrideParametersTypeDef](./type_defs.md#assetbundleimportjoboverrideparameterstypedef) 
6. See [:material-code-brackets: AssetBundleImportFailureActionType](./literals.md#assetbundleimportfailureactiontype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAssetBundleImportJobRequestRequestTypeDef

```python
# StartAssetBundleImportJobRequestRequestTypeDef definition

class StartAssetBundleImportJobRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AssetBundleImportJobId: str,
    AssetBundleImportSource: AssetBundleImportSourceTypeDef,  # (1)
    OverrideParameters: NotRequired[AssetBundleImportJobOverrideParametersTypeDef],  # (2)
    FailureAction: NotRequired[AssetBundleImportFailureActionType],  # (3)
```

1. See [:material-code-braces: AssetBundleImportSourceTypeDef](./type_defs.md#assetbundleimportsourcetypedef) 
2. See [:material-code-braces: AssetBundleImportJobOverrideParametersTypeDef](./type_defs.md#assetbundleimportjoboverrideparameterstypedef) 
3. See [:material-code-brackets: AssetBundleImportFailureActionType](./literals.md#assetbundleimportfailureactiontype) 
## CreateDataSourceRequestRequestTypeDef

```python
# CreateDataSourceRequestRequestTypeDef definition

class CreateDataSourceRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSourceId: str,
    Name: str,
    Type: DataSourceTypeType,  # (1)
    DataSourceParameters: NotRequired[DataSourceParametersTypeDef],  # (2)
    Credentials: NotRequired[DataSourceCredentialsTypeDef],  # (3)
    Permissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (4)
    VpcConnectionProperties: NotRequired[VpcConnectionPropertiesTypeDef],  # (5)
    SslProperties: NotRequired[SslPropertiesTypeDef],  # (6)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (7)
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
2. See [:material-code-braces: DataSourceParametersTypeDef](./type_defs.md#datasourceparameterstypedef) 
3. See [:material-code-braces: DataSourceCredentialsTypeDef](./type_defs.md#datasourcecredentialstypedef) 
4. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
5. See [:material-code-braces: VpcConnectionPropertiesTypeDef](./type_defs.md#vpcconnectionpropertiestypedef) 
6. See [:material-code-braces: SslPropertiesTypeDef](./type_defs.md#sslpropertiestypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateDataSourceRequestRequestTypeDef

```python
# UpdateDataSourceRequestRequestTypeDef definition

class UpdateDataSourceRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DataSourceId: str,
    Name: str,
    DataSourceParameters: NotRequired[DataSourceParametersTypeDef],  # (1)
    Credentials: NotRequired[DataSourceCredentialsTypeDef],  # (2)
    VpcConnectionProperties: NotRequired[VpcConnectionPropertiesTypeDef],  # (3)
    SslProperties: NotRequired[SslPropertiesTypeDef],  # (4)
```

1. See [:material-code-braces: DataSourceParametersTypeDef](./type_defs.md#datasourceparameterstypedef) 
2. See [:material-code-braces: DataSourceCredentialsTypeDef](./type_defs.md#datasourcecredentialstypedef) 
3. See [:material-code-braces: VpcConnectionPropertiesTypeDef](./type_defs.md#vpcconnectionpropertiestypedef) 
4. See [:material-code-braces: SslPropertiesTypeDef](./type_defs.md#sslpropertiestypedef) 
## ThemeTypeDef

```python
# ThemeTypeDef definition

class ThemeTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    ThemeId: NotRequired[str],
    Version: NotRequired[ThemeVersionTypeDef],  # (1)
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    Type: NotRequired[ThemeTypeType],  # (2)
```

1. See [:material-code-braces: ThemeVersionTypeDef](./type_defs.md#themeversiontypedef) 
2. See [:material-code-brackets: ThemeTypeType](./literals.md#themetypetype) 
## GaugeChartOptionsTypeDef

```python
# GaugeChartOptionsTypeDef definition

class GaugeChartOptionsTypeDef(TypedDict):
    PrimaryValueDisplayType: NotRequired[PrimaryValueDisplayTypeType],  # (1)
    Comparison: NotRequired[ComparisonConfigurationTypeDef],  # (2)
    ArcAxis: NotRequired[ArcAxisConfigurationTypeDef],  # (3)
    Arc: NotRequired[ArcConfigurationTypeDef],  # (4)
    PrimaryValueFontConfiguration: NotRequired[FontConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: PrimaryValueDisplayTypeType](./literals.md#primaryvaluedisplaytypetype) 
2. See [:material-code-braces: ComparisonConfigurationTypeDef](./type_defs.md#comparisonconfigurationtypedef) 
3. See [:material-code-braces: ArcAxisConfigurationTypeDef](./type_defs.md#arcaxisconfigurationtypedef) 
4. See [:material-code-braces: ArcConfigurationTypeDef](./type_defs.md#arcconfigurationtypedef) 
5. See [:material-code-braces: FontConfigurationTypeDef](./type_defs.md#fontconfigurationtypedef) 
## KPIOptionsTypeDef

```python
# KPIOptionsTypeDef definition

class KPIOptionsTypeDef(TypedDict):
    ProgressBar: NotRequired[ProgressBarOptionsTypeDef],  # (1)
    TrendArrows: NotRequired[TrendArrowOptionsTypeDef],  # (2)
    SecondaryValue: NotRequired[SecondaryValueOptionsTypeDef],  # (3)
    Comparison: NotRequired[ComparisonConfigurationTypeDef],  # (4)
    PrimaryValueDisplayType: NotRequired[PrimaryValueDisplayTypeType],  # (5)
    PrimaryValueFontConfiguration: NotRequired[FontConfigurationTypeDef],  # (6)
    SecondaryValueFontConfiguration: NotRequired[FontConfigurationTypeDef],  # (6)
```

1. See [:material-code-braces: ProgressBarOptionsTypeDef](./type_defs.md#progressbaroptionstypedef) 
2. See [:material-code-braces: TrendArrowOptionsTypeDef](./type_defs.md#trendarrowoptionstypedef) 
3. See [:material-code-braces: SecondaryValueOptionsTypeDef](./type_defs.md#secondaryvalueoptionstypedef) 
4. See [:material-code-braces: ComparisonConfigurationTypeDef](./type_defs.md#comparisonconfigurationtypedef) 
5. See [:material-code-brackets: PrimaryValueDisplayTypeType](./literals.md#primaryvaluedisplaytypetype) 
6. See [:material-code-braces: FontConfigurationTypeDef](./type_defs.md#fontconfigurationtypedef) 
7. See [:material-code-braces: FontConfigurationTypeDef](./type_defs.md#fontconfigurationtypedef) 
## DateDimensionFieldTypeDef

```python
# DateDimensionFieldTypeDef definition

class DateDimensionFieldTypeDef(TypedDict):
    FieldId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    DateGranularity: NotRequired[TimeGranularityType],  # (2)
    HierarchyId: NotRequired[str],
    FormatConfiguration: NotRequired[DateTimeFormatConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype) 
3. See [:material-code-braces: DateTimeFormatConfigurationTypeDef](./type_defs.md#datetimeformatconfigurationtypedef) 
## DateMeasureFieldTypeDef

```python
# DateMeasureFieldTypeDef definition

class DateMeasureFieldTypeDef(TypedDict):
    FieldId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    AggregationFunction: NotRequired[DateAggregationFunctionType],  # (2)
    FormatConfiguration: NotRequired[DateTimeFormatConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-brackets: DateAggregationFunctionType](./literals.md#dateaggregationfunctiontype) 
3. See [:material-code-braces: DateTimeFormatConfigurationTypeDef](./type_defs.md#datetimeformatconfigurationtypedef) 
## NumericalDimensionFieldTypeDef

```python
# NumericalDimensionFieldTypeDef definition

class NumericalDimensionFieldTypeDef(TypedDict):
    FieldId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    HierarchyId: NotRequired[str],
    FormatConfiguration: NotRequired[NumberFormatConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: NumberFormatConfigurationTypeDef](./type_defs.md#numberformatconfigurationtypedef) 
## NumericalMeasureFieldTypeDef

```python
# NumericalMeasureFieldTypeDef definition

class NumericalMeasureFieldTypeDef(TypedDict):
    FieldId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    AggregationFunction: NotRequired[NumericalAggregationFunctionTypeDef],  # (2)
    FormatConfiguration: NotRequired[NumberFormatConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: NumericalAggregationFunctionTypeDef](./type_defs.md#numericalaggregationfunctiontypedef) 
3. See [:material-code-braces: NumberFormatConfigurationTypeDef](./type_defs.md#numberformatconfigurationtypedef) 
## ReferenceLineLabelConfigurationTypeDef

```python
# ReferenceLineLabelConfigurationTypeDef definition

class ReferenceLineLabelConfigurationTypeDef(TypedDict):
    ValueLabelConfiguration: NotRequired[ReferenceLineValueLabelConfigurationTypeDef],  # (1)
    CustomLabelConfiguration: NotRequired[ReferenceLineCustomLabelConfigurationTypeDef],  # (2)
    FontConfiguration: NotRequired[FontConfigurationTypeDef],  # (3)
    FontColor: NotRequired[str],
    HorizontalPosition: NotRequired[ReferenceLineLabelHorizontalPositionType],  # (4)
    VerticalPosition: NotRequired[ReferenceLineLabelVerticalPositionType],  # (5)
```

1. See [:material-code-braces: ReferenceLineValueLabelConfigurationTypeDef](./type_defs.md#referencelinevaluelabelconfigurationtypedef) 
2. See [:material-code-braces: ReferenceLineCustomLabelConfigurationTypeDef](./type_defs.md#referencelinecustomlabelconfigurationtypedef) 
3. See [:material-code-braces: FontConfigurationTypeDef](./type_defs.md#fontconfigurationtypedef) 
4. See [:material-code-brackets: ReferenceLineLabelHorizontalPositionType](./literals.md#referencelinelabelhorizontalpositiontype) 
5. See [:material-code-brackets: ReferenceLineLabelVerticalPositionType](./literals.md#referencelinelabelverticalpositiontype) 
## CategoricalDimensionFieldTypeDef

```python
# CategoricalDimensionFieldTypeDef definition

class CategoricalDimensionFieldTypeDef(TypedDict):
    FieldId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    HierarchyId: NotRequired[str],
    FormatConfiguration: NotRequired[StringFormatConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: StringFormatConfigurationTypeDef](./type_defs.md#stringformatconfigurationtypedef) 
## CategoricalMeasureFieldTypeDef

```python
# CategoricalMeasureFieldTypeDef definition

class CategoricalMeasureFieldTypeDef(TypedDict):
    FieldId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    AggregationFunction: NotRequired[CategoricalAggregationFunctionType],  # (2)
    FormatConfiguration: NotRequired[StringFormatConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-brackets: CategoricalAggregationFunctionType](./literals.md#categoricalaggregationfunctiontype) 
3. See [:material-code-braces: StringFormatConfigurationTypeDef](./type_defs.md#stringformatconfigurationtypedef) 
## FormatConfigurationTypeDef

```python
# FormatConfigurationTypeDef definition

class FormatConfigurationTypeDef(TypedDict):
    StringFormatConfiguration: NotRequired[StringFormatConfigurationTypeDef],  # (1)
    NumberFormatConfiguration: NotRequired[NumberFormatConfigurationTypeDef],  # (2)
    DateTimeFormatConfiguration: NotRequired[DateTimeFormatConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: StringFormatConfigurationTypeDef](./type_defs.md#stringformatconfigurationtypedef) 
2. See [:material-code-braces: NumberFormatConfigurationTypeDef](./type_defs.md#numberformatconfigurationtypedef) 
3. See [:material-code-braces: DateTimeFormatConfigurationTypeDef](./type_defs.md#datetimeformatconfigurationtypedef) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    CategoryFilter: NotRequired[CategoryFilterTypeDef],  # (1)
    NumericRangeFilter: NotRequired[NumericRangeFilterTypeDef],  # (2)
    NumericEqualityFilter: NotRequired[NumericEqualityFilterTypeDef],  # (3)
    TimeEqualityFilter: NotRequired[TimeEqualityFilterTypeDef],  # (4)
    TimeRangeFilter: NotRequired[TimeRangeFilterTypeDef],  # (5)
    RelativeDatesFilter: NotRequired[RelativeDatesFilterTypeDef],  # (6)
    TopBottomFilter: NotRequired[TopBottomFilterTypeDef],  # (7)
```

1. See [:material-code-braces: CategoryFilterTypeDef](./type_defs.md#categoryfiltertypedef) 
2. See [:material-code-braces: NumericRangeFilterTypeDef](./type_defs.md#numericrangefiltertypedef) 
3. See [:material-code-braces: NumericEqualityFilterTypeDef](./type_defs.md#numericequalityfiltertypedef) 
4. See [:material-code-braces: TimeEqualityFilterTypeDef](./type_defs.md#timeequalityfiltertypedef) 
5. See [:material-code-braces: TimeRangeFilterTypeDef](./type_defs.md#timerangefiltertypedef) 
6. See [:material-code-braces: RelativeDatesFilterTypeDef](./type_defs.md#relativedatesfiltertypedef) 
7. See [:material-code-braces: TopBottomFilterTypeDef](./type_defs.md#topbottomfiltertypedef) 
## BarChartSortConfigurationTypeDef

```python
# BarChartSortConfigurationTypeDef definition

class BarChartSortConfigurationTypeDef(TypedDict):
    CategorySort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    CategoryItemsLimit: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
    ColorSort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    ColorItemsLimit: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
    SmallMultiplesSort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    SmallMultiplesLimitConfiguration: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
2. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
3. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
4. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
5. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
6. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
## BoxPlotSortConfigurationTypeDef

```python
# BoxPlotSortConfigurationTypeDef definition

class BoxPlotSortConfigurationTypeDef(TypedDict):
    CategorySort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    PaginationConfiguration: NotRequired[PaginationConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
2. See [:material-code-braces: PaginationConfigurationTypeDef](./type_defs.md#paginationconfigurationtypedef) 
## ComboChartSortConfigurationTypeDef

```python
# ComboChartSortConfigurationTypeDef definition

class ComboChartSortConfigurationTypeDef(TypedDict):
    CategorySort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    CategoryItemsLimit: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
    ColorSort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    ColorItemsLimit: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
2. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
3. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
4. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
## FilledMapSortConfigurationTypeDef

```python
# FilledMapSortConfigurationTypeDef definition

class FilledMapSortConfigurationTypeDef(TypedDict):
    CategorySort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
## FunnelChartSortConfigurationTypeDef

```python
# FunnelChartSortConfigurationTypeDef definition

class FunnelChartSortConfigurationTypeDef(TypedDict):
    CategorySort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    CategoryItemsLimit: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
2. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
## HeatMapSortConfigurationTypeDef

```python
# HeatMapSortConfigurationTypeDef definition

class HeatMapSortConfigurationTypeDef(TypedDict):
    HeatMapRowSort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    HeatMapColumnSort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    HeatMapRowItemsLimitConfiguration: NotRequired[ItemsLimitConfigurationTypeDef],  # (3)
    HeatMapColumnItemsLimitConfiguration: NotRequired[ItemsLimitConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
2. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
3. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
4. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
## KPISortConfigurationTypeDef

```python
# KPISortConfigurationTypeDef definition

class KPISortConfigurationTypeDef(TypedDict):
    TrendGroupSort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
## LineChartSortConfigurationTypeDef

```python
# LineChartSortConfigurationTypeDef definition

class LineChartSortConfigurationTypeDef(TypedDict):
    CategorySort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    CategoryItemsLimitConfiguration: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
    ColorItemsLimitConfiguration: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
    SmallMultiplesSort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    SmallMultiplesLimitConfiguration: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
2. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
3. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
4. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
5. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
## PieChartSortConfigurationTypeDef

```python
# PieChartSortConfigurationTypeDef definition

class PieChartSortConfigurationTypeDef(TypedDict):
    CategorySort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    CategoryItemsLimit: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
    SmallMultiplesSort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    SmallMultiplesLimitConfiguration: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
2. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
3. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
4. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
## RadarChartSortConfigurationTypeDef

```python
# RadarChartSortConfigurationTypeDef definition

class RadarChartSortConfigurationTypeDef(TypedDict):
    CategorySort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    CategoryItemsLimit: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
    ColorSort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    ColorItemsLimit: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
2. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
3. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
4. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
## SankeyDiagramSortConfigurationTypeDef

```python
# SankeyDiagramSortConfigurationTypeDef definition

class SankeyDiagramSortConfigurationTypeDef(TypedDict):
    WeightSort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    SourceItemsLimit: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
    DestinationItemsLimit: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
2. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
3. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
## TableSortConfigurationTypeDef

```python
# TableSortConfigurationTypeDef definition

class TableSortConfigurationTypeDef(TypedDict):
    RowSort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    PaginationConfiguration: NotRequired[PaginationConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
2. See [:material-code-braces: PaginationConfigurationTypeDef](./type_defs.md#paginationconfigurationtypedef) 
## TreeMapSortConfigurationTypeDef

```python
# TreeMapSortConfigurationTypeDef definition

class TreeMapSortConfigurationTypeDef(TypedDict):
    TreeMapSort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    TreeMapGroupItemsLimitConfiguration: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
2. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
## WaterfallChartSortConfigurationTypeDef

```python
# WaterfallChartSortConfigurationTypeDef definition

class WaterfallChartSortConfigurationTypeDef(TypedDict):
    CategorySort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (1)
    BreakdownItemsLimit: NotRequired[ItemsLimitConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
2. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
## WordCloudSortConfigurationTypeDef

```python
# WordCloudSortConfigurationTypeDef definition

class WordCloudSortConfigurationTypeDef(TypedDict):
    CategoryItemsLimit: NotRequired[ItemsLimitConfigurationTypeDef],  # (1)
    CategorySort: NotRequired[Sequence[FieldSortOptionsTypeDef]],  # (2)
```

1. See [:material-code-braces: ItemsLimitConfigurationTypeDef](./type_defs.md#itemslimitconfigurationtypedef) 
2. See [:material-code-braces: FieldSortOptionsTypeDef](./type_defs.md#fieldsortoptionstypedef) 
## PivotFieldSortOptionsTypeDef

```python
# PivotFieldSortOptionsTypeDef definition

class PivotFieldSortOptionsTypeDef(TypedDict):
    FieldId: str,
    SortBy: PivotTableSortByTypeDef,  # (1)
```

1. See [:material-code-braces: PivotTableSortByTypeDef](./type_defs.md#pivottablesortbytypedef) 
## FieldBasedTooltipTypeDef

```python
# FieldBasedTooltipTypeDef definition

class FieldBasedTooltipTypeDef(TypedDict):
    AggregationVisibility: NotRequired[VisibilityType],  # (1)
    TooltipTitleType: NotRequired[TooltipTitleTypeType],  # (2)
    TooltipFields: NotRequired[Sequence[TooltipItemTypeDef]],  # (3)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-brackets: TooltipTitleTypeType](./literals.md#tooltiptitletypetype) 
3. See [:material-code-braces: TooltipItemTypeDef](./type_defs.md#tooltipitemtypedef) 
## TopicDetailsTypeDef

```python
# TopicDetailsTypeDef definition

class TopicDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    DataSets: NotRequired[Sequence[DatasetMetadataTypeDef]],  # (1)
```

1. See [:material-code-braces: DatasetMetadataTypeDef](./type_defs.md#datasetmetadatatypedef) 
## SnapshotJobResultTypeDef

```python
# SnapshotJobResultTypeDef definition

class SnapshotJobResultTypeDef(TypedDict):
    AnonymousUsers: NotRequired[List[AnonymousUserSnapshotJobResultTypeDef]],  # (1)
```

1. See [:material-code-braces: AnonymousUserSnapshotJobResultTypeDef](./type_defs.md#anonymoususersnapshotjobresulttypedef) 
## DefaultNewSheetConfigurationTypeDef

```python
# DefaultNewSheetConfigurationTypeDef definition

class DefaultNewSheetConfigurationTypeDef(TypedDict):
    InteractiveLayoutConfiguration: NotRequired[DefaultInteractiveLayoutConfigurationTypeDef],  # (1)
    PaginatedLayoutConfiguration: NotRequired[DefaultPaginatedLayoutConfigurationTypeDef],  # (2)
    SheetContentType: NotRequired[SheetContentTypeType],  # (3)
```

1. See [:material-code-braces: DefaultInteractiveLayoutConfigurationTypeDef](./type_defs.md#defaultinteractivelayoutconfigurationtypedef) 
2. See [:material-code-braces: DefaultPaginatedLayoutConfigurationTypeDef](./type_defs.md#defaultpaginatedlayoutconfigurationtypedef) 
3. See [:material-code-brackets: SheetContentTypeType](./literals.md#sheetcontenttypetype) 
## BodySectionContentTypeDef

```python
# BodySectionContentTypeDef definition

class BodySectionContentTypeDef(TypedDict):
    Layout: NotRequired[SectionLayoutConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SectionLayoutConfigurationTypeDef](./type_defs.md#sectionlayoutconfigurationtypedef) 
## HeaderFooterSectionConfigurationTypeDef

```python
# HeaderFooterSectionConfigurationTypeDef definition

class HeaderFooterSectionConfigurationTypeDef(TypedDict):
    SectionId: str,
    Layout: SectionLayoutConfigurationTypeDef,  # (1)
    Style: NotRequired[SectionStyleTypeDef],  # (2)
```

1. See [:material-code-braces: SectionLayoutConfigurationTypeDef](./type_defs.md#sectionlayoutconfigurationtypedef) 
2. See [:material-code-braces: SectionStyleTypeDef](./type_defs.md#sectionstyletypedef) 
## VisualCustomActionOperationTypeDef

```python
# VisualCustomActionOperationTypeDef definition

class VisualCustomActionOperationTypeDef(TypedDict):
    FilterOperation: NotRequired[CustomActionFilterOperationTypeDef],  # (1)
    NavigationOperation: NotRequired[CustomActionNavigationOperationTypeDef],  # (2)
    URLOperation: NotRequired[CustomActionURLOperationTypeDef],  # (3)
    SetParametersOperation: NotRequired[CustomActionSetParametersOperationTypeDef],  # (4)
```

1. See [:material-code-braces: CustomActionFilterOperationTypeDef](./type_defs.md#customactionfilteroperationtypedef) 
2. See [:material-code-braces: CustomActionNavigationOperationTypeDef](./type_defs.md#customactionnavigationoperationtypedef) 
3. See [:material-code-braces: CustomActionURLOperationTypeDef](./type_defs.md#customactionurloperationtypedef) 
4. See [:material-code-braces: CustomActionSetParametersOperationTypeDef](./type_defs.md#customactionsetparametersoperationtypedef) 
## DescribeDataSetResponseTypeDef

```python
# DescribeDataSetResponseTypeDef definition

class DescribeDataSetResponseTypeDef(TypedDict):
    DataSet: DataSetTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TableFieldOptionTypeDef

```python
# TableFieldOptionTypeDef definition

class TableFieldOptionTypeDef(TypedDict):
    FieldId: str,
    Width: NotRequired[str],
    CustomLabel: NotRequired[str],
    Visibility: NotRequired[VisibilityType],  # (1)
    URLStyling: NotRequired[TableFieldURLConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-braces: TableFieldURLConfigurationTypeDef](./type_defs.md#tablefieldurlconfigurationtypedef) 
## GaugeChartConditionalFormattingTypeDef

```python
# GaugeChartConditionalFormattingTypeDef definition

class GaugeChartConditionalFormattingTypeDef(TypedDict):
    ConditionalFormattingOptions: NotRequired[Sequence[GaugeChartConditionalFormattingOptionTypeDef]],  # (1)
```

1. See [:material-code-braces: GaugeChartConditionalFormattingOptionTypeDef](./type_defs.md#gaugechartconditionalformattingoptiontypedef) 
## KPIConditionalFormattingTypeDef

```python
# KPIConditionalFormattingTypeDef definition

class KPIConditionalFormattingTypeDef(TypedDict):
    ConditionalFormattingOptions: NotRequired[Sequence[KPIConditionalFormattingOptionTypeDef]],  # (1)
```

1. See [:material-code-braces: KPIConditionalFormattingOptionTypeDef](./type_defs.md#kpiconditionalformattingoptiontypedef) 
## FilledMapConditionalFormattingOptionTypeDef

```python
# FilledMapConditionalFormattingOptionTypeDef definition

class FilledMapConditionalFormattingOptionTypeDef(TypedDict):
    Shape: FilledMapShapeConditionalFormattingTypeDef,  # (1)
```

1. See [:material-code-braces: FilledMapShapeConditionalFormattingTypeDef](./type_defs.md#filledmapshapeconditionalformattingtypedef) 
## PivotTableConditionalFormattingOptionTypeDef

```python
# PivotTableConditionalFormattingOptionTypeDef definition

class PivotTableConditionalFormattingOptionTypeDef(TypedDict):
    Cell: NotRequired[PivotTableCellConditionalFormattingTypeDef],  # (1)
```

1. See [:material-code-braces: PivotTableCellConditionalFormattingTypeDef](./type_defs.md#pivottablecellconditionalformattingtypedef) 
## TableConditionalFormattingOptionTypeDef

```python
# TableConditionalFormattingOptionTypeDef definition

class TableConditionalFormattingOptionTypeDef(TypedDict):
    Cell: NotRequired[TableCellConditionalFormattingTypeDef],  # (1)
    Row: NotRequired[TableRowConditionalFormattingTypeDef],  # (2)
```

1. See [:material-code-braces: TableCellConditionalFormattingTypeDef](./type_defs.md#tablecellconditionalformattingtypedef) 
2. See [:material-code-braces: TableRowConditionalFormattingTypeDef](./type_defs.md#tablerowconditionalformattingtypedef) 
## DescribeThemeResponseTypeDef

```python
# DescribeThemeResponseTypeDef definition

class DescribeThemeResponseTypeDef(TypedDict):
    Theme: ThemeTypeDef,  # (1)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeTypeDef](./type_defs.md#themetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReferenceLineTypeDef

```python
# ReferenceLineTypeDef definition

class ReferenceLineTypeDef(TypedDict):
    DataConfiguration: ReferenceLineDataConfigurationTypeDef,  # (2)
    Status: NotRequired[WidgetStatusType],  # (1)
    StyleConfiguration: NotRequired[ReferenceLineStyleConfigurationTypeDef],  # (3)
    LabelConfiguration: NotRequired[ReferenceLineLabelConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: WidgetStatusType](./literals.md#widgetstatustype) 
2. See [:material-code-braces: ReferenceLineDataConfigurationTypeDef](./type_defs.md#referencelinedataconfigurationtypedef) 
3. See [:material-code-braces: ReferenceLineStyleConfigurationTypeDef](./type_defs.md#referencelinestyleconfigurationtypedef) 
4. See [:material-code-braces: ReferenceLineLabelConfigurationTypeDef](./type_defs.md#referencelinelabelconfigurationtypedef) 
## DimensionFieldTypeDef

```python
# DimensionFieldTypeDef definition

class DimensionFieldTypeDef(TypedDict):
    NumericalDimensionField: NotRequired[NumericalDimensionFieldTypeDef],  # (1)
    CategoricalDimensionField: NotRequired[CategoricalDimensionFieldTypeDef],  # (2)
    DateDimensionField: NotRequired[DateDimensionFieldTypeDef],  # (3)
```

1. See [:material-code-braces: NumericalDimensionFieldTypeDef](./type_defs.md#numericaldimensionfieldtypedef) 
2. See [:material-code-braces: CategoricalDimensionFieldTypeDef](./type_defs.md#categoricaldimensionfieldtypedef) 
3. See [:material-code-braces: DateDimensionFieldTypeDef](./type_defs.md#datedimensionfieldtypedef) 
## MeasureFieldTypeDef

```python
# MeasureFieldTypeDef definition

class MeasureFieldTypeDef(TypedDict):
    NumericalMeasureField: NotRequired[NumericalMeasureFieldTypeDef],  # (1)
    CategoricalMeasureField: NotRequired[CategoricalMeasureFieldTypeDef],  # (2)
    DateMeasureField: NotRequired[DateMeasureFieldTypeDef],  # (3)
    CalculatedMeasureField: NotRequired[CalculatedMeasureFieldTypeDef],  # (4)
```

1. See [:material-code-braces: NumericalMeasureFieldTypeDef](./type_defs.md#numericalmeasurefieldtypedef) 
2. See [:material-code-braces: CategoricalMeasureFieldTypeDef](./type_defs.md#categoricalmeasurefieldtypedef) 
3. See [:material-code-braces: DateMeasureFieldTypeDef](./type_defs.md#datemeasurefieldtypedef) 
4. See [:material-code-braces: CalculatedMeasureFieldTypeDef](./type_defs.md#calculatedmeasurefieldtypedef) 
## ColumnConfigurationTypeDef

```python
# ColumnConfigurationTypeDef definition

class ColumnConfigurationTypeDef(TypedDict):
    Column: ColumnIdentifierTypeDef,  # (1)
    FormatConfiguration: NotRequired[FormatConfigurationTypeDef],  # (2)
    Role: NotRequired[ColumnRoleType],  # (3)
    ColorsConfiguration: NotRequired[ColorsConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: FormatConfigurationTypeDef](./type_defs.md#formatconfigurationtypedef) 
3. See [:material-code-brackets: ColumnRoleType](./literals.md#columnroletype) 
4. See [:material-code-braces: ColorsConfigurationTypeDef](./type_defs.md#colorsconfigurationtypedef) 
## UnaggregatedFieldTypeDef

```python
# UnaggregatedFieldTypeDef definition

class UnaggregatedFieldTypeDef(TypedDict):
    FieldId: str,
    Column: ColumnIdentifierTypeDef,  # (1)
    FormatConfiguration: NotRequired[FormatConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ColumnIdentifierTypeDef](./type_defs.md#columnidentifiertypedef) 
2. See [:material-code-braces: FormatConfigurationTypeDef](./type_defs.md#formatconfigurationtypedef) 
## FilterGroupTypeDef

```python
# FilterGroupTypeDef definition

class FilterGroupTypeDef(TypedDict):
    FilterGroupId: str,
    Filters: Sequence[FilterTypeDef],  # (1)
    ScopeConfiguration: FilterScopeConfigurationTypeDef,  # (2)
    CrossDataset: CrossDatasetTypesType,  # (4)
    Status: NotRequired[WidgetStatusType],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: FilterScopeConfigurationTypeDef](./type_defs.md#filterscopeconfigurationtypedef) 
3. See [:material-code-brackets: WidgetStatusType](./literals.md#widgetstatustype) 
4. See [:material-code-brackets: CrossDatasetTypesType](./literals.md#crossdatasettypestype) 
## PivotTableSortConfigurationTypeDef

```python
# PivotTableSortConfigurationTypeDef definition

class PivotTableSortConfigurationTypeDef(TypedDict):
    FieldSortOptions: NotRequired[Sequence[PivotFieldSortOptionsTypeDef]],  # (1)
```

1. See [:material-code-braces: PivotFieldSortOptionsTypeDef](./type_defs.md#pivotfieldsortoptionstypedef) 
## TooltipOptionsTypeDef

```python
# TooltipOptionsTypeDef definition

class TooltipOptionsTypeDef(TypedDict):
    TooltipVisibility: NotRequired[VisibilityType],  # (1)
    SelectedTooltipType: NotRequired[SelectedTooltipTypeType],  # (2)
    FieldBasedTooltip: NotRequired[FieldBasedTooltipTypeDef],  # (3)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-brackets: SelectedTooltipTypeType](./literals.md#selectedtooltiptypetype) 
3. See [:material-code-braces: FieldBasedTooltipTypeDef](./type_defs.md#fieldbasedtooltiptypedef) 
## CreateTopicRequestRequestTypeDef

```python
# CreateTopicRequestRequestTypeDef definition

class CreateTopicRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TopicId: str,
    Topic: TopicDetailsTypeDef,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: TopicDetailsTypeDef](./type_defs.md#topicdetailstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeTopicResponseTypeDef

```python
# DescribeTopicResponseTypeDef definition

class DescribeTopicResponseTypeDef(TypedDict):
    Arn: str,
    TopicId: str,
    Topic: TopicDetailsTypeDef,  # (1)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TopicDetailsTypeDef](./type_defs.md#topicdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTopicRequestRequestTypeDef

```python
# UpdateTopicRequestRequestTypeDef definition

class UpdateTopicRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TopicId: str,
    Topic: TopicDetailsTypeDef,  # (1)
```

1. See [:material-code-braces: TopicDetailsTypeDef](./type_defs.md#topicdetailstypedef) 
## DescribeDashboardSnapshotJobResultResponseTypeDef

```python
# DescribeDashboardSnapshotJobResultResponseTypeDef definition

class DescribeDashboardSnapshotJobResultResponseTypeDef(TypedDict):
    Arn: str,
    JobStatus: SnapshotJobStatusType,  # (1)
    CreatedTime: datetime,
    LastUpdatedTime: datetime,
    Result: SnapshotJobResultTypeDef,  # (2)
    ErrorInfo: SnapshotJobErrorInfoTypeDef,  # (3)
    RequestId: str,
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: SnapshotJobStatusType](./literals.md#snapshotjobstatustype) 
2. See [:material-code-braces: SnapshotJobResultTypeDef](./type_defs.md#snapshotjobresulttypedef) 
3. See [:material-code-braces: SnapshotJobErrorInfoTypeDef](./type_defs.md#snapshotjoberrorinfotypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AnalysisDefaultsTypeDef

```python
# AnalysisDefaultsTypeDef definition

class AnalysisDefaultsTypeDef(TypedDict):
    DefaultNewSheetConfiguration: DefaultNewSheetConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: DefaultNewSheetConfigurationTypeDef](./type_defs.md#defaultnewsheetconfigurationtypedef) 
## BodySectionConfigurationTypeDef

```python
# BodySectionConfigurationTypeDef definition

class BodySectionConfigurationTypeDef(TypedDict):
    SectionId: str,
    Content: BodySectionContentTypeDef,  # (1)
    Style: NotRequired[SectionStyleTypeDef],  # (2)
    PageBreakConfiguration: NotRequired[SectionPageBreakConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: BodySectionContentTypeDef](./type_defs.md#bodysectioncontenttypedef) 
2. See [:material-code-braces: SectionStyleTypeDef](./type_defs.md#sectionstyletypedef) 
3. See [:material-code-braces: SectionPageBreakConfigurationTypeDef](./type_defs.md#sectionpagebreakconfigurationtypedef) 
## VisualCustomActionTypeDef

```python
# VisualCustomActionTypeDef definition

class VisualCustomActionTypeDef(TypedDict):
    CustomActionId: str,
    Name: str,
    Trigger: VisualCustomActionTriggerType,  # (2)
    ActionOperations: Sequence[VisualCustomActionOperationTypeDef],  # (3)
    Status: NotRequired[WidgetStatusType],  # (1)
```

1. See [:material-code-brackets: WidgetStatusType](./literals.md#widgetstatustype) 
2. See [:material-code-brackets: VisualCustomActionTriggerType](./literals.md#visualcustomactiontriggertype) 
3. See [:material-code-braces: VisualCustomActionOperationTypeDef](./type_defs.md#visualcustomactionoperationtypedef) 
## TableFieldOptionsTypeDef

```python
# TableFieldOptionsTypeDef definition

class TableFieldOptionsTypeDef(TypedDict):
    SelectedFieldOptions: NotRequired[Sequence[TableFieldOptionTypeDef]],  # (1)
    Order: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: TableFieldOptionTypeDef](./type_defs.md#tablefieldoptiontypedef) 
## FilledMapConditionalFormattingTypeDef

```python
# FilledMapConditionalFormattingTypeDef definition

class FilledMapConditionalFormattingTypeDef(TypedDict):
    ConditionalFormattingOptions: Sequence[FilledMapConditionalFormattingOptionTypeDef],  # (1)
```

1. See [:material-code-braces: FilledMapConditionalFormattingOptionTypeDef](./type_defs.md#filledmapconditionalformattingoptiontypedef) 
## PivotTableConditionalFormattingTypeDef

```python
# PivotTableConditionalFormattingTypeDef definition

class PivotTableConditionalFormattingTypeDef(TypedDict):
    ConditionalFormattingOptions: NotRequired[Sequence[PivotTableConditionalFormattingOptionTypeDef]],  # (1)
```

1. See [:material-code-braces: PivotTableConditionalFormattingOptionTypeDef](./type_defs.md#pivottableconditionalformattingoptiontypedef) 
## TableConditionalFormattingTypeDef

```python
# TableConditionalFormattingTypeDef definition

class TableConditionalFormattingTypeDef(TypedDict):
    ConditionalFormattingOptions: NotRequired[Sequence[TableConditionalFormattingOptionTypeDef]],  # (1)
```

1. See [:material-code-braces: TableConditionalFormattingOptionTypeDef](./type_defs.md#tableconditionalformattingoptiontypedef) 
## UniqueValuesComputationTypeDef

```python
# UniqueValuesComputationTypeDef definition

class UniqueValuesComputationTypeDef(TypedDict):
    ComputationId: str,
    Category: DimensionFieldTypeDef,  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
## BarChartAggregatedFieldWellsTypeDef

```python
# BarChartAggregatedFieldWellsTypeDef definition

class BarChartAggregatedFieldWellsTypeDef(TypedDict):
    Category: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
    Colors: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    SmallMultiples: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
4. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
## BoxPlotAggregatedFieldWellsTypeDef

```python
# BoxPlotAggregatedFieldWellsTypeDef definition

class BoxPlotAggregatedFieldWellsTypeDef(TypedDict):
    GroupBy: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## ComboChartAggregatedFieldWellsTypeDef

```python
# ComboChartAggregatedFieldWellsTypeDef definition

class ComboChartAggregatedFieldWellsTypeDef(TypedDict):
    Category: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    BarValues: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
    Colors: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    LineValues: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
4. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## FilledMapAggregatedFieldWellsTypeDef

```python
# FilledMapAggregatedFieldWellsTypeDef definition

class FilledMapAggregatedFieldWellsTypeDef(TypedDict):
    Geospatial: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## ForecastComputationTypeDef

```python
# ForecastComputationTypeDef definition

class ForecastComputationTypeDef(TypedDict):
    ComputationId: str,
    Time: DimensionFieldTypeDef,  # (1)
    Name: NotRequired[str],
    Value: NotRequired[MeasureFieldTypeDef],  # (2)
    PeriodsForward: NotRequired[int],
    PeriodsBackward: NotRequired[int],
    UpperBoundary: NotRequired[float],
    LowerBoundary: NotRequired[float],
    PredictionInterval: NotRequired[int],
    Seasonality: NotRequired[ForecastComputationSeasonalityType],  # (3)
    CustomSeasonalityValue: NotRequired[int],
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-brackets: ForecastComputationSeasonalityType](./literals.md#forecastcomputationseasonalitytype) 
## FunnelChartAggregatedFieldWellsTypeDef

```python
# FunnelChartAggregatedFieldWellsTypeDef definition

class FunnelChartAggregatedFieldWellsTypeDef(TypedDict):
    Category: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## GaugeChartFieldWellsTypeDef

```python
# GaugeChartFieldWellsTypeDef definition

class GaugeChartFieldWellsTypeDef(TypedDict):
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (1)
    TargetValues: NotRequired[Sequence[MeasureFieldTypeDef]],  # (1)
```

1. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## GeospatialMapAggregatedFieldWellsTypeDef

```python
# GeospatialMapAggregatedFieldWellsTypeDef definition

class GeospatialMapAggregatedFieldWellsTypeDef(TypedDict):
    Geospatial: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
    Colors: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
## GrowthRateComputationTypeDef

```python
# GrowthRateComputationTypeDef definition

class GrowthRateComputationTypeDef(TypedDict):
    ComputationId: str,
    Time: DimensionFieldTypeDef,  # (1)
    Name: NotRequired[str],
    Value: NotRequired[MeasureFieldTypeDef],  # (2)
    PeriodSize: NotRequired[int],
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## HeatMapAggregatedFieldWellsTypeDef

```python
# HeatMapAggregatedFieldWellsTypeDef definition

class HeatMapAggregatedFieldWellsTypeDef(TypedDict):
    Rows: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Columns: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (3)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
3. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## HistogramAggregatedFieldWellsTypeDef

```python
# HistogramAggregatedFieldWellsTypeDef definition

class HistogramAggregatedFieldWellsTypeDef(TypedDict):
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (1)
```

1. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## KPIFieldWellsTypeDef

```python
# KPIFieldWellsTypeDef definition

class KPIFieldWellsTypeDef(TypedDict):
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (1)
    TargetValues: NotRequired[Sequence[MeasureFieldTypeDef]],  # (1)
    TrendGroups: NotRequired[Sequence[DimensionFieldTypeDef]],  # (3)
```

1. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
## LineChartAggregatedFieldWellsTypeDef

```python
# LineChartAggregatedFieldWellsTypeDef definition

class LineChartAggregatedFieldWellsTypeDef(TypedDict):
    Category: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
    Colors: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    SmallMultiples: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
4. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
## MaximumMinimumComputationTypeDef

```python
# MaximumMinimumComputationTypeDef definition

class MaximumMinimumComputationTypeDef(TypedDict):
    ComputationId: str,
    Time: DimensionFieldTypeDef,  # (1)
    Type: MaximumMinimumComputationTypeType,  # (3)
    Name: NotRequired[str],
    Value: NotRequired[MeasureFieldTypeDef],  # (2)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-brackets: MaximumMinimumComputationTypeType](./literals.md#maximumminimumcomputationtypetype) 
## MetricComparisonComputationTypeDef

```python
# MetricComparisonComputationTypeDef definition

class MetricComparisonComputationTypeDef(TypedDict):
    ComputationId: str,
    Time: DimensionFieldTypeDef,  # (1)
    FromValue: MeasureFieldTypeDef,  # (2)
    TargetValue: MeasureFieldTypeDef,  # (2)
    Name: NotRequired[str],
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## PeriodOverPeriodComputationTypeDef

```python
# PeriodOverPeriodComputationTypeDef definition

class PeriodOverPeriodComputationTypeDef(TypedDict):
    ComputationId: str,
    Time: DimensionFieldTypeDef,  # (1)
    Name: NotRequired[str],
    Value: NotRequired[MeasureFieldTypeDef],  # (2)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## PeriodToDateComputationTypeDef

```python
# PeriodToDateComputationTypeDef definition

class PeriodToDateComputationTypeDef(TypedDict):
    ComputationId: str,
    Time: DimensionFieldTypeDef,  # (1)
    Name: NotRequired[str],
    Value: NotRequired[MeasureFieldTypeDef],  # (2)
    PeriodTimeGranularity: NotRequired[TimeGranularityType],  # (3)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-brackets: TimeGranularityType](./literals.md#timegranularitytype) 
## PieChartAggregatedFieldWellsTypeDef

```python
# PieChartAggregatedFieldWellsTypeDef definition

class PieChartAggregatedFieldWellsTypeDef(TypedDict):
    Category: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
    SmallMultiples: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
## PivotTableAggregatedFieldWellsTypeDef

```python
# PivotTableAggregatedFieldWellsTypeDef definition

class PivotTableAggregatedFieldWellsTypeDef(TypedDict):
    Rows: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Columns: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (3)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
3. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## RadarChartAggregatedFieldWellsTypeDef

```python
# RadarChartAggregatedFieldWellsTypeDef definition

class RadarChartAggregatedFieldWellsTypeDef(TypedDict):
    Category: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Color: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (3)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
3. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## SankeyDiagramAggregatedFieldWellsTypeDef

```python
# SankeyDiagramAggregatedFieldWellsTypeDef definition

class SankeyDiagramAggregatedFieldWellsTypeDef(TypedDict):
    Source: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Destination: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Weight: NotRequired[Sequence[MeasureFieldTypeDef]],  # (3)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
3. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## ScatterPlotCategoricallyAggregatedFieldWellsTypeDef

```python
# ScatterPlotCategoricallyAggregatedFieldWellsTypeDef definition

class ScatterPlotCategoricallyAggregatedFieldWellsTypeDef(TypedDict):
    XAxis: NotRequired[Sequence[MeasureFieldTypeDef]],  # (1)
    YAxis: NotRequired[Sequence[MeasureFieldTypeDef]],  # (1)
    Category: NotRequired[Sequence[DimensionFieldTypeDef]],  # (3)
    Size: NotRequired[Sequence[MeasureFieldTypeDef]],  # (1)
    Label: NotRequired[Sequence[DimensionFieldTypeDef]],  # (3)
```

1. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
4. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
5. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
## ScatterPlotUnaggregatedFieldWellsTypeDef

```python
# ScatterPlotUnaggregatedFieldWellsTypeDef definition

class ScatterPlotUnaggregatedFieldWellsTypeDef(TypedDict):
    XAxis: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    YAxis: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Size: NotRequired[Sequence[MeasureFieldTypeDef]],  # (3)
    Category: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Label: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
3. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
4. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
5. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
## TableAggregatedFieldWellsTypeDef

```python
# TableAggregatedFieldWellsTypeDef definition

class TableAggregatedFieldWellsTypeDef(TypedDict):
    GroupBy: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## TopBottomMoversComputationTypeDef

```python
# TopBottomMoversComputationTypeDef definition

class TopBottomMoversComputationTypeDef(TypedDict):
    ComputationId: str,
    Time: DimensionFieldTypeDef,  # (1)
    Category: DimensionFieldTypeDef,  # (1)
    Type: TopBottomComputationTypeType,  # (5)
    Name: NotRequired[str],
    Value: NotRequired[MeasureFieldTypeDef],  # (3)
    MoverSize: NotRequired[int],
    SortOrder: NotRequired[TopBottomSortOrderType],  # (4)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
3. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
4. See [:material-code-brackets: TopBottomSortOrderType](./literals.md#topbottomsortordertype) 
5. See [:material-code-brackets: TopBottomComputationTypeType](./literals.md#topbottomcomputationtypetype) 
## TopBottomRankedComputationTypeDef

```python
# TopBottomRankedComputationTypeDef definition

class TopBottomRankedComputationTypeDef(TypedDict):
    ComputationId: str,
    Category: DimensionFieldTypeDef,  # (1)
    Type: TopBottomComputationTypeType,  # (3)
    Name: NotRequired[str],
    Value: NotRequired[MeasureFieldTypeDef],  # (2)
    ResultSize: NotRequired[int],
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-brackets: TopBottomComputationTypeType](./literals.md#topbottomcomputationtypetype) 
## TotalAggregationComputationTypeDef

```python
# TotalAggregationComputationTypeDef definition

class TotalAggregationComputationTypeDef(TypedDict):
    ComputationId: str,
    Value: MeasureFieldTypeDef,  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## TreeMapAggregatedFieldWellsTypeDef

```python
# TreeMapAggregatedFieldWellsTypeDef definition

class TreeMapAggregatedFieldWellsTypeDef(TypedDict):
    Groups: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Sizes: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
    Colors: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## WaterfallChartAggregatedFieldWellsTypeDef

```python
# WaterfallChartAggregatedFieldWellsTypeDef definition

class WaterfallChartAggregatedFieldWellsTypeDef(TypedDict):
    Categories: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Values: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
    Breakdowns: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
3. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
## WordCloudAggregatedFieldWellsTypeDef

```python
# WordCloudAggregatedFieldWellsTypeDef definition

class WordCloudAggregatedFieldWellsTypeDef(TypedDict):
    GroupBy: NotRequired[Sequence[DimensionFieldTypeDef]],  # (1)
    Size: NotRequired[Sequence[MeasureFieldTypeDef]],  # (2)
```

1. See [:material-code-braces: DimensionFieldTypeDef](./type_defs.md#dimensionfieldtypedef) 
2. See [:material-code-braces: MeasureFieldTypeDef](./type_defs.md#measurefieldtypedef) 
## TableUnaggregatedFieldWellsTypeDef

```python
# TableUnaggregatedFieldWellsTypeDef definition

class TableUnaggregatedFieldWellsTypeDef(TypedDict):
    Values: NotRequired[Sequence[UnaggregatedFieldTypeDef]],  # (1)
```

1. See [:material-code-braces: UnaggregatedFieldTypeDef](./type_defs.md#unaggregatedfieldtypedef) 
## SectionBasedLayoutConfigurationTypeDef

```python
# SectionBasedLayoutConfigurationTypeDef definition

class SectionBasedLayoutConfigurationTypeDef(TypedDict):
    HeaderSections: Sequence[HeaderFooterSectionConfigurationTypeDef],  # (1)
    BodySections: Sequence[BodySectionConfigurationTypeDef],  # (2)
    FooterSections: Sequence[HeaderFooterSectionConfigurationTypeDef],  # (1)
    CanvasSizeOptions: SectionBasedLayoutCanvasSizeOptionsTypeDef,  # (4)
```

1. See [:material-code-braces: HeaderFooterSectionConfigurationTypeDef](./type_defs.md#headerfootersectionconfigurationtypedef) 
2. See [:material-code-braces: BodySectionConfigurationTypeDef](./type_defs.md#bodysectionconfigurationtypedef) 
3. See [:material-code-braces: HeaderFooterSectionConfigurationTypeDef](./type_defs.md#headerfootersectionconfigurationtypedef) 
4. See [:material-code-braces: SectionBasedLayoutCanvasSizeOptionsTypeDef](./type_defs.md#sectionbasedlayoutcanvassizeoptionstypedef) 
## CustomContentVisualTypeDef

```python
# CustomContentVisualTypeDef definition

class CustomContentVisualTypeDef(TypedDict):
    VisualId: str,
    DataSetIdentifier: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[CustomContentConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: CustomContentConfigurationTypeDef](./type_defs.md#customcontentconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
## EmptyVisualTypeDef

```python
# EmptyVisualTypeDef definition

class EmptyVisualTypeDef(TypedDict):
    VisualId: str,
    DataSetIdentifier: str,
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (1)
```

1. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
## BarChartFieldWellsTypeDef

```python
# BarChartFieldWellsTypeDef definition

class BarChartFieldWellsTypeDef(TypedDict):
    BarChartAggregatedFieldWells: NotRequired[BarChartAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: BarChartAggregatedFieldWellsTypeDef](./type_defs.md#barchartaggregatedfieldwellstypedef) 
## BoxPlotFieldWellsTypeDef

```python
# BoxPlotFieldWellsTypeDef definition

class BoxPlotFieldWellsTypeDef(TypedDict):
    BoxPlotAggregatedFieldWells: NotRequired[BoxPlotAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: BoxPlotAggregatedFieldWellsTypeDef](./type_defs.md#boxplotaggregatedfieldwellstypedef) 
## ComboChartFieldWellsTypeDef

```python
# ComboChartFieldWellsTypeDef definition

class ComboChartFieldWellsTypeDef(TypedDict):
    ComboChartAggregatedFieldWells: NotRequired[ComboChartAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: ComboChartAggregatedFieldWellsTypeDef](./type_defs.md#combochartaggregatedfieldwellstypedef) 
## FilledMapFieldWellsTypeDef

```python
# FilledMapFieldWellsTypeDef definition

class FilledMapFieldWellsTypeDef(TypedDict):
    FilledMapAggregatedFieldWells: NotRequired[FilledMapAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: FilledMapAggregatedFieldWellsTypeDef](./type_defs.md#filledmapaggregatedfieldwellstypedef) 
## FunnelChartFieldWellsTypeDef

```python
# FunnelChartFieldWellsTypeDef definition

class FunnelChartFieldWellsTypeDef(TypedDict):
    FunnelChartAggregatedFieldWells: NotRequired[FunnelChartAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: FunnelChartAggregatedFieldWellsTypeDef](./type_defs.md#funnelchartaggregatedfieldwellstypedef) 
## GaugeChartConfigurationTypeDef

```python
# GaugeChartConfigurationTypeDef definition

class GaugeChartConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[GaugeChartFieldWellsTypeDef],  # (1)
    GaugeChartOptions: NotRequired[GaugeChartOptionsTypeDef],  # (2)
    DataLabels: NotRequired[DataLabelOptionsTypeDef],  # (3)
    TooltipOptions: NotRequired[TooltipOptionsTypeDef],  # (4)
    VisualPalette: NotRequired[VisualPaletteTypeDef],  # (5)
```

1. See [:material-code-braces: GaugeChartFieldWellsTypeDef](./type_defs.md#gaugechartfieldwellstypedef) 
2. See [:material-code-braces: GaugeChartOptionsTypeDef](./type_defs.md#gaugechartoptionstypedef) 
3. See [:material-code-braces: DataLabelOptionsTypeDef](./type_defs.md#datalabeloptionstypedef) 
4. See [:material-code-braces: TooltipOptionsTypeDef](./type_defs.md#tooltipoptionstypedef) 
5. See [:material-code-braces: VisualPaletteTypeDef](./type_defs.md#visualpalettetypedef) 
## GeospatialMapFieldWellsTypeDef

```python
# GeospatialMapFieldWellsTypeDef definition

class GeospatialMapFieldWellsTypeDef(TypedDict):
    GeospatialMapAggregatedFieldWells: NotRequired[GeospatialMapAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: GeospatialMapAggregatedFieldWellsTypeDef](./type_defs.md#geospatialmapaggregatedfieldwellstypedef) 
## HeatMapFieldWellsTypeDef

```python
# HeatMapFieldWellsTypeDef definition

class HeatMapFieldWellsTypeDef(TypedDict):
    HeatMapAggregatedFieldWells: NotRequired[HeatMapAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: HeatMapAggregatedFieldWellsTypeDef](./type_defs.md#heatmapaggregatedfieldwellstypedef) 
## HistogramFieldWellsTypeDef

```python
# HistogramFieldWellsTypeDef definition

class HistogramFieldWellsTypeDef(TypedDict):
    HistogramAggregatedFieldWells: NotRequired[HistogramAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: HistogramAggregatedFieldWellsTypeDef](./type_defs.md#histogramaggregatedfieldwellstypedef) 
## KPIConfigurationTypeDef

```python
# KPIConfigurationTypeDef definition

class KPIConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[KPIFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[KPISortConfigurationTypeDef],  # (2)
    KPIOptions: NotRequired[KPIOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: KPIFieldWellsTypeDef](./type_defs.md#kpifieldwellstypedef) 
2. See [:material-code-braces: KPISortConfigurationTypeDef](./type_defs.md#kpisortconfigurationtypedef) 
3. See [:material-code-braces: KPIOptionsTypeDef](./type_defs.md#kpioptionstypedef) 
## LineChartFieldWellsTypeDef

```python
# LineChartFieldWellsTypeDef definition

class LineChartFieldWellsTypeDef(TypedDict):
    LineChartAggregatedFieldWells: NotRequired[LineChartAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: LineChartAggregatedFieldWellsTypeDef](./type_defs.md#linechartaggregatedfieldwellstypedef) 
## PieChartFieldWellsTypeDef

```python
# PieChartFieldWellsTypeDef definition

class PieChartFieldWellsTypeDef(TypedDict):
    PieChartAggregatedFieldWells: NotRequired[PieChartAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: PieChartAggregatedFieldWellsTypeDef](./type_defs.md#piechartaggregatedfieldwellstypedef) 
## PivotTableFieldWellsTypeDef

```python
# PivotTableFieldWellsTypeDef definition

class PivotTableFieldWellsTypeDef(TypedDict):
    PivotTableAggregatedFieldWells: NotRequired[PivotTableAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: PivotTableAggregatedFieldWellsTypeDef](./type_defs.md#pivottableaggregatedfieldwellstypedef) 
## RadarChartFieldWellsTypeDef

```python
# RadarChartFieldWellsTypeDef definition

class RadarChartFieldWellsTypeDef(TypedDict):
    RadarChartAggregatedFieldWells: NotRequired[RadarChartAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: RadarChartAggregatedFieldWellsTypeDef](./type_defs.md#radarchartaggregatedfieldwellstypedef) 
## SankeyDiagramFieldWellsTypeDef

```python
# SankeyDiagramFieldWellsTypeDef definition

class SankeyDiagramFieldWellsTypeDef(TypedDict):
    SankeyDiagramAggregatedFieldWells: NotRequired[SankeyDiagramAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: SankeyDiagramAggregatedFieldWellsTypeDef](./type_defs.md#sankeydiagramaggregatedfieldwellstypedef) 
## ScatterPlotFieldWellsTypeDef

```python
# ScatterPlotFieldWellsTypeDef definition

class ScatterPlotFieldWellsTypeDef(TypedDict):
    ScatterPlotCategoricallyAggregatedFieldWells: NotRequired[ScatterPlotCategoricallyAggregatedFieldWellsTypeDef],  # (1)
    ScatterPlotUnaggregatedFieldWells: NotRequired[ScatterPlotUnaggregatedFieldWellsTypeDef],  # (2)
```

1. See [:material-code-braces: ScatterPlotCategoricallyAggregatedFieldWellsTypeDef](./type_defs.md#scatterplotcategoricallyaggregatedfieldwellstypedef) 
2. See [:material-code-braces: ScatterPlotUnaggregatedFieldWellsTypeDef](./type_defs.md#scatterplotunaggregatedfieldwellstypedef) 
## ComputationTypeDef

```python
# ComputationTypeDef definition

class ComputationTypeDef(TypedDict):
    TopBottomRanked: NotRequired[TopBottomRankedComputationTypeDef],  # (1)
    TopBottomMovers: NotRequired[TopBottomMoversComputationTypeDef],  # (2)
    TotalAggregation: NotRequired[TotalAggregationComputationTypeDef],  # (3)
    MaximumMinimum: NotRequired[MaximumMinimumComputationTypeDef],  # (4)
    MetricComparison: NotRequired[MetricComparisonComputationTypeDef],  # (5)
    PeriodOverPeriod: NotRequired[PeriodOverPeriodComputationTypeDef],  # (6)
    PeriodToDate: NotRequired[PeriodToDateComputationTypeDef],  # (7)
    GrowthRate: NotRequired[GrowthRateComputationTypeDef],  # (8)
    UniqueValues: NotRequired[UniqueValuesComputationTypeDef],  # (9)
    Forecast: NotRequired[ForecastComputationTypeDef],  # (10)
```

1. See [:material-code-braces: TopBottomRankedComputationTypeDef](./type_defs.md#topbottomrankedcomputationtypedef) 
2. See [:material-code-braces: TopBottomMoversComputationTypeDef](./type_defs.md#topbottommoverscomputationtypedef) 
3. See [:material-code-braces: TotalAggregationComputationTypeDef](./type_defs.md#totalaggregationcomputationtypedef) 
4. See [:material-code-braces: MaximumMinimumComputationTypeDef](./type_defs.md#maximumminimumcomputationtypedef) 
5. See [:material-code-braces: MetricComparisonComputationTypeDef](./type_defs.md#metriccomparisoncomputationtypedef) 
6. See [:material-code-braces: PeriodOverPeriodComputationTypeDef](./type_defs.md#periodoverperiodcomputationtypedef) 
7. See [:material-code-braces: PeriodToDateComputationTypeDef](./type_defs.md#periodtodatecomputationtypedef) 
8. See [:material-code-braces: GrowthRateComputationTypeDef](./type_defs.md#growthratecomputationtypedef) 
9. See [:material-code-braces: UniqueValuesComputationTypeDef](./type_defs.md#uniquevaluescomputationtypedef) 
10. See [:material-code-braces: ForecastComputationTypeDef](./type_defs.md#forecastcomputationtypedef) 
## TreeMapFieldWellsTypeDef

```python
# TreeMapFieldWellsTypeDef definition

class TreeMapFieldWellsTypeDef(TypedDict):
    TreeMapAggregatedFieldWells: NotRequired[TreeMapAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: TreeMapAggregatedFieldWellsTypeDef](./type_defs.md#treemapaggregatedfieldwellstypedef) 
## WaterfallChartFieldWellsTypeDef

```python
# WaterfallChartFieldWellsTypeDef definition

class WaterfallChartFieldWellsTypeDef(TypedDict):
    WaterfallChartAggregatedFieldWells: NotRequired[WaterfallChartAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: WaterfallChartAggregatedFieldWellsTypeDef](./type_defs.md#waterfallchartaggregatedfieldwellstypedef) 
## WordCloudFieldWellsTypeDef

```python
# WordCloudFieldWellsTypeDef definition

class WordCloudFieldWellsTypeDef(TypedDict):
    WordCloudAggregatedFieldWells: NotRequired[WordCloudAggregatedFieldWellsTypeDef],  # (1)
```

1. See [:material-code-braces: WordCloudAggregatedFieldWellsTypeDef](./type_defs.md#wordcloudaggregatedfieldwellstypedef) 
## TableFieldWellsTypeDef

```python
# TableFieldWellsTypeDef definition

class TableFieldWellsTypeDef(TypedDict):
    TableAggregatedFieldWells: NotRequired[TableAggregatedFieldWellsTypeDef],  # (1)
    TableUnaggregatedFieldWells: NotRequired[TableUnaggregatedFieldWellsTypeDef],  # (2)
```

1. See [:material-code-braces: TableAggregatedFieldWellsTypeDef](./type_defs.md#tableaggregatedfieldwellstypedef) 
2. See [:material-code-braces: TableUnaggregatedFieldWellsTypeDef](./type_defs.md#tableunaggregatedfieldwellstypedef) 
## LayoutConfigurationTypeDef

```python
# LayoutConfigurationTypeDef definition

class LayoutConfigurationTypeDef(TypedDict):
    GridLayout: NotRequired[GridLayoutConfigurationTypeDef],  # (1)
    FreeFormLayout: NotRequired[FreeFormLayoutConfigurationTypeDef],  # (2)
    SectionBasedLayout: NotRequired[SectionBasedLayoutConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: GridLayoutConfigurationTypeDef](./type_defs.md#gridlayoutconfigurationtypedef) 
2. See [:material-code-braces: FreeFormLayoutConfigurationTypeDef](./type_defs.md#freeformlayoutconfigurationtypedef) 
3. See [:material-code-braces: SectionBasedLayoutConfigurationTypeDef](./type_defs.md#sectionbasedlayoutconfigurationtypedef) 
## BarChartConfigurationTypeDef

```python
# BarChartConfigurationTypeDef definition

class BarChartConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[BarChartFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[BarChartSortConfigurationTypeDef],  # (2)
    Orientation: NotRequired[BarChartOrientationType],  # (3)
    BarsArrangement: NotRequired[BarsArrangementType],  # (4)
    VisualPalette: NotRequired[VisualPaletteTypeDef],  # (5)
    SmallMultiplesOptions: NotRequired[SmallMultiplesOptionsTypeDef],  # (6)
    CategoryAxis: NotRequired[AxisDisplayOptionsTypeDef],  # (7)
    CategoryLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (8)
    ValueAxis: NotRequired[AxisDisplayOptionsTypeDef],  # (7)
    ValueLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (8)
    ColorLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (8)
    Legend: NotRequired[LegendOptionsTypeDef],  # (12)
    DataLabels: NotRequired[DataLabelOptionsTypeDef],  # (13)
    Tooltip: NotRequired[TooltipOptionsTypeDef],  # (14)
    ReferenceLines: NotRequired[Sequence[ReferenceLineTypeDef]],  # (15)
    ContributionAnalysisDefaults: NotRequired[Sequence[ContributionAnalysisDefaultTypeDef]],  # (16)
```

1. See [:material-code-braces: BarChartFieldWellsTypeDef](./type_defs.md#barchartfieldwellstypedef) 
2. See [:material-code-braces: BarChartSortConfigurationTypeDef](./type_defs.md#barchartsortconfigurationtypedef) 
3. See [:material-code-brackets: BarChartOrientationType](./literals.md#barchartorientationtype) 
4. See [:material-code-brackets: BarsArrangementType](./literals.md#barsarrangementtype) 
5. See [:material-code-braces: VisualPaletteTypeDef](./type_defs.md#visualpalettetypedef) 
6. See [:material-code-braces: SmallMultiplesOptionsTypeDef](./type_defs.md#smallmultiplesoptionstypedef) 
7. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
8. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
9. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
10. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
11. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
12. See [:material-code-braces: LegendOptionsTypeDef](./type_defs.md#legendoptionstypedef) 
13. See [:material-code-braces: DataLabelOptionsTypeDef](./type_defs.md#datalabeloptionstypedef) 
14. See [:material-code-braces: TooltipOptionsTypeDef](./type_defs.md#tooltipoptionstypedef) 
15. See [:material-code-braces: ReferenceLineTypeDef](./type_defs.md#referencelinetypedef) 
16. See [:material-code-braces: ContributionAnalysisDefaultTypeDef](./type_defs.md#contributionanalysisdefaulttypedef) 
## BoxPlotChartConfigurationTypeDef

```python
# BoxPlotChartConfigurationTypeDef definition

class BoxPlotChartConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[BoxPlotFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[BoxPlotSortConfigurationTypeDef],  # (2)
    BoxPlotOptions: NotRequired[BoxPlotOptionsTypeDef],  # (3)
    CategoryAxis: NotRequired[AxisDisplayOptionsTypeDef],  # (4)
    CategoryLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (5)
    PrimaryYAxisDisplayOptions: NotRequired[AxisDisplayOptionsTypeDef],  # (4)
    PrimaryYAxisLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (5)
    Legend: NotRequired[LegendOptionsTypeDef],  # (8)
    Tooltip: NotRequired[TooltipOptionsTypeDef],  # (9)
    ReferenceLines: NotRequired[Sequence[ReferenceLineTypeDef]],  # (10)
    VisualPalette: NotRequired[VisualPaletteTypeDef],  # (11)
```

1. See [:material-code-braces: BoxPlotFieldWellsTypeDef](./type_defs.md#boxplotfieldwellstypedef) 
2. See [:material-code-braces: BoxPlotSortConfigurationTypeDef](./type_defs.md#boxplotsortconfigurationtypedef) 
3. See [:material-code-braces: BoxPlotOptionsTypeDef](./type_defs.md#boxplotoptionstypedef) 
4. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
5. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
6. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
7. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
8. See [:material-code-braces: LegendOptionsTypeDef](./type_defs.md#legendoptionstypedef) 
9. See [:material-code-braces: TooltipOptionsTypeDef](./type_defs.md#tooltipoptionstypedef) 
10. See [:material-code-braces: ReferenceLineTypeDef](./type_defs.md#referencelinetypedef) 
11. See [:material-code-braces: VisualPaletteTypeDef](./type_defs.md#visualpalettetypedef) 
## ComboChartConfigurationTypeDef

```python
# ComboChartConfigurationTypeDef definition

class ComboChartConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[ComboChartFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[ComboChartSortConfigurationTypeDef],  # (2)
    BarsArrangement: NotRequired[BarsArrangementType],  # (3)
    CategoryAxis: NotRequired[AxisDisplayOptionsTypeDef],  # (4)
    CategoryLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (5)
    PrimaryYAxisDisplayOptions: NotRequired[AxisDisplayOptionsTypeDef],  # (4)
    PrimaryYAxisLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (5)
    SecondaryYAxisDisplayOptions: NotRequired[AxisDisplayOptionsTypeDef],  # (4)
    SecondaryYAxisLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (5)
    ColorLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (5)
    Legend: NotRequired[LegendOptionsTypeDef],  # (11)
    BarDataLabels: NotRequired[DataLabelOptionsTypeDef],  # (12)
    LineDataLabels: NotRequired[DataLabelOptionsTypeDef],  # (12)
    Tooltip: NotRequired[TooltipOptionsTypeDef],  # (14)
    ReferenceLines: NotRequired[Sequence[ReferenceLineTypeDef]],  # (15)
    VisualPalette: NotRequired[VisualPaletteTypeDef],  # (16)
```

1. See [:material-code-braces: ComboChartFieldWellsTypeDef](./type_defs.md#combochartfieldwellstypedef) 
2. See [:material-code-braces: ComboChartSortConfigurationTypeDef](./type_defs.md#combochartsortconfigurationtypedef) 
3. See [:material-code-brackets: BarsArrangementType](./literals.md#barsarrangementtype) 
4. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
5. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
6. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
7. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
8. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
9. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
10. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
11. See [:material-code-braces: LegendOptionsTypeDef](./type_defs.md#legendoptionstypedef) 
12. See [:material-code-braces: DataLabelOptionsTypeDef](./type_defs.md#datalabeloptionstypedef) 
13. See [:material-code-braces: DataLabelOptionsTypeDef](./type_defs.md#datalabeloptionstypedef) 
14. See [:material-code-braces: TooltipOptionsTypeDef](./type_defs.md#tooltipoptionstypedef) 
15. See [:material-code-braces: ReferenceLineTypeDef](./type_defs.md#referencelinetypedef) 
16. See [:material-code-braces: VisualPaletteTypeDef](./type_defs.md#visualpalettetypedef) 
## FilledMapConfigurationTypeDef

```python
# FilledMapConfigurationTypeDef definition

class FilledMapConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[FilledMapFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[FilledMapSortConfigurationTypeDef],  # (2)
    Legend: NotRequired[LegendOptionsTypeDef],  # (3)
    Tooltip: NotRequired[TooltipOptionsTypeDef],  # (4)
    WindowOptions: NotRequired[GeospatialWindowOptionsTypeDef],  # (5)
    MapStyleOptions: NotRequired[GeospatialMapStyleOptionsTypeDef],  # (6)
```

1. See [:material-code-braces: FilledMapFieldWellsTypeDef](./type_defs.md#filledmapfieldwellstypedef) 
2. See [:material-code-braces: FilledMapSortConfigurationTypeDef](./type_defs.md#filledmapsortconfigurationtypedef) 
3. See [:material-code-braces: LegendOptionsTypeDef](./type_defs.md#legendoptionstypedef) 
4. See [:material-code-braces: TooltipOptionsTypeDef](./type_defs.md#tooltipoptionstypedef) 
5. See [:material-code-braces: GeospatialWindowOptionsTypeDef](./type_defs.md#geospatialwindowoptionstypedef) 
6. See [:material-code-braces: GeospatialMapStyleOptionsTypeDef](./type_defs.md#geospatialmapstyleoptionstypedef) 
## FunnelChartConfigurationTypeDef

```python
# FunnelChartConfigurationTypeDef definition

class FunnelChartConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[FunnelChartFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[FunnelChartSortConfigurationTypeDef],  # (2)
    CategoryLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (3)
    ValueLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (3)
    Tooltip: NotRequired[TooltipOptionsTypeDef],  # (5)
    DataLabelOptions: NotRequired[FunnelChartDataLabelOptionsTypeDef],  # (6)
    VisualPalette: NotRequired[VisualPaletteTypeDef],  # (7)
```

1. See [:material-code-braces: FunnelChartFieldWellsTypeDef](./type_defs.md#funnelchartfieldwellstypedef) 
2. See [:material-code-braces: FunnelChartSortConfigurationTypeDef](./type_defs.md#funnelchartsortconfigurationtypedef) 
3. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
4. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
5. See [:material-code-braces: TooltipOptionsTypeDef](./type_defs.md#tooltipoptionstypedef) 
6. See [:material-code-braces: FunnelChartDataLabelOptionsTypeDef](./type_defs.md#funnelchartdatalabeloptionstypedef) 
7. See [:material-code-braces: VisualPaletteTypeDef](./type_defs.md#visualpalettetypedef) 
## GaugeChartVisualTypeDef

```python
# GaugeChartVisualTypeDef definition

class GaugeChartVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[GaugeChartConfigurationTypeDef],  # (3)
    ConditionalFormatting: NotRequired[GaugeChartConditionalFormattingTypeDef],  # (4)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: GaugeChartConfigurationTypeDef](./type_defs.md#gaugechartconfigurationtypedef) 
4. See [:material-code-braces: GaugeChartConditionalFormattingTypeDef](./type_defs.md#gaugechartconditionalformattingtypedef) 
5. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
## GeospatialMapConfigurationTypeDef

```python
# GeospatialMapConfigurationTypeDef definition

class GeospatialMapConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[GeospatialMapFieldWellsTypeDef],  # (1)
    Legend: NotRequired[LegendOptionsTypeDef],  # (2)
    Tooltip: NotRequired[TooltipOptionsTypeDef],  # (3)
    WindowOptions: NotRequired[GeospatialWindowOptionsTypeDef],  # (4)
    MapStyleOptions: NotRequired[GeospatialMapStyleOptionsTypeDef],  # (5)
    PointStyleOptions: NotRequired[GeospatialPointStyleOptionsTypeDef],  # (6)
    VisualPalette: NotRequired[VisualPaletteTypeDef],  # (7)
```

1. See [:material-code-braces: GeospatialMapFieldWellsTypeDef](./type_defs.md#geospatialmapfieldwellstypedef) 
2. See [:material-code-braces: LegendOptionsTypeDef](./type_defs.md#legendoptionstypedef) 
3. See [:material-code-braces: TooltipOptionsTypeDef](./type_defs.md#tooltipoptionstypedef) 
4. See [:material-code-braces: GeospatialWindowOptionsTypeDef](./type_defs.md#geospatialwindowoptionstypedef) 
5. See [:material-code-braces: GeospatialMapStyleOptionsTypeDef](./type_defs.md#geospatialmapstyleoptionstypedef) 
6. See [:material-code-braces: GeospatialPointStyleOptionsTypeDef](./type_defs.md#geospatialpointstyleoptionstypedef) 
7. See [:material-code-braces: VisualPaletteTypeDef](./type_defs.md#visualpalettetypedef) 
## HeatMapConfigurationTypeDef

```python
# HeatMapConfigurationTypeDef definition

class HeatMapConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[HeatMapFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[HeatMapSortConfigurationTypeDef],  # (2)
    RowLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (3)
    ColumnLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (3)
    ColorScale: NotRequired[ColorScaleTypeDef],  # (5)
    Legend: NotRequired[LegendOptionsTypeDef],  # (6)
    DataLabels: NotRequired[DataLabelOptionsTypeDef],  # (7)
    Tooltip: NotRequired[TooltipOptionsTypeDef],  # (8)
```

1. See [:material-code-braces: HeatMapFieldWellsTypeDef](./type_defs.md#heatmapfieldwellstypedef) 
2. See [:material-code-braces: HeatMapSortConfigurationTypeDef](./type_defs.md#heatmapsortconfigurationtypedef) 
3. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
4. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
5. See [:material-code-braces: ColorScaleTypeDef](./type_defs.md#colorscaletypedef) 
6. See [:material-code-braces: LegendOptionsTypeDef](./type_defs.md#legendoptionstypedef) 
7. See [:material-code-braces: DataLabelOptionsTypeDef](./type_defs.md#datalabeloptionstypedef) 
8. See [:material-code-braces: TooltipOptionsTypeDef](./type_defs.md#tooltipoptionstypedef) 
## HistogramConfigurationTypeDef

```python
# HistogramConfigurationTypeDef definition

class HistogramConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[HistogramFieldWellsTypeDef],  # (1)
    XAxisDisplayOptions: NotRequired[AxisDisplayOptionsTypeDef],  # (2)
    XAxisLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (3)
    YAxisDisplayOptions: NotRequired[AxisDisplayOptionsTypeDef],  # (2)
    BinOptions: NotRequired[HistogramBinOptionsTypeDef],  # (5)
    DataLabels: NotRequired[DataLabelOptionsTypeDef],  # (6)
    Tooltip: NotRequired[TooltipOptionsTypeDef],  # (7)
    VisualPalette: NotRequired[VisualPaletteTypeDef],  # (8)
```

1. See [:material-code-braces: HistogramFieldWellsTypeDef](./type_defs.md#histogramfieldwellstypedef) 
2. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
3. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
4. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
5. See [:material-code-braces: HistogramBinOptionsTypeDef](./type_defs.md#histogrambinoptionstypedef) 
6. See [:material-code-braces: DataLabelOptionsTypeDef](./type_defs.md#datalabeloptionstypedef) 
7. See [:material-code-braces: TooltipOptionsTypeDef](./type_defs.md#tooltipoptionstypedef) 
8. See [:material-code-braces: VisualPaletteTypeDef](./type_defs.md#visualpalettetypedef) 
## KPIVisualTypeDef

```python
# KPIVisualTypeDef definition

class KPIVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[KPIConfigurationTypeDef],  # (3)
    ConditionalFormatting: NotRequired[KPIConditionalFormattingTypeDef],  # (4)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (5)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (6)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: KPIConfigurationTypeDef](./type_defs.md#kpiconfigurationtypedef) 
4. See [:material-code-braces: KPIConditionalFormattingTypeDef](./type_defs.md#kpiconditionalformattingtypedef) 
5. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
6. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
## LineChartConfigurationTypeDef

```python
# LineChartConfigurationTypeDef definition

class LineChartConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[LineChartFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[LineChartSortConfigurationTypeDef],  # (2)
    ForecastConfigurations: NotRequired[Sequence[ForecastConfigurationTypeDef]],  # (3)
    Type: NotRequired[LineChartTypeType],  # (4)
    SmallMultiplesOptions: NotRequired[SmallMultiplesOptionsTypeDef],  # (5)
    XAxisDisplayOptions: NotRequired[AxisDisplayOptionsTypeDef],  # (6)
    XAxisLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (7)
    PrimaryYAxisDisplayOptions: NotRequired[LineSeriesAxisDisplayOptionsTypeDef],  # (8)
    PrimaryYAxisLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (7)
    SecondaryYAxisDisplayOptions: NotRequired[LineSeriesAxisDisplayOptionsTypeDef],  # (8)
    SecondaryYAxisLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (7)
    DefaultSeriesSettings: NotRequired[LineChartDefaultSeriesSettingsTypeDef],  # (12)
    Series: NotRequired[Sequence[SeriesItemTypeDef]],  # (13)
    Legend: NotRequired[LegendOptionsTypeDef],  # (14)
    DataLabels: NotRequired[DataLabelOptionsTypeDef],  # (15)
    ReferenceLines: NotRequired[Sequence[ReferenceLineTypeDef]],  # (16)
    Tooltip: NotRequired[TooltipOptionsTypeDef],  # (17)
    ContributionAnalysisDefaults: NotRequired[Sequence[ContributionAnalysisDefaultTypeDef]],  # (18)
    VisualPalette: NotRequired[VisualPaletteTypeDef],  # (19)
```

1. See [:material-code-braces: LineChartFieldWellsTypeDef](./type_defs.md#linechartfieldwellstypedef) 
2. See [:material-code-braces: LineChartSortConfigurationTypeDef](./type_defs.md#linechartsortconfigurationtypedef) 
3. See [:material-code-braces: ForecastConfigurationTypeDef](./type_defs.md#forecastconfigurationtypedef) 
4. See [:material-code-brackets: LineChartTypeType](./literals.md#linecharttypetype) 
5. See [:material-code-braces: SmallMultiplesOptionsTypeDef](./type_defs.md#smallmultiplesoptionstypedef) 
6. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
7. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
8. See [:material-code-braces: LineSeriesAxisDisplayOptionsTypeDef](./type_defs.md#lineseriesaxisdisplayoptionstypedef) 
9. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
10. See [:material-code-braces: LineSeriesAxisDisplayOptionsTypeDef](./type_defs.md#lineseriesaxisdisplayoptionstypedef) 
11. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
12. See [:material-code-braces: LineChartDefaultSeriesSettingsTypeDef](./type_defs.md#linechartdefaultseriessettingstypedef) 
13. See [:material-code-braces: SeriesItemTypeDef](./type_defs.md#seriesitemtypedef) 
14. See [:material-code-braces: LegendOptionsTypeDef](./type_defs.md#legendoptionstypedef) 
15. See [:material-code-braces: DataLabelOptionsTypeDef](./type_defs.md#datalabeloptionstypedef) 
16. See [:material-code-braces: ReferenceLineTypeDef](./type_defs.md#referencelinetypedef) 
17. See [:material-code-braces: TooltipOptionsTypeDef](./type_defs.md#tooltipoptionstypedef) 
18. See [:material-code-braces: ContributionAnalysisDefaultTypeDef](./type_defs.md#contributionanalysisdefaulttypedef) 
19. See [:material-code-braces: VisualPaletteTypeDef](./type_defs.md#visualpalettetypedef) 
## PieChartConfigurationTypeDef

```python
# PieChartConfigurationTypeDef definition

class PieChartConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[PieChartFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[PieChartSortConfigurationTypeDef],  # (2)
    DonutOptions: NotRequired[DonutOptionsTypeDef],  # (3)
    SmallMultiplesOptions: NotRequired[SmallMultiplesOptionsTypeDef],  # (4)
    CategoryLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (5)
    ValueLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (5)
    Legend: NotRequired[LegendOptionsTypeDef],  # (7)
    DataLabels: NotRequired[DataLabelOptionsTypeDef],  # (8)
    Tooltip: NotRequired[TooltipOptionsTypeDef],  # (9)
    VisualPalette: NotRequired[VisualPaletteTypeDef],  # (10)
    ContributionAnalysisDefaults: NotRequired[Sequence[ContributionAnalysisDefaultTypeDef]],  # (11)
```

1. See [:material-code-braces: PieChartFieldWellsTypeDef](./type_defs.md#piechartfieldwellstypedef) 
2. See [:material-code-braces: PieChartSortConfigurationTypeDef](./type_defs.md#piechartsortconfigurationtypedef) 
3. See [:material-code-braces: DonutOptionsTypeDef](./type_defs.md#donutoptionstypedef) 
4. See [:material-code-braces: SmallMultiplesOptionsTypeDef](./type_defs.md#smallmultiplesoptionstypedef) 
5. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
6. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
7. See [:material-code-braces: LegendOptionsTypeDef](./type_defs.md#legendoptionstypedef) 
8. See [:material-code-braces: DataLabelOptionsTypeDef](./type_defs.md#datalabeloptionstypedef) 
9. See [:material-code-braces: TooltipOptionsTypeDef](./type_defs.md#tooltipoptionstypedef) 
10. See [:material-code-braces: VisualPaletteTypeDef](./type_defs.md#visualpalettetypedef) 
11. See [:material-code-braces: ContributionAnalysisDefaultTypeDef](./type_defs.md#contributionanalysisdefaulttypedef) 
## PivotTableConfigurationTypeDef

```python
# PivotTableConfigurationTypeDef definition

class PivotTableConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[PivotTableFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[PivotTableSortConfigurationTypeDef],  # (2)
    TableOptions: NotRequired[PivotTableOptionsTypeDef],  # (3)
    TotalOptions: NotRequired[PivotTableTotalOptionsTypeDef],  # (4)
    FieldOptions: NotRequired[PivotTableFieldOptionsTypeDef],  # (5)
    PaginatedReportOptions: NotRequired[PivotTablePaginatedReportOptionsTypeDef],  # (6)
```

1. See [:material-code-braces: PivotTableFieldWellsTypeDef](./type_defs.md#pivottablefieldwellstypedef) 
2. See [:material-code-braces: PivotTableSortConfigurationTypeDef](./type_defs.md#pivottablesortconfigurationtypedef) 
3. See [:material-code-braces: PivotTableOptionsTypeDef](./type_defs.md#pivottableoptionstypedef) 
4. See [:material-code-braces: PivotTableTotalOptionsTypeDef](./type_defs.md#pivottabletotaloptionstypedef) 
5. See [:material-code-braces: PivotTableFieldOptionsTypeDef](./type_defs.md#pivottablefieldoptionstypedef) 
6. See [:material-code-braces: PivotTablePaginatedReportOptionsTypeDef](./type_defs.md#pivottablepaginatedreportoptionstypedef) 
## RadarChartConfigurationTypeDef

```python
# RadarChartConfigurationTypeDef definition

class RadarChartConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[RadarChartFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[RadarChartSortConfigurationTypeDef],  # (2)
    Shape: NotRequired[RadarChartShapeType],  # (3)
    BaseSeriesSettings: NotRequired[RadarChartSeriesSettingsTypeDef],  # (4)
    StartAngle: NotRequired[float],
    VisualPalette: NotRequired[VisualPaletteTypeDef],  # (5)
    AlternateBandColorsVisibility: NotRequired[VisibilityType],  # (6)
    AlternateBandEvenColor: NotRequired[str],
    AlternateBandOddColor: NotRequired[str],
    CategoryAxis: NotRequired[AxisDisplayOptionsTypeDef],  # (7)
    CategoryLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (8)
    ColorAxis: NotRequired[AxisDisplayOptionsTypeDef],  # (7)
    ColorLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (8)
    Legend: NotRequired[LegendOptionsTypeDef],  # (11)
    AxesRangeScale: NotRequired[RadarChartAxesRangeScaleType],  # (12)
```

1. See [:material-code-braces: RadarChartFieldWellsTypeDef](./type_defs.md#radarchartfieldwellstypedef) 
2. See [:material-code-braces: RadarChartSortConfigurationTypeDef](./type_defs.md#radarchartsortconfigurationtypedef) 
3. See [:material-code-brackets: RadarChartShapeType](./literals.md#radarchartshapetype) 
4. See [:material-code-braces: RadarChartSeriesSettingsTypeDef](./type_defs.md#radarchartseriessettingstypedef) 
5. See [:material-code-braces: VisualPaletteTypeDef](./type_defs.md#visualpalettetypedef) 
6. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
7. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
8. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
9. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
10. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
11. See [:material-code-braces: LegendOptionsTypeDef](./type_defs.md#legendoptionstypedef) 
12. See [:material-code-brackets: RadarChartAxesRangeScaleType](./literals.md#radarchartaxesrangescaletype) 
## SankeyDiagramChartConfigurationTypeDef

```python
# SankeyDiagramChartConfigurationTypeDef definition

class SankeyDiagramChartConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[SankeyDiagramFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[SankeyDiagramSortConfigurationTypeDef],  # (2)
    DataLabels: NotRequired[DataLabelOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: SankeyDiagramFieldWellsTypeDef](./type_defs.md#sankeydiagramfieldwellstypedef) 
2. See [:material-code-braces: SankeyDiagramSortConfigurationTypeDef](./type_defs.md#sankeydiagramsortconfigurationtypedef) 
3. See [:material-code-braces: DataLabelOptionsTypeDef](./type_defs.md#datalabeloptionstypedef) 
## ScatterPlotConfigurationTypeDef

```python
# ScatterPlotConfigurationTypeDef definition

class ScatterPlotConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[ScatterPlotFieldWellsTypeDef],  # (1)
    XAxisLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (2)
    XAxisDisplayOptions: NotRequired[AxisDisplayOptionsTypeDef],  # (3)
    YAxisLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (2)
    YAxisDisplayOptions: NotRequired[AxisDisplayOptionsTypeDef],  # (3)
    Legend: NotRequired[LegendOptionsTypeDef],  # (6)
    DataLabels: NotRequired[DataLabelOptionsTypeDef],  # (7)
    Tooltip: NotRequired[TooltipOptionsTypeDef],  # (8)
    VisualPalette: NotRequired[VisualPaletteTypeDef],  # (9)
```

1. See [:material-code-braces: ScatterPlotFieldWellsTypeDef](./type_defs.md#scatterplotfieldwellstypedef) 
2. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
3. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
4. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
5. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
6. See [:material-code-braces: LegendOptionsTypeDef](./type_defs.md#legendoptionstypedef) 
7. See [:material-code-braces: DataLabelOptionsTypeDef](./type_defs.md#datalabeloptionstypedef) 
8. See [:material-code-braces: TooltipOptionsTypeDef](./type_defs.md#tooltipoptionstypedef) 
9. See [:material-code-braces: VisualPaletteTypeDef](./type_defs.md#visualpalettetypedef) 
## InsightConfigurationTypeDef

```python
# InsightConfigurationTypeDef definition

class InsightConfigurationTypeDef(TypedDict):
    Computations: NotRequired[Sequence[ComputationTypeDef]],  # (1)
    CustomNarrative: NotRequired[CustomNarrativeOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: ComputationTypeDef](./type_defs.md#computationtypedef) 
2. See [:material-code-braces: CustomNarrativeOptionsTypeDef](./type_defs.md#customnarrativeoptionstypedef) 
## TreeMapConfigurationTypeDef

```python
# TreeMapConfigurationTypeDef definition

class TreeMapConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[TreeMapFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[TreeMapSortConfigurationTypeDef],  # (2)
    GroupLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (3)
    SizeLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (3)
    ColorLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (3)
    ColorScale: NotRequired[ColorScaleTypeDef],  # (6)
    Legend: NotRequired[LegendOptionsTypeDef],  # (7)
    DataLabels: NotRequired[DataLabelOptionsTypeDef],  # (8)
    Tooltip: NotRequired[TooltipOptionsTypeDef],  # (9)
```

1. See [:material-code-braces: TreeMapFieldWellsTypeDef](./type_defs.md#treemapfieldwellstypedef) 
2. See [:material-code-braces: TreeMapSortConfigurationTypeDef](./type_defs.md#treemapsortconfigurationtypedef) 
3. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
4. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
5. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
6. See [:material-code-braces: ColorScaleTypeDef](./type_defs.md#colorscaletypedef) 
7. See [:material-code-braces: LegendOptionsTypeDef](./type_defs.md#legendoptionstypedef) 
8. See [:material-code-braces: DataLabelOptionsTypeDef](./type_defs.md#datalabeloptionstypedef) 
9. See [:material-code-braces: TooltipOptionsTypeDef](./type_defs.md#tooltipoptionstypedef) 
## WaterfallChartConfigurationTypeDef

```python
# WaterfallChartConfigurationTypeDef definition

class WaterfallChartConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[WaterfallChartFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[WaterfallChartSortConfigurationTypeDef],  # (2)
    WaterfallChartOptions: NotRequired[WaterfallChartOptionsTypeDef],  # (3)
    CategoryAxisLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (4)
    CategoryAxisDisplayOptions: NotRequired[AxisDisplayOptionsTypeDef],  # (5)
    PrimaryYAxisLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (4)
    PrimaryYAxisDisplayOptions: NotRequired[AxisDisplayOptionsTypeDef],  # (5)
    Legend: NotRequired[LegendOptionsTypeDef],  # (8)
    DataLabels: NotRequired[DataLabelOptionsTypeDef],  # (9)
    VisualPalette: NotRequired[VisualPaletteTypeDef],  # (10)
```

1. See [:material-code-braces: WaterfallChartFieldWellsTypeDef](./type_defs.md#waterfallchartfieldwellstypedef) 
2. See [:material-code-braces: WaterfallChartSortConfigurationTypeDef](./type_defs.md#waterfallchartsortconfigurationtypedef) 
3. See [:material-code-braces: WaterfallChartOptionsTypeDef](./type_defs.md#waterfallchartoptionstypedef) 
4. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
5. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
6. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
7. See [:material-code-braces: AxisDisplayOptionsTypeDef](./type_defs.md#axisdisplayoptionstypedef) 
8. See [:material-code-braces: LegendOptionsTypeDef](./type_defs.md#legendoptionstypedef) 
9. See [:material-code-braces: DataLabelOptionsTypeDef](./type_defs.md#datalabeloptionstypedef) 
10. See [:material-code-braces: VisualPaletteTypeDef](./type_defs.md#visualpalettetypedef) 
## WordCloudChartConfigurationTypeDef

```python
# WordCloudChartConfigurationTypeDef definition

class WordCloudChartConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[WordCloudFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[WordCloudSortConfigurationTypeDef],  # (2)
    CategoryLabelOptions: NotRequired[ChartAxisLabelOptionsTypeDef],  # (3)
    WordCloudOptions: NotRequired[WordCloudOptionsTypeDef],  # (4)
```

1. See [:material-code-braces: WordCloudFieldWellsTypeDef](./type_defs.md#wordcloudfieldwellstypedef) 
2. See [:material-code-braces: WordCloudSortConfigurationTypeDef](./type_defs.md#wordcloudsortconfigurationtypedef) 
3. See [:material-code-braces: ChartAxisLabelOptionsTypeDef](./type_defs.md#chartaxislabeloptionstypedef) 
4. See [:material-code-braces: WordCloudOptionsTypeDef](./type_defs.md#wordcloudoptionstypedef) 
## TableConfigurationTypeDef

```python
# TableConfigurationTypeDef definition

class TableConfigurationTypeDef(TypedDict):
    FieldWells: NotRequired[TableFieldWellsTypeDef],  # (1)
    SortConfiguration: NotRequired[TableSortConfigurationTypeDef],  # (2)
    TableOptions: NotRequired[TableOptionsTypeDef],  # (3)
    TotalOptions: NotRequired[TotalOptionsTypeDef],  # (4)
    FieldOptions: NotRequired[TableFieldOptionsTypeDef],  # (5)
    PaginatedReportOptions: NotRequired[TablePaginatedReportOptionsTypeDef],  # (6)
    TableInlineVisualizations: NotRequired[Sequence[TableInlineVisualizationTypeDef]],  # (7)
```

1. See [:material-code-braces: TableFieldWellsTypeDef](./type_defs.md#tablefieldwellstypedef) 
2. See [:material-code-braces: TableSortConfigurationTypeDef](./type_defs.md#tablesortconfigurationtypedef) 
3. See [:material-code-braces: TableOptionsTypeDef](./type_defs.md#tableoptionstypedef) 
4. See [:material-code-braces: TotalOptionsTypeDef](./type_defs.md#totaloptionstypedef) 
5. See [:material-code-braces: TableFieldOptionsTypeDef](./type_defs.md#tablefieldoptionstypedef) 
6. See [:material-code-braces: TablePaginatedReportOptionsTypeDef](./type_defs.md#tablepaginatedreportoptionstypedef) 
7. See [:material-code-braces: TableInlineVisualizationTypeDef](./type_defs.md#tableinlinevisualizationtypedef) 
## LayoutTypeDef

```python
# LayoutTypeDef definition

class LayoutTypeDef(TypedDict):
    Configuration: LayoutConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef) 
## BarChartVisualTypeDef

```python
# BarChartVisualTypeDef definition

class BarChartVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[BarChartConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: BarChartConfigurationTypeDef](./type_defs.md#barchartconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
5. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
## BoxPlotVisualTypeDef

```python
# BoxPlotVisualTypeDef definition

class BoxPlotVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[BoxPlotChartConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: BoxPlotChartConfigurationTypeDef](./type_defs.md#boxplotchartconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
5. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
## ComboChartVisualTypeDef

```python
# ComboChartVisualTypeDef definition

class ComboChartVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[ComboChartConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: ComboChartConfigurationTypeDef](./type_defs.md#combochartconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
5. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
## FilledMapVisualTypeDef

```python
# FilledMapVisualTypeDef definition

class FilledMapVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[FilledMapConfigurationTypeDef],  # (3)
    ConditionalFormatting: NotRequired[FilledMapConditionalFormattingTypeDef],  # (4)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (5)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (6)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: FilledMapConfigurationTypeDef](./type_defs.md#filledmapconfigurationtypedef) 
4. See [:material-code-braces: FilledMapConditionalFormattingTypeDef](./type_defs.md#filledmapconditionalformattingtypedef) 
5. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
6. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
## FunnelChartVisualTypeDef

```python
# FunnelChartVisualTypeDef definition

class FunnelChartVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[FunnelChartConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: FunnelChartConfigurationTypeDef](./type_defs.md#funnelchartconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
5. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
## GeospatialMapVisualTypeDef

```python
# GeospatialMapVisualTypeDef definition

class GeospatialMapVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[GeospatialMapConfigurationTypeDef],  # (3)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (4)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: GeospatialMapConfigurationTypeDef](./type_defs.md#geospatialmapconfigurationtypedef) 
4. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
5. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
## HeatMapVisualTypeDef

```python
# HeatMapVisualTypeDef definition

class HeatMapVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[HeatMapConfigurationTypeDef],  # (3)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (4)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: HeatMapConfigurationTypeDef](./type_defs.md#heatmapconfigurationtypedef) 
4. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
5. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
## HistogramVisualTypeDef

```python
# HistogramVisualTypeDef definition

class HistogramVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[HistogramConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: HistogramConfigurationTypeDef](./type_defs.md#histogramconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
## LineChartVisualTypeDef

```python
# LineChartVisualTypeDef definition

class LineChartVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[LineChartConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: LineChartConfigurationTypeDef](./type_defs.md#linechartconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
5. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
## PieChartVisualTypeDef

```python
# PieChartVisualTypeDef definition

class PieChartVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[PieChartConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: PieChartConfigurationTypeDef](./type_defs.md#piechartconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
5. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
## PivotTableVisualTypeDef

```python
# PivotTableVisualTypeDef definition

class PivotTableVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[PivotTableConfigurationTypeDef],  # (3)
    ConditionalFormatting: NotRequired[PivotTableConditionalFormattingTypeDef],  # (4)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: PivotTableConfigurationTypeDef](./type_defs.md#pivottableconfigurationtypedef) 
4. See [:material-code-braces: PivotTableConditionalFormattingTypeDef](./type_defs.md#pivottableconditionalformattingtypedef) 
5. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
## RadarChartVisualTypeDef

```python
# RadarChartVisualTypeDef definition

class RadarChartVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[RadarChartConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: RadarChartConfigurationTypeDef](./type_defs.md#radarchartconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
5. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
## SankeyDiagramVisualTypeDef

```python
# SankeyDiagramVisualTypeDef definition

class SankeyDiagramVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[SankeyDiagramChartConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: SankeyDiagramChartConfigurationTypeDef](./type_defs.md#sankeydiagramchartconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
## ScatterPlotVisualTypeDef

```python
# ScatterPlotVisualTypeDef definition

class ScatterPlotVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[ScatterPlotConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: ScatterPlotConfigurationTypeDef](./type_defs.md#scatterplotconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
5. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
## InsightVisualTypeDef

```python
# InsightVisualTypeDef definition

class InsightVisualTypeDef(TypedDict):
    VisualId: str,
    DataSetIdentifier: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    InsightConfiguration: NotRequired[InsightConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: InsightConfigurationTypeDef](./type_defs.md#insightconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
## TreeMapVisualTypeDef

```python
# TreeMapVisualTypeDef definition

class TreeMapVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[TreeMapConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: TreeMapConfigurationTypeDef](./type_defs.md#treemapconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
5. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
## WaterfallVisualTypeDef

```python
# WaterfallVisualTypeDef definition

class WaterfallVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[WaterfallChartConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: WaterfallChartConfigurationTypeDef](./type_defs.md#waterfallchartconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
5. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
## WordCloudVisualTypeDef

```python
# WordCloudVisualTypeDef definition

class WordCloudVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[WordCloudChartConfigurationTypeDef],  # (3)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (4)
    ColumnHierarchies: NotRequired[Sequence[ColumnHierarchyTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: WordCloudChartConfigurationTypeDef](./type_defs.md#wordcloudchartconfigurationtypedef) 
4. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
5. See [:material-code-braces: ColumnHierarchyTypeDef](./type_defs.md#columnhierarchytypedef) 
## TableVisualTypeDef

```python
# TableVisualTypeDef definition

class TableVisualTypeDef(TypedDict):
    VisualId: str,
    Title: NotRequired[VisualTitleLabelOptionsTypeDef],  # (1)
    Subtitle: NotRequired[VisualSubtitleLabelOptionsTypeDef],  # (2)
    ChartConfiguration: NotRequired[TableConfigurationTypeDef],  # (3)
    ConditionalFormatting: NotRequired[TableConditionalFormattingTypeDef],  # (4)
    Actions: NotRequired[Sequence[VisualCustomActionTypeDef]],  # (5)
```

1. See [:material-code-braces: VisualTitleLabelOptionsTypeDef](./type_defs.md#visualtitlelabeloptionstypedef) 
2. See [:material-code-braces: VisualSubtitleLabelOptionsTypeDef](./type_defs.md#visualsubtitlelabeloptionstypedef) 
3. See [:material-code-braces: TableConfigurationTypeDef](./type_defs.md#tableconfigurationtypedef) 
4. See [:material-code-braces: TableConditionalFormattingTypeDef](./type_defs.md#tableconditionalformattingtypedef) 
5. See [:material-code-braces: VisualCustomActionTypeDef](./type_defs.md#visualcustomactiontypedef) 
## VisualTypeDef

```python
# VisualTypeDef definition

class VisualTypeDef(TypedDict):
    TableVisual: NotRequired[TableVisualTypeDef],  # (1)
    PivotTableVisual: NotRequired[PivotTableVisualTypeDef],  # (2)
    BarChartVisual: NotRequired[BarChartVisualTypeDef],  # (3)
    KPIVisual: NotRequired[KPIVisualTypeDef],  # (4)
    PieChartVisual: NotRequired[PieChartVisualTypeDef],  # (5)
    GaugeChartVisual: NotRequired[GaugeChartVisualTypeDef],  # (6)
    LineChartVisual: NotRequired[LineChartVisualTypeDef],  # (7)
    HeatMapVisual: NotRequired[HeatMapVisualTypeDef],  # (8)
    TreeMapVisual: NotRequired[TreeMapVisualTypeDef],  # (9)
    GeospatialMapVisual: NotRequired[GeospatialMapVisualTypeDef],  # (10)
    FilledMapVisual: NotRequired[FilledMapVisualTypeDef],  # (11)
    FunnelChartVisual: NotRequired[FunnelChartVisualTypeDef],  # (12)
    ScatterPlotVisual: NotRequired[ScatterPlotVisualTypeDef],  # (13)
    ComboChartVisual: NotRequired[ComboChartVisualTypeDef],  # (14)
    BoxPlotVisual: NotRequired[BoxPlotVisualTypeDef],  # (15)
    WaterfallVisual: NotRequired[WaterfallVisualTypeDef],  # (16)
    HistogramVisual: NotRequired[HistogramVisualTypeDef],  # (17)
    WordCloudVisual: NotRequired[WordCloudVisualTypeDef],  # (18)
    InsightVisual: NotRequired[InsightVisualTypeDef],  # (19)
    SankeyDiagramVisual: NotRequired[SankeyDiagramVisualTypeDef],  # (20)
    CustomContentVisual: NotRequired[CustomContentVisualTypeDef],  # (21)
    EmptyVisual: NotRequired[EmptyVisualTypeDef],  # (22)
    RadarChartVisual: NotRequired[RadarChartVisualTypeDef],  # (23)
```

1. See [:material-code-braces: TableVisualTypeDef](./type_defs.md#tablevisualtypedef) 
2. See [:material-code-braces: PivotTableVisualTypeDef](./type_defs.md#pivottablevisualtypedef) 
3. See [:material-code-braces: BarChartVisualTypeDef](./type_defs.md#barchartvisualtypedef) 
4. See [:material-code-braces: KPIVisualTypeDef](./type_defs.md#kpivisualtypedef) 
5. See [:material-code-braces: PieChartVisualTypeDef](./type_defs.md#piechartvisualtypedef) 
6. See [:material-code-braces: GaugeChartVisualTypeDef](./type_defs.md#gaugechartvisualtypedef) 
7. See [:material-code-braces: LineChartVisualTypeDef](./type_defs.md#linechartvisualtypedef) 
8. See [:material-code-braces: HeatMapVisualTypeDef](./type_defs.md#heatmapvisualtypedef) 
9. See [:material-code-braces: TreeMapVisualTypeDef](./type_defs.md#treemapvisualtypedef) 
10. See [:material-code-braces: GeospatialMapVisualTypeDef](./type_defs.md#geospatialmapvisualtypedef) 
11. See [:material-code-braces: FilledMapVisualTypeDef](./type_defs.md#filledmapvisualtypedef) 
12. See [:material-code-braces: FunnelChartVisualTypeDef](./type_defs.md#funnelchartvisualtypedef) 
13. See [:material-code-braces: ScatterPlotVisualTypeDef](./type_defs.md#scatterplotvisualtypedef) 
14. See [:material-code-braces: ComboChartVisualTypeDef](./type_defs.md#combochartvisualtypedef) 
15. See [:material-code-braces: BoxPlotVisualTypeDef](./type_defs.md#boxplotvisualtypedef) 
16. See [:material-code-braces: WaterfallVisualTypeDef](./type_defs.md#waterfallvisualtypedef) 
17. See [:material-code-braces: HistogramVisualTypeDef](./type_defs.md#histogramvisualtypedef) 
18. See [:material-code-braces: WordCloudVisualTypeDef](./type_defs.md#wordcloudvisualtypedef) 
19. See [:material-code-braces: InsightVisualTypeDef](./type_defs.md#insightvisualtypedef) 
20. See [:material-code-braces: SankeyDiagramVisualTypeDef](./type_defs.md#sankeydiagramvisualtypedef) 
21. See [:material-code-braces: CustomContentVisualTypeDef](./type_defs.md#customcontentvisualtypedef) 
22. See [:material-code-braces: EmptyVisualTypeDef](./type_defs.md#emptyvisualtypedef) 
23. See [:material-code-braces: RadarChartVisualTypeDef](./type_defs.md#radarchartvisualtypedef) 
## SheetDefinitionTypeDef

```python
# SheetDefinitionTypeDef definition

class SheetDefinitionTypeDef(TypedDict):
    SheetId: str,
    Title: NotRequired[str],
    Description: NotRequired[str],
    Name: NotRequired[str],
    ParameterControls: NotRequired[Sequence[ParameterControlTypeDef]],  # (1)
    FilterControls: NotRequired[Sequence[FilterControlTypeDef]],  # (2)
    Visuals: NotRequired[Sequence[VisualTypeDef]],  # (3)
    TextBoxes: NotRequired[Sequence[SheetTextBoxTypeDef]],  # (4)
    Layouts: NotRequired[Sequence[LayoutTypeDef]],  # (5)
    SheetControlLayouts: NotRequired[Sequence[SheetControlLayoutTypeDef]],  # (6)
    ContentType: NotRequired[SheetContentTypeType],  # (7)
```

1. See [:material-code-braces: ParameterControlTypeDef](./type_defs.md#parametercontroltypedef) 
2. See [:material-code-braces: FilterControlTypeDef](./type_defs.md#filtercontroltypedef) 
3. See [:material-code-braces: VisualTypeDef](./type_defs.md#visualtypedef) 
4. See [:material-code-braces: SheetTextBoxTypeDef](./type_defs.md#sheettextboxtypedef) 
5. See [:material-code-braces: LayoutTypeDef](./type_defs.md#layouttypedef) 
6. See [:material-code-braces: SheetControlLayoutTypeDef](./type_defs.md#sheetcontrollayouttypedef) 
7. See [:material-code-brackets: SheetContentTypeType](./literals.md#sheetcontenttypetype) 
## AnalysisDefinitionTypeDef

```python
# AnalysisDefinitionTypeDef definition

class AnalysisDefinitionTypeDef(TypedDict):
    DataSetIdentifierDeclarations: Sequence[DataSetIdentifierDeclarationTypeDef],  # (1)
    Sheets: NotRequired[Sequence[SheetDefinitionTypeDef]],  # (2)
    CalculatedFields: NotRequired[Sequence[CalculatedFieldTypeDef]],  # (3)
    ParameterDeclarations: NotRequired[Sequence[ParameterDeclarationTypeDef]],  # (4)
    FilterGroups: NotRequired[Sequence[FilterGroupTypeDef]],  # (5)
    ColumnConfigurations: NotRequired[Sequence[ColumnConfigurationTypeDef]],  # (6)
    AnalysisDefaults: NotRequired[AnalysisDefaultsTypeDef],  # (7)
```

1. See [:material-code-braces: DataSetIdentifierDeclarationTypeDef](./type_defs.md#datasetidentifierdeclarationtypedef) 
2. See [:material-code-braces: SheetDefinitionTypeDef](./type_defs.md#sheetdefinitiontypedef) 
3. See [:material-code-braces: CalculatedFieldTypeDef](./type_defs.md#calculatedfieldtypedef) 
4. See [:material-code-braces: ParameterDeclarationTypeDef](./type_defs.md#parameterdeclarationtypedef) 
5. See [:material-code-braces: FilterGroupTypeDef](./type_defs.md#filtergrouptypedef) 
6. See [:material-code-braces: ColumnConfigurationTypeDef](./type_defs.md#columnconfigurationtypedef) 
7. See [:material-code-braces: AnalysisDefaultsTypeDef](./type_defs.md#analysisdefaultstypedef) 
## DashboardVersionDefinitionTypeDef

```python
# DashboardVersionDefinitionTypeDef definition

class DashboardVersionDefinitionTypeDef(TypedDict):
    DataSetIdentifierDeclarations: Sequence[DataSetIdentifierDeclarationTypeDef],  # (1)
    Sheets: NotRequired[Sequence[SheetDefinitionTypeDef]],  # (2)
    CalculatedFields: NotRequired[Sequence[CalculatedFieldTypeDef]],  # (3)
    ParameterDeclarations: NotRequired[Sequence[ParameterDeclarationTypeDef]],  # (4)
    FilterGroups: NotRequired[Sequence[FilterGroupTypeDef]],  # (5)
    ColumnConfigurations: NotRequired[Sequence[ColumnConfigurationTypeDef]],  # (6)
    AnalysisDefaults: NotRequired[AnalysisDefaultsTypeDef],  # (7)
```

1. See [:material-code-braces: DataSetIdentifierDeclarationTypeDef](./type_defs.md#datasetidentifierdeclarationtypedef) 
2. See [:material-code-braces: SheetDefinitionTypeDef](./type_defs.md#sheetdefinitiontypedef) 
3. See [:material-code-braces: CalculatedFieldTypeDef](./type_defs.md#calculatedfieldtypedef) 
4. See [:material-code-braces: ParameterDeclarationTypeDef](./type_defs.md#parameterdeclarationtypedef) 
5. See [:material-code-braces: FilterGroupTypeDef](./type_defs.md#filtergrouptypedef) 
6. See [:material-code-braces: ColumnConfigurationTypeDef](./type_defs.md#columnconfigurationtypedef) 
7. See [:material-code-braces: AnalysisDefaultsTypeDef](./type_defs.md#analysisdefaultstypedef) 
## TemplateVersionDefinitionTypeDef

```python
# TemplateVersionDefinitionTypeDef definition

class TemplateVersionDefinitionTypeDef(TypedDict):
    DataSetConfigurations: Sequence[DataSetConfigurationTypeDef],  # (1)
    Sheets: NotRequired[Sequence[SheetDefinitionTypeDef]],  # (2)
    CalculatedFields: NotRequired[Sequence[CalculatedFieldTypeDef]],  # (3)
    ParameterDeclarations: NotRequired[Sequence[ParameterDeclarationTypeDef]],  # (4)
    FilterGroups: NotRequired[Sequence[FilterGroupTypeDef]],  # (5)
    ColumnConfigurations: NotRequired[Sequence[ColumnConfigurationTypeDef]],  # (6)
    AnalysisDefaults: NotRequired[AnalysisDefaultsTypeDef],  # (7)
```

1. See [:material-code-braces: DataSetConfigurationTypeDef](./type_defs.md#datasetconfigurationtypedef) 
2. See [:material-code-braces: SheetDefinitionTypeDef](./type_defs.md#sheetdefinitiontypedef) 
3. See [:material-code-braces: CalculatedFieldTypeDef](./type_defs.md#calculatedfieldtypedef) 
4. See [:material-code-braces: ParameterDeclarationTypeDef](./type_defs.md#parameterdeclarationtypedef) 
5. See [:material-code-braces: FilterGroupTypeDef](./type_defs.md#filtergrouptypedef) 
6. See [:material-code-braces: ColumnConfigurationTypeDef](./type_defs.md#columnconfigurationtypedef) 
7. See [:material-code-braces: AnalysisDefaultsTypeDef](./type_defs.md#analysisdefaultstypedef) 
## CreateAnalysisRequestRequestTypeDef

```python
# CreateAnalysisRequestRequestTypeDef definition

class CreateAnalysisRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AnalysisId: str,
    Name: str,
    Parameters: NotRequired[ParametersTypeDef],  # (1)
    Permissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (2)
    SourceEntity: NotRequired[AnalysisSourceEntityTypeDef],  # (3)
    ThemeArn: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    Definition: NotRequired[AnalysisDefinitionTypeDef],  # (5)
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: AnalysisSourceEntityTypeDef](./type_defs.md#analysissourceentitytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: AnalysisDefinitionTypeDef](./type_defs.md#analysisdefinitiontypedef) 
## DescribeAnalysisDefinitionResponseTypeDef

```python
# DescribeAnalysisDefinitionResponseTypeDef definition

class DescribeAnalysisDefinitionResponseTypeDef(TypedDict):
    AnalysisId: str,
    Name: str,
    Errors: List[AnalysisErrorTypeDef],  # (1)
    ResourceStatus: ResourceStatusType,  # (2)
    ThemeArn: str,
    Definition: AnalysisDefinitionTypeDef,  # (3)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AnalysisErrorTypeDef](./type_defs.md#analysiserrortypedef) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
3. See [:material-code-braces: AnalysisDefinitionTypeDef](./type_defs.md#analysisdefinitiontypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAnalysisRequestRequestTypeDef

```python
# UpdateAnalysisRequestRequestTypeDef definition

class UpdateAnalysisRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    AnalysisId: str,
    Name: str,
    Parameters: NotRequired[ParametersTypeDef],  # (1)
    SourceEntity: NotRequired[AnalysisSourceEntityTypeDef],  # (2)
    ThemeArn: NotRequired[str],
    Definition: NotRequired[AnalysisDefinitionTypeDef],  # (3)
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
2. See [:material-code-braces: AnalysisSourceEntityTypeDef](./type_defs.md#analysissourceentitytypedef) 
3. See [:material-code-braces: AnalysisDefinitionTypeDef](./type_defs.md#analysisdefinitiontypedef) 
## CreateDashboardRequestRequestTypeDef

```python
# CreateDashboardRequestRequestTypeDef definition

class CreateDashboardRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    Name: str,
    Parameters: NotRequired[ParametersTypeDef],  # (1)
    Permissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (2)
    SourceEntity: NotRequired[DashboardSourceEntityTypeDef],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    VersionDescription: NotRequired[str],
    DashboardPublishOptions: NotRequired[DashboardPublishOptionsTypeDef],  # (5)
    ThemeArn: NotRequired[str],
    Definition: NotRequired[DashboardVersionDefinitionTypeDef],  # (6)
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: DashboardSourceEntityTypeDef](./type_defs.md#dashboardsourceentitytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: DashboardPublishOptionsTypeDef](./type_defs.md#dashboardpublishoptionstypedef) 
6. See [:material-code-braces: DashboardVersionDefinitionTypeDef](./type_defs.md#dashboardversiondefinitiontypedef) 
## DescribeDashboardDefinitionResponseTypeDef

```python
# DescribeDashboardDefinitionResponseTypeDef definition

class DescribeDashboardDefinitionResponseTypeDef(TypedDict):
    DashboardId: str,
    Errors: List[DashboardErrorTypeDef],  # (1)
    Name: str,
    ResourceStatus: ResourceStatusType,  # (2)
    ThemeArn: str,
    Definition: DashboardVersionDefinitionTypeDef,  # (3)
    Status: int,
    RequestId: str,
    DashboardPublishOptions: DashboardPublishOptionsTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DashboardErrorTypeDef](./type_defs.md#dashboarderrortypedef) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
3. See [:material-code-braces: DashboardVersionDefinitionTypeDef](./type_defs.md#dashboardversiondefinitiontypedef) 
4. See [:material-code-braces: DashboardPublishOptionsTypeDef](./type_defs.md#dashboardpublishoptionstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDashboardRequestRequestTypeDef

```python
# UpdateDashboardRequestRequestTypeDef definition

class UpdateDashboardRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    DashboardId: str,
    Name: str,
    SourceEntity: NotRequired[DashboardSourceEntityTypeDef],  # (1)
    Parameters: NotRequired[ParametersTypeDef],  # (2)
    VersionDescription: NotRequired[str],
    DashboardPublishOptions: NotRequired[DashboardPublishOptionsTypeDef],  # (3)
    ThemeArn: NotRequired[str],
    Definition: NotRequired[DashboardVersionDefinitionTypeDef],  # (4)
```

1. See [:material-code-braces: DashboardSourceEntityTypeDef](./type_defs.md#dashboardsourceentitytypedef) 
2. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
3. See [:material-code-braces: DashboardPublishOptionsTypeDef](./type_defs.md#dashboardpublishoptionstypedef) 
4. See [:material-code-braces: DashboardVersionDefinitionTypeDef](./type_defs.md#dashboardversiondefinitiontypedef) 
## CreateTemplateRequestRequestTypeDef

```python
# CreateTemplateRequestRequestTypeDef definition

class CreateTemplateRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    Name: NotRequired[str],
    Permissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
    SourceEntity: NotRequired[TemplateSourceEntityTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    VersionDescription: NotRequired[str],
    Definition: NotRequired[TemplateVersionDefinitionTypeDef],  # (4)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: TemplateSourceEntityTypeDef](./type_defs.md#templatesourceentitytypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: TemplateVersionDefinitionTypeDef](./type_defs.md#templateversiondefinitiontypedef) 
## DescribeTemplateDefinitionResponseTypeDef

```python
# DescribeTemplateDefinitionResponseTypeDef definition

class DescribeTemplateDefinitionResponseTypeDef(TypedDict):
    Name: str,
    TemplateId: str,
    Errors: List[TemplateErrorTypeDef],  # (1)
    ResourceStatus: ResourceStatusType,  # (2)
    ThemeArn: str,
    Definition: TemplateVersionDefinitionTypeDef,  # (3)
    Status: int,
    RequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TemplateErrorTypeDef](./type_defs.md#templateerrortypedef) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
3. See [:material-code-braces: TemplateVersionDefinitionTypeDef](./type_defs.md#templateversiondefinitiontypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTemplateRequestRequestTypeDef

```python
# UpdateTemplateRequestRequestTypeDef definition

class UpdateTemplateRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    TemplateId: str,
    SourceEntity: NotRequired[TemplateSourceEntityTypeDef],  # (1)
    VersionDescription: NotRequired[str],
    Name: NotRequired[str],
    Definition: NotRequired[TemplateVersionDefinitionTypeDef],  # (2)
```

1. See [:material-code-braces: TemplateSourceEntityTypeDef](./type_defs.md#templatesourceentitytypedef) 
2. See [:material-code-braces: TemplateVersionDefinitionTypeDef](./type_defs.md#templateversiondefinitiontypedef) 
