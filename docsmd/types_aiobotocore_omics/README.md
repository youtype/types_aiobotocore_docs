# Omics module

> [Index](../README.md) > Omics


!!! note ""

    Auto-generated documentation for [Omics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
    type annotations stubs module [types-aiobotocore-omics](https://pypi.org/project/types-aiobotocore-omics/).

## How to install



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
- [ListRunGroupsPaginator](./paginators.md#listrungroupspaginator)
- [ListRunTasksPaginator](./paginators.md#listruntaskspaginator)
- [ListRunsPaginator](./paginators.md#listrunspaginator)
- [ListSequenceStoresPaginator](./paginators.md#listsequencestorespaginator)
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
- [AnnotationTypeType](./literals.md#annotationtypetype)
- [CreationTypeType](./literals.md#creationtypetype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [FileTypeType](./literals.md#filetypetype)
- [FormatToHeaderKeyType](./literals.md#formattoheaderkeytype)
- [JobStatusType](./literals.md#jobstatustype)
- [ListAnnotationImportJobsPaginatorName](./literals.md#listannotationimportjobspaginatorname)
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
- [ListRunGroupsPaginatorName](./literals.md#listrungroupspaginatorname)
- [ListRunTasksPaginatorName](./literals.md#listruntaskspaginatorname)
- [ListRunsPaginatorName](./literals.md#listrunspaginatorname)
- [ListSequenceStoresPaginatorName](./literals.md#listsequencestorespaginatorname)
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
- [ReferenceFileType](./literals.md#referencefiletype)
- [ReferenceImportJobCompletedWaiterName](./literals.md#referenceimportjobcompletedwaitername)
- [ReferenceImportJobItemStatusType](./literals.md#referenceimportjobitemstatustype)
- [ReferenceImportJobStatusType](./literals.md#referenceimportjobstatustype)
- [ReferenceStatusType](./literals.md#referencestatustype)
- [RunCompletedWaiterName](./literals.md#runcompletedwaitername)
- [RunExportType](./literals.md#runexporttype)
- [RunLogLevelType](./literals.md#runlogleveltype)
- [RunRunningWaiterName](./literals.md#runrunningwaitername)
- [RunStatusType](./literals.md#runstatustype)
- [SchemaValueTypeType](./literals.md#schemavaluetypetype)
- [StoreFormatType](./literals.md#storeformattype)
- [StoreStatusType](./literals.md#storestatustype)
- [TaskCompletedWaiterName](./literals.md#taskcompletedwaitername)
- [TaskRunningWaiterName](./literals.md#taskrunningwaitername)
- [TaskStatusType](./literals.md#taskstatustype)
- [VariantImportJobCreatedWaiterName](./literals.md#variantimportjobcreatedwaitername)
- [VariantStoreCreatedWaiterName](./literals.md#variantstorecreatedwaitername)
- [VariantStoreDeletedWaiterName](./literals.md#variantstoredeletedwaitername)
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
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ActivateReadSetJobItemTypeDef](./type_defs.md#activatereadsetjobitemtypedef)
- [ActivateReadSetSourceItemTypeDef](./type_defs.md#activatereadsetsourceitemtypedef)
- [AnnotationImportItemDetailTypeDef](./type_defs.md#annotationimportitemdetailtypedef)
- [AnnotationImportItemSourceTypeDef](./type_defs.md#annotationimportitemsourcetypedef)
- [AnnotationImportJobItemTypeDef](./type_defs.md#annotationimportjobitemtypedef)
- [ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef)
- [SseConfigTypeDef](./type_defs.md#sseconfigtypedef)
- [BatchDeleteReadSetRequestRequestTypeDef](./type_defs.md#batchdeletereadsetrequestrequesttypedef)
- [ReadSetBatchErrorTypeDef](./type_defs.md#readsetbatcherrortypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CancelAnnotationImportRequestRequestTypeDef](./type_defs.md#cancelannotationimportrequestrequesttypedef)
- [CancelRunRequestRequestTypeDef](./type_defs.md#cancelrunrequestrequesttypedef)
- [CancelVariantImportRequestRequestTypeDef](./type_defs.md#cancelvariantimportrequestrequesttypedef)
- [CompleteReadSetUploadPartListItemTypeDef](./type_defs.md#completereadsetuploadpartlistitemtypedef)
- [CreateMultipartReadSetUploadRequestRequestTypeDef](./type_defs.md#createmultipartreadsetuploadrequestrequesttypedef)
- [CreateRunGroupRequestRequestTypeDef](./type_defs.md#createrungrouprequestrequesttypedef)
- [WorkflowParameterTypeDef](./type_defs.md#workflowparametertypedef)
- [DeleteAnnotationStoreRequestRequestTypeDef](./type_defs.md#deleteannotationstorerequestrequesttypedef)
- [DeleteReferenceRequestRequestTypeDef](./type_defs.md#deletereferencerequestrequesttypedef)
- [DeleteReferenceStoreRequestRequestTypeDef](./type_defs.md#deletereferencestorerequestrequesttypedef)
- [DeleteRunGroupRequestRequestTypeDef](./type_defs.md#deleterungrouprequestrequesttypedef)
- [DeleteRunRequestRequestTypeDef](./type_defs.md#deleterunrequestrequesttypedef)
- [DeleteSequenceStoreRequestRequestTypeDef](./type_defs.md#deletesequencestorerequestrequesttypedef)
- [DeleteVariantStoreRequestRequestTypeDef](./type_defs.md#deletevariantstorerequestrequesttypedef)
- [DeleteWorkflowRequestRequestTypeDef](./type_defs.md#deleteworkflowrequestrequesttypedef)
- [ExportReadSetDetailTypeDef](./type_defs.md#exportreadsetdetailtypedef)
- [ExportReadSetJobDetailTypeDef](./type_defs.md#exportreadsetjobdetailtypedef)
- [ExportReadSetTypeDef](./type_defs.md#exportreadsettypedef)
- [FileInformationTypeDef](./type_defs.md#fileinformationtypedef)
- [VcfOptionsTypeDef](./type_defs.md#vcfoptionstypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [GetAnnotationImportRequestRequestTypeDef](./type_defs.md#getannotationimportrequestrequesttypedef)
- [GetAnnotationStoreRequestRequestTypeDef](./type_defs.md#getannotationstorerequestrequesttypedef)
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
- [GetRunGroupRequestRequestTypeDef](./type_defs.md#getrungrouprequestrequesttypedef)
- [GetRunRequestRequestTypeDef](./type_defs.md#getrunrequestrequesttypedef)
- [GetRunTaskRequestRequestTypeDef](./type_defs.md#getruntaskrequestrequesttypedef)
- [GetSequenceStoreRequestRequestTypeDef](./type_defs.md#getsequencestorerequestrequesttypedef)
- [GetVariantImportRequestRequestTypeDef](./type_defs.md#getvariantimportrequestrequesttypedef)
- [VariantImportItemDetailTypeDef](./type_defs.md#variantimportitemdetailtypedef)
- [GetVariantStoreRequestRequestTypeDef](./type_defs.md#getvariantstorerequestrequesttypedef)
- [GetWorkflowRequestRequestTypeDef](./type_defs.md#getworkflowrequestrequesttypedef)
- [ImportReadSetJobItemTypeDef](./type_defs.md#importreadsetjobitemtypedef)
- [SourceFilesTypeDef](./type_defs.md#sourcefilestypedef)
- [ImportReferenceJobItemTypeDef](./type_defs.md#importreferencejobitemtypedef)
- [ListAnnotationImportJobsFilterTypeDef](./type_defs.md#listannotationimportjobsfiltertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAnnotationStoresFilterTypeDef](./type_defs.md#listannotationstoresfiltertypedef)
- [ListMultipartReadSetUploadsRequestRequestTypeDef](./type_defs.md#listmultipartreadsetuploadsrequestrequesttypedef)
- [MultipartReadSetUploadListItemTypeDef](./type_defs.md#multipartreadsetuploadlistitemtypedef)
- [ReadSetUploadPartListItemTypeDef](./type_defs.md#readsetuploadpartlistitemtypedef)
- [ReferenceListItemTypeDef](./type_defs.md#referencelistitemtypedef)
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
- [ReadOptionsTypeDef](./type_defs.md#readoptionstypedef)
- [StartReadSetActivationJobSourceItemTypeDef](./type_defs.md#startreadsetactivationjobsourceitemtypedef)
- [StartReferenceImportJobSourceItemTypeDef](./type_defs.md#startreferenceimportjobsourceitemtypedef)
- [StartRunRequestRequestTypeDef](./type_defs.md#startrunrequestrequesttypedef)
- [VariantImportItemSourceTypeDef](./type_defs.md#variantimportitemsourcetypedef)
- [TsvStoreOptionsTypeDef](./type_defs.md#tsvstoreoptionstypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAnnotationStoreRequestRequestTypeDef](./type_defs.md#updateannotationstorerequestrequesttypedef)
- [UpdateRunGroupRequestRequestTypeDef](./type_defs.md#updaterungrouprequestrequesttypedef)
- [UpdateVariantStoreRequestRequestTypeDef](./type_defs.md#updatevariantstorerequestrequesttypedef)
- [UpdateWorkflowRequestRequestTypeDef](./type_defs.md#updateworkflowrequestrequesttypedef)
- [ActivateReadSetFilterTypeDef](./type_defs.md#activatereadsetfiltertypedef)
- [ExportReadSetFilterTypeDef](./type_defs.md#exportreadsetfiltertypedef)
- [ImportReadSetFilterTypeDef](./type_defs.md#importreadsetfiltertypedef)
- [ImportReferenceFilterTypeDef](./type_defs.md#importreferencefiltertypedef)
- [ReadSetFilterTypeDef](./type_defs.md#readsetfiltertypedef)
- [ReadSetUploadPartListFilterTypeDef](./type_defs.md#readsetuploadpartlistfiltertypedef)
- [ReferenceFilterTypeDef](./type_defs.md#referencefiltertypedef)
- [ReferenceStoreFilterTypeDef](./type_defs.md#referencestorefiltertypedef)
- [SequenceStoreFilterTypeDef](./type_defs.md#sequencestorefiltertypedef)
- [AnnotationStoreItemTypeDef](./type_defs.md#annotationstoreitemtypedef)
- [CreateReferenceStoreRequestRequestTypeDef](./type_defs.md#createreferencestorerequestrequesttypedef)
- [CreateSequenceStoreRequestRequestTypeDef](./type_defs.md#createsequencestorerequestrequesttypedef)
- [CreateVariantStoreRequestRequestTypeDef](./type_defs.md#createvariantstorerequestrequesttypedef)
- [ReferenceStoreDetailTypeDef](./type_defs.md#referencestoredetailtypedef)
- [SequenceStoreDetailTypeDef](./type_defs.md#sequencestoredetailtypedef)
- [VariantStoreItemTypeDef](./type_defs.md#variantstoreitemtypedef)
- [BatchDeleteReadSetResponseTypeDef](./type_defs.md#batchdeletereadsetresponsetypedef)
- [CompleteMultipartReadSetUploadResponseTypeDef](./type_defs.md#completemultipartreadsetuploadresponsetypedef)
- [CreateMultipartReadSetUploadResponseTypeDef](./type_defs.md#createmultipartreadsetuploadresponsetypedef)
- [CreateReferenceStoreResponseTypeDef](./type_defs.md#createreferencestoreresponsetypedef)
- [CreateRunGroupResponseTypeDef](./type_defs.md#createrungroupresponsetypedef)
- [CreateSequenceStoreResponseTypeDef](./type_defs.md#createsequencestoreresponsetypedef)
- [CreateVariantStoreResponseTypeDef](./type_defs.md#createvariantstoreresponsetypedef)
- [CreateWorkflowResponseTypeDef](./type_defs.md#createworkflowresponsetypedef)
- [DeleteAnnotationStoreResponseTypeDef](./type_defs.md#deleteannotationstoreresponsetypedef)
- [DeleteVariantStoreResponseTypeDef](./type_defs.md#deletevariantstoreresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetReadSetActivationJobResponseTypeDef](./type_defs.md#getreadsetactivationjobresponsetypedef)
- [GetReadSetResponseTypeDef](./type_defs.md#getreadsetresponsetypedef)
- [GetReferenceResponseTypeDef](./type_defs.md#getreferenceresponsetypedef)
- [GetReferenceStoreResponseTypeDef](./type_defs.md#getreferencestoreresponsetypedef)
- [GetRunGroupResponseTypeDef](./type_defs.md#getrungroupresponsetypedef)
- [GetRunResponseTypeDef](./type_defs.md#getrunresponsetypedef)
- [GetRunTaskResponseTypeDef](./type_defs.md#getruntaskresponsetypedef)
- [GetSequenceStoreResponseTypeDef](./type_defs.md#getsequencestoreresponsetypedef)
- [GetVariantStoreResponseTypeDef](./type_defs.md#getvariantstoreresponsetypedef)
- [ListAnnotationImportJobsResponseTypeDef](./type_defs.md#listannotationimportjobsresponsetypedef)
- [ListReadSetActivationJobsResponseTypeDef](./type_defs.md#listreadsetactivationjobsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartAnnotationImportResponseTypeDef](./type_defs.md#startannotationimportresponsetypedef)
- [StartReadSetActivationJobResponseTypeDef](./type_defs.md#startreadsetactivationjobresponsetypedef)
- [StartReadSetExportJobResponseTypeDef](./type_defs.md#startreadsetexportjobresponsetypedef)
- [StartReadSetImportJobResponseTypeDef](./type_defs.md#startreadsetimportjobresponsetypedef)
- [StartReferenceImportJobResponseTypeDef](./type_defs.md#startreferenceimportjobresponsetypedef)
- [StartRunResponseTypeDef](./type_defs.md#startrunresponsetypedef)
- [StartVariantImportResponseTypeDef](./type_defs.md#startvariantimportresponsetypedef)
- [UpdateVariantStoreResponseTypeDef](./type_defs.md#updatevariantstoreresponsetypedef)
- [UploadReadSetPartResponseTypeDef](./type_defs.md#uploadreadsetpartresponsetypedef)
- [UploadReadSetPartRequestRequestTypeDef](./type_defs.md#uploadreadsetpartrequestrequesttypedef)
- [CompleteMultipartReadSetUploadRequestRequestTypeDef](./type_defs.md#completemultipartreadsetuploadrequestrequesttypedef)
- [CreateWorkflowRequestRequestTypeDef](./type_defs.md#createworkflowrequestrequesttypedef)
- [GetWorkflowResponseTypeDef](./type_defs.md#getworkflowresponsetypedef)
- [GetReadSetExportJobResponseTypeDef](./type_defs.md#getreadsetexportjobresponsetypedef)
- [ListReadSetExportJobsResponseTypeDef](./type_defs.md#listreadsetexportjobsresponsetypedef)
- [StartReadSetExportJobRequestRequestTypeDef](./type_defs.md#startreadsetexportjobrequestrequesttypedef)
- [ReadSetFilesTypeDef](./type_defs.md#readsetfilestypedef)
- [ReferenceFilesTypeDef](./type_defs.md#referencefilestypedef)
- [GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef](./type_defs.md#getannotationimportrequestannotationimportjobcreatedwaittypedef)
- [GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef](./type_defs.md#getannotationstorerequestannotationstorecreatedwaittypedef)
- [GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef](./type_defs.md#getannotationstorerequestannotationstoredeletedwaittypedef)
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
- [GetVariantImportResponseTypeDef](./type_defs.md#getvariantimportresponsetypedef)
- [ListReadSetImportJobsResponseTypeDef](./type_defs.md#listreadsetimportjobsresponsetypedef)
- [ImportReadSetSourceItemTypeDef](./type_defs.md#importreadsetsourceitemtypedef)
- [StartReadSetImportJobSourceItemTypeDef](./type_defs.md#startreadsetimportjobsourceitemtypedef)
- [ListReferenceImportJobsResponseTypeDef](./type_defs.md#listreferenceimportjobsresponsetypedef)
- [ListAnnotationImportJobsRequestRequestTypeDef](./type_defs.md#listannotationimportjobsrequestrequesttypedef)
- [ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef](./type_defs.md#listannotationimportjobsrequestlistannotationimportjobspaginatetypedef)
- [ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef](./type_defs.md#listmultipartreadsetuploadsrequestlistmultipartreadsetuploadspaginatetypedef)
- [ListRunGroupsRequestListRunGroupsPaginateTypeDef](./type_defs.md#listrungroupsrequestlistrungroupspaginatetypedef)
- [ListRunTasksRequestListRunTasksPaginateTypeDef](./type_defs.md#listruntasksrequestlistruntaskspaginatetypedef)
- [ListRunsRequestListRunsPaginateTypeDef](./type_defs.md#listrunsrequestlistrunspaginatetypedef)
- [ListWorkflowsRequestListWorkflowsPaginateTypeDef](./type_defs.md#listworkflowsrequestlistworkflowspaginatetypedef)
- [ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef](./type_defs.md#listannotationstoresrequestlistannotationstorespaginatetypedef)
- [ListAnnotationStoresRequestRequestTypeDef](./type_defs.md#listannotationstoresrequestrequesttypedef)
- [ListMultipartReadSetUploadsResponseTypeDef](./type_defs.md#listmultipartreadsetuploadsresponsetypedef)
- [ListReadSetUploadPartsResponseTypeDef](./type_defs.md#listreadsetuploadpartsresponsetypedef)
- [ListReferencesResponseTypeDef](./type_defs.md#listreferencesresponsetypedef)
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
- [StoreOptionsTypeDef](./type_defs.md#storeoptionstypedef)
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
- [GetReadSetMetadataResponseTypeDef](./type_defs.md#getreadsetmetadataresponsetypedef)
- [GetReferenceMetadataResponseTypeDef](./type_defs.md#getreferencemetadataresponsetypedef)
- [ListReadSetsResponseTypeDef](./type_defs.md#listreadsetsresponsetypedef)
- [GetReadSetImportJobResponseTypeDef](./type_defs.md#getreadsetimportjobresponsetypedef)
- [StartReadSetImportJobRequestRequestTypeDef](./type_defs.md#startreadsetimportjobrequestrequesttypedef)
- [FormatOptionsTypeDef](./type_defs.md#formatoptionstypedef)
- [CreateAnnotationStoreRequestRequestTypeDef](./type_defs.md#createannotationstorerequestrequesttypedef)
- [CreateAnnotationStoreResponseTypeDef](./type_defs.md#createannotationstoreresponsetypedef)
- [GetAnnotationStoreResponseTypeDef](./type_defs.md#getannotationstoreresponsetypedef)
- [UpdateAnnotationStoreResponseTypeDef](./type_defs.md#updateannotationstoreresponsetypedef)
- [GetAnnotationImportResponseTypeDef](./type_defs.md#getannotationimportresponsetypedef)
- [StartAnnotationImportRequestRequestTypeDef](./type_defs.md#startannotationimportrequestrequesttypedef)

