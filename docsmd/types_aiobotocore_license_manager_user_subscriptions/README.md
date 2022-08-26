# LicenseManagerUserSubscriptions module

> [Index](../README.md) > LicenseManagerUserSubscriptions


!!! note ""

    Auto-generated documentation for [LicenseManagerUserSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-user-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions/).

## How to install



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

```python title="Usage example"
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

```python title="Usage example"
from types_aiobotocore_license_manager_user_subscriptions.paginator import ListIdentityProvidersPaginator

def get_list_identity_providers_paginator() -> ListIdentityProvidersPaginator:
    return client.get_paginator("list_identity_providers"))
```

- [ListIdentityProvidersPaginator](./paginators.md#listidentityproviderspaginator)
- [ListInstancesPaginator](./paginators.md#listinstancespaginator)
- [ListProductSubscriptionsPaginator](./paginators.md#listproductsubscriptionspaginator)
- [ListUserAssociationsPaginator](./paginators.md#listuserassociationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_license_manager_user_subscriptions.literals import ListIdentityProvidersPaginatorName

def get_value() -> ListIdentityProvidersPaginatorName:
    return "list_identity_providers"
```

- [ListIdentityProvidersPaginatorName](./literals.md#listidentityproviderspaginatorname)
- [ListInstancesPaginatorName](./literals.md#listinstancespaginatorname)
- [ListProductSubscriptionsPaginatorName](./literals.md#listproductsubscriptionspaginatorname)
- [ListUserAssociationsPaginatorName](./literals.md#listuserassociationspaginatorname)
- [LicenseManagerUserSubscriptionsServiceName](./literals.md#licensemanagerusersubscriptionsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderTypeDef

def get_value() -> ActiveDirectoryIdentityProviderTypeDef:
    return {
        "DirectoryId": ...,
    }
```

- [ActiveDirectoryIdentityProviderTypeDef](./type_defs.md#activedirectoryidentityprovidertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [InstanceSummaryTypeDef](./type_defs.md#instancesummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListIdentityProvidersRequestRequestTypeDef](./type_defs.md#listidentityprovidersrequestrequesttypedef)
- [IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef)
- [ListInstancesRequestRequestTypeDef](./type_defs.md#listinstancesrequestrequesttypedef)
- [ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef)
- [ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef](./type_defs.md#listidentityprovidersrequestlistidentityproviderspaginatetypedef)
- [ListInstancesRequestListInstancesPaginateTypeDef](./type_defs.md#listinstancesrequestlistinstancespaginatetypedef)
- [AssociateUserRequestRequestTypeDef](./type_defs.md#associateuserrequestrequesttypedef)
- [DeregisterIdentityProviderRequestRequestTypeDef](./type_defs.md#deregisteridentityproviderrequestrequesttypedef)
- [DisassociateUserRequestRequestTypeDef](./type_defs.md#disassociateuserrequestrequesttypedef)
- [IdentityProviderSummaryTypeDef](./type_defs.md#identityprovidersummarytypedef)
- [InstanceUserSummaryTypeDef](./type_defs.md#instanceusersummarytypedef)
- [ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef](./type_defs.md#listproductsubscriptionsrequestlistproductsubscriptionspaginatetypedef)
- [ListProductSubscriptionsRequestRequestTypeDef](./type_defs.md#listproductsubscriptionsrequestrequesttypedef)
- [ListUserAssociationsRequestListUserAssociationsPaginateTypeDef](./type_defs.md#listuserassociationsrequestlistuserassociationspaginatetypedef)
- [ListUserAssociationsRequestRequestTypeDef](./type_defs.md#listuserassociationsrequestrequesttypedef)
- [ProductUserSummaryTypeDef](./type_defs.md#productusersummarytypedef)
- [RegisterIdentityProviderRequestRequestTypeDef](./type_defs.md#registeridentityproviderrequestrequesttypedef)
- [StartProductSubscriptionRequestRequestTypeDef](./type_defs.md#startproductsubscriptionrequestrequesttypedef)
- [StopProductSubscriptionRequestRequestTypeDef](./type_defs.md#stopproductsubscriptionrequestrequesttypedef)
- [DeregisterIdentityProviderResponseTypeDef](./type_defs.md#deregisteridentityproviderresponsetypedef)
- [ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef)
- [RegisterIdentityProviderResponseTypeDef](./type_defs.md#registeridentityproviderresponsetypedef)
- [AssociateUserResponseTypeDef](./type_defs.md#associateuserresponsetypedef)
- [DisassociateUserResponseTypeDef](./type_defs.md#disassociateuserresponsetypedef)
- [ListUserAssociationsResponseTypeDef](./type_defs.md#listuserassociationsresponsetypedef)
- [ListProductSubscriptionsResponseTypeDef](./type_defs.md#listproductsubscriptionsresponsetypedef)
- [StartProductSubscriptionResponseTypeDef](./type_defs.md#startproductsubscriptionresponsetypedef)
- [StopProductSubscriptionResponseTypeDef](./type_defs.md#stopproductsubscriptionresponsetypedef)

