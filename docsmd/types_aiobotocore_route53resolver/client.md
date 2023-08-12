# Route53ResolverClient

> [Index](../README.md) > [Route53Resolver](./README.md) > Route53ResolverClient

!!! note ""

    Auto-generated documentation for [Route53Resolver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
    type annotations stubs module [types-aiobotocore-route53resolver](https://pypi.org/project/types-aiobotocore-route53resolver/).

## Route53ResolverClient

Type annotations and code completion for `#!python session.create_client("route53resolver")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client)

```python
Route53ResolverClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_route53resolver.client import Route53ResolverClient

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("route53resolver").exceptions` structure.

```python
Route53ResolverClient.exceptions usage example

async with session.create_client("route53resolver") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServiceErrorException,
        client.InvalidNextTokenException,
        client.InvalidParameterException,
        client.InvalidPolicyDocument,
        client.InvalidRequestException,
        client.InvalidTagException,
        client.LimitExceededException,
        client.ResourceExistsException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.ResourceUnavailableException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.UnknownResourceException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
Route53ResolverClient usage type checking example

from types_aiobotocore_route53resolver.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_firewall\_rule\_group

Associates a  FirewallRuleGroup with a VPC, to provide DNS filtering for the
VPC.

Type annotations and code completion for `#!python session.create_client("route53resolver").associate_firewall_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.associate_firewall_rule_group)

```python
# associate_firewall_rule_group method definition

await def associate_firewall_rule_group(
    self,
    *,
    CreatorRequestId: str,
    FirewallRuleGroupId: str,
    VpcId: str,
    Priority: int,
    Name: str,
    MutationProtection: MutationProtectionStatusType = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> AssociateFirewallRuleGroupResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MutationProtectionStatusType](./literals.md#mutationprotectionstatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: AssociateFirewallRuleGroupResponseTypeDef](./type_defs.md#associatefirewallrulegroupresponsetypedef) 


```python
# associate_firewall_rule_group method usage example with argument unpacking

kwargs: AssociateFirewallRuleGroupRequestRequestTypeDef = {  # (1)
    "CreatorRequestId": ...,
    "FirewallRuleGroupId": ...,
    "VpcId": ...,
    "Priority": ...,
    "Name": ...,
}

parent.associate_firewall_rule_group(**kwargs)
```

1. See [:material-code-braces: AssociateFirewallRuleGroupRequestRequestTypeDef](./type_defs.md#associatefirewallrulegrouprequestrequesttypedef) 

### associate\_resolver\_endpoint\_ip\_address

Adds IP addresses to an inbound or an outbound Resolver endpoint.

Type annotations and code completion for `#!python session.create_client("route53resolver").associate_resolver_endpoint_ip_address` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.associate_resolver_endpoint_ip_address)

```python
# associate_resolver_endpoint_ip_address method definition

await def associate_resolver_endpoint_ip_address(
    self,
    *,
    ResolverEndpointId: str,
    IpAddress: IpAddressUpdateTypeDef,  # (1)
) -> AssociateResolverEndpointIpAddressResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IpAddressUpdateTypeDef](./type_defs.md#ipaddressupdatetypedef) 
2. See [:material-code-braces: AssociateResolverEndpointIpAddressResponseTypeDef](./type_defs.md#associateresolverendpointipaddressresponsetypedef) 


```python
# associate_resolver_endpoint_ip_address method usage example with argument unpacking

kwargs: AssociateResolverEndpointIpAddressRequestRequestTypeDef = {  # (1)
    "ResolverEndpointId": ...,
    "IpAddress": ...,
}

parent.associate_resolver_endpoint_ip_address(**kwargs)
```

1. See [:material-code-braces: AssociateResolverEndpointIpAddressRequestRequestTypeDef](./type_defs.md#associateresolverendpointipaddressrequestrequesttypedef) 

### associate\_resolver\_query\_log\_config

Associates an Amazon VPC with a specified query logging configuration.

Type annotations and code completion for `#!python session.create_client("route53resolver").associate_resolver_query_log_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.associate_resolver_query_log_config)

```python
# associate_resolver_query_log_config method definition

await def associate_resolver_query_log_config(
    self,
    *,
    ResolverQueryLogConfigId: str,
    ResourceId: str,
) -> AssociateResolverQueryLogConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateResolverQueryLogConfigResponseTypeDef](./type_defs.md#associateresolverquerylogconfigresponsetypedef) 


```python
# associate_resolver_query_log_config method usage example with argument unpacking

kwargs: AssociateResolverQueryLogConfigRequestRequestTypeDef = {  # (1)
    "ResolverQueryLogConfigId": ...,
    "ResourceId": ...,
}

parent.associate_resolver_query_log_config(**kwargs)
```

1. See [:material-code-braces: AssociateResolverQueryLogConfigRequestRequestTypeDef](./type_defs.md#associateresolverquerylogconfigrequestrequesttypedef) 

### associate\_resolver\_rule

Associates a Resolver rule with a VPC.

Type annotations and code completion for `#!python session.create_client("route53resolver").associate_resolver_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.associate_resolver_rule)

```python
# associate_resolver_rule method definition

await def associate_resolver_rule(
    self,
    *,
    ResolverRuleId: str,
    VPCId: str,
    Name: str = ...,
) -> AssociateResolverRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateResolverRuleResponseTypeDef](./type_defs.md#associateresolverruleresponsetypedef) 


```python
# associate_resolver_rule method usage example with argument unpacking

kwargs: AssociateResolverRuleRequestRequestTypeDef = {  # (1)
    "ResolverRuleId": ...,
    "VPCId": ...,
}

parent.associate_resolver_rule(**kwargs)
```

1. See [:material-code-braces: AssociateResolverRuleRequestRequestTypeDef](./type_defs.md#associateresolverrulerequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("route53resolver").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("route53resolver").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_firewall\_domain\_list

Creates an empty firewall domain list for use in DNS Firewall rules.

Type annotations and code completion for `#!python session.create_client("route53resolver").create_firewall_domain_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_firewall_domain_list)

```python
# create_firewall_domain_list method definition

await def create_firewall_domain_list(
    self,
    *,
    CreatorRequestId: str,
    Name: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateFirewallDomainListResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateFirewallDomainListResponseTypeDef](./type_defs.md#createfirewalldomainlistresponsetypedef) 


```python
# create_firewall_domain_list method usage example with argument unpacking

kwargs: CreateFirewallDomainListRequestRequestTypeDef = {  # (1)
    "CreatorRequestId": ...,
    "Name": ...,
}

parent.create_firewall_domain_list(**kwargs)
```

1. See [:material-code-braces: CreateFirewallDomainListRequestRequestTypeDef](./type_defs.md#createfirewalldomainlistrequestrequesttypedef) 

### create\_firewall\_rule

Creates a single DNS Firewall rule in the specified rule group, using the
specified domain list.

Type annotations and code completion for `#!python session.create_client("route53resolver").create_firewall_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_firewall_rule)

```python
# create_firewall_rule method definition

await def create_firewall_rule(
    self,
    *,
    CreatorRequestId: str,
    FirewallRuleGroupId: str,
    FirewallDomainListId: str,
    Priority: int,
    Action: ActionType,  # (1)
    Name: str,
    BlockResponse: BlockResponseType = ...,  # (2)
    BlockOverrideDomain: str = ...,
    BlockOverrideDnsType: BlockOverrideDnsTypeType = ...,  # (3)
    BlockOverrideTtl: int = ...,
) -> CreateFirewallRuleResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
2. See [:material-code-brackets: BlockResponseType](./literals.md#blockresponsetype) 
3. See [:material-code-brackets: BlockOverrideDnsTypeType](./literals.md#blockoverridednstypetype) 
4. See [:material-code-braces: CreateFirewallRuleResponseTypeDef](./type_defs.md#createfirewallruleresponsetypedef) 


```python
# create_firewall_rule method usage example with argument unpacking

kwargs: CreateFirewallRuleRequestRequestTypeDef = {  # (1)
    "CreatorRequestId": ...,
    "FirewallRuleGroupId": ...,
    "FirewallDomainListId": ...,
    "Priority": ...,
    "Action": ...,
    "Name": ...,
}

parent.create_firewall_rule(**kwargs)
```

1. See [:material-code-braces: CreateFirewallRuleRequestRequestTypeDef](./type_defs.md#createfirewallrulerequestrequesttypedef) 

### create\_firewall\_rule\_group

Creates an empty DNS Firewall rule group for filtering DNS network traffic in a
VPC.

Type annotations and code completion for `#!python session.create_client("route53resolver").create_firewall_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_firewall_rule_group)

```python
# create_firewall_rule_group method definition

await def create_firewall_rule_group(
    self,
    *,
    CreatorRequestId: str,
    Name: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateFirewallRuleGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateFirewallRuleGroupResponseTypeDef](./type_defs.md#createfirewallrulegroupresponsetypedef) 


```python
# create_firewall_rule_group method usage example with argument unpacking

kwargs: CreateFirewallRuleGroupRequestRequestTypeDef = {  # (1)
    "CreatorRequestId": ...,
    "Name": ...,
}

parent.create_firewall_rule_group(**kwargs)
```

1. See [:material-code-braces: CreateFirewallRuleGroupRequestRequestTypeDef](./type_defs.md#createfirewallrulegrouprequestrequesttypedef) 

### create\_outpost\_resolver

Creates an Route 53 Resolver on an Outpost.

Type annotations and code completion for `#!python session.create_client("route53resolver").create_outpost_resolver` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_outpost_resolver)

```python
# create_outpost_resolver method definition

await def create_outpost_resolver(
    self,
    *,
    CreatorRequestId: str,
    Name: str,
    PreferredInstanceType: str,
    OutpostArn: str,
    InstanceCount: int = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateOutpostResolverResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateOutpostResolverResponseTypeDef](./type_defs.md#createoutpostresolverresponsetypedef) 


```python
# create_outpost_resolver method usage example with argument unpacking

kwargs: CreateOutpostResolverRequestRequestTypeDef = {  # (1)
    "CreatorRequestId": ...,
    "Name": ...,
    "PreferredInstanceType": ...,
    "OutpostArn": ...,
}

parent.create_outpost_resolver(**kwargs)
```

1. See [:material-code-braces: CreateOutpostResolverRequestRequestTypeDef](./type_defs.md#createoutpostresolverrequestrequesttypedef) 

### create\_resolver\_endpoint

Creates a Resolver endpoint.

Type annotations and code completion for `#!python session.create_client("route53resolver").create_resolver_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_endpoint)

```python
# create_resolver_endpoint method definition

await def create_resolver_endpoint(
    self,
    *,
    CreatorRequestId: str,
    SecurityGroupIds: Sequence[str],
    Direction: ResolverEndpointDirectionType,  # (1)
    IpAddresses: Sequence[IpAddressRequestTypeDef],  # (2)
    Name: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    ResolverEndpointType: ResolverEndpointTypeType = ...,  # (4)
    OutpostArn: str = ...,
    PreferredInstanceType: str = ...,
) -> CreateResolverEndpointResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ResolverEndpointDirectionType](./literals.md#resolverendpointdirectiontype) 
2. See [:material-code-braces: IpAddressRequestTypeDef](./type_defs.md#ipaddressrequesttypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: ResolverEndpointTypeType](./literals.md#resolverendpointtypetype) 
5. See [:material-code-braces: CreateResolverEndpointResponseTypeDef](./type_defs.md#createresolverendpointresponsetypedef) 


```python
# create_resolver_endpoint method usage example with argument unpacking

kwargs: CreateResolverEndpointRequestRequestTypeDef = {  # (1)
    "CreatorRequestId": ...,
    "SecurityGroupIds": ...,
    "Direction": ...,
    "IpAddresses": ...,
}

parent.create_resolver_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateResolverEndpointRequestRequestTypeDef](./type_defs.md#createresolverendpointrequestrequesttypedef) 

### create\_resolver\_query\_log\_config

Creates a Resolver query logging configuration, which defines where you want
Resolver to save DNS query logs that originate in your VPCs.

Type annotations and code completion for `#!python session.create_client("route53resolver").create_resolver_query_log_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_query_log_config)

```python
# create_resolver_query_log_config method definition

await def create_resolver_query_log_config(
    self,
    *,
    Name: str,
    DestinationArn: str,
    CreatorRequestId: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateResolverQueryLogConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateResolverQueryLogConfigResponseTypeDef](./type_defs.md#createresolverquerylogconfigresponsetypedef) 


```python
# create_resolver_query_log_config method usage example with argument unpacking

kwargs: CreateResolverQueryLogConfigRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "DestinationArn": ...,
    "CreatorRequestId": ...,
}

parent.create_resolver_query_log_config(**kwargs)
```

1. See [:material-code-braces: CreateResolverQueryLogConfigRequestRequestTypeDef](./type_defs.md#createresolverquerylogconfigrequestrequesttypedef) 

### create\_resolver\_rule

For DNS queries that originate in your VPCs, specifies which Resolver endpoint
the queries pass through, one domain name that you want to forward to your
network, and the IP addresses of the DNS resolvers in your network.

Type annotations and code completion for `#!python session.create_client("route53resolver").create_resolver_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_rule)

```python
# create_resolver_rule method definition

await def create_resolver_rule(
    self,
    *,
    CreatorRequestId: str,
    RuleType: RuleTypeOptionType,  # (1)
    DomainName: str,
    Name: str = ...,
    TargetIps: Sequence[TargetAddressTypeDef] = ...,  # (2)
    ResolverEndpointId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateResolverRuleResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: RuleTypeOptionType](./literals.md#ruletypeoptiontype) 
2. See [:material-code-braces: TargetAddressTypeDef](./type_defs.md#targetaddresstypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateResolverRuleResponseTypeDef](./type_defs.md#createresolverruleresponsetypedef) 


```python
# create_resolver_rule method usage example with argument unpacking

kwargs: CreateResolverRuleRequestRequestTypeDef = {  # (1)
    "CreatorRequestId": ...,
    "RuleType": ...,
    "DomainName": ...,
}

parent.create_resolver_rule(**kwargs)
```

1. See [:material-code-braces: CreateResolverRuleRequestRequestTypeDef](./type_defs.md#createresolverrulerequestrequesttypedef) 

### delete\_firewall\_domain\_list

Deletes the specified domain list.

Type annotations and code completion for `#!python session.create_client("route53resolver").delete_firewall_domain_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_firewall_domain_list)

```python
# delete_firewall_domain_list method definition

await def delete_firewall_domain_list(
    self,
    *,
    FirewallDomainListId: str,
) -> DeleteFirewallDomainListResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFirewallDomainListResponseTypeDef](./type_defs.md#deletefirewalldomainlistresponsetypedef) 


```python
# delete_firewall_domain_list method usage example with argument unpacking

kwargs: DeleteFirewallDomainListRequestRequestTypeDef = {  # (1)
    "FirewallDomainListId": ...,
}

parent.delete_firewall_domain_list(**kwargs)
```

1. See [:material-code-braces: DeleteFirewallDomainListRequestRequestTypeDef](./type_defs.md#deletefirewalldomainlistrequestrequesttypedef) 

### delete\_firewall\_rule

Deletes the specified firewall rule.

Type annotations and code completion for `#!python session.create_client("route53resolver").delete_firewall_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_firewall_rule)

```python
# delete_firewall_rule method definition

await def delete_firewall_rule(
    self,
    *,
    FirewallRuleGroupId: str,
    FirewallDomainListId: str,
) -> DeleteFirewallRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFirewallRuleResponseTypeDef](./type_defs.md#deletefirewallruleresponsetypedef) 


```python
# delete_firewall_rule method usage example with argument unpacking

kwargs: DeleteFirewallRuleRequestRequestTypeDef = {  # (1)
    "FirewallRuleGroupId": ...,
    "FirewallDomainListId": ...,
}

parent.delete_firewall_rule(**kwargs)
```

1. See [:material-code-braces: DeleteFirewallRuleRequestRequestTypeDef](./type_defs.md#deletefirewallrulerequestrequesttypedef) 

### delete\_firewall\_rule\_group

Deletes the specified firewall rule group.

Type annotations and code completion for `#!python session.create_client("route53resolver").delete_firewall_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_firewall_rule_group)

```python
# delete_firewall_rule_group method definition

await def delete_firewall_rule_group(
    self,
    *,
    FirewallRuleGroupId: str,
) -> DeleteFirewallRuleGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFirewallRuleGroupResponseTypeDef](./type_defs.md#deletefirewallrulegroupresponsetypedef) 


```python
# delete_firewall_rule_group method usage example with argument unpacking

kwargs: DeleteFirewallRuleGroupRequestRequestTypeDef = {  # (1)
    "FirewallRuleGroupId": ...,
}

parent.delete_firewall_rule_group(**kwargs)
```

1. See [:material-code-braces: DeleteFirewallRuleGroupRequestRequestTypeDef](./type_defs.md#deletefirewallrulegrouprequestrequesttypedef) 

### delete\_outpost\_resolver

Deletes a Resolver on the Outpost.

Type annotations and code completion for `#!python session.create_client("route53resolver").delete_outpost_resolver` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_outpost_resolver)

```python
# delete_outpost_resolver method definition

await def delete_outpost_resolver(
    self,
    *,
    Id: str,
) -> DeleteOutpostResolverResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteOutpostResolverResponseTypeDef](./type_defs.md#deleteoutpostresolverresponsetypedef) 


```python
# delete_outpost_resolver method usage example with argument unpacking

kwargs: DeleteOutpostResolverRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_outpost_resolver(**kwargs)
```

1. See [:material-code-braces: DeleteOutpostResolverRequestRequestTypeDef](./type_defs.md#deleteoutpostresolverrequestrequesttypedef) 

### delete\_resolver\_endpoint

Deletes a Resolver endpoint.

Type annotations and code completion for `#!python session.create_client("route53resolver").delete_resolver_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_resolver_endpoint)

```python
# delete_resolver_endpoint method definition

await def delete_resolver_endpoint(
    self,
    *,
    ResolverEndpointId: str,
) -> DeleteResolverEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteResolverEndpointResponseTypeDef](./type_defs.md#deleteresolverendpointresponsetypedef) 


```python
# delete_resolver_endpoint method usage example with argument unpacking

kwargs: DeleteResolverEndpointRequestRequestTypeDef = {  # (1)
    "ResolverEndpointId": ...,
}

parent.delete_resolver_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteResolverEndpointRequestRequestTypeDef](./type_defs.md#deleteresolverendpointrequestrequesttypedef) 

### delete\_resolver\_query\_log\_config

Deletes a query logging configuration.

Type annotations and code completion for `#!python session.create_client("route53resolver").delete_resolver_query_log_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_resolver_query_log_config)

```python
# delete_resolver_query_log_config method definition

await def delete_resolver_query_log_config(
    self,
    *,
    ResolverQueryLogConfigId: str,
) -> DeleteResolverQueryLogConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteResolverQueryLogConfigResponseTypeDef](./type_defs.md#deleteresolverquerylogconfigresponsetypedef) 


```python
# delete_resolver_query_log_config method usage example with argument unpacking

kwargs: DeleteResolverQueryLogConfigRequestRequestTypeDef = {  # (1)
    "ResolverQueryLogConfigId": ...,
}

parent.delete_resolver_query_log_config(**kwargs)
```

1. See [:material-code-braces: DeleteResolverQueryLogConfigRequestRequestTypeDef](./type_defs.md#deleteresolverquerylogconfigrequestrequesttypedef) 

### delete\_resolver\_rule

Deletes a Resolver rule.

Type annotations and code completion for `#!python session.create_client("route53resolver").delete_resolver_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_resolver_rule)

```python
# delete_resolver_rule method definition

await def delete_resolver_rule(
    self,
    *,
    ResolverRuleId: str,
) -> DeleteResolverRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteResolverRuleResponseTypeDef](./type_defs.md#deleteresolverruleresponsetypedef) 


```python
# delete_resolver_rule method usage example with argument unpacking

kwargs: DeleteResolverRuleRequestRequestTypeDef = {  # (1)
    "ResolverRuleId": ...,
}

parent.delete_resolver_rule(**kwargs)
```

1. See [:material-code-braces: DeleteResolverRuleRequestRequestTypeDef](./type_defs.md#deleteresolverrulerequestrequesttypedef) 

### disassociate\_firewall\_rule\_group

Disassociates a  FirewallRuleGroup from a VPC, to remove DNS filtering from the
VPC.

Type annotations and code completion for `#!python session.create_client("route53resolver").disassociate_firewall_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.disassociate_firewall_rule_group)

```python
# disassociate_firewall_rule_group method definition

await def disassociate_firewall_rule_group(
    self,
    *,
    FirewallRuleGroupAssociationId: str,
) -> DisassociateFirewallRuleGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateFirewallRuleGroupResponseTypeDef](./type_defs.md#disassociatefirewallrulegroupresponsetypedef) 


```python
# disassociate_firewall_rule_group method usage example with argument unpacking

kwargs: DisassociateFirewallRuleGroupRequestRequestTypeDef = {  # (1)
    "FirewallRuleGroupAssociationId": ...,
}

parent.disassociate_firewall_rule_group(**kwargs)
```

1. See [:material-code-braces: DisassociateFirewallRuleGroupRequestRequestTypeDef](./type_defs.md#disassociatefirewallrulegrouprequestrequesttypedef) 

### disassociate\_resolver\_endpoint\_ip\_address

Removes IP addresses from an inbound or an outbound Resolver endpoint.

Type annotations and code completion for `#!python session.create_client("route53resolver").disassociate_resolver_endpoint_ip_address` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.disassociate_resolver_endpoint_ip_address)

```python
# disassociate_resolver_endpoint_ip_address method definition

await def disassociate_resolver_endpoint_ip_address(
    self,
    *,
    ResolverEndpointId: str,
    IpAddress: IpAddressUpdateTypeDef,  # (1)
) -> DisassociateResolverEndpointIpAddressResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IpAddressUpdateTypeDef](./type_defs.md#ipaddressupdatetypedef) 
2. See [:material-code-braces: DisassociateResolverEndpointIpAddressResponseTypeDef](./type_defs.md#disassociateresolverendpointipaddressresponsetypedef) 


```python
# disassociate_resolver_endpoint_ip_address method usage example with argument unpacking

kwargs: DisassociateResolverEndpointIpAddressRequestRequestTypeDef = {  # (1)
    "ResolverEndpointId": ...,
    "IpAddress": ...,
}

parent.disassociate_resolver_endpoint_ip_address(**kwargs)
```

1. See [:material-code-braces: DisassociateResolverEndpointIpAddressRequestRequestTypeDef](./type_defs.md#disassociateresolverendpointipaddressrequestrequesttypedef) 

### disassociate\_resolver\_query\_log\_config

Disassociates a VPC from a query logging configuration.

Type annotations and code completion for `#!python session.create_client("route53resolver").disassociate_resolver_query_log_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.disassociate_resolver_query_log_config)

```python
# disassociate_resolver_query_log_config method definition

await def disassociate_resolver_query_log_config(
    self,
    *,
    ResolverQueryLogConfigId: str,
    ResourceId: str,
) -> DisassociateResolverQueryLogConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateResolverQueryLogConfigResponseTypeDef](./type_defs.md#disassociateresolverquerylogconfigresponsetypedef) 


```python
# disassociate_resolver_query_log_config method usage example with argument unpacking

kwargs: DisassociateResolverQueryLogConfigRequestRequestTypeDef = {  # (1)
    "ResolverQueryLogConfigId": ...,
    "ResourceId": ...,
}

parent.disassociate_resolver_query_log_config(**kwargs)
```

1. See [:material-code-braces: DisassociateResolverQueryLogConfigRequestRequestTypeDef](./type_defs.md#disassociateresolverquerylogconfigrequestrequesttypedef) 

### disassociate\_resolver\_rule

Removes the association between a specified Resolver rule and a specified VPC.

Type annotations and code completion for `#!python session.create_client("route53resolver").disassociate_resolver_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.disassociate_resolver_rule)

```python
# disassociate_resolver_rule method definition

await def disassociate_resolver_rule(
    self,
    *,
    VPCId: str,
    ResolverRuleId: str,
) -> DisassociateResolverRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateResolverRuleResponseTypeDef](./type_defs.md#disassociateresolverruleresponsetypedef) 


```python
# disassociate_resolver_rule method usage example with argument unpacking

kwargs: DisassociateResolverRuleRequestRequestTypeDef = {  # (1)
    "VPCId": ...,
    "ResolverRuleId": ...,
}

parent.disassociate_resolver_rule(**kwargs)
```

1. See [:material-code-braces: DisassociateResolverRuleRequestRequestTypeDef](./type_defs.md#disassociateresolverrulerequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("route53resolver").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.generate_presigned_url)

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


### get\_firewall\_config

Retrieves the configuration of the firewall behavior provided by DNS Firewall
for a single VPC from Amazon Virtual Private Cloud (Amazon VPC).

Type annotations and code completion for `#!python session.create_client("route53resolver").get_firewall_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_firewall_config)

```python
# get_firewall_config method definition

await def get_firewall_config(
    self,
    *,
    ResourceId: str,
) -> GetFirewallConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFirewallConfigResponseTypeDef](./type_defs.md#getfirewallconfigresponsetypedef) 


```python
# get_firewall_config method usage example with argument unpacking

kwargs: GetFirewallConfigRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.get_firewall_config(**kwargs)
```

1. See [:material-code-braces: GetFirewallConfigRequestRequestTypeDef](./type_defs.md#getfirewallconfigrequestrequesttypedef) 

### get\_firewall\_domain\_list

Retrieves the specified firewall domain list.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_firewall_domain_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_firewall_domain_list)

```python
# get_firewall_domain_list method definition

await def get_firewall_domain_list(
    self,
    *,
    FirewallDomainListId: str,
) -> GetFirewallDomainListResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFirewallDomainListResponseTypeDef](./type_defs.md#getfirewalldomainlistresponsetypedef) 


```python
# get_firewall_domain_list method usage example with argument unpacking

kwargs: GetFirewallDomainListRequestRequestTypeDef = {  # (1)
    "FirewallDomainListId": ...,
}

parent.get_firewall_domain_list(**kwargs)
```

1. See [:material-code-braces: GetFirewallDomainListRequestRequestTypeDef](./type_defs.md#getfirewalldomainlistrequestrequesttypedef) 

### get\_firewall\_rule\_group

Retrieves the specified firewall rule group.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_firewall_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_firewall_rule_group)

```python
# get_firewall_rule_group method definition

await def get_firewall_rule_group(
    self,
    *,
    FirewallRuleGroupId: str,
) -> GetFirewallRuleGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFirewallRuleGroupResponseTypeDef](./type_defs.md#getfirewallrulegroupresponsetypedef) 


```python
# get_firewall_rule_group method usage example with argument unpacking

kwargs: GetFirewallRuleGroupRequestRequestTypeDef = {  # (1)
    "FirewallRuleGroupId": ...,
}

parent.get_firewall_rule_group(**kwargs)
```

1. See [:material-code-braces: GetFirewallRuleGroupRequestRequestTypeDef](./type_defs.md#getfirewallrulegrouprequestrequesttypedef) 

### get\_firewall\_rule\_group\_association

Retrieves a firewall rule group association, which enables DNS filtering for a
VPC with one rule group.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_firewall_rule_group_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_firewall_rule_group_association)

```python
# get_firewall_rule_group_association method definition

await def get_firewall_rule_group_association(
    self,
    *,
    FirewallRuleGroupAssociationId: str,
) -> GetFirewallRuleGroupAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFirewallRuleGroupAssociationResponseTypeDef](./type_defs.md#getfirewallrulegroupassociationresponsetypedef) 


```python
# get_firewall_rule_group_association method usage example with argument unpacking

kwargs: GetFirewallRuleGroupAssociationRequestRequestTypeDef = {  # (1)
    "FirewallRuleGroupAssociationId": ...,
}

parent.get_firewall_rule_group_association(**kwargs)
```

1. See [:material-code-braces: GetFirewallRuleGroupAssociationRequestRequestTypeDef](./type_defs.md#getfirewallrulegroupassociationrequestrequesttypedef) 

### get\_firewall\_rule\_group\_policy

Returns the Identity and Access Management (Amazon Web Services IAM) policy for
sharing the specified rule group.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_firewall_rule_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_firewall_rule_group_policy)

```python
# get_firewall_rule_group_policy method definition

await def get_firewall_rule_group_policy(
    self,
    *,
    Arn: str,
) -> GetFirewallRuleGroupPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFirewallRuleGroupPolicyResponseTypeDef](./type_defs.md#getfirewallrulegrouppolicyresponsetypedef) 


```python
# get_firewall_rule_group_policy method usage example with argument unpacking

kwargs: GetFirewallRuleGroupPolicyRequestRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.get_firewall_rule_group_policy(**kwargs)
```

1. See [:material-code-braces: GetFirewallRuleGroupPolicyRequestRequestTypeDef](./type_defs.md#getfirewallrulegrouppolicyrequestrequesttypedef) 

### get\_outpost\_resolver

Gets information about a specified Resolver on the Outpost, such as its instance
count and type, name, and the current status of the Resolver.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_outpost_resolver` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_outpost_resolver)

```python
# get_outpost_resolver method definition

await def get_outpost_resolver(
    self,
    *,
    Id: str,
) -> GetOutpostResolverResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOutpostResolverResponseTypeDef](./type_defs.md#getoutpostresolverresponsetypedef) 


```python
# get_outpost_resolver method usage example with argument unpacking

kwargs: GetOutpostResolverRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_outpost_resolver(**kwargs)
```

1. See [:material-code-braces: GetOutpostResolverRequestRequestTypeDef](./type_defs.md#getoutpostresolverrequestrequesttypedef) 

### get\_resolver\_config

Retrieves the behavior configuration of Route 53 Resolver behavior for a single
VPC from Amazon Virtual Private Cloud.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_resolver_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_resolver_config)

```python
# get_resolver_config method definition

await def get_resolver_config(
    self,
    *,
    ResourceId: str,
) -> GetResolverConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResolverConfigResponseTypeDef](./type_defs.md#getresolverconfigresponsetypedef) 


```python
# get_resolver_config method usage example with argument unpacking

kwargs: GetResolverConfigRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.get_resolver_config(**kwargs)
```

1. See [:material-code-braces: GetResolverConfigRequestRequestTypeDef](./type_defs.md#getresolverconfigrequestrequesttypedef) 

### get\_resolver\_dnssec\_config

Gets DNSSEC validation information for a specified resource.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_resolver_dnssec_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_resolver_dnssec_config)

```python
# get_resolver_dnssec_config method definition

await def get_resolver_dnssec_config(
    self,
    *,
    ResourceId: str,
) -> GetResolverDnssecConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResolverDnssecConfigResponseTypeDef](./type_defs.md#getresolverdnssecconfigresponsetypedef) 


```python
# get_resolver_dnssec_config method usage example with argument unpacking

kwargs: GetResolverDnssecConfigRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.get_resolver_dnssec_config(**kwargs)
```

1. See [:material-code-braces: GetResolverDnssecConfigRequestRequestTypeDef](./type_defs.md#getresolverdnssecconfigrequestrequesttypedef) 

### get\_resolver\_endpoint

Gets information about a specified Resolver endpoint, such as whether it's an
inbound or an outbound Resolver endpoint, and the current status of the
endpoint.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_resolver_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_resolver_endpoint)

```python
# get_resolver_endpoint method definition

await def get_resolver_endpoint(
    self,
    *,
    ResolverEndpointId: str,
) -> GetResolverEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResolverEndpointResponseTypeDef](./type_defs.md#getresolverendpointresponsetypedef) 


```python
# get_resolver_endpoint method usage example with argument unpacking

kwargs: GetResolverEndpointRequestRequestTypeDef = {  # (1)
    "ResolverEndpointId": ...,
}

parent.get_resolver_endpoint(**kwargs)
```

1. See [:material-code-braces: GetResolverEndpointRequestRequestTypeDef](./type_defs.md#getresolverendpointrequestrequesttypedef) 

### get\_resolver\_query\_log\_config

Gets information about a specified Resolver query logging configuration, such as
the number of VPCs that the configuration is logging queries for and the
location that logs are sent to.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_resolver_query_log_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_resolver_query_log_config)

```python
# get_resolver_query_log_config method definition

await def get_resolver_query_log_config(
    self,
    *,
    ResolverQueryLogConfigId: str,
) -> GetResolverQueryLogConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResolverQueryLogConfigResponseTypeDef](./type_defs.md#getresolverquerylogconfigresponsetypedef) 


```python
# get_resolver_query_log_config method usage example with argument unpacking

kwargs: GetResolverQueryLogConfigRequestRequestTypeDef = {  # (1)
    "ResolverQueryLogConfigId": ...,
}

parent.get_resolver_query_log_config(**kwargs)
```

1. See [:material-code-braces: GetResolverQueryLogConfigRequestRequestTypeDef](./type_defs.md#getresolverquerylogconfigrequestrequesttypedef) 

### get\_resolver\_query\_log\_config\_association

Gets information about a specified association between a Resolver query logging
configuration and an Amazon VPC.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_resolver_query_log_config_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_resolver_query_log_config_association)

```python
# get_resolver_query_log_config_association method definition

await def get_resolver_query_log_config_association(
    self,
    *,
    ResolverQueryLogConfigAssociationId: str,
) -> GetResolverQueryLogConfigAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResolverQueryLogConfigAssociationResponseTypeDef](./type_defs.md#getresolverquerylogconfigassociationresponsetypedef) 


```python
# get_resolver_query_log_config_association method usage example with argument unpacking

kwargs: GetResolverQueryLogConfigAssociationRequestRequestTypeDef = {  # (1)
    "ResolverQueryLogConfigAssociationId": ...,
}

parent.get_resolver_query_log_config_association(**kwargs)
```

1. See [:material-code-braces: GetResolverQueryLogConfigAssociationRequestRequestTypeDef](./type_defs.md#getresolverquerylogconfigassociationrequestrequesttypedef) 

### get\_resolver\_query\_log\_config\_policy

Gets information about a query logging policy.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_resolver_query_log_config_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_resolver_query_log_config_policy)

```python
# get_resolver_query_log_config_policy method definition

await def get_resolver_query_log_config_policy(
    self,
    *,
    Arn: str,
) -> GetResolverQueryLogConfigPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResolverQueryLogConfigPolicyResponseTypeDef](./type_defs.md#getresolverquerylogconfigpolicyresponsetypedef) 


```python
# get_resolver_query_log_config_policy method usage example with argument unpacking

kwargs: GetResolverQueryLogConfigPolicyRequestRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.get_resolver_query_log_config_policy(**kwargs)
```

1. See [:material-code-braces: GetResolverQueryLogConfigPolicyRequestRequestTypeDef](./type_defs.md#getresolverquerylogconfigpolicyrequestrequesttypedef) 

### get\_resolver\_rule

Gets information about a specified Resolver rule, such as the domain name that
the rule forwards DNS queries for and the ID of the outbound Resolver endpoint
that the rule is associated with.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_resolver_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_resolver_rule)

```python
# get_resolver_rule method definition

await def get_resolver_rule(
    self,
    *,
    ResolverRuleId: str,
) -> GetResolverRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResolverRuleResponseTypeDef](./type_defs.md#getresolverruleresponsetypedef) 


```python
# get_resolver_rule method usage example with argument unpacking

kwargs: GetResolverRuleRequestRequestTypeDef = {  # (1)
    "ResolverRuleId": ...,
}

parent.get_resolver_rule(**kwargs)
```

1. See [:material-code-braces: GetResolverRuleRequestRequestTypeDef](./type_defs.md#getresolverrulerequestrequesttypedef) 

### get\_resolver\_rule\_association

Gets information about an association between a specified Resolver rule and a
VPC.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_resolver_rule_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_resolver_rule_association)

```python
# get_resolver_rule_association method definition

await def get_resolver_rule_association(
    self,
    *,
    ResolverRuleAssociationId: str,
) -> GetResolverRuleAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResolverRuleAssociationResponseTypeDef](./type_defs.md#getresolverruleassociationresponsetypedef) 


```python
# get_resolver_rule_association method usage example with argument unpacking

kwargs: GetResolverRuleAssociationRequestRequestTypeDef = {  # (1)
    "ResolverRuleAssociationId": ...,
}

parent.get_resolver_rule_association(**kwargs)
```

1. See [:material-code-braces: GetResolverRuleAssociationRequestRequestTypeDef](./type_defs.md#getresolverruleassociationrequestrequesttypedef) 

### get\_resolver\_rule\_policy

Gets information about the Resolver rule policy for a specified rule.

Type annotations and code completion for `#!python session.create_client("route53resolver").get_resolver_rule_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_resolver_rule_policy)

```python
# get_resolver_rule_policy method definition

await def get_resolver_rule_policy(
    self,
    *,
    Arn: str,
) -> GetResolverRulePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResolverRulePolicyResponseTypeDef](./type_defs.md#getresolverrulepolicyresponsetypedef) 


```python
# get_resolver_rule_policy method usage example with argument unpacking

kwargs: GetResolverRulePolicyRequestRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.get_resolver_rule_policy(**kwargs)
```

1. See [:material-code-braces: GetResolverRulePolicyRequestRequestTypeDef](./type_defs.md#getresolverrulepolicyrequestrequesttypedef) 

### import\_firewall\_domains

Imports domain names from a file into a domain list, for use in a DNS firewall
rule group.

Type annotations and code completion for `#!python session.create_client("route53resolver").import_firewall_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.import_firewall_domains)

```python
# import_firewall_domains method definition

await def import_firewall_domains(
    self,
    *,
    FirewallDomainListId: str,
    Operation: FirewallDomainImportOperationType,  # (1)
    DomainFileUrl: str,
) -> ImportFirewallDomainsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FirewallDomainImportOperationType](./literals.md#firewalldomainimportoperationtype) 
2. See [:material-code-braces: ImportFirewallDomainsResponseTypeDef](./type_defs.md#importfirewalldomainsresponsetypedef) 


```python
# import_firewall_domains method usage example with argument unpacking

kwargs: ImportFirewallDomainsRequestRequestTypeDef = {  # (1)
    "FirewallDomainListId": ...,
    "Operation": ...,
    "DomainFileUrl": ...,
}

parent.import_firewall_domains(**kwargs)
```

1. See [:material-code-braces: ImportFirewallDomainsRequestRequestTypeDef](./type_defs.md#importfirewalldomainsrequestrequesttypedef) 

### list\_firewall\_configs

Retrieves the firewall configurations that you have defined.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_firewall_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_configs)

```python
# list_firewall_configs method definition

await def list_firewall_configs(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListFirewallConfigsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFirewallConfigsResponseTypeDef](./type_defs.md#listfirewallconfigsresponsetypedef) 


```python
# list_firewall_configs method usage example with argument unpacking

kwargs: ListFirewallConfigsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_firewall_configs(**kwargs)
```

1. See [:material-code-braces: ListFirewallConfigsRequestRequestTypeDef](./type_defs.md#listfirewallconfigsrequestrequesttypedef) 

### list\_firewall\_domain\_lists

Retrieves the firewall domain lists that you have defined.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_firewall_domain_lists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_domain_lists)

```python
# list_firewall_domain_lists method definition

await def list_firewall_domain_lists(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListFirewallDomainListsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFirewallDomainListsResponseTypeDef](./type_defs.md#listfirewalldomainlistsresponsetypedef) 


```python
# list_firewall_domain_lists method usage example with argument unpacking

kwargs: ListFirewallDomainListsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_firewall_domain_lists(**kwargs)
```

1. See [:material-code-braces: ListFirewallDomainListsRequestRequestTypeDef](./type_defs.md#listfirewalldomainlistsrequestrequesttypedef) 

### list\_firewall\_domains

Retrieves the domains that you have defined for the specified firewall domain
list.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_firewall_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_domains)

```python
# list_firewall_domains method definition

await def list_firewall_domains(
    self,
    *,
    FirewallDomainListId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListFirewallDomainsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFirewallDomainsResponseTypeDef](./type_defs.md#listfirewalldomainsresponsetypedef) 


```python
# list_firewall_domains method usage example with argument unpacking

kwargs: ListFirewallDomainsRequestRequestTypeDef = {  # (1)
    "FirewallDomainListId": ...,
}

parent.list_firewall_domains(**kwargs)
```

1. See [:material-code-braces: ListFirewallDomainsRequestRequestTypeDef](./type_defs.md#listfirewalldomainsrequestrequesttypedef) 

### list\_firewall\_rule\_group\_associations

Retrieves the firewall rule group associations that you have defined.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_firewall_rule_group_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rule_group_associations)

```python
# list_firewall_rule_group_associations method definition

await def list_firewall_rule_group_associations(
    self,
    *,
    FirewallRuleGroupId: str = ...,
    VpcId: str = ...,
    Priority: int = ...,
    Status: FirewallRuleGroupAssociationStatusType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListFirewallRuleGroupAssociationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FirewallRuleGroupAssociationStatusType](./literals.md#firewallrulegroupassociationstatustype) 
2. See [:material-code-braces: ListFirewallRuleGroupAssociationsResponseTypeDef](./type_defs.md#listfirewallrulegroupassociationsresponsetypedef) 


```python
# list_firewall_rule_group_associations method usage example with argument unpacking

kwargs: ListFirewallRuleGroupAssociationsRequestRequestTypeDef = {  # (1)
    "FirewallRuleGroupId": ...,
}

parent.list_firewall_rule_group_associations(**kwargs)
```

1. See [:material-code-braces: ListFirewallRuleGroupAssociationsRequestRequestTypeDef](./type_defs.md#listfirewallrulegroupassociationsrequestrequesttypedef) 

### list\_firewall\_rule\_groups

Retrieves the minimal high-level information for the rule groups that you have
defined.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_firewall_rule_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rule_groups)

```python
# list_firewall_rule_groups method definition

await def list_firewall_rule_groups(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListFirewallRuleGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFirewallRuleGroupsResponseTypeDef](./type_defs.md#listfirewallrulegroupsresponsetypedef) 


```python
# list_firewall_rule_groups method usage example with argument unpacking

kwargs: ListFirewallRuleGroupsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_firewall_rule_groups(**kwargs)
```

1. See [:material-code-braces: ListFirewallRuleGroupsRequestRequestTypeDef](./type_defs.md#listfirewallrulegroupsrequestrequesttypedef) 

### list\_firewall\_rules

Retrieves the firewall rules that you have defined for the specified firewall
rule group.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_firewall_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rules)

```python
# list_firewall_rules method definition

await def list_firewall_rules(
    self,
    *,
    FirewallRuleGroupId: str,
    Priority: int = ...,
    Action: ActionType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListFirewallRulesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
2. See [:material-code-braces: ListFirewallRulesResponseTypeDef](./type_defs.md#listfirewallrulesresponsetypedef) 


```python
# list_firewall_rules method usage example with argument unpacking

kwargs: ListFirewallRulesRequestRequestTypeDef = {  # (1)
    "FirewallRuleGroupId": ...,
}

parent.list_firewall_rules(**kwargs)
```

1. See [:material-code-braces: ListFirewallRulesRequestRequestTypeDef](./type_defs.md#listfirewallrulesrequestrequesttypedef) 

### list\_outpost\_resolvers

Lists all the Resolvers on Outposts that were created using the current Amazon
Web Services account.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_outpost_resolvers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_outpost_resolvers)

```python
# list_outpost_resolvers method definition

await def list_outpost_resolvers(
    self,
    *,
    OutpostArn: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListOutpostResolversResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOutpostResolversResponseTypeDef](./type_defs.md#listoutpostresolversresponsetypedef) 


```python
# list_outpost_resolvers method usage example with argument unpacking

kwargs: ListOutpostResolversRequestRequestTypeDef = {  # (1)
    "OutpostArn": ...,
}

parent.list_outpost_resolvers(**kwargs)
```

1. See [:material-code-braces: ListOutpostResolversRequestRequestTypeDef](./type_defs.md#listoutpostresolversrequestrequesttypedef) 

### list\_resolver\_configs

Retrieves the Resolver configurations that you have defined.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_resolver_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_configs)

```python
# list_resolver_configs method definition

await def list_resolver_configs(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListResolverConfigsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResolverConfigsResponseTypeDef](./type_defs.md#listresolverconfigsresponsetypedef) 


```python
# list_resolver_configs method usage example with argument unpacking

kwargs: ListResolverConfigsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_resolver_configs(**kwargs)
```

1. See [:material-code-braces: ListResolverConfigsRequestRequestTypeDef](./type_defs.md#listresolverconfigsrequestrequesttypedef) 

### list\_resolver\_dnssec\_configs

Lists the configurations for DNSSEC validation that are associated with the
current Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_resolver_dnssec_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_dnssec_configs)

```python
# list_resolver_dnssec_configs method definition

await def list_resolver_dnssec_configs(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListResolverDnssecConfigsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListResolverDnssecConfigsResponseTypeDef](./type_defs.md#listresolverdnssecconfigsresponsetypedef) 


```python
# list_resolver_dnssec_configs method usage example with argument unpacking

kwargs: ListResolverDnssecConfigsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_resolver_dnssec_configs(**kwargs)
```

1. See [:material-code-braces: ListResolverDnssecConfigsRequestRequestTypeDef](./type_defs.md#listresolverdnssecconfigsrequestrequesttypedef) 

### list\_resolver\_endpoint\_ip\_addresses

Gets the IP addresses for a specified Resolver endpoint.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_resolver_endpoint_ip_addresses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_endpoint_ip_addresses)

```python
# list_resolver_endpoint_ip_addresses method definition

await def list_resolver_endpoint_ip_addresses(
    self,
    *,
    ResolverEndpointId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListResolverEndpointIpAddressesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResolverEndpointIpAddressesResponseTypeDef](./type_defs.md#listresolverendpointipaddressesresponsetypedef) 


```python
# list_resolver_endpoint_ip_addresses method usage example with argument unpacking

kwargs: ListResolverEndpointIpAddressesRequestRequestTypeDef = {  # (1)
    "ResolverEndpointId": ...,
}

parent.list_resolver_endpoint_ip_addresses(**kwargs)
```

1. See [:material-code-braces: ListResolverEndpointIpAddressesRequestRequestTypeDef](./type_defs.md#listresolverendpointipaddressesrequestrequesttypedef) 

### list\_resolver\_endpoints

Lists all the Resolver endpoints that were created using the current Amazon Web
Services account.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_resolver_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_endpoints)

```python
# list_resolver_endpoints method definition

await def list_resolver_endpoints(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListResolverEndpointsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListResolverEndpointsResponseTypeDef](./type_defs.md#listresolverendpointsresponsetypedef) 


```python
# list_resolver_endpoints method usage example with argument unpacking

kwargs: ListResolverEndpointsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_resolver_endpoints(**kwargs)
```

1. See [:material-code-braces: ListResolverEndpointsRequestRequestTypeDef](./type_defs.md#listresolverendpointsrequestrequesttypedef) 

### list\_resolver\_query\_log\_config\_associations

Lists information about associations between Amazon VPCs and query logging
configurations.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_resolver_query_log_config_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_query_log_config_associations)

```python
# list_resolver_query_log_config_associations method definition

await def list_resolver_query_log_config_associations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortBy: str = ...,
    SortOrder: SortOrderType = ...,  # (2)
) -> ListResolverQueryLogConfigAssociationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListResolverQueryLogConfigAssociationsResponseTypeDef](./type_defs.md#listresolverquerylogconfigassociationsresponsetypedef) 


```python
# list_resolver_query_log_config_associations method usage example with argument unpacking

kwargs: ListResolverQueryLogConfigAssociationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_resolver_query_log_config_associations(**kwargs)
```

1. See [:material-code-braces: ListResolverQueryLogConfigAssociationsRequestRequestTypeDef](./type_defs.md#listresolverquerylogconfigassociationsrequestrequesttypedef) 

### list\_resolver\_query\_log\_configs

Lists information about the specified query logging configurations.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_resolver_query_log_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_query_log_configs)

```python
# list_resolver_query_log_configs method definition

await def list_resolver_query_log_configs(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortBy: str = ...,
    SortOrder: SortOrderType = ...,  # (2)
) -> ListResolverQueryLogConfigsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListResolverQueryLogConfigsResponseTypeDef](./type_defs.md#listresolverquerylogconfigsresponsetypedef) 


```python
# list_resolver_query_log_configs method usage example with argument unpacking

kwargs: ListResolverQueryLogConfigsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_resolver_query_log_configs(**kwargs)
```

1. See [:material-code-braces: ListResolverQueryLogConfigsRequestRequestTypeDef](./type_defs.md#listresolverquerylogconfigsrequestrequesttypedef) 

### list\_resolver\_rule\_associations

Lists the associations that were created between Resolver rules and VPCs using
the current Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_resolver_rule_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_rule_associations)

```python
# list_resolver_rule_associations method definition

await def list_resolver_rule_associations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListResolverRuleAssociationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListResolverRuleAssociationsResponseTypeDef](./type_defs.md#listresolverruleassociationsresponsetypedef) 


```python
# list_resolver_rule_associations method usage example with argument unpacking

kwargs: ListResolverRuleAssociationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_resolver_rule_associations(**kwargs)
```

1. See [:material-code-braces: ListResolverRuleAssociationsRequestRequestTypeDef](./type_defs.md#listresolverruleassociationsrequestrequesttypedef) 

### list\_resolver\_rules

Lists the Resolver rules that were created using the current Amazon Web Services
account.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_resolver_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_rules)

```python
# list_resolver_rules method definition

await def list_resolver_rules(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListResolverRulesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListResolverRulesResponseTypeDef](./type_defs.md#listresolverrulesresponsetypedef) 


```python
# list_resolver_rules method usage example with argument unpacking

kwargs: ListResolverRulesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_resolver_rules(**kwargs)
```

1. See [:material-code-braces: ListResolverRulesRequestRequestTypeDef](./type_defs.md#listresolverrulesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags that you associated with the specified resource.

Type annotations and code completion for `#!python session.create_client("route53resolver").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_firewall\_rule\_group\_policy

Attaches an Identity and Access Management (Amazon Web Services IAM) policy for
sharing the rule group.

Type annotations and code completion for `#!python session.create_client("route53resolver").put_firewall_rule_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.put_firewall_rule_group_policy)

```python
# put_firewall_rule_group_policy method definition

await def put_firewall_rule_group_policy(
    self,
    *,
    Arn: str,
    FirewallRuleGroupPolicy: str,
) -> PutFirewallRuleGroupPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutFirewallRuleGroupPolicyResponseTypeDef](./type_defs.md#putfirewallrulegrouppolicyresponsetypedef) 


```python
# put_firewall_rule_group_policy method usage example with argument unpacking

kwargs: PutFirewallRuleGroupPolicyRequestRequestTypeDef = {  # (1)
    "Arn": ...,
    "FirewallRuleGroupPolicy": ...,
}

parent.put_firewall_rule_group_policy(**kwargs)
```

1. See [:material-code-braces: PutFirewallRuleGroupPolicyRequestRequestTypeDef](./type_defs.md#putfirewallrulegrouppolicyrequestrequesttypedef) 

### put\_resolver\_query\_log\_config\_policy

Specifies an Amazon Web Services account that you want to share a query logging
configuration with, the query logging configuration that you want to share, and
the operations that you want the account to be able to perform on the
configuration.

Type annotations and code completion for `#!python session.create_client("route53resolver").put_resolver_query_log_config_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.put_resolver_query_log_config_policy)

```python
# put_resolver_query_log_config_policy method definition

await def put_resolver_query_log_config_policy(
    self,
    *,
    Arn: str,
    ResolverQueryLogConfigPolicy: str,
) -> PutResolverQueryLogConfigPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutResolverQueryLogConfigPolicyResponseTypeDef](./type_defs.md#putresolverquerylogconfigpolicyresponsetypedef) 


```python
# put_resolver_query_log_config_policy method usage example with argument unpacking

kwargs: PutResolverQueryLogConfigPolicyRequestRequestTypeDef = {  # (1)
    "Arn": ...,
    "ResolverQueryLogConfigPolicy": ...,
}

parent.put_resolver_query_log_config_policy(**kwargs)
```

1. See [:material-code-braces: PutResolverQueryLogConfigPolicyRequestRequestTypeDef](./type_defs.md#putresolverquerylogconfigpolicyrequestrequesttypedef) 

### put\_resolver\_rule\_policy

Specifies an Amazon Web Services rule that you want to share with another
account, the account that you want to share the rule with, and the operations
that you want the account to be able to perform on the rule.

Type annotations and code completion for `#!python session.create_client("route53resolver").put_resolver_rule_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.put_resolver_rule_policy)

```python
# put_resolver_rule_policy method definition

await def put_resolver_rule_policy(
    self,
    *,
    Arn: str,
    ResolverRulePolicy: str,
) -> PutResolverRulePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutResolverRulePolicyResponseTypeDef](./type_defs.md#putresolverrulepolicyresponsetypedef) 


```python
# put_resolver_rule_policy method usage example with argument unpacking

kwargs: PutResolverRulePolicyRequestRequestTypeDef = {  # (1)
    "Arn": ...,
    "ResolverRulePolicy": ...,
}

parent.put_resolver_rule_policy(**kwargs)
```

1. See [:material-code-braces: PutResolverRulePolicyRequestRequestTypeDef](./type_defs.md#putresolverrulepolicyrequestrequesttypedef) 

### tag\_resource

Adds one or more tags to a specified resource.

Type annotations and code completion for `#!python session.create_client("route53resolver").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes one or more tags from a specified resource.

Type annotations and code completion for `#!python session.create_client("route53resolver").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_firewall\_config

Updates the configuration of the firewall behavior provided by DNS Firewall for
a single VPC from Amazon Virtual Private Cloud (Amazon VPC).

Type annotations and code completion for `#!python session.create_client("route53resolver").update_firewall_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_config)

```python
# update_firewall_config method definition

await def update_firewall_config(
    self,
    *,
    ResourceId: str,
    FirewallFailOpen: FirewallFailOpenStatusType,  # (1)
) -> UpdateFirewallConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FirewallFailOpenStatusType](./literals.md#firewallfailopenstatustype) 
2. See [:material-code-braces: UpdateFirewallConfigResponseTypeDef](./type_defs.md#updatefirewallconfigresponsetypedef) 


```python
# update_firewall_config method usage example with argument unpacking

kwargs: UpdateFirewallConfigRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "FirewallFailOpen": ...,
}

parent.update_firewall_config(**kwargs)
```

1. See [:material-code-braces: UpdateFirewallConfigRequestRequestTypeDef](./type_defs.md#updatefirewallconfigrequestrequesttypedef) 

### update\_firewall\_domains

Updates the firewall domain list from an array of domain specifications.

Type annotations and code completion for `#!python session.create_client("route53resolver").update_firewall_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_domains)

```python
# update_firewall_domains method definition

await def update_firewall_domains(
    self,
    *,
    FirewallDomainListId: str,
    Operation: FirewallDomainUpdateOperationType,  # (1)
    Domains: Sequence[str],
) -> UpdateFirewallDomainsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FirewallDomainUpdateOperationType](./literals.md#firewalldomainupdateoperationtype) 
2. See [:material-code-braces: UpdateFirewallDomainsResponseTypeDef](./type_defs.md#updatefirewalldomainsresponsetypedef) 


```python
# update_firewall_domains method usage example with argument unpacking

kwargs: UpdateFirewallDomainsRequestRequestTypeDef = {  # (1)
    "FirewallDomainListId": ...,
    "Operation": ...,
    "Domains": ...,
}

parent.update_firewall_domains(**kwargs)
```

1. See [:material-code-braces: UpdateFirewallDomainsRequestRequestTypeDef](./type_defs.md#updatefirewalldomainsrequestrequesttypedef) 

### update\_firewall\_rule

Updates the specified firewall rule.

Type annotations and code completion for `#!python session.create_client("route53resolver").update_firewall_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule)

```python
# update_firewall_rule method definition

await def update_firewall_rule(
    self,
    *,
    FirewallRuleGroupId: str,
    FirewallDomainListId: str,
    Priority: int = ...,
    Action: ActionType = ...,  # (1)
    BlockResponse: BlockResponseType = ...,  # (2)
    BlockOverrideDomain: str = ...,
    BlockOverrideDnsType: BlockOverrideDnsTypeType = ...,  # (3)
    BlockOverrideTtl: int = ...,
    Name: str = ...,
) -> UpdateFirewallRuleResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
2. See [:material-code-brackets: BlockResponseType](./literals.md#blockresponsetype) 
3. See [:material-code-brackets: BlockOverrideDnsTypeType](./literals.md#blockoverridednstypetype) 
4. See [:material-code-braces: UpdateFirewallRuleResponseTypeDef](./type_defs.md#updatefirewallruleresponsetypedef) 


```python
# update_firewall_rule method usage example with argument unpacking

kwargs: UpdateFirewallRuleRequestRequestTypeDef = {  # (1)
    "FirewallRuleGroupId": ...,
    "FirewallDomainListId": ...,
}

parent.update_firewall_rule(**kwargs)
```

1. See [:material-code-braces: UpdateFirewallRuleRequestRequestTypeDef](./type_defs.md#updatefirewallrulerequestrequesttypedef) 

### update\_firewall\_rule\_group\_association

Changes the association of a  FirewallRuleGroup with a VPC.

Type annotations and code completion for `#!python session.create_client("route53resolver").update_firewall_rule_group_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule_group_association)

```python
# update_firewall_rule_group_association method definition

await def update_firewall_rule_group_association(
    self,
    *,
    FirewallRuleGroupAssociationId: str,
    Priority: int = ...,
    MutationProtection: MutationProtectionStatusType = ...,  # (1)
    Name: str = ...,
) -> UpdateFirewallRuleGroupAssociationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MutationProtectionStatusType](./literals.md#mutationprotectionstatustype) 
2. See [:material-code-braces: UpdateFirewallRuleGroupAssociationResponseTypeDef](./type_defs.md#updatefirewallrulegroupassociationresponsetypedef) 


```python
# update_firewall_rule_group_association method usage example with argument unpacking

kwargs: UpdateFirewallRuleGroupAssociationRequestRequestTypeDef = {  # (1)
    "FirewallRuleGroupAssociationId": ...,
}

parent.update_firewall_rule_group_association(**kwargs)
```

1. See [:material-code-braces: UpdateFirewallRuleGroupAssociationRequestRequestTypeDef](./type_defs.md#updatefirewallrulegroupassociationrequestrequesttypedef) 

### update\_outpost\_resolver

You can use `UpdateOutpostResolver` to update the instance count, type, or name
of a Resolver on an Outpost.

Type annotations and code completion for `#!python session.create_client("route53resolver").update_outpost_resolver` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_outpost_resolver)

```python
# update_outpost_resolver method definition

await def update_outpost_resolver(
    self,
    *,
    Id: str,
    Name: str = ...,
    InstanceCount: int = ...,
    PreferredInstanceType: str = ...,
) -> UpdateOutpostResolverResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateOutpostResolverResponseTypeDef](./type_defs.md#updateoutpostresolverresponsetypedef) 


```python
# update_outpost_resolver method usage example with argument unpacking

kwargs: UpdateOutpostResolverRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.update_outpost_resolver(**kwargs)
```

1. See [:material-code-braces: UpdateOutpostResolverRequestRequestTypeDef](./type_defs.md#updateoutpostresolverrequestrequesttypedef) 

### update\_resolver\_config

Updates the behavior configuration of Route 53 Resolver behavior for a single
VPC from Amazon Virtual Private Cloud.

Type annotations and code completion for `#!python session.create_client("route53resolver").update_resolver_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_resolver_config)

```python
# update_resolver_config method definition

await def update_resolver_config(
    self,
    *,
    ResourceId: str,
    AutodefinedReverseFlag: AutodefinedReverseFlagType,  # (1)
) -> UpdateResolverConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AutodefinedReverseFlagType](./literals.md#autodefinedreverseflagtype) 
2. See [:material-code-braces: UpdateResolverConfigResponseTypeDef](./type_defs.md#updateresolverconfigresponsetypedef) 


```python
# update_resolver_config method usage example with argument unpacking

kwargs: UpdateResolverConfigRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "AutodefinedReverseFlag": ...,
}

parent.update_resolver_config(**kwargs)
```

1. See [:material-code-braces: UpdateResolverConfigRequestRequestTypeDef](./type_defs.md#updateresolverconfigrequestrequesttypedef) 

### update\_resolver\_dnssec\_config

Updates an existing DNSSEC validation configuration.

Type annotations and code completion for `#!python session.create_client("route53resolver").update_resolver_dnssec_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_resolver_dnssec_config)

```python
# update_resolver_dnssec_config method definition

await def update_resolver_dnssec_config(
    self,
    *,
    ResourceId: str,
    Validation: ValidationType,  # (1)
) -> UpdateResolverDnssecConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ValidationType](./literals.md#validationtype) 
2. See [:material-code-braces: UpdateResolverDnssecConfigResponseTypeDef](./type_defs.md#updateresolverdnssecconfigresponsetypedef) 


```python
# update_resolver_dnssec_config method usage example with argument unpacking

kwargs: UpdateResolverDnssecConfigRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "Validation": ...,
}

parent.update_resolver_dnssec_config(**kwargs)
```

1. See [:material-code-braces: UpdateResolverDnssecConfigRequestRequestTypeDef](./type_defs.md#updateresolverdnssecconfigrequestrequesttypedef) 

### update\_resolver\_endpoint

Updates the name, or enpoint type for an inbound or an outbound Resolver
endpoint.

Type annotations and code completion for `#!python session.create_client("route53resolver").update_resolver_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_resolver_endpoint)

```python
# update_resolver_endpoint method definition

await def update_resolver_endpoint(
    self,
    *,
    ResolverEndpointId: str,
    Name: str = ...,
    ResolverEndpointType: ResolverEndpointTypeType = ...,  # (1)
    UpdateIpAddresses: Sequence[UpdateIpAddressTypeDef] = ...,  # (2)
) -> UpdateResolverEndpointResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ResolverEndpointTypeType](./literals.md#resolverendpointtypetype) 
2. See [:material-code-braces: UpdateIpAddressTypeDef](./type_defs.md#updateipaddresstypedef) 
3. See [:material-code-braces: UpdateResolverEndpointResponseTypeDef](./type_defs.md#updateresolverendpointresponsetypedef) 


```python
# update_resolver_endpoint method usage example with argument unpacking

kwargs: UpdateResolverEndpointRequestRequestTypeDef = {  # (1)
    "ResolverEndpointId": ...,
}

parent.update_resolver_endpoint(**kwargs)
```

1. See [:material-code-braces: UpdateResolverEndpointRequestRequestTypeDef](./type_defs.md#updateresolverendpointrequestrequesttypedef) 

### update\_resolver\_rule

Updates settings for a specified Resolver rule.

Type annotations and code completion for `#!python session.create_client("route53resolver").update_resolver_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_resolver_rule)

```python
# update_resolver_rule method definition

await def update_resolver_rule(
    self,
    *,
    ResolverRuleId: str,
    Config: ResolverRuleConfigTypeDef,  # (1)
) -> UpdateResolverRuleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResolverRuleConfigTypeDef](./type_defs.md#resolverruleconfigtypedef) 
2. See [:material-code-braces: UpdateResolverRuleResponseTypeDef](./type_defs.md#updateresolverruleresponsetypedef) 


```python
# update_resolver_rule method usage example with argument unpacking

kwargs: UpdateResolverRuleRequestRequestTypeDef = {  # (1)
    "ResolverRuleId": ...,
    "Config": ...,
}

parent.update_resolver_rule(**kwargs)
```

1. See [:material-code-braces: UpdateResolverRuleRequestRequestTypeDef](./type_defs.md#updateresolverrulerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("route53resolver").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Route53ResolverClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("route53resolver").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator` method with overloads.

- `client.get_paginator("list_firewall_configs")` -> [ListFirewallConfigsPaginator](./paginators.md#listfirewallconfigspaginator)
- `client.get_paginator("list_firewall_domain_lists")` -> [ListFirewallDomainListsPaginator](./paginators.md#listfirewalldomainlistspaginator)
- `client.get_paginator("list_firewall_domains")` -> [ListFirewallDomainsPaginator](./paginators.md#listfirewalldomainspaginator)
- `client.get_paginator("list_firewall_rule_group_associations")` -> [ListFirewallRuleGroupAssociationsPaginator](./paginators.md#listfirewallrulegroupassociationspaginator)
- `client.get_paginator("list_firewall_rule_groups")` -> [ListFirewallRuleGroupsPaginator](./paginators.md#listfirewallrulegroupspaginator)
- `client.get_paginator("list_firewall_rules")` -> [ListFirewallRulesPaginator](./paginators.md#listfirewallrulespaginator)
- `client.get_paginator("list_outpost_resolvers")` -> [ListOutpostResolversPaginator](./paginators.md#listoutpostresolverspaginator)
- `client.get_paginator("list_resolver_configs")` -> [ListResolverConfigsPaginator](./paginators.md#listresolverconfigspaginator)
- `client.get_paginator("list_resolver_dnssec_configs")` -> [ListResolverDnssecConfigsPaginator](./paginators.md#listresolverdnssecconfigspaginator)
- `client.get_paginator("list_resolver_endpoint_ip_addresses")` -> [ListResolverEndpointIpAddressesPaginator](./paginators.md#listresolverendpointipaddressespaginator)
- `client.get_paginator("list_resolver_endpoints")` -> [ListResolverEndpointsPaginator](./paginators.md#listresolverendpointspaginator)
- `client.get_paginator("list_resolver_query_log_config_associations")` -> [ListResolverQueryLogConfigAssociationsPaginator](./paginators.md#listresolverquerylogconfigassociationspaginator)
- `client.get_paginator("list_resolver_query_log_configs")` -> [ListResolverQueryLogConfigsPaginator](./paginators.md#listresolverquerylogconfigspaginator)
- `client.get_paginator("list_resolver_rule_associations")` -> [ListResolverRuleAssociationsPaginator](./paginators.md#listresolverruleassociationspaginator)
- `client.get_paginator("list_resolver_rules")` -> [ListResolverRulesPaginator](./paginators.md#listresolverrulespaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)



