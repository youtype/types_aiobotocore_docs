# Omics module

> [Index](../README.md) > Omics


!!! note ""

    Auto-generated documentation for [Omics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#omics)
    type annotations stubs module [types-aiobotocore-omics](https://pypi.org/project/types-aiobotocore-omics/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Omics` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Omics` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[omics]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[omics]'

# standalone installation
python -m pip install types-aiobotocore-omics
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-omics
```

## Usage

Code samples can be found in [Examples](./usage.md).

## OmicsClient

Type annotations and code completion for  `#!python session.create_client("omics")` as [OmicsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client)

```python
# OmicsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_omics.client import OmicsClient


session = get_session()
async with session.create_client("omics") as client:
    client: OmicsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("omics").get_paginator("...")`.

```python
# ListAnnotationImportJobsPaginator usage example

from types_aiobotocore_omics.paginator import ListAnnotationImportJobsPaginator

def get_list_annotation_import_jobs_paginator() -> ListAnnotationImportJobsPaginator:
    return client.get_paginator("list_annotation_import_jobs"))
```

- [ListAnnotationImportJobsPaginator](./paginators.md#listannotationimportjobspaginator)
- [ListAnnotationStoreVersionsPaginator](./paginators.md#listannotationstoreversionspaginator)
- [ListAnnotationStoresPaginator](./paginators.md#listannotationstorespaginator)
- [ListMultipartReadSetUploadsPaginator](./paginators.md#listmultipartreadsetuploadspaginator)
- [ListReadSetActivationJobsPaginator](./paginators.md#listreadsetactivationjobspaginator)
- [ListReadSetExportJobsPaginator](./paginators.md#listreadsetexportjobspaginator)
- [ListReadSetImportJobsPaginator](./paginators.md#listreadsetimportjobspaginator)
- [ListReadSetUploadPartsPaginator](./paginators.md#listreadsetuploadpartspaginator)
- [ListReadSetsPaginator](./paginators.md#listreadsetspaginator)
- [ListReferenceImportJobsPaginator](./paginators.md#listreferenceimportjobspaginator)
- [ListReferenceStoresPaginator](./paginators.md#listreferencestorespaginator)
- [ListReferencesPaginator](./paginators.md#listreferencespaginator)
- [ListRunCachesPaginator](./paginators.md#listruncachespaginator)
- [ListRunGroupsPaginator](./paginators.md#listrungroupspaginator)
- [ListRunTasksPaginator](./paginators.md#listruntaskspaginator)
- [ListRunsPaginator](./paginators.md#listrunspaginator)
- [ListSequenceStoresPaginator](./paginators.md#listsequencestorespaginator)
- [ListSharesPaginator](./paginators.md#listsharespaginator)
- [ListVariantImportJobsPaginator](./paginators.md#listvariantimportjobspaginator)
- [ListVariantStoresPaginator](./paginators.md#listvariantstorespaginator)
- [ListWorkflowsPaginator](./paginators.md#listworkflowspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("omics").get_waiter("...")`.

```python
# AnnotationImportJobCreatedWaiter usage example

from types_aiobotocore_omics.waiter import AnnotationImportJobCreatedWaiter

def get_annotation_import_job_created_waiter() -> AnnotationImportJobCreatedWaiter:
    return Session().client("omics").get_waiter("annotation_import_job_created")
```

- [AnnotationImportJobCreatedWaiter](./waiters.md#annotationimportjobcreatedwaiter)
- [AnnotationStoreCreatedWaiter](./waiters.md#annotationstorecreatedwaiter)
- [AnnotationStoreDeletedWaiter](./waiters.md#annotationstoredeletedwaiter)
- [AnnotationStoreVersionCreatedWaiter](./waiters.md#annotationstoreversioncreatedwaiter)
- [AnnotationStoreVersionDeletedWaiter](./waiters.md#annotationstoreversiondeletedwaiter)
- [ReadSetActivationJobCompletedWaiter](./waiters.md#readsetactivationjobcompletedwaiter)
- [ReadSetExportJobCompletedWaiter](./waiters.md#readsetexportjobcompletedwaiter)
- [ReadSetImportJobCompletedWaiter](./waiters.md#readsetimportjobcompletedwaiter)
- [ReferenceImportJobCompletedWaiter](./waiters.md#referenceimportjobcompletedwaiter)
- [RunCompletedWaiter](./waiters.md#runcompletedwaiter)
- [RunRunningWaiter](./waiters.md#runrunningwaiter)
- [TaskCompletedWaiter](./waiters.md#taskcompletedwaiter)
- [TaskRunningWaiter](./waiters.md#taskrunningwaiter)
- [VariantImportJobCreatedWaiter](./waiters.md#variantimportjobcreatedwaiter)
- [VariantStoreCreatedWaiter](./waiters.md#variantstorecreatedwaiter)
- [VariantStoreDeletedWaiter](./waiters.md#variantstoredeletedwaiter)
- [WorkflowActiveWaiter](./waiters.md#workflowactivewaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AcceleratorsType usage example

from types_aiobotocore_omics.literals import AcceleratorsType

def get_value() -> AcceleratorsType:
    return "GPU"
```

- [AcceleratorsType](./literals.md#acceleratorstype)
- [AnnotationImportJobCreatedWaiterName](./literals.md#annotationimportjobcreatedwaitername)
- [AnnotationStoreCreatedWaiterName](./literals.md#annotationstorecreatedwaitername)
- [AnnotationStoreDeletedWaiterName](./literals.md#annotationstoredeletedwaitername)
- [AnnotationStoreVersionCreatedWaiterName](./literals.md#annotationstoreversioncreatedwaitername)
- [AnnotationStoreVersionDeletedWaiterName](./literals.md#annotationstoreversiondeletedwaitername)
- [AnnotationTypeType](./literals.md#annotationtypetype)
- [CacheBehaviorType](./literals.md#cachebehaviortype)
- [CreationTypeType](./literals.md#creationtypetype)
- [ETagAlgorithmFamilyType](./literals.md#etagalgorithmfamilytype)
- [ETagAlgorithmType](./literals.md#etagalgorithmtype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [FileTypeType](./literals.md#filetypetype)
- [FormatToHeaderKeyType](./literals.md#formattoheaderkeytype)
- [JobStatusType](./literals.md#jobstatustype)
- [ListAnnotationImportJobsPaginatorName](./literals.md#listannotationimportjobspaginatorname)
- [ListAnnotationStoreVersionsPaginatorName](./literals.md#listannotationstoreversionspaginatorname)
- [ListAnnotationStoresPaginatorName](./literals.md#listannotationstorespaginatorname)
- [ListMultipartReadSetUploadsPaginatorName](./literals.md#listmultipartreadsetuploadspaginatorname)
- [ListReadSetActivationJobsPaginatorName](./literals.md#listreadsetactivationjobspaginatorname)
- [ListReadSetExportJobsPaginatorName](./literals.md#listreadsetexportjobspaginatorname)
- [ListReadSetImportJobsPaginatorName](./literals.md#listreadsetimportjobspaginatorname)
- [ListReadSetUploadPartsPaginatorName](./literals.md#listreadsetuploadpartspaginatorname)
- [ListReadSetsPaginatorName](./literals.md#listreadsetspaginatorname)
- [ListReferenceImportJobsPaginatorName](./literals.md#listreferenceimportjobspaginatorname)
- [ListReferenceStoresPaginatorName](./literals.md#listreferencestorespaginatorname)
- [ListReferencesPaginatorName](./literals.md#listreferencespaginatorname)
- [ListRunCachesPaginatorName](./literals.md#listruncachespaginatorname)
- [ListRunGroupsPaginatorName](./literals.md#listrungroupspaginatorname)
- [ListRunTasksPaginatorName](./literals.md#listruntaskspaginatorname)
- [ListRunsPaginatorName](./literals.md#listrunspaginatorname)
- [ListSequenceStoresPaginatorName](./literals.md#listsequencestorespaginatorname)
- [ListSharesPaginatorName](./literals.md#listsharespaginatorname)
- [ListVariantImportJobsPaginatorName](./literals.md#listvariantimportjobspaginatorname)
- [ListVariantStoresPaginatorName](./literals.md#listvariantstorespaginatorname)
- [ListWorkflowsPaginatorName](./literals.md#listworkflowspaginatorname)
- [ReadSetActivationJobCompletedWaiterName](./literals.md#readsetactivationjobcompletedwaitername)
- [ReadSetActivationJobItemStatusType](./literals.md#readsetactivationjobitemstatustype)
- [ReadSetActivationJobStatusType](./literals.md#readsetactivationjobstatustype)
- [ReadSetExportJobCompletedWaiterName](./literals.md#readsetexportjobcompletedwaitername)
- [ReadSetExportJobItemStatusType](./literals.md#readsetexportjobitemstatustype)
- [ReadSetExportJobStatusType](./literals.md#readsetexportjobstatustype)
- [ReadSetFileType](./literals.md#readsetfiletype)
- [ReadSetImportJobCompletedWaiterName](./literals.md#readsetimportjobcompletedwaitername)
- [ReadSetImportJobItemStatusType](./literals.md#readsetimportjobitemstatustype)
- [ReadSetImportJobStatusType](./literals.md#readsetimportjobstatustype)
- [ReadSetPartSourceType](./literals.md#readsetpartsourcetype)
- [ReadSetStatusType](./literals.md#readsetstatustype)
- [ReferenceCreationTypeType](./literals.md#referencecreationtypetype)
- [ReferenceFileType](./literals.md#referencefiletype)
- [ReferenceImportJobCompletedWaiterName](./literals.md#referenceimportjobcompletedwaitername)
- [ReferenceImportJobItemStatusType](./literals.md#referenceimportjobitemstatustype)
- [ReferenceImportJobStatusType](./literals.md#referenceimportjobstatustype)
- [ReferenceStatusType](./literals.md#referencestatustype)
- [ResourceOwnerType](./literals.md#resourceownertype)
- [RunCacheStatusType](./literals.md#runcachestatustype)
- [RunCompletedWaiterName](./literals.md#runcompletedwaitername)
- [RunExportType](./literals.md#runexporttype)
- [RunLogLevelType](./literals.md#runlogleveltype)
- [RunRetentionModeType](./literals.md#runretentionmodetype)
- [RunRunningWaiterName](./literals.md#runrunningwaitername)
- [RunStatusType](./literals.md#runstatustype)
- [SchemaValueTypeType](./literals.md#schemavaluetypetype)
- [SequenceStoreStatusType](./literals.md#sequencestorestatustype)
- [ShareResourceTypeType](./literals.md#shareresourcetypetype)
- [ShareStatusType](./literals.md#sharestatustype)
- [StorageTypeType](./literals.md#storagetypetype)
- [StoreFormatType](./literals.md#storeformattype)
- [StoreStatusType](./literals.md#storestatustype)
- [StoreTypeType](./literals.md#storetypetype)
- [TaskCompletedWaiterName](./literals.md#taskcompletedwaitername)
- [TaskRunningWaiterName](./literals.md#taskrunningwaitername)
- [TaskStatusType](./literals.md#taskstatustype)
- [VariantImportJobCreatedWaiterName](./literals.md#variantimportjobcreatedwaitername)
- [VariantStoreCreatedWaiterName](./literals.md#variantstorecreatedwaitername)
- [VariantStoreDeletedWaiterName](./literals.md#variantstoredeletedwaitername)
- [VersionStatusType](./literals.md#versionstatustype)
- [WorkflowActiveWaiterName](./literals.md#workflowactivewaitername)
- [WorkflowEngineType](./literals.md#workflowenginetype)
- [WorkflowExportType](./literals.md#workflowexporttype)
- [WorkflowStatusType](./literals.md#workflowstatustype)
- [WorkflowTypeType](./literals.md#workflowtypetype)
- [OmicsServiceName](./literals.md#omicsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AbortMultipartReadSetUploadRequestRequestTypeDef](./type_defs.md#abortmultipartreadsetuploadrequestrequesttypedef)
- [AcceptShareRequestRequestTypeDef](./type_defs.md#acceptsharerequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ActivateReadSetJobItemTypeDef](./type_defs.md#activatereadsetjobitemtypedef)
- [ActivateReadSetSourceItemTypeDef](./type_defs.md#activatereadsetsourceitemtypedef)
- [AnnotationImportItemDetailTypeDef](./type_defs.md#annotationimportitemdetailtypedef)
- [AnnotationImportItemSourceTypeDef](./type_defs.md#annotationimportitemsourcetypedef)
- [AnnotationImportJobItemTypeDef](./type_defs.md#annotationimportjobitemtypedef)
- [ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef)
- [SseConfigTypeDef](./type_defs.md#sseconfigtypedef)
- [AnnotationStoreVersionItemTypeDef](./type_defs.md#annotationstoreversionitemtypedef)
- [BatchDeleteReadSetRequestRequestTypeDef](./type_defs.md#batchdeletereadsetrequestrequesttypedef)
- [ReadSetBatchErrorTypeDef](./type_defs.md#readsetbatcherrortypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CancelAnnotationImportRequestRequestTypeDef](./type_defs.md#cancelannotationimportrequestrequesttypedef)
- [CancelRunRequestRequestTypeDef](./type_defs.md#cancelrunrequestrequesttypedef)
- [CancelVariantImportRequestRequestTypeDef](./type_defs.md#cancelvariantimportrequestrequesttypedef)
- [CompleteReadSetUploadPartListItemTypeDef](./type_defs.md#completereadsetuploadpartlistitemtypedef)
- [CreateMultipartReadSetUploadRequestRequestTypeDef](./type_defs.md#createmultipartreadsetuploadrequestrequesttypedef)
- [CreateRunCacheRequestRequestTypeDef](./type_defs.md#createruncacherequestrequesttypedef)
- [CreateRunGroupRequestRequestTypeDef](./type_defs.md#createrungrouprequestrequesttypedef)
- [S3AccessConfigTypeDef](./type_defs.md#s3accessconfigtypedef)
- [SequenceStoreS3AccessTypeDef](./type_defs.md#sequencestores3accesstypedef)
- [CreateShareRequestRequestTypeDef](./type_defs.md#createsharerequestrequesttypedef)
- [WorkflowParameterTypeDef](./type_defs.md#workflowparametertypedef)
- [DeleteAnnotationStoreRequestRequestTypeDef](./type_defs.md#deleteannotationstorerequestrequesttypedef)
- [DeleteAnnotationStoreVersionsRequestRequestTypeDef](./type_defs.md#deleteannotationstoreversionsrequestrequesttypedef)
- [VersionDeleteErrorTypeDef](./type_defs.md#versiondeleteerrortypedef)
- [DeleteReferenceRequestRequestTypeDef](./type_defs.md#deletereferencerequestrequesttypedef)
- [DeleteReferenceStoreRequestRequestTypeDef](./type_defs.md#deletereferencestorerequestrequesttypedef)
- [DeleteRunCacheRequestRequestTypeDef](./type_defs.md#deleteruncacherequestrequesttypedef)
- [DeleteRunGroupRequestRequestTypeDef](./type_defs.md#deleterungrouprequestrequesttypedef)
- [DeleteRunRequestRequestTypeDef](./type_defs.md#deleterunrequestrequesttypedef)
- [DeleteS3AccessPolicyRequestRequestTypeDef](./type_defs.md#deletes3accesspolicyrequestrequesttypedef)
- [DeleteSequenceStoreRequestRequestTypeDef](./type_defs.md#deletesequencestorerequestrequesttypedef)
- [DeleteShareRequestRequestTypeDef](./type_defs.md#deletesharerequestrequesttypedef)
- [DeleteVariantStoreRequestRequestTypeDef](./type_defs.md#deletevariantstorerequestrequesttypedef)
- [DeleteWorkflowRequestRequestTypeDef](./type_defs.md#deleteworkflowrequestrequesttypedef)
- [ETagTypeDef](./type_defs.md#etagtypedef)
- [ExportReadSetDetailTypeDef](./type_defs.md#exportreadsetdetailtypedef)
- [ExportReadSetJobDetailTypeDef](./type_defs.md#exportreadsetjobdetailtypedef)
- [ExportReadSetTypeDef](./type_defs.md#exportreadsettypedef)
- [ReadSetS3AccessTypeDef](./type_defs.md#readsets3accesstypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [VcfOptionsTypeDef](./type_defs.md#vcfoptionstypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [GetAnnotationImportRequestRequestTypeDef](./type_defs.md#getannotationimportrequestrequesttypedef)
- [GetAnnotationStoreRequestRequestTypeDef](./type_defs.md#getannotationstorerequestrequesttypedef)
- [GetAnnotationStoreVersionRequestRequestTypeDef](./type_defs.md#getannotationstoreversionrequestrequesttypedef)
- [GetReadSetActivationJobRequestRequestTypeDef](./type_defs.md#getreadsetactivationjobrequestrequesttypedef)
- [GetReadSetExportJobRequestRequestTypeDef](./type_defs.md#getreadsetexportjobrequestrequesttypedef)
- [GetReadSetImportJobRequestRequestTypeDef](./type_defs.md#getreadsetimportjobrequestrequesttypedef)
- [GetReadSetMetadataRequestRequestTypeDef](./type_defs.md#getreadsetmetadatarequestrequesttypedef)
- [SequenceInformationTypeDef](./type_defs.md#sequenceinformationtypedef)
- [GetReadSetRequestRequestTypeDef](./type_defs.md#getreadsetrequestrequesttypedef)
- [GetReferenceImportJobRequestRequestTypeDef](./type_defs.md#getreferenceimportjobrequestrequesttypedef)
- [ImportReferenceSourceItemTypeDef](./type_defs.md#importreferencesourceitemtypedef)
- [GetReferenceMetadataRequestRequestTypeDef](./type_defs.md#getreferencemetadatarequestrequesttypedef)
- [GetReferenceRequestRequestTypeDef](./type_defs.md#getreferencerequestrequesttypedef)
- [GetReferenceStoreRequestRequestTypeDef](./type_defs.md#getreferencestorerequestrequesttypedef)
- [GetRunCacheRequestRequestTypeDef](./type_defs.md#getruncacherequestrequesttypedef)
- [GetRunGroupRequestRequestTypeDef](./type_defs.md#getrungrouprequestrequesttypedef)
- [GetRunRequestRequestTypeDef](./type_defs.md#getrunrequestrequesttypedef)
- [RunLogLocationTypeDef](./type_defs.md#runloglocationtypedef)
- [GetRunTaskRequestRequestTypeDef](./type_defs.md#getruntaskrequestrequesttypedef)
- [GetS3AccessPolicyRequestRequestTypeDef](./type_defs.md#gets3accesspolicyrequestrequesttypedef)
- [GetSequenceStoreRequestRequestTypeDef](./type_defs.md#getsequencestorerequestrequesttypedef)
- [GetShareRequestRequestTypeDef](./type_defs.md#getsharerequestrequesttypedef)
- [ShareDetailsTypeDef](./type_defs.md#sharedetailstypedef)
- [GetVariantImportRequestRequestTypeDef](./type_defs.md#getvariantimportrequestrequesttypedef)
- [VariantImportItemDetailTypeDef](./type_defs.md#variantimportitemdetailtypedef)
- [GetVariantStoreRequestRequestTypeDef](./type_defs.md#getvariantstorerequestrequesttypedef)
- [GetWorkflowRequestRequestTypeDef](./type_defs.md#getworkflowrequestrequesttypedef)
- [ImportReadSetJobItemTypeDef](./type_defs.md#importreadsetjobitemtypedef)
- [SourceFilesTypeDef](./type_defs.md#sourcefilestypedef)
- [ImportReferenceJobItemTypeDef](./type_defs.md#importreferencejobitemtypedef)
- [ListAnnotationImportJobsFilterTypeDef](./type_defs.md#listannotationimportjobsfiltertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAnnotationStoreVersionsFilterTypeDef](./type_defs.md#listannotationstoreversionsfiltertypedef)
- [ListAnnotationStoresFilterTypeDef](./type_defs.md#listannotationstoresfiltertypedef)
- [ListMultipartReadSetUploadsRequestRequestTypeDef](./type_defs.md#listmultipartreadsetuploadsrequestrequesttypedef)
- [MultipartReadSetUploadListItemTypeDef](./type_defs.md#multipartreadsetuploadlistitemtypedef)
- [ReadSetUploadPartListItemTypeDef](./type_defs.md#readsetuploadpartlistitemtypedef)
- [ReferenceListItemTypeDef](./type_defs.md#referencelistitemtypedef)
- [ListRunCachesRequestRequestTypeDef](./type_defs.md#listruncachesrequestrequesttypedef)
- [RunCacheListItemTypeDef](./type_defs.md#runcachelistitemtypedef)
- [ListRunGroupsRequestRequestTypeDef](./type_defs.md#listrungroupsrequestrequesttypedef)
- [RunGroupListItemTypeDef](./type_defs.md#rungrouplistitemtypedef)
- [ListRunTasksRequestRequestTypeDef](./type_defs.md#listruntasksrequestrequesttypedef)
- [TaskListItemTypeDef](./type_defs.md#tasklistitemtypedef)
- [ListRunsRequestRequestTypeDef](./type_defs.md#listrunsrequestrequesttypedef)
- [RunListItemTypeDef](./type_defs.md#runlistitemtypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListVariantImportJobsFilterTypeDef](./type_defs.md#listvariantimportjobsfiltertypedef)
- [VariantImportJobItemTypeDef](./type_defs.md#variantimportjobitemtypedef)
- [ListVariantStoresFilterTypeDef](./type_defs.md#listvariantstoresfiltertypedef)
- [ListWorkflowsRequestRequestTypeDef](./type_defs.md#listworkflowsrequestrequesttypedef)
- [WorkflowListItemTypeDef](./type_defs.md#workflowlistitemtypedef)
- [PutS3AccessPolicyRequestRequestTypeDef](./type_defs.md#puts3accesspolicyrequestrequesttypedef)
- [ReadOptionsTypeDef](./type_defs.md#readoptionstypedef)
- [StartReadSetActivationJobSourceItemTypeDef](./type_defs.md#startreadsetactivationjobsourceitemtypedef)
- [StartReferenceImportJobSourceItemTypeDef](./type_defs.md#startreferenceimportjobsourceitemtypedef)
- [StartRunRequestRequestTypeDef](./type_defs.md#startrunrequestrequesttypedef)
- [VariantImportItemSourceTypeDef](./type_defs.md#variantimportitemsourcetypedef)
- [TsvStoreOptionsOutputTypeDef](./type_defs.md#tsvstoreoptionsoutputtypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TsvStoreOptionsTypeDef](./type_defs.md#tsvstoreoptionstypedef)
- [TsvVersionOptionsOutputTypeDef](./type_defs.md#tsvversionoptionsoutputtypedef)
- [TsvVersionOptionsTypeDef](./type_defs.md#tsvversionoptionstypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAnnotationStoreRequestRequestTypeDef](./type_defs.md#updateannotationstorerequestrequesttypedef)
- [UpdateAnnotationStoreVersionRequestRequestTypeDef](./type_defs.md#updateannotationstoreversionrequestrequesttypedef)
- [UpdateRunCacheRequestRequestTypeDef](./type_defs.md#updateruncacherequestrequesttypedef)
- [UpdateRunGroupRequestRequestTypeDef](./type_defs.md#updaterungrouprequestrequesttypedef)
- [UpdateVariantStoreRequestRequestTypeDef](./type_defs.md#updatevariantstorerequestrequesttypedef)
- [UpdateWorkflowRequestRequestTypeDef](./type_defs.md#updateworkflowrequestrequesttypedef)
- [AcceptShareResponseTypeDef](./type_defs.md#acceptshareresponsetypedef)
- [CompleteMultipartReadSetUploadResponseTypeDef](./type_defs.md#completemultipartreadsetuploadresponsetypedef)
- [CreateMultipartReadSetUploadResponseTypeDef](./type_defs.md#createmultipartreadsetuploadresponsetypedef)
- [CreateRunCacheResponseTypeDef](./type_defs.md#createruncacheresponsetypedef)
- [CreateRunGroupResponseTypeDef](./type_defs.md#createrungroupresponsetypedef)
- [CreateShareResponseTypeDef](./type_defs.md#createshareresponsetypedef)
- [CreateWorkflowResponseTypeDef](./type_defs.md#createworkflowresponsetypedef)
- [DeleteAnnotationStoreResponseTypeDef](./type_defs.md#deleteannotationstoreresponsetypedef)
- [DeleteShareResponseTypeDef](./type_defs.md#deleteshareresponsetypedef)
- [DeleteVariantStoreResponseTypeDef](./type_defs.md#deletevariantstoreresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetReadSetResponseTypeDef](./type_defs.md#getreadsetresponsetypedef)
- [GetReferenceResponseTypeDef](./type_defs.md#getreferenceresponsetypedef)
- [GetRunCacheResponseTypeDef](./type_defs.md#getruncacheresponsetypedef)
- [GetRunGroupResponseTypeDef](./type_defs.md#getrungroupresponsetypedef)
- [GetRunTaskResponseTypeDef](./type_defs.md#getruntaskresponsetypedef)
- [GetS3AccessPolicyResponseTypeDef](./type_defs.md#gets3accesspolicyresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutS3AccessPolicyResponseTypeDef](./type_defs.md#puts3accesspolicyresponsetypedef)
- [StartAnnotationImportResponseTypeDef](./type_defs.md#startannotationimportresponsetypedef)
- [StartReadSetActivationJobResponseTypeDef](./type_defs.md#startreadsetactivationjobresponsetypedef)
- [StartReadSetExportJobResponseTypeDef](./type_defs.md#startreadsetexportjobresponsetypedef)
- [StartReadSetImportJobResponseTypeDef](./type_defs.md#startreadsetimportjobresponsetypedef)
- [StartReferenceImportJobResponseTypeDef](./type_defs.md#startreferenceimportjobresponsetypedef)
- [StartRunResponseTypeDef](./type_defs.md#startrunresponsetypedef)
- [StartVariantImportResponseTypeDef](./type_defs.md#startvariantimportresponsetypedef)
- [UpdateAnnotationStoreVersionResponseTypeDef](./type_defs.md#updateannotationstoreversionresponsetypedef)
- [UploadReadSetPartResponseTypeDef](./type_defs.md#uploadreadsetpartresponsetypedef)
- [ActivateReadSetFilterTypeDef](./type_defs.md#activatereadsetfiltertypedef)
- [ExportReadSetFilterTypeDef](./type_defs.md#exportreadsetfiltertypedef)
- [ImportReadSetFilterTypeDef](./type_defs.md#importreadsetfiltertypedef)
- [ImportReferenceFilterTypeDef](./type_defs.md#importreferencefiltertypedef)
- [ReadSetFilterTypeDef](./type_defs.md#readsetfiltertypedef)
- [ReadSetUploadPartListFilterTypeDef](./type_defs.md#readsetuploadpartlistfiltertypedef)
- [ReferenceFilterTypeDef](./type_defs.md#referencefiltertypedef)
- [ReferenceStoreFilterTypeDef](./type_defs.md#referencestorefiltertypedef)
- [SequenceStoreFilterTypeDef](./type_defs.md#sequencestorefiltertypedef)
- [ListReadSetActivationJobsResponseTypeDef](./type_defs.md#listreadsetactivationjobsresponsetypedef)
- [GetReadSetActivationJobResponseTypeDef](./type_defs.md#getreadsetactivationjobresponsetypedef)
- [ListAnnotationImportJobsResponseTypeDef](./type_defs.md#listannotationimportjobsresponsetypedef)
- [CreateVariantStoreResponseTypeDef](./type_defs.md#createvariantstoreresponsetypedef)
- [UpdateVariantStoreResponseTypeDef](./type_defs.md#updatevariantstoreresponsetypedef)
- [AnnotationStoreItemTypeDef](./type_defs.md#annotationstoreitemtypedef)
- [CreateReferenceStoreRequestRequestTypeDef](./type_defs.md#createreferencestorerequestrequesttypedef)
- [CreateReferenceStoreResponseTypeDef](./type_defs.md#createreferencestoreresponsetypedef)
- [CreateVariantStoreRequestRequestTypeDef](./type_defs.md#createvariantstorerequestrequesttypedef)
- [GetReferenceStoreResponseTypeDef](./type_defs.md#getreferencestoreresponsetypedef)
- [GetVariantStoreResponseTypeDef](./type_defs.md#getvariantstoreresponsetypedef)
- [ReferenceStoreDetailTypeDef](./type_defs.md#referencestoredetailtypedef)
- [SequenceStoreDetailTypeDef](./type_defs.md#sequencestoredetailtypedef)
- [VariantStoreItemTypeDef](./type_defs.md#variantstoreitemtypedef)
- [ListAnnotationStoreVersionsResponseTypeDef](./type_defs.md#listannotationstoreversionsresponsetypedef)
- [BatchDeleteReadSetResponseTypeDef](./type_defs.md#batchdeletereadsetresponsetypedef)
- [UploadReadSetPartRequestRequestTypeDef](./type_defs.md#uploadreadsetpartrequestrequesttypedef)
- [CompleteMultipartReadSetUploadRequestRequestTypeDef](./type_defs.md#completemultipartreadsetuploadrequestrequesttypedef)
- [CreateSequenceStoreRequestRequestTypeDef](./type_defs.md#createsequencestorerequestrequesttypedef)
- [UpdateSequenceStoreRequestRequestTypeDef](./type_defs.md#updatesequencestorerequestrequesttypedef)
- [CreateSequenceStoreResponseTypeDef](./type_defs.md#createsequencestoreresponsetypedef)
- [GetSequenceStoreResponseTypeDef](./type_defs.md#getsequencestoreresponsetypedef)
- [UpdateSequenceStoreResponseTypeDef](./type_defs.md#updatesequencestoreresponsetypedef)
- [CreateWorkflowRequestRequestTypeDef](./type_defs.md#createworkflowrequestrequesttypedef)
- [GetWorkflowResponseTypeDef](./type_defs.md#getworkflowresponsetypedef)
- [DeleteAnnotationStoreVersionsResponseTypeDef](./type_defs.md#deleteannotationstoreversionsresponsetypedef)
- [GetReadSetExportJobResponseTypeDef](./type_defs.md#getreadsetexportjobresponsetypedef)
- [ListReadSetExportJobsResponseTypeDef](./type_defs.md#listreadsetexportjobsresponsetypedef)
- [StartReadSetExportJobRequestRequestTypeDef](./type_defs.md#startreadsetexportjobrequestrequesttypedef)
- [FileInformationTypeDef](./type_defs.md#fileinformationtypedef)
- [ListSharesRequestRequestTypeDef](./type_defs.md#listsharesrequestrequesttypedef)
- [GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef](./type_defs.md#getannotationimportrequestannotationimportjobcreatedwaittypedef)
- [GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef](./type_defs.md#getannotationstorerequestannotationstorecreatedwaittypedef)
- [GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef](./type_defs.md#getannotationstorerequestannotationstoredeletedwaittypedef)
- [GetAnnotationStoreVersionRequestAnnotationStoreVersionCreatedWaitTypeDef](./type_defs.md#getannotationstoreversionrequestannotationstoreversioncreatedwaittypedef)
- [GetAnnotationStoreVersionRequestAnnotationStoreVersionDeletedWaitTypeDef](./type_defs.md#getannotationstoreversionrequestannotationstoreversiondeletedwaittypedef)
- [GetReadSetActivationJobRequestReadSetActivationJobCompletedWaitTypeDef](./type_defs.md#getreadsetactivationjobrequestreadsetactivationjobcompletedwaittypedef)
- [GetReadSetExportJobRequestReadSetExportJobCompletedWaitTypeDef](./type_defs.md#getreadsetexportjobrequestreadsetexportjobcompletedwaittypedef)
- [GetReadSetImportJobRequestReadSetImportJobCompletedWaitTypeDef](./type_defs.md#getreadsetimportjobrequestreadsetimportjobcompletedwaittypedef)
- [GetReferenceImportJobRequestReferenceImportJobCompletedWaitTypeDef](./type_defs.md#getreferenceimportjobrequestreferenceimportjobcompletedwaittypedef)
- [GetRunRequestRunCompletedWaitTypeDef](./type_defs.md#getrunrequestruncompletedwaittypedef)
- [GetRunRequestRunRunningWaitTypeDef](./type_defs.md#getrunrequestrunrunningwaittypedef)
- [GetRunTaskRequestTaskCompletedWaitTypeDef](./type_defs.md#getruntaskrequesttaskcompletedwaittypedef)
- [GetRunTaskRequestTaskRunningWaitTypeDef](./type_defs.md#getruntaskrequesttaskrunningwaittypedef)
- [GetVariantImportRequestVariantImportJobCreatedWaitTypeDef](./type_defs.md#getvariantimportrequestvariantimportjobcreatedwaittypedef)
- [GetVariantStoreRequestVariantStoreCreatedWaitTypeDef](./type_defs.md#getvariantstorerequestvariantstorecreatedwaittypedef)
- [GetVariantStoreRequestVariantStoreDeletedWaitTypeDef](./type_defs.md#getvariantstorerequestvariantstoredeletedwaittypedef)
- [GetWorkflowRequestWorkflowActiveWaitTypeDef](./type_defs.md#getworkflowrequestworkflowactivewaittypedef)
- [ReadSetListItemTypeDef](./type_defs.md#readsetlistitemtypedef)
- [GetReferenceImportJobResponseTypeDef](./type_defs.md#getreferenceimportjobresponsetypedef)
- [GetRunResponseTypeDef](./type_defs.md#getrunresponsetypedef)
- [GetShareResponseTypeDef](./type_defs.md#getshareresponsetypedef)
- [ListSharesResponseTypeDef](./type_defs.md#listsharesresponsetypedef)
- [GetVariantImportResponseTypeDef](./type_defs.md#getvariantimportresponsetypedef)
- [ListReadSetImportJobsResponseTypeDef](./type_defs.md#listreadsetimportjobsresponsetypedef)
- [ImportReadSetSourceItemTypeDef](./type_defs.md#importreadsetsourceitemtypedef)
- [StartReadSetImportJobSourceItemTypeDef](./type_defs.md#startreadsetimportjobsourceitemtypedef)
- [ListReferenceImportJobsResponseTypeDef](./type_defs.md#listreferenceimportjobsresponsetypedef)
- [ListAnnotationImportJobsRequestRequestTypeDef](./type_defs.md#listannotationimportjobsrequestrequesttypedef)
- [ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef](./type_defs.md#listannotationimportjobsrequestlistannotationimportjobspaginatetypedef)
- [ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef](./type_defs.md#listmultipartreadsetuploadsrequestlistmultipartreadsetuploadspaginatetypedef)
- [ListRunCachesRequestListRunCachesPaginateTypeDef](./type_defs.md#listruncachesrequestlistruncachespaginatetypedef)
- [ListRunGroupsRequestListRunGroupsPaginateTypeDef](./type_defs.md#listrungroupsrequestlistrungroupspaginatetypedef)
- [ListRunTasksRequestListRunTasksPaginateTypeDef](./type_defs.md#listruntasksrequestlistruntaskspaginatetypedef)
- [ListRunsRequestListRunsPaginateTypeDef](./type_defs.md#listrunsrequestlistrunspaginatetypedef)
- [ListSharesRequestListSharesPaginateTypeDef](./type_defs.md#listsharesrequestlistsharespaginatetypedef)
- [ListWorkflowsRequestListWorkflowsPaginateTypeDef](./type_defs.md#listworkflowsrequestlistworkflowspaginatetypedef)
- [ListAnnotationStoreVersionsRequestListAnnotationStoreVersionsPaginateTypeDef](./type_defs.md#listannotationstoreversionsrequestlistannotationstoreversionspaginatetypedef)
- [ListAnnotationStoreVersionsRequestRequestTypeDef](./type_defs.md#listannotationstoreversionsrequestrequesttypedef)
- [ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef](./type_defs.md#listannotationstoresrequestlistannotationstorespaginatetypedef)
- [ListAnnotationStoresRequestRequestTypeDef](./type_defs.md#listannotationstoresrequestrequesttypedef)
- [ListMultipartReadSetUploadsResponseTypeDef](./type_defs.md#listmultipartreadsetuploadsresponsetypedef)
- [ListReadSetUploadPartsResponseTypeDef](./type_defs.md#listreadsetuploadpartsresponsetypedef)
- [ListReferencesResponseTypeDef](./type_defs.md#listreferencesresponsetypedef)
- [ListRunCachesResponseTypeDef](./type_defs.md#listruncachesresponsetypedef)
- [ListRunGroupsResponseTypeDef](./type_defs.md#listrungroupsresponsetypedef)
- [ListRunTasksResponseTypeDef](./type_defs.md#listruntasksresponsetypedef)
- [ListRunsResponseTypeDef](./type_defs.md#listrunsresponsetypedef)
- [ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef](./type_defs.md#listvariantimportjobsrequestlistvariantimportjobspaginatetypedef)
- [ListVariantImportJobsRequestRequestTypeDef](./type_defs.md#listvariantimportjobsrequestrequesttypedef)
- [ListVariantImportJobsResponseTypeDef](./type_defs.md#listvariantimportjobsresponsetypedef)
- [ListVariantStoresRequestListVariantStoresPaginateTypeDef](./type_defs.md#listvariantstoresrequestlistvariantstorespaginatetypedef)
- [ListVariantStoresRequestRequestTypeDef](./type_defs.md#listvariantstoresrequestrequesttypedef)
- [ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef)
- [TsvOptionsTypeDef](./type_defs.md#tsvoptionstypedef)
- [StartReadSetActivationJobRequestRequestTypeDef](./type_defs.md#startreadsetactivationjobrequestrequesttypedef)
- [StartReferenceImportJobRequestRequestTypeDef](./type_defs.md#startreferenceimportjobrequestrequesttypedef)
- [StartVariantImportRequestRequestTypeDef](./type_defs.md#startvariantimportrequestrequesttypedef)
- [StoreOptionsOutputTypeDef](./type_defs.md#storeoptionsoutputtypedef)
- [TsvStoreOptionsUnionTypeDef](./type_defs.md#tsvstoreoptionsuniontypedef)
- [VersionOptionsOutputTypeDef](./type_defs.md#versionoptionsoutputtypedef)
- [TsvVersionOptionsUnionTypeDef](./type_defs.md#tsvversionoptionsuniontypedef)
- [ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef](./type_defs.md#listreadsetactivationjobsrequestlistreadsetactivationjobspaginatetypedef)
- [ListReadSetActivationJobsRequestRequestTypeDef](./type_defs.md#listreadsetactivationjobsrequestrequesttypedef)
- [ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef](./type_defs.md#listreadsetexportjobsrequestlistreadsetexportjobspaginatetypedef)
- [ListReadSetExportJobsRequestRequestTypeDef](./type_defs.md#listreadsetexportjobsrequestrequesttypedef)
- [ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef](./type_defs.md#listreadsetimportjobsrequestlistreadsetimportjobspaginatetypedef)
- [ListReadSetImportJobsRequestRequestTypeDef](./type_defs.md#listreadsetimportjobsrequestrequesttypedef)
- [ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef](./type_defs.md#listreferenceimportjobsrequestlistreferenceimportjobspaginatetypedef)
- [ListReferenceImportJobsRequestRequestTypeDef](./type_defs.md#listreferenceimportjobsrequestrequesttypedef)
- [ListReadSetsRequestListReadSetsPaginateTypeDef](./type_defs.md#listreadsetsrequestlistreadsetspaginatetypedef)
- [ListReadSetsRequestRequestTypeDef](./type_defs.md#listreadsetsrequestrequesttypedef)
- [ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef](./type_defs.md#listreadsetuploadpartsrequestlistreadsetuploadpartspaginatetypedef)
- [ListReadSetUploadPartsRequestRequestTypeDef](./type_defs.md#listreadsetuploadpartsrequestrequesttypedef)
- [ListReferencesRequestListReferencesPaginateTypeDef](./type_defs.md#listreferencesrequestlistreferencespaginatetypedef)
- [ListReferencesRequestRequestTypeDef](./type_defs.md#listreferencesrequestrequesttypedef)
- [ListReferenceStoresRequestListReferenceStoresPaginateTypeDef](./type_defs.md#listreferencestoresrequestlistreferencestorespaginatetypedef)
- [ListReferenceStoresRequestRequestTypeDef](./type_defs.md#listreferencestoresrequestrequesttypedef)
- [ListSequenceStoresRequestListSequenceStoresPaginateTypeDef](./type_defs.md#listsequencestoresrequestlistsequencestorespaginatetypedef)
- [ListSequenceStoresRequestRequestTypeDef](./type_defs.md#listsequencestoresrequestrequesttypedef)
- [ListAnnotationStoresResponseTypeDef](./type_defs.md#listannotationstoresresponsetypedef)
- [ListReferenceStoresResponseTypeDef](./type_defs.md#listreferencestoresresponsetypedef)
- [ListSequenceStoresResponseTypeDef](./type_defs.md#listsequencestoresresponsetypedef)
- [ListVariantStoresResponseTypeDef](./type_defs.md#listvariantstoresresponsetypedef)
- [ReadSetFilesTypeDef](./type_defs.md#readsetfilestypedef)
- [ReferenceFilesTypeDef](./type_defs.md#referencefilestypedef)
- [ListReadSetsResponseTypeDef](./type_defs.md#listreadsetsresponsetypedef)
- [GetReadSetImportJobResponseTypeDef](./type_defs.md#getreadsetimportjobresponsetypedef)
- [StartReadSetImportJobRequestRequestTypeDef](./type_defs.md#startreadsetimportjobrequestrequesttypedef)
- [FormatOptionsTypeDef](./type_defs.md#formatoptionstypedef)
- [CreateAnnotationStoreResponseTypeDef](./type_defs.md#createannotationstoreresponsetypedef)
- [GetAnnotationStoreResponseTypeDef](./type_defs.md#getannotationstoreresponsetypedef)
- [UpdateAnnotationStoreResponseTypeDef](./type_defs.md#updateannotationstoreresponsetypedef)
- [StoreOptionsTypeDef](./type_defs.md#storeoptionstypedef)
- [CreateAnnotationStoreVersionResponseTypeDef](./type_defs.md#createannotationstoreversionresponsetypedef)
- [GetAnnotationStoreVersionResponseTypeDef](./type_defs.md#getannotationstoreversionresponsetypedef)
- [VersionOptionsTypeDef](./type_defs.md#versionoptionstypedef)
- [GetReadSetMetadataResponseTypeDef](./type_defs.md#getreadsetmetadataresponsetypedef)
- [GetReferenceMetadataResponseTypeDef](./type_defs.md#getreferencemetadataresponsetypedef)
- [GetAnnotationImportResponseTypeDef](./type_defs.md#getannotationimportresponsetypedef)
- [StartAnnotationImportRequestRequestTypeDef](./type_defs.md#startannotationimportrequestrequesttypedef)
- [CreateAnnotationStoreRequestRequestTypeDef](./type_defs.md#createannotationstorerequestrequesttypedef)
- [CreateAnnotationStoreVersionRequestRequestTypeDef](./type_defs.md#createannotationstoreversionrequestrequesttypedef)

