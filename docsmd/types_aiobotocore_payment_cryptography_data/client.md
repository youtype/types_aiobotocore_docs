# PaymentCryptographyDataPlaneClient

> [Index](../README.md) > [PaymentCryptographyDataPlane](./README.md) > PaymentCryptographyDataPlaneClient

!!! note ""

    Auto-generated documentation for [PaymentCryptographyDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
    type annotations stubs module [types-aiobotocore-payment-cryptography-data](https://pypi.org/project/types-aiobotocore-payment-cryptography-data/).

## PaymentCryptographyDataPlaneClient

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client)

```python
PaymentCryptographyDataPlaneClient usage example

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
PaymentCryptographyDataPlaneClient.exceptions usage example

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
PaymentCryptographyDataPlaneClient usage type checking example

from types_aiobotocore_payment_cryptography_data.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### decrypt\_data

Decrypts ciphertext data to plaintext using symmetric, asymmetric, or DUKPT data
encryption key.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").decrypt_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.decrypt_data)

```python
# decrypt_data method definition

await def decrypt_data(
    self,
    *,
    CipherText: str,
    DecryptionAttributes: EncryptionDecryptionAttributesTypeDef,  # (1)
    KeyIdentifier: str,
) -> DecryptDataOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EncryptionDecryptionAttributesTypeDef](./type_defs.md#encryptiondecryptionattributestypedef) 
2. See [:material-code-braces: DecryptDataOutputTypeDef](./type_defs.md#decryptdataoutputtypedef) 


```python
# decrypt_data method usage example with argument unpacking

kwargs: DecryptDataInputRequestTypeDef = {  # (1)
    "CipherText": ...,
    "DecryptionAttributes": ...,
    "KeyIdentifier": ...,
}

parent.decrypt_data(**kwargs)
```

1. See [:material-code-braces: DecryptDataInputRequestTypeDef](./type_defs.md#decryptdatainputrequesttypedef) 

### encrypt\_data

Encrypts plaintext data to ciphertext using symmetric, asymmetric, or DUKPT data
encryption key.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").encrypt_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.encrypt_data)

```python
# encrypt_data method definition

await def encrypt_data(
    self,
    *,
    EncryptionAttributes: EncryptionDecryptionAttributesTypeDef,  # (1)
    KeyIdentifier: str,
    PlainText: str,
) -> EncryptDataOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EncryptionDecryptionAttributesTypeDef](./type_defs.md#encryptiondecryptionattributestypedef) 
2. See [:material-code-braces: EncryptDataOutputTypeDef](./type_defs.md#encryptdataoutputtypedef) 


```python
# encrypt_data method usage example with argument unpacking

kwargs: EncryptDataInputRequestTypeDef = {  # (1)
    "EncryptionAttributes": ...,
    "KeyIdentifier": ...,
    "PlainText": ...,
}

parent.encrypt_data(**kwargs)
```

1. See [:material-code-braces: EncryptDataInputRequestTypeDef](./type_defs.md#encryptdatainputrequesttypedef) 

### generate\_card\_validation\_data

Generates card-related validation data using algorithms such as Card
Verification Values (CVV/CVV2), Dynamic Card Verification Values (dCVV/dCVV2),
or Card Security Codes (CSC).

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").generate_card_validation_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.generate_card_validation_data)

```python
# generate_card_validation_data method definition

await def generate_card_validation_data(
    self,
    *,
    GenerationAttributes: CardGenerationAttributesTypeDef,  # (1)
    KeyIdentifier: str,
    PrimaryAccountNumber: str,
    ValidationDataLength: int = ...,
) -> GenerateCardValidationDataOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CardGenerationAttributesTypeDef](./type_defs.md#cardgenerationattributestypedef) 
2. See [:material-code-braces: GenerateCardValidationDataOutputTypeDef](./type_defs.md#generatecardvalidationdataoutputtypedef) 


```python
# generate_card_validation_data method usage example with argument unpacking

kwargs: GenerateCardValidationDataInputRequestTypeDef = {  # (1)
    "GenerationAttributes": ...,
    "KeyIdentifier": ...,
    "PrimaryAccountNumber": ...,
}

parent.generate_card_validation_data(**kwargs)
```

1. See [:material-code-braces: GenerateCardValidationDataInputRequestTypeDef](./type_defs.md#generatecardvalidationdatainputrequesttypedef) 

### generate\_mac

Generates a Message Authentication Code (MAC) cryptogram within Amazon Web
Services Payment Cryptography.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").generate_mac` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.generate_mac)

```python
# generate_mac method definition

await def generate_mac(
    self,
    *,
    GenerationAttributes: MacAttributesTypeDef,  # (1)
    KeyIdentifier: str,
    MessageData: str,
    MacLength: int = ...,
) -> GenerateMacOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MacAttributesTypeDef](./type_defs.md#macattributestypedef) 
2. See [:material-code-braces: GenerateMacOutputTypeDef](./type_defs.md#generatemacoutputtypedef) 


```python
# generate_mac method usage example with argument unpacking

kwargs: GenerateMacInputRequestTypeDef = {  # (1)
    "GenerationAttributes": ...,
    "KeyIdentifier": ...,
    "MessageData": ...,
}

parent.generate_mac(**kwargs)
```

1. See [:material-code-braces: GenerateMacInputRequestTypeDef](./type_defs.md#generatemacinputrequesttypedef) 

### generate\_pin\_data

Generates pin-related data such as PIN, PIN Verification Value (PVV), PIN Block,
and PIN Offset during new card issuance or reissuance.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").generate_pin_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.generate_pin_data)

```python
# generate_pin_data method definition

await def generate_pin_data(
    self,
    *,
    EncryptionKeyIdentifier: str,
    GenerationAttributes: PinGenerationAttributesTypeDef,  # (1)
    GenerationKeyIdentifier: str,
    PinBlockFormat: PinBlockFormatForPinDataType,  # (2)
    PrimaryAccountNumber: str,
    PinDataLength: int = ...,
) -> GeneratePinDataOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: PinGenerationAttributesTypeDef](./type_defs.md#pingenerationattributestypedef) 
2. See [:material-code-brackets: PinBlockFormatForPinDataType](./literals.md#pinblockformatforpindatatype) 
3. See [:material-code-braces: GeneratePinDataOutputTypeDef](./type_defs.md#generatepindataoutputtypedef) 


```python
# generate_pin_data method usage example with argument unpacking

kwargs: GeneratePinDataInputRequestTypeDef = {  # (1)
    "EncryptionKeyIdentifier": ...,
    "GenerationAttributes": ...,
    "GenerationKeyIdentifier": ...,
    "PinBlockFormat": ...,
    "PrimaryAccountNumber": ...,
}

parent.generate_pin_data(**kwargs)
```

1. See [:material-code-braces: GeneratePinDataInputRequestTypeDef](./type_defs.md#generatepindatainputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.generate_presigned_url)

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


### re\_encrypt\_data

Re-encrypt ciphertext using DUKPT, Symmetric and Asymmetric Data Encryption
Keys.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").re_encrypt_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.re_encrypt_data)

```python
# re_encrypt_data method definition

await def re_encrypt_data(
    self,
    *,
    CipherText: str,
    IncomingEncryptionAttributes: ReEncryptionAttributesTypeDef,  # (1)
    IncomingKeyIdentifier: str,
    OutgoingEncryptionAttributes: ReEncryptionAttributesTypeDef,  # (1)
    OutgoingKeyIdentifier: str,
) -> ReEncryptDataOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ReEncryptionAttributesTypeDef](./type_defs.md#reencryptionattributestypedef) 
2. See [:material-code-braces: ReEncryptionAttributesTypeDef](./type_defs.md#reencryptionattributestypedef) 
3. See [:material-code-braces: ReEncryptDataOutputTypeDef](./type_defs.md#reencryptdataoutputtypedef) 


```python
# re_encrypt_data method usage example with argument unpacking

kwargs: ReEncryptDataInputRequestTypeDef = {  # (1)
    "CipherText": ...,
    "IncomingEncryptionAttributes": ...,
    "IncomingKeyIdentifier": ...,
    "OutgoingEncryptionAttributes": ...,
    "OutgoingKeyIdentifier": ...,
}

parent.re_encrypt_data(**kwargs)
```

1. See [:material-code-braces: ReEncryptDataInputRequestTypeDef](./type_defs.md#reencryptdatainputrequesttypedef) 

### translate\_pin\_data

Translates encrypted PIN block from and to ISO 9564 formats 0,1,3,4.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").translate_pin_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.translate_pin_data)

```python
# translate_pin_data method definition

await def translate_pin_data(
    self,
    *,
    EncryptedPinBlock: str,
    IncomingKeyIdentifier: str,
    IncomingTranslationAttributes: TranslationIsoFormatsTypeDef,  # (1)
    OutgoingKeyIdentifier: str,
    OutgoingTranslationAttributes: TranslationIsoFormatsTypeDef,  # (1)
    IncomingDukptAttributes: DukptDerivationAttributesTypeDef = ...,  # (3)
    OutgoingDukptAttributes: DukptDerivationAttributesTypeDef = ...,  # (3)
) -> TranslatePinDataOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: TranslationIsoFormatsTypeDef](./type_defs.md#translationisoformatstypedef) 
2. See [:material-code-braces: TranslationIsoFormatsTypeDef](./type_defs.md#translationisoformatstypedef) 
3. See [:material-code-braces: DukptDerivationAttributesTypeDef](./type_defs.md#dukptderivationattributestypedef) 
4. See [:material-code-braces: DukptDerivationAttributesTypeDef](./type_defs.md#dukptderivationattributestypedef) 
5. See [:material-code-braces: TranslatePinDataOutputTypeDef](./type_defs.md#translatepindataoutputtypedef) 


```python
# translate_pin_data method usage example with argument unpacking

kwargs: TranslatePinDataInputRequestTypeDef = {  # (1)
    "EncryptedPinBlock": ...,
    "IncomingKeyIdentifier": ...,
    "IncomingTranslationAttributes": ...,
    "OutgoingKeyIdentifier": ...,
    "OutgoingTranslationAttributes": ...,
}

parent.translate_pin_data(**kwargs)
```

1. See [:material-code-braces: TranslatePinDataInputRequestTypeDef](./type_defs.md#translatepindatainputrequesttypedef) 

### verify\_auth\_request\_cryptogram

Verifies Authorization Request Cryptogram (ARQC) for a EMV chip payment card
authorization.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").verify_auth_request_cryptogram` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.verify_auth_request_cryptogram)

```python
# verify_auth_request_cryptogram method definition

await def verify_auth_request_cryptogram(
    self,
    *,
    AuthRequestCryptogram: str,
    KeyIdentifier: str,
    MajorKeyDerivationMode: MajorKeyDerivationModeType,  # (1)
    SessionKeyDerivationAttributes: SessionKeyDerivationTypeDef,  # (2)
    TransactionData: str,
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

kwargs: VerifyAuthRequestCryptogramInputRequestTypeDef = {  # (1)
    "AuthRequestCryptogram": ...,
    "KeyIdentifier": ...,
    "MajorKeyDerivationMode": ...,
    "SessionKeyDerivationAttributes": ...,
    "TransactionData": ...,
}

parent.verify_auth_request_cryptogram(**kwargs)
```

1. See [:material-code-braces: VerifyAuthRequestCryptogramInputRequestTypeDef](./type_defs.md#verifyauthrequestcryptograminputrequesttypedef) 

### verify\_card\_validation\_data

Verifies card-related validation data using algorithms such as Card Verification
Values (CVV/CVV2), Dynamic Card Verification Values (dCVV/dCVV2) and Card
Security Codes (CSC).

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").verify_card_validation_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.verify_card_validation_data)

```python
# verify_card_validation_data method definition

await def verify_card_validation_data(
    self,
    *,
    KeyIdentifier: str,
    PrimaryAccountNumber: str,
    ValidationData: str,
    VerificationAttributes: CardVerificationAttributesTypeDef,  # (1)
) -> VerifyCardValidationDataOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CardVerificationAttributesTypeDef](./type_defs.md#cardverificationattributestypedef) 
2. See [:material-code-braces: VerifyCardValidationDataOutputTypeDef](./type_defs.md#verifycardvalidationdataoutputtypedef) 


```python
# verify_card_validation_data method usage example with argument unpacking

kwargs: VerifyCardValidationDataInputRequestTypeDef = {  # (1)
    "KeyIdentifier": ...,
    "PrimaryAccountNumber": ...,
    "ValidationData": ...,
    "VerificationAttributes": ...,
}

parent.verify_card_validation_data(**kwargs)
```

1. See [:material-code-braces: VerifyCardValidationDataInputRequestTypeDef](./type_defs.md#verifycardvalidationdatainputrequesttypedef) 

### verify\_mac

Verifies a Message Authentication Code (MAC).

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").verify_mac` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.verify_mac)

```python
# verify_mac method definition

await def verify_mac(
    self,
    *,
    KeyIdentifier: str,
    Mac: str,
    MessageData: str,
    VerificationAttributes: MacAttributesTypeDef,  # (1)
    MacLength: int = ...,
) -> VerifyMacOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MacAttributesTypeDef](./type_defs.md#macattributestypedef) 
2. See [:material-code-braces: VerifyMacOutputTypeDef](./type_defs.md#verifymacoutputtypedef) 


```python
# verify_mac method usage example with argument unpacking

kwargs: VerifyMacInputRequestTypeDef = {  # (1)
    "KeyIdentifier": ...,
    "Mac": ...,
    "MessageData": ...,
    "VerificationAttributes": ...,
}

parent.verify_mac(**kwargs)
```

1. See [:material-code-braces: VerifyMacInputRequestTypeDef](./type_defs.md#verifymacinputrequesttypedef) 

### verify\_pin\_data

Verifies pin-related data such as PIN and PIN Offset using algorithms including
VISA PVV and IBM3624.

Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").verify_pin_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.verify_pin_data)

```python
# verify_pin_data method definition

await def verify_pin_data(
    self,
    *,
    EncryptedPinBlock: str,
    EncryptionKeyIdentifier: str,
    PinBlockFormat: PinBlockFormatForPinDataType,  # (1)
    PrimaryAccountNumber: str,
    VerificationAttributes: PinVerificationAttributesTypeDef,  # (2)
    VerificationKeyIdentifier: str,
    DukptAttributes: DukptAttributesTypeDef = ...,  # (3)
    PinDataLength: int = ...,
) -> VerifyPinDataOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: PinBlockFormatForPinDataType](./literals.md#pinblockformatforpindatatype) 
2. See [:material-code-braces: PinVerificationAttributesTypeDef](./type_defs.md#pinverificationattributestypedef) 
3. See [:material-code-braces: DukptAttributesTypeDef](./type_defs.md#dukptattributestypedef) 
4. See [:material-code-braces: VerifyPinDataOutputTypeDef](./type_defs.md#verifypindataoutputtypedef) 


```python
# verify_pin_data method usage example with argument unpacking

kwargs: VerifyPinDataInputRequestTypeDef = {  # (1)
    "EncryptedPinBlock": ...,
    "EncryptionKeyIdentifier": ...,
    "PinBlockFormat": ...,
    "PrimaryAccountNumber": ...,
    "VerificationAttributes": ...,
    "VerificationKeyIdentifier": ...,
}

parent.verify_pin_data(**kwargs)
```

1. See [:material-code-braces: VerifyPinDataInputRequestTypeDef](./type_defs.md#verifypindatainputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> PaymentCryptographyDataPlaneClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("payment-cryptography-data").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





