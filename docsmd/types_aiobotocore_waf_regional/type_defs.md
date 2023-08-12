# Type definitions

> [Index](../README.md) > [WAFRegional](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [WAFRegional](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
    type annotations stubs module [types-aiobotocore-waf-regional](https://pypi.org/project/types-aiobotocore-waf-regional/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ExcludedRuleTypeDef

```python
# ExcludedRuleTypeDef definition

class ExcludedRuleTypeDef(TypedDict):
    RuleId: str,
```

## WafActionTypeDef

```python
# WafActionTypeDef definition

class WafActionTypeDef(TypedDict):
    Type: WafActionTypeType,  # (1)
```

1. See [:material-code-brackets: WafActionTypeType](./literals.md#wafactiontypetype) 
## WafOverrideActionTypeDef

```python
# WafOverrideActionTypeDef definition

class WafOverrideActionTypeDef(TypedDict):
    Type: WafOverrideActionTypeType,  # (1)
```

1. See [:material-code-brackets: WafOverrideActionTypeType](./literals.md#wafoverrideactiontypetype) 
## AssociateWebACLRequestRequestTypeDef

```python
# AssociateWebACLRequestRequestTypeDef definition

class AssociateWebACLRequestRequestTypeDef(TypedDict):
    WebACLId: str,
    ResourceArn: str,
```

## ByteMatchSetSummaryTypeDef

```python
# ByteMatchSetSummaryTypeDef definition

class ByteMatchSetSummaryTypeDef(TypedDict):
    ByteMatchSetId: str,
    Name: str,
```

## FieldToMatchTypeDef

```python
# FieldToMatchTypeDef definition

class FieldToMatchTypeDef(TypedDict):
    Type: MatchFieldTypeType,  # (1)
    Data: NotRequired[str],
```

1. See [:material-code-brackets: MatchFieldTypeType](./literals.md#matchfieldtypetype) 
## CreateByteMatchSetRequestRequestTypeDef

```python
# CreateByteMatchSetRequestRequestTypeDef definition

class CreateByteMatchSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
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

## CreateGeoMatchSetRequestRequestTypeDef

```python
# CreateGeoMatchSetRequestRequestTypeDef definition

class CreateGeoMatchSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## CreateIPSetRequestRequestTypeDef

```python
# CreateIPSetRequestRequestTypeDef definition

class CreateIPSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateRegexMatchSetRequestRequestTypeDef

```python
# CreateRegexMatchSetRequestRequestTypeDef definition

class CreateRegexMatchSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## CreateRegexPatternSetRequestRequestTypeDef

```python
# CreateRegexPatternSetRequestRequestTypeDef definition

class CreateRegexPatternSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## RegexPatternSetTypeDef

```python
# RegexPatternSetTypeDef definition

class RegexPatternSetTypeDef(TypedDict):
    RegexPatternSetId: str,
    RegexPatternStrings: List[str],
    Name: NotRequired[str],
```

## RuleGroupTypeDef

```python
# RuleGroupTypeDef definition

class RuleGroupTypeDef(TypedDict):
    RuleGroupId: str,
    Name: NotRequired[str],
    MetricName: NotRequired[str],
```

## CreateSizeConstraintSetRequestRequestTypeDef

```python
# CreateSizeConstraintSetRequestRequestTypeDef definition

class CreateSizeConstraintSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## CreateSqlInjectionMatchSetRequestRequestTypeDef

```python
# CreateSqlInjectionMatchSetRequestRequestTypeDef definition

class CreateSqlInjectionMatchSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## CreateWebACLMigrationStackRequestRequestTypeDef

```python
# CreateWebACLMigrationStackRequestRequestTypeDef definition

class CreateWebACLMigrationStackRequestRequestTypeDef(TypedDict):
    WebACLId: str,
    S3BucketName: str,
    IgnoreUnsupportedType: bool,
```

## CreateXssMatchSetRequestRequestTypeDef

```python
# CreateXssMatchSetRequestRequestTypeDef definition

class CreateXssMatchSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## DeleteByteMatchSetRequestRequestTypeDef

```python
# DeleteByteMatchSetRequestRequestTypeDef definition

class DeleteByteMatchSetRequestRequestTypeDef(TypedDict):
    ByteMatchSetId: str,
    ChangeToken: str,
```

## DeleteGeoMatchSetRequestRequestTypeDef

```python
# DeleteGeoMatchSetRequestRequestTypeDef definition

class DeleteGeoMatchSetRequestRequestTypeDef(TypedDict):
    GeoMatchSetId: str,
    ChangeToken: str,
```

## DeleteIPSetRequestRequestTypeDef

```python
# DeleteIPSetRequestRequestTypeDef definition

class DeleteIPSetRequestRequestTypeDef(TypedDict):
    IPSetId: str,
    ChangeToken: str,
```

## DeleteLoggingConfigurationRequestRequestTypeDef

```python
# DeleteLoggingConfigurationRequestRequestTypeDef definition

class DeleteLoggingConfigurationRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DeletePermissionPolicyRequestRequestTypeDef

```python
# DeletePermissionPolicyRequestRequestTypeDef definition

class DeletePermissionPolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DeleteRateBasedRuleRequestRequestTypeDef

```python
# DeleteRateBasedRuleRequestRequestTypeDef definition

class DeleteRateBasedRuleRequestRequestTypeDef(TypedDict):
    RuleId: str,
    ChangeToken: str,
```

## DeleteRegexMatchSetRequestRequestTypeDef

```python
# DeleteRegexMatchSetRequestRequestTypeDef definition

class DeleteRegexMatchSetRequestRequestTypeDef(TypedDict):
    RegexMatchSetId: str,
    ChangeToken: str,
```

## DeleteRegexPatternSetRequestRequestTypeDef

```python
# DeleteRegexPatternSetRequestRequestTypeDef definition

class DeleteRegexPatternSetRequestRequestTypeDef(TypedDict):
    RegexPatternSetId: str,
    ChangeToken: str,
```

## DeleteRuleGroupRequestRequestTypeDef

```python
# DeleteRuleGroupRequestRequestTypeDef definition

class DeleteRuleGroupRequestRequestTypeDef(TypedDict):
    RuleGroupId: str,
    ChangeToken: str,
```

## DeleteRuleRequestRequestTypeDef

```python
# DeleteRuleRequestRequestTypeDef definition

class DeleteRuleRequestRequestTypeDef(TypedDict):
    RuleId: str,
    ChangeToken: str,
```

## DeleteSizeConstraintSetRequestRequestTypeDef

```python
# DeleteSizeConstraintSetRequestRequestTypeDef definition

class DeleteSizeConstraintSetRequestRequestTypeDef(TypedDict):
    SizeConstraintSetId: str,
    ChangeToken: str,
```

## DeleteSqlInjectionMatchSetRequestRequestTypeDef

```python
# DeleteSqlInjectionMatchSetRequestRequestTypeDef definition

class DeleteSqlInjectionMatchSetRequestRequestTypeDef(TypedDict):
    SqlInjectionMatchSetId: str,
    ChangeToken: str,
```

## DeleteWebACLRequestRequestTypeDef

```python
# DeleteWebACLRequestRequestTypeDef definition

class DeleteWebACLRequestRequestTypeDef(TypedDict):
    WebACLId: str,
    ChangeToken: str,
```

## DeleteXssMatchSetRequestRequestTypeDef

```python
# DeleteXssMatchSetRequestRequestTypeDef definition

class DeleteXssMatchSetRequestRequestTypeDef(TypedDict):
    XssMatchSetId: str,
    ChangeToken: str,
```

## DisassociateWebACLRequestRequestTypeDef

```python
# DisassociateWebACLRequestRequestTypeDef definition

class DisassociateWebACLRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GeoMatchConstraintTypeDef

```python
# GeoMatchConstraintTypeDef definition

class GeoMatchConstraintTypeDef(TypedDict):
    Type: GeoMatchConstraintTypeType,  # (1)
    Value: GeoMatchConstraintValueType,  # (2)
```

1. See [:material-code-brackets: GeoMatchConstraintTypeType](./literals.md#geomatchconstrainttypetype) 
2. See [:material-code-brackets: GeoMatchConstraintValueType](./literals.md#geomatchconstraintvaluetype) 
## GeoMatchSetSummaryTypeDef

```python
# GeoMatchSetSummaryTypeDef definition

class GeoMatchSetSummaryTypeDef(TypedDict):
    GeoMatchSetId: str,
    Name: str,
```

## GetByteMatchSetRequestRequestTypeDef

```python
# GetByteMatchSetRequestRequestTypeDef definition

class GetByteMatchSetRequestRequestTypeDef(TypedDict):
    ByteMatchSetId: str,
```

## GetChangeTokenStatusRequestRequestTypeDef

```python
# GetChangeTokenStatusRequestRequestTypeDef definition

class GetChangeTokenStatusRequestRequestTypeDef(TypedDict):
    ChangeToken: str,
```

## GetGeoMatchSetRequestRequestTypeDef

```python
# GetGeoMatchSetRequestRequestTypeDef definition

class GetGeoMatchSetRequestRequestTypeDef(TypedDict):
    GeoMatchSetId: str,
```

## GetIPSetRequestRequestTypeDef

```python
# GetIPSetRequestRequestTypeDef definition

class GetIPSetRequestRequestTypeDef(TypedDict):
    IPSetId: str,
```

## GetLoggingConfigurationRequestRequestTypeDef

```python
# GetLoggingConfigurationRequestRequestTypeDef definition

class GetLoggingConfigurationRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetPermissionPolicyRequestRequestTypeDef

```python
# GetPermissionPolicyRequestRequestTypeDef definition

class GetPermissionPolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetRateBasedRuleManagedKeysRequestRequestTypeDef

```python
# GetRateBasedRuleManagedKeysRequestRequestTypeDef definition

class GetRateBasedRuleManagedKeysRequestRequestTypeDef(TypedDict):
    RuleId: str,
    NextMarker: NotRequired[str],
```

## GetRateBasedRuleRequestRequestTypeDef

```python
# GetRateBasedRuleRequestRequestTypeDef definition

class GetRateBasedRuleRequestRequestTypeDef(TypedDict):
    RuleId: str,
```

## GetRegexMatchSetRequestRequestTypeDef

```python
# GetRegexMatchSetRequestRequestTypeDef definition

class GetRegexMatchSetRequestRequestTypeDef(TypedDict):
    RegexMatchSetId: str,
```

## GetRegexPatternSetRequestRequestTypeDef

```python
# GetRegexPatternSetRequestRequestTypeDef definition

class GetRegexPatternSetRequestRequestTypeDef(TypedDict):
    RegexPatternSetId: str,
```

## GetRuleGroupRequestRequestTypeDef

```python
# GetRuleGroupRequestRequestTypeDef definition

class GetRuleGroupRequestRequestTypeDef(TypedDict):
    RuleGroupId: str,
```

## GetRuleRequestRequestTypeDef

```python
# GetRuleRequestRequestTypeDef definition

class GetRuleRequestRequestTypeDef(TypedDict):
    RuleId: str,
```

## GetSizeConstraintSetRequestRequestTypeDef

```python
# GetSizeConstraintSetRequestRequestTypeDef definition

class GetSizeConstraintSetRequestRequestTypeDef(TypedDict):
    SizeConstraintSetId: str,
```

## GetSqlInjectionMatchSetRequestRequestTypeDef

```python
# GetSqlInjectionMatchSetRequestRequestTypeDef definition

class GetSqlInjectionMatchSetRequestRequestTypeDef(TypedDict):
    SqlInjectionMatchSetId: str,
```

## GetWebACLForResourceRequestRequestTypeDef

```python
# GetWebACLForResourceRequestRequestTypeDef definition

class GetWebACLForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## WebACLSummaryTypeDef

```python
# WebACLSummaryTypeDef definition

class WebACLSummaryTypeDef(TypedDict):
    WebACLId: str,
    Name: str,
```

## GetWebACLRequestRequestTypeDef

```python
# GetWebACLRequestRequestTypeDef definition

class GetWebACLRequestRequestTypeDef(TypedDict):
    WebACLId: str,
```

## GetXssMatchSetRequestRequestTypeDef

```python
# GetXssMatchSetRequestRequestTypeDef definition

class GetXssMatchSetRequestRequestTypeDef(TypedDict):
    XssMatchSetId: str,
```

## HTTPHeaderTypeDef

```python
# HTTPHeaderTypeDef definition

class HTTPHeaderTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## IPSetDescriptorTypeDef

```python
# IPSetDescriptorTypeDef definition

class IPSetDescriptorTypeDef(TypedDict):
    Type: IPSetDescriptorTypeType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: IPSetDescriptorTypeType](./literals.md#ipsetdescriptortypetype) 
## IPSetSummaryTypeDef

```python
# IPSetSummaryTypeDef definition

class IPSetSummaryTypeDef(TypedDict):
    IPSetId: str,
    Name: str,
```

## ListActivatedRulesInRuleGroupRequestRequestTypeDef

```python
# ListActivatedRulesInRuleGroupRequestRequestTypeDef definition

class ListActivatedRulesInRuleGroupRequestRequestTypeDef(TypedDict):
    RuleGroupId: NotRequired[str],
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListByteMatchSetsRequestRequestTypeDef

```python
# ListByteMatchSetsRequestRequestTypeDef definition

class ListByteMatchSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListGeoMatchSetsRequestRequestTypeDef

```python
# ListGeoMatchSetsRequestRequestTypeDef definition

class ListGeoMatchSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListIPSetsRequestRequestTypeDef

```python
# ListIPSetsRequestRequestTypeDef definition

class ListIPSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListLoggingConfigurationsRequestRequestTypeDef

```python
# ListLoggingConfigurationsRequestRequestTypeDef definition

class ListLoggingConfigurationsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListRateBasedRulesRequestRequestTypeDef

```python
# ListRateBasedRulesRequestRequestTypeDef definition

class ListRateBasedRulesRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## RuleSummaryTypeDef

```python
# RuleSummaryTypeDef definition

class RuleSummaryTypeDef(TypedDict):
    RuleId: str,
    Name: str,
```

## ListRegexMatchSetsRequestRequestTypeDef

```python
# ListRegexMatchSetsRequestRequestTypeDef definition

class ListRegexMatchSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## RegexMatchSetSummaryTypeDef

```python
# RegexMatchSetSummaryTypeDef definition

class RegexMatchSetSummaryTypeDef(TypedDict):
    RegexMatchSetId: str,
    Name: str,
```

## ListRegexPatternSetsRequestRequestTypeDef

```python
# ListRegexPatternSetsRequestRequestTypeDef definition

class ListRegexPatternSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## RegexPatternSetSummaryTypeDef

```python
# RegexPatternSetSummaryTypeDef definition

class RegexPatternSetSummaryTypeDef(TypedDict):
    RegexPatternSetId: str,
    Name: str,
```

## ListResourcesForWebACLRequestRequestTypeDef

```python
# ListResourcesForWebACLRequestRequestTypeDef definition

class ListResourcesForWebACLRequestRequestTypeDef(TypedDict):
    WebACLId: str,
    ResourceType: NotRequired[ResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ListRuleGroupsRequestRequestTypeDef

```python
# ListRuleGroupsRequestRequestTypeDef definition

class ListRuleGroupsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## RuleGroupSummaryTypeDef

```python
# RuleGroupSummaryTypeDef definition

class RuleGroupSummaryTypeDef(TypedDict):
    RuleGroupId: str,
    Name: str,
```

## ListRulesRequestRequestTypeDef

```python
# ListRulesRequestRequestTypeDef definition

class ListRulesRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListSizeConstraintSetsRequestRequestTypeDef

```python
# ListSizeConstraintSetsRequestRequestTypeDef definition

class ListSizeConstraintSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## SizeConstraintSetSummaryTypeDef

```python
# SizeConstraintSetSummaryTypeDef definition

class SizeConstraintSetSummaryTypeDef(TypedDict):
    SizeConstraintSetId: str,
    Name: str,
```

## ListSqlInjectionMatchSetsRequestRequestTypeDef

```python
# ListSqlInjectionMatchSetsRequestRequestTypeDef definition

class ListSqlInjectionMatchSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## SqlInjectionMatchSetSummaryTypeDef

```python
# SqlInjectionMatchSetSummaryTypeDef definition

class SqlInjectionMatchSetSummaryTypeDef(TypedDict):
    SqlInjectionMatchSetId: str,
    Name: str,
```

## ListSubscribedRuleGroupsRequestRequestTypeDef

```python
# ListSubscribedRuleGroupsRequestRequestTypeDef definition

class ListSubscribedRuleGroupsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## SubscribedRuleGroupSummaryTypeDef

```python
# SubscribedRuleGroupSummaryTypeDef definition

class SubscribedRuleGroupSummaryTypeDef(TypedDict):
    RuleGroupId: str,
    Name: str,
    MetricName: str,
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListWebACLsRequestRequestTypeDef

```python
# ListWebACLsRequestRequestTypeDef definition

class ListWebACLsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListXssMatchSetsRequestRequestTypeDef

```python
# ListXssMatchSetsRequestRequestTypeDef definition

class ListXssMatchSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## XssMatchSetSummaryTypeDef

```python
# XssMatchSetSummaryTypeDef definition

class XssMatchSetSummaryTypeDef(TypedDict):
    XssMatchSetId: str,
    Name: str,
```

## PredicateTypeDef

```python
# PredicateTypeDef definition

class PredicateTypeDef(TypedDict):
    Negated: bool,
    Type: PredicateTypeType,  # (1)
    DataId: str,
```

1. See [:material-code-brackets: PredicateTypeType](./literals.md#predicatetypetype) 
## PutPermissionPolicyRequestRequestTypeDef

```python
# PutPermissionPolicyRequestRequestTypeDef definition

class PutPermissionPolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
```

## RegexPatternSetUpdateTypeDef

```python
# RegexPatternSetUpdateTypeDef definition

class RegexPatternSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    RegexPatternString: str,
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## ActivatedRuleTypeDef

```python
# ActivatedRuleTypeDef definition

class ActivatedRuleTypeDef(TypedDict):
    Priority: int,
    RuleId: str,
    Action: NotRequired[WafActionTypeDef],  # (1)
    OverrideAction: NotRequired[WafOverrideActionTypeDef],  # (2)
    Type: NotRequired[WafRuleTypeType],  # (3)
    ExcludedRules: NotRequired[List[ExcludedRuleTypeDef]],  # (4)
```

1. See [:material-code-braces: WafActionTypeDef](./type_defs.md#wafactiontypedef) 
2. See [:material-code-braces: WafOverrideActionTypeDef](./type_defs.md#wafoverrideactiontypedef) 
3. See [:material-code-brackets: WafRuleTypeType](./literals.md#wafruletypetype) 
4. See [:material-code-braces: ExcludedRuleTypeDef](./type_defs.md#excludedruletypedef) 
## ByteMatchTupleTypeDef

```python
# ByteMatchTupleTypeDef definition

class ByteMatchTupleTypeDef(TypedDict):
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TargetString: bytes,
    TextTransformation: TextTransformationType,  # (2)
    PositionalConstraint: PositionalConstraintType,  # (3)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-brackets: TextTransformationType](./literals.md#texttransformationtype) 
3. See [:material-code-brackets: PositionalConstraintType](./literals.md#positionalconstrainttype) 
## LoggingConfigurationTypeDef

```python
# LoggingConfigurationTypeDef definition

class LoggingConfigurationTypeDef(TypedDict):
    ResourceArn: str,
    LogDestinationConfigs: List[str],
    RedactedFields: NotRequired[List[FieldToMatchTypeDef]],  # (1)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
## RegexMatchTupleTypeDef

```python
# RegexMatchTupleTypeDef definition

class RegexMatchTupleTypeDef(TypedDict):
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TextTransformation: TextTransformationType,  # (2)
    RegexPatternSetId: str,
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-brackets: TextTransformationType](./literals.md#texttransformationtype) 
## SizeConstraintTypeDef

```python
# SizeConstraintTypeDef definition

class SizeConstraintTypeDef(TypedDict):
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TextTransformation: TextTransformationType,  # (2)
    ComparisonOperator: ComparisonOperatorType,  # (3)
    Size: int,
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-brackets: TextTransformationType](./literals.md#texttransformationtype) 
3. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## SqlInjectionMatchTupleTypeDef

```python
# SqlInjectionMatchTupleTypeDef definition

class SqlInjectionMatchTupleTypeDef(TypedDict):
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TextTransformation: TextTransformationType,  # (2)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-brackets: TextTransformationType](./literals.md#texttransformationtype) 
## XssMatchTupleTypeDef

```python
# XssMatchTupleTypeDef definition

class XssMatchTupleTypeDef(TypedDict):
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TextTransformation: TextTransformationType,  # (2)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-brackets: TextTransformationType](./literals.md#texttransformationtype) 
## CreateWebACLMigrationStackResponseTypeDef

```python
# CreateWebACLMigrationStackResponseTypeDef definition

class CreateWebACLMigrationStackResponseTypeDef(TypedDict):
    S3ObjectUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteByteMatchSetResponseTypeDef

```python
# DeleteByteMatchSetResponseTypeDef definition

class DeleteByteMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGeoMatchSetResponseTypeDef

```python
# DeleteGeoMatchSetResponseTypeDef definition

class DeleteGeoMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteIPSetResponseTypeDef

```python
# DeleteIPSetResponseTypeDef definition

class DeleteIPSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRateBasedRuleResponseTypeDef

```python
# DeleteRateBasedRuleResponseTypeDef definition

class DeleteRateBasedRuleResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRegexMatchSetResponseTypeDef

```python
# DeleteRegexMatchSetResponseTypeDef definition

class DeleteRegexMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRegexPatternSetResponseTypeDef

```python
# DeleteRegexPatternSetResponseTypeDef definition

class DeleteRegexPatternSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRuleGroupResponseTypeDef

```python
# DeleteRuleGroupResponseTypeDef definition

class DeleteRuleGroupResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRuleResponseTypeDef

```python
# DeleteRuleResponseTypeDef definition

class DeleteRuleResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSizeConstraintSetResponseTypeDef

```python
# DeleteSizeConstraintSetResponseTypeDef definition

class DeleteSizeConstraintSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSqlInjectionMatchSetResponseTypeDef

```python
# DeleteSqlInjectionMatchSetResponseTypeDef definition

class DeleteSqlInjectionMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWebACLResponseTypeDef

```python
# DeleteWebACLResponseTypeDef definition

class DeleteWebACLResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteXssMatchSetResponseTypeDef

```python
# DeleteXssMatchSetResponseTypeDef definition

class DeleteXssMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChangeTokenResponseTypeDef

```python
# GetChangeTokenResponseTypeDef definition

class GetChangeTokenResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChangeTokenStatusResponseTypeDef

```python
# GetChangeTokenStatusResponseTypeDef definition

class GetChangeTokenStatusResponseTypeDef(TypedDict):
    ChangeTokenStatus: ChangeTokenStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeTokenStatusType](./literals.md#changetokenstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPermissionPolicyResponseTypeDef

```python
# GetPermissionPolicyResponseTypeDef definition

class GetPermissionPolicyResponseTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRateBasedRuleManagedKeysResponseTypeDef

```python
# GetRateBasedRuleManagedKeysResponseTypeDef definition

class GetRateBasedRuleManagedKeysResponseTypeDef(TypedDict):
    ManagedKeys: List[str],
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListByteMatchSetsResponseTypeDef

```python
# ListByteMatchSetsResponseTypeDef definition

class ListByteMatchSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    ByteMatchSets: List[ByteMatchSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ByteMatchSetSummaryTypeDef](./type_defs.md#bytematchsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourcesForWebACLResponseTypeDef

```python
# ListResourcesForWebACLResponseTypeDef definition

class ListResourcesForWebACLResponseTypeDef(TypedDict):
    ResourceArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateByteMatchSetResponseTypeDef

```python
# UpdateByteMatchSetResponseTypeDef definition

class UpdateByteMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGeoMatchSetResponseTypeDef

```python
# UpdateGeoMatchSetResponseTypeDef definition

class UpdateGeoMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIPSetResponseTypeDef

```python
# UpdateIPSetResponseTypeDef definition

class UpdateIPSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRateBasedRuleResponseTypeDef

```python
# UpdateRateBasedRuleResponseTypeDef definition

class UpdateRateBasedRuleResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRegexMatchSetResponseTypeDef

```python
# UpdateRegexMatchSetResponseTypeDef definition

class UpdateRegexMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRegexPatternSetResponseTypeDef

```python
# UpdateRegexPatternSetResponseTypeDef definition

class UpdateRegexPatternSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRuleGroupResponseTypeDef

```python
# UpdateRuleGroupResponseTypeDef definition

class UpdateRuleGroupResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRuleResponseTypeDef

```python
# UpdateRuleResponseTypeDef definition

class UpdateRuleResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSizeConstraintSetResponseTypeDef

```python
# UpdateSizeConstraintSetResponseTypeDef definition

class UpdateSizeConstraintSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSqlInjectionMatchSetResponseTypeDef

```python
# UpdateSqlInjectionMatchSetResponseTypeDef definition

class UpdateSqlInjectionMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWebACLResponseTypeDef

```python
# UpdateWebACLResponseTypeDef definition

class UpdateWebACLResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateXssMatchSetResponseTypeDef

```python
# UpdateXssMatchSetResponseTypeDef definition

class UpdateXssMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRateBasedRuleRequestRequestTypeDef

```python
# CreateRateBasedRuleRequestRequestTypeDef definition

class CreateRateBasedRuleRequestRequestTypeDef(TypedDict):
    Name: str,
    MetricName: str,
    RateKey: RateKeyType,  # (1)
    RateLimit: int,
    ChangeToken: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: RateKeyType](./literals.md#ratekeytype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRuleGroupRequestRequestTypeDef

```python
# CreateRuleGroupRequestRequestTypeDef definition

class CreateRuleGroupRequestRequestTypeDef(TypedDict):
    Name: str,
    MetricName: str,
    ChangeToken: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRuleRequestRequestTypeDef

```python
# CreateRuleRequestRequestTypeDef definition

class CreateRuleRequestRequestTypeDef(TypedDict):
    Name: str,
    MetricName: str,
    ChangeToken: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateWebACLRequestRequestTypeDef

```python
# CreateWebACLRequestRequestTypeDef definition

class CreateWebACLRequestRequestTypeDef(TypedDict):
    Name: str,
    MetricName: str,
    DefaultAction: WafActionTypeDef,  # (1)
    ChangeToken: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: WafActionTypeDef](./type_defs.md#wafactiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagInfoForResourceTypeDef

```python
# TagInfoForResourceTypeDef definition

class TagInfoForResourceTypeDef(TypedDict):
    ResourceARN: NotRequired[str],
    TagList: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRegexPatternSetResponseTypeDef

```python
# CreateRegexPatternSetResponseTypeDef definition

class CreateRegexPatternSetResponseTypeDef(TypedDict):
    RegexPatternSet: RegexPatternSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexPatternSetTypeDef](./type_defs.md#regexpatternsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRegexPatternSetResponseTypeDef

```python
# GetRegexPatternSetResponseTypeDef definition

class GetRegexPatternSetResponseTypeDef(TypedDict):
    RegexPatternSet: RegexPatternSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexPatternSetTypeDef](./type_defs.md#regexpatternsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleGroupResponseTypeDef

```python
# CreateRuleGroupResponseTypeDef definition

class CreateRuleGroupResponseTypeDef(TypedDict):
    RuleGroup: RuleGroupTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupTypeDef](./type_defs.md#rulegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRuleGroupResponseTypeDef

```python
# GetRuleGroupResponseTypeDef definition

class GetRuleGroupResponseTypeDef(TypedDict):
    RuleGroup: RuleGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupTypeDef](./type_defs.md#rulegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GeoMatchSetTypeDef

```python
# GeoMatchSetTypeDef definition

class GeoMatchSetTypeDef(TypedDict):
    GeoMatchSetId: str,
    GeoMatchConstraints: List[GeoMatchConstraintTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: GeoMatchConstraintTypeDef](./type_defs.md#geomatchconstrainttypedef) 
## GeoMatchSetUpdateTypeDef

```python
# GeoMatchSetUpdateTypeDef definition

class GeoMatchSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    GeoMatchConstraint: GeoMatchConstraintTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: GeoMatchConstraintTypeDef](./type_defs.md#geomatchconstrainttypedef) 
## ListGeoMatchSetsResponseTypeDef

```python
# ListGeoMatchSetsResponseTypeDef definition

class ListGeoMatchSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    GeoMatchSets: List[GeoMatchSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeoMatchSetSummaryTypeDef](./type_defs.md#geomatchsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWebACLForResourceResponseTypeDef

```python
# GetWebACLForResourceResponseTypeDef definition

class GetWebACLForResourceResponseTypeDef(TypedDict):
    WebACLSummary: WebACLSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebACLSummaryTypeDef](./type_defs.md#webaclsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWebACLsResponseTypeDef

```python
# ListWebACLsResponseTypeDef definition

class ListWebACLsResponseTypeDef(TypedDict):
    NextMarker: str,
    WebACLs: List[WebACLSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebACLSummaryTypeDef](./type_defs.md#webaclsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HTTPRequestTypeDef

```python
# HTTPRequestTypeDef definition

class HTTPRequestTypeDef(TypedDict):
    ClientIP: NotRequired[str],
    Country: NotRequired[str],
    URI: NotRequired[str],
    Method: NotRequired[str],
    HTTPVersion: NotRequired[str],
    Headers: NotRequired[List[HTTPHeaderTypeDef]],  # (1)
```

1. See [:material-code-braces: HTTPHeaderTypeDef](./type_defs.md#httpheadertypedef) 
## IPSetTypeDef

```python
# IPSetTypeDef definition

class IPSetTypeDef(TypedDict):
    IPSetId: str,
    IPSetDescriptors: List[IPSetDescriptorTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: IPSetDescriptorTypeDef](./type_defs.md#ipsetdescriptortypedef) 
## IPSetUpdateTypeDef

```python
# IPSetUpdateTypeDef definition

class IPSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    IPSetDescriptor: IPSetDescriptorTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: IPSetDescriptorTypeDef](./type_defs.md#ipsetdescriptortypedef) 
## ListIPSetsResponseTypeDef

```python
# ListIPSetsResponseTypeDef definition

class ListIPSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    IPSets: List[IPSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IPSetSummaryTypeDef](./type_defs.md#ipsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRateBasedRulesResponseTypeDef

```python
# ListRateBasedRulesResponseTypeDef definition

class ListRateBasedRulesResponseTypeDef(TypedDict):
    NextMarker: str,
    Rules: List[RuleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRulesResponseTypeDef

```python
# ListRulesResponseTypeDef definition

class ListRulesResponseTypeDef(TypedDict):
    NextMarker: str,
    Rules: List[RuleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRegexMatchSetsResponseTypeDef

```python
# ListRegexMatchSetsResponseTypeDef definition

class ListRegexMatchSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    RegexMatchSets: List[RegexMatchSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexMatchSetSummaryTypeDef](./type_defs.md#regexmatchsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRegexPatternSetsResponseTypeDef

```python
# ListRegexPatternSetsResponseTypeDef definition

class ListRegexPatternSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    RegexPatternSets: List[RegexPatternSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexPatternSetSummaryTypeDef](./type_defs.md#regexpatternsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRuleGroupsResponseTypeDef

```python
# ListRuleGroupsResponseTypeDef definition

class ListRuleGroupsResponseTypeDef(TypedDict):
    NextMarker: str,
    RuleGroups: List[RuleGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupSummaryTypeDef](./type_defs.md#rulegroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSizeConstraintSetsResponseTypeDef

```python
# ListSizeConstraintSetsResponseTypeDef definition

class ListSizeConstraintSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    SizeConstraintSets: List[SizeConstraintSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SizeConstraintSetSummaryTypeDef](./type_defs.md#sizeconstraintsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSqlInjectionMatchSetsResponseTypeDef

```python
# ListSqlInjectionMatchSetsResponseTypeDef definition

class ListSqlInjectionMatchSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    SqlInjectionMatchSets: List[SqlInjectionMatchSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SqlInjectionMatchSetSummaryTypeDef](./type_defs.md#sqlinjectionmatchsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSubscribedRuleGroupsResponseTypeDef

```python
# ListSubscribedRuleGroupsResponseTypeDef definition

class ListSubscribedRuleGroupsResponseTypeDef(TypedDict):
    NextMarker: str,
    RuleGroups: List[SubscribedRuleGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscribedRuleGroupSummaryTypeDef](./type_defs.md#subscribedrulegroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListXssMatchSetsResponseTypeDef

```python
# ListXssMatchSetsResponseTypeDef definition

class ListXssMatchSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    XssMatchSets: List[XssMatchSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: XssMatchSetSummaryTypeDef](./type_defs.md#xssmatchsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RateBasedRuleTypeDef

```python
# RateBasedRuleTypeDef definition

class RateBasedRuleTypeDef(TypedDict):
    RuleId: str,
    MatchPredicates: List[PredicateTypeDef],  # (1)
    RateKey: RateKeyType,  # (2)
    RateLimit: int,
    Name: NotRequired[str],
    MetricName: NotRequired[str],
```

1. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
2. See [:material-code-brackets: RateKeyType](./literals.md#ratekeytype) 
## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    RuleId: str,
    Predicates: List[PredicateTypeDef],  # (1)
    Name: NotRequired[str],
    MetricName: NotRequired[str],
```

1. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
## RuleUpdateTypeDef

```python
# RuleUpdateTypeDef definition

class RuleUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    Predicate: PredicateTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
## UpdateRegexPatternSetRequestRequestTypeDef

```python
# UpdateRegexPatternSetRequestRequestTypeDef definition

class UpdateRegexPatternSetRequestRequestTypeDef(TypedDict):
    RegexPatternSetId: str,
    Updates: Sequence[RegexPatternSetUpdateTypeDef],  # (1)
    ChangeToken: str,
```

1. See [:material-code-braces: RegexPatternSetUpdateTypeDef](./type_defs.md#regexpatternsetupdatetypedef) 
## TimeWindowTypeDef

```python
# TimeWindowTypeDef definition

class TimeWindowTypeDef(TypedDict):
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
```

## ListActivatedRulesInRuleGroupResponseTypeDef

```python
# ListActivatedRulesInRuleGroupResponseTypeDef definition

class ListActivatedRulesInRuleGroupResponseTypeDef(TypedDict):
    NextMarker: str,
    ActivatedRules: List[ActivatedRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActivatedRuleTypeDef](./type_defs.md#activatedruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleGroupUpdateTypeDef

```python
# RuleGroupUpdateTypeDef definition

class RuleGroupUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    ActivatedRule: ActivatedRuleTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: ActivatedRuleTypeDef](./type_defs.md#activatedruletypedef) 
## WebACLTypeDef

```python
# WebACLTypeDef definition

class WebACLTypeDef(TypedDict):
    WebACLId: str,
    DefaultAction: WafActionTypeDef,  # (1)
    Rules: List[ActivatedRuleTypeDef],  # (2)
    Name: NotRequired[str],
    MetricName: NotRequired[str],
    WebACLArn: NotRequired[str],
```

1. See [:material-code-braces: WafActionTypeDef](./type_defs.md#wafactiontypedef) 
2. See [:material-code-braces: ActivatedRuleTypeDef](./type_defs.md#activatedruletypedef) 
## WebACLUpdateTypeDef

```python
# WebACLUpdateTypeDef definition

class WebACLUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    ActivatedRule: ActivatedRuleTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: ActivatedRuleTypeDef](./type_defs.md#activatedruletypedef) 
## ByteMatchSetTypeDef

```python
# ByteMatchSetTypeDef definition

class ByteMatchSetTypeDef(TypedDict):
    ByteMatchSetId: str,
    ByteMatchTuples: List[ByteMatchTupleTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: ByteMatchTupleTypeDef](./type_defs.md#bytematchtupletypedef) 
## ByteMatchSetUpdateTypeDef

```python
# ByteMatchSetUpdateTypeDef definition

class ByteMatchSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    ByteMatchTuple: ByteMatchTupleTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: ByteMatchTupleTypeDef](./type_defs.md#bytematchtupletypedef) 
## GetLoggingConfigurationResponseTypeDef

```python
# GetLoggingConfigurationResponseTypeDef definition

class GetLoggingConfigurationResponseTypeDef(TypedDict):
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLoggingConfigurationsResponseTypeDef

```python
# ListLoggingConfigurationsResponseTypeDef definition

class ListLoggingConfigurationsResponseTypeDef(TypedDict):
    LoggingConfigurations: List[LoggingConfigurationTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutLoggingConfigurationRequestRequestTypeDef

```python
# PutLoggingConfigurationRequestRequestTypeDef definition

class PutLoggingConfigurationRequestRequestTypeDef(TypedDict):
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
## PutLoggingConfigurationResponseTypeDef

```python
# PutLoggingConfigurationResponseTypeDef definition

class PutLoggingConfigurationResponseTypeDef(TypedDict):
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegexMatchSetTypeDef

```python
# RegexMatchSetTypeDef definition

class RegexMatchSetTypeDef(TypedDict):
    RegexMatchSetId: NotRequired[str],
    Name: NotRequired[str],
    RegexMatchTuples: NotRequired[List[RegexMatchTupleTypeDef]],  # (1)
```

1. See [:material-code-braces: RegexMatchTupleTypeDef](./type_defs.md#regexmatchtupletypedef) 
## RegexMatchSetUpdateTypeDef

```python
# RegexMatchSetUpdateTypeDef definition

class RegexMatchSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    RegexMatchTuple: RegexMatchTupleTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: RegexMatchTupleTypeDef](./type_defs.md#regexmatchtupletypedef) 
## SizeConstraintSetTypeDef

```python
# SizeConstraintSetTypeDef definition

class SizeConstraintSetTypeDef(TypedDict):
    SizeConstraintSetId: str,
    SizeConstraints: List[SizeConstraintTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: SizeConstraintTypeDef](./type_defs.md#sizeconstrainttypedef) 
## SizeConstraintSetUpdateTypeDef

```python
# SizeConstraintSetUpdateTypeDef definition

class SizeConstraintSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    SizeConstraint: SizeConstraintTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: SizeConstraintTypeDef](./type_defs.md#sizeconstrainttypedef) 
## SqlInjectionMatchSetTypeDef

```python
# SqlInjectionMatchSetTypeDef definition

class SqlInjectionMatchSetTypeDef(TypedDict):
    SqlInjectionMatchSetId: str,
    SqlInjectionMatchTuples: List[SqlInjectionMatchTupleTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: SqlInjectionMatchTupleTypeDef](./type_defs.md#sqlinjectionmatchtupletypedef) 
## SqlInjectionMatchSetUpdateTypeDef

```python
# SqlInjectionMatchSetUpdateTypeDef definition

class SqlInjectionMatchSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    SqlInjectionMatchTuple: SqlInjectionMatchTupleTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: SqlInjectionMatchTupleTypeDef](./type_defs.md#sqlinjectionmatchtupletypedef) 
## XssMatchSetTypeDef

```python
# XssMatchSetTypeDef definition

class XssMatchSetTypeDef(TypedDict):
    XssMatchSetId: str,
    XssMatchTuples: List[XssMatchTupleTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: XssMatchTupleTypeDef](./type_defs.md#xssmatchtupletypedef) 
## XssMatchSetUpdateTypeDef

```python
# XssMatchSetUpdateTypeDef definition

class XssMatchSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    XssMatchTuple: XssMatchTupleTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: XssMatchTupleTypeDef](./type_defs.md#xssmatchtupletypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    NextMarker: str,
    TagInfoForResource: TagInfoForResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagInfoForResourceTypeDef](./type_defs.md#taginfoforresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGeoMatchSetResponseTypeDef

```python
# CreateGeoMatchSetResponseTypeDef definition

class CreateGeoMatchSetResponseTypeDef(TypedDict):
    GeoMatchSet: GeoMatchSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeoMatchSetTypeDef](./type_defs.md#geomatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGeoMatchSetResponseTypeDef

```python
# GetGeoMatchSetResponseTypeDef definition

class GetGeoMatchSetResponseTypeDef(TypedDict):
    GeoMatchSet: GeoMatchSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeoMatchSetTypeDef](./type_defs.md#geomatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGeoMatchSetRequestRequestTypeDef

```python
# UpdateGeoMatchSetRequestRequestTypeDef definition

class UpdateGeoMatchSetRequestRequestTypeDef(TypedDict):
    GeoMatchSetId: str,
    ChangeToken: str,
    Updates: Sequence[GeoMatchSetUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: GeoMatchSetUpdateTypeDef](./type_defs.md#geomatchsetupdatetypedef) 
## SampledHTTPRequestTypeDef

```python
# SampledHTTPRequestTypeDef definition

class SampledHTTPRequestTypeDef(TypedDict):
    Request: HTTPRequestTypeDef,  # (1)
    Weight: int,
    Timestamp: NotRequired[datetime],
    Action: NotRequired[str],
    RuleWithinRuleGroup: NotRequired[str],
```

1. See [:material-code-braces: HTTPRequestTypeDef](./type_defs.md#httprequesttypedef) 
## CreateIPSetResponseTypeDef

```python
# CreateIPSetResponseTypeDef definition

class CreateIPSetResponseTypeDef(TypedDict):
    IPSet: IPSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IPSetTypeDef](./type_defs.md#ipsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIPSetResponseTypeDef

```python
# GetIPSetResponseTypeDef definition

class GetIPSetResponseTypeDef(TypedDict):
    IPSet: IPSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IPSetTypeDef](./type_defs.md#ipsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIPSetRequestRequestTypeDef

```python
# UpdateIPSetRequestRequestTypeDef definition

class UpdateIPSetRequestRequestTypeDef(TypedDict):
    IPSetId: str,
    ChangeToken: str,
    Updates: Sequence[IPSetUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: IPSetUpdateTypeDef](./type_defs.md#ipsetupdatetypedef) 
## CreateRateBasedRuleResponseTypeDef

```python
# CreateRateBasedRuleResponseTypeDef definition

class CreateRateBasedRuleResponseTypeDef(TypedDict):
    Rule: RateBasedRuleTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RateBasedRuleTypeDef](./type_defs.md#ratebasedruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRateBasedRuleResponseTypeDef

```python
# GetRateBasedRuleResponseTypeDef definition

class GetRateBasedRuleResponseTypeDef(TypedDict):
    Rule: RateBasedRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RateBasedRuleTypeDef](./type_defs.md#ratebasedruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleResponseTypeDef

```python
# CreateRuleResponseTypeDef definition

class CreateRuleResponseTypeDef(TypedDict):
    Rule: RuleTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRuleResponseTypeDef

```python
# GetRuleResponseTypeDef definition

class GetRuleResponseTypeDef(TypedDict):
    Rule: RuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRateBasedRuleRequestRequestTypeDef

```python
# UpdateRateBasedRuleRequestRequestTypeDef definition

class UpdateRateBasedRuleRequestRequestTypeDef(TypedDict):
    RuleId: str,
    ChangeToken: str,
    Updates: Sequence[RuleUpdateTypeDef],  # (1)
    RateLimit: int,
```

1. See [:material-code-braces: RuleUpdateTypeDef](./type_defs.md#ruleupdatetypedef) 
## UpdateRuleRequestRequestTypeDef

```python
# UpdateRuleRequestRequestTypeDef definition

class UpdateRuleRequestRequestTypeDef(TypedDict):
    RuleId: str,
    ChangeToken: str,
    Updates: Sequence[RuleUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: RuleUpdateTypeDef](./type_defs.md#ruleupdatetypedef) 
## GetSampledRequestsRequestRequestTypeDef

```python
# GetSampledRequestsRequestRequestTypeDef definition

class GetSampledRequestsRequestRequestTypeDef(TypedDict):
    WebAclId: str,
    RuleId: str,
    TimeWindow: TimeWindowTypeDef,  # (1)
    MaxItems: int,
```

1. See [:material-code-braces: TimeWindowTypeDef](./type_defs.md#timewindowtypedef) 
## UpdateRuleGroupRequestRequestTypeDef

```python
# UpdateRuleGroupRequestRequestTypeDef definition

class UpdateRuleGroupRequestRequestTypeDef(TypedDict):
    RuleGroupId: str,
    Updates: Sequence[RuleGroupUpdateTypeDef],  # (1)
    ChangeToken: str,
```

1. See [:material-code-braces: RuleGroupUpdateTypeDef](./type_defs.md#rulegroupupdatetypedef) 
## CreateWebACLResponseTypeDef

```python
# CreateWebACLResponseTypeDef definition

class CreateWebACLResponseTypeDef(TypedDict):
    WebACL: WebACLTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebACLTypeDef](./type_defs.md#webacltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWebACLResponseTypeDef

```python
# GetWebACLResponseTypeDef definition

class GetWebACLResponseTypeDef(TypedDict):
    WebACL: WebACLTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebACLTypeDef](./type_defs.md#webacltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWebACLRequestRequestTypeDef

```python
# UpdateWebACLRequestRequestTypeDef definition

class UpdateWebACLRequestRequestTypeDef(TypedDict):
    WebACLId: str,
    ChangeToken: str,
    Updates: NotRequired[Sequence[WebACLUpdateTypeDef]],  # (1)
    DefaultAction: NotRequired[WafActionTypeDef],  # (2)
```

1. See [:material-code-braces: WebACLUpdateTypeDef](./type_defs.md#webaclupdatetypedef) 
2. See [:material-code-braces: WafActionTypeDef](./type_defs.md#wafactiontypedef) 
## CreateByteMatchSetResponseTypeDef

```python
# CreateByteMatchSetResponseTypeDef definition

class CreateByteMatchSetResponseTypeDef(TypedDict):
    ByteMatchSet: ByteMatchSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ByteMatchSetTypeDef](./type_defs.md#bytematchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetByteMatchSetResponseTypeDef

```python
# GetByteMatchSetResponseTypeDef definition

class GetByteMatchSetResponseTypeDef(TypedDict):
    ByteMatchSet: ByteMatchSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ByteMatchSetTypeDef](./type_defs.md#bytematchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateByteMatchSetRequestRequestTypeDef

```python
# UpdateByteMatchSetRequestRequestTypeDef definition

class UpdateByteMatchSetRequestRequestTypeDef(TypedDict):
    ByteMatchSetId: str,
    ChangeToken: str,
    Updates: Sequence[ByteMatchSetUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: ByteMatchSetUpdateTypeDef](./type_defs.md#bytematchsetupdatetypedef) 
## CreateRegexMatchSetResponseTypeDef

```python
# CreateRegexMatchSetResponseTypeDef definition

class CreateRegexMatchSetResponseTypeDef(TypedDict):
    RegexMatchSet: RegexMatchSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexMatchSetTypeDef](./type_defs.md#regexmatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRegexMatchSetResponseTypeDef

```python
# GetRegexMatchSetResponseTypeDef definition

class GetRegexMatchSetResponseTypeDef(TypedDict):
    RegexMatchSet: RegexMatchSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexMatchSetTypeDef](./type_defs.md#regexmatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRegexMatchSetRequestRequestTypeDef

```python
# UpdateRegexMatchSetRequestRequestTypeDef definition

class UpdateRegexMatchSetRequestRequestTypeDef(TypedDict):
    RegexMatchSetId: str,
    Updates: Sequence[RegexMatchSetUpdateTypeDef],  # (1)
    ChangeToken: str,
```

1. See [:material-code-braces: RegexMatchSetUpdateTypeDef](./type_defs.md#regexmatchsetupdatetypedef) 
## CreateSizeConstraintSetResponseTypeDef

```python
# CreateSizeConstraintSetResponseTypeDef definition

class CreateSizeConstraintSetResponseTypeDef(TypedDict):
    SizeConstraintSet: SizeConstraintSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SizeConstraintSetTypeDef](./type_defs.md#sizeconstraintsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSizeConstraintSetResponseTypeDef

```python
# GetSizeConstraintSetResponseTypeDef definition

class GetSizeConstraintSetResponseTypeDef(TypedDict):
    SizeConstraintSet: SizeConstraintSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SizeConstraintSetTypeDef](./type_defs.md#sizeconstraintsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSizeConstraintSetRequestRequestTypeDef

```python
# UpdateSizeConstraintSetRequestRequestTypeDef definition

class UpdateSizeConstraintSetRequestRequestTypeDef(TypedDict):
    SizeConstraintSetId: str,
    ChangeToken: str,
    Updates: Sequence[SizeConstraintSetUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: SizeConstraintSetUpdateTypeDef](./type_defs.md#sizeconstraintsetupdatetypedef) 
## CreateSqlInjectionMatchSetResponseTypeDef

```python
# CreateSqlInjectionMatchSetResponseTypeDef definition

class CreateSqlInjectionMatchSetResponseTypeDef(TypedDict):
    SqlInjectionMatchSet: SqlInjectionMatchSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SqlInjectionMatchSetTypeDef](./type_defs.md#sqlinjectionmatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSqlInjectionMatchSetResponseTypeDef

```python
# GetSqlInjectionMatchSetResponseTypeDef definition

class GetSqlInjectionMatchSetResponseTypeDef(TypedDict):
    SqlInjectionMatchSet: SqlInjectionMatchSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SqlInjectionMatchSetTypeDef](./type_defs.md#sqlinjectionmatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSqlInjectionMatchSetRequestRequestTypeDef

```python
# UpdateSqlInjectionMatchSetRequestRequestTypeDef definition

class UpdateSqlInjectionMatchSetRequestRequestTypeDef(TypedDict):
    SqlInjectionMatchSetId: str,
    ChangeToken: str,
    Updates: Sequence[SqlInjectionMatchSetUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: SqlInjectionMatchSetUpdateTypeDef](./type_defs.md#sqlinjectionmatchsetupdatetypedef) 
## CreateXssMatchSetResponseTypeDef

```python
# CreateXssMatchSetResponseTypeDef definition

class CreateXssMatchSetResponseTypeDef(TypedDict):
    XssMatchSet: XssMatchSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: XssMatchSetTypeDef](./type_defs.md#xssmatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetXssMatchSetResponseTypeDef

```python
# GetXssMatchSetResponseTypeDef definition

class GetXssMatchSetResponseTypeDef(TypedDict):
    XssMatchSet: XssMatchSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: XssMatchSetTypeDef](./type_defs.md#xssmatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateXssMatchSetRequestRequestTypeDef

```python
# UpdateXssMatchSetRequestRequestTypeDef definition

class UpdateXssMatchSetRequestRequestTypeDef(TypedDict):
    XssMatchSetId: str,
    ChangeToken: str,
    Updates: Sequence[XssMatchSetUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: XssMatchSetUpdateTypeDef](./type_defs.md#xssmatchsetupdatetypedef) 
## GetSampledRequestsResponseTypeDef

```python
# GetSampledRequestsResponseTypeDef definition

class GetSampledRequestsResponseTypeDef(TypedDict):
    SampledRequests: List[SampledHTTPRequestTypeDef],  # (1)
    PopulationSize: int,
    TimeWindow: TimeWindowTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SampledHTTPRequestTypeDef](./type_defs.md#sampledhttprequesttypedef) 
2. See [:material-code-braces: TimeWindowTypeDef](./type_defs.md#timewindowtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
