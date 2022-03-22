<a id="cognitoidentityclient-for-aiobotocore-cognitoidentity-module"></a>

# CognitoIdentityClient for aiobotocore CognitoIdentity module

> [Index](../README.md) > [CognitoIdentity](./README.md) >
> CognitoIdentityClient

Auto-generated documentation for
[CognitoIdentity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
type annotations stubs module
[types-aiobotocore-cognito-identity](https://pypi.org/project/types-aiobotocore-cognito-identity/).

- [CognitoIdentityClient for aiobotocore CognitoIdentity module](#cognitoidentityclient-for-aiobotocore-cognitoidentity-module)
  - [CognitoIdentityClient](#cognitoidentityclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_identity_pool](#create_identity_pool)
    - [delete_identities](#delete_identities)
    - [delete_identity_pool](#delete_identity_pool)
    - [describe_identity](#describe_identity)
    - [describe_identity_pool](#describe_identity_pool)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_credentials_for_identity](#get_credentials_for_identity)
    - [get_id](#get_id)
    - [get_identity_pool_roles](#get_identity_pool_roles)
    - [get_open_id_token](#get_open_id_token)
    - [get_open_id_token_for_developer_identity](#get_open_id_token_for_developer_identity)
    - [get_principal_tag_attribute_map](#get_principal_tag_attribute_map)
    - [list_identities](#list_identities)
    - [list_identity_pools](#list_identity_pools)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [lookup_developer_identity](#lookup_developer_identity)
    - [merge_developer_identities](#merge_developer_identities)
    - [set_identity_pool_roles](#set_identity_pool_roles)
    - [set_principal_tag_attribute_map](#set_principal_tag_attribute_map)
    - [tag_resource](#tag_resource)
    - [unlink_developer_identity](#unlink_developer_identity)
    - [unlink_identity](#unlink_identity)
    - [untag_resource](#untag_resource)
    - [update_identity_pool](#update_identity_pool)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="cognitoidentityclient"></a>

## CognitoIdentityClient

Type annotations for `session.create_client("cognito-identity")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_cognito_identity.client import CognitoIdentityClient

session = get_session()
async with session.create_client("cognito-identity") as client:
    client: CognitoIdentityClient
```

Boto3 documentation:
[CognitoIdentity.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_cognito_identity.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConcurrentModificationException`
- `Exceptions.DeveloperUserAlreadyRegisteredException`
- `Exceptions.ExternalServiceException`
- `Exceptions.InternalErrorException`
- `Exceptions.InvalidIdentityPoolConfigurationException`
- `Exceptions.InvalidParameterException`
- `Exceptions.LimitExceededException`
- `Exceptions.NotAuthorizedException`
- `Exceptions.ResourceConflictException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.TooManyRequestsException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

CognitoIdentityClient exceptions.

Type annotations for `session.create_client("cognito-identity").exceptions`
method.

Boto3 documentation:
[CognitoIdentity.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("cognito-identity").can_paginate`
method.

Boto3 documentation:
[CognitoIdentity.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_identity\_pool"></a>

### create_identity_pool

Creates a new identity pool.

Type annotations for
`session.create_client("cognito-identity").create_identity_pool` method.

Boto3 documentation:
[CognitoIdentity.Client.create_identity_pool](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.create_identity_pool)

Asynchronous method. Use `await create_identity_pool(...)` for a synchronous
call.

Arguments mapping described in
[CreateIdentityPoolInputRequestTypeDef](./type_defs.md#createidentitypoolinputrequesttypedef).

Keyword-only arguments:

- `IdentityPoolName`: `str` *(required)*
- `AllowUnauthenticatedIdentities`: `bool` *(required)*
- `AllowClassicFlow`: `bool`
- `SupportedLoginProviders`: `Mapping`\[`str`, `str`\]
- `DeveloperProviderName`: `str`
- `OpenIdConnectProviderARNs`: `Sequence`\[`str`\]
- `CognitoIdentityProviders`:
  `Sequence`\[[CognitoIdentityProviderTypeDef](./type_defs.md#cognitoidentityprovidertypedef)\]
- `SamlProviderARNs`: `Sequence`\[`str`\]
- `IdentityPoolTags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[IdentityPoolTypeDef](./type_defs.md#identitypooltypedef).

<a id="delete\_identities"></a>

### delete_identities

Deletes identities from an identity pool.

Type annotations for
`session.create_client("cognito-identity").delete_identities` method.

Boto3 documentation:
[CognitoIdentity.Client.delete_identities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.delete_identities)

Asynchronous method. Use `await delete_identities(...)` for a synchronous call.

Arguments mapping described in
[DeleteIdentitiesInputRequestTypeDef](./type_defs.md#deleteidentitiesinputrequesttypedef).

Keyword-only arguments:

- `IdentityIdsToDelete`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[DeleteIdentitiesResponseTypeDef](./type_defs.md#deleteidentitiesresponsetypedef).

<a id="delete\_identity\_pool"></a>

### delete_identity_pool

Deletes an identity pool.

Type annotations for
`session.create_client("cognito-identity").delete_identity_pool` method.

Boto3 documentation:
[CognitoIdentity.Client.delete_identity_pool](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.delete_identity_pool)

Asynchronous method. Use `await delete_identity_pool(...)` for a synchronous
call.

Arguments mapping described in
[DeleteIdentityPoolInputRequestTypeDef](./type_defs.md#deleteidentitypoolinputrequesttypedef).

Keyword-only arguments:

- `IdentityPoolId`: `str` *(required)*

<a id="describe\_identity"></a>

### describe_identity

Returns metadata related to the given identity, including when the identity was
created and any associated linked logins.

Type annotations for
`session.create_client("cognito-identity").describe_identity` method.

Boto3 documentation:
[CognitoIdentity.Client.describe_identity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.describe_identity)

Asynchronous method. Use `await describe_identity(...)` for a synchronous call.

Arguments mapping described in
[DescribeIdentityInputRequestTypeDef](./type_defs.md#describeidentityinputrequesttypedef).

Keyword-only arguments:

- `IdentityId`: `str` *(required)*

Returns a `Coroutine` for
[IdentityDescriptionResponseMetadataTypeDef](./type_defs.md#identitydescriptionresponsemetadatatypedef).

<a id="describe\_identity\_pool"></a>

### describe_identity_pool

Gets details about a particular identity pool, including the pool name, ID
description, creation date, and current number of users.

Type annotations for
`session.create_client("cognito-identity").describe_identity_pool` method.

Boto3 documentation:
[CognitoIdentity.Client.describe_identity_pool](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.describe_identity_pool)

Asynchronous method. Use `await describe_identity_pool(...)` for a synchronous
call.

Arguments mapping described in
[DescribeIdentityPoolInputRequestTypeDef](./type_defs.md#describeidentitypoolinputrequesttypedef).

Keyword-only arguments:

- `IdentityPoolId`: `str` *(required)*

Returns a `Coroutine` for
[IdentityPoolTypeDef](./type_defs.md#identitypooltypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("cognito-identity").generate_presigned_url` method.

Boto3 documentation:
[CognitoIdentity.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_credentials\_for\_identity"></a>

### get_credentials_for_identity

Returns credentials for the provided identity ID.

Type annotations for
`session.create_client("cognito-identity").get_credentials_for_identity`
method.

Boto3 documentation:
[CognitoIdentity.Client.get_credentials_for_identity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.get_credentials_for_identity)

Asynchronous method. Use `await get_credentials_for_identity(...)` for a
synchronous call.

Arguments mapping described in
[GetCredentialsForIdentityInputRequestTypeDef](./type_defs.md#getcredentialsforidentityinputrequesttypedef).

Keyword-only arguments:

- `IdentityId`: `str` *(required)*
- `Logins`: `Mapping`\[`str`, `str`\]
- `CustomRoleArn`: `str`

Returns a `Coroutine` for
[GetCredentialsForIdentityResponseTypeDef](./type_defs.md#getcredentialsforidentityresponsetypedef).

<a id="get\_id"></a>

### get_id

Generates (or retrieves) a Cognito ID.

Type annotations for `session.create_client("cognito-identity").get_id` method.

Boto3 documentation:
[CognitoIdentity.Client.get_id](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.get_id)

Asynchronous method. Use `await get_id(...)` for a synchronous call.

Arguments mapping described in
[GetIdInputRequestTypeDef](./type_defs.md#getidinputrequesttypedef).

Keyword-only arguments:

- `IdentityPoolId`: `str` *(required)*
- `AccountId`: `str`
- `Logins`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[GetIdResponseTypeDef](./type_defs.md#getidresponsetypedef).

<a id="get\_identity\_pool\_roles"></a>

### get_identity_pool_roles

Gets the roles for an identity pool.

Type annotations for
`session.create_client("cognito-identity").get_identity_pool_roles` method.

Boto3 documentation:
[CognitoIdentity.Client.get_identity_pool_roles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.get_identity_pool_roles)

Asynchronous method. Use `await get_identity_pool_roles(...)` for a synchronous
call.

Arguments mapping described in
[GetIdentityPoolRolesInputRequestTypeDef](./type_defs.md#getidentitypoolrolesinputrequesttypedef).

Keyword-only arguments:

- `IdentityPoolId`: `str` *(required)*

Returns a `Coroutine` for
[GetIdentityPoolRolesResponseTypeDef](./type_defs.md#getidentitypoolrolesresponsetypedef).

<a id="get\_open\_id\_token"></a>

### get_open_id_token

Gets an OpenID token, using a known Cognito ID.

Type annotations for
`session.create_client("cognito-identity").get_open_id_token` method.

Boto3 documentation:
[CognitoIdentity.Client.get_open_id_token](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.get_open_id_token)

Asynchronous method. Use `await get_open_id_token(...)` for a synchronous call.

Arguments mapping described in
[GetOpenIdTokenInputRequestTypeDef](./type_defs.md#getopenidtokeninputrequesttypedef).

Keyword-only arguments:

- `IdentityId`: `str` *(required)*
- `Logins`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[GetOpenIdTokenResponseTypeDef](./type_defs.md#getopenidtokenresponsetypedef).

<a id="get\_open\_id\_token\_for\_developer\_identity"></a>

### get_open_id_token_for_developer_identity

Registers (or retrieves) a Cognito `IdentityId` and an OpenID Connect token for
a user authenticated by your backend authentication process.

Type annotations for
`session.create_client("cognito-identity").get_open_id_token_for_developer_identity`
method.

Boto3 documentation:
[CognitoIdentity.Client.get_open_id_token_for_developer_identity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.get_open_id_token_for_developer_identity)

Asynchronous method. Use `await get_open_id_token_for_developer_identity(...)`
for a synchronous call.

Arguments mapping described in
[GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef](./type_defs.md#getopenidtokenfordeveloperidentityinputrequesttypedef).

Keyword-only arguments:

- `IdentityPoolId`: `str` *(required)*
- `Logins`: `Mapping`\[`str`, `str`\] *(required)*
- `IdentityId`: `str`
- `PrincipalTags`: `Mapping`\[`str`, `str`\]
- `TokenDuration`: `int`

Returns a `Coroutine` for
[GetOpenIdTokenForDeveloperIdentityResponseTypeDef](./type_defs.md#getopenidtokenfordeveloperidentityresponsetypedef).

<a id="get\_principal\_tag\_attribute\_map"></a>

### get_principal_tag_attribute_map

Use `GetPrincipalTagAttributeMap` to list all mappings between `PrincipalTags`
and user attributes.

Type annotations for
`session.create_client("cognito-identity").get_principal_tag_attribute_map`
method.

Boto3 documentation:
[CognitoIdentity.Client.get_principal_tag_attribute_map](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.get_principal_tag_attribute_map)

Asynchronous method. Use `await get_principal_tag_attribute_map(...)` for a
synchronous call.

Arguments mapping described in
[GetPrincipalTagAttributeMapInputRequestTypeDef](./type_defs.md#getprincipaltagattributemapinputrequesttypedef).

Keyword-only arguments:

- `IdentityPoolId`: `str` *(required)*
- `IdentityProviderName`: `str` *(required)*

Returns a `Coroutine` for
[GetPrincipalTagAttributeMapResponseTypeDef](./type_defs.md#getprincipaltagattributemapresponsetypedef).

<a id="list\_identities"></a>

### list_identities

Lists the identities in an identity pool.

Type annotations for
`session.create_client("cognito-identity").list_identities` method.

Boto3 documentation:
[CognitoIdentity.Client.list_identities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.list_identities)

Asynchronous method. Use `await list_identities(...)` for a synchronous call.

Arguments mapping described in
[ListIdentitiesInputRequestTypeDef](./type_defs.md#listidentitiesinputrequesttypedef).

Keyword-only arguments:

- `IdentityPoolId`: `str` *(required)*
- `MaxResults`: `int` *(required)*
- `NextToken`: `str`
- `HideDisabled`: `bool`

Returns a `Coroutine` for
[ListIdentitiesResponseTypeDef](./type_defs.md#listidentitiesresponsetypedef).

<a id="list\_identity\_pools"></a>

### list_identity_pools

Lists all of the Cognito identity pools registered for your account.

Type annotations for
`session.create_client("cognito-identity").list_identity_pools` method.

Boto3 documentation:
[CognitoIdentity.Client.list_identity_pools](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.list_identity_pools)

Asynchronous method. Use `await list_identity_pools(...)` for a synchronous
call.

Arguments mapping described in
[ListIdentityPoolsInputRequestTypeDef](./type_defs.md#listidentitypoolsinputrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int` *(required)*
- `NextToken`: `str`

Returns a `Coroutine` for
[ListIdentityPoolsResponseTypeDef](./type_defs.md#listidentitypoolsresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Lists the tags that are assigned to an Amazon Cognito identity pool.

Type annotations for
`session.create_client("cognito-identity").list_tags_for_resource` method.

Boto3 documentation:
[CognitoIdentity.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="lookup\_developer\_identity"></a>

### lookup_developer_identity

Retrieves the `IdentityID` associated with a `DeveloperUserIdentifier` or the
list of `DeveloperUserIdentifier` values associated with an `IdentityId` for an
existing identity.

Type annotations for
`session.create_client("cognito-identity").lookup_developer_identity` method.

Boto3 documentation:
[CognitoIdentity.Client.lookup_developer_identity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.lookup_developer_identity)

Asynchronous method. Use `await lookup_developer_identity(...)` for a
synchronous call.

Arguments mapping described in
[LookupDeveloperIdentityInputRequestTypeDef](./type_defs.md#lookupdeveloperidentityinputrequesttypedef).

Keyword-only arguments:

- `IdentityPoolId`: `str` *(required)*
- `IdentityId`: `str`
- `DeveloperUserIdentifier`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[LookupDeveloperIdentityResponseTypeDef](./type_defs.md#lookupdeveloperidentityresponsetypedef).

<a id="merge\_developer\_identities"></a>

### merge_developer_identities

Merges two users having different `IdentityId` s, existing in the same identity
pool, and identified by the same developer provider.

Type annotations for
`session.create_client("cognito-identity").merge_developer_identities` method.

Boto3 documentation:
[CognitoIdentity.Client.merge_developer_identities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.merge_developer_identities)

Asynchronous method. Use `await merge_developer_identities(...)` for a
synchronous call.

Arguments mapping described in
[MergeDeveloperIdentitiesInputRequestTypeDef](./type_defs.md#mergedeveloperidentitiesinputrequesttypedef).

Keyword-only arguments:

- `SourceUserIdentifier`: `str` *(required)*
- `DestinationUserIdentifier`: `str` *(required)*
- `DeveloperProviderName`: `str` *(required)*
- `IdentityPoolId`: `str` *(required)*

Returns a `Coroutine` for
[MergeDeveloperIdentitiesResponseTypeDef](./type_defs.md#mergedeveloperidentitiesresponsetypedef).

<a id="set\_identity\_pool\_roles"></a>

### set_identity_pool_roles

Sets the roles for an identity pool.

Type annotations for
`session.create_client("cognito-identity").set_identity_pool_roles` method.

Boto3 documentation:
[CognitoIdentity.Client.set_identity_pool_roles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.set_identity_pool_roles)

Asynchronous method. Use `await set_identity_pool_roles(...)` for a synchronous
call.

Arguments mapping described in
[SetIdentityPoolRolesInputRequestTypeDef](./type_defs.md#setidentitypoolrolesinputrequesttypedef).

Keyword-only arguments:

- `IdentityPoolId`: `str` *(required)*
- `Roles`: `Mapping`\[`str`, `str`\] *(required)*
- `RoleMappings`: `Mapping`\[`str`,
  [RoleMappingTypeDef](./type_defs.md#rolemappingtypedef)\]

<a id="set\_principal\_tag\_attribute\_map"></a>

### set_principal_tag_attribute_map

You can use this operation to use default (username and clientID) attribute or
custom attribute mappings.

Type annotations for
`session.create_client("cognito-identity").set_principal_tag_attribute_map`
method.

Boto3 documentation:
[CognitoIdentity.Client.set_principal_tag_attribute_map](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.set_principal_tag_attribute_map)

Asynchronous method. Use `await set_principal_tag_attribute_map(...)` for a
synchronous call.

Arguments mapping described in
[SetPrincipalTagAttributeMapInputRequestTypeDef](./type_defs.md#setprincipaltagattributemapinputrequesttypedef).

Keyword-only arguments:

- `IdentityPoolId`: `str` *(required)*
- `IdentityProviderName`: `str` *(required)*
- `UseDefaults`: `bool`
- `PrincipalTags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[SetPrincipalTagAttributeMapResponseTypeDef](./type_defs.md#setprincipaltagattributemapresponsetypedef).

<a id="tag\_resource"></a>

### tag_resource

Assigns a set of tags to the specified Amazon Cognito identity pool.

Type annotations for `session.create_client("cognito-identity").tag_resource`
method.

Boto3 documentation:
[CognitoIdentity.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="unlink\_developer\_identity"></a>

### unlink_developer_identity

Unlinks a `DeveloperUserIdentifier` from an existing identity.

Type annotations for
`session.create_client("cognito-identity").unlink_developer_identity` method.

Boto3 documentation:
[CognitoIdentity.Client.unlink_developer_identity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.unlink_developer_identity)

Asynchronous method. Use `await unlink_developer_identity(...)` for a
synchronous call.

Arguments mapping described in
[UnlinkDeveloperIdentityInputRequestTypeDef](./type_defs.md#unlinkdeveloperidentityinputrequesttypedef).

Keyword-only arguments:

- `IdentityId`: `str` *(required)*
- `IdentityPoolId`: `str` *(required)*
- `DeveloperProviderName`: `str` *(required)*
- `DeveloperUserIdentifier`: `str` *(required)*

<a id="unlink\_identity"></a>

### unlink_identity

Unlinks a federated identity from an existing account.

Type annotations for
`session.create_client("cognito-identity").unlink_identity` method.

Boto3 documentation:
[CognitoIdentity.Client.unlink_identity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.unlink_identity)

Asynchronous method. Use `await unlink_identity(...)` for a synchronous call.

Arguments mapping described in
[UnlinkIdentityInputRequestTypeDef](./type_defs.md#unlinkidentityinputrequesttypedef).

Keyword-only arguments:

- `IdentityId`: `str` *(required)*
- `Logins`: `Mapping`\[`str`, `str`\] *(required)*
- `LoginsToRemove`: `Sequence`\[`str`\] *(required)*

<a id="untag\_resource"></a>

### untag_resource

Removes the specified tags from the specified Amazon Cognito identity pool.

Type annotations for `session.create_client("cognito-identity").untag_resource`
method.

Boto3 documentation:
[CognitoIdentity.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_identity\_pool"></a>

### update_identity_pool

Updates an identity pool.

Type annotations for
`session.create_client("cognito-identity").update_identity_pool` method.

Boto3 documentation:
[CognitoIdentity.Client.update_identity_pool](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.update_identity_pool)

Asynchronous method. Use `await update_identity_pool(...)` for a synchronous
call.

Arguments mapping described in
[IdentityPoolRequestTypeDef](./type_defs.md#identitypoolrequesttypedef).

Keyword-only arguments:

- `IdentityPoolId`: `str` *(required)*
- `IdentityPoolName`: `str` *(required)*
- `AllowUnauthenticatedIdentities`: `bool` *(required)*
- `AllowClassicFlow`: `bool`
- `SupportedLoginProviders`: `Mapping`\[`str`, `str`\]
- `DeveloperProviderName`: `str`
- `OpenIdConnectProviderARNs`: `Sequence`\[`str`\]
- `CognitoIdentityProviders`:
  `Sequence`\[[CognitoIdentityProviderTypeDef](./type_defs.md#cognitoidentityprovidertypedef)\]
- `SamlProviderARNs`: `Sequence`\[`str`\]
- `IdentityPoolTags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[IdentityPoolTypeDef](./type_defs.md#identitypooltypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("cognito-identity").__aenter__`
method.

Boto3 documentation:
[CognitoIdentity.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [CognitoIdentityClient](#cognitoidentityclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("cognito-identity").__aexit__`
method.

Boto3 documentation:
[CognitoIdentity.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("cognito-identity").get_paginator`
method with overloads.

- `client.get_paginator("list_identity_pools")` ->
  [ListIdentityPoolsPaginator](./paginators.md#listidentitypoolspaginator)
