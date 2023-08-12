# Type definitions

> [Index](../README.md) > [VerifiedPermissions](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [VerifiedPermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
    type annotations stubs module [types-aiobotocore-verifiedpermissions](https://pypi.org/project/types-aiobotocore-verifiedpermissions/).



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

## CognitoUserPoolConfigurationTypeDef

```python
# CognitoUserPoolConfigurationTypeDef definition

class CognitoUserPoolConfigurationTypeDef(TypedDict):
    userPoolArn: str,
    clientIds: NotRequired[Sequence[str]],
```

## ContextDefinitionTypeDef

```python
# ContextDefinitionTypeDef definition

class ContextDefinitionTypeDef(TypedDict):
    contextMap: NotRequired[Mapping[str, AttributeValueTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
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

## UpdateCognitoUserPoolConfigurationTypeDef

```python
# UpdateCognitoUserPoolConfigurationTypeDef definition

class UpdateCognitoUserPoolConfigurationTypeDef(TypedDict):
    userPoolArn: str,
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

## AttributeValueTypeDef

```python
# AttributeValueTypeDef definition

class AttributeValueTypeDef(TypedDict):
    boolean: NotRequired[bool],
    entityIdentifier: NotRequired[EntityIdentifierTypeDef],  # (1)
    long: NotRequired[int],
    string: NotRequired[str],
    set: NotRequired[Sequence[AttributeValueTypeDef]],  # (2)
    record: NotRequired[Mapping[str, AttributeValueTypeDef]],  # (3)
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## EntityItemTypeDef

```python
# EntityItemTypeDef definition

class EntityItemTypeDef(TypedDict):
    identifier: EntityIdentifierTypeDef,  # (1)
    attributes: NotRequired[Mapping[str, AttributeValueTypeDef]],  # (2)
    parents: NotRequired[Sequence[EntityIdentifierTypeDef]],  # (3)
```

1. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
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
## ConfigurationTypeDef

```python
# ConfigurationTypeDef definition

class ConfigurationTypeDef(TypedDict):
    cognitoUserPoolConfiguration: NotRequired[CognitoUserPoolConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CognitoUserPoolConfigurationTypeDef](./type_defs.md#cognitouserpoolconfigurationtypedef) 
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
    createdDate: datetime,
    lastUpdatedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    createdDate: datetime,
    lastUpdatedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## CreatePolicyStoreInputRequestTypeDef

```python
# CreatePolicyStoreInputRequestTypeDef definition

class CreatePolicyStoreInputRequestTypeDef(TypedDict):
    validationSettings: ValidationSettingsTypeDef,  # (1)
    clientToken: NotRequired[str],
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
```

1. See [:material-code-braces: ValidationSettingsTypeDef](./type_defs.md#validationsettingstypedef) 
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: DecisionType](./literals.md#decisiontype) 
2. See [:material-code-braces: DeterminingPolicyItemTypeDef](./type_defs.md#determiningpolicyitemtypedef) 
3. See [:material-code-braces: EvaluationErrorItemTypeDef](./type_defs.md#evaluationerroritemtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentitySourceDetailsTypeDef](./type_defs.md#identitysourcedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## IdentitySourceItemTypeDef

```python
# IdentitySourceItemTypeDef definition

class IdentitySourceItemTypeDef(TypedDict):
    createdDate: datetime,
    details: IdentitySourceItemDetailsTypeDef,  # (1)
    identitySourceId: str,
    lastUpdatedDate: datetime,
    policyStoreId: str,
    principalEntityType: str,
```

1. See [:material-code-braces: IdentitySourceItemDetailsTypeDef](./type_defs.md#identitysourceitemdetailstypedef) 
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
    nextToken: str,
    policyStores: List[PolicyStoreItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyStoreItemTypeDef](./type_defs.md#policystoreitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPolicyTemplatesOutputTypeDef

```python
# ListPolicyTemplatesOutputTypeDef definition

class ListPolicyTemplatesOutputTypeDef(TypedDict):
    nextToken: str,
    policyTemplates: List[PolicyTemplateItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTemplateItemTypeDef](./type_defs.md#policytemplateitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSchemaInputRequestTypeDef

```python
# PutSchemaInputRequestTypeDef definition

class PutSchemaInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    definition: SchemaDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef) 
## UpdateConfigurationTypeDef

```python
# UpdateConfigurationTypeDef definition

class UpdateConfigurationTypeDef(TypedDict):
    cognitoUserPoolConfiguration: NotRequired[UpdateCognitoUserPoolConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateCognitoUserPoolConfigurationTypeDef](./type_defs.md#updatecognitouserpoolconfigurationtypedef) 
## UpdatePolicyDefinitionTypeDef

```python
# UpdatePolicyDefinitionTypeDef definition

class UpdatePolicyDefinitionTypeDef(TypedDict):
    static: NotRequired[UpdateStaticPolicyDefinitionTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateStaticPolicyDefinitionTypeDef](./type_defs.md#updatestaticpolicydefinitiontypedef) 
## EntitiesDefinitionTypeDef

```python
# EntitiesDefinitionTypeDef definition

class EntitiesDefinitionTypeDef(TypedDict):
    entityList: NotRequired[Sequence[EntityItemTypeDef]],  # (1)
```

1. See [:material-code-braces: EntityItemTypeDef](./type_defs.md#entityitemtypedef) 
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
## ListIdentitySourcesOutputTypeDef

```python
# ListIdentitySourcesOutputTypeDef definition

class ListIdentitySourcesOutputTypeDef(TypedDict):
    nextToken: str,
    identitySources: List[IdentitySourceItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentitySourceItemTypeDef](./type_defs.md#identitysourceitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## UpdatePolicyInputRequestTypeDef

```python
# UpdatePolicyInputRequestTypeDef definition

class UpdatePolicyInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    policyId: str,
    definition: UpdatePolicyDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: UpdatePolicyDefinitionTypeDef](./type_defs.md#updatepolicydefinitiontypedef) 
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
    definition: PolicyDefinitionDetailTypeDef,  # (4)
    createdDate: datetime,
    lastUpdatedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
4. See [:material-code-braces: PolicyDefinitionDetailTypeDef](./type_defs.md#policydefinitiondetailtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyItemTypeDef

```python
# PolicyItemTypeDef definition

class PolicyItemTypeDef(TypedDict):
    policyStoreId: str,
    policyId: str,
    policyType: PolicyTypeType,  # (1)
    definition: PolicyDefinitionItemTypeDef,  # (4)
    createdDate: datetime,
    lastUpdatedDate: datetime,
    principal: NotRequired[EntityIdentifierTypeDef],  # (2)
    resource: NotRequired[EntityIdentifierTypeDef],  # (2)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
3. See [:material-code-braces: EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef) 
4. See [:material-code-braces: PolicyDefinitionItemTypeDef](./type_defs.md#policydefinitionitemtypedef) 
## CreatePolicyInputRequestTypeDef

```python
# CreatePolicyInputRequestTypeDef definition

class CreatePolicyInputRequestTypeDef(TypedDict):
    policyStoreId: str,
    definition: PolicyDefinitionTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: PolicyDefinitionTypeDef](./type_defs.md#policydefinitiontypedef) 
## ListPoliciesOutputTypeDef

```python
# ListPoliciesOutputTypeDef definition

class ListPoliciesOutputTypeDef(TypedDict):
    nextToken: str,
    policies: List[PolicyItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyItemTypeDef](./type_defs.md#policyitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
