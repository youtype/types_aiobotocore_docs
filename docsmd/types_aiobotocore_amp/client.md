# PrometheusServiceClient

> [Index](../README.md) > [PrometheusService](./README.md) > PrometheusServiceClient

!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## PrometheusServiceClient

Type annotations and code completion for `#!python session.create_client("amp")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client)

```python
# PrometheusServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_amp.client import PrometheusServiceClient

session = get_session()
async with session.create_client("amp") as client:
    client: PrometheusServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("amp").exceptions` structure.

```python
# PrometheusServiceClient.exceptions usage example

async with session.create_client("amp") as client:
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
# PrometheusServiceClient usage type checking example

from types_aiobotocore_amp.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("amp").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("amp").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_alert\_manager\_definition

The `CreateAlertManagerDefinition` operation creates the alert manager
definition in a
workspace.

Type annotations and code completion for `#!python session.create_client("amp").create_alert_manager_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_alert_manager_definition)

```python
# create_alert_manager_definition method definition

await def create_alert_manager_definition(
    self,
    *,
    data: BlobTypeDef,
    workspaceId: str,
    clientToken: str = ...,
) -> CreateAlertManagerDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAlertManagerDefinitionResponseTypeDef](./type_defs.md#createalertmanagerdefinitionresponsetypedef) 


```python
# create_alert_manager_definition method usage example with argument unpacking

kwargs: CreateAlertManagerDefinitionRequestRequestTypeDef = {  # (1)
    "data": ...,
    "workspaceId": ...,
}

parent.create_alert_manager_definition(**kwargs)
```

1. See [:material-code-braces: CreateAlertManagerDefinitionRequestRequestTypeDef](./type_defs.md#createalertmanagerdefinitionrequestrequesttypedef) 

### create\_logging\_configuration

The `CreateLoggingConfiguration` operation creates a logging configuration for
the
workspace.

Type annotations and code completion for `#!python session.create_client("amp").create_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_logging_configuration)

```python
# create_logging_configuration method definition

await def create_logging_configuration(
    self,
    *,
    logGroupArn: str,
    workspaceId: str,
    clientToken: str = ...,
) -> CreateLoggingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateLoggingConfigurationResponseTypeDef](./type_defs.md#createloggingconfigurationresponsetypedef) 


```python
# create_logging_configuration method usage example with argument unpacking

kwargs: CreateLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "logGroupArn": ...,
    "workspaceId": ...,
}

parent.create_logging_configuration(**kwargs)
```

1. See [:material-code-braces: CreateLoggingConfigurationRequestRequestTypeDef](./type_defs.md#createloggingconfigurationrequestrequesttypedef) 

### create\_rule\_groups\_namespace

The `CreateRuleGroupsNamespace` operation creates a rule groups namespace
within a
workspace.

Type annotations and code completion for `#!python session.create_client("amp").create_rule_groups_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_rule_groups_namespace)

```python
# create_rule_groups_namespace method definition

await def create_rule_groups_namespace(
    self,
    *,
    data: BlobTypeDef,
    name: str,
    workspaceId: str,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateRuleGroupsNamespaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateRuleGroupsNamespaceResponseTypeDef](./type_defs.md#createrulegroupsnamespaceresponsetypedef) 


```python
# create_rule_groups_namespace method usage example with argument unpacking

kwargs: CreateRuleGroupsNamespaceRequestRequestTypeDef = {  # (1)
    "data": ...,
    "name": ...,
    "workspaceId": ...,
}

parent.create_rule_groups_namespace(**kwargs)
```

1. See [:material-code-braces: CreateRuleGroupsNamespaceRequestRequestTypeDef](./type_defs.md#createrulegroupsnamespacerequestrequesttypedef) 

### create\_scraper

The `CreateScraper` operation creates a scraper to collect metrics.

Type annotations and code completion for `#!python session.create_client("amp").create_scraper` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_scraper)

```python
# create_scraper method definition

await def create_scraper(
    self,
    *,
    destination: DestinationTypeDef,  # (1)
    scrapeConfiguration: ScrapeConfigurationTypeDef,  # (2)
    source: SourceTypeDef,  # (3)
    alias: str = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateScraperResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: ScrapeConfigurationTypeDef](./type_defs.md#scrapeconfigurationtypedef) 
3. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
4. See [:material-code-braces: CreateScraperResponseTypeDef](./type_defs.md#createscraperresponsetypedef) 


```python
# create_scraper method usage example with argument unpacking

kwargs: CreateScraperRequestRequestTypeDef = {  # (1)
    "destination": ...,
    "scrapeConfiguration": ...,
    "source": ...,
}

parent.create_scraper(**kwargs)
```

1. See [:material-code-braces: CreateScraperRequestRequestTypeDef](./type_defs.md#createscraperrequestrequesttypedef) 

### create\_workspace

Creates a Prometheus workspace.

Type annotations and code completion for `#!python session.create_client("amp").create_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_workspace)

```python
# create_workspace method definition

await def create_workspace(
    self,
    *,
    alias: str = ...,
    clientToken: str = ...,
    kmsKeyArn: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateWorkspaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateWorkspaceResponseTypeDef](./type_defs.md#createworkspaceresponsetypedef) 


```python
# create_workspace method usage example with argument unpacking

kwargs: CreateWorkspaceRequestRequestTypeDef = {  # (1)
    "alias": ...,
}

parent.create_workspace(**kwargs)
```

1. See [:material-code-braces: CreateWorkspaceRequestRequestTypeDef](./type_defs.md#createworkspacerequestrequesttypedef) 

### delete\_alert\_manager\_definition

Deletes the alert manager definition from a workspace.

Type annotations and code completion for `#!python session.create_client("amp").delete_alert_manager_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.delete_alert_manager_definition)

```python
# delete_alert_manager_definition method definition

await def delete_alert_manager_definition(
    self,
    *,
    workspaceId: str,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_alert_manager_definition method usage example with argument unpacking

kwargs: DeleteAlertManagerDefinitionRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.delete_alert_manager_definition(**kwargs)
```

1. See [:material-code-braces: DeleteAlertManagerDefinitionRequestRequestTypeDef](./type_defs.md#deletealertmanagerdefinitionrequestrequesttypedef) 

### delete\_logging\_configuration

Deletes the logging configuration for a workspace.

Type annotations and code completion for `#!python session.create_client("amp").delete_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.delete_logging_configuration)

```python
# delete_logging_configuration method definition

await def delete_logging_configuration(
    self,
    *,
    workspaceId: str,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_logging_configuration method usage example with argument unpacking

kwargs: DeleteLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.delete_logging_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteLoggingConfigurationRequestRequestTypeDef](./type_defs.md#deleteloggingconfigurationrequestrequesttypedef) 

### delete\_rule\_groups\_namespace

Deletes one rule groups namespace and its associated rule groups definition.

Type annotations and code completion for `#!python session.create_client("amp").delete_rule_groups_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.delete_rule_groups_namespace)

```python
# delete_rule_groups_namespace method definition

await def delete_rule_groups_namespace(
    self,
    *,
    name: str,
    workspaceId: str,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_rule_groups_namespace method usage example with argument unpacking

kwargs: DeleteRuleGroupsNamespaceRequestRequestTypeDef = {  # (1)
    "name": ...,
    "workspaceId": ...,
}

parent.delete_rule_groups_namespace(**kwargs)
```

1. See [:material-code-braces: DeleteRuleGroupsNamespaceRequestRequestTypeDef](./type_defs.md#deleterulegroupsnamespacerequestrequesttypedef) 

### delete\_scraper

The `DeleteScraper` operation deletes one scraper, and stops any metrics
collection that the scraper
performs.

Type annotations and code completion for `#!python session.create_client("amp").delete_scraper` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.delete_scraper)

```python
# delete_scraper method definition

await def delete_scraper(
    self,
    *,
    scraperId: str,
    clientToken: str = ...,
) -> DeleteScraperResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteScraperResponseTypeDef](./type_defs.md#deletescraperresponsetypedef) 


```python
# delete_scraper method usage example with argument unpacking

kwargs: DeleteScraperRequestRequestTypeDef = {  # (1)
    "scraperId": ...,
}

parent.delete_scraper(**kwargs)
```

1. See [:material-code-braces: DeleteScraperRequestRequestTypeDef](./type_defs.md#deletescraperrequestrequesttypedef) 

### delete\_workspace

Deletes an existing workspace.

Type annotations and code completion for `#!python session.create_client("amp").delete_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.delete_workspace)

```python
# delete_workspace method definition

await def delete_workspace(
    self,
    *,
    workspaceId: str,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_workspace method usage example with argument unpacking

kwargs: DeleteWorkspaceRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.delete_workspace(**kwargs)
```

1. See [:material-code-braces: DeleteWorkspaceRequestRequestTypeDef](./type_defs.md#deleteworkspacerequestrequesttypedef) 

### describe\_alert\_manager\_definition

Retrieves the full information about the alert manager definition for a
workspace.

Type annotations and code completion for `#!python session.create_client("amp").describe_alert_manager_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.describe_alert_manager_definition)

```python
# describe_alert_manager_definition method definition

await def describe_alert_manager_definition(
    self,
    *,
    workspaceId: str,
) -> DescribeAlertManagerDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAlertManagerDefinitionResponseTypeDef](./type_defs.md#describealertmanagerdefinitionresponsetypedef) 


```python
# describe_alert_manager_definition method usage example with argument unpacking

kwargs: DescribeAlertManagerDefinitionRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.describe_alert_manager_definition(**kwargs)
```

1. See [:material-code-braces: DescribeAlertManagerDefinitionRequestRequestTypeDef](./type_defs.md#describealertmanagerdefinitionrequestrequesttypedef) 

### describe\_logging\_configuration

Returns complete information about the current logging configuration of the
workspace.

Type annotations and code completion for `#!python session.create_client("amp").describe_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.describe_logging_configuration)

```python
# describe_logging_configuration method definition

await def describe_logging_configuration(
    self,
    *,
    workspaceId: str,
) -> DescribeLoggingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLoggingConfigurationResponseTypeDef](./type_defs.md#describeloggingconfigurationresponsetypedef) 


```python
# describe_logging_configuration method usage example with argument unpacking

kwargs: DescribeLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.describe_logging_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeLoggingConfigurationRequestRequestTypeDef](./type_defs.md#describeloggingconfigurationrequestrequesttypedef) 

### describe\_rule\_groups\_namespace

Returns complete information about one rule groups namespace.

Type annotations and code completion for `#!python session.create_client("amp").describe_rule_groups_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.describe_rule_groups_namespace)

```python
# describe_rule_groups_namespace method definition

await def describe_rule_groups_namespace(
    self,
    *,
    name: str,
    workspaceId: str,
) -> DescribeRuleGroupsNamespaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRuleGroupsNamespaceResponseTypeDef](./type_defs.md#describerulegroupsnamespaceresponsetypedef) 


```python
# describe_rule_groups_namespace method usage example with argument unpacking

kwargs: DescribeRuleGroupsNamespaceRequestRequestTypeDef = {  # (1)
    "name": ...,
    "workspaceId": ...,
}

parent.describe_rule_groups_namespace(**kwargs)
```

1. See [:material-code-braces: DescribeRuleGroupsNamespaceRequestRequestTypeDef](./type_defs.md#describerulegroupsnamespacerequestrequesttypedef) 

### describe\_scraper

The `DescribeScraper` operation displays information about an existing scraper.

Type annotations and code completion for `#!python session.create_client("amp").describe_scraper` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.describe_scraper)

```python
# describe_scraper method definition

await def describe_scraper(
    self,
    *,
    scraperId: str,
) -> DescribeScraperResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeScraperResponseTypeDef](./type_defs.md#describescraperresponsetypedef) 


```python
# describe_scraper method usage example with argument unpacking

kwargs: DescribeScraperRequestRequestTypeDef = {  # (1)
    "scraperId": ...,
}

parent.describe_scraper(**kwargs)
```

1. See [:material-code-braces: DescribeScraperRequestRequestTypeDef](./type_defs.md#describescraperrequestrequesttypedef) 

### describe\_workspace

Returns information about an existing workspace.

Type annotations and code completion for `#!python session.create_client("amp").describe_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.describe_workspace)

```python
# describe_workspace method definition

await def describe_workspace(
    self,
    *,
    workspaceId: str,
) -> DescribeWorkspaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkspaceResponseTypeDef](./type_defs.md#describeworkspaceresponsetypedef) 


```python
# describe_workspace method usage example with argument unpacking

kwargs: DescribeWorkspaceRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.describe_workspace(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceRequestRequestTypeDef](./type_defs.md#describeworkspacerequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("amp").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.generate_presigned_url)

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


### get\_default\_scraper\_configuration

The `GetDefaultScraperConfiguration` operation returns the default scraper
configuration used when Amazon EKS creates a scraper for
you.

Type annotations and code completion for `#!python session.create_client("amp").get_default_scraper_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.get_default_scraper_configuration)

```python
# get_default_scraper_configuration method definition

await def get_default_scraper_configuration(
    self,
) -> GetDefaultScraperConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDefaultScraperConfigurationResponseTypeDef](./type_defs.md#getdefaultscraperconfigurationresponsetypedef) 

### list\_rule\_groups\_namespaces

Returns a list of rule groups namespaces in a workspace.

Type annotations and code completion for `#!python session.create_client("amp").list_rule_groups_namespaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_rule_groups_namespaces)

```python
# list_rule_groups_namespaces method definition

await def list_rule_groups_namespaces(
    self,
    *,
    workspaceId: str,
    maxResults: int = ...,
    name: str = ...,
    nextToken: str = ...,
) -> ListRuleGroupsNamespacesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRuleGroupsNamespacesResponseTypeDef](./type_defs.md#listrulegroupsnamespacesresponsetypedef) 


```python
# list_rule_groups_namespaces method usage example with argument unpacking

kwargs: ListRuleGroupsNamespacesRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.list_rule_groups_namespaces(**kwargs)
```

1. See [:material-code-braces: ListRuleGroupsNamespacesRequestRequestTypeDef](./type_defs.md#listrulegroupsnamespacesrequestrequesttypedef) 

### list\_scrapers

The `ListScrapers` operation lists all of the scrapers in your account.

Type annotations and code completion for `#!python session.create_client("amp").list_scrapers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_scrapers)

```python
# list_scrapers method definition

await def list_scrapers(
    self,
    *,
    filters: Mapping[str, Sequence[str]] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListScrapersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListScrapersResponseTypeDef](./type_defs.md#listscrapersresponsetypedef) 


```python
# list_scrapers method usage example with argument unpacking

kwargs: ListScrapersRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_scrapers(**kwargs)
```

1. See [:material-code-braces: ListScrapersRequestRequestTypeDef](./type_defs.md#listscrapersrequestrequesttypedef) 

### list\_tags\_for\_resource

The `ListTagsForResource` operation returns the tags that are associated with
an Amazon Managed Service for Prometheus
resource.

Type annotations and code completion for `#!python session.create_client("amp").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_tags_for_resource)

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

### list\_workspaces

Lists all of the Amazon Managed Service for Prometheus workspaces in your
account.

Type annotations and code completion for `#!python session.create_client("amp").list_workspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_workspaces)

```python
# list_workspaces method definition

await def list_workspaces(
    self,
    *,
    alias: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkspacesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef) 


```python
# list_workspaces method usage example with argument unpacking

kwargs: ListWorkspacesRequestRequestTypeDef = {  # (1)
    "alias": ...,
}

parent.list_workspaces(**kwargs)
```

1. See [:material-code-braces: ListWorkspacesRequestRequestTypeDef](./type_defs.md#listworkspacesrequestrequesttypedef) 

### put\_alert\_manager\_definition

Updates an existing alert manager definition in a workspace.

Type annotations and code completion for `#!python session.create_client("amp").put_alert_manager_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_alert_manager_definition)

```python
# put_alert_manager_definition method definition

await def put_alert_manager_definition(
    self,
    *,
    data: BlobTypeDef,
    workspaceId: str,
    clientToken: str = ...,
) -> PutAlertManagerDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutAlertManagerDefinitionResponseTypeDef](./type_defs.md#putalertmanagerdefinitionresponsetypedef) 


```python
# put_alert_manager_definition method usage example with argument unpacking

kwargs: PutAlertManagerDefinitionRequestRequestTypeDef = {  # (1)
    "data": ...,
    "workspaceId": ...,
}

parent.put_alert_manager_definition(**kwargs)
```

1. See [:material-code-braces: PutAlertManagerDefinitionRequestRequestTypeDef](./type_defs.md#putalertmanagerdefinitionrequestrequesttypedef) 

### put\_rule\_groups\_namespace

Updates an existing rule groups namespace within a workspace.

Type annotations and code completion for `#!python session.create_client("amp").put_rule_groups_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_rule_groups_namespace)

```python
# put_rule_groups_namespace method definition

await def put_rule_groups_namespace(
    self,
    *,
    data: BlobTypeDef,
    name: str,
    workspaceId: str,
    clientToken: str = ...,
) -> PutRuleGroupsNamespaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutRuleGroupsNamespaceResponseTypeDef](./type_defs.md#putrulegroupsnamespaceresponsetypedef) 


```python
# put_rule_groups_namespace method usage example with argument unpacking

kwargs: PutRuleGroupsNamespaceRequestRequestTypeDef = {  # (1)
    "data": ...,
    "name": ...,
    "workspaceId": ...,
}

parent.put_rule_groups_namespace(**kwargs)
```

1. See [:material-code-braces: PutRuleGroupsNamespaceRequestRequestTypeDef](./type_defs.md#putrulegroupsnamespacerequestrequesttypedef) 

### tag\_resource

The `TagResource` operation associates tags with an Amazon Managed Service for
Prometheus
resource.

Type annotations and code completion for `#!python session.create_client("amp").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.tag_resource)

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

Removes the specified tags from an Amazon Managed Service for Prometheus
resource.

Type annotations and code completion for `#!python session.create_client("amp").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.untag_resource)

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

### update\_logging\_configuration

Updates the log group ARN or the workspace ID of the current logging
configuration.

Type annotations and code completion for `#!python session.create_client("amp").update_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.update_logging_configuration)

```python
# update_logging_configuration method definition

await def update_logging_configuration(
    self,
    *,
    logGroupArn: str,
    workspaceId: str,
    clientToken: str = ...,
) -> UpdateLoggingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateLoggingConfigurationResponseTypeDef](./type_defs.md#updateloggingconfigurationresponsetypedef) 


```python
# update_logging_configuration method usage example with argument unpacking

kwargs: UpdateLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "logGroupArn": ...,
    "workspaceId": ...,
}

parent.update_logging_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateLoggingConfigurationRequestRequestTypeDef](./type_defs.md#updateloggingconfigurationrequestrequesttypedef) 

### update\_workspace\_alias

Updates the alias of an existing workspace.

Type annotations and code completion for `#!python session.create_client("amp").update_workspace_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.update_workspace_alias)

```python
# update_workspace_alias method definition

await def update_workspace_alias(
    self,
    *,
    workspaceId: str,
    alias: str = ...,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_workspace_alias method usage example with argument unpacking

kwargs: UpdateWorkspaceAliasRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.update_workspace_alias(**kwargs)
```

1. See [:material-code-braces: UpdateWorkspaceAliasRequestRequestTypeDef](./type_defs.md#updateworkspacealiasrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("amp").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "PrometheusServiceClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("amp").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("amp").get_paginator` method with overloads.

- `client.get_paginator("list_rule_groups_namespaces")` -> [ListRuleGroupsNamespacesPaginator](./paginators.md#listrulegroupsnamespacespaginator)
- `client.get_paginator("list_scrapers")` -> [ListScrapersPaginator](./paginators.md#listscraperspaginator)
- `client.get_paginator("list_workspaces")` -> [ListWorkspacesPaginator](./paginators.md#listworkspacespaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("amp").get_waiter` method with overloads.

- `client.get_waiter("scraper_active")` -> [ScraperActiveWaiter](./waiters.md#scraperactivewaiter)
- `client.get_waiter("scraper_deleted")` -> [ScraperDeletedWaiter](./waiters.md#scraperdeletedwaiter)
- `client.get_waiter("workspace_active")` -> [WorkspaceActiveWaiter](./waiters.md#workspaceactivewaiter)
- `client.get_waiter("workspace_deleted")` -> [WorkspaceDeletedWaiter](./waiters.md#workspacedeletedwaiter)

