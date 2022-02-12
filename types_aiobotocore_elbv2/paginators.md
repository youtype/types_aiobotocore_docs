<a id="paginators-for-aiobotocore-elasticloadbalancingv2-module"></a>

# Paginators for aiobotocore ElasticLoadBalancingv2 module

> [Index](..) > [ElasticLoadBalancingv2](.) > Paginators

Auto-generated documentation for
[ElasticLoadBalancingv2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
type annotations stubs module
[types-aiobotocore-elbv2](https://pypi.org/project/types-aiobotocore-elbv2/).

- [Paginators for aiobotocore ElasticLoadBalancingv2 module](#paginators-for-aiobotocore-elasticloadbalancingv2-module)
  - [DescribeAccountLimitsPaginator](#describeaccountlimitspaginator)
  - [DescribeListenerCertificatesPaginator](#describelistenercertificatespaginator)
  - [DescribeListenersPaginator](#describelistenerspaginator)
  - [DescribeLoadBalancersPaginator](#describeloadbalancerspaginator)
  - [DescribeRulesPaginator](#describerulespaginator)
  - [DescribeSSLPoliciesPaginator](#describesslpoliciespaginator)
  - [DescribeTargetGroupsPaginator](#describetargetgroupspaginator)

<a id="describeaccountlimitspaginator"></a>

## DescribeAccountLimitsPaginator

Type annotations for
`session.create_client("elbv2").get_paginator("describe_account_limits")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeAccountLimitsPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")
```

Boto3 documentation:
[ElasticLoadBalancingv2.Paginator.DescribeAccountLimits](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits)

Arguments for `DescribeAccountLimitsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeAccountLimitsPaginator.paginate` returns
`AsyncIterable`\[[DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef)\].

<a id="describelistenercertificatespaginator"></a>

## DescribeListenerCertificatesPaginator

Type annotations for
`session.create_client("elbv2").get_paginator("describe_listener_certificates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeListenerCertificatesPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeListenerCertificatesPaginator = client.get_paginator("describe_listener_certificates")
```

Boto3 documentation:
[ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates)

Arguments for `DescribeListenerCertificatesPaginator.paginate` method:

- `ListenerArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeListenerCertificatesPaginator.paginate` returns
`AsyncIterable`\[[DescribeListenerCertificatesOutputTypeDef](./type_defs.md#describelistenercertificatesoutputtypedef)\].

<a id="describelistenerspaginator"></a>

## DescribeListenersPaginator

Type annotations for
`session.create_client("elbv2").get_paginator("describe_listeners")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeListenersPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeListenersPaginator = client.get_paginator("describe_listeners")
```

Boto3 documentation:
[ElasticLoadBalancingv2.Paginator.DescribeListeners](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListeners)

Arguments for `DescribeListenersPaginator.paginate` method:

- `LoadBalancerArn`: `str`
- `ListenerArns`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeListenersPaginator.paginate` returns
`AsyncIterable`\[[DescribeListenersOutputTypeDef](./type_defs.md#describelistenersoutputtypedef)\].

<a id="describeloadbalancerspaginator"></a>

## DescribeLoadBalancersPaginator

Type annotations for
`session.create_client("elbv2").get_paginator("describe_load_balancers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeLoadBalancersPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")
```

Boto3 documentation:
[ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers)

Arguments for `DescribeLoadBalancersPaginator.paginate` method:

- `LoadBalancerArns`: `Sequence`\[`str`\]
- `Names`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeLoadBalancersPaginator.paginate` returns
`AsyncIterable`\[[DescribeLoadBalancersOutputTypeDef](./type_defs.md#describeloadbalancersoutputtypedef)\].

<a id="describerulespaginator"></a>

## DescribeRulesPaginator

Type annotations for
`session.create_client("elbv2").get_paginator("describe_rules")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeRulesPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeRulesPaginator = client.get_paginator("describe_rules")
```

Boto3 documentation:
[ElasticLoadBalancingv2.Paginator.DescribeRules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeRules)

Arguments for `DescribeRulesPaginator.paginate` method:

- `ListenerArn`: `str`
- `RuleArns`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeRulesPaginator.paginate` returns
`AsyncIterable`\[[DescribeRulesOutputTypeDef](./type_defs.md#describerulesoutputtypedef)\].

<a id="describesslpoliciespaginator"></a>

## DescribeSSLPoliciesPaginator

Type annotations for
`session.create_client("elbv2").get_paginator("describe_ssl_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeSSLPoliciesPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeSSLPoliciesPaginator = client.get_paginator("describe_ssl_policies")
```

Boto3 documentation:
[ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies)

Arguments for `DescribeSSLPoliciesPaginator.paginate` method:

- `Names`: `Sequence`\[`str`\]
- `LoadBalancerType`:
  [LoadBalancerTypeEnumType](./literals.md#loadbalancertypeenumtype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeSSLPoliciesPaginator.paginate` returns
`AsyncIterable`\[[DescribeSSLPoliciesOutputTypeDef](./type_defs.md#describesslpoliciesoutputtypedef)\].

<a id="describetargetgroupspaginator"></a>

## DescribeTargetGroupsPaginator

Type annotations for
`session.create_client("elbv2").get_paginator("describe_target_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeTargetGroupsPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeTargetGroupsPaginator = client.get_paginator("describe_target_groups")
```

Boto3 documentation:
[ElasticLoadBalancingv2.Paginator.DescribeTargetGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups)

Arguments for `DescribeTargetGroupsPaginator.paginate` method:

- `LoadBalancerArn`: `str`
- `TargetGroupArns`: `Sequence`\[`str`\]
- `Names`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeTargetGroupsPaginator.paginate` returns
`AsyncIterable`\[[DescribeTargetGroupsOutputTypeDef](./type_defs.md#describetargetgroupsoutputtypedef)\].
