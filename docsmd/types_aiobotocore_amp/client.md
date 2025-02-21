# PrometheusServiceClient

> [Index](../README.md) > [PrometheusService](./README.md) > PrometheusServiceClient

!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#prometheusservice)
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



Type annotations and code completion for `#!python session.create_client("amp").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("amp").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/generate_presigned_url.html)

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


### create\_alert\_manager\_definition

The <code>CreateAlertManagerDefinition</code> operation creates the alert
manager definition in a workspace.

Type annotations and code completion for `#!python session.create_client("amp").create_alert_manager_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/create_alert_manager_definition.html)

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

kwargs: CreateAlertManagerDefinitionRequestTypeDef = {  # (1)
    "data": ...,
    "workspaceId": ...,
}

parent.create_alert_manager_definition(**kwargs)
```

1. See [:material-code-braces: CreateAlertManagerDefinitionRequestTypeDef](./type_defs.md#createalertmanagerdefinitionrequesttypedef) 

### create\_logging\_configuration

The <code>CreateLoggingConfiguration</code> operation creates a logging
configuration for the workspace.

Type annotations and code completion for `#!python session.create_client("amp").create_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/create_logging_configuration.html)

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

kwargs: CreateLoggingConfigurationRequestTypeDef = {  # (1)
    "logGroupArn": ...,
    "workspaceId": ...,
}

parent.create_logging_configuration(**kwargs)
```

1. See [:material-code-braces: CreateLoggingConfigurationRequestTypeDef](./type_defs.md#createloggingconfigurationrequesttypedef) 

### create\_rule\_groups\_namespace

The <code>CreateRuleGroupsNamespace</code> operation creates a rule groups
namespace within a workspace.

Type annotations and code completion for `#!python session.create_client("amp").create_rule_groups_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/create_rule_groups_namespace.html)

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

kwargs: CreateRuleGroupsNamespaceRequestTypeDef = {  # (1)
    "data": ...,
    "name": ...,
    "workspaceId": ...,
}

parent.create_rule_groups_namespace(**kwargs)
```

1. See [:material-code-braces: CreateRuleGroupsNamespaceRequestTypeDef](./type_defs.md#createrulegroupsnamespacerequesttypedef) 

### create\_scraper

The <code>CreateScraper</code> operation creates a scraper to collect metrics.

Type annotations and code completion for `#!python session.create_client("amp").create_scraper` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/create_scraper.html)

```python
# create_scraper method definition

await def create_scraper(
    self,
    *,
    destination: DestinationTypeDef,  # (1)
    scrapeConfiguration: ScrapeConfigurationUnionTypeDef,  # (2)
    source: SourceUnionTypeDef,  # (3)
    alias: str = ...,
    clientToken: str = ...,
    roleConfiguration: RoleConfigurationTypeDef = ...,  # (4)
    tags: Mapping[str, str] = ...,
) -> CreateScraperResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: ScrapeConfigurationTypeDef](./type_defs.md#scrapeconfigurationtypedef) [:material-code-braces: ScrapeConfigurationOutputTypeDef](./type_defs.md#scrapeconfigurationoutputtypedef) 
3. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) [:material-code-braces: SourceOutputTypeDef](./type_defs.md#sourceoutputtypedef) 
4. See [:material-code-braces: RoleConfigurationTypeDef](./type_defs.md#roleconfigurationtypedef) 
5. See [:material-code-braces: CreateScraperResponseTypeDef](./type_defs.md#createscraperresponsetypedef) 


```python
# create_scraper method usage example with argument unpacking

kwargs: CreateScraperRequestTypeDef = {  # (1)
    "destination": ...,
    "scrapeConfiguration": ...,
    "source": ...,
}

parent.create_scraper(**kwargs)
```

1. See [:material-code-braces: CreateScraperRequestTypeDef](./type_defs.md#createscraperrequesttypedef) 

### create\_workspace

Creates a Prometheus workspace.

Type annotations and code completion for `#!python session.create_client("amp").create_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/create_workspace.html)

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

kwargs: CreateWorkspaceRequestTypeDef = {  # (1)
    "alias": ...,
}

parent.create_workspace(**kwargs)
```

1. See [:material-code-braces: CreateWorkspaceRequestTypeDef](./type_defs.md#createworkspacerequesttypedef) 

### delete\_alert\_manager\_definition

Deletes the alert manager definition from a workspace.

Type annotations and code completion for `#!python session.create_client("amp").delete_alert_manager_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/delete_alert_manager_definition.html)

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

kwargs: DeleteAlertManagerDefinitionRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.delete_alert_manager_definition(**kwargs)
```

1. See [:material-code-braces: DeleteAlertManagerDefinitionRequestTypeDef](./type_defs.md#deletealertmanagerdefinitionrequesttypedef) 

### delete\_logging\_configuration

Deletes the logging configuration for a workspace.

Type annotations and code completion for `#!python session.create_client("amp").delete_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/delete_logging_configuration.html)

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

kwargs: DeleteLoggingConfigurationRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.delete_logging_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteLoggingConfigurationRequestTypeDef](./type_defs.md#deleteloggingconfigurationrequesttypedef) 

### delete\_rule\_groups\_namespace

Deletes one rule groups namespace and its associated rule groups definition.

Type annotations and code completion for `#!python session.create_client("amp").delete_rule_groups_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/delete_rule_groups_namespace.html)

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

kwargs: DeleteRuleGroupsNamespaceRequestTypeDef = {  # (1)
    "name": ...,
    "workspaceId": ...,
}

parent.delete_rule_groups_namespace(**kwargs)
```

1. See [:material-code-braces: DeleteRuleGroupsNamespaceRequestTypeDef](./type_defs.md#deleterulegroupsnamespacerequesttypedef) 

### delete\_scraper

The <code>DeleteScraper</code> operation deletes one scraper, and stops any
metrics collection that the scraper performs.

Type annotations and code completion for `#!python session.create_client("amp").delete_scraper` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/delete_scraper.html)

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

kwargs: DeleteScraperRequestTypeDef = {  # (1)
    "scraperId": ...,
}

parent.delete_scraper(**kwargs)
```

1. See [:material-code-braces: DeleteScraperRequestTypeDef](./type_defs.md#deletescraperrequesttypedef) 

### delete\_workspace

Deletes an existing workspace.

Type annotations and code completion for `#!python session.create_client("amp").delete_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/delete_workspace.html)

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

kwargs: DeleteWorkspaceRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.delete_workspace(**kwargs)
```

1. See [:material-code-braces: DeleteWorkspaceRequestTypeDef](./type_defs.md#deleteworkspacerequesttypedef) 

### describe\_alert\_manager\_definition

Retrieves the full information about the alert manager definition for a
workspace.

Type annotations and code completion for `#!python session.create_client("amp").describe_alert_manager_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/describe_alert_manager_definition.html)

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

kwargs: DescribeAlertManagerDefinitionRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.describe_alert_manager_definition(**kwargs)
```

1. See [:material-code-braces: DescribeAlertManagerDefinitionRequestTypeDef](./type_defs.md#describealertmanagerdefinitionrequesttypedef) 

### describe\_logging\_configuration

Returns complete information about the current logging configuration of the
workspace.

Type annotations and code completion for `#!python session.create_client("amp").describe_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/describe_logging_configuration.html)

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

kwargs: DescribeLoggingConfigurationRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.describe_logging_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeLoggingConfigurationRequestTypeDef](./type_defs.md#describeloggingconfigurationrequesttypedef) 

### describe\_rule\_groups\_namespace

Returns complete information about one rule groups namespace.

Type annotations and code completion for `#!python session.create_client("amp").describe_rule_groups_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/describe_rule_groups_namespace.html)

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

kwargs: DescribeRuleGroupsNamespaceRequestTypeDef = {  # (1)
    "name": ...,
    "workspaceId": ...,
}

parent.describe_rule_groups_namespace(**kwargs)
```

1. See [:material-code-braces: DescribeRuleGroupsNamespaceRequestTypeDef](./type_defs.md#describerulegroupsnamespacerequesttypedef) 

### describe\_scraper

The <code>DescribeScraper</code> operation displays information about an
existing scraper.

Type annotations and code completion for `#!python session.create_client("amp").describe_scraper` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/describe_scraper.html)

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

kwargs: DescribeScraperRequestTypeDef = {  # (1)
    "scraperId": ...,
}

parent.describe_scraper(**kwargs)
```

1. See [:material-code-braces: DescribeScraperRequestTypeDef](./type_defs.md#describescraperrequesttypedef) 

### describe\_workspace

Returns information about an existing workspace.

Type annotations and code completion for `#!python session.create_client("amp").describe_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/describe_workspace.html)

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

kwargs: DescribeWorkspaceRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.describe_workspace(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceRequestTypeDef](./type_defs.md#describeworkspacerequesttypedef) 

### get\_default\_scraper\_configuration

The <code>GetDefaultScraperConfiguration</code> operation returns the default
scraper configuration used when Amazon EKS creates a scraper for you.

Type annotations and code completion for `#!python session.create_client("amp").get_default_scraper_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/get_default_scraper_configuration.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/list_rule_groups_namespaces.html)

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

kwargs: ListRuleGroupsNamespacesRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.list_rule_groups_namespaces(**kwargs)
```

1. See [:material-code-braces: ListRuleGroupsNamespacesRequestTypeDef](./type_defs.md#listrulegroupsnamespacesrequesttypedef) 

### list\_scrapers

The <code>ListScrapers</code> operation lists all of the scrapers in your
account.

Type annotations and code completion for `#!python session.create_client("amp").list_scrapers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/list_scrapers.html)

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

kwargs: ListScrapersRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_scrapers(**kwargs)
```

1. See [:material-code-braces: ListScrapersRequestTypeDef](./type_defs.md#listscrapersrequesttypedef) 

### list\_tags\_for\_resource

The <code>ListTagsForResource</code> operation returns the tags that are
associated with an Amazon Managed Service for Prometheus resource.

Type annotations and code completion for `#!python session.create_client("amp").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/list_tags_for_resource.html)

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

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### list\_workspaces

Lists all of the Amazon Managed Service for Prometheus workspaces in your
account.

Type annotations and code completion for `#!python session.create_client("amp").list_workspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/list_workspaces.html)

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

kwargs: ListWorkspacesRequestTypeDef = {  # (1)
    "alias": ...,
}

parent.list_workspaces(**kwargs)
```

1. See [:material-code-braces: ListWorkspacesRequestTypeDef](./type_defs.md#listworkspacesrequesttypedef) 

### put\_alert\_manager\_definition

Updates an existing alert manager definition in a workspace.

Type annotations and code completion for `#!python session.create_client("amp").put_alert_manager_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/put_alert_manager_definition.html)

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

kwargs: PutAlertManagerDefinitionRequestTypeDef = {  # (1)
    "data": ...,
    "workspaceId": ...,
}

parent.put_alert_manager_definition(**kwargs)
```

1. See [:material-code-braces: PutAlertManagerDefinitionRequestTypeDef](./type_defs.md#putalertmanagerdefinitionrequesttypedef) 

### put\_rule\_groups\_namespace

Updates an existing rule groups namespace within a workspace.

Type annotations and code completion for `#!python session.create_client("amp").put_rule_groups_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/put_rule_groups_namespace.html)

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

kwargs: PutRuleGroupsNamespaceRequestTypeDef = {  # (1)
    "data": ...,
    "name": ...,
    "workspaceId": ...,
}

parent.put_rule_groups_namespace(**kwargs)
```

1. See [:material-code-braces: PutRuleGroupsNamespaceRequestTypeDef](./type_defs.md#putrulegroupsnamespacerequesttypedef) 

### tag\_resource

The <code>TagResource</code> operation associates tags with an Amazon Managed
Service for Prometheus resource.

Type annotations and code completion for `#!python session.create_client("amp").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/tag_resource.html)

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

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes the specified tags from an Amazon Managed Service for Prometheus
resource.

Type annotations and code completion for `#!python session.create_client("amp").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/untag_resource.html)

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

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_logging\_configuration

Updates the log group ARN or the workspace ID of the current logging
configuration.

Type annotations and code completion for `#!python session.create_client("amp").update_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/update_logging_configuration.html)

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

kwargs: UpdateLoggingConfigurationRequestTypeDef = {  # (1)
    "logGroupArn": ...,
    "workspaceId": ...,
}

parent.update_logging_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateLoggingConfigurationRequestTypeDef](./type_defs.md#updateloggingconfigurationrequesttypedef) 

### update\_scraper

Updates an existing scraper.

Type annotations and code completion for `#!python session.create_client("amp").update_scraper` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/update_scraper.html)

```python
# update_scraper method definition

await def update_scraper(
    self,
    *,
    scraperId: str,
    alias: str = ...,
    clientToken: str = ...,
    destination: DestinationTypeDef = ...,  # (1)
    roleConfiguration: RoleConfigurationTypeDef = ...,  # (2)
    scrapeConfiguration: ScrapeConfigurationUnionTypeDef = ...,  # (3)
) -> UpdateScraperResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: RoleConfigurationTypeDef](./type_defs.md#roleconfigurationtypedef) 
3. See [:material-code-braces: ScrapeConfigurationTypeDef](./type_defs.md#scrapeconfigurationtypedef) [:material-code-braces: ScrapeConfigurationOutputTypeDef](./type_defs.md#scrapeconfigurationoutputtypedef) 
4. See [:material-code-braces: UpdateScraperResponseTypeDef](./type_defs.md#updatescraperresponsetypedef) 


```python
# update_scraper method usage example with argument unpacking

kwargs: UpdateScraperRequestTypeDef = {  # (1)
    "scraperId": ...,
}

parent.update_scraper(**kwargs)
```

1. See [:material-code-braces: UpdateScraperRequestTypeDef](./type_defs.md#updatescraperrequesttypedef) 

### update\_workspace\_alias

Updates the alias of an existing workspace.

Type annotations and code completion for `#!python session.create_client("amp").update_workspace_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/client/update_workspace_alias.html)

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

kwargs: UpdateWorkspaceAliasRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.update_workspace_alias(**kwargs)
```

1. See [:material-code-braces: UpdateWorkspaceAliasRequestTypeDef](./type_defs.md#updateworkspacealiasrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("amp").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("amp").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client)

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

