# WAFRegionalClient

> [Index](../README.md) > [WAFRegional](./README.md) > WAFRegionalClient

!!! note ""

    Auto-generated documentation for [WAFRegional](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
    type annotations stubs module [types-aiobotocore-waf-regional](https://pypi.org/project/types-aiobotocore-waf-regional/).

## WAFRegionalClient

Type annotations and code completion for `#!python session.create_client("waf-regional")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client)

```python
# WAFRegionalClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_waf_regional.client import WAFRegionalClient

session = get_session()
async with session.create_client("waf-regional") as client:
    client: WAFRegionalClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("waf-regional").exceptions` structure.

```python
# WAFRegionalClient.exceptions usage example

async with session.create_client("waf-regional") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.WAFBadRequestException,
        client.WAFDisallowedNameException,
        client.WAFEntityMigrationException,
        client.WAFInternalErrorException,
        client.WAFInvalidAccountException,
        client.WAFInvalidOperationException,
        client.WAFInvalidParameterException,
        client.WAFInvalidPermissionPolicyException,
        client.WAFInvalidRegexPatternException,
        client.WAFLimitsExceededException,
        client.WAFNonEmptyEntityException,
        client.WAFNonexistentContainerException,
        client.WAFNonexistentItemException,
        client.WAFReferencedItemException,
        client.WAFServiceLinkedRoleErrorException,
        client.WAFStaleDataException,
        client.WAFSubscriptionNotFoundException,
        client.WAFTagOperationException,
        client.WAFTagOperationInternalErrorException,
        client.WAFUnavailableEntityException,
    ) as e:
        print(e)
```

```python
# WAFRegionalClient usage type checking example

from types_aiobotocore_waf_regional.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### associate\_web\_acl

.

Type annotations and code completion for `#!python session.create_client("waf-regional").associate_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.associate_web_acl)

```python
# associate_web_acl method definition

await def associate_web_acl(
    self,
    *,
    WebACLId: str,
    ResourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_web_acl method usage example with argument unpacking

kwargs: AssociateWebACLRequestRequestTypeDef = {  # (1)
    "WebACLId": ...,
    "ResourceArn": ...,
}

parent.associate_web_acl(**kwargs)
```

1. See [:material-code-braces: AssociateWebACLRequestRequestTypeDef](./type_defs.md#associatewebaclrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("waf-regional").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("waf-regional").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_byte\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").create_byte_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.create_byte_match_set)

```python
# create_byte_match_set method definition

await def create_byte_match_set(
    self,
    *,
    Name: str,
    ChangeToken: str,
) -> CreateByteMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateByteMatchSetResponseTypeDef](./type_defs.md#createbytematchsetresponsetypedef) 


```python
# create_byte_match_set method usage example with argument unpacking

kwargs: CreateByteMatchSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ChangeToken": ...,
}

parent.create_byte_match_set(**kwargs)
```

1. See [:material-code-braces: CreateByteMatchSetRequestRequestTypeDef](./type_defs.md#createbytematchsetrequestrequesttypedef) 

### create\_geo\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").create_geo_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.create_geo_match_set)

```python
# create_geo_match_set method definition

await def create_geo_match_set(
    self,
    *,
    Name: str,
    ChangeToken: str,
) -> CreateGeoMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateGeoMatchSetResponseTypeDef](./type_defs.md#creategeomatchsetresponsetypedef) 


```python
# create_geo_match_set method usage example with argument unpacking

kwargs: CreateGeoMatchSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ChangeToken": ...,
}

parent.create_geo_match_set(**kwargs)
```

1. See [:material-code-braces: CreateGeoMatchSetRequestRequestTypeDef](./type_defs.md#creategeomatchsetrequestrequesttypedef) 

### create\_ip\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").create_ip_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.create_ip_set)

```python
# create_ip_set method definition

await def create_ip_set(
    self,
    *,
    Name: str,
    ChangeToken: str,
) -> CreateIPSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateIPSetResponseTypeDef](./type_defs.md#createipsetresponsetypedef) 


```python
# create_ip_set method usage example with argument unpacking

kwargs: CreateIPSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ChangeToken": ...,
}

parent.create_ip_set(**kwargs)
```

1. See [:material-code-braces: CreateIPSetRequestRequestTypeDef](./type_defs.md#createipsetrequestrequesttypedef) 

### create\_rate\_based\_rule

.

Type annotations and code completion for `#!python session.create_client("waf-regional").create_rate_based_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.create_rate_based_rule)

```python
# create_rate_based_rule method definition

await def create_rate_based_rule(
    self,
    *,
    Name: str,
    MetricName: str,
    RateKey: RateKeyType,  # (1)
    RateLimit: int,
    ChangeToken: str,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateRateBasedRuleResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RateKeyType](./literals.md#ratekeytype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateRateBasedRuleResponseTypeDef](./type_defs.md#createratebasedruleresponsetypedef) 


```python
# create_rate_based_rule method usage example with argument unpacking

kwargs: CreateRateBasedRuleRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "MetricName": ...,
    "RateKey": ...,
    "RateLimit": ...,
    "ChangeToken": ...,
}

parent.create_rate_based_rule(**kwargs)
```

1. See [:material-code-braces: CreateRateBasedRuleRequestRequestTypeDef](./type_defs.md#createratebasedrulerequestrequesttypedef) 

### create\_regex\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").create_regex_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.create_regex_match_set)

```python
# create_regex_match_set method definition

await def create_regex_match_set(
    self,
    *,
    Name: str,
    ChangeToken: str,
) -> CreateRegexMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateRegexMatchSetResponseTypeDef](./type_defs.md#createregexmatchsetresponsetypedef) 


```python
# create_regex_match_set method usage example with argument unpacking

kwargs: CreateRegexMatchSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ChangeToken": ...,
}

parent.create_regex_match_set(**kwargs)
```

1. See [:material-code-braces: CreateRegexMatchSetRequestRequestTypeDef](./type_defs.md#createregexmatchsetrequestrequesttypedef) 

### create\_regex\_pattern\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").create_regex_pattern_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.create_regex_pattern_set)

```python
# create_regex_pattern_set method definition

await def create_regex_pattern_set(
    self,
    *,
    Name: str,
    ChangeToken: str,
) -> CreateRegexPatternSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateRegexPatternSetResponseTypeDef](./type_defs.md#createregexpatternsetresponsetypedef) 


```python
# create_regex_pattern_set method usage example with argument unpacking

kwargs: CreateRegexPatternSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ChangeToken": ...,
}

parent.create_regex_pattern_set(**kwargs)
```

1. See [:material-code-braces: CreateRegexPatternSetRequestRequestTypeDef](./type_defs.md#createregexpatternsetrequestrequesttypedef) 

### create\_rule

.

Type annotations and code completion for `#!python session.create_client("waf-regional").create_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.create_rule)

```python
# create_rule method definition

await def create_rule(
    self,
    *,
    Name: str,
    MetricName: str,
    ChangeToken: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateRuleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateRuleResponseTypeDef](./type_defs.md#createruleresponsetypedef) 


```python
# create_rule method usage example with argument unpacking

kwargs: CreateRuleRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "MetricName": ...,
    "ChangeToken": ...,
}

parent.create_rule(**kwargs)
```

1. See [:material-code-braces: CreateRuleRequestRequestTypeDef](./type_defs.md#createrulerequestrequesttypedef) 

### create\_rule\_group

.

Type annotations and code completion for `#!python session.create_client("waf-regional").create_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.create_rule_group)

```python
# create_rule_group method definition

await def create_rule_group(
    self,
    *,
    Name: str,
    MetricName: str,
    ChangeToken: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateRuleGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateRuleGroupResponseTypeDef](./type_defs.md#createrulegroupresponsetypedef) 


```python
# create_rule_group method usage example with argument unpacking

kwargs: CreateRuleGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "MetricName": ...,
    "ChangeToken": ...,
}

parent.create_rule_group(**kwargs)
```

1. See [:material-code-braces: CreateRuleGroupRequestRequestTypeDef](./type_defs.md#createrulegrouprequestrequesttypedef) 

### create\_size\_constraint\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").create_size_constraint_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.create_size_constraint_set)

```python
# create_size_constraint_set method definition

await def create_size_constraint_set(
    self,
    *,
    Name: str,
    ChangeToken: str,
) -> CreateSizeConstraintSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSizeConstraintSetResponseTypeDef](./type_defs.md#createsizeconstraintsetresponsetypedef) 


```python
# create_size_constraint_set method usage example with argument unpacking

kwargs: CreateSizeConstraintSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ChangeToken": ...,
}

parent.create_size_constraint_set(**kwargs)
```

1. See [:material-code-braces: CreateSizeConstraintSetRequestRequestTypeDef](./type_defs.md#createsizeconstraintsetrequestrequesttypedef) 

### create\_sql\_injection\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").create_sql_injection_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.create_sql_injection_match_set)

```python
# create_sql_injection_match_set method definition

await def create_sql_injection_match_set(
    self,
    *,
    Name: str,
    ChangeToken: str,
) -> CreateSqlInjectionMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSqlInjectionMatchSetResponseTypeDef](./type_defs.md#createsqlinjectionmatchsetresponsetypedef) 


```python
# create_sql_injection_match_set method usage example with argument unpacking

kwargs: CreateSqlInjectionMatchSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ChangeToken": ...,
}

parent.create_sql_injection_match_set(**kwargs)
```

1. See [:material-code-braces: CreateSqlInjectionMatchSetRequestRequestTypeDef](./type_defs.md#createsqlinjectionmatchsetrequestrequesttypedef) 

### create\_web\_acl

.

Type annotations and code completion for `#!python session.create_client("waf-regional").create_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.create_web_acl)

```python
# create_web_acl method definition

await def create_web_acl(
    self,
    *,
    Name: str,
    MetricName: str,
    DefaultAction: WafActionTypeDef,  # (1)
    ChangeToken: str,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateWebACLResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: WafActionTypeDef](./type_defs.md#wafactiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateWebACLResponseTypeDef](./type_defs.md#createwebaclresponsetypedef) 


```python
# create_web_acl method usage example with argument unpacking

kwargs: CreateWebACLRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "MetricName": ...,
    "DefaultAction": ...,
    "ChangeToken": ...,
}

parent.create_web_acl(**kwargs)
```

1. See [:material-code-braces: CreateWebACLRequestRequestTypeDef](./type_defs.md#createwebaclrequestrequesttypedef) 

### create\_web\_acl\_migration\_stack

Creates an AWS CloudFormation WAFV2 template for the specified web ACL in the
specified Amazon S3
bucket.

Type annotations and code completion for `#!python session.create_client("waf-regional").create_web_acl_migration_stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.create_web_acl_migration_stack)

```python
# create_web_acl_migration_stack method definition

await def create_web_acl_migration_stack(
    self,
    *,
    WebACLId: str,
    S3BucketName: str,
    IgnoreUnsupportedType: bool,
) -> CreateWebACLMigrationStackResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateWebACLMigrationStackResponseTypeDef](./type_defs.md#createwebaclmigrationstackresponsetypedef) 


```python
# create_web_acl_migration_stack method usage example with argument unpacking

kwargs: CreateWebACLMigrationStackRequestRequestTypeDef = {  # (1)
    "WebACLId": ...,
    "S3BucketName": ...,
    "IgnoreUnsupportedType": ...,
}

parent.create_web_acl_migration_stack(**kwargs)
```

1. See [:material-code-braces: CreateWebACLMigrationStackRequestRequestTypeDef](./type_defs.md#createwebaclmigrationstackrequestrequesttypedef) 

### create\_xss\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").create_xss_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.create_xss_match_set)

```python
# create_xss_match_set method definition

await def create_xss_match_set(
    self,
    *,
    Name: str,
    ChangeToken: str,
) -> CreateXssMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateXssMatchSetResponseTypeDef](./type_defs.md#createxssmatchsetresponsetypedef) 


```python
# create_xss_match_set method usage example with argument unpacking

kwargs: CreateXssMatchSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ChangeToken": ...,
}

parent.create_xss_match_set(**kwargs)
```

1. See [:material-code-braces: CreateXssMatchSetRequestRequestTypeDef](./type_defs.md#createxssmatchsetrequestrequesttypedef) 

### delete\_byte\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_byte_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_byte_match_set)

```python
# delete_byte_match_set method definition

await def delete_byte_match_set(
    self,
    *,
    ByteMatchSetId: str,
    ChangeToken: str,
) -> DeleteByteMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteByteMatchSetResponseTypeDef](./type_defs.md#deletebytematchsetresponsetypedef) 


```python
# delete_byte_match_set method usage example with argument unpacking

kwargs: DeleteByteMatchSetRequestRequestTypeDef = {  # (1)
    "ByteMatchSetId": ...,
    "ChangeToken": ...,
}

parent.delete_byte_match_set(**kwargs)
```

1. See [:material-code-braces: DeleteByteMatchSetRequestRequestTypeDef](./type_defs.md#deletebytematchsetrequestrequesttypedef) 

### delete\_geo\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_geo_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_geo_match_set)

```python
# delete_geo_match_set method definition

await def delete_geo_match_set(
    self,
    *,
    GeoMatchSetId: str,
    ChangeToken: str,
) -> DeleteGeoMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteGeoMatchSetResponseTypeDef](./type_defs.md#deletegeomatchsetresponsetypedef) 


```python
# delete_geo_match_set method usage example with argument unpacking

kwargs: DeleteGeoMatchSetRequestRequestTypeDef = {  # (1)
    "GeoMatchSetId": ...,
    "ChangeToken": ...,
}

parent.delete_geo_match_set(**kwargs)
```

1. See [:material-code-braces: DeleteGeoMatchSetRequestRequestTypeDef](./type_defs.md#deletegeomatchsetrequestrequesttypedef) 

### delete\_ip\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_ip_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_ip_set)

```python
# delete_ip_set method definition

await def delete_ip_set(
    self,
    *,
    IPSetId: str,
    ChangeToken: str,
) -> DeleteIPSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteIPSetResponseTypeDef](./type_defs.md#deleteipsetresponsetypedef) 


```python
# delete_ip_set method usage example with argument unpacking

kwargs: DeleteIPSetRequestRequestTypeDef = {  # (1)
    "IPSetId": ...,
    "ChangeToken": ...,
}

parent.delete_ip_set(**kwargs)
```

1. See [:material-code-braces: DeleteIPSetRequestRequestTypeDef](./type_defs.md#deleteipsetrequestrequesttypedef) 

### delete\_logging\_configuration

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_logging_configuration)

```python
# delete_logging_configuration method definition

await def delete_logging_configuration(
    self,
    *,
    ResourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_logging_configuration method usage example with argument unpacking

kwargs: DeleteLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.delete_logging_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteLoggingConfigurationRequestRequestTypeDef](./type_defs.md#deleteloggingconfigurationrequestrequesttypedef) 

### delete\_permission\_policy

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_permission_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_permission_policy)

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

kwargs: DeletePermissionPolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.delete_permission_policy(**kwargs)
```

1. See [:material-code-braces: DeletePermissionPolicyRequestRequestTypeDef](./type_defs.md#deletepermissionpolicyrequestrequesttypedef) 

### delete\_rate\_based\_rule

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_rate_based_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_rate_based_rule)

```python
# delete_rate_based_rule method definition

await def delete_rate_based_rule(
    self,
    *,
    RuleId: str,
    ChangeToken: str,
) -> DeleteRateBasedRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteRateBasedRuleResponseTypeDef](./type_defs.md#deleteratebasedruleresponsetypedef) 


```python
# delete_rate_based_rule method usage example with argument unpacking

kwargs: DeleteRateBasedRuleRequestRequestTypeDef = {  # (1)
    "RuleId": ...,
    "ChangeToken": ...,
}

parent.delete_rate_based_rule(**kwargs)
```

1. See [:material-code-braces: DeleteRateBasedRuleRequestRequestTypeDef](./type_defs.md#deleteratebasedrulerequestrequesttypedef) 

### delete\_regex\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_regex_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_regex_match_set)

```python
# delete_regex_match_set method definition

await def delete_regex_match_set(
    self,
    *,
    RegexMatchSetId: str,
    ChangeToken: str,
) -> DeleteRegexMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteRegexMatchSetResponseTypeDef](./type_defs.md#deleteregexmatchsetresponsetypedef) 


```python
# delete_regex_match_set method usage example with argument unpacking

kwargs: DeleteRegexMatchSetRequestRequestTypeDef = {  # (1)
    "RegexMatchSetId": ...,
    "ChangeToken": ...,
}

parent.delete_regex_match_set(**kwargs)
```

1. See [:material-code-braces: DeleteRegexMatchSetRequestRequestTypeDef](./type_defs.md#deleteregexmatchsetrequestrequesttypedef) 

### delete\_regex\_pattern\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_regex_pattern_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_regex_pattern_set)

```python
# delete_regex_pattern_set method definition

await def delete_regex_pattern_set(
    self,
    *,
    RegexPatternSetId: str,
    ChangeToken: str,
) -> DeleteRegexPatternSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteRegexPatternSetResponseTypeDef](./type_defs.md#deleteregexpatternsetresponsetypedef) 


```python
# delete_regex_pattern_set method usage example with argument unpacking

kwargs: DeleteRegexPatternSetRequestRequestTypeDef = {  # (1)
    "RegexPatternSetId": ...,
    "ChangeToken": ...,
}

parent.delete_regex_pattern_set(**kwargs)
```

1. See [:material-code-braces: DeleteRegexPatternSetRequestRequestTypeDef](./type_defs.md#deleteregexpatternsetrequestrequesttypedef) 

### delete\_rule

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_rule)

```python
# delete_rule method definition

await def delete_rule(
    self,
    *,
    RuleId: str,
    ChangeToken: str,
) -> DeleteRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteRuleResponseTypeDef](./type_defs.md#deleteruleresponsetypedef) 


```python
# delete_rule method usage example with argument unpacking

kwargs: DeleteRuleRequestRequestTypeDef = {  # (1)
    "RuleId": ...,
    "ChangeToken": ...,
}

parent.delete_rule(**kwargs)
```

1. See [:material-code-braces: DeleteRuleRequestRequestTypeDef](./type_defs.md#deleterulerequestrequesttypedef) 

### delete\_rule\_group

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_rule_group)

```python
# delete_rule_group method definition

await def delete_rule_group(
    self,
    *,
    RuleGroupId: str,
    ChangeToken: str,
) -> DeleteRuleGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteRuleGroupResponseTypeDef](./type_defs.md#deleterulegroupresponsetypedef) 


```python
# delete_rule_group method usage example with argument unpacking

kwargs: DeleteRuleGroupRequestRequestTypeDef = {  # (1)
    "RuleGroupId": ...,
    "ChangeToken": ...,
}

parent.delete_rule_group(**kwargs)
```

1. See [:material-code-braces: DeleteRuleGroupRequestRequestTypeDef](./type_defs.md#deleterulegrouprequestrequesttypedef) 

### delete\_size\_constraint\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_size_constraint_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_size_constraint_set)

```python
# delete_size_constraint_set method definition

await def delete_size_constraint_set(
    self,
    *,
    SizeConstraintSetId: str,
    ChangeToken: str,
) -> DeleteSizeConstraintSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSizeConstraintSetResponseTypeDef](./type_defs.md#deletesizeconstraintsetresponsetypedef) 


```python
# delete_size_constraint_set method usage example with argument unpacking

kwargs: DeleteSizeConstraintSetRequestRequestTypeDef = {  # (1)
    "SizeConstraintSetId": ...,
    "ChangeToken": ...,
}

parent.delete_size_constraint_set(**kwargs)
```

1. See [:material-code-braces: DeleteSizeConstraintSetRequestRequestTypeDef](./type_defs.md#deletesizeconstraintsetrequestrequesttypedef) 

### delete\_sql\_injection\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_sql_injection_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_sql_injection_match_set)

```python
# delete_sql_injection_match_set method definition

await def delete_sql_injection_match_set(
    self,
    *,
    SqlInjectionMatchSetId: str,
    ChangeToken: str,
) -> DeleteSqlInjectionMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSqlInjectionMatchSetResponseTypeDef](./type_defs.md#deletesqlinjectionmatchsetresponsetypedef) 


```python
# delete_sql_injection_match_set method usage example with argument unpacking

kwargs: DeleteSqlInjectionMatchSetRequestRequestTypeDef = {  # (1)
    "SqlInjectionMatchSetId": ...,
    "ChangeToken": ...,
}

parent.delete_sql_injection_match_set(**kwargs)
```

1. See [:material-code-braces: DeleteSqlInjectionMatchSetRequestRequestTypeDef](./type_defs.md#deletesqlinjectionmatchsetrequestrequesttypedef) 

### delete\_web\_acl

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_web_acl)

```python
# delete_web_acl method definition

await def delete_web_acl(
    self,
    *,
    WebACLId: str,
    ChangeToken: str,
) -> DeleteWebACLResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteWebACLResponseTypeDef](./type_defs.md#deletewebaclresponsetypedef) 


```python
# delete_web_acl method usage example with argument unpacking

kwargs: DeleteWebACLRequestRequestTypeDef = {  # (1)
    "WebACLId": ...,
    "ChangeToken": ...,
}

parent.delete_web_acl(**kwargs)
```

1. See [:material-code-braces: DeleteWebACLRequestRequestTypeDef](./type_defs.md#deletewebaclrequestrequesttypedef) 

### delete\_xss\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").delete_xss_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.delete_xss_match_set)

```python
# delete_xss_match_set method definition

await def delete_xss_match_set(
    self,
    *,
    XssMatchSetId: str,
    ChangeToken: str,
) -> DeleteXssMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteXssMatchSetResponseTypeDef](./type_defs.md#deletexssmatchsetresponsetypedef) 


```python
# delete_xss_match_set method usage example with argument unpacking

kwargs: DeleteXssMatchSetRequestRequestTypeDef = {  # (1)
    "XssMatchSetId": ...,
    "ChangeToken": ...,
}

parent.delete_xss_match_set(**kwargs)
```

1. See [:material-code-braces: DeleteXssMatchSetRequestRequestTypeDef](./type_defs.md#deletexssmatchsetrequestrequesttypedef) 

### disassociate\_web\_acl

.

Type annotations and code completion for `#!python session.create_client("waf-regional").disassociate_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.disassociate_web_acl)

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

kwargs: DisassociateWebACLRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.disassociate_web_acl(**kwargs)
```

1. See [:material-code-braces: DisassociateWebACLRequestRequestTypeDef](./type_defs.md#disassociatewebaclrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("waf-regional").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.generate_presigned_url)

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


### get\_byte\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_byte_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_byte_match_set)

```python
# get_byte_match_set method definition

await def get_byte_match_set(
    self,
    *,
    ByteMatchSetId: str,
) -> GetByteMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetByteMatchSetResponseTypeDef](./type_defs.md#getbytematchsetresponsetypedef) 


```python
# get_byte_match_set method usage example with argument unpacking

kwargs: GetByteMatchSetRequestRequestTypeDef = {  # (1)
    "ByteMatchSetId": ...,
}

parent.get_byte_match_set(**kwargs)
```

1. See [:material-code-braces: GetByteMatchSetRequestRequestTypeDef](./type_defs.md#getbytematchsetrequestrequesttypedef) 

### get\_change\_token

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_change_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_change_token)

```python
# get_change_token method definition

await def get_change_token(
    self,
) -> GetChangeTokenResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChangeTokenResponseTypeDef](./type_defs.md#getchangetokenresponsetypedef) 

### get\_change\_token\_status

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_change_token_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_change_token_status)

```python
# get_change_token_status method definition

await def get_change_token_status(
    self,
    *,
    ChangeToken: str,
) -> GetChangeTokenStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChangeTokenStatusResponseTypeDef](./type_defs.md#getchangetokenstatusresponsetypedef) 


```python
# get_change_token_status method usage example with argument unpacking

kwargs: GetChangeTokenStatusRequestRequestTypeDef = {  # (1)
    "ChangeToken": ...,
}

parent.get_change_token_status(**kwargs)
```

1. See [:material-code-braces: GetChangeTokenStatusRequestRequestTypeDef](./type_defs.md#getchangetokenstatusrequestrequesttypedef) 

### get\_geo\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_geo_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_geo_match_set)

```python
# get_geo_match_set method definition

await def get_geo_match_set(
    self,
    *,
    GeoMatchSetId: str,
) -> GetGeoMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGeoMatchSetResponseTypeDef](./type_defs.md#getgeomatchsetresponsetypedef) 


```python
# get_geo_match_set method usage example with argument unpacking

kwargs: GetGeoMatchSetRequestRequestTypeDef = {  # (1)
    "GeoMatchSetId": ...,
}

parent.get_geo_match_set(**kwargs)
```

1. See [:material-code-braces: GetGeoMatchSetRequestRequestTypeDef](./type_defs.md#getgeomatchsetrequestrequesttypedef) 

### get\_ip\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_ip_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_ip_set)

```python
# get_ip_set method definition

await def get_ip_set(
    self,
    *,
    IPSetId: str,
) -> GetIPSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIPSetResponseTypeDef](./type_defs.md#getipsetresponsetypedef) 


```python
# get_ip_set method usage example with argument unpacking

kwargs: GetIPSetRequestRequestTypeDef = {  # (1)
    "IPSetId": ...,
}

parent.get_ip_set(**kwargs)
```

1. See [:material-code-braces: GetIPSetRequestRequestTypeDef](./type_defs.md#getipsetrequestrequesttypedef) 

### get\_logging\_configuration

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_logging_configuration)

```python
# get_logging_configuration method definition

await def get_logging_configuration(
    self,
    *,
    ResourceArn: str,
) -> GetLoggingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLoggingConfigurationResponseTypeDef](./type_defs.md#getloggingconfigurationresponsetypedef) 


```python
# get_logging_configuration method usage example with argument unpacking

kwargs: GetLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_logging_configuration(**kwargs)
```

1. See [:material-code-braces: GetLoggingConfigurationRequestRequestTypeDef](./type_defs.md#getloggingconfigurationrequestrequesttypedef) 

### get\_permission\_policy

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_permission_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_permission_policy)

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

kwargs: GetPermissionPolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_permission_policy(**kwargs)
```

1. See [:material-code-braces: GetPermissionPolicyRequestRequestTypeDef](./type_defs.md#getpermissionpolicyrequestrequesttypedef) 

### get\_rate\_based\_rule

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_rate_based_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_rate_based_rule)

```python
# get_rate_based_rule method definition

await def get_rate_based_rule(
    self,
    *,
    RuleId: str,
) -> GetRateBasedRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRateBasedRuleResponseTypeDef](./type_defs.md#getratebasedruleresponsetypedef) 


```python
# get_rate_based_rule method usage example with argument unpacking

kwargs: GetRateBasedRuleRequestRequestTypeDef = {  # (1)
    "RuleId": ...,
}

parent.get_rate_based_rule(**kwargs)
```

1. See [:material-code-braces: GetRateBasedRuleRequestRequestTypeDef](./type_defs.md#getratebasedrulerequestrequesttypedef) 

### get\_rate\_based\_rule\_managed\_keys

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_rate_based_rule_managed_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_rate_based_rule_managed_keys)

```python
# get_rate_based_rule_managed_keys method definition

await def get_rate_based_rule_managed_keys(
    self,
    *,
    RuleId: str,
    NextMarker: str = ...,
) -> GetRateBasedRuleManagedKeysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRateBasedRuleManagedKeysResponseTypeDef](./type_defs.md#getratebasedrulemanagedkeysresponsetypedef) 


```python
# get_rate_based_rule_managed_keys method usage example with argument unpacking

kwargs: GetRateBasedRuleManagedKeysRequestRequestTypeDef = {  # (1)
    "RuleId": ...,
}

parent.get_rate_based_rule_managed_keys(**kwargs)
```

1. See [:material-code-braces: GetRateBasedRuleManagedKeysRequestRequestTypeDef](./type_defs.md#getratebasedrulemanagedkeysrequestrequesttypedef) 

### get\_regex\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_regex_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_regex_match_set)

```python
# get_regex_match_set method definition

await def get_regex_match_set(
    self,
    *,
    RegexMatchSetId: str,
) -> GetRegexMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRegexMatchSetResponseTypeDef](./type_defs.md#getregexmatchsetresponsetypedef) 


```python
# get_regex_match_set method usage example with argument unpacking

kwargs: GetRegexMatchSetRequestRequestTypeDef = {  # (1)
    "RegexMatchSetId": ...,
}

parent.get_regex_match_set(**kwargs)
```

1. See [:material-code-braces: GetRegexMatchSetRequestRequestTypeDef](./type_defs.md#getregexmatchsetrequestrequesttypedef) 

### get\_regex\_pattern\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_regex_pattern_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_regex_pattern_set)

```python
# get_regex_pattern_set method definition

await def get_regex_pattern_set(
    self,
    *,
    RegexPatternSetId: str,
) -> GetRegexPatternSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRegexPatternSetResponseTypeDef](./type_defs.md#getregexpatternsetresponsetypedef) 


```python
# get_regex_pattern_set method usage example with argument unpacking

kwargs: GetRegexPatternSetRequestRequestTypeDef = {  # (1)
    "RegexPatternSetId": ...,
}

parent.get_regex_pattern_set(**kwargs)
```

1. See [:material-code-braces: GetRegexPatternSetRequestRequestTypeDef](./type_defs.md#getregexpatternsetrequestrequesttypedef) 

### get\_rule

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_rule)

```python
# get_rule method definition

await def get_rule(
    self,
    *,
    RuleId: str,
) -> GetRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRuleResponseTypeDef](./type_defs.md#getruleresponsetypedef) 


```python
# get_rule method usage example with argument unpacking

kwargs: GetRuleRequestRequestTypeDef = {  # (1)
    "RuleId": ...,
}

parent.get_rule(**kwargs)
```

1. See [:material-code-braces: GetRuleRequestRequestTypeDef](./type_defs.md#getrulerequestrequesttypedef) 

### get\_rule\_group

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_rule_group)

```python
# get_rule_group method definition

await def get_rule_group(
    self,
    *,
    RuleGroupId: str,
) -> GetRuleGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRuleGroupResponseTypeDef](./type_defs.md#getrulegroupresponsetypedef) 


```python
# get_rule_group method usage example with argument unpacking

kwargs: GetRuleGroupRequestRequestTypeDef = {  # (1)
    "RuleGroupId": ...,
}

parent.get_rule_group(**kwargs)
```

1. See [:material-code-braces: GetRuleGroupRequestRequestTypeDef](./type_defs.md#getrulegrouprequestrequesttypedef) 

### get\_sampled\_requests

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_sampled_requests` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_sampled_requests)

```python
# get_sampled_requests method definition

await def get_sampled_requests(
    self,
    *,
    WebAclId: str,
    RuleId: str,
    TimeWindow: TimeWindowTypeDef,  # (1)
    MaxItems: int,
) -> GetSampledRequestsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TimeWindowTypeDef](./type_defs.md#timewindowtypedef) 
2. See [:material-code-braces: GetSampledRequestsResponseTypeDef](./type_defs.md#getsampledrequestsresponsetypedef) 


```python
# get_sampled_requests method usage example with argument unpacking

kwargs: GetSampledRequestsRequestRequestTypeDef = {  # (1)
    "WebAclId": ...,
    "RuleId": ...,
    "TimeWindow": ...,
    "MaxItems": ...,
}

parent.get_sampled_requests(**kwargs)
```

1. See [:material-code-braces: GetSampledRequestsRequestRequestTypeDef](./type_defs.md#getsampledrequestsrequestrequesttypedef) 

### get\_size\_constraint\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_size_constraint_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_size_constraint_set)

```python
# get_size_constraint_set method definition

await def get_size_constraint_set(
    self,
    *,
    SizeConstraintSetId: str,
) -> GetSizeConstraintSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSizeConstraintSetResponseTypeDef](./type_defs.md#getsizeconstraintsetresponsetypedef) 


```python
# get_size_constraint_set method usage example with argument unpacking

kwargs: GetSizeConstraintSetRequestRequestTypeDef = {  # (1)
    "SizeConstraintSetId": ...,
}

parent.get_size_constraint_set(**kwargs)
```

1. See [:material-code-braces: GetSizeConstraintSetRequestRequestTypeDef](./type_defs.md#getsizeconstraintsetrequestrequesttypedef) 

### get\_sql\_injection\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_sql_injection_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_sql_injection_match_set)

```python
# get_sql_injection_match_set method definition

await def get_sql_injection_match_set(
    self,
    *,
    SqlInjectionMatchSetId: str,
) -> GetSqlInjectionMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSqlInjectionMatchSetResponseTypeDef](./type_defs.md#getsqlinjectionmatchsetresponsetypedef) 


```python
# get_sql_injection_match_set method usage example with argument unpacking

kwargs: GetSqlInjectionMatchSetRequestRequestTypeDef = {  # (1)
    "SqlInjectionMatchSetId": ...,
}

parent.get_sql_injection_match_set(**kwargs)
```

1. See [:material-code-braces: GetSqlInjectionMatchSetRequestRequestTypeDef](./type_defs.md#getsqlinjectionmatchsetrequestrequesttypedef) 

### get\_web\_acl

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_web_acl)

```python
# get_web_acl method definition

await def get_web_acl(
    self,
    *,
    WebACLId: str,
) -> GetWebACLResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWebACLResponseTypeDef](./type_defs.md#getwebaclresponsetypedef) 


```python
# get_web_acl method usage example with argument unpacking

kwargs: GetWebACLRequestRequestTypeDef = {  # (1)
    "WebACLId": ...,
}

parent.get_web_acl(**kwargs)
```

1. See [:material-code-braces: GetWebACLRequestRequestTypeDef](./type_defs.md#getwebaclrequestrequesttypedef) 

### get\_web\_acl\_for\_resource

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_web_acl_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_web_acl_for_resource)

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

kwargs: GetWebACLForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_web_acl_for_resource(**kwargs)
```

1. See [:material-code-braces: GetWebACLForResourceRequestRequestTypeDef](./type_defs.md#getwebaclforresourcerequestrequesttypedef) 

### get\_xss\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").get_xss_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_xss_match_set)

```python
# get_xss_match_set method definition

await def get_xss_match_set(
    self,
    *,
    XssMatchSetId: str,
) -> GetXssMatchSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetXssMatchSetResponseTypeDef](./type_defs.md#getxssmatchsetresponsetypedef) 


```python
# get_xss_match_set method usage example with argument unpacking

kwargs: GetXssMatchSetRequestRequestTypeDef = {  # (1)
    "XssMatchSetId": ...,
}

parent.get_xss_match_set(**kwargs)
```

1. See [:material-code-braces: GetXssMatchSetRequestRequestTypeDef](./type_defs.md#getxssmatchsetrequestrequesttypedef) 

### list\_activated\_rules\_in\_rule\_group

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_activated_rules_in_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_activated_rules_in_rule_group)

```python
# list_activated_rules_in_rule_group method definition

await def list_activated_rules_in_rule_group(
    self,
    *,
    RuleGroupId: str = ...,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListActivatedRulesInRuleGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListActivatedRulesInRuleGroupResponseTypeDef](./type_defs.md#listactivatedrulesinrulegroupresponsetypedef) 


```python
# list_activated_rules_in_rule_group method usage example with argument unpacking

kwargs: ListActivatedRulesInRuleGroupRequestRequestTypeDef = {  # (1)
    "RuleGroupId": ...,
}

parent.list_activated_rules_in_rule_group(**kwargs)
```

1. See [:material-code-braces: ListActivatedRulesInRuleGroupRequestRequestTypeDef](./type_defs.md#listactivatedrulesinrulegrouprequestrequesttypedef) 

### list\_byte\_match\_sets

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_byte_match_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_byte_match_sets)

```python
# list_byte_match_sets method definition

await def list_byte_match_sets(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListByteMatchSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListByteMatchSetsResponseTypeDef](./type_defs.md#listbytematchsetsresponsetypedef) 


```python
# list_byte_match_sets method usage example with argument unpacking

kwargs: ListByteMatchSetsRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_byte_match_sets(**kwargs)
```

1. See [:material-code-braces: ListByteMatchSetsRequestRequestTypeDef](./type_defs.md#listbytematchsetsrequestrequesttypedef) 

### list\_geo\_match\_sets

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_geo_match_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_geo_match_sets)

```python
# list_geo_match_sets method definition

await def list_geo_match_sets(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListGeoMatchSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGeoMatchSetsResponseTypeDef](./type_defs.md#listgeomatchsetsresponsetypedef) 


```python
# list_geo_match_sets method usage example with argument unpacking

kwargs: ListGeoMatchSetsRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_geo_match_sets(**kwargs)
```

1. See [:material-code-braces: ListGeoMatchSetsRequestRequestTypeDef](./type_defs.md#listgeomatchsetsrequestrequesttypedef) 

### list\_ip\_sets

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_ip_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_ip_sets)

```python
# list_ip_sets method definition

await def list_ip_sets(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListIPSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef) 


```python
# list_ip_sets method usage example with argument unpacking

kwargs: ListIPSetsRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_ip_sets(**kwargs)
```

1. See [:material-code-braces: ListIPSetsRequestRequestTypeDef](./type_defs.md#listipsetsrequestrequesttypedef) 

### list\_logging\_configurations

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_logging_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_logging_configurations)

```python
# list_logging_configurations method definition

await def list_logging_configurations(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListLoggingConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLoggingConfigurationsResponseTypeDef](./type_defs.md#listloggingconfigurationsresponsetypedef) 


```python
# list_logging_configurations method usage example with argument unpacking

kwargs: ListLoggingConfigurationsRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_logging_configurations(**kwargs)
```

1. See [:material-code-braces: ListLoggingConfigurationsRequestRequestTypeDef](./type_defs.md#listloggingconfigurationsrequestrequesttypedef) 

### list\_rate\_based\_rules

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_rate_based_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_rate_based_rules)

```python
# list_rate_based_rules method definition

await def list_rate_based_rules(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListRateBasedRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRateBasedRulesResponseTypeDef](./type_defs.md#listratebasedrulesresponsetypedef) 


```python
# list_rate_based_rules method usage example with argument unpacking

kwargs: ListRateBasedRulesRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_rate_based_rules(**kwargs)
```

1. See [:material-code-braces: ListRateBasedRulesRequestRequestTypeDef](./type_defs.md#listratebasedrulesrequestrequesttypedef) 

### list\_regex\_match\_sets

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_regex_match_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_regex_match_sets)

```python
# list_regex_match_sets method definition

await def list_regex_match_sets(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListRegexMatchSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRegexMatchSetsResponseTypeDef](./type_defs.md#listregexmatchsetsresponsetypedef) 


```python
# list_regex_match_sets method usage example with argument unpacking

kwargs: ListRegexMatchSetsRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_regex_match_sets(**kwargs)
```

1. See [:material-code-braces: ListRegexMatchSetsRequestRequestTypeDef](./type_defs.md#listregexmatchsetsrequestrequesttypedef) 

### list\_regex\_pattern\_sets

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_regex_pattern_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_regex_pattern_sets)

```python
# list_regex_pattern_sets method definition

await def list_regex_pattern_sets(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListRegexPatternSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRegexPatternSetsResponseTypeDef](./type_defs.md#listregexpatternsetsresponsetypedef) 


```python
# list_regex_pattern_sets method usage example with argument unpacking

kwargs: ListRegexPatternSetsRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_regex_pattern_sets(**kwargs)
```

1. See [:material-code-braces: ListRegexPatternSetsRequestRequestTypeDef](./type_defs.md#listregexpatternsetsrequestrequesttypedef) 

### list\_resources\_for\_web\_acl

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_resources_for_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_resources_for_web_acl)

```python
# list_resources_for_web_acl method definition

await def list_resources_for_web_acl(
    self,
    *,
    WebACLId: str,
    ResourceType: ResourceTypeType = ...,  # (1)
) -> ListResourcesForWebACLResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ListResourcesForWebACLResponseTypeDef](./type_defs.md#listresourcesforwebaclresponsetypedef) 


```python
# list_resources_for_web_acl method usage example with argument unpacking

kwargs: ListResourcesForWebACLRequestRequestTypeDef = {  # (1)
    "WebACLId": ...,
}

parent.list_resources_for_web_acl(**kwargs)
```

1. See [:material-code-braces: ListResourcesForWebACLRequestRequestTypeDef](./type_defs.md#listresourcesforwebaclrequestrequesttypedef) 

### list\_rule\_groups

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_rule_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_rule_groups)

```python
# list_rule_groups method definition

await def list_rule_groups(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListRuleGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRuleGroupsResponseTypeDef](./type_defs.md#listrulegroupsresponsetypedef) 


```python
# list_rule_groups method usage example with argument unpacking

kwargs: ListRuleGroupsRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_rule_groups(**kwargs)
```

1. See [:material-code-braces: ListRuleGroupsRequestRequestTypeDef](./type_defs.md#listrulegroupsrequestrequesttypedef) 

### list\_rules

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_rules)

```python
# list_rules method definition

await def list_rules(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef) 


```python
# list_rules method usage example with argument unpacking

kwargs: ListRulesRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_rules(**kwargs)
```

1. See [:material-code-braces: ListRulesRequestRequestTypeDef](./type_defs.md#listrulesrequestrequesttypedef) 

### list\_size\_constraint\_sets

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_size_constraint_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_size_constraint_sets)

```python
# list_size_constraint_sets method definition

await def list_size_constraint_sets(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListSizeConstraintSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSizeConstraintSetsResponseTypeDef](./type_defs.md#listsizeconstraintsetsresponsetypedef) 


```python
# list_size_constraint_sets method usage example with argument unpacking

kwargs: ListSizeConstraintSetsRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_size_constraint_sets(**kwargs)
```

1. See [:material-code-braces: ListSizeConstraintSetsRequestRequestTypeDef](./type_defs.md#listsizeconstraintsetsrequestrequesttypedef) 

### list\_sql\_injection\_match\_sets

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_sql_injection_match_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_sql_injection_match_sets)

```python
# list_sql_injection_match_sets method definition

await def list_sql_injection_match_sets(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListSqlInjectionMatchSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSqlInjectionMatchSetsResponseTypeDef](./type_defs.md#listsqlinjectionmatchsetsresponsetypedef) 


```python
# list_sql_injection_match_sets method usage example with argument unpacking

kwargs: ListSqlInjectionMatchSetsRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_sql_injection_match_sets(**kwargs)
```

1. See [:material-code-braces: ListSqlInjectionMatchSetsRequestRequestTypeDef](./type_defs.md#listsqlinjectionmatchsetsrequestrequesttypedef) 

### list\_subscribed\_rule\_groups

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_subscribed_rule_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_subscribed_rule_groups)

```python
# list_subscribed_rule_groups method definition

await def list_subscribed_rule_groups(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListSubscribedRuleGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSubscribedRuleGroupsResponseTypeDef](./type_defs.md#listsubscribedrulegroupsresponsetypedef) 


```python
# list_subscribed_rule_groups method usage example with argument unpacking

kwargs: ListSubscribedRuleGroupsRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_subscribed_rule_groups(**kwargs)
```

1. See [:material-code-braces: ListSubscribedRuleGroupsRequestRequestTypeDef](./type_defs.md#listsubscribedrulegroupsrequestrequesttypedef) 

### list\_tags\_for\_resource

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_tags_for_resource)

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

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_web\_acls

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_web_acls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_web_acls)

```python
# list_web_acls method definition

await def list_web_acls(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListWebACLsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWebACLsResponseTypeDef](./type_defs.md#listwebaclsresponsetypedef) 


```python
# list_web_acls method usage example with argument unpacking

kwargs: ListWebACLsRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_web_acls(**kwargs)
```

1. See [:material-code-braces: ListWebACLsRequestRequestTypeDef](./type_defs.md#listwebaclsrequestrequesttypedef) 

### list\_xss\_match\_sets

.

Type annotations and code completion for `#!python session.create_client("waf-regional").list_xss_match_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_xss_match_sets)

```python
# list_xss_match_sets method definition

await def list_xss_match_sets(
    self,
    *,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListXssMatchSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListXssMatchSetsResponseTypeDef](./type_defs.md#listxssmatchsetsresponsetypedef) 


```python
# list_xss_match_sets method usage example with argument unpacking

kwargs: ListXssMatchSetsRequestRequestTypeDef = {  # (1)
    "NextMarker": ...,
}

parent.list_xss_match_sets(**kwargs)
```

1. See [:material-code-braces: ListXssMatchSetsRequestRequestTypeDef](./type_defs.md#listxssmatchsetsrequestrequesttypedef) 

### put\_logging\_configuration

.

Type annotations and code completion for `#!python session.create_client("waf-regional").put_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.put_logging_configuration)

```python
# put_logging_configuration method definition

await def put_logging_configuration(
    self,
    *,
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
) -> PutLoggingConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: PutLoggingConfigurationResponseTypeDef](./type_defs.md#putloggingconfigurationresponsetypedef) 


```python
# put_logging_configuration method usage example with argument unpacking

kwargs: PutLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "LoggingConfiguration": ...,
}

parent.put_logging_configuration(**kwargs)
```

1. See [:material-code-braces: PutLoggingConfigurationRequestRequestTypeDef](./type_defs.md#putloggingconfigurationrequestrequesttypedef) 

### put\_permission\_policy

.

Type annotations and code completion for `#!python session.create_client("waf-regional").put_permission_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.put_permission_policy)

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

kwargs: PutPermissionPolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Policy": ...,
}

parent.put_permission_policy(**kwargs)
```

1. See [:material-code-braces: PutPermissionPolicyRequestRequestTypeDef](./type_defs.md#putpermissionpolicyrequestrequesttypedef) 

### tag\_resource

.

Type annotations and code completion for `#!python session.create_client("waf-regional").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.tag_resource)

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

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

.

Type annotations and code completion for `#!python session.create_client("waf-regional").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.untag_resource)

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

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_byte\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").update_byte_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.update_byte_match_set)

```python
# update_byte_match_set method definition

await def update_byte_match_set(
    self,
    *,
    ByteMatchSetId: str,
    ChangeToken: str,
    Updates: Sequence[ByteMatchSetUpdateTypeDef],  # (1)
) -> UpdateByteMatchSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ByteMatchSetUpdateTypeDef](./type_defs.md#bytematchsetupdatetypedef) 
2. See [:material-code-braces: UpdateByteMatchSetResponseTypeDef](./type_defs.md#updatebytematchsetresponsetypedef) 


```python
# update_byte_match_set method usage example with argument unpacking

kwargs: UpdateByteMatchSetRequestRequestTypeDef = {  # (1)
    "ByteMatchSetId": ...,
    "ChangeToken": ...,
    "Updates": ...,
}

parent.update_byte_match_set(**kwargs)
```

1. See [:material-code-braces: UpdateByteMatchSetRequestRequestTypeDef](./type_defs.md#updatebytematchsetrequestrequesttypedef) 

### update\_geo\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").update_geo_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.update_geo_match_set)

```python
# update_geo_match_set method definition

await def update_geo_match_set(
    self,
    *,
    GeoMatchSetId: str,
    ChangeToken: str,
    Updates: Sequence[GeoMatchSetUpdateTypeDef],  # (1)
) -> UpdateGeoMatchSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GeoMatchSetUpdateTypeDef](./type_defs.md#geomatchsetupdatetypedef) 
2. See [:material-code-braces: UpdateGeoMatchSetResponseTypeDef](./type_defs.md#updategeomatchsetresponsetypedef) 


```python
# update_geo_match_set method usage example with argument unpacking

kwargs: UpdateGeoMatchSetRequestRequestTypeDef = {  # (1)
    "GeoMatchSetId": ...,
    "ChangeToken": ...,
    "Updates": ...,
}

parent.update_geo_match_set(**kwargs)
```

1. See [:material-code-braces: UpdateGeoMatchSetRequestRequestTypeDef](./type_defs.md#updategeomatchsetrequestrequesttypedef) 

### update\_ip\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").update_ip_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.update_ip_set)

```python
# update_ip_set method definition

await def update_ip_set(
    self,
    *,
    IPSetId: str,
    ChangeToken: str,
    Updates: Sequence[IPSetUpdateTypeDef],  # (1)
) -> UpdateIPSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IPSetUpdateTypeDef](./type_defs.md#ipsetupdatetypedef) 
2. See [:material-code-braces: UpdateIPSetResponseTypeDef](./type_defs.md#updateipsetresponsetypedef) 


```python
# update_ip_set method usage example with argument unpacking

kwargs: UpdateIPSetRequestRequestTypeDef = {  # (1)
    "IPSetId": ...,
    "ChangeToken": ...,
    "Updates": ...,
}

parent.update_ip_set(**kwargs)
```

1. See [:material-code-braces: UpdateIPSetRequestRequestTypeDef](./type_defs.md#updateipsetrequestrequesttypedef) 

### update\_rate\_based\_rule

.

Type annotations and code completion for `#!python session.create_client("waf-regional").update_rate_based_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.update_rate_based_rule)

```python
# update_rate_based_rule method definition

await def update_rate_based_rule(
    self,
    *,
    RuleId: str,
    ChangeToken: str,
    Updates: Sequence[RuleUpdateTypeDef],  # (1)
    RateLimit: int,
) -> UpdateRateBasedRuleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RuleUpdateTypeDef](./type_defs.md#ruleupdatetypedef) 
2. See [:material-code-braces: UpdateRateBasedRuleResponseTypeDef](./type_defs.md#updateratebasedruleresponsetypedef) 


```python
# update_rate_based_rule method usage example with argument unpacking

kwargs: UpdateRateBasedRuleRequestRequestTypeDef = {  # (1)
    "RuleId": ...,
    "ChangeToken": ...,
    "Updates": ...,
    "RateLimit": ...,
}

parent.update_rate_based_rule(**kwargs)
```

1. See [:material-code-braces: UpdateRateBasedRuleRequestRequestTypeDef](./type_defs.md#updateratebasedrulerequestrequesttypedef) 

### update\_regex\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").update_regex_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.update_regex_match_set)

```python
# update_regex_match_set method definition

await def update_regex_match_set(
    self,
    *,
    RegexMatchSetId: str,
    Updates: Sequence[RegexMatchSetUpdateTypeDef],  # (1)
    ChangeToken: str,
) -> UpdateRegexMatchSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RegexMatchSetUpdateTypeDef](./type_defs.md#regexmatchsetupdatetypedef) 
2. See [:material-code-braces: UpdateRegexMatchSetResponseTypeDef](./type_defs.md#updateregexmatchsetresponsetypedef) 


```python
# update_regex_match_set method usage example with argument unpacking

kwargs: UpdateRegexMatchSetRequestRequestTypeDef = {  # (1)
    "RegexMatchSetId": ...,
    "Updates": ...,
    "ChangeToken": ...,
}

parent.update_regex_match_set(**kwargs)
```

1. See [:material-code-braces: UpdateRegexMatchSetRequestRequestTypeDef](./type_defs.md#updateregexmatchsetrequestrequesttypedef) 

### update\_regex\_pattern\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").update_regex_pattern_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.update_regex_pattern_set)

```python
# update_regex_pattern_set method definition

await def update_regex_pattern_set(
    self,
    *,
    RegexPatternSetId: str,
    Updates: Sequence[RegexPatternSetUpdateTypeDef],  # (1)
    ChangeToken: str,
) -> UpdateRegexPatternSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RegexPatternSetUpdateTypeDef](./type_defs.md#regexpatternsetupdatetypedef) 
2. See [:material-code-braces: UpdateRegexPatternSetResponseTypeDef](./type_defs.md#updateregexpatternsetresponsetypedef) 


```python
# update_regex_pattern_set method usage example with argument unpacking

kwargs: UpdateRegexPatternSetRequestRequestTypeDef = {  # (1)
    "RegexPatternSetId": ...,
    "Updates": ...,
    "ChangeToken": ...,
}

parent.update_regex_pattern_set(**kwargs)
```

1. See [:material-code-braces: UpdateRegexPatternSetRequestRequestTypeDef](./type_defs.md#updateregexpatternsetrequestrequesttypedef) 

### update\_rule

.

Type annotations and code completion for `#!python session.create_client("waf-regional").update_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.update_rule)

```python
# update_rule method definition

await def update_rule(
    self,
    *,
    RuleId: str,
    ChangeToken: str,
    Updates: Sequence[RuleUpdateTypeDef],  # (1)
) -> UpdateRuleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RuleUpdateTypeDef](./type_defs.md#ruleupdatetypedef) 
2. See [:material-code-braces: UpdateRuleResponseTypeDef](./type_defs.md#updateruleresponsetypedef) 


```python
# update_rule method usage example with argument unpacking

kwargs: UpdateRuleRequestRequestTypeDef = {  # (1)
    "RuleId": ...,
    "ChangeToken": ...,
    "Updates": ...,
}

parent.update_rule(**kwargs)
```

1. See [:material-code-braces: UpdateRuleRequestRequestTypeDef](./type_defs.md#updaterulerequestrequesttypedef) 

### update\_rule\_group

.

Type annotations and code completion for `#!python session.create_client("waf-regional").update_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.update_rule_group)

```python
# update_rule_group method definition

await def update_rule_group(
    self,
    *,
    RuleGroupId: str,
    Updates: Sequence[RuleGroupUpdateTypeDef],  # (1)
    ChangeToken: str,
) -> UpdateRuleGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RuleGroupUpdateTypeDef](./type_defs.md#rulegroupupdatetypedef) 
2. See [:material-code-braces: UpdateRuleGroupResponseTypeDef](./type_defs.md#updaterulegroupresponsetypedef) 


```python
# update_rule_group method usage example with argument unpacking

kwargs: UpdateRuleGroupRequestRequestTypeDef = {  # (1)
    "RuleGroupId": ...,
    "Updates": ...,
    "ChangeToken": ...,
}

parent.update_rule_group(**kwargs)
```

1. See [:material-code-braces: UpdateRuleGroupRequestRequestTypeDef](./type_defs.md#updaterulegrouprequestrequesttypedef) 

### update\_size\_constraint\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").update_size_constraint_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.update_size_constraint_set)

```python
# update_size_constraint_set method definition

await def update_size_constraint_set(
    self,
    *,
    SizeConstraintSetId: str,
    ChangeToken: str,
    Updates: Sequence[SizeConstraintSetUpdateTypeDef],  # (1)
) -> UpdateSizeConstraintSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SizeConstraintSetUpdateTypeDef](./type_defs.md#sizeconstraintsetupdatetypedef) 
2. See [:material-code-braces: UpdateSizeConstraintSetResponseTypeDef](./type_defs.md#updatesizeconstraintsetresponsetypedef) 


```python
# update_size_constraint_set method usage example with argument unpacking

kwargs: UpdateSizeConstraintSetRequestRequestTypeDef = {  # (1)
    "SizeConstraintSetId": ...,
    "ChangeToken": ...,
    "Updates": ...,
}

parent.update_size_constraint_set(**kwargs)
```

1. See [:material-code-braces: UpdateSizeConstraintSetRequestRequestTypeDef](./type_defs.md#updatesizeconstraintsetrequestrequesttypedef) 

### update\_sql\_injection\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").update_sql_injection_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.update_sql_injection_match_set)

```python
# update_sql_injection_match_set method definition

await def update_sql_injection_match_set(
    self,
    *,
    SqlInjectionMatchSetId: str,
    ChangeToken: str,
    Updates: Sequence[SqlInjectionMatchSetUpdateTypeDef],  # (1)
) -> UpdateSqlInjectionMatchSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SqlInjectionMatchSetUpdateTypeDef](./type_defs.md#sqlinjectionmatchsetupdatetypedef) 
2. See [:material-code-braces: UpdateSqlInjectionMatchSetResponseTypeDef](./type_defs.md#updatesqlinjectionmatchsetresponsetypedef) 


```python
# update_sql_injection_match_set method usage example with argument unpacking

kwargs: UpdateSqlInjectionMatchSetRequestRequestTypeDef = {  # (1)
    "SqlInjectionMatchSetId": ...,
    "ChangeToken": ...,
    "Updates": ...,
}

parent.update_sql_injection_match_set(**kwargs)
```

1. See [:material-code-braces: UpdateSqlInjectionMatchSetRequestRequestTypeDef](./type_defs.md#updatesqlinjectionmatchsetrequestrequesttypedef) 

### update\_web\_acl

.

Type annotations and code completion for `#!python session.create_client("waf-regional").update_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.update_web_acl)

```python
# update_web_acl method definition

await def update_web_acl(
    self,
    *,
    WebACLId: str,
    ChangeToken: str,
    Updates: Sequence[WebACLUpdateTypeDef] = ...,  # (1)
    DefaultAction: WafActionTypeDef = ...,  # (2)
) -> UpdateWebACLResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: WebACLUpdateTypeDef](./type_defs.md#webaclupdatetypedef) 
2. See [:material-code-braces: WafActionTypeDef](./type_defs.md#wafactiontypedef) 
3. See [:material-code-braces: UpdateWebACLResponseTypeDef](./type_defs.md#updatewebaclresponsetypedef) 


```python
# update_web_acl method usage example with argument unpacking

kwargs: UpdateWebACLRequestRequestTypeDef = {  # (1)
    "WebACLId": ...,
    "ChangeToken": ...,
}

parent.update_web_acl(**kwargs)
```

1. See [:material-code-braces: UpdateWebACLRequestRequestTypeDef](./type_defs.md#updatewebaclrequestrequesttypedef) 

### update\_xss\_match\_set

.

Type annotations and code completion for `#!python session.create_client("waf-regional").update_xss_match_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.update_xss_match_set)

```python
# update_xss_match_set method definition

await def update_xss_match_set(
    self,
    *,
    XssMatchSetId: str,
    ChangeToken: str,
    Updates: Sequence[XssMatchSetUpdateTypeDef],  # (1)
) -> UpdateXssMatchSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: XssMatchSetUpdateTypeDef](./type_defs.md#xssmatchsetupdatetypedef) 
2. See [:material-code-braces: UpdateXssMatchSetResponseTypeDef](./type_defs.md#updatexssmatchsetresponsetypedef) 


```python
# update_xss_match_set method usage example with argument unpacking

kwargs: UpdateXssMatchSetRequestRequestTypeDef = {  # (1)
    "XssMatchSetId": ...,
    "ChangeToken": ...,
    "Updates": ...,
}

parent.update_xss_match_set(**kwargs)
```

1. See [:material-code-braces: UpdateXssMatchSetRequestRequestTypeDef](./type_defs.md#updatexssmatchsetrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("waf-regional").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "WAFRegionalClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("waf-regional").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.__aexit__)

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





