# Type definitions

> [Index](../README.md) > [ACMPCA](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ACMPCA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
    type annotations stubs module [types-aiobotocore-acm-pca](https://pypi.org/project/types-aiobotocore-acm-pca/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## CustomAttributeTypeDef

```python
# CustomAttributeTypeDef definition

class CustomAttributeTypeDef(TypedDict):
    ObjectIdentifier: str,
    Value: str,
```

## AccessMethodTypeDef

```python
# AccessMethodTypeDef definition

class AccessMethodTypeDef(TypedDict):
    CustomObjectIdentifier: NotRequired[str],
    AccessMethodType: NotRequired[AccessMethodTypeType],  # (1)
```

1. See [:material-code-brackets: AccessMethodTypeType](./literals.md#accessmethodtypetype) 
## CreateCertificateAuthorityAuditReportRequestRequestTypeDef

```python
# CreateCertificateAuthorityAuditReportRequestRequestTypeDef definition

class CreateCertificateAuthorityAuditReportRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    S3BucketName: str,
    AuditReportResponseFormat: AuditReportResponseFormatType,  # (1)
```

1. See [:material-code-brackets: AuditReportResponseFormatType](./literals.md#auditreportresponseformattype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

## CreatePermissionRequestRequestTypeDef

```python
# CreatePermissionRequestRequestTypeDef definition

class CreatePermissionRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    Principal: str,
    Actions: Sequence[ActionTypeType],  # (1)
    SourceAccount: NotRequired[str],
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
## CrlConfigurationTypeDef

```python
# CrlConfigurationTypeDef definition

class CrlConfigurationTypeDef(TypedDict):
    Enabled: bool,
    ExpirationInDays: NotRequired[int],
    CustomCname: NotRequired[str],
    S3BucketName: NotRequired[str],
    S3ObjectAcl: NotRequired[S3ObjectAclType],  # (1)
```

1. See [:material-code-brackets: S3ObjectAclType](./literals.md#s3objectacltype) 
## KeyUsageTypeDef

```python
# KeyUsageTypeDef definition

class KeyUsageTypeDef(TypedDict):
    DigitalSignature: NotRequired[bool],
    NonRepudiation: NotRequired[bool],
    KeyEncipherment: NotRequired[bool],
    DataEncipherment: NotRequired[bool],
    KeyAgreement: NotRequired[bool],
    KeyCertSign: NotRequired[bool],
    CRLSign: NotRequired[bool],
    EncipherOnly: NotRequired[bool],
    DecipherOnly: NotRequired[bool],
```

## CustomExtensionTypeDef

```python
# CustomExtensionTypeDef definition

class CustomExtensionTypeDef(TypedDict):
    ObjectIdentifier: str,
    Value: str,
    Critical: NotRequired[bool],
```

## DeleteCertificateAuthorityRequestRequestTypeDef

```python
# DeleteCertificateAuthorityRequestRequestTypeDef definition

class DeleteCertificateAuthorityRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    PermanentDeletionTimeInDays: NotRequired[int],
```

## DeletePermissionRequestRequestTypeDef

```python
# DeletePermissionRequestRequestTypeDef definition

class DeletePermissionRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    Principal: str,
    SourceAccount: NotRequired[str],
```

## DeletePolicyRequestRequestTypeDef

```python
# DeletePolicyRequestRequestTypeDef definition

class DeletePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeCertificateAuthorityAuditReportRequestRequestTypeDef

```python
# DescribeCertificateAuthorityAuditReportRequestRequestTypeDef definition

class DescribeCertificateAuthorityAuditReportRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    AuditReportId: str,
```

## DescribeCertificateAuthorityRequestRequestTypeDef

```python
# DescribeCertificateAuthorityRequestRequestTypeDef definition

class DescribeCertificateAuthorityRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
```

## EdiPartyNameTypeDef

```python
# EdiPartyNameTypeDef definition

class EdiPartyNameTypeDef(TypedDict):
    PartyName: str,
    NameAssigner: NotRequired[str],
```

## ExtendedKeyUsageTypeDef

```python
# ExtendedKeyUsageTypeDef definition

class ExtendedKeyUsageTypeDef(TypedDict):
    ExtendedKeyUsageType: NotRequired[ExtendedKeyUsageTypeType],  # (1)
    ExtendedKeyUsageObjectIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: ExtendedKeyUsageTypeType](./literals.md#extendedkeyusagetypetype) 
## OtherNameTypeDef

```python
# OtherNameTypeDef definition

class OtherNameTypeDef(TypedDict):
    TypeId: str,
    Value: str,
```

## GetCertificateAuthorityCertificateRequestRequestTypeDef

```python
# GetCertificateAuthorityCertificateRequestRequestTypeDef definition

class GetCertificateAuthorityCertificateRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
```

## GetCertificateAuthorityCsrRequestRequestTypeDef

```python
# GetCertificateAuthorityCsrRequestRequestTypeDef definition

class GetCertificateAuthorityCsrRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
```

## GetCertificateRequestRequestTypeDef

```python
# GetCertificateRequestRequestTypeDef definition

class GetCertificateRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    CertificateArn: str,
```

## GetPolicyRequestRequestTypeDef

```python
# GetPolicyRequestRequestTypeDef definition

class GetPolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ValidityTypeDef

```python
# ValidityTypeDef definition

class ValidityTypeDef(TypedDict):
    Value: int,
    Type: ValidityPeriodTypeType,  # (1)
```

1. See [:material-code-brackets: ValidityPeriodTypeType](./literals.md#validityperiodtypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListCertificateAuthoritiesRequestRequestTypeDef

```python
# ListCertificateAuthoritiesRequestRequestTypeDef definition

class ListCertificateAuthoritiesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ResourceOwner: NotRequired[ResourceOwnerType],  # (1)
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
## ListPermissionsRequestRequestTypeDef

```python
# ListPermissionsRequestRequestTypeDef definition

class ListPermissionsRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PermissionTypeDef

```python
# PermissionTypeDef definition

class PermissionTypeDef(TypedDict):
    CertificateAuthorityArn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    Principal: NotRequired[str],
    SourceAccount: NotRequired[str],
    Actions: NotRequired[List[ActionTypeType]],  # (1)
    Policy: NotRequired[str],
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
## ListTagsRequestRequestTypeDef

```python
# ListTagsRequestRequestTypeDef definition

class ListTagsRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## OcspConfigurationTypeDef

```python
# OcspConfigurationTypeDef definition

class OcspConfigurationTypeDef(TypedDict):
    Enabled: bool,
    OcspCustomCname: NotRequired[str],
```

## QualifierTypeDef

```python
# QualifierTypeDef definition

class QualifierTypeDef(TypedDict):
    CpsUri: str,
```

## PutPolicyRequestRequestTypeDef

```python
# PutPolicyRequestRequestTypeDef definition

class PutPolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
```

## RestoreCertificateAuthorityRequestRequestTypeDef

```python
# RestoreCertificateAuthorityRequestRequestTypeDef definition

class RestoreCertificateAuthorityRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
```

## RevokeCertificateRequestRequestTypeDef

```python
# RevokeCertificateRequestRequestTypeDef definition

class RevokeCertificateRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    CertificateSerial: str,
    RevocationReason: RevocationReasonType,  # (1)
```

1. See [:material-code-brackets: RevocationReasonType](./literals.md#revocationreasontype) 
## ASN1SubjectTypeDef

```python
# ASN1SubjectTypeDef definition

class ASN1SubjectTypeDef(TypedDict):
    Country: NotRequired[str],
    Organization: NotRequired[str],
    OrganizationalUnit: NotRequired[str],
    DistinguishedNameQualifier: NotRequired[str],
    State: NotRequired[str],
    CommonName: NotRequired[str],
    SerialNumber: NotRequired[str],
    Locality: NotRequired[str],
    Title: NotRequired[str],
    Surname: NotRequired[str],
    GivenName: NotRequired[str],
    Initials: NotRequired[str],
    Pseudonym: NotRequired[str],
    GenerationQualifier: NotRequired[str],
    CustomAttributes: NotRequired[Sequence[CustomAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: CustomAttributeTypeDef](./type_defs.md#customattributetypedef) 
## ImportCertificateAuthorityCertificateRequestRequestTypeDef

```python
# ImportCertificateAuthorityCertificateRequestRequestTypeDef definition

class ImportCertificateAuthorityCertificateRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    Certificate: Union[str, bytes, IO[Any], StreamingBody],
    CertificateChain: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
```

## CreateCertificateAuthorityAuditReportResponseTypeDef

```python
# CreateCertificateAuthorityAuditReportResponseTypeDef definition

class CreateCertificateAuthorityAuditReportResponseTypeDef(TypedDict):
    AuditReportId: str,
    S3Key: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCertificateAuthorityResponseTypeDef

```python
# CreateCertificateAuthorityResponseTypeDef definition

class CreateCertificateAuthorityResponseTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCertificateAuthorityAuditReportResponseTypeDef

```python
# DescribeCertificateAuthorityAuditReportResponseTypeDef definition

class DescribeCertificateAuthorityAuditReportResponseTypeDef(TypedDict):
    AuditReportStatus: AuditReportStatusType,  # (1)
    S3BucketName: str,
    S3Key: str,
    CreatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AuditReportStatusType](./literals.md#auditreportstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCertificateAuthorityCertificateResponseTypeDef

```python
# GetCertificateAuthorityCertificateResponseTypeDef definition

class GetCertificateAuthorityCertificateResponseTypeDef(TypedDict):
    Certificate: str,
    CertificateChain: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCertificateAuthorityCsrResponseTypeDef

```python
# GetCertificateAuthorityCsrResponseTypeDef definition

class GetCertificateAuthorityCsrResponseTypeDef(TypedDict):
    Csr: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCertificateResponseTypeDef

```python
# GetCertificateResponseTypeDef definition

class GetCertificateResponseTypeDef(TypedDict):
    Certificate: str,
    CertificateChain: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPolicyResponseTypeDef

```python
# GetPolicyResponseTypeDef definition

class GetPolicyResponseTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IssueCertificateResponseTypeDef

```python
# IssueCertificateResponseTypeDef definition

class IssueCertificateResponseTypeDef(TypedDict):
    CertificateArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsResponseTypeDef

```python
# ListTagsResponseTypeDef definition

class ListTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagCertificateAuthorityRequestRequestTypeDef

```python
# TagCertificateAuthorityRequestRequestTypeDef definition

class TagCertificateAuthorityRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UntagCertificateAuthorityRequestRequestTypeDef

```python
# UntagCertificateAuthorityRequestRequestTypeDef definition

class UntagCertificateAuthorityRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef

```python
# DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef definition

class DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    AuditReportId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef

```python
# GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef definition

class GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetCertificateRequestCertificateIssuedWaitTypeDef

```python
# GetCertificateRequestCertificateIssuedWaitTypeDef definition

class GetCertificateRequestCertificateIssuedWaitTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    CertificateArn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef

```python
# ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef definition

class ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef(TypedDict):
    ResourceOwner: NotRequired[ResourceOwnerType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPermissionsRequestListPermissionsPaginateTypeDef

```python
# ListPermissionsRequestListPermissionsPaginateTypeDef definition

class ListPermissionsRequestListPermissionsPaginateTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsRequestListTagsPaginateTypeDef

```python
# ListTagsRequestListTagsPaginateTypeDef definition

class ListTagsRequestListTagsPaginateTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPermissionsResponseTypeDef

```python
# ListPermissionsResponseTypeDef definition

class ListPermissionsResponseTypeDef(TypedDict):
    Permissions: List[PermissionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionTypeDef](./type_defs.md#permissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RevocationConfigurationTypeDef

```python
# RevocationConfigurationTypeDef definition

class RevocationConfigurationTypeDef(TypedDict):
    CrlConfiguration: NotRequired[CrlConfigurationTypeDef],  # (1)
    OcspConfiguration: NotRequired[OcspConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: CrlConfigurationTypeDef](./type_defs.md#crlconfigurationtypedef) 
2. See [:material-code-braces: OcspConfigurationTypeDef](./type_defs.md#ocspconfigurationtypedef) 
## PolicyQualifierInfoTypeDef

```python
# PolicyQualifierInfoTypeDef definition

class PolicyQualifierInfoTypeDef(TypedDict):
    PolicyQualifierId: PolicyQualifierIdType,  # (1)
    Qualifier: QualifierTypeDef,  # (2)
```

1. See [:material-code-brackets: PolicyQualifierIdType](./literals.md#policyqualifieridtype) 
2. See [:material-code-braces: QualifierTypeDef](./type_defs.md#qualifiertypedef) 
## GeneralNameTypeDef

```python
# GeneralNameTypeDef definition

class GeneralNameTypeDef(TypedDict):
    OtherName: NotRequired[OtherNameTypeDef],  # (1)
    Rfc822Name: NotRequired[str],
    DnsName: NotRequired[str],
    DirectoryName: NotRequired[ASN1SubjectTypeDef],  # (2)
    EdiPartyName: NotRequired[EdiPartyNameTypeDef],  # (3)
    UniformResourceIdentifier: NotRequired[str],
    IpAddress: NotRequired[str],
    RegisteredId: NotRequired[str],
```

1. See [:material-code-braces: OtherNameTypeDef](./type_defs.md#othernametypedef) 
2. See [:material-code-braces: ASN1SubjectTypeDef](./type_defs.md#asn1subjecttypedef) 
3. See [:material-code-braces: EdiPartyNameTypeDef](./type_defs.md#edipartynametypedef) 
## UpdateCertificateAuthorityRequestRequestTypeDef

```python
# UpdateCertificateAuthorityRequestRequestTypeDef definition

class UpdateCertificateAuthorityRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    RevocationConfiguration: NotRequired[RevocationConfigurationTypeDef],  # (1)
    Status: NotRequired[CertificateAuthorityStatusType],  # (2)
```

1. See [:material-code-braces: RevocationConfigurationTypeDef](./type_defs.md#revocationconfigurationtypedef) 
2. See [:material-code-brackets: CertificateAuthorityStatusType](./literals.md#certificateauthoritystatustype) 
## PolicyInformationTypeDef

```python
# PolicyInformationTypeDef definition

class PolicyInformationTypeDef(TypedDict):
    CertPolicyId: str,
    PolicyQualifiers: NotRequired[Sequence[PolicyQualifierInfoTypeDef]],  # (1)
```

1. See [:material-code-braces: PolicyQualifierInfoTypeDef](./type_defs.md#policyqualifierinfotypedef) 
## AccessDescriptionTypeDef

```python
# AccessDescriptionTypeDef definition

class AccessDescriptionTypeDef(TypedDict):
    AccessMethod: AccessMethodTypeDef,  # (1)
    AccessLocation: GeneralNameTypeDef,  # (2)
```

1. See [:material-code-braces: AccessMethodTypeDef](./type_defs.md#accessmethodtypedef) 
2. See [:material-code-braces: GeneralNameTypeDef](./type_defs.md#generalnametypedef) 
## ExtensionsTypeDef

```python
# ExtensionsTypeDef definition

class ExtensionsTypeDef(TypedDict):
    CertificatePolicies: NotRequired[Sequence[PolicyInformationTypeDef]],  # (1)
    ExtendedKeyUsage: NotRequired[Sequence[ExtendedKeyUsageTypeDef]],  # (2)
    KeyUsage: NotRequired[KeyUsageTypeDef],  # (3)
    SubjectAlternativeNames: NotRequired[Sequence[GeneralNameTypeDef]],  # (4)
    CustomExtensions: NotRequired[Sequence[CustomExtensionTypeDef]],  # (5)
```

1. See [:material-code-braces: PolicyInformationTypeDef](./type_defs.md#policyinformationtypedef) 
2. See [:material-code-braces: ExtendedKeyUsageTypeDef](./type_defs.md#extendedkeyusagetypedef) 
3. See [:material-code-braces: KeyUsageTypeDef](./type_defs.md#keyusagetypedef) 
4. See [:material-code-braces: GeneralNameTypeDef](./type_defs.md#generalnametypedef) 
5. See [:material-code-braces: CustomExtensionTypeDef](./type_defs.md#customextensiontypedef) 
## CsrExtensionsTypeDef

```python
# CsrExtensionsTypeDef definition

class CsrExtensionsTypeDef(TypedDict):
    KeyUsage: NotRequired[KeyUsageTypeDef],  # (1)
    SubjectInformationAccess: NotRequired[Sequence[AccessDescriptionTypeDef]],  # (2)
```

1. See [:material-code-braces: KeyUsageTypeDef](./type_defs.md#keyusagetypedef) 
2. See [:material-code-braces: AccessDescriptionTypeDef](./type_defs.md#accessdescriptiontypedef) 
## ApiPassthroughTypeDef

```python
# ApiPassthroughTypeDef definition

class ApiPassthroughTypeDef(TypedDict):
    Extensions: NotRequired[ExtensionsTypeDef],  # (1)
    Subject: NotRequired[ASN1SubjectTypeDef],  # (2)
```

1. See [:material-code-braces: ExtensionsTypeDef](./type_defs.md#extensionstypedef) 
2. See [:material-code-braces: ASN1SubjectTypeDef](./type_defs.md#asn1subjecttypedef) 
## CertificateAuthorityConfigurationTypeDef

```python
# CertificateAuthorityConfigurationTypeDef definition

class CertificateAuthorityConfigurationTypeDef(TypedDict):
    KeyAlgorithm: KeyAlgorithmType,  # (1)
    SigningAlgorithm: SigningAlgorithmType,  # (2)
    Subject: ASN1SubjectTypeDef,  # (3)
    CsrExtensions: NotRequired[CsrExtensionsTypeDef],  # (4)
```

1. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype) 
2. See [:material-code-brackets: SigningAlgorithmType](./literals.md#signingalgorithmtype) 
3. See [:material-code-braces: ASN1SubjectTypeDef](./type_defs.md#asn1subjecttypedef) 
4. See [:material-code-braces: CsrExtensionsTypeDef](./type_defs.md#csrextensionstypedef) 
## IssueCertificateRequestRequestTypeDef

```python
# IssueCertificateRequestRequestTypeDef definition

class IssueCertificateRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    Csr: Union[str, bytes, IO[Any], StreamingBody],
    SigningAlgorithm: SigningAlgorithmType,  # (1)
    Validity: ValidityTypeDef,  # (2)
    ApiPassthrough: NotRequired[ApiPassthroughTypeDef],  # (3)
    TemplateArn: NotRequired[str],
    ValidityNotBefore: NotRequired[ValidityTypeDef],  # (2)
    IdempotencyToken: NotRequired[str],
```

1. See [:material-code-brackets: SigningAlgorithmType](./literals.md#signingalgorithmtype) 
2. See [:material-code-braces: ValidityTypeDef](./type_defs.md#validitytypedef) 
3. See [:material-code-braces: ApiPassthroughTypeDef](./type_defs.md#apipassthroughtypedef) 
4. See [:material-code-braces: ValidityTypeDef](./type_defs.md#validitytypedef) 
## CertificateAuthorityTypeDef

```python
# CertificateAuthorityTypeDef definition

class CertificateAuthorityTypeDef(TypedDict):
    Arn: NotRequired[str],
    OwnerAccount: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    LastStateChangeAt: NotRequired[datetime],
    Type: NotRequired[CertificateAuthorityTypeType],  # (1)
    Serial: NotRequired[str],
    Status: NotRequired[CertificateAuthorityStatusType],  # (2)
    NotBefore: NotRequired[datetime],
    NotAfter: NotRequired[datetime],
    FailureReason: NotRequired[FailureReasonType],  # (3)
    CertificateAuthorityConfiguration: NotRequired[CertificateAuthorityConfigurationTypeDef],  # (4)
    RevocationConfiguration: NotRequired[RevocationConfigurationTypeDef],  # (5)
    RestorableUntil: NotRequired[datetime],
    KeyStorageSecurityStandard: NotRequired[KeyStorageSecurityStandardType],  # (6)
    UsageMode: NotRequired[CertificateAuthorityUsageModeType],  # (7)
```

1. See [:material-code-brackets: CertificateAuthorityTypeType](./literals.md#certificateauthoritytypetype) 
2. See [:material-code-brackets: CertificateAuthorityStatusType](./literals.md#certificateauthoritystatustype) 
3. See [:material-code-brackets: FailureReasonType](./literals.md#failurereasontype) 
4. See [:material-code-braces: CertificateAuthorityConfigurationTypeDef](./type_defs.md#certificateauthorityconfigurationtypedef) 
5. See [:material-code-braces: RevocationConfigurationTypeDef](./type_defs.md#revocationconfigurationtypedef) 
6. See [:material-code-brackets: KeyStorageSecurityStandardType](./literals.md#keystoragesecuritystandardtype) 
7. See [:material-code-brackets: CertificateAuthorityUsageModeType](./literals.md#certificateauthorityusagemodetype) 
## CreateCertificateAuthorityRequestRequestTypeDef

```python
# CreateCertificateAuthorityRequestRequestTypeDef definition

class CreateCertificateAuthorityRequestRequestTypeDef(TypedDict):
    CertificateAuthorityConfiguration: CertificateAuthorityConfigurationTypeDef,  # (1)
    CertificateAuthorityType: CertificateAuthorityTypeType,  # (2)
    RevocationConfiguration: NotRequired[RevocationConfigurationTypeDef],  # (3)
    IdempotencyToken: NotRequired[str],
    KeyStorageSecurityStandard: NotRequired[KeyStorageSecurityStandardType],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
    UsageMode: NotRequired[CertificateAuthorityUsageModeType],  # (6)
```

1. See [:material-code-braces: CertificateAuthorityConfigurationTypeDef](./type_defs.md#certificateauthorityconfigurationtypedef) 
2. See [:material-code-brackets: CertificateAuthorityTypeType](./literals.md#certificateauthoritytypetype) 
3. See [:material-code-braces: RevocationConfigurationTypeDef](./type_defs.md#revocationconfigurationtypedef) 
4. See [:material-code-brackets: KeyStorageSecurityStandardType](./literals.md#keystoragesecuritystandardtype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-brackets: CertificateAuthorityUsageModeType](./literals.md#certificateauthorityusagemodetype) 
## DescribeCertificateAuthorityResponseTypeDef

```python
# DescribeCertificateAuthorityResponseTypeDef definition

class DescribeCertificateAuthorityResponseTypeDef(TypedDict):
    CertificateAuthority: CertificateAuthorityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateAuthorityTypeDef](./type_defs.md#certificateauthoritytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCertificateAuthoritiesResponseTypeDef

```python
# ListCertificateAuthoritiesResponseTypeDef definition

class ListCertificateAuthoritiesResponseTypeDef(TypedDict):
    CertificateAuthorities: List[CertificateAuthorityTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateAuthorityTypeDef](./type_defs.md#certificateauthoritytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
