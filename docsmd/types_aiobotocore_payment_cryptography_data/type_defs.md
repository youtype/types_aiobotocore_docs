# Type definitions

> [Index](../README.md) > [PaymentCryptographyDataPlane](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PaymentCryptographyDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
    type annotations stubs module [types-aiobotocore-payment-cryptography-data](https://pypi.org/project/types-aiobotocore-payment-cryptography-data/).



## AmexCardSecurityCodeVersion1TypeDef

```python
# AmexCardSecurityCodeVersion1TypeDef definition

class AmexCardSecurityCodeVersion1TypeDef(TypedDict):
    CardExpiryDate: str,
```

## AmexCardSecurityCodeVersion2TypeDef

```python
# AmexCardSecurityCodeVersion2TypeDef definition

class AmexCardSecurityCodeVersion2TypeDef(TypedDict):
    CardExpiryDate: str,
    ServiceCode: str,
```

## AsymmetricEncryptionAttributesTypeDef

```python
# AsymmetricEncryptionAttributesTypeDef definition

class AsymmetricEncryptionAttributesTypeDef(TypedDict):
    PaddingType: NotRequired[PaddingTypeType],  # (1)
```

1. See [:material-code-brackets: PaddingTypeType](./literals.md#paddingtypetype) 
## CardHolderVerificationValueTypeDef

```python
# CardHolderVerificationValueTypeDef definition

class CardHolderVerificationValueTypeDef(TypedDict):
    ApplicationTransactionCounter: str,
    PanSequenceNumber: str,
    UnpredictableNumber: str,
```

## CardVerificationValue1TypeDef

```python
# CardVerificationValue1TypeDef definition

class CardVerificationValue1TypeDef(TypedDict):
    CardExpiryDate: str,
    ServiceCode: str,
```

## CardVerificationValue2TypeDef

```python
# CardVerificationValue2TypeDef definition

class CardVerificationValue2TypeDef(TypedDict):
    CardExpiryDate: str,
```

## DynamicCardVerificationCodeTypeDef

```python
# DynamicCardVerificationCodeTypeDef definition

class DynamicCardVerificationCodeTypeDef(TypedDict):
    ApplicationTransactionCounter: str,
    PanSequenceNumber: str,
    TrackData: str,
    UnpredictableNumber: str,
```

## DynamicCardVerificationValueTypeDef

```python
# DynamicCardVerificationValueTypeDef definition

class DynamicCardVerificationValueTypeDef(TypedDict):
    ApplicationTransactionCounter: str,
    CardExpiryDate: str,
    PanSequenceNumber: str,
    ServiceCode: str,
```

## DiscoverDynamicCardVerificationCodeTypeDef

```python
# DiscoverDynamicCardVerificationCodeTypeDef definition

class DiscoverDynamicCardVerificationCodeTypeDef(TypedDict):
    ApplicationTransactionCounter: str,
    CardExpiryDate: str,
    UnpredictableNumber: str,
```

## CryptogramVerificationArpcMethod1TypeDef

```python
# CryptogramVerificationArpcMethod1TypeDef definition

class CryptogramVerificationArpcMethod1TypeDef(TypedDict):
    AuthResponseCode: str,
```

## CryptogramVerificationArpcMethod2TypeDef

```python
# CryptogramVerificationArpcMethod2TypeDef definition

class CryptogramVerificationArpcMethod2TypeDef(TypedDict):
    CardStatusUpdate: str,
    ProprietaryAuthenticationData: NotRequired[str],
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

## DukptAttributesTypeDef

```python
# DukptAttributesTypeDef definition

class DukptAttributesTypeDef(TypedDict):
    DukptDerivationType: DukptDerivationTypeType,  # (1)
    KeySerialNumber: str,
```

1. See [:material-code-brackets: DukptDerivationTypeType](./literals.md#dukptderivationtypetype) 
## DukptDerivationAttributesTypeDef

```python
# DukptDerivationAttributesTypeDef definition

class DukptDerivationAttributesTypeDef(TypedDict):
    KeySerialNumber: str,
    DukptKeyDerivationType: NotRequired[DukptDerivationTypeType],  # (1)
    DukptKeyVariant: NotRequired[DukptKeyVariantType],  # (2)
```

1. See [:material-code-brackets: DukptDerivationTypeType](./literals.md#dukptderivationtypetype) 
2. See [:material-code-brackets: DukptKeyVariantType](./literals.md#dukptkeyvarianttype) 
## DukptEncryptionAttributesTypeDef

```python
# DukptEncryptionAttributesTypeDef definition

class DukptEncryptionAttributesTypeDef(TypedDict):
    KeySerialNumber: str,
    DukptKeyDerivationType: NotRequired[DukptDerivationTypeType],  # (1)
    DukptKeyVariant: NotRequired[DukptKeyVariantType],  # (2)
    InitializationVector: NotRequired[str],
    Mode: NotRequired[DukptEncryptionModeType],  # (3)
```

1. See [:material-code-brackets: DukptDerivationTypeType](./literals.md#dukptderivationtypetype) 
2. See [:material-code-brackets: DukptKeyVariantType](./literals.md#dukptkeyvarianttype) 
3. See [:material-code-brackets: DukptEncryptionModeType](./literals.md#dukptencryptionmodetype) 
## SymmetricEncryptionAttributesTypeDef

```python
# SymmetricEncryptionAttributesTypeDef definition

class SymmetricEncryptionAttributesTypeDef(TypedDict):
    Mode: EncryptionModeType,  # (1)
    InitializationVector: NotRequired[str],
    PaddingType: NotRequired[PaddingTypeType],  # (2)
```

1. See [:material-code-brackets: EncryptionModeType](./literals.md#encryptionmodetype) 
2. See [:material-code-brackets: PaddingTypeType](./literals.md#paddingtypetype) 
## PinDataTypeDef

```python
# PinDataTypeDef definition

class PinDataTypeDef(TypedDict):
    PinOffset: NotRequired[str],
    VerificationValue: NotRequired[str],
```

## Ibm3624NaturalPinTypeDef

```python
# Ibm3624NaturalPinTypeDef definition

class Ibm3624NaturalPinTypeDef(TypedDict):
    DecimalizationTable: str,
    PinValidationData: str,
    PinValidationDataPadCharacter: str,
```

## Ibm3624PinFromOffsetTypeDef

```python
# Ibm3624PinFromOffsetTypeDef definition

class Ibm3624PinFromOffsetTypeDef(TypedDict):
    DecimalizationTable: str,
    PinOffset: str,
    PinValidationData: str,
    PinValidationDataPadCharacter: str,
```

## Ibm3624PinOffsetTypeDef

```python
# Ibm3624PinOffsetTypeDef definition

class Ibm3624PinOffsetTypeDef(TypedDict):
    DecimalizationTable: str,
    EncryptedPinBlock: str,
    PinValidationData: str,
    PinValidationDataPadCharacter: str,
```

## Ibm3624PinVerificationTypeDef

```python
# Ibm3624PinVerificationTypeDef definition

class Ibm3624PinVerificationTypeDef(TypedDict):
    DecimalizationTable: str,
    PinOffset: str,
    PinValidationData: str,
    PinValidationDataPadCharacter: str,
```

## Ibm3624RandomPinTypeDef

```python
# Ibm3624RandomPinTypeDef definition

class Ibm3624RandomPinTypeDef(TypedDict):
    DecimalizationTable: str,
    PinValidationData: str,
    PinValidationDataPadCharacter: str,
```

## MacAlgorithmDukptTypeDef

```python
# MacAlgorithmDukptTypeDef definition

class MacAlgorithmDukptTypeDef(TypedDict):
    DukptKeyVariant: DukptKeyVariantType,  # (2)
    KeySerialNumber: str,
    DukptDerivationType: NotRequired[DukptDerivationTypeType],  # (1)
```

1. See [:material-code-brackets: DukptDerivationTypeType](./literals.md#dukptderivationtypetype) 
2. See [:material-code-brackets: DukptKeyVariantType](./literals.md#dukptkeyvarianttype) 
## SessionKeyDerivationValueTypeDef

```python
# SessionKeyDerivationValueTypeDef definition

class SessionKeyDerivationValueTypeDef(TypedDict):
    ApplicationCryptogram: NotRequired[str],
    ApplicationTransactionCounter: NotRequired[str],
```

## VisaPinTypeDef

```python
# VisaPinTypeDef definition

class VisaPinTypeDef(TypedDict):
    PinVerificationKeyIndex: int,
```

## VisaPinVerificationValueTypeDef

```python
# VisaPinVerificationValueTypeDef definition

class VisaPinVerificationValueTypeDef(TypedDict):
    EncryptedPinBlock: str,
    PinVerificationKeyIndex: int,
```

## VisaPinVerificationTypeDef

```python
# VisaPinVerificationTypeDef definition

class VisaPinVerificationTypeDef(TypedDict):
    PinVerificationKeyIndex: int,
    VerificationValue: str,
```

## SessionKeyAmexTypeDef

```python
# SessionKeyAmexTypeDef definition

class SessionKeyAmexTypeDef(TypedDict):
    PanSequenceNumber: str,
    PrimaryAccountNumber: str,
```

## SessionKeyEmv2000TypeDef

```python
# SessionKeyEmv2000TypeDef definition

class SessionKeyEmv2000TypeDef(TypedDict):
    ApplicationTransactionCounter: str,
    PanSequenceNumber: str,
    PrimaryAccountNumber: str,
```

## SessionKeyEmvCommonTypeDef

```python
# SessionKeyEmvCommonTypeDef definition

class SessionKeyEmvCommonTypeDef(TypedDict):
    ApplicationTransactionCounter: str,
    PanSequenceNumber: str,
    PrimaryAccountNumber: str,
```

## SessionKeyMastercardTypeDef

```python
# SessionKeyMastercardTypeDef definition

class SessionKeyMastercardTypeDef(TypedDict):
    ApplicationTransactionCounter: str,
    PanSequenceNumber: str,
    PrimaryAccountNumber: str,
    UnpredictableNumber: str,
```

## SessionKeyVisaTypeDef

```python
# SessionKeyVisaTypeDef definition

class SessionKeyVisaTypeDef(TypedDict):
    PanSequenceNumber: str,
    PrimaryAccountNumber: str,
```

## TranslationPinDataIsoFormat034TypeDef

```python
# TranslationPinDataIsoFormat034TypeDef definition

class TranslationPinDataIsoFormat034TypeDef(TypedDict):
    PrimaryAccountNumber: str,
```

## CardGenerationAttributesTypeDef

```python
# CardGenerationAttributesTypeDef definition

class CardGenerationAttributesTypeDef(TypedDict):
    AmexCardSecurityCodeVersion1: NotRequired[AmexCardSecurityCodeVersion1TypeDef],  # (1)
    AmexCardSecurityCodeVersion2: NotRequired[AmexCardSecurityCodeVersion2TypeDef],  # (2)
    CardHolderVerificationValue: NotRequired[CardHolderVerificationValueTypeDef],  # (3)
    CardVerificationValue1: NotRequired[CardVerificationValue1TypeDef],  # (4)
    CardVerificationValue2: NotRequired[CardVerificationValue2TypeDef],  # (5)
    DynamicCardVerificationCode: NotRequired[DynamicCardVerificationCodeTypeDef],  # (6)
    DynamicCardVerificationValue: NotRequired[DynamicCardVerificationValueTypeDef],  # (7)
```

1. See [:material-code-braces: AmexCardSecurityCodeVersion1TypeDef](./type_defs.md#amexcardsecuritycodeversion1typedef) 
2. See [:material-code-braces: AmexCardSecurityCodeVersion2TypeDef](./type_defs.md#amexcardsecuritycodeversion2typedef) 
3. See [:material-code-braces: CardHolderVerificationValueTypeDef](./type_defs.md#cardholderverificationvaluetypedef) 
4. See [:material-code-braces: CardVerificationValue1TypeDef](./type_defs.md#cardverificationvalue1typedef) 
5. See [:material-code-braces: CardVerificationValue2TypeDef](./type_defs.md#cardverificationvalue2typedef) 
6. See [:material-code-braces: DynamicCardVerificationCodeTypeDef](./type_defs.md#dynamiccardverificationcodetypedef) 
7. See [:material-code-braces: DynamicCardVerificationValueTypeDef](./type_defs.md#dynamiccardverificationvaluetypedef) 
## CardVerificationAttributesTypeDef

```python
# CardVerificationAttributesTypeDef definition

class CardVerificationAttributesTypeDef(TypedDict):
    AmexCardSecurityCodeVersion1: NotRequired[AmexCardSecurityCodeVersion1TypeDef],  # (1)
    AmexCardSecurityCodeVersion2: NotRequired[AmexCardSecurityCodeVersion2TypeDef],  # (2)
    CardHolderVerificationValue: NotRequired[CardHolderVerificationValueTypeDef],  # (3)
    CardVerificationValue1: NotRequired[CardVerificationValue1TypeDef],  # (4)
    CardVerificationValue2: NotRequired[CardVerificationValue2TypeDef],  # (5)
    DiscoverDynamicCardVerificationCode: NotRequired[DiscoverDynamicCardVerificationCodeTypeDef],  # (6)
    DynamicCardVerificationCode: NotRequired[DynamicCardVerificationCodeTypeDef],  # (7)
    DynamicCardVerificationValue: NotRequired[DynamicCardVerificationValueTypeDef],  # (8)
```

1. See [:material-code-braces: AmexCardSecurityCodeVersion1TypeDef](./type_defs.md#amexcardsecuritycodeversion1typedef) 
2. See [:material-code-braces: AmexCardSecurityCodeVersion2TypeDef](./type_defs.md#amexcardsecuritycodeversion2typedef) 
3. See [:material-code-braces: CardHolderVerificationValueTypeDef](./type_defs.md#cardholderverificationvaluetypedef) 
4. See [:material-code-braces: CardVerificationValue1TypeDef](./type_defs.md#cardverificationvalue1typedef) 
5. See [:material-code-braces: CardVerificationValue2TypeDef](./type_defs.md#cardverificationvalue2typedef) 
6. See [:material-code-braces: DiscoverDynamicCardVerificationCodeTypeDef](./type_defs.md#discoverdynamiccardverificationcodetypedef) 
7. See [:material-code-braces: DynamicCardVerificationCodeTypeDef](./type_defs.md#dynamiccardverificationcodetypedef) 
8. See [:material-code-braces: DynamicCardVerificationValueTypeDef](./type_defs.md#dynamiccardverificationvaluetypedef) 
## CryptogramAuthResponseTypeDef

```python
# CryptogramAuthResponseTypeDef definition

class CryptogramAuthResponseTypeDef(TypedDict):
    ArpcMethod1: NotRequired[CryptogramVerificationArpcMethod1TypeDef],  # (1)
    ArpcMethod2: NotRequired[CryptogramVerificationArpcMethod2TypeDef],  # (2)
```

1. See [:material-code-braces: CryptogramVerificationArpcMethod1TypeDef](./type_defs.md#cryptogramverificationarpcmethod1typedef) 
2. See [:material-code-braces: CryptogramVerificationArpcMethod2TypeDef](./type_defs.md#cryptogramverificationarpcmethod2typedef) 
## DecryptDataOutputTypeDef

```python
# DecryptDataOutputTypeDef definition

class DecryptDataOutputTypeDef(TypedDict):
    KeyArn: str,
    KeyCheckValue: str,
    PlainText: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EncryptDataOutputTypeDef

```python
# EncryptDataOutputTypeDef definition

class EncryptDataOutputTypeDef(TypedDict):
    CipherText: str,
    KeyArn: str,
    KeyCheckValue: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateCardValidationDataOutputTypeDef

```python
# GenerateCardValidationDataOutputTypeDef definition

class GenerateCardValidationDataOutputTypeDef(TypedDict):
    KeyArn: str,
    KeyCheckValue: str,
    ValidationData: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateMacOutputTypeDef

```python
# GenerateMacOutputTypeDef definition

class GenerateMacOutputTypeDef(TypedDict):
    KeyArn: str,
    KeyCheckValue: str,
    Mac: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReEncryptDataOutputTypeDef

```python
# ReEncryptDataOutputTypeDef definition

class ReEncryptDataOutputTypeDef(TypedDict):
    CipherText: str,
    KeyArn: str,
    KeyCheckValue: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TranslatePinDataOutputTypeDef

```python
# TranslatePinDataOutputTypeDef definition

class TranslatePinDataOutputTypeDef(TypedDict):
    KeyArn: str,
    KeyCheckValue: str,
    PinBlock: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VerifyAuthRequestCryptogramOutputTypeDef

```python
# VerifyAuthRequestCryptogramOutputTypeDef definition

class VerifyAuthRequestCryptogramOutputTypeDef(TypedDict):
    AuthResponseValue: str,
    KeyArn: str,
    KeyCheckValue: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VerifyCardValidationDataOutputTypeDef

```python
# VerifyCardValidationDataOutputTypeDef definition

class VerifyCardValidationDataOutputTypeDef(TypedDict):
    KeyArn: str,
    KeyCheckValue: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VerifyMacOutputTypeDef

```python
# VerifyMacOutputTypeDef definition

class VerifyMacOutputTypeDef(TypedDict):
    KeyArn: str,
    KeyCheckValue: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VerifyPinDataOutputTypeDef

```python
# VerifyPinDataOutputTypeDef definition

class VerifyPinDataOutputTypeDef(TypedDict):
    EncryptionKeyArn: str,
    EncryptionKeyCheckValue: str,
    VerificationKeyArn: str,
    VerificationKeyCheckValue: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EncryptionDecryptionAttributesTypeDef

```python
# EncryptionDecryptionAttributesTypeDef definition

class EncryptionDecryptionAttributesTypeDef(TypedDict):
    Asymmetric: NotRequired[AsymmetricEncryptionAttributesTypeDef],  # (1)
    Dukpt: NotRequired[DukptEncryptionAttributesTypeDef],  # (2)
    Symmetric: NotRequired[SymmetricEncryptionAttributesTypeDef],  # (3)
```

1. See [:material-code-braces: AsymmetricEncryptionAttributesTypeDef](./type_defs.md#asymmetricencryptionattributestypedef) 
2. See [:material-code-braces: DukptEncryptionAttributesTypeDef](./type_defs.md#dukptencryptionattributestypedef) 
3. See [:material-code-braces: SymmetricEncryptionAttributesTypeDef](./type_defs.md#symmetricencryptionattributestypedef) 
## ReEncryptionAttributesTypeDef

```python
# ReEncryptionAttributesTypeDef definition

class ReEncryptionAttributesTypeDef(TypedDict):
    Dukpt: NotRequired[DukptEncryptionAttributesTypeDef],  # (1)
    Symmetric: NotRequired[SymmetricEncryptionAttributesTypeDef],  # (2)
```

1. See [:material-code-braces: DukptEncryptionAttributesTypeDef](./type_defs.md#dukptencryptionattributestypedef) 
2. See [:material-code-braces: SymmetricEncryptionAttributesTypeDef](./type_defs.md#symmetricencryptionattributestypedef) 
## GeneratePinDataOutputTypeDef

```python
# GeneratePinDataOutputTypeDef definition

class GeneratePinDataOutputTypeDef(TypedDict):
    EncryptedPinBlock: str,
    EncryptionKeyArn: str,
    EncryptionKeyCheckValue: str,
    GenerationKeyArn: str,
    GenerationKeyCheckValue: str,
    PinData: PinDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PinDataTypeDef](./type_defs.md#pindatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MacAlgorithmEmvTypeDef

```python
# MacAlgorithmEmvTypeDef definition

class MacAlgorithmEmvTypeDef(TypedDict):
    MajorKeyDerivationMode: MajorKeyDerivationModeType,  # (1)
    PanSequenceNumber: str,
    PrimaryAccountNumber: str,
    SessionKeyDerivationMode: SessionKeyDerivationModeType,  # (2)
    SessionKeyDerivationValue: SessionKeyDerivationValueTypeDef,  # (3)
```

1. See [:material-code-brackets: MajorKeyDerivationModeType](./literals.md#majorkeyderivationmodetype) 
2. See [:material-code-brackets: SessionKeyDerivationModeType](./literals.md#sessionkeyderivationmodetype) 
3. See [:material-code-braces: SessionKeyDerivationValueTypeDef](./type_defs.md#sessionkeyderivationvaluetypedef) 
## PinGenerationAttributesTypeDef

```python
# PinGenerationAttributesTypeDef definition

class PinGenerationAttributesTypeDef(TypedDict):
    Ibm3624NaturalPin: NotRequired[Ibm3624NaturalPinTypeDef],  # (1)
    Ibm3624PinFromOffset: NotRequired[Ibm3624PinFromOffsetTypeDef],  # (2)
    Ibm3624PinOffset: NotRequired[Ibm3624PinOffsetTypeDef],  # (3)
    Ibm3624RandomPin: NotRequired[Ibm3624RandomPinTypeDef],  # (4)
    VisaPin: NotRequired[VisaPinTypeDef],  # (5)
    VisaPinVerificationValue: NotRequired[VisaPinVerificationValueTypeDef],  # (6)
```

1. See [:material-code-braces: Ibm3624NaturalPinTypeDef](./type_defs.md#ibm3624naturalpintypedef) 
2. See [:material-code-braces: Ibm3624PinFromOffsetTypeDef](./type_defs.md#ibm3624pinfromoffsettypedef) 
3. See [:material-code-braces: Ibm3624PinOffsetTypeDef](./type_defs.md#ibm3624pinoffsettypedef) 
4. See [:material-code-braces: Ibm3624RandomPinTypeDef](./type_defs.md#ibm3624randompintypedef) 
5. See [:material-code-braces: VisaPinTypeDef](./type_defs.md#visapintypedef) 
6. See [:material-code-braces: VisaPinVerificationValueTypeDef](./type_defs.md#visapinverificationvaluetypedef) 
## PinVerificationAttributesTypeDef

```python
# PinVerificationAttributesTypeDef definition

class PinVerificationAttributesTypeDef(TypedDict):
    Ibm3624Pin: NotRequired[Ibm3624PinVerificationTypeDef],  # (1)
    VisaPin: NotRequired[VisaPinVerificationTypeDef],  # (2)
```

1. See [:material-code-braces: Ibm3624PinVerificationTypeDef](./type_defs.md#ibm3624pinverificationtypedef) 
2. See [:material-code-braces: VisaPinVerificationTypeDef](./type_defs.md#visapinverificationtypedef) 
## SessionKeyDerivationTypeDef

```python
# SessionKeyDerivationTypeDef definition

class SessionKeyDerivationTypeDef(TypedDict):
    Amex: NotRequired[SessionKeyAmexTypeDef],  # (1)
    Emv2000: NotRequired[SessionKeyEmv2000TypeDef],  # (2)
    EmvCommon: NotRequired[SessionKeyEmvCommonTypeDef],  # (3)
    Mastercard: NotRequired[SessionKeyMastercardTypeDef],  # (4)
    Visa: NotRequired[SessionKeyVisaTypeDef],  # (5)
```

1. See [:material-code-braces: SessionKeyAmexTypeDef](./type_defs.md#sessionkeyamextypedef) 
2. See [:material-code-braces: SessionKeyEmv2000TypeDef](./type_defs.md#sessionkeyemv2000typedef) 
3. See [:material-code-braces: SessionKeyEmvCommonTypeDef](./type_defs.md#sessionkeyemvcommontypedef) 
4. See [:material-code-braces: SessionKeyMastercardTypeDef](./type_defs.md#sessionkeymastercardtypedef) 
5. See [:material-code-braces: SessionKeyVisaTypeDef](./type_defs.md#sessionkeyvisatypedef) 
## TranslationIsoFormatsTypeDef

```python
# TranslationIsoFormatsTypeDef definition

class TranslationIsoFormatsTypeDef(TypedDict):
    IsoFormat0: NotRequired[TranslationPinDataIsoFormat034TypeDef],  # (1)
    IsoFormat1: NotRequired[Mapping[str, Any]],
    IsoFormat3: NotRequired[TranslationPinDataIsoFormat034TypeDef],  # (1)
    IsoFormat4: NotRequired[TranslationPinDataIsoFormat034TypeDef],  # (1)
```

1. See [:material-code-braces: TranslationPinDataIsoFormat034TypeDef](./type_defs.md#translationpindataisoformat034typedef) 
2. See [:material-code-braces: TranslationPinDataIsoFormat034TypeDef](./type_defs.md#translationpindataisoformat034typedef) 
3. See [:material-code-braces: TranslationPinDataIsoFormat034TypeDef](./type_defs.md#translationpindataisoformat034typedef) 
## GenerateCardValidationDataInputRequestTypeDef

```python
# GenerateCardValidationDataInputRequestTypeDef definition

class GenerateCardValidationDataInputRequestTypeDef(TypedDict):
    GenerationAttributes: CardGenerationAttributesTypeDef,  # (1)
    KeyIdentifier: str,
    PrimaryAccountNumber: str,
    ValidationDataLength: NotRequired[int],
```

1. See [:material-code-braces: CardGenerationAttributesTypeDef](./type_defs.md#cardgenerationattributestypedef) 
## VerifyCardValidationDataInputRequestTypeDef

```python
# VerifyCardValidationDataInputRequestTypeDef definition

class VerifyCardValidationDataInputRequestTypeDef(TypedDict):
    KeyIdentifier: str,
    PrimaryAccountNumber: str,
    ValidationData: str,
    VerificationAttributes: CardVerificationAttributesTypeDef,  # (1)
```

1. See [:material-code-braces: CardVerificationAttributesTypeDef](./type_defs.md#cardverificationattributestypedef) 
## DecryptDataInputRequestTypeDef

```python
# DecryptDataInputRequestTypeDef definition

class DecryptDataInputRequestTypeDef(TypedDict):
    CipherText: str,
    DecryptionAttributes: EncryptionDecryptionAttributesTypeDef,  # (1)
    KeyIdentifier: str,
```

1. See [:material-code-braces: EncryptionDecryptionAttributesTypeDef](./type_defs.md#encryptiondecryptionattributestypedef) 
## EncryptDataInputRequestTypeDef

```python
# EncryptDataInputRequestTypeDef definition

class EncryptDataInputRequestTypeDef(TypedDict):
    EncryptionAttributes: EncryptionDecryptionAttributesTypeDef,  # (1)
    KeyIdentifier: str,
    PlainText: str,
```

1. See [:material-code-braces: EncryptionDecryptionAttributesTypeDef](./type_defs.md#encryptiondecryptionattributestypedef) 
## ReEncryptDataInputRequestTypeDef

```python
# ReEncryptDataInputRequestTypeDef definition

class ReEncryptDataInputRequestTypeDef(TypedDict):
    CipherText: str,
    IncomingEncryptionAttributes: ReEncryptionAttributesTypeDef,  # (1)
    IncomingKeyIdentifier: str,
    OutgoingEncryptionAttributes: ReEncryptionAttributesTypeDef,  # (1)
    OutgoingKeyIdentifier: str,
```

1. See [:material-code-braces: ReEncryptionAttributesTypeDef](./type_defs.md#reencryptionattributestypedef) 
2. See [:material-code-braces: ReEncryptionAttributesTypeDef](./type_defs.md#reencryptionattributestypedef) 
## MacAttributesTypeDef

```python
# MacAttributesTypeDef definition

class MacAttributesTypeDef(TypedDict):
    Algorithm: NotRequired[MacAlgorithmType],  # (1)
    DukptCmac: NotRequired[MacAlgorithmDukptTypeDef],  # (2)
    DukptIso9797Algorithm1: NotRequired[MacAlgorithmDukptTypeDef],  # (2)
    DukptIso9797Algorithm3: NotRequired[MacAlgorithmDukptTypeDef],  # (2)
    EmvMac: NotRequired[MacAlgorithmEmvTypeDef],  # (5)
```

1. See [:material-code-brackets: MacAlgorithmType](./literals.md#macalgorithmtype) 
2. See [:material-code-braces: MacAlgorithmDukptTypeDef](./type_defs.md#macalgorithmdukpttypedef) 
3. See [:material-code-braces: MacAlgorithmDukptTypeDef](./type_defs.md#macalgorithmdukpttypedef) 
4. See [:material-code-braces: MacAlgorithmDukptTypeDef](./type_defs.md#macalgorithmdukpttypedef) 
5. See [:material-code-braces: MacAlgorithmEmvTypeDef](./type_defs.md#macalgorithmemvtypedef) 
## GeneratePinDataInputRequestTypeDef

```python
# GeneratePinDataInputRequestTypeDef definition

class GeneratePinDataInputRequestTypeDef(TypedDict):
    EncryptionKeyIdentifier: str,
    GenerationAttributes: PinGenerationAttributesTypeDef,  # (1)
    GenerationKeyIdentifier: str,
    PinBlockFormat: PinBlockFormatForPinDataType,  # (2)
    PrimaryAccountNumber: str,
    PinDataLength: NotRequired[int],
```

1. See [:material-code-braces: PinGenerationAttributesTypeDef](./type_defs.md#pingenerationattributestypedef) 
2. See [:material-code-brackets: PinBlockFormatForPinDataType](./literals.md#pinblockformatforpindatatype) 
## VerifyPinDataInputRequestTypeDef

```python
# VerifyPinDataInputRequestTypeDef definition

class VerifyPinDataInputRequestTypeDef(TypedDict):
    EncryptedPinBlock: str,
    EncryptionKeyIdentifier: str,
    PinBlockFormat: PinBlockFormatForPinDataType,  # (1)
    PrimaryAccountNumber: str,
    VerificationAttributes: PinVerificationAttributesTypeDef,  # (2)
    VerificationKeyIdentifier: str,
    DukptAttributes: NotRequired[DukptAttributesTypeDef],  # (3)
    PinDataLength: NotRequired[int],
```

1. See [:material-code-brackets: PinBlockFormatForPinDataType](./literals.md#pinblockformatforpindatatype) 
2. See [:material-code-braces: PinVerificationAttributesTypeDef](./type_defs.md#pinverificationattributestypedef) 
3. See [:material-code-braces: DukptAttributesTypeDef](./type_defs.md#dukptattributestypedef) 
## VerifyAuthRequestCryptogramInputRequestTypeDef

```python
# VerifyAuthRequestCryptogramInputRequestTypeDef definition

class VerifyAuthRequestCryptogramInputRequestTypeDef(TypedDict):
    AuthRequestCryptogram: str,
    KeyIdentifier: str,
    MajorKeyDerivationMode: MajorKeyDerivationModeType,  # (1)
    SessionKeyDerivationAttributes: SessionKeyDerivationTypeDef,  # (2)
    TransactionData: str,
    AuthResponseAttributes: NotRequired[CryptogramAuthResponseTypeDef],  # (3)
```

1. See [:material-code-brackets: MajorKeyDerivationModeType](./literals.md#majorkeyderivationmodetype) 
2. See [:material-code-braces: SessionKeyDerivationTypeDef](./type_defs.md#sessionkeyderivationtypedef) 
3. See [:material-code-braces: CryptogramAuthResponseTypeDef](./type_defs.md#cryptogramauthresponsetypedef) 
## TranslatePinDataInputRequestTypeDef

```python
# TranslatePinDataInputRequestTypeDef definition

class TranslatePinDataInputRequestTypeDef(TypedDict):
    EncryptedPinBlock: str,
    IncomingKeyIdentifier: str,
    IncomingTranslationAttributes: TranslationIsoFormatsTypeDef,  # (1)
    OutgoingKeyIdentifier: str,
    OutgoingTranslationAttributes: TranslationIsoFormatsTypeDef,  # (1)
    IncomingDukptAttributes: NotRequired[DukptDerivationAttributesTypeDef],  # (3)
    OutgoingDukptAttributes: NotRequired[DukptDerivationAttributesTypeDef],  # (3)
```

1. See [:material-code-braces: TranslationIsoFormatsTypeDef](./type_defs.md#translationisoformatstypedef) 
2. See [:material-code-braces: TranslationIsoFormatsTypeDef](./type_defs.md#translationisoformatstypedef) 
3. See [:material-code-braces: DukptDerivationAttributesTypeDef](./type_defs.md#dukptderivationattributestypedef) 
4. See [:material-code-braces: DukptDerivationAttributesTypeDef](./type_defs.md#dukptderivationattributestypedef) 
## GenerateMacInputRequestTypeDef

```python
# GenerateMacInputRequestTypeDef definition

class GenerateMacInputRequestTypeDef(TypedDict):
    GenerationAttributes: MacAttributesTypeDef,  # (1)
    KeyIdentifier: str,
    MessageData: str,
    MacLength: NotRequired[int],
```

1. See [:material-code-braces: MacAttributesTypeDef](./type_defs.md#macattributestypedef) 
## VerifyMacInputRequestTypeDef

```python
# VerifyMacInputRequestTypeDef definition

class VerifyMacInputRequestTypeDef(TypedDict):
    KeyIdentifier: str,
    Mac: str,
    MessageData: str,
    VerificationAttributes: MacAttributesTypeDef,  # (1)
    MacLength: NotRequired[int],
```

1. See [:material-code-braces: MacAttributesTypeDef](./type_defs.md#macattributestypedef) 
