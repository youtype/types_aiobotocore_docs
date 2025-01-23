# KMS module

> [Index](../README.md) > KMS


!!! note ""

    Auto-generated documentation for [KMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#kms)
    type annotations stubs module [types-aiobotocore-kms](https://pypi.org/project/types-aiobotocore-kms/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `KMS` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `KMS` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[kms]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[kms]'

# standalone installation
python -m pip install types-aiobotocore-kms
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-kms
```

## Usage

Code samples can be found in [Examples](./usage.md).

## KMSClient

Type annotations and code completion for  `#!python session.create_client("kms")` as [KMSClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)

```python
# KMSClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_kms.client import KMSClient


session = get_session()
async with session.create_client("kms") as client:
    client: KMSClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("kms").get_paginator("...")`.

```python
# DescribeCustomKeyStoresPaginator usage example

from types_aiobotocore_kms.paginator import DescribeCustomKeyStoresPaginator

def get_describe_custom_key_stores_paginator() -> DescribeCustomKeyStoresPaginator:
    return client.get_paginator("describe_custom_key_stores"))
```

- [DescribeCustomKeyStoresPaginator](./paginators.md#describecustomkeystorespaginator)
- [ListAliasesPaginator](./paginators.md#listaliasespaginator)
- [ListGrantsPaginator](./paginators.md#listgrantspaginator)
- [ListKeyPoliciesPaginator](./paginators.md#listkeypoliciespaginator)
- [ListKeyRotationsPaginator](./paginators.md#listkeyrotationspaginator)
- [ListKeysPaginator](./paginators.md#listkeyspaginator)
- [ListResourceTagsPaginator](./paginators.md#listresourcetagspaginator)
- [ListRetirableGrantsPaginator](./paginators.md#listretirablegrantspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AlgorithmSpecType usage example

from types_aiobotocore_kms.literals import AlgorithmSpecType

def get_value() -> AlgorithmSpecType:
    return "RSAES_OAEP_SHA_1"
```

- [AlgorithmSpecType](./literals.md#algorithmspectype)
- [ConnectionErrorCodeTypeType](./literals.md#connectionerrorcodetypetype)
- [ConnectionStateTypeType](./literals.md#connectionstatetypetype)
- [CustomKeyStoreTypeType](./literals.md#customkeystoretypetype)
- [CustomerMasterKeySpecType](./literals.md#customermasterkeyspectype)
- [DataKeyPairSpecType](./literals.md#datakeypairspectype)
- [DataKeySpecType](./literals.md#datakeyspectype)
- [DescribeCustomKeyStoresPaginatorName](./literals.md#describecustomkeystorespaginatorname)
- [EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype)
- [ExpirationModelTypeType](./literals.md#expirationmodeltypetype)
- [GrantOperationType](./literals.md#grantoperationtype)
- [KeyAgreementAlgorithmSpecType](./literals.md#keyagreementalgorithmspectype)
- [KeyEncryptionMechanismType](./literals.md#keyencryptionmechanismtype)
- [KeyManagerTypeType](./literals.md#keymanagertypetype)
- [KeySpecType](./literals.md#keyspectype)
- [KeyStateType](./literals.md#keystatetype)
- [KeyUsageTypeType](./literals.md#keyusagetypetype)
- [ListAliasesPaginatorName](./literals.md#listaliasespaginatorname)
- [ListGrantsPaginatorName](./literals.md#listgrantspaginatorname)
- [ListKeyPoliciesPaginatorName](./literals.md#listkeypoliciespaginatorname)
- [ListKeyRotationsPaginatorName](./literals.md#listkeyrotationspaginatorname)
- [ListKeysPaginatorName](./literals.md#listkeyspaginatorname)
- [ListResourceTagsPaginatorName](./literals.md#listresourcetagspaginatorname)
- [ListRetirableGrantsPaginatorName](./literals.md#listretirablegrantspaginatorname)
- [MacAlgorithmSpecType](./literals.md#macalgorithmspectype)
- [MessageTypeType](./literals.md#messagetypetype)
- [MultiRegionKeyTypeType](./literals.md#multiregionkeytypetype)
- [OriginTypeType](./literals.md#origintypetype)
- [RotationTypeType](./literals.md#rotationtypetype)
- [SigningAlgorithmSpecType](./literals.md#signingalgorithmspectype)
- [WrappingKeySpecType](./literals.md#wrappingkeyspectype)
- [XksProxyConnectivityTypeType](./literals.md#xksproxyconnectivitytypetype)
- [KMSServiceName](./literals.md#kmsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AliasListEntryTypeDef](./type_defs.md#aliaslistentrytypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CancelKeyDeletionRequestRequestTypeDef](./type_defs.md#cancelkeydeletionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ConnectCustomKeyStoreRequestRequestTypeDef](./type_defs.md#connectcustomkeystorerequestrequesttypedef)
- [CreateAliasRequestRequestTypeDef](./type_defs.md#createaliasrequestrequesttypedef)
- [XksProxyAuthenticationCredentialTypeTypeDef](./type_defs.md#xksproxyauthenticationcredentialtypetypedef)
- [GrantConstraintsTypeDef](./type_defs.md#grantconstraintstypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [XksProxyConfigurationTypeTypeDef](./type_defs.md#xksproxyconfigurationtypetypedef)
- [DeleteAliasRequestRequestTypeDef](./type_defs.md#deletealiasrequestrequesttypedef)
- [DeleteCustomKeyStoreRequestRequestTypeDef](./type_defs.md#deletecustomkeystorerequestrequesttypedef)
- [DeleteImportedKeyMaterialRequestRequestTypeDef](./type_defs.md#deleteimportedkeymaterialrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeCustomKeyStoresRequestRequestTypeDef](./type_defs.md#describecustomkeystoresrequestrequesttypedef)
- [DescribeKeyRequestRequestTypeDef](./type_defs.md#describekeyrequestrequesttypedef)
- [DisableKeyRequestRequestTypeDef](./type_defs.md#disablekeyrequestrequesttypedef)
- [DisableKeyRotationRequestRequestTypeDef](./type_defs.md#disablekeyrotationrequestrequesttypedef)
- [DisconnectCustomKeyStoreRequestRequestTypeDef](./type_defs.md#disconnectcustomkeystorerequestrequesttypedef)
- [EnableKeyRequestRequestTypeDef](./type_defs.md#enablekeyrequestrequesttypedef)
- [EnableKeyRotationRequestRequestTypeDef](./type_defs.md#enablekeyrotationrequestrequesttypedef)
- [GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef](./type_defs.md#generatedatakeypairwithoutplaintextrequestrequesttypedef)
- [GenerateDataKeyWithoutPlaintextRequestRequestTypeDef](./type_defs.md#generatedatakeywithoutplaintextrequestrequesttypedef)
- [GetKeyPolicyRequestRequestTypeDef](./type_defs.md#getkeypolicyrequestrequesttypedef)
- [GetKeyRotationStatusRequestRequestTypeDef](./type_defs.md#getkeyrotationstatusrequestrequesttypedef)
- [GetParametersForImportRequestRequestTypeDef](./type_defs.md#getparametersforimportrequestrequesttypedef)
- [GetPublicKeyRequestRequestTypeDef](./type_defs.md#getpublickeyrequestrequesttypedef)
- [GrantConstraintsOutputTypeDef](./type_defs.md#grantconstraintsoutputtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [KeyListEntryTypeDef](./type_defs.md#keylistentrytypedef)
- [XksKeyConfigurationTypeTypeDef](./type_defs.md#xkskeyconfigurationtypetypedef)
- [ListAliasesRequestRequestTypeDef](./type_defs.md#listaliasesrequestrequesttypedef)
- [ListGrantsRequestRequestTypeDef](./type_defs.md#listgrantsrequestrequesttypedef)
- [ListKeyPoliciesRequestRequestTypeDef](./type_defs.md#listkeypoliciesrequestrequesttypedef)
- [ListKeyRotationsRequestRequestTypeDef](./type_defs.md#listkeyrotationsrequestrequesttypedef)
- [RotationsListEntryTypeDef](./type_defs.md#rotationslistentrytypedef)
- [ListKeysRequestRequestTypeDef](./type_defs.md#listkeysrequestrequesttypedef)
- [ListResourceTagsRequestRequestTypeDef](./type_defs.md#listresourcetagsrequestrequesttypedef)
- [ListRetirableGrantsRequestRequestTypeDef](./type_defs.md#listretirablegrantsrequestrequesttypedef)
- [MultiRegionKeyTypeDef](./type_defs.md#multiregionkeytypedef)
- [PutKeyPolicyRequestRequestTypeDef](./type_defs.md#putkeypolicyrequestrequesttypedef)
- [RetireGrantRequestRequestTypeDef](./type_defs.md#retiregrantrequestrequesttypedef)
- [RevokeGrantRequestRequestTypeDef](./type_defs.md#revokegrantrequestrequesttypedef)
- [RotateKeyOnDemandRequestRequestTypeDef](./type_defs.md#rotatekeyondemandrequestrequesttypedef)
- [ScheduleKeyDeletionRequestRequestTypeDef](./type_defs.md#schedulekeydeletionrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAliasRequestRequestTypeDef](./type_defs.md#updatealiasrequestrequesttypedef)
- [UpdateKeyDescriptionRequestRequestTypeDef](./type_defs.md#updatekeydescriptionrequestrequesttypedef)
- [UpdatePrimaryRegionRequestRequestTypeDef](./type_defs.md#updateprimaryregionrequestrequesttypedef)
- [EncryptRequestRequestTypeDef](./type_defs.md#encryptrequestrequesttypedef)
- [GenerateMacRequestRequestTypeDef](./type_defs.md#generatemacrequestrequesttypedef)
- [ReEncryptRequestRequestTypeDef](./type_defs.md#reencryptrequestrequesttypedef)
- [RecipientInfoTypeDef](./type_defs.md#recipientinfotypedef)
- [SignRequestRequestTypeDef](./type_defs.md#signrequestrequesttypedef)
- [VerifyMacRequestRequestTypeDef](./type_defs.md#verifymacrequestrequesttypedef)
- [VerifyRequestRequestTypeDef](./type_defs.md#verifyrequestrequesttypedef)
- [CancelKeyDeletionResponseTypeDef](./type_defs.md#cancelkeydeletionresponsetypedef)
- [CreateCustomKeyStoreResponseTypeDef](./type_defs.md#createcustomkeystoreresponsetypedef)
- [CreateGrantResponseTypeDef](./type_defs.md#creategrantresponsetypedef)
- [DecryptResponseTypeDef](./type_defs.md#decryptresponsetypedef)
- [DeriveSharedSecretResponseTypeDef](./type_defs.md#derivesharedsecretresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [EncryptResponseTypeDef](./type_defs.md#encryptresponsetypedef)
- [GenerateDataKeyPairResponseTypeDef](./type_defs.md#generatedatakeypairresponsetypedef)
- [GenerateDataKeyPairWithoutPlaintextResponseTypeDef](./type_defs.md#generatedatakeypairwithoutplaintextresponsetypedef)
- [GenerateDataKeyResponseTypeDef](./type_defs.md#generatedatakeyresponsetypedef)
- [GenerateDataKeyWithoutPlaintextResponseTypeDef](./type_defs.md#generatedatakeywithoutplaintextresponsetypedef)
- [GenerateMacResponseTypeDef](./type_defs.md#generatemacresponsetypedef)
- [GenerateRandomResponseTypeDef](./type_defs.md#generaterandomresponsetypedef)
- [GetKeyPolicyResponseTypeDef](./type_defs.md#getkeypolicyresponsetypedef)
- [GetKeyRotationStatusResponseTypeDef](./type_defs.md#getkeyrotationstatusresponsetypedef)
- [GetParametersForImportResponseTypeDef](./type_defs.md#getparametersforimportresponsetypedef)
- [GetPublicKeyResponseTypeDef](./type_defs.md#getpublickeyresponsetypedef)
- [ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef)
- [ListKeyPoliciesResponseTypeDef](./type_defs.md#listkeypoliciesresponsetypedef)
- [ReEncryptResponseTypeDef](./type_defs.md#reencryptresponsetypedef)
- [RotateKeyOnDemandResponseTypeDef](./type_defs.md#rotatekeyondemandresponsetypedef)
- [ScheduleKeyDeletionResponseTypeDef](./type_defs.md#schedulekeydeletionresponsetypedef)
- [SignResponseTypeDef](./type_defs.md#signresponsetypedef)
- [VerifyMacResponseTypeDef](./type_defs.md#verifymacresponsetypedef)
- [VerifyResponseTypeDef](./type_defs.md#verifyresponsetypedef)
- [CreateCustomKeyStoreRequestRequestTypeDef](./type_defs.md#createcustomkeystorerequestrequesttypedef)
- [UpdateCustomKeyStoreRequestRequestTypeDef](./type_defs.md#updatecustomkeystorerequestrequesttypedef)
- [CreateGrantRequestRequestTypeDef](./type_defs.md#creategrantrequestrequesttypedef)
- [CreateKeyRequestRequestTypeDef](./type_defs.md#createkeyrequestrequesttypedef)
- [ListResourceTagsResponseTypeDef](./type_defs.md#listresourcetagsresponsetypedef)
- [ReplicateKeyRequestRequestTypeDef](./type_defs.md#replicatekeyrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CustomKeyStoresListEntryTypeDef](./type_defs.md#customkeystoreslistentrytypedef)
- [DescribeCustomKeyStoresRequestPaginateTypeDef](./type_defs.md#describecustomkeystoresrequestpaginatetypedef)
- [ListAliasesRequestPaginateTypeDef](./type_defs.md#listaliasesrequestpaginatetypedef)
- [ListGrantsRequestPaginateTypeDef](./type_defs.md#listgrantsrequestpaginatetypedef)
- [ListKeyPoliciesRequestPaginateTypeDef](./type_defs.md#listkeypoliciesrequestpaginatetypedef)
- [ListKeyRotationsRequestPaginateTypeDef](./type_defs.md#listkeyrotationsrequestpaginatetypedef)
- [ListKeysRequestPaginateTypeDef](./type_defs.md#listkeysrequestpaginatetypedef)
- [ListResourceTagsRequestPaginateTypeDef](./type_defs.md#listresourcetagsrequestpaginatetypedef)
- [ListRetirableGrantsRequestPaginateTypeDef](./type_defs.md#listretirablegrantsrequestpaginatetypedef)
- [GrantListEntryTypeDef](./type_defs.md#grantlistentrytypedef)
- [ImportKeyMaterialRequestRequestTypeDef](./type_defs.md#importkeymaterialrequestrequesttypedef)
- [ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef)
- [ListKeyRotationsResponseTypeDef](./type_defs.md#listkeyrotationsresponsetypedef)
- [MultiRegionConfigurationTypeDef](./type_defs.md#multiregionconfigurationtypedef)
- [DecryptRequestRequestTypeDef](./type_defs.md#decryptrequestrequesttypedef)
- [DeriveSharedSecretRequestRequestTypeDef](./type_defs.md#derivesharedsecretrequestrequesttypedef)
- [GenerateDataKeyPairRequestRequestTypeDef](./type_defs.md#generatedatakeypairrequestrequesttypedef)
- [GenerateDataKeyRequestRequestTypeDef](./type_defs.md#generatedatakeyrequestrequesttypedef)
- [GenerateRandomRequestRequestTypeDef](./type_defs.md#generaterandomrequestrequesttypedef)
- [DescribeCustomKeyStoresResponseTypeDef](./type_defs.md#describecustomkeystoresresponsetypedef)
- [ListGrantsResponseTypeDef](./type_defs.md#listgrantsresponsetypedef)
- [KeyMetadataTypeDef](./type_defs.md#keymetadatatypedef)
- [CreateKeyResponseTypeDef](./type_defs.md#createkeyresponsetypedef)
- [DescribeKeyResponseTypeDef](./type_defs.md#describekeyresponsetypedef)
- [ReplicateKeyResponseTypeDef](./type_defs.md#replicatekeyresponsetypedef)

