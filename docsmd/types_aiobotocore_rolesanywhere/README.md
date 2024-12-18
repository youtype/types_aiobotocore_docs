# IAMRolesAnywhere module

> [Index](../README.md) > IAMRolesAnywhere


!!! note ""

    Auto-generated documentation for [IAMRolesAnywhere](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#iamrolesanywhere)
    type annotations stubs module [types-aiobotocore-rolesanywhere](https://pypi.org/project/types-aiobotocore-rolesanywhere/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `IAMRolesAnywhere` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `IAMRolesAnywhere` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[rolesanywhere]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[rolesanywhere]'

# standalone installation
python -m pip install types-aiobotocore-rolesanywhere
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-rolesanywhere
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IAMRolesAnywhereClient

Type annotations and code completion for  `#!python session.create_client("rolesanywhere")` as [IAMRolesAnywhereClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# IAMRolesAnywhereClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_rolesanywhere.client import IAMRolesAnywhereClient


session = get_session()
async with session.create_client("rolesanywhere") as client:
    client: IAMRolesAnywhereClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("rolesanywhere").get_paginator("...")`.

```python
# ListCrlsPaginator usage example

from types_aiobotocore_rolesanywhere.paginator import ListCrlsPaginator

def get_list_crls_paginator() -> ListCrlsPaginator:
    return client.get_paginator("list_crls"))
```

- [ListCrlsPaginator](./paginators.md#listcrlspaginator)
- [ListProfilesPaginator](./paginators.md#listprofilespaginator)
- [ListSubjectsPaginator](./paginators.md#listsubjectspaginator)
- [ListTrustAnchorsPaginator](./paginators.md#listtrustanchorspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CertificateFieldType usage example

from types_aiobotocore_rolesanywhere.literals import CertificateFieldType

def get_value() -> CertificateFieldType:
    return "x509Issuer"
```

- [CertificateFieldType](./literals.md#certificatefieldtype)
- [ListCrlsPaginatorName](./literals.md#listcrlspaginatorname)
- [ListProfilesPaginatorName](./literals.md#listprofilespaginatorname)
- [ListSubjectsPaginatorName](./literals.md#listsubjectspaginatorname)
- [ListTrustAnchorsPaginatorName](./literals.md#listtrustanchorspaginatorname)
- [NotificationChannelType](./literals.md#notificationchanneltype)
- [NotificationEventType](./literals.md#notificationeventtype)
- [TrustAnchorTypeType](./literals.md#trustanchortypetype)
- [IAMRolesAnywhereServiceName](./literals.md#iamrolesanywhereservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [MappingRuleTypeDef](./type_defs.md#mappingruletypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [NotificationSettingTypeDef](./type_defs.md#notificationsettingtypedef)
- [CredentialSummaryTypeDef](./type_defs.md#credentialsummarytypedef)
- [CrlDetailTypeDef](./type_defs.md#crldetailtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteAttributeMappingRequestRequestTypeDef](./type_defs.md#deleteattributemappingrequestrequesttypedef)
- [InstancePropertyTypeDef](./type_defs.md#instancepropertytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListRequestRequestTypeDef](./type_defs.md#listrequestrequesttypedef)
- [SubjectSummaryTypeDef](./type_defs.md#subjectsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [NotificationSettingDetailTypeDef](./type_defs.md#notificationsettingdetailtypedef)
- [NotificationSettingKeyTypeDef](./type_defs.md#notificationsettingkeytypedef)
- [ScalarCrlRequestRequestTypeDef](./type_defs.md#scalarcrlrequestrequesttypedef)
- [ScalarProfileRequestRequestTypeDef](./type_defs.md#scalarprofilerequestrequesttypedef)
- [ScalarSubjectRequestRequestTypeDef](./type_defs.md#scalarsubjectrequestrequesttypedef)
- [ScalarTrustAnchorRequestRequestTypeDef](./type_defs.md#scalartrustanchorrequestrequesttypedef)
- [SourceDataTypeDef](./type_defs.md#sourcedatatypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateProfileRequestRequestTypeDef](./type_defs.md#updateprofilerequestrequesttypedef)
- [AttributeMappingTypeDef](./type_defs.md#attributemappingtypedef)
- [PutAttributeMappingRequestRequestTypeDef](./type_defs.md#putattributemappingrequestrequesttypedef)
- [UpdateCrlRequestRequestTypeDef](./type_defs.md#updatecrlrequestrequesttypedef)
- [CreateProfileRequestRequestTypeDef](./type_defs.md#createprofilerequestrequesttypedef)
- [ImportCrlRequestRequestTypeDef](./type_defs.md#importcrlrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [PutNotificationSettingsRequestRequestTypeDef](./type_defs.md#putnotificationsettingsrequestrequesttypedef)
- [CrlDetailResponseTypeDef](./type_defs.md#crldetailresponsetypedef)
- [ListCrlsResponseTypeDef](./type_defs.md#listcrlsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [SubjectDetailTypeDef](./type_defs.md#subjectdetailtypedef)
- [ListRequestListCrlsPaginateTypeDef](./type_defs.md#listrequestlistcrlspaginatetypedef)
- [ListRequestListProfilesPaginateTypeDef](./type_defs.md#listrequestlistprofilespaginatetypedef)
- [ListRequestListSubjectsPaginateTypeDef](./type_defs.md#listrequestlistsubjectspaginatetypedef)
- [ListRequestListTrustAnchorsPaginateTypeDef](./type_defs.md#listrequestlisttrustanchorspaginatetypedef)
- [ListSubjectsResponseTypeDef](./type_defs.md#listsubjectsresponsetypedef)
- [ResetNotificationSettingsRequestRequestTypeDef](./type_defs.md#resetnotificationsettingsrequestrequesttypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [ProfileDetailTypeDef](./type_defs.md#profiledetailtypedef)
- [SubjectDetailResponseTypeDef](./type_defs.md#subjectdetailresponsetypedef)
- [CreateTrustAnchorRequestRequestTypeDef](./type_defs.md#createtrustanchorrequestrequesttypedef)
- [TrustAnchorDetailTypeDef](./type_defs.md#trustanchordetailtypedef)
- [UpdateTrustAnchorRequestRequestTypeDef](./type_defs.md#updatetrustanchorrequestrequesttypedef)
- [DeleteAttributeMappingResponseTypeDef](./type_defs.md#deleteattributemappingresponsetypedef)
- [ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef)
- [ProfileDetailResponseTypeDef](./type_defs.md#profiledetailresponsetypedef)
- [PutAttributeMappingResponseTypeDef](./type_defs.md#putattributemappingresponsetypedef)
- [ListTrustAnchorsResponseTypeDef](./type_defs.md#listtrustanchorsresponsetypedef)
- [PutNotificationSettingsResponseTypeDef](./type_defs.md#putnotificationsettingsresponsetypedef)
- [ResetNotificationSettingsResponseTypeDef](./type_defs.md#resetnotificationsettingsresponsetypedef)
- [TrustAnchorDetailResponseTypeDef](./type_defs.md#trustanchordetailresponsetypedef)

