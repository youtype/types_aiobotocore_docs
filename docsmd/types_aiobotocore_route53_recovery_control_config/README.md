# Route53RecoveryControlConfig module

> [Index](../README.md) > Route53RecoveryControlConfig


!!! note ""

    Auto-generated documentation for [Route53RecoveryControlConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#route53recoverycontrolconfig)
    type annotations stubs module [types-aiobotocore-route53-recovery-control-config](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Route53RecoveryControlConfig` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Route53RecoveryControlConfig` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[route53-recovery-control-config]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[route53-recovery-control-config]'

# standalone installation
python -m pip install types-aiobotocore-route53-recovery-control-config
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-route53-recovery-control-config
```

## Usage

Code samples can be found in [Examples](./usage.md).

## Route53RecoveryControlConfigClient

Type annotations and code completion for  `#!python session.create_client("route53-recovery-control-config")` as [Route53RecoveryControlConfigClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client)

```python
# Route53RecoveryControlConfigClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53_recovery_control_config.client import Route53RecoveryControlConfigClient


session = get_session()
async with session.create_client("route53-recovery-control-config") as client:
    client: Route53RecoveryControlConfigClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("route53-recovery-control-config").get_paginator("...")`.

```python
# ListAssociatedRoute53HealthChecksPaginator usage example

from types_aiobotocore_route53_recovery_control_config.paginator import ListAssociatedRoute53HealthChecksPaginator

def get_list_associated_route53_health_checks_paginator() -> ListAssociatedRoute53HealthChecksPaginator:
    return client.get_paginator("list_associated_route53_health_checks"))
```

- [ListAssociatedRoute53HealthChecksPaginator](./paginators.md#listassociatedroute53healthcheckspaginator)
- [ListClustersPaginator](./paginators.md#listclusterspaginator)
- [ListControlPanelsPaginator](./paginators.md#listcontrolpanelspaginator)
- [ListRoutingControlsPaginator](./paginators.md#listroutingcontrolspaginator)
- [ListSafetyRulesPaginator](./paginators.md#listsafetyrulespaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("route53-recovery-control-config").get_waiter("...")`.

```python
# ClusterCreatedWaiter usage example

from types_aiobotocore_route53_recovery_control_config.waiter import ClusterCreatedWaiter

def get_cluster_created_waiter() -> ClusterCreatedWaiter:
    return Session().client("route53-recovery-control-config").get_waiter("cluster_created")
```

- [ClusterCreatedWaiter](./waiters.md#clustercreatedwaiter)
- [ClusterDeletedWaiter](./waiters.md#clusterdeletedwaiter)
- [ControlPanelCreatedWaiter](./waiters.md#controlpanelcreatedwaiter)
- [ControlPanelDeletedWaiter](./waiters.md#controlpaneldeletedwaiter)
- [RoutingControlCreatedWaiter](./waiters.md#routingcontrolcreatedwaiter)
- [RoutingControlDeletedWaiter](./waiters.md#routingcontroldeletedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ClusterCreatedWaiterName usage example

from types_aiobotocore_route53_recovery_control_config.literals import ClusterCreatedWaiterName

def get_value() -> ClusterCreatedWaiterName:
    return "cluster_created"
```

- [ClusterCreatedWaiterName](./literals.md#clustercreatedwaitername)
- [ClusterDeletedWaiterName](./literals.md#clusterdeletedwaitername)
- [ControlPanelCreatedWaiterName](./literals.md#controlpanelcreatedwaitername)
- [ControlPanelDeletedWaiterName](./literals.md#controlpaneldeletedwaitername)
- [ListAssociatedRoute53HealthChecksPaginatorName](./literals.md#listassociatedroute53healthcheckspaginatorname)
- [ListClustersPaginatorName](./literals.md#listclusterspaginatorname)
- [ListControlPanelsPaginatorName](./literals.md#listcontrolpanelspaginatorname)
- [ListRoutingControlsPaginatorName](./literals.md#listroutingcontrolspaginatorname)
- [ListSafetyRulesPaginatorName](./literals.md#listsafetyrulespaginatorname)
- [RoutingControlCreatedWaiterName](./literals.md#routingcontrolcreatedwaitername)
- [RoutingControlDeletedWaiterName](./literals.md#routingcontroldeletedwaitername)
- [RuleTypeType](./literals.md#ruletypetype)
- [StatusType](./literals.md#statustype)
- [Route53RecoveryControlConfigServiceName](./literals.md#route53recoverycontrolconfigservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [RuleConfigTypeDef](./type_defs.md#ruleconfigtypedef)
- [AssertionRuleUpdateTypeDef](./type_defs.md#assertionruleupdatetypedef)
- [ClusterEndpointTypeDef](./type_defs.md#clusterendpointtypedef)
- [ControlPanelTypeDef](./type_defs.md#controlpaneltypedef)
- [CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateControlPanelRequestRequestTypeDef](./type_defs.md#createcontrolpanelrequestrequesttypedef)
- [CreateRoutingControlRequestRequestTypeDef](./type_defs.md#createroutingcontrolrequestrequesttypedef)
- [RoutingControlTypeDef](./type_defs.md#routingcontroltypedef)
- [DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef)
- [DeleteControlPanelRequestRequestTypeDef](./type_defs.md#deletecontrolpanelrequestrequesttypedef)
- [DeleteRoutingControlRequestRequestTypeDef](./type_defs.md#deleteroutingcontrolrequestrequesttypedef)
- [DeleteSafetyRuleRequestRequestTypeDef](./type_defs.md#deletesafetyrulerequestrequesttypedef)
- [DescribeClusterRequestRequestTypeDef](./type_defs.md#describeclusterrequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeControlPanelRequestRequestTypeDef](./type_defs.md#describecontrolpanelrequestrequesttypedef)
- [DescribeRoutingControlRequestRequestTypeDef](./type_defs.md#describeroutingcontrolrequestrequesttypedef)
- [DescribeSafetyRuleRequestRequestTypeDef](./type_defs.md#describesafetyrulerequestrequesttypedef)
- [GatingRuleUpdateTypeDef](./type_defs.md#gatingruleupdatetypedef)
- [GetResourcePolicyRequestRequestTypeDef](./type_defs.md#getresourcepolicyrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAssociatedRoute53HealthChecksRequestRequestTypeDef](./type_defs.md#listassociatedroute53healthchecksrequestrequesttypedef)
- [ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef)
- [ListControlPanelsRequestRequestTypeDef](./type_defs.md#listcontrolpanelsrequestrequesttypedef)
- [ListRoutingControlsRequestRequestTypeDef](./type_defs.md#listroutingcontrolsrequestrequesttypedef)
- [ListSafetyRulesRequestRequestTypeDef](./type_defs.md#listsafetyrulesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateControlPanelRequestRequestTypeDef](./type_defs.md#updatecontrolpanelrequestrequesttypedef)
- [UpdateRoutingControlRequestRequestTypeDef](./type_defs.md#updateroutingcontrolrequestrequesttypedef)
- [AssertionRuleTypeDef](./type_defs.md#assertionruletypedef)
- [GatingRuleTypeDef](./type_defs.md#gatingruletypedef)
- [NewAssertionRuleTypeDef](./type_defs.md#newassertionruletypedef)
- [NewGatingRuleTypeDef](./type_defs.md#newgatingruletypedef)
- [ClusterTypeDef](./type_defs.md#clustertypedef)
- [CreateControlPanelResponseTypeDef](./type_defs.md#createcontrolpanelresponsetypedef)
- [DescribeControlPanelResponseTypeDef](./type_defs.md#describecontrolpanelresponsetypedef)
- [GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef)
- [ListAssociatedRoute53HealthChecksResponseTypeDef](./type_defs.md#listassociatedroute53healthchecksresponsetypedef)
- [ListControlPanelsResponseTypeDef](./type_defs.md#listcontrolpanelsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateControlPanelResponseTypeDef](./type_defs.md#updatecontrolpanelresponsetypedef)
- [CreateRoutingControlResponseTypeDef](./type_defs.md#createroutingcontrolresponsetypedef)
- [DescribeRoutingControlResponseTypeDef](./type_defs.md#describeroutingcontrolresponsetypedef)
- [ListRoutingControlsResponseTypeDef](./type_defs.md#listroutingcontrolsresponsetypedef)
- [UpdateRoutingControlResponseTypeDef](./type_defs.md#updateroutingcontrolresponsetypedef)
- [DescribeClusterRequestWaitTypeDef](./type_defs.md#describeclusterrequestwaittypedef)
- [DescribeControlPanelRequestWaitTypeDef](./type_defs.md#describecontrolpanelrequestwaittypedef)
- [DescribeRoutingControlRequestWaitTypeDef](./type_defs.md#describeroutingcontrolrequestwaittypedef)
- [UpdateSafetyRuleRequestRequestTypeDef](./type_defs.md#updatesafetyrulerequestrequesttypedef)
- [ListAssociatedRoute53HealthChecksRequestPaginateTypeDef](./type_defs.md#listassociatedroute53healthchecksrequestpaginatetypedef)
- [ListClustersRequestPaginateTypeDef](./type_defs.md#listclustersrequestpaginatetypedef)
- [ListControlPanelsRequestPaginateTypeDef](./type_defs.md#listcontrolpanelsrequestpaginatetypedef)
- [ListRoutingControlsRequestPaginateTypeDef](./type_defs.md#listroutingcontrolsrequestpaginatetypedef)
- [ListSafetyRulesRequestPaginateTypeDef](./type_defs.md#listsafetyrulesrequestpaginatetypedef)
- [CreateSafetyRuleResponseTypeDef](./type_defs.md#createsafetyruleresponsetypedef)
- [DescribeSafetyRuleResponseTypeDef](./type_defs.md#describesafetyruleresponsetypedef)
- [RuleTypeDef](./type_defs.md#ruletypedef)
- [UpdateSafetyRuleResponseTypeDef](./type_defs.md#updatesafetyruleresponsetypedef)
- [CreateSafetyRuleRequestRequestTypeDef](./type_defs.md#createsafetyrulerequestrequesttypedef)
- [CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)
- [DescribeClusterResponseTypeDef](./type_defs.md#describeclusterresponsetypedef)
- [ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef)
- [ListSafetyRulesResponseTypeDef](./type_defs.md#listsafetyrulesresponsetypedef)

