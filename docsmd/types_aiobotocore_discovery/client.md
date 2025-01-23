# ApplicationDiscoveryServiceClient

> [Index](../README.md) > [ApplicationDiscoveryService](./README.md) > ApplicationDiscoveryServiceClient

!!! note ""

    Auto-generated documentation for [ApplicationDiscoveryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#applicationdiscoveryservice)
    type annotations stubs module [types-aiobotocore-discovery](https://pypi.org/project/types-aiobotocore-discovery/).

## ApplicationDiscoveryServiceClient

Type annotations and code completion for `#!python session.create_client("discovery")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client)

```python
# ApplicationDiscoveryServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_discovery.client import ApplicationDiscoveryServiceClient

session = get_session()
async with session.create_client("discovery") as client:
    client: ApplicationDiscoveryServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("discovery").exceptions` structure.

```python
# ApplicationDiscoveryServiceClient.exceptions usage example

async with session.create_client("discovery") as client:
    try:
        do_something(client)
    except (
            client.AuthorizationErrorException,
        client.ClientError,
        client.ConflictErrorException,
        client.HomeRegionNotSetException,
        client.InvalidParameterException,
        client.InvalidParameterValueException,
        client.LimitExceededException,
        client.OperationNotPermittedException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.ServerInternalErrorException,
    ) as e:
        print(e)
```

```python
# ApplicationDiscoveryServiceClient usage type checking example

from types_aiobotocore_discovery.client import Exceptions

def handle_error(exc: Exceptions.AuthorizationErrorException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("discovery").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("discovery").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/generate_presigned_url.html)

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


### associate\_configuration\_items\_to\_application

Associates one or more configuration items with an application.

Type annotations and code completion for `#!python session.create_client("discovery").associate_configuration_items_to_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/associate_configuration_items_to_application.html)

```python
# associate_configuration_items_to_application method definition

await def associate_configuration_items_to_application(
    self,
    *,
    applicationConfigurationId: str,
    configurationIds: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# associate_configuration_items_to_application method usage example with argument unpacking

kwargs: AssociateConfigurationItemsToApplicationRequestRequestTypeDef = {  # (1)
    "applicationConfigurationId": ...,
    "configurationIds": ...,
}

parent.associate_configuration_items_to_application(**kwargs)
```

1. See [:material-code-braces: AssociateConfigurationItemsToApplicationRequestRequestTypeDef](./type_defs.md#associateconfigurationitemstoapplicationrequestrequesttypedef) 

### batch\_delete\_agents

Deletes one or more agents or collectors as specified by ID.

Type annotations and code completion for `#!python session.create_client("discovery").batch_delete_agents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/batch_delete_agents.html)

```python
# batch_delete_agents method definition

await def batch_delete_agents(
    self,
    *,
    deleteAgents: Sequence[DeleteAgentTypeDef],  # (1)
) -> BatchDeleteAgentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeleteAgentTypeDef](./type_defs.md#deleteagenttypedef) 
2. See [:material-code-braces: BatchDeleteAgentsResponseTypeDef](./type_defs.md#batchdeleteagentsresponsetypedef) 


```python
# batch_delete_agents method usage example with argument unpacking

kwargs: BatchDeleteAgentsRequestRequestTypeDef = {  # (1)
    "deleteAgents": ...,
}

parent.batch_delete_agents(**kwargs)
```

1. See [:material-code-braces: BatchDeleteAgentsRequestRequestTypeDef](./type_defs.md#batchdeleteagentsrequestrequesttypedef) 

### batch\_delete\_import\_data

Deletes one or more import tasks, each identified by their import ID.

Type annotations and code completion for `#!python session.create_client("discovery").batch_delete_import_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/batch_delete_import_data.html)

```python
# batch_delete_import_data method definition

await def batch_delete_import_data(
    self,
    *,
    importTaskIds: Sequence[str],
    deleteHistory: bool = ...,
) -> BatchDeleteImportDataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteImportDataResponseTypeDef](./type_defs.md#batchdeleteimportdataresponsetypedef) 


```python
# batch_delete_import_data method usage example with argument unpacking

kwargs: BatchDeleteImportDataRequestRequestTypeDef = {  # (1)
    "importTaskIds": ...,
}

parent.batch_delete_import_data(**kwargs)
```

1. See [:material-code-braces: BatchDeleteImportDataRequestRequestTypeDef](./type_defs.md#batchdeleteimportdatarequestrequesttypedef) 

### create\_application

Creates an application with the given name and description.

Type annotations and code completion for `#!python session.create_client("discovery").create_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/create_application.html)

```python
# create_application method definition

await def create_application(
    self,
    *,
    name: str,
    description: str = ...,
    wave: str = ...,
) -> CreateApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 


```python
# create_application method usage example with argument unpacking

kwargs: CreateApplicationRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_application(**kwargs)
```

1. See [:material-code-braces: CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef) 

### create\_tags

Creates one or more tags for configuration items.

Type annotations and code completion for `#!python session.create_client("discovery").create_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/create_tags.html)

```python
# create_tags method definition

await def create_tags(
    self,
    *,
    configurationIds: Sequence[str],
    tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create_tags method usage example with argument unpacking

kwargs: CreateTagsRequestRequestTypeDef = {  # (1)
    "configurationIds": ...,
    "tags": ...,
}

parent.create_tags(**kwargs)
```

1. See [:material-code-braces: CreateTagsRequestRequestTypeDef](./type_defs.md#createtagsrequestrequesttypedef) 

### delete\_applications

Deletes a list of applications and their associations with configuration items.

Type annotations and code completion for `#!python session.create_client("discovery").delete_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/delete_applications.html)

```python
# delete_applications method definition

await def delete_applications(
    self,
    *,
    configurationIds: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# delete_applications method usage example with argument unpacking

kwargs: DeleteApplicationsRequestRequestTypeDef = {  # (1)
    "configurationIds": ...,
}

parent.delete_applications(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationsRequestRequestTypeDef](./type_defs.md#deleteapplicationsrequestrequesttypedef) 

### delete\_tags

Deletes the association between configuration items and one or more tags.

Type annotations and code completion for `#!python session.create_client("discovery").delete_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/delete_tags.html)

```python
# delete_tags method definition

await def delete_tags(
    self,
    *,
    configurationIds: Sequence[str],
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# delete_tags method usage example with argument unpacking

kwargs: DeleteTagsRequestRequestTypeDef = {  # (1)
    "configurationIds": ...,
}

parent.delete_tags(**kwargs)
```

1. See [:material-code-braces: DeleteTagsRequestRequestTypeDef](./type_defs.md#deletetagsrequestrequesttypedef) 

### describe\_agents

Lists agents or collectors as specified by ID or other filters.

Type annotations and code completion for `#!python session.create_client("discovery").describe_agents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/describe_agents.html)

```python
# describe_agents method definition

await def describe_agents(
    self,
    *,
    agentIds: Sequence[str] = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeAgentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeAgentsResponseTypeDef](./type_defs.md#describeagentsresponsetypedef) 


```python
# describe_agents method usage example with argument unpacking

kwargs: DescribeAgentsRequestRequestTypeDef = {  # (1)
    "agentIds": ...,
}

parent.describe_agents(**kwargs)
```

1. See [:material-code-braces: DescribeAgentsRequestRequestTypeDef](./type_defs.md#describeagentsrequestrequesttypedef) 

### describe\_batch\_delete\_configuration\_task

Takes a unique deletion task identifier as input and returns metadata about a
configuration deletion task.

Type annotations and code completion for `#!python session.create_client("discovery").describe_batch_delete_configuration_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/describe_batch_delete_configuration_task.html)

```python
# describe_batch_delete_configuration_task method definition

await def describe_batch_delete_configuration_task(
    self,
    *,
    taskId: str,
) -> DescribeBatchDeleteConfigurationTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBatchDeleteConfigurationTaskResponseTypeDef](./type_defs.md#describebatchdeleteconfigurationtaskresponsetypedef) 


```python
# describe_batch_delete_configuration_task method usage example with argument unpacking

kwargs: DescribeBatchDeleteConfigurationTaskRequestRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.describe_batch_delete_configuration_task(**kwargs)
```

1. See [:material-code-braces: DescribeBatchDeleteConfigurationTaskRequestRequestTypeDef](./type_defs.md#describebatchdeleteconfigurationtaskrequestrequesttypedef) 

### describe\_configurations

Retrieves attributes for a list of configuration item IDs.

Type annotations and code completion for `#!python session.create_client("discovery").describe_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/describe_configurations.html)

```python
# describe_configurations method definition

await def describe_configurations(
    self,
    *,
    configurationIds: Sequence[str],
) -> DescribeConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConfigurationsResponseTypeDef](./type_defs.md#describeconfigurationsresponsetypedef) 


```python
# describe_configurations method usage example with argument unpacking

kwargs: DescribeConfigurationsRequestRequestTypeDef = {  # (1)
    "configurationIds": ...,
}

parent.describe_configurations(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationsRequestRequestTypeDef](./type_defs.md#describeconfigurationsrequestrequesttypedef) 

### describe\_continuous\_exports

Lists exports as specified by ID.

Type annotations and code completion for `#!python session.create_client("discovery").describe_continuous_exports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/describe_continuous_exports.html)

```python
# describe_continuous_exports method definition

await def describe_continuous_exports(
    self,
    *,
    exportIds: Sequence[str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeContinuousExportsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeContinuousExportsResponseTypeDef](./type_defs.md#describecontinuousexportsresponsetypedef) 


```python
# describe_continuous_exports method usage example with argument unpacking

kwargs: DescribeContinuousExportsRequestRequestTypeDef = {  # (1)
    "exportIds": ...,
}

parent.describe_continuous_exports(**kwargs)
```

1. See [:material-code-braces: DescribeContinuousExportsRequestRequestTypeDef](./type_defs.md#describecontinuousexportsrequestrequesttypedef) 

### describe\_export\_configurations

<code>DescribeExportConfigurations</code> is deprecated.

Type annotations and code completion for `#!python session.create_client("discovery").describe_export_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/describe_export_configurations.html)

```python
# describe_export_configurations method definition

await def describe_export_configurations(
    self,
    *,
    exportIds: Sequence[str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeExportConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeExportConfigurationsResponseTypeDef](./type_defs.md#describeexportconfigurationsresponsetypedef) 


```python
# describe_export_configurations method usage example with argument unpacking

kwargs: DescribeExportConfigurationsRequestRequestTypeDef = {  # (1)
    "exportIds": ...,
}

parent.describe_export_configurations(**kwargs)
```

1. See [:material-code-braces: DescribeExportConfigurationsRequestRequestTypeDef](./type_defs.md#describeexportconfigurationsrequestrequesttypedef) 

### describe\_export\_tasks

Retrieve status of one or more export tasks.

Type annotations and code completion for `#!python session.create_client("discovery").describe_export_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/describe_export_tasks.html)

```python
# describe_export_tasks method definition

await def describe_export_tasks(
    self,
    *,
    exportIds: Sequence[str] = ...,
    filters: Sequence[ExportFilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeExportTasksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ExportFilterTypeDef](./type_defs.md#exportfiltertypedef) 
2. See [:material-code-braces: DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef) 


```python
# describe_export_tasks method usage example with argument unpacking

kwargs: DescribeExportTasksRequestRequestTypeDef = {  # (1)
    "exportIds": ...,
}

parent.describe_export_tasks(**kwargs)
```

1. See [:material-code-braces: DescribeExportTasksRequestRequestTypeDef](./type_defs.md#describeexporttasksrequestrequesttypedef) 

### describe\_import\_tasks

Returns an array of import tasks for your account, including status
information, times, IDs, the Amazon S3 Object URL for the import file, and
more.

Type annotations and code completion for `#!python session.create_client("discovery").describe_import_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/describe_import_tasks.html)

```python
# describe_import_tasks method definition

await def describe_import_tasks(
    self,
    *,
    filters: Sequence[ImportTaskFilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeImportTasksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ImportTaskFilterTypeDef](./type_defs.md#importtaskfiltertypedef) 
2. See [:material-code-braces: DescribeImportTasksResponseTypeDef](./type_defs.md#describeimporttasksresponsetypedef) 


```python
# describe_import_tasks method usage example with argument unpacking

kwargs: DescribeImportTasksRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.describe_import_tasks(**kwargs)
```

1. See [:material-code-braces: DescribeImportTasksRequestRequestTypeDef](./type_defs.md#describeimporttasksrequestrequesttypedef) 

### describe\_tags

Retrieves a list of configuration items that have tags as specified by the
key-value pairs, name and value, passed to the optional parameter
<code>filters</code>.

Type annotations and code completion for `#!python session.create_client("discovery").describe_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/describe_tags.html)

```python
# describe_tags method definition

await def describe_tags(
    self,
    *,
    filters: Sequence[TagFilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeTagsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
2. See [:material-code-braces: DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef) 


```python
# describe_tags method usage example with argument unpacking

kwargs: DescribeTagsRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.describe_tags(**kwargs)
```

1. See [:material-code-braces: DescribeTagsRequestRequestTypeDef](./type_defs.md#describetagsrequestrequesttypedef) 

### disassociate\_configuration\_items\_from\_application

Disassociates one or more configuration items from an application.

Type annotations and code completion for `#!python session.create_client("discovery").disassociate_configuration_items_from_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/disassociate_configuration_items_from_application.html)

```python
# disassociate_configuration_items_from_application method definition

await def disassociate_configuration_items_from_application(
    self,
    *,
    applicationConfigurationId: str,
    configurationIds: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_configuration_items_from_application method usage example with argument unpacking

kwargs: DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef = {  # (1)
    "applicationConfigurationId": ...,
    "configurationIds": ...,
}

parent.disassociate_configuration_items_from_application(**kwargs)
```

1. See [:material-code-braces: DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef](./type_defs.md#disassociateconfigurationitemsfromapplicationrequestrequesttypedef) 

### export\_configurations

Deprecated.

Type annotations and code completion for `#!python session.create_client("discovery").export_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/export_configurations.html)

```python
# export_configurations method definition

await def export_configurations(
    self,
) -> ExportConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExportConfigurationsResponseTypeDef](./type_defs.md#exportconfigurationsresponsetypedef) 

### get\_discovery\_summary

Retrieves a short summary of discovered assets.

Type annotations and code completion for `#!python session.create_client("discovery").get_discovery_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/get_discovery_summary.html)

```python
# get_discovery_summary method definition

await def get_discovery_summary(
    self,
) -> GetDiscoverySummaryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDiscoverySummaryResponseTypeDef](./type_defs.md#getdiscoverysummaryresponsetypedef) 

### list\_configurations

Retrieves a list of configuration items as specified by the value passed to the
required parameter <code>configurationType</code>.

Type annotations and code completion for `#!python session.create_client("discovery").list_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/list_configurations.html)

```python
# list_configurations method definition

await def list_configurations(
    self,
    *,
    configurationType: ConfigurationItemTypeType,  # (1)
    filters: Sequence[FilterTypeDef] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
    orderBy: Sequence[OrderByElementTypeDef] = ...,  # (3)
) -> ListConfigurationsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ConfigurationItemTypeType](./literals.md#configurationitemtypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: OrderByElementTypeDef](./type_defs.md#orderbyelementtypedef) 
4. See [:material-code-braces: ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef) 


```python
# list_configurations method usage example with argument unpacking

kwargs: ListConfigurationsRequestRequestTypeDef = {  # (1)
    "configurationType": ...,
}

parent.list_configurations(**kwargs)
```

1. See [:material-code-braces: ListConfigurationsRequestRequestTypeDef](./type_defs.md#listconfigurationsrequestrequesttypedef) 

### list\_server\_neighbors

Retrieves a list of servers that are one network hop away from a specified
server.

Type annotations and code completion for `#!python session.create_client("discovery").list_server_neighbors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/list_server_neighbors.html)

```python
# list_server_neighbors method definition

await def list_server_neighbors(
    self,
    *,
    configurationId: str,
    portInformationNeeded: bool = ...,
    neighborConfigurationIds: Sequence[str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListServerNeighborsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServerNeighborsResponseTypeDef](./type_defs.md#listserverneighborsresponsetypedef) 


```python
# list_server_neighbors method usage example with argument unpacking

kwargs: ListServerNeighborsRequestRequestTypeDef = {  # (1)
    "configurationId": ...,
}

parent.list_server_neighbors(**kwargs)
```

1. See [:material-code-braces: ListServerNeighborsRequestRequestTypeDef](./type_defs.md#listserverneighborsrequestrequesttypedef) 

### start\_batch\_delete\_configuration\_task

Takes a list of configurationId as input and starts an asynchronous deletion
task to remove the configurationItems.

Type annotations and code completion for `#!python session.create_client("discovery").start_batch_delete_configuration_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/start_batch_delete_configuration_task.html)

```python
# start_batch_delete_configuration_task method definition

await def start_batch_delete_configuration_task(
    self,
    *,
    configurationType: DeletionConfigurationItemTypeType,  # (1)
    configurationIds: Sequence[str],
) -> StartBatchDeleteConfigurationTaskResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DeletionConfigurationItemTypeType](./literals.md#deletionconfigurationitemtypetype) 
2. See [:material-code-braces: StartBatchDeleteConfigurationTaskResponseTypeDef](./type_defs.md#startbatchdeleteconfigurationtaskresponsetypedef) 


```python
# start_batch_delete_configuration_task method usage example with argument unpacking

kwargs: StartBatchDeleteConfigurationTaskRequestRequestTypeDef = {  # (1)
    "configurationType": ...,
    "configurationIds": ...,
}

parent.start_batch_delete_configuration_task(**kwargs)
```

1. See [:material-code-braces: StartBatchDeleteConfigurationTaskRequestRequestTypeDef](./type_defs.md#startbatchdeleteconfigurationtaskrequestrequesttypedef) 

### start\_continuous\_export

Start the continuous flow of agent's discovered data into Amazon Athena.

Type annotations and code completion for `#!python session.create_client("discovery").start_continuous_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/start_continuous_export.html)

```python
# start_continuous_export method definition

await def start_continuous_export(
    self,
) -> StartContinuousExportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartContinuousExportResponseTypeDef](./type_defs.md#startcontinuousexportresponsetypedef) 

### start\_data\_collection\_by\_agent\_ids

Instructs the specified agents to start collecting data.

Type annotations and code completion for `#!python session.create_client("discovery").start_data_collection_by_agent_ids` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/start_data_collection_by_agent_ids.html)

```python
# start_data_collection_by_agent_ids method definition

await def start_data_collection_by_agent_ids(
    self,
    *,
    agentIds: Sequence[str],
) -> StartDataCollectionByAgentIdsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartDataCollectionByAgentIdsResponseTypeDef](./type_defs.md#startdatacollectionbyagentidsresponsetypedef) 


```python
# start_data_collection_by_agent_ids method usage example with argument unpacking

kwargs: StartDataCollectionByAgentIdsRequestRequestTypeDef = {  # (1)
    "agentIds": ...,
}

parent.start_data_collection_by_agent_ids(**kwargs)
```

1. See [:material-code-braces: StartDataCollectionByAgentIdsRequestRequestTypeDef](./type_defs.md#startdatacollectionbyagentidsrequestrequesttypedef) 

### start\_export\_task

Begins the export of a discovered data report to an Amazon S3 bucket managed by
Amazon Web Services.

Type annotations and code completion for `#!python session.create_client("discovery").start_export_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/start_export_task.html)

```python
# start_export_task method definition

await def start_export_task(
    self,
    *,
    exportDataFormat: Sequence[ExportDataFormatType] = ...,  # (1)
    filters: Sequence[ExportFilterTypeDef] = ...,  # (2)
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
    preferences: ExportPreferencesTypeDef = ...,  # (3)
) -> StartExportTaskResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ExportDataFormatType](./literals.md#exportdataformattype) 
2. See [:material-code-braces: ExportFilterTypeDef](./type_defs.md#exportfiltertypedef) 
3. See [:material-code-braces: ExportPreferencesTypeDef](./type_defs.md#exportpreferencestypedef) 
4. See [:material-code-braces: StartExportTaskResponseTypeDef](./type_defs.md#startexporttaskresponsetypedef) 


```python
# start_export_task method usage example with argument unpacking

kwargs: StartExportTaskRequestRequestTypeDef = {  # (1)
    "exportDataFormat": ...,
}

parent.start_export_task(**kwargs)
```

1. See [:material-code-braces: StartExportTaskRequestRequestTypeDef](./type_defs.md#startexporttaskrequestrequesttypedef) 

### start\_import\_task

Starts an import task, which allows you to import details of your on-premises
environment directly into Amazon Web Services Migration Hub without having to
use the Amazon Web Services Application Discovery Service (Application
Discovery Service) tools such as the Amazon Web Services Application D...

Type annotations and code completion for `#!python session.create_client("discovery").start_import_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/start_import_task.html)

```python
# start_import_task method definition

await def start_import_task(
    self,
    *,
    name: str,
    importUrl: str,
    clientRequestToken: str = ...,
) -> StartImportTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartImportTaskResponseTypeDef](./type_defs.md#startimporttaskresponsetypedef) 


```python
# start_import_task method usage example with argument unpacking

kwargs: StartImportTaskRequestRequestTypeDef = {  # (1)
    "name": ...,
    "importUrl": ...,
}

parent.start_import_task(**kwargs)
```

1. See [:material-code-braces: StartImportTaskRequestRequestTypeDef](./type_defs.md#startimporttaskrequestrequesttypedef) 

### stop\_continuous\_export

Stop the continuous flow of agent's discovered data into Amazon Athena.

Type annotations and code completion for `#!python session.create_client("discovery").stop_continuous_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/stop_continuous_export.html)

```python
# stop_continuous_export method definition

await def stop_continuous_export(
    self,
    *,
    exportId: str,
) -> StopContinuousExportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopContinuousExportResponseTypeDef](./type_defs.md#stopcontinuousexportresponsetypedef) 


```python
# stop_continuous_export method usage example with argument unpacking

kwargs: StopContinuousExportRequestRequestTypeDef = {  # (1)
    "exportId": ...,
}

parent.stop_continuous_export(**kwargs)
```

1. See [:material-code-braces: StopContinuousExportRequestRequestTypeDef](./type_defs.md#stopcontinuousexportrequestrequesttypedef) 

### stop\_data\_collection\_by\_agent\_ids

Instructs the specified agents to stop collecting data.

Type annotations and code completion for `#!python session.create_client("discovery").stop_data_collection_by_agent_ids` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/stop_data_collection_by_agent_ids.html)

```python
# stop_data_collection_by_agent_ids method definition

await def stop_data_collection_by_agent_ids(
    self,
    *,
    agentIds: Sequence[str],
) -> StopDataCollectionByAgentIdsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopDataCollectionByAgentIdsResponseTypeDef](./type_defs.md#stopdatacollectionbyagentidsresponsetypedef) 


```python
# stop_data_collection_by_agent_ids method usage example with argument unpacking

kwargs: StopDataCollectionByAgentIdsRequestRequestTypeDef = {  # (1)
    "agentIds": ...,
}

parent.stop_data_collection_by_agent_ids(**kwargs)
```

1. See [:material-code-braces: StopDataCollectionByAgentIdsRequestRequestTypeDef](./type_defs.md#stopdatacollectionbyagentidsrequestrequesttypedef) 

### update\_application

Updates metadata about an application.

Type annotations and code completion for `#!python session.create_client("discovery").update_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/client/update_application.html)

```python
# update_application method definition

await def update_application(
    self,
    *,
    configurationId: str,
    name: str = ...,
    description: str = ...,
    wave: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_application method usage example with argument unpacking

kwargs: UpdateApplicationRequestRequestTypeDef = {  # (1)
    "configurationId": ...,
}

parent.update_application(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("discovery").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("discovery").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("discovery").get_paginator` method with overloads.

- `client.get_paginator("describe_agents")` -> [DescribeAgentsPaginator](./paginators.md#describeagentspaginator)
- `client.get_paginator("describe_continuous_exports")` -> [DescribeContinuousExportsPaginator](./paginators.md#describecontinuousexportspaginator)
- `client.get_paginator("describe_export_configurations")` -> [DescribeExportConfigurationsPaginator](./paginators.md#describeexportconfigurationspaginator)
- `client.get_paginator("describe_export_tasks")` -> [DescribeExportTasksPaginator](./paginators.md#describeexporttaskspaginator)
- `client.get_paginator("describe_import_tasks")` -> [DescribeImportTasksPaginator](./paginators.md#describeimporttaskspaginator)
- `client.get_paginator("describe_tags")` -> [DescribeTagsPaginator](./paginators.md#describetagspaginator)
- `client.get_paginator("list_configurations")` -> [ListConfigurationsPaginator](./paginators.md#listconfigurationspaginator)



