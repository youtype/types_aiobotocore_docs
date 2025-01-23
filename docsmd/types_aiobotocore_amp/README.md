# PrometheusService module

> [Index](../README.md) > PrometheusService


!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#prometheusservice)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `PrometheusService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `PrometheusService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[amp]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[amp]'

# standalone installation
python -m pip install types-aiobotocore-amp
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-amp
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PrometheusServiceClient

Type annotations and code completion for  `#!python session.create_client("amp")` as [PrometheusServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client)

```python
# PrometheusServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_amp.client import PrometheusServiceClient


session = get_session()
async with session.create_client("amp") as client:
    client: PrometheusServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("amp").get_paginator("...")`.

```python
# ListRuleGroupsNamespacesPaginator usage example

from types_aiobotocore_amp.paginator import ListRuleGroupsNamespacesPaginator

def get_list_rule_groups_namespaces_paginator() -> ListRuleGroupsNamespacesPaginator:
    return client.get_paginator("list_rule_groups_namespaces"))
```

- [ListRuleGroupsNamespacesPaginator](./paginators.md#listrulegroupsnamespacespaginator)
- [ListScrapersPaginator](./paginators.md#listscraperspaginator)
- [ListWorkspacesPaginator](./paginators.md#listworkspacespaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("amp").get_waiter("...")`.

```python
# ScraperActiveWaiter usage example

from types_aiobotocore_amp.waiter import ScraperActiveWaiter

def get_scraper_active_waiter() -> ScraperActiveWaiter:
    return Session().client("amp").get_waiter("scraper_active")
```

- [ScraperActiveWaiter](./waiters.md#scraperactivewaiter)
- [ScraperDeletedWaiter](./waiters.md#scraperdeletedwaiter)
- [WorkspaceActiveWaiter](./waiters.md#workspaceactivewaiter)
- [WorkspaceDeletedWaiter](./waiters.md#workspacedeletedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AlertManagerDefinitionStatusCodeType usage example

from types_aiobotocore_amp.literals import AlertManagerDefinitionStatusCodeType

def get_value() -> AlertManagerDefinitionStatusCodeType:
    return "ACTIVE"
```

- [AlertManagerDefinitionStatusCodeType](./literals.md#alertmanagerdefinitionstatuscodetype)
- [ListRuleGroupsNamespacesPaginatorName](./literals.md#listrulegroupsnamespacespaginatorname)
- [ListScrapersPaginatorName](./literals.md#listscraperspaginatorname)
- [ListWorkspacesPaginatorName](./literals.md#listworkspacespaginatorname)
- [LoggingConfigurationStatusCodeType](./literals.md#loggingconfigurationstatuscodetype)
- [RuleGroupsNamespaceStatusCodeType](./literals.md#rulegroupsnamespacestatuscodetype)
- [ScraperActiveWaiterName](./literals.md#scraperactivewaitername)
- [ScraperDeletedWaiterName](./literals.md#scraperdeletedwaitername)
- [ScraperStatusCodeType](./literals.md#scraperstatuscodetype)
- [WorkspaceActiveWaiterName](./literals.md#workspaceactivewaitername)
- [WorkspaceDeletedWaiterName](./literals.md#workspacedeletedwaitername)
- [WorkspaceStatusCodeType](./literals.md#workspacestatuscodetype)
- [PrometheusServiceServiceName](./literals.md#prometheusserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AlertManagerDefinitionStatusTypeDef](./type_defs.md#alertmanagerdefinitionstatustypedef)
- [AmpConfigurationTypeDef](./type_defs.md#ampconfigurationtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateLoggingConfigurationRequestRequestTypeDef](./type_defs.md#createloggingconfigurationrequestrequesttypedef)
- [LoggingConfigurationStatusTypeDef](./type_defs.md#loggingconfigurationstatustypedef)
- [RuleGroupsNamespaceStatusTypeDef](./type_defs.md#rulegroupsnamespacestatustypedef)
- [ScraperStatusTypeDef](./type_defs.md#scraperstatustypedef)
- [CreateWorkspaceRequestRequestTypeDef](./type_defs.md#createworkspacerequestrequesttypedef)
- [WorkspaceStatusTypeDef](./type_defs.md#workspacestatustypedef)
- [DeleteAlertManagerDefinitionRequestRequestTypeDef](./type_defs.md#deletealertmanagerdefinitionrequestrequesttypedef)
- [DeleteLoggingConfigurationRequestRequestTypeDef](./type_defs.md#deleteloggingconfigurationrequestrequesttypedef)
- [DeleteRuleGroupsNamespaceRequestRequestTypeDef](./type_defs.md#deleterulegroupsnamespacerequestrequesttypedef)
- [DeleteScraperRequestRequestTypeDef](./type_defs.md#deletescraperrequestrequesttypedef)
- [DeleteWorkspaceRequestRequestTypeDef](./type_defs.md#deleteworkspacerequestrequesttypedef)
- [DescribeAlertManagerDefinitionRequestRequestTypeDef](./type_defs.md#describealertmanagerdefinitionrequestrequesttypedef)
- [DescribeLoggingConfigurationRequestRequestTypeDef](./type_defs.md#describeloggingconfigurationrequestrequesttypedef)
- [DescribeRuleGroupsNamespaceRequestRequestTypeDef](./type_defs.md#describerulegroupsnamespacerequestrequesttypedef)
- [DescribeScraperRequestRequestTypeDef](./type_defs.md#describescraperrequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeWorkspaceRequestRequestTypeDef](./type_defs.md#describeworkspacerequestrequesttypedef)
- [EksConfigurationOutputTypeDef](./type_defs.md#eksconfigurationoutputtypedef)
- [EksConfigurationTypeDef](./type_defs.md#eksconfigurationtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListRuleGroupsNamespacesRequestRequestTypeDef](./type_defs.md#listrulegroupsnamespacesrequestrequesttypedef)
- [ListScrapersRequestRequestTypeDef](./type_defs.md#listscrapersrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWorkspacesRequestRequestTypeDef](./type_defs.md#listworkspacesrequestrequesttypedef)
- [ScrapeConfigurationOutputTypeDef](./type_defs.md#scrapeconfigurationoutputtypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateLoggingConfigurationRequestRequestTypeDef](./type_defs.md#updateloggingconfigurationrequestrequesttypedef)
- [UpdateWorkspaceAliasRequestRequestTypeDef](./type_defs.md#updateworkspacealiasrequestrequesttypedef)
- [AlertManagerDefinitionDescriptionTypeDef](./type_defs.md#alertmanagerdefinitiondescriptiontypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [CreateAlertManagerDefinitionRequestRequestTypeDef](./type_defs.md#createalertmanagerdefinitionrequestrequesttypedef)
- [CreateRuleGroupsNamespaceRequestRequestTypeDef](./type_defs.md#createrulegroupsnamespacerequestrequesttypedef)
- [PutAlertManagerDefinitionRequestRequestTypeDef](./type_defs.md#putalertmanagerdefinitionrequestrequesttypedef)
- [PutRuleGroupsNamespaceRequestRequestTypeDef](./type_defs.md#putrulegroupsnamespacerequestrequesttypedef)
- [ScrapeConfigurationTypeDef](./type_defs.md#scrapeconfigurationtypedef)
- [CreateAlertManagerDefinitionResponseTypeDef](./type_defs.md#createalertmanagerdefinitionresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetDefaultScraperConfigurationResponseTypeDef](./type_defs.md#getdefaultscraperconfigurationresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutAlertManagerDefinitionResponseTypeDef](./type_defs.md#putalertmanagerdefinitionresponsetypedef)
- [CreateLoggingConfigurationResponseTypeDef](./type_defs.md#createloggingconfigurationresponsetypedef)
- [LoggingConfigurationMetadataTypeDef](./type_defs.md#loggingconfigurationmetadatatypedef)
- [UpdateLoggingConfigurationResponseTypeDef](./type_defs.md#updateloggingconfigurationresponsetypedef)
- [CreateRuleGroupsNamespaceResponseTypeDef](./type_defs.md#createrulegroupsnamespaceresponsetypedef)
- [PutRuleGroupsNamespaceResponseTypeDef](./type_defs.md#putrulegroupsnamespaceresponsetypedef)
- [RuleGroupsNamespaceDescriptionTypeDef](./type_defs.md#rulegroupsnamespacedescriptiontypedef)
- [RuleGroupsNamespaceSummaryTypeDef](./type_defs.md#rulegroupsnamespacesummarytypedef)
- [CreateScraperResponseTypeDef](./type_defs.md#createscraperresponsetypedef)
- [DeleteScraperResponseTypeDef](./type_defs.md#deletescraperresponsetypedef)
- [UpdateScraperResponseTypeDef](./type_defs.md#updatescraperresponsetypedef)
- [CreateWorkspaceResponseTypeDef](./type_defs.md#createworkspaceresponsetypedef)
- [WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef)
- [WorkspaceSummaryTypeDef](./type_defs.md#workspacesummarytypedef)
- [DescribeScraperRequestWaitTypeDef](./type_defs.md#describescraperrequestwaittypedef)
- [DescribeWorkspaceRequestWaitTypeDef](./type_defs.md#describeworkspacerequestwaittypedef)
- [SourceOutputTypeDef](./type_defs.md#sourceoutputtypedef)
- [EksConfigurationUnionTypeDef](./type_defs.md#eksconfigurationuniontypedef)
- [ListRuleGroupsNamespacesRequestPaginateTypeDef](./type_defs.md#listrulegroupsnamespacesrequestpaginatetypedef)
- [ListScrapersRequestPaginateTypeDef](./type_defs.md#listscrapersrequestpaginatetypedef)
- [ListWorkspacesRequestPaginateTypeDef](./type_defs.md#listworkspacesrequestpaginatetypedef)
- [DescribeAlertManagerDefinitionResponseTypeDef](./type_defs.md#describealertmanagerdefinitionresponsetypedef)
- [UpdateScraperRequestRequestTypeDef](./type_defs.md#updatescraperrequestrequesttypedef)
- [DescribeLoggingConfigurationResponseTypeDef](./type_defs.md#describeloggingconfigurationresponsetypedef)
- [DescribeRuleGroupsNamespaceResponseTypeDef](./type_defs.md#describerulegroupsnamespaceresponsetypedef)
- [ListRuleGroupsNamespacesResponseTypeDef](./type_defs.md#listrulegroupsnamespacesresponsetypedef)
- [DescribeWorkspaceResponseTypeDef](./type_defs.md#describeworkspaceresponsetypedef)
- [ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef)
- [ScraperDescriptionTypeDef](./type_defs.md#scraperdescriptiontypedef)
- [ScraperSummaryTypeDef](./type_defs.md#scrapersummarytypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [DescribeScraperResponseTypeDef](./type_defs.md#describescraperresponsetypedef)
- [ListScrapersResponseTypeDef](./type_defs.md#listscrapersresponsetypedef)
- [CreateScraperRequestRequestTypeDef](./type_defs.md#createscraperrequestrequesttypedef)

