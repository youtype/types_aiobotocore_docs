# Type definitions

> [Index](../README.md) > [LexModelsV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LexModelsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
    type annotations stubs module [types-aiobotocore-lexv2-models](https://pypi.org/project/types-aiobotocore-lexv2-models/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ActiveContextTypeDef

```python
# ActiveContextTypeDef definition

class ActiveContextTypeDef(TypedDict):
    name: str,
```

## AdvancedRecognitionSettingTypeDef

```python
# AdvancedRecognitionSettingTypeDef definition

class AdvancedRecognitionSettingTypeDef(TypedDict):
    audioRecognitionStrategy: NotRequired[AudioRecognitionStrategyType],  # (1)
```

1. See [:material-code-brackets: AudioRecognitionStrategyType](./literals.md#audiorecognitionstrategytype) 
## ExecutionErrorDetailsTypeDef

```python
# ExecutionErrorDetailsTypeDef definition

class ExecutionErrorDetailsTypeDef(TypedDict):
    errorCode: str,
    errorMessage: str,
```

## AgentTurnSpecificationTypeDef

```python
# AgentTurnSpecificationTypeDef definition

class AgentTurnSpecificationTypeDef(TypedDict):
    agentPrompt: str,
```

## AggregatedUtterancesFilterTypeDef

```python
# AggregatedUtterancesFilterTypeDef definition

class AggregatedUtterancesFilterTypeDef(TypedDict):
    name: AggregatedUtterancesFilterNameType,  # (1)
    values: Sequence[str],
    operator: AggregatedUtterancesFilterOperatorType,  # (2)
```

1. See [:material-code-brackets: AggregatedUtterancesFilterNameType](./literals.md#aggregatedutterancesfilternametype) 
2. See [:material-code-brackets: AggregatedUtterancesFilterOperatorType](./literals.md#aggregatedutterancesfilteroperatortype) 
## AggregatedUtterancesSortByTypeDef

```python
# AggregatedUtterancesSortByTypeDef definition

class AggregatedUtterancesSortByTypeDef(TypedDict):
    attribute: AggregatedUtterancesSortAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: AggregatedUtterancesSortAttributeType](./literals.md#aggregatedutterancessortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## AggregatedUtterancesSummaryTypeDef

```python
# AggregatedUtterancesSummaryTypeDef definition

class AggregatedUtterancesSummaryTypeDef(TypedDict):
    utterance: NotRequired[str],
    hitCount: NotRequired[int],
    missedCount: NotRequired[int],
    utteranceFirstRecordedInAggregationDuration: NotRequired[datetime],
    utteranceLastRecordedInAggregationDuration: NotRequired[datetime],
    containsDataFromDeletedResources: NotRequired[bool],
```

## AllowedInputTypesTypeDef

```python
# AllowedInputTypesTypeDef definition

class AllowedInputTypesTypeDef(TypedDict):
    allowAudioInput: bool,
    allowDTMFInput: bool,
```

## AnalyticsBinBySpecificationTypeDef

```python
# AnalyticsBinBySpecificationTypeDef definition

class AnalyticsBinBySpecificationTypeDef(TypedDict):
    name: AnalyticsBinByNameType,  # (1)
    interval: AnalyticsIntervalType,  # (2)
    order: NotRequired[AnalyticsSortOrderType],  # (3)
```

1. See [:material-code-brackets: AnalyticsBinByNameType](./literals.md#analyticsbinbynametype) 
2. See [:material-code-brackets: AnalyticsIntervalType](./literals.md#analyticsintervaltype) 
3. See [:material-code-brackets: AnalyticsSortOrderType](./literals.md#analyticssortordertype) 
## AnalyticsBinKeyTypeDef

```python
# AnalyticsBinKeyTypeDef definition

class AnalyticsBinKeyTypeDef(TypedDict):
    name: NotRequired[AnalyticsBinByNameType],  # (1)
    value: NotRequired[int],
```

1. See [:material-code-brackets: AnalyticsBinByNameType](./literals.md#analyticsbinbynametype) 
## AnalyticsIntentFilterTypeDef

```python
# AnalyticsIntentFilterTypeDef definition

class AnalyticsIntentFilterTypeDef(TypedDict):
    name: AnalyticsIntentFilterNameType,  # (1)
    operator: AnalyticsFilterOperatorType,  # (2)
    values: Sequence[str],
```

1. See [:material-code-brackets: AnalyticsIntentFilterNameType](./literals.md#analyticsintentfilternametype) 
2. See [:material-code-brackets: AnalyticsFilterOperatorType](./literals.md#analyticsfilteroperatortype) 
## AnalyticsIntentGroupByKeyTypeDef

```python
# AnalyticsIntentGroupByKeyTypeDef definition

class AnalyticsIntentGroupByKeyTypeDef(TypedDict):
    name: NotRequired[AnalyticsIntentFieldType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: AnalyticsIntentFieldType](./literals.md#analyticsintentfieldtype) 
## AnalyticsIntentGroupBySpecificationTypeDef

```python
# AnalyticsIntentGroupBySpecificationTypeDef definition

class AnalyticsIntentGroupBySpecificationTypeDef(TypedDict):
    name: AnalyticsIntentFieldType,  # (1)
```

1. See [:material-code-brackets: AnalyticsIntentFieldType](./literals.md#analyticsintentfieldtype) 
## AnalyticsIntentMetricResultTypeDef

```python
# AnalyticsIntentMetricResultTypeDef definition

class AnalyticsIntentMetricResultTypeDef(TypedDict):
    name: NotRequired[AnalyticsIntentMetricNameType],  # (1)
    statistic: NotRequired[AnalyticsMetricStatisticType],  # (2)
    value: NotRequired[float],
```

1. See [:material-code-brackets: AnalyticsIntentMetricNameType](./literals.md#analyticsintentmetricnametype) 
2. See [:material-code-brackets: AnalyticsMetricStatisticType](./literals.md#analyticsmetricstatistictype) 
## AnalyticsIntentMetricTypeDef

```python
# AnalyticsIntentMetricTypeDef definition

class AnalyticsIntentMetricTypeDef(TypedDict):
    name: AnalyticsIntentMetricNameType,  # (1)
    statistic: AnalyticsMetricStatisticType,  # (2)
    order: NotRequired[AnalyticsSortOrderType],  # (3)
```

1. See [:material-code-brackets: AnalyticsIntentMetricNameType](./literals.md#analyticsintentmetricnametype) 
2. See [:material-code-brackets: AnalyticsMetricStatisticType](./literals.md#analyticsmetricstatistictype) 
3. See [:material-code-brackets: AnalyticsSortOrderType](./literals.md#analyticssortordertype) 
## AnalyticsIntentNodeSummaryTypeDef

```python
# AnalyticsIntentNodeSummaryTypeDef definition

class AnalyticsIntentNodeSummaryTypeDef(TypedDict):
    intentName: NotRequired[str],
    intentPath: NotRequired[str],
    intentCount: NotRequired[int],
    intentLevel: NotRequired[int],
    nodeType: NotRequired[AnalyticsNodeTypeType],  # (1)
```

1. See [:material-code-brackets: AnalyticsNodeTypeType](./literals.md#analyticsnodetypetype) 
## AnalyticsIntentStageFilterTypeDef

```python
# AnalyticsIntentStageFilterTypeDef definition

class AnalyticsIntentStageFilterTypeDef(TypedDict):
    name: AnalyticsIntentStageFilterNameType,  # (1)
    operator: AnalyticsFilterOperatorType,  # (2)
    values: Sequence[str],
```

1. See [:material-code-brackets: AnalyticsIntentStageFilterNameType](./literals.md#analyticsintentstagefilternametype) 
2. See [:material-code-brackets: AnalyticsFilterOperatorType](./literals.md#analyticsfilteroperatortype) 
## AnalyticsIntentStageGroupByKeyTypeDef

```python
# AnalyticsIntentStageGroupByKeyTypeDef definition

class AnalyticsIntentStageGroupByKeyTypeDef(TypedDict):
    name: NotRequired[AnalyticsIntentStageFieldType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: AnalyticsIntentStageFieldType](./literals.md#analyticsintentstagefieldtype) 
## AnalyticsIntentStageGroupBySpecificationTypeDef

```python
# AnalyticsIntentStageGroupBySpecificationTypeDef definition

class AnalyticsIntentStageGroupBySpecificationTypeDef(TypedDict):
    name: AnalyticsIntentStageFieldType,  # (1)
```

1. See [:material-code-brackets: AnalyticsIntentStageFieldType](./literals.md#analyticsintentstagefieldtype) 
## AnalyticsIntentStageMetricResultTypeDef

```python
# AnalyticsIntentStageMetricResultTypeDef definition

class AnalyticsIntentStageMetricResultTypeDef(TypedDict):
    name: NotRequired[AnalyticsIntentStageMetricNameType],  # (1)
    statistic: NotRequired[AnalyticsMetricStatisticType],  # (2)
    value: NotRequired[float],
```

1. See [:material-code-brackets: AnalyticsIntentStageMetricNameType](./literals.md#analyticsintentstagemetricnametype) 
2. See [:material-code-brackets: AnalyticsMetricStatisticType](./literals.md#analyticsmetricstatistictype) 
## AnalyticsIntentStageMetricTypeDef

```python
# AnalyticsIntentStageMetricTypeDef definition

class AnalyticsIntentStageMetricTypeDef(TypedDict):
    name: AnalyticsIntentStageMetricNameType,  # (1)
    statistic: AnalyticsMetricStatisticType,  # (2)
    order: NotRequired[AnalyticsSortOrderType],  # (3)
```

1. See [:material-code-brackets: AnalyticsIntentStageMetricNameType](./literals.md#analyticsintentstagemetricnametype) 
2. See [:material-code-brackets: AnalyticsMetricStatisticType](./literals.md#analyticsmetricstatistictype) 
3. See [:material-code-brackets: AnalyticsSortOrderType](./literals.md#analyticssortordertype) 
## AnalyticsPathFilterTypeDef

```python
# AnalyticsPathFilterTypeDef definition

class AnalyticsPathFilterTypeDef(TypedDict):
    name: AnalyticsCommonFilterNameType,  # (1)
    operator: AnalyticsFilterOperatorType,  # (2)
    values: Sequence[str],
```

1. See [:material-code-brackets: AnalyticsCommonFilterNameType](./literals.md#analyticscommonfilternametype) 
2. See [:material-code-brackets: AnalyticsFilterOperatorType](./literals.md#analyticsfilteroperatortype) 
## AnalyticsSessionFilterTypeDef

```python
# AnalyticsSessionFilterTypeDef definition

class AnalyticsSessionFilterTypeDef(TypedDict):
    name: AnalyticsSessionFilterNameType,  # (1)
    operator: AnalyticsFilterOperatorType,  # (2)
    values: Sequence[str],
```

1. See [:material-code-brackets: AnalyticsSessionFilterNameType](./literals.md#analyticssessionfilternametype) 
2. See [:material-code-brackets: AnalyticsFilterOperatorType](./literals.md#analyticsfilteroperatortype) 
## AnalyticsSessionGroupByKeyTypeDef

```python
# AnalyticsSessionGroupByKeyTypeDef definition

class AnalyticsSessionGroupByKeyTypeDef(TypedDict):
    name: NotRequired[AnalyticsSessionFieldType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: AnalyticsSessionFieldType](./literals.md#analyticssessionfieldtype) 
## AnalyticsSessionGroupBySpecificationTypeDef

```python
# AnalyticsSessionGroupBySpecificationTypeDef definition

class AnalyticsSessionGroupBySpecificationTypeDef(TypedDict):
    name: AnalyticsSessionFieldType,  # (1)
```

1. See [:material-code-brackets: AnalyticsSessionFieldType](./literals.md#analyticssessionfieldtype) 
## AnalyticsSessionMetricResultTypeDef

```python
# AnalyticsSessionMetricResultTypeDef definition

class AnalyticsSessionMetricResultTypeDef(TypedDict):
    name: NotRequired[AnalyticsSessionMetricNameType],  # (1)
    statistic: NotRequired[AnalyticsMetricStatisticType],  # (2)
    value: NotRequired[float],
```

1. See [:material-code-brackets: AnalyticsSessionMetricNameType](./literals.md#analyticssessionmetricnametype) 
2. See [:material-code-brackets: AnalyticsMetricStatisticType](./literals.md#analyticsmetricstatistictype) 
## AnalyticsSessionMetricTypeDef

```python
# AnalyticsSessionMetricTypeDef definition

class AnalyticsSessionMetricTypeDef(TypedDict):
    name: AnalyticsSessionMetricNameType,  # (1)
    statistic: AnalyticsMetricStatisticType,  # (2)
    order: NotRequired[AnalyticsSortOrderType],  # (3)
```

1. See [:material-code-brackets: AnalyticsSessionMetricNameType](./literals.md#analyticssessionmetricnametype) 
2. See [:material-code-brackets: AnalyticsMetricStatisticType](./literals.md#analyticsmetricstatistictype) 
3. See [:material-code-brackets: AnalyticsSortOrderType](./literals.md#analyticssortordertype) 
## AnalyticsUtteranceAttributeResultTypeDef

```python
# AnalyticsUtteranceAttributeResultTypeDef definition

class AnalyticsUtteranceAttributeResultTypeDef(TypedDict):
    lastUsedIntent: NotRequired[str],
```

## AnalyticsUtteranceAttributeTypeDef

```python
# AnalyticsUtteranceAttributeTypeDef definition

class AnalyticsUtteranceAttributeTypeDef(TypedDict):
    name: AnalyticsUtteranceAttributeNameType,  # (1)
```

1. See [:material-code-brackets: AnalyticsUtteranceAttributeNameType](./literals.md#analyticsutteranceattributenametype) 
## AnalyticsUtteranceFilterTypeDef

```python
# AnalyticsUtteranceFilterTypeDef definition

class AnalyticsUtteranceFilterTypeDef(TypedDict):
    name: AnalyticsUtteranceFilterNameType,  # (1)
    operator: AnalyticsFilterOperatorType,  # (2)
    values: Sequence[str],
```

1. See [:material-code-brackets: AnalyticsUtteranceFilterNameType](./literals.md#analyticsutterancefilternametype) 
2. See [:material-code-brackets: AnalyticsFilterOperatorType](./literals.md#analyticsfilteroperatortype) 
## AnalyticsUtteranceGroupByKeyTypeDef

```python
# AnalyticsUtteranceGroupByKeyTypeDef definition

class AnalyticsUtteranceGroupByKeyTypeDef(TypedDict):
    name: NotRequired[AnalyticsUtteranceFieldType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: AnalyticsUtteranceFieldType](./literals.md#analyticsutterancefieldtype) 
## AnalyticsUtteranceGroupBySpecificationTypeDef

```python
# AnalyticsUtteranceGroupBySpecificationTypeDef definition

class AnalyticsUtteranceGroupBySpecificationTypeDef(TypedDict):
    name: AnalyticsUtteranceFieldType,  # (1)
```

1. See [:material-code-brackets: AnalyticsUtteranceFieldType](./literals.md#analyticsutterancefieldtype) 
## AnalyticsUtteranceMetricResultTypeDef

```python
# AnalyticsUtteranceMetricResultTypeDef definition

class AnalyticsUtteranceMetricResultTypeDef(TypedDict):
    name: NotRequired[AnalyticsUtteranceMetricNameType],  # (1)
    statistic: NotRequired[AnalyticsMetricStatisticType],  # (2)
    value: NotRequired[float],
```

1. See [:material-code-brackets: AnalyticsUtteranceMetricNameType](./literals.md#analyticsutterancemetricnametype) 
2. See [:material-code-brackets: AnalyticsMetricStatisticType](./literals.md#analyticsmetricstatistictype) 
## AnalyticsUtteranceMetricTypeDef

```python
# AnalyticsUtteranceMetricTypeDef definition

class AnalyticsUtteranceMetricTypeDef(TypedDict):
    name: AnalyticsUtteranceMetricNameType,  # (1)
    statistic: AnalyticsMetricStatisticType,  # (2)
    order: NotRequired[AnalyticsSortOrderType],  # (3)
```

1. See [:material-code-brackets: AnalyticsUtteranceMetricNameType](./literals.md#analyticsutterancemetricnametype) 
2. See [:material-code-brackets: AnalyticsMetricStatisticType](./literals.md#analyticsmetricstatistictype) 
3. See [:material-code-brackets: AnalyticsSortOrderType](./literals.md#analyticssortordertype) 
## AssociatedTranscriptFilterTypeDef

```python
# AssociatedTranscriptFilterTypeDef definition

class AssociatedTranscriptFilterTypeDef(TypedDict):
    name: AssociatedTranscriptFilterNameType,  # (1)
    values: Sequence[str],
```

1. See [:material-code-brackets: AssociatedTranscriptFilterNameType](./literals.md#associatedtranscriptfilternametype) 
## AssociatedTranscriptTypeDef

```python
# AssociatedTranscriptTypeDef definition

class AssociatedTranscriptTypeDef(TypedDict):
    transcript: NotRequired[str],
```

## AudioSpecificationTypeDef

```python
# AudioSpecificationTypeDef definition

class AudioSpecificationTypeDef(TypedDict):
    maxLengthMs: int,
    endTimeoutMs: int,
```

## DTMFSpecificationTypeDef

```python
# DTMFSpecificationTypeDef definition

class DTMFSpecificationTypeDef(TypedDict):
    maxLength: int,
    endTimeoutMs: int,
    deletionCharacter: str,
    endCharacter: str,
```

## S3BucketLogDestinationTypeDef

```python
# S3BucketLogDestinationTypeDef definition

class S3BucketLogDestinationTypeDef(TypedDict):
    s3BucketArn: str,
    logPrefix: str,
    kmsKeyArn: NotRequired[str],
```

## NewCustomVocabularyItemTypeDef

```python
# NewCustomVocabularyItemTypeDef definition

class NewCustomVocabularyItemTypeDef(TypedDict):
    phrase: str,
    weight: NotRequired[int],
    displayAs: NotRequired[str],
```

## CustomVocabularyItemTypeDef

```python
# CustomVocabularyItemTypeDef definition

class CustomVocabularyItemTypeDef(TypedDict):
    itemId: str,
    phrase: str,
    weight: NotRequired[int],
    displayAs: NotRequired[str],
```

## FailedCustomVocabularyItemTypeDef

```python
# FailedCustomVocabularyItemTypeDef definition

class FailedCustomVocabularyItemTypeDef(TypedDict):
    itemId: NotRequired[str],
    errorMessage: NotRequired[str],
    errorCode: NotRequired[ErrorCodeType],  # (1)
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
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

## CustomVocabularyEntryIdTypeDef

```python
# CustomVocabularyEntryIdTypeDef definition

class CustomVocabularyEntryIdTypeDef(TypedDict):
    itemId: str,
```

## BotAliasHistoryEventTypeDef

```python
# BotAliasHistoryEventTypeDef definition

class BotAliasHistoryEventTypeDef(TypedDict):
    botVersion: NotRequired[str],
    startDate: NotRequired[datetime],
    endDate: NotRequired[datetime],
```

## BotAliasSummaryTypeDef

```python
# BotAliasSummaryTypeDef definition

class BotAliasSummaryTypeDef(TypedDict):
    botAliasId: NotRequired[str],
    botAliasName: NotRequired[str],
    description: NotRequired[str],
    botVersion: NotRequired[str],
    botAliasStatus: NotRequired[BotAliasStatusType],  # (1)
    creationDateTime: NotRequired[datetime],
    lastUpdatedDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: BotAliasStatusType](./literals.md#botaliasstatustype) 
## BotAliasTestExecutionTargetTypeDef

```python
# BotAliasTestExecutionTargetTypeDef definition

class BotAliasTestExecutionTargetTypeDef(TypedDict):
    botId: str,
    botAliasId: str,
    localeId: str,
```

## BotExportSpecificationTypeDef

```python
# BotExportSpecificationTypeDef definition

class BotExportSpecificationTypeDef(TypedDict):
    botId: str,
    botVersion: str,
```

## BotFilterTypeDef

```python
# BotFilterTypeDef definition

class BotFilterTypeDef(TypedDict):
    name: BotFilterNameType,  # (1)
    values: Sequence[str],
    operator: BotFilterOperatorType,  # (2)
```

1. See [:material-code-brackets: BotFilterNameType](./literals.md#botfilternametype) 
2. See [:material-code-brackets: BotFilterOperatorType](./literals.md#botfilteroperatortype) 
## DataPrivacyTypeDef

```python
# DataPrivacyTypeDef definition

class DataPrivacyTypeDef(TypedDict):
    childDirected: bool,
```

## BotLocaleExportSpecificationTypeDef

```python
# BotLocaleExportSpecificationTypeDef definition

class BotLocaleExportSpecificationTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
```

## BotLocaleFilterTypeDef

```python
# BotLocaleFilterTypeDef definition

class BotLocaleFilterTypeDef(TypedDict):
    name: BotLocaleFilterNameType,  # (1)
    values: Sequence[str],
    operator: BotLocaleFilterOperatorType,  # (2)
```

1. See [:material-code-brackets: BotLocaleFilterNameType](./literals.md#botlocalefilternametype) 
2. See [:material-code-brackets: BotLocaleFilterOperatorType](./literals.md#botlocalefilteroperatortype) 
## BotLocaleHistoryEventTypeDef

```python
# BotLocaleHistoryEventTypeDef definition

class BotLocaleHistoryEventTypeDef(TypedDict):
    event: str,
    eventDate: datetime,
```

## VoiceSettingsTypeDef

```python
# VoiceSettingsTypeDef definition

class VoiceSettingsTypeDef(TypedDict):
    voiceId: str,
    engine: NotRequired[VoiceEngineType],  # (1)
```

1. See [:material-code-brackets: VoiceEngineType](./literals.md#voiceenginetype) 
## BotLocaleSortByTypeDef

```python
# BotLocaleSortByTypeDef definition

class BotLocaleSortByTypeDef(TypedDict):
    attribute: BotLocaleSortAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: BotLocaleSortAttributeType](./literals.md#botlocalesortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## BotLocaleSummaryTypeDef

```python
# BotLocaleSummaryTypeDef definition

class BotLocaleSummaryTypeDef(TypedDict):
    localeId: NotRequired[str],
    localeName: NotRequired[str],
    description: NotRequired[str],
    botLocaleStatus: NotRequired[BotLocaleStatusType],  # (1)
    lastUpdatedDateTime: NotRequired[datetime],
    lastBuildSubmittedDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: BotLocaleStatusType](./literals.md#botlocalestatustype) 
## BotMemberTypeDef

```python
# BotMemberTypeDef definition

class BotMemberTypeDef(TypedDict):
    botMemberId: str,
    botMemberName: str,
    botMemberAliasId: str,
    botMemberAliasName: str,
    botMemberVersion: str,
```

## IntentStatisticsTypeDef

```python
# IntentStatisticsTypeDef definition

class IntentStatisticsTypeDef(TypedDict):
    discoveredIntentCount: NotRequired[int],
```

## SlotTypeStatisticsTypeDef

```python
# SlotTypeStatisticsTypeDef definition

class SlotTypeStatisticsTypeDef(TypedDict):
    discoveredSlotTypeCount: NotRequired[int],
```

## BotRecommendationSummaryTypeDef

```python
# BotRecommendationSummaryTypeDef definition

class BotRecommendationSummaryTypeDef(TypedDict):
    botRecommendationStatus: BotRecommendationStatusType,  # (1)
    botRecommendationId: str,
    creationDateTime: NotRequired[datetime],
    lastUpdatedDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: BotRecommendationStatusType](./literals.md#botrecommendationstatustype) 
## BotSortByTypeDef

```python
# BotSortByTypeDef definition

class BotSortByTypeDef(TypedDict):
    attribute: BotSortAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: BotSortAttributeType](./literals.md#botsortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## BotSummaryTypeDef

```python
# BotSummaryTypeDef definition

class BotSummaryTypeDef(TypedDict):
    botId: NotRequired[str],
    botName: NotRequired[str],
    description: NotRequired[str],
    botStatus: NotRequired[BotStatusType],  # (1)
    latestBotVersion: NotRequired[str],
    lastUpdatedDateTime: NotRequired[datetime],
    botType: NotRequired[BotTypeType],  # (2)
```

1. See [:material-code-brackets: BotStatusType](./literals.md#botstatustype) 
2. See [:material-code-brackets: BotTypeType](./literals.md#bottypetype) 
## BotVersionLocaleDetailsTypeDef

```python
# BotVersionLocaleDetailsTypeDef definition

class BotVersionLocaleDetailsTypeDef(TypedDict):
    sourceBotVersion: str,
```

## BotVersionSortByTypeDef

```python
# BotVersionSortByTypeDef definition

class BotVersionSortByTypeDef(TypedDict):
    attribute: BotVersionSortAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: BotVersionSortAttributeType](./literals.md#botversionsortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## BotVersionSummaryTypeDef

```python
# BotVersionSummaryTypeDef definition

class BotVersionSummaryTypeDef(TypedDict):
    botName: NotRequired[str],
    botVersion: NotRequired[str],
    description: NotRequired[str],
    botStatus: NotRequired[BotStatusType],  # (1)
    creationDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: BotStatusType](./literals.md#botstatustype) 
## BuildBotLocaleRequestRequestTypeDef

```python
# BuildBotLocaleRequestRequestTypeDef definition

class BuildBotLocaleRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
```

## BuiltInIntentSortByTypeDef

```python
# BuiltInIntentSortByTypeDef definition

class BuiltInIntentSortByTypeDef(TypedDict):
    attribute: BuiltInIntentSortAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: BuiltInIntentSortAttributeType](./literals.md#builtinintentsortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## BuiltInIntentSummaryTypeDef

```python
# BuiltInIntentSummaryTypeDef definition

class BuiltInIntentSummaryTypeDef(TypedDict):
    intentSignature: NotRequired[str],
    description: NotRequired[str],
```

## BuiltInSlotTypeSortByTypeDef

```python
# BuiltInSlotTypeSortByTypeDef definition

class BuiltInSlotTypeSortByTypeDef(TypedDict):
    attribute: BuiltInSlotTypeSortAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: BuiltInSlotTypeSortAttributeType](./literals.md#builtinslottypesortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## BuiltInSlotTypeSummaryTypeDef

```python
# BuiltInSlotTypeSummaryTypeDef definition

class BuiltInSlotTypeSummaryTypeDef(TypedDict):
    slotTypeSignature: NotRequired[str],
    description: NotRequired[str],
```

## ButtonTypeDef

```python
# ButtonTypeDef definition

class ButtonTypeDef(TypedDict):
    text: str,
    value: str,
```

## CloudWatchLogGroupLogDestinationTypeDef

```python
# CloudWatchLogGroupLogDestinationTypeDef definition

class CloudWatchLogGroupLogDestinationTypeDef(TypedDict):
    cloudWatchLogGroupArn: str,
    logPrefix: str,
```

## LambdaCodeHookTypeDef

```python
# LambdaCodeHookTypeDef definition

class LambdaCodeHookTypeDef(TypedDict):
    lambdaARN: str,
    codeHookInterfaceVersion: str,
```

## SubSlotTypeCompositionTypeDef

```python
# SubSlotTypeCompositionTypeDef definition

class SubSlotTypeCompositionTypeDef(TypedDict):
    name: str,
    slotTypeId: str,
```

## ConditionTypeDef

```python
# ConditionTypeDef definition

class ConditionTypeDef(TypedDict):
    expressionString: str,
```

## ConversationLevelIntentClassificationResultItemTypeDef

```python
# ConversationLevelIntentClassificationResultItemTypeDef definition

class ConversationLevelIntentClassificationResultItemTypeDef(TypedDict):
    intentName: str,
    matchResult: TestResultMatchStatusType,  # (1)
```

1. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
## ConversationLevelResultDetailTypeDef

```python
# ConversationLevelResultDetailTypeDef definition

class ConversationLevelResultDetailTypeDef(TypedDict):
    endToEndResult: TestResultMatchStatusType,  # (1)
    speechTranscriptionResult: NotRequired[TestResultMatchStatusType],  # (1)
```

1. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
2. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
## ConversationLevelSlotResolutionResultItemTypeDef

```python
# ConversationLevelSlotResolutionResultItemTypeDef definition

class ConversationLevelSlotResolutionResultItemTypeDef(TypedDict):
    intentName: str,
    slotName: str,
    matchResult: TestResultMatchStatusType,  # (1)
```

1. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
## ConversationLevelTestResultsFilterByTypeDef

```python
# ConversationLevelTestResultsFilterByTypeDef definition

class ConversationLevelTestResultsFilterByTypeDef(TypedDict):
    endToEndResult: NotRequired[TestResultMatchStatusType],  # (1)
```

1. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
## ConversationLogsDataSourceFilterByTypeDef

```python
# ConversationLogsDataSourceFilterByTypeDef definition

class ConversationLogsDataSourceFilterByTypeDef(TypedDict):
    startTime: datetime,
    endTime: datetime,
    inputMode: ConversationLogsInputModeFilterType,  # (1)
```

1. See [:material-code-brackets: ConversationLogsInputModeFilterType](./literals.md#conversationlogsinputmodefiltertype) 
## SentimentAnalysisSettingsTypeDef

```python
# SentimentAnalysisSettingsTypeDef definition

class SentimentAnalysisSettingsTypeDef(TypedDict):
    detectSentiment: bool,
```

## DialogCodeHookSettingsTypeDef

```python
# DialogCodeHookSettingsTypeDef definition

class DialogCodeHookSettingsTypeDef(TypedDict):
    enabled: bool,
```

## InputContextTypeDef

```python
# InputContextTypeDef definition

class InputContextTypeDef(TypedDict):
    name: str,
```

## KendraConfigurationTypeDef

```python
# KendraConfigurationTypeDef definition

class KendraConfigurationTypeDef(TypedDict):
    kendraIndex: str,
    queryFilterStringEnabled: NotRequired[bool],
    queryFilterString: NotRequired[str],
```

## OutputContextTypeDef

```python
# OutputContextTypeDef definition

class OutputContextTypeDef(TypedDict):
    name: str,
    timeToLiveInSeconds: int,
    turnsToLive: int,
```

## SampleUtteranceTypeDef

```python
# SampleUtteranceTypeDef definition

class SampleUtteranceTypeDef(TypedDict):
    utterance: str,
```

## CreateResourcePolicyRequestRequestTypeDef

```python
# CreateResourcePolicyRequestRequestTypeDef definition

class CreateResourcePolicyRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    policy: str,
```

## PrincipalTypeDef

```python
# PrincipalTypeDef definition

class PrincipalTypeDef(TypedDict):
    service: NotRequired[str],
    arn: NotRequired[str],
```

## MultipleValuesSettingTypeDef

```python
# MultipleValuesSettingTypeDef definition

class MultipleValuesSettingTypeDef(TypedDict):
    allowMultipleValues: NotRequired[bool],
```

## ObfuscationSettingTypeDef

```python
# ObfuscationSettingTypeDef definition

class ObfuscationSettingTypeDef(TypedDict):
    obfuscationSettingType: ObfuscationSettingTypeType,  # (1)
```

1. See [:material-code-brackets: ObfuscationSettingTypeType](./literals.md#obfuscationsettingtypetype) 
## CustomPayloadTypeDef

```python
# CustomPayloadTypeDef definition

class CustomPayloadTypeDef(TypedDict):
    value: str,
```

## CustomVocabularyExportSpecificationTypeDef

```python
# CustomVocabularyExportSpecificationTypeDef definition

class CustomVocabularyExportSpecificationTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
```

## CustomVocabularyImportSpecificationTypeDef

```python
# CustomVocabularyImportSpecificationTypeDef definition

class CustomVocabularyImportSpecificationTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
```

## DateRangeFilterTypeDef

```python
# DateRangeFilterTypeDef definition

class DateRangeFilterTypeDef(TypedDict):
    startDateTime: datetime,
    endDateTime: datetime,
```

## DeleteBotAliasRequestRequestTypeDef

```python
# DeleteBotAliasRequestRequestTypeDef definition

class DeleteBotAliasRequestRequestTypeDef(TypedDict):
    botAliasId: str,
    botId: str,
    skipResourceInUseCheck: NotRequired[bool],
```

## DeleteBotLocaleRequestRequestTypeDef

```python
# DeleteBotLocaleRequestRequestTypeDef definition

class DeleteBotLocaleRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
```

## DeleteBotRequestRequestTypeDef

```python
# DeleteBotRequestRequestTypeDef definition

class DeleteBotRequestRequestTypeDef(TypedDict):
    botId: str,
    skipResourceInUseCheck: NotRequired[bool],
```

## DeleteBotVersionRequestRequestTypeDef

```python
# DeleteBotVersionRequestRequestTypeDef definition

class DeleteBotVersionRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    skipResourceInUseCheck: NotRequired[bool],
```

## DeleteCustomVocabularyRequestRequestTypeDef

```python
# DeleteCustomVocabularyRequestRequestTypeDef definition

class DeleteCustomVocabularyRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
```

## DeleteExportRequestRequestTypeDef

```python
# DeleteExportRequestRequestTypeDef definition

class DeleteExportRequestRequestTypeDef(TypedDict):
    exportId: str,
```

## DeleteImportRequestRequestTypeDef

```python
# DeleteImportRequestRequestTypeDef definition

class DeleteImportRequestRequestTypeDef(TypedDict):
    importId: str,
```

## DeleteIntentRequestRequestTypeDef

```python
# DeleteIntentRequestRequestTypeDef definition

class DeleteIntentRequestRequestTypeDef(TypedDict):
    intentId: str,
    botId: str,
    botVersion: str,
    localeId: str,
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    expectedRevisionId: NotRequired[str],
```

## DeleteResourcePolicyStatementRequestRequestTypeDef

```python
# DeleteResourcePolicyStatementRequestRequestTypeDef definition

class DeleteResourcePolicyStatementRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    statementId: str,
    expectedRevisionId: NotRequired[str],
```

## DeleteSlotRequestRequestTypeDef

```python
# DeleteSlotRequestRequestTypeDef definition

class DeleteSlotRequestRequestTypeDef(TypedDict):
    slotId: str,
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
```

## DeleteSlotTypeRequestRequestTypeDef

```python
# DeleteSlotTypeRequestRequestTypeDef definition

class DeleteSlotTypeRequestRequestTypeDef(TypedDict):
    slotTypeId: str,
    botId: str,
    botVersion: str,
    localeId: str,
    skipResourceInUseCheck: NotRequired[bool],
```

## DeleteTestSetRequestRequestTypeDef

```python
# DeleteTestSetRequestRequestTypeDef definition

class DeleteTestSetRequestRequestTypeDef(TypedDict):
    testSetId: str,
```

## DeleteUtterancesRequestRequestTypeDef

```python
# DeleteUtterancesRequestRequestTypeDef definition

class DeleteUtterancesRequestRequestTypeDef(TypedDict):
    botId: str,
    localeId: NotRequired[str],
    sessionId: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeBotAliasRequestRequestTypeDef

```python
# DescribeBotAliasRequestRequestTypeDef definition

class DescribeBotAliasRequestRequestTypeDef(TypedDict):
    botAliasId: str,
    botId: str,
```

## ParentBotNetworkTypeDef

```python
# ParentBotNetworkTypeDef definition

class ParentBotNetworkTypeDef(TypedDict):
    botId: str,
    botVersion: str,
```

## DescribeBotLocaleRequestRequestTypeDef

```python
# DescribeBotLocaleRequestRequestTypeDef definition

class DescribeBotLocaleRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
```

## DescribeBotRecommendationRequestRequestTypeDef

```python
# DescribeBotRecommendationRequestRequestTypeDef definition

class DescribeBotRecommendationRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationId: str,
```

## EncryptionSettingTypeDef

```python
# EncryptionSettingTypeDef definition

class EncryptionSettingTypeDef(TypedDict):
    kmsKeyArn: NotRequired[str],
    botLocaleExportPassword: NotRequired[str],
    associatedTranscriptsPassword: NotRequired[str],
```

## DescribeBotRequestRequestTypeDef

```python
# DescribeBotRequestRequestTypeDef definition

class DescribeBotRequestRequestTypeDef(TypedDict):
    botId: str,
```

## DescribeBotVersionRequestRequestTypeDef

```python
# DescribeBotVersionRequestRequestTypeDef definition

class DescribeBotVersionRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
```

## DescribeCustomVocabularyMetadataRequestRequestTypeDef

```python
# DescribeCustomVocabularyMetadataRequestRequestTypeDef definition

class DescribeCustomVocabularyMetadataRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
```

## DescribeExportRequestRequestTypeDef

```python
# DescribeExportRequestRequestTypeDef definition

class DescribeExportRequestRequestTypeDef(TypedDict):
    exportId: str,
```

## DescribeImportRequestRequestTypeDef

```python
# DescribeImportRequestRequestTypeDef definition

class DescribeImportRequestRequestTypeDef(TypedDict):
    importId: str,
```

## DescribeIntentRequestRequestTypeDef

```python
# DescribeIntentRequestRequestTypeDef definition

class DescribeIntentRequestRequestTypeDef(TypedDict):
    intentId: str,
    botId: str,
    botVersion: str,
    localeId: str,
```

## SlotPriorityTypeDef

```python
# SlotPriorityTypeDef definition

class SlotPriorityTypeDef(TypedDict):
    priority: int,
    slotId: str,
```

## DescribeResourcePolicyRequestRequestTypeDef

```python
# DescribeResourcePolicyRequestRequestTypeDef definition

class DescribeResourcePolicyRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## DescribeSlotRequestRequestTypeDef

```python
# DescribeSlotRequestRequestTypeDef definition

class DescribeSlotRequestRequestTypeDef(TypedDict):
    slotId: str,
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
```

## DescribeSlotTypeRequestRequestTypeDef

```python
# DescribeSlotTypeRequestRequestTypeDef definition

class DescribeSlotTypeRequestRequestTypeDef(TypedDict):
    slotTypeId: str,
    botId: str,
    botVersion: str,
    localeId: str,
```

## DescribeTestExecutionRequestRequestTypeDef

```python
# DescribeTestExecutionRequestRequestTypeDef definition

class DescribeTestExecutionRequestRequestTypeDef(TypedDict):
    testExecutionId: str,
```

## DescribeTestSetDiscrepancyReportRequestRequestTypeDef

```python
# DescribeTestSetDiscrepancyReportRequestRequestTypeDef definition

class DescribeTestSetDiscrepancyReportRequestRequestTypeDef(TypedDict):
    testSetDiscrepancyReportId: str,
```

## DescribeTestSetGenerationRequestRequestTypeDef

```python
# DescribeTestSetGenerationRequestRequestTypeDef definition

class DescribeTestSetGenerationRequestRequestTypeDef(TypedDict):
    testSetGenerationId: str,
```

## TestSetStorageLocationTypeDef

```python
# TestSetStorageLocationTypeDef definition

class TestSetStorageLocationTypeDef(TypedDict):
    s3BucketName: str,
    s3Path: str,
    kmsKeyArn: NotRequired[str],
```

## DescribeTestSetRequestRequestTypeDef

```python
# DescribeTestSetRequestRequestTypeDef definition

class DescribeTestSetRequestRequestTypeDef(TypedDict):
    testSetId: str,
```

## DialogActionTypeDef

```python
# DialogActionTypeDef definition

class DialogActionTypeDef(TypedDict):
    type: DialogActionTypeType,  # (1)
    slotToElicit: NotRequired[str],
    suppressNextMessage: NotRequired[bool],
```

1. See [:material-code-brackets: DialogActionTypeType](./literals.md#dialogactiontypetype) 
## IntentOverrideTypeDef

```python
# IntentOverrideTypeDef definition

class IntentOverrideTypeDef(TypedDict):
    name: NotRequired[str],
    slots: NotRequired[Mapping[str, SlotValueOverrideTypeDef]],  # (1)
```

1. See [:material-code-braces: SlotValueOverrideTypeDef](./type_defs.md#slotvalueoverridetypedef) 
## ElicitationCodeHookInvocationSettingTypeDef

```python
# ElicitationCodeHookInvocationSettingTypeDef definition

class ElicitationCodeHookInvocationSettingTypeDef(TypedDict):
    enableCodeHookInvocation: bool,
    invocationLabel: NotRequired[str],
```

## ExportFilterTypeDef

```python
# ExportFilterTypeDef definition

class ExportFilterTypeDef(TypedDict):
    name: ExportFilterNameType,  # (1)
    values: Sequence[str],
    operator: ExportFilterOperatorType,  # (2)
```

1. See [:material-code-brackets: ExportFilterNameType](./literals.md#exportfilternametype) 
2. See [:material-code-brackets: ExportFilterOperatorType](./literals.md#exportfilteroperatortype) 
## TestSetExportSpecificationTypeDef

```python
# TestSetExportSpecificationTypeDef definition

class TestSetExportSpecificationTypeDef(TypedDict):
    testSetId: str,
```

## ExportSortByTypeDef

```python
# ExportSortByTypeDef definition

class ExportSortByTypeDef(TypedDict):
    attribute: ExportSortAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: ExportSortAttributeType](./literals.md#exportsortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## GetTestExecutionArtifactsUrlRequestRequestTypeDef

```python
# GetTestExecutionArtifactsUrlRequestRequestTypeDef definition

class GetTestExecutionArtifactsUrlRequestRequestTypeDef(TypedDict):
    testExecutionId: str,
```

## GrammarSlotTypeSourceTypeDef

```python
# GrammarSlotTypeSourceTypeDef definition

class GrammarSlotTypeSourceTypeDef(TypedDict):
    s3BucketName: str,
    s3ObjectKey: str,
    kmsKeyArn: NotRequired[str],
```

## ImportFilterTypeDef

```python
# ImportFilterTypeDef definition

class ImportFilterTypeDef(TypedDict):
    name: ImportFilterNameType,  # (1)
    values: Sequence[str],
    operator: ImportFilterOperatorType,  # (2)
```

1. See [:material-code-brackets: ImportFilterNameType](./literals.md#importfilternametype) 
2. See [:material-code-brackets: ImportFilterOperatorType](./literals.md#importfilteroperatortype) 
## ImportSortByTypeDef

```python
# ImportSortByTypeDef definition

class ImportSortByTypeDef(TypedDict):
    attribute: ImportSortAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: ImportSortAttributeType](./literals.md#importsortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ImportSummaryTypeDef

```python
# ImportSummaryTypeDef definition

class ImportSummaryTypeDef(TypedDict):
    importId: NotRequired[str],
    importedResourceId: NotRequired[str],
    importedResourceName: NotRequired[str],
    importStatus: NotRequired[ImportStatusType],  # (1)
    mergeStrategy: NotRequired[MergeStrategyType],  # (2)
    creationDateTime: NotRequired[datetime],
    lastUpdatedDateTime: NotRequired[datetime],
    importedResourceType: NotRequired[ImportResourceTypeType],  # (3)
```

1. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
2. See [:material-code-brackets: MergeStrategyType](./literals.md#mergestrategytype) 
3. See [:material-code-brackets: ImportResourceTypeType](./literals.md#importresourcetypetype) 
## RuntimeHintsTypeDef

```python
# RuntimeHintsTypeDef definition

class RuntimeHintsTypeDef(TypedDict):
    slotHints: NotRequired[Dict[str, Dict[str, RuntimeHintDetailsTypeDef]]],  # (1)
```

1. See [:material-code-braces: RuntimeHintDetailsTypeDef](./type_defs.md#runtimehintdetailstypedef) 
## IntentClassificationTestResultItemCountsTypeDef

```python
# IntentClassificationTestResultItemCountsTypeDef definition

class IntentClassificationTestResultItemCountsTypeDef(TypedDict):
    totalResultCount: int,
    intentMatchResultCounts: Dict[TestResultMatchStatusType, int],  # (1)
    speechTranscriptionResultCounts: NotRequired[Dict[TestResultMatchStatusType, int]],  # (1)
```

1. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
2. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
## IntentFilterTypeDef

```python
# IntentFilterTypeDef definition

class IntentFilterTypeDef(TypedDict):
    name: IntentFilterNameType,  # (1)
    values: Sequence[str],
    operator: IntentFilterOperatorType,  # (2)
```

1. See [:material-code-brackets: IntentFilterNameType](./literals.md#intentfilternametype) 
2. See [:material-code-brackets: IntentFilterOperatorType](./literals.md#intentfilteroperatortype) 
## IntentSortByTypeDef

```python
# IntentSortByTypeDef definition

class IntentSortByTypeDef(TypedDict):
    attribute: IntentSortAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: IntentSortAttributeType](./literals.md#intentsortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## InvokedIntentSampleTypeDef

```python
# InvokedIntentSampleTypeDef definition

class InvokedIntentSampleTypeDef(TypedDict):
    intentName: NotRequired[str],
```

## ListBotAliasesRequestRequestTypeDef

```python
# ListBotAliasesRequestRequestTypeDef definition

class ListBotAliasesRequestRequestTypeDef(TypedDict):
    botId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListBotRecommendationsRequestRequestTypeDef

```python
# ListBotRecommendationsRequestRequestTypeDef definition

class ListBotRecommendationsRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListCustomVocabularyItemsRequestRequestTypeDef

```python
# ListCustomVocabularyItemsRequestRequestTypeDef definition

class ListCustomVocabularyItemsRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListRecommendedIntentsRequestRequestTypeDef

```python
# ListRecommendedIntentsRequestRequestTypeDef definition

class ListRecommendedIntentsRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## RecommendedIntentSummaryTypeDef

```python
# RecommendedIntentSummaryTypeDef definition

class RecommendedIntentSummaryTypeDef(TypedDict):
    intentId: NotRequired[str],
    intentName: NotRequired[str],
    sampleUtterancesCount: NotRequired[int],
```

## SessionDataSortByTypeDef

```python
# SessionDataSortByTypeDef definition

class SessionDataSortByTypeDef(TypedDict):
    name: AnalyticsSessionSortByNameType,  # (1)
    order: AnalyticsSortOrderType,  # (2)
```

1. See [:material-code-brackets: AnalyticsSessionSortByNameType](./literals.md#analyticssessionsortbynametype) 
2. See [:material-code-brackets: AnalyticsSortOrderType](./literals.md#analyticssortordertype) 
## SlotTypeFilterTypeDef

```python
# SlotTypeFilterTypeDef definition

class SlotTypeFilterTypeDef(TypedDict):
    name: SlotTypeFilterNameType,  # (1)
    values: Sequence[str],
    operator: SlotTypeFilterOperatorType,  # (2)
```

1. See [:material-code-brackets: SlotTypeFilterNameType](./literals.md#slottypefilternametype) 
2. See [:material-code-brackets: SlotTypeFilterOperatorType](./literals.md#slottypefilteroperatortype) 
## SlotTypeSortByTypeDef

```python
# SlotTypeSortByTypeDef definition

class SlotTypeSortByTypeDef(TypedDict):
    attribute: SlotTypeSortAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: SlotTypeSortAttributeType](./literals.md#slottypesortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## SlotTypeSummaryTypeDef

```python
# SlotTypeSummaryTypeDef definition

class SlotTypeSummaryTypeDef(TypedDict):
    slotTypeId: NotRequired[str],
    slotTypeName: NotRequired[str],
    description: NotRequired[str],
    parentSlotTypeSignature: NotRequired[str],
    lastUpdatedDateTime: NotRequired[datetime],
    slotTypeCategory: NotRequired[SlotTypeCategoryType],  # (1)
```

1. See [:material-code-brackets: SlotTypeCategoryType](./literals.md#slottypecategorytype) 
## SlotFilterTypeDef

```python
# SlotFilterTypeDef definition

class SlotFilterTypeDef(TypedDict):
    name: SlotFilterNameType,  # (1)
    values: Sequence[str],
    operator: SlotFilterOperatorType,  # (2)
```

1. See [:material-code-brackets: SlotFilterNameType](./literals.md#slotfilternametype) 
2. See [:material-code-brackets: SlotFilterOperatorType](./literals.md#slotfilteroperatortype) 
## SlotSortByTypeDef

```python
# SlotSortByTypeDef definition

class SlotSortByTypeDef(TypedDict):
    attribute: SlotSortAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: SlotSortAttributeType](./literals.md#slotsortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
```

## TestExecutionSortByTypeDef

```python
# TestExecutionSortByTypeDef definition

class TestExecutionSortByTypeDef(TypedDict):
    attribute: TestExecutionSortAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: TestExecutionSortAttributeType](./literals.md#testexecutionsortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListTestSetRecordsRequestRequestTypeDef

```python
# ListTestSetRecordsRequestRequestTypeDef definition

class ListTestSetRecordsRequestRequestTypeDef(TypedDict):
    testSetId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## TestSetSortByTypeDef

```python
# TestSetSortByTypeDef definition

class TestSetSortByTypeDef(TypedDict):
    attribute: TestSetSortAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: TestSetSortAttributeType](./literals.md#testsetsortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## UtteranceDataSortByTypeDef

```python
# UtteranceDataSortByTypeDef definition

class UtteranceDataSortByTypeDef(TypedDict):
    name: AnalyticsUtteranceSortByNameType,  # (1)
    order: AnalyticsSortOrderType,  # (2)
```

1. See [:material-code-brackets: AnalyticsUtteranceSortByNameType](./literals.md#analyticsutterancesortbynametype) 
2. See [:material-code-brackets: AnalyticsSortOrderType](./literals.md#analyticssortordertype) 
## PlainTextMessageTypeDef

```python
# PlainTextMessageTypeDef definition

class PlainTextMessageTypeDef(TypedDict):
    value: str,
```

## SSMLMessageTypeDef

```python
# SSMLMessageTypeDef definition

class SSMLMessageTypeDef(TypedDict):
    value: str,
```

## OverallTestResultItemTypeDef

```python
# OverallTestResultItemTypeDef definition

class OverallTestResultItemTypeDef(TypedDict):
    multiTurnConversation: bool,
    totalResultCount: int,
    endToEndResultCounts: Dict[TestResultMatchStatusType, int],  # (1)
    speechTranscriptionResultCounts: NotRequired[Dict[TestResultMatchStatusType, int]],  # (1)
```

1. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
2. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
## PathFormatTypeDef

```python
# PathFormatTypeDef definition

class PathFormatTypeDef(TypedDict):
    objectPrefixes: NotRequired[List[str]],
```

## TextInputSpecificationTypeDef

```python
# TextInputSpecificationTypeDef definition

class TextInputSpecificationTypeDef(TypedDict):
    startTimeoutMs: int,
```

## RelativeAggregationDurationTypeDef

```python
# RelativeAggregationDurationTypeDef definition

class RelativeAggregationDurationTypeDef(TypedDict):
    timeDimension: TimeDimensionType,  # (1)
    timeValue: int,
```

1. See [:material-code-brackets: TimeDimensionType](./literals.md#timedimensiontype) 
## RuntimeHintValueTypeDef

```python
# RuntimeHintValueTypeDef definition

class RuntimeHintValueTypeDef(TypedDict):
    phrase: str,
```

## SampleValueTypeDef

```python
# SampleValueTypeDef definition

class SampleValueTypeDef(TypedDict):
    value: str,
```

## SlotDefaultValueTypeDef

```python
# SlotDefaultValueTypeDef definition

class SlotDefaultValueTypeDef(TypedDict):
    defaultValue: str,
```

## SlotResolutionTestResultItemCountsTypeDef

```python
# SlotResolutionTestResultItemCountsTypeDef definition

class SlotResolutionTestResultItemCountsTypeDef(TypedDict):
    totalResultCount: int,
    slotMatchResultCounts: Dict[TestResultMatchStatusType, int],  # (1)
    speechTranscriptionResultCounts: NotRequired[Dict[TestResultMatchStatusType, int]],  # (1)
```

1. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
2. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
## SlotValueTypeDef

```python
# SlotValueTypeDef definition

class SlotValueTypeDef(TypedDict):
    interpretedValue: NotRequired[str],
```

## SlotValueRegexFilterTypeDef

```python
# SlotValueRegexFilterTypeDef definition

class SlotValueRegexFilterTypeDef(TypedDict):
    pattern: str,
```

## StopBotRecommendationRequestRequestTypeDef

```python
# StopBotRecommendationRequestRequestTypeDef definition

class StopBotRecommendationRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationId: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    tags: Mapping[str, str],
```

## TestSetIntentDiscrepancyItemTypeDef

```python
# TestSetIntentDiscrepancyItemTypeDef definition

class TestSetIntentDiscrepancyItemTypeDef(TypedDict):
    intentName: str,
    errorMessage: str,
```

## TestSetSlotDiscrepancyItemTypeDef

```python
# TestSetSlotDiscrepancyItemTypeDef definition

class TestSetSlotDiscrepancyItemTypeDef(TypedDict):
    intentName: str,
    slotName: str,
    errorMessage: str,
```

## TestSetDiscrepancyReportBotAliasTargetTypeDef

```python
# TestSetDiscrepancyReportBotAliasTargetTypeDef definition

class TestSetDiscrepancyReportBotAliasTargetTypeDef(TypedDict):
    botId: str,
    botAliasId: str,
    localeId: str,
```

## TestSetImportInputLocationTypeDef

```python
# TestSetImportInputLocationTypeDef definition

class TestSetImportInputLocationTypeDef(TypedDict):
    s3BucketName: str,
    s3Path: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    tagKeys: Sequence[str],
```

## UpdateExportRequestRequestTypeDef

```python
# UpdateExportRequestRequestTypeDef definition

class UpdateExportRequestRequestTypeDef(TypedDict):
    exportId: str,
    filePassword: NotRequired[str],
```

## UpdateResourcePolicyRequestRequestTypeDef

```python
# UpdateResourcePolicyRequestRequestTypeDef definition

class UpdateResourcePolicyRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    policy: str,
    expectedRevisionId: NotRequired[str],
```

## UpdateTestSetRequestRequestTypeDef

```python
# UpdateTestSetRequestRequestTypeDef definition

class UpdateTestSetRequestRequestTypeDef(TypedDict):
    testSetId: str,
    testSetName: str,
    description: NotRequired[str],
```

## UserTurnIntentOutputTypeDef

```python
# UserTurnIntentOutputTypeDef definition

class UserTurnIntentOutputTypeDef(TypedDict):
    name: str,
    slots: NotRequired[Dict[str, UserTurnSlotOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: UserTurnSlotOutputTypeDef](./type_defs.md#userturnslotoutputtypedef) 
## UserTurnSlotOutputTypeDef

```python
# UserTurnSlotOutputTypeDef definition

class UserTurnSlotOutputTypeDef(TypedDict):
    value: NotRequired[str],
    values: NotRequired[List[UserTurnSlotOutputTypeDef]],  # (1)
    subSlots: NotRequired[Dict[str, UserTurnSlotOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: UserTurnSlotOutputTypeDef](./type_defs.md#userturnslotoutputtypedef) 
2. See [:material-code-braces: UserTurnSlotOutputTypeDef](./type_defs.md#userturnslotoutputtypedef) 
## UtteranceAudioInputSpecificationTypeDef

```python
# UtteranceAudioInputSpecificationTypeDef definition

class UtteranceAudioInputSpecificationTypeDef(TypedDict):
    audioFileS3Location: str,
```

## AgentTurnResultTypeDef

```python
# AgentTurnResultTypeDef definition

class AgentTurnResultTypeDef(TypedDict):
    expectedAgentPrompt: str,
    actualAgentPrompt: NotRequired[str],
    errorDetails: NotRequired[ExecutionErrorDetailsTypeDef],  # (1)
    actualElicitedSlot: NotRequired[str],
    actualIntent: NotRequired[str],
```

1. See [:material-code-braces: ExecutionErrorDetailsTypeDef](./type_defs.md#executionerrordetailstypedef) 
## AnalyticsIntentResultTypeDef

```python
# AnalyticsIntentResultTypeDef definition

class AnalyticsIntentResultTypeDef(TypedDict):
    binKeys: NotRequired[List[AnalyticsBinKeyTypeDef]],  # (1)
    groupByKeys: NotRequired[List[AnalyticsIntentGroupByKeyTypeDef]],  # (2)
    metricsResults: NotRequired[List[AnalyticsIntentMetricResultTypeDef]],  # (3)
```

1. See [:material-code-braces: AnalyticsBinKeyTypeDef](./type_defs.md#analyticsbinkeytypedef) 
2. See [:material-code-braces: AnalyticsIntentGroupByKeyTypeDef](./type_defs.md#analyticsintentgroupbykeytypedef) 
3. See [:material-code-braces: AnalyticsIntentMetricResultTypeDef](./type_defs.md#analyticsintentmetricresulttypedef) 
## AnalyticsIntentStageResultTypeDef

```python
# AnalyticsIntentStageResultTypeDef definition

class AnalyticsIntentStageResultTypeDef(TypedDict):
    binKeys: NotRequired[List[AnalyticsBinKeyTypeDef]],  # (1)
    groupByKeys: NotRequired[List[AnalyticsIntentStageGroupByKeyTypeDef]],  # (2)
    metricsResults: NotRequired[List[AnalyticsIntentStageMetricResultTypeDef]],  # (3)
```

1. See [:material-code-braces: AnalyticsBinKeyTypeDef](./type_defs.md#analyticsbinkeytypedef) 
2. See [:material-code-braces: AnalyticsIntentStageGroupByKeyTypeDef](./type_defs.md#analyticsintentstagegroupbykeytypedef) 
3. See [:material-code-braces: AnalyticsIntentStageMetricResultTypeDef](./type_defs.md#analyticsintentstagemetricresulttypedef) 
## AnalyticsSessionResultTypeDef

```python
# AnalyticsSessionResultTypeDef definition

class AnalyticsSessionResultTypeDef(TypedDict):
    binKeys: NotRequired[List[AnalyticsBinKeyTypeDef]],  # (1)
    groupByKeys: NotRequired[List[AnalyticsSessionGroupByKeyTypeDef]],  # (2)
    metricsResults: NotRequired[List[AnalyticsSessionMetricResultTypeDef]],  # (3)
```

1. See [:material-code-braces: AnalyticsBinKeyTypeDef](./type_defs.md#analyticsbinkeytypedef) 
2. See [:material-code-braces: AnalyticsSessionGroupByKeyTypeDef](./type_defs.md#analyticssessiongroupbykeytypedef) 
3. See [:material-code-braces: AnalyticsSessionMetricResultTypeDef](./type_defs.md#analyticssessionmetricresulttypedef) 
## AnalyticsUtteranceResultTypeDef

```python
# AnalyticsUtteranceResultTypeDef definition

class AnalyticsUtteranceResultTypeDef(TypedDict):
    binKeys: NotRequired[List[AnalyticsBinKeyTypeDef]],  # (1)
    groupByKeys: NotRequired[List[AnalyticsUtteranceGroupByKeyTypeDef]],  # (2)
    metricsResults: NotRequired[List[AnalyticsUtteranceMetricResultTypeDef]],  # (3)
    attributeResults: NotRequired[List[AnalyticsUtteranceAttributeResultTypeDef]],  # (4)
```

1. See [:material-code-braces: AnalyticsBinKeyTypeDef](./type_defs.md#analyticsbinkeytypedef) 
2. See [:material-code-braces: AnalyticsUtteranceGroupByKeyTypeDef](./type_defs.md#analyticsutterancegroupbykeytypedef) 
3. See [:material-code-braces: AnalyticsUtteranceMetricResultTypeDef](./type_defs.md#analyticsutterancemetricresulttypedef) 
4. See [:material-code-braces: AnalyticsUtteranceAttributeResultTypeDef](./type_defs.md#analyticsutteranceattributeresulttypedef) 
## SearchAssociatedTranscriptsRequestRequestTypeDef

```python
# SearchAssociatedTranscriptsRequestRequestTypeDef definition

class SearchAssociatedTranscriptsRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationId: str,
    filters: Sequence[AssociatedTranscriptFilterTypeDef],  # (1)
    searchOrder: NotRequired[SearchOrderType],  # (2)
    maxResults: NotRequired[int],
    nextIndex: NotRequired[int],
```

1. See [:material-code-braces: AssociatedTranscriptFilterTypeDef](./type_defs.md#associatedtranscriptfiltertypedef) 
2. See [:material-code-brackets: SearchOrderType](./literals.md#searchordertype) 
## AudioAndDTMFInputSpecificationTypeDef

```python
# AudioAndDTMFInputSpecificationTypeDef definition

class AudioAndDTMFInputSpecificationTypeDef(TypedDict):
    startTimeoutMs: int,
    audioSpecification: NotRequired[AudioSpecificationTypeDef],  # (1)
    dtmfSpecification: NotRequired[DTMFSpecificationTypeDef],  # (2)
```

1. See [:material-code-braces: AudioSpecificationTypeDef](./type_defs.md#audiospecificationtypedef) 
2. See [:material-code-braces: DTMFSpecificationTypeDef](./type_defs.md#dtmfspecificationtypedef) 
## AudioLogDestinationTypeDef

```python
# AudioLogDestinationTypeDef definition

class AudioLogDestinationTypeDef(TypedDict):
    s3Bucket: S3BucketLogDestinationTypeDef,  # (1)
```

1. See [:material-code-braces: S3BucketLogDestinationTypeDef](./type_defs.md#s3bucketlogdestinationtypedef) 
## BatchCreateCustomVocabularyItemRequestRequestTypeDef

```python
# BatchCreateCustomVocabularyItemRequestRequestTypeDef definition

class BatchCreateCustomVocabularyItemRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    customVocabularyItemList: Sequence[NewCustomVocabularyItemTypeDef],  # (1)
```

1. See [:material-code-braces: NewCustomVocabularyItemTypeDef](./type_defs.md#newcustomvocabularyitemtypedef) 
## BatchUpdateCustomVocabularyItemRequestRequestTypeDef

```python
# BatchUpdateCustomVocabularyItemRequestRequestTypeDef definition

class BatchUpdateCustomVocabularyItemRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    customVocabularyItemList: Sequence[CustomVocabularyItemTypeDef],  # (1)
```

1. See [:material-code-braces: CustomVocabularyItemTypeDef](./type_defs.md#customvocabularyitemtypedef) 
## BatchCreateCustomVocabularyItemResponseTypeDef

```python
# BatchCreateCustomVocabularyItemResponseTypeDef definition

class BatchCreateCustomVocabularyItemResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    errors: List[FailedCustomVocabularyItemTypeDef],  # (1)
    resources: List[CustomVocabularyItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FailedCustomVocabularyItemTypeDef](./type_defs.md#failedcustomvocabularyitemtypedef) 
2. See [:material-code-braces: CustomVocabularyItemTypeDef](./type_defs.md#customvocabularyitemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteCustomVocabularyItemResponseTypeDef

```python
# BatchDeleteCustomVocabularyItemResponseTypeDef definition

class BatchDeleteCustomVocabularyItemResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    errors: List[FailedCustomVocabularyItemTypeDef],  # (1)
    resources: List[CustomVocabularyItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FailedCustomVocabularyItemTypeDef](./type_defs.md#failedcustomvocabularyitemtypedef) 
2. See [:material-code-braces: CustomVocabularyItemTypeDef](./type_defs.md#customvocabularyitemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateCustomVocabularyItemResponseTypeDef

```python
# BatchUpdateCustomVocabularyItemResponseTypeDef definition

class BatchUpdateCustomVocabularyItemResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    errors: List[FailedCustomVocabularyItemTypeDef],  # (1)
    resources: List[CustomVocabularyItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FailedCustomVocabularyItemTypeDef](./type_defs.md#failedcustomvocabularyitemtypedef) 
2. See [:material-code-braces: CustomVocabularyItemTypeDef](./type_defs.md#customvocabularyitemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BuildBotLocaleResponseTypeDef

```python
# BuildBotLocaleResponseTypeDef definition

class BuildBotLocaleResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botLocaleStatus: BotLocaleStatusType,  # (1)
    lastBuildSubmittedDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: BotLocaleStatusType](./literals.md#botlocalestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourcePolicyResponseTypeDef

```python
# CreateResourcePolicyResponseTypeDef definition

class CreateResourcePolicyResponseTypeDef(TypedDict):
    resourceArn: str,
    revisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourcePolicyStatementResponseTypeDef

```python
# CreateResourcePolicyStatementResponseTypeDef definition

class CreateResourcePolicyStatementResponseTypeDef(TypedDict):
    resourceArn: str,
    revisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUploadUrlResponseTypeDef

```python
# CreateUploadUrlResponseTypeDef definition

class CreateUploadUrlResponseTypeDef(TypedDict):
    importId: str,
    uploadUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBotAliasResponseTypeDef

```python
# DeleteBotAliasResponseTypeDef definition

class DeleteBotAliasResponseTypeDef(TypedDict):
    botAliasId: str,
    botId: str,
    botAliasStatus: BotAliasStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: BotAliasStatusType](./literals.md#botaliasstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBotLocaleResponseTypeDef

```python
# DeleteBotLocaleResponseTypeDef definition

class DeleteBotLocaleResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botLocaleStatus: BotLocaleStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: BotLocaleStatusType](./literals.md#botlocalestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBotResponseTypeDef

```python
# DeleteBotResponseTypeDef definition

class DeleteBotResponseTypeDef(TypedDict):
    botId: str,
    botStatus: BotStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: BotStatusType](./literals.md#botstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBotVersionResponseTypeDef

```python
# DeleteBotVersionResponseTypeDef definition

class DeleteBotVersionResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    botStatus: BotStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: BotStatusType](./literals.md#botstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCustomVocabularyResponseTypeDef

```python
# DeleteCustomVocabularyResponseTypeDef definition

class DeleteCustomVocabularyResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    customVocabularyStatus: CustomVocabularyStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CustomVocabularyStatusType](./literals.md#customvocabularystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteExportResponseTypeDef

```python
# DeleteExportResponseTypeDef definition

class DeleteExportResponseTypeDef(TypedDict):
    exportId: str,
    exportStatus: ExportStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteImportResponseTypeDef

```python
# DeleteImportResponseTypeDef definition

class DeleteImportResponseTypeDef(TypedDict):
    importId: str,
    importStatus: ImportStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteResourcePolicyResponseTypeDef

```python
# DeleteResourcePolicyResponseTypeDef definition

class DeleteResourcePolicyResponseTypeDef(TypedDict):
    resourceArn: str,
    revisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteResourcePolicyStatementResponseTypeDef

```python
# DeleteResourcePolicyStatementResponseTypeDef definition

class DeleteResourcePolicyStatementResponseTypeDef(TypedDict):
    resourceArn: str,
    revisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCustomVocabularyMetadataResponseTypeDef

```python
# DescribeCustomVocabularyMetadataResponseTypeDef definition

class DescribeCustomVocabularyMetadataResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    customVocabularyStatus: CustomVocabularyStatusType,  # (1)
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CustomVocabularyStatusType](./literals.md#customvocabularystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeResourcePolicyResponseTypeDef

```python
# DescribeResourcePolicyResponseTypeDef definition

class DescribeResourcePolicyResponseTypeDef(TypedDict):
    resourceArn: str,
    policy: str,
    revisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTestExecutionArtifactsUrlResponseTypeDef

```python
# GetTestExecutionArtifactsUrlResponseTypeDef definition

class GetTestExecutionArtifactsUrlResponseTypeDef(TypedDict):
    testExecutionId: str,
    downloadArtifactsUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomVocabularyItemsResponseTypeDef

```python
# ListCustomVocabularyItemsResponseTypeDef definition

class ListCustomVocabularyItemsResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    customVocabularyItems: List[CustomVocabularyItemTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomVocabularyItemTypeDef](./type_defs.md#customvocabularyitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIntentPathsResponseTypeDef

```python
# ListIntentPathsResponseTypeDef definition

class ListIntentPathsResponseTypeDef(TypedDict):
    nodeSummaries: List[AnalyticsIntentNodeSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalyticsIntentNodeSummaryTypeDef](./type_defs.md#analyticsintentnodesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchAssociatedTranscriptsResponseTypeDef

```python
# SearchAssociatedTranscriptsResponseTypeDef definition

class SearchAssociatedTranscriptsResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationId: str,
    nextIndex: int,
    associatedTranscripts: List[AssociatedTranscriptTypeDef],  # (1)
    totalResults: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssociatedTranscriptTypeDef](./type_defs.md#associatedtranscripttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopBotRecommendationResponseTypeDef

```python
# StopBotRecommendationResponseTypeDef definition

class StopBotRecommendationResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationStatus: BotRecommendationStatusType,  # (1)
    botRecommendationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: BotRecommendationStatusType](./literals.md#botrecommendationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResourcePolicyResponseTypeDef

```python
# UpdateResourcePolicyResponseTypeDef definition

class UpdateResourcePolicyResponseTypeDef(TypedDict):
    resourceArn: str,
    revisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteCustomVocabularyItemRequestRequestTypeDef

```python
# BatchDeleteCustomVocabularyItemRequestRequestTypeDef definition

class BatchDeleteCustomVocabularyItemRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    customVocabularyItemList: Sequence[CustomVocabularyEntryIdTypeDef],  # (1)
```

1. See [:material-code-braces: CustomVocabularyEntryIdTypeDef](./type_defs.md#customvocabularyentryidtypedef) 
## ListBotAliasesResponseTypeDef

```python
# ListBotAliasesResponseTypeDef definition

class ListBotAliasesResponseTypeDef(TypedDict):
    botAliasSummaries: List[BotAliasSummaryTypeDef],  # (1)
    nextToken: str,
    botId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BotAliasSummaryTypeDef](./type_defs.md#botaliassummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestExecutionTargetTypeDef

```python
# TestExecutionTargetTypeDef definition

class TestExecutionTargetTypeDef(TypedDict):
    botAliasTarget: NotRequired[BotAliasTestExecutionTargetTypeDef],  # (1)
```

1. See [:material-code-braces: BotAliasTestExecutionTargetTypeDef](./type_defs.md#botaliastestexecutiontargettypedef) 
## BotImportSpecificationTypeDef

```python
# BotImportSpecificationTypeDef definition

class BotImportSpecificationTypeDef(TypedDict):
    botName: str,
    roleArn: str,
    dataPrivacy: DataPrivacyTypeDef,  # (1)
    idleSessionTTLInSeconds: NotRequired[int],
    botTags: NotRequired[Dict[str, str]],
    testBotAliasTags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DataPrivacyTypeDef](./type_defs.md#dataprivacytypedef) 
## BotLocaleImportSpecificationTypeDef

```python
# BotLocaleImportSpecificationTypeDef definition

class BotLocaleImportSpecificationTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    nluIntentConfidenceThreshold: NotRequired[float],
    voiceSettings: NotRequired[VoiceSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: VoiceSettingsTypeDef](./type_defs.md#voicesettingstypedef) 
## CreateBotLocaleRequestRequestTypeDef

```python
# CreateBotLocaleRequestRequestTypeDef definition

class CreateBotLocaleRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    nluIntentConfidenceThreshold: float,
    description: NotRequired[str],
    voiceSettings: NotRequired[VoiceSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: VoiceSettingsTypeDef](./type_defs.md#voicesettingstypedef) 
## CreateBotLocaleResponseTypeDef

```python
# CreateBotLocaleResponseTypeDef definition

class CreateBotLocaleResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeName: str,
    localeId: str,
    description: str,
    nluIntentConfidenceThreshold: float,
    voiceSettings: VoiceSettingsTypeDef,  # (1)
    botLocaleStatus: BotLocaleStatusType,  # (2)
    creationDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: VoiceSettingsTypeDef](./type_defs.md#voicesettingstypedef) 
2. See [:material-code-brackets: BotLocaleStatusType](./literals.md#botlocalestatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBotLocaleResponseTypeDef

```python
# DescribeBotLocaleResponseTypeDef definition

class DescribeBotLocaleResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    localeName: str,
    description: str,
    nluIntentConfidenceThreshold: float,
    voiceSettings: VoiceSettingsTypeDef,  # (1)
    intentsCount: int,
    slotTypesCount: int,
    botLocaleStatus: BotLocaleStatusType,  # (2)
    failureReasons: List[str],
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    lastBuildSubmittedDateTime: datetime,
    botLocaleHistoryEvents: List[BotLocaleHistoryEventTypeDef],  # (3)
    recommendedActions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: VoiceSettingsTypeDef](./type_defs.md#voicesettingstypedef) 
2. See [:material-code-brackets: BotLocaleStatusType](./literals.md#botlocalestatustype) 
3. See [:material-code-braces: BotLocaleHistoryEventTypeDef](./type_defs.md#botlocalehistoryeventtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBotLocaleRequestRequestTypeDef

```python
# UpdateBotLocaleRequestRequestTypeDef definition

class UpdateBotLocaleRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    nluIntentConfidenceThreshold: float,
    description: NotRequired[str],
    voiceSettings: NotRequired[VoiceSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: VoiceSettingsTypeDef](./type_defs.md#voicesettingstypedef) 
## UpdateBotLocaleResponseTypeDef

```python
# UpdateBotLocaleResponseTypeDef definition

class UpdateBotLocaleResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    localeName: str,
    description: str,
    nluIntentConfidenceThreshold: float,
    voiceSettings: VoiceSettingsTypeDef,  # (1)
    botLocaleStatus: BotLocaleStatusType,  # (2)
    failureReasons: List[str],
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    recommendedActions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: VoiceSettingsTypeDef](./type_defs.md#voicesettingstypedef) 
2. See [:material-code-brackets: BotLocaleStatusType](./literals.md#botlocalestatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBotLocalesRequestRequestTypeDef

```python
# ListBotLocalesRequestRequestTypeDef definition

class ListBotLocalesRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    sortBy: NotRequired[BotLocaleSortByTypeDef],  # (1)
    filters: NotRequired[Sequence[BotLocaleFilterTypeDef]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BotLocaleSortByTypeDef](./type_defs.md#botlocalesortbytypedef) 
2. See [:material-code-braces: BotLocaleFilterTypeDef](./type_defs.md#botlocalefiltertypedef) 
## ListBotLocalesResponseTypeDef

```python
# ListBotLocalesResponseTypeDef definition

class ListBotLocalesResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    nextToken: str,
    botLocaleSummaries: List[BotLocaleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BotLocaleSummaryTypeDef](./type_defs.md#botlocalesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBotRequestRequestTypeDef

```python
# CreateBotRequestRequestTypeDef definition

class CreateBotRequestRequestTypeDef(TypedDict):
    botName: str,
    roleArn: str,
    dataPrivacy: DataPrivacyTypeDef,  # (1)
    idleSessionTTLInSeconds: int,
    description: NotRequired[str],
    botTags: NotRequired[Mapping[str, str]],
    testBotAliasTags: NotRequired[Mapping[str, str]],
    botType: NotRequired[BotTypeType],  # (2)
    botMembers: NotRequired[Sequence[BotMemberTypeDef]],  # (3)
```

1. See [:material-code-braces: DataPrivacyTypeDef](./type_defs.md#dataprivacytypedef) 
2. See [:material-code-brackets: BotTypeType](./literals.md#bottypetype) 
3. See [:material-code-braces: BotMemberTypeDef](./type_defs.md#botmembertypedef) 
## CreateBotResponseTypeDef

```python
# CreateBotResponseTypeDef definition

class CreateBotResponseTypeDef(TypedDict):
    botId: str,
    botName: str,
    description: str,
    roleArn: str,
    dataPrivacy: DataPrivacyTypeDef,  # (1)
    idleSessionTTLInSeconds: int,
    botStatus: BotStatusType,  # (2)
    creationDateTime: datetime,
    botTags: Dict[str, str],
    testBotAliasTags: Dict[str, str],
    botType: BotTypeType,  # (3)
    botMembers: List[BotMemberTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DataPrivacyTypeDef](./type_defs.md#dataprivacytypedef) 
2. See [:material-code-brackets: BotStatusType](./literals.md#botstatustype) 
3. See [:material-code-brackets: BotTypeType](./literals.md#bottypetype) 
4. See [:material-code-braces: BotMemberTypeDef](./type_defs.md#botmembertypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBotResponseTypeDef

```python
# DescribeBotResponseTypeDef definition

class DescribeBotResponseTypeDef(TypedDict):
    botId: str,
    botName: str,
    description: str,
    roleArn: str,
    dataPrivacy: DataPrivacyTypeDef,  # (1)
    idleSessionTTLInSeconds: int,
    botStatus: BotStatusType,  # (2)
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    botType: BotTypeType,  # (3)
    botMembers: List[BotMemberTypeDef],  # (4)
    failureReasons: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DataPrivacyTypeDef](./type_defs.md#dataprivacytypedef) 
2. See [:material-code-brackets: BotStatusType](./literals.md#botstatustype) 
3. See [:material-code-brackets: BotTypeType](./literals.md#bottypetype) 
4. See [:material-code-braces: BotMemberTypeDef](./type_defs.md#botmembertypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBotRequestRequestTypeDef

```python
# UpdateBotRequestRequestTypeDef definition

class UpdateBotRequestRequestTypeDef(TypedDict):
    botId: str,
    botName: str,
    roleArn: str,
    dataPrivacy: DataPrivacyTypeDef,  # (1)
    idleSessionTTLInSeconds: int,
    description: NotRequired[str],
    botType: NotRequired[BotTypeType],  # (2)
    botMembers: NotRequired[Sequence[BotMemberTypeDef]],  # (3)
```

1. See [:material-code-braces: DataPrivacyTypeDef](./type_defs.md#dataprivacytypedef) 
2. See [:material-code-brackets: BotTypeType](./literals.md#bottypetype) 
3. See [:material-code-braces: BotMemberTypeDef](./type_defs.md#botmembertypedef) 
## UpdateBotResponseTypeDef

```python
# UpdateBotResponseTypeDef definition

class UpdateBotResponseTypeDef(TypedDict):
    botId: str,
    botName: str,
    description: str,
    roleArn: str,
    dataPrivacy: DataPrivacyTypeDef,  # (1)
    idleSessionTTLInSeconds: int,
    botStatus: BotStatusType,  # (2)
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    botType: BotTypeType,  # (3)
    botMembers: List[BotMemberTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DataPrivacyTypeDef](./type_defs.md#dataprivacytypedef) 
2. See [:material-code-brackets: BotStatusType](./literals.md#botstatustype) 
3. See [:material-code-brackets: BotTypeType](./literals.md#bottypetype) 
4. See [:material-code-braces: BotMemberTypeDef](./type_defs.md#botmembertypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BotRecommendationResultStatisticsTypeDef

```python
# BotRecommendationResultStatisticsTypeDef definition

class BotRecommendationResultStatisticsTypeDef(TypedDict):
    intents: NotRequired[IntentStatisticsTypeDef],  # (1)
    slotTypes: NotRequired[SlotTypeStatisticsTypeDef],  # (2)
```

1. See [:material-code-braces: IntentStatisticsTypeDef](./type_defs.md#intentstatisticstypedef) 
2. See [:material-code-braces: SlotTypeStatisticsTypeDef](./type_defs.md#slottypestatisticstypedef) 
## ListBotRecommendationsResponseTypeDef

```python
# ListBotRecommendationsResponseTypeDef definition

class ListBotRecommendationsResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationSummaries: List[BotRecommendationSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BotRecommendationSummaryTypeDef](./type_defs.md#botrecommendationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBotsRequestRequestTypeDef

```python
# ListBotsRequestRequestTypeDef definition

class ListBotsRequestRequestTypeDef(TypedDict):
    sortBy: NotRequired[BotSortByTypeDef],  # (1)
    filters: NotRequired[Sequence[BotFilterTypeDef]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BotSortByTypeDef](./type_defs.md#botsortbytypedef) 
2. See [:material-code-braces: BotFilterTypeDef](./type_defs.md#botfiltertypedef) 
## ListBotsResponseTypeDef

```python
# ListBotsResponseTypeDef definition

class ListBotsResponseTypeDef(TypedDict):
    botSummaries: List[BotSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BotSummaryTypeDef](./type_defs.md#botsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBotVersionRequestRequestTypeDef

```python
# CreateBotVersionRequestRequestTypeDef definition

class CreateBotVersionRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersionLocaleSpecification: Mapping[str, BotVersionLocaleDetailsTypeDef],  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: BotVersionLocaleDetailsTypeDef](./type_defs.md#botversionlocaledetailstypedef) 
## CreateBotVersionResponseTypeDef

```python
# CreateBotVersionResponseTypeDef definition

class CreateBotVersionResponseTypeDef(TypedDict):
    botId: str,
    description: str,
    botVersion: str,
    botVersionLocaleSpecification: Dict[str, BotVersionLocaleDetailsTypeDef],  # (1)
    botStatus: BotStatusType,  # (2)
    creationDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BotVersionLocaleDetailsTypeDef](./type_defs.md#botversionlocaledetailstypedef) 
2. See [:material-code-brackets: BotStatusType](./literals.md#botstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBotVersionsRequestRequestTypeDef

```python
# ListBotVersionsRequestRequestTypeDef definition

class ListBotVersionsRequestRequestTypeDef(TypedDict):
    botId: str,
    sortBy: NotRequired[BotVersionSortByTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BotVersionSortByTypeDef](./type_defs.md#botversionsortbytypedef) 
## ListBotVersionsResponseTypeDef

```python
# ListBotVersionsResponseTypeDef definition

class ListBotVersionsResponseTypeDef(TypedDict):
    botId: str,
    botVersionSummaries: List[BotVersionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BotVersionSummaryTypeDef](./type_defs.md#botversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBuiltInIntentsRequestRequestTypeDef

```python
# ListBuiltInIntentsRequestRequestTypeDef definition

class ListBuiltInIntentsRequestRequestTypeDef(TypedDict):
    localeId: str,
    sortBy: NotRequired[BuiltInIntentSortByTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BuiltInIntentSortByTypeDef](./type_defs.md#builtinintentsortbytypedef) 
## ListBuiltInIntentsResponseTypeDef

```python
# ListBuiltInIntentsResponseTypeDef definition

class ListBuiltInIntentsResponseTypeDef(TypedDict):
    builtInIntentSummaries: List[BuiltInIntentSummaryTypeDef],  # (1)
    nextToken: str,
    localeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuiltInIntentSummaryTypeDef](./type_defs.md#builtinintentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBuiltInSlotTypesRequestRequestTypeDef

```python
# ListBuiltInSlotTypesRequestRequestTypeDef definition

class ListBuiltInSlotTypesRequestRequestTypeDef(TypedDict):
    localeId: str,
    sortBy: NotRequired[BuiltInSlotTypeSortByTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BuiltInSlotTypeSortByTypeDef](./type_defs.md#builtinslottypesortbytypedef) 
## ListBuiltInSlotTypesResponseTypeDef

```python
# ListBuiltInSlotTypesResponseTypeDef definition

class ListBuiltInSlotTypesResponseTypeDef(TypedDict):
    builtInSlotTypeSummaries: List[BuiltInSlotTypeSummaryTypeDef],  # (1)
    nextToken: str,
    localeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuiltInSlotTypeSummaryTypeDef](./type_defs.md#builtinslottypesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImageResponseCardTypeDef

```python
# ImageResponseCardTypeDef definition

class ImageResponseCardTypeDef(TypedDict):
    title: str,
    subtitle: NotRequired[str],
    imageUrl: NotRequired[str],
    buttons: NotRequired[Sequence[ButtonTypeDef]],  # (1)
```

1. See [:material-code-braces: ButtonTypeDef](./type_defs.md#buttontypedef) 
## TextLogDestinationTypeDef

```python
# TextLogDestinationTypeDef definition

class TextLogDestinationTypeDef(TypedDict):
    cloudWatch: CloudWatchLogGroupLogDestinationTypeDef,  # (1)
```

1. See [:material-code-braces: CloudWatchLogGroupLogDestinationTypeDef](./type_defs.md#cloudwatchloggrouplogdestinationtypedef) 
## CodeHookSpecificationTypeDef

```python
# CodeHookSpecificationTypeDef definition

class CodeHookSpecificationTypeDef(TypedDict):
    lambdaCodeHook: LambdaCodeHookTypeDef,  # (1)
```

1. See [:material-code-braces: LambdaCodeHookTypeDef](./type_defs.md#lambdacodehooktypedef) 
## CompositeSlotTypeSettingTypeDef

```python
# CompositeSlotTypeSettingTypeDef definition

class CompositeSlotTypeSettingTypeDef(TypedDict):
    subSlots: NotRequired[Sequence[SubSlotTypeCompositionTypeDef]],  # (1)
```

1. See [:material-code-braces: SubSlotTypeCompositionTypeDef](./type_defs.md#subslottypecompositiontypedef) 
## ConversationLevelTestResultItemTypeDef

```python
# ConversationLevelTestResultItemTypeDef definition

class ConversationLevelTestResultItemTypeDef(TypedDict):
    conversationId: str,
    endToEndResult: TestResultMatchStatusType,  # (1)
    intentClassificationResults: List[ConversationLevelIntentClassificationResultItemTypeDef],  # (3)
    slotResolutionResults: List[ConversationLevelSlotResolutionResultItemTypeDef],  # (4)
    speechTranscriptionResult: NotRequired[TestResultMatchStatusType],  # (1)
```

1. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
2. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
3. See [:material-code-braces: ConversationLevelIntentClassificationResultItemTypeDef](./type_defs.md#conversationlevelintentclassificationresultitemtypedef) 
4. See [:material-code-braces: ConversationLevelSlotResolutionResultItemTypeDef](./type_defs.md#conversationlevelslotresolutionresultitemtypedef) 
## TestExecutionResultFilterByTypeDef

```python
# TestExecutionResultFilterByTypeDef definition

class TestExecutionResultFilterByTypeDef(TypedDict):
    resultTypeFilter: TestResultTypeFilterType,  # (1)
    conversationLevelTestResultsFilterBy: NotRequired[ConversationLevelTestResultsFilterByTypeDef],  # (2)
```

1. See [:material-code-brackets: TestResultTypeFilterType](./literals.md#testresulttypefiltertype) 
2. See [:material-code-braces: ConversationLevelTestResultsFilterByTypeDef](./type_defs.md#conversationleveltestresultsfilterbytypedef) 
## ConversationLogsDataSourceTypeDef

```python
# ConversationLogsDataSourceTypeDef definition

class ConversationLogsDataSourceTypeDef(TypedDict):
    botId: str,
    botAliasId: str,
    localeId: str,
    filter: ConversationLogsDataSourceFilterByTypeDef,  # (1)
```

1. See [:material-code-braces: ConversationLogsDataSourceFilterByTypeDef](./type_defs.md#conversationlogsdatasourcefilterbytypedef) 
## IntentSummaryTypeDef

```python
# IntentSummaryTypeDef definition

class IntentSummaryTypeDef(TypedDict):
    intentId: NotRequired[str],
    intentName: NotRequired[str],
    description: NotRequired[str],
    parentIntentSignature: NotRequired[str],
    inputContexts: NotRequired[List[InputContextTypeDef]],  # (1)
    outputContexts: NotRequired[List[OutputContextTypeDef]],  # (2)
    lastUpdatedDateTime: NotRequired[datetime],
```

1. See [:material-code-braces: InputContextTypeDef](./type_defs.md#inputcontexttypedef) 
2. See [:material-code-braces: OutputContextTypeDef](./type_defs.md#outputcontexttypedef) 
## CreateResourcePolicyStatementRequestRequestTypeDef

```python
# CreateResourcePolicyStatementRequestRequestTypeDef definition

class CreateResourcePolicyStatementRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    statementId: str,
    effect: EffectType,  # (1)
    principal: Sequence[PrincipalTypeDef],  # (2)
    action: Sequence[str],
    condition: NotRequired[Mapping[str, Mapping[str, str]]],
    expectedRevisionId: NotRequired[str],
```

1. See [:material-code-brackets: EffectType](./literals.md#effecttype) 
2. See [:material-code-braces: PrincipalTypeDef](./type_defs.md#principaltypedef) 
## LexTranscriptFilterTypeDef

```python
# LexTranscriptFilterTypeDef definition

class LexTranscriptFilterTypeDef(TypedDict):
    dateRangeFilter: NotRequired[DateRangeFilterTypeDef],  # (1)
```

1. See [:material-code-braces: DateRangeFilterTypeDef](./type_defs.md#daterangefiltertypedef) 
## DescribeBotAliasRequestBotAliasAvailableWaitTypeDef

```python
# DescribeBotAliasRequestBotAliasAvailableWaitTypeDef definition

class DescribeBotAliasRequestBotAliasAvailableWaitTypeDef(TypedDict):
    botAliasId: str,
    botId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef

```python
# DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef definition

class DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef

```python
# DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef definition

class DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef

```python
# DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef definition

class DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeBotRequestBotAvailableWaitTypeDef

```python
# DescribeBotRequestBotAvailableWaitTypeDef definition

class DescribeBotRequestBotAvailableWaitTypeDef(TypedDict):
    botId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeBotVersionRequestBotVersionAvailableWaitTypeDef

```python
# DescribeBotVersionRequestBotVersionAvailableWaitTypeDef definition

class DescribeBotVersionRequestBotVersionAvailableWaitTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeExportRequestBotExportCompletedWaitTypeDef

```python
# DescribeExportRequestBotExportCompletedWaitTypeDef definition

class DescribeExportRequestBotExportCompletedWaitTypeDef(TypedDict):
    exportId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeImportRequestBotImportCompletedWaitTypeDef

```python
# DescribeImportRequestBotImportCompletedWaitTypeDef definition

class DescribeImportRequestBotImportCompletedWaitTypeDef(TypedDict):
    importId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeBotVersionResponseTypeDef

```python
# DescribeBotVersionResponseTypeDef definition

class DescribeBotVersionResponseTypeDef(TypedDict):
    botId: str,
    botName: str,
    botVersion: str,
    description: str,
    roleArn: str,
    dataPrivacy: DataPrivacyTypeDef,  # (1)
    idleSessionTTLInSeconds: int,
    botStatus: BotStatusType,  # (2)
    failureReasons: List[str],
    creationDateTime: datetime,
    parentBotNetworks: List[ParentBotNetworkTypeDef],  # (3)
    botType: BotTypeType,  # (4)
    botMembers: List[BotMemberTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: DataPrivacyTypeDef](./type_defs.md#dataprivacytypedef) 
2. See [:material-code-brackets: BotStatusType](./literals.md#botstatustype) 
3. See [:material-code-braces: ParentBotNetworkTypeDef](./type_defs.md#parentbotnetworktypedef) 
4. See [:material-code-brackets: BotTypeType](./literals.md#bottypetype) 
5. See [:material-code-braces: BotMemberTypeDef](./type_defs.md#botmembertypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBotRecommendationRequestRequestTypeDef

```python
# UpdateBotRecommendationRequestRequestTypeDef definition

class UpdateBotRecommendationRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationId: str,
    encryptionSetting: EncryptionSettingTypeDef,  # (1)
```

1. See [:material-code-braces: EncryptionSettingTypeDef](./type_defs.md#encryptionsettingtypedef) 
## DescribeTestSetResponseTypeDef

```python
# DescribeTestSetResponseTypeDef definition

class DescribeTestSetResponseTypeDef(TypedDict):
    testSetId: str,
    testSetName: str,
    description: str,
    modality: TestSetModalityType,  # (1)
    status: TestSetStatusType,  # (2)
    roleArn: str,
    numTurns: int,
    storageLocation: TestSetStorageLocationTypeDef,  # (3)
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: TestSetModalityType](./literals.md#testsetmodalitytype) 
2. See [:material-code-brackets: TestSetStatusType](./literals.md#testsetstatustype) 
3. See [:material-code-braces: TestSetStorageLocationTypeDef](./type_defs.md#testsetstoragelocationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestSetSummaryTypeDef

```python
# TestSetSummaryTypeDef definition

class TestSetSummaryTypeDef(TypedDict):
    testSetId: NotRequired[str],
    testSetName: NotRequired[str],
    description: NotRequired[str],
    modality: NotRequired[TestSetModalityType],  # (1)
    status: NotRequired[TestSetStatusType],  # (2)
    roleArn: NotRequired[str],
    numTurns: NotRequired[int],
    storageLocation: NotRequired[TestSetStorageLocationTypeDef],  # (3)
    creationDateTime: NotRequired[datetime],
    lastUpdatedDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: TestSetModalityType](./literals.md#testsetmodalitytype) 
2. See [:material-code-brackets: TestSetStatusType](./literals.md#testsetstatustype) 
3. See [:material-code-braces: TestSetStorageLocationTypeDef](./type_defs.md#testsetstoragelocationtypedef) 
## UpdateTestSetResponseTypeDef

```python
# UpdateTestSetResponseTypeDef definition

class UpdateTestSetResponseTypeDef(TypedDict):
    testSetId: str,
    testSetName: str,
    description: str,
    modality: TestSetModalityType,  # (1)
    status: TestSetStatusType,  # (2)
    roleArn: str,
    numTurns: int,
    storageLocation: TestSetStorageLocationTypeDef,  # (3)
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: TestSetModalityType](./literals.md#testsetmodalitytype) 
2. See [:material-code-brackets: TestSetStatusType](./literals.md#testsetstatustype) 
3. See [:material-code-braces: TestSetStorageLocationTypeDef](./type_defs.md#testsetstoragelocationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DialogStateTypeDef

```python
# DialogStateTypeDef definition

class DialogStateTypeDef(TypedDict):
    dialogAction: NotRequired[DialogActionTypeDef],  # (1)
    intent: NotRequired[IntentOverrideTypeDef],  # (2)
    sessionAttributes: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DialogActionTypeDef](./type_defs.md#dialogactiontypedef) 
2. See [:material-code-braces: IntentOverrideTypeDef](./type_defs.md#intentoverridetypedef) 
## ExportResourceSpecificationTypeDef

```python
# ExportResourceSpecificationTypeDef definition

class ExportResourceSpecificationTypeDef(TypedDict):
    botExportSpecification: NotRequired[BotExportSpecificationTypeDef],  # (1)
    botLocaleExportSpecification: NotRequired[BotLocaleExportSpecificationTypeDef],  # (2)
    customVocabularyExportSpecification: NotRequired[CustomVocabularyExportSpecificationTypeDef],  # (3)
    testSetExportSpecification: NotRequired[TestSetExportSpecificationTypeDef],  # (4)
```

1. See [:material-code-braces: BotExportSpecificationTypeDef](./type_defs.md#botexportspecificationtypedef) 
2. See [:material-code-braces: BotLocaleExportSpecificationTypeDef](./type_defs.md#botlocaleexportspecificationtypedef) 
3. See [:material-code-braces: CustomVocabularyExportSpecificationTypeDef](./type_defs.md#customvocabularyexportspecificationtypedef) 
4. See [:material-code-braces: TestSetExportSpecificationTypeDef](./type_defs.md#testsetexportspecificationtypedef) 
## ListExportsRequestRequestTypeDef

```python
# ListExportsRequestRequestTypeDef definition

class ListExportsRequestRequestTypeDef(TypedDict):
    botId: NotRequired[str],
    botVersion: NotRequired[str],
    sortBy: NotRequired[ExportSortByTypeDef],  # (1)
    filters: NotRequired[Sequence[ExportFilterTypeDef]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    localeId: NotRequired[str],
```

1. See [:material-code-braces: ExportSortByTypeDef](./type_defs.md#exportsortbytypedef) 
2. See [:material-code-braces: ExportFilterTypeDef](./type_defs.md#exportfiltertypedef) 
## GrammarSlotTypeSettingTypeDef

```python
# GrammarSlotTypeSettingTypeDef definition

class GrammarSlotTypeSettingTypeDef(TypedDict):
    source: NotRequired[GrammarSlotTypeSourceTypeDef],  # (1)
```

1. See [:material-code-braces: GrammarSlotTypeSourceTypeDef](./type_defs.md#grammarslottypesourcetypedef) 
## ListImportsRequestRequestTypeDef

```python
# ListImportsRequestRequestTypeDef definition

class ListImportsRequestRequestTypeDef(TypedDict):
    botId: NotRequired[str],
    botVersion: NotRequired[str],
    sortBy: NotRequired[ImportSortByTypeDef],  # (1)
    filters: NotRequired[Sequence[ImportFilterTypeDef]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    localeId: NotRequired[str],
```

1. See [:material-code-braces: ImportSortByTypeDef](./type_defs.md#importsortbytypedef) 
2. See [:material-code-braces: ImportFilterTypeDef](./type_defs.md#importfiltertypedef) 
## ListImportsResponseTypeDef

```python
# ListImportsResponseTypeDef definition

class ListImportsResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    importSummaries: List[ImportSummaryTypeDef],  # (1)
    nextToken: str,
    localeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportSummaryTypeDef](./type_defs.md#importsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InputSessionStateSpecificationTypeDef

```python
# InputSessionStateSpecificationTypeDef definition

class InputSessionStateSpecificationTypeDef(TypedDict):
    sessionAttributes: NotRequired[Dict[str, str]],
    activeContexts: NotRequired[List[ActiveContextTypeDef]],  # (1)
    runtimeHints: NotRequired[RuntimeHintsTypeDef],  # (2)
```

1. See [:material-code-braces: ActiveContextTypeDef](./type_defs.md#activecontexttypedef) 
2. See [:material-code-braces: RuntimeHintsTypeDef](./type_defs.md#runtimehintstypedef) 
## IntentClassificationTestResultItemTypeDef

```python
# IntentClassificationTestResultItemTypeDef definition

class IntentClassificationTestResultItemTypeDef(TypedDict):
    intentName: str,
    multiTurnConversation: bool,
    resultCounts: IntentClassificationTestResultItemCountsTypeDef,  # (1)
```

1. See [:material-code-braces: IntentClassificationTestResultItemCountsTypeDef](./type_defs.md#intentclassificationtestresultitemcountstypedef) 
## ListIntentsRequestRequestTypeDef

```python
# ListIntentsRequestRequestTypeDef definition

class ListIntentsRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    sortBy: NotRequired[IntentSortByTypeDef],  # (1)
    filters: NotRequired[Sequence[IntentFilterTypeDef]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IntentSortByTypeDef](./type_defs.md#intentsortbytypedef) 
2. See [:material-code-braces: IntentFilterTypeDef](./type_defs.md#intentfiltertypedef) 
## SessionSpecificationTypeDef

```python
# SessionSpecificationTypeDef definition

class SessionSpecificationTypeDef(TypedDict):
    botAliasId: NotRequired[str],
    botVersion: NotRequired[str],
    localeId: NotRequired[str],
    channel: NotRequired[str],
    sessionId: NotRequired[str],
    conversationStartTime: NotRequired[datetime],
    conversationEndTime: NotRequired[datetime],
    conversationDurationSeconds: NotRequired[int],
    conversationEndState: NotRequired[ConversationEndStateType],  # (1)
    mode: NotRequired[AnalyticsModalityType],  # (2)
    numberOfTurns: NotRequired[int],
    invokedIntentSamples: NotRequired[List[InvokedIntentSampleTypeDef]],  # (3)
    originatingRequestId: NotRequired[str],
```

1. See [:material-code-brackets: ConversationEndStateType](./literals.md#conversationendstatetype) 
2. See [:material-code-brackets: AnalyticsModalityType](./literals.md#analyticsmodalitytype) 
3. See [:material-code-braces: InvokedIntentSampleTypeDef](./type_defs.md#invokedintentsampletypedef) 
## ListIntentMetricsRequestRequestTypeDef

```python
# ListIntentMetricsRequestRequestTypeDef definition

class ListIntentMetricsRequestRequestTypeDef(TypedDict):
    botId: str,
    startDateTime: Union[datetime, str],
    endDateTime: Union[datetime, str],
    metrics: Sequence[AnalyticsIntentMetricTypeDef],  # (1)
    binBy: NotRequired[Sequence[AnalyticsBinBySpecificationTypeDef]],  # (2)
    groupBy: NotRequired[Sequence[AnalyticsIntentGroupBySpecificationTypeDef]],  # (3)
    filters: NotRequired[Sequence[AnalyticsIntentFilterTypeDef]],  # (4)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AnalyticsIntentMetricTypeDef](./type_defs.md#analyticsintentmetrictypedef) 
2. See [:material-code-braces: AnalyticsBinBySpecificationTypeDef](./type_defs.md#analyticsbinbyspecificationtypedef) 
3. See [:material-code-braces: AnalyticsIntentGroupBySpecificationTypeDef](./type_defs.md#analyticsintentgroupbyspecificationtypedef) 
4. See [:material-code-braces: AnalyticsIntentFilterTypeDef](./type_defs.md#analyticsintentfiltertypedef) 
## ListIntentPathsRequestRequestTypeDef

```python
# ListIntentPathsRequestRequestTypeDef definition

class ListIntentPathsRequestRequestTypeDef(TypedDict):
    botId: str,
    startDateTime: Union[datetime, str],
    endDateTime: Union[datetime, str],
    intentPath: str,
    filters: NotRequired[Sequence[AnalyticsPathFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: AnalyticsPathFilterTypeDef](./type_defs.md#analyticspathfiltertypedef) 
## ListIntentStageMetricsRequestRequestTypeDef

```python
# ListIntentStageMetricsRequestRequestTypeDef definition

class ListIntentStageMetricsRequestRequestTypeDef(TypedDict):
    botId: str,
    startDateTime: Union[datetime, str],
    endDateTime: Union[datetime, str],
    metrics: Sequence[AnalyticsIntentStageMetricTypeDef],  # (1)
    binBy: NotRequired[Sequence[AnalyticsBinBySpecificationTypeDef]],  # (2)
    groupBy: NotRequired[Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef]],  # (3)
    filters: NotRequired[Sequence[AnalyticsIntentStageFilterTypeDef]],  # (4)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AnalyticsIntentStageMetricTypeDef](./type_defs.md#analyticsintentstagemetrictypedef) 
2. See [:material-code-braces: AnalyticsBinBySpecificationTypeDef](./type_defs.md#analyticsbinbyspecificationtypedef) 
3. See [:material-code-braces: AnalyticsIntentStageGroupBySpecificationTypeDef](./type_defs.md#analyticsintentstagegroupbyspecificationtypedef) 
4. See [:material-code-braces: AnalyticsIntentStageFilterTypeDef](./type_defs.md#analyticsintentstagefiltertypedef) 
## ListSessionMetricsRequestRequestTypeDef

```python
# ListSessionMetricsRequestRequestTypeDef definition

class ListSessionMetricsRequestRequestTypeDef(TypedDict):
    botId: str,
    startDateTime: Union[datetime, str],
    endDateTime: Union[datetime, str],
    metrics: Sequence[AnalyticsSessionMetricTypeDef],  # (1)
    binBy: NotRequired[Sequence[AnalyticsBinBySpecificationTypeDef]],  # (2)
    groupBy: NotRequired[Sequence[AnalyticsSessionGroupBySpecificationTypeDef]],  # (3)
    filters: NotRequired[Sequence[AnalyticsSessionFilterTypeDef]],  # (4)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AnalyticsSessionMetricTypeDef](./type_defs.md#analyticssessionmetrictypedef) 
2. See [:material-code-braces: AnalyticsBinBySpecificationTypeDef](./type_defs.md#analyticsbinbyspecificationtypedef) 
3. See [:material-code-braces: AnalyticsSessionGroupBySpecificationTypeDef](./type_defs.md#analyticssessiongroupbyspecificationtypedef) 
4. See [:material-code-braces: AnalyticsSessionFilterTypeDef](./type_defs.md#analyticssessionfiltertypedef) 
## ListUtteranceMetricsRequestRequestTypeDef

```python
# ListUtteranceMetricsRequestRequestTypeDef definition

class ListUtteranceMetricsRequestRequestTypeDef(TypedDict):
    botId: str,
    startDateTime: Union[datetime, str],
    endDateTime: Union[datetime, str],
    metrics: Sequence[AnalyticsUtteranceMetricTypeDef],  # (1)
    binBy: NotRequired[Sequence[AnalyticsBinBySpecificationTypeDef]],  # (2)
    groupBy: NotRequired[Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef]],  # (3)
    attributes: NotRequired[Sequence[AnalyticsUtteranceAttributeTypeDef]],  # (4)
    filters: NotRequired[Sequence[AnalyticsUtteranceFilterTypeDef]],  # (5)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AnalyticsUtteranceMetricTypeDef](./type_defs.md#analyticsutterancemetrictypedef) 
2. See [:material-code-braces: AnalyticsBinBySpecificationTypeDef](./type_defs.md#analyticsbinbyspecificationtypedef) 
3. See [:material-code-braces: AnalyticsUtteranceGroupBySpecificationTypeDef](./type_defs.md#analyticsutterancegroupbyspecificationtypedef) 
4. See [:material-code-braces: AnalyticsUtteranceAttributeTypeDef](./type_defs.md#analyticsutteranceattributetypedef) 
5. See [:material-code-braces: AnalyticsUtteranceFilterTypeDef](./type_defs.md#analyticsutterancefiltertypedef) 
## ListRecommendedIntentsResponseTypeDef

```python
# ListRecommendedIntentsResponseTypeDef definition

class ListRecommendedIntentsResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationId: str,
    summaryList: List[RecommendedIntentSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommendedIntentSummaryTypeDef](./type_defs.md#recommendedintentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSessionAnalyticsDataRequestRequestTypeDef

```python
# ListSessionAnalyticsDataRequestRequestTypeDef definition

class ListSessionAnalyticsDataRequestRequestTypeDef(TypedDict):
    botId: str,
    startDateTime: Union[datetime, str],
    endDateTime: Union[datetime, str],
    sortBy: NotRequired[SessionDataSortByTypeDef],  # (1)
    filters: NotRequired[Sequence[AnalyticsSessionFilterTypeDef]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SessionDataSortByTypeDef](./type_defs.md#sessiondatasortbytypedef) 
2. See [:material-code-braces: AnalyticsSessionFilterTypeDef](./type_defs.md#analyticssessionfiltertypedef) 
## ListSlotTypesRequestRequestTypeDef

```python
# ListSlotTypesRequestRequestTypeDef definition

class ListSlotTypesRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    sortBy: NotRequired[SlotTypeSortByTypeDef],  # (1)
    filters: NotRequired[Sequence[SlotTypeFilterTypeDef]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SlotTypeSortByTypeDef](./type_defs.md#slottypesortbytypedef) 
2. See [:material-code-braces: SlotTypeFilterTypeDef](./type_defs.md#slottypefiltertypedef) 
## ListSlotTypesResponseTypeDef

```python
# ListSlotTypesResponseTypeDef definition

class ListSlotTypesResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    slotTypeSummaries: List[SlotTypeSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SlotTypeSummaryTypeDef](./type_defs.md#slottypesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSlotsRequestRequestTypeDef

```python
# ListSlotsRequestRequestTypeDef definition

class ListSlotsRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
    sortBy: NotRequired[SlotSortByTypeDef],  # (1)
    filters: NotRequired[Sequence[SlotFilterTypeDef]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SlotSortByTypeDef](./type_defs.md#slotsortbytypedef) 
2. See [:material-code-braces: SlotFilterTypeDef](./type_defs.md#slotfiltertypedef) 
## ListTestExecutionsRequestRequestTypeDef

```python
# ListTestExecutionsRequestRequestTypeDef definition

class ListTestExecutionsRequestRequestTypeDef(TypedDict):
    sortBy: NotRequired[TestExecutionSortByTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestExecutionSortByTypeDef](./type_defs.md#testexecutionsortbytypedef) 
## ListTestSetsRequestRequestTypeDef

```python
# ListTestSetsRequestRequestTypeDef definition

class ListTestSetsRequestRequestTypeDef(TypedDict):
    sortBy: NotRequired[TestSetSortByTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestSetSortByTypeDef](./type_defs.md#testsetsortbytypedef) 
## ListUtteranceAnalyticsDataRequestRequestTypeDef

```python
# ListUtteranceAnalyticsDataRequestRequestTypeDef definition

class ListUtteranceAnalyticsDataRequestRequestTypeDef(TypedDict):
    botId: str,
    startDateTime: Union[datetime, str],
    endDateTime: Union[datetime, str],
    sortBy: NotRequired[UtteranceDataSortByTypeDef],  # (1)
    filters: NotRequired[Sequence[AnalyticsUtteranceFilterTypeDef]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: UtteranceDataSortByTypeDef](./type_defs.md#utterancedatasortbytypedef) 
2. See [:material-code-braces: AnalyticsUtteranceFilterTypeDef](./type_defs.md#analyticsutterancefiltertypedef) 
## OverallTestResultsTypeDef

```python
# OverallTestResultsTypeDef definition

class OverallTestResultsTypeDef(TypedDict):
    items: List[OverallTestResultItemTypeDef],  # (1)
```

1. See [:material-code-braces: OverallTestResultItemTypeDef](./type_defs.md#overalltestresultitemtypedef) 
## UtteranceAggregationDurationTypeDef

```python
# UtteranceAggregationDurationTypeDef definition

class UtteranceAggregationDurationTypeDef(TypedDict):
    relativeAggregationDuration: RelativeAggregationDurationTypeDef,  # (1)
```

1. See [:material-code-braces: RelativeAggregationDurationTypeDef](./type_defs.md#relativeaggregationdurationtypedef) 
## RuntimeHintDetailsTypeDef

```python
# RuntimeHintDetailsTypeDef definition

class RuntimeHintDetailsTypeDef(TypedDict):
    runtimeHintValues: NotRequired[List[RuntimeHintValueTypeDef]],  # (1)
    subSlotHints: NotRequired[Dict[str, RuntimeHintDetailsTypeDef]],  # (2)
```

1. See [:material-code-braces: RuntimeHintValueTypeDef](./type_defs.md#runtimehintvaluetypedef) 
2. See [:material-code-braces: RuntimeHintDetailsTypeDef](./type_defs.md#runtimehintdetailstypedef) 
## SlotTypeValueTypeDef

```python
# SlotTypeValueTypeDef definition

class SlotTypeValueTypeDef(TypedDict):
    sampleValue: NotRequired[SampleValueTypeDef],  # (1)
    synonyms: NotRequired[Sequence[SampleValueTypeDef]],  # (2)
```

1. See [:material-code-braces: SampleValueTypeDef](./type_defs.md#samplevaluetypedef) 
2. See [:material-code-braces: SampleValueTypeDef](./type_defs.md#samplevaluetypedef) 
## SlotDefaultValueSpecificationTypeDef

```python
# SlotDefaultValueSpecificationTypeDef definition

class SlotDefaultValueSpecificationTypeDef(TypedDict):
    defaultValueList: Sequence[SlotDefaultValueTypeDef],  # (1)
```

1. See [:material-code-braces: SlotDefaultValueTypeDef](./type_defs.md#slotdefaultvaluetypedef) 
## SlotResolutionTestResultItemTypeDef

```python
# SlotResolutionTestResultItemTypeDef definition

class SlotResolutionTestResultItemTypeDef(TypedDict):
    slotName: str,
    resultCounts: SlotResolutionTestResultItemCountsTypeDef,  # (1)
```

1. See [:material-code-braces: SlotResolutionTestResultItemCountsTypeDef](./type_defs.md#slotresolutiontestresultitemcountstypedef) 
## SlotValueOverrideTypeDef

```python
# SlotValueOverrideTypeDef definition

class SlotValueOverrideTypeDef(TypedDict):
    shape: NotRequired[SlotShapeType],  # (1)
    value: NotRequired[SlotValueTypeDef],  # (2)
    values: NotRequired[Sequence[SlotValueOverrideTypeDef]],  # (3)
```

1. See [:material-code-brackets: SlotShapeType](./literals.md#slotshapetype) 
2. See [:material-code-braces: SlotValueTypeDef](./type_defs.md#slotvaluetypedef) 
3. See [:material-code-braces: SlotValueOverrideTypeDef](./type_defs.md#slotvalueoverridetypedef) 
## SlotValueSelectionSettingTypeDef

```python
# SlotValueSelectionSettingTypeDef definition

class SlotValueSelectionSettingTypeDef(TypedDict):
    resolutionStrategy: SlotValueResolutionStrategyType,  # (1)
    regexFilter: NotRequired[SlotValueRegexFilterTypeDef],  # (2)
    advancedRecognitionSetting: NotRequired[AdvancedRecognitionSettingTypeDef],  # (3)
```

1. See [:material-code-brackets: SlotValueResolutionStrategyType](./literals.md#slotvalueresolutionstrategytype) 
2. See [:material-code-braces: SlotValueRegexFilterTypeDef](./type_defs.md#slotvalueregexfiltertypedef) 
3. See [:material-code-braces: AdvancedRecognitionSettingTypeDef](./type_defs.md#advancedrecognitionsettingtypedef) 
## TestSetDiscrepancyErrorsTypeDef

```python
# TestSetDiscrepancyErrorsTypeDef definition

class TestSetDiscrepancyErrorsTypeDef(TypedDict):
    intentDiscrepancies: List[TestSetIntentDiscrepancyItemTypeDef],  # (1)
    slotDiscrepancies: List[TestSetSlotDiscrepancyItemTypeDef],  # (2)
```

1. See [:material-code-braces: TestSetIntentDiscrepancyItemTypeDef](./type_defs.md#testsetintentdiscrepancyitemtypedef) 
2. See [:material-code-braces: TestSetSlotDiscrepancyItemTypeDef](./type_defs.md#testsetslotdiscrepancyitemtypedef) 
## TestSetDiscrepancyReportResourceTargetTypeDef

```python
# TestSetDiscrepancyReportResourceTargetTypeDef definition

class TestSetDiscrepancyReportResourceTargetTypeDef(TypedDict):
    botAliasTarget: NotRequired[TestSetDiscrepancyReportBotAliasTargetTypeDef],  # (1)
```

1. See [:material-code-braces: TestSetDiscrepancyReportBotAliasTargetTypeDef](./type_defs.md#testsetdiscrepancyreportbotaliastargettypedef) 
## TestSetImportResourceSpecificationTypeDef

```python
# TestSetImportResourceSpecificationTypeDef definition

class TestSetImportResourceSpecificationTypeDef(TypedDict):
    testSetName: str,
    roleArn: str,
    storageLocation: TestSetStorageLocationTypeDef,  # (1)
    importInputLocation: TestSetImportInputLocationTypeDef,  # (2)
    modality: TestSetModalityType,  # (3)
    description: NotRequired[str],
    testSetTags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: TestSetStorageLocationTypeDef](./type_defs.md#testsetstoragelocationtypedef) 
2. See [:material-code-braces: TestSetImportInputLocationTypeDef](./type_defs.md#testsetimportinputlocationtypedef) 
3. See [:material-code-brackets: TestSetModalityType](./literals.md#testsetmodalitytype) 
## UserTurnOutputSpecificationTypeDef

```python
# UserTurnOutputSpecificationTypeDef definition

class UserTurnOutputSpecificationTypeDef(TypedDict):
    intent: UserTurnIntentOutputTypeDef,  # (1)
    activeContexts: NotRequired[List[ActiveContextTypeDef]],  # (2)
    transcript: NotRequired[str],
```

1. See [:material-code-braces: UserTurnIntentOutputTypeDef](./type_defs.md#userturnintentoutputtypedef) 
2. See [:material-code-braces: ActiveContextTypeDef](./type_defs.md#activecontexttypedef) 
## UtteranceInputSpecificationTypeDef

```python
# UtteranceInputSpecificationTypeDef definition

class UtteranceInputSpecificationTypeDef(TypedDict):
    textInput: NotRequired[str],
    audioInput: NotRequired[UtteranceAudioInputSpecificationTypeDef],  # (1)
```

1. See [:material-code-braces: UtteranceAudioInputSpecificationTypeDef](./type_defs.md#utteranceaudioinputspecificationtypedef) 
## ListIntentMetricsResponseTypeDef

```python
# ListIntentMetricsResponseTypeDef definition

class ListIntentMetricsResponseTypeDef(TypedDict):
    botId: str,
    results: List[AnalyticsIntentResultTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalyticsIntentResultTypeDef](./type_defs.md#analyticsintentresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIntentStageMetricsResponseTypeDef

```python
# ListIntentStageMetricsResponseTypeDef definition

class ListIntentStageMetricsResponseTypeDef(TypedDict):
    botId: str,
    results: List[AnalyticsIntentStageResultTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalyticsIntentStageResultTypeDef](./type_defs.md#analyticsintentstageresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSessionMetricsResponseTypeDef

```python
# ListSessionMetricsResponseTypeDef definition

class ListSessionMetricsResponseTypeDef(TypedDict):
    botId: str,
    results: List[AnalyticsSessionResultTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalyticsSessionResultTypeDef](./type_defs.md#analyticssessionresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUtteranceMetricsResponseTypeDef

```python
# ListUtteranceMetricsResponseTypeDef definition

class ListUtteranceMetricsResponseTypeDef(TypedDict):
    botId: str,
    results: List[AnalyticsUtteranceResultTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalyticsUtteranceResultTypeDef](./type_defs.md#analyticsutteranceresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PromptAttemptSpecificationTypeDef

```python
# PromptAttemptSpecificationTypeDef definition

class PromptAttemptSpecificationTypeDef(TypedDict):
    allowedInputTypes: AllowedInputTypesTypeDef,  # (1)
    allowInterrupt: NotRequired[bool],
    audioAndDTMFInputSpecification: NotRequired[AudioAndDTMFInputSpecificationTypeDef],  # (2)
    textInputSpecification: NotRequired[TextInputSpecificationTypeDef],  # (3)
```

1. See [:material-code-braces: AllowedInputTypesTypeDef](./type_defs.md#allowedinputtypestypedef) 
2. See [:material-code-braces: AudioAndDTMFInputSpecificationTypeDef](./type_defs.md#audioanddtmfinputspecificationtypedef) 
3. See [:material-code-braces: TextInputSpecificationTypeDef](./type_defs.md#textinputspecificationtypedef) 
## AudioLogSettingTypeDef

```python
# AudioLogSettingTypeDef definition

class AudioLogSettingTypeDef(TypedDict):
    enabled: bool,
    destination: AudioLogDestinationTypeDef,  # (1)
```

1. See [:material-code-braces: AudioLogDestinationTypeDef](./type_defs.md#audiologdestinationtypedef) 
## DescribeTestExecutionResponseTypeDef

```python
# DescribeTestExecutionResponseTypeDef definition

class DescribeTestExecutionResponseTypeDef(TypedDict):
    testExecutionId: str,
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    testExecutionStatus: TestExecutionStatusType,  # (1)
    testSetId: str,
    testSetName: str,
    target: TestExecutionTargetTypeDef,  # (2)
    apiMode: TestExecutionApiModeType,  # (3)
    testExecutionModality: TestExecutionModalityType,  # (4)
    failureReasons: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: TestExecutionStatusType](./literals.md#testexecutionstatustype) 
2. See [:material-code-braces: TestExecutionTargetTypeDef](./type_defs.md#testexecutiontargettypedef) 
3. See [:material-code-brackets: TestExecutionApiModeType](./literals.md#testexecutionapimodetype) 
4. See [:material-code-brackets: TestExecutionModalityType](./literals.md#testexecutionmodalitytype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTestExecutionRequestRequestTypeDef

```python
# StartTestExecutionRequestRequestTypeDef definition

class StartTestExecutionRequestRequestTypeDef(TypedDict):
    testSetId: str,
    target: TestExecutionTargetTypeDef,  # (1)
    apiMode: TestExecutionApiModeType,  # (2)
    testExecutionModality: NotRequired[TestExecutionModalityType],  # (3)
```

1. See [:material-code-braces: TestExecutionTargetTypeDef](./type_defs.md#testexecutiontargettypedef) 
2. See [:material-code-brackets: TestExecutionApiModeType](./literals.md#testexecutionapimodetype) 
3. See [:material-code-brackets: TestExecutionModalityType](./literals.md#testexecutionmodalitytype) 
## StartTestExecutionResponseTypeDef

```python
# StartTestExecutionResponseTypeDef definition

class StartTestExecutionResponseTypeDef(TypedDict):
    testExecutionId: str,
    creationDateTime: datetime,
    testSetId: str,
    target: TestExecutionTargetTypeDef,  # (1)
    apiMode: TestExecutionApiModeType,  # (2)
    testExecutionModality: TestExecutionModalityType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TestExecutionTargetTypeDef](./type_defs.md#testexecutiontargettypedef) 
2. See [:material-code-brackets: TestExecutionApiModeType](./literals.md#testexecutionapimodetype) 
3. See [:material-code-brackets: TestExecutionModalityType](./literals.md#testexecutionmodalitytype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestExecutionSummaryTypeDef

```python
# TestExecutionSummaryTypeDef definition

class TestExecutionSummaryTypeDef(TypedDict):
    testExecutionId: NotRequired[str],
    creationDateTime: NotRequired[datetime],
    lastUpdatedDateTime: NotRequired[datetime],
    testExecutionStatus: NotRequired[TestExecutionStatusType],  # (1)
    testSetId: NotRequired[str],
    testSetName: NotRequired[str],
    target: NotRequired[TestExecutionTargetTypeDef],  # (2)
    apiMode: NotRequired[TestExecutionApiModeType],  # (3)
    testExecutionModality: NotRequired[TestExecutionModalityType],  # (4)
```

1. See [:material-code-brackets: TestExecutionStatusType](./literals.md#testexecutionstatustype) 
2. See [:material-code-braces: TestExecutionTargetTypeDef](./type_defs.md#testexecutiontargettypedef) 
3. See [:material-code-brackets: TestExecutionApiModeType](./literals.md#testexecutionapimodetype) 
4. See [:material-code-brackets: TestExecutionModalityType](./literals.md#testexecutionmodalitytype) 
## BotRecommendationResultsTypeDef

```python
# BotRecommendationResultsTypeDef definition

class BotRecommendationResultsTypeDef(TypedDict):
    botLocaleExportUrl: NotRequired[str],
    associatedTranscriptsUrl: NotRequired[str],
    statistics: NotRequired[BotRecommendationResultStatisticsTypeDef],  # (1)
```

1. See [:material-code-braces: BotRecommendationResultStatisticsTypeDef](./type_defs.md#botrecommendationresultstatisticstypedef) 
## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    plainTextMessage: NotRequired[PlainTextMessageTypeDef],  # (1)
    customPayload: NotRequired[CustomPayloadTypeDef],  # (2)
    ssmlMessage: NotRequired[SSMLMessageTypeDef],  # (3)
    imageResponseCard: NotRequired[ImageResponseCardTypeDef],  # (4)
```

1. See [:material-code-braces: PlainTextMessageTypeDef](./type_defs.md#plaintextmessagetypedef) 
2. See [:material-code-braces: CustomPayloadTypeDef](./type_defs.md#custompayloadtypedef) 
3. See [:material-code-braces: SSMLMessageTypeDef](./type_defs.md#ssmlmessagetypedef) 
4. See [:material-code-braces: ImageResponseCardTypeDef](./type_defs.md#imageresponsecardtypedef) 
## UtteranceBotResponseTypeDef

```python
# UtteranceBotResponseTypeDef definition

class UtteranceBotResponseTypeDef(TypedDict):
    content: NotRequired[str],
    contentType: NotRequired[UtteranceContentTypeType],  # (1)
    imageResponseCard: NotRequired[ImageResponseCardTypeDef],  # (2)
```

1. See [:material-code-brackets: UtteranceContentTypeType](./literals.md#utterancecontenttypetype) 
2. See [:material-code-braces: ImageResponseCardTypeDef](./type_defs.md#imageresponsecardtypedef) 
## TextLogSettingTypeDef

```python
# TextLogSettingTypeDef definition

class TextLogSettingTypeDef(TypedDict):
    enabled: bool,
    destination: TextLogDestinationTypeDef,  # (1)
```

1. See [:material-code-braces: TextLogDestinationTypeDef](./type_defs.md#textlogdestinationtypedef) 
## BotAliasLocaleSettingsTypeDef

```python
# BotAliasLocaleSettingsTypeDef definition

class BotAliasLocaleSettingsTypeDef(TypedDict):
    enabled: bool,
    codeHookSpecification: NotRequired[CodeHookSpecificationTypeDef],  # (1)
```

1. See [:material-code-braces: CodeHookSpecificationTypeDef](./type_defs.md#codehookspecificationtypedef) 
## ConversationLevelTestResultsTypeDef

```python
# ConversationLevelTestResultsTypeDef definition

class ConversationLevelTestResultsTypeDef(TypedDict):
    items: List[ConversationLevelTestResultItemTypeDef],  # (1)
```

1. See [:material-code-braces: ConversationLevelTestResultItemTypeDef](./type_defs.md#conversationleveltestresultitemtypedef) 
## ListTestExecutionResultItemsRequestRequestTypeDef

```python
# ListTestExecutionResultItemsRequestRequestTypeDef definition

class ListTestExecutionResultItemsRequestRequestTypeDef(TypedDict):
    testExecutionId: str,
    resultFilterBy: TestExecutionResultFilterByTypeDef,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestExecutionResultFilterByTypeDef](./type_defs.md#testexecutionresultfilterbytypedef) 
## TestSetGenerationDataSourceTypeDef

```python
# TestSetGenerationDataSourceTypeDef definition

class TestSetGenerationDataSourceTypeDef(TypedDict):
    conversationLogsDataSource: NotRequired[ConversationLogsDataSourceTypeDef],  # (1)
```

1. See [:material-code-braces: ConversationLogsDataSourceTypeDef](./type_defs.md#conversationlogsdatasourcetypedef) 
## ListIntentsResponseTypeDef

```python
# ListIntentsResponseTypeDef definition

class ListIntentsResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    intentSummaries: List[IntentSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IntentSummaryTypeDef](./type_defs.md#intentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TranscriptFilterTypeDef

```python
# TranscriptFilterTypeDef definition

class TranscriptFilterTypeDef(TypedDict):
    lexTranscriptFilter: NotRequired[LexTranscriptFilterTypeDef],  # (1)
```

1. See [:material-code-braces: LexTranscriptFilterTypeDef](./type_defs.md#lextranscriptfiltertypedef) 
## ListTestSetsResponseTypeDef

```python
# ListTestSetsResponseTypeDef definition

class ListTestSetsResponseTypeDef(TypedDict):
    testSets: List[TestSetSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TestSetSummaryTypeDef](./type_defs.md#testsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExportRequestRequestTypeDef

```python
# CreateExportRequestRequestTypeDef definition

class CreateExportRequestRequestTypeDef(TypedDict):
    resourceSpecification: ExportResourceSpecificationTypeDef,  # (1)
    fileFormat: ImportExportFileFormatType,  # (2)
    filePassword: NotRequired[str],
```

1. See [:material-code-braces: ExportResourceSpecificationTypeDef](./type_defs.md#exportresourcespecificationtypedef) 
2. See [:material-code-brackets: ImportExportFileFormatType](./literals.md#importexportfileformattype) 
## CreateExportResponseTypeDef

```python
# CreateExportResponseTypeDef definition

class CreateExportResponseTypeDef(TypedDict):
    exportId: str,
    resourceSpecification: ExportResourceSpecificationTypeDef,  # (1)
    fileFormat: ImportExportFileFormatType,  # (2)
    exportStatus: ExportStatusType,  # (3)
    creationDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ExportResourceSpecificationTypeDef](./type_defs.md#exportresourcespecificationtypedef) 
2. See [:material-code-brackets: ImportExportFileFormatType](./literals.md#importexportfileformattype) 
3. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeExportResponseTypeDef

```python
# DescribeExportResponseTypeDef definition

class DescribeExportResponseTypeDef(TypedDict):
    exportId: str,
    resourceSpecification: ExportResourceSpecificationTypeDef,  # (1)
    fileFormat: ImportExportFileFormatType,  # (2)
    exportStatus: ExportStatusType,  # (3)
    failureReasons: List[str],
    downloadUrl: str,
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ExportResourceSpecificationTypeDef](./type_defs.md#exportresourcespecificationtypedef) 
2. See [:material-code-brackets: ImportExportFileFormatType](./literals.md#importexportfileformattype) 
3. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportSummaryTypeDef

```python
# ExportSummaryTypeDef definition

class ExportSummaryTypeDef(TypedDict):
    exportId: NotRequired[str],
    resourceSpecification: NotRequired[ExportResourceSpecificationTypeDef],  # (1)
    fileFormat: NotRequired[ImportExportFileFormatType],  # (2)
    exportStatus: NotRequired[ExportStatusType],  # (3)
    creationDateTime: NotRequired[datetime],
    lastUpdatedDateTime: NotRequired[datetime],
```

1. See [:material-code-braces: ExportResourceSpecificationTypeDef](./type_defs.md#exportresourcespecificationtypedef) 
2. See [:material-code-brackets: ImportExportFileFormatType](./literals.md#importexportfileformattype) 
3. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
## UpdateExportResponseTypeDef

```python
# UpdateExportResponseTypeDef definition

class UpdateExportResponseTypeDef(TypedDict):
    exportId: str,
    resourceSpecification: ExportResourceSpecificationTypeDef,  # (1)
    fileFormat: ImportExportFileFormatType,  # (2)
    exportStatus: ExportStatusType,  # (3)
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ExportResourceSpecificationTypeDef](./type_defs.md#exportresourcespecificationtypedef) 
2. See [:material-code-brackets: ImportExportFileFormatType](./literals.md#importexportfileformattype) 
3. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExternalSourceSettingTypeDef

```python
# ExternalSourceSettingTypeDef definition

class ExternalSourceSettingTypeDef(TypedDict):
    grammarSlotTypeSetting: NotRequired[GrammarSlotTypeSettingTypeDef],  # (1)
```

1. See [:material-code-braces: GrammarSlotTypeSettingTypeDef](./type_defs.md#grammarslottypesettingtypedef) 
## IntentClassificationTestResultsTypeDef

```python
# IntentClassificationTestResultsTypeDef definition

class IntentClassificationTestResultsTypeDef(TypedDict):
    items: List[IntentClassificationTestResultItemTypeDef],  # (1)
```

1. See [:material-code-braces: IntentClassificationTestResultItemTypeDef](./type_defs.md#intentclassificationtestresultitemtypedef) 
## ListSessionAnalyticsDataResponseTypeDef

```python
# ListSessionAnalyticsDataResponseTypeDef definition

class ListSessionAnalyticsDataResponseTypeDef(TypedDict):
    botId: str,
    nextToken: str,
    sessions: List[SessionSpecificationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionSpecificationTypeDef](./type_defs.md#sessionspecificationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAggregatedUtterancesRequestRequestTypeDef

```python
# ListAggregatedUtterancesRequestRequestTypeDef definition

class ListAggregatedUtterancesRequestRequestTypeDef(TypedDict):
    botId: str,
    localeId: str,
    aggregationDuration: UtteranceAggregationDurationTypeDef,  # (1)
    botAliasId: NotRequired[str],
    botVersion: NotRequired[str],
    sortBy: NotRequired[AggregatedUtterancesSortByTypeDef],  # (2)
    filters: NotRequired[Sequence[AggregatedUtterancesFilterTypeDef]],  # (3)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: UtteranceAggregationDurationTypeDef](./type_defs.md#utteranceaggregationdurationtypedef) 
2. See [:material-code-braces: AggregatedUtterancesSortByTypeDef](./type_defs.md#aggregatedutterancessortbytypedef) 
3. See [:material-code-braces: AggregatedUtterancesFilterTypeDef](./type_defs.md#aggregatedutterancesfiltertypedef) 
## ListAggregatedUtterancesResponseTypeDef

```python
# ListAggregatedUtterancesResponseTypeDef definition

class ListAggregatedUtterancesResponseTypeDef(TypedDict):
    botId: str,
    botAliasId: str,
    botVersion: str,
    localeId: str,
    aggregationDuration: UtteranceAggregationDurationTypeDef,  # (1)
    aggregationWindowStartTime: datetime,
    aggregationWindowEndTime: datetime,
    aggregationLastRefreshedDateTime: datetime,
    aggregatedUtterancesSummaries: List[AggregatedUtterancesSummaryTypeDef],  # (2)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: UtteranceAggregationDurationTypeDef](./type_defs.md#utteranceaggregationdurationtypedef) 
2. See [:material-code-braces: AggregatedUtterancesSummaryTypeDef](./type_defs.md#aggregatedutterancessummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntentLevelSlotResolutionTestResultItemTypeDef

```python
# IntentLevelSlotResolutionTestResultItemTypeDef definition

class IntentLevelSlotResolutionTestResultItemTypeDef(TypedDict):
    intentName: str,
    multiTurnConversation: bool,
    slotResolutionResults: List[SlotResolutionTestResultItemTypeDef],  # (1)
```

1. See [:material-code-braces: SlotResolutionTestResultItemTypeDef](./type_defs.md#slotresolutiontestresultitemtypedef) 
## CreateTestSetDiscrepancyReportRequestRequestTypeDef

```python
# CreateTestSetDiscrepancyReportRequestRequestTypeDef definition

class CreateTestSetDiscrepancyReportRequestRequestTypeDef(TypedDict):
    testSetId: str,
    target: TestSetDiscrepancyReportResourceTargetTypeDef,  # (1)
```

1. See [:material-code-braces: TestSetDiscrepancyReportResourceTargetTypeDef](./type_defs.md#testsetdiscrepancyreportresourcetargettypedef) 
## CreateTestSetDiscrepancyReportResponseTypeDef

```python
# CreateTestSetDiscrepancyReportResponseTypeDef definition

class CreateTestSetDiscrepancyReportResponseTypeDef(TypedDict):
    testSetDiscrepancyReportId: str,
    creationDateTime: datetime,
    testSetId: str,
    target: TestSetDiscrepancyReportResourceTargetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TestSetDiscrepancyReportResourceTargetTypeDef](./type_defs.md#testsetdiscrepancyreportresourcetargettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTestSetDiscrepancyReportResponseTypeDef

```python
# DescribeTestSetDiscrepancyReportResponseTypeDef definition

class DescribeTestSetDiscrepancyReportResponseTypeDef(TypedDict):
    testSetDiscrepancyReportId: str,
    testSetId: str,
    creationDateTime: datetime,
    target: TestSetDiscrepancyReportResourceTargetTypeDef,  # (1)
    testSetDiscrepancyReportStatus: TestSetDiscrepancyReportStatusType,  # (2)
    lastUpdatedDataTime: datetime,
    testSetDiscrepancyTopErrors: TestSetDiscrepancyErrorsTypeDef,  # (3)
    testSetDiscrepancyRawOutputUrl: str,
    failureReasons: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TestSetDiscrepancyReportResourceTargetTypeDef](./type_defs.md#testsetdiscrepancyreportresourcetargettypedef) 
2. See [:material-code-brackets: TestSetDiscrepancyReportStatusType](./literals.md#testsetdiscrepancyreportstatustype) 
3. See [:material-code-braces: TestSetDiscrepancyErrorsTypeDef](./type_defs.md#testsetdiscrepancyerrorstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportResourceSpecificationTypeDef

```python
# ImportResourceSpecificationTypeDef definition

class ImportResourceSpecificationTypeDef(TypedDict):
    botImportSpecification: NotRequired[BotImportSpecificationTypeDef],  # (1)
    botLocaleImportSpecification: NotRequired[BotLocaleImportSpecificationTypeDef],  # (2)
    customVocabularyImportSpecification: NotRequired[CustomVocabularyImportSpecificationTypeDef],  # (3)
    testSetImportResourceSpecification: NotRequired[TestSetImportResourceSpecificationTypeDef],  # (4)
```

1. See [:material-code-braces: BotImportSpecificationTypeDef](./type_defs.md#botimportspecificationtypedef) 
2. See [:material-code-braces: BotLocaleImportSpecificationTypeDef](./type_defs.md#botlocaleimportspecificationtypedef) 
3. See [:material-code-braces: CustomVocabularyImportSpecificationTypeDef](./type_defs.md#customvocabularyimportspecificationtypedef) 
4. See [:material-code-braces: TestSetImportResourceSpecificationTypeDef](./type_defs.md#testsetimportresourcespecificationtypedef) 
## UserTurnInputSpecificationTypeDef

```python
# UserTurnInputSpecificationTypeDef definition

class UserTurnInputSpecificationTypeDef(TypedDict):
    utteranceInput: UtteranceInputSpecificationTypeDef,  # (1)
    requestAttributes: NotRequired[Dict[str, str]],
    sessionState: NotRequired[InputSessionStateSpecificationTypeDef],  # (2)
```

1. See [:material-code-braces: UtteranceInputSpecificationTypeDef](./type_defs.md#utteranceinputspecificationtypedef) 
2. See [:material-code-braces: InputSessionStateSpecificationTypeDef](./type_defs.md#inputsessionstatespecificationtypedef) 
## ListTestExecutionsResponseTypeDef

```python
# ListTestExecutionsResponseTypeDef definition

class ListTestExecutionsResponseTypeDef(TypedDict):
    testExecutions: List[TestExecutionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TestExecutionSummaryTypeDef](./type_defs.md#testexecutionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MessageGroupTypeDef

```python
# MessageGroupTypeDef definition

class MessageGroupTypeDef(TypedDict):
    message: MessageTypeDef,  # (1)
    variations: NotRequired[Sequence[MessageTypeDef]],  # (2)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
## UtteranceSpecificationTypeDef

```python
# UtteranceSpecificationTypeDef definition

class UtteranceSpecificationTypeDef(TypedDict):
    botAliasId: NotRequired[str],
    botVersion: NotRequired[str],
    localeId: NotRequired[str],
    sessionId: NotRequired[str],
    channel: NotRequired[str],
    mode: NotRequired[AnalyticsModalityType],  # (1)
    conversationStartTime: NotRequired[datetime],
    conversationEndTime: NotRequired[datetime],
    utterance: NotRequired[str],
    utteranceTimestamp: NotRequired[datetime],
    audioVoiceDurationMillis: NotRequired[int],
    utteranceUnderstood: NotRequired[bool],
    inputType: NotRequired[str],
    outputType: NotRequired[str],
    associatedIntentName: NotRequired[str],
    associatedSlotName: NotRequired[str],
    intentState: NotRequired[IntentStateType],  # (2)
    dialogActionType: NotRequired[str],
    botResponseAudioVoiceId: NotRequired[str],
    slotsFilledInSession: NotRequired[str],
    utteranceRequestId: NotRequired[str],
    botResponses: NotRequired[List[UtteranceBotResponseTypeDef]],  # (3)
```

1. See [:material-code-brackets: AnalyticsModalityType](./literals.md#analyticsmodalitytype) 
2. See [:material-code-brackets: IntentStateType](./literals.md#intentstatetype) 
3. See [:material-code-braces: UtteranceBotResponseTypeDef](./type_defs.md#utterancebotresponsetypedef) 
## ConversationLogSettingsTypeDef

```python
# ConversationLogSettingsTypeDef definition

class ConversationLogSettingsTypeDef(TypedDict):
    textLogSettings: NotRequired[Sequence[TextLogSettingTypeDef]],  # (1)
    audioLogSettings: NotRequired[Sequence[AudioLogSettingTypeDef]],  # (2)
```

1. See [:material-code-braces: TextLogSettingTypeDef](./type_defs.md#textlogsettingtypedef) 
2. See [:material-code-braces: AudioLogSettingTypeDef](./type_defs.md#audiologsettingtypedef) 
## DescribeTestSetGenerationResponseTypeDef

```python
# DescribeTestSetGenerationResponseTypeDef definition

class DescribeTestSetGenerationResponseTypeDef(TypedDict):
    testSetGenerationId: str,
    testSetGenerationStatus: TestSetGenerationStatusType,  # (1)
    failureReasons: List[str],
    testSetId: str,
    testSetName: str,
    description: str,
    storageLocation: TestSetStorageLocationTypeDef,  # (2)
    generationDataSource: TestSetGenerationDataSourceTypeDef,  # (3)
    roleArn: str,
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: TestSetGenerationStatusType](./literals.md#testsetgenerationstatustype) 
2. See [:material-code-braces: TestSetStorageLocationTypeDef](./type_defs.md#testsetstoragelocationtypedef) 
3. See [:material-code-braces: TestSetGenerationDataSourceTypeDef](./type_defs.md#testsetgenerationdatasourcetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTestSetGenerationRequestRequestTypeDef

```python
# StartTestSetGenerationRequestRequestTypeDef definition

class StartTestSetGenerationRequestRequestTypeDef(TypedDict):
    testSetName: str,
    storageLocation: TestSetStorageLocationTypeDef,  # (1)
    generationDataSource: TestSetGenerationDataSourceTypeDef,  # (2)
    roleArn: str,
    description: NotRequired[str],
    testSetTags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: TestSetStorageLocationTypeDef](./type_defs.md#testsetstoragelocationtypedef) 
2. See [:material-code-braces: TestSetGenerationDataSourceTypeDef](./type_defs.md#testsetgenerationdatasourcetypedef) 
## StartTestSetGenerationResponseTypeDef

```python
# StartTestSetGenerationResponseTypeDef definition

class StartTestSetGenerationResponseTypeDef(TypedDict):
    testSetGenerationId: str,
    creationDateTime: datetime,
    testSetGenerationStatus: TestSetGenerationStatusType,  # (1)
    testSetName: str,
    description: str,
    storageLocation: TestSetStorageLocationTypeDef,  # (2)
    generationDataSource: TestSetGenerationDataSourceTypeDef,  # (3)
    roleArn: str,
    testSetTags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: TestSetGenerationStatusType](./literals.md#testsetgenerationstatustype) 
2. See [:material-code-braces: TestSetStorageLocationTypeDef](./type_defs.md#testsetstoragelocationtypedef) 
3. See [:material-code-braces: TestSetGenerationDataSourceTypeDef](./type_defs.md#testsetgenerationdatasourcetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## S3BucketTranscriptSourceTypeDef

```python
# S3BucketTranscriptSourceTypeDef definition

class S3BucketTranscriptSourceTypeDef(TypedDict):
    s3BucketName: str,
    transcriptFormat: TranscriptFormatType,  # (2)
    pathFormat: NotRequired[PathFormatTypeDef],  # (1)
    transcriptFilter: NotRequired[TranscriptFilterTypeDef],  # (3)
    kmsKeyArn: NotRequired[str],
```

1. See [:material-code-braces: PathFormatTypeDef](./type_defs.md#pathformattypedef) 
2. See [:material-code-brackets: TranscriptFormatType](./literals.md#transcriptformattype) 
3. See [:material-code-braces: TranscriptFilterTypeDef](./type_defs.md#transcriptfiltertypedef) 
## ListExportsResponseTypeDef

```python
# ListExportsResponseTypeDef definition

class ListExportsResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    exportSummaries: List[ExportSummaryTypeDef],  # (1)
    nextToken: str,
    localeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportSummaryTypeDef](./type_defs.md#exportsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSlotTypeRequestRequestTypeDef

```python
# CreateSlotTypeRequestRequestTypeDef definition

class CreateSlotTypeRequestRequestTypeDef(TypedDict):
    slotTypeName: str,
    botId: str,
    botVersion: str,
    localeId: str,
    description: NotRequired[str],
    slotTypeValues: NotRequired[Sequence[SlotTypeValueTypeDef]],  # (1)
    valueSelectionSetting: NotRequired[SlotValueSelectionSettingTypeDef],  # (2)
    parentSlotTypeSignature: NotRequired[str],
    externalSourceSetting: NotRequired[ExternalSourceSettingTypeDef],  # (3)
    compositeSlotTypeSetting: NotRequired[CompositeSlotTypeSettingTypeDef],  # (4)
```

1. See [:material-code-braces: SlotTypeValueTypeDef](./type_defs.md#slottypevaluetypedef) 
2. See [:material-code-braces: SlotValueSelectionSettingTypeDef](./type_defs.md#slotvalueselectionsettingtypedef) 
3. See [:material-code-braces: ExternalSourceSettingTypeDef](./type_defs.md#externalsourcesettingtypedef) 
4. See [:material-code-braces: CompositeSlotTypeSettingTypeDef](./type_defs.md#compositeslottypesettingtypedef) 
## CreateSlotTypeResponseTypeDef

```python
# CreateSlotTypeResponseTypeDef definition

class CreateSlotTypeResponseTypeDef(TypedDict):
    slotTypeId: str,
    slotTypeName: str,
    description: str,
    slotTypeValues: List[SlotTypeValueTypeDef],  # (1)
    valueSelectionSetting: SlotValueSelectionSettingTypeDef,  # (2)
    parentSlotTypeSignature: str,
    botId: str,
    botVersion: str,
    localeId: str,
    creationDateTime: datetime,
    externalSourceSetting: ExternalSourceSettingTypeDef,  # (3)
    compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SlotTypeValueTypeDef](./type_defs.md#slottypevaluetypedef) 
2. See [:material-code-braces: SlotValueSelectionSettingTypeDef](./type_defs.md#slotvalueselectionsettingtypedef) 
3. See [:material-code-braces: ExternalSourceSettingTypeDef](./type_defs.md#externalsourcesettingtypedef) 
4. See [:material-code-braces: CompositeSlotTypeSettingTypeDef](./type_defs.md#compositeslottypesettingtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSlotTypeResponseTypeDef

```python
# DescribeSlotTypeResponseTypeDef definition

class DescribeSlotTypeResponseTypeDef(TypedDict):
    slotTypeId: str,
    slotTypeName: str,
    description: str,
    slotTypeValues: List[SlotTypeValueTypeDef],  # (1)
    valueSelectionSetting: SlotValueSelectionSettingTypeDef,  # (2)
    parentSlotTypeSignature: str,
    botId: str,
    botVersion: str,
    localeId: str,
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    externalSourceSetting: ExternalSourceSettingTypeDef,  # (3)
    compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SlotTypeValueTypeDef](./type_defs.md#slottypevaluetypedef) 
2. See [:material-code-braces: SlotValueSelectionSettingTypeDef](./type_defs.md#slotvalueselectionsettingtypedef) 
3. See [:material-code-braces: ExternalSourceSettingTypeDef](./type_defs.md#externalsourcesettingtypedef) 
4. See [:material-code-braces: CompositeSlotTypeSettingTypeDef](./type_defs.md#compositeslottypesettingtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSlotTypeRequestRequestTypeDef

```python
# UpdateSlotTypeRequestRequestTypeDef definition

class UpdateSlotTypeRequestRequestTypeDef(TypedDict):
    slotTypeId: str,
    slotTypeName: str,
    botId: str,
    botVersion: str,
    localeId: str,
    description: NotRequired[str],
    slotTypeValues: NotRequired[Sequence[SlotTypeValueTypeDef]],  # (1)
    valueSelectionSetting: NotRequired[SlotValueSelectionSettingTypeDef],  # (2)
    parentSlotTypeSignature: NotRequired[str],
    externalSourceSetting: NotRequired[ExternalSourceSettingTypeDef],  # (3)
    compositeSlotTypeSetting: NotRequired[CompositeSlotTypeSettingTypeDef],  # (4)
```

1. See [:material-code-braces: SlotTypeValueTypeDef](./type_defs.md#slottypevaluetypedef) 
2. See [:material-code-braces: SlotValueSelectionSettingTypeDef](./type_defs.md#slotvalueselectionsettingtypedef) 
3. See [:material-code-braces: ExternalSourceSettingTypeDef](./type_defs.md#externalsourcesettingtypedef) 
4. See [:material-code-braces: CompositeSlotTypeSettingTypeDef](./type_defs.md#compositeslottypesettingtypedef) 
## UpdateSlotTypeResponseTypeDef

```python
# UpdateSlotTypeResponseTypeDef definition

class UpdateSlotTypeResponseTypeDef(TypedDict):
    slotTypeId: str,
    slotTypeName: str,
    description: str,
    slotTypeValues: List[SlotTypeValueTypeDef],  # (1)
    valueSelectionSetting: SlotValueSelectionSettingTypeDef,  # (2)
    parentSlotTypeSignature: str,
    botId: str,
    botVersion: str,
    localeId: str,
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    externalSourceSetting: ExternalSourceSettingTypeDef,  # (3)
    compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SlotTypeValueTypeDef](./type_defs.md#slottypevaluetypedef) 
2. See [:material-code-braces: SlotValueSelectionSettingTypeDef](./type_defs.md#slotvalueselectionsettingtypedef) 
3. See [:material-code-braces: ExternalSourceSettingTypeDef](./type_defs.md#externalsourcesettingtypedef) 
4. See [:material-code-braces: CompositeSlotTypeSettingTypeDef](./type_defs.md#compositeslottypesettingtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntentLevelSlotResolutionTestResultsTypeDef

```python
# IntentLevelSlotResolutionTestResultsTypeDef definition

class IntentLevelSlotResolutionTestResultsTypeDef(TypedDict):
    items: List[IntentLevelSlotResolutionTestResultItemTypeDef],  # (1)
```

1. See [:material-code-braces: IntentLevelSlotResolutionTestResultItemTypeDef](./type_defs.md#intentlevelslotresolutiontestresultitemtypedef) 
## DescribeImportResponseTypeDef

```python
# DescribeImportResponseTypeDef definition

class DescribeImportResponseTypeDef(TypedDict):
    importId: str,
    resourceSpecification: ImportResourceSpecificationTypeDef,  # (1)
    importedResourceId: str,
    importedResourceName: str,
    mergeStrategy: MergeStrategyType,  # (2)
    importStatus: ImportStatusType,  # (3)
    failureReasons: List[str],
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ImportResourceSpecificationTypeDef](./type_defs.md#importresourcespecificationtypedef) 
2. See [:material-code-brackets: MergeStrategyType](./literals.md#mergestrategytype) 
3. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartImportRequestRequestTypeDef

```python
# StartImportRequestRequestTypeDef definition

class StartImportRequestRequestTypeDef(TypedDict):
    importId: str,
    resourceSpecification: ImportResourceSpecificationTypeDef,  # (1)
    mergeStrategy: MergeStrategyType,  # (2)
    filePassword: NotRequired[str],
```

1. See [:material-code-braces: ImportResourceSpecificationTypeDef](./type_defs.md#importresourcespecificationtypedef) 
2. See [:material-code-brackets: MergeStrategyType](./literals.md#mergestrategytype) 
## StartImportResponseTypeDef

```python
# StartImportResponseTypeDef definition

class StartImportResponseTypeDef(TypedDict):
    importId: str,
    resourceSpecification: ImportResourceSpecificationTypeDef,  # (1)
    mergeStrategy: MergeStrategyType,  # (2)
    importStatus: ImportStatusType,  # (3)
    creationDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ImportResourceSpecificationTypeDef](./type_defs.md#importresourcespecificationtypedef) 
2. See [:material-code-brackets: MergeStrategyType](./literals.md#mergestrategytype) 
3. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UserTurnResultTypeDef

```python
# UserTurnResultTypeDef definition

class UserTurnResultTypeDef(TypedDict):
    input: UserTurnInputSpecificationTypeDef,  # (1)
    expectedOutput: UserTurnOutputSpecificationTypeDef,  # (2)
    actualOutput: NotRequired[UserTurnOutputSpecificationTypeDef],  # (2)
    errorDetails: NotRequired[ExecutionErrorDetailsTypeDef],  # (4)
    endToEndResult: NotRequired[TestResultMatchStatusType],  # (5)
    intentMatchResult: NotRequired[TestResultMatchStatusType],  # (5)
    slotMatchResult: NotRequired[TestResultMatchStatusType],  # (5)
    speechTranscriptionResult: NotRequired[TestResultMatchStatusType],  # (5)
    conversationLevelResult: NotRequired[ConversationLevelResultDetailTypeDef],  # (9)
```

1. See [:material-code-braces: UserTurnInputSpecificationTypeDef](./type_defs.md#userturninputspecificationtypedef) 
2. See [:material-code-braces: UserTurnOutputSpecificationTypeDef](./type_defs.md#userturnoutputspecificationtypedef) 
3. See [:material-code-braces: UserTurnOutputSpecificationTypeDef](./type_defs.md#userturnoutputspecificationtypedef) 
4. See [:material-code-braces: ExecutionErrorDetailsTypeDef](./type_defs.md#executionerrordetailstypedef) 
5. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
6. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
7. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
8. See [:material-code-brackets: TestResultMatchStatusType](./literals.md#testresultmatchstatustype) 
9. See [:material-code-braces: ConversationLevelResultDetailTypeDef](./type_defs.md#conversationlevelresultdetailtypedef) 
## UserTurnSpecificationTypeDef

```python
# UserTurnSpecificationTypeDef definition

class UserTurnSpecificationTypeDef(TypedDict):
    input: UserTurnInputSpecificationTypeDef,  # (1)
    expected: UserTurnOutputSpecificationTypeDef,  # (2)
```

1. See [:material-code-braces: UserTurnInputSpecificationTypeDef](./type_defs.md#userturninputspecificationtypedef) 
2. See [:material-code-braces: UserTurnOutputSpecificationTypeDef](./type_defs.md#userturnoutputspecificationtypedef) 
## FulfillmentStartResponseSpecificationTypeDef

```python
# FulfillmentStartResponseSpecificationTypeDef definition

class FulfillmentStartResponseSpecificationTypeDef(TypedDict):
    delayInSeconds: int,
    messageGroups: Sequence[MessageGroupTypeDef],  # (1)
    allowInterrupt: NotRequired[bool],
```

1. See [:material-code-braces: MessageGroupTypeDef](./type_defs.md#messagegrouptypedef) 
## FulfillmentUpdateResponseSpecificationTypeDef

```python
# FulfillmentUpdateResponseSpecificationTypeDef definition

class FulfillmentUpdateResponseSpecificationTypeDef(TypedDict):
    frequencyInSeconds: int,
    messageGroups: Sequence[MessageGroupTypeDef],  # (1)
    allowInterrupt: NotRequired[bool],
```

1. See [:material-code-braces: MessageGroupTypeDef](./type_defs.md#messagegrouptypedef) 
## PromptSpecificationTypeDef

```python
# PromptSpecificationTypeDef definition

class PromptSpecificationTypeDef(TypedDict):
    messageGroups: Sequence[MessageGroupTypeDef],  # (1)
    maxRetries: int,
    allowInterrupt: NotRequired[bool],
    messageSelectionStrategy: NotRequired[MessageSelectionStrategyType],  # (2)
    promptAttemptsSpecification: NotRequired[Mapping[PromptAttemptType, PromptAttemptSpecificationTypeDef]],  # (3)
```

1. See [:material-code-braces: MessageGroupTypeDef](./type_defs.md#messagegrouptypedef) 
2. See [:material-code-brackets: MessageSelectionStrategyType](./literals.md#messageselectionstrategytype) 
3. See [:material-code-brackets: PromptAttemptType](./literals.md#promptattempttype) [:material-code-braces: PromptAttemptSpecificationTypeDef](./type_defs.md#promptattemptspecificationtypedef) 
## ResponseSpecificationTypeDef

```python
# ResponseSpecificationTypeDef definition

class ResponseSpecificationTypeDef(TypedDict):
    messageGroups: Sequence[MessageGroupTypeDef],  # (1)
    allowInterrupt: NotRequired[bool],
```

1. See [:material-code-braces: MessageGroupTypeDef](./type_defs.md#messagegrouptypedef) 
## StillWaitingResponseSpecificationTypeDef

```python
# StillWaitingResponseSpecificationTypeDef definition

class StillWaitingResponseSpecificationTypeDef(TypedDict):
    messageGroups: Sequence[MessageGroupTypeDef],  # (1)
    frequencyInSeconds: int,
    timeoutInSeconds: int,
    allowInterrupt: NotRequired[bool],
```

1. See [:material-code-braces: MessageGroupTypeDef](./type_defs.md#messagegrouptypedef) 
## ListUtteranceAnalyticsDataResponseTypeDef

```python
# ListUtteranceAnalyticsDataResponseTypeDef definition

class ListUtteranceAnalyticsDataResponseTypeDef(TypedDict):
    botId: str,
    nextToken: str,
    utterances: List[UtteranceSpecificationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UtteranceSpecificationTypeDef](./type_defs.md#utterancespecificationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBotAliasRequestRequestTypeDef

```python
# CreateBotAliasRequestRequestTypeDef definition

class CreateBotAliasRequestRequestTypeDef(TypedDict):
    botAliasName: str,
    botId: str,
    description: NotRequired[str],
    botVersion: NotRequired[str],
    botAliasLocaleSettings: NotRequired[Mapping[str, BotAliasLocaleSettingsTypeDef]],  # (1)
    conversationLogSettings: NotRequired[ConversationLogSettingsTypeDef],  # (2)
    sentimentAnalysisSettings: NotRequired[SentimentAnalysisSettingsTypeDef],  # (3)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: BotAliasLocaleSettingsTypeDef](./type_defs.md#botaliaslocalesettingstypedef) 
2. See [:material-code-braces: ConversationLogSettingsTypeDef](./type_defs.md#conversationlogsettingstypedef) 
3. See [:material-code-braces: SentimentAnalysisSettingsTypeDef](./type_defs.md#sentimentanalysissettingstypedef) 
## CreateBotAliasResponseTypeDef

```python
# CreateBotAliasResponseTypeDef definition

class CreateBotAliasResponseTypeDef(TypedDict):
    botAliasId: str,
    botAliasName: str,
    description: str,
    botVersion: str,
    botAliasLocaleSettings: Dict[str, BotAliasLocaleSettingsTypeDef],  # (1)
    conversationLogSettings: ConversationLogSettingsTypeDef,  # (2)
    sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef,  # (3)
    botAliasStatus: BotAliasStatusType,  # (4)
    botId: str,
    creationDateTime: datetime,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: BotAliasLocaleSettingsTypeDef](./type_defs.md#botaliaslocalesettingstypedef) 
2. See [:material-code-braces: ConversationLogSettingsTypeDef](./type_defs.md#conversationlogsettingstypedef) 
3. See [:material-code-braces: SentimentAnalysisSettingsTypeDef](./type_defs.md#sentimentanalysissettingstypedef) 
4. See [:material-code-brackets: BotAliasStatusType](./literals.md#botaliasstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBotAliasResponseTypeDef

```python
# DescribeBotAliasResponseTypeDef definition

class DescribeBotAliasResponseTypeDef(TypedDict):
    botAliasId: str,
    botAliasName: str,
    description: str,
    botVersion: str,
    botAliasLocaleSettings: Dict[str, BotAliasLocaleSettingsTypeDef],  # (1)
    conversationLogSettings: ConversationLogSettingsTypeDef,  # (2)
    sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef,  # (3)
    botAliasHistoryEvents: List[BotAliasHistoryEventTypeDef],  # (4)
    botAliasStatus: BotAliasStatusType,  # (5)
    botId: str,
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    parentBotNetworks: List[ParentBotNetworkTypeDef],  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: BotAliasLocaleSettingsTypeDef](./type_defs.md#botaliaslocalesettingstypedef) 
2. See [:material-code-braces: ConversationLogSettingsTypeDef](./type_defs.md#conversationlogsettingstypedef) 
3. See [:material-code-braces: SentimentAnalysisSettingsTypeDef](./type_defs.md#sentimentanalysissettingstypedef) 
4. See [:material-code-braces: BotAliasHistoryEventTypeDef](./type_defs.md#botaliashistoryeventtypedef) 
5. See [:material-code-brackets: BotAliasStatusType](./literals.md#botaliasstatustype) 
6. See [:material-code-braces: ParentBotNetworkTypeDef](./type_defs.md#parentbotnetworktypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBotAliasRequestRequestTypeDef

```python
# UpdateBotAliasRequestRequestTypeDef definition

class UpdateBotAliasRequestRequestTypeDef(TypedDict):
    botAliasId: str,
    botAliasName: str,
    botId: str,
    description: NotRequired[str],
    botVersion: NotRequired[str],
    botAliasLocaleSettings: NotRequired[Mapping[str, BotAliasLocaleSettingsTypeDef]],  # (1)
    conversationLogSettings: NotRequired[ConversationLogSettingsTypeDef],  # (2)
    sentimentAnalysisSettings: NotRequired[SentimentAnalysisSettingsTypeDef],  # (3)
```

1. See [:material-code-braces: BotAliasLocaleSettingsTypeDef](./type_defs.md#botaliaslocalesettingstypedef) 
2. See [:material-code-braces: ConversationLogSettingsTypeDef](./type_defs.md#conversationlogsettingstypedef) 
3. See [:material-code-braces: SentimentAnalysisSettingsTypeDef](./type_defs.md#sentimentanalysissettingstypedef) 
## UpdateBotAliasResponseTypeDef

```python
# UpdateBotAliasResponseTypeDef definition

class UpdateBotAliasResponseTypeDef(TypedDict):
    botAliasId: str,
    botAliasName: str,
    description: str,
    botVersion: str,
    botAliasLocaleSettings: Dict[str, BotAliasLocaleSettingsTypeDef],  # (1)
    conversationLogSettings: ConversationLogSettingsTypeDef,  # (2)
    sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef,  # (3)
    botAliasStatus: BotAliasStatusType,  # (4)
    botId: str,
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: BotAliasLocaleSettingsTypeDef](./type_defs.md#botaliaslocalesettingstypedef) 
2. See [:material-code-braces: ConversationLogSettingsTypeDef](./type_defs.md#conversationlogsettingstypedef) 
3. See [:material-code-braces: SentimentAnalysisSettingsTypeDef](./type_defs.md#sentimentanalysissettingstypedef) 
4. See [:material-code-brackets: BotAliasStatusType](./literals.md#botaliasstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TranscriptSourceSettingTypeDef

```python
# TranscriptSourceSettingTypeDef definition

class TranscriptSourceSettingTypeDef(TypedDict):
    s3BucketTranscriptSource: NotRequired[S3BucketTranscriptSourceTypeDef],  # (1)
```

1. See [:material-code-braces: S3BucketTranscriptSourceTypeDef](./type_defs.md#s3buckettranscriptsourcetypedef) 
## TestSetTurnResultTypeDef

```python
# TestSetTurnResultTypeDef definition

class TestSetTurnResultTypeDef(TypedDict):
    agent: NotRequired[AgentTurnResultTypeDef],  # (1)
    user: NotRequired[UserTurnResultTypeDef],  # (2)
```

1. See [:material-code-braces: AgentTurnResultTypeDef](./type_defs.md#agentturnresulttypedef) 
2. See [:material-code-braces: UserTurnResultTypeDef](./type_defs.md#userturnresulttypedef) 
## TurnSpecificationTypeDef

```python
# TurnSpecificationTypeDef definition

class TurnSpecificationTypeDef(TypedDict):
    agentTurn: NotRequired[AgentTurnSpecificationTypeDef],  # (1)
    userTurn: NotRequired[UserTurnSpecificationTypeDef],  # (2)
```

1. See [:material-code-braces: AgentTurnSpecificationTypeDef](./type_defs.md#agentturnspecificationtypedef) 
2. See [:material-code-braces: UserTurnSpecificationTypeDef](./type_defs.md#userturnspecificationtypedef) 
## FulfillmentUpdatesSpecificationTypeDef

```python
# FulfillmentUpdatesSpecificationTypeDef definition

class FulfillmentUpdatesSpecificationTypeDef(TypedDict):
    active: bool,
    startResponse: NotRequired[FulfillmentStartResponseSpecificationTypeDef],  # (1)
    updateResponse: NotRequired[FulfillmentUpdateResponseSpecificationTypeDef],  # (2)
    timeoutInSeconds: NotRequired[int],
```

1. See [:material-code-braces: FulfillmentStartResponseSpecificationTypeDef](./type_defs.md#fulfillmentstartresponsespecificationtypedef) 
2. See [:material-code-braces: FulfillmentUpdateResponseSpecificationTypeDef](./type_defs.md#fulfillmentupdateresponsespecificationtypedef) 
## SlotSummaryTypeDef

```python
# SlotSummaryTypeDef definition

class SlotSummaryTypeDef(TypedDict):
    slotId: NotRequired[str],
    slotName: NotRequired[str],
    description: NotRequired[str],
    slotConstraint: NotRequired[SlotConstraintType],  # (1)
    slotTypeId: NotRequired[str],
    valueElicitationPromptSpecification: NotRequired[PromptSpecificationTypeDef],  # (2)
    lastUpdatedDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: SlotConstraintType](./literals.md#slotconstrainttype) 
2. See [:material-code-braces: PromptSpecificationTypeDef](./type_defs.md#promptspecificationtypedef) 
## ConditionalBranchTypeDef

```python
# ConditionalBranchTypeDef definition

class ConditionalBranchTypeDef(TypedDict):
    name: str,
    condition: ConditionTypeDef,  # (1)
    nextStep: DialogStateTypeDef,  # (2)
    response: NotRequired[ResponseSpecificationTypeDef],  # (3)
```

1. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
2. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
3. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
## DefaultConditionalBranchTypeDef

```python
# DefaultConditionalBranchTypeDef definition

class DefaultConditionalBranchTypeDef(TypedDict):
    nextStep: NotRequired[DialogStateTypeDef],  # (1)
    response: NotRequired[ResponseSpecificationTypeDef],  # (2)
```

1. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
2. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
## WaitAndContinueSpecificationTypeDef

```python
# WaitAndContinueSpecificationTypeDef definition

class WaitAndContinueSpecificationTypeDef(TypedDict):
    waitingResponse: ResponseSpecificationTypeDef,  # (1)
    continueResponse: ResponseSpecificationTypeDef,  # (1)
    stillWaitingResponse: NotRequired[StillWaitingResponseSpecificationTypeDef],  # (3)
    active: NotRequired[bool],
```

1. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
2. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
3. See [:material-code-braces: StillWaitingResponseSpecificationTypeDef](./type_defs.md#stillwaitingresponsespecificationtypedef) 
## DescribeBotRecommendationResponseTypeDef

```python
# DescribeBotRecommendationResponseTypeDef definition

class DescribeBotRecommendationResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationStatus: BotRecommendationStatusType,  # (1)
    botRecommendationId: str,
    failureReasons: List[str],
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    transcriptSourceSetting: TranscriptSourceSettingTypeDef,  # (2)
    encryptionSetting: EncryptionSettingTypeDef,  # (3)
    botRecommendationResults: BotRecommendationResultsTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: BotRecommendationStatusType](./literals.md#botrecommendationstatustype) 
2. See [:material-code-braces: TranscriptSourceSettingTypeDef](./type_defs.md#transcriptsourcesettingtypedef) 
3. See [:material-code-braces: EncryptionSettingTypeDef](./type_defs.md#encryptionsettingtypedef) 
4. See [:material-code-braces: BotRecommendationResultsTypeDef](./type_defs.md#botrecommendationresultstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartBotRecommendationRequestRequestTypeDef

```python
# StartBotRecommendationRequestRequestTypeDef definition

class StartBotRecommendationRequestRequestTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    transcriptSourceSetting: TranscriptSourceSettingTypeDef,  # (1)
    encryptionSetting: NotRequired[EncryptionSettingTypeDef],  # (2)
```

1. See [:material-code-braces: TranscriptSourceSettingTypeDef](./type_defs.md#transcriptsourcesettingtypedef) 
2. See [:material-code-braces: EncryptionSettingTypeDef](./type_defs.md#encryptionsettingtypedef) 
## StartBotRecommendationResponseTypeDef

```python
# StartBotRecommendationResponseTypeDef definition

class StartBotRecommendationResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationStatus: BotRecommendationStatusType,  # (1)
    botRecommendationId: str,
    creationDateTime: datetime,
    transcriptSourceSetting: TranscriptSourceSettingTypeDef,  # (2)
    encryptionSetting: EncryptionSettingTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: BotRecommendationStatusType](./literals.md#botrecommendationstatustype) 
2. See [:material-code-braces: TranscriptSourceSettingTypeDef](./type_defs.md#transcriptsourcesettingtypedef) 
3. See [:material-code-braces: EncryptionSettingTypeDef](./type_defs.md#encryptionsettingtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBotRecommendationResponseTypeDef

```python
# UpdateBotRecommendationResponseTypeDef definition

class UpdateBotRecommendationResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationStatus: BotRecommendationStatusType,  # (1)
    botRecommendationId: str,
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    transcriptSourceSetting: TranscriptSourceSettingTypeDef,  # (2)
    encryptionSetting: EncryptionSettingTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: BotRecommendationStatusType](./literals.md#botrecommendationstatustype) 
2. See [:material-code-braces: TranscriptSourceSettingTypeDef](./type_defs.md#transcriptsourcesettingtypedef) 
3. See [:material-code-braces: EncryptionSettingTypeDef](./type_defs.md#encryptionsettingtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UtteranceLevelTestResultItemTypeDef

```python
# UtteranceLevelTestResultItemTypeDef definition

class UtteranceLevelTestResultItemTypeDef(TypedDict):
    recordNumber: int,
    turnResult: TestSetTurnResultTypeDef,  # (1)
    conversationId: NotRequired[str],
```

1. See [:material-code-braces: TestSetTurnResultTypeDef](./type_defs.md#testsetturnresulttypedef) 
## TestSetTurnRecordTypeDef

```python
# TestSetTurnRecordTypeDef definition

class TestSetTurnRecordTypeDef(TypedDict):
    recordNumber: int,
    turnSpecification: TurnSpecificationTypeDef,  # (1)
    conversationId: NotRequired[str],
    turnNumber: NotRequired[int],
```

1. See [:material-code-braces: TurnSpecificationTypeDef](./type_defs.md#turnspecificationtypedef) 
## ListSlotsResponseTypeDef

```python
# ListSlotsResponseTypeDef definition

class ListSlotsResponseTypeDef(TypedDict):
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
    slotSummaries: List[SlotSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SlotSummaryTypeDef](./type_defs.md#slotsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConditionalSpecificationTypeDef

```python
# ConditionalSpecificationTypeDef definition

class ConditionalSpecificationTypeDef(TypedDict):
    active: bool,
    conditionalBranches: Sequence[ConditionalBranchTypeDef],  # (1)
    defaultBranch: DefaultConditionalBranchTypeDef,  # (2)
```

1. See [:material-code-braces: ConditionalBranchTypeDef](./type_defs.md#conditionalbranchtypedef) 
2. See [:material-code-braces: DefaultConditionalBranchTypeDef](./type_defs.md#defaultconditionalbranchtypedef) 
## SubSlotValueElicitationSettingTypeDef

```python
# SubSlotValueElicitationSettingTypeDef definition

class SubSlotValueElicitationSettingTypeDef(TypedDict):
    promptSpecification: PromptSpecificationTypeDef,  # (2)
    defaultValueSpecification: NotRequired[SlotDefaultValueSpecificationTypeDef],  # (1)
    sampleUtterances: NotRequired[Sequence[SampleUtteranceTypeDef]],  # (3)
    waitAndContinueSpecification: NotRequired[WaitAndContinueSpecificationTypeDef],  # (4)
```

1. See [:material-code-braces: SlotDefaultValueSpecificationTypeDef](./type_defs.md#slotdefaultvaluespecificationtypedef) 
2. See [:material-code-braces: PromptSpecificationTypeDef](./type_defs.md#promptspecificationtypedef) 
3. See [:material-code-braces: SampleUtteranceTypeDef](./type_defs.md#sampleutterancetypedef) 
4. See [:material-code-braces: WaitAndContinueSpecificationTypeDef](./type_defs.md#waitandcontinuespecificationtypedef) 
## UtteranceLevelTestResultsTypeDef

```python
# UtteranceLevelTestResultsTypeDef definition

class UtteranceLevelTestResultsTypeDef(TypedDict):
    items: List[UtteranceLevelTestResultItemTypeDef],  # (1)
```

1. See [:material-code-braces: UtteranceLevelTestResultItemTypeDef](./type_defs.md#utteranceleveltestresultitemtypedef) 
## ListTestSetRecordsResponseTypeDef

```python
# ListTestSetRecordsResponseTypeDef definition

class ListTestSetRecordsResponseTypeDef(TypedDict):
    testSetRecords: List[TestSetTurnRecordTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TestSetTurnRecordTypeDef](./type_defs.md#testsetturnrecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntentClosingSettingTypeDef

```python
# IntentClosingSettingTypeDef definition

class IntentClosingSettingTypeDef(TypedDict):
    closingResponse: NotRequired[ResponseSpecificationTypeDef],  # (1)
    active: NotRequired[bool],
    nextStep: NotRequired[DialogStateTypeDef],  # (2)
    conditional: NotRequired[ConditionalSpecificationTypeDef],  # (3)
```

1. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
2. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
3. See [:material-code-braces: ConditionalSpecificationTypeDef](./type_defs.md#conditionalspecificationtypedef) 
## PostDialogCodeHookInvocationSpecificationTypeDef

```python
# PostDialogCodeHookInvocationSpecificationTypeDef definition

class PostDialogCodeHookInvocationSpecificationTypeDef(TypedDict):
    successResponse: NotRequired[ResponseSpecificationTypeDef],  # (1)
    successNextStep: NotRequired[DialogStateTypeDef],  # (2)
    successConditional: NotRequired[ConditionalSpecificationTypeDef],  # (3)
    failureResponse: NotRequired[ResponseSpecificationTypeDef],  # (1)
    failureNextStep: NotRequired[DialogStateTypeDef],  # (2)
    failureConditional: NotRequired[ConditionalSpecificationTypeDef],  # (3)
    timeoutResponse: NotRequired[ResponseSpecificationTypeDef],  # (1)
    timeoutNextStep: NotRequired[DialogStateTypeDef],  # (2)
    timeoutConditional: NotRequired[ConditionalSpecificationTypeDef],  # (3)
```

1. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
2. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
3. See [:material-code-braces: ConditionalSpecificationTypeDef](./type_defs.md#conditionalspecificationtypedef) 
4. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
5. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
6. See [:material-code-braces: ConditionalSpecificationTypeDef](./type_defs.md#conditionalspecificationtypedef) 
7. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
8. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
9. See [:material-code-braces: ConditionalSpecificationTypeDef](./type_defs.md#conditionalspecificationtypedef) 
## PostFulfillmentStatusSpecificationTypeDef

```python
# PostFulfillmentStatusSpecificationTypeDef definition

class PostFulfillmentStatusSpecificationTypeDef(TypedDict):
    successResponse: NotRequired[ResponseSpecificationTypeDef],  # (1)
    failureResponse: NotRequired[ResponseSpecificationTypeDef],  # (1)
    timeoutResponse: NotRequired[ResponseSpecificationTypeDef],  # (1)
    successNextStep: NotRequired[DialogStateTypeDef],  # (4)
    successConditional: NotRequired[ConditionalSpecificationTypeDef],  # (5)
    failureNextStep: NotRequired[DialogStateTypeDef],  # (4)
    failureConditional: NotRequired[ConditionalSpecificationTypeDef],  # (5)
    timeoutNextStep: NotRequired[DialogStateTypeDef],  # (4)
    timeoutConditional: NotRequired[ConditionalSpecificationTypeDef],  # (5)
```

1. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
2. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
3. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
4. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
5. See [:material-code-braces: ConditionalSpecificationTypeDef](./type_defs.md#conditionalspecificationtypedef) 
6. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
7. See [:material-code-braces: ConditionalSpecificationTypeDef](./type_defs.md#conditionalspecificationtypedef) 
8. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
9. See [:material-code-braces: ConditionalSpecificationTypeDef](./type_defs.md#conditionalspecificationtypedef) 
## SpecificationsTypeDef

```python
# SpecificationsTypeDef definition

class SpecificationsTypeDef(TypedDict):
    slotTypeId: str,
    valueElicitationSetting: SubSlotValueElicitationSettingTypeDef,  # (1)
```

1. See [:material-code-braces: SubSlotValueElicitationSettingTypeDef](./type_defs.md#subslotvalueelicitationsettingtypedef) 
## TestExecutionResultItemsTypeDef

```python
# TestExecutionResultItemsTypeDef definition

class TestExecutionResultItemsTypeDef(TypedDict):
    overallTestResults: NotRequired[OverallTestResultsTypeDef],  # (1)
    conversationLevelTestResults: NotRequired[ConversationLevelTestResultsTypeDef],  # (2)
    intentClassificationTestResults: NotRequired[IntentClassificationTestResultsTypeDef],  # (3)
    intentLevelSlotResolutionTestResults: NotRequired[IntentLevelSlotResolutionTestResultsTypeDef],  # (4)
    utteranceLevelTestResults: NotRequired[UtteranceLevelTestResultsTypeDef],  # (5)
```

1. See [:material-code-braces: OverallTestResultsTypeDef](./type_defs.md#overalltestresultstypedef) 
2. See [:material-code-braces: ConversationLevelTestResultsTypeDef](./type_defs.md#conversationleveltestresultstypedef) 
3. See [:material-code-braces: IntentClassificationTestResultsTypeDef](./type_defs.md#intentclassificationtestresultstypedef) 
4. See [:material-code-braces: IntentLevelSlotResolutionTestResultsTypeDef](./type_defs.md#intentlevelslotresolutiontestresultstypedef) 
5. See [:material-code-braces: UtteranceLevelTestResultsTypeDef](./type_defs.md#utteranceleveltestresultstypedef) 
## DialogCodeHookInvocationSettingTypeDef

```python
# DialogCodeHookInvocationSettingTypeDef definition

class DialogCodeHookInvocationSettingTypeDef(TypedDict):
    enableCodeHookInvocation: bool,
    active: bool,
    postCodeHookSpecification: PostDialogCodeHookInvocationSpecificationTypeDef,  # (1)
    invocationLabel: NotRequired[str],
```

1. See [:material-code-braces: PostDialogCodeHookInvocationSpecificationTypeDef](./type_defs.md#postdialogcodehookinvocationspecificationtypedef) 
## FulfillmentCodeHookSettingsTypeDef

```python
# FulfillmentCodeHookSettingsTypeDef definition

class FulfillmentCodeHookSettingsTypeDef(TypedDict):
    enabled: bool,
    postFulfillmentStatusSpecification: NotRequired[PostFulfillmentStatusSpecificationTypeDef],  # (1)
    fulfillmentUpdatesSpecification: NotRequired[FulfillmentUpdatesSpecificationTypeDef],  # (2)
    active: NotRequired[bool],
```

1. See [:material-code-braces: PostFulfillmentStatusSpecificationTypeDef](./type_defs.md#postfulfillmentstatusspecificationtypedef) 
2. See [:material-code-braces: FulfillmentUpdatesSpecificationTypeDef](./type_defs.md#fulfillmentupdatesspecificationtypedef) 
## SubSlotSettingTypeDef

```python
# SubSlotSettingTypeDef definition

class SubSlotSettingTypeDef(TypedDict):
    expression: NotRequired[str],
    slotSpecifications: NotRequired[Mapping[str, SpecificationsTypeDef]],  # (1)
```

1. See [:material-code-braces: SpecificationsTypeDef](./type_defs.md#specificationstypedef) 
## ListTestExecutionResultItemsResponseTypeDef

```python
# ListTestExecutionResultItemsResponseTypeDef definition

class ListTestExecutionResultItemsResponseTypeDef(TypedDict):
    testExecutionResults: TestExecutionResultItemsTypeDef,  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TestExecutionResultItemsTypeDef](./type_defs.md#testexecutionresultitemstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InitialResponseSettingTypeDef

```python
# InitialResponseSettingTypeDef definition

class InitialResponseSettingTypeDef(TypedDict):
    initialResponse: NotRequired[ResponseSpecificationTypeDef],  # (1)
    nextStep: NotRequired[DialogStateTypeDef],  # (2)
    conditional: NotRequired[ConditionalSpecificationTypeDef],  # (3)
    codeHook: NotRequired[DialogCodeHookInvocationSettingTypeDef],  # (4)
```

1. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
2. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
3. See [:material-code-braces: ConditionalSpecificationTypeDef](./type_defs.md#conditionalspecificationtypedef) 
4. See [:material-code-braces: DialogCodeHookInvocationSettingTypeDef](./type_defs.md#dialogcodehookinvocationsettingtypedef) 
## IntentConfirmationSettingTypeDef

```python
# IntentConfirmationSettingTypeDef definition

class IntentConfirmationSettingTypeDef(TypedDict):
    promptSpecification: PromptSpecificationTypeDef,  # (1)
    declinationResponse: NotRequired[ResponseSpecificationTypeDef],  # (2)
    active: NotRequired[bool],
    confirmationResponse: NotRequired[ResponseSpecificationTypeDef],  # (2)
    confirmationNextStep: NotRequired[DialogStateTypeDef],  # (4)
    confirmationConditional: NotRequired[ConditionalSpecificationTypeDef],  # (5)
    declinationNextStep: NotRequired[DialogStateTypeDef],  # (4)
    declinationConditional: NotRequired[ConditionalSpecificationTypeDef],  # (5)
    failureResponse: NotRequired[ResponseSpecificationTypeDef],  # (2)
    failureNextStep: NotRequired[DialogStateTypeDef],  # (4)
    failureConditional: NotRequired[ConditionalSpecificationTypeDef],  # (5)
    codeHook: NotRequired[DialogCodeHookInvocationSettingTypeDef],  # (11)
    elicitationCodeHook: NotRequired[ElicitationCodeHookInvocationSettingTypeDef],  # (12)
```

1. See [:material-code-braces: PromptSpecificationTypeDef](./type_defs.md#promptspecificationtypedef) 
2. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
3. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
4. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
5. See [:material-code-braces: ConditionalSpecificationTypeDef](./type_defs.md#conditionalspecificationtypedef) 
6. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
7. See [:material-code-braces: ConditionalSpecificationTypeDef](./type_defs.md#conditionalspecificationtypedef) 
8. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
9. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
10. See [:material-code-braces: ConditionalSpecificationTypeDef](./type_defs.md#conditionalspecificationtypedef) 
11. See [:material-code-braces: DialogCodeHookInvocationSettingTypeDef](./type_defs.md#dialogcodehookinvocationsettingtypedef) 
12. See [:material-code-braces: ElicitationCodeHookInvocationSettingTypeDef](./type_defs.md#elicitationcodehookinvocationsettingtypedef) 
## SlotCaptureSettingTypeDef

```python
# SlotCaptureSettingTypeDef definition

class SlotCaptureSettingTypeDef(TypedDict):
    captureResponse: NotRequired[ResponseSpecificationTypeDef],  # (1)
    captureNextStep: NotRequired[DialogStateTypeDef],  # (2)
    captureConditional: NotRequired[ConditionalSpecificationTypeDef],  # (3)
    failureResponse: NotRequired[ResponseSpecificationTypeDef],  # (1)
    failureNextStep: NotRequired[DialogStateTypeDef],  # (2)
    failureConditional: NotRequired[ConditionalSpecificationTypeDef],  # (3)
    codeHook: NotRequired[DialogCodeHookInvocationSettingTypeDef],  # (7)
    elicitationCodeHook: NotRequired[ElicitationCodeHookInvocationSettingTypeDef],  # (8)
```

1. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
2. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
3. See [:material-code-braces: ConditionalSpecificationTypeDef](./type_defs.md#conditionalspecificationtypedef) 
4. See [:material-code-braces: ResponseSpecificationTypeDef](./type_defs.md#responsespecificationtypedef) 
5. See [:material-code-braces: DialogStateTypeDef](./type_defs.md#dialogstatetypedef) 
6. See [:material-code-braces: ConditionalSpecificationTypeDef](./type_defs.md#conditionalspecificationtypedef) 
7. See [:material-code-braces: DialogCodeHookInvocationSettingTypeDef](./type_defs.md#dialogcodehookinvocationsettingtypedef) 
8. See [:material-code-braces: ElicitationCodeHookInvocationSettingTypeDef](./type_defs.md#elicitationcodehookinvocationsettingtypedef) 
## CreateIntentRequestRequestTypeDef

```python
# CreateIntentRequestRequestTypeDef definition

class CreateIntentRequestRequestTypeDef(TypedDict):
    intentName: str,
    botId: str,
    botVersion: str,
    localeId: str,
    description: NotRequired[str],
    parentIntentSignature: NotRequired[str],
    sampleUtterances: NotRequired[Sequence[SampleUtteranceTypeDef]],  # (1)
    dialogCodeHook: NotRequired[DialogCodeHookSettingsTypeDef],  # (2)
    fulfillmentCodeHook: NotRequired[FulfillmentCodeHookSettingsTypeDef],  # (3)
    intentConfirmationSetting: NotRequired[IntentConfirmationSettingTypeDef],  # (4)
    intentClosingSetting: NotRequired[IntentClosingSettingTypeDef],  # (5)
    inputContexts: NotRequired[Sequence[InputContextTypeDef]],  # (6)
    outputContexts: NotRequired[Sequence[OutputContextTypeDef]],  # (7)
    kendraConfiguration: NotRequired[KendraConfigurationTypeDef],  # (8)
    initialResponseSetting: NotRequired[InitialResponseSettingTypeDef],  # (9)
```

1. See [:material-code-braces: SampleUtteranceTypeDef](./type_defs.md#sampleutterancetypedef) 
2. See [:material-code-braces: DialogCodeHookSettingsTypeDef](./type_defs.md#dialogcodehooksettingstypedef) 
3. See [:material-code-braces: FulfillmentCodeHookSettingsTypeDef](./type_defs.md#fulfillmentcodehooksettingstypedef) 
4. See [:material-code-braces: IntentConfirmationSettingTypeDef](./type_defs.md#intentconfirmationsettingtypedef) 
5. See [:material-code-braces: IntentClosingSettingTypeDef](./type_defs.md#intentclosingsettingtypedef) 
6. See [:material-code-braces: InputContextTypeDef](./type_defs.md#inputcontexttypedef) 
7. See [:material-code-braces: OutputContextTypeDef](./type_defs.md#outputcontexttypedef) 
8. See [:material-code-braces: KendraConfigurationTypeDef](./type_defs.md#kendraconfigurationtypedef) 
9. See [:material-code-braces: InitialResponseSettingTypeDef](./type_defs.md#initialresponsesettingtypedef) 
## CreateIntentResponseTypeDef

```python
# CreateIntentResponseTypeDef definition

class CreateIntentResponseTypeDef(TypedDict):
    intentId: str,
    intentName: str,
    description: str,
    parentIntentSignature: str,
    sampleUtterances: List[SampleUtteranceTypeDef],  # (1)
    dialogCodeHook: DialogCodeHookSettingsTypeDef,  # (2)
    fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef,  # (3)
    intentConfirmationSetting: IntentConfirmationSettingTypeDef,  # (4)
    intentClosingSetting: IntentClosingSettingTypeDef,  # (5)
    inputContexts: List[InputContextTypeDef],  # (6)
    outputContexts: List[OutputContextTypeDef],  # (7)
    kendraConfiguration: KendraConfigurationTypeDef,  # (8)
    botId: str,
    botVersion: str,
    localeId: str,
    creationDateTime: datetime,
    initialResponseSetting: InitialResponseSettingTypeDef,  # (9)
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-braces: SampleUtteranceTypeDef](./type_defs.md#sampleutterancetypedef) 
2. See [:material-code-braces: DialogCodeHookSettingsTypeDef](./type_defs.md#dialogcodehooksettingstypedef) 
3. See [:material-code-braces: FulfillmentCodeHookSettingsTypeDef](./type_defs.md#fulfillmentcodehooksettingstypedef) 
4. See [:material-code-braces: IntentConfirmationSettingTypeDef](./type_defs.md#intentconfirmationsettingtypedef) 
5. See [:material-code-braces: IntentClosingSettingTypeDef](./type_defs.md#intentclosingsettingtypedef) 
6. See [:material-code-braces: InputContextTypeDef](./type_defs.md#inputcontexttypedef) 
7. See [:material-code-braces: OutputContextTypeDef](./type_defs.md#outputcontexttypedef) 
8. See [:material-code-braces: KendraConfigurationTypeDef](./type_defs.md#kendraconfigurationtypedef) 
9. See [:material-code-braces: InitialResponseSettingTypeDef](./type_defs.md#initialresponsesettingtypedef) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeIntentResponseTypeDef

```python
# DescribeIntentResponseTypeDef definition

class DescribeIntentResponseTypeDef(TypedDict):
    intentId: str,
    intentName: str,
    description: str,
    parentIntentSignature: str,
    sampleUtterances: List[SampleUtteranceTypeDef],  # (1)
    dialogCodeHook: DialogCodeHookSettingsTypeDef,  # (2)
    fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef,  # (3)
    slotPriorities: List[SlotPriorityTypeDef],  # (4)
    intentConfirmationSetting: IntentConfirmationSettingTypeDef,  # (5)
    intentClosingSetting: IntentClosingSettingTypeDef,  # (6)
    inputContexts: List[InputContextTypeDef],  # (7)
    outputContexts: List[OutputContextTypeDef],  # (8)
    kendraConfiguration: KendraConfigurationTypeDef,  # (9)
    botId: str,
    botVersion: str,
    localeId: str,
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    initialResponseSetting: InitialResponseSettingTypeDef,  # (10)
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-braces: SampleUtteranceTypeDef](./type_defs.md#sampleutterancetypedef) 
2. See [:material-code-braces: DialogCodeHookSettingsTypeDef](./type_defs.md#dialogcodehooksettingstypedef) 
3. See [:material-code-braces: FulfillmentCodeHookSettingsTypeDef](./type_defs.md#fulfillmentcodehooksettingstypedef) 
4. See [:material-code-braces: SlotPriorityTypeDef](./type_defs.md#slotprioritytypedef) 
5. See [:material-code-braces: IntentConfirmationSettingTypeDef](./type_defs.md#intentconfirmationsettingtypedef) 
6. See [:material-code-braces: IntentClosingSettingTypeDef](./type_defs.md#intentclosingsettingtypedef) 
7. See [:material-code-braces: InputContextTypeDef](./type_defs.md#inputcontexttypedef) 
8. See [:material-code-braces: OutputContextTypeDef](./type_defs.md#outputcontexttypedef) 
9. See [:material-code-braces: KendraConfigurationTypeDef](./type_defs.md#kendraconfigurationtypedef) 
10. See [:material-code-braces: InitialResponseSettingTypeDef](./type_defs.md#initialresponsesettingtypedef) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIntentRequestRequestTypeDef

```python
# UpdateIntentRequestRequestTypeDef definition

class UpdateIntentRequestRequestTypeDef(TypedDict):
    intentId: str,
    intentName: str,
    botId: str,
    botVersion: str,
    localeId: str,
    description: NotRequired[str],
    parentIntentSignature: NotRequired[str],
    sampleUtterances: NotRequired[Sequence[SampleUtteranceTypeDef]],  # (1)
    dialogCodeHook: NotRequired[DialogCodeHookSettingsTypeDef],  # (2)
    fulfillmentCodeHook: NotRequired[FulfillmentCodeHookSettingsTypeDef],  # (3)
    slotPriorities: NotRequired[Sequence[SlotPriorityTypeDef]],  # (4)
    intentConfirmationSetting: NotRequired[IntentConfirmationSettingTypeDef],  # (5)
    intentClosingSetting: NotRequired[IntentClosingSettingTypeDef],  # (6)
    inputContexts: NotRequired[Sequence[InputContextTypeDef]],  # (7)
    outputContexts: NotRequired[Sequence[OutputContextTypeDef]],  # (8)
    kendraConfiguration: NotRequired[KendraConfigurationTypeDef],  # (9)
    initialResponseSetting: NotRequired[InitialResponseSettingTypeDef],  # (10)
```

1. See [:material-code-braces: SampleUtteranceTypeDef](./type_defs.md#sampleutterancetypedef) 
2. See [:material-code-braces: DialogCodeHookSettingsTypeDef](./type_defs.md#dialogcodehooksettingstypedef) 
3. See [:material-code-braces: FulfillmentCodeHookSettingsTypeDef](./type_defs.md#fulfillmentcodehooksettingstypedef) 
4. See [:material-code-braces: SlotPriorityTypeDef](./type_defs.md#slotprioritytypedef) 
5. See [:material-code-braces: IntentConfirmationSettingTypeDef](./type_defs.md#intentconfirmationsettingtypedef) 
6. See [:material-code-braces: IntentClosingSettingTypeDef](./type_defs.md#intentclosingsettingtypedef) 
7. See [:material-code-braces: InputContextTypeDef](./type_defs.md#inputcontexttypedef) 
8. See [:material-code-braces: OutputContextTypeDef](./type_defs.md#outputcontexttypedef) 
9. See [:material-code-braces: KendraConfigurationTypeDef](./type_defs.md#kendraconfigurationtypedef) 
10. See [:material-code-braces: InitialResponseSettingTypeDef](./type_defs.md#initialresponsesettingtypedef) 
## UpdateIntentResponseTypeDef

```python
# UpdateIntentResponseTypeDef definition

class UpdateIntentResponseTypeDef(TypedDict):
    intentId: str,
    intentName: str,
    description: str,
    parentIntentSignature: str,
    sampleUtterances: List[SampleUtteranceTypeDef],  # (1)
    dialogCodeHook: DialogCodeHookSettingsTypeDef,  # (2)
    fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef,  # (3)
    slotPriorities: List[SlotPriorityTypeDef],  # (4)
    intentConfirmationSetting: IntentConfirmationSettingTypeDef,  # (5)
    intentClosingSetting: IntentClosingSettingTypeDef,  # (6)
    inputContexts: List[InputContextTypeDef],  # (7)
    outputContexts: List[OutputContextTypeDef],  # (8)
    kendraConfiguration: KendraConfigurationTypeDef,  # (9)
    botId: str,
    botVersion: str,
    localeId: str,
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    initialResponseSetting: InitialResponseSettingTypeDef,  # (10)
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-braces: SampleUtteranceTypeDef](./type_defs.md#sampleutterancetypedef) 
2. See [:material-code-braces: DialogCodeHookSettingsTypeDef](./type_defs.md#dialogcodehooksettingstypedef) 
3. See [:material-code-braces: FulfillmentCodeHookSettingsTypeDef](./type_defs.md#fulfillmentcodehooksettingstypedef) 
4. See [:material-code-braces: SlotPriorityTypeDef](./type_defs.md#slotprioritytypedef) 
5. See [:material-code-braces: IntentConfirmationSettingTypeDef](./type_defs.md#intentconfirmationsettingtypedef) 
6. See [:material-code-braces: IntentClosingSettingTypeDef](./type_defs.md#intentclosingsettingtypedef) 
7. See [:material-code-braces: InputContextTypeDef](./type_defs.md#inputcontexttypedef) 
8. See [:material-code-braces: OutputContextTypeDef](./type_defs.md#outputcontexttypedef) 
9. See [:material-code-braces: KendraConfigurationTypeDef](./type_defs.md#kendraconfigurationtypedef) 
10. See [:material-code-braces: InitialResponseSettingTypeDef](./type_defs.md#initialresponsesettingtypedef) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SlotValueElicitationSettingTypeDef

```python
# SlotValueElicitationSettingTypeDef definition

class SlotValueElicitationSettingTypeDef(TypedDict):
    slotConstraint: SlotConstraintType,  # (2)
    defaultValueSpecification: NotRequired[SlotDefaultValueSpecificationTypeDef],  # (1)
    promptSpecification: NotRequired[PromptSpecificationTypeDef],  # (3)
    sampleUtterances: NotRequired[Sequence[SampleUtteranceTypeDef]],  # (4)
    waitAndContinueSpecification: NotRequired[WaitAndContinueSpecificationTypeDef],  # (5)
    slotCaptureSetting: NotRequired[SlotCaptureSettingTypeDef],  # (6)
```

1. See [:material-code-braces: SlotDefaultValueSpecificationTypeDef](./type_defs.md#slotdefaultvaluespecificationtypedef) 
2. See [:material-code-brackets: SlotConstraintType](./literals.md#slotconstrainttype) 
3. See [:material-code-braces: PromptSpecificationTypeDef](./type_defs.md#promptspecificationtypedef) 
4. See [:material-code-braces: SampleUtteranceTypeDef](./type_defs.md#sampleutterancetypedef) 
5. See [:material-code-braces: WaitAndContinueSpecificationTypeDef](./type_defs.md#waitandcontinuespecificationtypedef) 
6. See [:material-code-braces: SlotCaptureSettingTypeDef](./type_defs.md#slotcapturesettingtypedef) 
## CreateSlotRequestRequestTypeDef

```python
# CreateSlotRequestRequestTypeDef definition

class CreateSlotRequestRequestTypeDef(TypedDict):
    slotName: str,
    valueElicitationSetting: SlotValueElicitationSettingTypeDef,  # (1)
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
    description: NotRequired[str],
    slotTypeId: NotRequired[str],
    obfuscationSetting: NotRequired[ObfuscationSettingTypeDef],  # (2)
    multipleValuesSetting: NotRequired[MultipleValuesSettingTypeDef],  # (3)
    subSlotSetting: NotRequired[SubSlotSettingTypeDef],  # (4)
```

1. See [:material-code-braces: SlotValueElicitationSettingTypeDef](./type_defs.md#slotvalueelicitationsettingtypedef) 
2. See [:material-code-braces: ObfuscationSettingTypeDef](./type_defs.md#obfuscationsettingtypedef) 
3. See [:material-code-braces: MultipleValuesSettingTypeDef](./type_defs.md#multiplevaluessettingtypedef) 
4. See [:material-code-braces: SubSlotSettingTypeDef](./type_defs.md#subslotsettingtypedef) 
## CreateSlotResponseTypeDef

```python
# CreateSlotResponseTypeDef definition

class CreateSlotResponseTypeDef(TypedDict):
    slotId: str,
    slotName: str,
    description: str,
    slotTypeId: str,
    valueElicitationSetting: SlotValueElicitationSettingTypeDef,  # (1)
    obfuscationSetting: ObfuscationSettingTypeDef,  # (2)
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
    creationDateTime: datetime,
    multipleValuesSetting: MultipleValuesSettingTypeDef,  # (3)
    subSlotSetting: SubSlotSettingTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SlotValueElicitationSettingTypeDef](./type_defs.md#slotvalueelicitationsettingtypedef) 
2. See [:material-code-braces: ObfuscationSettingTypeDef](./type_defs.md#obfuscationsettingtypedef) 
3. See [:material-code-braces: MultipleValuesSettingTypeDef](./type_defs.md#multiplevaluessettingtypedef) 
4. See [:material-code-braces: SubSlotSettingTypeDef](./type_defs.md#subslotsettingtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSlotResponseTypeDef

```python
# DescribeSlotResponseTypeDef definition

class DescribeSlotResponseTypeDef(TypedDict):
    slotId: str,
    slotName: str,
    description: str,
    slotTypeId: str,
    valueElicitationSetting: SlotValueElicitationSettingTypeDef,  # (1)
    obfuscationSetting: ObfuscationSettingTypeDef,  # (2)
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    multipleValuesSetting: MultipleValuesSettingTypeDef,  # (3)
    subSlotSetting: SubSlotSettingTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SlotValueElicitationSettingTypeDef](./type_defs.md#slotvalueelicitationsettingtypedef) 
2. See [:material-code-braces: ObfuscationSettingTypeDef](./type_defs.md#obfuscationsettingtypedef) 
3. See [:material-code-braces: MultipleValuesSettingTypeDef](./type_defs.md#multiplevaluessettingtypedef) 
4. See [:material-code-braces: SubSlotSettingTypeDef](./type_defs.md#subslotsettingtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSlotRequestRequestTypeDef

```python
# UpdateSlotRequestRequestTypeDef definition

class UpdateSlotRequestRequestTypeDef(TypedDict):
    slotId: str,
    slotName: str,
    valueElicitationSetting: SlotValueElicitationSettingTypeDef,  # (1)
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
    description: NotRequired[str],
    slotTypeId: NotRequired[str],
    obfuscationSetting: NotRequired[ObfuscationSettingTypeDef],  # (2)
    multipleValuesSetting: NotRequired[MultipleValuesSettingTypeDef],  # (3)
    subSlotSetting: NotRequired[SubSlotSettingTypeDef],  # (4)
```

1. See [:material-code-braces: SlotValueElicitationSettingTypeDef](./type_defs.md#slotvalueelicitationsettingtypedef) 
2. See [:material-code-braces: ObfuscationSettingTypeDef](./type_defs.md#obfuscationsettingtypedef) 
3. See [:material-code-braces: MultipleValuesSettingTypeDef](./type_defs.md#multiplevaluessettingtypedef) 
4. See [:material-code-braces: SubSlotSettingTypeDef](./type_defs.md#subslotsettingtypedef) 
## UpdateSlotResponseTypeDef

```python
# UpdateSlotResponseTypeDef definition

class UpdateSlotResponseTypeDef(TypedDict):
    slotId: str,
    slotName: str,
    description: str,
    slotTypeId: str,
    valueElicitationSetting: SlotValueElicitationSettingTypeDef,  # (1)
    obfuscationSetting: ObfuscationSettingTypeDef,  # (2)
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
    creationDateTime: datetime,
    lastUpdatedDateTime: datetime,
    multipleValuesSetting: MultipleValuesSettingTypeDef,  # (3)
    subSlotSetting: SubSlotSettingTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SlotValueElicitationSettingTypeDef](./type_defs.md#slotvalueelicitationsettingtypedef) 
2. See [:material-code-braces: ObfuscationSettingTypeDef](./type_defs.md#obfuscationsettingtypedef) 
3. See [:material-code-braces: MultipleValuesSettingTypeDef](./type_defs.md#multiplevaluessettingtypedef) 
4. See [:material-code-braces: SubSlotSettingTypeDef](./type_defs.md#subslotsettingtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
