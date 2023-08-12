# WorkSpacesWebClient

> [Index](../README.md) > [WorkSpacesWeb](./README.md) > WorkSpacesWebClient

!!! note ""

    Auto-generated documentation for [WorkSpacesWeb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
    type annotations stubs module [types-aiobotocore-workspaces-web](https://pypi.org/project/types-aiobotocore-workspaces-web/).

## WorkSpacesWebClient

Type annotations and code completion for `#!python session.create_client("workspaces-web")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client)

```python
WorkSpacesWebClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_workspaces_web.client import WorkSpacesWebClient

session = get_session()
async with session.create_client("workspaces-web") as client:
    client: WorkSpacesWebClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("workspaces-web").exceptions` structure.

```python
WorkSpacesWebClient.exceptions usage example

async with session.create_client("workspaces-web") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.TooManyTagsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
WorkSpacesWebClient usage type checking example

from types_aiobotocore_workspaces_web.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_browser\_settings

Associates a browser settings resource with a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").associate_browser_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_browser_settings)

```python
# associate_browser_settings method definition

await def associate_browser_settings(
    self,
    *,
    browserSettingsArn: str,
    portalArn: str,
) -> AssociateBrowserSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateBrowserSettingsResponseTypeDef](./type_defs.md#associatebrowsersettingsresponsetypedef) 


```python
# associate_browser_settings method usage example with argument unpacking

kwargs: AssociateBrowserSettingsRequestRequestTypeDef = {  # (1)
    "browserSettingsArn": ...,
    "portalArn": ...,
}

parent.associate_browser_settings(**kwargs)
```

1. See [:material-code-braces: AssociateBrowserSettingsRequestRequestTypeDef](./type_defs.md#associatebrowsersettingsrequestrequesttypedef) 

### associate\_ip\_access\_settings

Associates an IP access settings resource with a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").associate_ip_access_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_ip_access_settings)

```python
# associate_ip_access_settings method definition

await def associate_ip_access_settings(
    self,
    *,
    ipAccessSettingsArn: str,
    portalArn: str,
) -> AssociateIpAccessSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateIpAccessSettingsResponseTypeDef](./type_defs.md#associateipaccesssettingsresponsetypedef) 


```python
# associate_ip_access_settings method usage example with argument unpacking

kwargs: AssociateIpAccessSettingsRequestRequestTypeDef = {  # (1)
    "ipAccessSettingsArn": ...,
    "portalArn": ...,
}

parent.associate_ip_access_settings(**kwargs)
```

1. See [:material-code-braces: AssociateIpAccessSettingsRequestRequestTypeDef](./type_defs.md#associateipaccesssettingsrequestrequesttypedef) 

### associate\_network\_settings

Associates a network settings resource with a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").associate_network_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_network_settings)

```python
# associate_network_settings method definition

await def associate_network_settings(
    self,
    *,
    networkSettingsArn: str,
    portalArn: str,
) -> AssociateNetworkSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateNetworkSettingsResponseTypeDef](./type_defs.md#associatenetworksettingsresponsetypedef) 


```python
# associate_network_settings method usage example with argument unpacking

kwargs: AssociateNetworkSettingsRequestRequestTypeDef = {  # (1)
    "networkSettingsArn": ...,
    "portalArn": ...,
}

parent.associate_network_settings(**kwargs)
```

1. See [:material-code-braces: AssociateNetworkSettingsRequestRequestTypeDef](./type_defs.md#associatenetworksettingsrequestrequesttypedef) 

### associate\_trust\_store

Associates a trust store with a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").associate_trust_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_trust_store)

```python
# associate_trust_store method definition

await def associate_trust_store(
    self,
    *,
    portalArn: str,
    trustStoreArn: str,
) -> AssociateTrustStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateTrustStoreResponseTypeDef](./type_defs.md#associatetruststoreresponsetypedef) 


```python
# associate_trust_store method usage example with argument unpacking

kwargs: AssociateTrustStoreRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
    "trustStoreArn": ...,
}

parent.associate_trust_store(**kwargs)
```

1. See [:material-code-braces: AssociateTrustStoreRequestRequestTypeDef](./type_defs.md#associatetruststorerequestrequesttypedef) 

### associate\_user\_access\_logging\_settings

Associates a user access logging settings resource with a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").associate_user_access_logging_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_user_access_logging_settings)

```python
# associate_user_access_logging_settings method definition

await def associate_user_access_logging_settings(
    self,
    *,
    portalArn: str,
    userAccessLoggingSettingsArn: str,
) -> AssociateUserAccessLoggingSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateUserAccessLoggingSettingsResponseTypeDef](./type_defs.md#associateuseraccessloggingsettingsresponsetypedef) 


```python
# associate_user_access_logging_settings method usage example with argument unpacking

kwargs: AssociateUserAccessLoggingSettingsRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
    "userAccessLoggingSettingsArn": ...,
}

parent.associate_user_access_logging_settings(**kwargs)
```

1. See [:material-code-braces: AssociateUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#associateuseraccessloggingsettingsrequestrequesttypedef) 

### associate\_user\_settings

Associates a user settings resource with a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").associate_user_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_user_settings)

```python
# associate_user_settings method definition

await def associate_user_settings(
    self,
    *,
    portalArn: str,
    userSettingsArn: str,
) -> AssociateUserSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateUserSettingsResponseTypeDef](./type_defs.md#associateusersettingsresponsetypedef) 


```python
# associate_user_settings method usage example with argument unpacking

kwargs: AssociateUserSettingsRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
    "userSettingsArn": ...,
}

parent.associate_user_settings(**kwargs)
```

1. See [:material-code-braces: AssociateUserSettingsRequestRequestTypeDef](./type_defs.md#associateusersettingsrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("workspaces-web").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("workspaces-web").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_browser\_settings

Creates a browser settings resource that can be associated with a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").create_browser_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_browser_settings)

```python
# create_browser_settings method definition

await def create_browser_settings(
    self,
    *,
    browserPolicy: str,
    additionalEncryptionContext: Mapping[str, str] = ...,
    clientToken: str = ...,
    customerManagedKey: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateBrowserSettingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateBrowserSettingsResponseTypeDef](./type_defs.md#createbrowsersettingsresponsetypedef) 


```python
# create_browser_settings method usage example with argument unpacking

kwargs: CreateBrowserSettingsRequestRequestTypeDef = {  # (1)
    "browserPolicy": ...,
}

parent.create_browser_settings(**kwargs)
```

1. See [:material-code-braces: CreateBrowserSettingsRequestRequestTypeDef](./type_defs.md#createbrowsersettingsrequestrequesttypedef) 

### create\_identity\_provider

Creates an identity provider resource that is then associated with a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").create_identity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_identity_provider)

```python
# create_identity_provider method definition

await def create_identity_provider(
    self,
    *,
    identityProviderDetails: Mapping[str, str],
    identityProviderName: str,
    identityProviderType: IdentityProviderTypeType,  # (1)
    portalArn: str,
    clientToken: str = ...,
) -> CreateIdentityProviderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: IdentityProviderTypeType](./literals.md#identityprovidertypetype) 
2. See [:material-code-braces: CreateIdentityProviderResponseTypeDef](./type_defs.md#createidentityproviderresponsetypedef) 


```python
# create_identity_provider method usage example with argument unpacking

kwargs: CreateIdentityProviderRequestRequestTypeDef = {  # (1)
    "identityProviderDetails": ...,
    "identityProviderName": ...,
    "identityProviderType": ...,
    "portalArn": ...,
}

parent.create_identity_provider(**kwargs)
```

1. See [:material-code-braces: CreateIdentityProviderRequestRequestTypeDef](./type_defs.md#createidentityproviderrequestrequesttypedef) 

### create\_ip\_access\_settings

Creates an IP access settings resource that can be associated with a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").create_ip_access_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_ip_access_settings)

```python
# create_ip_access_settings method definition

await def create_ip_access_settings(
    self,
    *,
    ipRules: Sequence[IpRuleTypeDef],  # (1)
    additionalEncryptionContext: Mapping[str, str] = ...,
    clientToken: str = ...,
    customerManagedKey: str = ...,
    description: str = ...,
    displayName: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateIpAccessSettingsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IpRuleTypeDef](./type_defs.md#ipruletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateIpAccessSettingsResponseTypeDef](./type_defs.md#createipaccesssettingsresponsetypedef) 


```python
# create_ip_access_settings method usage example with argument unpacking

kwargs: CreateIpAccessSettingsRequestRequestTypeDef = {  # (1)
    "ipRules": ...,
}

parent.create_ip_access_settings(**kwargs)
```

1. See [:material-code-braces: CreateIpAccessSettingsRequestRequestTypeDef](./type_defs.md#createipaccesssettingsrequestrequesttypedef) 

### create\_network\_settings

Creates a network settings resource that can be associated with a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").create_network_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_network_settings)

```python
# create_network_settings method definition

await def create_network_settings(
    self,
    *,
    securityGroupIds: Sequence[str],
    subnetIds: Sequence[str],
    vpcId: str,
    clientToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateNetworkSettingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateNetworkSettingsResponseTypeDef](./type_defs.md#createnetworksettingsresponsetypedef) 


```python
# create_network_settings method usage example with argument unpacking

kwargs: CreateNetworkSettingsRequestRequestTypeDef = {  # (1)
    "securityGroupIds": ...,
    "subnetIds": ...,
    "vpcId": ...,
}

parent.create_network_settings(**kwargs)
```

1. See [:material-code-braces: CreateNetworkSettingsRequestRequestTypeDef](./type_defs.md#createnetworksettingsrequestrequesttypedef) 

### create\_portal

Creates a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").create_portal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_portal)

```python
# create_portal method definition

await def create_portal(
    self,
    *,
    additionalEncryptionContext: Mapping[str, str] = ...,
    authenticationType: AuthenticationTypeType = ...,  # (1)
    clientToken: str = ...,
    customerManagedKey: str = ...,
    displayName: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreatePortalResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreatePortalResponseTypeDef](./type_defs.md#createportalresponsetypedef) 


```python
# create_portal method usage example with argument unpacking

kwargs: CreatePortalRequestRequestTypeDef = {  # (1)
    "additionalEncryptionContext": ...,
}

parent.create_portal(**kwargs)
```

1. See [:material-code-braces: CreatePortalRequestRequestTypeDef](./type_defs.md#createportalrequestrequesttypedef) 

### create\_trust\_store

Creates a trust store that can be associated with a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").create_trust_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_trust_store)

```python
# create_trust_store method definition

await def create_trust_store(
    self,
    *,
    certificateList: Sequence[Union[str, bytes, IO[Any], StreamingBody]],
    clientToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateTrustStoreResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateTrustStoreResponseTypeDef](./type_defs.md#createtruststoreresponsetypedef) 


```python
# create_trust_store method usage example with argument unpacking

kwargs: CreateTrustStoreRequestRequestTypeDef = {  # (1)
    "certificateList": ...,
}

parent.create_trust_store(**kwargs)
```

1. See [:material-code-braces: CreateTrustStoreRequestRequestTypeDef](./type_defs.md#createtruststorerequestrequesttypedef) 

### create\_user\_access\_logging\_settings

Creates a user access logging settings resource that can be associated with a
web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").create_user_access_logging_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_user_access_logging_settings)

```python
# create_user_access_logging_settings method definition

await def create_user_access_logging_settings(
    self,
    *,
    kinesisStreamArn: str,
    clientToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateUserAccessLoggingSettingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateUserAccessLoggingSettingsResponseTypeDef](./type_defs.md#createuseraccessloggingsettingsresponsetypedef) 


```python
# create_user_access_logging_settings method usage example with argument unpacking

kwargs: CreateUserAccessLoggingSettingsRequestRequestTypeDef = {  # (1)
    "kinesisStreamArn": ...,
}

parent.create_user_access_logging_settings(**kwargs)
```

1. See [:material-code-braces: CreateUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#createuseraccessloggingsettingsrequestrequesttypedef) 

### create\_user\_settings

Creates a user settings resource that can be associated with a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").create_user_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_user_settings)

```python
# create_user_settings method definition

await def create_user_settings(
    self,
    *,
    copyAllowed: EnabledTypeType,  # (1)
    downloadAllowed: EnabledTypeType,  # (1)
    pasteAllowed: EnabledTypeType,  # (1)
    printAllowed: EnabledTypeType,  # (1)
    uploadAllowed: EnabledTypeType,  # (1)
    clientToken: str = ...,
    disconnectTimeoutInMinutes: int = ...,
    idleDisconnectTimeoutInMinutes: int = ...,
    tags: Sequence[TagTypeDef] = ...,  # (6)
) -> CreateUserSettingsResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
2. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
3. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
4. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
5. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: CreateUserSettingsResponseTypeDef](./type_defs.md#createusersettingsresponsetypedef) 


```python
# create_user_settings method usage example with argument unpacking

kwargs: CreateUserSettingsRequestRequestTypeDef = {  # (1)
    "copyAllowed": ...,
    "downloadAllowed": ...,
    "pasteAllowed": ...,
    "printAllowed": ...,
    "uploadAllowed": ...,
}

parent.create_user_settings(**kwargs)
```

1. See [:material-code-braces: CreateUserSettingsRequestRequestTypeDef](./type_defs.md#createusersettingsrequestrequesttypedef) 

### delete\_browser\_settings

Deletes browser settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").delete_browser_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_browser_settings)

```python
# delete_browser_settings method definition

await def delete_browser_settings(
    self,
    *,
    browserSettingsArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_browser_settings method usage example with argument unpacking

kwargs: DeleteBrowserSettingsRequestRequestTypeDef = {  # (1)
    "browserSettingsArn": ...,
}

parent.delete_browser_settings(**kwargs)
```

1. See [:material-code-braces: DeleteBrowserSettingsRequestRequestTypeDef](./type_defs.md#deletebrowsersettingsrequestrequesttypedef) 

### delete\_identity\_provider

Deletes the identity provider.

Type annotations and code completion for `#!python session.create_client("workspaces-web").delete_identity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_identity_provider)

```python
# delete_identity_provider method definition

await def delete_identity_provider(
    self,
    *,
    identityProviderArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_identity_provider method usage example with argument unpacking

kwargs: DeleteIdentityProviderRequestRequestTypeDef = {  # (1)
    "identityProviderArn": ...,
}

parent.delete_identity_provider(**kwargs)
```

1. See [:material-code-braces: DeleteIdentityProviderRequestRequestTypeDef](./type_defs.md#deleteidentityproviderrequestrequesttypedef) 

### delete\_ip\_access\_settings

Deletes IP access settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").delete_ip_access_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_ip_access_settings)

```python
# delete_ip_access_settings method definition

await def delete_ip_access_settings(
    self,
    *,
    ipAccessSettingsArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ip_access_settings method usage example with argument unpacking

kwargs: DeleteIpAccessSettingsRequestRequestTypeDef = {  # (1)
    "ipAccessSettingsArn": ...,
}

parent.delete_ip_access_settings(**kwargs)
```

1. See [:material-code-braces: DeleteIpAccessSettingsRequestRequestTypeDef](./type_defs.md#deleteipaccesssettingsrequestrequesttypedef) 

### delete\_network\_settings

Deletes network settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").delete_network_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_network_settings)

```python
# delete_network_settings method definition

await def delete_network_settings(
    self,
    *,
    networkSettingsArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_network_settings method usage example with argument unpacking

kwargs: DeleteNetworkSettingsRequestRequestTypeDef = {  # (1)
    "networkSettingsArn": ...,
}

parent.delete_network_settings(**kwargs)
```

1. See [:material-code-braces: DeleteNetworkSettingsRequestRequestTypeDef](./type_defs.md#deletenetworksettingsrequestrequesttypedef) 

### delete\_portal

Deletes a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").delete_portal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_portal)

```python
# delete_portal method definition

await def delete_portal(
    self,
    *,
    portalArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_portal method usage example with argument unpacking

kwargs: DeletePortalRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
}

parent.delete_portal(**kwargs)
```

1. See [:material-code-braces: DeletePortalRequestRequestTypeDef](./type_defs.md#deleteportalrequestrequesttypedef) 

### delete\_trust\_store

Deletes the trust store.

Type annotations and code completion for `#!python session.create_client("workspaces-web").delete_trust_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_trust_store)

```python
# delete_trust_store method definition

await def delete_trust_store(
    self,
    *,
    trustStoreArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_trust_store method usage example with argument unpacking

kwargs: DeleteTrustStoreRequestRequestTypeDef = {  # (1)
    "trustStoreArn": ...,
}

parent.delete_trust_store(**kwargs)
```

1. See [:material-code-braces: DeleteTrustStoreRequestRequestTypeDef](./type_defs.md#deletetruststorerequestrequesttypedef) 

### delete\_user\_access\_logging\_settings

Deletes user access logging settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").delete_user_access_logging_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_user_access_logging_settings)

```python
# delete_user_access_logging_settings method definition

await def delete_user_access_logging_settings(
    self,
    *,
    userAccessLoggingSettingsArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_user_access_logging_settings method usage example with argument unpacking

kwargs: DeleteUserAccessLoggingSettingsRequestRequestTypeDef = {  # (1)
    "userAccessLoggingSettingsArn": ...,
}

parent.delete_user_access_logging_settings(**kwargs)
```

1. See [:material-code-braces: DeleteUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#deleteuseraccessloggingsettingsrequestrequesttypedef) 

### delete\_user\_settings

Deletes user settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").delete_user_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_user_settings)

```python
# delete_user_settings method definition

await def delete_user_settings(
    self,
    *,
    userSettingsArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_user_settings method usage example with argument unpacking

kwargs: DeleteUserSettingsRequestRequestTypeDef = {  # (1)
    "userSettingsArn": ...,
}

parent.delete_user_settings(**kwargs)
```

1. See [:material-code-braces: DeleteUserSettingsRequestRequestTypeDef](./type_defs.md#deleteusersettingsrequestrequesttypedef) 

### disassociate\_browser\_settings

Disassociates browser settings from a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").disassociate_browser_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_browser_settings)

```python
# disassociate_browser_settings method definition

await def disassociate_browser_settings(
    self,
    *,
    portalArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_browser_settings method usage example with argument unpacking

kwargs: DisassociateBrowserSettingsRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
}

parent.disassociate_browser_settings(**kwargs)
```

1. See [:material-code-braces: DisassociateBrowserSettingsRequestRequestTypeDef](./type_defs.md#disassociatebrowsersettingsrequestrequesttypedef) 

### disassociate\_ip\_access\_settings

Disassociates IP access settings from a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").disassociate_ip_access_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_ip_access_settings)

```python
# disassociate_ip_access_settings method definition

await def disassociate_ip_access_settings(
    self,
    *,
    portalArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_ip_access_settings method usage example with argument unpacking

kwargs: DisassociateIpAccessSettingsRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
}

parent.disassociate_ip_access_settings(**kwargs)
```

1. See [:material-code-braces: DisassociateIpAccessSettingsRequestRequestTypeDef](./type_defs.md#disassociateipaccesssettingsrequestrequesttypedef) 

### disassociate\_network\_settings

Disassociates network settings from a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").disassociate_network_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_network_settings)

```python
# disassociate_network_settings method definition

await def disassociate_network_settings(
    self,
    *,
    portalArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_network_settings method usage example with argument unpacking

kwargs: DisassociateNetworkSettingsRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
}

parent.disassociate_network_settings(**kwargs)
```

1. See [:material-code-braces: DisassociateNetworkSettingsRequestRequestTypeDef](./type_defs.md#disassociatenetworksettingsrequestrequesttypedef) 

### disassociate\_trust\_store

Disassociates a trust store from a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").disassociate_trust_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_trust_store)

```python
# disassociate_trust_store method definition

await def disassociate_trust_store(
    self,
    *,
    portalArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_trust_store method usage example with argument unpacking

kwargs: DisassociateTrustStoreRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
}

parent.disassociate_trust_store(**kwargs)
```

1. See [:material-code-braces: DisassociateTrustStoreRequestRequestTypeDef](./type_defs.md#disassociatetruststorerequestrequesttypedef) 

### disassociate\_user\_access\_logging\_settings

Disassociates user access logging settings from a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").disassociate_user_access_logging_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_user_access_logging_settings)

```python
# disassociate_user_access_logging_settings method definition

await def disassociate_user_access_logging_settings(
    self,
    *,
    portalArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_user_access_logging_settings method usage example with argument unpacking

kwargs: DisassociateUserAccessLoggingSettingsRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
}

parent.disassociate_user_access_logging_settings(**kwargs)
```

1. See [:material-code-braces: DisassociateUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#disassociateuseraccessloggingsettingsrequestrequesttypedef) 

### disassociate\_user\_settings

Disassociates user settings from a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").disassociate_user_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_user_settings)

```python
# disassociate_user_settings method definition

await def disassociate_user_settings(
    self,
    *,
    portalArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_user_settings method usage example with argument unpacking

kwargs: DisassociateUserSettingsRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
}

parent.disassociate_user_settings(**kwargs)
```

1. See [:material-code-braces: DisassociateUserSettingsRequestRequestTypeDef](./type_defs.md#disassociateusersettingsrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("workspaces-web").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.generate_presigned_url)

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


### get\_browser\_settings

Gets browser settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").get_browser_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_browser_settings)

```python
# get_browser_settings method definition

await def get_browser_settings(
    self,
    *,
    browserSettingsArn: str,
) -> GetBrowserSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBrowserSettingsResponseTypeDef](./type_defs.md#getbrowsersettingsresponsetypedef) 


```python
# get_browser_settings method usage example with argument unpacking

kwargs: GetBrowserSettingsRequestRequestTypeDef = {  # (1)
    "browserSettingsArn": ...,
}

parent.get_browser_settings(**kwargs)
```

1. See [:material-code-braces: GetBrowserSettingsRequestRequestTypeDef](./type_defs.md#getbrowsersettingsrequestrequesttypedef) 

### get\_identity\_provider

Gets the identity provider.

Type annotations and code completion for `#!python session.create_client("workspaces-web").get_identity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_identity_provider)

```python
# get_identity_provider method definition

await def get_identity_provider(
    self,
    *,
    identityProviderArn: str,
) -> GetIdentityProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdentityProviderResponseTypeDef](./type_defs.md#getidentityproviderresponsetypedef) 


```python
# get_identity_provider method usage example with argument unpacking

kwargs: GetIdentityProviderRequestRequestTypeDef = {  # (1)
    "identityProviderArn": ...,
}

parent.get_identity_provider(**kwargs)
```

1. See [:material-code-braces: GetIdentityProviderRequestRequestTypeDef](./type_defs.md#getidentityproviderrequestrequesttypedef) 

### get\_ip\_access\_settings

Gets the IP access settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").get_ip_access_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_ip_access_settings)

```python
# get_ip_access_settings method definition

await def get_ip_access_settings(
    self,
    *,
    ipAccessSettingsArn: str,
) -> GetIpAccessSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIpAccessSettingsResponseTypeDef](./type_defs.md#getipaccesssettingsresponsetypedef) 


```python
# get_ip_access_settings method usage example with argument unpacking

kwargs: GetIpAccessSettingsRequestRequestTypeDef = {  # (1)
    "ipAccessSettingsArn": ...,
}

parent.get_ip_access_settings(**kwargs)
```

1. See [:material-code-braces: GetIpAccessSettingsRequestRequestTypeDef](./type_defs.md#getipaccesssettingsrequestrequesttypedef) 

### get\_network\_settings

Gets the network settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").get_network_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_network_settings)

```python
# get_network_settings method definition

await def get_network_settings(
    self,
    *,
    networkSettingsArn: str,
) -> GetNetworkSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetNetworkSettingsResponseTypeDef](./type_defs.md#getnetworksettingsresponsetypedef) 


```python
# get_network_settings method usage example with argument unpacking

kwargs: GetNetworkSettingsRequestRequestTypeDef = {  # (1)
    "networkSettingsArn": ...,
}

parent.get_network_settings(**kwargs)
```

1. See [:material-code-braces: GetNetworkSettingsRequestRequestTypeDef](./type_defs.md#getnetworksettingsrequestrequesttypedef) 

### get\_portal

Gets the web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").get_portal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_portal)

```python
# get_portal method definition

await def get_portal(
    self,
    *,
    portalArn: str,
) -> GetPortalResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPortalResponseTypeDef](./type_defs.md#getportalresponsetypedef) 


```python
# get_portal method usage example with argument unpacking

kwargs: GetPortalRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
}

parent.get_portal(**kwargs)
```

1. See [:material-code-braces: GetPortalRequestRequestTypeDef](./type_defs.md#getportalrequestrequesttypedef) 

### get\_portal\_service\_provider\_metadata

Gets the service provider metadata.

Type annotations and code completion for `#!python session.create_client("workspaces-web").get_portal_service_provider_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_portal_service_provider_metadata)

```python
# get_portal_service_provider_metadata method definition

await def get_portal_service_provider_metadata(
    self,
    *,
    portalArn: str,
) -> GetPortalServiceProviderMetadataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPortalServiceProviderMetadataResponseTypeDef](./type_defs.md#getportalserviceprovidermetadataresponsetypedef) 


```python
# get_portal_service_provider_metadata method usage example with argument unpacking

kwargs: GetPortalServiceProviderMetadataRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
}

parent.get_portal_service_provider_metadata(**kwargs)
```

1. See [:material-code-braces: GetPortalServiceProviderMetadataRequestRequestTypeDef](./type_defs.md#getportalserviceprovidermetadatarequestrequesttypedef) 

### get\_trust\_store

Gets the trust store.

Type annotations and code completion for `#!python session.create_client("workspaces-web").get_trust_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_trust_store)

```python
# get_trust_store method definition

await def get_trust_store(
    self,
    *,
    trustStoreArn: str,
) -> GetTrustStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTrustStoreResponseTypeDef](./type_defs.md#gettruststoreresponsetypedef) 


```python
# get_trust_store method usage example with argument unpacking

kwargs: GetTrustStoreRequestRequestTypeDef = {  # (1)
    "trustStoreArn": ...,
}

parent.get_trust_store(**kwargs)
```

1. See [:material-code-braces: GetTrustStoreRequestRequestTypeDef](./type_defs.md#gettruststorerequestrequesttypedef) 

### get\_trust\_store\_certificate

Gets the trust store certificate.

Type annotations and code completion for `#!python session.create_client("workspaces-web").get_trust_store_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_trust_store_certificate)

```python
# get_trust_store_certificate method definition

await def get_trust_store_certificate(
    self,
    *,
    thumbprint: str,
    trustStoreArn: str,
) -> GetTrustStoreCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTrustStoreCertificateResponseTypeDef](./type_defs.md#gettruststorecertificateresponsetypedef) 


```python
# get_trust_store_certificate method usage example with argument unpacking

kwargs: GetTrustStoreCertificateRequestRequestTypeDef = {  # (1)
    "thumbprint": ...,
    "trustStoreArn": ...,
}

parent.get_trust_store_certificate(**kwargs)
```

1. See [:material-code-braces: GetTrustStoreCertificateRequestRequestTypeDef](./type_defs.md#gettruststorecertificaterequestrequesttypedef) 

### get\_user\_access\_logging\_settings

Gets user access logging settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").get_user_access_logging_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_user_access_logging_settings)

```python
# get_user_access_logging_settings method definition

await def get_user_access_logging_settings(
    self,
    *,
    userAccessLoggingSettingsArn: str,
) -> GetUserAccessLoggingSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUserAccessLoggingSettingsResponseTypeDef](./type_defs.md#getuseraccessloggingsettingsresponsetypedef) 


```python
# get_user_access_logging_settings method usage example with argument unpacking

kwargs: GetUserAccessLoggingSettingsRequestRequestTypeDef = {  # (1)
    "userAccessLoggingSettingsArn": ...,
}

parent.get_user_access_logging_settings(**kwargs)
```

1. See [:material-code-braces: GetUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#getuseraccessloggingsettingsrequestrequesttypedef) 

### get\_user\_settings

Gets user settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").get_user_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_user_settings)

```python
# get_user_settings method definition

await def get_user_settings(
    self,
    *,
    userSettingsArn: str,
) -> GetUserSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUserSettingsResponseTypeDef](./type_defs.md#getusersettingsresponsetypedef) 


```python
# get_user_settings method usage example with argument unpacking

kwargs: GetUserSettingsRequestRequestTypeDef = {  # (1)
    "userSettingsArn": ...,
}

parent.get_user_settings(**kwargs)
```

1. See [:material-code-braces: GetUserSettingsRequestRequestTypeDef](./type_defs.md#getusersettingsrequestrequesttypedef) 

### list\_browser\_settings

Retrieves a list of browser settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").list_browser_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_browser_settings)

```python
# list_browser_settings method definition

await def list_browser_settings(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListBrowserSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBrowserSettingsResponseTypeDef](./type_defs.md#listbrowsersettingsresponsetypedef) 


```python
# list_browser_settings method usage example with argument unpacking

kwargs: ListBrowserSettingsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_browser_settings(**kwargs)
```

1. See [:material-code-braces: ListBrowserSettingsRequestRequestTypeDef](./type_defs.md#listbrowsersettingsrequestrequesttypedef) 

### list\_identity\_providers

Retrieves a list of identity providers for a specific web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").list_identity_providers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_identity_providers)

```python
# list_identity_providers method definition

await def list_identity_providers(
    self,
    *,
    portalArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListIdentityProvidersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef) 


```python
# list_identity_providers method usage example with argument unpacking

kwargs: ListIdentityProvidersRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
}

parent.list_identity_providers(**kwargs)
```

1. See [:material-code-braces: ListIdentityProvidersRequestRequestTypeDef](./type_defs.md#listidentityprovidersrequestrequesttypedef) 

### list\_ip\_access\_settings

Retrieves a list of IP access settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").list_ip_access_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_ip_access_settings)

```python
# list_ip_access_settings method definition

await def list_ip_access_settings(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListIpAccessSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIpAccessSettingsResponseTypeDef](./type_defs.md#listipaccesssettingsresponsetypedef) 


```python
# list_ip_access_settings method usage example with argument unpacking

kwargs: ListIpAccessSettingsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_ip_access_settings(**kwargs)
```

1. See [:material-code-braces: ListIpAccessSettingsRequestRequestTypeDef](./type_defs.md#listipaccesssettingsrequestrequesttypedef) 

### list\_network\_settings

Retrieves a list of network settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").list_network_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_network_settings)

```python
# list_network_settings method definition

await def list_network_settings(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListNetworkSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListNetworkSettingsResponseTypeDef](./type_defs.md#listnetworksettingsresponsetypedef) 


```python
# list_network_settings method usage example with argument unpacking

kwargs: ListNetworkSettingsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_network_settings(**kwargs)
```

1. See [:material-code-braces: ListNetworkSettingsRequestRequestTypeDef](./type_defs.md#listnetworksettingsrequestrequesttypedef) 

### list\_portals

Retrieves a list or web portals.

Type annotations and code completion for `#!python session.create_client("workspaces-web").list_portals` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_portals)

```python
# list_portals method definition

await def list_portals(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListPortalsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPortalsResponseTypeDef](./type_defs.md#listportalsresponsetypedef) 


```python
# list_portals method usage example with argument unpacking

kwargs: ListPortalsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_portals(**kwargs)
```

1. See [:material-code-braces: ListPortalsRequestRequestTypeDef](./type_defs.md#listportalsrequestrequesttypedef) 

### list\_tags\_for\_resource

Retrieves a list of tags for a resource.

Type annotations and code completion for `#!python session.create_client("workspaces-web").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_trust\_store\_certificates

Retrieves a list of trust store certificates.

Type annotations and code completion for `#!python session.create_client("workspaces-web").list_trust_store_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_trust_store_certificates)

```python
# list_trust_store_certificates method definition

await def list_trust_store_certificates(
    self,
    *,
    trustStoreArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTrustStoreCertificatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTrustStoreCertificatesResponseTypeDef](./type_defs.md#listtruststorecertificatesresponsetypedef) 


```python
# list_trust_store_certificates method usage example with argument unpacking

kwargs: ListTrustStoreCertificatesRequestRequestTypeDef = {  # (1)
    "trustStoreArn": ...,
}

parent.list_trust_store_certificates(**kwargs)
```

1. See [:material-code-braces: ListTrustStoreCertificatesRequestRequestTypeDef](./type_defs.md#listtruststorecertificatesrequestrequesttypedef) 

### list\_trust\_stores

Retrieves a list of trust stores.

Type annotations and code completion for `#!python session.create_client("workspaces-web").list_trust_stores` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_trust_stores)

```python
# list_trust_stores method definition

await def list_trust_stores(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTrustStoresResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTrustStoresResponseTypeDef](./type_defs.md#listtruststoresresponsetypedef) 


```python
# list_trust_stores method usage example with argument unpacking

kwargs: ListTrustStoresRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_trust_stores(**kwargs)
```

1. See [:material-code-braces: ListTrustStoresRequestRequestTypeDef](./type_defs.md#listtruststoresrequestrequesttypedef) 

### list\_user\_access\_logging\_settings

Retrieves a list of user access logging settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").list_user_access_logging_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_user_access_logging_settings)

```python
# list_user_access_logging_settings method definition

await def list_user_access_logging_settings(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListUserAccessLoggingSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUserAccessLoggingSettingsResponseTypeDef](./type_defs.md#listuseraccessloggingsettingsresponsetypedef) 


```python
# list_user_access_logging_settings method usage example with argument unpacking

kwargs: ListUserAccessLoggingSettingsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_user_access_logging_settings(**kwargs)
```

1. See [:material-code-braces: ListUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#listuseraccessloggingsettingsrequestrequesttypedef) 

### list\_user\_settings

Retrieves a list of user settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").list_user_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_user_settings)

```python
# list_user_settings method definition

await def list_user_settings(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListUserSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUserSettingsResponseTypeDef](./type_defs.md#listusersettingsresponsetypedef) 


```python
# list_user_settings method usage example with argument unpacking

kwargs: ListUserSettingsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_user_settings(**kwargs)
```

1. See [:material-code-braces: ListUserSettingsRequestRequestTypeDef](./type_defs.md#listusersettingsrequestrequesttypedef) 

### tag\_resource

Adds or overwrites one or more tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("workspaces-web").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes one or more tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("workspaces-web").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_browser\_settings

Updates browser settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").update_browser_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_browser_settings)

```python
# update_browser_settings method definition

await def update_browser_settings(
    self,
    *,
    browserSettingsArn: str,
    browserPolicy: str = ...,
    clientToken: str = ...,
) -> UpdateBrowserSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateBrowserSettingsResponseTypeDef](./type_defs.md#updatebrowsersettingsresponsetypedef) 


```python
# update_browser_settings method usage example with argument unpacking

kwargs: UpdateBrowserSettingsRequestRequestTypeDef = {  # (1)
    "browserSettingsArn": ...,
}

parent.update_browser_settings(**kwargs)
```

1. See [:material-code-braces: UpdateBrowserSettingsRequestRequestTypeDef](./type_defs.md#updatebrowsersettingsrequestrequesttypedef) 

### update\_identity\_provider

Updates the identity provider.

Type annotations and code completion for `#!python session.create_client("workspaces-web").update_identity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_identity_provider)

```python
# update_identity_provider method definition

await def update_identity_provider(
    self,
    *,
    identityProviderArn: str,
    clientToken: str = ...,
    identityProviderDetails: Mapping[str, str] = ...,
    identityProviderName: str = ...,
    identityProviderType: IdentityProviderTypeType = ...,  # (1)
) -> UpdateIdentityProviderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: IdentityProviderTypeType](./literals.md#identityprovidertypetype) 
2. See [:material-code-braces: UpdateIdentityProviderResponseTypeDef](./type_defs.md#updateidentityproviderresponsetypedef) 


```python
# update_identity_provider method usage example with argument unpacking

kwargs: UpdateIdentityProviderRequestRequestTypeDef = {  # (1)
    "identityProviderArn": ...,
}

parent.update_identity_provider(**kwargs)
```

1. See [:material-code-braces: UpdateIdentityProviderRequestRequestTypeDef](./type_defs.md#updateidentityproviderrequestrequesttypedef) 

### update\_ip\_access\_settings

Updates IP access settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").update_ip_access_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_ip_access_settings)

```python
# update_ip_access_settings method definition

await def update_ip_access_settings(
    self,
    *,
    ipAccessSettingsArn: str,
    clientToken: str = ...,
    description: str = ...,
    displayName: str = ...,
    ipRules: Sequence[IpRuleTypeDef] = ...,  # (1)
) -> UpdateIpAccessSettingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IpRuleTypeDef](./type_defs.md#ipruletypedef) 
2. See [:material-code-braces: UpdateIpAccessSettingsResponseTypeDef](./type_defs.md#updateipaccesssettingsresponsetypedef) 


```python
# update_ip_access_settings method usage example with argument unpacking

kwargs: UpdateIpAccessSettingsRequestRequestTypeDef = {  # (1)
    "ipAccessSettingsArn": ...,
}

parent.update_ip_access_settings(**kwargs)
```

1. See [:material-code-braces: UpdateIpAccessSettingsRequestRequestTypeDef](./type_defs.md#updateipaccesssettingsrequestrequesttypedef) 

### update\_network\_settings

Updates network settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").update_network_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_network_settings)

```python
# update_network_settings method definition

await def update_network_settings(
    self,
    *,
    networkSettingsArn: str,
    clientToken: str = ...,
    securityGroupIds: Sequence[str] = ...,
    subnetIds: Sequence[str] = ...,
    vpcId: str = ...,
) -> UpdateNetworkSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateNetworkSettingsResponseTypeDef](./type_defs.md#updatenetworksettingsresponsetypedef) 


```python
# update_network_settings method usage example with argument unpacking

kwargs: UpdateNetworkSettingsRequestRequestTypeDef = {  # (1)
    "networkSettingsArn": ...,
}

parent.update_network_settings(**kwargs)
```

1. See [:material-code-braces: UpdateNetworkSettingsRequestRequestTypeDef](./type_defs.md#updatenetworksettingsrequestrequesttypedef) 

### update\_portal

Updates a web portal.

Type annotations and code completion for `#!python session.create_client("workspaces-web").update_portal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_portal)

```python
# update_portal method definition

await def update_portal(
    self,
    *,
    portalArn: str,
    authenticationType: AuthenticationTypeType = ...,  # (1)
    displayName: str = ...,
) -> UpdatePortalResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: UpdatePortalResponseTypeDef](./type_defs.md#updateportalresponsetypedef) 


```python
# update_portal method usage example with argument unpacking

kwargs: UpdatePortalRequestRequestTypeDef = {  # (1)
    "portalArn": ...,
}

parent.update_portal(**kwargs)
```

1. See [:material-code-braces: UpdatePortalRequestRequestTypeDef](./type_defs.md#updateportalrequestrequesttypedef) 

### update\_trust\_store

Updates the trust store.

Type annotations and code completion for `#!python session.create_client("workspaces-web").update_trust_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_trust_store)

```python
# update_trust_store method definition

await def update_trust_store(
    self,
    *,
    trustStoreArn: str,
    certificatesToAdd: Sequence[Union[str, bytes, IO[Any], StreamingBody]] = ...,
    certificatesToDelete: Sequence[str] = ...,
    clientToken: str = ...,
) -> UpdateTrustStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateTrustStoreResponseTypeDef](./type_defs.md#updatetruststoreresponsetypedef) 


```python
# update_trust_store method usage example with argument unpacking

kwargs: UpdateTrustStoreRequestRequestTypeDef = {  # (1)
    "trustStoreArn": ...,
}

parent.update_trust_store(**kwargs)
```

1. See [:material-code-braces: UpdateTrustStoreRequestRequestTypeDef](./type_defs.md#updatetruststorerequestrequesttypedef) 

### update\_user\_access\_logging\_settings

Updates the user access logging settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").update_user_access_logging_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_user_access_logging_settings)

```python
# update_user_access_logging_settings method definition

await def update_user_access_logging_settings(
    self,
    *,
    userAccessLoggingSettingsArn: str,
    clientToken: str = ...,
    kinesisStreamArn: str = ...,
) -> UpdateUserAccessLoggingSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateUserAccessLoggingSettingsResponseTypeDef](./type_defs.md#updateuseraccessloggingsettingsresponsetypedef) 


```python
# update_user_access_logging_settings method usage example with argument unpacking

kwargs: UpdateUserAccessLoggingSettingsRequestRequestTypeDef = {  # (1)
    "userAccessLoggingSettingsArn": ...,
}

parent.update_user_access_logging_settings(**kwargs)
```

1. See [:material-code-braces: UpdateUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#updateuseraccessloggingsettingsrequestrequesttypedef) 

### update\_user\_settings

Updates the user settings.

Type annotations and code completion for `#!python session.create_client("workspaces-web").update_user_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_user_settings)

```python
# update_user_settings method definition

await def update_user_settings(
    self,
    *,
    userSettingsArn: str,
    clientToken: str = ...,
    copyAllowed: EnabledTypeType = ...,  # (1)
    disconnectTimeoutInMinutes: int = ...,
    downloadAllowed: EnabledTypeType = ...,  # (1)
    idleDisconnectTimeoutInMinutes: int = ...,
    pasteAllowed: EnabledTypeType = ...,  # (1)
    printAllowed: EnabledTypeType = ...,  # (1)
    uploadAllowed: EnabledTypeType = ...,  # (1)
) -> UpdateUserSettingsResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
2. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
3. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
4. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
5. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
6. See [:material-code-braces: UpdateUserSettingsResponseTypeDef](./type_defs.md#updateusersettingsresponsetypedef) 


```python
# update_user_settings method usage example with argument unpacking

kwargs: UpdateUserSettingsRequestRequestTypeDef = {  # (1)
    "userSettingsArn": ...,
}

parent.update_user_settings(**kwargs)
```

1. See [:material-code-braces: UpdateUserSettingsRequestRequestTypeDef](./type_defs.md#updateusersettingsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("workspaces-web").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> WorkSpacesWebClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("workspaces-web").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.__aexit__)

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





