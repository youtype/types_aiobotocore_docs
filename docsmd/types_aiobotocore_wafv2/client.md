# WAFV2Client

> [Index](../README.md) > [WAFV2](./README.md) > WAFV2Client

!!! note ""

    Auto-generated documentation for [WAFV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#wafv2)
    type annotations stubs module [types-aiobotocore-wafv2](https://pypi.org/project/types-aiobotocore-wafv2/).

## WAFV2Client

Type annotations and code completion for `#!python session.create_client("wafv2")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# WAFV2Client usage example

from aiobotocore.session import get_session
from types_aiobotocore_wafv2.client import WAFV2Client

session = get_session()
async with session.create_client("wafv2") as client:
    client: WAFV2Client
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("wafv2").exceptions` structure.

```python
# WAFV2Client.exceptions usage example

async with session.create_client("wafv2") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.WAFAssociatedItemException,
        client.WAFConfigurationWarningException,
        client.WAFDuplicateItemException,
        client.WAFExpiredManagedRuleGroupVersionException,
        client.WAFInternalErrorException,
        client.WAFInvalidOperationException,
        client.WAFInvalidParameterException,
        client.WAFInvalidPermissionPolicyException,
        client.WAFInvalidResourceException,
        client.WAFLimitsExceededException,
        client.WAFLogDestinationPermissionIssueException,
        client.WAFNonexistentItemException,
        client.WAFOptimisticLockException,
        client.WAFServiceLinkedRoleErrorException,
        client.WAFSubscriptionNotFoundException,
        client.WAFTagOperationException,
        client.WAFTagOperationInternalErrorException,
        client.WAFUnavailableEntityException,
        client.WAFUnsupportedAggregateKeyTypeException,
    ) as e:
        print(e)
```

```python
# WAFV2Client usage type checking example

from types_aiobotocore_wafv2.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("wafv2").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("wafv2").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/generate_presigned_url.html)

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


### associate\_web\_acl

Associates a web ACL with a resource, to protect the resource.

Type annotations and code completion for `#!python session.create_client("wafv2").associate_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/associate_web_acl.html)

```python
# associate_web_acl method definition

await def associate_web_acl(
    self,
    *,
    WebACLArn: str,
    ResourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_web_acl method usage example with argument unpacking

kwargs: AssociateWebACLRequestTypeDef = {  # (1)
    "WebACLArn": ...,
    "ResourceArn": ...,
}

parent.associate_web_acl(**kwargs)
```

1. See [:material-code-braces: AssociateWebACLRequestTypeDef](./type_defs.md#associatewebaclrequesttypedef) 

### check\_capacity

Returns the web ACL capacity unit (WCU) requirements for a specified scope and
set of rules.

Type annotations and code completion for `#!python session.create_client("wafv2").check_capacity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/check_capacity.html)

```python
# check_capacity method definition

await def check_capacity(
    self,
    *,
    Scope: ScopeType,  # (1)
    Rules: Sequence[RuleUnionTypeDef],  # (2)
) -> CheckCapacityResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
3. See [:material-code-braces: CheckCapacityResponseTypeDef](./type_defs.md#checkcapacityresponsetypedef) 


```python
# check_capacity method usage example with argument unpacking

kwargs: CheckCapacityRequestTypeDef = {  # (1)
    "Scope": ...,
    "Rules": ...,
}

parent.check_capacity(**kwargs)
```

1. See [:material-code-braces: CheckCapacityRequestTypeDef](./type_defs.md#checkcapacityrequesttypedef) 

### create\_api\_key

Creates an API key that contains a set of token domains.

Type annotations and code completion for `#!python session.create_client("wafv2").create_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/create_api_key.html)

```python
# create_api_key method definition

await def create_api_key(
    self,
    *,
    Scope: ScopeType,  # (1)
    TokenDomains: Sequence[str],
) -> CreateAPIKeyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: CreateAPIKeyResponseTypeDef](./type_defs.md#createapikeyresponsetypedef) 


```python
# create_api_key method usage example with argument unpacking

kwargs: CreateAPIKeyRequestTypeDef = {  # (1)
    "Scope": ...,
    "TokenDomains": ...,
}

parent.create_api_key(**kwargs)
```

1. See [:material-code-braces: CreateAPIKeyRequestTypeDef](./type_defs.md#createapikeyrequesttypedef) 

### create\_ip\_set

Creates an <a>IPSet</a>, which you use to identify web requests that originate
from specific IP addresses or ranges of IP addresses.

Type annotations and code completion for `#!python session.create_client("wafv2").create_ip_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/create_ip_set.html)

```python
# create_ip_set method definition

await def create_ip_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    IPAddressVersion: IPAddressVersionType,  # (2)
    Addresses: Sequence[str],
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateIPSetResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-brackets: IPAddressVersionType](./literals.md#ipaddressversiontype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateIPSetResponseTypeDef](./type_defs.md#createipsetresponsetypedef) 


```python
# create_ip_set method usage example with argument unpacking

kwargs: CreateIPSetRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "IPAddressVersion": ...,
    "Addresses": ...,
}

parent.create_ip_set(**kwargs)
```

1. See [:material-code-braces: CreateIPSetRequestTypeDef](./type_defs.md#createipsetrequesttypedef) 

### create\_regex\_pattern\_set

Creates a <a>RegexPatternSet</a>, which you reference in a
<a>RegexPatternSetReferenceStatement</a>, to have WAF inspect a web request
component for the specified patterns.

Type annotations and code completion for `#!python session.create_client("wafv2").create_regex_pattern_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/create_regex_pattern_set.html)

```python
# create_regex_pattern_set method definition

await def create_regex_pattern_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    RegularExpressionList: Sequence[RegexTypeDef],  # (2)
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateRegexPatternSetResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: RegexTypeDef](./type_defs.md#regextypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateRegexPatternSetResponseTypeDef](./type_defs.md#createregexpatternsetresponsetypedef) 


```python
# create_regex_pattern_set method usage example with argument unpacking

kwargs: CreateRegexPatternSetRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "RegularExpressionList": ...,
}

parent.create_regex_pattern_set(**kwargs)
```

1. See [:material-code-braces: CreateRegexPatternSetRequestTypeDef](./type_defs.md#createregexpatternsetrequesttypedef) 

### create\_rule\_group

Creates a <a>RuleGroup</a> per the specifications provided.

Type annotations and code completion for `#!python session.create_client("wafv2").create_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/create_rule_group.html)

```python
# create_rule_group method definition

await def create_rule_group(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Capacity: int,
    VisibilityConfig: VisibilityConfigTypeDef,  # (2)
    Description: str = ...,
    Rules: Sequence[RuleUnionTypeDef] = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,  # (5)
) -> CreateRuleGroupResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
3. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
6. See [:material-code-braces: CreateRuleGroupResponseTypeDef](./type_defs.md#createrulegroupresponsetypedef) 


```python
# create_rule_group method usage example with argument unpacking

kwargs: CreateRuleGroupRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Capacity": ...,
    "VisibilityConfig": ...,
}

parent.create_rule_group(**kwargs)
```

1. See [:material-code-braces: CreateRuleGroupRequestTypeDef](./type_defs.md#createrulegrouprequesttypedef) 

### create\_web\_acl

Creates a <a>WebACL</a> per the specifications provided.

Type annotations and code completion for `#!python session.create_client("wafv2").create_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/create_web_acl.html)

```python
# create_web_acl method definition

await def create_web_acl(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    DefaultAction: DefaultActionUnionTypeDef,  # (2)
    VisibilityConfig: VisibilityConfigTypeDef,  # (3)
    Description: str = ...,
    Rules: Sequence[RuleUnionTypeDef] = ...,  # (4)
    DataProtectionConfig: DataProtectionConfigUnionTypeDef = ...,  # (5)
    Tags: Sequence[TagTypeDef] = ...,  # (6)
    CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,  # (7)
    CaptchaConfig: CaptchaConfigTypeDef = ...,  # (8)
    ChallengeConfig: ChallengeConfigTypeDef = ...,  # (9)
    TokenDomains: Sequence[str] = ...,
    AssociationConfig: AssociationConfigUnionTypeDef = ...,  # (10)
) -> CreateWebACLResponseTypeDef:  # (11)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DefaultActionTypeDef](./type_defs.md#defaultactiontypedef) [:material-code-braces: DefaultActionOutputTypeDef](./type_defs.md#defaultactionoutputtypedef) 
3. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
4. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
5. See [:material-code-braces: DataProtectionConfigTypeDef](./type_defs.md#dataprotectionconfigtypedef) [:material-code-braces: DataProtectionConfigOutputTypeDef](./type_defs.md#dataprotectionconfigoutputtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
8. See [:material-code-braces: CaptchaConfigTypeDef](./type_defs.md#captchaconfigtypedef) 
9. See [:material-code-braces: ChallengeConfigTypeDef](./type_defs.md#challengeconfigtypedef) 
10. See [:material-code-braces: AssociationConfigTypeDef](./type_defs.md#associationconfigtypedef) [:material-code-braces: AssociationConfigOutputTypeDef](./type_defs.md#associationconfigoutputtypedef) 
11. See [:material-code-braces: CreateWebACLResponseTypeDef](./type_defs.md#createwebaclresponsetypedef) 


```python
# create_web_acl method usage example with argument unpacking

kwargs: CreateWebACLRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "DefaultAction": ...,
    "VisibilityConfig": ...,
}

parent.create_web_acl(**kwargs)
```

1. See [:material-code-braces: CreateWebACLRequestTypeDef](./type_defs.md#createwebaclrequesttypedef) 

### delete\_api\_key

Deletes the specified API key.

Type annotations and code completion for `#!python session.create_client("wafv2").delete_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/delete_api_key.html)

```python
# delete_api_key method definition

await def delete_api_key(
    self,
    *,
    Scope: ScopeType,  # (1)
    APIKey: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 


```python
# delete_api_key method usage example with argument unpacking

kwargs: DeleteAPIKeyRequestTypeDef = {  # (1)
    "Scope": ...,
    "APIKey": ...,
}

parent.delete_api_key(**kwargs)
```

1. See [:material-code-braces: DeleteAPIKeyRequestTypeDef](./type_defs.md#deleteapikeyrequesttypedef) 

### delete\_firewall\_manager\_rule\_groups

Deletes all rule groups that are managed by Firewall Manager from the specified
<a>WebACL</a>.

Type annotations and code completion for `#!python session.create_client("wafv2").delete_firewall_manager_rule_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/delete_firewall_manager_rule_groups.html)

```python
# delete_firewall_manager_rule_groups method definition

await def delete_firewall_manager_rule_groups(
    self,
    *,
    WebACLArn: str,
    WebACLLockToken: str,
) -> DeleteFirewallManagerRuleGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFirewallManagerRuleGroupsResponseTypeDef](./type_defs.md#deletefirewallmanagerrulegroupsresponsetypedef) 


```python
# delete_firewall_manager_rule_groups method usage example with argument unpacking

kwargs: DeleteFirewallManagerRuleGroupsRequestTypeDef = {  # (1)
    "WebACLArn": ...,
    "WebACLLockToken": ...,
}

parent.delete_firewall_manager_rule_groups(**kwargs)
```

1. See [:material-code-braces: DeleteFirewallManagerRuleGroupsRequestTypeDef](./type_defs.md#deletefirewallmanagerrulegroupsrequesttypedef) 

### delete\_ip\_set

Deletes the specified <a>IPSet</a>.

Type annotations and code completion for `#!python session.create_client("wafv2").delete_ip_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/delete_ip_set.html)

```python
# delete_ip_set method definition

await def delete_ip_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 


```python
# delete_ip_set method usage example with argument unpacking

kwargs: DeleteIPSetRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "LockToken": ...,
}

parent.delete_ip_set(**kwargs)
```

1. See [:material-code-braces: DeleteIPSetRequestTypeDef](./type_defs.md#deleteipsetrequesttypedef) 

### delete\_logging\_configuration

Deletes the <a>LoggingConfiguration</a> from the specified web ACL.

Type annotations and code completion for `#!python session.create_client("wafv2").delete_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/delete_logging_configuration.html)

```python
# delete_logging_configuration method definition

await def delete_logging_configuration(
    self,
    *,
    ResourceArn: str,
    LogType: LogTypeType = ...,  # (1)
    LogScope: LogScopeType = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-brackets: LogScopeType](./literals.md#logscopetype) 


```python
# delete_logging_configuration method usage example with argument unpacking

kwargs: DeleteLoggingConfigurationRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.delete_logging_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteLoggingConfigurationRequestTypeDef](./type_defs.md#deleteloggingconfigurationrequesttypedef) 

### delete\_permission\_policy

Permanently deletes an IAM policy from the specified rule group.

Type annotations and code completion for `#!python session.create_client("wafv2").delete_permission_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/delete_permission_policy.html)

```python
# delete_permission_policy method definition

await def delete_permission_policy(
    self,
    *,
    ResourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_permission_policy method usage example with argument unpacking

kwargs: DeletePermissionPolicyRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.delete_permission_policy(**kwargs)
```

1. See [:material-code-braces: DeletePermissionPolicyRequestTypeDef](./type_defs.md#deletepermissionpolicyrequesttypedef) 

### delete\_regex\_pattern\_set

Deletes the specified <a>RegexPatternSet</a>.

Type annotations and code completion for `#!python session.create_client("wafv2").delete_regex_pattern_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/delete_regex_pattern_set.html)

```python
# delete_regex_pattern_set method definition

await def delete_regex_pattern_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 


```python
# delete_regex_pattern_set method usage example with argument unpacking

kwargs: DeleteRegexPatternSetRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "LockToken": ...,
}

parent.delete_regex_pattern_set(**kwargs)
```

1. See [:material-code-braces: DeleteRegexPatternSetRequestTypeDef](./type_defs.md#deleteregexpatternsetrequesttypedef) 

### delete\_rule\_group

Deletes the specified <a>RuleGroup</a>.

Type annotations and code completion for `#!python session.create_client("wafv2").delete_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/delete_rule_group.html)

```python
# delete_rule_group method definition

await def delete_rule_group(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 


```python
# delete_rule_group method usage example with argument unpacking

kwargs: DeleteRuleGroupRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "LockToken": ...,
}

parent.delete_rule_group(**kwargs)
```

1. See [:material-code-braces: DeleteRuleGroupRequestTypeDef](./type_defs.md#deleterulegrouprequesttypedef) 

### delete\_web\_acl

Deletes the specified <a>WebACL</a>.

Type annotations and code completion for `#!python session.create_client("wafv2").delete_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/delete_web_acl.html)

```python
# delete_web_acl method definition

await def delete_web_acl(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 


```python
# delete_web_acl method usage example with argument unpacking

kwargs: DeleteWebACLRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "LockToken": ...,
}

parent.delete_web_acl(**kwargs)
```

1. See [:material-code-braces: DeleteWebACLRequestTypeDef](./type_defs.md#deletewebaclrequesttypedef) 

### describe\_all\_managed\_products

Provides high-level information for the Amazon Web Services Managed Rules rule
groups and Amazon Web Services Marketplace managed rule groups.

Type annotations and code completion for `#!python session.create_client("wafv2").describe_all_managed_products` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/describe_all_managed_products.html)

```python
# describe_all_managed_products method definition

await def describe_all_managed_products(
    self,
    *,
    Scope: ScopeType,  # (1)
) -> DescribeAllManagedProductsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DescribeAllManagedProductsResponseTypeDef](./type_defs.md#describeallmanagedproductsresponsetypedef) 


```python
# describe_all_managed_products method usage example with argument unpacking

kwargs: DescribeAllManagedProductsRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.describe_all_managed_products(**kwargs)
```

1. See [:material-code-braces: DescribeAllManagedProductsRequestTypeDef](./type_defs.md#describeallmanagedproductsrequesttypedef) 

### describe\_managed\_products\_by\_vendor

Provides high-level information for the managed rule groups owned by a specific
vendor.

Type annotations and code completion for `#!python session.create_client("wafv2").describe_managed_products_by_vendor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/describe_managed_products_by_vendor.html)

```python
# describe_managed_products_by_vendor method definition

await def describe_managed_products_by_vendor(
    self,
    *,
    VendorName: str,
    Scope: ScopeType,  # (1)
) -> DescribeManagedProductsByVendorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DescribeManagedProductsByVendorResponseTypeDef](./type_defs.md#describemanagedproductsbyvendorresponsetypedef) 


```python
# describe_managed_products_by_vendor method usage example with argument unpacking

kwargs: DescribeManagedProductsByVendorRequestTypeDef = {  # (1)
    "VendorName": ...,
    "Scope": ...,
}

parent.describe_managed_products_by_vendor(**kwargs)
```

1. See [:material-code-braces: DescribeManagedProductsByVendorRequestTypeDef](./type_defs.md#describemanagedproductsbyvendorrequesttypedef) 

### describe\_managed\_rule\_group

Provides high-level information for a managed rule group, including
descriptions of the rules.

Type annotations and code completion for `#!python session.create_client("wafv2").describe_managed_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/describe_managed_rule_group.html)

```python
# describe_managed_rule_group method definition

await def describe_managed_rule_group(
    self,
    *,
    VendorName: str,
    Name: str,
    Scope: ScopeType,  # (1)
    VersionName: str = ...,
) -> DescribeManagedRuleGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DescribeManagedRuleGroupResponseTypeDef](./type_defs.md#describemanagedrulegroupresponsetypedef) 


```python
# describe_managed_rule_group method usage example with argument unpacking

kwargs: DescribeManagedRuleGroupRequestTypeDef = {  # (1)
    "VendorName": ...,
    "Name": ...,
    "Scope": ...,
}

parent.describe_managed_rule_group(**kwargs)
```

1. See [:material-code-braces: DescribeManagedRuleGroupRequestTypeDef](./type_defs.md#describemanagedrulegrouprequesttypedef) 

### disassociate\_web\_acl

Disassociates the specified resource from its web ACL association, if it has
one.

Type annotations and code completion for `#!python session.create_client("wafv2").disassociate_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/disassociate_web_acl.html)

```python
# disassociate_web_acl method definition

await def disassociate_web_acl(
    self,
    *,
    ResourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_web_acl method usage example with argument unpacking

kwargs: DisassociateWebACLRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.disassociate_web_acl(**kwargs)
```

1. See [:material-code-braces: DisassociateWebACLRequestTypeDef](./type_defs.md#disassociatewebaclrequesttypedef) 

### generate\_mobile\_sdk\_release\_url

Generates a presigned download URL for the specified release of the mobile SDK.

Type annotations and code completion for `#!python session.create_client("wafv2").generate_mobile_sdk_release_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/generate_mobile_sdk_release_url.html)

```python
# generate_mobile_sdk_release_url method definition

await def generate_mobile_sdk_release_url(
    self,
    *,
    Platform: PlatformType,  # (1)
    ReleaseVersion: str,
) -> GenerateMobileSdkReleaseUrlResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: GenerateMobileSdkReleaseUrlResponseTypeDef](./type_defs.md#generatemobilesdkreleaseurlresponsetypedef) 


```python
# generate_mobile_sdk_release_url method usage example with argument unpacking

kwargs: GenerateMobileSdkReleaseUrlRequestTypeDef = {  # (1)
    "Platform": ...,
    "ReleaseVersion": ...,
}

parent.generate_mobile_sdk_release_url(**kwargs)
```

1. See [:material-code-braces: GenerateMobileSdkReleaseUrlRequestTypeDef](./type_defs.md#generatemobilesdkreleaseurlrequesttypedef) 

### get\_decrypted\_api\_key

Returns your API key in decrypted form.

Type annotations and code completion for `#!python session.create_client("wafv2").get_decrypted_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/get_decrypted_api_key.html)

```python
# get_decrypted_api_key method definition

await def get_decrypted_api_key(
    self,
    *,
    Scope: ScopeType,  # (1)
    APIKey: str,
) -> GetDecryptedAPIKeyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetDecryptedAPIKeyResponseTypeDef](./type_defs.md#getdecryptedapikeyresponsetypedef) 


```python
# get_decrypted_api_key method usage example with argument unpacking

kwargs: GetDecryptedAPIKeyRequestTypeDef = {  # (1)
    "Scope": ...,
    "APIKey": ...,
}

parent.get_decrypted_api_key(**kwargs)
```

1. See [:material-code-braces: GetDecryptedAPIKeyRequestTypeDef](./type_defs.md#getdecryptedapikeyrequesttypedef) 

### get\_ip\_set

Retrieves the specified <a>IPSet</a>.

Type annotations and code completion for `#!python session.create_client("wafv2").get_ip_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/get_ip_set.html)

```python
# get_ip_set method definition

await def get_ip_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
) -> GetIPSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetIPSetResponseTypeDef](./type_defs.md#getipsetresponsetypedef) 


```python
# get_ip_set method usage example with argument unpacking

kwargs: GetIPSetRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
}

parent.get_ip_set(**kwargs)
```

1. See [:material-code-braces: GetIPSetRequestTypeDef](./type_defs.md#getipsetrequesttypedef) 

### get\_logging\_configuration

Returns the <a>LoggingConfiguration</a> for the specified web ACL.

Type annotations and code completion for `#!python session.create_client("wafv2").get_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/get_logging_configuration.html)

```python
# get_logging_configuration method definition

await def get_logging_configuration(
    self,
    *,
    ResourceArn: str,
    LogType: LogTypeType = ...,  # (1)
    LogScope: LogScopeType = ...,  # (2)
) -> GetLoggingConfigurationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-brackets: LogScopeType](./literals.md#logscopetype) 
3. See [:material-code-braces: GetLoggingConfigurationResponseTypeDef](./type_defs.md#getloggingconfigurationresponsetypedef) 


```python
# get_logging_configuration method usage example with argument unpacking

kwargs: GetLoggingConfigurationRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_logging_configuration(**kwargs)
```

1. See [:material-code-braces: GetLoggingConfigurationRequestTypeDef](./type_defs.md#getloggingconfigurationrequesttypedef) 

### get\_managed\_rule\_set

Retrieves the specified managed rule set.

Type annotations and code completion for `#!python session.create_client("wafv2").get_managed_rule_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/get_managed_rule_set.html)

```python
# get_managed_rule_set method definition

await def get_managed_rule_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
) -> GetManagedRuleSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetManagedRuleSetResponseTypeDef](./type_defs.md#getmanagedrulesetresponsetypedef) 


```python
# get_managed_rule_set method usage example with argument unpacking

kwargs: GetManagedRuleSetRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
}

parent.get_managed_rule_set(**kwargs)
```

1. See [:material-code-braces: GetManagedRuleSetRequestTypeDef](./type_defs.md#getmanagedrulesetrequesttypedef) 

### get\_mobile\_sdk\_release

Retrieves information for the specified mobile SDK release, including release
notes and tags.

Type annotations and code completion for `#!python session.create_client("wafv2").get_mobile_sdk_release` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/get_mobile_sdk_release.html)

```python
# get_mobile_sdk_release method definition

await def get_mobile_sdk_release(
    self,
    *,
    Platform: PlatformType,  # (1)
    ReleaseVersion: str,
) -> GetMobileSdkReleaseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: GetMobileSdkReleaseResponseTypeDef](./type_defs.md#getmobilesdkreleaseresponsetypedef) 


```python
# get_mobile_sdk_release method usage example with argument unpacking

kwargs: GetMobileSdkReleaseRequestTypeDef = {  # (1)
    "Platform": ...,
    "ReleaseVersion": ...,
}

parent.get_mobile_sdk_release(**kwargs)
```

1. See [:material-code-braces: GetMobileSdkReleaseRequestTypeDef](./type_defs.md#getmobilesdkreleaserequesttypedef) 

### get\_permission\_policy

Returns the IAM policy that is attached to the specified rule group.

Type annotations and code completion for `#!python session.create_client("wafv2").get_permission_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/get_permission_policy.html)

```python
# get_permission_policy method definition

await def get_permission_policy(
    self,
    *,
    ResourceArn: str,
) -> GetPermissionPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPermissionPolicyResponseTypeDef](./type_defs.md#getpermissionpolicyresponsetypedef) 


```python
# get_permission_policy method usage example with argument unpacking

kwargs: GetPermissionPolicyRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_permission_policy(**kwargs)
```

1. See [:material-code-braces: GetPermissionPolicyRequestTypeDef](./type_defs.md#getpermissionpolicyrequesttypedef) 

### get\_rate\_based\_statement\_managed\_keys

Retrieves the IP addresses that are currently blocked by a rate-based rule
instance.

Type annotations and code completion for `#!python session.create_client("wafv2").get_rate_based_statement_managed_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/get_rate_based_statement_managed_keys.html)

```python
# get_rate_based_statement_managed_keys method definition

await def get_rate_based_statement_managed_keys(
    self,
    *,
    Scope: ScopeType,  # (1)
    WebACLName: str,
    WebACLId: str,
    RuleName: str,
    RuleGroupRuleName: str = ...,
) -> GetRateBasedStatementManagedKeysResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetRateBasedStatementManagedKeysResponseTypeDef](./type_defs.md#getratebasedstatementmanagedkeysresponsetypedef) 


```python
# get_rate_based_statement_managed_keys method usage example with argument unpacking

kwargs: GetRateBasedStatementManagedKeysRequestTypeDef = {  # (1)
    "Scope": ...,
    "WebACLName": ...,
    "WebACLId": ...,
    "RuleName": ...,
}

parent.get_rate_based_statement_managed_keys(**kwargs)
```

1. See [:material-code-braces: GetRateBasedStatementManagedKeysRequestTypeDef](./type_defs.md#getratebasedstatementmanagedkeysrequesttypedef) 

### get\_regex\_pattern\_set

Retrieves the specified <a>RegexPatternSet</a>.

Type annotations and code completion for `#!python session.create_client("wafv2").get_regex_pattern_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/get_regex_pattern_set.html)

```python
# get_regex_pattern_set method definition

await def get_regex_pattern_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
) -> GetRegexPatternSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetRegexPatternSetResponseTypeDef](./type_defs.md#getregexpatternsetresponsetypedef) 


```python
# get_regex_pattern_set method usage example with argument unpacking

kwargs: GetRegexPatternSetRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
}

parent.get_regex_pattern_set(**kwargs)
```

1. See [:material-code-braces: GetRegexPatternSetRequestTypeDef](./type_defs.md#getregexpatternsetrequesttypedef) 

### get\_rule\_group

Retrieves the specified <a>RuleGroup</a>.

Type annotations and code completion for `#!python session.create_client("wafv2").get_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/get_rule_group.html)

```python
# get_rule_group method definition

await def get_rule_group(
    self,
    *,
    Name: str = ...,
    Scope: ScopeType = ...,  # (1)
    Id: str = ...,
    ARN: str = ...,
) -> GetRuleGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetRuleGroupResponseTypeDef](./type_defs.md#getrulegroupresponsetypedef) 


```python
# get_rule_group method usage example with argument unpacking

kwargs: GetRuleGroupRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_rule_group(**kwargs)
```

1. See [:material-code-braces: GetRuleGroupRequestTypeDef](./type_defs.md#getrulegrouprequesttypedef) 

### get\_sampled\_requests

Gets detailed information about a specified number of requests--a sample--that
WAF randomly selects from among the first 5,000 requests that your Amazon Web
Services resource received during a time range that you choose.

Type annotations and code completion for `#!python session.create_client("wafv2").get_sampled_requests` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/get_sampled_requests.html)

```python
# get_sampled_requests method definition

await def get_sampled_requests(
    self,
    *,
    WebAclArn: str,
    RuleMetricName: str,
    Scope: ScopeType,  # (1)
    TimeWindow: TimeWindowUnionTypeDef,  # (2)
    MaxItems: int,
) -> GetSampledRequestsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: TimeWindowTypeDef](./type_defs.md#timewindowtypedef) [:material-code-braces: TimeWindowOutputTypeDef](./type_defs.md#timewindowoutputtypedef) 
3. See [:material-code-braces: GetSampledRequestsResponseTypeDef](./type_defs.md#getsampledrequestsresponsetypedef) 


```python
# get_sampled_requests method usage example with argument unpacking

kwargs: GetSampledRequestsRequestTypeDef = {  # (1)
    "WebAclArn": ...,
    "RuleMetricName": ...,
    "Scope": ...,
    "TimeWindow": ...,
    "MaxItems": ...,
}

parent.get_sampled_requests(**kwargs)
```

1. See [:material-code-braces: GetSampledRequestsRequestTypeDef](./type_defs.md#getsampledrequestsrequesttypedef) 

### get\_web\_acl

Retrieves the specified <a>WebACL</a>.

Type annotations and code completion for `#!python session.create_client("wafv2").get_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/get_web_acl.html)

```python
# get_web_acl method definition

await def get_web_acl(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
) -> GetWebACLResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetWebACLResponseTypeDef](./type_defs.md#getwebaclresponsetypedef) 


```python
# get_web_acl method usage example with argument unpacking

kwargs: GetWebACLRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
}

parent.get_web_acl(**kwargs)
```

1. See [:material-code-braces: GetWebACLRequestTypeDef](./type_defs.md#getwebaclrequesttypedef) 

### get\_web\_acl\_for\_resource

Retrieves the <a>WebACL</a> for the specified resource.

Type annotations and code completion for `#!python session.create_client("wafv2").get_web_acl_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/get_web_acl_for_resource.html)

```python
# get_web_acl_for_resource method definition

await def get_web_acl_for_resource(
    self,
    *,
    ResourceArn: str,
) -> GetWebACLForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWebACLForResourceResponseTypeDef](./type_defs.md#getwebaclforresourceresponsetypedef) 


```python
# get_web_acl_for_resource method usage example with argument unpacking

kwargs: GetWebACLForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_web_acl_for_resource(**kwargs)
```

1. See [:material-code-braces: GetWebACLForResourceRequestTypeDef](./type_defs.md#getwebaclforresourcerequesttypedef) 

### list\_api\_keys

Retrieves a list of the API keys that you've defined for the specified scope.

Type annotations and code completion for `#!python session.create_client("wafv2").list_api_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/list_api_keys.html)

```python
# list_api_keys method definition

await def list_api_keys(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListAPIKeysResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListAPIKeysResponseTypeDef](./type_defs.md#listapikeysresponsetypedef) 


```python
# list_api_keys method usage example with argument unpacking

kwargs: ListAPIKeysRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_api_keys(**kwargs)
```

1. See [:material-code-braces: ListAPIKeysRequestTypeDef](./type_defs.md#listapikeysrequesttypedef) 

### list\_available\_managed\_rule\_group\_versions

Returns a list of the available versions for the specified managed rule group.

Type annotations and code completion for `#!python session.create_client("wafv2").list_available_managed_rule_group_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/list_available_managed_rule_group_versions.html)

```python
# list_available_managed_rule_group_versions method definition

await def list_available_managed_rule_group_versions(
    self,
    *,
    VendorName: str,
    Name: str,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListAvailableManagedRuleGroupVersionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListAvailableManagedRuleGroupVersionsResponseTypeDef](./type_defs.md#listavailablemanagedrulegroupversionsresponsetypedef) 


```python
# list_available_managed_rule_group_versions method usage example with argument unpacking

kwargs: ListAvailableManagedRuleGroupVersionsRequestTypeDef = {  # (1)
    "VendorName": ...,
    "Name": ...,
    "Scope": ...,
}

parent.list_available_managed_rule_group_versions(**kwargs)
```

1. See [:material-code-braces: ListAvailableManagedRuleGroupVersionsRequestTypeDef](./type_defs.md#listavailablemanagedrulegroupversionsrequesttypedef) 

### list\_available\_managed\_rule\_groups

Retrieves an array of managed rule groups that are available for you to use.

Type annotations and code completion for `#!python session.create_client("wafv2").list_available_managed_rule_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/list_available_managed_rule_groups.html)

```python
# list_available_managed_rule_groups method definition

await def list_available_managed_rule_groups(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListAvailableManagedRuleGroupsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListAvailableManagedRuleGroupsResponseTypeDef](./type_defs.md#listavailablemanagedrulegroupsresponsetypedef) 


```python
# list_available_managed_rule_groups method usage example with argument unpacking

kwargs: ListAvailableManagedRuleGroupsRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_available_managed_rule_groups(**kwargs)
```

1. See [:material-code-braces: ListAvailableManagedRuleGroupsRequestTypeDef](./type_defs.md#listavailablemanagedrulegroupsrequesttypedef) 

### list\_ip\_sets

Retrieves an array of <a>IPSetSummary</a> objects for the IP sets that you
manage.

Type annotations and code completion for `#!python session.create_client("wafv2").list_ip_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/list_ip_sets.html)

```python
# list_ip_sets method definition

await def list_ip_sets(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListIPSetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef) 


```python
# list_ip_sets method usage example with argument unpacking

kwargs: ListIPSetsRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_ip_sets(**kwargs)
```

1. See [:material-code-braces: ListIPSetsRequestTypeDef](./type_defs.md#listipsetsrequesttypedef) 

### list\_logging\_configurations

Retrieves an array of your <a>LoggingConfiguration</a> objects.

Type annotations and code completion for `#!python session.create_client("wafv2").list_logging_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/list_logging_configurations.html)

```python
# list_logging_configurations method definition

await def list_logging_configurations(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
    LogScope: LogScopeType = ...,  # (2)
) -> ListLoggingConfigurationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-brackets: LogScopeType](./literals.md#logscopetype) 
3. See [:material-code-braces: ListLoggingConfigurationsResponseTypeDef](./type_defs.md#listloggingconfigurationsresponsetypedef) 


```python
# list_logging_configurations method usage example with argument unpacking

kwargs: ListLoggingConfigurationsRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_logging_configurations(**kwargs)
```

1. See [:material-code-braces: ListLoggingConfigurationsRequestTypeDef](./type_defs.md#listloggingconfigurationsrequesttypedef) 

### list\_managed\_rule\_sets

Retrieves the managed rule sets that you own.

Type annotations and code completion for `#!python session.create_client("wafv2").list_managed_rule_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/list_managed_rule_sets.html)

```python
# list_managed_rule_sets method definition

await def list_managed_rule_sets(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListManagedRuleSetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListManagedRuleSetsResponseTypeDef](./type_defs.md#listmanagedrulesetsresponsetypedef) 


```python
# list_managed_rule_sets method usage example with argument unpacking

kwargs: ListManagedRuleSetsRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_managed_rule_sets(**kwargs)
```

1. See [:material-code-braces: ListManagedRuleSetsRequestTypeDef](./type_defs.md#listmanagedrulesetsrequesttypedef) 

### list\_mobile\_sdk\_releases

Retrieves a list of the available releases for the mobile SDK and the specified
device platform.

Type annotations and code completion for `#!python session.create_client("wafv2").list_mobile_sdk_releases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/list_mobile_sdk_releases.html)

```python
# list_mobile_sdk_releases method definition

await def list_mobile_sdk_releases(
    self,
    *,
    Platform: PlatformType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListMobileSdkReleasesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: ListMobileSdkReleasesResponseTypeDef](./type_defs.md#listmobilesdkreleasesresponsetypedef) 


```python
# list_mobile_sdk_releases method usage example with argument unpacking

kwargs: ListMobileSdkReleasesRequestTypeDef = {  # (1)
    "Platform": ...,
}

parent.list_mobile_sdk_releases(**kwargs)
```

1. See [:material-code-braces: ListMobileSdkReleasesRequestTypeDef](./type_defs.md#listmobilesdkreleasesrequesttypedef) 

### list\_regex\_pattern\_sets

Retrieves an array of <a>RegexPatternSetSummary</a> objects for the regex
pattern sets that you manage.

Type annotations and code completion for `#!python session.create_client("wafv2").list_regex_pattern_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/list_regex_pattern_sets.html)

```python
# list_regex_pattern_sets method definition

await def list_regex_pattern_sets(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListRegexPatternSetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListRegexPatternSetsResponseTypeDef](./type_defs.md#listregexpatternsetsresponsetypedef) 


```python
# list_regex_pattern_sets method usage example with argument unpacking

kwargs: ListRegexPatternSetsRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_regex_pattern_sets(**kwargs)
```

1. See [:material-code-braces: ListRegexPatternSetsRequestTypeDef](./type_defs.md#listregexpatternsetsrequesttypedef) 

### list\_resources\_for\_web\_acl

Retrieves an array of the Amazon Resource Names (ARNs) for the resources that
are associated with the specified web ACL.

Type annotations and code completion for `#!python session.create_client("wafv2").list_resources_for_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/list_resources_for_web_acl.html)

```python
# list_resources_for_web_acl method definition

await def list_resources_for_web_acl(
    self,
    *,
    WebACLArn: str,
    ResourceType: ResourceTypeType = ...,  # (1)
) -> ListResourcesForWebACLResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ListResourcesForWebACLResponseTypeDef](./type_defs.md#listresourcesforwebaclresponsetypedef) 


```python
# list_resources_for_web_acl method usage example with argument unpacking

kwargs: ListResourcesForWebACLRequestTypeDef = {  # (1)
    "WebACLArn": ...,
}

parent.list_resources_for_web_acl(**kwargs)
```

1. See [:material-code-braces: ListResourcesForWebACLRequestTypeDef](./type_defs.md#listresourcesforwebaclrequesttypedef) 

### list\_rule\_groups

Retrieves an array of <a>RuleGroupSummary</a> objects for the rule groups that
you manage.

Type annotations and code completion for `#!python session.create_client("wafv2").list_rule_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/list_rule_groups.html)

```python
# list_rule_groups method definition

await def list_rule_groups(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListRuleGroupsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListRuleGroupsResponseTypeDef](./type_defs.md#listrulegroupsresponsetypedef) 


```python
# list_rule_groups method usage example with argument unpacking

kwargs: ListRuleGroupsRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_rule_groups(**kwargs)
```

1. See [:material-code-braces: ListRuleGroupsRequestTypeDef](./type_defs.md#listrulegroupsrequesttypedef) 

### list\_tags\_for\_resource

Retrieves the <a>TagInfoForResource</a> for the specified resource.

Type annotations and code completion for `#!python session.create_client("wafv2").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### list\_web\_acls

Retrieves an array of <a>WebACLSummary</a> objects for the web ACLs that you
manage.

Type annotations and code completion for `#!python session.create_client("wafv2").list_web_acls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/list_web_acls.html)

```python
# list_web_acls method definition

await def list_web_acls(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListWebACLsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListWebACLsResponseTypeDef](./type_defs.md#listwebaclsresponsetypedef) 


```python
# list_web_acls method usage example with argument unpacking

kwargs: ListWebACLsRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_web_acls(**kwargs)
```

1. See [:material-code-braces: ListWebACLsRequestTypeDef](./type_defs.md#listwebaclsrequesttypedef) 

### put\_logging\_configuration

Enables the specified <a>LoggingConfiguration</a>, to start logging from a web
ACL, according to the configuration provided.

Type annotations and code completion for `#!python session.create_client("wafv2").put_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/put_logging_configuration.html)

```python
# put_logging_configuration method definition

await def put_logging_configuration(
    self,
    *,
    LoggingConfiguration: LoggingConfigurationUnionTypeDef,  # (1)
) -> PutLoggingConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) [:material-code-braces: LoggingConfigurationOutputTypeDef](./type_defs.md#loggingconfigurationoutputtypedef) 
2. See [:material-code-braces: PutLoggingConfigurationResponseTypeDef](./type_defs.md#putloggingconfigurationresponsetypedef) 


```python
# put_logging_configuration method usage example with argument unpacking

kwargs: PutLoggingConfigurationRequestTypeDef = {  # (1)
    "LoggingConfiguration": ...,
}

parent.put_logging_configuration(**kwargs)
```

1. See [:material-code-braces: PutLoggingConfigurationRequestTypeDef](./type_defs.md#putloggingconfigurationrequesttypedef) 

### put\_managed\_rule\_set\_versions

Defines the versions of your managed rule set that you are offering to the
customers.

Type annotations and code completion for `#!python session.create_client("wafv2").put_managed_rule_set_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/put_managed_rule_set_versions.html)

```python
# put_managed_rule_set_versions method definition

await def put_managed_rule_set_versions(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
    RecommendedVersion: str = ...,
    VersionsToPublish: Mapping[str, VersionToPublishTypeDef] = ...,  # (2)
) -> PutManagedRuleSetVersionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: VersionToPublishTypeDef](./type_defs.md#versiontopublishtypedef) 
3. See [:material-code-braces: PutManagedRuleSetVersionsResponseTypeDef](./type_defs.md#putmanagedrulesetversionsresponsetypedef) 


```python
# put_managed_rule_set_versions method usage example with argument unpacking

kwargs: PutManagedRuleSetVersionsRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "LockToken": ...,
}

parent.put_managed_rule_set_versions(**kwargs)
```

1. See [:material-code-braces: PutManagedRuleSetVersionsRequestTypeDef](./type_defs.md#putmanagedrulesetversionsrequesttypedef) 

### put\_permission\_policy

Use this to share a rule group with other accounts.

Type annotations and code completion for `#!python session.create_client("wafv2").put_permission_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/put_permission_policy.html)

```python
# put_permission_policy method definition

await def put_permission_policy(
    self,
    *,
    ResourceArn: str,
    Policy: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_permission_policy method usage example with argument unpacking

kwargs: PutPermissionPolicyRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Policy": ...,
}

parent.put_permission_policy(**kwargs)
```

1. See [:material-code-braces: PutPermissionPolicyRequestTypeDef](./type_defs.md#putpermissionpolicyrequesttypedef) 

### tag\_resource

Associates tags with the specified Amazon Web Services resource.

Type annotations and code completion for `#!python session.create_client("wafv2").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Disassociates tags from an Amazon Web Services resource.

Type annotations and code completion for `#!python session.create_client("wafv2").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_ip\_set

Updates the specified <a>IPSet</a>.

Type annotations and code completion for `#!python session.create_client("wafv2").update_ip_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/update_ip_set.html)

```python
# update_ip_set method definition

await def update_ip_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    Addresses: Sequence[str],
    LockToken: str,
    Description: str = ...,
) -> UpdateIPSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: UpdateIPSetResponseTypeDef](./type_defs.md#updateipsetresponsetypedef) 


```python
# update_ip_set method usage example with argument unpacking

kwargs: UpdateIPSetRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "Addresses": ...,
    "LockToken": ...,
}

parent.update_ip_set(**kwargs)
```

1. See [:material-code-braces: UpdateIPSetRequestTypeDef](./type_defs.md#updateipsetrequesttypedef) 

### update\_managed\_rule\_set\_version\_expiry\_date

Updates the expiration information for your managed rule set.

Type annotations and code completion for `#!python session.create_client("wafv2").update_managed_rule_set_version_expiry_date` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/update_managed_rule_set_version_expiry_date.html)

```python
# update_managed_rule_set_version_expiry_date method definition

await def update_managed_rule_set_version_expiry_date(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
    VersionToExpire: str,
    ExpiryTimestamp: TimestampTypeDef,
) -> UpdateManagedRuleSetVersionExpiryDateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: UpdateManagedRuleSetVersionExpiryDateResponseTypeDef](./type_defs.md#updatemanagedrulesetversionexpirydateresponsetypedef) 


```python
# update_managed_rule_set_version_expiry_date method usage example with argument unpacking

kwargs: UpdateManagedRuleSetVersionExpiryDateRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "LockToken": ...,
    "VersionToExpire": ...,
    "ExpiryTimestamp": ...,
}

parent.update_managed_rule_set_version_expiry_date(**kwargs)
```

1. See [:material-code-braces: UpdateManagedRuleSetVersionExpiryDateRequestTypeDef](./type_defs.md#updatemanagedrulesetversionexpirydaterequesttypedef) 

### update\_regex\_pattern\_set

Updates the specified <a>RegexPatternSet</a>.

Type annotations and code completion for `#!python session.create_client("wafv2").update_regex_pattern_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/update_regex_pattern_set.html)

```python
# update_regex_pattern_set method definition

await def update_regex_pattern_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    RegularExpressionList: Sequence[RegexTypeDef],  # (2)
    LockToken: str,
    Description: str = ...,
) -> UpdateRegexPatternSetResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: RegexTypeDef](./type_defs.md#regextypedef) 
3. See [:material-code-braces: UpdateRegexPatternSetResponseTypeDef](./type_defs.md#updateregexpatternsetresponsetypedef) 


```python
# update_regex_pattern_set method usage example with argument unpacking

kwargs: UpdateRegexPatternSetRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "RegularExpressionList": ...,
    "LockToken": ...,
}

parent.update_regex_pattern_set(**kwargs)
```

1. See [:material-code-braces: UpdateRegexPatternSetRequestTypeDef](./type_defs.md#updateregexpatternsetrequesttypedef) 

### update\_rule\_group

Updates the specified <a>RuleGroup</a>.

Type annotations and code completion for `#!python session.create_client("wafv2").update_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/update_rule_group.html)

```python
# update_rule_group method definition

await def update_rule_group(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    VisibilityConfig: VisibilityConfigTypeDef,  # (2)
    LockToken: str,
    Description: str = ...,
    Rules: Sequence[RuleUnionTypeDef] = ...,  # (3)
    CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,  # (4)
) -> UpdateRuleGroupResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
3. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
4. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
5. See [:material-code-braces: UpdateRuleGroupResponseTypeDef](./type_defs.md#updaterulegroupresponsetypedef) 


```python
# update_rule_group method usage example with argument unpacking

kwargs: UpdateRuleGroupRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "VisibilityConfig": ...,
    "LockToken": ...,
}

parent.update_rule_group(**kwargs)
```

1. See [:material-code-braces: UpdateRuleGroupRequestTypeDef](./type_defs.md#updaterulegrouprequesttypedef) 

### update\_web\_acl

Updates the specified <a>WebACL</a>.

Type annotations and code completion for `#!python session.create_client("wafv2").update_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2/client/update_web_acl.html)

```python
# update_web_acl method definition

await def update_web_acl(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    DefaultAction: DefaultActionUnionTypeDef,  # (2)
    VisibilityConfig: VisibilityConfigTypeDef,  # (3)
    LockToken: str,
    Description: str = ...,
    Rules: Sequence[RuleUnionTypeDef] = ...,  # (4)
    DataProtectionConfig: DataProtectionConfigUnionTypeDef = ...,  # (5)
    CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,  # (6)
    CaptchaConfig: CaptchaConfigTypeDef = ...,  # (7)
    ChallengeConfig: ChallengeConfigTypeDef = ...,  # (8)
    TokenDomains: Sequence[str] = ...,
    AssociationConfig: AssociationConfigUnionTypeDef = ...,  # (9)
) -> UpdateWebACLResponseTypeDef:  # (10)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DefaultActionTypeDef](./type_defs.md#defaultactiontypedef) [:material-code-braces: DefaultActionOutputTypeDef](./type_defs.md#defaultactionoutputtypedef) 
3. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
4. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
5. See [:material-code-braces: DataProtectionConfigTypeDef](./type_defs.md#dataprotectionconfigtypedef) [:material-code-braces: DataProtectionConfigOutputTypeDef](./type_defs.md#dataprotectionconfigoutputtypedef) 
6. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
7. See [:material-code-braces: CaptchaConfigTypeDef](./type_defs.md#captchaconfigtypedef) 
8. See [:material-code-braces: ChallengeConfigTypeDef](./type_defs.md#challengeconfigtypedef) 
9. See [:material-code-braces: AssociationConfigTypeDef](./type_defs.md#associationconfigtypedef) [:material-code-braces: AssociationConfigOutputTypeDef](./type_defs.md#associationconfigoutputtypedef) 
10. See [:material-code-braces: UpdateWebACLResponseTypeDef](./type_defs.md#updatewebaclresponsetypedef) 


```python
# update_web_acl method usage example with argument unpacking

kwargs: UpdateWebACLRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "DefaultAction": ...,
    "VisibilityConfig": ...,
    "LockToken": ...,
}

parent.update_web_acl(**kwargs)
```

1. See [:material-code-braces: UpdateWebACLRequestTypeDef](./type_defs.md#updatewebaclrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("wafv2").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("wafv2").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```





