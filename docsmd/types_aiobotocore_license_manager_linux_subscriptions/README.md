# LicenseManagerLinuxSubscriptions module

> [Index](../README.md) > LicenseManagerLinuxSubscriptions


!!! note ""

    Auto-generated documentation for [LicenseManagerLinuxSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#licensemanagerlinuxsubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-linux-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-linux-subscriptions/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `LicenseManagerLinuxSubscriptions` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `LicenseManagerLinuxSubscriptions` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[license-manager-linux-subscriptions]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[license-manager-linux-subscriptions]'

# standalone installation
python -m pip install types-aiobotocore-license-manager-linux-subscriptions
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-license-manager-linux-subscriptions
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LicenseManagerLinuxSubscriptionsClient

Type annotations and code completion for  `#!python session.create_client("license-manager-linux-subscriptions")` as [LicenseManagerLinuxSubscriptionsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client)

```python
# LicenseManagerLinuxSubscriptionsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager_linux_subscriptions.client import LicenseManagerLinuxSubscriptionsClient


session = get_session()
async with session.create_client("license-manager-linux-subscriptions") as client:
    client: LicenseManagerLinuxSubscriptionsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("license-manager-linux-subscriptions").get_paginator("...")`.

```python
# ListLinuxSubscriptionInstancesPaginator usage example

from types_aiobotocore_license_manager_linux_subscriptions.paginator import ListLinuxSubscriptionInstancesPaginator

def get_list_linux_subscription_instances_paginator() -> ListLinuxSubscriptionInstancesPaginator:
    return client.get_paginator("list_linux_subscription_instances"))
```

- [ListLinuxSubscriptionInstancesPaginator](./paginators.md#listlinuxsubscriptioninstancespaginator)
- [ListLinuxSubscriptionsPaginator](./paginators.md#listlinuxsubscriptionspaginator)
- [ListRegisteredSubscriptionProvidersPaginator](./paginators.md#listregisteredsubscriptionproviderspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# LinuxSubscriptionsDiscoveryType usage example

from types_aiobotocore_license_manager_linux_subscriptions.literals import LinuxSubscriptionsDiscoveryType

def get_value() -> LinuxSubscriptionsDiscoveryType:
    return "Disabled"
```

- [LinuxSubscriptionsDiscoveryType](./literals.md#linuxsubscriptionsdiscoverytype)
- [ListLinuxSubscriptionInstancesPaginatorName](./literals.md#listlinuxsubscriptioninstancespaginatorname)
- [ListLinuxSubscriptionsPaginatorName](./literals.md#listlinuxsubscriptionspaginatorname)
- [ListRegisteredSubscriptionProvidersPaginatorName](./literals.md#listregisteredsubscriptionproviderspaginatorname)
- [OperatorType](./literals.md#operatortype)
- [OrganizationIntegrationType](./literals.md#organizationintegrationtype)
- [StatusType](./literals.md#statustype)
- [SubscriptionProviderSourceType](./literals.md#subscriptionprovidersourcetype)
- [SubscriptionProviderStatusType](./literals.md#subscriptionproviderstatustype)
- [LicenseManagerLinuxSubscriptionsServiceName](./literals.md#licensemanagerlinuxsubscriptionsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [DeregisterSubscriptionProviderRequestRequestTypeDef](./type_defs.md#deregistersubscriptionproviderrequestrequesttypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetRegisteredSubscriptionProviderRequestRequestTypeDef](./type_defs.md#getregisteredsubscriptionproviderrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [LinuxSubscriptionsDiscoverySettingsOutputTypeDef](./type_defs.md#linuxsubscriptionsdiscoverysettingsoutputtypedef)
- [InstanceTypeDef](./type_defs.md#instancetypedef)
- [LinuxSubscriptionsDiscoverySettingsTypeDef](./type_defs.md#linuxsubscriptionsdiscoverysettingstypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [SubscriptionTypeDef](./type_defs.md#subscriptiontypedef)
- [ListRegisteredSubscriptionProvidersRequestRequestTypeDef](./type_defs.md#listregisteredsubscriptionprovidersrequestrequesttypedef)
- [RegisteredSubscriptionProviderTypeDef](./type_defs.md#registeredsubscriptionprovidertypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [RegisterSubscriptionProviderRequestRequestTypeDef](./type_defs.md#registersubscriptionproviderrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [ListLinuxSubscriptionInstancesRequestRequestTypeDef](./type_defs.md#listlinuxsubscriptioninstancesrequestrequesttypedef)
- [ListLinuxSubscriptionsRequestRequestTypeDef](./type_defs.md#listlinuxsubscriptionsrequestrequesttypedef)
- [GetRegisteredSubscriptionProviderResponseTypeDef](./type_defs.md#getregisteredsubscriptionproviderresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [RegisterSubscriptionProviderResponseTypeDef](./type_defs.md#registersubscriptionproviderresponsetypedef)
- [GetServiceSettingsResponseTypeDef](./type_defs.md#getservicesettingsresponsetypedef)
- [UpdateServiceSettingsResponseTypeDef](./type_defs.md#updateservicesettingsresponsetypedef)
- [ListLinuxSubscriptionInstancesResponseTypeDef](./type_defs.md#listlinuxsubscriptioninstancesresponsetypedef)
- [UpdateServiceSettingsRequestRequestTypeDef](./type_defs.md#updateservicesettingsrequestrequesttypedef)
- [ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef](./type_defs.md#listlinuxsubscriptioninstancesrequestlistlinuxsubscriptioninstancespaginatetypedef)
- [ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef](./type_defs.md#listlinuxsubscriptionsrequestlistlinuxsubscriptionspaginatetypedef)
- [ListRegisteredSubscriptionProvidersRequestListRegisteredSubscriptionProvidersPaginateTypeDef](./type_defs.md#listregisteredsubscriptionprovidersrequestlistregisteredsubscriptionproviderspaginatetypedef)
- [ListLinuxSubscriptionsResponseTypeDef](./type_defs.md#listlinuxsubscriptionsresponsetypedef)
- [ListRegisteredSubscriptionProvidersResponseTypeDef](./type_defs.md#listregisteredsubscriptionprovidersresponsetypedef)

