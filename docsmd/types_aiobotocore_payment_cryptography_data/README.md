# PaymentCryptographyDataPlane module

> [Index](../README.md) > PaymentCryptographyDataPlane


!!! note ""

    Auto-generated documentation for [PaymentCryptographyDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
    type annotations stubs module [types-aiobotocore-payment-cryptography-data](https://pypi.org/project/types-aiobotocore-payment-cryptography-data/).

## How to install



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
- [EncryptionModeType](./literals.md#encryptionmodetype)
- [MacAlgorithmType](./literals.md#macalgorithmtype)
- [MajorKeyDerivationModeType](./literals.md#majorkeyderivationmodetype)
- [PaddingTypeType](./literals.md#paddingtypetype)
- [PinBlockFormatForPinDataType](./literals.md#pinblockformatforpindatatype)
- [SessionKeyDerivationModeType](./literals.md#sessionkeyderivationmodetype)
- [PaymentCryptographyDataPlaneServiceName](./literals.md#paymentcryptographydataplaneservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AmexCardSecurityCodeVersion1TypeDef](./type_defs.md#amexcardsecuritycodeversion1typedef)
- [AmexCardSecurityCodeVersion2TypeDef](./type_defs.md#amexcardsecuritycodeversion2typedef)
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
- [DukptAttributesTypeDef](./type_defs.md#dukptattributestypedef)
- [DukptDerivationAttributesTypeDef](./type_defs.md#dukptderivationattributestypedef)
- [DukptEncryptionAttributesTypeDef](./type_defs.md#dukptencryptionattributestypedef)
- [SymmetricEncryptionAttributesTypeDef](./type_defs.md#symmetricencryptionattributestypedef)
- [PinDataTypeDef](./type_defs.md#pindatatypedef)
- [Ibm3624NaturalPinTypeDef](./type_defs.md#ibm3624naturalpintypedef)
- [Ibm3624PinFromOffsetTypeDef](./type_defs.md#ibm3624pinfromoffsettypedef)
- [Ibm3624PinOffsetTypeDef](./type_defs.md#ibm3624pinoffsettypedef)
- [Ibm3624PinVerificationTypeDef](./type_defs.md#ibm3624pinverificationtypedef)
- [Ibm3624RandomPinTypeDef](./type_defs.md#ibm3624randompintypedef)
- [MacAlgorithmDukptTypeDef](./type_defs.md#macalgorithmdukpttypedef)
- [SessionKeyDerivationValueTypeDef](./type_defs.md#sessionkeyderivationvaluetypedef)
- [VisaPinTypeDef](./type_defs.md#visapintypedef)
- [VisaPinVerificationValueTypeDef](./type_defs.md#visapinverificationvaluetypedef)
- [VisaPinVerificationTypeDef](./type_defs.md#visapinverificationtypedef)
- [SessionKeyAmexTypeDef](./type_defs.md#sessionkeyamextypedef)
- [SessionKeyEmv2000TypeDef](./type_defs.md#sessionkeyemv2000typedef)
- [SessionKeyEmvCommonTypeDef](./type_defs.md#sessionkeyemvcommontypedef)
- [SessionKeyMastercardTypeDef](./type_defs.md#sessionkeymastercardtypedef)
- [SessionKeyVisaTypeDef](./type_defs.md#sessionkeyvisatypedef)
- [TranslationPinDataIsoFormat034TypeDef](./type_defs.md#translationpindataisoformat034typedef)
- [CardGenerationAttributesTypeDef](./type_defs.md#cardgenerationattributestypedef)
- [CardVerificationAttributesTypeDef](./type_defs.md#cardverificationattributestypedef)
- [CryptogramAuthResponseTypeDef](./type_defs.md#cryptogramauthresponsetypedef)
- [DecryptDataOutputTypeDef](./type_defs.md#decryptdataoutputtypedef)
- [EncryptDataOutputTypeDef](./type_defs.md#encryptdataoutputtypedef)
- [GenerateCardValidationDataOutputTypeDef](./type_defs.md#generatecardvalidationdataoutputtypedef)
- [GenerateMacOutputTypeDef](./type_defs.md#generatemacoutputtypedef)
- [ReEncryptDataOutputTypeDef](./type_defs.md#reencryptdataoutputtypedef)
- [TranslatePinDataOutputTypeDef](./type_defs.md#translatepindataoutputtypedef)
- [VerifyAuthRequestCryptogramOutputTypeDef](./type_defs.md#verifyauthrequestcryptogramoutputtypedef)
- [VerifyCardValidationDataOutputTypeDef](./type_defs.md#verifycardvalidationdataoutputtypedef)
- [VerifyMacOutputTypeDef](./type_defs.md#verifymacoutputtypedef)
- [VerifyPinDataOutputTypeDef](./type_defs.md#verifypindataoutputtypedef)
- [EncryptionDecryptionAttributesTypeDef](./type_defs.md#encryptiondecryptionattributestypedef)
- [ReEncryptionAttributesTypeDef](./type_defs.md#reencryptionattributestypedef)
- [GeneratePinDataOutputTypeDef](./type_defs.md#generatepindataoutputtypedef)
- [MacAlgorithmEmvTypeDef](./type_defs.md#macalgorithmemvtypedef)
- [PinGenerationAttributesTypeDef](./type_defs.md#pingenerationattributestypedef)
- [PinVerificationAttributesTypeDef](./type_defs.md#pinverificationattributestypedef)
- [SessionKeyDerivationTypeDef](./type_defs.md#sessionkeyderivationtypedef)
- [TranslationIsoFormatsTypeDef](./type_defs.md#translationisoformatstypedef)
- [GenerateCardValidationDataInputRequestTypeDef](./type_defs.md#generatecardvalidationdatainputrequesttypedef)
- [VerifyCardValidationDataInputRequestTypeDef](./type_defs.md#verifycardvalidationdatainputrequesttypedef)
- [DecryptDataInputRequestTypeDef](./type_defs.md#decryptdatainputrequesttypedef)
- [EncryptDataInputRequestTypeDef](./type_defs.md#encryptdatainputrequesttypedef)
- [ReEncryptDataInputRequestTypeDef](./type_defs.md#reencryptdatainputrequesttypedef)
- [MacAttributesTypeDef](./type_defs.md#macattributestypedef)
- [GeneratePinDataInputRequestTypeDef](./type_defs.md#generatepindatainputrequesttypedef)
- [VerifyPinDataInputRequestTypeDef](./type_defs.md#verifypindatainputrequesttypedef)
- [VerifyAuthRequestCryptogramInputRequestTypeDef](./type_defs.md#verifyauthrequestcryptograminputrequesttypedef)
- [TranslatePinDataInputRequestTypeDef](./type_defs.md#translatepindatainputrequesttypedef)
- [GenerateMacInputRequestTypeDef](./type_defs.md#generatemacinputrequesttypedef)
- [VerifyMacInputRequestTypeDef](./type_defs.md#verifymacinputrequesttypedef)

