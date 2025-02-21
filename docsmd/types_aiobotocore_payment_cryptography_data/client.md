# PaymentCryptographyDataPlaneClient

> [Index](../README.md) > [PaymentCryptographyDataPlane](./README.md) > PaymentCryptographyDataPlaneClient

!!! note ""

    Auto-generated documentation for [PaymentCryptographyDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#paymentcryptographydataplane)
    type annotations stubs module [types-aiobotocore-payment-cryptography-data](https://pypi.org/project/types-aiobotocore-payment-cryptography-data/).

## PaymentCryptographyDataPlaneClient

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client)

```python
# PaymentCryptographyDataPlaneClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_payment_cryptography_data.client import PaymentCryptographyDataPlaneClient

session = get_session()
async with session.create_client("payment-cryptography-data") as client:
    client: PaymentCryptographyDataPlaneClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("payment-cryptography-data").exceptions` structure.

```python
# PaymentCryptographyDataPlaneClient.exceptions usage example

async with session.create_client("payment-cryptography-data") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.ValidationException,
        client.VerificationFailedException,
    ) as e:
        print(e)
```

```python
# PaymentCryptographyDataPlaneClient usage type checking example

from types_aiobotocore_payment_cryptography_data.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### decrypt\_data

Decrypts ciphertext data to plaintext using a symmetric (TDES, AES), asymmetric
(RSA), or derived (DUKPT or EMV) encryption key scheme.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").decrypt_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/decrypt_data.html)

```python
# decrypt_data method definition

await def decrypt_data(
    self,
    *,
    KeyIdentifier: str,
    CipherText: str,
    DecryptionAttributes: EncryptionDecryptionAttributesTypeDef,  # (1)
    WrappedKey: WrappedKeyTypeDef = ...,  # (2)
) -> DecryptDataOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EncryptionDecryptionAttributesTypeDef](./type_defs.md#encryptiondecryptionattributestypedef) 
2. See [:material-code-braces: WrappedKeyTypeDef](./type_defs.md#wrappedkeytypedef) 
3. See [:material-code-braces: DecryptDataOutputTypeDef](./type_defs.md#decryptdataoutputtypedef) 


```python
# decrypt_data method usage example with argument unpacking

kwargs: DecryptDataInputTypeDef = {  # (1)
    "KeyIdentifier": ...,
    "CipherText": ...,
    "DecryptionAttributes": ...,
}

parent.decrypt_data(**kwargs)
```

1. See [:material-code-braces: DecryptDataInputTypeDef](./type_defs.md#decryptdatainputtypedef) 

### encrypt\_data

Encrypts plaintext data to ciphertext using a symmetric (TDES, AES), asymmetric
(RSA), or derived (DUKPT or EMV) encryption key scheme.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").encrypt_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/encrypt_data.html)

```python
# encrypt_data method definition

await def encrypt_data(
    self,
    *,
    KeyIdentifier: str,
    PlainText: str,
    EncryptionAttributes: EncryptionDecryptionAttributesTypeDef,  # (1)
    WrappedKey: WrappedKeyTypeDef = ...,  # (2)
) -> EncryptDataOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EncryptionDecryptionAttributesTypeDef](./type_defs.md#encryptiondecryptionattributestypedef) 
2. See [:material-code-braces: WrappedKeyTypeDef](./type_defs.md#wrappedkeytypedef) 
3. See [:material-code-braces: EncryptDataOutputTypeDef](./type_defs.md#encryptdataoutputtypedef) 


```python
# encrypt_data method usage example with argument unpacking

kwargs: EncryptDataInputTypeDef = {  # (1)
    "KeyIdentifier": ...,
    "PlainText": ...,
    "EncryptionAttributes": ...,
}

parent.encrypt_data(**kwargs)
```

1. See [:material-code-braces: EncryptDataInputTypeDef](./type_defs.md#encryptdatainputtypedef) 

### generate\_card\_validation\_data

Generates card-related validation data using algorithms such as Card
Verification Values (CVV/CVV2), Dynamic Card Verification Values (dCVV/dCVV2),
or Card Security Codes (CSC).

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").generate_card_validation_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/generate_card_validation_data.html)

```python
# generate_card_validation_data method definition

await def generate_card_validation_data(
    self,
    *,
    KeyIdentifier: str,
    PrimaryAccountNumber: str,
    GenerationAttributes: CardGenerationAttributesTypeDef,  # (1)
    ValidationDataLength: int = ...,
) -> GenerateCardValidationDataOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CardGenerationAttributesTypeDef](./type_defs.md#cardgenerationattributestypedef) 
2. See [:material-code-braces: GenerateCardValidationDataOutputTypeDef](./type_defs.md#generatecardvalidationdataoutputtypedef) 


```python
# generate_card_validation_data method usage example with argument unpacking

kwargs: GenerateCardValidationDataInputTypeDef = {  # (1)
    "KeyIdentifier": ...,
    "PrimaryAccountNumber": ...,
    "GenerationAttributes": ...,
}

parent.generate_card_validation_data(**kwargs)
```

1. See [:material-code-braces: GenerateCardValidationDataInputTypeDef](./type_defs.md#generatecardvalidationdatainputtypedef) 

### generate\_mac

Generates a Message Authentication Code (MAC) cryptogram within Amazon Web
Services Payment Cryptography.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").generate_mac` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/generate_mac.html)

```python
# generate_mac method definition

await def generate_mac(
    self,
    *,
    KeyIdentifier: str,
    MessageData: str,
    GenerationAttributes: MacAttributesTypeDef,  # (1)
    MacLength: int = ...,
) -> GenerateMacOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MacAttributesTypeDef](./type_defs.md#macattributestypedef) 
2. See [:material-code-braces: GenerateMacOutputTypeDef](./type_defs.md#generatemacoutputtypedef) 


```python
# generate_mac method usage example with argument unpacking

kwargs: GenerateMacInputTypeDef = {  # (1)
    "KeyIdentifier": ...,
    "MessageData": ...,
    "GenerationAttributes": ...,
}

parent.generate_mac(**kwargs)
```

1. See [:material-code-braces: GenerateMacInputTypeDef](./type_defs.md#generatemacinputtypedef) 

### generate\_mac\_emv\_pin\_change

Generates an issuer script mac for EMV payment cards that use offline PINs as
the cardholder verification method (CVM).

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").generate_mac_emv_pin_change` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/generate_mac_emv_pin_change.html)

```python
# generate_mac_emv_pin_change method definition

await def generate_mac_emv_pin_change(
    self,
    *,
    NewPinPekIdentifier: str,
    NewEncryptedPinBlock: str,
    PinBlockFormat: PinBlockFormatForEmvPinChangeType,  # (1)
    SecureMessagingIntegrityKeyIdentifier: str,
    SecureMessagingConfidentialityKeyIdentifier: str,
    MessageData: str,
    DerivationMethodAttributes: DerivationMethodAttributesTypeDef,  # (2)
) -> GenerateMacEmvPinChangeOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PinBlockFormatForEmvPinChangeType](./literals.md#pinblockformatforemvpinchangetype) 
2. See [:material-code-braces: DerivationMethodAttributesTypeDef](./type_defs.md#derivationmethodattributestypedef) 
3. See [:material-code-braces: GenerateMacEmvPinChangeOutputTypeDef](./type_defs.md#generatemacemvpinchangeoutputtypedef) 


```python
# generate_mac_emv_pin_change method usage example with argument unpacking

kwargs: GenerateMacEmvPinChangeInputTypeDef = {  # (1)
    "NewPinPekIdentifier": ...,
    "NewEncryptedPinBlock": ...,
    "PinBlockFormat": ...,
    "SecureMessagingIntegrityKeyIdentifier": ...,
    "SecureMessagingConfidentialityKeyIdentifier": ...,
    "MessageData": ...,
    "DerivationMethodAttributes": ...,
}

parent.generate_mac_emv_pin_change(**kwargs)
```

1. See [:material-code-braces: GenerateMacEmvPinChangeInputTypeDef](./type_defs.md#generatemacemvpinchangeinputtypedef) 

### generate\_pin\_data

Generates pin-related data such as PIN, PIN Verification Value (PVV), PIN
Block, and PIN Offset during new card issuance or reissuance.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").generate_pin_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/generate_pin_data.html)

```python
# generate_pin_data method definition

await def generate_pin_data(
    self,
    *,
    GenerationKeyIdentifier: str,
    EncryptionKeyIdentifier: str,
    GenerationAttributes: PinGenerationAttributesTypeDef,  # (1)
    PrimaryAccountNumber: str,
    PinBlockFormat: PinBlockFormatForPinDataType,  # (2)
    PinDataLength: int = ...,
    EncryptionWrappedKey: WrappedKeyTypeDef = ...,  # (3)
) -> GeneratePinDataOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: PinGenerationAttributesTypeDef](./type_defs.md#pingenerationattributestypedef) 
2. See [:material-code-brackets: PinBlockFormatForPinDataType](./literals.md#pinblockformatforpindatatype) 
3. See [:material-code-braces: WrappedKeyTypeDef](./type_defs.md#wrappedkeytypedef) 
4. See [:material-code-braces: GeneratePinDataOutputTypeDef](./type_defs.md#generatepindataoutputtypedef) 


```python
# generate_pin_data method usage example with argument unpacking

kwargs: GeneratePinDataInputTypeDef = {  # (1)
    "GenerationKeyIdentifier": ...,
    "EncryptionKeyIdentifier": ...,
    "GenerationAttributes": ...,
    "PrimaryAccountNumber": ...,
    "PinBlockFormat": ...,
}

parent.generate_pin_data(**kwargs)
```

1. See [:material-code-braces: GeneratePinDataInputTypeDef](./type_defs.md#generatepindatainputtypedef) 

### re\_encrypt\_data

Re-encrypt ciphertext using DUKPT or Symmetric data encryption keys.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").re_encrypt_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/re_encrypt_data.html)

```python
# re_encrypt_data method definition

await def re_encrypt_data(
    self,
    *,
    IncomingKeyIdentifier: str,
    OutgoingKeyIdentifier: str,
    CipherText: str,
    IncomingEncryptionAttributes: ReEncryptionAttributesTypeDef,  # (1)
    OutgoingEncryptionAttributes: ReEncryptionAttributesTypeDef,  # (1)
    IncomingWrappedKey: WrappedKeyTypeDef = ...,  # (3)
    OutgoingWrappedKey: WrappedKeyTypeDef = ...,  # (3)
) -> ReEncryptDataOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ReEncryptionAttributesTypeDef](./type_defs.md#reencryptionattributestypedef) 
2. See [:material-code-braces: ReEncryptionAttributesTypeDef](./type_defs.md#reencryptionattributestypedef) 
3. See [:material-code-braces: WrappedKeyTypeDef](./type_defs.md#wrappedkeytypedef) 
4. See [:material-code-braces: WrappedKeyTypeDef](./type_defs.md#wrappedkeytypedef) 
5. See [:material-code-braces: ReEncryptDataOutputTypeDef](./type_defs.md#reencryptdataoutputtypedef) 


```python
# re_encrypt_data method usage example with argument unpacking

kwargs: ReEncryptDataInputTypeDef = {  # (1)
    "IncomingKeyIdentifier": ...,
    "OutgoingKeyIdentifier": ...,
    "CipherText": ...,
    "IncomingEncryptionAttributes": ...,
    "OutgoingEncryptionAttributes": ...,
}

parent.re_encrypt_data(**kwargs)
```

1. See [:material-code-braces: ReEncryptDataInputTypeDef](./type_defs.md#reencryptdatainputtypedef) 

### translate\_pin\_data

Translates encrypted PIN block from and to ISO 9564 formats 0,1,3,4.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").translate_pin_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/translate_pin_data.html)

```python
# translate_pin_data method definition

await def translate_pin_data(
    self,
    *,
    IncomingKeyIdentifier: str,
    OutgoingKeyIdentifier: str,
    IncomingTranslationAttributes: TranslationIsoFormatsTypeDef,  # (1)
    OutgoingTranslationAttributes: TranslationIsoFormatsTypeDef,  # (1)
    EncryptedPinBlock: str,
    IncomingDukptAttributes: DukptDerivationAttributesTypeDef = ...,  # (3)
    OutgoingDukptAttributes: DukptDerivationAttributesTypeDef = ...,  # (3)
    IncomingWrappedKey: WrappedKeyTypeDef = ...,  # (5)
    OutgoingWrappedKey: WrappedKeyTypeDef = ...,  # (5)
) -> TranslatePinDataOutputTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: TranslationIsoFormatsTypeDef](./type_defs.md#translationisoformatstypedef) 
2. See [:material-code-braces: TranslationIsoFormatsTypeDef](./type_defs.md#translationisoformatstypedef) 
3. See [:material-code-braces: DukptDerivationAttributesTypeDef](./type_defs.md#dukptderivationattributestypedef) 
4. See [:material-code-braces: DukptDerivationAttributesTypeDef](./type_defs.md#dukptderivationattributestypedef) 
5. See [:material-code-braces: WrappedKeyTypeDef](./type_defs.md#wrappedkeytypedef) 
6. See [:material-code-braces: WrappedKeyTypeDef](./type_defs.md#wrappedkeytypedef) 
7. See [:material-code-braces: TranslatePinDataOutputTypeDef](./type_defs.md#translatepindataoutputtypedef) 


```python
# translate_pin_data method usage example with argument unpacking

kwargs: TranslatePinDataInputTypeDef = {  # (1)
    "IncomingKeyIdentifier": ...,
    "OutgoingKeyIdentifier": ...,
    "IncomingTranslationAttributes": ...,
    "OutgoingTranslationAttributes": ...,
    "EncryptedPinBlock": ...,
}

parent.translate_pin_data(**kwargs)
```

1. See [:material-code-braces: TranslatePinDataInputTypeDef](./type_defs.md#translatepindatainputtypedef) 

### verify\_auth\_request\_cryptogram

Verifies Authorization Request Cryptogram (ARQC) for a EMV chip payment card
authorization.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").verify_auth_request_cryptogram` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/verify_auth_request_cryptogram.html)

```python
# verify_auth_request_cryptogram method definition

await def verify_auth_request_cryptogram(
    self,
    *,
    KeyIdentifier: str,
    TransactionData: str,
    AuthRequestCryptogram: str,
    MajorKeyDerivationMode: MajorKeyDerivationModeType,  # (1)
    SessionKeyDerivationAttributes: SessionKeyDerivationTypeDef,  # (2)
    AuthResponseAttributes: CryptogramAuthResponseTypeDef = ...,  # (3)
) -> VerifyAuthRequestCryptogramOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: MajorKeyDerivationModeType](./literals.md#majorkeyderivationmodetype) 
2. See [:material-code-braces: SessionKeyDerivationTypeDef](./type_defs.md#sessionkeyderivationtypedef) 
3. See [:material-code-braces: CryptogramAuthResponseTypeDef](./type_defs.md#cryptogramauthresponsetypedef) 
4. See [:material-code-braces: VerifyAuthRequestCryptogramOutputTypeDef](./type_defs.md#verifyauthrequestcryptogramoutputtypedef) 


```python
# verify_auth_request_cryptogram method usage example with argument unpacking

kwargs: VerifyAuthRequestCryptogramInputTypeDef = {  # (1)
    "KeyIdentifier": ...,
    "TransactionData": ...,
    "AuthRequestCryptogram": ...,
    "MajorKeyDerivationMode": ...,
    "SessionKeyDerivationAttributes": ...,
}

parent.verify_auth_request_cryptogram(**kwargs)
```

1. See [:material-code-braces: VerifyAuthRequestCryptogramInputTypeDef](./type_defs.md#verifyauthrequestcryptograminputtypedef) 

### verify\_card\_validation\_data

Verifies card-related validation data using algorithms such as Card
Verification Values (CVV/CVV2), Dynamic Card Verification Values (dCVV/dCVV2)
and Card Security Codes (CSC).

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").verify_card_validation_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/verify_card_validation_data.html)

```python
# verify_card_validation_data method definition

await def verify_card_validation_data(
    self,
    *,
    KeyIdentifier: str,
    PrimaryAccountNumber: str,
    VerificationAttributes: CardVerificationAttributesTypeDef,  # (1)
    ValidationData: str,
) -> VerifyCardValidationDataOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CardVerificationAttributesTypeDef](./type_defs.md#cardverificationattributestypedef) 
2. See [:material-code-braces: VerifyCardValidationDataOutputTypeDef](./type_defs.md#verifycardvalidationdataoutputtypedef) 


```python
# verify_card_validation_data method usage example with argument unpacking

kwargs: VerifyCardValidationDataInputTypeDef = {  # (1)
    "KeyIdentifier": ...,
    "PrimaryAccountNumber": ...,
    "VerificationAttributes": ...,
    "ValidationData": ...,
}

parent.verify_card_validation_data(**kwargs)
```

1. See [:material-code-braces: VerifyCardValidationDataInputTypeDef](./type_defs.md#verifycardvalidationdatainputtypedef) 

### verify\_mac

Verifies a Message Authentication Code (MAC).

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").verify_mac` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/verify_mac.html)

```python
# verify_mac method definition

await def verify_mac(
    self,
    *,
    KeyIdentifier: str,
    MessageData: str,
    Mac: str,
    VerificationAttributes: MacAttributesTypeDef,  # (1)
    MacLength: int = ...,
) -> VerifyMacOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MacAttributesTypeDef](./type_defs.md#macattributestypedef) 
2. See [:material-code-braces: VerifyMacOutputTypeDef](./type_defs.md#verifymacoutputtypedef) 


```python
# verify_mac method usage example with argument unpacking

kwargs: VerifyMacInputTypeDef = {  # (1)
    "KeyIdentifier": ...,
    "MessageData": ...,
    "Mac": ...,
    "VerificationAttributes": ...,
}

parent.verify_mac(**kwargs)
```

1. See [:material-code-braces: VerifyMacInputTypeDef](./type_defs.md#verifymacinputtypedef) 

### verify\_pin\_data

Verifies pin-related data such as PIN and PIN Offset using algorithms including
VISA PVV and IBM3624.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").verify_pin_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data/client/verify_pin_data.html)

```python
# verify_pin_data method definition

await def verify_pin_data(
    self,
    *,
    VerificationKeyIdentifier: str,
    EncryptionKeyIdentifier: str,
    VerificationAttributes: PinVerificationAttributesTypeDef,  # (1)
    EncryptedPinBlock: str,
    PrimaryAccountNumber: str,
    PinBlockFormat: PinBlockFormatForPinDataType,  # (2)
    PinDataLength: int = ...,
    DukptAttributes: DukptAttributesTypeDef = ...,  # (3)
    EncryptionWrappedKey: WrappedKeyTypeDef = ...,  # (4)
) -> VerifyPinDataOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: PinVerificationAttributesTypeDef](./type_defs.md#pinverificationattributestypedef) 
2. See [:material-code-brackets: PinBlockFormatForPinDataType](./literals.md#pinblockformatforpindatatype) 
3. See [:material-code-braces: DukptAttributesTypeDef](./type_defs.md#dukptattributestypedef) 
4. See [:material-code-braces: WrappedKeyTypeDef](./type_defs.md#wrappedkeytypedef) 
5. See [:material-code-braces: VerifyPinDataOutputTypeDef](./type_defs.md#verifypindataoutputtypedef) 


```python
# verify_pin_data method usage example with argument unpacking

kwargs: VerifyPinDataInputTypeDef = {  # (1)
    "VerificationKeyIdentifier": ...,
    "EncryptionKeyIdentifier": ...,
    "VerificationAttributes": ...,
    "EncryptedPinBlock": ...,
    "PrimaryAccountNumber": ...,
    "PinBlockFormat": ...,
}

parent.verify_pin_data(**kwargs)
```

1. See [:material-code-braces: VerifyPinDataInputTypeDef](./type_defs.md#verifypindatainputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```





