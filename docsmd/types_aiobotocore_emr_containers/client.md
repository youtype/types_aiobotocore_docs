# EMRContainersClient

> [Index](../README.md) > [EMRContainers](./README.md) > EMRContainersClient

!!! note ""

    Auto-generated documentation for [EMRContainers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
    type annotations stubs module [types-aiobotocore-emr-containers](https://pypi.org/project/types-aiobotocore-emr-containers/).

## EMRContainersClient

Type annotations and code completion for `#!python session.create_client("emr-containers")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client)

```python
EMRContainersClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_emr_containers.client import EMRContainersClient

session = get_session()
async with session.create_client("emr-containers") as client:
    client: EMRContainersClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("emr-containers").exceptions` structure.

```python
EMRContainersClient.exceptions usage example

async with session.create_client("emr-containers") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalServerException,
        client.RequestThrottledException,
        client.ResourceNotFoundException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
EMRContainersClient usage type checking example

from types_aiobotocore_emr_containers.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("emr-containers").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_job\_run

Cancels a job run.

Type annotations and code completion for `#!python session.create_client("emr-containers").cancel_job_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.cancel_job_run)

```python
# cancel_job_run method definition

await def cancel_job_run(
    self,
    *,
    id: str,
    virtualClusterId: str,
) -> CancelJobRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelJobRunResponseTypeDef](./type_defs.md#canceljobrunresponsetypedef) 


```python
# cancel_job_run method usage example with argument unpacking

kwargs: CancelJobRunRequestRequestTypeDef = {  # (1)
    "id": ...,
    "virtualClusterId": ...,
}

parent.cancel_job_run(**kwargs)
```

1. See [:material-code-braces: CancelJobRunRequestRequestTypeDef](./type_defs.md#canceljobrunrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("emr-containers").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_job\_template

Creates a job template.

Type annotations and code completion for `#!python session.create_client("emr-containers").create_job_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_job_template)

```python
# create_job_template method definition

await def create_job_template(
    self,
    *,
    name: str,
    clientToken: str,
    jobTemplateData: JobTemplateDataTypeDef,  # (1)
    tags: Mapping[str, str] = ...,
    kmsKeyArn: str = ...,
) -> CreateJobTemplateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: JobTemplateDataTypeDef](./type_defs.md#jobtemplatedatatypedef) 
2. See [:material-code-braces: CreateJobTemplateResponseTypeDef](./type_defs.md#createjobtemplateresponsetypedef) 


```python
# create_job_template method usage example with argument unpacking

kwargs: CreateJobTemplateRequestRequestTypeDef = {  # (1)
    "name": ...,
    "clientToken": ...,
    "jobTemplateData": ...,
}

parent.create_job_template(**kwargs)
```

1. See [:material-code-braces: CreateJobTemplateRequestRequestTypeDef](./type_defs.md#createjobtemplaterequestrequesttypedef) 

### create\_managed\_endpoint

Creates a managed endpoint.

Type annotations and code completion for `#!python session.create_client("emr-containers").create_managed_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_managed_endpoint)

```python
# create_managed_endpoint method definition

await def create_managed_endpoint(
    self,
    *,
    name: str,
    virtualClusterId: str,
    type: str,
    releaseLabel: str,
    executionRoleArn: str,
    clientToken: str,
    certificateArn: str = ...,
    configurationOverrides: ConfigurationOverridesTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateManagedEndpointResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConfigurationOverridesTypeDef](./type_defs.md#configurationoverridestypedef) 
2. See [:material-code-braces: CreateManagedEndpointResponseTypeDef](./type_defs.md#createmanagedendpointresponsetypedef) 


```python
# create_managed_endpoint method usage example with argument unpacking

kwargs: CreateManagedEndpointRequestRequestTypeDef = {  # (1)
    "name": ...,
    "virtualClusterId": ...,
    "type": ...,
    "releaseLabel": ...,
    "executionRoleArn": ...,
    "clientToken": ...,
}

parent.create_managed_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateManagedEndpointRequestRequestTypeDef](./type_defs.md#createmanagedendpointrequestrequesttypedef) 

### create\_virtual\_cluster

Creates a virtual cluster.

Type annotations and code completion for `#!python session.create_client("emr-containers").create_virtual_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_virtual_cluster)

```python
# create_virtual_cluster method definition

await def create_virtual_cluster(
    self,
    *,
    name: str,
    containerProvider: ContainerProviderTypeDef,  # (1)
    clientToken: str,
    tags: Mapping[str, str] = ...,
) -> CreateVirtualClusterResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ContainerProviderTypeDef](./type_defs.md#containerprovidertypedef) 
2. See [:material-code-braces: CreateVirtualClusterResponseTypeDef](./type_defs.md#createvirtualclusterresponsetypedef) 


```python
# create_virtual_cluster method usage example with argument unpacking

kwargs: CreateVirtualClusterRequestRequestTypeDef = {  # (1)
    "name": ...,
    "containerProvider": ...,
    "clientToken": ...,
}

parent.create_virtual_cluster(**kwargs)
```

1. See [:material-code-braces: CreateVirtualClusterRequestRequestTypeDef](./type_defs.md#createvirtualclusterrequestrequesttypedef) 

### delete\_job\_template

Deletes a job template.

Type annotations and code completion for `#!python session.create_client("emr-containers").delete_job_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.delete_job_template)

```python
# delete_job_template method definition

await def delete_job_template(
    self,
    *,
    id: str,
) -> DeleteJobTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteJobTemplateResponseTypeDef](./type_defs.md#deletejobtemplateresponsetypedef) 


```python
# delete_job_template method usage example with argument unpacking

kwargs: DeleteJobTemplateRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_job_template(**kwargs)
```

1. See [:material-code-braces: DeleteJobTemplateRequestRequestTypeDef](./type_defs.md#deletejobtemplaterequestrequesttypedef) 

### delete\_managed\_endpoint

Deletes a managed endpoint.

Type annotations and code completion for `#!python session.create_client("emr-containers").delete_managed_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.delete_managed_endpoint)

```python
# delete_managed_endpoint method definition

await def delete_managed_endpoint(
    self,
    *,
    id: str,
    virtualClusterId: str,
) -> DeleteManagedEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteManagedEndpointResponseTypeDef](./type_defs.md#deletemanagedendpointresponsetypedef) 


```python
# delete_managed_endpoint method usage example with argument unpacking

kwargs: DeleteManagedEndpointRequestRequestTypeDef = {  # (1)
    "id": ...,
    "virtualClusterId": ...,
}

parent.delete_managed_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteManagedEndpointRequestRequestTypeDef](./type_defs.md#deletemanagedendpointrequestrequesttypedef) 

### delete\_virtual\_cluster

Deletes a virtual cluster.

Type annotations and code completion for `#!python session.create_client("emr-containers").delete_virtual_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.delete_virtual_cluster)

```python
# delete_virtual_cluster method definition

await def delete_virtual_cluster(
    self,
    *,
    id: str,
) -> DeleteVirtualClusterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteVirtualClusterResponseTypeDef](./type_defs.md#deletevirtualclusterresponsetypedef) 


```python
# delete_virtual_cluster method usage example with argument unpacking

kwargs: DeleteVirtualClusterRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_virtual_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteVirtualClusterRequestRequestTypeDef](./type_defs.md#deletevirtualclusterrequestrequesttypedef) 

### describe\_job\_run

Displays detailed information about a job run.

Type annotations and code completion for `#!python session.create_client("emr-containers").describe_job_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_job_run)

```python
# describe_job_run method definition

await def describe_job_run(
    self,
    *,
    id: str,
    virtualClusterId: str,
) -> DescribeJobRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeJobRunResponseTypeDef](./type_defs.md#describejobrunresponsetypedef) 


```python
# describe_job_run method usage example with argument unpacking

kwargs: DescribeJobRunRequestRequestTypeDef = {  # (1)
    "id": ...,
    "virtualClusterId": ...,
}

parent.describe_job_run(**kwargs)
```

1. See [:material-code-braces: DescribeJobRunRequestRequestTypeDef](./type_defs.md#describejobrunrequestrequesttypedef) 

### describe\_job\_template

Displays detailed information about a specified job template.

Type annotations and code completion for `#!python session.create_client("emr-containers").describe_job_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_job_template)

```python
# describe_job_template method definition

await def describe_job_template(
    self,
    *,
    id: str,
) -> DescribeJobTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeJobTemplateResponseTypeDef](./type_defs.md#describejobtemplateresponsetypedef) 


```python
# describe_job_template method usage example with argument unpacking

kwargs: DescribeJobTemplateRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.describe_job_template(**kwargs)
```

1. See [:material-code-braces: DescribeJobTemplateRequestRequestTypeDef](./type_defs.md#describejobtemplaterequestrequesttypedef) 

### describe\_managed\_endpoint

Displays detailed information about a managed endpoint.

Type annotations and code completion for `#!python session.create_client("emr-containers").describe_managed_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_managed_endpoint)

```python
# describe_managed_endpoint method definition

await def describe_managed_endpoint(
    self,
    *,
    id: str,
    virtualClusterId: str,
) -> DescribeManagedEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeManagedEndpointResponseTypeDef](./type_defs.md#describemanagedendpointresponsetypedef) 


```python
# describe_managed_endpoint method usage example with argument unpacking

kwargs: DescribeManagedEndpointRequestRequestTypeDef = {  # (1)
    "id": ...,
    "virtualClusterId": ...,
}

parent.describe_managed_endpoint(**kwargs)
```

1. See [:material-code-braces: DescribeManagedEndpointRequestRequestTypeDef](./type_defs.md#describemanagedendpointrequestrequesttypedef) 

### describe\_virtual\_cluster

Displays detailed information about a specified virtual cluster.

Type annotations and code completion for `#!python session.create_client("emr-containers").describe_virtual_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_virtual_cluster)

```python
# describe_virtual_cluster method definition

await def describe_virtual_cluster(
    self,
    *,
    id: str,
) -> DescribeVirtualClusterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVirtualClusterResponseTypeDef](./type_defs.md#describevirtualclusterresponsetypedef) 


```python
# describe_virtual_cluster method usage example with argument unpacking

kwargs: DescribeVirtualClusterRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.describe_virtual_cluster(**kwargs)
```

1. See [:material-code-braces: DescribeVirtualClusterRequestRequestTypeDef](./type_defs.md#describevirtualclusterrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("emr-containers").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.generate_presigned_url)

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


### get\_managed\_endpoint\_session\_credentials

Generate a session token to connect to a managed endpoint.

Type annotations and code completion for `#!python session.create_client("emr-containers").get_managed_endpoint_session_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_managed_endpoint_session_credentials)

```python
# get_managed_endpoint_session_credentials method definition

await def get_managed_endpoint_session_credentials(
    self,
    *,
    endpointIdentifier: str,
    virtualClusterIdentifier: str,
    executionRoleArn: str,
    credentialType: str,
    durationInSeconds: int = ...,
    logContext: str = ...,
    clientToken: str = ...,
) -> GetManagedEndpointSessionCredentialsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetManagedEndpointSessionCredentialsResponseTypeDef](./type_defs.md#getmanagedendpointsessioncredentialsresponsetypedef) 


```python
# get_managed_endpoint_session_credentials method usage example with argument unpacking

kwargs: GetManagedEndpointSessionCredentialsRequestRequestTypeDef = {  # (1)
    "endpointIdentifier": ...,
    "virtualClusterIdentifier": ...,
    "executionRoleArn": ...,
    "credentialType": ...,
}

parent.get_managed_endpoint_session_credentials(**kwargs)
```

1. See [:material-code-braces: GetManagedEndpointSessionCredentialsRequestRequestTypeDef](./type_defs.md#getmanagedendpointsessioncredentialsrequestrequesttypedef) 

### list\_job\_runs

Lists job runs based on a set of parameters.

Type annotations and code completion for `#!python session.create_client("emr-containers").list_job_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_runs)

```python
# list_job_runs method definition

await def list_job_runs(
    self,
    *,
    virtualClusterId: str,
    createdBefore: Union[datetime, str] = ...,
    createdAfter: Union[datetime, str] = ...,
    name: str = ...,
    states: Sequence[JobRunStateType] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListJobRunsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
2. See [:material-code-braces: ListJobRunsResponseTypeDef](./type_defs.md#listjobrunsresponsetypedef) 


```python
# list_job_runs method usage example with argument unpacking

kwargs: ListJobRunsRequestRequestTypeDef = {  # (1)
    "virtualClusterId": ...,
}

parent.list_job_runs(**kwargs)
```

1. See [:material-code-braces: ListJobRunsRequestRequestTypeDef](./type_defs.md#listjobrunsrequestrequesttypedef) 

### list\_job\_templates

Lists job templates based on a set of parameters.

Type annotations and code completion for `#!python session.create_client("emr-containers").list_job_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_templates)

```python
# list_job_templates method definition

await def list_job_templates(
    self,
    *,
    createdAfter: Union[datetime, str] = ...,
    createdBefore: Union[datetime, str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListJobTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJobTemplatesResponseTypeDef](./type_defs.md#listjobtemplatesresponsetypedef) 


```python
# list_job_templates method usage example with argument unpacking

kwargs: ListJobTemplatesRequestRequestTypeDef = {  # (1)
    "createdAfter": ...,
}

parent.list_job_templates(**kwargs)
```

1. See [:material-code-braces: ListJobTemplatesRequestRequestTypeDef](./type_defs.md#listjobtemplatesrequestrequesttypedef) 

### list\_managed\_endpoints

Lists managed endpoints based on a set of parameters.

Type annotations and code completion for `#!python session.create_client("emr-containers").list_managed_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_managed_endpoints)

```python
# list_managed_endpoints method definition

await def list_managed_endpoints(
    self,
    *,
    virtualClusterId: str,
    createdBefore: Union[datetime, str] = ...,
    createdAfter: Union[datetime, str] = ...,
    types: Sequence[str] = ...,
    states: Sequence[EndpointStateType] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListManagedEndpointsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EndpointStateType](./literals.md#endpointstatetype) 
2. See [:material-code-braces: ListManagedEndpointsResponseTypeDef](./type_defs.md#listmanagedendpointsresponsetypedef) 


```python
# list_managed_endpoints method usage example with argument unpacking

kwargs: ListManagedEndpointsRequestRequestTypeDef = {  # (1)
    "virtualClusterId": ...,
}

parent.list_managed_endpoints(**kwargs)
```

1. See [:material-code-braces: ListManagedEndpointsRequestRequestTypeDef](./type_defs.md#listmanagedendpointsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags assigned to the resources.

Type annotations and code completion for `#!python session.create_client("emr-containers").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_tags_for_resource)

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

### list\_virtual\_clusters

Lists information about the specified virtual cluster.

Type annotations and code completion for `#!python session.create_client("emr-containers").list_virtual_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_virtual_clusters)

```python
# list_virtual_clusters method definition

await def list_virtual_clusters(
    self,
    *,
    containerProviderId: str = ...,
    containerProviderType: ContainerProviderTypeType = ...,  # (1)
    createdAfter: Union[datetime, str] = ...,
    createdBefore: Union[datetime, str] = ...,
    states: Sequence[VirtualClusterStateType] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListVirtualClustersResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ContainerProviderTypeType](./literals.md#containerprovidertypetype) 
2. See [:material-code-brackets: VirtualClusterStateType](./literals.md#virtualclusterstatetype) 
3. See [:material-code-braces: ListVirtualClustersResponseTypeDef](./type_defs.md#listvirtualclustersresponsetypedef) 


```python
# list_virtual_clusters method usage example with argument unpacking

kwargs: ListVirtualClustersRequestRequestTypeDef = {  # (1)
    "containerProviderId": ...,
}

parent.list_virtual_clusters(**kwargs)
```

1. See [:material-code-braces: ListVirtualClustersRequestRequestTypeDef](./type_defs.md#listvirtualclustersrequestrequesttypedef) 

### start\_job\_run

Starts a job run.

Type annotations and code completion for `#!python session.create_client("emr-containers").start_job_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.start_job_run)

```python
# start_job_run method definition

await def start_job_run(
    self,
    *,
    virtualClusterId: str,
    clientToken: str,
    name: str = ...,
    executionRoleArn: str = ...,
    releaseLabel: str = ...,
    jobDriver: JobDriverTypeDef = ...,  # (1)
    configurationOverrides: ConfigurationOverridesTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
    jobTemplateId: str = ...,
    jobTemplateParameters: Mapping[str, str] = ...,
    retryPolicyConfiguration: RetryPolicyConfigurationTypeDef = ...,  # (3)
) -> StartJobRunResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: JobDriverTypeDef](./type_defs.md#jobdrivertypedef) 
2. See [:material-code-braces: ConfigurationOverridesTypeDef](./type_defs.md#configurationoverridestypedef) 
3. See [:material-code-braces: RetryPolicyConfigurationTypeDef](./type_defs.md#retrypolicyconfigurationtypedef) 
4. See [:material-code-braces: StartJobRunResponseTypeDef](./type_defs.md#startjobrunresponsetypedef) 


```python
# start_job_run method usage example with argument unpacking

kwargs: StartJobRunRequestRequestTypeDef = {  # (1)
    "virtualClusterId": ...,
    "clientToken": ...,
}

parent.start_job_run(**kwargs)
```

1. See [:material-code-braces: StartJobRunRequestRequestTypeDef](./type_defs.md#startjobrunrequestrequesttypedef) 

### tag\_resource

Assigns tags to resources.

Type annotations and code completion for `#!python session.create_client("emr-containers").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.tag_resource)

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

Removes tags from resources.

Type annotations and code completion for `#!python session.create_client("emr-containers").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.untag_resource)

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

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("emr-containers").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> EMRContainersClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("emr-containers").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("emr-containers").get_paginator` method with overloads.

- `client.get_paginator("list_job_runs")` -> [ListJobRunsPaginator](./paginators.md#listjobrunspaginator)
- `client.get_paginator("list_job_templates")` -> [ListJobTemplatesPaginator](./paginators.md#listjobtemplatespaginator)
- `client.get_paginator("list_managed_endpoints")` -> [ListManagedEndpointsPaginator](./paginators.md#listmanagedendpointspaginator)
- `client.get_paginator("list_virtual_clusters")` -> [ListVirtualClustersPaginator](./paginators.md#listvirtualclusterspaginator)



