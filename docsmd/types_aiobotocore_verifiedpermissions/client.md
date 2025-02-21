# VerifiedPermissionsClient

> [Index](../README.md) > [VerifiedPermissions](./README.md) > VerifiedPermissionsClient

!!! note ""

    Auto-generated documentation for [VerifiedPermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#verifiedpermissions)
    type annotations stubs module [types-aiobotocore-verifiedpermissions](https://pypi.org/project/types-aiobotocore-verifiedpermissions/).

## VerifiedPermissionsClient

Type annotations and code completion for `#!python session.create_client("verifiedpermissions")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client)

```python
# VerifiedPermissionsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_verifiedpermissions.client import VerifiedPermissionsClient

session = get_session()
async with session.create_client("verifiedpermissions") as client:
    client: VerifiedPermissionsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("verifiedpermissions").exceptions` structure.

```python
# VerifiedPermissionsClient.exceptions usage example

async with session.create_client("verifiedpermissions") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# VerifiedPermissionsClient usage type checking example

from types_aiobotocore_verifiedpermissions.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("verifiedpermissions").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("verifiedpermissions").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/generate_presigned_url.html)

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


### batch\_get\_policy

Retrieves information about a group (batch) of policies.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").batch_get_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/batch_get_policy.html)

```python
# batch_get_policy method definition

await def batch_get_policy(
    self,
    *,
    requests: Sequence[BatchGetPolicyInputItemTypeDef],  # (1)
) -> BatchGetPolicyOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchGetPolicyInputItemTypeDef](./type_defs.md#batchgetpolicyinputitemtypedef) 
2. See [:material-code-braces: BatchGetPolicyOutputTypeDef](./type_defs.md#batchgetpolicyoutputtypedef) 


```python
# batch_get_policy method usage example with argument unpacking

kwargs: BatchGetPolicyInputTypeDef = {  # (1)
    "requests": ...,
}

parent.batch_get_policy(**kwargs)
```

1. See [:material-code-braces: BatchGetPolicyInputTypeDef](./type_defs.md#batchgetpolicyinputtypedef) 

### batch\_is\_authorized

Makes a series of decisions about multiple authorization requests for one
principal or resource.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").batch_is_authorized` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/batch_is_authorized.html)

```python
# batch_is_authorized method definition

await def batch_is_authorized(
    self,
    *,
    policyStoreId: str,
    requests: Sequence[BatchIsAuthorizedInputItemUnionTypeDef],  # (1)
    entities: EntitiesDefinitionTypeDef = ...,  # (2)
) -> BatchIsAuthorizedOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: BatchIsAuthorizedInputItemTypeDef](./type_defs.md#batchisauthorizedinputitemtypedef) [:material-code-braces: BatchIsAuthorizedInputItemOutputTypeDef](./type_defs.md#batchisauthorizedinputitemoutputtypedef) 
2. See [:material-code-braces: EntitiesDefinitionTypeDef](./type_defs.md#entitiesdefinitiontypedef) 
3. See [:material-code-braces: BatchIsAuthorizedOutputTypeDef](./type_defs.md#batchisauthorizedoutputtypedef) 


```python
# batch_is_authorized method usage example with argument unpacking

kwargs: BatchIsAuthorizedInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "requests": ...,
}

parent.batch_is_authorized(**kwargs)
```

1. See [:material-code-braces: BatchIsAuthorizedInputTypeDef](./type_defs.md#batchisauthorizedinputtypedef) 

### batch\_is\_authorized\_with\_token

Makes a series of decisions about multiple authorization requests for one token.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").batch_is_authorized_with_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/batch_is_authorized_with_token.html)

```python
# batch_is_authorized_with_token method definition

await def batch_is_authorized_with_token(
    self,
    *,
    policyStoreId: str,
    requests: Sequence[BatchIsAuthorizedWithTokenInputItemUnionTypeDef],  # (1)
    identityToken: str = ...,
    accessToken: str = ...,
    entities: EntitiesDefinitionTypeDef = ...,  # (2)
) -> BatchIsAuthorizedWithTokenOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: BatchIsAuthorizedWithTokenInputItemTypeDef](./type_defs.md#batchisauthorizedwithtokeninputitemtypedef) [:material-code-braces: BatchIsAuthorizedWithTokenInputItemOutputTypeDef](./type_defs.md#batchisauthorizedwithtokeninputitemoutputtypedef) 
2. See [:material-code-braces: EntitiesDefinitionTypeDef](./type_defs.md#entitiesdefinitiontypedef) 
3. See [:material-code-braces: BatchIsAuthorizedWithTokenOutputTypeDef](./type_defs.md#batchisauthorizedwithtokenoutputtypedef) 


```python
# batch_is_authorized_with_token method usage example with argument unpacking

kwargs: BatchIsAuthorizedWithTokenInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "requests": ...,
}

parent.batch_is_authorized_with_token(**kwargs)
```

1. See [:material-code-braces: BatchIsAuthorizedWithTokenInputTypeDef](./type_defs.md#batchisauthorizedwithtokeninputtypedef) 

### create\_identity\_source

Adds an identity source to a policy store-an Amazon Cognito user pool or OpenID
Connect (OIDC) identity provider (IdP).

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").create_identity_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/create_identity_source.html)

```python
# create_identity_source method definition

await def create_identity_source(
    self,
    *,
    policyStoreId: str,
    configuration: ConfigurationTypeDef,  # (1)
    clientToken: str = ...,
    principalEntityType: str = ...,
) -> CreateIdentitySourceOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
2. See [:material-code-braces: CreateIdentitySourceOutputTypeDef](./type_defs.md#createidentitysourceoutputtypedef) 


```python
# create_identity_source method usage example with argument unpacking

kwargs: CreateIdentitySourceInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "configuration": ...,
}

parent.create_identity_source(**kwargs)
```

1. See [:material-code-braces: CreateIdentitySourceInputTypeDef](./type_defs.md#createidentitysourceinputtypedef) 

### create\_policy

Creates a Cedar policy and saves it in the specified policy store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").create_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/create_policy.html)

```python
# create_policy method definition

await def create_policy(
    self,
    *,
    policyStoreId: str,
    definition: PolicyDefinitionTypeDef,  # (1)
    clientToken: str = ...,
) -> CreatePolicyOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PolicyDefinitionTypeDef](./type_defs.md#policydefinitiontypedef) 
2. See [:material-code-braces: CreatePolicyOutputTypeDef](./type_defs.md#createpolicyoutputtypedef) 


```python
# create_policy method usage example with argument unpacking

kwargs: CreatePolicyInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "definition": ...,
}

parent.create_policy(**kwargs)
```

1. See [:material-code-braces: CreatePolicyInputTypeDef](./type_defs.md#createpolicyinputtypedef) 

### create\_policy\_store

Creates a policy store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").create_policy_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/create_policy_store.html)

```python
# create_policy_store method definition

await def create_policy_store(
    self,
    *,
    validationSettings: ValidationSettingsTypeDef,  # (1)
    clientToken: str = ...,
    description: str = ...,
) -> CreatePolicyStoreOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ValidationSettingsTypeDef](./type_defs.md#validationsettingstypedef) 
2. See [:material-code-braces: CreatePolicyStoreOutputTypeDef](./type_defs.md#createpolicystoreoutputtypedef) 


```python
# create_policy_store method usage example with argument unpacking

kwargs: CreatePolicyStoreInputTypeDef = {  # (1)
    "validationSettings": ...,
}

parent.create_policy_store(**kwargs)
```

1. See [:material-code-braces: CreatePolicyStoreInputTypeDef](./type_defs.md#createpolicystoreinputtypedef) 

### create\_policy\_template

Creates a policy template.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").create_policy_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/create_policy_template.html)

```python
# create_policy_template method definition

await def create_policy_template(
    self,
    *,
    policyStoreId: str,
    statement: str,
    clientToken: str = ...,
    description: str = ...,
) -> CreatePolicyTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePolicyTemplateOutputTypeDef](./type_defs.md#createpolicytemplateoutputtypedef) 


```python
# create_policy_template method usage example with argument unpacking

kwargs: CreatePolicyTemplateInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "statement": ...,
}

parent.create_policy_template(**kwargs)
```

1. See [:material-code-braces: CreatePolicyTemplateInputTypeDef](./type_defs.md#createpolicytemplateinputtypedef) 

### delete\_identity\_source

Deletes an identity source that references an identity provider (IdP) such as
Amazon Cognito.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").delete_identity_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/delete_identity_source.html)

```python
# delete_identity_source method definition

await def delete_identity_source(
    self,
    *,
    policyStoreId: str,
    identitySourceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_identity_source method usage example with argument unpacking

kwargs: DeleteIdentitySourceInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "identitySourceId": ...,
}

parent.delete_identity_source(**kwargs)
```

1. See [:material-code-braces: DeleteIdentitySourceInputTypeDef](./type_defs.md#deleteidentitysourceinputtypedef) 

### delete\_policy

Deletes the specified policy from the policy store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").delete_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/delete_policy.html)

```python
# delete_policy method definition

await def delete_policy(
    self,
    *,
    policyStoreId: str,
    policyId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_policy method usage example with argument unpacking

kwargs: DeletePolicyInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "policyId": ...,
}

parent.delete_policy(**kwargs)
```

1. See [:material-code-braces: DeletePolicyInputTypeDef](./type_defs.md#deletepolicyinputtypedef) 

### delete\_policy\_store

Deletes the specified policy store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").delete_policy_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/delete_policy_store.html)

```python
# delete_policy_store method definition

await def delete_policy_store(
    self,
    *,
    policyStoreId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_policy_store method usage example with argument unpacking

kwargs: DeletePolicyStoreInputTypeDef = {  # (1)
    "policyStoreId": ...,
}

parent.delete_policy_store(**kwargs)
```

1. See [:material-code-braces: DeletePolicyStoreInputTypeDef](./type_defs.md#deletepolicystoreinputtypedef) 

### delete\_policy\_template

Deletes the specified policy template from the policy store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").delete_policy_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/delete_policy_template.html)

```python
# delete_policy_template method definition

await def delete_policy_template(
    self,
    *,
    policyStoreId: str,
    policyTemplateId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_policy_template method usage example with argument unpacking

kwargs: DeletePolicyTemplateInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "policyTemplateId": ...,
}

parent.delete_policy_template(**kwargs)
```

1. See [:material-code-braces: DeletePolicyTemplateInputTypeDef](./type_defs.md#deletepolicytemplateinputtypedef) 

### get\_identity\_source

Retrieves the details about the specified identity source.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").get_identity_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/get_identity_source.html)

```python
# get_identity_source method definition

await def get_identity_source(
    self,
    *,
    policyStoreId: str,
    identitySourceId: str,
) -> GetIdentitySourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdentitySourceOutputTypeDef](./type_defs.md#getidentitysourceoutputtypedef) 


```python
# get_identity_source method usage example with argument unpacking

kwargs: GetIdentitySourceInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "identitySourceId": ...,
}

parent.get_identity_source(**kwargs)
```

1. See [:material-code-braces: GetIdentitySourceInputTypeDef](./type_defs.md#getidentitysourceinputtypedef) 

### get\_policy

Retrieves information about the specified policy.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").get_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/get_policy.html)

```python
# get_policy method definition

await def get_policy(
    self,
    *,
    policyStoreId: str,
    policyId: str,
) -> GetPolicyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyOutputTypeDef](./type_defs.md#getpolicyoutputtypedef) 


```python
# get_policy method usage example with argument unpacking

kwargs: GetPolicyInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "policyId": ...,
}

parent.get_policy(**kwargs)
```

1. See [:material-code-braces: GetPolicyInputTypeDef](./type_defs.md#getpolicyinputtypedef) 

### get\_policy\_store

Retrieves details about a policy store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").get_policy_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/get_policy_store.html)

```python
# get_policy_store method definition

await def get_policy_store(
    self,
    *,
    policyStoreId: str,
) -> GetPolicyStoreOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyStoreOutputTypeDef](./type_defs.md#getpolicystoreoutputtypedef) 


```python
# get_policy_store method usage example with argument unpacking

kwargs: GetPolicyStoreInputTypeDef = {  # (1)
    "policyStoreId": ...,
}

parent.get_policy_store(**kwargs)
```

1. See [:material-code-braces: GetPolicyStoreInputTypeDef](./type_defs.md#getpolicystoreinputtypedef) 

### get\_policy\_template

Retrieve the details for the specified policy template in the specified policy
store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").get_policy_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/get_policy_template.html)

```python
# get_policy_template method definition

await def get_policy_template(
    self,
    *,
    policyStoreId: str,
    policyTemplateId: str,
) -> GetPolicyTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyTemplateOutputTypeDef](./type_defs.md#getpolicytemplateoutputtypedef) 


```python
# get_policy_template method usage example with argument unpacking

kwargs: GetPolicyTemplateInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "policyTemplateId": ...,
}

parent.get_policy_template(**kwargs)
```

1. See [:material-code-braces: GetPolicyTemplateInputTypeDef](./type_defs.md#getpolicytemplateinputtypedef) 

### get\_schema

Retrieve the details for the specified schema in the specified policy store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").get_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/get_schema.html)

```python
# get_schema method definition

await def get_schema(
    self,
    *,
    policyStoreId: str,
) -> GetSchemaOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSchemaOutputTypeDef](./type_defs.md#getschemaoutputtypedef) 


```python
# get_schema method usage example with argument unpacking

kwargs: GetSchemaInputTypeDef = {  # (1)
    "policyStoreId": ...,
}

parent.get_schema(**kwargs)
```

1. See [:material-code-braces: GetSchemaInputTypeDef](./type_defs.md#getschemainputtypedef) 

### is\_authorized

Makes an authorization decision about a service request described in the
parameters.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").is_authorized` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/is_authorized.html)

```python
# is_authorized method definition

await def is_authorized(
    self,
    *,
    policyStoreId: str,
    principal: EntityIdentifierTypeDef = ...,  # (1)
    action: ActionIdentifierTypeDef = ...,  # (2)
    resource: EntityIdentifierTypeDef = ...,  # (1)
    context: ContextDefinitionUnionTypeDef = ...,  # (4)
    entities: EntitiesDefinitionTypeDef = ...,  # (5)
) -> IsAuthorizedOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
2. See [:material-code-braces: ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
4. See [:material-code-braces: ContextDefinitionTypeDef](./type_defs.md#contextdefinitiontypedef) [:material-code-braces: ContextDefinitionOutputTypeDef](./type_defs.md#contextdefinitionoutputtypedef) 
5. See [:material-code-braces: EntitiesDefinitionTypeDef](./type_defs.md#entitiesdefinitiontypedef) 
6. See [:material-code-braces: IsAuthorizedOutputTypeDef](./type_defs.md#isauthorizedoutputtypedef) 


```python
# is_authorized method usage example with argument unpacking

kwargs: IsAuthorizedInputTypeDef = {  # (1)
    "policyStoreId": ...,
}

parent.is_authorized(**kwargs)
```

1. See [:material-code-braces: IsAuthorizedInputTypeDef](./type_defs.md#isauthorizedinputtypedef) 

### is\_authorized\_with\_token

Makes an authorization decision about a service request described in the
parameters.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").is_authorized_with_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/is_authorized_with_token.html)

```python
# is_authorized_with_token method definition

await def is_authorized_with_token(
    self,
    *,
    policyStoreId: str,
    identityToken: str = ...,
    accessToken: str = ...,
    action: ActionIdentifierTypeDef = ...,  # (1)
    resource: EntityIdentifierTypeDef = ...,  # (2)
    context: ContextDefinitionUnionTypeDef = ...,  # (3)
    entities: EntitiesDefinitionTypeDef = ...,  # (4)
) -> IsAuthorizedWithTokenOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
3. See [:material-code-braces: ContextDefinitionTypeDef](./type_defs.md#contextdefinitiontypedef) [:material-code-braces: ContextDefinitionOutputTypeDef](./type_defs.md#contextdefinitionoutputtypedef) 
4. See [:material-code-braces: EntitiesDefinitionTypeDef](./type_defs.md#entitiesdefinitiontypedef) 
5. See [:material-code-braces: IsAuthorizedWithTokenOutputTypeDef](./type_defs.md#isauthorizedwithtokenoutputtypedef) 


```python
# is_authorized_with_token method usage example with argument unpacking

kwargs: IsAuthorizedWithTokenInputTypeDef = {  # (1)
    "policyStoreId": ...,
}

parent.is_authorized_with_token(**kwargs)
```

1. See [:material-code-braces: IsAuthorizedWithTokenInputTypeDef](./type_defs.md#isauthorizedwithtokeninputtypedef) 

### list\_identity\_sources

Returns a paginated list of all of the identity sources defined in the
specified policy store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").list_identity_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/list_identity_sources.html)

```python
# list_identity_sources method definition

await def list_identity_sources(
    self,
    *,
    policyStoreId: str,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[IdentitySourceFilterTypeDef] = ...,  # (1)
) -> ListIdentitySourcesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IdentitySourceFilterTypeDef](./type_defs.md#identitysourcefiltertypedef) 
2. See [:material-code-braces: ListIdentitySourcesOutputTypeDef](./type_defs.md#listidentitysourcesoutputtypedef) 


```python
# list_identity_sources method usage example with argument unpacking

kwargs: ListIdentitySourcesInputTypeDef = {  # (1)
    "policyStoreId": ...,
}

parent.list_identity_sources(**kwargs)
```

1. See [:material-code-braces: ListIdentitySourcesInputTypeDef](./type_defs.md#listidentitysourcesinputtypedef) 

### list\_policies

Returns a paginated list of all policies stored in the specified policy store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").list_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/list_policies.html)

```python
# list_policies method definition

await def list_policies(
    self,
    *,
    policyStoreId: str,
    nextToken: str = ...,
    maxResults: int = ...,
    filter: PolicyFilterTypeDef = ...,  # (1)
) -> ListPoliciesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PolicyFilterTypeDef](./type_defs.md#policyfiltertypedef) 
2. See [:material-code-braces: ListPoliciesOutputTypeDef](./type_defs.md#listpoliciesoutputtypedef) 


```python
# list_policies method usage example with argument unpacking

kwargs: ListPoliciesInputTypeDef = {  # (1)
    "policyStoreId": ...,
}

parent.list_policies(**kwargs)
```

1. See [:material-code-braces: ListPoliciesInputTypeDef](./type_defs.md#listpoliciesinputtypedef) 

### list\_policy\_stores

Returns a paginated list of all policy stores in the calling Amazon Web
Services account.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").list_policy_stores` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/list_policy_stores.html)

```python
# list_policy_stores method definition

await def list_policy_stores(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPolicyStoresOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPolicyStoresOutputTypeDef](./type_defs.md#listpolicystoresoutputtypedef) 


```python
# list_policy_stores method usage example with argument unpacking

kwargs: ListPolicyStoresInputTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_policy_stores(**kwargs)
```

1. See [:material-code-braces: ListPolicyStoresInputTypeDef](./type_defs.md#listpolicystoresinputtypedef) 

### list\_policy\_templates

Returns a paginated list of all policy templates in the specified policy store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").list_policy_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/list_policy_templates.html)

```python
# list_policy_templates method definition

await def list_policy_templates(
    self,
    *,
    policyStoreId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPolicyTemplatesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPolicyTemplatesOutputTypeDef](./type_defs.md#listpolicytemplatesoutputtypedef) 


```python
# list_policy_templates method usage example with argument unpacking

kwargs: ListPolicyTemplatesInputTypeDef = {  # (1)
    "policyStoreId": ...,
}

parent.list_policy_templates(**kwargs)
```

1. See [:material-code-braces: ListPolicyTemplatesInputTypeDef](./type_defs.md#listpolicytemplatesinputtypedef) 

### put\_schema

Creates or updates the policy schema in the specified policy store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").put_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/put_schema.html)

```python
# put_schema method definition

await def put_schema(
    self,
    *,
    policyStoreId: str,
    definition: SchemaDefinitionTypeDef,  # (1)
) -> PutSchemaOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef) 
2. See [:material-code-braces: PutSchemaOutputTypeDef](./type_defs.md#putschemaoutputtypedef) 


```python
# put_schema method usage example with argument unpacking

kwargs: PutSchemaInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "definition": ...,
}

parent.put_schema(**kwargs)
```

1. See [:material-code-braces: PutSchemaInputTypeDef](./type_defs.md#putschemainputtypedef) 

### update\_identity\_source

Updates the specified identity source to use a new identity provider (IdP), or
to change the mapping of identities from the IdP to a different principal
entity type.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").update_identity_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/update_identity_source.html)

```python
# update_identity_source method definition

await def update_identity_source(
    self,
    *,
    policyStoreId: str,
    identitySourceId: str,
    updateConfiguration: UpdateConfigurationTypeDef,  # (1)
    principalEntityType: str = ...,
) -> UpdateIdentitySourceOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateConfigurationTypeDef](./type_defs.md#updateconfigurationtypedef) 
2. See [:material-code-braces: UpdateIdentitySourceOutputTypeDef](./type_defs.md#updateidentitysourceoutputtypedef) 


```python
# update_identity_source method usage example with argument unpacking

kwargs: UpdateIdentitySourceInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "identitySourceId": ...,
    "updateConfiguration": ...,
}

parent.update_identity_source(**kwargs)
```

1. See [:material-code-braces: UpdateIdentitySourceInputTypeDef](./type_defs.md#updateidentitysourceinputtypedef) 

### update\_policy

Modifies a Cedar static policy in the specified policy store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").update_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/update_policy.html)

```python
# update_policy method definition

await def update_policy(
    self,
    *,
    policyStoreId: str,
    policyId: str,
    definition: UpdatePolicyDefinitionTypeDef,  # (1)
) -> UpdatePolicyOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdatePolicyDefinitionTypeDef](./type_defs.md#updatepolicydefinitiontypedef) 
2. See [:material-code-braces: UpdatePolicyOutputTypeDef](./type_defs.md#updatepolicyoutputtypedef) 


```python
# update_policy method usage example with argument unpacking

kwargs: UpdatePolicyInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "policyId": ...,
    "definition": ...,
}

parent.update_policy(**kwargs)
```

1. See [:material-code-braces: UpdatePolicyInputTypeDef](./type_defs.md#updatepolicyinputtypedef) 

### update\_policy\_store

Modifies the validation setting for a policy store.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").update_policy_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/update_policy_store.html)

```python
# update_policy_store method definition

await def update_policy_store(
    self,
    *,
    policyStoreId: str,
    validationSettings: ValidationSettingsTypeDef,  # (1)
    description: str = ...,
) -> UpdatePolicyStoreOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ValidationSettingsTypeDef](./type_defs.md#validationsettingstypedef) 
2. See [:material-code-braces: UpdatePolicyStoreOutputTypeDef](./type_defs.md#updatepolicystoreoutputtypedef) 


```python
# update_policy_store method usage example with argument unpacking

kwargs: UpdatePolicyStoreInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "validationSettings": ...,
}

parent.update_policy_store(**kwargs)
```

1. See [:material-code-braces: UpdatePolicyStoreInputTypeDef](./type_defs.md#updatepolicystoreinputtypedef) 

### update\_policy\_template

Updates the specified policy template.

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").update_policy_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions/client/update_policy_template.html)

```python
# update_policy_template method definition

await def update_policy_template(
    self,
    *,
    policyStoreId: str,
    policyTemplateId: str,
    statement: str,
    description: str = ...,
) -> UpdatePolicyTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdatePolicyTemplateOutputTypeDef](./type_defs.md#updatepolicytemplateoutputtypedef) 


```python
# update_policy_template method usage example with argument unpacking

kwargs: UpdatePolicyTemplateInputTypeDef = {  # (1)
    "policyStoreId": ...,
    "policyTemplateId": ...,
    "statement": ...,
}

parent.update_policy_template(**kwargs)
```

1. See [:material-code-braces: UpdatePolicyTemplateInputTypeDef](./type_defs.md#updatepolicytemplateinputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("verifiedpermissions").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("verifiedpermissions").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("verifiedpermissions").get_paginator` method with overloads.

- `client.get_paginator("list_identity_sources")` -> [ListIdentitySourcesPaginator](./paginators.md#listidentitysourcespaginator)
- `client.get_paginator("list_policies")` -> [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
- `client.get_paginator("list_policy_stores")` -> [ListPolicyStoresPaginator](./paginators.md#listpolicystorespaginator)
- `client.get_paginator("list_policy_templates")` -> [ListPolicyTemplatesPaginator](./paginators.md#listpolicytemplatespaginator)



