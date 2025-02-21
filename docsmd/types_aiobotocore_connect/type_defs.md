# Type definitions

> [Index](../README.md) > [Connect](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Connect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#connect)
    type annotations stubs module [types-aiobotocore-connect](https://pypi.org/project/types-aiobotocore-connect/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_connect.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AgentsCriteriaUnionTypeDef

```python
# AgentsCriteriaUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import AgentsCriteriaUnionTypeDef


def get_value() -> AgentsCriteriaUnionTypeDef:
    return ...


# AgentsCriteriaUnionTypeDef definition

AgentsCriteriaUnionTypeDef = Union[
    AgentsCriteriaTypeDef,  # (1)
    AgentsCriteriaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AgentsCriteriaTypeDef](./type_defs.md#agentscriteriatypedef) 
2. See [:material-code-braces: AgentsCriteriaOutputTypeDef](./type_defs.md#agentscriteriaoutputtypedef) 

## ApplicationUnionTypeDef

```python
# ApplicationUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import ApplicationUnionTypeDef


def get_value() -> ApplicationUnionTypeDef:
    return ...


# ApplicationUnionTypeDef definition

ApplicationUnionTypeDef = Union[
    ApplicationTypeDef,  # (1)
    ApplicationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ApplicationOutputTypeDef](./type_defs.md#applicationoutputtypedef) 

## EvaluationFormSectionUnionTypeDef

```python
# EvaluationFormSectionUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import EvaluationFormSectionUnionTypeDef


def get_value() -> EvaluationFormSectionUnionTypeDef:
    return ...


# EvaluationFormSectionUnionTypeDef definition

EvaluationFormSectionUnionTypeDef = Union[
    EvaluationFormSectionTypeDef,  # (1)
    EvaluationFormSectionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EvaluationFormSectionTypeDef](./type_defs.md#evaluationformsectiontypedef) 
2. See [:material-code-braces: EvaluationFormSectionOutputTypeDef](./type_defs.md#evaluationformsectionoutputtypedef) 

## FieldValueUnionUnionTypeDef

```python
# FieldValueUnionUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import FieldValueUnionUnionTypeDef


def get_value() -> FieldValueUnionUnionTypeDef:
    return ...


# FieldValueUnionUnionTypeDef definition

FieldValueUnionUnionTypeDef = Union[
    FieldValueUnionTypeDef,  # (1)
    FieldValueUnionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FieldValueUnionTypeDef](./type_defs.md#fieldvalueuniontypedef) 
2. See [:material-code-braces: FieldValueUnionOutputTypeDef](./type_defs.md#fieldvalueunionoutputtypedef) 

## MetricFilterV2UnionTypeDef

```python
# MetricFilterV2UnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import MetricFilterV2UnionTypeDef


def get_value() -> MetricFilterV2UnionTypeDef:
    return ...


# MetricFilterV2UnionTypeDef definition

MetricFilterV2UnionTypeDef = Union[
    MetricFilterV2TypeDef,  # (1)
    MetricFilterV2OutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MetricFilterV2TypeDef](./type_defs.md#metricfilterv2typedef) 
2. See [:material-code-braces: MetricFilterV2OutputTypeDef](./type_defs.md#metricfilterv2outputtypedef) 

## NotificationRecipientTypeUnionTypeDef

```python
# NotificationRecipientTypeUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import NotificationRecipientTypeUnionTypeDef


def get_value() -> NotificationRecipientTypeUnionTypeDef:
    return ...


# NotificationRecipientTypeUnionTypeDef definition

NotificationRecipientTypeUnionTypeDef = Union[
    NotificationRecipientTypeTypeDef,  # (1)
    NotificationRecipientTypeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NotificationRecipientTypeTypeDef](./type_defs.md#notificationrecipienttypetypedef) 
2. See [:material-code-braces: NotificationRecipientTypeOutputTypeDef](./type_defs.md#notificationrecipienttypeoutputtypedef) 

## PredefinedAttributeValuesUnionTypeDef

```python
# PredefinedAttributeValuesUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import PredefinedAttributeValuesUnionTypeDef


def get_value() -> PredefinedAttributeValuesUnionTypeDef:
    return ...


# PredefinedAttributeValuesUnionTypeDef definition

PredefinedAttributeValuesUnionTypeDef = Union[
    PredefinedAttributeValuesTypeDef,  # (1)
    PredefinedAttributeValuesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PredefinedAttributeValuesTypeDef](./type_defs.md#predefinedattributevaluestypedef) 
2. See [:material-code-braces: PredefinedAttributeValuesOutputTypeDef](./type_defs.md#predefinedattributevaluesoutputtypedef) 

## SegmentAttributeValueUnionTypeDef

```python
# SegmentAttributeValueUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import SegmentAttributeValueUnionTypeDef


def get_value() -> SegmentAttributeValueUnionTypeDef:
    return ...


# SegmentAttributeValueUnionTypeDef definition

SegmentAttributeValueUnionTypeDef = Union[
    SegmentAttributeValueTypeDef,  # (1)
    SegmentAttributeValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) 
2. See [:material-code-braces: SegmentAttributeValueOutputTypeDef](./type_defs.md#segmentattributevalueoutputtypedef) 

## AgentConfigUnionTypeDef

```python
# AgentConfigUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import AgentConfigUnionTypeDef


def get_value() -> AgentConfigUnionTypeDef:
    return ...


# AgentConfigUnionTypeDef definition

AgentConfigUnionTypeDef = Union[
    AgentConfigTypeDef,  # (1)
    AgentConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AgentConfigTypeDef](./type_defs.md#agentconfigtypedef) 
2. See [:material-code-braces: AgentConfigOutputTypeDef](./type_defs.md#agentconfigoutputtypedef) 

## TelephonyConfigUnionTypeDef

```python
# TelephonyConfigUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import TelephonyConfigUnionTypeDef


def get_value() -> TelephonyConfigUnionTypeDef:
    return ...


# TelephonyConfigUnionTypeDef definition

TelephonyConfigUnionTypeDef = Union[
    TelephonyConfigTypeDef,  # (1)
    TelephonyConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TelephonyConfigTypeDef](./type_defs.md#telephonyconfigtypedef) 
2. See [:material-code-braces: TelephonyConfigOutputTypeDef](./type_defs.md#telephonyconfigoutputtypedef) 

## TaskActionDefinitionUnionTypeDef

```python
# TaskActionDefinitionUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import TaskActionDefinitionUnionTypeDef


def get_value() -> TaskActionDefinitionUnionTypeDef:
    return ...


# TaskActionDefinitionUnionTypeDef definition

TaskActionDefinitionUnionTypeDef = Union[
    TaskActionDefinitionTypeDef,  # (1)
    TaskActionDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TaskActionDefinitionTypeDef](./type_defs.md#taskactiondefinitiontypedef) 
2. See [:material-code-braces: TaskActionDefinitionOutputTypeDef](./type_defs.md#taskactiondefinitionoutputtypedef) 

## TaskTemplateFieldUnionTypeDef

```python
# TaskTemplateFieldUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import TaskTemplateFieldUnionTypeDef


def get_value() -> TaskTemplateFieldUnionTypeDef:
    return ...


# TaskTemplateFieldUnionTypeDef definition

TaskTemplateFieldUnionTypeDef = Union[
    TaskTemplateFieldTypeDef,  # (1)
    TaskTemplateFieldOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TaskTemplateFieldTypeDef](./type_defs.md#tasktemplatefieldtypedef) 
2. See [:material-code-braces: TaskTemplateFieldOutputTypeDef](./type_defs.md#tasktemplatefieldoutputtypedef) 

## SignInConfigUnionTypeDef

```python
# SignInConfigUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import SignInConfigUnionTypeDef


def get_value() -> SignInConfigUnionTypeDef:
    return ...


# SignInConfigUnionTypeDef definition

SignInConfigUnionTypeDef = Union[
    SignInConfigTypeDef,  # (1)
    SignInConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SignInConfigTypeDef](./type_defs.md#signinconfigtypedef) 
2. See [:material-code-braces: SignInConfigOutputTypeDef](./type_defs.md#signinconfigoutputtypedef) 

## MatchCriteriaUnionTypeDef

```python
# MatchCriteriaUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import MatchCriteriaUnionTypeDef


def get_value() -> MatchCriteriaUnionTypeDef:
    return ...


# MatchCriteriaUnionTypeDef definition

MatchCriteriaUnionTypeDef = Union[
    MatchCriteriaTypeDef,  # (1)
    MatchCriteriaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MatchCriteriaTypeDef](./type_defs.md#matchcriteriatypedef) 
2. See [:material-code-braces: MatchCriteriaOutputTypeDef](./type_defs.md#matchcriteriaoutputtypedef) 

## EvaluationFormNumericQuestionPropertiesUnionTypeDef

```python
# EvaluationFormNumericQuestionPropertiesUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import EvaluationFormNumericQuestionPropertiesUnionTypeDef


def get_value() -> EvaluationFormNumericQuestionPropertiesUnionTypeDef:
    return ...


# EvaluationFormNumericQuestionPropertiesUnionTypeDef definition

EvaluationFormNumericQuestionPropertiesUnionTypeDef = Union[
    EvaluationFormNumericQuestionPropertiesTypeDef,  # (1)
    EvaluationFormNumericQuestionPropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EvaluationFormNumericQuestionPropertiesTypeDef](./type_defs.md#evaluationformnumericquestionpropertiestypedef) 
2. See [:material-code-braces: EvaluationFormNumericQuestionPropertiesOutputTypeDef](./type_defs.md#evaluationformnumericquestionpropertiesoutputtypedef) 

## EvaluationFormSingleSelectQuestionAutomationUnionTypeDef

```python
# EvaluationFormSingleSelectQuestionAutomationUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import EvaluationFormSingleSelectQuestionAutomationUnionTypeDef


def get_value() -> EvaluationFormSingleSelectQuestionAutomationUnionTypeDef:
    return ...


# EvaluationFormSingleSelectQuestionAutomationUnionTypeDef definition

EvaluationFormSingleSelectQuestionAutomationUnionTypeDef = Union[
    EvaluationFormSingleSelectQuestionAutomationTypeDef,  # (1)
    EvaluationFormSingleSelectQuestionAutomationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EvaluationFormSingleSelectQuestionAutomationTypeDef](./type_defs.md#evaluationformsingleselectquestionautomationtypedef) 
2. See [:material-code-braces: EvaluationFormSingleSelectQuestionAutomationOutputTypeDef](./type_defs.md#evaluationformsingleselectquestionautomationoutputtypedef) 

## FieldValueUnionExtraTypeDef

```python
# FieldValueUnionExtraTypeDef Union usage example

from types_aiobotocore_connect.type_defs import FieldValueUnionExtraTypeDef


def get_value() -> FieldValueUnionExtraTypeDef:
    return ...


# FieldValueUnionExtraTypeDef definition

FieldValueUnionExtraTypeDef = Union[
    FieldValueTypeDef,  # (1)
    FieldValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
2. See [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 

## TaskTemplateConstraintsUnionTypeDef

```python
# TaskTemplateConstraintsUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import TaskTemplateConstraintsUnionTypeDef


def get_value() -> TaskTemplateConstraintsUnionTypeDef:
    return ...


# TaskTemplateConstraintsUnionTypeDef definition

TaskTemplateConstraintsUnionTypeDef = Union[
    TaskTemplateConstraintsTypeDef,  # (1)
    TaskTemplateConstraintsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TaskTemplateConstraintsTypeDef](./type_defs.md#tasktemplateconstraintstypedef) 
2. See [:material-code-braces: TaskTemplateConstraintsOutputTypeDef](./type_defs.md#tasktemplateconstraintsoutputtypedef) 

## TaskTemplateDefaultsUnionTypeDef

```python
# TaskTemplateDefaultsUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import TaskTemplateDefaultsUnionTypeDef


def get_value() -> TaskTemplateDefaultsUnionTypeDef:
    return ...


# TaskTemplateDefaultsUnionTypeDef definition

TaskTemplateDefaultsUnionTypeDef = Union[
    TaskTemplateDefaultsTypeDef,  # (1)
    TaskTemplateDefaultsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TaskTemplateDefaultsTypeDef](./type_defs.md#tasktemplatedefaultstypedef) 
2. See [:material-code-braces: TaskTemplateDefaultsOutputTypeDef](./type_defs.md#tasktemplatedefaultsoutputtypedef) 

## MetricV2UnionTypeDef

```python
# MetricV2UnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import MetricV2UnionTypeDef


def get_value() -> MetricV2UnionTypeDef:
    return ...


# MetricV2UnionTypeDef definition

MetricV2UnionTypeDef = Union[
    MetricV2TypeDef,  # (1)
    MetricV2OutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MetricV2TypeDef](./type_defs.md#metricv2typedef) 
2. See [:material-code-braces: MetricV2OutputTypeDef](./type_defs.md#metricv2outputtypedef) 

## SendNotificationActionDefinitionUnionTypeDef

```python
# SendNotificationActionDefinitionUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import SendNotificationActionDefinitionUnionTypeDef


def get_value() -> SendNotificationActionDefinitionUnionTypeDef:
    return ...


# SendNotificationActionDefinitionUnionTypeDef definition

SendNotificationActionDefinitionUnionTypeDef = Union[
    SendNotificationActionDefinitionTypeDef,  # (1)
    SendNotificationActionDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SendNotificationActionDefinitionTypeDef](./type_defs.md#sendnotificationactiondefinitiontypedef) 
2. See [:material-code-braces: SendNotificationActionDefinitionOutputTypeDef](./type_defs.md#sendnotificationactiondefinitionoutputtypedef) 

## AttributeConditionUnionTypeDef

```python
# AttributeConditionUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import AttributeConditionUnionTypeDef


def get_value() -> AttributeConditionUnionTypeDef:
    return ...


# AttributeConditionUnionTypeDef definition

AttributeConditionUnionTypeDef = Union[
    AttributeConditionTypeDef,  # (1)
    AttributeConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttributeConditionTypeDef](./type_defs.md#attributeconditiontypedef) 
2. See [:material-code-braces: AttributeConditionOutputTypeDef](./type_defs.md#attributeconditionoutputtypedef) 

## EvaluationFormSingleSelectQuestionPropertiesUnionTypeDef

```python
# EvaluationFormSingleSelectQuestionPropertiesUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import EvaluationFormSingleSelectQuestionPropertiesUnionTypeDef


def get_value() -> EvaluationFormSingleSelectQuestionPropertiesUnionTypeDef:
    return ...


# EvaluationFormSingleSelectQuestionPropertiesUnionTypeDef definition

EvaluationFormSingleSelectQuestionPropertiesUnionTypeDef = Union[
    EvaluationFormSingleSelectQuestionPropertiesTypeDef,  # (1)
    EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EvaluationFormSingleSelectQuestionPropertiesTypeDef](./type_defs.md#evaluationformsingleselectquestionpropertiestypedef) 
2. See [:material-code-braces: EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef](./type_defs.md#evaluationformsingleselectquestionpropertiesoutputtypedef) 

## CreateCaseActionDefinitionUnionTypeDef

```python
# CreateCaseActionDefinitionUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import CreateCaseActionDefinitionUnionTypeDef


def get_value() -> CreateCaseActionDefinitionUnionTypeDef:
    return ...


# CreateCaseActionDefinitionUnionTypeDef definition

CreateCaseActionDefinitionUnionTypeDef = Union[
    CreateCaseActionDefinitionTypeDef,  # (1)
    CreateCaseActionDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CreateCaseActionDefinitionTypeDef](./type_defs.md#createcaseactiondefinitiontypedef) 
2. See [:material-code-braces: CreateCaseActionDefinitionOutputTypeDef](./type_defs.md#createcaseactiondefinitionoutputtypedef) 

## UpdateCaseActionDefinitionUnionTypeDef

```python
# UpdateCaseActionDefinitionUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import UpdateCaseActionDefinitionUnionTypeDef


def get_value() -> UpdateCaseActionDefinitionUnionTypeDef:
    return ...


# UpdateCaseActionDefinitionUnionTypeDef definition

UpdateCaseActionDefinitionUnionTypeDef = Union[
    UpdateCaseActionDefinitionTypeDef,  # (1)
    UpdateCaseActionDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: UpdateCaseActionDefinitionTypeDef](./type_defs.md#updatecaseactiondefinitiontypedef) 
2. See [:material-code-braces: UpdateCaseActionDefinitionOutputTypeDef](./type_defs.md#updatecaseactiondefinitionoutputtypedef) 

## ExpressionUnionTypeDef

```python
# ExpressionUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import ExpressionUnionTypeDef


def get_value() -> ExpressionUnionTypeDef:
    return ...


# ExpressionUnionTypeDef definition

ExpressionUnionTypeDef = Union[
    ExpressionTypeDef,  # (1)
    ExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
2. See [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 

## EvaluationFormQuestionTypePropertiesUnionTypeDef

```python
# EvaluationFormQuestionTypePropertiesUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import EvaluationFormQuestionTypePropertiesUnionTypeDef


def get_value() -> EvaluationFormQuestionTypePropertiesUnionTypeDef:
    return ...


# EvaluationFormQuestionTypePropertiesUnionTypeDef definition

EvaluationFormQuestionTypePropertiesUnionTypeDef = Union[
    EvaluationFormQuestionTypePropertiesTypeDef,  # (1)
    EvaluationFormQuestionTypePropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EvaluationFormQuestionTypePropertiesTypeDef](./type_defs.md#evaluationformquestiontypepropertiestypedef) 
2. See [:material-code-braces: EvaluationFormQuestionTypePropertiesOutputTypeDef](./type_defs.md#evaluationformquestiontypepropertiesoutputtypedef) 

## RuleActionUnionTypeDef

```python
# RuleActionUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import RuleActionUnionTypeDef


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

## EvaluationFormQuestionUnionTypeDef

```python
# EvaluationFormQuestionUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import EvaluationFormQuestionUnionTypeDef


def get_value() -> EvaluationFormQuestionUnionTypeDef:
    return ...


# EvaluationFormQuestionUnionTypeDef definition

EvaluationFormQuestionUnionTypeDef = Union[
    EvaluationFormQuestionTypeDef,  # (1)
    EvaluationFormQuestionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EvaluationFormQuestionTypeDef](./type_defs.md#evaluationformquestiontypedef) 
2. See [:material-code-braces: EvaluationFormQuestionOutputTypeDef](./type_defs.md#evaluationformquestionoutputtypedef) 

## EvaluationFormItemUnionTypeDef

```python
# EvaluationFormItemUnionTypeDef Union usage example

from types_aiobotocore_connect.type_defs import EvaluationFormItemUnionTypeDef


def get_value() -> EvaluationFormItemUnionTypeDef:
    return ...


# EvaluationFormItemUnionTypeDef definition

EvaluationFormItemUnionTypeDef = Union[
    EvaluationFormItemTypeDef,  # (1)
    EvaluationFormItemOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EvaluationFormItemTypeDef](./type_defs.md#evaluationformitemtypedef) 
2. See [:material-code-braces: EvaluationFormItemOutputTypeDef](./type_defs.md#evaluationformitemoutputtypedef) 



## ActionSummaryTypeDef

```python
# ActionSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ActionSummaryTypeDef


def get_value() -> ActionSummaryTypeDef:
    return {
        "ActionType": ...,
    }


# ActionSummaryTypeDef definition

class ActionSummaryTypeDef(TypedDict):
    ActionType: ActionTypeType,  # (1)
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
## ActivateEvaluationFormRequestTypeDef

```python
# ActivateEvaluationFormRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ActivateEvaluationFormRequestTypeDef


def get_value() -> ActivateEvaluationFormRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ActivateEvaluationFormRequestTypeDef definition

class ActivateEvaluationFormRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: int,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ResponseMetadataTypeDef


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

## EmailRecipientTypeDef

```python
# EmailRecipientTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EmailRecipientTypeDef


def get_value() -> EmailRecipientTypeDef:
    return {
        "Address": ...,
    }


# EmailRecipientTypeDef definition

class EmailRecipientTypeDef(TypedDict):
    Address: NotRequired[str],
    DisplayName: NotRequired[str],
```

## DistributionTypeDef

```python
# DistributionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DistributionTypeDef


def get_value() -> DistributionTypeDef:
    return {
        "Region": ...,
    }


# DistributionTypeDef definition

class DistributionTypeDef(TypedDict):
    Region: str,
    Percentage: int,
```

## QueueReferenceTypeDef

```python
# QueueReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QueueReferenceTypeDef


def get_value() -> QueueReferenceTypeDef:
    return {
        "Id": ...,
    }


# QueueReferenceTypeDef definition

class QueueReferenceTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
```

## AgentHierarchyGroupTypeDef

```python
# AgentHierarchyGroupTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentHierarchyGroupTypeDef


def get_value() -> AgentHierarchyGroupTypeDef:
    return {
        "Arn": ...,
    }


# AgentHierarchyGroupTypeDef definition

class AgentHierarchyGroupTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## AgentHierarchyGroupsTypeDef

```python
# AgentHierarchyGroupsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentHierarchyGroupsTypeDef


def get_value() -> AgentHierarchyGroupsTypeDef:
    return {
        "L1Ids": ...,
    }


# AgentHierarchyGroupsTypeDef definition

class AgentHierarchyGroupsTypeDef(TypedDict):
    L1Ids: NotRequired[Sequence[str]],
    L2Ids: NotRequired[Sequence[str]],
    L3Ids: NotRequired[Sequence[str]],
    L4Ids: NotRequired[Sequence[str]],
    L5Ids: NotRequired[Sequence[str]],
```

## DeviceInfoTypeDef

```python
# DeviceInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeviceInfoTypeDef


def get_value() -> DeviceInfoTypeDef:
    return {
        "PlatformName": ...,
    }


# DeviceInfoTypeDef definition

class DeviceInfoTypeDef(TypedDict):
    PlatformName: NotRequired[str],
    PlatformVersion: NotRequired[str],
    OperatingSystem: NotRequired[str],
```

## ParticipantCapabilitiesTypeDef

```python
# ParticipantCapabilitiesTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ParticipantCapabilitiesTypeDef


def get_value() -> ParticipantCapabilitiesTypeDef:
    return {
        "Video": ...,
    }


# ParticipantCapabilitiesTypeDef definition

class ParticipantCapabilitiesTypeDef(TypedDict):
    Video: NotRequired[VideoCapabilityType],  # (1)
    ScreenShare: NotRequired[ScreenShareCapabilityType],  # (2)
```

1. See [:material-code-brackets: VideoCapabilityType](./literals.md#videocapabilitytype) 
2. See [:material-code-brackets: ScreenShareCapabilityType](./literals.md#screensharecapabilitytype) 
## AudioQualityMetricsInfoTypeDef

```python
# AudioQualityMetricsInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AudioQualityMetricsInfoTypeDef


def get_value() -> AudioQualityMetricsInfoTypeDef:
    return {
        "QualityScore": ...,
    }


# AudioQualityMetricsInfoTypeDef definition

class AudioQualityMetricsInfoTypeDef(TypedDict):
    QualityScore: NotRequired[float],
    PotentialQualityIssues: NotRequired[List[str]],
```

## AgentStatusReferenceTypeDef

```python
# AgentStatusReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentStatusReferenceTypeDef


def get_value() -> AgentStatusReferenceTypeDef:
    return {
        "StatusStartTimestamp": ...,
    }


# AgentStatusReferenceTypeDef definition

class AgentStatusReferenceTypeDef(TypedDict):
    StatusStartTimestamp: NotRequired[datetime],
    StatusArn: NotRequired[str],
    StatusName: NotRequired[str],
```

## StringConditionTypeDef

```python
# StringConditionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StringConditionTypeDef


def get_value() -> StringConditionTypeDef:
    return {
        "FieldName": ...,
    }


# StringConditionTypeDef definition

class StringConditionTypeDef(TypedDict):
    FieldName: NotRequired[str],
    Value: NotRequired[str],
    ComparisonType: NotRequired[StringComparisonTypeType],  # (1)
```

1. See [:material-code-brackets: StringComparisonTypeType](./literals.md#stringcomparisontypetype) 
## AgentStatusSummaryTypeDef

```python
# AgentStatusSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentStatusSummaryTypeDef


def get_value() -> AgentStatusSummaryTypeDef:
    return {
        "Id": ...,
    }


# AgentStatusSummaryTypeDef definition

class AgentStatusSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[AgentStatusTypeType],  # (1)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-brackets: AgentStatusTypeType](./literals.md#agentstatustypetype) 
## AgentStatusTypeDef

```python
# AgentStatusTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentStatusTypeDef


def get_value() -> AgentStatusTypeDef:
    return {
        "AgentStatusARN": ...,
    }


# AgentStatusTypeDef definition

class AgentStatusTypeDef(TypedDict):
    AgentStatusARN: NotRequired[str],
    AgentStatusId: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Type: NotRequired[AgentStatusTypeType],  # (1)
    DisplayOrder: NotRequired[int],
    State: NotRequired[AgentStatusStateType],  # (2)
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-brackets: AgentStatusTypeType](./literals.md#agentstatustypetype) 
2. See [:material-code-brackets: AgentStatusStateType](./literals.md#agentstatusstatetype) 
## AgentsCriteriaOutputTypeDef

```python
# AgentsCriteriaOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentsCriteriaOutputTypeDef


def get_value() -> AgentsCriteriaOutputTypeDef:
    return {
        "AgentIds": ...,
    }


# AgentsCriteriaOutputTypeDef definition

class AgentsCriteriaOutputTypeDef(TypedDict):
    AgentIds: NotRequired[List[str]],
```

## AgentsCriteriaTypeDef

```python
# AgentsCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentsCriteriaTypeDef


def get_value() -> AgentsCriteriaTypeDef:
    return {
        "AgentIds": ...,
    }


# AgentsCriteriaTypeDef definition

class AgentsCriteriaTypeDef(TypedDict):
    AgentIds: NotRequired[Sequence[str]],
```

## AnalyticsDataAssociationResultTypeDef

```python
# AnalyticsDataAssociationResultTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AnalyticsDataAssociationResultTypeDef


def get_value() -> AnalyticsDataAssociationResultTypeDef:
    return {
        "DataSetId": ...,
    }


# AnalyticsDataAssociationResultTypeDef definition

class AnalyticsDataAssociationResultTypeDef(TypedDict):
    DataSetId: NotRequired[str],
    TargetAccountId: NotRequired[str],
    ResourceShareId: NotRequired[str],
    ResourceShareArn: NotRequired[str],
    ResourceShareStatus: NotRequired[str],
```

## AnalyticsDataSetsResultTypeDef

```python
# AnalyticsDataSetsResultTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AnalyticsDataSetsResultTypeDef


def get_value() -> AnalyticsDataSetsResultTypeDef:
    return {
        "DataSetId": ...,
    }


# AnalyticsDataSetsResultTypeDef definition

class AnalyticsDataSetsResultTypeDef(TypedDict):
    DataSetId: NotRequired[str],
    DataSetName: NotRequired[str],
```

## AnswerMachineDetectionConfigTypeDef

```python
# AnswerMachineDetectionConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AnswerMachineDetectionConfigTypeDef


def get_value() -> AnswerMachineDetectionConfigTypeDef:
    return {
        "EnableAnswerMachineDetection": ...,
    }


# AnswerMachineDetectionConfigTypeDef definition

class AnswerMachineDetectionConfigTypeDef(TypedDict):
    EnableAnswerMachineDetection: NotRequired[bool],
    AwaitAnswerMachinePrompt: NotRequired[bool],
```

## ApplicationOutputTypeDef

```python
# ApplicationOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ApplicationOutputTypeDef


def get_value() -> ApplicationOutputTypeDef:
    return {
        "Namespace": ...,
    }


# ApplicationOutputTypeDef definition

class ApplicationOutputTypeDef(TypedDict):
    Namespace: NotRequired[str],
    ApplicationPermissions: NotRequired[List[str]],
```

## ApplicationTypeDef

```python
# ApplicationTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ApplicationTypeDef


def get_value() -> ApplicationTypeDef:
    return {
        "Namespace": ...,
    }


# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    Namespace: NotRequired[str],
    ApplicationPermissions: NotRequired[Sequence[str]],
```

## AssociateAnalyticsDataSetRequestTypeDef

```python
# AssociateAnalyticsDataSetRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateAnalyticsDataSetRequestTypeDef


def get_value() -> AssociateAnalyticsDataSetRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# AssociateAnalyticsDataSetRequestTypeDef definition

class AssociateAnalyticsDataSetRequestTypeDef(TypedDict):
    InstanceId: str,
    DataSetId: str,
    TargetAccountId: NotRequired[str],
```

## AssociateApprovedOriginRequestTypeDef

```python
# AssociateApprovedOriginRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateApprovedOriginRequestTypeDef


def get_value() -> AssociateApprovedOriginRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# AssociateApprovedOriginRequestTypeDef definition

class AssociateApprovedOriginRequestTypeDef(TypedDict):
    InstanceId: str,
    Origin: str,
    ClientToken: NotRequired[str],
```

## LexBotTypeDef

```python
# LexBotTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import LexBotTypeDef


def get_value() -> LexBotTypeDef:
    return {
        "Name": ...,
    }


# LexBotTypeDef definition

class LexBotTypeDef(TypedDict):
    Name: str,
    LexRegion: str,
```

## LexV2BotTypeDef

```python
# LexV2BotTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import LexV2BotTypeDef


def get_value() -> LexV2BotTypeDef:
    return {
        "AliasArn": ...,
    }


# LexV2BotTypeDef definition

class LexV2BotTypeDef(TypedDict):
    AliasArn: NotRequired[str],
```

## AssociateDefaultVocabularyRequestTypeDef

```python
# AssociateDefaultVocabularyRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateDefaultVocabularyRequestTypeDef


def get_value() -> AssociateDefaultVocabularyRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# AssociateDefaultVocabularyRequestTypeDef definition

class AssociateDefaultVocabularyRequestTypeDef(TypedDict):
    InstanceId: str,
    LanguageCode: VocabularyLanguageCodeType,  # (1)
    VocabularyId: NotRequired[str],
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
## AssociateFlowRequestTypeDef

```python
# AssociateFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateFlowRequestTypeDef


def get_value() -> AssociateFlowRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# AssociateFlowRequestTypeDef definition

class AssociateFlowRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceId: str,
    FlowId: str,
    ResourceType: FlowAssociationResourceTypeType,  # (1)
```

1. See [:material-code-brackets: FlowAssociationResourceTypeType](./literals.md#flowassociationresourcetypetype) 
## AssociateLambdaFunctionRequestTypeDef

```python
# AssociateLambdaFunctionRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateLambdaFunctionRequestTypeDef


def get_value() -> AssociateLambdaFunctionRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# AssociateLambdaFunctionRequestTypeDef definition

class AssociateLambdaFunctionRequestTypeDef(TypedDict):
    InstanceId: str,
    FunctionArn: str,
    ClientToken: NotRequired[str],
```

## AssociatePhoneNumberContactFlowRequestTypeDef

```python
# AssociatePhoneNumberContactFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociatePhoneNumberContactFlowRequestTypeDef


def get_value() -> AssociatePhoneNumberContactFlowRequestTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# AssociatePhoneNumberContactFlowRequestTypeDef definition

class AssociatePhoneNumberContactFlowRequestTypeDef(TypedDict):
    PhoneNumberId: str,
    InstanceId: str,
    ContactFlowId: str,
```

## AssociateQueueQuickConnectsRequestTypeDef

```python
# AssociateQueueQuickConnectsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateQueueQuickConnectsRequestTypeDef


def get_value() -> AssociateQueueQuickConnectsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# AssociateQueueQuickConnectsRequestTypeDef definition

class AssociateQueueQuickConnectsRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    QuickConnectIds: Sequence[str],
```

## AssociateSecurityKeyRequestTypeDef

```python
# AssociateSecurityKeyRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateSecurityKeyRequestTypeDef


def get_value() -> AssociateSecurityKeyRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# AssociateSecurityKeyRequestTypeDef definition

class AssociateSecurityKeyRequestTypeDef(TypedDict):
    InstanceId: str,
    Key: str,
    ClientToken: NotRequired[str],
```

## AssociateTrafficDistributionGroupUserRequestTypeDef

```python
# AssociateTrafficDistributionGroupUserRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateTrafficDistributionGroupUserRequestTypeDef


def get_value() -> AssociateTrafficDistributionGroupUserRequestTypeDef:
    return {
        "TrafficDistributionGroupId": ...,
    }


# AssociateTrafficDistributionGroupUserRequestTypeDef definition

class AssociateTrafficDistributionGroupUserRequestTypeDef(TypedDict):
    TrafficDistributionGroupId: str,
    UserId: str,
    InstanceId: str,
```

## UserProficiencyTypeDef

```python
# UserProficiencyTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserProficiencyTypeDef


def get_value() -> UserProficiencyTypeDef:
    return {
        "AttributeName": ...,
    }


# UserProficiencyTypeDef definition

class UserProficiencyTypeDef(TypedDict):
    AttributeName: str,
    AttributeValue: str,
    Level: float,
```

## AssociatedContactSummaryTypeDef

```python
# AssociatedContactSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociatedContactSummaryTypeDef


def get_value() -> AssociatedContactSummaryTypeDef:
    return {
        "ContactId": ...,
    }


# AssociatedContactSummaryTypeDef definition

class AssociatedContactSummaryTypeDef(TypedDict):
    ContactId: NotRequired[str],
    ContactArn: NotRequired[str],
    InitiationTimestamp: NotRequired[datetime],
    DisconnectTimestamp: NotRequired[datetime],
    InitialContactId: NotRequired[str],
    PreviousContactId: NotRequired[str],
    RelatedContactId: NotRequired[str],
    InitiationMethod: NotRequired[ContactInitiationMethodType],  # (1)
    Channel: NotRequired[ChannelType],  # (2)
```

1. See [:material-code-brackets: ContactInitiationMethodType](./literals.md#contactinitiationmethodtype) 
2. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
## AttachedFileErrorTypeDef

```python
# AttachedFileErrorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AttachedFileErrorTypeDef


def get_value() -> AttachedFileErrorTypeDef:
    return {
        "ErrorCode": ...,
    }


# AttachedFileErrorTypeDef definition

class AttachedFileErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
    FileId: NotRequired[str],
```

## CreatedByInfoTypeDef

```python
# CreatedByInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreatedByInfoTypeDef


def get_value() -> CreatedByInfoTypeDef:
    return {
        "ConnectUserArn": ...,
    }


# CreatedByInfoTypeDef definition

class CreatedByInfoTypeDef(TypedDict):
    ConnectUserArn: NotRequired[str],
    AWSIdentityArn: NotRequired[str],
```

## AttachmentReferenceTypeDef

```python
# AttachmentReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AttachmentReferenceTypeDef


def get_value() -> AttachmentReferenceTypeDef:
    return {
        "Name": ...,
    }


# AttachmentReferenceTypeDef definition

class AttachmentReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
    Status: NotRequired[ReferenceStatusType],  # (1)
    Arn: NotRequired[str],
```

1. See [:material-code-brackets: ReferenceStatusType](./literals.md#referencestatustype) 
## AttendeeTypeDef

```python
# AttendeeTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AttendeeTypeDef


def get_value() -> AttendeeTypeDef:
    return {
        "AttendeeId": ...,
    }


# AttendeeTypeDef definition

class AttendeeTypeDef(TypedDict):
    AttendeeId: NotRequired[str],
    JoinToken: NotRequired[str],
```

## HierarchyGroupConditionTypeDef

```python
# HierarchyGroupConditionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HierarchyGroupConditionTypeDef


def get_value() -> HierarchyGroupConditionTypeDef:
    return {
        "Value": ...,
    }


# HierarchyGroupConditionTypeDef definition

class HierarchyGroupConditionTypeDef(TypedDict):
    Value: NotRequired[str],
    HierarchyGroupMatchType: NotRequired[HierarchyGroupMatchTypeType],  # (1)
```

1. See [:material-code-brackets: HierarchyGroupMatchTypeType](./literals.md#hierarchygroupmatchtypetype) 
## TagConditionTypeDef

```python
# TagConditionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TagConditionTypeDef


def get_value() -> TagConditionTypeDef:
    return {
        "TagKey": ...,
    }


# TagConditionTypeDef definition

class TagConditionTypeDef(TypedDict):
    TagKey: NotRequired[str],
    TagValue: NotRequired[str],
```

## RangeTypeDef

```python
# RangeTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RangeTypeDef


def get_value() -> RangeTypeDef:
    return {
        "MinProficiencyLevel": ...,
    }


# RangeTypeDef definition

class RangeTypeDef(TypedDict):
    MinProficiencyLevel: NotRequired[float],
    MaxProficiencyLevel: NotRequired[float],
```

## AttributeTypeDef

```python
# AttributeTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AttributeTypeDef


def get_value() -> AttributeTypeDef:
    return {
        "AttributeType": ...,
    }


# AttributeTypeDef definition

class AttributeTypeDef(TypedDict):
    AttributeType: NotRequired[InstanceAttributeTypeType],  # (1)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: InstanceAttributeTypeType](./literals.md#instanceattributetypetype) 
## AudioFeaturesTypeDef

```python
# AudioFeaturesTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AudioFeaturesTypeDef


def get_value() -> AudioFeaturesTypeDef:
    return {
        "EchoReduction": ...,
    }


# AudioFeaturesTypeDef definition

class AudioFeaturesTypeDef(TypedDict):
    EchoReduction: NotRequired[MeetingFeatureStatusType],  # (1)
```

1. See [:material-code-brackets: MeetingFeatureStatusType](./literals.md#meetingfeaturestatustype) 
## AuthenticationProfileSummaryTypeDef

```python
# AuthenticationProfileSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AuthenticationProfileSummaryTypeDef


def get_value() -> AuthenticationProfileSummaryTypeDef:
    return {
        "Id": ...,
    }


# AuthenticationProfileSummaryTypeDef definition

class AuthenticationProfileSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    IsDefault: NotRequired[bool],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## AuthenticationProfileTypeDef

```python
# AuthenticationProfileTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AuthenticationProfileTypeDef


def get_value() -> AuthenticationProfileTypeDef:
    return {
        "Id": ...,
    }


# AuthenticationProfileTypeDef definition

class AuthenticationProfileTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    AllowedIps: NotRequired[List[str]],
    BlockedIps: NotRequired[List[str]],
    IsDefault: NotRequired[bool],
    CreatedTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
    PeriodicSessionDuration: NotRequired[int],
    MaxSessionDuration: NotRequired[int],
```

## AvailableNumberSummaryTypeDef

```python
# AvailableNumberSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AvailableNumberSummaryTypeDef


def get_value() -> AvailableNumberSummaryTypeDef:
    return {
        "PhoneNumber": ...,
    }


# AvailableNumberSummaryTypeDef definition

class AvailableNumberSummaryTypeDef(TypedDict):
    PhoneNumber: NotRequired[str],
    PhoneNumberCountryCode: NotRequired[PhoneNumberCountryCodeType],  # (1)
    PhoneNumberType: NotRequired[PhoneNumberTypeType],  # (2)
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
## BatchAssociateAnalyticsDataSetRequestTypeDef

```python
# BatchAssociateAnalyticsDataSetRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import BatchAssociateAnalyticsDataSetRequestTypeDef


def get_value() -> BatchAssociateAnalyticsDataSetRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# BatchAssociateAnalyticsDataSetRequestTypeDef definition

class BatchAssociateAnalyticsDataSetRequestTypeDef(TypedDict):
    InstanceId: str,
    DataSetIds: Sequence[str],
    TargetAccountId: NotRequired[str],
```

## ErrorResultTypeDef

```python
# ErrorResultTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ErrorResultTypeDef


def get_value() -> ErrorResultTypeDef:
    return {
        "ErrorCode": ...,
    }


# ErrorResultTypeDef definition

class ErrorResultTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## BatchDisassociateAnalyticsDataSetRequestTypeDef

```python
# BatchDisassociateAnalyticsDataSetRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import BatchDisassociateAnalyticsDataSetRequestTypeDef


def get_value() -> BatchDisassociateAnalyticsDataSetRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# BatchDisassociateAnalyticsDataSetRequestTypeDef definition

class BatchDisassociateAnalyticsDataSetRequestTypeDef(TypedDict):
    InstanceId: str,
    DataSetIds: Sequence[str],
    TargetAccountId: NotRequired[str],
```

## BatchGetAttachedFileMetadataRequestTypeDef

```python
# BatchGetAttachedFileMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import BatchGetAttachedFileMetadataRequestTypeDef


def get_value() -> BatchGetAttachedFileMetadataRequestTypeDef:
    return {
        "FileIds": ...,
    }


# BatchGetAttachedFileMetadataRequestTypeDef definition

class BatchGetAttachedFileMetadataRequestTypeDef(TypedDict):
    FileIds: Sequence[str],
    InstanceId: str,
    AssociatedResourceArn: str,
```

## BatchGetFlowAssociationRequestTypeDef

```python
# BatchGetFlowAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import BatchGetFlowAssociationRequestTypeDef


def get_value() -> BatchGetFlowAssociationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# BatchGetFlowAssociationRequestTypeDef definition

class BatchGetFlowAssociationRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceIds: Sequence[str],
    ResourceType: NotRequired[ListFlowAssociationResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ListFlowAssociationResourceTypeType](./literals.md#listflowassociationresourcetypetype) 
## FlowAssociationSummaryTypeDef

```python
# FlowAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import FlowAssociationSummaryTypeDef


def get_value() -> FlowAssociationSummaryTypeDef:
    return {
        "ResourceId": ...,
    }


# FlowAssociationSummaryTypeDef definition

class FlowAssociationSummaryTypeDef(TypedDict):
    ResourceId: NotRequired[str],
    FlowId: NotRequired[str],
    ResourceType: NotRequired[ListFlowAssociationResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ListFlowAssociationResourceTypeType](./literals.md#listflowassociationresourcetypetype) 
## FailedRequestTypeDef

```python
# FailedRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import FailedRequestTypeDef


def get_value() -> FailedRequestTypeDef:
    return {
        "RequestIdentifier": ...,
    }


# FailedRequestTypeDef definition

class FailedRequestTypeDef(TypedDict):
    RequestIdentifier: NotRequired[str],
    FailureReasonCode: NotRequired[FailureReasonCodeType],  # (1)
    FailureReasonMessage: NotRequired[str],
```

1. See [:material-code-brackets: FailureReasonCodeType](./literals.md#failurereasoncodetype) 
## SuccessfulRequestTypeDef

```python
# SuccessfulRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SuccessfulRequestTypeDef


def get_value() -> SuccessfulRequestTypeDef:
    return {
        "RequestIdentifier": ...,
    }


# SuccessfulRequestTypeDef definition

class SuccessfulRequestTypeDef(TypedDict):
    RequestIdentifier: NotRequired[str],
    ContactId: NotRequired[str],
```

## CampaignTypeDef

```python
# CampaignTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CampaignTypeDef


def get_value() -> CampaignTypeDef:
    return {
        "CampaignId": ...,
    }


# CampaignTypeDef definition

class CampaignTypeDef(TypedDict):
    CampaignId: NotRequired[str],
```

## ChatEventTypeDef

```python
# ChatEventTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ChatEventTypeDef


def get_value() -> ChatEventTypeDef:
    return {
        "Type": ...,
    }


# ChatEventTypeDef definition

class ChatEventTypeDef(TypedDict):
    Type: ChatEventTypeType,  # (1)
    ContentType: NotRequired[str],
    Content: NotRequired[str],
```

1. See [:material-code-brackets: ChatEventTypeType](./literals.md#chateventtypetype) 
## ChatMessageTypeDef

```python
# ChatMessageTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ChatMessageTypeDef


def get_value() -> ChatMessageTypeDef:
    return {
        "ContentType": ...,
    }


# ChatMessageTypeDef definition

class ChatMessageTypeDef(TypedDict):
    ContentType: str,
    Content: str,
```

## ChatStreamingConfigurationTypeDef

```python
# ChatStreamingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ChatStreamingConfigurationTypeDef


def get_value() -> ChatStreamingConfigurationTypeDef:
    return {
        "StreamingEndpointArn": ...,
    }


# ChatStreamingConfigurationTypeDef definition

class ChatStreamingConfigurationTypeDef(TypedDict):
    StreamingEndpointArn: str,
```

## ClaimPhoneNumberRequestTypeDef

```python
# ClaimPhoneNumberRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ClaimPhoneNumberRequestTypeDef


def get_value() -> ClaimPhoneNumberRequestTypeDef:
    return {
        "PhoneNumber": ...,
    }


# ClaimPhoneNumberRequestTypeDef definition

class ClaimPhoneNumberRequestTypeDef(TypedDict):
    PhoneNumber: str,
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    PhoneNumberDescription: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    ClientToken: NotRequired[str],
```

## PhoneNumberStatusTypeDef

```python
# PhoneNumberStatusTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PhoneNumberStatusTypeDef


def get_value() -> PhoneNumberStatusTypeDef:
    return {
        "Status": ...,
    }


# PhoneNumberStatusTypeDef definition

class PhoneNumberStatusTypeDef(TypedDict):
    Status: NotRequired[PhoneNumberWorkflowStatusType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberWorkflowStatusType](./literals.md#phonenumberworkflowstatustype) 
## CompleteAttachedFileUploadRequestTypeDef

```python
# CompleteAttachedFileUploadRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CompleteAttachedFileUploadRequestTypeDef


def get_value() -> CompleteAttachedFileUploadRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CompleteAttachedFileUploadRequestTypeDef definition

class CompleteAttachedFileUploadRequestTypeDef(TypedDict):
    InstanceId: str,
    FileId: str,
    AssociatedResourceArn: str,
```

## NumberConditionTypeDef

```python
# NumberConditionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import NumberConditionTypeDef


def get_value() -> NumberConditionTypeDef:
    return {
        "FieldName": ...,
    }


# NumberConditionTypeDef definition

class NumberConditionTypeDef(TypedDict):
    FieldName: NotRequired[str],
    MinValue: NotRequired[int],
    MaxValue: NotRequired[int],
    ComparisonType: NotRequired[NumberComparisonTypeType],  # (1)
```

1. See [:material-code-brackets: NumberComparisonTypeType](./literals.md#numbercomparisontypetype) 
## ContactConfigurationTypeDef

```python
# ContactConfigurationTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactConfigurationTypeDef


def get_value() -> ContactConfigurationTypeDef:
    return {
        "ContactId": ...,
    }


# ContactConfigurationTypeDef definition

class ContactConfigurationTypeDef(TypedDict):
    ContactId: str,
    ParticipantRole: NotRequired[ParticipantRoleType],  # (1)
    IncludeRawMessage: NotRequired[bool],
```

1. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
## EndpointTypeDef

```python
# EndpointTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EndpointTypeDef


def get_value() -> EndpointTypeDef:
    return {
        "Type": ...,
    }


# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Type: NotRequired[EndpointTypeType],  # (1)
    Address: NotRequired[str],
```

1. See [:material-code-brackets: EndpointTypeType](./literals.md#endpointtypetype) 
## ContactFilterTypeDef

```python
# ContactFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactFilterTypeDef


def get_value() -> ContactFilterTypeDef:
    return {
        "ContactStates": ...,
    }


# ContactFilterTypeDef definition

class ContactFilterTypeDef(TypedDict):
    ContactStates: NotRequired[Sequence[ContactStateType]],  # (1)
```

1. See [:material-code-brackets: ContactStateType](./literals.md#contactstatetype) 
## ContactFlowModuleSummaryTypeDef

```python
# ContactFlowModuleSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactFlowModuleSummaryTypeDef


def get_value() -> ContactFlowModuleSummaryTypeDef:
    return {
        "Id": ...,
    }


# ContactFlowModuleSummaryTypeDef definition

class ContactFlowModuleSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    State: NotRequired[ContactFlowModuleStateType],  # (1)
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
## ContactFlowModuleTypeDef

```python
# ContactFlowModuleTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactFlowModuleTypeDef


def get_value() -> ContactFlowModuleTypeDef:
    return {
        "Arn": ...,
    }


# ContactFlowModuleTypeDef definition

class ContactFlowModuleTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    Content: NotRequired[str],
    Description: NotRequired[str],
    State: NotRequired[ContactFlowModuleStateType],  # (1)
    Status: NotRequired[ContactFlowModuleStatusType],  # (2)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
2. See [:material-code-brackets: ContactFlowModuleStatusType](./literals.md#contactflowmodulestatustype) 
## ContactFlowSummaryTypeDef

```python
# ContactFlowSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactFlowSummaryTypeDef


def get_value() -> ContactFlowSummaryTypeDef:
    return {
        "Id": ...,
    }


# ContactFlowSummaryTypeDef definition

class ContactFlowSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    ContactFlowType: NotRequired[ContactFlowTypeType],  # (1)
    ContactFlowState: NotRequired[ContactFlowStateType],  # (2)
    ContactFlowStatus: NotRequired[ContactFlowStatusType],  # (3)
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
2. See [:material-code-brackets: ContactFlowStateType](./literals.md#contactflowstatetype) 
3. See [:material-code-brackets: ContactFlowStatusType](./literals.md#contactflowstatustype) 
## ContactFlowTypeDef

```python
# ContactFlowTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactFlowTypeDef


def get_value() -> ContactFlowTypeDef:
    return {
        "Arn": ...,
    }


# ContactFlowTypeDef definition

class ContactFlowTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[ContactFlowTypeType],  # (1)
    State: NotRequired[ContactFlowStateType],  # (2)
    Status: NotRequired[ContactFlowStatusType],  # (3)
    Description: NotRequired[str],
    Content: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    FlowContentSha256: NotRequired[str],
    Version: NotRequired[int],
    VersionDescription: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
2. See [:material-code-brackets: ContactFlowStateType](./literals.md#contactflowstatetype) 
3. See [:material-code-brackets: ContactFlowStatusType](./literals.md#contactflowstatustype) 
## ContactFlowVersionSummaryTypeDef

```python
# ContactFlowVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactFlowVersionSummaryTypeDef


def get_value() -> ContactFlowVersionSummaryTypeDef:
    return {
        "Arn": ...,
    }


# ContactFlowVersionSummaryTypeDef definition

class ContactFlowVersionSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    VersionDescription: NotRequired[str],
    Version: NotRequired[int],
```

## ContactSearchSummaryAgentInfoTypeDef

```python
# ContactSearchSummaryAgentInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactSearchSummaryAgentInfoTypeDef


def get_value() -> ContactSearchSummaryAgentInfoTypeDef:
    return {
        "Id": ...,
    }


# ContactSearchSummaryAgentInfoTypeDef definition

class ContactSearchSummaryAgentInfoTypeDef(TypedDict):
    Id: NotRequired[str],
    ConnectedToAgentTimestamp: NotRequired[datetime],
```

## ContactSearchSummaryQueueInfoTypeDef

```python
# ContactSearchSummaryQueueInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactSearchSummaryQueueInfoTypeDef


def get_value() -> ContactSearchSummaryQueueInfoTypeDef:
    return {
        "Id": ...,
    }


# ContactSearchSummaryQueueInfoTypeDef definition

class ContactSearchSummaryQueueInfoTypeDef(TypedDict):
    Id: NotRequired[str],
    EnqueueTimestamp: NotRequired[datetime],
```

## ContactSearchSummarySegmentAttributeValueTypeDef

```python
# ContactSearchSummarySegmentAttributeValueTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactSearchSummarySegmentAttributeValueTypeDef


def get_value() -> ContactSearchSummarySegmentAttributeValueTypeDef:
    return {
        "ValueString": ...,
    }


# ContactSearchSummarySegmentAttributeValueTypeDef definition

class ContactSearchSummarySegmentAttributeValueTypeDef(TypedDict):
    ValueString: NotRequired[str],
```

## CustomerVoiceActivityTypeDef

```python
# CustomerVoiceActivityTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CustomerVoiceActivityTypeDef


def get_value() -> CustomerVoiceActivityTypeDef:
    return {
        "GreetingStartTimestamp": ...,
    }


# CustomerVoiceActivityTypeDef definition

class CustomerVoiceActivityTypeDef(TypedDict):
    GreetingStartTimestamp: NotRequired[datetime],
    GreetingEndTimestamp: NotRequired[datetime],
```

## DisconnectDetailsTypeDef

```python
# DisconnectDetailsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisconnectDetailsTypeDef


def get_value() -> DisconnectDetailsTypeDef:
    return {
        "PotentialDisconnectIssue": ...,
    }


# DisconnectDetailsTypeDef definition

class DisconnectDetailsTypeDef(TypedDict):
    PotentialDisconnectIssue: NotRequired[str],
```

## EndpointInfoTypeDef

```python
# EndpointInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EndpointInfoTypeDef


def get_value() -> EndpointInfoTypeDef:
    return {
        "Type": ...,
    }


# EndpointInfoTypeDef definition

class EndpointInfoTypeDef(TypedDict):
    Type: NotRequired[EndpointTypeType],  # (1)
    Address: NotRequired[str],
    DisplayName: NotRequired[str],
```

1. See [:material-code-brackets: EndpointTypeType](./literals.md#endpointtypetype) 
## QueueInfoTypeDef

```python
# QueueInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QueueInfoTypeDef


def get_value() -> QueueInfoTypeDef:
    return {
        "Id": ...,
    }


# QueueInfoTypeDef definition

class QueueInfoTypeDef(TypedDict):
    Id: NotRequired[str],
    EnqueueTimestamp: NotRequired[datetime],
```

## SegmentAttributeValueOutputTypeDef

```python
# SegmentAttributeValueOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SegmentAttributeValueOutputTypeDef


def get_value() -> SegmentAttributeValueOutputTypeDef:
    return {
        "ValueString": ...,
    }


# SegmentAttributeValueOutputTypeDef definition

class SegmentAttributeValueOutputTypeDef(TypedDict):
    ValueString: NotRequired[str],
    ValueMap: NotRequired[Dict[str, Dict[str, Any]]],
    ValueInteger: NotRequired[int],
```

## WisdomInfoTypeDef

```python
# WisdomInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import WisdomInfoTypeDef


def get_value() -> WisdomInfoTypeDef:
    return {
        "SessionArn": ...,
    }


# WisdomInfoTypeDef definition

class WisdomInfoTypeDef(TypedDict):
    SessionArn: NotRequired[str],
```

## CreateAgentStatusRequestTypeDef

```python
# CreateAgentStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateAgentStatusRequestTypeDef


def get_value() -> CreateAgentStatusRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateAgentStatusRequestTypeDef definition

class CreateAgentStatusRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    State: AgentStatusStateType,  # (1)
    Description: NotRequired[str],
    DisplayOrder: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AgentStatusStateType](./literals.md#agentstatusstatetype) 
## CreateContactFlowModuleRequestTypeDef

```python
# CreateContactFlowModuleRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateContactFlowModuleRequestTypeDef


def get_value() -> CreateContactFlowModuleRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateContactFlowModuleRequestTypeDef definition

class CreateContactFlowModuleRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    Content: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    ClientToken: NotRequired[str],
```

## CreateContactFlowRequestTypeDef

```python
# CreateContactFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateContactFlowRequestTypeDef


def get_value() -> CreateContactFlowRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateContactFlowRequestTypeDef definition

class CreateContactFlowRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    Type: ContactFlowTypeType,  # (1)
    Content: str,
    Description: NotRequired[str],
    Status: NotRequired[ContactFlowStatusType],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
2. See [:material-code-brackets: ContactFlowStatusType](./literals.md#contactflowstatustype) 
## ReferenceTypeDef

```python
# ReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ReferenceTypeDef


def get_value() -> ReferenceTypeDef:
    return {
        "Value": ...,
    }


# ReferenceTypeDef definition

class ReferenceTypeDef(TypedDict):
    Type: ReferenceTypeType,  # (1)
    Value: NotRequired[str],
    Status: NotRequired[ReferenceStatusType],  # (2)
    Arn: NotRequired[str],
    StatusReason: NotRequired[str],
```

1. See [:material-code-brackets: ReferenceTypeType](./literals.md#referencetypetype) 
2. See [:material-code-brackets: ReferenceStatusType](./literals.md#referencestatustype) 
## UserInfoTypeDef

```python
# UserInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserInfoTypeDef


def get_value() -> UserInfoTypeDef:
    return {
        "UserId": ...,
    }


# UserInfoTypeDef definition

class UserInfoTypeDef(TypedDict):
    UserId: NotRequired[str],
```

## CreateEmailAddressRequestTypeDef

```python
# CreateEmailAddressRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateEmailAddressRequestTypeDef


def get_value() -> CreateEmailAddressRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateEmailAddressRequestTypeDef definition

class CreateEmailAddressRequestTypeDef(TypedDict):
    InstanceId: str,
    EmailAddress: str,
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    ClientToken: NotRequired[str],
```

## EvaluationFormScoringStrategyTypeDef

```python
# EvaluationFormScoringStrategyTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormScoringStrategyTypeDef


def get_value() -> EvaluationFormScoringStrategyTypeDef:
    return {
        "Mode": ...,
    }


# EvaluationFormScoringStrategyTypeDef definition

class EvaluationFormScoringStrategyTypeDef(TypedDict):
    Mode: EvaluationFormScoringModeType,  # (1)
    Status: EvaluationFormScoringStatusType,  # (2)
```

1. See [:material-code-brackets: EvaluationFormScoringModeType](./literals.md#evaluationformscoringmodetype) 
2. See [:material-code-brackets: EvaluationFormScoringStatusType](./literals.md#evaluationformscoringstatustype) 
## CreateInstanceRequestTypeDef

```python
# CreateInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateInstanceRequestTypeDef


def get_value() -> CreateInstanceRequestTypeDef:
    return {
        "IdentityManagementType": ...,
    }


# CreateInstanceRequestTypeDef definition

class CreateInstanceRequestTypeDef(TypedDict):
    IdentityManagementType: DirectoryTypeType,  # (1)
    InboundCallsEnabled: bool,
    OutboundCallsEnabled: bool,
    ClientToken: NotRequired[str],
    InstanceAlias: NotRequired[str],
    DirectoryId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DirectoryTypeType](./literals.md#directorytypetype) 
## CreateIntegrationAssociationRequestTypeDef

```python
# CreateIntegrationAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateIntegrationAssociationRequestTypeDef


def get_value() -> CreateIntegrationAssociationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateIntegrationAssociationRequestTypeDef definition

class CreateIntegrationAssociationRequestTypeDef(TypedDict):
    InstanceId: str,
    IntegrationType: IntegrationTypeType,  # (1)
    IntegrationArn: str,
    SourceApplicationUrl: NotRequired[str],
    SourceApplicationName: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## ParticipantDetailsToAddTypeDef

```python
# ParticipantDetailsToAddTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ParticipantDetailsToAddTypeDef


def get_value() -> ParticipantDetailsToAddTypeDef:
    return {
        "ParticipantRole": ...,
    }


# ParticipantDetailsToAddTypeDef definition

class ParticipantDetailsToAddTypeDef(TypedDict):
    ParticipantRole: NotRequired[ParticipantRoleType],  # (1)
    DisplayName: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
## ParticipantTokenCredentialsTypeDef

```python
# ParticipantTokenCredentialsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ParticipantTokenCredentialsTypeDef


def get_value() -> ParticipantTokenCredentialsTypeDef:
    return {
        "ParticipantToken": ...,
    }


# ParticipantTokenCredentialsTypeDef definition

class ParticipantTokenCredentialsTypeDef(TypedDict):
    ParticipantToken: NotRequired[str],
    Expiry: NotRequired[str],
```

## CreatePersistentContactAssociationRequestTypeDef

```python
# CreatePersistentContactAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreatePersistentContactAssociationRequestTypeDef


def get_value() -> CreatePersistentContactAssociationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreatePersistentContactAssociationRequestTypeDef definition

class CreatePersistentContactAssociationRequestTypeDef(TypedDict):
    InstanceId: str,
    InitialContactId: str,
    RehydrationType: RehydrationTypeType,  # (1)
    SourceContactId: str,
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: RehydrationTypeType](./literals.md#rehydrationtypetype) 
## CreatePromptRequestTypeDef

```python
# CreatePromptRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreatePromptRequestTypeDef


def get_value() -> CreatePromptRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreatePromptRequestTypeDef definition

class CreatePromptRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    S3Uri: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## OutboundCallerConfigTypeDef

```python
# OutboundCallerConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import OutboundCallerConfigTypeDef


def get_value() -> OutboundCallerConfigTypeDef:
    return {
        "OutboundCallerIdName": ...,
    }


# OutboundCallerConfigTypeDef definition

class OutboundCallerConfigTypeDef(TypedDict):
    OutboundCallerIdName: NotRequired[str],
    OutboundCallerIdNumberId: NotRequired[str],
    OutboundFlowId: NotRequired[str],
```

## OutboundEmailConfigTypeDef

```python
# OutboundEmailConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import OutboundEmailConfigTypeDef


def get_value() -> OutboundEmailConfigTypeDef:
    return {
        "OutboundEmailAddressId": ...,
    }


# OutboundEmailConfigTypeDef definition

class OutboundEmailConfigTypeDef(TypedDict):
    OutboundEmailAddressId: NotRequired[str],
```

## RuleTriggerEventSourceTypeDef

```python
# RuleTriggerEventSourceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RuleTriggerEventSourceTypeDef


def get_value() -> RuleTriggerEventSourceTypeDef:
    return {
        "EventSourceName": ...,
    }


# RuleTriggerEventSourceTypeDef definition

class RuleTriggerEventSourceTypeDef(TypedDict):
    EventSourceName: EventSourceNameType,  # (1)
    IntegrationAssociationId: NotRequired[str],
```

1. See [:material-code-brackets: EventSourceNameType](./literals.md#eventsourcenametype) 
## CreateTrafficDistributionGroupRequestTypeDef

```python
# CreateTrafficDistributionGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateTrafficDistributionGroupRequestTypeDef


def get_value() -> CreateTrafficDistributionGroupRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateTrafficDistributionGroupRequestTypeDef definition

class CreateTrafficDistributionGroupRequestTypeDef(TypedDict):
    Name: str,
    InstanceId: str,
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## CreateUseCaseRequestTypeDef

```python
# CreateUseCaseRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateUseCaseRequestTypeDef


def get_value() -> CreateUseCaseRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateUseCaseRequestTypeDef definition

class CreateUseCaseRequestTypeDef(TypedDict):
    InstanceId: str,
    IntegrationAssociationId: str,
    UseCaseType: UseCaseTypeType,  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: UseCaseTypeType](./literals.md#usecasetypetype) 
## CreateUserHierarchyGroupRequestTypeDef

```python
# CreateUserHierarchyGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateUserHierarchyGroupRequestTypeDef


def get_value() -> CreateUserHierarchyGroupRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateUserHierarchyGroupRequestTypeDef definition

class CreateUserHierarchyGroupRequestTypeDef(TypedDict):
    Name: str,
    InstanceId: str,
    ParentGroupId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## UserIdentityInfoTypeDef

```python
# UserIdentityInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserIdentityInfoTypeDef


def get_value() -> UserIdentityInfoTypeDef:
    return {
        "FirstName": ...,
    }


# UserIdentityInfoTypeDef definition

class UserIdentityInfoTypeDef(TypedDict):
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    Email: NotRequired[str],
    SecondaryEmail: NotRequired[str],
    Mobile: NotRequired[str],
```

## UserPhoneConfigTypeDef

```python
# UserPhoneConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserPhoneConfigTypeDef


def get_value() -> UserPhoneConfigTypeDef:
    return {
        "PhoneType": ...,
    }


# UserPhoneConfigTypeDef definition

class UserPhoneConfigTypeDef(TypedDict):
    PhoneType: PhoneTypeType,  # (1)
    AutoAccept: NotRequired[bool],
    AfterContactWorkTimeLimit: NotRequired[int],
    DeskPhoneNumber: NotRequired[str],
```

1. See [:material-code-brackets: PhoneTypeType](./literals.md#phonetypetype) 
## ViewInputContentTypeDef

```python
# ViewInputContentTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ViewInputContentTypeDef


def get_value() -> ViewInputContentTypeDef:
    return {
        "Template": ...,
    }


# ViewInputContentTypeDef definition

class ViewInputContentTypeDef(TypedDict):
    Template: NotRequired[str],
    Actions: NotRequired[Sequence[str]],
```

## CreateViewVersionRequestTypeDef

```python
# CreateViewVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateViewVersionRequestTypeDef


def get_value() -> CreateViewVersionRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateViewVersionRequestTypeDef definition

class CreateViewVersionRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
    VersionDescription: NotRequired[str],
    ViewContentSha256: NotRequired[str],
```

## CreateVocabularyRequestTypeDef

```python
# CreateVocabularyRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateVocabularyRequestTypeDef


def get_value() -> CreateVocabularyRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateVocabularyRequestTypeDef definition

class CreateVocabularyRequestTypeDef(TypedDict):
    InstanceId: str,
    VocabularyName: str,
    LanguageCode: VocabularyLanguageCodeType,  # (1)
    Content: str,
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
## CredentialsTypeDef

```python
# CredentialsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CredentialsTypeDef


def get_value() -> CredentialsTypeDef:
    return {
        "AccessToken": ...,
    }


# CredentialsTypeDef definition

class CredentialsTypeDef(TypedDict):
    AccessToken: NotRequired[str],
    AccessTokenExpiration: NotRequired[datetime],
    RefreshToken: NotRequired[str],
    RefreshTokenExpiration: NotRequired[datetime],
```

## CrossChannelBehaviorTypeDef

```python
# CrossChannelBehaviorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CrossChannelBehaviorTypeDef


def get_value() -> CrossChannelBehaviorTypeDef:
    return {
        "BehaviorType": ...,
    }


# CrossChannelBehaviorTypeDef definition

class CrossChannelBehaviorTypeDef(TypedDict):
    BehaviorType: BehaviorTypeType,  # (1)
```

1. See [:material-code-brackets: BehaviorTypeType](./literals.md#behaviortypetype) 
## CurrentMetricTypeDef

```python
# CurrentMetricTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CurrentMetricTypeDef


def get_value() -> CurrentMetricTypeDef:
    return {
        "Name": ...,
    }


# CurrentMetricTypeDef definition

class CurrentMetricTypeDef(TypedDict):
    Name: NotRequired[CurrentMetricNameType],  # (1)
    Unit: NotRequired[UnitType],  # (2)
```

1. See [:material-code-brackets: CurrentMetricNameType](./literals.md#currentmetricnametype) 
2. See [:material-code-brackets: UnitType](./literals.md#unittype) 
## CurrentMetricSortCriteriaTypeDef

```python
# CurrentMetricSortCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CurrentMetricSortCriteriaTypeDef


def get_value() -> CurrentMetricSortCriteriaTypeDef:
    return {
        "SortByMetric": ...,
    }


# CurrentMetricSortCriteriaTypeDef definition

class CurrentMetricSortCriteriaTypeDef(TypedDict):
    SortByMetric: NotRequired[CurrentMetricNameType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: CurrentMetricNameType](./literals.md#currentmetricnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## DateConditionTypeDef

```python
# DateConditionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DateConditionTypeDef


def get_value() -> DateConditionTypeDef:
    return {
        "FieldName": ...,
    }


# DateConditionTypeDef definition

class DateConditionTypeDef(TypedDict):
    FieldName: NotRequired[str],
    Value: NotRequired[str],
    ComparisonType: NotRequired[DateComparisonTypeType],  # (1)
```

1. See [:material-code-brackets: DateComparisonTypeType](./literals.md#datecomparisontypetype) 
## DateReferenceTypeDef

```python
# DateReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DateReferenceTypeDef


def get_value() -> DateReferenceTypeDef:
    return {
        "Name": ...,
    }


# DateReferenceTypeDef definition

class DateReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## DeactivateEvaluationFormRequestTypeDef

```python
# DeactivateEvaluationFormRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeactivateEvaluationFormRequestTypeDef


def get_value() -> DeactivateEvaluationFormRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeactivateEvaluationFormRequestTypeDef definition

class DeactivateEvaluationFormRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: int,
```

## DefaultVocabularyTypeDef

```python
# DefaultVocabularyTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DefaultVocabularyTypeDef


def get_value() -> DefaultVocabularyTypeDef:
    return {
        "InstanceId": ...,
    }


# DefaultVocabularyTypeDef definition

class DefaultVocabularyTypeDef(TypedDict):
    InstanceId: str,
    LanguageCode: VocabularyLanguageCodeType,  # (1)
    VocabularyId: str,
    VocabularyName: str,
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
## DeleteAttachedFileRequestTypeDef

```python
# DeleteAttachedFileRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteAttachedFileRequestTypeDef


def get_value() -> DeleteAttachedFileRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteAttachedFileRequestTypeDef definition

class DeleteAttachedFileRequestTypeDef(TypedDict):
    InstanceId: str,
    FileId: str,
    AssociatedResourceArn: str,
```

## DeleteContactEvaluationRequestTypeDef

```python
# DeleteContactEvaluationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteContactEvaluationRequestTypeDef


def get_value() -> DeleteContactEvaluationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteContactEvaluationRequestTypeDef definition

class DeleteContactEvaluationRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationId: str,
```

## DeleteContactFlowModuleRequestTypeDef

```python
# DeleteContactFlowModuleRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteContactFlowModuleRequestTypeDef


def get_value() -> DeleteContactFlowModuleRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteContactFlowModuleRequestTypeDef definition

class DeleteContactFlowModuleRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowModuleId: str,
```

## DeleteContactFlowRequestTypeDef

```python
# DeleteContactFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteContactFlowRequestTypeDef


def get_value() -> DeleteContactFlowRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteContactFlowRequestTypeDef definition

class DeleteContactFlowRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
```

## DeleteContactFlowVersionRequestTypeDef

```python
# DeleteContactFlowVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteContactFlowVersionRequestTypeDef


def get_value() -> DeleteContactFlowVersionRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteContactFlowVersionRequestTypeDef definition

class DeleteContactFlowVersionRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
    ContactFlowVersion: int,
```

## DeleteEmailAddressRequestTypeDef

```python
# DeleteEmailAddressRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteEmailAddressRequestTypeDef


def get_value() -> DeleteEmailAddressRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteEmailAddressRequestTypeDef definition

class DeleteEmailAddressRequestTypeDef(TypedDict):
    InstanceId: str,
    EmailAddressId: str,
```

## DeleteEvaluationFormRequestTypeDef

```python
# DeleteEvaluationFormRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteEvaluationFormRequestTypeDef


def get_value() -> DeleteEvaluationFormRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteEvaluationFormRequestTypeDef definition

class DeleteEvaluationFormRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: NotRequired[int],
```

## DeleteHoursOfOperationOverrideRequestTypeDef

```python
# DeleteHoursOfOperationOverrideRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteHoursOfOperationOverrideRequestTypeDef


def get_value() -> DeleteHoursOfOperationOverrideRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteHoursOfOperationOverrideRequestTypeDef definition

class DeleteHoursOfOperationOverrideRequestTypeDef(TypedDict):
    InstanceId: str,
    HoursOfOperationId: str,
    HoursOfOperationOverrideId: str,
```

## DeleteHoursOfOperationRequestTypeDef

```python
# DeleteHoursOfOperationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteHoursOfOperationRequestTypeDef


def get_value() -> DeleteHoursOfOperationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteHoursOfOperationRequestTypeDef definition

class DeleteHoursOfOperationRequestTypeDef(TypedDict):
    InstanceId: str,
    HoursOfOperationId: str,
```

## DeleteInstanceRequestTypeDef

```python
# DeleteInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteInstanceRequestTypeDef


def get_value() -> DeleteInstanceRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteInstanceRequestTypeDef definition

class DeleteInstanceRequestTypeDef(TypedDict):
    InstanceId: str,
    ClientToken: NotRequired[str],
```

## DeleteIntegrationAssociationRequestTypeDef

```python
# DeleteIntegrationAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteIntegrationAssociationRequestTypeDef


def get_value() -> DeleteIntegrationAssociationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteIntegrationAssociationRequestTypeDef definition

class DeleteIntegrationAssociationRequestTypeDef(TypedDict):
    InstanceId: str,
    IntegrationAssociationId: str,
```

## DeletePredefinedAttributeRequestTypeDef

```python
# DeletePredefinedAttributeRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeletePredefinedAttributeRequestTypeDef


def get_value() -> DeletePredefinedAttributeRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeletePredefinedAttributeRequestTypeDef definition

class DeletePredefinedAttributeRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
```

## DeletePromptRequestTypeDef

```python
# DeletePromptRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeletePromptRequestTypeDef


def get_value() -> DeletePromptRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeletePromptRequestTypeDef definition

class DeletePromptRequestTypeDef(TypedDict):
    InstanceId: str,
    PromptId: str,
```

## DeletePushNotificationRegistrationRequestTypeDef

```python
# DeletePushNotificationRegistrationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeletePushNotificationRegistrationRequestTypeDef


def get_value() -> DeletePushNotificationRegistrationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeletePushNotificationRegistrationRequestTypeDef definition

class DeletePushNotificationRegistrationRequestTypeDef(TypedDict):
    InstanceId: str,
    RegistrationId: str,
    ContactId: str,
```

## DeleteQueueRequestTypeDef

```python
# DeleteQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteQueueRequestTypeDef


def get_value() -> DeleteQueueRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteQueueRequestTypeDef definition

class DeleteQueueRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
```

## DeleteQuickConnectRequestTypeDef

```python
# DeleteQuickConnectRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteQuickConnectRequestTypeDef


def get_value() -> DeleteQuickConnectRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteQuickConnectRequestTypeDef definition

class DeleteQuickConnectRequestTypeDef(TypedDict):
    InstanceId: str,
    QuickConnectId: str,
```

## DeleteRoutingProfileRequestTypeDef

```python
# DeleteRoutingProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteRoutingProfileRequestTypeDef


def get_value() -> DeleteRoutingProfileRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteRoutingProfileRequestTypeDef definition

class DeleteRoutingProfileRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
```

## DeleteRuleRequestTypeDef

```python
# DeleteRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteRuleRequestTypeDef


def get_value() -> DeleteRuleRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteRuleRequestTypeDef definition

class DeleteRuleRequestTypeDef(TypedDict):
    InstanceId: str,
    RuleId: str,
```

## DeleteSecurityProfileRequestTypeDef

```python
# DeleteSecurityProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteSecurityProfileRequestTypeDef


def get_value() -> DeleteSecurityProfileRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteSecurityProfileRequestTypeDef definition

class DeleteSecurityProfileRequestTypeDef(TypedDict):
    InstanceId: str,
    SecurityProfileId: str,
```

## DeleteTaskTemplateRequestTypeDef

```python
# DeleteTaskTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteTaskTemplateRequestTypeDef


def get_value() -> DeleteTaskTemplateRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteTaskTemplateRequestTypeDef definition

class DeleteTaskTemplateRequestTypeDef(TypedDict):
    InstanceId: str,
    TaskTemplateId: str,
```

## DeleteTrafficDistributionGroupRequestTypeDef

```python
# DeleteTrafficDistributionGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteTrafficDistributionGroupRequestTypeDef


def get_value() -> DeleteTrafficDistributionGroupRequestTypeDef:
    return {
        "TrafficDistributionGroupId": ...,
    }


# DeleteTrafficDistributionGroupRequestTypeDef definition

class DeleteTrafficDistributionGroupRequestTypeDef(TypedDict):
    TrafficDistributionGroupId: str,
```

## DeleteUseCaseRequestTypeDef

```python
# DeleteUseCaseRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteUseCaseRequestTypeDef


def get_value() -> DeleteUseCaseRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteUseCaseRequestTypeDef definition

class DeleteUseCaseRequestTypeDef(TypedDict):
    InstanceId: str,
    IntegrationAssociationId: str,
    UseCaseId: str,
```

## DeleteUserHierarchyGroupRequestTypeDef

```python
# DeleteUserHierarchyGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteUserHierarchyGroupRequestTypeDef


def get_value() -> DeleteUserHierarchyGroupRequestTypeDef:
    return {
        "HierarchyGroupId": ...,
    }


# DeleteUserHierarchyGroupRequestTypeDef definition

class DeleteUserHierarchyGroupRequestTypeDef(TypedDict):
    HierarchyGroupId: str,
    InstanceId: str,
```

## DeleteUserRequestTypeDef

```python
# DeleteUserRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteUserRequestTypeDef


def get_value() -> DeleteUserRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteUserRequestTypeDef definition

class DeleteUserRequestTypeDef(TypedDict):
    InstanceId: str,
    UserId: str,
```

## DeleteViewRequestTypeDef

```python
# DeleteViewRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteViewRequestTypeDef


def get_value() -> DeleteViewRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteViewRequestTypeDef definition

class DeleteViewRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
```

## DeleteViewVersionRequestTypeDef

```python
# DeleteViewVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteViewVersionRequestTypeDef


def get_value() -> DeleteViewVersionRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteViewVersionRequestTypeDef definition

class DeleteViewVersionRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
    ViewVersion: int,
```

## DeleteVocabularyRequestTypeDef

```python
# DeleteVocabularyRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteVocabularyRequestTypeDef


def get_value() -> DeleteVocabularyRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteVocabularyRequestTypeDef definition

class DeleteVocabularyRequestTypeDef(TypedDict):
    InstanceId: str,
    VocabularyId: str,
```

## DescribeAgentStatusRequestTypeDef

```python
# DescribeAgentStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeAgentStatusRequestTypeDef


def get_value() -> DescribeAgentStatusRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeAgentStatusRequestTypeDef definition

class DescribeAgentStatusRequestTypeDef(TypedDict):
    InstanceId: str,
    AgentStatusId: str,
```

## DescribeAuthenticationProfileRequestTypeDef

```python
# DescribeAuthenticationProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeAuthenticationProfileRequestTypeDef


def get_value() -> DescribeAuthenticationProfileRequestTypeDef:
    return {
        "AuthenticationProfileId": ...,
    }


# DescribeAuthenticationProfileRequestTypeDef definition

class DescribeAuthenticationProfileRequestTypeDef(TypedDict):
    AuthenticationProfileId: str,
    InstanceId: str,
```

## DescribeContactEvaluationRequestTypeDef

```python
# DescribeContactEvaluationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeContactEvaluationRequestTypeDef


def get_value() -> DescribeContactEvaluationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeContactEvaluationRequestTypeDef definition

class DescribeContactEvaluationRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationId: str,
```

## DescribeContactFlowModuleRequestTypeDef

```python
# DescribeContactFlowModuleRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeContactFlowModuleRequestTypeDef


def get_value() -> DescribeContactFlowModuleRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeContactFlowModuleRequestTypeDef definition

class DescribeContactFlowModuleRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowModuleId: str,
```

## DescribeContactFlowRequestTypeDef

```python
# DescribeContactFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeContactFlowRequestTypeDef


def get_value() -> DescribeContactFlowRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeContactFlowRequestTypeDef definition

class DescribeContactFlowRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
```

## DescribeContactRequestTypeDef

```python
# DescribeContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeContactRequestTypeDef


def get_value() -> DescribeContactRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeContactRequestTypeDef definition

class DescribeContactRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
```

## DescribeEmailAddressRequestTypeDef

```python
# DescribeEmailAddressRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeEmailAddressRequestTypeDef


def get_value() -> DescribeEmailAddressRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeEmailAddressRequestTypeDef definition

class DescribeEmailAddressRequestTypeDef(TypedDict):
    InstanceId: str,
    EmailAddressId: str,
```

## DescribeEvaluationFormRequestTypeDef

```python
# DescribeEvaluationFormRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeEvaluationFormRequestTypeDef


def get_value() -> DescribeEvaluationFormRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeEvaluationFormRequestTypeDef definition

class DescribeEvaluationFormRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: NotRequired[int],
```

## DescribeHoursOfOperationOverrideRequestTypeDef

```python
# DescribeHoursOfOperationOverrideRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeHoursOfOperationOverrideRequestTypeDef


def get_value() -> DescribeHoursOfOperationOverrideRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeHoursOfOperationOverrideRequestTypeDef definition

class DescribeHoursOfOperationOverrideRequestTypeDef(TypedDict):
    InstanceId: str,
    HoursOfOperationId: str,
    HoursOfOperationOverrideId: str,
```

## DescribeHoursOfOperationRequestTypeDef

```python
# DescribeHoursOfOperationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeHoursOfOperationRequestTypeDef


def get_value() -> DescribeHoursOfOperationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeHoursOfOperationRequestTypeDef definition

class DescribeHoursOfOperationRequestTypeDef(TypedDict):
    InstanceId: str,
    HoursOfOperationId: str,
```

## DescribeInstanceAttributeRequestTypeDef

```python
# DescribeInstanceAttributeRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeInstanceAttributeRequestTypeDef


def get_value() -> DescribeInstanceAttributeRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeInstanceAttributeRequestTypeDef definition

class DescribeInstanceAttributeRequestTypeDef(TypedDict):
    InstanceId: str,
    AttributeType: InstanceAttributeTypeType,  # (1)
```

1. See [:material-code-brackets: InstanceAttributeTypeType](./literals.md#instanceattributetypetype) 
## DescribeInstanceRequestTypeDef

```python
# DescribeInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeInstanceRequestTypeDef


def get_value() -> DescribeInstanceRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeInstanceRequestTypeDef definition

class DescribeInstanceRequestTypeDef(TypedDict):
    InstanceId: str,
```

## DescribeInstanceStorageConfigRequestTypeDef

```python
# DescribeInstanceStorageConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeInstanceStorageConfigRequestTypeDef


def get_value() -> DescribeInstanceStorageConfigRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeInstanceStorageConfigRequestTypeDef definition

class DescribeInstanceStorageConfigRequestTypeDef(TypedDict):
    InstanceId: str,
    AssociationId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
## DescribePhoneNumberRequestTypeDef

```python
# DescribePhoneNumberRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribePhoneNumberRequestTypeDef


def get_value() -> DescribePhoneNumberRequestTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# DescribePhoneNumberRequestTypeDef definition

class DescribePhoneNumberRequestTypeDef(TypedDict):
    PhoneNumberId: str,
```

## DescribePredefinedAttributeRequestTypeDef

```python
# DescribePredefinedAttributeRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribePredefinedAttributeRequestTypeDef


def get_value() -> DescribePredefinedAttributeRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribePredefinedAttributeRequestTypeDef definition

class DescribePredefinedAttributeRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
```

## DescribePromptRequestTypeDef

```python
# DescribePromptRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribePromptRequestTypeDef


def get_value() -> DescribePromptRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribePromptRequestTypeDef definition

class DescribePromptRequestTypeDef(TypedDict):
    InstanceId: str,
    PromptId: str,
```

## PromptTypeDef

```python
# PromptTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PromptTypeDef


def get_value() -> PromptTypeDef:
    return {
        "PromptARN": ...,
    }


# PromptTypeDef definition

class PromptTypeDef(TypedDict):
    PromptARN: NotRequired[str],
    PromptId: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## DescribeQueueRequestTypeDef

```python
# DescribeQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeQueueRequestTypeDef


def get_value() -> DescribeQueueRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeQueueRequestTypeDef definition

class DescribeQueueRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
```

## DescribeQuickConnectRequestTypeDef

```python
# DescribeQuickConnectRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeQuickConnectRequestTypeDef


def get_value() -> DescribeQuickConnectRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeQuickConnectRequestTypeDef definition

class DescribeQuickConnectRequestTypeDef(TypedDict):
    InstanceId: str,
    QuickConnectId: str,
```

## DescribeRoutingProfileRequestTypeDef

```python
# DescribeRoutingProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeRoutingProfileRequestTypeDef


def get_value() -> DescribeRoutingProfileRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeRoutingProfileRequestTypeDef definition

class DescribeRoutingProfileRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
```

## DescribeRuleRequestTypeDef

```python
# DescribeRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeRuleRequestTypeDef


def get_value() -> DescribeRuleRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeRuleRequestTypeDef definition

class DescribeRuleRequestTypeDef(TypedDict):
    InstanceId: str,
    RuleId: str,
```

## DescribeSecurityProfileRequestTypeDef

```python
# DescribeSecurityProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeSecurityProfileRequestTypeDef


def get_value() -> DescribeSecurityProfileRequestTypeDef:
    return {
        "SecurityProfileId": ...,
    }


# DescribeSecurityProfileRequestTypeDef definition

class DescribeSecurityProfileRequestTypeDef(TypedDict):
    SecurityProfileId: str,
    InstanceId: str,
```

## SecurityProfileTypeDef

```python
# SecurityProfileTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SecurityProfileTypeDef


def get_value() -> SecurityProfileTypeDef:
    return {
        "Id": ...,
    }


# SecurityProfileTypeDef definition

class SecurityProfileTypeDef(TypedDict):
    Id: NotRequired[str],
    OrganizationResourceId: NotRequired[str],
    Arn: NotRequired[str],
    SecurityProfileName: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    AllowedAccessControlTags: NotRequired[Dict[str, str]],
    TagRestrictedResources: NotRequired[List[str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
    HierarchyRestrictedResources: NotRequired[List[str]],
    AllowedAccessControlHierarchyGroupId: NotRequired[str],
```

## DescribeTrafficDistributionGroupRequestTypeDef

```python
# DescribeTrafficDistributionGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeTrafficDistributionGroupRequestTypeDef


def get_value() -> DescribeTrafficDistributionGroupRequestTypeDef:
    return {
        "TrafficDistributionGroupId": ...,
    }


# DescribeTrafficDistributionGroupRequestTypeDef definition

class DescribeTrafficDistributionGroupRequestTypeDef(TypedDict):
    TrafficDistributionGroupId: str,
```

## TrafficDistributionGroupTypeDef

```python
# TrafficDistributionGroupTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TrafficDistributionGroupTypeDef


def get_value() -> TrafficDistributionGroupTypeDef:
    return {
        "Id": ...,
    }


# TrafficDistributionGroupTypeDef definition

class TrafficDistributionGroupTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    InstanceArn: NotRequired[str],
    Status: NotRequired[TrafficDistributionGroupStatusType],  # (1)
    Tags: NotRequired[Dict[str, str]],
    IsDefault: NotRequired[bool],
```

1. See [:material-code-brackets: TrafficDistributionGroupStatusType](./literals.md#trafficdistributiongroupstatustype) 
## DescribeUserHierarchyGroupRequestTypeDef

```python
# DescribeUserHierarchyGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeUserHierarchyGroupRequestTypeDef


def get_value() -> DescribeUserHierarchyGroupRequestTypeDef:
    return {
        "HierarchyGroupId": ...,
    }


# DescribeUserHierarchyGroupRequestTypeDef definition

class DescribeUserHierarchyGroupRequestTypeDef(TypedDict):
    HierarchyGroupId: str,
    InstanceId: str,
```

## DescribeUserHierarchyStructureRequestTypeDef

```python
# DescribeUserHierarchyStructureRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeUserHierarchyStructureRequestTypeDef


def get_value() -> DescribeUserHierarchyStructureRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeUserHierarchyStructureRequestTypeDef definition

class DescribeUserHierarchyStructureRequestTypeDef(TypedDict):
    InstanceId: str,
```

## DescribeUserRequestTypeDef

```python
# DescribeUserRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeUserRequestTypeDef


def get_value() -> DescribeUserRequestTypeDef:
    return {
        "UserId": ...,
    }


# DescribeUserRequestTypeDef definition

class DescribeUserRequestTypeDef(TypedDict):
    UserId: str,
    InstanceId: str,
```

## DescribeViewRequestTypeDef

```python
# DescribeViewRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeViewRequestTypeDef


def get_value() -> DescribeViewRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeViewRequestTypeDef definition

class DescribeViewRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
```

## DescribeVocabularyRequestTypeDef

```python
# DescribeVocabularyRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeVocabularyRequestTypeDef


def get_value() -> DescribeVocabularyRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeVocabularyRequestTypeDef definition

class DescribeVocabularyRequestTypeDef(TypedDict):
    InstanceId: str,
    VocabularyId: str,
```

## VocabularyTypeDef

```python
# VocabularyTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import VocabularyTypeDef


def get_value() -> VocabularyTypeDef:
    return {
        "Name": ...,
    }


# VocabularyTypeDef definition

class VocabularyTypeDef(TypedDict):
    Name: str,
    Id: str,
    Arn: str,
    LanguageCode: VocabularyLanguageCodeType,  # (1)
    State: VocabularyStateType,  # (2)
    LastModifiedTime: datetime,
    FailureReason: NotRequired[str],
    Content: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
2. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
## RoutingProfileReferenceTypeDef

```python
# RoutingProfileReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RoutingProfileReferenceTypeDef


def get_value() -> RoutingProfileReferenceTypeDef:
    return {
        "Id": ...,
    }


# RoutingProfileReferenceTypeDef definition

class RoutingProfileReferenceTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
```

## DisassociateAnalyticsDataSetRequestTypeDef

```python
# DisassociateAnalyticsDataSetRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisassociateAnalyticsDataSetRequestTypeDef


def get_value() -> DisassociateAnalyticsDataSetRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DisassociateAnalyticsDataSetRequestTypeDef definition

class DisassociateAnalyticsDataSetRequestTypeDef(TypedDict):
    InstanceId: str,
    DataSetId: str,
    TargetAccountId: NotRequired[str],
```

## DisassociateApprovedOriginRequestTypeDef

```python
# DisassociateApprovedOriginRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisassociateApprovedOriginRequestTypeDef


def get_value() -> DisassociateApprovedOriginRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DisassociateApprovedOriginRequestTypeDef definition

class DisassociateApprovedOriginRequestTypeDef(TypedDict):
    InstanceId: str,
    Origin: str,
    ClientToken: NotRequired[str],
```

## DisassociateFlowRequestTypeDef

```python
# DisassociateFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisassociateFlowRequestTypeDef


def get_value() -> DisassociateFlowRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DisassociateFlowRequestTypeDef definition

class DisassociateFlowRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceId: str,
    ResourceType: FlowAssociationResourceTypeType,  # (1)
```

1. See [:material-code-brackets: FlowAssociationResourceTypeType](./literals.md#flowassociationresourcetypetype) 
## DisassociateInstanceStorageConfigRequestTypeDef

```python
# DisassociateInstanceStorageConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisassociateInstanceStorageConfigRequestTypeDef


def get_value() -> DisassociateInstanceStorageConfigRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DisassociateInstanceStorageConfigRequestTypeDef definition

class DisassociateInstanceStorageConfigRequestTypeDef(TypedDict):
    InstanceId: str,
    AssociationId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
## DisassociateLambdaFunctionRequestTypeDef

```python
# DisassociateLambdaFunctionRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisassociateLambdaFunctionRequestTypeDef


def get_value() -> DisassociateLambdaFunctionRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DisassociateLambdaFunctionRequestTypeDef definition

class DisassociateLambdaFunctionRequestTypeDef(TypedDict):
    InstanceId: str,
    FunctionArn: str,
    ClientToken: NotRequired[str],
```

## DisassociateLexBotRequestTypeDef

```python
# DisassociateLexBotRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisassociateLexBotRequestTypeDef


def get_value() -> DisassociateLexBotRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DisassociateLexBotRequestTypeDef definition

class DisassociateLexBotRequestTypeDef(TypedDict):
    InstanceId: str,
    BotName: str,
    LexRegion: str,
    ClientToken: NotRequired[str],
```

## DisassociatePhoneNumberContactFlowRequestTypeDef

```python
# DisassociatePhoneNumberContactFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisassociatePhoneNumberContactFlowRequestTypeDef


def get_value() -> DisassociatePhoneNumberContactFlowRequestTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# DisassociatePhoneNumberContactFlowRequestTypeDef definition

class DisassociatePhoneNumberContactFlowRequestTypeDef(TypedDict):
    PhoneNumberId: str,
    InstanceId: str,
```

## DisassociateQueueQuickConnectsRequestTypeDef

```python
# DisassociateQueueQuickConnectsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisassociateQueueQuickConnectsRequestTypeDef


def get_value() -> DisassociateQueueQuickConnectsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DisassociateQueueQuickConnectsRequestTypeDef definition

class DisassociateQueueQuickConnectsRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    QuickConnectIds: Sequence[str],
```

## RoutingProfileQueueReferenceTypeDef

```python
# RoutingProfileQueueReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RoutingProfileQueueReferenceTypeDef


def get_value() -> RoutingProfileQueueReferenceTypeDef:
    return {
        "QueueId": ...,
    }


# RoutingProfileQueueReferenceTypeDef definition

class RoutingProfileQueueReferenceTypeDef(TypedDict):
    QueueId: str,
    Channel: ChannelType,  # (1)
```

1. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
## DisassociateSecurityKeyRequestTypeDef

```python
# DisassociateSecurityKeyRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisassociateSecurityKeyRequestTypeDef


def get_value() -> DisassociateSecurityKeyRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DisassociateSecurityKeyRequestTypeDef definition

class DisassociateSecurityKeyRequestTypeDef(TypedDict):
    InstanceId: str,
    AssociationId: str,
    ClientToken: NotRequired[str],
```

## DisassociateTrafficDistributionGroupUserRequestTypeDef

```python
# DisassociateTrafficDistributionGroupUserRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisassociateTrafficDistributionGroupUserRequestTypeDef


def get_value() -> DisassociateTrafficDistributionGroupUserRequestTypeDef:
    return {
        "TrafficDistributionGroupId": ...,
    }


# DisassociateTrafficDistributionGroupUserRequestTypeDef definition

class DisassociateTrafficDistributionGroupUserRequestTypeDef(TypedDict):
    TrafficDistributionGroupId: str,
    UserId: str,
    InstanceId: str,
```

## UserProficiencyDisassociateTypeDef

```python
# UserProficiencyDisassociateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserProficiencyDisassociateTypeDef


def get_value() -> UserProficiencyDisassociateTypeDef:
    return {
        "AttributeName": ...,
    }


# UserProficiencyDisassociateTypeDef definition

class UserProficiencyDisassociateTypeDef(TypedDict):
    AttributeName: str,
    AttributeValue: str,
```

## DisconnectReasonTypeDef

```python
# DisconnectReasonTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisconnectReasonTypeDef


def get_value() -> DisconnectReasonTypeDef:
    return {
        "Code": ...,
    }


# DisconnectReasonTypeDef definition

class DisconnectReasonTypeDef(TypedDict):
    Code: NotRequired[str],
```

## DismissUserContactRequestTypeDef

```python
# DismissUserContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DismissUserContactRequestTypeDef


def get_value() -> DismissUserContactRequestTypeDef:
    return {
        "UserId": ...,
    }


# DismissUserContactRequestTypeDef definition

class DismissUserContactRequestTypeDef(TypedDict):
    UserId: str,
    InstanceId: str,
    ContactId: str,
```

## DownloadUrlMetadataTypeDef

```python
# DownloadUrlMetadataTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DownloadUrlMetadataTypeDef


def get_value() -> DownloadUrlMetadataTypeDef:
    return {
        "Url": ...,
    }


# DownloadUrlMetadataTypeDef definition

class DownloadUrlMetadataTypeDef(TypedDict):
    Url: NotRequired[str],
    UrlExpiry: NotRequired[str],
```

## EmailAddressInfoTypeDef

```python
# EmailAddressInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EmailAddressInfoTypeDef


def get_value() -> EmailAddressInfoTypeDef:
    return {
        "EmailAddress": ...,
    }


# EmailAddressInfoTypeDef definition

class EmailAddressInfoTypeDef(TypedDict):
    EmailAddress: str,
    DisplayName: NotRequired[str],
```

## EmailAddressMetadataTypeDef

```python
# EmailAddressMetadataTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EmailAddressMetadataTypeDef


def get_value() -> EmailAddressMetadataTypeDef:
    return {
        "EmailAddressId": ...,
    }


# EmailAddressMetadataTypeDef definition

class EmailAddressMetadataTypeDef(TypedDict):
    EmailAddressId: NotRequired[str],
    EmailAddressArn: NotRequired[str],
    EmailAddress: NotRequired[str],
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
```

## EmailAttachmentTypeDef

```python
# EmailAttachmentTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EmailAttachmentTypeDef


def get_value() -> EmailAttachmentTypeDef:
    return {
        "FileName": ...,
    }


# EmailAttachmentTypeDef definition

class EmailAttachmentTypeDef(TypedDict):
    FileName: str,
    S3Url: str,
```

## EmailMessageReferenceTypeDef

```python
# EmailMessageReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EmailMessageReferenceTypeDef


def get_value() -> EmailMessageReferenceTypeDef:
    return {
        "Name": ...,
    }


# EmailMessageReferenceTypeDef definition

class EmailMessageReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
```

## EmailReferenceTypeDef

```python
# EmailReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EmailReferenceTypeDef


def get_value() -> EmailReferenceTypeDef:
    return {
        "Name": ...,
    }


# EmailReferenceTypeDef definition

class EmailReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## EncryptionConfigTypeDef

```python
# EncryptionConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EncryptionConfigTypeDef


def get_value() -> EncryptionConfigTypeDef:
    return {
        "EncryptionType": ...,
    }


# EncryptionConfigTypeDef definition

class EncryptionConfigTypeDef(TypedDict):
    EncryptionType: EncryptionTypeType,  # (1)
    KeyId: str,
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## EvaluationAnswerDataTypeDef

```python
# EvaluationAnswerDataTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationAnswerDataTypeDef


def get_value() -> EvaluationAnswerDataTypeDef:
    return {
        "StringValue": ...,
    }


# EvaluationAnswerDataTypeDef definition

class EvaluationAnswerDataTypeDef(TypedDict):
    StringValue: NotRequired[str],
    NumericValue: NotRequired[float],
    NotApplicable: NotRequired[bool],
```

## EvaluationFormSectionOutputTypeDef

```python
# EvaluationFormSectionOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormSectionOutputTypeDef


def get_value() -> EvaluationFormSectionOutputTypeDef:
    return {
        "Title": ...,
    }


# EvaluationFormSectionOutputTypeDef definition

class EvaluationFormSectionOutputTypeDef(TypedDict):
    Title: str,
    RefId: str,
    Items: List[Dict[str, Any]],
    Instructions: NotRequired[str],
    Weight: NotRequired[float],
```

## NumericQuestionPropertyValueAutomationTypeDef

```python
# NumericQuestionPropertyValueAutomationTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import NumericQuestionPropertyValueAutomationTypeDef


def get_value() -> NumericQuestionPropertyValueAutomationTypeDef:
    return {
        "Label": ...,
    }


# NumericQuestionPropertyValueAutomationTypeDef definition

class NumericQuestionPropertyValueAutomationTypeDef(TypedDict):
    Label: NumericQuestionPropertyAutomationLabelType,  # (1)
```

1. See [:material-code-brackets: NumericQuestionPropertyAutomationLabelType](./literals.md#numericquestionpropertyautomationlabeltype) 
## EvaluationFormNumericQuestionOptionTypeDef

```python
# EvaluationFormNumericQuestionOptionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormNumericQuestionOptionTypeDef


def get_value() -> EvaluationFormNumericQuestionOptionTypeDef:
    return {
        "MinValue": ...,
    }


# EvaluationFormNumericQuestionOptionTypeDef definition

class EvaluationFormNumericQuestionOptionTypeDef(TypedDict):
    MinValue: int,
    MaxValue: int,
    Score: NotRequired[int],
    AutomaticFail: NotRequired[bool],
```

## EvaluationFormSectionTypeDef

```python
# EvaluationFormSectionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormSectionTypeDef


def get_value() -> EvaluationFormSectionTypeDef:
    return {
        "Title": ...,
    }


# EvaluationFormSectionTypeDef definition

class EvaluationFormSectionTypeDef(TypedDict):
    Title: str,
    RefId: str,
    Items: Sequence[Mapping[str, Any]],
    Instructions: NotRequired[str],
    Weight: NotRequired[float],
```

## SingleSelectQuestionRuleCategoryAutomationTypeDef

```python
# SingleSelectQuestionRuleCategoryAutomationTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SingleSelectQuestionRuleCategoryAutomationTypeDef


def get_value() -> SingleSelectQuestionRuleCategoryAutomationTypeDef:
    return {
        "Category": ...,
    }


# SingleSelectQuestionRuleCategoryAutomationTypeDef definition

class SingleSelectQuestionRuleCategoryAutomationTypeDef(TypedDict):
    Category: str,
    Condition: SingleSelectQuestionRuleCategoryAutomationConditionType,  # (1)
    OptionRefId: str,
```

1. See [:material-code-brackets: SingleSelectQuestionRuleCategoryAutomationConditionType](./literals.md#singleselectquestionrulecategoryautomationconditiontype) 
## EvaluationFormSingleSelectQuestionOptionTypeDef

```python
# EvaluationFormSingleSelectQuestionOptionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormSingleSelectQuestionOptionTypeDef


def get_value() -> EvaluationFormSingleSelectQuestionOptionTypeDef:
    return {
        "RefId": ...,
    }


# EvaluationFormSingleSelectQuestionOptionTypeDef definition

class EvaluationFormSingleSelectQuestionOptionTypeDef(TypedDict):
    RefId: str,
    Text: str,
    Score: NotRequired[int],
    AutomaticFail: NotRequired[bool],
```

## EvaluationFormSummaryTypeDef

```python
# EvaluationFormSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormSummaryTypeDef


def get_value() -> EvaluationFormSummaryTypeDef:
    return {
        "EvaluationFormId": ...,
    }


# EvaluationFormSummaryTypeDef definition

class EvaluationFormSummaryTypeDef(TypedDict):
    EvaluationFormId: str,
    EvaluationFormArn: str,
    Title: str,
    CreatedTime: datetime,
    CreatedBy: str,
    LastModifiedTime: datetime,
    LastModifiedBy: str,
    LatestVersion: int,
    LastActivatedTime: NotRequired[datetime],
    LastActivatedBy: NotRequired[str],
    ActiveVersion: NotRequired[int],
```

## EvaluationFormVersionSummaryTypeDef

```python
# EvaluationFormVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormVersionSummaryTypeDef


def get_value() -> EvaluationFormVersionSummaryTypeDef:
    return {
        "EvaluationFormArn": ...,
    }


# EvaluationFormVersionSummaryTypeDef definition

class EvaluationFormVersionSummaryTypeDef(TypedDict):
    EvaluationFormArn: str,
    EvaluationFormId: str,
    EvaluationFormVersion: int,
    Locked: bool,
    Status: EvaluationFormVersionStatusType,  # (1)
    CreatedTime: datetime,
    CreatedBy: str,
    LastModifiedTime: datetime,
    LastModifiedBy: str,
```

1. See [:material-code-brackets: EvaluationFormVersionStatusType](./literals.md#evaluationformversionstatustype) 
## EvaluationScoreTypeDef

```python
# EvaluationScoreTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationScoreTypeDef


def get_value() -> EvaluationScoreTypeDef:
    return {
        "Percentage": ...,
    }


# EvaluationScoreTypeDef definition

class EvaluationScoreTypeDef(TypedDict):
    Percentage: NotRequired[float],
    NotApplicable: NotRequired[bool],
    AutomaticFail: NotRequired[bool],
```

## EvaluationNoteTypeDef

```python
# EvaluationNoteTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationNoteTypeDef


def get_value() -> EvaluationNoteTypeDef:
    return {
        "Value": ...,
    }


# EvaluationNoteTypeDef definition

class EvaluationNoteTypeDef(TypedDict):
    Value: NotRequired[str],
```

## EventBridgeActionDefinitionTypeDef

```python
# EventBridgeActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EventBridgeActionDefinitionTypeDef


def get_value() -> EventBridgeActionDefinitionTypeDef:
    return {
        "Name": ...,
    }


# EventBridgeActionDefinitionTypeDef definition

class EventBridgeActionDefinitionTypeDef(TypedDict):
    Name: str,
```

## ExpiryTypeDef

```python
# ExpiryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ExpiryTypeDef


def get_value() -> ExpiryTypeDef:
    return {
        "DurationInSeconds": ...,
    }


# ExpiryTypeDef definition

class ExpiryTypeDef(TypedDict):
    DurationInSeconds: NotRequired[int],
    ExpiryTimestamp: NotRequired[datetime],
```

## FieldValueUnionOutputTypeDef

```python
# FieldValueUnionOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import FieldValueUnionOutputTypeDef


def get_value() -> FieldValueUnionOutputTypeDef:
    return {
        "BooleanValue": ...,
    }


# FieldValueUnionOutputTypeDef definition

class FieldValueUnionOutputTypeDef(TypedDict):
    BooleanValue: NotRequired[bool],
    DoubleValue: NotRequired[float],
    EmptyValue: NotRequired[Dict[str, Any]],
    StringValue: NotRequired[str],
```

## FieldValueUnionTypeDef

```python
# FieldValueUnionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import FieldValueUnionTypeDef


def get_value() -> FieldValueUnionTypeDef:
    return {
        "BooleanValue": ...,
    }


# FieldValueUnionTypeDef definition

class FieldValueUnionTypeDef(TypedDict):
    BooleanValue: NotRequired[bool],
    DoubleValue: NotRequired[float],
    EmptyValue: NotRequired[Mapping[str, Any]],
    StringValue: NotRequired[str],
```

## FilterV2TypeDef

```python
# FilterV2TypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import FilterV2TypeDef


def get_value() -> FilterV2TypeDef:
    return {
        "FilterKey": ...,
    }


# FilterV2TypeDef definition

class FilterV2TypeDef(TypedDict):
    FilterKey: NotRequired[str],
    FilterValues: NotRequired[Sequence[str]],
```

## FiltersTypeDef

```python
# FiltersTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import FiltersTypeDef


def get_value() -> FiltersTypeDef:
    return {
        "Queues": ...,
    }


# FiltersTypeDef definition

class FiltersTypeDef(TypedDict):
    Queues: NotRequired[Sequence[str]],
    Channels: NotRequired[Sequence[ChannelType]],  # (1)
    RoutingProfiles: NotRequired[Sequence[str]],
    RoutingStepExpressions: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
## GetAttachedFileRequestTypeDef

```python
# GetAttachedFileRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetAttachedFileRequestTypeDef


def get_value() -> GetAttachedFileRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# GetAttachedFileRequestTypeDef definition

class GetAttachedFileRequestTypeDef(TypedDict):
    InstanceId: str,
    FileId: str,
    AssociatedResourceArn: str,
    UrlExpiryInSeconds: NotRequired[int],
```

## GetContactAttributesRequestTypeDef

```python
# GetContactAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetContactAttributesRequestTypeDef


def get_value() -> GetContactAttributesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# GetContactAttributesRequestTypeDef definition

class GetContactAttributesRequestTypeDef(TypedDict):
    InstanceId: str,
    InitialContactId: str,
```

## GetEffectiveHoursOfOperationsRequestTypeDef

```python
# GetEffectiveHoursOfOperationsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetEffectiveHoursOfOperationsRequestTypeDef


def get_value() -> GetEffectiveHoursOfOperationsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# GetEffectiveHoursOfOperationsRequestTypeDef definition

class GetEffectiveHoursOfOperationsRequestTypeDef(TypedDict):
    InstanceId: str,
    HoursOfOperationId: str,
    FromDate: str,
    ToDate: str,
```

## GetFederationTokenRequestTypeDef

```python
# GetFederationTokenRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetFederationTokenRequestTypeDef


def get_value() -> GetFederationTokenRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# GetFederationTokenRequestTypeDef definition

class GetFederationTokenRequestTypeDef(TypedDict):
    InstanceId: str,
```

## GetFlowAssociationRequestTypeDef

```python
# GetFlowAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetFlowAssociationRequestTypeDef


def get_value() -> GetFlowAssociationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# GetFlowAssociationRequestTypeDef definition

class GetFlowAssociationRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceId: str,
    ResourceType: FlowAssociationResourceTypeType,  # (1)
```

1. See [:material-code-brackets: FlowAssociationResourceTypeType](./literals.md#flowassociationresourcetypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PaginatorConfigTypeDef


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

## IntervalDetailsTypeDef

```python
# IntervalDetailsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import IntervalDetailsTypeDef


def get_value() -> IntervalDetailsTypeDef:
    return {
        "TimeZone": ...,
    }


# IntervalDetailsTypeDef definition

class IntervalDetailsTypeDef(TypedDict):
    TimeZone: NotRequired[str],
    IntervalPeriod: NotRequired[IntervalPeriodType],  # (1)
```

1. See [:material-code-brackets: IntervalPeriodType](./literals.md#intervalperiodtype) 
## GetPromptFileRequestTypeDef

```python
# GetPromptFileRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetPromptFileRequestTypeDef


def get_value() -> GetPromptFileRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# GetPromptFileRequestTypeDef definition

class GetPromptFileRequestTypeDef(TypedDict):
    InstanceId: str,
    PromptId: str,
```

## GetTaskTemplateRequestTypeDef

```python
# GetTaskTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetTaskTemplateRequestTypeDef


def get_value() -> GetTaskTemplateRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# GetTaskTemplateRequestTypeDef definition

class GetTaskTemplateRequestTypeDef(TypedDict):
    InstanceId: str,
    TaskTemplateId: str,
    SnapshotVersion: NotRequired[str],
```

## GetTrafficDistributionRequestTypeDef

```python
# GetTrafficDistributionRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetTrafficDistributionRequestTypeDef


def get_value() -> GetTrafficDistributionRequestTypeDef:
    return {
        "Id": ...,
    }


# GetTrafficDistributionRequestTypeDef definition

class GetTrafficDistributionRequestTypeDef(TypedDict):
    Id: str,
```

## HierarchyGroupSummaryReferenceTypeDef

```python
# HierarchyGroupSummaryReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HierarchyGroupSummaryReferenceTypeDef


def get_value() -> HierarchyGroupSummaryReferenceTypeDef:
    return {
        "Id": ...,
    }


# HierarchyGroupSummaryReferenceTypeDef definition

class HierarchyGroupSummaryReferenceTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
```

## HierarchyGroupSummaryTypeDef

```python
# HierarchyGroupSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HierarchyGroupSummaryTypeDef


def get_value() -> HierarchyGroupSummaryTypeDef:
    return {
        "Id": ...,
    }


# HierarchyGroupSummaryTypeDef definition

class HierarchyGroupSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## HierarchyLevelTypeDef

```python
# HierarchyLevelTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HierarchyLevelTypeDef


def get_value() -> HierarchyLevelTypeDef:
    return {
        "Id": ...,
    }


# HierarchyLevelTypeDef definition

class HierarchyLevelTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## HierarchyLevelUpdateTypeDef

```python
# HierarchyLevelUpdateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HierarchyLevelUpdateTypeDef


def get_value() -> HierarchyLevelUpdateTypeDef:
    return {
        "Name": ...,
    }


# HierarchyLevelUpdateTypeDef definition

class HierarchyLevelUpdateTypeDef(TypedDict):
    Name: str,
```

## ThresholdTypeDef

```python
# ThresholdTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ThresholdTypeDef


def get_value() -> ThresholdTypeDef:
    return {
        "Comparison": ...,
    }


# ThresholdTypeDef definition

class ThresholdTypeDef(TypedDict):
    Comparison: NotRequired[ComparisonType],  # (1)
    ThresholdValue: NotRequired[float],
```

1. See [:material-code-brackets: ComparisonType](./literals.md#comparisontype) 
## HoursOfOperationTimeSliceTypeDef

```python
# HoursOfOperationTimeSliceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HoursOfOperationTimeSliceTypeDef


def get_value() -> HoursOfOperationTimeSliceTypeDef:
    return {
        "Hours": ...,
    }


# HoursOfOperationTimeSliceTypeDef definition

class HoursOfOperationTimeSliceTypeDef(TypedDict):
    Hours: int,
    Minutes: int,
```

## OverrideTimeSliceTypeDef

```python
# OverrideTimeSliceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import OverrideTimeSliceTypeDef


def get_value() -> OverrideTimeSliceTypeDef:
    return {
        "Hours": ...,
    }


# OverrideTimeSliceTypeDef definition

class OverrideTimeSliceTypeDef(TypedDict):
    Hours: int,
    Minutes: int,
```

## HoursOfOperationSummaryTypeDef

```python
# HoursOfOperationSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HoursOfOperationSummaryTypeDef


def get_value() -> HoursOfOperationSummaryTypeDef:
    return {
        "Id": ...,
    }


# HoursOfOperationSummaryTypeDef definition

class HoursOfOperationSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## ImportPhoneNumberRequestTypeDef

```python
# ImportPhoneNumberRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ImportPhoneNumberRequestTypeDef


def get_value() -> ImportPhoneNumberRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ImportPhoneNumberRequestTypeDef definition

class ImportPhoneNumberRequestTypeDef(TypedDict):
    InstanceId: str,
    SourcePhoneNumberArn: str,
    PhoneNumberDescription: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    ClientToken: NotRequired[str],
```

## InboundRawMessageTypeDef

```python
# InboundRawMessageTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import InboundRawMessageTypeDef


def get_value() -> InboundRawMessageTypeDef:
    return {
        "Subject": ...,
    }


# InboundRawMessageTypeDef definition

class InboundRawMessageTypeDef(TypedDict):
    Subject: str,
    Body: str,
    ContentType: str,
    Headers: NotRequired[Mapping[EmailHeaderTypeType, str]],  # (1)
```

1. See [:material-code-brackets: EmailHeaderTypeType](./literals.md#emailheadertypetype) 
## InstanceStatusReasonTypeDef

```python
# InstanceStatusReasonTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import InstanceStatusReasonTypeDef


def get_value() -> InstanceStatusReasonTypeDef:
    return {
        "Message": ...,
    }


# InstanceStatusReasonTypeDef definition

class InstanceStatusReasonTypeDef(TypedDict):
    Message: NotRequired[str],
```

## KinesisFirehoseConfigTypeDef

```python
# KinesisFirehoseConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import KinesisFirehoseConfigTypeDef


def get_value() -> KinesisFirehoseConfigTypeDef:
    return {
        "FirehoseArn": ...,
    }


# KinesisFirehoseConfigTypeDef definition

class KinesisFirehoseConfigTypeDef(TypedDict):
    FirehoseArn: str,
```

## KinesisStreamConfigTypeDef

```python
# KinesisStreamConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import KinesisStreamConfigTypeDef


def get_value() -> KinesisStreamConfigTypeDef:
    return {
        "StreamArn": ...,
    }


# KinesisStreamConfigTypeDef definition

class KinesisStreamConfigTypeDef(TypedDict):
    StreamArn: str,
```

## InstanceSummaryTypeDef

```python
# InstanceSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import InstanceSummaryTypeDef


def get_value() -> InstanceSummaryTypeDef:
    return {
        "Id": ...,
    }


# InstanceSummaryTypeDef definition

class InstanceSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    IdentityManagementType: NotRequired[DirectoryTypeType],  # (1)
    InstanceAlias: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    ServiceRole: NotRequired[str],
    InstanceStatus: NotRequired[InstanceStatusType],  # (2)
    InboundCallsEnabled: NotRequired[bool],
    OutboundCallsEnabled: NotRequired[bool],
    InstanceAccessUrl: NotRequired[str],
```

1. See [:material-code-brackets: DirectoryTypeType](./literals.md#directorytypetype) 
2. See [:material-code-brackets: InstanceStatusType](./literals.md#instancestatustype) 
## IntegrationAssociationSummaryTypeDef

```python
# IntegrationAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import IntegrationAssociationSummaryTypeDef


def get_value() -> IntegrationAssociationSummaryTypeDef:
    return {
        "IntegrationAssociationId": ...,
    }


# IntegrationAssociationSummaryTypeDef definition

class IntegrationAssociationSummaryTypeDef(TypedDict):
    IntegrationAssociationId: NotRequired[str],
    IntegrationAssociationArn: NotRequired[str],
    InstanceId: NotRequired[str],
    IntegrationType: NotRequired[IntegrationTypeType],  # (1)
    IntegrationArn: NotRequired[str],
    SourceApplicationUrl: NotRequired[str],
    SourceApplicationName: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (2)
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## TaskTemplateFieldIdentifierTypeDef

```python
# TaskTemplateFieldIdentifierTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TaskTemplateFieldIdentifierTypeDef


def get_value() -> TaskTemplateFieldIdentifierTypeDef:
    return {
        "Name": ...,
    }


# TaskTemplateFieldIdentifierTypeDef definition

class TaskTemplateFieldIdentifierTypeDef(TypedDict):
    Name: NotRequired[str],
```

## ListAgentStatusRequestTypeDef

```python
# ListAgentStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListAgentStatusRequestTypeDef


def get_value() -> ListAgentStatusRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListAgentStatusRequestTypeDef definition

class ListAgentStatusRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    AgentStatusTypes: NotRequired[Sequence[AgentStatusTypeType]],  # (1)
```

1. See [:material-code-brackets: AgentStatusTypeType](./literals.md#agentstatustypetype) 
## ListAnalyticsDataAssociationsRequestTypeDef

```python
# ListAnalyticsDataAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListAnalyticsDataAssociationsRequestTypeDef


def get_value() -> ListAnalyticsDataAssociationsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListAnalyticsDataAssociationsRequestTypeDef definition

class ListAnalyticsDataAssociationsRequestTypeDef(TypedDict):
    InstanceId: str,
    DataSetId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListAnalyticsDataLakeDataSetsRequestTypeDef

```python
# ListAnalyticsDataLakeDataSetsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListAnalyticsDataLakeDataSetsRequestTypeDef


def get_value() -> ListAnalyticsDataLakeDataSetsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListAnalyticsDataLakeDataSetsRequestTypeDef definition

class ListAnalyticsDataLakeDataSetsRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListApprovedOriginsRequestTypeDef

```python
# ListApprovedOriginsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListApprovedOriginsRequestTypeDef


def get_value() -> ListApprovedOriginsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListApprovedOriginsRequestTypeDef definition

class ListApprovedOriginsRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListAssociatedContactsRequestTypeDef

```python
# ListAssociatedContactsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListAssociatedContactsRequestTypeDef


def get_value() -> ListAssociatedContactsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListAssociatedContactsRequestTypeDef definition

class ListAssociatedContactsRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAuthenticationProfilesRequestTypeDef

```python
# ListAuthenticationProfilesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListAuthenticationProfilesRequestTypeDef


def get_value() -> ListAuthenticationProfilesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListAuthenticationProfilesRequestTypeDef definition

class ListAuthenticationProfilesRequestTypeDef(TypedDict):
    InstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListBotsRequestTypeDef

```python
# ListBotsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListBotsRequestTypeDef


def get_value() -> ListBotsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListBotsRequestTypeDef definition

class ListBotsRequestTypeDef(TypedDict):
    InstanceId: str,
    LexVersion: LexVersionType,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: LexVersionType](./literals.md#lexversiontype) 
## ListContactEvaluationsRequestTypeDef

```python
# ListContactEvaluationsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactEvaluationsRequestTypeDef


def get_value() -> ListContactEvaluationsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListContactEvaluationsRequestTypeDef definition

class ListContactEvaluationsRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    NextToken: NotRequired[str],
```

## ListContactFlowModulesRequestTypeDef

```python
# ListContactFlowModulesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactFlowModulesRequestTypeDef


def get_value() -> ListContactFlowModulesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListContactFlowModulesRequestTypeDef definition

class ListContactFlowModulesRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ContactFlowModuleState: NotRequired[ContactFlowModuleStateType],  # (1)
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
## ListContactFlowVersionsRequestTypeDef

```python
# ListContactFlowVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactFlowVersionsRequestTypeDef


def get_value() -> ListContactFlowVersionsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListContactFlowVersionsRequestTypeDef definition

class ListContactFlowVersionsRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListContactFlowsRequestTypeDef

```python
# ListContactFlowsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactFlowsRequestTypeDef


def get_value() -> ListContactFlowsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListContactFlowsRequestTypeDef definition

class ListContactFlowsRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowTypes: NotRequired[Sequence[ContactFlowTypeType]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
## ListContactReferencesRequestTypeDef

```python
# ListContactReferencesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactReferencesRequestTypeDef


def get_value() -> ListContactReferencesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListContactReferencesRequestTypeDef definition

class ListContactReferencesRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ReferenceTypes: Sequence[ReferenceTypeType],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ReferenceTypeType](./literals.md#referencetypetype) 
## ListDefaultVocabulariesRequestTypeDef

```python
# ListDefaultVocabulariesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListDefaultVocabulariesRequestTypeDef


def get_value() -> ListDefaultVocabulariesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListDefaultVocabulariesRequestTypeDef definition

class ListDefaultVocabulariesRequestTypeDef(TypedDict):
    InstanceId: str,
    LanguageCode: NotRequired[VocabularyLanguageCodeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
## ListEvaluationFormVersionsRequestTypeDef

```python
# ListEvaluationFormVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListEvaluationFormVersionsRequestTypeDef


def get_value() -> ListEvaluationFormVersionsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListEvaluationFormVersionsRequestTypeDef definition

class ListEvaluationFormVersionsRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListEvaluationFormsRequestTypeDef

```python
# ListEvaluationFormsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListEvaluationFormsRequestTypeDef


def get_value() -> ListEvaluationFormsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListEvaluationFormsRequestTypeDef definition

class ListEvaluationFormsRequestTypeDef(TypedDict):
    InstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListFlowAssociationsRequestTypeDef

```python
# ListFlowAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListFlowAssociationsRequestTypeDef


def get_value() -> ListFlowAssociationsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListFlowAssociationsRequestTypeDef definition

class ListFlowAssociationsRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceType: NotRequired[ListFlowAssociationResourceTypeType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ListFlowAssociationResourceTypeType](./literals.md#listflowassociationresourcetypetype) 
## ListHoursOfOperationOverridesRequestTypeDef

```python
# ListHoursOfOperationOverridesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListHoursOfOperationOverridesRequestTypeDef


def get_value() -> ListHoursOfOperationOverridesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListHoursOfOperationOverridesRequestTypeDef definition

class ListHoursOfOperationOverridesRequestTypeDef(TypedDict):
    InstanceId: str,
    HoursOfOperationId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListHoursOfOperationsRequestTypeDef

```python
# ListHoursOfOperationsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListHoursOfOperationsRequestTypeDef


def get_value() -> ListHoursOfOperationsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListHoursOfOperationsRequestTypeDef definition

class ListHoursOfOperationsRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListInstanceAttributesRequestTypeDef

```python
# ListInstanceAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListInstanceAttributesRequestTypeDef


def get_value() -> ListInstanceAttributesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListInstanceAttributesRequestTypeDef definition

class ListInstanceAttributesRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListInstanceStorageConfigsRequestTypeDef

```python
# ListInstanceStorageConfigsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListInstanceStorageConfigsRequestTypeDef


def get_value() -> ListInstanceStorageConfigsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListInstanceStorageConfigsRequestTypeDef definition

class ListInstanceStorageConfigsRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
## ListInstancesRequestTypeDef

```python
# ListInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListInstancesRequestTypeDef


def get_value() -> ListInstancesRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListInstancesRequestTypeDef definition

class ListInstancesRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListIntegrationAssociationsRequestTypeDef

```python
# ListIntegrationAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListIntegrationAssociationsRequestTypeDef


def get_value() -> ListIntegrationAssociationsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListIntegrationAssociationsRequestTypeDef definition

class ListIntegrationAssociationsRequestTypeDef(TypedDict):
    InstanceId: str,
    IntegrationType: NotRequired[IntegrationTypeType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    IntegrationArn: NotRequired[str],
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
## ListLambdaFunctionsRequestTypeDef

```python
# ListLambdaFunctionsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListLambdaFunctionsRequestTypeDef


def get_value() -> ListLambdaFunctionsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListLambdaFunctionsRequestTypeDef definition

class ListLambdaFunctionsRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListLexBotsRequestTypeDef

```python
# ListLexBotsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListLexBotsRequestTypeDef


def get_value() -> ListLexBotsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListLexBotsRequestTypeDef definition

class ListLexBotsRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListPhoneNumbersRequestTypeDef

```python
# ListPhoneNumbersRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListPhoneNumbersRequestTypeDef


def get_value() -> ListPhoneNumbersRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListPhoneNumbersRequestTypeDef definition

class ListPhoneNumbersRequestTypeDef(TypedDict):
    InstanceId: str,
    PhoneNumberTypes: NotRequired[Sequence[PhoneNumberTypeType]],  # (1)
    PhoneNumberCountryCodes: NotRequired[Sequence[PhoneNumberCountryCodeType]],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
2. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
## PhoneNumberSummaryTypeDef

```python
# PhoneNumberSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PhoneNumberSummaryTypeDef


def get_value() -> PhoneNumberSummaryTypeDef:
    return {
        "Id": ...,
    }


# PhoneNumberSummaryTypeDef definition

class PhoneNumberSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    PhoneNumber: NotRequired[str],
    PhoneNumberType: NotRequired[PhoneNumberTypeType],  # (1)
    PhoneNumberCountryCode: NotRequired[PhoneNumberCountryCodeType],  # (2)
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
2. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
## ListPhoneNumbersSummaryTypeDef

```python
# ListPhoneNumbersSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListPhoneNumbersSummaryTypeDef


def get_value() -> ListPhoneNumbersSummaryTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# ListPhoneNumbersSummaryTypeDef definition

class ListPhoneNumbersSummaryTypeDef(TypedDict):
    PhoneNumberId: NotRequired[str],
    PhoneNumberArn: NotRequired[str],
    PhoneNumber: NotRequired[str],
    PhoneNumberCountryCode: NotRequired[PhoneNumberCountryCodeType],  # (1)
    PhoneNumberType: NotRequired[PhoneNumberTypeType],  # (2)
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    PhoneNumberDescription: NotRequired[str],
    SourcePhoneNumberArn: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
## ListPhoneNumbersV2RequestTypeDef

```python
# ListPhoneNumbersV2RequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListPhoneNumbersV2RequestTypeDef


def get_value() -> ListPhoneNumbersV2RequestTypeDef:
    return {
        "TargetArn": ...,
    }


# ListPhoneNumbersV2RequestTypeDef definition

class ListPhoneNumbersV2RequestTypeDef(TypedDict):
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    PhoneNumberCountryCodes: NotRequired[Sequence[PhoneNumberCountryCodeType]],  # (1)
    PhoneNumberTypes: NotRequired[Sequence[PhoneNumberTypeType]],  # (2)
    PhoneNumberPrefix: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
## ListPredefinedAttributesRequestTypeDef

```python
# ListPredefinedAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListPredefinedAttributesRequestTypeDef


def get_value() -> ListPredefinedAttributesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListPredefinedAttributesRequestTypeDef definition

class ListPredefinedAttributesRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PredefinedAttributeSummaryTypeDef

```python
# PredefinedAttributeSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PredefinedAttributeSummaryTypeDef


def get_value() -> PredefinedAttributeSummaryTypeDef:
    return {
        "Name": ...,
    }


# PredefinedAttributeSummaryTypeDef definition

class PredefinedAttributeSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## ListPromptsRequestTypeDef

```python
# ListPromptsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListPromptsRequestTypeDef


def get_value() -> ListPromptsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListPromptsRequestTypeDef definition

class ListPromptsRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PromptSummaryTypeDef

```python
# PromptSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PromptSummaryTypeDef


def get_value() -> PromptSummaryTypeDef:
    return {
        "Id": ...,
    }


# PromptSummaryTypeDef definition

class PromptSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## ListQueueQuickConnectsRequestTypeDef

```python
# ListQueueQuickConnectsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListQueueQuickConnectsRequestTypeDef


def get_value() -> ListQueueQuickConnectsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListQueueQuickConnectsRequestTypeDef definition

class ListQueueQuickConnectsRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## QuickConnectSummaryTypeDef

```python
# QuickConnectSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QuickConnectSummaryTypeDef


def get_value() -> QuickConnectSummaryTypeDef:
    return {
        "Id": ...,
    }


# QuickConnectSummaryTypeDef definition

class QuickConnectSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    QuickConnectType: NotRequired[QuickConnectTypeType],  # (1)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-brackets: QuickConnectTypeType](./literals.md#quickconnecttypetype) 
## ListQueuesRequestTypeDef

```python
# ListQueuesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListQueuesRequestTypeDef


def get_value() -> ListQueuesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListQueuesRequestTypeDef definition

class ListQueuesRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueTypes: NotRequired[Sequence[QueueTypeType]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: QueueTypeType](./literals.md#queuetypetype) 
## QueueSummaryTypeDef

```python
# QueueSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QueueSummaryTypeDef


def get_value() -> QueueSummaryTypeDef:
    return {
        "Id": ...,
    }


# QueueSummaryTypeDef definition

class QueueSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    QueueType: NotRequired[QueueTypeType],  # (1)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-brackets: QueueTypeType](./literals.md#queuetypetype) 
## ListQuickConnectsRequestTypeDef

```python
# ListQuickConnectsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListQuickConnectsRequestTypeDef


def get_value() -> ListQuickConnectsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListQuickConnectsRequestTypeDef definition

class ListQuickConnectsRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    QuickConnectTypes: NotRequired[Sequence[QuickConnectTypeType]],  # (1)
```

1. See [:material-code-brackets: QuickConnectTypeType](./literals.md#quickconnecttypetype) 
## ListRealtimeContactAnalysisSegmentsV2RequestTypeDef

```python
# ListRealtimeContactAnalysisSegmentsV2RequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListRealtimeContactAnalysisSegmentsV2RequestTypeDef


def get_value() -> ListRealtimeContactAnalysisSegmentsV2RequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListRealtimeContactAnalysisSegmentsV2RequestTypeDef definition

class ListRealtimeContactAnalysisSegmentsV2RequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    OutputType: RealTimeContactAnalysisOutputTypeType,  # (1)
    SegmentTypes: Sequence[RealTimeContactAnalysisSegmentTypeType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: RealTimeContactAnalysisOutputTypeType](./literals.md#realtimecontactanalysisoutputtypetype) 
2. See [:material-code-brackets: RealTimeContactAnalysisSegmentTypeType](./literals.md#realtimecontactanalysissegmenttypetype) 
## ListRoutingProfileQueuesRequestTypeDef

```python
# ListRoutingProfileQueuesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListRoutingProfileQueuesRequestTypeDef


def get_value() -> ListRoutingProfileQueuesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListRoutingProfileQueuesRequestTypeDef definition

class ListRoutingProfileQueuesRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## RoutingProfileQueueConfigSummaryTypeDef

```python
# RoutingProfileQueueConfigSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RoutingProfileQueueConfigSummaryTypeDef


def get_value() -> RoutingProfileQueueConfigSummaryTypeDef:
    return {
        "QueueId": ...,
    }


# RoutingProfileQueueConfigSummaryTypeDef definition

class RoutingProfileQueueConfigSummaryTypeDef(TypedDict):
    QueueId: str,
    QueueArn: str,
    QueueName: str,
    Priority: int,
    Delay: int,
    Channel: ChannelType,  # (1)
```

1. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
## ListRoutingProfilesRequestTypeDef

```python
# ListRoutingProfilesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListRoutingProfilesRequestTypeDef


def get_value() -> ListRoutingProfilesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListRoutingProfilesRequestTypeDef definition

class ListRoutingProfilesRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## RoutingProfileSummaryTypeDef

```python
# RoutingProfileSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RoutingProfileSummaryTypeDef


def get_value() -> RoutingProfileSummaryTypeDef:
    return {
        "Id": ...,
    }


# RoutingProfileSummaryTypeDef definition

class RoutingProfileSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## ListRulesRequestTypeDef

```python
# ListRulesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListRulesRequestTypeDef


def get_value() -> ListRulesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListRulesRequestTypeDef definition

class ListRulesRequestTypeDef(TypedDict):
    InstanceId: str,
    PublishStatus: NotRequired[RulePublishStatusType],  # (1)
    EventSourceName: NotRequired[EventSourceNameType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
2. See [:material-code-brackets: EventSourceNameType](./literals.md#eventsourcenametype) 
## ListSecurityKeysRequestTypeDef

```python
# ListSecurityKeysRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListSecurityKeysRequestTypeDef


def get_value() -> ListSecurityKeysRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListSecurityKeysRequestTypeDef definition

class ListSecurityKeysRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SecurityKeyTypeDef

```python
# SecurityKeyTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SecurityKeyTypeDef


def get_value() -> SecurityKeyTypeDef:
    return {
        "AssociationId": ...,
    }


# SecurityKeyTypeDef definition

class SecurityKeyTypeDef(TypedDict):
    AssociationId: NotRequired[str],
    Key: NotRequired[str],
    CreationTime: NotRequired[datetime],
```

## ListSecurityProfileApplicationsRequestTypeDef

```python
# ListSecurityProfileApplicationsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListSecurityProfileApplicationsRequestTypeDef


def get_value() -> ListSecurityProfileApplicationsRequestTypeDef:
    return {
        "SecurityProfileId": ...,
    }


# ListSecurityProfileApplicationsRequestTypeDef definition

class ListSecurityProfileApplicationsRequestTypeDef(TypedDict):
    SecurityProfileId: str,
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListSecurityProfilePermissionsRequestTypeDef

```python
# ListSecurityProfilePermissionsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListSecurityProfilePermissionsRequestTypeDef


def get_value() -> ListSecurityProfilePermissionsRequestTypeDef:
    return {
        "SecurityProfileId": ...,
    }


# ListSecurityProfilePermissionsRequestTypeDef definition

class ListSecurityProfilePermissionsRequestTypeDef(TypedDict):
    SecurityProfileId: str,
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListSecurityProfilesRequestTypeDef

```python
# ListSecurityProfilesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListSecurityProfilesRequestTypeDef


def get_value() -> ListSecurityProfilesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListSecurityProfilesRequestTypeDef definition

class ListSecurityProfilesRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SecurityProfileSummaryTypeDef

```python
# SecurityProfileSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SecurityProfileSummaryTypeDef


def get_value() -> SecurityProfileSummaryTypeDef:
    return {
        "Id": ...,
    }


# SecurityProfileSummaryTypeDef definition

class SecurityProfileSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTaskTemplatesRequestTypeDef

```python
# ListTaskTemplatesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListTaskTemplatesRequestTypeDef


def get_value() -> ListTaskTemplatesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListTaskTemplatesRequestTypeDef definition

class ListTaskTemplatesRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Status: NotRequired[TaskTemplateStatusType],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
## TaskTemplateMetadataTypeDef

```python
# TaskTemplateMetadataTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TaskTemplateMetadataTypeDef


def get_value() -> TaskTemplateMetadataTypeDef:
    return {
        "Id": ...,
    }


# TaskTemplateMetadataTypeDef definition

class TaskTemplateMetadataTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[TaskTemplateStatusType],  # (1)
    LastModifiedTime: NotRequired[datetime],
    CreatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
## ListTrafficDistributionGroupUsersRequestTypeDef

```python
# ListTrafficDistributionGroupUsersRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListTrafficDistributionGroupUsersRequestTypeDef


def get_value() -> ListTrafficDistributionGroupUsersRequestTypeDef:
    return {
        "TrafficDistributionGroupId": ...,
    }


# ListTrafficDistributionGroupUsersRequestTypeDef definition

class ListTrafficDistributionGroupUsersRequestTypeDef(TypedDict):
    TrafficDistributionGroupId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## TrafficDistributionGroupUserSummaryTypeDef

```python
# TrafficDistributionGroupUserSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TrafficDistributionGroupUserSummaryTypeDef


def get_value() -> TrafficDistributionGroupUserSummaryTypeDef:
    return {
        "UserId": ...,
    }


# TrafficDistributionGroupUserSummaryTypeDef definition

class TrafficDistributionGroupUserSummaryTypeDef(TypedDict):
    UserId: NotRequired[str],
```

## ListTrafficDistributionGroupsRequestTypeDef

```python
# ListTrafficDistributionGroupsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListTrafficDistributionGroupsRequestTypeDef


def get_value() -> ListTrafficDistributionGroupsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListTrafficDistributionGroupsRequestTypeDef definition

class ListTrafficDistributionGroupsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    InstanceId: NotRequired[str],
```

## TrafficDistributionGroupSummaryTypeDef

```python
# TrafficDistributionGroupSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TrafficDistributionGroupSummaryTypeDef


def get_value() -> TrafficDistributionGroupSummaryTypeDef:
    return {
        "Id": ...,
    }


# TrafficDistributionGroupSummaryTypeDef definition

class TrafficDistributionGroupSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    InstanceArn: NotRequired[str],
    Status: NotRequired[TrafficDistributionGroupStatusType],  # (1)
    IsDefault: NotRequired[bool],
```

1. See [:material-code-brackets: TrafficDistributionGroupStatusType](./literals.md#trafficdistributiongroupstatustype) 
## ListUseCasesRequestTypeDef

```python
# ListUseCasesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListUseCasesRequestTypeDef


def get_value() -> ListUseCasesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListUseCasesRequestTypeDef definition

class ListUseCasesRequestTypeDef(TypedDict):
    InstanceId: str,
    IntegrationAssociationId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## UseCaseTypeDef

```python
# UseCaseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UseCaseTypeDef


def get_value() -> UseCaseTypeDef:
    return {
        "UseCaseId": ...,
    }


# UseCaseTypeDef definition

class UseCaseTypeDef(TypedDict):
    UseCaseId: NotRequired[str],
    UseCaseArn: NotRequired[str],
    UseCaseType: NotRequired[UseCaseTypeType],  # (1)
```

1. See [:material-code-brackets: UseCaseTypeType](./literals.md#usecasetypetype) 
## ListUserHierarchyGroupsRequestTypeDef

```python
# ListUserHierarchyGroupsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListUserHierarchyGroupsRequestTypeDef


def get_value() -> ListUserHierarchyGroupsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListUserHierarchyGroupsRequestTypeDef definition

class ListUserHierarchyGroupsRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListUserProficienciesRequestTypeDef

```python
# ListUserProficienciesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListUserProficienciesRequestTypeDef


def get_value() -> ListUserProficienciesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListUserProficienciesRequestTypeDef definition

class ListUserProficienciesRequestTypeDef(TypedDict):
    InstanceId: str,
    UserId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListUsersRequestTypeDef

```python
# ListUsersRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListUsersRequestTypeDef


def get_value() -> ListUsersRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListUsersRequestTypeDef definition

class ListUsersRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## UserSummaryTypeDef

```python
# UserSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserSummaryTypeDef


def get_value() -> UserSummaryTypeDef:
    return {
        "Id": ...,
    }


# UserSummaryTypeDef definition

class UserSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Username: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## ListViewVersionsRequestTypeDef

```python
# ListViewVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListViewVersionsRequestTypeDef


def get_value() -> ListViewVersionsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListViewVersionsRequestTypeDef definition

class ListViewVersionsRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ViewVersionSummaryTypeDef

```python
# ViewVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ViewVersionSummaryTypeDef


def get_value() -> ViewVersionSummaryTypeDef:
    return {
        "Id": ...,
    }


# ViewVersionSummaryTypeDef definition

class ViewVersionSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Description: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[ViewTypeType],  # (1)
    Version: NotRequired[int],
    VersionDescription: NotRequired[str],
```

1. See [:material-code-brackets: ViewTypeType](./literals.md#viewtypetype) 
## ListViewsRequestTypeDef

```python
# ListViewsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListViewsRequestTypeDef


def get_value() -> ListViewsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListViewsRequestTypeDef definition

class ListViewsRequestTypeDef(TypedDict):
    InstanceId: str,
    Type: NotRequired[ViewTypeType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ViewTypeType](./literals.md#viewtypetype) 
## ViewSummaryTypeDef

```python
# ViewSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ViewSummaryTypeDef


def get_value() -> ViewSummaryTypeDef:
    return {
        "Id": ...,
    }


# ViewSummaryTypeDef definition

class ViewSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[ViewTypeType],  # (1)
    Status: NotRequired[ViewStatusType],  # (2)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: ViewTypeType](./literals.md#viewtypetype) 
2. See [:material-code-brackets: ViewStatusType](./literals.md#viewstatustype) 
## MediaPlacementTypeDef

```python
# MediaPlacementTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MediaPlacementTypeDef


def get_value() -> MediaPlacementTypeDef:
    return {
        "AudioHostUrl": ...,
    }


# MediaPlacementTypeDef definition

class MediaPlacementTypeDef(TypedDict):
    AudioHostUrl: NotRequired[str],
    AudioFallbackUrl: NotRequired[str],
    SignalingUrl: NotRequired[str],
    TurnControlUrl: NotRequired[str],
    EventIngestionUrl: NotRequired[str],
```

## MetricFilterV2OutputTypeDef

```python
# MetricFilterV2OutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MetricFilterV2OutputTypeDef


def get_value() -> MetricFilterV2OutputTypeDef:
    return {
        "MetricFilterKey": ...,
    }


# MetricFilterV2OutputTypeDef definition

class MetricFilterV2OutputTypeDef(TypedDict):
    MetricFilterKey: NotRequired[str],
    MetricFilterValues: NotRequired[List[str]],
    Negate: NotRequired[bool],
```

## MetricFilterV2TypeDef

```python
# MetricFilterV2TypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MetricFilterV2TypeDef


def get_value() -> MetricFilterV2TypeDef:
    return {
        "MetricFilterKey": ...,
    }


# MetricFilterV2TypeDef definition

class MetricFilterV2TypeDef(TypedDict):
    MetricFilterKey: NotRequired[str],
    MetricFilterValues: NotRequired[Sequence[str]],
    Negate: NotRequired[bool],
```

## MetricIntervalTypeDef

```python
# MetricIntervalTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MetricIntervalTypeDef


def get_value() -> MetricIntervalTypeDef:
    return {
        "Interval": ...,
    }


# MetricIntervalTypeDef definition

class MetricIntervalTypeDef(TypedDict):
    Interval: NotRequired[IntervalPeriodType],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: IntervalPeriodType](./literals.md#intervalperiodtype) 
## ThresholdV2TypeDef

```python
# ThresholdV2TypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ThresholdV2TypeDef


def get_value() -> ThresholdV2TypeDef:
    return {
        "Comparison": ...,
    }


# ThresholdV2TypeDef definition

class ThresholdV2TypeDef(TypedDict):
    Comparison: NotRequired[str],
    ThresholdValue: NotRequired[float],
```

## MonitorContactRequestTypeDef

```python
# MonitorContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MonitorContactRequestTypeDef


def get_value() -> MonitorContactRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# MonitorContactRequestTypeDef definition

class MonitorContactRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    UserId: str,
    AllowedMonitorCapabilities: NotRequired[Sequence[MonitorCapabilityType]],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: MonitorCapabilityType](./literals.md#monitorcapabilitytype) 
## ParticipantDetailsTypeDef

```python
# ParticipantDetailsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ParticipantDetailsTypeDef


def get_value() -> ParticipantDetailsTypeDef:
    return {
        "DisplayName": ...,
    }


# ParticipantDetailsTypeDef definition

class ParticipantDetailsTypeDef(TypedDict):
    DisplayName: str,
```

## NotificationRecipientTypeOutputTypeDef

```python
# NotificationRecipientTypeOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import NotificationRecipientTypeOutputTypeDef


def get_value() -> NotificationRecipientTypeOutputTypeDef:
    return {
        "UserTags": ...,
    }


# NotificationRecipientTypeOutputTypeDef definition

class NotificationRecipientTypeOutputTypeDef(TypedDict):
    UserTags: NotRequired[Dict[str, str]],
    UserIds: NotRequired[List[str]],
```

## NotificationRecipientTypeTypeDef

```python
# NotificationRecipientTypeTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import NotificationRecipientTypeTypeDef


def get_value() -> NotificationRecipientTypeTypeDef:
    return {
        "UserTags": ...,
    }


# NotificationRecipientTypeTypeDef definition

class NotificationRecipientTypeTypeDef(TypedDict):
    UserTags: NotRequired[Mapping[str, str]],
    UserIds: NotRequired[Sequence[str]],
```

## NumberReferenceTypeDef

```python
# NumberReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import NumberReferenceTypeDef


def get_value() -> NumberReferenceTypeDef:
    return {
        "Name": ...,
    }


# NumberReferenceTypeDef definition

class NumberReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## OutboundRawMessageTypeDef

```python
# OutboundRawMessageTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import OutboundRawMessageTypeDef


def get_value() -> OutboundRawMessageTypeDef:
    return {
        "Subject": ...,
    }


# OutboundRawMessageTypeDef definition

class OutboundRawMessageTypeDef(TypedDict):
    Subject: str,
    Body: str,
    ContentType: str,
```

## ParticipantTimerValueTypeDef

```python
# ParticipantTimerValueTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ParticipantTimerValueTypeDef


def get_value() -> ParticipantTimerValueTypeDef:
    return {
        "ParticipantTimerAction": ...,
    }


# ParticipantTimerValueTypeDef definition

class ParticipantTimerValueTypeDef(TypedDict):
    ParticipantTimerAction: NotRequired[ParticipantTimerActionType],  # (1)
    ParticipantTimerDurationInMinutes: NotRequired[int],
```

1. See [:material-code-brackets: ParticipantTimerActionType](./literals.md#participanttimeractiontype) 
## PauseContactRequestTypeDef

```python
# PauseContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PauseContactRequestTypeDef


def get_value() -> PauseContactRequestTypeDef:
    return {
        "ContactId": ...,
    }


# PauseContactRequestTypeDef definition

class PauseContactRequestTypeDef(TypedDict):
    ContactId: str,
    InstanceId: str,
    ContactFlowId: NotRequired[str],
```

## PersistentChatTypeDef

```python
# PersistentChatTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PersistentChatTypeDef


def get_value() -> PersistentChatTypeDef:
    return {
        "RehydrationType": ...,
    }


# PersistentChatTypeDef definition

class PersistentChatTypeDef(TypedDict):
    RehydrationType: NotRequired[RehydrationTypeType],  # (1)
    SourceContactId: NotRequired[str],
```

1. See [:material-code-brackets: RehydrationTypeType](./literals.md#rehydrationtypetype) 
## PhoneNumberQuickConnectConfigTypeDef

```python
# PhoneNumberQuickConnectConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PhoneNumberQuickConnectConfigTypeDef


def get_value() -> PhoneNumberQuickConnectConfigTypeDef:
    return {
        "PhoneNumber": ...,
    }


# PhoneNumberQuickConnectConfigTypeDef definition

class PhoneNumberQuickConnectConfigTypeDef(TypedDict):
    PhoneNumber: str,
```

## PredefinedAttributeValuesOutputTypeDef

```python
# PredefinedAttributeValuesOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PredefinedAttributeValuesOutputTypeDef


def get_value() -> PredefinedAttributeValuesOutputTypeDef:
    return {
        "StringList": ...,
    }


# PredefinedAttributeValuesOutputTypeDef definition

class PredefinedAttributeValuesOutputTypeDef(TypedDict):
    StringList: NotRequired[List[str]],
```

## PredefinedAttributeValuesTypeDef

```python
# PredefinedAttributeValuesTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PredefinedAttributeValuesTypeDef


def get_value() -> PredefinedAttributeValuesTypeDef:
    return {
        "StringList": ...,
    }


# PredefinedAttributeValuesTypeDef definition

class PredefinedAttributeValuesTypeDef(TypedDict):
    StringList: NotRequired[Sequence[str]],
```

## PutUserStatusRequestTypeDef

```python
# PutUserStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PutUserStatusRequestTypeDef


def get_value() -> PutUserStatusRequestTypeDef:
    return {
        "UserId": ...,
    }


# PutUserStatusRequestTypeDef definition

class PutUserStatusRequestTypeDef(TypedDict):
    UserId: str,
    InstanceId: str,
    AgentStatusId: str,
```

## QueueInfoInputTypeDef

```python
# QueueInfoInputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QueueInfoInputTypeDef


def get_value() -> QueueInfoInputTypeDef:
    return {
        "Id": ...,
    }


# QueueInfoInputTypeDef definition

class QueueInfoInputTypeDef(TypedDict):
    Id: NotRequired[str],
```

## QueueQuickConnectConfigTypeDef

```python
# QueueQuickConnectConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QueueQuickConnectConfigTypeDef


def get_value() -> QueueQuickConnectConfigTypeDef:
    return {
        "QueueId": ...,
    }


# QueueQuickConnectConfigTypeDef definition

class QueueQuickConnectConfigTypeDef(TypedDict):
    QueueId: str,
    ContactFlowId: str,
```

## UserQuickConnectConfigTypeDef

```python
# UserQuickConnectConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserQuickConnectConfigTypeDef


def get_value() -> UserQuickConnectConfigTypeDef:
    return {
        "UserId": ...,
    }


# UserQuickConnectConfigTypeDef definition

class UserQuickConnectConfigTypeDef(TypedDict):
    UserId: str,
    ContactFlowId: str,
```

## RealTimeContactAnalysisAttachmentTypeDef

```python
# RealTimeContactAnalysisAttachmentTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisAttachmentTypeDef


def get_value() -> RealTimeContactAnalysisAttachmentTypeDef:
    return {
        "AttachmentName": ...,
    }


# RealTimeContactAnalysisAttachmentTypeDef definition

class RealTimeContactAnalysisAttachmentTypeDef(TypedDict):
    AttachmentName: str,
    AttachmentId: str,
    ContentType: NotRequired[str],
    Status: NotRequired[ArtifactStatusType],  # (1)
```

1. See [:material-code-brackets: ArtifactStatusType](./literals.md#artifactstatustype) 
## RealTimeContactAnalysisCharacterIntervalTypeDef

```python
# RealTimeContactAnalysisCharacterIntervalTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisCharacterIntervalTypeDef


def get_value() -> RealTimeContactAnalysisCharacterIntervalTypeDef:
    return {
        "BeginOffsetChar": ...,
    }


# RealTimeContactAnalysisCharacterIntervalTypeDef definition

class RealTimeContactAnalysisCharacterIntervalTypeDef(TypedDict):
    BeginOffsetChar: int,
    EndOffsetChar: int,
```

## RealTimeContactAnalysisTimeDataTypeDef

```python
# RealTimeContactAnalysisTimeDataTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisTimeDataTypeDef


def get_value() -> RealTimeContactAnalysisTimeDataTypeDef:
    return {
        "AbsoluteTime": ...,
    }


# RealTimeContactAnalysisTimeDataTypeDef definition

class RealTimeContactAnalysisTimeDataTypeDef(TypedDict):
    AbsoluteTime: NotRequired[datetime],
```

## RealTimeContactAnalysisSegmentPostContactSummaryTypeDef

```python
# RealTimeContactAnalysisSegmentPostContactSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisSegmentPostContactSummaryTypeDef


def get_value() -> RealTimeContactAnalysisSegmentPostContactSummaryTypeDef:
    return {
        "Content": ...,
    }


# RealTimeContactAnalysisSegmentPostContactSummaryTypeDef definition

class RealTimeContactAnalysisSegmentPostContactSummaryTypeDef(TypedDict):
    Status: RealTimeContactAnalysisPostContactSummaryStatusType,  # (1)
    Content: NotRequired[str],
    FailureCode: NotRequired[RealTimeContactAnalysisPostContactSummaryFailureCodeType],  # (2)
```

1. See [:material-code-brackets: RealTimeContactAnalysisPostContactSummaryStatusType](./literals.md#realtimecontactanalysispostcontactsummarystatustype) 
2. See [:material-code-brackets: RealTimeContactAnalysisPostContactSummaryFailureCodeType](./literals.md#realtimecontactanalysispostcontactsummaryfailurecodetype) 
## StringReferenceTypeDef

```python
# StringReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StringReferenceTypeDef


def get_value() -> StringReferenceTypeDef:
    return {
        "Name": ...,
    }


# StringReferenceTypeDef definition

class StringReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## UrlReferenceTypeDef

```python
# UrlReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UrlReferenceTypeDef


def get_value() -> UrlReferenceTypeDef:
    return {
        "Name": ...,
    }


# UrlReferenceTypeDef definition

class UrlReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## ReleasePhoneNumberRequestTypeDef

```python
# ReleasePhoneNumberRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ReleasePhoneNumberRequestTypeDef


def get_value() -> ReleasePhoneNumberRequestTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# ReleasePhoneNumberRequestTypeDef definition

class ReleasePhoneNumberRequestTypeDef(TypedDict):
    PhoneNumberId: str,
    ClientToken: NotRequired[str],
```

## ReplicateInstanceRequestTypeDef

```python
# ReplicateInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ReplicateInstanceRequestTypeDef


def get_value() -> ReplicateInstanceRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ReplicateInstanceRequestTypeDef definition

class ReplicateInstanceRequestTypeDef(TypedDict):
    InstanceId: str,
    ReplicaRegion: str,
    ReplicaAlias: str,
    ClientToken: NotRequired[str],
```

## ReplicationStatusSummaryTypeDef

```python
# ReplicationStatusSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ReplicationStatusSummaryTypeDef


def get_value() -> ReplicationStatusSummaryTypeDef:
    return {
        "Region": ...,
    }


# ReplicationStatusSummaryTypeDef definition

class ReplicationStatusSummaryTypeDef(TypedDict):
    Region: NotRequired[str],
    ReplicationStatus: NotRequired[InstanceReplicationStatusType],  # (1)
    ReplicationStatusReason: NotRequired[str],
```

1. See [:material-code-brackets: InstanceReplicationStatusType](./literals.md#instancereplicationstatustype) 
## TagSearchConditionTypeDef

```python
# TagSearchConditionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TagSearchConditionTypeDef


def get_value() -> TagSearchConditionTypeDef:
    return {
        "tagKey": ...,
    }


# TagSearchConditionTypeDef definition

class TagSearchConditionTypeDef(TypedDict):
    tagKey: NotRequired[str],
    tagValue: NotRequired[str],
    tagKeyComparisonType: NotRequired[StringComparisonTypeType],  # (1)
    tagValueComparisonType: NotRequired[StringComparisonTypeType],  # (1)
```

1. See [:material-code-brackets: StringComparisonTypeType](./literals.md#stringcomparisontypetype) 
2. See [:material-code-brackets: StringComparisonTypeType](./literals.md#stringcomparisontypetype) 
## ResumeContactRecordingRequestTypeDef

```python
# ResumeContactRecordingRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ResumeContactRecordingRequestTypeDef


def get_value() -> ResumeContactRecordingRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ResumeContactRecordingRequestTypeDef definition

class ResumeContactRecordingRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
    ContactRecordingType: NotRequired[ContactRecordingTypeType],  # (1)
```

1. See [:material-code-brackets: ContactRecordingTypeType](./literals.md#contactrecordingtypetype) 
## ResumeContactRequestTypeDef

```python
# ResumeContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ResumeContactRequestTypeDef


def get_value() -> ResumeContactRequestTypeDef:
    return {
        "ContactId": ...,
    }


# ResumeContactRequestTypeDef definition

class ResumeContactRequestTypeDef(TypedDict):
    ContactId: str,
    InstanceId: str,
    ContactFlowId: NotRequired[str],
```

## RoutingCriteriaInputStepExpiryTypeDef

```python
# RoutingCriteriaInputStepExpiryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RoutingCriteriaInputStepExpiryTypeDef


def get_value() -> RoutingCriteriaInputStepExpiryTypeDef:
    return {
        "DurationInSeconds": ...,
    }


# RoutingCriteriaInputStepExpiryTypeDef definition

class RoutingCriteriaInputStepExpiryTypeDef(TypedDict):
    DurationInSeconds: NotRequired[int],
```

## SubmitAutoEvaluationActionDefinitionTypeDef

```python
# SubmitAutoEvaluationActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SubmitAutoEvaluationActionDefinitionTypeDef


def get_value() -> SubmitAutoEvaluationActionDefinitionTypeDef:
    return {
        "EvaluationFormId": ...,
    }


# SubmitAutoEvaluationActionDefinitionTypeDef definition

class SubmitAutoEvaluationActionDefinitionTypeDef(TypedDict):
    EvaluationFormId: str,
```

## SearchAvailablePhoneNumbersRequestTypeDef

```python
# SearchAvailablePhoneNumbersRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchAvailablePhoneNumbersRequestTypeDef


def get_value() -> SearchAvailablePhoneNumbersRequestTypeDef:
    return {
        "PhoneNumberCountryCode": ...,
    }


# SearchAvailablePhoneNumbersRequestTypeDef definition

class SearchAvailablePhoneNumbersRequestTypeDef(TypedDict):
    PhoneNumberCountryCode: PhoneNumberCountryCodeType,  # (1)
    PhoneNumberType: PhoneNumberTypeType,  # (2)
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    PhoneNumberPrefix: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
## SortTypeDef

```python
# SortTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SortTypeDef


def get_value() -> SortTypeDef:
    return {
        "FieldName": ...,
    }


# SortTypeDef definition

class SortTypeDef(TypedDict):
    FieldName: SortableFieldNameType,  # (1)
    Order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: SortableFieldNameType](./literals.md#sortablefieldnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## TagSetTypeDef

```python
# TagSetTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TagSetTypeDef


def get_value() -> TagSetTypeDef:
    return {
        "key": ...,
    }


# TagSetTypeDef definition

class TagSetTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## SecurityProfileSearchSummaryTypeDef

```python
# SecurityProfileSearchSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SecurityProfileSearchSummaryTypeDef


def get_value() -> SecurityProfileSearchSummaryTypeDef:
    return {
        "Id": ...,
    }


# SecurityProfileSearchSummaryTypeDef definition

class SecurityProfileSearchSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    OrganizationResourceId: NotRequired[str],
    Arn: NotRequired[str],
    SecurityProfileName: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

## SearchVocabulariesRequestTypeDef

```python
# SearchVocabulariesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchVocabulariesRequestTypeDef


def get_value() -> SearchVocabulariesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchVocabulariesRequestTypeDef definition

class SearchVocabulariesRequestTypeDef(TypedDict):
    InstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    State: NotRequired[VocabularyStateType],  # (1)
    NameStartsWith: NotRequired[str],
    LanguageCode: NotRequired[VocabularyLanguageCodeType],  # (2)
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
## VocabularySummaryTypeDef

```python
# VocabularySummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import VocabularySummaryTypeDef


def get_value() -> VocabularySummaryTypeDef:
    return {
        "Name": ...,
    }


# VocabularySummaryTypeDef definition

class VocabularySummaryTypeDef(TypedDict):
    Name: str,
    Id: str,
    Arn: str,
    LanguageCode: VocabularyLanguageCodeType,  # (1)
    State: VocabularyStateType,  # (2)
    LastModifiedTime: datetime,
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
2. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
## SearchableContactAttributesCriteriaTypeDef

```python
# SearchableContactAttributesCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchableContactAttributesCriteriaTypeDef


def get_value() -> SearchableContactAttributesCriteriaTypeDef:
    return {
        "Key": ...,
    }


# SearchableContactAttributesCriteriaTypeDef definition

class SearchableContactAttributesCriteriaTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
```

## SearchableSegmentAttributesCriteriaTypeDef

```python
# SearchableSegmentAttributesCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchableSegmentAttributesCriteriaTypeDef


def get_value() -> SearchableSegmentAttributesCriteriaTypeDef:
    return {
        "Key": ...,
    }


# SearchableSegmentAttributesCriteriaTypeDef definition

class SearchableSegmentAttributesCriteriaTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
```

## SegmentAttributeValueTypeDef

```python
# SegmentAttributeValueTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SegmentAttributeValueTypeDef


def get_value() -> SegmentAttributeValueTypeDef:
    return {
        "ValueString": ...,
    }


# SegmentAttributeValueTypeDef definition

class SegmentAttributeValueTypeDef(TypedDict):
    ValueString: NotRequired[str],
    ValueMap: NotRequired[Mapping[str, Mapping[str, Any]]],
    ValueInteger: NotRequired[int],
```

## SourceCampaignTypeDef

```python
# SourceCampaignTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SourceCampaignTypeDef


def get_value() -> SourceCampaignTypeDef:
    return {
        "CampaignId": ...,
    }


# SourceCampaignTypeDef definition

class SourceCampaignTypeDef(TypedDict):
    CampaignId: NotRequired[str],
    OutboundRequestId: NotRequired[str],
```

## SignInDistributionTypeDef

```python
# SignInDistributionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SignInDistributionTypeDef


def get_value() -> SignInDistributionTypeDef:
    return {
        "Region": ...,
    }


# SignInDistributionTypeDef definition

class SignInDistributionTypeDef(TypedDict):
    Region: str,
    Enabled: bool,
```

## UploadUrlMetadataTypeDef

```python
# UploadUrlMetadataTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UploadUrlMetadataTypeDef


def get_value() -> UploadUrlMetadataTypeDef:
    return {
        "Url": ...,
    }


# UploadUrlMetadataTypeDef definition

class UploadUrlMetadataTypeDef(TypedDict):
    Url: NotRequired[str],
    UrlExpiry: NotRequired[str],
    HeadersToInclude: NotRequired[Dict[str, str]],
```

## StartContactEvaluationRequestTypeDef

```python
# StartContactEvaluationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartContactEvaluationRequestTypeDef


def get_value() -> StartContactEvaluationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# StartContactEvaluationRequestTypeDef definition

class StartContactEvaluationRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    EvaluationFormId: str,
    ClientToken: NotRequired[str],
```

## VoiceRecordingConfigurationTypeDef

```python
# VoiceRecordingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import VoiceRecordingConfigurationTypeDef


def get_value() -> VoiceRecordingConfigurationTypeDef:
    return {
        "VoiceRecordingTrack": ...,
    }


# VoiceRecordingConfigurationTypeDef definition

class VoiceRecordingConfigurationTypeDef(TypedDict):
    VoiceRecordingTrack: NotRequired[VoiceRecordingTrackType],  # (1)
    IvrRecordingTrack: NotRequired[IvrRecordingTrackType],  # (2)
```

1. See [:material-code-brackets: VoiceRecordingTrackType](./literals.md#voicerecordingtracktype) 
2. See [:material-code-brackets: IvrRecordingTrackType](./literals.md#ivrrecordingtracktype) 
## StartScreenSharingRequestTypeDef

```python
# StartScreenSharingRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartScreenSharingRequestTypeDef


def get_value() -> StartScreenSharingRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# StartScreenSharingRequestTypeDef definition

class StartScreenSharingRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ClientToken: NotRequired[str],
```

## StopContactRecordingRequestTypeDef

```python
# StopContactRecordingRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StopContactRecordingRequestTypeDef


def get_value() -> StopContactRecordingRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# StopContactRecordingRequestTypeDef definition

class StopContactRecordingRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
    ContactRecordingType: NotRequired[ContactRecordingTypeType],  # (1)
```

1. See [:material-code-brackets: ContactRecordingTypeType](./literals.md#contactrecordingtypetype) 
## StopContactStreamingRequestTypeDef

```python
# StopContactStreamingRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StopContactStreamingRequestTypeDef


def get_value() -> StopContactStreamingRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# StopContactStreamingRequestTypeDef definition

class StopContactStreamingRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    StreamingId: str,
```

## SuspendContactRecordingRequestTypeDef

```python
# SuspendContactRecordingRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SuspendContactRecordingRequestTypeDef


def get_value() -> SuspendContactRecordingRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SuspendContactRecordingRequestTypeDef definition

class SuspendContactRecordingRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
    ContactRecordingType: NotRequired[ContactRecordingTypeType],  # (1)
```

1. See [:material-code-brackets: ContactRecordingTypeType](./literals.md#contactrecordingtypetype) 
## TagContactRequestTypeDef

```python
# TagContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TagContactRequestTypeDef


def get_value() -> TagContactRequestTypeDef:
    return {
        "ContactId": ...,
    }


# TagContactRequestTypeDef definition

class TagContactRequestTypeDef(TypedDict):
    ContactId: str,
    InstanceId: str,
    Tags: Mapping[str, str],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TemplateAttributesTypeDef

```python
# TemplateAttributesTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TemplateAttributesTypeDef


def get_value() -> TemplateAttributesTypeDef:
    return {
        "CustomAttributes": ...,
    }


# TemplateAttributesTypeDef definition

class TemplateAttributesTypeDef(TypedDict):
    CustomAttributes: NotRequired[Mapping[str, str]],
    CustomerProfileAttributes: NotRequired[str],
```

## TranscriptCriteriaTypeDef

```python
# TranscriptCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TranscriptCriteriaTypeDef


def get_value() -> TranscriptCriteriaTypeDef:
    return {
        "ParticipantRole": ...,
    }


# TranscriptCriteriaTypeDef definition

class TranscriptCriteriaTypeDef(TypedDict):
    ParticipantRole: ParticipantRoleType,  # (1)
    SearchText: Sequence[str],
    MatchType: SearchContactsMatchTypeType,  # (2)
```

1. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
2. See [:material-code-brackets: SearchContactsMatchTypeType](./literals.md#searchcontactsmatchtypetype) 
## TransferContactRequestTypeDef

```python
# TransferContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TransferContactRequestTypeDef


def get_value() -> TransferContactRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# TransferContactRequestTypeDef definition

class TransferContactRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ContactFlowId: str,
    QueueId: NotRequired[str],
    UserId: NotRequired[str],
    ClientToken: NotRequired[str],
```

## UntagContactRequestTypeDef

```python
# UntagContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UntagContactRequestTypeDef


def get_value() -> UntagContactRequestTypeDef:
    return {
        "ContactId": ...,
    }


# UntagContactRequestTypeDef definition

class UntagContactRequestTypeDef(TypedDict):
    ContactId: str,
    InstanceId: str,
    TagKeys: Sequence[str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAgentStatusRequestTypeDef

```python
# UpdateAgentStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateAgentStatusRequestTypeDef


def get_value() -> UpdateAgentStatusRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateAgentStatusRequestTypeDef definition

class UpdateAgentStatusRequestTypeDef(TypedDict):
    InstanceId: str,
    AgentStatusId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    State: NotRequired[AgentStatusStateType],  # (1)
    DisplayOrder: NotRequired[int],
    ResetOrderNumber: NotRequired[bool],
```

1. See [:material-code-brackets: AgentStatusStateType](./literals.md#agentstatusstatetype) 
## UpdateAuthenticationProfileRequestTypeDef

```python
# UpdateAuthenticationProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateAuthenticationProfileRequestTypeDef


def get_value() -> UpdateAuthenticationProfileRequestTypeDef:
    return {
        "AuthenticationProfileId": ...,
    }


# UpdateAuthenticationProfileRequestTypeDef definition

class UpdateAuthenticationProfileRequestTypeDef(TypedDict):
    AuthenticationProfileId: str,
    InstanceId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    AllowedIps: NotRequired[Sequence[str]],
    BlockedIps: NotRequired[Sequence[str]],
    PeriodicSessionDuration: NotRequired[int],
```

## UpdateContactAttributesRequestTypeDef

```python
# UpdateContactAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateContactAttributesRequestTypeDef


def get_value() -> UpdateContactAttributesRequestTypeDef:
    return {
        "InitialContactId": ...,
    }


# UpdateContactAttributesRequestTypeDef definition

class UpdateContactAttributesRequestTypeDef(TypedDict):
    InitialContactId: str,
    InstanceId: str,
    Attributes: Mapping[str, str],
```

## UpdateContactFlowContentRequestTypeDef

```python
# UpdateContactFlowContentRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateContactFlowContentRequestTypeDef


def get_value() -> UpdateContactFlowContentRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateContactFlowContentRequestTypeDef definition

class UpdateContactFlowContentRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
    Content: str,
```

## UpdateContactFlowMetadataRequestTypeDef

```python
# UpdateContactFlowMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateContactFlowMetadataRequestTypeDef


def get_value() -> UpdateContactFlowMetadataRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateContactFlowMetadataRequestTypeDef definition

class UpdateContactFlowMetadataRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    ContactFlowState: NotRequired[ContactFlowStateType],  # (1)
```

1. See [:material-code-brackets: ContactFlowStateType](./literals.md#contactflowstatetype) 
## UpdateContactFlowModuleContentRequestTypeDef

```python
# UpdateContactFlowModuleContentRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateContactFlowModuleContentRequestTypeDef


def get_value() -> UpdateContactFlowModuleContentRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateContactFlowModuleContentRequestTypeDef definition

class UpdateContactFlowModuleContentRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowModuleId: str,
    Content: str,
```

## UpdateContactFlowModuleMetadataRequestTypeDef

```python
# UpdateContactFlowModuleMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateContactFlowModuleMetadataRequestTypeDef


def get_value() -> UpdateContactFlowModuleMetadataRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateContactFlowModuleMetadataRequestTypeDef definition

class UpdateContactFlowModuleMetadataRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowModuleId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    State: NotRequired[ContactFlowModuleStateType],  # (1)
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
## UpdateContactFlowNameRequestTypeDef

```python
# UpdateContactFlowNameRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateContactFlowNameRequestTypeDef


def get_value() -> UpdateContactFlowNameRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateContactFlowNameRequestTypeDef definition

class UpdateContactFlowNameRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateEmailAddressMetadataRequestTypeDef

```python
# UpdateEmailAddressMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateEmailAddressMetadataRequestTypeDef


def get_value() -> UpdateEmailAddressMetadataRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateEmailAddressMetadataRequestTypeDef definition

class UpdateEmailAddressMetadataRequestTypeDef(TypedDict):
    InstanceId: str,
    EmailAddressId: str,
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    ClientToken: NotRequired[str],
```

## UpdateInstanceAttributeRequestTypeDef

```python
# UpdateInstanceAttributeRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateInstanceAttributeRequestTypeDef


def get_value() -> UpdateInstanceAttributeRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateInstanceAttributeRequestTypeDef definition

class UpdateInstanceAttributeRequestTypeDef(TypedDict):
    InstanceId: str,
    AttributeType: InstanceAttributeTypeType,  # (1)
    Value: str,
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: InstanceAttributeTypeType](./literals.md#instanceattributetypetype) 
## UpdateParticipantAuthenticationRequestTypeDef

```python
# UpdateParticipantAuthenticationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateParticipantAuthenticationRequestTypeDef


def get_value() -> UpdateParticipantAuthenticationRequestTypeDef:
    return {
        "State": ...,
    }


# UpdateParticipantAuthenticationRequestTypeDef definition

class UpdateParticipantAuthenticationRequestTypeDef(TypedDict):
    State: str,
    InstanceId: str,
    Code: NotRequired[str],
    Error: NotRequired[str],
    ErrorDescription: NotRequired[str],
```

## UpdatePhoneNumberMetadataRequestTypeDef

```python
# UpdatePhoneNumberMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdatePhoneNumberMetadataRequestTypeDef


def get_value() -> UpdatePhoneNumberMetadataRequestTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# UpdatePhoneNumberMetadataRequestTypeDef definition

class UpdatePhoneNumberMetadataRequestTypeDef(TypedDict):
    PhoneNumberId: str,
    PhoneNumberDescription: NotRequired[str],
    ClientToken: NotRequired[str],
```

## UpdatePhoneNumberRequestTypeDef

```python
# UpdatePhoneNumberRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdatePhoneNumberRequestTypeDef


def get_value() -> UpdatePhoneNumberRequestTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# UpdatePhoneNumberRequestTypeDef definition

class UpdatePhoneNumberRequestTypeDef(TypedDict):
    PhoneNumberId: str,
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    ClientToken: NotRequired[str],
```

## UpdatePromptRequestTypeDef

```python
# UpdatePromptRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdatePromptRequestTypeDef


def get_value() -> UpdatePromptRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdatePromptRequestTypeDef definition

class UpdatePromptRequestTypeDef(TypedDict):
    InstanceId: str,
    PromptId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    S3Uri: NotRequired[str],
```

## UpdateQueueHoursOfOperationRequestTypeDef

```python
# UpdateQueueHoursOfOperationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateQueueHoursOfOperationRequestTypeDef


def get_value() -> UpdateQueueHoursOfOperationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateQueueHoursOfOperationRequestTypeDef definition

class UpdateQueueHoursOfOperationRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    HoursOfOperationId: str,
```

## UpdateQueueMaxContactsRequestTypeDef

```python
# UpdateQueueMaxContactsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateQueueMaxContactsRequestTypeDef


def get_value() -> UpdateQueueMaxContactsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateQueueMaxContactsRequestTypeDef definition

class UpdateQueueMaxContactsRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    MaxContacts: NotRequired[int],
```

## UpdateQueueNameRequestTypeDef

```python
# UpdateQueueNameRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateQueueNameRequestTypeDef


def get_value() -> UpdateQueueNameRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateQueueNameRequestTypeDef definition

class UpdateQueueNameRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateQueueStatusRequestTypeDef

```python
# UpdateQueueStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateQueueStatusRequestTypeDef


def get_value() -> UpdateQueueStatusRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateQueueStatusRequestTypeDef definition

class UpdateQueueStatusRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    Status: QueueStatusType,  # (1)
```

1. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
## UpdateQuickConnectNameRequestTypeDef

```python
# UpdateQuickConnectNameRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateQuickConnectNameRequestTypeDef


def get_value() -> UpdateQuickConnectNameRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateQuickConnectNameRequestTypeDef definition

class UpdateQuickConnectNameRequestTypeDef(TypedDict):
    InstanceId: str,
    QuickConnectId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateRoutingProfileAgentAvailabilityTimerRequestTypeDef

```python
# UpdateRoutingProfileAgentAvailabilityTimerRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateRoutingProfileAgentAvailabilityTimerRequestTypeDef


def get_value() -> UpdateRoutingProfileAgentAvailabilityTimerRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateRoutingProfileAgentAvailabilityTimerRequestTypeDef definition

class UpdateRoutingProfileAgentAvailabilityTimerRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    AgentAvailabilityTimer: AgentAvailabilityTimerType,  # (1)
```

1. See [:material-code-brackets: AgentAvailabilityTimerType](./literals.md#agentavailabilitytimertype) 
## UpdateRoutingProfileDefaultOutboundQueueRequestTypeDef

```python
# UpdateRoutingProfileDefaultOutboundQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateRoutingProfileDefaultOutboundQueueRequestTypeDef


def get_value() -> UpdateRoutingProfileDefaultOutboundQueueRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateRoutingProfileDefaultOutboundQueueRequestTypeDef definition

class UpdateRoutingProfileDefaultOutboundQueueRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    DefaultOutboundQueueId: str,
```

## UpdateRoutingProfileNameRequestTypeDef

```python
# UpdateRoutingProfileNameRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateRoutingProfileNameRequestTypeDef


def get_value() -> UpdateRoutingProfileNameRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateRoutingProfileNameRequestTypeDef definition

class UpdateRoutingProfileNameRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateUserHierarchyGroupNameRequestTypeDef

```python
# UpdateUserHierarchyGroupNameRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateUserHierarchyGroupNameRequestTypeDef


def get_value() -> UpdateUserHierarchyGroupNameRequestTypeDef:
    return {
        "Name": ...,
    }


# UpdateUserHierarchyGroupNameRequestTypeDef definition

class UpdateUserHierarchyGroupNameRequestTypeDef(TypedDict):
    Name: str,
    HierarchyGroupId: str,
    InstanceId: str,
```

## UpdateUserHierarchyRequestTypeDef

```python
# UpdateUserHierarchyRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateUserHierarchyRequestTypeDef


def get_value() -> UpdateUserHierarchyRequestTypeDef:
    return {
        "UserId": ...,
    }


# UpdateUserHierarchyRequestTypeDef definition

class UpdateUserHierarchyRequestTypeDef(TypedDict):
    UserId: str,
    InstanceId: str,
    HierarchyGroupId: NotRequired[str],
```

## UpdateUserRoutingProfileRequestTypeDef

```python
# UpdateUserRoutingProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateUserRoutingProfileRequestTypeDef


def get_value() -> UpdateUserRoutingProfileRequestTypeDef:
    return {
        "RoutingProfileId": ...,
    }


# UpdateUserRoutingProfileRequestTypeDef definition

class UpdateUserRoutingProfileRequestTypeDef(TypedDict):
    RoutingProfileId: str,
    UserId: str,
    InstanceId: str,
```

## UpdateUserSecurityProfilesRequestTypeDef

```python
# UpdateUserSecurityProfilesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateUserSecurityProfilesRequestTypeDef


def get_value() -> UpdateUserSecurityProfilesRequestTypeDef:
    return {
        "SecurityProfileIds": ...,
    }


# UpdateUserSecurityProfilesRequestTypeDef definition

class UpdateUserSecurityProfilesRequestTypeDef(TypedDict):
    SecurityProfileIds: Sequence[str],
    UserId: str,
    InstanceId: str,
```

## UpdateViewMetadataRequestTypeDef

```python
# UpdateViewMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateViewMetadataRequestTypeDef


def get_value() -> UpdateViewMetadataRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateViewMetadataRequestTypeDef definition

class UpdateViewMetadataRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UserReferenceTypeDef

```python
# UserReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserReferenceTypeDef


def get_value() -> UserReferenceTypeDef:
    return {
        "Id": ...,
    }


# UserReferenceTypeDef definition

class UserReferenceTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
```

## UserIdentityInfoLiteTypeDef

```python
# UserIdentityInfoLiteTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserIdentityInfoLiteTypeDef


def get_value() -> UserIdentityInfoLiteTypeDef:
    return {
        "FirstName": ...,
    }


# UserIdentityInfoLiteTypeDef definition

class UserIdentityInfoLiteTypeDef(TypedDict):
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
```

## ViewContentTypeDef

```python
# ViewContentTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ViewContentTypeDef


def get_value() -> ViewContentTypeDef:
    return {
        "InputSchema": ...,
    }


# ViewContentTypeDef definition

class ViewContentTypeDef(TypedDict):
    InputSchema: NotRequired[str],
    Template: NotRequired[str],
    Actions: NotRequired[List[str]],
```

## RuleSummaryTypeDef

```python
# RuleSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RuleSummaryTypeDef


def get_value() -> RuleSummaryTypeDef:
    return {
        "Name": ...,
    }


# RuleSummaryTypeDef definition

class RuleSummaryTypeDef(TypedDict):
    Name: str,
    RuleId: str,
    RuleArn: str,
    EventSourceName: EventSourceNameType,  # (1)
    PublishStatus: RulePublishStatusType,  # (2)
    ActionSummaries: List[ActionSummaryTypeDef],  # (3)
    CreatedTime: datetime,
    LastUpdatedTime: datetime,
```

1. See [:material-code-brackets: EventSourceNameType](./literals.md#eventsourcenametype) 
2. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
3. See [:material-code-braces: ActionSummaryTypeDef](./type_defs.md#actionsummarytypedef) 
## ActivateEvaluationFormResponseTypeDef

```python
# ActivateEvaluationFormResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ActivateEvaluationFormResponseTypeDef


def get_value() -> ActivateEvaluationFormResponseTypeDef:
    return {
        "EvaluationFormId": ...,
    }


# ActivateEvaluationFormResponseTypeDef definition

class ActivateEvaluationFormResponseTypeDef(TypedDict):
    EvaluationFormId: str,
    EvaluationFormArn: str,
    EvaluationFormVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateAnalyticsDataSetResponseTypeDef

```python
# AssociateAnalyticsDataSetResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateAnalyticsDataSetResponseTypeDef


def get_value() -> AssociateAnalyticsDataSetResponseTypeDef:
    return {
        "DataSetId": ...,
    }


# AssociateAnalyticsDataSetResponseTypeDef definition

class AssociateAnalyticsDataSetResponseTypeDef(TypedDict):
    DataSetId: str,
    TargetAccountId: str,
    ResourceShareId: str,
    ResourceShareArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateInstanceStorageConfigResponseTypeDef

```python
# AssociateInstanceStorageConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateInstanceStorageConfigResponseTypeDef


def get_value() -> AssociateInstanceStorageConfigResponseTypeDef:
    return {
        "AssociationId": ...,
    }


# AssociateInstanceStorageConfigResponseTypeDef definition

class AssociateInstanceStorageConfigResponseTypeDef(TypedDict):
    AssociationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateSecurityKeyResponseTypeDef

```python
# AssociateSecurityKeyResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateSecurityKeyResponseTypeDef


def get_value() -> AssociateSecurityKeyResponseTypeDef:
    return {
        "AssociationId": ...,
    }


# AssociateSecurityKeyResponseTypeDef definition

class AssociateSecurityKeyResponseTypeDef(TypedDict):
    AssociationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClaimPhoneNumberResponseTypeDef

```python
# ClaimPhoneNumberResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ClaimPhoneNumberResponseTypeDef


def get_value() -> ClaimPhoneNumberResponseTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# ClaimPhoneNumberResponseTypeDef definition

class ClaimPhoneNumberResponseTypeDef(TypedDict):
    PhoneNumberId: str,
    PhoneNumberArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAgentStatusResponseTypeDef

```python
# CreateAgentStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateAgentStatusResponseTypeDef


def get_value() -> CreateAgentStatusResponseTypeDef:
    return {
        "AgentStatusARN": ...,
    }


# CreateAgentStatusResponseTypeDef definition

class CreateAgentStatusResponseTypeDef(TypedDict):
    AgentStatusARN: str,
    AgentStatusId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContactFlowModuleResponseTypeDef

```python
# CreateContactFlowModuleResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateContactFlowModuleResponseTypeDef


def get_value() -> CreateContactFlowModuleResponseTypeDef:
    return {
        "Id": ...,
    }


# CreateContactFlowModuleResponseTypeDef definition

class CreateContactFlowModuleResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContactFlowResponseTypeDef

```python
# CreateContactFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateContactFlowResponseTypeDef


def get_value() -> CreateContactFlowResponseTypeDef:
    return {
        "ContactFlowId": ...,
    }


# CreateContactFlowResponseTypeDef definition

class CreateContactFlowResponseTypeDef(TypedDict):
    ContactFlowId: str,
    ContactFlowArn: str,
    FlowContentSha256: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContactFlowVersionResponseTypeDef

```python
# CreateContactFlowVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateContactFlowVersionResponseTypeDef


def get_value() -> CreateContactFlowVersionResponseTypeDef:
    return {
        "ContactFlowArn": ...,
    }


# CreateContactFlowVersionResponseTypeDef definition

class CreateContactFlowVersionResponseTypeDef(TypedDict):
    ContactFlowArn: str,
    Version: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContactResponseTypeDef

```python
# CreateContactResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateContactResponseTypeDef


def get_value() -> CreateContactResponseTypeDef:
    return {
        "ContactId": ...,
    }


# CreateContactResponseTypeDef definition

class CreateContactResponseTypeDef(TypedDict):
    ContactId: str,
    ContactArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEmailAddressResponseTypeDef

```python
# CreateEmailAddressResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateEmailAddressResponseTypeDef


def get_value() -> CreateEmailAddressResponseTypeDef:
    return {
        "EmailAddressId": ...,
    }


# CreateEmailAddressResponseTypeDef definition

class CreateEmailAddressResponseTypeDef(TypedDict):
    EmailAddressId: str,
    EmailAddressArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEvaluationFormResponseTypeDef

```python
# CreateEvaluationFormResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateEvaluationFormResponseTypeDef


def get_value() -> CreateEvaluationFormResponseTypeDef:
    return {
        "EvaluationFormId": ...,
    }


# CreateEvaluationFormResponseTypeDef definition

class CreateEvaluationFormResponseTypeDef(TypedDict):
    EvaluationFormId: str,
    EvaluationFormArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHoursOfOperationOverrideResponseTypeDef

```python
# CreateHoursOfOperationOverrideResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateHoursOfOperationOverrideResponseTypeDef


def get_value() -> CreateHoursOfOperationOverrideResponseTypeDef:
    return {
        "HoursOfOperationOverrideId": ...,
    }


# CreateHoursOfOperationOverrideResponseTypeDef definition

class CreateHoursOfOperationOverrideResponseTypeDef(TypedDict):
    HoursOfOperationOverrideId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHoursOfOperationResponseTypeDef

```python
# CreateHoursOfOperationResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateHoursOfOperationResponseTypeDef


def get_value() -> CreateHoursOfOperationResponseTypeDef:
    return {
        "HoursOfOperationId": ...,
    }


# CreateHoursOfOperationResponseTypeDef definition

class CreateHoursOfOperationResponseTypeDef(TypedDict):
    HoursOfOperationId: str,
    HoursOfOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceResponseTypeDef

```python
# CreateInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateInstanceResponseTypeDef


def get_value() -> CreateInstanceResponseTypeDef:
    return {
        "Id": ...,
    }


# CreateInstanceResponseTypeDef definition

class CreateInstanceResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIntegrationAssociationResponseTypeDef

```python
# CreateIntegrationAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateIntegrationAssociationResponseTypeDef


def get_value() -> CreateIntegrationAssociationResponseTypeDef:
    return {
        "IntegrationAssociationId": ...,
    }


# CreateIntegrationAssociationResponseTypeDef definition

class CreateIntegrationAssociationResponseTypeDef(TypedDict):
    IntegrationAssociationId: str,
    IntegrationAssociationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePersistentContactAssociationResponseTypeDef

```python
# CreatePersistentContactAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreatePersistentContactAssociationResponseTypeDef


def get_value() -> CreatePersistentContactAssociationResponseTypeDef:
    return {
        "ContinuedFromContactId": ...,
    }


# CreatePersistentContactAssociationResponseTypeDef definition

class CreatePersistentContactAssociationResponseTypeDef(TypedDict):
    ContinuedFromContactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePromptResponseTypeDef

```python
# CreatePromptResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreatePromptResponseTypeDef


def get_value() -> CreatePromptResponseTypeDef:
    return {
        "PromptARN": ...,
    }


# CreatePromptResponseTypeDef definition

class CreatePromptResponseTypeDef(TypedDict):
    PromptARN: str,
    PromptId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePushNotificationRegistrationResponseTypeDef

```python
# CreatePushNotificationRegistrationResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreatePushNotificationRegistrationResponseTypeDef


def get_value() -> CreatePushNotificationRegistrationResponseTypeDef:
    return {
        "RegistrationId": ...,
    }


# CreatePushNotificationRegistrationResponseTypeDef definition

class CreatePushNotificationRegistrationResponseTypeDef(TypedDict):
    RegistrationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQueueResponseTypeDef

```python
# CreateQueueResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateQueueResponseTypeDef


def get_value() -> CreateQueueResponseTypeDef:
    return {
        "QueueArn": ...,
    }


# CreateQueueResponseTypeDef definition

class CreateQueueResponseTypeDef(TypedDict):
    QueueArn: str,
    QueueId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQuickConnectResponseTypeDef

```python
# CreateQuickConnectResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateQuickConnectResponseTypeDef


def get_value() -> CreateQuickConnectResponseTypeDef:
    return {
        "QuickConnectARN": ...,
    }


# CreateQuickConnectResponseTypeDef definition

class CreateQuickConnectResponseTypeDef(TypedDict):
    QuickConnectARN: str,
    QuickConnectId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRoutingProfileResponseTypeDef

```python
# CreateRoutingProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateRoutingProfileResponseTypeDef


def get_value() -> CreateRoutingProfileResponseTypeDef:
    return {
        "RoutingProfileArn": ...,
    }


# CreateRoutingProfileResponseTypeDef definition

class CreateRoutingProfileResponseTypeDef(TypedDict):
    RoutingProfileArn: str,
    RoutingProfileId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleResponseTypeDef

```python
# CreateRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateRuleResponseTypeDef


def get_value() -> CreateRuleResponseTypeDef:
    return {
        "RuleArn": ...,
    }


# CreateRuleResponseTypeDef definition

class CreateRuleResponseTypeDef(TypedDict):
    RuleArn: str,
    RuleId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSecurityProfileResponseTypeDef

```python
# CreateSecurityProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateSecurityProfileResponseTypeDef


def get_value() -> CreateSecurityProfileResponseTypeDef:
    return {
        "SecurityProfileId": ...,
    }


# CreateSecurityProfileResponseTypeDef definition

class CreateSecurityProfileResponseTypeDef(TypedDict):
    SecurityProfileId: str,
    SecurityProfileArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTaskTemplateResponseTypeDef

```python
# CreateTaskTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateTaskTemplateResponseTypeDef


def get_value() -> CreateTaskTemplateResponseTypeDef:
    return {
        "Id": ...,
    }


# CreateTaskTemplateResponseTypeDef definition

class CreateTaskTemplateResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrafficDistributionGroupResponseTypeDef

```python
# CreateTrafficDistributionGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateTrafficDistributionGroupResponseTypeDef


def get_value() -> CreateTrafficDistributionGroupResponseTypeDef:
    return {
        "Id": ...,
    }


# CreateTrafficDistributionGroupResponseTypeDef definition

class CreateTrafficDistributionGroupResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUseCaseResponseTypeDef

```python
# CreateUseCaseResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateUseCaseResponseTypeDef


def get_value() -> CreateUseCaseResponseTypeDef:
    return {
        "UseCaseId": ...,
    }


# CreateUseCaseResponseTypeDef definition

class CreateUseCaseResponseTypeDef(TypedDict):
    UseCaseId: str,
    UseCaseArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserHierarchyGroupResponseTypeDef

```python
# CreateUserHierarchyGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateUserHierarchyGroupResponseTypeDef


def get_value() -> CreateUserHierarchyGroupResponseTypeDef:
    return {
        "HierarchyGroupId": ...,
    }


# CreateUserHierarchyGroupResponseTypeDef definition

class CreateUserHierarchyGroupResponseTypeDef(TypedDict):
    HierarchyGroupId: str,
    HierarchyGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserResponseTypeDef

```python
# CreateUserResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateUserResponseTypeDef


def get_value() -> CreateUserResponseTypeDef:
    return {
        "UserId": ...,
    }


# CreateUserResponseTypeDef definition

class CreateUserResponseTypeDef(TypedDict):
    UserId: str,
    UserArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVocabularyResponseTypeDef

```python
# CreateVocabularyResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateVocabularyResponseTypeDef


def get_value() -> CreateVocabularyResponseTypeDef:
    return {
        "VocabularyArn": ...,
    }


# CreateVocabularyResponseTypeDef definition

class CreateVocabularyResponseTypeDef(TypedDict):
    VocabularyArn: str,
    VocabularyId: str,
    State: VocabularyStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeactivateEvaluationFormResponseTypeDef

```python
# DeactivateEvaluationFormResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeactivateEvaluationFormResponseTypeDef


def get_value() -> DeactivateEvaluationFormResponseTypeDef:
    return {
        "EvaluationFormId": ...,
    }


# DeactivateEvaluationFormResponseTypeDef definition

class DeactivateEvaluationFormResponseTypeDef(TypedDict):
    EvaluationFormId: str,
    EvaluationFormArn: str,
    EvaluationFormVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVocabularyResponseTypeDef

```python
# DeleteVocabularyResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DeleteVocabularyResponseTypeDef


def get_value() -> DeleteVocabularyResponseTypeDef:
    return {
        "VocabularyArn": ...,
    }


# DeleteVocabularyResponseTypeDef definition

class DeleteVocabularyResponseTypeDef(TypedDict):
    VocabularyArn: str,
    VocabularyId: str,
    State: VocabularyStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEmailAddressResponseTypeDef

```python
# DescribeEmailAddressResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeEmailAddressResponseTypeDef


def get_value() -> DescribeEmailAddressResponseTypeDef:
    return {
        "EmailAddressId": ...,
    }


# DescribeEmailAddressResponseTypeDef definition

class DescribeEmailAddressResponseTypeDef(TypedDict):
    EmailAddressId: str,
    EmailAddressArn: str,
    EmailAddress: str,
    DisplayName: str,
    Description: str,
    CreateTimestamp: str,
    ModifiedTimestamp: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContactAttributesResponseTypeDef

```python
# GetContactAttributesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetContactAttributesResponseTypeDef


def get_value() -> GetContactAttributesResponseTypeDef:
    return {
        "Attributes": ...,
    }


# GetContactAttributesResponseTypeDef definition

class GetContactAttributesResponseTypeDef(TypedDict):
    Attributes: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFlowAssociationResponseTypeDef

```python
# GetFlowAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetFlowAssociationResponseTypeDef


def get_value() -> GetFlowAssociationResponseTypeDef:
    return {
        "ResourceId": ...,
    }


# GetFlowAssociationResponseTypeDef definition

class GetFlowAssociationResponseTypeDef(TypedDict):
    ResourceId: str,
    FlowId: str,
    ResourceType: FlowAssociationResourceTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FlowAssociationResourceTypeType](./literals.md#flowassociationresourcetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPromptFileResponseTypeDef

```python
# GetPromptFileResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetPromptFileResponseTypeDef


def get_value() -> GetPromptFileResponseTypeDef:
    return {
        "PromptPresignedUrl": ...,
    }


# GetPromptFileResponseTypeDef definition

class GetPromptFileResponseTypeDef(TypedDict):
    PromptPresignedUrl: str,
    LastModifiedTime: datetime,
    LastModifiedRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportPhoneNumberResponseTypeDef

```python
# ImportPhoneNumberResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ImportPhoneNumberResponseTypeDef


def get_value() -> ImportPhoneNumberResponseTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# ImportPhoneNumberResponseTypeDef definition

class ImportPhoneNumberResponseTypeDef(TypedDict):
    PhoneNumberId: str,
    PhoneNumberArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApprovedOriginsResponseTypeDef

```python
# ListApprovedOriginsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListApprovedOriginsResponseTypeDef


def get_value() -> ListApprovedOriginsResponseTypeDef:
    return {
        "Origins": ...,
    }


# ListApprovedOriginsResponseTypeDef definition

class ListApprovedOriginsResponseTypeDef(TypedDict):
    Origins: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLambdaFunctionsResponseTypeDef

```python
# ListLambdaFunctionsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListLambdaFunctionsResponseTypeDef


def get_value() -> ListLambdaFunctionsResponseTypeDef:
    return {
        "LambdaFunctions": ...,
    }


# ListLambdaFunctionsResponseTypeDef definition

class ListLambdaFunctionsResponseTypeDef(TypedDict):
    LambdaFunctions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecurityProfilePermissionsResponseTypeDef

```python
# ListSecurityProfilePermissionsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListSecurityProfilePermissionsResponseTypeDef


def get_value() -> ListSecurityProfilePermissionsResponseTypeDef:
    return {
        "Permissions": ...,
    }


# ListSecurityProfilePermissionsResponseTypeDef definition

class ListSecurityProfilePermissionsResponseTypeDef(TypedDict):
    Permissions: List[str],
    LastModifiedTime: datetime,
    LastModifiedRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MonitorContactResponseTypeDef

```python
# MonitorContactResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MonitorContactResponseTypeDef


def get_value() -> MonitorContactResponseTypeDef:
    return {
        "ContactId": ...,
    }


# MonitorContactResponseTypeDef definition

class MonitorContactResponseTypeDef(TypedDict):
    ContactId: str,
    ContactArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicateInstanceResponseTypeDef

```python
# ReplicateInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ReplicateInstanceResponseTypeDef


def get_value() -> ReplicateInstanceResponseTypeDef:
    return {
        "Id": ...,
    }


# ReplicateInstanceResponseTypeDef definition

class ReplicateInstanceResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendChatIntegrationEventResponseTypeDef

```python
# SendChatIntegrationEventResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SendChatIntegrationEventResponseTypeDef


def get_value() -> SendChatIntegrationEventResponseTypeDef:
    return {
        "InitialContactId": ...,
    }


# SendChatIntegrationEventResponseTypeDef definition

class SendChatIntegrationEventResponseTypeDef(TypedDict):
    InitialContactId: str,
    NewChatCreated: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartChatContactResponseTypeDef

```python
# StartChatContactResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartChatContactResponseTypeDef


def get_value() -> StartChatContactResponseTypeDef:
    return {
        "ContactId": ...,
    }


# StartChatContactResponseTypeDef definition

class StartChatContactResponseTypeDef(TypedDict):
    ContactId: str,
    ParticipantId: str,
    ParticipantToken: str,
    ContinuedFromContactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartContactEvaluationResponseTypeDef

```python
# StartContactEvaluationResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartContactEvaluationResponseTypeDef


def get_value() -> StartContactEvaluationResponseTypeDef:
    return {
        "EvaluationId": ...,
    }


# StartContactEvaluationResponseTypeDef definition

class StartContactEvaluationResponseTypeDef(TypedDict):
    EvaluationId: str,
    EvaluationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartContactStreamingResponseTypeDef

```python
# StartContactStreamingResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartContactStreamingResponseTypeDef


def get_value() -> StartContactStreamingResponseTypeDef:
    return {
        "StreamingId": ...,
    }


# StartContactStreamingResponseTypeDef definition

class StartContactStreamingResponseTypeDef(TypedDict):
    StreamingId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartEmailContactResponseTypeDef

```python
# StartEmailContactResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartEmailContactResponseTypeDef


def get_value() -> StartEmailContactResponseTypeDef:
    return {
        "ContactId": ...,
    }


# StartEmailContactResponseTypeDef definition

class StartEmailContactResponseTypeDef(TypedDict):
    ContactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartOutboundChatContactResponseTypeDef

```python
# StartOutboundChatContactResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartOutboundChatContactResponseTypeDef


def get_value() -> StartOutboundChatContactResponseTypeDef:
    return {
        "ContactId": ...,
    }


# StartOutboundChatContactResponseTypeDef definition

class StartOutboundChatContactResponseTypeDef(TypedDict):
    ContactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartOutboundEmailContactResponseTypeDef

```python
# StartOutboundEmailContactResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartOutboundEmailContactResponseTypeDef


def get_value() -> StartOutboundEmailContactResponseTypeDef:
    return {
        "ContactId": ...,
    }


# StartOutboundEmailContactResponseTypeDef definition

class StartOutboundEmailContactResponseTypeDef(TypedDict):
    ContactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartOutboundVoiceContactResponseTypeDef

```python
# StartOutboundVoiceContactResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartOutboundVoiceContactResponseTypeDef


def get_value() -> StartOutboundVoiceContactResponseTypeDef:
    return {
        "ContactId": ...,
    }


# StartOutboundVoiceContactResponseTypeDef definition

class StartOutboundVoiceContactResponseTypeDef(TypedDict):
    ContactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTaskContactResponseTypeDef

```python
# StartTaskContactResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartTaskContactResponseTypeDef


def get_value() -> StartTaskContactResponseTypeDef:
    return {
        "ContactId": ...,
    }


# StartTaskContactResponseTypeDef definition

class StartTaskContactResponseTypeDef(TypedDict):
    ContactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubmitContactEvaluationResponseTypeDef

```python
# SubmitContactEvaluationResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SubmitContactEvaluationResponseTypeDef


def get_value() -> SubmitContactEvaluationResponseTypeDef:
    return {
        "EvaluationId": ...,
    }


# SubmitContactEvaluationResponseTypeDef definition

class SubmitContactEvaluationResponseTypeDef(TypedDict):
    EvaluationId: str,
    EvaluationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransferContactResponseTypeDef

```python
# TransferContactResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TransferContactResponseTypeDef


def get_value() -> TransferContactResponseTypeDef:
    return {
        "ContactId": ...,
    }


# TransferContactResponseTypeDef definition

class TransferContactResponseTypeDef(TypedDict):
    ContactId: str,
    ContactArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContactEvaluationResponseTypeDef

```python
# UpdateContactEvaluationResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateContactEvaluationResponseTypeDef


def get_value() -> UpdateContactEvaluationResponseTypeDef:
    return {
        "EvaluationId": ...,
    }


# UpdateContactEvaluationResponseTypeDef definition

class UpdateContactEvaluationResponseTypeDef(TypedDict):
    EvaluationId: str,
    EvaluationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEmailAddressMetadataResponseTypeDef

```python
# UpdateEmailAddressMetadataResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateEmailAddressMetadataResponseTypeDef


def get_value() -> UpdateEmailAddressMetadataResponseTypeDef:
    return {
        "EmailAddressId": ...,
    }


# UpdateEmailAddressMetadataResponseTypeDef definition

class UpdateEmailAddressMetadataResponseTypeDef(TypedDict):
    EmailAddressId: str,
    EmailAddressArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEvaluationFormResponseTypeDef

```python
# UpdateEvaluationFormResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateEvaluationFormResponseTypeDef


def get_value() -> UpdateEvaluationFormResponseTypeDef:
    return {
        "EvaluationFormId": ...,
    }


# UpdateEvaluationFormResponseTypeDef definition

class UpdateEvaluationFormResponseTypeDef(TypedDict):
    EvaluationFormId: str,
    EvaluationFormArn: str,
    EvaluationFormVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePhoneNumberResponseTypeDef

```python
# UpdatePhoneNumberResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdatePhoneNumberResponseTypeDef


def get_value() -> UpdatePhoneNumberResponseTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# UpdatePhoneNumberResponseTypeDef definition

class UpdatePhoneNumberResponseTypeDef(TypedDict):
    PhoneNumberId: str,
    PhoneNumberArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePromptResponseTypeDef

```python
# UpdatePromptResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdatePromptResponseTypeDef


def get_value() -> UpdatePromptResponseTypeDef:
    return {
        "PromptARN": ...,
    }


# UpdatePromptResponseTypeDef definition

class UpdatePromptResponseTypeDef(TypedDict):
    PromptARN: str,
    PromptId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdditionalEmailRecipientsTypeDef

```python
# AdditionalEmailRecipientsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AdditionalEmailRecipientsTypeDef


def get_value() -> AdditionalEmailRecipientsTypeDef:
    return {
        "ToList": ...,
    }


# AdditionalEmailRecipientsTypeDef definition

class AdditionalEmailRecipientsTypeDef(TypedDict):
    ToList: NotRequired[List[EmailRecipientTypeDef]],  # (1)
    CcList: NotRequired[List[EmailRecipientTypeDef]],  # (1)
```

1. See [:material-code-braces: EmailRecipientTypeDef](./type_defs.md#emailrecipienttypedef) 
2. See [:material-code-braces: EmailRecipientTypeDef](./type_defs.md#emailrecipienttypedef) 
## AgentConfigOutputTypeDef

```python
# AgentConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentConfigOutputTypeDef


def get_value() -> AgentConfigOutputTypeDef:
    return {
        "Distributions": ...,
    }


# AgentConfigOutputTypeDef definition

class AgentConfigOutputTypeDef(TypedDict):
    Distributions: List[DistributionTypeDef],  # (1)
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
## AgentConfigTypeDef

```python
# AgentConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentConfigTypeDef


def get_value() -> AgentConfigTypeDef:
    return {
        "Distributions": ...,
    }


# AgentConfigTypeDef definition

class AgentConfigTypeDef(TypedDict):
    Distributions: Sequence[DistributionTypeDef],  # (1)
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
## TelephonyConfigOutputTypeDef

```python
# TelephonyConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TelephonyConfigOutputTypeDef


def get_value() -> TelephonyConfigOutputTypeDef:
    return {
        "Distributions": ...,
    }


# TelephonyConfigOutputTypeDef definition

class TelephonyConfigOutputTypeDef(TypedDict):
    Distributions: List[DistributionTypeDef],  # (1)
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
## TelephonyConfigTypeDef

```python
# TelephonyConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TelephonyConfigTypeDef


def get_value() -> TelephonyConfigTypeDef:
    return {
        "Distributions": ...,
    }


# TelephonyConfigTypeDef definition

class TelephonyConfigTypeDef(TypedDict):
    Distributions: Sequence[DistributionTypeDef],  # (1)
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
## AgentContactReferenceTypeDef

```python
# AgentContactReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentContactReferenceTypeDef


def get_value() -> AgentContactReferenceTypeDef:
    return {
        "ContactId": ...,
    }


# AgentContactReferenceTypeDef definition

class AgentContactReferenceTypeDef(TypedDict):
    ContactId: NotRequired[str],
    Channel: NotRequired[ChannelType],  # (1)
    InitiationMethod: NotRequired[ContactInitiationMethodType],  # (2)
    AgentContactState: NotRequired[ContactStateType],  # (3)
    StateStartTimestamp: NotRequired[datetime],
    ConnectedToAgentTimestamp: NotRequired[datetime],
    Queue: NotRequired[QueueReferenceTypeDef],  # (4)
```

1. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
2. See [:material-code-brackets: ContactInitiationMethodType](./literals.md#contactinitiationmethodtype) 
3. See [:material-code-brackets: ContactStateType](./literals.md#contactstatetype) 
4. See [:material-code-braces: QueueReferenceTypeDef](./type_defs.md#queuereferencetypedef) 
## HierarchyGroupsTypeDef

```python
# HierarchyGroupsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HierarchyGroupsTypeDef


def get_value() -> HierarchyGroupsTypeDef:
    return {
        "Level1": ...,
    }


# HierarchyGroupsTypeDef definition

class HierarchyGroupsTypeDef(TypedDict):
    Level1: NotRequired[AgentHierarchyGroupTypeDef],  # (1)
    Level2: NotRequired[AgentHierarchyGroupTypeDef],  # (1)
    Level3: NotRequired[AgentHierarchyGroupTypeDef],  # (1)
    Level4: NotRequired[AgentHierarchyGroupTypeDef],  # (1)
    Level5: NotRequired[AgentHierarchyGroupTypeDef],  # (1)
```

1. See [:material-code-braces: AgentHierarchyGroupTypeDef](./type_defs.md#agenthierarchygrouptypedef) 
2. See [:material-code-braces: AgentHierarchyGroupTypeDef](./type_defs.md#agenthierarchygrouptypedef) 
3. See [:material-code-braces: AgentHierarchyGroupTypeDef](./type_defs.md#agenthierarchygrouptypedef) 
4. See [:material-code-braces: AgentHierarchyGroupTypeDef](./type_defs.md#agenthierarchygrouptypedef) 
5. See [:material-code-braces: AgentHierarchyGroupTypeDef](./type_defs.md#agenthierarchygrouptypedef) 
## AllowedCapabilitiesTypeDef

```python
# AllowedCapabilitiesTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AllowedCapabilitiesTypeDef


def get_value() -> AllowedCapabilitiesTypeDef:
    return {
        "Customer": ...,
    }


# AllowedCapabilitiesTypeDef definition

class AllowedCapabilitiesTypeDef(TypedDict):
    Customer: NotRequired[ParticipantCapabilitiesTypeDef],  # (1)
    Agent: NotRequired[ParticipantCapabilitiesTypeDef],  # (1)
```

1. See [:material-code-braces: ParticipantCapabilitiesTypeDef](./type_defs.md#participantcapabilitiestypedef) 
2. See [:material-code-braces: ParticipantCapabilitiesTypeDef](./type_defs.md#participantcapabilitiestypedef) 
## CustomerTypeDef

```python
# CustomerTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CustomerTypeDef


def get_value() -> CustomerTypeDef:
    return {
        "DeviceInfo": ...,
    }


# CustomerTypeDef definition

class CustomerTypeDef(TypedDict):
    DeviceInfo: NotRequired[DeviceInfoTypeDef],  # (1)
    Capabilities: NotRequired[ParticipantCapabilitiesTypeDef],  # (2)
```

1. See [:material-code-braces: DeviceInfoTypeDef](./type_defs.md#deviceinfotypedef) 
2. See [:material-code-braces: ParticipantCapabilitiesTypeDef](./type_defs.md#participantcapabilitiestypedef) 
## AgentQualityMetricsTypeDef

```python
# AgentQualityMetricsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentQualityMetricsTypeDef


def get_value() -> AgentQualityMetricsTypeDef:
    return {
        "Audio": ...,
    }


# AgentQualityMetricsTypeDef definition

class AgentQualityMetricsTypeDef(TypedDict):
    Audio: NotRequired[AudioQualityMetricsInfoTypeDef],  # (1)
```

1. See [:material-code-braces: AudioQualityMetricsInfoTypeDef](./type_defs.md#audioqualitymetricsinfotypedef) 
## CustomerQualityMetricsTypeDef

```python
# CustomerQualityMetricsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CustomerQualityMetricsTypeDef


def get_value() -> CustomerQualityMetricsTypeDef:
    return {
        "Audio": ...,
    }


# CustomerQualityMetricsTypeDef definition

class CustomerQualityMetricsTypeDef(TypedDict):
    Audio: NotRequired[AudioQualityMetricsInfoTypeDef],  # (1)
```

1. See [:material-code-braces: AudioQualityMetricsInfoTypeDef](./type_defs.md#audioqualitymetricsinfotypedef) 
## AgentStatusSearchCriteriaPaginatorTypeDef

```python
# AgentStatusSearchCriteriaPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentStatusSearchCriteriaPaginatorTypeDef


def get_value() -> AgentStatusSearchCriteriaPaginatorTypeDef:
    return {
        "OrConditions": ...,
    }


# AgentStatusSearchCriteriaPaginatorTypeDef definition

class AgentStatusSearchCriteriaPaginatorTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## AgentStatusSearchCriteriaTypeDef

```python
# AgentStatusSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentStatusSearchCriteriaTypeDef


def get_value() -> AgentStatusSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# AgentStatusSearchCriteriaTypeDef definition

class AgentStatusSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## ContactFlowModuleSearchCriteriaPaginatorTypeDef

```python
# ContactFlowModuleSearchCriteriaPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactFlowModuleSearchCriteriaPaginatorTypeDef


def get_value() -> ContactFlowModuleSearchCriteriaPaginatorTypeDef:
    return {
        "OrConditions": ...,
    }


# ContactFlowModuleSearchCriteriaPaginatorTypeDef definition

class ContactFlowModuleSearchCriteriaPaginatorTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
    StateCondition: NotRequired[ContactFlowModuleStateType],  # (2)
    StatusCondition: NotRequired[ContactFlowModuleStatusType],  # (3)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
3. See [:material-code-brackets: ContactFlowModuleStatusType](./literals.md#contactflowmodulestatustype) 
## ContactFlowModuleSearchCriteriaTypeDef

```python
# ContactFlowModuleSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactFlowModuleSearchCriteriaTypeDef


def get_value() -> ContactFlowModuleSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# ContactFlowModuleSearchCriteriaTypeDef definition

class ContactFlowModuleSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
    StateCondition: NotRequired[ContactFlowModuleStateType],  # (2)
    StatusCondition: NotRequired[ContactFlowModuleStatusType],  # (3)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
3. See [:material-code-brackets: ContactFlowModuleStatusType](./literals.md#contactflowmodulestatustype) 
## ContactFlowSearchCriteriaPaginatorTypeDef

```python
# ContactFlowSearchCriteriaPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactFlowSearchCriteriaPaginatorTypeDef


def get_value() -> ContactFlowSearchCriteriaPaginatorTypeDef:
    return {
        "OrConditions": ...,
    }


# ContactFlowSearchCriteriaPaginatorTypeDef definition

class ContactFlowSearchCriteriaPaginatorTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
    TypeCondition: NotRequired[ContactFlowTypeType],  # (2)
    StateCondition: NotRequired[ContactFlowStateType],  # (3)
    StatusCondition: NotRequired[ContactFlowStatusType],  # (4)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
3. See [:material-code-brackets: ContactFlowStateType](./literals.md#contactflowstatetype) 
4. See [:material-code-brackets: ContactFlowStatusType](./literals.md#contactflowstatustype) 
## ContactFlowSearchCriteriaTypeDef

```python
# ContactFlowSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactFlowSearchCriteriaTypeDef


def get_value() -> ContactFlowSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# ContactFlowSearchCriteriaTypeDef definition

class ContactFlowSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
    TypeCondition: NotRequired[ContactFlowTypeType],  # (2)
    StateCondition: NotRequired[ContactFlowStateType],  # (3)
    StatusCondition: NotRequired[ContactFlowStatusType],  # (4)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
3. See [:material-code-brackets: ContactFlowStateType](./literals.md#contactflowstatetype) 
4. See [:material-code-brackets: ContactFlowStatusType](./literals.md#contactflowstatustype) 
## EmailAddressSearchCriteriaTypeDef

```python
# EmailAddressSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EmailAddressSearchCriteriaTypeDef


def get_value() -> EmailAddressSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# EmailAddressSearchCriteriaTypeDef definition

class EmailAddressSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## HoursOfOperationSearchCriteriaPaginatorTypeDef

```python
# HoursOfOperationSearchCriteriaPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HoursOfOperationSearchCriteriaPaginatorTypeDef


def get_value() -> HoursOfOperationSearchCriteriaPaginatorTypeDef:
    return {
        "OrConditions": ...,
    }


# HoursOfOperationSearchCriteriaPaginatorTypeDef definition

class HoursOfOperationSearchCriteriaPaginatorTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## HoursOfOperationSearchCriteriaTypeDef

```python
# HoursOfOperationSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HoursOfOperationSearchCriteriaTypeDef


def get_value() -> HoursOfOperationSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# HoursOfOperationSearchCriteriaTypeDef definition

class HoursOfOperationSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## PredefinedAttributeSearchCriteriaPaginatorTypeDef

```python
# PredefinedAttributeSearchCriteriaPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PredefinedAttributeSearchCriteriaPaginatorTypeDef


def get_value() -> PredefinedAttributeSearchCriteriaPaginatorTypeDef:
    return {
        "OrConditions": ...,
    }


# PredefinedAttributeSearchCriteriaPaginatorTypeDef definition

class PredefinedAttributeSearchCriteriaPaginatorTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## PredefinedAttributeSearchCriteriaTypeDef

```python
# PredefinedAttributeSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PredefinedAttributeSearchCriteriaTypeDef


def get_value() -> PredefinedAttributeSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# PredefinedAttributeSearchCriteriaTypeDef definition

class PredefinedAttributeSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## PromptSearchCriteriaPaginatorTypeDef

```python
# PromptSearchCriteriaPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PromptSearchCriteriaPaginatorTypeDef


def get_value() -> PromptSearchCriteriaPaginatorTypeDef:
    return {
        "OrConditions": ...,
    }


# PromptSearchCriteriaPaginatorTypeDef definition

class PromptSearchCriteriaPaginatorTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## PromptSearchCriteriaTypeDef

```python
# PromptSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PromptSearchCriteriaTypeDef


def get_value() -> PromptSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# PromptSearchCriteriaTypeDef definition

class PromptSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## QueueSearchCriteriaPaginatorTypeDef

```python
# QueueSearchCriteriaPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QueueSearchCriteriaPaginatorTypeDef


def get_value() -> QueueSearchCriteriaPaginatorTypeDef:
    return {
        "OrConditions": ...,
    }


# QueueSearchCriteriaPaginatorTypeDef definition

class QueueSearchCriteriaPaginatorTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
    QueueTypeCondition: NotRequired[SearchableQueueTypeType],  # (2)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-brackets: SearchableQueueTypeType](./literals.md#searchablequeuetypetype) 
## QueueSearchCriteriaTypeDef

```python
# QueueSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QueueSearchCriteriaTypeDef


def get_value() -> QueueSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# QueueSearchCriteriaTypeDef definition

class QueueSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
    QueueTypeCondition: NotRequired[SearchableQueueTypeType],  # (2)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-brackets: SearchableQueueTypeType](./literals.md#searchablequeuetypetype) 
## QuickConnectSearchCriteriaPaginatorTypeDef

```python
# QuickConnectSearchCriteriaPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QuickConnectSearchCriteriaPaginatorTypeDef


def get_value() -> QuickConnectSearchCriteriaPaginatorTypeDef:
    return {
        "OrConditions": ...,
    }


# QuickConnectSearchCriteriaPaginatorTypeDef definition

class QuickConnectSearchCriteriaPaginatorTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## QuickConnectSearchCriteriaTypeDef

```python
# QuickConnectSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QuickConnectSearchCriteriaTypeDef


def get_value() -> QuickConnectSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# QuickConnectSearchCriteriaTypeDef definition

class QuickConnectSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## RoutingProfileSearchCriteriaPaginatorTypeDef

```python
# RoutingProfileSearchCriteriaPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RoutingProfileSearchCriteriaPaginatorTypeDef


def get_value() -> RoutingProfileSearchCriteriaPaginatorTypeDef:
    return {
        "OrConditions": ...,
    }


# RoutingProfileSearchCriteriaPaginatorTypeDef definition

class RoutingProfileSearchCriteriaPaginatorTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## RoutingProfileSearchCriteriaTypeDef

```python
# RoutingProfileSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RoutingProfileSearchCriteriaTypeDef


def get_value() -> RoutingProfileSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# RoutingProfileSearchCriteriaTypeDef definition

class RoutingProfileSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## SecurityProfileSearchCriteriaPaginatorTypeDef

```python
# SecurityProfileSearchCriteriaPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SecurityProfileSearchCriteriaPaginatorTypeDef


def get_value() -> SecurityProfileSearchCriteriaPaginatorTypeDef:
    return {
        "OrConditions": ...,
    }


# SecurityProfileSearchCriteriaPaginatorTypeDef definition

class SecurityProfileSearchCriteriaPaginatorTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## SecurityProfileSearchCriteriaTypeDef

```python
# SecurityProfileSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SecurityProfileSearchCriteriaTypeDef


def get_value() -> SecurityProfileSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# SecurityProfileSearchCriteriaTypeDef definition

class SecurityProfileSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## UserHierarchyGroupSearchCriteriaPaginatorTypeDef

```python
# UserHierarchyGroupSearchCriteriaPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserHierarchyGroupSearchCriteriaPaginatorTypeDef


def get_value() -> UserHierarchyGroupSearchCriteriaPaginatorTypeDef:
    return {
        "OrConditions": ...,
    }


# UserHierarchyGroupSearchCriteriaPaginatorTypeDef definition

class UserHierarchyGroupSearchCriteriaPaginatorTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## UserHierarchyGroupSearchCriteriaTypeDef

```python
# UserHierarchyGroupSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserHierarchyGroupSearchCriteriaTypeDef


def get_value() -> UserHierarchyGroupSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# UserHierarchyGroupSearchCriteriaTypeDef definition

class UserHierarchyGroupSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## ListAgentStatusResponseTypeDef

```python
# ListAgentStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListAgentStatusResponseTypeDef


def get_value() -> ListAgentStatusResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListAgentStatusResponseTypeDef definition

class ListAgentStatusResponseTypeDef(TypedDict):
    AgentStatusSummaryList: List[AgentStatusSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AgentStatusSummaryTypeDef](./type_defs.md#agentstatussummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAgentStatusResponseTypeDef

```python
# DescribeAgentStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeAgentStatusResponseTypeDef


def get_value() -> DescribeAgentStatusResponseTypeDef:
    return {
        "AgentStatus": ...,
    }


# DescribeAgentStatusResponseTypeDef definition

class DescribeAgentStatusResponseTypeDef(TypedDict):
    AgentStatus: AgentStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentStatusTypeDef](./type_defs.md#agentstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchAgentStatusesResponseTypeDef

```python
# SearchAgentStatusesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchAgentStatusesResponseTypeDef


def get_value() -> SearchAgentStatusesResponseTypeDef:
    return {
        "AgentStatuses": ...,
    }


# SearchAgentStatusesResponseTypeDef definition

class SearchAgentStatusesResponseTypeDef(TypedDict):
    AgentStatuses: List[AgentStatusTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AgentStatusTypeDef](./type_defs.md#agentstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MatchCriteriaOutputTypeDef

```python
# MatchCriteriaOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MatchCriteriaOutputTypeDef


def get_value() -> MatchCriteriaOutputTypeDef:
    return {
        "AgentsCriteria": ...,
    }


# MatchCriteriaOutputTypeDef definition

class MatchCriteriaOutputTypeDef(TypedDict):
    AgentsCriteria: NotRequired[AgentsCriteriaOutputTypeDef],  # (1)
```

1. See [:material-code-braces: AgentsCriteriaOutputTypeDef](./type_defs.md#agentscriteriaoutputtypedef) 
## ListAnalyticsDataAssociationsResponseTypeDef

```python
# ListAnalyticsDataAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListAnalyticsDataAssociationsResponseTypeDef


def get_value() -> ListAnalyticsDataAssociationsResponseTypeDef:
    return {
        "Results": ...,
    }


# ListAnalyticsDataAssociationsResponseTypeDef definition

class ListAnalyticsDataAssociationsResponseTypeDef(TypedDict):
    Results: List[AnalyticsDataAssociationResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AnalyticsDataAssociationResultTypeDef](./type_defs.md#analyticsdataassociationresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAnalyticsDataLakeDataSetsResponseTypeDef

```python
# ListAnalyticsDataLakeDataSetsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListAnalyticsDataLakeDataSetsResponseTypeDef


def get_value() -> ListAnalyticsDataLakeDataSetsResponseTypeDef:
    return {
        "Results": ...,
    }


# ListAnalyticsDataLakeDataSetsResponseTypeDef definition

class ListAnalyticsDataLakeDataSetsResponseTypeDef(TypedDict):
    Results: List[AnalyticsDataSetsResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AnalyticsDataSetsResultTypeDef](./type_defs.md#analyticsdatasetsresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecurityProfileApplicationsResponseTypeDef

```python
# ListSecurityProfileApplicationsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListSecurityProfileApplicationsResponseTypeDef


def get_value() -> ListSecurityProfileApplicationsResponseTypeDef:
    return {
        "Applications": ...,
    }


# ListSecurityProfileApplicationsResponseTypeDef definition

class ListSecurityProfileApplicationsResponseTypeDef(TypedDict):
    Applications: List[ApplicationOutputTypeDef],  # (1)
    LastModifiedTime: datetime,
    LastModifiedRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationOutputTypeDef](./type_defs.md#applicationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateLexBotRequestTypeDef

```python
# AssociateLexBotRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateLexBotRequestTypeDef


def get_value() -> AssociateLexBotRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# AssociateLexBotRequestTypeDef definition

class AssociateLexBotRequestTypeDef(TypedDict):
    InstanceId: str,
    LexBot: LexBotTypeDef,  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: LexBotTypeDef](./type_defs.md#lexbottypedef) 
## ListLexBotsResponseTypeDef

```python
# ListLexBotsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListLexBotsResponseTypeDef


def get_value() -> ListLexBotsResponseTypeDef:
    return {
        "LexBots": ...,
    }


# ListLexBotsResponseTypeDef definition

class ListLexBotsResponseTypeDef(TypedDict):
    LexBots: List[LexBotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LexBotTypeDef](./type_defs.md#lexbottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateBotRequestTypeDef

```python
# AssociateBotRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateBotRequestTypeDef


def get_value() -> AssociateBotRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# AssociateBotRequestTypeDef definition

class AssociateBotRequestTypeDef(TypedDict):
    InstanceId: str,
    LexBot: NotRequired[LexBotTypeDef],  # (1)
    LexV2Bot: NotRequired[LexV2BotTypeDef],  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: LexBotTypeDef](./type_defs.md#lexbottypedef) 
2. See [:material-code-braces: LexV2BotTypeDef](./type_defs.md#lexv2bottypedef) 
## DisassociateBotRequestTypeDef

```python
# DisassociateBotRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisassociateBotRequestTypeDef


def get_value() -> DisassociateBotRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DisassociateBotRequestTypeDef definition

class DisassociateBotRequestTypeDef(TypedDict):
    InstanceId: str,
    LexBot: NotRequired[LexBotTypeDef],  # (1)
    LexV2Bot: NotRequired[LexV2BotTypeDef],  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: LexBotTypeDef](./type_defs.md#lexbottypedef) 
2. See [:material-code-braces: LexV2BotTypeDef](./type_defs.md#lexv2bottypedef) 
## LexBotConfigTypeDef

```python
# LexBotConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import LexBotConfigTypeDef


def get_value() -> LexBotConfigTypeDef:
    return {
        "LexBot": ...,
    }


# LexBotConfigTypeDef definition

class LexBotConfigTypeDef(TypedDict):
    LexBot: NotRequired[LexBotTypeDef],  # (1)
    LexV2Bot: NotRequired[LexV2BotTypeDef],  # (2)
```

1. See [:material-code-braces: LexBotTypeDef](./type_defs.md#lexbottypedef) 
2. See [:material-code-braces: LexV2BotTypeDef](./type_defs.md#lexv2bottypedef) 
## AssociateUserProficienciesRequestTypeDef

```python
# AssociateUserProficienciesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateUserProficienciesRequestTypeDef


def get_value() -> AssociateUserProficienciesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# AssociateUserProficienciesRequestTypeDef definition

class AssociateUserProficienciesRequestTypeDef(TypedDict):
    InstanceId: str,
    UserId: str,
    UserProficiencies: Sequence[UserProficiencyTypeDef],  # (1)
```

1. See [:material-code-braces: UserProficiencyTypeDef](./type_defs.md#userproficiencytypedef) 
## ListUserProficienciesResponseTypeDef

```python
# ListUserProficienciesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListUserProficienciesResponseTypeDef


def get_value() -> ListUserProficienciesResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListUserProficienciesResponseTypeDef definition

class ListUserProficienciesResponseTypeDef(TypedDict):
    UserProficiencyList: List[UserProficiencyTypeDef],  # (1)
    LastModifiedTime: datetime,
    LastModifiedRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserProficiencyTypeDef](./type_defs.md#userproficiencytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserProficienciesRequestTypeDef

```python
# UpdateUserProficienciesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateUserProficienciesRequestTypeDef


def get_value() -> UpdateUserProficienciesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateUserProficienciesRequestTypeDef definition

class UpdateUserProficienciesRequestTypeDef(TypedDict):
    InstanceId: str,
    UserId: str,
    UserProficiencies: Sequence[UserProficiencyTypeDef],  # (1)
```

1. See [:material-code-braces: UserProficiencyTypeDef](./type_defs.md#userproficiencytypedef) 
## ListAssociatedContactsResponseTypeDef

```python
# ListAssociatedContactsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListAssociatedContactsResponseTypeDef


def get_value() -> ListAssociatedContactsResponseTypeDef:
    return {
        "ContactSummaryList": ...,
    }


# ListAssociatedContactsResponseTypeDef definition

class ListAssociatedContactsResponseTypeDef(TypedDict):
    ContactSummaryList: List[AssociatedContactSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociatedContactSummaryTypeDef](./type_defs.md#associatedcontactsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachedFileTypeDef

```python
# AttachedFileTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AttachedFileTypeDef


def get_value() -> AttachedFileTypeDef:
    return {
        "CreationTime": ...,
    }


# AttachedFileTypeDef definition

class AttachedFileTypeDef(TypedDict):
    CreationTime: str,
    FileArn: str,
    FileId: str,
    FileName: str,
    FileSizeInBytes: int,
    FileStatus: FileStatusTypeType,  # (1)
    CreatedBy: NotRequired[CreatedByInfoTypeDef],  # (2)
    FileUseCaseType: NotRequired[FileUseCaseTypeType],  # (3)
    AssociatedResourceArn: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: FileStatusTypeType](./literals.md#filestatustypetype) 
2. See [:material-code-braces: CreatedByInfoTypeDef](./type_defs.md#createdbyinfotypedef) 
3. See [:material-code-brackets: FileUseCaseTypeType](./literals.md#fileusecasetypetype) 
## StartAttachedFileUploadRequestTypeDef

```python
# StartAttachedFileUploadRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartAttachedFileUploadRequestTypeDef


def get_value() -> StartAttachedFileUploadRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# StartAttachedFileUploadRequestTypeDef definition

class StartAttachedFileUploadRequestTypeDef(TypedDict):
    InstanceId: str,
    FileName: str,
    FileSizeInBytes: int,
    FileUseCaseType: FileUseCaseTypeType,  # (1)
    AssociatedResourceArn: str,
    ClientToken: NotRequired[str],
    UrlExpiryInSeconds: NotRequired[int],
    CreatedBy: NotRequired[CreatedByInfoTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: FileUseCaseTypeType](./literals.md#fileusecasetypetype) 
2. See [:material-code-braces: CreatedByInfoTypeDef](./type_defs.md#createdbyinfotypedef) 
## AttributeAndConditionTypeDef

```python
# AttributeAndConditionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AttributeAndConditionTypeDef


def get_value() -> AttributeAndConditionTypeDef:
    return {
        "TagConditions": ...,
    }


# AttributeAndConditionTypeDef definition

class AttributeAndConditionTypeDef(TypedDict):
    TagConditions: NotRequired[Sequence[TagConditionTypeDef]],  # (1)
    HierarchyGroupCondition: NotRequired[HierarchyGroupConditionTypeDef],  # (2)
```

1. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
2. See [:material-code-braces: HierarchyGroupConditionTypeDef](./type_defs.md#hierarchygroupconditiontypedef) 
## CommonAttributeAndConditionTypeDef

```python
# CommonAttributeAndConditionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CommonAttributeAndConditionTypeDef


def get_value() -> CommonAttributeAndConditionTypeDef:
    return {
        "TagConditions": ...,
    }


# CommonAttributeAndConditionTypeDef definition

class CommonAttributeAndConditionTypeDef(TypedDict):
    TagConditions: NotRequired[Sequence[TagConditionTypeDef]],  # (1)
```

1. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
## ControlPlaneTagFilterTypeDef

```python
# ControlPlaneTagFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ControlPlaneTagFilterTypeDef


def get_value() -> ControlPlaneTagFilterTypeDef:
    return {
        "OrConditions": ...,
    }


# ControlPlaneTagFilterTypeDef definition

class ControlPlaneTagFilterTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Sequence[TagConditionTypeDef]]],  # (1)
    AndConditions: NotRequired[Sequence[TagConditionTypeDef]],  # (2)
    TagCondition: NotRequired[TagConditionTypeDef],  # (3)
```

1. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
2. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
3. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
## DescribeInstanceAttributeResponseTypeDef

```python
# DescribeInstanceAttributeResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeInstanceAttributeResponseTypeDef


def get_value() -> DescribeInstanceAttributeResponseTypeDef:
    return {
        "Attribute": ...,
    }


# DescribeInstanceAttributeResponseTypeDef definition

class DescribeInstanceAttributeResponseTypeDef(TypedDict):
    Attribute: AttributeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstanceAttributesResponseTypeDef

```python
# ListInstanceAttributesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListInstanceAttributesResponseTypeDef


def get_value() -> ListInstanceAttributesResponseTypeDef:
    return {
        "Attributes": ...,
    }


# ListInstanceAttributesResponseTypeDef definition

class ListInstanceAttributesResponseTypeDef(TypedDict):
    Attributes: List[AttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MeetingFeaturesConfigurationTypeDef

```python
# MeetingFeaturesConfigurationTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MeetingFeaturesConfigurationTypeDef


def get_value() -> MeetingFeaturesConfigurationTypeDef:
    return {
        "Audio": ...,
    }


# MeetingFeaturesConfigurationTypeDef definition

class MeetingFeaturesConfigurationTypeDef(TypedDict):
    Audio: NotRequired[AudioFeaturesTypeDef],  # (1)
```

1. See [:material-code-braces: AudioFeaturesTypeDef](./type_defs.md#audiofeaturestypedef) 
## ListAuthenticationProfilesResponseTypeDef

```python
# ListAuthenticationProfilesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListAuthenticationProfilesResponseTypeDef


def get_value() -> ListAuthenticationProfilesResponseTypeDef:
    return {
        "AuthenticationProfileSummaryList": ...,
    }


# ListAuthenticationProfilesResponseTypeDef definition

class ListAuthenticationProfilesResponseTypeDef(TypedDict):
    AuthenticationProfileSummaryList: List[AuthenticationProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AuthenticationProfileSummaryTypeDef](./type_defs.md#authenticationprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAuthenticationProfileResponseTypeDef

```python
# DescribeAuthenticationProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeAuthenticationProfileResponseTypeDef


def get_value() -> DescribeAuthenticationProfileResponseTypeDef:
    return {
        "AuthenticationProfile": ...,
    }


# DescribeAuthenticationProfileResponseTypeDef definition

class DescribeAuthenticationProfileResponseTypeDef(TypedDict):
    AuthenticationProfile: AuthenticationProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthenticationProfileTypeDef](./type_defs.md#authenticationprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchAvailablePhoneNumbersResponseTypeDef

```python
# SearchAvailablePhoneNumbersResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchAvailablePhoneNumbersResponseTypeDef


def get_value() -> SearchAvailablePhoneNumbersResponseTypeDef:
    return {
        "NextToken": ...,
    }


# SearchAvailablePhoneNumbersResponseTypeDef definition

class SearchAvailablePhoneNumbersResponseTypeDef(TypedDict):
    AvailableNumbersList: List[AvailableNumberSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AvailableNumberSummaryTypeDef](./type_defs.md#availablenumbersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchAssociateAnalyticsDataSetResponseTypeDef

```python
# BatchAssociateAnalyticsDataSetResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import BatchAssociateAnalyticsDataSetResponseTypeDef


def get_value() -> BatchAssociateAnalyticsDataSetResponseTypeDef:
    return {
        "Created": ...,
    }


# BatchAssociateAnalyticsDataSetResponseTypeDef definition

class BatchAssociateAnalyticsDataSetResponseTypeDef(TypedDict):
    Created: List[AnalyticsDataAssociationResultTypeDef],  # (1)
    Errors: List[ErrorResultTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AnalyticsDataAssociationResultTypeDef](./type_defs.md#analyticsdataassociationresulttypedef) 
2. See [:material-code-braces: ErrorResultTypeDef](./type_defs.md#errorresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisassociateAnalyticsDataSetResponseTypeDef

```python
# BatchDisassociateAnalyticsDataSetResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import BatchDisassociateAnalyticsDataSetResponseTypeDef


def get_value() -> BatchDisassociateAnalyticsDataSetResponseTypeDef:
    return {
        "Deleted": ...,
    }


# BatchDisassociateAnalyticsDataSetResponseTypeDef definition

class BatchDisassociateAnalyticsDataSetResponseTypeDef(TypedDict):
    Deleted: List[str],
    Errors: List[ErrorResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ErrorResultTypeDef](./type_defs.md#errorresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetFlowAssociationResponseTypeDef

```python
# BatchGetFlowAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import BatchGetFlowAssociationResponseTypeDef


def get_value() -> BatchGetFlowAssociationResponseTypeDef:
    return {
        "FlowAssociationSummaryList": ...,
    }


# BatchGetFlowAssociationResponseTypeDef definition

class BatchGetFlowAssociationResponseTypeDef(TypedDict):
    FlowAssociationSummaryList: List[FlowAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowAssociationSummaryTypeDef](./type_defs.md#flowassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFlowAssociationsResponseTypeDef

```python
# ListFlowAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListFlowAssociationsResponseTypeDef


def get_value() -> ListFlowAssociationsResponseTypeDef:
    return {
        "FlowAssociationSummaryList": ...,
    }


# ListFlowAssociationsResponseTypeDef definition

class ListFlowAssociationsResponseTypeDef(TypedDict):
    FlowAssociationSummaryList: List[FlowAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FlowAssociationSummaryTypeDef](./type_defs.md#flowassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutContactResponseTypeDef

```python
# BatchPutContactResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import BatchPutContactResponseTypeDef


def get_value() -> BatchPutContactResponseTypeDef:
    return {
        "SuccessfulRequestList": ...,
    }


# BatchPutContactResponseTypeDef definition

class BatchPutContactResponseTypeDef(TypedDict):
    SuccessfulRequestList: List[SuccessfulRequestTypeDef],  # (1)
    FailedRequestList: List[FailedRequestTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SuccessfulRequestTypeDef](./type_defs.md#successfulrequesttypedef) 
2. See [:material-code-braces: FailedRequestTypeDef](./type_defs.md#failedrequesttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartContactStreamingRequestTypeDef

```python
# StartContactStreamingRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartContactStreamingRequestTypeDef


def get_value() -> StartContactStreamingRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# StartContactStreamingRequestTypeDef definition

class StartContactStreamingRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ChatStreamingConfiguration: ChatStreamingConfigurationTypeDef,  # (1)
    ClientToken: str,
```

1. See [:material-code-braces: ChatStreamingConfigurationTypeDef](./type_defs.md#chatstreamingconfigurationtypedef) 
## ClaimedPhoneNumberSummaryTypeDef

```python
# ClaimedPhoneNumberSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ClaimedPhoneNumberSummaryTypeDef


def get_value() -> ClaimedPhoneNumberSummaryTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# ClaimedPhoneNumberSummaryTypeDef definition

class ClaimedPhoneNumberSummaryTypeDef(TypedDict):
    PhoneNumberId: NotRequired[str],
    PhoneNumberArn: NotRequired[str],
    PhoneNumber: NotRequired[str],
    PhoneNumberCountryCode: NotRequired[PhoneNumberCountryCodeType],  # (1)
    PhoneNumberType: NotRequired[PhoneNumberTypeType],  # (2)
    PhoneNumberDescription: NotRequired[str],
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    PhoneNumberStatus: NotRequired[PhoneNumberStatusTypeDef],  # (3)
    SourcePhoneNumberArn: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
3. See [:material-code-braces: PhoneNumberStatusTypeDef](./type_defs.md#phonenumberstatustypedef) 
## ConditionTypeDef

```python
# ConditionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ConditionTypeDef


def get_value() -> ConditionTypeDef:
    return {
        "StringCondition": ...,
    }


# ConditionTypeDef definition

class ConditionTypeDef(TypedDict):
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
    NumberCondition: NotRequired[NumberConditionTypeDef],  # (2)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-braces: NumberConditionTypeDef](./type_defs.md#numberconditiontypedef) 
## CreatePushNotificationRegistrationRequestTypeDef

```python
# CreatePushNotificationRegistrationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreatePushNotificationRegistrationRequestTypeDef


def get_value() -> CreatePushNotificationRegistrationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreatePushNotificationRegistrationRequestTypeDef definition

class CreatePushNotificationRegistrationRequestTypeDef(TypedDict):
    InstanceId: str,
    PinpointAppArn: str,
    DeviceToken: str,
    DeviceType: DeviceTypeType,  # (1)
    ContactConfiguration: ContactConfigurationTypeDef,  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: DeviceTypeType](./literals.md#devicetypetype) 
2. See [:material-code-braces: ContactConfigurationTypeDef](./type_defs.md#contactconfigurationtypedef) 
## ContactDataRequestTypeDef

```python
# ContactDataRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactDataRequestTypeDef


def get_value() -> ContactDataRequestTypeDef:
    return {
        "SystemEndpoint": ...,
    }


# ContactDataRequestTypeDef definition

class ContactDataRequestTypeDef(TypedDict):
    SystemEndpoint: NotRequired[EndpointTypeDef],  # (1)
    CustomerEndpoint: NotRequired[EndpointTypeDef],  # (1)
    RequestIdentifier: NotRequired[str],
    QueueId: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
    Campaign: NotRequired[CampaignTypeDef],  # (3)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
3. See [:material-code-braces: CampaignTypeDef](./type_defs.md#campaigntypedef) 
## UserDataFiltersTypeDef

```python
# UserDataFiltersTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserDataFiltersTypeDef


def get_value() -> UserDataFiltersTypeDef:
    return {
        "Queues": ...,
    }


# UserDataFiltersTypeDef definition

class UserDataFiltersTypeDef(TypedDict):
    Queues: NotRequired[Sequence[str]],
    ContactFilter: NotRequired[ContactFilterTypeDef],  # (1)
    RoutingProfiles: NotRequired[Sequence[str]],
    Agents: NotRequired[Sequence[str]],
    UserHierarchyGroups: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ContactFilterTypeDef](./type_defs.md#contactfiltertypedef) 
## ListContactFlowModulesResponseTypeDef

```python
# ListContactFlowModulesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactFlowModulesResponseTypeDef


def get_value() -> ListContactFlowModulesResponseTypeDef:
    return {
        "ContactFlowModulesSummaryList": ...,
    }


# ListContactFlowModulesResponseTypeDef definition

class ListContactFlowModulesResponseTypeDef(TypedDict):
    ContactFlowModulesSummaryList: List[ContactFlowModuleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContactFlowModuleSummaryTypeDef](./type_defs.md#contactflowmodulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContactFlowModuleResponseTypeDef

```python
# DescribeContactFlowModuleResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeContactFlowModuleResponseTypeDef


def get_value() -> DescribeContactFlowModuleResponseTypeDef:
    return {
        "ContactFlowModule": ...,
    }


# DescribeContactFlowModuleResponseTypeDef definition

class DescribeContactFlowModuleResponseTypeDef(TypedDict):
    ContactFlowModule: ContactFlowModuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContactFlowModuleTypeDef](./type_defs.md#contactflowmoduletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchContactFlowModulesResponseTypeDef

```python
# SearchContactFlowModulesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchContactFlowModulesResponseTypeDef


def get_value() -> SearchContactFlowModulesResponseTypeDef:
    return {
        "ContactFlowModules": ...,
    }


# SearchContactFlowModulesResponseTypeDef definition

class SearchContactFlowModulesResponseTypeDef(TypedDict):
    ContactFlowModules: List[ContactFlowModuleTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContactFlowModuleTypeDef](./type_defs.md#contactflowmoduletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContactFlowsResponseTypeDef

```python
# ListContactFlowsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactFlowsResponseTypeDef


def get_value() -> ListContactFlowsResponseTypeDef:
    return {
        "ContactFlowSummaryList": ...,
    }


# ListContactFlowsResponseTypeDef definition

class ListContactFlowsResponseTypeDef(TypedDict):
    ContactFlowSummaryList: List[ContactFlowSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContactFlowSummaryTypeDef](./type_defs.md#contactflowsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContactFlowResponseTypeDef

```python
# DescribeContactFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeContactFlowResponseTypeDef


def get_value() -> DescribeContactFlowResponseTypeDef:
    return {
        "ContactFlow": ...,
    }


# DescribeContactFlowResponseTypeDef definition

class DescribeContactFlowResponseTypeDef(TypedDict):
    ContactFlow: ContactFlowTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContactFlowTypeDef](./type_defs.md#contactflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchContactFlowsResponseTypeDef

```python
# SearchContactFlowsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchContactFlowsResponseTypeDef


def get_value() -> SearchContactFlowsResponseTypeDef:
    return {
        "ContactFlows": ...,
    }


# SearchContactFlowsResponseTypeDef definition

class SearchContactFlowsResponseTypeDef(TypedDict):
    ContactFlows: List[ContactFlowTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContactFlowTypeDef](./type_defs.md#contactflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContactFlowVersionsResponseTypeDef

```python
# ListContactFlowVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactFlowVersionsResponseTypeDef


def get_value() -> ListContactFlowVersionsResponseTypeDef:
    return {
        "ContactFlowVersionSummaryList": ...,
    }


# ListContactFlowVersionsResponseTypeDef definition

class ListContactFlowVersionsResponseTypeDef(TypedDict):
    ContactFlowVersionSummaryList: List[ContactFlowVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContactFlowVersionSummaryTypeDef](./type_defs.md#contactflowversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContactSearchSummaryTypeDef

```python
# ContactSearchSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactSearchSummaryTypeDef


def get_value() -> ContactSearchSummaryTypeDef:
    return {
        "Arn": ...,
    }


# ContactSearchSummaryTypeDef definition

class ContactSearchSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    InitialContactId: NotRequired[str],
    PreviousContactId: NotRequired[str],
    InitiationMethod: NotRequired[ContactInitiationMethodType],  # (1)
    Channel: NotRequired[ChannelType],  # (2)
    QueueInfo: NotRequired[ContactSearchSummaryQueueInfoTypeDef],  # (3)
    AgentInfo: NotRequired[ContactSearchSummaryAgentInfoTypeDef],  # (4)
    InitiationTimestamp: NotRequired[datetime],
    DisconnectTimestamp: NotRequired[datetime],
    ScheduledTimestamp: NotRequired[datetime],
    SegmentAttributes: NotRequired[Dict[str, ContactSearchSummarySegmentAttributeValueTypeDef]],  # (5)
```

1. See [:material-code-brackets: ContactInitiationMethodType](./literals.md#contactinitiationmethodtype) 
2. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
3. See [:material-code-braces: ContactSearchSummaryQueueInfoTypeDef](./type_defs.md#contactsearchsummaryqueueinfotypedef) 
4. See [:material-code-braces: ContactSearchSummaryAgentInfoTypeDef](./type_defs.md#contactsearchsummaryagentinfotypedef) 
5. See [:material-code-braces: ContactSearchSummarySegmentAttributeValueTypeDef](./type_defs.md#contactsearchsummarysegmentattributevaluetypedef) 
## CreateContactFlowVersionRequestTypeDef

```python
# CreateContactFlowVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateContactFlowVersionRequestTypeDef


def get_value() -> CreateContactFlowVersionRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateContactFlowVersionRequestTypeDef definition

class CreateContactFlowVersionRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
    Description: NotRequired[str],
    FlowContentSha256: NotRequired[str],
    ContactFlowVersion: NotRequired[int],
    LastModifiedTime: NotRequired[TimestampTypeDef],
    LastModifiedRegion: NotRequired[str],
```

## SearchContactsTimeRangeTypeDef

```python
# SearchContactsTimeRangeTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchContactsTimeRangeTypeDef


def get_value() -> SearchContactsTimeRangeTypeDef:
    return {
        "Type": ...,
    }


# SearchContactsTimeRangeTypeDef definition

class SearchContactsTimeRangeTypeDef(TypedDict):
    Type: SearchContactsTimeRangeTypeType,  # (1)
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
```

1. See [:material-code-brackets: SearchContactsTimeRangeTypeType](./literals.md#searchcontactstimerangetypetype) 
## UpdateContactScheduleRequestTypeDef

```python
# UpdateContactScheduleRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateContactScheduleRequestTypeDef


def get_value() -> UpdateContactScheduleRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateContactScheduleRequestTypeDef definition

class UpdateContactScheduleRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ScheduledTime: TimestampTypeDef,
```

## StartOutboundVoiceContactRequestTypeDef

```python
# StartOutboundVoiceContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartOutboundVoiceContactRequestTypeDef


def get_value() -> StartOutboundVoiceContactRequestTypeDef:
    return {
        "DestinationPhoneNumber": ...,
    }


# StartOutboundVoiceContactRequestTypeDef definition

class StartOutboundVoiceContactRequestTypeDef(TypedDict):
    DestinationPhoneNumber: str,
    ContactFlowId: str,
    InstanceId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    References: NotRequired[Mapping[str, ReferenceTypeDef]],  # (1)
    RelatedContactId: NotRequired[str],
    ClientToken: NotRequired[str],
    SourcePhoneNumber: NotRequired[str],
    QueueId: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
    AnswerMachineDetectionConfig: NotRequired[AnswerMachineDetectionConfigTypeDef],  # (2)
    CampaignId: NotRequired[str],
    TrafficType: NotRequired[TrafficTypeType],  # (3)
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
2. See [:material-code-braces: AnswerMachineDetectionConfigTypeDef](./type_defs.md#answermachinedetectionconfigtypedef) 
3. See [:material-code-brackets: TrafficTypeType](./literals.md#traffictypetype) 
## TaskActionDefinitionOutputTypeDef

```python
# TaskActionDefinitionOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TaskActionDefinitionOutputTypeDef


def get_value() -> TaskActionDefinitionOutputTypeDef:
    return {
        "Name": ...,
    }


# TaskActionDefinitionOutputTypeDef definition

class TaskActionDefinitionOutputTypeDef(TypedDict):
    Name: str,
    ContactFlowId: str,
    Description: NotRequired[str],
    References: NotRequired[Dict[str, ReferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
## TaskActionDefinitionTypeDef

```python
# TaskActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TaskActionDefinitionTypeDef


def get_value() -> TaskActionDefinitionTypeDef:
    return {
        "Name": ...,
    }


# TaskActionDefinitionTypeDef definition

class TaskActionDefinitionTypeDef(TypedDict):
    Name: str,
    ContactFlowId: str,
    Description: NotRequired[str],
    References: NotRequired[Mapping[str, ReferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
## CreateParticipantRequestTypeDef

```python
# CreateParticipantRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateParticipantRequestTypeDef


def get_value() -> CreateParticipantRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateParticipantRequestTypeDef definition

class CreateParticipantRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ParticipantDetails: ParticipantDetailsToAddTypeDef,  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: ParticipantDetailsToAddTypeDef](./type_defs.md#participantdetailstoaddtypedef) 
## CreateParticipantResponseTypeDef

```python
# CreateParticipantResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateParticipantResponseTypeDef


def get_value() -> CreateParticipantResponseTypeDef:
    return {
        "ParticipantCredentials": ...,
    }


# CreateParticipantResponseTypeDef definition

class CreateParticipantResponseTypeDef(TypedDict):
    ParticipantCredentials: ParticipantTokenCredentialsTypeDef,  # (1)
    ParticipantId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParticipantTokenCredentialsTypeDef](./type_defs.md#participanttokencredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateQueueOutboundCallerConfigRequestTypeDef

```python
# UpdateQueueOutboundCallerConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateQueueOutboundCallerConfigRequestTypeDef


def get_value() -> UpdateQueueOutboundCallerConfigRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateQueueOutboundCallerConfigRequestTypeDef definition

class UpdateQueueOutboundCallerConfigRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    OutboundCallerConfig: OutboundCallerConfigTypeDef,  # (1)
```

1. See [:material-code-braces: OutboundCallerConfigTypeDef](./type_defs.md#outboundcallerconfigtypedef) 
## CreateQueueRequestTypeDef

```python
# CreateQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateQueueRequestTypeDef


def get_value() -> CreateQueueRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateQueueRequestTypeDef definition

class CreateQueueRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    HoursOfOperationId: str,
    Description: NotRequired[str],
    OutboundCallerConfig: NotRequired[OutboundCallerConfigTypeDef],  # (1)
    OutboundEmailConfig: NotRequired[OutboundEmailConfigTypeDef],  # (2)
    MaxContacts: NotRequired[int],
    QuickConnectIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: OutboundCallerConfigTypeDef](./type_defs.md#outboundcallerconfigtypedef) 
2. See [:material-code-braces: OutboundEmailConfigTypeDef](./type_defs.md#outboundemailconfigtypedef) 
## QueueTypeDef

```python
# QueueTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QueueTypeDef


def get_value() -> QueueTypeDef:
    return {
        "Name": ...,
    }


# QueueTypeDef definition

class QueueTypeDef(TypedDict):
    Name: NotRequired[str],
    QueueArn: NotRequired[str],
    QueueId: NotRequired[str],
    Description: NotRequired[str],
    OutboundCallerConfig: NotRequired[OutboundCallerConfigTypeDef],  # (1)
    OutboundEmailConfig: NotRequired[OutboundEmailConfigTypeDef],  # (2)
    HoursOfOperationId: NotRequired[str],
    MaxContacts: NotRequired[int],
    Status: NotRequired[QueueStatusType],  # (3)
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-braces: OutboundCallerConfigTypeDef](./type_defs.md#outboundcallerconfigtypedef) 
2. See [:material-code-braces: OutboundEmailConfigTypeDef](./type_defs.md#outboundemailconfigtypedef) 
3. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
## UpdateQueueOutboundEmailConfigRequestTypeDef

```python
# UpdateQueueOutboundEmailConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateQueueOutboundEmailConfigRequestTypeDef


def get_value() -> UpdateQueueOutboundEmailConfigRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateQueueOutboundEmailConfigRequestTypeDef definition

class UpdateQueueOutboundEmailConfigRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    OutboundEmailConfig: OutboundEmailConfigTypeDef,  # (1)
```

1. See [:material-code-braces: OutboundEmailConfigTypeDef](./type_defs.md#outboundemailconfigtypedef) 
## UpdateUserIdentityInfoRequestTypeDef

```python
# UpdateUserIdentityInfoRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateUserIdentityInfoRequestTypeDef


def get_value() -> UpdateUserIdentityInfoRequestTypeDef:
    return {
        "IdentityInfo": ...,
    }


# UpdateUserIdentityInfoRequestTypeDef definition

class UpdateUserIdentityInfoRequestTypeDef(TypedDict):
    IdentityInfo: UserIdentityInfoTypeDef,  # (1)
    UserId: str,
    InstanceId: str,
```

1. See [:material-code-braces: UserIdentityInfoTypeDef](./type_defs.md#useridentityinfotypedef) 
## CreateUserRequestTypeDef

```python
# CreateUserRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateUserRequestTypeDef


def get_value() -> CreateUserRequestTypeDef:
    return {
        "Username": ...,
    }


# CreateUserRequestTypeDef definition

class CreateUserRequestTypeDef(TypedDict):
    Username: str,
    PhoneConfig: UserPhoneConfigTypeDef,  # (1)
    SecurityProfileIds: Sequence[str],
    RoutingProfileId: str,
    InstanceId: str,
    Password: NotRequired[str],
    IdentityInfo: NotRequired[UserIdentityInfoTypeDef],  # (2)
    DirectoryUserId: NotRequired[str],
    HierarchyGroupId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: UserPhoneConfigTypeDef](./type_defs.md#userphoneconfigtypedef) 
2. See [:material-code-braces: UserIdentityInfoTypeDef](./type_defs.md#useridentityinfotypedef) 
## UpdateUserPhoneConfigRequestTypeDef

```python
# UpdateUserPhoneConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateUserPhoneConfigRequestTypeDef


def get_value() -> UpdateUserPhoneConfigRequestTypeDef:
    return {
        "PhoneConfig": ...,
    }


# UpdateUserPhoneConfigRequestTypeDef definition

class UpdateUserPhoneConfigRequestTypeDef(TypedDict):
    PhoneConfig: UserPhoneConfigTypeDef,  # (1)
    UserId: str,
    InstanceId: str,
```

1. See [:material-code-braces: UserPhoneConfigTypeDef](./type_defs.md#userphoneconfigtypedef) 
## UserTypeDef

```python
# UserTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserTypeDef


def get_value() -> UserTypeDef:
    return {
        "Id": ...,
    }


# UserTypeDef definition

class UserTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Username: NotRequired[str],
    IdentityInfo: NotRequired[UserIdentityInfoTypeDef],  # (1)
    PhoneConfig: NotRequired[UserPhoneConfigTypeDef],  # (2)
    DirectoryUserId: NotRequired[str],
    SecurityProfileIds: NotRequired[List[str]],
    RoutingProfileId: NotRequired[str],
    HierarchyGroupId: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-braces: UserIdentityInfoTypeDef](./type_defs.md#useridentityinfotypedef) 
2. See [:material-code-braces: UserPhoneConfigTypeDef](./type_defs.md#userphoneconfigtypedef) 
## CreateViewRequestTypeDef

```python
# CreateViewRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateViewRequestTypeDef


def get_value() -> CreateViewRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateViewRequestTypeDef definition

class CreateViewRequestTypeDef(TypedDict):
    InstanceId: str,
    Status: ViewStatusType,  # (1)
    Content: ViewInputContentTypeDef,  # (2)
    Name: str,
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ViewStatusType](./literals.md#viewstatustype) 
2. See [:material-code-braces: ViewInputContentTypeDef](./type_defs.md#viewinputcontenttypedef) 
## UpdateViewContentRequestTypeDef

```python
# UpdateViewContentRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateViewContentRequestTypeDef


def get_value() -> UpdateViewContentRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateViewContentRequestTypeDef definition

class UpdateViewContentRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
    Status: ViewStatusType,  # (1)
    Content: ViewInputContentTypeDef,  # (2)
```

1. See [:material-code-brackets: ViewStatusType](./literals.md#viewstatustype) 
2. See [:material-code-braces: ViewInputContentTypeDef](./type_defs.md#viewinputcontenttypedef) 
## GetFederationTokenResponseTypeDef

```python
# GetFederationTokenResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetFederationTokenResponseTypeDef


def get_value() -> GetFederationTokenResponseTypeDef:
    return {
        "Credentials": ...,
    }


# GetFederationTokenResponseTypeDef definition

class GetFederationTokenResponseTypeDef(TypedDict):
    Credentials: CredentialsTypeDef,  # (1)
    SignInUrl: str,
    UserArn: str,
    UserId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MediaConcurrencyTypeDef

```python
# MediaConcurrencyTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MediaConcurrencyTypeDef


def get_value() -> MediaConcurrencyTypeDef:
    return {
        "Channel": ...,
    }


# MediaConcurrencyTypeDef definition

class MediaConcurrencyTypeDef(TypedDict):
    Channel: ChannelType,  # (1)
    Concurrency: int,
    CrossChannelBehavior: NotRequired[CrossChannelBehaviorTypeDef],  # (2)
```

1. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
2. See [:material-code-braces: CrossChannelBehaviorTypeDef](./type_defs.md#crosschannelbehaviortypedef) 
## CurrentMetricDataTypeDef

```python
# CurrentMetricDataTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CurrentMetricDataTypeDef


def get_value() -> CurrentMetricDataTypeDef:
    return {
        "Metric": ...,
    }


# CurrentMetricDataTypeDef definition

class CurrentMetricDataTypeDef(TypedDict):
    Metric: NotRequired[CurrentMetricTypeDef],  # (1)
    Value: NotRequired[float],
```

1. See [:material-code-braces: CurrentMetricTypeDef](./type_defs.md#currentmetrictypedef) 
## HoursOfOperationOverrideSearchCriteriaPaginatorTypeDef

```python
# HoursOfOperationOverrideSearchCriteriaPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HoursOfOperationOverrideSearchCriteriaPaginatorTypeDef


def get_value() -> HoursOfOperationOverrideSearchCriteriaPaginatorTypeDef:
    return {
        "OrConditions": ...,
    }


# HoursOfOperationOverrideSearchCriteriaPaginatorTypeDef definition

class HoursOfOperationOverrideSearchCriteriaPaginatorTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
    DateCondition: NotRequired[DateConditionTypeDef],  # (2)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-braces: DateConditionTypeDef](./type_defs.md#dateconditiontypedef) 
## HoursOfOperationOverrideSearchCriteriaTypeDef

```python
# HoursOfOperationOverrideSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HoursOfOperationOverrideSearchCriteriaTypeDef


def get_value() -> HoursOfOperationOverrideSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# HoursOfOperationOverrideSearchCriteriaTypeDef definition

class HoursOfOperationOverrideSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
    DateCondition: NotRequired[DateConditionTypeDef],  # (2)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-braces: DateConditionTypeDef](./type_defs.md#dateconditiontypedef) 
## ListDefaultVocabulariesResponseTypeDef

```python
# ListDefaultVocabulariesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListDefaultVocabulariesResponseTypeDef


def get_value() -> ListDefaultVocabulariesResponseTypeDef:
    return {
        "DefaultVocabularyList": ...,
    }


# ListDefaultVocabulariesResponseTypeDef definition

class ListDefaultVocabulariesResponseTypeDef(TypedDict):
    DefaultVocabularyList: List[DefaultVocabularyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DefaultVocabularyTypeDef](./type_defs.md#defaultvocabularytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePromptResponseTypeDef

```python
# DescribePromptResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribePromptResponseTypeDef


def get_value() -> DescribePromptResponseTypeDef:
    return {
        "Prompt": ...,
    }


# DescribePromptResponseTypeDef definition

class DescribePromptResponseTypeDef(TypedDict):
    Prompt: PromptTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PromptTypeDef](./type_defs.md#prompttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchPromptsResponseTypeDef

```python
# SearchPromptsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchPromptsResponseTypeDef


def get_value() -> SearchPromptsResponseTypeDef:
    return {
        "Prompts": ...,
    }


# SearchPromptsResponseTypeDef definition

class SearchPromptsResponseTypeDef(TypedDict):
    Prompts: List[PromptTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PromptTypeDef](./type_defs.md#prompttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSecurityProfileResponseTypeDef

```python
# DescribeSecurityProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeSecurityProfileResponseTypeDef


def get_value() -> DescribeSecurityProfileResponseTypeDef:
    return {
        "SecurityProfile": ...,
    }


# DescribeSecurityProfileResponseTypeDef definition

class DescribeSecurityProfileResponseTypeDef(TypedDict):
    SecurityProfile: SecurityProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityProfileTypeDef](./type_defs.md#securityprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTrafficDistributionGroupResponseTypeDef

```python
# DescribeTrafficDistributionGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeTrafficDistributionGroupResponseTypeDef


def get_value() -> DescribeTrafficDistributionGroupResponseTypeDef:
    return {
        "TrafficDistributionGroup": ...,
    }


# DescribeTrafficDistributionGroupResponseTypeDef definition

class DescribeTrafficDistributionGroupResponseTypeDef(TypedDict):
    TrafficDistributionGroup: TrafficDistributionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficDistributionGroupTypeDef](./type_defs.md#trafficdistributiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVocabularyResponseTypeDef

```python
# DescribeVocabularyResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeVocabularyResponseTypeDef


def get_value() -> DescribeVocabularyResponseTypeDef:
    return {
        "Vocabulary": ...,
    }


# DescribeVocabularyResponseTypeDef definition

class DescribeVocabularyResponseTypeDef(TypedDict):
    Vocabulary: VocabularyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VocabularyTypeDef](./type_defs.md#vocabularytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DimensionsTypeDef

```python
# DimensionsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DimensionsTypeDef


def get_value() -> DimensionsTypeDef:
    return {
        "Queue": ...,
    }


# DimensionsTypeDef definition

class DimensionsTypeDef(TypedDict):
    Queue: NotRequired[QueueReferenceTypeDef],  # (1)
    Channel: NotRequired[ChannelType],  # (2)
    RoutingProfile: NotRequired[RoutingProfileReferenceTypeDef],  # (3)
    RoutingStepExpression: NotRequired[str],
```

1. See [:material-code-braces: QueueReferenceTypeDef](./type_defs.md#queuereferencetypedef) 
2. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
3. See [:material-code-braces: RoutingProfileReferenceTypeDef](./type_defs.md#routingprofilereferencetypedef) 
## DisassociateRoutingProfileQueuesRequestTypeDef

```python
# DisassociateRoutingProfileQueuesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisassociateRoutingProfileQueuesRequestTypeDef


def get_value() -> DisassociateRoutingProfileQueuesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DisassociateRoutingProfileQueuesRequestTypeDef definition

class DisassociateRoutingProfileQueuesRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    QueueReferences: Sequence[RoutingProfileQueueReferenceTypeDef],  # (1)
```

1. See [:material-code-braces: RoutingProfileQueueReferenceTypeDef](./type_defs.md#routingprofilequeuereferencetypedef) 
## RoutingProfileQueueConfigTypeDef

```python
# RoutingProfileQueueConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RoutingProfileQueueConfigTypeDef


def get_value() -> RoutingProfileQueueConfigTypeDef:
    return {
        "QueueReference": ...,
    }


# RoutingProfileQueueConfigTypeDef definition

class RoutingProfileQueueConfigTypeDef(TypedDict):
    QueueReference: RoutingProfileQueueReferenceTypeDef,  # (1)
    Priority: int,
    Delay: int,
```

1. See [:material-code-braces: RoutingProfileQueueReferenceTypeDef](./type_defs.md#routingprofilequeuereferencetypedef) 
## DisassociateUserProficienciesRequestTypeDef

```python
# DisassociateUserProficienciesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DisassociateUserProficienciesRequestTypeDef


def get_value() -> DisassociateUserProficienciesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DisassociateUserProficienciesRequestTypeDef definition

class DisassociateUserProficienciesRequestTypeDef(TypedDict):
    InstanceId: str,
    UserId: str,
    UserProficiencies: Sequence[UserProficiencyDisassociateTypeDef],  # (1)
```

1. See [:material-code-braces: UserProficiencyDisassociateTypeDef](./type_defs.md#userproficiencydisassociatetypedef) 
## StopContactRequestTypeDef

```python
# StopContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StopContactRequestTypeDef


def get_value() -> StopContactRequestTypeDef:
    return {
        "ContactId": ...,
    }


# StopContactRequestTypeDef definition

class StopContactRequestTypeDef(TypedDict):
    ContactId: str,
    InstanceId: str,
    DisconnectReason: NotRequired[DisconnectReasonTypeDef],  # (1)
```

1. See [:material-code-braces: DisconnectReasonTypeDef](./type_defs.md#disconnectreasontypedef) 
## GetAttachedFileResponseTypeDef

```python
# GetAttachedFileResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetAttachedFileResponseTypeDef


def get_value() -> GetAttachedFileResponseTypeDef:
    return {
        "FileArn": ...,
    }


# GetAttachedFileResponseTypeDef definition

class GetAttachedFileResponseTypeDef(TypedDict):
    FileArn: str,
    FileId: str,
    CreationTime: str,
    FileStatus: FileStatusTypeType,  # (1)
    FileName: str,
    FileSizeInBytes: int,
    AssociatedResourceArn: str,
    FileUseCaseType: FileUseCaseTypeType,  # (2)
    CreatedBy: CreatedByInfoTypeDef,  # (3)
    DownloadUrlMetadata: DownloadUrlMetadataTypeDef,  # (4)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: FileStatusTypeType](./literals.md#filestatustypetype) 
2. See [:material-code-brackets: FileUseCaseTypeType](./literals.md#fileusecasetypetype) 
3. See [:material-code-braces: CreatedByInfoTypeDef](./type_defs.md#createdbyinfotypedef) 
4. See [:material-code-braces: DownloadUrlMetadataTypeDef](./type_defs.md#downloadurlmetadatatypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InboundAdditionalRecipientsTypeDef

```python
# InboundAdditionalRecipientsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import InboundAdditionalRecipientsTypeDef


def get_value() -> InboundAdditionalRecipientsTypeDef:
    return {
        "ToAddresses": ...,
    }


# InboundAdditionalRecipientsTypeDef definition

class InboundAdditionalRecipientsTypeDef(TypedDict):
    ToAddresses: NotRequired[Sequence[EmailAddressInfoTypeDef]],  # (1)
    CcAddresses: NotRequired[Sequence[EmailAddressInfoTypeDef]],  # (1)
```

1. See [:material-code-braces: EmailAddressInfoTypeDef](./type_defs.md#emailaddressinfotypedef) 
2. See [:material-code-braces: EmailAddressInfoTypeDef](./type_defs.md#emailaddressinfotypedef) 
## OutboundAdditionalRecipientsTypeDef

```python
# OutboundAdditionalRecipientsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import OutboundAdditionalRecipientsTypeDef


def get_value() -> OutboundAdditionalRecipientsTypeDef:
    return {
        "CcEmailAddresses": ...,
    }


# OutboundAdditionalRecipientsTypeDef definition

class OutboundAdditionalRecipientsTypeDef(TypedDict):
    CcEmailAddresses: NotRequired[Sequence[EmailAddressInfoTypeDef]],  # (1)
```

1. See [:material-code-braces: EmailAddressInfoTypeDef](./type_defs.md#emailaddressinfotypedef) 
## SearchEmailAddressesResponseTypeDef

```python
# SearchEmailAddressesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchEmailAddressesResponseTypeDef


def get_value() -> SearchEmailAddressesResponseTypeDef:
    return {
        "NextToken": ...,
    }


# SearchEmailAddressesResponseTypeDef definition

class SearchEmailAddressesResponseTypeDef(TypedDict):
    EmailAddresses: List[EmailAddressMetadataTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EmailAddressMetadataTypeDef](./type_defs.md#emailaddressmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KinesisVideoStreamConfigTypeDef

```python
# KinesisVideoStreamConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import KinesisVideoStreamConfigTypeDef


def get_value() -> KinesisVideoStreamConfigTypeDef:
    return {
        "Prefix": ...,
    }


# KinesisVideoStreamConfigTypeDef definition

class KinesisVideoStreamConfigTypeDef(TypedDict):
    Prefix: str,
    RetentionPeriodHours: int,
    EncryptionConfig: EncryptionConfigTypeDef,  # (1)
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
## S3ConfigTypeDef

```python
# S3ConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import S3ConfigTypeDef


def get_value() -> S3ConfigTypeDef:
    return {
        "BucketName": ...,
    }


# S3ConfigTypeDef definition

class S3ConfigTypeDef(TypedDict):
    BucketName: str,
    BucketPrefix: str,
    EncryptionConfig: NotRequired[EncryptionConfigTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
## EvaluationAnswerInputTypeDef

```python
# EvaluationAnswerInputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationAnswerInputTypeDef


def get_value() -> EvaluationAnswerInputTypeDef:
    return {
        "Value": ...,
    }


# EvaluationAnswerInputTypeDef definition

class EvaluationAnswerInputTypeDef(TypedDict):
    Value: NotRequired[EvaluationAnswerDataTypeDef],  # (1)
```

1. See [:material-code-braces: EvaluationAnswerDataTypeDef](./type_defs.md#evaluationanswerdatatypedef) 
## EvaluationAnswerOutputTypeDef

```python
# EvaluationAnswerOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationAnswerOutputTypeDef


def get_value() -> EvaluationAnswerOutputTypeDef:
    return {
        "Value": ...,
    }


# EvaluationAnswerOutputTypeDef definition

class EvaluationAnswerOutputTypeDef(TypedDict):
    Value: NotRequired[EvaluationAnswerDataTypeDef],  # (1)
    SystemSuggestedValue: NotRequired[EvaluationAnswerDataTypeDef],  # (1)
```

1. See [:material-code-braces: EvaluationAnswerDataTypeDef](./type_defs.md#evaluationanswerdatatypedef) 
2. See [:material-code-braces: EvaluationAnswerDataTypeDef](./type_defs.md#evaluationanswerdatatypedef) 
## EvaluationFormNumericQuestionAutomationTypeDef

```python
# EvaluationFormNumericQuestionAutomationTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormNumericQuestionAutomationTypeDef


def get_value() -> EvaluationFormNumericQuestionAutomationTypeDef:
    return {
        "PropertyValue": ...,
    }


# EvaluationFormNumericQuestionAutomationTypeDef definition

class EvaluationFormNumericQuestionAutomationTypeDef(TypedDict):
    PropertyValue: NotRequired[NumericQuestionPropertyValueAutomationTypeDef],  # (1)
```

1. See [:material-code-braces: NumericQuestionPropertyValueAutomationTypeDef](./type_defs.md#numericquestionpropertyvalueautomationtypedef) 
## EvaluationFormSingleSelectQuestionAutomationOptionTypeDef

```python
# EvaluationFormSingleSelectQuestionAutomationOptionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormSingleSelectQuestionAutomationOptionTypeDef


def get_value() -> EvaluationFormSingleSelectQuestionAutomationOptionTypeDef:
    return {
        "RuleCategory": ...,
    }


# EvaluationFormSingleSelectQuestionAutomationOptionTypeDef definition

class EvaluationFormSingleSelectQuestionAutomationOptionTypeDef(TypedDict):
    RuleCategory: NotRequired[SingleSelectQuestionRuleCategoryAutomationTypeDef],  # (1)
```

1. See [:material-code-braces: SingleSelectQuestionRuleCategoryAutomationTypeDef](./type_defs.md#singleselectquestionrulecategoryautomationtypedef) 
## ListEvaluationFormsResponseTypeDef

```python
# ListEvaluationFormsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListEvaluationFormsResponseTypeDef


def get_value() -> ListEvaluationFormsResponseTypeDef:
    return {
        "EvaluationFormSummaryList": ...,
    }


# ListEvaluationFormsResponseTypeDef definition

class ListEvaluationFormsResponseTypeDef(TypedDict):
    EvaluationFormSummaryList: List[EvaluationFormSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EvaluationFormSummaryTypeDef](./type_defs.md#evaluationformsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEvaluationFormVersionsResponseTypeDef

```python
# ListEvaluationFormVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListEvaluationFormVersionsResponseTypeDef


def get_value() -> ListEvaluationFormVersionsResponseTypeDef:
    return {
        "EvaluationFormVersionSummaryList": ...,
    }


# ListEvaluationFormVersionsResponseTypeDef definition

class ListEvaluationFormVersionsResponseTypeDef(TypedDict):
    EvaluationFormVersionSummaryList: List[EvaluationFormVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EvaluationFormVersionSummaryTypeDef](./type_defs.md#evaluationformversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EvaluationMetadataTypeDef

```python
# EvaluationMetadataTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationMetadataTypeDef


def get_value() -> EvaluationMetadataTypeDef:
    return {
        "ContactId": ...,
    }


# EvaluationMetadataTypeDef definition

class EvaluationMetadataTypeDef(TypedDict):
    ContactId: str,
    EvaluatorArn: str,
    ContactAgentId: NotRequired[str],
    Score: NotRequired[EvaluationScoreTypeDef],  # (1)
```

1. See [:material-code-braces: EvaluationScoreTypeDef](./type_defs.md#evaluationscoretypedef) 
## EvaluationSummaryTypeDef

```python
# EvaluationSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationSummaryTypeDef


def get_value() -> EvaluationSummaryTypeDef:
    return {
        "EvaluationId": ...,
    }


# EvaluationSummaryTypeDef definition

class EvaluationSummaryTypeDef(TypedDict):
    EvaluationId: str,
    EvaluationArn: str,
    EvaluationFormTitle: str,
    EvaluationFormId: str,
    Status: EvaluationStatusType,  # (1)
    EvaluatorArn: str,
    CreatedTime: datetime,
    LastModifiedTime: datetime,
    Score: NotRequired[EvaluationScoreTypeDef],  # (2)
```

1. See [:material-code-brackets: EvaluationStatusType](./literals.md#evaluationstatustype) 
2. See [:material-code-braces: EvaluationScoreTypeDef](./type_defs.md#evaluationscoretypedef) 
## FieldValueOutputTypeDef

```python
# FieldValueOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import FieldValueOutputTypeDef


def get_value() -> FieldValueOutputTypeDef:
    return {
        "Id": ...,
    }


# FieldValueOutputTypeDef definition

class FieldValueOutputTypeDef(TypedDict):
    Id: str,
    Value: FieldValueUnionOutputTypeDef,  # (1)
```

1. See [:material-code-braces: FieldValueUnionOutputTypeDef](./type_defs.md#fieldvalueunionoutputtypedef) 
## GetCurrentMetricDataRequestTypeDef

```python
# GetCurrentMetricDataRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetCurrentMetricDataRequestTypeDef


def get_value() -> GetCurrentMetricDataRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# GetCurrentMetricDataRequestTypeDef definition

class GetCurrentMetricDataRequestTypeDef(TypedDict):
    InstanceId: str,
    Filters: FiltersTypeDef,  # (1)
    CurrentMetrics: Sequence[CurrentMetricTypeDef],  # (2)
    Groupings: NotRequired[Sequence[GroupingType]],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SortCriteria: NotRequired[Sequence[CurrentMetricSortCriteriaTypeDef]],  # (4)
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
2. See [:material-code-braces: CurrentMetricTypeDef](./type_defs.md#currentmetrictypedef) 
3. See [:material-code-brackets: GroupingType](./literals.md#groupingtype) 
4. See [:material-code-braces: CurrentMetricSortCriteriaTypeDef](./type_defs.md#currentmetricsortcriteriatypedef) 
## ListAgentStatusRequestPaginateTypeDef

```python
# ListAgentStatusRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListAgentStatusRequestPaginateTypeDef


def get_value() -> ListAgentStatusRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListAgentStatusRequestPaginateTypeDef definition

class ListAgentStatusRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    AgentStatusTypes: NotRequired[Sequence[AgentStatusTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AgentStatusTypeType](./literals.md#agentstatustypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApprovedOriginsRequestPaginateTypeDef

```python
# ListApprovedOriginsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListApprovedOriginsRequestPaginateTypeDef


def get_value() -> ListApprovedOriginsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListApprovedOriginsRequestPaginateTypeDef definition

class ListApprovedOriginsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAuthenticationProfilesRequestPaginateTypeDef

```python
# ListAuthenticationProfilesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListAuthenticationProfilesRequestPaginateTypeDef


def get_value() -> ListAuthenticationProfilesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListAuthenticationProfilesRequestPaginateTypeDef definition

class ListAuthenticationProfilesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBotsRequestPaginateTypeDef

```python
# ListBotsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListBotsRequestPaginateTypeDef


def get_value() -> ListBotsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListBotsRequestPaginateTypeDef definition

class ListBotsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    LexVersion: LexVersionType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LexVersionType](./literals.md#lexversiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContactEvaluationsRequestPaginateTypeDef

```python
# ListContactEvaluationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactEvaluationsRequestPaginateTypeDef


def get_value() -> ListContactEvaluationsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListContactEvaluationsRequestPaginateTypeDef definition

class ListContactEvaluationsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContactFlowModulesRequestPaginateTypeDef

```python
# ListContactFlowModulesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactFlowModulesRequestPaginateTypeDef


def get_value() -> ListContactFlowModulesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListContactFlowModulesRequestPaginateTypeDef definition

class ListContactFlowModulesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowModuleState: NotRequired[ContactFlowModuleStateType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContactFlowVersionsRequestPaginateTypeDef

```python
# ListContactFlowVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactFlowVersionsRequestPaginateTypeDef


def get_value() -> ListContactFlowVersionsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListContactFlowVersionsRequestPaginateTypeDef definition

class ListContactFlowVersionsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContactFlowsRequestPaginateTypeDef

```python
# ListContactFlowsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactFlowsRequestPaginateTypeDef


def get_value() -> ListContactFlowsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListContactFlowsRequestPaginateTypeDef definition

class ListContactFlowsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowTypes: NotRequired[Sequence[ContactFlowTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContactReferencesRequestPaginateTypeDef

```python
# ListContactReferencesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactReferencesRequestPaginateTypeDef


def get_value() -> ListContactReferencesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListContactReferencesRequestPaginateTypeDef definition

class ListContactReferencesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ReferenceTypes: Sequence[ReferenceTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ReferenceTypeType](./literals.md#referencetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDefaultVocabulariesRequestPaginateTypeDef

```python
# ListDefaultVocabulariesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListDefaultVocabulariesRequestPaginateTypeDef


def get_value() -> ListDefaultVocabulariesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListDefaultVocabulariesRequestPaginateTypeDef definition

class ListDefaultVocabulariesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    LanguageCode: NotRequired[VocabularyLanguageCodeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEvaluationFormVersionsRequestPaginateTypeDef

```python
# ListEvaluationFormVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListEvaluationFormVersionsRequestPaginateTypeDef


def get_value() -> ListEvaluationFormVersionsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListEvaluationFormVersionsRequestPaginateTypeDef definition

class ListEvaluationFormVersionsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEvaluationFormsRequestPaginateTypeDef

```python
# ListEvaluationFormsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListEvaluationFormsRequestPaginateTypeDef


def get_value() -> ListEvaluationFormsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListEvaluationFormsRequestPaginateTypeDef definition

class ListEvaluationFormsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFlowAssociationsRequestPaginateTypeDef

```python
# ListFlowAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListFlowAssociationsRequestPaginateTypeDef


def get_value() -> ListFlowAssociationsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListFlowAssociationsRequestPaginateTypeDef definition

class ListFlowAssociationsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    ResourceType: NotRequired[ListFlowAssociationResourceTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ListFlowAssociationResourceTypeType](./literals.md#listflowassociationresourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHoursOfOperationOverridesRequestPaginateTypeDef

```python
# ListHoursOfOperationOverridesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListHoursOfOperationOverridesRequestPaginateTypeDef


def get_value() -> ListHoursOfOperationOverridesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListHoursOfOperationOverridesRequestPaginateTypeDef definition

class ListHoursOfOperationOverridesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    HoursOfOperationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHoursOfOperationsRequestPaginateTypeDef

```python
# ListHoursOfOperationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListHoursOfOperationsRequestPaginateTypeDef


def get_value() -> ListHoursOfOperationsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListHoursOfOperationsRequestPaginateTypeDef definition

class ListHoursOfOperationsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstanceAttributesRequestPaginateTypeDef

```python
# ListInstanceAttributesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListInstanceAttributesRequestPaginateTypeDef


def get_value() -> ListInstanceAttributesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListInstanceAttributesRequestPaginateTypeDef definition

class ListInstanceAttributesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstanceStorageConfigsRequestPaginateTypeDef

```python
# ListInstanceStorageConfigsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListInstanceStorageConfigsRequestPaginateTypeDef


def get_value() -> ListInstanceStorageConfigsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListInstanceStorageConfigsRequestPaginateTypeDef definition

class ListInstanceStorageConfigsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstancesRequestPaginateTypeDef

```python
# ListInstancesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListInstancesRequestPaginateTypeDef


def get_value() -> ListInstancesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListInstancesRequestPaginateTypeDef definition

class ListInstancesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIntegrationAssociationsRequestPaginateTypeDef

```python
# ListIntegrationAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListIntegrationAssociationsRequestPaginateTypeDef


def get_value() -> ListIntegrationAssociationsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListIntegrationAssociationsRequestPaginateTypeDef definition

class ListIntegrationAssociationsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    IntegrationType: NotRequired[IntegrationTypeType],  # (1)
    IntegrationArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLambdaFunctionsRequestPaginateTypeDef

```python
# ListLambdaFunctionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListLambdaFunctionsRequestPaginateTypeDef


def get_value() -> ListLambdaFunctionsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListLambdaFunctionsRequestPaginateTypeDef definition

class ListLambdaFunctionsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLexBotsRequestPaginateTypeDef

```python
# ListLexBotsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListLexBotsRequestPaginateTypeDef


def get_value() -> ListLexBotsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListLexBotsRequestPaginateTypeDef definition

class ListLexBotsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPhoneNumbersRequestPaginateTypeDef

```python
# ListPhoneNumbersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListPhoneNumbersRequestPaginateTypeDef


def get_value() -> ListPhoneNumbersRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListPhoneNumbersRequestPaginateTypeDef definition

class ListPhoneNumbersRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PhoneNumberTypes: NotRequired[Sequence[PhoneNumberTypeType]],  # (1)
    PhoneNumberCountryCodes: NotRequired[Sequence[PhoneNumberCountryCodeType]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
2. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPhoneNumbersV2RequestPaginateTypeDef

```python
# ListPhoneNumbersV2RequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListPhoneNumbersV2RequestPaginateTypeDef


def get_value() -> ListPhoneNumbersV2RequestPaginateTypeDef:
    return {
        "TargetArn": ...,
    }


# ListPhoneNumbersV2RequestPaginateTypeDef definition

class ListPhoneNumbersV2RequestPaginateTypeDef(TypedDict):
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    PhoneNumberCountryCodes: NotRequired[Sequence[PhoneNumberCountryCodeType]],  # (1)
    PhoneNumberTypes: NotRequired[Sequence[PhoneNumberTypeType]],  # (2)
    PhoneNumberPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPredefinedAttributesRequestPaginateTypeDef

```python
# ListPredefinedAttributesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListPredefinedAttributesRequestPaginateTypeDef


def get_value() -> ListPredefinedAttributesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListPredefinedAttributesRequestPaginateTypeDef definition

class ListPredefinedAttributesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPromptsRequestPaginateTypeDef

```python
# ListPromptsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListPromptsRequestPaginateTypeDef


def get_value() -> ListPromptsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListPromptsRequestPaginateTypeDef definition

class ListPromptsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueueQuickConnectsRequestPaginateTypeDef

```python
# ListQueueQuickConnectsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListQueueQuickConnectsRequestPaginateTypeDef


def get_value() -> ListQueueQuickConnectsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListQueueQuickConnectsRequestPaginateTypeDef definition

class ListQueueQuickConnectsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueuesRequestPaginateTypeDef

```python
# ListQueuesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListQueuesRequestPaginateTypeDef


def get_value() -> ListQueuesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListQueuesRequestPaginateTypeDef definition

class ListQueuesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    QueueTypes: NotRequired[Sequence[QueueTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: QueueTypeType](./literals.md#queuetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQuickConnectsRequestPaginateTypeDef

```python
# ListQuickConnectsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListQuickConnectsRequestPaginateTypeDef


def get_value() -> ListQuickConnectsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListQuickConnectsRequestPaginateTypeDef definition

class ListQuickConnectsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    QuickConnectTypes: NotRequired[Sequence[QuickConnectTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: QuickConnectTypeType](./literals.md#quickconnecttypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRoutingProfileQueuesRequestPaginateTypeDef

```python
# ListRoutingProfileQueuesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListRoutingProfileQueuesRequestPaginateTypeDef


def get_value() -> ListRoutingProfileQueuesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListRoutingProfileQueuesRequestPaginateTypeDef definition

class ListRoutingProfileQueuesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRoutingProfilesRequestPaginateTypeDef

```python
# ListRoutingProfilesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListRoutingProfilesRequestPaginateTypeDef


def get_value() -> ListRoutingProfilesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListRoutingProfilesRequestPaginateTypeDef definition

class ListRoutingProfilesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRulesRequestPaginateTypeDef

```python
# ListRulesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListRulesRequestPaginateTypeDef


def get_value() -> ListRulesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListRulesRequestPaginateTypeDef definition

class ListRulesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PublishStatus: NotRequired[RulePublishStatusType],  # (1)
    EventSourceName: NotRequired[EventSourceNameType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
2. See [:material-code-brackets: EventSourceNameType](./literals.md#eventsourcenametype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSecurityKeysRequestPaginateTypeDef

```python
# ListSecurityKeysRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListSecurityKeysRequestPaginateTypeDef


def get_value() -> ListSecurityKeysRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListSecurityKeysRequestPaginateTypeDef definition

class ListSecurityKeysRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSecurityProfileApplicationsRequestPaginateTypeDef

```python
# ListSecurityProfileApplicationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListSecurityProfileApplicationsRequestPaginateTypeDef


def get_value() -> ListSecurityProfileApplicationsRequestPaginateTypeDef:
    return {
        "SecurityProfileId": ...,
    }


# ListSecurityProfileApplicationsRequestPaginateTypeDef definition

class ListSecurityProfileApplicationsRequestPaginateTypeDef(TypedDict):
    SecurityProfileId: str,
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSecurityProfilePermissionsRequestPaginateTypeDef

```python
# ListSecurityProfilePermissionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListSecurityProfilePermissionsRequestPaginateTypeDef


def get_value() -> ListSecurityProfilePermissionsRequestPaginateTypeDef:
    return {
        "SecurityProfileId": ...,
    }


# ListSecurityProfilePermissionsRequestPaginateTypeDef definition

class ListSecurityProfilePermissionsRequestPaginateTypeDef(TypedDict):
    SecurityProfileId: str,
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSecurityProfilesRequestPaginateTypeDef

```python
# ListSecurityProfilesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListSecurityProfilesRequestPaginateTypeDef


def get_value() -> ListSecurityProfilesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListSecurityProfilesRequestPaginateTypeDef definition

class ListSecurityProfilesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTaskTemplatesRequestPaginateTypeDef

```python
# ListTaskTemplatesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListTaskTemplatesRequestPaginateTypeDef


def get_value() -> ListTaskTemplatesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListTaskTemplatesRequestPaginateTypeDef definition

class ListTaskTemplatesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    Status: NotRequired[TaskTemplateStatusType],  # (1)
    Name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrafficDistributionGroupUsersRequestPaginateTypeDef

```python
# ListTrafficDistributionGroupUsersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListTrafficDistributionGroupUsersRequestPaginateTypeDef


def get_value() -> ListTrafficDistributionGroupUsersRequestPaginateTypeDef:
    return {
        "TrafficDistributionGroupId": ...,
    }


# ListTrafficDistributionGroupUsersRequestPaginateTypeDef definition

class ListTrafficDistributionGroupUsersRequestPaginateTypeDef(TypedDict):
    TrafficDistributionGroupId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrafficDistributionGroupsRequestPaginateTypeDef

```python
# ListTrafficDistributionGroupsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListTrafficDistributionGroupsRequestPaginateTypeDef


def get_value() -> ListTrafficDistributionGroupsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListTrafficDistributionGroupsRequestPaginateTypeDef definition

class ListTrafficDistributionGroupsRequestPaginateTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUseCasesRequestPaginateTypeDef

```python
# ListUseCasesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListUseCasesRequestPaginateTypeDef


def get_value() -> ListUseCasesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListUseCasesRequestPaginateTypeDef definition

class ListUseCasesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    IntegrationAssociationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUserHierarchyGroupsRequestPaginateTypeDef

```python
# ListUserHierarchyGroupsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListUserHierarchyGroupsRequestPaginateTypeDef


def get_value() -> ListUserHierarchyGroupsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListUserHierarchyGroupsRequestPaginateTypeDef definition

class ListUserHierarchyGroupsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUserProficienciesRequestPaginateTypeDef

```python
# ListUserProficienciesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListUserProficienciesRequestPaginateTypeDef


def get_value() -> ListUserProficienciesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListUserProficienciesRequestPaginateTypeDef definition

class ListUserProficienciesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    UserId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsersRequestPaginateTypeDef

```python
# ListUsersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListUsersRequestPaginateTypeDef


def get_value() -> ListUsersRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListUsersRequestPaginateTypeDef definition

class ListUsersRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListViewVersionsRequestPaginateTypeDef

```python
# ListViewVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListViewVersionsRequestPaginateTypeDef


def get_value() -> ListViewVersionsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListViewVersionsRequestPaginateTypeDef definition

class ListViewVersionsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListViewsRequestPaginateTypeDef

```python
# ListViewsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListViewsRequestPaginateTypeDef


def get_value() -> ListViewsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# ListViewsRequestPaginateTypeDef definition

class ListViewsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    Type: NotRequired[ViewTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ViewTypeType](./literals.md#viewtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchAvailablePhoneNumbersRequestPaginateTypeDef

```python
# SearchAvailablePhoneNumbersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchAvailablePhoneNumbersRequestPaginateTypeDef


def get_value() -> SearchAvailablePhoneNumbersRequestPaginateTypeDef:
    return {
        "PhoneNumberCountryCode": ...,
    }


# SearchAvailablePhoneNumbersRequestPaginateTypeDef definition

class SearchAvailablePhoneNumbersRequestPaginateTypeDef(TypedDict):
    PhoneNumberCountryCode: PhoneNumberCountryCodeType,  # (1)
    PhoneNumberType: PhoneNumberTypeType,  # (2)
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    PhoneNumberPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchVocabulariesRequestPaginateTypeDef

```python
# SearchVocabulariesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchVocabulariesRequestPaginateTypeDef


def get_value() -> SearchVocabulariesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchVocabulariesRequestPaginateTypeDef definition

class SearchVocabulariesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    State: NotRequired[VocabularyStateType],  # (1)
    NameStartsWith: NotRequired[str],
    LanguageCode: NotRequired[VocabularyLanguageCodeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## HierarchyPathReferenceTypeDef

```python
# HierarchyPathReferenceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HierarchyPathReferenceTypeDef


def get_value() -> HierarchyPathReferenceTypeDef:
    return {
        "LevelOne": ...,
    }


# HierarchyPathReferenceTypeDef definition

class HierarchyPathReferenceTypeDef(TypedDict):
    LevelOne: NotRequired[HierarchyGroupSummaryReferenceTypeDef],  # (1)
    LevelTwo: NotRequired[HierarchyGroupSummaryReferenceTypeDef],  # (1)
    LevelThree: NotRequired[HierarchyGroupSummaryReferenceTypeDef],  # (1)
    LevelFour: NotRequired[HierarchyGroupSummaryReferenceTypeDef],  # (1)
    LevelFive: NotRequired[HierarchyGroupSummaryReferenceTypeDef],  # (1)
```

1. See [:material-code-braces: HierarchyGroupSummaryReferenceTypeDef](./type_defs.md#hierarchygroupsummaryreferencetypedef) 
2. See [:material-code-braces: HierarchyGroupSummaryReferenceTypeDef](./type_defs.md#hierarchygroupsummaryreferencetypedef) 
3. See [:material-code-braces: HierarchyGroupSummaryReferenceTypeDef](./type_defs.md#hierarchygroupsummaryreferencetypedef) 
4. See [:material-code-braces: HierarchyGroupSummaryReferenceTypeDef](./type_defs.md#hierarchygroupsummaryreferencetypedef) 
5. See [:material-code-braces: HierarchyGroupSummaryReferenceTypeDef](./type_defs.md#hierarchygroupsummaryreferencetypedef) 
## HierarchyPathTypeDef

```python
# HierarchyPathTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HierarchyPathTypeDef


def get_value() -> HierarchyPathTypeDef:
    return {
        "LevelOne": ...,
    }


# HierarchyPathTypeDef definition

class HierarchyPathTypeDef(TypedDict):
    LevelOne: NotRequired[HierarchyGroupSummaryTypeDef],  # (1)
    LevelTwo: NotRequired[HierarchyGroupSummaryTypeDef],  # (1)
    LevelThree: NotRequired[HierarchyGroupSummaryTypeDef],  # (1)
    LevelFour: NotRequired[HierarchyGroupSummaryTypeDef],  # (1)
    LevelFive: NotRequired[HierarchyGroupSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef) 
2. See [:material-code-braces: HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef) 
3. See [:material-code-braces: HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef) 
4. See [:material-code-braces: HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef) 
5. See [:material-code-braces: HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef) 
## ListUserHierarchyGroupsResponseTypeDef

```python
# ListUserHierarchyGroupsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListUserHierarchyGroupsResponseTypeDef


def get_value() -> ListUserHierarchyGroupsResponseTypeDef:
    return {
        "UserHierarchyGroupSummaryList": ...,
    }


# ListUserHierarchyGroupsResponseTypeDef definition

class ListUserHierarchyGroupsResponseTypeDef(TypedDict):
    UserHierarchyGroupSummaryList: List[HierarchyGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HierarchyStructureTypeDef

```python
# HierarchyStructureTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HierarchyStructureTypeDef


def get_value() -> HierarchyStructureTypeDef:
    return {
        "LevelOne": ...,
    }


# HierarchyStructureTypeDef definition

class HierarchyStructureTypeDef(TypedDict):
    LevelOne: NotRequired[HierarchyLevelTypeDef],  # (1)
    LevelTwo: NotRequired[HierarchyLevelTypeDef],  # (1)
    LevelThree: NotRequired[HierarchyLevelTypeDef],  # (1)
    LevelFour: NotRequired[HierarchyLevelTypeDef],  # (1)
    LevelFive: NotRequired[HierarchyLevelTypeDef],  # (1)
```

1. See [:material-code-braces: HierarchyLevelTypeDef](./type_defs.md#hierarchyleveltypedef) 
2. See [:material-code-braces: HierarchyLevelTypeDef](./type_defs.md#hierarchyleveltypedef) 
3. See [:material-code-braces: HierarchyLevelTypeDef](./type_defs.md#hierarchyleveltypedef) 
4. See [:material-code-braces: HierarchyLevelTypeDef](./type_defs.md#hierarchyleveltypedef) 
5. See [:material-code-braces: HierarchyLevelTypeDef](./type_defs.md#hierarchyleveltypedef) 
## HierarchyStructureUpdateTypeDef

```python
# HierarchyStructureUpdateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HierarchyStructureUpdateTypeDef


def get_value() -> HierarchyStructureUpdateTypeDef:
    return {
        "LevelOne": ...,
    }


# HierarchyStructureUpdateTypeDef definition

class HierarchyStructureUpdateTypeDef(TypedDict):
    LevelOne: NotRequired[HierarchyLevelUpdateTypeDef],  # (1)
    LevelTwo: NotRequired[HierarchyLevelUpdateTypeDef],  # (1)
    LevelThree: NotRequired[HierarchyLevelUpdateTypeDef],  # (1)
    LevelFour: NotRequired[HierarchyLevelUpdateTypeDef],  # (1)
    LevelFive: NotRequired[HierarchyLevelUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: HierarchyLevelUpdateTypeDef](./type_defs.md#hierarchylevelupdatetypedef) 
2. See [:material-code-braces: HierarchyLevelUpdateTypeDef](./type_defs.md#hierarchylevelupdatetypedef) 
3. See [:material-code-braces: HierarchyLevelUpdateTypeDef](./type_defs.md#hierarchylevelupdatetypedef) 
4. See [:material-code-braces: HierarchyLevelUpdateTypeDef](./type_defs.md#hierarchylevelupdatetypedef) 
5. See [:material-code-braces: HierarchyLevelUpdateTypeDef](./type_defs.md#hierarchylevelupdatetypedef) 
## HistoricalMetricTypeDef

```python
# HistoricalMetricTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HistoricalMetricTypeDef


def get_value() -> HistoricalMetricTypeDef:
    return {
        "Name": ...,
    }


# HistoricalMetricTypeDef definition

class HistoricalMetricTypeDef(TypedDict):
    Name: NotRequired[HistoricalMetricNameType],  # (1)
    Threshold: NotRequired[ThresholdTypeDef],  # (2)
    Statistic: NotRequired[StatisticType],  # (3)
    Unit: NotRequired[UnitType],  # (4)
```

1. See [:material-code-brackets: HistoricalMetricNameType](./literals.md#historicalmetricnametype) 
2. See [:material-code-braces: ThresholdTypeDef](./type_defs.md#thresholdtypedef) 
3. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
4. See [:material-code-brackets: UnitType](./literals.md#unittype) 
## HoursOfOperationConfigTypeDef

```python
# HoursOfOperationConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HoursOfOperationConfigTypeDef


def get_value() -> HoursOfOperationConfigTypeDef:
    return {
        "Day": ...,
    }


# HoursOfOperationConfigTypeDef definition

class HoursOfOperationConfigTypeDef(TypedDict):
    Day: HoursOfOperationDaysType,  # (1)
    StartTime: HoursOfOperationTimeSliceTypeDef,  # (2)
    EndTime: HoursOfOperationTimeSliceTypeDef,  # (2)
```

1. See [:material-code-brackets: HoursOfOperationDaysType](./literals.md#hoursofoperationdaystype) 
2. See [:material-code-braces: HoursOfOperationTimeSliceTypeDef](./type_defs.md#hoursofoperationtimeslicetypedef) 
3. See [:material-code-braces: HoursOfOperationTimeSliceTypeDef](./type_defs.md#hoursofoperationtimeslicetypedef) 
## HoursOfOperationOverrideConfigTypeDef

```python
# HoursOfOperationOverrideConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HoursOfOperationOverrideConfigTypeDef


def get_value() -> HoursOfOperationOverrideConfigTypeDef:
    return {
        "Day": ...,
    }


# HoursOfOperationOverrideConfigTypeDef definition

class HoursOfOperationOverrideConfigTypeDef(TypedDict):
    Day: NotRequired[OverrideDaysType],  # (1)
    StartTime: NotRequired[OverrideTimeSliceTypeDef],  # (2)
    EndTime: NotRequired[OverrideTimeSliceTypeDef],  # (2)
```

1. See [:material-code-brackets: OverrideDaysType](./literals.md#overridedaystype) 
2. See [:material-code-braces: OverrideTimeSliceTypeDef](./type_defs.md#overridetimeslicetypedef) 
3. See [:material-code-braces: OverrideTimeSliceTypeDef](./type_defs.md#overridetimeslicetypedef) 
## OperationalHourTypeDef

```python
# OperationalHourTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import OperationalHourTypeDef


def get_value() -> OperationalHourTypeDef:
    return {
        "Start": ...,
    }


# OperationalHourTypeDef definition

class OperationalHourTypeDef(TypedDict):
    Start: NotRequired[OverrideTimeSliceTypeDef],  # (1)
    End: NotRequired[OverrideTimeSliceTypeDef],  # (1)
```

1. See [:material-code-braces: OverrideTimeSliceTypeDef](./type_defs.md#overridetimeslicetypedef) 
2. See [:material-code-braces: OverrideTimeSliceTypeDef](./type_defs.md#overridetimeslicetypedef) 
## ListHoursOfOperationsResponseTypeDef

```python
# ListHoursOfOperationsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListHoursOfOperationsResponseTypeDef


def get_value() -> ListHoursOfOperationsResponseTypeDef:
    return {
        "HoursOfOperationSummaryList": ...,
    }


# ListHoursOfOperationsResponseTypeDef definition

class ListHoursOfOperationsResponseTypeDef(TypedDict):
    HoursOfOperationSummaryList: List[HoursOfOperationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HoursOfOperationSummaryTypeDef](./type_defs.md#hoursofoperationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InboundEmailContentTypeDef

```python
# InboundEmailContentTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import InboundEmailContentTypeDef


def get_value() -> InboundEmailContentTypeDef:
    return {
        "MessageSourceType": ...,
    }


# InboundEmailContentTypeDef definition

class InboundEmailContentTypeDef(TypedDict):
    MessageSourceType: InboundMessageSourceTypeType,  # (1)
    RawMessage: NotRequired[InboundRawMessageTypeDef],  # (2)
```

1. See [:material-code-brackets: InboundMessageSourceTypeType](./literals.md#inboundmessagesourcetypetype) 
2. See [:material-code-braces: InboundRawMessageTypeDef](./type_defs.md#inboundrawmessagetypedef) 
## InstanceTypeDef

```python
# InstanceTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import InstanceTypeDef


def get_value() -> InstanceTypeDef:
    return {
        "Id": ...,
    }


# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    IdentityManagementType: NotRequired[DirectoryTypeType],  # (1)
    InstanceAlias: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    ServiceRole: NotRequired[str],
    InstanceStatus: NotRequired[InstanceStatusType],  # (2)
    StatusReason: NotRequired[InstanceStatusReasonTypeDef],  # (3)
    InboundCallsEnabled: NotRequired[bool],
    OutboundCallsEnabled: NotRequired[bool],
    InstanceAccessUrl: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: DirectoryTypeType](./literals.md#directorytypetype) 
2. See [:material-code-brackets: InstanceStatusType](./literals.md#instancestatustype) 
3. See [:material-code-braces: InstanceStatusReasonTypeDef](./type_defs.md#instancestatusreasontypedef) 
## ListInstancesResponseTypeDef

```python
# ListInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListInstancesResponseTypeDef


def get_value() -> ListInstancesResponseTypeDef:
    return {
        "InstanceSummaryList": ...,
    }


# ListInstancesResponseTypeDef definition

class ListInstancesResponseTypeDef(TypedDict):
    InstanceSummaryList: List[InstanceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceSummaryTypeDef](./type_defs.md#instancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIntegrationAssociationsResponseTypeDef

```python
# ListIntegrationAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListIntegrationAssociationsResponseTypeDef


def get_value() -> ListIntegrationAssociationsResponseTypeDef:
    return {
        "IntegrationAssociationSummaryList": ...,
    }


# ListIntegrationAssociationsResponseTypeDef definition

class ListIntegrationAssociationsResponseTypeDef(TypedDict):
    IntegrationAssociationSummaryList: List[IntegrationAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IntegrationAssociationSummaryTypeDef](./type_defs.md#integrationassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvisibleFieldInfoTypeDef

```python
# InvisibleFieldInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import InvisibleFieldInfoTypeDef


def get_value() -> InvisibleFieldInfoTypeDef:
    return {
        "Id": ...,
    }


# InvisibleFieldInfoTypeDef definition

class InvisibleFieldInfoTypeDef(TypedDict):
    Id: NotRequired[TaskTemplateFieldIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: TaskTemplateFieldIdentifierTypeDef](./type_defs.md#tasktemplatefieldidentifiertypedef) 
## ReadOnlyFieldInfoTypeDef

```python
# ReadOnlyFieldInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ReadOnlyFieldInfoTypeDef


def get_value() -> ReadOnlyFieldInfoTypeDef:
    return {
        "Id": ...,
    }


# ReadOnlyFieldInfoTypeDef definition

class ReadOnlyFieldInfoTypeDef(TypedDict):
    Id: NotRequired[TaskTemplateFieldIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: TaskTemplateFieldIdentifierTypeDef](./type_defs.md#tasktemplatefieldidentifiertypedef) 
## RequiredFieldInfoTypeDef

```python
# RequiredFieldInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RequiredFieldInfoTypeDef


def get_value() -> RequiredFieldInfoTypeDef:
    return {
        "Id": ...,
    }


# RequiredFieldInfoTypeDef definition

class RequiredFieldInfoTypeDef(TypedDict):
    Id: NotRequired[TaskTemplateFieldIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: TaskTemplateFieldIdentifierTypeDef](./type_defs.md#tasktemplatefieldidentifiertypedef) 
## TaskTemplateDefaultFieldValueTypeDef

```python
# TaskTemplateDefaultFieldValueTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TaskTemplateDefaultFieldValueTypeDef


def get_value() -> TaskTemplateDefaultFieldValueTypeDef:
    return {
        "Id": ...,
    }


# TaskTemplateDefaultFieldValueTypeDef definition

class TaskTemplateDefaultFieldValueTypeDef(TypedDict):
    Id: NotRequired[TaskTemplateFieldIdentifierTypeDef],  # (1)
    DefaultValue: NotRequired[str],
```

1. See [:material-code-braces: TaskTemplateFieldIdentifierTypeDef](./type_defs.md#tasktemplatefieldidentifiertypedef) 
## TaskTemplateFieldOutputTypeDef

```python
# TaskTemplateFieldOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TaskTemplateFieldOutputTypeDef


def get_value() -> TaskTemplateFieldOutputTypeDef:
    return {
        "Id": ...,
    }


# TaskTemplateFieldOutputTypeDef definition

class TaskTemplateFieldOutputTypeDef(TypedDict):
    Id: TaskTemplateFieldIdentifierTypeDef,  # (1)
    Description: NotRequired[str],
    Type: NotRequired[TaskTemplateFieldTypeType],  # (2)
    SingleSelectOptions: NotRequired[List[str]],
```

1. See [:material-code-braces: TaskTemplateFieldIdentifierTypeDef](./type_defs.md#tasktemplatefieldidentifiertypedef) 
2. See [:material-code-brackets: TaskTemplateFieldTypeType](./literals.md#tasktemplatefieldtypetype) 
## TaskTemplateFieldTypeDef

```python
# TaskTemplateFieldTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TaskTemplateFieldTypeDef


def get_value() -> TaskTemplateFieldTypeDef:
    return {
        "Id": ...,
    }


# TaskTemplateFieldTypeDef definition

class TaskTemplateFieldTypeDef(TypedDict):
    Id: TaskTemplateFieldIdentifierTypeDef,  # (1)
    Description: NotRequired[str],
    Type: NotRequired[TaskTemplateFieldTypeType],  # (2)
    SingleSelectOptions: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: TaskTemplateFieldIdentifierTypeDef](./type_defs.md#tasktemplatefieldidentifiertypedef) 
2. See [:material-code-brackets: TaskTemplateFieldTypeType](./literals.md#tasktemplatefieldtypetype) 
## ListPhoneNumbersResponseTypeDef

```python
# ListPhoneNumbersResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListPhoneNumbersResponseTypeDef


def get_value() -> ListPhoneNumbersResponseTypeDef:
    return {
        "PhoneNumberSummaryList": ...,
    }


# ListPhoneNumbersResponseTypeDef definition

class ListPhoneNumbersResponseTypeDef(TypedDict):
    PhoneNumberSummaryList: List[PhoneNumberSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PhoneNumberSummaryTypeDef](./type_defs.md#phonenumbersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPhoneNumbersV2ResponseTypeDef

```python
# ListPhoneNumbersV2ResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListPhoneNumbersV2ResponseTypeDef


def get_value() -> ListPhoneNumbersV2ResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListPhoneNumbersV2ResponseTypeDef definition

class ListPhoneNumbersV2ResponseTypeDef(TypedDict):
    ListPhoneNumbersSummaryList: List[ListPhoneNumbersSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListPhoneNumbersSummaryTypeDef](./type_defs.md#listphonenumberssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPredefinedAttributesResponseTypeDef

```python
# ListPredefinedAttributesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListPredefinedAttributesResponseTypeDef


def get_value() -> ListPredefinedAttributesResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListPredefinedAttributesResponseTypeDef definition

class ListPredefinedAttributesResponseTypeDef(TypedDict):
    PredefinedAttributeSummaryList: List[PredefinedAttributeSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PredefinedAttributeSummaryTypeDef](./type_defs.md#predefinedattributesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPromptsResponseTypeDef

```python
# ListPromptsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListPromptsResponseTypeDef


def get_value() -> ListPromptsResponseTypeDef:
    return {
        "PromptSummaryList": ...,
    }


# ListPromptsResponseTypeDef definition

class ListPromptsResponseTypeDef(TypedDict):
    PromptSummaryList: List[PromptSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PromptSummaryTypeDef](./type_defs.md#promptsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueueQuickConnectsResponseTypeDef

```python
# ListQueueQuickConnectsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListQueueQuickConnectsResponseTypeDef


def get_value() -> ListQueueQuickConnectsResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListQueueQuickConnectsResponseTypeDef definition

class ListQueueQuickConnectsResponseTypeDef(TypedDict):
    QuickConnectSummaryList: List[QuickConnectSummaryTypeDef],  # (1)
    LastModifiedTime: datetime,
    LastModifiedRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QuickConnectSummaryTypeDef](./type_defs.md#quickconnectsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQuickConnectsResponseTypeDef

```python
# ListQuickConnectsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListQuickConnectsResponseTypeDef


def get_value() -> ListQuickConnectsResponseTypeDef:
    return {
        "QuickConnectSummaryList": ...,
    }


# ListQuickConnectsResponseTypeDef definition

class ListQuickConnectsResponseTypeDef(TypedDict):
    QuickConnectSummaryList: List[QuickConnectSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QuickConnectSummaryTypeDef](./type_defs.md#quickconnectsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueuesResponseTypeDef

```python
# ListQueuesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListQueuesResponseTypeDef


def get_value() -> ListQueuesResponseTypeDef:
    return {
        "QueueSummaryList": ...,
    }


# ListQueuesResponseTypeDef definition

class ListQueuesResponseTypeDef(TypedDict):
    QueueSummaryList: List[QueueSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QueueSummaryTypeDef](./type_defs.md#queuesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRoutingProfileQueuesResponseTypeDef

```python
# ListRoutingProfileQueuesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListRoutingProfileQueuesResponseTypeDef


def get_value() -> ListRoutingProfileQueuesResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListRoutingProfileQueuesResponseTypeDef definition

class ListRoutingProfileQueuesResponseTypeDef(TypedDict):
    RoutingProfileQueueConfigSummaryList: List[RoutingProfileQueueConfigSummaryTypeDef],  # (1)
    LastModifiedTime: datetime,
    LastModifiedRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RoutingProfileQueueConfigSummaryTypeDef](./type_defs.md#routingprofilequeueconfigsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRoutingProfilesResponseTypeDef

```python
# ListRoutingProfilesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListRoutingProfilesResponseTypeDef


def get_value() -> ListRoutingProfilesResponseTypeDef:
    return {
        "RoutingProfileSummaryList": ...,
    }


# ListRoutingProfilesResponseTypeDef definition

class ListRoutingProfilesResponseTypeDef(TypedDict):
    RoutingProfileSummaryList: List[RoutingProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RoutingProfileSummaryTypeDef](./type_defs.md#routingprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecurityKeysResponseTypeDef

```python
# ListSecurityKeysResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListSecurityKeysResponseTypeDef


def get_value() -> ListSecurityKeysResponseTypeDef:
    return {
        "SecurityKeys": ...,
    }


# ListSecurityKeysResponseTypeDef definition

class ListSecurityKeysResponseTypeDef(TypedDict):
    SecurityKeys: List[SecurityKeyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SecurityKeyTypeDef](./type_defs.md#securitykeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecurityProfilesResponseTypeDef

```python
# ListSecurityProfilesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListSecurityProfilesResponseTypeDef


def get_value() -> ListSecurityProfilesResponseTypeDef:
    return {
        "SecurityProfileSummaryList": ...,
    }


# ListSecurityProfilesResponseTypeDef definition

class ListSecurityProfilesResponseTypeDef(TypedDict):
    SecurityProfileSummaryList: List[SecurityProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SecurityProfileSummaryTypeDef](./type_defs.md#securityprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTaskTemplatesResponseTypeDef

```python
# ListTaskTemplatesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListTaskTemplatesResponseTypeDef


def get_value() -> ListTaskTemplatesResponseTypeDef:
    return {
        "TaskTemplates": ...,
    }


# ListTaskTemplatesResponseTypeDef definition

class ListTaskTemplatesResponseTypeDef(TypedDict):
    TaskTemplates: List[TaskTemplateMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TaskTemplateMetadataTypeDef](./type_defs.md#tasktemplatemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrafficDistributionGroupUsersResponseTypeDef

```python
# ListTrafficDistributionGroupUsersResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListTrafficDistributionGroupUsersResponseTypeDef


def get_value() -> ListTrafficDistributionGroupUsersResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListTrafficDistributionGroupUsersResponseTypeDef definition

class ListTrafficDistributionGroupUsersResponseTypeDef(TypedDict):
    TrafficDistributionGroupUserSummaryList: List[TrafficDistributionGroupUserSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TrafficDistributionGroupUserSummaryTypeDef](./type_defs.md#trafficdistributiongroupusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrafficDistributionGroupsResponseTypeDef

```python
# ListTrafficDistributionGroupsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListTrafficDistributionGroupsResponseTypeDef


def get_value() -> ListTrafficDistributionGroupsResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListTrafficDistributionGroupsResponseTypeDef definition

class ListTrafficDistributionGroupsResponseTypeDef(TypedDict):
    TrafficDistributionGroupSummaryList: List[TrafficDistributionGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TrafficDistributionGroupSummaryTypeDef](./type_defs.md#trafficdistributiongroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUseCasesResponseTypeDef

```python
# ListUseCasesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListUseCasesResponseTypeDef


def get_value() -> ListUseCasesResponseTypeDef:
    return {
        "UseCaseSummaryList": ...,
    }


# ListUseCasesResponseTypeDef definition

class ListUseCasesResponseTypeDef(TypedDict):
    UseCaseSummaryList: List[UseCaseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UseCaseTypeDef](./type_defs.md#usecasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersResponseTypeDef

```python
# ListUsersResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListUsersResponseTypeDef


def get_value() -> ListUsersResponseTypeDef:
    return {
        "UserSummaryList": ...,
    }


# ListUsersResponseTypeDef definition

class ListUsersResponseTypeDef(TypedDict):
    UserSummaryList: List[UserSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserSummaryTypeDef](./type_defs.md#usersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListViewVersionsResponseTypeDef

```python
# ListViewVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListViewVersionsResponseTypeDef


def get_value() -> ListViewVersionsResponseTypeDef:
    return {
        "ViewVersionSummaryList": ...,
    }


# ListViewVersionsResponseTypeDef definition

class ListViewVersionsResponseTypeDef(TypedDict):
    ViewVersionSummaryList: List[ViewVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ViewVersionSummaryTypeDef](./type_defs.md#viewversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListViewsResponseTypeDef

```python
# ListViewsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListViewsResponseTypeDef


def get_value() -> ListViewsResponseTypeDef:
    return {
        "ViewsSummaryList": ...,
    }


# ListViewsResponseTypeDef definition

class ListViewsResponseTypeDef(TypedDict):
    ViewsSummaryList: List[ViewSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ViewSummaryTypeDef](./type_defs.md#viewsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricV2OutputTypeDef

```python
# MetricV2OutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MetricV2OutputTypeDef


def get_value() -> MetricV2OutputTypeDef:
    return {
        "Name": ...,
    }


# MetricV2OutputTypeDef definition

class MetricV2OutputTypeDef(TypedDict):
    Name: NotRequired[str],
    Threshold: NotRequired[List[ThresholdV2TypeDef]],  # (1)
    MetricFilters: NotRequired[List[MetricFilterV2OutputTypeDef]],  # (2)
```

1. See [:material-code-braces: ThresholdV2TypeDef](./type_defs.md#thresholdv2typedef) 
2. See [:material-code-braces: MetricFilterV2OutputTypeDef](./type_defs.md#metricfilterv2outputtypedef) 
## NewSessionDetailsTypeDef

```python
# NewSessionDetailsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import NewSessionDetailsTypeDef


def get_value() -> NewSessionDetailsTypeDef:
    return {
        "SupportedMessagingContentTypes": ...,
    }


# NewSessionDetailsTypeDef definition

class NewSessionDetailsTypeDef(TypedDict):
    SupportedMessagingContentTypes: NotRequired[Sequence[str]],
    ParticipantDetails: NotRequired[ParticipantDetailsTypeDef],  # (1)
    Attributes: NotRequired[Mapping[str, str]],
    StreamingConfiguration: NotRequired[ChatStreamingConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ParticipantDetailsTypeDef](./type_defs.md#participantdetailstypedef) 
2. See [:material-code-braces: ChatStreamingConfigurationTypeDef](./type_defs.md#chatstreamingconfigurationtypedef) 
## SendNotificationActionDefinitionOutputTypeDef

```python
# SendNotificationActionDefinitionOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SendNotificationActionDefinitionOutputTypeDef


def get_value() -> SendNotificationActionDefinitionOutputTypeDef:
    return {
        "DeliveryMethod": ...,
    }


# SendNotificationActionDefinitionOutputTypeDef definition

class SendNotificationActionDefinitionOutputTypeDef(TypedDict):
    DeliveryMethod: NotificationDeliveryTypeType,  # (1)
    Content: str,
    ContentType: NotificationContentTypeType,  # (2)
    Recipient: NotificationRecipientTypeOutputTypeDef,  # (3)
    Subject: NotRequired[str],
```

1. See [:material-code-brackets: NotificationDeliveryTypeType](./literals.md#notificationdeliverytypetype) 
2. See [:material-code-brackets: NotificationContentTypeType](./literals.md#notificationcontenttypetype) 
3. See [:material-code-braces: NotificationRecipientTypeOutputTypeDef](./type_defs.md#notificationrecipienttypeoutputtypedef) 
## ParticipantTimerConfigurationTypeDef

```python
# ParticipantTimerConfigurationTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ParticipantTimerConfigurationTypeDef


def get_value() -> ParticipantTimerConfigurationTypeDef:
    return {
        "ParticipantRole": ...,
    }


# ParticipantTimerConfigurationTypeDef definition

class ParticipantTimerConfigurationTypeDef(TypedDict):
    ParticipantRole: TimerEligibleParticipantRolesType,  # (1)
    TimerType: ParticipantTimerTypeType,  # (2)
    TimerValue: ParticipantTimerValueTypeDef,  # (3)
```

1. See [:material-code-brackets: TimerEligibleParticipantRolesType](./literals.md#timereligibleparticipantrolestype) 
2. See [:material-code-brackets: ParticipantTimerTypeType](./literals.md#participanttimertypetype) 
3. See [:material-code-braces: ParticipantTimerValueTypeDef](./type_defs.md#participanttimervaluetypedef) 
## PredefinedAttributeTypeDef

```python
# PredefinedAttributeTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PredefinedAttributeTypeDef


def get_value() -> PredefinedAttributeTypeDef:
    return {
        "Name": ...,
    }


# PredefinedAttributeTypeDef definition

class PredefinedAttributeTypeDef(TypedDict):
    Name: NotRequired[str],
    Values: NotRequired[PredefinedAttributeValuesOutputTypeDef],  # (1)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-braces: PredefinedAttributeValuesOutputTypeDef](./type_defs.md#predefinedattributevaluesoutputtypedef) 
## QuickConnectConfigTypeDef

```python
# QuickConnectConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QuickConnectConfigTypeDef


def get_value() -> QuickConnectConfigTypeDef:
    return {
        "QuickConnectType": ...,
    }


# QuickConnectConfigTypeDef definition

class QuickConnectConfigTypeDef(TypedDict):
    QuickConnectType: QuickConnectTypeType,  # (1)
    UserConfig: NotRequired[UserQuickConnectConfigTypeDef],  # (2)
    QueueConfig: NotRequired[QueueQuickConnectConfigTypeDef],  # (3)
    PhoneConfig: NotRequired[PhoneNumberQuickConnectConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: QuickConnectTypeType](./literals.md#quickconnecttypetype) 
2. See [:material-code-braces: UserQuickConnectConfigTypeDef](./type_defs.md#userquickconnectconfigtypedef) 
3. See [:material-code-braces: QueueQuickConnectConfigTypeDef](./type_defs.md#queuequickconnectconfigtypedef) 
4. See [:material-code-braces: PhoneNumberQuickConnectConfigTypeDef](./type_defs.md#phonenumberquickconnectconfigtypedef) 
## RealTimeContactAnalysisTranscriptItemRedactionTypeDef

```python
# RealTimeContactAnalysisTranscriptItemRedactionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisTranscriptItemRedactionTypeDef


def get_value() -> RealTimeContactAnalysisTranscriptItemRedactionTypeDef:
    return {
        "CharacterOffsets": ...,
    }


# RealTimeContactAnalysisTranscriptItemRedactionTypeDef definition

class RealTimeContactAnalysisTranscriptItemRedactionTypeDef(TypedDict):
    CharacterOffsets: NotRequired[List[RealTimeContactAnalysisCharacterIntervalTypeDef]],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisCharacterIntervalTypeDef](./type_defs.md#realtimecontactanalysischaracterintervaltypedef) 
## RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef

```python
# RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef


def get_value() -> RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef:
    return {
        "Id": ...,
    }


# RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef definition

class RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef(TypedDict):
    Id: str,
    CharacterOffsets: NotRequired[RealTimeContactAnalysisCharacterIntervalTypeDef],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisCharacterIntervalTypeDef](./type_defs.md#realtimecontactanalysischaracterintervaltypedef) 
## RealTimeContactAnalysisTranscriptItemWithContentTypeDef

```python
# RealTimeContactAnalysisTranscriptItemWithContentTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisTranscriptItemWithContentTypeDef


def get_value() -> RealTimeContactAnalysisTranscriptItemWithContentTypeDef:
    return {
        "Content": ...,
    }


# RealTimeContactAnalysisTranscriptItemWithContentTypeDef definition

class RealTimeContactAnalysisTranscriptItemWithContentTypeDef(TypedDict):
    Id: str,
    Content: NotRequired[str],
    CharacterOffsets: NotRequired[RealTimeContactAnalysisCharacterIntervalTypeDef],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisCharacterIntervalTypeDef](./type_defs.md#realtimecontactanalysischaracterintervaltypedef) 
## RealTimeContactAnalysisSegmentAttachmentsTypeDef

```python
# RealTimeContactAnalysisSegmentAttachmentsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisSegmentAttachmentsTypeDef


def get_value() -> RealTimeContactAnalysisSegmentAttachmentsTypeDef:
    return {
        "Id": ...,
    }


# RealTimeContactAnalysisSegmentAttachmentsTypeDef definition

class RealTimeContactAnalysisSegmentAttachmentsTypeDef(TypedDict):
    Id: str,
    ParticipantId: str,
    ParticipantRole: ParticipantRoleType,  # (1)
    Attachments: List[RealTimeContactAnalysisAttachmentTypeDef],  # (2)
    Time: RealTimeContactAnalysisTimeDataTypeDef,  # (3)
    DisplayName: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
2. See [:material-code-braces: RealTimeContactAnalysisAttachmentTypeDef](./type_defs.md#realtimecontactanalysisattachmenttypedef) 
3. See [:material-code-braces: RealTimeContactAnalysisTimeDataTypeDef](./type_defs.md#realtimecontactanalysistimedatatypedef) 
## RealTimeContactAnalysisSegmentEventTypeDef

```python
# RealTimeContactAnalysisSegmentEventTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisSegmentEventTypeDef


def get_value() -> RealTimeContactAnalysisSegmentEventTypeDef:
    return {
        "Id": ...,
    }


# RealTimeContactAnalysisSegmentEventTypeDef definition

class RealTimeContactAnalysisSegmentEventTypeDef(TypedDict):
    Id: str,
    EventType: str,
    Time: RealTimeContactAnalysisTimeDataTypeDef,  # (2)
    ParticipantId: NotRequired[str],
    ParticipantRole: NotRequired[ParticipantRoleType],  # (1)
    DisplayName: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
2. See [:material-code-braces: RealTimeContactAnalysisTimeDataTypeDef](./type_defs.md#realtimecontactanalysistimedatatypedef) 
## ReferenceSummaryTypeDef

```python
# ReferenceSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ReferenceSummaryTypeDef


def get_value() -> ReferenceSummaryTypeDef:
    return {
        "Url": ...,
    }


# ReferenceSummaryTypeDef definition

class ReferenceSummaryTypeDef(TypedDict):
    Url: NotRequired[UrlReferenceTypeDef],  # (1)
    Attachment: NotRequired[AttachmentReferenceTypeDef],  # (2)
    EmailMessage: NotRequired[EmailMessageReferenceTypeDef],  # (3)
    String: NotRequired[StringReferenceTypeDef],  # (4)
    Number: NotRequired[NumberReferenceTypeDef],  # (5)
    Date: NotRequired[DateReferenceTypeDef],  # (6)
    Email: NotRequired[EmailReferenceTypeDef],  # (7)
```

1. See [:material-code-braces: UrlReferenceTypeDef](./type_defs.md#urlreferencetypedef) 
2. See [:material-code-braces: AttachmentReferenceTypeDef](./type_defs.md#attachmentreferencetypedef) 
3. See [:material-code-braces: EmailMessageReferenceTypeDef](./type_defs.md#emailmessagereferencetypedef) 
4. See [:material-code-braces: StringReferenceTypeDef](./type_defs.md#stringreferencetypedef) 
5. See [:material-code-braces: NumberReferenceTypeDef](./type_defs.md#numberreferencetypedef) 
6. See [:material-code-braces: DateReferenceTypeDef](./type_defs.md#datereferencetypedef) 
7. See [:material-code-braces: EmailReferenceTypeDef](./type_defs.md#emailreferencetypedef) 
## ReplicationConfigurationTypeDef

```python
# ReplicationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ReplicationConfigurationTypeDef


def get_value() -> ReplicationConfigurationTypeDef:
    return {
        "ReplicationStatusSummaryList": ...,
    }


# ReplicationConfigurationTypeDef definition

class ReplicationConfigurationTypeDef(TypedDict):
    ReplicationStatusSummaryList: NotRequired[List[ReplicationStatusSummaryTypeDef]],  # (1)
    SourceRegion: NotRequired[str],
    GlobalSignInEndpoint: NotRequired[str],
```

1. See [:material-code-braces: ReplicationStatusSummaryTypeDef](./type_defs.md#replicationstatussummarytypedef) 
## ResourceTagsSearchCriteriaTypeDef

```python
# ResourceTagsSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ResourceTagsSearchCriteriaTypeDef


def get_value() -> ResourceTagsSearchCriteriaTypeDef:
    return {
        "TagSearchCondition": ...,
    }


# ResourceTagsSearchCriteriaTypeDef definition

class ResourceTagsSearchCriteriaTypeDef(TypedDict):
    TagSearchCondition: NotRequired[TagSearchConditionTypeDef],  # (1)
```

1. See [:material-code-braces: TagSearchConditionTypeDef](./type_defs.md#tagsearchconditiontypedef) 
## SearchResourceTagsResponseTypeDef

```python
# SearchResourceTagsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchResourceTagsResponseTypeDef


def get_value() -> SearchResourceTagsResponseTypeDef:
    return {
        "Tags": ...,
    }


# SearchResourceTagsResponseTypeDef definition

class SearchResourceTagsResponseTypeDef(TypedDict):
    Tags: List[TagSetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagSetTypeDef](./type_defs.md#tagsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchSecurityProfilesResponseTypeDef

```python
# SearchSecurityProfilesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchSecurityProfilesResponseTypeDef


def get_value() -> SearchSecurityProfilesResponseTypeDef:
    return {
        "SecurityProfiles": ...,
    }


# SearchSecurityProfilesResponseTypeDef definition

class SearchSecurityProfilesResponseTypeDef(TypedDict):
    SecurityProfiles: List[SecurityProfileSearchSummaryTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SecurityProfileSearchSummaryTypeDef](./type_defs.md#securityprofilesearchsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchVocabulariesResponseTypeDef

```python
# SearchVocabulariesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchVocabulariesResponseTypeDef


def get_value() -> SearchVocabulariesResponseTypeDef:
    return {
        "VocabularySummaryList": ...,
    }


# SearchVocabulariesResponseTypeDef definition

class SearchVocabulariesResponseTypeDef(TypedDict):
    VocabularySummaryList: List[VocabularySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VocabularySummaryTypeDef](./type_defs.md#vocabularysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchableContactAttributesTypeDef

```python
# SearchableContactAttributesTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchableContactAttributesTypeDef


def get_value() -> SearchableContactAttributesTypeDef:
    return {
        "Criteria": ...,
    }


# SearchableContactAttributesTypeDef definition

class SearchableContactAttributesTypeDef(TypedDict):
    Criteria: Sequence[SearchableContactAttributesCriteriaTypeDef],  # (1)
    MatchType: NotRequired[SearchContactsMatchTypeType],  # (2)
```

1. See [:material-code-braces: SearchableContactAttributesCriteriaTypeDef](./type_defs.md#searchablecontactattributescriteriatypedef) 
2. See [:material-code-brackets: SearchContactsMatchTypeType](./literals.md#searchcontactsmatchtypetype) 
## SearchableSegmentAttributesTypeDef

```python
# SearchableSegmentAttributesTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchableSegmentAttributesTypeDef


def get_value() -> SearchableSegmentAttributesTypeDef:
    return {
        "Criteria": ...,
    }


# SearchableSegmentAttributesTypeDef definition

class SearchableSegmentAttributesTypeDef(TypedDict):
    Criteria: Sequence[SearchableSegmentAttributesCriteriaTypeDef],  # (1)
    MatchType: NotRequired[SearchContactsMatchTypeType],  # (2)
```

1. See [:material-code-braces: SearchableSegmentAttributesCriteriaTypeDef](./type_defs.md#searchablesegmentattributescriteriatypedef) 
2. See [:material-code-brackets: SearchContactsMatchTypeType](./literals.md#searchcontactsmatchtypetype) 
## SignInConfigOutputTypeDef

```python
# SignInConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SignInConfigOutputTypeDef


def get_value() -> SignInConfigOutputTypeDef:
    return {
        "Distributions": ...,
    }


# SignInConfigOutputTypeDef definition

class SignInConfigOutputTypeDef(TypedDict):
    Distributions: List[SignInDistributionTypeDef],  # (1)
```

1. See [:material-code-braces: SignInDistributionTypeDef](./type_defs.md#signindistributiontypedef) 
## SignInConfigTypeDef

```python
# SignInConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SignInConfigTypeDef


def get_value() -> SignInConfigTypeDef:
    return {
        "Distributions": ...,
    }


# SignInConfigTypeDef definition

class SignInConfigTypeDef(TypedDict):
    Distributions: Sequence[SignInDistributionTypeDef],  # (1)
```

1. See [:material-code-braces: SignInDistributionTypeDef](./type_defs.md#signindistributiontypedef) 
## StartAttachedFileUploadResponseTypeDef

```python
# StartAttachedFileUploadResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartAttachedFileUploadResponseTypeDef


def get_value() -> StartAttachedFileUploadResponseTypeDef:
    return {
        "FileArn": ...,
    }


# StartAttachedFileUploadResponseTypeDef definition

class StartAttachedFileUploadResponseTypeDef(TypedDict):
    FileArn: str,
    FileId: str,
    CreationTime: str,
    FileStatus: FileStatusTypeType,  # (1)
    CreatedBy: CreatedByInfoTypeDef,  # (2)
    UploadUrlMetadata: UploadUrlMetadataTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: FileStatusTypeType](./literals.md#filestatustypetype) 
2. See [:material-code-braces: CreatedByInfoTypeDef](./type_defs.md#createdbyinfotypedef) 
3. See [:material-code-braces: UploadUrlMetadataTypeDef](./type_defs.md#uploadurlmetadatatypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartContactRecordingRequestTypeDef

```python
# StartContactRecordingRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartContactRecordingRequestTypeDef


def get_value() -> StartContactRecordingRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# StartContactRecordingRequestTypeDef definition

class StartContactRecordingRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
    VoiceRecordingConfiguration: VoiceRecordingConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: VoiceRecordingConfigurationTypeDef](./type_defs.md#voicerecordingconfigurationtypedef) 
## TemplatedMessageConfigTypeDef

```python
# TemplatedMessageConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TemplatedMessageConfigTypeDef


def get_value() -> TemplatedMessageConfigTypeDef:
    return {
        "KnowledgeBaseId": ...,
    }


# TemplatedMessageConfigTypeDef definition

class TemplatedMessageConfigTypeDef(TypedDict):
    KnowledgeBaseId: str,
    MessageTemplateId: str,
    TemplateAttributes: TemplateAttributesTypeDef,  # (1)
```

1. See [:material-code-braces: TemplateAttributesTypeDef](./type_defs.md#templateattributestypedef) 
## TranscriptTypeDef

```python
# TranscriptTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TranscriptTypeDef


def get_value() -> TranscriptTypeDef:
    return {
        "Criteria": ...,
    }


# TranscriptTypeDef definition

class TranscriptTypeDef(TypedDict):
    Criteria: Sequence[TranscriptCriteriaTypeDef],  # (1)
    MatchType: NotRequired[SearchContactsMatchTypeType],  # (2)
```

1. See [:material-code-braces: TranscriptCriteriaTypeDef](./type_defs.md#transcriptcriteriatypedef) 
2. See [:material-code-brackets: SearchContactsMatchTypeType](./literals.md#searchcontactsmatchtypetype) 
## UserSearchSummaryTypeDef

```python
# UserSearchSummaryTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserSearchSummaryTypeDef


def get_value() -> UserSearchSummaryTypeDef:
    return {
        "Arn": ...,
    }


# UserSearchSummaryTypeDef definition

class UserSearchSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    DirectoryUserId: NotRequired[str],
    HierarchyGroupId: NotRequired[str],
    Id: NotRequired[str],
    IdentityInfo: NotRequired[UserIdentityInfoLiteTypeDef],  # (1)
    PhoneConfig: NotRequired[UserPhoneConfigTypeDef],  # (2)
    RoutingProfileId: NotRequired[str],
    SecurityProfileIds: NotRequired[List[str]],
    Tags: NotRequired[Dict[str, str]],
    Username: NotRequired[str],
```

1. See [:material-code-braces: UserIdentityInfoLiteTypeDef](./type_defs.md#useridentityinfolitetypedef) 
2. See [:material-code-braces: UserPhoneConfigTypeDef](./type_defs.md#userphoneconfigtypedef) 
## ViewTypeDef

```python
# ViewTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ViewTypeDef


def get_value() -> ViewTypeDef:
    return {
        "Id": ...,
    }


# ViewTypeDef definition

class ViewTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[ViewStatusType],  # (1)
    Type: NotRequired[ViewTypeType],  # (2)
    Description: NotRequired[str],
    Version: NotRequired[int],
    VersionDescription: NotRequired[str],
    Content: NotRequired[ViewContentTypeDef],  # (3)
    Tags: NotRequired[Dict[str, str]],
    CreatedTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    ViewContentSha256: NotRequired[str],
```

1. See [:material-code-brackets: ViewStatusType](./literals.md#viewstatustype) 
2. See [:material-code-brackets: ViewTypeType](./literals.md#viewtypetype) 
3. See [:material-code-braces: ViewContentTypeDef](./type_defs.md#viewcontenttypedef) 
## ListRulesResponseTypeDef

```python
# ListRulesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListRulesResponseTypeDef


def get_value() -> ListRulesResponseTypeDef:
    return {
        "RuleSummaryList": ...,
    }


# ListRulesResponseTypeDef definition

class ListRulesResponseTypeDef(TypedDict):
    RuleSummaryList: List[RuleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AgentInfoTypeDef

```python
# AgentInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentInfoTypeDef


def get_value() -> AgentInfoTypeDef:
    return {
        "Id": ...,
    }


# AgentInfoTypeDef definition

class AgentInfoTypeDef(TypedDict):
    Id: NotRequired[str],
    ConnectedToAgentTimestamp: NotRequired[datetime],
    AgentPauseDurationInSeconds: NotRequired[int],
    HierarchyGroups: NotRequired[HierarchyGroupsTypeDef],  # (1)
    DeviceInfo: NotRequired[DeviceInfoTypeDef],  # (2)
    Capabilities: NotRequired[ParticipantCapabilitiesTypeDef],  # (3)
```

1. See [:material-code-braces: HierarchyGroupsTypeDef](./type_defs.md#hierarchygroupstypedef) 
2. See [:material-code-braces: DeviceInfoTypeDef](./type_defs.md#deviceinfotypedef) 
3. See [:material-code-braces: ParticipantCapabilitiesTypeDef](./type_defs.md#participantcapabilitiestypedef) 
## StartWebRTCContactRequestTypeDef

```python
# StartWebRTCContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartWebRTCContactRequestTypeDef


def get_value() -> StartWebRTCContactRequestTypeDef:
    return {
        "ContactFlowId": ...,
    }


# StartWebRTCContactRequestTypeDef definition

class StartWebRTCContactRequestTypeDef(TypedDict):
    ContactFlowId: str,
    InstanceId: str,
    ParticipantDetails: ParticipantDetailsTypeDef,  # (1)
    Attributes: NotRequired[Mapping[str, str]],
    ClientToken: NotRequired[str],
    AllowedCapabilities: NotRequired[AllowedCapabilitiesTypeDef],  # (2)
    RelatedContactId: NotRequired[str],
    References: NotRequired[Mapping[str, ReferenceTypeDef]],  # (3)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ParticipantDetailsTypeDef](./type_defs.md#participantdetailstypedef) 
2. See [:material-code-braces: AllowedCapabilitiesTypeDef](./type_defs.md#allowedcapabilitiestypedef) 
3. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
## QualityMetricsTypeDef

```python
# QualityMetricsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QualityMetricsTypeDef


def get_value() -> QualityMetricsTypeDef:
    return {
        "Agent": ...,
    }


# QualityMetricsTypeDef definition

class QualityMetricsTypeDef(TypedDict):
    Agent: NotRequired[AgentQualityMetricsTypeDef],  # (1)
    Customer: NotRequired[CustomerQualityMetricsTypeDef],  # (2)
```

1. See [:material-code-braces: AgentQualityMetricsTypeDef](./type_defs.md#agentqualitymetricstypedef) 
2. See [:material-code-braces: CustomerQualityMetricsTypeDef](./type_defs.md#customerqualitymetricstypedef) 
## SearchPredefinedAttributesRequestPaginateTypeDef

```python
# SearchPredefinedAttributesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchPredefinedAttributesRequestPaginateTypeDef


def get_value() -> SearchPredefinedAttributesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchPredefinedAttributesRequestPaginateTypeDef definition

class SearchPredefinedAttributesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchCriteria: NotRequired[PredefinedAttributeSearchCriteriaPaginatorTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PredefinedAttributeSearchCriteriaPaginatorTypeDef](./type_defs.md#predefinedattributesearchcriteriapaginatortypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchPredefinedAttributesRequestTypeDef

```python
# SearchPredefinedAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchPredefinedAttributesRequestTypeDef


def get_value() -> SearchPredefinedAttributesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchPredefinedAttributesRequestTypeDef definition

class SearchPredefinedAttributesRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchCriteria: NotRequired[PredefinedAttributeSearchCriteriaTypeDef],  # (1)
```

1. See [:material-code-braces: PredefinedAttributeSearchCriteriaTypeDef](./type_defs.md#predefinedattributesearchcriteriatypedef) 
## AttributeConditionOutputTypeDef

```python
# AttributeConditionOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AttributeConditionOutputTypeDef


def get_value() -> AttributeConditionOutputTypeDef:
    return {
        "Name": ...,
    }


# AttributeConditionOutputTypeDef definition

class AttributeConditionOutputTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
    ProficiencyLevel: NotRequired[float],
    Range: NotRequired[RangeTypeDef],  # (1)
    MatchCriteria: NotRequired[MatchCriteriaOutputTypeDef],  # (2)
    ComparisonOperator: NotRequired[str],
```

1. See [:material-code-braces: RangeTypeDef](./type_defs.md#rangetypedef) 
2. See [:material-code-braces: MatchCriteriaOutputTypeDef](./type_defs.md#matchcriteriaoutputtypedef) 
## MatchCriteriaTypeDef

```python
# MatchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MatchCriteriaTypeDef


def get_value() -> MatchCriteriaTypeDef:
    return {
        "AgentsCriteria": ...,
    }


# MatchCriteriaTypeDef definition

class MatchCriteriaTypeDef(TypedDict):
    AgentsCriteria: NotRequired[AgentsCriteriaUnionTypeDef],  # (1)
```

1. See [:material-code-braces: AgentsCriteriaTypeDef](./type_defs.md#agentscriteriatypedef) [:material-code-braces: AgentsCriteriaOutputTypeDef](./type_defs.md#agentscriteriaoutputtypedef) 
## CreateSecurityProfileRequestTypeDef

```python
# CreateSecurityProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateSecurityProfileRequestTypeDef


def get_value() -> CreateSecurityProfileRequestTypeDef:
    return {
        "SecurityProfileName": ...,
    }


# CreateSecurityProfileRequestTypeDef definition

class CreateSecurityProfileRequestTypeDef(TypedDict):
    SecurityProfileName: str,
    InstanceId: str,
    Description: NotRequired[str],
    Permissions: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
    AllowedAccessControlTags: NotRequired[Mapping[str, str]],
    TagRestrictedResources: NotRequired[Sequence[str]],
    Applications: NotRequired[Sequence[ApplicationUnionTypeDef]],  # (1)
    HierarchyRestrictedResources: NotRequired[Sequence[str]],
    AllowedAccessControlHierarchyGroupId: NotRequired[str],
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) [:material-code-braces: ApplicationOutputTypeDef](./type_defs.md#applicationoutputtypedef) 
## UpdateSecurityProfileRequestTypeDef

```python
# UpdateSecurityProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateSecurityProfileRequestTypeDef


def get_value() -> UpdateSecurityProfileRequestTypeDef:
    return {
        "SecurityProfileId": ...,
    }


# UpdateSecurityProfileRequestTypeDef definition

class UpdateSecurityProfileRequestTypeDef(TypedDict):
    SecurityProfileId: str,
    InstanceId: str,
    Description: NotRequired[str],
    Permissions: NotRequired[Sequence[str]],
    AllowedAccessControlTags: NotRequired[Mapping[str, str]],
    TagRestrictedResources: NotRequired[Sequence[str]],
    Applications: NotRequired[Sequence[ApplicationUnionTypeDef]],  # (1)
    HierarchyRestrictedResources: NotRequired[Sequence[str]],
    AllowedAccessControlHierarchyGroupId: NotRequired[str],
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) [:material-code-braces: ApplicationOutputTypeDef](./type_defs.md#applicationoutputtypedef) 
## ListBotsResponseTypeDef

```python
# ListBotsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListBotsResponseTypeDef


def get_value() -> ListBotsResponseTypeDef:
    return {
        "LexBots": ...,
    }


# ListBotsResponseTypeDef definition

class ListBotsResponseTypeDef(TypedDict):
    LexBots: List[LexBotConfigTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LexBotConfigTypeDef](./type_defs.md#lexbotconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetAttachedFileMetadataResponseTypeDef

```python
# BatchGetAttachedFileMetadataResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import BatchGetAttachedFileMetadataResponseTypeDef


def get_value() -> BatchGetAttachedFileMetadataResponseTypeDef:
    return {
        "Files": ...,
    }


# BatchGetAttachedFileMetadataResponseTypeDef definition

class BatchGetAttachedFileMetadataResponseTypeDef(TypedDict):
    Files: List[AttachedFileTypeDef],  # (1)
    Errors: List[AttachedFileErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AttachedFileTypeDef](./type_defs.md#attachedfiletypedef) 
2. See [:material-code-braces: AttachedFileErrorTypeDef](./type_defs.md#attachedfileerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ControlPlaneUserAttributeFilterTypeDef

```python
# ControlPlaneUserAttributeFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ControlPlaneUserAttributeFilterTypeDef


def get_value() -> ControlPlaneUserAttributeFilterTypeDef:
    return {
        "OrConditions": ...,
    }


# ControlPlaneUserAttributeFilterTypeDef definition

class ControlPlaneUserAttributeFilterTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[AttributeAndConditionTypeDef]],  # (1)
    AndCondition: NotRequired[AttributeAndConditionTypeDef],  # (2)
    TagCondition: NotRequired[TagConditionTypeDef],  # (3)
    HierarchyGroupCondition: NotRequired[HierarchyGroupConditionTypeDef],  # (4)
```

1. See [:material-code-braces: AttributeAndConditionTypeDef](./type_defs.md#attributeandconditiontypedef) 
2. See [:material-code-braces: AttributeAndConditionTypeDef](./type_defs.md#attributeandconditiontypedef) 
3. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
4. See [:material-code-braces: HierarchyGroupConditionTypeDef](./type_defs.md#hierarchygroupconditiontypedef) 
## ControlPlaneAttributeFilterTypeDef

```python
# ControlPlaneAttributeFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ControlPlaneAttributeFilterTypeDef


def get_value() -> ControlPlaneAttributeFilterTypeDef:
    return {
        "OrConditions": ...,
    }


# ControlPlaneAttributeFilterTypeDef definition

class ControlPlaneAttributeFilterTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[CommonAttributeAndConditionTypeDef]],  # (1)
    AndCondition: NotRequired[CommonAttributeAndConditionTypeDef],  # (2)
    TagCondition: NotRequired[TagConditionTypeDef],  # (3)
```

1. See [:material-code-braces: CommonAttributeAndConditionTypeDef](./type_defs.md#commonattributeandconditiontypedef) 
2. See [:material-code-braces: CommonAttributeAndConditionTypeDef](./type_defs.md#commonattributeandconditiontypedef) 
3. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
## ContactFlowModuleSearchFilterTypeDef

```python
# ContactFlowModuleSearchFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactFlowModuleSearchFilterTypeDef


def get_value() -> ContactFlowModuleSearchFilterTypeDef:
    return {
        "TagFilter": ...,
    }


# ContactFlowModuleSearchFilterTypeDef definition

class ContactFlowModuleSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## ContactFlowSearchFilterTypeDef

```python
# ContactFlowSearchFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactFlowSearchFilterTypeDef


def get_value() -> ContactFlowSearchFilterTypeDef:
    return {
        "TagFilter": ...,
    }


# ContactFlowSearchFilterTypeDef definition

class ContactFlowSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## EmailAddressSearchFilterTypeDef

```python
# EmailAddressSearchFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EmailAddressSearchFilterTypeDef


def get_value() -> EmailAddressSearchFilterTypeDef:
    return {
        "TagFilter": ...,
    }


# EmailAddressSearchFilterTypeDef definition

class EmailAddressSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## HoursOfOperationSearchFilterTypeDef

```python
# HoursOfOperationSearchFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HoursOfOperationSearchFilterTypeDef


def get_value() -> HoursOfOperationSearchFilterTypeDef:
    return {
        "TagFilter": ...,
    }


# HoursOfOperationSearchFilterTypeDef definition

class HoursOfOperationSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## PromptSearchFilterTypeDef

```python
# PromptSearchFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import PromptSearchFilterTypeDef


def get_value() -> PromptSearchFilterTypeDef:
    return {
        "TagFilter": ...,
    }


# PromptSearchFilterTypeDef definition

class PromptSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## QueueSearchFilterTypeDef

```python
# QueueSearchFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QueueSearchFilterTypeDef


def get_value() -> QueueSearchFilterTypeDef:
    return {
        "TagFilter": ...,
    }


# QueueSearchFilterTypeDef definition

class QueueSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## QuickConnectSearchFilterTypeDef

```python
# QuickConnectSearchFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QuickConnectSearchFilterTypeDef


def get_value() -> QuickConnectSearchFilterTypeDef:
    return {
        "TagFilter": ...,
    }


# QuickConnectSearchFilterTypeDef definition

class QuickConnectSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## RoutingProfileSearchFilterTypeDef

```python
# RoutingProfileSearchFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RoutingProfileSearchFilterTypeDef


def get_value() -> RoutingProfileSearchFilterTypeDef:
    return {
        "TagFilter": ...,
    }


# RoutingProfileSearchFilterTypeDef definition

class RoutingProfileSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## SecurityProfilesSearchFilterTypeDef

```python
# SecurityProfilesSearchFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SecurityProfilesSearchFilterTypeDef


def get_value() -> SecurityProfilesSearchFilterTypeDef:
    return {
        "TagFilter": ...,
    }


# SecurityProfilesSearchFilterTypeDef definition

class SecurityProfilesSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## MeetingTypeDef

```python
# MeetingTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MeetingTypeDef


def get_value() -> MeetingTypeDef:
    return {
        "MediaRegion": ...,
    }


# MeetingTypeDef definition

class MeetingTypeDef(TypedDict):
    MediaRegion: NotRequired[str],
    MediaPlacement: NotRequired[MediaPlacementTypeDef],  # (1)
    MeetingFeatures: NotRequired[MeetingFeaturesConfigurationTypeDef],  # (2)
    MeetingId: NotRequired[str],
```

1. See [:material-code-braces: MediaPlacementTypeDef](./type_defs.md#mediaplacementtypedef) 
2. See [:material-code-braces: MeetingFeaturesConfigurationTypeDef](./type_defs.md#meetingfeaturesconfigurationtypedef) 
## DescribePhoneNumberResponseTypeDef

```python
# DescribePhoneNumberResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribePhoneNumberResponseTypeDef


def get_value() -> DescribePhoneNumberResponseTypeDef:
    return {
        "ClaimedPhoneNumberSummary": ...,
    }


# DescribePhoneNumberResponseTypeDef definition

class DescribePhoneNumberResponseTypeDef(TypedDict):
    ClaimedPhoneNumberSummary: ClaimedPhoneNumberSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClaimedPhoneNumberSummaryTypeDef](./type_defs.md#claimedphonenumbersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConditionTypeDef

```python
# ListConditionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListConditionTypeDef


def get_value() -> ListConditionTypeDef:
    return {
        "TargetListType": ...,
    }


# ListConditionTypeDef definition

class ListConditionTypeDef(TypedDict):
    TargetListType: NotRequired[TargetListTypeType],  # (1)
    Conditions: NotRequired[Sequence[ConditionTypeDef]],  # (2)
```

1. See [:material-code-brackets: TargetListTypeType](./literals.md#targetlisttypetype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
## BatchPutContactRequestTypeDef

```python
# BatchPutContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import BatchPutContactRequestTypeDef


def get_value() -> BatchPutContactRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# BatchPutContactRequestTypeDef definition

class BatchPutContactRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactDataRequestList: Sequence[ContactDataRequestTypeDef],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: ContactDataRequestTypeDef](./type_defs.md#contactdatarequesttypedef) 
## GetCurrentUserDataRequestTypeDef

```python
# GetCurrentUserDataRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetCurrentUserDataRequestTypeDef


def get_value() -> GetCurrentUserDataRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# GetCurrentUserDataRequestTypeDef definition

class GetCurrentUserDataRequestTypeDef(TypedDict):
    InstanceId: str,
    Filters: UserDataFiltersTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: UserDataFiltersTypeDef](./type_defs.md#userdatafilterstypedef) 
## SearchContactsResponseTypeDef

```python
# SearchContactsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchContactsResponseTypeDef


def get_value() -> SearchContactsResponseTypeDef:
    return {
        "Contacts": ...,
    }


# SearchContactsResponseTypeDef definition

class SearchContactsResponseTypeDef(TypedDict):
    Contacts: List[ContactSearchSummaryTypeDef],  # (1)
    TotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContactSearchSummaryTypeDef](./type_defs.md#contactsearchsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeQueueResponseTypeDef

```python
# DescribeQueueResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeQueueResponseTypeDef


def get_value() -> DescribeQueueResponseTypeDef:
    return {
        "Queue": ...,
    }


# DescribeQueueResponseTypeDef definition

class DescribeQueueResponseTypeDef(TypedDict):
    Queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchQueuesResponseTypeDef

```python
# SearchQueuesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchQueuesResponseTypeDef


def get_value() -> SearchQueuesResponseTypeDef:
    return {
        "Queues": ...,
    }


# SearchQueuesResponseTypeDef definition

class SearchQueuesResponseTypeDef(TypedDict):
    Queues: List[QueueTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserResponseTypeDef

```python
# DescribeUserResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeUserResponseTypeDef


def get_value() -> DescribeUserResponseTypeDef:
    return {
        "User": ...,
    }


# DescribeUserResponseTypeDef definition

class DescribeUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RoutingProfileTypeDef

```python
# RoutingProfileTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RoutingProfileTypeDef


def get_value() -> RoutingProfileTypeDef:
    return {
        "InstanceId": ...,
    }


# RoutingProfileTypeDef definition

class RoutingProfileTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    Name: NotRequired[str],
    RoutingProfileArn: NotRequired[str],
    RoutingProfileId: NotRequired[str],
    Description: NotRequired[str],
    MediaConcurrencies: NotRequired[List[MediaConcurrencyTypeDef]],  # (1)
    DefaultOutboundQueueId: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    NumberOfAssociatedQueues: NotRequired[int],
    NumberOfAssociatedUsers: NotRequired[int],
    AgentAvailabilityTimer: NotRequired[AgentAvailabilityTimerType],  # (2)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
    IsDefault: NotRequired[bool],
    AssociatedQueueIds: NotRequired[List[str]],
```

1. See [:material-code-braces: MediaConcurrencyTypeDef](./type_defs.md#mediaconcurrencytypedef) 
2. See [:material-code-brackets: AgentAvailabilityTimerType](./literals.md#agentavailabilitytimertype) 
## UpdateRoutingProfileConcurrencyRequestTypeDef

```python
# UpdateRoutingProfileConcurrencyRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateRoutingProfileConcurrencyRequestTypeDef


def get_value() -> UpdateRoutingProfileConcurrencyRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateRoutingProfileConcurrencyRequestTypeDef definition

class UpdateRoutingProfileConcurrencyRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    MediaConcurrencies: Sequence[MediaConcurrencyTypeDef],  # (1)
```

1. See [:material-code-braces: MediaConcurrencyTypeDef](./type_defs.md#mediaconcurrencytypedef) 
## CurrentMetricResultTypeDef

```python
# CurrentMetricResultTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CurrentMetricResultTypeDef


def get_value() -> CurrentMetricResultTypeDef:
    return {
        "Dimensions": ...,
    }


# CurrentMetricResultTypeDef definition

class CurrentMetricResultTypeDef(TypedDict):
    Dimensions: NotRequired[DimensionsTypeDef],  # (1)
    Collections: NotRequired[List[CurrentMetricDataTypeDef]],  # (2)
```

1. See [:material-code-braces: DimensionsTypeDef](./type_defs.md#dimensionstypedef) 
2. See [:material-code-braces: CurrentMetricDataTypeDef](./type_defs.md#currentmetricdatatypedef) 
## AssociateRoutingProfileQueuesRequestTypeDef

```python
# AssociateRoutingProfileQueuesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateRoutingProfileQueuesRequestTypeDef


def get_value() -> AssociateRoutingProfileQueuesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# AssociateRoutingProfileQueuesRequestTypeDef definition

class AssociateRoutingProfileQueuesRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef],  # (1)
```

1. See [:material-code-braces: RoutingProfileQueueConfigTypeDef](./type_defs.md#routingprofilequeueconfigtypedef) 
## CreateRoutingProfileRequestTypeDef

```python
# CreateRoutingProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateRoutingProfileRequestTypeDef


def get_value() -> CreateRoutingProfileRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateRoutingProfileRequestTypeDef definition

class CreateRoutingProfileRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    Description: str,
    DefaultOutboundQueueId: str,
    MediaConcurrencies: Sequence[MediaConcurrencyTypeDef],  # (1)
    QueueConfigs: NotRequired[Sequence[RoutingProfileQueueConfigTypeDef]],  # (2)
    Tags: NotRequired[Mapping[str, str]],
    AgentAvailabilityTimer: NotRequired[AgentAvailabilityTimerType],  # (3)
```

1. See [:material-code-braces: MediaConcurrencyTypeDef](./type_defs.md#mediaconcurrencytypedef) 
2. See [:material-code-braces: RoutingProfileQueueConfigTypeDef](./type_defs.md#routingprofilequeueconfigtypedef) 
3. See [:material-code-brackets: AgentAvailabilityTimerType](./literals.md#agentavailabilitytimertype) 
## UpdateRoutingProfileQueuesRequestTypeDef

```python
# UpdateRoutingProfileQueuesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateRoutingProfileQueuesRequestTypeDef


def get_value() -> UpdateRoutingProfileQueuesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateRoutingProfileQueuesRequestTypeDef definition

class UpdateRoutingProfileQueuesRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef],  # (1)
```

1. See [:material-code-braces: RoutingProfileQueueConfigTypeDef](./type_defs.md#routingprofilequeueconfigtypedef) 
## InstanceStorageConfigTypeDef

```python
# InstanceStorageConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import InstanceStorageConfigTypeDef


def get_value() -> InstanceStorageConfigTypeDef:
    return {
        "AssociationId": ...,
    }


# InstanceStorageConfigTypeDef definition

class InstanceStorageConfigTypeDef(TypedDict):
    StorageType: StorageTypeType,  # (1)
    AssociationId: NotRequired[str],
    S3Config: NotRequired[S3ConfigTypeDef],  # (2)
    KinesisVideoStreamConfig: NotRequired[KinesisVideoStreamConfigTypeDef],  # (3)
    KinesisStreamConfig: NotRequired[KinesisStreamConfigTypeDef],  # (4)
    KinesisFirehoseConfig: NotRequired[KinesisFirehoseConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
2. See [:material-code-braces: S3ConfigTypeDef](./type_defs.md#s3configtypedef) 
3. See [:material-code-braces: KinesisVideoStreamConfigTypeDef](./type_defs.md#kinesisvideostreamconfigtypedef) 
4. See [:material-code-braces: KinesisStreamConfigTypeDef](./type_defs.md#kinesisstreamconfigtypedef) 
5. See [:material-code-braces: KinesisFirehoseConfigTypeDef](./type_defs.md#kinesisfirehoseconfigtypedef) 
## SubmitContactEvaluationRequestTypeDef

```python
# SubmitContactEvaluationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SubmitContactEvaluationRequestTypeDef


def get_value() -> SubmitContactEvaluationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SubmitContactEvaluationRequestTypeDef definition

class SubmitContactEvaluationRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationId: str,
    Answers: NotRequired[Mapping[str, EvaluationAnswerInputTypeDef]],  # (1)
    Notes: NotRequired[Mapping[str, EvaluationNoteTypeDef]],  # (2)
```

1. See [:material-code-braces: EvaluationAnswerInputTypeDef](./type_defs.md#evaluationanswerinputtypedef) 
2. See [:material-code-braces: EvaluationNoteTypeDef](./type_defs.md#evaluationnotetypedef) 
## UpdateContactEvaluationRequestTypeDef

```python
# UpdateContactEvaluationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateContactEvaluationRequestTypeDef


def get_value() -> UpdateContactEvaluationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateContactEvaluationRequestTypeDef definition

class UpdateContactEvaluationRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationId: str,
    Answers: NotRequired[Mapping[str, EvaluationAnswerInputTypeDef]],  # (1)
    Notes: NotRequired[Mapping[str, EvaluationNoteTypeDef]],  # (2)
```

1. See [:material-code-braces: EvaluationAnswerInputTypeDef](./type_defs.md#evaluationanswerinputtypedef) 
2. See [:material-code-braces: EvaluationNoteTypeDef](./type_defs.md#evaluationnotetypedef) 
## EvaluationFormNumericQuestionPropertiesOutputTypeDef

```python
# EvaluationFormNumericQuestionPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormNumericQuestionPropertiesOutputTypeDef


def get_value() -> EvaluationFormNumericQuestionPropertiesOutputTypeDef:
    return {
        "MinValue": ...,
    }


# EvaluationFormNumericQuestionPropertiesOutputTypeDef definition

class EvaluationFormNumericQuestionPropertiesOutputTypeDef(TypedDict):
    MinValue: int,
    MaxValue: int,
    Options: NotRequired[List[EvaluationFormNumericQuestionOptionTypeDef]],  # (1)
    Automation: NotRequired[EvaluationFormNumericQuestionAutomationTypeDef],  # (2)
```

1. See [:material-code-braces: EvaluationFormNumericQuestionOptionTypeDef](./type_defs.md#evaluationformnumericquestionoptiontypedef) 
2. See [:material-code-braces: EvaluationFormNumericQuestionAutomationTypeDef](./type_defs.md#evaluationformnumericquestionautomationtypedef) 
## EvaluationFormNumericQuestionPropertiesTypeDef

```python
# EvaluationFormNumericQuestionPropertiesTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormNumericQuestionPropertiesTypeDef


def get_value() -> EvaluationFormNumericQuestionPropertiesTypeDef:
    return {
        "MinValue": ...,
    }


# EvaluationFormNumericQuestionPropertiesTypeDef definition

class EvaluationFormNumericQuestionPropertiesTypeDef(TypedDict):
    MinValue: int,
    MaxValue: int,
    Options: NotRequired[Sequence[EvaluationFormNumericQuestionOptionTypeDef]],  # (1)
    Automation: NotRequired[EvaluationFormNumericQuestionAutomationTypeDef],  # (2)
```

1. See [:material-code-braces: EvaluationFormNumericQuestionOptionTypeDef](./type_defs.md#evaluationformnumericquestionoptiontypedef) 
2. See [:material-code-braces: EvaluationFormNumericQuestionAutomationTypeDef](./type_defs.md#evaluationformnumericquestionautomationtypedef) 
## EvaluationFormSingleSelectQuestionAutomationOutputTypeDef

```python
# EvaluationFormSingleSelectQuestionAutomationOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormSingleSelectQuestionAutomationOutputTypeDef


def get_value() -> EvaluationFormSingleSelectQuestionAutomationOutputTypeDef:
    return {
        "Options": ...,
    }


# EvaluationFormSingleSelectQuestionAutomationOutputTypeDef definition

class EvaluationFormSingleSelectQuestionAutomationOutputTypeDef(TypedDict):
    Options: List[EvaluationFormSingleSelectQuestionAutomationOptionTypeDef],  # (1)
    DefaultOptionRefId: NotRequired[str],
```

1. See [:material-code-braces: EvaluationFormSingleSelectQuestionAutomationOptionTypeDef](./type_defs.md#evaluationformsingleselectquestionautomationoptiontypedef) 
## EvaluationFormSingleSelectQuestionAutomationTypeDef

```python
# EvaluationFormSingleSelectQuestionAutomationTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormSingleSelectQuestionAutomationTypeDef


def get_value() -> EvaluationFormSingleSelectQuestionAutomationTypeDef:
    return {
        "Options": ...,
    }


# EvaluationFormSingleSelectQuestionAutomationTypeDef definition

class EvaluationFormSingleSelectQuestionAutomationTypeDef(TypedDict):
    Options: Sequence[EvaluationFormSingleSelectQuestionAutomationOptionTypeDef],  # (1)
    DefaultOptionRefId: NotRequired[str],
```

1. See [:material-code-braces: EvaluationFormSingleSelectQuestionAutomationOptionTypeDef](./type_defs.md#evaluationformsingleselectquestionautomationoptiontypedef) 
## EvaluationTypeDef

```python
# EvaluationTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationTypeDef


def get_value() -> EvaluationTypeDef:
    return {
        "EvaluationId": ...,
    }


# EvaluationTypeDef definition

class EvaluationTypeDef(TypedDict):
    EvaluationId: str,
    EvaluationArn: str,
    Metadata: EvaluationMetadataTypeDef,  # (1)
    Answers: Dict[str, EvaluationAnswerOutputTypeDef],  # (2)
    Notes: Dict[str, EvaluationNoteTypeDef],  # (3)
    Status: EvaluationStatusType,  # (4)
    CreatedTime: datetime,
    LastModifiedTime: datetime,
    Scores: NotRequired[Dict[str, EvaluationScoreTypeDef]],  # (5)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: EvaluationMetadataTypeDef](./type_defs.md#evaluationmetadatatypedef) 
2. See [:material-code-braces: EvaluationAnswerOutputTypeDef](./type_defs.md#evaluationansweroutputtypedef) 
3. See [:material-code-braces: EvaluationNoteTypeDef](./type_defs.md#evaluationnotetypedef) 
4. See [:material-code-brackets: EvaluationStatusType](./literals.md#evaluationstatustype) 
5. See [:material-code-braces: EvaluationScoreTypeDef](./type_defs.md#evaluationscoretypedef) 
## ListContactEvaluationsResponseTypeDef

```python
# ListContactEvaluationsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactEvaluationsResponseTypeDef


def get_value() -> ListContactEvaluationsResponseTypeDef:
    return {
        "EvaluationSummaryList": ...,
    }


# ListContactEvaluationsResponseTypeDef definition

class ListContactEvaluationsResponseTypeDef(TypedDict):
    EvaluationSummaryList: List[EvaluationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EvaluationSummaryTypeDef](./type_defs.md#evaluationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCaseActionDefinitionOutputTypeDef

```python
# CreateCaseActionDefinitionOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateCaseActionDefinitionOutputTypeDef


def get_value() -> CreateCaseActionDefinitionOutputTypeDef:
    return {
        "Fields": ...,
    }


# CreateCaseActionDefinitionOutputTypeDef definition

class CreateCaseActionDefinitionOutputTypeDef(TypedDict):
    Fields: List[FieldValueOutputTypeDef],  # (1)
    TemplateId: str,
```

1. See [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
## UpdateCaseActionDefinitionOutputTypeDef

```python
# UpdateCaseActionDefinitionOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateCaseActionDefinitionOutputTypeDef


def get_value() -> UpdateCaseActionDefinitionOutputTypeDef:
    return {
        "Fields": ...,
    }


# UpdateCaseActionDefinitionOutputTypeDef definition

class UpdateCaseActionDefinitionOutputTypeDef(TypedDict):
    Fields: List[FieldValueOutputTypeDef],  # (1)
```

1. See [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
## FieldValueTypeDef

```python
# FieldValueTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import FieldValueTypeDef


def get_value() -> FieldValueTypeDef:
    return {
        "Id": ...,
    }


# FieldValueTypeDef definition

class FieldValueTypeDef(TypedDict):
    Id: str,
    Value: FieldValueUnionUnionTypeDef,  # (1)
```

1. See [:material-code-braces: FieldValueUnionTypeDef](./type_defs.md#fieldvalueuniontypedef) [:material-code-braces: FieldValueUnionOutputTypeDef](./type_defs.md#fieldvalueunionoutputtypedef) 
## UserDataTypeDef

```python
# UserDataTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserDataTypeDef


def get_value() -> UserDataTypeDef:
    return {
        "User": ...,
    }


# UserDataTypeDef definition

class UserDataTypeDef(TypedDict):
    User: NotRequired[UserReferenceTypeDef],  # (1)
    RoutingProfile: NotRequired[RoutingProfileReferenceTypeDef],  # (2)
    HierarchyPath: NotRequired[HierarchyPathReferenceTypeDef],  # (3)
    Status: NotRequired[AgentStatusReferenceTypeDef],  # (4)
    AvailableSlotsByChannel: NotRequired[Dict[ChannelType, int]],  # (5)
    MaxSlotsByChannel: NotRequired[Dict[ChannelType, int]],  # (5)
    ActiveSlotsByChannel: NotRequired[Dict[ChannelType, int]],  # (5)
    Contacts: NotRequired[List[AgentContactReferenceTypeDef]],  # (8)
    NextStatus: NotRequired[str],
```

1. See [:material-code-braces: UserReferenceTypeDef](./type_defs.md#userreferencetypedef) 
2. See [:material-code-braces: RoutingProfileReferenceTypeDef](./type_defs.md#routingprofilereferencetypedef) 
3. See [:material-code-braces: HierarchyPathReferenceTypeDef](./type_defs.md#hierarchypathreferencetypedef) 
4. See [:material-code-braces: AgentStatusReferenceTypeDef](./type_defs.md#agentstatusreferencetypedef) 
5. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
6. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
7. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
8. See [:material-code-braces: AgentContactReferenceTypeDef](./type_defs.md#agentcontactreferencetypedef) 
## HierarchyGroupTypeDef

```python
# HierarchyGroupTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HierarchyGroupTypeDef


def get_value() -> HierarchyGroupTypeDef:
    return {
        "Id": ...,
    }


# HierarchyGroupTypeDef definition

class HierarchyGroupTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LevelId: NotRequired[str],
    HierarchyPath: NotRequired[HierarchyPathTypeDef],  # (1)
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-braces: HierarchyPathTypeDef](./type_defs.md#hierarchypathtypedef) 
## DescribeUserHierarchyStructureResponseTypeDef

```python
# DescribeUserHierarchyStructureResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeUserHierarchyStructureResponseTypeDef


def get_value() -> DescribeUserHierarchyStructureResponseTypeDef:
    return {
        "HierarchyStructure": ...,
    }


# DescribeUserHierarchyStructureResponseTypeDef definition

class DescribeUserHierarchyStructureResponseTypeDef(TypedDict):
    HierarchyStructure: HierarchyStructureTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HierarchyStructureTypeDef](./type_defs.md#hierarchystructuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserHierarchyStructureRequestTypeDef

```python
# UpdateUserHierarchyStructureRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateUserHierarchyStructureRequestTypeDef


def get_value() -> UpdateUserHierarchyStructureRequestTypeDef:
    return {
        "HierarchyStructure": ...,
    }


# UpdateUserHierarchyStructureRequestTypeDef definition

class UpdateUserHierarchyStructureRequestTypeDef(TypedDict):
    HierarchyStructure: HierarchyStructureUpdateTypeDef,  # (1)
    InstanceId: str,
```

1. See [:material-code-braces: HierarchyStructureUpdateTypeDef](./type_defs.md#hierarchystructureupdatetypedef) 
## GetMetricDataRequestPaginateTypeDef

```python
# GetMetricDataRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetMetricDataRequestPaginateTypeDef


def get_value() -> GetMetricDataRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# GetMetricDataRequestPaginateTypeDef definition

class GetMetricDataRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Filters: FiltersTypeDef,  # (1)
    HistoricalMetrics: Sequence[HistoricalMetricTypeDef],  # (2)
    Groupings: NotRequired[Sequence[GroupingType]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
2. See [:material-code-braces: HistoricalMetricTypeDef](./type_defs.md#historicalmetrictypedef) 
3. See [:material-code-brackets: GroupingType](./literals.md#groupingtype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetMetricDataRequestTypeDef

```python
# GetMetricDataRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetMetricDataRequestTypeDef


def get_value() -> GetMetricDataRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# GetMetricDataRequestTypeDef definition

class GetMetricDataRequestTypeDef(TypedDict):
    InstanceId: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Filters: FiltersTypeDef,  # (1)
    HistoricalMetrics: Sequence[HistoricalMetricTypeDef],  # (2)
    Groupings: NotRequired[Sequence[GroupingType]],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
2. See [:material-code-braces: HistoricalMetricTypeDef](./type_defs.md#historicalmetrictypedef) 
3. See [:material-code-brackets: GroupingType](./literals.md#groupingtype) 
## HistoricalMetricDataTypeDef

```python
# HistoricalMetricDataTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HistoricalMetricDataTypeDef


def get_value() -> HistoricalMetricDataTypeDef:
    return {
        "Metric": ...,
    }


# HistoricalMetricDataTypeDef definition

class HistoricalMetricDataTypeDef(TypedDict):
    Metric: NotRequired[HistoricalMetricTypeDef],  # (1)
    Value: NotRequired[float],
```

1. See [:material-code-braces: HistoricalMetricTypeDef](./type_defs.md#historicalmetrictypedef) 
## CreateHoursOfOperationRequestTypeDef

```python
# CreateHoursOfOperationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateHoursOfOperationRequestTypeDef


def get_value() -> CreateHoursOfOperationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateHoursOfOperationRequestTypeDef definition

class CreateHoursOfOperationRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    TimeZone: str,
    Config: Sequence[HoursOfOperationConfigTypeDef],  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: HoursOfOperationConfigTypeDef](./type_defs.md#hoursofoperationconfigtypedef) 
## HoursOfOperationTypeDef

```python
# HoursOfOperationTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HoursOfOperationTypeDef


def get_value() -> HoursOfOperationTypeDef:
    return {
        "HoursOfOperationId": ...,
    }


# HoursOfOperationTypeDef definition

class HoursOfOperationTypeDef(TypedDict):
    HoursOfOperationId: NotRequired[str],
    HoursOfOperationArn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    TimeZone: NotRequired[str],
    Config: NotRequired[List[HoursOfOperationConfigTypeDef]],  # (1)
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-braces: HoursOfOperationConfigTypeDef](./type_defs.md#hoursofoperationconfigtypedef) 
## UpdateHoursOfOperationRequestTypeDef

```python
# UpdateHoursOfOperationRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateHoursOfOperationRequestTypeDef


def get_value() -> UpdateHoursOfOperationRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateHoursOfOperationRequestTypeDef definition

class UpdateHoursOfOperationRequestTypeDef(TypedDict):
    InstanceId: str,
    HoursOfOperationId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    TimeZone: NotRequired[str],
    Config: NotRequired[Sequence[HoursOfOperationConfigTypeDef]],  # (1)
```

1. See [:material-code-braces: HoursOfOperationConfigTypeDef](./type_defs.md#hoursofoperationconfigtypedef) 
## CreateHoursOfOperationOverrideRequestTypeDef

```python
# CreateHoursOfOperationOverrideRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateHoursOfOperationOverrideRequestTypeDef


def get_value() -> CreateHoursOfOperationOverrideRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateHoursOfOperationOverrideRequestTypeDef definition

class CreateHoursOfOperationOverrideRequestTypeDef(TypedDict):
    InstanceId: str,
    HoursOfOperationId: str,
    Name: str,
    Config: Sequence[HoursOfOperationOverrideConfigTypeDef],  # (1)
    EffectiveFrom: str,
    EffectiveTill: str,
    Description: NotRequired[str],
```

1. See [:material-code-braces: HoursOfOperationOverrideConfigTypeDef](./type_defs.md#hoursofoperationoverrideconfigtypedef) 
## HoursOfOperationOverrideTypeDef

```python
# HoursOfOperationOverrideTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HoursOfOperationOverrideTypeDef


def get_value() -> HoursOfOperationOverrideTypeDef:
    return {
        "HoursOfOperationOverrideId": ...,
    }


# HoursOfOperationOverrideTypeDef definition

class HoursOfOperationOverrideTypeDef(TypedDict):
    HoursOfOperationOverrideId: NotRequired[str],
    HoursOfOperationId: NotRequired[str],
    HoursOfOperationArn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Config: NotRequired[List[HoursOfOperationOverrideConfigTypeDef]],  # (1)
    EffectiveFrom: NotRequired[str],
    EffectiveTill: NotRequired[str],
```

1. See [:material-code-braces: HoursOfOperationOverrideConfigTypeDef](./type_defs.md#hoursofoperationoverrideconfigtypedef) 
## UpdateHoursOfOperationOverrideRequestTypeDef

```python
# UpdateHoursOfOperationOverrideRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateHoursOfOperationOverrideRequestTypeDef


def get_value() -> UpdateHoursOfOperationOverrideRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateHoursOfOperationOverrideRequestTypeDef definition

class UpdateHoursOfOperationOverrideRequestTypeDef(TypedDict):
    InstanceId: str,
    HoursOfOperationId: str,
    HoursOfOperationOverrideId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    Config: NotRequired[Sequence[HoursOfOperationOverrideConfigTypeDef]],  # (1)
    EffectiveFrom: NotRequired[str],
    EffectiveTill: NotRequired[str],
```

1. See [:material-code-braces: HoursOfOperationOverrideConfigTypeDef](./type_defs.md#hoursofoperationoverrideconfigtypedef) 
## EffectiveHoursOfOperationsTypeDef

```python
# EffectiveHoursOfOperationsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EffectiveHoursOfOperationsTypeDef


def get_value() -> EffectiveHoursOfOperationsTypeDef:
    return {
        "Date": ...,
    }


# EffectiveHoursOfOperationsTypeDef definition

class EffectiveHoursOfOperationsTypeDef(TypedDict):
    Date: NotRequired[str],
    OperationalHours: NotRequired[List[OperationalHourTypeDef]],  # (1)
```

1. See [:material-code-braces: OperationalHourTypeDef](./type_defs.md#operationalhourtypedef) 
## TaskTemplateConstraintsOutputTypeDef

```python
# TaskTemplateConstraintsOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TaskTemplateConstraintsOutputTypeDef


def get_value() -> TaskTemplateConstraintsOutputTypeDef:
    return {
        "RequiredFields": ...,
    }


# TaskTemplateConstraintsOutputTypeDef definition

class TaskTemplateConstraintsOutputTypeDef(TypedDict):
    RequiredFields: NotRequired[List[RequiredFieldInfoTypeDef]],  # (1)
    ReadOnlyFields: NotRequired[List[ReadOnlyFieldInfoTypeDef]],  # (2)
    InvisibleFields: NotRequired[List[InvisibleFieldInfoTypeDef]],  # (3)
```

1. See [:material-code-braces: RequiredFieldInfoTypeDef](./type_defs.md#requiredfieldinfotypedef) 
2. See [:material-code-braces: ReadOnlyFieldInfoTypeDef](./type_defs.md#readonlyfieldinfotypedef) 
3. See [:material-code-braces: InvisibleFieldInfoTypeDef](./type_defs.md#invisiblefieldinfotypedef) 
## TaskTemplateConstraintsTypeDef

```python
# TaskTemplateConstraintsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TaskTemplateConstraintsTypeDef


def get_value() -> TaskTemplateConstraintsTypeDef:
    return {
        "RequiredFields": ...,
    }


# TaskTemplateConstraintsTypeDef definition

class TaskTemplateConstraintsTypeDef(TypedDict):
    RequiredFields: NotRequired[Sequence[RequiredFieldInfoTypeDef]],  # (1)
    ReadOnlyFields: NotRequired[Sequence[ReadOnlyFieldInfoTypeDef]],  # (2)
    InvisibleFields: NotRequired[Sequence[InvisibleFieldInfoTypeDef]],  # (3)
```

1. See [:material-code-braces: RequiredFieldInfoTypeDef](./type_defs.md#requiredfieldinfotypedef) 
2. See [:material-code-braces: ReadOnlyFieldInfoTypeDef](./type_defs.md#readonlyfieldinfotypedef) 
3. See [:material-code-braces: InvisibleFieldInfoTypeDef](./type_defs.md#invisiblefieldinfotypedef) 
## TaskTemplateDefaultsOutputTypeDef

```python
# TaskTemplateDefaultsOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TaskTemplateDefaultsOutputTypeDef


def get_value() -> TaskTemplateDefaultsOutputTypeDef:
    return {
        "DefaultFieldValues": ...,
    }


# TaskTemplateDefaultsOutputTypeDef definition

class TaskTemplateDefaultsOutputTypeDef(TypedDict):
    DefaultFieldValues: NotRequired[List[TaskTemplateDefaultFieldValueTypeDef]],  # (1)
```

1. See [:material-code-braces: TaskTemplateDefaultFieldValueTypeDef](./type_defs.md#tasktemplatedefaultfieldvaluetypedef) 
## TaskTemplateDefaultsTypeDef

```python
# TaskTemplateDefaultsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import TaskTemplateDefaultsTypeDef


def get_value() -> TaskTemplateDefaultsTypeDef:
    return {
        "DefaultFieldValues": ...,
    }


# TaskTemplateDefaultsTypeDef definition

class TaskTemplateDefaultsTypeDef(TypedDict):
    DefaultFieldValues: NotRequired[Sequence[TaskTemplateDefaultFieldValueTypeDef]],  # (1)
```

1. See [:material-code-braces: TaskTemplateDefaultFieldValueTypeDef](./type_defs.md#tasktemplatedefaultfieldvaluetypedef) 
## MetricV2TypeDef

```python
# MetricV2TypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MetricV2TypeDef


def get_value() -> MetricV2TypeDef:
    return {
        "Name": ...,
    }


# MetricV2TypeDef definition

class MetricV2TypeDef(TypedDict):
    Name: NotRequired[str],
    Threshold: NotRequired[Sequence[ThresholdV2TypeDef]],  # (1)
    MetricFilters: NotRequired[Sequence[MetricFilterV2UnionTypeDef]],  # (2)
```

1. See [:material-code-braces: ThresholdV2TypeDef](./type_defs.md#thresholdv2typedef) 
2. See [:material-code-braces: MetricFilterV2TypeDef](./type_defs.md#metricfilterv2typedef) [:material-code-braces: MetricFilterV2OutputTypeDef](./type_defs.md#metricfilterv2outputtypedef) 
## MetricDataV2TypeDef

```python
# MetricDataV2TypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MetricDataV2TypeDef


def get_value() -> MetricDataV2TypeDef:
    return {
        "Metric": ...,
    }


# MetricDataV2TypeDef definition

class MetricDataV2TypeDef(TypedDict):
    Metric: NotRequired[MetricV2OutputTypeDef],  # (1)
    Value: NotRequired[float],
```

1. See [:material-code-braces: MetricV2OutputTypeDef](./type_defs.md#metricv2outputtypedef) 
## SendChatIntegrationEventRequestTypeDef

```python
# SendChatIntegrationEventRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SendChatIntegrationEventRequestTypeDef


def get_value() -> SendChatIntegrationEventRequestTypeDef:
    return {
        "SourceId": ...,
    }


# SendChatIntegrationEventRequestTypeDef definition

class SendChatIntegrationEventRequestTypeDef(TypedDict):
    SourceId: str,
    DestinationId: str,
    Event: ChatEventTypeDef,  # (1)
    Subtype: NotRequired[str],
    NewSessionDetails: NotRequired[NewSessionDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: ChatEventTypeDef](./type_defs.md#chateventtypedef) 
2. See [:material-code-braces: NewSessionDetailsTypeDef](./type_defs.md#newsessiondetailstypedef) 
## SendNotificationActionDefinitionTypeDef

```python
# SendNotificationActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SendNotificationActionDefinitionTypeDef


def get_value() -> SendNotificationActionDefinitionTypeDef:
    return {
        "DeliveryMethod": ...,
    }


# SendNotificationActionDefinitionTypeDef definition

class SendNotificationActionDefinitionTypeDef(TypedDict):
    DeliveryMethod: NotificationDeliveryTypeType,  # (1)
    Content: str,
    ContentType: NotificationContentTypeType,  # (2)
    Recipient: NotificationRecipientTypeUnionTypeDef,  # (3)
    Subject: NotRequired[str],
```

1. See [:material-code-brackets: NotificationDeliveryTypeType](./literals.md#notificationdeliverytypetype) 
2. See [:material-code-brackets: NotificationContentTypeType](./literals.md#notificationcontenttypetype) 
3. See [:material-code-braces: NotificationRecipientTypeTypeDef](./type_defs.md#notificationrecipienttypetypedef) [:material-code-braces: NotificationRecipientTypeOutputTypeDef](./type_defs.md#notificationrecipienttypeoutputtypedef) 
## ChatParticipantRoleConfigTypeDef

```python
# ChatParticipantRoleConfigTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ChatParticipantRoleConfigTypeDef


def get_value() -> ChatParticipantRoleConfigTypeDef:
    return {
        "ParticipantTimerConfigList": ...,
    }


# ChatParticipantRoleConfigTypeDef definition

class ChatParticipantRoleConfigTypeDef(TypedDict):
    ParticipantTimerConfigList: Sequence[ParticipantTimerConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ParticipantTimerConfigurationTypeDef](./type_defs.md#participanttimerconfigurationtypedef) 
## DescribePredefinedAttributeResponseTypeDef

```python
# DescribePredefinedAttributeResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribePredefinedAttributeResponseTypeDef


def get_value() -> DescribePredefinedAttributeResponseTypeDef:
    return {
        "PredefinedAttribute": ...,
    }


# DescribePredefinedAttributeResponseTypeDef definition

class DescribePredefinedAttributeResponseTypeDef(TypedDict):
    PredefinedAttribute: PredefinedAttributeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PredefinedAttributeTypeDef](./type_defs.md#predefinedattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchPredefinedAttributesResponseTypeDef

```python
# SearchPredefinedAttributesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchPredefinedAttributesResponseTypeDef


def get_value() -> SearchPredefinedAttributesResponseTypeDef:
    return {
        "PredefinedAttributes": ...,
    }


# SearchPredefinedAttributesResponseTypeDef definition

class SearchPredefinedAttributesResponseTypeDef(TypedDict):
    PredefinedAttributes: List[PredefinedAttributeTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PredefinedAttributeTypeDef](./type_defs.md#predefinedattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePredefinedAttributeRequestTypeDef

```python
# CreatePredefinedAttributeRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreatePredefinedAttributeRequestTypeDef


def get_value() -> CreatePredefinedAttributeRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreatePredefinedAttributeRequestTypeDef definition

class CreatePredefinedAttributeRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    Values: PredefinedAttributeValuesUnionTypeDef,  # (1)
```

1. See [:material-code-braces: PredefinedAttributeValuesTypeDef](./type_defs.md#predefinedattributevaluestypedef) [:material-code-braces: PredefinedAttributeValuesOutputTypeDef](./type_defs.md#predefinedattributevaluesoutputtypedef) 
## UpdatePredefinedAttributeRequestTypeDef

```python
# UpdatePredefinedAttributeRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdatePredefinedAttributeRequestTypeDef


def get_value() -> UpdatePredefinedAttributeRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdatePredefinedAttributeRequestTypeDef definition

class UpdatePredefinedAttributeRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    Values: NotRequired[PredefinedAttributeValuesUnionTypeDef],  # (1)
```

1. See [:material-code-braces: PredefinedAttributeValuesTypeDef](./type_defs.md#predefinedattributevaluestypedef) [:material-code-braces: PredefinedAttributeValuesOutputTypeDef](./type_defs.md#predefinedattributevaluesoutputtypedef) 
## CreateQuickConnectRequestTypeDef

```python
# CreateQuickConnectRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateQuickConnectRequestTypeDef


def get_value() -> CreateQuickConnectRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateQuickConnectRequestTypeDef definition

class CreateQuickConnectRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    QuickConnectConfig: QuickConnectConfigTypeDef,  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: QuickConnectConfigTypeDef](./type_defs.md#quickconnectconfigtypedef) 
## QuickConnectTypeDef

```python
# QuickConnectTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import QuickConnectTypeDef


def get_value() -> QuickConnectTypeDef:
    return {
        "QuickConnectARN": ...,
    }


# QuickConnectTypeDef definition

class QuickConnectTypeDef(TypedDict):
    QuickConnectARN: NotRequired[str],
    QuickConnectId: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    QuickConnectConfig: NotRequired[QuickConnectConfigTypeDef],  # (1)
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-braces: QuickConnectConfigTypeDef](./type_defs.md#quickconnectconfigtypedef) 
## UpdateQuickConnectConfigRequestTypeDef

```python
# UpdateQuickConnectConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateQuickConnectConfigRequestTypeDef


def get_value() -> UpdateQuickConnectConfigRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateQuickConnectConfigRequestTypeDef definition

class UpdateQuickConnectConfigRequestTypeDef(TypedDict):
    InstanceId: str,
    QuickConnectId: str,
    QuickConnectConfig: QuickConnectConfigTypeDef,  # (1)
```

1. See [:material-code-braces: QuickConnectConfigTypeDef](./type_defs.md#quickconnectconfigtypedef) 
## RealTimeContactAnalysisSegmentTranscriptTypeDef

```python
# RealTimeContactAnalysisSegmentTranscriptTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisSegmentTranscriptTypeDef


def get_value() -> RealTimeContactAnalysisSegmentTranscriptTypeDef:
    return {
        "Id": ...,
    }


# RealTimeContactAnalysisSegmentTranscriptTypeDef definition

class RealTimeContactAnalysisSegmentTranscriptTypeDef(TypedDict):
    Id: str,
    ParticipantId: str,
    ParticipantRole: ParticipantRoleType,  # (1)
    Content: str,
    Time: RealTimeContactAnalysisTimeDataTypeDef,  # (2)
    DisplayName: NotRequired[str],
    ContentType: NotRequired[str],
    Redaction: NotRequired[RealTimeContactAnalysisTranscriptItemRedactionTypeDef],  # (3)
    Sentiment: NotRequired[RealTimeContactAnalysisSentimentLabelType],  # (4)
```

1. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
2. See [:material-code-braces: RealTimeContactAnalysisTimeDataTypeDef](./type_defs.md#realtimecontactanalysistimedatatypedef) 
3. See [:material-code-braces: RealTimeContactAnalysisTranscriptItemRedactionTypeDef](./type_defs.md#realtimecontactanalysistranscriptitemredactiontypedef) 
4. See [:material-code-brackets: RealTimeContactAnalysisSentimentLabelType](./literals.md#realtimecontactanalysissentimentlabeltype) 
## RealTimeContactAnalysisPointOfInterestTypeDef

```python
# RealTimeContactAnalysisPointOfInterestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisPointOfInterestTypeDef


def get_value() -> RealTimeContactAnalysisPointOfInterestTypeDef:
    return {
        "TranscriptItems": ...,
    }


# RealTimeContactAnalysisPointOfInterestTypeDef definition

class RealTimeContactAnalysisPointOfInterestTypeDef(TypedDict):
    TranscriptItems: NotRequired[List[RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef]],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef](./type_defs.md#realtimecontactanalysistranscriptitemwithcharacteroffsetstypedef) 
## RealTimeContactAnalysisIssueDetectedTypeDef

```python
# RealTimeContactAnalysisIssueDetectedTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisIssueDetectedTypeDef


def get_value() -> RealTimeContactAnalysisIssueDetectedTypeDef:
    return {
        "TranscriptItems": ...,
    }


# RealTimeContactAnalysisIssueDetectedTypeDef definition

class RealTimeContactAnalysisIssueDetectedTypeDef(TypedDict):
    TranscriptItems: List[RealTimeContactAnalysisTranscriptItemWithContentTypeDef],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisTranscriptItemWithContentTypeDef](./type_defs.md#realtimecontactanalysistranscriptitemwithcontenttypedef) 
## ListContactReferencesResponseTypeDef

```python
# ListContactReferencesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListContactReferencesResponseTypeDef


def get_value() -> ListContactReferencesResponseTypeDef:
    return {
        "ReferenceSummaryList": ...,
    }


# ListContactReferencesResponseTypeDef definition

class ListContactReferencesResponseTypeDef(TypedDict):
    ReferenceSummaryList: List[ReferenceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReferenceSummaryTypeDef](./type_defs.md#referencesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInstanceResponseTypeDef

```python
# DescribeInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeInstanceResponseTypeDef


def get_value() -> DescribeInstanceResponseTypeDef:
    return {
        "Instance": ...,
    }


# DescribeInstanceResponseTypeDef definition

class DescribeInstanceResponseTypeDef(TypedDict):
    Instance: InstanceTypeDef,  # (1)
    ReplicationConfiguration: ReplicationConfigurationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchResourceTagsRequestPaginateTypeDef

```python
# SearchResourceTagsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchResourceTagsRequestPaginateTypeDef


def get_value() -> SearchResourceTagsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchResourceTagsRequestPaginateTypeDef definition

class SearchResourceTagsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    ResourceTypes: NotRequired[Sequence[str]],
    SearchCriteria: NotRequired[ResourceTagsSearchCriteriaTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceTagsSearchCriteriaTypeDef](./type_defs.md#resourcetagssearchcriteriatypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchResourceTagsRequestTypeDef

```python
# SearchResourceTagsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchResourceTagsRequestTypeDef


def get_value() -> SearchResourceTagsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchResourceTagsRequestTypeDef definition

class SearchResourceTagsRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceTypes: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchCriteria: NotRequired[ResourceTagsSearchCriteriaTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceTagsSearchCriteriaTypeDef](./type_defs.md#resourcetagssearchcriteriatypedef) 
## CreateContactRequestTypeDef

```python
# CreateContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateContactRequestTypeDef


def get_value() -> CreateContactRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateContactRequestTypeDef definition

class CreateContactRequestTypeDef(TypedDict):
    InstanceId: str,
    Channel: ChannelType,  # (1)
    InitiationMethod: ContactInitiationMethodType,  # (2)
    ClientToken: NotRequired[str],
    RelatedContactId: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
    References: NotRequired[Mapping[str, ReferenceTypeDef]],  # (3)
    ExpiryDurationInMinutes: NotRequired[int],
    UserInfo: NotRequired[UserInfoTypeDef],  # (4)
    InitiateAs: NotRequired[InitiateAsType],  # (5)
    Name: NotRequired[str],
    Description: NotRequired[str],
    SegmentAttributes: NotRequired[Mapping[str, SegmentAttributeValueUnionTypeDef]],  # (6)
```

1. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
2. See [:material-code-brackets: ContactInitiationMethodType](./literals.md#contactinitiationmethodtype) 
3. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
4. See [:material-code-braces: UserInfoTypeDef](./type_defs.md#userinfotypedef) 
5. See [:material-code-brackets: InitiateAsType](./literals.md#initiateastype) 
6. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) [:material-code-braces: SegmentAttributeValueOutputTypeDef](./type_defs.md#segmentattributevalueoutputtypedef) 
## StartChatContactRequestTypeDef

```python
# StartChatContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartChatContactRequestTypeDef


def get_value() -> StartChatContactRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# StartChatContactRequestTypeDef definition

class StartChatContactRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
    ParticipantDetails: ParticipantDetailsTypeDef,  # (1)
    Attributes: NotRequired[Mapping[str, str]],
    InitialMessage: NotRequired[ChatMessageTypeDef],  # (2)
    ClientToken: NotRequired[str],
    ChatDurationInMinutes: NotRequired[int],
    SupportedMessagingContentTypes: NotRequired[Sequence[str]],
    PersistentChat: NotRequired[PersistentChatTypeDef],  # (3)
    RelatedContactId: NotRequired[str],
    SegmentAttributes: NotRequired[Mapping[str, SegmentAttributeValueUnionTypeDef]],  # (4)
    CustomerId: NotRequired[str],
```

1. See [:material-code-braces: ParticipantDetailsTypeDef](./type_defs.md#participantdetailstypedef) 
2. See [:material-code-braces: ChatMessageTypeDef](./type_defs.md#chatmessagetypedef) 
3. See [:material-code-braces: PersistentChatTypeDef](./type_defs.md#persistentchattypedef) 
4. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) [:material-code-braces: SegmentAttributeValueOutputTypeDef](./type_defs.md#segmentattributevalueoutputtypedef) 
## StartEmailContactRequestTypeDef

```python
# StartEmailContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartEmailContactRequestTypeDef


def get_value() -> StartEmailContactRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# StartEmailContactRequestTypeDef definition

class StartEmailContactRequestTypeDef(TypedDict):
    InstanceId: str,
    FromEmailAddress: EmailAddressInfoTypeDef,  # (1)
    DestinationEmailAddress: str,
    EmailMessage: InboundEmailContentTypeDef,  # (2)
    Description: NotRequired[str],
    References: NotRequired[Mapping[str, ReferenceTypeDef]],  # (3)
    Name: NotRequired[str],
    AdditionalRecipients: NotRequired[InboundAdditionalRecipientsTypeDef],  # (4)
    Attachments: NotRequired[Sequence[EmailAttachmentTypeDef]],  # (5)
    ContactFlowId: NotRequired[str],
    RelatedContactId: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
    SegmentAttributes: NotRequired[Mapping[str, SegmentAttributeValueUnionTypeDef]],  # (6)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: EmailAddressInfoTypeDef](./type_defs.md#emailaddressinfotypedef) 
2. See [:material-code-braces: InboundEmailContentTypeDef](./type_defs.md#inboundemailcontenttypedef) 
3. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
4. See [:material-code-braces: InboundAdditionalRecipientsTypeDef](./type_defs.md#inboundadditionalrecipientstypedef) 
5. See [:material-code-braces: EmailAttachmentTypeDef](./type_defs.md#emailattachmenttypedef) 
6. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) [:material-code-braces: SegmentAttributeValueOutputTypeDef](./type_defs.md#segmentattributevalueoutputtypedef) 
## StartOutboundChatContactRequestTypeDef

```python
# StartOutboundChatContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartOutboundChatContactRequestTypeDef


def get_value() -> StartOutboundChatContactRequestTypeDef:
    return {
        "SourceEndpoint": ...,
    }


# StartOutboundChatContactRequestTypeDef definition

class StartOutboundChatContactRequestTypeDef(TypedDict):
    SourceEndpoint: EndpointTypeDef,  # (1)
    DestinationEndpoint: EndpointTypeDef,  # (1)
    InstanceId: str,
    SegmentAttributes: Mapping[str, SegmentAttributeValueUnionTypeDef],  # (3)
    ContactFlowId: str,
    Attributes: NotRequired[Mapping[str, str]],
    ChatDurationInMinutes: NotRequired[int],
    ParticipantDetails: NotRequired[ParticipantDetailsTypeDef],  # (4)
    InitialSystemMessage: NotRequired[ChatMessageTypeDef],  # (5)
    RelatedContactId: NotRequired[str],
    SupportedMessagingContentTypes: NotRequired[Sequence[str]],
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
3. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) [:material-code-braces: SegmentAttributeValueOutputTypeDef](./type_defs.md#segmentattributevalueoutputtypedef) 
4. See [:material-code-braces: ParticipantDetailsTypeDef](./type_defs.md#participantdetailstypedef) 
5. See [:material-code-braces: ChatMessageTypeDef](./type_defs.md#chatmessagetypedef) 
## StartTaskContactRequestTypeDef

```python
# StartTaskContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartTaskContactRequestTypeDef


def get_value() -> StartTaskContactRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# StartTaskContactRequestTypeDef definition

class StartTaskContactRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    PreviousContactId: NotRequired[str],
    ContactFlowId: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
    References: NotRequired[Mapping[str, ReferenceTypeDef]],  # (1)
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
    ScheduledTime: NotRequired[TimestampTypeDef],
    TaskTemplateId: NotRequired[str],
    QuickConnectId: NotRequired[str],
    RelatedContactId: NotRequired[str],
    SegmentAttributes: NotRequired[Mapping[str, SegmentAttributeValueUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
2. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) [:material-code-braces: SegmentAttributeValueOutputTypeDef](./type_defs.md#segmentattributevalueoutputtypedef) 
## UpdateContactRequestTypeDef

```python
# UpdateContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateContactRequestTypeDef


def get_value() -> UpdateContactRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateContactRequestTypeDef definition

class UpdateContactRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    References: NotRequired[Mapping[str, ReferenceTypeDef]],  # (1)
    SegmentAttributes: NotRequired[Mapping[str, SegmentAttributeValueUnionTypeDef]],  # (2)
    QueueInfo: NotRequired[QueueInfoInputTypeDef],  # (3)
    UserInfo: NotRequired[UserInfoTypeDef],  # (4)
    CustomerEndpoint: NotRequired[EndpointTypeDef],  # (5)
    SystemEndpoint: NotRequired[EndpointTypeDef],  # (5)
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
2. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) [:material-code-braces: SegmentAttributeValueOutputTypeDef](./type_defs.md#segmentattributevalueoutputtypedef) 
3. See [:material-code-braces: QueueInfoInputTypeDef](./type_defs.md#queueinfoinputtypedef) 
4. See [:material-code-braces: UserInfoTypeDef](./type_defs.md#userinfotypedef) 
5. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
6. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
## GetTrafficDistributionResponseTypeDef

```python
# GetTrafficDistributionResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetTrafficDistributionResponseTypeDef


def get_value() -> GetTrafficDistributionResponseTypeDef:
    return {
        "TelephonyConfig": ...,
    }


# GetTrafficDistributionResponseTypeDef definition

class GetTrafficDistributionResponseTypeDef(TypedDict):
    TelephonyConfig: TelephonyConfigOutputTypeDef,  # (1)
    Id: str,
    Arn: str,
    SignInConfig: SignInConfigOutputTypeDef,  # (2)
    AgentConfig: AgentConfigOutputTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TelephonyConfigOutputTypeDef](./type_defs.md#telephonyconfigoutputtypedef) 
2. See [:material-code-braces: SignInConfigOutputTypeDef](./type_defs.md#signinconfigoutputtypedef) 
3. See [:material-code-braces: AgentConfigOutputTypeDef](./type_defs.md#agentconfigoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OutboundEmailContentTypeDef

```python
# OutboundEmailContentTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import OutboundEmailContentTypeDef


def get_value() -> OutboundEmailContentTypeDef:
    return {
        "MessageSourceType": ...,
    }


# OutboundEmailContentTypeDef definition

class OutboundEmailContentTypeDef(TypedDict):
    MessageSourceType: OutboundMessageSourceTypeType,  # (1)
    TemplatedMessageConfig: NotRequired[TemplatedMessageConfigTypeDef],  # (2)
    RawMessage: NotRequired[OutboundRawMessageTypeDef],  # (3)
```

1. See [:material-code-brackets: OutboundMessageSourceTypeType](./literals.md#outboundmessagesourcetypetype) 
2. See [:material-code-braces: TemplatedMessageConfigTypeDef](./type_defs.md#templatedmessageconfigtypedef) 
3. See [:material-code-braces: OutboundRawMessageTypeDef](./type_defs.md#outboundrawmessagetypedef) 
## ContactAnalysisTypeDef

```python
# ContactAnalysisTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactAnalysisTypeDef


def get_value() -> ContactAnalysisTypeDef:
    return {
        "Transcript": ...,
    }


# ContactAnalysisTypeDef definition

class ContactAnalysisTypeDef(TypedDict):
    Transcript: NotRequired[TranscriptTypeDef],  # (1)
```

1. See [:material-code-braces: TranscriptTypeDef](./type_defs.md#transcripttypedef) 
## SearchUsersResponseTypeDef

```python
# SearchUsersResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchUsersResponseTypeDef


def get_value() -> SearchUsersResponseTypeDef:
    return {
        "Users": ...,
    }


# SearchUsersResponseTypeDef definition

class SearchUsersResponseTypeDef(TypedDict):
    Users: List[UserSearchSummaryTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserSearchSummaryTypeDef](./type_defs.md#usersearchsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateViewResponseTypeDef

```python
# CreateViewResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateViewResponseTypeDef


def get_value() -> CreateViewResponseTypeDef:
    return {
        "View": ...,
    }


# CreateViewResponseTypeDef definition

class CreateViewResponseTypeDef(TypedDict):
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateViewVersionResponseTypeDef

```python
# CreateViewVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateViewVersionResponseTypeDef


def get_value() -> CreateViewVersionResponseTypeDef:
    return {
        "View": ...,
    }


# CreateViewVersionResponseTypeDef definition

class CreateViewVersionResponseTypeDef(TypedDict):
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeViewResponseTypeDef

```python
# DescribeViewResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeViewResponseTypeDef


def get_value() -> DescribeViewResponseTypeDef:
    return {
        "View": ...,
    }


# DescribeViewResponseTypeDef definition

class DescribeViewResponseTypeDef(TypedDict):
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateViewContentResponseTypeDef

```python
# UpdateViewContentResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateViewContentResponseTypeDef


def get_value() -> UpdateViewContentResponseTypeDef:
    return {
        "View": ...,
    }


# UpdateViewContentResponseTypeDef definition

class UpdateViewContentResponseTypeDef(TypedDict):
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExpressionOutputTypeDef

```python
# ExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ExpressionOutputTypeDef


def get_value() -> ExpressionOutputTypeDef:
    return {
        "AttributeCondition": ...,
    }


# ExpressionOutputTypeDef definition

class ExpressionOutputTypeDef(TypedDict):
    AttributeCondition: NotRequired[AttributeConditionOutputTypeDef],  # (1)
    AndExpression: NotRequired[List[Dict[str, Any]]],
    OrExpression: NotRequired[List[Dict[str, Any]]],
    NotAttributeCondition: NotRequired[AttributeConditionOutputTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeConditionOutputTypeDef](./type_defs.md#attributeconditionoutputtypedef) 
2. See [:material-code-braces: AttributeConditionOutputTypeDef](./type_defs.md#attributeconditionoutputtypedef) 
## UserSearchFilterTypeDef

```python
# UserSearchFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserSearchFilterTypeDef


def get_value() -> UserSearchFilterTypeDef:
    return {
        "TagFilter": ...,
    }


# UserSearchFilterTypeDef definition

class UserSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
    UserAttributeFilter: NotRequired[ControlPlaneUserAttributeFilterTypeDef],  # (2)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
2. See [:material-code-braces: ControlPlaneUserAttributeFilterTypeDef](./type_defs.md#controlplaneuserattributefiltertypedef) 
## AgentStatusSearchFilterTypeDef

```python
# AgentStatusSearchFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AgentStatusSearchFilterTypeDef


def get_value() -> AgentStatusSearchFilterTypeDef:
    return {
        "AttributeFilter": ...,
    }


# AgentStatusSearchFilterTypeDef definition

class AgentStatusSearchFilterTypeDef(TypedDict):
    AttributeFilter: NotRequired[ControlPlaneAttributeFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneAttributeFilterTypeDef](./type_defs.md#controlplaneattributefiltertypedef) 
## UserHierarchyGroupSearchFilterTypeDef

```python
# UserHierarchyGroupSearchFilterTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserHierarchyGroupSearchFilterTypeDef


def get_value() -> UserHierarchyGroupSearchFilterTypeDef:
    return {
        "AttributeFilter": ...,
    }


# UserHierarchyGroupSearchFilterTypeDef definition

class UserHierarchyGroupSearchFilterTypeDef(TypedDict):
    AttributeFilter: NotRequired[ControlPlaneAttributeFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneAttributeFilterTypeDef](./type_defs.md#controlplaneattributefiltertypedef) 
## SearchContactFlowModulesRequestPaginateTypeDef

```python
# SearchContactFlowModulesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchContactFlowModulesRequestPaginateTypeDef


def get_value() -> SearchContactFlowModulesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchContactFlowModulesRequestPaginateTypeDef definition

class SearchContactFlowModulesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[ContactFlowModuleSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[ContactFlowModuleSearchCriteriaPaginatorTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ContactFlowModuleSearchFilterTypeDef](./type_defs.md#contactflowmodulesearchfiltertypedef) 
2. See [:material-code-braces: ContactFlowModuleSearchCriteriaPaginatorTypeDef](./type_defs.md#contactflowmodulesearchcriteriapaginatortypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchContactFlowModulesRequestTypeDef

```python
# SearchContactFlowModulesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchContactFlowModulesRequestTypeDef


def get_value() -> SearchContactFlowModulesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchContactFlowModulesRequestTypeDef definition

class SearchContactFlowModulesRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[ContactFlowModuleSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[ContactFlowModuleSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: ContactFlowModuleSearchFilterTypeDef](./type_defs.md#contactflowmodulesearchfiltertypedef) 
2. See [:material-code-braces: ContactFlowModuleSearchCriteriaTypeDef](./type_defs.md#contactflowmodulesearchcriteriatypedef) 
## SearchContactFlowsRequestPaginateTypeDef

```python
# SearchContactFlowsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchContactFlowsRequestPaginateTypeDef


def get_value() -> SearchContactFlowsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchContactFlowsRequestPaginateTypeDef definition

class SearchContactFlowsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[ContactFlowSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[ContactFlowSearchCriteriaPaginatorTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ContactFlowSearchFilterTypeDef](./type_defs.md#contactflowsearchfiltertypedef) 
2. See [:material-code-braces: ContactFlowSearchCriteriaPaginatorTypeDef](./type_defs.md#contactflowsearchcriteriapaginatortypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchContactFlowsRequestTypeDef

```python
# SearchContactFlowsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchContactFlowsRequestTypeDef


def get_value() -> SearchContactFlowsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchContactFlowsRequestTypeDef definition

class SearchContactFlowsRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[ContactFlowSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[ContactFlowSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: ContactFlowSearchFilterTypeDef](./type_defs.md#contactflowsearchfiltertypedef) 
2. See [:material-code-braces: ContactFlowSearchCriteriaTypeDef](./type_defs.md#contactflowsearchcriteriatypedef) 
## SearchEmailAddressesRequestTypeDef

```python
# SearchEmailAddressesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchEmailAddressesRequestTypeDef


def get_value() -> SearchEmailAddressesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchEmailAddressesRequestTypeDef definition

class SearchEmailAddressesRequestTypeDef(TypedDict):
    InstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SearchCriteria: NotRequired[EmailAddressSearchCriteriaTypeDef],  # (1)
    SearchFilter: NotRequired[EmailAddressSearchFilterTypeDef],  # (2)
```

1. See [:material-code-braces: EmailAddressSearchCriteriaTypeDef](./type_defs.md#emailaddresssearchcriteriatypedef) 
2. See [:material-code-braces: EmailAddressSearchFilterTypeDef](./type_defs.md#emailaddresssearchfiltertypedef) 
## SearchHoursOfOperationOverridesRequestPaginateTypeDef

```python
# SearchHoursOfOperationOverridesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchHoursOfOperationOverridesRequestPaginateTypeDef


def get_value() -> SearchHoursOfOperationOverridesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchHoursOfOperationOverridesRequestPaginateTypeDef definition

class SearchHoursOfOperationOverridesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[HoursOfOperationSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[HoursOfOperationOverrideSearchCriteriaPaginatorTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: HoursOfOperationSearchFilterTypeDef](./type_defs.md#hoursofoperationsearchfiltertypedef) 
2. See [:material-code-braces: HoursOfOperationOverrideSearchCriteriaPaginatorTypeDef](./type_defs.md#hoursofoperationoverridesearchcriteriapaginatortypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchHoursOfOperationOverridesRequestTypeDef

```python
# SearchHoursOfOperationOverridesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchHoursOfOperationOverridesRequestTypeDef


def get_value() -> SearchHoursOfOperationOverridesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchHoursOfOperationOverridesRequestTypeDef definition

class SearchHoursOfOperationOverridesRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[HoursOfOperationSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[HoursOfOperationOverrideSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: HoursOfOperationSearchFilterTypeDef](./type_defs.md#hoursofoperationsearchfiltertypedef) 
2. See [:material-code-braces: HoursOfOperationOverrideSearchCriteriaTypeDef](./type_defs.md#hoursofoperationoverridesearchcriteriatypedef) 
## SearchHoursOfOperationsRequestPaginateTypeDef

```python
# SearchHoursOfOperationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchHoursOfOperationsRequestPaginateTypeDef


def get_value() -> SearchHoursOfOperationsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchHoursOfOperationsRequestPaginateTypeDef definition

class SearchHoursOfOperationsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[HoursOfOperationSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[HoursOfOperationSearchCriteriaPaginatorTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: HoursOfOperationSearchFilterTypeDef](./type_defs.md#hoursofoperationsearchfiltertypedef) 
2. See [:material-code-braces: HoursOfOperationSearchCriteriaPaginatorTypeDef](./type_defs.md#hoursofoperationsearchcriteriapaginatortypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchHoursOfOperationsRequestTypeDef

```python
# SearchHoursOfOperationsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchHoursOfOperationsRequestTypeDef


def get_value() -> SearchHoursOfOperationsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchHoursOfOperationsRequestTypeDef definition

class SearchHoursOfOperationsRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[HoursOfOperationSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[HoursOfOperationSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: HoursOfOperationSearchFilterTypeDef](./type_defs.md#hoursofoperationsearchfiltertypedef) 
2. See [:material-code-braces: HoursOfOperationSearchCriteriaTypeDef](./type_defs.md#hoursofoperationsearchcriteriatypedef) 
## SearchPromptsRequestPaginateTypeDef

```python
# SearchPromptsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchPromptsRequestPaginateTypeDef


def get_value() -> SearchPromptsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchPromptsRequestPaginateTypeDef definition

class SearchPromptsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[PromptSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[PromptSearchCriteriaPaginatorTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: PromptSearchFilterTypeDef](./type_defs.md#promptsearchfiltertypedef) 
2. See [:material-code-braces: PromptSearchCriteriaPaginatorTypeDef](./type_defs.md#promptsearchcriteriapaginatortypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchPromptsRequestTypeDef

```python
# SearchPromptsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchPromptsRequestTypeDef


def get_value() -> SearchPromptsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchPromptsRequestTypeDef definition

class SearchPromptsRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[PromptSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[PromptSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: PromptSearchFilterTypeDef](./type_defs.md#promptsearchfiltertypedef) 
2. See [:material-code-braces: PromptSearchCriteriaTypeDef](./type_defs.md#promptsearchcriteriatypedef) 
## SearchQueuesRequestPaginateTypeDef

```python
# SearchQueuesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchQueuesRequestPaginateTypeDef


def get_value() -> SearchQueuesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchQueuesRequestPaginateTypeDef definition

class SearchQueuesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[QueueSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[QueueSearchCriteriaPaginatorTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: QueueSearchFilterTypeDef](./type_defs.md#queuesearchfiltertypedef) 
2. See [:material-code-braces: QueueSearchCriteriaPaginatorTypeDef](./type_defs.md#queuesearchcriteriapaginatortypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchQueuesRequestTypeDef

```python
# SearchQueuesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchQueuesRequestTypeDef


def get_value() -> SearchQueuesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchQueuesRequestTypeDef definition

class SearchQueuesRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[QueueSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[QueueSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: QueueSearchFilterTypeDef](./type_defs.md#queuesearchfiltertypedef) 
2. See [:material-code-braces: QueueSearchCriteriaTypeDef](./type_defs.md#queuesearchcriteriatypedef) 
## SearchQuickConnectsRequestPaginateTypeDef

```python
# SearchQuickConnectsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchQuickConnectsRequestPaginateTypeDef


def get_value() -> SearchQuickConnectsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchQuickConnectsRequestPaginateTypeDef definition

class SearchQuickConnectsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[QuickConnectSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[QuickConnectSearchCriteriaPaginatorTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: QuickConnectSearchFilterTypeDef](./type_defs.md#quickconnectsearchfiltertypedef) 
2. See [:material-code-braces: QuickConnectSearchCriteriaPaginatorTypeDef](./type_defs.md#quickconnectsearchcriteriapaginatortypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchQuickConnectsRequestTypeDef

```python
# SearchQuickConnectsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchQuickConnectsRequestTypeDef


def get_value() -> SearchQuickConnectsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchQuickConnectsRequestTypeDef definition

class SearchQuickConnectsRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[QuickConnectSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[QuickConnectSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: QuickConnectSearchFilterTypeDef](./type_defs.md#quickconnectsearchfiltertypedef) 
2. See [:material-code-braces: QuickConnectSearchCriteriaTypeDef](./type_defs.md#quickconnectsearchcriteriatypedef) 
## SearchRoutingProfilesRequestPaginateTypeDef

```python
# SearchRoutingProfilesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchRoutingProfilesRequestPaginateTypeDef


def get_value() -> SearchRoutingProfilesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchRoutingProfilesRequestPaginateTypeDef definition

class SearchRoutingProfilesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[RoutingProfileSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[RoutingProfileSearchCriteriaPaginatorTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: RoutingProfileSearchFilterTypeDef](./type_defs.md#routingprofilesearchfiltertypedef) 
2. See [:material-code-braces: RoutingProfileSearchCriteriaPaginatorTypeDef](./type_defs.md#routingprofilesearchcriteriapaginatortypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchRoutingProfilesRequestTypeDef

```python
# SearchRoutingProfilesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchRoutingProfilesRequestTypeDef


def get_value() -> SearchRoutingProfilesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchRoutingProfilesRequestTypeDef definition

class SearchRoutingProfilesRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[RoutingProfileSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[RoutingProfileSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: RoutingProfileSearchFilterTypeDef](./type_defs.md#routingprofilesearchfiltertypedef) 
2. See [:material-code-braces: RoutingProfileSearchCriteriaTypeDef](./type_defs.md#routingprofilesearchcriteriatypedef) 
## SearchSecurityProfilesRequestPaginateTypeDef

```python
# SearchSecurityProfilesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchSecurityProfilesRequestPaginateTypeDef


def get_value() -> SearchSecurityProfilesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchSecurityProfilesRequestPaginateTypeDef definition

class SearchSecurityProfilesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchCriteria: NotRequired[SecurityProfileSearchCriteriaPaginatorTypeDef],  # (1)
    SearchFilter: NotRequired[SecurityProfilesSearchFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: SecurityProfileSearchCriteriaPaginatorTypeDef](./type_defs.md#securityprofilesearchcriteriapaginatortypedef) 
2. See [:material-code-braces: SecurityProfilesSearchFilterTypeDef](./type_defs.md#securityprofilessearchfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchSecurityProfilesRequestTypeDef

```python
# SearchSecurityProfilesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchSecurityProfilesRequestTypeDef


def get_value() -> SearchSecurityProfilesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchSecurityProfilesRequestTypeDef definition

class SearchSecurityProfilesRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchCriteria: NotRequired[SecurityProfileSearchCriteriaTypeDef],  # (1)
    SearchFilter: NotRequired[SecurityProfilesSearchFilterTypeDef],  # (2)
```

1. See [:material-code-braces: SecurityProfileSearchCriteriaTypeDef](./type_defs.md#securityprofilesearchcriteriatypedef) 
2. See [:material-code-braces: SecurityProfilesSearchFilterTypeDef](./type_defs.md#securityprofilessearchfiltertypedef) 
## ConnectionDataTypeDef

```python
# ConnectionDataTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ConnectionDataTypeDef


def get_value() -> ConnectionDataTypeDef:
    return {
        "Attendee": ...,
    }


# ConnectionDataTypeDef definition

class ConnectionDataTypeDef(TypedDict):
    Attendee: NotRequired[AttendeeTypeDef],  # (1)
    Meeting: NotRequired[MeetingTypeDef],  # (2)
```

1. See [:material-code-braces: AttendeeTypeDef](./type_defs.md#attendeetypedef) 
2. See [:material-code-braces: MeetingTypeDef](./type_defs.md#meetingtypedef) 
## UserSearchCriteriaPaginatorTypeDef

```python
# UserSearchCriteriaPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserSearchCriteriaPaginatorTypeDef


def get_value() -> UserSearchCriteriaPaginatorTypeDef:
    return {
        "OrConditions": ...,
    }


# UserSearchCriteriaPaginatorTypeDef definition

class UserSearchCriteriaPaginatorTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
    ListCondition: NotRequired[ListConditionTypeDef],  # (2)
    HierarchyGroupCondition: NotRequired[HierarchyGroupConditionTypeDef],  # (3)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-braces: ListConditionTypeDef](./type_defs.md#listconditiontypedef) 
3. See [:material-code-braces: HierarchyGroupConditionTypeDef](./type_defs.md#hierarchygroupconditiontypedef) 
## UserSearchCriteriaTypeDef

```python
# UserSearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UserSearchCriteriaTypeDef


def get_value() -> UserSearchCriteriaTypeDef:
    return {
        "OrConditions": ...,
    }


# UserSearchCriteriaTypeDef definition

class UserSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Mapping[str, Any]]],
    AndConditions: NotRequired[Sequence[Mapping[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
    ListCondition: NotRequired[ListConditionTypeDef],  # (2)
    HierarchyGroupCondition: NotRequired[HierarchyGroupConditionTypeDef],  # (3)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-braces: ListConditionTypeDef](./type_defs.md#listconditiontypedef) 
3. See [:material-code-braces: HierarchyGroupConditionTypeDef](./type_defs.md#hierarchygroupconditiontypedef) 
## DescribeRoutingProfileResponseTypeDef

```python
# DescribeRoutingProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeRoutingProfileResponseTypeDef


def get_value() -> DescribeRoutingProfileResponseTypeDef:
    return {
        "RoutingProfile": ...,
    }


# DescribeRoutingProfileResponseTypeDef definition

class DescribeRoutingProfileResponseTypeDef(TypedDict):
    RoutingProfile: RoutingProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoutingProfileTypeDef](./type_defs.md#routingprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchRoutingProfilesResponseTypeDef

```python
# SearchRoutingProfilesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchRoutingProfilesResponseTypeDef


def get_value() -> SearchRoutingProfilesResponseTypeDef:
    return {
        "RoutingProfiles": ...,
    }


# SearchRoutingProfilesResponseTypeDef definition

class SearchRoutingProfilesResponseTypeDef(TypedDict):
    RoutingProfiles: List[RoutingProfileTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RoutingProfileTypeDef](./type_defs.md#routingprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCurrentMetricDataResponseTypeDef

```python
# GetCurrentMetricDataResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetCurrentMetricDataResponseTypeDef


def get_value() -> GetCurrentMetricDataResponseTypeDef:
    return {
        "NextToken": ...,
    }


# GetCurrentMetricDataResponseTypeDef definition

class GetCurrentMetricDataResponseTypeDef(TypedDict):
    MetricResults: List[CurrentMetricResultTypeDef],  # (1)
    DataSnapshotTime: datetime,
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CurrentMetricResultTypeDef](./type_defs.md#currentmetricresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateInstanceStorageConfigRequestTypeDef

```python
# AssociateInstanceStorageConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AssociateInstanceStorageConfigRequestTypeDef


def get_value() -> AssociateInstanceStorageConfigRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# AssociateInstanceStorageConfigRequestTypeDef definition

class AssociateInstanceStorageConfigRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    StorageConfig: InstanceStorageConfigTypeDef,  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
2. See [:material-code-braces: InstanceStorageConfigTypeDef](./type_defs.md#instancestorageconfigtypedef) 
## DescribeInstanceStorageConfigResponseTypeDef

```python
# DescribeInstanceStorageConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeInstanceStorageConfigResponseTypeDef


def get_value() -> DescribeInstanceStorageConfigResponseTypeDef:
    return {
        "StorageConfig": ...,
    }


# DescribeInstanceStorageConfigResponseTypeDef definition

class DescribeInstanceStorageConfigResponseTypeDef(TypedDict):
    StorageConfig: InstanceStorageConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceStorageConfigTypeDef](./type_defs.md#instancestorageconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstanceStorageConfigsResponseTypeDef

```python
# ListInstanceStorageConfigsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListInstanceStorageConfigsResponseTypeDef


def get_value() -> ListInstanceStorageConfigsResponseTypeDef:
    return {
        "StorageConfigs": ...,
    }


# ListInstanceStorageConfigsResponseTypeDef definition

class ListInstanceStorageConfigsResponseTypeDef(TypedDict):
    StorageConfigs: List[InstanceStorageConfigTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceStorageConfigTypeDef](./type_defs.md#instancestorageconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInstanceStorageConfigRequestTypeDef

```python
# UpdateInstanceStorageConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateInstanceStorageConfigRequestTypeDef


def get_value() -> UpdateInstanceStorageConfigRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateInstanceStorageConfigRequestTypeDef definition

class UpdateInstanceStorageConfigRequestTypeDef(TypedDict):
    InstanceId: str,
    AssociationId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    StorageConfig: InstanceStorageConfigTypeDef,  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
2. See [:material-code-braces: InstanceStorageConfigTypeDef](./type_defs.md#instancestorageconfigtypedef) 
## EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef

```python
# EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef


def get_value() -> EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef:
    return {
        "Options": ...,
    }


# EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef definition

class EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef(TypedDict):
    Options: List[EvaluationFormSingleSelectQuestionOptionTypeDef],  # (1)
    DisplayAs: NotRequired[EvaluationFormSingleSelectQuestionDisplayModeType],  # (2)
    Automation: NotRequired[EvaluationFormSingleSelectQuestionAutomationOutputTypeDef],  # (3)
```

1. See [:material-code-braces: EvaluationFormSingleSelectQuestionOptionTypeDef](./type_defs.md#evaluationformsingleselectquestionoptiontypedef) 
2. See [:material-code-brackets: EvaluationFormSingleSelectQuestionDisplayModeType](./literals.md#evaluationformsingleselectquestiondisplaymodetype) 
3. See [:material-code-braces: EvaluationFormSingleSelectQuestionAutomationOutputTypeDef](./type_defs.md#evaluationformsingleselectquestionautomationoutputtypedef) 
## RuleActionOutputTypeDef

```python
# RuleActionOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RuleActionOutputTypeDef


def get_value() -> RuleActionOutputTypeDef:
    return {
        "ActionType": ...,
    }


# RuleActionOutputTypeDef definition

class RuleActionOutputTypeDef(TypedDict):
    ActionType: ActionTypeType,  # (1)
    TaskAction: NotRequired[TaskActionDefinitionOutputTypeDef],  # (2)
    EventBridgeAction: NotRequired[EventBridgeActionDefinitionTypeDef],  # (3)
    AssignContactCategoryAction: NotRequired[Dict[str, Any]],
    SendNotificationAction: NotRequired[SendNotificationActionDefinitionOutputTypeDef],  # (4)
    CreateCaseAction: NotRequired[CreateCaseActionDefinitionOutputTypeDef],  # (5)
    UpdateCaseAction: NotRequired[UpdateCaseActionDefinitionOutputTypeDef],  # (6)
    EndAssociatedTasksAction: NotRequired[Dict[str, Any]],
    SubmitAutoEvaluationAction: NotRequired[SubmitAutoEvaluationActionDefinitionTypeDef],  # (7)
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-braces: TaskActionDefinitionOutputTypeDef](./type_defs.md#taskactiondefinitionoutputtypedef) 
3. See [:material-code-braces: EventBridgeActionDefinitionTypeDef](./type_defs.md#eventbridgeactiondefinitiontypedef) 
4. See [:material-code-braces: SendNotificationActionDefinitionOutputTypeDef](./type_defs.md#sendnotificationactiondefinitionoutputtypedef) 
5. See [:material-code-braces: CreateCaseActionDefinitionOutputTypeDef](./type_defs.md#createcaseactiondefinitionoutputtypedef) 
6. See [:material-code-braces: UpdateCaseActionDefinitionOutputTypeDef](./type_defs.md#updatecaseactiondefinitionoutputtypedef) 
7. See [:material-code-braces: SubmitAutoEvaluationActionDefinitionTypeDef](./type_defs.md#submitautoevaluationactiondefinitiontypedef) 
## GetCurrentUserDataResponseTypeDef

```python
# GetCurrentUserDataResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetCurrentUserDataResponseTypeDef


def get_value() -> GetCurrentUserDataResponseTypeDef:
    return {
        "NextToken": ...,
    }


# GetCurrentUserDataResponseTypeDef definition

class GetCurrentUserDataResponseTypeDef(TypedDict):
    UserDataList: List[UserDataTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserDataTypeDef](./type_defs.md#userdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserHierarchyGroupResponseTypeDef

```python
# DescribeUserHierarchyGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeUserHierarchyGroupResponseTypeDef


def get_value() -> DescribeUserHierarchyGroupResponseTypeDef:
    return {
        "HierarchyGroup": ...,
    }


# DescribeUserHierarchyGroupResponseTypeDef definition

class DescribeUserHierarchyGroupResponseTypeDef(TypedDict):
    HierarchyGroup: HierarchyGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HierarchyGroupTypeDef](./type_defs.md#hierarchygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchUserHierarchyGroupsResponseTypeDef

```python
# SearchUserHierarchyGroupsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchUserHierarchyGroupsResponseTypeDef


def get_value() -> SearchUserHierarchyGroupsResponseTypeDef:
    return {
        "UserHierarchyGroups": ...,
    }


# SearchUserHierarchyGroupsResponseTypeDef definition

class SearchUserHierarchyGroupsResponseTypeDef(TypedDict):
    UserHierarchyGroups: List[HierarchyGroupTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HierarchyGroupTypeDef](./type_defs.md#hierarchygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HistoricalMetricResultTypeDef

```python
# HistoricalMetricResultTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import HistoricalMetricResultTypeDef


def get_value() -> HistoricalMetricResultTypeDef:
    return {
        "Dimensions": ...,
    }


# HistoricalMetricResultTypeDef definition

class HistoricalMetricResultTypeDef(TypedDict):
    Dimensions: NotRequired[DimensionsTypeDef],  # (1)
    Collections: NotRequired[List[HistoricalMetricDataTypeDef]],  # (2)
```

1. See [:material-code-braces: DimensionsTypeDef](./type_defs.md#dimensionstypedef) 
2. See [:material-code-braces: HistoricalMetricDataTypeDef](./type_defs.md#historicalmetricdatatypedef) 
## DescribeHoursOfOperationResponseTypeDef

```python
# DescribeHoursOfOperationResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeHoursOfOperationResponseTypeDef


def get_value() -> DescribeHoursOfOperationResponseTypeDef:
    return {
        "HoursOfOperation": ...,
    }


# DescribeHoursOfOperationResponseTypeDef definition

class DescribeHoursOfOperationResponseTypeDef(TypedDict):
    HoursOfOperation: HoursOfOperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HoursOfOperationTypeDef](./type_defs.md#hoursofoperationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchHoursOfOperationsResponseTypeDef

```python
# SearchHoursOfOperationsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchHoursOfOperationsResponseTypeDef


def get_value() -> SearchHoursOfOperationsResponseTypeDef:
    return {
        "HoursOfOperations": ...,
    }


# SearchHoursOfOperationsResponseTypeDef definition

class SearchHoursOfOperationsResponseTypeDef(TypedDict):
    HoursOfOperations: List[HoursOfOperationTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HoursOfOperationTypeDef](./type_defs.md#hoursofoperationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeHoursOfOperationOverrideResponseTypeDef

```python
# DescribeHoursOfOperationOverrideResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeHoursOfOperationOverrideResponseTypeDef


def get_value() -> DescribeHoursOfOperationOverrideResponseTypeDef:
    return {
        "HoursOfOperationOverride": ...,
    }


# DescribeHoursOfOperationOverrideResponseTypeDef definition

class DescribeHoursOfOperationOverrideResponseTypeDef(TypedDict):
    HoursOfOperationOverride: HoursOfOperationOverrideTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HoursOfOperationOverrideTypeDef](./type_defs.md#hoursofoperationoverridetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHoursOfOperationOverridesResponseTypeDef

```python
# ListHoursOfOperationOverridesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListHoursOfOperationOverridesResponseTypeDef


def get_value() -> ListHoursOfOperationOverridesResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListHoursOfOperationOverridesResponseTypeDef definition

class ListHoursOfOperationOverridesResponseTypeDef(TypedDict):
    HoursOfOperationOverrideList: List[HoursOfOperationOverrideTypeDef],  # (1)
    LastModifiedRegion: str,
    LastModifiedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HoursOfOperationOverrideTypeDef](./type_defs.md#hoursofoperationoverridetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchHoursOfOperationOverridesResponseTypeDef

```python
# SearchHoursOfOperationOverridesResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchHoursOfOperationOverridesResponseTypeDef


def get_value() -> SearchHoursOfOperationOverridesResponseTypeDef:
    return {
        "HoursOfOperationOverrides": ...,
    }


# SearchHoursOfOperationOverridesResponseTypeDef definition

class SearchHoursOfOperationOverridesResponseTypeDef(TypedDict):
    HoursOfOperationOverrides: List[HoursOfOperationOverrideTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HoursOfOperationOverrideTypeDef](./type_defs.md#hoursofoperationoverridetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEffectiveHoursOfOperationsResponseTypeDef

```python
# GetEffectiveHoursOfOperationsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetEffectiveHoursOfOperationsResponseTypeDef


def get_value() -> GetEffectiveHoursOfOperationsResponseTypeDef:
    return {
        "EffectiveHoursOfOperationList": ...,
    }


# GetEffectiveHoursOfOperationsResponseTypeDef definition

class GetEffectiveHoursOfOperationsResponseTypeDef(TypedDict):
    EffectiveHoursOfOperationList: List[EffectiveHoursOfOperationsTypeDef],  # (1)
    TimeZone: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EffectiveHoursOfOperationsTypeDef](./type_defs.md#effectivehoursofoperationstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTaskTemplateResponseTypeDef

```python
# GetTaskTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetTaskTemplateResponseTypeDef


def get_value() -> GetTaskTemplateResponseTypeDef:
    return {
        "InstanceId": ...,
    }


# GetTaskTemplateResponseTypeDef definition

class GetTaskTemplateResponseTypeDef(TypedDict):
    InstanceId: str,
    Id: str,
    Arn: str,
    Name: str,
    Description: str,
    ContactFlowId: str,
    SelfAssignFlowId: str,
    Constraints: TaskTemplateConstraintsOutputTypeDef,  # (1)
    Defaults: TaskTemplateDefaultsOutputTypeDef,  # (2)
    Fields: List[TaskTemplateFieldOutputTypeDef],  # (3)
    Status: TaskTemplateStatusType,  # (4)
    LastModifiedTime: datetime,
    CreatedTime: datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: TaskTemplateConstraintsOutputTypeDef](./type_defs.md#tasktemplateconstraintsoutputtypedef) 
2. See [:material-code-braces: TaskTemplateDefaultsOutputTypeDef](./type_defs.md#tasktemplatedefaultsoutputtypedef) 
3. See [:material-code-braces: TaskTemplateFieldOutputTypeDef](./type_defs.md#tasktemplatefieldoutputtypedef) 
4. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTaskTemplateResponseTypeDef

```python
# UpdateTaskTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateTaskTemplateResponseTypeDef


def get_value() -> UpdateTaskTemplateResponseTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateTaskTemplateResponseTypeDef definition

class UpdateTaskTemplateResponseTypeDef(TypedDict):
    InstanceId: str,
    Id: str,
    Arn: str,
    Name: str,
    Description: str,
    ContactFlowId: str,
    SelfAssignFlowId: str,
    Constraints: TaskTemplateConstraintsOutputTypeDef,  # (1)
    Defaults: TaskTemplateDefaultsOutputTypeDef,  # (2)
    Fields: List[TaskTemplateFieldOutputTypeDef],  # (3)
    Status: TaskTemplateStatusType,  # (4)
    LastModifiedTime: datetime,
    CreatedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: TaskTemplateConstraintsOutputTypeDef](./type_defs.md#tasktemplateconstraintsoutputtypedef) 
2. See [:material-code-braces: TaskTemplateDefaultsOutputTypeDef](./type_defs.md#tasktemplatedefaultsoutputtypedef) 
3. See [:material-code-braces: TaskTemplateFieldOutputTypeDef](./type_defs.md#tasktemplatefieldoutputtypedef) 
4. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricResultV2TypeDef

```python
# MetricResultV2TypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import MetricResultV2TypeDef


def get_value() -> MetricResultV2TypeDef:
    return {
        "Dimensions": ...,
    }


# MetricResultV2TypeDef definition

class MetricResultV2TypeDef(TypedDict):
    Dimensions: NotRequired[Dict[str, str]],
    MetricInterval: NotRequired[MetricIntervalTypeDef],  # (1)
    Collections: NotRequired[List[MetricDataV2TypeDef]],  # (2)
```

1. See [:material-code-braces: MetricIntervalTypeDef](./type_defs.md#metricintervaltypedef) 
2. See [:material-code-braces: MetricDataV2TypeDef](./type_defs.md#metricdatav2typedef) 
## UpdateParticipantRoleConfigChannelInfoTypeDef

```python
# UpdateParticipantRoleConfigChannelInfoTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateParticipantRoleConfigChannelInfoTypeDef


def get_value() -> UpdateParticipantRoleConfigChannelInfoTypeDef:
    return {
        "Chat": ...,
    }


# UpdateParticipantRoleConfigChannelInfoTypeDef definition

class UpdateParticipantRoleConfigChannelInfoTypeDef(TypedDict):
    Chat: NotRequired[ChatParticipantRoleConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ChatParticipantRoleConfigTypeDef](./type_defs.md#chatparticipantroleconfigtypedef) 
## DescribeQuickConnectResponseTypeDef

```python
# DescribeQuickConnectResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeQuickConnectResponseTypeDef


def get_value() -> DescribeQuickConnectResponseTypeDef:
    return {
        "QuickConnect": ...,
    }


# DescribeQuickConnectResponseTypeDef definition

class DescribeQuickConnectResponseTypeDef(TypedDict):
    QuickConnect: QuickConnectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QuickConnectTypeDef](./type_defs.md#quickconnecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchQuickConnectsResponseTypeDef

```python
# SearchQuickConnectsResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchQuickConnectsResponseTypeDef


def get_value() -> SearchQuickConnectsResponseTypeDef:
    return {
        "QuickConnects": ...,
    }


# SearchQuickConnectsResponseTypeDef definition

class SearchQuickConnectsResponseTypeDef(TypedDict):
    QuickConnects: List[QuickConnectTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QuickConnectTypeDef](./type_defs.md#quickconnecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RealTimeContactAnalysisCategoryDetailsTypeDef

```python
# RealTimeContactAnalysisCategoryDetailsTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisCategoryDetailsTypeDef


def get_value() -> RealTimeContactAnalysisCategoryDetailsTypeDef:
    return {
        "PointsOfInterest": ...,
    }


# RealTimeContactAnalysisCategoryDetailsTypeDef definition

class RealTimeContactAnalysisCategoryDetailsTypeDef(TypedDict):
    PointsOfInterest: List[RealTimeContactAnalysisPointOfInterestTypeDef],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisPointOfInterestTypeDef](./type_defs.md#realtimecontactanalysispointofinteresttypedef) 
## RealTimeContactAnalysisSegmentIssuesTypeDef

```python
# RealTimeContactAnalysisSegmentIssuesTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisSegmentIssuesTypeDef


def get_value() -> RealTimeContactAnalysisSegmentIssuesTypeDef:
    return {
        "IssuesDetected": ...,
    }


# RealTimeContactAnalysisSegmentIssuesTypeDef definition

class RealTimeContactAnalysisSegmentIssuesTypeDef(TypedDict):
    IssuesDetected: List[RealTimeContactAnalysisIssueDetectedTypeDef],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisIssueDetectedTypeDef](./type_defs.md#realtimecontactanalysisissuedetectedtypedef) 
## UpdateTrafficDistributionRequestTypeDef

```python
# UpdateTrafficDistributionRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateTrafficDistributionRequestTypeDef


def get_value() -> UpdateTrafficDistributionRequestTypeDef:
    return {
        "Id": ...,
    }


# UpdateTrafficDistributionRequestTypeDef definition

class UpdateTrafficDistributionRequestTypeDef(TypedDict):
    Id: str,
    TelephonyConfig: NotRequired[TelephonyConfigUnionTypeDef],  # (1)
    SignInConfig: NotRequired[SignInConfigUnionTypeDef],  # (2)
    AgentConfig: NotRequired[AgentConfigUnionTypeDef],  # (3)
```

1. See [:material-code-braces: TelephonyConfigTypeDef](./type_defs.md#telephonyconfigtypedef) [:material-code-braces: TelephonyConfigOutputTypeDef](./type_defs.md#telephonyconfigoutputtypedef) 
2. See [:material-code-braces: SignInConfigTypeDef](./type_defs.md#signinconfigtypedef) [:material-code-braces: SignInConfigOutputTypeDef](./type_defs.md#signinconfigoutputtypedef) 
3. See [:material-code-braces: AgentConfigTypeDef](./type_defs.md#agentconfigtypedef) [:material-code-braces: AgentConfigOutputTypeDef](./type_defs.md#agentconfigoutputtypedef) 
## SendOutboundEmailRequestTypeDef

```python
# SendOutboundEmailRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SendOutboundEmailRequestTypeDef


def get_value() -> SendOutboundEmailRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SendOutboundEmailRequestTypeDef definition

class SendOutboundEmailRequestTypeDef(TypedDict):
    InstanceId: str,
    FromEmailAddress: EmailAddressInfoTypeDef,  # (1)
    DestinationEmailAddress: EmailAddressInfoTypeDef,  # (1)
    EmailMessage: OutboundEmailContentTypeDef,  # (3)
    TrafficType: TrafficTypeType,  # (4)
    AdditionalRecipients: NotRequired[OutboundAdditionalRecipientsTypeDef],  # (5)
    SourceCampaign: NotRequired[SourceCampaignTypeDef],  # (6)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: EmailAddressInfoTypeDef](./type_defs.md#emailaddressinfotypedef) 
2. See [:material-code-braces: EmailAddressInfoTypeDef](./type_defs.md#emailaddressinfotypedef) 
3. See [:material-code-braces: OutboundEmailContentTypeDef](./type_defs.md#outboundemailcontenttypedef) 
4. See [:material-code-brackets: TrafficTypeType](./literals.md#traffictypetype) 
5. See [:material-code-braces: OutboundAdditionalRecipientsTypeDef](./type_defs.md#outboundadditionalrecipientstypedef) 
6. See [:material-code-braces: SourceCampaignTypeDef](./type_defs.md#sourcecampaigntypedef) 
## StartOutboundEmailContactRequestTypeDef

```python
# StartOutboundEmailContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartOutboundEmailContactRequestTypeDef


def get_value() -> StartOutboundEmailContactRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# StartOutboundEmailContactRequestTypeDef definition

class StartOutboundEmailContactRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    DestinationEmailAddress: EmailAddressInfoTypeDef,  # (1)
    EmailMessage: OutboundEmailContentTypeDef,  # (2)
    FromEmailAddress: NotRequired[EmailAddressInfoTypeDef],  # (1)
    AdditionalRecipients: NotRequired[OutboundAdditionalRecipientsTypeDef],  # (4)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: EmailAddressInfoTypeDef](./type_defs.md#emailaddressinfotypedef) 
2. See [:material-code-braces: OutboundEmailContentTypeDef](./type_defs.md#outboundemailcontenttypedef) 
3. See [:material-code-braces: EmailAddressInfoTypeDef](./type_defs.md#emailaddressinfotypedef) 
4. See [:material-code-braces: OutboundAdditionalRecipientsTypeDef](./type_defs.md#outboundadditionalrecipientstypedef) 
## SearchCriteriaTypeDef

```python
# SearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchCriteriaTypeDef


def get_value() -> SearchCriteriaTypeDef:
    return {
        "AgentIds": ...,
    }


# SearchCriteriaTypeDef definition

class SearchCriteriaTypeDef(TypedDict):
    AgentIds: NotRequired[Sequence[str]],
    AgentHierarchyGroups: NotRequired[AgentHierarchyGroupsTypeDef],  # (1)
    Channels: NotRequired[Sequence[ChannelType]],  # (2)
    ContactAnalysis: NotRequired[ContactAnalysisTypeDef],  # (3)
    InitiationMethods: NotRequired[Sequence[ContactInitiationMethodType]],  # (4)
    QueueIds: NotRequired[Sequence[str]],
    SearchableContactAttributes: NotRequired[SearchableContactAttributesTypeDef],  # (5)
    SearchableSegmentAttributes: NotRequired[SearchableSegmentAttributesTypeDef],  # (6)
```

1. See [:material-code-braces: AgentHierarchyGroupsTypeDef](./type_defs.md#agenthierarchygroupstypedef) 
2. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
3. See [:material-code-braces: ContactAnalysisTypeDef](./type_defs.md#contactanalysistypedef) 
4. See [:material-code-brackets: ContactInitiationMethodType](./literals.md#contactinitiationmethodtype) 
5. See [:material-code-braces: SearchableContactAttributesTypeDef](./type_defs.md#searchablecontactattributestypedef) 
6. See [:material-code-braces: SearchableSegmentAttributesTypeDef](./type_defs.md#searchablesegmentattributestypedef) 
## StepTypeDef

```python
# StepTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StepTypeDef


def get_value() -> StepTypeDef:
    return {
        "Expiry": ...,
    }


# StepTypeDef definition

class StepTypeDef(TypedDict):
    Expiry: NotRequired[ExpiryTypeDef],  # (1)
    Expression: NotRequired[ExpressionOutputTypeDef],  # (2)
    Status: NotRequired[RoutingCriteriaStepStatusType],  # (3)
```

1. See [:material-code-braces: ExpiryTypeDef](./type_defs.md#expirytypedef) 
2. See [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
3. See [:material-code-brackets: RoutingCriteriaStepStatusType](./literals.md#routingcriteriastepstatustype) 
## AttributeConditionTypeDef

```python
# AttributeConditionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import AttributeConditionTypeDef


def get_value() -> AttributeConditionTypeDef:
    return {
        "Name": ...,
    }


# AttributeConditionTypeDef definition

class AttributeConditionTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
    ProficiencyLevel: NotRequired[float],
    Range: NotRequired[RangeTypeDef],  # (1)
    MatchCriteria: NotRequired[MatchCriteriaUnionTypeDef],  # (2)
    ComparisonOperator: NotRequired[str],
```

1. See [:material-code-braces: RangeTypeDef](./type_defs.md#rangetypedef) 
2. See [:material-code-braces: MatchCriteriaTypeDef](./type_defs.md#matchcriteriatypedef) [:material-code-braces: MatchCriteriaOutputTypeDef](./type_defs.md#matchcriteriaoutputtypedef) 
## SearchAgentStatusesRequestPaginateTypeDef

```python
# SearchAgentStatusesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchAgentStatusesRequestPaginateTypeDef


def get_value() -> SearchAgentStatusesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchAgentStatusesRequestPaginateTypeDef definition

class SearchAgentStatusesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[AgentStatusSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[AgentStatusSearchCriteriaPaginatorTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: AgentStatusSearchFilterTypeDef](./type_defs.md#agentstatussearchfiltertypedef) 
2. See [:material-code-braces: AgentStatusSearchCriteriaPaginatorTypeDef](./type_defs.md#agentstatussearchcriteriapaginatortypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchAgentStatusesRequestTypeDef

```python
# SearchAgentStatusesRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchAgentStatusesRequestTypeDef


def get_value() -> SearchAgentStatusesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchAgentStatusesRequestTypeDef definition

class SearchAgentStatusesRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[AgentStatusSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[AgentStatusSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: AgentStatusSearchFilterTypeDef](./type_defs.md#agentstatussearchfiltertypedef) 
2. See [:material-code-braces: AgentStatusSearchCriteriaTypeDef](./type_defs.md#agentstatussearchcriteriatypedef) 
## SearchUserHierarchyGroupsRequestPaginateTypeDef

```python
# SearchUserHierarchyGroupsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchUserHierarchyGroupsRequestPaginateTypeDef


def get_value() -> SearchUserHierarchyGroupsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchUserHierarchyGroupsRequestPaginateTypeDef definition

class SearchUserHierarchyGroupsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[UserHierarchyGroupSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[UserHierarchyGroupSearchCriteriaPaginatorTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: UserHierarchyGroupSearchFilterTypeDef](./type_defs.md#userhierarchygroupsearchfiltertypedef) 
2. See [:material-code-braces: UserHierarchyGroupSearchCriteriaPaginatorTypeDef](./type_defs.md#userhierarchygroupsearchcriteriapaginatortypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchUserHierarchyGroupsRequestTypeDef

```python
# SearchUserHierarchyGroupsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchUserHierarchyGroupsRequestTypeDef


def get_value() -> SearchUserHierarchyGroupsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchUserHierarchyGroupsRequestTypeDef definition

class SearchUserHierarchyGroupsRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[UserHierarchyGroupSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[UserHierarchyGroupSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: UserHierarchyGroupSearchFilterTypeDef](./type_defs.md#userhierarchygroupsearchfiltertypedef) 
2. See [:material-code-braces: UserHierarchyGroupSearchCriteriaTypeDef](./type_defs.md#userhierarchygroupsearchcriteriatypedef) 
## StartWebRTCContactResponseTypeDef

```python
# StartWebRTCContactResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import StartWebRTCContactResponseTypeDef


def get_value() -> StartWebRTCContactResponseTypeDef:
    return {
        "ConnectionData": ...,
    }


# StartWebRTCContactResponseTypeDef definition

class StartWebRTCContactResponseTypeDef(TypedDict):
    ConnectionData: ConnectionDataTypeDef,  # (1)
    ContactId: str,
    ParticipantId: str,
    ParticipantToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionDataTypeDef](./type_defs.md#connectiondatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchUsersRequestPaginateTypeDef

```python
# SearchUsersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchUsersRequestPaginateTypeDef


def get_value() -> SearchUsersRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchUsersRequestPaginateTypeDef definition

class SearchUsersRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[UserSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[UserSearchCriteriaPaginatorTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: UserSearchFilterTypeDef](./type_defs.md#usersearchfiltertypedef) 
2. See [:material-code-braces: UserSearchCriteriaPaginatorTypeDef](./type_defs.md#usersearchcriteriapaginatortypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchUsersRequestTypeDef

```python
# SearchUsersRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchUsersRequestTypeDef


def get_value() -> SearchUsersRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchUsersRequestTypeDef definition

class SearchUsersRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[UserSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[UserSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: UserSearchFilterTypeDef](./type_defs.md#usersearchfiltertypedef) 
2. See [:material-code-braces: UserSearchCriteriaTypeDef](./type_defs.md#usersearchcriteriatypedef) 
## EvaluationFormQuestionTypePropertiesOutputTypeDef

```python
# EvaluationFormQuestionTypePropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormQuestionTypePropertiesOutputTypeDef


def get_value() -> EvaluationFormQuestionTypePropertiesOutputTypeDef:
    return {
        "Numeric": ...,
    }


# EvaluationFormQuestionTypePropertiesOutputTypeDef definition

class EvaluationFormQuestionTypePropertiesOutputTypeDef(TypedDict):
    Numeric: NotRequired[EvaluationFormNumericQuestionPropertiesOutputTypeDef],  # (1)
    SingleSelect: NotRequired[EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef],  # (2)
```

1. See [:material-code-braces: EvaluationFormNumericQuestionPropertiesOutputTypeDef](./type_defs.md#evaluationformnumericquestionpropertiesoutputtypedef) 
2. See [:material-code-braces: EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef](./type_defs.md#evaluationformsingleselectquestionpropertiesoutputtypedef) 
## EvaluationFormSingleSelectQuestionPropertiesTypeDef

```python
# EvaluationFormSingleSelectQuestionPropertiesTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormSingleSelectQuestionPropertiesTypeDef


def get_value() -> EvaluationFormSingleSelectQuestionPropertiesTypeDef:
    return {
        "Options": ...,
    }


# EvaluationFormSingleSelectQuestionPropertiesTypeDef definition

class EvaluationFormSingleSelectQuestionPropertiesTypeDef(TypedDict):
    Options: Sequence[EvaluationFormSingleSelectQuestionOptionTypeDef],  # (1)
    DisplayAs: NotRequired[EvaluationFormSingleSelectQuestionDisplayModeType],  # (2)
    Automation: NotRequired[EvaluationFormSingleSelectQuestionAutomationUnionTypeDef],  # (3)
```

1. See [:material-code-braces: EvaluationFormSingleSelectQuestionOptionTypeDef](./type_defs.md#evaluationformsingleselectquestionoptiontypedef) 
2. See [:material-code-brackets: EvaluationFormSingleSelectQuestionDisplayModeType](./literals.md#evaluationformsingleselectquestiondisplaymodetype) 
3. See [:material-code-braces: EvaluationFormSingleSelectQuestionAutomationTypeDef](./type_defs.md#evaluationformsingleselectquestionautomationtypedef) [:material-code-braces: EvaluationFormSingleSelectQuestionAutomationOutputTypeDef](./type_defs.md#evaluationformsingleselectquestionautomationoutputtypedef) 
## RuleTypeDef

```python
# RuleTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RuleTypeDef


def get_value() -> RuleTypeDef:
    return {
        "Name": ...,
    }


# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    Name: str,
    RuleId: str,
    RuleArn: str,
    TriggerEventSource: RuleTriggerEventSourceTypeDef,  # (1)
    Function: str,
    Actions: List[RuleActionOutputTypeDef],  # (2)
    PublishStatus: RulePublishStatusType,  # (3)
    CreatedTime: datetime,
    LastUpdatedTime: datetime,
    LastUpdatedBy: str,
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: RuleTriggerEventSourceTypeDef](./type_defs.md#ruletriggereventsourcetypedef) 
2. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
3. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
## CreateCaseActionDefinitionTypeDef

```python
# CreateCaseActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateCaseActionDefinitionTypeDef


def get_value() -> CreateCaseActionDefinitionTypeDef:
    return {
        "Fields": ...,
    }


# CreateCaseActionDefinitionTypeDef definition

class CreateCaseActionDefinitionTypeDef(TypedDict):
    Fields: Sequence[FieldValueUnionExtraTypeDef],  # (1)
    TemplateId: str,
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
## UpdateCaseActionDefinitionTypeDef

```python
# UpdateCaseActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateCaseActionDefinitionTypeDef


def get_value() -> UpdateCaseActionDefinitionTypeDef:
    return {
        "Fields": ...,
    }


# UpdateCaseActionDefinitionTypeDef definition

class UpdateCaseActionDefinitionTypeDef(TypedDict):
    Fields: Sequence[FieldValueUnionExtraTypeDef],  # (1)
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
## GetMetricDataResponseTypeDef

```python
# GetMetricDataResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetMetricDataResponseTypeDef


def get_value() -> GetMetricDataResponseTypeDef:
    return {
        "NextToken": ...,
    }


# GetMetricDataResponseTypeDef definition

class GetMetricDataResponseTypeDef(TypedDict):
    MetricResults: List[HistoricalMetricResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HistoricalMetricResultTypeDef](./type_defs.md#historicalmetricresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTaskTemplateRequestTypeDef

```python
# CreateTaskTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateTaskTemplateRequestTypeDef


def get_value() -> CreateTaskTemplateRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateTaskTemplateRequestTypeDef definition

class CreateTaskTemplateRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    Fields: Sequence[TaskTemplateFieldUnionTypeDef],  # (1)
    Description: NotRequired[str],
    ContactFlowId: NotRequired[str],
    SelfAssignFlowId: NotRequired[str],
    Constraints: NotRequired[TaskTemplateConstraintsUnionTypeDef],  # (2)
    Defaults: NotRequired[TaskTemplateDefaultsUnionTypeDef],  # (3)
    Status: NotRequired[TaskTemplateStatusType],  # (4)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: TaskTemplateFieldTypeDef](./type_defs.md#tasktemplatefieldtypedef) [:material-code-braces: TaskTemplateFieldOutputTypeDef](./type_defs.md#tasktemplatefieldoutputtypedef) 
2. See [:material-code-braces: TaskTemplateConstraintsTypeDef](./type_defs.md#tasktemplateconstraintstypedef) [:material-code-braces: TaskTemplateConstraintsOutputTypeDef](./type_defs.md#tasktemplateconstraintsoutputtypedef) 
3. See [:material-code-braces: TaskTemplateDefaultsTypeDef](./type_defs.md#tasktemplatedefaultstypedef) [:material-code-braces: TaskTemplateDefaultsOutputTypeDef](./type_defs.md#tasktemplatedefaultsoutputtypedef) 
4. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
## UpdateTaskTemplateRequestTypeDef

```python
# UpdateTaskTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateTaskTemplateRequestTypeDef


def get_value() -> UpdateTaskTemplateRequestTypeDef:
    return {
        "TaskTemplateId": ...,
    }


# UpdateTaskTemplateRequestTypeDef definition

class UpdateTaskTemplateRequestTypeDef(TypedDict):
    TaskTemplateId: str,
    InstanceId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    ContactFlowId: NotRequired[str],
    SelfAssignFlowId: NotRequired[str],
    Constraints: NotRequired[TaskTemplateConstraintsUnionTypeDef],  # (1)
    Defaults: NotRequired[TaskTemplateDefaultsUnionTypeDef],  # (2)
    Status: NotRequired[TaskTemplateStatusType],  # (3)
    Fields: NotRequired[Sequence[TaskTemplateFieldUnionTypeDef]],  # (4)
```

1. See [:material-code-braces: TaskTemplateConstraintsTypeDef](./type_defs.md#tasktemplateconstraintstypedef) [:material-code-braces: TaskTemplateConstraintsOutputTypeDef](./type_defs.md#tasktemplateconstraintsoutputtypedef) 
2. See [:material-code-braces: TaskTemplateDefaultsTypeDef](./type_defs.md#tasktemplatedefaultstypedef) [:material-code-braces: TaskTemplateDefaultsOutputTypeDef](./type_defs.md#tasktemplatedefaultsoutputtypedef) 
3. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
4. See [:material-code-braces: TaskTemplateFieldTypeDef](./type_defs.md#tasktemplatefieldtypedef) [:material-code-braces: TaskTemplateFieldOutputTypeDef](./type_defs.md#tasktemplatefieldoutputtypedef) 
## GetMetricDataV2RequestTypeDef

```python
# GetMetricDataV2RequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetMetricDataV2RequestTypeDef


def get_value() -> GetMetricDataV2RequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# GetMetricDataV2RequestTypeDef definition

class GetMetricDataV2RequestTypeDef(TypedDict):
    ResourceArn: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Filters: Sequence[FilterV2TypeDef],  # (1)
    Metrics: Sequence[MetricV2UnionTypeDef],  # (2)
    Interval: NotRequired[IntervalDetailsTypeDef],  # (3)
    Groupings: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterV2TypeDef](./type_defs.md#filterv2typedef) 
2. See [:material-code-braces: MetricV2TypeDef](./type_defs.md#metricv2typedef) [:material-code-braces: MetricV2OutputTypeDef](./type_defs.md#metricv2outputtypedef) 
3. See [:material-code-braces: IntervalDetailsTypeDef](./type_defs.md#intervaldetailstypedef) 
## GetMetricDataV2ResponseTypeDef

```python
# GetMetricDataV2ResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import GetMetricDataV2ResponseTypeDef


def get_value() -> GetMetricDataV2ResponseTypeDef:
    return {
        "NextToken": ...,
    }


# GetMetricDataV2ResponseTypeDef definition

class GetMetricDataV2ResponseTypeDef(TypedDict):
    MetricResults: List[MetricResultV2TypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MetricResultV2TypeDef](./type_defs.md#metricresultv2typedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateParticipantRoleConfigRequestTypeDef

```python
# UpdateParticipantRoleConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateParticipantRoleConfigRequestTypeDef


def get_value() -> UpdateParticipantRoleConfigRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateParticipantRoleConfigRequestTypeDef definition

class UpdateParticipantRoleConfigRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ChannelConfiguration: UpdateParticipantRoleConfigChannelInfoTypeDef,  # (1)
```

1. See [:material-code-braces: UpdateParticipantRoleConfigChannelInfoTypeDef](./type_defs.md#updateparticipantroleconfigchannelinfotypedef) 
## RealTimeContactAnalysisSegmentCategoriesTypeDef

```python
# RealTimeContactAnalysisSegmentCategoriesTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealTimeContactAnalysisSegmentCategoriesTypeDef


def get_value() -> RealTimeContactAnalysisSegmentCategoriesTypeDef:
    return {
        "MatchedDetails": ...,
    }


# RealTimeContactAnalysisSegmentCategoriesTypeDef definition

class RealTimeContactAnalysisSegmentCategoriesTypeDef(TypedDict):
    MatchedDetails: Dict[str, RealTimeContactAnalysisCategoryDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisCategoryDetailsTypeDef](./type_defs.md#realtimecontactanalysiscategorydetailstypedef) 
## SearchContactsRequestPaginateTypeDef

```python
# SearchContactsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchContactsRequestPaginateTypeDef


def get_value() -> SearchContactsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchContactsRequestPaginateTypeDef definition

class SearchContactsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    TimeRange: SearchContactsTimeRangeTypeDef,  # (1)
    SearchCriteria: NotRequired[SearchCriteriaTypeDef],  # (2)
    Sort: NotRequired[SortTypeDef],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: SearchContactsTimeRangeTypeDef](./type_defs.md#searchcontactstimerangetypedef) 
2. See [:material-code-braces: SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef) 
3. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchContactsRequestTypeDef

```python
# SearchContactsRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import SearchContactsRequestTypeDef


def get_value() -> SearchContactsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SearchContactsRequestTypeDef definition

class SearchContactsRequestTypeDef(TypedDict):
    InstanceId: str,
    TimeRange: SearchContactsTimeRangeTypeDef,  # (1)
    SearchCriteria: NotRequired[SearchCriteriaTypeDef],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Sort: NotRequired[SortTypeDef],  # (3)
```

1. See [:material-code-braces: SearchContactsTimeRangeTypeDef](./type_defs.md#searchcontactstimerangetypedef) 
2. See [:material-code-braces: SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef) 
3. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## RoutingCriteriaTypeDef

```python
# RoutingCriteriaTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RoutingCriteriaTypeDef


def get_value() -> RoutingCriteriaTypeDef:
    return {
        "Steps": ...,
    }


# RoutingCriteriaTypeDef definition

class RoutingCriteriaTypeDef(TypedDict):
    Steps: NotRequired[List[StepTypeDef]],  # (1)
    ActivationTimestamp: NotRequired[datetime],
    Index: NotRequired[int],
```

1. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
## EvaluationFormQuestionOutputTypeDef

```python
# EvaluationFormQuestionOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormQuestionOutputTypeDef


def get_value() -> EvaluationFormQuestionOutputTypeDef:
    return {
        "Title": ...,
    }


# EvaluationFormQuestionOutputTypeDef definition

class EvaluationFormQuestionOutputTypeDef(TypedDict):
    Title: str,
    RefId: str,
    QuestionType: EvaluationFormQuestionTypeType,  # (1)
    Instructions: NotRequired[str],
    NotApplicableEnabled: NotRequired[bool],
    QuestionTypeProperties: NotRequired[EvaluationFormQuestionTypePropertiesOutputTypeDef],  # (2)
    Weight: NotRequired[float],
```

1. See [:material-code-brackets: EvaluationFormQuestionTypeType](./literals.md#evaluationformquestiontypetype) 
2. See [:material-code-braces: EvaluationFormQuestionTypePropertiesOutputTypeDef](./type_defs.md#evaluationformquestiontypepropertiesoutputtypedef) 
## DescribeRuleResponseTypeDef

```python
# DescribeRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeRuleResponseTypeDef


def get_value() -> DescribeRuleResponseTypeDef:
    return {
        "Rule": ...,
    }


# DescribeRuleResponseTypeDef definition

class DescribeRuleResponseTypeDef(TypedDict):
    Rule: RuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RealtimeContactAnalysisSegmentTypeDef

```python
# RealtimeContactAnalysisSegmentTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RealtimeContactAnalysisSegmentTypeDef


def get_value() -> RealtimeContactAnalysisSegmentTypeDef:
    return {
        "Transcript": ...,
    }


# RealtimeContactAnalysisSegmentTypeDef definition

class RealtimeContactAnalysisSegmentTypeDef(TypedDict):
    Transcript: NotRequired[RealTimeContactAnalysisSegmentTranscriptTypeDef],  # (1)
    Categories: NotRequired[RealTimeContactAnalysisSegmentCategoriesTypeDef],  # (2)
    Issues: NotRequired[RealTimeContactAnalysisSegmentIssuesTypeDef],  # (3)
    Event: NotRequired[RealTimeContactAnalysisSegmentEventTypeDef],  # (4)
    Attachments: NotRequired[RealTimeContactAnalysisSegmentAttachmentsTypeDef],  # (5)
    PostContactSummary: NotRequired[RealTimeContactAnalysisSegmentPostContactSummaryTypeDef],  # (6)
```

1. See [:material-code-braces: RealTimeContactAnalysisSegmentTranscriptTypeDef](./type_defs.md#realtimecontactanalysissegmenttranscripttypedef) 
2. See [:material-code-braces: RealTimeContactAnalysisSegmentCategoriesTypeDef](./type_defs.md#realtimecontactanalysissegmentcategoriestypedef) 
3. See [:material-code-braces: RealTimeContactAnalysisSegmentIssuesTypeDef](./type_defs.md#realtimecontactanalysissegmentissuestypedef) 
4. See [:material-code-braces: RealTimeContactAnalysisSegmentEventTypeDef](./type_defs.md#realtimecontactanalysissegmenteventtypedef) 
5. See [:material-code-braces: RealTimeContactAnalysisSegmentAttachmentsTypeDef](./type_defs.md#realtimecontactanalysissegmentattachmentstypedef) 
6. See [:material-code-braces: RealTimeContactAnalysisSegmentPostContactSummaryTypeDef](./type_defs.md#realtimecontactanalysissegmentpostcontactsummarytypedef) 
## ContactTypeDef

```python
# ContactTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ContactTypeDef


def get_value() -> ContactTypeDef:
    return {
        "Arn": ...,
    }


# ContactTypeDef definition

class ContactTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    InitialContactId: NotRequired[str],
    PreviousContactId: NotRequired[str],
    ContactAssociationId: NotRequired[str],
    InitiationMethod: NotRequired[ContactInitiationMethodType],  # (1)
    Name: NotRequired[str],
    Description: NotRequired[str],
    Channel: NotRequired[ChannelType],  # (2)
    QueueInfo: NotRequired[QueueInfoTypeDef],  # (3)
    AgentInfo: NotRequired[AgentInfoTypeDef],  # (4)
    InitiationTimestamp: NotRequired[datetime],
    DisconnectTimestamp: NotRequired[datetime],
    LastUpdateTimestamp: NotRequired[datetime],
    LastPausedTimestamp: NotRequired[datetime],
    LastResumedTimestamp: NotRequired[datetime],
    TotalPauseCount: NotRequired[int],
    TotalPauseDurationInSeconds: NotRequired[int],
    ScheduledTimestamp: NotRequired[datetime],
    RelatedContactId: NotRequired[str],
    WisdomInfo: NotRequired[WisdomInfoTypeDef],  # (5)
    CustomerId: NotRequired[str],
    CustomerEndpoint: NotRequired[EndpointInfoTypeDef],  # (6)
    SystemEndpoint: NotRequired[EndpointInfoTypeDef],  # (6)
    QueueTimeAdjustmentSeconds: NotRequired[int],
    QueuePriority: NotRequired[int],
    Tags: NotRequired[Dict[str, str]],
    ConnectedToSystemTimestamp: NotRequired[datetime],
    RoutingCriteria: NotRequired[RoutingCriteriaTypeDef],  # (8)
    Customer: NotRequired[CustomerTypeDef],  # (9)
    Campaign: NotRequired[CampaignTypeDef],  # (10)
    AnsweringMachineDetectionStatus: NotRequired[AnsweringMachineDetectionStatusType],  # (11)
    CustomerVoiceActivity: NotRequired[CustomerVoiceActivityTypeDef],  # (12)
    QualityMetrics: NotRequired[QualityMetricsTypeDef],  # (13)
    DisconnectDetails: NotRequired[DisconnectDetailsTypeDef],  # (14)
    AdditionalEmailRecipients: NotRequired[AdditionalEmailRecipientsTypeDef],  # (15)
    SegmentAttributes: NotRequired[Dict[str, SegmentAttributeValueOutputTypeDef]],  # (16)
```

1. See [:material-code-brackets: ContactInitiationMethodType](./literals.md#contactinitiationmethodtype) 
2. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
3. See [:material-code-braces: QueueInfoTypeDef](./type_defs.md#queueinfotypedef) 
4. See [:material-code-braces: AgentInfoTypeDef](./type_defs.md#agentinfotypedef) 
5. See [:material-code-braces: WisdomInfoTypeDef](./type_defs.md#wisdominfotypedef) 
6. See [:material-code-braces: EndpointInfoTypeDef](./type_defs.md#endpointinfotypedef) 
7. See [:material-code-braces: EndpointInfoTypeDef](./type_defs.md#endpointinfotypedef) 
8. See [:material-code-braces: RoutingCriteriaTypeDef](./type_defs.md#routingcriteriatypedef) 
9. See [:material-code-braces: CustomerTypeDef](./type_defs.md#customertypedef) 
10. See [:material-code-braces: CampaignTypeDef](./type_defs.md#campaigntypedef) 
11. See [:material-code-brackets: AnsweringMachineDetectionStatusType](./literals.md#answeringmachinedetectionstatustype) 
12. See [:material-code-braces: CustomerVoiceActivityTypeDef](./type_defs.md#customervoiceactivitytypedef) 
13. See [:material-code-braces: QualityMetricsTypeDef](./type_defs.md#qualitymetricstypedef) 
14. See [:material-code-braces: DisconnectDetailsTypeDef](./type_defs.md#disconnectdetailstypedef) 
15. See [:material-code-braces: AdditionalEmailRecipientsTypeDef](./type_defs.md#additionalemailrecipientstypedef) 
16. See [:material-code-braces: SegmentAttributeValueOutputTypeDef](./type_defs.md#segmentattributevalueoutputtypedef) 
## ExpressionTypeDef

```python
# ExpressionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ExpressionTypeDef


def get_value() -> ExpressionTypeDef:
    return {
        "AttributeCondition": ...,
    }


# ExpressionTypeDef definition

class ExpressionTypeDef(TypedDict):
    AttributeCondition: NotRequired[AttributeConditionUnionTypeDef],  # (1)
    AndExpression: NotRequired[Sequence[Mapping[str, Any]]],
    OrExpression: NotRequired[Sequence[Mapping[str, Any]]],
    NotAttributeCondition: NotRequired[AttributeConditionUnionTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeConditionTypeDef](./type_defs.md#attributeconditiontypedef) [:material-code-braces: AttributeConditionOutputTypeDef](./type_defs.md#attributeconditionoutputtypedef) 
2. See [:material-code-braces: AttributeConditionTypeDef](./type_defs.md#attributeconditiontypedef) [:material-code-braces: AttributeConditionOutputTypeDef](./type_defs.md#attributeconditionoutputtypedef) 
## EvaluationFormItemOutputTypeDef

```python
# EvaluationFormItemOutputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormItemOutputTypeDef


def get_value() -> EvaluationFormItemOutputTypeDef:
    return {
        "Section": ...,
    }


# EvaluationFormItemOutputTypeDef definition

class EvaluationFormItemOutputTypeDef(TypedDict):
    Section: NotRequired[EvaluationFormSectionOutputTypeDef],  # (1)
    Question: NotRequired[EvaluationFormQuestionOutputTypeDef],  # (2)
```

1. See [:material-code-braces: EvaluationFormSectionOutputTypeDef](./type_defs.md#evaluationformsectionoutputtypedef) 
2. See [:material-code-braces: EvaluationFormQuestionOutputTypeDef](./type_defs.md#evaluationformquestionoutputtypedef) 
## EvaluationFormQuestionTypePropertiesTypeDef

```python
# EvaluationFormQuestionTypePropertiesTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormQuestionTypePropertiesTypeDef


def get_value() -> EvaluationFormQuestionTypePropertiesTypeDef:
    return {
        "Numeric": ...,
    }


# EvaluationFormQuestionTypePropertiesTypeDef definition

class EvaluationFormQuestionTypePropertiesTypeDef(TypedDict):
    Numeric: NotRequired[EvaluationFormNumericQuestionPropertiesUnionTypeDef],  # (1)
    SingleSelect: NotRequired[EvaluationFormSingleSelectQuestionPropertiesUnionTypeDef],  # (2)
```

1. See [:material-code-braces: EvaluationFormNumericQuestionPropertiesTypeDef](./type_defs.md#evaluationformnumericquestionpropertiestypedef) [:material-code-braces: EvaluationFormNumericQuestionPropertiesOutputTypeDef](./type_defs.md#evaluationformnumericquestionpropertiesoutputtypedef) 
2. See [:material-code-braces: EvaluationFormSingleSelectQuestionPropertiesTypeDef](./type_defs.md#evaluationformsingleselectquestionpropertiestypedef) [:material-code-braces: EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef](./type_defs.md#evaluationformsingleselectquestionpropertiesoutputtypedef) 
## RuleActionTypeDef

```python
# RuleActionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RuleActionTypeDef


def get_value() -> RuleActionTypeDef:
    return {
        "ActionType": ...,
    }


# RuleActionTypeDef definition

class RuleActionTypeDef(TypedDict):
    ActionType: ActionTypeType,  # (1)
    TaskAction: NotRequired[TaskActionDefinitionUnionTypeDef],  # (2)
    EventBridgeAction: NotRequired[EventBridgeActionDefinitionTypeDef],  # (3)
    AssignContactCategoryAction: NotRequired[Mapping[str, Any]],
    SendNotificationAction: NotRequired[SendNotificationActionDefinitionUnionTypeDef],  # (4)
    CreateCaseAction: NotRequired[CreateCaseActionDefinitionUnionTypeDef],  # (5)
    UpdateCaseAction: NotRequired[UpdateCaseActionDefinitionUnionTypeDef],  # (6)
    EndAssociatedTasksAction: NotRequired[Mapping[str, Any]],
    SubmitAutoEvaluationAction: NotRequired[SubmitAutoEvaluationActionDefinitionTypeDef],  # (7)
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-braces: TaskActionDefinitionTypeDef](./type_defs.md#taskactiondefinitiontypedef) [:material-code-braces: TaskActionDefinitionOutputTypeDef](./type_defs.md#taskactiondefinitionoutputtypedef) 
3. See [:material-code-braces: EventBridgeActionDefinitionTypeDef](./type_defs.md#eventbridgeactiondefinitiontypedef) 
4. See [:material-code-braces: SendNotificationActionDefinitionTypeDef](./type_defs.md#sendnotificationactiondefinitiontypedef) [:material-code-braces: SendNotificationActionDefinitionOutputTypeDef](./type_defs.md#sendnotificationactiondefinitionoutputtypedef) 
5. See [:material-code-braces: CreateCaseActionDefinitionTypeDef](./type_defs.md#createcaseactiondefinitiontypedef) [:material-code-braces: CreateCaseActionDefinitionOutputTypeDef](./type_defs.md#createcaseactiondefinitionoutputtypedef) 
6. See [:material-code-braces: UpdateCaseActionDefinitionTypeDef](./type_defs.md#updatecaseactiondefinitiontypedef) [:material-code-braces: UpdateCaseActionDefinitionOutputTypeDef](./type_defs.md#updatecaseactiondefinitionoutputtypedef) 
7. See [:material-code-braces: SubmitAutoEvaluationActionDefinitionTypeDef](./type_defs.md#submitautoevaluationactiondefinitiontypedef) 
## ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef

```python
# ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef


def get_value() -> ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef:
    return {
        "Channel": ...,
    }


# ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef definition

class ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef(TypedDict):
    Channel: RealTimeContactAnalysisSupportedChannelType,  # (1)
    Status: RealTimeContactAnalysisStatusType,  # (2)
    Segments: List[RealtimeContactAnalysisSegmentTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: RealTimeContactAnalysisSupportedChannelType](./literals.md#realtimecontactanalysissupportedchanneltype) 
2. See [:material-code-brackets: RealTimeContactAnalysisStatusType](./literals.md#realtimecontactanalysisstatustype) 
3. See [:material-code-braces: RealtimeContactAnalysisSegmentTypeDef](./type_defs.md#realtimecontactanalysissegmenttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContactResponseTypeDef

```python
# DescribeContactResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeContactResponseTypeDef


def get_value() -> DescribeContactResponseTypeDef:
    return {
        "Contact": ...,
    }


# DescribeContactResponseTypeDef definition

class DescribeContactResponseTypeDef(TypedDict):
    Contact: ContactTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EvaluationFormContentTypeDef

```python
# EvaluationFormContentTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormContentTypeDef


def get_value() -> EvaluationFormContentTypeDef:
    return {
        "EvaluationFormVersion": ...,
    }


# EvaluationFormContentTypeDef definition

class EvaluationFormContentTypeDef(TypedDict):
    EvaluationFormVersion: int,
    EvaluationFormId: str,
    EvaluationFormArn: str,
    Title: str,
    Items: List[EvaluationFormItemOutputTypeDef],  # (1)
    Description: NotRequired[str],
    ScoringStrategy: NotRequired[EvaluationFormScoringStrategyTypeDef],  # (2)
```

1. See [:material-code-braces: EvaluationFormItemOutputTypeDef](./type_defs.md#evaluationformitemoutputtypedef) 
2. See [:material-code-braces: EvaluationFormScoringStrategyTypeDef](./type_defs.md#evaluationformscoringstrategytypedef) 
## EvaluationFormTypeDef

```python
# EvaluationFormTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormTypeDef


def get_value() -> EvaluationFormTypeDef:
    return {
        "EvaluationFormId": ...,
    }


# EvaluationFormTypeDef definition

class EvaluationFormTypeDef(TypedDict):
    EvaluationFormId: str,
    EvaluationFormVersion: int,
    Locked: bool,
    EvaluationFormArn: str,
    Title: str,
    Status: EvaluationFormVersionStatusType,  # (1)
    Items: List[EvaluationFormItemOutputTypeDef],  # (2)
    CreatedTime: datetime,
    CreatedBy: str,
    LastModifiedTime: datetime,
    LastModifiedBy: str,
    Description: NotRequired[str],
    ScoringStrategy: NotRequired[EvaluationFormScoringStrategyTypeDef],  # (3)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: EvaluationFormVersionStatusType](./literals.md#evaluationformversionstatustype) 
2. See [:material-code-braces: EvaluationFormItemOutputTypeDef](./type_defs.md#evaluationformitemoutputtypedef) 
3. See [:material-code-braces: EvaluationFormScoringStrategyTypeDef](./type_defs.md#evaluationformscoringstrategytypedef) 
## RoutingCriteriaInputStepTypeDef

```python
# RoutingCriteriaInputStepTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RoutingCriteriaInputStepTypeDef


def get_value() -> RoutingCriteriaInputStepTypeDef:
    return {
        "Expiry": ...,
    }


# RoutingCriteriaInputStepTypeDef definition

class RoutingCriteriaInputStepTypeDef(TypedDict):
    Expiry: NotRequired[RoutingCriteriaInputStepExpiryTypeDef],  # (1)
    Expression: NotRequired[ExpressionUnionTypeDef],  # (2)
```

1. See [:material-code-braces: RoutingCriteriaInputStepExpiryTypeDef](./type_defs.md#routingcriteriainputstepexpirytypedef) 
2. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
## DescribeContactEvaluationResponseTypeDef

```python
# DescribeContactEvaluationResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeContactEvaluationResponseTypeDef


def get_value() -> DescribeContactEvaluationResponseTypeDef:
    return {
        "Evaluation": ...,
    }


# DescribeContactEvaluationResponseTypeDef definition

class DescribeContactEvaluationResponseTypeDef(TypedDict):
    Evaluation: EvaluationTypeDef,  # (1)
    EvaluationForm: EvaluationFormContentTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EvaluationTypeDef](./type_defs.md#evaluationtypedef) 
2. See [:material-code-braces: EvaluationFormContentTypeDef](./type_defs.md#evaluationformcontenttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEvaluationFormResponseTypeDef

```python
# DescribeEvaluationFormResponseTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import DescribeEvaluationFormResponseTypeDef


def get_value() -> DescribeEvaluationFormResponseTypeDef:
    return {
        "EvaluationForm": ...,
    }


# DescribeEvaluationFormResponseTypeDef definition

class DescribeEvaluationFormResponseTypeDef(TypedDict):
    EvaluationForm: EvaluationFormTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EvaluationFormTypeDef](./type_defs.md#evaluationformtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EvaluationFormQuestionTypeDef

```python
# EvaluationFormQuestionTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormQuestionTypeDef


def get_value() -> EvaluationFormQuestionTypeDef:
    return {
        "Title": ...,
    }


# EvaluationFormQuestionTypeDef definition

class EvaluationFormQuestionTypeDef(TypedDict):
    Title: str,
    RefId: str,
    QuestionType: EvaluationFormQuestionTypeType,  # (1)
    Instructions: NotRequired[str],
    NotApplicableEnabled: NotRequired[bool],
    QuestionTypeProperties: NotRequired[EvaluationFormQuestionTypePropertiesUnionTypeDef],  # (2)
    Weight: NotRequired[float],
```

1. See [:material-code-brackets: EvaluationFormQuestionTypeType](./literals.md#evaluationformquestiontypetype) 
2. See [:material-code-braces: EvaluationFormQuestionTypePropertiesTypeDef](./type_defs.md#evaluationformquestiontypepropertiestypedef) [:material-code-braces: EvaluationFormQuestionTypePropertiesOutputTypeDef](./type_defs.md#evaluationformquestiontypepropertiesoutputtypedef) 
## CreateRuleRequestTypeDef

```python
# CreateRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateRuleRequestTypeDef


def get_value() -> CreateRuleRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateRuleRequestTypeDef definition

class CreateRuleRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    TriggerEventSource: RuleTriggerEventSourceTypeDef,  # (1)
    Function: str,
    Actions: Sequence[RuleActionUnionTypeDef],  # (2)
    PublishStatus: RulePublishStatusType,  # (3)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: RuleTriggerEventSourceTypeDef](./type_defs.md#ruletriggereventsourcetypedef) 
2. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
3. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
## UpdateRuleRequestTypeDef

```python
# UpdateRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateRuleRequestTypeDef


def get_value() -> UpdateRuleRequestTypeDef:
    return {
        "RuleId": ...,
    }


# UpdateRuleRequestTypeDef definition

class UpdateRuleRequestTypeDef(TypedDict):
    RuleId: str,
    InstanceId: str,
    Name: str,
    Function: str,
    Actions: Sequence[RuleActionUnionTypeDef],  # (1)
    PublishStatus: RulePublishStatusType,  # (2)
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
## RoutingCriteriaInputTypeDef

```python
# RoutingCriteriaInputTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import RoutingCriteriaInputTypeDef


def get_value() -> RoutingCriteriaInputTypeDef:
    return {
        "Steps": ...,
    }


# RoutingCriteriaInputTypeDef definition

class RoutingCriteriaInputTypeDef(TypedDict):
    Steps: NotRequired[Sequence[RoutingCriteriaInputStepTypeDef]],  # (1)
```

1. See [:material-code-braces: RoutingCriteriaInputStepTypeDef](./type_defs.md#routingcriteriainputsteptypedef) 
## UpdateContactRoutingDataRequestTypeDef

```python
# UpdateContactRoutingDataRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateContactRoutingDataRequestTypeDef


def get_value() -> UpdateContactRoutingDataRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateContactRoutingDataRequestTypeDef definition

class UpdateContactRoutingDataRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    QueueTimeAdjustmentSeconds: NotRequired[int],
    QueuePriority: NotRequired[int],
    RoutingCriteria: NotRequired[RoutingCriteriaInputTypeDef],  # (1)
```

1. See [:material-code-braces: RoutingCriteriaInputTypeDef](./type_defs.md#routingcriteriainputtypedef) 
## EvaluationFormItemTypeDef

```python
# EvaluationFormItemTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import EvaluationFormItemTypeDef


def get_value() -> EvaluationFormItemTypeDef:
    return {
        "Section": ...,
    }


# EvaluationFormItemTypeDef definition

class EvaluationFormItemTypeDef(TypedDict):
    Section: NotRequired[EvaluationFormSectionUnionTypeDef],  # (1)
    Question: NotRequired[EvaluationFormQuestionUnionTypeDef],  # (2)
```

1. See [:material-code-braces: EvaluationFormSectionTypeDef](./type_defs.md#evaluationformsectiontypedef) [:material-code-braces: EvaluationFormSectionOutputTypeDef](./type_defs.md#evaluationformsectionoutputtypedef) 
2. See [:material-code-braces: EvaluationFormQuestionTypeDef](./type_defs.md#evaluationformquestiontypedef) [:material-code-braces: EvaluationFormQuestionOutputTypeDef](./type_defs.md#evaluationformquestionoutputtypedef) 
## CreateEvaluationFormRequestTypeDef

```python
# CreateEvaluationFormRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import CreateEvaluationFormRequestTypeDef


def get_value() -> CreateEvaluationFormRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateEvaluationFormRequestTypeDef definition

class CreateEvaluationFormRequestTypeDef(TypedDict):
    InstanceId: str,
    Title: str,
    Items: Sequence[EvaluationFormItemUnionTypeDef],  # (1)
    Description: NotRequired[str],
    ScoringStrategy: NotRequired[EvaluationFormScoringStrategyTypeDef],  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: EvaluationFormItemTypeDef](./type_defs.md#evaluationformitemtypedef) [:material-code-braces: EvaluationFormItemOutputTypeDef](./type_defs.md#evaluationformitemoutputtypedef) 
2. See [:material-code-braces: EvaluationFormScoringStrategyTypeDef](./type_defs.md#evaluationformscoringstrategytypedef) 
## UpdateEvaluationFormRequestTypeDef

```python
# UpdateEvaluationFormRequestTypeDef TypedDict usage example

from types_aiobotocore_connect.type_defs import UpdateEvaluationFormRequestTypeDef


def get_value() -> UpdateEvaluationFormRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateEvaluationFormRequestTypeDef definition

class UpdateEvaluationFormRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: int,
    Title: str,
    Items: Sequence[EvaluationFormItemUnionTypeDef],  # (1)
    CreateNewVersion: NotRequired[bool],
    Description: NotRequired[str],
    ScoringStrategy: NotRequired[EvaluationFormScoringStrategyTypeDef],  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: EvaluationFormItemTypeDef](./type_defs.md#evaluationformitemtypedef) [:material-code-braces: EvaluationFormItemOutputTypeDef](./type_defs.md#evaluationformitemoutputtypedef) 
2. See [:material-code-braces: EvaluationFormScoringStrategyTypeDef](./type_defs.md#evaluationformscoringstrategytypedef) 
