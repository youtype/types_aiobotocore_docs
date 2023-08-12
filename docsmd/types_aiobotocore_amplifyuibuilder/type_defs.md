# Type definitions

> [Index](../README.md) > [AmplifyUIBuilder](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AmplifyUIBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
    type annotations stubs module [types-aiobotocore-amplifyuibuilder](https://pypi.org/project/types-aiobotocore-amplifyuibuilder/).



## MutationActionSetStateParameterTypeDef

```python
# MutationActionSetStateParameterTypeDef definition

class MutationActionSetStateParameterTypeDef(TypedDict):
    componentName: str,
    property: str,
    set: ComponentPropertyTypeDef,  # (1)
```

1. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
## GraphQLRenderConfigTypeDef

```python
# GraphQLRenderConfigTypeDef definition

class GraphQLRenderConfigTypeDef(TypedDict):
    typesFilePath: str,
    queriesFilePath: str,
    mutationsFilePath: str,
    subscriptionsFilePath: str,
    fragmentsFilePath: str,
```

## CodegenFeatureFlagsTypeDef

```python
# CodegenFeatureFlagsTypeDef definition

class CodegenFeatureFlagsTypeDef(TypedDict):
    isRelationshipSupported: NotRequired[bool],
    isNonModelSupported: NotRequired[bool],
```

## CodegenGenericDataEnumTypeDef

```python
# CodegenGenericDataEnumTypeDef definition

class CodegenGenericDataEnumTypeDef(TypedDict):
    values: List[str],
```

## CodegenGenericDataRelationshipTypeTypeDef

```python
# CodegenGenericDataRelationshipTypeTypeDef definition

class CodegenGenericDataRelationshipTypeTypeDef(TypedDict):
    type: GenericDataRelationshipTypeType,  # (1)
    relatedModelName: str,
    relatedModelFields: NotRequired[List[str]],
    canUnlinkAssociatedModel: NotRequired[bool],
    relatedJoinFieldName: NotRequired[str],
    relatedJoinTableName: NotRequired[str],
    belongsToFieldOnRelatedModel: NotRequired[str],
    associatedFields: NotRequired[List[str]],
    isHasManyIndex: NotRequired[bool],
```

1. See [:material-code-brackets: GenericDataRelationshipTypeType](./literals.md#genericdatarelationshiptypetype) 
## CodegenJobAssetTypeDef

```python
# CodegenJobAssetTypeDef definition

class CodegenJobAssetTypeDef(TypedDict):
    downloadUrl: NotRequired[str],
```

## CodegenJobSummaryTypeDef

```python
# CodegenJobSummaryTypeDef definition

class CodegenJobSummaryTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
    createdAt: NotRequired[datetime],
    modifiedAt: NotRequired[datetime],
```

## ComponentBindingPropertiesValuePropertiesTypeDef

```python
# ComponentBindingPropertiesValuePropertiesTypeDef definition

class ComponentBindingPropertiesValuePropertiesTypeDef(TypedDict):
    model: NotRequired[str],
    field: NotRequired[str],
    predicates: NotRequired[Sequence[PredicateTypeDef]],  # (1)
    userAttribute: NotRequired[str],
    bucket: NotRequired[str],
    key: NotRequired[str],
    defaultValue: NotRequired[str],
    slotName: NotRequired[str],
```

1. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
## ComponentConditionPropertyTypeDef

```python
# ComponentConditionPropertyTypeDef definition

class ComponentConditionPropertyTypeDef(TypedDict):
    property: NotRequired[str],
    field: NotRequired[str],
    operator: NotRequired[str],
    operand: NotRequired[str],
    then: NotRequired[ComponentPropertyTypeDef],  # (1)
    else: NotRequired[ComponentPropertyTypeDef],  # (1)
    operandType: NotRequired[str],
```

1. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
2. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
## SortPropertyTypeDef

```python
# SortPropertyTypeDef definition

class SortPropertyTypeDef(TypedDict):
    field: str,
    direction: SortDirectionType,  # (1)
```

1. See [:material-code-brackets: SortDirectionType](./literals.md#sortdirectiontype) 
## ComponentPropertyBindingPropertiesTypeDef

```python
# ComponentPropertyBindingPropertiesTypeDef definition

class ComponentPropertyBindingPropertiesTypeDef(TypedDict):
    property: str,
    field: NotRequired[str],
```

## FormBindingElementTypeDef

```python
# FormBindingElementTypeDef definition

class FormBindingElementTypeDef(TypedDict):
    element: str,
    property: str,
```

## ComponentSummaryTypeDef

```python
# ComponentSummaryTypeDef definition

class ComponentSummaryTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
    name: str,
    componentType: str,
```

## ComponentVariantTypeDef

```python
# ComponentVariantTypeDef definition

class ComponentVariantTypeDef(TypedDict):
    variantValues: NotRequired[Mapping[str, str]],
    overrides: NotRequired[Mapping[str, Mapping[str, str]]],
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

## FormDataTypeConfigTypeDef

```python
# FormDataTypeConfigTypeDef definition

class FormDataTypeConfigTypeDef(TypedDict):
    dataSourceType: FormDataSourceTypeType,  # (1)
    dataTypeName: str,
```

1. See [:material-code-brackets: FormDataSourceTypeType](./literals.md#formdatasourcetypetype) 
## CreateThemeDataTypeDef

```python
# CreateThemeDataTypeDef definition

class CreateThemeDataTypeDef(TypedDict):
    name: str,
    values: Sequence[ThemeValuesTypeDef],  # (1)
    overrides: NotRequired[Sequence[ThemeValuesTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ThemeValuesTypeDef](./type_defs.md#themevaluestypedef) 
2. See [:material-code-braces: ThemeValuesTypeDef](./type_defs.md#themevaluestypedef) 
## ThemeTypeDef

```python
# ThemeTypeDef definition

class ThemeTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
    name: str,
    createdAt: datetime,
    values: List[ThemeValuesTypeDef],  # (1)
    modifiedAt: NotRequired[datetime],
    overrides: NotRequired[List[ThemeValuesTypeDef]],  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ThemeValuesTypeDef](./type_defs.md#themevaluestypedef) 
2. See [:material-code-braces: ThemeValuesTypeDef](./type_defs.md#themevaluestypedef) 
## DeleteComponentRequestRequestTypeDef

```python
# DeleteComponentRequestRequestTypeDef definition

class DeleteComponentRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
```

## DeleteFormRequestRequestTypeDef

```python
# DeleteFormRequestRequestTypeDef definition

class DeleteFormRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
```

## DeleteThemeRequestRequestTypeDef

```python
# DeleteThemeRequestRequestTypeDef definition

class DeleteThemeRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
```

## ExchangeCodeForTokenRequestBodyTypeDef

```python
# ExchangeCodeForTokenRequestBodyTypeDef definition

class ExchangeCodeForTokenRequestBodyTypeDef(TypedDict):
    code: str,
    redirectUri: str,
    clientId: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ExportComponentsRequestRequestTypeDef

```python
# ExportComponentsRequestRequestTypeDef definition

class ExportComponentsRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    nextToken: NotRequired[str],
```

## ExportFormsRequestRequestTypeDef

```python
# ExportFormsRequestRequestTypeDef definition

class ExportFormsRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    nextToken: NotRequired[str],
```

## ExportThemesRequestRequestTypeDef

```python
# ExportThemesRequestRequestTypeDef definition

class ExportThemesRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    nextToken: NotRequired[str],
```

## FieldPositionTypeDef

```python
# FieldPositionTypeDef definition

class FieldPositionTypeDef(TypedDict):
    fixed: NotRequired[FixedPositionType],  # (1)
    rightOf: NotRequired[str],
    below: NotRequired[str],
```

1. See [:material-code-brackets: FixedPositionType](./literals.md#fixedpositiontype) 
## FieldValidationConfigurationTypeDef

```python
# FieldValidationConfigurationTypeDef definition

class FieldValidationConfigurationTypeDef(TypedDict):
    type: str,
    strValues: NotRequired[Sequence[str]],
    numValues: NotRequired[Sequence[int]],
    validationMessage: NotRequired[str],
```

## FileUploaderFieldConfigTypeDef

```python
# FileUploaderFieldConfigTypeDef definition

class FileUploaderFieldConfigTypeDef(TypedDict):
    accessLevel: StorageAccessLevelType,  # (1)
    acceptedFileTypes: Sequence[str],
    showThumbnails: NotRequired[bool],
    isResumable: NotRequired[bool],
    maxFileCount: NotRequired[int],
    maxSize: NotRequired[int],
```

1. See [:material-code-brackets: StorageAccessLevelType](./literals.md#storageaccessleveltype) 
## FormInputBindingPropertiesValuePropertiesTypeDef

```python
# FormInputBindingPropertiesValuePropertiesTypeDef definition

class FormInputBindingPropertiesValuePropertiesTypeDef(TypedDict):
    model: NotRequired[str],
```

## FormInputValuePropertyBindingPropertiesTypeDef

```python
# FormInputValuePropertyBindingPropertiesTypeDef definition

class FormInputValuePropertyBindingPropertiesTypeDef(TypedDict):
    property: str,
    field: NotRequired[str],
```

## FormStyleConfigTypeDef

```python
# FormStyleConfigTypeDef definition

class FormStyleConfigTypeDef(TypedDict):
    tokenReference: NotRequired[str],
    value: NotRequired[str],
```

## GetCodegenJobRequestRequestTypeDef

```python
# GetCodegenJobRequestRequestTypeDef definition

class GetCodegenJobRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
```

## GetComponentRequestRequestTypeDef

```python
# GetComponentRequestRequestTypeDef definition

class GetComponentRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
```

## GetFormRequestRequestTypeDef

```python
# GetFormRequestRequestTypeDef definition

class GetFormRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
```

## GetMetadataRequestRequestTypeDef

```python
# GetMetadataRequestRequestTypeDef definition

class GetMetadataRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
```

## GetThemeRequestRequestTypeDef

```python
# GetThemeRequestRequestTypeDef definition

class GetThemeRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
```

## ListCodegenJobsRequestRequestTypeDef

```python
# ListCodegenJobsRequestRequestTypeDef definition

class ListCodegenJobsRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListComponentsRequestRequestTypeDef

```python
# ListComponentsRequestRequestTypeDef definition

class ListComponentsRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListFormsRequestRequestTypeDef

```python
# ListFormsRequestRequestTypeDef definition

class ListFormsRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListThemesRequestRequestTypeDef

```python
# ListThemesRequestRequestTypeDef definition

class ListThemesRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ThemeSummaryTypeDef

```python
# ThemeSummaryTypeDef definition

class ThemeSummaryTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
    name: str,
```

## PredicateTypeDef

```python
# PredicateTypeDef definition

class PredicateTypeDef(TypedDict):
    or: NotRequired[Sequence[PredicateTypeDef]],  # (1)
    and: NotRequired[Sequence[PredicateTypeDef]],  # (1)
    field: NotRequired[str],
    operator: NotRequired[str],
    operand: NotRequired[str],
    operandType: NotRequired[str],
```

1. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
2. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
## PutMetadataFlagBodyTypeDef

```python
# PutMetadataFlagBodyTypeDef definition

class PutMetadataFlagBodyTypeDef(TypedDict):
    newValue: str,
```

## RefreshTokenRequestBodyTypeDef

```python
# RefreshTokenRequestBodyTypeDef definition

class RefreshTokenRequestBodyTypeDef(TypedDict):
    token: str,
    clientId: NotRequired[str],
```

## ThemeValueTypeDef

```python
# ThemeValueTypeDef definition

class ThemeValueTypeDef(TypedDict):
    value: NotRequired[str],
    children: NotRequired[Sequence[ThemeValuesTypeDef]],  # (1)
```

1. See [:material-code-braces: ThemeValuesTypeDef](./type_defs.md#themevaluestypedef) 
## ThemeValuesTypeDef

```python
# ThemeValuesTypeDef definition

class ThemeValuesTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[ThemeValueTypeDef],  # (1)
```

1. See [:material-code-braces: ThemeValueTypeDef](./type_defs.md#themevaluetypedef) 
## UpdateThemeDataTypeDef

```python
# UpdateThemeDataTypeDef definition

class UpdateThemeDataTypeDef(TypedDict):
    values: Sequence[ThemeValuesTypeDef],  # (1)
    id: NotRequired[str],
    name: NotRequired[str],
    overrides: NotRequired[Sequence[ThemeValuesTypeDef]],  # (1)
```

1. See [:material-code-braces: ThemeValuesTypeDef](./type_defs.md#themevaluestypedef) 
2. See [:material-code-braces: ThemeValuesTypeDef](./type_defs.md#themevaluestypedef) 
## ValueMappingTypeDef

```python
# ValueMappingTypeDef definition

class ValueMappingTypeDef(TypedDict):
    value: FormInputValuePropertyTypeDef,  # (1)
    displayValue: NotRequired[FormInputValuePropertyTypeDef],  # (1)
```

1. See [:material-code-braces: FormInputValuePropertyTypeDef](./type_defs.md#forminputvaluepropertytypedef) 
2. See [:material-code-braces: FormInputValuePropertyTypeDef](./type_defs.md#forminputvaluepropertytypedef) 
## ActionParametersTypeDef

```python
# ActionParametersTypeDef definition

class ActionParametersTypeDef(TypedDict):
    type: NotRequired[ComponentPropertyTypeDef],  # (1)
    url: NotRequired[ComponentPropertyTypeDef],  # (1)
    anchor: NotRequired[ComponentPropertyTypeDef],  # (1)
    target: NotRequired[ComponentPropertyTypeDef],  # (1)
    global: NotRequired[ComponentPropertyTypeDef],  # (1)
    model: NotRequired[str],
    id: NotRequired[ComponentPropertyTypeDef],  # (1)
    fields: NotRequired[Mapping[str, ComponentPropertyTypeDef]],  # (7)
    state: NotRequired[MutationActionSetStateParameterTypeDef],  # (8)
```

1. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
2. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
3. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
4. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
5. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
6. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
7. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
8. See [:material-code-braces: MutationActionSetStateParameterTypeDef](./type_defs.md#mutationactionsetstateparametertypedef) 
## ApiConfigurationTypeDef

```python
# ApiConfigurationTypeDef definition

class ApiConfigurationTypeDef(TypedDict):
    graphQLConfig: NotRequired[GraphQLRenderConfigTypeDef],  # (1)
    dataStoreConfig: NotRequired[Dict[str, Any]],
    noApiConfig: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: GraphQLRenderConfigTypeDef](./type_defs.md#graphqlrenderconfigtypedef) 
## CodegenGenericDataFieldTypeDef

```python
# CodegenGenericDataFieldTypeDef definition

class CodegenGenericDataFieldTypeDef(TypedDict):
    dataType: CodegenGenericDataFieldDataTypeType,  # (1)
    dataTypeValue: str,
    required: bool,
    readOnly: bool,
    isArray: bool,
    relationship: NotRequired[CodegenGenericDataRelationshipTypeTypeDef],  # (2)
```

1. See [:material-code-brackets: CodegenGenericDataFieldDataTypeType](./literals.md#codegengenericdatafielddatatypetype) 
2. See [:material-code-braces: CodegenGenericDataRelationshipTypeTypeDef](./type_defs.md#codegengenericdatarelationshiptypetypedef) 
## ComponentBindingPropertiesValueTypeDef

```python
# ComponentBindingPropertiesValueTypeDef definition

class ComponentBindingPropertiesValueTypeDef(TypedDict):
    type: NotRequired[str],
    bindingProperties: NotRequired[ComponentBindingPropertiesValuePropertiesTypeDef],  # (1)
    defaultValue: NotRequired[str],
```

1. See [:material-code-braces: ComponentBindingPropertiesValuePropertiesTypeDef](./type_defs.md#componentbindingpropertiesvaluepropertiestypedef) 
## ComponentDataConfigurationTypeDef

```python
# ComponentDataConfigurationTypeDef definition

class ComponentDataConfigurationTypeDef(TypedDict):
    model: str,
    sort: NotRequired[Sequence[SortPropertyTypeDef]],  # (1)
    predicate: NotRequired[PredicateTypeDef],  # (2)
    identifiers: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: SortPropertyTypeDef](./type_defs.md#sortpropertytypedef) 
2. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
## ComponentPropertyTypeDef

```python
# ComponentPropertyTypeDef definition

class ComponentPropertyTypeDef(TypedDict):
    value: NotRequired[str],
    bindingProperties: NotRequired[ComponentPropertyBindingPropertiesTypeDef],  # (1)
    collectionBindingProperties: NotRequired[ComponentPropertyBindingPropertiesTypeDef],  # (1)
    defaultValue: NotRequired[str],
    model: NotRequired[str],
    bindings: NotRequired[Mapping[str, FormBindingElementTypeDef]],  # (3)
    event: NotRequired[str],
    userAttribute: NotRequired[str],
    concat: NotRequired[Sequence[ComponentPropertyTypeDef]],  # (4)
    condition: NotRequired[ComponentConditionPropertyTypeDef],  # (5)
    configured: NotRequired[bool],
    type: NotRequired[str],
    importedValue: NotRequired[str],
    componentName: NotRequired[str],
    property: NotRequired[str],
```

1. See [:material-code-braces: ComponentPropertyBindingPropertiesTypeDef](./type_defs.md#componentpropertybindingpropertiestypedef) 
2. See [:material-code-braces: ComponentPropertyBindingPropertiesTypeDef](./type_defs.md#componentpropertybindingpropertiestypedef) 
3. See [:material-code-braces: FormBindingElementTypeDef](./type_defs.md#formbindingelementtypedef) 
4. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
5. See [:material-code-braces: ComponentConditionPropertyTypeDef](./type_defs.md#componentconditionpropertytypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExchangeCodeForTokenResponseTypeDef

```python
# ExchangeCodeForTokenResponseTypeDef definition

class ExchangeCodeForTokenResponseTypeDef(TypedDict):
    accessToken: str,
    expiresIn: int,
    refreshToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMetadataResponseTypeDef

```python
# GetMetadataResponseTypeDef definition

class GetMetadataResponseTypeDef(TypedDict):
    features: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCodegenJobsResponseTypeDef

```python
# ListCodegenJobsResponseTypeDef definition

class ListCodegenJobsResponseTypeDef(TypedDict):
    entities: List[CodegenJobSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodegenJobSummaryTypeDef](./type_defs.md#codegenjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListComponentsResponseTypeDef

```python
# ListComponentsResponseTypeDef definition

class ListComponentsResponseTypeDef(TypedDict):
    entities: List[ComponentSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentSummaryTypeDef](./type_defs.md#componentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RefreshTokenResponseTypeDef

```python
# RefreshTokenResponseTypeDef definition

class RefreshTokenResponseTypeDef(TypedDict):
    accessToken: str,
    expiresIn: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FormSummaryTypeDef

```python
# FormSummaryTypeDef definition

class FormSummaryTypeDef(TypedDict):
    appId: str,
    dataType: FormDataTypeConfigTypeDef,  # (1)
    environmentName: str,
    formActionType: FormActionTypeType,  # (2)
    id: str,
    name: str,
```

1. See [:material-code-braces: FormDataTypeConfigTypeDef](./type_defs.md#formdatatypeconfigtypedef) 
2. See [:material-code-brackets: FormActionTypeType](./literals.md#formactiontypetype) 
## CreateThemeRequestRequestTypeDef

```python
# CreateThemeRequestRequestTypeDef definition

class CreateThemeRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    themeToCreate: CreateThemeDataTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: CreateThemeDataTypeDef](./type_defs.md#createthemedatatypedef) 
## CreateThemeResponseTypeDef

```python
# CreateThemeResponseTypeDef definition

class CreateThemeResponseTypeDef(TypedDict):
    entity: ThemeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeTypeDef](./type_defs.md#themetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportThemesResponseTypeDef

```python
# ExportThemesResponseTypeDef definition

class ExportThemesResponseTypeDef(TypedDict):
    entities: List[ThemeTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeTypeDef](./type_defs.md#themetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetThemeResponseTypeDef

```python
# GetThemeResponseTypeDef definition

class GetThemeResponseTypeDef(TypedDict):
    theme: ThemeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeTypeDef](./type_defs.md#themetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateThemeResponseTypeDef

```python
# UpdateThemeResponseTypeDef definition

class UpdateThemeResponseTypeDef(TypedDict):
    entity: ThemeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeTypeDef](./type_defs.md#themetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExchangeCodeForTokenRequestRequestTypeDef

```python
# ExchangeCodeForTokenRequestRequestTypeDef definition

class ExchangeCodeForTokenRequestRequestTypeDef(TypedDict):
    provider: TokenProvidersType,  # (1)
    request: ExchangeCodeForTokenRequestBodyTypeDef,  # (2)
```

1. See [:material-code-brackets: TokenProvidersType](./literals.md#tokenproviderstype) 
2. See [:material-code-braces: ExchangeCodeForTokenRequestBodyTypeDef](./type_defs.md#exchangecodefortokenrequestbodytypedef) 
## ExportComponentsRequestExportComponentsPaginateTypeDef

```python
# ExportComponentsRequestExportComponentsPaginateTypeDef definition

class ExportComponentsRequestExportComponentsPaginateTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ExportFormsRequestExportFormsPaginateTypeDef

```python
# ExportFormsRequestExportFormsPaginateTypeDef definition

class ExportFormsRequestExportFormsPaginateTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ExportThemesRequestExportThemesPaginateTypeDef

```python
# ExportThemesRequestExportThemesPaginateTypeDef definition

class ExportThemesRequestExportThemesPaginateTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCodegenJobsRequestListCodegenJobsPaginateTypeDef

```python
# ListCodegenJobsRequestListCodegenJobsPaginateTypeDef definition

class ListCodegenJobsRequestListCodegenJobsPaginateTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListComponentsRequestListComponentsPaginateTypeDef

```python
# ListComponentsRequestListComponentsPaginateTypeDef definition

class ListComponentsRequestListComponentsPaginateTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFormsRequestListFormsPaginateTypeDef

```python
# ListFormsRequestListFormsPaginateTypeDef definition

class ListFormsRequestListFormsPaginateTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThemesRequestListThemesPaginateTypeDef

```python
# ListThemesRequestListThemesPaginateTypeDef definition

class ListThemesRequestListThemesPaginateTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## FormButtonTypeDef

```python
# FormButtonTypeDef definition

class FormButtonTypeDef(TypedDict):
    excluded: NotRequired[bool],
    children: NotRequired[str],
    position: NotRequired[FieldPositionTypeDef],  # (1)
```

1. See [:material-code-braces: FieldPositionTypeDef](./type_defs.md#fieldpositiontypedef) 
## SectionalElementTypeDef

```python
# SectionalElementTypeDef definition

class SectionalElementTypeDef(TypedDict):
    type: str,
    position: NotRequired[FieldPositionTypeDef],  # (1)
    text: NotRequired[str],
    level: NotRequired[int],
    orientation: NotRequired[str],
    excluded: NotRequired[bool],
```

1. See [:material-code-braces: FieldPositionTypeDef](./type_defs.md#fieldpositiontypedef) 
## FormInputBindingPropertiesValueTypeDef

```python
# FormInputBindingPropertiesValueTypeDef definition

class FormInputBindingPropertiesValueTypeDef(TypedDict):
    type: NotRequired[str],
    bindingProperties: NotRequired[FormInputBindingPropertiesValuePropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: FormInputBindingPropertiesValuePropertiesTypeDef](./type_defs.md#forminputbindingpropertiesvaluepropertiestypedef) 
## FormInputValuePropertyTypeDef

```python
# FormInputValuePropertyTypeDef definition

class FormInputValuePropertyTypeDef(TypedDict):
    value: NotRequired[str],
    bindingProperties: NotRequired[FormInputValuePropertyBindingPropertiesTypeDef],  # (1)
    concat: NotRequired[Sequence[FormInputValuePropertyTypeDef]],  # (2)
```

1. See [:material-code-braces: FormInputValuePropertyBindingPropertiesTypeDef](./type_defs.md#forminputvaluepropertybindingpropertiestypedef) 
2. See [:material-code-braces: FormInputValuePropertyTypeDef](./type_defs.md#forminputvaluepropertytypedef) 
## FormStyleTypeDef

```python
# FormStyleTypeDef definition

class FormStyleTypeDef(TypedDict):
    horizontalGap: NotRequired[FormStyleConfigTypeDef],  # (1)
    verticalGap: NotRequired[FormStyleConfigTypeDef],  # (1)
    outerPadding: NotRequired[FormStyleConfigTypeDef],  # (1)
```

1. See [:material-code-braces: FormStyleConfigTypeDef](./type_defs.md#formstyleconfigtypedef) 
2. See [:material-code-braces: FormStyleConfigTypeDef](./type_defs.md#formstyleconfigtypedef) 
3. See [:material-code-braces: FormStyleConfigTypeDef](./type_defs.md#formstyleconfigtypedef) 
## ListThemesResponseTypeDef

```python
# ListThemesResponseTypeDef definition

class ListThemesResponseTypeDef(TypedDict):
    entities: List[ThemeSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeSummaryTypeDef](./type_defs.md#themesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutMetadataFlagRequestRequestTypeDef

```python
# PutMetadataFlagRequestRequestTypeDef definition

class PutMetadataFlagRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    featureName: str,
    body: PutMetadataFlagBodyTypeDef,  # (1)
```

1. See [:material-code-braces: PutMetadataFlagBodyTypeDef](./type_defs.md#putmetadataflagbodytypedef) 
## RefreshTokenRequestRequestTypeDef

```python
# RefreshTokenRequestRequestTypeDef definition

class RefreshTokenRequestRequestTypeDef(TypedDict):
    provider: TokenProvidersType,  # (1)
    refreshTokenBody: RefreshTokenRequestBodyTypeDef,  # (2)
```

1. See [:material-code-brackets: TokenProvidersType](./literals.md#tokenproviderstype) 
2. See [:material-code-braces: RefreshTokenRequestBodyTypeDef](./type_defs.md#refreshtokenrequestbodytypedef) 
## UpdateThemeRequestRequestTypeDef

```python
# UpdateThemeRequestRequestTypeDef definition

class UpdateThemeRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
    updatedTheme: UpdateThemeDataTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: UpdateThemeDataTypeDef](./type_defs.md#updatethemedatatypedef) 
## ComponentEventTypeDef

```python
# ComponentEventTypeDef definition

class ComponentEventTypeDef(TypedDict):
    action: NotRequired[str],
    parameters: NotRequired[ActionParametersTypeDef],  # (1)
    bindingEvent: NotRequired[str],
```

1. See [:material-code-braces: ActionParametersTypeDef](./type_defs.md#actionparameterstypedef) 
## ReactStartCodegenJobDataTypeDef

```python
# ReactStartCodegenJobDataTypeDef definition

class ReactStartCodegenJobDataTypeDef(TypedDict):
    module: NotRequired[JSModuleType],  # (1)
    target: NotRequired[JSTargetType],  # (2)
    script: NotRequired[JSScriptType],  # (3)
    renderTypeDeclarations: NotRequired[bool],
    inlineSourceMap: NotRequired[bool],
    apiConfiguration: NotRequired[ApiConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: JSModuleType](./literals.md#jsmoduletype) 
2. See [:material-code-brackets: JSTargetType](./literals.md#jstargettype) 
3. See [:material-code-brackets: JSScriptType](./literals.md#jsscripttype) 
4. See [:material-code-braces: ApiConfigurationTypeDef](./type_defs.md#apiconfigurationtypedef) 
## CodegenGenericDataModelTypeDef

```python
# CodegenGenericDataModelTypeDef definition

class CodegenGenericDataModelTypeDef(TypedDict):
    fields: Dict[str, CodegenGenericDataFieldTypeDef],  # (1)
    primaryKeys: List[str],
    isJoinTable: NotRequired[bool],
```

1. See [:material-code-braces: CodegenGenericDataFieldTypeDef](./type_defs.md#codegengenericdatafieldtypedef) 
## CodegenGenericDataNonModelTypeDef

```python
# CodegenGenericDataNonModelTypeDef definition

class CodegenGenericDataNonModelTypeDef(TypedDict):
    fields: Dict[str, CodegenGenericDataFieldTypeDef],  # (1)
```

1. See [:material-code-braces: CodegenGenericDataFieldTypeDef](./type_defs.md#codegengenericdatafieldtypedef) 
## ListFormsResponseTypeDef

```python
# ListFormsResponseTypeDef definition

class ListFormsResponseTypeDef(TypedDict):
    entities: List[FormSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FormSummaryTypeDef](./type_defs.md#formsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FormCTATypeDef

```python
# FormCTATypeDef definition

class FormCTATypeDef(TypedDict):
    position: NotRequired[FormButtonsPositionType],  # (1)
    clear: NotRequired[FormButtonTypeDef],  # (2)
    cancel: NotRequired[FormButtonTypeDef],  # (2)
    submit: NotRequired[FormButtonTypeDef],  # (2)
```

1. See [:material-code-brackets: FormButtonsPositionType](./literals.md#formbuttonspositiontype) 
2. See [:material-code-braces: FormButtonTypeDef](./type_defs.md#formbuttontypedef) 
3. See [:material-code-braces: FormButtonTypeDef](./type_defs.md#formbuttontypedef) 
4. See [:material-code-braces: FormButtonTypeDef](./type_defs.md#formbuttontypedef) 
## ValueMappingsTypeDef

```python
# ValueMappingsTypeDef definition

class ValueMappingsTypeDef(TypedDict):
    values: Sequence[ValueMappingTypeDef],  # (1)
    bindingProperties: NotRequired[Mapping[str, FormInputBindingPropertiesValueTypeDef]],  # (2)
```

1. See [:material-code-braces: ValueMappingTypeDef](./type_defs.md#valuemappingtypedef) 
2. See [:material-code-braces: FormInputBindingPropertiesValueTypeDef](./type_defs.md#forminputbindingpropertiesvaluetypedef) 
## ComponentChildTypeDef

```python
# ComponentChildTypeDef definition

class ComponentChildTypeDef(TypedDict):
    componentType: str,
    name: str,
    properties: Mapping[str, ComponentPropertyTypeDef],  # (1)
    children: NotRequired[Sequence[ComponentChildTypeDef]],  # (2)
    events: NotRequired[Mapping[str, ComponentEventTypeDef]],  # (3)
    sourceId: NotRequired[str],
```

1. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
2. See [:material-code-braces: ComponentChildTypeDef](./type_defs.md#componentchildtypedef) 
3. See [:material-code-braces: ComponentEventTypeDef](./type_defs.md#componenteventtypedef) 
## ComponentTypeDef

```python
# ComponentTypeDef definition

class ComponentTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
    name: str,
    componentType: str,
    properties: Dict[str, ComponentPropertyTypeDef],  # (1)
    variants: List[ComponentVariantTypeDef],  # (3)
    overrides: Dict[str, Dict[str, str]],
    bindingProperties: Dict[str, ComponentBindingPropertiesValueTypeDef],  # (4)
    createdAt: datetime,
    sourceId: NotRequired[str],
    children: NotRequired[List[ComponentChildTypeDef]],  # (2)
    collectionProperties: NotRequired[Dict[str, ComponentDataConfigurationTypeDef]],  # (5)
    modifiedAt: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
    events: NotRequired[Dict[str, ComponentEventTypeDef]],  # (6)
    schemaVersion: NotRequired[str],
```

1. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
2. See [:material-code-braces: ComponentChildTypeDef](./type_defs.md#componentchildtypedef) 
3. See [:material-code-braces: ComponentVariantTypeDef](./type_defs.md#componentvarianttypedef) 
4. See [:material-code-braces: ComponentBindingPropertiesValueTypeDef](./type_defs.md#componentbindingpropertiesvaluetypedef) 
5. See [:material-code-braces: ComponentDataConfigurationTypeDef](./type_defs.md#componentdataconfigurationtypedef) 
6. See [:material-code-braces: ComponentEventTypeDef](./type_defs.md#componenteventtypedef) 
## CreateComponentDataTypeDef

```python
# CreateComponentDataTypeDef definition

class CreateComponentDataTypeDef(TypedDict):
    name: str,
    componentType: str,
    properties: Mapping[str, ComponentPropertyTypeDef],  # (1)
    variants: Sequence[ComponentVariantTypeDef],  # (3)
    overrides: Mapping[str, Mapping[str, str]],
    bindingProperties: Mapping[str, ComponentBindingPropertiesValueTypeDef],  # (4)
    sourceId: NotRequired[str],
    children: NotRequired[Sequence[ComponentChildTypeDef]],  # (2)
    collectionProperties: NotRequired[Mapping[str, ComponentDataConfigurationTypeDef]],  # (5)
    tags: NotRequired[Mapping[str, str]],
    events: NotRequired[Mapping[str, ComponentEventTypeDef]],  # (6)
    schemaVersion: NotRequired[str],
```

1. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
2. See [:material-code-braces: ComponentChildTypeDef](./type_defs.md#componentchildtypedef) 
3. See [:material-code-braces: ComponentVariantTypeDef](./type_defs.md#componentvarianttypedef) 
4. See [:material-code-braces: ComponentBindingPropertiesValueTypeDef](./type_defs.md#componentbindingpropertiesvaluetypedef) 
5. See [:material-code-braces: ComponentDataConfigurationTypeDef](./type_defs.md#componentdataconfigurationtypedef) 
6. See [:material-code-braces: ComponentEventTypeDef](./type_defs.md#componenteventtypedef) 
## UpdateComponentDataTypeDef

```python
# UpdateComponentDataTypeDef definition

class UpdateComponentDataTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    sourceId: NotRequired[str],
    componentType: NotRequired[str],
    properties: NotRequired[Mapping[str, ComponentPropertyTypeDef]],  # (1)
    children: NotRequired[Sequence[ComponentChildTypeDef]],  # (2)
    variants: NotRequired[Sequence[ComponentVariantTypeDef]],  # (3)
    overrides: NotRequired[Mapping[str, Mapping[str, str]]],
    bindingProperties: NotRequired[Mapping[str, ComponentBindingPropertiesValueTypeDef]],  # (4)
    collectionProperties: NotRequired[Mapping[str, ComponentDataConfigurationTypeDef]],  # (5)
    events: NotRequired[Mapping[str, ComponentEventTypeDef]],  # (6)
    schemaVersion: NotRequired[str],
```

1. See [:material-code-braces: ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef) 
2. See [:material-code-braces: ComponentChildTypeDef](./type_defs.md#componentchildtypedef) 
3. See [:material-code-braces: ComponentVariantTypeDef](./type_defs.md#componentvarianttypedef) 
4. See [:material-code-braces: ComponentBindingPropertiesValueTypeDef](./type_defs.md#componentbindingpropertiesvaluetypedef) 
5. See [:material-code-braces: ComponentDataConfigurationTypeDef](./type_defs.md#componentdataconfigurationtypedef) 
6. See [:material-code-braces: ComponentEventTypeDef](./type_defs.md#componenteventtypedef) 
## CodegenJobRenderConfigTypeDef

```python
# CodegenJobRenderConfigTypeDef definition

class CodegenJobRenderConfigTypeDef(TypedDict):
    react: NotRequired[ReactStartCodegenJobDataTypeDef],  # (1)
```

1. See [:material-code-braces: ReactStartCodegenJobDataTypeDef](./type_defs.md#reactstartcodegenjobdatatypedef) 
## CodegenJobGenericDataSchemaTypeDef

```python
# CodegenJobGenericDataSchemaTypeDef definition

class CodegenJobGenericDataSchemaTypeDef(TypedDict):
    dataSourceType: CodegenJobGenericDataSourceTypeType,  # (1)
    models: Dict[str, CodegenGenericDataModelTypeDef],  # (2)
    enums: Dict[str, CodegenGenericDataEnumTypeDef],  # (3)
    nonModels: Dict[str, CodegenGenericDataNonModelTypeDef],  # (4)
```

1. See [:material-code-brackets: CodegenJobGenericDataSourceTypeType](./literals.md#codegenjobgenericdatasourcetypetype) 
2. See [:material-code-braces: CodegenGenericDataModelTypeDef](./type_defs.md#codegengenericdatamodeltypedef) 
3. See [:material-code-braces: CodegenGenericDataEnumTypeDef](./type_defs.md#codegengenericdataenumtypedef) 
4. See [:material-code-braces: CodegenGenericDataNonModelTypeDef](./type_defs.md#codegengenericdatanonmodeltypedef) 
## FieldInputConfigTypeDef

```python
# FieldInputConfigTypeDef definition

class FieldInputConfigTypeDef(TypedDict):
    type: str,
    required: NotRequired[bool],
    readOnly: NotRequired[bool],
    placeholder: NotRequired[str],
    defaultValue: NotRequired[str],
    descriptiveText: NotRequired[str],
    defaultChecked: NotRequired[bool],
    defaultCountryCode: NotRequired[str],
    valueMappings: NotRequired[ValueMappingsTypeDef],  # (1)
    name: NotRequired[str],
    minValue: NotRequired[float],
    maxValue: NotRequired[float],
    step: NotRequired[float],
    value: NotRequired[str],
    isArray: NotRequired[bool],
    fileUploaderConfig: NotRequired[FileUploaderFieldConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ValueMappingsTypeDef](./type_defs.md#valuemappingstypedef) 
2. See [:material-code-braces: FileUploaderFieldConfigTypeDef](./type_defs.md#fileuploaderfieldconfigtypedef) 
## CreateComponentResponseTypeDef

```python
# CreateComponentResponseTypeDef definition

class CreateComponentResponseTypeDef(TypedDict):
    entity: ComponentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentTypeDef](./type_defs.md#componenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportComponentsResponseTypeDef

```python
# ExportComponentsResponseTypeDef definition

class ExportComponentsResponseTypeDef(TypedDict):
    entities: List[ComponentTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentTypeDef](./type_defs.md#componenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComponentResponseTypeDef

```python
# GetComponentResponseTypeDef definition

class GetComponentResponseTypeDef(TypedDict):
    component: ComponentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentTypeDef](./type_defs.md#componenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateComponentResponseTypeDef

```python
# UpdateComponentResponseTypeDef definition

class UpdateComponentResponseTypeDef(TypedDict):
    entity: ComponentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentTypeDef](./type_defs.md#componenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateComponentRequestRequestTypeDef

```python
# CreateComponentRequestRequestTypeDef definition

class CreateComponentRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    componentToCreate: CreateComponentDataTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: CreateComponentDataTypeDef](./type_defs.md#createcomponentdatatypedef) 
## UpdateComponentRequestRequestTypeDef

```python
# UpdateComponentRequestRequestTypeDef definition

class UpdateComponentRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
    updatedComponent: UpdateComponentDataTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: UpdateComponentDataTypeDef](./type_defs.md#updatecomponentdatatypedef) 
## CodegenJobTypeDef

```python
# CodegenJobTypeDef definition

class CodegenJobTypeDef(TypedDict):
    id: str,
    appId: str,
    environmentName: str,
    renderConfig: NotRequired[CodegenJobRenderConfigTypeDef],  # (1)
    genericDataSchema: NotRequired[CodegenJobGenericDataSchemaTypeDef],  # (2)
    autoGenerateForms: NotRequired[bool],
    features: NotRequired[CodegenFeatureFlagsTypeDef],  # (3)
    status: NotRequired[CodegenJobStatusType],  # (4)
    statusMessage: NotRequired[str],
    asset: NotRequired[CodegenJobAssetTypeDef],  # (5)
    tags: NotRequired[Dict[str, str]],
    createdAt: NotRequired[datetime],
    modifiedAt: NotRequired[datetime],
```

1. See [:material-code-braces: CodegenJobRenderConfigTypeDef](./type_defs.md#codegenjobrenderconfigtypedef) 
2. See [:material-code-braces: CodegenJobGenericDataSchemaTypeDef](./type_defs.md#codegenjobgenericdataschematypedef) 
3. See [:material-code-braces: CodegenFeatureFlagsTypeDef](./type_defs.md#codegenfeatureflagstypedef) 
4. See [:material-code-brackets: CodegenJobStatusType](./literals.md#codegenjobstatustype) 
5. See [:material-code-braces: CodegenJobAssetTypeDef](./type_defs.md#codegenjobassettypedef) 
## StartCodegenJobDataTypeDef

```python
# StartCodegenJobDataTypeDef definition

class StartCodegenJobDataTypeDef(TypedDict):
    renderConfig: CodegenJobRenderConfigTypeDef,  # (1)
    genericDataSchema: NotRequired[CodegenJobGenericDataSchemaTypeDef],  # (2)
    autoGenerateForms: NotRequired[bool],
    features: NotRequired[CodegenFeatureFlagsTypeDef],  # (3)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CodegenJobRenderConfigTypeDef](./type_defs.md#codegenjobrenderconfigtypedef) 
2. See [:material-code-braces: CodegenJobGenericDataSchemaTypeDef](./type_defs.md#codegenjobgenericdataschematypedef) 
3. See [:material-code-braces: CodegenFeatureFlagsTypeDef](./type_defs.md#codegenfeatureflagstypedef) 
## FieldConfigTypeDef

```python
# FieldConfigTypeDef definition

class FieldConfigTypeDef(TypedDict):
    label: NotRequired[str],
    position: NotRequired[FieldPositionTypeDef],  # (1)
    excluded: NotRequired[bool],
    inputType: NotRequired[FieldInputConfigTypeDef],  # (2)
    validations: NotRequired[Sequence[FieldValidationConfigurationTypeDef]],  # (3)
```

1. See [:material-code-braces: FieldPositionTypeDef](./type_defs.md#fieldpositiontypedef) 
2. See [:material-code-braces: FieldInputConfigTypeDef](./type_defs.md#fieldinputconfigtypedef) 
3. See [:material-code-braces: FieldValidationConfigurationTypeDef](./type_defs.md#fieldvalidationconfigurationtypedef) 
## GetCodegenJobResponseTypeDef

```python
# GetCodegenJobResponseTypeDef definition

class GetCodegenJobResponseTypeDef(TypedDict):
    job: CodegenJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodegenJobTypeDef](./type_defs.md#codegenjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCodegenJobResponseTypeDef

```python
# StartCodegenJobResponseTypeDef definition

class StartCodegenJobResponseTypeDef(TypedDict):
    entity: CodegenJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodegenJobTypeDef](./type_defs.md#codegenjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCodegenJobRequestRequestTypeDef

```python
# StartCodegenJobRequestRequestTypeDef definition

class StartCodegenJobRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    codegenJobToCreate: StartCodegenJobDataTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: StartCodegenJobDataTypeDef](./type_defs.md#startcodegenjobdatatypedef) 
## CreateFormDataTypeDef

```python
# CreateFormDataTypeDef definition

class CreateFormDataTypeDef(TypedDict):
    name: str,
    dataType: FormDataTypeConfigTypeDef,  # (1)
    formActionType: FormActionTypeType,  # (2)
    fields: Mapping[str, FieldConfigTypeDef],  # (3)
    style: FormStyleTypeDef,  # (4)
    sectionalElements: Mapping[str, SectionalElementTypeDef],  # (5)
    schemaVersion: str,
    cta: NotRequired[FormCTATypeDef],  # (6)
    tags: NotRequired[Mapping[str, str]],
    labelDecorator: NotRequired[LabelDecoratorType],  # (7)
```

1. See [:material-code-braces: FormDataTypeConfigTypeDef](./type_defs.md#formdatatypeconfigtypedef) 
2. See [:material-code-brackets: FormActionTypeType](./literals.md#formactiontypetype) 
3. See [:material-code-braces: FieldConfigTypeDef](./type_defs.md#fieldconfigtypedef) 
4. See [:material-code-braces: FormStyleTypeDef](./type_defs.md#formstyletypedef) 
5. See [:material-code-braces: SectionalElementTypeDef](./type_defs.md#sectionalelementtypedef) 
6. See [:material-code-braces: FormCTATypeDef](./type_defs.md#formctatypedef) 
7. See [:material-code-brackets: LabelDecoratorType](./literals.md#labeldecoratortype) 
## FormTypeDef

```python
# FormTypeDef definition

class FormTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
    name: str,
    formActionType: FormActionTypeType,  # (1)
    style: FormStyleTypeDef,  # (2)
    dataType: FormDataTypeConfigTypeDef,  # (3)
    fields: Dict[str, FieldConfigTypeDef],  # (4)
    sectionalElements: Dict[str, SectionalElementTypeDef],  # (5)
    schemaVersion: str,
    tags: NotRequired[Dict[str, str]],
    cta: NotRequired[FormCTATypeDef],  # (6)
    labelDecorator: NotRequired[LabelDecoratorType],  # (7)
```

1. See [:material-code-brackets: FormActionTypeType](./literals.md#formactiontypetype) 
2. See [:material-code-braces: FormStyleTypeDef](./type_defs.md#formstyletypedef) 
3. See [:material-code-braces: FormDataTypeConfigTypeDef](./type_defs.md#formdatatypeconfigtypedef) 
4. See [:material-code-braces: FieldConfigTypeDef](./type_defs.md#fieldconfigtypedef) 
5. See [:material-code-braces: SectionalElementTypeDef](./type_defs.md#sectionalelementtypedef) 
6. See [:material-code-braces: FormCTATypeDef](./type_defs.md#formctatypedef) 
7. See [:material-code-brackets: LabelDecoratorType](./literals.md#labeldecoratortype) 
## UpdateFormDataTypeDef

```python
# UpdateFormDataTypeDef definition

class UpdateFormDataTypeDef(TypedDict):
    name: NotRequired[str],
    dataType: NotRequired[FormDataTypeConfigTypeDef],  # (1)
    formActionType: NotRequired[FormActionTypeType],  # (2)
    fields: NotRequired[Mapping[str, FieldConfigTypeDef]],  # (3)
    style: NotRequired[FormStyleTypeDef],  # (4)
    sectionalElements: NotRequired[Mapping[str, SectionalElementTypeDef]],  # (5)
    schemaVersion: NotRequired[str],
    cta: NotRequired[FormCTATypeDef],  # (6)
    labelDecorator: NotRequired[LabelDecoratorType],  # (7)
```

1. See [:material-code-braces: FormDataTypeConfigTypeDef](./type_defs.md#formdatatypeconfigtypedef) 
2. See [:material-code-brackets: FormActionTypeType](./literals.md#formactiontypetype) 
3. See [:material-code-braces: FieldConfigTypeDef](./type_defs.md#fieldconfigtypedef) 
4. See [:material-code-braces: FormStyleTypeDef](./type_defs.md#formstyletypedef) 
5. See [:material-code-braces: SectionalElementTypeDef](./type_defs.md#sectionalelementtypedef) 
6. See [:material-code-braces: FormCTATypeDef](./type_defs.md#formctatypedef) 
7. See [:material-code-brackets: LabelDecoratorType](./literals.md#labeldecoratortype) 
## CreateFormRequestRequestTypeDef

```python
# CreateFormRequestRequestTypeDef definition

class CreateFormRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    formToCreate: CreateFormDataTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: CreateFormDataTypeDef](./type_defs.md#createformdatatypedef) 
## CreateFormResponseTypeDef

```python
# CreateFormResponseTypeDef definition

class CreateFormResponseTypeDef(TypedDict):
    entity: FormTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FormTypeDef](./type_defs.md#formtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportFormsResponseTypeDef

```python
# ExportFormsResponseTypeDef definition

class ExportFormsResponseTypeDef(TypedDict):
    entities: List[FormTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FormTypeDef](./type_defs.md#formtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFormResponseTypeDef

```python
# GetFormResponseTypeDef definition

class GetFormResponseTypeDef(TypedDict):
    form: FormTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FormTypeDef](./type_defs.md#formtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFormResponseTypeDef

```python
# UpdateFormResponseTypeDef definition

class UpdateFormResponseTypeDef(TypedDict):
    entity: FormTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FormTypeDef](./type_defs.md#formtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFormRequestRequestTypeDef

```python
# UpdateFormRequestRequestTypeDef definition

class UpdateFormRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    id: str,
    updatedForm: UpdateFormDataTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: UpdateFormDataTypeDef](./type_defs.md#updateformdatatypedef) 
