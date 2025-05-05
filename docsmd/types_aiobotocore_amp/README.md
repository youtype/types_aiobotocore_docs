# PrometheusService module

> [Index](../README.md) > PrometheusService


!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#prometheusservice)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.22.0' mypy-boto3-builder`
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
- [WorkspaceConfigurationStatusCodeType](./literals.md#workspaceconfigurationstatuscodetype)
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
- [CreateLoggingConfigurationRequestTypeDef](./type_defs.md#createloggingconfigurationrequesttypedef)
- [LoggingConfigurationStatusTypeDef](./type_defs.md#loggingconfigurationstatustypedef)
- [RuleGroupsNamespaceStatusTypeDef](./type_defs.md#rulegroupsnamespacestatustypedef)
- [RoleConfigurationTypeDef](./type_defs.md#roleconfigurationtypedef)
- [ScraperStatusTypeDef](./type_defs.md#scraperstatustypedef)
- [CreateWorkspaceRequestTypeDef](./type_defs.md#createworkspacerequesttypedef)
- [WorkspaceStatusTypeDef](./type_defs.md#workspacestatustypedef)
- [DeleteAlertManagerDefinitionRequestTypeDef](./type_defs.md#deletealertmanagerdefinitionrequesttypedef)
- [DeleteLoggingConfigurationRequestTypeDef](./type_defs.md#deleteloggingconfigurationrequesttypedef)
- [DeleteRuleGroupsNamespaceRequestTypeDef](./type_defs.md#deleterulegroupsnamespacerequesttypedef)
- [DeleteScraperRequestTypeDef](./type_defs.md#deletescraperrequesttypedef)
- [DeleteWorkspaceRequestTypeDef](./type_defs.md#deleteworkspacerequesttypedef)
- [DescribeAlertManagerDefinitionRequestTypeDef](./type_defs.md#describealertmanagerdefinitionrequesttypedef)
- [DescribeLoggingConfigurationRequestTypeDef](./type_defs.md#describeloggingconfigurationrequesttypedef)
- [DescribeRuleGroupsNamespaceRequestTypeDef](./type_defs.md#describerulegroupsnamespacerequesttypedef)
- [DescribeScraperRequestTypeDef](./type_defs.md#describescraperrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeWorkspaceConfigurationRequestTypeDef](./type_defs.md#describeworkspaceconfigurationrequesttypedef)
- [DescribeWorkspaceRequestTypeDef](./type_defs.md#describeworkspacerequesttypedef)
- [EksConfigurationOutputTypeDef](./type_defs.md#eksconfigurationoutputtypedef)
- [EksConfigurationTypeDef](./type_defs.md#eksconfigurationtypedef)
- [LimitsPerLabelSetEntryTypeDef](./type_defs.md#limitsperlabelsetentrytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListRuleGroupsNamespacesRequestTypeDef](./type_defs.md#listrulegroupsnamespacesrequesttypedef)
- [ListScrapersRequestTypeDef](./type_defs.md#listscrapersrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ListWorkspacesRequestTypeDef](./type_defs.md#listworkspacesrequesttypedef)
- [ScrapeConfigurationOutputTypeDef](./type_defs.md#scrapeconfigurationoutputtypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateLoggingConfigurationRequestTypeDef](./type_defs.md#updateloggingconfigurationrequesttypedef)
- [UpdateWorkspaceAliasRequestTypeDef](./type_defs.md#updateworkspacealiasrequesttypedef)
- [WorkspaceConfigurationStatusTypeDef](./type_defs.md#workspaceconfigurationstatustypedef)
- [AlertManagerDefinitionDescriptionTypeDef](./type_defs.md#alertmanagerdefinitiondescriptiontypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [CreateAlertManagerDefinitionRequestTypeDef](./type_defs.md#createalertmanagerdefinitionrequesttypedef)
- [CreateRuleGroupsNamespaceRequestTypeDef](./type_defs.md#createrulegroupsnamespacerequesttypedef)
- [PutAlertManagerDefinitionRequestTypeDef](./type_defs.md#putalertmanagerdefinitionrequesttypedef)
- [PutRuleGroupsNamespaceRequestTypeDef](./type_defs.md#putrulegroupsnamespacerequesttypedef)
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
- [DescribeScraperRequestWaitExtraTypeDef](./type_defs.md#describescraperrequestwaitextratypedef)
- [DescribeScraperRequestWaitTypeDef](./type_defs.md#describescraperrequestwaittypedef)
- [DescribeWorkspaceRequestWaitExtraTypeDef](./type_defs.md#describeworkspacerequestwaitextratypedef)
- [DescribeWorkspaceRequestWaitTypeDef](./type_defs.md#describeworkspacerequestwaittypedef)
- [SourceOutputTypeDef](./type_defs.md#sourceoutputtypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [LimitsPerLabelSetOutputTypeDef](./type_defs.md#limitsperlabelsetoutputtypedef)
- [LimitsPerLabelSetTypeDef](./type_defs.md#limitsperlabelsettypedef)
- [ListRuleGroupsNamespacesRequestPaginateTypeDef](./type_defs.md#listrulegroupsnamespacesrequestpaginatetypedef)
- [ListScrapersRequestPaginateTypeDef](./type_defs.md#listscrapersrequestpaginatetypedef)
- [ListWorkspacesRequestPaginateTypeDef](./type_defs.md#listworkspacesrequestpaginatetypedef)
- [UpdateWorkspaceConfigurationResponseTypeDef](./type_defs.md#updateworkspaceconfigurationresponsetypedef)
- [DescribeAlertManagerDefinitionResponseTypeDef](./type_defs.md#describealertmanagerdefinitionresponsetypedef)
- [ScrapeConfigurationUnionTypeDef](./type_defs.md#scrapeconfigurationuniontypedef)
- [DescribeLoggingConfigurationResponseTypeDef](./type_defs.md#describeloggingconfigurationresponsetypedef)
- [DescribeRuleGroupsNamespaceResponseTypeDef](./type_defs.md#describerulegroupsnamespaceresponsetypedef)
- [ListRuleGroupsNamespacesResponseTypeDef](./type_defs.md#listrulegroupsnamespacesresponsetypedef)
- [DescribeWorkspaceResponseTypeDef](./type_defs.md#describeworkspaceresponsetypedef)
- [ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef)
- [ScraperDescriptionTypeDef](./type_defs.md#scraperdescriptiontypedef)
- [ScraperSummaryTypeDef](./type_defs.md#scrapersummarytypedef)
- [SourceUnionTypeDef](./type_defs.md#sourceuniontypedef)
- [WorkspaceConfigurationDescriptionTypeDef](./type_defs.md#workspaceconfigurationdescriptiontypedef)
- [LimitsPerLabelSetUnionTypeDef](./type_defs.md#limitsperlabelsetuniontypedef)
- [UpdateScraperRequestTypeDef](./type_defs.md#updatescraperrequesttypedef)
- [DescribeScraperResponseTypeDef](./type_defs.md#describescraperresponsetypedef)
- [ListScrapersResponseTypeDef](./type_defs.md#listscrapersresponsetypedef)
- [CreateScraperRequestTypeDef](./type_defs.md#createscraperrequesttypedef)
- [DescribeWorkspaceConfigurationResponseTypeDef](./type_defs.md#describeworkspaceconfigurationresponsetypedef)
- [UpdateWorkspaceConfigurationRequestTypeDef](./type_defs.md#updateworkspaceconfigurationrequesttypedef)

