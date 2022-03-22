<a id="route53client-for-aiobotocore-route53-module"></a>

# Route53Client for aiobotocore Route53 module

> [Index](../README.md) > [Route53](./README.md) > Route53Client

Auto-generated documentation for
[Route53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
type annotations stubs module
[types-aiobotocore-route53](https://pypi.org/project/types-aiobotocore-route53/).

- [Route53Client for aiobotocore Route53 module](#route53client-for-aiobotocore-route53-module)
  - [Route53Client](#route53client)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [activate_key_signing_key](#activate_key_signing_key)
    - [associate_vpc_with_hosted_zone](#associate_vpc_with_hosted_zone)
    - [can_paginate](#can_paginate)
    - [change_resource_record_sets](#change_resource_record_sets)
    - [change_tags_for_resource](#change_tags_for_resource)
    - [create_health_check](#create_health_check)
    - [create_hosted_zone](#create_hosted_zone)
    - [create_key_signing_key](#create_key_signing_key)
    - [create_query_logging_config](#create_query_logging_config)
    - [create_reusable_delegation_set](#create_reusable_delegation_set)
    - [create_traffic_policy](#create_traffic_policy)
    - [create_traffic_policy_instance](#create_traffic_policy_instance)
    - [create_traffic_policy_version](#create_traffic_policy_version)
    - [create_vpc_association_authorization](#create_vpc_association_authorization)
    - [deactivate_key_signing_key](#deactivate_key_signing_key)
    - [delete_health_check](#delete_health_check)
    - [delete_hosted_zone](#delete_hosted_zone)
    - [delete_key_signing_key](#delete_key_signing_key)
    - [delete_query_logging_config](#delete_query_logging_config)
    - [delete_reusable_delegation_set](#delete_reusable_delegation_set)
    - [delete_traffic_policy](#delete_traffic_policy)
    - [delete_traffic_policy_instance](#delete_traffic_policy_instance)
    - [delete_vpc_association_authorization](#delete_vpc_association_authorization)
    - [disable_hosted_zone_dnssec](#disable_hosted_zone_dnssec)
    - [disassociate_vpc_from_hosted_zone](#disassociate_vpc_from_hosted_zone)
    - [enable_hosted_zone_dnssec](#enable_hosted_zone_dnssec)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_account_limit](#get_account_limit)
    - [get_change](#get_change)
    - [get_checker_ip_ranges](#get_checker_ip_ranges)
    - [get_dnssec](#get_dnssec)
    - [get_geo_location](#get_geo_location)
    - [get_health_check](#get_health_check)
    - [get_health_check_count](#get_health_check_count)
    - [get_health_check_last_failure_reason](#get_health_check_last_failure_reason)
    - [get_health_check_status](#get_health_check_status)
    - [get_hosted_zone](#get_hosted_zone)
    - [get_hosted_zone_count](#get_hosted_zone_count)
    - [get_hosted_zone_limit](#get_hosted_zone_limit)
    - [get_query_logging_config](#get_query_logging_config)
    - [get_reusable_delegation_set](#get_reusable_delegation_set)
    - [get_reusable_delegation_set_limit](#get_reusable_delegation_set_limit)
    - [get_traffic_policy](#get_traffic_policy)
    - [get_traffic_policy_instance](#get_traffic_policy_instance)
    - [get_traffic_policy_instance_count](#get_traffic_policy_instance_count)
    - [list_geo_locations](#list_geo_locations)
    - [list_health_checks](#list_health_checks)
    - [list_hosted_zones](#list_hosted_zones)
    - [list_hosted_zones_by_name](#list_hosted_zones_by_name)
    - [list_hosted_zones_by_vpc](#list_hosted_zones_by_vpc)
    - [list_query_logging_configs](#list_query_logging_configs)
    - [list_resource_record_sets](#list_resource_record_sets)
    - [list_reusable_delegation_sets](#list_reusable_delegation_sets)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_tags_for_resources](#list_tags_for_resources)
    - [list_traffic_policies](#list_traffic_policies)
    - [list_traffic_policy_instances](#list_traffic_policy_instances)
    - [list_traffic_policy_instances_by_hosted_zone](#list_traffic_policy_instances_by_hosted_zone)
    - [list_traffic_policy_instances_by_policy](#list_traffic_policy_instances_by_policy)
    - [list_traffic_policy_versions](#list_traffic_policy_versions)
    - [list_vpc_association_authorizations](#list_vpc_association_authorizations)
    - [test_dns_answer](#test_dns_answer)
    - [update_health_check](#update_health_check)
    - [update_hosted_zone_comment](#update_hosted_zone_comment)
    - [update_traffic_policy_comment](#update_traffic_policy_comment)
    - [update_traffic_policy_instance](#update_traffic_policy_instance)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="route53client"></a>

## Route53Client

Type annotations for `session.create_client("route53")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_route53.client import Route53Client

session = get_session()
async with session.create_client("route53") as client:
    client: Route53Client
```

Boto3 documentation:
[Route53.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_route53.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConcurrentModification`
- `Exceptions.ConflictingDomainExists`
- `Exceptions.ConflictingTypes`
- `Exceptions.DNSSECNotFound`
- `Exceptions.DelegationSetAlreadyCreated`
- `Exceptions.DelegationSetAlreadyReusable`
- `Exceptions.DelegationSetInUse`
- `Exceptions.DelegationSetNotAvailable`
- `Exceptions.DelegationSetNotReusable`
- `Exceptions.HealthCheckAlreadyExists`
- `Exceptions.HealthCheckInUse`
- `Exceptions.HealthCheckVersionMismatch`
- `Exceptions.HostedZoneAlreadyExists`
- `Exceptions.HostedZoneNotEmpty`
- `Exceptions.HostedZoneNotFound`
- `Exceptions.HostedZoneNotPrivate`
- `Exceptions.HostedZonePartiallyDelegated`
- `Exceptions.IncompatibleVersion`
- `Exceptions.InsufficientCloudWatchLogsResourcePolicy`
- `Exceptions.InvalidArgument`
- `Exceptions.InvalidChangeBatch`
- `Exceptions.InvalidDomainName`
- `Exceptions.InvalidInput`
- `Exceptions.InvalidKMSArn`
- `Exceptions.InvalidKeySigningKeyName`
- `Exceptions.InvalidKeySigningKeyStatus`
- `Exceptions.InvalidPaginationToken`
- `Exceptions.InvalidSigningStatus`
- `Exceptions.InvalidTrafficPolicyDocument`
- `Exceptions.InvalidVPCId`
- `Exceptions.KeySigningKeyAlreadyExists`
- `Exceptions.KeySigningKeyInParentDSRecord`
- `Exceptions.KeySigningKeyInUse`
- `Exceptions.KeySigningKeyWithActiveStatusNotFound`
- `Exceptions.LastVPCAssociation`
- `Exceptions.LimitsExceeded`
- `Exceptions.NoSuchChange`
- `Exceptions.NoSuchCloudWatchLogsLogGroup`
- `Exceptions.NoSuchDelegationSet`
- `Exceptions.NoSuchGeoLocation`
- `Exceptions.NoSuchHealthCheck`
- `Exceptions.NoSuchHostedZone`
- `Exceptions.NoSuchKeySigningKey`
- `Exceptions.NoSuchQueryLoggingConfig`
- `Exceptions.NoSuchTrafficPolicy`
- `Exceptions.NoSuchTrafficPolicyInstance`
- `Exceptions.NotAuthorizedException`
- `Exceptions.PriorRequestNotComplete`
- `Exceptions.PublicZoneVPCAssociation`
- `Exceptions.QueryLoggingConfigAlreadyExists`
- `Exceptions.ThrottlingException`
- `Exceptions.TooManyHealthChecks`
- `Exceptions.TooManyHostedZones`
- `Exceptions.TooManyKeySigningKeys`
- `Exceptions.TooManyTrafficPolicies`
- `Exceptions.TooManyTrafficPolicyInstances`
- `Exceptions.TooManyTrafficPolicyVersionsForCurrentPolicy`
- `Exceptions.TooManyVPCAssociationAuthorizations`
- `Exceptions.TrafficPolicyAlreadyExists`
- `Exceptions.TrafficPolicyInUse`
- `Exceptions.TrafficPolicyInstanceAlreadyExists`
- `Exceptions.VPCAssociationAuthorizationNotFound`
- `Exceptions.VPCAssociationNotFound`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

Route53Client exceptions.

Type annotations for `session.create_client("route53").exceptions` method.

Boto3 documentation:
[Route53.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="activate\_key\_signing\_key"></a>

### activate_key_signing_key

Activates a key-signing key (KSK) so that it can be used for signing by DNSSEC.

Type annotations for
`session.create_client("route53").activate_key_signing_key` method.

Boto3 documentation:
[Route53.Client.activate_key_signing_key](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.activate_key_signing_key)

Asynchronous method. Use `await activate_key_signing_key(...)` for a
synchronous call.

Arguments mapping described in
[ActivateKeySigningKeyRequestRequestTypeDef](./type_defs.md#activatekeysigningkeyrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `Name`: `str` *(required)*

Returns a `Coroutine` for
[ActivateKeySigningKeyResponseTypeDef](./type_defs.md#activatekeysigningkeyresponsetypedef).

<a id="associate\_vpc\_with\_hosted\_zone"></a>

### associate_vpc_with_hosted_zone

Associates an Amazon VPC with a private hosted zone.

Type annotations for
`session.create_client("route53").associate_vpc_with_hosted_zone` method.

Boto3 documentation:
[Route53.Client.associate_vpc_with_hosted_zone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.associate_vpc_with_hosted_zone)

Asynchronous method. Use `await associate_vpc_with_hosted_zone(...)` for a
synchronous call.

Arguments mapping described in
[AssociateVPCWithHostedZoneRequestRequestTypeDef](./type_defs.md#associatevpcwithhostedzonerequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `VPC`: [VPCTypeDef](./type_defs.md#vpctypedef) *(required)*
- `Comment`: `str`

Returns a `Coroutine` for
[AssociateVPCWithHostedZoneResponseTypeDef](./type_defs.md#associatevpcwithhostedzoneresponsetypedef).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("route53").can_paginate` method.

Boto3 documentation:
[Route53.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="change\_resource\_record\_sets"></a>

### change_resource_record_sets

Creates, changes, or deletes a resource record set, which contains
authoritative DNS information for a specified domain name or subdomain name.

Type annotations for
`session.create_client("route53").change_resource_record_sets` method.

Boto3 documentation:
[Route53.Client.change_resource_record_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.change_resource_record_sets)

Asynchronous method. Use `await change_resource_record_sets(...)` for a
synchronous call.

Arguments mapping described in
[ChangeResourceRecordSetsRequestRequestTypeDef](./type_defs.md#changeresourcerecordsetsrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `ChangeBatch`: [ChangeBatchTypeDef](./type_defs.md#changebatchtypedef)
  *(required)*

Returns a `Coroutine` for
[ChangeResourceRecordSetsResponseTypeDef](./type_defs.md#changeresourcerecordsetsresponsetypedef).

<a id="change\_tags\_for\_resource"></a>

### change_tags_for_resource

Adds, edits, or deletes tags for a health check or a hosted zone.

Type annotations for
`session.create_client("route53").change_tags_for_resource` method.

Boto3 documentation:
[Route53.Client.change_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.change_tags_for_resource)

Asynchronous method. Use `await change_tags_for_resource(...)` for a
synchronous call.

Arguments mapping described in
[ChangeTagsForResourceRequestRequestTypeDef](./type_defs.md#changetagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceType`: [TagResourceTypeType](./literals.md#tagresourcetypetype)
  *(required)*
- `ResourceId`: `str` *(required)*
- `AddTags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `RemoveTagKeys`: `Sequence`\[`str`\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="create\_health\_check"></a>

### create_health_check

Creates a new health check.

Type annotations for `session.create_client("route53").create_health_check`
method.

Boto3 documentation:
[Route53.Client.create_health_check](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_health_check)

Asynchronous method. Use `await create_health_check(...)` for a synchronous
call.

Arguments mapping described in
[CreateHealthCheckRequestRequestTypeDef](./type_defs.md#createhealthcheckrequestrequesttypedef).

Keyword-only arguments:

- `CallerReference`: `str` *(required)*
- `HealthCheckConfig`:
  [HealthCheckConfigTypeDef](./type_defs.md#healthcheckconfigtypedef)
  *(required)*

Returns a `Coroutine` for
[CreateHealthCheckResponseTypeDef](./type_defs.md#createhealthcheckresponsetypedef).

<a id="create\_hosted\_zone"></a>

### create_hosted_zone

Creates a new public or private hosted zone.

Type annotations for `session.create_client("route53").create_hosted_zone`
method.

Boto3 documentation:
[Route53.Client.create_hosted_zone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_hosted_zone)

Asynchronous method. Use `await create_hosted_zone(...)` for a synchronous
call.

Arguments mapping described in
[CreateHostedZoneRequestRequestTypeDef](./type_defs.md#createhostedzonerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `CallerReference`: `str` *(required)*
- `VPC`: [VPCTypeDef](./type_defs.md#vpctypedef)
- `HostedZoneConfig`:
  [HostedZoneConfigTypeDef](./type_defs.md#hostedzoneconfigtypedef)
- `DelegationSetId`: `str`

Returns a `Coroutine` for
[CreateHostedZoneResponseTypeDef](./type_defs.md#createhostedzoneresponsetypedef).

<a id="create\_key\_signing\_key"></a>

### create_key_signing_key

Creates a new key-signing key (KSK) associated with a hosted zone.

Type annotations for `session.create_client("route53").create_key_signing_key`
method.

Boto3 documentation:
[Route53.Client.create_key_signing_key](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_key_signing_key)

Asynchronous method. Use `await create_key_signing_key(...)` for a synchronous
call.

Arguments mapping described in
[CreateKeySigningKeyRequestRequestTypeDef](./type_defs.md#createkeysigningkeyrequestrequesttypedef).

Keyword-only arguments:

- `CallerReference`: `str` *(required)*
- `HostedZoneId`: `str` *(required)*
- `KeyManagementServiceArn`: `str` *(required)*
- `Name`: `str` *(required)*
- `Status`: `str` *(required)*

Returns a `Coroutine` for
[CreateKeySigningKeyResponseTypeDef](./type_defs.md#createkeysigningkeyresponsetypedef).

<a id="create\_query\_logging\_config"></a>

### create_query_logging_config

Creates a configuration for DNS query logging.

Type annotations for
`session.create_client("route53").create_query_logging_config` method.

Boto3 documentation:
[Route53.Client.create_query_logging_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_query_logging_config)

Asynchronous method. Use `await create_query_logging_config(...)` for a
synchronous call.

Arguments mapping described in
[CreateQueryLoggingConfigRequestRequestTypeDef](./type_defs.md#createqueryloggingconfigrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `CloudWatchLogsLogGroupArn`: `str` *(required)*

Returns a `Coroutine` for
[CreateQueryLoggingConfigResponseTypeDef](./type_defs.md#createqueryloggingconfigresponsetypedef).

<a id="create\_reusable\_delegation\_set"></a>

### create_reusable_delegation_set

Creates a delegation set (a group of four name servers) that can be reused by
multiple hosted zones that were created by the same Amazon Web Services
account.

Type annotations for
`session.create_client("route53").create_reusable_delegation_set` method.

Boto3 documentation:
[Route53.Client.create_reusable_delegation_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_reusable_delegation_set)

Asynchronous method. Use `await create_reusable_delegation_set(...)` for a
synchronous call.

Arguments mapping described in
[CreateReusableDelegationSetRequestRequestTypeDef](./type_defs.md#createreusabledelegationsetrequestrequesttypedef).

Keyword-only arguments:

- `CallerReference`: `str` *(required)*
- `HostedZoneId`: `str`

Returns a `Coroutine` for
[CreateReusableDelegationSetResponseTypeDef](./type_defs.md#createreusabledelegationsetresponsetypedef).

<a id="create\_traffic\_policy"></a>

### create_traffic_policy

Creates a traffic policy, which you use to create multiple DNS resource record
sets for one domain name (such as example.com) or one subdomain name (such as
www.example.com).

Type annotations for `session.create_client("route53").create_traffic_policy`
method.

Boto3 documentation:
[Route53.Client.create_traffic_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_traffic_policy)

Asynchronous method. Use `await create_traffic_policy(...)` for a synchronous
call.

Arguments mapping described in
[CreateTrafficPolicyRequestRequestTypeDef](./type_defs.md#createtrafficpolicyrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Document`: `str` *(required)*
- `Comment`: `str`

Returns a `Coroutine` for
[CreateTrafficPolicyResponseTypeDef](./type_defs.md#createtrafficpolicyresponsetypedef).

<a id="create\_traffic\_policy\_instance"></a>

### create_traffic_policy_instance

Creates resource record sets in a specified hosted zone based on the settings
in a specified traffic policy version.

Type annotations for
`session.create_client("route53").create_traffic_policy_instance` method.

Boto3 documentation:
[Route53.Client.create_traffic_policy_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_traffic_policy_instance)

Asynchronous method. Use `await create_traffic_policy_instance(...)` for a
synchronous call.

Arguments mapping described in
[CreateTrafficPolicyInstanceRequestRequestTypeDef](./type_defs.md#createtrafficpolicyinstancerequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `Name`: `str` *(required)*
- `TTL`: `int` *(required)*
- `TrafficPolicyId`: `str` *(required)*
- `TrafficPolicyVersion`: `int` *(required)*

Returns a `Coroutine` for
[CreateTrafficPolicyInstanceResponseTypeDef](./type_defs.md#createtrafficpolicyinstanceresponsetypedef).

<a id="create\_traffic\_policy\_version"></a>

### create_traffic_policy_version

Creates a new version of an existing traffic policy.

Type annotations for
`session.create_client("route53").create_traffic_policy_version` method.

Boto3 documentation:
[Route53.Client.create_traffic_policy_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_traffic_policy_version)

Asynchronous method. Use `await create_traffic_policy_version(...)` for a
synchronous call.

Arguments mapping described in
[CreateTrafficPolicyVersionRequestRequestTypeDef](./type_defs.md#createtrafficpolicyversionrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Document`: `str` *(required)*
- `Comment`: `str`

Returns a `Coroutine` for
[CreateTrafficPolicyVersionResponseTypeDef](./type_defs.md#createtrafficpolicyversionresponsetypedef).

<a id="create\_vpc\_association\_authorization"></a>

### create_vpc_association_authorization

Authorizes the Amazon Web Services account that created a specified VPC to
submit an `AssociateVPCWithHostedZone` request to associate the VPC with a
specified hosted zone that was created by a different account.

Type annotations for
`session.create_client("route53").create_vpc_association_authorization` method.

Boto3 documentation:
[Route53.Client.create_vpc_association_authorization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_vpc_association_authorization)

Asynchronous method. Use `await create_vpc_association_authorization(...)` for
a synchronous call.

Arguments mapping described in
[CreateVPCAssociationAuthorizationRequestRequestTypeDef](./type_defs.md#createvpcassociationauthorizationrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `VPC`: [VPCTypeDef](./type_defs.md#vpctypedef) *(required)*

Returns a `Coroutine` for
[CreateVPCAssociationAuthorizationResponseTypeDef](./type_defs.md#createvpcassociationauthorizationresponsetypedef).

<a id="deactivate\_key\_signing\_key"></a>

### deactivate_key_signing_key

Deactivates a key-signing key (KSK) so that it will not be used for signing by
DNSSEC.

Type annotations for
`session.create_client("route53").deactivate_key_signing_key` method.

Boto3 documentation:
[Route53.Client.deactivate_key_signing_key](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.deactivate_key_signing_key)

Asynchronous method. Use `await deactivate_key_signing_key(...)` for a
synchronous call.

Arguments mapping described in
[DeactivateKeySigningKeyRequestRequestTypeDef](./type_defs.md#deactivatekeysigningkeyrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `Name`: `str` *(required)*

Returns a `Coroutine` for
[DeactivateKeySigningKeyResponseTypeDef](./type_defs.md#deactivatekeysigningkeyresponsetypedef).

<a id="delete\_health\_check"></a>

### delete_health_check

Deletes a health check.

Type annotations for `session.create_client("route53").delete_health_check`
method.

Boto3 documentation:
[Route53.Client.delete_health_check](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.delete_health_check)

Asynchronous method. Use `await delete_health_check(...)` for a synchronous
call.

Arguments mapping described in
[DeleteHealthCheckRequestRequestTypeDef](./type_defs.md#deletehealthcheckrequestrequesttypedef).

Keyword-only arguments:

- `HealthCheckId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_hosted\_zone"></a>

### delete_hosted_zone

Deletes a hosted zone.

Type annotations for `session.create_client("route53").delete_hosted_zone`
method.

Boto3 documentation:
[Route53.Client.delete_hosted_zone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.delete_hosted_zone)

Asynchronous method. Use `await delete_hosted_zone(...)` for a synchronous
call.

Arguments mapping described in
[DeleteHostedZoneRequestRequestTypeDef](./type_defs.md#deletehostedzonerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[DeleteHostedZoneResponseTypeDef](./type_defs.md#deletehostedzoneresponsetypedef).

<a id="delete\_key\_signing\_key"></a>

### delete_key_signing_key

Deletes a key-signing key (KSK).

Type annotations for `session.create_client("route53").delete_key_signing_key`
method.

Boto3 documentation:
[Route53.Client.delete_key_signing_key](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.delete_key_signing_key)

Asynchronous method. Use `await delete_key_signing_key(...)` for a synchronous
call.

Arguments mapping described in
[DeleteKeySigningKeyRequestRequestTypeDef](./type_defs.md#deletekeysigningkeyrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `Name`: `str` *(required)*

Returns a `Coroutine` for
[DeleteKeySigningKeyResponseTypeDef](./type_defs.md#deletekeysigningkeyresponsetypedef).

<a id="delete\_query\_logging\_config"></a>

### delete_query_logging_config

Deletes a configuration for DNS query logging.

Type annotations for
`session.create_client("route53").delete_query_logging_config` method.

Boto3 documentation:
[Route53.Client.delete_query_logging_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.delete_query_logging_config)

Asynchronous method. Use `await delete_query_logging_config(...)` for a
synchronous call.

Arguments mapping described in
[DeleteQueryLoggingConfigRequestRequestTypeDef](./type_defs.md#deletequeryloggingconfigrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_reusable\_delegation\_set"></a>

### delete_reusable_delegation_set

Deletes a reusable delegation set.

Type annotations for
`session.create_client("route53").delete_reusable_delegation_set` method.

Boto3 documentation:
[Route53.Client.delete_reusable_delegation_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.delete_reusable_delegation_set)

Asynchronous method. Use `await delete_reusable_delegation_set(...)` for a
synchronous call.

Arguments mapping described in
[DeleteReusableDelegationSetRequestRequestTypeDef](./type_defs.md#deletereusabledelegationsetrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_traffic\_policy"></a>

### delete_traffic_policy

Deletes a traffic policy.

Type annotations for `session.create_client("route53").delete_traffic_policy`
method.

Boto3 documentation:
[Route53.Client.delete_traffic_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.delete_traffic_policy)

Asynchronous method. Use `await delete_traffic_policy(...)` for a synchronous
call.

Arguments mapping described in
[DeleteTrafficPolicyRequestRequestTypeDef](./type_defs.md#deletetrafficpolicyrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Version`: `int` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_traffic\_policy\_instance"></a>

### delete_traffic_policy_instance

Deletes a traffic policy instance and all of the resource record sets that
Amazon Route 53 created when you created the instance.

Type annotations for
`session.create_client("route53").delete_traffic_policy_instance` method.

Boto3 documentation:
[Route53.Client.delete_traffic_policy_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.delete_traffic_policy_instance)

Asynchronous method. Use `await delete_traffic_policy_instance(...)` for a
synchronous call.

Arguments mapping described in
[DeleteTrafficPolicyInstanceRequestRequestTypeDef](./type_defs.md#deletetrafficpolicyinstancerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_vpc\_association\_authorization"></a>

### delete_vpc_association_authorization

Removes authorization to submit an `AssociateVPCWithHostedZone` request to
associate a specified VPC with a hosted zone that was created by a different
account.

Type annotations for
`session.create_client("route53").delete_vpc_association_authorization` method.

Boto3 documentation:
[Route53.Client.delete_vpc_association_authorization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.delete_vpc_association_authorization)

Asynchronous method. Use `await delete_vpc_association_authorization(...)` for
a synchronous call.

Arguments mapping described in
[DeleteVPCAssociationAuthorizationRequestRequestTypeDef](./type_defs.md#deletevpcassociationauthorizationrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `VPC`: [VPCTypeDef](./type_defs.md#vpctypedef) *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disable\_hosted\_zone\_dnssec"></a>

### disable_hosted_zone_dnssec

Disables DNSSEC signing in a specific hosted zone.

Type annotations for
`session.create_client("route53").disable_hosted_zone_dnssec` method.

Boto3 documentation:
[Route53.Client.disable_hosted_zone_dnssec](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.disable_hosted_zone_dnssec)

Asynchronous method. Use `await disable_hosted_zone_dnssec(...)` for a
synchronous call.

Arguments mapping described in
[DisableHostedZoneDNSSECRequestRequestTypeDef](./type_defs.md#disablehostedzonednssecrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*

Returns a `Coroutine` for
[DisableHostedZoneDNSSECResponseTypeDef](./type_defs.md#disablehostedzonednssecresponsetypedef).

<a id="disassociate\_vpc\_from\_hosted\_zone"></a>

### disassociate_vpc_from_hosted_zone

Disassociates an Amazon Virtual Private Cloud (Amazon VPC) from an Amazon Route
53 private hosted zone.

Type annotations for
`session.create_client("route53").disassociate_vpc_from_hosted_zone` method.

Boto3 documentation:
[Route53.Client.disassociate_vpc_from_hosted_zone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.disassociate_vpc_from_hosted_zone)

Asynchronous method. Use `await disassociate_vpc_from_hosted_zone(...)` for a
synchronous call.

Arguments mapping described in
[DisassociateVPCFromHostedZoneRequestRequestTypeDef](./type_defs.md#disassociatevpcfromhostedzonerequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `VPC`: [VPCTypeDef](./type_defs.md#vpctypedef) *(required)*
- `Comment`: `str`

Returns a `Coroutine` for
[DisassociateVPCFromHostedZoneResponseTypeDef](./type_defs.md#disassociatevpcfromhostedzoneresponsetypedef).

<a id="enable\_hosted\_zone\_dnssec"></a>

### enable_hosted_zone_dnssec

Enables DNSSEC signing in a specific hosted zone.

Type annotations for
`session.create_client("route53").enable_hosted_zone_dnssec` method.

Boto3 documentation:
[Route53.Client.enable_hosted_zone_dnssec](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.enable_hosted_zone_dnssec)

Asynchronous method. Use `await enable_hosted_zone_dnssec(...)` for a
synchronous call.

Arguments mapping described in
[EnableHostedZoneDNSSECRequestRequestTypeDef](./type_defs.md#enablehostedzonednssecrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*

Returns a `Coroutine` for
[EnableHostedZoneDNSSECResponseTypeDef](./type_defs.md#enablehostedzonednssecresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("route53").generate_presigned_url`
method.

Boto3 documentation:
[Route53.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_account\_limit"></a>

### get_account_limit

Gets the specified limit for the current account, for example, the maximum
number of health checks that you can create using the account.

Type annotations for `session.create_client("route53").get_account_limit`
method.

Boto3 documentation:
[Route53.Client.get_account_limit](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_account_limit)

Asynchronous method. Use `await get_account_limit(...)` for a synchronous call.

Arguments mapping described in
[GetAccountLimitRequestRequestTypeDef](./type_defs.md#getaccountlimitrequestrequesttypedef).

Keyword-only arguments:

- `Type`: [AccountLimitTypeType](./literals.md#accountlimittypetype)
  *(required)*

Returns a `Coroutine` for
[GetAccountLimitResponseTypeDef](./type_defs.md#getaccountlimitresponsetypedef).

<a id="get\_change"></a>

### get_change

Returns the current status of a change batch request.

Type annotations for `session.create_client("route53").get_change` method.

Boto3 documentation:
[Route53.Client.get_change](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_change)

Asynchronous method. Use `await get_change(...)` for a synchronous call.

Arguments mapping described in
[GetChangeRequestRequestTypeDef](./type_defs.md#getchangerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetChangeResponseTypeDef](./type_defs.md#getchangeresponsetypedef).

<a id="get\_checker\_ip\_ranges"></a>

### get_checker_ip_ranges

Route 53 does not perform authorization for this API because it retrieves
information that is already available to the public.

Type annotations for `session.create_client("route53").get_checker_ip_ranges`
method.

Boto3 documentation:
[Route53.Client.get_checker_ip_ranges](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_checker_ip_ranges)

Asynchronous method. Use `await get_checker_ip_ranges(...)` for a synchronous
call.

Returns a `Coroutine` for
[GetCheckerIpRangesResponseTypeDef](./type_defs.md#getcheckeriprangesresponsetypedef).

<a id="get\_dnssec"></a>

### get_dnssec

Returns information about DNSSEC for a specific hosted zone, including the key-
signing keys (KSKs) in the hosted zone.

Type annotations for `session.create_client("route53").get_dnssec` method.

Boto3 documentation:
[Route53.Client.get_dnssec](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_dnssec)

Asynchronous method. Use `await get_dnssec(...)` for a synchronous call.

Arguments mapping described in
[GetDNSSECRequestRequestTypeDef](./type_defs.md#getdnssecrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*

Returns a `Coroutine` for
[GetDNSSECResponseTypeDef](./type_defs.md#getdnssecresponsetypedef).

<a id="get\_geo\_location"></a>

### get_geo_location

Gets information about whether a specified geographic location is supported for
Amazon Route 53 geolocation resource record sets.

Type annotations for `session.create_client("route53").get_geo_location`
method.

Boto3 documentation:
[Route53.Client.get_geo_location](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_geo_location)

Asynchronous method. Use `await get_geo_location(...)` for a synchronous call.

Arguments mapping described in
[GetGeoLocationRequestRequestTypeDef](./type_defs.md#getgeolocationrequestrequesttypedef).

Keyword-only arguments:

- `ContinentCode`: `str`
- `CountryCode`: `str`
- `SubdivisionCode`: `str`

Returns a `Coroutine` for
[GetGeoLocationResponseTypeDef](./type_defs.md#getgeolocationresponsetypedef).

<a id="get\_health\_check"></a>

### get_health_check

Gets information about a specified health check.

Type annotations for `session.create_client("route53").get_health_check`
method.

Boto3 documentation:
[Route53.Client.get_health_check](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_health_check)

Asynchronous method. Use `await get_health_check(...)` for a synchronous call.

Arguments mapping described in
[GetHealthCheckRequestRequestTypeDef](./type_defs.md#gethealthcheckrequestrequesttypedef).

Keyword-only arguments:

- `HealthCheckId`: `str` *(required)*

Returns a `Coroutine` for
[GetHealthCheckResponseTypeDef](./type_defs.md#gethealthcheckresponsetypedef).

<a id="get\_health\_check\_count"></a>

### get_health_check_count

Retrieves the number of health checks that are associated with the current
Amazon Web Services account.

Type annotations for `session.create_client("route53").get_health_check_count`
method.

Boto3 documentation:
[Route53.Client.get_health_check_count](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_health_check_count)

Asynchronous method. Use `await get_health_check_count(...)` for a synchronous
call.

Returns a `Coroutine` for
[GetHealthCheckCountResponseTypeDef](./type_defs.md#gethealthcheckcountresponsetypedef).

<a id="get\_health\_check\_last\_failure\_reason"></a>

### get_health_check_last_failure_reason

Gets the reason that a specified health check failed most recently.

Type annotations for
`session.create_client("route53").get_health_check_last_failure_reason` method.

Boto3 documentation:
[Route53.Client.get_health_check_last_failure_reason](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_health_check_last_failure_reason)

Asynchronous method. Use `await get_health_check_last_failure_reason(...)` for
a synchronous call.

Arguments mapping described in
[GetHealthCheckLastFailureReasonRequestRequestTypeDef](./type_defs.md#gethealthchecklastfailurereasonrequestrequesttypedef).

Keyword-only arguments:

- `HealthCheckId`: `str` *(required)*

Returns a `Coroutine` for
[GetHealthCheckLastFailureReasonResponseTypeDef](./type_defs.md#gethealthchecklastfailurereasonresponsetypedef).

<a id="get\_health\_check\_status"></a>

### get_health_check_status

Gets status of a specified health check.

Type annotations for `session.create_client("route53").get_health_check_status`
method.

Boto3 documentation:
[Route53.Client.get_health_check_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_health_check_status)

Asynchronous method. Use `await get_health_check_status(...)` for a synchronous
call.

Arguments mapping described in
[GetHealthCheckStatusRequestRequestTypeDef](./type_defs.md#gethealthcheckstatusrequestrequesttypedef).

Keyword-only arguments:

- `HealthCheckId`: `str` *(required)*

Returns a `Coroutine` for
[GetHealthCheckStatusResponseTypeDef](./type_defs.md#gethealthcheckstatusresponsetypedef).

<a id="get\_hosted\_zone"></a>

### get_hosted_zone

Gets information about a specified hosted zone including the four name servers
assigned to the hosted zone.

Type annotations for `session.create_client("route53").get_hosted_zone` method.

Boto3 documentation:
[Route53.Client.get_hosted_zone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_hosted_zone)

Asynchronous method. Use `await get_hosted_zone(...)` for a synchronous call.

Arguments mapping described in
[GetHostedZoneRequestRequestTypeDef](./type_defs.md#gethostedzonerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetHostedZoneResponseTypeDef](./type_defs.md#gethostedzoneresponsetypedef).

<a id="get\_hosted\_zone\_count"></a>

### get_hosted_zone_count

Retrieves the number of hosted zones that are associated with the current
Amazon Web Services account.

Type annotations for `session.create_client("route53").get_hosted_zone_count`
method.

Boto3 documentation:
[Route53.Client.get_hosted_zone_count](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_hosted_zone_count)

Asynchronous method. Use `await get_hosted_zone_count(...)` for a synchronous
call.

Returns a `Coroutine` for
[GetHostedZoneCountResponseTypeDef](./type_defs.md#gethostedzonecountresponsetypedef).

<a id="get\_hosted\_zone\_limit"></a>

### get_hosted_zone_limit

Gets the specified limit for a specified hosted zone, for example, the maximum
number of records that you can create in the hosted zone.

Type annotations for `session.create_client("route53").get_hosted_zone_limit`
method.

Boto3 documentation:
[Route53.Client.get_hosted_zone_limit](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_hosted_zone_limit)

Asynchronous method. Use `await get_hosted_zone_limit(...)` for a synchronous
call.

Arguments mapping described in
[GetHostedZoneLimitRequestRequestTypeDef](./type_defs.md#gethostedzonelimitrequestrequesttypedef).

Keyword-only arguments:

- `Type`: [HostedZoneLimitTypeType](./literals.md#hostedzonelimittypetype)
  *(required)*
- `HostedZoneId`: `str` *(required)*

Returns a `Coroutine` for
[GetHostedZoneLimitResponseTypeDef](./type_defs.md#gethostedzonelimitresponsetypedef).

<a id="get\_query\_logging\_config"></a>

### get_query_logging_config

Gets information about a specified configuration for DNS query logging.

Type annotations for
`session.create_client("route53").get_query_logging_config` method.

Boto3 documentation:
[Route53.Client.get_query_logging_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_query_logging_config)

Asynchronous method. Use `await get_query_logging_config(...)` for a
synchronous call.

Arguments mapping described in
[GetQueryLoggingConfigRequestRequestTypeDef](./type_defs.md#getqueryloggingconfigrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetQueryLoggingConfigResponseTypeDef](./type_defs.md#getqueryloggingconfigresponsetypedef).

<a id="get\_reusable\_delegation\_set"></a>

### get_reusable_delegation_set

Retrieves information about a specified reusable delegation set, including the
four name servers that are assigned to the delegation set.

Type annotations for
`session.create_client("route53").get_reusable_delegation_set` method.

Boto3 documentation:
[Route53.Client.get_reusable_delegation_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_reusable_delegation_set)

Asynchronous method. Use `await get_reusable_delegation_set(...)` for a
synchronous call.

Arguments mapping described in
[GetReusableDelegationSetRequestRequestTypeDef](./type_defs.md#getreusabledelegationsetrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetReusableDelegationSetResponseTypeDef](./type_defs.md#getreusabledelegationsetresponsetypedef).

<a id="get\_reusable\_delegation\_set\_limit"></a>

### get_reusable_delegation_set_limit

Gets the maximum number of hosted zones that you can associate with the
specified reusable delegation set.

Type annotations for
`session.create_client("route53").get_reusable_delegation_set_limit` method.

Boto3 documentation:
[Route53.Client.get_reusable_delegation_set_limit](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_reusable_delegation_set_limit)

Asynchronous method. Use `await get_reusable_delegation_set_limit(...)` for a
synchronous call.

Arguments mapping described in
[GetReusableDelegationSetLimitRequestRequestTypeDef](./type_defs.md#getreusabledelegationsetlimitrequestrequesttypedef).

Keyword-only arguments:

- `Type`: `Literal['MAX_ZONES_BY_REUSABLE_DELEGATION_SET']` (see
  [ReusableDelegationSetLimitTypeType](./literals.md#reusabledelegationsetlimittypetype))
  *(required)*
- `DelegationSetId`: `str` *(required)*

Returns a `Coroutine` for
[GetReusableDelegationSetLimitResponseTypeDef](./type_defs.md#getreusabledelegationsetlimitresponsetypedef).

<a id="get\_traffic\_policy"></a>

### get_traffic_policy

Gets information about a specific traffic policy version.

Type annotations for `session.create_client("route53").get_traffic_policy`
method.

Boto3 documentation:
[Route53.Client.get_traffic_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_traffic_policy)

Asynchronous method. Use `await get_traffic_policy(...)` for a synchronous
call.

Arguments mapping described in
[GetTrafficPolicyRequestRequestTypeDef](./type_defs.md#gettrafficpolicyrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Version`: `int` *(required)*

Returns a `Coroutine` for
[GetTrafficPolicyResponseTypeDef](./type_defs.md#gettrafficpolicyresponsetypedef).

<a id="get\_traffic\_policy\_instance"></a>

### get_traffic_policy_instance

Gets information about a specified traffic policy instance.

Type annotations for
`session.create_client("route53").get_traffic_policy_instance` method.

Boto3 documentation:
[Route53.Client.get_traffic_policy_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_traffic_policy_instance)

Asynchronous method. Use `await get_traffic_policy_instance(...)` for a
synchronous call.

Arguments mapping described in
[GetTrafficPolicyInstanceRequestRequestTypeDef](./type_defs.md#gettrafficpolicyinstancerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetTrafficPolicyInstanceResponseTypeDef](./type_defs.md#gettrafficpolicyinstanceresponsetypedef).

<a id="get\_traffic\_policy\_instance\_count"></a>

### get_traffic_policy_instance_count

Gets the number of traffic policy instances that are associated with the
current Amazon Web Services account.

Type annotations for
`session.create_client("route53").get_traffic_policy_instance_count` method.

Boto3 documentation:
[Route53.Client.get_traffic_policy_instance_count](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.get_traffic_policy_instance_count)

Asynchronous method. Use `await get_traffic_policy_instance_count(...)` for a
synchronous call.

Returns a `Coroutine` for
[GetTrafficPolicyInstanceCountResponseTypeDef](./type_defs.md#gettrafficpolicyinstancecountresponsetypedef).

<a id="list\_geo\_locations"></a>

### list_geo_locations

Retrieves a list of supported geographic locations.

Type annotations for `session.create_client("route53").list_geo_locations`
method.

Boto3 documentation:
[Route53.Client.list_geo_locations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_geo_locations)

Asynchronous method. Use `await list_geo_locations(...)` for a synchronous
call.

Arguments mapping described in
[ListGeoLocationsRequestRequestTypeDef](./type_defs.md#listgeolocationsrequestrequesttypedef).

Keyword-only arguments:

- `StartContinentCode`: `str`
- `StartCountryCode`: `str`
- `StartSubdivisionCode`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListGeoLocationsResponseTypeDef](./type_defs.md#listgeolocationsresponsetypedef).

<a id="list\_health\_checks"></a>

### list_health_checks

Retrieve a list of the health checks that are associated with the current
Amazon Web Services account.

Type annotations for `session.create_client("route53").list_health_checks`
method.

Boto3 documentation:
[Route53.Client.list_health_checks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_health_checks)

Asynchronous method. Use `await list_health_checks(...)` for a synchronous
call.

Arguments mapping described in
[ListHealthChecksRequestRequestTypeDef](./type_defs.md#listhealthchecksrequestrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListHealthChecksResponseTypeDef](./type_defs.md#listhealthchecksresponsetypedef).

<a id="list\_hosted\_zones"></a>

### list_hosted_zones

Retrieves a list of the public and private hosted zones that are associated
with the current Amazon Web Services account.

Type annotations for `session.create_client("route53").list_hosted_zones`
method.

Boto3 documentation:
[Route53.Client.list_hosted_zones](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_hosted_zones)

Asynchronous method. Use `await list_hosted_zones(...)` for a synchronous call.

Arguments mapping described in
[ListHostedZonesRequestRequestTypeDef](./type_defs.md#listhostedzonesrequestrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`
- `MaxItems`: `str`
- `DelegationSetId`: `str`

Returns a `Coroutine` for
[ListHostedZonesResponseTypeDef](./type_defs.md#listhostedzonesresponsetypedef).

<a id="list\_hosted\_zones\_by\_name"></a>

### list_hosted_zones_by_name

Retrieves a list of your hosted zones in lexicographic order.

Type annotations for
`session.create_client("route53").list_hosted_zones_by_name` method.

Boto3 documentation:
[Route53.Client.list_hosted_zones_by_name](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_hosted_zones_by_name)

Asynchronous method. Use `await list_hosted_zones_by_name(...)` for a
synchronous call.

Arguments mapping described in
[ListHostedZonesByNameRequestRequestTypeDef](./type_defs.md#listhostedzonesbynamerequestrequesttypedef).

Keyword-only arguments:

- `DNSName`: `str`
- `HostedZoneId`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListHostedZonesByNameResponseTypeDef](./type_defs.md#listhostedzonesbynameresponsetypedef).

<a id="list\_hosted\_zones\_by\_vpc"></a>

### list_hosted_zones_by_vpc

Lists all the private hosted zones that a specified VPC is associated with,
regardless of which Amazon Web Services account or Amazon Web Services service
owns the hosted zones.

Type annotations for
`session.create_client("route53").list_hosted_zones_by_vpc` method.

Boto3 documentation:
[Route53.Client.list_hosted_zones_by_vpc](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_hosted_zones_by_vpc)

Asynchronous method. Use `await list_hosted_zones_by_vpc(...)` for a
synchronous call.

Arguments mapping described in
[ListHostedZonesByVPCRequestRequestTypeDef](./type_defs.md#listhostedzonesbyvpcrequestrequesttypedef).

Keyword-only arguments:

- `VPCId`: `str` *(required)*
- `VPCRegion`: [VPCRegionType](./literals.md#vpcregiontype) *(required)*
- `MaxItems`: `str`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListHostedZonesByVPCResponseTypeDef](./type_defs.md#listhostedzonesbyvpcresponsetypedef).

<a id="list\_query\_logging\_configs"></a>

### list_query_logging_configs

Lists the configurations for DNS query logging that are associated with the
current Amazon Web Services account or the configuration that is associated
with a specified hosted zone.

Type annotations for
`session.create_client("route53").list_query_logging_configs` method.

Boto3 documentation:
[Route53.Client.list_query_logging_configs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_query_logging_configs)

Asynchronous method. Use `await list_query_logging_configs(...)` for a
synchronous call.

Arguments mapping described in
[ListQueryLoggingConfigsRequestRequestTypeDef](./type_defs.md#listqueryloggingconfigsrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str`
- `NextToken`: `str`
- `MaxResults`: `str`

Returns a `Coroutine` for
[ListQueryLoggingConfigsResponseTypeDef](./type_defs.md#listqueryloggingconfigsresponsetypedef).

<a id="list\_resource\_record\_sets"></a>

### list_resource_record_sets

Lists the resource record sets in a specified hosted zone.

Type annotations for
`session.create_client("route53").list_resource_record_sets` method.

Boto3 documentation:
[Route53.Client.list_resource_record_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_resource_record_sets)

Asynchronous method. Use `await list_resource_record_sets(...)` for a
synchronous call.

Arguments mapping described in
[ListResourceRecordSetsRequestRequestTypeDef](./type_defs.md#listresourcerecordsetsrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `StartRecordName`: `str`
- `StartRecordType`: [RRTypeType](./literals.md#rrtypetype)
- `StartRecordIdentifier`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListResourceRecordSetsResponseTypeDef](./type_defs.md#listresourcerecordsetsresponsetypedef).

<a id="list\_reusable\_delegation\_sets"></a>

### list_reusable_delegation_sets

Retrieves a list of the reusable delegation sets that are associated with the
current Amazon Web Services account.

Type annotations for
`session.create_client("route53").list_reusable_delegation_sets` method.

Boto3 documentation:
[Route53.Client.list_reusable_delegation_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_reusable_delegation_sets)

Asynchronous method. Use `await list_reusable_delegation_sets(...)` for a
synchronous call.

Arguments mapping described in
[ListReusableDelegationSetsRequestRequestTypeDef](./type_defs.md#listreusabledelegationsetsrequestrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListReusableDelegationSetsResponseTypeDef](./type_defs.md#listreusabledelegationsetsresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Lists tags for one health check or hosted zone.

Type annotations for `session.create_client("route53").list_tags_for_resource`
method.

Boto3 documentation:
[Route53.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceType`: [TagResourceTypeType](./literals.md#tagresourcetypetype)
  *(required)*
- `ResourceId`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="list\_tags\_for\_resources"></a>

### list_tags_for_resources

Lists tags for up to 10 health checks or hosted zones.

Type annotations for `session.create_client("route53").list_tags_for_resources`
method.

Boto3 documentation:
[Route53.Client.list_tags_for_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_tags_for_resources)

Asynchronous method. Use `await list_tags_for_resources(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourcesRequestRequestTypeDef](./type_defs.md#listtagsforresourcesrequestrequesttypedef).

Keyword-only arguments:

- `ResourceType`: [TagResourceTypeType](./literals.md#tagresourcetypetype)
  *(required)*
- `ResourceIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[ListTagsForResourcesResponseTypeDef](./type_defs.md#listtagsforresourcesresponsetypedef).

<a id="list\_traffic\_policies"></a>

### list_traffic_policies

Gets information about the latest version for every traffic policy that is
associated with the current Amazon Web Services account.

Type annotations for `session.create_client("route53").list_traffic_policies`
method.

Boto3 documentation:
[Route53.Client.list_traffic_policies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_traffic_policies)

Asynchronous method. Use `await list_traffic_policies(...)` for a synchronous
call.

Arguments mapping described in
[ListTrafficPoliciesRequestRequestTypeDef](./type_defs.md#listtrafficpoliciesrequestrequesttypedef).

Keyword-only arguments:

- `TrafficPolicyIdMarker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListTrafficPoliciesResponseTypeDef](./type_defs.md#listtrafficpoliciesresponsetypedef).

<a id="list\_traffic\_policy\_instances"></a>

### list_traffic_policy_instances

Gets information about the traffic policy instances that you created by using
the current Amazon Web Services account.

Type annotations for
`session.create_client("route53").list_traffic_policy_instances` method.

Boto3 documentation:
[Route53.Client.list_traffic_policy_instances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_traffic_policy_instances)

Asynchronous method. Use `await list_traffic_policy_instances(...)` for a
synchronous call.

Arguments mapping described in
[ListTrafficPolicyInstancesRequestRequestTypeDef](./type_defs.md#listtrafficpolicyinstancesrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneIdMarker`: `str`
- `TrafficPolicyInstanceNameMarker`: `str`
- `TrafficPolicyInstanceTypeMarker`: [RRTypeType](./literals.md#rrtypetype)
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListTrafficPolicyInstancesResponseTypeDef](./type_defs.md#listtrafficpolicyinstancesresponsetypedef).

<a id="list\_traffic\_policy\_instances\_by\_hosted\_zone"></a>

### list_traffic_policy_instances_by_hosted_zone

Gets information about the traffic policy instances that you created in a
specified hosted zone.

Type annotations for
`session.create_client("route53").list_traffic_policy_instances_by_hosted_zone`
method.

Boto3 documentation:
[Route53.Client.list_traffic_policy_instances_by_hosted_zone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_traffic_policy_instances_by_hosted_zone)

Asynchronous method. Use
`await list_traffic_policy_instances_by_hosted_zone(...)` for a synchronous
call.

Arguments mapping described in
[ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef](./type_defs.md#listtrafficpolicyinstancesbyhostedzonerequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `TrafficPolicyInstanceNameMarker`: `str`
- `TrafficPolicyInstanceTypeMarker`: [RRTypeType](./literals.md#rrtypetype)
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListTrafficPolicyInstancesByHostedZoneResponseTypeDef](./type_defs.md#listtrafficpolicyinstancesbyhostedzoneresponsetypedef).

<a id="list\_traffic\_policy\_instances\_by\_policy"></a>

### list_traffic_policy_instances_by_policy

Gets information about the traffic policy instances that you created by using a
specify traffic policy version.

Type annotations for
`session.create_client("route53").list_traffic_policy_instances_by_policy`
method.

Boto3 documentation:
[Route53.Client.list_traffic_policy_instances_by_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_traffic_policy_instances_by_policy)

Asynchronous method. Use `await list_traffic_policy_instances_by_policy(...)`
for a synchronous call.

Arguments mapping described in
[ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef](./type_defs.md#listtrafficpolicyinstancesbypolicyrequestrequesttypedef).

Keyword-only arguments:

- `TrafficPolicyId`: `str` *(required)*
- `TrafficPolicyVersion`: `int` *(required)*
- `HostedZoneIdMarker`: `str`
- `TrafficPolicyInstanceNameMarker`: `str`
- `TrafficPolicyInstanceTypeMarker`: [RRTypeType](./literals.md#rrtypetype)
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListTrafficPolicyInstancesByPolicyResponseTypeDef](./type_defs.md#listtrafficpolicyinstancesbypolicyresponsetypedef).

<a id="list\_traffic\_policy\_versions"></a>

### list_traffic_policy_versions

Gets information about all of the versions for a specified traffic policy.

Type annotations for
`session.create_client("route53").list_traffic_policy_versions` method.

Boto3 documentation:
[Route53.Client.list_traffic_policy_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_traffic_policy_versions)

Asynchronous method. Use `await list_traffic_policy_versions(...)` for a
synchronous call.

Arguments mapping described in
[ListTrafficPolicyVersionsRequestRequestTypeDef](./type_defs.md#listtrafficpolicyversionsrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `TrafficPolicyVersionMarker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListTrafficPolicyVersionsResponseTypeDef](./type_defs.md#listtrafficpolicyversionsresponsetypedef).

<a id="list\_vpc\_association\_authorizations"></a>

### list_vpc_association_authorizations

Gets a list of the VPCs that were created by other accounts and that can be
associated with a specified hosted zone because you've submitted one or more
`CreateVPCAssociationAuthorization` requests.

Type annotations for
`session.create_client("route53").list_vpc_association_authorizations` method.

Boto3 documentation:
[Route53.Client.list_vpc_association_authorizations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_vpc_association_authorizations)

Asynchronous method. Use `await list_vpc_association_authorizations(...)` for a
synchronous call.

Arguments mapping described in
[ListVPCAssociationAuthorizationsRequestRequestTypeDef](./type_defs.md#listvpcassociationauthorizationsrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `str`

Returns a `Coroutine` for
[ListVPCAssociationAuthorizationsResponseTypeDef](./type_defs.md#listvpcassociationauthorizationsresponsetypedef).

<a id="test\_dns\_answer"></a>

### test_dns_answer

Gets the value that Amazon Route 53 returns in response to a DNS request for a
specified record name and type.

Type annotations for `session.create_client("route53").test_dns_answer` method.

Boto3 documentation:
[Route53.Client.test_dns_answer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.test_dns_answer)

Asynchronous method. Use `await test_dns_answer(...)` for a synchronous call.

Arguments mapping described in
[TestDNSAnswerRequestRequestTypeDef](./type_defs.md#testdnsanswerrequestrequesttypedef).

Keyword-only arguments:

- `HostedZoneId`: `str` *(required)*
- `RecordName`: `str` *(required)*
- `RecordType`: [RRTypeType](./literals.md#rrtypetype) *(required)*
- `ResolverIP`: `str`
- `EDNS0ClientSubnetIP`: `str`
- `EDNS0ClientSubnetMask`: `str`

Returns a `Coroutine` for
[TestDNSAnswerResponseTypeDef](./type_defs.md#testdnsanswerresponsetypedef).

<a id="update\_health\_check"></a>

### update_health_check

Updates an existing health check.

Type annotations for `session.create_client("route53").update_health_check`
method.

Boto3 documentation:
[Route53.Client.update_health_check](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.update_health_check)

Asynchronous method. Use `await update_health_check(...)` for a synchronous
call.

Arguments mapping described in
[UpdateHealthCheckRequestRequestTypeDef](./type_defs.md#updatehealthcheckrequestrequesttypedef).

Keyword-only arguments:

- `HealthCheckId`: `str` *(required)*
- `HealthCheckVersion`: `int`
- `IPAddress`: `str`
- `Port`: `int`
- `ResourcePath`: `str`
- `FullyQualifiedDomainName`: `str`
- `SearchString`: `str`
- `FailureThreshold`: `int`
- `Inverted`: `bool`
- `Disabled`: `bool`
- `HealthThreshold`: `int`
- `ChildHealthChecks`: `Sequence`\[`str`\]
- `EnableSNI`: `bool`
- `Regions`:
  `Sequence`\[[HealthCheckRegionType](./literals.md#healthcheckregiontype)\]
- `AlarmIdentifier`:
  [AlarmIdentifierTypeDef](./type_defs.md#alarmidentifiertypedef)
- `InsufficientDataHealthStatus`:
  [InsufficientDataHealthStatusType](./literals.md#insufficientdatahealthstatustype)
- `ResetElements`:
  `Sequence`\[[ResettableElementNameType](./literals.md#resettableelementnametype)\]

Returns a `Coroutine` for
[UpdateHealthCheckResponseTypeDef](./type_defs.md#updatehealthcheckresponsetypedef).

<a id="update\_hosted\_zone\_comment"></a>

### update_hosted_zone_comment

Updates the comment for a specified hosted zone.

Type annotations for
`session.create_client("route53").update_hosted_zone_comment` method.

Boto3 documentation:
[Route53.Client.update_hosted_zone_comment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.update_hosted_zone_comment)

Asynchronous method. Use `await update_hosted_zone_comment(...)` for a
synchronous call.

Arguments mapping described in
[UpdateHostedZoneCommentRequestRequestTypeDef](./type_defs.md#updatehostedzonecommentrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Comment`: `str`

Returns a `Coroutine` for
[UpdateHostedZoneCommentResponseTypeDef](./type_defs.md#updatehostedzonecommentresponsetypedef).

<a id="update\_traffic\_policy\_comment"></a>

### update_traffic_policy_comment

Updates the comment for a specified traffic policy version.

Type annotations for
`session.create_client("route53").update_traffic_policy_comment` method.

Boto3 documentation:
[Route53.Client.update_traffic_policy_comment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.update_traffic_policy_comment)

Asynchronous method. Use `await update_traffic_policy_comment(...)` for a
synchronous call.

Arguments mapping described in
[UpdateTrafficPolicyCommentRequestRequestTypeDef](./type_defs.md#updatetrafficpolicycommentrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Version`: `int` *(required)*
- `Comment`: `str` *(required)*

Returns a `Coroutine` for
[UpdateTrafficPolicyCommentResponseTypeDef](./type_defs.md#updatetrafficpolicycommentresponsetypedef).

<a id="update\_traffic\_policy\_instance"></a>

### update_traffic_policy_instance

Updates the resource record sets in a specified hosted zone that were created
based on the settings in a specified traffic policy version.

Type annotations for
`session.create_client("route53").update_traffic_policy_instance` method.

Boto3 documentation:
[Route53.Client.update_traffic_policy_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.update_traffic_policy_instance)

Asynchronous method. Use `await update_traffic_policy_instance(...)` for a
synchronous call.

Arguments mapping described in
[UpdateTrafficPolicyInstanceRequestRequestTypeDef](./type_defs.md#updatetrafficpolicyinstancerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `TTL`: `int` *(required)*
- `TrafficPolicyId`: `str` *(required)*
- `TrafficPolicyVersion`: `int` *(required)*

Returns a `Coroutine` for
[UpdateTrafficPolicyInstanceResponseTypeDef](./type_defs.md#updatetrafficpolicyinstanceresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("route53").__aenter__` method.

Boto3 documentation:
[Route53.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [Route53Client](#route53client).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("route53").__aexit__` method.

Boto3 documentation:
[Route53.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("route53").get_paginator` method
with overloads.

- `client.get_paginator("list_health_checks")` ->
  [ListHealthChecksPaginator](./paginators.md#listhealthcheckspaginator)
- `client.get_paginator("list_hosted_zones")` ->
  [ListHostedZonesPaginator](./paginators.md#listhostedzonespaginator)
- `client.get_paginator("list_query_logging_configs")` ->
  [ListQueryLoggingConfigsPaginator](./paginators.md#listqueryloggingconfigspaginator)
- `client.get_paginator("list_resource_record_sets")` ->
  [ListResourceRecordSetsPaginator](./paginators.md#listresourcerecordsetspaginator)
- `client.get_paginator("list_vpc_association_authorizations")` ->
  [ListVPCAssociationAuthorizationsPaginator](./paginators.md#listvpcassociationauthorizationspaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("route53").get_waiter` method with
overloads.

- `client.get_waiter("resource_record_sets_changed")` ->
  [ResourceRecordSetsChangedWaiter](./waiters.md#resourcerecordsetschangedwaiter)
