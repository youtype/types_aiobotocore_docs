<a id="worklinkclient-for-aiobotocore-worklink-module"></a>

# WorkLinkClient for aiobotocore WorkLink module

> [Index](..) > [WorkLink](.) > WorkLinkClient

Auto-generated documentation for
[WorkLink](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
type annotations stubs module
[types-aiobotocore-worklink](https://pypi.org/project/types-aiobotocore-worklink/).

- [WorkLinkClient for aiobotocore WorkLink module](#worklinkclient-for-aiobotocore-worklink-module)
  - [WorkLinkClient](#worklinkclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [associate_domain](#associate_domain)
    - [associate_website_authorization_provider](#associate_website_authorization_provider)
    - [associate_website_certificate_authority](#associate_website_certificate_authority)
    - [can_paginate](#can_paginate)
    - [create_fleet](#create_fleet)
    - [delete_fleet](#delete_fleet)
    - [describe_audit_stream_configuration](#describe_audit_stream_configuration)
    - [describe_company_network_configuration](#describe_company_network_configuration)
    - [describe_device](#describe_device)
    - [describe_device_policy_configuration](#describe_device_policy_configuration)
    - [describe_domain](#describe_domain)
    - [describe_fleet_metadata](#describe_fleet_metadata)
    - [describe_identity_provider_configuration](#describe_identity_provider_configuration)
    - [describe_website_certificate_authority](#describe_website_certificate_authority)
    - [disassociate_domain](#disassociate_domain)
    - [disassociate_website_authorization_provider](#disassociate_website_authorization_provider)
    - [disassociate_website_certificate_authority](#disassociate_website_certificate_authority)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_devices](#list_devices)
    - [list_domains](#list_domains)
    - [list_fleets](#list_fleets)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_website_authorization_providers](#list_website_authorization_providers)
    - [list_website_certificate_authorities](#list_website_certificate_authorities)
    - [restore_domain_access](#restore_domain_access)
    - [revoke_domain_access](#revoke_domain_access)
    - [sign_out_user](#sign_out_user)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_audit_stream_configuration](#update_audit_stream_configuration)
    - [update_company_network_configuration](#update_company_network_configuration)
    - [update_device_policy_configuration](#update_device_policy_configuration)
    - [update_domain_metadata](#update_domain_metadata)
    - [update_fleet_metadata](#update_fleet_metadata)
    - [update_identity_provider_configuration](#update_identity_provider_configuration)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)

<a id="worklinkclient"></a>

## WorkLinkClient

Type annotations for `session.create_client("worklink")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_worklink.client import WorkLinkClient

session = get_session()
async with session.create_client("worklink") as client:
    client: WorkLinkClient
```

Boto3 documentation:
[WorkLink.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_worklink.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InternalServerErrorException`
- `Exceptions.InvalidRequestException`
- `Exceptions.ResourceAlreadyExistsException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.TooManyRequestsException`
- `Exceptions.UnauthorizedException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

WorkLinkClient exceptions.

Type annotations for `session.create_client("worklink").exceptions` method.

Boto3 documentation:
[WorkLink.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="associate_domain"></a>

### associate_domain

Specifies a domain to be associated to Amazon WorkLink.

Type annotations for `session.create_client("worklink").associate_domain`
method.

Boto3 documentation:
[WorkLink.Client.associate_domain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.associate_domain)

Asynchronous method. Use `await associate_domain(...)` for a synchronous call.

Arguments mapping described in
[AssociateDomainRequestRequestTypeDef](./type_defs.md#associatedomainrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `DomainName`: `str` *(required)*
- `AcmCertificateArn`: `str` *(required)*
- `DisplayName`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="associate_website_authorization_provider"></a>

### associate_website_authorization_provider

Associates a website authorization provider with a specified fleet.

Type annotations for
`session.create_client("worklink").associate_website_authorization_provider`
method.

Boto3 documentation:
[WorkLink.Client.associate_website_authorization_provider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.associate_website_authorization_provider)

Asynchronous method. Use `await associate_website_authorization_provider(...)`
for a synchronous call.

Arguments mapping described in
[AssociateWebsiteAuthorizationProviderRequestRequestTypeDef](./type_defs.md#associatewebsiteauthorizationproviderrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `AuthorizationProviderType`: `Literal['SAML']` (see
  [AuthorizationProviderTypeType](./literals.md#authorizationprovidertypetype))
  *(required)*
- `DomainName`: `str`

Returns a `Coroutine` for
[AssociateWebsiteAuthorizationProviderResponseTypeDef](./type_defs.md#associatewebsiteauthorizationproviderresponsetypedef).

<a id="associate_website_certificate_authority"></a>

### associate_website_certificate_authority

Imports the root certificate of a certificate authority (CA) used to obtain TLS
certificates used by associated websites within the company network.

Type annotations for
`session.create_client("worklink").associate_website_certificate_authority`
method.

Boto3 documentation:
[WorkLink.Client.associate_website_certificate_authority](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.associate_website_certificate_authority)

Asynchronous method. Use `await associate_website_certificate_authority(...)`
for a synchronous call.

Arguments mapping described in
[AssociateWebsiteCertificateAuthorityRequestRequestTypeDef](./type_defs.md#associatewebsitecertificateauthorityrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `Certificate`: `str` *(required)*
- `DisplayName`: `str`

Returns a `Coroutine` for
[AssociateWebsiteCertificateAuthorityResponseTypeDef](./type_defs.md#associatewebsitecertificateauthorityresponsetypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("worklink").can_paginate` method.

Boto3 documentation:
[WorkLink.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_fleet"></a>

### create_fleet

Creates a fleet.

Type annotations for `session.create_client("worklink").create_fleet` method.

Boto3 documentation:
[WorkLink.Client.create_fleet](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.create_fleet)

Asynchronous method. Use `await create_fleet(...)` for a synchronous call.

Arguments mapping described in
[CreateFleetRequestRequestTypeDef](./type_defs.md#createfleetrequestrequesttypedef).

Keyword-only arguments:

- `FleetName`: `str` *(required)*
- `DisplayName`: `str`
- `OptimizeForEndUserLocation`: `bool`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateFleetResponseTypeDef](./type_defs.md#createfleetresponsetypedef).

<a id="delete_fleet"></a>

### delete_fleet

Deletes a fleet.

Type annotations for `session.create_client("worklink").delete_fleet` method.

Boto3 documentation:
[WorkLink.Client.delete_fleet](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.delete_fleet)

Asynchronous method. Use `await delete_fleet(...)` for a synchronous call.

Arguments mapping described in
[DeleteFleetRequestRequestTypeDef](./type_defs.md#deletefleetrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_audit_stream_configuration"></a>

### describe_audit_stream_configuration

Describes the configuration for delivering audit streams to the customer
account.

Type annotations for
`session.create_client("worklink").describe_audit_stream_configuration` method.

Boto3 documentation:
[WorkLink.Client.describe_audit_stream_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.describe_audit_stream_configuration)

Asynchronous method. Use `await describe_audit_stream_configuration(...)` for a
synchronous call.

Arguments mapping described in
[DescribeAuditStreamConfigurationRequestRequestTypeDef](./type_defs.md#describeauditstreamconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAuditStreamConfigurationResponseTypeDef](./type_defs.md#describeauditstreamconfigurationresponsetypedef).

<a id="describe_company_network_configuration"></a>

### describe_company_network_configuration

Describes the networking configuration to access the internal websites
associated with the specified fleet.

Type annotations for
`session.create_client("worklink").describe_company_network_configuration`
method.

Boto3 documentation:
[WorkLink.Client.describe_company_network_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.describe_company_network_configuration)

Asynchronous method. Use `await describe_company_network_configuration(...)`
for a synchronous call.

Arguments mapping described in
[DescribeCompanyNetworkConfigurationRequestRequestTypeDef](./type_defs.md#describecompanynetworkconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeCompanyNetworkConfigurationResponseTypeDef](./type_defs.md#describecompanynetworkconfigurationresponsetypedef).

<a id="describe_device"></a>

### describe_device

Provides information about a user's device.

Type annotations for `session.create_client("worklink").describe_device`
method.

Boto3 documentation:
[WorkLink.Client.describe_device](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.describe_device)

Asynchronous method. Use `await describe_device(...)` for a synchronous call.

Arguments mapping described in
[DescribeDeviceRequestRequestTypeDef](./type_defs.md#describedevicerequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `DeviceId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDeviceResponseTypeDef](./type_defs.md#describedeviceresponsetypedef).

<a id="describe_device_policy_configuration"></a>

### describe_device_policy_configuration

Describes the device policy configuration for the specified fleet.

Type annotations for
`session.create_client("worklink").describe_device_policy_configuration`
method.

Boto3 documentation:
[WorkLink.Client.describe_device_policy_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.describe_device_policy_configuration)

Asynchronous method. Use `await describe_device_policy_configuration(...)` for
a synchronous call.

Arguments mapping described in
[DescribeDevicePolicyConfigurationRequestRequestTypeDef](./type_defs.md#describedevicepolicyconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDevicePolicyConfigurationResponseTypeDef](./type_defs.md#describedevicepolicyconfigurationresponsetypedef).

<a id="describe_domain"></a>

### describe_domain

Provides information about the domain.

Type annotations for `session.create_client("worklink").describe_domain`
method.

Boto3 documentation:
[WorkLink.Client.describe_domain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.describe_domain)

Asynchronous method. Use `await describe_domain(...)` for a synchronous call.

Arguments mapping described in
[DescribeDomainRequestRequestTypeDef](./type_defs.md#describedomainrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `DomainName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDomainResponseTypeDef](./type_defs.md#describedomainresponsetypedef).

<a id="describe_fleet_metadata"></a>

### describe_fleet_metadata

Provides basic information for the specified fleet, excluding identity
provider, networking, and device configuration details.

Type annotations for
`session.create_client("worklink").describe_fleet_metadata` method.

Boto3 documentation:
[WorkLink.Client.describe_fleet_metadata](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.describe_fleet_metadata)

Asynchronous method. Use `await describe_fleet_metadata(...)` for a synchronous
call.

Arguments mapping described in
[DescribeFleetMetadataRequestRequestTypeDef](./type_defs.md#describefleetmetadatarequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeFleetMetadataResponseTypeDef](./type_defs.md#describefleetmetadataresponsetypedef).

<a id="describe_identity_provider_configuration"></a>

### describe_identity_provider_configuration

Describes the identity provider configuration of the specified fleet.

Type annotations for
`session.create_client("worklink").describe_identity_provider_configuration`
method.

Boto3 documentation:
[WorkLink.Client.describe_identity_provider_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.describe_identity_provider_configuration)

Asynchronous method. Use `await describe_identity_provider_configuration(...)`
for a synchronous call.

Arguments mapping described in
[DescribeIdentityProviderConfigurationRequestRequestTypeDef](./type_defs.md#describeidentityproviderconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeIdentityProviderConfigurationResponseTypeDef](./type_defs.md#describeidentityproviderconfigurationresponsetypedef).

<a id="describe_website_certificate_authority"></a>

### describe_website_certificate_authority

Provides information about the certificate authority.

Type annotations for
`session.create_client("worklink").describe_website_certificate_authority`
method.

Boto3 documentation:
[WorkLink.Client.describe_website_certificate_authority](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.describe_website_certificate_authority)

Asynchronous method. Use `await describe_website_certificate_authority(...)`
for a synchronous call.

Arguments mapping described in
[DescribeWebsiteCertificateAuthorityRequestRequestTypeDef](./type_defs.md#describewebsitecertificateauthorityrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `WebsiteCaId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeWebsiteCertificateAuthorityResponseTypeDef](./type_defs.md#describewebsitecertificateauthorityresponsetypedef).

<a id="disassociate_domain"></a>

### disassociate_domain

Disassociates a domain from Amazon WorkLink.

Type annotations for `session.create_client("worklink").disassociate_domain`
method.

Boto3 documentation:
[WorkLink.Client.disassociate_domain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.disassociate_domain)

Asynchronous method. Use `await disassociate_domain(...)` for a synchronous
call.

Arguments mapping described in
[DisassociateDomainRequestRequestTypeDef](./type_defs.md#disassociatedomainrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `DomainName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate_website_authorization_provider"></a>

### disassociate_website_authorization_provider

Disassociates a website authorization provider from a specified fleet.

Type annotations for
`session.create_client("worklink").disassociate_website_authorization_provider`
method.

Boto3 documentation:
[WorkLink.Client.disassociate_website_authorization_provider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.disassociate_website_authorization_provider)

Asynchronous method. Use
`await disassociate_website_authorization_provider(...)` for a synchronous
call.

Arguments mapping described in
[DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef](./type_defs.md#disassociatewebsiteauthorizationproviderrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `AuthorizationProviderId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate_website_certificate_authority"></a>

### disassociate_website_certificate_authority

Removes a certificate authority (CA).

Type annotations for
`session.create_client("worklink").disassociate_website_certificate_authority`
method.

Boto3 documentation:
[WorkLink.Client.disassociate_website_certificate_authority](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.disassociate_website_certificate_authority)

Asynchronous method. Use
`await disassociate_website_certificate_authority(...)` for a synchronous call.

Arguments mapping described in
[DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef](./type_defs.md#disassociatewebsitecertificateauthorityrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `WebsiteCaId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("worklink").generate_presigned_url`
method.

Boto3 documentation:
[WorkLink.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_devices"></a>

### list_devices

Retrieves a list of devices registered with the specified fleet.

Type annotations for `session.create_client("worklink").list_devices` method.

Boto3 documentation:
[WorkLink.Client.list_devices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.list_devices)

Asynchronous method. Use `await list_devices(...)` for a synchronous call.

Arguments mapping described in
[ListDevicesRequestRequestTypeDef](./type_defs.md#listdevicesrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef).

<a id="list_domains"></a>

### list_domains

Retrieves a list of domains associated to a specified fleet.

Type annotations for `session.create_client("worklink").list_domains` method.

Boto3 documentation:
[WorkLink.Client.list_domains](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.list_domains)

Asynchronous method. Use `await list_domains(...)` for a synchronous call.

Arguments mapping described in
[ListDomainsRequestRequestTypeDef](./type_defs.md#listdomainsrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef).

<a id="list_fleets"></a>

### list_fleets

Retrieves a list of fleets for the current account and Region.

Type annotations for `session.create_client("worklink").list_fleets` method.

Boto3 documentation:
[WorkLink.Client.list_fleets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.list_fleets)

Asynchronous method. Use `await list_fleets(...)` for a synchronous call.

Arguments mapping described in
[ListFleetsRequestRequestTypeDef](./type_defs.md#listfleetsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListFleetsResponseTypeDef](./type_defs.md#listfleetsresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Retrieves a list of tags for the specified resource.

Type annotations for `session.create_client("worklink").list_tags_for_resource`
method.

Boto3 documentation:
[WorkLink.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="list_website_authorization_providers"></a>

### list_website_authorization_providers

Retrieves a list of website authorization providers associated with a specified
fleet.

Type annotations for
`session.create_client("worklink").list_website_authorization_providers`
method.

Boto3 documentation:
[WorkLink.Client.list_website_authorization_providers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.list_website_authorization_providers)

Asynchronous method. Use `await list_website_authorization_providers(...)` for
a synchronous call.

Arguments mapping described in
[ListWebsiteAuthorizationProvidersRequestRequestTypeDef](./type_defs.md#listwebsiteauthorizationprovidersrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListWebsiteAuthorizationProvidersResponseTypeDef](./type_defs.md#listwebsiteauthorizationprovidersresponsetypedef).

<a id="list_website_certificate_authorities"></a>

### list_website_certificate_authorities

Retrieves a list of certificate authorities added for the current account and
Region.

Type annotations for
`session.create_client("worklink").list_website_certificate_authorities`
method.

Boto3 documentation:
[WorkLink.Client.list_website_certificate_authorities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.list_website_certificate_authorities)

Asynchronous method. Use `await list_website_certificate_authorities(...)` for
a synchronous call.

Arguments mapping described in
[ListWebsiteCertificateAuthoritiesRequestRequestTypeDef](./type_defs.md#listwebsitecertificateauthoritiesrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListWebsiteCertificateAuthoritiesResponseTypeDef](./type_defs.md#listwebsitecertificateauthoritiesresponsetypedef).

<a id="restore_domain_access"></a>

### restore_domain_access

Moves a domain to ACTIVE status if it was in the INACTIVE status.

Type annotations for `session.create_client("worklink").restore_domain_access`
method.

Boto3 documentation:
[WorkLink.Client.restore_domain_access](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.restore_domain_access)

Asynchronous method. Use `await restore_domain_access(...)` for a synchronous
call.

Arguments mapping described in
[RestoreDomainAccessRequestRequestTypeDef](./type_defs.md#restoredomainaccessrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `DomainName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="revoke_domain_access"></a>

### revoke_domain_access

Moves a domain to INACTIVE status if it was in the ACTIVE status.

Type annotations for `session.create_client("worklink").revoke_domain_access`
method.

Boto3 documentation:
[WorkLink.Client.revoke_domain_access](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.revoke_domain_access)

Asynchronous method. Use `await revoke_domain_access(...)` for a synchronous
call.

Arguments mapping described in
[RevokeDomainAccessRequestRequestTypeDef](./type_defs.md#revokedomainaccessrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `DomainName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="sign_out_user"></a>

### sign_out_user

Signs the user out from all of their devices.

Type annotations for `session.create_client("worklink").sign_out_user` method.

Boto3 documentation:
[WorkLink.Client.sign_out_user](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.sign_out_user)

Asynchronous method. Use `await sign_out_user(...)` for a synchronous call.

Arguments mapping described in
[SignOutUserRequestRequestTypeDef](./type_defs.md#signoutuserrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `Username`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="tag_resource"></a>

### tag_resource

Adds or overwrites one or more tags for the specified resource, such as a
fleet.

Type annotations for `session.create_client("worklink").tag_resource` method.

Boto3 documentation:
[WorkLink.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes one or more tags from the specified resource.

Type annotations for `session.create_client("worklink").untag_resource` method.

Boto3 documentation:
[WorkLink.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_audit_stream_configuration"></a>

### update_audit_stream_configuration

Updates the audit stream configuration for the fleet.

Type annotations for
`session.create_client("worklink").update_audit_stream_configuration` method.

Boto3 documentation:
[WorkLink.Client.update_audit_stream_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.update_audit_stream_configuration)

Asynchronous method. Use `await update_audit_stream_configuration(...)` for a
synchronous call.

Arguments mapping described in
[UpdateAuditStreamConfigurationRequestRequestTypeDef](./type_defs.md#updateauditstreamconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `AuditStreamArn`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_company_network_configuration"></a>

### update_company_network_configuration

Updates the company network configuration for the fleet.

Type annotations for
`session.create_client("worklink").update_company_network_configuration`
method.

Boto3 documentation:
[WorkLink.Client.update_company_network_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.update_company_network_configuration)

Asynchronous method. Use `await update_company_network_configuration(...)` for
a synchronous call.

Arguments mapping described in
[UpdateCompanyNetworkConfigurationRequestRequestTypeDef](./type_defs.md#updatecompanynetworkconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `VpcId`: `str` *(required)*
- `SubnetIds`: `Sequence`\[`str`\] *(required)*
- `SecurityGroupIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_device_policy_configuration"></a>

### update_device_policy_configuration

Updates the device policy configuration for the fleet.

Type annotations for
`session.create_client("worklink").update_device_policy_configuration` method.

Boto3 documentation:
[WorkLink.Client.update_device_policy_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.update_device_policy_configuration)

Asynchronous method. Use `await update_device_policy_configuration(...)` for a
synchronous call.

Arguments mapping described in
[UpdateDevicePolicyConfigurationRequestRequestTypeDef](./type_defs.md#updatedevicepolicyconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `DeviceCaCertificate`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_domain_metadata"></a>

### update_domain_metadata

Updates domain metadata, such as DisplayName.

Type annotations for `session.create_client("worklink").update_domain_metadata`
method.

Boto3 documentation:
[WorkLink.Client.update_domain_metadata](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.update_domain_metadata)

Asynchronous method. Use `await update_domain_metadata(...)` for a synchronous
call.

Arguments mapping described in
[UpdateDomainMetadataRequestRequestTypeDef](./type_defs.md#updatedomainmetadatarequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `DomainName`: `str` *(required)*
- `DisplayName`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_fleet_metadata"></a>

### update_fleet_metadata

Updates fleet metadata, such as DisplayName.

Type annotations for `session.create_client("worklink").update_fleet_metadata`
method.

Boto3 documentation:
[WorkLink.Client.update_fleet_metadata](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.update_fleet_metadata)

Asynchronous method. Use `await update_fleet_metadata(...)` for a synchronous
call.

Arguments mapping described in
[UpdateFleetMetadataRequestRequestTypeDef](./type_defs.md#updatefleetmetadatarequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `DisplayName`: `str`
- `OptimizeForEndUserLocation`: `bool`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_identity_provider_configuration"></a>

### update_identity_provider_configuration

Updates the identity provider configuration for the fleet.

Type annotations for
`session.create_client("worklink").update_identity_provider_configuration`
method.

Boto3 documentation:
[WorkLink.Client.update_identity_provider_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.update_identity_provider_configuration)

Asynchronous method. Use `await update_identity_provider_configuration(...)`
for a synchronous call.

Arguments mapping described in
[UpdateIdentityProviderConfigurationRequestRequestTypeDef](./type_defs.md#updateidentityproviderconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `FleetArn`: `str` *(required)*
- `IdentityProviderType`: `Literal['SAML']` (see
  [IdentityProviderTypeType](./literals.md#identityprovidertypetype))
  *(required)*
- `IdentityProviderSamlMetadata`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("worklink").__aenter__` method.

Boto3 documentation:
[WorkLink.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [WorkLinkClient](#worklinkclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("worklink").__aexit__` method.

Boto3 documentation:
[WorkLink.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
