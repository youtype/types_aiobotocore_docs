# Type definitions

> [Index](../README.md) > [MailManager](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MailManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager.html#mailmanager)
    type annotations stubs module [types-aiobotocore-mailmanager](https://pypi.org/project/types-aiobotocore-mailmanager/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## IngressIsInAddressListUnionTypeDef

```python
# IngressIsInAddressListUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import IngressIsInAddressListUnionTypeDef


def get_value() -> IngressIsInAddressListUnionTypeDef:
    return ...


# IngressIsInAddressListUnionTypeDef definition

IngressIsInAddressListUnionTypeDef = Union[
    IngressIsInAddressListTypeDef,  # (1)
    IngressIsInAddressListOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IngressIsInAddressListTypeDef](./type_defs.md#ingressisinaddresslisttypedef) 
2. See [:material-code-braces: IngressIsInAddressListOutputTypeDef](./type_defs.md#ingressisinaddresslistoutputtypedef) 

## RelayAuthenticationUnionTypeDef

```python
# RelayAuthenticationUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import RelayAuthenticationUnionTypeDef


def get_value() -> RelayAuthenticationUnionTypeDef:
    return ...


# RelayAuthenticationUnionTypeDef definition

RelayAuthenticationUnionTypeDef = Union[
    RelayAuthenticationTypeDef,  # (1)
    RelayAuthenticationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RelayAuthenticationTypeDef](./type_defs.md#relayauthenticationtypedef) 
2. See [:material-code-braces: RelayAuthenticationOutputTypeDef](./type_defs.md#relayauthenticationoutputtypedef) 

## ReplaceRecipientActionUnionTypeDef

```python
# ReplaceRecipientActionUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import ReplaceRecipientActionUnionTypeDef


def get_value() -> ReplaceRecipientActionUnionTypeDef:
    return ...


# ReplaceRecipientActionUnionTypeDef definition

ReplaceRecipientActionUnionTypeDef = Union[
    ReplaceRecipientActionTypeDef,  # (1)
    ReplaceRecipientActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ReplaceRecipientActionTypeDef](./type_defs.md#replacerecipientactiontypedef) 
2. See [:material-code-braces: ReplaceRecipientActionOutputTypeDef](./type_defs.md#replacerecipientactionoutputtypedef) 

## RuleDmarcExpressionUnionTypeDef

```python
# RuleDmarcExpressionUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import RuleDmarcExpressionUnionTypeDef


def get_value() -> RuleDmarcExpressionUnionTypeDef:
    return ...


# RuleDmarcExpressionUnionTypeDef definition

RuleDmarcExpressionUnionTypeDef = Union[
    RuleDmarcExpressionTypeDef,  # (1)
    RuleDmarcExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleDmarcExpressionTypeDef](./type_defs.md#ruledmarcexpressiontypedef) 
2. See [:material-code-braces: RuleDmarcExpressionOutputTypeDef](./type_defs.md#ruledmarcexpressionoutputtypedef) 

## RuleIsInAddressListUnionTypeDef

```python
# RuleIsInAddressListUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import RuleIsInAddressListUnionTypeDef


def get_value() -> RuleIsInAddressListUnionTypeDef:
    return ...


# RuleIsInAddressListUnionTypeDef definition

RuleIsInAddressListUnionTypeDef = Union[
    RuleIsInAddressListTypeDef,  # (1)
    RuleIsInAddressListOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleIsInAddressListTypeDef](./type_defs.md#ruleisinaddresslisttypedef) 
2. See [:material-code-braces: RuleIsInAddressListOutputTypeDef](./type_defs.md#ruleisinaddresslistoutputtypedef) 

## IngressIpv4ExpressionUnionTypeDef

```python
# IngressIpv4ExpressionUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import IngressIpv4ExpressionUnionTypeDef


def get_value() -> IngressIpv4ExpressionUnionTypeDef:
    return ...


# IngressIpv4ExpressionUnionTypeDef definition

IngressIpv4ExpressionUnionTypeDef = Union[
    IngressIpv4ExpressionTypeDef,  # (1)
    IngressIpv4ExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IngressIpv4ExpressionTypeDef](./type_defs.md#ingressipv4expressiontypedef) 
2. See [:material-code-braces: IngressIpv4ExpressionOutputTypeDef](./type_defs.md#ingressipv4expressionoutputtypedef) 

## IngressStringExpressionUnionTypeDef

```python
# IngressStringExpressionUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import IngressStringExpressionUnionTypeDef


def get_value() -> IngressStringExpressionUnionTypeDef:
    return ...


# IngressStringExpressionUnionTypeDef definition

IngressStringExpressionUnionTypeDef = Union[
    IngressStringExpressionTypeDef,  # (1)
    IngressStringExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IngressStringExpressionTypeDef](./type_defs.md#ingressstringexpressiontypedef) 
2. See [:material-code-braces: IngressStringExpressionOutputTypeDef](./type_defs.md#ingressstringexpressionoutputtypedef) 

## RuleIpExpressionUnionTypeDef

```python
# RuleIpExpressionUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import RuleIpExpressionUnionTypeDef


def get_value() -> RuleIpExpressionUnionTypeDef:
    return ...


# RuleIpExpressionUnionTypeDef definition

RuleIpExpressionUnionTypeDef = Union[
    RuleIpExpressionTypeDef,  # (1)
    RuleIpExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleIpExpressionTypeDef](./type_defs.md#ruleipexpressiontypedef) 
2. See [:material-code-braces: RuleIpExpressionOutputTypeDef](./type_defs.md#ruleipexpressionoutputtypedef) 

## RuleStringExpressionUnionTypeDef

```python
# RuleStringExpressionUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import RuleStringExpressionUnionTypeDef


def get_value() -> RuleStringExpressionUnionTypeDef:
    return ...


# RuleStringExpressionUnionTypeDef definition

RuleStringExpressionUnionTypeDef = Union[
    RuleStringExpressionTypeDef,  # (1)
    RuleStringExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleStringExpressionTypeDef](./type_defs.md#rulestringexpressiontypedef) 
2. See [:material-code-braces: RuleStringExpressionOutputTypeDef](./type_defs.md#rulestringexpressionoutputtypedef) 

## RuleVerdictExpressionUnionTypeDef

```python
# RuleVerdictExpressionUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import RuleVerdictExpressionUnionTypeDef


def get_value() -> RuleVerdictExpressionUnionTypeDef:
    return ...


# RuleVerdictExpressionUnionTypeDef definition

RuleVerdictExpressionUnionTypeDef = Union[
    RuleVerdictExpressionTypeDef,  # (1)
    RuleVerdictExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleVerdictExpressionTypeDef](./type_defs.md#ruleverdictexpressiontypedef) 
2. See [:material-code-braces: RuleVerdictExpressionOutputTypeDef](./type_defs.md#ruleverdictexpressionoutputtypedef) 

## IngressBooleanToEvaluateUnionTypeDef

```python
# IngressBooleanToEvaluateUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import IngressBooleanToEvaluateUnionTypeDef


def get_value() -> IngressBooleanToEvaluateUnionTypeDef:
    return ...


# IngressBooleanToEvaluateUnionTypeDef definition

IngressBooleanToEvaluateUnionTypeDef = Union[
    IngressBooleanToEvaluateTypeDef,  # (1)
    IngressBooleanToEvaluateOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IngressBooleanToEvaluateTypeDef](./type_defs.md#ingressbooleantoevaluatetypedef) 
2. See [:material-code-braces: IngressBooleanToEvaluateOutputTypeDef](./type_defs.md#ingressbooleantoevaluateoutputtypedef) 

## RuleActionUnionTypeDef

```python
# RuleActionUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import RuleActionUnionTypeDef


def get_value() -> RuleActionUnionTypeDef:
    return ...


# RuleActionUnionTypeDef definition

RuleActionUnionTypeDef = Union[
    RuleActionTypeDef,  # (1)
    RuleActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
2. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 

## RuleBooleanToEvaluateUnionTypeDef

```python
# RuleBooleanToEvaluateUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import RuleBooleanToEvaluateUnionTypeDef


def get_value() -> RuleBooleanToEvaluateUnionTypeDef:
    return ...


# RuleBooleanToEvaluateUnionTypeDef definition

RuleBooleanToEvaluateUnionTypeDef = Union[
    RuleBooleanToEvaluateTypeDef,  # (1)
    RuleBooleanToEvaluateOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleBooleanToEvaluateTypeDef](./type_defs.md#rulebooleantoevaluatetypedef) 
2. See [:material-code-braces: RuleBooleanToEvaluateOutputTypeDef](./type_defs.md#rulebooleantoevaluateoutputtypedef) 

## ArchiveFiltersUnionTypeDef

```python
# ArchiveFiltersUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import ArchiveFiltersUnionTypeDef


def get_value() -> ArchiveFiltersUnionTypeDef:
    return ...


# ArchiveFiltersUnionTypeDef definition

ArchiveFiltersUnionTypeDef = Union[
    ArchiveFiltersTypeDef,  # (1)
    ArchiveFiltersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ArchiveFiltersTypeDef](./type_defs.md#archivefilterstypedef) 
2. See [:material-code-braces: ArchiveFiltersOutputTypeDef](./type_defs.md#archivefiltersoutputtypedef) 

## IngressBooleanExpressionUnionTypeDef

```python
# IngressBooleanExpressionUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import IngressBooleanExpressionUnionTypeDef


def get_value() -> IngressBooleanExpressionUnionTypeDef:
    return ...


# IngressBooleanExpressionUnionTypeDef definition

IngressBooleanExpressionUnionTypeDef = Union[
    IngressBooleanExpressionTypeDef,  # (1)
    IngressBooleanExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IngressBooleanExpressionTypeDef](./type_defs.md#ingressbooleanexpressiontypedef) 
2. See [:material-code-braces: IngressBooleanExpressionOutputTypeDef](./type_defs.md#ingressbooleanexpressionoutputtypedef) 

## RuleBooleanExpressionUnionTypeDef

```python
# RuleBooleanExpressionUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import RuleBooleanExpressionUnionTypeDef


def get_value() -> RuleBooleanExpressionUnionTypeDef:
    return ...


# RuleBooleanExpressionUnionTypeDef definition

RuleBooleanExpressionUnionTypeDef = Union[
    RuleBooleanExpressionTypeDef,  # (1)
    RuleBooleanExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleBooleanExpressionTypeDef](./type_defs.md#rulebooleanexpressiontypedef) 
2. See [:material-code-braces: RuleBooleanExpressionOutputTypeDef](./type_defs.md#rulebooleanexpressionoutputtypedef) 

## PolicyConditionUnionTypeDef

```python
# PolicyConditionUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import PolicyConditionUnionTypeDef


def get_value() -> PolicyConditionUnionTypeDef:
    return ...


# PolicyConditionUnionTypeDef definition

PolicyConditionUnionTypeDef = Union[
    PolicyConditionTypeDef,  # (1)
    PolicyConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PolicyConditionTypeDef](./type_defs.md#policyconditiontypedef) 
2. See [:material-code-braces: PolicyConditionOutputTypeDef](./type_defs.md#policyconditionoutputtypedef) 

## RuleConditionUnionTypeDef

```python
# RuleConditionUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import RuleConditionUnionTypeDef


def get_value() -> RuleConditionUnionTypeDef:
    return ...


# RuleConditionUnionTypeDef definition

RuleConditionUnionTypeDef = Union[
    RuleConditionTypeDef,  # (1)
    RuleConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleConditionTypeDef](./type_defs.md#ruleconditiontypedef) 
2. See [:material-code-braces: RuleConditionOutputTypeDef](./type_defs.md#ruleconditionoutputtypedef) 

## PolicyStatementUnionTypeDef

```python
# PolicyStatementUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import PolicyStatementUnionTypeDef


def get_value() -> PolicyStatementUnionTypeDef:
    return ...


# PolicyStatementUnionTypeDef definition

PolicyStatementUnionTypeDef = Union[
    PolicyStatementTypeDef,  # (1)
    PolicyStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PolicyStatementTypeDef](./type_defs.md#policystatementtypedef) 
2. See [:material-code-braces: PolicyStatementOutputTypeDef](./type_defs.md#policystatementoutputtypedef) 

## RuleUnionTypeDef

```python
# RuleUnionTypeDef Union usage example

from types_aiobotocore_mailmanager.type_defs import RuleUnionTypeDef


def get_value() -> RuleUnionTypeDef:
    return ...


# RuleUnionTypeDef definition

RuleUnionTypeDef = Union[
    RuleTypeDef,  # (1)
    RuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 



## AddHeaderActionTypeDef

```python
# AddHeaderActionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import AddHeaderActionTypeDef


def get_value() -> AddHeaderActionTypeDef:
    return {
        "HeaderName": ...,
    }


# AddHeaderActionTypeDef definition

class AddHeaderActionTypeDef(TypedDict):
    HeaderName: str,
    HeaderValue: str,
```

## AddonInstanceTypeDef

```python
# AddonInstanceTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import AddonInstanceTypeDef


def get_value() -> AddonInstanceTypeDef:
    return {
        "AddonInstanceArn": ...,
    }


# AddonInstanceTypeDef definition

class AddonInstanceTypeDef(TypedDict):
    AddonInstanceArn: NotRequired[str],
    AddonInstanceId: NotRequired[str],
    AddonName: NotRequired[str],
    AddonSubscriptionId: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
```

## AddonSubscriptionTypeDef

```python
# AddonSubscriptionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import AddonSubscriptionTypeDef


def get_value() -> AddonSubscriptionTypeDef:
    return {
        "AddonName": ...,
    }


# AddonSubscriptionTypeDef definition

class AddonSubscriptionTypeDef(TypedDict):
    AddonName: NotRequired[str],
    AddonSubscriptionArn: NotRequired[str],
    AddonSubscriptionId: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
```

## AddressFilterTypeDef

```python
# AddressFilterTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import AddressFilterTypeDef


def get_value() -> AddressFilterTypeDef:
    return {
        "AddressPrefix": ...,
    }


# AddressFilterTypeDef definition

class AddressFilterTypeDef(TypedDict):
    AddressPrefix: NotRequired[str],
```

## AddressListTypeDef

```python
# AddressListTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import AddressListTypeDef


def get_value() -> AddressListTypeDef:
    return {
        "AddressListArn": ...,
    }


# AddressListTypeDef definition

class AddressListTypeDef(TypedDict):
    AddressListArn: str,
    AddressListId: str,
    AddressListName: str,
    CreatedTimestamp: datetime,
    LastUpdatedTimestamp: datetime,
```

## AnalysisTypeDef

```python
# AnalysisTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import AnalysisTypeDef


def get_value() -> AnalysisTypeDef:
    return {
        "Analyzer": ...,
    }


# AnalysisTypeDef definition

class AnalysisTypeDef(TypedDict):
    Analyzer: str,
    ResultField: str,
```

## ArchiveActionTypeDef

```python
# ArchiveActionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ArchiveActionTypeDef


def get_value() -> ArchiveActionTypeDef:
    return {
        "ActionFailurePolicy": ...,
    }


# ArchiveActionTypeDef definition

class ArchiveActionTypeDef(TypedDict):
    TargetArchive: str,
    ActionFailurePolicy: NotRequired[ActionFailurePolicyType],  # (1)
```

1. See [:material-code-brackets: ActionFailurePolicyType](./literals.md#actionfailurepolicytype) 
## ArchiveBooleanToEvaluateTypeDef

```python
# ArchiveBooleanToEvaluateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ArchiveBooleanToEvaluateTypeDef


def get_value() -> ArchiveBooleanToEvaluateTypeDef:
    return {
        "Attribute": ...,
    }


# ArchiveBooleanToEvaluateTypeDef definition

class ArchiveBooleanToEvaluateTypeDef(TypedDict):
    Attribute: NotRequired[ArchiveBooleanEmailAttributeType],  # (1)
```

1. See [:material-code-brackets: ArchiveBooleanEmailAttributeType](./literals.md#archivebooleanemailattributetype) 
## ArchiveRetentionTypeDef

```python
# ArchiveRetentionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ArchiveRetentionTypeDef


def get_value() -> ArchiveRetentionTypeDef:
    return {
        "RetentionPeriod": ...,
    }


# ArchiveRetentionTypeDef definition

class ArchiveRetentionTypeDef(TypedDict):
    RetentionPeriod: NotRequired[RetentionPeriodType],  # (1)
```

1. See [:material-code-brackets: RetentionPeriodType](./literals.md#retentionperiodtype) 
## ArchiveStringToEvaluateTypeDef

```python
# ArchiveStringToEvaluateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ArchiveStringToEvaluateTypeDef


def get_value() -> ArchiveStringToEvaluateTypeDef:
    return {
        "Attribute": ...,
    }


# ArchiveStringToEvaluateTypeDef definition

class ArchiveStringToEvaluateTypeDef(TypedDict):
    Attribute: NotRequired[ArchiveStringEmailAttributeType],  # (1)
```

1. See [:material-code-brackets: ArchiveStringEmailAttributeType](./literals.md#archivestringemailattributetype) 
## ArchiveTypeDef

```python
# ArchiveTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ArchiveTypeDef


def get_value() -> ArchiveTypeDef:
    return {
        "ArchiveId": ...,
    }


# ArchiveTypeDef definition

class ArchiveTypeDef(TypedDict):
    ArchiveId: str,
    ArchiveName: NotRequired[str],
    ArchiveState: NotRequired[ArchiveStateType],  # (1)
    LastUpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ArchiveStateType](./literals.md#archivestatetype) 
## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## ImportDataFormatTypeDef

```python
# ImportDataFormatTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ImportDataFormatTypeDef


def get_value() -> ImportDataFormatTypeDef:
    return {
        "ImportDataType": ...,
    }


# ImportDataFormatTypeDef definition

class ImportDataFormatTypeDef(TypedDict):
    ImportDataType: ImportDataTypeType,  # (1)
```

1. See [:material-code-brackets: ImportDataTypeType](./literals.md#importdatatypetype) 
## IngressPointConfigurationTypeDef

```python
# IngressPointConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressPointConfigurationTypeDef


def get_value() -> IngressPointConfigurationTypeDef:
    return {
        "SecretArn": ...,
    }


# IngressPointConfigurationTypeDef definition

class IngressPointConfigurationTypeDef(TypedDict):
    SecretArn: NotRequired[str],
    SmtpPassword: NotRequired[str],
```

## DeleteAddonInstanceRequestTypeDef

```python
# DeleteAddonInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import DeleteAddonInstanceRequestTypeDef


def get_value() -> DeleteAddonInstanceRequestTypeDef:
    return {
        "AddonInstanceId": ...,
    }


# DeleteAddonInstanceRequestTypeDef definition

class DeleteAddonInstanceRequestTypeDef(TypedDict):
    AddonInstanceId: str,
```

## DeleteAddonSubscriptionRequestTypeDef

```python
# DeleteAddonSubscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import DeleteAddonSubscriptionRequestTypeDef


def get_value() -> DeleteAddonSubscriptionRequestTypeDef:
    return {
        "AddonSubscriptionId": ...,
    }


# DeleteAddonSubscriptionRequestTypeDef definition

class DeleteAddonSubscriptionRequestTypeDef(TypedDict):
    AddonSubscriptionId: str,
```

## DeleteAddressListRequestTypeDef

```python
# DeleteAddressListRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import DeleteAddressListRequestTypeDef


def get_value() -> DeleteAddressListRequestTypeDef:
    return {
        "AddressListId": ...,
    }


# DeleteAddressListRequestTypeDef definition

class DeleteAddressListRequestTypeDef(TypedDict):
    AddressListId: str,
```

## DeleteArchiveRequestTypeDef

```python
# DeleteArchiveRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import DeleteArchiveRequestTypeDef


def get_value() -> DeleteArchiveRequestTypeDef:
    return {
        "ArchiveId": ...,
    }


# DeleteArchiveRequestTypeDef definition

class DeleteArchiveRequestTypeDef(TypedDict):
    ArchiveId: str,
```

## DeleteIngressPointRequestTypeDef

```python
# DeleteIngressPointRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import DeleteIngressPointRequestTypeDef


def get_value() -> DeleteIngressPointRequestTypeDef:
    return {
        "IngressPointId": ...,
    }


# DeleteIngressPointRequestTypeDef definition

class DeleteIngressPointRequestTypeDef(TypedDict):
    IngressPointId: str,
```

## DeleteRelayRequestTypeDef

```python
# DeleteRelayRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import DeleteRelayRequestTypeDef


def get_value() -> DeleteRelayRequestTypeDef:
    return {
        "RelayId": ...,
    }


# DeleteRelayRequestTypeDef definition

class DeleteRelayRequestTypeDef(TypedDict):
    RelayId: str,
```

## DeleteRuleSetRequestTypeDef

```python
# DeleteRuleSetRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import DeleteRuleSetRequestTypeDef


def get_value() -> DeleteRuleSetRequestTypeDef:
    return {
        "RuleSetId": ...,
    }


# DeleteRuleSetRequestTypeDef definition

class DeleteRuleSetRequestTypeDef(TypedDict):
    RuleSetId: str,
```

## DeleteTrafficPolicyRequestTypeDef

```python
# DeleteTrafficPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import DeleteTrafficPolicyRequestTypeDef


def get_value() -> DeleteTrafficPolicyRequestTypeDef:
    return {
        "TrafficPolicyId": ...,
    }


# DeleteTrafficPolicyRequestTypeDef definition

class DeleteTrafficPolicyRequestTypeDef(TypedDict):
    TrafficPolicyId: str,
```

## DeliverToMailboxActionTypeDef

```python
# DeliverToMailboxActionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import DeliverToMailboxActionTypeDef


def get_value() -> DeliverToMailboxActionTypeDef:
    return {
        "ActionFailurePolicy": ...,
    }


# DeliverToMailboxActionTypeDef definition

class DeliverToMailboxActionTypeDef(TypedDict):
    MailboxArn: str,
    RoleArn: str,
    ActionFailurePolicy: NotRequired[ActionFailurePolicyType],  # (1)
```

1. See [:material-code-brackets: ActionFailurePolicyType](./literals.md#actionfailurepolicytype) 
## DeliverToQBusinessActionTypeDef

```python
# DeliverToQBusinessActionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import DeliverToQBusinessActionTypeDef


def get_value() -> DeliverToQBusinessActionTypeDef:
    return {
        "ActionFailurePolicy": ...,
    }


# DeliverToQBusinessActionTypeDef definition

class DeliverToQBusinessActionTypeDef(TypedDict):
    ApplicationId: str,
    IndexId: str,
    RoleArn: str,
    ActionFailurePolicy: NotRequired[ActionFailurePolicyType],  # (1)
```

1. See [:material-code-brackets: ActionFailurePolicyType](./literals.md#actionfailurepolicytype) 
## DeregisterMemberFromAddressListRequestTypeDef

```python
# DeregisterMemberFromAddressListRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import DeregisterMemberFromAddressListRequestTypeDef


def get_value() -> DeregisterMemberFromAddressListRequestTypeDef:
    return {
        "Address": ...,
    }


# DeregisterMemberFromAddressListRequestTypeDef definition

class DeregisterMemberFromAddressListRequestTypeDef(TypedDict):
    Address: str,
    AddressListId: str,
```

## EnvelopeTypeDef

```python
# EnvelopeTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import EnvelopeTypeDef


def get_value() -> EnvelopeTypeDef:
    return {
        "From": ...,
    }


# EnvelopeTypeDef definition

class EnvelopeTypeDef(TypedDict):
    From: NotRequired[str],
    Helo: NotRequired[str],
    To: NotRequired[List[str]],
```

## S3ExportDestinationConfigurationTypeDef

```python
# S3ExportDestinationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import S3ExportDestinationConfigurationTypeDef


def get_value() -> S3ExportDestinationConfigurationTypeDef:
    return {
        "S3Location": ...,
    }


# S3ExportDestinationConfigurationTypeDef definition

class S3ExportDestinationConfigurationTypeDef(TypedDict):
    S3Location: NotRequired[str],
```

## ExportStatusTypeDef

```python
# ExportStatusTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ExportStatusTypeDef


def get_value() -> ExportStatusTypeDef:
    return {
        "CompletionTimestamp": ...,
    }


# ExportStatusTypeDef definition

class ExportStatusTypeDef(TypedDict):
    CompletionTimestamp: NotRequired[datetime],
    ErrorMessage: NotRequired[str],
    State: NotRequired[ExportStateType],  # (1)
    SubmissionTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ExportStateType](./literals.md#exportstatetype) 
## GetAddonInstanceRequestTypeDef

```python
# GetAddonInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetAddonInstanceRequestTypeDef


def get_value() -> GetAddonInstanceRequestTypeDef:
    return {
        "AddonInstanceId": ...,
    }


# GetAddonInstanceRequestTypeDef definition

class GetAddonInstanceRequestTypeDef(TypedDict):
    AddonInstanceId: str,
```

## GetAddonSubscriptionRequestTypeDef

```python
# GetAddonSubscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetAddonSubscriptionRequestTypeDef


def get_value() -> GetAddonSubscriptionRequestTypeDef:
    return {
        "AddonSubscriptionId": ...,
    }


# GetAddonSubscriptionRequestTypeDef definition

class GetAddonSubscriptionRequestTypeDef(TypedDict):
    AddonSubscriptionId: str,
```

## GetAddressListImportJobRequestTypeDef

```python
# GetAddressListImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetAddressListImportJobRequestTypeDef


def get_value() -> GetAddressListImportJobRequestTypeDef:
    return {
        "JobId": ...,
    }


# GetAddressListImportJobRequestTypeDef definition

class GetAddressListImportJobRequestTypeDef(TypedDict):
    JobId: str,
```

## GetAddressListRequestTypeDef

```python
# GetAddressListRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetAddressListRequestTypeDef


def get_value() -> GetAddressListRequestTypeDef:
    return {
        "AddressListId": ...,
    }


# GetAddressListRequestTypeDef definition

class GetAddressListRequestTypeDef(TypedDict):
    AddressListId: str,
```

## GetArchiveExportRequestTypeDef

```python
# GetArchiveExportRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetArchiveExportRequestTypeDef


def get_value() -> GetArchiveExportRequestTypeDef:
    return {
        "ExportId": ...,
    }


# GetArchiveExportRequestTypeDef definition

class GetArchiveExportRequestTypeDef(TypedDict):
    ExportId: str,
```

## GetArchiveMessageContentRequestTypeDef

```python
# GetArchiveMessageContentRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetArchiveMessageContentRequestTypeDef


def get_value() -> GetArchiveMessageContentRequestTypeDef:
    return {
        "ArchivedMessageId": ...,
    }


# GetArchiveMessageContentRequestTypeDef definition

class GetArchiveMessageContentRequestTypeDef(TypedDict):
    ArchivedMessageId: str,
```

## MessageBodyTypeDef

```python
# MessageBodyTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import MessageBodyTypeDef


def get_value() -> MessageBodyTypeDef:
    return {
        "Html": ...,
    }


# MessageBodyTypeDef definition

class MessageBodyTypeDef(TypedDict):
    Html: NotRequired[str],
    MessageMalformed: NotRequired[bool],
    Text: NotRequired[str],
```

## GetArchiveMessageRequestTypeDef

```python
# GetArchiveMessageRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetArchiveMessageRequestTypeDef


def get_value() -> GetArchiveMessageRequestTypeDef:
    return {
        "ArchivedMessageId": ...,
    }


# GetArchiveMessageRequestTypeDef definition

class GetArchiveMessageRequestTypeDef(TypedDict):
    ArchivedMessageId: str,
```

## MetadataTypeDef

```python
# MetadataTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import MetadataTypeDef


def get_value() -> MetadataTypeDef:
    return {
        "ConfigurationSet": ...,
    }


# MetadataTypeDef definition

class MetadataTypeDef(TypedDict):
    ConfigurationSet: NotRequired[str],
    IngressPointId: NotRequired[str],
    RuleSetId: NotRequired[str],
    SenderHostname: NotRequired[str],
    SenderIpAddress: NotRequired[str],
    SendingMethod: NotRequired[str],
    SendingPool: NotRequired[str],
    SourceArn: NotRequired[str],
    SourceIdentity: NotRequired[str],
    Timestamp: NotRequired[datetime],
    TlsCipherSuite: NotRequired[str],
    TlsProtocol: NotRequired[str],
    TrafficPolicyId: NotRequired[str],
```

## GetArchiveRequestTypeDef

```python
# GetArchiveRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetArchiveRequestTypeDef


def get_value() -> GetArchiveRequestTypeDef:
    return {
        "ArchiveId": ...,
    }


# GetArchiveRequestTypeDef definition

class GetArchiveRequestTypeDef(TypedDict):
    ArchiveId: str,
```

## GetArchiveSearchRequestTypeDef

```python
# GetArchiveSearchRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetArchiveSearchRequestTypeDef


def get_value() -> GetArchiveSearchRequestTypeDef:
    return {
        "SearchId": ...,
    }


# GetArchiveSearchRequestTypeDef definition

class GetArchiveSearchRequestTypeDef(TypedDict):
    SearchId: str,
```

## SearchStatusTypeDef

```python
# SearchStatusTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import SearchStatusTypeDef


def get_value() -> SearchStatusTypeDef:
    return {
        "CompletionTimestamp": ...,
    }


# SearchStatusTypeDef definition

class SearchStatusTypeDef(TypedDict):
    CompletionTimestamp: NotRequired[datetime],
    ErrorMessage: NotRequired[str],
    State: NotRequired[SearchStateType],  # (1)
    SubmissionTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: SearchStateType](./literals.md#searchstatetype) 
## GetArchiveSearchResultsRequestTypeDef

```python
# GetArchiveSearchResultsRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetArchiveSearchResultsRequestTypeDef


def get_value() -> GetArchiveSearchResultsRequestTypeDef:
    return {
        "SearchId": ...,
    }


# GetArchiveSearchResultsRequestTypeDef definition

class GetArchiveSearchResultsRequestTypeDef(TypedDict):
    SearchId: str,
```

## GetIngressPointRequestTypeDef

```python
# GetIngressPointRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetIngressPointRequestTypeDef


def get_value() -> GetIngressPointRequestTypeDef:
    return {
        "IngressPointId": ...,
    }


# GetIngressPointRequestTypeDef definition

class GetIngressPointRequestTypeDef(TypedDict):
    IngressPointId: str,
```

## GetMemberOfAddressListRequestTypeDef

```python
# GetMemberOfAddressListRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetMemberOfAddressListRequestTypeDef


def get_value() -> GetMemberOfAddressListRequestTypeDef:
    return {
        "Address": ...,
    }


# GetMemberOfAddressListRequestTypeDef definition

class GetMemberOfAddressListRequestTypeDef(TypedDict):
    Address: str,
    AddressListId: str,
```

## GetRelayRequestTypeDef

```python
# GetRelayRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetRelayRequestTypeDef


def get_value() -> GetRelayRequestTypeDef:
    return {
        "RelayId": ...,
    }


# GetRelayRequestTypeDef definition

class GetRelayRequestTypeDef(TypedDict):
    RelayId: str,
```

## RelayAuthenticationOutputTypeDef

```python
# RelayAuthenticationOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RelayAuthenticationOutputTypeDef


def get_value() -> RelayAuthenticationOutputTypeDef:
    return {
        "NoAuthentication": ...,
    }


# RelayAuthenticationOutputTypeDef definition

class RelayAuthenticationOutputTypeDef(TypedDict):
    NoAuthentication: NotRequired[Dict[str, Any]],
    SecretArn: NotRequired[str],
```

## GetRuleSetRequestTypeDef

```python
# GetRuleSetRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetRuleSetRequestTypeDef


def get_value() -> GetRuleSetRequestTypeDef:
    return {
        "RuleSetId": ...,
    }


# GetRuleSetRequestTypeDef definition

class GetRuleSetRequestTypeDef(TypedDict):
    RuleSetId: str,
```

## GetTrafficPolicyRequestTypeDef

```python
# GetTrafficPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetTrafficPolicyRequestTypeDef


def get_value() -> GetTrafficPolicyRequestTypeDef:
    return {
        "TrafficPolicyId": ...,
    }


# GetTrafficPolicyRequestTypeDef definition

class GetTrafficPolicyRequestTypeDef(TypedDict):
    TrafficPolicyId: str,
```

## IngressAnalysisTypeDef

```python
# IngressAnalysisTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressAnalysisTypeDef


def get_value() -> IngressAnalysisTypeDef:
    return {
        "Analyzer": ...,
    }


# IngressAnalysisTypeDef definition

class IngressAnalysisTypeDef(TypedDict):
    Analyzer: str,
    ResultField: str,
```

## IngressIsInAddressListOutputTypeDef

```python
# IngressIsInAddressListOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressIsInAddressListOutputTypeDef


def get_value() -> IngressIsInAddressListOutputTypeDef:
    return {
        "AddressLists": ...,
    }


# IngressIsInAddressListOutputTypeDef definition

class IngressIsInAddressListOutputTypeDef(TypedDict):
    AddressLists: List[str],
    Attribute: IngressAddressListEmailAttributeType,  # (1)
```

1. See [:material-code-brackets: IngressAddressListEmailAttributeType](./literals.md#ingressaddresslistemailattributetype) 
## IngressIpToEvaluateTypeDef

```python
# IngressIpToEvaluateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressIpToEvaluateTypeDef


def get_value() -> IngressIpToEvaluateTypeDef:
    return {
        "Attribute": ...,
    }


# IngressIpToEvaluateTypeDef definition

class IngressIpToEvaluateTypeDef(TypedDict):
    Attribute: NotRequired[IngressIpv4AttributeType],  # (1)
```

1. See [:material-code-brackets: IngressIpv4AttributeType](./literals.md#ingressipv4attributetype) 
## IngressIsInAddressListTypeDef

```python
# IngressIsInAddressListTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressIsInAddressListTypeDef


def get_value() -> IngressIsInAddressListTypeDef:
    return {
        "AddressLists": ...,
    }


# IngressIsInAddressListTypeDef definition

class IngressIsInAddressListTypeDef(TypedDict):
    AddressLists: Sequence[str],
    Attribute: IngressAddressListEmailAttributeType,  # (1)
```

1. See [:material-code-brackets: IngressAddressListEmailAttributeType](./literals.md#ingressaddresslistemailattributetype) 
## IngressPointPasswordConfigurationTypeDef

```python
# IngressPointPasswordConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressPointPasswordConfigurationTypeDef


def get_value() -> IngressPointPasswordConfigurationTypeDef:
    return {
        "PreviousSmtpPasswordExpiryTimestamp": ...,
    }


# IngressPointPasswordConfigurationTypeDef definition

class IngressPointPasswordConfigurationTypeDef(TypedDict):
    PreviousSmtpPasswordExpiryTimestamp: NotRequired[datetime],
    PreviousSmtpPasswordVersion: NotRequired[str],
    SmtpPasswordVersion: NotRequired[str],
```

## IngressPointTypeDef

```python
# IngressPointTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressPointTypeDef


def get_value() -> IngressPointTypeDef:
    return {
        "ARecord": ...,
    }


# IngressPointTypeDef definition

class IngressPointTypeDef(TypedDict):
    IngressPointId: str,
    IngressPointName: str,
    Status: IngressPointStatusType,  # (1)
    Type: IngressPointTypeType,  # (2)
    ARecord: NotRequired[str],
```

1. See [:material-code-brackets: IngressPointStatusType](./literals.md#ingresspointstatustype) 
2. See [:material-code-brackets: IngressPointTypeType](./literals.md#ingresspointtypetype) 
## IngressStringToEvaluateTypeDef

```python
# IngressStringToEvaluateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressStringToEvaluateTypeDef


def get_value() -> IngressStringToEvaluateTypeDef:
    return {
        "Attribute": ...,
    }


# IngressStringToEvaluateTypeDef definition

class IngressStringToEvaluateTypeDef(TypedDict):
    Attribute: NotRequired[IngressStringEmailAttributeType],  # (1)
```

1. See [:material-code-brackets: IngressStringEmailAttributeType](./literals.md#ingressstringemailattributetype) 
## IngressTlsProtocolToEvaluateTypeDef

```python
# IngressTlsProtocolToEvaluateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressTlsProtocolToEvaluateTypeDef


def get_value() -> IngressTlsProtocolToEvaluateTypeDef:
    return {
        "Attribute": ...,
    }


# IngressTlsProtocolToEvaluateTypeDef definition

class IngressTlsProtocolToEvaluateTypeDef(TypedDict):
    Attribute: NotRequired[IngressTlsAttributeType],  # (1)
```

1. See [:material-code-brackets: IngressTlsAttributeType](./literals.md#ingresstlsattributetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAddonInstancesRequestTypeDef

```python
# ListAddonInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListAddonInstancesRequestTypeDef


def get_value() -> ListAddonInstancesRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListAddonInstancesRequestTypeDef definition

class ListAddonInstancesRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListAddonSubscriptionsRequestTypeDef

```python
# ListAddonSubscriptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListAddonSubscriptionsRequestTypeDef


def get_value() -> ListAddonSubscriptionsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListAddonSubscriptionsRequestTypeDef definition

class ListAddonSubscriptionsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListAddressListImportJobsRequestTypeDef

```python
# ListAddressListImportJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListAddressListImportJobsRequestTypeDef


def get_value() -> ListAddressListImportJobsRequestTypeDef:
    return {
        "AddressListId": ...,
    }


# ListAddressListImportJobsRequestTypeDef definition

class ListAddressListImportJobsRequestTypeDef(TypedDict):
    AddressListId: str,
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListAddressListsRequestTypeDef

```python
# ListAddressListsRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListAddressListsRequestTypeDef


def get_value() -> ListAddressListsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListAddressListsRequestTypeDef definition

class ListAddressListsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListArchiveExportsRequestTypeDef

```python
# ListArchiveExportsRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListArchiveExportsRequestTypeDef


def get_value() -> ListArchiveExportsRequestTypeDef:
    return {
        "ArchiveId": ...,
    }


# ListArchiveExportsRequestTypeDef definition

class ListArchiveExportsRequestTypeDef(TypedDict):
    ArchiveId: str,
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListArchiveSearchesRequestTypeDef

```python
# ListArchiveSearchesRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListArchiveSearchesRequestTypeDef


def get_value() -> ListArchiveSearchesRequestTypeDef:
    return {
        "ArchiveId": ...,
    }


# ListArchiveSearchesRequestTypeDef definition

class ListArchiveSearchesRequestTypeDef(TypedDict):
    ArchiveId: str,
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListArchivesRequestTypeDef

```python
# ListArchivesRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListArchivesRequestTypeDef


def get_value() -> ListArchivesRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListArchivesRequestTypeDef definition

class ListArchivesRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListIngressPointsRequestTypeDef

```python
# ListIngressPointsRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListIngressPointsRequestTypeDef


def get_value() -> ListIngressPointsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListIngressPointsRequestTypeDef definition

class ListIngressPointsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## SavedAddressTypeDef

```python
# SavedAddressTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import SavedAddressTypeDef


def get_value() -> SavedAddressTypeDef:
    return {
        "Address": ...,
    }


# SavedAddressTypeDef definition

class SavedAddressTypeDef(TypedDict):
    Address: str,
    CreatedTimestamp: datetime,
```

## ListRelaysRequestTypeDef

```python
# ListRelaysRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListRelaysRequestTypeDef


def get_value() -> ListRelaysRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListRelaysRequestTypeDef definition

class ListRelaysRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## RelayTypeDef

```python
# RelayTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RelayTypeDef


def get_value() -> RelayTypeDef:
    return {
        "LastModifiedTimestamp": ...,
    }


# RelayTypeDef definition

class RelayTypeDef(TypedDict):
    LastModifiedTimestamp: NotRequired[datetime],
    RelayId: NotRequired[str],
    RelayName: NotRequired[str],
```

## ListRuleSetsRequestTypeDef

```python
# ListRuleSetsRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListRuleSetsRequestTypeDef


def get_value() -> ListRuleSetsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListRuleSetsRequestTypeDef definition

class ListRuleSetsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## RuleSetTypeDef

```python
# RuleSetTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleSetTypeDef


def get_value() -> RuleSetTypeDef:
    return {
        "LastModificationDate": ...,
    }


# RuleSetTypeDef definition

class RuleSetTypeDef(TypedDict):
    LastModificationDate: NotRequired[datetime],
    RuleSetId: NotRequired[str],
    RuleSetName: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListTrafficPoliciesRequestTypeDef

```python
# ListTrafficPoliciesRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListTrafficPoliciesRequestTypeDef


def get_value() -> ListTrafficPoliciesRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListTrafficPoliciesRequestTypeDef definition

class ListTrafficPoliciesRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## TrafficPolicyTypeDef

```python
# TrafficPolicyTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import TrafficPolicyTypeDef


def get_value() -> TrafficPolicyTypeDef:
    return {
        "DefaultAction": ...,
    }


# TrafficPolicyTypeDef definition

class TrafficPolicyTypeDef(TypedDict):
    DefaultAction: AcceptActionType,  # (1)
    TrafficPolicyId: str,
    TrafficPolicyName: str,
```

1. See [:material-code-brackets: AcceptActionType](./literals.md#acceptactiontype) 
## RegisterMemberToAddressListRequestTypeDef

```python
# RegisterMemberToAddressListRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RegisterMemberToAddressListRequestTypeDef


def get_value() -> RegisterMemberToAddressListRequestTypeDef:
    return {
        "Address": ...,
    }


# RegisterMemberToAddressListRequestTypeDef definition

class RegisterMemberToAddressListRequestTypeDef(TypedDict):
    Address: str,
    AddressListId: str,
```

## RelayActionTypeDef

```python
# RelayActionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RelayActionTypeDef


def get_value() -> RelayActionTypeDef:
    return {
        "ActionFailurePolicy": ...,
    }


# RelayActionTypeDef definition

class RelayActionTypeDef(TypedDict):
    Relay: str,
    ActionFailurePolicy: NotRequired[ActionFailurePolicyType],  # (1)
    MailFrom: NotRequired[MailFromType],  # (2)
```

1. See [:material-code-brackets: ActionFailurePolicyType](./literals.md#actionfailurepolicytype) 
2. See [:material-code-brackets: MailFromType](./literals.md#mailfromtype) 
## RelayAuthenticationTypeDef

```python
# RelayAuthenticationTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RelayAuthenticationTypeDef


def get_value() -> RelayAuthenticationTypeDef:
    return {
        "NoAuthentication": ...,
    }


# RelayAuthenticationTypeDef definition

class RelayAuthenticationTypeDef(TypedDict):
    NoAuthentication: NotRequired[Mapping[str, Any]],
    SecretArn: NotRequired[str],
```

## ReplaceRecipientActionOutputTypeDef

```python
# ReplaceRecipientActionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ReplaceRecipientActionOutputTypeDef


def get_value() -> ReplaceRecipientActionOutputTypeDef:
    return {
        "ReplaceWith": ...,
    }


# ReplaceRecipientActionOutputTypeDef definition

class ReplaceRecipientActionOutputTypeDef(TypedDict):
    ReplaceWith: NotRequired[List[str]],
```

## ReplaceRecipientActionTypeDef

```python
# ReplaceRecipientActionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ReplaceRecipientActionTypeDef


def get_value() -> ReplaceRecipientActionTypeDef:
    return {
        "ReplaceWith": ...,
    }


# ReplaceRecipientActionTypeDef definition

class ReplaceRecipientActionTypeDef(TypedDict):
    ReplaceWith: NotRequired[Sequence[str]],
```

## S3ActionTypeDef

```python
# S3ActionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import S3ActionTypeDef


def get_value() -> S3ActionTypeDef:
    return {
        "ActionFailurePolicy": ...,
    }


# S3ActionTypeDef definition

class S3ActionTypeDef(TypedDict):
    RoleArn: str,
    S3Bucket: str,
    ActionFailurePolicy: NotRequired[ActionFailurePolicyType],  # (1)
    S3Prefix: NotRequired[str],
    S3SseKmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: ActionFailurePolicyType](./literals.md#actionfailurepolicytype) 
## SendActionTypeDef

```python
# SendActionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import SendActionTypeDef


def get_value() -> SendActionTypeDef:
    return {
        "ActionFailurePolicy": ...,
    }


# SendActionTypeDef definition

class SendActionTypeDef(TypedDict):
    RoleArn: str,
    ActionFailurePolicy: NotRequired[ActionFailurePolicyType],  # (1)
```

1. See [:material-code-brackets: ActionFailurePolicyType](./literals.md#actionfailurepolicytype) 
## RuleIsInAddressListOutputTypeDef

```python
# RuleIsInAddressListOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleIsInAddressListOutputTypeDef


def get_value() -> RuleIsInAddressListOutputTypeDef:
    return {
        "AddressLists": ...,
    }


# RuleIsInAddressListOutputTypeDef definition

class RuleIsInAddressListOutputTypeDef(TypedDict):
    AddressLists: List[str],
    Attribute: RuleAddressListEmailAttributeType,  # (1)
```

1. See [:material-code-brackets: RuleAddressListEmailAttributeType](./literals.md#ruleaddresslistemailattributetype) 
## RuleDmarcExpressionOutputTypeDef

```python
# RuleDmarcExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleDmarcExpressionOutputTypeDef


def get_value() -> RuleDmarcExpressionOutputTypeDef:
    return {
        "Operator": ...,
    }


# RuleDmarcExpressionOutputTypeDef definition

class RuleDmarcExpressionOutputTypeDef(TypedDict):
    Operator: RuleDmarcOperatorType,  # (1)
    Values: List[RuleDmarcPolicyType],  # (2)
```

1. See [:material-code-brackets: RuleDmarcOperatorType](./literals.md#ruledmarcoperatortype) 
2. See [:material-code-brackets: RuleDmarcPolicyType](./literals.md#ruledmarcpolicytype) 
## RuleDmarcExpressionTypeDef

```python
# RuleDmarcExpressionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleDmarcExpressionTypeDef


def get_value() -> RuleDmarcExpressionTypeDef:
    return {
        "Operator": ...,
    }


# RuleDmarcExpressionTypeDef definition

class RuleDmarcExpressionTypeDef(TypedDict):
    Operator: RuleDmarcOperatorType,  # (1)
    Values: Sequence[RuleDmarcPolicyType],  # (2)
```

1. See [:material-code-brackets: RuleDmarcOperatorType](./literals.md#ruledmarcoperatortype) 
2. See [:material-code-brackets: RuleDmarcPolicyType](./literals.md#ruledmarcpolicytype) 
## RuleIpToEvaluateTypeDef

```python
# RuleIpToEvaluateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleIpToEvaluateTypeDef


def get_value() -> RuleIpToEvaluateTypeDef:
    return {
        "Attribute": ...,
    }


# RuleIpToEvaluateTypeDef definition

class RuleIpToEvaluateTypeDef(TypedDict):
    Attribute: NotRequired[RuleIpEmailAttributeType],  # (1)
```

1. See [:material-code-brackets: RuleIpEmailAttributeType](./literals.md#ruleipemailattributetype) 
## RuleIsInAddressListTypeDef

```python
# RuleIsInAddressListTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleIsInAddressListTypeDef


def get_value() -> RuleIsInAddressListTypeDef:
    return {
        "AddressLists": ...,
    }


# RuleIsInAddressListTypeDef definition

class RuleIsInAddressListTypeDef(TypedDict):
    AddressLists: Sequence[str],
    Attribute: RuleAddressListEmailAttributeType,  # (1)
```

1. See [:material-code-brackets: RuleAddressListEmailAttributeType](./literals.md#ruleaddresslistemailattributetype) 
## RuleNumberToEvaluateTypeDef

```python
# RuleNumberToEvaluateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleNumberToEvaluateTypeDef


def get_value() -> RuleNumberToEvaluateTypeDef:
    return {
        "Attribute": ...,
    }


# RuleNumberToEvaluateTypeDef definition

class RuleNumberToEvaluateTypeDef(TypedDict):
    Attribute: NotRequired[RuleNumberEmailAttributeType],  # (1)
```

1. See [:material-code-brackets: RuleNumberEmailAttributeType](./literals.md#rulenumberemailattributetype) 
## RuleStringToEvaluateTypeDef

```python
# RuleStringToEvaluateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleStringToEvaluateTypeDef


def get_value() -> RuleStringToEvaluateTypeDef:
    return {
        "Attribute": ...,
    }


# RuleStringToEvaluateTypeDef definition

class RuleStringToEvaluateTypeDef(TypedDict):
    Attribute: NotRequired[RuleStringEmailAttributeType],  # (1)
    MimeHeaderAttribute: NotRequired[str],
```

1. See [:material-code-brackets: RuleStringEmailAttributeType](./literals.md#rulestringemailattributetype) 
## StartAddressListImportJobRequestTypeDef

```python
# StartAddressListImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import StartAddressListImportJobRequestTypeDef


def get_value() -> StartAddressListImportJobRequestTypeDef:
    return {
        "JobId": ...,
    }


# StartAddressListImportJobRequestTypeDef definition

class StartAddressListImportJobRequestTypeDef(TypedDict):
    JobId: str,
```

## StopAddressListImportJobRequestTypeDef

```python
# StopAddressListImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import StopAddressListImportJobRequestTypeDef


def get_value() -> StopAddressListImportJobRequestTypeDef:
    return {
        "JobId": ...,
    }


# StopAddressListImportJobRequestTypeDef definition

class StopAddressListImportJobRequestTypeDef(TypedDict):
    JobId: str,
```

## StopArchiveExportRequestTypeDef

```python
# StopArchiveExportRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import StopArchiveExportRequestTypeDef


def get_value() -> StopArchiveExportRequestTypeDef:
    return {
        "ExportId": ...,
    }


# StopArchiveExportRequestTypeDef definition

class StopArchiveExportRequestTypeDef(TypedDict):
    ExportId: str,
```

## StopArchiveSearchRequestTypeDef

```python
# StopArchiveSearchRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import StopArchiveSearchRequestTypeDef


def get_value() -> StopArchiveSearchRequestTypeDef:
    return {
        "SearchId": ...,
    }


# StopArchiveSearchRequestTypeDef definition

class StopArchiveSearchRequestTypeDef(TypedDict):
    SearchId: str,
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## ListMembersOfAddressListRequestTypeDef

```python
# ListMembersOfAddressListRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListMembersOfAddressListRequestTypeDef


def get_value() -> ListMembersOfAddressListRequestTypeDef:
    return {
        "AddressListId": ...,
    }


# ListMembersOfAddressListRequestTypeDef definition

class ListMembersOfAddressListRequestTypeDef(TypedDict):
    AddressListId: str,
    Filter: NotRequired[AddressFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

1. See [:material-code-braces: AddressFilterTypeDef](./type_defs.md#addressfiltertypedef) 
## RuleVerdictToEvaluateTypeDef

```python
# RuleVerdictToEvaluateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleVerdictToEvaluateTypeDef


def get_value() -> RuleVerdictToEvaluateTypeDef:
    return {
        "Analysis": ...,
    }


# RuleVerdictToEvaluateTypeDef definition

class RuleVerdictToEvaluateTypeDef(TypedDict):
    Analysis: NotRequired[AnalysisTypeDef],  # (1)
    Attribute: NotRequired[RuleVerdictAttributeType],  # (2)
```

1. See [:material-code-braces: AnalysisTypeDef](./type_defs.md#analysistypedef) 
2. See [:material-code-brackets: RuleVerdictAttributeType](./literals.md#ruleverdictattributetype) 
## ArchiveBooleanExpressionTypeDef

```python
# ArchiveBooleanExpressionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ArchiveBooleanExpressionTypeDef


def get_value() -> ArchiveBooleanExpressionTypeDef:
    return {
        "Evaluate": ...,
    }


# ArchiveBooleanExpressionTypeDef definition

class ArchiveBooleanExpressionTypeDef(TypedDict):
    Evaluate: ArchiveBooleanToEvaluateTypeDef,  # (1)
    Operator: ArchiveBooleanOperatorType,  # (2)
```

1. See [:material-code-braces: ArchiveBooleanToEvaluateTypeDef](./type_defs.md#archivebooleantoevaluatetypedef) 
2. See [:material-code-brackets: ArchiveBooleanOperatorType](./literals.md#archivebooleanoperatortype) 
## UpdateArchiveRequestTypeDef

```python
# UpdateArchiveRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import UpdateArchiveRequestTypeDef


def get_value() -> UpdateArchiveRequestTypeDef:
    return {
        "ArchiveId": ...,
    }


# UpdateArchiveRequestTypeDef definition

class UpdateArchiveRequestTypeDef(TypedDict):
    ArchiveId: str,
    ArchiveName: NotRequired[str],
    Retention: NotRequired[ArchiveRetentionTypeDef],  # (1)
```

1. See [:material-code-braces: ArchiveRetentionTypeDef](./type_defs.md#archiveretentiontypedef) 
## ArchiveStringExpressionOutputTypeDef

```python
# ArchiveStringExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ArchiveStringExpressionOutputTypeDef


def get_value() -> ArchiveStringExpressionOutputTypeDef:
    return {
        "Evaluate": ...,
    }


# ArchiveStringExpressionOutputTypeDef definition

class ArchiveStringExpressionOutputTypeDef(TypedDict):
    Evaluate: ArchiveStringToEvaluateTypeDef,  # (1)
    Operator: ArchiveStringOperatorType,  # (2)
    Values: List[str],
```

1. See [:material-code-braces: ArchiveStringToEvaluateTypeDef](./type_defs.md#archivestringtoevaluatetypedef) 
2. See [:material-code-brackets: ArchiveStringOperatorType](./literals.md#archivestringoperatortype) 
## ArchiveStringExpressionTypeDef

```python
# ArchiveStringExpressionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ArchiveStringExpressionTypeDef


def get_value() -> ArchiveStringExpressionTypeDef:
    return {
        "Evaluate": ...,
    }


# ArchiveStringExpressionTypeDef definition

class ArchiveStringExpressionTypeDef(TypedDict):
    Evaluate: ArchiveStringToEvaluateTypeDef,  # (1)
    Operator: ArchiveStringOperatorType,  # (2)
    Values: Sequence[str],
```

1. See [:material-code-braces: ArchiveStringToEvaluateTypeDef](./type_defs.md#archivestringtoevaluatetypedef) 
2. See [:material-code-brackets: ArchiveStringOperatorType](./literals.md#archivestringoperatortype) 
## CreateAddonInstanceRequestTypeDef

```python
# CreateAddonInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateAddonInstanceRequestTypeDef


def get_value() -> CreateAddonInstanceRequestTypeDef:
    return {
        "AddonSubscriptionId": ...,
    }


# CreateAddonInstanceRequestTypeDef definition

class CreateAddonInstanceRequestTypeDef(TypedDict):
    AddonSubscriptionId: str,
    ClientToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAddonSubscriptionRequestTypeDef

```python
# CreateAddonSubscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateAddonSubscriptionRequestTypeDef


def get_value() -> CreateAddonSubscriptionRequestTypeDef:
    return {
        "AddonName": ...,
    }


# CreateAddonSubscriptionRequestTypeDef definition

class CreateAddonSubscriptionRequestTypeDef(TypedDict):
    AddonName: str,
    ClientToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAddressListRequestTypeDef

```python
# CreateAddressListRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateAddressListRequestTypeDef


def get_value() -> CreateAddressListRequestTypeDef:
    return {
        "AddressListName": ...,
    }


# CreateAddressListRequestTypeDef definition

class CreateAddressListRequestTypeDef(TypedDict):
    AddressListName: str,
    ClientToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateArchiveRequestTypeDef

```python
# CreateArchiveRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateArchiveRequestTypeDef


def get_value() -> CreateArchiveRequestTypeDef:
    return {
        "ArchiveName": ...,
    }


# CreateArchiveRequestTypeDef definition

class CreateArchiveRequestTypeDef(TypedDict):
    ArchiveName: str,
    ClientToken: NotRequired[str],
    KmsKeyArn: NotRequired[str],
    Retention: NotRequired[ArchiveRetentionTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ArchiveRetentionTypeDef](./type_defs.md#archiveretentiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAddonInstanceResponseTypeDef

```python
# CreateAddonInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateAddonInstanceResponseTypeDef


def get_value() -> CreateAddonInstanceResponseTypeDef:
    return {
        "AddonInstanceId": ...,
    }


# CreateAddonInstanceResponseTypeDef definition

class CreateAddonInstanceResponseTypeDef(TypedDict):
    AddonInstanceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAddonSubscriptionResponseTypeDef

```python
# CreateAddonSubscriptionResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateAddonSubscriptionResponseTypeDef


def get_value() -> CreateAddonSubscriptionResponseTypeDef:
    return {
        "AddonSubscriptionId": ...,
    }


# CreateAddonSubscriptionResponseTypeDef definition

class CreateAddonSubscriptionResponseTypeDef(TypedDict):
    AddonSubscriptionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAddressListImportJobResponseTypeDef

```python
# CreateAddressListImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateAddressListImportJobResponseTypeDef


def get_value() -> CreateAddressListImportJobResponseTypeDef:
    return {
        "JobId": ...,
    }


# CreateAddressListImportJobResponseTypeDef definition

class CreateAddressListImportJobResponseTypeDef(TypedDict):
    JobId: str,
    PreSignedUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAddressListResponseTypeDef

```python
# CreateAddressListResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateAddressListResponseTypeDef


def get_value() -> CreateAddressListResponseTypeDef:
    return {
        "AddressListId": ...,
    }


# CreateAddressListResponseTypeDef definition

class CreateAddressListResponseTypeDef(TypedDict):
    AddressListId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateArchiveResponseTypeDef

```python
# CreateArchiveResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateArchiveResponseTypeDef


def get_value() -> CreateArchiveResponseTypeDef:
    return {
        "ArchiveId": ...,
    }


# CreateArchiveResponseTypeDef definition

class CreateArchiveResponseTypeDef(TypedDict):
    ArchiveId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIngressPointResponseTypeDef

```python
# CreateIngressPointResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateIngressPointResponseTypeDef


def get_value() -> CreateIngressPointResponseTypeDef:
    return {
        "IngressPointId": ...,
    }


# CreateIngressPointResponseTypeDef definition

class CreateIngressPointResponseTypeDef(TypedDict):
    IngressPointId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRelayResponseTypeDef

```python
# CreateRelayResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateRelayResponseTypeDef


def get_value() -> CreateRelayResponseTypeDef:
    return {
        "RelayId": ...,
    }


# CreateRelayResponseTypeDef definition

class CreateRelayResponseTypeDef(TypedDict):
    RelayId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleSetResponseTypeDef

```python
# CreateRuleSetResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateRuleSetResponseTypeDef


def get_value() -> CreateRuleSetResponseTypeDef:
    return {
        "RuleSetId": ...,
    }


# CreateRuleSetResponseTypeDef definition

class CreateRuleSetResponseTypeDef(TypedDict):
    RuleSetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrafficPolicyResponseTypeDef

```python
# CreateTrafficPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateTrafficPolicyResponseTypeDef


def get_value() -> CreateTrafficPolicyResponseTypeDef:
    return {
        "TrafficPolicyId": ...,
    }


# CreateTrafficPolicyResponseTypeDef definition

class CreateTrafficPolicyResponseTypeDef(TypedDict):
    TrafficPolicyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAddonInstanceResponseTypeDef

```python
# GetAddonInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetAddonInstanceResponseTypeDef


def get_value() -> GetAddonInstanceResponseTypeDef:
    return {
        "AddonInstanceArn": ...,
    }


# GetAddonInstanceResponseTypeDef definition

class GetAddonInstanceResponseTypeDef(TypedDict):
    AddonInstanceArn: str,
    AddonName: str,
    AddonSubscriptionId: str,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAddonSubscriptionResponseTypeDef

```python
# GetAddonSubscriptionResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetAddonSubscriptionResponseTypeDef


def get_value() -> GetAddonSubscriptionResponseTypeDef:
    return {
        "AddonName": ...,
    }


# GetAddonSubscriptionResponseTypeDef definition

class GetAddonSubscriptionResponseTypeDef(TypedDict):
    AddonName: str,
    AddonSubscriptionArn: str,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAddressListResponseTypeDef

```python
# GetAddressListResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetAddressListResponseTypeDef


def get_value() -> GetAddressListResponseTypeDef:
    return {
        "AddressListArn": ...,
    }


# GetAddressListResponseTypeDef definition

class GetAddressListResponseTypeDef(TypedDict):
    AddressListArn: str,
    AddressListId: str,
    AddressListName: str,
    CreatedTimestamp: datetime,
    LastUpdatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetArchiveResponseTypeDef

```python
# GetArchiveResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetArchiveResponseTypeDef


def get_value() -> GetArchiveResponseTypeDef:
    return {
        "ArchiveArn": ...,
    }


# GetArchiveResponseTypeDef definition

class GetArchiveResponseTypeDef(TypedDict):
    ArchiveArn: str,
    ArchiveId: str,
    ArchiveName: str,
    ArchiveState: ArchiveStateType,  # (1)
    CreatedTimestamp: datetime,
    KmsKeyArn: str,
    LastUpdatedTimestamp: datetime,
    Retention: ArchiveRetentionTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ArchiveStateType](./literals.md#archivestatetype) 
2. See [:material-code-braces: ArchiveRetentionTypeDef](./type_defs.md#archiveretentiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMemberOfAddressListResponseTypeDef

```python
# GetMemberOfAddressListResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetMemberOfAddressListResponseTypeDef


def get_value() -> GetMemberOfAddressListResponseTypeDef:
    return {
        "Address": ...,
    }


# GetMemberOfAddressListResponseTypeDef definition

class GetMemberOfAddressListResponseTypeDef(TypedDict):
    Address: str,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAddonInstancesResponseTypeDef

```python
# ListAddonInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListAddonInstancesResponseTypeDef


def get_value() -> ListAddonInstancesResponseTypeDef:
    return {
        "AddonInstances": ...,
    }


# ListAddonInstancesResponseTypeDef definition

class ListAddonInstancesResponseTypeDef(TypedDict):
    AddonInstances: List[AddonInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AddonInstanceTypeDef](./type_defs.md#addoninstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAddonSubscriptionsResponseTypeDef

```python
# ListAddonSubscriptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListAddonSubscriptionsResponseTypeDef


def get_value() -> ListAddonSubscriptionsResponseTypeDef:
    return {
        "AddonSubscriptions": ...,
    }


# ListAddonSubscriptionsResponseTypeDef definition

class ListAddonSubscriptionsResponseTypeDef(TypedDict):
    AddonSubscriptions: List[AddonSubscriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AddonSubscriptionTypeDef](./type_defs.md#addonsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAddressListsResponseTypeDef

```python
# ListAddressListsResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListAddressListsResponseTypeDef


def get_value() -> ListAddressListsResponseTypeDef:
    return {
        "AddressLists": ...,
    }


# ListAddressListsResponseTypeDef definition

class ListAddressListsResponseTypeDef(TypedDict):
    AddressLists: List[AddressListTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AddressListTypeDef](./type_defs.md#addresslisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListArchivesResponseTypeDef

```python
# ListArchivesResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListArchivesResponseTypeDef


def get_value() -> ListArchivesResponseTypeDef:
    return {
        "Archives": ...,
    }


# ListArchivesResponseTypeDef definition

class ListArchivesResponseTypeDef(TypedDict):
    Archives: List[ArchiveTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ArchiveTypeDef](./type_defs.md#archivetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartArchiveExportResponseTypeDef

```python
# StartArchiveExportResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import StartArchiveExportResponseTypeDef


def get_value() -> StartArchiveExportResponseTypeDef:
    return {
        "ExportId": ...,
    }


# StartArchiveExportResponseTypeDef definition

class StartArchiveExportResponseTypeDef(TypedDict):
    ExportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartArchiveSearchResponseTypeDef

```python
# StartArchiveSearchResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import StartArchiveSearchResponseTypeDef


def get_value() -> StartArchiveSearchResponseTypeDef:
    return {
        "SearchId": ...,
    }


# StartArchiveSearchResponseTypeDef definition

class StartArchiveSearchResponseTypeDef(TypedDict):
    SearchId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAddressListImportJobRequestTypeDef

```python
# CreateAddressListImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateAddressListImportJobRequestTypeDef


def get_value() -> CreateAddressListImportJobRequestTypeDef:
    return {
        "AddressListId": ...,
    }


# CreateAddressListImportJobRequestTypeDef definition

class CreateAddressListImportJobRequestTypeDef(TypedDict):
    AddressListId: str,
    ImportDataFormat: ImportDataFormatTypeDef,  # (1)
    Name: str,
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: ImportDataFormatTypeDef](./type_defs.md#importdataformattypedef) 
## GetAddressListImportJobResponseTypeDef

```python
# GetAddressListImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetAddressListImportJobResponseTypeDef


def get_value() -> GetAddressListImportJobResponseTypeDef:
    return {
        "AddressListId": ...,
    }


# GetAddressListImportJobResponseTypeDef definition

class GetAddressListImportJobResponseTypeDef(TypedDict):
    AddressListId: str,
    CompletedTimestamp: datetime,
    CreatedTimestamp: datetime,
    Error: str,
    FailedItemsCount: int,
    ImportDataFormat: ImportDataFormatTypeDef,  # (1)
    ImportedItemsCount: int,
    JobId: str,
    Name: str,
    PreSignedUrl: str,
    StartTimestamp: datetime,
    Status: ImportJobStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ImportDataFormatTypeDef](./type_defs.md#importdataformattypedef) 
2. See [:material-code-brackets: ImportJobStatusType](./literals.md#importjobstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportJobTypeDef

```python
# ImportJobTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ImportJobTypeDef


def get_value() -> ImportJobTypeDef:
    return {
        "AddressListId": ...,
    }


# ImportJobTypeDef definition

class ImportJobTypeDef(TypedDict):
    AddressListId: str,
    CreatedTimestamp: datetime,
    ImportDataFormat: ImportDataFormatTypeDef,  # (1)
    JobId: str,
    Name: str,
    PreSignedUrl: str,
    Status: ImportJobStatusType,  # (2)
    CompletedTimestamp: NotRequired[datetime],
    Error: NotRequired[str],
    FailedItemsCount: NotRequired[int],
    ImportedItemsCount: NotRequired[int],
    StartTimestamp: NotRequired[datetime],
```

1. See [:material-code-braces: ImportDataFormatTypeDef](./type_defs.md#importdataformattypedef) 
2. See [:material-code-brackets: ImportJobStatusType](./literals.md#importjobstatustype) 
## CreateIngressPointRequestTypeDef

```python
# CreateIngressPointRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateIngressPointRequestTypeDef


def get_value() -> CreateIngressPointRequestTypeDef:
    return {
        "IngressPointName": ...,
    }


# CreateIngressPointRequestTypeDef definition

class CreateIngressPointRequestTypeDef(TypedDict):
    IngressPointName: str,
    RuleSetId: str,
    TrafficPolicyId: str,
    Type: IngressPointTypeType,  # (1)
    ClientToken: NotRequired[str],
    IngressPointConfiguration: NotRequired[IngressPointConfigurationTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: IngressPointTypeType](./literals.md#ingresspointtypetype) 
2. See [:material-code-braces: IngressPointConfigurationTypeDef](./type_defs.md#ingresspointconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateIngressPointRequestTypeDef

```python
# UpdateIngressPointRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import UpdateIngressPointRequestTypeDef


def get_value() -> UpdateIngressPointRequestTypeDef:
    return {
        "IngressPointId": ...,
    }


# UpdateIngressPointRequestTypeDef definition

class UpdateIngressPointRequestTypeDef(TypedDict):
    IngressPointId: str,
    IngressPointConfiguration: NotRequired[IngressPointConfigurationTypeDef],  # (1)
    IngressPointName: NotRequired[str],
    RuleSetId: NotRequired[str],
    StatusToUpdate: NotRequired[IngressPointStatusToUpdateType],  # (2)
    TrafficPolicyId: NotRequired[str],
```

1. See [:material-code-braces: IngressPointConfigurationTypeDef](./type_defs.md#ingresspointconfigurationtypedef) 
2. See [:material-code-brackets: IngressPointStatusToUpdateType](./literals.md#ingresspointstatustoupdatetype) 
## RowTypeDef

```python
# RowTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RowTypeDef


def get_value() -> RowTypeDef:
    return {
        "ArchivedMessageId": ...,
    }


# RowTypeDef definition

class RowTypeDef(TypedDict):
    ArchivedMessageId: NotRequired[str],
    Cc: NotRequired[str],
    Date: NotRequired[str],
    Envelope: NotRequired[EnvelopeTypeDef],  # (1)
    From: NotRequired[str],
    HasAttachments: NotRequired[bool],
    InReplyTo: NotRequired[str],
    IngressPointId: NotRequired[str],
    MessageId: NotRequired[str],
    ReceivedHeaders: NotRequired[List[str]],
    ReceivedTimestamp: NotRequired[datetime],
    SenderHostname: NotRequired[str],
    SenderIpAddress: NotRequired[str],
    SourceArn: NotRequired[str],
    Subject: NotRequired[str],
    To: NotRequired[str],
    XMailer: NotRequired[str],
    XOriginalMailer: NotRequired[str],
    XPriority: NotRequired[str],
```

1. See [:material-code-braces: EnvelopeTypeDef](./type_defs.md#envelopetypedef) 
## ExportDestinationConfigurationTypeDef

```python
# ExportDestinationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ExportDestinationConfigurationTypeDef


def get_value() -> ExportDestinationConfigurationTypeDef:
    return {
        "S3": ...,
    }


# ExportDestinationConfigurationTypeDef definition

class ExportDestinationConfigurationTypeDef(TypedDict):
    S3: NotRequired[S3ExportDestinationConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: S3ExportDestinationConfigurationTypeDef](./type_defs.md#s3exportdestinationconfigurationtypedef) 
## ExportSummaryTypeDef

```python
# ExportSummaryTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ExportSummaryTypeDef


def get_value() -> ExportSummaryTypeDef:
    return {
        "ExportId": ...,
    }


# ExportSummaryTypeDef definition

class ExportSummaryTypeDef(TypedDict):
    ExportId: NotRequired[str],
    Status: NotRequired[ExportStatusTypeDef],  # (1)
```

1. See [:material-code-braces: ExportStatusTypeDef](./type_defs.md#exportstatustypedef) 
## GetArchiveMessageContentResponseTypeDef

```python
# GetArchiveMessageContentResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetArchiveMessageContentResponseTypeDef


def get_value() -> GetArchiveMessageContentResponseTypeDef:
    return {
        "Body": ...,
    }


# GetArchiveMessageContentResponseTypeDef definition

class GetArchiveMessageContentResponseTypeDef(TypedDict):
    Body: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetArchiveMessageResponseTypeDef

```python
# GetArchiveMessageResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetArchiveMessageResponseTypeDef


def get_value() -> GetArchiveMessageResponseTypeDef:
    return {
        "Envelope": ...,
    }


# GetArchiveMessageResponseTypeDef definition

class GetArchiveMessageResponseTypeDef(TypedDict):
    Envelope: EnvelopeTypeDef,  # (1)
    MessageDownloadLink: str,
    Metadata: MetadataTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EnvelopeTypeDef](./type_defs.md#envelopetypedef) 
2. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchSummaryTypeDef

```python
# SearchSummaryTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import SearchSummaryTypeDef


def get_value() -> SearchSummaryTypeDef:
    return {
        "SearchId": ...,
    }


# SearchSummaryTypeDef definition

class SearchSummaryTypeDef(TypedDict):
    SearchId: NotRequired[str],
    Status: NotRequired[SearchStatusTypeDef],  # (1)
```

1. See [:material-code-braces: SearchStatusTypeDef](./type_defs.md#searchstatustypedef) 
## GetRelayResponseTypeDef

```python
# GetRelayResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetRelayResponseTypeDef


def get_value() -> GetRelayResponseTypeDef:
    return {
        "Authentication": ...,
    }


# GetRelayResponseTypeDef definition

class GetRelayResponseTypeDef(TypedDict):
    Authentication: RelayAuthenticationOutputTypeDef,  # (1)
    CreatedTimestamp: datetime,
    LastModifiedTimestamp: datetime,
    RelayArn: str,
    RelayId: str,
    RelayName: str,
    ServerName: str,
    ServerPort: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RelayAuthenticationOutputTypeDef](./type_defs.md#relayauthenticationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IngressBooleanToEvaluateOutputTypeDef

```python
# IngressBooleanToEvaluateOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressBooleanToEvaluateOutputTypeDef


def get_value() -> IngressBooleanToEvaluateOutputTypeDef:
    return {
        "Analysis": ...,
    }


# IngressBooleanToEvaluateOutputTypeDef definition

class IngressBooleanToEvaluateOutputTypeDef(TypedDict):
    Analysis: NotRequired[IngressAnalysisTypeDef],  # (1)
    IsInAddressList: NotRequired[IngressIsInAddressListOutputTypeDef],  # (2)
```

1. See [:material-code-braces: IngressAnalysisTypeDef](./type_defs.md#ingressanalysistypedef) 
2. See [:material-code-braces: IngressIsInAddressListOutputTypeDef](./type_defs.md#ingressisinaddresslistoutputtypedef) 
## IngressIpv4ExpressionOutputTypeDef

```python
# IngressIpv4ExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressIpv4ExpressionOutputTypeDef


def get_value() -> IngressIpv4ExpressionOutputTypeDef:
    return {
        "Evaluate": ...,
    }


# IngressIpv4ExpressionOutputTypeDef definition

class IngressIpv4ExpressionOutputTypeDef(TypedDict):
    Evaluate: IngressIpToEvaluateTypeDef,  # (1)
    Operator: IngressIpOperatorType,  # (2)
    Values: List[str],
```

1. See [:material-code-braces: IngressIpToEvaluateTypeDef](./type_defs.md#ingressiptoevaluatetypedef) 
2. See [:material-code-brackets: IngressIpOperatorType](./literals.md#ingressipoperatortype) 
## IngressIpv4ExpressionTypeDef

```python
# IngressIpv4ExpressionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressIpv4ExpressionTypeDef


def get_value() -> IngressIpv4ExpressionTypeDef:
    return {
        "Evaluate": ...,
    }


# IngressIpv4ExpressionTypeDef definition

class IngressIpv4ExpressionTypeDef(TypedDict):
    Evaluate: IngressIpToEvaluateTypeDef,  # (1)
    Operator: IngressIpOperatorType,  # (2)
    Values: Sequence[str],
```

1. See [:material-code-braces: IngressIpToEvaluateTypeDef](./type_defs.md#ingressiptoevaluatetypedef) 
2. See [:material-code-brackets: IngressIpOperatorType](./literals.md#ingressipoperatortype) 
## IngressPointAuthConfigurationTypeDef

```python
# IngressPointAuthConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressPointAuthConfigurationTypeDef


def get_value() -> IngressPointAuthConfigurationTypeDef:
    return {
        "IngressPointPasswordConfiguration": ...,
    }


# IngressPointAuthConfigurationTypeDef definition

class IngressPointAuthConfigurationTypeDef(TypedDict):
    IngressPointPasswordConfiguration: NotRequired[IngressPointPasswordConfigurationTypeDef],  # (1)
    SecretArn: NotRequired[str],
```

1. See [:material-code-braces: IngressPointPasswordConfigurationTypeDef](./type_defs.md#ingresspointpasswordconfigurationtypedef) 
## ListIngressPointsResponseTypeDef

```python
# ListIngressPointsResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListIngressPointsResponseTypeDef


def get_value() -> ListIngressPointsResponseTypeDef:
    return {
        "IngressPoints": ...,
    }


# ListIngressPointsResponseTypeDef definition

class ListIngressPointsResponseTypeDef(TypedDict):
    IngressPoints: List[IngressPointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IngressPointTypeDef](./type_defs.md#ingresspointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IngressStringExpressionOutputTypeDef

```python
# IngressStringExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressStringExpressionOutputTypeDef


def get_value() -> IngressStringExpressionOutputTypeDef:
    return {
        "Evaluate": ...,
    }


# IngressStringExpressionOutputTypeDef definition

class IngressStringExpressionOutputTypeDef(TypedDict):
    Evaluate: IngressStringToEvaluateTypeDef,  # (1)
    Operator: IngressStringOperatorType,  # (2)
    Values: List[str],
```

1. See [:material-code-braces: IngressStringToEvaluateTypeDef](./type_defs.md#ingressstringtoevaluatetypedef) 
2. See [:material-code-brackets: IngressStringOperatorType](./literals.md#ingressstringoperatortype) 
## IngressStringExpressionTypeDef

```python
# IngressStringExpressionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressStringExpressionTypeDef


def get_value() -> IngressStringExpressionTypeDef:
    return {
        "Evaluate": ...,
    }


# IngressStringExpressionTypeDef definition

class IngressStringExpressionTypeDef(TypedDict):
    Evaluate: IngressStringToEvaluateTypeDef,  # (1)
    Operator: IngressStringOperatorType,  # (2)
    Values: Sequence[str],
```

1. See [:material-code-braces: IngressStringToEvaluateTypeDef](./type_defs.md#ingressstringtoevaluatetypedef) 
2. See [:material-code-brackets: IngressStringOperatorType](./literals.md#ingressstringoperatortype) 
## IngressTlsProtocolExpressionTypeDef

```python
# IngressTlsProtocolExpressionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressTlsProtocolExpressionTypeDef


def get_value() -> IngressTlsProtocolExpressionTypeDef:
    return {
        "Evaluate": ...,
    }


# IngressTlsProtocolExpressionTypeDef definition

class IngressTlsProtocolExpressionTypeDef(TypedDict):
    Evaluate: IngressTlsProtocolToEvaluateTypeDef,  # (1)
    Operator: IngressTlsProtocolOperatorType,  # (2)
    Value: IngressTlsProtocolAttributeType,  # (3)
```

1. See [:material-code-braces: IngressTlsProtocolToEvaluateTypeDef](./type_defs.md#ingresstlsprotocoltoevaluatetypedef) 
2. See [:material-code-brackets: IngressTlsProtocolOperatorType](./literals.md#ingresstlsprotocoloperatortype) 
3. See [:material-code-brackets: IngressTlsProtocolAttributeType](./literals.md#ingresstlsprotocolattributetype) 
## ListAddonInstancesRequestPaginateTypeDef

```python
# ListAddonInstancesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListAddonInstancesRequestPaginateTypeDef


def get_value() -> ListAddonInstancesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListAddonInstancesRequestPaginateTypeDef definition

class ListAddonInstancesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAddonSubscriptionsRequestPaginateTypeDef

```python
# ListAddonSubscriptionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListAddonSubscriptionsRequestPaginateTypeDef


def get_value() -> ListAddonSubscriptionsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListAddonSubscriptionsRequestPaginateTypeDef definition

class ListAddonSubscriptionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAddressListImportJobsRequestPaginateTypeDef

```python
# ListAddressListImportJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListAddressListImportJobsRequestPaginateTypeDef


def get_value() -> ListAddressListImportJobsRequestPaginateTypeDef:
    return {
        "AddressListId": ...,
    }


# ListAddressListImportJobsRequestPaginateTypeDef definition

class ListAddressListImportJobsRequestPaginateTypeDef(TypedDict):
    AddressListId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAddressListsRequestPaginateTypeDef

```python
# ListAddressListsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListAddressListsRequestPaginateTypeDef


def get_value() -> ListAddressListsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListAddressListsRequestPaginateTypeDef definition

class ListAddressListsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListArchiveExportsRequestPaginateTypeDef

```python
# ListArchiveExportsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListArchiveExportsRequestPaginateTypeDef


def get_value() -> ListArchiveExportsRequestPaginateTypeDef:
    return {
        "ArchiveId": ...,
    }


# ListArchiveExportsRequestPaginateTypeDef definition

class ListArchiveExportsRequestPaginateTypeDef(TypedDict):
    ArchiveId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListArchiveSearchesRequestPaginateTypeDef

```python
# ListArchiveSearchesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListArchiveSearchesRequestPaginateTypeDef


def get_value() -> ListArchiveSearchesRequestPaginateTypeDef:
    return {
        "ArchiveId": ...,
    }


# ListArchiveSearchesRequestPaginateTypeDef definition

class ListArchiveSearchesRequestPaginateTypeDef(TypedDict):
    ArchiveId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListArchivesRequestPaginateTypeDef

```python
# ListArchivesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListArchivesRequestPaginateTypeDef


def get_value() -> ListArchivesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListArchivesRequestPaginateTypeDef definition

class ListArchivesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIngressPointsRequestPaginateTypeDef

```python
# ListIngressPointsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListIngressPointsRequestPaginateTypeDef


def get_value() -> ListIngressPointsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListIngressPointsRequestPaginateTypeDef definition

class ListIngressPointsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembersOfAddressListRequestPaginateTypeDef

```python
# ListMembersOfAddressListRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListMembersOfAddressListRequestPaginateTypeDef


def get_value() -> ListMembersOfAddressListRequestPaginateTypeDef:
    return {
        "AddressListId": ...,
    }


# ListMembersOfAddressListRequestPaginateTypeDef definition

class ListMembersOfAddressListRequestPaginateTypeDef(TypedDict):
    AddressListId: str,
    Filter: NotRequired[AddressFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AddressFilterTypeDef](./type_defs.md#addressfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRelaysRequestPaginateTypeDef

```python
# ListRelaysRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListRelaysRequestPaginateTypeDef


def get_value() -> ListRelaysRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListRelaysRequestPaginateTypeDef definition

class ListRelaysRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRuleSetsRequestPaginateTypeDef

```python
# ListRuleSetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListRuleSetsRequestPaginateTypeDef


def get_value() -> ListRuleSetsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListRuleSetsRequestPaginateTypeDef definition

class ListRuleSetsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrafficPoliciesRequestPaginateTypeDef

```python
# ListTrafficPoliciesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListTrafficPoliciesRequestPaginateTypeDef


def get_value() -> ListTrafficPoliciesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListTrafficPoliciesRequestPaginateTypeDef definition

class ListTrafficPoliciesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembersOfAddressListResponseTypeDef

```python
# ListMembersOfAddressListResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListMembersOfAddressListResponseTypeDef


def get_value() -> ListMembersOfAddressListResponseTypeDef:
    return {
        "Addresses": ...,
    }


# ListMembersOfAddressListResponseTypeDef definition

class ListMembersOfAddressListResponseTypeDef(TypedDict):
    Addresses: List[SavedAddressTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SavedAddressTypeDef](./type_defs.md#savedaddresstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRelaysResponseTypeDef

```python
# ListRelaysResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListRelaysResponseTypeDef


def get_value() -> ListRelaysResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListRelaysResponseTypeDef definition

class ListRelaysResponseTypeDef(TypedDict):
    Relays: List[RelayTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RelayTypeDef](./type_defs.md#relaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRuleSetsResponseTypeDef

```python
# ListRuleSetsResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListRuleSetsResponseTypeDef


def get_value() -> ListRuleSetsResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListRuleSetsResponseTypeDef definition

class ListRuleSetsResponseTypeDef(TypedDict):
    RuleSets: List[RuleSetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RuleSetTypeDef](./type_defs.md#rulesettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrafficPoliciesResponseTypeDef

```python
# ListTrafficPoliciesResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListTrafficPoliciesResponseTypeDef


def get_value() -> ListTrafficPoliciesResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListTrafficPoliciesResponseTypeDef definition

class ListTrafficPoliciesResponseTypeDef(TypedDict):
    TrafficPolicies: List[TrafficPolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TrafficPolicyTypeDef](./type_defs.md#trafficpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleActionOutputTypeDef

```python
# RuleActionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleActionOutputTypeDef


def get_value() -> RuleActionOutputTypeDef:
    return {
        "AddHeader": ...,
    }


# RuleActionOutputTypeDef definition

class RuleActionOutputTypeDef(TypedDict):
    AddHeader: NotRequired[AddHeaderActionTypeDef],  # (1)
    Archive: NotRequired[ArchiveActionTypeDef],  # (2)
    DeliverToMailbox: NotRequired[DeliverToMailboxActionTypeDef],  # (3)
    DeliverToQBusiness: NotRequired[DeliverToQBusinessActionTypeDef],  # (4)
    Drop: NotRequired[Dict[str, Any]],
    Relay: NotRequired[RelayActionTypeDef],  # (5)
    ReplaceRecipient: NotRequired[ReplaceRecipientActionOutputTypeDef],  # (6)
    Send: NotRequired[SendActionTypeDef],  # (7)
    WriteToS3: NotRequired[S3ActionTypeDef],  # (8)
```

1. See [:material-code-braces: AddHeaderActionTypeDef](./type_defs.md#addheaderactiontypedef) 
2. See [:material-code-braces: ArchiveActionTypeDef](./type_defs.md#archiveactiontypedef) 
3. See [:material-code-braces: DeliverToMailboxActionTypeDef](./type_defs.md#delivertomailboxactiontypedef) 
4. See [:material-code-braces: DeliverToQBusinessActionTypeDef](./type_defs.md#delivertoqbusinessactiontypedef) 
5. See [:material-code-braces: RelayActionTypeDef](./type_defs.md#relayactiontypedef) 
6. See [:material-code-braces: ReplaceRecipientActionOutputTypeDef](./type_defs.md#replacerecipientactionoutputtypedef) 
7. See [:material-code-braces: SendActionTypeDef](./type_defs.md#sendactiontypedef) 
8. See [:material-code-braces: S3ActionTypeDef](./type_defs.md#s3actiontypedef) 
## RuleBooleanToEvaluateOutputTypeDef

```python
# RuleBooleanToEvaluateOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleBooleanToEvaluateOutputTypeDef


def get_value() -> RuleBooleanToEvaluateOutputTypeDef:
    return {
        "Attribute": ...,
    }


# RuleBooleanToEvaluateOutputTypeDef definition

class RuleBooleanToEvaluateOutputTypeDef(TypedDict):
    Attribute: NotRequired[RuleBooleanEmailAttributeType],  # (1)
    IsInAddressList: NotRequired[RuleIsInAddressListOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: RuleBooleanEmailAttributeType](./literals.md#rulebooleanemailattributetype) 
2. See [:material-code-braces: RuleIsInAddressListOutputTypeDef](./type_defs.md#ruleisinaddresslistoutputtypedef) 
## RuleIpExpressionOutputTypeDef

```python
# RuleIpExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleIpExpressionOutputTypeDef


def get_value() -> RuleIpExpressionOutputTypeDef:
    return {
        "Evaluate": ...,
    }


# RuleIpExpressionOutputTypeDef definition

class RuleIpExpressionOutputTypeDef(TypedDict):
    Evaluate: RuleIpToEvaluateTypeDef,  # (1)
    Operator: RuleIpOperatorType,  # (2)
    Values: List[str],
```

1. See [:material-code-braces: RuleIpToEvaluateTypeDef](./type_defs.md#ruleiptoevaluatetypedef) 
2. See [:material-code-brackets: RuleIpOperatorType](./literals.md#ruleipoperatortype) 
## RuleIpExpressionTypeDef

```python
# RuleIpExpressionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleIpExpressionTypeDef


def get_value() -> RuleIpExpressionTypeDef:
    return {
        "Evaluate": ...,
    }


# RuleIpExpressionTypeDef definition

class RuleIpExpressionTypeDef(TypedDict):
    Evaluate: RuleIpToEvaluateTypeDef,  # (1)
    Operator: RuleIpOperatorType,  # (2)
    Values: Sequence[str],
```

1. See [:material-code-braces: RuleIpToEvaluateTypeDef](./type_defs.md#ruleiptoevaluatetypedef) 
2. See [:material-code-brackets: RuleIpOperatorType](./literals.md#ruleipoperatortype) 
## RuleNumberExpressionTypeDef

```python
# RuleNumberExpressionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleNumberExpressionTypeDef


def get_value() -> RuleNumberExpressionTypeDef:
    return {
        "Evaluate": ...,
    }


# RuleNumberExpressionTypeDef definition

class RuleNumberExpressionTypeDef(TypedDict):
    Evaluate: RuleNumberToEvaluateTypeDef,  # (1)
    Operator: RuleNumberOperatorType,  # (2)
    Value: float,
```

1. See [:material-code-braces: RuleNumberToEvaluateTypeDef](./type_defs.md#rulenumbertoevaluatetypedef) 
2. See [:material-code-brackets: RuleNumberOperatorType](./literals.md#rulenumberoperatortype) 
## RuleStringExpressionOutputTypeDef

```python
# RuleStringExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleStringExpressionOutputTypeDef


def get_value() -> RuleStringExpressionOutputTypeDef:
    return {
        "Evaluate": ...,
    }


# RuleStringExpressionOutputTypeDef definition

class RuleStringExpressionOutputTypeDef(TypedDict):
    Evaluate: RuleStringToEvaluateTypeDef,  # (1)
    Operator: RuleStringOperatorType,  # (2)
    Values: List[str],
```

1. See [:material-code-braces: RuleStringToEvaluateTypeDef](./type_defs.md#rulestringtoevaluatetypedef) 
2. See [:material-code-brackets: RuleStringOperatorType](./literals.md#rulestringoperatortype) 
## RuleStringExpressionTypeDef

```python
# RuleStringExpressionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleStringExpressionTypeDef


def get_value() -> RuleStringExpressionTypeDef:
    return {
        "Evaluate": ...,
    }


# RuleStringExpressionTypeDef definition

class RuleStringExpressionTypeDef(TypedDict):
    Evaluate: RuleStringToEvaluateTypeDef,  # (1)
    Operator: RuleStringOperatorType,  # (2)
    Values: Sequence[str],
```

1. See [:material-code-braces: RuleStringToEvaluateTypeDef](./type_defs.md#rulestringtoevaluatetypedef) 
2. See [:material-code-brackets: RuleStringOperatorType](./literals.md#rulestringoperatortype) 
## RuleVerdictExpressionOutputTypeDef

```python
# RuleVerdictExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleVerdictExpressionOutputTypeDef


def get_value() -> RuleVerdictExpressionOutputTypeDef:
    return {
        "Evaluate": ...,
    }


# RuleVerdictExpressionOutputTypeDef definition

class RuleVerdictExpressionOutputTypeDef(TypedDict):
    Evaluate: RuleVerdictToEvaluateTypeDef,  # (1)
    Operator: RuleVerdictOperatorType,  # (2)
    Values: List[RuleVerdictType],  # (3)
```

1. See [:material-code-braces: RuleVerdictToEvaluateTypeDef](./type_defs.md#ruleverdicttoevaluatetypedef) 
2. See [:material-code-brackets: RuleVerdictOperatorType](./literals.md#ruleverdictoperatortype) 
3. See [:material-code-brackets: RuleVerdictType](./literals.md#ruleverdicttype) 
## RuleVerdictExpressionTypeDef

```python
# RuleVerdictExpressionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleVerdictExpressionTypeDef


def get_value() -> RuleVerdictExpressionTypeDef:
    return {
        "Evaluate": ...,
    }


# RuleVerdictExpressionTypeDef definition

class RuleVerdictExpressionTypeDef(TypedDict):
    Evaluate: RuleVerdictToEvaluateTypeDef,  # (1)
    Operator: RuleVerdictOperatorType,  # (2)
    Values: Sequence[RuleVerdictType],  # (3)
```

1. See [:material-code-braces: RuleVerdictToEvaluateTypeDef](./type_defs.md#ruleverdicttoevaluatetypedef) 
2. See [:material-code-brackets: RuleVerdictOperatorType](./literals.md#ruleverdictoperatortype) 
3. See [:material-code-brackets: RuleVerdictType](./literals.md#ruleverdicttype) 
## ArchiveFilterConditionOutputTypeDef

```python
# ArchiveFilterConditionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ArchiveFilterConditionOutputTypeDef


def get_value() -> ArchiveFilterConditionOutputTypeDef:
    return {
        "BooleanExpression": ...,
    }


# ArchiveFilterConditionOutputTypeDef definition

class ArchiveFilterConditionOutputTypeDef(TypedDict):
    BooleanExpression: NotRequired[ArchiveBooleanExpressionTypeDef],  # (1)
    StringExpression: NotRequired[ArchiveStringExpressionOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ArchiveBooleanExpressionTypeDef](./type_defs.md#archivebooleanexpressiontypedef) 
2. See [:material-code-braces: ArchiveStringExpressionOutputTypeDef](./type_defs.md#archivestringexpressionoutputtypedef) 
## ArchiveFilterConditionTypeDef

```python
# ArchiveFilterConditionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ArchiveFilterConditionTypeDef


def get_value() -> ArchiveFilterConditionTypeDef:
    return {
        "BooleanExpression": ...,
    }


# ArchiveFilterConditionTypeDef definition

class ArchiveFilterConditionTypeDef(TypedDict):
    BooleanExpression: NotRequired[ArchiveBooleanExpressionTypeDef],  # (1)
    StringExpression: NotRequired[ArchiveStringExpressionTypeDef],  # (2)
```

1. See [:material-code-braces: ArchiveBooleanExpressionTypeDef](./type_defs.md#archivebooleanexpressiontypedef) 
2. See [:material-code-braces: ArchiveStringExpressionTypeDef](./type_defs.md#archivestringexpressiontypedef) 
## ListAddressListImportJobsResponseTypeDef

```python
# ListAddressListImportJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListAddressListImportJobsResponseTypeDef


def get_value() -> ListAddressListImportJobsResponseTypeDef:
    return {
        "ImportJobs": ...,
    }


# ListAddressListImportJobsResponseTypeDef definition

class ListAddressListImportJobsResponseTypeDef(TypedDict):
    ImportJobs: List[ImportJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportJobTypeDef](./type_defs.md#importjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetArchiveSearchResultsResponseTypeDef

```python
# GetArchiveSearchResultsResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetArchiveSearchResultsResponseTypeDef


def get_value() -> GetArchiveSearchResultsResponseTypeDef:
    return {
        "Rows": ...,
    }


# GetArchiveSearchResultsResponseTypeDef definition

class GetArchiveSearchResultsResponseTypeDef(TypedDict):
    Rows: List[RowTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RowTypeDef](./type_defs.md#rowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListArchiveExportsResponseTypeDef

```python
# ListArchiveExportsResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListArchiveExportsResponseTypeDef


def get_value() -> ListArchiveExportsResponseTypeDef:
    return {
        "Exports": ...,
    }


# ListArchiveExportsResponseTypeDef definition

class ListArchiveExportsResponseTypeDef(TypedDict):
    Exports: List[ExportSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportSummaryTypeDef](./type_defs.md#exportsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListArchiveSearchesResponseTypeDef

```python
# ListArchiveSearchesResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ListArchiveSearchesResponseTypeDef


def get_value() -> ListArchiveSearchesResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListArchiveSearchesResponseTypeDef definition

class ListArchiveSearchesResponseTypeDef(TypedDict):
    Searches: List[SearchSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchSummaryTypeDef](./type_defs.md#searchsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IngressBooleanExpressionOutputTypeDef

```python
# IngressBooleanExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressBooleanExpressionOutputTypeDef


def get_value() -> IngressBooleanExpressionOutputTypeDef:
    return {
        "Evaluate": ...,
    }


# IngressBooleanExpressionOutputTypeDef definition

class IngressBooleanExpressionOutputTypeDef(TypedDict):
    Evaluate: IngressBooleanToEvaluateOutputTypeDef,  # (1)
    Operator: IngressBooleanOperatorType,  # (2)
```

1. See [:material-code-braces: IngressBooleanToEvaluateOutputTypeDef](./type_defs.md#ingressbooleantoevaluateoutputtypedef) 
2. See [:material-code-brackets: IngressBooleanOperatorType](./literals.md#ingressbooleanoperatortype) 
## IngressBooleanToEvaluateTypeDef

```python
# IngressBooleanToEvaluateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressBooleanToEvaluateTypeDef


def get_value() -> IngressBooleanToEvaluateTypeDef:
    return {
        "Analysis": ...,
    }


# IngressBooleanToEvaluateTypeDef definition

class IngressBooleanToEvaluateTypeDef(TypedDict):
    Analysis: NotRequired[IngressAnalysisTypeDef],  # (1)
    IsInAddressList: NotRequired[IngressIsInAddressListUnionTypeDef],  # (2)
```

1. See [:material-code-braces: IngressAnalysisTypeDef](./type_defs.md#ingressanalysistypedef) 
2. See [:material-code-braces: IngressIsInAddressListTypeDef](./type_defs.md#ingressisinaddresslisttypedef) [:material-code-braces: IngressIsInAddressListOutputTypeDef](./type_defs.md#ingressisinaddresslistoutputtypedef) 
## GetIngressPointResponseTypeDef

```python
# GetIngressPointResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetIngressPointResponseTypeDef


def get_value() -> GetIngressPointResponseTypeDef:
    return {
        "ARecord": ...,
    }


# GetIngressPointResponseTypeDef definition

class GetIngressPointResponseTypeDef(TypedDict):
    ARecord: str,
    CreatedTimestamp: datetime,
    IngressPointArn: str,
    IngressPointAuthConfiguration: IngressPointAuthConfigurationTypeDef,  # (1)
    IngressPointId: str,
    IngressPointName: str,
    LastUpdatedTimestamp: datetime,
    RuleSetId: str,
    Status: IngressPointStatusType,  # (2)
    TrafficPolicyId: str,
    Type: IngressPointTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: IngressPointAuthConfigurationTypeDef](./type_defs.md#ingresspointauthconfigurationtypedef) 
2. See [:material-code-brackets: IngressPointStatusType](./literals.md#ingresspointstatustype) 
3. See [:material-code-brackets: IngressPointTypeType](./literals.md#ingresspointtypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRelayRequestTypeDef

```python
# CreateRelayRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateRelayRequestTypeDef


def get_value() -> CreateRelayRequestTypeDef:
    return {
        "Authentication": ...,
    }


# CreateRelayRequestTypeDef definition

class CreateRelayRequestTypeDef(TypedDict):
    Authentication: RelayAuthenticationUnionTypeDef,  # (1)
    RelayName: str,
    ServerName: str,
    ServerPort: int,
    ClientToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: RelayAuthenticationTypeDef](./type_defs.md#relayauthenticationtypedef) [:material-code-braces: RelayAuthenticationOutputTypeDef](./type_defs.md#relayauthenticationoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateRelayRequestTypeDef

```python
# UpdateRelayRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import UpdateRelayRequestTypeDef


def get_value() -> UpdateRelayRequestTypeDef:
    return {
        "RelayId": ...,
    }


# UpdateRelayRequestTypeDef definition

class UpdateRelayRequestTypeDef(TypedDict):
    RelayId: str,
    Authentication: NotRequired[RelayAuthenticationUnionTypeDef],  # (1)
    RelayName: NotRequired[str],
    ServerName: NotRequired[str],
    ServerPort: NotRequired[int],
```

1. See [:material-code-braces: RelayAuthenticationTypeDef](./type_defs.md#relayauthenticationtypedef) [:material-code-braces: RelayAuthenticationOutputTypeDef](./type_defs.md#relayauthenticationoutputtypedef) 
## RuleActionTypeDef

```python
# RuleActionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleActionTypeDef


def get_value() -> RuleActionTypeDef:
    return {
        "AddHeader": ...,
    }


# RuleActionTypeDef definition

class RuleActionTypeDef(TypedDict):
    AddHeader: NotRequired[AddHeaderActionTypeDef],  # (1)
    Archive: NotRequired[ArchiveActionTypeDef],  # (2)
    DeliverToMailbox: NotRequired[DeliverToMailboxActionTypeDef],  # (3)
    DeliverToQBusiness: NotRequired[DeliverToQBusinessActionTypeDef],  # (4)
    Drop: NotRequired[Mapping[str, Any]],
    Relay: NotRequired[RelayActionTypeDef],  # (5)
    ReplaceRecipient: NotRequired[ReplaceRecipientActionUnionTypeDef],  # (6)
    Send: NotRequired[SendActionTypeDef],  # (7)
    WriteToS3: NotRequired[S3ActionTypeDef],  # (8)
```

1. See [:material-code-braces: AddHeaderActionTypeDef](./type_defs.md#addheaderactiontypedef) 
2. See [:material-code-braces: ArchiveActionTypeDef](./type_defs.md#archiveactiontypedef) 
3. See [:material-code-braces: DeliverToMailboxActionTypeDef](./type_defs.md#delivertomailboxactiontypedef) 
4. See [:material-code-braces: DeliverToQBusinessActionTypeDef](./type_defs.md#delivertoqbusinessactiontypedef) 
5. See [:material-code-braces: RelayActionTypeDef](./type_defs.md#relayactiontypedef) 
6. See [:material-code-braces: ReplaceRecipientActionTypeDef](./type_defs.md#replacerecipientactiontypedef) [:material-code-braces: ReplaceRecipientActionOutputTypeDef](./type_defs.md#replacerecipientactionoutputtypedef) 
7. See [:material-code-braces: SendActionTypeDef](./type_defs.md#sendactiontypedef) 
8. See [:material-code-braces: S3ActionTypeDef](./type_defs.md#s3actiontypedef) 
## RuleBooleanExpressionOutputTypeDef

```python
# RuleBooleanExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleBooleanExpressionOutputTypeDef


def get_value() -> RuleBooleanExpressionOutputTypeDef:
    return {
        "Evaluate": ...,
    }


# RuleBooleanExpressionOutputTypeDef definition

class RuleBooleanExpressionOutputTypeDef(TypedDict):
    Evaluate: RuleBooleanToEvaluateOutputTypeDef,  # (1)
    Operator: RuleBooleanOperatorType,  # (2)
```

1. See [:material-code-braces: RuleBooleanToEvaluateOutputTypeDef](./type_defs.md#rulebooleantoevaluateoutputtypedef) 
2. See [:material-code-brackets: RuleBooleanOperatorType](./literals.md#rulebooleanoperatortype) 
## RuleBooleanToEvaluateTypeDef

```python
# RuleBooleanToEvaluateTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleBooleanToEvaluateTypeDef


def get_value() -> RuleBooleanToEvaluateTypeDef:
    return {
        "Attribute": ...,
    }


# RuleBooleanToEvaluateTypeDef definition

class RuleBooleanToEvaluateTypeDef(TypedDict):
    Attribute: NotRequired[RuleBooleanEmailAttributeType],  # (1)
    IsInAddressList: NotRequired[RuleIsInAddressListUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: RuleBooleanEmailAttributeType](./literals.md#rulebooleanemailattributetype) 
2. See [:material-code-braces: RuleIsInAddressListTypeDef](./type_defs.md#ruleisinaddresslisttypedef) [:material-code-braces: RuleIsInAddressListOutputTypeDef](./type_defs.md#ruleisinaddresslistoutputtypedef) 
## ArchiveFiltersOutputTypeDef

```python
# ArchiveFiltersOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ArchiveFiltersOutputTypeDef


def get_value() -> ArchiveFiltersOutputTypeDef:
    return {
        "Include": ...,
    }


# ArchiveFiltersOutputTypeDef definition

class ArchiveFiltersOutputTypeDef(TypedDict):
    Include: NotRequired[List[ArchiveFilterConditionOutputTypeDef]],  # (1)
    Unless: NotRequired[List[ArchiveFilterConditionOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: ArchiveFilterConditionOutputTypeDef](./type_defs.md#archivefilterconditionoutputtypedef) 
2. See [:material-code-braces: ArchiveFilterConditionOutputTypeDef](./type_defs.md#archivefilterconditionoutputtypedef) 
## ArchiveFiltersTypeDef

```python
# ArchiveFiltersTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import ArchiveFiltersTypeDef


def get_value() -> ArchiveFiltersTypeDef:
    return {
        "Include": ...,
    }


# ArchiveFiltersTypeDef definition

class ArchiveFiltersTypeDef(TypedDict):
    Include: NotRequired[Sequence[ArchiveFilterConditionTypeDef]],  # (1)
    Unless: NotRequired[Sequence[ArchiveFilterConditionTypeDef]],  # (1)
```

1. See [:material-code-braces: ArchiveFilterConditionTypeDef](./type_defs.md#archivefilterconditiontypedef) 
2. See [:material-code-braces: ArchiveFilterConditionTypeDef](./type_defs.md#archivefilterconditiontypedef) 
## PolicyConditionOutputTypeDef

```python
# PolicyConditionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import PolicyConditionOutputTypeDef


def get_value() -> PolicyConditionOutputTypeDef:
    return {
        "BooleanExpression": ...,
    }


# PolicyConditionOutputTypeDef definition

class PolicyConditionOutputTypeDef(TypedDict):
    BooleanExpression: NotRequired[IngressBooleanExpressionOutputTypeDef],  # (1)
    IpExpression: NotRequired[IngressIpv4ExpressionOutputTypeDef],  # (2)
    StringExpression: NotRequired[IngressStringExpressionOutputTypeDef],  # (3)
    TlsExpression: NotRequired[IngressTlsProtocolExpressionTypeDef],  # (4)
```

1. See [:material-code-braces: IngressBooleanExpressionOutputTypeDef](./type_defs.md#ingressbooleanexpressionoutputtypedef) 
2. See [:material-code-braces: IngressIpv4ExpressionOutputTypeDef](./type_defs.md#ingressipv4expressionoutputtypedef) 
3. See [:material-code-braces: IngressStringExpressionOutputTypeDef](./type_defs.md#ingressstringexpressionoutputtypedef) 
4. See [:material-code-braces: IngressTlsProtocolExpressionTypeDef](./type_defs.md#ingresstlsprotocolexpressiontypedef) 
## RuleConditionOutputTypeDef

```python
# RuleConditionOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleConditionOutputTypeDef


def get_value() -> RuleConditionOutputTypeDef:
    return {
        "BooleanExpression": ...,
    }


# RuleConditionOutputTypeDef definition

class RuleConditionOutputTypeDef(TypedDict):
    BooleanExpression: NotRequired[RuleBooleanExpressionOutputTypeDef],  # (1)
    DmarcExpression: NotRequired[RuleDmarcExpressionOutputTypeDef],  # (2)
    IpExpression: NotRequired[RuleIpExpressionOutputTypeDef],  # (3)
    NumberExpression: NotRequired[RuleNumberExpressionTypeDef],  # (4)
    StringExpression: NotRequired[RuleStringExpressionOutputTypeDef],  # (5)
    VerdictExpression: NotRequired[RuleVerdictExpressionOutputTypeDef],  # (6)
```

1. See [:material-code-braces: RuleBooleanExpressionOutputTypeDef](./type_defs.md#rulebooleanexpressionoutputtypedef) 
2. See [:material-code-braces: RuleDmarcExpressionOutputTypeDef](./type_defs.md#ruledmarcexpressionoutputtypedef) 
3. See [:material-code-braces: RuleIpExpressionOutputTypeDef](./type_defs.md#ruleipexpressionoutputtypedef) 
4. See [:material-code-braces: RuleNumberExpressionTypeDef](./type_defs.md#rulenumberexpressiontypedef) 
5. See [:material-code-braces: RuleStringExpressionOutputTypeDef](./type_defs.md#rulestringexpressionoutputtypedef) 
6. See [:material-code-braces: RuleVerdictExpressionOutputTypeDef](./type_defs.md#ruleverdictexpressionoutputtypedef) 
## GetArchiveExportResponseTypeDef

```python
# GetArchiveExportResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetArchiveExportResponseTypeDef


def get_value() -> GetArchiveExportResponseTypeDef:
    return {
        "ArchiveId": ...,
    }


# GetArchiveExportResponseTypeDef definition

class GetArchiveExportResponseTypeDef(TypedDict):
    ArchiveId: str,
    ExportDestinationConfiguration: ExportDestinationConfigurationTypeDef,  # (1)
    Filters: ArchiveFiltersOutputTypeDef,  # (2)
    FromTimestamp: datetime,
    MaxResults: int,
    Status: ExportStatusTypeDef,  # (3)
    ToTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ExportDestinationConfigurationTypeDef](./type_defs.md#exportdestinationconfigurationtypedef) 
2. See [:material-code-braces: ArchiveFiltersOutputTypeDef](./type_defs.md#archivefiltersoutputtypedef) 
3. See [:material-code-braces: ExportStatusTypeDef](./type_defs.md#exportstatustypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetArchiveSearchResponseTypeDef

```python
# GetArchiveSearchResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetArchiveSearchResponseTypeDef


def get_value() -> GetArchiveSearchResponseTypeDef:
    return {
        "ArchiveId": ...,
    }


# GetArchiveSearchResponseTypeDef definition

class GetArchiveSearchResponseTypeDef(TypedDict):
    ArchiveId: str,
    Filters: ArchiveFiltersOutputTypeDef,  # (1)
    FromTimestamp: datetime,
    MaxResults: int,
    Status: SearchStatusTypeDef,  # (2)
    ToTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ArchiveFiltersOutputTypeDef](./type_defs.md#archivefiltersoutputtypedef) 
2. See [:material-code-braces: SearchStatusTypeDef](./type_defs.md#searchstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyStatementOutputTypeDef

```python
# PolicyStatementOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import PolicyStatementOutputTypeDef


def get_value() -> PolicyStatementOutputTypeDef:
    return {
        "Action": ...,
    }


# PolicyStatementOutputTypeDef definition

class PolicyStatementOutputTypeDef(TypedDict):
    Action: AcceptActionType,  # (1)
    Conditions: List[PolicyConditionOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: AcceptActionType](./literals.md#acceptactiontype) 
2. See [:material-code-braces: PolicyConditionOutputTypeDef](./type_defs.md#policyconditionoutputtypedef) 
## IngressBooleanExpressionTypeDef

```python
# IngressBooleanExpressionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import IngressBooleanExpressionTypeDef


def get_value() -> IngressBooleanExpressionTypeDef:
    return {
        "Evaluate": ...,
    }


# IngressBooleanExpressionTypeDef definition

class IngressBooleanExpressionTypeDef(TypedDict):
    Evaluate: IngressBooleanToEvaluateUnionTypeDef,  # (1)
    Operator: IngressBooleanOperatorType,  # (2)
```

1. See [:material-code-braces: IngressBooleanToEvaluateTypeDef](./type_defs.md#ingressbooleantoevaluatetypedef) [:material-code-braces: IngressBooleanToEvaluateOutputTypeDef](./type_defs.md#ingressbooleantoevaluateoutputtypedef) 
2. See [:material-code-brackets: IngressBooleanOperatorType](./literals.md#ingressbooleanoperatortype) 
## RuleOutputTypeDef

```python
# RuleOutputTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleOutputTypeDef


def get_value() -> RuleOutputTypeDef:
    return {
        "Actions": ...,
    }


# RuleOutputTypeDef definition

class RuleOutputTypeDef(TypedDict):
    Actions: List[RuleActionOutputTypeDef],  # (1)
    Conditions: NotRequired[List[RuleConditionOutputTypeDef]],  # (2)
    Name: NotRequired[str],
    Unless: NotRequired[List[RuleConditionOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-braces: RuleConditionOutputTypeDef](./type_defs.md#ruleconditionoutputtypedef) 
3. See [:material-code-braces: RuleConditionOutputTypeDef](./type_defs.md#ruleconditionoutputtypedef) 
## RuleBooleanExpressionTypeDef

```python
# RuleBooleanExpressionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleBooleanExpressionTypeDef


def get_value() -> RuleBooleanExpressionTypeDef:
    return {
        "Evaluate": ...,
    }


# RuleBooleanExpressionTypeDef definition

class RuleBooleanExpressionTypeDef(TypedDict):
    Evaluate: RuleBooleanToEvaluateUnionTypeDef,  # (1)
    Operator: RuleBooleanOperatorType,  # (2)
```

1. See [:material-code-braces: RuleBooleanToEvaluateTypeDef](./type_defs.md#rulebooleantoevaluatetypedef) [:material-code-braces: RuleBooleanToEvaluateOutputTypeDef](./type_defs.md#rulebooleantoevaluateoutputtypedef) 
2. See [:material-code-brackets: RuleBooleanOperatorType](./literals.md#rulebooleanoperatortype) 
## StartArchiveExportRequestTypeDef

```python
# StartArchiveExportRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import StartArchiveExportRequestTypeDef


def get_value() -> StartArchiveExportRequestTypeDef:
    return {
        "ArchiveId": ...,
    }


# StartArchiveExportRequestTypeDef definition

class StartArchiveExportRequestTypeDef(TypedDict):
    ArchiveId: str,
    ExportDestinationConfiguration: ExportDestinationConfigurationTypeDef,  # (1)
    FromTimestamp: TimestampTypeDef,
    ToTimestamp: TimestampTypeDef,
    Filters: NotRequired[ArchiveFiltersUnionTypeDef],  # (2)
    IncludeMetadata: NotRequired[bool],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ExportDestinationConfigurationTypeDef](./type_defs.md#exportdestinationconfigurationtypedef) 
2. See [:material-code-braces: ArchiveFiltersTypeDef](./type_defs.md#archivefilterstypedef) [:material-code-braces: ArchiveFiltersOutputTypeDef](./type_defs.md#archivefiltersoutputtypedef) 
## StartArchiveSearchRequestTypeDef

```python
# StartArchiveSearchRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import StartArchiveSearchRequestTypeDef


def get_value() -> StartArchiveSearchRequestTypeDef:
    return {
        "ArchiveId": ...,
    }


# StartArchiveSearchRequestTypeDef definition

class StartArchiveSearchRequestTypeDef(TypedDict):
    ArchiveId: str,
    FromTimestamp: TimestampTypeDef,
    MaxResults: int,
    ToTimestamp: TimestampTypeDef,
    Filters: NotRequired[ArchiveFiltersUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ArchiveFiltersTypeDef](./type_defs.md#archivefilterstypedef) [:material-code-braces: ArchiveFiltersOutputTypeDef](./type_defs.md#archivefiltersoutputtypedef) 
## GetTrafficPolicyResponseTypeDef

```python
# GetTrafficPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetTrafficPolicyResponseTypeDef


def get_value() -> GetTrafficPolicyResponseTypeDef:
    return {
        "CreatedTimestamp": ...,
    }


# GetTrafficPolicyResponseTypeDef definition

class GetTrafficPolicyResponseTypeDef(TypedDict):
    CreatedTimestamp: datetime,
    DefaultAction: AcceptActionType,  # (1)
    LastUpdatedTimestamp: datetime,
    MaxMessageSizeBytes: int,
    PolicyStatements: List[PolicyStatementOutputTypeDef],  # (2)
    TrafficPolicyArn: str,
    TrafficPolicyId: str,
    TrafficPolicyName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AcceptActionType](./literals.md#acceptactiontype) 
2. See [:material-code-braces: PolicyStatementOutputTypeDef](./type_defs.md#policystatementoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRuleSetResponseTypeDef

```python
# GetRuleSetResponseTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import GetRuleSetResponseTypeDef


def get_value() -> GetRuleSetResponseTypeDef:
    return {
        "CreatedDate": ...,
    }


# GetRuleSetResponseTypeDef definition

class GetRuleSetResponseTypeDef(TypedDict):
    CreatedDate: datetime,
    LastModificationDate: datetime,
    RuleSetArn: str,
    RuleSetId: str,
    RuleSetName: str,
    Rules: List[RuleOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyConditionTypeDef

```python
# PolicyConditionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import PolicyConditionTypeDef


def get_value() -> PolicyConditionTypeDef:
    return {
        "BooleanExpression": ...,
    }


# PolicyConditionTypeDef definition

class PolicyConditionTypeDef(TypedDict):
    BooleanExpression: NotRequired[IngressBooleanExpressionUnionTypeDef],  # (1)
    IpExpression: NotRequired[IngressIpv4ExpressionUnionTypeDef],  # (2)
    StringExpression: NotRequired[IngressStringExpressionUnionTypeDef],  # (3)
    TlsExpression: NotRequired[IngressTlsProtocolExpressionTypeDef],  # (4)
```

1. See [:material-code-braces: IngressBooleanExpressionTypeDef](./type_defs.md#ingressbooleanexpressiontypedef) [:material-code-braces: IngressBooleanExpressionOutputTypeDef](./type_defs.md#ingressbooleanexpressionoutputtypedef) 
2. See [:material-code-braces: IngressIpv4ExpressionTypeDef](./type_defs.md#ingressipv4expressiontypedef) [:material-code-braces: IngressIpv4ExpressionOutputTypeDef](./type_defs.md#ingressipv4expressionoutputtypedef) 
3. See [:material-code-braces: IngressStringExpressionTypeDef](./type_defs.md#ingressstringexpressiontypedef) [:material-code-braces: IngressStringExpressionOutputTypeDef](./type_defs.md#ingressstringexpressionoutputtypedef) 
4. See [:material-code-braces: IngressTlsProtocolExpressionTypeDef](./type_defs.md#ingresstlsprotocolexpressiontypedef) 
## RuleConditionTypeDef

```python
# RuleConditionTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleConditionTypeDef


def get_value() -> RuleConditionTypeDef:
    return {
        "BooleanExpression": ...,
    }


# RuleConditionTypeDef definition

class RuleConditionTypeDef(TypedDict):
    BooleanExpression: NotRequired[RuleBooleanExpressionUnionTypeDef],  # (1)
    DmarcExpression: NotRequired[RuleDmarcExpressionUnionTypeDef],  # (2)
    IpExpression: NotRequired[RuleIpExpressionUnionTypeDef],  # (3)
    NumberExpression: NotRequired[RuleNumberExpressionTypeDef],  # (4)
    StringExpression: NotRequired[RuleStringExpressionUnionTypeDef],  # (5)
    VerdictExpression: NotRequired[RuleVerdictExpressionUnionTypeDef],  # (6)
```

1. See [:material-code-braces: RuleBooleanExpressionTypeDef](./type_defs.md#rulebooleanexpressiontypedef) [:material-code-braces: RuleBooleanExpressionOutputTypeDef](./type_defs.md#rulebooleanexpressionoutputtypedef) 
2. See [:material-code-braces: RuleDmarcExpressionTypeDef](./type_defs.md#ruledmarcexpressiontypedef) [:material-code-braces: RuleDmarcExpressionOutputTypeDef](./type_defs.md#ruledmarcexpressionoutputtypedef) 
3. See [:material-code-braces: RuleIpExpressionTypeDef](./type_defs.md#ruleipexpressiontypedef) [:material-code-braces: RuleIpExpressionOutputTypeDef](./type_defs.md#ruleipexpressionoutputtypedef) 
4. See [:material-code-braces: RuleNumberExpressionTypeDef](./type_defs.md#rulenumberexpressiontypedef) 
5. See [:material-code-braces: RuleStringExpressionTypeDef](./type_defs.md#rulestringexpressiontypedef) [:material-code-braces: RuleStringExpressionOutputTypeDef](./type_defs.md#rulestringexpressionoutputtypedef) 
6. See [:material-code-braces: RuleVerdictExpressionTypeDef](./type_defs.md#ruleverdictexpressiontypedef) [:material-code-braces: RuleVerdictExpressionOutputTypeDef](./type_defs.md#ruleverdictexpressionoutputtypedef) 
## PolicyStatementTypeDef

```python
# PolicyStatementTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import PolicyStatementTypeDef


def get_value() -> PolicyStatementTypeDef:
    return {
        "Action": ...,
    }


# PolicyStatementTypeDef definition

class PolicyStatementTypeDef(TypedDict):
    Action: AcceptActionType,  # (1)
    Conditions: Sequence[PolicyConditionUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: AcceptActionType](./literals.md#acceptactiontype) 
2. See [:material-code-braces: PolicyConditionTypeDef](./type_defs.md#policyconditiontypedef) [:material-code-braces: PolicyConditionOutputTypeDef](./type_defs.md#policyconditionoutputtypedef) 
## RuleTypeDef

```python
# RuleTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import RuleTypeDef


def get_value() -> RuleTypeDef:
    return {
        "Actions": ...,
    }


# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    Actions: Sequence[RuleActionUnionTypeDef],  # (1)
    Conditions: NotRequired[Sequence[RuleConditionUnionTypeDef]],  # (2)
    Name: NotRequired[str],
    Unless: NotRequired[Sequence[RuleConditionUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-braces: RuleConditionTypeDef](./type_defs.md#ruleconditiontypedef) [:material-code-braces: RuleConditionOutputTypeDef](./type_defs.md#ruleconditionoutputtypedef) 
3. See [:material-code-braces: RuleConditionTypeDef](./type_defs.md#ruleconditiontypedef) [:material-code-braces: RuleConditionOutputTypeDef](./type_defs.md#ruleconditionoutputtypedef) 
## CreateTrafficPolicyRequestTypeDef

```python
# CreateTrafficPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateTrafficPolicyRequestTypeDef


def get_value() -> CreateTrafficPolicyRequestTypeDef:
    return {
        "DefaultAction": ...,
    }


# CreateTrafficPolicyRequestTypeDef definition

class CreateTrafficPolicyRequestTypeDef(TypedDict):
    DefaultAction: AcceptActionType,  # (1)
    PolicyStatements: Sequence[PolicyStatementUnionTypeDef],  # (2)
    TrafficPolicyName: str,
    ClientToken: NotRequired[str],
    MaxMessageSizeBytes: NotRequired[int],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: AcceptActionType](./literals.md#acceptactiontype) 
2. See [:material-code-braces: PolicyStatementTypeDef](./type_defs.md#policystatementtypedef) [:material-code-braces: PolicyStatementOutputTypeDef](./type_defs.md#policystatementoutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateTrafficPolicyRequestTypeDef

```python
# UpdateTrafficPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import UpdateTrafficPolicyRequestTypeDef


def get_value() -> UpdateTrafficPolicyRequestTypeDef:
    return {
        "TrafficPolicyId": ...,
    }


# UpdateTrafficPolicyRequestTypeDef definition

class UpdateTrafficPolicyRequestTypeDef(TypedDict):
    TrafficPolicyId: str,
    DefaultAction: NotRequired[AcceptActionType],  # (1)
    MaxMessageSizeBytes: NotRequired[int],
    PolicyStatements: NotRequired[Sequence[PolicyStatementUnionTypeDef]],  # (2)
    TrafficPolicyName: NotRequired[str],
```

1. See [:material-code-brackets: AcceptActionType](./literals.md#acceptactiontype) 
2. See [:material-code-braces: PolicyStatementTypeDef](./type_defs.md#policystatementtypedef) [:material-code-braces: PolicyStatementOutputTypeDef](./type_defs.md#policystatementoutputtypedef) 
## CreateRuleSetRequestTypeDef

```python
# CreateRuleSetRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import CreateRuleSetRequestTypeDef


def get_value() -> CreateRuleSetRequestTypeDef:
    return {
        "RuleSetName": ...,
    }


# CreateRuleSetRequestTypeDef definition

class CreateRuleSetRequestTypeDef(TypedDict):
    RuleSetName: str,
    Rules: Sequence[RuleUnionTypeDef],  # (1)
    ClientToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateRuleSetRequestTypeDef

```python
# UpdateRuleSetRequestTypeDef TypedDict usage example

from types_aiobotocore_mailmanager.type_defs import UpdateRuleSetRequestTypeDef


def get_value() -> UpdateRuleSetRequestTypeDef:
    return {
        "RuleSetId": ...,
    }


# UpdateRuleSetRequestTypeDef definition

class UpdateRuleSetRequestTypeDef(TypedDict):
    RuleSetId: str,
    RuleSetName: NotRequired[str],
    Rules: NotRequired[Sequence[RuleUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
