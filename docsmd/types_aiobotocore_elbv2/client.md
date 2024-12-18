# ElasticLoadBalancingv2Client

> [Index](../README.md) > [ElasticLoadBalancingv2](./README.md) > ElasticLoadBalancingv2Client

!!! note ""

    Auto-generated documentation for [ElasticLoadBalancingv2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#elasticloadbalancingv2)
    type annotations stubs module [types-aiobotocore-elbv2](https://pypi.org/project/types-aiobotocore-elbv2/).

## ElasticLoadBalancingv2Client

Type annotations and code completion for `#!python session.create_client("elbv2")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client)

```python
# ElasticLoadBalancingv2Client usage example

from aiobotocore.session import get_session
from types_aiobotocore_elbv2.client import ElasticLoadBalancingv2Client

session = get_session()
async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("elbv2").exceptions` structure.

```python
# ElasticLoadBalancingv2Client.exceptions usage example

async with session.create_client("elbv2") as client:
    try:
        do_something(client)
    except (
            client.ALPNPolicyNotSupportedException,
        client.AllocationIdNotFoundException,
        client.AvailabilityZoneNotSupportedException,
        client.CaCertificatesBundleNotFoundException,
        client.CapacityDecreaseRequestsLimitExceededException,
        client.CapacityReservationPendingException,
        client.CapacityUnitsLimitExceededException,
        client.CertificateNotFoundException,
        client.ClientError,
        client.DeleteAssociationSameAccountException,
        client.DuplicateListenerException,
        client.DuplicateLoadBalancerNameException,
        client.DuplicateTagKeysException,
        client.DuplicateTargetGroupNameException,
        client.DuplicateTrustStoreNameException,
        client.HealthUnavailableException,
        client.IncompatibleProtocolsException,
        client.InsufficientCapacityException,
        client.InvalidCaCertificatesBundleException,
        client.InvalidConfigurationRequestException,
        client.InvalidLoadBalancerActionException,
        client.InvalidRevocationContentException,
        client.InvalidSchemeException,
        client.InvalidSecurityGroupException,
        client.InvalidSubnetException,
        client.InvalidTargetException,
        client.ListenerNotFoundException,
        client.LoadBalancerNotFoundException,
        client.OperationNotPermittedException,
        client.PriorRequestNotCompleteException,
        client.PriorityInUseException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.RevocationContentNotFoundException,
        client.RevocationIdNotFoundException,
        client.RuleNotFoundException,
        client.SSLPolicyNotFoundException,
        client.SubnetNotFoundException,
        client.TargetGroupAssociationLimitException,
        client.TargetGroupNotFoundException,
        client.TooManyActionsException,
        client.TooManyCertificatesException,
        client.TooManyListenersException,
        client.TooManyLoadBalancersException,
        client.TooManyRegistrationsForTargetIdException,
        client.TooManyRulesException,
        client.TooManyTagsException,
        client.TooManyTargetGroupsException,
        client.TooManyTargetsException,
        client.TooManyTrustStoreRevocationEntriesException,
        client.TooManyTrustStoresException,
        client.TooManyUniqueTargetGroupsPerLoadBalancerException,
        client.TrustStoreAssociationNotFoundException,
        client.TrustStoreInUseException,
        client.TrustStoreNotFoundException,
        client.TrustStoreNotReadyException,
        client.UnsupportedProtocolException,
    ) as e:
        print(e)
```

```python
# ElasticLoadBalancingv2Client usage type checking example

from types_aiobotocore_elbv2.client import Exceptions

def handle_error(exc: Exceptions.ALPNPolicyNotSupportedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("elbv2").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("elbv2").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/generate_presigned_url.html)

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



Type annotations and code completion for `#!python session.create_client("elbv2").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### add\_listener\_certificates

Adds the specified SSL server certificate to the certificate list for the
specified HTTPS or TLS listener.

Type annotations and code completion for `#!python session.create_client("elbv2").add_listener_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/add_listener_certificates.html)

```python
# add_listener_certificates method definition

await def add_listener_certificates(
    self,
    *,
    ListenerArn: str,
    Certificates: Sequence[CertificateTypeDef],  # (1)
) -> AddListenerCertificatesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
2. See [:material-code-braces: AddListenerCertificatesOutputTypeDef](./type_defs.md#addlistenercertificatesoutputtypedef) 


```python
# add_listener_certificates method usage example with argument unpacking

kwargs: AddListenerCertificatesInputRequestTypeDef = {  # (1)
    "ListenerArn": ...,
    "Certificates": ...,
}

parent.add_listener_certificates(**kwargs)
```

1. See [:material-code-braces: AddListenerCertificatesInputRequestTypeDef](./type_defs.md#addlistenercertificatesinputrequesttypedef) 

### add\_tags

Adds the specified tags to the specified Elastic Load Balancing resource.

Type annotations and code completion for `#!python session.create_client("elbv2").add_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/add_tags.html)

```python
# add_tags method definition

await def add_tags(
    self,
    *,
    ResourceArns: Sequence[str],
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# add_tags method usage example with argument unpacking

kwargs: AddTagsInputRequestTypeDef = {  # (1)
    "ResourceArns": ...,
    "Tags": ...,
}

parent.add_tags(**kwargs)
```

1. See [:material-code-braces: AddTagsInputRequestTypeDef](./type_defs.md#addtagsinputrequesttypedef) 

### add\_trust\_store\_revocations

Adds the specified revocation file to the specified trust store.

Type annotations and code completion for `#!python session.create_client("elbv2").add_trust_store_revocations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/add_trust_store_revocations.html)

```python
# add_trust_store_revocations method definition

await def add_trust_store_revocations(
    self,
    *,
    TrustStoreArn: str,
    RevocationContents: Sequence[RevocationContentTypeDef] = ...,  # (1)
) -> AddTrustStoreRevocationsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RevocationContentTypeDef](./type_defs.md#revocationcontenttypedef) 
2. See [:material-code-braces: AddTrustStoreRevocationsOutputTypeDef](./type_defs.md#addtruststorerevocationsoutputtypedef) 


```python
# add_trust_store_revocations method usage example with argument unpacking

kwargs: AddTrustStoreRevocationsInputRequestTypeDef = {  # (1)
    "TrustStoreArn": ...,
}

parent.add_trust_store_revocations(**kwargs)
```

1. See [:material-code-braces: AddTrustStoreRevocationsInputRequestTypeDef](./type_defs.md#addtruststorerevocationsinputrequesttypedef) 

### create\_listener

Creates a listener for the specified Application Load Balancer, Network Load
Balancer, or Gateway Load Balancer.

Type annotations and code completion for `#!python session.create_client("elbv2").create_listener` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/create_listener.html)

```python
# create_listener method definition

await def create_listener(
    self,
    *,
    LoadBalancerArn: str,
    DefaultActions: Sequence[ActionUnionTypeDef],  # (1)
    Protocol: ProtocolEnumType = ...,  # (2)
    Port: int = ...,
    SslPolicy: str = ...,
    Certificates: Sequence[CertificateTypeDef] = ...,  # (3)
    AlpnPolicy: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    MutualAuthentication: MutualAuthenticationAttributesTypeDef = ...,  # (5)
) -> CreateListenerOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
2. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
3. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: MutualAuthenticationAttributesTypeDef](./type_defs.md#mutualauthenticationattributestypedef) 
6. See [:material-code-braces: CreateListenerOutputTypeDef](./type_defs.md#createlisteneroutputtypedef) 


```python
# create_listener method usage example with argument unpacking

kwargs: CreateListenerInputRequestTypeDef = {  # (1)
    "LoadBalancerArn": ...,
    "DefaultActions": ...,
}

parent.create_listener(**kwargs)
```

1. See [:material-code-braces: CreateListenerInputRequestTypeDef](./type_defs.md#createlistenerinputrequesttypedef) 

### create\_load\_balancer

Creates an Application Load Balancer, Network Load Balancer, or Gateway Load
Balancer.

Type annotations and code completion for `#!python session.create_client("elbv2").create_load_balancer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/create_load_balancer.html)

```python
# create_load_balancer method definition

await def create_load_balancer(
    self,
    *,
    Name: str,
    Subnets: Sequence[str] = ...,
    SubnetMappings: Sequence[SubnetMappingTypeDef] = ...,  # (1)
    SecurityGroups: Sequence[str] = ...,
    Scheme: LoadBalancerSchemeEnumType = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    Type: LoadBalancerTypeEnumType = ...,  # (4)
    IpAddressType: IpAddressTypeType = ...,  # (5)
    CustomerOwnedIpv4Pool: str = ...,
    EnablePrefixForIpv6SourceNat: EnablePrefixForIpv6SourceNatEnumType = ...,  # (6)
) -> CreateLoadBalancerOutputTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: SubnetMappingTypeDef](./type_defs.md#subnetmappingtypedef) 
2. See [:material-code-brackets: LoadBalancerSchemeEnumType](./literals.md#loadbalancerschemeenumtype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: LoadBalancerTypeEnumType](./literals.md#loadbalancertypeenumtype) 
5. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
6. See [:material-code-brackets: EnablePrefixForIpv6SourceNatEnumType](./literals.md#enableprefixforipv6sourcenatenumtype) 
7. See [:material-code-braces: CreateLoadBalancerOutputTypeDef](./type_defs.md#createloadbalanceroutputtypedef) 


```python
# create_load_balancer method usage example with argument unpacking

kwargs: CreateLoadBalancerInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_load_balancer(**kwargs)
```

1. See [:material-code-braces: CreateLoadBalancerInputRequestTypeDef](./type_defs.md#createloadbalancerinputrequesttypedef) 

### create\_rule

Creates a rule for the specified listener.

Type annotations and code completion for `#!python session.create_client("elbv2").create_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/create_rule.html)

```python
# create_rule method definition

await def create_rule(
    self,
    *,
    ListenerArn: str,
    Conditions: Sequence[RuleConditionUnionTypeDef],  # (1)
    Priority: int,
    Actions: Sequence[ActionTypeDef],  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateRuleOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RuleConditionTypeDef](./type_defs.md#ruleconditiontypedef) [:material-code-braces: RuleConditionOutputTypeDef](./type_defs.md#ruleconditionoutputtypedef) 
2. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateRuleOutputTypeDef](./type_defs.md#createruleoutputtypedef) 


```python
# create_rule method usage example with argument unpacking

kwargs: CreateRuleInputRequestTypeDef = {  # (1)
    "ListenerArn": ...,
    "Conditions": ...,
    "Priority": ...,
    "Actions": ...,
}

parent.create_rule(**kwargs)
```

1. See [:material-code-braces: CreateRuleInputRequestTypeDef](./type_defs.md#createruleinputrequesttypedef) 

### create\_target\_group

Creates a target group.

Type annotations and code completion for `#!python session.create_client("elbv2").create_target_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/create_target_group.html)

```python
# create_target_group method definition

await def create_target_group(
    self,
    *,
    Name: str,
    Protocol: ProtocolEnumType = ...,  # (1)
    ProtocolVersion: str = ...,
    Port: int = ...,
    VpcId: str = ...,
    HealthCheckProtocol: ProtocolEnumType = ...,  # (1)
    HealthCheckPort: str = ...,
    HealthCheckEnabled: bool = ...,
    HealthCheckPath: str = ...,
    HealthCheckIntervalSeconds: int = ...,
    HealthCheckTimeoutSeconds: int = ...,
    HealthyThresholdCount: int = ...,
    UnhealthyThresholdCount: int = ...,
    Matcher: MatcherTypeDef = ...,  # (3)
    TargetType: TargetTypeEnumType = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
    IpAddressType: TargetGroupIpAddressTypeEnumType = ...,  # (6)
) -> CreateTargetGroupOutputTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
2. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
3. See [:material-code-braces: MatcherTypeDef](./type_defs.md#matchertypedef) 
4. See [:material-code-brackets: TargetTypeEnumType](./literals.md#targettypeenumtype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-brackets: TargetGroupIpAddressTypeEnumType](./literals.md#targetgroupipaddresstypeenumtype) 
7. See [:material-code-braces: CreateTargetGroupOutputTypeDef](./type_defs.md#createtargetgroupoutputtypedef) 


```python
# create_target_group method usage example with argument unpacking

kwargs: CreateTargetGroupInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_target_group(**kwargs)
```

1. See [:material-code-braces: CreateTargetGroupInputRequestTypeDef](./type_defs.md#createtargetgroupinputrequesttypedef) 

### create\_trust\_store

Creates a trust store.

Type annotations and code completion for `#!python session.create_client("elbv2").create_trust_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/create_trust_store.html)

```python
# create_trust_store method definition

await def create_trust_store(
    self,
    *,
    Name: str,
    CaCertificatesBundleS3Bucket: str,
    CaCertificatesBundleS3Key: str,
    CaCertificatesBundleS3ObjectVersion: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateTrustStoreOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateTrustStoreOutputTypeDef](./type_defs.md#createtruststoreoutputtypedef) 


```python
# create_trust_store method usage example with argument unpacking

kwargs: CreateTrustStoreInputRequestTypeDef = {  # (1)
    "Name": ...,
    "CaCertificatesBundleS3Bucket": ...,
    "CaCertificatesBundleS3Key": ...,
}

parent.create_trust_store(**kwargs)
```

1. See [:material-code-braces: CreateTrustStoreInputRequestTypeDef](./type_defs.md#createtruststoreinputrequesttypedef) 

### delete\_listener

Deletes the specified listener.

Type annotations and code completion for `#!python session.create_client("elbv2").delete_listener` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/delete_listener.html)

```python
# delete_listener method definition

await def delete_listener(
    self,
    *,
    ListenerArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_listener method usage example with argument unpacking

kwargs: DeleteListenerInputRequestTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.delete_listener(**kwargs)
```

1. See [:material-code-braces: DeleteListenerInputRequestTypeDef](./type_defs.md#deletelistenerinputrequesttypedef) 

### delete\_load\_balancer

Deletes the specified Application Load Balancer, Network Load Balancer, or
Gateway Load Balancer.

Type annotations and code completion for `#!python session.create_client("elbv2").delete_load_balancer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/delete_load_balancer.html)

```python
# delete_load_balancer method definition

await def delete_load_balancer(
    self,
    *,
    LoadBalancerArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_load_balancer method usage example with argument unpacking

kwargs: DeleteLoadBalancerInputRequestTypeDef = {  # (1)
    "LoadBalancerArn": ...,
}

parent.delete_load_balancer(**kwargs)
```

1. See [:material-code-braces: DeleteLoadBalancerInputRequestTypeDef](./type_defs.md#deleteloadbalancerinputrequesttypedef) 

### delete\_rule

Deletes the specified rule.

Type annotations and code completion for `#!python session.create_client("elbv2").delete_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/delete_rule.html)

```python
# delete_rule method definition

await def delete_rule(
    self,
    *,
    RuleArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_rule method usage example with argument unpacking

kwargs: DeleteRuleInputRequestTypeDef = {  # (1)
    "RuleArn": ...,
}

parent.delete_rule(**kwargs)
```

1. See [:material-code-braces: DeleteRuleInputRequestTypeDef](./type_defs.md#deleteruleinputrequesttypedef) 

### delete\_shared\_trust\_store\_association

Deletes a shared trust store association.

Type annotations and code completion for `#!python session.create_client("elbv2").delete_shared_trust_store_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/delete_shared_trust_store_association.html)

```python
# delete_shared_trust_store_association method definition

await def delete_shared_trust_store_association(
    self,
    *,
    TrustStoreArn: str,
    ResourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_shared_trust_store_association method usage example with argument unpacking

kwargs: DeleteSharedTrustStoreAssociationInputRequestTypeDef = {  # (1)
    "TrustStoreArn": ...,
    "ResourceArn": ...,
}

parent.delete_shared_trust_store_association(**kwargs)
```

1. See [:material-code-braces: DeleteSharedTrustStoreAssociationInputRequestTypeDef](./type_defs.md#deletesharedtruststoreassociationinputrequesttypedef) 

### delete\_target\_group

Deletes the specified target group.

Type annotations and code completion for `#!python session.create_client("elbv2").delete_target_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/delete_target_group.html)

```python
# delete_target_group method definition

await def delete_target_group(
    self,
    *,
    TargetGroupArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_target_group method usage example with argument unpacking

kwargs: DeleteTargetGroupInputRequestTypeDef = {  # (1)
    "TargetGroupArn": ...,
}

parent.delete_target_group(**kwargs)
```

1. See [:material-code-braces: DeleteTargetGroupInputRequestTypeDef](./type_defs.md#deletetargetgroupinputrequesttypedef) 

### delete\_trust\_store

Deletes a trust store.

Type annotations and code completion for `#!python session.create_client("elbv2").delete_trust_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/delete_trust_store.html)

```python
# delete_trust_store method definition

await def delete_trust_store(
    self,
    *,
    TrustStoreArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_trust_store method usage example with argument unpacking

kwargs: DeleteTrustStoreInputRequestTypeDef = {  # (1)
    "TrustStoreArn": ...,
}

parent.delete_trust_store(**kwargs)
```

1. See [:material-code-braces: DeleteTrustStoreInputRequestTypeDef](./type_defs.md#deletetruststoreinputrequesttypedef) 

### deregister\_targets

Deregisters the specified targets from the specified target group.

Type annotations and code completion for `#!python session.create_client("elbv2").deregister_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/deregister_targets.html)

```python
# deregister_targets method definition

await def deregister_targets(
    self,
    *,
    TargetGroupArn: str,
    Targets: Sequence[TargetDescriptionTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TargetDescriptionTypeDef](./type_defs.md#targetdescriptiontypedef) 


```python
# deregister_targets method usage example with argument unpacking

kwargs: DeregisterTargetsInputRequestTypeDef = {  # (1)
    "TargetGroupArn": ...,
    "Targets": ...,
}

parent.deregister_targets(**kwargs)
```

1. See [:material-code-braces: DeregisterTargetsInputRequestTypeDef](./type_defs.md#deregistertargetsinputrequesttypedef) 

### describe\_account\_limits

Describes the current Elastic Load Balancing resource limits for your Amazon
Web Services account.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_account_limits` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_account_limits.html)

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

### describe\_capacity\_reservation

Describes the capacity reservation status for the specified load balancer.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_capacity_reservation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_capacity_reservation.html)

```python
# describe_capacity_reservation method definition

await def describe_capacity_reservation(
    self,
    *,
    LoadBalancerArn: str,
) -> DescribeCapacityReservationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCapacityReservationOutputTypeDef](./type_defs.md#describecapacityreservationoutputtypedef) 


```python
# describe_capacity_reservation method usage example with argument unpacking

kwargs: DescribeCapacityReservationInputRequestTypeDef = {  # (1)
    "LoadBalancerArn": ...,
}

parent.describe_capacity_reservation(**kwargs)
```

1. See [:material-code-braces: DescribeCapacityReservationInputRequestTypeDef](./type_defs.md#describecapacityreservationinputrequesttypedef) 

### describe\_listener\_attributes

Describes the attributes for the specified listener.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_listener_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_listener_attributes.html)

```python
# describe_listener_attributes method definition

await def describe_listener_attributes(
    self,
    *,
    ListenerArn: str,
) -> DescribeListenerAttributesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeListenerAttributesOutputTypeDef](./type_defs.md#describelistenerattributesoutputtypedef) 


```python
# describe_listener_attributes method usage example with argument unpacking

kwargs: DescribeListenerAttributesInputRequestTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.describe_listener_attributes(**kwargs)
```

1. See [:material-code-braces: DescribeListenerAttributesInputRequestTypeDef](./type_defs.md#describelistenerattributesinputrequesttypedef) 

### describe\_listener\_certificates

Describes the default certificate and the certificate list for the specified
HTTPS or TLS listener.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_listener_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_listener_certificates.html)

```python
# describe_listener_certificates method definition

await def describe_listener_certificates(
    self,
    *,
    ListenerArn: str,
    Marker: str = ...,
    PageSize: int = ...,
) -> DescribeListenerCertificatesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeListenerCertificatesOutputTypeDef](./type_defs.md#describelistenercertificatesoutputtypedef) 


```python
# describe_listener_certificates method usage example with argument unpacking

kwargs: DescribeListenerCertificatesInputRequestTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.describe_listener_certificates(**kwargs)
```

1. See [:material-code-braces: DescribeListenerCertificatesInputRequestTypeDef](./type_defs.md#describelistenercertificatesinputrequesttypedef) 

### describe\_listeners

Describes the specified listeners or the listeners for the specified
Application Load Balancer, Network Load Balancer, or Gateway Load Balancer.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_listeners` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_listeners.html)

```python
# describe_listeners method definition

await def describe_listeners(
    self,
    *,
    LoadBalancerArn: str = ...,
    ListenerArns: Sequence[str] = ...,
    Marker: str = ...,
    PageSize: int = ...,
) -> DescribeListenersOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeListenersOutputTypeDef](./type_defs.md#describelistenersoutputtypedef) 


```python
# describe_listeners method usage example with argument unpacking

kwargs: DescribeListenersInputRequestTypeDef = {  # (1)
    "LoadBalancerArn": ...,
}

parent.describe_listeners(**kwargs)
```

1. See [:material-code-braces: DescribeListenersInputRequestTypeDef](./type_defs.md#describelistenersinputrequesttypedef) 

### describe\_load\_balancer\_attributes

Describes the attributes for the specified Application Load Balancer, Network
Load Balancer, or Gateway Load Balancer.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_load_balancer_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_load_balancer_attributes.html)

```python
# describe_load_balancer_attributes method definition

await def describe_load_balancer_attributes(
    self,
    *,
    LoadBalancerArn: str,
) -> DescribeLoadBalancerAttributesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLoadBalancerAttributesOutputTypeDef](./type_defs.md#describeloadbalancerattributesoutputtypedef) 


```python
# describe_load_balancer_attributes method usage example with argument unpacking

kwargs: DescribeLoadBalancerAttributesInputRequestTypeDef = {  # (1)
    "LoadBalancerArn": ...,
}

parent.describe_load_balancer_attributes(**kwargs)
```

1. See [:material-code-braces: DescribeLoadBalancerAttributesInputRequestTypeDef](./type_defs.md#describeloadbalancerattributesinputrequesttypedef) 

### describe\_load\_balancers

Describes the specified load balancers or all of your load balancers.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_load_balancers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_load_balancers.html)

```python
# describe_load_balancers method definition

await def describe_load_balancers(
    self,
    *,
    LoadBalancerArns: Sequence[str] = ...,
    Names: Sequence[str] = ...,
    Marker: str = ...,
    PageSize: int = ...,
) -> DescribeLoadBalancersOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLoadBalancersOutputTypeDef](./type_defs.md#describeloadbalancersoutputtypedef) 


```python
# describe_load_balancers method usage example with argument unpacking

kwargs: DescribeLoadBalancersInputRequestTypeDef = {  # (1)
    "LoadBalancerArns": ...,
}

parent.describe_load_balancers(**kwargs)
```

1. See [:material-code-braces: DescribeLoadBalancersInputRequestTypeDef](./type_defs.md#describeloadbalancersinputrequesttypedef) 

### describe\_rules

Describes the specified rules or the rules for the specified listener.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_rules.html)

```python
# describe_rules method definition

await def describe_rules(
    self,
    *,
    ListenerArn: str = ...,
    RuleArns: Sequence[str] = ...,
    Marker: str = ...,
    PageSize: int = ...,
) -> DescribeRulesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRulesOutputTypeDef](./type_defs.md#describerulesoutputtypedef) 


```python
# describe_rules method usage example with argument unpacking

kwargs: DescribeRulesInputRequestTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.describe_rules(**kwargs)
```

1. See [:material-code-braces: DescribeRulesInputRequestTypeDef](./type_defs.md#describerulesinputrequesttypedef) 

### describe\_ssl\_policies

Describes the specified policies or all policies used for SSL negotiation.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_ssl_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_ssl_policies.html)

```python
# describe_ssl_policies method definition

await def describe_ssl_policies(
    self,
    *,
    Names: Sequence[str] = ...,
    Marker: str = ...,
    PageSize: int = ...,
    LoadBalancerType: LoadBalancerTypeEnumType = ...,  # (1)
) -> DescribeSSLPoliciesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LoadBalancerTypeEnumType](./literals.md#loadbalancertypeenumtype) 
2. See [:material-code-braces: DescribeSSLPoliciesOutputTypeDef](./type_defs.md#describesslpoliciesoutputtypedef) 


```python
# describe_ssl_policies method usage example with argument unpacking

kwargs: DescribeSSLPoliciesInputRequestTypeDef = {  # (1)
    "Names": ...,
}

parent.describe_ssl_policies(**kwargs)
```

1. See [:material-code-braces: DescribeSSLPoliciesInputRequestTypeDef](./type_defs.md#describesslpoliciesinputrequesttypedef) 

### describe\_tags

Describes the tags for the specified Elastic Load Balancing resources.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_tags.html)

```python
# describe_tags method definition

await def describe_tags(
    self,
    *,
    ResourceArns: Sequence[str],
) -> DescribeTagsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTagsOutputTypeDef](./type_defs.md#describetagsoutputtypedef) 


```python
# describe_tags method usage example with argument unpacking

kwargs: DescribeTagsInputRequestTypeDef = {  # (1)
    "ResourceArns": ...,
}

parent.describe_tags(**kwargs)
```

1. See [:material-code-braces: DescribeTagsInputRequestTypeDef](./type_defs.md#describetagsinputrequesttypedef) 

### describe\_target\_group\_attributes

Describes the attributes for the specified target group.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_target_group_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_target_group_attributes.html)

```python
# describe_target_group_attributes method definition

await def describe_target_group_attributes(
    self,
    *,
    TargetGroupArn: str,
) -> DescribeTargetGroupAttributesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTargetGroupAttributesOutputTypeDef](./type_defs.md#describetargetgroupattributesoutputtypedef) 


```python
# describe_target_group_attributes method usage example with argument unpacking

kwargs: DescribeTargetGroupAttributesInputRequestTypeDef = {  # (1)
    "TargetGroupArn": ...,
}

parent.describe_target_group_attributes(**kwargs)
```

1. See [:material-code-braces: DescribeTargetGroupAttributesInputRequestTypeDef](./type_defs.md#describetargetgroupattributesinputrequesttypedef) 

### describe\_target\_groups

Describes the specified target groups or all of your target groups.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_target_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_target_groups.html)

```python
# describe_target_groups method definition

await def describe_target_groups(
    self,
    *,
    LoadBalancerArn: str = ...,
    TargetGroupArns: Sequence[str] = ...,
    Names: Sequence[str] = ...,
    Marker: str = ...,
    PageSize: int = ...,
) -> DescribeTargetGroupsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTargetGroupsOutputTypeDef](./type_defs.md#describetargetgroupsoutputtypedef) 


```python
# describe_target_groups method usage example with argument unpacking

kwargs: DescribeTargetGroupsInputRequestTypeDef = {  # (1)
    "LoadBalancerArn": ...,
}

parent.describe_target_groups(**kwargs)
```

1. See [:material-code-braces: DescribeTargetGroupsInputRequestTypeDef](./type_defs.md#describetargetgroupsinputrequesttypedef) 

### describe\_target\_health

Describes the health of the specified targets or all of your targets.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_target_health` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_target_health.html)

```python
# describe_target_health method definition

await def describe_target_health(
    self,
    *,
    TargetGroupArn: str,
    Targets: Sequence[TargetDescriptionTypeDef] = ...,  # (1)
    Include: Sequence[DescribeTargetHealthInputIncludeEnumType] = ...,  # (2)
) -> DescribeTargetHealthOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TargetDescriptionTypeDef](./type_defs.md#targetdescriptiontypedef) 
2. See [:material-code-brackets: DescribeTargetHealthInputIncludeEnumType](./literals.md#describetargethealthinputincludeenumtype) 
3. See [:material-code-braces: DescribeTargetHealthOutputTypeDef](./type_defs.md#describetargethealthoutputtypedef) 


```python
# describe_target_health method usage example with argument unpacking

kwargs: DescribeTargetHealthInputRequestTypeDef = {  # (1)
    "TargetGroupArn": ...,
}

parent.describe_target_health(**kwargs)
```

1. See [:material-code-braces: DescribeTargetHealthInputRequestTypeDef](./type_defs.md#describetargethealthinputrequesttypedef) 

### describe\_trust\_store\_associations

Describes all resources associated with the specified trust store.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_trust_store_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_trust_store_associations.html)

```python
# describe_trust_store_associations method definition

await def describe_trust_store_associations(
    self,
    *,
    TrustStoreArn: str,
    Marker: str = ...,
    PageSize: int = ...,
) -> DescribeTrustStoreAssociationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrustStoreAssociationsOutputTypeDef](./type_defs.md#describetruststoreassociationsoutputtypedef) 


```python
# describe_trust_store_associations method usage example with argument unpacking

kwargs: DescribeTrustStoreAssociationsInputRequestTypeDef = {  # (1)
    "TrustStoreArn": ...,
}

parent.describe_trust_store_associations(**kwargs)
```

1. See [:material-code-braces: DescribeTrustStoreAssociationsInputRequestTypeDef](./type_defs.md#describetruststoreassociationsinputrequesttypedef) 

### describe\_trust\_store\_revocations

Describes the revocation files in use by the specified trust store or
revocation files.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_trust_store_revocations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_trust_store_revocations.html)

```python
# describe_trust_store_revocations method definition

await def describe_trust_store_revocations(
    self,
    *,
    TrustStoreArn: str,
    RevocationIds: Sequence[int] = ...,
    Marker: str = ...,
    PageSize: int = ...,
) -> DescribeTrustStoreRevocationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrustStoreRevocationsOutputTypeDef](./type_defs.md#describetruststorerevocationsoutputtypedef) 


```python
# describe_trust_store_revocations method usage example with argument unpacking

kwargs: DescribeTrustStoreRevocationsInputRequestTypeDef = {  # (1)
    "TrustStoreArn": ...,
}

parent.describe_trust_store_revocations(**kwargs)
```

1. See [:material-code-braces: DescribeTrustStoreRevocationsInputRequestTypeDef](./type_defs.md#describetruststorerevocationsinputrequesttypedef) 

### describe\_trust\_stores

Describes all trust stores for the specified account.

Type annotations and code completion for `#!python session.create_client("elbv2").describe_trust_stores` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/describe_trust_stores.html)

```python
# describe_trust_stores method definition

await def describe_trust_stores(
    self,
    *,
    TrustStoreArns: Sequence[str] = ...,
    Names: Sequence[str] = ...,
    Marker: str = ...,
    PageSize: int = ...,
) -> DescribeTrustStoresOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrustStoresOutputTypeDef](./type_defs.md#describetruststoresoutputtypedef) 


```python
# describe_trust_stores method usage example with argument unpacking

kwargs: DescribeTrustStoresInputRequestTypeDef = {  # (1)
    "TrustStoreArns": ...,
}

parent.describe_trust_stores(**kwargs)
```

1. See [:material-code-braces: DescribeTrustStoresInputRequestTypeDef](./type_defs.md#describetruststoresinputrequesttypedef) 

### get\_resource\_policy

Retrieves the resource policy for a specified resource.

Type annotations and code completion for `#!python session.create_client("elbv2").get_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/get_resource_policy.html)

```python
# get_resource_policy method definition

await def get_resource_policy(
    self,
    *,
    ResourceArn: str,
) -> GetResourcePolicyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourcePolicyOutputTypeDef](./type_defs.md#getresourcepolicyoutputtypedef) 


```python
# get_resource_policy method usage example with argument unpacking

kwargs: GetResourcePolicyInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_resource_policy(**kwargs)
```

1. See [:material-code-braces: GetResourcePolicyInputRequestTypeDef](./type_defs.md#getresourcepolicyinputrequesttypedef) 

### get\_trust\_store\_ca\_certificates\_bundle

Retrieves the ca certificate bundle.

Type annotations and code completion for `#!python session.create_client("elbv2").get_trust_store_ca_certificates_bundle` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/get_trust_store_ca_certificates_bundle.html)

```python
# get_trust_store_ca_certificates_bundle method definition

await def get_trust_store_ca_certificates_bundle(
    self,
    *,
    TrustStoreArn: str,
) -> GetTrustStoreCaCertificatesBundleOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTrustStoreCaCertificatesBundleOutputTypeDef](./type_defs.md#gettruststorecacertificatesbundleoutputtypedef) 


```python
# get_trust_store_ca_certificates_bundle method usage example with argument unpacking

kwargs: GetTrustStoreCaCertificatesBundleInputRequestTypeDef = {  # (1)
    "TrustStoreArn": ...,
}

parent.get_trust_store_ca_certificates_bundle(**kwargs)
```

1. See [:material-code-braces: GetTrustStoreCaCertificatesBundleInputRequestTypeDef](./type_defs.md#gettruststorecacertificatesbundleinputrequesttypedef) 

### get\_trust\_store\_revocation\_content

Retrieves the specified revocation file.

Type annotations and code completion for `#!python session.create_client("elbv2").get_trust_store_revocation_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/get_trust_store_revocation_content.html)

```python
# get_trust_store_revocation_content method definition

await def get_trust_store_revocation_content(
    self,
    *,
    TrustStoreArn: str,
    RevocationId: int,
) -> GetTrustStoreRevocationContentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTrustStoreRevocationContentOutputTypeDef](./type_defs.md#gettruststorerevocationcontentoutputtypedef) 


```python
# get_trust_store_revocation_content method usage example with argument unpacking

kwargs: GetTrustStoreRevocationContentInputRequestTypeDef = {  # (1)
    "TrustStoreArn": ...,
    "RevocationId": ...,
}

parent.get_trust_store_revocation_content(**kwargs)
```

1. See [:material-code-braces: GetTrustStoreRevocationContentInputRequestTypeDef](./type_defs.md#gettruststorerevocationcontentinputrequesttypedef) 

### modify\_capacity\_reservation

Modifies the capacity reservation of the specified load balancer.

Type annotations and code completion for `#!python session.create_client("elbv2").modify_capacity_reservation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/modify_capacity_reservation.html)

```python
# modify_capacity_reservation method definition

await def modify_capacity_reservation(
    self,
    *,
    LoadBalancerArn: str,
    MinimumLoadBalancerCapacity: MinimumLoadBalancerCapacityTypeDef = ...,  # (1)
    ResetCapacityReservation: bool = ...,
) -> ModifyCapacityReservationOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MinimumLoadBalancerCapacityTypeDef](./type_defs.md#minimumloadbalancercapacitytypedef) 
2. See [:material-code-braces: ModifyCapacityReservationOutputTypeDef](./type_defs.md#modifycapacityreservationoutputtypedef) 


```python
# modify_capacity_reservation method usage example with argument unpacking

kwargs: ModifyCapacityReservationInputRequestTypeDef = {  # (1)
    "LoadBalancerArn": ...,
}

parent.modify_capacity_reservation(**kwargs)
```

1. See [:material-code-braces: ModifyCapacityReservationInputRequestTypeDef](./type_defs.md#modifycapacityreservationinputrequesttypedef) 

### modify\_listener

Replaces the specified properties of the specified listener.

Type annotations and code completion for `#!python session.create_client("elbv2").modify_listener` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/modify_listener.html)

```python
# modify_listener method definition

await def modify_listener(
    self,
    *,
    ListenerArn: str,
    Port: int = ...,
    Protocol: ProtocolEnumType = ...,  # (1)
    SslPolicy: str = ...,
    Certificates: Sequence[CertificateTypeDef] = ...,  # (2)
    DefaultActions: Sequence[ActionTypeDef] = ...,  # (3)
    AlpnPolicy: Sequence[str] = ...,
    MutualAuthentication: MutualAuthenticationAttributesTypeDef = ...,  # (4)
) -> ModifyListenerOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
2. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
3. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
4. See [:material-code-braces: MutualAuthenticationAttributesTypeDef](./type_defs.md#mutualauthenticationattributestypedef) 
5. See [:material-code-braces: ModifyListenerOutputTypeDef](./type_defs.md#modifylisteneroutputtypedef) 


```python
# modify_listener method usage example with argument unpacking

kwargs: ModifyListenerInputRequestTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.modify_listener(**kwargs)
```

1. See [:material-code-braces: ModifyListenerInputRequestTypeDef](./type_defs.md#modifylistenerinputrequesttypedef) 

### modify\_listener\_attributes

Modifies the specified attributes of the specified listener.

Type annotations and code completion for `#!python session.create_client("elbv2").modify_listener_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/modify_listener_attributes.html)

```python
# modify_listener_attributes method definition

await def modify_listener_attributes(
    self,
    *,
    ListenerArn: str,
    Attributes: Sequence[ListenerAttributeTypeDef],  # (1)
) -> ModifyListenerAttributesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListenerAttributeTypeDef](./type_defs.md#listenerattributetypedef) 
2. See [:material-code-braces: ModifyListenerAttributesOutputTypeDef](./type_defs.md#modifylistenerattributesoutputtypedef) 


```python
# modify_listener_attributes method usage example with argument unpacking

kwargs: ModifyListenerAttributesInputRequestTypeDef = {  # (1)
    "ListenerArn": ...,
    "Attributes": ...,
}

parent.modify_listener_attributes(**kwargs)
```

1. See [:material-code-braces: ModifyListenerAttributesInputRequestTypeDef](./type_defs.md#modifylistenerattributesinputrequesttypedef) 

### modify\_load\_balancer\_attributes

Modifies the specified attributes of the specified Application Load Balancer,
Network Load Balancer, or Gateway Load Balancer.

Type annotations and code completion for `#!python session.create_client("elbv2").modify_load_balancer_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/modify_load_balancer_attributes.html)

```python
# modify_load_balancer_attributes method definition

await def modify_load_balancer_attributes(
    self,
    *,
    LoadBalancerArn: str,
    Attributes: Sequence[LoadBalancerAttributeTypeDef],  # (1)
) -> ModifyLoadBalancerAttributesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LoadBalancerAttributeTypeDef](./type_defs.md#loadbalancerattributetypedef) 
2. See [:material-code-braces: ModifyLoadBalancerAttributesOutputTypeDef](./type_defs.md#modifyloadbalancerattributesoutputtypedef) 


```python
# modify_load_balancer_attributes method usage example with argument unpacking

kwargs: ModifyLoadBalancerAttributesInputRequestTypeDef = {  # (1)
    "LoadBalancerArn": ...,
    "Attributes": ...,
}

parent.modify_load_balancer_attributes(**kwargs)
```

1. See [:material-code-braces: ModifyLoadBalancerAttributesInputRequestTypeDef](./type_defs.md#modifyloadbalancerattributesinputrequesttypedef) 

### modify\_rule

Replaces the specified properties of the specified rule.

Type annotations and code completion for `#!python session.create_client("elbv2").modify_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/modify_rule.html)

```python
# modify_rule method definition

await def modify_rule(
    self,
    *,
    RuleArn: str,
    Conditions: Sequence[RuleConditionTypeDef] = ...,  # (1)
    Actions: Sequence[ActionTypeDef] = ...,  # (2)
) -> ModifyRuleOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RuleConditionTypeDef](./type_defs.md#ruleconditiontypedef) 
2. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
3. See [:material-code-braces: ModifyRuleOutputTypeDef](./type_defs.md#modifyruleoutputtypedef) 


```python
# modify_rule method usage example with argument unpacking

kwargs: ModifyRuleInputRequestTypeDef = {  # (1)
    "RuleArn": ...,
}

parent.modify_rule(**kwargs)
```

1. See [:material-code-braces: ModifyRuleInputRequestTypeDef](./type_defs.md#modifyruleinputrequesttypedef) 

### modify\_target\_group

Modifies the health checks used when evaluating the health state of the targets
in the specified target group.

Type annotations and code completion for `#!python session.create_client("elbv2").modify_target_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/modify_target_group.html)

```python
# modify_target_group method definition

await def modify_target_group(
    self,
    *,
    TargetGroupArn: str,
    HealthCheckProtocol: ProtocolEnumType = ...,  # (1)
    HealthCheckPort: str = ...,
    HealthCheckPath: str = ...,
    HealthCheckEnabled: bool = ...,
    HealthCheckIntervalSeconds: int = ...,
    HealthCheckTimeoutSeconds: int = ...,
    HealthyThresholdCount: int = ...,
    UnhealthyThresholdCount: int = ...,
    Matcher: MatcherTypeDef = ...,  # (2)
) -> ModifyTargetGroupOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
2. See [:material-code-braces: MatcherTypeDef](./type_defs.md#matchertypedef) 
3. See [:material-code-braces: ModifyTargetGroupOutputTypeDef](./type_defs.md#modifytargetgroupoutputtypedef) 


```python
# modify_target_group method usage example with argument unpacking

kwargs: ModifyTargetGroupInputRequestTypeDef = {  # (1)
    "TargetGroupArn": ...,
}

parent.modify_target_group(**kwargs)
```

1. See [:material-code-braces: ModifyTargetGroupInputRequestTypeDef](./type_defs.md#modifytargetgroupinputrequesttypedef) 

### modify\_target\_group\_attributes

Modifies the specified attributes of the specified target group.

Type annotations and code completion for `#!python session.create_client("elbv2").modify_target_group_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/modify_target_group_attributes.html)

```python
# modify_target_group_attributes method definition

await def modify_target_group_attributes(
    self,
    *,
    TargetGroupArn: str,
    Attributes: Sequence[TargetGroupAttributeTypeDef],  # (1)
) -> ModifyTargetGroupAttributesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TargetGroupAttributeTypeDef](./type_defs.md#targetgroupattributetypedef) 
2. See [:material-code-braces: ModifyTargetGroupAttributesOutputTypeDef](./type_defs.md#modifytargetgroupattributesoutputtypedef) 


```python
# modify_target_group_attributes method usage example with argument unpacking

kwargs: ModifyTargetGroupAttributesInputRequestTypeDef = {  # (1)
    "TargetGroupArn": ...,
    "Attributes": ...,
}

parent.modify_target_group_attributes(**kwargs)
```

1. See [:material-code-braces: ModifyTargetGroupAttributesInputRequestTypeDef](./type_defs.md#modifytargetgroupattributesinputrequesttypedef) 

### modify\_trust\_store

Update the ca certificate bundle for the specified trust store.

Type annotations and code completion for `#!python session.create_client("elbv2").modify_trust_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/modify_trust_store.html)

```python
# modify_trust_store method definition

await def modify_trust_store(
    self,
    *,
    TrustStoreArn: str,
    CaCertificatesBundleS3Bucket: str,
    CaCertificatesBundleS3Key: str,
    CaCertificatesBundleS3ObjectVersion: str = ...,
) -> ModifyTrustStoreOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyTrustStoreOutputTypeDef](./type_defs.md#modifytruststoreoutputtypedef) 


```python
# modify_trust_store method usage example with argument unpacking

kwargs: ModifyTrustStoreInputRequestTypeDef = {  # (1)
    "TrustStoreArn": ...,
    "CaCertificatesBundleS3Bucket": ...,
    "CaCertificatesBundleS3Key": ...,
}

parent.modify_trust_store(**kwargs)
```

1. See [:material-code-braces: ModifyTrustStoreInputRequestTypeDef](./type_defs.md#modifytruststoreinputrequesttypedef) 

### register\_targets

Registers the specified targets with the specified target group.

Type annotations and code completion for `#!python session.create_client("elbv2").register_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/register_targets.html)

```python
# register_targets method definition

await def register_targets(
    self,
    *,
    TargetGroupArn: str,
    Targets: Sequence[TargetDescriptionTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TargetDescriptionTypeDef](./type_defs.md#targetdescriptiontypedef) 


```python
# register_targets method usage example with argument unpacking

kwargs: RegisterTargetsInputRequestTypeDef = {  # (1)
    "TargetGroupArn": ...,
    "Targets": ...,
}

parent.register_targets(**kwargs)
```

1. See [:material-code-braces: RegisterTargetsInputRequestTypeDef](./type_defs.md#registertargetsinputrequesttypedef) 

### remove\_listener\_certificates

Removes the specified certificate from the certificate list for the specified
HTTPS or TLS listener.

Type annotations and code completion for `#!python session.create_client("elbv2").remove_listener_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/remove_listener_certificates.html)

```python
# remove_listener_certificates method definition

await def remove_listener_certificates(
    self,
    *,
    ListenerArn: str,
    Certificates: Sequence[CertificateTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 


```python
# remove_listener_certificates method usage example with argument unpacking

kwargs: RemoveListenerCertificatesInputRequestTypeDef = {  # (1)
    "ListenerArn": ...,
    "Certificates": ...,
}

parent.remove_listener_certificates(**kwargs)
```

1. See [:material-code-braces: RemoveListenerCertificatesInputRequestTypeDef](./type_defs.md#removelistenercertificatesinputrequesttypedef) 

### remove\_tags

Removes the specified tags from the specified Elastic Load Balancing resources.

Type annotations and code completion for `#!python session.create_client("elbv2").remove_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/remove_tags.html)

```python
# remove_tags method definition

await def remove_tags(
    self,
    *,
    ResourceArns: Sequence[str],
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# remove_tags method usage example with argument unpacking

kwargs: RemoveTagsInputRequestTypeDef = {  # (1)
    "ResourceArns": ...,
    "TagKeys": ...,
}

parent.remove_tags(**kwargs)
```

1. See [:material-code-braces: RemoveTagsInputRequestTypeDef](./type_defs.md#removetagsinputrequesttypedef) 

### remove\_trust\_store\_revocations

Removes the specified revocation file from the specified trust store.

Type annotations and code completion for `#!python session.create_client("elbv2").remove_trust_store_revocations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/remove_trust_store_revocations.html)

```python
# remove_trust_store_revocations method definition

await def remove_trust_store_revocations(
    self,
    *,
    TrustStoreArn: str,
    RevocationIds: Sequence[int],
) -> Dict[str, Any]:
    ...
```



```python
# remove_trust_store_revocations method usage example with argument unpacking

kwargs: RemoveTrustStoreRevocationsInputRequestTypeDef = {  # (1)
    "TrustStoreArn": ...,
    "RevocationIds": ...,
}

parent.remove_trust_store_revocations(**kwargs)
```

1. See [:material-code-braces: RemoveTrustStoreRevocationsInputRequestTypeDef](./type_defs.md#removetruststorerevocationsinputrequesttypedef) 

### set\_ip\_address\_type

Sets the type of IP addresses used by the subnets of the specified load
balancer.

Type annotations and code completion for `#!python session.create_client("elbv2").set_ip_address_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/set_ip_address_type.html)

```python
# set_ip_address_type method definition

await def set_ip_address_type(
    self,
    *,
    LoadBalancerArn: str,
    IpAddressType: IpAddressTypeType,  # (1)
) -> SetIpAddressTypeOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
2. See [:material-code-braces: SetIpAddressTypeOutputTypeDef](./type_defs.md#setipaddresstypeoutputtypedef) 


```python
# set_ip_address_type method usage example with argument unpacking

kwargs: SetIpAddressTypeInputRequestTypeDef = {  # (1)
    "LoadBalancerArn": ...,
    "IpAddressType": ...,
}

parent.set_ip_address_type(**kwargs)
```

1. See [:material-code-braces: SetIpAddressTypeInputRequestTypeDef](./type_defs.md#setipaddresstypeinputrequesttypedef) 

### set\_rule\_priorities

Sets the priorities of the specified rules.

Type annotations and code completion for `#!python session.create_client("elbv2").set_rule_priorities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/set_rule_priorities.html)

```python
# set_rule_priorities method definition

await def set_rule_priorities(
    self,
    *,
    RulePriorities: Sequence[RulePriorityPairTypeDef],  # (1)
) -> SetRulePrioritiesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RulePriorityPairTypeDef](./type_defs.md#ruleprioritypairtypedef) 
2. See [:material-code-braces: SetRulePrioritiesOutputTypeDef](./type_defs.md#setruleprioritiesoutputtypedef) 


```python
# set_rule_priorities method usage example with argument unpacking

kwargs: SetRulePrioritiesInputRequestTypeDef = {  # (1)
    "RulePriorities": ...,
}

parent.set_rule_priorities(**kwargs)
```

1. See [:material-code-braces: SetRulePrioritiesInputRequestTypeDef](./type_defs.md#setruleprioritiesinputrequesttypedef) 

### set\_security\_groups

Associates the specified security groups with the specified Application Load
Balancer or Network Load Balancer.

Type annotations and code completion for `#!python session.create_client("elbv2").set_security_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/set_security_groups.html)

```python
# set_security_groups method definition

await def set_security_groups(
    self,
    *,
    LoadBalancerArn: str,
    SecurityGroups: Sequence[str],
    EnforceSecurityGroupInboundRulesOnPrivateLinkTraffic: EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType = ...,  # (1)
) -> SetSecurityGroupsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType](./literals.md#enforcesecuritygroupinboundrulesonprivatelinktrafficenumtype) 
2. See [:material-code-braces: SetSecurityGroupsOutputTypeDef](./type_defs.md#setsecuritygroupsoutputtypedef) 


```python
# set_security_groups method usage example with argument unpacking

kwargs: SetSecurityGroupsInputRequestTypeDef = {  # (1)
    "LoadBalancerArn": ...,
    "SecurityGroups": ...,
}

parent.set_security_groups(**kwargs)
```

1. See [:material-code-braces: SetSecurityGroupsInputRequestTypeDef](./type_defs.md#setsecuritygroupsinputrequesttypedef) 

### set\_subnets

Enables the Availability Zones for the specified public subnets for the
specified Application Load Balancer, Network Load Balancer or Gateway Load
Balancer.

Type annotations and code completion for `#!python session.create_client("elbv2").set_subnets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/set_subnets.html)

```python
# set_subnets method definition

await def set_subnets(
    self,
    *,
    LoadBalancerArn: str,
    Subnets: Sequence[str] = ...,
    SubnetMappings: Sequence[SubnetMappingTypeDef] = ...,  # (1)
    IpAddressType: IpAddressTypeType = ...,  # (2)
    EnablePrefixForIpv6SourceNat: EnablePrefixForIpv6SourceNatEnumType = ...,  # (3)
) -> SetSubnetsOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: SubnetMappingTypeDef](./type_defs.md#subnetmappingtypedef) 
2. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
3. See [:material-code-brackets: EnablePrefixForIpv6SourceNatEnumType](./literals.md#enableprefixforipv6sourcenatenumtype) 
4. See [:material-code-braces: SetSubnetsOutputTypeDef](./type_defs.md#setsubnetsoutputtypedef) 


```python
# set_subnets method usage example with argument unpacking

kwargs: SetSubnetsInputRequestTypeDef = {  # (1)
    "LoadBalancerArn": ...,
}

parent.set_subnets(**kwargs)
```

1. See [:material-code-braces: SetSubnetsInputRequestTypeDef](./type_defs.md#setsubnetsinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("elbv2").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "ElasticLoadBalancingv2Client":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("elbv2").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client)

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

Type annotations and code completion for `#!python session.create_client("elbv2").get_paginator` method with overloads.

- `client.get_paginator("describe_account_limits")` -> [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
- `client.get_paginator("describe_listener_certificates")` -> [DescribeListenerCertificatesPaginator](./paginators.md#describelistenercertificatespaginator)
- `client.get_paginator("describe_listeners")` -> [DescribeListenersPaginator](./paginators.md#describelistenerspaginator)
- `client.get_paginator("describe_load_balancers")` -> [DescribeLoadBalancersPaginator](./paginators.md#describeloadbalancerspaginator)
- `client.get_paginator("describe_rules")` -> [DescribeRulesPaginator](./paginators.md#describerulespaginator)
- `client.get_paginator("describe_ssl_policies")` -> [DescribeSSLPoliciesPaginator](./paginators.md#describesslpoliciespaginator)
- `client.get_paginator("describe_target_groups")` -> [DescribeTargetGroupsPaginator](./paginators.md#describetargetgroupspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("elbv2").get_waiter` method with overloads.

- `client.get_waiter("load_balancer_available")` -> [LoadBalancerAvailableWaiter](./waiters.md#loadbalanceravailablewaiter)
- `client.get_waiter("load_balancer_exists")` -> [LoadBalancerExistsWaiter](./waiters.md#loadbalancerexistswaiter)
- `client.get_waiter("load_balancers_deleted")` -> [LoadBalancersDeletedWaiter](./waiters.md#loadbalancersdeletedwaiter)
- `client.get_waiter("target_deregistered")` -> [TargetDeregisteredWaiter](./waiters.md#targetderegisteredwaiter)
- `client.get_waiter("target_in_service")` -> [TargetInServiceWaiter](./waiters.md#targetinservicewaiter)

