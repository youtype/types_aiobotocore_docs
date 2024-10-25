# OmicsClient

> [Index](../README.md) > [Omics](./README.md) > OmicsClient

!!! note ""

    Auto-generated documentation for [Omics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
    type annotations stubs module [types-aiobotocore-omics](https://pypi.org/project/types-aiobotocore-omics/).

## OmicsClient

Type annotations and code completion for `#!python session.create_client("omics")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client)

```python
# OmicsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_omics.client import OmicsClient

session = get_session()
async with session.create_client("omics") as client:
    client: OmicsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("omics").exceptions` structure.

```python
# OmicsClient.exceptions usage example

async with session.create_client("omics") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.NotSupportedOperationException,
        client.RangeNotSatisfiableException,
        client.RequestTimeoutException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# OmicsClient usage type checking example

from types_aiobotocore_omics.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### abort\_multipart\_read\_set\_upload

Stops a multipart upload.

Type annotations and code completion for `#!python session.create_client("omics").abort_multipart_read_set_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.abort_multipart_read_set_upload)

```python
# abort_multipart_read_set_upload method definition

await def abort_multipart_read_set_upload(
    self,
    *,
    sequenceStoreId: str,
    uploadId: str,
) -> Dict[str, Any]:
    ...
```



```python
# abort_multipart_read_set_upload method usage example with argument unpacking

kwargs: AbortMultipartReadSetUploadRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
    "uploadId": ...,
}

parent.abort_multipart_read_set_upload(**kwargs)
```

1. See [:material-code-braces: AbortMultipartReadSetUploadRequestRequestTypeDef](./type_defs.md#abortmultipartreadsetuploadrequestrequesttypedef) 

### accept\_share

Accept a resource share request.

Type annotations and code completion for `#!python session.create_client("omics").accept_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.accept_share)

```python
# accept_share method definition

await def accept_share(
    self,
    *,
    shareId: str,
) -> AcceptShareResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AcceptShareResponseTypeDef](./type_defs.md#acceptshareresponsetypedef) 


```python
# accept_share method usage example with argument unpacking

kwargs: AcceptShareRequestRequestTypeDef = {  # (1)
    "shareId": ...,
}

parent.accept_share(**kwargs)
```

1. See [:material-code-braces: AcceptShareRequestRequestTypeDef](./type_defs.md#acceptsharerequestrequesttypedef) 

### batch\_delete\_read\_set

Deletes one or more read sets.

Type annotations and code completion for `#!python session.create_client("omics").batch_delete_read_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.batch_delete_read_set)

```python
# batch_delete_read_set method definition

await def batch_delete_read_set(
    self,
    *,
    ids: Sequence[str],
    sequenceStoreId: str,
) -> BatchDeleteReadSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteReadSetResponseTypeDef](./type_defs.md#batchdeletereadsetresponsetypedef) 


```python
# batch_delete_read_set method usage example with argument unpacking

kwargs: BatchDeleteReadSetRequestRequestTypeDef = {  # (1)
    "ids": ...,
    "sequenceStoreId": ...,
}

parent.batch_delete_read_set(**kwargs)
```

1. See [:material-code-braces: BatchDeleteReadSetRequestRequestTypeDef](./type_defs.md#batchdeletereadsetrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("omics").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_annotation\_import\_job

Cancels an annotation import job.

Type annotations and code completion for `#!python session.create_client("omics").cancel_annotation_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.cancel_annotation_import_job)

```python
# cancel_annotation_import_job method definition

await def cancel_annotation_import_job(
    self,
    *,
    jobId: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_annotation_import_job method usage example with argument unpacking

kwargs: CancelAnnotationImportRequestRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.cancel_annotation_import_job(**kwargs)
```

1. See [:material-code-braces: CancelAnnotationImportRequestRequestTypeDef](./type_defs.md#cancelannotationimportrequestrequesttypedef) 

### cancel\_run

Cancels a run.

Type annotations and code completion for `#!python session.create_client("omics").cancel_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.cancel_run)

```python
# cancel_run method definition

await def cancel_run(
    self,
    *,
    id: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# cancel_run method usage example with argument unpacking

kwargs: CancelRunRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.cancel_run(**kwargs)
```

1. See [:material-code-braces: CancelRunRequestRequestTypeDef](./type_defs.md#cancelrunrequestrequesttypedef) 

### cancel\_variant\_import\_job

Cancels a variant import job.

Type annotations and code completion for `#!python session.create_client("omics").cancel_variant_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.cancel_variant_import_job)

```python
# cancel_variant_import_job method definition

await def cancel_variant_import_job(
    self,
    *,
    jobId: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_variant_import_job method usage example with argument unpacking

kwargs: CancelVariantImportRequestRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.cancel_variant_import_job(**kwargs)
```

1. See [:material-code-braces: CancelVariantImportRequestRequestTypeDef](./type_defs.md#cancelvariantimportrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("omics").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### complete\_multipart\_read\_set\_upload

Concludes a multipart upload once you have uploaded all the components.

Type annotations and code completion for `#!python session.create_client("omics").complete_multipart_read_set_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.complete_multipart_read_set_upload)

```python
# complete_multipart_read_set_upload method definition

await def complete_multipart_read_set_upload(
    self,
    *,
    sequenceStoreId: str,
    uploadId: str,
    parts: Sequence[CompleteReadSetUploadPartListItemTypeDef],  # (1)
) -> CompleteMultipartReadSetUploadResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CompleteReadSetUploadPartListItemTypeDef](./type_defs.md#completereadsetuploadpartlistitemtypedef) 
2. See [:material-code-braces: CompleteMultipartReadSetUploadResponseTypeDef](./type_defs.md#completemultipartreadsetuploadresponsetypedef) 


```python
# complete_multipart_read_set_upload method usage example with argument unpacking

kwargs: CompleteMultipartReadSetUploadRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
    "uploadId": ...,
    "parts": ...,
}

parent.complete_multipart_read_set_upload(**kwargs)
```

1. See [:material-code-braces: CompleteMultipartReadSetUploadRequestRequestTypeDef](./type_defs.md#completemultipartreadsetuploadrequestrequesttypedef) 

### create\_annotation\_store

Creates an annotation store.

Type annotations and code completion for `#!python session.create_client("omics").create_annotation_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store)

```python
# create_annotation_store method definition

await def create_annotation_store(
    self,
    *,
    storeFormat: StoreFormatType,  # (1)
    reference: ReferenceItemTypeDef = ...,  # (2)
    name: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
    versionName: str = ...,
    sseConfig: SseConfigTypeDef = ...,  # (3)
    storeOptions: StoreOptionsTypeDef = ...,  # (4)
) -> CreateAnnotationStoreResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: StoreFormatType](./literals.md#storeformattype) 
2. See [:material-code-braces: ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef) 
3. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
4. See [:material-code-braces: StoreOptionsTypeDef](./type_defs.md#storeoptionstypedef) 
5. See [:material-code-braces: CreateAnnotationStoreResponseTypeDef](./type_defs.md#createannotationstoreresponsetypedef) 


```python
# create_annotation_store method usage example with argument unpacking

kwargs: CreateAnnotationStoreRequestRequestTypeDef = {  # (1)
    "storeFormat": ...,
}

parent.create_annotation_store(**kwargs)
```

1. See [:material-code-braces: CreateAnnotationStoreRequestRequestTypeDef](./type_defs.md#createannotationstorerequestrequesttypedef) 

### create\_annotation\_store\_version

Creates a new version of an annotation store.

Type annotations and code completion for `#!python session.create_client("omics").create_annotation_store_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store_version)

```python
# create_annotation_store_version method definition

await def create_annotation_store_version(
    self,
    *,
    name: str,
    versionName: str,
    description: str = ...,
    versionOptions: VersionOptionsTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateAnnotationStoreVersionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VersionOptionsTypeDef](./type_defs.md#versionoptionstypedef) 
2. See [:material-code-braces: CreateAnnotationStoreVersionResponseTypeDef](./type_defs.md#createannotationstoreversionresponsetypedef) 


```python
# create_annotation_store_version method usage example with argument unpacking

kwargs: CreateAnnotationStoreVersionRequestRequestTypeDef = {  # (1)
    "name": ...,
    "versionName": ...,
}

parent.create_annotation_store_version(**kwargs)
```

1. See [:material-code-braces: CreateAnnotationStoreVersionRequestRequestTypeDef](./type_defs.md#createannotationstoreversionrequestrequesttypedef) 

### create\_multipart\_read\_set\_upload

Begins a multipart read set upload.

Type annotations and code completion for `#!python session.create_client("omics").create_multipart_read_set_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_multipart_read_set_upload)

```python
# create_multipart_read_set_upload method definition

await def create_multipart_read_set_upload(
    self,
    *,
    sequenceStoreId: str,
    sourceFileType: FileTypeType,  # (1)
    subjectId: str,
    sampleId: str,
    name: str,
    clientToken: str = ...,
    generatedFrom: str = ...,
    referenceArn: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateMultipartReadSetUploadResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FileTypeType](./literals.md#filetypetype) 
2. See [:material-code-braces: CreateMultipartReadSetUploadResponseTypeDef](./type_defs.md#createmultipartreadsetuploadresponsetypedef) 


```python
# create_multipart_read_set_upload method usage example with argument unpacking

kwargs: CreateMultipartReadSetUploadRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
    "sourceFileType": ...,
    "subjectId": ...,
    "sampleId": ...,
    "name": ...,
}

parent.create_multipart_read_set_upload(**kwargs)
```

1. See [:material-code-braces: CreateMultipartReadSetUploadRequestRequestTypeDef](./type_defs.md#createmultipartreadsetuploadrequestrequesttypedef) 

### create\_reference\_store

Creates a reference store.

Type annotations and code completion for `#!python session.create_client("omics").create_reference_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_reference_store)

```python
# create_reference_store method definition

await def create_reference_store(
    self,
    *,
    name: str,
    description: str = ...,
    sseConfig: SseConfigTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
    clientToken: str = ...,
) -> CreateReferenceStoreResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
2. See [:material-code-braces: CreateReferenceStoreResponseTypeDef](./type_defs.md#createreferencestoreresponsetypedef) 


```python
# create_reference_store method usage example with argument unpacking

kwargs: CreateReferenceStoreRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_reference_store(**kwargs)
```

1. See [:material-code-braces: CreateReferenceStoreRequestRequestTypeDef](./type_defs.md#createreferencestorerequestrequesttypedef) 

### create\_run\_group

You can optionally create a run group to limit the compute resources for the
runs that you add to the
group.

Type annotations and code completion for `#!python session.create_client("omics").create_run_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_run_group)

```python
# create_run_group method definition

await def create_run_group(
    self,
    *,
    requestId: str,
    name: str = ...,
    maxCpus: int = ...,
    maxRuns: int = ...,
    maxDuration: int = ...,
    tags: Mapping[str, str] = ...,
    maxGpus: int = ...,
) -> CreateRunGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateRunGroupResponseTypeDef](./type_defs.md#createrungroupresponsetypedef) 


```python
# create_run_group method usage example with argument unpacking

kwargs: CreateRunGroupRequestRequestTypeDef = {  # (1)
    "requestId": ...,
}

parent.create_run_group(**kwargs)
```

1. See [:material-code-braces: CreateRunGroupRequestRequestTypeDef](./type_defs.md#createrungrouprequestrequesttypedef) 

### create\_sequence\_store

Creates a sequence store.

Type annotations and code completion for `#!python session.create_client("omics").create_sequence_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_sequence_store)

```python
# create_sequence_store method definition

await def create_sequence_store(
    self,
    *,
    name: str,
    description: str = ...,
    sseConfig: SseConfigTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
    clientToken: str = ...,
    fallbackLocation: str = ...,
    eTagAlgorithmFamily: ETagAlgorithmFamilyType = ...,  # (2)
) -> CreateSequenceStoreResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
2. See [:material-code-brackets: ETagAlgorithmFamilyType](./literals.md#etagalgorithmfamilytype) 
3. See [:material-code-braces: CreateSequenceStoreResponseTypeDef](./type_defs.md#createsequencestoreresponsetypedef) 


```python
# create_sequence_store method usage example with argument unpacking

kwargs: CreateSequenceStoreRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_sequence_store(**kwargs)
```

1. See [:material-code-braces: CreateSequenceStoreRequestRequestTypeDef](./type_defs.md#createsequencestorerequestrequesttypedef) 

### create\_share

Creates a cross-account shared resource.

Type annotations and code completion for `#!python session.create_client("omics").create_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_share)

```python
# create_share method definition

await def create_share(
    self,
    *,
    resourceArn: str,
    principalSubscriber: str,
    shareName: str = ...,
) -> CreateShareResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateShareResponseTypeDef](./type_defs.md#createshareresponsetypedef) 


```python
# create_share method usage example with argument unpacking

kwargs: CreateShareRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "principalSubscriber": ...,
}

parent.create_share(**kwargs)
```

1. See [:material-code-braces: CreateShareRequestRequestTypeDef](./type_defs.md#createsharerequestrequesttypedef) 

### create\_variant\_store

Creates a variant store.

Type annotations and code completion for `#!python session.create_client("omics").create_variant_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_variant_store)

```python
# create_variant_store method definition

await def create_variant_store(
    self,
    *,
    reference: ReferenceItemTypeDef,  # (1)
    name: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
    sseConfig: SseConfigTypeDef = ...,  # (2)
) -> CreateVariantStoreResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef) 
2. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
3. See [:material-code-braces: CreateVariantStoreResponseTypeDef](./type_defs.md#createvariantstoreresponsetypedef) 


```python
# create_variant_store method usage example with argument unpacking

kwargs: CreateVariantStoreRequestRequestTypeDef = {  # (1)
    "reference": ...,
}

parent.create_variant_store(**kwargs)
```

1. See [:material-code-braces: CreateVariantStoreRequestRequestTypeDef](./type_defs.md#createvariantstorerequestrequesttypedef) 

### create\_workflow

Creates a workflow.

Type annotations and code completion for `#!python session.create_client("omics").create_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_workflow)

```python
# create_workflow method definition

await def create_workflow(
    self,
    *,
    requestId: str,
    name: str = ...,
    description: str = ...,
    engine: WorkflowEngineType = ...,  # (1)
    definitionZip: BlobTypeDef = ...,
    definitionUri: str = ...,
    main: str = ...,
    parameterTemplate: Mapping[str, WorkflowParameterTypeDef] = ...,  # (2)
    storageCapacity: int = ...,
    tags: Mapping[str, str] = ...,
    accelerators: AcceleratorsType = ...,  # (3)
) -> CreateWorkflowResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: WorkflowEngineType](./literals.md#workflowenginetype) 
2. See [:material-code-braces: WorkflowParameterTypeDef](./type_defs.md#workflowparametertypedef) 
3. See [:material-code-brackets: AcceleratorsType](./literals.md#acceleratorstype) 
4. See [:material-code-braces: CreateWorkflowResponseTypeDef](./type_defs.md#createworkflowresponsetypedef) 


```python
# create_workflow method usage example with argument unpacking

kwargs: CreateWorkflowRequestRequestTypeDef = {  # (1)
    "requestId": ...,
}

parent.create_workflow(**kwargs)
```

1. See [:material-code-braces: CreateWorkflowRequestRequestTypeDef](./type_defs.md#createworkflowrequestrequesttypedef) 

### delete\_annotation\_store

Deletes an annotation store.

Type annotations and code completion for `#!python session.create_client("omics").delete_annotation_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.delete_annotation_store)

```python
# delete_annotation_store method definition

await def delete_annotation_store(
    self,
    *,
    name: str,
    force: bool = ...,
) -> DeleteAnnotationStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAnnotationStoreResponseTypeDef](./type_defs.md#deleteannotationstoreresponsetypedef) 


```python
# delete_annotation_store method usage example with argument unpacking

kwargs: DeleteAnnotationStoreRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_annotation_store(**kwargs)
```

1. See [:material-code-braces: DeleteAnnotationStoreRequestRequestTypeDef](./type_defs.md#deleteannotationstorerequestrequesttypedef) 

### delete\_annotation\_store\_versions

Deletes one or multiple versions of an annotation store.

Type annotations and code completion for `#!python session.create_client("omics").delete_annotation_store_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.delete_annotation_store_versions)

```python
# delete_annotation_store_versions method definition

await def delete_annotation_store_versions(
    self,
    *,
    name: str,
    versions: Sequence[str],
    force: bool = ...,
) -> DeleteAnnotationStoreVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAnnotationStoreVersionsResponseTypeDef](./type_defs.md#deleteannotationstoreversionsresponsetypedef) 


```python
# delete_annotation_store_versions method usage example with argument unpacking

kwargs: DeleteAnnotationStoreVersionsRequestRequestTypeDef = {  # (1)
    "name": ...,
    "versions": ...,
}

parent.delete_annotation_store_versions(**kwargs)
```

1. See [:material-code-braces: DeleteAnnotationStoreVersionsRequestRequestTypeDef](./type_defs.md#deleteannotationstoreversionsrequestrequesttypedef) 

### delete\_reference

Deletes a genome reference.

Type annotations and code completion for `#!python session.create_client("omics").delete_reference` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.delete_reference)

```python
# delete_reference method definition

await def delete_reference(
    self,
    *,
    id: str,
    referenceStoreId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_reference method usage example with argument unpacking

kwargs: DeleteReferenceRequestRequestTypeDef = {  # (1)
    "id": ...,
    "referenceStoreId": ...,
}

parent.delete_reference(**kwargs)
```

1. See [:material-code-braces: DeleteReferenceRequestRequestTypeDef](./type_defs.md#deletereferencerequestrequesttypedef) 

### delete\_reference\_store

Deletes a genome reference store.

Type annotations and code completion for `#!python session.create_client("omics").delete_reference_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.delete_reference_store)

```python
# delete_reference_store method definition

await def delete_reference_store(
    self,
    *,
    id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_reference_store method usage example with argument unpacking

kwargs: DeleteReferenceStoreRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_reference_store(**kwargs)
```

1. See [:material-code-braces: DeleteReferenceStoreRequestRequestTypeDef](./type_defs.md#deletereferencestorerequestrequesttypedef) 

### delete\_run

Deletes a workflow run.

Type annotations and code completion for `#!python session.create_client("omics").delete_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.delete_run)

```python
# delete_run method definition

await def delete_run(
    self,
    *,
    id: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_run method usage example with argument unpacking

kwargs: DeleteRunRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_run(**kwargs)
```

1. See [:material-code-braces: DeleteRunRequestRequestTypeDef](./type_defs.md#deleterunrequestrequesttypedef) 

### delete\_run\_group

Deletes a workflow run group.

Type annotations and code completion for `#!python session.create_client("omics").delete_run_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.delete_run_group)

```python
# delete_run_group method definition

await def delete_run_group(
    self,
    *,
    id: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_run_group method usage example with argument unpacking

kwargs: DeleteRunGroupRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_run_group(**kwargs)
```

1. See [:material-code-braces: DeleteRunGroupRequestRequestTypeDef](./type_defs.md#deleterungrouprequestrequesttypedef) 

### delete\_sequence\_store

Deletes a sequence store.

Type annotations and code completion for `#!python session.create_client("omics").delete_sequence_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.delete_sequence_store)

```python
# delete_sequence_store method definition

await def delete_sequence_store(
    self,
    *,
    id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_sequence_store method usage example with argument unpacking

kwargs: DeleteSequenceStoreRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_sequence_store(**kwargs)
```

1. See [:material-code-braces: DeleteSequenceStoreRequestRequestTypeDef](./type_defs.md#deletesequencestorerequestrequesttypedef) 

### delete\_share

Deletes a resource share.

Type annotations and code completion for `#!python session.create_client("omics").delete_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.delete_share)

```python
# delete_share method definition

await def delete_share(
    self,
    *,
    shareId: str,
) -> DeleteShareResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteShareResponseTypeDef](./type_defs.md#deleteshareresponsetypedef) 


```python
# delete_share method usage example with argument unpacking

kwargs: DeleteShareRequestRequestTypeDef = {  # (1)
    "shareId": ...,
}

parent.delete_share(**kwargs)
```

1. See [:material-code-braces: DeleteShareRequestRequestTypeDef](./type_defs.md#deletesharerequestrequesttypedef) 

### delete\_variant\_store

Deletes a variant store.

Type annotations and code completion for `#!python session.create_client("omics").delete_variant_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.delete_variant_store)

```python
# delete_variant_store method definition

await def delete_variant_store(
    self,
    *,
    name: str,
    force: bool = ...,
) -> DeleteVariantStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteVariantStoreResponseTypeDef](./type_defs.md#deletevariantstoreresponsetypedef) 


```python
# delete_variant_store method usage example with argument unpacking

kwargs: DeleteVariantStoreRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_variant_store(**kwargs)
```

1. See [:material-code-braces: DeleteVariantStoreRequestRequestTypeDef](./type_defs.md#deletevariantstorerequestrequesttypedef) 

### delete\_workflow

Deletes a workflow.

Type annotations and code completion for `#!python session.create_client("omics").delete_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.delete_workflow)

```python
# delete_workflow method definition

await def delete_workflow(
    self,
    *,
    id: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_workflow method usage example with argument unpacking

kwargs: DeleteWorkflowRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_workflow(**kwargs)
```

1. See [:material-code-braces: DeleteWorkflowRequestRequestTypeDef](./type_defs.md#deleteworkflowrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("omics").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_annotation\_import\_job

Gets information about an annotation import job.

Type annotations and code completion for `#!python session.create_client("omics").get_annotation_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_annotation_import_job)

```python
# get_annotation_import_job method definition

await def get_annotation_import_job(
    self,
    *,
    jobId: str,
) -> GetAnnotationImportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAnnotationImportResponseTypeDef](./type_defs.md#getannotationimportresponsetypedef) 


```python
# get_annotation_import_job method usage example with argument unpacking

kwargs: GetAnnotationImportRequestRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.get_annotation_import_job(**kwargs)
```

1. See [:material-code-braces: GetAnnotationImportRequestRequestTypeDef](./type_defs.md#getannotationimportrequestrequesttypedef) 

### get\_annotation\_store

Gets information about an annotation store.

Type annotations and code completion for `#!python session.create_client("omics").get_annotation_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_annotation_store)

```python
# get_annotation_store method definition

await def get_annotation_store(
    self,
    *,
    name: str,
) -> GetAnnotationStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAnnotationStoreResponseTypeDef](./type_defs.md#getannotationstoreresponsetypedef) 


```python
# get_annotation_store method usage example with argument unpacking

kwargs: GetAnnotationStoreRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.get_annotation_store(**kwargs)
```

1. See [:material-code-braces: GetAnnotationStoreRequestRequestTypeDef](./type_defs.md#getannotationstorerequestrequesttypedef) 

### get\_annotation\_store\_version

Retrieves the metadata for an annotation store version.

Type annotations and code completion for `#!python session.create_client("omics").get_annotation_store_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_annotation_store_version)

```python
# get_annotation_store_version method definition

await def get_annotation_store_version(
    self,
    *,
    name: str,
    versionName: str,
) -> GetAnnotationStoreVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAnnotationStoreVersionResponseTypeDef](./type_defs.md#getannotationstoreversionresponsetypedef) 


```python
# get_annotation_store_version method usage example with argument unpacking

kwargs: GetAnnotationStoreVersionRequestRequestTypeDef = {  # (1)
    "name": ...,
    "versionName": ...,
}

parent.get_annotation_store_version(**kwargs)
```

1. See [:material-code-braces: GetAnnotationStoreVersionRequestRequestTypeDef](./type_defs.md#getannotationstoreversionrequestrequesttypedef) 

### get\_read\_set

Gets a file from a read set.

Type annotations and code completion for `#!python session.create_client("omics").get_read_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_read_set)

```python
# get_read_set method definition

await def get_read_set(
    self,
    *,
    id: str,
    sequenceStoreId: str,
    partNumber: int,
    file: ReadSetFileType = ...,  # (1)
) -> GetReadSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ReadSetFileType](./literals.md#readsetfiletype) 
2. See [:material-code-braces: GetReadSetResponseTypeDef](./type_defs.md#getreadsetresponsetypedef) 


```python
# get_read_set method usage example with argument unpacking

kwargs: GetReadSetRequestRequestTypeDef = {  # (1)
    "id": ...,
    "sequenceStoreId": ...,
    "partNumber": ...,
}

parent.get_read_set(**kwargs)
```

1. See [:material-code-braces: GetReadSetRequestRequestTypeDef](./type_defs.md#getreadsetrequestrequesttypedef) 

### get\_read\_set\_activation\_job

Gets information about a read set activation job.

Type annotations and code completion for `#!python session.create_client("omics").get_read_set_activation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_read_set_activation_job)

```python
# get_read_set_activation_job method definition

await def get_read_set_activation_job(
    self,
    *,
    id: str,
    sequenceStoreId: str,
) -> GetReadSetActivationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReadSetActivationJobResponseTypeDef](./type_defs.md#getreadsetactivationjobresponsetypedef) 


```python
# get_read_set_activation_job method usage example with argument unpacking

kwargs: GetReadSetActivationJobRequestRequestTypeDef = {  # (1)
    "id": ...,
    "sequenceStoreId": ...,
}

parent.get_read_set_activation_job(**kwargs)
```

1. See [:material-code-braces: GetReadSetActivationJobRequestRequestTypeDef](./type_defs.md#getreadsetactivationjobrequestrequesttypedef) 

### get\_read\_set\_export\_job

Gets information about a read set export job.

Type annotations and code completion for `#!python session.create_client("omics").get_read_set_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_read_set_export_job)

```python
# get_read_set_export_job method definition

await def get_read_set_export_job(
    self,
    *,
    sequenceStoreId: str,
    id: str,
) -> GetReadSetExportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReadSetExportJobResponseTypeDef](./type_defs.md#getreadsetexportjobresponsetypedef) 


```python
# get_read_set_export_job method usage example with argument unpacking

kwargs: GetReadSetExportJobRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
    "id": ...,
}

parent.get_read_set_export_job(**kwargs)
```

1. See [:material-code-braces: GetReadSetExportJobRequestRequestTypeDef](./type_defs.md#getreadsetexportjobrequestrequesttypedef) 

### get\_read\_set\_import\_job

Gets information about a read set import job.

Type annotations and code completion for `#!python session.create_client("omics").get_read_set_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_read_set_import_job)

```python
# get_read_set_import_job method definition

await def get_read_set_import_job(
    self,
    *,
    id: str,
    sequenceStoreId: str,
) -> GetReadSetImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReadSetImportJobResponseTypeDef](./type_defs.md#getreadsetimportjobresponsetypedef) 


```python
# get_read_set_import_job method usage example with argument unpacking

kwargs: GetReadSetImportJobRequestRequestTypeDef = {  # (1)
    "id": ...,
    "sequenceStoreId": ...,
}

parent.get_read_set_import_job(**kwargs)
```

1. See [:material-code-braces: GetReadSetImportJobRequestRequestTypeDef](./type_defs.md#getreadsetimportjobrequestrequesttypedef) 

### get\_read\_set\_metadata

Gets details about a read set.

Type annotations and code completion for `#!python session.create_client("omics").get_read_set_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_read_set_metadata)

```python
# get_read_set_metadata method definition

await def get_read_set_metadata(
    self,
    *,
    id: str,
    sequenceStoreId: str,
) -> GetReadSetMetadataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReadSetMetadataResponseTypeDef](./type_defs.md#getreadsetmetadataresponsetypedef) 


```python
# get_read_set_metadata method usage example with argument unpacking

kwargs: GetReadSetMetadataRequestRequestTypeDef = {  # (1)
    "id": ...,
    "sequenceStoreId": ...,
}

parent.get_read_set_metadata(**kwargs)
```

1. See [:material-code-braces: GetReadSetMetadataRequestRequestTypeDef](./type_defs.md#getreadsetmetadatarequestrequesttypedef) 

### get\_reference

Gets a reference file.

Type annotations and code completion for `#!python session.create_client("omics").get_reference` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_reference)

```python
# get_reference method definition

await def get_reference(
    self,
    *,
    id: str,
    referenceStoreId: str,
    partNumber: int,
    range: str = ...,
    file: ReferenceFileType = ...,  # (1)
) -> GetReferenceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ReferenceFileType](./literals.md#referencefiletype) 
2. See [:material-code-braces: GetReferenceResponseTypeDef](./type_defs.md#getreferenceresponsetypedef) 


```python
# get_reference method usage example with argument unpacking

kwargs: GetReferenceRequestRequestTypeDef = {  # (1)
    "id": ...,
    "referenceStoreId": ...,
    "partNumber": ...,
}

parent.get_reference(**kwargs)
```

1. See [:material-code-braces: GetReferenceRequestRequestTypeDef](./type_defs.md#getreferencerequestrequesttypedef) 

### get\_reference\_import\_job

Gets information about a reference import job.

Type annotations and code completion for `#!python session.create_client("omics").get_reference_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_reference_import_job)

```python
# get_reference_import_job method definition

await def get_reference_import_job(
    self,
    *,
    id: str,
    referenceStoreId: str,
) -> GetReferenceImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReferenceImportJobResponseTypeDef](./type_defs.md#getreferenceimportjobresponsetypedef) 


```python
# get_reference_import_job method usage example with argument unpacking

kwargs: GetReferenceImportJobRequestRequestTypeDef = {  # (1)
    "id": ...,
    "referenceStoreId": ...,
}

parent.get_reference_import_job(**kwargs)
```

1. See [:material-code-braces: GetReferenceImportJobRequestRequestTypeDef](./type_defs.md#getreferenceimportjobrequestrequesttypedef) 

### get\_reference\_metadata

Gets information about a genome reference's metadata.

Type annotations and code completion for `#!python session.create_client("omics").get_reference_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_reference_metadata)

```python
# get_reference_metadata method definition

await def get_reference_metadata(
    self,
    *,
    id: str,
    referenceStoreId: str,
) -> GetReferenceMetadataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReferenceMetadataResponseTypeDef](./type_defs.md#getreferencemetadataresponsetypedef) 


```python
# get_reference_metadata method usage example with argument unpacking

kwargs: GetReferenceMetadataRequestRequestTypeDef = {  # (1)
    "id": ...,
    "referenceStoreId": ...,
}

parent.get_reference_metadata(**kwargs)
```

1. See [:material-code-braces: GetReferenceMetadataRequestRequestTypeDef](./type_defs.md#getreferencemetadatarequestrequesttypedef) 

### get\_reference\_store

Gets information about a reference store.

Type annotations and code completion for `#!python session.create_client("omics").get_reference_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_reference_store)

```python
# get_reference_store method definition

await def get_reference_store(
    self,
    *,
    id: str,
) -> GetReferenceStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReferenceStoreResponseTypeDef](./type_defs.md#getreferencestoreresponsetypedef) 


```python
# get_reference_store method usage example with argument unpacking

kwargs: GetReferenceStoreRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_reference_store(**kwargs)
```

1. See [:material-code-braces: GetReferenceStoreRequestRequestTypeDef](./type_defs.md#getreferencestorerequestrequesttypedef) 

### get\_run

Gets information about a workflow run.

Type annotations and code completion for `#!python session.create_client("omics").get_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_run)

```python
# get_run method definition

await def get_run(
    self,
    *,
    id: str,
    export: Sequence[RunExportType] = ...,  # (1)
) -> GetRunResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RunExportType](./literals.md#runexporttype) 
2. See [:material-code-braces: GetRunResponseTypeDef](./type_defs.md#getrunresponsetypedef) 


```python
# get_run method usage example with argument unpacking

kwargs: GetRunRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_run(**kwargs)
```

1. See [:material-code-braces: GetRunRequestRequestTypeDef](./type_defs.md#getrunrequestrequesttypedef) 

### get\_run\_group

Gets information about a workflow run group.

Type annotations and code completion for `#!python session.create_client("omics").get_run_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_run_group)

```python
# get_run_group method definition

await def get_run_group(
    self,
    *,
    id: str,
) -> GetRunGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRunGroupResponseTypeDef](./type_defs.md#getrungroupresponsetypedef) 


```python
# get_run_group method usage example with argument unpacking

kwargs: GetRunGroupRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_run_group(**kwargs)
```

1. See [:material-code-braces: GetRunGroupRequestRequestTypeDef](./type_defs.md#getrungrouprequestrequesttypedef) 

### get\_run\_task

Gets information about a workflow run task.

Type annotations and code completion for `#!python session.create_client("omics").get_run_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_run_task)

```python
# get_run_task method definition

await def get_run_task(
    self,
    *,
    id: str,
    taskId: str,
) -> GetRunTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRunTaskResponseTypeDef](./type_defs.md#getruntaskresponsetypedef) 


```python
# get_run_task method usage example with argument unpacking

kwargs: GetRunTaskRequestRequestTypeDef = {  # (1)
    "id": ...,
    "taskId": ...,
}

parent.get_run_task(**kwargs)
```

1. See [:material-code-braces: GetRunTaskRequestRequestTypeDef](./type_defs.md#getruntaskrequestrequesttypedef) 

### get\_sequence\_store

Gets information about a sequence store.

Type annotations and code completion for `#!python session.create_client("omics").get_sequence_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_sequence_store)

```python
# get_sequence_store method definition

await def get_sequence_store(
    self,
    *,
    id: str,
) -> GetSequenceStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSequenceStoreResponseTypeDef](./type_defs.md#getsequencestoreresponsetypedef) 


```python
# get_sequence_store method usage example with argument unpacking

kwargs: GetSequenceStoreRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_sequence_store(**kwargs)
```

1. See [:material-code-braces: GetSequenceStoreRequestRequestTypeDef](./type_defs.md#getsequencestorerequestrequesttypedef) 

### get\_share

Retrieves the metadata for the specified resource share.

Type annotations and code completion for `#!python session.create_client("omics").get_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_share)

```python
# get_share method definition

await def get_share(
    self,
    *,
    shareId: str,
) -> GetShareResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetShareResponseTypeDef](./type_defs.md#getshareresponsetypedef) 


```python
# get_share method usage example with argument unpacking

kwargs: GetShareRequestRequestTypeDef = {  # (1)
    "shareId": ...,
}

parent.get_share(**kwargs)
```

1. See [:material-code-braces: GetShareRequestRequestTypeDef](./type_defs.md#getsharerequestrequesttypedef) 

### get\_variant\_import\_job

Gets information about a variant import job.

Type annotations and code completion for `#!python session.create_client("omics").get_variant_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_variant_import_job)

```python
# get_variant_import_job method definition

await def get_variant_import_job(
    self,
    *,
    jobId: str,
) -> GetVariantImportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVariantImportResponseTypeDef](./type_defs.md#getvariantimportresponsetypedef) 


```python
# get_variant_import_job method usage example with argument unpacking

kwargs: GetVariantImportRequestRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.get_variant_import_job(**kwargs)
```

1. See [:material-code-braces: GetVariantImportRequestRequestTypeDef](./type_defs.md#getvariantimportrequestrequesttypedef) 

### get\_variant\_store

Gets information about a variant store.

Type annotations and code completion for `#!python session.create_client("omics").get_variant_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_variant_store)

```python
# get_variant_store method definition

await def get_variant_store(
    self,
    *,
    name: str,
) -> GetVariantStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVariantStoreResponseTypeDef](./type_defs.md#getvariantstoreresponsetypedef) 


```python
# get_variant_store method usage example with argument unpacking

kwargs: GetVariantStoreRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.get_variant_store(**kwargs)
```

1. See [:material-code-braces: GetVariantStoreRequestRequestTypeDef](./type_defs.md#getvariantstorerequestrequesttypedef) 

### get\_workflow

Gets information about a workflow.

Type annotations and code completion for `#!python session.create_client("omics").get_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_workflow)

```python
# get_workflow method definition

await def get_workflow(
    self,
    *,
    id: str,
    type: WorkflowTypeType = ...,  # (1)
    export: Sequence[WorkflowExportType] = ...,  # (2)
    workflowOwnerId: str = ...,
) -> GetWorkflowResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-brackets: WorkflowExportType](./literals.md#workflowexporttype) 
3. See [:material-code-braces: GetWorkflowResponseTypeDef](./type_defs.md#getworkflowresponsetypedef) 


```python
# get_workflow method usage example with argument unpacking

kwargs: GetWorkflowRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_workflow(**kwargs)
```

1. See [:material-code-braces: GetWorkflowRequestRequestTypeDef](./type_defs.md#getworkflowrequestrequesttypedef) 

### list\_annotation\_import\_jobs

Retrieves a list of annotation import jobs.

Type annotations and code completion for `#!python session.create_client("omics").list_annotation_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_annotation_import_jobs)

```python
# list_annotation_import_jobs method definition

await def list_annotation_import_jobs(
    self,
    *,
    maxResults: int = ...,
    ids: Sequence[str] = ...,
    nextToken: str = ...,
    filter: ListAnnotationImportJobsFilterTypeDef = ...,  # (1)
) -> ListAnnotationImportJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListAnnotationImportJobsFilterTypeDef](./type_defs.md#listannotationimportjobsfiltertypedef) 
2. See [:material-code-braces: ListAnnotationImportJobsResponseTypeDef](./type_defs.md#listannotationimportjobsresponsetypedef) 


```python
# list_annotation_import_jobs method usage example with argument unpacking

kwargs: ListAnnotationImportJobsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_annotation_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListAnnotationImportJobsRequestRequestTypeDef](./type_defs.md#listannotationimportjobsrequestrequesttypedef) 

### list\_annotation\_store\_versions

Lists the versions of an annotation store.

Type annotations and code completion for `#!python session.create_client("omics").list_annotation_store_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_annotation_store_versions)

```python
# list_annotation_store_versions method definition

await def list_annotation_store_versions(
    self,
    *,
    name: str,
    maxResults: int = ...,
    nextToken: str = ...,
    filter: ListAnnotationStoreVersionsFilterTypeDef = ...,  # (1)
) -> ListAnnotationStoreVersionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListAnnotationStoreVersionsFilterTypeDef](./type_defs.md#listannotationstoreversionsfiltertypedef) 
2. See [:material-code-braces: ListAnnotationStoreVersionsResponseTypeDef](./type_defs.md#listannotationstoreversionsresponsetypedef) 


```python
# list_annotation_store_versions method usage example with argument unpacking

kwargs: ListAnnotationStoreVersionsRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.list_annotation_store_versions(**kwargs)
```

1. See [:material-code-braces: ListAnnotationStoreVersionsRequestRequestTypeDef](./type_defs.md#listannotationstoreversionsrequestrequesttypedef) 

### list\_annotation\_stores

Retrieves a list of annotation stores.

Type annotations and code completion for `#!python session.create_client("omics").list_annotation_stores` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_annotation_stores)

```python
# list_annotation_stores method definition

await def list_annotation_stores(
    self,
    *,
    ids: Sequence[str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    filter: ListAnnotationStoresFilterTypeDef = ...,  # (1)
) -> ListAnnotationStoresResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListAnnotationStoresFilterTypeDef](./type_defs.md#listannotationstoresfiltertypedef) 
2. See [:material-code-braces: ListAnnotationStoresResponseTypeDef](./type_defs.md#listannotationstoresresponsetypedef) 


```python
# list_annotation_stores method usage example with argument unpacking

kwargs: ListAnnotationStoresRequestRequestTypeDef = {  # (1)
    "ids": ...,
}

parent.list_annotation_stores(**kwargs)
```

1. See [:material-code-braces: ListAnnotationStoresRequestRequestTypeDef](./type_defs.md#listannotationstoresrequestrequesttypedef) 

### list\_multipart\_read\_set\_uploads

Lists multipart read set uploads and for in progress uploads.

Type annotations and code completion for `#!python session.create_client("omics").list_multipart_read_set_uploads` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_multipart_read_set_uploads)

```python
# list_multipart_read_set_uploads method definition

await def list_multipart_read_set_uploads(
    self,
    *,
    sequenceStoreId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMultipartReadSetUploadsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMultipartReadSetUploadsResponseTypeDef](./type_defs.md#listmultipartreadsetuploadsresponsetypedef) 


```python
# list_multipart_read_set_uploads method usage example with argument unpacking

kwargs: ListMultipartReadSetUploadsRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
}

parent.list_multipart_read_set_uploads(**kwargs)
```

1. See [:material-code-braces: ListMultipartReadSetUploadsRequestRequestTypeDef](./type_defs.md#listmultipartreadsetuploadsrequestrequesttypedef) 

### list\_read\_set\_activation\_jobs

Retrieves a list of read set activation jobs.

Type annotations and code completion for `#!python session.create_client("omics").list_read_set_activation_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_set_activation_jobs)

```python
# list_read_set_activation_jobs method definition

await def list_read_set_activation_jobs(
    self,
    *,
    sequenceStoreId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    filter: ActivateReadSetFilterTypeDef = ...,  # (1)
) -> ListReadSetActivationJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ActivateReadSetFilterTypeDef](./type_defs.md#activatereadsetfiltertypedef) 
2. See [:material-code-braces: ListReadSetActivationJobsResponseTypeDef](./type_defs.md#listreadsetactivationjobsresponsetypedef) 


```python
# list_read_set_activation_jobs method usage example with argument unpacking

kwargs: ListReadSetActivationJobsRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
}

parent.list_read_set_activation_jobs(**kwargs)
```

1. See [:material-code-braces: ListReadSetActivationJobsRequestRequestTypeDef](./type_defs.md#listreadsetactivationjobsrequestrequesttypedef) 

### list\_read\_set\_export\_jobs

Retrieves a list of read set export jobs.

Type annotations and code completion for `#!python session.create_client("omics").list_read_set_export_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_set_export_jobs)

```python
# list_read_set_export_jobs method definition

await def list_read_set_export_jobs(
    self,
    *,
    sequenceStoreId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    filter: ExportReadSetFilterTypeDef = ...,  # (1)
) -> ListReadSetExportJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ExportReadSetFilterTypeDef](./type_defs.md#exportreadsetfiltertypedef) 
2. See [:material-code-braces: ListReadSetExportJobsResponseTypeDef](./type_defs.md#listreadsetexportjobsresponsetypedef) 


```python
# list_read_set_export_jobs method usage example with argument unpacking

kwargs: ListReadSetExportJobsRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
}

parent.list_read_set_export_jobs(**kwargs)
```

1. See [:material-code-braces: ListReadSetExportJobsRequestRequestTypeDef](./type_defs.md#listreadsetexportjobsrequestrequesttypedef) 

### list\_read\_set\_import\_jobs

Retrieves a list of read set import jobs.

Type annotations and code completion for `#!python session.create_client("omics").list_read_set_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_set_import_jobs)

```python
# list_read_set_import_jobs method definition

await def list_read_set_import_jobs(
    self,
    *,
    sequenceStoreId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    filter: ImportReadSetFilterTypeDef = ...,  # (1)
) -> ListReadSetImportJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ImportReadSetFilterTypeDef](./type_defs.md#importreadsetfiltertypedef) 
2. See [:material-code-braces: ListReadSetImportJobsResponseTypeDef](./type_defs.md#listreadsetimportjobsresponsetypedef) 


```python
# list_read_set_import_jobs method usage example with argument unpacking

kwargs: ListReadSetImportJobsRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
}

parent.list_read_set_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListReadSetImportJobsRequestRequestTypeDef](./type_defs.md#listreadsetimportjobsrequestrequesttypedef) 

### list\_read\_set\_upload\_parts

This operation will list all parts in a requested multipart upload for a
sequence
store.

Type annotations and code completion for `#!python session.create_client("omics").list_read_set_upload_parts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_set_upload_parts)

```python
# list_read_set_upload_parts method definition

await def list_read_set_upload_parts(
    self,
    *,
    sequenceStoreId: str,
    uploadId: str,
    partSource: ReadSetPartSourceType,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    filter: ReadSetUploadPartListFilterTypeDef = ...,  # (2)
) -> ListReadSetUploadPartsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ReadSetPartSourceType](./literals.md#readsetpartsourcetype) 
2. See [:material-code-braces: ReadSetUploadPartListFilterTypeDef](./type_defs.md#readsetuploadpartlistfiltertypedef) 
3. See [:material-code-braces: ListReadSetUploadPartsResponseTypeDef](./type_defs.md#listreadsetuploadpartsresponsetypedef) 


```python
# list_read_set_upload_parts method usage example with argument unpacking

kwargs: ListReadSetUploadPartsRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
    "uploadId": ...,
    "partSource": ...,
}

parent.list_read_set_upload_parts(**kwargs)
```

1. See [:material-code-braces: ListReadSetUploadPartsRequestRequestTypeDef](./type_defs.md#listreadsetuploadpartsrequestrequesttypedef) 

### list\_read\_sets

Retrieves a list of read sets.

Type annotations and code completion for `#!python session.create_client("omics").list_read_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_sets)

```python
# list_read_sets method definition

await def list_read_sets(
    self,
    *,
    sequenceStoreId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    filter: ReadSetFilterTypeDef = ...,  # (1)
) -> ListReadSetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ReadSetFilterTypeDef](./type_defs.md#readsetfiltertypedef) 
2. See [:material-code-braces: ListReadSetsResponseTypeDef](./type_defs.md#listreadsetsresponsetypedef) 


```python
# list_read_sets method usage example with argument unpacking

kwargs: ListReadSetsRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
}

parent.list_read_sets(**kwargs)
```

1. See [:material-code-braces: ListReadSetsRequestRequestTypeDef](./type_defs.md#listreadsetsrequestrequesttypedef) 

### list\_reference\_import\_jobs

Retrieves a list of reference import jobs.

Type annotations and code completion for `#!python session.create_client("omics").list_reference_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_reference_import_jobs)

```python
# list_reference_import_jobs method definition

await def list_reference_import_jobs(
    self,
    *,
    referenceStoreId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    filter: ImportReferenceFilterTypeDef = ...,  # (1)
) -> ListReferenceImportJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ImportReferenceFilterTypeDef](./type_defs.md#importreferencefiltertypedef) 
2. See [:material-code-braces: ListReferenceImportJobsResponseTypeDef](./type_defs.md#listreferenceimportjobsresponsetypedef) 


```python
# list_reference_import_jobs method usage example with argument unpacking

kwargs: ListReferenceImportJobsRequestRequestTypeDef = {  # (1)
    "referenceStoreId": ...,
}

parent.list_reference_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListReferenceImportJobsRequestRequestTypeDef](./type_defs.md#listreferenceimportjobsrequestrequesttypedef) 

### list\_reference\_stores

Retrieves a list of reference stores.

Type annotations and code completion for `#!python session.create_client("omics").list_reference_stores` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_reference_stores)

```python
# list_reference_stores method definition

await def list_reference_stores(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    filter: ReferenceStoreFilterTypeDef = ...,  # (1)
) -> ListReferenceStoresResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ReferenceStoreFilterTypeDef](./type_defs.md#referencestorefiltertypedef) 
2. See [:material-code-braces: ListReferenceStoresResponseTypeDef](./type_defs.md#listreferencestoresresponsetypedef) 


```python
# list_reference_stores method usage example with argument unpacking

kwargs: ListReferenceStoresRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_reference_stores(**kwargs)
```

1. See [:material-code-braces: ListReferenceStoresRequestRequestTypeDef](./type_defs.md#listreferencestoresrequestrequesttypedef) 

### list\_references

Retrieves a list of references.

Type annotations and code completion for `#!python session.create_client("omics").list_references` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_references)

```python
# list_references method definition

await def list_references(
    self,
    *,
    referenceStoreId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    filter: ReferenceFilterTypeDef = ...,  # (1)
) -> ListReferencesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ReferenceFilterTypeDef](./type_defs.md#referencefiltertypedef) 
2. See [:material-code-braces: ListReferencesResponseTypeDef](./type_defs.md#listreferencesresponsetypedef) 


```python
# list_references method usage example with argument unpacking

kwargs: ListReferencesRequestRequestTypeDef = {  # (1)
    "referenceStoreId": ...,
}

parent.list_references(**kwargs)
```

1. See [:material-code-braces: ListReferencesRequestRequestTypeDef](./type_defs.md#listreferencesrequestrequesttypedef) 

### list\_run\_groups

Retrieves a list of run groups.

Type annotations and code completion for `#!python session.create_client("omics").list_run_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_run_groups)

```python
# list_run_groups method definition

await def list_run_groups(
    self,
    *,
    name: str = ...,
    startingToken: str = ...,
    maxResults: int = ...,
) -> ListRunGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRunGroupsResponseTypeDef](./type_defs.md#listrungroupsresponsetypedef) 


```python
# list_run_groups method usage example with argument unpacking

kwargs: ListRunGroupsRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.list_run_groups(**kwargs)
```

1. See [:material-code-braces: ListRunGroupsRequestRequestTypeDef](./type_defs.md#listrungroupsrequestrequesttypedef) 

### list\_run\_tasks

Retrieves a list of tasks for a run.

Type annotations and code completion for `#!python session.create_client("omics").list_run_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_run_tasks)

```python
# list_run_tasks method definition

await def list_run_tasks(
    self,
    *,
    id: str,
    status: TaskStatusType = ...,  # (1)
    startingToken: str = ...,
    maxResults: int = ...,
) -> ListRunTasksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
2. See [:material-code-braces: ListRunTasksResponseTypeDef](./type_defs.md#listruntasksresponsetypedef) 


```python
# list_run_tasks method usage example with argument unpacking

kwargs: ListRunTasksRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.list_run_tasks(**kwargs)
```

1. See [:material-code-braces: ListRunTasksRequestRequestTypeDef](./type_defs.md#listruntasksrequestrequesttypedef) 

### list\_runs

Retrieves a list of runs.

Type annotations and code completion for `#!python session.create_client("omics").list_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_runs)

```python
# list_runs method definition

await def list_runs(
    self,
    *,
    name: str = ...,
    runGroupId: str = ...,
    startingToken: str = ...,
    maxResults: int = ...,
    status: RunStatusType = ...,  # (1)
) -> ListRunsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RunStatusType](./literals.md#runstatustype) 
2. See [:material-code-braces: ListRunsResponseTypeDef](./type_defs.md#listrunsresponsetypedef) 


```python
# list_runs method usage example with argument unpacking

kwargs: ListRunsRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.list_runs(**kwargs)
```

1. See [:material-code-braces: ListRunsRequestRequestTypeDef](./type_defs.md#listrunsrequestrequesttypedef) 

### list\_sequence\_stores

Retrieves a list of sequence stores.

Type annotations and code completion for `#!python session.create_client("omics").list_sequence_stores` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_sequence_stores)

```python
# list_sequence_stores method definition

await def list_sequence_stores(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    filter: SequenceStoreFilterTypeDef = ...,  # (1)
) -> ListSequenceStoresResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SequenceStoreFilterTypeDef](./type_defs.md#sequencestorefiltertypedef) 
2. See [:material-code-braces: ListSequenceStoresResponseTypeDef](./type_defs.md#listsequencestoresresponsetypedef) 


```python
# list_sequence_stores method usage example with argument unpacking

kwargs: ListSequenceStoresRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_sequence_stores(**kwargs)
```

1. See [:material-code-braces: ListSequenceStoresRequestRequestTypeDef](./type_defs.md#listsequencestoresrequestrequesttypedef) 

### list\_shares

Retrieves the resource shares associated with an account.

Type annotations and code completion for `#!python session.create_client("omics").list_shares` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_shares)

```python
# list_shares method definition

await def list_shares(
    self,
    *,
    resourceOwner: ResourceOwnerType,  # (1)
    filter: FilterTypeDef = ...,  # (2)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListSharesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: ListSharesResponseTypeDef](./type_defs.md#listsharesresponsetypedef) 


```python
# list_shares method usage example with argument unpacking

kwargs: ListSharesRequestRequestTypeDef = {  # (1)
    "resourceOwner": ...,
}

parent.list_shares(**kwargs)
```

1. See [:material-code-braces: ListSharesRequestRequestTypeDef](./type_defs.md#listsharesrequestrequesttypedef) 

### list\_tags\_for\_resource

Retrieves a list of tags for a resource.

Type annotations and code completion for `#!python session.create_client("omics").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_variant\_import\_jobs

Retrieves a list of variant import jobs.

Type annotations and code completion for `#!python session.create_client("omics").list_variant_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_variant_import_jobs)

```python
# list_variant_import_jobs method definition

await def list_variant_import_jobs(
    self,
    *,
    maxResults: int = ...,
    ids: Sequence[str] = ...,
    nextToken: str = ...,
    filter: ListVariantImportJobsFilterTypeDef = ...,  # (1)
) -> ListVariantImportJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListVariantImportJobsFilterTypeDef](./type_defs.md#listvariantimportjobsfiltertypedef) 
2. See [:material-code-braces: ListVariantImportJobsResponseTypeDef](./type_defs.md#listvariantimportjobsresponsetypedef) 


```python
# list_variant_import_jobs method usage example with argument unpacking

kwargs: ListVariantImportJobsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_variant_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListVariantImportJobsRequestRequestTypeDef](./type_defs.md#listvariantimportjobsrequestrequesttypedef) 

### list\_variant\_stores

Retrieves a list of variant stores.

Type annotations and code completion for `#!python session.create_client("omics").list_variant_stores` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_variant_stores)

```python
# list_variant_stores method definition

await def list_variant_stores(
    self,
    *,
    maxResults: int = ...,
    ids: Sequence[str] = ...,
    nextToken: str = ...,
    filter: ListVariantStoresFilterTypeDef = ...,  # (1)
) -> ListVariantStoresResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListVariantStoresFilterTypeDef](./type_defs.md#listvariantstoresfiltertypedef) 
2. See [:material-code-braces: ListVariantStoresResponseTypeDef](./type_defs.md#listvariantstoresresponsetypedef) 


```python
# list_variant_stores method usage example with argument unpacking

kwargs: ListVariantStoresRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_variant_stores(**kwargs)
```

1. See [:material-code-braces: ListVariantStoresRequestRequestTypeDef](./type_defs.md#listvariantstoresrequestrequesttypedef) 

### list\_workflows

Retrieves a list of workflows.

Type annotations and code completion for `#!python session.create_client("omics").list_workflows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_workflows)

```python
# list_workflows method definition

await def list_workflows(
    self,
    *,
    type: WorkflowTypeType = ...,  # (1)
    name: str = ...,
    startingToken: str = ...,
    maxResults: int = ...,
) -> ListWorkflowsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-braces: ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef) 


```python
# list_workflows method usage example with argument unpacking

kwargs: ListWorkflowsRequestRequestTypeDef = {  # (1)
    "type": ...,
}

parent.list_workflows(**kwargs)
```

1. See [:material-code-braces: ListWorkflowsRequestRequestTypeDef](./type_defs.md#listworkflowsrequestrequesttypedef) 

### start\_annotation\_import\_job

Starts an annotation import job.

Type annotations and code completion for `#!python session.create_client("omics").start_annotation_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_annotation_import_job)

```python
# start_annotation_import_job method definition

await def start_annotation_import_job(
    self,
    *,
    destinationName: str,
    roleArn: str,
    items: Sequence[AnnotationImportItemSourceTypeDef],  # (1)
    versionName: str = ...,
    formatOptions: FormatOptionsTypeDef = ...,  # (2)
    runLeftNormalization: bool = ...,
    annotationFields: Mapping[str, str] = ...,
) -> StartAnnotationImportResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AnnotationImportItemSourceTypeDef](./type_defs.md#annotationimportitemsourcetypedef) 
2. See [:material-code-braces: FormatOptionsTypeDef](./type_defs.md#formatoptionstypedef) 
3. See [:material-code-braces: StartAnnotationImportResponseTypeDef](./type_defs.md#startannotationimportresponsetypedef) 


```python
# start_annotation_import_job method usage example with argument unpacking

kwargs: StartAnnotationImportRequestRequestTypeDef = {  # (1)
    "destinationName": ...,
    "roleArn": ...,
    "items": ...,
}

parent.start_annotation_import_job(**kwargs)
```

1. See [:material-code-braces: StartAnnotationImportRequestRequestTypeDef](./type_defs.md#startannotationimportrequestrequesttypedef) 

### start\_read\_set\_activation\_job

Activates an archived read set.

Type annotations and code completion for `#!python session.create_client("omics").start_read_set_activation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_read_set_activation_job)

```python
# start_read_set_activation_job method definition

await def start_read_set_activation_job(
    self,
    *,
    sequenceStoreId: str,
    sources: Sequence[StartReadSetActivationJobSourceItemTypeDef],  # (1)
    clientToken: str = ...,
) -> StartReadSetActivationJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StartReadSetActivationJobSourceItemTypeDef](./type_defs.md#startreadsetactivationjobsourceitemtypedef) 
2. See [:material-code-braces: StartReadSetActivationJobResponseTypeDef](./type_defs.md#startreadsetactivationjobresponsetypedef) 


```python
# start_read_set_activation_job method usage example with argument unpacking

kwargs: StartReadSetActivationJobRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
    "sources": ...,
}

parent.start_read_set_activation_job(**kwargs)
```

1. See [:material-code-braces: StartReadSetActivationJobRequestRequestTypeDef](./type_defs.md#startreadsetactivationjobrequestrequesttypedef) 

### start\_read\_set\_export\_job

Exports a read set to Amazon S3.

Type annotations and code completion for `#!python session.create_client("omics").start_read_set_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_read_set_export_job)

```python
# start_read_set_export_job method definition

await def start_read_set_export_job(
    self,
    *,
    sequenceStoreId: str,
    destination: str,
    roleArn: str,
    sources: Sequence[ExportReadSetTypeDef],  # (1)
    clientToken: str = ...,
) -> StartReadSetExportJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ExportReadSetTypeDef](./type_defs.md#exportreadsettypedef) 
2. See [:material-code-braces: StartReadSetExportJobResponseTypeDef](./type_defs.md#startreadsetexportjobresponsetypedef) 


```python
# start_read_set_export_job method usage example with argument unpacking

kwargs: StartReadSetExportJobRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
    "destination": ...,
    "roleArn": ...,
    "sources": ...,
}

parent.start_read_set_export_job(**kwargs)
```

1. See [:material-code-braces: StartReadSetExportJobRequestRequestTypeDef](./type_defs.md#startreadsetexportjobrequestrequesttypedef) 

### start\_read\_set\_import\_job

Starts a read set import job.

Type annotations and code completion for `#!python session.create_client("omics").start_read_set_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_read_set_import_job)

```python
# start_read_set_import_job method definition

await def start_read_set_import_job(
    self,
    *,
    sequenceStoreId: str,
    roleArn: str,
    sources: Sequence[StartReadSetImportJobSourceItemTypeDef],  # (1)
    clientToken: str = ...,
) -> StartReadSetImportJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StartReadSetImportJobSourceItemTypeDef](./type_defs.md#startreadsetimportjobsourceitemtypedef) 
2. See [:material-code-braces: StartReadSetImportJobResponseTypeDef](./type_defs.md#startreadsetimportjobresponsetypedef) 


```python
# start_read_set_import_job method usage example with argument unpacking

kwargs: StartReadSetImportJobRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
    "roleArn": ...,
    "sources": ...,
}

parent.start_read_set_import_job(**kwargs)
```

1. See [:material-code-braces: StartReadSetImportJobRequestRequestTypeDef](./type_defs.md#startreadsetimportjobrequestrequesttypedef) 

### start\_reference\_import\_job

Starts a reference import job.

Type annotations and code completion for `#!python session.create_client("omics").start_reference_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_reference_import_job)

```python
# start_reference_import_job method definition

await def start_reference_import_job(
    self,
    *,
    referenceStoreId: str,
    roleArn: str,
    sources: Sequence[StartReferenceImportJobSourceItemTypeDef],  # (1)
    clientToken: str = ...,
) -> StartReferenceImportJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StartReferenceImportJobSourceItemTypeDef](./type_defs.md#startreferenceimportjobsourceitemtypedef) 
2. See [:material-code-braces: StartReferenceImportJobResponseTypeDef](./type_defs.md#startreferenceimportjobresponsetypedef) 


```python
# start_reference_import_job method usage example with argument unpacking

kwargs: StartReferenceImportJobRequestRequestTypeDef = {  # (1)
    "referenceStoreId": ...,
    "roleArn": ...,
    "sources": ...,
}

parent.start_reference_import_job(**kwargs)
```

1. See [:material-code-braces: StartReferenceImportJobRequestRequestTypeDef](./type_defs.md#startreferenceimportjobrequestrequesttypedef) 

### start\_run

Starts a workflow run.

Type annotations and code completion for `#!python session.create_client("omics").start_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_run)

```python
# start_run method definition

await def start_run(
    self,
    *,
    roleArn: str,
    requestId: str,
    workflowId: str = ...,
    workflowType: WorkflowTypeType = ...,  # (1)
    runId: str = ...,
    name: str = ...,
    runGroupId: str = ...,
    priority: int = ...,
    parameters: Mapping[str, Any] = ...,
    storageCapacity: int = ...,
    outputUri: str = ...,
    logLevel: RunLogLevelType = ...,  # (2)
    tags: Mapping[str, str] = ...,
    retentionMode: RunRetentionModeType = ...,  # (3)
    storageType: StorageTypeType = ...,  # (4)
    workflowOwnerId: str = ...,
) -> StartRunResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-brackets: RunLogLevelType](./literals.md#runlogleveltype) 
3. See [:material-code-brackets: RunRetentionModeType](./literals.md#runretentionmodetype) 
4. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
5. See [:material-code-braces: StartRunResponseTypeDef](./type_defs.md#startrunresponsetypedef) 


```python
# start_run method usage example with argument unpacking

kwargs: StartRunRequestRequestTypeDef = {  # (1)
    "roleArn": ...,
    "requestId": ...,
}

parent.start_run(**kwargs)
```

1. See [:material-code-braces: StartRunRequestRequestTypeDef](./type_defs.md#startrunrequestrequesttypedef) 

### start\_variant\_import\_job

Starts a variant import job.

Type annotations and code completion for `#!python session.create_client("omics").start_variant_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_variant_import_job)

```python
# start_variant_import_job method definition

await def start_variant_import_job(
    self,
    *,
    destinationName: str,
    roleArn: str,
    items: Sequence[VariantImportItemSourceTypeDef],  # (1)
    runLeftNormalization: bool = ...,
    annotationFields: Mapping[str, str] = ...,
) -> StartVariantImportResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VariantImportItemSourceTypeDef](./type_defs.md#variantimportitemsourcetypedef) 
2. See [:material-code-braces: StartVariantImportResponseTypeDef](./type_defs.md#startvariantimportresponsetypedef) 


```python
# start_variant_import_job method usage example with argument unpacking

kwargs: StartVariantImportRequestRequestTypeDef = {  # (1)
    "destinationName": ...,
    "roleArn": ...,
    "items": ...,
}

parent.start_variant_import_job(**kwargs)
```

1. See [:material-code-braces: StartVariantImportRequestRequestTypeDef](./type_defs.md#startvariantimportrequestrequesttypedef) 

### tag\_resource

Tags a resource.

Type annotations and code completion for `#!python session.create_client("omics").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from a resource.

Type annotations and code completion for `#!python session.create_client("omics").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_annotation\_store

Updates an annotation store.

Type annotations and code completion for `#!python session.create_client("omics").update_annotation_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.update_annotation_store)

```python
# update_annotation_store method definition

await def update_annotation_store(
    self,
    *,
    name: str,
    description: str = ...,
) -> UpdateAnnotationStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAnnotationStoreResponseTypeDef](./type_defs.md#updateannotationstoreresponsetypedef) 


```python
# update_annotation_store method usage example with argument unpacking

kwargs: UpdateAnnotationStoreRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.update_annotation_store(**kwargs)
```

1. See [:material-code-braces: UpdateAnnotationStoreRequestRequestTypeDef](./type_defs.md#updateannotationstorerequestrequesttypedef) 

### update\_annotation\_store\_version

Updates the description of an annotation store version.

Type annotations and code completion for `#!python session.create_client("omics").update_annotation_store_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.update_annotation_store_version)

```python
# update_annotation_store_version method definition

await def update_annotation_store_version(
    self,
    *,
    name: str,
    versionName: str,
    description: str = ...,
) -> UpdateAnnotationStoreVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAnnotationStoreVersionResponseTypeDef](./type_defs.md#updateannotationstoreversionresponsetypedef) 


```python
# update_annotation_store_version method usage example with argument unpacking

kwargs: UpdateAnnotationStoreVersionRequestRequestTypeDef = {  # (1)
    "name": ...,
    "versionName": ...,
}

parent.update_annotation_store_version(**kwargs)
```

1. See [:material-code-braces: UpdateAnnotationStoreVersionRequestRequestTypeDef](./type_defs.md#updateannotationstoreversionrequestrequesttypedef) 

### update\_run\_group

Updates a run group.

Type annotations and code completion for `#!python session.create_client("omics").update_run_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.update_run_group)

```python
# update_run_group method definition

await def update_run_group(
    self,
    *,
    id: str,
    name: str = ...,
    maxCpus: int = ...,
    maxRuns: int = ...,
    maxDuration: int = ...,
    maxGpus: int = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_run_group method usage example with argument unpacking

kwargs: UpdateRunGroupRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.update_run_group(**kwargs)
```

1. See [:material-code-braces: UpdateRunGroupRequestRequestTypeDef](./type_defs.md#updaterungrouprequestrequesttypedef) 

### update\_variant\_store

Updates a variant store.

Type annotations and code completion for `#!python session.create_client("omics").update_variant_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.update_variant_store)

```python
# update_variant_store method definition

await def update_variant_store(
    self,
    *,
    name: str,
    description: str = ...,
) -> UpdateVariantStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateVariantStoreResponseTypeDef](./type_defs.md#updatevariantstoreresponsetypedef) 


```python
# update_variant_store method usage example with argument unpacking

kwargs: UpdateVariantStoreRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.update_variant_store(**kwargs)
```

1. See [:material-code-braces: UpdateVariantStoreRequestRequestTypeDef](./type_defs.md#updatevariantstorerequestrequesttypedef) 

### update\_workflow

Updates a workflow.

Type annotations and code completion for `#!python session.create_client("omics").update_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.update_workflow)

```python
# update_workflow method definition

await def update_workflow(
    self,
    *,
    id: str,
    name: str = ...,
    description: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_workflow method usage example with argument unpacking

kwargs: UpdateWorkflowRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.update_workflow(**kwargs)
```

1. See [:material-code-braces: UpdateWorkflowRequestRequestTypeDef](./type_defs.md#updateworkflowrequestrequesttypedef) 

### upload\_read\_set\_part

This operation uploads a specific part of a read set.

Type annotations and code completion for `#!python session.create_client("omics").upload_read_set_part` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.upload_read_set_part)

```python
# upload_read_set_part method definition

await def upload_read_set_part(
    self,
    *,
    sequenceStoreId: str,
    uploadId: str,
    partSource: ReadSetPartSourceType,  # (1)
    partNumber: int,
    payload: BlobTypeDef,
) -> UploadReadSetPartResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ReadSetPartSourceType](./literals.md#readsetpartsourcetype) 
2. See [:material-code-braces: UploadReadSetPartResponseTypeDef](./type_defs.md#uploadreadsetpartresponsetypedef) 


```python
# upload_read_set_part method usage example with argument unpacking

kwargs: UploadReadSetPartRequestRequestTypeDef = {  # (1)
    "sequenceStoreId": ...,
    "uploadId": ...,
    "partSource": ...,
    "partNumber": ...,
    "payload": ...,
}

parent.upload_read_set_part(**kwargs)
```

1. See [:material-code-braces: UploadReadSetPartRequestRequestTypeDef](./type_defs.md#uploadreadsetpartrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("omics").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "OmicsClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("omics").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("omics").get_paginator` method with overloads.

- `client.get_paginator("list_annotation_import_jobs")` -> [ListAnnotationImportJobsPaginator](./paginators.md#listannotationimportjobspaginator)
- `client.get_paginator("list_annotation_store_versions")` -> [ListAnnotationStoreVersionsPaginator](./paginators.md#listannotationstoreversionspaginator)
- `client.get_paginator("list_annotation_stores")` -> [ListAnnotationStoresPaginator](./paginators.md#listannotationstorespaginator)
- `client.get_paginator("list_multipart_read_set_uploads")` -> [ListMultipartReadSetUploadsPaginator](./paginators.md#listmultipartreadsetuploadspaginator)
- `client.get_paginator("list_read_set_activation_jobs")` -> [ListReadSetActivationJobsPaginator](./paginators.md#listreadsetactivationjobspaginator)
- `client.get_paginator("list_read_set_export_jobs")` -> [ListReadSetExportJobsPaginator](./paginators.md#listreadsetexportjobspaginator)
- `client.get_paginator("list_read_set_import_jobs")` -> [ListReadSetImportJobsPaginator](./paginators.md#listreadsetimportjobspaginator)
- `client.get_paginator("list_read_set_upload_parts")` -> [ListReadSetUploadPartsPaginator](./paginators.md#listreadsetuploadpartspaginator)
- `client.get_paginator("list_read_sets")` -> [ListReadSetsPaginator](./paginators.md#listreadsetspaginator)
- `client.get_paginator("list_reference_import_jobs")` -> [ListReferenceImportJobsPaginator](./paginators.md#listreferenceimportjobspaginator)
- `client.get_paginator("list_reference_stores")` -> [ListReferenceStoresPaginator](./paginators.md#listreferencestorespaginator)
- `client.get_paginator("list_references")` -> [ListReferencesPaginator](./paginators.md#listreferencespaginator)
- `client.get_paginator("list_run_groups")` -> [ListRunGroupsPaginator](./paginators.md#listrungroupspaginator)
- `client.get_paginator("list_run_tasks")` -> [ListRunTasksPaginator](./paginators.md#listruntaskspaginator)
- `client.get_paginator("list_runs")` -> [ListRunsPaginator](./paginators.md#listrunspaginator)
- `client.get_paginator("list_sequence_stores")` -> [ListSequenceStoresPaginator](./paginators.md#listsequencestorespaginator)
- `client.get_paginator("list_shares")` -> [ListSharesPaginator](./paginators.md#listsharespaginator)
- `client.get_paginator("list_variant_import_jobs")` -> [ListVariantImportJobsPaginator](./paginators.md#listvariantimportjobspaginator)
- `client.get_paginator("list_variant_stores")` -> [ListVariantStoresPaginator](./paginators.md#listvariantstorespaginator)
- `client.get_paginator("list_workflows")` -> [ListWorkflowsPaginator](./paginators.md#listworkflowspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter` method with overloads.

- `client.get_waiter("annotation_import_job_created")` -> [AnnotationImportJobCreatedWaiter](./waiters.md#annotationimportjobcreatedwaiter)
- `client.get_waiter("annotation_store_created")` -> [AnnotationStoreCreatedWaiter](./waiters.md#annotationstorecreatedwaiter)
- `client.get_waiter("annotation_store_deleted")` -> [AnnotationStoreDeletedWaiter](./waiters.md#annotationstoredeletedwaiter)
- `client.get_waiter("annotation_store_version_created")` -> [AnnotationStoreVersionCreatedWaiter](./waiters.md#annotationstoreversioncreatedwaiter)
- `client.get_waiter("annotation_store_version_deleted")` -> [AnnotationStoreVersionDeletedWaiter](./waiters.md#annotationstoreversiondeletedwaiter)
- `client.get_waiter("read_set_activation_job_completed")` -> [ReadSetActivationJobCompletedWaiter](./waiters.md#readsetactivationjobcompletedwaiter)
- `client.get_waiter("read_set_export_job_completed")` -> [ReadSetExportJobCompletedWaiter](./waiters.md#readsetexportjobcompletedwaiter)
- `client.get_waiter("read_set_import_job_completed")` -> [ReadSetImportJobCompletedWaiter](./waiters.md#readsetimportjobcompletedwaiter)
- `client.get_waiter("reference_import_job_completed")` -> [ReferenceImportJobCompletedWaiter](./waiters.md#referenceimportjobcompletedwaiter)
- `client.get_waiter("run_completed")` -> [RunCompletedWaiter](./waiters.md#runcompletedwaiter)
- `client.get_waiter("run_running")` -> [RunRunningWaiter](./waiters.md#runrunningwaiter)
- `client.get_waiter("task_completed")` -> [TaskCompletedWaiter](./waiters.md#taskcompletedwaiter)
- `client.get_waiter("task_running")` -> [TaskRunningWaiter](./waiters.md#taskrunningwaiter)
- `client.get_waiter("variant_import_job_created")` -> [VariantImportJobCreatedWaiter](./waiters.md#variantimportjobcreatedwaiter)
- `client.get_waiter("variant_store_created")` -> [VariantStoreCreatedWaiter](./waiters.md#variantstorecreatedwaiter)
- `client.get_waiter("variant_store_deleted")` -> [VariantStoreDeletedWaiter](./waiters.md#variantstoredeletedwaiter)
- `client.get_waiter("workflow_active")` -> [WorkflowActiveWaiter](./waiters.md#workflowactivewaiter)

