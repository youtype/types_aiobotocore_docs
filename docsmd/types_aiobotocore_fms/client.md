# FMSClient

> [Index](../README.md) > [FMS](./README.md) > FMSClient

!!! note ""

    Auto-generated documentation for [FMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
    type annotations stubs module [types-aiobotocore-fms](https://pypi.org/project/types-aiobotocore-fms/).

## FMSClient

Type annotations and code completion for `#!python session.create_client("fms")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client)

```python
FMSClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_fms.client import FMSClient

session = get_session()
async with session.create_client("fms") as client:
    client: FMSClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("fms").exceptions` structure.

```python
FMSClient.exceptions usage example

async with session.create_client("fms") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalErrorException,
        client.InvalidInputException,
        client.InvalidOperationException,
        client.InvalidTypeException,
        client.LimitExceededException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
FMSClient usage type checking example

from types_aiobotocore_fms.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### associate\_admin\_account

Sets a Firewall Manager default administrator account.

Type annotations and code completion for `#!python session.create_client("fms").associate_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.associate_admin_account)

```python
# associate_admin_account method definition

await def associate_admin_account(
    self,
    *,
    AdminAccount: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_admin_account method usage example with argument unpacking

kwargs: AssociateAdminAccountRequestRequestTypeDef = {  # (1)
    "AdminAccount": ...,
}

parent.associate_admin_account(**kwargs)
```

1. See [:material-code-braces: AssociateAdminAccountRequestRequestTypeDef](./type_defs.md#associateadminaccountrequestrequesttypedef) 

### associate\_third\_party\_firewall

Sets the Firewall Manager policy administrator as a tenant administrator of a
third-party firewall service.

Type annotations and code completion for `#!python session.create_client("fms").associate_third_party_firewall` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.associate_third_party_firewall)

```python
# associate_third_party_firewall method definition

await def associate_third_party_firewall(
    self,
    *,
    ThirdPartyFirewall: ThirdPartyFirewallType,  # (1)
) -> AssociateThirdPartyFirewallResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ThirdPartyFirewallType](./literals.md#thirdpartyfirewalltype) 
2. See [:material-code-braces: AssociateThirdPartyFirewallResponseTypeDef](./type_defs.md#associatethirdpartyfirewallresponsetypedef) 


```python
# associate_third_party_firewall method usage example with argument unpacking

kwargs: AssociateThirdPartyFirewallRequestRequestTypeDef = {  # (1)
    "ThirdPartyFirewall": ...,
}

parent.associate_third_party_firewall(**kwargs)
```

1. See [:material-code-braces: AssociateThirdPartyFirewallRequestRequestTypeDef](./type_defs.md#associatethirdpartyfirewallrequestrequesttypedef) 

### batch\_associate\_resource

Associate resources to a Firewall Manager resource set.

Type annotations and code completion for `#!python session.create_client("fms").batch_associate_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.batch_associate_resource)

```python
# batch_associate_resource method definition

await def batch_associate_resource(
    self,
    *,
    ResourceSetIdentifier: str,
    Items: Sequence[str],
) -> BatchAssociateResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchAssociateResourceResponseTypeDef](./type_defs.md#batchassociateresourceresponsetypedef) 


```python
# batch_associate_resource method usage example with argument unpacking

kwargs: BatchAssociateResourceRequestRequestTypeDef = {  # (1)
    "ResourceSetIdentifier": ...,
    "Items": ...,
}

parent.batch_associate_resource(**kwargs)
```

1. See [:material-code-braces: BatchAssociateResourceRequestRequestTypeDef](./type_defs.md#batchassociateresourcerequestrequesttypedef) 

### batch\_disassociate\_resource

Disassociates resources from a Firewall Manager resource set.

Type annotations and code completion for `#!python session.create_client("fms").batch_disassociate_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.batch_disassociate_resource)

```python
# batch_disassociate_resource method definition

await def batch_disassociate_resource(
    self,
    *,
    ResourceSetIdentifier: str,
    Items: Sequence[str],
) -> BatchDisassociateResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDisassociateResourceResponseTypeDef](./type_defs.md#batchdisassociateresourceresponsetypedef) 


```python
# batch_disassociate_resource method usage example with argument unpacking

kwargs: BatchDisassociateResourceRequestRequestTypeDef = {  # (1)
    "ResourceSetIdentifier": ...,
    "Items": ...,
}

parent.batch_disassociate_resource(**kwargs)
```

1. See [:material-code-braces: BatchDisassociateResourceRequestRequestTypeDef](./type_defs.md#batchdisassociateresourcerequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("fms").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("fms").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### delete\_apps\_list

Permanently deletes an Firewall Manager applications list.

Type annotations and code completion for `#!python session.create_client("fms").delete_apps_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.delete_apps_list)

```python
# delete_apps_list method definition

await def delete_apps_list(
    self,
    *,
    ListId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_apps_list method usage example with argument unpacking

kwargs: DeleteAppsListRequestRequestTypeDef = {  # (1)
    "ListId": ...,
}

parent.delete_apps_list(**kwargs)
```

1. See [:material-code-braces: DeleteAppsListRequestRequestTypeDef](./type_defs.md#deleteappslistrequestrequesttypedef) 

### delete\_notification\_channel

Deletes an Firewall Manager association with the IAM role and the Amazon Simple
Notification Service (SNS) topic that is used to record Firewall Manager SNS
logs.

Type annotations and code completion for `#!python session.create_client("fms").delete_notification_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.delete_notification_channel)

```python
# delete_notification_channel method definition

await def delete_notification_channel(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 

### delete\_policy

Permanently deletes an Firewall Manager policy.

Type annotations and code completion for `#!python session.create_client("fms").delete_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.delete_policy)

```python
# delete_policy method definition

await def delete_policy(
    self,
    *,
    PolicyId: str,
    DeleteAllPolicyResources: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_policy method usage example with argument unpacking

kwargs: DeletePolicyRequestRequestTypeDef = {  # (1)
    "PolicyId": ...,
}

parent.delete_policy(**kwargs)
```

1. See [:material-code-braces: DeletePolicyRequestRequestTypeDef](./type_defs.md#deletepolicyrequestrequesttypedef) 

### delete\_protocols\_list

Permanently deletes an Firewall Manager protocols list.

Type annotations and code completion for `#!python session.create_client("fms").delete_protocols_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.delete_protocols_list)

```python
# delete_protocols_list method definition

await def delete_protocols_list(
    self,
    *,
    ListId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_protocols_list method usage example with argument unpacking

kwargs: DeleteProtocolsListRequestRequestTypeDef = {  # (1)
    "ListId": ...,
}

parent.delete_protocols_list(**kwargs)
```

1. See [:material-code-braces: DeleteProtocolsListRequestRequestTypeDef](./type_defs.md#deleteprotocolslistrequestrequesttypedef) 

### delete\_resource\_set

Deletes the specified  ResourceSet.

Type annotations and code completion for `#!python session.create_client("fms").delete_resource_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.delete_resource_set)

```python
# delete_resource_set method definition

await def delete_resource_set(
    self,
    *,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_resource_set method usage example with argument unpacking

kwargs: DeleteResourceSetRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.delete_resource_set(**kwargs)
```

1. See [:material-code-braces: DeleteResourceSetRequestRequestTypeDef](./type_defs.md#deleteresourcesetrequestrequesttypedef) 

### disassociate\_admin\_account

Disassociates an Firewall Manager administrator account.

Type annotations and code completion for `#!python session.create_client("fms").disassociate_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.disassociate_admin_account)

```python
# disassociate_admin_account method definition

await def disassociate_admin_account(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 

### disassociate\_third\_party\_firewall

Disassociates a Firewall Manager policy administrator from a third-party
firewall tenant.

Type annotations and code completion for `#!python session.create_client("fms").disassociate_third_party_firewall` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.disassociate_third_party_firewall)

```python
# disassociate_third_party_firewall method definition

await def disassociate_third_party_firewall(
    self,
    *,
    ThirdPartyFirewall: ThirdPartyFirewallType,  # (1)
) -> DisassociateThirdPartyFirewallResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ThirdPartyFirewallType](./literals.md#thirdpartyfirewalltype) 
2. See [:material-code-braces: DisassociateThirdPartyFirewallResponseTypeDef](./type_defs.md#disassociatethirdpartyfirewallresponsetypedef) 


```python
# disassociate_third_party_firewall method usage example with argument unpacking

kwargs: DisassociateThirdPartyFirewallRequestRequestTypeDef = {  # (1)
    "ThirdPartyFirewall": ...,
}

parent.disassociate_third_party_firewall(**kwargs)
```

1. See [:material-code-braces: DisassociateThirdPartyFirewallRequestRequestTypeDef](./type_defs.md#disassociatethirdpartyfirewallrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("fms").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.generate_presigned_url)

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


### get\_admin\_account

Returns the Organizations account that is associated with Firewall Manager as
the Firewall Manager default administrator.

Type annotations and code completion for `#!python session.create_client("fms").get_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_admin_account)

```python
# get_admin_account method definition

await def get_admin_account(
    self,
) -> GetAdminAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAdminAccountResponseTypeDef](./type_defs.md#getadminaccountresponsetypedef) 

### get\_admin\_scope

Returns information about the specified account's administrative scope.

Type annotations and code completion for `#!python session.create_client("fms").get_admin_scope` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_admin_scope)

```python
# get_admin_scope method definition

await def get_admin_scope(
    self,
    *,
    AdminAccount: str,
) -> GetAdminScopeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAdminScopeResponseTypeDef](./type_defs.md#getadminscoperesponsetypedef) 


```python
# get_admin_scope method usage example with argument unpacking

kwargs: GetAdminScopeRequestRequestTypeDef = {  # (1)
    "AdminAccount": ...,
}

parent.get_admin_scope(**kwargs)
```

1. See [:material-code-braces: GetAdminScopeRequestRequestTypeDef](./type_defs.md#getadminscoperequestrequesttypedef) 

### get\_apps\_list

Returns information about the specified Firewall Manager applications list.

Type annotations and code completion for `#!python session.create_client("fms").get_apps_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_apps_list)

```python
# get_apps_list method definition

await def get_apps_list(
    self,
    *,
    ListId: str,
    DefaultList: bool = ...,
) -> GetAppsListResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAppsListResponseTypeDef](./type_defs.md#getappslistresponsetypedef) 


```python
# get_apps_list method usage example with argument unpacking

kwargs: GetAppsListRequestRequestTypeDef = {  # (1)
    "ListId": ...,
}

parent.get_apps_list(**kwargs)
```

1. See [:material-code-braces: GetAppsListRequestRequestTypeDef](./type_defs.md#getappslistrequestrequesttypedef) 

### get\_compliance\_detail

Returns detailed compliance information about the specified member account.

Type annotations and code completion for `#!python session.create_client("fms").get_compliance_detail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_compliance_detail)

```python
# get_compliance_detail method definition

await def get_compliance_detail(
    self,
    *,
    PolicyId: str,
    MemberAccount: str,
) -> GetComplianceDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetComplianceDetailResponseTypeDef](./type_defs.md#getcompliancedetailresponsetypedef) 


```python
# get_compliance_detail method usage example with argument unpacking

kwargs: GetComplianceDetailRequestRequestTypeDef = {  # (1)
    "PolicyId": ...,
    "MemberAccount": ...,
}

parent.get_compliance_detail(**kwargs)
```

1. See [:material-code-braces: GetComplianceDetailRequestRequestTypeDef](./type_defs.md#getcompliancedetailrequestrequesttypedef) 

### get\_notification\_channel

Information about the Amazon Simple Notification Service (SNS) topic that is
used to record Firewall Manager SNS logs.

Type annotations and code completion for `#!python session.create_client("fms").get_notification_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_notification_channel)

```python
# get_notification_channel method definition

await def get_notification_channel(
    self,
) -> GetNotificationChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetNotificationChannelResponseTypeDef](./type_defs.md#getnotificationchannelresponsetypedef) 

### get\_policy

Returns information about the specified Firewall Manager policy.

Type annotations and code completion for `#!python session.create_client("fms").get_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_policy)

```python
# get_policy method definition

await def get_policy(
    self,
    *,
    PolicyId: str,
) -> GetPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyResponseTypeDef](./type_defs.md#getpolicyresponsetypedef) 


```python
# get_policy method usage example with argument unpacking

kwargs: GetPolicyRequestRequestTypeDef = {  # (1)
    "PolicyId": ...,
}

parent.get_policy(**kwargs)
```

1. See [:material-code-braces: GetPolicyRequestRequestTypeDef](./type_defs.md#getpolicyrequestrequesttypedef) 

### get\_protection\_status

If you created a Shield Advanced policy, returns policy-level attack summary
information in the event of a potential DDoS attack.

Type annotations and code completion for `#!python session.create_client("fms").get_protection_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_protection_status)

```python
# get_protection_status method definition

await def get_protection_status(
    self,
    *,
    PolicyId: str,
    MemberAccountId: str = ...,
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetProtectionStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProtectionStatusResponseTypeDef](./type_defs.md#getprotectionstatusresponsetypedef) 


```python
# get_protection_status method usage example with argument unpacking

kwargs: GetProtectionStatusRequestRequestTypeDef = {  # (1)
    "PolicyId": ...,
}

parent.get_protection_status(**kwargs)
```

1. See [:material-code-braces: GetProtectionStatusRequestRequestTypeDef](./type_defs.md#getprotectionstatusrequestrequesttypedef) 

### get\_protocols\_list

Returns information about the specified Firewall Manager protocols list.

Type annotations and code completion for `#!python session.create_client("fms").get_protocols_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_protocols_list)

```python
# get_protocols_list method definition

await def get_protocols_list(
    self,
    *,
    ListId: str,
    DefaultList: bool = ...,
) -> GetProtocolsListResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProtocolsListResponseTypeDef](./type_defs.md#getprotocolslistresponsetypedef) 


```python
# get_protocols_list method usage example with argument unpacking

kwargs: GetProtocolsListRequestRequestTypeDef = {  # (1)
    "ListId": ...,
}

parent.get_protocols_list(**kwargs)
```

1. See [:material-code-braces: GetProtocolsListRequestRequestTypeDef](./type_defs.md#getprotocolslistrequestrequesttypedef) 

### get\_resource\_set

Gets information about a specific resource set.

Type annotations and code completion for `#!python session.create_client("fms").get_resource_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_resource_set)

```python
# get_resource_set method definition

await def get_resource_set(
    self,
    *,
    Identifier: str,
) -> GetResourceSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourceSetResponseTypeDef](./type_defs.md#getresourcesetresponsetypedef) 


```python
# get_resource_set method usage example with argument unpacking

kwargs: GetResourceSetRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.get_resource_set(**kwargs)
```

1. See [:material-code-braces: GetResourceSetRequestRequestTypeDef](./type_defs.md#getresourcesetrequestrequesttypedef) 

### get\_third\_party\_firewall\_association\_status

The onboarding status of a Firewall Manager admin account to third-party
firewall vendor tenant.

Type annotations and code completion for `#!python session.create_client("fms").get_third_party_firewall_association_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_third_party_firewall_association_status)

```python
# get_third_party_firewall_association_status method definition

await def get_third_party_firewall_association_status(
    self,
    *,
    ThirdPartyFirewall: ThirdPartyFirewallType,  # (1)
) -> GetThirdPartyFirewallAssociationStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ThirdPartyFirewallType](./literals.md#thirdpartyfirewalltype) 
2. See [:material-code-braces: GetThirdPartyFirewallAssociationStatusResponseTypeDef](./type_defs.md#getthirdpartyfirewallassociationstatusresponsetypedef) 


```python
# get_third_party_firewall_association_status method usage example with argument unpacking

kwargs: GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef = {  # (1)
    "ThirdPartyFirewall": ...,
}

parent.get_third_party_firewall_association_status(**kwargs)
```

1. See [:material-code-braces: GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef](./type_defs.md#getthirdpartyfirewallassociationstatusrequestrequesttypedef) 

### get\_violation\_details

Retrieves violations for a resource based on the specified Firewall Manager
policy and Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("fms").get_violation_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_violation_details)

```python
# get_violation_details method definition

await def get_violation_details(
    self,
    *,
    PolicyId: str,
    MemberAccount: str,
    ResourceId: str,
    ResourceType: str,
) -> GetViolationDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetViolationDetailsResponseTypeDef](./type_defs.md#getviolationdetailsresponsetypedef) 


```python
# get_violation_details method usage example with argument unpacking

kwargs: GetViolationDetailsRequestRequestTypeDef = {  # (1)
    "PolicyId": ...,
    "MemberAccount": ...,
    "ResourceId": ...,
    "ResourceType": ...,
}

parent.get_violation_details(**kwargs)
```

1. See [:material-code-braces: GetViolationDetailsRequestRequestTypeDef](./type_defs.md#getviolationdetailsrequestrequesttypedef) 

### list\_admin\_accounts\_for\_organization

Returns a `AdminAccounts` object that lists the Firewall Manager administrators
within the organization that are onboarded to Firewall Manager by
AssociateAdminAccount.

Type annotations and code completion for `#!python session.create_client("fms").list_admin_accounts_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_admin_accounts_for_organization)

```python
# list_admin_accounts_for_organization method definition

await def list_admin_accounts_for_organization(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAdminAccountsForOrganizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAdminAccountsForOrganizationResponseTypeDef](./type_defs.md#listadminaccountsfororganizationresponsetypedef) 


```python
# list_admin_accounts_for_organization method usage example with argument unpacking

kwargs: ListAdminAccountsForOrganizationRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_admin_accounts_for_organization(**kwargs)
```

1. See [:material-code-braces: ListAdminAccountsForOrganizationRequestRequestTypeDef](./type_defs.md#listadminaccountsfororganizationrequestrequesttypedef) 

### list\_admins\_managing\_account

Lists the accounts that are managing the specified Organizations member account.

Type annotations and code completion for `#!python session.create_client("fms").list_admins_managing_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_admins_managing_account)

```python
# list_admins_managing_account method definition

await def list_admins_managing_account(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAdminsManagingAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAdminsManagingAccountResponseTypeDef](./type_defs.md#listadminsmanagingaccountresponsetypedef) 


```python
# list_admins_managing_account method usage example with argument unpacking

kwargs: ListAdminsManagingAccountRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_admins_managing_account(**kwargs)
```

1. See [:material-code-braces: ListAdminsManagingAccountRequestRequestTypeDef](./type_defs.md#listadminsmanagingaccountrequestrequesttypedef) 

### list\_apps\_lists

Returns an array of `AppsListDataSummary` objects.

Type annotations and code completion for `#!python session.create_client("fms").list_apps_lists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_apps_lists)

```python
# list_apps_lists method definition

await def list_apps_lists(
    self,
    *,
    MaxResults: int,
    DefaultLists: bool = ...,
    NextToken: str = ...,
) -> ListAppsListsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppsListsResponseTypeDef](./type_defs.md#listappslistsresponsetypedef) 


```python
# list_apps_lists method usage example with argument unpacking

kwargs: ListAppsListsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_apps_lists(**kwargs)
```

1. See [:material-code-braces: ListAppsListsRequestRequestTypeDef](./type_defs.md#listappslistsrequestrequesttypedef) 

### list\_compliance\_status

Returns an array of `PolicyComplianceStatus` objects.

Type annotations and code completion for `#!python session.create_client("fms").list_compliance_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_compliance_status)

```python
# list_compliance_status method definition

await def list_compliance_status(
    self,
    *,
    PolicyId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListComplianceStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListComplianceStatusResponseTypeDef](./type_defs.md#listcompliancestatusresponsetypedef) 


```python
# list_compliance_status method usage example with argument unpacking

kwargs: ListComplianceStatusRequestRequestTypeDef = {  # (1)
    "PolicyId": ...,
}

parent.list_compliance_status(**kwargs)
```

1. See [:material-code-braces: ListComplianceStatusRequestRequestTypeDef](./type_defs.md#listcompliancestatusrequestrequesttypedef) 

### list\_discovered\_resources

Returns an array of resources in the organization's accounts that are available
to be associated with a resource set.

Type annotations and code completion for `#!python session.create_client("fms").list_discovered_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_discovered_resources)

```python
# list_discovered_resources method definition

await def list_discovered_resources(
    self,
    *,
    MemberAccountIds: Sequence[str],
    ResourceType: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDiscoveredResourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDiscoveredResourcesResponseTypeDef](./type_defs.md#listdiscoveredresourcesresponsetypedef) 


```python
# list_discovered_resources method usage example with argument unpacking

kwargs: ListDiscoveredResourcesRequestRequestTypeDef = {  # (1)
    "MemberAccountIds": ...,
    "ResourceType": ...,
}

parent.list_discovered_resources(**kwargs)
```

1. See [:material-code-braces: ListDiscoveredResourcesRequestRequestTypeDef](./type_defs.md#listdiscoveredresourcesrequestrequesttypedef) 

### list\_member\_accounts

Returns a `MemberAccounts` object that lists the member accounts in the
administrator's Amazon Web Services organization.

Type annotations and code completion for `#!python session.create_client("fms").list_member_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_member_accounts)

```python
# list_member_accounts method definition

await def list_member_accounts(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMemberAccountsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMemberAccountsResponseTypeDef](./type_defs.md#listmemberaccountsresponsetypedef) 


```python
# list_member_accounts method usage example with argument unpacking

kwargs: ListMemberAccountsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_member_accounts(**kwargs)
```

1. See [:material-code-braces: ListMemberAccountsRequestRequestTypeDef](./type_defs.md#listmemberaccountsrequestrequesttypedef) 

### list\_policies

Returns an array of `PolicySummary` objects.

Type annotations and code completion for `#!python session.create_client("fms").list_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_policies)

```python
# list_policies method definition

await def list_policies(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


```python
# list_policies method usage example with argument unpacking

kwargs: ListPoliciesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_policies(**kwargs)
```

1. See [:material-code-braces: ListPoliciesRequestRequestTypeDef](./type_defs.md#listpoliciesrequestrequesttypedef) 

### list\_protocols\_lists

Returns an array of `ProtocolsListDataSummary` objects.

Type annotations and code completion for `#!python session.create_client("fms").list_protocols_lists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_protocols_lists)

```python
# list_protocols_lists method definition

await def list_protocols_lists(
    self,
    *,
    MaxResults: int,
    DefaultLists: bool = ...,
    NextToken: str = ...,
) -> ListProtocolsListsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProtocolsListsResponseTypeDef](./type_defs.md#listprotocolslistsresponsetypedef) 


```python
# list_protocols_lists method usage example with argument unpacking

kwargs: ListProtocolsListsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_protocols_lists(**kwargs)
```

1. See [:material-code-braces: ListProtocolsListsRequestRequestTypeDef](./type_defs.md#listprotocolslistsrequestrequesttypedef) 

### list\_resource\_set\_resources

Returns an array of resources that are currently associated to a resource set.

Type annotations and code completion for `#!python session.create_client("fms").list_resource_set_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_resource_set_resources)

```python
# list_resource_set_resources method definition

await def list_resource_set_resources(
    self,
    *,
    Identifier: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListResourceSetResourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResourceSetResourcesResponseTypeDef](./type_defs.md#listresourcesetresourcesresponsetypedef) 


```python
# list_resource_set_resources method usage example with argument unpacking

kwargs: ListResourceSetResourcesRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.list_resource_set_resources(**kwargs)
```

1. See [:material-code-braces: ListResourceSetResourcesRequestRequestTypeDef](./type_defs.md#listresourcesetresourcesrequestrequesttypedef) 

### list\_resource\_sets

Returns an array of `ResourceSetSummary` objects.

Type annotations and code completion for `#!python session.create_client("fms").list_resource_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_resource_sets)

```python
# list_resource_sets method definition

await def list_resource_sets(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListResourceSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResourceSetsResponseTypeDef](./type_defs.md#listresourcesetsresponsetypedef) 


```python
# list_resource_sets method usage example with argument unpacking

kwargs: ListResourceSetsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_resource_sets(**kwargs)
```

1. See [:material-code-braces: ListResourceSetsRequestRequestTypeDef](./type_defs.md#listresourcesetsrequestrequesttypedef) 

### list\_tags\_for\_resource

Retrieves the list of tags for the specified Amazon Web Services resource.

Type annotations and code completion for `#!python session.create_client("fms").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
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

### list\_third\_party\_firewall\_firewall\_policies

Retrieves a list of all of the third-party firewall policies that are associated
with the third-party firewall administrator's account.

Type annotations and code completion for `#!python session.create_client("fms").list_third_party_firewall_firewall_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)

```python
# list_third_party_firewall_firewall_policies method definition

await def list_third_party_firewall_firewall_policies(
    self,
    *,
    ThirdPartyFirewall: ThirdPartyFirewallType,  # (1)
    MaxResults: int,
    NextToken: str = ...,
) -> ListThirdPartyFirewallFirewallPoliciesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ThirdPartyFirewallType](./literals.md#thirdpartyfirewalltype) 
2. See [:material-code-braces: ListThirdPartyFirewallFirewallPoliciesResponseTypeDef](./type_defs.md#listthirdpartyfirewallfirewallpoliciesresponsetypedef) 


```python
# list_third_party_firewall_firewall_policies method usage example with argument unpacking

kwargs: ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = {  # (1)
    "ThirdPartyFirewall": ...,
    "MaxResults": ...,
}

parent.list_third_party_firewall_firewall_policies(**kwargs)
```

1. See [:material-code-braces: ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef](./type_defs.md#listthirdpartyfirewallfirewallpoliciesrequestrequesttypedef) 

### put\_admin\_account

Creates or updates an Firewall Manager administrator account.

Type annotations and code completion for `#!python session.create_client("fms").put_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_admin_account)

```python
# put_admin_account method definition

await def put_admin_account(
    self,
    *,
    AdminAccount: str,
    AdminScope: AdminScopeTypeDef = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AdminScopeTypeDef](./type_defs.md#adminscopetypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_admin_account method usage example with argument unpacking

kwargs: PutAdminAccountRequestRequestTypeDef = {  # (1)
    "AdminAccount": ...,
}

parent.put_admin_account(**kwargs)
```

1. See [:material-code-braces: PutAdminAccountRequestRequestTypeDef](./type_defs.md#putadminaccountrequestrequesttypedef) 

### put\_apps\_list

Creates an Firewall Manager applications list.

Type annotations and code completion for `#!python session.create_client("fms").put_apps_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_apps_list)

```python
# put_apps_list method definition

await def put_apps_list(
    self,
    *,
    AppsList: AppsListDataTypeDef,  # (1)
    TagList: Sequence[TagTypeDef] = ...,  # (2)
) -> PutAppsListResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AppsListDataTypeDef](./type_defs.md#appslistdatatypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: PutAppsListResponseTypeDef](./type_defs.md#putappslistresponsetypedef) 


```python
# put_apps_list method usage example with argument unpacking

kwargs: PutAppsListRequestRequestTypeDef = {  # (1)
    "AppsList": ...,
}

parent.put_apps_list(**kwargs)
```

1. See [:material-code-braces: PutAppsListRequestRequestTypeDef](./type_defs.md#putappslistrequestrequesttypedef) 

### put\_notification\_channel

Designates the IAM role and Amazon Simple Notification Service (SNS) topic that
Firewall Manager uses to record SNS logs.

Type annotations and code completion for `#!python session.create_client("fms").put_notification_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_notification_channel)

```python
# put_notification_channel method definition

await def put_notification_channel(
    self,
    *,
    SnsTopicArn: str,
    SnsRoleName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_notification_channel method usage example with argument unpacking

kwargs: PutNotificationChannelRequestRequestTypeDef = {  # (1)
    "SnsTopicArn": ...,
    "SnsRoleName": ...,
}

parent.put_notification_channel(**kwargs)
```

1. See [:material-code-braces: PutNotificationChannelRequestRequestTypeDef](./type_defs.md#putnotificationchannelrequestrequesttypedef) 

### put\_policy

Creates an Firewall Manager policy.

Type annotations and code completion for `#!python session.create_client("fms").put_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_policy)

```python
# put_policy method definition

await def put_policy(
    self,
    *,
    Policy: PolicyTypeDef,  # (1)
    TagList: Sequence[TagTypeDef] = ...,  # (2)
) -> PutPolicyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: PutPolicyResponseTypeDef](./type_defs.md#putpolicyresponsetypedef) 


```python
# put_policy method usage example with argument unpacking

kwargs: PutPolicyRequestRequestTypeDef = {  # (1)
    "Policy": ...,
}

parent.put_policy(**kwargs)
```

1. See [:material-code-braces: PutPolicyRequestRequestTypeDef](./type_defs.md#putpolicyrequestrequesttypedef) 

### put\_protocols\_list

Creates an Firewall Manager protocols list.

Type annotations and code completion for `#!python session.create_client("fms").put_protocols_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_protocols_list)

```python
# put_protocols_list method definition

await def put_protocols_list(
    self,
    *,
    ProtocolsList: ProtocolsListDataTypeDef,  # (1)
    TagList: Sequence[TagTypeDef] = ...,  # (2)
) -> PutProtocolsListResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ProtocolsListDataTypeDef](./type_defs.md#protocolslistdatatypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: PutProtocolsListResponseTypeDef](./type_defs.md#putprotocolslistresponsetypedef) 


```python
# put_protocols_list method usage example with argument unpacking

kwargs: PutProtocolsListRequestRequestTypeDef = {  # (1)
    "ProtocolsList": ...,
}

parent.put_protocols_list(**kwargs)
```

1. See [:material-code-braces: PutProtocolsListRequestRequestTypeDef](./type_defs.md#putprotocolslistrequestrequesttypedef) 

### put\_resource\_set

Creates the resource set.

Type annotations and code completion for `#!python session.create_client("fms").put_resource_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_resource_set)

```python
# put_resource_set method definition

await def put_resource_set(
    self,
    *,
    ResourceSet: ResourceSetTypeDef,  # (1)
    TagList: Sequence[TagTypeDef] = ...,  # (2)
) -> PutResourceSetResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourceSetTypeDef](./type_defs.md#resourcesettypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: PutResourceSetResponseTypeDef](./type_defs.md#putresourcesetresponsetypedef) 


```python
# put_resource_set method usage example with argument unpacking

kwargs: PutResourceSetRequestRequestTypeDef = {  # (1)
    "ResourceSet": ...,
}

parent.put_resource_set(**kwargs)
```

1. See [:material-code-braces: PutResourceSetRequestRequestTypeDef](./type_defs.md#putresourcesetrequestrequesttypedef) 

### tag\_resource

Adds one or more tags to an Amazon Web Services resource.

Type annotations and code completion for `#!python session.create_client("fms").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    TagList: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagList": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes one or more tags from an Amazon Web Services resource.

Type annotations and code completion for `#!python session.create_client("fms").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.untag_resource)

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

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("fms").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> FMSClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("fms").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("fms").get_paginator` method with overloads.

- `client.get_paginator("list_admin_accounts_for_organization")` -> [ListAdminAccountsForOrganizationPaginator](./paginators.md#listadminaccountsfororganizationpaginator)
- `client.get_paginator("list_admins_managing_account")` -> [ListAdminsManagingAccountPaginator](./paginators.md#listadminsmanagingaccountpaginator)
- `client.get_paginator("list_apps_lists")` -> [ListAppsListsPaginator](./paginators.md#listappslistspaginator)
- `client.get_paginator("list_compliance_status")` -> [ListComplianceStatusPaginator](./paginators.md#listcompliancestatuspaginator)
- `client.get_paginator("list_member_accounts")` -> [ListMemberAccountsPaginator](./paginators.md#listmemberaccountspaginator)
- `client.get_paginator("list_policies")` -> [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
- `client.get_paginator("list_protocols_lists")` -> [ListProtocolsListsPaginator](./paginators.md#listprotocolslistspaginator)
- `client.get_paginator("list_third_party_firewall_firewall_policies")` -> [ListThirdPartyFirewallFirewallPoliciesPaginator](./paginators.md#listthirdpartyfirewallfirewallpoliciespaginator)



