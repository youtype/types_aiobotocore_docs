# Type definitions

> [Index](../README.md) > [CloudWatchObservabilityAdminService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAdminService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#cloudwatchobservabilityadminservice)
    type annotations stubs module [types-aiobotocore-observabilityadmin](https://pypi.org/project/types-aiobotocore-observabilityadmin/).



## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ResponseMetadataTypeDef


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


## DeleteTelemetryRuleForOrganizationInputTypeDef

```python
# DeleteTelemetryRuleForOrganizationInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import DeleteTelemetryRuleForOrganizationInputTypeDef


def get_value() -> DeleteTelemetryRuleForOrganizationInputTypeDef:
    return {
        "RuleIdentifier": ...,
    }


# DeleteTelemetryRuleForOrganizationInputTypeDef definition

class DeleteTelemetryRuleForOrganizationInputTypeDef(TypedDict):
    RuleIdentifier: str,
```


## DeleteTelemetryRuleInputTypeDef

```python
# DeleteTelemetryRuleInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import DeleteTelemetryRuleInputTypeDef


def get_value() -> DeleteTelemetryRuleInputTypeDef:
    return {
        "RuleIdentifier": ...,
    }


# DeleteTelemetryRuleInputTypeDef definition

class DeleteTelemetryRuleInputTypeDef(TypedDict):
    RuleIdentifier: str,
```


## GetTelemetryRuleForOrganizationInputTypeDef

```python
# GetTelemetryRuleForOrganizationInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import GetTelemetryRuleForOrganizationInputTypeDef


def get_value() -> GetTelemetryRuleForOrganizationInputTypeDef:
    return {
        "RuleIdentifier": ...,
    }


# GetTelemetryRuleForOrganizationInputTypeDef definition

class GetTelemetryRuleForOrganizationInputTypeDef(TypedDict):
    RuleIdentifier: str,
```


## GetTelemetryRuleInputTypeDef

```python
# GetTelemetryRuleInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import GetTelemetryRuleInputTypeDef


def get_value() -> GetTelemetryRuleInputTypeDef:
    return {
        "RuleIdentifier": ...,
    }


# GetTelemetryRuleInputTypeDef definition

class GetTelemetryRuleInputTypeDef(TypedDict):
    RuleIdentifier: str,
```


## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import PaginatorConfigTypeDef


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


## ListResourceTelemetryForOrganizationInputTypeDef

```python
# ListResourceTelemetryForOrganizationInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryForOrganizationInputTypeDef


def get_value() -> ListResourceTelemetryForOrganizationInputTypeDef:
    return {
        "AccountIdentifiers": ...,
    }


# ListResourceTelemetryForOrganizationInputTypeDef definition

class ListResourceTelemetryForOrganizationInputTypeDef(TypedDict):
    AccountIdentifiers: NotRequired[Sequence[str]],
    ResourceIdentifierPrefix: NotRequired[str],
    ResourceTypes: NotRequired[Sequence[ResourceTypeType]],  # (1)
    TelemetryConfigurationState: NotRequired[Mapping[TelemetryTypeType, TelemetryStateType]],  # (2)
    ResourceTags: NotRequired[Mapping[str, str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See `Sequence[ResourceTypeType]`
2. See `Mapping[TelemetryTypeType, TelemetryStateType]`

## TelemetryConfigurationTypeDef

```python
# TelemetryConfigurationTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import TelemetryConfigurationTypeDef


def get_value() -> TelemetryConfigurationTypeDef:
    return {
        "AccountIdentifier": ...,
    }


# TelemetryConfigurationTypeDef definition

class TelemetryConfigurationTypeDef(TypedDict):
    AccountIdentifier: NotRequired[str],
    TelemetryConfigurationState: NotRequired[Dict[TelemetryTypeType, TelemetryStateType]],  # (1)
    ResourceType: NotRequired[ResourceTypeType],  # (2)
    ResourceIdentifier: NotRequired[str],
    ResourceTags: NotRequired[Dict[str, str]],
    LastUpdateTimeStamp: NotRequired[int],
```

1. See `Dict[TelemetryTypeType, TelemetryStateType]`
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype)

## ListResourceTelemetryInputTypeDef

```python
# ListResourceTelemetryInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryInputTypeDef


def get_value() -> ListResourceTelemetryInputTypeDef:
    return {
        "ResourceIdentifierPrefix": ...,
    }


# ListResourceTelemetryInputTypeDef definition

class ListResourceTelemetryInputTypeDef(TypedDict):
    ResourceIdentifierPrefix: NotRequired[str],
    ResourceTypes: NotRequired[Sequence[ResourceTypeType]],  # (1)
    TelemetryConfigurationState: NotRequired[Mapping[TelemetryTypeType, TelemetryStateType]],  # (2)
    ResourceTags: NotRequired[Mapping[str, str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See `Sequence[ResourceTypeType]`
2. See `Mapping[TelemetryTypeType, TelemetryStateType]`

## ListTagsForResourceInputTypeDef

```python
# ListTagsForResourceInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListTagsForResourceInputTypeDef


def get_value() -> ListTagsForResourceInputTypeDef:
    return {
        "ResourceARN": ...,
    }


# ListTagsForResourceInputTypeDef definition

class ListTagsForResourceInputTypeDef(TypedDict):
    ResourceARN: str,
```


## ListTelemetryRulesForOrganizationInputTypeDef

```python
# ListTelemetryRulesForOrganizationInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListTelemetryRulesForOrganizationInputTypeDef


def get_value() -> ListTelemetryRulesForOrganizationInputTypeDef:
    return {
        "RuleNamePrefix": ...,
    }


# ListTelemetryRulesForOrganizationInputTypeDef definition

class ListTelemetryRulesForOrganizationInputTypeDef(TypedDict):
    RuleNamePrefix: NotRequired[str],
    SourceAccountIds: NotRequired[Sequence[str]],
    SourceOrganizationUnitIds: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```


## TelemetryRuleSummaryTypeDef

```python
# TelemetryRuleSummaryTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import TelemetryRuleSummaryTypeDef


def get_value() -> TelemetryRuleSummaryTypeDef:
    return {
        "RuleName": ...,
    }


# TelemetryRuleSummaryTypeDef definition

class TelemetryRuleSummaryTypeDef(TypedDict):
    RuleName: NotRequired[str],
    RuleArn: NotRequired[str],
    CreatedTimeStamp: NotRequired[int],
    LastUpdateTimeStamp: NotRequired[int],
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    TelemetryType: NotRequired[TelemetryTypeType],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype)
2. See [:material-code-brackets: TelemetryTypeType](./literals.md#telemetrytypetype)

## ListTelemetryRulesInputTypeDef

```python
# ListTelemetryRulesInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListTelemetryRulesInputTypeDef


def get_value() -> ListTelemetryRulesInputTypeDef:
    return {
        "RuleNamePrefix": ...,
    }


# ListTelemetryRulesInputTypeDef definition

class ListTelemetryRulesInputTypeDef(TypedDict):
    RuleNamePrefix: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```


## TagResourceInputTypeDef

```python
# TagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import TagResourceInputTypeDef


def get_value() -> TagResourceInputTypeDef:
    return {
        "ResourceARN": ...,
    }


# TagResourceInputTypeDef definition

class TagResourceInputTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Mapping[str, str],
```


## VPCFlowLogParametersTypeDef

```python
# VPCFlowLogParametersTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import VPCFlowLogParametersTypeDef


def get_value() -> VPCFlowLogParametersTypeDef:
    return {
        "LogFormat": ...,
    }


# VPCFlowLogParametersTypeDef definition

class VPCFlowLogParametersTypeDef(TypedDict):
    LogFormat: NotRequired[str],
    TrafficType: NotRequired[str],
    MaxAggregationInterval: NotRequired[int],
```


## UntagResourceInputTypeDef

```python
# UntagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import UntagResourceInputTypeDef


def get_value() -> UntagResourceInputTypeDef:
    return {
        "ResourceARN": ...,
    }


# UntagResourceInputTypeDef definition

class UntagResourceInputTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```


## CreateTelemetryRuleForOrganizationOutputTypeDef

```python
# CreateTelemetryRuleForOrganizationOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import CreateTelemetryRuleForOrganizationOutputTypeDef


def get_value() -> CreateTelemetryRuleForOrganizationOutputTypeDef:
    return {
        "RuleArn": ...,
    }


# CreateTelemetryRuleForOrganizationOutputTypeDef definition

class CreateTelemetryRuleForOrganizationOutputTypeDef(TypedDict):
    RuleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateTelemetryRuleOutputTypeDef

```python
# CreateTelemetryRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import CreateTelemetryRuleOutputTypeDef


def get_value() -> CreateTelemetryRuleOutputTypeDef:
    return {
        "RuleArn": ...,
    }


# CreateTelemetryRuleOutputTypeDef definition

class CreateTelemetryRuleOutputTypeDef(TypedDict):
    RuleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetTelemetryEvaluationStatusForOrganizationOutputTypeDef

```python
# GetTelemetryEvaluationStatusForOrganizationOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import GetTelemetryEvaluationStatusForOrganizationOutputTypeDef


def get_value() -> GetTelemetryEvaluationStatusForOrganizationOutputTypeDef:
    return {
        "Status": ...,
    }


# GetTelemetryEvaluationStatusForOrganizationOutputTypeDef definition

class GetTelemetryEvaluationStatusForOrganizationOutputTypeDef(TypedDict):
    Status: StatusType,  # (1)
    FailureReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetTelemetryEvaluationStatusOutputTypeDef

```python
# GetTelemetryEvaluationStatusOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import GetTelemetryEvaluationStatusOutputTypeDef


def get_value() -> GetTelemetryEvaluationStatusOutputTypeDef:
    return {
        "Status": ...,
    }


# GetTelemetryEvaluationStatusOutputTypeDef definition

class GetTelemetryEvaluationStatusOutputTypeDef(TypedDict):
    Status: StatusType,  # (1)
    FailureReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListTagsForResourceOutputTypeDef


def get_value() -> ListTagsForResourceOutputTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateTelemetryRuleForOrganizationOutputTypeDef

```python
# UpdateTelemetryRuleForOrganizationOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import UpdateTelemetryRuleForOrganizationOutputTypeDef


def get_value() -> UpdateTelemetryRuleForOrganizationOutputTypeDef:
    return {
        "RuleArn": ...,
    }


# UpdateTelemetryRuleForOrganizationOutputTypeDef definition

class UpdateTelemetryRuleForOrganizationOutputTypeDef(TypedDict):
    RuleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateTelemetryRuleOutputTypeDef

```python
# UpdateTelemetryRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import UpdateTelemetryRuleOutputTypeDef


def get_value() -> UpdateTelemetryRuleOutputTypeDef:
    return {
        "RuleArn": ...,
    }


# UpdateTelemetryRuleOutputTypeDef definition

class UpdateTelemetryRuleOutputTypeDef(TypedDict):
    RuleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListResourceTelemetryForOrganizationInputPaginateTypeDef

```python
# ListResourceTelemetryForOrganizationInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryForOrganizationInputPaginateTypeDef


def get_value() -> ListResourceTelemetryForOrganizationInputPaginateTypeDef:
    return {
        "AccountIdentifiers": ...,
    }


# ListResourceTelemetryForOrganizationInputPaginateTypeDef definition

class ListResourceTelemetryForOrganizationInputPaginateTypeDef(TypedDict):
    AccountIdentifiers: NotRequired[Sequence[str]],
    ResourceIdentifierPrefix: NotRequired[str],
    ResourceTypes: NotRequired[Sequence[ResourceTypeType]],  # (1)
    TelemetryConfigurationState: NotRequired[Mapping[TelemetryTypeType, TelemetryStateType]],  # (2)
    ResourceTags: NotRequired[Mapping[str, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See `Sequence[ResourceTypeType]`
2. See `Mapping[TelemetryTypeType, TelemetryStateType]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListResourceTelemetryInputPaginateTypeDef

```python
# ListResourceTelemetryInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryInputPaginateTypeDef


def get_value() -> ListResourceTelemetryInputPaginateTypeDef:
    return {
        "ResourceIdentifierPrefix": ...,
    }


# ListResourceTelemetryInputPaginateTypeDef definition

class ListResourceTelemetryInputPaginateTypeDef(TypedDict):
    ResourceIdentifierPrefix: NotRequired[str],
    ResourceTypes: NotRequired[Sequence[ResourceTypeType]],  # (1)
    TelemetryConfigurationState: NotRequired[Mapping[TelemetryTypeType, TelemetryStateType]],  # (2)
    ResourceTags: NotRequired[Mapping[str, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See `Sequence[ResourceTypeType]`
2. See `Mapping[TelemetryTypeType, TelemetryStateType]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListTelemetryRulesForOrganizationInputPaginateTypeDef

```python
# ListTelemetryRulesForOrganizationInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListTelemetryRulesForOrganizationInputPaginateTypeDef


def get_value() -> ListTelemetryRulesForOrganizationInputPaginateTypeDef:
    return {
        "RuleNamePrefix": ...,
    }


# ListTelemetryRulesForOrganizationInputPaginateTypeDef definition

class ListTelemetryRulesForOrganizationInputPaginateTypeDef(TypedDict):
    RuleNamePrefix: NotRequired[str],
    SourceAccountIds: NotRequired[Sequence[str]],
    SourceOrganizationUnitIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListTelemetryRulesInputPaginateTypeDef

```python
# ListTelemetryRulesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListTelemetryRulesInputPaginateTypeDef


def get_value() -> ListTelemetryRulesInputPaginateTypeDef:
    return {
        "RuleNamePrefix": ...,
    }


# ListTelemetryRulesInputPaginateTypeDef definition

class ListTelemetryRulesInputPaginateTypeDef(TypedDict):
    RuleNamePrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListResourceTelemetryForOrganizationOutputTypeDef

```python
# ListResourceTelemetryForOrganizationOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryForOrganizationOutputTypeDef


def get_value() -> ListResourceTelemetryForOrganizationOutputTypeDef:
    return {
        "TelemetryConfigurations": ...,
    }


# ListResourceTelemetryForOrganizationOutputTypeDef definition

class ListResourceTelemetryForOrganizationOutputTypeDef(TypedDict):
    TelemetryConfigurations: List[TelemetryConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[TelemetryConfigurationTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListResourceTelemetryOutputTypeDef

```python
# ListResourceTelemetryOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryOutputTypeDef


def get_value() -> ListResourceTelemetryOutputTypeDef:
    return {
        "TelemetryConfigurations": ...,
    }


# ListResourceTelemetryOutputTypeDef definition

class ListResourceTelemetryOutputTypeDef(TypedDict):
    TelemetryConfigurations: List[TelemetryConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[TelemetryConfigurationTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListTelemetryRulesForOrganizationOutputTypeDef

```python
# ListTelemetryRulesForOrganizationOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListTelemetryRulesForOrganizationOutputTypeDef


def get_value() -> ListTelemetryRulesForOrganizationOutputTypeDef:
    return {
        "TelemetryRuleSummaries": ...,
    }


# ListTelemetryRulesForOrganizationOutputTypeDef definition

class ListTelemetryRulesForOrganizationOutputTypeDef(TypedDict):
    TelemetryRuleSummaries: List[TelemetryRuleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[TelemetryRuleSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListTelemetryRulesOutputTypeDef

```python
# ListTelemetryRulesOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListTelemetryRulesOutputTypeDef


def get_value() -> ListTelemetryRulesOutputTypeDef:
    return {
        "TelemetryRuleSummaries": ...,
    }


# ListTelemetryRulesOutputTypeDef definition

class ListTelemetryRulesOutputTypeDef(TypedDict):
    TelemetryRuleSummaries: List[TelemetryRuleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[TelemetryRuleSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## TelemetryDestinationConfigurationTypeDef

```python
# TelemetryDestinationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import TelemetryDestinationConfigurationTypeDef


def get_value() -> TelemetryDestinationConfigurationTypeDef:
    return {
        "DestinationType": ...,
    }


# TelemetryDestinationConfigurationTypeDef definition

class TelemetryDestinationConfigurationTypeDef(TypedDict):
    DestinationType: NotRequired[DestinationTypeType],  # (1)
    DestinationPattern: NotRequired[str],
    RetentionInDays: NotRequired[int],
    VPCFlowLogParameters: NotRequired[VPCFlowLogParametersTypeDef],  # (2)
```

1. See [:material-code-brackets: DestinationTypeType](./literals.md#destinationtypetype)
2. See [:material-code-braces: VPCFlowLogParametersTypeDef](./type_defs.md#vpcflowlogparameterstypedef)

## TelemetryRuleTypeDef

```python
# TelemetryRuleTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import TelemetryRuleTypeDef


def get_value() -> TelemetryRuleTypeDef:
    return {
        "ResourceType": ...,
    }


# TelemetryRuleTypeDef definition

class TelemetryRuleTypeDef(TypedDict):
    TelemetryType: TelemetryTypeType,  # (2)
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    DestinationConfiguration: NotRequired[TelemetryDestinationConfigurationTypeDef],  # (3)
    Scope: NotRequired[str],
    SelectionCriteria: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype)
2. See [:material-code-brackets: TelemetryTypeType](./literals.md#telemetrytypetype)
3. See [:material-code-braces: TelemetryDestinationConfigurationTypeDef](./type_defs.md#telemetrydestinationconfigurationtypedef)

## CreateTelemetryRuleForOrganizationInputTypeDef

```python
# CreateTelemetryRuleForOrganizationInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import CreateTelemetryRuleForOrganizationInputTypeDef


def get_value() -> CreateTelemetryRuleForOrganizationInputTypeDef:
    return {
        "RuleName": ...,
    }


# CreateTelemetryRuleForOrganizationInputTypeDef definition

class CreateTelemetryRuleForOrganizationInputTypeDef(TypedDict):
    RuleName: str,
    Rule: TelemetryRuleTypeDef,  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: TelemetryRuleTypeDef](./type_defs.md#telemetryruletypedef)

## CreateTelemetryRuleInputTypeDef

```python
# CreateTelemetryRuleInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import CreateTelemetryRuleInputTypeDef


def get_value() -> CreateTelemetryRuleInputTypeDef:
    return {
        "RuleName": ...,
    }


# CreateTelemetryRuleInputTypeDef definition

class CreateTelemetryRuleInputTypeDef(TypedDict):
    RuleName: str,
    Rule: TelemetryRuleTypeDef,  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: TelemetryRuleTypeDef](./type_defs.md#telemetryruletypedef)

## GetTelemetryRuleForOrganizationOutputTypeDef

```python
# GetTelemetryRuleForOrganizationOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import GetTelemetryRuleForOrganizationOutputTypeDef


def get_value() -> GetTelemetryRuleForOrganizationOutputTypeDef:
    return {
        "RuleName": ...,
    }


# GetTelemetryRuleForOrganizationOutputTypeDef definition

class GetTelemetryRuleForOrganizationOutputTypeDef(TypedDict):
    RuleName: str,
    RuleArn: str,
    CreatedTimeStamp: int,
    LastUpdateTimeStamp: int,
    TelemetryRule: TelemetryRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TelemetryRuleTypeDef](./type_defs.md#telemetryruletypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetTelemetryRuleOutputTypeDef

```python
# GetTelemetryRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import GetTelemetryRuleOutputTypeDef


def get_value() -> GetTelemetryRuleOutputTypeDef:
    return {
        "RuleName": ...,
    }


# GetTelemetryRuleOutputTypeDef definition

class GetTelemetryRuleOutputTypeDef(TypedDict):
    RuleName: str,
    RuleArn: str,
    CreatedTimeStamp: int,
    LastUpdateTimeStamp: int,
    TelemetryRule: TelemetryRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TelemetryRuleTypeDef](./type_defs.md#telemetryruletypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateTelemetryRuleForOrganizationInputTypeDef

```python
# UpdateTelemetryRuleForOrganizationInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import UpdateTelemetryRuleForOrganizationInputTypeDef


def get_value() -> UpdateTelemetryRuleForOrganizationInputTypeDef:
    return {
        "RuleIdentifier": ...,
    }


# UpdateTelemetryRuleForOrganizationInputTypeDef definition

class UpdateTelemetryRuleForOrganizationInputTypeDef(TypedDict):
    RuleIdentifier: str,
    Rule: TelemetryRuleTypeDef,  # (1)
```

1. See [:material-code-braces: TelemetryRuleTypeDef](./type_defs.md#telemetryruletypedef)

## UpdateTelemetryRuleInputTypeDef

```python
# UpdateTelemetryRuleInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import UpdateTelemetryRuleInputTypeDef


def get_value() -> UpdateTelemetryRuleInputTypeDef:
    return {
        "RuleIdentifier": ...,
    }


# UpdateTelemetryRuleInputTypeDef definition

class UpdateTelemetryRuleInputTypeDef(TypedDict):
    RuleIdentifier: str,
    Rule: TelemetryRuleTypeDef,  # (1)
```

1. See [:material-code-braces: TelemetryRuleTypeDef](./type_defs.md#telemetryruletypedef)

