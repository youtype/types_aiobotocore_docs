<a id="typed-dictionaries-for-aiobotocore-cloudhsm-module"></a>

# Typed dictionaries for aiobotocore CloudHSM module

> [Index](../README.md) > [CloudHSM](./README.md) > Typed dictionaries

Auto-generated documentation for
[CloudHSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
type annotations stubs module
[types-aiobotocore-cloudhsm](https://pypi.org/project/types-aiobotocore-cloudhsm/).

- [Typed dictionaries for aiobotocore CloudHSM module](#typed-dictionaries-for-aiobotocore-cloudhsm-module)
  - [AddTagsToResourceRequestRequestTypeDef](#addtagstoresourcerequestrequesttypedef)
  - [AddTagsToResourceResponseTypeDef](#addtagstoresourceresponsetypedef)
  - [CreateHapgRequestRequestTypeDef](#createhapgrequestrequesttypedef)
  - [CreateHapgResponseTypeDef](#createhapgresponsetypedef)
  - [CreateHsmRequestRequestTypeDef](#createhsmrequestrequesttypedef)
  - [CreateHsmResponseTypeDef](#createhsmresponsetypedef)
  - [CreateLunaClientRequestRequestTypeDef](#createlunaclientrequestrequesttypedef)
  - [CreateLunaClientResponseTypeDef](#createlunaclientresponsetypedef)
  - [DeleteHapgRequestRequestTypeDef](#deletehapgrequestrequesttypedef)
  - [DeleteHapgResponseTypeDef](#deletehapgresponsetypedef)
  - [DeleteHsmRequestRequestTypeDef](#deletehsmrequestrequesttypedef)
  - [DeleteHsmResponseTypeDef](#deletehsmresponsetypedef)
  - [DeleteLunaClientRequestRequestTypeDef](#deletelunaclientrequestrequesttypedef)
  - [DeleteLunaClientResponseTypeDef](#deletelunaclientresponsetypedef)
  - [DescribeHapgRequestRequestTypeDef](#describehapgrequestrequesttypedef)
  - [DescribeHapgResponseTypeDef](#describehapgresponsetypedef)
  - [DescribeHsmRequestRequestTypeDef](#describehsmrequestrequesttypedef)
  - [DescribeHsmResponseTypeDef](#describehsmresponsetypedef)
  - [DescribeLunaClientRequestRequestTypeDef](#describelunaclientrequestrequesttypedef)
  - [DescribeLunaClientResponseTypeDef](#describelunaclientresponsetypedef)
  - [GetConfigRequestRequestTypeDef](#getconfigrequestrequesttypedef)
  - [GetConfigResponseTypeDef](#getconfigresponsetypedef)
  - [ListAvailableZonesResponseTypeDef](#listavailablezonesresponsetypedef)
  - [ListHapgsRequestRequestTypeDef](#listhapgsrequestrequesttypedef)
  - [ListHapgsResponseTypeDef](#listhapgsresponsetypedef)
  - [ListHsmsRequestRequestTypeDef](#listhsmsrequestrequesttypedef)
  - [ListHsmsResponseTypeDef](#listhsmsresponsetypedef)
  - [ListLunaClientsRequestRequestTypeDef](#listlunaclientsrequestrequesttypedef)
  - [ListLunaClientsResponseTypeDef](#listlunaclientsresponsetypedef)
  - [ListTagsForResourceRequestRequestTypeDef](#listtagsforresourcerequestrequesttypedef)
  - [ListTagsForResourceResponseTypeDef](#listtagsforresourceresponsetypedef)
  - [ModifyHapgRequestRequestTypeDef](#modifyhapgrequestrequesttypedef)
  - [ModifyHapgResponseTypeDef](#modifyhapgresponsetypedef)
  - [ModifyHsmRequestRequestTypeDef](#modifyhsmrequestrequesttypedef)
  - [ModifyHsmResponseTypeDef](#modifyhsmresponsetypedef)
  - [ModifyLunaClientRequestRequestTypeDef](#modifylunaclientrequestrequesttypedef)
  - [ModifyLunaClientResponseTypeDef](#modifylunaclientresponsetypedef)
  - [PaginatorConfigTypeDef](#paginatorconfigtypedef)
  - [RemoveTagsFromResourceRequestRequestTypeDef](#removetagsfromresourcerequestrequesttypedef)
  - [RemoveTagsFromResourceResponseTypeDef](#removetagsfromresourceresponsetypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [TagTypeDef](#tagtypedef)

<a id="addtagstoresourcerequestrequesttypedef"></a>

## AddTagsToResourceRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import AddTagsToResourceRequestRequestTypeDef
```

Required fields:

- `ResourceArn`: `str`
- `TagList`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="addtagstoresourceresponsetypedef"></a>

## AddTagsToResourceResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import AddTagsToResourceResponseTypeDef
```

Required fields:

- `Status`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createhapgrequestrequesttypedef"></a>

## CreateHapgRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import CreateHapgRequestRequestTypeDef
```

Required fields:

- `Label`: `str`

<a id="createhapgresponsetypedef"></a>

## CreateHapgResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import CreateHapgResponseTypeDef
```

Required fields:

- `HapgArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createhsmrequestrequesttypedef"></a>

## CreateHsmRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import CreateHsmRequestRequestTypeDef
```

Required fields:

- `SubnetId`: `str`
- `SshKey`: `str`
- `IamRoleArn`: `str`
- `SubscriptionType`: `Literal['PRODUCTION']` (see
  [SubscriptionTypeType](./literals.md#subscriptiontypetype))

Optional fields:

- `EniIp`: `str`
- `ExternalId`: `str`
- `ClientToken`: `str`
- `SyslogIp`: `str`

<a id="createhsmresponsetypedef"></a>

## CreateHsmResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import CreateHsmResponseTypeDef
```

Required fields:

- `HsmArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createlunaclientrequestrequesttypedef"></a>

## CreateLunaClientRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import CreateLunaClientRequestRequestTypeDef
```

Required fields:

- `Certificate`: `str`

Optional fields:

- `Label`: `str`

<a id="createlunaclientresponsetypedef"></a>

## CreateLunaClientResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import CreateLunaClientResponseTypeDef
```

Required fields:

- `ClientArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deletehapgrequestrequesttypedef"></a>

## DeleteHapgRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import DeleteHapgRequestRequestTypeDef
```

Required fields:

- `HapgArn`: `str`

<a id="deletehapgresponsetypedef"></a>

## DeleteHapgResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import DeleteHapgResponseTypeDef
```

Required fields:

- `Status`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deletehsmrequestrequesttypedef"></a>

## DeleteHsmRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import DeleteHsmRequestRequestTypeDef
```

Required fields:

- `HsmArn`: `str`

<a id="deletehsmresponsetypedef"></a>

## DeleteHsmResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import DeleteHsmResponseTypeDef
```

Required fields:

- `Status`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deletelunaclientrequestrequesttypedef"></a>

## DeleteLunaClientRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import DeleteLunaClientRequestRequestTypeDef
```

Required fields:

- `ClientArn`: `str`

<a id="deletelunaclientresponsetypedef"></a>

## DeleteLunaClientResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import DeleteLunaClientResponseTypeDef
```

Required fields:

- `Status`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describehapgrequestrequesttypedef"></a>

## DescribeHapgRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import DescribeHapgRequestRequestTypeDef
```

Required fields:

- `HapgArn`: `str`

<a id="describehapgresponsetypedef"></a>

## DescribeHapgResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import DescribeHapgResponseTypeDef
```

Required fields:

- `HapgArn`: `str`
- `HapgSerial`: `str`
- `HsmsLastActionFailed`: `List`\[`str`\]
- `HsmsPendingDeletion`: `List`\[`str`\]
- `HsmsPendingRegistration`: `List`\[`str`\]
- `Label`: `str`
- `LastModifiedTimestamp`: `str`
- `PartitionSerialList`: `List`\[`str`\]
- `State`: [CloudHsmObjectStateType](./literals.md#cloudhsmobjectstatetype)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describehsmrequestrequesttypedef"></a>

## DescribeHsmRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import DescribeHsmRequestRequestTypeDef
```

Optional fields:

- `HsmArn`: `str`
- `HsmSerialNumber`: `str`

<a id="describehsmresponsetypedef"></a>

## DescribeHsmResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import DescribeHsmResponseTypeDef
```

Required fields:

- `HsmArn`: `str`
- `Status`: [HsmStatusType](./literals.md#hsmstatustype)
- `StatusDetails`: `str`
- `AvailabilityZone`: `str`
- `EniId`: `str`
- `EniIp`: `str`
- `SubscriptionType`: `Literal['PRODUCTION']` (see
  [SubscriptionTypeType](./literals.md#subscriptiontypetype))
- `SubscriptionStartDate`: `str`
- `SubscriptionEndDate`: `str`
- `VpcId`: `str`
- `SubnetId`: `str`
- `IamRoleArn`: `str`
- `SerialNumber`: `str`
- `VendorName`: `str`
- `HsmType`: `str`
- `SoftwareVersion`: `str`
- `SshPublicKey`: `str`
- `SshKeyLastUpdated`: `str`
- `ServerCertUri`: `str`
- `ServerCertLastUpdated`: `str`
- `Partitions`: `List`\[`str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describelunaclientrequestrequesttypedef"></a>

## DescribeLunaClientRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import DescribeLunaClientRequestRequestTypeDef
```

Optional fields:

- `ClientArn`: `str`
- `CertificateFingerprint`: `str`

<a id="describelunaclientresponsetypedef"></a>

## DescribeLunaClientResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import DescribeLunaClientResponseTypeDef
```

Required fields:

- `ClientArn`: `str`
- `Certificate`: `str`
- `CertificateFingerprint`: `str`
- `LastModifiedTimestamp`: `str`
- `Label`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getconfigrequestrequesttypedef"></a>

## GetConfigRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import GetConfigRequestRequestTypeDef
```

Required fields:

- `ClientArn`: `str`
- `ClientVersion`: [ClientVersionType](./literals.md#clientversiontype)
- `HapgList`: `Sequence`\[`str`\]

<a id="getconfigresponsetypedef"></a>

## GetConfigResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import GetConfigResponseTypeDef
```

Required fields:

- `ConfigType`: `str`
- `ConfigFile`: `str`
- `ConfigCred`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listavailablezonesresponsetypedef"></a>

## ListAvailableZonesResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ListAvailableZonesResponseTypeDef
```

Required fields:

- `AZList`: `List`\[`str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listhapgsrequestrequesttypedef"></a>

## ListHapgsRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ListHapgsRequestRequestTypeDef
```

Optional fields:

- `NextToken`: `str`

<a id="listhapgsresponsetypedef"></a>

## ListHapgsResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ListHapgsResponseTypeDef
```

Required fields:

- `HapgList`: `List`\[`str`\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listhsmsrequestrequesttypedef"></a>

## ListHsmsRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ListHsmsRequestRequestTypeDef
```

Optional fields:

- `NextToken`: `str`

<a id="listhsmsresponsetypedef"></a>

## ListHsmsResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ListHsmsResponseTypeDef
```

Required fields:

- `HsmList`: `List`\[`str`\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listlunaclientsrequestrequesttypedef"></a>

## ListLunaClientsRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ListLunaClientsRequestRequestTypeDef
```

Optional fields:

- `NextToken`: `str`

<a id="listlunaclientsresponsetypedef"></a>

## ListLunaClientsResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ListLunaClientsResponseTypeDef
```

Required fields:

- `ClientList`: `List`\[`str`\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtagsforresourcerequestrequesttypedef"></a>

## ListTagsForResourceRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ListTagsForResourceRequestRequestTypeDef
```

Required fields:

- `ResourceArn`: `str`

<a id="listtagsforresourceresponsetypedef"></a>

## ListTagsForResourceResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ListTagsForResourceResponseTypeDef
```

Required fields:

- `TagList`: `List`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="modifyhapgrequestrequesttypedef"></a>

## ModifyHapgRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ModifyHapgRequestRequestTypeDef
```

Required fields:

- `HapgArn`: `str`

Optional fields:

- `Label`: `str`
- `PartitionSerialList`: `Sequence`\[`str`\]

<a id="modifyhapgresponsetypedef"></a>

## ModifyHapgResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ModifyHapgResponseTypeDef
```

Required fields:

- `HapgArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="modifyhsmrequestrequesttypedef"></a>

## ModifyHsmRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ModifyHsmRequestRequestTypeDef
```

Required fields:

- `HsmArn`: `str`

Optional fields:

- `SubnetId`: `str`
- `EniIp`: `str`
- `IamRoleArn`: `str`
- `ExternalId`: `str`
- `SyslogIp`: `str`

<a id="modifyhsmresponsetypedef"></a>

## ModifyHsmResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ModifyHsmResponseTypeDef
```

Required fields:

- `HsmArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="modifylunaclientrequestrequesttypedef"></a>

## ModifyLunaClientRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ModifyLunaClientRequestRequestTypeDef
```

Required fields:

- `ClientArn`: `str`
- `Certificate`: `str`

<a id="modifylunaclientresponsetypedef"></a>

## ModifyLunaClientResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ModifyLunaClientResponseTypeDef
```

Required fields:

- `ClientArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="paginatorconfigtypedef"></a>

## PaginatorConfigTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import PaginatorConfigTypeDef
```

Optional fields:

- `MaxItems`: `int`
- `PageSize`: `int`
- `StartingToken`: `str`

<a id="removetagsfromresourcerequestrequesttypedef"></a>

## RemoveTagsFromResourceRequestRequestTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import RemoveTagsFromResourceRequestRequestTypeDef
```

Required fields:

- `ResourceArn`: `str`
- `TagKeyList`: `Sequence`\[`str`\]

<a id="removetagsfromresourceresponsetypedef"></a>

## RemoveTagsFromResourceResponseTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import RemoveTagsFromResourceResponseTypeDef
```

Required fields:

- `Status`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="tagtypedef"></a>

## TagTypeDef

```python
from types_aiobotocore_cloudhsm.type_defs import TagTypeDef
```

Required fields:

- `Key`: `str`
- `Value`: `str`
