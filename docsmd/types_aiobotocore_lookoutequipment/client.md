# LookoutEquipmentClient

> [Index](../README.md) > [LookoutEquipment](./README.md) > LookoutEquipmentClient

!!! note ""

    Auto-generated documentation for [LookoutEquipment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
    type annotations stubs module [types-aiobotocore-lookoutequipment](https://pypi.org/project/types-aiobotocore-lookoutequipment/).

## LookoutEquipmentClient

Type annotations and code completion for `#!python session.create_client("lookoutequipment")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client)

```python
# LookoutEquipmentClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_lookoutequipment.client import LookoutEquipmentClient

session = get_session()
async with session.create_client("lookoutequipment") as client:
    client: LookoutEquipmentClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("lookoutequipment").exceptions` structure.

```python
# LookoutEquipmentClient.exceptions usage example

async with session.create_client("lookoutequipment") as client:
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
# LookoutEquipmentClient usage type checking example

from types_aiobotocore_lookoutequipment.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_dataset

Creates a container for a collection of data being ingested for analysis.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").create_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_dataset)

```python
# create_dataset method definition

await def create_dataset(
    self,
    *,
    DatasetName: str,
    ClientToken: str,
    DatasetSchema: DatasetSchemaTypeDef = ...,  # (1)
    ServerSideKmsKeyId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateDatasetResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DatasetSchemaTypeDef](./type_defs.md#datasetschematypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef) 


```python
# create_dataset method usage example with argument unpacking

kwargs: CreateDatasetRequestRequestTypeDef = {  # (1)
    "DatasetName": ...,
    "ClientToken": ...,
}

parent.create_dataset(**kwargs)
```

1. See [:material-code-braces: CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef) 

### create\_inference\_scheduler

Creates a scheduled inference.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").create_inference_scheduler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_inference_scheduler)

```python
# create_inference_scheduler method definition

await def create_inference_scheduler(
    self,
    *,
    ModelName: str,
    InferenceSchedulerName: str,
    DataUploadFrequency: DataUploadFrequencyType,  # (1)
    DataInputConfiguration: InferenceInputConfigurationTypeDef,  # (2)
    DataOutputConfiguration: InferenceOutputConfigurationTypeDef,  # (3)
    RoleArn: str,
    ClientToken: str,
    DataDelayOffsetInMinutes: int = ...,
    ServerSideKmsKeyId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateInferenceSchedulerResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: DataUploadFrequencyType](./literals.md#datauploadfrequencytype) 
2. See [:material-code-braces: InferenceInputConfigurationTypeDef](./type_defs.md#inferenceinputconfigurationtypedef) 
3. See [:material-code-braces: InferenceOutputConfigurationTypeDef](./type_defs.md#inferenceoutputconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateInferenceSchedulerResponseTypeDef](./type_defs.md#createinferenceschedulerresponsetypedef) 


```python
# create_inference_scheduler method usage example with argument unpacking

kwargs: CreateInferenceSchedulerRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
    "InferenceSchedulerName": ...,
    "DataUploadFrequency": ...,
    "DataInputConfiguration": ...,
    "DataOutputConfiguration": ...,
    "RoleArn": ...,
    "ClientToken": ...,
}

parent.create_inference_scheduler(**kwargs)
```

1. See [:material-code-braces: CreateInferenceSchedulerRequestRequestTypeDef](./type_defs.md#createinferenceschedulerrequestrequesttypedef) 

### create\_label

Creates a label for an event.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").create_label` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_label)

```python
# create_label method definition

await def create_label(
    self,
    *,
    LabelGroupName: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Rating: LabelRatingType,  # (1)
    ClientToken: str,
    FaultCode: str = ...,
    Notes: str = ...,
    Equipment: str = ...,
) -> CreateLabelResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LabelRatingType](./literals.md#labelratingtype) 
2. See [:material-code-braces: CreateLabelResponseTypeDef](./type_defs.md#createlabelresponsetypedef) 


```python
# create_label method usage example with argument unpacking

kwargs: CreateLabelRequestRequestTypeDef = {  # (1)
    "LabelGroupName": ...,
    "StartTime": ...,
    "EndTime": ...,
    "Rating": ...,
    "ClientToken": ...,
}

parent.create_label(**kwargs)
```

1. See [:material-code-braces: CreateLabelRequestRequestTypeDef](./type_defs.md#createlabelrequestrequesttypedef) 

### create\_label\_group

Creates a group of labels.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").create_label_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_label_group)

```python
# create_label_group method definition

await def create_label_group(
    self,
    *,
    LabelGroupName: str,
    ClientToken: str,
    FaultCodes: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateLabelGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateLabelGroupResponseTypeDef](./type_defs.md#createlabelgroupresponsetypedef) 


```python
# create_label_group method usage example with argument unpacking

kwargs: CreateLabelGroupRequestRequestTypeDef = {  # (1)
    "LabelGroupName": ...,
    "ClientToken": ...,
}

parent.create_label_group(**kwargs)
```

1. See [:material-code-braces: CreateLabelGroupRequestRequestTypeDef](./type_defs.md#createlabelgrouprequestrequesttypedef) 

### create\_model

Creates a machine learning model for data inference.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").create_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_model)

```python
# create_model method definition

await def create_model(
    self,
    *,
    ModelName: str,
    DatasetName: str,
    ClientToken: str,
    DatasetSchema: DatasetSchemaTypeDef = ...,  # (1)
    LabelsInputConfiguration: LabelsInputConfigurationTypeDef = ...,  # (2)
    TrainingDataStartTime: TimestampTypeDef = ...,
    TrainingDataEndTime: TimestampTypeDef = ...,
    EvaluationDataStartTime: TimestampTypeDef = ...,
    EvaluationDataEndTime: TimestampTypeDef = ...,
    RoleArn: str = ...,
    DataPreProcessingConfiguration: DataPreProcessingConfigurationTypeDef = ...,  # (3)
    ServerSideKmsKeyId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    OffCondition: str = ...,
    ModelDiagnosticsOutputConfiguration: ModelDiagnosticsOutputConfigurationTypeDef = ...,  # (5)
) -> CreateModelResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DatasetSchemaTypeDef](./type_defs.md#datasetschematypedef) 
2. See [:material-code-braces: LabelsInputConfigurationTypeDef](./type_defs.md#labelsinputconfigurationtypedef) 
3. See [:material-code-braces: DataPreProcessingConfigurationTypeDef](./type_defs.md#datapreprocessingconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: ModelDiagnosticsOutputConfigurationTypeDef](./type_defs.md#modeldiagnosticsoutputconfigurationtypedef) 
6. See [:material-code-braces: CreateModelResponseTypeDef](./type_defs.md#createmodelresponsetypedef) 


```python
# create_model method usage example with argument unpacking

kwargs: CreateModelRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
    "DatasetName": ...,
    "ClientToken": ...,
}

parent.create_model(**kwargs)
```

1. See [:material-code-braces: CreateModelRequestRequestTypeDef](./type_defs.md#createmodelrequestrequesttypedef) 

### create\_retraining\_scheduler

Creates a retraining scheduler on the specified model.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").create_retraining_scheduler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_retraining_scheduler)

```python
# create_retraining_scheduler method definition

await def create_retraining_scheduler(
    self,
    *,
    ModelName: str,
    RetrainingFrequency: str,
    LookbackWindow: str,
    ClientToken: str,
    RetrainingStartDate: TimestampTypeDef = ...,
    PromoteMode: ModelPromoteModeType = ...,  # (1)
) -> CreateRetrainingSchedulerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ModelPromoteModeType](./literals.md#modelpromotemodetype) 
2. See [:material-code-braces: CreateRetrainingSchedulerResponseTypeDef](./type_defs.md#createretrainingschedulerresponsetypedef) 


```python
# create_retraining_scheduler method usage example with argument unpacking

kwargs: CreateRetrainingSchedulerRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
    "RetrainingFrequency": ...,
    "LookbackWindow": ...,
    "ClientToken": ...,
}

parent.create_retraining_scheduler(**kwargs)
```

1. See [:material-code-braces: CreateRetrainingSchedulerRequestRequestTypeDef](./type_defs.md#createretrainingschedulerrequestrequesttypedef) 

### delete\_dataset

Deletes a dataset and associated artifacts.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").delete_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.delete_dataset)

```python
# delete_dataset method definition

await def delete_dataset(
    self,
    *,
    DatasetName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_dataset method usage example with argument unpacking

kwargs: DeleteDatasetRequestRequestTypeDef = {  # (1)
    "DatasetName": ...,
}

parent.delete_dataset(**kwargs)
```

1. See [:material-code-braces: DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef) 

### delete\_inference\_scheduler

Deletes an inference scheduler that has been set up.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").delete_inference_scheduler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.delete_inference_scheduler)

```python
# delete_inference_scheduler method definition

await def delete_inference_scheduler(
    self,
    *,
    InferenceSchedulerName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_inference_scheduler method usage example with argument unpacking

kwargs: DeleteInferenceSchedulerRequestRequestTypeDef = {  # (1)
    "InferenceSchedulerName": ...,
}

parent.delete_inference_scheduler(**kwargs)
```

1. See [:material-code-braces: DeleteInferenceSchedulerRequestRequestTypeDef](./type_defs.md#deleteinferenceschedulerrequestrequesttypedef) 

### delete\_label

Deletes a label.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").delete_label` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.delete_label)

```python
# delete_label method definition

await def delete_label(
    self,
    *,
    LabelGroupName: str,
    LabelId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_label method usage example with argument unpacking

kwargs: DeleteLabelRequestRequestTypeDef = {  # (1)
    "LabelGroupName": ...,
    "LabelId": ...,
}

parent.delete_label(**kwargs)
```

1. See [:material-code-braces: DeleteLabelRequestRequestTypeDef](./type_defs.md#deletelabelrequestrequesttypedef) 

### delete\_label\_group

Deletes a group of labels.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").delete_label_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.delete_label_group)

```python
# delete_label_group method definition

await def delete_label_group(
    self,
    *,
    LabelGroupName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_label_group method usage example with argument unpacking

kwargs: DeleteLabelGroupRequestRequestTypeDef = {  # (1)
    "LabelGroupName": ...,
}

parent.delete_label_group(**kwargs)
```

1. See [:material-code-braces: DeleteLabelGroupRequestRequestTypeDef](./type_defs.md#deletelabelgrouprequestrequesttypedef) 

### delete\_model

Deletes a machine learning model currently available for Amazon Lookout for
Equipment.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").delete_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.delete_model)

```python
# delete_model method definition

await def delete_model(
    self,
    *,
    ModelName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_model method usage example with argument unpacking

kwargs: DeleteModelRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
}

parent.delete_model(**kwargs)
```

1. See [:material-code-braces: DeleteModelRequestRequestTypeDef](./type_defs.md#deletemodelrequestrequesttypedef) 

### delete\_resource\_policy

Deletes the resource policy attached to the resource.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.delete_resource_policy)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    ResourceArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef) 

### delete\_retraining\_scheduler

Deletes a retraining scheduler from a model.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").delete_retraining_scheduler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.delete_retraining_scheduler)

```python
# delete_retraining_scheduler method definition

await def delete_retraining_scheduler(
    self,
    *,
    ModelName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_retraining_scheduler method usage example with argument unpacking

kwargs: DeleteRetrainingSchedulerRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
}

parent.delete_retraining_scheduler(**kwargs)
```

1. See [:material-code-braces: DeleteRetrainingSchedulerRequestRequestTypeDef](./type_defs.md#deleteretrainingschedulerrequestrequesttypedef) 

### describe\_data\_ingestion\_job

Provides information on a specific data ingestion job such as creation time,
dataset ARN, and
status.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").describe_data_ingestion_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_data_ingestion_job)

```python
# describe_data_ingestion_job method definition

await def describe_data_ingestion_job(
    self,
    *,
    JobId: str,
) -> DescribeDataIngestionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDataIngestionJobResponseTypeDef](./type_defs.md#describedataingestionjobresponsetypedef) 


```python
# describe_data_ingestion_job method usage example with argument unpacking

kwargs: DescribeDataIngestionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_data_ingestion_job(**kwargs)
```

1. See [:material-code-braces: DescribeDataIngestionJobRequestRequestTypeDef](./type_defs.md#describedataingestionjobrequestrequesttypedef) 

### describe\_dataset

Provides a JSON description of the data in each time series dataset, including
names, column names, and data
types.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").describe_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_dataset)

```python
# describe_dataset method definition

await def describe_dataset(
    self,
    *,
    DatasetName: str,
) -> DescribeDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef) 


```python
# describe_dataset method usage example with argument unpacking

kwargs: DescribeDatasetRequestRequestTypeDef = {  # (1)
    "DatasetName": ...,
}

parent.describe_dataset(**kwargs)
```

1. See [:material-code-braces: DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef) 

### describe\_inference\_scheduler

Specifies information about the inference scheduler being used, including name,
model, status, and associated metadata See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/lookoutequipment-2020-12-15/DescribeInferenceScheduler).

Type annotations and code completion for `#!python session.create_client("lookoutequipment").describe_inference_scheduler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_inference_scheduler)

```python
# describe_inference_scheduler method definition

await def describe_inference_scheduler(
    self,
    *,
    InferenceSchedulerName: str,
) -> DescribeInferenceSchedulerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInferenceSchedulerResponseTypeDef](./type_defs.md#describeinferenceschedulerresponsetypedef) 


```python
# describe_inference_scheduler method usage example with argument unpacking

kwargs: DescribeInferenceSchedulerRequestRequestTypeDef = {  # (1)
    "InferenceSchedulerName": ...,
}

parent.describe_inference_scheduler(**kwargs)
```

1. See [:material-code-braces: DescribeInferenceSchedulerRequestRequestTypeDef](./type_defs.md#describeinferenceschedulerrequestrequesttypedef) 

### describe\_label

Returns the name of the label.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").describe_label` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_label)

```python
# describe_label method definition

await def describe_label(
    self,
    *,
    LabelGroupName: str,
    LabelId: str,
) -> DescribeLabelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLabelResponseTypeDef](./type_defs.md#describelabelresponsetypedef) 


```python
# describe_label method usage example with argument unpacking

kwargs: DescribeLabelRequestRequestTypeDef = {  # (1)
    "LabelGroupName": ...,
    "LabelId": ...,
}

parent.describe_label(**kwargs)
```

1. See [:material-code-braces: DescribeLabelRequestRequestTypeDef](./type_defs.md#describelabelrequestrequesttypedef) 

### describe\_label\_group

Returns information about the label group.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").describe_label_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_label_group)

```python
# describe_label_group method definition

await def describe_label_group(
    self,
    *,
    LabelGroupName: str,
) -> DescribeLabelGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLabelGroupResponseTypeDef](./type_defs.md#describelabelgroupresponsetypedef) 


```python
# describe_label_group method usage example with argument unpacking

kwargs: DescribeLabelGroupRequestRequestTypeDef = {  # (1)
    "LabelGroupName": ...,
}

parent.describe_label_group(**kwargs)
```

1. See [:material-code-braces: DescribeLabelGroupRequestRequestTypeDef](./type_defs.md#describelabelgrouprequestrequesttypedef) 

### describe\_model

Provides a JSON containing the overall information about a specific machine
learning model, including model name and ARN, dataset, training and evaluation
information, status, and so
on.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").describe_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_model)

```python
# describe_model method definition

await def describe_model(
    self,
    *,
    ModelName: str,
) -> DescribeModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeModelResponseTypeDef](./type_defs.md#describemodelresponsetypedef) 


```python
# describe_model method usage example with argument unpacking

kwargs: DescribeModelRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
}

parent.describe_model(**kwargs)
```

1. See [:material-code-braces: DescribeModelRequestRequestTypeDef](./type_defs.md#describemodelrequestrequesttypedef) 

### describe\_model\_version

Retrieves information about a specific machine learning model version.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").describe_model_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_model_version)

```python
# describe_model_version method definition

await def describe_model_version(
    self,
    *,
    ModelName: str,
    ModelVersion: int,
) -> DescribeModelVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeModelVersionResponseTypeDef](./type_defs.md#describemodelversionresponsetypedef) 


```python
# describe_model_version method usage example with argument unpacking

kwargs: DescribeModelVersionRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
    "ModelVersion": ...,
}

parent.describe_model_version(**kwargs)
```

1. See [:material-code-braces: DescribeModelVersionRequestRequestTypeDef](./type_defs.md#describemodelversionrequestrequesttypedef) 

### describe\_resource\_policy

Provides the details of a resource policy attached to a resource.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").describe_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_resource_policy)

```python
# describe_resource_policy method definition

await def describe_resource_policy(
    self,
    *,
    ResourceArn: str,
) -> DescribeResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeResourcePolicyResponseTypeDef](./type_defs.md#describeresourcepolicyresponsetypedef) 


```python
# describe_resource_policy method usage example with argument unpacking

kwargs: DescribeResourcePolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.describe_resource_policy(**kwargs)
```

1. See [:material-code-braces: DescribeResourcePolicyRequestRequestTypeDef](./type_defs.md#describeresourcepolicyrequestrequesttypedef) 

### describe\_retraining\_scheduler

Provides a description of the retraining scheduler, including information such
as the model name and retraining
parameters.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").describe_retraining_scheduler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_retraining_scheduler)

```python
# describe_retraining_scheduler method definition

await def describe_retraining_scheduler(
    self,
    *,
    ModelName: str,
) -> DescribeRetrainingSchedulerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRetrainingSchedulerResponseTypeDef](./type_defs.md#describeretrainingschedulerresponsetypedef) 


```python
# describe_retraining_scheduler method usage example with argument unpacking

kwargs: DescribeRetrainingSchedulerRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
}

parent.describe_retraining_scheduler(**kwargs)
```

1. See [:material-code-braces: DescribeRetrainingSchedulerRequestRequestTypeDef](./type_defs.md#describeretrainingschedulerrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.generate_presigned_url)

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


### import\_dataset

Imports a dataset.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").import_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.import_dataset)

```python
# import_dataset method definition

await def import_dataset(
    self,
    *,
    SourceDatasetArn: str,
    ClientToken: str,
    DatasetName: str = ...,
    ServerSideKmsKeyId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> ImportDatasetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ImportDatasetResponseTypeDef](./type_defs.md#importdatasetresponsetypedef) 


```python
# import_dataset method usage example with argument unpacking

kwargs: ImportDatasetRequestRequestTypeDef = {  # (1)
    "SourceDatasetArn": ...,
    "ClientToken": ...,
}

parent.import_dataset(**kwargs)
```

1. See [:material-code-braces: ImportDatasetRequestRequestTypeDef](./type_defs.md#importdatasetrequestrequesttypedef) 

### import\_model\_version

Imports a model that has been trained successfully.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").import_model_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.import_model_version)

```python
# import_model_version method definition

await def import_model_version(
    self,
    *,
    SourceModelVersionArn: str,
    DatasetName: str,
    ClientToken: str,
    ModelName: str = ...,
    LabelsInputConfiguration: LabelsInputConfigurationTypeDef = ...,  # (1)
    RoleArn: str = ...,
    ServerSideKmsKeyId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    InferenceDataImportStrategy: InferenceDataImportStrategyType = ...,  # (3)
) -> ImportModelVersionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: LabelsInputConfigurationTypeDef](./type_defs.md#labelsinputconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: InferenceDataImportStrategyType](./literals.md#inferencedataimportstrategytype) 
4. See [:material-code-braces: ImportModelVersionResponseTypeDef](./type_defs.md#importmodelversionresponsetypedef) 


```python
# import_model_version method usage example with argument unpacking

kwargs: ImportModelVersionRequestRequestTypeDef = {  # (1)
    "SourceModelVersionArn": ...,
    "DatasetName": ...,
    "ClientToken": ...,
}

parent.import_model_version(**kwargs)
```

1. See [:material-code-braces: ImportModelVersionRequestRequestTypeDef](./type_defs.md#importmodelversionrequestrequesttypedef) 

### list\_data\_ingestion\_jobs

Provides a list of all data ingestion jobs, including dataset name and ARN, S3
location of the input data, status, and so
on.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").list_data_ingestion_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_data_ingestion_jobs)

```python
# list_data_ingestion_jobs method definition

await def list_data_ingestion_jobs(
    self,
    *,
    DatasetName: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    Status: IngestionJobStatusType = ...,  # (1)
) -> ListDataIngestionJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: IngestionJobStatusType](./literals.md#ingestionjobstatustype) 
2. See [:material-code-braces: ListDataIngestionJobsResponseTypeDef](./type_defs.md#listdataingestionjobsresponsetypedef) 


```python
# list_data_ingestion_jobs method usage example with argument unpacking

kwargs: ListDataIngestionJobsRequestRequestTypeDef = {  # (1)
    "DatasetName": ...,
}

parent.list_data_ingestion_jobs(**kwargs)
```

1. See [:material-code-braces: ListDataIngestionJobsRequestRequestTypeDef](./type_defs.md#listdataingestionjobsrequestrequesttypedef) 

### list\_datasets

Lists all datasets currently available in your account, filtering on the
dataset
name.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").list_datasets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_datasets)

```python
# list_datasets method definition

await def list_datasets(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    DatasetNameBeginsWith: str = ...,
) -> ListDatasetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# list_datasets method usage example with argument unpacking

kwargs: ListDatasetsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_datasets(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef) 

### list\_inference\_events

Lists all inference events that have been found for the specified inference
scheduler.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").list_inference_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_inference_events)

```python
# list_inference_events method definition

await def list_inference_events(
    self,
    *,
    InferenceSchedulerName: str,
    IntervalStartTime: TimestampTypeDef,
    IntervalEndTime: TimestampTypeDef,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListInferenceEventsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInferenceEventsResponseTypeDef](./type_defs.md#listinferenceeventsresponsetypedef) 


```python
# list_inference_events method usage example with argument unpacking

kwargs: ListInferenceEventsRequestRequestTypeDef = {  # (1)
    "InferenceSchedulerName": ...,
    "IntervalStartTime": ...,
    "IntervalEndTime": ...,
}

parent.list_inference_events(**kwargs)
```

1. See [:material-code-braces: ListInferenceEventsRequestRequestTypeDef](./type_defs.md#listinferenceeventsrequestrequesttypedef) 

### list\_inference\_executions

Lists all inference executions that have been performed by the specified
inference
scheduler.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").list_inference_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_inference_executions)

```python
# list_inference_executions method definition

await def list_inference_executions(
    self,
    *,
    InferenceSchedulerName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    DataStartTimeAfter: TimestampTypeDef = ...,
    DataEndTimeBefore: TimestampTypeDef = ...,
    Status: InferenceExecutionStatusType = ...,  # (1)
) -> ListInferenceExecutionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: InferenceExecutionStatusType](./literals.md#inferenceexecutionstatustype) 
2. See [:material-code-braces: ListInferenceExecutionsResponseTypeDef](./type_defs.md#listinferenceexecutionsresponsetypedef) 


```python
# list_inference_executions method usage example with argument unpacking

kwargs: ListInferenceExecutionsRequestRequestTypeDef = {  # (1)
    "InferenceSchedulerName": ...,
}

parent.list_inference_executions(**kwargs)
```

1. See [:material-code-braces: ListInferenceExecutionsRequestRequestTypeDef](./type_defs.md#listinferenceexecutionsrequestrequesttypedef) 

### list\_inference\_schedulers

Retrieves a list of all inference schedulers currently available for your
account.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").list_inference_schedulers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_inference_schedulers)

```python
# list_inference_schedulers method definition

await def list_inference_schedulers(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    InferenceSchedulerNameBeginsWith: str = ...,
    ModelName: str = ...,
    Status: InferenceSchedulerStatusType = ...,  # (1)
) -> ListInferenceSchedulersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: InferenceSchedulerStatusType](./literals.md#inferenceschedulerstatustype) 
2. See [:material-code-braces: ListInferenceSchedulersResponseTypeDef](./type_defs.md#listinferenceschedulersresponsetypedef) 


```python
# list_inference_schedulers method usage example with argument unpacking

kwargs: ListInferenceSchedulersRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_inference_schedulers(**kwargs)
```

1. See [:material-code-braces: ListInferenceSchedulersRequestRequestTypeDef](./type_defs.md#listinferenceschedulersrequestrequesttypedef) 

### list\_label\_groups

Returns a list of the label groups.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").list_label_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_label_groups)

```python
# list_label_groups method definition

await def list_label_groups(
    self,
    *,
    LabelGroupNameBeginsWith: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListLabelGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLabelGroupsResponseTypeDef](./type_defs.md#listlabelgroupsresponsetypedef) 


```python
# list_label_groups method usage example with argument unpacking

kwargs: ListLabelGroupsRequestRequestTypeDef = {  # (1)
    "LabelGroupNameBeginsWith": ...,
}

parent.list_label_groups(**kwargs)
```

1. See [:material-code-braces: ListLabelGroupsRequestRequestTypeDef](./type_defs.md#listlabelgroupsrequestrequesttypedef) 

### list\_labels

Provides a list of labels.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").list_labels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_labels)

```python
# list_labels method definition

await def list_labels(
    self,
    *,
    LabelGroupName: str,
    IntervalStartTime: TimestampTypeDef = ...,
    IntervalEndTime: TimestampTypeDef = ...,
    FaultCode: str = ...,
    Equipment: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListLabelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLabelsResponseTypeDef](./type_defs.md#listlabelsresponsetypedef) 


```python
# list_labels method usage example with argument unpacking

kwargs: ListLabelsRequestRequestTypeDef = {  # (1)
    "LabelGroupName": ...,
}

parent.list_labels(**kwargs)
```

1. See [:material-code-braces: ListLabelsRequestRequestTypeDef](./type_defs.md#listlabelsrequestrequesttypedef) 

### list\_model\_versions

Generates a list of all model versions for a given model, including the model
version, model version ARN, and
status.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").list_model_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_model_versions)

```python
# list_model_versions method definition

await def list_model_versions(
    self,
    *,
    ModelName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    Status: ModelVersionStatusType = ...,  # (1)
    SourceType: ModelVersionSourceTypeType = ...,  # (2)
    CreatedAtEndTime: TimestampTypeDef = ...,
    CreatedAtStartTime: TimestampTypeDef = ...,
    MaxModelVersion: int = ...,
    MinModelVersion: int = ...,
) -> ListModelVersionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ModelVersionStatusType](./literals.md#modelversionstatustype) 
2. See [:material-code-brackets: ModelVersionSourceTypeType](./literals.md#modelversionsourcetypetype) 
3. See [:material-code-braces: ListModelVersionsResponseTypeDef](./type_defs.md#listmodelversionsresponsetypedef) 


```python
# list_model_versions method usage example with argument unpacking

kwargs: ListModelVersionsRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
}

parent.list_model_versions(**kwargs)
```

1. See [:material-code-braces: ListModelVersionsRequestRequestTypeDef](./type_defs.md#listmodelversionsrequestrequesttypedef) 

### list\_models

Generates a list of all models in the account, including model name and ARN,
dataset, and
status.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").list_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_models)

```python
# list_models method definition

await def list_models(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Status: ModelStatusType = ...,  # (1)
    ModelNameBeginsWith: str = ...,
    DatasetNameBeginsWith: str = ...,
) -> ListModelsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
2. See [:material-code-braces: ListModelsResponseTypeDef](./type_defs.md#listmodelsresponsetypedef) 


```python
# list_models method usage example with argument unpacking

kwargs: ListModelsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_models(**kwargs)
```

1. See [:material-code-braces: ListModelsRequestRequestTypeDef](./type_defs.md#listmodelsrequestrequesttypedef) 

### list\_retraining\_schedulers

Lists all retraining schedulers in your account, filtering by model name prefix
and
status.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").list_retraining_schedulers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_retraining_schedulers)

```python
# list_retraining_schedulers method definition

await def list_retraining_schedulers(
    self,
    *,
    ModelNameBeginsWith: str = ...,
    Status: RetrainingSchedulerStatusType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListRetrainingSchedulersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RetrainingSchedulerStatusType](./literals.md#retrainingschedulerstatustype) 
2. See [:material-code-braces: ListRetrainingSchedulersResponseTypeDef](./type_defs.md#listretrainingschedulersresponsetypedef) 


```python
# list_retraining_schedulers method usage example with argument unpacking

kwargs: ListRetrainingSchedulersRequestRequestTypeDef = {  # (1)
    "ModelNameBeginsWith": ...,
}

parent.list_retraining_schedulers(**kwargs)
```

1. See [:material-code-braces: ListRetrainingSchedulersRequestRequestTypeDef](./type_defs.md#listretrainingschedulersrequestrequesttypedef) 

### list\_sensor\_statistics

Lists statistics about the data collected for each of the sensors that have
been successfully ingested in the particular
dataset.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").list_sensor_statistics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_sensor_statistics)

```python
# list_sensor_statistics method definition

await def list_sensor_statistics(
    self,
    *,
    DatasetName: str,
    IngestionJobId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListSensorStatisticsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSensorStatisticsResponseTypeDef](./type_defs.md#listsensorstatisticsresponsetypedef) 


```python
# list_sensor_statistics method usage example with argument unpacking

kwargs: ListSensorStatisticsRequestRequestTypeDef = {  # (1)
    "DatasetName": ...,
}

parent.list_sensor_statistics(**kwargs)
```

1. See [:material-code-braces: ListSensorStatisticsRequestRequestTypeDef](./type_defs.md#listsensorstatisticsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists all the tags for a specified resource, including key and value.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_resource\_policy

Creates a resource control policy for a given resource.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").put_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.put_resource_policy)

```python
# put_resource_policy method definition

await def put_resource_policy(
    self,
    *,
    ResourceArn: str,
    ResourcePolicy: str,
    ClientToken: str,
    PolicyRevisionId: str = ...,
) -> PutResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef) 


```python
# put_resource_policy method usage example with argument unpacking

kwargs: PutResourcePolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "ResourcePolicy": ...,
    "ClientToken": ...,
}

parent.put_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef) 

### start\_data\_ingestion\_job

Starts a data ingestion job.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").start_data_ingestion_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.start_data_ingestion_job)

```python
# start_data_ingestion_job method definition

await def start_data_ingestion_job(
    self,
    *,
    DatasetName: str,
    IngestionInputConfiguration: IngestionInputConfigurationTypeDef,  # (1)
    RoleArn: str,
    ClientToken: str,
) -> StartDataIngestionJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IngestionInputConfigurationTypeDef](./type_defs.md#ingestioninputconfigurationtypedef) 
2. See [:material-code-braces: StartDataIngestionJobResponseTypeDef](./type_defs.md#startdataingestionjobresponsetypedef) 


```python
# start_data_ingestion_job method usage example with argument unpacking

kwargs: StartDataIngestionJobRequestRequestTypeDef = {  # (1)
    "DatasetName": ...,
    "IngestionInputConfiguration": ...,
    "RoleArn": ...,
    "ClientToken": ...,
}

parent.start_data_ingestion_job(**kwargs)
```

1. See [:material-code-braces: StartDataIngestionJobRequestRequestTypeDef](./type_defs.md#startdataingestionjobrequestrequesttypedef) 

### start\_inference\_scheduler

Starts an inference scheduler.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").start_inference_scheduler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.start_inference_scheduler)

```python
# start_inference_scheduler method definition

await def start_inference_scheduler(
    self,
    *,
    InferenceSchedulerName: str,
) -> StartInferenceSchedulerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartInferenceSchedulerResponseTypeDef](./type_defs.md#startinferenceschedulerresponsetypedef) 


```python
# start_inference_scheduler method usage example with argument unpacking

kwargs: StartInferenceSchedulerRequestRequestTypeDef = {  # (1)
    "InferenceSchedulerName": ...,
}

parent.start_inference_scheduler(**kwargs)
```

1. See [:material-code-braces: StartInferenceSchedulerRequestRequestTypeDef](./type_defs.md#startinferenceschedulerrequestrequesttypedef) 

### start\_retraining\_scheduler

Starts a retraining scheduler.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").start_retraining_scheduler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.start_retraining_scheduler)

```python
# start_retraining_scheduler method definition

await def start_retraining_scheduler(
    self,
    *,
    ModelName: str,
) -> StartRetrainingSchedulerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartRetrainingSchedulerResponseTypeDef](./type_defs.md#startretrainingschedulerresponsetypedef) 


```python
# start_retraining_scheduler method usage example with argument unpacking

kwargs: StartRetrainingSchedulerRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
}

parent.start_retraining_scheduler(**kwargs)
```

1. See [:material-code-braces: StartRetrainingSchedulerRequestRequestTypeDef](./type_defs.md#startretrainingschedulerrequestrequesttypedef) 

### stop\_inference\_scheduler

Stops an inference scheduler.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").stop_inference_scheduler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.stop_inference_scheduler)

```python
# stop_inference_scheduler method definition

await def stop_inference_scheduler(
    self,
    *,
    InferenceSchedulerName: str,
) -> StopInferenceSchedulerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopInferenceSchedulerResponseTypeDef](./type_defs.md#stopinferenceschedulerresponsetypedef) 


```python
# stop_inference_scheduler method usage example with argument unpacking

kwargs: StopInferenceSchedulerRequestRequestTypeDef = {  # (1)
    "InferenceSchedulerName": ...,
}

parent.stop_inference_scheduler(**kwargs)
```

1. See [:material-code-braces: StopInferenceSchedulerRequestRequestTypeDef](./type_defs.md#stopinferenceschedulerrequestrequesttypedef) 

### stop\_retraining\_scheduler

Stops a retraining scheduler.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").stop_retraining_scheduler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.stop_retraining_scheduler)

```python
# stop_retraining_scheduler method definition

await def stop_retraining_scheduler(
    self,
    *,
    ModelName: str,
) -> StopRetrainingSchedulerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopRetrainingSchedulerResponseTypeDef](./type_defs.md#stopretrainingschedulerresponsetypedef) 


```python
# stop_retraining_scheduler method usage example with argument unpacking

kwargs: StopRetrainingSchedulerRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
}

parent.stop_retraining_scheduler(**kwargs)
```

1. See [:material-code-braces: StopRetrainingSchedulerRequestRequestTypeDef](./type_defs.md#stopretrainingschedulerrequestrequesttypedef) 

### tag\_resource

Associates a given tag to a resource in your account.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes a specific tag from a given resource.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_active\_model\_version

Sets the active model version for a given machine learning model.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").update_active_model_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.update_active_model_version)

```python
# update_active_model_version method definition

await def update_active_model_version(
    self,
    *,
    ModelName: str,
    ModelVersion: int,
) -> UpdateActiveModelVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateActiveModelVersionResponseTypeDef](./type_defs.md#updateactivemodelversionresponsetypedef) 


```python
# update_active_model_version method usage example with argument unpacking

kwargs: UpdateActiveModelVersionRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
    "ModelVersion": ...,
}

parent.update_active_model_version(**kwargs)
```

1. See [:material-code-braces: UpdateActiveModelVersionRequestRequestTypeDef](./type_defs.md#updateactivemodelversionrequestrequesttypedef) 

### update\_inference\_scheduler

Updates an inference scheduler.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").update_inference_scheduler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.update_inference_scheduler)

```python
# update_inference_scheduler method definition

await def update_inference_scheduler(
    self,
    *,
    InferenceSchedulerName: str,
    DataDelayOffsetInMinutes: int = ...,
    DataUploadFrequency: DataUploadFrequencyType = ...,  # (1)
    DataInputConfiguration: InferenceInputConfigurationTypeDef = ...,  # (2)
    DataOutputConfiguration: InferenceOutputConfigurationTypeDef = ...,  # (3)
    RoleArn: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: DataUploadFrequencyType](./literals.md#datauploadfrequencytype) 
2. See [:material-code-braces: InferenceInputConfigurationTypeDef](./type_defs.md#inferenceinputconfigurationtypedef) 
3. See [:material-code-braces: InferenceOutputConfigurationTypeDef](./type_defs.md#inferenceoutputconfigurationtypedef) 
4. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_inference_scheduler method usage example with argument unpacking

kwargs: UpdateInferenceSchedulerRequestRequestTypeDef = {  # (1)
    "InferenceSchedulerName": ...,
}

parent.update_inference_scheduler(**kwargs)
```

1. See [:material-code-braces: UpdateInferenceSchedulerRequestRequestTypeDef](./type_defs.md#updateinferenceschedulerrequestrequesttypedef) 

### update\_label\_group

Updates the label group.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").update_label_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.update_label_group)

```python
# update_label_group method definition

await def update_label_group(
    self,
    *,
    LabelGroupName: str,
    FaultCodes: Sequence[str] = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_label_group method usage example with argument unpacking

kwargs: UpdateLabelGroupRequestRequestTypeDef = {  # (1)
    "LabelGroupName": ...,
}

parent.update_label_group(**kwargs)
```

1. See [:material-code-braces: UpdateLabelGroupRequestRequestTypeDef](./type_defs.md#updatelabelgrouprequestrequesttypedef) 

### update\_model

Updates a model in the account.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").update_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.update_model)

```python
# update_model method definition

await def update_model(
    self,
    *,
    ModelName: str,
    LabelsInputConfiguration: LabelsInputConfigurationTypeDef = ...,  # (1)
    RoleArn: str = ...,
    ModelDiagnosticsOutputConfiguration: ModelDiagnosticsOutputConfigurationTypeDef = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LabelsInputConfigurationTypeDef](./type_defs.md#labelsinputconfigurationtypedef) 
2. See [:material-code-braces: ModelDiagnosticsOutputConfigurationTypeDef](./type_defs.md#modeldiagnosticsoutputconfigurationtypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_model method usage example with argument unpacking

kwargs: UpdateModelRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
}

parent.update_model(**kwargs)
```

1. See [:material-code-braces: UpdateModelRequestRequestTypeDef](./type_defs.md#updatemodelrequestrequesttypedef) 

### update\_retraining\_scheduler

Updates a retraining scheduler.

Type annotations and code completion for `#!python session.create_client("lookoutequipment").update_retraining_scheduler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.update_retraining_scheduler)

```python
# update_retraining_scheduler method definition

await def update_retraining_scheduler(
    self,
    *,
    ModelName: str,
    RetrainingStartDate: TimestampTypeDef = ...,
    RetrainingFrequency: str = ...,
    LookbackWindow: str = ...,
    PromoteMode: ModelPromoteModeType = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ModelPromoteModeType](./literals.md#modelpromotemodetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_retraining_scheduler method usage example with argument unpacking

kwargs: UpdateRetrainingSchedulerRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
}

parent.update_retraining_scheduler(**kwargs)
```

1. See [:material-code-braces: UpdateRetrainingSchedulerRequestRequestTypeDef](./type_defs.md#updateretrainingschedulerrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("lookoutequipment").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "LookoutEquipmentClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("lookoutequipment").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.__aexit__)

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





