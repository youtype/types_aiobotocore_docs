<a id="wafclient-for-aiobotocore-waf-module"></a>

# WAFClient for aiobotocore WAF module

> [Index](..) > [WAF](.) > WAFClient

Auto-generated documentation for
[WAF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
type annotations stubs module
[types-aiobotocore-waf](https://pypi.org/project/types-aiobotocore-waf/).

- [WAFClient for aiobotocore WAF module](#wafclient-for-aiobotocore-waf-module)
  - [WAFClient](#wafclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_byte_match_set](#create_byte_match_set)
    - [create_geo_match_set](#create_geo_match_set)
    - [create_ip_set](#create_ip_set)
    - [create_rate_based_rule](#create_rate_based_rule)
    - [create_regex_match_set](#create_regex_match_set)
    - [create_regex_pattern_set](#create_regex_pattern_set)
    - [create_rule](#create_rule)
    - [create_rule_group](#create_rule_group)
    - [create_size_constraint_set](#create_size_constraint_set)
    - [create_sql_injection_match_set](#create_sql_injection_match_set)
    - [create_web_acl](#create_web_acl)
    - [create_web_acl_migration_stack](#create_web_acl_migration_stack)
    - [create_xss_match_set](#create_xss_match_set)
    - [delete_byte_match_set](#delete_byte_match_set)
    - [delete_geo_match_set](#delete_geo_match_set)
    - [delete_ip_set](#delete_ip_set)
    - [delete_logging_configuration](#delete_logging_configuration)
    - [delete_permission_policy](#delete_permission_policy)
    - [delete_rate_based_rule](#delete_rate_based_rule)
    - [delete_regex_match_set](#delete_regex_match_set)
    - [delete_regex_pattern_set](#delete_regex_pattern_set)
    - [delete_rule](#delete_rule)
    - [delete_rule_group](#delete_rule_group)
    - [delete_size_constraint_set](#delete_size_constraint_set)
    - [delete_sql_injection_match_set](#delete_sql_injection_match_set)
    - [delete_web_acl](#delete_web_acl)
    - [delete_xss_match_set](#delete_xss_match_set)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_byte_match_set](#get_byte_match_set)
    - [get_change_token](#get_change_token)
    - [get_change_token_status](#get_change_token_status)
    - [get_geo_match_set](#get_geo_match_set)
    - [get_ip_set](#get_ip_set)
    - [get_logging_configuration](#get_logging_configuration)
    - [get_permission_policy](#get_permission_policy)
    - [get_rate_based_rule](#get_rate_based_rule)
    - [get_rate_based_rule_managed_keys](#get_rate_based_rule_managed_keys)
    - [get_regex_match_set](#get_regex_match_set)
    - [get_regex_pattern_set](#get_regex_pattern_set)
    - [get_rule](#get_rule)
    - [get_rule_group](#get_rule_group)
    - [get_sampled_requests](#get_sampled_requests)
    - [get_size_constraint_set](#get_size_constraint_set)
    - [get_sql_injection_match_set](#get_sql_injection_match_set)
    - [get_web_acl](#get_web_acl)
    - [get_xss_match_set](#get_xss_match_set)
    - [list_activated_rules_in_rule_group](#list_activated_rules_in_rule_group)
    - [list_byte_match_sets](#list_byte_match_sets)
    - [list_geo_match_sets](#list_geo_match_sets)
    - [list_ip_sets](#list_ip_sets)
    - [list_logging_configurations](#list_logging_configurations)
    - [list_rate_based_rules](#list_rate_based_rules)
    - [list_regex_match_sets](#list_regex_match_sets)
    - [list_regex_pattern_sets](#list_regex_pattern_sets)
    - [list_rule_groups](#list_rule_groups)
    - [list_rules](#list_rules)
    - [list_size_constraint_sets](#list_size_constraint_sets)
    - [list_sql_injection_match_sets](#list_sql_injection_match_sets)
    - [list_subscribed_rule_groups](#list_subscribed_rule_groups)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_web_acls](#list_web_acls)
    - [list_xss_match_sets](#list_xss_match_sets)
    - [put_logging_configuration](#put_logging_configuration)
    - [put_permission_policy](#put_permission_policy)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_byte_match_set](#update_byte_match_set)
    - [update_geo_match_set](#update_geo_match_set)
    - [update_ip_set](#update_ip_set)
    - [update_rate_based_rule](#update_rate_based_rule)
    - [update_regex_match_set](#update_regex_match_set)
    - [update_regex_pattern_set](#update_regex_pattern_set)
    - [update_rule](#update_rule)
    - [update_rule_group](#update_rule_group)
    - [update_size_constraint_set](#update_size_constraint_set)
    - [update_sql_injection_match_set](#update_sql_injection_match_set)
    - [update_web_acl](#update_web_acl)
    - [update_xss_match_set](#update_xss_match_set)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="wafclient"></a>

## WAFClient

Type annotations for `session.create_client("waf")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_waf.client import WAFClient

session = get_session()
async with session.create_client("waf") as client:
    client: WAFClient
```

Boto3 documentation:
[WAF.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_waf.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.WAFBadRequestException`
- `Exceptions.WAFDisallowedNameException`
- `Exceptions.WAFEntityMigrationException`
- `Exceptions.WAFInternalErrorException`
- `Exceptions.WAFInvalidAccountException`
- `Exceptions.WAFInvalidOperationException`
- `Exceptions.WAFInvalidParameterException`
- `Exceptions.WAFInvalidPermissionPolicyException`
- `Exceptions.WAFInvalidRegexPatternException`
- `Exceptions.WAFLimitsExceededException`
- `Exceptions.WAFNonEmptyEntityException`
- `Exceptions.WAFNonexistentContainerException`
- `Exceptions.WAFNonexistentItemException`
- `Exceptions.WAFReferencedItemException`
- `Exceptions.WAFServiceLinkedRoleErrorException`
- `Exceptions.WAFStaleDataException`
- `Exceptions.WAFSubscriptionNotFoundException`
- `Exceptions.WAFTagOperationException`
- `Exceptions.WAFTagOperationInternalErrorException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

WAFClient exceptions.

Type annotations for `session.create_client("waf").exceptions` method.

Boto3 documentation:
[WAF.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("waf").can_paginate` method.

Boto3 documentation:
[WAF.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_byte_match_set"></a>

### create_byte_match_set

.

Type annotations for `session.create_client("waf").create_byte_match_set`
method.

Boto3 documentation:
[WAF.Client.create_byte_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_byte_match_set)

Asynchronous method. Use `await create_byte_match_set(...)` for a synchronous
call.

Arguments mapping described in
[CreateByteMatchSetRequestRequestTypeDef](./type_defs.md#createbytematchsetrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[CreateByteMatchSetResponseTypeDef](./type_defs.md#createbytematchsetresponsetypedef).

<a id="create_geo_match_set"></a>

### create_geo_match_set

.

Type annotations for `session.create_client("waf").create_geo_match_set`
method.

Boto3 documentation:
[WAF.Client.create_geo_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_geo_match_set)

Asynchronous method. Use `await create_geo_match_set(...)` for a synchronous
call.

Arguments mapping described in
[CreateGeoMatchSetRequestRequestTypeDef](./type_defs.md#creategeomatchsetrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[CreateGeoMatchSetResponseTypeDef](./type_defs.md#creategeomatchsetresponsetypedef).

<a id="create_ip_set"></a>

### create_ip_set

.

Type annotations for `session.create_client("waf").create_ip_set` method.

Boto3 documentation:
[WAF.Client.create_ip_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_ip_set)

Asynchronous method. Use `await create_ip_set(...)` for a synchronous call.

Arguments mapping described in
[CreateIPSetRequestRequestTypeDef](./type_defs.md#createipsetrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[CreateIPSetResponseTypeDef](./type_defs.md#createipsetresponsetypedef).

<a id="create_rate_based_rule"></a>

### create_rate_based_rule

.

Type annotations for `session.create_client("waf").create_rate_based_rule`
method.

Boto3 documentation:
[WAF.Client.create_rate_based_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_rate_based_rule)

Asynchronous method. Use `await create_rate_based_rule(...)` for a synchronous
call.

Arguments mapping described in
[CreateRateBasedRuleRequestRequestTypeDef](./type_defs.md#createratebasedrulerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `MetricName`: `str` *(required)*
- `RateKey`: `Literal['IP']` (see [RateKeyType](./literals.md#ratekeytype))
  *(required)*
- `RateLimit`: `int` *(required)*
- `ChangeToken`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateRateBasedRuleResponseTypeDef](./type_defs.md#createratebasedruleresponsetypedef).

<a id="create_regex_match_set"></a>

### create_regex_match_set

.

Type annotations for `session.create_client("waf").create_regex_match_set`
method.

Boto3 documentation:
[WAF.Client.create_regex_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_regex_match_set)

Asynchronous method. Use `await create_regex_match_set(...)` for a synchronous
call.

Arguments mapping described in
[CreateRegexMatchSetRequestRequestTypeDef](./type_defs.md#createregexmatchsetrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[CreateRegexMatchSetResponseTypeDef](./type_defs.md#createregexmatchsetresponsetypedef).

<a id="create_regex_pattern_set"></a>

### create_regex_pattern_set

.

Type annotations for `session.create_client("waf").create_regex_pattern_set`
method.

Boto3 documentation:
[WAF.Client.create_regex_pattern_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_regex_pattern_set)

Asynchronous method. Use `await create_regex_pattern_set(...)` for a
synchronous call.

Arguments mapping described in
[CreateRegexPatternSetRequestRequestTypeDef](./type_defs.md#createregexpatternsetrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[CreateRegexPatternSetResponseTypeDef](./type_defs.md#createregexpatternsetresponsetypedef).

<a id="create_rule"></a>

### create_rule

.

Type annotations for `session.create_client("waf").create_rule` method.

Boto3 documentation:
[WAF.Client.create_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_rule)

Asynchronous method. Use `await create_rule(...)` for a synchronous call.

Arguments mapping described in
[CreateRuleRequestRequestTypeDef](./type_defs.md#createrulerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `MetricName`: `str` *(required)*
- `ChangeToken`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateRuleResponseTypeDef](./type_defs.md#createruleresponsetypedef).

<a id="create_rule_group"></a>

### create_rule_group

.

Type annotations for `session.create_client("waf").create_rule_group` method.

Boto3 documentation:
[WAF.Client.create_rule_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_rule_group)

Asynchronous method. Use `await create_rule_group(...)` for a synchronous call.

Arguments mapping described in
[CreateRuleGroupRequestRequestTypeDef](./type_defs.md#createrulegrouprequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `MetricName`: `str` *(required)*
- `ChangeToken`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateRuleGroupResponseTypeDef](./type_defs.md#createrulegroupresponsetypedef).

<a id="create_size_constraint_set"></a>

### create_size_constraint_set

.

Type annotations for `session.create_client("waf").create_size_constraint_set`
method.

Boto3 documentation:
[WAF.Client.create_size_constraint_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_size_constraint_set)

Asynchronous method. Use `await create_size_constraint_set(...)` for a
synchronous call.

Arguments mapping described in
[CreateSizeConstraintSetRequestRequestTypeDef](./type_defs.md#createsizeconstraintsetrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[CreateSizeConstraintSetResponseTypeDef](./type_defs.md#createsizeconstraintsetresponsetypedef).

<a id="create_sql_injection_match_set"></a>

### create_sql_injection_match_set

.

Type annotations for
`session.create_client("waf").create_sql_injection_match_set` method.

Boto3 documentation:
[WAF.Client.create_sql_injection_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_sql_injection_match_set)

Asynchronous method. Use `await create_sql_injection_match_set(...)` for a
synchronous call.

Arguments mapping described in
[CreateSqlInjectionMatchSetRequestRequestTypeDef](./type_defs.md#createsqlinjectionmatchsetrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[CreateSqlInjectionMatchSetResponseTypeDef](./type_defs.md#createsqlinjectionmatchsetresponsetypedef).

<a id="create_web_acl"></a>

### create_web_acl

.

Type annotations for `session.create_client("waf").create_web_acl` method.

Boto3 documentation:
[WAF.Client.create_web_acl](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_web_acl)

Asynchronous method. Use `await create_web_acl(...)` for a synchronous call.

Arguments mapping described in
[CreateWebACLRequestRequestTypeDef](./type_defs.md#createwebaclrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `MetricName`: `str` *(required)*
- `DefaultAction`: [WafActionTypeDef](./type_defs.md#wafactiontypedef)
  *(required)*
- `ChangeToken`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateWebACLResponseTypeDef](./type_defs.md#createwebaclresponsetypedef).

<a id="create_web_acl_migration_stack"></a>

### create_web_acl_migration_stack

Creates an AWS CloudFormation WAFV2 template for the specified web ACL in the
specified Amazon S3 bucket.

Type annotations for
`session.create_client("waf").create_web_acl_migration_stack` method.

Boto3 documentation:
[WAF.Client.create_web_acl_migration_stack](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_web_acl_migration_stack)

Asynchronous method. Use `await create_web_acl_migration_stack(...)` for a
synchronous call.

Arguments mapping described in
[CreateWebACLMigrationStackRequestRequestTypeDef](./type_defs.md#createwebaclmigrationstackrequestrequesttypedef).

Keyword-only arguments:

- `WebACLId`: `str` *(required)*
- `S3BucketName`: `str` *(required)*
- `IgnoreUnsupportedType`: `bool` *(required)*

Returns a `Coroutine` for
[CreateWebACLMigrationStackResponseTypeDef](./type_defs.md#createwebaclmigrationstackresponsetypedef).

<a id="create_xss_match_set"></a>

### create_xss_match_set

.

Type annotations for `session.create_client("waf").create_xss_match_set`
method.

Boto3 documentation:
[WAF.Client.create_xss_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_xss_match_set)

Asynchronous method. Use `await create_xss_match_set(...)` for a synchronous
call.

Arguments mapping described in
[CreateXssMatchSetRequestRequestTypeDef](./type_defs.md#createxssmatchsetrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[CreateXssMatchSetResponseTypeDef](./type_defs.md#createxssmatchsetresponsetypedef).

<a id="delete_byte_match_set"></a>

### delete_byte_match_set

.

Type annotations for `session.create_client("waf").delete_byte_match_set`
method.

Boto3 documentation:
[WAF.Client.delete_byte_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_byte_match_set)

Asynchronous method. Use `await delete_byte_match_set(...)` for a synchronous
call.

Arguments mapping described in
[DeleteByteMatchSetRequestRequestTypeDef](./type_defs.md#deletebytematchsetrequestrequesttypedef).

Keyword-only arguments:

- `ByteMatchSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[DeleteByteMatchSetResponseTypeDef](./type_defs.md#deletebytematchsetresponsetypedef).

<a id="delete_geo_match_set"></a>

### delete_geo_match_set

.

Type annotations for `session.create_client("waf").delete_geo_match_set`
method.

Boto3 documentation:
[WAF.Client.delete_geo_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_geo_match_set)

Asynchronous method. Use `await delete_geo_match_set(...)` for a synchronous
call.

Arguments mapping described in
[DeleteGeoMatchSetRequestRequestTypeDef](./type_defs.md#deletegeomatchsetrequestrequesttypedef).

Keyword-only arguments:

- `GeoMatchSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[DeleteGeoMatchSetResponseTypeDef](./type_defs.md#deletegeomatchsetresponsetypedef).

<a id="delete_ip_set"></a>

### delete_ip_set

.

Type annotations for `session.create_client("waf").delete_ip_set` method.

Boto3 documentation:
[WAF.Client.delete_ip_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_ip_set)

Asynchronous method. Use `await delete_ip_set(...)` for a synchronous call.

Arguments mapping described in
[DeleteIPSetRequestRequestTypeDef](./type_defs.md#deleteipsetrequestrequesttypedef).

Keyword-only arguments:

- `IPSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[DeleteIPSetResponseTypeDef](./type_defs.md#deleteipsetresponsetypedef).

<a id="delete_logging_configuration"></a>

### delete_logging_configuration

.

Type annotations for
`session.create_client("waf").delete_logging_configuration` method.

Boto3 documentation:
[WAF.Client.delete_logging_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_logging_configuration)

Asynchronous method. Use `await delete_logging_configuration(...)` for a
synchronous call.

Arguments mapping described in
[DeleteLoggingConfigurationRequestRequestTypeDef](./type_defs.md#deleteloggingconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_permission_policy"></a>

### delete_permission_policy

.

Type annotations for `session.create_client("waf").delete_permission_policy`
method.

Boto3 documentation:
[WAF.Client.delete_permission_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_permission_policy)

Asynchronous method. Use `await delete_permission_policy(...)` for a
synchronous call.

Arguments mapping described in
[DeletePermissionPolicyRequestRequestTypeDef](./type_defs.md#deletepermissionpolicyrequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_rate_based_rule"></a>

### delete_rate_based_rule

.

Type annotations for `session.create_client("waf").delete_rate_based_rule`
method.

Boto3 documentation:
[WAF.Client.delete_rate_based_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_rate_based_rule)

Asynchronous method. Use `await delete_rate_based_rule(...)` for a synchronous
call.

Arguments mapping described in
[DeleteRateBasedRuleRequestRequestTypeDef](./type_defs.md#deleteratebasedrulerequestrequesttypedef).

Keyword-only arguments:

- `RuleId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[DeleteRateBasedRuleResponseTypeDef](./type_defs.md#deleteratebasedruleresponsetypedef).

<a id="delete_regex_match_set"></a>

### delete_regex_match_set

.

Type annotations for `session.create_client("waf").delete_regex_match_set`
method.

Boto3 documentation:
[WAF.Client.delete_regex_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_regex_match_set)

Asynchronous method. Use `await delete_regex_match_set(...)` for a synchronous
call.

Arguments mapping described in
[DeleteRegexMatchSetRequestRequestTypeDef](./type_defs.md#deleteregexmatchsetrequestrequesttypedef).

Keyword-only arguments:

- `RegexMatchSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[DeleteRegexMatchSetResponseTypeDef](./type_defs.md#deleteregexmatchsetresponsetypedef).

<a id="delete_regex_pattern_set"></a>

### delete_regex_pattern_set

.

Type annotations for `session.create_client("waf").delete_regex_pattern_set`
method.

Boto3 documentation:
[WAF.Client.delete_regex_pattern_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_regex_pattern_set)

Asynchronous method. Use `await delete_regex_pattern_set(...)` for a
synchronous call.

Arguments mapping described in
[DeleteRegexPatternSetRequestRequestTypeDef](./type_defs.md#deleteregexpatternsetrequestrequesttypedef).

Keyword-only arguments:

- `RegexPatternSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[DeleteRegexPatternSetResponseTypeDef](./type_defs.md#deleteregexpatternsetresponsetypedef).

<a id="delete_rule"></a>

### delete_rule

.

Type annotations for `session.create_client("waf").delete_rule` method.

Boto3 documentation:
[WAF.Client.delete_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_rule)

Asynchronous method. Use `await delete_rule(...)` for a synchronous call.

Arguments mapping described in
[DeleteRuleRequestRequestTypeDef](./type_defs.md#deleterulerequestrequesttypedef).

Keyword-only arguments:

- `RuleId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[DeleteRuleResponseTypeDef](./type_defs.md#deleteruleresponsetypedef).

<a id="delete_rule_group"></a>

### delete_rule_group

.

Type annotations for `session.create_client("waf").delete_rule_group` method.

Boto3 documentation:
[WAF.Client.delete_rule_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_rule_group)

Asynchronous method. Use `await delete_rule_group(...)` for a synchronous call.

Arguments mapping described in
[DeleteRuleGroupRequestRequestTypeDef](./type_defs.md#deleterulegrouprequestrequesttypedef).

Keyword-only arguments:

- `RuleGroupId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[DeleteRuleGroupResponseTypeDef](./type_defs.md#deleterulegroupresponsetypedef).

<a id="delete_size_constraint_set"></a>

### delete_size_constraint_set

.

Type annotations for `session.create_client("waf").delete_size_constraint_set`
method.

Boto3 documentation:
[WAF.Client.delete_size_constraint_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_size_constraint_set)

Asynchronous method. Use `await delete_size_constraint_set(...)` for a
synchronous call.

Arguments mapping described in
[DeleteSizeConstraintSetRequestRequestTypeDef](./type_defs.md#deletesizeconstraintsetrequestrequesttypedef).

Keyword-only arguments:

- `SizeConstraintSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[DeleteSizeConstraintSetResponseTypeDef](./type_defs.md#deletesizeconstraintsetresponsetypedef).

<a id="delete_sql_injection_match_set"></a>

### delete_sql_injection_match_set

.

Type annotations for
`session.create_client("waf").delete_sql_injection_match_set` method.

Boto3 documentation:
[WAF.Client.delete_sql_injection_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_sql_injection_match_set)

Asynchronous method. Use `await delete_sql_injection_match_set(...)` for a
synchronous call.

Arguments mapping described in
[DeleteSqlInjectionMatchSetRequestRequestTypeDef](./type_defs.md#deletesqlinjectionmatchsetrequestrequesttypedef).

Keyword-only arguments:

- `SqlInjectionMatchSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[DeleteSqlInjectionMatchSetResponseTypeDef](./type_defs.md#deletesqlinjectionmatchsetresponsetypedef).

<a id="delete_web_acl"></a>

### delete_web_acl

.

Type annotations for `session.create_client("waf").delete_web_acl` method.

Boto3 documentation:
[WAF.Client.delete_web_acl](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_web_acl)

Asynchronous method. Use `await delete_web_acl(...)` for a synchronous call.

Arguments mapping described in
[DeleteWebACLRequestRequestTypeDef](./type_defs.md#deletewebaclrequestrequesttypedef).

Keyword-only arguments:

- `WebACLId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[DeleteWebACLResponseTypeDef](./type_defs.md#deletewebaclresponsetypedef).

<a id="delete_xss_match_set"></a>

### delete_xss_match_set

.

Type annotations for `session.create_client("waf").delete_xss_match_set`
method.

Boto3 documentation:
[WAF.Client.delete_xss_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.delete_xss_match_set)

Asynchronous method. Use `await delete_xss_match_set(...)` for a synchronous
call.

Arguments mapping described in
[DeleteXssMatchSetRequestRequestTypeDef](./type_defs.md#deletexssmatchsetrequestrequesttypedef).

Keyword-only arguments:

- `XssMatchSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[DeleteXssMatchSetResponseTypeDef](./type_defs.md#deletexssmatchsetresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("waf").generate_presigned_url`
method.

Boto3 documentation:
[WAF.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_byte_match_set"></a>

### get_byte_match_set

.

Type annotations for `session.create_client("waf").get_byte_match_set` method.

Boto3 documentation:
[WAF.Client.get_byte_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_byte_match_set)

Asynchronous method. Use `await get_byte_match_set(...)` for a synchronous
call.

Arguments mapping described in
[GetByteMatchSetRequestRequestTypeDef](./type_defs.md#getbytematchsetrequestrequesttypedef).

Keyword-only arguments:

- `ByteMatchSetId`: `str` *(required)*

Returns a `Coroutine` for
[GetByteMatchSetResponseTypeDef](./type_defs.md#getbytematchsetresponsetypedef).

<a id="get_change_token"></a>

### get_change_token

.

Type annotations for `session.create_client("waf").get_change_token` method.

Boto3 documentation:
[WAF.Client.get_change_token](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_change_token)

Asynchronous method. Use `await get_change_token(...)` for a synchronous call.

Returns a `Coroutine` for
[GetChangeTokenResponseTypeDef](./type_defs.md#getchangetokenresponsetypedef).

<a id="get_change_token_status"></a>

### get_change_token_status

.

Type annotations for `session.create_client("waf").get_change_token_status`
method.

Boto3 documentation:
[WAF.Client.get_change_token_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_change_token_status)

Asynchronous method. Use `await get_change_token_status(...)` for a synchronous
call.

Arguments mapping described in
[GetChangeTokenStatusRequestRequestTypeDef](./type_defs.md#getchangetokenstatusrequestrequesttypedef).

Keyword-only arguments:

- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[GetChangeTokenStatusResponseTypeDef](./type_defs.md#getchangetokenstatusresponsetypedef).

<a id="get_geo_match_set"></a>

### get_geo_match_set

.

Type annotations for `session.create_client("waf").get_geo_match_set` method.

Boto3 documentation:
[WAF.Client.get_geo_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_geo_match_set)

Asynchronous method. Use `await get_geo_match_set(...)` for a synchronous call.

Arguments mapping described in
[GetGeoMatchSetRequestRequestTypeDef](./type_defs.md#getgeomatchsetrequestrequesttypedef).

Keyword-only arguments:

- `GeoMatchSetId`: `str` *(required)*

Returns a `Coroutine` for
[GetGeoMatchSetResponseTypeDef](./type_defs.md#getgeomatchsetresponsetypedef).

<a id="get_ip_set"></a>

### get_ip_set

.

Type annotations for `session.create_client("waf").get_ip_set` method.

Boto3 documentation:
[WAF.Client.get_ip_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_ip_set)

Asynchronous method. Use `await get_ip_set(...)` for a synchronous call.

Arguments mapping described in
[GetIPSetRequestRequestTypeDef](./type_defs.md#getipsetrequestrequesttypedef).

Keyword-only arguments:

- `IPSetId`: `str` *(required)*

Returns a `Coroutine` for
[GetIPSetResponseTypeDef](./type_defs.md#getipsetresponsetypedef).

<a id="get_logging_configuration"></a>

### get_logging_configuration

.

Type annotations for `session.create_client("waf").get_logging_configuration`
method.

Boto3 documentation:
[WAF.Client.get_logging_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_logging_configuration)

Asynchronous method. Use `await get_logging_configuration(...)` for a
synchronous call.

Arguments mapping described in
[GetLoggingConfigurationRequestRequestTypeDef](./type_defs.md#getloggingconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[GetLoggingConfigurationResponseTypeDef](./type_defs.md#getloggingconfigurationresponsetypedef).

<a id="get_permission_policy"></a>

### get_permission_policy

.

Type annotations for `session.create_client("waf").get_permission_policy`
method.

Boto3 documentation:
[WAF.Client.get_permission_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_permission_policy)

Asynchronous method. Use `await get_permission_policy(...)` for a synchronous
call.

Arguments mapping described in
[GetPermissionPolicyRequestRequestTypeDef](./type_defs.md#getpermissionpolicyrequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[GetPermissionPolicyResponseTypeDef](./type_defs.md#getpermissionpolicyresponsetypedef).

<a id="get_rate_based_rule"></a>

### get_rate_based_rule

.

Type annotations for `session.create_client("waf").get_rate_based_rule` method.

Boto3 documentation:
[WAF.Client.get_rate_based_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_rate_based_rule)

Asynchronous method. Use `await get_rate_based_rule(...)` for a synchronous
call.

Arguments mapping described in
[GetRateBasedRuleRequestRequestTypeDef](./type_defs.md#getratebasedrulerequestrequesttypedef).

Keyword-only arguments:

- `RuleId`: `str` *(required)*

Returns a `Coroutine` for
[GetRateBasedRuleResponseTypeDef](./type_defs.md#getratebasedruleresponsetypedef).

<a id="get_rate_based_rule_managed_keys"></a>

### get_rate_based_rule_managed_keys

.

Type annotations for
`session.create_client("waf").get_rate_based_rule_managed_keys` method.

Boto3 documentation:
[WAF.Client.get_rate_based_rule_managed_keys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_rate_based_rule_managed_keys)

Asynchronous method. Use `await get_rate_based_rule_managed_keys(...)` for a
synchronous call.

Arguments mapping described in
[GetRateBasedRuleManagedKeysRequestRequestTypeDef](./type_defs.md#getratebasedrulemanagedkeysrequestrequesttypedef).

Keyword-only arguments:

- `RuleId`: `str` *(required)*
- `NextMarker`: `str`

Returns a `Coroutine` for
[GetRateBasedRuleManagedKeysResponseTypeDef](./type_defs.md#getratebasedrulemanagedkeysresponsetypedef).

<a id="get_regex_match_set"></a>

### get_regex_match_set

.

Type annotations for `session.create_client("waf").get_regex_match_set` method.

Boto3 documentation:
[WAF.Client.get_regex_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_regex_match_set)

Asynchronous method. Use `await get_regex_match_set(...)` for a synchronous
call.

Arguments mapping described in
[GetRegexMatchSetRequestRequestTypeDef](./type_defs.md#getregexmatchsetrequestrequesttypedef).

Keyword-only arguments:

- `RegexMatchSetId`: `str` *(required)*

Returns a `Coroutine` for
[GetRegexMatchSetResponseTypeDef](./type_defs.md#getregexmatchsetresponsetypedef).

<a id="get_regex_pattern_set"></a>

### get_regex_pattern_set

.

Type annotations for `session.create_client("waf").get_regex_pattern_set`
method.

Boto3 documentation:
[WAF.Client.get_regex_pattern_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_regex_pattern_set)

Asynchronous method. Use `await get_regex_pattern_set(...)` for a synchronous
call.

Arguments mapping described in
[GetRegexPatternSetRequestRequestTypeDef](./type_defs.md#getregexpatternsetrequestrequesttypedef).

Keyword-only arguments:

- `RegexPatternSetId`: `str` *(required)*

Returns a `Coroutine` for
[GetRegexPatternSetResponseTypeDef](./type_defs.md#getregexpatternsetresponsetypedef).

<a id="get_rule"></a>

### get_rule

.

Type annotations for `session.create_client("waf").get_rule` method.

Boto3 documentation:
[WAF.Client.get_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_rule)

Asynchronous method. Use `await get_rule(...)` for a synchronous call.

Arguments mapping described in
[GetRuleRequestRequestTypeDef](./type_defs.md#getrulerequestrequesttypedef).

Keyword-only arguments:

- `RuleId`: `str` *(required)*

Returns a `Coroutine` for
[GetRuleResponseTypeDef](./type_defs.md#getruleresponsetypedef).

<a id="get_rule_group"></a>

### get_rule_group

.

Type annotations for `session.create_client("waf").get_rule_group` method.

Boto3 documentation:
[WAF.Client.get_rule_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_rule_group)

Asynchronous method. Use `await get_rule_group(...)` for a synchronous call.

Arguments mapping described in
[GetRuleGroupRequestRequestTypeDef](./type_defs.md#getrulegrouprequestrequesttypedef).

Keyword-only arguments:

- `RuleGroupId`: `str` *(required)*

Returns a `Coroutine` for
[GetRuleGroupResponseTypeDef](./type_defs.md#getrulegroupresponsetypedef).

<a id="get_sampled_requests"></a>

### get_sampled_requests

.

Type annotations for `session.create_client("waf").get_sampled_requests`
method.

Boto3 documentation:
[WAF.Client.get_sampled_requests](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_sampled_requests)

Asynchronous method. Use `await get_sampled_requests(...)` for a synchronous
call.

Arguments mapping described in
[GetSampledRequestsRequestRequestTypeDef](./type_defs.md#getsampledrequestsrequestrequesttypedef).

Keyword-only arguments:

- `WebAclId`: `str` *(required)*
- `RuleId`: `str` *(required)*
- `TimeWindow`: [TimeWindowTypeDef](./type_defs.md#timewindowtypedef)
  *(required)*
- `MaxItems`: `int` *(required)*

Returns a `Coroutine` for
[GetSampledRequestsResponseTypeDef](./type_defs.md#getsampledrequestsresponsetypedef).

<a id="get_size_constraint_set"></a>

### get_size_constraint_set

.

Type annotations for `session.create_client("waf").get_size_constraint_set`
method.

Boto3 documentation:
[WAF.Client.get_size_constraint_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_size_constraint_set)

Asynchronous method. Use `await get_size_constraint_set(...)` for a synchronous
call.

Arguments mapping described in
[GetSizeConstraintSetRequestRequestTypeDef](./type_defs.md#getsizeconstraintsetrequestrequesttypedef).

Keyword-only arguments:

- `SizeConstraintSetId`: `str` *(required)*

Returns a `Coroutine` for
[GetSizeConstraintSetResponseTypeDef](./type_defs.md#getsizeconstraintsetresponsetypedef).

<a id="get_sql_injection_match_set"></a>

### get_sql_injection_match_set

.

Type annotations for `session.create_client("waf").get_sql_injection_match_set`
method.

Boto3 documentation:
[WAF.Client.get_sql_injection_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_sql_injection_match_set)

Asynchronous method. Use `await get_sql_injection_match_set(...)` for a
synchronous call.

Arguments mapping described in
[GetSqlInjectionMatchSetRequestRequestTypeDef](./type_defs.md#getsqlinjectionmatchsetrequestrequesttypedef).

Keyword-only arguments:

- `SqlInjectionMatchSetId`: `str` *(required)*

Returns a `Coroutine` for
[GetSqlInjectionMatchSetResponseTypeDef](./type_defs.md#getsqlinjectionmatchsetresponsetypedef).

<a id="get_web_acl"></a>

### get_web_acl

.

Type annotations for `session.create_client("waf").get_web_acl` method.

Boto3 documentation:
[WAF.Client.get_web_acl](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_web_acl)

Asynchronous method. Use `await get_web_acl(...)` for a synchronous call.

Arguments mapping described in
[GetWebACLRequestRequestTypeDef](./type_defs.md#getwebaclrequestrequesttypedef).

Keyword-only arguments:

- `WebACLId`: `str` *(required)*

Returns a `Coroutine` for
[GetWebACLResponseTypeDef](./type_defs.md#getwebaclresponsetypedef).

<a id="get_xss_match_set"></a>

### get_xss_match_set

.

Type annotations for `session.create_client("waf").get_xss_match_set` method.

Boto3 documentation:
[WAF.Client.get_xss_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_xss_match_set)

Asynchronous method. Use `await get_xss_match_set(...)` for a synchronous call.

Arguments mapping described in
[GetXssMatchSetRequestRequestTypeDef](./type_defs.md#getxssmatchsetrequestrequesttypedef).

Keyword-only arguments:

- `XssMatchSetId`: `str` *(required)*

Returns a `Coroutine` for
[GetXssMatchSetResponseTypeDef](./type_defs.md#getxssmatchsetresponsetypedef).

<a id="list_activated_rules_in_rule_group"></a>

### list_activated_rules_in_rule_group

.

Type annotations for
`session.create_client("waf").list_activated_rules_in_rule_group` method.

Boto3 documentation:
[WAF.Client.list_activated_rules_in_rule_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_activated_rules_in_rule_group)

Asynchronous method. Use `await list_activated_rules_in_rule_group(...)` for a
synchronous call.

Arguments mapping described in
[ListActivatedRulesInRuleGroupRequestRequestTypeDef](./type_defs.md#listactivatedrulesinrulegrouprequestrequesttypedef).

Keyword-only arguments:

- `RuleGroupId`: `str`
- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListActivatedRulesInRuleGroupResponseTypeDef](./type_defs.md#listactivatedrulesinrulegroupresponsetypedef).

<a id="list_byte_match_sets"></a>

### list_byte_match_sets

.

Type annotations for `session.create_client("waf").list_byte_match_sets`
method.

Boto3 documentation:
[WAF.Client.list_byte_match_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_byte_match_sets)

Asynchronous method. Use `await list_byte_match_sets(...)` for a synchronous
call.

Arguments mapping described in
[ListByteMatchSetsRequestRequestTypeDef](./type_defs.md#listbytematchsetsrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListByteMatchSetsResponseTypeDef](./type_defs.md#listbytematchsetsresponsetypedef).

<a id="list_geo_match_sets"></a>

### list_geo_match_sets

.

Type annotations for `session.create_client("waf").list_geo_match_sets` method.

Boto3 documentation:
[WAF.Client.list_geo_match_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_geo_match_sets)

Asynchronous method. Use `await list_geo_match_sets(...)` for a synchronous
call.

Arguments mapping described in
[ListGeoMatchSetsRequestRequestTypeDef](./type_defs.md#listgeomatchsetsrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListGeoMatchSetsResponseTypeDef](./type_defs.md#listgeomatchsetsresponsetypedef).

<a id="list_ip_sets"></a>

### list_ip_sets

.

Type annotations for `session.create_client("waf").list_ip_sets` method.

Boto3 documentation:
[WAF.Client.list_ip_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_ip_sets)

Asynchronous method. Use `await list_ip_sets(...)` for a synchronous call.

Arguments mapping described in
[ListIPSetsRequestRequestTypeDef](./type_defs.md#listipsetsrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef).

<a id="list_logging_configurations"></a>

### list_logging_configurations

.

Type annotations for `session.create_client("waf").list_logging_configurations`
method.

Boto3 documentation:
[WAF.Client.list_logging_configurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_logging_configurations)

Asynchronous method. Use `await list_logging_configurations(...)` for a
synchronous call.

Arguments mapping described in
[ListLoggingConfigurationsRequestRequestTypeDef](./type_defs.md#listloggingconfigurationsrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListLoggingConfigurationsResponseTypeDef](./type_defs.md#listloggingconfigurationsresponsetypedef).

<a id="list_rate_based_rules"></a>

### list_rate_based_rules

.

Type annotations for `session.create_client("waf").list_rate_based_rules`
method.

Boto3 documentation:
[WAF.Client.list_rate_based_rules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_rate_based_rules)

Asynchronous method. Use `await list_rate_based_rules(...)` for a synchronous
call.

Arguments mapping described in
[ListRateBasedRulesRequestRequestTypeDef](./type_defs.md#listratebasedrulesrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListRateBasedRulesResponseTypeDef](./type_defs.md#listratebasedrulesresponsetypedef).

<a id="list_regex_match_sets"></a>

### list_regex_match_sets

.

Type annotations for `session.create_client("waf").list_regex_match_sets`
method.

Boto3 documentation:
[WAF.Client.list_regex_match_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_regex_match_sets)

Asynchronous method. Use `await list_regex_match_sets(...)` for a synchronous
call.

Arguments mapping described in
[ListRegexMatchSetsRequestRequestTypeDef](./type_defs.md#listregexmatchsetsrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListRegexMatchSetsResponseTypeDef](./type_defs.md#listregexmatchsetsresponsetypedef).

<a id="list_regex_pattern_sets"></a>

### list_regex_pattern_sets

.

Type annotations for `session.create_client("waf").list_regex_pattern_sets`
method.

Boto3 documentation:
[WAF.Client.list_regex_pattern_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_regex_pattern_sets)

Asynchronous method. Use `await list_regex_pattern_sets(...)` for a synchronous
call.

Arguments mapping described in
[ListRegexPatternSetsRequestRequestTypeDef](./type_defs.md#listregexpatternsetsrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListRegexPatternSetsResponseTypeDef](./type_defs.md#listregexpatternsetsresponsetypedef).

<a id="list_rule_groups"></a>

### list_rule_groups

.

Type annotations for `session.create_client("waf").list_rule_groups` method.

Boto3 documentation:
[WAF.Client.list_rule_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_rule_groups)

Asynchronous method. Use `await list_rule_groups(...)` for a synchronous call.

Arguments mapping described in
[ListRuleGroupsRequestRequestTypeDef](./type_defs.md#listrulegroupsrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListRuleGroupsResponseTypeDef](./type_defs.md#listrulegroupsresponsetypedef).

<a id="list_rules"></a>

### list_rules

.

Type annotations for `session.create_client("waf").list_rules` method.

Boto3 documentation:
[WAF.Client.list_rules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_rules)

Asynchronous method. Use `await list_rules(...)` for a synchronous call.

Arguments mapping described in
[ListRulesRequestRequestTypeDef](./type_defs.md#listrulesrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef).

<a id="list_size_constraint_sets"></a>

### list_size_constraint_sets

.

Type annotations for `session.create_client("waf").list_size_constraint_sets`
method.

Boto3 documentation:
[WAF.Client.list_size_constraint_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_size_constraint_sets)

Asynchronous method. Use `await list_size_constraint_sets(...)` for a
synchronous call.

Arguments mapping described in
[ListSizeConstraintSetsRequestRequestTypeDef](./type_defs.md#listsizeconstraintsetsrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListSizeConstraintSetsResponseTypeDef](./type_defs.md#listsizeconstraintsetsresponsetypedef).

<a id="list_sql_injection_match_sets"></a>

### list_sql_injection_match_sets

.

Type annotations for
`session.create_client("waf").list_sql_injection_match_sets` method.

Boto3 documentation:
[WAF.Client.list_sql_injection_match_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_sql_injection_match_sets)

Asynchronous method. Use `await list_sql_injection_match_sets(...)` for a
synchronous call.

Arguments mapping described in
[ListSqlInjectionMatchSetsRequestRequestTypeDef](./type_defs.md#listsqlinjectionmatchsetsrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListSqlInjectionMatchSetsResponseTypeDef](./type_defs.md#listsqlinjectionmatchsetsresponsetypedef).

<a id="list_subscribed_rule_groups"></a>

### list_subscribed_rule_groups

.

Type annotations for `session.create_client("waf").list_subscribed_rule_groups`
method.

Boto3 documentation:
[WAF.Client.list_subscribed_rule_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_subscribed_rule_groups)

Asynchronous method. Use `await list_subscribed_rule_groups(...)` for a
synchronous call.

Arguments mapping described in
[ListSubscribedRuleGroupsRequestRequestTypeDef](./type_defs.md#listsubscribedrulegroupsrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListSubscribedRuleGroupsResponseTypeDef](./type_defs.md#listsubscribedrulegroupsresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

.

Type annotations for `session.create_client("waf").list_tags_for_resource`
method.

Boto3 documentation:
[WAF.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="list_web_acls"></a>

### list_web_acls

.

Type annotations for `session.create_client("waf").list_web_acls` method.

Boto3 documentation:
[WAF.Client.list_web_acls](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_web_acls)

Asynchronous method. Use `await list_web_acls(...)` for a synchronous call.

Arguments mapping described in
[ListWebACLsRequestRequestTypeDef](./type_defs.md#listwebaclsrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListWebACLsResponseTypeDef](./type_defs.md#listwebaclsresponsetypedef).

<a id="list_xss_match_sets"></a>

### list_xss_match_sets

.

Type annotations for `session.create_client("waf").list_xss_match_sets` method.

Boto3 documentation:
[WAF.Client.list_xss_match_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_xss_match_sets)

Asynchronous method. Use `await list_xss_match_sets(...)` for a synchronous
call.

Arguments mapping described in
[ListXssMatchSetsRequestRequestTypeDef](./type_defs.md#listxssmatchsetsrequestrequesttypedef).

Keyword-only arguments:

- `NextMarker`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListXssMatchSetsResponseTypeDef](./type_defs.md#listxssmatchsetsresponsetypedef).

<a id="put_logging_configuration"></a>

### put_logging_configuration

.

Type annotations for `session.create_client("waf").put_logging_configuration`
method.

Boto3 documentation:
[WAF.Client.put_logging_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.put_logging_configuration)

Asynchronous method. Use `await put_logging_configuration(...)` for a
synchronous call.

Arguments mapping described in
[PutLoggingConfigurationRequestRequestTypeDef](./type_defs.md#putloggingconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `LoggingConfiguration`:
  [LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef)
  *(required)*

Returns a `Coroutine` for
[PutLoggingConfigurationResponseTypeDef](./type_defs.md#putloggingconfigurationresponsetypedef).

<a id="put_permission_policy"></a>

### put_permission_policy

.

Type annotations for `session.create_client("waf").put_permission_policy`
method.

Boto3 documentation:
[WAF.Client.put_permission_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.put_permission_policy)

Asynchronous method. Use `await put_permission_policy(...)` for a synchronous
call.

Arguments mapping described in
[PutPermissionPolicyRequestRequestTypeDef](./type_defs.md#putpermissionpolicyrequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Policy`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="tag_resource"></a>

### tag_resource

.

Type annotations for `session.create_client("waf").tag_resource` method.

Boto3 documentation:
[WAF.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

.

Type annotations for `session.create_client("waf").untag_resource` method.

Boto3 documentation:
[WAF.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_byte_match_set"></a>

### update_byte_match_set

.

Type annotations for `session.create_client("waf").update_byte_match_set`
method.

Boto3 documentation:
[WAF.Client.update_byte_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_byte_match_set)

Asynchronous method. Use `await update_byte_match_set(...)` for a synchronous
call.

Arguments mapping described in
[UpdateByteMatchSetRequestRequestTypeDef](./type_defs.md#updatebytematchsetrequestrequesttypedef).

Keyword-only arguments:

- `ByteMatchSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*
- `Updates`:
  `Sequence`\[[ByteMatchSetUpdateTypeDef](./type_defs.md#bytematchsetupdatetypedef)\]
  *(required)*

Returns a `Coroutine` for
[UpdateByteMatchSetResponseTypeDef](./type_defs.md#updatebytematchsetresponsetypedef).

<a id="update_geo_match_set"></a>

### update_geo_match_set

.

Type annotations for `session.create_client("waf").update_geo_match_set`
method.

Boto3 documentation:
[WAF.Client.update_geo_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_geo_match_set)

Asynchronous method. Use `await update_geo_match_set(...)` for a synchronous
call.

Arguments mapping described in
[UpdateGeoMatchSetRequestRequestTypeDef](./type_defs.md#updategeomatchsetrequestrequesttypedef).

Keyword-only arguments:

- `GeoMatchSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*
- `Updates`:
  `Sequence`\[[GeoMatchSetUpdateTypeDef](./type_defs.md#geomatchsetupdatetypedef)\]
  *(required)*

Returns a `Coroutine` for
[UpdateGeoMatchSetResponseTypeDef](./type_defs.md#updategeomatchsetresponsetypedef).

<a id="update_ip_set"></a>

### update_ip_set

.

Type annotations for `session.create_client("waf").update_ip_set` method.

Boto3 documentation:
[WAF.Client.update_ip_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_ip_set)

Asynchronous method. Use `await update_ip_set(...)` for a synchronous call.

Arguments mapping described in
[UpdateIPSetRequestRequestTypeDef](./type_defs.md#updateipsetrequestrequesttypedef).

Keyword-only arguments:

- `IPSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*
- `Updates`:
  `Sequence`\[[IPSetUpdateTypeDef](./type_defs.md#ipsetupdatetypedef)\]
  *(required)*

Returns a `Coroutine` for
[UpdateIPSetResponseTypeDef](./type_defs.md#updateipsetresponsetypedef).

<a id="update_rate_based_rule"></a>

### update_rate_based_rule

.

Type annotations for `session.create_client("waf").update_rate_based_rule`
method.

Boto3 documentation:
[WAF.Client.update_rate_based_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_rate_based_rule)

Asynchronous method. Use `await update_rate_based_rule(...)` for a synchronous
call.

Arguments mapping described in
[UpdateRateBasedRuleRequestRequestTypeDef](./type_defs.md#updateratebasedrulerequestrequesttypedef).

Keyword-only arguments:

- `RuleId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*
- `Updates`:
  `Sequence`\[[RuleUpdateTypeDef](./type_defs.md#ruleupdatetypedef)\]
  *(required)*
- `RateLimit`: `int` *(required)*

Returns a `Coroutine` for
[UpdateRateBasedRuleResponseTypeDef](./type_defs.md#updateratebasedruleresponsetypedef).

<a id="update_regex_match_set"></a>

### update_regex_match_set

.

Type annotations for `session.create_client("waf").update_regex_match_set`
method.

Boto3 documentation:
[WAF.Client.update_regex_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_regex_match_set)

Asynchronous method. Use `await update_regex_match_set(...)` for a synchronous
call.

Arguments mapping described in
[UpdateRegexMatchSetRequestRequestTypeDef](./type_defs.md#updateregexmatchsetrequestrequesttypedef).

Keyword-only arguments:

- `RegexMatchSetId`: `str` *(required)*
- `Updates`:
  `Sequence`\[[RegexMatchSetUpdateTypeDef](./type_defs.md#regexmatchsetupdatetypedef)\]
  *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[UpdateRegexMatchSetResponseTypeDef](./type_defs.md#updateregexmatchsetresponsetypedef).

<a id="update_regex_pattern_set"></a>

### update_regex_pattern_set

.

Type annotations for `session.create_client("waf").update_regex_pattern_set`
method.

Boto3 documentation:
[WAF.Client.update_regex_pattern_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_regex_pattern_set)

Asynchronous method. Use `await update_regex_pattern_set(...)` for a
synchronous call.

Arguments mapping described in
[UpdateRegexPatternSetRequestRequestTypeDef](./type_defs.md#updateregexpatternsetrequestrequesttypedef).

Keyword-only arguments:

- `RegexPatternSetId`: `str` *(required)*
- `Updates`:
  `Sequence`\[[RegexPatternSetUpdateTypeDef](./type_defs.md#regexpatternsetupdatetypedef)\]
  *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[UpdateRegexPatternSetResponseTypeDef](./type_defs.md#updateregexpatternsetresponsetypedef).

<a id="update_rule"></a>

### update_rule

.

Type annotations for `session.create_client("waf").update_rule` method.

Boto3 documentation:
[WAF.Client.update_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_rule)

Asynchronous method. Use `await update_rule(...)` for a synchronous call.

Arguments mapping described in
[UpdateRuleRequestRequestTypeDef](./type_defs.md#updaterulerequestrequesttypedef).

Keyword-only arguments:

- `RuleId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*
- `Updates`:
  `Sequence`\[[RuleUpdateTypeDef](./type_defs.md#ruleupdatetypedef)\]
  *(required)*

Returns a `Coroutine` for
[UpdateRuleResponseTypeDef](./type_defs.md#updateruleresponsetypedef).

<a id="update_rule_group"></a>

### update_rule_group

.

Type annotations for `session.create_client("waf").update_rule_group` method.

Boto3 documentation:
[WAF.Client.update_rule_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_rule_group)

Asynchronous method. Use `await update_rule_group(...)` for a synchronous call.

Arguments mapping described in
[UpdateRuleGroupRequestRequestTypeDef](./type_defs.md#updaterulegrouprequestrequesttypedef).

Keyword-only arguments:

- `RuleGroupId`: `str` *(required)*
- `Updates`:
  `Sequence`\[[RuleGroupUpdateTypeDef](./type_defs.md#rulegroupupdatetypedef)\]
  *(required)*
- `ChangeToken`: `str` *(required)*

Returns a `Coroutine` for
[UpdateRuleGroupResponseTypeDef](./type_defs.md#updaterulegroupresponsetypedef).

<a id="update_size_constraint_set"></a>

### update_size_constraint_set

.

Type annotations for `session.create_client("waf").update_size_constraint_set`
method.

Boto3 documentation:
[WAF.Client.update_size_constraint_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_size_constraint_set)

Asynchronous method. Use `await update_size_constraint_set(...)` for a
synchronous call.

Arguments mapping described in
[UpdateSizeConstraintSetRequestRequestTypeDef](./type_defs.md#updatesizeconstraintsetrequestrequesttypedef).

Keyword-only arguments:

- `SizeConstraintSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*
- `Updates`:
  `Sequence`\[[SizeConstraintSetUpdateTypeDef](./type_defs.md#sizeconstraintsetupdatetypedef)\]
  *(required)*

Returns a `Coroutine` for
[UpdateSizeConstraintSetResponseTypeDef](./type_defs.md#updatesizeconstraintsetresponsetypedef).

<a id="update_sql_injection_match_set"></a>

### update_sql_injection_match_set

.

Type annotations for
`session.create_client("waf").update_sql_injection_match_set` method.

Boto3 documentation:
[WAF.Client.update_sql_injection_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_sql_injection_match_set)

Asynchronous method. Use `await update_sql_injection_match_set(...)` for a
synchronous call.

Arguments mapping described in
[UpdateSqlInjectionMatchSetRequestRequestTypeDef](./type_defs.md#updatesqlinjectionmatchsetrequestrequesttypedef).

Keyword-only arguments:

- `SqlInjectionMatchSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*
- `Updates`:
  `Sequence`\[[SqlInjectionMatchSetUpdateTypeDef](./type_defs.md#sqlinjectionmatchsetupdatetypedef)\]
  *(required)*

Returns a `Coroutine` for
[UpdateSqlInjectionMatchSetResponseTypeDef](./type_defs.md#updatesqlinjectionmatchsetresponsetypedef).

<a id="update_web_acl"></a>

### update_web_acl

.

Type annotations for `session.create_client("waf").update_web_acl` method.

Boto3 documentation:
[WAF.Client.update_web_acl](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_web_acl)

Asynchronous method. Use `await update_web_acl(...)` for a synchronous call.

Arguments mapping described in
[UpdateWebACLRequestRequestTypeDef](./type_defs.md#updatewebaclrequestrequesttypedef).

Keyword-only arguments:

- `WebACLId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*
- `Updates`:
  `Sequence`\[[WebACLUpdateTypeDef](./type_defs.md#webaclupdatetypedef)\]
- `DefaultAction`: [WafActionTypeDef](./type_defs.md#wafactiontypedef)

Returns a `Coroutine` for
[UpdateWebACLResponseTypeDef](./type_defs.md#updatewebaclresponsetypedef).

<a id="update_xss_match_set"></a>

### update_xss_match_set

.

Type annotations for `session.create_client("waf").update_xss_match_set`
method.

Boto3 documentation:
[WAF.Client.update_xss_match_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_xss_match_set)

Asynchronous method. Use `await update_xss_match_set(...)` for a synchronous
call.

Arguments mapping described in
[UpdateXssMatchSetRequestRequestTypeDef](./type_defs.md#updatexssmatchsetrequestrequesttypedef).

Keyword-only arguments:

- `XssMatchSetId`: `str` *(required)*
- `ChangeToken`: `str` *(required)*
- `Updates`:
  `Sequence`\[[XssMatchSetUpdateTypeDef](./type_defs.md#xssmatchsetupdatetypedef)\]
  *(required)*

Returns a `Coroutine` for
[UpdateXssMatchSetResponseTypeDef](./type_defs.md#updatexssmatchsetresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("waf").__aenter__` method.

Boto3 documentation:
[WAF.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [WAFClient](#wafclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("waf").__aexit__` method.

Boto3 documentation:
[WAF.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("waf").get_paginator` method with
overloads.

- `client.get_paginator("get_rate_based_rule_managed_keys")` ->
  [GetRateBasedRuleManagedKeysPaginator](./paginators.md#getratebasedrulemanagedkeyspaginator)
- `client.get_paginator("list_activated_rules_in_rule_group")` ->
  [ListActivatedRulesInRuleGroupPaginator](./paginators.md#listactivatedrulesinrulegrouppaginator)
- `client.get_paginator("list_byte_match_sets")` ->
  [ListByteMatchSetsPaginator](./paginators.md#listbytematchsetspaginator)
- `client.get_paginator("list_geo_match_sets")` ->
  [ListGeoMatchSetsPaginator](./paginators.md#listgeomatchsetspaginator)
- `client.get_paginator("list_ip_sets")` ->
  [ListIPSetsPaginator](./paginators.md#listipsetspaginator)
- `client.get_paginator("list_logging_configurations")` ->
  [ListLoggingConfigurationsPaginator](./paginators.md#listloggingconfigurationspaginator)
- `client.get_paginator("list_rate_based_rules")` ->
  [ListRateBasedRulesPaginator](./paginators.md#listratebasedrulespaginator)
- `client.get_paginator("list_regex_match_sets")` ->
  [ListRegexMatchSetsPaginator](./paginators.md#listregexmatchsetspaginator)
- `client.get_paginator("list_regex_pattern_sets")` ->
  [ListRegexPatternSetsPaginator](./paginators.md#listregexpatternsetspaginator)
- `client.get_paginator("list_rule_groups")` ->
  [ListRuleGroupsPaginator](./paginators.md#listrulegroupspaginator)
- `client.get_paginator("list_rules")` ->
  [ListRulesPaginator](./paginators.md#listrulespaginator)
- `client.get_paginator("list_size_constraint_sets")` ->
  [ListSizeConstraintSetsPaginator](./paginators.md#listsizeconstraintsetspaginator)
- `client.get_paginator("list_sql_injection_match_sets")` ->
  [ListSqlInjectionMatchSetsPaginator](./paginators.md#listsqlinjectionmatchsetspaginator)
- `client.get_paginator("list_subscribed_rule_groups")` ->
  [ListSubscribedRuleGroupsPaginator](./paginators.md#listsubscribedrulegroupspaginator)
- `client.get_paginator("list_web_acls")` ->
  [ListWebACLsPaginator](./paginators.md#listwebaclspaginator)
- `client.get_paginator("list_xss_match_sets")` ->
  [ListXssMatchSetsPaginator](./paginators.md#listxssmatchsetspaginator)
