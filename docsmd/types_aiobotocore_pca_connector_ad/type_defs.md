# Type definitions

> [Index](../README.md) > [PcaConnectorAd](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PcaConnectorAd](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#pcaconnectorad)
    type annotations stubs module [types-aiobotocore-pca-connector-ad](https://pypi.org/project/types-aiobotocore-pca-connector-ad/).

## PrivateKeyAttributesV2UnionTypeDef

```python
# PrivateKeyAttributesV2UnionTypeDef definition

PrivateKeyAttributesV2UnionTypeDef = Union[
    PrivateKeyAttributesV2TypeDef,  # (1)
    PrivateKeyAttributesV2OutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PrivateKeyAttributesV2TypeDef](./type_defs.md#privatekeyattributesv2typedef) 
2. See [:material-code-braces: PrivateKeyAttributesV2OutputTypeDef](./type_defs.md#privatekeyattributesv2outputtypedef) 

## ApplicationPoliciesUnionTypeDef

```python
# ApplicationPoliciesUnionTypeDef definition

ApplicationPoliciesUnionTypeDef = Union[
    ApplicationPoliciesTypeDef,  # (1)
    ApplicationPoliciesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ApplicationPoliciesTypeDef](./type_defs.md#applicationpoliciestypedef) 
2. See [:material-code-braces: ApplicationPoliciesOutputTypeDef](./type_defs.md#applicationpoliciesoutputtypedef) 

## PrivateKeyAttributesV3UnionTypeDef

```python
# PrivateKeyAttributesV3UnionTypeDef definition

PrivateKeyAttributesV3UnionTypeDef = Union[
    PrivateKeyAttributesV3TypeDef,  # (1)
    PrivateKeyAttributesV3OutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PrivateKeyAttributesV3TypeDef](./type_defs.md#privatekeyattributesv3typedef) 
2. See [:material-code-braces: PrivateKeyAttributesV3OutputTypeDef](./type_defs.md#privatekeyattributesv3outputtypedef) 

## PrivateKeyAttributesV4UnionTypeDef

```python
# PrivateKeyAttributesV4UnionTypeDef definition

PrivateKeyAttributesV4UnionTypeDef = Union[
    PrivateKeyAttributesV4TypeDef,  # (1)
    PrivateKeyAttributesV4OutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PrivateKeyAttributesV4TypeDef](./type_defs.md#privatekeyattributesv4typedef) 
2. See [:material-code-braces: PrivateKeyAttributesV4OutputTypeDef](./type_defs.md#privatekeyattributesv4outputtypedef) 

## ExtensionsV2UnionTypeDef

```python
# ExtensionsV2UnionTypeDef definition

ExtensionsV2UnionTypeDef = Union[
    ExtensionsV2TypeDef,  # (1)
    ExtensionsV2OutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ExtensionsV2TypeDef](./type_defs.md#extensionsv2typedef) 
2. See [:material-code-braces: ExtensionsV2OutputTypeDef](./type_defs.md#extensionsv2outputtypedef) 

## ExtensionsV3UnionTypeDef

```python
# ExtensionsV3UnionTypeDef definition

ExtensionsV3UnionTypeDef = Union[
    ExtensionsV3TypeDef,  # (1)
    ExtensionsV3OutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ExtensionsV3TypeDef](./type_defs.md#extensionsv3typedef) 
2. See [:material-code-braces: ExtensionsV3OutputTypeDef](./type_defs.md#extensionsv3outputtypedef) 

## ExtensionsV4UnionTypeDef

```python
# ExtensionsV4UnionTypeDef definition

ExtensionsV4UnionTypeDef = Union[
    ExtensionsV4TypeDef,  # (1)
    ExtensionsV4OutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ExtensionsV4TypeDef](./type_defs.md#extensionsv4typedef) 
2. See [:material-code-braces: ExtensionsV4OutputTypeDef](./type_defs.md#extensionsv4outputtypedef) 

## TemplateV2UnionTypeDef

```python
# TemplateV2UnionTypeDef definition

TemplateV2UnionTypeDef = Union[
    TemplateV2TypeDef,  # (1)
    TemplateV2OutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TemplateV2TypeDef](./type_defs.md#templatev2typedef) 
2. See [:material-code-braces: TemplateV2OutputTypeDef](./type_defs.md#templatev2outputtypedef) 

## TemplateV3UnionTypeDef

```python
# TemplateV3UnionTypeDef definition

TemplateV3UnionTypeDef = Union[
    TemplateV3TypeDef,  # (1)
    TemplateV3OutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TemplateV3TypeDef](./type_defs.md#templatev3typedef) 
2. See [:material-code-braces: TemplateV3OutputTypeDef](./type_defs.md#templatev3outputtypedef) 

## TemplateV4UnionTypeDef

```python
# TemplateV4UnionTypeDef definition

TemplateV4UnionTypeDef = Union[
    TemplateV4TypeDef,  # (1)
    TemplateV4OutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TemplateV4TypeDef](./type_defs.md#templatev4typedef) 
2. See [:material-code-braces: TemplateV4OutputTypeDef](./type_defs.md#templatev4outputtypedef) 



## AccessRightsTypeDef

```python
# AccessRightsTypeDef definition

class AccessRightsTypeDef(TypedDict):
    AutoEnroll: NotRequired[AccessRightType],  # (1)
    Enroll: NotRequired[AccessRightType],  # (1)
```

1. See [:material-code-brackets: AccessRightType](./literals.md#accessrighttype) 
2. See [:material-code-brackets: AccessRightType](./literals.md#accessrighttype) 
## ApplicationPolicyTypeDef

```python
# ApplicationPolicyTypeDef definition

class ApplicationPolicyTypeDef(TypedDict):
    PolicyObjectIdentifier: NotRequired[str],
    PolicyType: NotRequired[ApplicationPolicyTypeType],  # (1)
```

1. See [:material-code-brackets: ApplicationPolicyTypeType](./literals.md#applicationpolicytypetype) 
## ValidityPeriodTypeDef

```python
# ValidityPeriodTypeDef definition

class ValidityPeriodTypeDef(TypedDict):
    Period: int,
    PeriodType: ValidityPeriodTypeType,  # (1)
```

1. See [:material-code-brackets: ValidityPeriodTypeType](./literals.md#validityperiodtypetype) 
## VpcInformationOutputTypeDef

```python
# VpcInformationOutputTypeDef definition

class VpcInformationOutputTypeDef(TypedDict):
    SecurityGroupIds: List[str],
```

## VpcInformationTypeDef

```python
# VpcInformationTypeDef definition

class VpcInformationTypeDef(TypedDict):
    SecurityGroupIds: Sequence[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## CreateDirectoryRegistrationRequestRequestTypeDef

```python
# CreateDirectoryRegistrationRequestRequestTypeDef definition

class CreateDirectoryRegistrationRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## CreateServicePrincipalNameRequestRequestTypeDef

```python
# CreateServicePrincipalNameRequestRequestTypeDef definition

class CreateServicePrincipalNameRequestRequestTypeDef(TypedDict):
    ConnectorArn: str,
    DirectoryRegistrationArn: str,
    ClientToken: NotRequired[str],
```

## DeleteConnectorRequestRequestTypeDef

```python
# DeleteConnectorRequestRequestTypeDef definition

class DeleteConnectorRequestRequestTypeDef(TypedDict):
    ConnectorArn: str,
```

## DeleteDirectoryRegistrationRequestRequestTypeDef

```python
# DeleteDirectoryRegistrationRequestRequestTypeDef definition

class DeleteDirectoryRegistrationRequestRequestTypeDef(TypedDict):
    DirectoryRegistrationArn: str,
```

## DeleteServicePrincipalNameRequestRequestTypeDef

```python
# DeleteServicePrincipalNameRequestRequestTypeDef definition

class DeleteServicePrincipalNameRequestRequestTypeDef(TypedDict):
    ConnectorArn: str,
    DirectoryRegistrationArn: str,
```

## DeleteTemplateGroupAccessControlEntryRequestRequestTypeDef

```python
# DeleteTemplateGroupAccessControlEntryRequestRequestTypeDef definition

class DeleteTemplateGroupAccessControlEntryRequestRequestTypeDef(TypedDict):
    GroupSecurityIdentifier: str,
    TemplateArn: str,
```

## DeleteTemplateRequestRequestTypeDef

```python
# DeleteTemplateRequestRequestTypeDef definition

class DeleteTemplateRequestRequestTypeDef(TypedDict):
    TemplateArn: str,
```

## DirectoryRegistrationSummaryTypeDef

```python
# DirectoryRegistrationSummaryTypeDef definition

class DirectoryRegistrationSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    DirectoryId: NotRequired[str],
    Status: NotRequired[DirectoryRegistrationStatusType],  # (1)
    StatusReason: NotRequired[DirectoryRegistrationStatusReasonType],  # (2)
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: DirectoryRegistrationStatusType](./literals.md#directoryregistrationstatustype) 
2. See [:material-code-brackets: DirectoryRegistrationStatusReasonType](./literals.md#directoryregistrationstatusreasontype) 
## DirectoryRegistrationTypeDef

```python
# DirectoryRegistrationTypeDef definition

class DirectoryRegistrationTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    DirectoryId: NotRequired[str],
    Status: NotRequired[DirectoryRegistrationStatusType],  # (1)
    StatusReason: NotRequired[DirectoryRegistrationStatusReasonType],  # (2)
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: DirectoryRegistrationStatusType](./literals.md#directoryregistrationstatustype) 
2. See [:material-code-brackets: DirectoryRegistrationStatusReasonType](./literals.md#directoryregistrationstatusreasontype) 
## EnrollmentFlagsV2TypeDef

```python
# EnrollmentFlagsV2TypeDef definition

class EnrollmentFlagsV2TypeDef(TypedDict):
    EnableKeyReuseOnNtTokenKeysetStorageFull: NotRequired[bool],
    IncludeSymmetricAlgorithms: NotRequired[bool],
    NoSecurityExtension: NotRequired[bool],
    RemoveInvalidCertificateFromPersonalStore: NotRequired[bool],
    UserInteractionRequired: NotRequired[bool],
```

## EnrollmentFlagsV3TypeDef

```python
# EnrollmentFlagsV3TypeDef definition

class EnrollmentFlagsV3TypeDef(TypedDict):
    EnableKeyReuseOnNtTokenKeysetStorageFull: NotRequired[bool],
    IncludeSymmetricAlgorithms: NotRequired[bool],
    NoSecurityExtension: NotRequired[bool],
    RemoveInvalidCertificateFromPersonalStore: NotRequired[bool],
    UserInteractionRequired: NotRequired[bool],
```

## EnrollmentFlagsV4TypeDef

```python
# EnrollmentFlagsV4TypeDef definition

class EnrollmentFlagsV4TypeDef(TypedDict):
    EnableKeyReuseOnNtTokenKeysetStorageFull: NotRequired[bool],
    IncludeSymmetricAlgorithms: NotRequired[bool],
    NoSecurityExtension: NotRequired[bool],
    RemoveInvalidCertificateFromPersonalStore: NotRequired[bool],
    UserInteractionRequired: NotRequired[bool],
```

## GeneralFlagsV2TypeDef

```python
# GeneralFlagsV2TypeDef definition

class GeneralFlagsV2TypeDef(TypedDict):
    AutoEnrollment: NotRequired[bool],
    MachineType: NotRequired[bool],
```

## GeneralFlagsV3TypeDef

```python
# GeneralFlagsV3TypeDef definition

class GeneralFlagsV3TypeDef(TypedDict):
    AutoEnrollment: NotRequired[bool],
    MachineType: NotRequired[bool],
```

## GeneralFlagsV4TypeDef

```python
# GeneralFlagsV4TypeDef definition

class GeneralFlagsV4TypeDef(TypedDict):
    AutoEnrollment: NotRequired[bool],
    MachineType: NotRequired[bool],
```

## GetConnectorRequestRequestTypeDef

```python
# GetConnectorRequestRequestTypeDef definition

class GetConnectorRequestRequestTypeDef(TypedDict):
    ConnectorArn: str,
```

## GetDirectoryRegistrationRequestRequestTypeDef

```python
# GetDirectoryRegistrationRequestRequestTypeDef definition

class GetDirectoryRegistrationRequestRequestTypeDef(TypedDict):
    DirectoryRegistrationArn: str,
```

## GetServicePrincipalNameRequestRequestTypeDef

```python
# GetServicePrincipalNameRequestRequestTypeDef definition

class GetServicePrincipalNameRequestRequestTypeDef(TypedDict):
    ConnectorArn: str,
    DirectoryRegistrationArn: str,
```

## ServicePrincipalNameTypeDef

```python
# ServicePrincipalNameTypeDef definition

class ServicePrincipalNameTypeDef(TypedDict):
    ConnectorArn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    DirectoryRegistrationArn: NotRequired[str],
    Status: NotRequired[ServicePrincipalNameStatusType],  # (1)
    StatusReason: NotRequired[ServicePrincipalNameStatusReasonType],  # (2)
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: ServicePrincipalNameStatusType](./literals.md#serviceprincipalnamestatustype) 
2. See [:material-code-brackets: ServicePrincipalNameStatusReasonType](./literals.md#serviceprincipalnamestatusreasontype) 
## GetTemplateGroupAccessControlEntryRequestRequestTypeDef

```python
# GetTemplateGroupAccessControlEntryRequestRequestTypeDef definition

class GetTemplateGroupAccessControlEntryRequestRequestTypeDef(TypedDict):
    GroupSecurityIdentifier: str,
    TemplateArn: str,
```

## GetTemplateRequestRequestTypeDef

```python
# GetTemplateRequestRequestTypeDef definition

class GetTemplateRequestRequestTypeDef(TypedDict):
    TemplateArn: str,
```

## KeyUsageFlagsTypeDef

```python
# KeyUsageFlagsTypeDef definition

class KeyUsageFlagsTypeDef(TypedDict):
    DataEncipherment: NotRequired[bool],
    DigitalSignature: NotRequired[bool],
    KeyAgreement: NotRequired[bool],
    KeyEncipherment: NotRequired[bool],
    NonRepudiation: NotRequired[bool],
```

## KeyUsagePropertyFlagsTypeDef

```python
# KeyUsagePropertyFlagsTypeDef definition

class KeyUsagePropertyFlagsTypeDef(TypedDict):
    Decrypt: NotRequired[bool],
    KeyAgreement: NotRequired[bool],
    Sign: NotRequired[bool],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListConnectorsRequestRequestTypeDef

```python
# ListConnectorsRequestRequestTypeDef definition

class ListConnectorsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListDirectoryRegistrationsRequestRequestTypeDef

```python
# ListDirectoryRegistrationsRequestRequestTypeDef definition

class ListDirectoryRegistrationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListServicePrincipalNamesRequestRequestTypeDef

```python
# ListServicePrincipalNamesRequestRequestTypeDef definition

class ListServicePrincipalNamesRequestRequestTypeDef(TypedDict):
    DirectoryRegistrationArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ServicePrincipalNameSummaryTypeDef

```python
# ServicePrincipalNameSummaryTypeDef definition

class ServicePrincipalNameSummaryTypeDef(TypedDict):
    ConnectorArn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    DirectoryRegistrationArn: NotRequired[str],
    Status: NotRequired[ServicePrincipalNameStatusType],  # (1)
    StatusReason: NotRequired[ServicePrincipalNameStatusReasonType],  # (2)
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: ServicePrincipalNameStatusType](./literals.md#serviceprincipalnamestatustype) 
2. See [:material-code-brackets: ServicePrincipalNameStatusReasonType](./literals.md#serviceprincipalnamestatusreasontype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListTemplateGroupAccessControlEntriesRequestRequestTypeDef

```python
# ListTemplateGroupAccessControlEntriesRequestRequestTypeDef definition

class ListTemplateGroupAccessControlEntriesRequestRequestTypeDef(TypedDict):
    TemplateArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTemplatesRequestRequestTypeDef

```python
# ListTemplatesRequestRequestTypeDef definition

class ListTemplatesRequestRequestTypeDef(TypedDict):
    ConnectorArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PrivateKeyAttributesV2OutputTypeDef

```python
# PrivateKeyAttributesV2OutputTypeDef definition

class PrivateKeyAttributesV2OutputTypeDef(TypedDict):
    KeySpec: KeySpecType,  # (1)
    MinimalKeyLength: int,
    CryptoProviders: NotRequired[List[str]],
```

1. See [:material-code-brackets: KeySpecType](./literals.md#keyspectype) 
## PrivateKeyAttributesV2TypeDef

```python
# PrivateKeyAttributesV2TypeDef definition

class PrivateKeyAttributesV2TypeDef(TypedDict):
    KeySpec: KeySpecType,  # (1)
    MinimalKeyLength: int,
    CryptoProviders: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: KeySpecType](./literals.md#keyspectype) 
## PrivateKeyFlagsV2TypeDef

```python
# PrivateKeyFlagsV2TypeDef definition

class PrivateKeyFlagsV2TypeDef(TypedDict):
    ClientVersion: ClientCompatibilityV2Type,  # (1)
    ExportableKey: NotRequired[bool],
    StrongKeyProtectionRequired: NotRequired[bool],
```

1. See [:material-code-brackets: ClientCompatibilityV2Type](./literals.md#clientcompatibilityv2type) 
## PrivateKeyFlagsV3TypeDef

```python
# PrivateKeyFlagsV3TypeDef definition

class PrivateKeyFlagsV3TypeDef(TypedDict):
    ClientVersion: ClientCompatibilityV3Type,  # (1)
    ExportableKey: NotRequired[bool],
    RequireAlternateSignatureAlgorithm: NotRequired[bool],
    StrongKeyProtectionRequired: NotRequired[bool],
```

1. See [:material-code-brackets: ClientCompatibilityV3Type](./literals.md#clientcompatibilityv3type) 
## PrivateKeyFlagsV4TypeDef

```python
# PrivateKeyFlagsV4TypeDef definition

class PrivateKeyFlagsV4TypeDef(TypedDict):
    ClientVersion: ClientCompatibilityV4Type,  # (1)
    ExportableKey: NotRequired[bool],
    RequireAlternateSignatureAlgorithm: NotRequired[bool],
    RequireSameKeyRenewal: NotRequired[bool],
    StrongKeyProtectionRequired: NotRequired[bool],
    UseLegacyProvider: NotRequired[bool],
```

1. See [:material-code-brackets: ClientCompatibilityV4Type](./literals.md#clientcompatibilityv4type) 
## SubjectNameFlagsV2TypeDef

```python
# SubjectNameFlagsV2TypeDef definition

class SubjectNameFlagsV2TypeDef(TypedDict):
    RequireCommonName: NotRequired[bool],
    RequireDirectoryPath: NotRequired[bool],
    RequireDnsAsCn: NotRequired[bool],
    RequireEmail: NotRequired[bool],
    SanRequireDirectoryGuid: NotRequired[bool],
    SanRequireDns: NotRequired[bool],
    SanRequireDomainDns: NotRequired[bool],
    SanRequireEmail: NotRequired[bool],
    SanRequireSpn: NotRequired[bool],
    SanRequireUpn: NotRequired[bool],
```

## SubjectNameFlagsV3TypeDef

```python
# SubjectNameFlagsV3TypeDef definition

class SubjectNameFlagsV3TypeDef(TypedDict):
    RequireCommonName: NotRequired[bool],
    RequireDirectoryPath: NotRequired[bool],
    RequireDnsAsCn: NotRequired[bool],
    RequireEmail: NotRequired[bool],
    SanRequireDirectoryGuid: NotRequired[bool],
    SanRequireDns: NotRequired[bool],
    SanRequireDomainDns: NotRequired[bool],
    SanRequireEmail: NotRequired[bool],
    SanRequireSpn: NotRequired[bool],
    SanRequireUpn: NotRequired[bool],
```

## SubjectNameFlagsV4TypeDef

```python
# SubjectNameFlagsV4TypeDef definition

class SubjectNameFlagsV4TypeDef(TypedDict):
    RequireCommonName: NotRequired[bool],
    RequireDirectoryPath: NotRequired[bool],
    RequireDnsAsCn: NotRequired[bool],
    RequireEmail: NotRequired[bool],
    SanRequireDirectoryGuid: NotRequired[bool],
    SanRequireDns: NotRequired[bool],
    SanRequireDomainDns: NotRequired[bool],
    SanRequireEmail: NotRequired[bool],
    SanRequireSpn: NotRequired[bool],
    SanRequireUpn: NotRequired[bool],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## TemplateRevisionTypeDef

```python
# TemplateRevisionTypeDef definition

class TemplateRevisionTypeDef(TypedDict):
    MajorRevision: int,
    MinorRevision: int,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## AccessControlEntrySummaryTypeDef

```python
# AccessControlEntrySummaryTypeDef definition

class AccessControlEntrySummaryTypeDef(TypedDict):
    AccessRights: NotRequired[AccessRightsTypeDef],  # (1)
    CreatedAt: NotRequired[datetime],
    GroupDisplayName: NotRequired[str],
    GroupSecurityIdentifier: NotRequired[str],
    TemplateArn: NotRequired[str],
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: AccessRightsTypeDef](./type_defs.md#accessrightstypedef) 
## AccessControlEntryTypeDef

```python
# AccessControlEntryTypeDef definition

class AccessControlEntryTypeDef(TypedDict):
    AccessRights: NotRequired[AccessRightsTypeDef],  # (1)
    CreatedAt: NotRequired[datetime],
    GroupDisplayName: NotRequired[str],
    GroupSecurityIdentifier: NotRequired[str],
    TemplateArn: NotRequired[str],
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: AccessRightsTypeDef](./type_defs.md#accessrightstypedef) 
## CreateTemplateGroupAccessControlEntryRequestRequestTypeDef

```python
# CreateTemplateGroupAccessControlEntryRequestRequestTypeDef definition

class CreateTemplateGroupAccessControlEntryRequestRequestTypeDef(TypedDict):
    AccessRights: AccessRightsTypeDef,  # (1)
    GroupDisplayName: str,
    GroupSecurityIdentifier: str,
    TemplateArn: str,
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: AccessRightsTypeDef](./type_defs.md#accessrightstypedef) 
## UpdateTemplateGroupAccessControlEntryRequestRequestTypeDef

```python
# UpdateTemplateGroupAccessControlEntryRequestRequestTypeDef definition

class UpdateTemplateGroupAccessControlEntryRequestRequestTypeDef(TypedDict):
    GroupSecurityIdentifier: str,
    TemplateArn: str,
    AccessRights: NotRequired[AccessRightsTypeDef],  # (1)
    GroupDisplayName: NotRequired[str],
```

1. See [:material-code-braces: AccessRightsTypeDef](./type_defs.md#accessrightstypedef) 
## ApplicationPoliciesOutputTypeDef

```python
# ApplicationPoliciesOutputTypeDef definition

class ApplicationPoliciesOutputTypeDef(TypedDict):
    Policies: List[ApplicationPolicyTypeDef],  # (1)
    Critical: NotRequired[bool],
```

1. See [:material-code-braces: ApplicationPolicyTypeDef](./type_defs.md#applicationpolicytypedef) 
## ApplicationPoliciesTypeDef

```python
# ApplicationPoliciesTypeDef definition

class ApplicationPoliciesTypeDef(TypedDict):
    Policies: Sequence[ApplicationPolicyTypeDef],  # (1)
    Critical: NotRequired[bool],
```

1. See [:material-code-braces: ApplicationPolicyTypeDef](./type_defs.md#applicationpolicytypedef) 
## CertificateValidityTypeDef

```python
# CertificateValidityTypeDef definition

class CertificateValidityTypeDef(TypedDict):
    RenewalPeriod: ValidityPeriodTypeDef,  # (1)
    ValidityPeriod: ValidityPeriodTypeDef,  # (1)
```

1. See [:material-code-braces: ValidityPeriodTypeDef](./type_defs.md#validityperiodtypedef) 
2. See [:material-code-braces: ValidityPeriodTypeDef](./type_defs.md#validityperiodtypedef) 
## ConnectorSummaryTypeDef

```python
# ConnectorSummaryTypeDef definition

class ConnectorSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    CertificateAuthorityArn: NotRequired[str],
    CertificateEnrollmentPolicyServerEndpoint: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    DirectoryId: NotRequired[str],
    Status: NotRequired[ConnectorStatusType],  # (1)
    StatusReason: NotRequired[ConnectorStatusReasonType],  # (2)
    UpdatedAt: NotRequired[datetime],
    VpcInformation: NotRequired[VpcInformationOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: ConnectorStatusType](./literals.md#connectorstatustype) 
2. See [:material-code-brackets: ConnectorStatusReasonType](./literals.md#connectorstatusreasontype) 
3. See [:material-code-braces: VpcInformationOutputTypeDef](./type_defs.md#vpcinformationoutputtypedef) 
## ConnectorTypeDef

```python
# ConnectorTypeDef definition

class ConnectorTypeDef(TypedDict):
    Arn: NotRequired[str],
    CertificateAuthorityArn: NotRequired[str],
    CertificateEnrollmentPolicyServerEndpoint: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    DirectoryId: NotRequired[str],
    Status: NotRequired[ConnectorStatusType],  # (1)
    StatusReason: NotRequired[ConnectorStatusReasonType],  # (2)
    UpdatedAt: NotRequired[datetime],
    VpcInformation: NotRequired[VpcInformationOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: ConnectorStatusType](./literals.md#connectorstatustype) 
2. See [:material-code-brackets: ConnectorStatusReasonType](./literals.md#connectorstatusreasontype) 
3. See [:material-code-braces: VpcInformationOutputTypeDef](./type_defs.md#vpcinformationoutputtypedef) 
## CreateConnectorRequestRequestTypeDef

```python
# CreateConnectorRequestRequestTypeDef definition

class CreateConnectorRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    DirectoryId: str,
    VpcInformation: VpcInformationTypeDef,  # (1)
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: VpcInformationTypeDef](./type_defs.md#vpcinformationtypedef) 
## CreateConnectorResponseTypeDef

```python
# CreateConnectorResponseTypeDef definition

class CreateConnectorResponseTypeDef(TypedDict):
    ConnectorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDirectoryRegistrationResponseTypeDef

```python
# CreateDirectoryRegistrationResponseTypeDef definition

class CreateDirectoryRegistrationResponseTypeDef(TypedDict):
    DirectoryRegistrationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTemplateResponseTypeDef

```python
# CreateTemplateResponseTypeDef definition

class CreateTemplateResponseTypeDef(TypedDict):
    TemplateArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDirectoryRegistrationsResponseTypeDef

```python
# ListDirectoryRegistrationsResponseTypeDef definition

class ListDirectoryRegistrationsResponseTypeDef(TypedDict):
    DirectoryRegistrations: List[DirectoryRegistrationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DirectoryRegistrationSummaryTypeDef](./type_defs.md#directoryregistrationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDirectoryRegistrationResponseTypeDef

```python
# GetDirectoryRegistrationResponseTypeDef definition

class GetDirectoryRegistrationResponseTypeDef(TypedDict):
    DirectoryRegistration: DirectoryRegistrationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DirectoryRegistrationTypeDef](./type_defs.md#directoryregistrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServicePrincipalNameResponseTypeDef

```python
# GetServicePrincipalNameResponseTypeDef definition

class GetServicePrincipalNameResponseTypeDef(TypedDict):
    ServicePrincipalName: ServicePrincipalNameTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServicePrincipalNameTypeDef](./type_defs.md#serviceprincipalnametypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KeyUsageTypeDef

```python
# KeyUsageTypeDef definition

class KeyUsageTypeDef(TypedDict):
    UsageFlags: KeyUsageFlagsTypeDef,  # (1)
    Critical: NotRequired[bool],
```

1. See [:material-code-braces: KeyUsageFlagsTypeDef](./type_defs.md#keyusageflagstypedef) 
## KeyUsagePropertyTypeDef

```python
# KeyUsagePropertyTypeDef definition

class KeyUsagePropertyTypeDef(TypedDict):
    PropertyFlags: NotRequired[KeyUsagePropertyFlagsTypeDef],  # (1)
    PropertyType: NotRequired[KeyUsagePropertyTypeType],  # (2)
```

1. See [:material-code-braces: KeyUsagePropertyFlagsTypeDef](./type_defs.md#keyusagepropertyflagstypedef) 
2. See [:material-code-brackets: KeyUsagePropertyTypeType](./literals.md#keyusagepropertytypetype) 
## ListConnectorsRequestPaginateTypeDef

```python
# ListConnectorsRequestPaginateTypeDef definition

class ListConnectorsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDirectoryRegistrationsRequestPaginateTypeDef

```python
# ListDirectoryRegistrationsRequestPaginateTypeDef definition

class ListDirectoryRegistrationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicePrincipalNamesRequestPaginateTypeDef

```python
# ListServicePrincipalNamesRequestPaginateTypeDef definition

class ListServicePrincipalNamesRequestPaginateTypeDef(TypedDict):
    DirectoryRegistrationArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTemplateGroupAccessControlEntriesRequestPaginateTypeDef

```python
# ListTemplateGroupAccessControlEntriesRequestPaginateTypeDef definition

class ListTemplateGroupAccessControlEntriesRequestPaginateTypeDef(TypedDict):
    TemplateArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTemplatesRequestPaginateTypeDef

```python
# ListTemplatesRequestPaginateTypeDef definition

class ListTemplatesRequestPaginateTypeDef(TypedDict):
    ConnectorArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicePrincipalNamesResponseTypeDef

```python
# ListServicePrincipalNamesResponseTypeDef definition

class ListServicePrincipalNamesResponseTypeDef(TypedDict):
    ServicePrincipalNames: List[ServicePrincipalNameSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServicePrincipalNameSummaryTypeDef](./type_defs.md#serviceprincipalnamesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTemplateGroupAccessControlEntriesResponseTypeDef

```python
# ListTemplateGroupAccessControlEntriesResponseTypeDef definition

class ListTemplateGroupAccessControlEntriesResponseTypeDef(TypedDict):
    AccessControlEntries: List[AccessControlEntrySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccessControlEntrySummaryTypeDef](./type_defs.md#accesscontrolentrysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTemplateGroupAccessControlEntryResponseTypeDef

```python
# GetTemplateGroupAccessControlEntryResponseTypeDef definition

class GetTemplateGroupAccessControlEntryResponseTypeDef(TypedDict):
    AccessControlEntry: AccessControlEntryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessControlEntryTypeDef](./type_defs.md#accesscontrolentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConnectorsResponseTypeDef

```python
# ListConnectorsResponseTypeDef definition

class ListConnectorsResponseTypeDef(TypedDict):
    Connectors: List[ConnectorSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConnectorSummaryTypeDef](./type_defs.md#connectorsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConnectorResponseTypeDef

```python
# GetConnectorResponseTypeDef definition

class GetConnectorResponseTypeDef(TypedDict):
    Connector: ConnectorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectorTypeDef](./type_defs.md#connectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExtensionsV2OutputTypeDef

```python
# ExtensionsV2OutputTypeDef definition

class ExtensionsV2OutputTypeDef(TypedDict):
    KeyUsage: KeyUsageTypeDef,  # (2)
    ApplicationPolicies: NotRequired[ApplicationPoliciesOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ApplicationPoliciesOutputTypeDef](./type_defs.md#applicationpoliciesoutputtypedef) 
2. See [:material-code-braces: KeyUsageTypeDef](./type_defs.md#keyusagetypedef) 
## ExtensionsV3OutputTypeDef

```python
# ExtensionsV3OutputTypeDef definition

class ExtensionsV3OutputTypeDef(TypedDict):
    KeyUsage: KeyUsageTypeDef,  # (2)
    ApplicationPolicies: NotRequired[ApplicationPoliciesOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ApplicationPoliciesOutputTypeDef](./type_defs.md#applicationpoliciesoutputtypedef) 
2. See [:material-code-braces: KeyUsageTypeDef](./type_defs.md#keyusagetypedef) 
## ExtensionsV4OutputTypeDef

```python
# ExtensionsV4OutputTypeDef definition

class ExtensionsV4OutputTypeDef(TypedDict):
    KeyUsage: KeyUsageTypeDef,  # (2)
    ApplicationPolicies: NotRequired[ApplicationPoliciesOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ApplicationPoliciesOutputTypeDef](./type_defs.md#applicationpoliciesoutputtypedef) 
2. See [:material-code-braces: KeyUsageTypeDef](./type_defs.md#keyusagetypedef) 
## PrivateKeyAttributesV3OutputTypeDef

```python
# PrivateKeyAttributesV3OutputTypeDef definition

class PrivateKeyAttributesV3OutputTypeDef(TypedDict):
    Algorithm: PrivateKeyAlgorithmType,  # (1)
    KeySpec: KeySpecType,  # (2)
    KeyUsageProperty: KeyUsagePropertyTypeDef,  # (3)
    MinimalKeyLength: int,
    CryptoProviders: NotRequired[List[str]],
```

1. See [:material-code-brackets: PrivateKeyAlgorithmType](./literals.md#privatekeyalgorithmtype) 
2. See [:material-code-brackets: KeySpecType](./literals.md#keyspectype) 
3. See [:material-code-braces: KeyUsagePropertyTypeDef](./type_defs.md#keyusagepropertytypedef) 
## PrivateKeyAttributesV3TypeDef

```python
# PrivateKeyAttributesV3TypeDef definition

class PrivateKeyAttributesV3TypeDef(TypedDict):
    Algorithm: PrivateKeyAlgorithmType,  # (1)
    KeySpec: KeySpecType,  # (2)
    KeyUsageProperty: KeyUsagePropertyTypeDef,  # (3)
    MinimalKeyLength: int,
    CryptoProviders: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: PrivateKeyAlgorithmType](./literals.md#privatekeyalgorithmtype) 
2. See [:material-code-brackets: KeySpecType](./literals.md#keyspectype) 
3. See [:material-code-braces: KeyUsagePropertyTypeDef](./type_defs.md#keyusagepropertytypedef) 
## PrivateKeyAttributesV4OutputTypeDef

```python
# PrivateKeyAttributesV4OutputTypeDef definition

class PrivateKeyAttributesV4OutputTypeDef(TypedDict):
    KeySpec: KeySpecType,  # (2)
    MinimalKeyLength: int,
    Algorithm: NotRequired[PrivateKeyAlgorithmType],  # (1)
    CryptoProviders: NotRequired[List[str]],
    KeyUsageProperty: NotRequired[KeyUsagePropertyTypeDef],  # (3)
```

1. See [:material-code-brackets: PrivateKeyAlgorithmType](./literals.md#privatekeyalgorithmtype) 
2. See [:material-code-brackets: KeySpecType](./literals.md#keyspectype) 
3. See [:material-code-braces: KeyUsagePropertyTypeDef](./type_defs.md#keyusagepropertytypedef) 
## PrivateKeyAttributesV4TypeDef

```python
# PrivateKeyAttributesV4TypeDef definition

class PrivateKeyAttributesV4TypeDef(TypedDict):
    KeySpec: KeySpecType,  # (2)
    MinimalKeyLength: int,
    Algorithm: NotRequired[PrivateKeyAlgorithmType],  # (1)
    CryptoProviders: NotRequired[Sequence[str]],
    KeyUsageProperty: NotRequired[KeyUsagePropertyTypeDef],  # (3)
```

1. See [:material-code-brackets: PrivateKeyAlgorithmType](./literals.md#privatekeyalgorithmtype) 
2. See [:material-code-brackets: KeySpecType](./literals.md#keyspectype) 
3. See [:material-code-braces: KeyUsagePropertyTypeDef](./type_defs.md#keyusagepropertytypedef) 
## ExtensionsV2TypeDef

```python
# ExtensionsV2TypeDef definition

class ExtensionsV2TypeDef(TypedDict):
    KeyUsage: KeyUsageTypeDef,  # (2)
    ApplicationPolicies: NotRequired[ApplicationPoliciesUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ApplicationPoliciesTypeDef](./type_defs.md#applicationpoliciestypedef) [:material-code-braces: ApplicationPoliciesOutputTypeDef](./type_defs.md#applicationpoliciesoutputtypedef) 
2. See [:material-code-braces: KeyUsageTypeDef](./type_defs.md#keyusagetypedef) 
## ExtensionsV3TypeDef

```python
# ExtensionsV3TypeDef definition

class ExtensionsV3TypeDef(TypedDict):
    KeyUsage: KeyUsageTypeDef,  # (2)
    ApplicationPolicies: NotRequired[ApplicationPoliciesUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ApplicationPoliciesTypeDef](./type_defs.md#applicationpoliciestypedef) [:material-code-braces: ApplicationPoliciesOutputTypeDef](./type_defs.md#applicationpoliciesoutputtypedef) 
2. See [:material-code-braces: KeyUsageTypeDef](./type_defs.md#keyusagetypedef) 
## ExtensionsV4TypeDef

```python
# ExtensionsV4TypeDef definition

class ExtensionsV4TypeDef(TypedDict):
    KeyUsage: KeyUsageTypeDef,  # (2)
    ApplicationPolicies: NotRequired[ApplicationPoliciesUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ApplicationPoliciesTypeDef](./type_defs.md#applicationpoliciestypedef) [:material-code-braces: ApplicationPoliciesOutputTypeDef](./type_defs.md#applicationpoliciesoutputtypedef) 
2. See [:material-code-braces: KeyUsageTypeDef](./type_defs.md#keyusagetypedef) 
## TemplateV2OutputTypeDef

```python
# TemplateV2OutputTypeDef definition

class TemplateV2OutputTypeDef(TypedDict):
    CertificateValidity: CertificateValidityTypeDef,  # (1)
    EnrollmentFlags: EnrollmentFlagsV2TypeDef,  # (2)
    Extensions: ExtensionsV2OutputTypeDef,  # (3)
    GeneralFlags: GeneralFlagsV2TypeDef,  # (4)
    PrivateKeyAttributes: PrivateKeyAttributesV2OutputTypeDef,  # (5)
    PrivateKeyFlags: PrivateKeyFlagsV2TypeDef,  # (6)
    SubjectNameFlags: SubjectNameFlagsV2TypeDef,  # (7)
    SupersededTemplates: NotRequired[List[str]],
```

1. See [:material-code-braces: CertificateValidityTypeDef](./type_defs.md#certificatevaliditytypedef) 
2. See [:material-code-braces: EnrollmentFlagsV2TypeDef](./type_defs.md#enrollmentflagsv2typedef) 
3. See [:material-code-braces: ExtensionsV2OutputTypeDef](./type_defs.md#extensionsv2outputtypedef) 
4. See [:material-code-braces: GeneralFlagsV2TypeDef](./type_defs.md#generalflagsv2typedef) 
5. See [:material-code-braces: PrivateKeyAttributesV2OutputTypeDef](./type_defs.md#privatekeyattributesv2outputtypedef) 
6. See [:material-code-braces: PrivateKeyFlagsV2TypeDef](./type_defs.md#privatekeyflagsv2typedef) 
7. See [:material-code-braces: SubjectNameFlagsV2TypeDef](./type_defs.md#subjectnameflagsv2typedef) 
## TemplateV3OutputTypeDef

```python
# TemplateV3OutputTypeDef definition

class TemplateV3OutputTypeDef(TypedDict):
    CertificateValidity: CertificateValidityTypeDef,  # (1)
    EnrollmentFlags: EnrollmentFlagsV3TypeDef,  # (2)
    Extensions: ExtensionsV3OutputTypeDef,  # (3)
    GeneralFlags: GeneralFlagsV3TypeDef,  # (4)
    HashAlgorithm: HashAlgorithmType,  # (5)
    PrivateKeyAttributes: PrivateKeyAttributesV3OutputTypeDef,  # (6)
    PrivateKeyFlags: PrivateKeyFlagsV3TypeDef,  # (7)
    SubjectNameFlags: SubjectNameFlagsV3TypeDef,  # (8)
    SupersededTemplates: NotRequired[List[str]],
```

1. See [:material-code-braces: CertificateValidityTypeDef](./type_defs.md#certificatevaliditytypedef) 
2. See [:material-code-braces: EnrollmentFlagsV3TypeDef](./type_defs.md#enrollmentflagsv3typedef) 
3. See [:material-code-braces: ExtensionsV3OutputTypeDef](./type_defs.md#extensionsv3outputtypedef) 
4. See [:material-code-braces: GeneralFlagsV3TypeDef](./type_defs.md#generalflagsv3typedef) 
5. See [:material-code-brackets: HashAlgorithmType](./literals.md#hashalgorithmtype) 
6. See [:material-code-braces: PrivateKeyAttributesV3OutputTypeDef](./type_defs.md#privatekeyattributesv3outputtypedef) 
7. See [:material-code-braces: PrivateKeyFlagsV3TypeDef](./type_defs.md#privatekeyflagsv3typedef) 
8. See [:material-code-braces: SubjectNameFlagsV3TypeDef](./type_defs.md#subjectnameflagsv3typedef) 
## TemplateV4OutputTypeDef

```python
# TemplateV4OutputTypeDef definition

class TemplateV4OutputTypeDef(TypedDict):
    CertificateValidity: CertificateValidityTypeDef,  # (1)
    EnrollmentFlags: EnrollmentFlagsV4TypeDef,  # (2)
    Extensions: ExtensionsV4OutputTypeDef,  # (3)
    GeneralFlags: GeneralFlagsV4TypeDef,  # (4)
    PrivateKeyAttributes: PrivateKeyAttributesV4OutputTypeDef,  # (6)
    PrivateKeyFlags: PrivateKeyFlagsV4TypeDef,  # (7)
    SubjectNameFlags: SubjectNameFlagsV4TypeDef,  # (8)
    HashAlgorithm: NotRequired[HashAlgorithmType],  # (5)
    SupersededTemplates: NotRequired[List[str]],
```

1. See [:material-code-braces: CertificateValidityTypeDef](./type_defs.md#certificatevaliditytypedef) 
2. See [:material-code-braces: EnrollmentFlagsV4TypeDef](./type_defs.md#enrollmentflagsv4typedef) 
3. See [:material-code-braces: ExtensionsV4OutputTypeDef](./type_defs.md#extensionsv4outputtypedef) 
4. See [:material-code-braces: GeneralFlagsV4TypeDef](./type_defs.md#generalflagsv4typedef) 
5. See [:material-code-brackets: HashAlgorithmType](./literals.md#hashalgorithmtype) 
6. See [:material-code-braces: PrivateKeyAttributesV4OutputTypeDef](./type_defs.md#privatekeyattributesv4outputtypedef) 
7. See [:material-code-braces: PrivateKeyFlagsV4TypeDef](./type_defs.md#privatekeyflagsv4typedef) 
8. See [:material-code-braces: SubjectNameFlagsV4TypeDef](./type_defs.md#subjectnameflagsv4typedef) 
## TemplateDefinitionOutputTypeDef

```python
# TemplateDefinitionOutputTypeDef definition

class TemplateDefinitionOutputTypeDef(TypedDict):
    TemplateV2: NotRequired[TemplateV2OutputTypeDef],  # (1)
    TemplateV3: NotRequired[TemplateV3OutputTypeDef],  # (2)
    TemplateV4: NotRequired[TemplateV4OutputTypeDef],  # (3)
```

1. See [:material-code-braces: TemplateV2OutputTypeDef](./type_defs.md#templatev2outputtypedef) 
2. See [:material-code-braces: TemplateV3OutputTypeDef](./type_defs.md#templatev3outputtypedef) 
3. See [:material-code-braces: TemplateV4OutputTypeDef](./type_defs.md#templatev4outputtypedef) 
## TemplateV2TypeDef

```python
# TemplateV2TypeDef definition

class TemplateV2TypeDef(TypedDict):
    CertificateValidity: CertificateValidityTypeDef,  # (1)
    EnrollmentFlags: EnrollmentFlagsV2TypeDef,  # (2)
    Extensions: ExtensionsV2UnionTypeDef,  # (3)
    GeneralFlags: GeneralFlagsV2TypeDef,  # (4)
    PrivateKeyAttributes: PrivateKeyAttributesV2UnionTypeDef,  # (5)
    PrivateKeyFlags: PrivateKeyFlagsV2TypeDef,  # (6)
    SubjectNameFlags: SubjectNameFlagsV2TypeDef,  # (7)
    SupersededTemplates: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: CertificateValidityTypeDef](./type_defs.md#certificatevaliditytypedef) 
2. See [:material-code-braces: EnrollmentFlagsV2TypeDef](./type_defs.md#enrollmentflagsv2typedef) 
3. See [:material-code-braces: ExtensionsV2TypeDef](./type_defs.md#extensionsv2typedef) [:material-code-braces: ExtensionsV2OutputTypeDef](./type_defs.md#extensionsv2outputtypedef) 
4. See [:material-code-braces: GeneralFlagsV2TypeDef](./type_defs.md#generalflagsv2typedef) 
5. See [:material-code-braces: PrivateKeyAttributesV2TypeDef](./type_defs.md#privatekeyattributesv2typedef) [:material-code-braces: PrivateKeyAttributesV2OutputTypeDef](./type_defs.md#privatekeyattributesv2outputtypedef) 
6. See [:material-code-braces: PrivateKeyFlagsV2TypeDef](./type_defs.md#privatekeyflagsv2typedef) 
7. See [:material-code-braces: SubjectNameFlagsV2TypeDef](./type_defs.md#subjectnameflagsv2typedef) 
## TemplateV3TypeDef

```python
# TemplateV3TypeDef definition

class TemplateV3TypeDef(TypedDict):
    CertificateValidity: CertificateValidityTypeDef,  # (1)
    EnrollmentFlags: EnrollmentFlagsV3TypeDef,  # (2)
    Extensions: ExtensionsV3UnionTypeDef,  # (3)
    GeneralFlags: GeneralFlagsV3TypeDef,  # (4)
    HashAlgorithm: HashAlgorithmType,  # (5)
    PrivateKeyAttributes: PrivateKeyAttributesV3UnionTypeDef,  # (6)
    PrivateKeyFlags: PrivateKeyFlagsV3TypeDef,  # (7)
    SubjectNameFlags: SubjectNameFlagsV3TypeDef,  # (8)
    SupersededTemplates: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: CertificateValidityTypeDef](./type_defs.md#certificatevaliditytypedef) 
2. See [:material-code-braces: EnrollmentFlagsV3TypeDef](./type_defs.md#enrollmentflagsv3typedef) 
3. See [:material-code-braces: ExtensionsV3TypeDef](./type_defs.md#extensionsv3typedef) [:material-code-braces: ExtensionsV3OutputTypeDef](./type_defs.md#extensionsv3outputtypedef) 
4. See [:material-code-braces: GeneralFlagsV3TypeDef](./type_defs.md#generalflagsv3typedef) 
5. See [:material-code-brackets: HashAlgorithmType](./literals.md#hashalgorithmtype) 
6. See [:material-code-braces: PrivateKeyAttributesV3TypeDef](./type_defs.md#privatekeyattributesv3typedef) [:material-code-braces: PrivateKeyAttributesV3OutputTypeDef](./type_defs.md#privatekeyattributesv3outputtypedef) 
7. See [:material-code-braces: PrivateKeyFlagsV3TypeDef](./type_defs.md#privatekeyflagsv3typedef) 
8. See [:material-code-braces: SubjectNameFlagsV3TypeDef](./type_defs.md#subjectnameflagsv3typedef) 
## TemplateV4TypeDef

```python
# TemplateV4TypeDef definition

class TemplateV4TypeDef(TypedDict):
    CertificateValidity: CertificateValidityTypeDef,  # (1)
    EnrollmentFlags: EnrollmentFlagsV4TypeDef,  # (2)
    Extensions: ExtensionsV4UnionTypeDef,  # (3)
    GeneralFlags: GeneralFlagsV4TypeDef,  # (4)
    PrivateKeyAttributes: PrivateKeyAttributesV4UnionTypeDef,  # (6)
    PrivateKeyFlags: PrivateKeyFlagsV4TypeDef,  # (7)
    SubjectNameFlags: SubjectNameFlagsV4TypeDef,  # (8)
    HashAlgorithm: NotRequired[HashAlgorithmType],  # (5)
    SupersededTemplates: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: CertificateValidityTypeDef](./type_defs.md#certificatevaliditytypedef) 
2. See [:material-code-braces: EnrollmentFlagsV4TypeDef](./type_defs.md#enrollmentflagsv4typedef) 
3. See [:material-code-braces: ExtensionsV4TypeDef](./type_defs.md#extensionsv4typedef) [:material-code-braces: ExtensionsV4OutputTypeDef](./type_defs.md#extensionsv4outputtypedef) 
4. See [:material-code-braces: GeneralFlagsV4TypeDef](./type_defs.md#generalflagsv4typedef) 
5. See [:material-code-brackets: HashAlgorithmType](./literals.md#hashalgorithmtype) 
6. See [:material-code-braces: PrivateKeyAttributesV4TypeDef](./type_defs.md#privatekeyattributesv4typedef) [:material-code-braces: PrivateKeyAttributesV4OutputTypeDef](./type_defs.md#privatekeyattributesv4outputtypedef) 
7. See [:material-code-braces: PrivateKeyFlagsV4TypeDef](./type_defs.md#privatekeyflagsv4typedef) 
8. See [:material-code-braces: SubjectNameFlagsV4TypeDef](./type_defs.md#subjectnameflagsv4typedef) 
## TemplateSummaryTypeDef

```python
# TemplateSummaryTypeDef definition

class TemplateSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    ConnectorArn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    Definition: NotRequired[TemplateDefinitionOutputTypeDef],  # (1)
    Name: NotRequired[str],
    ObjectIdentifier: NotRequired[str],
    PolicySchema: NotRequired[int],
    Revision: NotRequired[TemplateRevisionTypeDef],  # (2)
    Status: NotRequired[TemplateStatusType],  # (3)
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: TemplateDefinitionOutputTypeDef](./type_defs.md#templatedefinitionoutputtypedef) 
2. See [:material-code-braces: TemplateRevisionTypeDef](./type_defs.md#templaterevisiontypedef) 
3. See [:material-code-brackets: TemplateStatusType](./literals.md#templatestatustype) 
## TemplateTypeDef

```python
# TemplateTypeDef definition

class TemplateTypeDef(TypedDict):
    Arn: NotRequired[str],
    ConnectorArn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    Definition: NotRequired[TemplateDefinitionOutputTypeDef],  # (1)
    Name: NotRequired[str],
    ObjectIdentifier: NotRequired[str],
    PolicySchema: NotRequired[int],
    Revision: NotRequired[TemplateRevisionTypeDef],  # (2)
    Status: NotRequired[TemplateStatusType],  # (3)
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: TemplateDefinitionOutputTypeDef](./type_defs.md#templatedefinitionoutputtypedef) 
2. See [:material-code-braces: TemplateRevisionTypeDef](./type_defs.md#templaterevisiontypedef) 
3. See [:material-code-brackets: TemplateStatusType](./literals.md#templatestatustype) 
## ListTemplatesResponseTypeDef

```python
# ListTemplatesResponseTypeDef definition

class ListTemplatesResponseTypeDef(TypedDict):
    Templates: List[TemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TemplateSummaryTypeDef](./type_defs.md#templatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTemplateResponseTypeDef

```python
# GetTemplateResponseTypeDef definition

class GetTemplateResponseTypeDef(TypedDict):
    Template: TemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TemplateDefinitionTypeDef

```python
# TemplateDefinitionTypeDef definition

class TemplateDefinitionTypeDef(TypedDict):
    TemplateV2: NotRequired[TemplateV2UnionTypeDef],  # (1)
    TemplateV3: NotRequired[TemplateV3UnionTypeDef],  # (2)
    TemplateV4: NotRequired[TemplateV4UnionTypeDef],  # (3)
```

1. See [:material-code-braces: TemplateV2TypeDef](./type_defs.md#templatev2typedef) [:material-code-braces: TemplateV2OutputTypeDef](./type_defs.md#templatev2outputtypedef) 
2. See [:material-code-braces: TemplateV3TypeDef](./type_defs.md#templatev3typedef) [:material-code-braces: TemplateV3OutputTypeDef](./type_defs.md#templatev3outputtypedef) 
3. See [:material-code-braces: TemplateV4TypeDef](./type_defs.md#templatev4typedef) [:material-code-braces: TemplateV4OutputTypeDef](./type_defs.md#templatev4outputtypedef) 
## CreateTemplateRequestRequestTypeDef

```python
# CreateTemplateRequestRequestTypeDef definition

class CreateTemplateRequestRequestTypeDef(TypedDict):
    ConnectorArn: str,
    Definition: TemplateDefinitionTypeDef,  # (1)
    Name: str,
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: TemplateDefinitionTypeDef](./type_defs.md#templatedefinitiontypedef) 
## UpdateTemplateRequestRequestTypeDef

```python
# UpdateTemplateRequestRequestTypeDef definition

class UpdateTemplateRequestRequestTypeDef(TypedDict):
    TemplateArn: str,
    Definition: NotRequired[TemplateDefinitionTypeDef],  # (1)
    ReenrollAllCertificateHolders: NotRequired[bool],
```

1. See [:material-code-braces: TemplateDefinitionTypeDef](./type_defs.md#templatedefinitiontypedef) 
