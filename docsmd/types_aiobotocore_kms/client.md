# KMSClient

> [Index](../README.md) > [KMS](./README.md) > KMSClient

!!! note ""

    Auto-generated documentation for [KMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
    type annotations stubs module [types-aiobotocore-kms](https://pypi.org/project/types-aiobotocore-kms/).

## KMSClient

Type annotations and code completion for `#!python session.create_client("kms")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)

```python
# KMSClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_kms.client import KMSClient

session = get_session()
async with session.create_client("kms") as client:
    client: KMSClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("kms").exceptions` structure.

```python
# KMSClient.exceptions usage example

async with session.create_client("kms") as client:
    try:
        do_something(client)
    except (
            client.AlreadyExistsException,
        client.ClientError,
        client.CloudHsmClusterInUseException,
        client.CloudHsmClusterInvalidConfigurationException,
        client.CloudHsmClusterNotActiveException,
        client.CloudHsmClusterNotFoundException,
        client.CloudHsmClusterNotRelatedException,
        client.ConflictException,
        client.CustomKeyStoreHasCMKsException,
        client.CustomKeyStoreInvalidStateException,
        client.CustomKeyStoreNameInUseException,
        client.CustomKeyStoreNotFoundException,
        client.DependencyTimeoutException,
        client.DisabledException,
        client.DryRunOperationException,
        client.ExpiredImportTokenException,
        client.IncorrectKeyException,
        client.IncorrectKeyMaterialException,
        client.IncorrectTrustAnchorException,
        client.InvalidAliasNameException,
        client.InvalidArnException,
        client.InvalidCiphertextException,
        client.InvalidGrantIdException,
        client.InvalidGrantTokenException,
        client.InvalidImportTokenException,
        client.InvalidKeyUsageException,
        client.InvalidMarkerException,
        client.KMSInternalException,
        client.KMSInvalidMacException,
        client.KMSInvalidSignatureException,
        client.KMSInvalidStateException,
        client.KeyUnavailableException,
        client.LimitExceededException,
        client.MalformedPolicyDocumentException,
        client.NotFoundException,
        client.TagException,
        client.UnsupportedOperationException,
        client.XksKeyAlreadyInUseException,
        client.XksKeyInvalidConfigurationException,
        client.XksKeyNotFoundException,
        client.XksProxyIncorrectAuthenticationCredentialException,
        client.XksProxyInvalidConfigurationException,
        client.XksProxyInvalidResponseException,
        client.XksProxyUriEndpointInUseException,
        client.XksProxyUriInUseException,
        client.XksProxyUriUnreachableException,
        client.XksProxyVpcEndpointServiceInUseException,
        client.XksProxyVpcEndpointServiceInvalidConfigurationException,
        client.XksProxyVpcEndpointServiceNotFoundException,
    ) as e:
        print(e)
```

```python
# KMSClient usage type checking example

from types_aiobotocore_kms.client import Exceptions

def handle_error(exc: Exceptions.AlreadyExistsException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("kms").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_key\_deletion

Cancels the deletion of a KMS key.

Type annotations and code completion for `#!python session.create_client("kms").cancel_key_deletion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.cancel_key_deletion)

```python
# cancel_key_deletion method definition

await def cancel_key_deletion(
    self,
    *,
    KeyId: str,
) -> CancelKeyDeletionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelKeyDeletionResponseTypeDef](./type_defs.md#cancelkeydeletionresponsetypedef) 


```python
# cancel_key_deletion method usage example with argument unpacking

kwargs: CancelKeyDeletionRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.cancel_key_deletion(**kwargs)
```

1. See [:material-code-braces: CancelKeyDeletionRequestRequestTypeDef](./type_defs.md#cancelkeydeletionrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("kms").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### connect\_custom\_key\_store

Connects or reconnects a [custom key
store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-overview.html)
to its backing key
store.

Type annotations and code completion for `#!python session.create_client("kms").connect_custom_key_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.connect_custom_key_store)

```python
# connect_custom_key_store method definition

await def connect_custom_key_store(
    self,
    *,
    CustomKeyStoreId: str,
) -> Dict[str, Any]:
    ...
```



```python
# connect_custom_key_store method usage example with argument unpacking

kwargs: ConnectCustomKeyStoreRequestRequestTypeDef = {  # (1)
    "CustomKeyStoreId": ...,
}

parent.connect_custom_key_store(**kwargs)
```

1. See [:material-code-braces: ConnectCustomKeyStoreRequestRequestTypeDef](./type_defs.md#connectcustomkeystorerequestrequesttypedef) 

### create\_alias

Creates a friendly name for a KMS key.

Type annotations and code completion for `#!python session.create_client("kms").create_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_alias)

```python
# create_alias method definition

await def create_alias(
    self,
    *,
    AliasName: str,
    TargetKeyId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_alias method usage example with argument unpacking

kwargs: CreateAliasRequestRequestTypeDef = {  # (1)
    "AliasName": ...,
    "TargetKeyId": ...,
}

parent.create_alias(**kwargs)
```

1. See [:material-code-braces: CreateAliasRequestRequestTypeDef](./type_defs.md#createaliasrequestrequesttypedef) 

### create\_custom\_key\_store

Creates a [custom key
store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-overview.html)
backed by a key store that you own and
manage.

Type annotations and code completion for `#!python session.create_client("kms").create_custom_key_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_custom_key_store)

```python
# create_custom_key_store method definition

await def create_custom_key_store(
    self,
    *,
    CustomKeyStoreName: str,
    CloudHsmClusterId: str = ...,
    TrustAnchorCertificate: str = ...,
    KeyStorePassword: str = ...,
    CustomKeyStoreType: CustomKeyStoreTypeType = ...,  # (1)
    XksProxyUriEndpoint: str = ...,
    XksProxyUriPath: str = ...,
    XksProxyVpcEndpointServiceName: str = ...,
    XksProxyAuthenticationCredential: XksProxyAuthenticationCredentialTypeTypeDef = ...,  # (2)
    XksProxyConnectivity: XksProxyConnectivityTypeType = ...,  # (3)
) -> CreateCustomKeyStoreResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: CustomKeyStoreTypeType](./literals.md#customkeystoretypetype) 
2. See [:material-code-braces: XksProxyAuthenticationCredentialTypeTypeDef](./type_defs.md#xksproxyauthenticationcredentialtypetypedef) 
3. See [:material-code-brackets: XksProxyConnectivityTypeType](./literals.md#xksproxyconnectivitytypetype) 
4. See [:material-code-braces: CreateCustomKeyStoreResponseTypeDef](./type_defs.md#createcustomkeystoreresponsetypedef) 


```python
# create_custom_key_store method usage example with argument unpacking

kwargs: CreateCustomKeyStoreRequestRequestTypeDef = {  # (1)
    "CustomKeyStoreName": ...,
}

parent.create_custom_key_store(**kwargs)
```

1. See [:material-code-braces: CreateCustomKeyStoreRequestRequestTypeDef](./type_defs.md#createcustomkeystorerequestrequesttypedef) 

### create\_grant

Adds a grant to a KMS key.

Type annotations and code completion for `#!python session.create_client("kms").create_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_grant)

```python
# create_grant method definition

await def create_grant(
    self,
    *,
    KeyId: str,
    GranteePrincipal: str,
    Operations: Sequence[GrantOperationType],  # (1)
    RetiringPrincipal: str = ...,
    Constraints: GrantConstraintsTypeDef = ...,  # (2)
    GrantTokens: Sequence[str] = ...,
    Name: str = ...,
    DryRun: bool = ...,
) -> CreateGrantResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: GrantOperationType](./literals.md#grantoperationtype) 
2. See [:material-code-braces: GrantConstraintsTypeDef](./type_defs.md#grantconstraintstypedef) 
3. See [:material-code-braces: CreateGrantResponseTypeDef](./type_defs.md#creategrantresponsetypedef) 


```python
# create_grant method usage example with argument unpacking

kwargs: CreateGrantRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "GranteePrincipal": ...,
    "Operations": ...,
}

parent.create_grant(**kwargs)
```

1. See [:material-code-braces: CreateGrantRequestRequestTypeDef](./type_defs.md#creategrantrequestrequesttypedef) 

### create\_key

Creates a unique customer managed [KMS
key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#kms-keys)
in your Amazon Web Services account and
Region.

Type annotations and code completion for `#!python session.create_client("kms").create_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_key)

```python
# create_key method definition

await def create_key(
    self,
    *,
    Policy: str = ...,
    Description: str = ...,
    KeyUsage: KeyUsageTypeType = ...,  # (1)
    CustomerMasterKeySpec: CustomerMasterKeySpecType = ...,  # (2)
    KeySpec: KeySpecType = ...,  # (3)
    Origin: OriginTypeType = ...,  # (4)
    CustomKeyStoreId: str = ...,
    BypassPolicyLockoutSafetyCheck: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (5)
    MultiRegion: bool = ...,
    XksKeyId: str = ...,
) -> CreateKeyResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: KeyUsageTypeType](./literals.md#keyusagetypetype) 
2. See [:material-code-brackets: CustomerMasterKeySpecType](./literals.md#customermasterkeyspectype) 
3. See [:material-code-brackets: KeySpecType](./literals.md#keyspectype) 
4. See [:material-code-brackets: OriginTypeType](./literals.md#origintypetype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CreateKeyResponseTypeDef](./type_defs.md#createkeyresponsetypedef) 


```python
# create_key method usage example with argument unpacking

kwargs: CreateKeyRequestRequestTypeDef = {  # (1)
    "Policy": ...,
}

parent.create_key(**kwargs)
```

1. See [:material-code-braces: CreateKeyRequestRequestTypeDef](./type_defs.md#createkeyrequestrequesttypedef) 

### decrypt

Decrypts ciphertext that was encrypted by a KMS key using any of the following
operations: *  Encrypt *  GenerateDataKey *  GenerateDataKeyPair *
GenerateDataKeyWithoutPlaintext *  GenerateDataKeyPairWithoutPlaintext You can
use this operation to decrypt ciphertext that was
enc...

Type annotations and code completion for `#!python session.create_client("kms").decrypt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.decrypt)

```python
# decrypt method definition

await def decrypt(
    self,
    *,
    CiphertextBlob: BlobTypeDef,
    EncryptionContext: Mapping[str, str] = ...,
    GrantTokens: Sequence[str] = ...,
    KeyId: str = ...,
    EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,  # (1)
    Recipient: RecipientInfoTypeDef = ...,  # (2)
    DryRun: bool = ...,
) -> DecryptResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
2. See [:material-code-braces: RecipientInfoTypeDef](./type_defs.md#recipientinfotypedef) 
3. See [:material-code-braces: DecryptResponseTypeDef](./type_defs.md#decryptresponsetypedef) 


```python
# decrypt method usage example with argument unpacking

kwargs: DecryptRequestRequestTypeDef = {  # (1)
    "CiphertextBlob": ...,
}

parent.decrypt(**kwargs)
```

1. See [:material-code-braces: DecryptRequestRequestTypeDef](./type_defs.md#decryptrequestrequesttypedef) 

### delete\_alias

Deletes the specified alias.

Type annotations and code completion for `#!python session.create_client("kms").delete_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_alias)

```python
# delete_alias method definition

await def delete_alias(
    self,
    *,
    AliasName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_alias method usage example with argument unpacking

kwargs: DeleteAliasRequestRequestTypeDef = {  # (1)
    "AliasName": ...,
}

parent.delete_alias(**kwargs)
```

1. See [:material-code-braces: DeleteAliasRequestRequestTypeDef](./type_defs.md#deletealiasrequestrequesttypedef) 

### delete\_custom\_key\_store

Deletes a [custom key
store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-overview.html).

Type annotations and code completion for `#!python session.create_client("kms").delete_custom_key_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_custom_key_store)

```python
# delete_custom_key_store method definition

await def delete_custom_key_store(
    self,
    *,
    CustomKeyStoreId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_custom_key_store method usage example with argument unpacking

kwargs: DeleteCustomKeyStoreRequestRequestTypeDef = {  # (1)
    "CustomKeyStoreId": ...,
}

parent.delete_custom_key_store(**kwargs)
```

1. See [:material-code-braces: DeleteCustomKeyStoreRequestRequestTypeDef](./type_defs.md#deletecustomkeystorerequestrequesttypedef) 

### delete\_imported\_key\_material

Deletes key material that was previously imported.

Type annotations and code completion for `#!python session.create_client("kms").delete_imported_key_material` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_imported_key_material)

```python
# delete_imported_key_material method definition

await def delete_imported_key_material(
    self,
    *,
    KeyId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_imported_key_material method usage example with argument unpacking

kwargs: DeleteImportedKeyMaterialRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.delete_imported_key_material(**kwargs)
```

1. See [:material-code-braces: DeleteImportedKeyMaterialRequestRequestTypeDef](./type_defs.md#deleteimportedkeymaterialrequestrequesttypedef) 

### derive\_shared\_secret

Derives a shared secret using a key agreement algorithm.

Type annotations and code completion for `#!python session.create_client("kms").derive_shared_secret` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.derive_shared_secret)

```python
# derive_shared_secret method definition

await def derive_shared_secret(
    self,
    *,
    KeyId: str,
    KeyAgreementAlgorithm: KeyAgreementAlgorithmSpecType,  # (1)
    PublicKey: BlobTypeDef,
    GrantTokens: Sequence[str] = ...,
    DryRun: bool = ...,
    Recipient: RecipientInfoTypeDef = ...,  # (2)
) -> DeriveSharedSecretResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: KeyAgreementAlgorithmSpecType](./literals.md#keyagreementalgorithmspectype) 
2. See [:material-code-braces: RecipientInfoTypeDef](./type_defs.md#recipientinfotypedef) 
3. See [:material-code-braces: DeriveSharedSecretResponseTypeDef](./type_defs.md#derivesharedsecretresponsetypedef) 


```python
# derive_shared_secret method usage example with argument unpacking

kwargs: DeriveSharedSecretRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "KeyAgreementAlgorithm": ...,
    "PublicKey": ...,
}

parent.derive_shared_secret(**kwargs)
```

1. See [:material-code-braces: DeriveSharedSecretRequestRequestTypeDef](./type_defs.md#derivesharedsecretrequestrequesttypedef) 

### describe\_custom\_key\_stores

Gets information about [custom key
stores](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-overview.html)
in the account and
Region.

Type annotations and code completion for `#!python session.create_client("kms").describe_custom_key_stores` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.describe_custom_key_stores)

```python
# describe_custom_key_stores method definition

await def describe_custom_key_stores(
    self,
    *,
    CustomKeyStoreId: str = ...,
    CustomKeyStoreName: str = ...,
    Limit: int = ...,
    Marker: str = ...,
) -> DescribeCustomKeyStoresResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCustomKeyStoresResponseTypeDef](./type_defs.md#describecustomkeystoresresponsetypedef) 


```python
# describe_custom_key_stores method usage example with argument unpacking

kwargs: DescribeCustomKeyStoresRequestRequestTypeDef = {  # (1)
    "CustomKeyStoreId": ...,
}

parent.describe_custom_key_stores(**kwargs)
```

1. See [:material-code-braces: DescribeCustomKeyStoresRequestRequestTypeDef](./type_defs.md#describecustomkeystoresrequestrequesttypedef) 

### describe\_key

Provides detailed information about a KMS key.

Type annotations and code completion for `#!python session.create_client("kms").describe_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.describe_key)

```python
# describe_key method definition

await def describe_key(
    self,
    *,
    KeyId: str,
    GrantTokens: Sequence[str] = ...,
) -> DescribeKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeKeyResponseTypeDef](./type_defs.md#describekeyresponsetypedef) 


```python
# describe_key method usage example with argument unpacking

kwargs: DescribeKeyRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.describe_key(**kwargs)
```

1. See [:material-code-braces: DescribeKeyRequestRequestTypeDef](./type_defs.md#describekeyrequestrequesttypedef) 

### disable\_key

Sets the state of a KMS key to disabled.

Type annotations and code completion for `#!python session.create_client("kms").disable_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disable_key)

```python
# disable_key method definition

await def disable_key(
    self,
    *,
    KeyId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disable_key method usage example with argument unpacking

kwargs: DisableKeyRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.disable_key(**kwargs)
```

1. See [:material-code-braces: DisableKeyRequestRequestTypeDef](./type_defs.md#disablekeyrequestrequesttypedef) 

### disable\_key\_rotation

Disables [automatic rotation of the key
material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-keys.html)
of the specified symmetric encryption KMS
key.

Type annotations and code completion for `#!python session.create_client("kms").disable_key_rotation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disable_key_rotation)

```python
# disable_key_rotation method definition

await def disable_key_rotation(
    self,
    *,
    KeyId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disable_key_rotation method usage example with argument unpacking

kwargs: DisableKeyRotationRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.disable_key_rotation(**kwargs)
```

1. See [:material-code-braces: DisableKeyRotationRequestRequestTypeDef](./type_defs.md#disablekeyrotationrequestrequesttypedef) 

### disconnect\_custom\_key\_store

Disconnects the [custom key
store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-overview.html)
from its backing key
store.

Type annotations and code completion for `#!python session.create_client("kms").disconnect_custom_key_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disconnect_custom_key_store)

```python
# disconnect_custom_key_store method definition

await def disconnect_custom_key_store(
    self,
    *,
    CustomKeyStoreId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disconnect_custom_key_store method usage example with argument unpacking

kwargs: DisconnectCustomKeyStoreRequestRequestTypeDef = {  # (1)
    "CustomKeyStoreId": ...,
}

parent.disconnect_custom_key_store(**kwargs)
```

1. See [:material-code-braces: DisconnectCustomKeyStoreRequestRequestTypeDef](./type_defs.md#disconnectcustomkeystorerequestrequesttypedef) 

### enable\_key

Sets the key state of a KMS key to enabled.

Type annotations and code completion for `#!python session.create_client("kms").enable_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key)

```python
# enable_key method definition

await def enable_key(
    self,
    *,
    KeyId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# enable_key method usage example with argument unpacking

kwargs: EnableKeyRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.enable_key(**kwargs)
```

1. See [:material-code-braces: EnableKeyRequestRequestTypeDef](./type_defs.md#enablekeyrequestrequesttypedef) 

### enable\_key\_rotation

Enables [automatic rotation of the key
material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-keys.html#rotating-keys-enable-disable)
of the specified symmetric encryption KMS
key.

Type annotations and code completion for `#!python session.create_client("kms").enable_key_rotation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key_rotation)

```python
# enable_key_rotation method definition

await def enable_key_rotation(
    self,
    *,
    KeyId: str,
    RotationPeriodInDays: int = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# enable_key_rotation method usage example with argument unpacking

kwargs: EnableKeyRotationRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.enable_key_rotation(**kwargs)
```

1. See [:material-code-braces: EnableKeyRotationRequestRequestTypeDef](./type_defs.md#enablekeyrotationrequestrequesttypedef) 

### encrypt

Encrypts plaintext of up to 4,096 bytes using a KMS key.

Type annotations and code completion for `#!python session.create_client("kms").encrypt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.encrypt)

```python
# encrypt method definition

await def encrypt(
    self,
    *,
    KeyId: str,
    Plaintext: BlobTypeDef,
    EncryptionContext: Mapping[str, str] = ...,
    GrantTokens: Sequence[str] = ...,
    EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,  # (1)
    DryRun: bool = ...,
) -> EncryptResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
2. See [:material-code-braces: EncryptResponseTypeDef](./type_defs.md#encryptresponsetypedef) 


```python
# encrypt method usage example with argument unpacking

kwargs: EncryptRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "Plaintext": ...,
}

parent.encrypt(**kwargs)
```

1. See [:material-code-braces: EncryptRequestRequestTypeDef](./type_defs.md#encryptrequestrequesttypedef) 

### generate\_data\_key

Returns a unique symmetric data key for use outside of KMS.

Type annotations and code completion for `#!python session.create_client("kms").generate_data_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key)

```python
# generate_data_key method definition

await def generate_data_key(
    self,
    *,
    KeyId: str,
    EncryptionContext: Mapping[str, str] = ...,
    NumberOfBytes: int = ...,
    KeySpec: DataKeySpecType = ...,  # (1)
    GrantTokens: Sequence[str] = ...,
    Recipient: RecipientInfoTypeDef = ...,  # (2)
    DryRun: bool = ...,
) -> GenerateDataKeyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: DataKeySpecType](./literals.md#datakeyspectype) 
2. See [:material-code-braces: RecipientInfoTypeDef](./type_defs.md#recipientinfotypedef) 
3. See [:material-code-braces: GenerateDataKeyResponseTypeDef](./type_defs.md#generatedatakeyresponsetypedef) 


```python
# generate_data_key method usage example with argument unpacking

kwargs: GenerateDataKeyRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.generate_data_key(**kwargs)
```

1. See [:material-code-braces: GenerateDataKeyRequestRequestTypeDef](./type_defs.md#generatedatakeyrequestrequesttypedef) 

### generate\_data\_key\_pair

Returns a unique asymmetric data key pair for use outside of KMS.

Type annotations and code completion for `#!python session.create_client("kms").generate_data_key_pair` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair)

```python
# generate_data_key_pair method definition

await def generate_data_key_pair(
    self,
    *,
    KeyId: str,
    KeyPairSpec: DataKeyPairSpecType,  # (1)
    EncryptionContext: Mapping[str, str] = ...,
    GrantTokens: Sequence[str] = ...,
    Recipient: RecipientInfoTypeDef = ...,  # (2)
    DryRun: bool = ...,
) -> GenerateDataKeyPairResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: DataKeyPairSpecType](./literals.md#datakeypairspectype) 
2. See [:material-code-braces: RecipientInfoTypeDef](./type_defs.md#recipientinfotypedef) 
3. See [:material-code-braces: GenerateDataKeyPairResponseTypeDef](./type_defs.md#generatedatakeypairresponsetypedef) 


```python
# generate_data_key_pair method usage example with argument unpacking

kwargs: GenerateDataKeyPairRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "KeyPairSpec": ...,
}

parent.generate_data_key_pair(**kwargs)
```

1. See [:material-code-braces: GenerateDataKeyPairRequestRequestTypeDef](./type_defs.md#generatedatakeypairrequestrequesttypedef) 

### generate\_data\_key\_pair\_without\_plaintext

Returns a unique asymmetric data key pair for use outside of KMS.

Type annotations and code completion for `#!python session.create_client("kms").generate_data_key_pair_without_plaintext` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair_without_plaintext)

```python
# generate_data_key_pair_without_plaintext method definition

await def generate_data_key_pair_without_plaintext(
    self,
    *,
    KeyId: str,
    KeyPairSpec: DataKeyPairSpecType,  # (1)
    EncryptionContext: Mapping[str, str] = ...,
    GrantTokens: Sequence[str] = ...,
    DryRun: bool = ...,
) -> GenerateDataKeyPairWithoutPlaintextResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataKeyPairSpecType](./literals.md#datakeypairspectype) 
2. See [:material-code-braces: GenerateDataKeyPairWithoutPlaintextResponseTypeDef](./type_defs.md#generatedatakeypairwithoutplaintextresponsetypedef) 


```python
# generate_data_key_pair_without_plaintext method usage example with argument unpacking

kwargs: GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "KeyPairSpec": ...,
}

parent.generate_data_key_pair_without_plaintext(**kwargs)
```

1. See [:material-code-braces: GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef](./type_defs.md#generatedatakeypairwithoutplaintextrequestrequesttypedef) 

### generate\_data\_key\_without\_plaintext

Returns a unique symmetric data key for use outside of KMS.

Type annotations and code completion for `#!python session.create_client("kms").generate_data_key_without_plaintext` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_without_plaintext)

```python
# generate_data_key_without_plaintext method definition

await def generate_data_key_without_plaintext(
    self,
    *,
    KeyId: str,
    EncryptionContext: Mapping[str, str] = ...,
    KeySpec: DataKeySpecType = ...,  # (1)
    NumberOfBytes: int = ...,
    GrantTokens: Sequence[str] = ...,
    DryRun: bool = ...,
) -> GenerateDataKeyWithoutPlaintextResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataKeySpecType](./literals.md#datakeyspectype) 
2. See [:material-code-braces: GenerateDataKeyWithoutPlaintextResponseTypeDef](./type_defs.md#generatedatakeywithoutplaintextresponsetypedef) 


```python
# generate_data_key_without_plaintext method usage example with argument unpacking

kwargs: GenerateDataKeyWithoutPlaintextRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.generate_data_key_without_plaintext(**kwargs)
```

1. See [:material-code-braces: GenerateDataKeyWithoutPlaintextRequestRequestTypeDef](./type_defs.md#generatedatakeywithoutplaintextrequestrequesttypedef) 

### generate\_mac

Generates a hash-based message authentication code (HMAC) for a message using
an HMAC KMS key and a MAC algorithm that the key
supports.

Type annotations and code completion for `#!python session.create_client("kms").generate_mac` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_mac)

```python
# generate_mac method definition

await def generate_mac(
    self,
    *,
    Message: BlobTypeDef,
    KeyId: str,
    MacAlgorithm: MacAlgorithmSpecType,  # (1)
    GrantTokens: Sequence[str] = ...,
    DryRun: bool = ...,
) -> GenerateMacResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MacAlgorithmSpecType](./literals.md#macalgorithmspectype) 
2. See [:material-code-braces: GenerateMacResponseTypeDef](./type_defs.md#generatemacresponsetypedef) 


```python
# generate_mac method usage example with argument unpacking

kwargs: GenerateMacRequestRequestTypeDef = {  # (1)
    "Message": ...,
    "KeyId": ...,
    "MacAlgorithm": ...,
}

parent.generate_mac(**kwargs)
```

1. See [:material-code-braces: GenerateMacRequestRequestTypeDef](./type_defs.md#generatemacrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("kms").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_presigned_url)

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


### generate\_random

Returns a random byte string that is cryptographically secure.

Type annotations and code completion for `#!python session.create_client("kms").generate_random` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_random)

```python
# generate_random method definition

await def generate_random(
    self,
    *,
    NumberOfBytes: int = ...,
    CustomKeyStoreId: str = ...,
    Recipient: RecipientInfoTypeDef = ...,  # (1)
) -> GenerateRandomResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RecipientInfoTypeDef](./type_defs.md#recipientinfotypedef) 
2. See [:material-code-braces: GenerateRandomResponseTypeDef](./type_defs.md#generaterandomresponsetypedef) 


```python
# generate_random method usage example with argument unpacking

kwargs: GenerateRandomRequestRequestTypeDef = {  # (1)
    "NumberOfBytes": ...,
}

parent.generate_random(**kwargs)
```

1. See [:material-code-braces: GenerateRandomRequestRequestTypeDef](./type_defs.md#generaterandomrequestrequesttypedef) 

### get\_key\_policy

Gets a key policy attached to the specified KMS key.

Type annotations and code completion for `#!python session.create_client("kms").get_key_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_policy)

```python
# get_key_policy method definition

await def get_key_policy(
    self,
    *,
    KeyId: str,
    PolicyName: str = ...,
) -> GetKeyPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKeyPolicyResponseTypeDef](./type_defs.md#getkeypolicyresponsetypedef) 


```python
# get_key_policy method usage example with argument unpacking

kwargs: GetKeyPolicyRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.get_key_policy(**kwargs)
```

1. See [:material-code-braces: GetKeyPolicyRequestRequestTypeDef](./type_defs.md#getkeypolicyrequestrequesttypedef) 

### get\_key\_rotation\_status

Provides detailed information about the rotation status for a KMS key,
including whether [automatic rotation of the key
material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-keys.html)
is enabled for the specified KMS key, the `rotation period
<https://docs.aws.amazon.com/kms/...`.

Type annotations and code completion for `#!python session.create_client("kms").get_key_rotation_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_rotation_status)

```python
# get_key_rotation_status method definition

await def get_key_rotation_status(
    self,
    *,
    KeyId: str,
) -> GetKeyRotationStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKeyRotationStatusResponseTypeDef](./type_defs.md#getkeyrotationstatusresponsetypedef) 


```python
# get_key_rotation_status method usage example with argument unpacking

kwargs: GetKeyRotationStatusRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.get_key_rotation_status(**kwargs)
```

1. See [:material-code-braces: GetKeyRotationStatusRequestRequestTypeDef](./type_defs.md#getkeyrotationstatusrequestrequesttypedef) 

### get\_parameters\_for\_import

Returns the public key and an import token you need to import or reimport key
material for a KMS
key.

Type annotations and code completion for `#!python session.create_client("kms").get_parameters_for_import` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_parameters_for_import)

```python
# get_parameters_for_import method definition

await def get_parameters_for_import(
    self,
    *,
    KeyId: str,
    WrappingAlgorithm: AlgorithmSpecType,  # (1)
    WrappingKeySpec: WrappingKeySpecType,  # (2)
) -> GetParametersForImportResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AlgorithmSpecType](./literals.md#algorithmspectype) 
2. See [:material-code-brackets: WrappingKeySpecType](./literals.md#wrappingkeyspectype) 
3. See [:material-code-braces: GetParametersForImportResponseTypeDef](./type_defs.md#getparametersforimportresponsetypedef) 


```python
# get_parameters_for_import method usage example with argument unpacking

kwargs: GetParametersForImportRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "WrappingAlgorithm": ...,
    "WrappingKeySpec": ...,
}

parent.get_parameters_for_import(**kwargs)
```

1. See [:material-code-braces: GetParametersForImportRequestRequestTypeDef](./type_defs.md#getparametersforimportrequestrequesttypedef) 

### get\_public\_key

Returns the public key of an asymmetric KMS key.

Type annotations and code completion for `#!python session.create_client("kms").get_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_public_key)

```python
# get_public_key method definition

await def get_public_key(
    self,
    *,
    KeyId: str,
    GrantTokens: Sequence[str] = ...,
) -> GetPublicKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPublicKeyResponseTypeDef](./type_defs.md#getpublickeyresponsetypedef) 


```python
# get_public_key method usage example with argument unpacking

kwargs: GetPublicKeyRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.get_public_key(**kwargs)
```

1. See [:material-code-braces: GetPublicKeyRequestRequestTypeDef](./type_defs.md#getpublickeyrequestrequesttypedef) 

### import\_key\_material

Imports or reimports key material into an existing KMS key that was created
without key
material.

Type annotations and code completion for `#!python session.create_client("kms").import_key_material` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.import_key_material)

```python
# import_key_material method definition

await def import_key_material(
    self,
    *,
    KeyId: str,
    ImportToken: BlobTypeDef,
    EncryptedKeyMaterial: BlobTypeDef,
    ValidTo: TimestampTypeDef = ...,
    ExpirationModel: ExpirationModelTypeType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ExpirationModelTypeType](./literals.md#expirationmodeltypetype) 


```python
# import_key_material method usage example with argument unpacking

kwargs: ImportKeyMaterialRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "ImportToken": ...,
    "EncryptedKeyMaterial": ...,
}

parent.import_key_material(**kwargs)
```

1. See [:material-code-braces: ImportKeyMaterialRequestRequestTypeDef](./type_defs.md#importkeymaterialrequestrequesttypedef) 

### list\_aliases

Gets a list of aliases in the caller's Amazon Web Services account and region.

Type annotations and code completion for `#!python session.create_client("kms").list_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_aliases)

```python
# list_aliases method definition

await def list_aliases(
    self,
    *,
    KeyId: str = ...,
    Limit: int = ...,
    Marker: str = ...,
) -> ListAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 


```python
# list_aliases method usage example with argument unpacking

kwargs: ListAliasesRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.list_aliases(**kwargs)
```

1. See [:material-code-braces: ListAliasesRequestRequestTypeDef](./type_defs.md#listaliasesrequestrequesttypedef) 

### list\_grants

Gets a list of all grants for the specified KMS key.

Type annotations and code completion for `#!python session.create_client("kms").list_grants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_grants)

```python
# list_grants method definition

await def list_grants(
    self,
    *,
    KeyId: str,
    Limit: int = ...,
    Marker: str = ...,
    GrantId: str = ...,
    GranteePrincipal: str = ...,
) -> ListGrantsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGrantsResponseTypeDef](./type_defs.md#listgrantsresponsetypedef) 


```python
# list_grants method usage example with argument unpacking

kwargs: ListGrantsRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.list_grants(**kwargs)
```

1. See [:material-code-braces: ListGrantsRequestRequestTypeDef](./type_defs.md#listgrantsrequestrequesttypedef) 

### list\_key\_policies

Gets the names of the key policies that are attached to a KMS key.

Type annotations and code completion for `#!python session.create_client("kms").list_key_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_key_policies)

```python
# list_key_policies method definition

await def list_key_policies(
    self,
    *,
    KeyId: str,
    Limit: int = ...,
    Marker: str = ...,
) -> ListKeyPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKeyPoliciesResponseTypeDef](./type_defs.md#listkeypoliciesresponsetypedef) 


```python
# list_key_policies method usage example with argument unpacking

kwargs: ListKeyPoliciesRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.list_key_policies(**kwargs)
```

1. See [:material-code-braces: ListKeyPoliciesRequestRequestTypeDef](./type_defs.md#listkeypoliciesrequestrequesttypedef) 

### list\_key\_rotations

Returns information about all completed key material rotations for the
specified KMS
key.

Type annotations and code completion for `#!python session.create_client("kms").list_key_rotations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_key_rotations)

```python
# list_key_rotations method definition

await def list_key_rotations(
    self,
    *,
    KeyId: str,
    Limit: int = ...,
    Marker: str = ...,
) -> ListKeyRotationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKeyRotationsResponseTypeDef](./type_defs.md#listkeyrotationsresponsetypedef) 


```python
# list_key_rotations method usage example with argument unpacking

kwargs: ListKeyRotationsRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.list_key_rotations(**kwargs)
```

1. See [:material-code-braces: ListKeyRotationsRequestRequestTypeDef](./type_defs.md#listkeyrotationsrequestrequesttypedef) 

### list\_keys

Gets a list of all KMS keys in the caller's Amazon Web Services account and
Region.

Type annotations and code completion for `#!python session.create_client("kms").list_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_keys)

```python
# list_keys method definition

await def list_keys(
    self,
    *,
    Limit: int = ...,
    Marker: str = ...,
) -> ListKeysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef) 


```python
# list_keys method usage example with argument unpacking

kwargs: ListKeysRequestRequestTypeDef = {  # (1)
    "Limit": ...,
}

parent.list_keys(**kwargs)
```

1. See [:material-code-braces: ListKeysRequestRequestTypeDef](./type_defs.md#listkeysrequestrequesttypedef) 

### list\_resource\_tags

Returns all tags on the specified KMS key.

Type annotations and code completion for `#!python session.create_client("kms").list_resource_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_resource_tags)

```python
# list_resource_tags method definition

await def list_resource_tags(
    self,
    *,
    KeyId: str,
    Limit: int = ...,
    Marker: str = ...,
) -> ListResourceTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResourceTagsResponseTypeDef](./type_defs.md#listresourcetagsresponsetypedef) 


```python
# list_resource_tags method usage example with argument unpacking

kwargs: ListResourceTagsRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.list_resource_tags(**kwargs)
```

1. See [:material-code-braces: ListResourceTagsRequestRequestTypeDef](./type_defs.md#listresourcetagsrequestrequesttypedef) 

### list\_retirable\_grants

Returns information about all grants in the Amazon Web Services account and
Region that have the specified retiring
principal.

Type annotations and code completion for `#!python session.create_client("kms").list_retirable_grants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_retirable_grants)

```python
# list_retirable_grants method definition

await def list_retirable_grants(
    self,
    *,
    RetiringPrincipal: str,
    Limit: int = ...,
    Marker: str = ...,
) -> ListGrantsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGrantsResponseTypeDef](./type_defs.md#listgrantsresponsetypedef) 


```python
# list_retirable_grants method usage example with argument unpacking

kwargs: ListRetirableGrantsRequestRequestTypeDef = {  # (1)
    "RetiringPrincipal": ...,
}

parent.list_retirable_grants(**kwargs)
```

1. See [:material-code-braces: ListRetirableGrantsRequestRequestTypeDef](./type_defs.md#listretirablegrantsrequestrequesttypedef) 

### put\_key\_policy

Attaches a key policy to the specified KMS key.

Type annotations and code completion for `#!python session.create_client("kms").put_key_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.put_key_policy)

```python
# put_key_policy method definition

await def put_key_policy(
    self,
    *,
    KeyId: str,
    Policy: str,
    PolicyName: str = ...,
    BypassPolicyLockoutSafetyCheck: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_key_policy method usage example with argument unpacking

kwargs: PutKeyPolicyRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "Policy": ...,
}

parent.put_key_policy(**kwargs)
```

1. See [:material-code-braces: PutKeyPolicyRequestRequestTypeDef](./type_defs.md#putkeypolicyrequestrequesttypedef) 

### re\_encrypt

Decrypts ciphertext and then reencrypts it entirely within KMS.

Type annotations and code completion for `#!python session.create_client("kms").re_encrypt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.re_encrypt)

```python
# re_encrypt method definition

await def re_encrypt(
    self,
    *,
    CiphertextBlob: BlobTypeDef,
    DestinationKeyId: str,
    SourceEncryptionContext: Mapping[str, str] = ...,
    SourceKeyId: str = ...,
    DestinationEncryptionContext: Mapping[str, str] = ...,
    SourceEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,  # (1)
    DestinationEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,  # (1)
    GrantTokens: Sequence[str] = ...,
    DryRun: bool = ...,
) -> ReEncryptResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
2. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
3. See [:material-code-braces: ReEncryptResponseTypeDef](./type_defs.md#reencryptresponsetypedef) 


```python
# re_encrypt method usage example with argument unpacking

kwargs: ReEncryptRequestRequestTypeDef = {  # (1)
    "CiphertextBlob": ...,
    "DestinationKeyId": ...,
}

parent.re_encrypt(**kwargs)
```

1. See [:material-code-braces: ReEncryptRequestRequestTypeDef](./type_defs.md#reencryptrequestrequesttypedef) 

### replicate\_key

Replicates a multi-Region key into the specified Region.

Type annotations and code completion for `#!python session.create_client("kms").replicate_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.replicate_key)

```python
# replicate_key method definition

await def replicate_key(
    self,
    *,
    KeyId: str,
    ReplicaRegion: str,
    Policy: str = ...,
    BypassPolicyLockoutSafetyCheck: bool = ...,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> ReplicateKeyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ReplicateKeyResponseTypeDef](./type_defs.md#replicatekeyresponsetypedef) 


```python
# replicate_key method usage example with argument unpacking

kwargs: ReplicateKeyRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "ReplicaRegion": ...,
}

parent.replicate_key(**kwargs)
```

1. See [:material-code-braces: ReplicateKeyRequestRequestTypeDef](./type_defs.md#replicatekeyrequestrequesttypedef) 

### retire\_grant

Deletes a grant.

Type annotations and code completion for `#!python session.create_client("kms").retire_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.retire_grant)

```python
# retire_grant method definition

await def retire_grant(
    self,
    *,
    GrantToken: str = ...,
    KeyId: str = ...,
    GrantId: str = ...,
    DryRun: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# retire_grant method usage example with argument unpacking

kwargs: RetireGrantRequestRequestTypeDef = {  # (1)
    "GrantToken": ...,
}

parent.retire_grant(**kwargs)
```

1. See [:material-code-braces: RetireGrantRequestRequestTypeDef](./type_defs.md#retiregrantrequestrequesttypedef) 

### revoke\_grant

Deletes the specified grant.

Type annotations and code completion for `#!python session.create_client("kms").revoke_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.revoke_grant)

```python
# revoke_grant method definition

await def revoke_grant(
    self,
    *,
    KeyId: str,
    GrantId: str,
    DryRun: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# revoke_grant method usage example with argument unpacking

kwargs: RevokeGrantRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "GrantId": ...,
}

parent.revoke_grant(**kwargs)
```

1. See [:material-code-braces: RevokeGrantRequestRequestTypeDef](./type_defs.md#revokegrantrequestrequesttypedef) 

### rotate\_key\_on\_demand

Immediately initiates rotation of the key material of the specified symmetric
encryption KMS
key.

Type annotations and code completion for `#!python session.create_client("kms").rotate_key_on_demand` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.rotate_key_on_demand)

```python
# rotate_key_on_demand method definition

await def rotate_key_on_demand(
    self,
    *,
    KeyId: str,
) -> RotateKeyOnDemandResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RotateKeyOnDemandResponseTypeDef](./type_defs.md#rotatekeyondemandresponsetypedef) 


```python
# rotate_key_on_demand method usage example with argument unpacking

kwargs: RotateKeyOnDemandRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.rotate_key_on_demand(**kwargs)
```

1. See [:material-code-braces: RotateKeyOnDemandRequestRequestTypeDef](./type_defs.md#rotatekeyondemandrequestrequesttypedef) 

### schedule\_key\_deletion

Schedules the deletion of a KMS key.

Type annotations and code completion for `#!python session.create_client("kms").schedule_key_deletion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.schedule_key_deletion)

```python
# schedule_key_deletion method definition

await def schedule_key_deletion(
    self,
    *,
    KeyId: str,
    PendingWindowInDays: int = ...,
) -> ScheduleKeyDeletionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ScheduleKeyDeletionResponseTypeDef](./type_defs.md#schedulekeydeletionresponsetypedef) 


```python
# schedule_key_deletion method usage example with argument unpacking

kwargs: ScheduleKeyDeletionRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
}

parent.schedule_key_deletion(**kwargs)
```

1. See [:material-code-braces: ScheduleKeyDeletionRequestRequestTypeDef](./type_defs.md#schedulekeydeletionrequestrequesttypedef) 

### sign

Creates a [digital signature](https://en.wikipedia.org/wiki/Digital_signature)
for a message or message digest by using the private key in an asymmetric
signing KMS
key.

Type annotations and code completion for `#!python session.create_client("kms").sign` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.sign)

```python
# sign method definition

await def sign(
    self,
    *,
    KeyId: str,
    Message: BlobTypeDef,
    SigningAlgorithm: SigningAlgorithmSpecType,  # (1)
    MessageType: MessageTypeType = ...,  # (2)
    GrantTokens: Sequence[str] = ...,
    DryRun: bool = ...,
) -> SignResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SigningAlgorithmSpecType](./literals.md#signingalgorithmspectype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-braces: SignResponseTypeDef](./type_defs.md#signresponsetypedef) 


```python
# sign method usage example with argument unpacking

kwargs: SignRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "Message": ...,
    "SigningAlgorithm": ...,
}

parent.sign(**kwargs)
```

1. See [:material-code-braces: SignRequestRequestTypeDef](./type_defs.md#signrequestrequesttypedef) 

### tag\_resource

Adds or edits tags on a [customer managed
key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#customer-cmk).

Type annotations and code completion for `#!python session.create_client("kms").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    KeyId: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Deletes tags from a [customer managed
key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#customer-cmk).

Type annotations and code completion for `#!python session.create_client("kms").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    KeyId: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_alias

Associates an existing KMS alias with a different KMS key.

Type annotations and code completion for `#!python session.create_client("kms").update_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_alias)

```python
# update_alias method definition

await def update_alias(
    self,
    *,
    AliasName: str,
    TargetKeyId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_alias method usage example with argument unpacking

kwargs: UpdateAliasRequestRequestTypeDef = {  # (1)
    "AliasName": ...,
    "TargetKeyId": ...,
}

parent.update_alias(**kwargs)
```

1. See [:material-code-braces: UpdateAliasRequestRequestTypeDef](./type_defs.md#updatealiasrequestrequesttypedef) 

### update\_custom\_key\_store

Changes the properties of a custom key store.

Type annotations and code completion for `#!python session.create_client("kms").update_custom_key_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_custom_key_store)

```python
# update_custom_key_store method definition

await def update_custom_key_store(
    self,
    *,
    CustomKeyStoreId: str,
    NewCustomKeyStoreName: str = ...,
    KeyStorePassword: str = ...,
    CloudHsmClusterId: str = ...,
    XksProxyUriEndpoint: str = ...,
    XksProxyUriPath: str = ...,
    XksProxyVpcEndpointServiceName: str = ...,
    XksProxyAuthenticationCredential: XksProxyAuthenticationCredentialTypeTypeDef = ...,  # (1)
    XksProxyConnectivity: XksProxyConnectivityTypeType = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: XksProxyAuthenticationCredentialTypeTypeDef](./type_defs.md#xksproxyauthenticationcredentialtypetypedef) 
2. See [:material-code-brackets: XksProxyConnectivityTypeType](./literals.md#xksproxyconnectivitytypetype) 


```python
# update_custom_key_store method usage example with argument unpacking

kwargs: UpdateCustomKeyStoreRequestRequestTypeDef = {  # (1)
    "CustomKeyStoreId": ...,
}

parent.update_custom_key_store(**kwargs)
```

1. See [:material-code-braces: UpdateCustomKeyStoreRequestRequestTypeDef](./type_defs.md#updatecustomkeystorerequestrequesttypedef) 

### update\_key\_description

Updates the description of a KMS key.

Type annotations and code completion for `#!python session.create_client("kms").update_key_description` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_key_description)

```python
# update_key_description method definition

await def update_key_description(
    self,
    *,
    KeyId: str,
    Description: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_key_description method usage example with argument unpacking

kwargs: UpdateKeyDescriptionRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "Description": ...,
}

parent.update_key_description(**kwargs)
```

1. See [:material-code-braces: UpdateKeyDescriptionRequestRequestTypeDef](./type_defs.md#updatekeydescriptionrequestrequesttypedef) 

### update\_primary\_region

Changes the primary key of a multi-Region key.

Type annotations and code completion for `#!python session.create_client("kms").update_primary_region` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_primary_region)

```python
# update_primary_region method definition

await def update_primary_region(
    self,
    *,
    KeyId: str,
    PrimaryRegion: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_primary_region method usage example with argument unpacking

kwargs: UpdatePrimaryRegionRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "PrimaryRegion": ...,
}

parent.update_primary_region(**kwargs)
```

1. See [:material-code-braces: UpdatePrimaryRegionRequestRequestTypeDef](./type_defs.md#updateprimaryregionrequestrequesttypedef) 

### verify

Verifies a digital signature that was generated by the  Sign operation.

Type annotations and code completion for `#!python session.create_client("kms").verify` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify)

```python
# verify method definition

await def verify(
    self,
    *,
    KeyId: str,
    Message: BlobTypeDef,
    Signature: BlobTypeDef,
    SigningAlgorithm: SigningAlgorithmSpecType,  # (1)
    MessageType: MessageTypeType = ...,  # (2)
    GrantTokens: Sequence[str] = ...,
    DryRun: bool = ...,
) -> VerifyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SigningAlgorithmSpecType](./literals.md#signingalgorithmspectype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-braces: VerifyResponseTypeDef](./type_defs.md#verifyresponsetypedef) 


```python
# verify method usage example with argument unpacking

kwargs: VerifyRequestRequestTypeDef = {  # (1)
    "KeyId": ...,
    "Message": ...,
    "Signature": ...,
    "SigningAlgorithm": ...,
}

parent.verify(**kwargs)
```

1. See [:material-code-braces: VerifyRequestRequestTypeDef](./type_defs.md#verifyrequestrequesttypedef) 

### verify\_mac

Verifies the hash-based message authentication code (HMAC) for a specified
message, HMAC KMS key, and MAC
algorithm.

Type annotations and code completion for `#!python session.create_client("kms").verify_mac` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify_mac)

```python
# verify_mac method definition

await def verify_mac(
    self,
    *,
    Message: BlobTypeDef,
    KeyId: str,
    MacAlgorithm: MacAlgorithmSpecType,  # (1)
    Mac: BlobTypeDef,
    GrantTokens: Sequence[str] = ...,
    DryRun: bool = ...,
) -> VerifyMacResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MacAlgorithmSpecType](./literals.md#macalgorithmspectype) 
2. See [:material-code-braces: VerifyMacResponseTypeDef](./type_defs.md#verifymacresponsetypedef) 


```python
# verify_mac method usage example with argument unpacking

kwargs: VerifyMacRequestRequestTypeDef = {  # (1)
    "Message": ...,
    "KeyId": ...,
    "MacAlgorithm": ...,
    "Mac": ...,
}

parent.verify_mac(**kwargs)
```

1. See [:material-code-braces: VerifyMacRequestRequestTypeDef](./type_defs.md#verifymacrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("kms").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "KMSClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("kms").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.__aexit__)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator` method with overloads.

- `client.get_paginator("describe_custom_key_stores")` -> [DescribeCustomKeyStoresPaginator](./paginators.md#describecustomkeystorespaginator)
- `client.get_paginator("list_aliases")` -> [ListAliasesPaginator](./paginators.md#listaliasespaginator)
- `client.get_paginator("list_grants")` -> [ListGrantsPaginator](./paginators.md#listgrantspaginator)
- `client.get_paginator("list_key_policies")` -> [ListKeyPoliciesPaginator](./paginators.md#listkeypoliciespaginator)
- `client.get_paginator("list_key_rotations")` -> [ListKeyRotationsPaginator](./paginators.md#listkeyrotationspaginator)
- `client.get_paginator("list_keys")` -> [ListKeysPaginator](./paginators.md#listkeyspaginator)
- `client.get_paginator("list_resource_tags")` -> [ListResourceTagsPaginator](./paginators.md#listresourcetagspaginator)
- `client.get_paginator("list_retirable_grants")` -> [ListRetirableGrantsPaginator](./paginators.md#listretirablegrantspaginator)



