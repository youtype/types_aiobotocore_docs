# PaymentCryptographyControlPlane module

> [Index](../README.md) > PaymentCryptographyControlPlane


!!! note ""

    Auto-generated documentation for [PaymentCryptographyControlPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#paymentcryptographycontrolplane)
    type annotations stubs module [types-aiobotocore-payment-cryptography](https://pypi.org/project/types-aiobotocore-payment-cryptography/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `PaymentCryptographyControlPlane` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `PaymentCryptographyControlPlane` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[payment-cryptography]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[payment-cryptography]'

# standalone installation
python -m pip install types-aiobotocore-payment-cryptography
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-payment-cryptography
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PaymentCryptographyControlPlaneClient

Type annotations and code completion for  `#!python session.create_client("payment-cryptography")` as [PaymentCryptographyControlPlaneClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Client)

```python
# PaymentCryptographyControlPlaneClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_payment_cryptography.client import PaymentCryptographyControlPlaneClient


session = get_session()
async with session.create_client("payment-cryptography") as client:
    client: PaymentCryptographyControlPlaneClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("payment-cryptography").get_paginator("...")`.

```python
# ListAliasesPaginator usage example

from types_aiobotocore_payment_cryptography.paginator import ListAliasesPaginator

def get_list_aliases_paginator() -> ListAliasesPaginator:
    return client.get_paginator("list_aliases"))
```

- [ListAliasesPaginator](./paginators.md#listaliasespaginator)
- [ListKeysPaginator](./paginators.md#listkeyspaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# KeyAlgorithmType usage example

from types_aiobotocore_payment_cryptography.literals import KeyAlgorithmType

def get_value() -> KeyAlgorithmType:
    return "AES_128"
```

- [KeyAlgorithmType](./literals.md#keyalgorithmtype)
- [KeyCheckValueAlgorithmType](./literals.md#keycheckvaluealgorithmtype)
- [KeyClassType](./literals.md#keyclasstype)
- [KeyExportabilityType](./literals.md#keyexportabilitytype)
- [KeyMaterialTypeType](./literals.md#keymaterialtypetype)
- [KeyOriginType](./literals.md#keyorigintype)
- [KeyStateType](./literals.md#keystatetype)
- [KeyUsageType](./literals.md#keyusagetype)
- [ListAliasesPaginatorName](./literals.md#listaliasespaginatorname)
- [ListKeysPaginatorName](./literals.md#listkeyspaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [Tr34KeyBlockFormatType](./literals.md#tr34keyblockformattype)
- [WrappedKeyMaterialFormatType](./literals.md#wrappedkeymaterialformattype)
- [WrappingKeySpecType](./literals.md#wrappingkeyspectype)
- [PaymentCryptographyControlPlaneServiceName](./literals.md#paymentcryptographycontrolplaneservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AliasTypeDef](./type_defs.md#aliastypedef)
- [CreateAliasInputRequestTypeDef](./type_defs.md#createaliasinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DeleteAliasInputRequestTypeDef](./type_defs.md#deletealiasinputrequesttypedef)
- [DeleteKeyInputRequestTypeDef](./type_defs.md#deletekeyinputrequesttypedef)
- [ExportDukptInitialKeyTypeDef](./type_defs.md#exportdukptinitialkeytypedef)
- [ExportKeyCryptogramTypeDef](./type_defs.md#exportkeycryptogramtypedef)
- [WrappedKeyTypeDef](./type_defs.md#wrappedkeytypedef)
- [GetAliasInputRequestTypeDef](./type_defs.md#getaliasinputrequesttypedef)
- [GetKeyInputRequestTypeDef](./type_defs.md#getkeyinputrequesttypedef)
- [GetParametersForExportInputRequestTypeDef](./type_defs.md#getparametersforexportinputrequesttypedef)
- [GetParametersForImportInputRequestTypeDef](./type_defs.md#getparametersforimportinputrequesttypedef)
- [GetPublicKeyCertificateInputRequestTypeDef](./type_defs.md#getpublickeycertificateinputrequesttypedef)
- [ImportTr31KeyBlockTypeDef](./type_defs.md#importtr31keyblocktypedef)
- [ImportTr34KeyBlockTypeDef](./type_defs.md#importtr34keyblocktypedef)
- [KeyModesOfUseTypeDef](./type_defs.md#keymodesofusetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAliasesInputRequestTypeDef](./type_defs.md#listaliasesinputrequesttypedef)
- [ListKeysInputRequestTypeDef](./type_defs.md#listkeysinputrequesttypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [RestoreKeyInputRequestTypeDef](./type_defs.md#restorekeyinputrequesttypedef)
- [StartKeyUsageInputRequestTypeDef](./type_defs.md#startkeyusageinputrequesttypedef)
- [StopKeyUsageInputRequestTypeDef](./type_defs.md#stopkeyusageinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateAliasInputRequestTypeDef](./type_defs.md#updatealiasinputrequesttypedef)
- [CreateAliasOutputTypeDef](./type_defs.md#createaliasoutputtypedef)
- [GetAliasOutputTypeDef](./type_defs.md#getaliasoutputtypedef)
- [GetParametersForExportOutputTypeDef](./type_defs.md#getparametersforexportoutputtypedef)
- [GetParametersForImportOutputTypeDef](./type_defs.md#getparametersforimportoutputtypedef)
- [GetPublicKeyCertificateOutputTypeDef](./type_defs.md#getpublickeycertificateoutputtypedef)
- [ListAliasesOutputTypeDef](./type_defs.md#listaliasesoutputtypedef)
- [UpdateAliasOutputTypeDef](./type_defs.md#updatealiasoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [ExportAttributesTypeDef](./type_defs.md#exportattributestypedef)
- [ExportKeyOutputTypeDef](./type_defs.md#exportkeyoutputtypedef)
- [KeyAttributesTypeDef](./type_defs.md#keyattributestypedef)
- [KeyBlockHeadersTypeDef](./type_defs.md#keyblockheaderstypedef)
- [ListAliasesInputPaginateTypeDef](./type_defs.md#listaliasesinputpaginatetypedef)
- [ListKeysInputPaginateTypeDef](./type_defs.md#listkeysinputpaginatetypedef)
- [ListTagsForResourceInputPaginateTypeDef](./type_defs.md#listtagsforresourceinputpaginatetypedef)
- [CreateKeyInputRequestTypeDef](./type_defs.md#createkeyinputrequesttypedef)
- [ImportKeyCryptogramTypeDef](./type_defs.md#importkeycryptogramtypedef)
- [KeySummaryTypeDef](./type_defs.md#keysummarytypedef)
- [KeyTypeDef](./type_defs.md#keytypedef)
- [RootCertificatePublicKeyTypeDef](./type_defs.md#rootcertificatepublickeytypedef)
- [TrustedCertificatePublicKeyTypeDef](./type_defs.md#trustedcertificatepublickeytypedef)
- [ExportTr31KeyBlockTypeDef](./type_defs.md#exporttr31keyblocktypedef)
- [ExportTr34KeyBlockTypeDef](./type_defs.md#exporttr34keyblocktypedef)
- [ListKeysOutputTypeDef](./type_defs.md#listkeysoutputtypedef)
- [CreateKeyOutputTypeDef](./type_defs.md#createkeyoutputtypedef)
- [DeleteKeyOutputTypeDef](./type_defs.md#deletekeyoutputtypedef)
- [GetKeyOutputTypeDef](./type_defs.md#getkeyoutputtypedef)
- [ImportKeyOutputTypeDef](./type_defs.md#importkeyoutputtypedef)
- [RestoreKeyOutputTypeDef](./type_defs.md#restorekeyoutputtypedef)
- [StartKeyUsageOutputTypeDef](./type_defs.md#startkeyusageoutputtypedef)
- [StopKeyUsageOutputTypeDef](./type_defs.md#stopkeyusageoutputtypedef)
- [ImportKeyMaterialTypeDef](./type_defs.md#importkeymaterialtypedef)
- [ExportKeyMaterialTypeDef](./type_defs.md#exportkeymaterialtypedef)
- [ImportKeyInputRequestTypeDef](./type_defs.md#importkeyinputrequesttypedef)
- [ExportKeyInputRequestTypeDef](./type_defs.md#exportkeyinputrequesttypedef)

