# Paginators

> [Index](../README.md) > [Greengrass](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Greengrass](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#greengrass)
    type annotations stubs module [types-aiobotocore-greengrass](https://pypi.org/project/types-aiobotocore-greengrass/).

## ListBulkDeploymentDetailedReportsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_bulk_deployment_detailed_reports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListBulkDeploymentDetailedReports.html#Greengrass.Paginator.ListBulkDeploymentDetailedReports)

```python
# ListBulkDeploymentDetailedReportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListBulkDeploymentDetailedReportsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListBulkDeploymentDetailedReportsPaginator = client.get_paginator("list_bulk_deployment_detailed_reports")  # (2)
    async for item in paginator.paginate(...):
        item: ListBulkDeploymentDetailedReportsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListBulkDeploymentDetailedReportsPaginator](./paginators.md#listbulkdeploymentdetailedreportspaginator)
3. item: [:material-code-braces: ListBulkDeploymentDetailedReportsResponseTypeDef](./type_defs.md#listbulkdeploymentdetailedreportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBulkDeploymentDetailedReportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    BulkDeploymentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListBulkDeploymentDetailedReportsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBulkDeploymentDetailedReportsResponseTypeDef](./type_defs.md#listbulkdeploymentdetailedreportsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBulkDeploymentDetailedReportsRequestPaginateTypeDef = {  # (1)
    "BulkDeploymentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBulkDeploymentDetailedReportsRequestPaginateTypeDef](./type_defs.md#listbulkdeploymentdetailedreportsrequestpaginatetypedef) 
## ListBulkDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_bulk_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListBulkDeployments.html#Greengrass.Paginator.ListBulkDeployments)

```python
# ListBulkDeploymentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListBulkDeploymentsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListBulkDeploymentsPaginator = client.get_paginator("list_bulk_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: ListBulkDeploymentsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListBulkDeploymentsPaginator](./paginators.md#listbulkdeploymentspaginator)
3. item: [:material-code-braces: ListBulkDeploymentsResponseTypeDef](./type_defs.md#listbulkdeploymentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBulkDeploymentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListBulkDeploymentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBulkDeploymentsResponseTypeDef](./type_defs.md#listbulkdeploymentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBulkDeploymentsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBulkDeploymentsRequestPaginateTypeDef](./type_defs.md#listbulkdeploymentsrequestpaginatetypedef) 
## ListConnectorDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_connector_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListConnectorDefinitionVersions.html#Greengrass.Paginator.ListConnectorDefinitionVersions)

```python
# ListConnectorDefinitionVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListConnectorDefinitionVersionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListConnectorDefinitionVersionsPaginator = client.get_paginator("list_connector_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectorDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListConnectorDefinitionVersionsPaginator](./paginators.md#listconnectordefinitionversionspaginator)
3. item: [:material-code-braces: ListConnectorDefinitionVersionsResponseTypeDef](./type_defs.md#listconnectordefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConnectorDefinitionVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConnectorDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConnectorDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConnectorDefinitionVersionsResponseTypeDef](./type_defs.md#listconnectordefinitionversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConnectorDefinitionVersionsRequestPaginateTypeDef = {  # (1)
    "ConnectorDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectorDefinitionVersionsRequestPaginateTypeDef](./type_defs.md#listconnectordefinitionversionsrequestpaginatetypedef) 
## ListConnectorDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_connector_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListConnectorDefinitions.html#Greengrass.Paginator.ListConnectorDefinitions)

```python
# ListConnectorDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListConnectorDefinitionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListConnectorDefinitionsPaginator = client.get_paginator("list_connector_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectorDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListConnectorDefinitionsPaginator](./paginators.md#listconnectordefinitionspaginator)
3. item: [:material-code-braces: ListConnectorDefinitionsResponseTypeDef](./type_defs.md#listconnectordefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConnectorDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConnectorDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConnectorDefinitionsResponseTypeDef](./type_defs.md#listconnectordefinitionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConnectorDefinitionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectorDefinitionsRequestPaginateTypeDef](./type_defs.md#listconnectordefinitionsrequestpaginatetypedef) 
## ListCoreDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_core_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListCoreDefinitionVersions.html#Greengrass.Paginator.ListCoreDefinitionVersions)

```python
# ListCoreDefinitionVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListCoreDefinitionVersionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListCoreDefinitionVersionsPaginator = client.get_paginator("list_core_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListCoreDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListCoreDefinitionVersionsPaginator](./paginators.md#listcoredefinitionversionspaginator)
3. item: [:material-code-braces: ListCoreDefinitionVersionsResponseTypeDef](./type_defs.md#listcoredefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCoreDefinitionVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CoreDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCoreDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCoreDefinitionVersionsResponseTypeDef](./type_defs.md#listcoredefinitionversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCoreDefinitionVersionsRequestPaginateTypeDef = {  # (1)
    "CoreDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCoreDefinitionVersionsRequestPaginateTypeDef](./type_defs.md#listcoredefinitionversionsrequestpaginatetypedef) 
## ListCoreDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_core_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListCoreDefinitions.html#Greengrass.Paginator.ListCoreDefinitions)

```python
# ListCoreDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListCoreDefinitionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListCoreDefinitionsPaginator = client.get_paginator("list_core_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListCoreDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListCoreDefinitionsPaginator](./paginators.md#listcoredefinitionspaginator)
3. item: [:material-code-braces: ListCoreDefinitionsResponseTypeDef](./type_defs.md#listcoredefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCoreDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCoreDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCoreDefinitionsResponseTypeDef](./type_defs.md#listcoredefinitionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCoreDefinitionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCoreDefinitionsRequestPaginateTypeDef](./type_defs.md#listcoredefinitionsrequestpaginatetypedef) 
## ListDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListDeployments.html#Greengrass.Paginator.ListDeployments)

```python
# ListDeploymentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListDeploymentsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
3. item: [:material-code-braces: ListDeploymentsResponseTypeDef](./type_defs.md#listdeploymentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDeploymentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GroupId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDeploymentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeploymentsResponseTypeDef](./type_defs.md#listdeploymentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeploymentsRequestPaginateTypeDef = {  # (1)
    "GroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsRequestPaginateTypeDef](./type_defs.md#listdeploymentsrequestpaginatetypedef) 
## ListDeviceDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_device_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListDeviceDefinitionVersions.html#Greengrass.Paginator.ListDeviceDefinitionVersions)

```python
# ListDeviceDefinitionVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListDeviceDefinitionVersionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListDeviceDefinitionVersionsPaginator = client.get_paginator("list_device_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeviceDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListDeviceDefinitionVersionsPaginator](./paginators.md#listdevicedefinitionversionspaginator)
3. item: [:material-code-braces: ListDeviceDefinitionVersionsResponseTypeDef](./type_defs.md#listdevicedefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDeviceDefinitionVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DeviceDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDeviceDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeviceDefinitionVersionsResponseTypeDef](./type_defs.md#listdevicedefinitionversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeviceDefinitionVersionsRequestPaginateTypeDef = {  # (1)
    "DeviceDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeviceDefinitionVersionsRequestPaginateTypeDef](./type_defs.md#listdevicedefinitionversionsrequestpaginatetypedef) 
## ListDeviceDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_device_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListDeviceDefinitions.html#Greengrass.Paginator.ListDeviceDefinitions)

```python
# ListDeviceDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListDeviceDefinitionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListDeviceDefinitionsPaginator = client.get_paginator("list_device_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeviceDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListDeviceDefinitionsPaginator](./paginators.md#listdevicedefinitionspaginator)
3. item: [:material-code-braces: ListDeviceDefinitionsResponseTypeDef](./type_defs.md#listdevicedefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDeviceDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDeviceDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeviceDefinitionsResponseTypeDef](./type_defs.md#listdevicedefinitionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeviceDefinitionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeviceDefinitionsRequestPaginateTypeDef](./type_defs.md#listdevicedefinitionsrequestpaginatetypedef) 
## ListFunctionDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_function_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListFunctionDefinitionVersions.html#Greengrass.Paginator.ListFunctionDefinitionVersions)

```python
# ListFunctionDefinitionVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListFunctionDefinitionVersionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListFunctionDefinitionVersionsPaginator = client.get_paginator("list_function_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListFunctionDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListFunctionDefinitionVersionsPaginator](./paginators.md#listfunctiondefinitionversionspaginator)
3. item: [:material-code-braces: ListFunctionDefinitionVersionsResponseTypeDef](./type_defs.md#listfunctiondefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFunctionDefinitionVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FunctionDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFunctionDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFunctionDefinitionVersionsResponseTypeDef](./type_defs.md#listfunctiondefinitionversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFunctionDefinitionVersionsRequestPaginateTypeDef = {  # (1)
    "FunctionDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFunctionDefinitionVersionsRequestPaginateTypeDef](./type_defs.md#listfunctiondefinitionversionsrequestpaginatetypedef) 
## ListFunctionDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_function_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListFunctionDefinitions.html#Greengrass.Paginator.ListFunctionDefinitions)

```python
# ListFunctionDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListFunctionDefinitionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListFunctionDefinitionsPaginator = client.get_paginator("list_function_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListFunctionDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListFunctionDefinitionsPaginator](./paginators.md#listfunctiondefinitionspaginator)
3. item: [:material-code-braces: ListFunctionDefinitionsResponseTypeDef](./type_defs.md#listfunctiondefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFunctionDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFunctionDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFunctionDefinitionsResponseTypeDef](./type_defs.md#listfunctiondefinitionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFunctionDefinitionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFunctionDefinitionsRequestPaginateTypeDef](./type_defs.md#listfunctiondefinitionsrequestpaginatetypedef) 
## ListGroupVersionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_group_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListGroupVersions.html#Greengrass.Paginator.ListGroupVersions)

```python
# ListGroupVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListGroupVersionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListGroupVersionsPaginator = client.get_paginator("list_group_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListGroupVersionsPaginator](./paginators.md#listgroupversionspaginator)
3. item: [:material-code-braces: ListGroupVersionsResponseTypeDef](./type_defs.md#listgroupversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GroupId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGroupVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupVersionsResponseTypeDef](./type_defs.md#listgroupversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupVersionsRequestPaginateTypeDef = {  # (1)
    "GroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupVersionsRequestPaginateTypeDef](./type_defs.md#listgroupversionsrequestpaginatetypedef) 
## ListGroupsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListGroups.html#Greengrass.Paginator.ListGroups)

```python
# ListGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListGroupsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListGroupsPaginator](./paginators.md#listgroupspaginator)
3. item: [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestPaginateTypeDef](./type_defs.md#listgroupsrequestpaginatetypedef) 
## ListLoggerDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_logger_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListLoggerDefinitionVersions.html#Greengrass.Paginator.ListLoggerDefinitionVersions)

```python
# ListLoggerDefinitionVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListLoggerDefinitionVersionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListLoggerDefinitionVersionsPaginator = client.get_paginator("list_logger_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListLoggerDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListLoggerDefinitionVersionsPaginator](./paginators.md#listloggerdefinitionversionspaginator)
3. item: [:material-code-braces: ListLoggerDefinitionVersionsResponseTypeDef](./type_defs.md#listloggerdefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLoggerDefinitionVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LoggerDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListLoggerDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLoggerDefinitionVersionsResponseTypeDef](./type_defs.md#listloggerdefinitionversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLoggerDefinitionVersionsRequestPaginateTypeDef = {  # (1)
    "LoggerDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLoggerDefinitionVersionsRequestPaginateTypeDef](./type_defs.md#listloggerdefinitionversionsrequestpaginatetypedef) 
## ListLoggerDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_logger_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListLoggerDefinitions.html#Greengrass.Paginator.ListLoggerDefinitions)

```python
# ListLoggerDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListLoggerDefinitionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListLoggerDefinitionsPaginator = client.get_paginator("list_logger_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListLoggerDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListLoggerDefinitionsPaginator](./paginators.md#listloggerdefinitionspaginator)
3. item: [:material-code-braces: ListLoggerDefinitionsResponseTypeDef](./type_defs.md#listloggerdefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLoggerDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListLoggerDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLoggerDefinitionsResponseTypeDef](./type_defs.md#listloggerdefinitionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLoggerDefinitionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLoggerDefinitionsRequestPaginateTypeDef](./type_defs.md#listloggerdefinitionsrequestpaginatetypedef) 
## ListResourceDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_resource_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListResourceDefinitionVersions.html#Greengrass.Paginator.ListResourceDefinitionVersions)

```python
# ListResourceDefinitionVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListResourceDefinitionVersionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListResourceDefinitionVersionsPaginator = client.get_paginator("list_resource_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListResourceDefinitionVersionsPaginator](./paginators.md#listresourcedefinitionversionspaginator)
3. item: [:material-code-braces: ListResourceDefinitionVersionsResponseTypeDef](./type_defs.md#listresourcedefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceDefinitionVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListResourceDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceDefinitionVersionsResponseTypeDef](./type_defs.md#listresourcedefinitionversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceDefinitionVersionsRequestPaginateTypeDef = {  # (1)
    "ResourceDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceDefinitionVersionsRequestPaginateTypeDef](./type_defs.md#listresourcedefinitionversionsrequestpaginatetypedef) 
## ListResourceDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_resource_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListResourceDefinitions.html#Greengrass.Paginator.ListResourceDefinitions)

```python
# ListResourceDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListResourceDefinitionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListResourceDefinitionsPaginator = client.get_paginator("list_resource_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListResourceDefinitionsPaginator](./paginators.md#listresourcedefinitionspaginator)
3. item: [:material-code-braces: ListResourceDefinitionsResponseTypeDef](./type_defs.md#listresourcedefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListResourceDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceDefinitionsResponseTypeDef](./type_defs.md#listresourcedefinitionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceDefinitionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceDefinitionsRequestPaginateTypeDef](./type_defs.md#listresourcedefinitionsrequestpaginatetypedef) 
## ListSubscriptionDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_subscription_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListSubscriptionDefinitionVersions.html#Greengrass.Paginator.ListSubscriptionDefinitionVersions)

```python
# ListSubscriptionDefinitionVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListSubscriptionDefinitionVersionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListSubscriptionDefinitionVersionsPaginator = client.get_paginator("list_subscription_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListSubscriptionDefinitionVersionsPaginator](./paginators.md#listsubscriptiondefinitionversionspaginator)
3. item: [:material-code-braces: ListSubscriptionDefinitionVersionsResponseTypeDef](./type_defs.md#listsubscriptiondefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscriptionDefinitionVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SubscriptionDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSubscriptionDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubscriptionDefinitionVersionsResponseTypeDef](./type_defs.md#listsubscriptiondefinitionversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSubscriptionDefinitionVersionsRequestPaginateTypeDef = {  # (1)
    "SubscriptionDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionDefinitionVersionsRequestPaginateTypeDef](./type_defs.md#listsubscriptiondefinitionversionsrequestpaginatetypedef) 
## ListSubscriptionDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrass").get_paginator("list_subscription_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass/paginator/ListSubscriptionDefinitions.html#Greengrass.Paginator.ListSubscriptionDefinitions)

```python
# ListSubscriptionDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.paginator import ListSubscriptionDefinitionsPaginator

session = get_session()
async with session.create_client("greengrass") as client:  # (1)
    paginator: ListSubscriptionDefinitionsPaginator = client.get_paginator("list_subscription_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListSubscriptionDefinitionsPaginator](./paginators.md#listsubscriptiondefinitionspaginator)
3. item: [:material-code-braces: ListSubscriptionDefinitionsResponseTypeDef](./type_defs.md#listsubscriptiondefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscriptionDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSubscriptionDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubscriptionDefinitionsResponseTypeDef](./type_defs.md#listsubscriptiondefinitionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSubscriptionDefinitionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionDefinitionsRequestPaginateTypeDef](./type_defs.md#listsubscriptiondefinitionsrequestpaginatetypedef) 
