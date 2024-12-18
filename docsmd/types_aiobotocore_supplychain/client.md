# SupplyChainClient

> [Index](../README.md) > [SupplyChain](./README.md) > SupplyChainClient

!!! note ""

    Auto-generated documentation for [SupplyChain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#supplychain)
    type annotations stubs module [types-aiobotocore-supplychain](https://pypi.org/project/types-aiobotocore-supplychain/).

## SupplyChainClient

Type annotations and code completion for `#!python session.create_client("supplychain")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client)

```python
# SupplyChainClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_supplychain.client import SupplyChainClient

session = get_session()
async with session.create_client("supplychain") as client:
    client: SupplyChainClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("supplychain").exceptions` structure.

```python
# SupplyChainClient.exceptions usage example

async with session.create_client("supplychain") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# SupplyChainClient usage type checking example

from types_aiobotocore_supplychain.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("supplychain").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("supplychain").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/generate_presigned_url.html)

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


### close



Type annotations and code completion for `#!python session.create_client("supplychain").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_bill\_of\_materials\_import\_job

CreateBillOfMaterialsImportJob creates an import job for the Product Bill Of
Materials (BOM) entity.

Type annotations and code completion for `#!python session.create_client("supplychain").create_bill_of_materials_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/create_bill_of_materials_import_job.html)

```python
# create_bill_of_materials_import_job method definition

await def create_bill_of_materials_import_job(
    self,
    *,
    instanceId: str,
    s3uri: str,
    clientToken: str = ...,
) -> CreateBillOfMaterialsImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateBillOfMaterialsImportJobResponseTypeDef](./type_defs.md#createbillofmaterialsimportjobresponsetypedef) 


```python
# create_bill_of_materials_import_job method usage example with argument unpacking

kwargs: CreateBillOfMaterialsImportJobRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "s3uri": ...,
}

parent.create_bill_of_materials_import_job(**kwargs)
```

1. See [:material-code-braces: CreateBillOfMaterialsImportJobRequestRequestTypeDef](./type_defs.md#createbillofmaterialsimportjobrequestrequesttypedef) 

### create\_data\_integration\_flow

Enables you to programmatically create a data pipeline to ingest data from
source systems such as Amazon S3 buckets, to a predefined Amazon Web Services
Supply Chain dataset (product, inbound_order) or a temporary dataset along with
the data transformation query provided with the API.

Type annotations and code completion for `#!python session.create_client("supplychain").create_data_integration_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/create_data_integration_flow.html)

```python
# create_data_integration_flow method definition

await def create_data_integration_flow(
    self,
    *,
    instanceId: str,
    name: str,
    sources: Sequence[DataIntegrationFlowSourceTypeDef],  # (1)
    transformation: DataIntegrationFlowTransformationTypeDef,  # (2)
    target: DataIntegrationFlowTargetTypeDef,  # (3)
    tags: Mapping[str, str] = ...,
) -> CreateDataIntegrationFlowResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DataIntegrationFlowSourceTypeDef](./type_defs.md#dataintegrationflowsourcetypedef) 
2. See [:material-code-braces: DataIntegrationFlowTransformationTypeDef](./type_defs.md#dataintegrationflowtransformationtypedef) 
3. See [:material-code-braces: DataIntegrationFlowTargetTypeDef](./type_defs.md#dataintegrationflowtargettypedef) 
4. See [:material-code-braces: CreateDataIntegrationFlowResponseTypeDef](./type_defs.md#createdataintegrationflowresponsetypedef) 


```python
# create_data_integration_flow method usage example with argument unpacking

kwargs: CreateDataIntegrationFlowRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "name": ...,
    "sources": ...,
    "transformation": ...,
    "target": ...,
}

parent.create_data_integration_flow(**kwargs)
```

1. See [:material-code-braces: CreateDataIntegrationFlowRequestRequestTypeDef](./type_defs.md#createdataintegrationflowrequestrequesttypedef) 

### create\_data\_lake\_dataset

Enables you to programmatically create an Amazon Web Services Supply Chain data
lake dataset.

Type annotations and code completion for `#!python session.create_client("supplychain").create_data_lake_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/create_data_lake_dataset.html)

```python
# create_data_lake_dataset method definition

await def create_data_lake_dataset(
    self,
    *,
    instanceId: str,
    namespace: str,
    name: str,
    schema: DataLakeDatasetSchemaTypeDef = ...,  # (1)
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateDataLakeDatasetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataLakeDatasetSchemaTypeDef](./type_defs.md#datalakedatasetschematypedef) 
2. See [:material-code-braces: CreateDataLakeDatasetResponseTypeDef](./type_defs.md#createdatalakedatasetresponsetypedef) 


```python
# create_data_lake_dataset method usage example with argument unpacking

kwargs: CreateDataLakeDatasetRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "namespace": ...,
    "name": ...,
}

parent.create_data_lake_dataset(**kwargs)
```

1. See [:material-code-braces: CreateDataLakeDatasetRequestRequestTypeDef](./type_defs.md#createdatalakedatasetrequestrequesttypedef) 

### create\_instance

Enables you to programmatically create an Amazon Web Services Supply Chain
instance by applying KMS keys and relevant information associated with the API
without using the Amazon Web Services console.

Type annotations and code completion for `#!python session.create_client("supplychain").create_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/create_instance.html)

```python
# create_instance method definition

await def create_instance(
    self,
    *,
    instanceName: str = ...,
    instanceDescription: str = ...,
    kmsKeyArn: str = ...,
    tags: Mapping[str, str] = ...,
    clientToken: str = ...,
) -> CreateInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateInstanceResponseTypeDef](./type_defs.md#createinstanceresponsetypedef) 


```python
# create_instance method usage example with argument unpacking

kwargs: CreateInstanceRequestRequestTypeDef = {  # (1)
    "instanceName": ...,
}

parent.create_instance(**kwargs)
```

1. See [:material-code-braces: CreateInstanceRequestRequestTypeDef](./type_defs.md#createinstancerequestrequesttypedef) 

### delete\_data\_integration\_flow

Enable you to programmatically delete an existing data pipeline for the
provided Amazon Web Services Supply Chain instance and DataIntegrationFlow
name.

Type annotations and code completion for `#!python session.create_client("supplychain").delete_data_integration_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/delete_data_integration_flow.html)

```python
# delete_data_integration_flow method definition

await def delete_data_integration_flow(
    self,
    *,
    instanceId: str,
    name: str,
) -> DeleteDataIntegrationFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataIntegrationFlowResponseTypeDef](./type_defs.md#deletedataintegrationflowresponsetypedef) 


```python
# delete_data_integration_flow method usage example with argument unpacking

kwargs: DeleteDataIntegrationFlowRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "name": ...,
}

parent.delete_data_integration_flow(**kwargs)
```

1. See [:material-code-braces: DeleteDataIntegrationFlowRequestRequestTypeDef](./type_defs.md#deletedataintegrationflowrequestrequesttypedef) 

### delete\_data\_lake\_dataset

Enables you to programmatically delete an Amazon Web Services Supply Chain data
lake dataset.

Type annotations and code completion for `#!python session.create_client("supplychain").delete_data_lake_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/delete_data_lake_dataset.html)

```python
# delete_data_lake_dataset method definition

await def delete_data_lake_dataset(
    self,
    *,
    instanceId: str,
    namespace: str,
    name: str,
) -> DeleteDataLakeDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataLakeDatasetResponseTypeDef](./type_defs.md#deletedatalakedatasetresponsetypedef) 


```python
# delete_data_lake_dataset method usage example with argument unpacking

kwargs: DeleteDataLakeDatasetRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "namespace": ...,
    "name": ...,
}

parent.delete_data_lake_dataset(**kwargs)
```

1. See [:material-code-braces: DeleteDataLakeDatasetRequestRequestTypeDef](./type_defs.md#deletedatalakedatasetrequestrequesttypedef) 

### delete\_instance

Enables you to programmatically delete an Amazon Web Services Supply Chain
instance by deleting the KMS keys and relevant information associated with the
API without using the Amazon Web Services console.

Type annotations and code completion for `#!python session.create_client("supplychain").delete_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/delete_instance.html)

```python
# delete_instance method definition

await def delete_instance(
    self,
    *,
    instanceId: str,
) -> DeleteInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteInstanceResponseTypeDef](./type_defs.md#deleteinstanceresponsetypedef) 


```python
# delete_instance method usage example with argument unpacking

kwargs: DeleteInstanceRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
}

parent.delete_instance(**kwargs)
```

1. See [:material-code-braces: DeleteInstanceRequestRequestTypeDef](./type_defs.md#deleteinstancerequestrequesttypedef) 

### get\_bill\_of\_materials\_import\_job

Get status and details of a BillOfMaterialsImportJob.

Type annotations and code completion for `#!python session.create_client("supplychain").get_bill_of_materials_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/get_bill_of_materials_import_job.html)

```python
# get_bill_of_materials_import_job method definition

await def get_bill_of_materials_import_job(
    self,
    *,
    instanceId: str,
    jobId: str,
) -> GetBillOfMaterialsImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBillOfMaterialsImportJobResponseTypeDef](./type_defs.md#getbillofmaterialsimportjobresponsetypedef) 


```python
# get_bill_of_materials_import_job method usage example with argument unpacking

kwargs: GetBillOfMaterialsImportJobRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "jobId": ...,
}

parent.get_bill_of_materials_import_job(**kwargs)
```

1. See [:material-code-braces: GetBillOfMaterialsImportJobRequestRequestTypeDef](./type_defs.md#getbillofmaterialsimportjobrequestrequesttypedef) 

### get\_data\_integration\_flow

Enables you to programmatically view a specific data pipeline for the provided
Amazon Web Services Supply Chain instance and DataIntegrationFlow name.

Type annotations and code completion for `#!python session.create_client("supplychain").get_data_integration_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/get_data_integration_flow.html)

```python
# get_data_integration_flow method definition

await def get_data_integration_flow(
    self,
    *,
    instanceId: str,
    name: str,
) -> GetDataIntegrationFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataIntegrationFlowResponseTypeDef](./type_defs.md#getdataintegrationflowresponsetypedef) 


```python
# get_data_integration_flow method usage example with argument unpacking

kwargs: GetDataIntegrationFlowRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "name": ...,
}

parent.get_data_integration_flow(**kwargs)
```

1. See [:material-code-braces: GetDataIntegrationFlowRequestRequestTypeDef](./type_defs.md#getdataintegrationflowrequestrequesttypedef) 

### get\_data\_lake\_dataset

Enables you to programmatically view an Amazon Web Services Supply Chain data
lake dataset.

Type annotations and code completion for `#!python session.create_client("supplychain").get_data_lake_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/get_data_lake_dataset.html)

```python
# get_data_lake_dataset method definition

await def get_data_lake_dataset(
    self,
    *,
    instanceId: str,
    namespace: str,
    name: str,
) -> GetDataLakeDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataLakeDatasetResponseTypeDef](./type_defs.md#getdatalakedatasetresponsetypedef) 


```python
# get_data_lake_dataset method usage example with argument unpacking

kwargs: GetDataLakeDatasetRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "namespace": ...,
    "name": ...,
}

parent.get_data_lake_dataset(**kwargs)
```

1. See [:material-code-braces: GetDataLakeDatasetRequestRequestTypeDef](./type_defs.md#getdatalakedatasetrequestrequesttypedef) 

### get\_instance

Enables you to programmatically retrieve the information related to an Amazon
Web Services Supply Chain instance ID.

Type annotations and code completion for `#!python session.create_client("supplychain").get_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/get_instance.html)

```python
# get_instance method definition

await def get_instance(
    self,
    *,
    instanceId: str,
) -> GetInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInstanceResponseTypeDef](./type_defs.md#getinstanceresponsetypedef) 


```python
# get_instance method usage example with argument unpacking

kwargs: GetInstanceRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
}

parent.get_instance(**kwargs)
```

1. See [:material-code-braces: GetInstanceRequestRequestTypeDef](./type_defs.md#getinstancerequestrequesttypedef) 

### list\_data\_integration\_flows

Enables you to programmatically list all data pipelines for the provided Amazon
Web Services Supply Chain instance.

Type annotations and code completion for `#!python session.create_client("supplychain").list_data_integration_flows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/list_data_integration_flows.html)

```python
# list_data_integration_flows method definition

await def list_data_integration_flows(
    self,
    *,
    instanceId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDataIntegrationFlowsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataIntegrationFlowsResponseTypeDef](./type_defs.md#listdataintegrationflowsresponsetypedef) 


```python
# list_data_integration_flows method usage example with argument unpacking

kwargs: ListDataIntegrationFlowsRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
}

parent.list_data_integration_flows(**kwargs)
```

1. See [:material-code-braces: ListDataIntegrationFlowsRequestRequestTypeDef](./type_defs.md#listdataintegrationflowsrequestrequesttypedef) 

### list\_data\_lake\_datasets

Enables you to programmatically view the list of Amazon Web Services Supply
Chain data lake datasets.

Type annotations and code completion for `#!python session.create_client("supplychain").list_data_lake_datasets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/list_data_lake_datasets.html)

```python
# list_data_lake_datasets method definition

await def list_data_lake_datasets(
    self,
    *,
    instanceId: str,
    namespace: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDataLakeDatasetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataLakeDatasetsResponseTypeDef](./type_defs.md#listdatalakedatasetsresponsetypedef) 


```python
# list_data_lake_datasets method usage example with argument unpacking

kwargs: ListDataLakeDatasetsRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "namespace": ...,
}

parent.list_data_lake_datasets(**kwargs)
```

1. See [:material-code-braces: ListDataLakeDatasetsRequestRequestTypeDef](./type_defs.md#listdatalakedatasetsrequestrequesttypedef) 

### list\_instances

List all Amazon Web Services Supply Chain instances for a specific account.

Type annotations and code completion for `#!python session.create_client("supplychain").list_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/list_instances.html)

```python
# list_instances method definition

await def list_instances(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    instanceNameFilter: Sequence[str] = ...,
    instanceStateFilter: Sequence[InstanceStateType] = ...,  # (1)
) -> ListInstancesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
2. See [:material-code-braces: ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef) 


```python
# list_instances method usage example with argument unpacking

kwargs: ListInstancesRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_instances(**kwargs)
```

1. See [:material-code-braces: ListInstancesRequestRequestTypeDef](./type_defs.md#listinstancesrequestrequesttypedef) 

### list\_tags\_for\_resource

List all the tags for an Amazon Web ServicesSupply Chain resource.

Type annotations and code completion for `#!python session.create_client("supplychain").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/list_tags_for_resource.html)

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

### send\_data\_integration\_event

Send the transactional data payload for the event with real-time data for
analysis or monitoring.

Type annotations and code completion for `#!python session.create_client("supplychain").send_data_integration_event` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/send_data_integration_event.html)

```python
# send_data_integration_event method definition

await def send_data_integration_event(
    self,
    *,
    instanceId: str,
    eventType: DataIntegrationEventTypeType,  # (1)
    data: str,
    eventGroupId: str,
    eventTimestamp: TimestampTypeDef = ...,
    clientToken: str = ...,
) -> SendDataIntegrationEventResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataIntegrationEventTypeType](./literals.md#dataintegrationeventtypetype) 
2. See [:material-code-braces: SendDataIntegrationEventResponseTypeDef](./type_defs.md#senddataintegrationeventresponsetypedef) 


```python
# send_data_integration_event method usage example with argument unpacking

kwargs: SendDataIntegrationEventRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "eventType": ...,
    "data": ...,
    "eventGroupId": ...,
}

parent.send_data_integration_event(**kwargs)
```

1. See [:material-code-braces: SendDataIntegrationEventRequestRequestTypeDef](./type_defs.md#senddataintegrationeventrequestrequesttypedef) 

### tag\_resource

You can create tags during or after creating a resource such as instance, data
flow, or dataset in AWS Supply chain.

Type annotations and code completion for `#!python session.create_client("supplychain").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/tag_resource.html)

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

You can delete tags for an Amazon Web Services Supply chain resource such as
instance, data flow, or dataset in AWS Supply Chain.

Type annotations and code completion for `#!python session.create_client("supplychain").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/untag_resource.html)

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

### update\_data\_integration\_flow

Enables you to programmatically update an existing data pipeline to ingest data
from the source systems such as, Amazon S3 buckets, to a predefined Amazon Web
Services Supply Chain dataset (product, inbound_order) or a temporary dataset
along with the data transformation query provided with the API.

Type annotations and code completion for `#!python session.create_client("supplychain").update_data_integration_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/update_data_integration_flow.html)

```python
# update_data_integration_flow method definition

await def update_data_integration_flow(
    self,
    *,
    instanceId: str,
    name: str,
    sources: Sequence[DataIntegrationFlowSourceTypeDef] = ...,  # (1)
    transformation: DataIntegrationFlowTransformationTypeDef = ...,  # (2)
    target: DataIntegrationFlowTargetTypeDef = ...,  # (3)
) -> UpdateDataIntegrationFlowResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DataIntegrationFlowSourceTypeDef](./type_defs.md#dataintegrationflowsourcetypedef) 
2. See [:material-code-braces: DataIntegrationFlowTransformationTypeDef](./type_defs.md#dataintegrationflowtransformationtypedef) 
3. See [:material-code-braces: DataIntegrationFlowTargetTypeDef](./type_defs.md#dataintegrationflowtargettypedef) 
4. See [:material-code-braces: UpdateDataIntegrationFlowResponseTypeDef](./type_defs.md#updatedataintegrationflowresponsetypedef) 


```python
# update_data_integration_flow method usage example with argument unpacking

kwargs: UpdateDataIntegrationFlowRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "name": ...,
}

parent.update_data_integration_flow(**kwargs)
```

1. See [:material-code-braces: UpdateDataIntegrationFlowRequestRequestTypeDef](./type_defs.md#updatedataintegrationflowrequestrequesttypedef) 

### update\_data\_lake\_dataset

Enables you to programmatically update an Amazon Web Services Supply Chain data
lake dataset.

Type annotations and code completion for `#!python session.create_client("supplychain").update_data_lake_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/update_data_lake_dataset.html)

```python
# update_data_lake_dataset method definition

await def update_data_lake_dataset(
    self,
    *,
    instanceId: str,
    namespace: str,
    name: str,
    description: str = ...,
) -> UpdateDataLakeDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDataLakeDatasetResponseTypeDef](./type_defs.md#updatedatalakedatasetresponsetypedef) 


```python
# update_data_lake_dataset method usage example with argument unpacking

kwargs: UpdateDataLakeDatasetRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "namespace": ...,
    "name": ...,
}

parent.update_data_lake_dataset(**kwargs)
```

1. See [:material-code-braces: UpdateDataLakeDatasetRequestRequestTypeDef](./type_defs.md#updatedatalakedatasetrequestrequesttypedef) 

### update\_instance

Enables you to programmatically update an Amazon Web Services Supply Chain
instance description by providing all the relevant information such as account
ID, instance ID and so on without using the AWS console.

Type annotations and code completion for `#!python session.create_client("supplychain").update_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/client/update_instance.html)

```python
# update_instance method definition

await def update_instance(
    self,
    *,
    instanceId: str,
    instanceName: str = ...,
    instanceDescription: str = ...,
) -> UpdateInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateInstanceResponseTypeDef](./type_defs.md#updateinstanceresponsetypedef) 


```python
# update_instance method usage example with argument unpacking

kwargs: UpdateInstanceRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
}

parent.update_instance(**kwargs)
```

1. See [:material-code-braces: UpdateInstanceRequestRequestTypeDef](./type_defs.md#updateinstancerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("supplychain").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "SupplyChainClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("supplychain").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client)

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

Type annotations and code completion for `#!python session.create_client("supplychain").get_paginator` method with overloads.

- `client.get_paginator("list_data_integration_flows")` -> [ListDataIntegrationFlowsPaginator](./paginators.md#listdataintegrationflowspaginator)
- `client.get_paginator("list_data_lake_datasets")` -> [ListDataLakeDatasetsPaginator](./paginators.md#listdatalakedatasetspaginator)
- `client.get_paginator("list_instances")` -> [ListInstancesPaginator](./paginators.md#listinstancespaginator)



