# Type definitions

> [Index](../README.md) > [DeviceFarm](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DeviceFarm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
    type annotations stubs module [types-aiobotocore-devicefarm](https://pypi.org/project/types-aiobotocore-devicefarm/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## CustomerArtifactPathsUnionTypeDef

```python
# CustomerArtifactPathsUnionTypeDef definition

CustomerArtifactPathsUnionTypeDef = Union[
    CustomerArtifactPathsTypeDef,  # (1)
    CustomerArtifactPathsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomerArtifactPathsTypeDef](./type_defs.md#customerartifactpathstypedef) 
2. See [:material-code-braces: CustomerArtifactPathsOutputTypeDef](./type_defs.md#customerartifactpathsoutputtypedef) 

## DeviceFilterUnionTypeDef

```python
# DeviceFilterUnionTypeDef definition

DeviceFilterUnionTypeDef = Union[
    DeviceFilterTypeDef,  # (1)
    DeviceFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DeviceFilterTypeDef](./type_defs.md#devicefiltertypedef) 
2. See [:material-code-braces: DeviceFilterOutputTypeDef](./type_defs.md#devicefilteroutputtypedef) 



## TrialMinutesTypeDef

```python
# TrialMinutesTypeDef definition

class TrialMinutesTypeDef(TypedDict):
    total: NotRequired[float],
    remaining: NotRequired[float],
```

## ArtifactTypeDef

```python
# ArtifactTypeDef definition

class ArtifactTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    type: NotRequired[ArtifactTypeType],  # (1)
    extension: NotRequired[str],
    url: NotRequired[str],
```

1. See [:material-code-brackets: ArtifactTypeType](./literals.md#artifacttypetype) 
## CPUTypeDef

```python
# CPUTypeDef definition

class CPUTypeDef(TypedDict):
    frequency: NotRequired[str],
    architecture: NotRequired[str],
    clock: NotRequired[float],
```

## CountersTypeDef

```python
# CountersTypeDef definition

class CountersTypeDef(TypedDict):
    total: NotRequired[int],
    passed: NotRequired[int],
    failed: NotRequired[int],
    warned: NotRequired[int],
    errored: NotRequired[int],
    stopped: NotRequired[int],
    skipped: NotRequired[int],
```

## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    attribute: NotRequired[DeviceAttributeType],  # (1)
    operator: NotRequired[RuleOperatorType],  # (2)
    value: NotRequired[str],
```

1. See [:material-code-brackets: DeviceAttributeType](./literals.md#deviceattributetype) 
2. See [:material-code-brackets: RuleOperatorType](./literals.md#ruleoperatortype) 
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

## CreateInstanceProfileRequestRequestTypeDef

```python
# CreateInstanceProfileRequestRequestTypeDef definition

class CreateInstanceProfileRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    packageCleanup: NotRequired[bool],
    excludeAppPackagesFromCleanup: NotRequired[Sequence[str]],
    rebootAfterUse: NotRequired[bool],
```

## InstanceProfileTypeDef

```python
# InstanceProfileTypeDef definition

class InstanceProfileTypeDef(TypedDict):
    arn: NotRequired[str],
    packageCleanup: NotRequired[bool],
    excludeAppPackagesFromCleanup: NotRequired[List[str]],
    rebootAfterUse: NotRequired[bool],
    name: NotRequired[str],
    description: NotRequired[str],
```

## CreateNetworkProfileRequestRequestTypeDef

```python
# CreateNetworkProfileRequestRequestTypeDef definition

class CreateNetworkProfileRequestRequestTypeDef(TypedDict):
    projectArn: str,
    name: str,
    description: NotRequired[str],
    type: NotRequired[NetworkProfileTypeType],  # (1)
    uplinkBandwidthBits: NotRequired[int],
    downlinkBandwidthBits: NotRequired[int],
    uplinkDelayMs: NotRequired[int],
    downlinkDelayMs: NotRequired[int],
    uplinkJitterMs: NotRequired[int],
    downlinkJitterMs: NotRequired[int],
    uplinkLossPercent: NotRequired[int],
    downlinkLossPercent: NotRequired[int],
```

1. See [:material-code-brackets: NetworkProfileTypeType](./literals.md#networkprofiletypetype) 
## NetworkProfileTypeDef

```python
# NetworkProfileTypeDef definition

class NetworkProfileTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    type: NotRequired[NetworkProfileTypeType],  # (1)
    uplinkBandwidthBits: NotRequired[int],
    downlinkBandwidthBits: NotRequired[int],
    uplinkDelayMs: NotRequired[int],
    downlinkDelayMs: NotRequired[int],
    uplinkJitterMs: NotRequired[int],
    downlinkJitterMs: NotRequired[int],
    uplinkLossPercent: NotRequired[int],
    downlinkLossPercent: NotRequired[int],
```

1. See [:material-code-brackets: NetworkProfileTypeType](./literals.md#networkprofiletypetype) 
## VpcConfigTypeDef

```python
# VpcConfigTypeDef definition

class VpcConfigTypeDef(TypedDict):
    securityGroupIds: Sequence[str],
    subnetIds: Sequence[str],
    vpcId: str,
```

## CreateRemoteAccessSessionConfigurationTypeDef

```python
# CreateRemoteAccessSessionConfigurationTypeDef definition

class CreateRemoteAccessSessionConfigurationTypeDef(TypedDict):
    billingMethod: NotRequired[BillingMethodType],  # (1)
    vpceConfigurationArns: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: BillingMethodType](./literals.md#billingmethodtype) 
## TestGridVpcConfigTypeDef

```python
# TestGridVpcConfigTypeDef definition

class TestGridVpcConfigTypeDef(TypedDict):
    securityGroupIds: Sequence[str],
    subnetIds: Sequence[str],
    vpcId: str,
```

## CreateTestGridUrlRequestRequestTypeDef

```python
# CreateTestGridUrlRequestRequestTypeDef definition

class CreateTestGridUrlRequestRequestTypeDef(TypedDict):
    projectArn: str,
    expiresInSeconds: int,
```

## CreateUploadRequestRequestTypeDef

```python
# CreateUploadRequestRequestTypeDef definition

class CreateUploadRequestRequestTypeDef(TypedDict):
    projectArn: str,
    name: str,
    type: UploadTypeType,  # (1)
    contentType: NotRequired[str],
```

1. See [:material-code-brackets: UploadTypeType](./literals.md#uploadtypetype) 
## UploadTypeDef

```python
# UploadTypeDef definition

class UploadTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    created: NotRequired[datetime],
    type: NotRequired[UploadTypeType],  # (1)
    status: NotRequired[UploadStatusType],  # (2)
    url: NotRequired[str],
    metadata: NotRequired[str],
    contentType: NotRequired[str],
    message: NotRequired[str],
    category: NotRequired[UploadCategoryType],  # (3)
```

1. See [:material-code-brackets: UploadTypeType](./literals.md#uploadtypetype) 
2. See [:material-code-brackets: UploadStatusType](./literals.md#uploadstatustype) 
3. See [:material-code-brackets: UploadCategoryType](./literals.md#uploadcategorytype) 
## CreateVPCEConfigurationRequestRequestTypeDef

```python
# CreateVPCEConfigurationRequestRequestTypeDef definition

class CreateVPCEConfigurationRequestRequestTypeDef(TypedDict):
    vpceConfigurationName: str,
    vpceServiceName: str,
    serviceDnsName: str,
    vpceConfigurationDescription: NotRequired[str],
```

## VPCEConfigurationTypeDef

```python
# VPCEConfigurationTypeDef definition

class VPCEConfigurationTypeDef(TypedDict):
    arn: NotRequired[str],
    vpceConfigurationName: NotRequired[str],
    vpceServiceName: NotRequired[str],
    serviceDnsName: NotRequired[str],
    vpceConfigurationDescription: NotRequired[str],
```

## CustomerArtifactPathsOutputTypeDef

```python
# CustomerArtifactPathsOutputTypeDef definition

class CustomerArtifactPathsOutputTypeDef(TypedDict):
    iosPaths: NotRequired[List[str]],
    androidPaths: NotRequired[List[str]],
    deviceHostPaths: NotRequired[List[str]],
```

## CustomerArtifactPathsTypeDef

```python
# CustomerArtifactPathsTypeDef definition

class CustomerArtifactPathsTypeDef(TypedDict):
    iosPaths: NotRequired[Sequence[str]],
    androidPaths: NotRequired[Sequence[str]],
    deviceHostPaths: NotRequired[Sequence[str]],
```

## DeleteDevicePoolRequestRequestTypeDef

```python
# DeleteDevicePoolRequestRequestTypeDef definition

class DeleteDevicePoolRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteInstanceProfileRequestRequestTypeDef

```python
# DeleteInstanceProfileRequestRequestTypeDef definition

class DeleteInstanceProfileRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteNetworkProfileRequestRequestTypeDef

```python
# DeleteNetworkProfileRequestRequestTypeDef definition

class DeleteNetworkProfileRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteProjectRequestRequestTypeDef

```python
# DeleteProjectRequestRequestTypeDef definition

class DeleteProjectRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteRemoteAccessSessionRequestRequestTypeDef

```python
# DeleteRemoteAccessSessionRequestRequestTypeDef definition

class DeleteRemoteAccessSessionRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteRunRequestRequestTypeDef

```python
# DeleteRunRequestRequestTypeDef definition

class DeleteRunRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteTestGridProjectRequestRequestTypeDef

```python
# DeleteTestGridProjectRequestRequestTypeDef definition

class DeleteTestGridProjectRequestRequestTypeDef(TypedDict):
    projectArn: str,
```

## DeleteUploadRequestRequestTypeDef

```python
# DeleteUploadRequestRequestTypeDef definition

class DeleteUploadRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteVPCEConfigurationRequestRequestTypeDef

```python
# DeleteVPCEConfigurationRequestRequestTypeDef definition

class DeleteVPCEConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeviceFilterOutputTypeDef

```python
# DeviceFilterOutputTypeDef definition

class DeviceFilterOutputTypeDef(TypedDict):
    attribute: DeviceFilterAttributeType,  # (1)
    operator: RuleOperatorType,  # (2)
    values: List[str],
```

1. See [:material-code-brackets: DeviceFilterAttributeType](./literals.md#devicefilterattributetype) 
2. See [:material-code-brackets: RuleOperatorType](./literals.md#ruleoperatortype) 
## DeviceFilterTypeDef

```python
# DeviceFilterTypeDef definition

class DeviceFilterTypeDef(TypedDict):
    attribute: DeviceFilterAttributeType,  # (1)
    operator: RuleOperatorType,  # (2)
    values: Sequence[str],
```

1. See [:material-code-brackets: DeviceFilterAttributeType](./literals.md#devicefilterattributetype) 
2. See [:material-code-brackets: RuleOperatorType](./literals.md#ruleoperatortype) 
## DeviceMinutesTypeDef

```python
# DeviceMinutesTypeDef definition

class DeviceMinutesTypeDef(TypedDict):
    total: NotRequired[float],
    metered: NotRequired[float],
    unmetered: NotRequired[float],
```

## IncompatibilityMessageTypeDef

```python
# IncompatibilityMessageTypeDef definition

class IncompatibilityMessageTypeDef(TypedDict):
    message: NotRequired[str],
    type: NotRequired[DeviceAttributeType],  # (1)
```

1. See [:material-code-brackets: DeviceAttributeType](./literals.md#deviceattributetype) 
## ResolutionTypeDef

```python
# ResolutionTypeDef definition

class ResolutionTypeDef(TypedDict):
    width: NotRequired[int],
    height: NotRequired[int],
```

## ExecutionConfigurationTypeDef

```python
# ExecutionConfigurationTypeDef definition

class ExecutionConfigurationTypeDef(TypedDict):
    jobTimeoutMinutes: NotRequired[int],
    accountsCleanup: NotRequired[bool],
    appPackagesCleanup: NotRequired[bool],
    videoCapture: NotRequired[bool],
    skipAppResign: NotRequired[bool],
```

## GetDeviceInstanceRequestRequestTypeDef

```python
# GetDeviceInstanceRequestRequestTypeDef definition

class GetDeviceInstanceRequestRequestTypeDef(TypedDict):
    arn: str,
```

## ScheduleRunTestTypeDef

```python
# ScheduleRunTestTypeDef definition

class ScheduleRunTestTypeDef(TypedDict):
    type: TestTypeType,  # (1)
    testPackageArn: NotRequired[str],
    testSpecArn: NotRequired[str],
    filter: NotRequired[str],
    parameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: TestTypeType](./literals.md#testtypetype) 
## GetDevicePoolRequestRequestTypeDef

```python
# GetDevicePoolRequestRequestTypeDef definition

class GetDevicePoolRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetDeviceRequestRequestTypeDef

```python
# GetDeviceRequestRequestTypeDef definition

class GetDeviceRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetInstanceProfileRequestRequestTypeDef

```python
# GetInstanceProfileRequestRequestTypeDef definition

class GetInstanceProfileRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetJobRequestRequestTypeDef

```python
# GetJobRequestRequestTypeDef definition

class GetJobRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetNetworkProfileRequestRequestTypeDef

```python
# GetNetworkProfileRequestRequestTypeDef definition

class GetNetworkProfileRequestRequestTypeDef(TypedDict):
    arn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetOfferingStatusRequestRequestTypeDef

```python
# GetOfferingStatusRequestRequestTypeDef definition

class GetOfferingStatusRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
```

## GetProjectRequestRequestTypeDef

```python
# GetProjectRequestRequestTypeDef definition

class GetProjectRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetRemoteAccessSessionRequestRequestTypeDef

```python
# GetRemoteAccessSessionRequestRequestTypeDef definition

class GetRemoteAccessSessionRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetRunRequestRequestTypeDef

```python
# GetRunRequestRequestTypeDef definition

class GetRunRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetSuiteRequestRequestTypeDef

```python
# GetSuiteRequestRequestTypeDef definition

class GetSuiteRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetTestGridProjectRequestRequestTypeDef

```python
# GetTestGridProjectRequestRequestTypeDef definition

class GetTestGridProjectRequestRequestTypeDef(TypedDict):
    projectArn: str,
```

## GetTestGridSessionRequestRequestTypeDef

```python
# GetTestGridSessionRequestRequestTypeDef definition

class GetTestGridSessionRequestRequestTypeDef(TypedDict):
    projectArn: NotRequired[str],
    sessionId: NotRequired[str],
    sessionArn: NotRequired[str],
```

## TestGridSessionTypeDef

```python
# TestGridSessionTypeDef definition

class TestGridSessionTypeDef(TypedDict):
    arn: NotRequired[str],
    status: NotRequired[TestGridSessionStatusType],  # (1)
    created: NotRequired[datetime],
    ended: NotRequired[datetime],
    billingMinutes: NotRequired[float],
    seleniumProperties: NotRequired[str],
```

1. See [:material-code-brackets: TestGridSessionStatusType](./literals.md#testgridsessionstatustype) 
## GetTestRequestRequestTypeDef

```python
# GetTestRequestRequestTypeDef definition

class GetTestRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetUploadRequestRequestTypeDef

```python
# GetUploadRequestRequestTypeDef definition

class GetUploadRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetVPCEConfigurationRequestRequestTypeDef

```python
# GetVPCEConfigurationRequestRequestTypeDef definition

class GetVPCEConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## InstallToRemoteAccessSessionRequestRequestTypeDef

```python
# InstallToRemoteAccessSessionRequestRequestTypeDef definition

class InstallToRemoteAccessSessionRequestRequestTypeDef(TypedDict):
    remoteAccessSessionArn: str,
    appArn: str,
```

## ListArtifactsRequestRequestTypeDef

```python
# ListArtifactsRequestRequestTypeDef definition

class ListArtifactsRequestRequestTypeDef(TypedDict):
    arn: str,
    type: ArtifactCategoryType,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: ArtifactCategoryType](./literals.md#artifactcategorytype) 
## ListDeviceInstancesRequestRequestTypeDef

```python
# ListDeviceInstancesRequestRequestTypeDef definition

class ListDeviceInstancesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDevicePoolsRequestRequestTypeDef

```python
# ListDevicePoolsRequestRequestTypeDef definition

class ListDevicePoolsRequestRequestTypeDef(TypedDict):
    arn: str,
    type: NotRequired[DevicePoolTypeType],  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: DevicePoolTypeType](./literals.md#devicepooltypetype) 
## ListInstanceProfilesRequestRequestTypeDef

```python
# ListInstanceProfilesRequestRequestTypeDef definition

class ListInstanceProfilesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListJobsRequestRequestTypeDef

```python
# ListJobsRequestRequestTypeDef definition

class ListJobsRequestRequestTypeDef(TypedDict):
    arn: str,
    nextToken: NotRequired[str],
```

## ListNetworkProfilesRequestRequestTypeDef

```python
# ListNetworkProfilesRequestRequestTypeDef definition

class ListNetworkProfilesRequestRequestTypeDef(TypedDict):
    arn: str,
    type: NotRequired[NetworkProfileTypeType],  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: NetworkProfileTypeType](./literals.md#networkprofiletypetype) 
## ListOfferingPromotionsRequestRequestTypeDef

```python
# ListOfferingPromotionsRequestRequestTypeDef definition

class ListOfferingPromotionsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
```

## OfferingPromotionTypeDef

```python
# OfferingPromotionTypeDef definition

class OfferingPromotionTypeDef(TypedDict):
    id: NotRequired[str],
    description: NotRequired[str],
```

## ListOfferingTransactionsRequestRequestTypeDef

```python
# ListOfferingTransactionsRequestRequestTypeDef definition

class ListOfferingTransactionsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
```

## ListOfferingsRequestRequestTypeDef

```python
# ListOfferingsRequestRequestTypeDef definition

class ListOfferingsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
```

## ListProjectsRequestRequestTypeDef

```python
# ListProjectsRequestRequestTypeDef definition

class ListProjectsRequestRequestTypeDef(TypedDict):
    arn: NotRequired[str],
    nextToken: NotRequired[str],
```

## ListRemoteAccessSessionsRequestRequestTypeDef

```python
# ListRemoteAccessSessionsRequestRequestTypeDef definition

class ListRemoteAccessSessionsRequestRequestTypeDef(TypedDict):
    arn: str,
    nextToken: NotRequired[str],
```

## ListRunsRequestRequestTypeDef

```python
# ListRunsRequestRequestTypeDef definition

class ListRunsRequestRequestTypeDef(TypedDict):
    arn: str,
    nextToken: NotRequired[str],
```

## ListSamplesRequestRequestTypeDef

```python
# ListSamplesRequestRequestTypeDef definition

class ListSamplesRequestRequestTypeDef(TypedDict):
    arn: str,
    nextToken: NotRequired[str],
```

## SampleTypeDef

```python
# SampleTypeDef definition

class SampleTypeDef(TypedDict):
    arn: NotRequired[str],
    type: NotRequired[SampleTypeType],  # (1)
    url: NotRequired[str],
```

1. See [:material-code-brackets: SampleTypeType](./literals.md#sampletypetype) 
## ListSuitesRequestRequestTypeDef

```python
# ListSuitesRequestRequestTypeDef definition

class ListSuitesRequestRequestTypeDef(TypedDict):
    arn: str,
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## ListTestGridProjectsRequestRequestTypeDef

```python
# ListTestGridProjectsRequestRequestTypeDef definition

class ListTestGridProjectsRequestRequestTypeDef(TypedDict):
    maxResult: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTestGridSessionActionsRequestRequestTypeDef

```python
# ListTestGridSessionActionsRequestRequestTypeDef definition

class ListTestGridSessionActionsRequestRequestTypeDef(TypedDict):
    sessionArn: str,
    maxResult: NotRequired[int],
    nextToken: NotRequired[str],
```

## TestGridSessionActionTypeDef

```python
# TestGridSessionActionTypeDef definition

class TestGridSessionActionTypeDef(TypedDict):
    action: NotRequired[str],
    started: NotRequired[datetime],
    duration: NotRequired[int],
    statusCode: NotRequired[str],
    requestMethod: NotRequired[str],
```

## ListTestGridSessionArtifactsRequestRequestTypeDef

```python
# ListTestGridSessionArtifactsRequestRequestTypeDef definition

class ListTestGridSessionArtifactsRequestRequestTypeDef(TypedDict):
    sessionArn: str,
    type: NotRequired[TestGridSessionArtifactCategoryType],  # (1)
    maxResult: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: TestGridSessionArtifactCategoryType](./literals.md#testgridsessionartifactcategorytype) 
## TestGridSessionArtifactTypeDef

```python
# TestGridSessionArtifactTypeDef definition

class TestGridSessionArtifactTypeDef(TypedDict):
    filename: NotRequired[str],
    type: NotRequired[TestGridSessionArtifactTypeType],  # (1)
    url: NotRequired[str],
```

1. See [:material-code-brackets: TestGridSessionArtifactTypeType](./literals.md#testgridsessionartifacttypetype) 
## ListTestsRequestRequestTypeDef

```python
# ListTestsRequestRequestTypeDef definition

class ListTestsRequestRequestTypeDef(TypedDict):
    arn: str,
    nextToken: NotRequired[str],
```

## ListUniqueProblemsRequestRequestTypeDef

```python
# ListUniqueProblemsRequestRequestTypeDef definition

class ListUniqueProblemsRequestRequestTypeDef(TypedDict):
    arn: str,
    nextToken: NotRequired[str],
```

## ListUploadsRequestRequestTypeDef

```python
# ListUploadsRequestRequestTypeDef definition

class ListUploadsRequestRequestTypeDef(TypedDict):
    arn: str,
    type: NotRequired[UploadTypeType],  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: UploadTypeType](./literals.md#uploadtypetype) 
## ListVPCEConfigurationsRequestRequestTypeDef

```python
# ListVPCEConfigurationsRequestRequestTypeDef definition

class ListVPCEConfigurationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## LocationTypeDef

```python
# LocationTypeDef definition

class LocationTypeDef(TypedDict):
    latitude: float,
    longitude: float,
```

## MonetaryAmountTypeDef

```python
# MonetaryAmountTypeDef definition

class MonetaryAmountTypeDef(TypedDict):
    amount: NotRequired[float],
    currencyCode: NotRequired[CurrencyCodeType],  # (1)
```

1. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
## ProblemDetailTypeDef

```python
# ProblemDetailTypeDef definition

class ProblemDetailTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
```

## VpcConfigOutputTypeDef

```python
# VpcConfigOutputTypeDef definition

class VpcConfigOutputTypeDef(TypedDict):
    securityGroupIds: List[str],
    subnetIds: List[str],
    vpcId: str,
```

## PurchaseOfferingRequestRequestTypeDef

```python
# PurchaseOfferingRequestRequestTypeDef definition

class PurchaseOfferingRequestRequestTypeDef(TypedDict):
    offeringId: str,
    quantity: int,
    offeringPromotionId: NotRequired[str],
```

## RadiosTypeDef

```python
# RadiosTypeDef definition

class RadiosTypeDef(TypedDict):
    wifi: NotRequired[bool],
    bluetooth: NotRequired[bool],
    nfc: NotRequired[bool],
    gps: NotRequired[bool],
```

## RenewOfferingRequestRequestTypeDef

```python
# RenewOfferingRequestRequestTypeDef definition

class RenewOfferingRequestRequestTypeDef(TypedDict):
    offeringId: str,
    quantity: int,
```

## StopJobRequestRequestTypeDef

```python
# StopJobRequestRequestTypeDef definition

class StopJobRequestRequestTypeDef(TypedDict):
    arn: str,
```

## StopRemoteAccessSessionRequestRequestTypeDef

```python
# StopRemoteAccessSessionRequestRequestTypeDef definition

class StopRemoteAccessSessionRequestRequestTypeDef(TypedDict):
    arn: str,
```

## StopRunRequestRequestTypeDef

```python
# StopRunRequestRequestTypeDef definition

class StopRunRequestRequestTypeDef(TypedDict):
    arn: str,
```

## TestGridVpcConfigOutputTypeDef

```python
# TestGridVpcConfigOutputTypeDef definition

class TestGridVpcConfigOutputTypeDef(TypedDict):
    securityGroupIds: List[str],
    subnetIds: List[str],
    vpcId: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateDeviceInstanceRequestRequestTypeDef

```python
# UpdateDeviceInstanceRequestRequestTypeDef definition

class UpdateDeviceInstanceRequestRequestTypeDef(TypedDict):
    arn: str,
    profileArn: NotRequired[str],
    labels: NotRequired[Sequence[str]],
```

## UpdateInstanceProfileRequestRequestTypeDef

```python
# UpdateInstanceProfileRequestRequestTypeDef definition

class UpdateInstanceProfileRequestRequestTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    description: NotRequired[str],
    packageCleanup: NotRequired[bool],
    excludeAppPackagesFromCleanup: NotRequired[Sequence[str]],
    rebootAfterUse: NotRequired[bool],
```

## UpdateNetworkProfileRequestRequestTypeDef

```python
# UpdateNetworkProfileRequestRequestTypeDef definition

class UpdateNetworkProfileRequestRequestTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    description: NotRequired[str],
    type: NotRequired[NetworkProfileTypeType],  # (1)
    uplinkBandwidthBits: NotRequired[int],
    downlinkBandwidthBits: NotRequired[int],
    uplinkDelayMs: NotRequired[int],
    downlinkDelayMs: NotRequired[int],
    uplinkJitterMs: NotRequired[int],
    downlinkJitterMs: NotRequired[int],
    uplinkLossPercent: NotRequired[int],
    downlinkLossPercent: NotRequired[int],
```

1. See [:material-code-brackets: NetworkProfileTypeType](./literals.md#networkprofiletypetype) 
## UpdateUploadRequestRequestTypeDef

```python
# UpdateUploadRequestRequestTypeDef definition

class UpdateUploadRequestRequestTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    contentType: NotRequired[str],
    editContent: NotRequired[bool],
```

## UpdateVPCEConfigurationRequestRequestTypeDef

```python
# UpdateVPCEConfigurationRequestRequestTypeDef definition

class UpdateVPCEConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
    vpceConfigurationName: NotRequired[str],
    vpceServiceName: NotRequired[str],
    serviceDnsName: NotRequired[str],
    vpceConfigurationDescription: NotRequired[str],
```

## AccountSettingsTypeDef

```python
# AccountSettingsTypeDef definition

class AccountSettingsTypeDef(TypedDict):
    awsAccountNumber: NotRequired[str],
    unmeteredDevices: NotRequired[Dict[DevicePlatformType, int]],  # (1)
    unmeteredRemoteAccessDevices: NotRequired[Dict[DevicePlatformType, int]],  # (1)
    maxJobTimeoutMinutes: NotRequired[int],
    trialMinutes: NotRequired[TrialMinutesTypeDef],  # (3)
    maxSlots: NotRequired[Dict[str, int]],
    defaultJobTimeoutMinutes: NotRequired[int],
    skipAppResign: NotRequired[bool],
```

1. See [:material-code-brackets: DevicePlatformType](./literals.md#deviceplatformtype) 
2. See [:material-code-brackets: DevicePlatformType](./literals.md#deviceplatformtype) 
3. See [:material-code-braces: TrialMinutesTypeDef](./type_defs.md#trialminutestypedef) 
## CreateDevicePoolRequestRequestTypeDef

```python
# CreateDevicePoolRequestRequestTypeDef definition

class CreateDevicePoolRequestRequestTypeDef(TypedDict):
    projectArn: str,
    name: str,
    rules: Sequence[RuleTypeDef],  # (1)
    description: NotRequired[str],
    maxDevices: NotRequired[int],
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
## DevicePoolTypeDef

```python
# DevicePoolTypeDef definition

class DevicePoolTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    type: NotRequired[DevicePoolTypeType],  # (1)
    rules: NotRequired[List[RuleTypeDef]],  # (2)
    maxDevices: NotRequired[int],
```

1. See [:material-code-brackets: DevicePoolTypeType](./literals.md#devicepooltypetype) 
2. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
## UpdateDevicePoolRequestRequestTypeDef

```python
# UpdateDevicePoolRequestRequestTypeDef definition

class UpdateDevicePoolRequestRequestTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    description: NotRequired[str],
    rules: NotRequired[Sequence[RuleTypeDef]],  # (1)
    maxDevices: NotRequired[int],
    clearMaxDevices: NotRequired[bool],
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
## CreateTestGridUrlResultTypeDef

```python
# CreateTestGridUrlResultTypeDef definition

class CreateTestGridUrlResultTypeDef(TypedDict):
    url: str,
    expires: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListArtifactsResultTypeDef

```python
# ListArtifactsResultTypeDef definition

class ListArtifactsResultTypeDef(TypedDict):
    artifacts: List[ArtifactTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ArtifactTypeDef](./type_defs.md#artifacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceProfileResultTypeDef

```python
# CreateInstanceProfileResultTypeDef definition

class CreateInstanceProfileResultTypeDef(TypedDict):
    instanceProfile: InstanceProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeviceInstanceTypeDef

```python
# DeviceInstanceTypeDef definition

class DeviceInstanceTypeDef(TypedDict):
    arn: NotRequired[str],
    deviceArn: NotRequired[str],
    labels: NotRequired[List[str]],
    status: NotRequired[InstanceStatusType],  # (1)
    udid: NotRequired[str],
    instanceProfile: NotRequired[InstanceProfileTypeDef],  # (2)
```

1. See [:material-code-brackets: InstanceStatusType](./literals.md#instancestatustype) 
2. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
## GetInstanceProfileResultTypeDef

```python
# GetInstanceProfileResultTypeDef definition

class GetInstanceProfileResultTypeDef(TypedDict):
    instanceProfile: InstanceProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstanceProfilesResultTypeDef

```python
# ListInstanceProfilesResultTypeDef definition

class ListInstanceProfilesResultTypeDef(TypedDict):
    instanceProfiles: List[InstanceProfileTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInstanceProfileResultTypeDef

```python
# UpdateInstanceProfileResultTypeDef definition

class UpdateInstanceProfileResultTypeDef(TypedDict):
    instanceProfile: InstanceProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNetworkProfileResultTypeDef

```python
# CreateNetworkProfileResultTypeDef definition

class CreateNetworkProfileResultTypeDef(TypedDict):
    networkProfile: NetworkProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkProfileTypeDef](./type_defs.md#networkprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNetworkProfileResultTypeDef

```python
# GetNetworkProfileResultTypeDef definition

class GetNetworkProfileResultTypeDef(TypedDict):
    networkProfile: NetworkProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkProfileTypeDef](./type_defs.md#networkprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNetworkProfilesResultTypeDef

```python
# ListNetworkProfilesResultTypeDef definition

class ListNetworkProfilesResultTypeDef(TypedDict):
    networkProfiles: List[NetworkProfileTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NetworkProfileTypeDef](./type_defs.md#networkprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNetworkProfileResultTypeDef

```python
# UpdateNetworkProfileResultTypeDef definition

class UpdateNetworkProfileResultTypeDef(TypedDict):
    networkProfile: NetworkProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkProfileTypeDef](./type_defs.md#networkprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectRequestRequestTypeDef

```python
# CreateProjectRequestRequestTypeDef definition

class CreateProjectRequestRequestTypeDef(TypedDict):
    name: str,
    defaultJobTimeoutMinutes: NotRequired[int],
    vpcConfig: NotRequired[VpcConfigTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
## UpdateProjectRequestRequestTypeDef

```python
# UpdateProjectRequestRequestTypeDef definition

class UpdateProjectRequestRequestTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    defaultJobTimeoutMinutes: NotRequired[int],
    vpcConfig: NotRequired[VpcConfigTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
## CreateRemoteAccessSessionRequestRequestTypeDef

```python
# CreateRemoteAccessSessionRequestRequestTypeDef definition

class CreateRemoteAccessSessionRequestRequestTypeDef(TypedDict):
    projectArn: str,
    deviceArn: str,
    instanceArn: NotRequired[str],
    sshPublicKey: NotRequired[str],
    remoteDebugEnabled: NotRequired[bool],
    remoteRecordEnabled: NotRequired[bool],
    remoteRecordAppArn: NotRequired[str],
    name: NotRequired[str],
    clientId: NotRequired[str],
    configuration: NotRequired[CreateRemoteAccessSessionConfigurationTypeDef],  # (1)
    interactionMode: NotRequired[InteractionModeType],  # (2)
    skipAppResign: NotRequired[bool],
```

1. See [:material-code-braces: CreateRemoteAccessSessionConfigurationTypeDef](./type_defs.md#createremoteaccesssessionconfigurationtypedef) 
2. See [:material-code-brackets: InteractionModeType](./literals.md#interactionmodetype) 
## CreateTestGridProjectRequestRequestTypeDef

```python
# CreateTestGridProjectRequestRequestTypeDef definition

class CreateTestGridProjectRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    vpcConfig: NotRequired[TestGridVpcConfigTypeDef],  # (1)
```

1. See [:material-code-braces: TestGridVpcConfigTypeDef](./type_defs.md#testgridvpcconfigtypedef) 
## UpdateTestGridProjectRequestRequestTypeDef

```python
# UpdateTestGridProjectRequestRequestTypeDef definition

class UpdateTestGridProjectRequestRequestTypeDef(TypedDict):
    projectArn: str,
    name: NotRequired[str],
    description: NotRequired[str],
    vpcConfig: NotRequired[TestGridVpcConfigTypeDef],  # (1)
```

1. See [:material-code-braces: TestGridVpcConfigTypeDef](./type_defs.md#testgridvpcconfigtypedef) 
## CreateUploadResultTypeDef

```python
# CreateUploadResultTypeDef definition

class CreateUploadResultTypeDef(TypedDict):
    upload: UploadTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UploadTypeDef](./type_defs.md#uploadtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUploadResultTypeDef

```python
# GetUploadResultTypeDef definition

class GetUploadResultTypeDef(TypedDict):
    upload: UploadTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UploadTypeDef](./type_defs.md#uploadtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstallToRemoteAccessSessionResultTypeDef

```python
# InstallToRemoteAccessSessionResultTypeDef definition

class InstallToRemoteAccessSessionResultTypeDef(TypedDict):
    appUpload: UploadTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UploadTypeDef](./type_defs.md#uploadtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUploadsResultTypeDef

```python
# ListUploadsResultTypeDef definition

class ListUploadsResultTypeDef(TypedDict):
    uploads: List[UploadTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: UploadTypeDef](./type_defs.md#uploadtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUploadResultTypeDef

```python
# UpdateUploadResultTypeDef definition

class UpdateUploadResultTypeDef(TypedDict):
    upload: UploadTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UploadTypeDef](./type_defs.md#uploadtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVPCEConfigurationResultTypeDef

```python
# CreateVPCEConfigurationResultTypeDef definition

class CreateVPCEConfigurationResultTypeDef(TypedDict):
    vpceConfiguration: VPCEConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VPCEConfigurationTypeDef](./type_defs.md#vpceconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVPCEConfigurationResultTypeDef

```python
# GetVPCEConfigurationResultTypeDef definition

class GetVPCEConfigurationResultTypeDef(TypedDict):
    vpceConfiguration: VPCEConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VPCEConfigurationTypeDef](./type_defs.md#vpceconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVPCEConfigurationsResultTypeDef

```python
# ListVPCEConfigurationsResultTypeDef definition

class ListVPCEConfigurationsResultTypeDef(TypedDict):
    vpceConfigurations: List[VPCEConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: VPCEConfigurationTypeDef](./type_defs.md#vpceconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVPCEConfigurationResultTypeDef

```python
# UpdateVPCEConfigurationResultTypeDef definition

class UpdateVPCEConfigurationResultTypeDef(TypedDict):
    vpceConfiguration: VPCEConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VPCEConfigurationTypeDef](./type_defs.md#vpceconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeviceSelectionResultTypeDef

```python
# DeviceSelectionResultTypeDef definition

class DeviceSelectionResultTypeDef(TypedDict):
    filters: NotRequired[List[DeviceFilterOutputTypeDef]],  # (1)
    matchedDevicesCount: NotRequired[int],
    maxDevices: NotRequired[int],
```

1. See [:material-code-braces: DeviceFilterOutputTypeDef](./type_defs.md#devicefilteroutputtypedef) 
## SuiteTypeDef

```python
# SuiteTypeDef definition

class SuiteTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    type: NotRequired[TestTypeType],  # (1)
    created: NotRequired[datetime],
    status: NotRequired[ExecutionStatusType],  # (2)
    result: NotRequired[ExecutionResultType],  # (3)
    started: NotRequired[datetime],
    stopped: NotRequired[datetime],
    counters: NotRequired[CountersTypeDef],  # (4)
    message: NotRequired[str],
    deviceMinutes: NotRequired[DeviceMinutesTypeDef],  # (5)
```

1. See [:material-code-brackets: TestTypeType](./literals.md#testtypetype) 
2. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
3. See [:material-code-brackets: ExecutionResultType](./literals.md#executionresulttype) 
4. See [:material-code-braces: CountersTypeDef](./type_defs.md#counterstypedef) 
5. See [:material-code-braces: DeviceMinutesTypeDef](./type_defs.md#deviceminutestypedef) 
## TestTypeDef

```python
# TestTypeDef definition

class TestTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    type: NotRequired[TestTypeType],  # (1)
    created: NotRequired[datetime],
    status: NotRequired[ExecutionStatusType],  # (2)
    result: NotRequired[ExecutionResultType],  # (3)
    started: NotRequired[datetime],
    stopped: NotRequired[datetime],
    counters: NotRequired[CountersTypeDef],  # (4)
    message: NotRequired[str],
    deviceMinutes: NotRequired[DeviceMinutesTypeDef],  # (5)
```

1. See [:material-code-brackets: TestTypeType](./literals.md#testtypetype) 
2. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
3. See [:material-code-brackets: ExecutionResultType](./literals.md#executionresulttype) 
4. See [:material-code-braces: CountersTypeDef](./type_defs.md#counterstypedef) 
5. See [:material-code-braces: DeviceMinutesTypeDef](./type_defs.md#deviceminutestypedef) 
## GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef

```python
# GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef definition

class GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListArtifactsRequestListArtifactsPaginateTypeDef

```python
# ListArtifactsRequestListArtifactsPaginateTypeDef definition

class ListArtifactsRequestListArtifactsPaginateTypeDef(TypedDict):
    arn: str,
    type: ArtifactCategoryType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ArtifactCategoryType](./literals.md#artifactcategorytype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef

```python
# ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef definition

class ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDevicePoolsRequestListDevicePoolsPaginateTypeDef

```python
# ListDevicePoolsRequestListDevicePoolsPaginateTypeDef definition

class ListDevicePoolsRequestListDevicePoolsPaginateTypeDef(TypedDict):
    arn: str,
    type: NotRequired[DevicePoolTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DevicePoolTypeType](./literals.md#devicepooltypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDevicesRequestListDevicesPaginateTypeDef

```python
# ListDevicesRequestListDevicesPaginateTypeDef definition

class ListDevicesRequestListDevicesPaginateTypeDef(TypedDict):
    arn: NotRequired[str],
    filters: NotRequired[Sequence[DeviceFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DeviceFilterTypeDef](./type_defs.md#devicefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef

```python
# ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef definition

class ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsRequestListJobsPaginateTypeDef

```python
# ListJobsRequestListJobsPaginateTypeDef definition

class ListJobsRequestListJobsPaginateTypeDef(TypedDict):
    arn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef

```python
# ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef definition

class ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef(TypedDict):
    arn: str,
    type: NotRequired[NetworkProfileTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: NetworkProfileTypeType](./literals.md#networkprofiletypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef

```python
# ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef definition

class ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef

```python
# ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef definition

class ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOfferingsRequestListOfferingsPaginateTypeDef

```python
# ListOfferingsRequestListOfferingsPaginateTypeDef definition

class ListOfferingsRequestListOfferingsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsRequestListProjectsPaginateTypeDef

```python
# ListProjectsRequestListProjectsPaginateTypeDef definition

class ListProjectsRequestListProjectsPaginateTypeDef(TypedDict):
    arn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef

```python
# ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef definition

class ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef(TypedDict):
    arn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRunsRequestListRunsPaginateTypeDef

```python
# ListRunsRequestListRunsPaginateTypeDef definition

class ListRunsRequestListRunsPaginateTypeDef(TypedDict):
    arn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSamplesRequestListSamplesPaginateTypeDef

```python
# ListSamplesRequestListSamplesPaginateTypeDef definition

class ListSamplesRequestListSamplesPaginateTypeDef(TypedDict):
    arn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSuitesRequestListSuitesPaginateTypeDef

```python
# ListSuitesRequestListSuitesPaginateTypeDef definition

class ListSuitesRequestListSuitesPaginateTypeDef(TypedDict):
    arn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTestsRequestListTestsPaginateTypeDef

```python
# ListTestsRequestListTestsPaginateTypeDef definition

class ListTestsRequestListTestsPaginateTypeDef(TypedDict):
    arn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef

```python
# ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef definition

class ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef(TypedDict):
    arn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUploadsRequestListUploadsPaginateTypeDef

```python
# ListUploadsRequestListUploadsPaginateTypeDef definition

class ListUploadsRequestListUploadsPaginateTypeDef(TypedDict):
    arn: str,
    type: NotRequired[UploadTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: UploadTypeType](./literals.md#uploadtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef

```python
# ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef definition

class ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTestGridSessionResultTypeDef

```python
# GetTestGridSessionResultTypeDef definition

class GetTestGridSessionResultTypeDef(TypedDict):
    testGridSession: TestGridSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TestGridSessionTypeDef](./type_defs.md#testgridsessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTestGridSessionsResultTypeDef

```python
# ListTestGridSessionsResultTypeDef definition

class ListTestGridSessionsResultTypeDef(TypedDict):
    testGridSessions: List[TestGridSessionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestGridSessionTypeDef](./type_defs.md#testgridsessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOfferingPromotionsResultTypeDef

```python
# ListOfferingPromotionsResultTypeDef definition

class ListOfferingPromotionsResultTypeDef(TypedDict):
    offeringPromotions: List[OfferingPromotionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: OfferingPromotionTypeDef](./type_defs.md#offeringpromotiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSamplesResultTypeDef

```python
# ListSamplesResultTypeDef definition

class ListSamplesResultTypeDef(TypedDict):
    samples: List[SampleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SampleTypeDef](./type_defs.md#sampletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTestGridSessionActionsResultTypeDef

```python
# ListTestGridSessionActionsResultTypeDef definition

class ListTestGridSessionActionsResultTypeDef(TypedDict):
    actions: List[TestGridSessionActionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestGridSessionActionTypeDef](./type_defs.md#testgridsessionactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTestGridSessionArtifactsResultTypeDef

```python
# ListTestGridSessionArtifactsResultTypeDef definition

class ListTestGridSessionArtifactsResultTypeDef(TypedDict):
    artifacts: List[TestGridSessionArtifactTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestGridSessionArtifactTypeDef](./type_defs.md#testgridsessionartifacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTestGridSessionsRequestRequestTypeDef

```python
# ListTestGridSessionsRequestRequestTypeDef definition

class ListTestGridSessionsRequestRequestTypeDef(TypedDict):
    projectArn: str,
    status: NotRequired[TestGridSessionStatusType],  # (1)
    creationTimeAfter: NotRequired[TimestampTypeDef],
    creationTimeBefore: NotRequired[TimestampTypeDef],
    endTimeAfter: NotRequired[TimestampTypeDef],
    endTimeBefore: NotRequired[TimestampTypeDef],
    maxResult: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: TestGridSessionStatusType](./literals.md#testgridsessionstatustype) 
## RecurringChargeTypeDef

```python
# RecurringChargeTypeDef definition

class RecurringChargeTypeDef(TypedDict):
    cost: NotRequired[MonetaryAmountTypeDef],  # (1)
    frequency: NotRequired[RecurringChargeFrequencyType],  # (2)
```

1. See [:material-code-braces: MonetaryAmountTypeDef](./type_defs.md#monetaryamounttypedef) 
2. See [:material-code-brackets: RecurringChargeFrequencyType](./literals.md#recurringchargefrequencytype) 
## ProjectTypeDef

```python
# ProjectTypeDef definition

class ProjectTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    defaultJobTimeoutMinutes: NotRequired[int],
    created: NotRequired[datetime],
    vpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## TestGridProjectTypeDef

```python
# TestGridProjectTypeDef definition

class TestGridProjectTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    vpcConfig: NotRequired[TestGridVpcConfigOutputTypeDef],  # (1)
    created: NotRequired[datetime],
```

1. See [:material-code-braces: TestGridVpcConfigOutputTypeDef](./type_defs.md#testgridvpcconfigoutputtypedef) 
## GetAccountSettingsResultTypeDef

```python
# GetAccountSettingsResultTypeDef definition

class GetAccountSettingsResultTypeDef(TypedDict):
    accountSettings: AccountSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDevicePoolResultTypeDef

```python
# CreateDevicePoolResultTypeDef definition

class CreateDevicePoolResultTypeDef(TypedDict):
    devicePool: DevicePoolTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DevicePoolTypeDef](./type_defs.md#devicepooltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDevicePoolResultTypeDef

```python
# GetDevicePoolResultTypeDef definition

class GetDevicePoolResultTypeDef(TypedDict):
    devicePool: DevicePoolTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DevicePoolTypeDef](./type_defs.md#devicepooltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDevicePoolsResultTypeDef

```python
# ListDevicePoolsResultTypeDef definition

class ListDevicePoolsResultTypeDef(TypedDict):
    devicePools: List[DevicePoolTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DevicePoolTypeDef](./type_defs.md#devicepooltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDevicePoolResultTypeDef

```python
# UpdateDevicePoolResultTypeDef definition

class UpdateDevicePoolResultTypeDef(TypedDict):
    devicePool: DevicePoolTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DevicePoolTypeDef](./type_defs.md#devicepooltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeviceTypeDef

```python
# DeviceTypeDef definition

class DeviceTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    manufacturer: NotRequired[str],
    model: NotRequired[str],
    modelId: NotRequired[str],
    formFactor: NotRequired[DeviceFormFactorType],  # (1)
    platform: NotRequired[DevicePlatformType],  # (2)
    os: NotRequired[str],
    cpu: NotRequired[CPUTypeDef],  # (3)
    resolution: NotRequired[ResolutionTypeDef],  # (4)
    heapSize: NotRequired[int],
    memory: NotRequired[int],
    image: NotRequired[str],
    carrier: NotRequired[str],
    radio: NotRequired[str],
    remoteAccessEnabled: NotRequired[bool],
    remoteDebugEnabled: NotRequired[bool],
    fleetType: NotRequired[str],
    fleetName: NotRequired[str],
    instances: NotRequired[List[DeviceInstanceTypeDef]],  # (5)
    availability: NotRequired[DeviceAvailabilityType],  # (6)
```

1. See [:material-code-brackets: DeviceFormFactorType](./literals.md#deviceformfactortype) 
2. See [:material-code-brackets: DevicePlatformType](./literals.md#deviceplatformtype) 
3. See [:material-code-braces: CPUTypeDef](./type_defs.md#cputypedef) 
4. See [:material-code-braces: ResolutionTypeDef](./type_defs.md#resolutiontypedef) 
5. See [:material-code-braces: DeviceInstanceTypeDef](./type_defs.md#deviceinstancetypedef) 
6. See [:material-code-brackets: DeviceAvailabilityType](./literals.md#deviceavailabilitytype) 
## GetDeviceInstanceResultTypeDef

```python
# GetDeviceInstanceResultTypeDef definition

class GetDeviceInstanceResultTypeDef(TypedDict):
    deviceInstance: DeviceInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceInstanceTypeDef](./type_defs.md#deviceinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeviceInstancesResultTypeDef

```python
# ListDeviceInstancesResultTypeDef definition

class ListDeviceInstancesResultTypeDef(TypedDict):
    deviceInstances: List[DeviceInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeviceInstanceTypeDef](./type_defs.md#deviceinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDeviceInstanceResultTypeDef

```python
# UpdateDeviceInstanceResultTypeDef definition

class UpdateDeviceInstanceResultTypeDef(TypedDict):
    deviceInstance: DeviceInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceInstanceTypeDef](./type_defs.md#deviceinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScheduleRunConfigurationTypeDef

```python
# ScheduleRunConfigurationTypeDef definition

class ScheduleRunConfigurationTypeDef(TypedDict):
    extraDataPackageArn: NotRequired[str],
    networkProfileArn: NotRequired[str],
    locale: NotRequired[str],
    location: NotRequired[LocationTypeDef],  # (1)
    vpceConfigurationArns: NotRequired[Sequence[str]],
    customerArtifactPaths: NotRequired[CustomerArtifactPathsUnionTypeDef],  # (2)
    radios: NotRequired[RadiosTypeDef],  # (3)
    auxiliaryApps: NotRequired[Sequence[str]],
    billingMethod: NotRequired[BillingMethodType],  # (4)
```

1. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
2. See [:material-code-braces: CustomerArtifactPathsTypeDef](./type_defs.md#customerartifactpathstypedef) [:material-code-braces: CustomerArtifactPathsOutputTypeDef](./type_defs.md#customerartifactpathsoutputtypedef) 
3. See [:material-code-braces: RadiosTypeDef](./type_defs.md#radiostypedef) 
4. See [:material-code-brackets: BillingMethodType](./literals.md#billingmethodtype) 
## RunTypeDef

```python
# RunTypeDef definition

class RunTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    type: NotRequired[TestTypeType],  # (1)
    platform: NotRequired[DevicePlatformType],  # (2)
    created: NotRequired[datetime],
    status: NotRequired[ExecutionStatusType],  # (3)
    result: NotRequired[ExecutionResultType],  # (4)
    started: NotRequired[datetime],
    stopped: NotRequired[datetime],
    counters: NotRequired[CountersTypeDef],  # (5)
    message: NotRequired[str],
    totalJobs: NotRequired[int],
    completedJobs: NotRequired[int],
    billingMethod: NotRequired[BillingMethodType],  # (6)
    deviceMinutes: NotRequired[DeviceMinutesTypeDef],  # (7)
    networkProfile: NotRequired[NetworkProfileTypeDef],  # (8)
    parsingResultUrl: NotRequired[str],
    resultCode: NotRequired[ExecutionResultCodeType],  # (9)
    seed: NotRequired[int],
    appUpload: NotRequired[str],
    eventCount: NotRequired[int],
    jobTimeoutMinutes: NotRequired[int],
    devicePoolArn: NotRequired[str],
    locale: NotRequired[str],
    radios: NotRequired[RadiosTypeDef],  # (10)
    location: NotRequired[LocationTypeDef],  # (11)
    customerArtifactPaths: NotRequired[CustomerArtifactPathsOutputTypeDef],  # (12)
    webUrl: NotRequired[str],
    skipAppResign: NotRequired[bool],
    testSpecArn: NotRequired[str],
    deviceSelectionResult: NotRequired[DeviceSelectionResultTypeDef],  # (13)
    vpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (14)
```

1. See [:material-code-brackets: TestTypeType](./literals.md#testtypetype) 
2. See [:material-code-brackets: DevicePlatformType](./literals.md#deviceplatformtype) 
3. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
4. See [:material-code-brackets: ExecutionResultType](./literals.md#executionresulttype) 
5. See [:material-code-braces: CountersTypeDef](./type_defs.md#counterstypedef) 
6. See [:material-code-brackets: BillingMethodType](./literals.md#billingmethodtype) 
7. See [:material-code-braces: DeviceMinutesTypeDef](./type_defs.md#deviceminutestypedef) 
8. See [:material-code-braces: NetworkProfileTypeDef](./type_defs.md#networkprofiletypedef) 
9. See [:material-code-brackets: ExecutionResultCodeType](./literals.md#executionresultcodetype) 
10. See [:material-code-braces: RadiosTypeDef](./type_defs.md#radiostypedef) 
11. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
12. See [:material-code-braces: CustomerArtifactPathsOutputTypeDef](./type_defs.md#customerartifactpathsoutputtypedef) 
13. See [:material-code-braces: DeviceSelectionResultTypeDef](./type_defs.md#deviceselectionresulttypedef) 
14. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## DeviceSelectionConfigurationTypeDef

```python
# DeviceSelectionConfigurationTypeDef definition

class DeviceSelectionConfigurationTypeDef(TypedDict):
    filters: Sequence[DeviceFilterUnionTypeDef],  # (1)
    maxDevices: int,
```

1. See [:material-code-braces: DeviceFilterTypeDef](./type_defs.md#devicefiltertypedef) [:material-code-braces: DeviceFilterOutputTypeDef](./type_defs.md#devicefilteroutputtypedef) 
## ListDevicesRequestRequestTypeDef

```python
# ListDevicesRequestRequestTypeDef definition

class ListDevicesRequestRequestTypeDef(TypedDict):
    arn: NotRequired[str],
    nextToken: NotRequired[str],
    filters: NotRequired[Sequence[DeviceFilterUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: DeviceFilterTypeDef](./type_defs.md#devicefiltertypedef) [:material-code-braces: DeviceFilterOutputTypeDef](./type_defs.md#devicefilteroutputtypedef) 
## GetSuiteResultTypeDef

```python
# GetSuiteResultTypeDef definition

class GetSuiteResultTypeDef(TypedDict):
    suite: SuiteTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SuiteTypeDef](./type_defs.md#suitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSuitesResultTypeDef

```python
# ListSuitesResultTypeDef definition

class ListSuitesResultTypeDef(TypedDict):
    suites: List[SuiteTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SuiteTypeDef](./type_defs.md#suitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTestResultTypeDef

```python
# GetTestResultTypeDef definition

class GetTestResultTypeDef(TypedDict):
    test: TestTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TestTypeDef](./type_defs.md#testtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTestsResultTypeDef

```python
# ListTestsResultTypeDef definition

class ListTestsResultTypeDef(TypedDict):
    tests: List[TestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestTypeDef](./type_defs.md#testtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OfferingTypeDef

```python
# OfferingTypeDef definition

class OfferingTypeDef(TypedDict):
    id: NotRequired[str],
    description: NotRequired[str],
    type: NotRequired[OfferingTypeType],  # (1)
    platform: NotRequired[DevicePlatformType],  # (2)
    recurringCharges: NotRequired[List[RecurringChargeTypeDef]],  # (3)
```

1. See [:material-code-brackets: OfferingTypeType](./literals.md#offeringtypetype) 
2. See [:material-code-brackets: DevicePlatformType](./literals.md#deviceplatformtype) 
3. See [:material-code-braces: RecurringChargeTypeDef](./type_defs.md#recurringchargetypedef) 
## CreateProjectResultTypeDef

```python
# CreateProjectResultTypeDef definition

class CreateProjectResultTypeDef(TypedDict):
    project: ProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProjectResultTypeDef

```python
# GetProjectResultTypeDef definition

class GetProjectResultTypeDef(TypedDict):
    project: ProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProjectsResultTypeDef

```python
# ListProjectsResultTypeDef definition

class ListProjectsResultTypeDef(TypedDict):
    projects: List[ProjectTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectResultTypeDef

```python
# UpdateProjectResultTypeDef definition

class UpdateProjectResultTypeDef(TypedDict):
    project: ProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTestGridProjectResultTypeDef

```python
# CreateTestGridProjectResultTypeDef definition

class CreateTestGridProjectResultTypeDef(TypedDict):
    testGridProject: TestGridProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TestGridProjectTypeDef](./type_defs.md#testgridprojecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTestGridProjectResultTypeDef

```python
# GetTestGridProjectResultTypeDef definition

class GetTestGridProjectResultTypeDef(TypedDict):
    testGridProject: TestGridProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TestGridProjectTypeDef](./type_defs.md#testgridprojecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTestGridProjectsResultTypeDef

```python
# ListTestGridProjectsResultTypeDef definition

class ListTestGridProjectsResultTypeDef(TypedDict):
    testGridProjects: List[TestGridProjectTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestGridProjectTypeDef](./type_defs.md#testgridprojecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTestGridProjectResultTypeDef

```python
# UpdateTestGridProjectResultTypeDef definition

class UpdateTestGridProjectResultTypeDef(TypedDict):
    testGridProject: TestGridProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TestGridProjectTypeDef](./type_defs.md#testgridprojecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DevicePoolCompatibilityResultTypeDef

```python
# DevicePoolCompatibilityResultTypeDef definition

class DevicePoolCompatibilityResultTypeDef(TypedDict):
    device: NotRequired[DeviceTypeDef],  # (1)
    compatible: NotRequired[bool],
    incompatibilityMessages: NotRequired[List[IncompatibilityMessageTypeDef]],  # (2)
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
2. See [:material-code-braces: IncompatibilityMessageTypeDef](./type_defs.md#incompatibilitymessagetypedef) 
## GetDeviceResultTypeDef

```python
# GetDeviceResultTypeDef definition

class GetDeviceResultTypeDef(TypedDict):
    device: DeviceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobTypeDef

```python
# JobTypeDef definition

class JobTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    type: NotRequired[TestTypeType],  # (1)
    created: NotRequired[datetime],
    status: NotRequired[ExecutionStatusType],  # (2)
    result: NotRequired[ExecutionResultType],  # (3)
    started: NotRequired[datetime],
    stopped: NotRequired[datetime],
    counters: NotRequired[CountersTypeDef],  # (4)
    message: NotRequired[str],
    device: NotRequired[DeviceTypeDef],  # (5)
    instanceArn: NotRequired[str],
    deviceMinutes: NotRequired[DeviceMinutesTypeDef],  # (6)
    videoEndpoint: NotRequired[str],
    videoCapture: NotRequired[bool],
```

1. See [:material-code-brackets: TestTypeType](./literals.md#testtypetype) 
2. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
3. See [:material-code-brackets: ExecutionResultType](./literals.md#executionresulttype) 
4. See [:material-code-braces: CountersTypeDef](./type_defs.md#counterstypedef) 
5. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
6. See [:material-code-braces: DeviceMinutesTypeDef](./type_defs.md#deviceminutestypedef) 
## ListDevicesResultTypeDef

```python
# ListDevicesResultTypeDef definition

class ListDevicesResultTypeDef(TypedDict):
    devices: List[DeviceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProblemTypeDef

```python
# ProblemTypeDef definition

class ProblemTypeDef(TypedDict):
    run: NotRequired[ProblemDetailTypeDef],  # (1)
    job: NotRequired[ProblemDetailTypeDef],  # (1)
    suite: NotRequired[ProblemDetailTypeDef],  # (1)
    test: NotRequired[ProblemDetailTypeDef],  # (1)
    device: NotRequired[DeviceTypeDef],  # (5)
    result: NotRequired[ExecutionResultType],  # (6)
    message: NotRequired[str],
```

1. See [:material-code-braces: ProblemDetailTypeDef](./type_defs.md#problemdetailtypedef) 
2. See [:material-code-braces: ProblemDetailTypeDef](./type_defs.md#problemdetailtypedef) 
3. See [:material-code-braces: ProblemDetailTypeDef](./type_defs.md#problemdetailtypedef) 
4. See [:material-code-braces: ProblemDetailTypeDef](./type_defs.md#problemdetailtypedef) 
5. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
6. See [:material-code-brackets: ExecutionResultType](./literals.md#executionresulttype) 
## RemoteAccessSessionTypeDef

```python
# RemoteAccessSessionTypeDef definition

class RemoteAccessSessionTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    created: NotRequired[datetime],
    status: NotRequired[ExecutionStatusType],  # (1)
    result: NotRequired[ExecutionResultType],  # (2)
    message: NotRequired[str],
    started: NotRequired[datetime],
    stopped: NotRequired[datetime],
    device: NotRequired[DeviceTypeDef],  # (3)
    instanceArn: NotRequired[str],
    remoteDebugEnabled: NotRequired[bool],
    remoteRecordEnabled: NotRequired[bool],
    remoteRecordAppArn: NotRequired[str],
    hostAddress: NotRequired[str],
    clientId: NotRequired[str],
    billingMethod: NotRequired[BillingMethodType],  # (4)
    deviceMinutes: NotRequired[DeviceMinutesTypeDef],  # (5)
    endpoint: NotRequired[str],
    deviceUdid: NotRequired[str],
    interactionMode: NotRequired[InteractionModeType],  # (6)
    skipAppResign: NotRequired[bool],
    vpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (7)
```

1. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
2. See [:material-code-brackets: ExecutionResultType](./literals.md#executionresulttype) 
3. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
4. See [:material-code-brackets: BillingMethodType](./literals.md#billingmethodtype) 
5. See [:material-code-braces: DeviceMinutesTypeDef](./type_defs.md#deviceminutestypedef) 
6. See [:material-code-brackets: InteractionModeType](./literals.md#interactionmodetype) 
7. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## GetDevicePoolCompatibilityRequestRequestTypeDef

```python
# GetDevicePoolCompatibilityRequestRequestTypeDef definition

class GetDevicePoolCompatibilityRequestRequestTypeDef(TypedDict):
    devicePoolArn: str,
    appArn: NotRequired[str],
    testType: NotRequired[TestTypeType],  # (1)
    test: NotRequired[ScheduleRunTestTypeDef],  # (2)
    configuration: NotRequired[ScheduleRunConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: TestTypeType](./literals.md#testtypetype) 
2. See [:material-code-braces: ScheduleRunTestTypeDef](./type_defs.md#scheduleruntesttypedef) 
3. See [:material-code-braces: ScheduleRunConfigurationTypeDef](./type_defs.md#schedulerunconfigurationtypedef) 
## GetRunResultTypeDef

```python
# GetRunResultTypeDef definition

class GetRunResultTypeDef(TypedDict):
    run: RunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RunTypeDef](./type_defs.md#runtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRunsResultTypeDef

```python
# ListRunsResultTypeDef definition

class ListRunsResultTypeDef(TypedDict):
    runs: List[RunTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RunTypeDef](./type_defs.md#runtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScheduleRunResultTypeDef

```python
# ScheduleRunResultTypeDef definition

class ScheduleRunResultTypeDef(TypedDict):
    run: RunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RunTypeDef](./type_defs.md#runtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopRunResultTypeDef

```python
# StopRunResultTypeDef definition

class StopRunResultTypeDef(TypedDict):
    run: RunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RunTypeDef](./type_defs.md#runtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScheduleRunRequestRequestTypeDef

```python
# ScheduleRunRequestRequestTypeDef definition

class ScheduleRunRequestRequestTypeDef(TypedDict):
    projectArn: str,
    test: ScheduleRunTestTypeDef,  # (1)
    appArn: NotRequired[str],
    devicePoolArn: NotRequired[str],
    deviceSelectionConfiguration: NotRequired[DeviceSelectionConfigurationTypeDef],  # (2)
    name: NotRequired[str],
    configuration: NotRequired[ScheduleRunConfigurationTypeDef],  # (3)
    executionConfiguration: NotRequired[ExecutionConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: ScheduleRunTestTypeDef](./type_defs.md#scheduleruntesttypedef) 
2. See [:material-code-braces: DeviceSelectionConfigurationTypeDef](./type_defs.md#deviceselectionconfigurationtypedef) 
3. See [:material-code-braces: ScheduleRunConfigurationTypeDef](./type_defs.md#schedulerunconfigurationtypedef) 
4. See [:material-code-braces: ExecutionConfigurationTypeDef](./type_defs.md#executionconfigurationtypedef) 
## ListOfferingsResultTypeDef

```python
# ListOfferingsResultTypeDef definition

class ListOfferingsResultTypeDef(TypedDict):
    offerings: List[OfferingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: OfferingTypeDef](./type_defs.md#offeringtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OfferingStatusTypeDef

```python
# OfferingStatusTypeDef definition

class OfferingStatusTypeDef(TypedDict):
    type: NotRequired[OfferingTransactionTypeType],  # (1)
    offering: NotRequired[OfferingTypeDef],  # (2)
    quantity: NotRequired[int],
    effectiveOn: NotRequired[datetime],
```

1. See [:material-code-brackets: OfferingTransactionTypeType](./literals.md#offeringtransactiontypetype) 
2. See [:material-code-braces: OfferingTypeDef](./type_defs.md#offeringtypedef) 
## GetDevicePoolCompatibilityResultTypeDef

```python
# GetDevicePoolCompatibilityResultTypeDef definition

class GetDevicePoolCompatibilityResultTypeDef(TypedDict):
    compatibleDevices: List[DevicePoolCompatibilityResultTypeDef],  # (1)
    incompatibleDevices: List[DevicePoolCompatibilityResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DevicePoolCompatibilityResultTypeDef](./type_defs.md#devicepoolcompatibilityresulttypedef) 
2. See [:material-code-braces: DevicePoolCompatibilityResultTypeDef](./type_defs.md#devicepoolcompatibilityresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobResultTypeDef

```python
# GetJobResultTypeDef definition

class GetJobResultTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobsResultTypeDef

```python
# ListJobsResultTypeDef definition

class ListJobsResultTypeDef(TypedDict):
    jobs: List[JobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopJobResultTypeDef

```python
# StopJobResultTypeDef definition

class StopJobResultTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UniqueProblemTypeDef

```python
# UniqueProblemTypeDef definition

class UniqueProblemTypeDef(TypedDict):
    message: NotRequired[str],
    problems: NotRequired[List[ProblemTypeDef]],  # (1)
```

1. See [:material-code-braces: ProblemTypeDef](./type_defs.md#problemtypedef) 
## CreateRemoteAccessSessionResultTypeDef

```python
# CreateRemoteAccessSessionResultTypeDef definition

class CreateRemoteAccessSessionResultTypeDef(TypedDict):
    remoteAccessSession: RemoteAccessSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RemoteAccessSessionTypeDef](./type_defs.md#remoteaccesssessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRemoteAccessSessionResultTypeDef

```python
# GetRemoteAccessSessionResultTypeDef definition

class GetRemoteAccessSessionResultTypeDef(TypedDict):
    remoteAccessSession: RemoteAccessSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RemoteAccessSessionTypeDef](./type_defs.md#remoteaccesssessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRemoteAccessSessionsResultTypeDef

```python
# ListRemoteAccessSessionsResultTypeDef definition

class ListRemoteAccessSessionsResultTypeDef(TypedDict):
    remoteAccessSessions: List[RemoteAccessSessionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RemoteAccessSessionTypeDef](./type_defs.md#remoteaccesssessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopRemoteAccessSessionResultTypeDef

```python
# StopRemoteAccessSessionResultTypeDef definition

class StopRemoteAccessSessionResultTypeDef(TypedDict):
    remoteAccessSession: RemoteAccessSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RemoteAccessSessionTypeDef](./type_defs.md#remoteaccesssessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOfferingStatusResultTypeDef

```python
# GetOfferingStatusResultTypeDef definition

class GetOfferingStatusResultTypeDef(TypedDict):
    current: Dict[str, OfferingStatusTypeDef],  # (1)
    nextPeriod: Dict[str, OfferingStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: OfferingStatusTypeDef](./type_defs.md#offeringstatustypedef) 
2. See [:material-code-braces: OfferingStatusTypeDef](./type_defs.md#offeringstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OfferingTransactionTypeDef

```python
# OfferingTransactionTypeDef definition

class OfferingTransactionTypeDef(TypedDict):
    offeringStatus: NotRequired[OfferingStatusTypeDef],  # (1)
    transactionId: NotRequired[str],
    offeringPromotionId: NotRequired[str],
    createdOn: NotRequired[datetime],
    cost: NotRequired[MonetaryAmountTypeDef],  # (2)
```

1. See [:material-code-braces: OfferingStatusTypeDef](./type_defs.md#offeringstatustypedef) 
2. See [:material-code-braces: MonetaryAmountTypeDef](./type_defs.md#monetaryamounttypedef) 
## ListUniqueProblemsResultTypeDef

```python
# ListUniqueProblemsResultTypeDef definition

class ListUniqueProblemsResultTypeDef(TypedDict):
    uniqueProblems: Dict[ExecutionResultType, List[UniqueProblemTypeDef]],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: ExecutionResultType](./literals.md#executionresulttype) [:material-code-braces: UniqueProblemTypeDef](./type_defs.md#uniqueproblemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOfferingTransactionsResultTypeDef

```python
# ListOfferingTransactionsResultTypeDef definition

class ListOfferingTransactionsResultTypeDef(TypedDict):
    offeringTransactions: List[OfferingTransactionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: OfferingTransactionTypeDef](./type_defs.md#offeringtransactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PurchaseOfferingResultTypeDef

```python
# PurchaseOfferingResultTypeDef definition

class PurchaseOfferingResultTypeDef(TypedDict):
    offeringTransaction: OfferingTransactionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OfferingTransactionTypeDef](./type_defs.md#offeringtransactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RenewOfferingResultTypeDef

```python
# RenewOfferingResultTypeDef definition

class RenewOfferingResultTypeDef(TypedDict):
    offeringTransaction: OfferingTransactionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OfferingTransactionTypeDef](./type_defs.md#offeringtransactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
