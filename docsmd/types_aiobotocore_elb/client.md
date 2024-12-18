# ElasticLoadBalancingClient

> [Index](../README.md) > [ElasticLoadBalancing](./README.md) > ElasticLoadBalancingClient

!!! note ""

    Auto-generated documentation for [ElasticLoadBalancing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#elasticloadbalancing)
    type annotations stubs module [types-aiobotocore-elb](https://pypi.org/project/types-aiobotocore-elb/).

## ElasticLoadBalancingClient

Type annotations and code completion for `#!python session.create_client("elb")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client)

```python
# ElasticLoadBalancingClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_elb.client import ElasticLoadBalancingClient

session = get_session()
async with session.create_client("elb") as client:
    client: ElasticLoadBalancingClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("elb").exceptions` structure.

```python
# ElasticLoadBalancingClient.exceptions usage example

async with session.create_client("elb") as client:
    try:
        do_something(client)
    except (
            client.AccessPointNotFoundException,
        client.CertificateNotFoundException,
        client.ClientError,
        client.DependencyThrottleException,
        client.DuplicateAccessPointNameException,
        client.DuplicateListenerException,
        client.DuplicatePolicyNameException,
        client.DuplicateTagKeysException,
        client.InvalidConfigurationRequestException,
        client.InvalidEndPointException,
        client.InvalidSchemeException,
        client.InvalidSecurityGroupException,
        client.InvalidSubnetException,
        client.ListenerNotFoundException,
        client.LoadBalancerAttributeNotFoundException,
        client.OperationNotPermittedException,
        client.PolicyNotFoundException,
        client.PolicyTypeNotFoundException,
        client.SubnetNotFoundException,
        client.TooManyAccessPointsException,
        client.TooManyPoliciesException,
        client.TooManyTagsException,
        client.UnsupportedProtocolException,
    ) as e:
        print(e)
```

```python
# ElasticLoadBalancingClient usage type checking example

from types_aiobotocore_elb.client import Exceptions

def handle_error(exc: Exceptions.AccessPointNotFoundException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("elb").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("elb").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/generate_presigned_url.html)

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


### close



Type annotations and code completion for `#!python session.create_client("elb").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### add\_tags

Adds the specified tags to the specified load balancer.

Type annotations and code completion for `#!python session.create_client("elb").add_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/add_tags.html)

```python
# add_tags method definition

await def add_tags(
    self,
    *,
    LoadBalancerNames: Sequence[str],
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# add_tags method usage example with argument unpacking

kwargs: AddTagsInputRequestTypeDef = {  # (1)
    "LoadBalancerNames": ...,
    "Tags": ...,
}

parent.add_tags(**kwargs)
```

1. See [:material-code-braces: AddTagsInputRequestTypeDef](./type_defs.md#addtagsinputrequesttypedef) 

### apply\_security\_groups\_to\_load\_balancer

Associates one or more security groups with your load balancer in a virtual
private cloud (VPC).

Type annotations and code completion for `#!python session.create_client("elb").apply_security_groups_to_load_balancer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/apply_security_groups_to_load_balancer.html)

```python
# apply_security_groups_to_load_balancer method definition

await def apply_security_groups_to_load_balancer(
    self,
    *,
    LoadBalancerName: str,
    SecurityGroups: Sequence[str],
) -> ApplySecurityGroupsToLoadBalancerOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ApplySecurityGroupsToLoadBalancerOutputTypeDef](./type_defs.md#applysecuritygroupstoloadbalanceroutputtypedef) 


```python
# apply_security_groups_to_load_balancer method usage example with argument unpacking

kwargs: ApplySecurityGroupsToLoadBalancerInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "SecurityGroups": ...,
}

parent.apply_security_groups_to_load_balancer(**kwargs)
```

1. See [:material-code-braces: ApplySecurityGroupsToLoadBalancerInputRequestTypeDef](./type_defs.md#applysecuritygroupstoloadbalancerinputrequesttypedef) 

### attach\_load\_balancer\_to\_subnets

Adds one or more subnets to the set of configured subnets for the specified
load balancer.

Type annotations and code completion for `#!python session.create_client("elb").attach_load_balancer_to_subnets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/attach_load_balancer_to_subnets.html)

```python
# attach_load_balancer_to_subnets method definition

await def attach_load_balancer_to_subnets(
    self,
    *,
    LoadBalancerName: str,
    Subnets: Sequence[str],
) -> AttachLoadBalancerToSubnetsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AttachLoadBalancerToSubnetsOutputTypeDef](./type_defs.md#attachloadbalancertosubnetsoutputtypedef) 


```python
# attach_load_balancer_to_subnets method usage example with argument unpacking

kwargs: AttachLoadBalancerToSubnetsInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "Subnets": ...,
}

parent.attach_load_balancer_to_subnets(**kwargs)
```

1. See [:material-code-braces: AttachLoadBalancerToSubnetsInputRequestTypeDef](./type_defs.md#attachloadbalancertosubnetsinputrequesttypedef) 

### configure\_health\_check

Specifies the health check settings to use when evaluating the health state of
your EC2 instances.

Type annotations and code completion for `#!python session.create_client("elb").configure_health_check` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/configure_health_check.html)

```python
# configure_health_check method definition

await def configure_health_check(
    self,
    *,
    LoadBalancerName: str,
    HealthCheck: HealthCheckTypeDef,  # (1)
) -> ConfigureHealthCheckOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: HealthCheckTypeDef](./type_defs.md#healthchecktypedef) 
2. See [:material-code-braces: ConfigureHealthCheckOutputTypeDef](./type_defs.md#configurehealthcheckoutputtypedef) 


```python
# configure_health_check method usage example with argument unpacking

kwargs: ConfigureHealthCheckInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "HealthCheck": ...,
}

parent.configure_health_check(**kwargs)
```

1. See [:material-code-braces: ConfigureHealthCheckInputRequestTypeDef](./type_defs.md#configurehealthcheckinputrequesttypedef) 

### create\_app\_cookie\_stickiness\_policy

Generates a stickiness policy with sticky session lifetimes that follow that of
an application-generated cookie.

Type annotations and code completion for `#!python session.create_client("elb").create_app_cookie_stickiness_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/create_app_cookie_stickiness_policy.html)

```python
# create_app_cookie_stickiness_policy method definition

await def create_app_cookie_stickiness_policy(
    self,
    *,
    LoadBalancerName: str,
    PolicyName: str,
    CookieName: str,
) -> Dict[str, Any]:
    ...
```



```python
# create_app_cookie_stickiness_policy method usage example with argument unpacking

kwargs: CreateAppCookieStickinessPolicyInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "PolicyName": ...,
    "CookieName": ...,
}

parent.create_app_cookie_stickiness_policy(**kwargs)
```

1. See [:material-code-braces: CreateAppCookieStickinessPolicyInputRequestTypeDef](./type_defs.md#createappcookiestickinesspolicyinputrequesttypedef) 

### create\_lb\_cookie\_stickiness\_policy

Generates a stickiness policy with sticky session lifetimes controlled by the
lifetime of the browser (user-agent) or a specified expiration period.

Type annotations and code completion for `#!python session.create_client("elb").create_lb_cookie_stickiness_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/create_lb_cookie_stickiness_policy.html)

```python
# create_lb_cookie_stickiness_policy method definition

await def create_lb_cookie_stickiness_policy(
    self,
    *,
    LoadBalancerName: str,
    PolicyName: str,
    CookieExpirationPeriod: int = ...,
) -> Dict[str, Any]:
    ...
```



```python
# create_lb_cookie_stickiness_policy method usage example with argument unpacking

kwargs: CreateLBCookieStickinessPolicyInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "PolicyName": ...,
}

parent.create_lb_cookie_stickiness_policy(**kwargs)
```

1. See [:material-code-braces: CreateLBCookieStickinessPolicyInputRequestTypeDef](./type_defs.md#createlbcookiestickinesspolicyinputrequesttypedef) 

### create\_load\_balancer

Creates a Classic Load Balancer.

Type annotations and code completion for `#!python session.create_client("elb").create_load_balancer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/create_load_balancer.html)

```python
# create_load_balancer method definition

await def create_load_balancer(
    self,
    *,
    LoadBalancerName: str,
    Listeners: Sequence[ListenerTypeDef],  # (1)
    AvailabilityZones: Sequence[str] = ...,
    Subnets: Sequence[str] = ...,
    SecurityGroups: Sequence[str] = ...,
    Scheme: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateAccessPointOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateAccessPointOutputTypeDef](./type_defs.md#createaccesspointoutputtypedef) 


```python
# create_load_balancer method usage example with argument unpacking

kwargs: CreateAccessPointInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "Listeners": ...,
}

parent.create_load_balancer(**kwargs)
```

1. See [:material-code-braces: CreateAccessPointInputRequestTypeDef](./type_defs.md#createaccesspointinputrequesttypedef) 

### create\_load\_balancer\_listeners

Creates one or more listeners for the specified load balancer.

Type annotations and code completion for `#!python session.create_client("elb").create_load_balancer_listeners` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/create_load_balancer_listeners.html)

```python
# create_load_balancer_listeners method definition

await def create_load_balancer_listeners(
    self,
    *,
    LoadBalancerName: str,
    Listeners: Sequence[ListenerTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 


```python
# create_load_balancer_listeners method usage example with argument unpacking

kwargs: CreateLoadBalancerListenerInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "Listeners": ...,
}

parent.create_load_balancer_listeners(**kwargs)
```

1. See [:material-code-braces: CreateLoadBalancerListenerInputRequestTypeDef](./type_defs.md#createloadbalancerlistenerinputrequesttypedef) 

### create\_load\_balancer\_policy

Creates a policy with the specified attributes for the specified load balancer.

Type annotations and code completion for `#!python session.create_client("elb").create_load_balancer_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/create_load_balancer_policy.html)

```python
# create_load_balancer_policy method definition

await def create_load_balancer_policy(
    self,
    *,
    LoadBalancerName: str,
    PolicyName: str,
    PolicyTypeName: str,
    PolicyAttributes: Sequence[PolicyAttributeTypeDef] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: PolicyAttributeTypeDef](./type_defs.md#policyattributetypedef) 


```python
# create_load_balancer_policy method usage example with argument unpacking

kwargs: CreateLoadBalancerPolicyInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "PolicyName": ...,
    "PolicyTypeName": ...,
}

parent.create_load_balancer_policy(**kwargs)
```

1. See [:material-code-braces: CreateLoadBalancerPolicyInputRequestTypeDef](./type_defs.md#createloadbalancerpolicyinputrequesttypedef) 

### delete\_load\_balancer

Deletes the specified load balancer.

Type annotations and code completion for `#!python session.create_client("elb").delete_load_balancer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/delete_load_balancer.html)

```python
# delete_load_balancer method definition

await def delete_load_balancer(
    self,
    *,
    LoadBalancerName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_load_balancer method usage example with argument unpacking

kwargs: DeleteAccessPointInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
}

parent.delete_load_balancer(**kwargs)
```

1. See [:material-code-braces: DeleteAccessPointInputRequestTypeDef](./type_defs.md#deleteaccesspointinputrequesttypedef) 

### delete\_load\_balancer\_listeners

Deletes the specified listeners from the specified load balancer.

Type annotations and code completion for `#!python session.create_client("elb").delete_load_balancer_listeners` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/delete_load_balancer_listeners.html)

```python
# delete_load_balancer_listeners method definition

await def delete_load_balancer_listeners(
    self,
    *,
    LoadBalancerName: str,
    LoadBalancerPorts: Sequence[int],
) -> Dict[str, Any]:
    ...
```



```python
# delete_load_balancer_listeners method usage example with argument unpacking

kwargs: DeleteLoadBalancerListenerInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "LoadBalancerPorts": ...,
}

parent.delete_load_balancer_listeners(**kwargs)
```

1. See [:material-code-braces: DeleteLoadBalancerListenerInputRequestTypeDef](./type_defs.md#deleteloadbalancerlistenerinputrequesttypedef) 

### delete\_load\_balancer\_policy

Deletes the specified policy from the specified load balancer.

Type annotations and code completion for `#!python session.create_client("elb").delete_load_balancer_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/delete_load_balancer_policy.html)

```python
# delete_load_balancer_policy method definition

await def delete_load_balancer_policy(
    self,
    *,
    LoadBalancerName: str,
    PolicyName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_load_balancer_policy method usage example with argument unpacking

kwargs: DeleteLoadBalancerPolicyInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "PolicyName": ...,
}

parent.delete_load_balancer_policy(**kwargs)
```

1. See [:material-code-braces: DeleteLoadBalancerPolicyInputRequestTypeDef](./type_defs.md#deleteloadbalancerpolicyinputrequesttypedef) 

### deregister\_instances\_from\_load\_balancer

Deregisters the specified instances from the specified load balancer.

Type annotations and code completion for `#!python session.create_client("elb").deregister_instances_from_load_balancer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/deregister_instances_from_load_balancer.html)

```python
# deregister_instances_from_load_balancer method definition

await def deregister_instances_from_load_balancer(
    self,
    *,
    LoadBalancerName: str,
    Instances: Sequence[InstanceTypeDef],  # (1)
) -> DeregisterEndPointsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: DeregisterEndPointsOutputTypeDef](./type_defs.md#deregisterendpointsoutputtypedef) 


```python
# deregister_instances_from_load_balancer method usage example with argument unpacking

kwargs: DeregisterEndPointsInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "Instances": ...,
}

parent.deregister_instances_from_load_balancer(**kwargs)
```

1. See [:material-code-braces: DeregisterEndPointsInputRequestTypeDef](./type_defs.md#deregisterendpointsinputrequesttypedef) 

### describe\_account\_limits

Describes the current Elastic Load Balancing resource limits for your AWS
account.

Type annotations and code completion for `#!python session.create_client("elb").describe_account_limits` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/describe_account_limits.html)

```python
# describe_account_limits method definition

await def describe_account_limits(
    self,
    *,
    Marker: str = ...,
    PageSize: int = ...,
) -> DescribeAccountLimitsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef) 


```python
# describe_account_limits method usage example with argument unpacking

kwargs: DescribeAccountLimitsInputRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.describe_account_limits(**kwargs)
```

1. See [:material-code-braces: DescribeAccountLimitsInputRequestTypeDef](./type_defs.md#describeaccountlimitsinputrequesttypedef) 

### describe\_instance\_health

Describes the state of the specified instances with respect to the specified
load balancer.

Type annotations and code completion for `#!python session.create_client("elb").describe_instance_health` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/describe_instance_health.html)

```python
# describe_instance_health method definition

await def describe_instance_health(
    self,
    *,
    LoadBalancerName: str,
    Instances: Sequence[InstanceTypeDef] = ...,  # (1)
) -> DescribeEndPointStateOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: DescribeEndPointStateOutputTypeDef](./type_defs.md#describeendpointstateoutputtypedef) 


```python
# describe_instance_health method usage example with argument unpacking

kwargs: DescribeEndPointStateInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
}

parent.describe_instance_health(**kwargs)
```

1. See [:material-code-braces: DescribeEndPointStateInputRequestTypeDef](./type_defs.md#describeendpointstateinputrequesttypedef) 

### describe\_load\_balancer\_attributes

Describes the attributes for the specified load balancer.

Type annotations and code completion for `#!python session.create_client("elb").describe_load_balancer_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/describe_load_balancer_attributes.html)

```python
# describe_load_balancer_attributes method definition

await def describe_load_balancer_attributes(
    self,
    *,
    LoadBalancerName: str,
) -> DescribeLoadBalancerAttributesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLoadBalancerAttributesOutputTypeDef](./type_defs.md#describeloadbalancerattributesoutputtypedef) 


```python
# describe_load_balancer_attributes method usage example with argument unpacking

kwargs: DescribeLoadBalancerAttributesInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
}

parent.describe_load_balancer_attributes(**kwargs)
```

1. See [:material-code-braces: DescribeLoadBalancerAttributesInputRequestTypeDef](./type_defs.md#describeloadbalancerattributesinputrequesttypedef) 

### describe\_load\_balancer\_policies

Describes the specified policies.

Type annotations and code completion for `#!python session.create_client("elb").describe_load_balancer_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/describe_load_balancer_policies.html)

```python
# describe_load_balancer_policies method definition

await def describe_load_balancer_policies(
    self,
    *,
    LoadBalancerName: str = ...,
    PolicyNames: Sequence[str] = ...,
) -> DescribeLoadBalancerPoliciesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLoadBalancerPoliciesOutputTypeDef](./type_defs.md#describeloadbalancerpoliciesoutputtypedef) 


```python
# describe_load_balancer_policies method usage example with argument unpacking

kwargs: DescribeLoadBalancerPoliciesInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
}

parent.describe_load_balancer_policies(**kwargs)
```

1. See [:material-code-braces: DescribeLoadBalancerPoliciesInputRequestTypeDef](./type_defs.md#describeloadbalancerpoliciesinputrequesttypedef) 

### describe\_load\_balancer\_policy\_types

Describes the specified load balancer policy types or all load balancer policy
types.

Type annotations and code completion for `#!python session.create_client("elb").describe_load_balancer_policy_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/describe_load_balancer_policy_types.html)

```python
# describe_load_balancer_policy_types method definition

await def describe_load_balancer_policy_types(
    self,
    *,
    PolicyTypeNames: Sequence[str] = ...,
) -> DescribeLoadBalancerPolicyTypesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLoadBalancerPolicyTypesOutputTypeDef](./type_defs.md#describeloadbalancerpolicytypesoutputtypedef) 


```python
# describe_load_balancer_policy_types method usage example with argument unpacking

kwargs: DescribeLoadBalancerPolicyTypesInputRequestTypeDef = {  # (1)
    "PolicyTypeNames": ...,
}

parent.describe_load_balancer_policy_types(**kwargs)
```

1. See [:material-code-braces: DescribeLoadBalancerPolicyTypesInputRequestTypeDef](./type_defs.md#describeloadbalancerpolicytypesinputrequesttypedef) 

### describe\_load\_balancers

Describes the specified the load balancers.

Type annotations and code completion for `#!python session.create_client("elb").describe_load_balancers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/describe_load_balancers.html)

```python
# describe_load_balancers method definition

await def describe_load_balancers(
    self,
    *,
    LoadBalancerNames: Sequence[str] = ...,
    Marker: str = ...,
    PageSize: int = ...,
) -> DescribeAccessPointsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccessPointsOutputTypeDef](./type_defs.md#describeaccesspointsoutputtypedef) 


```python
# describe_load_balancers method usage example with argument unpacking

kwargs: DescribeAccessPointsInputRequestTypeDef = {  # (1)
    "LoadBalancerNames": ...,
}

parent.describe_load_balancers(**kwargs)
```

1. See [:material-code-braces: DescribeAccessPointsInputRequestTypeDef](./type_defs.md#describeaccesspointsinputrequesttypedef) 

### describe\_tags

Describes the tags associated with the specified load balancers.

Type annotations and code completion for `#!python session.create_client("elb").describe_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/describe_tags.html)

```python
# describe_tags method definition

await def describe_tags(
    self,
    *,
    LoadBalancerNames: Sequence[str],
) -> DescribeTagsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTagsOutputTypeDef](./type_defs.md#describetagsoutputtypedef) 


```python
# describe_tags method usage example with argument unpacking

kwargs: DescribeTagsInputRequestTypeDef = {  # (1)
    "LoadBalancerNames": ...,
}

parent.describe_tags(**kwargs)
```

1. See [:material-code-braces: DescribeTagsInputRequestTypeDef](./type_defs.md#describetagsinputrequesttypedef) 

### detach\_load\_balancer\_from\_subnets

Removes the specified subnets from the set of configured subnets for the load
balancer.

Type annotations and code completion for `#!python session.create_client("elb").detach_load_balancer_from_subnets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/detach_load_balancer_from_subnets.html)

```python
# detach_load_balancer_from_subnets method definition

await def detach_load_balancer_from_subnets(
    self,
    *,
    LoadBalancerName: str,
    Subnets: Sequence[str],
) -> DetachLoadBalancerFromSubnetsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DetachLoadBalancerFromSubnetsOutputTypeDef](./type_defs.md#detachloadbalancerfromsubnetsoutputtypedef) 


```python
# detach_load_balancer_from_subnets method usage example with argument unpacking

kwargs: DetachLoadBalancerFromSubnetsInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "Subnets": ...,
}

parent.detach_load_balancer_from_subnets(**kwargs)
```

1. See [:material-code-braces: DetachLoadBalancerFromSubnetsInputRequestTypeDef](./type_defs.md#detachloadbalancerfromsubnetsinputrequesttypedef) 

### disable\_availability\_zones\_for\_load\_balancer

Removes the specified Availability Zones from the set of Availability Zones for
the specified load balancer in EC2-Classic or a default VPC.

Type annotations and code completion for `#!python session.create_client("elb").disable_availability_zones_for_load_balancer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/disable_availability_zones_for_load_balancer.html)

```python
# disable_availability_zones_for_load_balancer method definition

await def disable_availability_zones_for_load_balancer(
    self,
    *,
    LoadBalancerName: str,
    AvailabilityZones: Sequence[str],
) -> RemoveAvailabilityZonesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RemoveAvailabilityZonesOutputTypeDef](./type_defs.md#removeavailabilityzonesoutputtypedef) 


```python
# disable_availability_zones_for_load_balancer method usage example with argument unpacking

kwargs: RemoveAvailabilityZonesInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "AvailabilityZones": ...,
}

parent.disable_availability_zones_for_load_balancer(**kwargs)
```

1. See [:material-code-braces: RemoveAvailabilityZonesInputRequestTypeDef](./type_defs.md#removeavailabilityzonesinputrequesttypedef) 

### enable\_availability\_zones\_for\_load\_balancer

Adds the specified Availability Zones to the set of Availability Zones for the
specified load balancer in EC2-Classic or a default VPC.

Type annotations and code completion for `#!python session.create_client("elb").enable_availability_zones_for_load_balancer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/enable_availability_zones_for_load_balancer.html)

```python
# enable_availability_zones_for_load_balancer method definition

await def enable_availability_zones_for_load_balancer(
    self,
    *,
    LoadBalancerName: str,
    AvailabilityZones: Sequence[str],
) -> AddAvailabilityZonesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AddAvailabilityZonesOutputTypeDef](./type_defs.md#addavailabilityzonesoutputtypedef) 


```python
# enable_availability_zones_for_load_balancer method usage example with argument unpacking

kwargs: AddAvailabilityZonesInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "AvailabilityZones": ...,
}

parent.enable_availability_zones_for_load_balancer(**kwargs)
```

1. See [:material-code-braces: AddAvailabilityZonesInputRequestTypeDef](./type_defs.md#addavailabilityzonesinputrequesttypedef) 

### modify\_load\_balancer\_attributes

Modifies the attributes of the specified load balancer.

Type annotations and code completion for `#!python session.create_client("elb").modify_load_balancer_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/modify_load_balancer_attributes.html)

```python
# modify_load_balancer_attributes method definition

await def modify_load_balancer_attributes(
    self,
    *,
    LoadBalancerName: str,
    LoadBalancerAttributes: LoadBalancerAttributesTypeDef,  # (1)
) -> ModifyLoadBalancerAttributesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LoadBalancerAttributesTypeDef](./type_defs.md#loadbalancerattributestypedef) 
2. See [:material-code-braces: ModifyLoadBalancerAttributesOutputTypeDef](./type_defs.md#modifyloadbalancerattributesoutputtypedef) 


```python
# modify_load_balancer_attributes method usage example with argument unpacking

kwargs: ModifyLoadBalancerAttributesInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "LoadBalancerAttributes": ...,
}

parent.modify_load_balancer_attributes(**kwargs)
```

1. See [:material-code-braces: ModifyLoadBalancerAttributesInputRequestTypeDef](./type_defs.md#modifyloadbalancerattributesinputrequesttypedef) 

### register\_instances\_with\_load\_balancer

Adds the specified instances to the specified load balancer.

Type annotations and code completion for `#!python session.create_client("elb").register_instances_with_load_balancer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/register_instances_with_load_balancer.html)

```python
# register_instances_with_load_balancer method definition

await def register_instances_with_load_balancer(
    self,
    *,
    LoadBalancerName: str,
    Instances: Sequence[InstanceTypeDef],  # (1)
) -> RegisterEndPointsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: RegisterEndPointsOutputTypeDef](./type_defs.md#registerendpointsoutputtypedef) 


```python
# register_instances_with_load_balancer method usage example with argument unpacking

kwargs: RegisterEndPointsInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "Instances": ...,
}

parent.register_instances_with_load_balancer(**kwargs)
```

1. See [:material-code-braces: RegisterEndPointsInputRequestTypeDef](./type_defs.md#registerendpointsinputrequesttypedef) 

### remove\_tags

Removes one or more tags from the specified load balancer.

Type annotations and code completion for `#!python session.create_client("elb").remove_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/remove_tags.html)

```python
# remove_tags method definition

await def remove_tags(
    self,
    *,
    LoadBalancerNames: Sequence[str],
    Tags: Sequence[TagKeyOnlyTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagKeyOnlyTypeDef](./type_defs.md#tagkeyonlytypedef) 


```python
# remove_tags method usage example with argument unpacking

kwargs: RemoveTagsInputRequestTypeDef = {  # (1)
    "LoadBalancerNames": ...,
    "Tags": ...,
}

parent.remove_tags(**kwargs)
```

1. See [:material-code-braces: RemoveTagsInputRequestTypeDef](./type_defs.md#removetagsinputrequesttypedef) 

### set\_load\_balancer\_listener\_ssl\_certificate

Sets the certificate that terminates the specified listener's SSL connections.

Type annotations and code completion for `#!python session.create_client("elb").set_load_balancer_listener_ssl_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/set_load_balancer_listener_ssl_certificate.html)

```python
# set_load_balancer_listener_ssl_certificate method definition

await def set_load_balancer_listener_ssl_certificate(
    self,
    *,
    LoadBalancerName: str,
    LoadBalancerPort: int,
    SSLCertificateId: str,
) -> Dict[str, Any]:
    ...
```



```python
# set_load_balancer_listener_ssl_certificate method usage example with argument unpacking

kwargs: SetLoadBalancerListenerSSLCertificateInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "LoadBalancerPort": ...,
    "SSLCertificateId": ...,
}

parent.set_load_balancer_listener_ssl_certificate(**kwargs)
```

1. See [:material-code-braces: SetLoadBalancerListenerSSLCertificateInputRequestTypeDef](./type_defs.md#setloadbalancerlistenersslcertificateinputrequesttypedef) 

### set\_load\_balancer\_policies\_for\_backend\_server

Replaces the set of policies associated with the specified port on which the
EC2 instance is listening with a new set of policies.

Type annotations and code completion for `#!python session.create_client("elb").set_load_balancer_policies_for_backend_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/set_load_balancer_policies_for_backend_server.html)

```python
# set_load_balancer_policies_for_backend_server method definition

await def set_load_balancer_policies_for_backend_server(
    self,
    *,
    LoadBalancerName: str,
    InstancePort: int,
    PolicyNames: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# set_load_balancer_policies_for_backend_server method usage example with argument unpacking

kwargs: SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "InstancePort": ...,
    "PolicyNames": ...,
}

parent.set_load_balancer_policies_for_backend_server(**kwargs)
```

1. See [:material-code-braces: SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef](./type_defs.md#setloadbalancerpoliciesforbackendserverinputrequesttypedef) 

### set\_load\_balancer\_policies\_of\_listener

Replaces the current set of policies for the specified load balancer port with
the specified set of policies.

Type annotations and code completion for `#!python session.create_client("elb").set_load_balancer_policies_of_listener` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb/client/set_load_balancer_policies_of_listener.html)

```python
# set_load_balancer_policies_of_listener method definition

await def set_load_balancer_policies_of_listener(
    self,
    *,
    LoadBalancerName: str,
    LoadBalancerPort: int,
    PolicyNames: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# set_load_balancer_policies_of_listener method usage example with argument unpacking

kwargs: SetLoadBalancerPoliciesOfListenerInputRequestTypeDef = {  # (1)
    "LoadBalancerName": ...,
    "LoadBalancerPort": ...,
    "PolicyNames": ...,
}

parent.set_load_balancer_policies_of_listener(**kwargs)
```

1. See [:material-code-braces: SetLoadBalancerPoliciesOfListenerInputRequestTypeDef](./type_defs.md#setloadbalancerpoliciesoflistenerinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("elb").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "ElasticLoadBalancingClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("elb").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client)

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

Type annotations and code completion for `#!python session.create_client("elb").get_paginator` method with overloads.

- `client.get_paginator("describe_account_limits")` -> [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
- `client.get_paginator("describe_load_balancers")` -> [DescribeLoadBalancersPaginator](./paginators.md#describeloadbalancerspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("elb").get_waiter` method with overloads.

- `client.get_waiter("any_instance_in_service")` -> [AnyInstanceInServiceWaiter](./waiters.md#anyinstanceinservicewaiter)
- `client.get_waiter("instance_deregistered")` -> [InstanceDeregisteredWaiter](./waiters.md#instancederegisteredwaiter)
- `client.get_waiter("instance_in_service")` -> [InstanceInServiceWaiter](./waiters.md#instanceinservicewaiter)

