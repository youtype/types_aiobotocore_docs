# S3 module

> [Index](../README.md) > S3


!!! note ""

    Auto-generated documentation for [S3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
    type annotations stubs module [types-aiobotocore-s3](https://pypi.org/project/types-aiobotocore-s3/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `S3` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[s3]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[s3]'


# standalone installation
python -m pip install types-aiobotocore-s3
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-s3
```

## Usage

Code samples can be found in [Examples](./usage.md).

## S3Client

Type annotations and code completion for  `#!python session.create_client("s3")` as [S3Client](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client)

```python
# S3Client usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3.client import S3Client


session = get_session()
async with session.create_client("s3") as client:
    client: S3Client
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("s3").get_paginator("...")`.

```python
# ListBucketsPaginator usage example

from types_aiobotocore_s3.paginator import ListBucketsPaginator

def get_list_buckets_paginator() -> ListBucketsPaginator:
    return client.get_paginator("list_buckets"))
```

- [ListBucketsPaginator](./paginators.md#listbucketspaginator)
- [ListDirectoryBucketsPaginator](./paginators.md#listdirectorybucketspaginator)
- [ListMultipartUploadsPaginator](./paginators.md#listmultipartuploadspaginator)
- [ListObjectVersionsPaginator](./paginators.md#listobjectversionspaginator)
- [ListObjectsPaginator](./paginators.md#listobjectspaginator)
- [ListObjectsV2Paginator](./paginators.md#listobjectsv2paginator)
- [ListPartsPaginator](./paginators.md#listpartspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("s3").get_waiter("...")`.

```python
# BucketExistsWaiter usage example

from types_aiobotocore_s3.waiter import BucketExistsWaiter

def get_bucket_exists_waiter() -> BucketExistsWaiter:
    return Session().client("s3").get_waiter("bucket_exists")
```

- [BucketExistsWaiter](./waiters.md#bucketexistswaiter)
- [BucketNotExistsWaiter](./waiters.md#bucketnotexistswaiter)
- [ObjectExistsWaiter](./waiters.md#objectexistswaiter)
- [ObjectNotExistsWaiter](./waiters.md#objectnotexistswaiter)




## S3ServiceResource

Type annotations and code completion for `#!python session.resource("s3")` as
[S3ServiceResource](./service_resource.md#s3serviceresource)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource)

```python
# S3ServiceResource usage example

from types_aiobotocore_s3.service_resource import S3ServiceResource
```


### Collections

Type annotations and code completion for collections
from `#!python session.resource("s3").*`.

```python
# ServiceResourceBucketsCollection usage example

from types_aiobotocore_s3.service_resource import ServiceResourceBucketsCollection

def get_collection() -> ServiceResourceBucketsCollection:
    return resource.buckets
```

- [ServiceResourceBucketsCollection](./service_resource.md#s3serviceresourcebuckets)





### Resources

Type annotations and code completion for additional resources
from `#!python session.resource("s3").*`.

```python
# Bucket usage example

from types_aiobotocore_s3.service_resource import Bucket

def get_resource() -> Bucket:
    return resource.Bucket(...)
```

- [Bucket](./service_resource.md#bucket)
- [BucketAcl](./service_resource.md#bucketacl)
- [BucketCors](./service_resource.md#bucketcors)
- [BucketLifecycle](./service_resource.md#bucketlifecycle)
- [BucketLifecycleConfiguration](./service_resource.md#bucketlifecycleconfiguration)
- [BucketLogging](./service_resource.md#bucketlogging)
- [BucketNotification](./service_resource.md#bucketnotification)
- [BucketPolicy](./service_resource.md#bucketpolicy)
- [BucketRequestPayment](./service_resource.md#bucketrequestpayment)
- [BucketTagging](./service_resource.md#buckettagging)
- [BucketVersioning](./service_resource.md#bucketversioning)
- [BucketWebsite](./service_resource.md#bucketwebsite)
- [MultipartUpload](./service_resource.md#multipartupload)
- [MultipartUploadPart](./service_resource.md#multipartuploadpart)
- [Object](./service_resource.md#object)
- [ObjectAcl](./service_resource.md#objectacl)
- [ObjectSummary](./service_resource.md#objectsummary)
- [ObjectVersion](./service_resource.md#objectversion)





## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AnalyticsS3ExportFileFormatType usage example

from types_aiobotocore_s3.literals import AnalyticsS3ExportFileFormatType

def get_value() -> AnalyticsS3ExportFileFormatType:
    return "CSV"
```

- [AnalyticsS3ExportFileFormatType](./literals.md#analyticss3exportfileformattype)
- [ArchiveStatusType](./literals.md#archivestatustype)
- [BucketAccelerateStatusType](./literals.md#bucketacceleratestatustype)
- [BucketCannedACLType](./literals.md#bucketcannedacltype)
- [BucketExistsWaiterName](./literals.md#bucketexistswaitername)
- [BucketLocationConstraintType](./literals.md#bucketlocationconstrainttype)
- [BucketLogsPermissionType](./literals.md#bucketlogspermissiontype)
- [BucketNotExistsWaiterName](./literals.md#bucketnotexistswaitername)
- [BucketTypeType](./literals.md#buckettypetype)
- [BucketVersioningStatusType](./literals.md#bucketversioningstatustype)
- [ChecksumAlgorithmType](./literals.md#checksumalgorithmtype)
- [ChecksumModeType](./literals.md#checksummodetype)
- [CompressionTypeType](./literals.md#compressiontypetype)
- [DataRedundancyType](./literals.md#dataredundancytype)
- [DeleteMarkerReplicationStatusType](./literals.md#deletemarkerreplicationstatustype)
- [EncodingTypeType](./literals.md#encodingtypetype)
- [EventType](./literals.md#eventtype)
- [ExistingObjectReplicationStatusType](./literals.md#existingobjectreplicationstatustype)
- [ExpirationStatusType](./literals.md#expirationstatustype)
- [ExpressionTypeType](./literals.md#expressiontypetype)
- [FileHeaderInfoType](./literals.md#fileheaderinfotype)
- [FilterRuleNameType](./literals.md#filterrulenametype)
- [IntelligentTieringAccessTierType](./literals.md#intelligenttieringaccesstiertype)
- [IntelligentTieringStatusType](./literals.md#intelligenttieringstatustype)
- [InventoryFormatType](./literals.md#inventoryformattype)
- [InventoryFrequencyType](./literals.md#inventoryfrequencytype)
- [InventoryIncludedObjectVersionsType](./literals.md#inventoryincludedobjectversionstype)
- [InventoryOptionalFieldType](./literals.md#inventoryoptionalfieldtype)
- [JSONTypeType](./literals.md#jsontypetype)
- [ListBucketsPaginatorName](./literals.md#listbucketspaginatorname)
- [ListDirectoryBucketsPaginatorName](./literals.md#listdirectorybucketspaginatorname)
- [ListMultipartUploadsPaginatorName](./literals.md#listmultipartuploadspaginatorname)
- [ListObjectVersionsPaginatorName](./literals.md#listobjectversionspaginatorname)
- [ListObjectsPaginatorName](./literals.md#listobjectspaginatorname)
- [ListObjectsV2PaginatorName](./literals.md#listobjectsv2paginatorname)
- [ListPartsPaginatorName](./literals.md#listpartspaginatorname)
- [LocationTypeType](./literals.md#locationtypetype)
- [MFADeleteStatusType](./literals.md#mfadeletestatustype)
- [MFADeleteType](./literals.md#mfadeletetype)
- [MetadataDirectiveType](./literals.md#metadatadirectivetype)
- [MetricsStatusType](./literals.md#metricsstatustype)
- [ObjectAttributesType](./literals.md#objectattributestype)
- [ObjectCannedACLType](./literals.md#objectcannedacltype)
- [ObjectExistsWaiterName](./literals.md#objectexistswaitername)
- [ObjectLockEnabledType](./literals.md#objectlockenabledtype)
- [ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype)
- [ObjectLockModeType](./literals.md#objectlockmodetype)
- [ObjectLockRetentionModeType](./literals.md#objectlockretentionmodetype)
- [ObjectNotExistsWaiterName](./literals.md#objectnotexistswaitername)
- [ObjectOwnershipType](./literals.md#objectownershiptype)
- [ObjectStorageClassType](./literals.md#objectstorageclasstype)
- [ObjectVersionStorageClassType](./literals.md#objectversionstorageclasstype)
- [OptionalObjectAttributesType](./literals.md#optionalobjectattributestype)
- [OwnerOverrideType](./literals.md#owneroverridetype)
- [PartitionDateSourceType](./literals.md#partitiondatesourcetype)
- [PayerType](./literals.md#payertype)
- [PermissionType](./literals.md#permissiontype)
- [ProtocolType](./literals.md#protocoltype)
- [QuoteFieldsType](./literals.md#quotefieldstype)
- [ReplicaModificationsStatusType](./literals.md#replicamodificationsstatustype)
- [ReplicationRuleStatusType](./literals.md#replicationrulestatustype)
- [ReplicationStatusType](./literals.md#replicationstatustype)
- [ReplicationTimeStatusType](./literals.md#replicationtimestatustype)
- [RequestChargedType](./literals.md#requestchargedtype)
- [RequestPayerType](./literals.md#requestpayertype)
- [RestoreRequestTypeType](./literals.md#restorerequesttypetype)
- [ServerSideEncryptionType](./literals.md#serversideencryptiontype)
- [SessionModeType](./literals.md#sessionmodetype)
- [SseKmsEncryptedObjectsStatusType](./literals.md#ssekmsencryptedobjectsstatustype)
- [StorageClassAnalysisSchemaVersionType](./literals.md#storageclassanalysisschemaversiontype)
- [StorageClassType](./literals.md#storageclasstype)
- [TaggingDirectiveType](./literals.md#taggingdirectivetype)
- [TierType](./literals.md#tiertype)
- [TransitionDefaultMinimumObjectSizeType](./literals.md#transitiondefaultminimumobjectsizetype)
- [TransitionStorageClassType](./literals.md#transitionstorageclasstype)
- [TypeType](./literals.md#typetype)
- [S3ServiceName](./literals.md#s3servicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AbortIncompleteMultipartUploadTypeDef](./type_defs.md#abortincompletemultipartuploadtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AbortMultipartUploadRequestMultipartUploadAbortTypeDef](./type_defs.md#abortmultipartuploadrequestmultipartuploadaborttypedef)
- [AbortMultipartUploadRequestRequestTypeDef](./type_defs.md#abortmultipartuploadrequestrequesttypedef)
- [AccelerateConfigurationTypeDef](./type_defs.md#accelerateconfigurationtypedef)
- [OwnerTypeDef](./type_defs.md#ownertypedef)
- [AccessControlTranslationTypeDef](./type_defs.md#accesscontroltranslationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [AnalyticsS3BucketDestinationTypeDef](./type_defs.md#analyticss3bucketdestinationtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CopySourceTypeDef](./type_defs.md#copysourcetypedef)
- [BucketDownloadFileRequestTypeDef](./type_defs.md#bucketdownloadfilerequesttypedef)
- [FileobjTypeDef](./type_defs.md#fileobjtypedef)
- [BucketInfoTypeDef](./type_defs.md#bucketinfotypedef)
- [BucketTypeDef](./type_defs.md#buckettypedef)
- [BucketUploadFileRequestTypeDef](./type_defs.md#bucketuploadfilerequesttypedef)
- [CORSRuleTypeDef](./type_defs.md#corsruletypedef)
- [CORSRuleOutputTypeDef](./type_defs.md#corsruleoutputtypedef)
- [CSVInputTypeDef](./type_defs.md#csvinputtypedef)
- [CSVOutputTypeDef](./type_defs.md#csvoutputtypedef)
- [ChecksumTypeDef](./type_defs.md#checksumtypedef)
- [ClientDownloadFileRequestTypeDef](./type_defs.md#clientdownloadfilerequesttypedef)
- [ClientGeneratePresignedPostRequestTypeDef](./type_defs.md#clientgeneratepresignedpostrequesttypedef)
- [ClientUploadFileRequestTypeDef](./type_defs.md#clientuploadfilerequesttypedef)
- [CloudFunctionConfigurationOutputTypeDef](./type_defs.md#cloudfunctionconfigurationoutputtypedef)
- [CloudFunctionConfigurationTypeDef](./type_defs.md#cloudfunctionconfigurationtypedef)
- [CommonPrefixTypeDef](./type_defs.md#commonprefixtypedef)
- [CompletedPartTypeDef](./type_defs.md#completedparttypedef)
- [ConditionTypeDef](./type_defs.md#conditiontypedef)
- [CopyObjectResultTypeDef](./type_defs.md#copyobjectresulttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [CopyPartResultTypeDef](./type_defs.md#copypartresulttypedef)
- [LocationInfoTypeDef](./type_defs.md#locationinfotypedef)
- [SessionCredentialsTypeDef](./type_defs.md#sessioncredentialstypedef)
- [CreateSessionRequestRequestTypeDef](./type_defs.md#createsessionrequestrequesttypedef)
- [DefaultRetentionTypeDef](./type_defs.md#defaultretentiontypedef)
- [DeleteBucketAnalyticsConfigurationRequestRequestTypeDef](./type_defs.md#deletebucketanalyticsconfigurationrequestrequesttypedef)
- [DeleteBucketCorsRequestBucketCorsDeleteTypeDef](./type_defs.md#deletebucketcorsrequestbucketcorsdeletetypedef)
- [DeleteBucketCorsRequestRequestTypeDef](./type_defs.md#deletebucketcorsrequestrequesttypedef)
- [DeleteBucketEncryptionRequestRequestTypeDef](./type_defs.md#deletebucketencryptionrequestrequesttypedef)
- [DeleteBucketIntelligentTieringConfigurationRequestRequestTypeDef](./type_defs.md#deletebucketintelligenttieringconfigurationrequestrequesttypedef)
- [DeleteBucketInventoryConfigurationRequestRequestTypeDef](./type_defs.md#deletebucketinventoryconfigurationrequestrequesttypedef)
- [DeleteBucketLifecycleRequestBucketLifecycleConfigurationDeleteTypeDef](./type_defs.md#deletebucketlifecyclerequestbucketlifecycleconfigurationdeletetypedef)
- [DeleteBucketLifecycleRequestBucketLifecycleDeleteTypeDef](./type_defs.md#deletebucketlifecyclerequestbucketlifecycledeletetypedef)
- [DeleteBucketLifecycleRequestRequestTypeDef](./type_defs.md#deletebucketlifecyclerequestrequesttypedef)
- [DeleteBucketMetricsConfigurationRequestRequestTypeDef](./type_defs.md#deletebucketmetricsconfigurationrequestrequesttypedef)
- [DeleteBucketOwnershipControlsRequestRequestTypeDef](./type_defs.md#deletebucketownershipcontrolsrequestrequesttypedef)
- [DeleteBucketPolicyRequestBucketPolicyDeleteTypeDef](./type_defs.md#deletebucketpolicyrequestbucketpolicydeletetypedef)
- [DeleteBucketPolicyRequestRequestTypeDef](./type_defs.md#deletebucketpolicyrequestrequesttypedef)
- [DeleteBucketReplicationRequestRequestTypeDef](./type_defs.md#deletebucketreplicationrequestrequesttypedef)
- [DeleteBucketRequestBucketDeleteTypeDef](./type_defs.md#deletebucketrequestbucketdeletetypedef)
- [DeleteBucketRequestRequestTypeDef](./type_defs.md#deletebucketrequestrequesttypedef)
- [DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef](./type_defs.md#deletebuckettaggingrequestbuckettaggingdeletetypedef)
- [DeleteBucketTaggingRequestRequestTypeDef](./type_defs.md#deletebuckettaggingrequestrequesttypedef)
- [DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef](./type_defs.md#deletebucketwebsiterequestbucketwebsitedeletetypedef)
- [DeleteBucketWebsiteRequestRequestTypeDef](./type_defs.md#deletebucketwebsiterequestrequesttypedef)
- [DeleteMarkerReplicationTypeDef](./type_defs.md#deletemarkerreplicationtypedef)
- [DeleteObjectRequestObjectDeleteTypeDef](./type_defs.md#deleteobjectrequestobjectdeletetypedef)
- [DeleteObjectRequestObjectSummaryDeleteTypeDef](./type_defs.md#deleteobjectrequestobjectsummarydeletetypedef)
- [DeleteObjectRequestObjectVersionDeleteTypeDef](./type_defs.md#deleteobjectrequestobjectversiondeletetypedef)
- [DeleteObjectRequestRequestTypeDef](./type_defs.md#deleteobjectrequestrequesttypedef)
- [DeleteObjectTaggingRequestRequestTypeDef](./type_defs.md#deleteobjecttaggingrequestrequesttypedef)
- [DeletedObjectTypeDef](./type_defs.md#deletedobjecttypedef)
- [ErrorTypeDef](./type_defs.md#errortypedef)
- [DeletePublicAccessBlockRequestRequestTypeDef](./type_defs.md#deletepublicaccessblockrequestrequesttypedef)
- [ObjectIdentifierTypeDef](./type_defs.md#objectidentifiertypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [EncryptionTypeDef](./type_defs.md#encryptiontypedef)
- [ErrorDocumentTypeDef](./type_defs.md#errordocumenttypedef)
- [ExistingObjectReplicationTypeDef](./type_defs.md#existingobjectreplicationtypedef)
- [FilterRuleTypeDef](./type_defs.md#filterruletypedef)
- [GetBucketAccelerateConfigurationRequestRequestTypeDef](./type_defs.md#getbucketaccelerateconfigurationrequestrequesttypedef)
- [GetBucketAclRequestRequestTypeDef](./type_defs.md#getbucketaclrequestrequesttypedef)
- [GetBucketAnalyticsConfigurationRequestRequestTypeDef](./type_defs.md#getbucketanalyticsconfigurationrequestrequesttypedef)
- [GetBucketCorsRequestRequestTypeDef](./type_defs.md#getbucketcorsrequestrequesttypedef)
- [GetBucketEncryptionRequestRequestTypeDef](./type_defs.md#getbucketencryptionrequestrequesttypedef)
- [GetBucketIntelligentTieringConfigurationRequestRequestTypeDef](./type_defs.md#getbucketintelligenttieringconfigurationrequestrequesttypedef)
- [GetBucketInventoryConfigurationRequestRequestTypeDef](./type_defs.md#getbucketinventoryconfigurationrequestrequesttypedef)
- [GetBucketLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#getbucketlifecycleconfigurationrequestrequesttypedef)
- [GetBucketLifecycleRequestRequestTypeDef](./type_defs.md#getbucketlifecyclerequestrequesttypedef)
- [GetBucketLocationRequestRequestTypeDef](./type_defs.md#getbucketlocationrequestrequesttypedef)
- [GetBucketLoggingRequestRequestTypeDef](./type_defs.md#getbucketloggingrequestrequesttypedef)
- [GetBucketMetricsConfigurationRequestRequestTypeDef](./type_defs.md#getbucketmetricsconfigurationrequestrequesttypedef)
- [GetBucketNotificationConfigurationRequestRequestTypeDef](./type_defs.md#getbucketnotificationconfigurationrequestrequesttypedef)
- [GetBucketOwnershipControlsRequestRequestTypeDef](./type_defs.md#getbucketownershipcontrolsrequestrequesttypedef)
- [GetBucketPolicyRequestRequestTypeDef](./type_defs.md#getbucketpolicyrequestrequesttypedef)
- [PolicyStatusTypeDef](./type_defs.md#policystatustypedef)
- [GetBucketPolicyStatusRequestRequestTypeDef](./type_defs.md#getbucketpolicystatusrequestrequesttypedef)
- [GetBucketReplicationRequestRequestTypeDef](./type_defs.md#getbucketreplicationrequestrequesttypedef)
- [GetBucketRequestPaymentRequestRequestTypeDef](./type_defs.md#getbucketrequestpaymentrequestrequesttypedef)
- [GetBucketTaggingRequestRequestTypeDef](./type_defs.md#getbuckettaggingrequestrequesttypedef)
- [GetBucketVersioningRequestRequestTypeDef](./type_defs.md#getbucketversioningrequestrequesttypedef)
- [IndexDocumentTypeDef](./type_defs.md#indexdocumenttypedef)
- [RedirectAllRequestsToTypeDef](./type_defs.md#redirectallrequeststotypedef)
- [GetBucketWebsiteRequestRequestTypeDef](./type_defs.md#getbucketwebsiterequestrequesttypedef)
- [GetObjectAclRequestRequestTypeDef](./type_defs.md#getobjectaclrequestrequesttypedef)
- [ObjectPartTypeDef](./type_defs.md#objectparttypedef)
- [GetObjectAttributesRequestRequestTypeDef](./type_defs.md#getobjectattributesrequestrequesttypedef)
- [ObjectLockLegalHoldTypeDef](./type_defs.md#objectlocklegalholdtypedef)
- [GetObjectLegalHoldRequestRequestTypeDef](./type_defs.md#getobjectlegalholdrequestrequesttypedef)
- [GetObjectLockConfigurationRequestRequestTypeDef](./type_defs.md#getobjectlockconfigurationrequestrequesttypedef)
- [ObjectLockRetentionOutputTypeDef](./type_defs.md#objectlockretentionoutputtypedef)
- [GetObjectRetentionRequestRequestTypeDef](./type_defs.md#getobjectretentionrequestrequesttypedef)
- [GetObjectTaggingRequestRequestTypeDef](./type_defs.md#getobjecttaggingrequestrequesttypedef)
- [GetObjectTorrentRequestRequestTypeDef](./type_defs.md#getobjecttorrentrequestrequesttypedef)
- [PublicAccessBlockConfigurationTypeDef](./type_defs.md#publicaccessblockconfigurationtypedef)
- [GetPublicAccessBlockRequestRequestTypeDef](./type_defs.md#getpublicaccessblockrequestrequesttypedef)
- [GlacierJobParametersTypeDef](./type_defs.md#glacierjobparameterstypedef)
- [GranteeTypeDef](./type_defs.md#granteetypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [HeadBucketRequestRequestTypeDef](./type_defs.md#headbucketrequestrequesttypedef)
- [InitiatorTypeDef](./type_defs.md#initiatortypedef)
- [JSONInputTypeDef](./type_defs.md#jsoninputtypedef)
- [TieringTypeDef](./type_defs.md#tieringtypedef)
- [InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef)
- [InventoryScheduleTypeDef](./type_defs.md#inventoryscheduletypedef)
- [SSEKMSTypeDef](./type_defs.md#ssekmstypedef)
- [JSONOutputTypeDef](./type_defs.md#jsonoutputtypedef)
- [LifecycleExpirationOutputTypeDef](./type_defs.md#lifecycleexpirationoutputtypedef)
- [NoncurrentVersionExpirationTypeDef](./type_defs.md#noncurrentversionexpirationtypedef)
- [NoncurrentVersionTransitionTypeDef](./type_defs.md#noncurrentversiontransitiontypedef)
- [TransitionOutputTypeDef](./type_defs.md#transitionoutputtypedef)
- [ListBucketAnalyticsConfigurationsRequestRequestTypeDef](./type_defs.md#listbucketanalyticsconfigurationsrequestrequesttypedef)
- [ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef](./type_defs.md#listbucketintelligenttieringconfigurationsrequestrequesttypedef)
- [ListBucketInventoryConfigurationsRequestRequestTypeDef](./type_defs.md#listbucketinventoryconfigurationsrequestrequesttypedef)
- [ListBucketMetricsConfigurationsRequestRequestTypeDef](./type_defs.md#listbucketmetricsconfigurationsrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListBucketsRequestRequestTypeDef](./type_defs.md#listbucketsrequestrequesttypedef)
- [ListDirectoryBucketsRequestRequestTypeDef](./type_defs.md#listdirectorybucketsrequestrequesttypedef)
- [ListMultipartUploadsRequestRequestTypeDef](./type_defs.md#listmultipartuploadsrequestrequesttypedef)
- [ListObjectVersionsRequestRequestTypeDef](./type_defs.md#listobjectversionsrequestrequesttypedef)
- [ListObjectsRequestRequestTypeDef](./type_defs.md#listobjectsrequestrequesttypedef)
- [ListObjectsV2RequestRequestTypeDef](./type_defs.md#listobjectsv2requestrequesttypedef)
- [PartTypeDef](./type_defs.md#parttypedef)
- [ListPartsRequestRequestTypeDef](./type_defs.md#listpartsrequestrequesttypedef)
- [MetadataEntryTypeDef](./type_defs.md#metadataentrytypedef)
- [ReplicationTimeValueTypeDef](./type_defs.md#replicationtimevaluetypedef)
- [QueueConfigurationDeprecatedOutputTypeDef](./type_defs.md#queueconfigurationdeprecatedoutputtypedef)
- [TopicConfigurationDeprecatedOutputTypeDef](./type_defs.md#topicconfigurationdeprecatedoutputtypedef)
- [ObjectDownloadFileRequestTypeDef](./type_defs.md#objectdownloadfilerequesttypedef)
- [RestoreStatusTypeDef](./type_defs.md#restorestatustypedef)
- [ObjectUploadFileRequestTypeDef](./type_defs.md#objectuploadfilerequesttypedef)
- [OwnershipControlsRuleTypeDef](./type_defs.md#ownershipcontrolsruletypedef)
- [PartitionedPrefixTypeDef](./type_defs.md#partitionedprefixtypedef)
- [ProgressTypeDef](./type_defs.md#progresstypedef)
- [PutBucketPolicyRequestBucketPolicyPutTypeDef](./type_defs.md#putbucketpolicyrequestbucketpolicyputtypedef)
- [PutBucketPolicyRequestRequestTypeDef](./type_defs.md#putbucketpolicyrequestrequesttypedef)
- [RequestPaymentConfigurationTypeDef](./type_defs.md#requestpaymentconfigurationtypedef)
- [PutBucketVersioningRequestBucketVersioningEnableTypeDef](./type_defs.md#putbucketversioningrequestbucketversioningenabletypedef)
- [VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef)
- [PutBucketVersioningRequestBucketVersioningSuspendTypeDef](./type_defs.md#putbucketversioningrequestbucketversioningsuspendtypedef)
- [QueueConfigurationDeprecatedTypeDef](./type_defs.md#queueconfigurationdeprecatedtypedef)
- [RecordsEventTypeDef](./type_defs.md#recordseventtypedef)
- [RedirectTypeDef](./type_defs.md#redirecttypedef)
- [ReplicaModificationsTypeDef](./type_defs.md#replicamodificationstypedef)
- [RequestProgressTypeDef](./type_defs.md#requestprogresstypedef)
- [ScanRangeTypeDef](./type_defs.md#scanrangetypedef)
- [ServerSideEncryptionByDefaultTypeDef](./type_defs.md#serversideencryptionbydefaulttypedef)
- [SseKmsEncryptedObjectsTypeDef](./type_defs.md#ssekmsencryptedobjectstypedef)
- [StatsTypeDef](./type_defs.md#statstypedef)
- [TopicConfigurationDeprecatedTypeDef](./type_defs.md#topicconfigurationdeprecatedtypedef)
- [AbortMultipartUploadOutputTypeDef](./type_defs.md#abortmultipartuploadoutputtypedef)
- [CompleteMultipartUploadOutputTypeDef](./type_defs.md#completemultipartuploadoutputtypedef)
- [CreateBucketOutputTypeDef](./type_defs.md#createbucketoutputtypedef)
- [CreateMultipartUploadOutputTypeDef](./type_defs.md#createmultipartuploadoutputtypedef)
- [DeleteObjectOutputTypeDef](./type_defs.md#deleteobjectoutputtypedef)
- [DeleteObjectTaggingOutputTypeDef](./type_defs.md#deleteobjecttaggingoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetBucketAccelerateConfigurationOutputTypeDef](./type_defs.md#getbucketaccelerateconfigurationoutputtypedef)
- [GetBucketLocationOutputTypeDef](./type_defs.md#getbucketlocationoutputtypedef)
- [GetBucketPolicyOutputTypeDef](./type_defs.md#getbucketpolicyoutputtypedef)
- [GetBucketRequestPaymentOutputTypeDef](./type_defs.md#getbucketrequestpaymentoutputtypedef)
- [GetBucketVersioningOutputTypeDef](./type_defs.md#getbucketversioningoutputtypedef)
- [GetObjectOutputTypeDef](./type_defs.md#getobjectoutputtypedef)
- [GetObjectTorrentOutputTypeDef](./type_defs.md#getobjecttorrentoutputtypedef)
- [HeadBucketOutputTypeDef](./type_defs.md#headbucketoutputtypedef)
- [HeadObjectOutputTypeDef](./type_defs.md#headobjectoutputtypedef)
- [PutBucketLifecycleConfigurationOutputTypeDef](./type_defs.md#putbucketlifecycleconfigurationoutputtypedef)
- [PutObjectAclOutputTypeDef](./type_defs.md#putobjectacloutputtypedef)
- [PutObjectLegalHoldOutputTypeDef](./type_defs.md#putobjectlegalholdoutputtypedef)
- [PutObjectLockConfigurationOutputTypeDef](./type_defs.md#putobjectlockconfigurationoutputtypedef)
- [PutObjectOutputTypeDef](./type_defs.md#putobjectoutputtypedef)
- [PutObjectRetentionOutputTypeDef](./type_defs.md#putobjectretentionoutputtypedef)
- [PutObjectTaggingOutputTypeDef](./type_defs.md#putobjecttaggingoutputtypedef)
- [RestoreObjectOutputTypeDef](./type_defs.md#restoreobjectoutputtypedef)
- [UploadPartOutputTypeDef](./type_defs.md#uploadpartoutputtypedef)
- [PutBucketAccelerateConfigurationRequestRequestTypeDef](./type_defs.md#putbucketaccelerateconfigurationrequestrequesttypedef)
- [DeleteMarkerEntryTypeDef](./type_defs.md#deletemarkerentrytypedef)
- [AnalyticsAndOperatorOutputTypeDef](./type_defs.md#analyticsandoperatoroutputtypedef)
- [AnalyticsAndOperatorTypeDef](./type_defs.md#analyticsandoperatortypedef)
- [GetBucketTaggingOutputTypeDef](./type_defs.md#getbuckettaggingoutputtypedef)
- [GetObjectTaggingOutputTypeDef](./type_defs.md#getobjecttaggingoutputtypedef)
- [IntelligentTieringAndOperatorOutputTypeDef](./type_defs.md#intelligenttieringandoperatoroutputtypedef)
- [IntelligentTieringAndOperatorTypeDef](./type_defs.md#intelligenttieringandoperatortypedef)
- [LifecycleRuleAndOperatorOutputTypeDef](./type_defs.md#lifecycleruleandoperatoroutputtypedef)
- [LifecycleRuleAndOperatorTypeDef](./type_defs.md#lifecycleruleandoperatortypedef)
- [MetricsAndOperatorOutputTypeDef](./type_defs.md#metricsandoperatoroutputtypedef)
- [MetricsAndOperatorTypeDef](./type_defs.md#metricsandoperatortypedef)
- [ReplicationRuleAndOperatorOutputTypeDef](./type_defs.md#replicationruleandoperatoroutputtypedef)
- [ReplicationRuleAndOperatorTypeDef](./type_defs.md#replicationruleandoperatortypedef)
- [TaggingTypeDef](./type_defs.md#taggingtypedef)
- [AnalyticsExportDestinationTypeDef](./type_defs.md#analyticsexportdestinationtypedef)
- [UploadPartRequestMultipartUploadPartUploadTypeDef](./type_defs.md#uploadpartrequestmultipartuploadpartuploadtypedef)
- [UploadPartRequestRequestTypeDef](./type_defs.md#uploadpartrequestrequesttypedef)
- [BucketCopyRequestTypeDef](./type_defs.md#bucketcopyrequesttypedef)
- [ClientCopyRequestTypeDef](./type_defs.md#clientcopyrequesttypedef)
- [CopySourceOrStrTypeDef](./type_defs.md#copysourceorstrtypedef)
- [ObjectCopyRequestTypeDef](./type_defs.md#objectcopyrequesttypedef)
- [BucketDownloadFileobjRequestTypeDef](./type_defs.md#bucketdownloadfileobjrequesttypedef)
- [BucketUploadFileobjRequestTypeDef](./type_defs.md#bucketuploadfileobjrequesttypedef)
- [ClientDownloadFileobjRequestTypeDef](./type_defs.md#clientdownloadfileobjrequesttypedef)
- [ClientUploadFileobjRequestTypeDef](./type_defs.md#clientuploadfileobjrequesttypedef)
- [ObjectDownloadFileobjRequestTypeDef](./type_defs.md#objectdownloadfileobjrequesttypedef)
- [ObjectUploadFileobjRequestTypeDef](./type_defs.md#objectuploadfileobjrequesttypedef)
- [ListBucketsOutputTypeDef](./type_defs.md#listbucketsoutputtypedef)
- [ListDirectoryBucketsOutputTypeDef](./type_defs.md#listdirectorybucketsoutputtypedef)
- [CORSConfigurationTypeDef](./type_defs.md#corsconfigurationtypedef)
- [GetBucketCorsOutputTypeDef](./type_defs.md#getbucketcorsoutputtypedef)
- [CloudFunctionConfigurationUnionTypeDef](./type_defs.md#cloudfunctionconfigurationuniontypedef)
- [CompletedMultipartUploadTypeDef](./type_defs.md#completedmultipartuploadtypedef)
- [CopyObjectOutputTypeDef](./type_defs.md#copyobjectoutputtypedef)
- [CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef](./type_defs.md#createmultipartuploadrequestobjectinitiatemultipartuploadtypedef)
- [CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef](./type_defs.md#createmultipartuploadrequestobjectsummaryinitiatemultipartuploadtypedef)
- [CreateMultipartUploadRequestRequestTypeDef](./type_defs.md#createmultipartuploadrequestrequesttypedef)
- [GetObjectRequestObjectGetTypeDef](./type_defs.md#getobjectrequestobjectgettypedef)
- [GetObjectRequestObjectSummaryGetTypeDef](./type_defs.md#getobjectrequestobjectsummarygettypedef)
- [GetObjectRequestObjectVersionGetTypeDef](./type_defs.md#getobjectrequestobjectversiongettypedef)
- [GetObjectRequestRequestTypeDef](./type_defs.md#getobjectrequestrequesttypedef)
- [HeadObjectRequestObjectVersionHeadTypeDef](./type_defs.md#headobjectrequestobjectversionheadtypedef)
- [HeadObjectRequestRequestTypeDef](./type_defs.md#headobjectrequestrequesttypedef)
- [LifecycleExpirationTypeDef](./type_defs.md#lifecycleexpirationtypedef)
- [ObjectLockRetentionTypeDef](./type_defs.md#objectlockretentiontypedef)
- [PutObjectRequestBucketPutObjectTypeDef](./type_defs.md#putobjectrequestbucketputobjecttypedef)
- [PutObjectRequestObjectPutTypeDef](./type_defs.md#putobjectrequestobjectputtypedef)
- [PutObjectRequestObjectSummaryPutTypeDef](./type_defs.md#putobjectrequestobjectsummaryputtypedef)
- [PutObjectRequestRequestTypeDef](./type_defs.md#putobjectrequestrequesttypedef)
- [TransitionTypeDef](./type_defs.md#transitiontypedef)
- [WriteGetObjectResponseRequestRequestTypeDef](./type_defs.md#writegetobjectresponserequestrequesttypedef)
- [UploadPartCopyOutputTypeDef](./type_defs.md#uploadpartcopyoutputtypedef)
- [CreateBucketConfigurationTypeDef](./type_defs.md#createbucketconfigurationtypedef)
- [CreateSessionOutputTypeDef](./type_defs.md#createsessionoutputtypedef)
- [ObjectLockRuleTypeDef](./type_defs.md#objectlockruletypedef)
- [DeleteObjectsOutputTypeDef](./type_defs.md#deleteobjectsoutputtypedef)
- [DeleteTypeDef](./type_defs.md#deletetypedef)
- [S3KeyFilterOutputTypeDef](./type_defs.md#s3keyfilteroutputtypedef)
- [S3KeyFilterTypeDef](./type_defs.md#s3keyfiltertypedef)
- [GetBucketPolicyStatusOutputTypeDef](./type_defs.md#getbucketpolicystatusoutputtypedef)
- [GetObjectAttributesPartsTypeDef](./type_defs.md#getobjectattributespartstypedef)
- [GetObjectLegalHoldOutputTypeDef](./type_defs.md#getobjectlegalholdoutputtypedef)
- [PutObjectLegalHoldRequestRequestTypeDef](./type_defs.md#putobjectlegalholdrequestrequesttypedef)
- [GetObjectRetentionOutputTypeDef](./type_defs.md#getobjectretentionoutputtypedef)
- [GetPublicAccessBlockOutputTypeDef](./type_defs.md#getpublicaccessblockoutputtypedef)
- [PutPublicAccessBlockRequestRequestTypeDef](./type_defs.md#putpublicaccessblockrequestrequesttypedef)
- [GrantTypeDef](./type_defs.md#granttypedef)
- [TargetGrantTypeDef](./type_defs.md#targetgranttypedef)
- [HeadBucketRequestBucketExistsWaitTypeDef](./type_defs.md#headbucketrequestbucketexistswaittypedef)
- [HeadBucketRequestBucketNotExistsWaitTypeDef](./type_defs.md#headbucketrequestbucketnotexistswaittypedef)
- [HeadObjectRequestObjectExistsWaitTypeDef](./type_defs.md#headobjectrequestobjectexistswaittypedef)
- [HeadObjectRequestObjectNotExistsWaitTypeDef](./type_defs.md#headobjectrequestobjectnotexistswaittypedef)
- [MultipartUploadTypeDef](./type_defs.md#multipartuploadtypedef)
- [InputSerializationTypeDef](./type_defs.md#inputserializationtypedef)
- [InventoryEncryptionOutputTypeDef](./type_defs.md#inventoryencryptionoutputtypedef)
- [InventoryEncryptionTypeDef](./type_defs.md#inventoryencryptiontypedef)
- [OutputSerializationTypeDef](./type_defs.md#outputserializationtypedef)
- [RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef)
- [ListBucketsRequestListBucketsPaginateTypeDef](./type_defs.md#listbucketsrequestlistbucketspaginatetypedef)
- [ListDirectoryBucketsRequestListDirectoryBucketsPaginateTypeDef](./type_defs.md#listdirectorybucketsrequestlistdirectorybucketspaginatetypedef)
- [ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef](./type_defs.md#listmultipartuploadsrequestlistmultipartuploadspaginatetypedef)
- [ListObjectVersionsRequestListObjectVersionsPaginateTypeDef](./type_defs.md#listobjectversionsrequestlistobjectversionspaginatetypedef)
- [ListObjectsRequestListObjectsPaginateTypeDef](./type_defs.md#listobjectsrequestlistobjectspaginatetypedef)
- [ListObjectsV2RequestListObjectsV2PaginateTypeDef](./type_defs.md#listobjectsv2requestlistobjectsv2paginatetypedef)
- [ListPartsRequestListPartsPaginateTypeDef](./type_defs.md#listpartsrequestlistpartspaginatetypedef)
- [ListPartsOutputTypeDef](./type_defs.md#listpartsoutputtypedef)
- [MetricsTypeDef](./type_defs.md#metricstypedef)
- [ReplicationTimeTypeDef](./type_defs.md#replicationtimetypedef)
- [NotificationConfigurationDeprecatedResponseTypeDef](./type_defs.md#notificationconfigurationdeprecatedresponsetypedef)
- [ObjectTypeDef](./type_defs.md#objecttypedef)
- [ObjectVersionTypeDef](./type_defs.md#objectversiontypedef)
- [OwnershipControlsOutputTypeDef](./type_defs.md#ownershipcontrolsoutputtypedef)
- [OwnershipControlsTypeDef](./type_defs.md#ownershipcontrolstypedef)
- [TargetObjectKeyFormatOutputTypeDef](./type_defs.md#targetobjectkeyformatoutputtypedef)
- [TargetObjectKeyFormatTypeDef](./type_defs.md#targetobjectkeyformattypedef)
- [ProgressEventTypeDef](./type_defs.md#progresseventtypedef)
- [PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef](./type_defs.md#putbucketrequestpaymentrequestbucketrequestpaymentputtypedef)
- [PutBucketRequestPaymentRequestRequestTypeDef](./type_defs.md#putbucketrequestpaymentrequestrequesttypedef)
- [PutBucketVersioningRequestBucketVersioningPutTypeDef](./type_defs.md#putbucketversioningrequestbucketversioningputtypedef)
- [PutBucketVersioningRequestRequestTypeDef](./type_defs.md#putbucketversioningrequestrequesttypedef)
- [QueueConfigurationDeprecatedUnionTypeDef](./type_defs.md#queueconfigurationdeprecateduniontypedef)
- [RoutingRuleTypeDef](./type_defs.md#routingruletypedef)
- [ServerSideEncryptionRuleTypeDef](./type_defs.md#serversideencryptionruletypedef)
- [SourceSelectionCriteriaTypeDef](./type_defs.md#sourceselectioncriteriatypedef)
- [StatsEventTypeDef](./type_defs.md#statseventtypedef)
- [TopicConfigurationDeprecatedUnionTypeDef](./type_defs.md#topicconfigurationdeprecateduniontypedef)
- [AnalyticsFilterOutputTypeDef](./type_defs.md#analyticsfilteroutputtypedef)
- [AnalyticsAndOperatorUnionTypeDef](./type_defs.md#analyticsandoperatoruniontypedef)
- [IntelligentTieringFilterOutputTypeDef](./type_defs.md#intelligenttieringfilteroutputtypedef)
- [IntelligentTieringAndOperatorUnionTypeDef](./type_defs.md#intelligenttieringandoperatoruniontypedef)
- [LifecycleRuleFilterOutputTypeDef](./type_defs.md#lifecyclerulefilteroutputtypedef)
- [LifecycleRuleFilterTypeDef](./type_defs.md#lifecyclerulefiltertypedef)
- [MetricsFilterOutputTypeDef](./type_defs.md#metricsfilteroutputtypedef)
- [MetricsAndOperatorUnionTypeDef](./type_defs.md#metricsandoperatoruniontypedef)
- [ReplicationRuleFilterOutputTypeDef](./type_defs.md#replicationrulefilteroutputtypedef)
- [ReplicationRuleAndOperatorUnionTypeDef](./type_defs.md#replicationruleandoperatoruniontypedef)
- [PutBucketTaggingRequestBucketTaggingPutTypeDef](./type_defs.md#putbuckettaggingrequestbuckettaggingputtypedef)
- [PutBucketTaggingRequestRequestTypeDef](./type_defs.md#putbuckettaggingrequestrequesttypedef)
- [PutObjectTaggingRequestRequestTypeDef](./type_defs.md#putobjecttaggingrequestrequesttypedef)
- [StorageClassAnalysisDataExportTypeDef](./type_defs.md#storageclassanalysisdataexporttypedef)
- [CopyObjectRequestObjectCopyFromTypeDef](./type_defs.md#copyobjectrequestobjectcopyfromtypedef)
- [CopyObjectRequestObjectSummaryCopyFromTypeDef](./type_defs.md#copyobjectrequestobjectsummarycopyfromtypedef)
- [CopyObjectRequestRequestTypeDef](./type_defs.md#copyobjectrequestrequesttypedef)
- [UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef](./type_defs.md#uploadpartcopyrequestmultipartuploadpartcopyfromtypedef)
- [UploadPartCopyRequestRequestTypeDef](./type_defs.md#uploadpartcopyrequestrequesttypedef)
- [PutBucketCorsRequestBucketCorsPutTypeDef](./type_defs.md#putbucketcorsrequestbucketcorsputtypedef)
- [PutBucketCorsRequestRequestTypeDef](./type_defs.md#putbucketcorsrequestrequesttypedef)
- [CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef](./type_defs.md#completemultipartuploadrequestmultipartuploadcompletetypedef)
- [CompleteMultipartUploadRequestRequestTypeDef](./type_defs.md#completemultipartuploadrequestrequesttypedef)
- [PutObjectRetentionRequestRequestTypeDef](./type_defs.md#putobjectretentionrequestrequesttypedef)
- [RuleTypeDef](./type_defs.md#ruletypedef)
- [CreateBucketRequestBucketCreateTypeDef](./type_defs.md#createbucketrequestbucketcreatetypedef)
- [CreateBucketRequestRequestTypeDef](./type_defs.md#createbucketrequestrequesttypedef)
- [CreateBucketRequestServiceResourceCreateBucketTypeDef](./type_defs.md#createbucketrequestserviceresourcecreatebuckettypedef)
- [ObjectLockConfigurationTypeDef](./type_defs.md#objectlockconfigurationtypedef)
- [DeleteObjectsRequestBucketDeleteObjectsTypeDef](./type_defs.md#deleteobjectsrequestbucketdeleteobjectstypedef)
- [DeleteObjectsRequestRequestTypeDef](./type_defs.md#deleteobjectsrequestrequesttypedef)
- [NotificationConfigurationFilterOutputTypeDef](./type_defs.md#notificationconfigurationfilteroutputtypedef)
- [NotificationConfigurationFilterTypeDef](./type_defs.md#notificationconfigurationfiltertypedef)
- [GetObjectAttributesOutputTypeDef](./type_defs.md#getobjectattributesoutputtypedef)
- [AccessControlPolicyTypeDef](./type_defs.md#accesscontrolpolicytypedef)
- [GetBucketAclOutputTypeDef](./type_defs.md#getbucketacloutputtypedef)
- [GetObjectAclOutputTypeDef](./type_defs.md#getobjectacloutputtypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [ListMultipartUploadsOutputTypeDef](./type_defs.md#listmultipartuploadsoutputtypedef)
- [InventoryS3BucketDestinationOutputTypeDef](./type_defs.md#inventorys3bucketdestinationoutputtypedef)
- [InventoryEncryptionUnionTypeDef](./type_defs.md#inventoryencryptionuniontypedef)
- [SelectObjectContentRequestRequestTypeDef](./type_defs.md#selectobjectcontentrequestrequesttypedef)
- [SelectParametersTypeDef](./type_defs.md#selectparameterstypedef)
- [GetBucketLifecycleOutputTypeDef](./type_defs.md#getbucketlifecycleoutputtypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [ListObjectsOutputTypeDef](./type_defs.md#listobjectsoutputtypedef)
- [ListObjectsV2OutputTypeDef](./type_defs.md#listobjectsv2outputtypedef)
- [ListObjectVersionsOutputTypeDef](./type_defs.md#listobjectversionsoutputtypedef)
- [GetBucketOwnershipControlsOutputTypeDef](./type_defs.md#getbucketownershipcontrolsoutputtypedef)
- [PutBucketOwnershipControlsRequestRequestTypeDef](./type_defs.md#putbucketownershipcontrolsrequestrequesttypedef)
- [LoggingEnabledOutputTypeDef](./type_defs.md#loggingenabledoutputtypedef)
- [LoggingEnabledTypeDef](./type_defs.md#loggingenabledtypedef)
- [GetBucketWebsiteOutputTypeDef](./type_defs.md#getbucketwebsiteoutputtypedef)
- [WebsiteConfigurationTypeDef](./type_defs.md#websiteconfigurationtypedef)
- [ServerSideEncryptionConfigurationOutputTypeDef](./type_defs.md#serversideencryptionconfigurationoutputtypedef)
- [ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef)
- [SelectObjectContentEventStreamTypeDef](./type_defs.md#selectobjectcontenteventstreamtypedef)
- [NotificationConfigurationDeprecatedTypeDef](./type_defs.md#notificationconfigurationdeprecatedtypedef)
- [AnalyticsFilterTypeDef](./type_defs.md#analyticsfiltertypedef)
- [IntelligentTieringConfigurationOutputTypeDef](./type_defs.md#intelligenttieringconfigurationoutputtypedef)
- [IntelligentTieringFilterTypeDef](./type_defs.md#intelligenttieringfiltertypedef)
- [LifecycleRuleOutputTypeDef](./type_defs.md#lifecycleruleoutputtypedef)
- [LifecycleRuleTypeDef](./type_defs.md#lifecycleruletypedef)
- [MetricsConfigurationOutputTypeDef](./type_defs.md#metricsconfigurationoutputtypedef)
- [MetricsFilterTypeDef](./type_defs.md#metricsfiltertypedef)
- [ReplicationRuleFilterTypeDef](./type_defs.md#replicationrulefiltertypedef)
- [StorageClassAnalysisTypeDef](./type_defs.md#storageclassanalysistypedef)
- [LifecycleConfigurationTypeDef](./type_defs.md#lifecycleconfigurationtypedef)
- [GetObjectLockConfigurationOutputTypeDef](./type_defs.md#getobjectlockconfigurationoutputtypedef)
- [PutObjectLockConfigurationRequestRequestTypeDef](./type_defs.md#putobjectlockconfigurationrequestrequesttypedef)
- [LambdaFunctionConfigurationOutputTypeDef](./type_defs.md#lambdafunctionconfigurationoutputtypedef)
- [QueueConfigurationOutputTypeDef](./type_defs.md#queueconfigurationoutputtypedef)
- [TopicConfigurationOutputTypeDef](./type_defs.md#topicconfigurationoutputtypedef)
- [LambdaFunctionConfigurationTypeDef](./type_defs.md#lambdafunctionconfigurationtypedef)
- [QueueConfigurationTypeDef](./type_defs.md#queueconfigurationtypedef)
- [TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef)
- [PutBucketAclRequestBucketAclPutTypeDef](./type_defs.md#putbucketaclrequestbucketaclputtypedef)
- [PutBucketAclRequestRequestTypeDef](./type_defs.md#putbucketaclrequestrequesttypedef)
- [PutObjectAclRequestObjectAclPutTypeDef](./type_defs.md#putobjectaclrequestobjectaclputtypedef)
- [PutObjectAclRequestRequestTypeDef](./type_defs.md#putobjectaclrequestrequesttypedef)
- [OutputLocationTypeDef](./type_defs.md#outputlocationtypedef)
- [InventoryDestinationOutputTypeDef](./type_defs.md#inventorydestinationoutputtypedef)
- [InventoryS3BucketDestinationTypeDef](./type_defs.md#inventorys3bucketdestinationtypedef)
- [ReplicationRuleOutputTypeDef](./type_defs.md#replicationruleoutputtypedef)
- [GetBucketLoggingOutputTypeDef](./type_defs.md#getbucketloggingoutputtypedef)
- [BucketLoggingStatusTypeDef](./type_defs.md#bucketloggingstatustypedef)
- [PutBucketWebsiteRequestBucketWebsitePutTypeDef](./type_defs.md#putbucketwebsiterequestbucketwebsiteputtypedef)
- [PutBucketWebsiteRequestRequestTypeDef](./type_defs.md#putbucketwebsiterequestrequesttypedef)
- [GetBucketEncryptionOutputTypeDef](./type_defs.md#getbucketencryptionoutputtypedef)
- [PutBucketEncryptionRequestRequestTypeDef](./type_defs.md#putbucketencryptionrequestrequesttypedef)
- [SelectObjectContentOutputTypeDef](./type_defs.md#selectobjectcontentoutputtypedef)
- [PutBucketNotificationRequestRequestTypeDef](./type_defs.md#putbucketnotificationrequestrequesttypedef)
- [AnalyticsFilterUnionTypeDef](./type_defs.md#analyticsfilteruniontypedef)
- [GetBucketIntelligentTieringConfigurationOutputTypeDef](./type_defs.md#getbucketintelligenttieringconfigurationoutputtypedef)
- [ListBucketIntelligentTieringConfigurationsOutputTypeDef](./type_defs.md#listbucketintelligenttieringconfigurationsoutputtypedef)
- [IntelligentTieringFilterUnionTypeDef](./type_defs.md#intelligenttieringfilteruniontypedef)
- [GetBucketLifecycleConfigurationOutputTypeDef](./type_defs.md#getbucketlifecycleconfigurationoutputtypedef)
- [BucketLifecycleConfigurationTypeDef](./type_defs.md#bucketlifecycleconfigurationtypedef)
- [GetBucketMetricsConfigurationOutputTypeDef](./type_defs.md#getbucketmetricsconfigurationoutputtypedef)
- [ListBucketMetricsConfigurationsOutputTypeDef](./type_defs.md#listbucketmetricsconfigurationsoutputtypedef)
- [MetricsFilterUnionTypeDef](./type_defs.md#metricsfilteruniontypedef)
- [ReplicationRuleFilterUnionTypeDef](./type_defs.md#replicationrulefilteruniontypedef)
- [AnalyticsConfigurationOutputTypeDef](./type_defs.md#analyticsconfigurationoutputtypedef)
- [PutBucketLifecycleRequestBucketLifecyclePutTypeDef](./type_defs.md#putbucketlifecyclerequestbucketlifecycleputtypedef)
- [PutBucketLifecycleRequestRequestTypeDef](./type_defs.md#putbucketlifecyclerequestrequesttypedef)
- [NotificationConfigurationResponseTypeDef](./type_defs.md#notificationconfigurationresponsetypedef)
- [NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef)
- [RestoreRequestTypeDef](./type_defs.md#restorerequesttypedef)
- [InventoryConfigurationOutputTypeDef](./type_defs.md#inventoryconfigurationoutputtypedef)
- [InventoryS3BucketDestinationUnionTypeDef](./type_defs.md#inventorys3bucketdestinationuniontypedef)
- [ReplicationConfigurationOutputTypeDef](./type_defs.md#replicationconfigurationoutputtypedef)
- [PutBucketLoggingRequestBucketLoggingPutTypeDef](./type_defs.md#putbucketloggingrequestbucketloggingputtypedef)
- [PutBucketLoggingRequestRequestTypeDef](./type_defs.md#putbucketloggingrequestrequesttypedef)
- [AnalyticsConfigurationTypeDef](./type_defs.md#analyticsconfigurationtypedef)
- [IntelligentTieringConfigurationTypeDef](./type_defs.md#intelligenttieringconfigurationtypedef)
- [PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef](./type_defs.md#putbucketlifecycleconfigurationrequestbucketlifecycleconfigurationputtypedef)
- [PutBucketLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#putbucketlifecycleconfigurationrequestrequesttypedef)
- [MetricsConfigurationTypeDef](./type_defs.md#metricsconfigurationtypedef)
- [ReplicationRuleTypeDef](./type_defs.md#replicationruletypedef)
- [GetBucketAnalyticsConfigurationOutputTypeDef](./type_defs.md#getbucketanalyticsconfigurationoutputtypedef)
- [ListBucketAnalyticsConfigurationsOutputTypeDef](./type_defs.md#listbucketanalyticsconfigurationsoutputtypedef)
- [PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef](./type_defs.md#putbucketnotificationconfigurationrequestbucketnotificationputtypedef)
- [PutBucketNotificationConfigurationRequestRequestTypeDef](./type_defs.md#putbucketnotificationconfigurationrequestrequesttypedef)
- [RestoreObjectRequestObjectRestoreObjectTypeDef](./type_defs.md#restoreobjectrequestobjectrestoreobjecttypedef)
- [RestoreObjectRequestObjectSummaryRestoreObjectTypeDef](./type_defs.md#restoreobjectrequestobjectsummaryrestoreobjecttypedef)
- [RestoreObjectRequestRequestTypeDef](./type_defs.md#restoreobjectrequestrequesttypedef)
- [GetBucketInventoryConfigurationOutputTypeDef](./type_defs.md#getbucketinventoryconfigurationoutputtypedef)
- [ListBucketInventoryConfigurationsOutputTypeDef](./type_defs.md#listbucketinventoryconfigurationsoutputtypedef)
- [InventoryDestinationTypeDef](./type_defs.md#inventorydestinationtypedef)
- [GetBucketReplicationOutputTypeDef](./type_defs.md#getbucketreplicationoutputtypedef)
- [PutBucketAnalyticsConfigurationRequestRequestTypeDef](./type_defs.md#putbucketanalyticsconfigurationrequestrequesttypedef)
- [PutBucketIntelligentTieringConfigurationRequestRequestTypeDef](./type_defs.md#putbucketintelligenttieringconfigurationrequestrequesttypedef)
- [PutBucketMetricsConfigurationRequestRequestTypeDef](./type_defs.md#putbucketmetricsconfigurationrequestrequesttypedef)
- [ReplicationRuleUnionTypeDef](./type_defs.md#replicationruleuniontypedef)
- [InventoryDestinationUnionTypeDef](./type_defs.md#inventorydestinationuniontypedef)
- [ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef)
- [InventoryConfigurationTypeDef](./type_defs.md#inventoryconfigurationtypedef)
- [PutBucketReplicationRequestRequestTypeDef](./type_defs.md#putbucketreplicationrequestrequesttypedef)
- [PutBucketInventoryConfigurationRequestRequestTypeDef](./type_defs.md#putbucketinventoryconfigurationrequestrequesttypedef)

