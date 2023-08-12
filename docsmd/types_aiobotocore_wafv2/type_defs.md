# Type definitions

> [Index](../README.md) > [WAFV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [WAFV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
    type annotations stubs module [types-aiobotocore-wafv2](https://pypi.org/project/types-aiobotocore-wafv2/).

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




## APIKeySummaryTypeDef

```python
# APIKeySummaryTypeDef definition

class APIKeySummaryTypeDef(TypedDict):
    TokenDomains: NotRequired[List[str]],
    APIKey: NotRequired[str],
    CreationTimestamp: NotRequired[datetime],
    Version: NotRequired[int],
```

## AWSManagedRulesBotControlRuleSetTypeDef

```python
# AWSManagedRulesBotControlRuleSetTypeDef definition

class AWSManagedRulesBotControlRuleSetTypeDef(TypedDict):
    InspectionLevel: InspectionLevelType,  # (1)
```

1. See [:material-code-brackets: InspectionLevelType](./literals.md#inspectionleveltype) 
## ActionConditionTypeDef

```python
# ActionConditionTypeDef definition

class ActionConditionTypeDef(TypedDict):
    Action: ActionValueType,  # (1)
```

1. See [:material-code-brackets: ActionValueType](./literals.md#actionvaluetype) 
## AddressFieldTypeDef

```python
# AddressFieldTypeDef definition

class AddressFieldTypeDef(TypedDict):
    Identifier: str,
```

## AndStatementTypeDef

```python
# AndStatementTypeDef definition

class AndStatementTypeDef(TypedDict):
    Statements: Sequence[StatementTypeDef],  # (1)
```

1. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
## AssociateWebACLRequestRequestTypeDef

```python
# AssociateWebACLRequestRequestTypeDef definition

class AssociateWebACLRequestRequestTypeDef(TypedDict):
    WebACLArn: str,
    ResourceArn: str,
```

## RequestBodyAssociatedResourceTypeConfigTypeDef

```python
# RequestBodyAssociatedResourceTypeConfigTypeDef definition

class RequestBodyAssociatedResourceTypeConfigTypeDef(TypedDict):
    DefaultSizeInspectionLimit: SizeInspectionLimitType,  # (1)
```

1. See [:material-code-brackets: SizeInspectionLimitType](./literals.md#sizeinspectionlimittype) 
## BodyTypeDef

```python
# BodyTypeDef definition

class BodyTypeDef(TypedDict):
    OversizeHandling: NotRequired[OversizeHandlingType],  # (1)
```

1. See [:material-code-brackets: OversizeHandlingType](./literals.md#oversizehandlingtype) 
## TextTransformationTypeDef

```python
# TextTransformationTypeDef definition

class TextTransformationTypeDef(TypedDict):
    Priority: int,
    Type: TextTransformationTypeType,  # (1)
```

1. See [:material-code-brackets: TextTransformationTypeType](./literals.md#texttransformationtypetype) 
## ImmunityTimePropertyTypeDef

```python
# ImmunityTimePropertyTypeDef definition

class ImmunityTimePropertyTypeDef(TypedDict):
    ImmunityTime: int,
```

## CaptchaResponseTypeDef

```python
# CaptchaResponseTypeDef definition

class CaptchaResponseTypeDef(TypedDict):
    ResponseCode: NotRequired[int],
    SolveTimestamp: NotRequired[int],
    FailureReason: NotRequired[FailureReasonType],  # (1)
```

1. See [:material-code-brackets: FailureReasonType](./literals.md#failurereasontype) 
## ChallengeResponseTypeDef

```python
# ChallengeResponseTypeDef definition

class ChallengeResponseTypeDef(TypedDict):
    ResponseCode: NotRequired[int],
    SolveTimestamp: NotRequired[int],
    FailureReason: NotRequired[FailureReasonType],  # (1)
```

1. See [:material-code-brackets: FailureReasonType](./literals.md#failurereasontype) 
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

## LabelNameConditionTypeDef

```python
# LabelNameConditionTypeDef definition

class LabelNameConditionTypeDef(TypedDict):
    LabelName: str,
```

## CookieMatchPatternTypeDef

```python
# CookieMatchPatternTypeDef definition

class CookieMatchPatternTypeDef(TypedDict):
    All: NotRequired[Mapping[str, Any]],
    IncludedCookies: NotRequired[Sequence[str]],
    ExcludedCookies: NotRequired[Sequence[str]],
```

## CreateAPIKeyRequestRequestTypeDef

```python
# CreateAPIKeyRequestRequestTypeDef definition

class CreateAPIKeyRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
    TokenDomains: Sequence[str],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## IPSetSummaryTypeDef

```python
# IPSetSummaryTypeDef definition

class IPSetSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    Id: NotRequired[str],
    Description: NotRequired[str],
    LockToken: NotRequired[str],
    ARN: NotRequired[str],
```

## RegexTypeDef

```python
# RegexTypeDef definition

class RegexTypeDef(TypedDict):
    RegexString: NotRequired[str],
```

## RegexPatternSetSummaryTypeDef

```python
# RegexPatternSetSummaryTypeDef definition

class RegexPatternSetSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    Id: NotRequired[str],
    Description: NotRequired[str],
    LockToken: NotRequired[str],
    ARN: NotRequired[str],
```

## CustomResponseBodyTypeDef

```python
# CustomResponseBodyTypeDef definition

class CustomResponseBodyTypeDef(TypedDict):
    ContentType: ResponseContentTypeType,  # (1)
    Content: str,
```

1. See [:material-code-brackets: ResponseContentTypeType](./literals.md#responsecontenttypetype) 
## VisibilityConfigTypeDef

```python
# VisibilityConfigTypeDef definition

class VisibilityConfigTypeDef(TypedDict):
    SampledRequestsEnabled: bool,
    CloudWatchMetricsEnabled: bool,
    MetricName: str,
```

## RuleGroupSummaryTypeDef

```python
# RuleGroupSummaryTypeDef definition

class RuleGroupSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    Id: NotRequired[str],
    Description: NotRequired[str],
    LockToken: NotRequired[str],
    ARN: NotRequired[str],
```

## WebACLSummaryTypeDef

```python
# WebACLSummaryTypeDef definition

class WebACLSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    Id: NotRequired[str],
    Description: NotRequired[str],
    LockToken: NotRequired[str],
    ARN: NotRequired[str],
```

## CustomHTTPHeaderTypeDef

```python
# CustomHTTPHeaderTypeDef definition

class CustomHTTPHeaderTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## DeleteFirewallManagerRuleGroupsRequestRequestTypeDef

```python
# DeleteFirewallManagerRuleGroupsRequestRequestTypeDef definition

class DeleteFirewallManagerRuleGroupsRequestRequestTypeDef(TypedDict):
    WebACLArn: str,
    WebACLLockToken: str,
```

## DeleteIPSetRequestRequestTypeDef

```python
# DeleteIPSetRequestRequestTypeDef definition

class DeleteIPSetRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
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

## DeleteRegexPatternSetRequestRequestTypeDef

```python
# DeleteRegexPatternSetRequestRequestTypeDef definition

class DeleteRegexPatternSetRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## DeleteRuleGroupRequestRequestTypeDef

```python
# DeleteRuleGroupRequestRequestTypeDef definition

class DeleteRuleGroupRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## DeleteWebACLRequestRequestTypeDef

```python
# DeleteWebACLRequestRequestTypeDef definition

class DeleteWebACLRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## DescribeAllManagedProductsRequestRequestTypeDef

```python
# DescribeAllManagedProductsRequestRequestTypeDef definition

class DescribeAllManagedProductsRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## ManagedProductDescriptorTypeDef

```python
# ManagedProductDescriptorTypeDef definition

class ManagedProductDescriptorTypeDef(TypedDict):
    VendorName: NotRequired[str],
    ManagedRuleSetName: NotRequired[str],
    ProductId: NotRequired[str],
    ProductLink: NotRequired[str],
    ProductTitle: NotRequired[str],
    ProductDescription: NotRequired[str],
    SnsTopicArn: NotRequired[str],
    IsVersioningSupported: NotRequired[bool],
    IsAdvancedManagedRuleSet: NotRequired[bool],
```

## DescribeManagedProductsByVendorRequestRequestTypeDef

```python
# DescribeManagedProductsByVendorRequestRequestTypeDef definition

class DescribeManagedProductsByVendorRequestRequestTypeDef(TypedDict):
    VendorName: str,
    Scope: ScopeType,  # (1)
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## DescribeManagedRuleGroupRequestRequestTypeDef

```python
# DescribeManagedRuleGroupRequestRequestTypeDef definition

class DescribeManagedRuleGroupRequestRequestTypeDef(TypedDict):
    VendorName: str,
    Name: str,
    Scope: ScopeType,  # (1)
    VersionName: NotRequired[str],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## LabelSummaryTypeDef

```python
# LabelSummaryTypeDef definition

class LabelSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
```

## DisassociateWebACLRequestRequestTypeDef

```python
# DisassociateWebACLRequestRequestTypeDef definition

class DisassociateWebACLRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## EmailFieldTypeDef

```python
# EmailFieldTypeDef definition

class EmailFieldTypeDef(TypedDict):
    Identifier: str,
```

## ExcludedRuleTypeDef

```python
# ExcludedRuleTypeDef definition

class ExcludedRuleTypeDef(TypedDict):
    Name: str,
```

## HeaderOrderTypeDef

```python
# HeaderOrderTypeDef definition

class HeaderOrderTypeDef(TypedDict):
    OversizeHandling: OversizeHandlingType,  # (1)
```

1. See [:material-code-brackets: OversizeHandlingType](./literals.md#oversizehandlingtype) 
## SingleHeaderTypeDef

```python
# SingleHeaderTypeDef definition

class SingleHeaderTypeDef(TypedDict):
    Name: str,
```

## SingleQueryArgumentTypeDef

```python
# SingleQueryArgumentTypeDef definition

class SingleQueryArgumentTypeDef(TypedDict):
    Name: str,
```

## ForwardedIPConfigTypeDef

```python
# ForwardedIPConfigTypeDef definition

class ForwardedIPConfigTypeDef(TypedDict):
    HeaderName: str,
    FallbackBehavior: FallbackBehaviorType,  # (1)
```

1. See [:material-code-brackets: FallbackBehaviorType](./literals.md#fallbackbehaviortype) 
## GenerateMobileSdkReleaseUrlRequestRequestTypeDef

```python
# GenerateMobileSdkReleaseUrlRequestRequestTypeDef definition

class GenerateMobileSdkReleaseUrlRequestRequestTypeDef(TypedDict):
    Platform: PlatformType,  # (1)
    ReleaseVersion: str,
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
## GetDecryptedAPIKeyRequestRequestTypeDef

```python
# GetDecryptedAPIKeyRequestRequestTypeDef definition

class GetDecryptedAPIKeyRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
    APIKey: str,
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## GetIPSetRequestRequestTypeDef

```python
# GetIPSetRequestRequestTypeDef definition

class GetIPSetRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## IPSetTypeDef

```python
# IPSetTypeDef definition

class IPSetTypeDef(TypedDict):
    Name: str,
    Id: str,
    ARN: str,
    IPAddressVersion: IPAddressVersionType,  # (1)
    Addresses: List[str],
    Description: NotRequired[str],
```

1. See [:material-code-brackets: IPAddressVersionType](./literals.md#ipaddressversiontype) 
## GetLoggingConfigurationRequestRequestTypeDef

```python
# GetLoggingConfigurationRequestRequestTypeDef definition

class GetLoggingConfigurationRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetManagedRuleSetRequestRequestTypeDef

```python
# GetManagedRuleSetRequestRequestTypeDef definition

class GetManagedRuleSetRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## GetMobileSdkReleaseRequestRequestTypeDef

```python
# GetMobileSdkReleaseRequestRequestTypeDef definition

class GetMobileSdkReleaseRequestRequestTypeDef(TypedDict):
    Platform: PlatformType,  # (1)
    ReleaseVersion: str,
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
## GetPermissionPolicyRequestRequestTypeDef

```python
# GetPermissionPolicyRequestRequestTypeDef definition

class GetPermissionPolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetRateBasedStatementManagedKeysRequestRequestTypeDef

```python
# GetRateBasedStatementManagedKeysRequestRequestTypeDef definition

class GetRateBasedStatementManagedKeysRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
    WebACLName: str,
    WebACLId: str,
    RuleName: str,
    RuleGroupRuleName: NotRequired[str],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## RateBasedStatementManagedKeysIPSetTypeDef

```python
# RateBasedStatementManagedKeysIPSetTypeDef definition

class RateBasedStatementManagedKeysIPSetTypeDef(TypedDict):
    IPAddressVersion: NotRequired[IPAddressVersionType],  # (1)
    Addresses: NotRequired[List[str]],
```

1. See [:material-code-brackets: IPAddressVersionType](./literals.md#ipaddressversiontype) 
## GetRegexPatternSetRequestRequestTypeDef

```python
# GetRegexPatternSetRequestRequestTypeDef definition

class GetRegexPatternSetRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## GetRuleGroupRequestRequestTypeDef

```python
# GetRuleGroupRequestRequestTypeDef definition

class GetRuleGroupRequestRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    Scope: NotRequired[ScopeType],  # (1)
    Id: NotRequired[str],
    ARN: NotRequired[str],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## GetWebACLForResourceRequestRequestTypeDef

```python
# GetWebACLForResourceRequestRequestTypeDef definition

class GetWebACLForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetWebACLRequestRequestTypeDef

```python
# GetWebACLRequestRequestTypeDef definition

class GetWebACLRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## HTTPHeaderTypeDef

```python
# HTTPHeaderTypeDef definition

class HTTPHeaderTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## HeaderMatchPatternTypeDef

```python
# HeaderMatchPatternTypeDef definition

class HeaderMatchPatternTypeDef(TypedDict):
    All: NotRequired[Mapping[str, Any]],
    IncludedHeaders: NotRequired[Sequence[str]],
    ExcludedHeaders: NotRequired[Sequence[str]],
```

## IPSetForwardedIPConfigTypeDef

```python
# IPSetForwardedIPConfigTypeDef definition

class IPSetForwardedIPConfigTypeDef(TypedDict):
    HeaderName: str,
    FallbackBehavior: FallbackBehaviorType,  # (1)
    Position: ForwardedIPPositionType,  # (2)
```

1. See [:material-code-brackets: FallbackBehaviorType](./literals.md#fallbackbehaviortype) 
2. See [:material-code-brackets: ForwardedIPPositionType](./literals.md#forwardedippositiontype) 
## JsonMatchPatternTypeDef

```python
# JsonMatchPatternTypeDef definition

class JsonMatchPatternTypeDef(TypedDict):
    All: NotRequired[Mapping[str, Any]],
    IncludedPaths: NotRequired[Sequence[str]],
```

## LabelMatchStatementTypeDef

```python
# LabelMatchStatementTypeDef definition

class LabelMatchStatementTypeDef(TypedDict):
    Scope: LabelMatchScopeType,  # (1)
    Key: str,
```

1. See [:material-code-brackets: LabelMatchScopeType](./literals.md#labelmatchscopetype) 
## LabelTypeDef

```python
# LabelTypeDef definition

class LabelTypeDef(TypedDict):
    Name: str,
```

## ListAPIKeysRequestRequestTypeDef

```python
# ListAPIKeysRequestRequestTypeDef definition

class ListAPIKeysRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef

```python
# ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef definition

class ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef(TypedDict):
    VendorName: str,
    Name: str,
    Scope: ScopeType,  # (1)
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## ManagedRuleGroupVersionTypeDef

```python
# ManagedRuleGroupVersionTypeDef definition

class ManagedRuleGroupVersionTypeDef(TypedDict):
    Name: NotRequired[str],
    LastUpdateTimestamp: NotRequired[datetime],
```

## ListAvailableManagedRuleGroupsRequestRequestTypeDef

```python
# ListAvailableManagedRuleGroupsRequestRequestTypeDef definition

class ListAvailableManagedRuleGroupsRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## ManagedRuleGroupSummaryTypeDef

```python
# ManagedRuleGroupSummaryTypeDef definition

class ManagedRuleGroupSummaryTypeDef(TypedDict):
    VendorName: NotRequired[str],
    Name: NotRequired[str],
    VersioningSupported: NotRequired[bool],
    Description: NotRequired[str],
```

## ListIPSetsRequestRequestTypeDef

```python
# ListIPSetsRequestRequestTypeDef definition

class ListIPSetsRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## ListLoggingConfigurationsRequestRequestTypeDef

```python
# ListLoggingConfigurationsRequestRequestTypeDef definition

class ListLoggingConfigurationsRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## ListManagedRuleSetsRequestRequestTypeDef

```python
# ListManagedRuleSetsRequestRequestTypeDef definition

class ListManagedRuleSetsRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## ManagedRuleSetSummaryTypeDef

```python
# ManagedRuleSetSummaryTypeDef definition

class ManagedRuleSetSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    Id: NotRequired[str],
    Description: NotRequired[str],
    LockToken: NotRequired[str],
    ARN: NotRequired[str],
    LabelNamespace: NotRequired[str],
```

## ListMobileSdkReleasesRequestRequestTypeDef

```python
# ListMobileSdkReleasesRequestRequestTypeDef definition

class ListMobileSdkReleasesRequestRequestTypeDef(TypedDict):
    Platform: PlatformType,  # (1)
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
## ReleaseSummaryTypeDef

```python
# ReleaseSummaryTypeDef definition

class ReleaseSummaryTypeDef(TypedDict):
    ReleaseVersion: NotRequired[str],
    Timestamp: NotRequired[datetime],
```

## ListRegexPatternSetsRequestRequestTypeDef

```python
# ListRegexPatternSetsRequestRequestTypeDef definition

class ListRegexPatternSetsRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## ListResourcesForWebACLRequestRequestTypeDef

```python
# ListResourcesForWebACLRequestRequestTypeDef definition

class ListResourcesForWebACLRequestRequestTypeDef(TypedDict):
    WebACLArn: str,
    ResourceType: NotRequired[ResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ListRuleGroupsRequestRequestTypeDef

```python
# ListRuleGroupsRequestRequestTypeDef definition

class ListRuleGroupsRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
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
    Scope: ScopeType,  # (1)
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## PasswordFieldTypeDef

```python
# PasswordFieldTypeDef definition

class PasswordFieldTypeDef(TypedDict):
    Identifier: str,
```

## UsernameFieldTypeDef

```python
# UsernameFieldTypeDef definition

class UsernameFieldTypeDef(TypedDict):
    Identifier: str,
```

## ManagedRuleSetVersionTypeDef

```python
# ManagedRuleSetVersionTypeDef definition

class ManagedRuleSetVersionTypeDef(TypedDict):
    AssociatedRuleGroupArn: NotRequired[str],
    Capacity: NotRequired[int],
    ForecastedLifetime: NotRequired[int],
    PublishTimestamp: NotRequired[datetime],
    LastUpdateTimestamp: NotRequired[datetime],
    ExpiryTimestamp: NotRequired[datetime],
```

## NotStatementTypeDef

```python
# NotStatementTypeDef definition

class NotStatementTypeDef(TypedDict):
    Statement: StatementTypeDef,  # (1)
```

1. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
## OrStatementTypeDef

```python
# OrStatementTypeDef definition

class OrStatementTypeDef(TypedDict):
    Statements: Sequence[StatementTypeDef],  # (1)
```

1. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
## PhoneNumberFieldTypeDef

```python
# PhoneNumberFieldTypeDef definition

class PhoneNumberFieldTypeDef(TypedDict):
    Identifier: str,
```

## VersionToPublishTypeDef

```python
# VersionToPublishTypeDef definition

class VersionToPublishTypeDef(TypedDict):
    AssociatedRuleGroupArn: NotRequired[str],
    ForecastedLifetime: NotRequired[int],
```

## PutPermissionPolicyRequestRequestTypeDef

```python
# PutPermissionPolicyRequestRequestTypeDef definition

class PutPermissionPolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
```

## RateLimitLabelNamespaceTypeDef

```python
# RateLimitLabelNamespaceTypeDef definition

class RateLimitLabelNamespaceTypeDef(TypedDict):
    Namespace: str,
```

## ResponseInspectionBodyContainsTypeDef

```python
# ResponseInspectionBodyContainsTypeDef definition

class ResponseInspectionBodyContainsTypeDef(TypedDict):
    SuccessStrings: Sequence[str],
    FailureStrings: Sequence[str],
```

## ResponseInspectionHeaderTypeDef

```python
# ResponseInspectionHeaderTypeDef definition

class ResponseInspectionHeaderTypeDef(TypedDict):
    Name: str,
    SuccessValues: Sequence[str],
    FailureValues: Sequence[str],
```

## ResponseInspectionJsonTypeDef

```python
# ResponseInspectionJsonTypeDef definition

class ResponseInspectionJsonTypeDef(TypedDict):
    Identifier: str,
    SuccessValues: Sequence[str],
    FailureValues: Sequence[str],
```

## ResponseInspectionStatusCodeTypeDef

```python
# ResponseInspectionStatusCodeTypeDef definition

class ResponseInspectionStatusCodeTypeDef(TypedDict):
    SuccessCodes: Sequence[int],
    FailureCodes: Sequence[int],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateIPSetRequestRequestTypeDef

```python
# UpdateIPSetRequestRequestTypeDef definition

class UpdateIPSetRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    Addresses: Sequence[str],
    LockToken: str,
    Description: NotRequired[str],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## AssociationConfigTypeDef

```python
# AssociationConfigTypeDef definition

class AssociationConfigTypeDef(TypedDict):
    RequestBody: NotRequired[Mapping[AssociatedResourceTypeType, RequestBodyAssociatedResourceTypeConfigTypeDef]],  # (1)
```

1. See [:material-code-brackets: AssociatedResourceTypeType](./literals.md#associatedresourcetypetype) [:material-code-braces: RequestBodyAssociatedResourceTypeConfigTypeDef](./type_defs.md#requestbodyassociatedresourcetypeconfigtypedef) 
## RateLimitCookieTypeDef

```python
# RateLimitCookieTypeDef definition

class RateLimitCookieTypeDef(TypedDict):
    Name: str,
    TextTransformations: Sequence[TextTransformationTypeDef],  # (1)
```

1. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## RateLimitHeaderTypeDef

```python
# RateLimitHeaderTypeDef definition

class RateLimitHeaderTypeDef(TypedDict):
    Name: str,
    TextTransformations: Sequence[TextTransformationTypeDef],  # (1)
```

1. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## RateLimitQueryArgumentTypeDef

```python
# RateLimitQueryArgumentTypeDef definition

class RateLimitQueryArgumentTypeDef(TypedDict):
    Name: str,
    TextTransformations: Sequence[TextTransformationTypeDef],  # (1)
```

1. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## RateLimitQueryStringTypeDef

```python
# RateLimitQueryStringTypeDef definition

class RateLimitQueryStringTypeDef(TypedDict):
    TextTransformations: Sequence[TextTransformationTypeDef],  # (1)
```

1. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## RateLimitUriPathTypeDef

```python
# RateLimitUriPathTypeDef definition

class RateLimitUriPathTypeDef(TypedDict):
    TextTransformations: Sequence[TextTransformationTypeDef],  # (1)
```

1. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## CaptchaConfigTypeDef

```python
# CaptchaConfigTypeDef definition

class CaptchaConfigTypeDef(TypedDict):
    ImmunityTimeProperty: NotRequired[ImmunityTimePropertyTypeDef],  # (1)
```

1. See [:material-code-braces: ImmunityTimePropertyTypeDef](./type_defs.md#immunitytimepropertytypedef) 
## ChallengeConfigTypeDef

```python
# ChallengeConfigTypeDef definition

class ChallengeConfigTypeDef(TypedDict):
    ImmunityTimeProperty: NotRequired[ImmunityTimePropertyTypeDef],  # (1)
```

1. See [:material-code-braces: ImmunityTimePropertyTypeDef](./type_defs.md#immunitytimepropertytypedef) 
## CheckCapacityResponseTypeDef

```python
# CheckCapacityResponseTypeDef definition

class CheckCapacityResponseTypeDef(TypedDict):
    Capacity: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAPIKeyResponseTypeDef

```python
# CreateAPIKeyResponseTypeDef definition

class CreateAPIKeyResponseTypeDef(TypedDict):
    APIKey: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFirewallManagerRuleGroupsResponseTypeDef

```python
# DeleteFirewallManagerRuleGroupsResponseTypeDef definition

class DeleteFirewallManagerRuleGroupsResponseTypeDef(TypedDict):
    NextWebACLLockToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateMobileSdkReleaseUrlResponseTypeDef

```python
# GenerateMobileSdkReleaseUrlResponseTypeDef definition

class GenerateMobileSdkReleaseUrlResponseTypeDef(TypedDict):
    Url: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDecryptedAPIKeyResponseTypeDef

```python
# GetDecryptedAPIKeyResponseTypeDef definition

class GetDecryptedAPIKeyResponseTypeDef(TypedDict):
    TokenDomains: List[str],
    CreationTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPermissionPolicyResponseTypeDef

```python
# GetPermissionPolicyResponseTypeDef definition

class GetPermissionPolicyResponseTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAPIKeysResponseTypeDef

```python
# ListAPIKeysResponseTypeDef definition

class ListAPIKeysResponseTypeDef(TypedDict):
    NextMarker: str,
    APIKeySummaries: List[APIKeySummaryTypeDef],  # (1)
    ApplicationIntegrationURL: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: APIKeySummaryTypeDef](./type_defs.md#apikeysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourcesForWebACLResponseTypeDef

```python
# ListResourcesForWebACLResponseTypeDef definition

class ListResourcesForWebACLResponseTypeDef(TypedDict):
    ResourceArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutManagedRuleSetVersionsResponseTypeDef

```python
# PutManagedRuleSetVersionsResponseTypeDef definition

class PutManagedRuleSetVersionsResponseTypeDef(TypedDict):
    NextLockToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIPSetResponseTypeDef

```python
# UpdateIPSetResponseTypeDef definition

class UpdateIPSetResponseTypeDef(TypedDict):
    NextLockToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateManagedRuleSetVersionExpiryDateResponseTypeDef

```python
# UpdateManagedRuleSetVersionExpiryDateResponseTypeDef definition

class UpdateManagedRuleSetVersionExpiryDateResponseTypeDef(TypedDict):
    ExpiringVersion: str,
    ExpiryTimestamp: datetime,
    NextLockToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRegexPatternSetResponseTypeDef

```python
# UpdateRegexPatternSetResponseTypeDef definition

class UpdateRegexPatternSetResponseTypeDef(TypedDict):
    NextLockToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRuleGroupResponseTypeDef

```python
# UpdateRuleGroupResponseTypeDef definition

class UpdateRuleGroupResponseTypeDef(TypedDict):
    NextLockToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWebACLResponseTypeDef

```python
# UpdateWebACLResponseTypeDef definition

class UpdateWebACLResponseTypeDef(TypedDict):
    NextLockToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConditionTypeDef

```python
# ConditionTypeDef definition

class ConditionTypeDef(TypedDict):
    ActionCondition: NotRequired[ActionConditionTypeDef],  # (1)
    LabelNameCondition: NotRequired[LabelNameConditionTypeDef],  # (2)
```

1. See [:material-code-braces: ActionConditionTypeDef](./type_defs.md#actionconditiontypedef) 
2. See [:material-code-braces: LabelNameConditionTypeDef](./type_defs.md#labelnameconditiontypedef) 
## CookiesTypeDef

```python
# CookiesTypeDef definition

class CookiesTypeDef(TypedDict):
    MatchPattern: CookieMatchPatternTypeDef,  # (1)
    MatchScope: MapMatchScopeType,  # (2)
    OversizeHandling: OversizeHandlingType,  # (3)
```

1. See [:material-code-braces: CookieMatchPatternTypeDef](./type_defs.md#cookiematchpatterntypedef) 
2. See [:material-code-brackets: MapMatchScopeType](./literals.md#mapmatchscopetype) 
3. See [:material-code-brackets: OversizeHandlingType](./literals.md#oversizehandlingtype) 
## CreateIPSetRequestRequestTypeDef

```python
# CreateIPSetRequestRequestTypeDef definition

class CreateIPSetRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    IPAddressVersion: IPAddressVersionType,  # (2)
    Addresses: Sequence[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-brackets: IPAddressVersionType](./literals.md#ipaddressversiontype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## MobileSdkReleaseTypeDef

```python
# MobileSdkReleaseTypeDef definition

class MobileSdkReleaseTypeDef(TypedDict):
    ReleaseVersion: NotRequired[str],
    Timestamp: NotRequired[datetime],
    ReleaseNotes: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
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
## CreateIPSetResponseTypeDef

```python
# CreateIPSetResponseTypeDef definition

class CreateIPSetResponseTypeDef(TypedDict):
    Summary: IPSetSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IPSetSummaryTypeDef](./type_defs.md#ipsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## CreateRegexPatternSetRequestRequestTypeDef

```python
# CreateRegexPatternSetRequestRequestTypeDef definition

class CreateRegexPatternSetRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    RegularExpressionList: Sequence[RegexTypeDef],  # (2)
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: RegexTypeDef](./type_defs.md#regextypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RegexPatternSetTypeDef

```python
# RegexPatternSetTypeDef definition

class RegexPatternSetTypeDef(TypedDict):
    Name: NotRequired[str],
    Id: NotRequired[str],
    ARN: NotRequired[str],
    Description: NotRequired[str],
    RegularExpressionList: NotRequired[List[RegexTypeDef]],  # (1)
```

1. See [:material-code-braces: RegexTypeDef](./type_defs.md#regextypedef) 
## UpdateRegexPatternSetRequestRequestTypeDef

```python
# UpdateRegexPatternSetRequestRequestTypeDef definition

class UpdateRegexPatternSetRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    RegularExpressionList: Sequence[RegexTypeDef],  # (2)
    LockToken: str,
    Description: NotRequired[str],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: RegexTypeDef](./type_defs.md#regextypedef) 
## CreateRegexPatternSetResponseTypeDef

```python
# CreateRegexPatternSetResponseTypeDef definition

class CreateRegexPatternSetResponseTypeDef(TypedDict):
    Summary: RegexPatternSetSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexPatternSetSummaryTypeDef](./type_defs.md#regexpatternsetsummarytypedef) 
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
## CreateRuleGroupResponseTypeDef

```python
# CreateRuleGroupResponseTypeDef definition

class CreateRuleGroupResponseTypeDef(TypedDict):
    Summary: RuleGroupSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupSummaryTypeDef](./type_defs.md#rulegroupsummarytypedef) 
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
## CreateWebACLResponseTypeDef

```python
# CreateWebACLResponseTypeDef definition

class CreateWebACLResponseTypeDef(TypedDict):
    Summary: WebACLSummaryTypeDef,  # (1)
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
## CustomRequestHandlingTypeDef

```python
# CustomRequestHandlingTypeDef definition

class CustomRequestHandlingTypeDef(TypedDict):
    InsertHeaders: Sequence[CustomHTTPHeaderTypeDef],  # (1)
```

1. See [:material-code-braces: CustomHTTPHeaderTypeDef](./type_defs.md#customhttpheadertypedef) 
## CustomResponseTypeDef

```python
# CustomResponseTypeDef definition

class CustomResponseTypeDef(TypedDict):
    ResponseCode: int,
    CustomResponseBodyKey: NotRequired[str],
    ResponseHeaders: NotRequired[Sequence[CustomHTTPHeaderTypeDef]],  # (1)
```

1. See [:material-code-braces: CustomHTTPHeaderTypeDef](./type_defs.md#customhttpheadertypedef) 
## DescribeAllManagedProductsResponseTypeDef

```python
# DescribeAllManagedProductsResponseTypeDef definition

class DescribeAllManagedProductsResponseTypeDef(TypedDict):
    ManagedProducts: List[ManagedProductDescriptorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedProductDescriptorTypeDef](./type_defs.md#managedproductdescriptortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeManagedProductsByVendorResponseTypeDef

```python
# DescribeManagedProductsByVendorResponseTypeDef definition

class DescribeManagedProductsByVendorResponseTypeDef(TypedDict):
    ManagedProducts: List[ManagedProductDescriptorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedProductDescriptorTypeDef](./type_defs.md#managedproductdescriptortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GeoMatchStatementTypeDef

```python
# GeoMatchStatementTypeDef definition

class GeoMatchStatementTypeDef(TypedDict):
    CountryCodes: NotRequired[Sequence[CountryCodeType]],  # (1)
    ForwardedIPConfig: NotRequired[ForwardedIPConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: CountryCodeType](./literals.md#countrycodetype) 
2. See [:material-code-braces: ForwardedIPConfigTypeDef](./type_defs.md#forwardedipconfigtypedef) 
## GetIPSetResponseTypeDef

```python
# GetIPSetResponseTypeDef definition

class GetIPSetResponseTypeDef(TypedDict):
    IPSet: IPSetTypeDef,  # (1)
    LockToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IPSetTypeDef](./type_defs.md#ipsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRateBasedStatementManagedKeysResponseTypeDef

```python
# GetRateBasedStatementManagedKeysResponseTypeDef definition

class GetRateBasedStatementManagedKeysResponseTypeDef(TypedDict):
    ManagedKeysIPV4: RateBasedStatementManagedKeysIPSetTypeDef,  # (1)
    ManagedKeysIPV6: RateBasedStatementManagedKeysIPSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RateBasedStatementManagedKeysIPSetTypeDef](./type_defs.md#ratebasedstatementmanagedkeysipsettypedef) 
2. See [:material-code-braces: RateBasedStatementManagedKeysIPSetTypeDef](./type_defs.md#ratebasedstatementmanagedkeysipsettypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## HeadersTypeDef

```python
# HeadersTypeDef definition

class HeadersTypeDef(TypedDict):
    MatchPattern: HeaderMatchPatternTypeDef,  # (1)
    MatchScope: MapMatchScopeType,  # (2)
    OversizeHandling: OversizeHandlingType,  # (3)
```

1. See [:material-code-braces: HeaderMatchPatternTypeDef](./type_defs.md#headermatchpatterntypedef) 
2. See [:material-code-brackets: MapMatchScopeType](./literals.md#mapmatchscopetype) 
3. See [:material-code-brackets: OversizeHandlingType](./literals.md#oversizehandlingtype) 
## IPSetReferenceStatementTypeDef

```python
# IPSetReferenceStatementTypeDef definition

class IPSetReferenceStatementTypeDef(TypedDict):
    ARN: str,
    IPSetForwardedIPConfig: NotRequired[IPSetForwardedIPConfigTypeDef],  # (1)
```

1. See [:material-code-braces: IPSetForwardedIPConfigTypeDef](./type_defs.md#ipsetforwardedipconfigtypedef) 
## JsonBodyTypeDef

```python
# JsonBodyTypeDef definition

class JsonBodyTypeDef(TypedDict):
    MatchPattern: JsonMatchPatternTypeDef,  # (1)
    MatchScope: JsonMatchScopeType,  # (2)
    InvalidFallbackBehavior: NotRequired[BodyParsingFallbackBehaviorType],  # (3)
    OversizeHandling: NotRequired[OversizeHandlingType],  # (4)
```

1. See [:material-code-braces: JsonMatchPatternTypeDef](./type_defs.md#jsonmatchpatterntypedef) 
2. See [:material-code-brackets: JsonMatchScopeType](./literals.md#jsonmatchscopetype) 
3. See [:material-code-brackets: BodyParsingFallbackBehaviorType](./literals.md#bodyparsingfallbackbehaviortype) 
4. See [:material-code-brackets: OversizeHandlingType](./literals.md#oversizehandlingtype) 
## ListAvailableManagedRuleGroupVersionsResponseTypeDef

```python
# ListAvailableManagedRuleGroupVersionsResponseTypeDef definition

class ListAvailableManagedRuleGroupVersionsResponseTypeDef(TypedDict):
    NextMarker: str,
    Versions: List[ManagedRuleGroupVersionTypeDef],  # (1)
    CurrentDefaultVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedRuleGroupVersionTypeDef](./type_defs.md#managedrulegroupversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAvailableManagedRuleGroupsResponseTypeDef

```python
# ListAvailableManagedRuleGroupsResponseTypeDef definition

class ListAvailableManagedRuleGroupsResponseTypeDef(TypedDict):
    NextMarker: str,
    ManagedRuleGroups: List[ManagedRuleGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedRuleGroupSummaryTypeDef](./type_defs.md#managedrulegroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListManagedRuleSetsResponseTypeDef

```python
# ListManagedRuleSetsResponseTypeDef definition

class ListManagedRuleSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    ManagedRuleSets: List[ManagedRuleSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedRuleSetSummaryTypeDef](./type_defs.md#managedrulesetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMobileSdkReleasesResponseTypeDef

```python
# ListMobileSdkReleasesResponseTypeDef definition

class ListMobileSdkReleasesResponseTypeDef(TypedDict):
    ReleaseSummaries: List[ReleaseSummaryTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReleaseSummaryTypeDef](./type_defs.md#releasesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RequestInspectionTypeDef

```python
# RequestInspectionTypeDef definition

class RequestInspectionTypeDef(TypedDict):
    PayloadType: PayloadTypeType,  # (1)
    UsernameField: UsernameFieldTypeDef,  # (2)
    PasswordField: PasswordFieldTypeDef,  # (3)
```

1. See [:material-code-brackets: PayloadTypeType](./literals.md#payloadtypetype) 
2. See [:material-code-braces: UsernameFieldTypeDef](./type_defs.md#usernamefieldtypedef) 
3. See [:material-code-braces: PasswordFieldTypeDef](./type_defs.md#passwordfieldtypedef) 
## ManagedRuleSetTypeDef

```python
# ManagedRuleSetTypeDef definition

class ManagedRuleSetTypeDef(TypedDict):
    Name: str,
    Id: str,
    ARN: str,
    Description: NotRequired[str],
    PublishedVersions: NotRequired[Dict[str, ManagedRuleSetVersionTypeDef]],  # (1)
    RecommendedVersion: NotRequired[str],
    LabelNamespace: NotRequired[str],
```

1. See [:material-code-braces: ManagedRuleSetVersionTypeDef](./type_defs.md#managedrulesetversiontypedef) 
## RequestInspectionACFPTypeDef

```python
# RequestInspectionACFPTypeDef definition

class RequestInspectionACFPTypeDef(TypedDict):
    PayloadType: PayloadTypeType,  # (1)
    UsernameField: NotRequired[UsernameFieldTypeDef],  # (2)
    PasswordField: NotRequired[PasswordFieldTypeDef],  # (3)
    EmailField: NotRequired[EmailFieldTypeDef],  # (4)
    PhoneNumberFields: NotRequired[Sequence[PhoneNumberFieldTypeDef]],  # (5)
    AddressFields: NotRequired[Sequence[AddressFieldTypeDef]],  # (6)
```

1. See [:material-code-brackets: PayloadTypeType](./literals.md#payloadtypetype) 
2. See [:material-code-braces: UsernameFieldTypeDef](./type_defs.md#usernamefieldtypedef) 
3. See [:material-code-braces: PasswordFieldTypeDef](./type_defs.md#passwordfieldtypedef) 
4. See [:material-code-braces: EmailFieldTypeDef](./type_defs.md#emailfieldtypedef) 
5. See [:material-code-braces: PhoneNumberFieldTypeDef](./type_defs.md#phonenumberfieldtypedef) 
6. See [:material-code-braces: AddressFieldTypeDef](./type_defs.md#addressfieldtypedef) 
## PutManagedRuleSetVersionsRequestRequestTypeDef

```python
# PutManagedRuleSetVersionsRequestRequestTypeDef definition

class PutManagedRuleSetVersionsRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
    RecommendedVersion: NotRequired[str],
    VersionsToPublish: NotRequired[Mapping[str, VersionToPublishTypeDef]],  # (2)
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: VersionToPublishTypeDef](./type_defs.md#versiontopublishtypedef) 
## ResponseInspectionTypeDef

```python
# ResponseInspectionTypeDef definition

class ResponseInspectionTypeDef(TypedDict):
    StatusCode: NotRequired[ResponseInspectionStatusCodeTypeDef],  # (1)
    Header: NotRequired[ResponseInspectionHeaderTypeDef],  # (2)
    BodyContains: NotRequired[ResponseInspectionBodyContainsTypeDef],  # (3)
    Json: NotRequired[ResponseInspectionJsonTypeDef],  # (4)
```

1. See [:material-code-braces: ResponseInspectionStatusCodeTypeDef](./type_defs.md#responseinspectionstatuscodetypedef) 
2. See [:material-code-braces: ResponseInspectionHeaderTypeDef](./type_defs.md#responseinspectionheadertypedef) 
3. See [:material-code-braces: ResponseInspectionBodyContainsTypeDef](./type_defs.md#responseinspectionbodycontainstypedef) 
4. See [:material-code-braces: ResponseInspectionJsonTypeDef](./type_defs.md#responseinspectionjsontypedef) 
## TimeWindowTypeDef

```python
# TimeWindowTypeDef definition

class TimeWindowTypeDef(TypedDict):
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
```

## UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef

```python
# UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef definition

class UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
    VersionToExpire: str,
    ExpiryTimestamp: Union[datetime, str],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## RateBasedStatementCustomKeyTypeDef

```python
# RateBasedStatementCustomKeyTypeDef definition

class RateBasedStatementCustomKeyTypeDef(TypedDict):
    Header: NotRequired[RateLimitHeaderTypeDef],  # (1)
    Cookie: NotRequired[RateLimitCookieTypeDef],  # (2)
    QueryArgument: NotRequired[RateLimitQueryArgumentTypeDef],  # (3)
    QueryString: NotRequired[RateLimitQueryStringTypeDef],  # (4)
    HTTPMethod: NotRequired[Mapping[str, Any]],
    ForwardedIP: NotRequired[Mapping[str, Any]],
    IP: NotRequired[Mapping[str, Any]],
    LabelNamespace: NotRequired[RateLimitLabelNamespaceTypeDef],  # (5)
    UriPath: NotRequired[RateLimitUriPathTypeDef],  # (6)
```

1. See [:material-code-braces: RateLimitHeaderTypeDef](./type_defs.md#ratelimitheadertypedef) 
2. See [:material-code-braces: RateLimitCookieTypeDef](./type_defs.md#ratelimitcookietypedef) 
3. See [:material-code-braces: RateLimitQueryArgumentTypeDef](./type_defs.md#ratelimitqueryargumenttypedef) 
4. See [:material-code-braces: RateLimitQueryStringTypeDef](./type_defs.md#ratelimitquerystringtypedef) 
5. See [:material-code-braces: RateLimitLabelNamespaceTypeDef](./type_defs.md#ratelimitlabelnamespacetypedef) 
6. See [:material-code-braces: RateLimitUriPathTypeDef](./type_defs.md#ratelimituripathtypedef) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Behavior: FilterBehaviorType,  # (1)
    Requirement: FilterRequirementType,  # (2)
    Conditions: List[ConditionTypeDef],  # (3)
```

1. See [:material-code-brackets: FilterBehaviorType](./literals.md#filterbehaviortype) 
2. See [:material-code-brackets: FilterRequirementType](./literals.md#filterrequirementtype) 
3. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
## GetMobileSdkReleaseResponseTypeDef

```python
# GetMobileSdkReleaseResponseTypeDef definition

class GetMobileSdkReleaseResponseTypeDef(TypedDict):
    MobileSdkRelease: MobileSdkReleaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MobileSdkReleaseTypeDef](./type_defs.md#mobilesdkreleasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## GetRegexPatternSetResponseTypeDef

```python
# GetRegexPatternSetResponseTypeDef definition

class GetRegexPatternSetResponseTypeDef(TypedDict):
    RegexPatternSet: RegexPatternSetTypeDef,  # (1)
    LockToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexPatternSetTypeDef](./type_defs.md#regexpatternsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AllowActionTypeDef

```python
# AllowActionTypeDef definition

class AllowActionTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[CustomRequestHandlingTypeDef],  # (1)
```

1. See [:material-code-braces: CustomRequestHandlingTypeDef](./type_defs.md#customrequesthandlingtypedef) 
## CaptchaActionTypeDef

```python
# CaptchaActionTypeDef definition

class CaptchaActionTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[CustomRequestHandlingTypeDef],  # (1)
```

1. See [:material-code-braces: CustomRequestHandlingTypeDef](./type_defs.md#customrequesthandlingtypedef) 
## ChallengeActionTypeDef

```python
# ChallengeActionTypeDef definition

class ChallengeActionTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[CustomRequestHandlingTypeDef],  # (1)
```

1. See [:material-code-braces: CustomRequestHandlingTypeDef](./type_defs.md#customrequesthandlingtypedef) 
## CountActionTypeDef

```python
# CountActionTypeDef definition

class CountActionTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[CustomRequestHandlingTypeDef],  # (1)
```

1. See [:material-code-braces: CustomRequestHandlingTypeDef](./type_defs.md#customrequesthandlingtypedef) 
## BlockActionTypeDef

```python
# BlockActionTypeDef definition

class BlockActionTypeDef(TypedDict):
    CustomResponse: NotRequired[CustomResponseTypeDef],  # (1)
```

1. See [:material-code-braces: CustomResponseTypeDef](./type_defs.md#customresponsetypedef) 
## SampledHTTPRequestTypeDef

```python
# SampledHTTPRequestTypeDef definition

class SampledHTTPRequestTypeDef(TypedDict):
    Request: HTTPRequestTypeDef,  # (1)
    Weight: int,
    Timestamp: NotRequired[datetime],
    Action: NotRequired[str],
    RuleNameWithinRuleGroup: NotRequired[str],
    RequestHeadersInserted: NotRequired[List[HTTPHeaderTypeDef]],  # (2)
    ResponseCodeSent: NotRequired[int],
    Labels: NotRequired[List[LabelTypeDef]],  # (3)
    CaptchaResponse: NotRequired[CaptchaResponseTypeDef],  # (4)
    ChallengeResponse: NotRequired[ChallengeResponseTypeDef],  # (5)
    OverriddenAction: NotRequired[str],
```

1. See [:material-code-braces: HTTPRequestTypeDef](./type_defs.md#httprequesttypedef) 
2. See [:material-code-braces: HTTPHeaderTypeDef](./type_defs.md#httpheadertypedef) 
3. See [:material-code-braces: LabelTypeDef](./type_defs.md#labeltypedef) 
4. See [:material-code-braces: CaptchaResponseTypeDef](./type_defs.md#captcharesponsetypedef) 
5. See [:material-code-braces: ChallengeResponseTypeDef](./type_defs.md#challengeresponsetypedef) 
## FieldToMatchTypeDef

```python
# FieldToMatchTypeDef definition

class FieldToMatchTypeDef(TypedDict):
    SingleHeader: NotRequired[SingleHeaderTypeDef],  # (1)
    SingleQueryArgument: NotRequired[SingleQueryArgumentTypeDef],  # (2)
    AllQueryArguments: NotRequired[Mapping[str, Any]],
    UriPath: NotRequired[Mapping[str, Any]],
    QueryString: NotRequired[Mapping[str, Any]],
    Body: NotRequired[BodyTypeDef],  # (3)
    Method: NotRequired[Mapping[str, Any]],
    JsonBody: NotRequired[JsonBodyTypeDef],  # (4)
    Headers: NotRequired[HeadersTypeDef],  # (5)
    Cookies: NotRequired[CookiesTypeDef],  # (6)
    HeaderOrder: NotRequired[HeaderOrderTypeDef],  # (7)
```

1. See [:material-code-braces: SingleHeaderTypeDef](./type_defs.md#singleheadertypedef) 
2. See [:material-code-braces: SingleQueryArgumentTypeDef](./type_defs.md#singlequeryargumenttypedef) 
3. See [:material-code-braces: BodyTypeDef](./type_defs.md#bodytypedef) 
4. See [:material-code-braces: JsonBodyTypeDef](./type_defs.md#jsonbodytypedef) 
5. See [:material-code-braces: HeadersTypeDef](./type_defs.md#headerstypedef) 
6. See [:material-code-braces: CookiesTypeDef](./type_defs.md#cookiestypedef) 
7. See [:material-code-braces: HeaderOrderTypeDef](./type_defs.md#headerordertypedef) 
## GetManagedRuleSetResponseTypeDef

```python
# GetManagedRuleSetResponseTypeDef definition

class GetManagedRuleSetResponseTypeDef(TypedDict):
    ManagedRuleSet: ManagedRuleSetTypeDef,  # (1)
    LockToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedRuleSetTypeDef](./type_defs.md#managedrulesettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AWSManagedRulesACFPRuleSetTypeDef

```python
# AWSManagedRulesACFPRuleSetTypeDef definition

class AWSManagedRulesACFPRuleSetTypeDef(TypedDict):
    CreationPath: str,
    RegistrationPagePath: str,
    RequestInspection: RequestInspectionACFPTypeDef,  # (1)
    ResponseInspection: NotRequired[ResponseInspectionTypeDef],  # (2)
    EnableRegexInPath: NotRequired[bool],
```

1. See [:material-code-braces: RequestInspectionACFPTypeDef](./type_defs.md#requestinspectionacfptypedef) 
2. See [:material-code-braces: ResponseInspectionTypeDef](./type_defs.md#responseinspectiontypedef) 
## AWSManagedRulesATPRuleSetTypeDef

```python
# AWSManagedRulesATPRuleSetTypeDef definition

class AWSManagedRulesATPRuleSetTypeDef(TypedDict):
    LoginPath: str,
    RequestInspection: NotRequired[RequestInspectionTypeDef],  # (1)
    ResponseInspection: NotRequired[ResponseInspectionTypeDef],  # (2)
    EnableRegexInPath: NotRequired[bool],
```

1. See [:material-code-braces: RequestInspectionTypeDef](./type_defs.md#requestinspectiontypedef) 
2. See [:material-code-braces: ResponseInspectionTypeDef](./type_defs.md#responseinspectiontypedef) 
## GetSampledRequestsRequestRequestTypeDef

```python
# GetSampledRequestsRequestRequestTypeDef definition

class GetSampledRequestsRequestRequestTypeDef(TypedDict):
    WebAclArn: str,
    RuleMetricName: str,
    Scope: ScopeType,  # (1)
    TimeWindow: TimeWindowTypeDef,  # (2)
    MaxItems: int,
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: TimeWindowTypeDef](./type_defs.md#timewindowtypedef) 
## RateBasedStatementTypeDef

```python
# RateBasedStatementTypeDef definition

class RateBasedStatementTypeDef(TypedDict):
    Limit: int,
    AggregateKeyType: RateBasedStatementAggregateKeyTypeType,  # (1)
    ScopeDownStatement: NotRequired[StatementTypeDef],  # (2)
    ForwardedIPConfig: NotRequired[ForwardedIPConfigTypeDef],  # (3)
    CustomKeys: NotRequired[Sequence[RateBasedStatementCustomKeyTypeDef]],  # (4)
```

1. See [:material-code-brackets: RateBasedStatementAggregateKeyTypeType](./literals.md#ratebasedstatementaggregatekeytypetype) 
2. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
3. See [:material-code-braces: ForwardedIPConfigTypeDef](./type_defs.md#forwardedipconfigtypedef) 
4. See [:material-code-braces: RateBasedStatementCustomKeyTypeDef](./type_defs.md#ratebasedstatementcustomkeytypedef) 
## LoggingFilterTypeDef

```python
# LoggingFilterTypeDef definition

class LoggingFilterTypeDef(TypedDict):
    Filters: List[FilterTypeDef],  # (1)
    DefaultBehavior: FilterBehaviorType,  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: FilterBehaviorType](./literals.md#filterbehaviortype) 
## OverrideActionTypeDef

```python
# OverrideActionTypeDef definition

class OverrideActionTypeDef(TypedDict):
    Count: NotRequired[CountActionTypeDef],  # (1)
    None: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: CountActionTypeDef](./type_defs.md#countactiontypedef) 
## DefaultActionTypeDef

```python
# DefaultActionTypeDef definition

class DefaultActionTypeDef(TypedDict):
    Block: NotRequired[BlockActionTypeDef],  # (1)
    Allow: NotRequired[AllowActionTypeDef],  # (2)
```

1. See [:material-code-braces: BlockActionTypeDef](./type_defs.md#blockactiontypedef) 
2. See [:material-code-braces: AllowActionTypeDef](./type_defs.md#allowactiontypedef) 
## RuleActionTypeDef

```python
# RuleActionTypeDef definition

class RuleActionTypeDef(TypedDict):
    Block: NotRequired[BlockActionTypeDef],  # (1)
    Allow: NotRequired[AllowActionTypeDef],  # (2)
    Count: NotRequired[CountActionTypeDef],  # (3)
    Captcha: NotRequired[CaptchaActionTypeDef],  # (4)
    Challenge: NotRequired[ChallengeActionTypeDef],  # (5)
```

1. See [:material-code-braces: BlockActionTypeDef](./type_defs.md#blockactiontypedef) 
2. See [:material-code-braces: AllowActionTypeDef](./type_defs.md#allowactiontypedef) 
3. See [:material-code-braces: CountActionTypeDef](./type_defs.md#countactiontypedef) 
4. See [:material-code-braces: CaptchaActionTypeDef](./type_defs.md#captchaactiontypedef) 
5. See [:material-code-braces: ChallengeActionTypeDef](./type_defs.md#challengeactiontypedef) 
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
## ByteMatchStatementTypeDef

```python
# ByteMatchStatementTypeDef definition

class ByteMatchStatementTypeDef(TypedDict):
    SearchString: Union[str, bytes, IO[Any], StreamingBody],
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TextTransformations: Sequence[TextTransformationTypeDef],  # (2)
    PositionalConstraint: PositionalConstraintType,  # (3)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
3. See [:material-code-brackets: PositionalConstraintType](./literals.md#positionalconstrainttype) 
## RegexMatchStatementTypeDef

```python
# RegexMatchStatementTypeDef definition

class RegexMatchStatementTypeDef(TypedDict):
    RegexString: str,
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TextTransformations: Sequence[TextTransformationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## RegexPatternSetReferenceStatementTypeDef

```python
# RegexPatternSetReferenceStatementTypeDef definition

class RegexPatternSetReferenceStatementTypeDef(TypedDict):
    ARN: str,
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TextTransformations: Sequence[TextTransformationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## SizeConstraintStatementTypeDef

```python
# SizeConstraintStatementTypeDef definition

class SizeConstraintStatementTypeDef(TypedDict):
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    ComparisonOperator: ComparisonOperatorType,  # (2)
    Size: int,
    TextTransformations: Sequence[TextTransformationTypeDef],  # (3)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
3. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## SqliMatchStatementTypeDef

```python
# SqliMatchStatementTypeDef definition

class SqliMatchStatementTypeDef(TypedDict):
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TextTransformations: Sequence[TextTransformationTypeDef],  # (2)
    SensitivityLevel: NotRequired[SensitivityLevelType],  # (3)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
3. See [:material-code-brackets: SensitivityLevelType](./literals.md#sensitivityleveltype) 
## XssMatchStatementTypeDef

```python
# XssMatchStatementTypeDef definition

class XssMatchStatementTypeDef(TypedDict):
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TextTransformations: Sequence[TextTransformationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## ManagedRuleGroupConfigTypeDef

```python
# ManagedRuleGroupConfigTypeDef definition

class ManagedRuleGroupConfigTypeDef(TypedDict):
    LoginPath: NotRequired[str],
    PayloadType: NotRequired[PayloadTypeType],  # (1)
    UsernameField: NotRequired[UsernameFieldTypeDef],  # (2)
    PasswordField: NotRequired[PasswordFieldTypeDef],  # (3)
    AWSManagedRulesBotControlRuleSet: NotRequired[AWSManagedRulesBotControlRuleSetTypeDef],  # (4)
    AWSManagedRulesATPRuleSet: NotRequired[AWSManagedRulesATPRuleSetTypeDef],  # (5)
    AWSManagedRulesACFPRuleSet: NotRequired[AWSManagedRulesACFPRuleSetTypeDef],  # (6)
```

1. See [:material-code-brackets: PayloadTypeType](./literals.md#payloadtypetype) 
2. See [:material-code-braces: UsernameFieldTypeDef](./type_defs.md#usernamefieldtypedef) 
3. See [:material-code-braces: PasswordFieldTypeDef](./type_defs.md#passwordfieldtypedef) 
4. See [:material-code-braces: AWSManagedRulesBotControlRuleSetTypeDef](./type_defs.md#awsmanagedrulesbotcontrolrulesettypedef) 
5. See [:material-code-braces: AWSManagedRulesATPRuleSetTypeDef](./type_defs.md#awsmanagedrulesatprulesettypedef) 
6. See [:material-code-braces: AWSManagedRulesACFPRuleSetTypeDef](./type_defs.md#awsmanagedrulesacfprulesettypedef) 
## LoggingConfigurationTypeDef

```python
# LoggingConfigurationTypeDef definition

class LoggingConfigurationTypeDef(TypedDict):
    ResourceArn: str,
    LogDestinationConfigs: List[str],
    RedactedFields: NotRequired[List[FieldToMatchTypeDef]],  # (1)
    ManagedByFirewallManager: NotRequired[bool],
    LoggingFilter: NotRequired[LoggingFilterTypeDef],  # (2)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-braces: LoggingFilterTypeDef](./type_defs.md#loggingfiltertypedef) 
## RuleActionOverrideTypeDef

```python
# RuleActionOverrideTypeDef definition

class RuleActionOverrideTypeDef(TypedDict):
    Name: str,
    ActionToUse: RuleActionTypeDef,  # (1)
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
## RuleSummaryTypeDef

```python
# RuleSummaryTypeDef definition

class RuleSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    Action: NotRequired[RuleActionTypeDef],  # (1)
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    Name: str,
    Priority: int,
    Statement: StatementTypeDef,  # (1)
    VisibilityConfig: VisibilityConfigTypeDef,  # (5)
    Action: NotRequired[RuleActionTypeDef],  # (2)
    OverrideAction: NotRequired[OverrideActionTypeDef],  # (3)
    RuleLabels: NotRequired[Sequence[LabelTypeDef]],  # (4)
    CaptchaConfig: NotRequired[CaptchaConfigTypeDef],  # (6)
    ChallengeConfig: NotRequired[ChallengeConfigTypeDef],  # (7)
```

1. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
2. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
3. See [:material-code-braces: OverrideActionTypeDef](./type_defs.md#overrideactiontypedef) 
4. See [:material-code-braces: LabelTypeDef](./type_defs.md#labeltypedef) 
5. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
6. See [:material-code-braces: CaptchaConfigTypeDef](./type_defs.md#captchaconfigtypedef) 
7. See [:material-code-braces: ChallengeConfigTypeDef](./type_defs.md#challengeconfigtypedef) 
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
## ManagedRuleGroupStatementTypeDef

```python
# ManagedRuleGroupStatementTypeDef definition

class ManagedRuleGroupStatementTypeDef(TypedDict):
    VendorName: str,
    Name: str,
    Version: NotRequired[str],
    ExcludedRules: NotRequired[Sequence[ExcludedRuleTypeDef]],  # (1)
    ScopeDownStatement: NotRequired[StatementTypeDef],  # (2)
    ManagedRuleGroupConfigs: NotRequired[Sequence[ManagedRuleGroupConfigTypeDef]],  # (3)
    RuleActionOverrides: NotRequired[Sequence[RuleActionOverrideTypeDef]],  # (4)
```

1. See [:material-code-braces: ExcludedRuleTypeDef](./type_defs.md#excludedruletypedef) 
2. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
3. See [:material-code-braces: ManagedRuleGroupConfigTypeDef](./type_defs.md#managedrulegroupconfigtypedef) 
4. See [:material-code-braces: RuleActionOverrideTypeDef](./type_defs.md#ruleactionoverridetypedef) 
## RuleGroupReferenceStatementTypeDef

```python
# RuleGroupReferenceStatementTypeDef definition

class RuleGroupReferenceStatementTypeDef(TypedDict):
    ARN: str,
    ExcludedRules: NotRequired[Sequence[ExcludedRuleTypeDef]],  # (1)
    RuleActionOverrides: NotRequired[Sequence[RuleActionOverrideTypeDef]],  # (2)
```

1. See [:material-code-braces: ExcludedRuleTypeDef](./type_defs.md#excludedruletypedef) 
2. See [:material-code-braces: RuleActionOverrideTypeDef](./type_defs.md#ruleactionoverridetypedef) 
## DescribeManagedRuleGroupResponseTypeDef

```python
# DescribeManagedRuleGroupResponseTypeDef definition

class DescribeManagedRuleGroupResponseTypeDef(TypedDict):
    VersionName: str,
    SnsTopicArn: str,
    Capacity: int,
    Rules: List[RuleSummaryTypeDef],  # (1)
    LabelNamespace: str,
    AvailableLabels: List[LabelSummaryTypeDef],  # (2)
    ConsumedLabels: List[LabelSummaryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef) 
2. See [:material-code-braces: LabelSummaryTypeDef](./type_defs.md#labelsummarytypedef) 
3. See [:material-code-braces: LabelSummaryTypeDef](./type_defs.md#labelsummarytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CheckCapacityRequestRequestTypeDef

```python
# CheckCapacityRequestRequestTypeDef definition

class CheckCapacityRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
    Rules: Sequence[RuleTypeDef],  # (2)
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
## CreateRuleGroupRequestRequestTypeDef

```python
# CreateRuleGroupRequestRequestTypeDef definition

class CreateRuleGroupRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Capacity: int,
    VisibilityConfig: VisibilityConfigTypeDef,  # (2)
    Description: NotRequired[str],
    Rules: NotRequired[Sequence[RuleTypeDef]],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    CustomResponseBodies: NotRequired[Mapping[str, CustomResponseBodyTypeDef]],  # (5)
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
3. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
## CreateWebACLRequestRequestTypeDef

```python
# CreateWebACLRequestRequestTypeDef definition

class CreateWebACLRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    DefaultAction: DefaultActionTypeDef,  # (2)
    VisibilityConfig: VisibilityConfigTypeDef,  # (3)
    Description: NotRequired[str],
    Rules: NotRequired[Sequence[RuleTypeDef]],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
    CustomResponseBodies: NotRequired[Mapping[str, CustomResponseBodyTypeDef]],  # (6)
    CaptchaConfig: NotRequired[CaptchaConfigTypeDef],  # (7)
    ChallengeConfig: NotRequired[ChallengeConfigTypeDef],  # (8)
    TokenDomains: NotRequired[Sequence[str]],
    AssociationConfig: NotRequired[AssociationConfigTypeDef],  # (9)
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DefaultActionTypeDef](./type_defs.md#defaultactiontypedef) 
3. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
4. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
7. See [:material-code-braces: CaptchaConfigTypeDef](./type_defs.md#captchaconfigtypedef) 
8. See [:material-code-braces: ChallengeConfigTypeDef](./type_defs.md#challengeconfigtypedef) 
9. See [:material-code-braces: AssociationConfigTypeDef](./type_defs.md#associationconfigtypedef) 
## RuleGroupTypeDef

```python
# RuleGroupTypeDef definition

class RuleGroupTypeDef(TypedDict):
    Name: str,
    Id: str,
    Capacity: int,
    ARN: str,
    VisibilityConfig: VisibilityConfigTypeDef,  # (2)
    Description: NotRequired[str],
    Rules: NotRequired[List[RuleTypeDef]],  # (1)
    LabelNamespace: NotRequired[str],
    CustomResponseBodies: NotRequired[Dict[str, CustomResponseBodyTypeDef]],  # (3)
    AvailableLabels: NotRequired[List[LabelSummaryTypeDef]],  # (4)
    ConsumedLabels: NotRequired[List[LabelSummaryTypeDef]],  # (4)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
3. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
4. See [:material-code-braces: LabelSummaryTypeDef](./type_defs.md#labelsummarytypedef) 
5. See [:material-code-braces: LabelSummaryTypeDef](./type_defs.md#labelsummarytypedef) 
## UpdateRuleGroupRequestRequestTypeDef

```python
# UpdateRuleGroupRequestRequestTypeDef definition

class UpdateRuleGroupRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    VisibilityConfig: VisibilityConfigTypeDef,  # (2)
    LockToken: str,
    Description: NotRequired[str],
    Rules: NotRequired[Sequence[RuleTypeDef]],  # (3)
    CustomResponseBodies: NotRequired[Mapping[str, CustomResponseBodyTypeDef]],  # (4)
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
3. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
4. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
## UpdateWebACLRequestRequestTypeDef

```python
# UpdateWebACLRequestRequestTypeDef definition

class UpdateWebACLRequestRequestTypeDef(TypedDict):
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    DefaultAction: DefaultActionTypeDef,  # (2)
    VisibilityConfig: VisibilityConfigTypeDef,  # (3)
    LockToken: str,
    Description: NotRequired[str],
    Rules: NotRequired[Sequence[RuleTypeDef]],  # (4)
    CustomResponseBodies: NotRequired[Mapping[str, CustomResponseBodyTypeDef]],  # (5)
    CaptchaConfig: NotRequired[CaptchaConfigTypeDef],  # (6)
    ChallengeConfig: NotRequired[ChallengeConfigTypeDef],  # (7)
    TokenDomains: NotRequired[Sequence[str]],
    AssociationConfig: NotRequired[AssociationConfigTypeDef],  # (8)
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DefaultActionTypeDef](./type_defs.md#defaultactiontypedef) 
3. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
4. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
5. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
6. See [:material-code-braces: CaptchaConfigTypeDef](./type_defs.md#captchaconfigtypedef) 
7. See [:material-code-braces: ChallengeConfigTypeDef](./type_defs.md#challengeconfigtypedef) 
8. See [:material-code-braces: AssociationConfigTypeDef](./type_defs.md#associationconfigtypedef) 
## FirewallManagerStatementTypeDef

```python
# FirewallManagerStatementTypeDef definition

class FirewallManagerStatementTypeDef(TypedDict):
    ManagedRuleGroupStatement: NotRequired[ManagedRuleGroupStatementTypeDef],  # (1)
    RuleGroupReferenceStatement: NotRequired[RuleGroupReferenceStatementTypeDef],  # (2)
```

1. See [:material-code-braces: ManagedRuleGroupStatementTypeDef](./type_defs.md#managedrulegroupstatementtypedef) 
2. See [:material-code-braces: RuleGroupReferenceStatementTypeDef](./type_defs.md#rulegroupreferencestatementtypedef) 
## StatementTypeDef

```python
# StatementTypeDef definition

class StatementTypeDef(TypedDict):
    ByteMatchStatement: NotRequired[ByteMatchStatementTypeDef],  # (1)
    SqliMatchStatement: NotRequired[SqliMatchStatementTypeDef],  # (2)
    XssMatchStatement: NotRequired[XssMatchStatementTypeDef],  # (3)
    SizeConstraintStatement: NotRequired[SizeConstraintStatementTypeDef],  # (4)
    GeoMatchStatement: NotRequired[GeoMatchStatementTypeDef],  # (5)
    RuleGroupReferenceStatement: NotRequired[RuleGroupReferenceStatementTypeDef],  # (6)
    IPSetReferenceStatement: NotRequired[IPSetReferenceStatementTypeDef],  # (7)
    RegexPatternSetReferenceStatement: NotRequired[RegexPatternSetReferenceStatementTypeDef],  # (8)
    RateBasedStatement: NotRequired[RateBasedStatementTypeDef],  # (9)
    AndStatement: NotRequired[AndStatementTypeDef],  # (10)
    OrStatement: NotRequired[OrStatementTypeDef],  # (11)
    NotStatement: NotRequired[NotStatementTypeDef],  # (12)
    ManagedRuleGroupStatement: NotRequired[ManagedRuleGroupStatementTypeDef],  # (13)
    LabelMatchStatement: NotRequired[LabelMatchStatementTypeDef],  # (14)
    RegexMatchStatement: NotRequired[RegexMatchStatementTypeDef],  # (15)
```

1. See [:material-code-braces: ByteMatchStatementTypeDef](./type_defs.md#bytematchstatementtypedef) 
2. See [:material-code-braces: SqliMatchStatementTypeDef](./type_defs.md#sqlimatchstatementtypedef) 
3. See [:material-code-braces: XssMatchStatementTypeDef](./type_defs.md#xssmatchstatementtypedef) 
4. See [:material-code-braces: SizeConstraintStatementTypeDef](./type_defs.md#sizeconstraintstatementtypedef) 
5. See [:material-code-braces: GeoMatchStatementTypeDef](./type_defs.md#geomatchstatementtypedef) 
6. See [:material-code-braces: RuleGroupReferenceStatementTypeDef](./type_defs.md#rulegroupreferencestatementtypedef) 
7. See [:material-code-braces: IPSetReferenceStatementTypeDef](./type_defs.md#ipsetreferencestatementtypedef) 
8. See [:material-code-braces: RegexPatternSetReferenceStatementTypeDef](./type_defs.md#regexpatternsetreferencestatementtypedef) 
9. See [:material-code-braces: RateBasedStatementTypeDef](./type_defs.md#ratebasedstatementtypedef) 
10. See [:material-code-braces: AndStatementTypeDef](./type_defs.md#andstatementtypedef) 
11. See [:material-code-braces: OrStatementTypeDef](./type_defs.md#orstatementtypedef) 
12. See [:material-code-braces: NotStatementTypeDef](./type_defs.md#notstatementtypedef) 
13. See [:material-code-braces: ManagedRuleGroupStatementTypeDef](./type_defs.md#managedrulegroupstatementtypedef) 
14. See [:material-code-braces: LabelMatchStatementTypeDef](./type_defs.md#labelmatchstatementtypedef) 
15. See [:material-code-braces: RegexMatchStatementTypeDef](./type_defs.md#regexmatchstatementtypedef) 
## GetRuleGroupResponseTypeDef

```python
# GetRuleGroupResponseTypeDef definition

class GetRuleGroupResponseTypeDef(TypedDict):
    RuleGroup: RuleGroupTypeDef,  # (1)
    LockToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupTypeDef](./type_defs.md#rulegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FirewallManagerRuleGroupTypeDef

```python
# FirewallManagerRuleGroupTypeDef definition

class FirewallManagerRuleGroupTypeDef(TypedDict):
    Name: str,
    Priority: int,
    FirewallManagerStatement: FirewallManagerStatementTypeDef,  # (1)
    OverrideAction: OverrideActionTypeDef,  # (2)
    VisibilityConfig: VisibilityConfigTypeDef,  # (3)
```

1. See [:material-code-braces: FirewallManagerStatementTypeDef](./type_defs.md#firewallmanagerstatementtypedef) 
2. See [:material-code-braces: OverrideActionTypeDef](./type_defs.md#overrideactiontypedef) 
3. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
## WebACLTypeDef

```python
# WebACLTypeDef definition

class WebACLTypeDef(TypedDict):
    Name: str,
    Id: str,
    ARN: str,
    DefaultAction: DefaultActionTypeDef,  # (1)
    VisibilityConfig: VisibilityConfigTypeDef,  # (3)
    Description: NotRequired[str],
    Rules: NotRequired[List[RuleTypeDef]],  # (2)
    Capacity: NotRequired[int],
    PreProcessFirewallManagerRuleGroups: NotRequired[List[FirewallManagerRuleGroupTypeDef]],  # (4)
    PostProcessFirewallManagerRuleGroups: NotRequired[List[FirewallManagerRuleGroupTypeDef]],  # (4)
    ManagedByFirewallManager: NotRequired[bool],
    LabelNamespace: NotRequired[str],
    CustomResponseBodies: NotRequired[Dict[str, CustomResponseBodyTypeDef]],  # (6)
    CaptchaConfig: NotRequired[CaptchaConfigTypeDef],  # (7)
    ChallengeConfig: NotRequired[ChallengeConfigTypeDef],  # (8)
    TokenDomains: NotRequired[List[str]],
    AssociationConfig: NotRequired[AssociationConfigTypeDef],  # (9)
```

1. See [:material-code-braces: DefaultActionTypeDef](./type_defs.md#defaultactiontypedef) 
2. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
3. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
4. See [:material-code-braces: FirewallManagerRuleGroupTypeDef](./type_defs.md#firewallmanagerrulegrouptypedef) 
5. See [:material-code-braces: FirewallManagerRuleGroupTypeDef](./type_defs.md#firewallmanagerrulegrouptypedef) 
6. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
7. See [:material-code-braces: CaptchaConfigTypeDef](./type_defs.md#captchaconfigtypedef) 
8. See [:material-code-braces: ChallengeConfigTypeDef](./type_defs.md#challengeconfigtypedef) 
9. See [:material-code-braces: AssociationConfigTypeDef](./type_defs.md#associationconfigtypedef) 
## GetWebACLForResourceResponseTypeDef

```python
# GetWebACLForResourceResponseTypeDef definition

class GetWebACLForResourceResponseTypeDef(TypedDict):
    WebACL: WebACLTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebACLTypeDef](./type_defs.md#webacltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWebACLResponseTypeDef

```python
# GetWebACLResponseTypeDef definition

class GetWebACLResponseTypeDef(TypedDict):
    WebACL: WebACLTypeDef,  # (1)
    LockToken: str,
    ApplicationIntegrationURL: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebACLTypeDef](./type_defs.md#webacltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
