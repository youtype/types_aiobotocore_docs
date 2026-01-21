# PaymentCryptographyDataPlane module

> [Index](../README.md) > PaymentCryptographyDataPlane


!!! note ""

    Auto-generated documentation for [PaymentCryptographyDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#paymentcryptographydataplane)
    type annotations stubs module [types-aiobotocore-payment-cryptography-data](https://pypi.org/project/types-aiobotocore-payment-cryptography-data/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `PaymentCryptographyDataPlane` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `PaymentCryptographyDataPlane` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[payment-cryptography-data]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[payment-cryptography-data]'

# standalone installation
python -m pip install types-aiobotocore-payment-cryptography-data
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-payment-cryptography-data
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PaymentCryptographyDataPlaneClient

Type annotations and code completion for  `#!python session.create_client("payment-cryptography-data")` as [PaymentCryptographyDataPlaneClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client)

```python
# PaymentCryptographyDataPlaneClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_payment_cryptography_data.client import PaymentCryptographyDataPlaneClient


session = get_session()
async with session.create_client("payment-cryptography-data") as client:
    client: PaymentCryptographyDataPlaneClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DukptDerivationTypeType usage example

from types_aiobotocore_payment_cryptography_data.literals import DukptDerivationTypeType

def get_value() -> DukptDerivationTypeType:
    return "AES_128"
```

- [DukptDerivationTypeType](./literals.md#dukptderivationtypetype)
- [DukptEncryptionModeType](./literals.md#dukptencryptionmodetype)
- [DukptKeyVariantType](./literals.md#dukptkeyvarianttype)
- [EmvEncryptionModeType](./literals.md#emvencryptionmodetype)
- [EmvMajorKeyDerivationModeType](./literals.md#emvmajorkeyderivationmodetype)
- [EncryptionModeType](./literals.md#encryptionmodetype)
- [KeyCheckValueAlgorithmType](./literals.md#keycheckvaluealgorithmtype)
- [KeyDerivationFunctionType](./literals.md#keyderivationfunctiontype)
- [KeyDerivationHashAlgorithmType](./literals.md#keyderivationhashalgorithmtype)
- [MacAlgorithmType](./literals.md#macalgorithmtype)
- [MajorKeyDerivationModeType](./literals.md#majorkeyderivationmodetype)
- [PaddingTypeType](./literals.md#paddingtypetype)
- [PinBlockFormatForEmvPinChangeType](./literals.md#pinblockformatforemvpinchangetype)
- [PinBlockFormatForPinDataType](./literals.md#pinblockformatforpindatatype)
- [PinBlockLengthPositionType](./literals.md#pinblocklengthpositiontype)
- [PinBlockPaddingTypeType](./literals.md#pinblockpaddingtypetype)
- [RandomKeySendVariantMaskType](./literals.md#randomkeysendvariantmasktype)
- [SessionKeyDerivationModeType](./literals.md#sessionkeyderivationmodetype)
- [SymmetricKeyAlgorithmType](./literals.md#symmetrickeyalgorithmtype)
- [WrappedKeyMaterialFormatType](./literals.md#wrappedkeymaterialformattype)
- [PaymentCryptographyDataPlaneServiceName](./literals.md#paymentcryptographydataplaneservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CurrentPinAttributesTypeDef](./type_defs.md#currentpinattributestypedef)
- [AmexCardSecurityCodeVersion1TypeDef](./type_defs.md#amexcardsecuritycodeversion1typedef)
- [AmexCardSecurityCodeVersion2TypeDef](./type_defs.md#amexcardsecuritycodeversion2typedef)
- [KekValidationRequestTypeDef](./type_defs.md#kekvalidationrequesttypedef)
- [KekValidationResponseTypeDef](./type_defs.md#kekvalidationresponsetypedef)
- [As2805PekDerivationAttributesTypeDef](./type_defs.md#as2805pekderivationattributestypedef)
- [AsymmetricEncryptionAttributesTypeDef](./type_defs.md#asymmetricencryptionattributestypedef)
- [CardHolderVerificationValueTypeDef](./type_defs.md#cardholderverificationvaluetypedef)
- [CardVerificationValue1TypeDef](./type_defs.md#cardverificationvalue1typedef)
- [CardVerificationValue2TypeDef](./type_defs.md#cardverificationvalue2typedef)
- [DynamicCardVerificationCodeTypeDef](./type_defs.md#dynamiccardverificationcodetypedef)
- [DynamicCardVerificationValueTypeDef](./type_defs.md#dynamiccardverificationvaluetypedef)
- [DiscoverDynamicCardVerificationCodeTypeDef](./type_defs.md#discoverdynamiccardverificationcodetypedef)
- [CryptogramVerificationArpcMethod1TypeDef](./type_defs.md#cryptogramverificationarpcmethod1typedef)
- [CryptogramVerificationArpcMethod2TypeDef](./type_defs.md#cryptogramverificationarpcmethod2typedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [Emv2000AttributesTypeDef](./type_defs.md#emv2000attributestypedef)
- [EmvCommonAttributesTypeDef](./type_defs.md#emvcommonattributestypedef)
- [MasterCardAttributesTypeDef](./type_defs.md#mastercardattributestypedef)
- [DiffieHellmanDerivationDataTypeDef](./type_defs.md#diffiehellmanderivationdatatypedef)
- [DukptAttributesTypeDef](./type_defs.md#dukptattributestypedef)
- [DukptDerivationAttributesTypeDef](./type_defs.md#dukptderivationattributestypedef)
- [DukptEncryptionAttributesTypeDef](./type_defs.md#dukptencryptionattributestypedef)
- [EcdhDerivationAttributesTypeDef](./type_defs.md#ecdhderivationattributestypedef)
- [EmvEncryptionAttributesTypeDef](./type_defs.md#emvencryptionattributestypedef)
- [SymmetricEncryptionAttributesTypeDef](./type_defs.md#symmetricencryptionattributestypedef)
- [VisaAmexDerivationOutputsTypeDef](./type_defs.md#visaamexderivationoutputstypedef)
- [PinDataTypeDef](./type_defs.md#pindatatypedef)
- [Ibm3624NaturalPinTypeDef](./type_defs.md#ibm3624naturalpintypedef)
- [Ibm3624PinFromOffsetTypeDef](./type_defs.md#ibm3624pinfromoffsettypedef)
- [Ibm3624PinOffsetTypeDef](./type_defs.md#ibm3624pinoffsettypedef)
- [Ibm3624PinVerificationTypeDef](./type_defs.md#ibm3624pinverificationtypedef)
- [Ibm3624RandomPinTypeDef](./type_defs.md#ibm3624randompintypedef)
- [MacAlgorithmDukptTypeDef](./type_defs.md#macalgorithmdukpttypedef)
- [SessionKeyDerivationValueTypeDef](./type_defs.md#sessionkeyderivationvaluetypedef)
- [OutgoingTr31KeyBlockTypeDef](./type_defs.md#outgoingtr31keyblocktypedef)
- [VisaPinTypeDef](./type_defs.md#visapintypedef)
- [VisaPinVerificationValueTypeDef](./type_defs.md#visapinverificationvaluetypedef)
- [VisaPinVerificationTypeDef](./type_defs.md#visapinverificationtypedef)
- [SessionKeyAmexTypeDef](./type_defs.md#sessionkeyamextypedef)
- [SessionKeyEmv2000TypeDef](./type_defs.md#sessionkeyemv2000typedef)
- [SessionKeyEmvCommonTypeDef](./type_defs.md#sessionkeyemvcommontypedef)
- [SessionKeyMastercardTypeDef](./type_defs.md#sessionkeymastercardtypedef)
- [SessionKeyVisaTypeDef](./type_defs.md#sessionkeyvisatypedef)
- [WrappedWorkingKeyTypeDef](./type_defs.md#wrappedworkingkeytypedef)
- [TranslationPinDataAs2805Format0TypeDef](./type_defs.md#translationpindataas2805format0typedef)
- [TranslationPinDataIsoFormat034TypeDef](./type_defs.md#translationpindataisoformat034typedef)
- [AmexAttributesTypeDef](./type_defs.md#amexattributestypedef)
- [VisaAttributesTypeDef](./type_defs.md#visaattributestypedef)
- [As2805KekValidationTypeTypeDef](./type_defs.md#as2805kekvalidationtypetypedef)
- [CardGenerationAttributesTypeDef](./type_defs.md#cardgenerationattributestypedef)
- [CardVerificationAttributesTypeDef](./type_defs.md#cardverificationattributestypedef)
- [CryptogramAuthResponseTypeDef](./type_defs.md#cryptogramauthresponsetypedef)
- [DecryptDataOutputTypeDef](./type_defs.md#decryptdataoutputtypedef)
- [EncryptDataOutputTypeDef](./type_defs.md#encryptdataoutputtypedef)
- [GenerateAs2805KekValidationOutputTypeDef](./type_defs.md#generateas2805kekvalidationoutputtypedef)
- [GenerateCardValidationDataOutputTypeDef](./type_defs.md#generatecardvalidationdataoutputtypedef)
- [GenerateMacOutputTypeDef](./type_defs.md#generatemacoutputtypedef)
- [ReEncryptDataOutputTypeDef](./type_defs.md#reencryptdataoutputtypedef)
- [TranslatePinDataOutputTypeDef](./type_defs.md#translatepindataoutputtypedef)
- [VerifyAuthRequestCryptogramOutputTypeDef](./type_defs.md#verifyauthrequestcryptogramoutputtypedef)
- [VerifyCardValidationDataOutputTypeDef](./type_defs.md#verifycardvalidationdataoutputtypedef)
- [VerifyMacOutputTypeDef](./type_defs.md#verifymacoutputtypedef)
- [VerifyPinDataOutputTypeDef](./type_defs.md#verifypindataoutputtypedef)
- [IncomingDiffieHellmanTr31KeyBlockTypeDef](./type_defs.md#incomingdiffiehellmantr31keyblocktypedef)
- [WrappedKeyMaterialTypeDef](./type_defs.md#wrappedkeymaterialtypedef)
- [EncryptionDecryptionAttributesTypeDef](./type_defs.md#encryptiondecryptionattributestypedef)
- [ReEncryptionAttributesTypeDef](./type_defs.md#reencryptionattributestypedef)
- [GenerateMacEmvPinChangeOutputTypeDef](./type_defs.md#generatemacemvpinchangeoutputtypedef)
- [GeneratePinDataOutputTypeDef](./type_defs.md#generatepindataoutputtypedef)
- [MacAlgorithmEmvTypeDef](./type_defs.md#macalgorithmemvtypedef)
- [OutgoingKeyMaterialTypeDef](./type_defs.md#outgoingkeymaterialtypedef)
- [PinGenerationAttributesTypeDef](./type_defs.md#pingenerationattributestypedef)
- [PinVerificationAttributesTypeDef](./type_defs.md#pinverificationattributestypedef)
- [SessionKeyDerivationTypeDef](./type_defs.md#sessionkeyderivationtypedef)
- [TranslateKeyMaterialOutputTypeDef](./type_defs.md#translatekeymaterialoutputtypedef)
- [TranslationIsoFormatsTypeDef](./type_defs.md#translationisoformatstypedef)
- [DerivationMethodAttributesTypeDef](./type_defs.md#derivationmethodattributestypedef)
- [GenerateAs2805KekValidationInputTypeDef](./type_defs.md#generateas2805kekvalidationinputtypedef)
- [GenerateCardValidationDataInputTypeDef](./type_defs.md#generatecardvalidationdatainputtypedef)
- [VerifyCardValidationDataInputTypeDef](./type_defs.md#verifycardvalidationdatainputtypedef)
- [IncomingKeyMaterialTypeDef](./type_defs.md#incomingkeymaterialtypedef)
- [WrappedKeyTypeDef](./type_defs.md#wrappedkeytypedef)
- [MacAttributesTypeDef](./type_defs.md#macattributestypedef)
- [VerifyAuthRequestCryptogramInputTypeDef](./type_defs.md#verifyauthrequestcryptograminputtypedef)
- [GenerateMacEmvPinChangeInputTypeDef](./type_defs.md#generatemacemvpinchangeinputtypedef)
- [TranslateKeyMaterialInputTypeDef](./type_defs.md#translatekeymaterialinputtypedef)
- [DecryptDataInputTypeDef](./type_defs.md#decryptdatainputtypedef)
- [EncryptDataInputTypeDef](./type_defs.md#encryptdatainputtypedef)
- [GeneratePinDataInputTypeDef](./type_defs.md#generatepindatainputtypedef)
- [ReEncryptDataInputTypeDef](./type_defs.md#reencryptdatainputtypedef)
- [TranslatePinDataInputTypeDef](./type_defs.md#translatepindatainputtypedef)
- [VerifyPinDataInputTypeDef](./type_defs.md#verifypindatainputtypedef)
- [GenerateMacInputTypeDef](./type_defs.md#generatemacinputtypedef)
- [VerifyMacInputTypeDef](./type_defs.md#verifymacinputtypedef)

