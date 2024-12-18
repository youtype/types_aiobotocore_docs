# LicenseManagerUserSubscriptions module

> [Index](../README.md) > LicenseManagerUserSubscriptions


!!! note ""

    Auto-generated documentation for [LicenseManagerUserSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#licensemanagerusersubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-user-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `LicenseManagerUserSubscriptions` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `LicenseManagerUserSubscriptions` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[license-manager-user-subscriptions]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[license-manager-user-subscriptions]'

# standalone installation
python -m pip install types-aiobotocore-license-manager-user-subscriptions
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-license-manager-user-subscriptions
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LicenseManagerUserSubscriptionsClient

Type annotations and code completion for  `#!python session.create_client("license-manager-user-subscriptions")` as [LicenseManagerUserSubscriptionsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# LicenseManagerUserSubscriptionsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager_user_subscriptions.client import LicenseManagerUserSubscriptionsClient


session = get_session()
async with session.create_client("license-manager-user-subscriptions") as client:
    client: LicenseManagerUserSubscriptionsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("license-manager-user-subscriptions").get_paginator("...")`.

```python
# ListIdentityProvidersPaginator usage example

from types_aiobotocore_license_manager_user_subscriptions.paginator import ListIdentityProvidersPaginator

def get_list_identity_providers_paginator() -> ListIdentityProvidersPaginator:
    return client.get_paginator("list_identity_providers"))
```

- [ListIdentityProvidersPaginator](./paginators.md#listidentityproviderspaginator)
- [ListInstancesPaginator](./paginators.md#listinstancespaginator)
- [ListLicenseServerEndpointsPaginator](./paginators.md#listlicenseserverendpointspaginator)
- [ListProductSubscriptionsPaginator](./paginators.md#listproductsubscriptionspaginator)
- [ListUserAssociationsPaginator](./paginators.md#listuserassociationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActiveDirectoryTypeType usage example

from types_aiobotocore_license_manager_user_subscriptions.literals import ActiveDirectoryTypeType

def get_value() -> ActiveDirectoryTypeType:
    return "AWS_MANAGED"
```

- [ActiveDirectoryTypeType](./literals.md#activedirectorytypetype)
- [LicenseServerEndpointProvisioningStatusType](./literals.md#licenseserverendpointprovisioningstatustype)
- [LicenseServerHealthStatusType](./literals.md#licenseserverhealthstatustype)
- [ListIdentityProvidersPaginatorName](./literals.md#listidentityproviderspaginatorname)
- [ListInstancesPaginatorName](./literals.md#listinstancespaginatorname)
- [ListLicenseServerEndpointsPaginatorName](./literals.md#listlicenseserverendpointspaginatorname)
- [ListProductSubscriptionsPaginatorName](./literals.md#listproductsubscriptionspaginatorname)
- [ListUserAssociationsPaginatorName](./literals.md#listuserassociationspaginatorname)
- [ServerTypeType](./literals.md#servertypetype)
- [LicenseManagerUserSubscriptionsServiceName](./literals.md#licensemanagerusersubscriptionsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [DomainNetworkSettingsOutputTypeDef](./type_defs.md#domainnetworksettingsoutputtypedef)
- [DomainNetworkSettingsTypeDef](./type_defs.md#domainnetworksettingstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SecretsManagerCredentialsProviderTypeDef](./type_defs.md#secretsmanagercredentialsprovidertypedef)
- [DeleteLicenseServerEndpointRequestRequestTypeDef](./type_defs.md#deletelicenseserverendpointrequestrequesttypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [SettingsOutputTypeDef](./type_defs.md#settingsoutputtypedef)
- [InstanceSummaryTypeDef](./type_defs.md#instancesummarytypedef)
- [LicenseServerTypeDef](./type_defs.md#licenseservertypedef)
- [ServerEndpointTypeDef](./type_defs.md#serverendpointtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [SettingsTypeDef](./type_defs.md#settingstypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateSettingsTypeDef](./type_defs.md#updatesettingstypedef)
- [CreateLicenseServerEndpointResponseTypeDef](./type_defs.md#createlicenseserverendpointresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CredentialsProviderTypeDef](./type_defs.md#credentialsprovidertypedef)
- [ListIdentityProvidersRequestRequestTypeDef](./type_defs.md#listidentityprovidersrequestrequesttypedef)
- [ListInstancesRequestRequestTypeDef](./type_defs.md#listinstancesrequestrequesttypedef)
- [ListLicenseServerEndpointsRequestRequestTypeDef](./type_defs.md#listlicenseserverendpointsrequestrequesttypedef)
- [ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef)
- [LicenseServerEndpointTypeDef](./type_defs.md#licenseserverendpointtypedef)
- [ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef](./type_defs.md#listidentityprovidersrequestlistidentityproviderspaginatetypedef)
- [ListInstancesRequestListInstancesPaginateTypeDef](./type_defs.md#listinstancesrequestlistinstancespaginatetypedef)
- [ListLicenseServerEndpointsRequestListLicenseServerEndpointsPaginateTypeDef](./type_defs.md#listlicenseserverendpointsrequestlistlicenseserverendpointspaginatetypedef)
- [ActiveDirectorySettingsOutputTypeDef](./type_defs.md#activedirectorysettingsoutputtypedef)
- [ActiveDirectorySettingsTypeDef](./type_defs.md#activedirectorysettingstypedef)
- [RdsSalSettingsTypeDef](./type_defs.md#rdssalsettingstypedef)
- [DeleteLicenseServerEndpointResponseTypeDef](./type_defs.md#deletelicenseserverendpointresponsetypedef)
- [ListLicenseServerEndpointsResponseTypeDef](./type_defs.md#listlicenseserverendpointsresponsetypedef)
- [ActiveDirectoryIdentityProviderOutputTypeDef](./type_defs.md#activedirectoryidentityprovideroutputtypedef)
- [ActiveDirectoryIdentityProviderTypeDef](./type_defs.md#activedirectoryidentityprovidertypedef)
- [ServerSettingsTypeDef](./type_defs.md#serversettingstypedef)
- [IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef)
- [ActiveDirectoryIdentityProviderUnionTypeDef](./type_defs.md#activedirectoryidentityprovideruniontypedef)
- [LicenseServerSettingsTypeDef](./type_defs.md#licenseserversettingstypedef)
- [IdentityProviderSummaryTypeDef](./type_defs.md#identityprovidersummarytypedef)
- [InstanceUserSummaryTypeDef](./type_defs.md#instanceusersummarytypedef)
- [ProductUserSummaryTypeDef](./type_defs.md#productusersummarytypedef)
- [IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef)
- [CreateLicenseServerEndpointRequestRequestTypeDef](./type_defs.md#createlicenseserverendpointrequestrequesttypedef)
- [DeregisterIdentityProviderResponseTypeDef](./type_defs.md#deregisteridentityproviderresponsetypedef)
- [ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef)
- [RegisterIdentityProviderResponseTypeDef](./type_defs.md#registeridentityproviderresponsetypedef)
- [UpdateIdentityProviderSettingsResponseTypeDef](./type_defs.md#updateidentityprovidersettingsresponsetypedef)
- [AssociateUserResponseTypeDef](./type_defs.md#associateuserresponsetypedef)
- [DisassociateUserResponseTypeDef](./type_defs.md#disassociateuserresponsetypedef)
- [ListUserAssociationsResponseTypeDef](./type_defs.md#listuserassociationsresponsetypedef)
- [ListProductSubscriptionsResponseTypeDef](./type_defs.md#listproductsubscriptionsresponsetypedef)
- [StartProductSubscriptionResponseTypeDef](./type_defs.md#startproductsubscriptionresponsetypedef)
- [StopProductSubscriptionResponseTypeDef](./type_defs.md#stopproductsubscriptionresponsetypedef)
- [AssociateUserRequestRequestTypeDef](./type_defs.md#associateuserrequestrequesttypedef)
- [DeregisterIdentityProviderRequestRequestTypeDef](./type_defs.md#deregisteridentityproviderrequestrequesttypedef)
- [DisassociateUserRequestRequestTypeDef](./type_defs.md#disassociateuserrequestrequesttypedef)
- [ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef](./type_defs.md#listproductsubscriptionsrequestlistproductsubscriptionspaginatetypedef)
- [ListProductSubscriptionsRequestRequestTypeDef](./type_defs.md#listproductsubscriptionsrequestrequesttypedef)
- [ListUserAssociationsRequestListUserAssociationsPaginateTypeDef](./type_defs.md#listuserassociationsrequestlistuserassociationspaginatetypedef)
- [ListUserAssociationsRequestRequestTypeDef](./type_defs.md#listuserassociationsrequestrequesttypedef)
- [RegisterIdentityProviderRequestRequestTypeDef](./type_defs.md#registeridentityproviderrequestrequesttypedef)
- [StartProductSubscriptionRequestRequestTypeDef](./type_defs.md#startproductsubscriptionrequestrequesttypedef)
- [StopProductSubscriptionRequestRequestTypeDef](./type_defs.md#stopproductsubscriptionrequestrequesttypedef)
- [UpdateIdentityProviderSettingsRequestRequestTypeDef](./type_defs.md#updateidentityprovidersettingsrequestrequesttypedef)

