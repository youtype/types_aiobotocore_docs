# LicenseManagerUserSubscriptions module

> [Index](../README.md) > LicenseManagerUserSubscriptions


!!! note ""

    Auto-generated documentation for [LicenseManagerUserSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#licensemanagerusersubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-user-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
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
- [DeleteLicenseServerEndpointRequestTypeDef](./type_defs.md#deletelicenseserverendpointrequesttypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [SettingsOutputTypeDef](./type_defs.md#settingsoutputtypedef)
- [InstanceSummaryTypeDef](./type_defs.md#instancesummarytypedef)
- [LicenseServerTypeDef](./type_defs.md#licenseservertypedef)
- [ServerEndpointTypeDef](./type_defs.md#serverendpointtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [SettingsTypeDef](./type_defs.md#settingstypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateSettingsTypeDef](./type_defs.md#updatesettingstypedef)
- [CreateLicenseServerEndpointResponseTypeDef](./type_defs.md#createlicenseserverendpointresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CredentialsProviderTypeDef](./type_defs.md#credentialsprovidertypedef)
- [ListIdentityProvidersRequestTypeDef](./type_defs.md#listidentityprovidersrequesttypedef)
- [ListInstancesRequestTypeDef](./type_defs.md#listinstancesrequesttypedef)
- [ListLicenseServerEndpointsRequestTypeDef](./type_defs.md#listlicenseserverendpointsrequesttypedef)
- [ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef)
- [LicenseServerEndpointTypeDef](./type_defs.md#licenseserverendpointtypedef)
- [ListIdentityProvidersRequestPaginateTypeDef](./type_defs.md#listidentityprovidersrequestpaginatetypedef)
- [ListInstancesRequestPaginateTypeDef](./type_defs.md#listinstancesrequestpaginatetypedef)
- [ListLicenseServerEndpointsRequestPaginateTypeDef](./type_defs.md#listlicenseserverendpointsrequestpaginatetypedef)
- [SettingsUnionTypeDef](./type_defs.md#settingsuniontypedef)
- [ActiveDirectorySettingsOutputTypeDef](./type_defs.md#activedirectorysettingsoutputtypedef)
- [ActiveDirectorySettingsTypeDef](./type_defs.md#activedirectorysettingstypedef)
- [RdsSalSettingsTypeDef](./type_defs.md#rdssalsettingstypedef)
- [DeleteLicenseServerEndpointResponseTypeDef](./type_defs.md#deletelicenseserverendpointresponsetypedef)
- [ListLicenseServerEndpointsResponseTypeDef](./type_defs.md#listlicenseserverendpointsresponsetypedef)
- [ActiveDirectoryIdentityProviderOutputTypeDef](./type_defs.md#activedirectoryidentityprovideroutputtypedef)
- [ActiveDirectoryIdentityProviderTypeDef](./type_defs.md#activedirectoryidentityprovidertypedef)
- [ServerSettingsTypeDef](./type_defs.md#serversettingstypedef)
- [IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef)
- [IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef)
- [LicenseServerSettingsTypeDef](./type_defs.md#licenseserversettingstypedef)
- [IdentityProviderSummaryTypeDef](./type_defs.md#identityprovidersummarytypedef)
- [InstanceUserSummaryTypeDef](./type_defs.md#instanceusersummarytypedef)
- [ProductUserSummaryTypeDef](./type_defs.md#productusersummarytypedef)
- [IdentityProviderUnionTypeDef](./type_defs.md#identityprovideruniontypedef)
- [CreateLicenseServerEndpointRequestTypeDef](./type_defs.md#createlicenseserverendpointrequesttypedef)
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
- [AssociateUserRequestTypeDef](./type_defs.md#associateuserrequesttypedef)
- [DeregisterIdentityProviderRequestTypeDef](./type_defs.md#deregisteridentityproviderrequesttypedef)
- [DisassociateUserRequestTypeDef](./type_defs.md#disassociateuserrequesttypedef)
- [ListProductSubscriptionsRequestPaginateTypeDef](./type_defs.md#listproductsubscriptionsrequestpaginatetypedef)
- [ListProductSubscriptionsRequestTypeDef](./type_defs.md#listproductsubscriptionsrequesttypedef)
- [ListUserAssociationsRequestPaginateTypeDef](./type_defs.md#listuserassociationsrequestpaginatetypedef)
- [ListUserAssociationsRequestTypeDef](./type_defs.md#listuserassociationsrequesttypedef)
- [RegisterIdentityProviderRequestTypeDef](./type_defs.md#registeridentityproviderrequesttypedef)
- [StartProductSubscriptionRequestTypeDef](./type_defs.md#startproductsubscriptionrequesttypedef)
- [StopProductSubscriptionRequestTypeDef](./type_defs.md#stopproductsubscriptionrequesttypedef)
- [UpdateIdentityProviderSettingsRequestTypeDef](./type_defs.md#updateidentityprovidersettingsrequesttypedef)

