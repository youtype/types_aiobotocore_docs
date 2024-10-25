# Route53Profiles module

> [Index](../README.md) > Route53Profiles


!!! note ""

    Auto-generated documentation for [Route53Profiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles.html#Route53Profiles)
    type annotations stubs module [types-aiobotocore-route53profiles](https://pypi.org/project/types-aiobotocore-route53profiles/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Route53Profiles` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[route53profiles]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[route53profiles]'


# standalone installation
python -m pip install types-aiobotocore-route53profiles
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-route53profiles
```

## Usage

Code samples can be found in [Examples](./usage.md).

## Route53ProfilesClient

Type annotations and code completion for  `#!python session.create_client("route53profiles")` as [Route53ProfilesClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles.html#Route53Profiles.Client)

```python
# Route53ProfilesClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53profiles.client import Route53ProfilesClient


session = get_session()
async with session.create_client("route53profiles") as client:
    client: Route53ProfilesClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("route53profiles").get_paginator("...")`.

```python
# ListProfileAssociationsPaginator usage example

from types_aiobotocore_route53profiles.paginator import ListProfileAssociationsPaginator

def get_list_profile_associations_paginator() -> ListProfileAssociationsPaginator:
    return client.get_paginator("list_profile_associations"))
```

- [ListProfileAssociationsPaginator](./paginators.md#listprofileassociationspaginator)
- [ListProfileResourceAssociationsPaginator](./paginators.md#listprofileresourceassociationspaginator)
- [ListProfilesPaginator](./paginators.md#listprofilespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListProfileAssociationsPaginatorName usage example

from types_aiobotocore_route53profiles.literals import ListProfileAssociationsPaginatorName

def get_value() -> ListProfileAssociationsPaginatorName:
    return "list_profile_associations"
```

- [ListProfileAssociationsPaginatorName](./literals.md#listprofileassociationspaginatorname)
- [ListProfileResourceAssociationsPaginatorName](./literals.md#listprofileresourceassociationspaginatorname)
- [ListProfilesPaginatorName](./literals.md#listprofilespaginatorname)
- [ProfileStatusType](./literals.md#profilestatustype)
- [ShareStatusType](./literals.md#sharestatustype)
- [Route53ProfilesServiceName](./literals.md#route53profilesservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TagTypeDef](./type_defs.md#tagtypedef)
- [ProfileAssociationTypeDef](./type_defs.md#profileassociationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AssociateResourceToProfileRequestRequestTypeDef](./type_defs.md#associateresourcetoprofilerequestrequesttypedef)
- [ProfileResourceAssociationTypeDef](./type_defs.md#profileresourceassociationtypedef)
- [ProfileTypeDef](./type_defs.md#profiletypedef)
- [DeleteProfileRequestRequestTypeDef](./type_defs.md#deleteprofilerequestrequesttypedef)
- [DisassociateProfileRequestRequestTypeDef](./type_defs.md#disassociateprofilerequestrequesttypedef)
- [DisassociateResourceFromProfileRequestRequestTypeDef](./type_defs.md#disassociateresourcefromprofilerequestrequesttypedef)
- [GetProfileAssociationRequestRequestTypeDef](./type_defs.md#getprofileassociationrequestrequesttypedef)
- [GetProfileRequestRequestTypeDef](./type_defs.md#getprofilerequestrequesttypedef)
- [GetProfileResourceAssociationRequestRequestTypeDef](./type_defs.md#getprofileresourceassociationrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListProfileAssociationsRequestRequestTypeDef](./type_defs.md#listprofileassociationsrequestrequesttypedef)
- [ListProfileResourceAssociationsRequestRequestTypeDef](./type_defs.md#listprofileresourceassociationsrequestrequesttypedef)
- [ListProfilesRequestRequestTypeDef](./type_defs.md#listprofilesrequestrequesttypedef)
- [ProfileSummaryTypeDef](./type_defs.md#profilesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateProfileResourceAssociationRequestRequestTypeDef](./type_defs.md#updateprofileresourceassociationrequestrequesttypedef)
- [AssociateProfileRequestRequestTypeDef](./type_defs.md#associateprofilerequestrequesttypedef)
- [CreateProfileRequestRequestTypeDef](./type_defs.md#createprofilerequestrequesttypedef)
- [AssociateProfileResponseTypeDef](./type_defs.md#associateprofileresponsetypedef)
- [DisassociateProfileResponseTypeDef](./type_defs.md#disassociateprofileresponsetypedef)
- [GetProfileAssociationResponseTypeDef](./type_defs.md#getprofileassociationresponsetypedef)
- [ListProfileAssociationsResponseTypeDef](./type_defs.md#listprofileassociationsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [AssociateResourceToProfileResponseTypeDef](./type_defs.md#associateresourcetoprofileresponsetypedef)
- [DisassociateResourceFromProfileResponseTypeDef](./type_defs.md#disassociateresourcefromprofileresponsetypedef)
- [GetProfileResourceAssociationResponseTypeDef](./type_defs.md#getprofileresourceassociationresponsetypedef)
- [ListProfileResourceAssociationsResponseTypeDef](./type_defs.md#listprofileresourceassociationsresponsetypedef)
- [UpdateProfileResourceAssociationResponseTypeDef](./type_defs.md#updateprofileresourceassociationresponsetypedef)
- [CreateProfileResponseTypeDef](./type_defs.md#createprofileresponsetypedef)
- [DeleteProfileResponseTypeDef](./type_defs.md#deleteprofileresponsetypedef)
- [GetProfileResponseTypeDef](./type_defs.md#getprofileresponsetypedef)
- [ListProfileAssociationsRequestListProfileAssociationsPaginateTypeDef](./type_defs.md#listprofileassociationsrequestlistprofileassociationspaginatetypedef)
- [ListProfileResourceAssociationsRequestListProfileResourceAssociationsPaginateTypeDef](./type_defs.md#listprofileresourceassociationsrequestlistprofileresourceassociationspaginatetypedef)
- [ListProfilesRequestListProfilesPaginateTypeDef](./type_defs.md#listprofilesrequestlistprofilespaginatetypedef)
- [ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef)

