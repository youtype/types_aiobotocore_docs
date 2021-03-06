# Paginators

> [Index](../README.md) > [ElasticLoadBalancingv2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElasticLoadBalancingv2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
    type annotations stubs module [types-aiobotocore-elbv2](https://pypi.org/project/types-aiobotocore-elbv2/).

## DescribeAccountLimitsPaginator

Type annotations and code completion for `#!python session.create_client("elbv2").get_paginator("describe_account_limits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeAccountLimitsPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")
```


### paginate

Type annotations and code completion for `#!python DescribeAccountLimitsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeAccountLimitsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef](./type_defs.md#describeaccountlimitsinputdescribeaccountlimitspaginatetypedef) 
## DescribeListenerCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("elbv2").get_paginator("describe_listener_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeListenerCertificatesPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeListenerCertificatesPaginator = client.get_paginator("describe_listener_certificates")
```


### paginate

Type annotations and code completion for `#!python DescribeListenerCertificatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ListenerArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeListenerCertificatesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeListenerCertificatesOutputTypeDef](./type_defs.md#describelistenercertificatesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef](./type_defs.md#describelistenercertificatesinputdescribelistenercertificatespaginatetypedef) 
## DescribeListenersPaginator

Type annotations and code completion for `#!python session.create_client("elbv2").get_paginator("describe_listeners")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListeners)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeListenersPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeListenersPaginator = client.get_paginator("describe_listeners")
```


### paginate

Type annotations and code completion for `#!python DescribeListenersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LoadBalancerArn: str = ...,
    ListenerArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeListenersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeListenersOutputTypeDef](./type_defs.md#describelistenersoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeListenersInputDescribeListenersPaginateTypeDef = {  # (1)
    "LoadBalancerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeListenersInputDescribeListenersPaginateTypeDef](./type_defs.md#describelistenersinputdescribelistenerspaginatetypedef) 
## DescribeLoadBalancersPaginator

Type annotations and code completion for `#!python session.create_client("elbv2").get_paginator("describe_load_balancers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeLoadBalancersPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")
```


### paginate

Type annotations and code completion for `#!python DescribeLoadBalancersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LoadBalancerArns: Sequence[str] = ...,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeLoadBalancersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeLoadBalancersOutputTypeDef](./type_defs.md#describeloadbalancersoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = {  # (1)
    "LoadBalancerArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef](./type_defs.md#describeloadbalancersinputdescribeloadbalancerspaginatetypedef) 
## DescribeRulesPaginator

Type annotations and code completion for `#!python session.create_client("elbv2").get_paginator("describe_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeRules)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeRulesPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeRulesPaginator = client.get_paginator("describe_rules")
```


### paginate

Type annotations and code completion for `#!python DescribeRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ListenerArn: str = ...,
    RuleArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeRulesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRulesOutputTypeDef](./type_defs.md#describerulesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeRulesInputDescribeRulesPaginateTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRulesInputDescribeRulesPaginateTypeDef](./type_defs.md#describerulesinputdescriberulespaginatetypedef) 
## DescribeSSLPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("elbv2").get_paginator("describe_ssl_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeSSLPoliciesPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeSSLPoliciesPaginator = client.get_paginator("describe_ssl_policies")
```


### paginate

Type annotations and code completion for `#!python DescribeSSLPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    LoadBalancerType: LoadBalancerTypeEnumType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeSSLPoliciesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LoadBalancerTypeEnumType](./literals.md#loadbalancertypeenumtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSSLPoliciesOutputTypeDef](./type_defs.md#describesslpoliciesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef](./type_defs.md#describesslpoliciesinputdescribesslpoliciespaginatetypedef) 
## DescribeTargetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("elbv2").get_paginator("describe_target_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.paginator import DescribeTargetGroupsPaginator

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeTargetGroupsPaginator = client.get_paginator("describe_target_groups")
```


### paginate

Type annotations and code completion for `#!python DescribeTargetGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LoadBalancerArn: str = ...,
    TargetGroupArns: Sequence[str] = ...,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeTargetGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeTargetGroupsOutputTypeDef](./type_defs.md#describetargetgroupsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = {  # (1)
    "LoadBalancerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef](./type_defs.md#describetargetgroupsinputdescribetargetgroupspaginatetypedef) 
