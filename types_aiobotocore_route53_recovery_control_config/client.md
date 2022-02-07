<a id="route53recoverycontrolconfigclient-for-aiobotocore-route53recoverycontrolconfig-module"></a>

# Route53RecoveryControlConfigClient for aiobotocore Route53RecoveryControlConfig module

> [Index](..) > [Route53RecoveryControlConfig](.) >
> Route53RecoveryControlConfigClient

Auto-generated documentation for
[Route53RecoveryControlConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
type annotations stubs module
[types-aiobotocore-route53-recovery-control-config](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config/).

- [Route53RecoveryControlConfigClient for aiobotocore Route53RecoveryControlConfig module](#route53recoverycontrolconfigclient-for-aiobotocore-route53recoverycontrolconfig-module)
  - [Route53RecoveryControlConfigClient](#route53recoverycontrolconfigclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_cluster](#create_cluster)
    - [create_control_panel](#create_control_panel)
    - [create_routing_control](#create_routing_control)
    - [create_safety_rule](#create_safety_rule)
    - [delete_cluster](#delete_cluster)
    - [delete_control_panel](#delete_control_panel)
    - [delete_routing_control](#delete_routing_control)
    - [delete_safety_rule](#delete_safety_rule)
    - [describe_cluster](#describe_cluster)
    - [describe_control_panel](#describe_control_panel)
    - [describe_routing_control](#describe_routing_control)
    - [describe_safety_rule](#describe_safety_rule)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_associated_route53_health_checks](#list_associated_route53_health_checks)
    - [list_clusters](#list_clusters)
    - [list_control_panels](#list_control_panels)
    - [list_routing_controls](#list_routing_controls)
    - [list_safety_rules](#list_safety_rules)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_control_panel](#update_control_panel)
    - [update_routing_control](#update_routing_control)
    - [update_safety_rule](#update_safety_rule)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_waiter](#get_waiter)

<a id="route53recoverycontrolconfigclient"></a>

## Route53RecoveryControlConfigClient

Type annotations for `session.create_client("route53-recovery-control-config")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_route53_recovery_control_config.client import Route53RecoveryControlConfigClient

session = get_session()
async with session.create_client("route53-recovery-control-config") as client:
    client: Route53RecoveryControlConfigClient
```

Boto3 documentation:
[Route53RecoveryControlConfig.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_route53_recovery_control_config.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

Route53RecoveryControlConfigClient exceptions.

Type annotations for
`session.create_client("route53-recovery-control-config").exceptions` method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`session.create_client("route53-recovery-control-config").can_paginate` method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_cluster"></a>

### create_cluster

Create a new cluster.

Type annotations for
`session.create_client("route53-recovery-control-config").create_cluster`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.create_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.create_cluster)

Asynchronous method. Use `await create_cluster(...)` for a synchronous call.

Arguments mapping described in
[CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef).

Keyword-only arguments:

- `ClusterName`: `str` *(required)*
- `ClientToken`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef).

<a id="create_control_panel"></a>

### create_control_panel

Creates a new control panel.

Type annotations for
`session.create_client("route53-recovery-control-config").create_control_panel`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.create_control_panel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.create_control_panel)

Asynchronous method. Use `await create_control_panel(...)` for a synchronous
call.

Arguments mapping described in
[CreateControlPanelRequestRequestTypeDef](./type_defs.md#createcontrolpanelrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `ControlPanelName`: `str` *(required)*
- `ClientToken`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateControlPanelResponseTypeDef](./type_defs.md#createcontrolpanelresponsetypedef).

<a id="create_routing_control"></a>

### create_routing_control

Creates a new routing control.

Type annotations for
`session.create_client("route53-recovery-control-config").create_routing_control`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.create_routing_control](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.create_routing_control)

Asynchronous method. Use `await create_routing_control(...)` for a synchronous
call.

Arguments mapping described in
[CreateRoutingControlRequestRequestTypeDef](./type_defs.md#createroutingcontrolrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `RoutingControlName`: `str` *(required)*
- `ClientToken`: `str`
- `ControlPanelArn`: `str`

Returns a `Coroutine` for
[CreateRoutingControlResponseTypeDef](./type_defs.md#createroutingcontrolresponsetypedef).

<a id="create_safety_rule"></a>

### create_safety_rule

Creates a safety rule in a control panel.

Type annotations for
`session.create_client("route53-recovery-control-config").create_safety_rule`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.create_safety_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.create_safety_rule)

Asynchronous method. Use `await create_safety_rule(...)` for a synchronous
call.

Arguments mapping described in
[CreateSafetyRuleRequestRequestTypeDef](./type_defs.md#createsafetyrulerequestrequesttypedef).

Keyword-only arguments:

- `AssertionRule`:
  [NewAssertionRuleTypeDef](./type_defs.md#newassertionruletypedef)
- `ClientToken`: `str`
- `GatingRule`: [NewGatingRuleTypeDef](./type_defs.md#newgatingruletypedef)
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateSafetyRuleResponseTypeDef](./type_defs.md#createsafetyruleresponsetypedef).

<a id="delete_cluster"></a>

### delete_cluster

Delete a cluster.

Type annotations for
`session.create_client("route53-recovery-control-config").delete_cluster`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.delete_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.delete_cluster)

Asynchronous method. Use `await delete_cluster(...)` for a synchronous call.

Arguments mapping described in
[DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_control_panel"></a>

### delete_control_panel

Deletes a control panel.

Type annotations for
`session.create_client("route53-recovery-control-config").delete_control_panel`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.delete_control_panel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.delete_control_panel)

Asynchronous method. Use `await delete_control_panel(...)` for a synchronous
call.

Arguments mapping described in
[DeleteControlPanelRequestRequestTypeDef](./type_defs.md#deletecontrolpanelrequestrequesttypedef).

Keyword-only arguments:

- `ControlPanelArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_routing_control"></a>

### delete_routing_control

Deletes a routing control.

Type annotations for
`session.create_client("route53-recovery-control-config").delete_routing_control`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.delete_routing_control](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.delete_routing_control)

Asynchronous method. Use `await delete_routing_control(...)` for a synchronous
call.

Arguments mapping described in
[DeleteRoutingControlRequestRequestTypeDef](./type_defs.md#deleteroutingcontrolrequestrequesttypedef).

Keyword-only arguments:

- `RoutingControlArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_safety_rule"></a>

### delete_safety_rule

Deletes a safety rule.

Type annotations for
`session.create_client("route53-recovery-control-config").delete_safety_rule`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.delete_safety_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.delete_safety_rule)

Asynchronous method. Use `await delete_safety_rule(...)` for a synchronous
call.

Arguments mapping described in
[DeleteSafetyRuleRequestRequestTypeDef](./type_defs.md#deletesafetyrulerequestrequesttypedef).

Keyword-only arguments:

- `SafetyRuleArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_cluster"></a>

### describe_cluster

Display the details about a cluster.

Type annotations for
`session.create_client("route53-recovery-control-config").describe_cluster`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.describe_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.describe_cluster)

Asynchronous method. Use `await describe_cluster(...)` for a synchronous call.

Arguments mapping described in
[DescribeClusterRequestRequestTypeDef](./type_defs.md#describeclusterrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeClusterResponseTypeDef](./type_defs.md#describeclusterresponsetypedef).

<a id="describe_control_panel"></a>

### describe_control_panel

Displays details about a control panel.

Type annotations for
`session.create_client("route53-recovery-control-config").describe_control_panel`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.describe_control_panel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.describe_control_panel)

Asynchronous method. Use `await describe_control_panel(...)` for a synchronous
call.

Arguments mapping described in
[DescribeControlPanelRequestRequestTypeDef](./type_defs.md#describecontrolpanelrequestrequesttypedef).

Keyword-only arguments:

- `ControlPanelArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeControlPanelResponseTypeDef](./type_defs.md#describecontrolpanelresponsetypedef).

<a id="describe_routing_control"></a>

### describe_routing_control

Displays details about a routing control.

Type annotations for
`session.create_client("route53-recovery-control-config").describe_routing_control`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.describe_routing_control](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.describe_routing_control)

Asynchronous method. Use `await describe_routing_control(...)` for a
synchronous call.

Arguments mapping described in
[DescribeRoutingControlRequestRequestTypeDef](./type_defs.md#describeroutingcontrolrequestrequesttypedef).

Keyword-only arguments:

- `RoutingControlArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeRoutingControlResponseTypeDef](./type_defs.md#describeroutingcontrolresponsetypedef).

<a id="describe_safety_rule"></a>

### describe_safety_rule

Returns information about a safety rule.

Type annotations for
`session.create_client("route53-recovery-control-config").describe_safety_rule`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.describe_safety_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.describe_safety_rule)

Asynchronous method. Use `await describe_safety_rule(...)` for a synchronous
call.

Arguments mapping described in
[DescribeSafetyRuleRequestRequestTypeDef](./type_defs.md#describesafetyrulerequestrequesttypedef).

Keyword-only arguments:

- `SafetyRuleArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeSafetyRuleResponseTypeDef](./type_defs.md#describesafetyruleresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("route53-recovery-control-config").generate_presigned_url`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_associated_route53_health_checks"></a>

### list_associated_route53_health_checks

Returns an array of all Amazon Route 53 health checks associated with a
specific routing control.

Type annotations for
`session.create_client("route53-recovery-control-config").list_associated_route53_health_checks`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.list_associated_route53_health_checks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.list_associated_route53_health_checks)

Asynchronous method. Use `await list_associated_route53_health_checks(...)` for
a synchronous call.

Arguments mapping described in
[ListAssociatedRoute53HealthChecksRequestRequestTypeDef](./type_defs.md#listassociatedroute53healthchecksrequestrequesttypedef).

Keyword-only arguments:

- `RoutingControlArn`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListAssociatedRoute53HealthChecksResponseTypeDef](./type_defs.md#listassociatedroute53healthchecksresponsetypedef).

<a id="list_clusters"></a>

### list_clusters

Returns an array of all the clusters in an account.

Type annotations for
`session.create_client("route53-recovery-control-config").list_clusters`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.list_clusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.list_clusters)

Asynchronous method. Use `await list_clusters(...)` for a synchronous call.

Arguments mapping described in
[ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef).

<a id="list_control_panels"></a>

### list_control_panels

Returns an array of control panels in an account or in a cluster.

Type annotations for
`session.create_client("route53-recovery-control-config").list_control_panels`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.list_control_panels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.list_control_panels)

Asynchronous method. Use `await list_control_panels(...)` for a synchronous
call.

Arguments mapping described in
[ListControlPanelsRequestRequestTypeDef](./type_defs.md#listcontrolpanelsrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListControlPanelsResponseTypeDef](./type_defs.md#listcontrolpanelsresponsetypedef).

<a id="list_routing_controls"></a>

### list_routing_controls

Returns an array of routing controls for a control panel.

Type annotations for
`session.create_client("route53-recovery-control-config").list_routing_controls`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.list_routing_controls](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.list_routing_controls)

Asynchronous method. Use `await list_routing_controls(...)` for a synchronous
call.

Arguments mapping described in
[ListRoutingControlsRequestRequestTypeDef](./type_defs.md#listroutingcontrolsrequestrequesttypedef).

Keyword-only arguments:

- `ControlPanelArn`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListRoutingControlsResponseTypeDef](./type_defs.md#listroutingcontrolsresponsetypedef).

<a id="list_safety_rules"></a>

### list_safety_rules

List the safety rules (the assertion rules and gating rules) that you've
defined for the routing controls in a control panel.

Type annotations for
`session.create_client("route53-recovery-control-config").list_safety_rules`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.list_safety_rules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.list_safety_rules)

Asynchronous method. Use `await list_safety_rules(...)` for a synchronous call.

Arguments mapping described in
[ListSafetyRulesRequestRequestTypeDef](./type_defs.md#listsafetyrulesrequestrequesttypedef).

Keyword-only arguments:

- `ControlPanelArn`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListSafetyRulesResponseTypeDef](./type_defs.md#listsafetyrulesresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Lists the tags for a resource.

Type annotations for
`session.create_client("route53-recovery-control-config").list_tags_for_resource`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Adds a tag to a resource.

Type annotations for
`session.create_client("route53-recovery-control-config").tag_resource` method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes a tag from a resource.

Type annotations for
`session.create_client("route53-recovery-control-config").untag_resource`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_control_panel"></a>

### update_control_panel

Updates a control panel.

Type annotations for
`session.create_client("route53-recovery-control-config").update_control_panel`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.update_control_panel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.update_control_panel)

Asynchronous method. Use `await update_control_panel(...)` for a synchronous
call.

Arguments mapping described in
[UpdateControlPanelRequestRequestTypeDef](./type_defs.md#updatecontrolpanelrequestrequesttypedef).

Keyword-only arguments:

- `ControlPanelArn`: `str` *(required)*
- `ControlPanelName`: `str` *(required)*

Returns a `Coroutine` for
[UpdateControlPanelResponseTypeDef](./type_defs.md#updatecontrolpanelresponsetypedef).

<a id="update_routing_control"></a>

### update_routing_control

Updates a routing control.

Type annotations for
`session.create_client("route53-recovery-control-config").update_routing_control`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.update_routing_control](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.update_routing_control)

Asynchronous method. Use `await update_routing_control(...)` for a synchronous
call.

Arguments mapping described in
[UpdateRoutingControlRequestRequestTypeDef](./type_defs.md#updateroutingcontrolrequestrequesttypedef).

Keyword-only arguments:

- `RoutingControlArn`: `str` *(required)*
- `RoutingControlName`: `str` *(required)*

Returns a `Coroutine` for
[UpdateRoutingControlResponseTypeDef](./type_defs.md#updateroutingcontrolresponsetypedef).

<a id="update_safety_rule"></a>

### update_safety_rule

Update a safety rule (an assertion rule or gating rule).

Type annotations for
`session.create_client("route53-recovery-control-config").update_safety_rule`
method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.update_safety_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.update_safety_rule)

Asynchronous method. Use `await update_safety_rule(...)` for a synchronous
call.

Arguments mapping described in
[UpdateSafetyRuleRequestRequestTypeDef](./type_defs.md#updatesafetyrulerequestrequesttypedef).

Keyword-only arguments:

- `AssertionRuleUpdate`:
  [AssertionRuleUpdateTypeDef](./type_defs.md#assertionruleupdatetypedef)
- `GatingRuleUpdate`:
  [GatingRuleUpdateTypeDef](./type_defs.md#gatingruleupdatetypedef)

Returns a `Coroutine` for
[UpdateSafetyRuleResponseTypeDef](./type_defs.md#updatesafetyruleresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for
`session.create_client("route53-recovery-control-config").__aenter__` method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[Route53RecoveryControlConfigClient](#route53recoverycontrolconfigclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for
`session.create_client("route53-recovery-control-config").__aexit__` method.

Boto3 documentation:
[Route53RecoveryControlConfig.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_waiter"></a>

### get_waiter

Type annotations for
`session.create_client("route53-recovery-control-config").get_waiter` method
with overloads.

- `client.get_waiter("cluster_created")` ->
  [ClusterCreatedWaiter](./waiters.md#clustercreatedwaiter)
- `client.get_waiter("cluster_deleted")` ->
  [ClusterDeletedWaiter](./waiters.md#clusterdeletedwaiter)
- `client.get_waiter("control_panel_created")` ->
  [ControlPanelCreatedWaiter](./waiters.md#controlpanelcreatedwaiter)
- `client.get_waiter("control_panel_deleted")` ->
  [ControlPanelDeletedWaiter](./waiters.md#controlpaneldeletedwaiter)
- `client.get_waiter("routing_control_created")` ->
  [RoutingControlCreatedWaiter](./waiters.md#routingcontrolcreatedwaiter)
- `client.get_waiter("routing_control_deleted")` ->
  [RoutingControlDeletedWaiter](./waiters.md#routingcontroldeletedwaiter)
