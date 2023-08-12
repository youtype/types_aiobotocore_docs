# Type definitions

> [Index](../README.md) > [CloudHSM](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudHSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
    type annotations stubs module [types-aiobotocore-cloudhsm](https://pypi.org/project/types-aiobotocore-cloudhsm/).



## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
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

## CreateHapgRequestRequestTypeDef

```python
# CreateHapgRequestRequestTypeDef definition

class CreateHapgRequestRequestTypeDef(TypedDict):
    Label: str,
```

## CreateHsmRequestRequestTypeDef

```python
# CreateHsmRequestRequestTypeDef definition

class CreateHsmRequestRequestTypeDef(TypedDict):
    SubnetId: str,
    SshKey: str,
    IamRoleArn: str,
    SubscriptionType: SubscriptionTypeType,  # (1)
    EniIp: NotRequired[str],
    ExternalId: NotRequired[str],
    ClientToken: NotRequired[str],
    SyslogIp: NotRequired[str],
```

1. See [:material-code-brackets: SubscriptionTypeType](./literals.md#subscriptiontypetype) 
## CreateLunaClientRequestRequestTypeDef

```python
# CreateLunaClientRequestRequestTypeDef definition

class CreateLunaClientRequestRequestTypeDef(TypedDict):
    Certificate: str,
    Label: NotRequired[str],
```

## DeleteHapgRequestRequestTypeDef

```python
# DeleteHapgRequestRequestTypeDef definition

class DeleteHapgRequestRequestTypeDef(TypedDict):
    HapgArn: str,
```

## DeleteHsmRequestRequestTypeDef

```python
# DeleteHsmRequestRequestTypeDef definition

class DeleteHsmRequestRequestTypeDef(TypedDict):
    HsmArn: str,
```

## DeleteLunaClientRequestRequestTypeDef

```python
# DeleteLunaClientRequestRequestTypeDef definition

class DeleteLunaClientRequestRequestTypeDef(TypedDict):
    ClientArn: str,
```

## DescribeHapgRequestRequestTypeDef

```python
# DescribeHapgRequestRequestTypeDef definition

class DescribeHapgRequestRequestTypeDef(TypedDict):
    HapgArn: str,
```

## DescribeHsmRequestRequestTypeDef

```python
# DescribeHsmRequestRequestTypeDef definition

class DescribeHsmRequestRequestTypeDef(TypedDict):
    HsmArn: NotRequired[str],
    HsmSerialNumber: NotRequired[str],
```

## DescribeLunaClientRequestRequestTypeDef

```python
# DescribeLunaClientRequestRequestTypeDef definition

class DescribeLunaClientRequestRequestTypeDef(TypedDict):
    ClientArn: NotRequired[str],
    CertificateFingerprint: NotRequired[str],
```

## GetConfigRequestRequestTypeDef

```python
# GetConfigRequestRequestTypeDef definition

class GetConfigRequestRequestTypeDef(TypedDict):
    ClientArn: str,
    ClientVersion: ClientVersionType,  # (1)
    HapgList: Sequence[str],
```

1. See [:material-code-brackets: ClientVersionType](./literals.md#clientversiontype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListHapgsRequestRequestTypeDef

```python
# ListHapgsRequestRequestTypeDef definition

class ListHapgsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## ListHsmsRequestRequestTypeDef

```python
# ListHsmsRequestRequestTypeDef definition

class ListHsmsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## ListLunaClientsRequestRequestTypeDef

```python
# ListLunaClientsRequestRequestTypeDef definition

class ListLunaClientsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ModifyHapgRequestRequestTypeDef

```python
# ModifyHapgRequestRequestTypeDef definition

class ModifyHapgRequestRequestTypeDef(TypedDict):
    HapgArn: str,
    Label: NotRequired[str],
    PartitionSerialList: NotRequired[Sequence[str]],
```

## ModifyHsmRequestRequestTypeDef

```python
# ModifyHsmRequestRequestTypeDef definition

class ModifyHsmRequestRequestTypeDef(TypedDict):
    HsmArn: str,
    SubnetId: NotRequired[str],
    EniIp: NotRequired[str],
    IamRoleArn: NotRequired[str],
    ExternalId: NotRequired[str],
    SyslogIp: NotRequired[str],
```

## ModifyLunaClientRequestRequestTypeDef

```python
# ModifyLunaClientRequestRequestTypeDef definition

class ModifyLunaClientRequestRequestTypeDef(TypedDict):
    ClientArn: str,
    Certificate: str,
```

## RemoveTagsFromResourceRequestRequestTypeDef

```python
# RemoveTagsFromResourceRequestRequestTypeDef definition

class RemoveTagsFromResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeyList: Sequence[str],
```

## AddTagsToResourceRequestRequestTypeDef

```python
# AddTagsToResourceRequestRequestTypeDef definition

class AddTagsToResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagList: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AddTagsToResourceResponseTypeDef

```python
# AddTagsToResourceResponseTypeDef definition

class AddTagsToResourceResponseTypeDef(TypedDict):
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHapgResponseTypeDef

```python
# CreateHapgResponseTypeDef definition

class CreateHapgResponseTypeDef(TypedDict):
    HapgArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHsmResponseTypeDef

```python
# CreateHsmResponseTypeDef definition

class CreateHsmResponseTypeDef(TypedDict):
    HsmArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLunaClientResponseTypeDef

```python
# CreateLunaClientResponseTypeDef definition

class CreateLunaClientResponseTypeDef(TypedDict):
    ClientArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteHapgResponseTypeDef

```python
# DeleteHapgResponseTypeDef definition

class DeleteHapgResponseTypeDef(TypedDict):
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteHsmResponseTypeDef

```python
# DeleteHsmResponseTypeDef definition

class DeleteHsmResponseTypeDef(TypedDict):
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteLunaClientResponseTypeDef

```python
# DeleteLunaClientResponseTypeDef definition

class DeleteLunaClientResponseTypeDef(TypedDict):
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeHapgResponseTypeDef

```python
# DescribeHapgResponseTypeDef definition

class DescribeHapgResponseTypeDef(TypedDict):
    HapgArn: str,
    HapgSerial: str,
    HsmsLastActionFailed: List[str],
    HsmsPendingDeletion: List[str],
    HsmsPendingRegistration: List[str],
    Label: str,
    LastModifiedTimestamp: str,
    PartitionSerialList: List[str],
    State: CloudHsmObjectStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CloudHsmObjectStateType](./literals.md#cloudhsmobjectstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeHsmResponseTypeDef

```python
# DescribeHsmResponseTypeDef definition

class DescribeHsmResponseTypeDef(TypedDict):
    HsmArn: str,
    Status: HsmStatusType,  # (1)
    StatusDetails: str,
    AvailabilityZone: str,
    EniId: str,
    EniIp: str,
    SubscriptionType: SubscriptionTypeType,  # (2)
    SubscriptionStartDate: str,
    SubscriptionEndDate: str,
    VpcId: str,
    SubnetId: str,
    IamRoleArn: str,
    SerialNumber: str,
    VendorName: str,
    HsmType: str,
    SoftwareVersion: str,
    SshPublicKey: str,
    SshKeyLastUpdated: str,
    ServerCertUri: str,
    ServerCertLastUpdated: str,
    Partitions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: HsmStatusType](./literals.md#hsmstatustype) 
2. See [:material-code-brackets: SubscriptionTypeType](./literals.md#subscriptiontypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLunaClientResponseTypeDef

```python
# DescribeLunaClientResponseTypeDef definition

class DescribeLunaClientResponseTypeDef(TypedDict):
    ClientArn: str,
    Certificate: str,
    CertificateFingerprint: str,
    LastModifiedTimestamp: str,
    Label: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfigResponseTypeDef

```python
# GetConfigResponseTypeDef definition

class GetConfigResponseTypeDef(TypedDict):
    ConfigType: str,
    ConfigFile: str,
    ConfigCred: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAvailableZonesResponseTypeDef

```python
# ListAvailableZonesResponseTypeDef definition

class ListAvailableZonesResponseTypeDef(TypedDict):
    AZList: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHapgsResponseTypeDef

```python
# ListHapgsResponseTypeDef definition

class ListHapgsResponseTypeDef(TypedDict):
    HapgList: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHsmsResponseTypeDef

```python
# ListHsmsResponseTypeDef definition

class ListHsmsResponseTypeDef(TypedDict):
    HsmList: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLunaClientsResponseTypeDef

```python
# ListLunaClientsResponseTypeDef definition

class ListLunaClientsResponseTypeDef(TypedDict):
    ClientList: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyHapgResponseTypeDef

```python
# ModifyHapgResponseTypeDef definition

class ModifyHapgResponseTypeDef(TypedDict):
    HapgArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyHsmResponseTypeDef

```python
# ModifyHsmResponseTypeDef definition

class ModifyHsmResponseTypeDef(TypedDict):
    HsmArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyLunaClientResponseTypeDef

```python
# ModifyLunaClientResponseTypeDef definition

class ModifyLunaClientResponseTypeDef(TypedDict):
    ClientArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveTagsFromResourceResponseTypeDef

```python
# RemoveTagsFromResourceResponseTypeDef definition

class RemoveTagsFromResourceResponseTypeDef(TypedDict):
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHapgsRequestListHapgsPaginateTypeDef

```python
# ListHapgsRequestListHapgsPaginateTypeDef definition

class ListHapgsRequestListHapgsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHsmsRequestListHsmsPaginateTypeDef

```python
# ListHsmsRequestListHsmsPaginateTypeDef definition

class ListHsmsRequestListHsmsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLunaClientsRequestListLunaClientsPaginateTypeDef

```python
# ListLunaClientsRequestListLunaClientsPaginateTypeDef definition

class ListLunaClientsRequestListLunaClientsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
