# Type definitions

> [Index](../README.md) > [Lambda](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Lambda](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
    type annotations stubs module [types-aiobotocore-lambda](https://pypi.org/project/types-aiobotocore-lambda/).

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




## AccountLimitTypeDef

```python
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
# AccountUsageTypeDef definition

class AccountUsageTypeDef(TypedDict):
    TotalCodeSize: NotRequired[int],
    FunctionCount: NotRequired[int],
```

## AddLayerVersionPermissionRequestRequestTypeDef

```python
# AddLayerVersionPermissionRequestRequestTypeDef definition

class AddLayerVersionPermissionRequestRequestTypeDef(TypedDict):
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
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## AddPermissionRequestRequestTypeDef

```python
# AddPermissionRequestRequestTypeDef definition

class AddPermissionRequestRequestTypeDef(TypedDict):
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
# AliasRoutingConfigurationOutputTypeDef definition

class AliasRoutingConfigurationOutputTypeDef(TypedDict):
    AdditionalVersionWeights: NotRequired[Dict[str, float]],
```

## AliasRoutingConfigurationTypeDef

```python
# AliasRoutingConfigurationTypeDef definition

class AliasRoutingConfigurationTypeDef(TypedDict):
    AdditionalVersionWeights: NotRequired[Mapping[str, float]],
```

## AllowedPublishersOutputTypeDef

```python
# AllowedPublishersOutputTypeDef definition

class AllowedPublishersOutputTypeDef(TypedDict):
    SigningProfileVersionArns: List[str],
```

## AllowedPublishersTypeDef

```python
# AllowedPublishersTypeDef definition

class AllowedPublishersTypeDef(TypedDict):
    SigningProfileVersionArns: Sequence[str],
```

## AmazonManagedKafkaEventSourceConfigTypeDef

```python
# AmazonManagedKafkaEventSourceConfigTypeDef definition

class AmazonManagedKafkaEventSourceConfigTypeDef(TypedDict):
    ConsumerGroupId: NotRequired[str],
```

## CodeSigningPoliciesTypeDef

```python
# CodeSigningPoliciesTypeDef definition

class CodeSigningPoliciesTypeDef(TypedDict):
    UntrustedArtifactOnDeployment: NotRequired[CodeSigningPolicyType],  # (1)
```

1. See [:material-code-brackets: CodeSigningPolicyType](./literals.md#codesigningpolicytype) 
## ConcurrencyTypeDef

```python
# ConcurrencyTypeDef definition

class ConcurrencyTypeDef(TypedDict):
    ReservedConcurrentExecutions: NotRequired[int],
```

## CorsOutputTypeDef

```python
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
# DocumentDBEventSourceConfigTypeDef definition

class DocumentDBEventSourceConfigTypeDef(TypedDict):
    DatabaseName: NotRequired[str],
    CollectionName: NotRequired[str],
    FullDocument: NotRequired[FullDocumentType],  # (1)
```

1. See [:material-code-brackets: FullDocumentType](./literals.md#fulldocumenttype) 
## ScalingConfigTypeDef

```python
# ScalingConfigTypeDef definition

class ScalingConfigTypeDef(TypedDict):
    MaximumConcurrency: NotRequired[int],
```

## SelfManagedEventSourceTypeDef

```python
# SelfManagedEventSourceTypeDef definition

class SelfManagedEventSourceTypeDef(TypedDict):
    Endpoints: NotRequired[Mapping[EndPointTypeType, Sequence[str]]],  # (1)
```

1. See [:material-code-brackets: EndPointTypeType](./literals.md#endpointtypetype) 
## SelfManagedKafkaEventSourceConfigTypeDef

```python
# SelfManagedKafkaEventSourceConfigTypeDef definition

class SelfManagedKafkaEventSourceConfigTypeDef(TypedDict):
    ConsumerGroupId: NotRequired[str],
```

## SourceAccessConfigurationTypeDef

```python
# SourceAccessConfigurationTypeDef definition

class SourceAccessConfigurationTypeDef(TypedDict):
    Type: NotRequired[SourceAccessTypeType],  # (1)
    URI: NotRequired[str],
```

1. See [:material-code-brackets: SourceAccessTypeType](./literals.md#sourceaccesstypetype) 
## DeadLetterConfigTypeDef

```python
# DeadLetterConfigTypeDef definition

class DeadLetterConfigTypeDef(TypedDict):
    TargetArn: NotRequired[str],
```

## EnvironmentTypeDef

```python
# EnvironmentTypeDef definition

class EnvironmentTypeDef(TypedDict):
    Variables: NotRequired[Mapping[str, str]],
```

## EphemeralStorageTypeDef

```python
# EphemeralStorageTypeDef definition

class EphemeralStorageTypeDef(TypedDict):
    Size: int,
```

## FileSystemConfigTypeDef

```python
# FileSystemConfigTypeDef definition

class FileSystemConfigTypeDef(TypedDict):
    Arn: str,
    LocalMountPath: str,
```

## ImageConfigTypeDef

```python
# ImageConfigTypeDef definition

class ImageConfigTypeDef(TypedDict):
    EntryPoint: NotRequired[Sequence[str]],
    Command: NotRequired[Sequence[str]],
    WorkingDirectory: NotRequired[str],
```

## LoggingConfigTypeDef

```python
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
# SnapStartTypeDef definition

class SnapStartTypeDef(TypedDict):
    ApplyOn: NotRequired[SnapStartApplyOnType],  # (1)
```

1. See [:material-code-brackets: SnapStartApplyOnType](./literals.md#snapstartapplyontype) 
## TracingConfigTypeDef

```python
# TracingConfigTypeDef definition

class TracingConfigTypeDef(TypedDict):
    Mode: NotRequired[TracingModeType],  # (1)
```

1. See [:material-code-brackets: TracingModeType](./literals.md#tracingmodetype) 
## VpcConfigTypeDef

```python
# VpcConfigTypeDef definition

class VpcConfigTypeDef(TypedDict):
    SubnetIds: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
    Ipv6AllowedForDualStack: NotRequired[bool],
```

## DeleteAliasRequestRequestTypeDef

```python
# DeleteAliasRequestRequestTypeDef definition

class DeleteAliasRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Name: str,
```

## DeleteCodeSigningConfigRequestRequestTypeDef

```python
# DeleteCodeSigningConfigRequestRequestTypeDef definition

class DeleteCodeSigningConfigRequestRequestTypeDef(TypedDict):
    CodeSigningConfigArn: str,
```

## DeleteEventSourceMappingRequestRequestTypeDef

```python
# DeleteEventSourceMappingRequestRequestTypeDef definition

class DeleteEventSourceMappingRequestRequestTypeDef(TypedDict):
    UUID: str,
```

## DeleteFunctionCodeSigningConfigRequestRequestTypeDef

```python
# DeleteFunctionCodeSigningConfigRequestRequestTypeDef definition

class DeleteFunctionCodeSigningConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
```

## DeleteFunctionConcurrencyRequestRequestTypeDef

```python
# DeleteFunctionConcurrencyRequestRequestTypeDef definition

class DeleteFunctionConcurrencyRequestRequestTypeDef(TypedDict):
    FunctionName: str,
```

## DeleteFunctionEventInvokeConfigRequestRequestTypeDef

```python
# DeleteFunctionEventInvokeConfigRequestRequestTypeDef definition

class DeleteFunctionEventInvokeConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## DeleteFunctionRequestRequestTypeDef

```python
# DeleteFunctionRequestRequestTypeDef definition

class DeleteFunctionRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## DeleteFunctionUrlConfigRequestRequestTypeDef

```python
# DeleteFunctionUrlConfigRequestRequestTypeDef definition

class DeleteFunctionUrlConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## DeleteLayerVersionRequestRequestTypeDef

```python
# DeleteLayerVersionRequestRequestTypeDef definition

class DeleteLayerVersionRequestRequestTypeDef(TypedDict):
    LayerName: str,
    VersionNumber: int,
```

## DeleteProvisionedConcurrencyConfigRequestRequestTypeDef

```python
# DeleteProvisionedConcurrencyConfigRequestRequestTypeDef definition

class DeleteProvisionedConcurrencyConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: str,
```

## OnFailureTypeDef

```python
# OnFailureTypeDef definition

class OnFailureTypeDef(TypedDict):
    Destination: NotRequired[str],
```

## OnSuccessTypeDef

```python
# OnSuccessTypeDef definition

class OnSuccessTypeDef(TypedDict):
    Destination: NotRequired[str],
```

## EnvironmentErrorTypeDef

```python
# EnvironmentErrorTypeDef definition

class EnvironmentErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## FilterCriteriaErrorTypeDef

```python
# FilterCriteriaErrorTypeDef definition

class FilterCriteriaErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## SelfManagedEventSourceOutputTypeDef

```python
# SelfManagedEventSourceOutputTypeDef definition

class SelfManagedEventSourceOutputTypeDef(TypedDict):
    Endpoints: NotRequired[Dict[EndPointTypeType, List[str]]],  # (1)
```

1. See [:material-code-brackets: EndPointTypeType](./literals.md#endpointtypetype) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Pattern: NotRequired[str],
```

## FunctionCodeLocationTypeDef

```python
# FunctionCodeLocationTypeDef definition

class FunctionCodeLocationTypeDef(TypedDict):
    RepositoryType: NotRequired[str],
    Location: NotRequired[str],
    ImageUri: NotRequired[str],
    ResolvedImageUri: NotRequired[str],
```

## LayerTypeDef

```python
# LayerTypeDef definition

class LayerTypeDef(TypedDict):
    Arn: NotRequired[str],
    CodeSize: NotRequired[int],
    SigningProfileVersionArn: NotRequired[str],
    SigningJobArn: NotRequired[str],
```

## SnapStartResponseTypeDef

```python
# SnapStartResponseTypeDef definition

class SnapStartResponseTypeDef(TypedDict):
    ApplyOn: NotRequired[SnapStartApplyOnType],  # (1)
    OptimizationStatus: NotRequired[SnapStartOptimizationStatusType],  # (2)
```

1. See [:material-code-brackets: SnapStartApplyOnType](./literals.md#snapstartapplyontype) 
2. See [:material-code-brackets: SnapStartOptimizationStatusType](./literals.md#snapstartoptimizationstatustype) 
## TracingConfigResponseTypeDef

```python
# TracingConfigResponseTypeDef definition

class TracingConfigResponseTypeDef(TypedDict):
    Mode: NotRequired[TracingModeType],  # (1)
```

1. See [:material-code-brackets: TracingModeType](./literals.md#tracingmodetype) 
## VpcConfigResponseTypeDef

```python
# VpcConfigResponseTypeDef definition

class VpcConfigResponseTypeDef(TypedDict):
    SubnetIds: NotRequired[List[str]],
    SecurityGroupIds: NotRequired[List[str]],
    VpcId: NotRequired[str],
    Ipv6AllowedForDualStack: NotRequired[bool],
```

## GetAliasRequestRequestTypeDef

```python
# GetAliasRequestRequestTypeDef definition

class GetAliasRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Name: str,
```

## GetCodeSigningConfigRequestRequestTypeDef

```python
# GetCodeSigningConfigRequestRequestTypeDef definition

class GetCodeSigningConfigRequestRequestTypeDef(TypedDict):
    CodeSigningConfigArn: str,
```

## GetEventSourceMappingRequestRequestTypeDef

```python
# GetEventSourceMappingRequestRequestTypeDef definition

class GetEventSourceMappingRequestRequestTypeDef(TypedDict):
    UUID: str,
```

## GetFunctionCodeSigningConfigRequestRequestTypeDef

```python
# GetFunctionCodeSigningConfigRequestRequestTypeDef definition

class GetFunctionCodeSigningConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
```

## GetFunctionConcurrencyRequestRequestTypeDef

```python
# GetFunctionConcurrencyRequestRequestTypeDef definition

class GetFunctionConcurrencyRequestRequestTypeDef(TypedDict):
    FunctionName: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## GetFunctionConfigurationRequestRequestTypeDef

```python
# GetFunctionConfigurationRequestRequestTypeDef definition

class GetFunctionConfigurationRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## GetFunctionEventInvokeConfigRequestRequestTypeDef

```python
# GetFunctionEventInvokeConfigRequestRequestTypeDef definition

class GetFunctionEventInvokeConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## GetFunctionRecursionConfigRequestRequestTypeDef

```python
# GetFunctionRecursionConfigRequestRequestTypeDef definition

class GetFunctionRecursionConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
```

## GetFunctionRequestRequestTypeDef

```python
# GetFunctionRequestRequestTypeDef definition

class GetFunctionRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## GetFunctionUrlConfigRequestRequestTypeDef

```python
# GetFunctionUrlConfigRequestRequestTypeDef definition

class GetFunctionUrlConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## GetLayerVersionByArnRequestRequestTypeDef

```python
# GetLayerVersionByArnRequestRequestTypeDef definition

class GetLayerVersionByArnRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## GetLayerVersionPolicyRequestRequestTypeDef

```python
# GetLayerVersionPolicyRequestRequestTypeDef definition

class GetLayerVersionPolicyRequestRequestTypeDef(TypedDict):
    LayerName: str,
    VersionNumber: int,
```

## GetLayerVersionRequestRequestTypeDef

```python
# GetLayerVersionRequestRequestTypeDef definition

class GetLayerVersionRequestRequestTypeDef(TypedDict):
    LayerName: str,
    VersionNumber: int,
```

## LayerVersionContentOutputTypeDef

```python
# LayerVersionContentOutputTypeDef definition

class LayerVersionContentOutputTypeDef(TypedDict):
    Location: NotRequired[str],
    CodeSha256: NotRequired[str],
    CodeSize: NotRequired[int],
    SigningProfileVersionArn: NotRequired[str],
    SigningJobArn: NotRequired[str],
```

## GetPolicyRequestRequestTypeDef

```python
# GetPolicyRequestRequestTypeDef definition

class GetPolicyRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## GetProvisionedConcurrencyConfigRequestRequestTypeDef

```python
# GetProvisionedConcurrencyConfigRequestRequestTypeDef definition

class GetProvisionedConcurrencyConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: str,
```

## GetRuntimeManagementConfigRequestRequestTypeDef

```python
# GetRuntimeManagementConfigRequestRequestTypeDef definition

class GetRuntimeManagementConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
```

## ImageConfigErrorTypeDef

```python
# ImageConfigErrorTypeDef definition

class ImageConfigErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## ImageConfigOutputTypeDef

```python
# ImageConfigOutputTypeDef definition

class ImageConfigOutputTypeDef(TypedDict):
    EntryPoint: NotRequired[List[str]],
    Command: NotRequired[List[str]],
    WorkingDirectory: NotRequired[str],
```

## InvokeResponseStreamUpdateTypeDef

```python
# InvokeResponseStreamUpdateTypeDef definition

class InvokeResponseStreamUpdateTypeDef(TypedDict):
    Payload: NotRequired[bytes],
```

## InvokeWithResponseStreamCompleteEventTypeDef

```python
# InvokeWithResponseStreamCompleteEventTypeDef definition

class InvokeWithResponseStreamCompleteEventTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorDetails: NotRequired[str],
    LogResult: NotRequired[str],
```

## LayerVersionsListItemTypeDef

```python
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
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAliasesRequestRequestTypeDef

```python
# ListAliasesRequestRequestTypeDef definition

class ListAliasesRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    FunctionVersion: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListCodeSigningConfigsRequestRequestTypeDef

```python
# ListCodeSigningConfigsRequestRequestTypeDef definition

class ListCodeSigningConfigsRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListEventSourceMappingsRequestRequestTypeDef

```python
# ListEventSourceMappingsRequestRequestTypeDef definition

class ListEventSourceMappingsRequestRequestTypeDef(TypedDict):
    EventSourceArn: NotRequired[str],
    FunctionName: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListFunctionEventInvokeConfigsRequestRequestTypeDef

```python
# ListFunctionEventInvokeConfigsRequestRequestTypeDef definition

class ListFunctionEventInvokeConfigsRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListFunctionUrlConfigsRequestRequestTypeDef

```python
# ListFunctionUrlConfigsRequestRequestTypeDef definition

class ListFunctionUrlConfigsRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListFunctionsByCodeSigningConfigRequestRequestTypeDef

```python
# ListFunctionsByCodeSigningConfigRequestRequestTypeDef definition

class ListFunctionsByCodeSigningConfigRequestRequestTypeDef(TypedDict):
    CodeSigningConfigArn: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListFunctionsRequestRequestTypeDef

```python
# ListFunctionsRequestRequestTypeDef definition

class ListFunctionsRequestRequestTypeDef(TypedDict):
    MasterRegion: NotRequired[str],
    FunctionVersion: NotRequired[FunctionVersionType],  # (1)
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

1. See [:material-code-brackets: FunctionVersionType](./literals.md#functionversiontype) 
## ListLayerVersionsRequestRequestTypeDef

```python
# ListLayerVersionsRequestRequestTypeDef definition

class ListLayerVersionsRequestRequestTypeDef(TypedDict):
    LayerName: str,
    CompatibleRuntime: NotRequired[RuntimeType],  # (1)
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
    CompatibleArchitecture: NotRequired[ArchitectureType],  # (2)
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## ListLayersRequestRequestTypeDef

```python
# ListLayersRequestRequestTypeDef definition

class ListLayersRequestRequestTypeDef(TypedDict):
    CompatibleRuntime: NotRequired[RuntimeType],  # (1)
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
    CompatibleArchitecture: NotRequired[ArchitectureType],  # (2)
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## ListProvisionedConcurrencyConfigsRequestRequestTypeDef

```python
# ListProvisionedConcurrencyConfigsRequestRequestTypeDef definition

class ListProvisionedConcurrencyConfigsRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ProvisionedConcurrencyConfigListItemTypeDef

```python
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
## ListTagsRequestRequestTypeDef

```python
# ListTagsRequestRequestTypeDef definition

class ListTagsRequestRequestTypeDef(TypedDict):
    Resource: str,
```

## ListVersionsByFunctionRequestRequestTypeDef

```python
# ListVersionsByFunctionRequestRequestTypeDef definition

class ListVersionsByFunctionRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## PublishVersionRequestRequestTypeDef

```python
# PublishVersionRequestRequestTypeDef definition

class PublishVersionRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    CodeSha256: NotRequired[str],
    Description: NotRequired[str],
    RevisionId: NotRequired[str],
```

## PutFunctionCodeSigningConfigRequestRequestTypeDef

```python
# PutFunctionCodeSigningConfigRequestRequestTypeDef definition

class PutFunctionCodeSigningConfigRequestRequestTypeDef(TypedDict):
    CodeSigningConfigArn: str,
    FunctionName: str,
```

## PutFunctionConcurrencyRequestRequestTypeDef

```python
# PutFunctionConcurrencyRequestRequestTypeDef definition

class PutFunctionConcurrencyRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    ReservedConcurrentExecutions: int,
```

## PutFunctionRecursionConfigRequestRequestTypeDef

```python
# PutFunctionRecursionConfigRequestRequestTypeDef definition

class PutFunctionRecursionConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    RecursiveLoop: RecursiveLoopType,  # (1)
```

1. See [:material-code-brackets: RecursiveLoopType](./literals.md#recursivelooptype) 
## PutProvisionedConcurrencyConfigRequestRequestTypeDef

```python
# PutProvisionedConcurrencyConfigRequestRequestTypeDef definition

class PutProvisionedConcurrencyConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: str,
    ProvisionedConcurrentExecutions: int,
```

## PutRuntimeManagementConfigRequestRequestTypeDef

```python
# PutRuntimeManagementConfigRequestRequestTypeDef definition

class PutRuntimeManagementConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    UpdateRuntimeOn: UpdateRuntimeOnType,  # (1)
    Qualifier: NotRequired[str],
    RuntimeVersionArn: NotRequired[str],
```

1. See [:material-code-brackets: UpdateRuntimeOnType](./literals.md#updateruntimeontype) 
## RemoveLayerVersionPermissionRequestRequestTypeDef

```python
# RemoveLayerVersionPermissionRequestRequestTypeDef definition

class RemoveLayerVersionPermissionRequestRequestTypeDef(TypedDict):
    LayerName: str,
    VersionNumber: int,
    StatementId: str,
    RevisionId: NotRequired[str],
```

## RemovePermissionRequestRequestTypeDef

```python
# RemovePermissionRequestRequestTypeDef definition

class RemovePermissionRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    StatementId: str,
    Qualifier: NotRequired[str],
    RevisionId: NotRequired[str],
```

## RuntimeVersionErrorTypeDef

```python
# RuntimeVersionErrorTypeDef definition

class RuntimeVersionErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    Resource: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    Resource: str,
    TagKeys: Sequence[str],
```

## AddLayerVersionPermissionResponseTypeDef

```python
# AddLayerVersionPermissionResponseTypeDef definition

class AddLayerVersionPermissionResponseTypeDef(TypedDict):
    Statement: str,
    RevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddPermissionResponseTypeDef

```python
# AddPermissionResponseTypeDef definition

class AddPermissionResponseTypeDef(TypedDict):
    Statement: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConcurrencyResponseTypeDef

```python
# ConcurrencyResponseTypeDef definition

class ConcurrencyResponseTypeDef(TypedDict):
    ReservedConcurrentExecutions: int,
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
## GetAccountSettingsResponseTypeDef

```python
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
# GetFunctionCodeSigningConfigResponseTypeDef definition

class GetFunctionCodeSigningConfigResponseTypeDef(TypedDict):
    CodeSigningConfigArn: str,
    FunctionName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFunctionConcurrencyResponseTypeDef

```python
# GetFunctionConcurrencyResponseTypeDef definition

class GetFunctionConcurrencyResponseTypeDef(TypedDict):
    ReservedConcurrentExecutions: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFunctionRecursionConfigResponseTypeDef

```python
# GetFunctionRecursionConfigResponseTypeDef definition

class GetFunctionRecursionConfigResponseTypeDef(TypedDict):
    RecursiveLoop: RecursiveLoopType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RecursiveLoopType](./literals.md#recursivelooptype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLayerVersionPolicyResponseTypeDef

```python
# GetLayerVersionPolicyResponseTypeDef definition

class GetLayerVersionPolicyResponseTypeDef(TypedDict):
    Policy: str,
    RevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPolicyResponseTypeDef

```python
# GetPolicyResponseTypeDef definition

class GetPolicyResponseTypeDef(TypedDict):
    Policy: str,
    RevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProvisionedConcurrencyConfigResponseTypeDef

```python
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
# InvokeAsyncResponseTypeDef definition

class InvokeAsyncResponseTypeDef(TypedDict):
    Status: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFunctionsByCodeSigningConfigResponseTypeDef

```python
# ListFunctionsByCodeSigningConfigResponseTypeDef definition

class ListFunctionsByCodeSigningConfigResponseTypeDef(TypedDict):
    NextMarker: str,
    FunctionArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsResponseTypeDef

```python
# ListTagsResponseTypeDef definition

class ListTagsResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutFunctionCodeSigningConfigResponseTypeDef

```python
# PutFunctionCodeSigningConfigResponseTypeDef definition

class PutFunctionCodeSigningConfigResponseTypeDef(TypedDict):
    CodeSigningConfigArn: str,
    FunctionName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutFunctionRecursionConfigResponseTypeDef

```python
# PutFunctionRecursionConfigResponseTypeDef definition

class PutFunctionRecursionConfigResponseTypeDef(TypedDict):
    RecursiveLoop: RecursiveLoopType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RecursiveLoopType](./literals.md#recursivelooptype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutProvisionedConcurrencyConfigResponseTypeDef

```python
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
## CreateAliasRequestRequestTypeDef

```python
# CreateAliasRequestRequestTypeDef definition

class CreateAliasRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Name: str,
    FunctionVersion: str,
    Description: NotRequired[str],
    RoutingConfig: NotRequired[AliasRoutingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AliasRoutingConfigurationTypeDef](./type_defs.md#aliasroutingconfigurationtypedef) 
## UpdateAliasRequestRequestTypeDef

```python
# UpdateAliasRequestRequestTypeDef definition

class UpdateAliasRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Name: str,
    FunctionVersion: NotRequired[str],
    Description: NotRequired[str],
    RoutingConfig: NotRequired[AliasRoutingConfigurationTypeDef],  # (1)
    RevisionId: NotRequired[str],
```

1. See [:material-code-braces: AliasRoutingConfigurationTypeDef](./type_defs.md#aliasroutingconfigurationtypedef) 
## FunctionCodeTypeDef

```python
# FunctionCodeTypeDef definition

class FunctionCodeTypeDef(TypedDict):
    ZipFile: NotRequired[BlobTypeDef],
    S3Bucket: NotRequired[str],
    S3Key: NotRequired[str],
    S3ObjectVersion: NotRequired[str],
    ImageUri: NotRequired[str],
```

## InvocationRequestRequestTypeDef

```python
# InvocationRequestRequestTypeDef definition

class InvocationRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    InvocationType: NotRequired[InvocationTypeType],  # (1)
    LogType: NotRequired[LogTypeType],  # (2)
    ClientContext: NotRequired[str],
    Payload: NotRequired[BlobTypeDef],
    Qualifier: NotRequired[str],
```

1. See [:material-code-brackets: InvocationTypeType](./literals.md#invocationtypetype) 
2. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
## InvokeAsyncRequestRequestTypeDef

```python
# InvokeAsyncRequestRequestTypeDef definition

class InvokeAsyncRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    InvokeArgs: BlobTypeDef,
```

## InvokeWithResponseStreamRequestRequestTypeDef

```python
# InvokeWithResponseStreamRequestRequestTypeDef definition

class InvokeWithResponseStreamRequestRequestTypeDef(TypedDict):
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
# LayerVersionContentInputTypeDef definition

class LayerVersionContentInputTypeDef(TypedDict):
    S3Bucket: NotRequired[str],
    S3Key: NotRequired[str],
    S3ObjectVersion: NotRequired[str],
    ZipFile: NotRequired[BlobTypeDef],
```

## UpdateFunctionCodeRequestRequestTypeDef

```python
# UpdateFunctionCodeRequestRequestTypeDef definition

class UpdateFunctionCodeRequestRequestTypeDef(TypedDict):
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
```

1. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## CodeSigningConfigTypeDef

```python
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
## CreateCodeSigningConfigRequestRequestTypeDef

```python
# CreateCodeSigningConfigRequestRequestTypeDef definition

class CreateCodeSigningConfigRequestRequestTypeDef(TypedDict):
    AllowedPublishers: AllowedPublishersTypeDef,  # (1)
    Description: NotRequired[str],
    CodeSigningPolicies: NotRequired[CodeSigningPoliciesTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AllowedPublishersTypeDef](./type_defs.md#allowedpublisherstypedef) 
2. See [:material-code-braces: CodeSigningPoliciesTypeDef](./type_defs.md#codesigningpoliciestypedef) 
## UpdateCodeSigningConfigRequestRequestTypeDef

```python
# UpdateCodeSigningConfigRequestRequestTypeDef definition

class UpdateCodeSigningConfigRequestRequestTypeDef(TypedDict):
    CodeSigningConfigArn: str,
    Description: NotRequired[str],
    AllowedPublishers: NotRequired[AllowedPublishersTypeDef],  # (1)
    CodeSigningPolicies: NotRequired[CodeSigningPoliciesTypeDef],  # (2)
```

1. See [:material-code-braces: AllowedPublishersTypeDef](./type_defs.md#allowedpublisherstypedef) 
2. See [:material-code-braces: CodeSigningPoliciesTypeDef](./type_defs.md#codesigningpoliciestypedef) 
## CreateFunctionUrlConfigResponseTypeDef

```python
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
## CreateFunctionUrlConfigRequestRequestTypeDef

```python
# CreateFunctionUrlConfigRequestRequestTypeDef definition

class CreateFunctionUrlConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    AuthType: FunctionUrlAuthTypeType,  # (1)
    Qualifier: NotRequired[str],
    Cors: NotRequired[CorsTypeDef],  # (2)
    InvokeMode: NotRequired[InvokeModeType],  # (3)
```

1. See [:material-code-brackets: FunctionUrlAuthTypeType](./literals.md#functionurlauthtypetype) 
2. See [:material-code-braces: CorsTypeDef](./type_defs.md#corstypedef) 
3. See [:material-code-brackets: InvokeModeType](./literals.md#invokemodetype) 
## UpdateFunctionUrlConfigRequestRequestTypeDef

```python
# UpdateFunctionUrlConfigRequestRequestTypeDef definition

class UpdateFunctionUrlConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    AuthType: NotRequired[FunctionUrlAuthTypeType],  # (1)
    Cors: NotRequired[CorsTypeDef],  # (2)
    InvokeMode: NotRequired[InvokeModeType],  # (3)
```

1. See [:material-code-brackets: FunctionUrlAuthTypeType](./literals.md#functionurlauthtypetype) 
2. See [:material-code-braces: CorsTypeDef](./type_defs.md#corstypedef) 
3. See [:material-code-brackets: InvokeModeType](./literals.md#invokemodetype) 
## UpdateFunctionConfigurationRequestRequestTypeDef

```python
# UpdateFunctionConfigurationRequestRequestTypeDef definition

class UpdateFunctionConfigurationRequestRequestTypeDef(TypedDict):
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
    ImageConfig: NotRequired[ImageConfigTypeDef],  # (7)
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
7. See [:material-code-braces: ImageConfigTypeDef](./type_defs.md#imageconfigtypedef) 
8. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
9. See [:material-code-braces: SnapStartTypeDef](./type_defs.md#snapstarttypedef) 
10. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
## DestinationConfigTypeDef

```python
# DestinationConfigTypeDef definition

class DestinationConfigTypeDef(TypedDict):
    OnSuccess: NotRequired[OnSuccessTypeDef],  # (1)
    OnFailure: NotRequired[OnFailureTypeDef],  # (2)
```

1. See [:material-code-braces: OnSuccessTypeDef](./type_defs.md#onsuccesstypedef) 
2. See [:material-code-braces: OnFailureTypeDef](./type_defs.md#onfailuretypedef) 
## EnvironmentResponseTypeDef

```python
# EnvironmentResponseTypeDef definition

class EnvironmentResponseTypeDef(TypedDict):
    Variables: NotRequired[Dict[str, str]],
    Error: NotRequired[EnvironmentErrorTypeDef],  # (1)
```

1. See [:material-code-braces: EnvironmentErrorTypeDef](./type_defs.md#environmenterrortypedef) 
## FilterCriteriaOutputTypeDef

```python
# FilterCriteriaOutputTypeDef definition

class FilterCriteriaOutputTypeDef(TypedDict):
    Filters: NotRequired[List[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## FilterCriteriaTypeDef

```python
# FilterCriteriaTypeDef definition

class FilterCriteriaTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## GetFunctionConfigurationRequestFunctionActiveWaitTypeDef

```python
# GetFunctionConfigurationRequestFunctionActiveWaitTypeDef definition

class GetFunctionConfigurationRequestFunctionActiveWaitTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef

```python
# GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef definition

class GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef

```python
# GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef definition

class GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetFunctionRequestFunctionActiveV2WaitTypeDef

```python
# GetFunctionRequestFunctionActiveV2WaitTypeDef definition

class GetFunctionRequestFunctionActiveV2WaitTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetFunctionRequestFunctionExistsWaitTypeDef

```python
# GetFunctionRequestFunctionExistsWaitTypeDef definition

class GetFunctionRequestFunctionExistsWaitTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetFunctionRequestFunctionUpdatedV2WaitTypeDef

```python
# GetFunctionRequestFunctionUpdatedV2WaitTypeDef definition

class GetFunctionRequestFunctionUpdatedV2WaitTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetLayerVersionResponseTypeDef

```python
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
# ImageConfigResponseTypeDef definition

class ImageConfigResponseTypeDef(TypedDict):
    ImageConfig: NotRequired[ImageConfigOutputTypeDef],  # (1)
    Error: NotRequired[ImageConfigErrorTypeDef],  # (2)
```

1. See [:material-code-braces: ImageConfigOutputTypeDef](./type_defs.md#imageconfigoutputtypedef) 
2. See [:material-code-braces: ImageConfigErrorTypeDef](./type_defs.md#imageconfigerrortypedef) 
## InvokeWithResponseStreamResponseEventTypeDef

```python
# InvokeWithResponseStreamResponseEventTypeDef definition

class InvokeWithResponseStreamResponseEventTypeDef(TypedDict):
    PayloadChunk: NotRequired[InvokeResponseStreamUpdateTypeDef],  # (1)
    InvokeComplete: NotRequired[InvokeWithResponseStreamCompleteEventTypeDef],  # (2)
```

1. See [:material-code-braces: InvokeResponseStreamUpdateTypeDef](./type_defs.md#invokeresponsestreamupdatetypedef) 
2. See [:material-code-braces: InvokeWithResponseStreamCompleteEventTypeDef](./type_defs.md#invokewithresponsestreamcompleteeventtypedef) 
## LayersListItemTypeDef

```python
# LayersListItemTypeDef definition

class LayersListItemTypeDef(TypedDict):
    LayerName: NotRequired[str],
    LayerArn: NotRequired[str],
    LatestMatchingVersion: NotRequired[LayerVersionsListItemTypeDef],  # (1)
```

1. See [:material-code-braces: LayerVersionsListItemTypeDef](./type_defs.md#layerversionslistitemtypedef) 
## ListLayerVersionsResponseTypeDef

```python
# ListLayerVersionsResponseTypeDef definition

class ListLayerVersionsResponseTypeDef(TypedDict):
    NextMarker: str,
    LayerVersions: List[LayerVersionsListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LayerVersionsListItemTypeDef](./type_defs.md#layerversionslistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAliasesRequestListAliasesPaginateTypeDef

```python
# ListAliasesRequestListAliasesPaginateTypeDef definition

class ListAliasesRequestListAliasesPaginateTypeDef(TypedDict):
    FunctionName: str,
    FunctionVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef

```python
# ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef definition

class ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef

```python
# ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef definition

class ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef(TypedDict):
    EventSourceArn: NotRequired[str],
    FunctionName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef

```python
# ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef definition

class ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef(TypedDict):
    FunctionName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef

```python
# ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef definition

class ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef(TypedDict):
    FunctionName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef

```python
# ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef definition

class ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef(TypedDict):
    CodeSigningConfigArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFunctionsRequestListFunctionsPaginateTypeDef

```python
# ListFunctionsRequestListFunctionsPaginateTypeDef definition

class ListFunctionsRequestListFunctionsPaginateTypeDef(TypedDict):
    MasterRegion: NotRequired[str],
    FunctionVersion: NotRequired[FunctionVersionType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FunctionVersionType](./literals.md#functionversiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLayerVersionsRequestListLayerVersionsPaginateTypeDef

```python
# ListLayerVersionsRequestListLayerVersionsPaginateTypeDef definition

class ListLayerVersionsRequestListLayerVersionsPaginateTypeDef(TypedDict):
    LayerName: str,
    CompatibleRuntime: NotRequired[RuntimeType],  # (1)
    CompatibleArchitecture: NotRequired[ArchitectureType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLayersRequestListLayersPaginateTypeDef

```python
# ListLayersRequestListLayersPaginateTypeDef definition

class ListLayersRequestListLayersPaginateTypeDef(TypedDict):
    CompatibleRuntime: NotRequired[RuntimeType],  # (1)
    CompatibleArchitecture: NotRequired[ArchitectureType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef

```python
# ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef definition

class ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef(TypedDict):
    FunctionName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef

```python
# ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef definition

class ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef(TypedDict):
    FunctionName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProvisionedConcurrencyConfigsResponseTypeDef

```python
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
# RuntimeVersionConfigTypeDef definition

class RuntimeVersionConfigTypeDef(TypedDict):
    RuntimeVersionArn: NotRequired[str],
    Error: NotRequired[RuntimeVersionErrorTypeDef],  # (1)
```

1. See [:material-code-braces: RuntimeVersionErrorTypeDef](./type_defs.md#runtimeversionerrortypedef) 
## ListAliasesResponseTypeDef

```python
# ListAliasesResponseTypeDef definition

class ListAliasesResponseTypeDef(TypedDict):
    NextMarker: str,
    Aliases: List[AliasConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AliasConfigurationTypeDef](./type_defs.md#aliasconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFunctionRequestRequestTypeDef

```python
# CreateFunctionRequestRequestTypeDef definition

class CreateFunctionRequestRequestTypeDef(TypedDict):
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
    ImageConfig: NotRequired[ImageConfigTypeDef],  # (9)
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
9. See [:material-code-braces: ImageConfigTypeDef](./type_defs.md#imageconfigtypedef) 
10. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
11. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
12. See [:material-code-braces: SnapStartTypeDef](./type_defs.md#snapstarttypedef) 
13. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
## PublishLayerVersionRequestRequestTypeDef

```python
# PublishLayerVersionRequestRequestTypeDef definition

class PublishLayerVersionRequestRequestTypeDef(TypedDict):
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
# CreateCodeSigningConfigResponseTypeDef definition

class CreateCodeSigningConfigResponseTypeDef(TypedDict):
    CodeSigningConfig: CodeSigningConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeSigningConfigTypeDef](./type_defs.md#codesigningconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCodeSigningConfigResponseTypeDef

```python
# GetCodeSigningConfigResponseTypeDef definition

class GetCodeSigningConfigResponseTypeDef(TypedDict):
    CodeSigningConfig: CodeSigningConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeSigningConfigTypeDef](./type_defs.md#codesigningconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCodeSigningConfigsResponseTypeDef

```python
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
# UpdateCodeSigningConfigResponseTypeDef definition

class UpdateCodeSigningConfigResponseTypeDef(TypedDict):
    CodeSigningConfig: CodeSigningConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeSigningConfigTypeDef](./type_defs.md#codesigningconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFunctionUrlConfigsResponseTypeDef

```python
# ListFunctionUrlConfigsResponseTypeDef definition

class ListFunctionUrlConfigsResponseTypeDef(TypedDict):
    FunctionUrlConfigs: List[FunctionUrlConfigTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FunctionUrlConfigTypeDef](./type_defs.md#functionurlconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FunctionEventInvokeConfigResponseTypeDef

```python
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
# FunctionEventInvokeConfigTypeDef definition

class FunctionEventInvokeConfigTypeDef(TypedDict):
    LastModified: NotRequired[datetime],
    FunctionArn: NotRequired[str],
    MaximumRetryAttempts: NotRequired[int],
    MaximumEventAgeInSeconds: NotRequired[int],
    DestinationConfig: NotRequired[DestinationConfigTypeDef],  # (1)
```

1. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
## PutFunctionEventInvokeConfigRequestRequestTypeDef

```python
# PutFunctionEventInvokeConfigRequestRequestTypeDef definition

class PutFunctionEventInvokeConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    MaximumRetryAttempts: NotRequired[int],
    MaximumEventAgeInSeconds: NotRequired[int],
    DestinationConfig: NotRequired[DestinationConfigTypeDef],  # (1)
```

1. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
## UpdateFunctionEventInvokeConfigRequestRequestTypeDef

```python
# UpdateFunctionEventInvokeConfigRequestRequestTypeDef definition

class UpdateFunctionEventInvokeConfigRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    Qualifier: NotRequired[str],
    MaximumRetryAttempts: NotRequired[int],
    MaximumEventAgeInSeconds: NotRequired[int],
    DestinationConfig: NotRequired[DestinationConfigTypeDef],  # (1)
```

1. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
## EventSourceMappingConfigurationResponseTypeDef

```python
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (12)
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
12. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventSourceMappingConfigurationTypeDef

```python
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
## CreateEventSourceMappingRequestRequestTypeDef

```python
# CreateEventSourceMappingRequestRequestTypeDef definition

class CreateEventSourceMappingRequestRequestTypeDef(TypedDict):
    FunctionName: str,
    EventSourceArn: NotRequired[str],
    Enabled: NotRequired[bool],
    BatchSize: NotRequired[int],
    FilterCriteria: NotRequired[FilterCriteriaTypeDef],  # (1)
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
    SelfManagedEventSource: NotRequired[SelfManagedEventSourceTypeDef],  # (5)
    FunctionResponseTypes: NotRequired[Sequence[FunctionResponseTypeType]],  # (6)
    AmazonManagedKafkaEventSourceConfig: NotRequired[AmazonManagedKafkaEventSourceConfigTypeDef],  # (7)
    SelfManagedKafkaEventSourceConfig: NotRequired[SelfManagedKafkaEventSourceConfigTypeDef],  # (8)
    ScalingConfig: NotRequired[ScalingConfigTypeDef],  # (9)
    DocumentDBEventSourceConfig: NotRequired[DocumentDBEventSourceConfigTypeDef],  # (10)
    KMSKeyArn: NotRequired[str],
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-brackets: EventSourcePositionType](./literals.md#eventsourcepositiontype) 
3. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
4. See [:material-code-braces: SourceAccessConfigurationTypeDef](./type_defs.md#sourceaccessconfigurationtypedef) 
5. See [:material-code-braces: SelfManagedEventSourceTypeDef](./type_defs.md#selfmanagedeventsourcetypedef) 
6. See [:material-code-brackets: FunctionResponseTypeType](./literals.md#functionresponsetypetype) 
7. See [:material-code-braces: AmazonManagedKafkaEventSourceConfigTypeDef](./type_defs.md#amazonmanagedkafkaeventsourceconfigtypedef) 
8. See [:material-code-braces: SelfManagedKafkaEventSourceConfigTypeDef](./type_defs.md#selfmanagedkafkaeventsourceconfigtypedef) 
9. See [:material-code-braces: ScalingConfigTypeDef](./type_defs.md#scalingconfigtypedef) 
10. See [:material-code-braces: DocumentDBEventSourceConfigTypeDef](./type_defs.md#documentdbeventsourceconfigtypedef) 
## UpdateEventSourceMappingRequestRequestTypeDef

```python
# UpdateEventSourceMappingRequestRequestTypeDef definition

class UpdateEventSourceMappingRequestRequestTypeDef(TypedDict):
    UUID: str,
    FunctionName: NotRequired[str],
    Enabled: NotRequired[bool],
    BatchSize: NotRequired[int],
    FilterCriteria: NotRequired[FilterCriteriaTypeDef],  # (1)
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
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
3. See [:material-code-braces: SourceAccessConfigurationTypeDef](./type_defs.md#sourceaccessconfigurationtypedef) 
4. See [:material-code-brackets: FunctionResponseTypeType](./literals.md#functionresponsetypetype) 
5. See [:material-code-braces: ScalingConfigTypeDef](./type_defs.md#scalingconfigtypedef) 
6. See [:material-code-braces: DocumentDBEventSourceConfigTypeDef](./type_defs.md#documentdbeventsourceconfigtypedef) 
## InvokeWithResponseStreamResponseTypeDef

```python
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
# ListEventSourceMappingsResponseTypeDef definition

class ListEventSourceMappingsResponseTypeDef(TypedDict):
    NextMarker: str,
    EventSourceMappings: List[EventSourceMappingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSourceMappingConfigurationTypeDef](./type_defs.md#eventsourcemappingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFunctionResponseTypeDef

```python
# GetFunctionResponseTypeDef definition

class GetFunctionResponseTypeDef(TypedDict):
    Configuration: FunctionConfigurationTypeDef,  # (1)
    Code: FunctionCodeLocationTypeDef,  # (2)
    Tags: Dict[str, str],
    Concurrency: ConcurrencyTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: FunctionConfigurationTypeDef](./type_defs.md#functionconfigurationtypedef) 
2. See [:material-code-braces: FunctionCodeLocationTypeDef](./type_defs.md#functioncodelocationtypedef) 
3. See [:material-code-braces: ConcurrencyTypeDef](./type_defs.md#concurrencytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFunctionsResponseTypeDef

```python
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
# ListVersionsByFunctionResponseTypeDef definition

class ListVersionsByFunctionResponseTypeDef(TypedDict):
    NextMarker: str,
    Versions: List[FunctionConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FunctionConfigurationTypeDef](./type_defs.md#functionconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
