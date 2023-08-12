# Type definitions

> [Index](../README.md) > [NimbleStudio](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [NimbleStudio](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
    type annotations stubs module [types-aiobotocore-nimble](https://pypi.org/project/types-aiobotocore-nimble/).



## AcceptEulasRequestRequestTypeDef

```python
# AcceptEulasRequestRequestTypeDef definition

class AcceptEulasRequestRequestTypeDef(TypedDict):
    studioId: str,
    clientToken: NotRequired[str],
    eulaIds: NotRequired[Sequence[str]],
```

## EulaAcceptanceTypeDef

```python
# EulaAcceptanceTypeDef definition

class EulaAcceptanceTypeDef(TypedDict):
    acceptedAt: NotRequired[datetime],
    acceptedBy: NotRequired[str],
    accepteeId: NotRequired[str],
    eulaAcceptanceId: NotRequired[str],
    eulaId: NotRequired[str],
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

## ActiveDirectoryComputerAttributeTypeDef

```python
# ActiveDirectoryComputerAttributeTypeDef definition

class ActiveDirectoryComputerAttributeTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[str],
```

## ComputeFarmConfigurationTypeDef

```python
# ComputeFarmConfigurationTypeDef definition

class ComputeFarmConfigurationTypeDef(TypedDict):
    activeDirectoryUser: NotRequired[str],
    endpoint: NotRequired[str],
```

## CreateStreamingImageRequestRequestTypeDef

```python
# CreateStreamingImageRequestRequestTypeDef definition

class CreateStreamingImageRequestRequestTypeDef(TypedDict):
    ec2ImageId: str,
    name: str,
    studioId: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CreateStreamingSessionRequestRequestTypeDef

```python
# CreateStreamingSessionRequestRequestTypeDef definition

class CreateStreamingSessionRequestRequestTypeDef(TypedDict):
    launchProfileId: str,
    studioId: str,
    clientToken: NotRequired[str],
    ec2InstanceType: NotRequired[StreamingInstanceTypeType],  # (1)
    ownedBy: NotRequired[str],
    streamingImageId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: StreamingInstanceTypeType](./literals.md#streaminginstancetypetype) 
## CreateStreamingSessionStreamRequestRequestTypeDef

```python
# CreateStreamingSessionStreamRequestRequestTypeDef definition

class CreateStreamingSessionStreamRequestRequestTypeDef(TypedDict):
    sessionId: str,
    studioId: str,
    clientToken: NotRequired[str],
    expirationInSeconds: NotRequired[int],
```

## StreamingSessionStreamTypeDef

```python
# StreamingSessionStreamTypeDef definition

class StreamingSessionStreamTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    expiresAt: NotRequired[datetime],
    ownedBy: NotRequired[str],
    state: NotRequired[StreamingSessionStreamStateType],  # (1)
    statusCode: NotRequired[StreamingSessionStreamStatusCodeType],  # (2)
    streamId: NotRequired[str],
    url: NotRequired[str],
```

1. See [:material-code-brackets: StreamingSessionStreamStateType](./literals.md#streamingsessionstreamstatetype) 
2. See [:material-code-brackets: StreamingSessionStreamStatusCodeType](./literals.md#streamingsessionstreamstatuscodetype) 
## ScriptParameterKeyValueTypeDef

```python
# ScriptParameterKeyValueTypeDef definition

class ScriptParameterKeyValueTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## StudioComponentInitializationScriptTypeDef

```python
# StudioComponentInitializationScriptTypeDef definition

class StudioComponentInitializationScriptTypeDef(TypedDict):
    launchProfileProtocolVersion: NotRequired[str],
    platform: NotRequired[LaunchProfilePlatformType],  # (1)
    runContext: NotRequired[StudioComponentInitializationScriptRunContextType],  # (2)
    script: NotRequired[str],
```

1. See [:material-code-brackets: LaunchProfilePlatformType](./literals.md#launchprofileplatformtype) 
2. See [:material-code-brackets: StudioComponentInitializationScriptRunContextType](./literals.md#studiocomponentinitializationscriptruncontexttype) 
## StudioEncryptionConfigurationTypeDef

```python
# StudioEncryptionConfigurationTypeDef definition

class StudioEncryptionConfigurationTypeDef(TypedDict):
    keyType: StudioEncryptionConfigurationKeyTypeType,  # (1)
    keyArn: NotRequired[str],
```

1. See [:material-code-brackets: StudioEncryptionConfigurationKeyTypeType](./literals.md#studioencryptionconfigurationkeytypetype) 
## DeleteLaunchProfileMemberRequestRequestTypeDef

```python
# DeleteLaunchProfileMemberRequestRequestTypeDef definition

class DeleteLaunchProfileMemberRequestRequestTypeDef(TypedDict):
    launchProfileId: str,
    principalId: str,
    studioId: str,
    clientToken: NotRequired[str],
```

## DeleteLaunchProfileRequestRequestTypeDef

```python
# DeleteLaunchProfileRequestRequestTypeDef definition

class DeleteLaunchProfileRequestRequestTypeDef(TypedDict):
    launchProfileId: str,
    studioId: str,
    clientToken: NotRequired[str],
```

## DeleteStreamingImageRequestRequestTypeDef

```python
# DeleteStreamingImageRequestRequestTypeDef definition

class DeleteStreamingImageRequestRequestTypeDef(TypedDict):
    streamingImageId: str,
    studioId: str,
    clientToken: NotRequired[str],
```

## DeleteStreamingSessionRequestRequestTypeDef

```python
# DeleteStreamingSessionRequestRequestTypeDef definition

class DeleteStreamingSessionRequestRequestTypeDef(TypedDict):
    sessionId: str,
    studioId: str,
    clientToken: NotRequired[str],
```

## DeleteStudioComponentRequestRequestTypeDef

```python
# DeleteStudioComponentRequestRequestTypeDef definition

class DeleteStudioComponentRequestRequestTypeDef(TypedDict):
    studioComponentId: str,
    studioId: str,
    clientToken: NotRequired[str],
```

## DeleteStudioMemberRequestRequestTypeDef

```python
# DeleteStudioMemberRequestRequestTypeDef definition

class DeleteStudioMemberRequestRequestTypeDef(TypedDict):
    principalId: str,
    studioId: str,
    clientToken: NotRequired[str],
```

## DeleteStudioRequestRequestTypeDef

```python
# DeleteStudioRequestRequestTypeDef definition

class DeleteStudioRequestRequestTypeDef(TypedDict):
    studioId: str,
    clientToken: NotRequired[str],
```

## EulaTypeDef

```python
# EulaTypeDef definition

class EulaTypeDef(TypedDict):
    content: NotRequired[str],
    createdAt: NotRequired[datetime],
    eulaId: NotRequired[str],
    name: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

## GetEulaRequestRequestTypeDef

```python
# GetEulaRequestRequestTypeDef definition

class GetEulaRequestRequestTypeDef(TypedDict):
    eulaId: str,
```

## GetLaunchProfileDetailsRequestRequestTypeDef

```python
# GetLaunchProfileDetailsRequestRequestTypeDef definition

class GetLaunchProfileDetailsRequestRequestTypeDef(TypedDict):
    launchProfileId: str,
    studioId: str,
```

## StudioComponentSummaryTypeDef

```python
# StudioComponentSummaryTypeDef definition

class StudioComponentSummaryTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    description: NotRequired[str],
    name: NotRequired[str],
    studioComponentId: NotRequired[str],
    subtype: NotRequired[StudioComponentSubtypeType],  # (1)
    type: NotRequired[StudioComponentTypeType],  # (2)
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

1. See [:material-code-brackets: StudioComponentSubtypeType](./literals.md#studiocomponentsubtypetype) 
2. See [:material-code-brackets: StudioComponentTypeType](./literals.md#studiocomponenttypetype) 
## GetLaunchProfileInitializationRequestRequestTypeDef

```python
# GetLaunchProfileInitializationRequestRequestTypeDef definition

class GetLaunchProfileInitializationRequestRequestTypeDef(TypedDict):
    launchProfileId: str,
    launchProfileProtocolVersions: Sequence[str],
    launchPurpose: str,
    platform: str,
    studioId: str,
```

## GetLaunchProfileMemberRequestRequestTypeDef

```python
# GetLaunchProfileMemberRequestRequestTypeDef definition

class GetLaunchProfileMemberRequestRequestTypeDef(TypedDict):
    launchProfileId: str,
    principalId: str,
    studioId: str,
```

## LaunchProfileMembershipTypeDef

```python
# LaunchProfileMembershipTypeDef definition

class LaunchProfileMembershipTypeDef(TypedDict):
    identityStoreId: NotRequired[str],
    persona: NotRequired[LaunchProfilePersonaType],  # (1)
    principalId: NotRequired[str],
    sid: NotRequired[str],
```

1. See [:material-code-brackets: LaunchProfilePersonaType](./literals.md#launchprofilepersonatype) 
## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## GetLaunchProfileRequestRequestTypeDef

```python
# GetLaunchProfileRequestRequestTypeDef definition

class GetLaunchProfileRequestRequestTypeDef(TypedDict):
    launchProfileId: str,
    studioId: str,
```

## GetStreamingImageRequestRequestTypeDef

```python
# GetStreamingImageRequestRequestTypeDef definition

class GetStreamingImageRequestRequestTypeDef(TypedDict):
    streamingImageId: str,
    studioId: str,
```

## GetStreamingSessionBackupRequestRequestTypeDef

```python
# GetStreamingSessionBackupRequestRequestTypeDef definition

class GetStreamingSessionBackupRequestRequestTypeDef(TypedDict):
    backupId: str,
    studioId: str,
```

## StreamingSessionBackupTypeDef

```python
# StreamingSessionBackupTypeDef definition

class StreamingSessionBackupTypeDef(TypedDict):
    arn: NotRequired[str],
    backupId: NotRequired[str],
    createdAt: NotRequired[datetime],
    launchProfileId: NotRequired[str],
    ownedBy: NotRequired[str],
    sessionId: NotRequired[str],
    state: NotRequired[StreamingSessionStateType],  # (1)
    statusCode: NotRequired[StreamingSessionStatusCodeType],  # (2)
    statusMessage: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: StreamingSessionStateType](./literals.md#streamingsessionstatetype) 
2. See [:material-code-brackets: StreamingSessionStatusCodeType](./literals.md#streamingsessionstatuscodetype) 
## GetStreamingSessionRequestRequestTypeDef

```python
# GetStreamingSessionRequestRequestTypeDef definition

class GetStreamingSessionRequestRequestTypeDef(TypedDict):
    sessionId: str,
    studioId: str,
```

## GetStreamingSessionStreamRequestRequestTypeDef

```python
# GetStreamingSessionStreamRequestRequestTypeDef definition

class GetStreamingSessionStreamRequestRequestTypeDef(TypedDict):
    sessionId: str,
    streamId: str,
    studioId: str,
```

## GetStudioComponentRequestRequestTypeDef

```python
# GetStudioComponentRequestRequestTypeDef definition

class GetStudioComponentRequestRequestTypeDef(TypedDict):
    studioComponentId: str,
    studioId: str,
```

## GetStudioMemberRequestRequestTypeDef

```python
# GetStudioMemberRequestRequestTypeDef definition

class GetStudioMemberRequestRequestTypeDef(TypedDict):
    principalId: str,
    studioId: str,
```

## StudioMembershipTypeDef

```python
# StudioMembershipTypeDef definition

class StudioMembershipTypeDef(TypedDict):
    identityStoreId: NotRequired[str],
    persona: NotRequired[StudioPersonaType],  # (1)
    principalId: NotRequired[str],
    sid: NotRequired[str],
```

1. See [:material-code-brackets: StudioPersonaType](./literals.md#studiopersonatype) 
## GetStudioRequestRequestTypeDef

```python
# GetStudioRequestRequestTypeDef definition

class GetStudioRequestRequestTypeDef(TypedDict):
    studioId: str,
```

## LaunchProfileInitializationScriptTypeDef

```python
# LaunchProfileInitializationScriptTypeDef definition

class LaunchProfileInitializationScriptTypeDef(TypedDict):
    runtimeRoleArn: NotRequired[str],
    script: NotRequired[str],
    secureInitializationRoleArn: NotRequired[str],
    studioComponentId: NotRequired[str],
    studioComponentName: NotRequired[str],
```

## ValidationResultTypeDef

```python
# ValidationResultTypeDef definition

class ValidationResultTypeDef(TypedDict):
    state: LaunchProfileValidationStateType,  # (1)
    statusCode: LaunchProfileValidationStatusCodeType,  # (2)
    statusMessage: str,
    type: LaunchProfileValidationTypeType,  # (3)
```

1. See [:material-code-brackets: LaunchProfileValidationStateType](./literals.md#launchprofilevalidationstatetype) 
2. See [:material-code-brackets: LaunchProfileValidationStatusCodeType](./literals.md#launchprofilevalidationstatuscodetype) 
3. See [:material-code-brackets: LaunchProfileValidationTypeType](./literals.md#launchprofilevalidationtypetype) 
## LicenseServiceConfigurationTypeDef

```python
# LicenseServiceConfigurationTypeDef definition

class LicenseServiceConfigurationTypeDef(TypedDict):
    endpoint: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListEulaAcceptancesRequestRequestTypeDef

```python
# ListEulaAcceptancesRequestRequestTypeDef definition

class ListEulaAcceptancesRequestRequestTypeDef(TypedDict):
    studioId: str,
    eulaIds: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
```

## ListEulasRequestRequestTypeDef

```python
# ListEulasRequestRequestTypeDef definition

class ListEulasRequestRequestTypeDef(TypedDict):
    eulaIds: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
```

## ListLaunchProfileMembersRequestRequestTypeDef

```python
# ListLaunchProfileMembersRequestRequestTypeDef definition

class ListLaunchProfileMembersRequestRequestTypeDef(TypedDict):
    launchProfileId: str,
    studioId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListLaunchProfilesRequestRequestTypeDef

```python
# ListLaunchProfilesRequestRequestTypeDef definition

class ListLaunchProfilesRequestRequestTypeDef(TypedDict):
    studioId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    principalId: NotRequired[str],
    states: NotRequired[Sequence[LaunchProfileStateType]],  # (1)
```

1. See [:material-code-brackets: LaunchProfileStateType](./literals.md#launchprofilestatetype) 
## ListStreamingImagesRequestRequestTypeDef

```python
# ListStreamingImagesRequestRequestTypeDef definition

class ListStreamingImagesRequestRequestTypeDef(TypedDict):
    studioId: str,
    nextToken: NotRequired[str],
    owner: NotRequired[str],
```

## ListStreamingSessionBackupsRequestRequestTypeDef

```python
# ListStreamingSessionBackupsRequestRequestTypeDef definition

class ListStreamingSessionBackupsRequestRequestTypeDef(TypedDict):
    studioId: str,
    nextToken: NotRequired[str],
    ownedBy: NotRequired[str],
```

## ListStreamingSessionsRequestRequestTypeDef

```python
# ListStreamingSessionsRequestRequestTypeDef definition

class ListStreamingSessionsRequestRequestTypeDef(TypedDict):
    studioId: str,
    createdBy: NotRequired[str],
    nextToken: NotRequired[str],
    ownedBy: NotRequired[str],
    sessionIds: NotRequired[str],
```

## ListStudioComponentsRequestRequestTypeDef

```python
# ListStudioComponentsRequestRequestTypeDef definition

class ListStudioComponentsRequestRequestTypeDef(TypedDict):
    studioId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    states: NotRequired[Sequence[StudioComponentStateType]],  # (1)
    types: NotRequired[Sequence[StudioComponentTypeType]],  # (2)
```

1. See [:material-code-brackets: StudioComponentStateType](./literals.md#studiocomponentstatetype) 
2. See [:material-code-brackets: StudioComponentTypeType](./literals.md#studiocomponenttypetype) 
## ListStudioMembersRequestRequestTypeDef

```python
# ListStudioMembersRequestRequestTypeDef definition

class ListStudioMembersRequestRequestTypeDef(TypedDict):
    studioId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListStudiosRequestRequestTypeDef

```python
# ListStudiosRequestRequestTypeDef definition

class ListStudiosRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## NewLaunchProfileMemberTypeDef

```python
# NewLaunchProfileMemberTypeDef definition

class NewLaunchProfileMemberTypeDef(TypedDict):
    persona: LaunchProfilePersonaType,  # (1)
    principalId: str,
```

1. See [:material-code-brackets: LaunchProfilePersonaType](./literals.md#launchprofilepersonatype) 
## NewStudioMemberTypeDef

```python
# NewStudioMemberTypeDef definition

class NewStudioMemberTypeDef(TypedDict):
    persona: StudioPersonaType,  # (1)
    principalId: str,
```

1. See [:material-code-brackets: StudioPersonaType](./literals.md#studiopersonatype) 
## SharedFileSystemConfigurationTypeDef

```python
# SharedFileSystemConfigurationTypeDef definition

class SharedFileSystemConfigurationTypeDef(TypedDict):
    endpoint: NotRequired[str],
    fileSystemId: NotRequired[str],
    linuxMountPoint: NotRequired[str],
    shareName: NotRequired[str],
    windowsMountDrive: NotRequired[str],
```

## StartStreamingSessionRequestRequestTypeDef

```python
# StartStreamingSessionRequestRequestTypeDef definition

class StartStreamingSessionRequestRequestTypeDef(TypedDict):
    sessionId: str,
    studioId: str,
    backupId: NotRequired[str],
    clientToken: NotRequired[str],
```

## StartStudioSSOConfigurationRepairRequestRequestTypeDef

```python
# StartStudioSSOConfigurationRepairRequestRequestTypeDef definition

class StartStudioSSOConfigurationRepairRequestRequestTypeDef(TypedDict):
    studioId: str,
    clientToken: NotRequired[str],
```

## StopStreamingSessionRequestRequestTypeDef

```python
# StopStreamingSessionRequestRequestTypeDef definition

class StopStreamingSessionRequestRequestTypeDef(TypedDict):
    sessionId: str,
    studioId: str,
    clientToken: NotRequired[str],
    volumeRetentionMode: NotRequired[VolumeRetentionModeType],  # (1)
```

1. See [:material-code-brackets: VolumeRetentionModeType](./literals.md#volumeretentionmodetype) 
## StreamConfigurationSessionBackupTypeDef

```python
# StreamConfigurationSessionBackupTypeDef definition

class StreamConfigurationSessionBackupTypeDef(TypedDict):
    maxBackupsToRetain: NotRequired[int],
    mode: NotRequired[SessionBackupModeType],  # (1)
```

1. See [:material-code-brackets: SessionBackupModeType](./literals.md#sessionbackupmodetype) 
## VolumeConfigurationTypeDef

```python
# VolumeConfigurationTypeDef definition

class VolumeConfigurationTypeDef(TypedDict):
    iops: NotRequired[int],
    size: NotRequired[int],
    throughput: NotRequired[int],
```

## StreamingSessionStorageRootTypeDef

```python
# StreamingSessionStorageRootTypeDef definition

class StreamingSessionStorageRootTypeDef(TypedDict):
    linux: NotRequired[str],
    windows: NotRequired[str],
```

## StreamingImageEncryptionConfigurationTypeDef

```python
# StreamingImageEncryptionConfigurationTypeDef definition

class StreamingImageEncryptionConfigurationTypeDef(TypedDict):
    keyType: StreamingImageEncryptionConfigurationKeyTypeType,  # (1)
    keyArn: NotRequired[str],
```

1. See [:material-code-brackets: StreamingImageEncryptionConfigurationKeyTypeType](./literals.md#streamingimageencryptionconfigurationkeytypetype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: NotRequired[Mapping[str, str]],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateLaunchProfileMemberRequestRequestTypeDef

```python
# UpdateLaunchProfileMemberRequestRequestTypeDef definition

class UpdateLaunchProfileMemberRequestRequestTypeDef(TypedDict):
    launchProfileId: str,
    persona: LaunchProfilePersonaType,  # (1)
    principalId: str,
    studioId: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: LaunchProfilePersonaType](./literals.md#launchprofilepersonatype) 
## UpdateStreamingImageRequestRequestTypeDef

```python
# UpdateStreamingImageRequestRequestTypeDef definition

class UpdateStreamingImageRequestRequestTypeDef(TypedDict):
    streamingImageId: str,
    studioId: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    name: NotRequired[str],
```

## UpdateStudioRequestRequestTypeDef

```python
# UpdateStudioRequestRequestTypeDef definition

class UpdateStudioRequestRequestTypeDef(TypedDict):
    studioId: str,
    adminRoleArn: NotRequired[str],
    clientToken: NotRequired[str],
    displayName: NotRequired[str],
    userRoleArn: NotRequired[str],
```

## AcceptEulasResponseTypeDef

```python
# AcceptEulasResponseTypeDef definition

class AcceptEulasResponseTypeDef(TypedDict):
    eulaAcceptances: List[EulaAcceptanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EulaAcceptanceTypeDef](./type_defs.md#eulaacceptancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEulaAcceptancesResponseTypeDef

```python
# ListEulaAcceptancesResponseTypeDef definition

class ListEulaAcceptancesResponseTypeDef(TypedDict):
    eulaAcceptances: List[EulaAcceptanceTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EulaAcceptanceTypeDef](./type_defs.md#eulaacceptancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActiveDirectoryConfigurationTypeDef

```python
# ActiveDirectoryConfigurationTypeDef definition

class ActiveDirectoryConfigurationTypeDef(TypedDict):
    computerAttributes: NotRequired[Sequence[ActiveDirectoryComputerAttributeTypeDef]],  # (1)
    directoryId: NotRequired[str],
    organizationalUnitDistinguishedName: NotRequired[str],
```

1. See [:material-code-braces: ActiveDirectoryComputerAttributeTypeDef](./type_defs.md#activedirectorycomputerattributetypedef) 
## LaunchProfileInitializationActiveDirectoryTypeDef

```python
# LaunchProfileInitializationActiveDirectoryTypeDef definition

class LaunchProfileInitializationActiveDirectoryTypeDef(TypedDict):
    computerAttributes: NotRequired[List[ActiveDirectoryComputerAttributeTypeDef]],  # (1)
    directoryId: NotRequired[str],
    directoryName: NotRequired[str],
    dnsIpAddresses: NotRequired[List[str]],
    organizationalUnitDistinguishedName: NotRequired[str],
    studioComponentId: NotRequired[str],
    studioComponentName: NotRequired[str],
```

1. See [:material-code-braces: ActiveDirectoryComputerAttributeTypeDef](./type_defs.md#activedirectorycomputerattributetypedef) 
## CreateStreamingSessionStreamResponseTypeDef

```python
# CreateStreamingSessionStreamResponseTypeDef definition

class CreateStreamingSessionStreamResponseTypeDef(TypedDict):
    stream: StreamingSessionStreamTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingSessionStreamTypeDef](./type_defs.md#streamingsessionstreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStreamingSessionStreamResponseTypeDef

```python
# GetStreamingSessionStreamResponseTypeDef definition

class GetStreamingSessionStreamResponseTypeDef(TypedDict):
    stream: StreamingSessionStreamTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingSessionStreamTypeDef](./type_defs.md#streamingsessionstreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStudioRequestRequestTypeDef

```python
# CreateStudioRequestRequestTypeDef definition

class CreateStudioRequestRequestTypeDef(TypedDict):
    adminRoleArn: str,
    displayName: str,
    studioName: str,
    userRoleArn: str,
    clientToken: NotRequired[str],
    studioEncryptionConfiguration: NotRequired[StudioEncryptionConfigurationTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: StudioEncryptionConfigurationTypeDef](./type_defs.md#studioencryptionconfigurationtypedef) 
## StudioTypeDef

```python
# StudioTypeDef definition

class StudioTypeDef(TypedDict):
    adminRoleArn: NotRequired[str],
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    displayName: NotRequired[str],
    homeRegion: NotRequired[str],
    ssoClientId: NotRequired[str],
    state: NotRequired[StudioStateType],  # (1)
    statusCode: NotRequired[StudioStatusCodeType],  # (2)
    statusMessage: NotRequired[str],
    studioEncryptionConfiguration: NotRequired[StudioEncryptionConfigurationTypeDef],  # (3)
    studioId: NotRequired[str],
    studioName: NotRequired[str],
    studioUrl: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    updatedAt: NotRequired[datetime],
    userRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: StudioStateType](./literals.md#studiostatetype) 
2. See [:material-code-brackets: StudioStatusCodeType](./literals.md#studiostatuscodetype) 
3. See [:material-code-braces: StudioEncryptionConfigurationTypeDef](./type_defs.md#studioencryptionconfigurationtypedef) 
## GetEulaResponseTypeDef

```python
# GetEulaResponseTypeDef definition

class GetEulaResponseTypeDef(TypedDict):
    eula: EulaTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EulaTypeDef](./type_defs.md#eulatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEulasResponseTypeDef

```python
# ListEulasResponseTypeDef definition

class ListEulasResponseTypeDef(TypedDict):
    eulas: List[EulaTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EulaTypeDef](./type_defs.md#eulatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLaunchProfileMemberResponseTypeDef

```python
# GetLaunchProfileMemberResponseTypeDef definition

class GetLaunchProfileMemberResponseTypeDef(TypedDict):
    member: LaunchProfileMembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchProfileMembershipTypeDef](./type_defs.md#launchprofilemembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLaunchProfileMembersResponseTypeDef

```python
# ListLaunchProfileMembersResponseTypeDef definition

class ListLaunchProfileMembersResponseTypeDef(TypedDict):
    members: List[LaunchProfileMembershipTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchProfileMembershipTypeDef](./type_defs.md#launchprofilemembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLaunchProfileMemberResponseTypeDef

```python
# UpdateLaunchProfileMemberResponseTypeDef definition

class UpdateLaunchProfileMemberResponseTypeDef(TypedDict):
    member: LaunchProfileMembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchProfileMembershipTypeDef](./type_defs.md#launchprofilemembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef

```python
# GetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef definition

class GetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef(TypedDict):
    launchProfileId: str,
    studioId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetLaunchProfileRequestLaunchProfileReadyWaitTypeDef

```python
# GetLaunchProfileRequestLaunchProfileReadyWaitTypeDef definition

class GetLaunchProfileRequestLaunchProfileReadyWaitTypeDef(TypedDict):
    launchProfileId: str,
    studioId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetStreamingImageRequestStreamingImageDeletedWaitTypeDef

```python
# GetStreamingImageRequestStreamingImageDeletedWaitTypeDef definition

class GetStreamingImageRequestStreamingImageDeletedWaitTypeDef(TypedDict):
    streamingImageId: str,
    studioId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetStreamingImageRequestStreamingImageReadyWaitTypeDef

```python
# GetStreamingImageRequestStreamingImageReadyWaitTypeDef definition

class GetStreamingImageRequestStreamingImageReadyWaitTypeDef(TypedDict):
    streamingImageId: str,
    studioId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef

```python
# GetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef definition

class GetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef(TypedDict):
    sessionId: str,
    studioId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetStreamingSessionRequestStreamingSessionReadyWaitTypeDef

```python
# GetStreamingSessionRequestStreamingSessionReadyWaitTypeDef definition

class GetStreamingSessionRequestStreamingSessionReadyWaitTypeDef(TypedDict):
    sessionId: str,
    studioId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef

```python
# GetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef definition

class GetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef(TypedDict):
    sessionId: str,
    studioId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef

```python
# GetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef definition

class GetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef(TypedDict):
    sessionId: str,
    streamId: str,
    studioId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetStudioComponentRequestStudioComponentDeletedWaitTypeDef

```python
# GetStudioComponentRequestStudioComponentDeletedWaitTypeDef definition

class GetStudioComponentRequestStudioComponentDeletedWaitTypeDef(TypedDict):
    studioComponentId: str,
    studioId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetStudioComponentRequestStudioComponentReadyWaitTypeDef

```python
# GetStudioComponentRequestStudioComponentReadyWaitTypeDef definition

class GetStudioComponentRequestStudioComponentReadyWaitTypeDef(TypedDict):
    studioComponentId: str,
    studioId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetStudioRequestStudioDeletedWaitTypeDef

```python
# GetStudioRequestStudioDeletedWaitTypeDef definition

class GetStudioRequestStudioDeletedWaitTypeDef(TypedDict):
    studioId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetStudioRequestStudioReadyWaitTypeDef

```python
# GetStudioRequestStudioReadyWaitTypeDef definition

class GetStudioRequestStudioReadyWaitTypeDef(TypedDict):
    studioId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetStreamingSessionBackupResponseTypeDef

```python
# GetStreamingSessionBackupResponseTypeDef definition

class GetStreamingSessionBackupResponseTypeDef(TypedDict):
    streamingSessionBackup: StreamingSessionBackupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingSessionBackupTypeDef](./type_defs.md#streamingsessionbackuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStreamingSessionBackupsResponseTypeDef

```python
# ListStreamingSessionBackupsResponseTypeDef definition

class ListStreamingSessionBackupsResponseTypeDef(TypedDict):
    nextToken: str,
    streamingSessionBackups: List[StreamingSessionBackupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingSessionBackupTypeDef](./type_defs.md#streamingsessionbackuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStudioMemberResponseTypeDef

```python
# GetStudioMemberResponseTypeDef definition

class GetStudioMemberResponseTypeDef(TypedDict):
    member: StudioMembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioMembershipTypeDef](./type_defs.md#studiomembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStudioMembersResponseTypeDef

```python
# ListStudioMembersResponseTypeDef definition

class ListStudioMembersResponseTypeDef(TypedDict):
    members: List[StudioMembershipTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioMembershipTypeDef](./type_defs.md#studiomembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef

```python
# ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef definition

class ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef(TypedDict):
    studioId: str,
    eulaIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEulasRequestListEulasPaginateTypeDef

```python
# ListEulasRequestListEulasPaginateTypeDef definition

class ListEulasRequestListEulasPaginateTypeDef(TypedDict):
    eulaIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef

```python
# ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef definition

class ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef(TypedDict):
    launchProfileId: str,
    studioId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef

```python
# ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef definition

class ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef(TypedDict):
    studioId: str,
    principalId: NotRequired[str],
    states: NotRequired[Sequence[LaunchProfileStateType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LaunchProfileStateType](./literals.md#launchprofilestatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStreamingImagesRequestListStreamingImagesPaginateTypeDef

```python
# ListStreamingImagesRequestListStreamingImagesPaginateTypeDef definition

class ListStreamingImagesRequestListStreamingImagesPaginateTypeDef(TypedDict):
    studioId: str,
    owner: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef

```python
# ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef definition

class ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef(TypedDict):
    studioId: str,
    ownedBy: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef

```python
# ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef definition

class ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef(TypedDict):
    studioId: str,
    createdBy: NotRequired[str],
    ownedBy: NotRequired[str],
    sessionIds: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStudioComponentsRequestListStudioComponentsPaginateTypeDef

```python
# ListStudioComponentsRequestListStudioComponentsPaginateTypeDef definition

class ListStudioComponentsRequestListStudioComponentsPaginateTypeDef(TypedDict):
    studioId: str,
    states: NotRequired[Sequence[StudioComponentStateType]],  # (1)
    types: NotRequired[Sequence[StudioComponentTypeType]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: StudioComponentStateType](./literals.md#studiocomponentstatetype) 
2. See [:material-code-brackets: StudioComponentTypeType](./literals.md#studiocomponenttypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStudioMembersRequestListStudioMembersPaginateTypeDef

```python
# ListStudioMembersRequestListStudioMembersPaginateTypeDef definition

class ListStudioMembersRequestListStudioMembersPaginateTypeDef(TypedDict):
    studioId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStudiosRequestListStudiosPaginateTypeDef

```python
# ListStudiosRequestListStudiosPaginateTypeDef definition

class ListStudiosRequestListStudiosPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## PutLaunchProfileMembersRequestRequestTypeDef

```python
# PutLaunchProfileMembersRequestRequestTypeDef definition

class PutLaunchProfileMembersRequestRequestTypeDef(TypedDict):
    identityStoreId: str,
    launchProfileId: str,
    members: Sequence[NewLaunchProfileMemberTypeDef],  # (1)
    studioId: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: NewLaunchProfileMemberTypeDef](./type_defs.md#newlaunchprofilemembertypedef) 
## PutStudioMembersRequestRequestTypeDef

```python
# PutStudioMembersRequestRequestTypeDef definition

class PutStudioMembersRequestRequestTypeDef(TypedDict):
    identityStoreId: str,
    members: Sequence[NewStudioMemberTypeDef],  # (1)
    studioId: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: NewStudioMemberTypeDef](./type_defs.md#newstudiomembertypedef) 
## StreamingSessionTypeDef

```python
# StreamingSessionTypeDef definition

class StreamingSessionTypeDef(TypedDict):
    arn: NotRequired[str],
    automaticTerminationMode: NotRequired[AutomaticTerminationModeType],  # (1)
    backupMode: NotRequired[SessionBackupModeType],  # (2)
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    ec2InstanceType: NotRequired[str],
    launchProfileId: NotRequired[str],
    maxBackupsToRetain: NotRequired[int],
    ownedBy: NotRequired[str],
    sessionId: NotRequired[str],
    sessionPersistenceMode: NotRequired[SessionPersistenceModeType],  # (3)
    startedAt: NotRequired[datetime],
    startedBy: NotRequired[str],
    startedFromBackupId: NotRequired[str],
    state: NotRequired[StreamingSessionStateType],  # (4)
    statusCode: NotRequired[StreamingSessionStatusCodeType],  # (5)
    statusMessage: NotRequired[str],
    stopAt: NotRequired[datetime],
    stoppedAt: NotRequired[datetime],
    stoppedBy: NotRequired[str],
    streamingImageId: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    terminateAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
    volumeConfiguration: NotRequired[VolumeConfigurationTypeDef],  # (6)
    volumeRetentionMode: NotRequired[VolumeRetentionModeType],  # (7)
```

1. See [:material-code-brackets: AutomaticTerminationModeType](./literals.md#automaticterminationmodetype) 
2. See [:material-code-brackets: SessionBackupModeType](./literals.md#sessionbackupmodetype) 
3. See [:material-code-brackets: SessionPersistenceModeType](./literals.md#sessionpersistencemodetype) 
4. See [:material-code-brackets: StreamingSessionStateType](./literals.md#streamingsessionstatetype) 
5. See [:material-code-brackets: StreamingSessionStatusCodeType](./literals.md#streamingsessionstatuscodetype) 
6. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
7. See [:material-code-brackets: VolumeRetentionModeType](./literals.md#volumeretentionmodetype) 
## StreamConfigurationSessionStorageTypeDef

```python
# StreamConfigurationSessionStorageTypeDef definition

class StreamConfigurationSessionStorageTypeDef(TypedDict):
    mode: Sequence[StreamingSessionStorageModeType],  # (1)
    root: NotRequired[StreamingSessionStorageRootTypeDef],  # (2)
```

1. See [:material-code-brackets: StreamingSessionStorageModeType](./literals.md#streamingsessionstoragemodetype) 
2. See [:material-code-braces: StreamingSessionStorageRootTypeDef](./type_defs.md#streamingsessionstorageroottypedef) 
## StreamingImageTypeDef

```python
# StreamingImageTypeDef definition

class StreamingImageTypeDef(TypedDict):
    arn: NotRequired[str],
    description: NotRequired[str],
    ec2ImageId: NotRequired[str],
    encryptionConfiguration: NotRequired[StreamingImageEncryptionConfigurationTypeDef],  # (1)
    eulaIds: NotRequired[List[str]],
    name: NotRequired[str],
    owner: NotRequired[str],
    platform: NotRequired[str],
    state: NotRequired[StreamingImageStateType],  # (2)
    statusCode: NotRequired[StreamingImageStatusCodeType],  # (3)
    statusMessage: NotRequired[str],
    streamingImageId: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: StreamingImageEncryptionConfigurationTypeDef](./type_defs.md#streamingimageencryptionconfigurationtypedef) 
2. See [:material-code-brackets: StreamingImageStateType](./literals.md#streamingimagestatetype) 
3. See [:material-code-brackets: StreamingImageStatusCodeType](./literals.md#streamingimagestatuscodetype) 
## StudioComponentConfigurationTypeDef

```python
# StudioComponentConfigurationTypeDef definition

class StudioComponentConfigurationTypeDef(TypedDict):
    activeDirectoryConfiguration: NotRequired[ActiveDirectoryConfigurationTypeDef],  # (1)
    computeFarmConfiguration: NotRequired[ComputeFarmConfigurationTypeDef],  # (2)
    licenseServiceConfiguration: NotRequired[LicenseServiceConfigurationTypeDef],  # (3)
    sharedFileSystemConfiguration: NotRequired[SharedFileSystemConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: ActiveDirectoryConfigurationTypeDef](./type_defs.md#activedirectoryconfigurationtypedef) 
2. See [:material-code-braces: ComputeFarmConfigurationTypeDef](./type_defs.md#computefarmconfigurationtypedef) 
3. See [:material-code-braces: LicenseServiceConfigurationTypeDef](./type_defs.md#licenseserviceconfigurationtypedef) 
4. See [:material-code-braces: SharedFileSystemConfigurationTypeDef](./type_defs.md#sharedfilesystemconfigurationtypedef) 
## LaunchProfileInitializationTypeDef

```python
# LaunchProfileInitializationTypeDef definition

class LaunchProfileInitializationTypeDef(TypedDict):
    activeDirectory: NotRequired[LaunchProfileInitializationActiveDirectoryTypeDef],  # (1)
    ec2SecurityGroupIds: NotRequired[List[str]],
    launchProfileId: NotRequired[str],
    launchProfileProtocolVersion: NotRequired[str],
    launchPurpose: NotRequired[str],
    name: NotRequired[str],
    platform: NotRequired[LaunchProfilePlatformType],  # (2)
    systemInitializationScripts: NotRequired[List[LaunchProfileInitializationScriptTypeDef]],  # (3)
    userInitializationScripts: NotRequired[List[LaunchProfileInitializationScriptTypeDef]],  # (3)
```

1. See [:material-code-braces: LaunchProfileInitializationActiveDirectoryTypeDef](./type_defs.md#launchprofileinitializationactivedirectorytypedef) 
2. See [:material-code-brackets: LaunchProfilePlatformType](./literals.md#launchprofileplatformtype) 
3. See [:material-code-braces: LaunchProfileInitializationScriptTypeDef](./type_defs.md#launchprofileinitializationscripttypedef) 
4. See [:material-code-braces: LaunchProfileInitializationScriptTypeDef](./type_defs.md#launchprofileinitializationscripttypedef) 
## CreateStudioResponseTypeDef

```python
# CreateStudioResponseTypeDef definition

class CreateStudioResponseTypeDef(TypedDict):
    studio: StudioTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioTypeDef](./type_defs.md#studiotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteStudioResponseTypeDef

```python
# DeleteStudioResponseTypeDef definition

class DeleteStudioResponseTypeDef(TypedDict):
    studio: StudioTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioTypeDef](./type_defs.md#studiotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStudioResponseTypeDef

```python
# GetStudioResponseTypeDef definition

class GetStudioResponseTypeDef(TypedDict):
    studio: StudioTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioTypeDef](./type_defs.md#studiotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStudiosResponseTypeDef

```python
# ListStudiosResponseTypeDef definition

class ListStudiosResponseTypeDef(TypedDict):
    nextToken: str,
    studios: List[StudioTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioTypeDef](./type_defs.md#studiotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartStudioSSOConfigurationRepairResponseTypeDef

```python
# StartStudioSSOConfigurationRepairResponseTypeDef definition

class StartStudioSSOConfigurationRepairResponseTypeDef(TypedDict):
    studio: StudioTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioTypeDef](./type_defs.md#studiotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStudioResponseTypeDef

```python
# UpdateStudioResponseTypeDef definition

class UpdateStudioResponseTypeDef(TypedDict):
    studio: StudioTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioTypeDef](./type_defs.md#studiotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStreamingSessionResponseTypeDef

```python
# CreateStreamingSessionResponseTypeDef definition

class CreateStreamingSessionResponseTypeDef(TypedDict):
    session: StreamingSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingSessionTypeDef](./type_defs.md#streamingsessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteStreamingSessionResponseTypeDef

```python
# DeleteStreamingSessionResponseTypeDef definition

class DeleteStreamingSessionResponseTypeDef(TypedDict):
    session: StreamingSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingSessionTypeDef](./type_defs.md#streamingsessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStreamingSessionResponseTypeDef

```python
# GetStreamingSessionResponseTypeDef definition

class GetStreamingSessionResponseTypeDef(TypedDict):
    session: StreamingSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingSessionTypeDef](./type_defs.md#streamingsessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStreamingSessionsResponseTypeDef

```python
# ListStreamingSessionsResponseTypeDef definition

class ListStreamingSessionsResponseTypeDef(TypedDict):
    nextToken: str,
    sessions: List[StreamingSessionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingSessionTypeDef](./type_defs.md#streamingsessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartStreamingSessionResponseTypeDef

```python
# StartStreamingSessionResponseTypeDef definition

class StartStreamingSessionResponseTypeDef(TypedDict):
    session: StreamingSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingSessionTypeDef](./type_defs.md#streamingsessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopStreamingSessionResponseTypeDef

```python
# StopStreamingSessionResponseTypeDef definition

class StopStreamingSessionResponseTypeDef(TypedDict):
    session: StreamingSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingSessionTypeDef](./type_defs.md#streamingsessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StreamConfigurationCreateTypeDef

```python
# StreamConfigurationCreateTypeDef definition

class StreamConfigurationCreateTypeDef(TypedDict):
    clipboardMode: StreamingClipboardModeType,  # (2)
    ec2InstanceTypes: Sequence[StreamingInstanceTypeType],  # (3)
    streamingImageIds: Sequence[str],
    automaticTerminationMode: NotRequired[AutomaticTerminationModeType],  # (1)
    maxSessionLengthInMinutes: NotRequired[int],
    maxStoppedSessionLengthInMinutes: NotRequired[int],
    sessionBackup: NotRequired[StreamConfigurationSessionBackupTypeDef],  # (4)
    sessionPersistenceMode: NotRequired[SessionPersistenceModeType],  # (5)
    sessionStorage: NotRequired[StreamConfigurationSessionStorageTypeDef],  # (6)
    volumeConfiguration: NotRequired[VolumeConfigurationTypeDef],  # (7)
```

1. See [:material-code-brackets: AutomaticTerminationModeType](./literals.md#automaticterminationmodetype) 
2. See [:material-code-brackets: StreamingClipboardModeType](./literals.md#streamingclipboardmodetype) 
3. See [:material-code-brackets: StreamingInstanceTypeType](./literals.md#streaminginstancetypetype) 
4. See [:material-code-braces: StreamConfigurationSessionBackupTypeDef](./type_defs.md#streamconfigurationsessionbackuptypedef) 
5. See [:material-code-brackets: SessionPersistenceModeType](./literals.md#sessionpersistencemodetype) 
6. See [:material-code-braces: StreamConfigurationSessionStorageTypeDef](./type_defs.md#streamconfigurationsessionstoragetypedef) 
7. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
## StreamConfigurationTypeDef

```python
# StreamConfigurationTypeDef definition

class StreamConfigurationTypeDef(TypedDict):
    clipboardMode: StreamingClipboardModeType,  # (2)
    ec2InstanceTypes: List[StreamingInstanceTypeType],  # (3)
    streamingImageIds: List[str],
    automaticTerminationMode: NotRequired[AutomaticTerminationModeType],  # (1)
    maxSessionLengthInMinutes: NotRequired[int],
    maxStoppedSessionLengthInMinutes: NotRequired[int],
    sessionBackup: NotRequired[StreamConfigurationSessionBackupTypeDef],  # (4)
    sessionPersistenceMode: NotRequired[SessionPersistenceModeType],  # (5)
    sessionStorage: NotRequired[StreamConfigurationSessionStorageTypeDef],  # (6)
    volumeConfiguration: NotRequired[VolumeConfigurationTypeDef],  # (7)
```

1. See [:material-code-brackets: AutomaticTerminationModeType](./literals.md#automaticterminationmodetype) 
2. See [:material-code-brackets: StreamingClipboardModeType](./literals.md#streamingclipboardmodetype) 
3. See [:material-code-brackets: StreamingInstanceTypeType](./literals.md#streaminginstancetypetype) 
4. See [:material-code-braces: StreamConfigurationSessionBackupTypeDef](./type_defs.md#streamconfigurationsessionbackuptypedef) 
5. See [:material-code-brackets: SessionPersistenceModeType](./literals.md#sessionpersistencemodetype) 
6. See [:material-code-braces: StreamConfigurationSessionStorageTypeDef](./type_defs.md#streamconfigurationsessionstoragetypedef) 
7. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
## CreateStreamingImageResponseTypeDef

```python
# CreateStreamingImageResponseTypeDef definition

class CreateStreamingImageResponseTypeDef(TypedDict):
    streamingImage: StreamingImageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingImageTypeDef](./type_defs.md#streamingimagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteStreamingImageResponseTypeDef

```python
# DeleteStreamingImageResponseTypeDef definition

class DeleteStreamingImageResponseTypeDef(TypedDict):
    streamingImage: StreamingImageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingImageTypeDef](./type_defs.md#streamingimagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStreamingImageResponseTypeDef

```python
# GetStreamingImageResponseTypeDef definition

class GetStreamingImageResponseTypeDef(TypedDict):
    streamingImage: StreamingImageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingImageTypeDef](./type_defs.md#streamingimagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStreamingImagesResponseTypeDef

```python
# ListStreamingImagesResponseTypeDef definition

class ListStreamingImagesResponseTypeDef(TypedDict):
    nextToken: str,
    streamingImages: List[StreamingImageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingImageTypeDef](./type_defs.md#streamingimagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStreamingImageResponseTypeDef

```python
# UpdateStreamingImageResponseTypeDef definition

class UpdateStreamingImageResponseTypeDef(TypedDict):
    streamingImage: StreamingImageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingImageTypeDef](./type_defs.md#streamingimagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStudioComponentRequestRequestTypeDef

```python
# CreateStudioComponentRequestRequestTypeDef definition

class CreateStudioComponentRequestRequestTypeDef(TypedDict):
    name: str,
    studioId: str,
    type: StudioComponentTypeType,  # (1)
    clientToken: NotRequired[str],
    configuration: NotRequired[StudioComponentConfigurationTypeDef],  # (2)
    description: NotRequired[str],
    ec2SecurityGroupIds: NotRequired[Sequence[str]],
    initializationScripts: NotRequired[Sequence[StudioComponentInitializationScriptTypeDef]],  # (3)
    runtimeRoleArn: NotRequired[str],
    scriptParameters: NotRequired[Sequence[ScriptParameterKeyValueTypeDef]],  # (4)
    secureInitializationRoleArn: NotRequired[str],
    subtype: NotRequired[StudioComponentSubtypeType],  # (5)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: StudioComponentTypeType](./literals.md#studiocomponenttypetype) 
2. See [:material-code-braces: StudioComponentConfigurationTypeDef](./type_defs.md#studiocomponentconfigurationtypedef) 
3. See [:material-code-braces: StudioComponentInitializationScriptTypeDef](./type_defs.md#studiocomponentinitializationscripttypedef) 
4. See [:material-code-braces: ScriptParameterKeyValueTypeDef](./type_defs.md#scriptparameterkeyvaluetypedef) 
5. See [:material-code-brackets: StudioComponentSubtypeType](./literals.md#studiocomponentsubtypetype) 
## StudioComponentTypeDef

```python
# StudioComponentTypeDef definition

class StudioComponentTypeDef(TypedDict):
    arn: NotRequired[str],
    configuration: NotRequired[StudioComponentConfigurationTypeDef],  # (1)
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    description: NotRequired[str],
    ec2SecurityGroupIds: NotRequired[List[str]],
    initializationScripts: NotRequired[List[StudioComponentInitializationScriptTypeDef]],  # (2)
    name: NotRequired[str],
    runtimeRoleArn: NotRequired[str],
    scriptParameters: NotRequired[List[ScriptParameterKeyValueTypeDef]],  # (3)
    secureInitializationRoleArn: NotRequired[str],
    state: NotRequired[StudioComponentStateType],  # (4)
    statusCode: NotRequired[StudioComponentStatusCodeType],  # (5)
    statusMessage: NotRequired[str],
    studioComponentId: NotRequired[str],
    subtype: NotRequired[StudioComponentSubtypeType],  # (6)
    tags: NotRequired[Dict[str, str]],
    type: NotRequired[StudioComponentTypeType],  # (7)
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

1. See [:material-code-braces: StudioComponentConfigurationTypeDef](./type_defs.md#studiocomponentconfigurationtypedef) 
2. See [:material-code-braces: StudioComponentInitializationScriptTypeDef](./type_defs.md#studiocomponentinitializationscripttypedef) 
3. See [:material-code-braces: ScriptParameterKeyValueTypeDef](./type_defs.md#scriptparameterkeyvaluetypedef) 
4. See [:material-code-brackets: StudioComponentStateType](./literals.md#studiocomponentstatetype) 
5. See [:material-code-brackets: StudioComponentStatusCodeType](./literals.md#studiocomponentstatuscodetype) 
6. See [:material-code-brackets: StudioComponentSubtypeType](./literals.md#studiocomponentsubtypetype) 
7. See [:material-code-brackets: StudioComponentTypeType](./literals.md#studiocomponenttypetype) 
## UpdateStudioComponentRequestRequestTypeDef

```python
# UpdateStudioComponentRequestRequestTypeDef definition

class UpdateStudioComponentRequestRequestTypeDef(TypedDict):
    studioComponentId: str,
    studioId: str,
    clientToken: NotRequired[str],
    configuration: NotRequired[StudioComponentConfigurationTypeDef],  # (1)
    description: NotRequired[str],
    ec2SecurityGroupIds: NotRequired[Sequence[str]],
    initializationScripts: NotRequired[Sequence[StudioComponentInitializationScriptTypeDef]],  # (2)
    name: NotRequired[str],
    runtimeRoleArn: NotRequired[str],
    scriptParameters: NotRequired[Sequence[ScriptParameterKeyValueTypeDef]],  # (3)
    secureInitializationRoleArn: NotRequired[str],
    subtype: NotRequired[StudioComponentSubtypeType],  # (4)
    type: NotRequired[StudioComponentTypeType],  # (5)
```

1. See [:material-code-braces: StudioComponentConfigurationTypeDef](./type_defs.md#studiocomponentconfigurationtypedef) 
2. See [:material-code-braces: StudioComponentInitializationScriptTypeDef](./type_defs.md#studiocomponentinitializationscripttypedef) 
3. See [:material-code-braces: ScriptParameterKeyValueTypeDef](./type_defs.md#scriptparameterkeyvaluetypedef) 
4. See [:material-code-brackets: StudioComponentSubtypeType](./literals.md#studiocomponentsubtypetype) 
5. See [:material-code-brackets: StudioComponentTypeType](./literals.md#studiocomponenttypetype) 
## GetLaunchProfileInitializationResponseTypeDef

```python
# GetLaunchProfileInitializationResponseTypeDef definition

class GetLaunchProfileInitializationResponseTypeDef(TypedDict):
    launchProfileInitialization: LaunchProfileInitializationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchProfileInitializationTypeDef](./type_defs.md#launchprofileinitializationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLaunchProfileRequestRequestTypeDef

```python
# CreateLaunchProfileRequestRequestTypeDef definition

class CreateLaunchProfileRequestRequestTypeDef(TypedDict):
    ec2SubnetIds: Sequence[str],
    launchProfileProtocolVersions: Sequence[str],
    name: str,
    streamConfiguration: StreamConfigurationCreateTypeDef,  # (1)
    studioComponentIds: Sequence[str],
    studioId: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: StreamConfigurationCreateTypeDef](./type_defs.md#streamconfigurationcreatetypedef) 
## UpdateLaunchProfileRequestRequestTypeDef

```python
# UpdateLaunchProfileRequestRequestTypeDef definition

class UpdateLaunchProfileRequestRequestTypeDef(TypedDict):
    launchProfileId: str,
    studioId: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    launchProfileProtocolVersions: NotRequired[Sequence[str]],
    name: NotRequired[str],
    streamConfiguration: NotRequired[StreamConfigurationCreateTypeDef],  # (1)
    studioComponentIds: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: StreamConfigurationCreateTypeDef](./type_defs.md#streamconfigurationcreatetypedef) 
## LaunchProfileTypeDef

```python
# LaunchProfileTypeDef definition

class LaunchProfileTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    description: NotRequired[str],
    ec2SubnetIds: NotRequired[List[str]],
    launchProfileId: NotRequired[str],
    launchProfileProtocolVersions: NotRequired[List[str]],
    name: NotRequired[str],
    state: NotRequired[LaunchProfileStateType],  # (1)
    statusCode: NotRequired[LaunchProfileStatusCodeType],  # (2)
    statusMessage: NotRequired[str],
    streamConfiguration: NotRequired[StreamConfigurationTypeDef],  # (3)
    studioComponentIds: NotRequired[List[str]],
    tags: NotRequired[Dict[str, str]],
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
    validationResults: NotRequired[List[ValidationResultTypeDef]],  # (4)
```

1. See [:material-code-brackets: LaunchProfileStateType](./literals.md#launchprofilestatetype) 
2. See [:material-code-brackets: LaunchProfileStatusCodeType](./literals.md#launchprofilestatuscodetype) 
3. See [:material-code-braces: StreamConfigurationTypeDef](./type_defs.md#streamconfigurationtypedef) 
4. See [:material-code-braces: ValidationResultTypeDef](./type_defs.md#validationresulttypedef) 
## CreateStudioComponentResponseTypeDef

```python
# CreateStudioComponentResponseTypeDef definition

class CreateStudioComponentResponseTypeDef(TypedDict):
    studioComponent: StudioComponentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioComponentTypeDef](./type_defs.md#studiocomponenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteStudioComponentResponseTypeDef

```python
# DeleteStudioComponentResponseTypeDef definition

class DeleteStudioComponentResponseTypeDef(TypedDict):
    studioComponent: StudioComponentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioComponentTypeDef](./type_defs.md#studiocomponenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStudioComponentResponseTypeDef

```python
# GetStudioComponentResponseTypeDef definition

class GetStudioComponentResponseTypeDef(TypedDict):
    studioComponent: StudioComponentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioComponentTypeDef](./type_defs.md#studiocomponenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStudioComponentsResponseTypeDef

```python
# ListStudioComponentsResponseTypeDef definition

class ListStudioComponentsResponseTypeDef(TypedDict):
    nextToken: str,
    studioComponents: List[StudioComponentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioComponentTypeDef](./type_defs.md#studiocomponenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStudioComponentResponseTypeDef

```python
# UpdateStudioComponentResponseTypeDef definition

class UpdateStudioComponentResponseTypeDef(TypedDict):
    studioComponent: StudioComponentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioComponentTypeDef](./type_defs.md#studiocomponenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLaunchProfileResponseTypeDef

```python
# CreateLaunchProfileResponseTypeDef definition

class CreateLaunchProfileResponseTypeDef(TypedDict):
    launchProfile: LaunchProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchProfileTypeDef](./type_defs.md#launchprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteLaunchProfileResponseTypeDef

```python
# DeleteLaunchProfileResponseTypeDef definition

class DeleteLaunchProfileResponseTypeDef(TypedDict):
    launchProfile: LaunchProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchProfileTypeDef](./type_defs.md#launchprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLaunchProfileDetailsResponseTypeDef

```python
# GetLaunchProfileDetailsResponseTypeDef definition

class GetLaunchProfileDetailsResponseTypeDef(TypedDict):
    launchProfile: LaunchProfileTypeDef,  # (1)
    streamingImages: List[StreamingImageTypeDef],  # (2)
    studioComponentSummaries: List[StudioComponentSummaryTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: LaunchProfileTypeDef](./type_defs.md#launchprofiletypedef) 
2. See [:material-code-braces: StreamingImageTypeDef](./type_defs.md#streamingimagetypedef) 
3. See [:material-code-braces: StudioComponentSummaryTypeDef](./type_defs.md#studiocomponentsummarytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLaunchProfileResponseTypeDef

```python
# GetLaunchProfileResponseTypeDef definition

class GetLaunchProfileResponseTypeDef(TypedDict):
    launchProfile: LaunchProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchProfileTypeDef](./type_defs.md#launchprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLaunchProfilesResponseTypeDef

```python
# ListLaunchProfilesResponseTypeDef definition

class ListLaunchProfilesResponseTypeDef(TypedDict):
    launchProfiles: List[LaunchProfileTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchProfileTypeDef](./type_defs.md#launchprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLaunchProfileResponseTypeDef

```python
# UpdateLaunchProfileResponseTypeDef definition

class UpdateLaunchProfileResponseTypeDef(TypedDict):
    launchProfile: LaunchProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchProfileTypeDef](./type_defs.md#launchprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
