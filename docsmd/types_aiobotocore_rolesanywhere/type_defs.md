# Type definitions

> [Index](../README.md) > [IAMRolesAnywhere](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IAMRolesAnywhere](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
    type annotations stubs module [types-aiobotocore-rolesanywhere](https://pypi.org/project/types-aiobotocore-rolesanywhere/).

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




## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## NotificationSettingTypeDef

```python
# NotificationSettingTypeDef definition

class NotificationSettingTypeDef(TypedDict):
    enabled: bool,
    event: NotificationEventType,  # (2)
    channel: NotRequired[NotificationChannelType],  # (1)
    threshold: NotRequired[int],
```

1. See [:material-code-brackets: NotificationChannelType](./literals.md#notificationchanneltype) 
2. See [:material-code-brackets: NotificationEventType](./literals.md#notificationeventtype) 
## CredentialSummaryTypeDef

```python
# CredentialSummaryTypeDef definition

class CredentialSummaryTypeDef(TypedDict):
    enabled: NotRequired[bool],
    failed: NotRequired[bool],
    issuer: NotRequired[str],
    seenAt: NotRequired[datetime],
    serialNumber: NotRequired[str],
    x509CertificateData: NotRequired[str],
```

## CrlDetailTypeDef

```python
# CrlDetailTypeDef definition

class CrlDetailTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    crlArn: NotRequired[str],
    crlData: NotRequired[bytes],
    crlId: NotRequired[str],
    enabled: NotRequired[bool],
    name: NotRequired[str],
    trustAnchorArn: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

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

## InstancePropertyTypeDef

```python
# InstancePropertyTypeDef definition

class InstancePropertyTypeDef(TypedDict):
    failed: NotRequired[bool],
    properties: NotRequired[Dict[str, str]],
    seenAt: NotRequired[datetime],
```

## ProfileDetailTypeDef

```python
# ProfileDetailTypeDef definition

class ProfileDetailTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    durationSeconds: NotRequired[int],
    enabled: NotRequired[bool],
    managedPolicyArns: NotRequired[List[str]],
    name: NotRequired[str],
    profileArn: NotRequired[str],
    profileId: NotRequired[str],
    requireInstanceProperties: NotRequired[bool],
    roleArns: NotRequired[List[str]],
    sessionPolicy: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListRequestRequestTypeDef

```python
# ListRequestRequestTypeDef definition

class ListRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    pageSize: NotRequired[int],
```

## SubjectSummaryTypeDef

```python
# SubjectSummaryTypeDef definition

class SubjectSummaryTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    enabled: NotRequired[bool],
    lastSeenAt: NotRequired[datetime],
    subjectArn: NotRequired[str],
    subjectId: NotRequired[str],
    updatedAt: NotRequired[datetime],
    x509Subject: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## NotificationSettingDetailTypeDef

```python
# NotificationSettingDetailTypeDef definition

class NotificationSettingDetailTypeDef(TypedDict):
    enabled: bool,
    event: NotificationEventType,  # (2)
    channel: NotRequired[NotificationChannelType],  # (1)
    configuredBy: NotRequired[str],
    threshold: NotRequired[int],
```

1. See [:material-code-brackets: NotificationChannelType](./literals.md#notificationchanneltype) 
2. See [:material-code-brackets: NotificationEventType](./literals.md#notificationeventtype) 
## NotificationSettingKeyTypeDef

```python
# NotificationSettingKeyTypeDef definition

class NotificationSettingKeyTypeDef(TypedDict):
    event: NotificationEventType,  # (2)
    channel: NotRequired[NotificationChannelType],  # (1)
```

1. See [:material-code-brackets: NotificationChannelType](./literals.md#notificationchanneltype) 
2. See [:material-code-brackets: NotificationEventType](./literals.md#notificationeventtype) 
## ScalarCrlRequestRequestTypeDef

```python
# ScalarCrlRequestRequestTypeDef definition

class ScalarCrlRequestRequestTypeDef(TypedDict):
    crlId: str,
```

## ScalarProfileRequestRequestTypeDef

```python
# ScalarProfileRequestRequestTypeDef definition

class ScalarProfileRequestRequestTypeDef(TypedDict):
    profileId: str,
```

## ScalarSubjectRequestRequestTypeDef

```python
# ScalarSubjectRequestRequestTypeDef definition

class ScalarSubjectRequestRequestTypeDef(TypedDict):
    subjectId: str,
```

## ScalarTrustAnchorRequestRequestTypeDef

```python
# ScalarTrustAnchorRequestRequestTypeDef definition

class ScalarTrustAnchorRequestRequestTypeDef(TypedDict):
    trustAnchorId: str,
```

## SourceDataTypeDef

```python
# SourceDataTypeDef definition

class SourceDataTypeDef(TypedDict):
    acmPcaArn: NotRequired[str],
    x509CertificateData: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateProfileRequestRequestTypeDef

```python
# UpdateProfileRequestRequestTypeDef definition

class UpdateProfileRequestRequestTypeDef(TypedDict):
    profileId: str,
    durationSeconds: NotRequired[int],
    managedPolicyArns: NotRequired[Sequence[str]],
    name: NotRequired[str],
    roleArns: NotRequired[Sequence[str]],
    sessionPolicy: NotRequired[str],
```

## UpdateCrlRequestRequestTypeDef

```python
# UpdateCrlRequestRequestTypeDef definition

class UpdateCrlRequestRequestTypeDef(TypedDict):
    crlId: str,
    crlData: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    name: NotRequired[str],
```

## CreateProfileRequestRequestTypeDef

```python
# CreateProfileRequestRequestTypeDef definition

class CreateProfileRequestRequestTypeDef(TypedDict):
    name: str,
    roleArns: Sequence[str],
    durationSeconds: NotRequired[int],
    enabled: NotRequired[bool],
    managedPolicyArns: NotRequired[Sequence[str]],
    requireInstanceProperties: NotRequired[bool],
    sessionPolicy: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ImportCrlRequestRequestTypeDef

```python
# ImportCrlRequestRequestTypeDef definition

class ImportCrlRequestRequestTypeDef(TypedDict):
    crlData: Union[str, bytes, IO[Any], StreamingBody],
    name: str,
    trustAnchorArn: str,
    enabled: NotRequired[bool],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutNotificationSettingsRequestRequestTypeDef

```python
# PutNotificationSettingsRequestRequestTypeDef definition

class PutNotificationSettingsRequestRequestTypeDef(TypedDict):
    notificationSettings: Sequence[NotificationSettingTypeDef],  # (1)
    trustAnchorId: str,
```

1. See [:material-code-braces: NotificationSettingTypeDef](./type_defs.md#notificationsettingtypedef) 
## CrlDetailResponseTypeDef

```python
# CrlDetailResponseTypeDef definition

class CrlDetailResponseTypeDef(TypedDict):
    crl: CrlDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CrlDetailTypeDef](./type_defs.md#crldetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCrlsResponseTypeDef

```python
# ListCrlsResponseTypeDef definition

class ListCrlsResponseTypeDef(TypedDict):
    crls: List[CrlDetailTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CrlDetailTypeDef](./type_defs.md#crldetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubjectDetailTypeDef

```python
# SubjectDetailTypeDef definition

class SubjectDetailTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    credentials: NotRequired[List[CredentialSummaryTypeDef]],  # (1)
    enabled: NotRequired[bool],
    instanceProperties: NotRequired[List[InstancePropertyTypeDef]],  # (2)
    lastSeenAt: NotRequired[datetime],
    subjectArn: NotRequired[str],
    subjectId: NotRequired[str],
    updatedAt: NotRequired[datetime],
    x509Subject: NotRequired[str],
```

1. See [:material-code-braces: CredentialSummaryTypeDef](./type_defs.md#credentialsummarytypedef) 
2. See [:material-code-braces: InstancePropertyTypeDef](./type_defs.md#instancepropertytypedef) 
## ListProfilesResponseTypeDef

```python
# ListProfilesResponseTypeDef definition

class ListProfilesResponseTypeDef(TypedDict):
    nextToken: str,
    profiles: List[ProfileDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileDetailTypeDef](./type_defs.md#profiledetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProfileDetailResponseTypeDef

```python
# ProfileDetailResponseTypeDef definition

class ProfileDetailResponseTypeDef(TypedDict):
    profile: ProfileDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileDetailTypeDef](./type_defs.md#profiledetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRequestListCrlsPaginateTypeDef

```python
# ListRequestListCrlsPaginateTypeDef definition

class ListRequestListCrlsPaginateTypeDef(TypedDict):
    pageSize: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRequestListProfilesPaginateTypeDef

```python
# ListRequestListProfilesPaginateTypeDef definition

class ListRequestListProfilesPaginateTypeDef(TypedDict):
    pageSize: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRequestListSubjectsPaginateTypeDef

```python
# ListRequestListSubjectsPaginateTypeDef definition

class ListRequestListSubjectsPaginateTypeDef(TypedDict):
    pageSize: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRequestListTrustAnchorsPaginateTypeDef

```python
# ListRequestListTrustAnchorsPaginateTypeDef definition

class ListRequestListTrustAnchorsPaginateTypeDef(TypedDict):
    pageSize: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubjectsResponseTypeDef

```python
# ListSubjectsResponseTypeDef definition

class ListSubjectsResponseTypeDef(TypedDict):
    nextToken: str,
    subjects: List[SubjectSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubjectSummaryTypeDef](./type_defs.md#subjectsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetNotificationSettingsRequestRequestTypeDef

```python
# ResetNotificationSettingsRequestRequestTypeDef definition

class ResetNotificationSettingsRequestRequestTypeDef(TypedDict):
    notificationSettingKeys: Sequence[NotificationSettingKeyTypeDef],  # (1)
    trustAnchorId: str,
```

1. See [:material-code-braces: NotificationSettingKeyTypeDef](./type_defs.md#notificationsettingkeytypedef) 
## SourceTypeDef

```python
# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    sourceData: NotRequired[SourceDataTypeDef],  # (1)
    sourceType: NotRequired[TrustAnchorTypeType],  # (2)
```

1. See [:material-code-braces: SourceDataTypeDef](./type_defs.md#sourcedatatypedef) 
2. See [:material-code-brackets: TrustAnchorTypeType](./literals.md#trustanchortypetype) 
## SubjectDetailResponseTypeDef

```python
# SubjectDetailResponseTypeDef definition

class SubjectDetailResponseTypeDef(TypedDict):
    subject: SubjectDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubjectDetailTypeDef](./type_defs.md#subjectdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrustAnchorRequestRequestTypeDef

```python
# CreateTrustAnchorRequestRequestTypeDef definition

class CreateTrustAnchorRequestRequestTypeDef(TypedDict):
    name: str,
    source: SourceTypeDef,  # (1)
    enabled: NotRequired[bool],
    notificationSettings: NotRequired[Sequence[NotificationSettingTypeDef]],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: NotificationSettingTypeDef](./type_defs.md#notificationsettingtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TrustAnchorDetailTypeDef

```python
# TrustAnchorDetailTypeDef definition

class TrustAnchorDetailTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    enabled: NotRequired[bool],
    name: NotRequired[str],
    notificationSettings: NotRequired[List[NotificationSettingDetailTypeDef]],  # (1)
    source: NotRequired[SourceTypeDef],  # (2)
    trustAnchorArn: NotRequired[str],
    trustAnchorId: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: NotificationSettingDetailTypeDef](./type_defs.md#notificationsettingdetailtypedef) 
2. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
## UpdateTrustAnchorRequestRequestTypeDef

```python
# UpdateTrustAnchorRequestRequestTypeDef definition

class UpdateTrustAnchorRequestRequestTypeDef(TypedDict):
    trustAnchorId: str,
    name: NotRequired[str],
    source: NotRequired[SourceTypeDef],  # (1)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
## ListTrustAnchorsResponseTypeDef

```python
# ListTrustAnchorsResponseTypeDef definition

class ListTrustAnchorsResponseTypeDef(TypedDict):
    nextToken: str,
    trustAnchors: List[TrustAnchorDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustAnchorDetailTypeDef](./type_defs.md#trustanchordetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutNotificationSettingsResponseTypeDef

```python
# PutNotificationSettingsResponseTypeDef definition

class PutNotificationSettingsResponseTypeDef(TypedDict):
    trustAnchor: TrustAnchorDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustAnchorDetailTypeDef](./type_defs.md#trustanchordetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetNotificationSettingsResponseTypeDef

```python
# ResetNotificationSettingsResponseTypeDef definition

class ResetNotificationSettingsResponseTypeDef(TypedDict):
    trustAnchor: TrustAnchorDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustAnchorDetailTypeDef](./type_defs.md#trustanchordetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TrustAnchorDetailResponseTypeDef

```python
# TrustAnchorDetailResponseTypeDef definition

class TrustAnchorDetailResponseTypeDef(TypedDict):
    trustAnchor: TrustAnchorDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustAnchorDetailTypeDef](./type_defs.md#trustanchordetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
