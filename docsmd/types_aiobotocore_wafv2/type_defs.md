# Type definitions

> [Index](../README.md) > [WAFV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [WAFV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#wafv2)
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


## AndStatementUnionTypeDef

```python
# AndStatementUnionTypeDef definition

AndStatementUnionTypeDef = Union[
    AndStatementTypeDef,  # (1)
    AndStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AndStatementTypeDef](./type_defs.md#andstatementtypedef) 
2. See [:material-code-braces: AndStatementOutputTypeDef](./type_defs.md#andstatementoutputtypedef) 

## CookieMatchPatternUnionTypeDef

```python
# CookieMatchPatternUnionTypeDef definition

CookieMatchPatternUnionTypeDef = Union[
    CookieMatchPatternTypeDef,  # (1)
    CookieMatchPatternOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CookieMatchPatternTypeDef](./type_defs.md#cookiematchpatterntypedef) 
2. See [:material-code-braces: CookieMatchPatternOutputTypeDef](./type_defs.md#cookiematchpatternoutputtypedef) 

## HeaderMatchPatternUnionTypeDef

```python
# HeaderMatchPatternUnionTypeDef definition

HeaderMatchPatternUnionTypeDef = Union[
    HeaderMatchPatternTypeDef,  # (1)
    HeaderMatchPatternOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HeaderMatchPatternTypeDef](./type_defs.md#headermatchpatterntypedef) 
2. See [:material-code-braces: HeaderMatchPatternOutputTypeDef](./type_defs.md#headermatchpatternoutputtypedef) 

## JsonMatchPatternUnionTypeDef

```python
# JsonMatchPatternUnionTypeDef definition

JsonMatchPatternUnionTypeDef = Union[
    JsonMatchPatternTypeDef,  # (1)
    JsonMatchPatternOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JsonMatchPatternTypeDef](./type_defs.md#jsonmatchpatterntypedef) 
2. See [:material-code-braces: JsonMatchPatternOutputTypeDef](./type_defs.md#jsonmatchpatternoutputtypedef) 

## NotStatementUnionTypeDef

```python
# NotStatementUnionTypeDef definition

NotStatementUnionTypeDef = Union[
    NotStatementTypeDef,  # (1)
    NotStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NotStatementTypeDef](./type_defs.md#notstatementtypedef) 
2. See [:material-code-braces: NotStatementOutputTypeDef](./type_defs.md#notstatementoutputtypedef) 

## OrStatementUnionTypeDef

```python
# OrStatementUnionTypeDef definition

OrStatementUnionTypeDef = Union[
    OrStatementTypeDef,  # (1)
    OrStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OrStatementTypeDef](./type_defs.md#orstatementtypedef) 
2. See [:material-code-braces: OrStatementOutputTypeDef](./type_defs.md#orstatementoutputtypedef) 

## ResponseInspectionBodyContainsUnionTypeDef

```python
# ResponseInspectionBodyContainsUnionTypeDef definition

ResponseInspectionBodyContainsUnionTypeDef = Union[
    ResponseInspectionBodyContainsTypeDef,  # (1)
    ResponseInspectionBodyContainsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResponseInspectionBodyContainsTypeDef](./type_defs.md#responseinspectionbodycontainstypedef) 
2. See [:material-code-braces: ResponseInspectionBodyContainsOutputTypeDef](./type_defs.md#responseinspectionbodycontainsoutputtypedef) 

## ResponseInspectionHeaderUnionTypeDef

```python
# ResponseInspectionHeaderUnionTypeDef definition

ResponseInspectionHeaderUnionTypeDef = Union[
    ResponseInspectionHeaderTypeDef,  # (1)
    ResponseInspectionHeaderOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResponseInspectionHeaderTypeDef](./type_defs.md#responseinspectionheadertypedef) 
2. See [:material-code-braces: ResponseInspectionHeaderOutputTypeDef](./type_defs.md#responseinspectionheaderoutputtypedef) 

## ResponseInspectionJsonUnionTypeDef

```python
# ResponseInspectionJsonUnionTypeDef definition

ResponseInspectionJsonUnionTypeDef = Union[
    ResponseInspectionJsonTypeDef,  # (1)
    ResponseInspectionJsonOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResponseInspectionJsonTypeDef](./type_defs.md#responseinspectionjsontypedef) 
2. See [:material-code-braces: ResponseInspectionJsonOutputTypeDef](./type_defs.md#responseinspectionjsonoutputtypedef) 

## ResponseInspectionStatusCodeUnionTypeDef

```python
# ResponseInspectionStatusCodeUnionTypeDef definition

ResponseInspectionStatusCodeUnionTypeDef = Union[
    ResponseInspectionStatusCodeTypeDef,  # (1)
    ResponseInspectionStatusCodeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResponseInspectionStatusCodeTypeDef](./type_defs.md#responseinspectionstatuscodetypedef) 
2. See [:material-code-braces: ResponseInspectionStatusCodeOutputTypeDef](./type_defs.md#responseinspectionstatuscodeoutputtypedef) 

## RateLimitCookieUnionTypeDef

```python
# RateLimitCookieUnionTypeDef definition

RateLimitCookieUnionTypeDef = Union[
    RateLimitCookieTypeDef,  # (1)
    RateLimitCookieOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RateLimitCookieTypeDef](./type_defs.md#ratelimitcookietypedef) 
2. See [:material-code-braces: RateLimitCookieOutputTypeDef](./type_defs.md#ratelimitcookieoutputtypedef) 

## RateLimitHeaderUnionTypeDef

```python
# RateLimitHeaderUnionTypeDef definition

RateLimitHeaderUnionTypeDef = Union[
    RateLimitHeaderTypeDef,  # (1)
    RateLimitHeaderOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RateLimitHeaderTypeDef](./type_defs.md#ratelimitheadertypedef) 
2. See [:material-code-braces: RateLimitHeaderOutputTypeDef](./type_defs.md#ratelimitheaderoutputtypedef) 

## RateLimitQueryArgumentUnionTypeDef

```python
# RateLimitQueryArgumentUnionTypeDef definition

RateLimitQueryArgumentUnionTypeDef = Union[
    RateLimitQueryArgumentTypeDef,  # (1)
    RateLimitQueryArgumentOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RateLimitQueryArgumentTypeDef](./type_defs.md#ratelimitqueryargumenttypedef) 
2. See [:material-code-braces: RateLimitQueryArgumentOutputTypeDef](./type_defs.md#ratelimitqueryargumentoutputtypedef) 

## RateLimitQueryStringUnionTypeDef

```python
# RateLimitQueryStringUnionTypeDef definition

RateLimitQueryStringUnionTypeDef = Union[
    RateLimitQueryStringTypeDef,  # (1)
    RateLimitQueryStringOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RateLimitQueryStringTypeDef](./type_defs.md#ratelimitquerystringtypedef) 
2. See [:material-code-braces: RateLimitQueryStringOutputTypeDef](./type_defs.md#ratelimitquerystringoutputtypedef) 

## RateLimitUriPathUnionTypeDef

```python
# RateLimitUriPathUnionTypeDef definition

RateLimitUriPathUnionTypeDef = Union[
    RateLimitUriPathTypeDef,  # (1)
    RateLimitUriPathOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RateLimitUriPathTypeDef](./type_defs.md#ratelimituripathtypedef) 
2. See [:material-code-braces: RateLimitUriPathOutputTypeDef](./type_defs.md#ratelimituripathoutputtypedef) 

## CustomRequestHandlingUnionTypeDef

```python
# CustomRequestHandlingUnionTypeDef definition

CustomRequestHandlingUnionTypeDef = Union[
    CustomRequestHandlingTypeDef,  # (1)
    CustomRequestHandlingOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomRequestHandlingTypeDef](./type_defs.md#customrequesthandlingtypedef) 
2. See [:material-code-braces: CustomRequestHandlingOutputTypeDef](./type_defs.md#customrequesthandlingoutputtypedef) 

## CustomResponseUnionTypeDef

```python
# CustomResponseUnionTypeDef definition

CustomResponseUnionTypeDef = Union[
    CustomResponseTypeDef,  # (1)
    CustomResponseOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomResponseTypeDef](./type_defs.md#customresponsetypedef) 
2. See [:material-code-braces: CustomResponseOutputTypeDef](./type_defs.md#customresponseoutputtypedef) 

## GeoMatchStatementUnionTypeDef

```python
# GeoMatchStatementUnionTypeDef definition

GeoMatchStatementUnionTypeDef = Union[
    GeoMatchStatementTypeDef,  # (1)
    GeoMatchStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GeoMatchStatementTypeDef](./type_defs.md#geomatchstatementtypedef) 
2. See [:material-code-braces: GeoMatchStatementOutputTypeDef](./type_defs.md#geomatchstatementoutputtypedef) 

## RequestInspectionACFPUnionTypeDef

```python
# RequestInspectionACFPUnionTypeDef definition

RequestInspectionACFPUnionTypeDef = Union[
    RequestInspectionACFPTypeDef,  # (1)
    RequestInspectionACFPOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RequestInspectionACFPTypeDef](./type_defs.md#requestinspectionacfptypedef) 
2. See [:material-code-braces: RequestInspectionACFPOutputTypeDef](./type_defs.md#requestinspectionacfpoutputtypedef) 

## FilterUnionTypeDef

```python
# FilterUnionTypeDef definition

FilterUnionTypeDef = Union[
    FilterTypeDef,  # (1)
    FilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: FilterOutputTypeDef](./type_defs.md#filteroutputtypedef) 

## CookiesUnionTypeDef

```python
# CookiesUnionTypeDef definition

CookiesUnionTypeDef = Union[
    CookiesTypeDef,  # (1)
    CookiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CookiesTypeDef](./type_defs.md#cookiestypedef) 
2. See [:material-code-braces: CookiesOutputTypeDef](./type_defs.md#cookiesoutputtypedef) 

## HeadersUnionTypeDef

```python
# HeadersUnionTypeDef definition

HeadersUnionTypeDef = Union[
    HeadersTypeDef,  # (1)
    HeadersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HeadersTypeDef](./type_defs.md#headerstypedef) 
2. See [:material-code-braces: HeadersOutputTypeDef](./type_defs.md#headersoutputtypedef) 

## JsonBodyUnionTypeDef

```python
# JsonBodyUnionTypeDef definition

JsonBodyUnionTypeDef = Union[
    JsonBodyTypeDef,  # (1)
    JsonBodyOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JsonBodyTypeDef](./type_defs.md#jsonbodytypedef) 
2. See [:material-code-braces: JsonBodyOutputTypeDef](./type_defs.md#jsonbodyoutputtypedef) 

## ResponseInspectionUnionTypeDef

```python
# ResponseInspectionUnionTypeDef definition

ResponseInspectionUnionTypeDef = Union[
    ResponseInspectionTypeDef,  # (1)
    ResponseInspectionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResponseInspectionTypeDef](./type_defs.md#responseinspectiontypedef) 
2. See [:material-code-braces: ResponseInspectionOutputTypeDef](./type_defs.md#responseinspectionoutputtypedef) 

## RateBasedStatementCustomKeyUnionTypeDef

```python
# RateBasedStatementCustomKeyUnionTypeDef definition

RateBasedStatementCustomKeyUnionTypeDef = Union[
    RateBasedStatementCustomKeyTypeDef,  # (1)
    RateBasedStatementCustomKeyOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RateBasedStatementCustomKeyTypeDef](./type_defs.md#ratebasedstatementcustomkeytypedef) 
2. See [:material-code-braces: RateBasedStatementCustomKeyOutputTypeDef](./type_defs.md#ratebasedstatementcustomkeyoutputtypedef) 

## AllowActionUnionTypeDef

```python
# AllowActionUnionTypeDef definition

AllowActionUnionTypeDef = Union[
    AllowActionTypeDef,  # (1)
    AllowActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AllowActionTypeDef](./type_defs.md#allowactiontypedef) 
2. See [:material-code-braces: AllowActionOutputTypeDef](./type_defs.md#allowactionoutputtypedef) 

## CaptchaActionUnionTypeDef

```python
# CaptchaActionUnionTypeDef definition

CaptchaActionUnionTypeDef = Union[
    CaptchaActionTypeDef,  # (1)
    CaptchaActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CaptchaActionTypeDef](./type_defs.md#captchaactiontypedef) 
2. See [:material-code-braces: CaptchaActionOutputTypeDef](./type_defs.md#captchaactionoutputtypedef) 

## ChallengeActionUnionTypeDef

```python
# ChallengeActionUnionTypeDef definition

ChallengeActionUnionTypeDef = Union[
    ChallengeActionTypeDef,  # (1)
    ChallengeActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ChallengeActionTypeDef](./type_defs.md#challengeactiontypedef) 
2. See [:material-code-braces: ChallengeActionOutputTypeDef](./type_defs.md#challengeactionoutputtypedef) 

## CountActionUnionTypeDef

```python
# CountActionUnionTypeDef definition

CountActionUnionTypeDef = Union[
    CountActionTypeDef,  # (1)
    CountActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CountActionTypeDef](./type_defs.md#countactiontypedef) 
2. See [:material-code-braces: CountActionOutputTypeDef](./type_defs.md#countactionoutputtypedef) 

## BlockActionUnionTypeDef

```python
# BlockActionUnionTypeDef definition

BlockActionUnionTypeDef = Union[
    BlockActionTypeDef,  # (1)
    BlockActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BlockActionTypeDef](./type_defs.md#blockactiontypedef) 
2. See [:material-code-braces: BlockActionOutputTypeDef](./type_defs.md#blockactionoutputtypedef) 

## LoggingFilterUnionTypeDef

```python
# LoggingFilterUnionTypeDef definition

LoggingFilterUnionTypeDef = Union[
    LoggingFilterTypeDef,  # (1)
    LoggingFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LoggingFilterTypeDef](./type_defs.md#loggingfiltertypedef) 
2. See [:material-code-braces: LoggingFilterOutputTypeDef](./type_defs.md#loggingfilteroutputtypedef) 

## FieldToMatchUnionTypeDef

```python
# FieldToMatchUnionTypeDef definition

FieldToMatchUnionTypeDef = Union[
    FieldToMatchTypeDef,  # (1)
    FieldToMatchOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 

## AWSManagedRulesACFPRuleSetUnionTypeDef

```python
# AWSManagedRulesACFPRuleSetUnionTypeDef definition

AWSManagedRulesACFPRuleSetUnionTypeDef = Union[
    AWSManagedRulesACFPRuleSetTypeDef,  # (1)
    AWSManagedRulesACFPRuleSetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AWSManagedRulesACFPRuleSetTypeDef](./type_defs.md#awsmanagedrulesacfprulesettypedef) 
2. See [:material-code-braces: AWSManagedRulesACFPRuleSetOutputTypeDef](./type_defs.md#awsmanagedrulesacfprulesetoutputtypedef) 

## AWSManagedRulesATPRuleSetUnionTypeDef

```python
# AWSManagedRulesATPRuleSetUnionTypeDef definition

AWSManagedRulesATPRuleSetUnionTypeDef = Union[
    AWSManagedRulesATPRuleSetTypeDef,  # (1)
    AWSManagedRulesATPRuleSetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AWSManagedRulesATPRuleSetTypeDef](./type_defs.md#awsmanagedrulesatprulesettypedef) 
2. See [:material-code-braces: AWSManagedRulesATPRuleSetOutputTypeDef](./type_defs.md#awsmanagedrulesatprulesetoutputtypedef) 

## RateBasedStatementUnionTypeDef

```python
# RateBasedStatementUnionTypeDef definition

RateBasedStatementUnionTypeDef = Union[
    RateBasedStatementTypeDef,  # (1)
    RateBasedStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RateBasedStatementTypeDef](./type_defs.md#ratebasedstatementtypedef) 
2. See [:material-code-braces: RateBasedStatementOutputTypeDef](./type_defs.md#ratebasedstatementoutputtypedef) 

## OverrideActionUnionTypeDef

```python
# OverrideActionUnionTypeDef definition

OverrideActionUnionTypeDef = Union[
    OverrideActionTypeDef,  # (1)
    OverrideActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OverrideActionTypeDef](./type_defs.md#overrideactiontypedef) 
2. See [:material-code-braces: OverrideActionOutputTypeDef](./type_defs.md#overrideactionoutputtypedef) 

## RuleActionUnionTypeDef

```python
# RuleActionUnionTypeDef definition

RuleActionUnionTypeDef = Union[
    RuleActionTypeDef,  # (1)
    RuleActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
2. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 

## ByteMatchStatementUnionTypeDef

```python
# ByteMatchStatementUnionTypeDef definition

ByteMatchStatementUnionTypeDef = Union[
    ByteMatchStatementTypeDef,  # (1)
    ByteMatchStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ByteMatchStatementTypeDef](./type_defs.md#bytematchstatementtypedef) 
2. See [:material-code-braces: ByteMatchStatementOutputTypeDef](./type_defs.md#bytematchstatementoutputtypedef) 

## RegexMatchStatementUnionTypeDef

```python
# RegexMatchStatementUnionTypeDef definition

RegexMatchStatementUnionTypeDef = Union[
    RegexMatchStatementTypeDef,  # (1)
    RegexMatchStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RegexMatchStatementTypeDef](./type_defs.md#regexmatchstatementtypedef) 
2. See [:material-code-braces: RegexMatchStatementOutputTypeDef](./type_defs.md#regexmatchstatementoutputtypedef) 

## RegexPatternSetReferenceStatementUnionTypeDef

```python
# RegexPatternSetReferenceStatementUnionTypeDef definition

RegexPatternSetReferenceStatementUnionTypeDef = Union[
    RegexPatternSetReferenceStatementTypeDef,  # (1)
    RegexPatternSetReferenceStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RegexPatternSetReferenceStatementTypeDef](./type_defs.md#regexpatternsetreferencestatementtypedef) 
2. See [:material-code-braces: RegexPatternSetReferenceStatementOutputTypeDef](./type_defs.md#regexpatternsetreferencestatementoutputtypedef) 

## SizeConstraintStatementUnionTypeDef

```python
# SizeConstraintStatementUnionTypeDef definition

SizeConstraintStatementUnionTypeDef = Union[
    SizeConstraintStatementTypeDef,  # (1)
    SizeConstraintStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SizeConstraintStatementTypeDef](./type_defs.md#sizeconstraintstatementtypedef) 
2. See [:material-code-braces: SizeConstraintStatementOutputTypeDef](./type_defs.md#sizeconstraintstatementoutputtypedef) 

## SqliMatchStatementUnionTypeDef

```python
# SqliMatchStatementUnionTypeDef definition

SqliMatchStatementUnionTypeDef = Union[
    SqliMatchStatementTypeDef,  # (1)
    SqliMatchStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SqliMatchStatementTypeDef](./type_defs.md#sqlimatchstatementtypedef) 
2. See [:material-code-braces: SqliMatchStatementOutputTypeDef](./type_defs.md#sqlimatchstatementoutputtypedef) 

## XssMatchStatementUnionTypeDef

```python
# XssMatchStatementUnionTypeDef definition

XssMatchStatementUnionTypeDef = Union[
    XssMatchStatementTypeDef,  # (1)
    XssMatchStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: XssMatchStatementTypeDef](./type_defs.md#xssmatchstatementtypedef) 
2. See [:material-code-braces: XssMatchStatementOutputTypeDef](./type_defs.md#xssmatchstatementoutputtypedef) 

## ManagedRuleGroupConfigUnionTypeDef

```python
# ManagedRuleGroupConfigUnionTypeDef definition

ManagedRuleGroupConfigUnionTypeDef = Union[
    ManagedRuleGroupConfigTypeDef,  # (1)
    ManagedRuleGroupConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ManagedRuleGroupConfigTypeDef](./type_defs.md#managedrulegroupconfigtypedef) 
2. See [:material-code-braces: ManagedRuleGroupConfigOutputTypeDef](./type_defs.md#managedrulegroupconfigoutputtypedef) 

## RuleActionOverrideUnionTypeDef

```python
# RuleActionOverrideUnionTypeDef definition

RuleActionOverrideUnionTypeDef = Union[
    RuleActionOverrideTypeDef,  # (1)
    RuleActionOverrideOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleActionOverrideTypeDef](./type_defs.md#ruleactionoverridetypedef) 
2. See [:material-code-braces: RuleActionOverrideOutputTypeDef](./type_defs.md#ruleactionoverrideoutputtypedef) 

## RuleGroupReferenceStatementUnionTypeDef

```python
# RuleGroupReferenceStatementUnionTypeDef definition

RuleGroupReferenceStatementUnionTypeDef = Union[
    RuleGroupReferenceStatementTypeDef,  # (1)
    RuleGroupReferenceStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleGroupReferenceStatementTypeDef](./type_defs.md#rulegroupreferencestatementtypedef) 
2. See [:material-code-braces: RuleGroupReferenceStatementOutputTypeDef](./type_defs.md#rulegroupreferencestatementoutputtypedef) 

## ManagedRuleGroupStatementUnionTypeDef

```python
# ManagedRuleGroupStatementUnionTypeDef definition

ManagedRuleGroupStatementUnionTypeDef = Union[
    ManagedRuleGroupStatementTypeDef,  # (1)
    ManagedRuleGroupStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ManagedRuleGroupStatementTypeDef](./type_defs.md#managedrulegroupstatementtypedef) 
2. See [:material-code-braces: ManagedRuleGroupStatementOutputTypeDef](./type_defs.md#managedrulegroupstatementoutputtypedef) 

## StatementUnionTypeDef

```python
# StatementUnionTypeDef definition

StatementUnionTypeDef = Union[
    StatementTypeDef,  # (1)
    StatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
2. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 

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
    EnableMachineLearning: NotRequired[bool],
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

## AndStatementOutputTypeDef

```python
# AndStatementOutputTypeDef definition

class AndStatementOutputTypeDef(TypedDict):
    Statements: List[Dict[str, Any]],
```

## AndStatementTypeDef

```python
# AndStatementTypeDef definition

class AndStatementTypeDef(TypedDict):
    Statements: Sequence[Mapping[str, Any]],
```

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
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## LabelNameConditionTypeDef

```python
# LabelNameConditionTypeDef definition

class LabelNameConditionTypeDef(TypedDict):
    LabelName: str,
```

## CookieMatchPatternOutputTypeDef

```python
# CookieMatchPatternOutputTypeDef definition

class CookieMatchPatternOutputTypeDef(TypedDict):
    All: NotRequired[Dict[str, Any]],
    IncludedCookies: NotRequired[List[str]],
    ExcludedCookies: NotRequired[List[str]],
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

## DeleteAPIKeyRequestRequestTypeDef

```python
# DeleteAPIKeyRequestRequestTypeDef definition

class DeleteAPIKeyRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
    APIKey: str,
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
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
    LogType: NotRequired[LogTypeType],  # (1)
    LogScope: NotRequired[LogScopeType],  # (2)
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-brackets: LogScopeType](./literals.md#logscopetype) 
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
## JA3FingerprintTypeDef

```python
# JA3FingerprintTypeDef definition

class JA3FingerprintTypeDef(TypedDict):
    FallbackBehavior: FallbackBehaviorType,  # (1)
```

1. See [:material-code-brackets: FallbackBehaviorType](./literals.md#fallbackbehaviortype) 
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
    LogType: NotRequired[LogTypeType],  # (1)
    LogScope: NotRequired[LogScopeType],  # (2)
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-brackets: LogScopeType](./literals.md#logscopetype) 
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
## TimeWindowOutputTypeDef

```python
# TimeWindowOutputTypeDef definition

class TimeWindowOutputTypeDef(TypedDict):
    StartTime: datetime,
    EndTime: datetime,
```

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

## HeaderMatchPatternOutputTypeDef

```python
# HeaderMatchPatternOutputTypeDef definition

class HeaderMatchPatternOutputTypeDef(TypedDict):
    All: NotRequired[Dict[str, Any]],
    IncludedHeaders: NotRequired[List[str]],
    ExcludedHeaders: NotRequired[List[str]],
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
## JsonMatchPatternOutputTypeDef

```python
# JsonMatchPatternOutputTypeDef definition

class JsonMatchPatternOutputTypeDef(TypedDict):
    All: NotRequired[Dict[str, Any]],
    IncludedPaths: NotRequired[List[str]],
```

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
    LogScope: NotRequired[LogScopeType],  # (2)
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-brackets: LogScopeType](./literals.md#logscopetype) 
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

## NotStatementOutputTypeDef

```python
# NotStatementOutputTypeDef definition

class NotStatementOutputTypeDef(TypedDict):
    Statement: Dict[str, Any],
```

## NotStatementTypeDef

```python
# NotStatementTypeDef definition

class NotStatementTypeDef(TypedDict):
    Statement: Mapping[str, Any],
```

## OrStatementOutputTypeDef

```python
# OrStatementOutputTypeDef definition

class OrStatementOutputTypeDef(TypedDict):
    Statements: List[Dict[str, Any]],
```

## OrStatementTypeDef

```python
# OrStatementTypeDef definition

class OrStatementTypeDef(TypedDict):
    Statements: Sequence[Mapping[str, Any]],
```

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

## ResponseInspectionBodyContainsOutputTypeDef

```python
# ResponseInspectionBodyContainsOutputTypeDef definition

class ResponseInspectionBodyContainsOutputTypeDef(TypedDict):
    SuccessStrings: List[str],
    FailureStrings: List[str],
```

## ResponseInspectionBodyContainsTypeDef

```python
# ResponseInspectionBodyContainsTypeDef definition

class ResponseInspectionBodyContainsTypeDef(TypedDict):
    SuccessStrings: Sequence[str],
    FailureStrings: Sequence[str],
```

## ResponseInspectionHeaderOutputTypeDef

```python
# ResponseInspectionHeaderOutputTypeDef definition

class ResponseInspectionHeaderOutputTypeDef(TypedDict):
    Name: str,
    SuccessValues: List[str],
    FailureValues: List[str],
```

## ResponseInspectionHeaderTypeDef

```python
# ResponseInspectionHeaderTypeDef definition

class ResponseInspectionHeaderTypeDef(TypedDict):
    Name: str,
    SuccessValues: Sequence[str],
    FailureValues: Sequence[str],
```

## ResponseInspectionJsonOutputTypeDef

```python
# ResponseInspectionJsonOutputTypeDef definition

class ResponseInspectionJsonOutputTypeDef(TypedDict):
    Identifier: str,
    SuccessValues: List[str],
    FailureValues: List[str],
```

## ResponseInspectionJsonTypeDef

```python
# ResponseInspectionJsonTypeDef definition

class ResponseInspectionJsonTypeDef(TypedDict):
    Identifier: str,
    SuccessValues: Sequence[str],
    FailureValues: Sequence[str],
```

## ResponseInspectionStatusCodeOutputTypeDef

```python
# ResponseInspectionStatusCodeOutputTypeDef definition

class ResponseInspectionStatusCodeOutputTypeDef(TypedDict):
    SuccessCodes: List[int],
    FailureCodes: List[int],
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
## AssociationConfigOutputTypeDef

```python
# AssociationConfigOutputTypeDef definition

class AssociationConfigOutputTypeDef(TypedDict):
    RequestBody: NotRequired[Dict[AssociatedResourceTypeType, RequestBodyAssociatedResourceTypeConfigTypeDef]],  # (1)
```

1. See [:material-code-brackets: AssociatedResourceTypeType](./literals.md#associatedresourcetypetype) [:material-code-braces: RequestBodyAssociatedResourceTypeConfigTypeDef](./type_defs.md#requestbodyassociatedresourcetypeconfigtypedef) 
## AssociationConfigTypeDef

```python
# AssociationConfigTypeDef definition

class AssociationConfigTypeDef(TypedDict):
    RequestBody: NotRequired[Mapping[AssociatedResourceTypeType, RequestBodyAssociatedResourceTypeConfigTypeDef]],  # (1)
```

1. See [:material-code-brackets: AssociatedResourceTypeType](./literals.md#associatedresourcetypetype) [:material-code-braces: RequestBodyAssociatedResourceTypeConfigTypeDef](./type_defs.md#requestbodyassociatedresourcetypeconfigtypedef) 
## RateLimitCookieOutputTypeDef

```python
# RateLimitCookieOutputTypeDef definition

class RateLimitCookieOutputTypeDef(TypedDict):
    Name: str,
    TextTransformations: List[TextTransformationTypeDef],  # (1)
```

1. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## RateLimitCookieTypeDef

```python
# RateLimitCookieTypeDef definition

class RateLimitCookieTypeDef(TypedDict):
    Name: str,
    TextTransformations: Sequence[TextTransformationTypeDef],  # (1)
```

1. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## RateLimitHeaderOutputTypeDef

```python
# RateLimitHeaderOutputTypeDef definition

class RateLimitHeaderOutputTypeDef(TypedDict):
    Name: str,
    TextTransformations: List[TextTransformationTypeDef],  # (1)
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
## RateLimitQueryArgumentOutputTypeDef

```python
# RateLimitQueryArgumentOutputTypeDef definition

class RateLimitQueryArgumentOutputTypeDef(TypedDict):
    Name: str,
    TextTransformations: List[TextTransformationTypeDef],  # (1)
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
## RateLimitQueryStringOutputTypeDef

```python
# RateLimitQueryStringOutputTypeDef definition

class RateLimitQueryStringOutputTypeDef(TypedDict):
    TextTransformations: List[TextTransformationTypeDef],  # (1)
```

1. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## RateLimitQueryStringTypeDef

```python
# RateLimitQueryStringTypeDef definition

class RateLimitQueryStringTypeDef(TypedDict):
    TextTransformations: Sequence[TextTransformationTypeDef],  # (1)
```

1. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## RateLimitUriPathOutputTypeDef

```python
# RateLimitUriPathOutputTypeDef definition

class RateLimitUriPathOutputTypeDef(TypedDict):
    TextTransformations: List[TextTransformationTypeDef],  # (1)
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
## CookiesOutputTypeDef

```python
# CookiesOutputTypeDef definition

class CookiesOutputTypeDef(TypedDict):
    MatchPattern: CookieMatchPatternOutputTypeDef,  # (1)
    MatchScope: MapMatchScopeType,  # (2)
    OversizeHandling: OversizeHandlingType,  # (3)
```

1. See [:material-code-braces: CookieMatchPatternOutputTypeDef](./type_defs.md#cookiematchpatternoutputtypedef) 
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
## CustomRequestHandlingOutputTypeDef

```python
# CustomRequestHandlingOutputTypeDef definition

class CustomRequestHandlingOutputTypeDef(TypedDict):
    InsertHeaders: List[CustomHTTPHeaderTypeDef],  # (1)
```

1. See [:material-code-braces: CustomHTTPHeaderTypeDef](./type_defs.md#customhttpheadertypedef) 
## CustomRequestHandlingTypeDef

```python
# CustomRequestHandlingTypeDef definition

class CustomRequestHandlingTypeDef(TypedDict):
    InsertHeaders: Sequence[CustomHTTPHeaderTypeDef],  # (1)
```

1. See [:material-code-braces: CustomHTTPHeaderTypeDef](./type_defs.md#customhttpheadertypedef) 
## CustomResponseOutputTypeDef

```python
# CustomResponseOutputTypeDef definition

class CustomResponseOutputTypeDef(TypedDict):
    ResponseCode: int,
    CustomResponseBodyKey: NotRequired[str],
    ResponseHeaders: NotRequired[List[CustomHTTPHeaderTypeDef]],  # (1)
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
## GeoMatchStatementOutputTypeDef

```python
# GeoMatchStatementOutputTypeDef definition

class GeoMatchStatementOutputTypeDef(TypedDict):
    CountryCodes: NotRequired[List[CountryCodeType]],  # (1)
    ForwardedIPConfig: NotRequired[ForwardedIPConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: CountryCodeType](./literals.md#countrycodetype) 
2. See [:material-code-braces: ForwardedIPConfigTypeDef](./type_defs.md#forwardedipconfigtypedef) 
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
## HeadersOutputTypeDef

```python
# HeadersOutputTypeDef definition

class HeadersOutputTypeDef(TypedDict):
    MatchPattern: HeaderMatchPatternOutputTypeDef,  # (1)
    MatchScope: MapMatchScopeType,  # (2)
    OversizeHandling: OversizeHandlingType,  # (3)
```

1. See [:material-code-braces: HeaderMatchPatternOutputTypeDef](./type_defs.md#headermatchpatternoutputtypedef) 
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
## JsonBodyOutputTypeDef

```python
# JsonBodyOutputTypeDef definition

class JsonBodyOutputTypeDef(TypedDict):
    MatchPattern: JsonMatchPatternOutputTypeDef,  # (1)
    MatchScope: JsonMatchScopeType,  # (2)
    InvalidFallbackBehavior: NotRequired[BodyParsingFallbackBehaviorType],  # (3)
    OversizeHandling: NotRequired[OversizeHandlingType],  # (4)
```

1. See [:material-code-braces: JsonMatchPatternOutputTypeDef](./type_defs.md#jsonmatchpatternoutputtypedef) 
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
## RequestInspectionACFPOutputTypeDef

```python
# RequestInspectionACFPOutputTypeDef definition

class RequestInspectionACFPOutputTypeDef(TypedDict):
    PayloadType: PayloadTypeType,  # (1)
    UsernameField: NotRequired[UsernameFieldTypeDef],  # (2)
    PasswordField: NotRequired[PasswordFieldTypeDef],  # (3)
    EmailField: NotRequired[EmailFieldTypeDef],  # (4)
    PhoneNumberFields: NotRequired[List[PhoneNumberFieldTypeDef]],  # (5)
    AddressFields: NotRequired[List[AddressFieldTypeDef]],  # (6)
```

1. See [:material-code-brackets: PayloadTypeType](./literals.md#payloadtypetype) 
2. See [:material-code-braces: UsernameFieldTypeDef](./type_defs.md#usernamefieldtypedef) 
3. See [:material-code-braces: PasswordFieldTypeDef](./type_defs.md#passwordfieldtypedef) 
4. See [:material-code-braces: EmailFieldTypeDef](./type_defs.md#emailfieldtypedef) 
5. See [:material-code-braces: PhoneNumberFieldTypeDef](./type_defs.md#phonenumberfieldtypedef) 
6. See [:material-code-braces: AddressFieldTypeDef](./type_defs.md#addressfieldtypedef) 
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
## ResponseInspectionOutputTypeDef

```python
# ResponseInspectionOutputTypeDef definition

class ResponseInspectionOutputTypeDef(TypedDict):
    StatusCode: NotRequired[ResponseInspectionStatusCodeOutputTypeDef],  # (1)
    Header: NotRequired[ResponseInspectionHeaderOutputTypeDef],  # (2)
    BodyContains: NotRequired[ResponseInspectionBodyContainsOutputTypeDef],  # (3)
    Json: NotRequired[ResponseInspectionJsonOutputTypeDef],  # (4)
```

1. See [:material-code-braces: ResponseInspectionStatusCodeOutputTypeDef](./type_defs.md#responseinspectionstatuscodeoutputtypedef) 
2. See [:material-code-braces: ResponseInspectionHeaderOutputTypeDef](./type_defs.md#responseinspectionheaderoutputtypedef) 
3. See [:material-code-braces: ResponseInspectionBodyContainsOutputTypeDef](./type_defs.md#responseinspectionbodycontainsoutputtypedef) 
4. See [:material-code-braces: ResponseInspectionJsonOutputTypeDef](./type_defs.md#responseinspectionjsonoutputtypedef) 
## TimeWindowTypeDef

```python
# TimeWindowTypeDef definition

class TimeWindowTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
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
    ExpiryTimestamp: TimestampTypeDef,
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## RateBasedStatementCustomKeyOutputTypeDef

```python
# RateBasedStatementCustomKeyOutputTypeDef definition

class RateBasedStatementCustomKeyOutputTypeDef(TypedDict):
    Header: NotRequired[RateLimitHeaderOutputTypeDef],  # (1)
    Cookie: NotRequired[RateLimitCookieOutputTypeDef],  # (2)
    QueryArgument: NotRequired[RateLimitQueryArgumentOutputTypeDef],  # (3)
    QueryString: NotRequired[RateLimitQueryStringOutputTypeDef],  # (4)
    HTTPMethod: NotRequired[Dict[str, Any]],
    ForwardedIP: NotRequired[Dict[str, Any]],
    IP: NotRequired[Dict[str, Any]],
    LabelNamespace: NotRequired[RateLimitLabelNamespaceTypeDef],  # (5)
    UriPath: NotRequired[RateLimitUriPathOutputTypeDef],  # (6)
```

1. See [:material-code-braces: RateLimitHeaderOutputTypeDef](./type_defs.md#ratelimitheaderoutputtypedef) 
2. See [:material-code-braces: RateLimitCookieOutputTypeDef](./type_defs.md#ratelimitcookieoutputtypedef) 
3. See [:material-code-braces: RateLimitQueryArgumentOutputTypeDef](./type_defs.md#ratelimitqueryargumentoutputtypedef) 
4. See [:material-code-braces: RateLimitQueryStringOutputTypeDef](./type_defs.md#ratelimitquerystringoutputtypedef) 
5. See [:material-code-braces: RateLimitLabelNamespaceTypeDef](./type_defs.md#ratelimitlabelnamespacetypedef) 
6. See [:material-code-braces: RateLimitUriPathOutputTypeDef](./type_defs.md#ratelimituripathoutputtypedef) 
## FilterOutputTypeDef

```python
# FilterOutputTypeDef definition

class FilterOutputTypeDef(TypedDict):
    Behavior: FilterBehaviorType,  # (1)
    Requirement: FilterRequirementType,  # (2)
    Conditions: List[ConditionTypeDef],  # (3)
```

1. See [:material-code-brackets: FilterBehaviorType](./literals.md#filterbehaviortype) 
2. See [:material-code-brackets: FilterRequirementType](./literals.md#filterrequirementtype) 
3. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Behavior: FilterBehaviorType,  # (1)
    Requirement: FilterRequirementType,  # (2)
    Conditions: Sequence[ConditionTypeDef],  # (3)
```

1. See [:material-code-brackets: FilterBehaviorType](./literals.md#filterbehaviortype) 
2. See [:material-code-brackets: FilterRequirementType](./literals.md#filterrequirementtype) 
3. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
## CookiesTypeDef

```python
# CookiesTypeDef definition

class CookiesTypeDef(TypedDict):
    MatchPattern: CookieMatchPatternUnionTypeDef,  # (1)
    MatchScope: MapMatchScopeType,  # (2)
    OversizeHandling: OversizeHandlingType,  # (3)
```

1. See [:material-code-braces: CookieMatchPatternTypeDef](./type_defs.md#cookiematchpatterntypedef) [:material-code-braces: CookieMatchPatternOutputTypeDef](./type_defs.md#cookiematchpatternoutputtypedef) 
2. See [:material-code-brackets: MapMatchScopeType](./literals.md#mapmatchscopetype) 
3. See [:material-code-brackets: OversizeHandlingType](./literals.md#oversizehandlingtype) 
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
## AllowActionOutputTypeDef

```python
# AllowActionOutputTypeDef definition

class AllowActionOutputTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[CustomRequestHandlingOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CustomRequestHandlingOutputTypeDef](./type_defs.md#customrequesthandlingoutputtypedef) 
## CaptchaActionOutputTypeDef

```python
# CaptchaActionOutputTypeDef definition

class CaptchaActionOutputTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[CustomRequestHandlingOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CustomRequestHandlingOutputTypeDef](./type_defs.md#customrequesthandlingoutputtypedef) 
## ChallengeActionOutputTypeDef

```python
# ChallengeActionOutputTypeDef definition

class ChallengeActionOutputTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[CustomRequestHandlingOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CustomRequestHandlingOutputTypeDef](./type_defs.md#customrequesthandlingoutputtypedef) 
## CountActionOutputTypeDef

```python
# CountActionOutputTypeDef definition

class CountActionOutputTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[CustomRequestHandlingOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CustomRequestHandlingOutputTypeDef](./type_defs.md#customrequesthandlingoutputtypedef) 
## BlockActionOutputTypeDef

```python
# BlockActionOutputTypeDef definition

class BlockActionOutputTypeDef(TypedDict):
    CustomResponse: NotRequired[CustomResponseOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CustomResponseOutputTypeDef](./type_defs.md#customresponseoutputtypedef) 
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
## HeadersTypeDef

```python
# HeadersTypeDef definition

class HeadersTypeDef(TypedDict):
    MatchPattern: HeaderMatchPatternUnionTypeDef,  # (1)
    MatchScope: MapMatchScopeType,  # (2)
    OversizeHandling: OversizeHandlingType,  # (3)
```

1. See [:material-code-braces: HeaderMatchPatternTypeDef](./type_defs.md#headermatchpatterntypedef) [:material-code-braces: HeaderMatchPatternOutputTypeDef](./type_defs.md#headermatchpatternoutputtypedef) 
2. See [:material-code-brackets: MapMatchScopeType](./literals.md#mapmatchscopetype) 
3. See [:material-code-brackets: OversizeHandlingType](./literals.md#oversizehandlingtype) 
## FieldToMatchOutputTypeDef

```python
# FieldToMatchOutputTypeDef definition

class FieldToMatchOutputTypeDef(TypedDict):
    SingleHeader: NotRequired[SingleHeaderTypeDef],  # (1)
    SingleQueryArgument: NotRequired[SingleQueryArgumentTypeDef],  # (2)
    AllQueryArguments: NotRequired[Dict[str, Any]],
    UriPath: NotRequired[Dict[str, Any]],
    QueryString: NotRequired[Dict[str, Any]],
    Body: NotRequired[BodyTypeDef],  # (3)
    Method: NotRequired[Dict[str, Any]],
    JsonBody: NotRequired[JsonBodyOutputTypeDef],  # (4)
    Headers: NotRequired[HeadersOutputTypeDef],  # (5)
    Cookies: NotRequired[CookiesOutputTypeDef],  # (6)
    HeaderOrder: NotRequired[HeaderOrderTypeDef],  # (7)
    JA3Fingerprint: NotRequired[JA3FingerprintTypeDef],  # (8)
```

1. See [:material-code-braces: SingleHeaderTypeDef](./type_defs.md#singleheadertypedef) 
2. See [:material-code-braces: SingleQueryArgumentTypeDef](./type_defs.md#singlequeryargumenttypedef) 
3. See [:material-code-braces: BodyTypeDef](./type_defs.md#bodytypedef) 
4. See [:material-code-braces: JsonBodyOutputTypeDef](./type_defs.md#jsonbodyoutputtypedef) 
5. See [:material-code-braces: HeadersOutputTypeDef](./type_defs.md#headersoutputtypedef) 
6. See [:material-code-braces: CookiesOutputTypeDef](./type_defs.md#cookiesoutputtypedef) 
7. See [:material-code-braces: HeaderOrderTypeDef](./type_defs.md#headerordertypedef) 
8. See [:material-code-braces: JA3FingerprintTypeDef](./type_defs.md#ja3fingerprinttypedef) 
## JsonBodyTypeDef

```python
# JsonBodyTypeDef definition

class JsonBodyTypeDef(TypedDict):
    MatchPattern: JsonMatchPatternUnionTypeDef,  # (1)
    MatchScope: JsonMatchScopeType,  # (2)
    InvalidFallbackBehavior: NotRequired[BodyParsingFallbackBehaviorType],  # (3)
    OversizeHandling: NotRequired[OversizeHandlingType],  # (4)
```

1. See [:material-code-braces: JsonMatchPatternTypeDef](./type_defs.md#jsonmatchpatterntypedef) [:material-code-braces: JsonMatchPatternOutputTypeDef](./type_defs.md#jsonmatchpatternoutputtypedef) 
2. See [:material-code-brackets: JsonMatchScopeType](./literals.md#jsonmatchscopetype) 
3. See [:material-code-brackets: BodyParsingFallbackBehaviorType](./literals.md#bodyparsingfallbackbehaviortype) 
4. See [:material-code-brackets: OversizeHandlingType](./literals.md#oversizehandlingtype) 
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
## AWSManagedRulesACFPRuleSetOutputTypeDef

```python
# AWSManagedRulesACFPRuleSetOutputTypeDef definition

class AWSManagedRulesACFPRuleSetOutputTypeDef(TypedDict):
    CreationPath: str,
    RegistrationPagePath: str,
    RequestInspection: RequestInspectionACFPOutputTypeDef,  # (1)
    ResponseInspection: NotRequired[ResponseInspectionOutputTypeDef],  # (2)
    EnableRegexInPath: NotRequired[bool],
```

1. See [:material-code-braces: RequestInspectionACFPOutputTypeDef](./type_defs.md#requestinspectionacfpoutputtypedef) 
2. See [:material-code-braces: ResponseInspectionOutputTypeDef](./type_defs.md#responseinspectionoutputtypedef) 
## AWSManagedRulesATPRuleSetOutputTypeDef

```python
# AWSManagedRulesATPRuleSetOutputTypeDef definition

class AWSManagedRulesATPRuleSetOutputTypeDef(TypedDict):
    LoginPath: str,
    RequestInspection: NotRequired[RequestInspectionTypeDef],  # (1)
    ResponseInspection: NotRequired[ResponseInspectionOutputTypeDef],  # (2)
    EnableRegexInPath: NotRequired[bool],
```

1. See [:material-code-braces: RequestInspectionTypeDef](./type_defs.md#requestinspectiontypedef) 
2. See [:material-code-braces: ResponseInspectionOutputTypeDef](./type_defs.md#responseinspectionoutputtypedef) 
## ResponseInspectionTypeDef

```python
# ResponseInspectionTypeDef definition

class ResponseInspectionTypeDef(TypedDict):
    StatusCode: NotRequired[ResponseInspectionStatusCodeUnionTypeDef],  # (1)
    Header: NotRequired[ResponseInspectionHeaderUnionTypeDef],  # (2)
    BodyContains: NotRequired[ResponseInspectionBodyContainsUnionTypeDef],  # (3)
    Json: NotRequired[ResponseInspectionJsonUnionTypeDef],  # (4)
```

1. See [:material-code-braces: ResponseInspectionStatusCodeTypeDef](./type_defs.md#responseinspectionstatuscodetypedef) [:material-code-braces: ResponseInspectionStatusCodeOutputTypeDef](./type_defs.md#responseinspectionstatuscodeoutputtypedef) 
2. See [:material-code-braces: ResponseInspectionHeaderTypeDef](./type_defs.md#responseinspectionheadertypedef) [:material-code-braces: ResponseInspectionHeaderOutputTypeDef](./type_defs.md#responseinspectionheaderoutputtypedef) 
3. See [:material-code-braces: ResponseInspectionBodyContainsTypeDef](./type_defs.md#responseinspectionbodycontainstypedef) [:material-code-braces: ResponseInspectionBodyContainsOutputTypeDef](./type_defs.md#responseinspectionbodycontainsoutputtypedef) 
4. See [:material-code-braces: ResponseInspectionJsonTypeDef](./type_defs.md#responseinspectionjsontypedef) [:material-code-braces: ResponseInspectionJsonOutputTypeDef](./type_defs.md#responseinspectionjsonoutputtypedef) 
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
## RateBasedStatementOutputTypeDef

```python
# RateBasedStatementOutputTypeDef definition

class RateBasedStatementOutputTypeDef(TypedDict):
    Limit: int,
    AggregateKeyType: RateBasedStatementAggregateKeyTypeType,  # (1)
    EvaluationWindowSec: NotRequired[int],
    ScopeDownStatement: NotRequired[Dict[str, Any]],
    ForwardedIPConfig: NotRequired[ForwardedIPConfigTypeDef],  # (2)
    CustomKeys: NotRequired[List[RateBasedStatementCustomKeyOutputTypeDef]],  # (3)
```

1. See [:material-code-brackets: RateBasedStatementAggregateKeyTypeType](./literals.md#ratebasedstatementaggregatekeytypetype) 
2. See [:material-code-braces: ForwardedIPConfigTypeDef](./type_defs.md#forwardedipconfigtypedef) 
3. See [:material-code-braces: RateBasedStatementCustomKeyOutputTypeDef](./type_defs.md#ratebasedstatementcustomkeyoutputtypedef) 
## RateBasedStatementCustomKeyTypeDef

```python
# RateBasedStatementCustomKeyTypeDef definition

class RateBasedStatementCustomKeyTypeDef(TypedDict):
    Header: NotRequired[RateLimitHeaderUnionTypeDef],  # (1)
    Cookie: NotRequired[RateLimitCookieUnionTypeDef],  # (2)
    QueryArgument: NotRequired[RateLimitQueryArgumentUnionTypeDef],  # (3)
    QueryString: NotRequired[RateLimitQueryStringUnionTypeDef],  # (4)
    HTTPMethod: NotRequired[Mapping[str, Any]],
    ForwardedIP: NotRequired[Mapping[str, Any]],
    IP: NotRequired[Mapping[str, Any]],
    LabelNamespace: NotRequired[RateLimitLabelNamespaceTypeDef],  # (5)
    UriPath: NotRequired[RateLimitUriPathUnionTypeDef],  # (6)
```

1. See [:material-code-braces: RateLimitHeaderTypeDef](./type_defs.md#ratelimitheadertypedef) [:material-code-braces: RateLimitHeaderOutputTypeDef](./type_defs.md#ratelimitheaderoutputtypedef) 
2. See [:material-code-braces: RateLimitCookieTypeDef](./type_defs.md#ratelimitcookietypedef) [:material-code-braces: RateLimitCookieOutputTypeDef](./type_defs.md#ratelimitcookieoutputtypedef) 
3. See [:material-code-braces: RateLimitQueryArgumentTypeDef](./type_defs.md#ratelimitqueryargumenttypedef) [:material-code-braces: RateLimitQueryArgumentOutputTypeDef](./type_defs.md#ratelimitqueryargumentoutputtypedef) 
4. See [:material-code-braces: RateLimitQueryStringTypeDef](./type_defs.md#ratelimitquerystringtypedef) [:material-code-braces: RateLimitQueryStringOutputTypeDef](./type_defs.md#ratelimitquerystringoutputtypedef) 
5. See [:material-code-braces: RateLimitLabelNamespaceTypeDef](./type_defs.md#ratelimitlabelnamespacetypedef) 
6. See [:material-code-braces: RateLimitUriPathTypeDef](./type_defs.md#ratelimituripathtypedef) [:material-code-braces: RateLimitUriPathOutputTypeDef](./type_defs.md#ratelimituripathoutputtypedef) 
## LoggingFilterOutputTypeDef

```python
# LoggingFilterOutputTypeDef definition

class LoggingFilterOutputTypeDef(TypedDict):
    Filters: List[FilterOutputTypeDef],  # (1)
    DefaultBehavior: FilterBehaviorType,  # (2)
```

1. See [:material-code-braces: FilterOutputTypeDef](./type_defs.md#filteroutputtypedef) 
2. See [:material-code-brackets: FilterBehaviorType](./literals.md#filterbehaviortype) 
## OverrideActionOutputTypeDef

```python
# OverrideActionOutputTypeDef definition

class OverrideActionOutputTypeDef(TypedDict):
    Count: NotRequired[CountActionOutputTypeDef],  # (1)
    None: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: CountActionOutputTypeDef](./type_defs.md#countactionoutputtypedef) 
## AllowActionTypeDef

```python
# AllowActionTypeDef definition

class AllowActionTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[CustomRequestHandlingUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CustomRequestHandlingTypeDef](./type_defs.md#customrequesthandlingtypedef) [:material-code-braces: CustomRequestHandlingOutputTypeDef](./type_defs.md#customrequesthandlingoutputtypedef) 
## CaptchaActionTypeDef

```python
# CaptchaActionTypeDef definition

class CaptchaActionTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[CustomRequestHandlingUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CustomRequestHandlingTypeDef](./type_defs.md#customrequesthandlingtypedef) [:material-code-braces: CustomRequestHandlingOutputTypeDef](./type_defs.md#customrequesthandlingoutputtypedef) 
## ChallengeActionTypeDef

```python
# ChallengeActionTypeDef definition

class ChallengeActionTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[CustomRequestHandlingUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CustomRequestHandlingTypeDef](./type_defs.md#customrequesthandlingtypedef) [:material-code-braces: CustomRequestHandlingOutputTypeDef](./type_defs.md#customrequesthandlingoutputtypedef) 
## CountActionTypeDef

```python
# CountActionTypeDef definition

class CountActionTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[CustomRequestHandlingUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CustomRequestHandlingTypeDef](./type_defs.md#customrequesthandlingtypedef) [:material-code-braces: CustomRequestHandlingOutputTypeDef](./type_defs.md#customrequesthandlingoutputtypedef) 
## DefaultActionOutputTypeDef

```python
# DefaultActionOutputTypeDef definition

class DefaultActionOutputTypeDef(TypedDict):
    Block: NotRequired[BlockActionOutputTypeDef],  # (1)
    Allow: NotRequired[AllowActionOutputTypeDef],  # (2)
```

1. See [:material-code-braces: BlockActionOutputTypeDef](./type_defs.md#blockactionoutputtypedef) 
2. See [:material-code-braces: AllowActionOutputTypeDef](./type_defs.md#allowactionoutputtypedef) 
## RuleActionOutputTypeDef

```python
# RuleActionOutputTypeDef definition

class RuleActionOutputTypeDef(TypedDict):
    Block: NotRequired[BlockActionOutputTypeDef],  # (1)
    Allow: NotRequired[AllowActionOutputTypeDef],  # (2)
    Count: NotRequired[CountActionOutputTypeDef],  # (3)
    Captcha: NotRequired[CaptchaActionOutputTypeDef],  # (4)
    Challenge: NotRequired[ChallengeActionOutputTypeDef],  # (5)
```

1. See [:material-code-braces: BlockActionOutputTypeDef](./type_defs.md#blockactionoutputtypedef) 
2. See [:material-code-braces: AllowActionOutputTypeDef](./type_defs.md#allowactionoutputtypedef) 
3. See [:material-code-braces: CountActionOutputTypeDef](./type_defs.md#countactionoutputtypedef) 
4. See [:material-code-braces: CaptchaActionOutputTypeDef](./type_defs.md#captchaactionoutputtypedef) 
5. See [:material-code-braces: ChallengeActionOutputTypeDef](./type_defs.md#challengeactionoutputtypedef) 
## BlockActionTypeDef

```python
# BlockActionTypeDef definition

class BlockActionTypeDef(TypedDict):
    CustomResponse: NotRequired[CustomResponseUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CustomResponseTypeDef](./type_defs.md#customresponsetypedef) [:material-code-braces: CustomResponseOutputTypeDef](./type_defs.md#customresponseoutputtypedef) 
## GetSampledRequestsResponseTypeDef

```python
# GetSampledRequestsResponseTypeDef definition

class GetSampledRequestsResponseTypeDef(TypedDict):
    SampledRequests: List[SampledHTTPRequestTypeDef],  # (1)
    PopulationSize: int,
    TimeWindow: TimeWindowOutputTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SampledHTTPRequestTypeDef](./type_defs.md#sampledhttprequesttypedef) 
2. See [:material-code-braces: TimeWindowOutputTypeDef](./type_defs.md#timewindowoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ByteMatchStatementOutputTypeDef

```python
# ByteMatchStatementOutputTypeDef definition

class ByteMatchStatementOutputTypeDef(TypedDict):
    SearchString: bytes,
    FieldToMatch: FieldToMatchOutputTypeDef,  # (1)
    TextTransformations: List[TextTransformationTypeDef],  # (2)
    PositionalConstraint: PositionalConstraintType,  # (3)
```

1. See [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
3. See [:material-code-brackets: PositionalConstraintType](./literals.md#positionalconstrainttype) 
## RegexMatchStatementOutputTypeDef

```python
# RegexMatchStatementOutputTypeDef definition

class RegexMatchStatementOutputTypeDef(TypedDict):
    RegexString: str,
    FieldToMatch: FieldToMatchOutputTypeDef,  # (1)
    TextTransformations: List[TextTransformationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## RegexPatternSetReferenceStatementOutputTypeDef

```python
# RegexPatternSetReferenceStatementOutputTypeDef definition

class RegexPatternSetReferenceStatementOutputTypeDef(TypedDict):
    ARN: str,
    FieldToMatch: FieldToMatchOutputTypeDef,  # (1)
    TextTransformations: List[TextTransformationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## SizeConstraintStatementOutputTypeDef

```python
# SizeConstraintStatementOutputTypeDef definition

class SizeConstraintStatementOutputTypeDef(TypedDict):
    FieldToMatch: FieldToMatchOutputTypeDef,  # (1)
    ComparisonOperator: ComparisonOperatorType,  # (2)
    Size: int,
    TextTransformations: List[TextTransformationTypeDef],  # (3)
```

1. See [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
2. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
3. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## SqliMatchStatementOutputTypeDef

```python
# SqliMatchStatementOutputTypeDef definition

class SqliMatchStatementOutputTypeDef(TypedDict):
    FieldToMatch: FieldToMatchOutputTypeDef,  # (1)
    TextTransformations: List[TextTransformationTypeDef],  # (2)
    SensitivityLevel: NotRequired[SensitivityLevelType],  # (3)
```

1. See [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
3. See [:material-code-brackets: SensitivityLevelType](./literals.md#sensitivityleveltype) 
## XssMatchStatementOutputTypeDef

```python
# XssMatchStatementOutputTypeDef definition

class XssMatchStatementOutputTypeDef(TypedDict):
    FieldToMatch: FieldToMatchOutputTypeDef,  # (1)
    TextTransformations: List[TextTransformationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## ManagedRuleGroupConfigOutputTypeDef

```python
# ManagedRuleGroupConfigOutputTypeDef definition

class ManagedRuleGroupConfigOutputTypeDef(TypedDict):
    LoginPath: NotRequired[str],
    PayloadType: NotRequired[PayloadTypeType],  # (1)
    UsernameField: NotRequired[UsernameFieldTypeDef],  # (2)
    PasswordField: NotRequired[PasswordFieldTypeDef],  # (3)
    AWSManagedRulesBotControlRuleSet: NotRequired[AWSManagedRulesBotControlRuleSetTypeDef],  # (4)
    AWSManagedRulesATPRuleSet: NotRequired[AWSManagedRulesATPRuleSetOutputTypeDef],  # (5)
    AWSManagedRulesACFPRuleSet: NotRequired[AWSManagedRulesACFPRuleSetOutputTypeDef],  # (6)
```

1. See [:material-code-brackets: PayloadTypeType](./literals.md#payloadtypetype) 
2. See [:material-code-braces: UsernameFieldTypeDef](./type_defs.md#usernamefieldtypedef) 
3. See [:material-code-braces: PasswordFieldTypeDef](./type_defs.md#passwordfieldtypedef) 
4. See [:material-code-braces: AWSManagedRulesBotControlRuleSetTypeDef](./type_defs.md#awsmanagedrulesbotcontrolrulesettypedef) 
5. See [:material-code-braces: AWSManagedRulesATPRuleSetOutputTypeDef](./type_defs.md#awsmanagedrulesatprulesetoutputtypedef) 
6. See [:material-code-braces: AWSManagedRulesACFPRuleSetOutputTypeDef](./type_defs.md#awsmanagedrulesacfprulesetoutputtypedef) 
## LoggingConfigurationOutputTypeDef

```python
# LoggingConfigurationOutputTypeDef definition

class LoggingConfigurationOutputTypeDef(TypedDict):
    ResourceArn: str,
    LogDestinationConfigs: List[str],
    RedactedFields: NotRequired[List[FieldToMatchOutputTypeDef]],  # (1)
    ManagedByFirewallManager: NotRequired[bool],
    LoggingFilter: NotRequired[LoggingFilterOutputTypeDef],  # (2)
    LogType: NotRequired[LogTypeType],  # (3)
    LogScope: NotRequired[LogScopeType],  # (4)
```

1. See [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
2. See [:material-code-braces: LoggingFilterOutputTypeDef](./type_defs.md#loggingfilteroutputtypedef) 
3. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
4. See [:material-code-brackets: LogScopeType](./literals.md#logscopetype) 
## LoggingFilterTypeDef

```python
# LoggingFilterTypeDef definition

class LoggingFilterTypeDef(TypedDict):
    Filters: Sequence[FilterUnionTypeDef],  # (1)
    DefaultBehavior: FilterBehaviorType,  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) [:material-code-braces: FilterOutputTypeDef](./type_defs.md#filteroutputtypedef) 
2. See [:material-code-brackets: FilterBehaviorType](./literals.md#filterbehaviortype) 
## RuleActionOverrideOutputTypeDef

```python
# RuleActionOverrideOutputTypeDef definition

class RuleActionOverrideOutputTypeDef(TypedDict):
    Name: str,
    ActionToUse: RuleActionOutputTypeDef,  # (1)
```

1. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
## RuleSummaryTypeDef

```python
# RuleSummaryTypeDef definition

class RuleSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    Action: NotRequired[RuleActionOutputTypeDef],  # (1)
```

1. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
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
    JsonBody: NotRequired[JsonBodyUnionTypeDef],  # (4)
    Headers: NotRequired[HeadersUnionTypeDef],  # (5)
    Cookies: NotRequired[CookiesUnionTypeDef],  # (6)
    HeaderOrder: NotRequired[HeaderOrderTypeDef],  # (7)
    JA3Fingerprint: NotRequired[JA3FingerprintTypeDef],  # (8)
```

1. See [:material-code-braces: SingleHeaderTypeDef](./type_defs.md#singleheadertypedef) 
2. See [:material-code-braces: SingleQueryArgumentTypeDef](./type_defs.md#singlequeryargumenttypedef) 
3. See [:material-code-braces: BodyTypeDef](./type_defs.md#bodytypedef) 
4. See [:material-code-braces: JsonBodyTypeDef](./type_defs.md#jsonbodytypedef) [:material-code-braces: JsonBodyOutputTypeDef](./type_defs.md#jsonbodyoutputtypedef) 
5. See [:material-code-braces: HeadersTypeDef](./type_defs.md#headerstypedef) [:material-code-braces: HeadersOutputTypeDef](./type_defs.md#headersoutputtypedef) 
6. See [:material-code-braces: CookiesTypeDef](./type_defs.md#cookiestypedef) [:material-code-braces: CookiesOutputTypeDef](./type_defs.md#cookiesoutputtypedef) 
7. See [:material-code-braces: HeaderOrderTypeDef](./type_defs.md#headerordertypedef) 
8. See [:material-code-braces: JA3FingerprintTypeDef](./type_defs.md#ja3fingerprinttypedef) 
## AWSManagedRulesACFPRuleSetTypeDef

```python
# AWSManagedRulesACFPRuleSetTypeDef definition

class AWSManagedRulesACFPRuleSetTypeDef(TypedDict):
    CreationPath: str,
    RegistrationPagePath: str,
    RequestInspection: RequestInspectionACFPUnionTypeDef,  # (1)
    ResponseInspection: NotRequired[ResponseInspectionUnionTypeDef],  # (2)
    EnableRegexInPath: NotRequired[bool],
```

1. See [:material-code-braces: RequestInspectionACFPTypeDef](./type_defs.md#requestinspectionacfptypedef) [:material-code-braces: RequestInspectionACFPOutputTypeDef](./type_defs.md#requestinspectionacfpoutputtypedef) 
2. See [:material-code-braces: ResponseInspectionTypeDef](./type_defs.md#responseinspectiontypedef) [:material-code-braces: ResponseInspectionOutputTypeDef](./type_defs.md#responseinspectionoutputtypedef) 
## AWSManagedRulesATPRuleSetTypeDef

```python
# AWSManagedRulesATPRuleSetTypeDef definition

class AWSManagedRulesATPRuleSetTypeDef(TypedDict):
    LoginPath: str,
    RequestInspection: NotRequired[RequestInspectionTypeDef],  # (1)
    ResponseInspection: NotRequired[ResponseInspectionUnionTypeDef],  # (2)
    EnableRegexInPath: NotRequired[bool],
```

1. See [:material-code-braces: RequestInspectionTypeDef](./type_defs.md#requestinspectiontypedef) 
2. See [:material-code-braces: ResponseInspectionTypeDef](./type_defs.md#responseinspectiontypedef) [:material-code-braces: ResponseInspectionOutputTypeDef](./type_defs.md#responseinspectionoutputtypedef) 
## RateBasedStatementTypeDef

```python
# RateBasedStatementTypeDef definition

class RateBasedStatementTypeDef(TypedDict):
    Limit: int,
    AggregateKeyType: RateBasedStatementAggregateKeyTypeType,  # (1)
    EvaluationWindowSec: NotRequired[int],
    ScopeDownStatement: NotRequired[Mapping[str, Any]],
    ForwardedIPConfig: NotRequired[ForwardedIPConfigTypeDef],  # (2)
    CustomKeys: NotRequired[Sequence[RateBasedStatementCustomKeyUnionTypeDef]],  # (3)
```

1. See [:material-code-brackets: RateBasedStatementAggregateKeyTypeType](./literals.md#ratebasedstatementaggregatekeytypetype) 
2. See [:material-code-braces: ForwardedIPConfigTypeDef](./type_defs.md#forwardedipconfigtypedef) 
3. See [:material-code-braces: RateBasedStatementCustomKeyTypeDef](./type_defs.md#ratebasedstatementcustomkeytypedef) [:material-code-braces: RateBasedStatementCustomKeyOutputTypeDef](./type_defs.md#ratebasedstatementcustomkeyoutputtypedef) 
## GetLoggingConfigurationResponseTypeDef

```python
# GetLoggingConfigurationResponseTypeDef definition

class GetLoggingConfigurationResponseTypeDef(TypedDict):
    LoggingConfiguration: LoggingConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationOutputTypeDef](./type_defs.md#loggingconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLoggingConfigurationsResponseTypeDef

```python
# ListLoggingConfigurationsResponseTypeDef definition

class ListLoggingConfigurationsResponseTypeDef(TypedDict):
    LoggingConfigurations: List[LoggingConfigurationOutputTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationOutputTypeDef](./type_defs.md#loggingconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutLoggingConfigurationResponseTypeDef

```python
# PutLoggingConfigurationResponseTypeDef definition

class PutLoggingConfigurationResponseTypeDef(TypedDict):
    LoggingConfiguration: LoggingConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationOutputTypeDef](./type_defs.md#loggingconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OverrideActionTypeDef

```python
# OverrideActionTypeDef definition

class OverrideActionTypeDef(TypedDict):
    Count: NotRequired[CountActionUnionTypeDef],  # (1)
    None: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: CountActionTypeDef](./type_defs.md#countactiontypedef) [:material-code-braces: CountActionOutputTypeDef](./type_defs.md#countactionoutputtypedef) 
## ManagedRuleGroupStatementOutputTypeDef

```python
# ManagedRuleGroupStatementOutputTypeDef definition

class ManagedRuleGroupStatementOutputTypeDef(TypedDict):
    VendorName: str,
    Name: str,
    Version: NotRequired[str],
    ExcludedRules: NotRequired[List[ExcludedRuleTypeDef]],  # (1)
    ScopeDownStatement: NotRequired[Dict[str, Any]],
    ManagedRuleGroupConfigs: NotRequired[List[ManagedRuleGroupConfigOutputTypeDef]],  # (2)
    RuleActionOverrides: NotRequired[List[RuleActionOverrideOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: ExcludedRuleTypeDef](./type_defs.md#excludedruletypedef) 
2. See [:material-code-braces: ManagedRuleGroupConfigOutputTypeDef](./type_defs.md#managedrulegroupconfigoutputtypedef) 
3. See [:material-code-braces: RuleActionOverrideOutputTypeDef](./type_defs.md#ruleactionoverrideoutputtypedef) 
## RuleGroupReferenceStatementOutputTypeDef

```python
# RuleGroupReferenceStatementOutputTypeDef definition

class RuleGroupReferenceStatementOutputTypeDef(TypedDict):
    ARN: str,
    ExcludedRules: NotRequired[List[ExcludedRuleTypeDef]],  # (1)
    RuleActionOverrides: NotRequired[List[RuleActionOverrideOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: ExcludedRuleTypeDef](./type_defs.md#excludedruletypedef) 
2. See [:material-code-braces: RuleActionOverrideOutputTypeDef](./type_defs.md#ruleactionoverrideoutputtypedef) 
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
## DefaultActionTypeDef

```python
# DefaultActionTypeDef definition

class DefaultActionTypeDef(TypedDict):
    Block: NotRequired[BlockActionUnionTypeDef],  # (1)
    Allow: NotRequired[AllowActionUnionTypeDef],  # (2)
```

1. See [:material-code-braces: BlockActionTypeDef](./type_defs.md#blockactiontypedef) [:material-code-braces: BlockActionOutputTypeDef](./type_defs.md#blockactionoutputtypedef) 
2. See [:material-code-braces: AllowActionTypeDef](./type_defs.md#allowactiontypedef) [:material-code-braces: AllowActionOutputTypeDef](./type_defs.md#allowactionoutputtypedef) 
## RuleActionTypeDef

```python
# RuleActionTypeDef definition

class RuleActionTypeDef(TypedDict):
    Block: NotRequired[BlockActionUnionTypeDef],  # (1)
    Allow: NotRequired[AllowActionUnionTypeDef],  # (2)
    Count: NotRequired[CountActionUnionTypeDef],  # (3)
    Captcha: NotRequired[CaptchaActionUnionTypeDef],  # (4)
    Challenge: NotRequired[ChallengeActionUnionTypeDef],  # (5)
```

1. See [:material-code-braces: BlockActionTypeDef](./type_defs.md#blockactiontypedef) [:material-code-braces: BlockActionOutputTypeDef](./type_defs.md#blockactionoutputtypedef) 
2. See [:material-code-braces: AllowActionTypeDef](./type_defs.md#allowactiontypedef) [:material-code-braces: AllowActionOutputTypeDef](./type_defs.md#allowactionoutputtypedef) 
3. See [:material-code-braces: CountActionTypeDef](./type_defs.md#countactiontypedef) [:material-code-braces: CountActionOutputTypeDef](./type_defs.md#countactionoutputtypedef) 
4. See [:material-code-braces: CaptchaActionTypeDef](./type_defs.md#captchaactiontypedef) [:material-code-braces: CaptchaActionOutputTypeDef](./type_defs.md#captchaactionoutputtypedef) 
5. See [:material-code-braces: ChallengeActionTypeDef](./type_defs.md#challengeactiontypedef) [:material-code-braces: ChallengeActionOutputTypeDef](./type_defs.md#challengeactionoutputtypedef) 
## FirewallManagerStatementTypeDef

```python
# FirewallManagerStatementTypeDef definition

class FirewallManagerStatementTypeDef(TypedDict):
    ManagedRuleGroupStatement: NotRequired[ManagedRuleGroupStatementOutputTypeDef],  # (1)
    RuleGroupReferenceStatement: NotRequired[RuleGroupReferenceStatementOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ManagedRuleGroupStatementOutputTypeDef](./type_defs.md#managedrulegroupstatementoutputtypedef) 
2. See [:material-code-braces: RuleGroupReferenceStatementOutputTypeDef](./type_defs.md#rulegroupreferencestatementoutputtypedef) 
## StatementOutputTypeDef

```python
# StatementOutputTypeDef definition

class StatementOutputTypeDef(TypedDict):
    ByteMatchStatement: NotRequired[ByteMatchStatementOutputTypeDef],  # (1)
    SqliMatchStatement: NotRequired[SqliMatchStatementOutputTypeDef],  # (2)
    XssMatchStatement: NotRequired[XssMatchStatementOutputTypeDef],  # (3)
    SizeConstraintStatement: NotRequired[SizeConstraintStatementOutputTypeDef],  # (4)
    GeoMatchStatement: NotRequired[GeoMatchStatementOutputTypeDef],  # (5)
    RuleGroupReferenceStatement: NotRequired[RuleGroupReferenceStatementOutputTypeDef],  # (6)
    IPSetReferenceStatement: NotRequired[IPSetReferenceStatementTypeDef],  # (7)
    RegexPatternSetReferenceStatement: NotRequired[RegexPatternSetReferenceStatementOutputTypeDef],  # (8)
    RateBasedStatement: NotRequired[RateBasedStatementOutputTypeDef],  # (9)
    AndStatement: NotRequired[AndStatementOutputTypeDef],  # (10)
    OrStatement: NotRequired[OrStatementOutputTypeDef],  # (11)
    NotStatement: NotRequired[NotStatementOutputTypeDef],  # (12)
    ManagedRuleGroupStatement: NotRequired[ManagedRuleGroupStatementOutputTypeDef],  # (13)
    LabelMatchStatement: NotRequired[LabelMatchStatementTypeDef],  # (14)
    RegexMatchStatement: NotRequired[RegexMatchStatementOutputTypeDef],  # (15)
```

1. See [:material-code-braces: ByteMatchStatementOutputTypeDef](./type_defs.md#bytematchstatementoutputtypedef) 
2. See [:material-code-braces: SqliMatchStatementOutputTypeDef](./type_defs.md#sqlimatchstatementoutputtypedef) 
3. See [:material-code-braces: XssMatchStatementOutputTypeDef](./type_defs.md#xssmatchstatementoutputtypedef) 
4. See [:material-code-braces: SizeConstraintStatementOutputTypeDef](./type_defs.md#sizeconstraintstatementoutputtypedef) 
5. See [:material-code-braces: GeoMatchStatementOutputTypeDef](./type_defs.md#geomatchstatementoutputtypedef) 
6. See [:material-code-braces: RuleGroupReferenceStatementOutputTypeDef](./type_defs.md#rulegroupreferencestatementoutputtypedef) 
7. See [:material-code-braces: IPSetReferenceStatementTypeDef](./type_defs.md#ipsetreferencestatementtypedef) 
8. See [:material-code-braces: RegexPatternSetReferenceStatementOutputTypeDef](./type_defs.md#regexpatternsetreferencestatementoutputtypedef) 
9. See [:material-code-braces: RateBasedStatementOutputTypeDef](./type_defs.md#ratebasedstatementoutputtypedef) 
10. See [:material-code-braces: AndStatementOutputTypeDef](./type_defs.md#andstatementoutputtypedef) 
11. See [:material-code-braces: OrStatementOutputTypeDef](./type_defs.md#orstatementoutputtypedef) 
12. See [:material-code-braces: NotStatementOutputTypeDef](./type_defs.md#notstatementoutputtypedef) 
13. See [:material-code-braces: ManagedRuleGroupStatementOutputTypeDef](./type_defs.md#managedrulegroupstatementoutputtypedef) 
14. See [:material-code-braces: LabelMatchStatementTypeDef](./type_defs.md#labelmatchstatementtypedef) 
15. See [:material-code-braces: RegexMatchStatementOutputTypeDef](./type_defs.md#regexmatchstatementoutputtypedef) 
## ByteMatchStatementTypeDef

```python
# ByteMatchStatementTypeDef definition

class ByteMatchStatementTypeDef(TypedDict):
    SearchString: BlobTypeDef,
    FieldToMatch: FieldToMatchUnionTypeDef,  # (1)
    TextTransformations: Sequence[TextTransformationTypeDef],  # (2)
    PositionalConstraint: PositionalConstraintType,  # (3)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
3. See [:material-code-brackets: PositionalConstraintType](./literals.md#positionalconstrainttype) 
## LoggingConfigurationTypeDef

```python
# LoggingConfigurationTypeDef definition

class LoggingConfigurationTypeDef(TypedDict):
    ResourceArn: str,
    LogDestinationConfigs: Sequence[str],
    RedactedFields: NotRequired[Sequence[FieldToMatchUnionTypeDef]],  # (1)
    ManagedByFirewallManager: NotRequired[bool],
    LoggingFilter: NotRequired[LoggingFilterUnionTypeDef],  # (2)
    LogType: NotRequired[LogTypeType],  # (3)
    LogScope: NotRequired[LogScopeType],  # (4)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
2. See [:material-code-braces: LoggingFilterTypeDef](./type_defs.md#loggingfiltertypedef) [:material-code-braces: LoggingFilterOutputTypeDef](./type_defs.md#loggingfilteroutputtypedef) 
3. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
4. See [:material-code-brackets: LogScopeType](./literals.md#logscopetype) 
## RegexMatchStatementTypeDef

```python
# RegexMatchStatementTypeDef definition

class RegexMatchStatementTypeDef(TypedDict):
    RegexString: str,
    FieldToMatch: FieldToMatchUnionTypeDef,  # (1)
    TextTransformations: Sequence[TextTransformationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## RegexPatternSetReferenceStatementTypeDef

```python
# RegexPatternSetReferenceStatementTypeDef definition

class RegexPatternSetReferenceStatementTypeDef(TypedDict):
    ARN: str,
    FieldToMatch: FieldToMatchUnionTypeDef,  # (1)
    TextTransformations: Sequence[TextTransformationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## SizeConstraintStatementTypeDef

```python
# SizeConstraintStatementTypeDef definition

class SizeConstraintStatementTypeDef(TypedDict):
    FieldToMatch: FieldToMatchUnionTypeDef,  # (1)
    ComparisonOperator: ComparisonOperatorType,  # (2)
    Size: int,
    TextTransformations: Sequence[TextTransformationTypeDef],  # (3)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
2. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
3. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
## SqliMatchStatementTypeDef

```python
# SqliMatchStatementTypeDef definition

class SqliMatchStatementTypeDef(TypedDict):
    FieldToMatch: FieldToMatchUnionTypeDef,  # (1)
    TextTransformations: Sequence[TextTransformationTypeDef],  # (2)
    SensitivityLevel: NotRequired[SensitivityLevelType],  # (3)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
2. See [:material-code-braces: TextTransformationTypeDef](./type_defs.md#texttransformationtypedef) 
3. See [:material-code-brackets: SensitivityLevelType](./literals.md#sensitivityleveltype) 
## XssMatchStatementTypeDef

```python
# XssMatchStatementTypeDef definition

class XssMatchStatementTypeDef(TypedDict):
    FieldToMatch: FieldToMatchUnionTypeDef,  # (1)
    TextTransformations: Sequence[TextTransformationTypeDef],  # (2)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) [:material-code-braces: FieldToMatchOutputTypeDef](./type_defs.md#fieldtomatchoutputtypedef) 
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
    AWSManagedRulesATPRuleSet: NotRequired[AWSManagedRulesATPRuleSetUnionTypeDef],  # (5)
    AWSManagedRulesACFPRuleSet: NotRequired[AWSManagedRulesACFPRuleSetUnionTypeDef],  # (6)
```

1. See [:material-code-brackets: PayloadTypeType](./literals.md#payloadtypetype) 
2. See [:material-code-braces: UsernameFieldTypeDef](./type_defs.md#usernamefieldtypedef) 
3. See [:material-code-braces: PasswordFieldTypeDef](./type_defs.md#passwordfieldtypedef) 
4. See [:material-code-braces: AWSManagedRulesBotControlRuleSetTypeDef](./type_defs.md#awsmanagedrulesbotcontrolrulesettypedef) 
5. See [:material-code-braces: AWSManagedRulesATPRuleSetTypeDef](./type_defs.md#awsmanagedrulesatprulesettypedef) [:material-code-braces: AWSManagedRulesATPRuleSetOutputTypeDef](./type_defs.md#awsmanagedrulesatprulesetoutputtypedef) 
6. See [:material-code-braces: AWSManagedRulesACFPRuleSetTypeDef](./type_defs.md#awsmanagedrulesacfprulesettypedef) [:material-code-braces: AWSManagedRulesACFPRuleSetOutputTypeDef](./type_defs.md#awsmanagedrulesacfprulesetoutputtypedef) 
## FirewallManagerRuleGroupTypeDef

```python
# FirewallManagerRuleGroupTypeDef definition

class FirewallManagerRuleGroupTypeDef(TypedDict):
    Name: str,
    Priority: int,
    FirewallManagerStatement: FirewallManagerStatementTypeDef,  # (1)
    OverrideAction: OverrideActionOutputTypeDef,  # (2)
    VisibilityConfig: VisibilityConfigTypeDef,  # (3)
```

1. See [:material-code-braces: FirewallManagerStatementTypeDef](./type_defs.md#firewallmanagerstatementtypedef) 
2. See [:material-code-braces: OverrideActionOutputTypeDef](./type_defs.md#overrideactionoutputtypedef) 
3. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
## RuleOutputTypeDef

```python
# RuleOutputTypeDef definition

class RuleOutputTypeDef(TypedDict):
    Name: str,
    Priority: int,
    Statement: StatementOutputTypeDef,  # (1)
    VisibilityConfig: VisibilityConfigTypeDef,  # (5)
    Action: NotRequired[RuleActionOutputTypeDef],  # (2)
    OverrideAction: NotRequired[OverrideActionOutputTypeDef],  # (3)
    RuleLabels: NotRequired[List[LabelTypeDef]],  # (4)
    CaptchaConfig: NotRequired[CaptchaConfigTypeDef],  # (6)
    ChallengeConfig: NotRequired[ChallengeConfigTypeDef],  # (7)
```

1. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
2. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
3. See [:material-code-braces: OverrideActionOutputTypeDef](./type_defs.md#overrideactionoutputtypedef) 
4. See [:material-code-braces: LabelTypeDef](./type_defs.md#labeltypedef) 
5. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
6. See [:material-code-braces: CaptchaConfigTypeDef](./type_defs.md#captchaconfigtypedef) 
7. See [:material-code-braces: ChallengeConfigTypeDef](./type_defs.md#challengeconfigtypedef) 
## RuleActionOverrideTypeDef

```python
# RuleActionOverrideTypeDef definition

class RuleActionOverrideTypeDef(TypedDict):
    Name: str,
    ActionToUse: RuleActionUnionTypeDef,  # (1)
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
## PutLoggingConfigurationRequestRequestTypeDef

```python
# PutLoggingConfigurationRequestRequestTypeDef definition

class PutLoggingConfigurationRequestRequestTypeDef(TypedDict):
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
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
    Rules: NotRequired[List[RuleOutputTypeDef]],  # (1)
    LabelNamespace: NotRequired[str],
    CustomResponseBodies: NotRequired[Dict[str, CustomResponseBodyTypeDef]],  # (3)
    AvailableLabels: NotRequired[List[LabelSummaryTypeDef]],  # (4)
    ConsumedLabels: NotRequired[List[LabelSummaryTypeDef]],  # (4)
```

1. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
2. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
3. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
4. See [:material-code-braces: LabelSummaryTypeDef](./type_defs.md#labelsummarytypedef) 
5. See [:material-code-braces: LabelSummaryTypeDef](./type_defs.md#labelsummarytypedef) 
## WebACLTypeDef

```python
# WebACLTypeDef definition

class WebACLTypeDef(TypedDict):
    Name: str,
    Id: str,
    ARN: str,
    DefaultAction: DefaultActionOutputTypeDef,  # (1)
    VisibilityConfig: VisibilityConfigTypeDef,  # (3)
    Description: NotRequired[str],
    Rules: NotRequired[List[RuleOutputTypeDef]],  # (2)
    Capacity: NotRequired[int],
    PreProcessFirewallManagerRuleGroups: NotRequired[List[FirewallManagerRuleGroupTypeDef]],  # (4)
    PostProcessFirewallManagerRuleGroups: NotRequired[List[FirewallManagerRuleGroupTypeDef]],  # (4)
    ManagedByFirewallManager: NotRequired[bool],
    LabelNamespace: NotRequired[str],
    CustomResponseBodies: NotRequired[Dict[str, CustomResponseBodyTypeDef]],  # (6)
    CaptchaConfig: NotRequired[CaptchaConfigTypeDef],  # (7)
    ChallengeConfig: NotRequired[ChallengeConfigTypeDef],  # (8)
    TokenDomains: NotRequired[List[str]],
    AssociationConfig: NotRequired[AssociationConfigOutputTypeDef],  # (9)
    RetrofittedByFirewallManager: NotRequired[bool],
```

1. See [:material-code-braces: DefaultActionOutputTypeDef](./type_defs.md#defaultactionoutputtypedef) 
2. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
3. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
4. See [:material-code-braces: FirewallManagerRuleGroupTypeDef](./type_defs.md#firewallmanagerrulegrouptypedef) 
5. See [:material-code-braces: FirewallManagerRuleGroupTypeDef](./type_defs.md#firewallmanagerrulegrouptypedef) 
6. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
7. See [:material-code-braces: CaptchaConfigTypeDef](./type_defs.md#captchaconfigtypedef) 
8. See [:material-code-braces: ChallengeConfigTypeDef](./type_defs.md#challengeconfigtypedef) 
9. See [:material-code-braces: AssociationConfigOutputTypeDef](./type_defs.md#associationconfigoutputtypedef) 
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
## ManagedRuleGroupStatementTypeDef

```python
# ManagedRuleGroupStatementTypeDef definition

class ManagedRuleGroupStatementTypeDef(TypedDict):
    VendorName: str,
    Name: str,
    Version: NotRequired[str],
    ExcludedRules: NotRequired[Sequence[ExcludedRuleTypeDef]],  # (1)
    ScopeDownStatement: NotRequired[Mapping[str, Any]],
    ManagedRuleGroupConfigs: NotRequired[Sequence[ManagedRuleGroupConfigUnionTypeDef]],  # (2)
    RuleActionOverrides: NotRequired[Sequence[RuleActionOverrideUnionTypeDef]],  # (3)
```

1. See [:material-code-braces: ExcludedRuleTypeDef](./type_defs.md#excludedruletypedef) 
2. See [:material-code-braces: ManagedRuleGroupConfigTypeDef](./type_defs.md#managedrulegroupconfigtypedef) [:material-code-braces: ManagedRuleGroupConfigOutputTypeDef](./type_defs.md#managedrulegroupconfigoutputtypedef) 
3. See [:material-code-braces: RuleActionOverrideTypeDef](./type_defs.md#ruleactionoverridetypedef) [:material-code-braces: RuleActionOverrideOutputTypeDef](./type_defs.md#ruleactionoverrideoutputtypedef) 
## StatementTypeDef

```python
# StatementTypeDef definition

class StatementTypeDef(TypedDict):
    ByteMatchStatement: NotRequired[ByteMatchStatementUnionTypeDef],  # (1)
    SqliMatchStatement: NotRequired[SqliMatchStatementUnionTypeDef],  # (2)
    XssMatchStatement: NotRequired[XssMatchStatementUnionTypeDef],  # (3)
    SizeConstraintStatement: NotRequired[SizeConstraintStatementUnionTypeDef],  # (4)
    GeoMatchStatement: NotRequired[GeoMatchStatementUnionTypeDef],  # (5)
    RuleGroupReferenceStatement: NotRequired[RuleGroupReferenceStatementUnionTypeDef],  # (6)
    IPSetReferenceStatement: NotRequired[IPSetReferenceStatementTypeDef],  # (7)
    RegexPatternSetReferenceStatement: NotRequired[RegexPatternSetReferenceStatementUnionTypeDef],  # (8)
    RateBasedStatement: NotRequired[RateBasedStatementUnionTypeDef],  # (9)
    AndStatement: NotRequired[AndStatementUnionTypeDef],  # (10)
    OrStatement: NotRequired[OrStatementUnionTypeDef],  # (11)
    NotStatement: NotRequired[NotStatementUnionTypeDef],  # (12)
    ManagedRuleGroupStatement: NotRequired[ManagedRuleGroupStatementUnionTypeDef],  # (13)
    LabelMatchStatement: NotRequired[LabelMatchStatementTypeDef],  # (14)
    RegexMatchStatement: NotRequired[RegexMatchStatementUnionTypeDef],  # (15)
```

1. See [:material-code-braces: ByteMatchStatementTypeDef](./type_defs.md#bytematchstatementtypedef) [:material-code-braces: ByteMatchStatementOutputTypeDef](./type_defs.md#bytematchstatementoutputtypedef) 
2. See [:material-code-braces: SqliMatchStatementTypeDef](./type_defs.md#sqlimatchstatementtypedef) [:material-code-braces: SqliMatchStatementOutputTypeDef](./type_defs.md#sqlimatchstatementoutputtypedef) 
3. See [:material-code-braces: XssMatchStatementTypeDef](./type_defs.md#xssmatchstatementtypedef) [:material-code-braces: XssMatchStatementOutputTypeDef](./type_defs.md#xssmatchstatementoutputtypedef) 
4. See [:material-code-braces: SizeConstraintStatementTypeDef](./type_defs.md#sizeconstraintstatementtypedef) [:material-code-braces: SizeConstraintStatementOutputTypeDef](./type_defs.md#sizeconstraintstatementoutputtypedef) 
5. See [:material-code-braces: GeoMatchStatementTypeDef](./type_defs.md#geomatchstatementtypedef) [:material-code-braces: GeoMatchStatementOutputTypeDef](./type_defs.md#geomatchstatementoutputtypedef) 
6. See [:material-code-braces: RuleGroupReferenceStatementTypeDef](./type_defs.md#rulegroupreferencestatementtypedef) [:material-code-braces: RuleGroupReferenceStatementOutputTypeDef](./type_defs.md#rulegroupreferencestatementoutputtypedef) 
7. See [:material-code-braces: IPSetReferenceStatementTypeDef](./type_defs.md#ipsetreferencestatementtypedef) 
8. See [:material-code-braces: RegexPatternSetReferenceStatementTypeDef](./type_defs.md#regexpatternsetreferencestatementtypedef) [:material-code-braces: RegexPatternSetReferenceStatementOutputTypeDef](./type_defs.md#regexpatternsetreferencestatementoutputtypedef) 
9. See [:material-code-braces: RateBasedStatementTypeDef](./type_defs.md#ratebasedstatementtypedef) [:material-code-braces: RateBasedStatementOutputTypeDef](./type_defs.md#ratebasedstatementoutputtypedef) 
10. See [:material-code-braces: AndStatementTypeDef](./type_defs.md#andstatementtypedef) [:material-code-braces: AndStatementOutputTypeDef](./type_defs.md#andstatementoutputtypedef) 
11. See [:material-code-braces: OrStatementTypeDef](./type_defs.md#orstatementtypedef) [:material-code-braces: OrStatementOutputTypeDef](./type_defs.md#orstatementoutputtypedef) 
12. See [:material-code-braces: NotStatementTypeDef](./type_defs.md#notstatementtypedef) [:material-code-braces: NotStatementOutputTypeDef](./type_defs.md#notstatementoutputtypedef) 
13. See [:material-code-braces: ManagedRuleGroupStatementTypeDef](./type_defs.md#managedrulegroupstatementtypedef) [:material-code-braces: ManagedRuleGroupStatementOutputTypeDef](./type_defs.md#managedrulegroupstatementoutputtypedef) 
14. See [:material-code-braces: LabelMatchStatementTypeDef](./type_defs.md#labelmatchstatementtypedef) 
15. See [:material-code-braces: RegexMatchStatementTypeDef](./type_defs.md#regexmatchstatementtypedef) [:material-code-braces: RegexMatchStatementOutputTypeDef](./type_defs.md#regexmatchstatementoutputtypedef) 
## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    Name: str,
    Priority: int,
    Statement: StatementUnionTypeDef,  # (1)
    VisibilityConfig: VisibilityConfigTypeDef,  # (5)
    Action: NotRequired[RuleActionUnionTypeDef],  # (2)
    OverrideAction: NotRequired[OverrideActionUnionTypeDef],  # (3)
    RuleLabels: NotRequired[Sequence[LabelTypeDef]],  # (4)
    CaptchaConfig: NotRequired[CaptchaConfigTypeDef],  # (6)
    ChallengeConfig: NotRequired[ChallengeConfigTypeDef],  # (7)
```

1. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
2. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
3. See [:material-code-braces: OverrideActionTypeDef](./type_defs.md#overrideactiontypedef) [:material-code-braces: OverrideActionOutputTypeDef](./type_defs.md#overrideactionoutputtypedef) 
4. See [:material-code-braces: LabelTypeDef](./type_defs.md#labeltypedef) 
5. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
6. See [:material-code-braces: CaptchaConfigTypeDef](./type_defs.md#captchaconfigtypedef) 
7. See [:material-code-braces: ChallengeConfigTypeDef](./type_defs.md#challengeconfigtypedef) 
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
## CheckCapacityRequestRequestTypeDef

```python
# CheckCapacityRequestRequestTypeDef definition

class CheckCapacityRequestRequestTypeDef(TypedDict):
    Scope: ScopeType,  # (1)
    Rules: Sequence[RuleUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
