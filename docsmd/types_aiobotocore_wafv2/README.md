# WAFV2 module

> [Index](../README.md) > WAFV2


!!! note ""

    Auto-generated documentation for [WAFV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
    type annotations stubs module [types-aiobotocore-wafv2](https://pypi.org/project/types-aiobotocore-wafv2/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `WAFV2` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[wafv2]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[wafv2]'


# standalone installation
python -m pip install types-aiobotocore-wafv2
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-wafv2
```

## Usage

Code samples can be found in [Examples](./usage.md).

## WAFV2Client

Type annotations and code completion for  `#!python session.create_client("wafv2")` as [WAFV2Client](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# WAFV2Client usage example

from aiobotocore.session import get_session

from types_aiobotocore_wafv2.client import WAFV2Client


session = get_session()
async with session.create_client("wafv2") as client:
    client: WAFV2Client
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionValueType usage example

from types_aiobotocore_wafv2.literals import ActionValueType

def get_value() -> ActionValueType:
    return "ALLOW"
```

- [ActionValueType](./literals.md#actionvaluetype)
- [AssociatedResourceTypeType](./literals.md#associatedresourcetypetype)
- [BodyParsingFallbackBehaviorType](./literals.md#bodyparsingfallbackbehaviortype)
- [ComparisonOperatorType](./literals.md#comparisonoperatortype)
- [CountryCodeType](./literals.md#countrycodetype)
- [FailureReasonType](./literals.md#failurereasontype)
- [FallbackBehaviorType](./literals.md#fallbackbehaviortype)
- [FilterBehaviorType](./literals.md#filterbehaviortype)
- [FilterRequirementType](./literals.md#filterrequirementtype)
- [ForwardedIPPositionType](./literals.md#forwardedippositiontype)
- [IPAddressVersionType](./literals.md#ipaddressversiontype)
- [InspectionLevelType](./literals.md#inspectionleveltype)
- [JsonMatchScopeType](./literals.md#jsonmatchscopetype)
- [LabelMatchScopeType](./literals.md#labelmatchscopetype)
- [LogScopeType](./literals.md#logscopetype)
- [LogTypeType](./literals.md#logtypetype)
- [MapMatchScopeType](./literals.md#mapmatchscopetype)
- [OversizeHandlingType](./literals.md#oversizehandlingtype)
- [PayloadTypeType](./literals.md#payloadtypetype)
- [PlatformType](./literals.md#platformtype)
- [PositionalConstraintType](./literals.md#positionalconstrainttype)
- [RateBasedStatementAggregateKeyTypeType](./literals.md#ratebasedstatementaggregatekeytypetype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [ResponseContentTypeType](./literals.md#responsecontenttypetype)
- [ScopeType](./literals.md#scopetype)
- [SensitivityLevelType](./literals.md#sensitivityleveltype)
- [SizeInspectionLimitType](./literals.md#sizeinspectionlimittype)
- [TextTransformationTypeType](./literals.md#texttransformationtypetype)
- [WAFV2ServiceName](./literals.md#wafv2servicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [APIKeySummaryTypeDef](./type_defs.md#apikeysummarytypedef)
- [AWSManagedRulesBotControlRuleSetTypeDef](./type_defs.md#awsmanagedrulesbotcontrolrulesettypedef)
- [ActionConditionTypeDef](./type_defs.md#actionconditiontypedef)
- [AddressFieldTypeDef](./type_defs.md#addressfieldtypedef)
- [AndStatementOutputTypeDef](./type_defs.md#andstatementoutputtypedef)
- [AndStatementTypeDef](./type_defs.md#andstatementtypedef)
- [AssociateWebACLRequestRequestTypeDef](./type_defs.md#associatewebaclrequestrequesttypedef)
- [RequestBodyAssociatedResourceTypeConfigTypeDef](./type_defs.md#requestbodyassociatedresourcetypeconfigtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [BodyTypeDef](./type_defs.md#bodytypedef)
- [TextTransformationTypeDef](./type_defs.md#texttransformationtypedef)
- [ImmunityTimePropertyTypeDef](./type_defs.md#immunitytimepropertytypedef)
- [CaptchaResponseTypeDef](./type_defs.md#captcharesponsetypedef)
- [ChallengeResponseTypeDef](./type_defs.md#challengeresponsetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [LabelNameConditionTypeDef](./type_defs.md#labelnameconditiontypedef)
- [CookieMatchPatternOutputTypeDef](./type_defs.md#cookiematchpatternoutputtypedef)
- [CookieMatchPatternTypeDef](./type_defs.md#cookiematchpatterntypedef)
- [CreateAPIKeyRequestRequestTypeDef](./type_defs.md#createapikeyrequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [IPSetSummaryTypeDef](./type_defs.md#ipsetsummarytypedef)
- [RegexTypeDef](./type_defs.md#regextypedef)
- [RegexPatternSetSummaryTypeDef](./type_defs.md#regexpatternsetsummarytypedef)
- [CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef)
- [VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef)
- [RuleGroupSummaryTypeDef](./type_defs.md#rulegroupsummarytypedef)
- [WebACLSummaryTypeDef](./type_defs.md#webaclsummarytypedef)
- [CustomHTTPHeaderTypeDef](./type_defs.md#customhttpheadertypedef)
- [DeleteAPIKeyRequestRequestTypeDef](./type_defs.md#deleteapikeyrequestrequesttypedef)
- [DeleteFirewallManagerRuleGroupsRequestRequestTypeDef](./type_defs.md#deletefirewallmanagerrulegroupsrequestrequesttypedef)
- [DeleteIPSetRequestRequestTypeDef](./type_defs.md#deleteipsetrequestrequesttypedef)
- [DeleteLoggingConfigurationRequestRequestTypeDef](./type_defs.md#deleteloggingconfigurationrequestrequesttypedef)
- [DeletePermissionPolicyRequestRequestTypeDef](./type_defs.md#deletepermissionpolicyrequestrequesttypedef)
- [DeleteRegexPatternSetRequestRequestTypeDef](./type_defs.md#deleteregexpatternsetrequestrequesttypedef)
- [DeleteRuleGroupRequestRequestTypeDef](./type_defs.md#deleterulegrouprequestrequesttypedef)
- [DeleteWebACLRequestRequestTypeDef](./type_defs.md#deletewebaclrequestrequesttypedef)
- [DescribeAllManagedProductsRequestRequestTypeDef](./type_defs.md#describeallmanagedproductsrequestrequesttypedef)
- [ManagedProductDescriptorTypeDef](./type_defs.md#managedproductdescriptortypedef)
- [DescribeManagedProductsByVendorRequestRequestTypeDef](./type_defs.md#describemanagedproductsbyvendorrequestrequesttypedef)
- [DescribeManagedRuleGroupRequestRequestTypeDef](./type_defs.md#describemanagedrulegrouprequestrequesttypedef)
- [LabelSummaryTypeDef](./type_defs.md#labelsummarytypedef)
- [DisassociateWebACLRequestRequestTypeDef](./type_defs.md#disassociatewebaclrequestrequesttypedef)
- [EmailFieldTypeDef](./type_defs.md#emailfieldtypedef)
- [ExcludedRuleTypeDef](./type_defs.md#excludedruletypedef)
- [HeaderOrderTypeDef](./type_defs.md#headerordertypedef)
- [JA3FingerprintTypeDef](./type_defs.md#ja3fingerprinttypedef)
- [SingleHeaderTypeDef](./type_defs.md#singleheadertypedef)
- [SingleQueryArgumentTypeDef](./type_defs.md#singlequeryargumenttypedef)
- [ForwardedIPConfigTypeDef](./type_defs.md#forwardedipconfigtypedef)
- [GenerateMobileSdkReleaseUrlRequestRequestTypeDef](./type_defs.md#generatemobilesdkreleaseurlrequestrequesttypedef)
- [GetDecryptedAPIKeyRequestRequestTypeDef](./type_defs.md#getdecryptedapikeyrequestrequesttypedef)
- [GetIPSetRequestRequestTypeDef](./type_defs.md#getipsetrequestrequesttypedef)
- [IPSetTypeDef](./type_defs.md#ipsettypedef)
- [GetLoggingConfigurationRequestRequestTypeDef](./type_defs.md#getloggingconfigurationrequestrequesttypedef)
- [GetManagedRuleSetRequestRequestTypeDef](./type_defs.md#getmanagedrulesetrequestrequesttypedef)
- [GetMobileSdkReleaseRequestRequestTypeDef](./type_defs.md#getmobilesdkreleaserequestrequesttypedef)
- [GetPermissionPolicyRequestRequestTypeDef](./type_defs.md#getpermissionpolicyrequestrequesttypedef)
- [GetRateBasedStatementManagedKeysRequestRequestTypeDef](./type_defs.md#getratebasedstatementmanagedkeysrequestrequesttypedef)
- [RateBasedStatementManagedKeysIPSetTypeDef](./type_defs.md#ratebasedstatementmanagedkeysipsettypedef)
- [GetRegexPatternSetRequestRequestTypeDef](./type_defs.md#getregexpatternsetrequestrequesttypedef)
- [GetRuleGroupRequestRequestTypeDef](./type_defs.md#getrulegrouprequestrequesttypedef)
- [TimeWindowOutputTypeDef](./type_defs.md#timewindowoutputtypedef)
- [GetWebACLForResourceRequestRequestTypeDef](./type_defs.md#getwebaclforresourcerequestrequesttypedef)
- [GetWebACLRequestRequestTypeDef](./type_defs.md#getwebaclrequestrequesttypedef)
- [HTTPHeaderTypeDef](./type_defs.md#httpheadertypedef)
- [HeaderMatchPatternOutputTypeDef](./type_defs.md#headermatchpatternoutputtypedef)
- [HeaderMatchPatternTypeDef](./type_defs.md#headermatchpatterntypedef)
- [IPSetForwardedIPConfigTypeDef](./type_defs.md#ipsetforwardedipconfigtypedef)
- [JsonMatchPatternOutputTypeDef](./type_defs.md#jsonmatchpatternoutputtypedef)
- [JsonMatchPatternTypeDef](./type_defs.md#jsonmatchpatterntypedef)
- [LabelMatchStatementTypeDef](./type_defs.md#labelmatchstatementtypedef)
- [LabelTypeDef](./type_defs.md#labeltypedef)
- [ListAPIKeysRequestRequestTypeDef](./type_defs.md#listapikeysrequestrequesttypedef)
- [ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef](./type_defs.md#listavailablemanagedrulegroupversionsrequestrequesttypedef)
- [ManagedRuleGroupVersionTypeDef](./type_defs.md#managedrulegroupversiontypedef)
- [ListAvailableManagedRuleGroupsRequestRequestTypeDef](./type_defs.md#listavailablemanagedrulegroupsrequestrequesttypedef)
- [ManagedRuleGroupSummaryTypeDef](./type_defs.md#managedrulegroupsummarytypedef)
- [ListIPSetsRequestRequestTypeDef](./type_defs.md#listipsetsrequestrequesttypedef)
- [ListLoggingConfigurationsRequestRequestTypeDef](./type_defs.md#listloggingconfigurationsrequestrequesttypedef)
- [ListManagedRuleSetsRequestRequestTypeDef](./type_defs.md#listmanagedrulesetsrequestrequesttypedef)
- [ManagedRuleSetSummaryTypeDef](./type_defs.md#managedrulesetsummarytypedef)
- [ListMobileSdkReleasesRequestRequestTypeDef](./type_defs.md#listmobilesdkreleasesrequestrequesttypedef)
- [ReleaseSummaryTypeDef](./type_defs.md#releasesummarytypedef)
- [ListRegexPatternSetsRequestRequestTypeDef](./type_defs.md#listregexpatternsetsrequestrequesttypedef)
- [ListResourcesForWebACLRequestRequestTypeDef](./type_defs.md#listresourcesforwebaclrequestrequesttypedef)
- [ListRuleGroupsRequestRequestTypeDef](./type_defs.md#listrulegroupsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWebACLsRequestRequestTypeDef](./type_defs.md#listwebaclsrequestrequesttypedef)
- [PasswordFieldTypeDef](./type_defs.md#passwordfieldtypedef)
- [UsernameFieldTypeDef](./type_defs.md#usernamefieldtypedef)
- [ManagedRuleSetVersionTypeDef](./type_defs.md#managedrulesetversiontypedef)
- [NotStatementOutputTypeDef](./type_defs.md#notstatementoutputtypedef)
- [NotStatementTypeDef](./type_defs.md#notstatementtypedef)
- [OrStatementOutputTypeDef](./type_defs.md#orstatementoutputtypedef)
- [OrStatementTypeDef](./type_defs.md#orstatementtypedef)
- [PhoneNumberFieldTypeDef](./type_defs.md#phonenumberfieldtypedef)
- [VersionToPublishTypeDef](./type_defs.md#versiontopublishtypedef)
- [PutPermissionPolicyRequestRequestTypeDef](./type_defs.md#putpermissionpolicyrequestrequesttypedef)
- [RateLimitLabelNamespaceTypeDef](./type_defs.md#ratelimitlabelnamespacetypedef)
- [ResponseInspectionBodyContainsOutputTypeDef](./type_defs.md#responseinspectionbodycontainsoutputtypedef)
- [ResponseInspectionBodyContainsTypeDef](./type_defs.md#responseinspectionbodycontainstypedef)
- [ResponseInspectionHeaderOutputTypeDef](./type_defs.md#responseinspectionheaderoutputtypedef)
- [ResponseInspectionHeaderTypeDef](./type_defs.md#responseinspectionheadertypedef)
- [ResponseInspectionJsonOutputTypeDef](./type_defs.md#responseinspectionjsonoutputtypedef)
- [ResponseInspectionJsonTypeDef](./type_defs.md#responseinspectionjsontypedef)
- [ResponseInspectionStatusCodeOutputTypeDef](./type_defs.md#responseinspectionstatuscodeoutputtypedef)
- [ResponseInspectionStatusCodeTypeDef](./type_defs.md#responseinspectionstatuscodetypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateIPSetRequestRequestTypeDef](./type_defs.md#updateipsetrequestrequesttypedef)
- [AndStatementUnionTypeDef](./type_defs.md#andstatementuniontypedef)
- [AssociationConfigOutputTypeDef](./type_defs.md#associationconfigoutputtypedef)
- [AssociationConfigTypeDef](./type_defs.md#associationconfigtypedef)
- [RateLimitCookieOutputTypeDef](./type_defs.md#ratelimitcookieoutputtypedef)
- [RateLimitCookieTypeDef](./type_defs.md#ratelimitcookietypedef)
- [RateLimitHeaderOutputTypeDef](./type_defs.md#ratelimitheaderoutputtypedef)
- [RateLimitHeaderTypeDef](./type_defs.md#ratelimitheadertypedef)
- [RateLimitQueryArgumentOutputTypeDef](./type_defs.md#ratelimitqueryargumentoutputtypedef)
- [RateLimitQueryArgumentTypeDef](./type_defs.md#ratelimitqueryargumenttypedef)
- [RateLimitQueryStringOutputTypeDef](./type_defs.md#ratelimitquerystringoutputtypedef)
- [RateLimitQueryStringTypeDef](./type_defs.md#ratelimitquerystringtypedef)
- [RateLimitUriPathOutputTypeDef](./type_defs.md#ratelimituripathoutputtypedef)
- [RateLimitUriPathTypeDef](./type_defs.md#ratelimituripathtypedef)
- [CaptchaConfigTypeDef](./type_defs.md#captchaconfigtypedef)
- [ChallengeConfigTypeDef](./type_defs.md#challengeconfigtypedef)
- [CheckCapacityResponseTypeDef](./type_defs.md#checkcapacityresponsetypedef)
- [CreateAPIKeyResponseTypeDef](./type_defs.md#createapikeyresponsetypedef)
- [DeleteFirewallManagerRuleGroupsResponseTypeDef](./type_defs.md#deletefirewallmanagerrulegroupsresponsetypedef)
- [GenerateMobileSdkReleaseUrlResponseTypeDef](./type_defs.md#generatemobilesdkreleaseurlresponsetypedef)
- [GetDecryptedAPIKeyResponseTypeDef](./type_defs.md#getdecryptedapikeyresponsetypedef)
- [GetPermissionPolicyResponseTypeDef](./type_defs.md#getpermissionpolicyresponsetypedef)
- [ListAPIKeysResponseTypeDef](./type_defs.md#listapikeysresponsetypedef)
- [ListResourcesForWebACLResponseTypeDef](./type_defs.md#listresourcesforwebaclresponsetypedef)
- [PutManagedRuleSetVersionsResponseTypeDef](./type_defs.md#putmanagedrulesetversionsresponsetypedef)
- [UpdateIPSetResponseTypeDef](./type_defs.md#updateipsetresponsetypedef)
- [UpdateManagedRuleSetVersionExpiryDateResponseTypeDef](./type_defs.md#updatemanagedrulesetversionexpirydateresponsetypedef)
- [UpdateRegexPatternSetResponseTypeDef](./type_defs.md#updateregexpatternsetresponsetypedef)
- [UpdateRuleGroupResponseTypeDef](./type_defs.md#updaterulegroupresponsetypedef)
- [UpdateWebACLResponseTypeDef](./type_defs.md#updatewebaclresponsetypedef)
- [ConditionTypeDef](./type_defs.md#conditiontypedef)
- [CookiesOutputTypeDef](./type_defs.md#cookiesoutputtypedef)
- [CookieMatchPatternUnionTypeDef](./type_defs.md#cookiematchpatternuniontypedef)
- [CreateIPSetRequestRequestTypeDef](./type_defs.md#createipsetrequestrequesttypedef)
- [MobileSdkReleaseTypeDef](./type_defs.md#mobilesdkreleasetypedef)
- [TagInfoForResourceTypeDef](./type_defs.md#taginfoforresourcetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateIPSetResponseTypeDef](./type_defs.md#createipsetresponsetypedef)
- [ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef)
- [CreateRegexPatternSetRequestRequestTypeDef](./type_defs.md#createregexpatternsetrequestrequesttypedef)
- [RegexPatternSetTypeDef](./type_defs.md#regexpatternsettypedef)
- [UpdateRegexPatternSetRequestRequestTypeDef](./type_defs.md#updateregexpatternsetrequestrequesttypedef)
- [CreateRegexPatternSetResponseTypeDef](./type_defs.md#createregexpatternsetresponsetypedef)
- [ListRegexPatternSetsResponseTypeDef](./type_defs.md#listregexpatternsetsresponsetypedef)
- [CreateRuleGroupResponseTypeDef](./type_defs.md#createrulegroupresponsetypedef)
- [ListRuleGroupsResponseTypeDef](./type_defs.md#listrulegroupsresponsetypedef)
- [CreateWebACLResponseTypeDef](./type_defs.md#createwebaclresponsetypedef)
- [ListWebACLsResponseTypeDef](./type_defs.md#listwebaclsresponsetypedef)
- [CustomRequestHandlingOutputTypeDef](./type_defs.md#customrequesthandlingoutputtypedef)
- [CustomRequestHandlingTypeDef](./type_defs.md#customrequesthandlingtypedef)
- [CustomResponseOutputTypeDef](./type_defs.md#customresponseoutputtypedef)
- [CustomResponseTypeDef](./type_defs.md#customresponsetypedef)
- [DescribeAllManagedProductsResponseTypeDef](./type_defs.md#describeallmanagedproductsresponsetypedef)
- [DescribeManagedProductsByVendorResponseTypeDef](./type_defs.md#describemanagedproductsbyvendorresponsetypedef)
- [GeoMatchStatementOutputTypeDef](./type_defs.md#geomatchstatementoutputtypedef)
- [GeoMatchStatementTypeDef](./type_defs.md#geomatchstatementtypedef)
- [GetIPSetResponseTypeDef](./type_defs.md#getipsetresponsetypedef)
- [GetRateBasedStatementManagedKeysResponseTypeDef](./type_defs.md#getratebasedstatementmanagedkeysresponsetypedef)
- [HTTPRequestTypeDef](./type_defs.md#httprequesttypedef)
- [HeadersOutputTypeDef](./type_defs.md#headersoutputtypedef)
- [HeaderMatchPatternUnionTypeDef](./type_defs.md#headermatchpatternuniontypedef)
- [IPSetReferenceStatementTypeDef](./type_defs.md#ipsetreferencestatementtypedef)
- [JsonBodyOutputTypeDef](./type_defs.md#jsonbodyoutputtypedef)
- [JsonMatchPatternUnionTypeDef](./type_defs.md#jsonmatchpatternuniontypedef)
- [ListAvailableManagedRuleGroupVersionsResponseTypeDef](./type_defs.md#listavailablemanagedrulegroupversionsresponsetypedef)
- [ListAvailableManagedRuleGroupsResponseTypeDef](./type_defs.md#listavailablemanagedrulegroupsresponsetypedef)
- [ListManagedRuleSetsResponseTypeDef](./type_defs.md#listmanagedrulesetsresponsetypedef)
- [ListMobileSdkReleasesResponseTypeDef](./type_defs.md#listmobilesdkreleasesresponsetypedef)
- [RequestInspectionTypeDef](./type_defs.md#requestinspectiontypedef)
- [ManagedRuleSetTypeDef](./type_defs.md#managedrulesettypedef)
- [NotStatementUnionTypeDef](./type_defs.md#notstatementuniontypedef)
- [OrStatementUnionTypeDef](./type_defs.md#orstatementuniontypedef)
- [RequestInspectionACFPOutputTypeDef](./type_defs.md#requestinspectionacfpoutputtypedef)
- [RequestInspectionACFPTypeDef](./type_defs.md#requestinspectionacfptypedef)
- [PutManagedRuleSetVersionsRequestRequestTypeDef](./type_defs.md#putmanagedrulesetversionsrequestrequesttypedef)
- [ResponseInspectionBodyContainsUnionTypeDef](./type_defs.md#responseinspectionbodycontainsuniontypedef)
- [ResponseInspectionHeaderUnionTypeDef](./type_defs.md#responseinspectionheaderuniontypedef)
- [ResponseInspectionJsonUnionTypeDef](./type_defs.md#responseinspectionjsonuniontypedef)
- [ResponseInspectionOutputTypeDef](./type_defs.md#responseinspectionoutputtypedef)
- [ResponseInspectionStatusCodeUnionTypeDef](./type_defs.md#responseinspectionstatuscodeuniontypedef)
- [TimeWindowTypeDef](./type_defs.md#timewindowtypedef)
- [UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef](./type_defs.md#updatemanagedrulesetversionexpirydaterequestrequesttypedef)
- [RateLimitCookieUnionTypeDef](./type_defs.md#ratelimitcookieuniontypedef)
- [RateLimitHeaderUnionTypeDef](./type_defs.md#ratelimitheaderuniontypedef)
- [RateLimitQueryArgumentUnionTypeDef](./type_defs.md#ratelimitqueryargumentuniontypedef)
- [RateLimitQueryStringUnionTypeDef](./type_defs.md#ratelimitquerystringuniontypedef)
- [RateBasedStatementCustomKeyOutputTypeDef](./type_defs.md#ratebasedstatementcustomkeyoutputtypedef)
- [RateLimitUriPathUnionTypeDef](./type_defs.md#ratelimituripathuniontypedef)
- [FilterOutputTypeDef](./type_defs.md#filteroutputtypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [CookiesTypeDef](./type_defs.md#cookiestypedef)
- [GetMobileSdkReleaseResponseTypeDef](./type_defs.md#getmobilesdkreleaseresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [GetRegexPatternSetResponseTypeDef](./type_defs.md#getregexpatternsetresponsetypedef)
- [AllowActionOutputTypeDef](./type_defs.md#allowactionoutputtypedef)
- [CaptchaActionOutputTypeDef](./type_defs.md#captchaactionoutputtypedef)
- [ChallengeActionOutputTypeDef](./type_defs.md#challengeactionoutputtypedef)
- [CountActionOutputTypeDef](./type_defs.md#countactionoutputtypedef)
- [CustomRequestHandlingUnionTypeDef](./type_defs.md#customrequesthandlinguniontypedef)
- [BlockActionOutputTypeDef](./type_defs.md#blockactionoutputtypedef)
- [CustomResponseUnionTypeDef](./type_defs.md#customresponseuniontypedef)
- [GeoMatchStatementUnionTypeDef](./type_defs.md#geomatchstatementuniontypedef)
- [SampledHTTPRequestTypeDef](./type_defs.md#sampledhttprequesttypedef)
- [HeadersTypeDef](./type_defs.md#headerstypedef)
- [FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef)
- [JsonBodyTypeDef](./type_defs.md#jsonbodytypedef)
- [GetManagedRuleSetResponseTypeDef](./type_defs.md#getmanagedrulesetresponsetypedef)
- [RequestInspectionACFPUnionTypeDef](./type_defs.md#requestinspectionacfpuniontypedef)
- [AWSManagedRulesACFPRuleSetOutputTypeDef](./type_defs.md#awsmanagedrulesacfprulesetoutputtypedef)
- [AWSManagedRulesATPRuleSetOutputTypeDef](./type_defs.md#awsmanagedrulesatprulesetoutputtypedef)
- [ResponseInspectionTypeDef](./type_defs.md#responseinspectiontypedef)
- [GetSampledRequestsRequestRequestTypeDef](./type_defs.md#getsampledrequestsrequestrequesttypedef)
- [RateBasedStatementOutputTypeDef](./type_defs.md#ratebasedstatementoutputtypedef)
- [RateBasedStatementCustomKeyTypeDef](./type_defs.md#ratebasedstatementcustomkeytypedef)
- [LoggingFilterOutputTypeDef](./type_defs.md#loggingfilteroutputtypedef)
- [FilterUnionTypeDef](./type_defs.md#filteruniontypedef)
- [CookiesUnionTypeDef](./type_defs.md#cookiesuniontypedef)
- [OverrideActionOutputTypeDef](./type_defs.md#overrideactionoutputtypedef)
- [AllowActionTypeDef](./type_defs.md#allowactiontypedef)
- [CaptchaActionTypeDef](./type_defs.md#captchaactiontypedef)
- [ChallengeActionTypeDef](./type_defs.md#challengeactiontypedef)
- [CountActionTypeDef](./type_defs.md#countactiontypedef)
- [DefaultActionOutputTypeDef](./type_defs.md#defaultactionoutputtypedef)
- [RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef)
- [BlockActionTypeDef](./type_defs.md#blockactiontypedef)
- [GetSampledRequestsResponseTypeDef](./type_defs.md#getsampledrequestsresponsetypedef)
- [HeadersUnionTypeDef](./type_defs.md#headersuniontypedef)
- [ByteMatchStatementOutputTypeDef](./type_defs.md#bytematchstatementoutputtypedef)
- [RegexMatchStatementOutputTypeDef](./type_defs.md#regexmatchstatementoutputtypedef)
- [RegexPatternSetReferenceStatementOutputTypeDef](./type_defs.md#regexpatternsetreferencestatementoutputtypedef)
- [SizeConstraintStatementOutputTypeDef](./type_defs.md#sizeconstraintstatementoutputtypedef)
- [SqliMatchStatementOutputTypeDef](./type_defs.md#sqlimatchstatementoutputtypedef)
- [XssMatchStatementOutputTypeDef](./type_defs.md#xssmatchstatementoutputtypedef)
- [JsonBodyUnionTypeDef](./type_defs.md#jsonbodyuniontypedef)
- [ManagedRuleGroupConfigOutputTypeDef](./type_defs.md#managedrulegroupconfigoutputtypedef)
- [ResponseInspectionUnionTypeDef](./type_defs.md#responseinspectionuniontypedef)
- [RateBasedStatementCustomKeyUnionTypeDef](./type_defs.md#ratebasedstatementcustomkeyuniontypedef)
- [LoggingConfigurationOutputTypeDef](./type_defs.md#loggingconfigurationoutputtypedef)
- [LoggingFilterTypeDef](./type_defs.md#loggingfiltertypedef)
- [AllowActionUnionTypeDef](./type_defs.md#allowactionuniontypedef)
- [CaptchaActionUnionTypeDef](./type_defs.md#captchaactionuniontypedef)
- [ChallengeActionUnionTypeDef](./type_defs.md#challengeactionuniontypedef)
- [CountActionUnionTypeDef](./type_defs.md#countactionuniontypedef)
- [RuleActionOverrideOutputTypeDef](./type_defs.md#ruleactionoverrideoutputtypedef)
- [RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef)
- [BlockActionUnionTypeDef](./type_defs.md#blockactionuniontypedef)
- [FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef)
- [AWSManagedRulesACFPRuleSetTypeDef](./type_defs.md#awsmanagedrulesacfprulesettypedef)
- [AWSManagedRulesATPRuleSetTypeDef](./type_defs.md#awsmanagedrulesatprulesettypedef)
- [RateBasedStatementTypeDef](./type_defs.md#ratebasedstatementtypedef)
- [GetLoggingConfigurationResponseTypeDef](./type_defs.md#getloggingconfigurationresponsetypedef)
- [ListLoggingConfigurationsResponseTypeDef](./type_defs.md#listloggingconfigurationsresponsetypedef)
- [PutLoggingConfigurationResponseTypeDef](./type_defs.md#putloggingconfigurationresponsetypedef)
- [LoggingFilterUnionTypeDef](./type_defs.md#loggingfilteruniontypedef)
- [OverrideActionTypeDef](./type_defs.md#overrideactiontypedef)
- [ManagedRuleGroupStatementOutputTypeDef](./type_defs.md#managedrulegroupstatementoutputtypedef)
- [RuleGroupReferenceStatementOutputTypeDef](./type_defs.md#rulegroupreferencestatementoutputtypedef)
- [DescribeManagedRuleGroupResponseTypeDef](./type_defs.md#describemanagedrulegroupresponsetypedef)
- [DefaultActionTypeDef](./type_defs.md#defaultactiontypedef)
- [RuleActionTypeDef](./type_defs.md#ruleactiontypedef)
- [FieldToMatchUnionTypeDef](./type_defs.md#fieldtomatchuniontypedef)
- [AWSManagedRulesACFPRuleSetUnionTypeDef](./type_defs.md#awsmanagedrulesacfprulesetuniontypedef)
- [AWSManagedRulesATPRuleSetUnionTypeDef](./type_defs.md#awsmanagedrulesatprulesetuniontypedef)
- [RateBasedStatementUnionTypeDef](./type_defs.md#ratebasedstatementuniontypedef)
- [OverrideActionUnionTypeDef](./type_defs.md#overrideactionuniontypedef)
- [FirewallManagerStatementTypeDef](./type_defs.md#firewallmanagerstatementtypedef)
- [StatementOutputTypeDef](./type_defs.md#statementoutputtypedef)
- [RuleActionUnionTypeDef](./type_defs.md#ruleactionuniontypedef)
- [ByteMatchStatementTypeDef](./type_defs.md#bytematchstatementtypedef)
- [LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef)
- [RegexMatchStatementTypeDef](./type_defs.md#regexmatchstatementtypedef)
- [RegexPatternSetReferenceStatementTypeDef](./type_defs.md#regexpatternsetreferencestatementtypedef)
- [SizeConstraintStatementTypeDef](./type_defs.md#sizeconstraintstatementtypedef)
- [SqliMatchStatementTypeDef](./type_defs.md#sqlimatchstatementtypedef)
- [XssMatchStatementTypeDef](./type_defs.md#xssmatchstatementtypedef)
- [ManagedRuleGroupConfigTypeDef](./type_defs.md#managedrulegroupconfigtypedef)
- [FirewallManagerRuleGroupTypeDef](./type_defs.md#firewallmanagerrulegrouptypedef)
- [RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef)
- [RuleActionOverrideTypeDef](./type_defs.md#ruleactionoverridetypedef)
- [ByteMatchStatementUnionTypeDef](./type_defs.md#bytematchstatementuniontypedef)
- [PutLoggingConfigurationRequestRequestTypeDef](./type_defs.md#putloggingconfigurationrequestrequesttypedef)
- [RegexMatchStatementUnionTypeDef](./type_defs.md#regexmatchstatementuniontypedef)
- [RegexPatternSetReferenceStatementUnionTypeDef](./type_defs.md#regexpatternsetreferencestatementuniontypedef)
- [SizeConstraintStatementUnionTypeDef](./type_defs.md#sizeconstraintstatementuniontypedef)
- [SqliMatchStatementUnionTypeDef](./type_defs.md#sqlimatchstatementuniontypedef)
- [XssMatchStatementUnionTypeDef](./type_defs.md#xssmatchstatementuniontypedef)
- [ManagedRuleGroupConfigUnionTypeDef](./type_defs.md#managedrulegroupconfiguniontypedef)
- [RuleGroupTypeDef](./type_defs.md#rulegrouptypedef)
- [WebACLTypeDef](./type_defs.md#webacltypedef)
- [RuleActionOverrideUnionTypeDef](./type_defs.md#ruleactionoverrideuniontypedef)
- [ManagedRuleGroupStatementTypeDef](./type_defs.md#managedrulegroupstatementtypedef)
- [GetRuleGroupResponseTypeDef](./type_defs.md#getrulegroupresponsetypedef)
- [GetWebACLForResourceResponseTypeDef](./type_defs.md#getwebaclforresourceresponsetypedef)
- [GetWebACLResponseTypeDef](./type_defs.md#getwebaclresponsetypedef)
- [RuleGroupReferenceStatementTypeDef](./type_defs.md#rulegroupreferencestatementtypedef)
- [ManagedRuleGroupStatementUnionTypeDef](./type_defs.md#managedrulegroupstatementuniontypedef)
- [RuleGroupReferenceStatementUnionTypeDef](./type_defs.md#rulegroupreferencestatementuniontypedef)
- [StatementTypeDef](./type_defs.md#statementtypedef)
- [StatementUnionTypeDef](./type_defs.md#statementuniontypedef)
- [RuleTypeDef](./type_defs.md#ruletypedef)
- [CreateRuleGroupRequestRequestTypeDef](./type_defs.md#createrulegrouprequestrequesttypedef)
- [CreateWebACLRequestRequestTypeDef](./type_defs.md#createwebaclrequestrequesttypedef)
- [RuleUnionTypeDef](./type_defs.md#ruleuniontypedef)
- [UpdateRuleGroupRequestRequestTypeDef](./type_defs.md#updaterulegrouprequestrequesttypedef)
- [UpdateWebACLRequestRequestTypeDef](./type_defs.md#updatewebaclrequestrequesttypedef)
- [CheckCapacityRequestRequestTypeDef](./type_defs.md#checkcapacityrequestrequesttypedef)

