# MailManagerClient

> [Index](../README.md) > [MailManager](./README.md) > MailManagerClient

!!! note ""

    Auto-generated documentation for [MailManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager.html#mailmanager)
    type annotations stubs module [types-aiobotocore-mailmanager](https://pypi.org/project/types-aiobotocore-mailmanager/).

## MailManagerClient

Type annotations and code completion for `#!python session.create_client("mailmanager")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager.html#MailManager.Client)

```python
# MailManagerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_mailmanager.client import MailManagerClient

session = get_session()
async with session.create_client("mailmanager") as client:
    client: MailManagerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("mailmanager").exceptions` structure.

```python
# MailManagerClient.exceptions usage example

async with session.create_client("mailmanager") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# MailManagerClient usage type checking example

from types_aiobotocore_mailmanager.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("mailmanager").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("mailmanager").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/generate_presigned_url.html)

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



Type annotations and code completion for `#!python session.create_client("mailmanager").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_addon\_instance

Creates an Add On instance for the subscription indicated in the request.

Type annotations and code completion for `#!python session.create_client("mailmanager").create_addon_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/create_addon_instance.html)

```python
# create_addon_instance method definition

await def create_addon_instance(
    self,
    *,
    AddonSubscriptionId: str,
    ClientToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateAddonInstanceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateAddonInstanceResponseTypeDef](./type_defs.md#createaddoninstanceresponsetypedef) 


```python
# create_addon_instance method usage example with argument unpacking

kwargs: CreateAddonInstanceRequestRequestTypeDef = {  # (1)
    "AddonSubscriptionId": ...,
}

parent.create_addon_instance(**kwargs)
```

1. See [:material-code-braces: CreateAddonInstanceRequestRequestTypeDef](./type_defs.md#createaddoninstancerequestrequesttypedef) 

### create\_addon\_subscription

Creates a subscription for an Add On representing the acceptance of its terms
of use and additional pricing.

Type annotations and code completion for `#!python session.create_client("mailmanager").create_addon_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/create_addon_subscription.html)

```python
# create_addon_subscription method definition

await def create_addon_subscription(
    self,
    *,
    AddonName: str,
    ClientToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateAddonSubscriptionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateAddonSubscriptionResponseTypeDef](./type_defs.md#createaddonsubscriptionresponsetypedef) 


```python
# create_addon_subscription method usage example with argument unpacking

kwargs: CreateAddonSubscriptionRequestRequestTypeDef = {  # (1)
    "AddonName": ...,
}

parent.create_addon_subscription(**kwargs)
```

1. See [:material-code-braces: CreateAddonSubscriptionRequestRequestTypeDef](./type_defs.md#createaddonsubscriptionrequestrequesttypedef) 

### create\_archive

Creates a new email archive resource for storing and retaining emails.

Type annotations and code completion for `#!python session.create_client("mailmanager").create_archive` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/create_archive.html)

```python
# create_archive method definition

await def create_archive(
    self,
    *,
    ArchiveName: str,
    ClientToken: str = ...,
    KmsKeyArn: str = ...,
    Retention: ArchiveRetentionTypeDef = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateArchiveResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ArchiveRetentionTypeDef](./type_defs.md#archiveretentiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateArchiveResponseTypeDef](./type_defs.md#createarchiveresponsetypedef) 


```python
# create_archive method usage example with argument unpacking

kwargs: CreateArchiveRequestRequestTypeDef = {  # (1)
    "ArchiveName": ...,
}

parent.create_archive(**kwargs)
```

1. See [:material-code-braces: CreateArchiveRequestRequestTypeDef](./type_defs.md#createarchiverequestrequesttypedef) 

### create\_ingress\_point

Provision a new ingress endpoint resource.

Type annotations and code completion for `#!python session.create_client("mailmanager").create_ingress_point` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/create_ingress_point.html)

```python
# create_ingress_point method definition

await def create_ingress_point(
    self,
    *,
    IngressPointName: str,
    RuleSetId: str,
    TrafficPolicyId: str,
    Type: IngressPointTypeType,  # (1)
    ClientToken: str = ...,
    IngressPointConfiguration: IngressPointConfigurationTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateIngressPointResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: IngressPointTypeType](./literals.md#ingresspointtypetype) 
2. See [:material-code-braces: IngressPointConfigurationTypeDef](./type_defs.md#ingresspointconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateIngressPointResponseTypeDef](./type_defs.md#createingresspointresponsetypedef) 


```python
# create_ingress_point method usage example with argument unpacking

kwargs: CreateIngressPointRequestRequestTypeDef = {  # (1)
    "IngressPointName": ...,
    "RuleSetId": ...,
    "TrafficPolicyId": ...,
    "Type": ...,
}

parent.create_ingress_point(**kwargs)
```

1. See [:material-code-braces: CreateIngressPointRequestRequestTypeDef](./type_defs.md#createingresspointrequestrequesttypedef) 

### create\_relay

Creates a relay resource which can be used in rules to relay incoming emails to
defined relay destinations.

Type annotations and code completion for `#!python session.create_client("mailmanager").create_relay` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/create_relay.html)

```python
# create_relay method definition

await def create_relay(
    self,
    *,
    Authentication: RelayAuthenticationTypeDef,  # (1)
    RelayName: str,
    ServerName: str,
    ServerPort: int,
    ClientToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateRelayResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RelayAuthenticationTypeDef](./type_defs.md#relayauthenticationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateRelayResponseTypeDef](./type_defs.md#createrelayresponsetypedef) 


```python
# create_relay method usage example with argument unpacking

kwargs: CreateRelayRequestRequestTypeDef = {  # (1)
    "Authentication": ...,
    "RelayName": ...,
    "ServerName": ...,
    "ServerPort": ...,
}

parent.create_relay(**kwargs)
```

1. See [:material-code-braces: CreateRelayRequestRequestTypeDef](./type_defs.md#createrelayrequestrequesttypedef) 

### create\_rule\_set

Provision a new rule set.

Type annotations and code completion for `#!python session.create_client("mailmanager").create_rule_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/create_rule_set.html)

```python
# create_rule_set method definition

await def create_rule_set(
    self,
    *,
    RuleSetName: str,
    Rules: Sequence[RuleUnionTypeDef],  # (1)
    ClientToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateRuleSetResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateRuleSetResponseTypeDef](./type_defs.md#createrulesetresponsetypedef) 


```python
# create_rule_set method usage example with argument unpacking

kwargs: CreateRuleSetRequestRequestTypeDef = {  # (1)
    "RuleSetName": ...,
    "Rules": ...,
}

parent.create_rule_set(**kwargs)
```

1. See [:material-code-braces: CreateRuleSetRequestRequestTypeDef](./type_defs.md#createrulesetrequestrequesttypedef) 

### create\_traffic\_policy

Provision a new traffic policy resource.

Type annotations and code completion for `#!python session.create_client("mailmanager").create_traffic_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/create_traffic_policy.html)

```python
# create_traffic_policy method definition

await def create_traffic_policy(
    self,
    *,
    DefaultAction: AcceptActionType,  # (1)
    PolicyStatements: Sequence[PolicyStatementUnionTypeDef],  # (2)
    TrafficPolicyName: str,
    ClientToken: str = ...,
    MaxMessageSizeBytes: int = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateTrafficPolicyResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AcceptActionType](./literals.md#acceptactiontype) 
2. See [:material-code-braces: PolicyStatementTypeDef](./type_defs.md#policystatementtypedef) [:material-code-braces: PolicyStatementOutputTypeDef](./type_defs.md#policystatementoutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateTrafficPolicyResponseTypeDef](./type_defs.md#createtrafficpolicyresponsetypedef) 


```python
# create_traffic_policy method usage example with argument unpacking

kwargs: CreateTrafficPolicyRequestRequestTypeDef = {  # (1)
    "DefaultAction": ...,
    "PolicyStatements": ...,
    "TrafficPolicyName": ...,
}

parent.create_traffic_policy(**kwargs)
```

1. See [:material-code-braces: CreateTrafficPolicyRequestRequestTypeDef](./type_defs.md#createtrafficpolicyrequestrequesttypedef) 

### delete\_addon\_instance

Deletes an Add On instance.

Type annotations and code completion for `#!python session.create_client("mailmanager").delete_addon_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/delete_addon_instance.html)

```python
# delete_addon_instance method definition

await def delete_addon_instance(
    self,
    *,
    AddonInstanceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_addon_instance method usage example with argument unpacking

kwargs: DeleteAddonInstanceRequestRequestTypeDef = {  # (1)
    "AddonInstanceId": ...,
}

parent.delete_addon_instance(**kwargs)
```

1. See [:material-code-braces: DeleteAddonInstanceRequestRequestTypeDef](./type_defs.md#deleteaddoninstancerequestrequesttypedef) 

### delete\_addon\_subscription

Deletes an Add On subscription.

Type annotations and code completion for `#!python session.create_client("mailmanager").delete_addon_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/delete_addon_subscription.html)

```python
# delete_addon_subscription method definition

await def delete_addon_subscription(
    self,
    *,
    AddonSubscriptionId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_addon_subscription method usage example with argument unpacking

kwargs: DeleteAddonSubscriptionRequestRequestTypeDef = {  # (1)
    "AddonSubscriptionId": ...,
}

parent.delete_addon_subscription(**kwargs)
```

1. See [:material-code-braces: DeleteAddonSubscriptionRequestRequestTypeDef](./type_defs.md#deleteaddonsubscriptionrequestrequesttypedef) 

### delete\_archive

Initiates deletion of an email archive.

Type annotations and code completion for `#!python session.create_client("mailmanager").delete_archive` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/delete_archive.html)

```python
# delete_archive method definition

await def delete_archive(
    self,
    *,
    ArchiveId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_archive method usage example with argument unpacking

kwargs: DeleteArchiveRequestRequestTypeDef = {  # (1)
    "ArchiveId": ...,
}

parent.delete_archive(**kwargs)
```

1. See [:material-code-braces: DeleteArchiveRequestRequestTypeDef](./type_defs.md#deletearchiverequestrequesttypedef) 

### delete\_ingress\_point

Delete an ingress endpoint resource.

Type annotations and code completion for `#!python session.create_client("mailmanager").delete_ingress_point` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/delete_ingress_point.html)

```python
# delete_ingress_point method definition

await def delete_ingress_point(
    self,
    *,
    IngressPointId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ingress_point method usage example with argument unpacking

kwargs: DeleteIngressPointRequestRequestTypeDef = {  # (1)
    "IngressPointId": ...,
}

parent.delete_ingress_point(**kwargs)
```

1. See [:material-code-braces: DeleteIngressPointRequestRequestTypeDef](./type_defs.md#deleteingresspointrequestrequesttypedef) 

### delete\_relay

Deletes an existing relay resource.

Type annotations and code completion for `#!python session.create_client("mailmanager").delete_relay` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/delete_relay.html)

```python
# delete_relay method definition

await def delete_relay(
    self,
    *,
    RelayId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_relay method usage example with argument unpacking

kwargs: DeleteRelayRequestRequestTypeDef = {  # (1)
    "RelayId": ...,
}

parent.delete_relay(**kwargs)
```

1. See [:material-code-braces: DeleteRelayRequestRequestTypeDef](./type_defs.md#deleterelayrequestrequesttypedef) 

### delete\_rule\_set

Delete a rule set.

Type annotations and code completion for `#!python session.create_client("mailmanager").delete_rule_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/delete_rule_set.html)

```python
# delete_rule_set method definition

await def delete_rule_set(
    self,
    *,
    RuleSetId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_rule_set method usage example with argument unpacking

kwargs: DeleteRuleSetRequestRequestTypeDef = {  # (1)
    "RuleSetId": ...,
}

parent.delete_rule_set(**kwargs)
```

1. See [:material-code-braces: DeleteRuleSetRequestRequestTypeDef](./type_defs.md#deleterulesetrequestrequesttypedef) 

### delete\_traffic\_policy

Delete a traffic policy resource.

Type annotations and code completion for `#!python session.create_client("mailmanager").delete_traffic_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/delete_traffic_policy.html)

```python
# delete_traffic_policy method definition

await def delete_traffic_policy(
    self,
    *,
    TrafficPolicyId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_traffic_policy method usage example with argument unpacking

kwargs: DeleteTrafficPolicyRequestRequestTypeDef = {  # (1)
    "TrafficPolicyId": ...,
}

parent.delete_traffic_policy(**kwargs)
```

1. See [:material-code-braces: DeleteTrafficPolicyRequestRequestTypeDef](./type_defs.md#deletetrafficpolicyrequestrequesttypedef) 

### get\_addon\_instance

Gets detailed information about an Add On instance.

Type annotations and code completion for `#!python session.create_client("mailmanager").get_addon_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/get_addon_instance.html)

```python
# get_addon_instance method definition

await def get_addon_instance(
    self,
    *,
    AddonInstanceId: str,
) -> GetAddonInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAddonInstanceResponseTypeDef](./type_defs.md#getaddoninstanceresponsetypedef) 


```python
# get_addon_instance method usage example with argument unpacking

kwargs: GetAddonInstanceRequestRequestTypeDef = {  # (1)
    "AddonInstanceId": ...,
}

parent.get_addon_instance(**kwargs)
```

1. See [:material-code-braces: GetAddonInstanceRequestRequestTypeDef](./type_defs.md#getaddoninstancerequestrequesttypedef) 

### get\_addon\_subscription

Gets detailed information about an Add On subscription.

Type annotations and code completion for `#!python session.create_client("mailmanager").get_addon_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/get_addon_subscription.html)

```python
# get_addon_subscription method definition

await def get_addon_subscription(
    self,
    *,
    AddonSubscriptionId: str,
) -> GetAddonSubscriptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAddonSubscriptionResponseTypeDef](./type_defs.md#getaddonsubscriptionresponsetypedef) 


```python
# get_addon_subscription method usage example with argument unpacking

kwargs: GetAddonSubscriptionRequestRequestTypeDef = {  # (1)
    "AddonSubscriptionId": ...,
}

parent.get_addon_subscription(**kwargs)
```

1. See [:material-code-braces: GetAddonSubscriptionRequestRequestTypeDef](./type_defs.md#getaddonsubscriptionrequestrequesttypedef) 

### get\_archive

Retrieves the full details and current state of a specified email archive.

Type annotations and code completion for `#!python session.create_client("mailmanager").get_archive` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/get_archive.html)

```python
# get_archive method definition

await def get_archive(
    self,
    *,
    ArchiveId: str,
) -> GetArchiveResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetArchiveResponseTypeDef](./type_defs.md#getarchiveresponsetypedef) 


```python
# get_archive method usage example with argument unpacking

kwargs: GetArchiveRequestRequestTypeDef = {  # (1)
    "ArchiveId": ...,
}

parent.get_archive(**kwargs)
```

1. See [:material-code-braces: GetArchiveRequestRequestTypeDef](./type_defs.md#getarchiverequestrequesttypedef) 

### get\_archive\_export

Retrieves the details and current status of a specific email archive export job.

Type annotations and code completion for `#!python session.create_client("mailmanager").get_archive_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/get_archive_export.html)

```python
# get_archive_export method definition

await def get_archive_export(
    self,
    *,
    ExportId: str,
) -> GetArchiveExportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetArchiveExportResponseTypeDef](./type_defs.md#getarchiveexportresponsetypedef) 


```python
# get_archive_export method usage example with argument unpacking

kwargs: GetArchiveExportRequestRequestTypeDef = {  # (1)
    "ExportId": ...,
}

parent.get_archive_export(**kwargs)
```

1. See [:material-code-braces: GetArchiveExportRequestRequestTypeDef](./type_defs.md#getarchiveexportrequestrequesttypedef) 

### get\_archive\_message

Returns a pre-signed URL that provides temporary download access to the
specific email message stored in the archive.

Type annotations and code completion for `#!python session.create_client("mailmanager").get_archive_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/get_archive_message.html)

```python
# get_archive_message method definition

await def get_archive_message(
    self,
    *,
    ArchivedMessageId: str,
) -> GetArchiveMessageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetArchiveMessageResponseTypeDef](./type_defs.md#getarchivemessageresponsetypedef) 


```python
# get_archive_message method usage example with argument unpacking

kwargs: GetArchiveMessageRequestRequestTypeDef = {  # (1)
    "ArchivedMessageId": ...,
}

parent.get_archive_message(**kwargs)
```

1. See [:material-code-braces: GetArchiveMessageRequestRequestTypeDef](./type_defs.md#getarchivemessagerequestrequesttypedef) 

### get\_archive\_message\_content

Returns the textual content of a specific email message stored in the archive.

Type annotations and code completion for `#!python session.create_client("mailmanager").get_archive_message_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/get_archive_message_content.html)

```python
# get_archive_message_content method definition

await def get_archive_message_content(
    self,
    *,
    ArchivedMessageId: str,
) -> GetArchiveMessageContentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetArchiveMessageContentResponseTypeDef](./type_defs.md#getarchivemessagecontentresponsetypedef) 


```python
# get_archive_message_content method usage example with argument unpacking

kwargs: GetArchiveMessageContentRequestRequestTypeDef = {  # (1)
    "ArchivedMessageId": ...,
}

parent.get_archive_message_content(**kwargs)
```

1. See [:material-code-braces: GetArchiveMessageContentRequestRequestTypeDef](./type_defs.md#getarchivemessagecontentrequestrequesttypedef) 

### get\_archive\_search

Retrieves the details and current status of a specific email archive search job.

Type annotations and code completion for `#!python session.create_client("mailmanager").get_archive_search` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/get_archive_search.html)

```python
# get_archive_search method definition

await def get_archive_search(
    self,
    *,
    SearchId: str,
) -> GetArchiveSearchResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetArchiveSearchResponseTypeDef](./type_defs.md#getarchivesearchresponsetypedef) 


```python
# get_archive_search method usage example with argument unpacking

kwargs: GetArchiveSearchRequestRequestTypeDef = {  # (1)
    "SearchId": ...,
}

parent.get_archive_search(**kwargs)
```

1. See [:material-code-braces: GetArchiveSearchRequestRequestTypeDef](./type_defs.md#getarchivesearchrequestrequesttypedef) 

### get\_archive\_search\_results

Returns the results of a completed email archive search job.

Type annotations and code completion for `#!python session.create_client("mailmanager").get_archive_search_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/get_archive_search_results.html)

```python
# get_archive_search_results method definition

await def get_archive_search_results(
    self,
    *,
    SearchId: str,
) -> GetArchiveSearchResultsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetArchiveSearchResultsResponseTypeDef](./type_defs.md#getarchivesearchresultsresponsetypedef) 


```python
# get_archive_search_results method usage example with argument unpacking

kwargs: GetArchiveSearchResultsRequestRequestTypeDef = {  # (1)
    "SearchId": ...,
}

parent.get_archive_search_results(**kwargs)
```

1. See [:material-code-braces: GetArchiveSearchResultsRequestRequestTypeDef](./type_defs.md#getarchivesearchresultsrequestrequesttypedef) 

### get\_ingress\_point

Fetch ingress endpoint resource attributes.

Type annotations and code completion for `#!python session.create_client("mailmanager").get_ingress_point` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/get_ingress_point.html)

```python
# get_ingress_point method definition

await def get_ingress_point(
    self,
    *,
    IngressPointId: str,
) -> GetIngressPointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIngressPointResponseTypeDef](./type_defs.md#getingresspointresponsetypedef) 


```python
# get_ingress_point method usage example with argument unpacking

kwargs: GetIngressPointRequestRequestTypeDef = {  # (1)
    "IngressPointId": ...,
}

parent.get_ingress_point(**kwargs)
```

1. See [:material-code-braces: GetIngressPointRequestRequestTypeDef](./type_defs.md#getingresspointrequestrequesttypedef) 

### get\_relay

Fetch the relay resource and it's attributes.

Type annotations and code completion for `#!python session.create_client("mailmanager").get_relay` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/get_relay.html)

```python
# get_relay method definition

await def get_relay(
    self,
    *,
    RelayId: str,
) -> GetRelayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRelayResponseTypeDef](./type_defs.md#getrelayresponsetypedef) 


```python
# get_relay method usage example with argument unpacking

kwargs: GetRelayRequestRequestTypeDef = {  # (1)
    "RelayId": ...,
}

parent.get_relay(**kwargs)
```

1. See [:material-code-braces: GetRelayRequestRequestTypeDef](./type_defs.md#getrelayrequestrequesttypedef) 

### get\_rule\_set

Fetch attributes of a rule set.

Type annotations and code completion for `#!python session.create_client("mailmanager").get_rule_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/get_rule_set.html)

```python
# get_rule_set method definition

await def get_rule_set(
    self,
    *,
    RuleSetId: str,
) -> GetRuleSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRuleSetResponseTypeDef](./type_defs.md#getrulesetresponsetypedef) 


```python
# get_rule_set method usage example with argument unpacking

kwargs: GetRuleSetRequestRequestTypeDef = {  # (1)
    "RuleSetId": ...,
}

parent.get_rule_set(**kwargs)
```

1. See [:material-code-braces: GetRuleSetRequestRequestTypeDef](./type_defs.md#getrulesetrequestrequesttypedef) 

### get\_traffic\_policy

Fetch attributes of a traffic policy resource.

Type annotations and code completion for `#!python session.create_client("mailmanager").get_traffic_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/get_traffic_policy.html)

```python
# get_traffic_policy method definition

await def get_traffic_policy(
    self,
    *,
    TrafficPolicyId: str,
) -> GetTrafficPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTrafficPolicyResponseTypeDef](./type_defs.md#gettrafficpolicyresponsetypedef) 


```python
# get_traffic_policy method usage example with argument unpacking

kwargs: GetTrafficPolicyRequestRequestTypeDef = {  # (1)
    "TrafficPolicyId": ...,
}

parent.get_traffic_policy(**kwargs)
```

1. See [:material-code-braces: GetTrafficPolicyRequestRequestTypeDef](./type_defs.md#gettrafficpolicyrequestrequesttypedef) 

### list\_addon\_instances

Lists all Add On instances in your account.

Type annotations and code completion for `#!python session.create_client("mailmanager").list_addon_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/list_addon_instances.html)

```python
# list_addon_instances method definition

await def list_addon_instances(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListAddonInstancesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAddonInstancesResponseTypeDef](./type_defs.md#listaddoninstancesresponsetypedef) 


```python
# list_addon_instances method usage example with argument unpacking

kwargs: ListAddonInstancesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_addon_instances(**kwargs)
```

1. See [:material-code-braces: ListAddonInstancesRequestRequestTypeDef](./type_defs.md#listaddoninstancesrequestrequesttypedef) 

### list\_addon\_subscriptions

Lists all Add On subscriptions in your account.

Type annotations and code completion for `#!python session.create_client("mailmanager").list_addon_subscriptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/list_addon_subscriptions.html)

```python
# list_addon_subscriptions method definition

await def list_addon_subscriptions(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListAddonSubscriptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAddonSubscriptionsResponseTypeDef](./type_defs.md#listaddonsubscriptionsresponsetypedef) 


```python
# list_addon_subscriptions method usage example with argument unpacking

kwargs: ListAddonSubscriptionsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_addon_subscriptions(**kwargs)
```

1. See [:material-code-braces: ListAddonSubscriptionsRequestRequestTypeDef](./type_defs.md#listaddonsubscriptionsrequestrequesttypedef) 

### list\_archive\_exports

Returns a list of email archive export jobs.

Type annotations and code completion for `#!python session.create_client("mailmanager").list_archive_exports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/list_archive_exports.html)

```python
# list_archive_exports method definition

await def list_archive_exports(
    self,
    *,
    ArchiveId: str,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListArchiveExportsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListArchiveExportsResponseTypeDef](./type_defs.md#listarchiveexportsresponsetypedef) 


```python
# list_archive_exports method usage example with argument unpacking

kwargs: ListArchiveExportsRequestRequestTypeDef = {  # (1)
    "ArchiveId": ...,
}

parent.list_archive_exports(**kwargs)
```

1. See [:material-code-braces: ListArchiveExportsRequestRequestTypeDef](./type_defs.md#listarchiveexportsrequestrequesttypedef) 

### list\_archive\_searches

Returns a list of email archive search jobs.

Type annotations and code completion for `#!python session.create_client("mailmanager").list_archive_searches` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/list_archive_searches.html)

```python
# list_archive_searches method definition

await def list_archive_searches(
    self,
    *,
    ArchiveId: str,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListArchiveSearchesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListArchiveSearchesResponseTypeDef](./type_defs.md#listarchivesearchesresponsetypedef) 


```python
# list_archive_searches method usage example with argument unpacking

kwargs: ListArchiveSearchesRequestRequestTypeDef = {  # (1)
    "ArchiveId": ...,
}

parent.list_archive_searches(**kwargs)
```

1. See [:material-code-braces: ListArchiveSearchesRequestRequestTypeDef](./type_defs.md#listarchivesearchesrequestrequesttypedef) 

### list\_archives

Returns a list of all email archives in your account.

Type annotations and code completion for `#!python session.create_client("mailmanager").list_archives` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/list_archives.html)

```python
# list_archives method definition

await def list_archives(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListArchivesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListArchivesResponseTypeDef](./type_defs.md#listarchivesresponsetypedef) 


```python
# list_archives method usage example with argument unpacking

kwargs: ListArchivesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_archives(**kwargs)
```

1. See [:material-code-braces: ListArchivesRequestRequestTypeDef](./type_defs.md#listarchivesrequestrequesttypedef) 

### list\_ingress\_points

List all ingress endpoint resources.

Type annotations and code completion for `#!python session.create_client("mailmanager").list_ingress_points` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/list_ingress_points.html)

```python
# list_ingress_points method definition

await def list_ingress_points(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListIngressPointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIngressPointsResponseTypeDef](./type_defs.md#listingresspointsresponsetypedef) 


```python
# list_ingress_points method usage example with argument unpacking

kwargs: ListIngressPointsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_ingress_points(**kwargs)
```

1. See [:material-code-braces: ListIngressPointsRequestRequestTypeDef](./type_defs.md#listingresspointsrequestrequesttypedef) 

### list\_relays

Lists all the existing relay resources.

Type annotations and code completion for `#!python session.create_client("mailmanager").list_relays` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/list_relays.html)

```python
# list_relays method definition

await def list_relays(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListRelaysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRelaysResponseTypeDef](./type_defs.md#listrelaysresponsetypedef) 


```python
# list_relays method usage example with argument unpacking

kwargs: ListRelaysRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_relays(**kwargs)
```

1. See [:material-code-braces: ListRelaysRequestRequestTypeDef](./type_defs.md#listrelaysrequestrequesttypedef) 

### list\_rule\_sets

List rule sets for this account.

Type annotations and code completion for `#!python session.create_client("mailmanager").list_rule_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/list_rule_sets.html)

```python
# list_rule_sets method definition

await def list_rule_sets(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListRuleSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRuleSetsResponseTypeDef](./type_defs.md#listrulesetsresponsetypedef) 


```python
# list_rule_sets method usage example with argument unpacking

kwargs: ListRuleSetsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_rule_sets(**kwargs)
```

1. See [:material-code-braces: ListRuleSetsRequestRequestTypeDef](./type_defs.md#listrulesetsrequestrequesttypedef) 

### list\_tags\_for\_resource

Retrieves the list of tags (keys and values) assigned to the resource.

Type annotations and code completion for `#!python session.create_client("mailmanager").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/list_tags_for_resource.html)

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

### list\_traffic\_policies

List traffic policy resources.

Type annotations and code completion for `#!python session.create_client("mailmanager").list_traffic_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/list_traffic_policies.html)

```python
# list_traffic_policies method definition

await def list_traffic_policies(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListTrafficPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTrafficPoliciesResponseTypeDef](./type_defs.md#listtrafficpoliciesresponsetypedef) 


```python
# list_traffic_policies method usage example with argument unpacking

kwargs: ListTrafficPoliciesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_traffic_policies(**kwargs)
```

1. See [:material-code-braces: ListTrafficPoliciesRequestRequestTypeDef](./type_defs.md#listtrafficpoliciesrequestrequesttypedef) 

### start\_archive\_export

Initiates an export of emails from the specified archive.

Type annotations and code completion for `#!python session.create_client("mailmanager").start_archive_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/start_archive_export.html)

```python
# start_archive_export method definition

await def start_archive_export(
    self,
    *,
    ArchiveId: str,
    ExportDestinationConfiguration: ExportDestinationConfigurationTypeDef,  # (1)
    FromTimestamp: TimestampTypeDef,
    ToTimestamp: TimestampTypeDef,
    Filters: ArchiveFiltersTypeDef = ...,  # (2)
    IncludeMetadata: bool = ...,
    MaxResults: int = ...,
) -> StartArchiveExportResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ExportDestinationConfigurationTypeDef](./type_defs.md#exportdestinationconfigurationtypedef) 
2. See [:material-code-braces: ArchiveFiltersTypeDef](./type_defs.md#archivefilterstypedef) 
3. See [:material-code-braces: StartArchiveExportResponseTypeDef](./type_defs.md#startarchiveexportresponsetypedef) 


```python
# start_archive_export method usage example with argument unpacking

kwargs: StartArchiveExportRequestRequestTypeDef = {  # (1)
    "ArchiveId": ...,
    "ExportDestinationConfiguration": ...,
    "FromTimestamp": ...,
    "ToTimestamp": ...,
}

parent.start_archive_export(**kwargs)
```

1. See [:material-code-braces: StartArchiveExportRequestRequestTypeDef](./type_defs.md#startarchiveexportrequestrequesttypedef) 

### start\_archive\_search

Initiates a search across emails in the specified archive.

Type annotations and code completion for `#!python session.create_client("mailmanager").start_archive_search` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/start_archive_search.html)

```python
# start_archive_search method definition

await def start_archive_search(
    self,
    *,
    ArchiveId: str,
    FromTimestamp: TimestampTypeDef,
    MaxResults: int,
    ToTimestamp: TimestampTypeDef,
    Filters: ArchiveFiltersTypeDef = ...,  # (1)
) -> StartArchiveSearchResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ArchiveFiltersTypeDef](./type_defs.md#archivefilterstypedef) 
2. See [:material-code-braces: StartArchiveSearchResponseTypeDef](./type_defs.md#startarchivesearchresponsetypedef) 


```python
# start_archive_search method usage example with argument unpacking

kwargs: StartArchiveSearchRequestRequestTypeDef = {  # (1)
    "ArchiveId": ...,
    "FromTimestamp": ...,
    "MaxResults": ...,
    "ToTimestamp": ...,
}

parent.start_archive_search(**kwargs)
```

1. See [:material-code-braces: StartArchiveSearchRequestRequestTypeDef](./type_defs.md#startarchivesearchrequestrequesttypedef) 

### stop\_archive\_export

Stops an in-progress export of emails from an archive.

Type annotations and code completion for `#!python session.create_client("mailmanager").stop_archive_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/stop_archive_export.html)

```python
# stop_archive_export method definition

await def stop_archive_export(
    self,
    *,
    ExportId: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_archive_export method usage example with argument unpacking

kwargs: StopArchiveExportRequestRequestTypeDef = {  # (1)
    "ExportId": ...,
}

parent.stop_archive_export(**kwargs)
```

1. See [:material-code-braces: StopArchiveExportRequestRequestTypeDef](./type_defs.md#stoparchiveexportrequestrequesttypedef) 

### stop\_archive\_search

Stops an in-progress archive search job.

Type annotations and code completion for `#!python session.create_client("mailmanager").stop_archive_search` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/stop_archive_search.html)

```python
# stop_archive_search method definition

await def stop_archive_search(
    self,
    *,
    SearchId: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_archive_search method usage example with argument unpacking

kwargs: StopArchiveSearchRequestRequestTypeDef = {  # (1)
    "SearchId": ...,
}

parent.stop_archive_search(**kwargs)
```

1. See [:material-code-braces: StopArchiveSearchRequestRequestTypeDef](./type_defs.md#stoparchivesearchrequestrequesttypedef) 

### tag\_resource

Adds one or more tags (keys and values) to a specified resource.

Type annotations and code completion for `#!python session.create_client("mailmanager").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/tag_resource.html)

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

Remove one or more tags (keys and values) from a specified resource.

Type annotations and code completion for `#!python session.create_client("mailmanager").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/untag_resource.html)

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

### update\_archive

Updates the attributes of an existing email archive.

Type annotations and code completion for `#!python session.create_client("mailmanager").update_archive` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/update_archive.html)

```python
# update_archive method definition

await def update_archive(
    self,
    *,
    ArchiveId: str,
    ArchiveName: str = ...,
    Retention: ArchiveRetentionTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ArchiveRetentionTypeDef](./type_defs.md#archiveretentiontypedef) 


```python
# update_archive method usage example with argument unpacking

kwargs: UpdateArchiveRequestRequestTypeDef = {  # (1)
    "ArchiveId": ...,
}

parent.update_archive(**kwargs)
```

1. See [:material-code-braces: UpdateArchiveRequestRequestTypeDef](./type_defs.md#updatearchiverequestrequesttypedef) 

### update\_ingress\_point

Update attributes of a provisioned ingress endpoint resource.

Type annotations and code completion for `#!python session.create_client("mailmanager").update_ingress_point` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/update_ingress_point.html)

```python
# update_ingress_point method definition

await def update_ingress_point(
    self,
    *,
    IngressPointId: str,
    IngressPointConfiguration: IngressPointConfigurationTypeDef = ...,  # (1)
    IngressPointName: str = ...,
    RuleSetId: str = ...,
    StatusToUpdate: IngressPointStatusToUpdateType = ...,  # (2)
    TrafficPolicyId: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: IngressPointConfigurationTypeDef](./type_defs.md#ingresspointconfigurationtypedef) 
2. See [:material-code-brackets: IngressPointStatusToUpdateType](./literals.md#ingresspointstatustoupdatetype) 


```python
# update_ingress_point method usage example with argument unpacking

kwargs: UpdateIngressPointRequestRequestTypeDef = {  # (1)
    "IngressPointId": ...,
}

parent.update_ingress_point(**kwargs)
```

1. See [:material-code-braces: UpdateIngressPointRequestRequestTypeDef](./type_defs.md#updateingresspointrequestrequesttypedef) 

### update\_relay

Updates the attributes of an existing relay resource.

Type annotations and code completion for `#!python session.create_client("mailmanager").update_relay` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/update_relay.html)

```python
# update_relay method definition

await def update_relay(
    self,
    *,
    RelayId: str,
    Authentication: RelayAuthenticationTypeDef = ...,  # (1)
    RelayName: str = ...,
    ServerName: str = ...,
    ServerPort: int = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: RelayAuthenticationTypeDef](./type_defs.md#relayauthenticationtypedef) 


```python
# update_relay method usage example with argument unpacking

kwargs: UpdateRelayRequestRequestTypeDef = {  # (1)
    "RelayId": ...,
}

parent.update_relay(**kwargs)
```

1. See [:material-code-braces: UpdateRelayRequestRequestTypeDef](./type_defs.md#updaterelayrequestrequesttypedef) 

### update\_rule\_set

Update attributes of an already provisioned rule set.

Type annotations and code completion for `#!python session.create_client("mailmanager").update_rule_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/update_rule_set.html)

```python
# update_rule_set method definition

await def update_rule_set(
    self,
    *,
    RuleSetId: str,
    RuleSetName: str = ...,
    Rules: Sequence[RuleTypeDef] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 


```python
# update_rule_set method usage example with argument unpacking

kwargs: UpdateRuleSetRequestRequestTypeDef = {  # (1)
    "RuleSetId": ...,
}

parent.update_rule_set(**kwargs)
```

1. See [:material-code-braces: UpdateRuleSetRequestRequestTypeDef](./type_defs.md#updaterulesetrequestrequesttypedef) 

### update\_traffic\_policy

Update attributes of an already provisioned traffic policy resource.

Type annotations and code completion for `#!python session.create_client("mailmanager").update_traffic_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager/client/update_traffic_policy.html)

```python
# update_traffic_policy method definition

await def update_traffic_policy(
    self,
    *,
    TrafficPolicyId: str,
    DefaultAction: AcceptActionType = ...,  # (1)
    MaxMessageSizeBytes: int = ...,
    PolicyStatements: Sequence[PolicyStatementTypeDef] = ...,  # (2)
    TrafficPolicyName: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: AcceptActionType](./literals.md#acceptactiontype) 
2. See [:material-code-braces: PolicyStatementTypeDef](./type_defs.md#policystatementtypedef) 


```python
# update_traffic_policy method usage example with argument unpacking

kwargs: UpdateTrafficPolicyRequestRequestTypeDef = {  # (1)
    "TrafficPolicyId": ...,
}

parent.update_traffic_policy(**kwargs)
```

1. See [:material-code-braces: UpdateTrafficPolicyRequestRequestTypeDef](./type_defs.md#updatetrafficpolicyrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("mailmanager").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager.html#MailManager.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "MailManagerClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("mailmanager").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager.html#MailManager.Client)

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

Type annotations and code completion for `#!python session.create_client("mailmanager").get_paginator` method with overloads.

- `client.get_paginator("list_addon_instances")` -> [ListAddonInstancesPaginator](./paginators.md#listaddoninstancespaginator)
- `client.get_paginator("list_addon_subscriptions")` -> [ListAddonSubscriptionsPaginator](./paginators.md#listaddonsubscriptionspaginator)
- `client.get_paginator("list_archive_exports")` -> [ListArchiveExportsPaginator](./paginators.md#listarchiveexportspaginator)
- `client.get_paginator("list_archive_searches")` -> [ListArchiveSearchesPaginator](./paginators.md#listarchivesearchespaginator)
- `client.get_paginator("list_archives")` -> [ListArchivesPaginator](./paginators.md#listarchivespaginator)
- `client.get_paginator("list_ingress_points")` -> [ListIngressPointsPaginator](./paginators.md#listingresspointspaginator)
- `client.get_paginator("list_relays")` -> [ListRelaysPaginator](./paginators.md#listrelayspaginator)
- `client.get_paginator("list_rule_sets")` -> [ListRuleSetsPaginator](./paginators.md#listrulesetspaginator)
- `client.get_paginator("list_traffic_policies")` -> [ListTrafficPoliciesPaginator](./paginators.md#listtrafficpoliciespaginator)



