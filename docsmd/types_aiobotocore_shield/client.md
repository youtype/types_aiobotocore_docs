# ShieldClient

> [Index](../README.md) > [Shield](./README.md) > ShieldClient

!!! note ""

    Auto-generated documentation for [Shield](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#shield)
    type annotations stubs module [types-aiobotocore-shield](https://pypi.org/project/types-aiobotocore-shield/).

## ShieldClient

Type annotations and code completion for `#!python session.create_client("shield")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client)

```python
# ShieldClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_shield.client import ShieldClient

session = get_session()
async with session.create_client("shield") as client:
    client: ShieldClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("shield").exceptions` structure.

```python
# ShieldClient.exceptions usage example

async with session.create_client("shield") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.AccessDeniedForDependencyException,
        client.ClientError,
        client.InternalErrorException,
        client.InvalidOperationException,
        client.InvalidPaginationTokenException,
        client.InvalidParameterException,
        client.InvalidResourceException,
        client.LimitsExceededException,
        client.LockedSubscriptionException,
        client.NoAssociatedRoleException,
        client.OptimisticLockException,
        client.ResourceAlreadyExistsException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# ShieldClient usage type checking example

from types_aiobotocore_shield.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("shield").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("shield").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/generate_presigned_url.html)

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


### associate\_drt\_log\_bucket

Authorizes the Shield Response Team (SRT) to access the specified Amazon S3
bucket containing log data such as Application Load Balancer access logs,
CloudFront logs, or logs from third party sources.

Type annotations and code completion for `#!python session.create_client("shield").associate_drt_log_bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/associate_drt_log_bucket.html)

```python
# associate_drt_log_bucket method definition

await def associate_drt_log_bucket(
    self,
    *,
    LogBucket: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_drt_log_bucket method usage example with argument unpacking

kwargs: AssociateDRTLogBucketRequestTypeDef = {  # (1)
    "LogBucket": ...,
}

parent.associate_drt_log_bucket(**kwargs)
```

1. See [:material-code-braces: AssociateDRTLogBucketRequestTypeDef](./type_defs.md#associatedrtlogbucketrequesttypedef) 

### associate\_drt\_role

Authorizes the Shield Response Team (SRT) using the specified role, to access
your Amazon Web Services account to assist with DDoS attack mitigation during
potential attacks.

Type annotations and code completion for `#!python session.create_client("shield").associate_drt_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/associate_drt_role.html)

```python
# associate_drt_role method definition

await def associate_drt_role(
    self,
    *,
    RoleArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_drt_role method usage example with argument unpacking

kwargs: AssociateDRTRoleRequestTypeDef = {  # (1)
    "RoleArn": ...,
}

parent.associate_drt_role(**kwargs)
```

1. See [:material-code-braces: AssociateDRTRoleRequestTypeDef](./type_defs.md#associatedrtrolerequesttypedef) 

### associate\_health\_check

Adds health-based detection to the Shield Advanced protection for a resource.

Type annotations and code completion for `#!python session.create_client("shield").associate_health_check` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/associate_health_check.html)

```python
# associate_health_check method definition

await def associate_health_check(
    self,
    *,
    ProtectionId: str,
    HealthCheckArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_health_check method usage example with argument unpacking

kwargs: AssociateHealthCheckRequestTypeDef = {  # (1)
    "ProtectionId": ...,
    "HealthCheckArn": ...,
}

parent.associate_health_check(**kwargs)
```

1. See [:material-code-braces: AssociateHealthCheckRequestTypeDef](./type_defs.md#associatehealthcheckrequesttypedef) 

### associate\_proactive\_engagement\_details

Initializes proactive engagement and sets the list of contacts for the Shield
Response Team (SRT) to use.

Type annotations and code completion for `#!python session.create_client("shield").associate_proactive_engagement_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/associate_proactive_engagement_details.html)

```python
# associate_proactive_engagement_details method definition

await def associate_proactive_engagement_details(
    self,
    *,
    EmergencyContactList: Sequence[EmergencyContactTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: EmergencyContactTypeDef](./type_defs.md#emergencycontacttypedef) 


```python
# associate_proactive_engagement_details method usage example with argument unpacking

kwargs: AssociateProactiveEngagementDetailsRequestTypeDef = {  # (1)
    "EmergencyContactList": ...,
}

parent.associate_proactive_engagement_details(**kwargs)
```

1. See [:material-code-braces: AssociateProactiveEngagementDetailsRequestTypeDef](./type_defs.md#associateproactiveengagementdetailsrequesttypedef) 

### create\_protection

Enables Shield Advanced for a specific Amazon Web Services resource.

Type annotations and code completion for `#!python session.create_client("shield").create_protection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/create_protection.html)

```python
# create_protection method definition

await def create_protection(
    self,
    *,
    Name: str,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateProtectionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateProtectionResponseTypeDef](./type_defs.md#createprotectionresponsetypedef) 


```python
# create_protection method usage example with argument unpacking

kwargs: CreateProtectionRequestTypeDef = {  # (1)
    "Name": ...,
    "ResourceArn": ...,
}

parent.create_protection(**kwargs)
```

1. See [:material-code-braces: CreateProtectionRequestTypeDef](./type_defs.md#createprotectionrequesttypedef) 

### create\_protection\_group

Creates a grouping of protected resources so they can be handled as a
collective.

Type annotations and code completion for `#!python session.create_client("shield").create_protection_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/create_protection_group.html)

```python
# create_protection_group method definition

await def create_protection_group(
    self,
    *,
    ProtectionGroupId: str,
    Aggregation: ProtectionGroupAggregationType,  # (1)
    Pattern: ProtectionGroupPatternType,  # (2)
    ResourceType: ProtectedResourceTypeType = ...,  # (3)
    Members: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ProtectionGroupAggregationType](./literals.md#protectiongroupaggregationtype) 
2. See [:material-code-brackets: ProtectionGroupPatternType](./literals.md#protectiongrouppatterntype) 
3. See [:material-code-brackets: ProtectedResourceTypeType](./literals.md#protectedresourcetypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create_protection_group method usage example with argument unpacking

kwargs: CreateProtectionGroupRequestTypeDef = {  # (1)
    "ProtectionGroupId": ...,
    "Aggregation": ...,
    "Pattern": ...,
}

parent.create_protection_group(**kwargs)
```

1. See [:material-code-braces: CreateProtectionGroupRequestTypeDef](./type_defs.md#createprotectiongrouprequesttypedef) 

### create\_subscription

Activates Shield Advanced for an account.

Type annotations and code completion for `#!python session.create_client("shield").create_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/create_subscription.html)

```python
# create_subscription method definition

await def create_subscription(
    self,
) -> Dict[str, Any]:
    ...
```


### delete\_protection

Deletes an Shield Advanced <a>Protection</a>.

Type annotations and code completion for `#!python session.create_client("shield").delete_protection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/delete_protection.html)

```python
# delete_protection method definition

await def delete_protection(
    self,
    *,
    ProtectionId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_protection method usage example with argument unpacking

kwargs: DeleteProtectionRequestTypeDef = {  # (1)
    "ProtectionId": ...,
}

parent.delete_protection(**kwargs)
```

1. See [:material-code-braces: DeleteProtectionRequestTypeDef](./type_defs.md#deleteprotectionrequesttypedef) 

### delete\_protection\_group

Removes the specified protection group.

Type annotations and code completion for `#!python session.create_client("shield").delete_protection_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/delete_protection_group.html)

```python
# delete_protection_group method definition

await def delete_protection_group(
    self,
    *,
    ProtectionGroupId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_protection_group method usage example with argument unpacking

kwargs: DeleteProtectionGroupRequestTypeDef = {  # (1)
    "ProtectionGroupId": ...,
}

parent.delete_protection_group(**kwargs)
```

1. See [:material-code-braces: DeleteProtectionGroupRequestTypeDef](./type_defs.md#deleteprotectiongrouprequesttypedef) 

### delete\_subscription

Removes Shield Advanced from an account.

Type annotations and code completion for `#!python session.create_client("shield").delete_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/delete_subscription.html)

```python
# delete_subscription method definition

await def delete_subscription(
    self,
) -> Dict[str, Any]:
    ...
```


### describe\_attack

Describes the details of a DDoS attack.

Type annotations and code completion for `#!python session.create_client("shield").describe_attack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/describe_attack.html)

```python
# describe_attack method definition

await def describe_attack(
    self,
    *,
    AttackId: str,
) -> DescribeAttackResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAttackResponseTypeDef](./type_defs.md#describeattackresponsetypedef) 


```python
# describe_attack method usage example with argument unpacking

kwargs: DescribeAttackRequestTypeDef = {  # (1)
    "AttackId": ...,
}

parent.describe_attack(**kwargs)
```

1. See [:material-code-braces: DescribeAttackRequestTypeDef](./type_defs.md#describeattackrequesttypedef) 

### describe\_attack\_statistics

Provides information about the number and type of attacks Shield has detected
in the last year for all resources that belong to your account, regardless of
whether you've defined Shield protections for them.

Type annotations and code completion for `#!python session.create_client("shield").describe_attack_statistics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/describe_attack_statistics.html)

```python
# describe_attack_statistics method definition

await def describe_attack_statistics(
    self,
) -> DescribeAttackStatisticsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAttackStatisticsResponseTypeDef](./type_defs.md#describeattackstatisticsresponsetypedef) 

### describe\_drt\_access

Returns the current role and list of Amazon S3 log buckets used by the Shield
Response Team (SRT) to access your Amazon Web Services account while assisting
with attack mitigation.

Type annotations and code completion for `#!python session.create_client("shield").describe_drt_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/describe_drt_access.html)

```python
# describe_drt_access method definition

await def describe_drt_access(
    self,
) -> DescribeDRTAccessResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDRTAccessResponseTypeDef](./type_defs.md#describedrtaccessresponsetypedef) 

### describe\_emergency\_contact\_settings

A list of email addresses and phone numbers that the Shield Response Team (SRT)
can use to contact you if you have proactive engagement enabled, for
escalations to the SRT and to initiate proactive customer support.

Type annotations and code completion for `#!python session.create_client("shield").describe_emergency_contact_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/describe_emergency_contact_settings.html)

```python
# describe_emergency_contact_settings method definition

await def describe_emergency_contact_settings(
    self,
) -> DescribeEmergencyContactSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEmergencyContactSettingsResponseTypeDef](./type_defs.md#describeemergencycontactsettingsresponsetypedef) 

### describe\_protection

Lists the details of a <a>Protection</a> object.

Type annotations and code completion for `#!python session.create_client("shield").describe_protection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/describe_protection.html)

```python
# describe_protection method definition

await def describe_protection(
    self,
    *,
    ProtectionId: str = ...,
    ResourceArn: str = ...,
) -> DescribeProtectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProtectionResponseTypeDef](./type_defs.md#describeprotectionresponsetypedef) 


```python
# describe_protection method usage example with argument unpacking

kwargs: DescribeProtectionRequestTypeDef = {  # (1)
    "ProtectionId": ...,
}

parent.describe_protection(**kwargs)
```

1. See [:material-code-braces: DescribeProtectionRequestTypeDef](./type_defs.md#describeprotectionrequesttypedef) 

### describe\_protection\_group

Returns the specification for the specified protection group.

Type annotations and code completion for `#!python session.create_client("shield").describe_protection_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/describe_protection_group.html)

```python
# describe_protection_group method definition

await def describe_protection_group(
    self,
    *,
    ProtectionGroupId: str,
) -> DescribeProtectionGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProtectionGroupResponseTypeDef](./type_defs.md#describeprotectiongroupresponsetypedef) 


```python
# describe_protection_group method usage example with argument unpacking

kwargs: DescribeProtectionGroupRequestTypeDef = {  # (1)
    "ProtectionGroupId": ...,
}

parent.describe_protection_group(**kwargs)
```

1. See [:material-code-braces: DescribeProtectionGroupRequestTypeDef](./type_defs.md#describeprotectiongrouprequesttypedef) 

### describe\_subscription

Provides details about the Shield Advanced subscription for an account.

Type annotations and code completion for `#!python session.create_client("shield").describe_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/describe_subscription.html)

```python
# describe_subscription method definition

await def describe_subscription(
    self,
) -> DescribeSubscriptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSubscriptionResponseTypeDef](./type_defs.md#describesubscriptionresponsetypedef) 

### disable\_application\_layer\_automatic\_response

Disable the Shield Advanced automatic application layer DDoS mitigation feature
for the protected resource.

Type annotations and code completion for `#!python session.create_client("shield").disable_application_layer_automatic_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/disable_application_layer_automatic_response.html)

```python
# disable_application_layer_automatic_response method definition

await def disable_application_layer_automatic_response(
    self,
    *,
    ResourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disable_application_layer_automatic_response method usage example with argument unpacking

kwargs: DisableApplicationLayerAutomaticResponseRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.disable_application_layer_automatic_response(**kwargs)
```

1. See [:material-code-braces: DisableApplicationLayerAutomaticResponseRequestTypeDef](./type_defs.md#disableapplicationlayerautomaticresponserequesttypedef) 

### disable\_proactive\_engagement

Removes authorization from the Shield Response Team (SRT) to notify contacts
about escalations to the SRT and to initiate proactive customer support.

Type annotations and code completion for `#!python session.create_client("shield").disable_proactive_engagement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/disable_proactive_engagement.html)

```python
# disable_proactive_engagement method definition

await def disable_proactive_engagement(
    self,
) -> Dict[str, Any]:
    ...
```


### disassociate\_drt\_log\_bucket

Removes the Shield Response Team's (SRT) access to the specified Amazon S3
bucket containing the logs that you shared previously.

Type annotations and code completion for `#!python session.create_client("shield").disassociate_drt_log_bucket` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/disassociate_drt_log_bucket.html)

```python
# disassociate_drt_log_bucket method definition

await def disassociate_drt_log_bucket(
    self,
    *,
    LogBucket: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_drt_log_bucket method usage example with argument unpacking

kwargs: DisassociateDRTLogBucketRequestTypeDef = {  # (1)
    "LogBucket": ...,
}

parent.disassociate_drt_log_bucket(**kwargs)
```

1. See [:material-code-braces: DisassociateDRTLogBucketRequestTypeDef](./type_defs.md#disassociatedrtlogbucketrequesttypedef) 

### disassociate\_drt\_role

Removes the Shield Response Team's (SRT) access to your Amazon Web Services
account.

Type annotations and code completion for `#!python session.create_client("shield").disassociate_drt_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/disassociate_drt_role.html)

```python
# disassociate_drt_role method definition

await def disassociate_drt_role(
    self,
) -> Dict[str, Any]:
    ...
```


### disassociate\_health\_check

Removes health-based detection from the Shield Advanced protection for a
resource.

Type annotations and code completion for `#!python session.create_client("shield").disassociate_health_check` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/disassociate_health_check.html)

```python
# disassociate_health_check method definition

await def disassociate_health_check(
    self,
    *,
    ProtectionId: str,
    HealthCheckArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_health_check method usage example with argument unpacking

kwargs: DisassociateHealthCheckRequestTypeDef = {  # (1)
    "ProtectionId": ...,
    "HealthCheckArn": ...,
}

parent.disassociate_health_check(**kwargs)
```

1. See [:material-code-braces: DisassociateHealthCheckRequestTypeDef](./type_defs.md#disassociatehealthcheckrequesttypedef) 

### enable\_application\_layer\_automatic\_response

Enable the Shield Advanced automatic application layer DDoS mitigation for the
protected resource.

Type annotations and code completion for `#!python session.create_client("shield").enable_application_layer_automatic_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/enable_application_layer_automatic_response.html)

```python
# enable_application_layer_automatic_response method definition

await def enable_application_layer_automatic_response(
    self,
    *,
    ResourceArn: str,
    Action: ResponseActionUnionTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ResponseActionTypeDef](./type_defs.md#responseactiontypedef) [:material-code-braces: ResponseActionOutputTypeDef](./type_defs.md#responseactionoutputtypedef) 


```python
# enable_application_layer_automatic_response method usage example with argument unpacking

kwargs: EnableApplicationLayerAutomaticResponseRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Action": ...,
}

parent.enable_application_layer_automatic_response(**kwargs)
```

1. See [:material-code-braces: EnableApplicationLayerAutomaticResponseRequestTypeDef](./type_defs.md#enableapplicationlayerautomaticresponserequesttypedef) 

### enable\_proactive\_engagement

Authorizes the Shield Response Team (SRT) to use email and phone to notify
contacts about escalations to the SRT and to initiate proactive customer
support.

Type annotations and code completion for `#!python session.create_client("shield").enable_proactive_engagement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/enable_proactive_engagement.html)

```python
# enable_proactive_engagement method definition

await def enable_proactive_engagement(
    self,
) -> Dict[str, Any]:
    ...
```


### get\_subscription\_state

Returns the <code>SubscriptionState</code>, either <code>Active</code> or
<code>Inactive</code>.

Type annotations and code completion for `#!python session.create_client("shield").get_subscription_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/get_subscription_state.html)

```python
# get_subscription_state method definition

await def get_subscription_state(
    self,
) -> GetSubscriptionStateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSubscriptionStateResponseTypeDef](./type_defs.md#getsubscriptionstateresponsetypedef) 

### list\_attacks

Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
period.

Type annotations and code completion for `#!python session.create_client("shield").list_attacks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/list_attacks.html)

```python
# list_attacks method definition

await def list_attacks(
    self,
    *,
    ResourceArns: Sequence[str] = ...,
    StartTime: TimeRangeUnionTypeDef = ...,  # (1)
    EndTime: TimeRangeUnionTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAttacksResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) [:material-code-braces: TimeRangeOutputTypeDef](./type_defs.md#timerangeoutputtypedef) 
2. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) [:material-code-braces: TimeRangeOutputTypeDef](./type_defs.md#timerangeoutputtypedef) 
3. See [:material-code-braces: ListAttacksResponseTypeDef](./type_defs.md#listattacksresponsetypedef) 


```python
# list_attacks method usage example with argument unpacking

kwargs: ListAttacksRequestTypeDef = {  # (1)
    "ResourceArns": ...,
}

parent.list_attacks(**kwargs)
```

1. See [:material-code-braces: ListAttacksRequestTypeDef](./type_defs.md#listattacksrequesttypedef) 

### list\_protection\_groups

Retrieves <a>ProtectionGroup</a> objects for the account.

Type annotations and code completion for `#!python session.create_client("shield").list_protection_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/list_protection_groups.html)

```python
# list_protection_groups method definition

await def list_protection_groups(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    InclusionFilters: InclusionProtectionGroupFiltersTypeDef = ...,  # (1)
) -> ListProtectionGroupsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InclusionProtectionGroupFiltersTypeDef](./type_defs.md#inclusionprotectiongroupfilterstypedef) 
2. See [:material-code-braces: ListProtectionGroupsResponseTypeDef](./type_defs.md#listprotectiongroupsresponsetypedef) 


```python
# list_protection_groups method usage example with argument unpacking

kwargs: ListProtectionGroupsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_protection_groups(**kwargs)
```

1. See [:material-code-braces: ListProtectionGroupsRequestTypeDef](./type_defs.md#listprotectiongroupsrequesttypedef) 

### list\_protections

Retrieves <a>Protection</a> objects for the account.

Type annotations and code completion for `#!python session.create_client("shield").list_protections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/list_protections.html)

```python
# list_protections method definition

await def list_protections(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    InclusionFilters: InclusionProtectionFiltersTypeDef = ...,  # (1)
) -> ListProtectionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InclusionProtectionFiltersTypeDef](./type_defs.md#inclusionprotectionfilterstypedef) 
2. See [:material-code-braces: ListProtectionsResponseTypeDef](./type_defs.md#listprotectionsresponsetypedef) 


```python
# list_protections method usage example with argument unpacking

kwargs: ListProtectionsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_protections(**kwargs)
```

1. See [:material-code-braces: ListProtectionsRequestTypeDef](./type_defs.md#listprotectionsrequesttypedef) 

### list\_resources\_in\_protection\_group

Retrieves the resources that are included in the protection group.

Type annotations and code completion for `#!python session.create_client("shield").list_resources_in_protection_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/list_resources_in_protection_group.html)

```python
# list_resources_in_protection_group method definition

await def list_resources_in_protection_group(
    self,
    *,
    ProtectionGroupId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListResourcesInProtectionGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResourcesInProtectionGroupResponseTypeDef](./type_defs.md#listresourcesinprotectiongroupresponsetypedef) 


```python
# list_resources_in_protection_group method usage example with argument unpacking

kwargs: ListResourcesInProtectionGroupRequestTypeDef = {  # (1)
    "ProtectionGroupId": ...,
}

parent.list_resources_in_protection_group(**kwargs)
```

1. See [:material-code-braces: ListResourcesInProtectionGroupRequestTypeDef](./type_defs.md#listresourcesinprotectiongrouprequesttypedef) 

### list\_tags\_for\_resource

Gets information about Amazon Web Services tags for a specified Amazon Resource
Name (ARN) in Shield.

Type annotations and code completion for `#!python session.create_client("shield").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
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

### tag\_resource

Adds or updates tags for a resource in Shield.

Type annotations and code completion for `#!python session.create_client("shield").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/tag_resource.html)

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

Removes tags from a resource in Shield.

Type annotations and code completion for `#!python session.create_client("shield").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/untag_resource.html)

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

### update\_application\_layer\_automatic\_response

Updates an existing Shield Advanced automatic application layer DDoS mitigation
configuration for the specified resource.

Type annotations and code completion for `#!python session.create_client("shield").update_application_layer_automatic_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/update_application_layer_automatic_response.html)

```python
# update_application_layer_automatic_response method definition

await def update_application_layer_automatic_response(
    self,
    *,
    ResourceArn: str,
    Action: ResponseActionUnionTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ResponseActionTypeDef](./type_defs.md#responseactiontypedef) [:material-code-braces: ResponseActionOutputTypeDef](./type_defs.md#responseactionoutputtypedef) 


```python
# update_application_layer_automatic_response method usage example with argument unpacking

kwargs: UpdateApplicationLayerAutomaticResponseRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Action": ...,
}

parent.update_application_layer_automatic_response(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationLayerAutomaticResponseRequestTypeDef](./type_defs.md#updateapplicationlayerautomaticresponserequesttypedef) 

### update\_emergency\_contact\_settings

Updates the details of the list of email addresses and phone numbers that the
Shield Response Team (SRT) can use to contact you if you have proactive
engagement enabled, for escalations to the SRT and to initiate proactive
customer support.

Type annotations and code completion for `#!python session.create_client("shield").update_emergency_contact_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/update_emergency_contact_settings.html)

```python
# update_emergency_contact_settings method definition

await def update_emergency_contact_settings(
    self,
    *,
    EmergencyContactList: Sequence[EmergencyContactTypeDef] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: EmergencyContactTypeDef](./type_defs.md#emergencycontacttypedef) 


```python
# update_emergency_contact_settings method usage example with argument unpacking

kwargs: UpdateEmergencyContactSettingsRequestTypeDef = {  # (1)
    "EmergencyContactList": ...,
}

parent.update_emergency_contact_settings(**kwargs)
```

1. See [:material-code-braces: UpdateEmergencyContactSettingsRequestTypeDef](./type_defs.md#updateemergencycontactsettingsrequesttypedef) 

### update\_protection\_group

Updates an existing protection group.

Type annotations and code completion for `#!python session.create_client("shield").update_protection_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/update_protection_group.html)

```python
# update_protection_group method definition

await def update_protection_group(
    self,
    *,
    ProtectionGroupId: str,
    Aggregation: ProtectionGroupAggregationType,  # (1)
    Pattern: ProtectionGroupPatternType,  # (2)
    ResourceType: ProtectedResourceTypeType = ...,  # (3)
    Members: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ProtectionGroupAggregationType](./literals.md#protectiongroupaggregationtype) 
2. See [:material-code-brackets: ProtectionGroupPatternType](./literals.md#protectiongrouppatterntype) 
3. See [:material-code-brackets: ProtectedResourceTypeType](./literals.md#protectedresourcetypetype) 


```python
# update_protection_group method usage example with argument unpacking

kwargs: UpdateProtectionGroupRequestTypeDef = {  # (1)
    "ProtectionGroupId": ...,
    "Aggregation": ...,
    "Pattern": ...,
}

parent.update_protection_group(**kwargs)
```

1. See [:material-code-braces: UpdateProtectionGroupRequestTypeDef](./type_defs.md#updateprotectiongrouprequesttypedef) 

### update\_subscription

Updates the details of an existing subscription.

Type annotations and code completion for `#!python session.create_client("shield").update_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/client/update_subscription.html)

```python
# update_subscription method definition

await def update_subscription(
    self,
    *,
    AutoRenew: AutoRenewType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: AutoRenewType](./literals.md#autorenewtype) 


```python
# update_subscription method usage example with argument unpacking

kwargs: UpdateSubscriptionRequestTypeDef = {  # (1)
    "AutoRenew": ...,
}

parent.update_subscription(**kwargs)
```

1. See [:material-code-braces: UpdateSubscriptionRequestTypeDef](./type_defs.md#updatesubscriptionrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("shield").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("shield").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("shield").get_paginator` method with overloads.

- `client.get_paginator("list_attacks")` -> [ListAttacksPaginator](./paginators.md#listattackspaginator)
- `client.get_paginator("list_protections")` -> [ListProtectionsPaginator](./paginators.md#listprotectionspaginator)



