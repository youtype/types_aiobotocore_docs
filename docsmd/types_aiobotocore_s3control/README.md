# S3Control module

> [Index](../README.md) > S3Control


!!! note ""

    Auto-generated documentation for [S3Control](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#s3control)
    type annotations stubs module [types-aiobotocore-s3control](https://pypi.org/project/types-aiobotocore-s3control/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `S3Control` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `S3Control` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[s3control]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[s3control]'

# standalone installation
python -m pip install types-aiobotocore-s3control
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-s3control
```

## Usage

Code samples can be found in [Examples](./usage.md).

## S3ControlClient

Type annotations and code completion for  `#!python session.create_client("s3control")` as [S3ControlClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client)

```python
# S3ControlClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3control.client import S3ControlClient


session = get_session()
async with session.create_client("s3control") as client:
    client: S3ControlClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("s3control").get_paginator("...")`.

```python
# ListAccessPointsForObjectLambdaPaginator usage example

from types_aiobotocore_s3control.paginator import ListAccessPointsForObjectLambdaPaginator

def get_list_access_points_for_object_lambda_paginator() -> ListAccessPointsForObjectLambdaPaginator:
    return client.get_paginator("list_access_points_for_object_lambda"))
```

- [ListAccessPointsForObjectLambdaPaginator](./paginators.md#listaccesspointsforobjectlambdapaginator)
- [ListCallerAccessGrantsPaginator](./paginators.md#listcalleraccessgrantspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AsyncOperationNameType usage example

from types_aiobotocore_s3control.literals import AsyncOperationNameType

def get_value() -> AsyncOperationNameType:
    return "CreateMultiRegionAccessPoint"
```

- [AsyncOperationNameType](./literals.md#asyncoperationnametype)
- [BucketCannedACLType](./literals.md#bucketcannedacltype)
- [BucketLocationConstraintType](./literals.md#bucketlocationconstrainttype)
- [BucketVersioningStatusType](./literals.md#bucketversioningstatustype)
- [DeleteMarkerReplicationStatusType](./literals.md#deletemarkerreplicationstatustype)
- [ExistingObjectReplicationStatusType](./literals.md#existingobjectreplicationstatustype)
- [ExpirationStatusType](./literals.md#expirationstatustype)
- [FormatType](./literals.md#formattype)
- [GeneratedManifestFormatType](./literals.md#generatedmanifestformattype)
- [GranteeTypeType](./literals.md#granteetypetype)
- [JobManifestFieldNameType](./literals.md#jobmanifestfieldnametype)
- [JobManifestFormatType](./literals.md#jobmanifestformattype)
- [JobReportFormatType](./literals.md#jobreportformattype)
- [JobReportScopeType](./literals.md#jobreportscopetype)
- [JobStatusType](./literals.md#jobstatustype)
- [ListAccessPointsForObjectLambdaPaginatorName](./literals.md#listaccesspointsforobjectlambdapaginatorname)
- [ListCallerAccessGrantsPaginatorName](./literals.md#listcalleraccessgrantspaginatorname)
- [MFADeleteStatusType](./literals.md#mfadeletestatustype)
- [MFADeleteType](./literals.md#mfadeletetype)
- [MetricsStatusType](./literals.md#metricsstatustype)
- [MultiRegionAccessPointStatusType](./literals.md#multiregionaccesspointstatustype)
- [NetworkOriginType](./literals.md#networkorigintype)
- [ObjectLambdaAccessPointAliasStatusType](./literals.md#objectlambdaaccesspointaliasstatustype)
- [ObjectLambdaAllowedFeatureType](./literals.md#objectlambdaallowedfeaturetype)
- [ObjectLambdaTransformationConfigurationActionType](./literals.md#objectlambdatransformationconfigurationactiontype)
- [OperationNameType](./literals.md#operationnametype)
- [OutputSchemaVersionType](./literals.md#outputschemaversiontype)
- [OwnerOverrideType](./literals.md#owneroverridetype)
- [PermissionType](./literals.md#permissiontype)
- [PrivilegeType](./literals.md#privilegetype)
- [ReplicaModificationsStatusType](./literals.md#replicamodificationsstatustype)
- [ReplicationRuleStatusType](./literals.md#replicationrulestatustype)
- [ReplicationStatusType](./literals.md#replicationstatustype)
- [ReplicationStorageClassType](./literals.md#replicationstorageclasstype)
- [ReplicationTimeStatusType](./literals.md#replicationtimestatustype)
- [RequestedJobStatusType](./literals.md#requestedjobstatustype)
- [S3CannedAccessControlListType](./literals.md#s3cannedaccesscontrollisttype)
- [S3ChecksumAlgorithmType](./literals.md#s3checksumalgorithmtype)
- [S3GlacierJobTierType](./literals.md#s3glacierjobtiertype)
- [S3GranteeTypeIdentifierType](./literals.md#s3granteetypeidentifiertype)
- [S3MetadataDirectiveType](./literals.md#s3metadatadirectivetype)
- [S3ObjectLockLegalHoldStatusType](./literals.md#s3objectlocklegalholdstatustype)
- [S3ObjectLockModeType](./literals.md#s3objectlockmodetype)
- [S3ObjectLockRetentionModeType](./literals.md#s3objectlockretentionmodetype)
- [S3PermissionType](./literals.md#s3permissiontype)
- [S3PrefixTypeType](./literals.md#s3prefixtypetype)
- [S3SSEAlgorithmType](./literals.md#s3ssealgorithmtype)
- [S3StorageClassType](./literals.md#s3storageclasstype)
- [SseKmsEncryptedObjectsStatusType](./literals.md#ssekmsencryptedobjectsstatustype)
- [TransitionStorageClassType](./literals.md#transitionstorageclasstype)
- [S3ControlServiceName](./literals.md#s3controlservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AbortIncompleteMultipartUploadTypeDef](./type_defs.md#abortincompletemultipartuploadtypedef)
- [AccessControlTranslationTypeDef](./type_defs.md#accesscontroltranslationtypedef)
- [AccessGrantsLocationConfigurationTypeDef](./type_defs.md#accessgrantslocationconfigurationtypedef)
- [VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef)
- [ActivityMetricsTypeDef](./type_defs.md#activitymetricstypedef)
- [AdvancedCostOptimizationMetricsTypeDef](./type_defs.md#advancedcostoptimizationmetricstypedef)
- [AdvancedDataProtectionMetricsTypeDef](./type_defs.md#advanceddataprotectionmetricstypedef)
- [DetailedStatusCodesMetricsTypeDef](./type_defs.md#detailedstatuscodesmetricstypedef)
- [AssociateAccessGrantsIdentityCenterRequestRequestTypeDef](./type_defs.md#associateaccessgrantsidentitycenterrequestrequesttypedef)
- [AsyncErrorDetailsTypeDef](./type_defs.md#asyncerrordetailstypedef)
- [DeleteMultiRegionAccessPointInputTypeDef](./type_defs.md#deletemultiregionaccesspointinputtypedef)
- [PutMultiRegionAccessPointPolicyInputTypeDef](./type_defs.md#putmultiregionaccesspointpolicyinputtypedef)
- [AwsLambdaTransformationTypeDef](./type_defs.md#awslambdatransformationtypedef)
- [CloudWatchMetricsTypeDef](./type_defs.md#cloudwatchmetricstypedef)
- [GranteeTypeDef](./type_defs.md#granteetypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ObjectLambdaAccessPointAliasTypeDef](./type_defs.md#objectlambdaaccesspointaliastypedef)
- [PublicAccessBlockConfigurationTypeDef](./type_defs.md#publicaccessblockconfigurationtypedef)
- [CreateBucketConfigurationTypeDef](./type_defs.md#createbucketconfigurationtypedef)
- [JobReportTypeDef](./type_defs.md#jobreporttypedef)
- [S3TagTypeDef](./type_defs.md#s3tagtypedef)
- [RegionTypeDef](./type_defs.md#regiontypedef)
- [CredentialsTypeDef](./type_defs.md#credentialstypedef)
- [DeleteAccessGrantRequestRequestTypeDef](./type_defs.md#deleteaccessgrantrequestrequesttypedef)
- [DeleteAccessGrantsInstanceRequestRequestTypeDef](./type_defs.md#deleteaccessgrantsinstancerequestrequesttypedef)
- [DeleteAccessGrantsInstanceResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteaccessgrantsinstanceresourcepolicyrequestrequesttypedef)
- [DeleteAccessGrantsLocationRequestRequestTypeDef](./type_defs.md#deleteaccessgrantslocationrequestrequesttypedef)
- [DeleteAccessPointForObjectLambdaRequestRequestTypeDef](./type_defs.md#deleteaccesspointforobjectlambdarequestrequesttypedef)
- [DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef](./type_defs.md#deleteaccesspointpolicyforobjectlambdarequestrequesttypedef)
- [DeleteAccessPointPolicyRequestRequestTypeDef](./type_defs.md#deleteaccesspointpolicyrequestrequesttypedef)
- [DeleteAccessPointRequestRequestTypeDef](./type_defs.md#deleteaccesspointrequestrequesttypedef)
- [DeleteBucketLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#deletebucketlifecycleconfigurationrequestrequesttypedef)
- [DeleteBucketPolicyRequestRequestTypeDef](./type_defs.md#deletebucketpolicyrequestrequesttypedef)
- [DeleteBucketReplicationRequestRequestTypeDef](./type_defs.md#deletebucketreplicationrequestrequesttypedef)
- [DeleteBucketRequestRequestTypeDef](./type_defs.md#deletebucketrequestrequesttypedef)
- [DeleteBucketTaggingRequestRequestTypeDef](./type_defs.md#deletebuckettaggingrequestrequesttypedef)
- [DeleteJobTaggingRequestRequestTypeDef](./type_defs.md#deletejobtaggingrequestrequesttypedef)
- [DeleteMarkerReplicationTypeDef](./type_defs.md#deletemarkerreplicationtypedef)
- [DeletePublicAccessBlockRequestRequestTypeDef](./type_defs.md#deletepublicaccessblockrequestrequesttypedef)
- [DeleteStorageLensConfigurationRequestRequestTypeDef](./type_defs.md#deletestoragelensconfigurationrequestrequesttypedef)
- [DeleteStorageLensConfigurationTaggingRequestRequestTypeDef](./type_defs.md#deletestoragelensconfigurationtaggingrequestrequesttypedef)
- [DeleteStorageLensGroupRequestRequestTypeDef](./type_defs.md#deletestoragelensgrouprequestrequesttypedef)
- [DescribeJobRequestRequestTypeDef](./type_defs.md#describejobrequestrequesttypedef)
- [DescribeMultiRegionAccessPointOperationRequestRequestTypeDef](./type_defs.md#describemultiregionaccesspointoperationrequestrequesttypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [DissociateAccessGrantsIdentityCenterRequestRequestTypeDef](./type_defs.md#dissociateaccessgrantsidentitycenterrequestrequesttypedef)
- [EstablishedMultiRegionAccessPointPolicyTypeDef](./type_defs.md#establishedmultiregionaccesspointpolicytypedef)
- [ExcludeOutputTypeDef](./type_defs.md#excludeoutputtypedef)
- [ExcludeTypeDef](./type_defs.md#excludetypedef)
- [ExistingObjectReplicationTypeDef](./type_defs.md#existingobjectreplicationtypedef)
- [SSEKMSEncryptionTypeDef](./type_defs.md#ssekmsencryptiontypedef)
- [GetAccessGrantRequestRequestTypeDef](./type_defs.md#getaccessgrantrequestrequesttypedef)
- [GetAccessGrantsInstanceForPrefixRequestRequestTypeDef](./type_defs.md#getaccessgrantsinstanceforprefixrequestrequesttypedef)
- [GetAccessGrantsInstanceRequestRequestTypeDef](./type_defs.md#getaccessgrantsinstancerequestrequesttypedef)
- [GetAccessGrantsInstanceResourcePolicyRequestRequestTypeDef](./type_defs.md#getaccessgrantsinstanceresourcepolicyrequestrequesttypedef)
- [GetAccessGrantsLocationRequestRequestTypeDef](./type_defs.md#getaccessgrantslocationrequestrequesttypedef)
- [GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef](./type_defs.md#getaccesspointconfigurationforobjectlambdarequestrequesttypedef)
- [GetAccessPointForObjectLambdaRequestRequestTypeDef](./type_defs.md#getaccesspointforobjectlambdarequestrequesttypedef)
- [GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef](./type_defs.md#getaccesspointpolicyforobjectlambdarequestrequesttypedef)
- [GetAccessPointPolicyRequestRequestTypeDef](./type_defs.md#getaccesspointpolicyrequestrequesttypedef)
- [GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef](./type_defs.md#getaccesspointpolicystatusforobjectlambdarequestrequesttypedef)
- [PolicyStatusTypeDef](./type_defs.md#policystatustypedef)
- [GetAccessPointPolicyStatusRequestRequestTypeDef](./type_defs.md#getaccesspointpolicystatusrequestrequesttypedef)
- [GetAccessPointRequestRequestTypeDef](./type_defs.md#getaccesspointrequestrequesttypedef)
- [GetBucketLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#getbucketlifecycleconfigurationrequestrequesttypedef)
- [GetBucketPolicyRequestRequestTypeDef](./type_defs.md#getbucketpolicyrequestrequesttypedef)
- [GetBucketReplicationRequestRequestTypeDef](./type_defs.md#getbucketreplicationrequestrequesttypedef)
- [GetBucketRequestRequestTypeDef](./type_defs.md#getbucketrequestrequesttypedef)
- [GetBucketTaggingRequestRequestTypeDef](./type_defs.md#getbuckettaggingrequestrequesttypedef)
- [GetBucketVersioningRequestRequestTypeDef](./type_defs.md#getbucketversioningrequestrequesttypedef)
- [GetDataAccessRequestRequestTypeDef](./type_defs.md#getdataaccessrequestrequesttypedef)
- [GetJobTaggingRequestRequestTypeDef](./type_defs.md#getjobtaggingrequestrequesttypedef)
- [GetMultiRegionAccessPointPolicyRequestRequestTypeDef](./type_defs.md#getmultiregionaccesspointpolicyrequestrequesttypedef)
- [GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef](./type_defs.md#getmultiregionaccesspointpolicystatusrequestrequesttypedef)
- [GetMultiRegionAccessPointRequestRequestTypeDef](./type_defs.md#getmultiregionaccesspointrequestrequesttypedef)
- [GetMultiRegionAccessPointRoutesRequestRequestTypeDef](./type_defs.md#getmultiregionaccesspointroutesrequestrequesttypedef)
- [MultiRegionAccessPointRouteTypeDef](./type_defs.md#multiregionaccesspointroutetypedef)
- [GetPublicAccessBlockRequestRequestTypeDef](./type_defs.md#getpublicaccessblockrequestrequesttypedef)
- [GetStorageLensConfigurationRequestRequestTypeDef](./type_defs.md#getstoragelensconfigurationrequestrequesttypedef)
- [GetStorageLensConfigurationTaggingRequestRequestTypeDef](./type_defs.md#getstoragelensconfigurationtaggingrequestrequesttypedef)
- [StorageLensTagTypeDef](./type_defs.md#storagelenstagtypedef)
- [GetStorageLensGroupRequestRequestTypeDef](./type_defs.md#getstoragelensgrouprequestrequesttypedef)
- [IncludeOutputTypeDef](./type_defs.md#includeoutputtypedef)
- [IncludeTypeDef](./type_defs.md#includetypedef)
- [JobFailureTypeDef](./type_defs.md#jobfailuretypedef)
- [KeyNameConstraintOutputTypeDef](./type_defs.md#keynameconstraintoutputtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [JobManifestLocationTypeDef](./type_defs.md#jobmanifestlocationtypedef)
- [JobManifestSpecOutputTypeDef](./type_defs.md#jobmanifestspecoutputtypedef)
- [JobManifestSpecTypeDef](./type_defs.md#jobmanifestspectypedef)
- [LambdaInvokeOperationOutputTypeDef](./type_defs.md#lambdainvokeoperationoutputtypedef)
- [S3InitiateRestoreObjectOperationTypeDef](./type_defs.md#s3initiaterestoreobjectoperationtypedef)
- [JobTimersTypeDef](./type_defs.md#jobtimerstypedef)
- [KeyNameConstraintTypeDef](./type_defs.md#keynameconstrainttypedef)
- [LambdaInvokeOperationTypeDef](./type_defs.md#lambdainvokeoperationtypedef)
- [LifecycleExpirationOutputTypeDef](./type_defs.md#lifecycleexpirationoutputtypedef)
- [NoncurrentVersionExpirationTypeDef](./type_defs.md#noncurrentversionexpirationtypedef)
- [NoncurrentVersionTransitionTypeDef](./type_defs.md#noncurrentversiontransitiontypedef)
- [TransitionOutputTypeDef](./type_defs.md#transitionoutputtypedef)
- [ListAccessGrantsInstanceEntryTypeDef](./type_defs.md#listaccessgrantsinstanceentrytypedef)
- [ListAccessGrantsInstancesRequestRequestTypeDef](./type_defs.md#listaccessgrantsinstancesrequestrequesttypedef)
- [ListAccessGrantsLocationsEntryTypeDef](./type_defs.md#listaccessgrantslocationsentrytypedef)
- [ListAccessGrantsLocationsRequestRequestTypeDef](./type_defs.md#listaccessgrantslocationsrequestrequesttypedef)
- [ListAccessGrantsRequestRequestTypeDef](./type_defs.md#listaccessgrantsrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAccessPointsForObjectLambdaRequestRequestTypeDef](./type_defs.md#listaccesspointsforobjectlambdarequestrequesttypedef)
- [ListAccessPointsRequestRequestTypeDef](./type_defs.md#listaccesspointsrequestrequesttypedef)
- [ListCallerAccessGrantsEntryTypeDef](./type_defs.md#listcalleraccessgrantsentrytypedef)
- [ListCallerAccessGrantsRequestRequestTypeDef](./type_defs.md#listcalleraccessgrantsrequestrequesttypedef)
- [ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef)
- [ListMultiRegionAccessPointsRequestRequestTypeDef](./type_defs.md#listmultiregionaccesspointsrequestrequesttypedef)
- [ListRegionalBucketsRequestRequestTypeDef](./type_defs.md#listregionalbucketsrequestrequesttypedef)
- [RegionalBucketTypeDef](./type_defs.md#regionalbuckettypedef)
- [ListStorageLensConfigurationEntryTypeDef](./type_defs.md#liststoragelensconfigurationentrytypedef)
- [ListStorageLensConfigurationsRequestRequestTypeDef](./type_defs.md#liststoragelensconfigurationsrequestrequesttypedef)
- [ListStorageLensGroupEntryTypeDef](./type_defs.md#liststoragelensgroupentrytypedef)
- [ListStorageLensGroupsRequestRequestTypeDef](./type_defs.md#liststoragelensgroupsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [MatchObjectAgeTypeDef](./type_defs.md#matchobjectagetypedef)
- [MatchObjectSizeTypeDef](./type_defs.md#matchobjectsizetypedef)
- [ReplicationTimeValueTypeDef](./type_defs.md#replicationtimevaluetypedef)
- [ProposedMultiRegionAccessPointPolicyTypeDef](./type_defs.md#proposedmultiregionaccesspointpolicytypedef)
- [MultiRegionAccessPointRegionalResponseTypeDef](./type_defs.md#multiregionaccesspointregionalresponsetypedef)
- [RegionReportTypeDef](./type_defs.md#regionreporttypedef)
- [SelectionCriteriaTypeDef](./type_defs.md#selectioncriteriatypedef)
- [PutAccessGrantsInstanceResourcePolicyRequestRequestTypeDef](./type_defs.md#putaccessgrantsinstanceresourcepolicyrequestrequesttypedef)
- [PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef](./type_defs.md#putaccesspointpolicyforobjectlambdarequestrequesttypedef)
- [PutAccessPointPolicyRequestRequestTypeDef](./type_defs.md#putaccesspointpolicyrequestrequesttypedef)
- [PutBucketPolicyRequestRequestTypeDef](./type_defs.md#putbucketpolicyrequestrequesttypedef)
- [VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef)
- [ReplicaModificationsTypeDef](./type_defs.md#replicamodificationstypedef)
- [S3ObjectOwnerTypeDef](./type_defs.md#s3objectownertypedef)
- [S3ObjectMetadataOutputTypeDef](./type_defs.md#s3objectmetadataoutputtypedef)
- [S3GranteeTypeDef](./type_defs.md#s3granteetypedef)
- [S3ObjectLockLegalHoldTypeDef](./type_defs.md#s3objectlocklegalholdtypedef)
- [S3RetentionOutputTypeDef](./type_defs.md#s3retentionoutputtypedef)
- [SSEKMSTypeDef](./type_defs.md#ssekmstypedef)
- [SseKmsEncryptedObjectsTypeDef](./type_defs.md#ssekmsencryptedobjectstypedef)
- [StorageLensAwsOrgTypeDef](./type_defs.md#storagelensawsorgtypedef)
- [StorageLensGroupLevelSelectionCriteriaOutputTypeDef](./type_defs.md#storagelensgrouplevelselectioncriteriaoutputtypedef)
- [StorageLensGroupLevelSelectionCriteriaTypeDef](./type_defs.md#storagelensgrouplevelselectioncriteriatypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAccessGrantsLocationRequestRequestTypeDef](./type_defs.md#updateaccessgrantslocationrequestrequesttypedef)
- [UpdateJobPriorityRequestRequestTypeDef](./type_defs.md#updatejobpriorityrequestrequesttypedef)
- [UpdateJobStatusRequestRequestTypeDef](./type_defs.md#updatejobstatusrequestrequesttypedef)
- [AccessPointTypeDef](./type_defs.md#accesspointtypedef)
- [DeleteMultiRegionAccessPointRequestRequestTypeDef](./type_defs.md#deletemultiregionaccesspointrequestrequesttypedef)
- [PutMultiRegionAccessPointPolicyRequestRequestTypeDef](./type_defs.md#putmultiregionaccesspointpolicyrequestrequesttypedef)
- [ObjectLambdaContentTransformationTypeDef](./type_defs.md#objectlambdacontenttransformationtypedef)
- [ListAccessGrantEntryTypeDef](./type_defs.md#listaccessgrantentrytypedef)
- [CreateAccessGrantRequestRequestTypeDef](./type_defs.md#createaccessgrantrequestrequesttypedef)
- [CreateAccessGrantsInstanceRequestRequestTypeDef](./type_defs.md#createaccessgrantsinstancerequestrequesttypedef)
- [CreateAccessGrantsLocationRequestRequestTypeDef](./type_defs.md#createaccessgrantslocationrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateAccessGrantResultTypeDef](./type_defs.md#createaccessgrantresulttypedef)
- [CreateAccessGrantsInstanceResultTypeDef](./type_defs.md#createaccessgrantsinstanceresulttypedef)
- [CreateAccessGrantsLocationResultTypeDef](./type_defs.md#createaccessgrantslocationresulttypedef)
- [CreateAccessPointResultTypeDef](./type_defs.md#createaccesspointresulttypedef)
- [CreateBucketResultTypeDef](./type_defs.md#createbucketresulttypedef)
- [CreateJobResultTypeDef](./type_defs.md#createjobresulttypedef)
- [CreateMultiRegionAccessPointResultTypeDef](./type_defs.md#createmultiregionaccesspointresulttypedef)
- [DeleteMultiRegionAccessPointResultTypeDef](./type_defs.md#deletemultiregionaccesspointresulttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetAccessGrantResultTypeDef](./type_defs.md#getaccessgrantresulttypedef)
- [GetAccessGrantsInstanceForPrefixResultTypeDef](./type_defs.md#getaccessgrantsinstanceforprefixresulttypedef)
- [GetAccessGrantsInstanceResourcePolicyResultTypeDef](./type_defs.md#getaccessgrantsinstanceresourcepolicyresulttypedef)
- [GetAccessGrantsInstanceResultTypeDef](./type_defs.md#getaccessgrantsinstanceresulttypedef)
- [GetAccessGrantsLocationResultTypeDef](./type_defs.md#getaccessgrantslocationresulttypedef)
- [GetAccessPointPolicyForObjectLambdaResultTypeDef](./type_defs.md#getaccesspointpolicyforobjectlambdaresulttypedef)
- [GetAccessPointPolicyResultTypeDef](./type_defs.md#getaccesspointpolicyresulttypedef)
- [GetBucketPolicyResultTypeDef](./type_defs.md#getbucketpolicyresulttypedef)
- [GetBucketResultTypeDef](./type_defs.md#getbucketresulttypedef)
- [GetBucketVersioningResultTypeDef](./type_defs.md#getbucketversioningresulttypedef)
- [ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef)
- [PutAccessGrantsInstanceResourcePolicyResultTypeDef](./type_defs.md#putaccessgrantsinstanceresourcepolicyresulttypedef)
- [PutMultiRegionAccessPointPolicyResultTypeDef](./type_defs.md#putmultiregionaccesspointpolicyresulttypedef)
- [UpdateAccessGrantsLocationResultTypeDef](./type_defs.md#updateaccessgrantslocationresulttypedef)
- [UpdateJobPriorityResultTypeDef](./type_defs.md#updatejobpriorityresulttypedef)
- [UpdateJobStatusResultTypeDef](./type_defs.md#updatejobstatusresulttypedef)
- [CreateAccessPointForObjectLambdaResultTypeDef](./type_defs.md#createaccesspointforobjectlambdaresulttypedef)
- [ObjectLambdaAccessPointTypeDef](./type_defs.md#objectlambdaaccesspointtypedef)
- [CreateAccessPointRequestRequestTypeDef](./type_defs.md#createaccesspointrequestrequesttypedef)
- [GetAccessPointForObjectLambdaResultTypeDef](./type_defs.md#getaccesspointforobjectlambdaresulttypedef)
- [GetAccessPointResultTypeDef](./type_defs.md#getaccesspointresulttypedef)
- [GetPublicAccessBlockOutputTypeDef](./type_defs.md#getpublicaccessblockoutputtypedef)
- [PutPublicAccessBlockRequestRequestTypeDef](./type_defs.md#putpublicaccessblockrequestrequesttypedef)
- [CreateBucketRequestRequestTypeDef](./type_defs.md#createbucketrequestrequesttypedef)
- [GetBucketTaggingResultTypeDef](./type_defs.md#getbuckettaggingresulttypedef)
- [GetJobTaggingResultTypeDef](./type_defs.md#getjobtaggingresulttypedef)
- [LifecycleRuleAndOperatorOutputTypeDef](./type_defs.md#lifecycleruleandoperatoroutputtypedef)
- [LifecycleRuleAndOperatorTypeDef](./type_defs.md#lifecycleruleandoperatortypedef)
- [PutJobTaggingRequestRequestTypeDef](./type_defs.md#putjobtaggingrequestrequesttypedef)
- [ReplicationRuleAndOperatorOutputTypeDef](./type_defs.md#replicationruleandoperatoroutputtypedef)
- [ReplicationRuleAndOperatorTypeDef](./type_defs.md#replicationruleandoperatortypedef)
- [S3SetObjectTaggingOperationOutputTypeDef](./type_defs.md#s3setobjecttaggingoperationoutputtypedef)
- [S3SetObjectTaggingOperationTypeDef](./type_defs.md#s3setobjecttaggingoperationtypedef)
- [TaggingTypeDef](./type_defs.md#taggingtypedef)
- [CreateMultiRegionAccessPointInputOutputTypeDef](./type_defs.md#createmultiregionaccesspointinputoutputtypedef)
- [CreateMultiRegionAccessPointInputTypeDef](./type_defs.md#createmultiregionaccesspointinputtypedef)
- [GetDataAccessResultTypeDef](./type_defs.md#getdataaccessresulttypedef)
- [ExcludeUnionTypeDef](./type_defs.md#excludeuniontypedef)
- [GeneratedManifestEncryptionOutputTypeDef](./type_defs.md#generatedmanifestencryptionoutputtypedef)
- [GeneratedManifestEncryptionTypeDef](./type_defs.md#generatedmanifestencryptiontypedef)
- [GetAccessPointPolicyStatusForObjectLambdaResultTypeDef](./type_defs.md#getaccesspointpolicystatusforobjectlambdaresulttypedef)
- [GetAccessPointPolicyStatusResultTypeDef](./type_defs.md#getaccesspointpolicystatusresulttypedef)
- [GetMultiRegionAccessPointPolicyStatusResultTypeDef](./type_defs.md#getmultiregionaccesspointpolicystatusresulttypedef)
- [GetMultiRegionAccessPointRoutesResultTypeDef](./type_defs.md#getmultiregionaccesspointroutesresulttypedef)
- [SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef](./type_defs.md#submitmultiregionaccesspointroutesrequestrequesttypedef)
- [GetStorageLensConfigurationTaggingResultTypeDef](./type_defs.md#getstoragelensconfigurationtaggingresulttypedef)
- [PutStorageLensConfigurationTaggingRequestRequestTypeDef](./type_defs.md#putstoragelensconfigurationtaggingrequestrequesttypedef)
- [IncludeUnionTypeDef](./type_defs.md#includeuniontypedef)
- [JobManifestGeneratorFilterOutputTypeDef](./type_defs.md#jobmanifestgeneratorfilteroutputtypedef)
- [LifecycleExpirationTypeDef](./type_defs.md#lifecycleexpirationtypedef)
- [S3ObjectMetadataTypeDef](./type_defs.md#s3objectmetadatatypedef)
- [S3RetentionTypeDef](./type_defs.md#s3retentiontypedef)
- [TransitionTypeDef](./type_defs.md#transitiontypedef)
- [S3GeneratedManifestDescriptorTypeDef](./type_defs.md#s3generatedmanifestdescriptortypedef)
- [JobManifestOutputTypeDef](./type_defs.md#jobmanifestoutputtypedef)
- [JobManifestSpecUnionTypeDef](./type_defs.md#jobmanifestspecuniontypedef)
- [JobProgressSummaryTypeDef](./type_defs.md#jobprogresssummarytypedef)
- [KeyNameConstraintUnionTypeDef](./type_defs.md#keynameconstraintuniontypedef)
- [LambdaInvokeOperationUnionTypeDef](./type_defs.md#lambdainvokeoperationuniontypedef)
- [ListAccessGrantsInstancesResultTypeDef](./type_defs.md#listaccessgrantsinstancesresulttypedef)
- [ListAccessGrantsLocationsResultTypeDef](./type_defs.md#listaccessgrantslocationsresulttypedef)
- [ListAccessPointsForObjectLambdaRequestPaginateTypeDef](./type_defs.md#listaccesspointsforobjectlambdarequestpaginatetypedef)
- [ListCallerAccessGrantsRequestPaginateTypeDef](./type_defs.md#listcalleraccessgrantsrequestpaginatetypedef)
- [ListCallerAccessGrantsResultTypeDef](./type_defs.md#listcalleraccessgrantsresulttypedef)
- [ListRegionalBucketsResultTypeDef](./type_defs.md#listregionalbucketsresulttypedef)
- [ListStorageLensConfigurationsResultTypeDef](./type_defs.md#liststoragelensconfigurationsresulttypedef)
- [ListStorageLensGroupsResultTypeDef](./type_defs.md#liststoragelensgroupsresulttypedef)
- [StorageLensGroupAndOperatorOutputTypeDef](./type_defs.md#storagelensgroupandoperatoroutputtypedef)
- [StorageLensGroupAndOperatorTypeDef](./type_defs.md#storagelensgroupandoperatortypedef)
- [StorageLensGroupOrOperatorOutputTypeDef](./type_defs.md#storagelensgrouporoperatoroutputtypedef)
- [StorageLensGroupOrOperatorTypeDef](./type_defs.md#storagelensgrouporoperatortypedef)
- [MetricsTypeDef](./type_defs.md#metricstypedef)
- [ReplicationTimeTypeDef](./type_defs.md#replicationtimetypedef)
- [MultiRegionAccessPointPolicyDocumentTypeDef](./type_defs.md#multiregionaccesspointpolicydocumenttypedef)
- [MultiRegionAccessPointsAsyncResponseTypeDef](./type_defs.md#multiregionaccesspointsasyncresponsetypedef)
- [MultiRegionAccessPointReportTypeDef](./type_defs.md#multiregionaccesspointreporttypedef)
- [PrefixLevelStorageMetricsTypeDef](./type_defs.md#prefixlevelstoragemetricstypedef)
- [PutBucketVersioningRequestRequestTypeDef](./type_defs.md#putbucketversioningrequestrequesttypedef)
- [S3GrantTypeDef](./type_defs.md#s3granttypedef)
- [S3SetObjectLegalHoldOperationTypeDef](./type_defs.md#s3setobjectlegalholdoperationtypedef)
- [S3SetObjectRetentionOperationOutputTypeDef](./type_defs.md#s3setobjectretentionoperationoutputtypedef)
- [StorageLensDataExportEncryptionOutputTypeDef](./type_defs.md#storagelensdataexportencryptionoutputtypedef)
- [StorageLensDataExportEncryptionTypeDef](./type_defs.md#storagelensdataexportencryptiontypedef)
- [SourceSelectionCriteriaTypeDef](./type_defs.md#sourceselectioncriteriatypedef)
- [StorageLensGroupLevelOutputTypeDef](./type_defs.md#storagelensgroupleveloutputtypedef)
- [StorageLensGroupLevelSelectionCriteriaUnionTypeDef](./type_defs.md#storagelensgrouplevelselectioncriteriauniontypedef)
- [ListAccessPointsResultTypeDef](./type_defs.md#listaccesspointsresulttypedef)
- [ObjectLambdaTransformationConfigurationOutputTypeDef](./type_defs.md#objectlambdatransformationconfigurationoutputtypedef)
- [ObjectLambdaTransformationConfigurationTypeDef](./type_defs.md#objectlambdatransformationconfigurationtypedef)
- [ListAccessGrantsResultTypeDef](./type_defs.md#listaccessgrantsresulttypedef)
- [ListAccessPointsForObjectLambdaResultTypeDef](./type_defs.md#listaccesspointsforobjectlambdaresulttypedef)
- [LifecycleRuleFilterOutputTypeDef](./type_defs.md#lifecyclerulefilteroutputtypedef)
- [LifecycleRuleAndOperatorUnionTypeDef](./type_defs.md#lifecycleruleandoperatoruniontypedef)
- [ReplicationRuleFilterOutputTypeDef](./type_defs.md#replicationrulefilteroutputtypedef)
- [ReplicationRuleAndOperatorUnionTypeDef](./type_defs.md#replicationruleandoperatoruniontypedef)
- [S3SetObjectTaggingOperationUnionTypeDef](./type_defs.md#s3setobjecttaggingoperationuniontypedef)
- [PutBucketTaggingRequestRequestTypeDef](./type_defs.md#putbuckettaggingrequestrequesttypedef)
- [AsyncRequestParametersTypeDef](./type_defs.md#asyncrequestparameterstypedef)
- [CreateMultiRegionAccessPointRequestRequestTypeDef](./type_defs.md#createmultiregionaccesspointrequestrequesttypedef)
- [S3ManifestOutputLocationOutputTypeDef](./type_defs.md#s3manifestoutputlocationoutputtypedef)
- [GeneratedManifestEncryptionUnionTypeDef](./type_defs.md#generatedmanifestencryptionuniontypedef)
- [LifecycleExpirationUnionTypeDef](./type_defs.md#lifecycleexpirationuniontypedef)
- [S3ObjectMetadataUnionTypeDef](./type_defs.md#s3objectmetadatauniontypedef)
- [S3RetentionUnionTypeDef](./type_defs.md#s3retentionuniontypedef)
- [TransitionUnionTypeDef](./type_defs.md#transitionuniontypedef)
- [JobManifestTypeDef](./type_defs.md#jobmanifesttypedef)
- [JobListDescriptorTypeDef](./type_defs.md#joblistdescriptortypedef)
- [JobManifestGeneratorFilterTypeDef](./type_defs.md#jobmanifestgeneratorfiltertypedef)
- [StorageLensGroupAndOperatorUnionTypeDef](./type_defs.md#storagelensgroupandoperatoruniontypedef)
- [StorageLensGroupFilterOutputTypeDef](./type_defs.md#storagelensgroupfilteroutputtypedef)
- [StorageLensGroupOrOperatorUnionTypeDef](./type_defs.md#storagelensgrouporoperatoruniontypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [GetMultiRegionAccessPointPolicyResultTypeDef](./type_defs.md#getmultiregionaccesspointpolicyresulttypedef)
- [AsyncResponseDetailsTypeDef](./type_defs.md#asyncresponsedetailstypedef)
- [GetMultiRegionAccessPointResultTypeDef](./type_defs.md#getmultiregionaccesspointresulttypedef)
- [ListMultiRegionAccessPointsResultTypeDef](./type_defs.md#listmultiregionaccesspointsresulttypedef)
- [PrefixLevelTypeDef](./type_defs.md#prefixleveltypedef)
- [S3AccessControlListOutputTypeDef](./type_defs.md#s3accesscontrollistoutputtypedef)
- [S3AccessControlListTypeDef](./type_defs.md#s3accesscontrollisttypedef)
- [S3CopyObjectOperationOutputTypeDef](./type_defs.md#s3copyobjectoperationoutputtypedef)
- [S3BucketDestinationOutputTypeDef](./type_defs.md#s3bucketdestinationoutputtypedef)
- [StorageLensDataExportEncryptionUnionTypeDef](./type_defs.md#storagelensdataexportencryptionuniontypedef)
- [StorageLensGroupLevelTypeDef](./type_defs.md#storagelensgroupleveltypedef)
- [ObjectLambdaConfigurationOutputTypeDef](./type_defs.md#objectlambdaconfigurationoutputtypedef)
- [ObjectLambdaTransformationConfigurationUnionTypeDef](./type_defs.md#objectlambdatransformationconfigurationuniontypedef)
- [LifecycleRuleOutputTypeDef](./type_defs.md#lifecycleruleoutputtypedef)
- [LifecycleRuleFilterTypeDef](./type_defs.md#lifecyclerulefiltertypedef)
- [ReplicationRuleFilterTypeDef](./type_defs.md#replicationrulefiltertypedef)
- [S3JobManifestGeneratorOutputTypeDef](./type_defs.md#s3jobmanifestgeneratoroutputtypedef)
- [S3ManifestOutputLocationTypeDef](./type_defs.md#s3manifestoutputlocationtypedef)
- [S3CopyObjectOperationTypeDef](./type_defs.md#s3copyobjectoperationtypedef)
- [S3SetObjectRetentionOperationTypeDef](./type_defs.md#s3setobjectretentionoperationtypedef)
- [ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef)
- [JobManifestGeneratorFilterUnionTypeDef](./type_defs.md#jobmanifestgeneratorfilteruniontypedef)
- [StorageLensGroupOutputTypeDef](./type_defs.md#storagelensgroupoutputtypedef)
- [StorageLensGroupFilterTypeDef](./type_defs.md#storagelensgroupfiltertypedef)
- [ReplicationRuleOutputTypeDef](./type_defs.md#replicationruleoutputtypedef)
- [AsyncOperationTypeDef](./type_defs.md#asyncoperationtypedef)
- [BucketLevelTypeDef](./type_defs.md#bucketleveltypedef)
- [S3AccessControlPolicyOutputTypeDef](./type_defs.md#s3accesscontrolpolicyoutputtypedef)
- [S3AccessControlListUnionTypeDef](./type_defs.md#s3accesscontrollistuniontypedef)
- [StorageLensDataExportOutputTypeDef](./type_defs.md#storagelensdataexportoutputtypedef)
- [S3BucketDestinationTypeDef](./type_defs.md#s3bucketdestinationtypedef)
- [StorageLensGroupLevelUnionTypeDef](./type_defs.md#storagelensgroupleveluniontypedef)
- [GetAccessPointConfigurationForObjectLambdaResultTypeDef](./type_defs.md#getaccesspointconfigurationforobjectlambdaresulttypedef)
- [ObjectLambdaConfigurationTypeDef](./type_defs.md#objectlambdaconfigurationtypedef)
- [GetBucketLifecycleConfigurationResultTypeDef](./type_defs.md#getbucketlifecycleconfigurationresulttypedef)
- [LifecycleRuleFilterUnionTypeDef](./type_defs.md#lifecyclerulefilteruniontypedef)
- [ReplicationRuleFilterUnionTypeDef](./type_defs.md#replicationrulefilteruniontypedef)
- [JobManifestGeneratorOutputTypeDef](./type_defs.md#jobmanifestgeneratoroutputtypedef)
- [S3ManifestOutputLocationUnionTypeDef](./type_defs.md#s3manifestoutputlocationuniontypedef)
- [S3CopyObjectOperationUnionTypeDef](./type_defs.md#s3copyobjectoperationuniontypedef)
- [S3SetObjectRetentionOperationUnionTypeDef](./type_defs.md#s3setobjectretentionoperationuniontypedef)
- [GetStorageLensGroupResultTypeDef](./type_defs.md#getstoragelensgroupresulttypedef)
- [StorageLensGroupFilterUnionTypeDef](./type_defs.md#storagelensgroupfilteruniontypedef)
- [ReplicationConfigurationOutputTypeDef](./type_defs.md#replicationconfigurationoutputtypedef)
- [DescribeMultiRegionAccessPointOperationResultTypeDef](./type_defs.md#describemultiregionaccesspointoperationresulttypedef)
- [AccountLevelOutputTypeDef](./type_defs.md#accountleveloutputtypedef)
- [S3SetObjectAclOperationOutputTypeDef](./type_defs.md#s3setobjectacloperationoutputtypedef)
- [S3AccessControlPolicyTypeDef](./type_defs.md#s3accesscontrolpolicytypedef)
- [S3BucketDestinationUnionTypeDef](./type_defs.md#s3bucketdestinationuniontypedef)
- [AccountLevelTypeDef](./type_defs.md#accountleveltypedef)
- [CreateAccessPointForObjectLambdaRequestRequestTypeDef](./type_defs.md#createaccesspointforobjectlambdarequestrequesttypedef)
- [PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef](./type_defs.md#putaccesspointconfigurationforobjectlambdarequestrequesttypedef)
- [LifecycleRuleTypeDef](./type_defs.md#lifecycleruletypedef)
- [ReplicationRuleTypeDef](./type_defs.md#replicationruletypedef)
- [S3JobManifestGeneratorTypeDef](./type_defs.md#s3jobmanifestgeneratortypedef)
- [StorageLensGroupTypeDef](./type_defs.md#storagelensgrouptypedef)
- [GetBucketReplicationResultTypeDef](./type_defs.md#getbucketreplicationresulttypedef)
- [StorageLensConfigurationOutputTypeDef](./type_defs.md#storagelensconfigurationoutputtypedef)
- [JobOperationOutputTypeDef](./type_defs.md#joboperationoutputtypedef)
- [S3AccessControlPolicyUnionTypeDef](./type_defs.md#s3accesscontrolpolicyuniontypedef)
- [StorageLensDataExportTypeDef](./type_defs.md#storagelensdataexporttypedef)
- [AccountLevelUnionTypeDef](./type_defs.md#accountleveluniontypedef)
- [LifecycleRuleUnionTypeDef](./type_defs.md#lifecycleruleuniontypedef)
- [ReplicationRuleUnionTypeDef](./type_defs.md#replicationruleuniontypedef)
- [S3JobManifestGeneratorUnionTypeDef](./type_defs.md#s3jobmanifestgeneratoruniontypedef)
- [CreateStorageLensGroupRequestRequestTypeDef](./type_defs.md#createstoragelensgrouprequestrequesttypedef)
- [UpdateStorageLensGroupRequestRequestTypeDef](./type_defs.md#updatestoragelensgrouprequestrequesttypedef)
- [GetStorageLensConfigurationResultTypeDef](./type_defs.md#getstoragelensconfigurationresulttypedef)
- [JobDescriptorTypeDef](./type_defs.md#jobdescriptortypedef)
- [S3SetObjectAclOperationTypeDef](./type_defs.md#s3setobjectacloperationtypedef)
- [StorageLensDataExportUnionTypeDef](./type_defs.md#storagelensdataexportuniontypedef)
- [LifecycleConfigurationTypeDef](./type_defs.md#lifecycleconfigurationtypedef)
- [ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef)
- [JobManifestGeneratorTypeDef](./type_defs.md#jobmanifestgeneratortypedef)
- [DescribeJobResultTypeDef](./type_defs.md#describejobresulttypedef)
- [S3SetObjectAclOperationUnionTypeDef](./type_defs.md#s3setobjectacloperationuniontypedef)
- [StorageLensConfigurationTypeDef](./type_defs.md#storagelensconfigurationtypedef)
- [PutBucketLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#putbucketlifecycleconfigurationrequestrequesttypedef)
- [PutBucketReplicationRequestRequestTypeDef](./type_defs.md#putbucketreplicationrequestrequesttypedef)
- [JobOperationTypeDef](./type_defs.md#joboperationtypedef)
- [PutStorageLensConfigurationRequestRequestTypeDef](./type_defs.md#putstoragelensconfigurationrequestrequesttypedef)
- [CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef)

