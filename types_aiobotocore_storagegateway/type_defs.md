<a id="typed-dictionaries-for-aiobotocore-storagegateway-module"></a>

# Typed dictionaries for aiobotocore StorageGateway module

> [Index](..) > [StorageGateway](.) > Typed dictionaries

Auto-generated documentation for
[StorageGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
type annotations stubs module
[types-aiobotocore-storagegateway](https://pypi.org/project/types-aiobotocore-storagegateway/).

- [Typed dictionaries for aiobotocore StorageGateway module](#typed-dictionaries-for-aiobotocore-storagegateway-module)
  - [ActivateGatewayInputRequestTypeDef](#activategatewayinputrequesttypedef)
  - [ActivateGatewayOutputTypeDef](#activategatewayoutputtypedef)
  - [AddCacheInputRequestTypeDef](#addcacheinputrequesttypedef)
  - [AddCacheOutputTypeDef](#addcacheoutputtypedef)
  - [AddTagsToResourceInputRequestTypeDef](#addtagstoresourceinputrequesttypedef)
  - [AddTagsToResourceOutputTypeDef](#addtagstoresourceoutputtypedef)
  - [AddUploadBufferInputRequestTypeDef](#adduploadbufferinputrequesttypedef)
  - [AddUploadBufferOutputTypeDef](#adduploadbufferoutputtypedef)
  - [AddWorkingStorageInputRequestTypeDef](#addworkingstorageinputrequesttypedef)
  - [AddWorkingStorageOutputTypeDef](#addworkingstorageoutputtypedef)
  - [AssignTapePoolInputRequestTypeDef](#assigntapepoolinputrequesttypedef)
  - [AssignTapePoolOutputTypeDef](#assigntapepooloutputtypedef)
  - [AssociateFileSystemInputRequestTypeDef](#associatefilesysteminputrequesttypedef)
  - [AssociateFileSystemOutputTypeDef](#associatefilesystemoutputtypedef)
  - [AttachVolumeInputRequestTypeDef](#attachvolumeinputrequesttypedef)
  - [AttachVolumeOutputTypeDef](#attachvolumeoutputtypedef)
  - [AutomaticTapeCreationPolicyInfoTypeDef](#automatictapecreationpolicyinfotypedef)
  - [AutomaticTapeCreationRuleTypeDef](#automatictapecreationruletypedef)
  - [BandwidthRateLimitIntervalTypeDef](#bandwidthratelimitintervaltypedef)
  - [CacheAttributesTypeDef](#cacheattributestypedef)
  - [CachediSCSIVolumeTypeDef](#cachediscsivolumetypedef)
  - [CancelArchivalInputRequestTypeDef](#cancelarchivalinputrequesttypedef)
  - [CancelArchivalOutputTypeDef](#cancelarchivaloutputtypedef)
  - [CancelRetrievalInputRequestTypeDef](#cancelretrievalinputrequesttypedef)
  - [CancelRetrievalOutputTypeDef](#cancelretrievaloutputtypedef)
  - [ChapInfoTypeDef](#chapinfotypedef)
  - [CreateCachediSCSIVolumeInputRequestTypeDef](#createcachediscsivolumeinputrequesttypedef)
  - [CreateCachediSCSIVolumeOutputTypeDef](#createcachediscsivolumeoutputtypedef)
  - [CreateNFSFileShareInputRequestTypeDef](#createnfsfileshareinputrequesttypedef)
  - [CreateNFSFileShareOutputTypeDef](#createnfsfileshareoutputtypedef)
  - [CreateSMBFileShareInputRequestTypeDef](#createsmbfileshareinputrequesttypedef)
  - [CreateSMBFileShareOutputTypeDef](#createsmbfileshareoutputtypedef)
  - [CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef](#createsnapshotfromvolumerecoverypointinputrequesttypedef)
  - [CreateSnapshotFromVolumeRecoveryPointOutputTypeDef](#createsnapshotfromvolumerecoverypointoutputtypedef)
  - [CreateSnapshotInputRequestTypeDef](#createsnapshotinputrequesttypedef)
  - [CreateSnapshotOutputTypeDef](#createsnapshotoutputtypedef)
  - [CreateStorediSCSIVolumeInputRequestTypeDef](#createstorediscsivolumeinputrequesttypedef)
  - [CreateStorediSCSIVolumeOutputTypeDef](#createstorediscsivolumeoutputtypedef)
  - [CreateTapePoolInputRequestTypeDef](#createtapepoolinputrequesttypedef)
  - [CreateTapePoolOutputTypeDef](#createtapepooloutputtypedef)
  - [CreateTapeWithBarcodeInputRequestTypeDef](#createtapewithbarcodeinputrequesttypedef)
  - [CreateTapeWithBarcodeOutputTypeDef](#createtapewithbarcodeoutputtypedef)
  - [CreateTapesInputRequestTypeDef](#createtapesinputrequesttypedef)
  - [CreateTapesOutputTypeDef](#createtapesoutputtypedef)
  - [DeleteAutomaticTapeCreationPolicyInputRequestTypeDef](#deleteautomatictapecreationpolicyinputrequesttypedef)
  - [DeleteAutomaticTapeCreationPolicyOutputTypeDef](#deleteautomatictapecreationpolicyoutputtypedef)
  - [DeleteBandwidthRateLimitInputRequestTypeDef](#deletebandwidthratelimitinputrequesttypedef)
  - [DeleteBandwidthRateLimitOutputTypeDef](#deletebandwidthratelimitoutputtypedef)
  - [DeleteChapCredentialsInputRequestTypeDef](#deletechapcredentialsinputrequesttypedef)
  - [DeleteChapCredentialsOutputTypeDef](#deletechapcredentialsoutputtypedef)
  - [DeleteFileShareInputRequestTypeDef](#deletefileshareinputrequesttypedef)
  - [DeleteFileShareOutputTypeDef](#deletefileshareoutputtypedef)
  - [DeleteGatewayInputRequestTypeDef](#deletegatewayinputrequesttypedef)
  - [DeleteGatewayOutputTypeDef](#deletegatewayoutputtypedef)
  - [DeleteSnapshotScheduleInputRequestTypeDef](#deletesnapshotscheduleinputrequesttypedef)
  - [DeleteSnapshotScheduleOutputTypeDef](#deletesnapshotscheduleoutputtypedef)
  - [DeleteTapeArchiveInputRequestTypeDef](#deletetapearchiveinputrequesttypedef)
  - [DeleteTapeArchiveOutputTypeDef](#deletetapearchiveoutputtypedef)
  - [DeleteTapeInputRequestTypeDef](#deletetapeinputrequesttypedef)
  - [DeleteTapeOutputTypeDef](#deletetapeoutputtypedef)
  - [DeleteTapePoolInputRequestTypeDef](#deletetapepoolinputrequesttypedef)
  - [DeleteTapePoolOutputTypeDef](#deletetapepooloutputtypedef)
  - [DeleteVolumeInputRequestTypeDef](#deletevolumeinputrequesttypedef)
  - [DeleteVolumeOutputTypeDef](#deletevolumeoutputtypedef)
  - [DescribeAvailabilityMonitorTestInputRequestTypeDef](#describeavailabilitymonitortestinputrequesttypedef)
  - [DescribeAvailabilityMonitorTestOutputTypeDef](#describeavailabilitymonitortestoutputtypedef)
  - [DescribeBandwidthRateLimitInputRequestTypeDef](#describebandwidthratelimitinputrequesttypedef)
  - [DescribeBandwidthRateLimitOutputTypeDef](#describebandwidthratelimitoutputtypedef)
  - [DescribeBandwidthRateLimitScheduleInputRequestTypeDef](#describebandwidthratelimitscheduleinputrequesttypedef)
  - [DescribeBandwidthRateLimitScheduleOutputTypeDef](#describebandwidthratelimitscheduleoutputtypedef)
  - [DescribeCacheInputRequestTypeDef](#describecacheinputrequesttypedef)
  - [DescribeCacheOutputTypeDef](#describecacheoutputtypedef)
  - [DescribeCachediSCSIVolumesInputRequestTypeDef](#describecachediscsivolumesinputrequesttypedef)
  - [DescribeCachediSCSIVolumesOutputTypeDef](#describecachediscsivolumesoutputtypedef)
  - [DescribeChapCredentialsInputRequestTypeDef](#describechapcredentialsinputrequesttypedef)
  - [DescribeChapCredentialsOutputTypeDef](#describechapcredentialsoutputtypedef)
  - [DescribeFileSystemAssociationsInputRequestTypeDef](#describefilesystemassociationsinputrequesttypedef)
  - [DescribeFileSystemAssociationsOutputTypeDef](#describefilesystemassociationsoutputtypedef)
  - [DescribeGatewayInformationInputRequestTypeDef](#describegatewayinformationinputrequesttypedef)
  - [DescribeGatewayInformationOutputTypeDef](#describegatewayinformationoutputtypedef)
  - [DescribeMaintenanceStartTimeInputRequestTypeDef](#describemaintenancestarttimeinputrequesttypedef)
  - [DescribeMaintenanceStartTimeOutputTypeDef](#describemaintenancestarttimeoutputtypedef)
  - [DescribeNFSFileSharesInputRequestTypeDef](#describenfsfilesharesinputrequesttypedef)
  - [DescribeNFSFileSharesOutputTypeDef](#describenfsfilesharesoutputtypedef)
  - [DescribeSMBFileSharesInputRequestTypeDef](#describesmbfilesharesinputrequesttypedef)
  - [DescribeSMBFileSharesOutputTypeDef](#describesmbfilesharesoutputtypedef)
  - [DescribeSMBSettingsInputRequestTypeDef](#describesmbsettingsinputrequesttypedef)
  - [DescribeSMBSettingsOutputTypeDef](#describesmbsettingsoutputtypedef)
  - [DescribeSnapshotScheduleInputRequestTypeDef](#describesnapshotscheduleinputrequesttypedef)
  - [DescribeSnapshotScheduleOutputTypeDef](#describesnapshotscheduleoutputtypedef)
  - [DescribeStorediSCSIVolumesInputRequestTypeDef](#describestorediscsivolumesinputrequesttypedef)
  - [DescribeStorediSCSIVolumesOutputTypeDef](#describestorediscsivolumesoutputtypedef)
  - [DescribeTapeArchivesInputRequestTypeDef](#describetapearchivesinputrequesttypedef)
  - [DescribeTapeArchivesOutputTypeDef](#describetapearchivesoutputtypedef)
  - [DescribeTapeRecoveryPointsInputRequestTypeDef](#describetaperecoverypointsinputrequesttypedef)
  - [DescribeTapeRecoveryPointsOutputTypeDef](#describetaperecoverypointsoutputtypedef)
  - [DescribeTapesInputRequestTypeDef](#describetapesinputrequesttypedef)
  - [DescribeTapesOutputTypeDef](#describetapesoutputtypedef)
  - [DescribeUploadBufferInputRequestTypeDef](#describeuploadbufferinputrequesttypedef)
  - [DescribeUploadBufferOutputTypeDef](#describeuploadbufferoutputtypedef)
  - [DescribeVTLDevicesInputRequestTypeDef](#describevtldevicesinputrequesttypedef)
  - [DescribeVTLDevicesOutputTypeDef](#describevtldevicesoutputtypedef)
  - [DescribeWorkingStorageInputRequestTypeDef](#describeworkingstorageinputrequesttypedef)
  - [DescribeWorkingStorageOutputTypeDef](#describeworkingstorageoutputtypedef)
  - [DetachVolumeInputRequestTypeDef](#detachvolumeinputrequesttypedef)
  - [DetachVolumeOutputTypeDef](#detachvolumeoutputtypedef)
  - [DeviceiSCSIAttributesTypeDef](#deviceiscsiattributestypedef)
  - [DisableGatewayInputRequestTypeDef](#disablegatewayinputrequesttypedef)
  - [DisableGatewayOutputTypeDef](#disablegatewayoutputtypedef)
  - [DisassociateFileSystemInputRequestTypeDef](#disassociatefilesysteminputrequesttypedef)
  - [DisassociateFileSystemOutputTypeDef](#disassociatefilesystemoutputtypedef)
  - [DiskTypeDef](#disktypedef)
  - [EndpointNetworkConfigurationTypeDef](#endpointnetworkconfigurationtypedef)
  - [FileShareInfoTypeDef](#fileshareinfotypedef)
  - [FileSystemAssociationInfoTypeDef](#filesystemassociationinfotypedef)
  - [FileSystemAssociationStatusDetailTypeDef](#filesystemassociationstatusdetailtypedef)
  - [FileSystemAssociationSummaryTypeDef](#filesystemassociationsummarytypedef)
  - [GatewayInfoTypeDef](#gatewayinfotypedef)
  - [JoinDomainInputRequestTypeDef](#joindomaininputrequesttypedef)
  - [JoinDomainOutputTypeDef](#joindomainoutputtypedef)
  - [ListAutomaticTapeCreationPoliciesInputRequestTypeDef](#listautomatictapecreationpoliciesinputrequesttypedef)
  - [ListAutomaticTapeCreationPoliciesOutputTypeDef](#listautomatictapecreationpoliciesoutputtypedef)
  - [ListFileSharesInputRequestTypeDef](#listfilesharesinputrequesttypedef)
  - [ListFileSharesOutputTypeDef](#listfilesharesoutputtypedef)
  - [ListFileSystemAssociationsInputRequestTypeDef](#listfilesystemassociationsinputrequesttypedef)
  - [ListFileSystemAssociationsOutputTypeDef](#listfilesystemassociationsoutputtypedef)
  - [ListGatewaysInputRequestTypeDef](#listgatewaysinputrequesttypedef)
  - [ListGatewaysOutputTypeDef](#listgatewaysoutputtypedef)
  - [ListLocalDisksInputRequestTypeDef](#listlocaldisksinputrequesttypedef)
  - [ListLocalDisksOutputTypeDef](#listlocaldisksoutputtypedef)
  - [ListTagsForResourceInputRequestTypeDef](#listtagsforresourceinputrequesttypedef)
  - [ListTagsForResourceOutputTypeDef](#listtagsforresourceoutputtypedef)
  - [ListTapePoolsInputRequestTypeDef](#listtapepoolsinputrequesttypedef)
  - [ListTapePoolsOutputTypeDef](#listtapepoolsoutputtypedef)
  - [ListTapesInputRequestTypeDef](#listtapesinputrequesttypedef)
  - [ListTapesOutputTypeDef](#listtapesoutputtypedef)
  - [ListVolumeInitiatorsInputRequestTypeDef](#listvolumeinitiatorsinputrequesttypedef)
  - [ListVolumeInitiatorsOutputTypeDef](#listvolumeinitiatorsoutputtypedef)
  - [ListVolumeRecoveryPointsInputRequestTypeDef](#listvolumerecoverypointsinputrequesttypedef)
  - [ListVolumeRecoveryPointsOutputTypeDef](#listvolumerecoverypointsoutputtypedef)
  - [ListVolumesInputRequestTypeDef](#listvolumesinputrequesttypedef)
  - [ListVolumesOutputTypeDef](#listvolumesoutputtypedef)
  - [NFSFileShareDefaultsTypeDef](#nfsfilesharedefaultstypedef)
  - [NFSFileShareInfoTypeDef](#nfsfileshareinfotypedef)
  - [NetworkInterfaceTypeDef](#networkinterfacetypedef)
  - [NotifyWhenUploadedInputRequestTypeDef](#notifywhenuploadedinputrequesttypedef)
  - [NotifyWhenUploadedOutputTypeDef](#notifywhenuploadedoutputtypedef)
  - [PaginatorConfigTypeDef](#paginatorconfigtypedef)
  - [PoolInfoTypeDef](#poolinfotypedef)
  - [RefreshCacheInputRequestTypeDef](#refreshcacheinputrequesttypedef)
  - [RefreshCacheOutputTypeDef](#refreshcacheoutputtypedef)
  - [RemoveTagsFromResourceInputRequestTypeDef](#removetagsfromresourceinputrequesttypedef)
  - [RemoveTagsFromResourceOutputTypeDef](#removetagsfromresourceoutputtypedef)
  - [ResetCacheInputRequestTypeDef](#resetcacheinputrequesttypedef)
  - [ResetCacheOutputTypeDef](#resetcacheoutputtypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [RetrieveTapeArchiveInputRequestTypeDef](#retrievetapearchiveinputrequesttypedef)
  - [RetrieveTapeArchiveOutputTypeDef](#retrievetapearchiveoutputtypedef)
  - [RetrieveTapeRecoveryPointInputRequestTypeDef](#retrievetaperecoverypointinputrequesttypedef)
  - [RetrieveTapeRecoveryPointOutputTypeDef](#retrievetaperecoverypointoutputtypedef)
  - [SMBFileShareInfoTypeDef](#smbfileshareinfotypedef)
  - [SMBLocalGroupsTypeDef](#smblocalgroupstypedef)
  - [SetLocalConsolePasswordInputRequestTypeDef](#setlocalconsolepasswordinputrequesttypedef)
  - [SetLocalConsolePasswordOutputTypeDef](#setlocalconsolepasswordoutputtypedef)
  - [SetSMBGuestPasswordInputRequestTypeDef](#setsmbguestpasswordinputrequesttypedef)
  - [SetSMBGuestPasswordOutputTypeDef](#setsmbguestpasswordoutputtypedef)
  - [ShutdownGatewayInputRequestTypeDef](#shutdowngatewayinputrequesttypedef)
  - [ShutdownGatewayOutputTypeDef](#shutdowngatewayoutputtypedef)
  - [StartAvailabilityMonitorTestInputRequestTypeDef](#startavailabilitymonitortestinputrequesttypedef)
  - [StartAvailabilityMonitorTestOutputTypeDef](#startavailabilitymonitortestoutputtypedef)
  - [StartGatewayInputRequestTypeDef](#startgatewayinputrequesttypedef)
  - [StartGatewayOutputTypeDef](#startgatewayoutputtypedef)
  - [StorediSCSIVolumeTypeDef](#storediscsivolumetypedef)
  - [TagTypeDef](#tagtypedef)
  - [TapeArchiveTypeDef](#tapearchivetypedef)
  - [TapeInfoTypeDef](#tapeinfotypedef)
  - [TapeRecoveryPointInfoTypeDef](#taperecoverypointinfotypedef)
  - [TapeTypeDef](#tapetypedef)
  - [UpdateAutomaticTapeCreationPolicyInputRequestTypeDef](#updateautomatictapecreationpolicyinputrequesttypedef)
  - [UpdateAutomaticTapeCreationPolicyOutputTypeDef](#updateautomatictapecreationpolicyoutputtypedef)
  - [UpdateBandwidthRateLimitInputRequestTypeDef](#updatebandwidthratelimitinputrequesttypedef)
  - [UpdateBandwidthRateLimitOutputTypeDef](#updatebandwidthratelimitoutputtypedef)
  - [UpdateBandwidthRateLimitScheduleInputRequestTypeDef](#updatebandwidthratelimitscheduleinputrequesttypedef)
  - [UpdateBandwidthRateLimitScheduleOutputTypeDef](#updatebandwidthratelimitscheduleoutputtypedef)
  - [UpdateChapCredentialsInputRequestTypeDef](#updatechapcredentialsinputrequesttypedef)
  - [UpdateChapCredentialsOutputTypeDef](#updatechapcredentialsoutputtypedef)
  - [UpdateFileSystemAssociationInputRequestTypeDef](#updatefilesystemassociationinputrequesttypedef)
  - [UpdateFileSystemAssociationOutputTypeDef](#updatefilesystemassociationoutputtypedef)
  - [UpdateGatewayInformationInputRequestTypeDef](#updategatewayinformationinputrequesttypedef)
  - [UpdateGatewayInformationOutputTypeDef](#updategatewayinformationoutputtypedef)
  - [UpdateGatewaySoftwareNowInputRequestTypeDef](#updategatewaysoftwarenowinputrequesttypedef)
  - [UpdateGatewaySoftwareNowOutputTypeDef](#updategatewaysoftwarenowoutputtypedef)
  - [UpdateMaintenanceStartTimeInputRequestTypeDef](#updatemaintenancestarttimeinputrequesttypedef)
  - [UpdateMaintenanceStartTimeOutputTypeDef](#updatemaintenancestarttimeoutputtypedef)
  - [UpdateNFSFileShareInputRequestTypeDef](#updatenfsfileshareinputrequesttypedef)
  - [UpdateNFSFileShareOutputTypeDef](#updatenfsfileshareoutputtypedef)
  - [UpdateSMBFileShareInputRequestTypeDef](#updatesmbfileshareinputrequesttypedef)
  - [UpdateSMBFileShareOutputTypeDef](#updatesmbfileshareoutputtypedef)
  - [UpdateSMBFileShareVisibilityInputRequestTypeDef](#updatesmbfilesharevisibilityinputrequesttypedef)
  - [UpdateSMBFileShareVisibilityOutputTypeDef](#updatesmbfilesharevisibilityoutputtypedef)
  - [UpdateSMBLocalGroupsInputRequestTypeDef](#updatesmblocalgroupsinputrequesttypedef)
  - [UpdateSMBLocalGroupsOutputTypeDef](#updatesmblocalgroupsoutputtypedef)
  - [UpdateSMBSecurityStrategyInputRequestTypeDef](#updatesmbsecuritystrategyinputrequesttypedef)
  - [UpdateSMBSecurityStrategyOutputTypeDef](#updatesmbsecuritystrategyoutputtypedef)
  - [UpdateSnapshotScheduleInputRequestTypeDef](#updatesnapshotscheduleinputrequesttypedef)
  - [UpdateSnapshotScheduleOutputTypeDef](#updatesnapshotscheduleoutputtypedef)
  - [UpdateVTLDeviceTypeInputRequestTypeDef](#updatevtldevicetypeinputrequesttypedef)
  - [UpdateVTLDeviceTypeOutputTypeDef](#updatevtldevicetypeoutputtypedef)
  - [VTLDeviceTypeDef](#vtldevicetypedef)
  - [VolumeInfoTypeDef](#volumeinfotypedef)
  - [VolumeRecoveryPointInfoTypeDef](#volumerecoverypointinfotypedef)
  - [VolumeiSCSIAttributesTypeDef](#volumeiscsiattributestypedef)

<a id="activategatewayinputrequesttypedef"></a>

## ActivateGatewayInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ActivateGatewayInputRequestTypeDef
```

Required fields:

- `ActivationKey`: `str`
- `GatewayName`: `str`
- `GatewayTimezone`: `str`
- `GatewayRegion`: `str`

Optional fields:

- `GatewayType`: `str`
- `TapeDriveType`: `str`
- `MediumChangerType`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="activategatewayoutputtypedef"></a>

## ActivateGatewayOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ActivateGatewayOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="addcacheinputrequesttypedef"></a>

## AddCacheInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AddCacheInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `DiskIds`: `Sequence`\[`str`\]

<a id="addcacheoutputtypedef"></a>

## AddCacheOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AddCacheOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="addtagstoresourceinputrequesttypedef"></a>

## AddTagsToResourceInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AddTagsToResourceInputRequestTypeDef
```

Required fields:

- `ResourceARN`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="addtagstoresourceoutputtypedef"></a>

## AddTagsToResourceOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AddTagsToResourceOutputTypeDef
```

Required fields:

- `ResourceARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="adduploadbufferinputrequesttypedef"></a>

## AddUploadBufferInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AddUploadBufferInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `DiskIds`: `Sequence`\[`str`\]

<a id="adduploadbufferoutputtypedef"></a>

## AddUploadBufferOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AddUploadBufferOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="addworkingstorageinputrequesttypedef"></a>

## AddWorkingStorageInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AddWorkingStorageInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `DiskIds`: `Sequence`\[`str`\]

<a id="addworkingstorageoutputtypedef"></a>

## AddWorkingStorageOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AddWorkingStorageOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="assigntapepoolinputrequesttypedef"></a>

## AssignTapePoolInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AssignTapePoolInputRequestTypeDef
```

Required fields:

- `TapeARN`: `str`
- `PoolId`: `str`

Optional fields:

- `BypassGovernanceRetention`: `bool`

<a id="assigntapepooloutputtypedef"></a>

## AssignTapePoolOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AssignTapePoolOutputTypeDef
```

Required fields:

- `TapeARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="associatefilesysteminputrequesttypedef"></a>

## AssociateFileSystemInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AssociateFileSystemInputRequestTypeDef
```

Required fields:

- `UserName`: `str`
- `Password`: `str`
- `ClientToken`: `str`
- `GatewayARN`: `str`
- `LocationARN`: `str`

Optional fields:

- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `AuditDestinationARN`: `str`
- `CacheAttributes`:
  [CacheAttributesTypeDef](./type_defs.md#cacheattributestypedef)
- `EndpointNetworkConfiguration`:
  [EndpointNetworkConfigurationTypeDef](./type_defs.md#endpointnetworkconfigurationtypedef)

<a id="associatefilesystemoutputtypedef"></a>

## AssociateFileSystemOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AssociateFileSystemOutputTypeDef
```

Required fields:

- `FileSystemAssociationARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="attachvolumeinputrequesttypedef"></a>

## AttachVolumeInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AttachVolumeInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `VolumeARN`: `str`
- `NetworkInterfaceId`: `str`

Optional fields:

- `TargetName`: `str`
- `DiskId`: `str`

<a id="attachvolumeoutputtypedef"></a>

## AttachVolumeOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AttachVolumeOutputTypeDef
```

Required fields:

- `VolumeARN`: `str`
- `TargetARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="automatictapecreationpolicyinfotypedef"></a>

## AutomaticTapeCreationPolicyInfoTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AutomaticTapeCreationPolicyInfoTypeDef
```

Optional fields:

- `AutomaticTapeCreationRules`:
  `List`\[[AutomaticTapeCreationRuleTypeDef](./type_defs.md#automatictapecreationruletypedef)\]
- `GatewayARN`: `str`

<a id="automatictapecreationruletypedef"></a>

## AutomaticTapeCreationRuleTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import AutomaticTapeCreationRuleTypeDef
```

Required fields:

- `TapeBarcodePrefix`: `str`
- `PoolId`: `str`
- `TapeSizeInBytes`: `int`
- `MinimumNumTapes`: `int`

Optional fields:

- `Worm`: `bool`

<a id="bandwidthratelimitintervaltypedef"></a>

## BandwidthRateLimitIntervalTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import BandwidthRateLimitIntervalTypeDef
```

Required fields:

- `StartHourOfDay`: `int`
- `StartMinuteOfHour`: `int`
- `EndHourOfDay`: `int`
- `EndMinuteOfHour`: `int`
- `DaysOfWeek`: `List`\[`int`\]

Optional fields:

- `AverageUploadRateLimitInBitsPerSec`: `int`
- `AverageDownloadRateLimitInBitsPerSec`: `int`

<a id="cacheattributestypedef"></a>

## CacheAttributesTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CacheAttributesTypeDef
```

Optional fields:

- `CacheStaleTimeoutInSeconds`: `int`

<a id="cachediscsivolumetypedef"></a>

## CachediSCSIVolumeTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CachediSCSIVolumeTypeDef
```

Optional fields:

- `VolumeARN`: `str`
- `VolumeId`: `str`
- `VolumeType`: `str`
- `VolumeStatus`: `str`
- `VolumeAttachmentStatus`: `str`
- `VolumeSizeInBytes`: `int`
- `VolumeProgress`: `float`
- `SourceSnapshotId`: `str`
- `VolumeiSCSIAttributes`:
  [VolumeiSCSIAttributesTypeDef](./type_defs.md#volumeiscsiattributestypedef)
- `CreatedDate`: `datetime`
- `VolumeUsedInBytes`: `int`
- `KMSKey`: `str`
- `TargetName`: `str`

<a id="cancelarchivalinputrequesttypedef"></a>

## CancelArchivalInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CancelArchivalInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `TapeARN`: `str`

<a id="cancelarchivaloutputtypedef"></a>

## CancelArchivalOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CancelArchivalOutputTypeDef
```

Required fields:

- `TapeARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="cancelretrievalinputrequesttypedef"></a>

## CancelRetrievalInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CancelRetrievalInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `TapeARN`: `str`

<a id="cancelretrievaloutputtypedef"></a>

## CancelRetrievalOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CancelRetrievalOutputTypeDef
```

Required fields:

- `TapeARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="chapinfotypedef"></a>

## ChapInfoTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ChapInfoTypeDef
```

Optional fields:

- `TargetARN`: `str`
- `SecretToAuthenticateInitiator`: `str`
- `InitiatorName`: `str`
- `SecretToAuthenticateTarget`: `str`

<a id="createcachediscsivolumeinputrequesttypedef"></a>

## CreateCachediSCSIVolumeInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateCachediSCSIVolumeInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `VolumeSizeInBytes`: `int`
- `TargetName`: `str`
- `NetworkInterfaceId`: `str`
- `ClientToken`: `str`

Optional fields:

- `SnapshotId`: `str`
- `SourceVolumeARN`: `str`
- `KMSEncrypted`: `bool`
- `KMSKey`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="createcachediscsivolumeoutputtypedef"></a>

## CreateCachediSCSIVolumeOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateCachediSCSIVolumeOutputTypeDef
```

Required fields:

- `VolumeARN`: `str`
- `TargetARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createnfsfileshareinputrequesttypedef"></a>

## CreateNFSFileShareInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateNFSFileShareInputRequestTypeDef
```

Required fields:

- `ClientToken`: `str`
- `GatewayARN`: `str`
- `Role`: `str`
- `LocationARN`: `str`

Optional fields:

- `NFSFileShareDefaults`:
  [NFSFileShareDefaultsTypeDef](./type_defs.md#nfsfilesharedefaultstypedef)
- `KMSEncrypted`: `bool`
- `KMSKey`: `str`
- `DefaultStorageClass`: `str`
- `ObjectACL`: [ObjectACLType](./literals.md#objectacltype)
- `ClientList`: `Sequence`\[`str`\]
- `Squash`: `str`
- `ReadOnly`: `bool`
- `GuessMIMETypeEnabled`: `bool`
- `RequesterPays`: `bool`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `FileShareName`: `str`
- `CacheAttributes`:
  [CacheAttributesTypeDef](./type_defs.md#cacheattributestypedef)
- `NotificationPolicy`: `str`
- `VPCEndpointDNSName`: `str`
- `BucketRegion`: `str`
- `AuditDestinationARN`: `str`

<a id="createnfsfileshareoutputtypedef"></a>

## CreateNFSFileShareOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateNFSFileShareOutputTypeDef
```

Required fields:

- `FileShareARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createsmbfileshareinputrequesttypedef"></a>

## CreateSMBFileShareInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateSMBFileShareInputRequestTypeDef
```

Required fields:

- `ClientToken`: `str`
- `GatewayARN`: `str`
- `Role`: `str`
- `LocationARN`: `str`

Optional fields:

- `KMSEncrypted`: `bool`
- `KMSKey`: `str`
- `DefaultStorageClass`: `str`
- `ObjectACL`: [ObjectACLType](./literals.md#objectacltype)
- `ReadOnly`: `bool`
- `GuessMIMETypeEnabled`: `bool`
- `RequesterPays`: `bool`
- `SMBACLEnabled`: `bool`
- `AccessBasedEnumeration`: `bool`
- `AdminUserList`: `Sequence`\[`str`\]
- `ValidUserList`: `Sequence`\[`str`\]
- `InvalidUserList`: `Sequence`\[`str`\]
- `AuditDestinationARN`: `str`
- `Authentication`: `str`
- `CaseSensitivity`: [CaseSensitivityType](./literals.md#casesensitivitytype)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `FileShareName`: `str`
- `CacheAttributes`:
  [CacheAttributesTypeDef](./type_defs.md#cacheattributestypedef)
- `NotificationPolicy`: `str`
- `VPCEndpointDNSName`: `str`
- `BucketRegion`: `str`
- `OplocksEnabled`: `bool`

<a id="createsmbfileshareoutputtypedef"></a>

## CreateSMBFileShareOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateSMBFileShareOutputTypeDef
```

Required fields:

- `FileShareARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createsnapshotfromvolumerecoverypointinputrequesttypedef"></a>

## CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef
```

Required fields:

- `VolumeARN`: `str`
- `SnapshotDescription`: `str`

Optional fields:

- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="createsnapshotfromvolumerecoverypointoutputtypedef"></a>

## CreateSnapshotFromVolumeRecoveryPointOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateSnapshotFromVolumeRecoveryPointOutputTypeDef
```

Required fields:

- `SnapshotId`: `str`
- `VolumeARN`: `str`
- `VolumeRecoveryPointTime`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createsnapshotinputrequesttypedef"></a>

## CreateSnapshotInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateSnapshotInputRequestTypeDef
```

Required fields:

- `VolumeARN`: `str`
- `SnapshotDescription`: `str`

Optional fields:

- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="createsnapshotoutputtypedef"></a>

## CreateSnapshotOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateSnapshotOutputTypeDef
```

Required fields:

- `VolumeARN`: `str`
- `SnapshotId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createstorediscsivolumeinputrequesttypedef"></a>

## CreateStorediSCSIVolumeInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateStorediSCSIVolumeInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `DiskId`: `str`
- `PreserveExistingData`: `bool`
- `TargetName`: `str`
- `NetworkInterfaceId`: `str`

Optional fields:

- `SnapshotId`: `str`
- `KMSEncrypted`: `bool`
- `KMSKey`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="createstorediscsivolumeoutputtypedef"></a>

## CreateStorediSCSIVolumeOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateStorediSCSIVolumeOutputTypeDef
```

Required fields:

- `VolumeARN`: `str`
- `VolumeSizeInBytes`: `int`
- `TargetARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createtapepoolinputrequesttypedef"></a>

## CreateTapePoolInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateTapePoolInputRequestTypeDef
```

Required fields:

- `PoolName`: `str`
- `StorageClass`: [TapeStorageClassType](./literals.md#tapestorageclasstype)

Optional fields:

- `RetentionLockType`:
  [RetentionLockTypeType](./literals.md#retentionlocktypetype)
- `RetentionLockTimeInDays`: `int`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="createtapepooloutputtypedef"></a>

## CreateTapePoolOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateTapePoolOutputTypeDef
```

Required fields:

- `PoolARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createtapewithbarcodeinputrequesttypedef"></a>

## CreateTapeWithBarcodeInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateTapeWithBarcodeInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `TapeSizeInBytes`: `int`
- `TapeBarcode`: `str`

Optional fields:

- `KMSEncrypted`: `bool`
- `KMSKey`: `str`
- `PoolId`: `str`
- `Worm`: `bool`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="createtapewithbarcodeoutputtypedef"></a>

## CreateTapeWithBarcodeOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateTapeWithBarcodeOutputTypeDef
```

Required fields:

- `TapeARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createtapesinputrequesttypedef"></a>

## CreateTapesInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateTapesInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `TapeSizeInBytes`: `int`
- `ClientToken`: `str`
- `NumTapesToCreate`: `int`
- `TapeBarcodePrefix`: `str`

Optional fields:

- `KMSEncrypted`: `bool`
- `KMSKey`: `str`
- `PoolId`: `str`
- `Worm`: `bool`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="createtapesoutputtypedef"></a>

## CreateTapesOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import CreateTapesOutputTypeDef
```

Required fields:

- `TapeARNs`: `List`\[`str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deleteautomatictapecreationpolicyinputrequesttypedef"></a>

## DeleteAutomaticTapeCreationPolicyInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteAutomaticTapeCreationPolicyInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="deleteautomatictapecreationpolicyoutputtypedef"></a>

## DeleteAutomaticTapeCreationPolicyOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteAutomaticTapeCreationPolicyOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deletebandwidthratelimitinputrequesttypedef"></a>

## DeleteBandwidthRateLimitInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteBandwidthRateLimitInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `BandwidthType`: `str`

<a id="deletebandwidthratelimitoutputtypedef"></a>

## DeleteBandwidthRateLimitOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteBandwidthRateLimitOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deletechapcredentialsinputrequesttypedef"></a>

## DeleteChapCredentialsInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteChapCredentialsInputRequestTypeDef
```

Required fields:

- `TargetARN`: `str`
- `InitiatorName`: `str`

<a id="deletechapcredentialsoutputtypedef"></a>

## DeleteChapCredentialsOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteChapCredentialsOutputTypeDef
```

Required fields:

- `TargetARN`: `str`
- `InitiatorName`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deletefileshareinputrequesttypedef"></a>

## DeleteFileShareInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteFileShareInputRequestTypeDef
```

Required fields:

- `FileShareARN`: `str`

Optional fields:

- `ForceDelete`: `bool`

<a id="deletefileshareoutputtypedef"></a>

## DeleteFileShareOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteFileShareOutputTypeDef
```

Required fields:

- `FileShareARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deletegatewayinputrequesttypedef"></a>

## DeleteGatewayInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteGatewayInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="deletegatewayoutputtypedef"></a>

## DeleteGatewayOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteGatewayOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deletesnapshotscheduleinputrequesttypedef"></a>

## DeleteSnapshotScheduleInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteSnapshotScheduleInputRequestTypeDef
```

Required fields:

- `VolumeARN`: `str`

<a id="deletesnapshotscheduleoutputtypedef"></a>

## DeleteSnapshotScheduleOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteSnapshotScheduleOutputTypeDef
```

Required fields:

- `VolumeARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deletetapearchiveinputrequesttypedef"></a>

## DeleteTapeArchiveInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteTapeArchiveInputRequestTypeDef
```

Required fields:

- `TapeARN`: `str`

Optional fields:

- `BypassGovernanceRetention`: `bool`

<a id="deletetapearchiveoutputtypedef"></a>

## DeleteTapeArchiveOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteTapeArchiveOutputTypeDef
```

Required fields:

- `TapeARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deletetapeinputrequesttypedef"></a>

## DeleteTapeInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteTapeInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `TapeARN`: `str`

Optional fields:

- `BypassGovernanceRetention`: `bool`

<a id="deletetapeoutputtypedef"></a>

## DeleteTapeOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteTapeOutputTypeDef
```

Required fields:

- `TapeARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deletetapepoolinputrequesttypedef"></a>

## DeleteTapePoolInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteTapePoolInputRequestTypeDef
```

Required fields:

- `PoolARN`: `str`

<a id="deletetapepooloutputtypedef"></a>

## DeleteTapePoolOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteTapePoolOutputTypeDef
```

Required fields:

- `PoolARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deletevolumeinputrequesttypedef"></a>

## DeleteVolumeInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteVolumeInputRequestTypeDef
```

Required fields:

- `VolumeARN`: `str`

<a id="deletevolumeoutputtypedef"></a>

## DeleteVolumeOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeleteVolumeOutputTypeDef
```

Required fields:

- `VolumeARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describeavailabilitymonitortestinputrequesttypedef"></a>

## DescribeAvailabilityMonitorTestInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeAvailabilityMonitorTestInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="describeavailabilitymonitortestoutputtypedef"></a>

## DescribeAvailabilityMonitorTestOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeAvailabilityMonitorTestOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `Status`:
  [AvailabilityMonitorTestStatusType](./literals.md#availabilitymonitorteststatustype)
- `StartTime`: `datetime`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describebandwidthratelimitinputrequesttypedef"></a>

## DescribeBandwidthRateLimitInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeBandwidthRateLimitInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="describebandwidthratelimitoutputtypedef"></a>

## DescribeBandwidthRateLimitOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeBandwidthRateLimitOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `AverageUploadRateLimitInBitsPerSec`: `int`
- `AverageDownloadRateLimitInBitsPerSec`: `int`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describebandwidthratelimitscheduleinputrequesttypedef"></a>

## DescribeBandwidthRateLimitScheduleInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeBandwidthRateLimitScheduleInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="describebandwidthratelimitscheduleoutputtypedef"></a>

## DescribeBandwidthRateLimitScheduleOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeBandwidthRateLimitScheduleOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `BandwidthRateLimitIntervals`:
  `List`\[[BandwidthRateLimitIntervalTypeDef](./type_defs.md#bandwidthratelimitintervaltypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describecacheinputrequesttypedef"></a>

## DescribeCacheInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeCacheInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="describecacheoutputtypedef"></a>

## DescribeCacheOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeCacheOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `DiskIds`: `List`\[`str`\]
- `CacheAllocatedInBytes`: `int`
- `CacheUsedPercentage`: `float`
- `CacheDirtyPercentage`: `float`
- `CacheHitPercentage`: `float`
- `CacheMissPercentage`: `float`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describecachediscsivolumesinputrequesttypedef"></a>

## DescribeCachediSCSIVolumesInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeCachediSCSIVolumesInputRequestTypeDef
```

Required fields:

- `VolumeARNs`: `Sequence`\[`str`\]

<a id="describecachediscsivolumesoutputtypedef"></a>

## DescribeCachediSCSIVolumesOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeCachediSCSIVolumesOutputTypeDef
```

Required fields:

- `CachediSCSIVolumes`:
  `List`\[[CachediSCSIVolumeTypeDef](./type_defs.md#cachediscsivolumetypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describechapcredentialsinputrequesttypedef"></a>

## DescribeChapCredentialsInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeChapCredentialsInputRequestTypeDef
```

Required fields:

- `TargetARN`: `str`

<a id="describechapcredentialsoutputtypedef"></a>

## DescribeChapCredentialsOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeChapCredentialsOutputTypeDef
```

Required fields:

- `ChapCredentials`:
  `List`\[[ChapInfoTypeDef](./type_defs.md#chapinfotypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describefilesystemassociationsinputrequesttypedef"></a>

## DescribeFileSystemAssociationsInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeFileSystemAssociationsInputRequestTypeDef
```

Required fields:

- `FileSystemAssociationARNList`: `Sequence`\[`str`\]

<a id="describefilesystemassociationsoutputtypedef"></a>

## DescribeFileSystemAssociationsOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeFileSystemAssociationsOutputTypeDef
```

Required fields:

- `FileSystemAssociationInfoList`:
  `List`\[[FileSystemAssociationInfoTypeDef](./type_defs.md#filesystemassociationinfotypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describegatewayinformationinputrequesttypedef"></a>

## DescribeGatewayInformationInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeGatewayInformationInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="describegatewayinformationoutputtypedef"></a>

## DescribeGatewayInformationOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeGatewayInformationOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `GatewayId`: `str`
- `GatewayName`: `str`
- `GatewayTimezone`: `str`
- `GatewayState`: `str`
- `GatewayNetworkInterfaces`:
  `List`\[[NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef)\]
- `GatewayType`: `str`
- `NextUpdateAvailabilityDate`: `str`
- `LastSoftwareUpdate`: `str`
- `Ec2InstanceId`: `str`
- `Ec2InstanceRegion`: `str`
- `Tags`: `List`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `VPCEndpoint`: `str`
- `CloudWatchLogGroupARN`: `str`
- `HostEnvironment`: [HostEnvironmentType](./literals.md#hostenvironmenttype)
- `EndpointType`: `str`
- `SoftwareUpdatesEndDate`: `str`
- `DeprecationDate`: `str`
- `GatewayCapacity`: [GatewayCapacityType](./literals.md#gatewaycapacitytype)
- `SupportedGatewayCapacities`:
  `List`\[[GatewayCapacityType](./literals.md#gatewaycapacitytype)\]
- `HostEnvironmentId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describemaintenancestarttimeinputrequesttypedef"></a>

## DescribeMaintenanceStartTimeInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeMaintenanceStartTimeInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="describemaintenancestarttimeoutputtypedef"></a>

## DescribeMaintenanceStartTimeOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeMaintenanceStartTimeOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `HourOfDay`: `int`
- `MinuteOfHour`: `int`
- `DayOfWeek`: `int`
- `DayOfMonth`: `int`
- `Timezone`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describenfsfilesharesinputrequesttypedef"></a>

## DescribeNFSFileSharesInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeNFSFileSharesInputRequestTypeDef
```

Required fields:

- `FileShareARNList`: `Sequence`\[`str`\]

<a id="describenfsfilesharesoutputtypedef"></a>

## DescribeNFSFileSharesOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeNFSFileSharesOutputTypeDef
```

Required fields:

- `NFSFileShareInfoList`:
  `List`\[[NFSFileShareInfoTypeDef](./type_defs.md#nfsfileshareinfotypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describesmbfilesharesinputrequesttypedef"></a>

## DescribeSMBFileSharesInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeSMBFileSharesInputRequestTypeDef
```

Required fields:

- `FileShareARNList`: `Sequence`\[`str`\]

<a id="describesmbfilesharesoutputtypedef"></a>

## DescribeSMBFileSharesOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeSMBFileSharesOutputTypeDef
```

Required fields:

- `SMBFileShareInfoList`:
  `List`\[[SMBFileShareInfoTypeDef](./type_defs.md#smbfileshareinfotypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describesmbsettingsinputrequesttypedef"></a>

## DescribeSMBSettingsInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeSMBSettingsInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="describesmbsettingsoutputtypedef"></a>

## DescribeSMBSettingsOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeSMBSettingsOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `DomainName`: `str`
- `ActiveDirectoryStatus`:
  [ActiveDirectoryStatusType](./literals.md#activedirectorystatustype)
- `SMBGuestPasswordSet`: `bool`
- `SMBSecurityStrategy`:
  [SMBSecurityStrategyType](./literals.md#smbsecuritystrategytype)
- `FileSharesVisible`: `bool`
- `SMBLocalGroups`:
  [SMBLocalGroupsTypeDef](./type_defs.md#smblocalgroupstypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describesnapshotscheduleinputrequesttypedef"></a>

## DescribeSnapshotScheduleInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeSnapshotScheduleInputRequestTypeDef
```

Required fields:

- `VolumeARN`: `str`

<a id="describesnapshotscheduleoutputtypedef"></a>

## DescribeSnapshotScheduleOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeSnapshotScheduleOutputTypeDef
```

Required fields:

- `VolumeARN`: `str`
- `StartAt`: `int`
- `RecurrenceInHours`: `int`
- `Description`: `str`
- `Timezone`: `str`
- `Tags`: `List`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describestorediscsivolumesinputrequesttypedef"></a>

## DescribeStorediSCSIVolumesInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeStorediSCSIVolumesInputRequestTypeDef
```

Required fields:

- `VolumeARNs`: `Sequence`\[`str`\]

<a id="describestorediscsivolumesoutputtypedef"></a>

## DescribeStorediSCSIVolumesOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeStorediSCSIVolumesOutputTypeDef
```

Required fields:

- `StorediSCSIVolumes`:
  `List`\[[StorediSCSIVolumeTypeDef](./type_defs.md#storediscsivolumetypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describetapearchivesinputrequesttypedef"></a>

## DescribeTapeArchivesInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeTapeArchivesInputRequestTypeDef
```

Optional fields:

- `TapeARNs`: `Sequence`\[`str`\]
- `Marker`: `str`
- `Limit`: `int`

<a id="describetapearchivesoutputtypedef"></a>

## DescribeTapeArchivesOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeTapeArchivesOutputTypeDef
```

Required fields:

- `TapeArchives`:
  `List`\[[TapeArchiveTypeDef](./type_defs.md#tapearchivetypedef)\]
- `Marker`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describetaperecoverypointsinputrequesttypedef"></a>

## DescribeTapeRecoveryPointsInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeTapeRecoveryPointsInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

Optional fields:

- `Marker`: `str`
- `Limit`: `int`

<a id="describetaperecoverypointsoutputtypedef"></a>

## DescribeTapeRecoveryPointsOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeTapeRecoveryPointsOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `TapeRecoveryPointInfos`:
  `List`\[[TapeRecoveryPointInfoTypeDef](./type_defs.md#taperecoverypointinfotypedef)\]
- `Marker`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describetapesinputrequesttypedef"></a>

## DescribeTapesInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeTapesInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

Optional fields:

- `TapeARNs`: `Sequence`\[`str`\]
- `Marker`: `str`
- `Limit`: `int`

<a id="describetapesoutputtypedef"></a>

## DescribeTapesOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeTapesOutputTypeDef
```

Required fields:

- `Tapes`: `List`\[[TapeTypeDef](./type_defs.md#tapetypedef)\]
- `Marker`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describeuploadbufferinputrequesttypedef"></a>

## DescribeUploadBufferInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeUploadBufferInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="describeuploadbufferoutputtypedef"></a>

## DescribeUploadBufferOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeUploadBufferOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `DiskIds`: `List`\[`str`\]
- `UploadBufferUsedInBytes`: `int`
- `UploadBufferAllocatedInBytes`: `int`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describevtldevicesinputrequesttypedef"></a>

## DescribeVTLDevicesInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeVTLDevicesInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

Optional fields:

- `VTLDeviceARNs`: `Sequence`\[`str`\]
- `Marker`: `str`
- `Limit`: `int`

<a id="describevtldevicesoutputtypedef"></a>

## DescribeVTLDevicesOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeVTLDevicesOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `VTLDevices`: `List`\[[VTLDeviceTypeDef](./type_defs.md#vtldevicetypedef)\]
- `Marker`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describeworkingstorageinputrequesttypedef"></a>

## DescribeWorkingStorageInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeWorkingStorageInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="describeworkingstorageoutputtypedef"></a>

## DescribeWorkingStorageOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DescribeWorkingStorageOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `DiskIds`: `List`\[`str`\]
- `WorkingStorageUsedInBytes`: `int`
- `WorkingStorageAllocatedInBytes`: `int`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="detachvolumeinputrequesttypedef"></a>

## DetachVolumeInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DetachVolumeInputRequestTypeDef
```

Required fields:

- `VolumeARN`: `str`

Optional fields:

- `ForceDetach`: `bool`

<a id="detachvolumeoutputtypedef"></a>

## DetachVolumeOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DetachVolumeOutputTypeDef
```

Required fields:

- `VolumeARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deviceiscsiattributestypedef"></a>

## DeviceiSCSIAttributesTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DeviceiSCSIAttributesTypeDef
```

Optional fields:

- `TargetARN`: `str`
- `NetworkInterfaceId`: `str`
- `NetworkInterfacePort`: `int`
- `ChapEnabled`: `bool`

<a id="disablegatewayinputrequesttypedef"></a>

## DisableGatewayInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DisableGatewayInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="disablegatewayoutputtypedef"></a>

## DisableGatewayOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DisableGatewayOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="disassociatefilesysteminputrequesttypedef"></a>

## DisassociateFileSystemInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DisassociateFileSystemInputRequestTypeDef
```

Required fields:

- `FileSystemAssociationARN`: `str`

Optional fields:

- `ForceDelete`: `bool`

<a id="disassociatefilesystemoutputtypedef"></a>

## DisassociateFileSystemOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DisassociateFileSystemOutputTypeDef
```

Required fields:

- `FileSystemAssociationARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="disktypedef"></a>

## DiskTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import DiskTypeDef
```

Optional fields:

- `DiskId`: `str`
- `DiskPath`: `str`
- `DiskNode`: `str`
- `DiskStatus`: `str`
- `DiskSizeInBytes`: `int`
- `DiskAllocationType`: `str`
- `DiskAllocationResource`: `str`
- `DiskAttributeList`: `List`\[`str`\]

<a id="endpointnetworkconfigurationtypedef"></a>

## EndpointNetworkConfigurationTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import EndpointNetworkConfigurationTypeDef
```

Optional fields:

- `IpAddresses`: `Sequence`\[`str`\]

<a id="fileshareinfotypedef"></a>

## FileShareInfoTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import FileShareInfoTypeDef
```

Optional fields:

- `FileShareType`: [FileShareTypeType](./literals.md#filesharetypetype)
- `FileShareARN`: `str`
- `FileShareId`: `str`
- `FileShareStatus`: `str`
- `GatewayARN`: `str`

<a id="filesystemassociationinfotypedef"></a>

## FileSystemAssociationInfoTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import FileSystemAssociationInfoTypeDef
```

Optional fields:

- `FileSystemAssociationARN`: `str`
- `LocationARN`: `str`
- `FileSystemAssociationStatus`: `str`
- `AuditDestinationARN`: `str`
- `GatewayARN`: `str`
- `Tags`: `List`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `CacheAttributes`:
  [CacheAttributesTypeDef](./type_defs.md#cacheattributestypedef)
- `EndpointNetworkConfiguration`:
  [EndpointNetworkConfigurationTypeDef](./type_defs.md#endpointnetworkconfigurationtypedef)
- `FileSystemAssociationStatusDetails`:
  `List`\[[FileSystemAssociationStatusDetailTypeDef](./type_defs.md#filesystemassociationstatusdetailtypedef)\]

<a id="filesystemassociationstatusdetailtypedef"></a>

## FileSystemAssociationStatusDetailTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import FileSystemAssociationStatusDetailTypeDef
```

Optional fields:

- `ErrorCode`: `str`

<a id="filesystemassociationsummarytypedef"></a>

## FileSystemAssociationSummaryTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import FileSystemAssociationSummaryTypeDef
```

Optional fields:

- `FileSystemAssociationId`: `str`
- `FileSystemAssociationARN`: `str`
- `FileSystemAssociationStatus`: `str`
- `GatewayARN`: `str`

<a id="gatewayinfotypedef"></a>

## GatewayInfoTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import GatewayInfoTypeDef
```

Optional fields:

- `GatewayId`: `str`
- `GatewayARN`: `str`
- `GatewayType`: `str`
- `GatewayOperationalState`: `str`
- `GatewayName`: `str`
- `Ec2InstanceId`: `str`
- `Ec2InstanceRegion`: `str`
- `HostEnvironment`: [HostEnvironmentType](./literals.md#hostenvironmenttype)
- `HostEnvironmentId`: `str`

<a id="joindomaininputrequesttypedef"></a>

## JoinDomainInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import JoinDomainInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `DomainName`: `str`
- `UserName`: `str`
- `Password`: `str`

Optional fields:

- `OrganizationalUnit`: `str`
- `DomainControllers`: `Sequence`\[`str`\]
- `TimeoutInSeconds`: `int`

<a id="joindomainoutputtypedef"></a>

## JoinDomainOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import JoinDomainOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ActiveDirectoryStatus`:
  [ActiveDirectoryStatusType](./literals.md#activedirectorystatustype)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listautomatictapecreationpoliciesinputrequesttypedef"></a>

## ListAutomaticTapeCreationPoliciesInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListAutomaticTapeCreationPoliciesInputRequestTypeDef
```

Optional fields:

- `GatewayARN`: `str`

<a id="listautomatictapecreationpoliciesoutputtypedef"></a>

## ListAutomaticTapeCreationPoliciesOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListAutomaticTapeCreationPoliciesOutputTypeDef
```

Required fields:

- `AutomaticTapeCreationPolicyInfos`:
  `List`\[[AutomaticTapeCreationPolicyInfoTypeDef](./type_defs.md#automatictapecreationpolicyinfotypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listfilesharesinputrequesttypedef"></a>

## ListFileSharesInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListFileSharesInputRequestTypeDef
```

Optional fields:

- `GatewayARN`: `str`
- `Limit`: `int`
- `Marker`: `str`

<a id="listfilesharesoutputtypedef"></a>

## ListFileSharesOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListFileSharesOutputTypeDef
```

Required fields:

- `Marker`: `str`
- `NextMarker`: `str`
- `FileShareInfoList`:
  `List`\[[FileShareInfoTypeDef](./type_defs.md#fileshareinfotypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listfilesystemassociationsinputrequesttypedef"></a>

## ListFileSystemAssociationsInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListFileSystemAssociationsInputRequestTypeDef
```

Optional fields:

- `GatewayARN`: `str`
- `Limit`: `int`
- `Marker`: `str`

<a id="listfilesystemassociationsoutputtypedef"></a>

## ListFileSystemAssociationsOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListFileSystemAssociationsOutputTypeDef
```

Required fields:

- `Marker`: `str`
- `NextMarker`: `str`
- `FileSystemAssociationSummaryList`:
  `List`\[[FileSystemAssociationSummaryTypeDef](./type_defs.md#filesystemassociationsummarytypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listgatewaysinputrequesttypedef"></a>

## ListGatewaysInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListGatewaysInputRequestTypeDef
```

Optional fields:

- `Marker`: `str`
- `Limit`: `int`

<a id="listgatewaysoutputtypedef"></a>

## ListGatewaysOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListGatewaysOutputTypeDef
```

Required fields:

- `Gateways`: `List`\[[GatewayInfoTypeDef](./type_defs.md#gatewayinfotypedef)\]
- `Marker`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listlocaldisksinputrequesttypedef"></a>

## ListLocalDisksInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListLocalDisksInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="listlocaldisksoutputtypedef"></a>

## ListLocalDisksOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListLocalDisksOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `Disks`: `List`\[[DiskTypeDef](./type_defs.md#disktypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtagsforresourceinputrequesttypedef"></a>

## ListTagsForResourceInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListTagsForResourceInputRequestTypeDef
```

Required fields:

- `ResourceARN`: `str`

Optional fields:

- `Marker`: `str`
- `Limit`: `int`

<a id="listtagsforresourceoutputtypedef"></a>

## ListTagsForResourceOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListTagsForResourceOutputTypeDef
```

Required fields:

- `ResourceARN`: `str`
- `Marker`: `str`
- `Tags`: `List`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtapepoolsinputrequesttypedef"></a>

## ListTapePoolsInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListTapePoolsInputRequestTypeDef
```

Optional fields:

- `PoolARNs`: `Sequence`\[`str`\]
- `Marker`: `str`
- `Limit`: `int`

<a id="listtapepoolsoutputtypedef"></a>

## ListTapePoolsOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListTapePoolsOutputTypeDef
```

Required fields:

- `PoolInfos`: `List`\[[PoolInfoTypeDef](./type_defs.md#poolinfotypedef)\]
- `Marker`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtapesinputrequesttypedef"></a>

## ListTapesInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListTapesInputRequestTypeDef
```

Optional fields:

- `TapeARNs`: `Sequence`\[`str`\]
- `Marker`: `str`
- `Limit`: `int`

<a id="listtapesoutputtypedef"></a>

## ListTapesOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListTapesOutputTypeDef
```

Required fields:

- `TapeInfos`: `List`\[[TapeInfoTypeDef](./type_defs.md#tapeinfotypedef)\]
- `Marker`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listvolumeinitiatorsinputrequesttypedef"></a>

## ListVolumeInitiatorsInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListVolumeInitiatorsInputRequestTypeDef
```

Required fields:

- `VolumeARN`: `str`

<a id="listvolumeinitiatorsoutputtypedef"></a>

## ListVolumeInitiatorsOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListVolumeInitiatorsOutputTypeDef
```

Required fields:

- `Initiators`: `List`\[`str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listvolumerecoverypointsinputrequesttypedef"></a>

## ListVolumeRecoveryPointsInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListVolumeRecoveryPointsInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="listvolumerecoverypointsoutputtypedef"></a>

## ListVolumeRecoveryPointsOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListVolumeRecoveryPointsOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `VolumeRecoveryPointInfos`:
  `List`\[[VolumeRecoveryPointInfoTypeDef](./type_defs.md#volumerecoverypointinfotypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listvolumesinputrequesttypedef"></a>

## ListVolumesInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListVolumesInputRequestTypeDef
```

Optional fields:

- `GatewayARN`: `str`
- `Marker`: `str`
- `Limit`: `int`

<a id="listvolumesoutputtypedef"></a>

## ListVolumesOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ListVolumesOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `Marker`: `str`
- `VolumeInfos`:
  `List`\[[VolumeInfoTypeDef](./type_defs.md#volumeinfotypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="nfsfilesharedefaultstypedef"></a>

## NFSFileShareDefaultsTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import NFSFileShareDefaultsTypeDef
```

Optional fields:

- `FileMode`: `str`
- `DirectoryMode`: `str`
- `GroupId`: `int`
- `OwnerId`: `int`

<a id="nfsfileshareinfotypedef"></a>

## NFSFileShareInfoTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import NFSFileShareInfoTypeDef
```

Optional fields:

- `NFSFileShareDefaults`:
  [NFSFileShareDefaultsTypeDef](./type_defs.md#nfsfilesharedefaultstypedef)
- `FileShareARN`: `str`
- `FileShareId`: `str`
- `FileShareStatus`: `str`
- `GatewayARN`: `str`
- `KMSEncrypted`: `bool`
- `KMSKey`: `str`
- `Path`: `str`
- `Role`: `str`
- `LocationARN`: `str`
- `DefaultStorageClass`: `str`
- `ObjectACL`: [ObjectACLType](./literals.md#objectacltype)
- `ClientList`: `List`\[`str`\]
- `Squash`: `str`
- `ReadOnly`: `bool`
- `GuessMIMETypeEnabled`: `bool`
- `RequesterPays`: `bool`
- `Tags`: `List`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `FileShareName`: `str`
- `CacheAttributes`:
  [CacheAttributesTypeDef](./type_defs.md#cacheattributestypedef)
- `NotificationPolicy`: `str`
- `VPCEndpointDNSName`: `str`
- `BucketRegion`: `str`
- `AuditDestinationARN`: `str`

<a id="networkinterfacetypedef"></a>

## NetworkInterfaceTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import NetworkInterfaceTypeDef
```

Optional fields:

- `Ipv4Address`: `str`
- `MacAddress`: `str`
- `Ipv6Address`: `str`

<a id="notifywhenuploadedinputrequesttypedef"></a>

## NotifyWhenUploadedInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import NotifyWhenUploadedInputRequestTypeDef
```

Required fields:

- `FileShareARN`: `str`

<a id="notifywhenuploadedoutputtypedef"></a>

## NotifyWhenUploadedOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import NotifyWhenUploadedOutputTypeDef
```

Required fields:

- `FileShareARN`: `str`
- `NotificationId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="paginatorconfigtypedef"></a>

## PaginatorConfigTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import PaginatorConfigTypeDef
```

Optional fields:

- `MaxItems`: `int`
- `PageSize`: `int`
- `StartingToken`: `str`

<a id="poolinfotypedef"></a>

## PoolInfoTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import PoolInfoTypeDef
```

Optional fields:

- `PoolARN`: `str`
- `PoolName`: `str`
- `StorageClass`: [TapeStorageClassType](./literals.md#tapestorageclasstype)
- `RetentionLockType`:
  [RetentionLockTypeType](./literals.md#retentionlocktypetype)
- `RetentionLockTimeInDays`: `int`
- `PoolStatus`: [PoolStatusType](./literals.md#poolstatustype)

<a id="refreshcacheinputrequesttypedef"></a>

## RefreshCacheInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import RefreshCacheInputRequestTypeDef
```

Required fields:

- `FileShareARN`: `str`

Optional fields:

- `FolderList`: `Sequence`\[`str`\]
- `Recursive`: `bool`

<a id="refreshcacheoutputtypedef"></a>

## RefreshCacheOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import RefreshCacheOutputTypeDef
```

Required fields:

- `FileShareARN`: `str`
- `NotificationId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="removetagsfromresourceinputrequesttypedef"></a>

## RemoveTagsFromResourceInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import RemoveTagsFromResourceInputRequestTypeDef
```

Required fields:

- `ResourceARN`: `str`
- `TagKeys`: `Sequence`\[`str`\]

<a id="removetagsfromresourceoutputtypedef"></a>

## RemoveTagsFromResourceOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import RemoveTagsFromResourceOutputTypeDef
```

Required fields:

- `ResourceARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="resetcacheinputrequesttypedef"></a>

## ResetCacheInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ResetCacheInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="resetcacheoutputtypedef"></a>

## ResetCacheOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ResetCacheOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="retrievetapearchiveinputrequesttypedef"></a>

## RetrieveTapeArchiveInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import RetrieveTapeArchiveInputRequestTypeDef
```

Required fields:

- `TapeARN`: `str`
- `GatewayARN`: `str`

<a id="retrievetapearchiveoutputtypedef"></a>

## RetrieveTapeArchiveOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import RetrieveTapeArchiveOutputTypeDef
```

Required fields:

- `TapeARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="retrievetaperecoverypointinputrequesttypedef"></a>

## RetrieveTapeRecoveryPointInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import RetrieveTapeRecoveryPointInputRequestTypeDef
```

Required fields:

- `TapeARN`: `str`
- `GatewayARN`: `str`

<a id="retrievetaperecoverypointoutputtypedef"></a>

## RetrieveTapeRecoveryPointOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import RetrieveTapeRecoveryPointOutputTypeDef
```

Required fields:

- `TapeARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="smbfileshareinfotypedef"></a>

## SMBFileShareInfoTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import SMBFileShareInfoTypeDef
```

Optional fields:

- `FileShareARN`: `str`
- `FileShareId`: `str`
- `FileShareStatus`: `str`
- `GatewayARN`: `str`
- `KMSEncrypted`: `bool`
- `KMSKey`: `str`
- `Path`: `str`
- `Role`: `str`
- `LocationARN`: `str`
- `DefaultStorageClass`: `str`
- `ObjectACL`: [ObjectACLType](./literals.md#objectacltype)
- `ReadOnly`: `bool`
- `GuessMIMETypeEnabled`: `bool`
- `RequesterPays`: `bool`
- `SMBACLEnabled`: `bool`
- `AccessBasedEnumeration`: `bool`
- `AdminUserList`: `List`\[`str`\]
- `ValidUserList`: `List`\[`str`\]
- `InvalidUserList`: `List`\[`str`\]
- `AuditDestinationARN`: `str`
- `Authentication`: `str`
- `CaseSensitivity`: [CaseSensitivityType](./literals.md#casesensitivitytype)
- `Tags`: `List`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `FileShareName`: `str`
- `CacheAttributes`:
  [CacheAttributesTypeDef](./type_defs.md#cacheattributestypedef)
- `NotificationPolicy`: `str`
- `VPCEndpointDNSName`: `str`
- `BucketRegion`: `str`
- `OplocksEnabled`: `bool`

<a id="smblocalgroupstypedef"></a>

## SMBLocalGroupsTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import SMBLocalGroupsTypeDef
```

Optional fields:

- `GatewayAdmins`: `List`\[`str`\]

<a id="setlocalconsolepasswordinputrequesttypedef"></a>

## SetLocalConsolePasswordInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import SetLocalConsolePasswordInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `LocalConsolePassword`: `str`

<a id="setlocalconsolepasswordoutputtypedef"></a>

## SetLocalConsolePasswordOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import SetLocalConsolePasswordOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="setsmbguestpasswordinputrequesttypedef"></a>

## SetSMBGuestPasswordInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import SetSMBGuestPasswordInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `Password`: `str`

<a id="setsmbguestpasswordoutputtypedef"></a>

## SetSMBGuestPasswordOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import SetSMBGuestPasswordOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="shutdowngatewayinputrequesttypedef"></a>

## ShutdownGatewayInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ShutdownGatewayInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="shutdowngatewayoutputtypedef"></a>

## ShutdownGatewayOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import ShutdownGatewayOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="startavailabilitymonitortestinputrequesttypedef"></a>

## StartAvailabilityMonitorTestInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import StartAvailabilityMonitorTestInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="startavailabilitymonitortestoutputtypedef"></a>

## StartAvailabilityMonitorTestOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import StartAvailabilityMonitorTestOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="startgatewayinputrequesttypedef"></a>

## StartGatewayInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import StartGatewayInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="startgatewayoutputtypedef"></a>

## StartGatewayOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import StartGatewayOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="storediscsivolumetypedef"></a>

## StorediSCSIVolumeTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import StorediSCSIVolumeTypeDef
```

Optional fields:

- `VolumeARN`: `str`
- `VolumeId`: `str`
- `VolumeType`: `str`
- `VolumeStatus`: `str`
- `VolumeAttachmentStatus`: `str`
- `VolumeSizeInBytes`: `int`
- `VolumeProgress`: `float`
- `VolumeDiskId`: `str`
- `SourceSnapshotId`: `str`
- `PreservedExistingData`: `bool`
- `VolumeiSCSIAttributes`:
  [VolumeiSCSIAttributesTypeDef](./type_defs.md#volumeiscsiattributestypedef)
- `CreatedDate`: `datetime`
- `VolumeUsedInBytes`: `int`
- `KMSKey`: `str`
- `TargetName`: `str`

<a id="tagtypedef"></a>

## TagTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import TagTypeDef
```

Required fields:

- `Key`: `str`
- `Value`: `str`

<a id="tapearchivetypedef"></a>

## TapeArchiveTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import TapeArchiveTypeDef
```

Optional fields:

- `TapeARN`: `str`
- `TapeBarcode`: `str`
- `TapeCreatedDate`: `datetime`
- `TapeSizeInBytes`: `int`
- `CompletionTime`: `datetime`
- `RetrievedTo`: `str`
- `TapeStatus`: `str`
- `TapeUsedInBytes`: `int`
- `KMSKey`: `str`
- `PoolId`: `str`
- `Worm`: `bool`
- `RetentionStartDate`: `datetime`
- `PoolEntryDate`: `datetime`

<a id="tapeinfotypedef"></a>

## TapeInfoTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import TapeInfoTypeDef
```

Optional fields:

- `TapeARN`: `str`
- `TapeBarcode`: `str`
- `TapeSizeInBytes`: `int`
- `TapeStatus`: `str`
- `GatewayARN`: `str`
- `PoolId`: `str`
- `RetentionStartDate`: `datetime`
- `PoolEntryDate`: `datetime`

<a id="taperecoverypointinfotypedef"></a>

## TapeRecoveryPointInfoTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import TapeRecoveryPointInfoTypeDef
```

Optional fields:

- `TapeARN`: `str`
- `TapeRecoveryPointTime`: `datetime`
- `TapeSizeInBytes`: `int`
- `TapeStatus`: `str`

<a id="tapetypedef"></a>

## TapeTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import TapeTypeDef
```

Optional fields:

- `TapeARN`: `str`
- `TapeBarcode`: `str`
- `TapeCreatedDate`: `datetime`
- `TapeSizeInBytes`: `int`
- `TapeStatus`: `str`
- `VTLDevice`: `str`
- `Progress`: `float`
- `TapeUsedInBytes`: `int`
- `KMSKey`: `str`
- `PoolId`: `str`
- `Worm`: `bool`
- `RetentionStartDate`: `datetime`
- `PoolEntryDate`: `datetime`

<a id="updateautomatictapecreationpolicyinputrequesttypedef"></a>

## UpdateAutomaticTapeCreationPolicyInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateAutomaticTapeCreationPolicyInputRequestTypeDef
```

Required fields:

- `AutomaticTapeCreationRules`:
  `Sequence`\[[AutomaticTapeCreationRuleTypeDef](./type_defs.md#automatictapecreationruletypedef)\]
- `GatewayARN`: `str`

<a id="updateautomatictapecreationpolicyoutputtypedef"></a>

## UpdateAutomaticTapeCreationPolicyOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateAutomaticTapeCreationPolicyOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updatebandwidthratelimitinputrequesttypedef"></a>

## UpdateBandwidthRateLimitInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateBandwidthRateLimitInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

Optional fields:

- `AverageUploadRateLimitInBitsPerSec`: `int`
- `AverageDownloadRateLimitInBitsPerSec`: `int`

<a id="updatebandwidthratelimitoutputtypedef"></a>

## UpdateBandwidthRateLimitOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateBandwidthRateLimitOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updatebandwidthratelimitscheduleinputrequesttypedef"></a>

## UpdateBandwidthRateLimitScheduleInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateBandwidthRateLimitScheduleInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `BandwidthRateLimitIntervals`:
  `Sequence`\[[BandwidthRateLimitIntervalTypeDef](./type_defs.md#bandwidthratelimitintervaltypedef)\]

<a id="updatebandwidthratelimitscheduleoutputtypedef"></a>

## UpdateBandwidthRateLimitScheduleOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateBandwidthRateLimitScheduleOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updatechapcredentialsinputrequesttypedef"></a>

## UpdateChapCredentialsInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateChapCredentialsInputRequestTypeDef
```

Required fields:

- `TargetARN`: `str`
- `SecretToAuthenticateInitiator`: `str`
- `InitiatorName`: `str`

Optional fields:

- `SecretToAuthenticateTarget`: `str`

<a id="updatechapcredentialsoutputtypedef"></a>

## UpdateChapCredentialsOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateChapCredentialsOutputTypeDef
```

Required fields:

- `TargetARN`: `str`
- `InitiatorName`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updatefilesystemassociationinputrequesttypedef"></a>

## UpdateFileSystemAssociationInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateFileSystemAssociationInputRequestTypeDef
```

Required fields:

- `FileSystemAssociationARN`: `str`

Optional fields:

- `UserName`: `str`
- `Password`: `str`
- `AuditDestinationARN`: `str`
- `CacheAttributes`:
  [CacheAttributesTypeDef](./type_defs.md#cacheattributestypedef)

<a id="updatefilesystemassociationoutputtypedef"></a>

## UpdateFileSystemAssociationOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateFileSystemAssociationOutputTypeDef
```

Required fields:

- `FileSystemAssociationARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updategatewayinformationinputrequesttypedef"></a>

## UpdateGatewayInformationInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateGatewayInformationInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

Optional fields:

- `GatewayName`: `str`
- `GatewayTimezone`: `str`
- `CloudWatchLogGroupARN`: `str`
- `GatewayCapacity`: [GatewayCapacityType](./literals.md#gatewaycapacitytype)

<a id="updategatewayinformationoutputtypedef"></a>

## UpdateGatewayInformationOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateGatewayInformationOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `GatewayName`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updategatewaysoftwarenowinputrequesttypedef"></a>

## UpdateGatewaySoftwareNowInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateGatewaySoftwareNowInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`

<a id="updategatewaysoftwarenowoutputtypedef"></a>

## UpdateGatewaySoftwareNowOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateGatewaySoftwareNowOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updatemaintenancestarttimeinputrequesttypedef"></a>

## UpdateMaintenanceStartTimeInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateMaintenanceStartTimeInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `HourOfDay`: `int`
- `MinuteOfHour`: `int`

Optional fields:

- `DayOfWeek`: `int`
- `DayOfMonth`: `int`

<a id="updatemaintenancestarttimeoutputtypedef"></a>

## UpdateMaintenanceStartTimeOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateMaintenanceStartTimeOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updatenfsfileshareinputrequesttypedef"></a>

## UpdateNFSFileShareInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateNFSFileShareInputRequestTypeDef
```

Required fields:

- `FileShareARN`: `str`

Optional fields:

- `KMSEncrypted`: `bool`
- `KMSKey`: `str`
- `NFSFileShareDefaults`:
  [NFSFileShareDefaultsTypeDef](./type_defs.md#nfsfilesharedefaultstypedef)
- `DefaultStorageClass`: `str`
- `ObjectACL`: [ObjectACLType](./literals.md#objectacltype)
- `ClientList`: `Sequence`\[`str`\]
- `Squash`: `str`
- `ReadOnly`: `bool`
- `GuessMIMETypeEnabled`: `bool`
- `RequesterPays`: `bool`
- `FileShareName`: `str`
- `CacheAttributes`:
  [CacheAttributesTypeDef](./type_defs.md#cacheattributestypedef)
- `NotificationPolicy`: `str`
- `AuditDestinationARN`: `str`

<a id="updatenfsfileshareoutputtypedef"></a>

## UpdateNFSFileShareOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateNFSFileShareOutputTypeDef
```

Required fields:

- `FileShareARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updatesmbfileshareinputrequesttypedef"></a>

## UpdateSMBFileShareInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateSMBFileShareInputRequestTypeDef
```

Required fields:

- `FileShareARN`: `str`

Optional fields:

- `KMSEncrypted`: `bool`
- `KMSKey`: `str`
- `DefaultStorageClass`: `str`
- `ObjectACL`: [ObjectACLType](./literals.md#objectacltype)
- `ReadOnly`: `bool`
- `GuessMIMETypeEnabled`: `bool`
- `RequesterPays`: `bool`
- `SMBACLEnabled`: `bool`
- `AccessBasedEnumeration`: `bool`
- `AdminUserList`: `Sequence`\[`str`\]
- `ValidUserList`: `Sequence`\[`str`\]
- `InvalidUserList`: `Sequence`\[`str`\]
- `AuditDestinationARN`: `str`
- `CaseSensitivity`: [CaseSensitivityType](./literals.md#casesensitivitytype)
- `FileShareName`: `str`
- `CacheAttributes`:
  [CacheAttributesTypeDef](./type_defs.md#cacheattributestypedef)
- `NotificationPolicy`: `str`
- `OplocksEnabled`: `bool`

<a id="updatesmbfileshareoutputtypedef"></a>

## UpdateSMBFileShareOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateSMBFileShareOutputTypeDef
```

Required fields:

- `FileShareARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updatesmbfilesharevisibilityinputrequesttypedef"></a>

## UpdateSMBFileShareVisibilityInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateSMBFileShareVisibilityInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `FileSharesVisible`: `bool`

<a id="updatesmbfilesharevisibilityoutputtypedef"></a>

## UpdateSMBFileShareVisibilityOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateSMBFileShareVisibilityOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updatesmblocalgroupsinputrequesttypedef"></a>

## UpdateSMBLocalGroupsInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateSMBLocalGroupsInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `SMBLocalGroups`:
  [SMBLocalGroupsTypeDef](./type_defs.md#smblocalgroupstypedef)

<a id="updatesmblocalgroupsoutputtypedef"></a>

## UpdateSMBLocalGroupsOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateSMBLocalGroupsOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updatesmbsecuritystrategyinputrequesttypedef"></a>

## UpdateSMBSecurityStrategyInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateSMBSecurityStrategyInputRequestTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `SMBSecurityStrategy`:
  [SMBSecurityStrategyType](./literals.md#smbsecuritystrategytype)

<a id="updatesmbsecuritystrategyoutputtypedef"></a>

## UpdateSMBSecurityStrategyOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateSMBSecurityStrategyOutputTypeDef
```

Required fields:

- `GatewayARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updatesnapshotscheduleinputrequesttypedef"></a>

## UpdateSnapshotScheduleInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateSnapshotScheduleInputRequestTypeDef
```

Required fields:

- `VolumeARN`: `str`
- `StartAt`: `int`
- `RecurrenceInHours`: `int`

Optional fields:

- `Description`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="updatesnapshotscheduleoutputtypedef"></a>

## UpdateSnapshotScheduleOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateSnapshotScheduleOutputTypeDef
```

Required fields:

- `VolumeARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updatevtldevicetypeinputrequesttypedef"></a>

## UpdateVTLDeviceTypeInputRequestTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateVTLDeviceTypeInputRequestTypeDef
```

Required fields:

- `VTLDeviceARN`: `str`
- `DeviceType`: `str`

<a id="updatevtldevicetypeoutputtypedef"></a>

## UpdateVTLDeviceTypeOutputTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import UpdateVTLDeviceTypeOutputTypeDef
```

Required fields:

- `VTLDeviceARN`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="vtldevicetypedef"></a>

## VTLDeviceTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import VTLDeviceTypeDef
```

Optional fields:

- `VTLDeviceARN`: `str`
- `VTLDeviceType`: `str`
- `VTLDeviceVendor`: `str`
- `VTLDeviceProductIdentifier`: `str`
- `DeviceiSCSIAttributes`:
  [DeviceiSCSIAttributesTypeDef](./type_defs.md#deviceiscsiattributestypedef)

<a id="volumeinfotypedef"></a>

## VolumeInfoTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import VolumeInfoTypeDef
```

Optional fields:

- `VolumeARN`: `str`
- `VolumeId`: `str`
- `GatewayARN`: `str`
- `GatewayId`: `str`
- `VolumeType`: `str`
- `VolumeSizeInBytes`: `int`
- `VolumeAttachmentStatus`: `str`

<a id="volumerecoverypointinfotypedef"></a>

## VolumeRecoveryPointInfoTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import VolumeRecoveryPointInfoTypeDef
```

Optional fields:

- `VolumeARN`: `str`
- `VolumeSizeInBytes`: `int`
- `VolumeUsageInBytes`: `int`
- `VolumeRecoveryPointTime`: `str`

<a id="volumeiscsiattributestypedef"></a>

## VolumeiSCSIAttributesTypeDef

```python
from types_aiobotocore_storagegateway.type_defs import VolumeiSCSIAttributesTypeDef
```

Optional fields:

- `TargetARN`: `str`
- `NetworkInterfaceId`: `str`
- `NetworkInterfacePort`: `int`
- `LunNumber`: `int`
- `ChapEnabled`: `bool`
