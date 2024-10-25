# Type definitions

> [Index](../README.md) > [VerifiedPermissions](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [VerifiedPermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
    type annotations stubs module [types-aiobotocore-verifiedpermissions](https://pypi.org/project/types-aiobotocore-verifiedpermissions/).

## AttributeValueUnionTypeDef

```python
# AttributeValueUnionTypeDef definition

AttributeValueUnionTypeDef = Union[
    AttributeValueTypeDef,  # (1)
    AttributeValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 

## ContextDefinitionUnionTypeDef

```python
# ContextDefinitionUnionTypeDef definition

ContextDefinitionUnionTypeDef = Union[
    ContextDefinitionTypeDef,  # (1)
    ContextDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ContextDefinitionTypeDef](./type_defs.md#contextdefinitiontypedef) 
2. See [:material-code-braces: ContextDefinitionOutputTypeDef](./type_defs.md#contextdefinitionoutputtypedef) 

## BatchIsAuthorizedInputItemUnionTypeDef

```python
# BatchIsAuthorizedInputItemUnionTypeDef definition

BatchIsAuthorizedInputItemUnionTypeDef = Union[
    BatchIsAuthorizedInputItemTypeDef,  # (1)
    BatchIsAuthorizedInputItemOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BatchIsAuthorizedInputItemTypeDef](./type_defs.md#batchisauthorizedinputitemtypedef) 
2. See [:material-code-braces: BatchIsAuthorizedInputItemOutputTypeDef](./type_defs.md#batchisauthorizedinputitemoutputtypedef) 

## BatchIsAuthorizedWithTokenInputItemUnionTypeDef

```python
# BatchIsAuthorizedWithTokenInputItemUnionTypeDef definition

BatchIsAuthorizedWithTokenInputItemUnionTypeDef = Union[
    BatchIsAuthorizedWithTokenInputItemTypeDef,  # (1)
    BatchIsAuthorizedWithTokenInputItemOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BatchIsAuthorizedWithTokenInputItemTypeDef](./type_defs.md#batchisauthorizedwithtokeninputitemtypedef) 
2. See [:material-code-braces: BatchIsAuthorizedWithTokenInputItemOutputTypeDef](./type_defs.md#batchisauthorizedwithtokeninputitemoutputtypedef) 



## ActionIdentifierTypeDef

```python
# ActionIdentifierTypeDef definition

class ActionIdentifierTypeDef(TypedDict):
    actionType: str,
    actionId: str,
```

## EntityIdentifierTypeDef

```python
# EntityIdentifierTypeDef definition

class EntityIdentifierTypeDef(TypedDict):
    entityType: str,
    entityId: str,
```

## DeterminingPolicyItemTypeDef

```python
# DeterminingPolicyItemTypeDef definition

class DeterminingPolicyItemTypeDef(TypedDict):
    policyId: str,
```

## EvaluationErrorItemTypeDef

```python
# EvaluationErrorItemTypeDef definition

class EvaluationErrorItemTypeDef(TypedDict):
    errorDescription: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## CognitoGroupConfigurationDetailTypeDef

```python
# CognitoGroupConfigurationDetailTypeDef definition

class CognitoGroupConfigurationDetailTypeDef(TypedDict):
    groupEntityType: NotRequired[str],
```

## CognitoGroupConfigurationItemTypeDef

```python
# CognitoGroupConfigurationItemTypeDef definition

class CognitoGroupConfigurationItemTypeDef(TypedDict):
    groupEntityType: NotRequired[str],
```

## CognitoGroupConfigurationTypeDef

```python
# CognitoGroupConfigurationTypeDef definition

class CognitoGroupConfigurationTypeDef(TypedDict):
    groupEntityType: str,
```

## ValidationSettingsTypeDef

```python
# ValidationSettingsTypeDef definition

class ValidationSettingsTypeDef(TypedDict):
    mode: ValidationModeType,  # (1)
```

1. See [:material-code-brackets: ValidationModeType](./literals.md#validationmodetype) 
## CreatePolicyTemplateInputRequestTypeDef

```python
# CreatePolicyTemplateInputRequestTypeDef definition

class CreatePolicyTemplateInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    statement: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

## DeleteIdentitySourceInputRequestTypeDef

```python
# DeleteIdentitySourceInputRequestTypeDef definition

class DeleteIdentitySourceInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    identitySourceId: str,
```

## DeletePolicyInputRequestTypeDef

```python
# DeletePolicyInputRequestTypeDef definition

class DeletePolicyInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    policyId: str,
```

## DeletePolicyStoreInputRequestTypeDef

```python
# DeletePolicyStoreInputRequestTypeDef definition

class DeletePolicyStoreInputRequestTypeDef(TypedDict):
    policyStoreId: str,
```

## DeletePolicyTemplateInputRequestTypeDef

```python
# DeletePolicyTemplateInputRequestTypeDef definition

class DeletePolicyTemplateInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    policyTemplateId: str,
```

## GetIdentitySourceInputRequestTypeDef

```python
# GetIdentitySourceInputRequestTypeDef definition

class GetIdentitySourceInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    identitySourceId: str,
```

## IdentitySourceDetailsTypeDef

```python
# IdentitySourceDetailsTypeDef definition

class IdentitySourceDetailsTypeDef(TypedDict):
    clientIds: NotRequired[List[str]],
    userPoolArn: NotRequired[str],
    discoveryUrl: NotRequired[str],
    openIdIssuer: NotRequired[OpenIdIssuerType],  # (1)
```

1. See [:material-code-brackets: OpenIdIssuerType](./literals.md#openidissuertype) 
## GetPolicyInputRequestTypeDef

```python
# GetPolicyInputRequestTypeDef definition

class GetPolicyInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    policyId: str,
```

## GetPolicyStoreInputRequestTypeDef

```python
# GetPolicyStoreInputRequestTypeDef definition

class GetPolicyStoreInputRequestTypeDef(TypedDict):
    policyStoreId: str,
```

## GetPolicyTemplateInputRequestTypeDef

```python
# GetPolicyTemplateInputRequestTypeDef definition

class GetPolicyTemplateInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    policyTemplateId: str,
```

## GetSchemaInputRequestTypeDef

```python
# GetSchemaInputRequestTypeDef definition

class GetSchemaInputRequestTypeDef(TypedDict):
    policyStoreId: str,
```

## IdentitySourceFilterTypeDef

```python
# IdentitySourceFilterTypeDef definition

class IdentitySourceFilterTypeDef(TypedDict):
    principalEntityType: NotRequired[str],
```

## IdentitySourceItemDetailsTypeDef

```python
# IdentitySourceItemDetailsTypeDef definition

class IdentitySourceItemDetailsTypeDef(TypedDict):
    clientIds: NotRequired[List[str]],
    userPoolArn: NotRequired[str],
    discoveryUrl: NotRequired[str],
    openIdIssuer: NotRequired[OpenIdIssuerType],  # (1)
```

1. See [:material-code-brackets: OpenIdIssuerType](./literals.md#openidissuertype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListPolicyStoresInputRequestTypeDef

```python
# ListPolicyStoresInputRequestTypeDef definition

class ListPolicyStoresInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PolicyStoreItemTypeDef

```python
# PolicyStoreItemTypeDef definition

class PolicyStoreItemTypeDef(TypedDict):
    policyStoreId: str,
    arn: str,
    createdDate: datetime,
    lastUpdatedDate: NotRequired[datetime],
    description: NotRequired[str],
```

## ListPolicyTemplatesInputRequestTypeDef

```python
# ListPolicyTemplatesInputRequestTypeDef definition

class ListPolicyTemplatesInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PolicyTemplateItemTypeDef

```python
# PolicyTemplateItemTypeDef definition

class PolicyTemplateItemTypeDef(TypedDict):
    policyStoreId: str,
    policyTemplateId: str,
    createdDate: datetime,
    lastUpdatedDate: datetime,
    description: NotRequired[str],
```

## OpenIdConnectAccessTokenConfigurationDetailTypeDef

```python
# OpenIdConnectAccessTokenConfigurationDetailTypeDef definition

class OpenIdConnectAccessTokenConfigurationDetailTypeDef(TypedDict):
    principalIdClaim: NotRequired[str],
    audiences: NotRequired[List[str]],
```

## OpenIdConnectAccessTokenConfigurationItemTypeDef

```python
# OpenIdConnectAccessTokenConfigurationItemTypeDef definition

class OpenIdConnectAccessTokenConfigurationItemTypeDef(TypedDict):
    principalIdClaim: NotRequired[str],
    audiences: NotRequired[List[str]],
```

## OpenIdConnectAccessTokenConfigurationTypeDef

```python
# OpenIdConnectAccessTokenConfigurationTypeDef definition

class OpenIdConnectAccessTokenConfigurationTypeDef(TypedDict):
    principalIdClaim: NotRequired[str],
    audiences: NotRequired[Sequence[str]],
```

## OpenIdConnectGroupConfigurationDetailTypeDef

```python
# OpenIdConnectGroupConfigurationDetailTypeDef definition

class OpenIdConnectGroupConfigurationDetailTypeDef(TypedDict):
    groupClaim: str,
    groupEntityType: str,
```

## OpenIdConnectGroupConfigurationItemTypeDef

```python
# OpenIdConnectGroupConfigurationItemTypeDef definition

class OpenIdConnectGroupConfigurationItemTypeDef(TypedDict):
    groupClaim: str,
    groupEntityType: str,
```

## OpenIdConnectGroupConfigurationTypeDef

```python
# OpenIdConnectGroupConfigurationTypeDef definition

class OpenIdConnectGroupConfigurationTypeDef(TypedDict):
    groupClaim: str,
    groupEntityType: str,
```

## OpenIdConnectIdentityTokenConfigurationDetailTypeDef

```python
# OpenIdConnectIdentityTokenConfigurationDetailTypeDef definition

class OpenIdConnectIdentityTokenConfigurationDetailTypeDef(TypedDict):
    principalIdClaim: NotRequired[str],
    clientIds: NotRequired[List[str]],
```

## OpenIdConnectIdentityTokenConfigurationItemTypeDef

```python
# OpenIdConnectIdentityTokenConfigurationItemTypeDef definition

class OpenIdConnectIdentityTokenConfigurationItemTypeDef(TypedDict):
    principalIdClaim: NotRequired[str],
    clientIds: NotRequired[List[str]],
```

## OpenIdConnectIdentityTokenConfigurationTypeDef

```python
# OpenIdConnectIdentityTokenConfigurationTypeDef definition

class OpenIdConnectIdentityTokenConfigurationTypeDef(TypedDict):
    principalIdClaim: NotRequired[str],
    clientIds: NotRequired[Sequence[str]],
```

## StaticPolicyDefinitionDetailTypeDef

```python
# StaticPolicyDefinitionDetailTypeDef definition

class StaticPolicyDefinitionDetailTypeDef(TypedDict):
    statement: str,
    description: NotRequired[str],
```

## StaticPolicyDefinitionItemTypeDef

```python
# StaticPolicyDefinitionItemTypeDef definition

class StaticPolicyDefinitionItemTypeDef(TypedDict):
    description: NotRequired[str],
```

## StaticPolicyDefinitionTypeDef

```python
# StaticPolicyDefinitionTypeDef definition

class StaticPolicyDefinitionTypeDef(TypedDict):
    statement: str,
    description: NotRequired[str],
```

## SchemaDefinitionTypeDef

```python
# SchemaDefinitionTypeDef definition

class SchemaDefinitionTypeDef(TypedDict):
    cedarJson: NotRequired[str],
```

## UpdateCognitoGroupConfigurationTypeDef

```python
# UpdateCognitoGroupConfigurationTypeDef definition

class UpdateCognitoGroupConfigurationTypeDef(TypedDict):
    groupEntityType: str,
```

## UpdateOpenIdConnectAccessTokenConfigurationTypeDef

```python
# UpdateOpenIdConnectAccessTokenConfigurationTypeDef definition

class UpdateOpenIdConnectAccessTokenConfigurationTypeDef(TypedDict):
    principalIdClaim: NotRequired[str],
    audiences: NotRequired[Sequence[str]],
```

## UpdateOpenIdConnectGroupConfigurationTypeDef

```python
# UpdateOpenIdConnectGroupConfigurationTypeDef definition

class UpdateOpenIdConnectGroupConfigurationTypeDef(TypedDict):
    groupClaim: str,
    groupEntityType: str,
```

## UpdateOpenIdConnectIdentityTokenConfigurationTypeDef

```python
# UpdateOpenIdConnectIdentityTokenConfigurationTypeDef definition

class UpdateOpenIdConnectIdentityTokenConfigurationTypeDef(TypedDict):
    principalIdClaim: NotRequired[str],
    clientIds: NotRequired[Sequence[str]],
```

## UpdateStaticPolicyDefinitionTypeDef

```python
# UpdateStaticPolicyDefinitionTypeDef definition

class UpdateStaticPolicyDefinitionTypeDef(TypedDict):
    statement: str,
    description: NotRequired[str],
```

## UpdatePolicyTemplateInputRequestTypeDef

```python
# UpdatePolicyTemplateInputRequestTypeDef definition

class UpdatePolicyTemplateInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    policyTemplateId: str,
    statement: str,
    description: NotRequired[str],
```

## AttributeValueOutputTypeDef

```python
# AttributeValueOutputTypeDef definition

class AttributeValueOutputTypeDef(TypedDict):
    boolean: NotRequired[bool],
    entityIdentifier: NotRequired[EntityIdentifierTypeDef],  # (1)
    long: NotRequired[int],
    string: NotRequired[str],
    set: NotRequired[List[Dict[str, Any]]],
    record: NotRequired[Dict[str, Dict[str, Any]]],
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
## AttributeValueTypeDef

```python
# AttributeValueTypeDef definition

class AttributeValueTypeDef(TypedDict):
    boolean: NotRequired[bool],
    entityIdentifier: NotRequired[EntityIdentifierTypeDef],  # (1)
    long: NotRequired[int],
    string: NotRequired[str],
    set: NotRequired[Sequence[Mapping[str, Any]]],
    record: NotRequired[Mapping[str, Mapping[str, Any]]],
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
## EntityReferenceTypeDef

```python
# EntityReferenceTypeDef definition

class EntityReferenceTypeDef(TypedDict):
    unspecified: NotRequired[bool],
    identifier: NotRequired[EntityIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
## TemplateLinkedPolicyDefinitionDetailTypeDef

```python
# TemplateLinkedPolicyDefinitionDetailTypeDef definition

class TemplateLinkedPolicyDefinitionDetailTypeDef(TypedDict):
    policyTemplateId: str,
    principal: NotRequired[EntityIdentifierTypeDef],  # (1)
    resource: NotRequired[EntityIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
## TemplateLinkedPolicyDefinitionItemTypeDef

```python
# TemplateLinkedPolicyDefinitionItemTypeDef definition

class TemplateLinkedPolicyDefinitionItemTypeDef(TypedDict):
    policyTemplateId: str,
    principal: NotRequired[EntityIdentifierTypeDef],  # (1)
    resource: NotRequired[EntityIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
## TemplateLinkedPolicyDefinitionTypeDef

```python
# TemplateLinkedPolicyDefinitionTypeDef definition

class TemplateLinkedPolicyDefinitionTypeDef(TypedDict):
    policyTemplateId: str,
    principal: NotRequired[EntityIdentifierTypeDef],  # (1)
    resource: NotRequired[EntityIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
## CreateIdentitySourceOutputTypeDef

```python
# CreateIdentitySourceOutputTypeDef definition

class CreateIdentitySourceOutputTypeDef(TypedDict):
    createdDate: datetime,
    identitySourceId: str,
    lastUpdatedDate: datetime,
    policyStoreId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePolicyOutputTypeDef

```python
# CreatePolicyOutputTypeDef definition

class CreatePolicyOutputTypeDef(TypedDict):
    policyStoreId: str,
    policyId: str,
    policyType: PolicyTypeType,  # (1)
    principal: EntityIdentifierTypeDef,  # (2)
    resource: EntityIdentifierTypeDef,  # (2)
    actions: List[ActionIdentifierTypeDef],  # (4)
    createdDate: datetime,
    lastUpdatedDate: datetime,
    effect: PolicyEffectType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
4. See [:material-code-braces: ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef) 
5. See [:material-code-brackets: PolicyEffectType](./literals.md#policyeffecttype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePolicyStoreOutputTypeDef

```python
# CreatePolicyStoreOutputTypeDef definition

class CreatePolicyStoreOutputTypeDef(TypedDict):
    policyStoreId: str,
    arn: str,
    createdDate: datetime,
    lastUpdatedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePolicyTemplateOutputTypeDef

```python
# CreatePolicyTemplateOutputTypeDef definition

class CreatePolicyTemplateOutputTypeDef(TypedDict):
    policyStoreId: str,
    policyTemplateId: str,
    createdDate: datetime,
    lastUpdatedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPolicyTemplateOutputTypeDef

```python
# GetPolicyTemplateOutputTypeDef definition

class GetPolicyTemplateOutputTypeDef(TypedDict):
    policyStoreId: str,
    policyTemplateId: str,
    description: str,
    statement: str,
    createdDate: datetime,
    lastUpdatedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaOutputTypeDef

```python
# GetSchemaOutputTypeDef definition

class GetSchemaOutputTypeDef(TypedDict):
    policyStoreId: str,
    schema: str,
    createdDate: datetime,
    lastUpdatedDate: datetime,
    namespaces: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IsAuthorizedOutputTypeDef

```python
# IsAuthorizedOutputTypeDef definition

class IsAuthorizedOutputTypeDef(TypedDict):
    decision: DecisionType,  # (1)
    determiningPolicies: List[DeterminingPolicyItemTypeDef],  # (2)
    errors: List[EvaluationErrorItemTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: DecisionType](./literals.md#decisiontype) 
2. See [:material-code-braces: DeterminingPolicyItemTypeDef](./type_defs.md#determiningpolicyitemtypedef) 
3. See [:material-code-braces: EvaluationErrorItemTypeDef](./type_defs.md#evaluationerroritemtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IsAuthorizedWithTokenOutputTypeDef

```python
# IsAuthorizedWithTokenOutputTypeDef definition

class IsAuthorizedWithTokenOutputTypeDef(TypedDict):
    decision: DecisionType,  # (1)
    determiningPolicies: List[DeterminingPolicyItemTypeDef],  # (2)
    errors: List[EvaluationErrorItemTypeDef],  # (3)
    principal: EntityIdentifierTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: DecisionType](./literals.md#decisiontype) 
2. See [:material-code-braces: DeterminingPolicyItemTypeDef](./type_defs.md#determiningpolicyitemtypedef) 
3. See [:material-code-braces: EvaluationErrorItemTypeDef](./type_defs.md#evaluationerroritemtypedef) 
4. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSchemaOutputTypeDef

```python
# PutSchemaOutputTypeDef definition

class PutSchemaOutputTypeDef(TypedDict):
    policyStoreId: str,
    namespaces: List[str],
    createdDate: datetime,
    lastUpdatedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIdentitySourceOutputTypeDef

```python
# UpdateIdentitySourceOutputTypeDef definition

class UpdateIdentitySourceOutputTypeDef(TypedDict):
    createdDate: datetime,
    identitySourceId: str,
    lastUpdatedDate: datetime,
    policyStoreId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePolicyOutputTypeDef

```python
# UpdatePolicyOutputTypeDef definition

class UpdatePolicyOutputTypeDef(TypedDict):
    policyStoreId: str,
    policyId: str,
    policyType: PolicyTypeType,  # (1)
    principal: EntityIdentifierTypeDef,  # (2)
    resource: EntityIdentifierTypeDef,  # (2)
    actions: List[ActionIdentifierTypeDef],  # (4)
    createdDate: datetime,
    lastUpdatedDate: datetime,
    effect: PolicyEffectType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
4. See [:material-code-braces: ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef) 
5. See [:material-code-brackets: PolicyEffectType](./literals.md#policyeffecttype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePolicyStoreOutputTypeDef

```python
# UpdatePolicyStoreOutputTypeDef definition

class UpdatePolicyStoreOutputTypeDef(TypedDict):
    policyStoreId: str,
    arn: str,
    createdDate: datetime,
    lastUpdatedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePolicyTemplateOutputTypeDef

```python
# UpdatePolicyTemplateOutputTypeDef definition

class UpdatePolicyTemplateOutputTypeDef(TypedDict):
    policyStoreId: str,
    policyTemplateId: str,
    createdDate: datetime,
    lastUpdatedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CognitoUserPoolConfigurationDetailTypeDef

```python
# CognitoUserPoolConfigurationDetailTypeDef definition

class CognitoUserPoolConfigurationDetailTypeDef(TypedDict):
    userPoolArn: str,
    clientIds: List[str],
    issuer: str,
    groupConfiguration: NotRequired[CognitoGroupConfigurationDetailTypeDef],  # (1)
```

1. See [:material-code-braces: CognitoGroupConfigurationDetailTypeDef](./type_defs.md#cognitogroupconfigurationdetailtypedef) 
## CognitoUserPoolConfigurationItemTypeDef

```python
# CognitoUserPoolConfigurationItemTypeDef definition

class CognitoUserPoolConfigurationItemTypeDef(TypedDict):
    userPoolArn: str,
    clientIds: List[str],
    issuer: str,
    groupConfiguration: NotRequired[CognitoGroupConfigurationItemTypeDef],  # (1)
```

1. See [:material-code-braces: CognitoGroupConfigurationItemTypeDef](./type_defs.md#cognitogroupconfigurationitemtypedef) 
## CognitoUserPoolConfigurationTypeDef

```python
# CognitoUserPoolConfigurationTypeDef definition

class CognitoUserPoolConfigurationTypeDef(TypedDict):
    userPoolArn: str,
    clientIds: NotRequired[Sequence[str]],
    groupConfiguration: NotRequired[CognitoGroupConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CognitoGroupConfigurationTypeDef](./type_defs.md#cognitogroupconfigurationtypedef) 
## CreatePolicyStoreInputRequestTypeDef

```python
# CreatePolicyStoreInputRequestTypeDef definition

class CreatePolicyStoreInputRequestTypeDef(TypedDict):
    validationSettings: ValidationSettingsTypeDef,  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

1. See [:material-code-braces: ValidationSettingsTypeDef](./type_defs.md#validationsettingstypedef) 
## GetPolicyStoreOutputTypeDef

```python
# GetPolicyStoreOutputTypeDef definition

class GetPolicyStoreOutputTypeDef(TypedDict):
    policyStoreId: str,
    arn: str,
    validationSettings: ValidationSettingsTypeDef,  # (1)
    createdDate: datetime,
    lastUpdatedDate: datetime,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValidationSettingsTypeDef](./type_defs.md#validationsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePolicyStoreInputRequestTypeDef

```python
# UpdatePolicyStoreInputRequestTypeDef definition

class UpdatePolicyStoreInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    validationSettings: ValidationSettingsTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: ValidationSettingsTypeDef](./type_defs.md#validationsettingstypedef) 
## ListIdentitySourcesInputRequestTypeDef

```python
# ListIdentitySourcesInputRequestTypeDef definition

class ListIdentitySourcesInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[IdentitySourceFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: IdentitySourceFilterTypeDef](./type_defs.md#identitysourcefiltertypedef) 
## ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef

```python
# ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef definition

class ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef(TypedDict):
    policyStoreId: str,
    filters: NotRequired[Sequence[IdentitySourceFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: IdentitySourceFilterTypeDef](./type_defs.md#identitysourcefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPolicyStoresInputListPolicyStoresPaginateTypeDef

```python
# ListPolicyStoresInputListPolicyStoresPaginateTypeDef definition

class ListPolicyStoresInputListPolicyStoresPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef

```python
# ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef definition

class ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef(TypedDict):
    policyStoreId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPolicyStoresOutputTypeDef

```python
# ListPolicyStoresOutputTypeDef definition

class ListPolicyStoresOutputTypeDef(TypedDict):
    policyStores: List[PolicyStoreItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PolicyStoreItemTypeDef](./type_defs.md#policystoreitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPolicyTemplatesOutputTypeDef

```python
# ListPolicyTemplatesOutputTypeDef definition

class ListPolicyTemplatesOutputTypeDef(TypedDict):
    policyTemplates: List[PolicyTemplateItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PolicyTemplateItemTypeDef](./type_defs.md#policytemplateitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OpenIdConnectTokenSelectionDetailTypeDef

```python
# OpenIdConnectTokenSelectionDetailTypeDef definition

class OpenIdConnectTokenSelectionDetailTypeDef(TypedDict):
    accessTokenOnly: NotRequired[OpenIdConnectAccessTokenConfigurationDetailTypeDef],  # (1)
    identityTokenOnly: NotRequired[OpenIdConnectIdentityTokenConfigurationDetailTypeDef],  # (2)
```

1. See [:material-code-braces: OpenIdConnectAccessTokenConfigurationDetailTypeDef](./type_defs.md#openidconnectaccesstokenconfigurationdetailtypedef) 
2. See [:material-code-braces: OpenIdConnectIdentityTokenConfigurationDetailTypeDef](./type_defs.md#openidconnectidentitytokenconfigurationdetailtypedef) 
## OpenIdConnectTokenSelectionItemTypeDef

```python
# OpenIdConnectTokenSelectionItemTypeDef definition

class OpenIdConnectTokenSelectionItemTypeDef(TypedDict):
    accessTokenOnly: NotRequired[OpenIdConnectAccessTokenConfigurationItemTypeDef],  # (1)
    identityTokenOnly: NotRequired[OpenIdConnectIdentityTokenConfigurationItemTypeDef],  # (2)
```

1. See [:material-code-braces: OpenIdConnectAccessTokenConfigurationItemTypeDef](./type_defs.md#openidconnectaccesstokenconfigurationitemtypedef) 
2. See [:material-code-braces: OpenIdConnectIdentityTokenConfigurationItemTypeDef](./type_defs.md#openidconnectidentitytokenconfigurationitemtypedef) 
## OpenIdConnectTokenSelectionTypeDef

```python
# OpenIdConnectTokenSelectionTypeDef definition

class OpenIdConnectTokenSelectionTypeDef(TypedDict):
    accessTokenOnly: NotRequired[OpenIdConnectAccessTokenConfigurationTypeDef],  # (1)
    identityTokenOnly: NotRequired[OpenIdConnectIdentityTokenConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: OpenIdConnectAccessTokenConfigurationTypeDef](./type_defs.md#openidconnectaccesstokenconfigurationtypedef) 
2. See [:material-code-braces: OpenIdConnectIdentityTokenConfigurationTypeDef](./type_defs.md#openidconnectidentitytokenconfigurationtypedef) 
## PutSchemaInputRequestTypeDef

```python
# PutSchemaInputRequestTypeDef definition

class PutSchemaInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    definition: SchemaDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef) 
## UpdateCognitoUserPoolConfigurationTypeDef

```python
# UpdateCognitoUserPoolConfigurationTypeDef definition

class UpdateCognitoUserPoolConfigurationTypeDef(TypedDict):
    userPoolArn: str,
    clientIds: NotRequired[Sequence[str]],
    groupConfiguration: NotRequired[UpdateCognitoGroupConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateCognitoGroupConfigurationTypeDef](./type_defs.md#updatecognitogroupconfigurationtypedef) 
## UpdateOpenIdConnectTokenSelectionTypeDef

```python
# UpdateOpenIdConnectTokenSelectionTypeDef definition

class UpdateOpenIdConnectTokenSelectionTypeDef(TypedDict):
    accessTokenOnly: NotRequired[UpdateOpenIdConnectAccessTokenConfigurationTypeDef],  # (1)
    identityTokenOnly: NotRequired[UpdateOpenIdConnectIdentityTokenConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: UpdateOpenIdConnectAccessTokenConfigurationTypeDef](./type_defs.md#updateopenidconnectaccesstokenconfigurationtypedef) 
2. See [:material-code-braces: UpdateOpenIdConnectIdentityTokenConfigurationTypeDef](./type_defs.md#updateopenidconnectidentitytokenconfigurationtypedef) 
## UpdatePolicyDefinitionTypeDef

```python
# UpdatePolicyDefinitionTypeDef definition

class UpdatePolicyDefinitionTypeDef(TypedDict):
    static: NotRequired[UpdateStaticPolicyDefinitionTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateStaticPolicyDefinitionTypeDef](./type_defs.md#updatestaticpolicydefinitiontypedef) 
## ContextDefinitionOutputTypeDef

```python
# ContextDefinitionOutputTypeDef definition

class ContextDefinitionOutputTypeDef(TypedDict):
    contextMap: NotRequired[Dict[str, AttributeValueOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 
## PolicyFilterTypeDef

```python
# PolicyFilterTypeDef definition

class PolicyFilterTypeDef(TypedDict):
    principal: NotRequired[EntityReferenceTypeDef],  # (1)
    resource: NotRequired[EntityReferenceTypeDef],  # (1)
    policyType: NotRequired[PolicyTypeType],  # (3)
    policyTemplateId: NotRequired[str],
```

1. See [:material-code-braces: EntityReferenceTypeDef](./type_defs.md#entityreferencetypedef) 
2. See [:material-code-braces: EntityReferenceTypeDef](./type_defs.md#entityreferencetypedef) 
3. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
## PolicyDefinitionDetailTypeDef

```python
# PolicyDefinitionDetailTypeDef definition

class PolicyDefinitionDetailTypeDef(TypedDict):
    static: NotRequired[StaticPolicyDefinitionDetailTypeDef],  # (1)
    templateLinked: NotRequired[TemplateLinkedPolicyDefinitionDetailTypeDef],  # (2)
```

1. See [:material-code-braces: StaticPolicyDefinitionDetailTypeDef](./type_defs.md#staticpolicydefinitiondetailtypedef) 
2. See [:material-code-braces: TemplateLinkedPolicyDefinitionDetailTypeDef](./type_defs.md#templatelinkedpolicydefinitiondetailtypedef) 
## PolicyDefinitionItemTypeDef

```python
# PolicyDefinitionItemTypeDef definition

class PolicyDefinitionItemTypeDef(TypedDict):
    static: NotRequired[StaticPolicyDefinitionItemTypeDef],  # (1)
    templateLinked: NotRequired[TemplateLinkedPolicyDefinitionItemTypeDef],  # (2)
```

1. See [:material-code-braces: StaticPolicyDefinitionItemTypeDef](./type_defs.md#staticpolicydefinitionitemtypedef) 
2. See [:material-code-braces: TemplateLinkedPolicyDefinitionItemTypeDef](./type_defs.md#templatelinkedpolicydefinitionitemtypedef) 
## PolicyDefinitionTypeDef

```python
# PolicyDefinitionTypeDef definition

class PolicyDefinitionTypeDef(TypedDict):
    static: NotRequired[StaticPolicyDefinitionTypeDef],  # (1)
    templateLinked: NotRequired[TemplateLinkedPolicyDefinitionTypeDef],  # (2)
```

1. See [:material-code-braces: StaticPolicyDefinitionTypeDef](./type_defs.md#staticpolicydefinitiontypedef) 
2. See [:material-code-braces: TemplateLinkedPolicyDefinitionTypeDef](./type_defs.md#templatelinkedpolicydefinitiontypedef) 
## OpenIdConnectConfigurationDetailTypeDef

```python
# OpenIdConnectConfigurationDetailTypeDef definition

class OpenIdConnectConfigurationDetailTypeDef(TypedDict):
    issuer: str,
    tokenSelection: OpenIdConnectTokenSelectionDetailTypeDef,  # (2)
    entityIdPrefix: NotRequired[str],
    groupConfiguration: NotRequired[OpenIdConnectGroupConfigurationDetailTypeDef],  # (1)
```

1. See [:material-code-braces: OpenIdConnectGroupConfigurationDetailTypeDef](./type_defs.md#openidconnectgroupconfigurationdetailtypedef) 
2. See [:material-code-braces: OpenIdConnectTokenSelectionDetailTypeDef](./type_defs.md#openidconnecttokenselectiondetailtypedef) 
## OpenIdConnectConfigurationItemTypeDef

```python
# OpenIdConnectConfigurationItemTypeDef definition

class OpenIdConnectConfigurationItemTypeDef(TypedDict):
    issuer: str,
    tokenSelection: OpenIdConnectTokenSelectionItemTypeDef,  # (2)
    entityIdPrefix: NotRequired[str],
    groupConfiguration: NotRequired[OpenIdConnectGroupConfigurationItemTypeDef],  # (1)
```

1. See [:material-code-braces: OpenIdConnectGroupConfigurationItemTypeDef](./type_defs.md#openidconnectgroupconfigurationitemtypedef) 
2. See [:material-code-braces: OpenIdConnectTokenSelectionItemTypeDef](./type_defs.md#openidconnecttokenselectionitemtypedef) 
## OpenIdConnectConfigurationTypeDef

```python
# OpenIdConnectConfigurationTypeDef definition

class OpenIdConnectConfigurationTypeDef(TypedDict):
    issuer: str,
    tokenSelection: OpenIdConnectTokenSelectionTypeDef,  # (2)
    entityIdPrefix: NotRequired[str],
    groupConfiguration: NotRequired[OpenIdConnectGroupConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: OpenIdConnectGroupConfigurationTypeDef](./type_defs.md#openidconnectgroupconfigurationtypedef) 
2. See [:material-code-braces: OpenIdConnectTokenSelectionTypeDef](./type_defs.md#openidconnecttokenselectiontypedef) 
## UpdateOpenIdConnectConfigurationTypeDef

```python
# UpdateOpenIdConnectConfigurationTypeDef definition

class UpdateOpenIdConnectConfigurationTypeDef(TypedDict):
    issuer: str,
    tokenSelection: UpdateOpenIdConnectTokenSelectionTypeDef,  # (2)
    entityIdPrefix: NotRequired[str],
    groupConfiguration: NotRequired[UpdateOpenIdConnectGroupConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateOpenIdConnectGroupConfigurationTypeDef](./type_defs.md#updateopenidconnectgroupconfigurationtypedef) 
2. See [:material-code-braces: UpdateOpenIdConnectTokenSelectionTypeDef](./type_defs.md#updateopenidconnecttokenselectiontypedef) 
## UpdatePolicyInputRequestTypeDef

```python
# UpdatePolicyInputRequestTypeDef definition

class UpdatePolicyInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    policyId: str,
    definition: UpdatePolicyDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: UpdatePolicyDefinitionTypeDef](./type_defs.md#updatepolicydefinitiontypedef) 
## BatchIsAuthorizedInputItemOutputTypeDef

```python
# BatchIsAuthorizedInputItemOutputTypeDef definition

class BatchIsAuthorizedInputItemOutputTypeDef(TypedDict):
    principal: NotRequired[EntityIdentifierTypeDef],  # (1)
    action: NotRequired[ActionIdentifierTypeDef],  # (2)
    resource: NotRequired[EntityIdentifierTypeDef],  # (1)
    context: NotRequired[ContextDefinitionOutputTypeDef],  # (4)
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
2. See [:material-code-braces: ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
4. See [:material-code-braces: ContextDefinitionOutputTypeDef](./type_defs.md#contextdefinitionoutputtypedef) 
## BatchIsAuthorizedWithTokenInputItemOutputTypeDef

```python
# BatchIsAuthorizedWithTokenInputItemOutputTypeDef definition

class BatchIsAuthorizedWithTokenInputItemOutputTypeDef(TypedDict):
    action: NotRequired[ActionIdentifierTypeDef],  # (1)
    resource: NotRequired[EntityIdentifierTypeDef],  # (2)
    context: NotRequired[ContextDefinitionOutputTypeDef],  # (3)
```

1. See [:material-code-braces: ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
3. See [:material-code-braces: ContextDefinitionOutputTypeDef](./type_defs.md#contextdefinitionoutputtypedef) 
## ContextDefinitionTypeDef

```python
# ContextDefinitionTypeDef definition

class ContextDefinitionTypeDef(TypedDict):
    contextMap: NotRequired[Mapping[str, AttributeValueUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 
## EntityItemTypeDef

```python
# EntityItemTypeDef definition

class EntityItemTypeDef(TypedDict):
    identifier: EntityIdentifierTypeDef,  # (1)
    attributes: NotRequired[Mapping[str, AttributeValueUnionTypeDef]],  # (2)
    parents: NotRequired[Sequence[EntityIdentifierTypeDef]],  # (3)
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
## ListPoliciesInputListPoliciesPaginateTypeDef

```python
# ListPoliciesInputListPoliciesPaginateTypeDef definition

class ListPoliciesInputListPoliciesPaginateTypeDef(TypedDict):
    policyStoreId: str,
    filter: NotRequired[PolicyFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PolicyFilterTypeDef](./type_defs.md#policyfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPoliciesInputRequestTypeDef

```python
# ListPoliciesInputRequestTypeDef definition

class ListPoliciesInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filter: NotRequired[PolicyFilterTypeDef],  # (1)
```

1. See [:material-code-braces: PolicyFilterTypeDef](./type_defs.md#policyfiltertypedef) 
## GetPolicyOutputTypeDef

```python
# GetPolicyOutputTypeDef definition

class GetPolicyOutputTypeDef(TypedDict):
    policyStoreId: str,
    policyId: str,
    policyType: PolicyTypeType,  # (1)
    principal: EntityIdentifierTypeDef,  # (2)
    resource: EntityIdentifierTypeDef,  # (2)
    actions: List[ActionIdentifierTypeDef],  # (4)
    definition: PolicyDefinitionDetailTypeDef,  # (5)
    createdDate: datetime,
    lastUpdatedDate: datetime,
    effect: PolicyEffectType,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
4. See [:material-code-braces: ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef) 
5. See [:material-code-braces: PolicyDefinitionDetailTypeDef](./type_defs.md#policydefinitiondetailtypedef) 
6. See [:material-code-brackets: PolicyEffectType](./literals.md#policyeffecttype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyItemTypeDef

```python
# PolicyItemTypeDef definition

class PolicyItemTypeDef(TypedDict):
    policyStoreId: str,
    policyId: str,
    policyType: PolicyTypeType,  # (1)
    definition: PolicyDefinitionItemTypeDef,  # (5)
    createdDate: datetime,
    lastUpdatedDate: datetime,
    principal: NotRequired[EntityIdentifierTypeDef],  # (2)
    resource: NotRequired[EntityIdentifierTypeDef],  # (2)
    actions: NotRequired[List[ActionIdentifierTypeDef]],  # (4)
    effect: NotRequired[PolicyEffectType],  # (6)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
4. See [:material-code-braces: ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef) 
5. See [:material-code-braces: PolicyDefinitionItemTypeDef](./type_defs.md#policydefinitionitemtypedef) 
6. See [:material-code-brackets: PolicyEffectType](./literals.md#policyeffecttype) 
## CreatePolicyInputRequestTypeDef

```python
# CreatePolicyInputRequestTypeDef definition

class CreatePolicyInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    definition: PolicyDefinitionTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: PolicyDefinitionTypeDef](./type_defs.md#policydefinitiontypedef) 
## ConfigurationDetailTypeDef

```python
# ConfigurationDetailTypeDef definition

class ConfigurationDetailTypeDef(TypedDict):
    cognitoUserPoolConfiguration: NotRequired[CognitoUserPoolConfigurationDetailTypeDef],  # (1)
    openIdConnectConfiguration: NotRequired[OpenIdConnectConfigurationDetailTypeDef],  # (2)
```

1. See [:material-code-braces: CognitoUserPoolConfigurationDetailTypeDef](./type_defs.md#cognitouserpoolconfigurationdetailtypedef) 
2. See [:material-code-braces: OpenIdConnectConfigurationDetailTypeDef](./type_defs.md#openidconnectconfigurationdetailtypedef) 
## ConfigurationItemTypeDef

```python
# ConfigurationItemTypeDef definition

class ConfigurationItemTypeDef(TypedDict):
    cognitoUserPoolConfiguration: NotRequired[CognitoUserPoolConfigurationItemTypeDef],  # (1)
    openIdConnectConfiguration: NotRequired[OpenIdConnectConfigurationItemTypeDef],  # (2)
```

1. See [:material-code-braces: CognitoUserPoolConfigurationItemTypeDef](./type_defs.md#cognitouserpoolconfigurationitemtypedef) 
2. See [:material-code-braces: OpenIdConnectConfigurationItemTypeDef](./type_defs.md#openidconnectconfigurationitemtypedef) 
## ConfigurationTypeDef

```python
# ConfigurationTypeDef definition

class ConfigurationTypeDef(TypedDict):
    cognitoUserPoolConfiguration: NotRequired[CognitoUserPoolConfigurationTypeDef],  # (1)
    openIdConnectConfiguration: NotRequired[OpenIdConnectConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: CognitoUserPoolConfigurationTypeDef](./type_defs.md#cognitouserpoolconfigurationtypedef) 
2. See [:material-code-braces: OpenIdConnectConfigurationTypeDef](./type_defs.md#openidconnectconfigurationtypedef) 
## UpdateConfigurationTypeDef

```python
# UpdateConfigurationTypeDef definition

class UpdateConfigurationTypeDef(TypedDict):
    cognitoUserPoolConfiguration: NotRequired[UpdateCognitoUserPoolConfigurationTypeDef],  # (1)
    openIdConnectConfiguration: NotRequired[UpdateOpenIdConnectConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: UpdateCognitoUserPoolConfigurationTypeDef](./type_defs.md#updatecognitouserpoolconfigurationtypedef) 
2. See [:material-code-braces: UpdateOpenIdConnectConfigurationTypeDef](./type_defs.md#updateopenidconnectconfigurationtypedef) 
## BatchIsAuthorizedOutputItemTypeDef

```python
# BatchIsAuthorizedOutputItemTypeDef definition

class BatchIsAuthorizedOutputItemTypeDef(TypedDict):
    request: BatchIsAuthorizedInputItemOutputTypeDef,  # (1)
    decision: DecisionType,  # (2)
    determiningPolicies: List[DeterminingPolicyItemTypeDef],  # (3)
    errors: List[EvaluationErrorItemTypeDef],  # (4)
```

1. See [:material-code-braces: BatchIsAuthorizedInputItemOutputTypeDef](./type_defs.md#batchisauthorizedinputitemoutputtypedef) 
2. See [:material-code-brackets: DecisionType](./literals.md#decisiontype) 
3. See [:material-code-braces: DeterminingPolicyItemTypeDef](./type_defs.md#determiningpolicyitemtypedef) 
4. See [:material-code-braces: EvaluationErrorItemTypeDef](./type_defs.md#evaluationerroritemtypedef) 
## BatchIsAuthorizedWithTokenOutputItemTypeDef

```python
# BatchIsAuthorizedWithTokenOutputItemTypeDef definition

class BatchIsAuthorizedWithTokenOutputItemTypeDef(TypedDict):
    request: BatchIsAuthorizedWithTokenInputItemOutputTypeDef,  # (1)
    decision: DecisionType,  # (2)
    determiningPolicies: List[DeterminingPolicyItemTypeDef],  # (3)
    errors: List[EvaluationErrorItemTypeDef],  # (4)
```

1. See [:material-code-braces: BatchIsAuthorizedWithTokenInputItemOutputTypeDef](./type_defs.md#batchisauthorizedwithtokeninputitemoutputtypedef) 
2. See [:material-code-brackets: DecisionType](./literals.md#decisiontype) 
3. See [:material-code-braces: DeterminingPolicyItemTypeDef](./type_defs.md#determiningpolicyitemtypedef) 
4. See [:material-code-braces: EvaluationErrorItemTypeDef](./type_defs.md#evaluationerroritemtypedef) 
## EntitiesDefinitionTypeDef

```python
# EntitiesDefinitionTypeDef definition

class EntitiesDefinitionTypeDef(TypedDict):
    entityList: NotRequired[Sequence[EntityItemTypeDef]],  # (1)
```

1. See [:material-code-braces: EntityItemTypeDef](./type_defs.md#entityitemtypedef) 
## ListPoliciesOutputTypeDef

```python
# ListPoliciesOutputTypeDef definition

class ListPoliciesOutputTypeDef(TypedDict):
    policies: List[PolicyItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PolicyItemTypeDef](./type_defs.md#policyitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdentitySourceOutputTypeDef

```python
# GetIdentitySourceOutputTypeDef definition

class GetIdentitySourceOutputTypeDef(TypedDict):
    createdDate: datetime,
    details: IdentitySourceDetailsTypeDef,  # (1)
    identitySourceId: str,
    lastUpdatedDate: datetime,
    policyStoreId: str,
    principalEntityType: str,
    configuration: ConfigurationDetailTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: IdentitySourceDetailsTypeDef](./type_defs.md#identitysourcedetailstypedef) 
2. See [:material-code-braces: ConfigurationDetailTypeDef](./type_defs.md#configurationdetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IdentitySourceItemTypeDef

```python
# IdentitySourceItemTypeDef definition

class IdentitySourceItemTypeDef(TypedDict):
    createdDate: datetime,
    identitySourceId: str,
    lastUpdatedDate: datetime,
    policyStoreId: str,
    principalEntityType: str,
    details: NotRequired[IdentitySourceItemDetailsTypeDef],  # (1)
    configuration: NotRequired[ConfigurationItemTypeDef],  # (2)
```

1. See [:material-code-braces: IdentitySourceItemDetailsTypeDef](./type_defs.md#identitysourceitemdetailstypedef) 
2. See [:material-code-braces: ConfigurationItemTypeDef](./type_defs.md#configurationitemtypedef) 
## CreateIdentitySourceInputRequestTypeDef

```python
# CreateIdentitySourceInputRequestTypeDef definition

class CreateIdentitySourceInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    configuration: ConfigurationTypeDef,  # (1)
    clientToken: NotRequired[str],
    principalEntityType: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
## UpdateIdentitySourceInputRequestTypeDef

```python
# UpdateIdentitySourceInputRequestTypeDef definition

class UpdateIdentitySourceInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    identitySourceId: str,
    updateConfiguration: UpdateConfigurationTypeDef,  # (1)
    principalEntityType: NotRequired[str],
```

1. See [:material-code-braces: UpdateConfigurationTypeDef](./type_defs.md#updateconfigurationtypedef) 
## BatchIsAuthorizedOutputTypeDef

```python
# BatchIsAuthorizedOutputTypeDef definition

class BatchIsAuthorizedOutputTypeDef(TypedDict):
    results: List[BatchIsAuthorizedOutputItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchIsAuthorizedOutputItemTypeDef](./type_defs.md#batchisauthorizedoutputitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchIsAuthorizedWithTokenOutputTypeDef

```python
# BatchIsAuthorizedWithTokenOutputTypeDef definition

class BatchIsAuthorizedWithTokenOutputTypeDef(TypedDict):
    principal: EntityIdentifierTypeDef,  # (1)
    results: List[BatchIsAuthorizedWithTokenOutputItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
2. See [:material-code-braces: BatchIsAuthorizedWithTokenOutputItemTypeDef](./type_defs.md#batchisauthorizedwithtokenoutputitemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchIsAuthorizedInputItemTypeDef

```python
# BatchIsAuthorizedInputItemTypeDef definition

class BatchIsAuthorizedInputItemTypeDef(TypedDict):
    principal: NotRequired[EntityIdentifierTypeDef],  # (1)
    action: NotRequired[ActionIdentifierTypeDef],  # (2)
    resource: NotRequired[EntityIdentifierTypeDef],  # (1)
    context: NotRequired[ContextDefinitionUnionTypeDef],  # (4)
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
2. See [:material-code-braces: ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
4. See [:material-code-braces: ContextDefinitionTypeDef](./type_defs.md#contextdefinitiontypedef) [:material-code-braces: ContextDefinitionOutputTypeDef](./type_defs.md#contextdefinitionoutputtypedef) 
## BatchIsAuthorizedWithTokenInputItemTypeDef

```python
# BatchIsAuthorizedWithTokenInputItemTypeDef definition

class BatchIsAuthorizedWithTokenInputItemTypeDef(TypedDict):
    action: NotRequired[ActionIdentifierTypeDef],  # (1)
    resource: NotRequired[EntityIdentifierTypeDef],  # (2)
    context: NotRequired[ContextDefinitionUnionTypeDef],  # (3)
```

1. See [:material-code-braces: ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
3. See [:material-code-braces: ContextDefinitionTypeDef](./type_defs.md#contextdefinitiontypedef) [:material-code-braces: ContextDefinitionOutputTypeDef](./type_defs.md#contextdefinitionoutputtypedef) 
## IsAuthorizedInputRequestTypeDef

```python
# IsAuthorizedInputRequestTypeDef definition

class IsAuthorizedInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    principal: NotRequired[EntityIdentifierTypeDef],  # (1)
    action: NotRequired[ActionIdentifierTypeDef],  # (2)
    resource: NotRequired[EntityIdentifierTypeDef],  # (1)
    context: NotRequired[ContextDefinitionTypeDef],  # (4)
    entities: NotRequired[EntitiesDefinitionTypeDef],  # (5)
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
2. See [:material-code-braces: ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
4. See [:material-code-braces: ContextDefinitionTypeDef](./type_defs.md#contextdefinitiontypedef) 
5. See [:material-code-braces: EntitiesDefinitionTypeDef](./type_defs.md#entitiesdefinitiontypedef) 
## IsAuthorizedWithTokenInputRequestTypeDef

```python
# IsAuthorizedWithTokenInputRequestTypeDef definition

class IsAuthorizedWithTokenInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    identityToken: NotRequired[str],
    accessToken: NotRequired[str],
    action: NotRequired[ActionIdentifierTypeDef],  # (1)
    resource: NotRequired[EntityIdentifierTypeDef],  # (2)
    context: NotRequired[ContextDefinitionTypeDef],  # (3)
    entities: NotRequired[EntitiesDefinitionTypeDef],  # (4)
```

1. See [:material-code-braces: ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
3. See [:material-code-braces: ContextDefinitionTypeDef](./type_defs.md#contextdefinitiontypedef) 
4. See [:material-code-braces: EntitiesDefinitionTypeDef](./type_defs.md#entitiesdefinitiontypedef) 
## ListIdentitySourcesOutputTypeDef

```python
# ListIdentitySourcesOutputTypeDef definition

class ListIdentitySourcesOutputTypeDef(TypedDict):
    identitySources: List[IdentitySourceItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IdentitySourceItemTypeDef](./type_defs.md#identitysourceitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchIsAuthorizedInputRequestTypeDef

```python
# BatchIsAuthorizedInputRequestTypeDef definition

class BatchIsAuthorizedInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    requests: Sequence[BatchIsAuthorizedInputItemUnionTypeDef],  # (1)
    entities: NotRequired[EntitiesDefinitionTypeDef],  # (2)
```

1. See [:material-code-braces: BatchIsAuthorizedInputItemTypeDef](./type_defs.md#batchisauthorizedinputitemtypedef) [:material-code-braces: BatchIsAuthorizedInputItemOutputTypeDef](./type_defs.md#batchisauthorizedinputitemoutputtypedef) 
2. See [:material-code-braces: EntitiesDefinitionTypeDef](./type_defs.md#entitiesdefinitiontypedef) 
## BatchIsAuthorizedWithTokenInputRequestTypeDef

```python
# BatchIsAuthorizedWithTokenInputRequestTypeDef definition

class BatchIsAuthorizedWithTokenInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    requests: Sequence[BatchIsAuthorizedWithTokenInputItemUnionTypeDef],  # (1)
    identityToken: NotRequired[str],
    accessToken: NotRequired[str],
    entities: NotRequired[EntitiesDefinitionTypeDef],  # (2)
```

1. See [:material-code-braces: BatchIsAuthorizedWithTokenInputItemTypeDef](./type_defs.md#batchisauthorizedwithtokeninputitemtypedef) [:material-code-braces: BatchIsAuthorizedWithTokenInputItemOutputTypeDef](./type_defs.md#batchisauthorizedwithtokeninputitemoutputtypedef) 
2. See [:material-code-braces: EntitiesDefinitionTypeDef](./type_defs.md#entitiesdefinitiontypedef) 
