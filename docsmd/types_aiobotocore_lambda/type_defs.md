# Type definitions

> [Index](../README.md) > [Lambda](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Lambda](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#lambda)
    type annotations stubs module [types-aiobotocore-lambda](https://pypi.org/project/types-aiobotocore-lambda/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_lambda.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


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
# TimestampTypeDef Union usage example

from types_aiobotocore_lambda.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AliasRoutingConfigurationUnionTypeDef

```python
# AliasRoutingConfigurationUnionTypeDef Union usage example

from types_aiobotocore_lambda.type_defs import AliasRoutingConfigurationUnionTypeDef


def get_value() -> AliasRoutingConfigurationUnionTypeDef:
    return ...


# AliasRoutingConfigurationUnionTypeDef definition

AliasRoutingConfigurationUnionTypeDef = Union[
    AliasRoutingConfigurationTypeDef,  # (1)
    AliasRoutingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AliasRoutingConfigurationTypeDef](./type_defs.md#aliasroutingconfigurationtypedef) 
2. See [:material-code-braces: AliasRoutingConfigurationOutputTypeDef](./type_defs.md#aliasroutingconfigurationoutputtypedef) 

## AllowedPublishersUnionTypeDef

```python
# AllowedPublishersUnionTypeDef Union usage example

from types_aiobotocore_lambda.type_defs import AllowedPublishersUnionTypeDef


def get_value() -> AllowedPublishersUnionTypeDef:
    return ...


# AllowedPublishersUnionTypeDef definition

AllowedPublishersUnionTypeDef = Union[
    AllowedPublishersTypeDef,  # (1)
    AllowedPublishersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AllowedPublishersTypeDef](./type_defs.md#allowedpublisherstypedef) 
2. See [:material-code-braces: AllowedPublishersOutputTypeDef](./type_defs.md#allowedpublishersoutputtypedef) 

## CorsUnionTypeDef

```python
# CorsUnionTypeDef Union usage example

from types_aiobotocore_lambda.type_defs import CorsUnionTypeDef


def get_value() -> CorsUnionTypeDef:
    return ...


# CorsUnionTypeDef definition

CorsUnionTypeDef = Union[
    CorsTypeDef,  # (1)
    CorsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CorsTypeDef](./type_defs.md#corstypedef) 
2. See [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 

## EventSourceMappingMetricsConfigUnionTypeDef

```python
# EventSourceMappingMetricsConfigUnionTypeDef Union usage example

from types_aiobotocore_lambda.type_defs import EventSourceMappingMetricsConfigUnionTypeDef


def get_value() -> EventSourceMappingMetricsConfigUnionTypeDef:
    return ...


# EventSourceMappingMetricsConfigUnionTypeDef definition

EventSourceMappingMetricsConfigUnionTypeDef = Union[
    EventSourceMappingMetricsConfigTypeDef,  # (1)
    EventSourceMappingMetricsConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EventSourceMappingMetricsConfigTypeDef](./type_defs.md#eventsourcemappingmetricsconfigtypedef) 
2. See [:material-code-braces: EventSourceMappingMetricsConfigOutputTypeDef](./type_defs.md#eventsourcemappingmetricsconfigoutputtypedef) 

## ImageConfigUnionTypeDef

```python
# ImageConfigUnionTypeDef Union usage example

from types_aiobotocore_lambda.type_defs import ImageConfigUnionTypeDef


def get_value() -> ImageConfigUnionTypeDef:
    return ...


# ImageConfigUnionTypeDef definition

ImageConfigUnionTypeDef = Union[
    ImageConfigTypeDef,  # (1)
    ImageConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ImageConfigTypeDef](./type_defs.md#imageconfigtypedef) 
2. See [:material-code-braces: ImageConfigOutputTypeDef](./type_defs.md#imageconfigoutputtypedef) 

## SelfManagedEventSourceUnionTypeDef

```python
# SelfManagedEventSourceUnionTypeDef Union usage example

from types_aiobotocore_lambda.type_defs import SelfManagedEventSourceUnionTypeDef


def get_value() -> SelfManagedEventSourceUnionTypeDef:
    return ...


# SelfManagedEventSourceUnionTypeDef definition

SelfManagedEventSourceUnionTypeDef = Union[
    SelfManagedEventSourceTypeDef,  # (1)
    SelfManagedEventSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SelfManagedEventSourceTypeDef](./type_defs.md#selfmanagedeventsourcetypedef) 
2. See [:material-code-braces: SelfManagedEventSourceOutputTypeDef](./type_defs.md#selfmanagedeventsourceoutputtypedef) 

## FilterCriteriaUnionTypeDef

```python
# FilterCriteriaUnionTypeDef Union usage example

from types_aiobotocore_lambda.type_defs import FilterCriteriaUnionTypeDef


def get_value() -> FilterCriteriaUnionTypeDef:
    return ...


# FilterCriteriaUnionTypeDef definition

FilterCriteriaUnionTypeDef = Union[
    FilterCriteriaTypeDef,  # (1)
    FilterCriteriaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-braces: FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef) 



## AccountLimitTypeDef

```python
# AccountLimitTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import AccountLimitTypeDef


def get_value() -> AccountLimitTypeDef:
    return {
        "TotalCodeSize": ...,
    }


# AccountLimitTypeDef definition

class AccountLimitTypeDef(TypedDict):
    TotalCodeSize: NotRequired[int],
    CodeSizeUnzipped: NotRequired[int],
    CodeSizeZipped: NotRequired[int],
    ConcurrentExecutions: NotRequired[int],
    UnreservedConcurrentExecutions: NotRequired[int],
```

## AccountUsageTypeDef

```python
# AccountUsageTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import AccountUsageTypeDef


def get_value() -> AccountUsageTypeDef:
    return {
        "TotalCodeSize": ...,
    }


# AccountUsageTypeDef definition

class AccountUsageTypeDef(TypedDict):
    TotalCodeSize: NotRequired[int],
    FunctionCount: NotRequired[int],
```

## AddLayerVersionPermissionRequestTypeDef

```python
# AddLayerVersionPermissionRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import AddLayerVersionPermissionRequestTypeDef


def get_value() -> AddLayerVersionPermissionRequestTypeDef:
    return {
        "LayerName": ...,
    }


# AddLayerVersionPermissionRequestTypeDef definition

class AddLayerVersionPermissionRequestTypeDef(TypedDict):
    LayerName: str,
    VersionNumber: int,
    StatementId: str,
    Action: str,
    Principal: str,
    OrganizationId: NotRequired[str],
    RevisionId: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ResponseMetadataTypeDef


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

## AddPermissionRequestTypeDef

```python
# AddPermissionRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import AddPermissionRequestTypeDef


def get_value() -> AddPermissionRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# AddPermissionRequestTypeDef definition

class AddPermissionRequestTypeDef(TypedDict):
    FunctionName: str,
    StatementId: str,
    Action: str,
    Principal: str,
    SourceArn: NotRequired[str],
    SourceAccount: NotRequired[str],
    EventSourceToken: NotRequired[str],
    Qualifier: NotRequired[str],
    RevisionId: NotRequired[str],
    PrincipalOrgID: NotRequired[str],
    FunctionUrlAuthType: NotRequired[FunctionUrlAuthTypeType],  # (1)
```

1. See [:material-code-brackets: FunctionUrlAuthTypeType](./literals.md#functionurlauthtypetype) 
## AliasRoutingConfigurationOutputTypeDef

```python
# AliasRoutingConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import AliasRoutingConfigurationOutputTypeDef


def get_value() -> AliasRoutingConfigurationOutputTypeDef:
    return {
        "AdditionalVersionWeights": ...,
    }


# AliasRoutingConfigurationOutputTypeDef definition

class AliasRoutingConfigurationOutputTypeDef(TypedDict):
    AdditionalVersionWeights: NotRequired[Dict[str, float]],
```

## AliasRoutingConfigurationTypeDef

```python
# AliasRoutingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import AliasRoutingConfigurationTypeDef


def get_value() -> AliasRoutingConfigurationTypeDef:
    return {
        "AdditionalVersionWeights": ...,
    }


# AliasRoutingConfigurationTypeDef definition

class AliasRoutingConfigurationTypeDef(TypedDict):
    AdditionalVersionWeights: NotRequired[Mapping[str, float]],
```

## AllowedPublishersOutputTypeDef

```python
# AllowedPublishersOutputTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import AllowedPublishersOutputTypeDef


def get_value() -> AllowedPublishersOutputTypeDef:
    return {
        "SigningProfileVersionArns": ...,
    }


# AllowedPublishersOutputTypeDef definition

class AllowedPublishersOutputTypeDef(TypedDict):
    SigningProfileVersionArns: List[str],
```

## AllowedPublishersTypeDef

```python
# AllowedPublishersTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import AllowedPublishersTypeDef


def get_value() -> AllowedPublishersTypeDef:
    return {
        "SigningProfileVersionArns": ...,
    }


# AllowedPublishersTypeDef definition

class AllowedPublishersTypeDef(TypedDict):
    SigningProfileVersionArns: Sequence[str],
```

## AmazonManagedKafkaEventSourceConfigTypeDef

```python
# AmazonManagedKafkaEventSourceConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import AmazonManagedKafkaEventSourceConfigTypeDef


def get_value() -> AmazonManagedKafkaEventSourceConfigTypeDef:
    return {
        "ConsumerGroupId": ...,
    }


# AmazonManagedKafkaEventSourceConfigTypeDef definition

class AmazonManagedKafkaEventSourceConfigTypeDef(TypedDict):
    ConsumerGroupId: NotRequired[str],
```

## CodeSigningPoliciesTypeDef

```python
# CodeSigningPoliciesTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import CodeSigningPoliciesTypeDef


def get_value() -> CodeSigningPoliciesTypeDef:
    return {
        "UntrustedArtifactOnDeployment": ...,
    }


# CodeSigningPoliciesTypeDef definition

class CodeSigningPoliciesTypeDef(TypedDict):
    UntrustedArtifactOnDeployment: NotRequired[CodeSigningPolicyType],  # (1)
```

1. See [:material-code-brackets: CodeSigningPolicyType](./literals.md#codesigningpolicytype) 
## ConcurrencyTypeDef

```python
# ConcurrencyTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ConcurrencyTypeDef


def get_value() -> ConcurrencyTypeDef:
    return {
        "ReservedConcurrentExecutions": ...,
    }


# ConcurrencyTypeDef definition

class ConcurrencyTypeDef(TypedDict):
    ReservedConcurrentExecutions: NotRequired[int],
```

## CorsOutputTypeDef

```python
# CorsOutputTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import CorsOutputTypeDef


def get_value() -> CorsOutputTypeDef:
    return {
        "AllowCredentials": ...,
    }


# CorsOutputTypeDef definition

class CorsOutputTypeDef(TypedDict):
    AllowCredentials: NotRequired[bool],
    AllowHeaders: NotRequired[List[str]],
    AllowMethods: NotRequired[List[str]],
    AllowOrigins: NotRequired[List[str]],
    ExposeHeaders: NotRequired[List[str]],
    MaxAge: NotRequired[int],
```

## CorsTypeDef

```python
# CorsTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import CorsTypeDef


def get_value() -> CorsTypeDef:
    return {
        "AllowCredentials": ...,
    }


# CorsTypeDef definition

class CorsTypeDef(TypedDict):
    AllowCredentials: NotRequired[bool],
    AllowHeaders: NotRequired[Sequence[str]],
    AllowMethods: NotRequired[Sequence[str]],
    AllowOrigins: NotRequired[Sequence[str]],
    ExposeHeaders: NotRequired[Sequence[str]],
    MaxAge: NotRequired[int],
```

## DocumentDBEventSourceConfigTypeDef

```python
# DocumentDBEventSourceConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import DocumentDBEventSourceConfigTypeDef


def get_value() -> DocumentDBEventSourceConfigTypeDef:
    return {
        "DatabaseName": ...,
    }


# DocumentDBEventSourceConfigTypeDef definition

class DocumentDBEventSourceConfigTypeDef(TypedDict):
    DatabaseName: NotRequired[str],
    CollectionName: NotRequired[str],
    FullDocument: NotRequired[FullDocumentType],  # (1)
```

1. See [:material-code-brackets: FullDocumentType](./literals.md#fulldocumenttype) 
## ProvisionedPollerConfigTypeDef

```python
# ProvisionedPollerConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ProvisionedPollerConfigTypeDef


def get_value() -> ProvisionedPollerConfigTypeDef:
    return {
        "MinimumPollers": ...,
    }


# ProvisionedPollerConfigTypeDef definition

class ProvisionedPollerConfigTypeDef(TypedDict):
    MinimumPollers: NotRequired[int],
    MaximumPollers: NotRequired[int],
```

## ScalingConfigTypeDef

```python
# ScalingConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ScalingConfigTypeDef


def get_value() -> ScalingConfigTypeDef:
    return {
        "MaximumConcurrency": ...,
    }


# ScalingConfigTypeDef definition

class ScalingConfigTypeDef(TypedDict):
    MaximumConcurrency: NotRequired[int],
```

## SelfManagedKafkaEventSourceConfigTypeDef

```python
# SelfManagedKafkaEventSourceConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import SelfManagedKafkaEventSourceConfigTypeDef


def get_value() -> SelfManagedKafkaEventSourceConfigTypeDef:
    return {
        "ConsumerGroupId": ...,
    }


# SelfManagedKafkaEventSourceConfigTypeDef definition

class SelfManagedKafkaEventSourceConfigTypeDef(TypedDict):
    ConsumerGroupId: NotRequired[str],
```

## SourceAccessConfigurationTypeDef

```python
# SourceAccessConfigurationTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import SourceAccessConfigurationTypeDef


def get_value() -> SourceAccessConfigurationTypeDef:
    return {
        "Type": ...,
    }


# SourceAccessConfigurationTypeDef definition

class SourceAccessConfigurationTypeDef(TypedDict):
    Type: NotRequired[SourceAccessTypeType],  # (1)
    URI: NotRequired[str],
```

1. See [:material-code-brackets: SourceAccessTypeType](./literals.md#sourceaccesstypetype) 
## DeadLetterConfigTypeDef

```python
# DeadLetterConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import DeadLetterConfigTypeDef


def get_value() -> DeadLetterConfigTypeDef:
    return {
        "TargetArn": ...,
    }


# DeadLetterConfigTypeDef definition

class DeadLetterConfigTypeDef(TypedDict):
    TargetArn: NotRequired[str],
```

## EnvironmentTypeDef

```python
# EnvironmentTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import EnvironmentTypeDef


def get_value() -> EnvironmentTypeDef:
    return {
        "Variables": ...,
    }


# EnvironmentTypeDef definition

class EnvironmentTypeDef(TypedDict):
    Variables: NotRequired[Mapping[str, str]],
```

## EphemeralStorageTypeDef

```python
# EphemeralStorageTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import EphemeralStorageTypeDef


def get_value() -> EphemeralStorageTypeDef:
    return {
        "Size": ...,
    }


# EphemeralStorageTypeDef definition

class EphemeralStorageTypeDef(TypedDict):
    Size: int,
```

## FileSystemConfigTypeDef

```python
# FileSystemConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import FileSystemConfigTypeDef


def get_value() -> FileSystemConfigTypeDef:
    return {
        "Arn": ...,
    }


# FileSystemConfigTypeDef definition

class FileSystemConfigTypeDef(TypedDict):
    Arn: str,
    LocalMountPath: str,
```

## LoggingConfigTypeDef

```python
# LoggingConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import LoggingConfigTypeDef


def get_value() -> LoggingConfigTypeDef:
    return {
        "LogFormat": ...,
    }


# LoggingConfigTypeDef definition

class LoggingConfigTypeDef(TypedDict):
    LogFormat: NotRequired[LogFormatType],  # (1)
    ApplicationLogLevel: NotRequired[ApplicationLogLevelType],  # (2)
    SystemLogLevel: NotRequired[SystemLogLevelType],  # (3)
    LogGroup: NotRequired[str],
```

1. See [:material-code-brackets: LogFormatType](./literals.md#logformattype) 
2. See [:material-code-brackets: ApplicationLogLevelType](./literals.md#applicationlogleveltype) 
3. See [:material-code-brackets: SystemLogLevelType](./literals.md#systemlogleveltype) 
## SnapStartTypeDef

```python
# SnapStartTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import SnapStartTypeDef


def get_value() -> SnapStartTypeDef:
    return {
        "ApplyOn": ...,
    }


# SnapStartTypeDef definition

class SnapStartTypeDef(TypedDict):
    ApplyOn: NotRequired[SnapStartApplyOnType],  # (1)
```

1. See [:material-code-brackets: SnapStartApplyOnType](./literals.md#snapstartapplyontype) 
## TracingConfigTypeDef

```python
# TracingConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import TracingConfigTypeDef


def get_value() -> TracingConfigTypeDef:
    return {
        "Mode": ...,
    }


# TracingConfigTypeDef definition

class TracingConfigTypeDef(TypedDict):
    Mode: NotRequired[TracingModeType],  # (1)
```

1. See [:material-code-brackets: TracingModeType](./literals.md#tracingmodetype) 
## VpcConfigTypeDef

```python
# VpcConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import VpcConfigTypeDef


def get_value() -> VpcConfigTypeDef:
    return {
        "SubnetIds": ...,
    }


# VpcConfigTypeDef definition

class VpcConfigTypeDef(TypedDict):
    SubnetIds: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
    Ipv6AllowedForDualStack: NotRequired[bool],
```

## DeleteAliasRequestTypeDef

```python
# DeleteAliasRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import DeleteAliasRequestTypeDef


def get_value() -> DeleteAliasRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# DeleteAliasRequestTypeDef definition

class DeleteAliasRequestTypeDef(TypedDict):
    FunctionName: str,
    Name: str,
```

## DeleteCodeSigningConfigRequestTypeDef

```python
# DeleteCodeSigningConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import DeleteCodeSigningConfigRequestTypeDef


def get_value() -> DeleteCodeSigningConfigRequestTypeDef:
    return {
        "CodeSigningConfigArn": ...,
    }


# DeleteCodeSigningConfigRequestTypeDef definition

class DeleteCodeSigningConfigRequestTypeDef(TypedDict):
    CodeSigningConfigArn: str,
```

## DeleteEventSourceMappingRequestTypeDef

```python
# DeleteEventSourceMappingRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import DeleteEventSourceMappingRequestTypeDef


def get_value() -> DeleteEventSourceMappingRequestTypeDef:
    return {
        "UUID": ...,
    }


# DeleteEventSourceMappingRequestTypeDef definition

class DeleteEventSourceMappingRequestTypeDef(TypedDict):
    UUID: str,
```

## DeleteFunctionCodeSigningConfigRequestTypeDef

```python
# DeleteFunctionCodeSigningConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import DeleteFunctionCodeSigningConfigRequestTypeDef


def get_value() -> DeleteFunctionCodeSigningConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# DeleteFunctionCodeSigningConfigRequestTypeDef definition

class DeleteFunctionCodeSigningConfigRequestTypeDef(TypedDict):
    FunctionName: str,
```

## DeleteFunctionConcurrencyRequestTypeDef

```python
# DeleteFunctionConcurrencyRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import DeleteFunctionConcurrencyRequestTypeDef


def get_value() -> DeleteFunctionConcurrencyRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# DeleteFunctionConcurrencyRequestTypeDef definition

class DeleteFunctionConcurrencyRequestTypeDef(TypedDict):
    FunctionName: str,
```

## DeleteFunctionEventInvokeConfigRequestTypeDef

```python
# DeleteFunctionEventInvokeConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import DeleteFunctionEventInvokeConfigRequestTypeDef


def get_value() -> DeleteFunctionEventInvokeConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# DeleteFunctionEventInvokeConfigRequestTypeDef definition

class DeleteFunctionEventInvokeConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## DeleteFunctionRequestTypeDef

```python
# DeleteFunctionRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import DeleteFunctionRequestTypeDef


def get_value() -> DeleteFunctionRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# DeleteFunctionRequestTypeDef definition

class DeleteFunctionRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## DeleteFunctionUrlConfigRequestTypeDef

```python
# DeleteFunctionUrlConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import DeleteFunctionUrlConfigRequestTypeDef


def get_value() -> DeleteFunctionUrlConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# DeleteFunctionUrlConfigRequestTypeDef definition

class DeleteFunctionUrlConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## DeleteLayerVersionRequestTypeDef

```python
# DeleteLayerVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import DeleteLayerVersionRequestTypeDef


def get_value() -> DeleteLayerVersionRequestTypeDef:
    return {
        "LayerName": ...,
    }


# DeleteLayerVersionRequestTypeDef definition

class DeleteLayerVersionRequestTypeDef(TypedDict):
    LayerName: str,
    VersionNumber: int,
```

## DeleteProvisionedConcurrencyConfigRequestTypeDef

```python
# DeleteProvisionedConcurrencyConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import DeleteProvisionedConcurrencyConfigRequestTypeDef


def get_value() -> DeleteProvisionedConcurrencyConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# DeleteProvisionedConcurrencyConfigRequestTypeDef definition

class DeleteProvisionedConcurrencyConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: str,
```

## OnFailureTypeDef

```python
# OnFailureTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import OnFailureTypeDef


def get_value() -> OnFailureTypeDef:
    return {
        "Destination": ...,
    }


# OnFailureTypeDef definition

class OnFailureTypeDef(TypedDict):
    Destination: NotRequired[str],
```

## OnSuccessTypeDef

```python
# OnSuccessTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import OnSuccessTypeDef


def get_value() -> OnSuccessTypeDef:
    return {
        "Destination": ...,
    }


# OnSuccessTypeDef definition

class OnSuccessTypeDef(TypedDict):
    Destination: NotRequired[str],
```

## EnvironmentErrorTypeDef

```python
# EnvironmentErrorTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import EnvironmentErrorTypeDef


def get_value() -> EnvironmentErrorTypeDef:
    return {
        "ErrorCode": ...,
    }


# EnvironmentErrorTypeDef definition

class EnvironmentErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## EventSourceMappingMetricsConfigOutputTypeDef

```python
# EventSourceMappingMetricsConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import EventSourceMappingMetricsConfigOutputTypeDef


def get_value() -> EventSourceMappingMetricsConfigOutputTypeDef:
    return {
        "Metrics": ...,
    }


# EventSourceMappingMetricsConfigOutputTypeDef definition

class EventSourceMappingMetricsConfigOutputTypeDef(TypedDict):
    Metrics: NotRequired[List[EventSourceMappingMetricType]],  # (1)
```

1. See [:material-code-brackets: EventSourceMappingMetricType](./literals.md#eventsourcemappingmetrictype) 
## FilterCriteriaErrorTypeDef

```python
# FilterCriteriaErrorTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import FilterCriteriaErrorTypeDef


def get_value() -> FilterCriteriaErrorTypeDef:
    return {
        "ErrorCode": ...,
    }


# FilterCriteriaErrorTypeDef definition

class FilterCriteriaErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## SelfManagedEventSourceOutputTypeDef

```python
# SelfManagedEventSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import SelfManagedEventSourceOutputTypeDef


def get_value() -> SelfManagedEventSourceOutputTypeDef:
    return {
        "Endpoints": ...,
    }


# SelfManagedEventSourceOutputTypeDef definition

class SelfManagedEventSourceOutputTypeDef(TypedDict):
    Endpoints: NotRequired[Dict[EndPointTypeType, List[str]]],  # (1)
```

1. See [:material-code-brackets: EndPointTypeType](./literals.md#endpointtypetype) 
## EventSourceMappingMetricsConfigTypeDef

```python
# EventSourceMappingMetricsConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import EventSourceMappingMetricsConfigTypeDef


def get_value() -> EventSourceMappingMetricsConfigTypeDef:
    return {
        "Metrics": ...,
    }


# EventSourceMappingMetricsConfigTypeDef definition

class EventSourceMappingMetricsConfigTypeDef(TypedDict):
    Metrics: NotRequired[Sequence[EventSourceMappingMetricType]],  # (1)
```

1. See [:material-code-brackets: EventSourceMappingMetricType](./literals.md#eventsourcemappingmetrictype) 
## FilterTypeDef

```python
# FilterTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import FilterTypeDef


def get_value() -> FilterTypeDef:
    return {
        "Pattern": ...,
    }


# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Pattern: NotRequired[str],
```

## FunctionCodeLocationTypeDef

```python
# FunctionCodeLocationTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import FunctionCodeLocationTypeDef


def get_value() -> FunctionCodeLocationTypeDef:
    return {
        "RepositoryType": ...,
    }


# FunctionCodeLocationTypeDef definition

class FunctionCodeLocationTypeDef(TypedDict):
    RepositoryType: NotRequired[str],
    Location: NotRequired[str],
    ImageUri: NotRequired[str],
    ResolvedImageUri: NotRequired[str],
    SourceKMSKeyArn: NotRequired[str],
```

## LayerTypeDef

```python
# LayerTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import LayerTypeDef


def get_value() -> LayerTypeDef:
    return {
        "Arn": ...,
    }


# LayerTypeDef definition

class LayerTypeDef(TypedDict):
    Arn: NotRequired[str],
    CodeSize: NotRequired[int],
    SigningProfileVersionArn: NotRequired[str],
    SigningJobArn: NotRequired[str],
```

## SnapStartResponseTypeDef

```python
# SnapStartResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import SnapStartResponseTypeDef


def get_value() -> SnapStartResponseTypeDef:
    return {
        "ApplyOn": ...,
    }


# SnapStartResponseTypeDef definition

class SnapStartResponseTypeDef(TypedDict):
    ApplyOn: NotRequired[SnapStartApplyOnType],  # (1)
    OptimizationStatus: NotRequired[SnapStartOptimizationStatusType],  # (2)
```

1. See [:material-code-brackets: SnapStartApplyOnType](./literals.md#snapstartapplyontype) 
2. See [:material-code-brackets: SnapStartOptimizationStatusType](./literals.md#snapstartoptimizationstatustype) 
## TracingConfigResponseTypeDef

```python
# TracingConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import TracingConfigResponseTypeDef


def get_value() -> TracingConfigResponseTypeDef:
    return {
        "Mode": ...,
    }


# TracingConfigResponseTypeDef definition

class TracingConfigResponseTypeDef(TypedDict):
    Mode: NotRequired[TracingModeType],  # (1)
```

1. See [:material-code-brackets: TracingModeType](./literals.md#tracingmodetype) 
## VpcConfigResponseTypeDef

```python
# VpcConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import VpcConfigResponseTypeDef


def get_value() -> VpcConfigResponseTypeDef:
    return {
        "SubnetIds": ...,
    }


# VpcConfigResponseTypeDef definition

class VpcConfigResponseTypeDef(TypedDict):
    SubnetIds: NotRequired[List[str]],
    SecurityGroupIds: NotRequired[List[str]],
    VpcId: NotRequired[str],
    Ipv6AllowedForDualStack: NotRequired[bool],
```

## GetAliasRequestTypeDef

```python
# GetAliasRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetAliasRequestTypeDef


def get_value() -> GetAliasRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# GetAliasRequestTypeDef definition

class GetAliasRequestTypeDef(TypedDict):
    FunctionName: str,
    Name: str,
```

## GetCodeSigningConfigRequestTypeDef

```python
# GetCodeSigningConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetCodeSigningConfigRequestTypeDef


def get_value() -> GetCodeSigningConfigRequestTypeDef:
    return {
        "CodeSigningConfigArn": ...,
    }


# GetCodeSigningConfigRequestTypeDef definition

class GetCodeSigningConfigRequestTypeDef(TypedDict):
    CodeSigningConfigArn: str,
```

## GetEventSourceMappingRequestTypeDef

```python
# GetEventSourceMappingRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetEventSourceMappingRequestTypeDef


def get_value() -> GetEventSourceMappingRequestTypeDef:
    return {
        "UUID": ...,
    }


# GetEventSourceMappingRequestTypeDef definition

class GetEventSourceMappingRequestTypeDef(TypedDict):
    UUID: str,
```

## GetFunctionCodeSigningConfigRequestTypeDef

```python
# GetFunctionCodeSigningConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionCodeSigningConfigRequestTypeDef


def get_value() -> GetFunctionCodeSigningConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# GetFunctionCodeSigningConfigRequestTypeDef definition

class GetFunctionCodeSigningConfigRequestTypeDef(TypedDict):
    FunctionName: str,
```

## GetFunctionConcurrencyRequestTypeDef

```python
# GetFunctionConcurrencyRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionConcurrencyRequestTypeDef


def get_value() -> GetFunctionConcurrencyRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# GetFunctionConcurrencyRequestTypeDef definition

class GetFunctionConcurrencyRequestTypeDef(TypedDict):
    FunctionName: str,
```

## GetFunctionConfigurationRequestTypeDef

```python
# GetFunctionConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionConfigurationRequestTypeDef


def get_value() -> GetFunctionConfigurationRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# GetFunctionConfigurationRequestTypeDef definition

class GetFunctionConfigurationRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## GetFunctionEventInvokeConfigRequestTypeDef

```python
# GetFunctionEventInvokeConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionEventInvokeConfigRequestTypeDef


def get_value() -> GetFunctionEventInvokeConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# GetFunctionEventInvokeConfigRequestTypeDef definition

class GetFunctionEventInvokeConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## GetFunctionRecursionConfigRequestTypeDef

```python
# GetFunctionRecursionConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionRecursionConfigRequestTypeDef


def get_value() -> GetFunctionRecursionConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# GetFunctionRecursionConfigRequestTypeDef definition

class GetFunctionRecursionConfigRequestTypeDef(TypedDict):
    FunctionName: str,
```

## GetFunctionRequestTypeDef

```python
# GetFunctionRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionRequestTypeDef


def get_value() -> GetFunctionRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# GetFunctionRequestTypeDef definition

class GetFunctionRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## TagsErrorTypeDef

```python
# TagsErrorTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import TagsErrorTypeDef


def get_value() -> TagsErrorTypeDef:
    return {
        "ErrorCode": ...,
    }


# TagsErrorTypeDef definition

class TagsErrorTypeDef(TypedDict):
    ErrorCode: str,
    Message: str,
```

## GetFunctionUrlConfigRequestTypeDef

```python
# GetFunctionUrlConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionUrlConfigRequestTypeDef


def get_value() -> GetFunctionUrlConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# GetFunctionUrlConfigRequestTypeDef definition

class GetFunctionUrlConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## GetLayerVersionByArnRequestTypeDef

```python
# GetLayerVersionByArnRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetLayerVersionByArnRequestTypeDef


def get_value() -> GetLayerVersionByArnRequestTypeDef:
    return {
        "Arn": ...,
    }


# GetLayerVersionByArnRequestTypeDef definition

class GetLayerVersionByArnRequestTypeDef(TypedDict):
    Arn: str,
```

## GetLayerVersionPolicyRequestTypeDef

```python
# GetLayerVersionPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetLayerVersionPolicyRequestTypeDef


def get_value() -> GetLayerVersionPolicyRequestTypeDef:
    return {
        "LayerName": ...,
    }


# GetLayerVersionPolicyRequestTypeDef definition

class GetLayerVersionPolicyRequestTypeDef(TypedDict):
    LayerName: str,
    VersionNumber: int,
```

## GetLayerVersionRequestTypeDef

```python
# GetLayerVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetLayerVersionRequestTypeDef


def get_value() -> GetLayerVersionRequestTypeDef:
    return {
        "LayerName": ...,
    }


# GetLayerVersionRequestTypeDef definition

class GetLayerVersionRequestTypeDef(TypedDict):
    LayerName: str,
    VersionNumber: int,
```

## LayerVersionContentOutputTypeDef

```python
# LayerVersionContentOutputTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import LayerVersionContentOutputTypeDef


def get_value() -> LayerVersionContentOutputTypeDef:
    return {
        "Location": ...,
    }


# LayerVersionContentOutputTypeDef definition

class LayerVersionContentOutputTypeDef(TypedDict):
    Location: NotRequired[str],
    CodeSha256: NotRequired[str],
    CodeSize: NotRequired[int],
    SigningProfileVersionArn: NotRequired[str],
    SigningJobArn: NotRequired[str],
```

## GetPolicyRequestTypeDef

```python
# GetPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetPolicyRequestTypeDef


def get_value() -> GetPolicyRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# GetPolicyRequestTypeDef definition

class GetPolicyRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## GetProvisionedConcurrencyConfigRequestTypeDef

```python
# GetProvisionedConcurrencyConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetProvisionedConcurrencyConfigRequestTypeDef


def get_value() -> GetProvisionedConcurrencyConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# GetProvisionedConcurrencyConfigRequestTypeDef definition

class GetProvisionedConcurrencyConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: str,
```

## GetRuntimeManagementConfigRequestTypeDef

```python
# GetRuntimeManagementConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetRuntimeManagementConfigRequestTypeDef


def get_value() -> GetRuntimeManagementConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# GetRuntimeManagementConfigRequestTypeDef definition

class GetRuntimeManagementConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## ImageConfigErrorTypeDef

```python
# ImageConfigErrorTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ImageConfigErrorTypeDef


def get_value() -> ImageConfigErrorTypeDef:
    return {
        "ErrorCode": ...,
    }


# ImageConfigErrorTypeDef definition

class ImageConfigErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## ImageConfigOutputTypeDef

```python
# ImageConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ImageConfigOutputTypeDef


def get_value() -> ImageConfigOutputTypeDef:
    return {
        "EntryPoint": ...,
    }


# ImageConfigOutputTypeDef definition

class ImageConfigOutputTypeDef(TypedDict):
    EntryPoint: NotRequired[List[str]],
    Command: NotRequired[List[str]],
    WorkingDirectory: NotRequired[str],
```

## ImageConfigTypeDef

```python
# ImageConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ImageConfigTypeDef


def get_value() -> ImageConfigTypeDef:
    return {
        "EntryPoint": ...,
    }


# ImageConfigTypeDef definition

class ImageConfigTypeDef(TypedDict):
    EntryPoint: NotRequired[Sequence[str]],
    Command: NotRequired[Sequence[str]],
    WorkingDirectory: NotRequired[str],
```

## InvokeResponseStreamUpdateTypeDef

```python
# InvokeResponseStreamUpdateTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import InvokeResponseStreamUpdateTypeDef


def get_value() -> InvokeResponseStreamUpdateTypeDef:
    return {
        "Payload": ...,
    }


# InvokeResponseStreamUpdateTypeDef definition

class InvokeResponseStreamUpdateTypeDef(TypedDict):
    Payload: NotRequired[bytes],
```

## InvokeWithResponseStreamCompleteEventTypeDef

```python
# InvokeWithResponseStreamCompleteEventTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import InvokeWithResponseStreamCompleteEventTypeDef


def get_value() -> InvokeWithResponseStreamCompleteEventTypeDef:
    return {
        "ErrorCode": ...,
    }


# InvokeWithResponseStreamCompleteEventTypeDef definition

class InvokeWithResponseStreamCompleteEventTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorDetails: NotRequired[str],
    LogResult: NotRequired[str],
```

## LayerVersionsListItemTypeDef

```python
# LayerVersionsListItemTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import LayerVersionsListItemTypeDef


def get_value() -> LayerVersionsListItemTypeDef:
    return {
        "LayerVersionArn": ...,
    }


# LayerVersionsListItemTypeDef definition

class LayerVersionsListItemTypeDef(TypedDict):
    LayerVersionArn: NotRequired[str],
    Version: NotRequired[int],
    Description: NotRequired[str],
    CreatedDate: NotRequired[str],
    CompatibleRuntimes: NotRequired[List[RuntimeType]],  # (1)
    LicenseInfo: NotRequired[str],
    CompatibleArchitectures: NotRequired[List[ArchitectureType]],  # (2)
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PaginatorConfigTypeDef


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

## ListAliasesRequestTypeDef

```python
# ListAliasesRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListAliasesRequestTypeDef


def get_value() -> ListAliasesRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# ListAliasesRequestTypeDef definition

class ListAliasesRequestTypeDef(TypedDict):
    FunctionName: str,
    FunctionVersion: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListCodeSigningConfigsRequestTypeDef

```python
# ListCodeSigningConfigsRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListCodeSigningConfigsRequestTypeDef


def get_value() -> ListCodeSigningConfigsRequestTypeDef:
    return {
        "Marker": ...,
    }


# ListCodeSigningConfigsRequestTypeDef definition

class ListCodeSigningConfigsRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListEventSourceMappingsRequestTypeDef

```python
# ListEventSourceMappingsRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListEventSourceMappingsRequestTypeDef


def get_value() -> ListEventSourceMappingsRequestTypeDef:
    return {
        "EventSourceArn": ...,
    }


# ListEventSourceMappingsRequestTypeDef definition

class ListEventSourceMappingsRequestTypeDef(TypedDict):
    EventSourceArn: NotRequired[str],
    FunctionName: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListFunctionEventInvokeConfigsRequestTypeDef

```python
# ListFunctionEventInvokeConfigsRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListFunctionEventInvokeConfigsRequestTypeDef


def get_value() -> ListFunctionEventInvokeConfigsRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# ListFunctionEventInvokeConfigsRequestTypeDef definition

class ListFunctionEventInvokeConfigsRequestTypeDef(TypedDict):
    FunctionName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListFunctionUrlConfigsRequestTypeDef

```python
# ListFunctionUrlConfigsRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListFunctionUrlConfigsRequestTypeDef


def get_value() -> ListFunctionUrlConfigsRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# ListFunctionUrlConfigsRequestTypeDef definition

class ListFunctionUrlConfigsRequestTypeDef(TypedDict):
    FunctionName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListFunctionsByCodeSigningConfigRequestTypeDef

```python
# ListFunctionsByCodeSigningConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListFunctionsByCodeSigningConfigRequestTypeDef


def get_value() -> ListFunctionsByCodeSigningConfigRequestTypeDef:
    return {
        "CodeSigningConfigArn": ...,
    }


# ListFunctionsByCodeSigningConfigRequestTypeDef definition

class ListFunctionsByCodeSigningConfigRequestTypeDef(TypedDict):
    CodeSigningConfigArn: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListFunctionsRequestTypeDef

```python
# ListFunctionsRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListFunctionsRequestTypeDef


def get_value() -> ListFunctionsRequestTypeDef:
    return {
        "MasterRegion": ...,
    }


# ListFunctionsRequestTypeDef definition

class ListFunctionsRequestTypeDef(TypedDict):
    MasterRegion: NotRequired[str],
    FunctionVersion: NotRequired[FunctionVersionType],  # (1)
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

1. See [:material-code-brackets: FunctionVersionType](./literals.md#functionversiontype) 
## ListLayerVersionsRequestTypeDef

```python
# ListLayerVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListLayerVersionsRequestTypeDef


def get_value() -> ListLayerVersionsRequestTypeDef:
    return {
        "LayerName": ...,
    }


# ListLayerVersionsRequestTypeDef definition

class ListLayerVersionsRequestTypeDef(TypedDict):
    LayerName: str,
    CompatibleRuntime: NotRequired[RuntimeType],  # (1)
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
    CompatibleArchitecture: NotRequired[ArchitectureType],  # (2)
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## ListLayersRequestTypeDef

```python
# ListLayersRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListLayersRequestTypeDef


def get_value() -> ListLayersRequestTypeDef:
    return {
        "CompatibleRuntime": ...,
    }


# ListLayersRequestTypeDef definition

class ListLayersRequestTypeDef(TypedDict):
    CompatibleRuntime: NotRequired[RuntimeType],  # (1)
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
    CompatibleArchitecture: NotRequired[ArchitectureType],  # (2)
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## ListProvisionedConcurrencyConfigsRequestTypeDef

```python
# ListProvisionedConcurrencyConfigsRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListProvisionedConcurrencyConfigsRequestTypeDef


def get_value() -> ListProvisionedConcurrencyConfigsRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# ListProvisionedConcurrencyConfigsRequestTypeDef definition

class ListProvisionedConcurrencyConfigsRequestTypeDef(TypedDict):
    FunctionName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ProvisionedConcurrencyConfigListItemTypeDef

```python
# ProvisionedConcurrencyConfigListItemTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ProvisionedConcurrencyConfigListItemTypeDef


def get_value() -> ProvisionedConcurrencyConfigListItemTypeDef:
    return {
        "FunctionArn": ...,
    }


# ProvisionedConcurrencyConfigListItemTypeDef definition

class ProvisionedConcurrencyConfigListItemTypeDef(TypedDict):
    FunctionArn: NotRequired[str],
    RequestedProvisionedConcurrentExecutions: NotRequired[int],
    AvailableProvisionedConcurrentExecutions: NotRequired[int],
    AllocatedProvisionedConcurrentExecutions: NotRequired[int],
    Status: NotRequired[ProvisionedConcurrencyStatusEnumType],  # (1)
    StatusReason: NotRequired[str],
    LastModified: NotRequired[str],
```

1. See [:material-code-brackets: ProvisionedConcurrencyStatusEnumType](./literals.md#provisionedconcurrencystatusenumtype) 
## ListTagsRequestTypeDef

```python
# ListTagsRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListTagsRequestTypeDef


def get_value() -> ListTagsRequestTypeDef:
    return {
        "Resource": ...,
    }


# ListTagsRequestTypeDef definition

class ListTagsRequestTypeDef(TypedDict):
    Resource: str,
```

## ListVersionsByFunctionRequestTypeDef

```python
# ListVersionsByFunctionRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListVersionsByFunctionRequestTypeDef


def get_value() -> ListVersionsByFunctionRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# ListVersionsByFunctionRequestTypeDef definition

class ListVersionsByFunctionRequestTypeDef(TypedDict):
    FunctionName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## PublishVersionRequestTypeDef

```python
# PublishVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PublishVersionRequestTypeDef


def get_value() -> PublishVersionRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# PublishVersionRequestTypeDef definition

class PublishVersionRequestTypeDef(TypedDict):
    FunctionName: str,
    CodeSha256: NotRequired[str],
    Description: NotRequired[str],
    RevisionId: NotRequired[str],
```

## PutFunctionCodeSigningConfigRequestTypeDef

```python
# PutFunctionCodeSigningConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PutFunctionCodeSigningConfigRequestTypeDef


def get_value() -> PutFunctionCodeSigningConfigRequestTypeDef:
    return {
        "CodeSigningConfigArn": ...,
    }


# PutFunctionCodeSigningConfigRequestTypeDef definition

class PutFunctionCodeSigningConfigRequestTypeDef(TypedDict):
    CodeSigningConfigArn: str,
    FunctionName: str,
```

## PutFunctionConcurrencyRequestTypeDef

```python
# PutFunctionConcurrencyRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PutFunctionConcurrencyRequestTypeDef


def get_value() -> PutFunctionConcurrencyRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# PutFunctionConcurrencyRequestTypeDef definition

class PutFunctionConcurrencyRequestTypeDef(TypedDict):
    FunctionName: str,
    ReservedConcurrentExecutions: int,
```

## PutFunctionRecursionConfigRequestTypeDef

```python
# PutFunctionRecursionConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PutFunctionRecursionConfigRequestTypeDef


def get_value() -> PutFunctionRecursionConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# PutFunctionRecursionConfigRequestTypeDef definition

class PutFunctionRecursionConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    RecursiveLoop: RecursiveLoopType,  # (1)
```

1. See [:material-code-brackets: RecursiveLoopType](./literals.md#recursivelooptype) 
## PutProvisionedConcurrencyConfigRequestTypeDef

```python
# PutProvisionedConcurrencyConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PutProvisionedConcurrencyConfigRequestTypeDef


def get_value() -> PutProvisionedConcurrencyConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# PutProvisionedConcurrencyConfigRequestTypeDef definition

class PutProvisionedConcurrencyConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: str,
    ProvisionedConcurrentExecutions: int,
```

## PutRuntimeManagementConfigRequestTypeDef

```python
# PutRuntimeManagementConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PutRuntimeManagementConfigRequestTypeDef


def get_value() -> PutRuntimeManagementConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# PutRuntimeManagementConfigRequestTypeDef definition

class PutRuntimeManagementConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    UpdateRuntimeOn: UpdateRuntimeOnType,  # (1)
    Qualifier: NotRequired[str],
    RuntimeVersionArn: NotRequired[str],
```

1. See [:material-code-brackets: UpdateRuntimeOnType](./literals.md#updateruntimeontype) 
## RemoveLayerVersionPermissionRequestTypeDef

```python
# RemoveLayerVersionPermissionRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import RemoveLayerVersionPermissionRequestTypeDef


def get_value() -> RemoveLayerVersionPermissionRequestTypeDef:
    return {
        "LayerName": ...,
    }


# RemoveLayerVersionPermissionRequestTypeDef definition

class RemoveLayerVersionPermissionRequestTypeDef(TypedDict):
    LayerName: str,
    VersionNumber: int,
    StatementId: str,
    RevisionId: NotRequired[str],
```

## RemovePermissionRequestTypeDef

```python
# RemovePermissionRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import RemovePermissionRequestTypeDef


def get_value() -> RemovePermissionRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# RemovePermissionRequestTypeDef definition

class RemovePermissionRequestTypeDef(TypedDict):
    FunctionName: str,
    StatementId: str,
    Qualifier: NotRequired[str],
    RevisionId: NotRequired[str],
```

## RuntimeVersionErrorTypeDef

```python
# RuntimeVersionErrorTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import RuntimeVersionErrorTypeDef


def get_value() -> RuntimeVersionErrorTypeDef:
    return {
        "ErrorCode": ...,
    }


# RuntimeVersionErrorTypeDef definition

class RuntimeVersionErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## SelfManagedEventSourceTypeDef

```python
# SelfManagedEventSourceTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import SelfManagedEventSourceTypeDef


def get_value() -> SelfManagedEventSourceTypeDef:
    return {
        "Endpoints": ...,
    }


# SelfManagedEventSourceTypeDef definition

class SelfManagedEventSourceTypeDef(TypedDict):
    Endpoints: NotRequired[Mapping[EndPointTypeType, Sequence[str]]],  # (1)
```

1. See [:material-code-brackets: EndPointTypeType](./literals.md#endpointtypetype) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "Resource": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    Resource: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "Resource": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    Resource: str,
    TagKeys: Sequence[str],
```

## AddLayerVersionPermissionResponseTypeDef

```python
# AddLayerVersionPermissionResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import AddLayerVersionPermissionResponseTypeDef


def get_value() -> AddLayerVersionPermissionResponseTypeDef:
    return {
        "Statement": ...,
    }


# AddLayerVersionPermissionResponseTypeDef definition

class AddLayerVersionPermissionResponseTypeDef(TypedDict):
    Statement: str,
    RevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddPermissionResponseTypeDef

```python
# AddPermissionResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import AddPermissionResponseTypeDef


def get_value() -> AddPermissionResponseTypeDef:
    return {
        "Statement": ...,
    }


# AddPermissionResponseTypeDef definition

class AddPermissionResponseTypeDef(TypedDict):
    Statement: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConcurrencyResponseTypeDef

```python
# ConcurrencyResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ConcurrencyResponseTypeDef


def get_value() -> ConcurrencyResponseTypeDef:
    return {
        "ReservedConcurrentExecutions": ...,
    }


# ConcurrencyResponseTypeDef definition

class ConcurrencyResponseTypeDef(TypedDict):
    ReservedConcurrentExecutions: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountSettingsResponseTypeDef

```python
# GetAccountSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetAccountSettingsResponseTypeDef


def get_value() -> GetAccountSettingsResponseTypeDef:
    return {
        "AccountLimit": ...,
    }


# GetAccountSettingsResponseTypeDef definition

class GetAccountSettingsResponseTypeDef(TypedDict):
    AccountLimit: AccountLimitTypeDef,  # (1)
    AccountUsage: AccountUsageTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AccountLimitTypeDef](./type_defs.md#accountlimittypedef) 
2. See [:material-code-braces: AccountUsageTypeDef](./type_defs.md#accountusagetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFunctionCodeSigningConfigResponseTypeDef

```python
# GetFunctionCodeSigningConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionCodeSigningConfigResponseTypeDef


def get_value() -> GetFunctionCodeSigningConfigResponseTypeDef:
    return {
        "CodeSigningConfigArn": ...,
    }


# GetFunctionCodeSigningConfigResponseTypeDef definition

class GetFunctionCodeSigningConfigResponseTypeDef(TypedDict):
    CodeSigningConfigArn: str,
    FunctionName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFunctionConcurrencyResponseTypeDef

```python
# GetFunctionConcurrencyResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionConcurrencyResponseTypeDef


def get_value() -> GetFunctionConcurrencyResponseTypeDef:
    return {
        "ReservedConcurrentExecutions": ...,
    }


# GetFunctionConcurrencyResponseTypeDef definition

class GetFunctionConcurrencyResponseTypeDef(TypedDict):
    ReservedConcurrentExecutions: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFunctionRecursionConfigResponseTypeDef

```python
# GetFunctionRecursionConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionRecursionConfigResponseTypeDef


def get_value() -> GetFunctionRecursionConfigResponseTypeDef:
    return {
        "RecursiveLoop": ...,
    }


# GetFunctionRecursionConfigResponseTypeDef definition

class GetFunctionRecursionConfigResponseTypeDef(TypedDict):
    RecursiveLoop: RecursiveLoopType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RecursiveLoopType](./literals.md#recursivelooptype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLayerVersionPolicyResponseTypeDef

```python
# GetLayerVersionPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetLayerVersionPolicyResponseTypeDef


def get_value() -> GetLayerVersionPolicyResponseTypeDef:
    return {
        "Policy": ...,
    }


# GetLayerVersionPolicyResponseTypeDef definition

class GetLayerVersionPolicyResponseTypeDef(TypedDict):
    Policy: str,
    RevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPolicyResponseTypeDef

```python
# GetPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetPolicyResponseTypeDef


def get_value() -> GetPolicyResponseTypeDef:
    return {
        "Policy": ...,
    }


# GetPolicyResponseTypeDef definition

class GetPolicyResponseTypeDef(TypedDict):
    Policy: str,
    RevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProvisionedConcurrencyConfigResponseTypeDef

```python
# GetProvisionedConcurrencyConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetProvisionedConcurrencyConfigResponseTypeDef


def get_value() -> GetProvisionedConcurrencyConfigResponseTypeDef:
    return {
        "RequestedProvisionedConcurrentExecutions": ...,
    }


# GetProvisionedConcurrencyConfigResponseTypeDef definition

class GetProvisionedConcurrencyConfigResponseTypeDef(TypedDict):
    RequestedProvisionedConcurrentExecutions: int,
    AvailableProvisionedConcurrentExecutions: int,
    AllocatedProvisionedConcurrentExecutions: int,
    Status: ProvisionedConcurrencyStatusEnumType,  # (1)
    StatusReason: str,
    LastModified: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ProvisionedConcurrencyStatusEnumType](./literals.md#provisionedconcurrencystatusenumtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRuntimeManagementConfigResponseTypeDef

```python
# GetRuntimeManagementConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetRuntimeManagementConfigResponseTypeDef


def get_value() -> GetRuntimeManagementConfigResponseTypeDef:
    return {
        "UpdateRuntimeOn": ...,
    }


# GetRuntimeManagementConfigResponseTypeDef definition

class GetRuntimeManagementConfigResponseTypeDef(TypedDict):
    UpdateRuntimeOn: UpdateRuntimeOnType,  # (1)
    RuntimeVersionArn: str,
    FunctionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: UpdateRuntimeOnType](./literals.md#updateruntimeontype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvocationResponseTypeDef

```python
# InvocationResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import InvocationResponseTypeDef


def get_value() -> InvocationResponseTypeDef:
    return {
        "StatusCode": ...,
    }


# InvocationResponseTypeDef definition

class InvocationResponseTypeDef(TypedDict):
    StatusCode: int,
    FunctionError: str,
    LogResult: str,
    Payload: StreamingBody,
    ExecutedVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvokeAsyncResponseTypeDef

```python
# InvokeAsyncResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import InvokeAsyncResponseTypeDef


def get_value() -> InvokeAsyncResponseTypeDef:
    return {
        "Status": ...,
    }


# InvokeAsyncResponseTypeDef definition

class InvokeAsyncResponseTypeDef(TypedDict):
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFunctionsByCodeSigningConfigResponseTypeDef

```python
# ListFunctionsByCodeSigningConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListFunctionsByCodeSigningConfigResponseTypeDef


def get_value() -> ListFunctionsByCodeSigningConfigResponseTypeDef:
    return {
        "NextMarker": ...,
    }


# ListFunctionsByCodeSigningConfigResponseTypeDef definition

class ListFunctionsByCodeSigningConfigResponseTypeDef(TypedDict):
    NextMarker: str,
    FunctionArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsResponseTypeDef

```python
# ListTagsResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListTagsResponseTypeDef


def get_value() -> ListTagsResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsResponseTypeDef definition

class ListTagsResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutFunctionCodeSigningConfigResponseTypeDef

```python
# PutFunctionCodeSigningConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PutFunctionCodeSigningConfigResponseTypeDef


def get_value() -> PutFunctionCodeSigningConfigResponseTypeDef:
    return {
        "CodeSigningConfigArn": ...,
    }


# PutFunctionCodeSigningConfigResponseTypeDef definition

class PutFunctionCodeSigningConfigResponseTypeDef(TypedDict):
    CodeSigningConfigArn: str,
    FunctionName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutFunctionRecursionConfigResponseTypeDef

```python
# PutFunctionRecursionConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PutFunctionRecursionConfigResponseTypeDef


def get_value() -> PutFunctionRecursionConfigResponseTypeDef:
    return {
        "RecursiveLoop": ...,
    }


# PutFunctionRecursionConfigResponseTypeDef definition

class PutFunctionRecursionConfigResponseTypeDef(TypedDict):
    RecursiveLoop: RecursiveLoopType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RecursiveLoopType](./literals.md#recursivelooptype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutProvisionedConcurrencyConfigResponseTypeDef

```python
# PutProvisionedConcurrencyConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PutProvisionedConcurrencyConfigResponseTypeDef


def get_value() -> PutProvisionedConcurrencyConfigResponseTypeDef:
    return {
        "RequestedProvisionedConcurrentExecutions": ...,
    }


# PutProvisionedConcurrencyConfigResponseTypeDef definition

class PutProvisionedConcurrencyConfigResponseTypeDef(TypedDict):
    RequestedProvisionedConcurrentExecutions: int,
    AvailableProvisionedConcurrentExecutions: int,
    AllocatedProvisionedConcurrentExecutions: int,
    Status: ProvisionedConcurrencyStatusEnumType,  # (1)
    StatusReason: str,
    LastModified: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ProvisionedConcurrencyStatusEnumType](./literals.md#provisionedconcurrencystatusenumtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRuntimeManagementConfigResponseTypeDef

```python
# PutRuntimeManagementConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PutRuntimeManagementConfigResponseTypeDef


def get_value() -> PutRuntimeManagementConfigResponseTypeDef:
    return {
        "UpdateRuntimeOn": ...,
    }


# PutRuntimeManagementConfigResponseTypeDef definition

class PutRuntimeManagementConfigResponseTypeDef(TypedDict):
    UpdateRuntimeOn: UpdateRuntimeOnType,  # (1)
    FunctionArn: str,
    RuntimeVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: UpdateRuntimeOnType](./literals.md#updateruntimeontype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AliasConfigurationResponseTypeDef

```python
# AliasConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import AliasConfigurationResponseTypeDef


def get_value() -> AliasConfigurationResponseTypeDef:
    return {
        "AliasArn": ...,
    }


# AliasConfigurationResponseTypeDef definition

class AliasConfigurationResponseTypeDef(TypedDict):
    AliasArn: str,
    Name: str,
    FunctionVersion: str,
    Description: str,
    RoutingConfig: AliasRoutingConfigurationOutputTypeDef,  # (1)
    RevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AliasRoutingConfigurationOutputTypeDef](./type_defs.md#aliasroutingconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AliasConfigurationTypeDef

```python
# AliasConfigurationTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import AliasConfigurationTypeDef


def get_value() -> AliasConfigurationTypeDef:
    return {
        "AliasArn": ...,
    }


# AliasConfigurationTypeDef definition

class AliasConfigurationTypeDef(TypedDict):
    AliasArn: NotRequired[str],
    Name: NotRequired[str],
    FunctionVersion: NotRequired[str],
    Description: NotRequired[str],
    RoutingConfig: NotRequired[AliasRoutingConfigurationOutputTypeDef],  # (1)
    RevisionId: NotRequired[str],
```

1. See [:material-code-braces: AliasRoutingConfigurationOutputTypeDef](./type_defs.md#aliasroutingconfigurationoutputtypedef) 
## FunctionCodeTypeDef

```python
# FunctionCodeTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import FunctionCodeTypeDef


def get_value() -> FunctionCodeTypeDef:
    return {
        "ZipFile": ...,
    }


# FunctionCodeTypeDef definition

class FunctionCodeTypeDef(TypedDict):
    ZipFile: NotRequired[BlobTypeDef],
    S3Bucket: NotRequired[str],
    S3Key: NotRequired[str],
    S3ObjectVersion: NotRequired[str],
    ImageUri: NotRequired[str],
    SourceKMSKeyArn: NotRequired[str],
```

## InvocationRequestTypeDef

```python
# InvocationRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import InvocationRequestTypeDef


def get_value() -> InvocationRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# InvocationRequestTypeDef definition

class InvocationRequestTypeDef(TypedDict):
    FunctionName: str,
    InvocationType: NotRequired[InvocationTypeType],  # (1)
    LogType: NotRequired[LogTypeType],  # (2)
    ClientContext: NotRequired[str],
    Payload: NotRequired[BlobTypeDef],
    Qualifier: NotRequired[str],
```

1. See [:material-code-brackets: InvocationTypeType](./literals.md#invocationtypetype) 
2. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
## InvokeAsyncRequestTypeDef

```python
# InvokeAsyncRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import InvokeAsyncRequestTypeDef


def get_value() -> InvokeAsyncRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# InvokeAsyncRequestTypeDef definition

class InvokeAsyncRequestTypeDef(TypedDict):
    FunctionName: str,
    InvokeArgs: BlobTypeDef,
```

## InvokeWithResponseStreamRequestTypeDef

```python
# InvokeWithResponseStreamRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import InvokeWithResponseStreamRequestTypeDef


def get_value() -> InvokeWithResponseStreamRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# InvokeWithResponseStreamRequestTypeDef definition

class InvokeWithResponseStreamRequestTypeDef(TypedDict):
    FunctionName: str,
    InvocationType: NotRequired[ResponseStreamingInvocationTypeType],  # (1)
    LogType: NotRequired[LogTypeType],  # (2)
    ClientContext: NotRequired[str],
    Qualifier: NotRequired[str],
    Payload: NotRequired[BlobTypeDef],
```

1. See [:material-code-brackets: ResponseStreamingInvocationTypeType](./literals.md#responsestreaminginvocationtypetype) 
2. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
## LayerVersionContentInputTypeDef

```python
# LayerVersionContentInputTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import LayerVersionContentInputTypeDef


def get_value() -> LayerVersionContentInputTypeDef:
    return {
        "S3Bucket": ...,
    }


# LayerVersionContentInputTypeDef definition

class LayerVersionContentInputTypeDef(TypedDict):
    S3Bucket: NotRequired[str],
    S3Key: NotRequired[str],
    S3ObjectVersion: NotRequired[str],
    ZipFile: NotRequired[BlobTypeDef],
```

## UpdateFunctionCodeRequestTypeDef

```python
# UpdateFunctionCodeRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import UpdateFunctionCodeRequestTypeDef


def get_value() -> UpdateFunctionCodeRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# UpdateFunctionCodeRequestTypeDef definition

class UpdateFunctionCodeRequestTypeDef(TypedDict):
    FunctionName: str,
    ZipFile: NotRequired[BlobTypeDef],
    S3Bucket: NotRequired[str],
    S3Key: NotRequired[str],
    S3ObjectVersion: NotRequired[str],
    ImageUri: NotRequired[str],
    Publish: NotRequired[bool],
    DryRun: NotRequired[bool],
    RevisionId: NotRequired[str],
    Architectures: NotRequired[Sequence[ArchitectureType]],  # (1)
    SourceKMSKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## CodeSigningConfigTypeDef

```python
# CodeSigningConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import CodeSigningConfigTypeDef


def get_value() -> CodeSigningConfigTypeDef:
    return {
        "CodeSigningConfigId": ...,
    }


# CodeSigningConfigTypeDef definition

class CodeSigningConfigTypeDef(TypedDict):
    CodeSigningConfigId: str,
    CodeSigningConfigArn: str,
    AllowedPublishers: AllowedPublishersOutputTypeDef,  # (1)
    CodeSigningPolicies: CodeSigningPoliciesTypeDef,  # (2)
    LastModified: str,
    Description: NotRequired[str],
```

1. See [:material-code-braces: AllowedPublishersOutputTypeDef](./type_defs.md#allowedpublishersoutputtypedef) 
2. See [:material-code-braces: CodeSigningPoliciesTypeDef](./type_defs.md#codesigningpoliciestypedef) 
## CreateFunctionUrlConfigResponseTypeDef

```python
# CreateFunctionUrlConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import CreateFunctionUrlConfigResponseTypeDef


def get_value() -> CreateFunctionUrlConfigResponseTypeDef:
    return {
        "FunctionUrl": ...,
    }


# CreateFunctionUrlConfigResponseTypeDef definition

class CreateFunctionUrlConfigResponseTypeDef(TypedDict):
    FunctionUrl: str,
    FunctionArn: str,
    AuthType: FunctionUrlAuthTypeType,  # (1)
    Cors: CorsOutputTypeDef,  # (2)
    CreationTime: str,
    InvokeMode: InvokeModeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: FunctionUrlAuthTypeType](./literals.md#functionurlauthtypetype) 
2. See [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
3. See [:material-code-brackets: InvokeModeType](./literals.md#invokemodetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FunctionUrlConfigTypeDef

```python
# FunctionUrlConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import FunctionUrlConfigTypeDef


def get_value() -> FunctionUrlConfigTypeDef:
    return {
        "FunctionUrl": ...,
    }


# FunctionUrlConfigTypeDef definition

class FunctionUrlConfigTypeDef(TypedDict):
    FunctionUrl: str,
    FunctionArn: str,
    CreationTime: str,
    LastModifiedTime: str,
    AuthType: FunctionUrlAuthTypeType,  # (2)
    Cors: NotRequired[CorsOutputTypeDef],  # (1)
    InvokeMode: NotRequired[InvokeModeType],  # (3)
```

1. See [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
2. See [:material-code-brackets: FunctionUrlAuthTypeType](./literals.md#functionurlauthtypetype) 
3. See [:material-code-brackets: InvokeModeType](./literals.md#invokemodetype) 
## GetFunctionUrlConfigResponseTypeDef

```python
# GetFunctionUrlConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionUrlConfigResponseTypeDef


def get_value() -> GetFunctionUrlConfigResponseTypeDef:
    return {
        "FunctionUrl": ...,
    }


# GetFunctionUrlConfigResponseTypeDef definition

class GetFunctionUrlConfigResponseTypeDef(TypedDict):
    FunctionUrl: str,
    FunctionArn: str,
    AuthType: FunctionUrlAuthTypeType,  # (1)
    Cors: CorsOutputTypeDef,  # (2)
    CreationTime: str,
    LastModifiedTime: str,
    InvokeMode: InvokeModeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: FunctionUrlAuthTypeType](./literals.md#functionurlauthtypetype) 
2. See [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
3. See [:material-code-brackets: InvokeModeType](./literals.md#invokemodetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFunctionUrlConfigResponseTypeDef

```python
# UpdateFunctionUrlConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import UpdateFunctionUrlConfigResponseTypeDef


def get_value() -> UpdateFunctionUrlConfigResponseTypeDef:
    return {
        "FunctionUrl": ...,
    }


# UpdateFunctionUrlConfigResponseTypeDef definition

class UpdateFunctionUrlConfigResponseTypeDef(TypedDict):
    FunctionUrl: str,
    FunctionArn: str,
    AuthType: FunctionUrlAuthTypeType,  # (1)
    Cors: CorsOutputTypeDef,  # (2)
    CreationTime: str,
    LastModifiedTime: str,
    InvokeMode: InvokeModeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: FunctionUrlAuthTypeType](./literals.md#functionurlauthtypetype) 
2. See [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
3. See [:material-code-brackets: InvokeModeType](./literals.md#invokemodetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationConfigTypeDef

```python
# DestinationConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import DestinationConfigTypeDef


def get_value() -> DestinationConfigTypeDef:
    return {
        "OnSuccess": ...,
    }


# DestinationConfigTypeDef definition

class DestinationConfigTypeDef(TypedDict):
    OnSuccess: NotRequired[OnSuccessTypeDef],  # (1)
    OnFailure: NotRequired[OnFailureTypeDef],  # (2)
```

1. See [:material-code-braces: OnSuccessTypeDef](./type_defs.md#onsuccesstypedef) 
2. See [:material-code-braces: OnFailureTypeDef](./type_defs.md#onfailuretypedef) 
## EnvironmentResponseTypeDef

```python
# EnvironmentResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import EnvironmentResponseTypeDef


def get_value() -> EnvironmentResponseTypeDef:
    return {
        "Variables": ...,
    }


# EnvironmentResponseTypeDef definition

class EnvironmentResponseTypeDef(TypedDict):
    Variables: NotRequired[Dict[str, str]],
    Error: NotRequired[EnvironmentErrorTypeDef],  # (1)
```

1. See [:material-code-braces: EnvironmentErrorTypeDef](./type_defs.md#environmenterrortypedef) 
## FilterCriteriaOutputTypeDef

```python
# FilterCriteriaOutputTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import FilterCriteriaOutputTypeDef


def get_value() -> FilterCriteriaOutputTypeDef:
    return {
        "Filters": ...,
    }


# FilterCriteriaOutputTypeDef definition

class FilterCriteriaOutputTypeDef(TypedDict):
    Filters: NotRequired[List[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## FilterCriteriaTypeDef

```python
# FilterCriteriaTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import FilterCriteriaTypeDef


def get_value() -> FilterCriteriaTypeDef:
    return {
        "Filters": ...,
    }


# FilterCriteriaTypeDef definition

class FilterCriteriaTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## GetFunctionConfigurationRequestWaitExtraExtraTypeDef

```python
# GetFunctionConfigurationRequestWaitExtraExtraTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionConfigurationRequestWaitExtraExtraTypeDef


def get_value() -> GetFunctionConfigurationRequestWaitExtraExtraTypeDef:
    return {
        "FunctionName": ...,
    }


# GetFunctionConfigurationRequestWaitExtraExtraTypeDef definition

class GetFunctionConfigurationRequestWaitExtraExtraTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetFunctionConfigurationRequestWaitExtraTypeDef

```python
# GetFunctionConfigurationRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionConfigurationRequestWaitExtraTypeDef


def get_value() -> GetFunctionConfigurationRequestWaitExtraTypeDef:
    return {
        "FunctionName": ...,
    }


# GetFunctionConfigurationRequestWaitExtraTypeDef definition

class GetFunctionConfigurationRequestWaitExtraTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetFunctionConfigurationRequestWaitTypeDef

```python
# GetFunctionConfigurationRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionConfigurationRequestWaitTypeDef


def get_value() -> GetFunctionConfigurationRequestWaitTypeDef:
    return {
        "FunctionName": ...,
    }


# GetFunctionConfigurationRequestWaitTypeDef definition

class GetFunctionConfigurationRequestWaitTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetFunctionRequestWaitExtraExtraTypeDef

```python
# GetFunctionRequestWaitExtraExtraTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionRequestWaitExtraExtraTypeDef


def get_value() -> GetFunctionRequestWaitExtraExtraTypeDef:
    return {
        "FunctionName": ...,
    }


# GetFunctionRequestWaitExtraExtraTypeDef definition

class GetFunctionRequestWaitExtraExtraTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetFunctionRequestWaitExtraTypeDef

```python
# GetFunctionRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionRequestWaitExtraTypeDef


def get_value() -> GetFunctionRequestWaitExtraTypeDef:
    return {
        "FunctionName": ...,
    }


# GetFunctionRequestWaitExtraTypeDef definition

class GetFunctionRequestWaitExtraTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetFunctionRequestWaitTypeDef

```python
# GetFunctionRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionRequestWaitTypeDef


def get_value() -> GetFunctionRequestWaitTypeDef:
    return {
        "FunctionName": ...,
    }


# GetFunctionRequestWaitTypeDef definition

class GetFunctionRequestWaitTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetLayerVersionResponseTypeDef

```python
# GetLayerVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetLayerVersionResponseTypeDef


def get_value() -> GetLayerVersionResponseTypeDef:
    return {
        "Content": ...,
    }


# GetLayerVersionResponseTypeDef definition

class GetLayerVersionResponseTypeDef(TypedDict):
    Content: LayerVersionContentOutputTypeDef,  # (1)
    LayerArn: str,
    LayerVersionArn: str,
    Description: str,
    CreatedDate: str,
    Version: int,
    CompatibleRuntimes: List[RuntimeType],  # (2)
    LicenseInfo: str,
    CompatibleArchitectures: List[ArchitectureType],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: LayerVersionContentOutputTypeDef](./type_defs.md#layerversioncontentoutputtypedef) 
2. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
3. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PublishLayerVersionResponseTypeDef

```python
# PublishLayerVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PublishLayerVersionResponseTypeDef


def get_value() -> PublishLayerVersionResponseTypeDef:
    return {
        "Content": ...,
    }


# PublishLayerVersionResponseTypeDef definition

class PublishLayerVersionResponseTypeDef(TypedDict):
    Content: LayerVersionContentOutputTypeDef,  # (1)
    LayerArn: str,
    LayerVersionArn: str,
    Description: str,
    CreatedDate: str,
    Version: int,
    CompatibleRuntimes: List[RuntimeType],  # (2)
    LicenseInfo: str,
    CompatibleArchitectures: List[ArchitectureType],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: LayerVersionContentOutputTypeDef](./type_defs.md#layerversioncontentoutputtypedef) 
2. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
3. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImageConfigResponseTypeDef

```python
# ImageConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ImageConfigResponseTypeDef


def get_value() -> ImageConfigResponseTypeDef:
    return {
        "ImageConfig": ...,
    }


# ImageConfigResponseTypeDef definition

class ImageConfigResponseTypeDef(TypedDict):
    ImageConfig: NotRequired[ImageConfigOutputTypeDef],  # (1)
    Error: NotRequired[ImageConfigErrorTypeDef],  # (2)
```

1. See [:material-code-braces: ImageConfigOutputTypeDef](./type_defs.md#imageconfigoutputtypedef) 
2. See [:material-code-braces: ImageConfigErrorTypeDef](./type_defs.md#imageconfigerrortypedef) 
## InvokeWithResponseStreamResponseEventTypeDef

```python
# InvokeWithResponseStreamResponseEventTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import InvokeWithResponseStreamResponseEventTypeDef


def get_value() -> InvokeWithResponseStreamResponseEventTypeDef:
    return {
        "PayloadChunk": ...,
    }


# InvokeWithResponseStreamResponseEventTypeDef definition

class InvokeWithResponseStreamResponseEventTypeDef(TypedDict):
    PayloadChunk: NotRequired[InvokeResponseStreamUpdateTypeDef],  # (1)
    InvokeComplete: NotRequired[InvokeWithResponseStreamCompleteEventTypeDef],  # (2)
```

1. See [:material-code-braces: InvokeResponseStreamUpdateTypeDef](./type_defs.md#invokeresponsestreamupdatetypedef) 
2. See [:material-code-braces: InvokeWithResponseStreamCompleteEventTypeDef](./type_defs.md#invokewithresponsestreamcompleteeventtypedef) 
## LayersListItemTypeDef

```python
# LayersListItemTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import LayersListItemTypeDef


def get_value() -> LayersListItemTypeDef:
    return {
        "LayerName": ...,
    }


# LayersListItemTypeDef definition

class LayersListItemTypeDef(TypedDict):
    LayerName: NotRequired[str],
    LayerArn: NotRequired[str],
    LatestMatchingVersion: NotRequired[LayerVersionsListItemTypeDef],  # (1)
```

1. See [:material-code-braces: LayerVersionsListItemTypeDef](./type_defs.md#layerversionslistitemtypedef) 
## ListLayerVersionsResponseTypeDef

```python
# ListLayerVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListLayerVersionsResponseTypeDef


def get_value() -> ListLayerVersionsResponseTypeDef:
    return {
        "NextMarker": ...,
    }


# ListLayerVersionsResponseTypeDef definition

class ListLayerVersionsResponseTypeDef(TypedDict):
    NextMarker: str,
    LayerVersions: List[LayerVersionsListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LayerVersionsListItemTypeDef](./type_defs.md#layerversionslistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAliasesRequestPaginateTypeDef

```python
# ListAliasesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListAliasesRequestPaginateTypeDef


def get_value() -> ListAliasesRequestPaginateTypeDef:
    return {
        "FunctionName": ...,
    }


# ListAliasesRequestPaginateTypeDef definition

class ListAliasesRequestPaginateTypeDef(TypedDict):
    FunctionName: str,
    FunctionVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCodeSigningConfigsRequestPaginateTypeDef

```python
# ListCodeSigningConfigsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListCodeSigningConfigsRequestPaginateTypeDef


def get_value() -> ListCodeSigningConfigsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListCodeSigningConfigsRequestPaginateTypeDef definition

class ListCodeSigningConfigsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEventSourceMappingsRequestPaginateTypeDef

```python
# ListEventSourceMappingsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListEventSourceMappingsRequestPaginateTypeDef


def get_value() -> ListEventSourceMappingsRequestPaginateTypeDef:
    return {
        "EventSourceArn": ...,
    }


# ListEventSourceMappingsRequestPaginateTypeDef definition

class ListEventSourceMappingsRequestPaginateTypeDef(TypedDict):
    EventSourceArn: NotRequired[str],
    FunctionName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFunctionEventInvokeConfigsRequestPaginateTypeDef

```python
# ListFunctionEventInvokeConfigsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListFunctionEventInvokeConfigsRequestPaginateTypeDef


def get_value() -> ListFunctionEventInvokeConfigsRequestPaginateTypeDef:
    return {
        "FunctionName": ...,
    }


# ListFunctionEventInvokeConfigsRequestPaginateTypeDef definition

class ListFunctionEventInvokeConfigsRequestPaginateTypeDef(TypedDict):
    FunctionName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFunctionUrlConfigsRequestPaginateTypeDef

```python
# ListFunctionUrlConfigsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListFunctionUrlConfigsRequestPaginateTypeDef


def get_value() -> ListFunctionUrlConfigsRequestPaginateTypeDef:
    return {
        "FunctionName": ...,
    }


# ListFunctionUrlConfigsRequestPaginateTypeDef definition

class ListFunctionUrlConfigsRequestPaginateTypeDef(TypedDict):
    FunctionName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFunctionsByCodeSigningConfigRequestPaginateTypeDef

```python
# ListFunctionsByCodeSigningConfigRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListFunctionsByCodeSigningConfigRequestPaginateTypeDef


def get_value() -> ListFunctionsByCodeSigningConfigRequestPaginateTypeDef:
    return {
        "CodeSigningConfigArn": ...,
    }


# ListFunctionsByCodeSigningConfigRequestPaginateTypeDef definition

class ListFunctionsByCodeSigningConfigRequestPaginateTypeDef(TypedDict):
    CodeSigningConfigArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFunctionsRequestPaginateTypeDef

```python
# ListFunctionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListFunctionsRequestPaginateTypeDef


def get_value() -> ListFunctionsRequestPaginateTypeDef:
    return {
        "MasterRegion": ...,
    }


# ListFunctionsRequestPaginateTypeDef definition

class ListFunctionsRequestPaginateTypeDef(TypedDict):
    MasterRegion: NotRequired[str],
    FunctionVersion: NotRequired[FunctionVersionType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FunctionVersionType](./literals.md#functionversiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLayerVersionsRequestPaginateTypeDef

```python
# ListLayerVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListLayerVersionsRequestPaginateTypeDef


def get_value() -> ListLayerVersionsRequestPaginateTypeDef:
    return {
        "LayerName": ...,
    }


# ListLayerVersionsRequestPaginateTypeDef definition

class ListLayerVersionsRequestPaginateTypeDef(TypedDict):
    LayerName: str,
    CompatibleRuntime: NotRequired[RuntimeType],  # (1)
    CompatibleArchitecture: NotRequired[ArchitectureType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLayersRequestPaginateTypeDef

```python
# ListLayersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListLayersRequestPaginateTypeDef


def get_value() -> ListLayersRequestPaginateTypeDef:
    return {
        "CompatibleRuntime": ...,
    }


# ListLayersRequestPaginateTypeDef definition

class ListLayersRequestPaginateTypeDef(TypedDict):
    CompatibleRuntime: NotRequired[RuntimeType],  # (1)
    CompatibleArchitecture: NotRequired[ArchitectureType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProvisionedConcurrencyConfigsRequestPaginateTypeDef

```python
# ListProvisionedConcurrencyConfigsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListProvisionedConcurrencyConfigsRequestPaginateTypeDef


def get_value() -> ListProvisionedConcurrencyConfigsRequestPaginateTypeDef:
    return {
        "FunctionName": ...,
    }


# ListProvisionedConcurrencyConfigsRequestPaginateTypeDef definition

class ListProvisionedConcurrencyConfigsRequestPaginateTypeDef(TypedDict):
    FunctionName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVersionsByFunctionRequestPaginateTypeDef

```python
# ListVersionsByFunctionRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListVersionsByFunctionRequestPaginateTypeDef


def get_value() -> ListVersionsByFunctionRequestPaginateTypeDef:
    return {
        "FunctionName": ...,
    }


# ListVersionsByFunctionRequestPaginateTypeDef definition

class ListVersionsByFunctionRequestPaginateTypeDef(TypedDict):
    FunctionName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProvisionedConcurrencyConfigsResponseTypeDef

```python
# ListProvisionedConcurrencyConfigsResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListProvisionedConcurrencyConfigsResponseTypeDef


def get_value() -> ListProvisionedConcurrencyConfigsResponseTypeDef:
    return {
        "ProvisionedConcurrencyConfigs": ...,
    }


# ListProvisionedConcurrencyConfigsResponseTypeDef definition

class ListProvisionedConcurrencyConfigsResponseTypeDef(TypedDict):
    ProvisionedConcurrencyConfigs: List[ProvisionedConcurrencyConfigListItemTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProvisionedConcurrencyConfigListItemTypeDef](./type_defs.md#provisionedconcurrencyconfiglistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuntimeVersionConfigTypeDef

```python
# RuntimeVersionConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import RuntimeVersionConfigTypeDef


def get_value() -> RuntimeVersionConfigTypeDef:
    return {
        "RuntimeVersionArn": ...,
    }


# RuntimeVersionConfigTypeDef definition

class RuntimeVersionConfigTypeDef(TypedDict):
    RuntimeVersionArn: NotRequired[str],
    Error: NotRequired[RuntimeVersionErrorTypeDef],  # (1)
```

1. See [:material-code-braces: RuntimeVersionErrorTypeDef](./type_defs.md#runtimeversionerrortypedef) 
## ListAliasesResponseTypeDef

```python
# ListAliasesResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListAliasesResponseTypeDef


def get_value() -> ListAliasesResponseTypeDef:
    return {
        "NextMarker": ...,
    }


# ListAliasesResponseTypeDef definition

class ListAliasesResponseTypeDef(TypedDict):
    NextMarker: str,
    Aliases: List[AliasConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AliasConfigurationTypeDef](./type_defs.md#aliasconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAliasRequestTypeDef

```python
# CreateAliasRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import CreateAliasRequestTypeDef


def get_value() -> CreateAliasRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# CreateAliasRequestTypeDef definition

class CreateAliasRequestTypeDef(TypedDict):
    FunctionName: str,
    Name: str,
    FunctionVersion: str,
    Description: NotRequired[str],
    RoutingConfig: NotRequired[AliasRoutingConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: AliasRoutingConfigurationTypeDef](./type_defs.md#aliasroutingconfigurationtypedef) [:material-code-braces: AliasRoutingConfigurationOutputTypeDef](./type_defs.md#aliasroutingconfigurationoutputtypedef) 
## UpdateAliasRequestTypeDef

```python
# UpdateAliasRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import UpdateAliasRequestTypeDef


def get_value() -> UpdateAliasRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# UpdateAliasRequestTypeDef definition

class UpdateAliasRequestTypeDef(TypedDict):
    FunctionName: str,
    Name: str,
    FunctionVersion: NotRequired[str],
    Description: NotRequired[str],
    RoutingConfig: NotRequired[AliasRoutingConfigurationUnionTypeDef],  # (1)
    RevisionId: NotRequired[str],
```

1. See [:material-code-braces: AliasRoutingConfigurationTypeDef](./type_defs.md#aliasroutingconfigurationtypedef) [:material-code-braces: AliasRoutingConfigurationOutputTypeDef](./type_defs.md#aliasroutingconfigurationoutputtypedef) 
## CreateCodeSigningConfigRequestTypeDef

```python
# CreateCodeSigningConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import CreateCodeSigningConfigRequestTypeDef


def get_value() -> CreateCodeSigningConfigRequestTypeDef:
    return {
        "AllowedPublishers": ...,
    }


# CreateCodeSigningConfigRequestTypeDef definition

class CreateCodeSigningConfigRequestTypeDef(TypedDict):
    AllowedPublishers: AllowedPublishersUnionTypeDef,  # (1)
    Description: NotRequired[str],
    CodeSigningPolicies: NotRequired[CodeSigningPoliciesTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AllowedPublishersTypeDef](./type_defs.md#allowedpublisherstypedef) [:material-code-braces: AllowedPublishersOutputTypeDef](./type_defs.md#allowedpublishersoutputtypedef) 
2. See [:material-code-braces: CodeSigningPoliciesTypeDef](./type_defs.md#codesigningpoliciestypedef) 
## UpdateCodeSigningConfigRequestTypeDef

```python
# UpdateCodeSigningConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import UpdateCodeSigningConfigRequestTypeDef


def get_value() -> UpdateCodeSigningConfigRequestTypeDef:
    return {
        "CodeSigningConfigArn": ...,
    }


# UpdateCodeSigningConfigRequestTypeDef definition

class UpdateCodeSigningConfigRequestTypeDef(TypedDict):
    CodeSigningConfigArn: str,
    Description: NotRequired[str],
    AllowedPublishers: NotRequired[AllowedPublishersUnionTypeDef],  # (1)
    CodeSigningPolicies: NotRequired[CodeSigningPoliciesTypeDef],  # (2)
```

1. See [:material-code-braces: AllowedPublishersTypeDef](./type_defs.md#allowedpublisherstypedef) [:material-code-braces: AllowedPublishersOutputTypeDef](./type_defs.md#allowedpublishersoutputtypedef) 
2. See [:material-code-braces: CodeSigningPoliciesTypeDef](./type_defs.md#codesigningpoliciestypedef) 
## PublishLayerVersionRequestTypeDef

```python
# PublishLayerVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PublishLayerVersionRequestTypeDef


def get_value() -> PublishLayerVersionRequestTypeDef:
    return {
        "LayerName": ...,
    }


# PublishLayerVersionRequestTypeDef definition

class PublishLayerVersionRequestTypeDef(TypedDict):
    LayerName: str,
    Content: LayerVersionContentInputTypeDef,  # (1)
    Description: NotRequired[str],
    CompatibleRuntimes: NotRequired[Sequence[RuntimeType]],  # (2)
    LicenseInfo: NotRequired[str],
    CompatibleArchitectures: NotRequired[Sequence[ArchitectureType]],  # (3)
```

1. See [:material-code-braces: LayerVersionContentInputTypeDef](./type_defs.md#layerversioncontentinputtypedef) 
2. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
3. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## CreateCodeSigningConfigResponseTypeDef

```python
# CreateCodeSigningConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import CreateCodeSigningConfigResponseTypeDef


def get_value() -> CreateCodeSigningConfigResponseTypeDef:
    return {
        "CodeSigningConfig": ...,
    }


# CreateCodeSigningConfigResponseTypeDef definition

class CreateCodeSigningConfigResponseTypeDef(TypedDict):
    CodeSigningConfig: CodeSigningConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeSigningConfigTypeDef](./type_defs.md#codesigningconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCodeSigningConfigResponseTypeDef

```python
# GetCodeSigningConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetCodeSigningConfigResponseTypeDef


def get_value() -> GetCodeSigningConfigResponseTypeDef:
    return {
        "CodeSigningConfig": ...,
    }


# GetCodeSigningConfigResponseTypeDef definition

class GetCodeSigningConfigResponseTypeDef(TypedDict):
    CodeSigningConfig: CodeSigningConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeSigningConfigTypeDef](./type_defs.md#codesigningconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCodeSigningConfigsResponseTypeDef

```python
# ListCodeSigningConfigsResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListCodeSigningConfigsResponseTypeDef


def get_value() -> ListCodeSigningConfigsResponseTypeDef:
    return {
        "NextMarker": ...,
    }


# ListCodeSigningConfigsResponseTypeDef definition

class ListCodeSigningConfigsResponseTypeDef(TypedDict):
    NextMarker: str,
    CodeSigningConfigs: List[CodeSigningConfigTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeSigningConfigTypeDef](./type_defs.md#codesigningconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCodeSigningConfigResponseTypeDef

```python
# UpdateCodeSigningConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import UpdateCodeSigningConfigResponseTypeDef


def get_value() -> UpdateCodeSigningConfigResponseTypeDef:
    return {
        "CodeSigningConfig": ...,
    }


# UpdateCodeSigningConfigResponseTypeDef definition

class UpdateCodeSigningConfigResponseTypeDef(TypedDict):
    CodeSigningConfig: CodeSigningConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeSigningConfigTypeDef](./type_defs.md#codesigningconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFunctionUrlConfigsResponseTypeDef

```python
# ListFunctionUrlConfigsResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListFunctionUrlConfigsResponseTypeDef


def get_value() -> ListFunctionUrlConfigsResponseTypeDef:
    return {
        "FunctionUrlConfigs": ...,
    }


# ListFunctionUrlConfigsResponseTypeDef definition

class ListFunctionUrlConfigsResponseTypeDef(TypedDict):
    FunctionUrlConfigs: List[FunctionUrlConfigTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FunctionUrlConfigTypeDef](./type_defs.md#functionurlconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFunctionUrlConfigRequestTypeDef

```python
# CreateFunctionUrlConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import CreateFunctionUrlConfigRequestTypeDef


def get_value() -> CreateFunctionUrlConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# CreateFunctionUrlConfigRequestTypeDef definition

class CreateFunctionUrlConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    AuthType: FunctionUrlAuthTypeType,  # (1)
    Qualifier: NotRequired[str],
    Cors: NotRequired[CorsUnionTypeDef],  # (2)
    InvokeMode: NotRequired[InvokeModeType],  # (3)
```

1. See [:material-code-brackets: FunctionUrlAuthTypeType](./literals.md#functionurlauthtypetype) 
2. See [:material-code-braces: CorsTypeDef](./type_defs.md#corstypedef) [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
3. See [:material-code-brackets: InvokeModeType](./literals.md#invokemodetype) 
## UpdateFunctionUrlConfigRequestTypeDef

```python
# UpdateFunctionUrlConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import UpdateFunctionUrlConfigRequestTypeDef


def get_value() -> UpdateFunctionUrlConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# UpdateFunctionUrlConfigRequestTypeDef definition

class UpdateFunctionUrlConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    AuthType: NotRequired[FunctionUrlAuthTypeType],  # (1)
    Cors: NotRequired[CorsUnionTypeDef],  # (2)
    InvokeMode: NotRequired[InvokeModeType],  # (3)
```

1. See [:material-code-brackets: FunctionUrlAuthTypeType](./literals.md#functionurlauthtypetype) 
2. See [:material-code-braces: CorsTypeDef](./type_defs.md#corstypedef) [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
3. See [:material-code-brackets: InvokeModeType](./literals.md#invokemodetype) 
## FunctionEventInvokeConfigResponseTypeDef

```python
# FunctionEventInvokeConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import FunctionEventInvokeConfigResponseTypeDef


def get_value() -> FunctionEventInvokeConfigResponseTypeDef:
    return {
        "LastModified": ...,
    }


# FunctionEventInvokeConfigResponseTypeDef definition

class FunctionEventInvokeConfigResponseTypeDef(TypedDict):
    LastModified: datetime,
    FunctionArn: str,
    MaximumRetryAttempts: int,
    MaximumEventAgeInSeconds: int,
    DestinationConfig: DestinationConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FunctionEventInvokeConfigTypeDef

```python
# FunctionEventInvokeConfigTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import FunctionEventInvokeConfigTypeDef


def get_value() -> FunctionEventInvokeConfigTypeDef:
    return {
        "LastModified": ...,
    }


# FunctionEventInvokeConfigTypeDef definition

class FunctionEventInvokeConfigTypeDef(TypedDict):
    LastModified: NotRequired[datetime],
    FunctionArn: NotRequired[str],
    MaximumRetryAttempts: NotRequired[int],
    MaximumEventAgeInSeconds: NotRequired[int],
    DestinationConfig: NotRequired[DestinationConfigTypeDef],  # (1)
```

1. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
## PutFunctionEventInvokeConfigRequestTypeDef

```python
# PutFunctionEventInvokeConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import PutFunctionEventInvokeConfigRequestTypeDef


def get_value() -> PutFunctionEventInvokeConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# PutFunctionEventInvokeConfigRequestTypeDef definition

class PutFunctionEventInvokeConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    MaximumRetryAttempts: NotRequired[int],
    MaximumEventAgeInSeconds: NotRequired[int],
    DestinationConfig: NotRequired[DestinationConfigTypeDef],  # (1)
```

1. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
## UpdateFunctionEventInvokeConfigRequestTypeDef

```python
# UpdateFunctionEventInvokeConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import UpdateFunctionEventInvokeConfigRequestTypeDef


def get_value() -> UpdateFunctionEventInvokeConfigRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# UpdateFunctionEventInvokeConfigRequestTypeDef definition

class UpdateFunctionEventInvokeConfigRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    MaximumRetryAttempts: NotRequired[int],
    MaximumEventAgeInSeconds: NotRequired[int],
    DestinationConfig: NotRequired[DestinationConfigTypeDef],  # (1)
```

1. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
## EventSourceMappingConfigurationResponseTypeDef

```python
# EventSourceMappingConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import EventSourceMappingConfigurationResponseTypeDef


def get_value() -> EventSourceMappingConfigurationResponseTypeDef:
    return {
        "UUID": ...,
    }


# EventSourceMappingConfigurationResponseTypeDef definition

class EventSourceMappingConfigurationResponseTypeDef(TypedDict):
    UUID: str,
    StartingPosition: EventSourcePositionType,  # (1)
    StartingPositionTimestamp: datetime,
    BatchSize: int,
    MaximumBatchingWindowInSeconds: int,
    ParallelizationFactor: int,
    EventSourceArn: str,
    FilterCriteria: FilterCriteriaOutputTypeDef,  # (2)
    FunctionArn: str,
    LastModified: datetime,
    LastProcessingResult: str,
    State: str,
    StateTransitionReason: str,
    DestinationConfig: DestinationConfigTypeDef,  # (3)
    Topics: List[str],
    Queues: List[str],
    SourceAccessConfigurations: List[SourceAccessConfigurationTypeDef],  # (4)
    SelfManagedEventSource: SelfManagedEventSourceOutputTypeDef,  # (5)
    MaximumRecordAgeInSeconds: int,
    BisectBatchOnFunctionError: bool,
    MaximumRetryAttempts: int,
    TumblingWindowInSeconds: int,
    FunctionResponseTypes: List[FunctionResponseTypeType],  # (6)
    AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef,  # (7)
    SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef,  # (8)
    ScalingConfig: ScalingConfigTypeDef,  # (9)
    DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef,  # (10)
    KMSKeyArn: str,
    FilterCriteriaError: FilterCriteriaErrorTypeDef,  # (11)
    EventSourceMappingArn: str,
    MetricsConfig: EventSourceMappingMetricsConfigOutputTypeDef,  # (12)
    ProvisionedPollerConfig: ProvisionedPollerConfigTypeDef,  # (13)
    ResponseMetadata: ResponseMetadataTypeDef,  # (14)
```

1. See [:material-code-brackets: EventSourcePositionType](./literals.md#eventsourcepositiontype) 
2. See [:material-code-braces: FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef) 
3. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
4. See [:material-code-braces: SourceAccessConfigurationTypeDef](./type_defs.md#sourceaccessconfigurationtypedef) 
5. See [:material-code-braces: SelfManagedEventSourceOutputTypeDef](./type_defs.md#selfmanagedeventsourceoutputtypedef) 
6. See [:material-code-brackets: FunctionResponseTypeType](./literals.md#functionresponsetypetype) 
7. See [:material-code-braces: AmazonManagedKafkaEventSourceConfigTypeDef](./type_defs.md#amazonmanagedkafkaeventsourceconfigtypedef) 
8. See [:material-code-braces: SelfManagedKafkaEventSourceConfigTypeDef](./type_defs.md#selfmanagedkafkaeventsourceconfigtypedef) 
9. See [:material-code-braces: ScalingConfigTypeDef](./type_defs.md#scalingconfigtypedef) 
10. See [:material-code-braces: DocumentDBEventSourceConfigTypeDef](./type_defs.md#documentdbeventsourceconfigtypedef) 
11. See [:material-code-braces: FilterCriteriaErrorTypeDef](./type_defs.md#filtercriteriaerrortypedef) 
12. See [:material-code-braces: EventSourceMappingMetricsConfigOutputTypeDef](./type_defs.md#eventsourcemappingmetricsconfigoutputtypedef) 
13. See [:material-code-braces: ProvisionedPollerConfigTypeDef](./type_defs.md#provisionedpollerconfigtypedef) 
14. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventSourceMappingConfigurationTypeDef

```python
# EventSourceMappingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import EventSourceMappingConfigurationTypeDef


def get_value() -> EventSourceMappingConfigurationTypeDef:
    return {
        "UUID": ...,
    }


# EventSourceMappingConfigurationTypeDef definition

class EventSourceMappingConfigurationTypeDef(TypedDict):
    UUID: NotRequired[str],
    StartingPosition: NotRequired[EventSourcePositionType],  # (1)
    StartingPositionTimestamp: NotRequired[datetime],
    BatchSize: NotRequired[int],
    MaximumBatchingWindowInSeconds: NotRequired[int],
    ParallelizationFactor: NotRequired[int],
    EventSourceArn: NotRequired[str],
    FilterCriteria: NotRequired[FilterCriteriaOutputTypeDef],  # (2)
    FunctionArn: NotRequired[str],
    LastModified: NotRequired[datetime],
    LastProcessingResult: NotRequired[str],
    State: NotRequired[str],
    StateTransitionReason: NotRequired[str],
    DestinationConfig: NotRequired[DestinationConfigTypeDef],  # (3)
    Topics: NotRequired[List[str]],
    Queues: NotRequired[List[str]],
    SourceAccessConfigurations: NotRequired[List[SourceAccessConfigurationTypeDef]],  # (4)
    SelfManagedEventSource: NotRequired[SelfManagedEventSourceOutputTypeDef],  # (5)
    MaximumRecordAgeInSeconds: NotRequired[int],
    BisectBatchOnFunctionError: NotRequired[bool],
    MaximumRetryAttempts: NotRequired[int],
    TumblingWindowInSeconds: NotRequired[int],
    FunctionResponseTypes: NotRequired[List[FunctionResponseTypeType]],  # (6)
    AmazonManagedKafkaEventSourceConfig: NotRequired[AmazonManagedKafkaEventSourceConfigTypeDef],  # (7)
    SelfManagedKafkaEventSourceConfig: NotRequired[SelfManagedKafkaEventSourceConfigTypeDef],  # (8)
    ScalingConfig: NotRequired[ScalingConfigTypeDef],  # (9)
    DocumentDBEventSourceConfig: NotRequired[DocumentDBEventSourceConfigTypeDef],  # (10)
    KMSKeyArn: NotRequired[str],
    FilterCriteriaError: NotRequired[FilterCriteriaErrorTypeDef],  # (11)
    EventSourceMappingArn: NotRequired[str],
    MetricsConfig: NotRequired[EventSourceMappingMetricsConfigOutputTypeDef],  # (12)
    ProvisionedPollerConfig: NotRequired[ProvisionedPollerConfigTypeDef],  # (13)
```

1. See [:material-code-brackets: EventSourcePositionType](./literals.md#eventsourcepositiontype) 
2. See [:material-code-braces: FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef) 
3. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
4. See [:material-code-braces: SourceAccessConfigurationTypeDef](./type_defs.md#sourceaccessconfigurationtypedef) 
5. See [:material-code-braces: SelfManagedEventSourceOutputTypeDef](./type_defs.md#selfmanagedeventsourceoutputtypedef) 
6. See [:material-code-brackets: FunctionResponseTypeType](./literals.md#functionresponsetypetype) 
7. See [:material-code-braces: AmazonManagedKafkaEventSourceConfigTypeDef](./type_defs.md#amazonmanagedkafkaeventsourceconfigtypedef) 
8. See [:material-code-braces: SelfManagedKafkaEventSourceConfigTypeDef](./type_defs.md#selfmanagedkafkaeventsourceconfigtypedef) 
9. See [:material-code-braces: ScalingConfigTypeDef](./type_defs.md#scalingconfigtypedef) 
10. See [:material-code-braces: DocumentDBEventSourceConfigTypeDef](./type_defs.md#documentdbeventsourceconfigtypedef) 
11. See [:material-code-braces: FilterCriteriaErrorTypeDef](./type_defs.md#filtercriteriaerrortypedef) 
12. See [:material-code-braces: EventSourceMappingMetricsConfigOutputTypeDef](./type_defs.md#eventsourcemappingmetricsconfigoutputtypedef) 
13. See [:material-code-braces: ProvisionedPollerConfigTypeDef](./type_defs.md#provisionedpollerconfigtypedef) 
## CreateFunctionRequestTypeDef

```python
# CreateFunctionRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import CreateFunctionRequestTypeDef


def get_value() -> CreateFunctionRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# CreateFunctionRequestTypeDef definition

class CreateFunctionRequestTypeDef(TypedDict):
    FunctionName: str,
    Role: str,
    Code: FunctionCodeTypeDef,  # (1)
    Runtime: NotRequired[RuntimeType],  # (2)
    Handler: NotRequired[str],
    Description: NotRequired[str],
    Timeout: NotRequired[int],
    MemorySize: NotRequired[int],
    Publish: NotRequired[bool],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (3)
    PackageType: NotRequired[PackageTypeType],  # (4)
    DeadLetterConfig: NotRequired[DeadLetterConfigTypeDef],  # (5)
    Environment: NotRequired[EnvironmentTypeDef],  # (6)
    KMSKeyArn: NotRequired[str],
    TracingConfig: NotRequired[TracingConfigTypeDef],  # (7)
    Tags: NotRequired[Mapping[str, str]],
    Layers: NotRequired[Sequence[str]],
    FileSystemConfigs: NotRequired[Sequence[FileSystemConfigTypeDef]],  # (8)
    ImageConfig: NotRequired[ImageConfigUnionTypeDef],  # (9)
    CodeSigningConfigArn: NotRequired[str],
    Architectures: NotRequired[Sequence[ArchitectureType]],  # (10)
    EphemeralStorage: NotRequired[EphemeralStorageTypeDef],  # (11)
    SnapStart: NotRequired[SnapStartTypeDef],  # (12)
    LoggingConfig: NotRequired[LoggingConfigTypeDef],  # (13)
```

1. See [:material-code-braces: FunctionCodeTypeDef](./type_defs.md#functioncodetypedef) 
2. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
3. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
4. See [:material-code-brackets: PackageTypeType](./literals.md#packagetypetype) 
5. See [:material-code-braces: DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef) 
6. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
7. See [:material-code-braces: TracingConfigTypeDef](./type_defs.md#tracingconfigtypedef) 
8. See [:material-code-braces: FileSystemConfigTypeDef](./type_defs.md#filesystemconfigtypedef) 
9. See [:material-code-braces: ImageConfigTypeDef](./type_defs.md#imageconfigtypedef) [:material-code-braces: ImageConfigOutputTypeDef](./type_defs.md#imageconfigoutputtypedef) 
10. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
11. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
12. See [:material-code-braces: SnapStartTypeDef](./type_defs.md#snapstarttypedef) 
13. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
## UpdateFunctionConfigurationRequestTypeDef

```python
# UpdateFunctionConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import UpdateFunctionConfigurationRequestTypeDef


def get_value() -> UpdateFunctionConfigurationRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# UpdateFunctionConfigurationRequestTypeDef definition

class UpdateFunctionConfigurationRequestTypeDef(TypedDict):
    FunctionName: str,
    Role: NotRequired[str],
    Handler: NotRequired[str],
    Description: NotRequired[str],
    Timeout: NotRequired[int],
    MemorySize: NotRequired[int],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (1)
    Environment: NotRequired[EnvironmentTypeDef],  # (2)
    Runtime: NotRequired[RuntimeType],  # (3)
    DeadLetterConfig: NotRequired[DeadLetterConfigTypeDef],  # (4)
    KMSKeyArn: NotRequired[str],
    TracingConfig: NotRequired[TracingConfigTypeDef],  # (5)
    RevisionId: NotRequired[str],
    Layers: NotRequired[Sequence[str]],
    FileSystemConfigs: NotRequired[Sequence[FileSystemConfigTypeDef]],  # (6)
    ImageConfig: NotRequired[ImageConfigUnionTypeDef],  # (7)
    EphemeralStorage: NotRequired[EphemeralStorageTypeDef],  # (8)
    SnapStart: NotRequired[SnapStartTypeDef],  # (9)
    LoggingConfig: NotRequired[LoggingConfigTypeDef],  # (10)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
2. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
3. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
4. See [:material-code-braces: DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef) 
5. See [:material-code-braces: TracingConfigTypeDef](./type_defs.md#tracingconfigtypedef) 
6. See [:material-code-braces: FileSystemConfigTypeDef](./type_defs.md#filesystemconfigtypedef) 
7. See [:material-code-braces: ImageConfigTypeDef](./type_defs.md#imageconfigtypedef) [:material-code-braces: ImageConfigOutputTypeDef](./type_defs.md#imageconfigoutputtypedef) 
8. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
9. See [:material-code-braces: SnapStartTypeDef](./type_defs.md#snapstarttypedef) 
10. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
## InvokeWithResponseStreamResponseTypeDef

```python
# InvokeWithResponseStreamResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import InvokeWithResponseStreamResponseTypeDef


def get_value() -> InvokeWithResponseStreamResponseTypeDef:
    return {
        "StatusCode": ...,
    }


# InvokeWithResponseStreamResponseTypeDef definition

class InvokeWithResponseStreamResponseTypeDef(TypedDict):
    StatusCode: int,
    ExecutedVersion: str,
    EventStream: AioEventStream[InvokeWithResponseStreamResponseEventTypeDef],  # (1)
    ResponseStreamContentType: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InvokeWithResponseStreamResponseEventTypeDef](./type_defs.md#invokewithresponsestreamresponseeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLayersResponseTypeDef

```python
# ListLayersResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListLayersResponseTypeDef


def get_value() -> ListLayersResponseTypeDef:
    return {
        "NextMarker": ...,
    }


# ListLayersResponseTypeDef definition

class ListLayersResponseTypeDef(TypedDict):
    NextMarker: str,
    Layers: List[LayersListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LayersListItemTypeDef](./type_defs.md#layerslistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FunctionConfigurationResponseTypeDef

```python
# FunctionConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import FunctionConfigurationResponseTypeDef


def get_value() -> FunctionConfigurationResponseTypeDef:
    return {
        "FunctionName": ...,
    }


# FunctionConfigurationResponseTypeDef definition

class FunctionConfigurationResponseTypeDef(TypedDict):
    FunctionName: str,
    FunctionArn: str,
    Runtime: RuntimeType,  # (1)
    Role: str,
    Handler: str,
    CodeSize: int,
    Description: str,
    Timeout: int,
    MemorySize: int,
    LastModified: str,
    CodeSha256: str,
    Version: str,
    VpcConfig: VpcConfigResponseTypeDef,  # (2)
    DeadLetterConfig: DeadLetterConfigTypeDef,  # (3)
    Environment: EnvironmentResponseTypeDef,  # (4)
    KMSKeyArn: str,
    TracingConfig: TracingConfigResponseTypeDef,  # (5)
    MasterArn: str,
    RevisionId: str,
    Layers: List[LayerTypeDef],  # (6)
    State: StateType,  # (7)
    StateReason: str,
    StateReasonCode: StateReasonCodeType,  # (8)
    LastUpdateStatus: LastUpdateStatusType,  # (9)
    LastUpdateStatusReason: str,
    LastUpdateStatusReasonCode: LastUpdateStatusReasonCodeType,  # (10)
    FileSystemConfigs: List[FileSystemConfigTypeDef],  # (11)
    PackageType: PackageTypeType,  # (12)
    ImageConfigResponse: ImageConfigResponseTypeDef,  # (13)
    SigningProfileVersionArn: str,
    SigningJobArn: str,
    Architectures: List[ArchitectureType],  # (14)
    EphemeralStorage: EphemeralStorageTypeDef,  # (15)
    SnapStart: SnapStartResponseTypeDef,  # (16)
    RuntimeVersionConfig: RuntimeVersionConfigTypeDef,  # (17)
    LoggingConfig: LoggingConfigTypeDef,  # (18)
    ResponseMetadata: ResponseMetadataTypeDef,  # (19)
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-braces: VpcConfigResponseTypeDef](./type_defs.md#vpcconfigresponsetypedef) 
3. See [:material-code-braces: DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef) 
4. See [:material-code-braces: EnvironmentResponseTypeDef](./type_defs.md#environmentresponsetypedef) 
5. See [:material-code-braces: TracingConfigResponseTypeDef](./type_defs.md#tracingconfigresponsetypedef) 
6. See [:material-code-braces: LayerTypeDef](./type_defs.md#layertypedef) 
7. See [:material-code-brackets: StateType](./literals.md#statetype) 
8. See [:material-code-brackets: StateReasonCodeType](./literals.md#statereasoncodetype) 
9. See [:material-code-brackets: LastUpdateStatusType](./literals.md#lastupdatestatustype) 
10. See [:material-code-brackets: LastUpdateStatusReasonCodeType](./literals.md#lastupdatestatusreasoncodetype) 
11. See [:material-code-braces: FileSystemConfigTypeDef](./type_defs.md#filesystemconfigtypedef) 
12. See [:material-code-brackets: PackageTypeType](./literals.md#packagetypetype) 
13. See [:material-code-braces: ImageConfigResponseTypeDef](./type_defs.md#imageconfigresponsetypedef) 
14. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
15. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
16. See [:material-code-braces: SnapStartResponseTypeDef](./type_defs.md#snapstartresponsetypedef) 
17. See [:material-code-braces: RuntimeVersionConfigTypeDef](./type_defs.md#runtimeversionconfigtypedef) 
18. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
19. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FunctionConfigurationTypeDef

```python
# FunctionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import FunctionConfigurationTypeDef


def get_value() -> FunctionConfigurationTypeDef:
    return {
        "FunctionName": ...,
    }


# FunctionConfigurationTypeDef definition

class FunctionConfigurationTypeDef(TypedDict):
    FunctionName: NotRequired[str],
    FunctionArn: NotRequired[str],
    Runtime: NotRequired[RuntimeType],  # (1)
    Role: NotRequired[str],
    Handler: NotRequired[str],
    CodeSize: NotRequired[int],
    Description: NotRequired[str],
    Timeout: NotRequired[int],
    MemorySize: NotRequired[int],
    LastModified: NotRequired[str],
    CodeSha256: NotRequired[str],
    Version: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigResponseTypeDef],  # (2)
    DeadLetterConfig: NotRequired[DeadLetterConfigTypeDef],  # (3)
    Environment: NotRequired[EnvironmentResponseTypeDef],  # (4)
    KMSKeyArn: NotRequired[str],
    TracingConfig: NotRequired[TracingConfigResponseTypeDef],  # (5)
    MasterArn: NotRequired[str],
    RevisionId: NotRequired[str],
    Layers: NotRequired[List[LayerTypeDef]],  # (6)
    State: NotRequired[StateType],  # (7)
    StateReason: NotRequired[str],
    StateReasonCode: NotRequired[StateReasonCodeType],  # (8)
    LastUpdateStatus: NotRequired[LastUpdateStatusType],  # (9)
    LastUpdateStatusReason: NotRequired[str],
    LastUpdateStatusReasonCode: NotRequired[LastUpdateStatusReasonCodeType],  # (10)
    FileSystemConfigs: NotRequired[List[FileSystemConfigTypeDef]],  # (11)
    PackageType: NotRequired[PackageTypeType],  # (12)
    ImageConfigResponse: NotRequired[ImageConfigResponseTypeDef],  # (13)
    SigningProfileVersionArn: NotRequired[str],
    SigningJobArn: NotRequired[str],
    Architectures: NotRequired[List[ArchitectureType]],  # (14)
    EphemeralStorage: NotRequired[EphemeralStorageTypeDef],  # (15)
    SnapStart: NotRequired[SnapStartResponseTypeDef],  # (16)
    RuntimeVersionConfig: NotRequired[RuntimeVersionConfigTypeDef],  # (17)
    LoggingConfig: NotRequired[LoggingConfigTypeDef],  # (18)
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-braces: VpcConfigResponseTypeDef](./type_defs.md#vpcconfigresponsetypedef) 
3. See [:material-code-braces: DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef) 
4. See [:material-code-braces: EnvironmentResponseTypeDef](./type_defs.md#environmentresponsetypedef) 
5. See [:material-code-braces: TracingConfigResponseTypeDef](./type_defs.md#tracingconfigresponsetypedef) 
6. See [:material-code-braces: LayerTypeDef](./type_defs.md#layertypedef) 
7. See [:material-code-brackets: StateType](./literals.md#statetype) 
8. See [:material-code-brackets: StateReasonCodeType](./literals.md#statereasoncodetype) 
9. See [:material-code-brackets: LastUpdateStatusType](./literals.md#lastupdatestatustype) 
10. See [:material-code-brackets: LastUpdateStatusReasonCodeType](./literals.md#lastupdatestatusreasoncodetype) 
11. See [:material-code-braces: FileSystemConfigTypeDef](./type_defs.md#filesystemconfigtypedef) 
12. See [:material-code-brackets: PackageTypeType](./literals.md#packagetypetype) 
13. See [:material-code-braces: ImageConfigResponseTypeDef](./type_defs.md#imageconfigresponsetypedef) 
14. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
15. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
16. See [:material-code-braces: SnapStartResponseTypeDef](./type_defs.md#snapstartresponsetypedef) 
17. See [:material-code-braces: RuntimeVersionConfigTypeDef](./type_defs.md#runtimeversionconfigtypedef) 
18. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
## ListFunctionEventInvokeConfigsResponseTypeDef

```python
# ListFunctionEventInvokeConfigsResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListFunctionEventInvokeConfigsResponseTypeDef


def get_value() -> ListFunctionEventInvokeConfigsResponseTypeDef:
    return {
        "FunctionEventInvokeConfigs": ...,
    }


# ListFunctionEventInvokeConfigsResponseTypeDef definition

class ListFunctionEventInvokeConfigsResponseTypeDef(TypedDict):
    FunctionEventInvokeConfigs: List[FunctionEventInvokeConfigTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FunctionEventInvokeConfigTypeDef](./type_defs.md#functioneventinvokeconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventSourceMappingsResponseTypeDef

```python
# ListEventSourceMappingsResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListEventSourceMappingsResponseTypeDef


def get_value() -> ListEventSourceMappingsResponseTypeDef:
    return {
        "NextMarker": ...,
    }


# ListEventSourceMappingsResponseTypeDef definition

class ListEventSourceMappingsResponseTypeDef(TypedDict):
    NextMarker: str,
    EventSourceMappings: List[EventSourceMappingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSourceMappingConfigurationTypeDef](./type_defs.md#eventsourcemappingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEventSourceMappingRequestTypeDef

```python
# CreateEventSourceMappingRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import CreateEventSourceMappingRequestTypeDef


def get_value() -> CreateEventSourceMappingRequestTypeDef:
    return {
        "FunctionName": ...,
    }


# CreateEventSourceMappingRequestTypeDef definition

class CreateEventSourceMappingRequestTypeDef(TypedDict):
    FunctionName: str,
    EventSourceArn: NotRequired[str],
    Enabled: NotRequired[bool],
    BatchSize: NotRequired[int],
    FilterCriteria: NotRequired[FilterCriteriaUnionTypeDef],  # (1)
    MaximumBatchingWindowInSeconds: NotRequired[int],
    ParallelizationFactor: NotRequired[int],
    StartingPosition: NotRequired[EventSourcePositionType],  # (2)
    StartingPositionTimestamp: NotRequired[TimestampTypeDef],
    DestinationConfig: NotRequired[DestinationConfigTypeDef],  # (3)
    MaximumRecordAgeInSeconds: NotRequired[int],
    BisectBatchOnFunctionError: NotRequired[bool],
    MaximumRetryAttempts: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
    TumblingWindowInSeconds: NotRequired[int],
    Topics: NotRequired[Sequence[str]],
    Queues: NotRequired[Sequence[str]],
    SourceAccessConfigurations: NotRequired[Sequence[SourceAccessConfigurationTypeDef]],  # (4)
    SelfManagedEventSource: NotRequired[SelfManagedEventSourceUnionTypeDef],  # (5)
    FunctionResponseTypes: NotRequired[Sequence[FunctionResponseTypeType]],  # (6)
    AmazonManagedKafkaEventSourceConfig: NotRequired[AmazonManagedKafkaEventSourceConfigTypeDef],  # (7)
    SelfManagedKafkaEventSourceConfig: NotRequired[SelfManagedKafkaEventSourceConfigTypeDef],  # (8)
    ScalingConfig: NotRequired[ScalingConfigTypeDef],  # (9)
    DocumentDBEventSourceConfig: NotRequired[DocumentDBEventSourceConfigTypeDef],  # (10)
    KMSKeyArn: NotRequired[str],
    MetricsConfig: NotRequired[EventSourceMappingMetricsConfigUnionTypeDef],  # (11)
    ProvisionedPollerConfig: NotRequired[ProvisionedPollerConfigTypeDef],  # (12)
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) [:material-code-braces: FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef) 
2. See [:material-code-brackets: EventSourcePositionType](./literals.md#eventsourcepositiontype) 
3. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
4. See [:material-code-braces: SourceAccessConfigurationTypeDef](./type_defs.md#sourceaccessconfigurationtypedef) 
5. See [:material-code-braces: SelfManagedEventSourceTypeDef](./type_defs.md#selfmanagedeventsourcetypedef) [:material-code-braces: SelfManagedEventSourceOutputTypeDef](./type_defs.md#selfmanagedeventsourceoutputtypedef) 
6. See [:material-code-brackets: FunctionResponseTypeType](./literals.md#functionresponsetypetype) 
7. See [:material-code-braces: AmazonManagedKafkaEventSourceConfigTypeDef](./type_defs.md#amazonmanagedkafkaeventsourceconfigtypedef) 
8. See [:material-code-braces: SelfManagedKafkaEventSourceConfigTypeDef](./type_defs.md#selfmanagedkafkaeventsourceconfigtypedef) 
9. See [:material-code-braces: ScalingConfigTypeDef](./type_defs.md#scalingconfigtypedef) 
10. See [:material-code-braces: DocumentDBEventSourceConfigTypeDef](./type_defs.md#documentdbeventsourceconfigtypedef) 
11. See [:material-code-braces: EventSourceMappingMetricsConfigTypeDef](./type_defs.md#eventsourcemappingmetricsconfigtypedef) [:material-code-braces: EventSourceMappingMetricsConfigOutputTypeDef](./type_defs.md#eventsourcemappingmetricsconfigoutputtypedef) 
12. See [:material-code-braces: ProvisionedPollerConfigTypeDef](./type_defs.md#provisionedpollerconfigtypedef) 
## UpdateEventSourceMappingRequestTypeDef

```python
# UpdateEventSourceMappingRequestTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import UpdateEventSourceMappingRequestTypeDef


def get_value() -> UpdateEventSourceMappingRequestTypeDef:
    return {
        "UUID": ...,
    }


# UpdateEventSourceMappingRequestTypeDef definition

class UpdateEventSourceMappingRequestTypeDef(TypedDict):
    UUID: str,
    FunctionName: NotRequired[str],
    Enabled: NotRequired[bool],
    BatchSize: NotRequired[int],
    FilterCriteria: NotRequired[FilterCriteriaUnionTypeDef],  # (1)
    MaximumBatchingWindowInSeconds: NotRequired[int],
    DestinationConfig: NotRequired[DestinationConfigTypeDef],  # (2)
    MaximumRecordAgeInSeconds: NotRequired[int],
    BisectBatchOnFunctionError: NotRequired[bool],
    MaximumRetryAttempts: NotRequired[int],
    ParallelizationFactor: NotRequired[int],
    SourceAccessConfigurations: NotRequired[Sequence[SourceAccessConfigurationTypeDef]],  # (3)
    TumblingWindowInSeconds: NotRequired[int],
    FunctionResponseTypes: NotRequired[Sequence[FunctionResponseTypeType]],  # (4)
    ScalingConfig: NotRequired[ScalingConfigTypeDef],  # (5)
    DocumentDBEventSourceConfig: NotRequired[DocumentDBEventSourceConfigTypeDef],  # (6)
    KMSKeyArn: NotRequired[str],
    MetricsConfig: NotRequired[EventSourceMappingMetricsConfigUnionTypeDef],  # (7)
    ProvisionedPollerConfig: NotRequired[ProvisionedPollerConfigTypeDef],  # (8)
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) [:material-code-braces: FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef) 
2. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
3. See [:material-code-braces: SourceAccessConfigurationTypeDef](./type_defs.md#sourceaccessconfigurationtypedef) 
4. See [:material-code-brackets: FunctionResponseTypeType](./literals.md#functionresponsetypetype) 
5. See [:material-code-braces: ScalingConfigTypeDef](./type_defs.md#scalingconfigtypedef) 
6. See [:material-code-braces: DocumentDBEventSourceConfigTypeDef](./type_defs.md#documentdbeventsourceconfigtypedef) 
7. See [:material-code-braces: EventSourceMappingMetricsConfigTypeDef](./type_defs.md#eventsourcemappingmetricsconfigtypedef) [:material-code-braces: EventSourceMappingMetricsConfigOutputTypeDef](./type_defs.md#eventsourcemappingmetricsconfigoutputtypedef) 
8. See [:material-code-braces: ProvisionedPollerConfigTypeDef](./type_defs.md#provisionedpollerconfigtypedef) 
## GetFunctionResponseTypeDef

```python
# GetFunctionResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import GetFunctionResponseTypeDef


def get_value() -> GetFunctionResponseTypeDef:
    return {
        "Configuration": ...,
    }


# GetFunctionResponseTypeDef definition

class GetFunctionResponseTypeDef(TypedDict):
    Configuration: FunctionConfigurationTypeDef,  # (1)
    Code: FunctionCodeLocationTypeDef,  # (2)
    Tags: Dict[str, str],
    TagsError: TagsErrorTypeDef,  # (3)
    Concurrency: ConcurrencyTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: FunctionConfigurationTypeDef](./type_defs.md#functionconfigurationtypedef) 
2. See [:material-code-braces: FunctionCodeLocationTypeDef](./type_defs.md#functioncodelocationtypedef) 
3. See [:material-code-braces: TagsErrorTypeDef](./type_defs.md#tagserrortypedef) 
4. See [:material-code-braces: ConcurrencyTypeDef](./type_defs.md#concurrencytypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFunctionsResponseTypeDef

```python
# ListFunctionsResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListFunctionsResponseTypeDef


def get_value() -> ListFunctionsResponseTypeDef:
    return {
        "NextMarker": ...,
    }


# ListFunctionsResponseTypeDef definition

class ListFunctionsResponseTypeDef(TypedDict):
    NextMarker: str,
    Functions: List[FunctionConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FunctionConfigurationTypeDef](./type_defs.md#functionconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVersionsByFunctionResponseTypeDef

```python
# ListVersionsByFunctionResponseTypeDef TypedDict usage example

from types_aiobotocore_lambda.type_defs import ListVersionsByFunctionResponseTypeDef


def get_value() -> ListVersionsByFunctionResponseTypeDef:
    return {
        "NextMarker": ...,
    }


# ListVersionsByFunctionResponseTypeDef definition

class ListVersionsByFunctionResponseTypeDef(TypedDict):
    NextMarker: str,
    Versions: List[FunctionConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FunctionConfigurationTypeDef](./type_defs.md#functionconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
