<a id="workspaceswebclient-for-aiobotocore-workspacesweb-module"></a>

# WorkSpacesWebClient for aiobotocore WorkSpacesWeb module

> [Index](../README.md) > [WorkSpacesWeb](./README.md) > WorkSpacesWebClient

Auto-generated documentation for
[WorkSpacesWeb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
type annotations stubs module
[types-aiobotocore-workspaces-web](https://pypi.org/project/types-aiobotocore-workspaces-web/).

- [WorkSpacesWebClient for aiobotocore WorkSpacesWeb module](#workspaceswebclient-for-aiobotocore-workspacesweb-module)
  - [WorkSpacesWebClient](#workspaceswebclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [associate_browser_settings](#associate_browser_settings)
    - [associate_network_settings](#associate_network_settings)
    - [associate_trust_store](#associate_trust_store)
    - [associate_user_settings](#associate_user_settings)
    - [can_paginate](#can_paginate)
    - [create_browser_settings](#create_browser_settings)
    - [create_identity_provider](#create_identity_provider)
    - [create_network_settings](#create_network_settings)
    - [create_portal](#create_portal)
    - [create_trust_store](#create_trust_store)
    - [create_user_settings](#create_user_settings)
    - [delete_browser_settings](#delete_browser_settings)
    - [delete_identity_provider](#delete_identity_provider)
    - [delete_network_settings](#delete_network_settings)
    - [delete_portal](#delete_portal)
    - [delete_trust_store](#delete_trust_store)
    - [delete_user_settings](#delete_user_settings)
    - [disassociate_browser_settings](#disassociate_browser_settings)
    - [disassociate_network_settings](#disassociate_network_settings)
    - [disassociate_trust_store](#disassociate_trust_store)
    - [disassociate_user_settings](#disassociate_user_settings)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_browser_settings](#get_browser_settings)
    - [get_identity_provider](#get_identity_provider)
    - [get_network_settings](#get_network_settings)
    - [get_portal](#get_portal)
    - [get_portal_service_provider_metadata](#get_portal_service_provider_metadata)
    - [get_trust_store](#get_trust_store)
    - [get_trust_store_certificate](#get_trust_store_certificate)
    - [get_user_settings](#get_user_settings)
    - [list_browser_settings](#list_browser_settings)
    - [list_identity_providers](#list_identity_providers)
    - [list_network_settings](#list_network_settings)
    - [list_portals](#list_portals)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_trust_store_certificates](#list_trust_store_certificates)
    - [list_trust_stores](#list_trust_stores)
    - [list_user_settings](#list_user_settings)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_browser_settings](#update_browser_settings)
    - [update_identity_provider](#update_identity_provider)
    - [update_network_settings](#update_network_settings)
    - [update_portal](#update_portal)
    - [update_trust_store](#update_trust_store)
    - [update_user_settings](#update_user_settings)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="workspaceswebclient"></a>

## WorkSpacesWebClient

Type annotations for `session.create_client("workspaces-web")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_workspaces_web.client import WorkSpacesWebClient

session = get_session()
async with session.create_client("workspaces-web") as client:
    client: WorkSpacesWebClient
```

Boto3 documentation:
[WorkSpacesWeb.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_workspaces_web.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.TooManyTagsException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

WorkSpacesWebClient exceptions.

Type annotations for `session.create_client("workspaces-web").exceptions`
method.

Boto3 documentation:
[WorkSpacesWeb.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="associate\_browser\_settings"></a>

### associate_browser_settings

Associates a browser settings resource with a web portal.

Type annotations for
`session.create_client("workspaces-web").associate_browser_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.associate_browser_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_browser_settings)

Asynchronous method. Use `await associate_browser_settings(...)` for a
synchronous call.

Arguments mapping described in
[AssociateBrowserSettingsRequestRequestTypeDef](./type_defs.md#associatebrowsersettingsrequestrequesttypedef).

Keyword-only arguments:

- `browserSettingsArn`: `str` *(required)*
- `portalArn`: `str` *(required)*

Returns a `Coroutine` for
[AssociateBrowserSettingsResponseTypeDef](./type_defs.md#associatebrowsersettingsresponsetypedef).

<a id="associate\_network\_settings"></a>

### associate_network_settings

Associates a network settings resource with a web portal.

Type annotations for
`session.create_client("workspaces-web").associate_network_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.associate_network_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_network_settings)

Asynchronous method. Use `await associate_network_settings(...)` for a
synchronous call.

Arguments mapping described in
[AssociateNetworkSettingsRequestRequestTypeDef](./type_defs.md#associatenetworksettingsrequestrequesttypedef).

Keyword-only arguments:

- `networkSettingsArn`: `str` *(required)*
- `portalArn`: `str` *(required)*

Returns a `Coroutine` for
[AssociateNetworkSettingsResponseTypeDef](./type_defs.md#associatenetworksettingsresponsetypedef).

<a id="associate\_trust\_store"></a>

### associate_trust_store

Associates a trust store with a web portal.

Type annotations for
`session.create_client("workspaces-web").associate_trust_store` method.

Boto3 documentation:
[WorkSpacesWeb.Client.associate_trust_store](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_trust_store)

Asynchronous method. Use `await associate_trust_store(...)` for a synchronous
call.

Arguments mapping described in
[AssociateTrustStoreRequestRequestTypeDef](./type_defs.md#associatetruststorerequestrequesttypedef).

Keyword-only arguments:

- `portalArn`: `str` *(required)*
- `trustStoreArn`: `str` *(required)*

Returns a `Coroutine` for
[AssociateTrustStoreResponseTypeDef](./type_defs.md#associatetruststoreresponsetypedef).

<a id="associate\_user\_settings"></a>

### associate_user_settings

Associates a user settings resource with a web portal.

Type annotations for
`session.create_client("workspaces-web").associate_user_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.associate_user_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_user_settings)

Asynchronous method. Use `await associate_user_settings(...)` for a synchronous
call.

Arguments mapping described in
[AssociateUserSettingsRequestRequestTypeDef](./type_defs.md#associateusersettingsrequestrequesttypedef).

Keyword-only arguments:

- `portalArn`: `str` *(required)*
- `userSettingsArn`: `str` *(required)*

Returns a `Coroutine` for
[AssociateUserSettingsResponseTypeDef](./type_defs.md#associateusersettingsresponsetypedef).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("workspaces-web").can_paginate`
method.

Boto3 documentation:
[WorkSpacesWeb.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_browser\_settings"></a>

### create_browser_settings

Creates a browser settings resource that can be associated with a web portal.

Type annotations for
`session.create_client("workspaces-web").create_browser_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.create_browser_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_browser_settings)

Asynchronous method. Use `await create_browser_settings(...)` for a synchronous
call.

Arguments mapping described in
[CreateBrowserSettingsRequestRequestTypeDef](./type_defs.md#createbrowsersettingsrequestrequesttypedef).

Keyword-only arguments:

- `browserPolicy`: `str` *(required)*
- `additionalEncryptionContext`: `Mapping`\[`str`, `str`\]
- `clientToken`: `str`
- `customerManagedKey`: `str`
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateBrowserSettingsResponseTypeDef](./type_defs.md#createbrowsersettingsresponsetypedef).

<a id="create\_identity\_provider"></a>

### create_identity_provider

Creates an identity provider resource that is then associated with a web
portal.

Type annotations for
`session.create_client("workspaces-web").create_identity_provider` method.

Boto3 documentation:
[WorkSpacesWeb.Client.create_identity_provider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_identity_provider)

Asynchronous method. Use `await create_identity_provider(...)` for a
synchronous call.

Arguments mapping described in
[CreateIdentityProviderRequestRequestTypeDef](./type_defs.md#createidentityproviderrequestrequesttypedef).

Keyword-only arguments:

- `identityProviderDetails`: `Mapping`\[`str`, `str`\] *(required)*
- `identityProviderName`: `str` *(required)*
- `identityProviderType`:
  [IdentityProviderTypeType](./literals.md#identityprovidertypetype)
  *(required)*
- `portalArn`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[CreateIdentityProviderResponseTypeDef](./type_defs.md#createidentityproviderresponsetypedef).

<a id="create\_network\_settings"></a>

### create_network_settings

Creates a network settings resource that can be associated with a web portal.

Type annotations for
`session.create_client("workspaces-web").create_network_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.create_network_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_network_settings)

Asynchronous method. Use `await create_network_settings(...)` for a synchronous
call.

Arguments mapping described in
[CreateNetworkSettingsRequestRequestTypeDef](./type_defs.md#createnetworksettingsrequestrequesttypedef).

Keyword-only arguments:

- `securityGroupIds`: `Sequence`\[`str`\] *(required)*
- `subnetIds`: `Sequence`\[`str`\] *(required)*
- `vpcId`: `str` *(required)*
- `clientToken`: `str`
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateNetworkSettingsResponseTypeDef](./type_defs.md#createnetworksettingsresponsetypedef).

<a id="create\_portal"></a>

### create_portal

Creates a web portal.

Type annotations for `session.create_client("workspaces-web").create_portal`
method.

Boto3 documentation:
[WorkSpacesWeb.Client.create_portal](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_portal)

Asynchronous method. Use `await create_portal(...)` for a synchronous call.

Arguments mapping described in
[CreatePortalRequestRequestTypeDef](./type_defs.md#createportalrequestrequesttypedef).

Keyword-only arguments:

- `additionalEncryptionContext`: `Mapping`\[`str`, `str`\]
- `clientToken`: `str`
- `customerManagedKey`: `str`
- `displayName`: `str`
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreatePortalResponseTypeDef](./type_defs.md#createportalresponsetypedef).

<a id="create\_trust\_store"></a>

### create_trust_store

Creates a trust store that can be associated with a web portal.

Type annotations for
`session.create_client("workspaces-web").create_trust_store` method.

Boto3 documentation:
[WorkSpacesWeb.Client.create_trust_store](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_trust_store)

Asynchronous method. Use `await create_trust_store(...)` for a synchronous
call.

Arguments mapping described in
[CreateTrustStoreRequestRequestTypeDef](./type_defs.md#createtruststorerequestrequesttypedef).

Keyword-only arguments:

- `certificateList`: `Sequence`\[`Union`\[`bytes`, `IO`\[`bytes`\],
  `StreamingBody`\]\] *(required)*
- `clientToken`: `str`
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateTrustStoreResponseTypeDef](./type_defs.md#createtruststoreresponsetypedef).

<a id="create\_user\_settings"></a>

### create_user_settings

Creates a user settings resource that can be associated with a web portal.

Type annotations for
`session.create_client("workspaces-web").create_user_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.create_user_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_user_settings)

Asynchronous method. Use `await create_user_settings(...)` for a synchronous
call.

Arguments mapping described in
[CreateUserSettingsRequestRequestTypeDef](./type_defs.md#createusersettingsrequestrequesttypedef).

Keyword-only arguments:

- `copyAllowed`: [EnabledTypeType](./literals.md#enabledtypetype) *(required)*
- `downloadAllowed`: [EnabledTypeType](./literals.md#enabledtypetype)
  *(required)*
- `pasteAllowed`: [EnabledTypeType](./literals.md#enabledtypetype) *(required)*
- `printAllowed`: [EnabledTypeType](./literals.md#enabledtypetype) *(required)*
- `uploadAllowed`: [EnabledTypeType](./literals.md#enabledtypetype)
  *(required)*
- `clientToken`: `str`
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateUserSettingsResponseTypeDef](./type_defs.md#createusersettingsresponsetypedef).

<a id="delete\_browser\_settings"></a>

### delete_browser_settings

Deletes browser settings.

Type annotations for
`session.create_client("workspaces-web").delete_browser_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.delete_browser_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_browser_settings)

Asynchronous method. Use `await delete_browser_settings(...)` for a synchronous
call.

Arguments mapping described in
[DeleteBrowserSettingsRequestRequestTypeDef](./type_defs.md#deletebrowsersettingsrequestrequesttypedef).

Keyword-only arguments:

- `browserSettingsArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_identity\_provider"></a>

### delete_identity_provider

Deletes the identity provider.

Type annotations for
`session.create_client("workspaces-web").delete_identity_provider` method.

Boto3 documentation:
[WorkSpacesWeb.Client.delete_identity_provider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_identity_provider)

Asynchronous method. Use `await delete_identity_provider(...)` for a
synchronous call.

Arguments mapping described in
[DeleteIdentityProviderRequestRequestTypeDef](./type_defs.md#deleteidentityproviderrequestrequesttypedef).

Keyword-only arguments:

- `identityProviderArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_network\_settings"></a>

### delete_network_settings

Deletes network settings.

Type annotations for
`session.create_client("workspaces-web").delete_network_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.delete_network_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_network_settings)

Asynchronous method. Use `await delete_network_settings(...)` for a synchronous
call.

Arguments mapping described in
[DeleteNetworkSettingsRequestRequestTypeDef](./type_defs.md#deletenetworksettingsrequestrequesttypedef).

Keyword-only arguments:

- `networkSettingsArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_portal"></a>

### delete_portal

Deletes a web portal.

Type annotations for `session.create_client("workspaces-web").delete_portal`
method.

Boto3 documentation:
[WorkSpacesWeb.Client.delete_portal](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_portal)

Asynchronous method. Use `await delete_portal(...)` for a synchronous call.

Arguments mapping described in
[DeletePortalRequestRequestTypeDef](./type_defs.md#deleteportalrequestrequesttypedef).

Keyword-only arguments:

- `portalArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_trust\_store"></a>

### delete_trust_store

Deletes the trust store.

Type annotations for
`session.create_client("workspaces-web").delete_trust_store` method.

Boto3 documentation:
[WorkSpacesWeb.Client.delete_trust_store](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_trust_store)

Asynchronous method. Use `await delete_trust_store(...)` for a synchronous
call.

Arguments mapping described in
[DeleteTrustStoreRequestRequestTypeDef](./type_defs.md#deletetruststorerequestrequesttypedef).

Keyword-only arguments:

- `trustStoreArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_user\_settings"></a>

### delete_user_settings

Deletes user settings.

Type annotations for
`session.create_client("workspaces-web").delete_user_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.delete_user_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_user_settings)

Asynchronous method. Use `await delete_user_settings(...)` for a synchronous
call.

Arguments mapping described in
[DeleteUserSettingsRequestRequestTypeDef](./type_defs.md#deleteusersettingsrequestrequesttypedef).

Keyword-only arguments:

- `userSettingsArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate\_browser\_settings"></a>

### disassociate_browser_settings

Disassociates browser settings from a web portal.

Type annotations for
`session.create_client("workspaces-web").disassociate_browser_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.disassociate_browser_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_browser_settings)

Asynchronous method. Use `await disassociate_browser_settings(...)` for a
synchronous call.

Arguments mapping described in
[DisassociateBrowserSettingsRequestRequestTypeDef](./type_defs.md#disassociatebrowsersettingsrequestrequesttypedef).

Keyword-only arguments:

- `portalArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate\_network\_settings"></a>

### disassociate_network_settings

Disassociates network settings from a web portal.

Type annotations for
`session.create_client("workspaces-web").disassociate_network_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.disassociate_network_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_network_settings)

Asynchronous method. Use `await disassociate_network_settings(...)` for a
synchronous call.

Arguments mapping described in
[DisassociateNetworkSettingsRequestRequestTypeDef](./type_defs.md#disassociatenetworksettingsrequestrequesttypedef).

Keyword-only arguments:

- `portalArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate\_trust\_store"></a>

### disassociate_trust_store

Disassociates a trust store from a web portal.

Type annotations for
`session.create_client("workspaces-web").disassociate_trust_store` method.

Boto3 documentation:
[WorkSpacesWeb.Client.disassociate_trust_store](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_trust_store)

Asynchronous method. Use `await disassociate_trust_store(...)` for a
synchronous call.

Arguments mapping described in
[DisassociateTrustStoreRequestRequestTypeDef](./type_defs.md#disassociatetruststorerequestrequesttypedef).

Keyword-only arguments:

- `portalArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate\_user\_settings"></a>

### disassociate_user_settings

Disassociates user settings from a web portal.

Type annotations for
`session.create_client("workspaces-web").disassociate_user_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.disassociate_user_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_user_settings)

Asynchronous method. Use `await disassociate_user_settings(...)` for a
synchronous call.

Arguments mapping described in
[DisassociateUserSettingsRequestRequestTypeDef](./type_defs.md#disassociateusersettingsrequestrequesttypedef).

Keyword-only arguments:

- `portalArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("workspaces-web").generate_presigned_url` method.

Boto3 documentation:
[WorkSpacesWeb.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_browser\_settings"></a>

### get_browser_settings

Gets browser settings.

Type annotations for
`session.create_client("workspaces-web").get_browser_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.get_browser_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_browser_settings)

Asynchronous method. Use `await get_browser_settings(...)` for a synchronous
call.

Arguments mapping described in
[GetBrowserSettingsRequestRequestTypeDef](./type_defs.md#getbrowsersettingsrequestrequesttypedef).

Keyword-only arguments:

- `browserSettingsArn`: `str` *(required)*

Returns a `Coroutine` for
[GetBrowserSettingsResponseTypeDef](./type_defs.md#getbrowsersettingsresponsetypedef).

<a id="get\_identity\_provider"></a>

### get_identity_provider

Gets the identity provider.

Type annotations for
`session.create_client("workspaces-web").get_identity_provider` method.

Boto3 documentation:
[WorkSpacesWeb.Client.get_identity_provider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_identity_provider)

Asynchronous method. Use `await get_identity_provider(...)` for a synchronous
call.

Arguments mapping described in
[GetIdentityProviderRequestRequestTypeDef](./type_defs.md#getidentityproviderrequestrequesttypedef).

Keyword-only arguments:

- `identityProviderArn`: `str` *(required)*

Returns a `Coroutine` for
[GetIdentityProviderResponseTypeDef](./type_defs.md#getidentityproviderresponsetypedef).

<a id="get\_network\_settings"></a>

### get_network_settings

Gets the network settings.

Type annotations for
`session.create_client("workspaces-web").get_network_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.get_network_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_network_settings)

Asynchronous method. Use `await get_network_settings(...)` for a synchronous
call.

Arguments mapping described in
[GetNetworkSettingsRequestRequestTypeDef](./type_defs.md#getnetworksettingsrequestrequesttypedef).

Keyword-only arguments:

- `networkSettingsArn`: `str` *(required)*

Returns a `Coroutine` for
[GetNetworkSettingsResponseTypeDef](./type_defs.md#getnetworksettingsresponsetypedef).

<a id="get\_portal"></a>

### get_portal

Gets the web portal.

Type annotations for `session.create_client("workspaces-web").get_portal`
method.

Boto3 documentation:
[WorkSpacesWeb.Client.get_portal](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_portal)

Asynchronous method. Use `await get_portal(...)` for a synchronous call.

Arguments mapping described in
[GetPortalRequestRequestTypeDef](./type_defs.md#getportalrequestrequesttypedef).

Keyword-only arguments:

- `portalArn`: `str` *(required)*

Returns a `Coroutine` for
[GetPortalResponseTypeDef](./type_defs.md#getportalresponsetypedef).

<a id="get\_portal\_service\_provider\_metadata"></a>

### get_portal_service_provider_metadata

Gets the service provider metadata.

Type annotations for
`session.create_client("workspaces-web").get_portal_service_provider_metadata`
method.

Boto3 documentation:
[WorkSpacesWeb.Client.get_portal_service_provider_metadata](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_portal_service_provider_metadata)

Asynchronous method. Use `await get_portal_service_provider_metadata(...)` for
a synchronous call.

Arguments mapping described in
[GetPortalServiceProviderMetadataRequestRequestTypeDef](./type_defs.md#getportalserviceprovidermetadatarequestrequesttypedef).

Keyword-only arguments:

- `portalArn`: `str` *(required)*

Returns a `Coroutine` for
[GetPortalServiceProviderMetadataResponseTypeDef](./type_defs.md#getportalserviceprovidermetadataresponsetypedef).

<a id="get\_trust\_store"></a>

### get_trust_store

Gets the trust store.

Type annotations for `session.create_client("workspaces-web").get_trust_store`
method.

Boto3 documentation:
[WorkSpacesWeb.Client.get_trust_store](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_trust_store)

Asynchronous method. Use `await get_trust_store(...)` for a synchronous call.

Arguments mapping described in
[GetTrustStoreRequestRequestTypeDef](./type_defs.md#gettruststorerequestrequesttypedef).

Keyword-only arguments:

- `trustStoreArn`: `str` *(required)*

Returns a `Coroutine` for
[GetTrustStoreResponseTypeDef](./type_defs.md#gettruststoreresponsetypedef).

<a id="get\_trust\_store\_certificate"></a>

### get_trust_store_certificate

Gets the trust store certificate.

Type annotations for
`session.create_client("workspaces-web").get_trust_store_certificate` method.

Boto3 documentation:
[WorkSpacesWeb.Client.get_trust_store_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_trust_store_certificate)

Asynchronous method. Use `await get_trust_store_certificate(...)` for a
synchronous call.

Arguments mapping described in
[GetTrustStoreCertificateRequestRequestTypeDef](./type_defs.md#gettruststorecertificaterequestrequesttypedef).

Keyword-only arguments:

- `thumbprint`: `str` *(required)*
- `trustStoreArn`: `str` *(required)*

Returns a `Coroutine` for
[GetTrustStoreCertificateResponseTypeDef](./type_defs.md#gettruststorecertificateresponsetypedef).

<a id="get\_user\_settings"></a>

### get_user_settings

Gets user settings.

Type annotations for
`session.create_client("workspaces-web").get_user_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.get_user_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_user_settings)

Asynchronous method. Use `await get_user_settings(...)` for a synchronous call.

Arguments mapping described in
[GetUserSettingsRequestRequestTypeDef](./type_defs.md#getusersettingsrequestrequesttypedef).

Keyword-only arguments:

- `userSettingsArn`: `str` *(required)*

Returns a `Coroutine` for
[GetUserSettingsResponseTypeDef](./type_defs.md#getusersettingsresponsetypedef).

<a id="list\_browser\_settings"></a>

### list_browser_settings

Retrieves a list of browser settings.

Type annotations for
`session.create_client("workspaces-web").list_browser_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.list_browser_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_browser_settings)

Asynchronous method. Use `await list_browser_settings(...)` for a synchronous
call.

Arguments mapping described in
[ListBrowserSettingsRequestRequestTypeDef](./type_defs.md#listbrowsersettingsrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListBrowserSettingsResponseTypeDef](./type_defs.md#listbrowsersettingsresponsetypedef).

<a id="list\_identity\_providers"></a>

### list_identity_providers

Retrieves a list of identity providers for a specific web portal.

Type annotations for
`session.create_client("workspaces-web").list_identity_providers` method.

Boto3 documentation:
[WorkSpacesWeb.Client.list_identity_providers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_identity_providers)

Asynchronous method. Use `await list_identity_providers(...)` for a synchronous
call.

Arguments mapping described in
[ListIdentityProvidersRequestRequestTypeDef](./type_defs.md#listidentityprovidersrequestrequesttypedef).

Keyword-only arguments:

- `portalArn`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef).

<a id="list\_network\_settings"></a>

### list_network_settings

Retrieves a list of network settings.

Type annotations for
`session.create_client("workspaces-web").list_network_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.list_network_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_network_settings)

Asynchronous method. Use `await list_network_settings(...)` for a synchronous
call.

Arguments mapping described in
[ListNetworkSettingsRequestRequestTypeDef](./type_defs.md#listnetworksettingsrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListNetworkSettingsResponseTypeDef](./type_defs.md#listnetworksettingsresponsetypedef).

<a id="list\_portals"></a>

### list_portals

Retrieves a list or web portals.

Type annotations for `session.create_client("workspaces-web").list_portals`
method.

Boto3 documentation:
[WorkSpacesWeb.Client.list_portals](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_portals)

Asynchronous method. Use `await list_portals(...)` for a synchronous call.

Arguments mapping described in
[ListPortalsRequestRequestTypeDef](./type_defs.md#listportalsrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListPortalsResponseTypeDef](./type_defs.md#listportalsresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Retrieves a list of tags for a resource.

Type annotations for
`session.create_client("workspaces-web").list_tags_for_resource` method.

Boto3 documentation:
[WorkSpacesWeb.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="list\_trust\_store\_certificates"></a>

### list_trust_store_certificates

Retrieves a list of trust store certificates.

Type annotations for
`session.create_client("workspaces-web").list_trust_store_certificates` method.

Boto3 documentation:
[WorkSpacesWeb.Client.list_trust_store_certificates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_trust_store_certificates)

Asynchronous method. Use `await list_trust_store_certificates(...)` for a
synchronous call.

Arguments mapping described in
[ListTrustStoreCertificatesRequestRequestTypeDef](./type_defs.md#listtruststorecertificatesrequestrequesttypedef).

Keyword-only arguments:

- `trustStoreArn`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListTrustStoreCertificatesResponseTypeDef](./type_defs.md#listtruststorecertificatesresponsetypedef).

<a id="list\_trust\_stores"></a>

### list_trust_stores

Retrieves a list of trust stores.

Type annotations for
`session.create_client("workspaces-web").list_trust_stores` method.

Boto3 documentation:
[WorkSpacesWeb.Client.list_trust_stores](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_trust_stores)

Asynchronous method. Use `await list_trust_stores(...)` for a synchronous call.

Arguments mapping described in
[ListTrustStoresRequestRequestTypeDef](./type_defs.md#listtruststoresrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListTrustStoresResponseTypeDef](./type_defs.md#listtruststoresresponsetypedef).

<a id="list\_user\_settings"></a>

### list_user_settings

Retrieves a list of user settings.

Type annotations for
`session.create_client("workspaces-web").list_user_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.list_user_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_user_settings)

Asynchronous method. Use `await list_user_settings(...)` for a synchronous
call.

Arguments mapping described in
[ListUserSettingsRequestRequestTypeDef](./type_defs.md#listusersettingsrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListUserSettingsResponseTypeDef](./type_defs.md#listusersettingsresponsetypedef).

<a id="tag\_resource"></a>

### tag_resource

Adds or overwrites one or more tags for the specified resource.

Type annotations for `session.create_client("workspaces-web").tag_resource`
method.

Boto3 documentation:
[WorkSpacesWeb.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Removes one or more tags from the specified resource.

Type annotations for `session.create_client("workspaces-web").untag_resource`
method.

Boto3 documentation:
[WorkSpacesWeb.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_browser\_settings"></a>

### update_browser_settings

Updates browser settings.

Type annotations for
`session.create_client("workspaces-web").update_browser_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.update_browser_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_browser_settings)

Asynchronous method. Use `await update_browser_settings(...)` for a synchronous
call.

Arguments mapping described in
[UpdateBrowserSettingsRequestRequestTypeDef](./type_defs.md#updatebrowsersettingsrequestrequesttypedef).

Keyword-only arguments:

- `browserSettingsArn`: `str` *(required)*
- `browserPolicy`: `str`
- `clientToken`: `str`

Returns a `Coroutine` for
[UpdateBrowserSettingsResponseTypeDef](./type_defs.md#updatebrowsersettingsresponsetypedef).

<a id="update\_identity\_provider"></a>

### update_identity_provider

Updates the identity provider.

Type annotations for
`session.create_client("workspaces-web").update_identity_provider` method.

Boto3 documentation:
[WorkSpacesWeb.Client.update_identity_provider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_identity_provider)

Asynchronous method. Use `await update_identity_provider(...)` for a
synchronous call.

Arguments mapping described in
[UpdateIdentityProviderRequestRequestTypeDef](./type_defs.md#updateidentityproviderrequestrequesttypedef).

Keyword-only arguments:

- `identityProviderArn`: `str` *(required)*
- `clientToken`: `str`
- `identityProviderDetails`: `Mapping`\[`str`, `str`\]
- `identityProviderName`: `str`
- `identityProviderType`:
  [IdentityProviderTypeType](./literals.md#identityprovidertypetype)

Returns a `Coroutine` for
[UpdateIdentityProviderResponseTypeDef](./type_defs.md#updateidentityproviderresponsetypedef).

<a id="update\_network\_settings"></a>

### update_network_settings

Updates network settings.

Type annotations for
`session.create_client("workspaces-web").update_network_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.update_network_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_network_settings)

Asynchronous method. Use `await update_network_settings(...)` for a synchronous
call.

Arguments mapping described in
[UpdateNetworkSettingsRequestRequestTypeDef](./type_defs.md#updatenetworksettingsrequestrequesttypedef).

Keyword-only arguments:

- `networkSettingsArn`: `str` *(required)*
- `clientToken`: `str`
- `securityGroupIds`: `Sequence`\[`str`\]
- `subnetIds`: `Sequence`\[`str`\]
- `vpcId`: `str`

Returns a `Coroutine` for
[UpdateNetworkSettingsResponseTypeDef](./type_defs.md#updatenetworksettingsresponsetypedef).

<a id="update\_portal"></a>

### update_portal

Updates a web portal.

Type annotations for `session.create_client("workspaces-web").update_portal`
method.

Boto3 documentation:
[WorkSpacesWeb.Client.update_portal](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_portal)

Asynchronous method. Use `await update_portal(...)` for a synchronous call.

Arguments mapping described in
[UpdatePortalRequestRequestTypeDef](./type_defs.md#updateportalrequestrequesttypedef).

Keyword-only arguments:

- `portalArn`: `str` *(required)*
- `displayName`: `str`

Returns a `Coroutine` for
[UpdatePortalResponseTypeDef](./type_defs.md#updateportalresponsetypedef).

<a id="update\_trust\_store"></a>

### update_trust_store

Updates the trust store.

Type annotations for
`session.create_client("workspaces-web").update_trust_store` method.

Boto3 documentation:
[WorkSpacesWeb.Client.update_trust_store](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_trust_store)

Asynchronous method. Use `await update_trust_store(...)` for a synchronous
call.

Arguments mapping described in
[UpdateTrustStoreRequestRequestTypeDef](./type_defs.md#updatetruststorerequestrequesttypedef).

Keyword-only arguments:

- `trustStoreArn`: `str` *(required)*
- `certificatesToAdd`: `Sequence`\[`Union`\[`bytes`, `IO`\[`bytes`\],
  `StreamingBody`\]\]
- `certificatesToDelete`: `Sequence`\[`str`\]
- `clientToken`: `str`

Returns a `Coroutine` for
[UpdateTrustStoreResponseTypeDef](./type_defs.md#updatetruststoreresponsetypedef).

<a id="update\_user\_settings"></a>

### update_user_settings

Updates the user settings.

Type annotations for
`session.create_client("workspaces-web").update_user_settings` method.

Boto3 documentation:
[WorkSpacesWeb.Client.update_user_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_user_settings)

Asynchronous method. Use `await update_user_settings(...)` for a synchronous
call.

Arguments mapping described in
[UpdateUserSettingsRequestRequestTypeDef](./type_defs.md#updateusersettingsrequestrequesttypedef).

Keyword-only arguments:

- `userSettingsArn`: `str` *(required)*
- `clientToken`: `str`
- `copyAllowed`: [EnabledTypeType](./literals.md#enabledtypetype)
- `downloadAllowed`: [EnabledTypeType](./literals.md#enabledtypetype)
- `pasteAllowed`: [EnabledTypeType](./literals.md#enabledtypetype)
- `printAllowed`: [EnabledTypeType](./literals.md#enabledtypetype)
- `uploadAllowed`: [EnabledTypeType](./literals.md#enabledtypetype)

Returns a `Coroutine` for
[UpdateUserSettingsResponseTypeDef](./type_defs.md#updateusersettingsresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("workspaces-web").__aenter__`
method.

Boto3 documentation:
[WorkSpacesWeb.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [WorkSpacesWebClient](#workspaceswebclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("workspaces-web").__aexit__`
method.

Boto3 documentation:
[WorkSpacesWeb.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
