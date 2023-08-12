# Waiters

> [Index](../README.md) > [Omics](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [Omics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
    type annotations stubs module [types-aiobotocore-omics](https://pypi.org/project/types-aiobotocore-omics/).

## AnnotationImportJobCreatedWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("annotation_import_job_created")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.AnnotationImportJobCreated)

```python
# AnnotationImportJobCreatedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import AnnotationImportJobCreatedWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: AnnotationImportJobCreatedWaiter = client.get_waiter("annotation_import_job_created")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [AnnotationImportJobCreatedWaiter](./waiters.md#annotationimportjobcreatedwaiter)


### wait

Type annotations and code completion for `#!python AnnotationImportJobCreatedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    jobId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef = {  # (1)
    "jobId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef](./type_defs.md#getannotationimportrequestannotationimportjobcreatedwaittypedef) 
## AnnotationStoreCreatedWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("annotation_store_created")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.AnnotationStoreCreated)

```python
# AnnotationStoreCreatedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import AnnotationStoreCreatedWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: AnnotationStoreCreatedWaiter = client.get_waiter("annotation_store_created")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [AnnotationStoreCreatedWaiter](./waiters.md#annotationstorecreatedwaiter)


### wait

Type annotations and code completion for `#!python AnnotationStoreCreatedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    name: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef = {  # (1)
    "name": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef](./type_defs.md#getannotationstorerequestannotationstorecreatedwaittypedef) 
## AnnotationStoreDeletedWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("annotation_store_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.AnnotationStoreDeleted)

```python
# AnnotationStoreDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import AnnotationStoreDeletedWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: AnnotationStoreDeletedWaiter = client.get_waiter("annotation_store_deleted")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [AnnotationStoreDeletedWaiter](./waiters.md#annotationstoredeletedwaiter)


### wait

Type annotations and code completion for `#!python AnnotationStoreDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    name: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef = {  # (1)
    "name": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef](./type_defs.md#getannotationstorerequestannotationstoredeletedwaittypedef) 
## ReadSetActivationJobCompletedWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("read_set_activation_job_completed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.ReadSetActivationJobCompleted)

```python
# ReadSetActivationJobCompletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import ReadSetActivationJobCompletedWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: ReadSetActivationJobCompletedWaiter = client.get_waiter("read_set_activation_job_completed")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [ReadSetActivationJobCompletedWaiter](./waiters.md#readsetactivationjobcompletedwaiter)


### wait

Type annotations and code completion for `#!python ReadSetActivationJobCompletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    id: str,
    sequenceStoreId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetReadSetActivationJobRequestReadSetActivationJobCompletedWaitTypeDef = {  # (1)
    "id": ...,
    "sequenceStoreId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetReadSetActivationJobRequestReadSetActivationJobCompletedWaitTypeDef](./type_defs.md#getreadsetactivationjobrequestreadsetactivationjobcompletedwaittypedef) 
## ReadSetExportJobCompletedWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("read_set_export_job_completed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.ReadSetExportJobCompleted)

```python
# ReadSetExportJobCompletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import ReadSetExportJobCompletedWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: ReadSetExportJobCompletedWaiter = client.get_waiter("read_set_export_job_completed")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [ReadSetExportJobCompletedWaiter](./waiters.md#readsetexportjobcompletedwaiter)


### wait

Type annotations and code completion for `#!python ReadSetExportJobCompletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    sequenceStoreId: str,
    id: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetReadSetExportJobRequestReadSetExportJobCompletedWaitTypeDef = {  # (1)
    "sequenceStoreId": ...,
    "id": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetReadSetExportJobRequestReadSetExportJobCompletedWaitTypeDef](./type_defs.md#getreadsetexportjobrequestreadsetexportjobcompletedwaittypedef) 
## ReadSetImportJobCompletedWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("read_set_import_job_completed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.ReadSetImportJobCompleted)

```python
# ReadSetImportJobCompletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import ReadSetImportJobCompletedWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: ReadSetImportJobCompletedWaiter = client.get_waiter("read_set_import_job_completed")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [ReadSetImportJobCompletedWaiter](./waiters.md#readsetimportjobcompletedwaiter)


### wait

Type annotations and code completion for `#!python ReadSetImportJobCompletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    id: str,
    sequenceStoreId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetReadSetImportJobRequestReadSetImportJobCompletedWaitTypeDef = {  # (1)
    "id": ...,
    "sequenceStoreId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetReadSetImportJobRequestReadSetImportJobCompletedWaitTypeDef](./type_defs.md#getreadsetimportjobrequestreadsetimportjobcompletedwaittypedef) 
## ReferenceImportJobCompletedWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("reference_import_job_completed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.ReferenceImportJobCompleted)

```python
# ReferenceImportJobCompletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import ReferenceImportJobCompletedWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: ReferenceImportJobCompletedWaiter = client.get_waiter("reference_import_job_completed")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [ReferenceImportJobCompletedWaiter](./waiters.md#referenceimportjobcompletedwaiter)


### wait

Type annotations and code completion for `#!python ReferenceImportJobCompletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    id: str,
    referenceStoreId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetReferenceImportJobRequestReferenceImportJobCompletedWaitTypeDef = {  # (1)
    "id": ...,
    "referenceStoreId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetReferenceImportJobRequestReferenceImportJobCompletedWaitTypeDef](./type_defs.md#getreferenceimportjobrequestreferenceimportjobcompletedwaittypedef) 
## RunCompletedWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("run_completed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.RunCompleted)

```python
# RunCompletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import RunCompletedWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: RunCompletedWaiter = client.get_waiter("run_completed")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [RunCompletedWaiter](./waiters.md#runcompletedwaiter)


### wait

Type annotations and code completion for `#!python RunCompletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    id: str,
    export: Sequence[RunExportType] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-brackets: RunExportType](./literals.md#runexporttype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetRunRequestRunCompletedWaitTypeDef = {  # (1)
    "id": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetRunRequestRunCompletedWaitTypeDef](./type_defs.md#getrunrequestruncompletedwaittypedef) 
## RunRunningWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("run_running")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.RunRunning)

```python
# RunRunningWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import RunRunningWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: RunRunningWaiter = client.get_waiter("run_running")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [RunRunningWaiter](./waiters.md#runrunningwaiter)


### wait

Type annotations and code completion for `#!python RunRunningWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    id: str,
    export: Sequence[RunExportType] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-brackets: RunExportType](./literals.md#runexporttype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetRunRequestRunRunningWaitTypeDef = {  # (1)
    "id": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetRunRequestRunRunningWaitTypeDef](./type_defs.md#getrunrequestrunrunningwaittypedef) 
## TaskCompletedWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("task_completed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.TaskCompleted)

```python
# TaskCompletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import TaskCompletedWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: TaskCompletedWaiter = client.get_waiter("task_completed")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [TaskCompletedWaiter](./waiters.md#taskcompletedwaiter)


### wait

Type annotations and code completion for `#!python TaskCompletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    id: str,
    taskId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetRunTaskRequestTaskCompletedWaitTypeDef = {  # (1)
    "id": ...,
    "taskId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetRunTaskRequestTaskCompletedWaitTypeDef](./type_defs.md#getruntaskrequesttaskcompletedwaittypedef) 
## TaskRunningWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("task_running")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.TaskRunning)

```python
# TaskRunningWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import TaskRunningWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: TaskRunningWaiter = client.get_waiter("task_running")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [TaskRunningWaiter](./waiters.md#taskrunningwaiter)


### wait

Type annotations and code completion for `#!python TaskRunningWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    id: str,
    taskId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetRunTaskRequestTaskRunningWaitTypeDef = {  # (1)
    "id": ...,
    "taskId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetRunTaskRequestTaskRunningWaitTypeDef](./type_defs.md#getruntaskrequesttaskrunningwaittypedef) 
## VariantImportJobCreatedWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("variant_import_job_created")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.VariantImportJobCreated)

```python
# VariantImportJobCreatedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import VariantImportJobCreatedWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: VariantImportJobCreatedWaiter = client.get_waiter("variant_import_job_created")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [VariantImportJobCreatedWaiter](./waiters.md#variantimportjobcreatedwaiter)


### wait

Type annotations and code completion for `#!python VariantImportJobCreatedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    jobId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetVariantImportRequestVariantImportJobCreatedWaitTypeDef = {  # (1)
    "jobId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetVariantImportRequestVariantImportJobCreatedWaitTypeDef](./type_defs.md#getvariantimportrequestvariantimportjobcreatedwaittypedef) 
## VariantStoreCreatedWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("variant_store_created")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.VariantStoreCreated)

```python
# VariantStoreCreatedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import VariantStoreCreatedWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: VariantStoreCreatedWaiter = client.get_waiter("variant_store_created")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [VariantStoreCreatedWaiter](./waiters.md#variantstorecreatedwaiter)


### wait

Type annotations and code completion for `#!python VariantStoreCreatedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    name: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetVariantStoreRequestVariantStoreCreatedWaitTypeDef = {  # (1)
    "name": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetVariantStoreRequestVariantStoreCreatedWaitTypeDef](./type_defs.md#getvariantstorerequestvariantstorecreatedwaittypedef) 
## VariantStoreDeletedWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("variant_store_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.VariantStoreDeleted)

```python
# VariantStoreDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import VariantStoreDeletedWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: VariantStoreDeletedWaiter = client.get_waiter("variant_store_deleted")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [VariantStoreDeletedWaiter](./waiters.md#variantstoredeletedwaiter)


### wait

Type annotations and code completion for `#!python VariantStoreDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    name: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetVariantStoreRequestVariantStoreDeletedWaitTypeDef = {  # (1)
    "name": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetVariantStoreRequestVariantStoreDeletedWaitTypeDef](./type_defs.md#getvariantstorerequestvariantstoredeletedwaittypedef) 
## WorkflowActiveWaiter

Type annotations and code completion for `#!python session.create_client("omics").get_waiter("workflow_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.WorkflowActive)

```python
# WorkflowActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_omics.waiter import WorkflowActiveWaiter

session = get_session()
async with session.create_client("omics") as client:  # (1)
    waiter: WorkflowActiveWaiter = client.get_waiter("workflow_active")  # (2)
    await waiter.wait()
```

1. client: [OmicsClient](./client.md)
2. waiter: [WorkflowActiveWaiter](./waiters.md#workflowactivewaiter)


### wait

Type annotations and code completion for `#!python WorkflowActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    id: str,
    type: WorkflowTypeType = ...,  # (1)
    export: Sequence[WorkflowExportType] = ...,  # (2)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (3)
) -> None:
    ...
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-brackets: WorkflowExportType](./literals.md#workflowexporttype) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetWorkflowRequestWorkflowActiveWaitTypeDef = {  # (1)
    "id": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetWorkflowRequestWorkflowActiveWaitTypeDef](./type_defs.md#getworkflowrequestworkflowactivewaittypedef) 
