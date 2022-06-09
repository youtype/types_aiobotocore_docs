# PrometheusService module

> [Index](../README.md) > PrometheusService


!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `PrometheusService`.

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

```python title="Usage example"
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

```python title="Usage example"
from types_aiobotocore_amp.paginator import ListRuleGroupsNamespacesPaginator

def get_list_rule_groups_namespaces_paginator() -> ListRuleGroupsNamespacesPaginator:
    return client.get_paginator("list_rule_groups_namespaces"))
```

- [ListRuleGroupsNamespacesPaginator](./paginators.md#listrulegroupsnamespacespaginator)
- [ListWorkspacesPaginator](./paginators.md#listworkspacespaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("amp").get_waiter("...")`.

```python title="Usage example"
from types_aiobotocore_amp.waiter import WorkspaceActiveWaiter

def get_workspace_active_waiter() -> WorkspaceActiveWaiter:
    return Session().client("amp").get_waiter("workspace_active")
```

- [WorkspaceActiveWaiter](./waiters.md#workspaceactivewaiter)
- [WorkspaceDeletedWaiter](./waiters.md#workspacedeletedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_amp.literals import AlertManagerDefinitionStatusCodeType

def get_value() -> AlertManagerDefinitionStatusCodeType:
    return "ACTIVE"
```

- [AlertManagerDefinitionStatusCodeType](./literals.md#alertmanagerdefinitionstatuscodetype)
- [ListRuleGroupsNamespacesPaginatorName](./literals.md#listrulegroupsnamespacespaginatorname)
- [ListWorkspacesPaginatorName](./literals.md#listworkspacespaginatorname)
- [RuleGroupsNamespaceStatusCodeType](./literals.md#rulegroupsnamespacestatuscodetype)
- [WorkspaceActiveWaiterName](./literals.md#workspaceactivewaitername)
- [WorkspaceDeletedWaiterName](./literals.md#workspacedeletedwaitername)
- [WorkspaceStatusCodeType](./literals.md#workspacestatuscodetype)
- [PrometheusServiceServiceName](./literals.md#prometheusserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_amp.type_defs import AlertManagerDefinitionStatusTypeDef

def get_value() -> AlertManagerDefinitionStatusTypeDef:
    return {
        "statusCode": ...,
    }
```

- [AlertManagerDefinitionStatusTypeDef](./type_defs.md#alertmanagerdefinitionstatustypedef)
- [CreateAlertManagerDefinitionRequestRequestTypeDef](./type_defs.md#createalertmanagerdefinitionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateRuleGroupsNamespaceRequestRequestTypeDef](./type_defs.md#createrulegroupsnamespacerequestrequesttypedef)
- [RuleGroupsNamespaceStatusTypeDef](./type_defs.md#rulegroupsnamespacestatustypedef)
- [CreateWorkspaceRequestRequestTypeDef](./type_defs.md#createworkspacerequestrequesttypedef)
- [WorkspaceStatusTypeDef](./type_defs.md#workspacestatustypedef)
- [DeleteAlertManagerDefinitionRequestRequestTypeDef](./type_defs.md#deletealertmanagerdefinitionrequestrequesttypedef)
- [DeleteRuleGroupsNamespaceRequestRequestTypeDef](./type_defs.md#deleterulegroupsnamespacerequestrequesttypedef)
- [DeleteWorkspaceRequestRequestTypeDef](./type_defs.md#deleteworkspacerequestrequesttypedef)
- [DescribeAlertManagerDefinitionRequestRequestTypeDef](./type_defs.md#describealertmanagerdefinitionrequestrequesttypedef)
- [DescribeRuleGroupsNamespaceRequestRequestTypeDef](./type_defs.md#describerulegroupsnamespacerequestrequesttypedef)
- [DescribeWorkspaceRequestRequestTypeDef](./type_defs.md#describeworkspacerequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListRuleGroupsNamespacesRequestRequestTypeDef](./type_defs.md#listrulegroupsnamespacesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWorkspacesRequestRequestTypeDef](./type_defs.md#listworkspacesrequestrequesttypedef)
- [PutAlertManagerDefinitionRequestRequestTypeDef](./type_defs.md#putalertmanagerdefinitionrequestrequesttypedef)
- [PutRuleGroupsNamespaceRequestRequestTypeDef](./type_defs.md#putrulegroupsnamespacerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateWorkspaceAliasRequestRequestTypeDef](./type_defs.md#updateworkspacealiasrequestrequesttypedef)
- [AlertManagerDefinitionDescriptionTypeDef](./type_defs.md#alertmanagerdefinitiondescriptiontypedef)
- [CreateAlertManagerDefinitionResponseTypeDef](./type_defs.md#createalertmanagerdefinitionresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutAlertManagerDefinitionResponseTypeDef](./type_defs.md#putalertmanagerdefinitionresponsetypedef)
- [CreateRuleGroupsNamespaceResponseTypeDef](./type_defs.md#createrulegroupsnamespaceresponsetypedef)
- [PutRuleGroupsNamespaceResponseTypeDef](./type_defs.md#putrulegroupsnamespaceresponsetypedef)
- [RuleGroupsNamespaceDescriptionTypeDef](./type_defs.md#rulegroupsnamespacedescriptiontypedef)
- [RuleGroupsNamespaceSummaryTypeDef](./type_defs.md#rulegroupsnamespacesummarytypedef)
- [CreateWorkspaceResponseTypeDef](./type_defs.md#createworkspaceresponsetypedef)
- [WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef)
- [WorkspaceSummaryTypeDef](./type_defs.md#workspacesummarytypedef)
- [DescribeWorkspaceRequestWorkspaceActiveWaitTypeDef](./type_defs.md#describeworkspacerequestworkspaceactivewaittypedef)
- [DescribeWorkspaceRequestWorkspaceDeletedWaitTypeDef](./type_defs.md#describeworkspacerequestworkspacedeletedwaittypedef)
- [ListRuleGroupsNamespacesRequestListRuleGroupsNamespacesPaginateTypeDef](./type_defs.md#listrulegroupsnamespacesrequestlistrulegroupsnamespacespaginatetypedef)
- [ListWorkspacesRequestListWorkspacesPaginateTypeDef](./type_defs.md#listworkspacesrequestlistworkspacespaginatetypedef)
- [DescribeAlertManagerDefinitionResponseTypeDef](./type_defs.md#describealertmanagerdefinitionresponsetypedef)
- [DescribeRuleGroupsNamespaceResponseTypeDef](./type_defs.md#describerulegroupsnamespaceresponsetypedef)
- [ListRuleGroupsNamespacesResponseTypeDef](./type_defs.md#listrulegroupsnamespacesresponsetypedef)
- [DescribeWorkspaceResponseTypeDef](./type_defs.md#describeworkspaceresponsetypedef)
- [ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef)

