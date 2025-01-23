# PcaConnectorAd module

> [Index](../README.md) > PcaConnectorAd


!!! note ""

    Auto-generated documentation for [PcaConnectorAd](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#pcaconnectorad)
    type annotations stubs module [types-aiobotocore-pca-connector-ad](https://pypi.org/project/types-aiobotocore-pca-connector-ad/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `PcaConnectorAd` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `PcaConnectorAd` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[pca-connector-ad]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[pca-connector-ad]'

# standalone installation
python -m pip install types-aiobotocore-pca-connector-ad
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-pca-connector-ad
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PcaConnectorAdClient

Type annotations and code completion for  `#!python session.create_client("pca-connector-ad")` as [PcaConnectorAdClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client)

```python
# PcaConnectorAdClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_pca_connector_ad.client import PcaConnectorAdClient


session = get_session()
async with session.create_client("pca-connector-ad") as client:
    client: PcaConnectorAdClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("pca-connector-ad").get_paginator("...")`.

```python
# ListConnectorsPaginator usage example

from types_aiobotocore_pca_connector_ad.paginator import ListConnectorsPaginator

def get_list_connectors_paginator() -> ListConnectorsPaginator:
    return client.get_paginator("list_connectors"))
```

- [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
- [ListDirectoryRegistrationsPaginator](./paginators.md#listdirectoryregistrationspaginator)
- [ListServicePrincipalNamesPaginator](./paginators.md#listserviceprincipalnamespaginator)
- [ListTemplateGroupAccessControlEntriesPaginator](./paginators.md#listtemplategroupaccesscontrolentriespaginator)
- [ListTemplatesPaginator](./paginators.md#listtemplatespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccessRightType usage example

from types_aiobotocore_pca_connector_ad.literals import AccessRightType

def get_value() -> AccessRightType:
    return "ALLOW"
```

- [AccessRightType](./literals.md#accessrighttype)
- [ApplicationPolicyTypeType](./literals.md#applicationpolicytypetype)
- [ClientCompatibilityV2Type](./literals.md#clientcompatibilityv2type)
- [ClientCompatibilityV3Type](./literals.md#clientcompatibilityv3type)
- [ClientCompatibilityV4Type](./literals.md#clientcompatibilityv4type)
- [ConnectorStatusReasonType](./literals.md#connectorstatusreasontype)
- [ConnectorStatusType](./literals.md#connectorstatustype)
- [DirectoryRegistrationStatusReasonType](./literals.md#directoryregistrationstatusreasontype)
- [DirectoryRegistrationStatusType](./literals.md#directoryregistrationstatustype)
- [HashAlgorithmType](./literals.md#hashalgorithmtype)
- [KeySpecType](./literals.md#keyspectype)
- [KeyUsagePropertyTypeType](./literals.md#keyusagepropertytypetype)
- [ListConnectorsPaginatorName](./literals.md#listconnectorspaginatorname)
- [ListDirectoryRegistrationsPaginatorName](./literals.md#listdirectoryregistrationspaginatorname)
- [ListServicePrincipalNamesPaginatorName](./literals.md#listserviceprincipalnamespaginatorname)
- [ListTemplateGroupAccessControlEntriesPaginatorName](./literals.md#listtemplategroupaccesscontrolentriespaginatorname)
- [ListTemplatesPaginatorName](./literals.md#listtemplatespaginatorname)
- [PrivateKeyAlgorithmType](./literals.md#privatekeyalgorithmtype)
- [ServicePrincipalNameStatusReasonType](./literals.md#serviceprincipalnamestatusreasontype)
- [ServicePrincipalNameStatusType](./literals.md#serviceprincipalnamestatustype)
- [TemplateStatusType](./literals.md#templatestatustype)
- [ValidityPeriodTypeType](./literals.md#validityperiodtypetype)
- [PcaConnectorAdServiceName](./literals.md#pcaconnectoradservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessRightsTypeDef](./type_defs.md#accessrightstypedef)
- [ApplicationPolicyTypeDef](./type_defs.md#applicationpolicytypedef)
- [ValidityPeriodTypeDef](./type_defs.md#validityperiodtypedef)
- [VpcInformationOutputTypeDef](./type_defs.md#vpcinformationoutputtypedef)
- [VpcInformationTypeDef](./type_defs.md#vpcinformationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateDirectoryRegistrationRequestRequestTypeDef](./type_defs.md#createdirectoryregistrationrequestrequesttypedef)
- [CreateServicePrincipalNameRequestRequestTypeDef](./type_defs.md#createserviceprincipalnamerequestrequesttypedef)
- [DeleteConnectorRequestRequestTypeDef](./type_defs.md#deleteconnectorrequestrequesttypedef)
- [DeleteDirectoryRegistrationRequestRequestTypeDef](./type_defs.md#deletedirectoryregistrationrequestrequesttypedef)
- [DeleteServicePrincipalNameRequestRequestTypeDef](./type_defs.md#deleteserviceprincipalnamerequestrequesttypedef)
- [DeleteTemplateGroupAccessControlEntryRequestRequestTypeDef](./type_defs.md#deletetemplategroupaccesscontrolentryrequestrequesttypedef)
- [DeleteTemplateRequestRequestTypeDef](./type_defs.md#deletetemplaterequestrequesttypedef)
- [DirectoryRegistrationSummaryTypeDef](./type_defs.md#directoryregistrationsummarytypedef)
- [DirectoryRegistrationTypeDef](./type_defs.md#directoryregistrationtypedef)
- [EnrollmentFlagsV2TypeDef](./type_defs.md#enrollmentflagsv2typedef)
- [EnrollmentFlagsV3TypeDef](./type_defs.md#enrollmentflagsv3typedef)
- [EnrollmentFlagsV4TypeDef](./type_defs.md#enrollmentflagsv4typedef)
- [GeneralFlagsV2TypeDef](./type_defs.md#generalflagsv2typedef)
- [GeneralFlagsV3TypeDef](./type_defs.md#generalflagsv3typedef)
- [GeneralFlagsV4TypeDef](./type_defs.md#generalflagsv4typedef)
- [GetConnectorRequestRequestTypeDef](./type_defs.md#getconnectorrequestrequesttypedef)
- [GetDirectoryRegistrationRequestRequestTypeDef](./type_defs.md#getdirectoryregistrationrequestrequesttypedef)
- [GetServicePrincipalNameRequestRequestTypeDef](./type_defs.md#getserviceprincipalnamerequestrequesttypedef)
- [ServicePrincipalNameTypeDef](./type_defs.md#serviceprincipalnametypedef)
- [GetTemplateGroupAccessControlEntryRequestRequestTypeDef](./type_defs.md#gettemplategroupaccesscontrolentryrequestrequesttypedef)
- [GetTemplateRequestRequestTypeDef](./type_defs.md#gettemplaterequestrequesttypedef)
- [KeyUsageFlagsTypeDef](./type_defs.md#keyusageflagstypedef)
- [KeyUsagePropertyFlagsTypeDef](./type_defs.md#keyusagepropertyflagstypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListConnectorsRequestRequestTypeDef](./type_defs.md#listconnectorsrequestrequesttypedef)
- [ListDirectoryRegistrationsRequestRequestTypeDef](./type_defs.md#listdirectoryregistrationsrequestrequesttypedef)
- [ListServicePrincipalNamesRequestRequestTypeDef](./type_defs.md#listserviceprincipalnamesrequestrequesttypedef)
- [ServicePrincipalNameSummaryTypeDef](./type_defs.md#serviceprincipalnamesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTemplateGroupAccessControlEntriesRequestRequestTypeDef](./type_defs.md#listtemplategroupaccesscontrolentriesrequestrequesttypedef)
- [ListTemplatesRequestRequestTypeDef](./type_defs.md#listtemplatesrequestrequesttypedef)
- [PrivateKeyAttributesV2OutputTypeDef](./type_defs.md#privatekeyattributesv2outputtypedef)
- [PrivateKeyAttributesV2TypeDef](./type_defs.md#privatekeyattributesv2typedef)
- [PrivateKeyFlagsV2TypeDef](./type_defs.md#privatekeyflagsv2typedef)
- [PrivateKeyFlagsV3TypeDef](./type_defs.md#privatekeyflagsv3typedef)
- [PrivateKeyFlagsV4TypeDef](./type_defs.md#privatekeyflagsv4typedef)
- [SubjectNameFlagsV2TypeDef](./type_defs.md#subjectnameflagsv2typedef)
- [SubjectNameFlagsV3TypeDef](./type_defs.md#subjectnameflagsv3typedef)
- [SubjectNameFlagsV4TypeDef](./type_defs.md#subjectnameflagsv4typedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TemplateRevisionTypeDef](./type_defs.md#templaterevisiontypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AccessControlEntrySummaryTypeDef](./type_defs.md#accesscontrolentrysummarytypedef)
- [AccessControlEntryTypeDef](./type_defs.md#accesscontrolentrytypedef)
- [CreateTemplateGroupAccessControlEntryRequestRequestTypeDef](./type_defs.md#createtemplategroupaccesscontrolentryrequestrequesttypedef)
- [UpdateTemplateGroupAccessControlEntryRequestRequestTypeDef](./type_defs.md#updatetemplategroupaccesscontrolentryrequestrequesttypedef)
- [ApplicationPoliciesOutputTypeDef](./type_defs.md#applicationpoliciesoutputtypedef)
- [ApplicationPoliciesTypeDef](./type_defs.md#applicationpoliciestypedef)
- [CertificateValidityTypeDef](./type_defs.md#certificatevaliditytypedef)
- [ConnectorSummaryTypeDef](./type_defs.md#connectorsummarytypedef)
- [ConnectorTypeDef](./type_defs.md#connectortypedef)
- [CreateConnectorRequestRequestTypeDef](./type_defs.md#createconnectorrequestrequesttypedef)
- [CreateConnectorResponseTypeDef](./type_defs.md#createconnectorresponsetypedef)
- [CreateDirectoryRegistrationResponseTypeDef](./type_defs.md#createdirectoryregistrationresponsetypedef)
- [CreateTemplateResponseTypeDef](./type_defs.md#createtemplateresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListDirectoryRegistrationsResponseTypeDef](./type_defs.md#listdirectoryregistrationsresponsetypedef)
- [GetDirectoryRegistrationResponseTypeDef](./type_defs.md#getdirectoryregistrationresponsetypedef)
- [GetServicePrincipalNameResponseTypeDef](./type_defs.md#getserviceprincipalnameresponsetypedef)
- [KeyUsageTypeDef](./type_defs.md#keyusagetypedef)
- [KeyUsagePropertyTypeDef](./type_defs.md#keyusagepropertytypedef)
- [ListConnectorsRequestPaginateTypeDef](./type_defs.md#listconnectorsrequestpaginatetypedef)
- [ListDirectoryRegistrationsRequestPaginateTypeDef](./type_defs.md#listdirectoryregistrationsrequestpaginatetypedef)
- [ListServicePrincipalNamesRequestPaginateTypeDef](./type_defs.md#listserviceprincipalnamesrequestpaginatetypedef)
- [ListTemplateGroupAccessControlEntriesRequestPaginateTypeDef](./type_defs.md#listtemplategroupaccesscontrolentriesrequestpaginatetypedef)
- [ListTemplatesRequestPaginateTypeDef](./type_defs.md#listtemplatesrequestpaginatetypedef)
- [ListServicePrincipalNamesResponseTypeDef](./type_defs.md#listserviceprincipalnamesresponsetypedef)
- [PrivateKeyAttributesV2UnionTypeDef](./type_defs.md#privatekeyattributesv2uniontypedef)
- [ListTemplateGroupAccessControlEntriesResponseTypeDef](./type_defs.md#listtemplategroupaccesscontrolentriesresponsetypedef)
- [GetTemplateGroupAccessControlEntryResponseTypeDef](./type_defs.md#gettemplategroupaccesscontrolentryresponsetypedef)
- [ApplicationPoliciesUnionTypeDef](./type_defs.md#applicationpoliciesuniontypedef)
- [ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef)
- [GetConnectorResponseTypeDef](./type_defs.md#getconnectorresponsetypedef)
- [ExtensionsV2OutputTypeDef](./type_defs.md#extensionsv2outputtypedef)
- [ExtensionsV3OutputTypeDef](./type_defs.md#extensionsv3outputtypedef)
- [ExtensionsV4OutputTypeDef](./type_defs.md#extensionsv4outputtypedef)
- [PrivateKeyAttributesV3OutputTypeDef](./type_defs.md#privatekeyattributesv3outputtypedef)
- [PrivateKeyAttributesV3TypeDef](./type_defs.md#privatekeyattributesv3typedef)
- [PrivateKeyAttributesV4OutputTypeDef](./type_defs.md#privatekeyattributesv4outputtypedef)
- [PrivateKeyAttributesV4TypeDef](./type_defs.md#privatekeyattributesv4typedef)
- [ExtensionsV2TypeDef](./type_defs.md#extensionsv2typedef)
- [ExtensionsV3TypeDef](./type_defs.md#extensionsv3typedef)
- [ExtensionsV4TypeDef](./type_defs.md#extensionsv4typedef)
- [TemplateV2OutputTypeDef](./type_defs.md#templatev2outputtypedef)
- [TemplateV3OutputTypeDef](./type_defs.md#templatev3outputtypedef)
- [PrivateKeyAttributesV3UnionTypeDef](./type_defs.md#privatekeyattributesv3uniontypedef)
- [TemplateV4OutputTypeDef](./type_defs.md#templatev4outputtypedef)
- [PrivateKeyAttributesV4UnionTypeDef](./type_defs.md#privatekeyattributesv4uniontypedef)
- [ExtensionsV2UnionTypeDef](./type_defs.md#extensionsv2uniontypedef)
- [ExtensionsV3UnionTypeDef](./type_defs.md#extensionsv3uniontypedef)
- [ExtensionsV4UnionTypeDef](./type_defs.md#extensionsv4uniontypedef)
- [TemplateDefinitionOutputTypeDef](./type_defs.md#templatedefinitionoutputtypedef)
- [TemplateV2TypeDef](./type_defs.md#templatev2typedef)
- [TemplateV3TypeDef](./type_defs.md#templatev3typedef)
- [TemplateV4TypeDef](./type_defs.md#templatev4typedef)
- [TemplateSummaryTypeDef](./type_defs.md#templatesummarytypedef)
- [TemplateTypeDef](./type_defs.md#templatetypedef)
- [TemplateV2UnionTypeDef](./type_defs.md#templatev2uniontypedef)
- [TemplateV3UnionTypeDef](./type_defs.md#templatev3uniontypedef)
- [TemplateV4UnionTypeDef](./type_defs.md#templatev4uniontypedef)
- [ListTemplatesResponseTypeDef](./type_defs.md#listtemplatesresponsetypedef)
- [GetTemplateResponseTypeDef](./type_defs.md#gettemplateresponsetypedef)
- [TemplateDefinitionTypeDef](./type_defs.md#templatedefinitiontypedef)
- [CreateTemplateRequestRequestTypeDef](./type_defs.md#createtemplaterequestrequesttypedef)
- [UpdateTemplateRequestRequestTypeDef](./type_defs.md#updatetemplaterequestrequesttypedef)

