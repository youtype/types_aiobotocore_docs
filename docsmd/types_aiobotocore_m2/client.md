# MainframeModernizationClient

> [Index](../README.md) > [MainframeModernization](./README.md) > MainframeModernizationClient

!!! note ""

    Auto-generated documentation for [MainframeModernization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
    type annotations stubs module [types-aiobotocore-m2](https://pypi.org/project/types-aiobotocore-m2/).

## MainframeModernizationClient

Type annotations and code completion for `#!python session.create_client("m2")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client)

```python
# MainframeModernizationClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_m2.client import MainframeModernizationClient

session = get_session()
async with session.create_client("m2") as client:
    client: MainframeModernizationClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("m2").exceptions` structure.

```python
# MainframeModernizationClient.exceptions usage example

async with session.create_client("m2") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.ExecutionTimeoutException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# MainframeModernizationClient usage type checking example

from types_aiobotocore_m2.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("m2").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_batch\_job\_execution

Cancels the running of a specific batch job execution.

Type annotations and code completion for `#!python session.create_client("m2").cancel_batch_job_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.cancel_batch_job_execution)

```python
# cancel_batch_job_execution method definition

await def cancel_batch_job_execution(
    self,
    *,
    applicationId: str,
    executionId: str,
    authSecretsManagerArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_batch_job_execution method usage example with argument unpacking

kwargs: CancelBatchJobExecutionRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "executionId": ...,
}

parent.cancel_batch_job_execution(**kwargs)
```

1. See [:material-code-braces: CancelBatchJobExecutionRequestRequestTypeDef](./type_defs.md#cancelbatchjobexecutionrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("m2").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_application

Creates a new application with given parameters.

Type annotations and code completion for `#!python session.create_client("m2").create_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_application)

```python
# create_application method definition

await def create_application(
    self,
    *,
    definition: DefinitionTypeDef,  # (1)
    engineType: EngineTypeType,  # (2)
    name: str,
    clientToken: str = ...,
    description: str = ...,
    kmsKeyId: str = ...,
    roleArn: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateApplicationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DefinitionTypeDef](./type_defs.md#definitiontypedef) 
2. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
3. See [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 


```python
# create_application method usage example with argument unpacking

kwargs: CreateApplicationRequestRequestTypeDef = {  # (1)
    "definition": ...,
    "engineType": ...,
    "name": ...,
}

parent.create_application(**kwargs)
```

1. See [:material-code-braces: CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef) 

### create\_data\_set\_import\_task

Starts a data set import task for a specific application.

Type annotations and code completion for `#!python session.create_client("m2").create_data_set_import_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_data_set_import_task)

```python
# create_data_set_import_task method definition

await def create_data_set_import_task(
    self,
    *,
    applicationId: str,
    importConfig: DataSetImportConfigTypeDef,  # (1)
    clientToken: str = ...,
) -> CreateDataSetImportTaskResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataSetImportConfigTypeDef](./type_defs.md#datasetimportconfigtypedef) 
2. See [:material-code-braces: CreateDataSetImportTaskResponseTypeDef](./type_defs.md#createdatasetimporttaskresponsetypedef) 


```python
# create_data_set_import_task method usage example with argument unpacking

kwargs: CreateDataSetImportTaskRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "importConfig": ...,
}

parent.create_data_set_import_task(**kwargs)
```

1. See [:material-code-braces: CreateDataSetImportTaskRequestRequestTypeDef](./type_defs.md#createdatasetimporttaskrequestrequesttypedef) 

### create\_deployment

Creates and starts a deployment to deploy an application into a runtime
environment.

Type annotations and code completion for `#!python session.create_client("m2").create_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_deployment)

```python
# create_deployment method definition

await def create_deployment(
    self,
    *,
    applicationId: str,
    applicationVersion: int,
    environmentId: str,
    clientToken: str = ...,
) -> CreateDeploymentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateDeploymentResponseTypeDef](./type_defs.md#createdeploymentresponsetypedef) 


```python
# create_deployment method usage example with argument unpacking

kwargs: CreateDeploymentRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "applicationVersion": ...,
    "environmentId": ...,
}

parent.create_deployment(**kwargs)
```

1. See [:material-code-braces: CreateDeploymentRequestRequestTypeDef](./type_defs.md#createdeploymentrequestrequesttypedef) 

### create\_environment

Creates a runtime environment for a given runtime engine.

Type annotations and code completion for `#!python session.create_client("m2").create_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_environment)

```python
# create_environment method definition

await def create_environment(
    self,
    *,
    engineType: EngineTypeType,  # (1)
    instanceType: str,
    name: str,
    clientToken: str = ...,
    description: str = ...,
    engineVersion: str = ...,
    highAvailabilityConfig: HighAvailabilityConfigTypeDef = ...,  # (2)
    kmsKeyId: str = ...,
    preferredMaintenanceWindow: str = ...,
    publiclyAccessible: bool = ...,
    securityGroupIds: Sequence[str] = ...,
    storageConfigurations: Sequence[StorageConfigurationTypeDef] = ...,  # (3)
    subnetIds: Sequence[str] = ...,
    tags: Mapping[str, str] = ...,
) -> CreateEnvironmentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-braces: HighAvailabilityConfigTypeDef](./type_defs.md#highavailabilityconfigtypedef) 
3. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
4. See [:material-code-braces: CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef) 


```python
# create_environment method usage example with argument unpacking

kwargs: CreateEnvironmentRequestRequestTypeDef = {  # (1)
    "engineType": ...,
    "instanceType": ...,
    "name": ...,
}

parent.create_environment(**kwargs)
```

1. See [:material-code-braces: CreateEnvironmentRequestRequestTypeDef](./type_defs.md#createenvironmentrequestrequesttypedef) 

### delete\_application

Deletes a specific application.

Type annotations and code completion for `#!python session.create_client("m2").delete_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.delete_application)

```python
# delete_application method definition

await def delete_application(
    self,
    *,
    applicationId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_application method usage example with argument unpacking

kwargs: DeleteApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.delete_application(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef) 

### delete\_application\_from\_environment

Deletes a specific application from the specific runtime environment where it
was previously
deployed.

Type annotations and code completion for `#!python session.create_client("m2").delete_application_from_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.delete_application_from_environment)

```python
# delete_application_from_environment method definition

await def delete_application_from_environment(
    self,
    *,
    applicationId: str,
    environmentId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_application_from_environment method usage example with argument unpacking

kwargs: DeleteApplicationFromEnvironmentRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "environmentId": ...,
}

parent.delete_application_from_environment(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationFromEnvironmentRequestRequestTypeDef](./type_defs.md#deleteapplicationfromenvironmentrequestrequesttypedef) 

### delete\_environment

Deletes a specific runtime environment.

Type annotations and code completion for `#!python session.create_client("m2").delete_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.delete_environment)

```python
# delete_environment method definition

await def delete_environment(
    self,
    *,
    environmentId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_environment method usage example with argument unpacking

kwargs: DeleteEnvironmentRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.delete_environment(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentRequestRequestTypeDef](./type_defs.md#deleteenvironmentrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("m2").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.generate_presigned_url)

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


### get\_application

Describes the details of a specific application.

Type annotations and code completion for `#!python session.create_client("m2").get_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_application)

```python
# get_application method definition

await def get_application(
    self,
    *,
    applicationId: str,
) -> GetApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApplicationResponseTypeDef](./type_defs.md#getapplicationresponsetypedef) 


```python
# get_application method usage example with argument unpacking

kwargs: GetApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.get_application(**kwargs)
```

1. See [:material-code-braces: GetApplicationRequestRequestTypeDef](./type_defs.md#getapplicationrequestrequesttypedef) 

### get\_application\_version

Returns details about a specific version of a specific application.

Type annotations and code completion for `#!python session.create_client("m2").get_application_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_application_version)

```python
# get_application_version method definition

await def get_application_version(
    self,
    *,
    applicationId: str,
    applicationVersion: int,
) -> GetApplicationVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApplicationVersionResponseTypeDef](./type_defs.md#getapplicationversionresponsetypedef) 


```python
# get_application_version method usage example with argument unpacking

kwargs: GetApplicationVersionRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "applicationVersion": ...,
}

parent.get_application_version(**kwargs)
```

1. See [:material-code-braces: GetApplicationVersionRequestRequestTypeDef](./type_defs.md#getapplicationversionrequestrequesttypedef) 

### get\_batch\_job\_execution

Gets the details of a specific batch job execution for a specific application.

Type annotations and code completion for `#!python session.create_client("m2").get_batch_job_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_batch_job_execution)

```python
# get_batch_job_execution method definition

await def get_batch_job_execution(
    self,
    *,
    applicationId: str,
    executionId: str,
) -> GetBatchJobExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBatchJobExecutionResponseTypeDef](./type_defs.md#getbatchjobexecutionresponsetypedef) 


```python
# get_batch_job_execution method usage example with argument unpacking

kwargs: GetBatchJobExecutionRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "executionId": ...,
}

parent.get_batch_job_execution(**kwargs)
```

1. See [:material-code-braces: GetBatchJobExecutionRequestRequestTypeDef](./type_defs.md#getbatchjobexecutionrequestrequesttypedef) 

### get\_data\_set\_details

Gets the details of a specific data set.

Type annotations and code completion for `#!python session.create_client("m2").get_data_set_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_data_set_details)

```python
# get_data_set_details method definition

await def get_data_set_details(
    self,
    *,
    applicationId: str,
    dataSetName: str,
) -> GetDataSetDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataSetDetailsResponseTypeDef](./type_defs.md#getdatasetdetailsresponsetypedef) 


```python
# get_data_set_details method usage example with argument unpacking

kwargs: GetDataSetDetailsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "dataSetName": ...,
}

parent.get_data_set_details(**kwargs)
```

1. See [:material-code-braces: GetDataSetDetailsRequestRequestTypeDef](./type_defs.md#getdatasetdetailsrequestrequesttypedef) 

### get\_data\_set\_import\_task

Gets the status of a data set import task initiated with the
CreateDataSetImportTask
operation.

Type annotations and code completion for `#!python session.create_client("m2").get_data_set_import_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_data_set_import_task)

```python
# get_data_set_import_task method definition

await def get_data_set_import_task(
    self,
    *,
    applicationId: str,
    taskId: str,
) -> GetDataSetImportTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataSetImportTaskResponseTypeDef](./type_defs.md#getdatasetimporttaskresponsetypedef) 


```python
# get_data_set_import_task method usage example with argument unpacking

kwargs: GetDataSetImportTaskRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "taskId": ...,
}

parent.get_data_set_import_task(**kwargs)
```

1. See [:material-code-braces: GetDataSetImportTaskRequestRequestTypeDef](./type_defs.md#getdatasetimporttaskrequestrequesttypedef) 

### get\_deployment

Gets details of a specific deployment with a given deployment identifier.

Type annotations and code completion for `#!python session.create_client("m2").get_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_deployment)

```python
# get_deployment method definition

await def get_deployment(
    self,
    *,
    applicationId: str,
    deploymentId: str,
) -> GetDeploymentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeploymentResponseTypeDef](./type_defs.md#getdeploymentresponsetypedef) 


```python
# get_deployment method usage example with argument unpacking

kwargs: GetDeploymentRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "deploymentId": ...,
}

parent.get_deployment(**kwargs)
```

1. See [:material-code-braces: GetDeploymentRequestRequestTypeDef](./type_defs.md#getdeploymentrequestrequesttypedef) 

### get\_environment

Describes a specific runtime environment.

Type annotations and code completion for `#!python session.create_client("m2").get_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_environment)

```python
# get_environment method definition

await def get_environment(
    self,
    *,
    environmentId: str,
) -> GetEnvironmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnvironmentResponseTypeDef](./type_defs.md#getenvironmentresponsetypedef) 


```python
# get_environment method usage example with argument unpacking

kwargs: GetEnvironmentRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.get_environment(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentRequestRequestTypeDef](./type_defs.md#getenvironmentrequestrequesttypedef) 

### get\_signed\_bluinsights\_url

Gets a single sign-on URL that can be used to connect to AWS Blu Insights.

Type annotations and code completion for `#!python session.create_client("m2").get_signed_bluinsights_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_signed_bluinsights_url)

```python
# get_signed_bluinsights_url method definition

await def get_signed_bluinsights_url(
    self,
) -> GetSignedBluinsightsUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSignedBluinsightsUrlResponseTypeDef](./type_defs.md#getsignedbluinsightsurlresponsetypedef) 

### list\_application\_versions

Returns a list of the application versions for a specific application.

Type annotations and code completion for `#!python session.create_client("m2").list_application_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_application_versions)

```python
# list_application_versions method definition

await def list_application_versions(
    self,
    *,
    applicationId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListApplicationVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationVersionsResponseTypeDef](./type_defs.md#listapplicationversionsresponsetypedef) 


```python
# list_application_versions method usage example with argument unpacking

kwargs: ListApplicationVersionsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_application_versions(**kwargs)
```

1. See [:material-code-braces: ListApplicationVersionsRequestRequestTypeDef](./type_defs.md#listapplicationversionsrequestrequesttypedef) 

### list\_applications

Lists the applications associated with a specific Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("m2").list_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_applications)

```python
# list_applications method definition

await def list_applications(
    self,
    *,
    environmentId: str = ...,
    maxResults: int = ...,
    names: Sequence[str] = ...,
    nextToken: str = ...,
) -> ListApplicationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python
# list_applications method usage example with argument unpacking

kwargs: ListApplicationsRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.list_applications(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef) 

### list\_batch\_job\_definitions

Lists all the available batch job definitions based on the batch job resources
uploaded during the application
creation.

Type annotations and code completion for `#!python session.create_client("m2").list_batch_job_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_batch_job_definitions)

```python
# list_batch_job_definitions method definition

await def list_batch_job_definitions(
    self,
    *,
    applicationId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    prefix: str = ...,
) -> ListBatchJobDefinitionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBatchJobDefinitionsResponseTypeDef](./type_defs.md#listbatchjobdefinitionsresponsetypedef) 


```python
# list_batch_job_definitions method usage example with argument unpacking

kwargs: ListBatchJobDefinitionsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_batch_job_definitions(**kwargs)
```

1. See [:material-code-braces: ListBatchJobDefinitionsRequestRequestTypeDef](./type_defs.md#listbatchjobdefinitionsrequestrequesttypedef) 

### list\_batch\_job\_executions

Lists historical, current, and scheduled batch job executions for a specific
application.

Type annotations and code completion for `#!python session.create_client("m2").list_batch_job_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_batch_job_executions)

```python
# list_batch_job_executions method definition

await def list_batch_job_executions(
    self,
    *,
    applicationId: str,
    executionIds: Sequence[str] = ...,
    jobName: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    startedAfter: TimestampTypeDef = ...,
    startedBefore: TimestampTypeDef = ...,
    status: BatchJobExecutionStatusType = ...,  # (1)
) -> ListBatchJobExecutionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: BatchJobExecutionStatusType](./literals.md#batchjobexecutionstatustype) 
2. See [:material-code-braces: ListBatchJobExecutionsResponseTypeDef](./type_defs.md#listbatchjobexecutionsresponsetypedef) 


```python
# list_batch_job_executions method usage example with argument unpacking

kwargs: ListBatchJobExecutionsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_batch_job_executions(**kwargs)
```

1. See [:material-code-braces: ListBatchJobExecutionsRequestRequestTypeDef](./type_defs.md#listbatchjobexecutionsrequestrequesttypedef) 

### list\_batch\_job\_restart\_points

Lists all the job steps for a JCL file to restart a batch job.

Type annotations and code completion for `#!python session.create_client("m2").list_batch_job_restart_points` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_batch_job_restart_points)

```python
# list_batch_job_restart_points method definition

await def list_batch_job_restart_points(
    self,
    *,
    applicationId: str,
    executionId: str,
    authSecretsManagerArn: str = ...,
) -> ListBatchJobRestartPointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBatchJobRestartPointsResponseTypeDef](./type_defs.md#listbatchjobrestartpointsresponsetypedef) 


```python
# list_batch_job_restart_points method usage example with argument unpacking

kwargs: ListBatchJobRestartPointsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "executionId": ...,
}

parent.list_batch_job_restart_points(**kwargs)
```

1. See [:material-code-braces: ListBatchJobRestartPointsRequestRequestTypeDef](./type_defs.md#listbatchjobrestartpointsrequestrequesttypedef) 

### list\_data\_set\_import\_history

Lists the data set imports for the specified application.

Type annotations and code completion for `#!python session.create_client("m2").list_data_set_import_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_data_set_import_history)

```python
# list_data_set_import_history method definition

await def list_data_set_import_history(
    self,
    *,
    applicationId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDataSetImportHistoryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataSetImportHistoryResponseTypeDef](./type_defs.md#listdatasetimporthistoryresponsetypedef) 


```python
# list_data_set_import_history method usage example with argument unpacking

kwargs: ListDataSetImportHistoryRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_data_set_import_history(**kwargs)
```

1. See [:material-code-braces: ListDataSetImportHistoryRequestRequestTypeDef](./type_defs.md#listdatasetimporthistoryrequestrequesttypedef) 

### list\_data\_sets

Lists the data sets imported for a specific application.

Type annotations and code completion for `#!python session.create_client("m2").list_data_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_data_sets)

```python
# list_data_sets method definition

await def list_data_sets(
    self,
    *,
    applicationId: str,
    maxResults: int = ...,
    nameFilter: str = ...,
    nextToken: str = ...,
    prefix: str = ...,
) -> ListDataSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataSetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# list_data_sets method usage example with argument unpacking

kwargs: ListDataSetsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_data_sets(**kwargs)
```

1. See [:material-code-braces: ListDataSetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef) 

### list\_deployments

Returns a list of all deployments of a specific application.

Type annotations and code completion for `#!python session.create_client("m2").list_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_deployments)

```python
# list_deployments method definition

await def list_deployments(
    self,
    *,
    applicationId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDeploymentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDeploymentsResponseTypeDef](./type_defs.md#listdeploymentsresponsetypedef) 


```python
# list_deployments method usage example with argument unpacking

kwargs: ListDeploymentsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_deployments(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsRequestRequestTypeDef](./type_defs.md#listdeploymentsrequestrequesttypedef) 

### list\_engine\_versions

Lists the available engine versions.

Type annotations and code completion for `#!python session.create_client("m2").list_engine_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_engine_versions)

```python
# list_engine_versions method definition

await def list_engine_versions(
    self,
    *,
    engineType: EngineTypeType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListEngineVersionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-braces: ListEngineVersionsResponseTypeDef](./type_defs.md#listengineversionsresponsetypedef) 


```python
# list_engine_versions method usage example with argument unpacking

kwargs: ListEngineVersionsRequestRequestTypeDef = {  # (1)
    "engineType": ...,
}

parent.list_engine_versions(**kwargs)
```

1. See [:material-code-braces: ListEngineVersionsRequestRequestTypeDef](./type_defs.md#listengineversionsrequestrequesttypedef) 

### list\_environments

Lists the runtime environments.

Type annotations and code completion for `#!python session.create_client("m2").list_environments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_environments)

```python
# list_environments method definition

await def list_environments(
    self,
    *,
    engineType: EngineTypeType = ...,  # (1)
    maxResults: int = ...,
    names: Sequence[str] = ...,
    nextToken: str = ...,
) -> ListEnvironmentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-braces: ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef) 


```python
# list_environments method usage example with argument unpacking

kwargs: ListEnvironmentsRequestRequestTypeDef = {  # (1)
    "engineType": ...,
}

parent.list_environments(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsRequestRequestTypeDef](./type_defs.md#listenvironmentsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("m2").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_tags_for_resource)

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

### start\_application

Starts an application that is currently stopped.

Type annotations and code completion for `#!python session.create_client("m2").start_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.start_application)

```python
# start_application method definition

await def start_application(
    self,
    *,
    applicationId: str,
) -> Dict[str, Any]:
    ...
```



```python
# start_application method usage example with argument unpacking

kwargs: StartApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.start_application(**kwargs)
```

1. See [:material-code-braces: StartApplicationRequestRequestTypeDef](./type_defs.md#startapplicationrequestrequesttypedef) 

### start\_batch\_job

Starts a batch job and returns the unique identifier of this execution of the
batch
job.

Type annotations and code completion for `#!python session.create_client("m2").start_batch_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.start_batch_job)

```python
# start_batch_job method definition

await def start_batch_job(
    self,
    *,
    applicationId: str,
    batchJobIdentifier: BatchJobIdentifierTypeDef,  # (1)
    authSecretsManagerArn: str = ...,
    jobParams: Mapping[str, str] = ...,
) -> StartBatchJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchJobIdentifierTypeDef](./type_defs.md#batchjobidentifiertypedef) 
2. See [:material-code-braces: StartBatchJobResponseTypeDef](./type_defs.md#startbatchjobresponsetypedef) 


```python
# start_batch_job method usage example with argument unpacking

kwargs: StartBatchJobRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "batchJobIdentifier": ...,
}

parent.start_batch_job(**kwargs)
```

1. See [:material-code-braces: StartBatchJobRequestRequestTypeDef](./type_defs.md#startbatchjobrequestrequesttypedef) 

### stop\_application

Stops a running application.

Type annotations and code completion for `#!python session.create_client("m2").stop_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.stop_application)

```python
# stop_application method definition

await def stop_application(
    self,
    *,
    applicationId: str,
    forceStop: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# stop_application method usage example with argument unpacking

kwargs: StopApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.stop_application(**kwargs)
```

1. See [:material-code-braces: StopApplicationRequestRequestTypeDef](./type_defs.md#stopapplicationrequestrequesttypedef) 

### tag\_resource

Adds one or more tags to the specified resource.

Type annotations and code completion for `#!python session.create_client("m2").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.tag_resource)

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

Removes one or more tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("m2").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.untag_resource)

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

### update\_application

Updates an application and creates a new version.

Type annotations and code completion for `#!python session.create_client("m2").update_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.update_application)

```python
# update_application method definition

await def update_application(
    self,
    *,
    applicationId: str,
    currentApplicationVersion: int,
    definition: DefinitionTypeDef = ...,  # (1)
    description: str = ...,
) -> UpdateApplicationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DefinitionTypeDef](./type_defs.md#definitiontypedef) 
2. See [:material-code-braces: UpdateApplicationResponseTypeDef](./type_defs.md#updateapplicationresponsetypedef) 


```python
# update_application method usage example with argument unpacking

kwargs: UpdateApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "currentApplicationVersion": ...,
}

parent.update_application(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef) 

### update\_environment

Updates the configuration details for a specific runtime environment.

Type annotations and code completion for `#!python session.create_client("m2").update_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.update_environment)

```python
# update_environment method definition

await def update_environment(
    self,
    *,
    environmentId: str,
    applyDuringMaintenanceWindow: bool = ...,
    desiredCapacity: int = ...,
    engineVersion: str = ...,
    forceUpdate: bool = ...,
    instanceType: str = ...,
    preferredMaintenanceWindow: str = ...,
) -> UpdateEnvironmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateEnvironmentResponseTypeDef](./type_defs.md#updateenvironmentresponsetypedef) 


```python
# update_environment method usage example with argument unpacking

kwargs: UpdateEnvironmentRequestRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.update_environment(**kwargs)
```

1. See [:material-code-braces: UpdateEnvironmentRequestRequestTypeDef](./type_defs.md#updateenvironmentrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("m2").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "MainframeModernizationClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("m2").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("m2").get_paginator` method with overloads.

- `client.get_paginator("list_application_versions")` -> [ListApplicationVersionsPaginator](./paginators.md#listapplicationversionspaginator)
- `client.get_paginator("list_applications")` -> [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- `client.get_paginator("list_batch_job_definitions")` -> [ListBatchJobDefinitionsPaginator](./paginators.md#listbatchjobdefinitionspaginator)
- `client.get_paginator("list_batch_job_executions")` -> [ListBatchJobExecutionsPaginator](./paginators.md#listbatchjobexecutionspaginator)
- `client.get_paginator("list_data_set_import_history")` -> [ListDataSetImportHistoryPaginator](./paginators.md#listdatasetimporthistorypaginator)
- `client.get_paginator("list_data_sets")` -> [ListDataSetsPaginator](./paginators.md#listdatasetspaginator)
- `client.get_paginator("list_deployments")` -> [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
- `client.get_paginator("list_engine_versions")` -> [ListEngineVersionsPaginator](./paginators.md#listengineversionspaginator)
- `client.get_paginator("list_environments")` -> [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)



