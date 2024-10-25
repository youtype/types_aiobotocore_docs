# ACMPCA module

> [Index](../README.md) > ACMPCA


!!! note ""

    Auto-generated documentation for [ACMPCA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
    type annotations stubs module [types-aiobotocore-acm-pca](https://pypi.org/project/types-aiobotocore-acm-pca/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ACMPCA` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[acm-pca]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[acm-pca]'


# standalone installation
python -m pip install types-aiobotocore-acm-pca
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-acm-pca
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ACMPCAClient

Type annotations and code completion for  `#!python session.create_client("acm-pca")` as [ACMPCAClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client)

```python
# ACMPCAClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_acm_pca.client import ACMPCAClient


session = get_session()
async with session.create_client("acm-pca") as client:
    client: ACMPCAClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("acm-pca").get_paginator("...")`.

```python
# ListCertificateAuthoritiesPaginator usage example

from types_aiobotocore_acm_pca.paginator import ListCertificateAuthoritiesPaginator

def get_list_certificate_authorities_paginator() -> ListCertificateAuthoritiesPaginator:
    return client.get_paginator("list_certificate_authorities"))
```

- [ListCertificateAuthoritiesPaginator](./paginators.md#listcertificateauthoritiespaginator)
- [ListPermissionsPaginator](./paginators.md#listpermissionspaginator)
- [ListTagsPaginator](./paginators.md#listtagspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("acm-pca").get_waiter("...")`.

```python
# AuditReportCreatedWaiter usage example

from types_aiobotocore_acm_pca.waiter import AuditReportCreatedWaiter

def get_audit_report_created_waiter() -> AuditReportCreatedWaiter:
    return Session().client("acm-pca").get_waiter("audit_report_created")
```

- [AuditReportCreatedWaiter](./waiters.md#auditreportcreatedwaiter)
- [CertificateAuthorityCSRCreatedWaiter](./waiters.md#certificateauthoritycsrcreatedwaiter)
- [CertificateIssuedWaiter](./waiters.md#certificateissuedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccessMethodTypeType usage example

from types_aiobotocore_acm_pca.literals import AccessMethodTypeType

def get_value() -> AccessMethodTypeType:
    return "CA_REPOSITORY"
```

- [AccessMethodTypeType](./literals.md#accessmethodtypetype)
- [ActionTypeType](./literals.md#actiontypetype)
- [AuditReportCreatedWaiterName](./literals.md#auditreportcreatedwaitername)
- [AuditReportResponseFormatType](./literals.md#auditreportresponseformattype)
- [AuditReportStatusType](./literals.md#auditreportstatustype)
- [CertificateAuthorityCSRCreatedWaiterName](./literals.md#certificateauthoritycsrcreatedwaitername)
- [CertificateAuthorityStatusType](./literals.md#certificateauthoritystatustype)
- [CertificateAuthorityTypeType](./literals.md#certificateauthoritytypetype)
- [CertificateAuthorityUsageModeType](./literals.md#certificateauthorityusagemodetype)
- [CertificateIssuedWaiterName](./literals.md#certificateissuedwaitername)
- [ExtendedKeyUsageTypeType](./literals.md#extendedkeyusagetypetype)
- [FailureReasonType](./literals.md#failurereasontype)
- [KeyAlgorithmType](./literals.md#keyalgorithmtype)
- [KeyStorageSecurityStandardType](./literals.md#keystoragesecuritystandardtype)
- [ListCertificateAuthoritiesPaginatorName](./literals.md#listcertificateauthoritiespaginatorname)
- [ListPermissionsPaginatorName](./literals.md#listpermissionspaginatorname)
- [ListTagsPaginatorName](./literals.md#listtagspaginatorname)
- [PolicyQualifierIdType](./literals.md#policyqualifieridtype)
- [ResourceOwnerType](./literals.md#resourceownertype)
- [RevocationReasonType](./literals.md#revocationreasontype)
- [S3ObjectAclType](./literals.md#s3objectacltype)
- [SigningAlgorithmType](./literals.md#signingalgorithmtype)
- [ValidityPeriodTypeType](./literals.md#validityperiodtypetype)
- [ACMPCAServiceName](./literals.md#acmpcaservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CustomAttributeTypeDef](./type_defs.md#customattributetypedef)
- [AccessMethodTypeDef](./type_defs.md#accessmethodtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CreateCertificateAuthorityAuditReportRequestRequestTypeDef](./type_defs.md#createcertificateauthorityauditreportrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CreatePermissionRequestRequestTypeDef](./type_defs.md#createpermissionrequestrequesttypedef)
- [CrlDistributionPointExtensionConfigurationTypeDef](./type_defs.md#crldistributionpointextensionconfigurationtypedef)
- [KeyUsageTypeDef](./type_defs.md#keyusagetypedef)
- [CustomExtensionTypeDef](./type_defs.md#customextensiontypedef)
- [DeleteCertificateAuthorityRequestRequestTypeDef](./type_defs.md#deletecertificateauthorityrequestrequesttypedef)
- [DeletePermissionRequestRequestTypeDef](./type_defs.md#deletepermissionrequestrequesttypedef)
- [DeletePolicyRequestRequestTypeDef](./type_defs.md#deletepolicyrequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeCertificateAuthorityAuditReportRequestRequestTypeDef](./type_defs.md#describecertificateauthorityauditreportrequestrequesttypedef)
- [DescribeCertificateAuthorityRequestRequestTypeDef](./type_defs.md#describecertificateauthorityrequestrequesttypedef)
- [EdiPartyNameTypeDef](./type_defs.md#edipartynametypedef)
- [ExtendedKeyUsageTypeDef](./type_defs.md#extendedkeyusagetypedef)
- [OtherNameTypeDef](./type_defs.md#othernametypedef)
- [GetCertificateAuthorityCertificateRequestRequestTypeDef](./type_defs.md#getcertificateauthoritycertificaterequestrequesttypedef)
- [GetCertificateAuthorityCsrRequestRequestTypeDef](./type_defs.md#getcertificateauthoritycsrrequestrequesttypedef)
- [GetCertificateRequestRequestTypeDef](./type_defs.md#getcertificaterequestrequesttypedef)
- [GetPolicyRequestRequestTypeDef](./type_defs.md#getpolicyrequestrequesttypedef)
- [ValidityTypeDef](./type_defs.md#validitytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListCertificateAuthoritiesRequestRequestTypeDef](./type_defs.md#listcertificateauthoritiesrequestrequesttypedef)
- [ListPermissionsRequestRequestTypeDef](./type_defs.md#listpermissionsrequestrequesttypedef)
- [PermissionTypeDef](./type_defs.md#permissiontypedef)
- [ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef)
- [OcspConfigurationTypeDef](./type_defs.md#ocspconfigurationtypedef)
- [QualifierTypeDef](./type_defs.md#qualifiertypedef)
- [PutPolicyRequestRequestTypeDef](./type_defs.md#putpolicyrequestrequesttypedef)
- [RestoreCertificateAuthorityRequestRequestTypeDef](./type_defs.md#restorecertificateauthorityrequestrequesttypedef)
- [RevokeCertificateRequestRequestTypeDef](./type_defs.md#revokecertificaterequestrequesttypedef)
- [ASN1SubjectOutputTypeDef](./type_defs.md#asn1subjectoutputtypedef)
- [ASN1SubjectTypeDef](./type_defs.md#asn1subjecttypedef)
- [ImportCertificateAuthorityCertificateRequestRequestTypeDef](./type_defs.md#importcertificateauthoritycertificaterequestrequesttypedef)
- [CreateCertificateAuthorityAuditReportResponseTypeDef](./type_defs.md#createcertificateauthorityauditreportresponsetypedef)
- [CreateCertificateAuthorityResponseTypeDef](./type_defs.md#createcertificateauthorityresponsetypedef)
- [DescribeCertificateAuthorityAuditReportResponseTypeDef](./type_defs.md#describecertificateauthorityauditreportresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetCertificateAuthorityCertificateResponseTypeDef](./type_defs.md#getcertificateauthoritycertificateresponsetypedef)
- [GetCertificateAuthorityCsrResponseTypeDef](./type_defs.md#getcertificateauthoritycsrresponsetypedef)
- [GetCertificateResponseTypeDef](./type_defs.md#getcertificateresponsetypedef)
- [GetPolicyResponseTypeDef](./type_defs.md#getpolicyresponsetypedef)
- [IssueCertificateResponseTypeDef](./type_defs.md#issuecertificateresponsetypedef)
- [ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef)
- [TagCertificateAuthorityRequestRequestTypeDef](./type_defs.md#tagcertificateauthorityrequestrequesttypedef)
- [UntagCertificateAuthorityRequestRequestTypeDef](./type_defs.md#untagcertificateauthorityrequestrequesttypedef)
- [CrlConfigurationTypeDef](./type_defs.md#crlconfigurationtypedef)
- [DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef](./type_defs.md#describecertificateauthorityauditreportrequestauditreportcreatedwaittypedef)
- [GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef](./type_defs.md#getcertificateauthoritycsrrequestcertificateauthoritycsrcreatedwaittypedef)
- [GetCertificateRequestCertificateIssuedWaitTypeDef](./type_defs.md#getcertificaterequestcertificateissuedwaittypedef)
- [ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef](./type_defs.md#listcertificateauthoritiesrequestlistcertificateauthoritiespaginatetypedef)
- [ListPermissionsRequestListPermissionsPaginateTypeDef](./type_defs.md#listpermissionsrequestlistpermissionspaginatetypedef)
- [ListTagsRequestListTagsPaginateTypeDef](./type_defs.md#listtagsrequestlisttagspaginatetypedef)
- [ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef)
- [PolicyQualifierInfoTypeDef](./type_defs.md#policyqualifierinfotypedef)
- [GeneralNameOutputTypeDef](./type_defs.md#generalnameoutputtypedef)
- [ASN1SubjectUnionTypeDef](./type_defs.md#asn1subjectuniontypedef)
- [RevocationConfigurationTypeDef](./type_defs.md#revocationconfigurationtypedef)
- [PolicyInformationTypeDef](./type_defs.md#policyinformationtypedef)
- [AccessDescriptionOutputTypeDef](./type_defs.md#accessdescriptionoutputtypedef)
- [GeneralNameTypeDef](./type_defs.md#generalnametypedef)
- [UpdateCertificateAuthorityRequestRequestTypeDef](./type_defs.md#updatecertificateauthorityrequestrequesttypedef)
- [CsrExtensionsOutputTypeDef](./type_defs.md#csrextensionsoutputtypedef)
- [GeneralNameUnionTypeDef](./type_defs.md#generalnameuniontypedef)
- [CertificateAuthorityConfigurationOutputTypeDef](./type_defs.md#certificateauthorityconfigurationoutputtypedef)
- [AccessDescriptionTypeDef](./type_defs.md#accessdescriptiontypedef)
- [ExtensionsTypeDef](./type_defs.md#extensionstypedef)
- [CertificateAuthorityTypeDef](./type_defs.md#certificateauthoritytypedef)
- [AccessDescriptionUnionTypeDef](./type_defs.md#accessdescriptionuniontypedef)
- [ApiPassthroughTypeDef](./type_defs.md#apipassthroughtypedef)
- [DescribeCertificateAuthorityResponseTypeDef](./type_defs.md#describecertificateauthorityresponsetypedef)
- [ListCertificateAuthoritiesResponseTypeDef](./type_defs.md#listcertificateauthoritiesresponsetypedef)
- [CsrExtensionsTypeDef](./type_defs.md#csrextensionstypedef)
- [IssueCertificateRequestRequestTypeDef](./type_defs.md#issuecertificaterequestrequesttypedef)
- [CsrExtensionsUnionTypeDef](./type_defs.md#csrextensionsuniontypedef)
- [CertificateAuthorityConfigurationTypeDef](./type_defs.md#certificateauthorityconfigurationtypedef)
- [CreateCertificateAuthorityRequestRequestTypeDef](./type_defs.md#createcertificateauthorityrequestrequesttypedef)

