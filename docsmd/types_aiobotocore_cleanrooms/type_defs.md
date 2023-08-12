# Type definitions

> [Index](../README.md) > [CleanRoomsService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CleanRoomsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
    type annotations stubs module [types-aiobotocore-cleanrooms](https://pypi.org/project/types-aiobotocore-cleanrooms/).



## AggregateColumnTypeDef

```python
# AggregateColumnTypeDef definition

class AggregateColumnTypeDef(TypedDict):
    columnNames: Sequence[str],
    function: AggregateFunctionNameType,  # (1)
```

1. See [:material-code-brackets: AggregateFunctionNameType](./literals.md#aggregatefunctionnametype) 
## AggregationConstraintTypeDef

```python
# AggregationConstraintTypeDef definition

class AggregationConstraintTypeDef(TypedDict):
    columnName: str,
    minimum: int,
    type: AggregationTypeType,  # (1)
```

1. See [:material-code-brackets: AggregationTypeType](./literals.md#aggregationtypetype) 
## AnalysisParameterTypeDef

```python
# AnalysisParameterTypeDef definition

class AnalysisParameterTypeDef(TypedDict):
    name: str,
    type: ParameterTypeType,  # (1)
    defaultValue: NotRequired[str],
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
## AnalysisRuleCustomTypeDef

```python
# AnalysisRuleCustomTypeDef definition

class AnalysisRuleCustomTypeDef(TypedDict):
    allowedAnalyses: Sequence[str],
    allowedAnalysisProviders: NotRequired[Sequence[str]],
```

## AnalysisRuleListTypeDef

```python
# AnalysisRuleListTypeDef definition

class AnalysisRuleListTypeDef(TypedDict):
    joinColumns: Sequence[str],
    listColumns: Sequence[str],
    allowedJoinOperators: NotRequired[Sequence[JoinOperatorType]],  # (1)
```

1. See [:material-code-brackets: JoinOperatorType](./literals.md#joinoperatortype) 
## AnalysisSchemaTypeDef

```python
# AnalysisSchemaTypeDef definition

class AnalysisSchemaTypeDef(TypedDict):
    referencedTables: NotRequired[List[str]],
```

## AnalysisSourceTypeDef

```python
# AnalysisSourceTypeDef definition

class AnalysisSourceTypeDef(TypedDict):
    text: NotRequired[str],
```

## AnalysisTemplateSummaryTypeDef

```python
# AnalysisTemplateSummaryTypeDef definition

class AnalysisTemplateSummaryTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    id: str,
    name: str,
    updateTime: datetime,
    membershipArn: str,
    membershipId: str,
    collaborationArn: str,
    collaborationId: str,
    description: NotRequired[str],
```

## BatchGetCollaborationAnalysisTemplateErrorTypeDef

```python
# BatchGetCollaborationAnalysisTemplateErrorTypeDef definition

class BatchGetCollaborationAnalysisTemplateErrorTypeDef(TypedDict):
    arn: str,
    code: str,
    message: str,
```

## BatchGetCollaborationAnalysisTemplateInputRequestTypeDef

```python
# BatchGetCollaborationAnalysisTemplateInputRequestTypeDef definition

class BatchGetCollaborationAnalysisTemplateInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    analysisTemplateArns: Sequence[str],
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

## BatchGetSchemaErrorTypeDef

```python
# BatchGetSchemaErrorTypeDef definition

class BatchGetSchemaErrorTypeDef(TypedDict):
    name: str,
    code: str,
    message: str,
```

## BatchGetSchemaInputRequestTypeDef

```python
# BatchGetSchemaInputRequestTypeDef definition

class BatchGetSchemaInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    names: Sequence[str],
```

## CollaborationAnalysisTemplateSummaryTypeDef

```python
# CollaborationAnalysisTemplateSummaryTypeDef definition

class CollaborationAnalysisTemplateSummaryTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    id: str,
    name: str,
    updateTime: datetime,
    collaborationArn: str,
    collaborationId: str,
    creatorAccountId: str,
    description: NotRequired[str],
```

## CollaborationSummaryTypeDef

```python
# CollaborationSummaryTypeDef definition

class CollaborationSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    creatorAccountId: str,
    creatorDisplayName: str,
    createTime: datetime,
    updateTime: datetime,
    memberStatus: MemberStatusType,  # (1)
    membershipId: NotRequired[str],
    membershipArn: NotRequired[str],
```

1. See [:material-code-brackets: MemberStatusType](./literals.md#memberstatustype) 
## DataEncryptionMetadataTypeDef

```python
# DataEncryptionMetadataTypeDef definition

class DataEncryptionMetadataTypeDef(TypedDict):
    allowCleartext: bool,
    allowDuplicates: bool,
    allowJoinsOnColumnsWithDifferentNames: bool,
    preserveNulls: bool,
```

## ColumnTypeDef

```python
# ColumnTypeDef definition

class ColumnTypeDef(TypedDict):
    name: str,
    type: str,
```

## ConfiguredTableAssociationSummaryTypeDef

```python
# ConfiguredTableAssociationSummaryTypeDef definition

class ConfiguredTableAssociationSummaryTypeDef(TypedDict):
    configuredTableId: str,
    membershipId: str,
    membershipArn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    id: str,
    arn: str,
```

## ConfiguredTableAssociationTypeDef

```python
# ConfiguredTableAssociationTypeDef definition

class ConfiguredTableAssociationTypeDef(TypedDict):
    arn: str,
    id: str,
    configuredTableId: str,
    configuredTableArn: str,
    membershipId: str,
    membershipArn: str,
    roleArn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    description: NotRequired[str],
```

## ConfiguredTableSummaryTypeDef

```python
# ConfiguredTableSummaryTypeDef definition

class ConfiguredTableSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    analysisRuleTypes: List[ConfiguredTableAnalysisRuleTypeType],  # (1)
    analysisMethod: AnalysisMethodType,  # (2)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
## MemberSpecificationTypeDef

```python
# MemberSpecificationTypeDef definition

class MemberSpecificationTypeDef(TypedDict):
    accountId: str,
    memberAbilities: Sequence[MemberAbilityType],  # (1)
    displayName: str,
```

1. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
## CreateConfiguredTableAssociationInputRequestTypeDef

```python
# CreateConfiguredTableAssociationInputRequestTypeDef definition

class CreateConfiguredTableAssociationInputRequestTypeDef(TypedDict):
    name: str,
    membershipIdentifier: str,
    configuredTableIdentifier: str,
    roleArn: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CreateMembershipInputRequestTypeDef

```python
# CreateMembershipInputRequestTypeDef definition

class CreateMembershipInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    queryLogStatus: MembershipQueryLogStatusType,  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype) 
## MembershipTypeDef

```python
# MembershipTypeDef definition

class MembershipTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationArn: str,
    collaborationId: str,
    collaborationCreatorAccountId: str,
    collaborationCreatorDisplayName: str,
    collaborationName: str,
    createTime: datetime,
    updateTime: datetime,
    status: MembershipStatusType,  # (1)
    memberAbilities: List[MemberAbilityType],  # (2)
    queryLogStatus: MembershipQueryLogStatusType,  # (3)
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
3. See [:material-code-brackets: MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype) 
## DeleteAnalysisTemplateInputRequestTypeDef

```python
# DeleteAnalysisTemplateInputRequestTypeDef definition

class DeleteAnalysisTemplateInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    analysisTemplateIdentifier: str,
```

## DeleteCollaborationInputRequestTypeDef

```python
# DeleteCollaborationInputRequestTypeDef definition

class DeleteCollaborationInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
```

## DeleteConfiguredTableAnalysisRuleInputRequestTypeDef

```python
# DeleteConfiguredTableAnalysisRuleInputRequestTypeDef definition

class DeleteConfiguredTableAnalysisRuleInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
## DeleteConfiguredTableAssociationInputRequestTypeDef

```python
# DeleteConfiguredTableAssociationInputRequestTypeDef definition

class DeleteConfiguredTableAssociationInputRequestTypeDef(TypedDict):
    configuredTableAssociationIdentifier: str,
    membershipIdentifier: str,
```

## DeleteConfiguredTableInputRequestTypeDef

```python
# DeleteConfiguredTableInputRequestTypeDef definition

class DeleteConfiguredTableInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
```

## DeleteMemberInputRequestTypeDef

```python
# DeleteMemberInputRequestTypeDef definition

class DeleteMemberInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    accountId: str,
```

## DeleteMembershipInputRequestTypeDef

```python
# DeleteMembershipInputRequestTypeDef definition

class DeleteMembershipInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
```

## GetAnalysisTemplateInputRequestTypeDef

```python
# GetAnalysisTemplateInputRequestTypeDef definition

class GetAnalysisTemplateInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    analysisTemplateIdentifier: str,
```

## GetCollaborationAnalysisTemplateInputRequestTypeDef

```python
# GetCollaborationAnalysisTemplateInputRequestTypeDef definition

class GetCollaborationAnalysisTemplateInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    analysisTemplateArn: str,
```

## GetCollaborationInputRequestTypeDef

```python
# GetCollaborationInputRequestTypeDef definition

class GetCollaborationInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
```

## GetConfiguredTableAnalysisRuleInputRequestTypeDef

```python
# GetConfiguredTableAnalysisRuleInputRequestTypeDef definition

class GetConfiguredTableAnalysisRuleInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
## GetConfiguredTableAssociationInputRequestTypeDef

```python
# GetConfiguredTableAssociationInputRequestTypeDef definition

class GetConfiguredTableAssociationInputRequestTypeDef(TypedDict):
    configuredTableAssociationIdentifier: str,
    membershipIdentifier: str,
```

## GetConfiguredTableInputRequestTypeDef

```python
# GetConfiguredTableInputRequestTypeDef definition

class GetConfiguredTableInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
```

## GetMembershipInputRequestTypeDef

```python
# GetMembershipInputRequestTypeDef definition

class GetMembershipInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
```

## GetProtectedQueryInputRequestTypeDef

```python
# GetProtectedQueryInputRequestTypeDef definition

class GetProtectedQueryInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    protectedQueryIdentifier: str,
```

## GetSchemaAnalysisRuleInputRequestTypeDef

```python
# GetSchemaAnalysisRuleInputRequestTypeDef definition

class GetSchemaAnalysisRuleInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    name: str,
    type: AnalysisRuleTypeType,  # (1)
```

1. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
## GetSchemaInputRequestTypeDef

```python
# GetSchemaInputRequestTypeDef definition

class GetSchemaInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    name: str,
```

## GlueTableReferenceTypeDef

```python
# GlueTableReferenceTypeDef definition

class GlueTableReferenceTypeDef(TypedDict):
    tableName: str,
    databaseName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAnalysisTemplatesInputRequestTypeDef

```python
# ListAnalysisTemplatesInputRequestTypeDef definition

class ListAnalysisTemplatesInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationAnalysisTemplatesInputRequestTypeDef

```python
# ListCollaborationAnalysisTemplatesInputRequestTypeDef definition

class ListCollaborationAnalysisTemplatesInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationsInputRequestTypeDef

```python
# ListCollaborationsInputRequestTypeDef definition

class ListCollaborationsInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    memberStatus: NotRequired[FilterableMemberStatusType],  # (1)
```

1. See [:material-code-brackets: FilterableMemberStatusType](./literals.md#filterablememberstatustype) 
## ListConfiguredTableAssociationsInputRequestTypeDef

```python
# ListConfiguredTableAssociationsInputRequestTypeDef definition

class ListConfiguredTableAssociationsInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListConfiguredTablesInputRequestTypeDef

```python
# ListConfiguredTablesInputRequestTypeDef definition

class ListConfiguredTablesInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListMembersInputRequestTypeDef

```python
# ListMembersInputRequestTypeDef definition

class ListMembersInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## MemberSummaryTypeDef

```python
# MemberSummaryTypeDef definition

class MemberSummaryTypeDef(TypedDict):
    accountId: str,
    status: MemberStatusType,  # (1)
    displayName: str,
    abilities: List[MemberAbilityType],  # (2)
    createTime: datetime,
    updateTime: datetime,
    membershipId: NotRequired[str],
    membershipArn: NotRequired[str],
```

1. See [:material-code-brackets: MemberStatusType](./literals.md#memberstatustype) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
## ListMembershipsInputRequestTypeDef

```python
# ListMembershipsInputRequestTypeDef definition

class ListMembershipsInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    status: NotRequired[MembershipStatusType],  # (1)
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
## MembershipSummaryTypeDef

```python
# MembershipSummaryTypeDef definition

class MembershipSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationArn: str,
    collaborationId: str,
    collaborationCreatorAccountId: str,
    collaborationCreatorDisplayName: str,
    collaborationName: str,
    createTime: datetime,
    updateTime: datetime,
    status: MembershipStatusType,  # (1)
    memberAbilities: List[MemberAbilityType],  # (2)
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
## ListProtectedQueriesInputRequestTypeDef

```python
# ListProtectedQueriesInputRequestTypeDef definition

class ListProtectedQueriesInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    status: NotRequired[ProtectedQueryStatusType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype) 
## ProtectedQuerySummaryTypeDef

```python
# ProtectedQuerySummaryTypeDef definition

class ProtectedQuerySummaryTypeDef(TypedDict):
    id: str,
    membershipId: str,
    membershipArn: str,
    createTime: datetime,
    status: ProtectedQueryStatusType,  # (1)
```

1. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype) 
## ListSchemasInputRequestTypeDef

```python
# ListSchemasInputRequestTypeDef definition

class ListSchemasInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    schemaType: NotRequired[SchemaTypeType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype) 
## SchemaSummaryTypeDef

```python
# SchemaSummaryTypeDef definition

class SchemaSummaryTypeDef(TypedDict):
    name: str,
    type: SchemaTypeType,  # (1)
    creatorAccountId: str,
    createTime: datetime,
    updateTime: datetime,
    collaborationId: str,
    collaborationArn: str,
    analysisRuleTypes: List[AnalysisRuleTypeType],  # (2)
    analysisMethod: NotRequired[AnalysisMethodType],  # (3)
```

1. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype) 
2. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
3. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ProtectedQueryErrorTypeDef

```python
# ProtectedQueryErrorTypeDef definition

class ProtectedQueryErrorTypeDef(TypedDict):
    message: str,
    code: str,
```

## ProtectedQueryS3OutputConfigurationTypeDef

```python
# ProtectedQueryS3OutputConfigurationTypeDef definition

class ProtectedQueryS3OutputConfigurationTypeDef(TypedDict):
    resultFormat: ResultFormatType,  # (1)
    bucket: str,
    keyPrefix: NotRequired[str],
```

1. See [:material-code-brackets: ResultFormatType](./literals.md#resultformattype) 
## ProtectedQueryS3OutputTypeDef

```python
# ProtectedQueryS3OutputTypeDef definition

class ProtectedQueryS3OutputTypeDef(TypedDict):
    location: str,
```

## ProtectedQuerySQLParametersTypeDef

```python
# ProtectedQuerySQLParametersTypeDef definition

class ProtectedQuerySQLParametersTypeDef(TypedDict):
    queryString: NotRequired[str],
    analysisTemplateArn: NotRequired[str],
    parameters: NotRequired[Dict[str, str]],
```

## ProtectedQueryStatisticsTypeDef

```python
# ProtectedQueryStatisticsTypeDef definition

class ProtectedQueryStatisticsTypeDef(TypedDict):
    totalDurationInMillis: NotRequired[int],
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAnalysisTemplateInputRequestTypeDef

```python
# UpdateAnalysisTemplateInputRequestTypeDef definition

class UpdateAnalysisTemplateInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    analysisTemplateIdentifier: str,
    description: NotRequired[str],
```

## UpdateCollaborationInputRequestTypeDef

```python
# UpdateCollaborationInputRequestTypeDef definition

class UpdateCollaborationInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    name: NotRequired[str],
    description: NotRequired[str],
```

## UpdateConfiguredTableAssociationInputRequestTypeDef

```python
# UpdateConfiguredTableAssociationInputRequestTypeDef definition

class UpdateConfiguredTableAssociationInputRequestTypeDef(TypedDict):
    configuredTableAssociationIdentifier: str,
    membershipIdentifier: str,
    description: NotRequired[str],
    roleArn: NotRequired[str],
```

## UpdateConfiguredTableInputRequestTypeDef

```python
# UpdateConfiguredTableInputRequestTypeDef definition

class UpdateConfiguredTableInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
    name: NotRequired[str],
    description: NotRequired[str],
```

## UpdateMembershipInputRequestTypeDef

```python
# UpdateMembershipInputRequestTypeDef definition

class UpdateMembershipInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    queryLogStatus: NotRequired[MembershipQueryLogStatusType],  # (1)
```

1. See [:material-code-brackets: MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype) 
## UpdateProtectedQueryInputRequestTypeDef

```python
# UpdateProtectedQueryInputRequestTypeDef definition

class UpdateProtectedQueryInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    protectedQueryIdentifier: str,
    targetStatus: TargetProtectedQueryStatusType,  # (1)
```

1. See [:material-code-brackets: TargetProtectedQueryStatusType](./literals.md#targetprotectedquerystatustype) 
## AnalysisRuleAggregationTypeDef

```python
# AnalysisRuleAggregationTypeDef definition

class AnalysisRuleAggregationTypeDef(TypedDict):
    aggregateColumns: Sequence[AggregateColumnTypeDef],  # (1)
    joinColumns: Sequence[str],
    dimensionColumns: Sequence[str],
    scalarFunctions: Sequence[ScalarFunctionsType],  # (4)
    outputConstraints: Sequence[AggregationConstraintTypeDef],  # (5)
    joinRequired: NotRequired[JoinRequiredOptionType],  # (2)
    allowedJoinOperators: NotRequired[Sequence[JoinOperatorType]],  # (3)
```

1. See [:material-code-braces: AggregateColumnTypeDef](./type_defs.md#aggregatecolumntypedef) 
2. See [:material-code-brackets: JoinRequiredOptionType](./literals.md#joinrequiredoptiontype) 
3. See [:material-code-brackets: JoinOperatorType](./literals.md#joinoperatortype) 
4. See [:material-code-brackets: ScalarFunctionsType](./literals.md#scalarfunctionstype) 
5. See [:material-code-braces: AggregationConstraintTypeDef](./type_defs.md#aggregationconstrainttypedef) 
## AnalysisTemplateTypeDef

```python
# AnalysisTemplateTypeDef definition

class AnalysisTemplateTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationId: str,
    collaborationArn: str,
    membershipId: str,
    membershipArn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    schema: AnalysisSchemaTypeDef,  # (1)
    format: AnalysisFormatType,  # (2)
    source: AnalysisSourceTypeDef,  # (3)
    description: NotRequired[str],
    analysisParameters: NotRequired[List[AnalysisParameterTypeDef]],  # (4)
```

1. See [:material-code-braces: AnalysisSchemaTypeDef](./type_defs.md#analysisschematypedef) 
2. See [:material-code-brackets: AnalysisFormatType](./literals.md#analysisformattype) 
3. See [:material-code-braces: AnalysisSourceTypeDef](./type_defs.md#analysissourcetypedef) 
4. See [:material-code-braces: AnalysisParameterTypeDef](./type_defs.md#analysisparametertypedef) 
## CollaborationAnalysisTemplateTypeDef

```python
# CollaborationAnalysisTemplateTypeDef definition

class CollaborationAnalysisTemplateTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationId: str,
    collaborationArn: str,
    creatorAccountId: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    schema: AnalysisSchemaTypeDef,  # (1)
    format: AnalysisFormatType,  # (2)
    source: AnalysisSourceTypeDef,  # (3)
    description: NotRequired[str],
    analysisParameters: NotRequired[List[AnalysisParameterTypeDef]],  # (4)
```

1. See [:material-code-braces: AnalysisSchemaTypeDef](./type_defs.md#analysisschematypedef) 
2. See [:material-code-brackets: AnalysisFormatType](./literals.md#analysisformattype) 
3. See [:material-code-braces: AnalysisSourceTypeDef](./type_defs.md#analysissourcetypedef) 
4. See [:material-code-braces: AnalysisParameterTypeDef](./type_defs.md#analysisparametertypedef) 
## CreateAnalysisTemplateInputRequestTypeDef

```python
# CreateAnalysisTemplateInputRequestTypeDef definition

class CreateAnalysisTemplateInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    name: str,
    format: AnalysisFormatType,  # (1)
    source: AnalysisSourceTypeDef,  # (2)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    analysisParameters: NotRequired[Sequence[AnalysisParameterTypeDef]],  # (3)
```

1. See [:material-code-brackets: AnalysisFormatType](./literals.md#analysisformattype) 
2. See [:material-code-braces: AnalysisSourceTypeDef](./type_defs.md#analysissourcetypedef) 
3. See [:material-code-braces: AnalysisParameterTypeDef](./type_defs.md#analysisparametertypedef) 
## ListAnalysisTemplatesOutputTypeDef

```python
# ListAnalysisTemplatesOutputTypeDef definition

class ListAnalysisTemplatesOutputTypeDef(TypedDict):
    nextToken: str,
    analysisTemplateSummaries: List[AnalysisTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisTemplateSummaryTypeDef](./type_defs.md#analysistemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollaborationAnalysisTemplatesOutputTypeDef

```python
# ListCollaborationAnalysisTemplatesOutputTypeDef definition

class ListCollaborationAnalysisTemplatesOutputTypeDef(TypedDict):
    nextToken: str,
    collaborationAnalysisTemplateSummaries: List[CollaborationAnalysisTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationAnalysisTemplateSummaryTypeDef](./type_defs.md#collaborationanalysistemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollaborationsOutputTypeDef

```python
# ListCollaborationsOutputTypeDef definition

class ListCollaborationsOutputTypeDef(TypedDict):
    nextToken: str,
    collaborationList: List[CollaborationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationSummaryTypeDef](./type_defs.md#collaborationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CollaborationTypeDef

```python
# CollaborationTypeDef definition

class CollaborationTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    creatorAccountId: str,
    creatorDisplayName: str,
    createTime: datetime,
    updateTime: datetime,
    memberStatus: MemberStatusType,  # (1)
    queryLogStatus: CollaborationQueryLogStatusType,  # (3)
    description: NotRequired[str],
    membershipId: NotRequired[str],
    membershipArn: NotRequired[str],
    dataEncryptionMetadata: NotRequired[DataEncryptionMetadataTypeDef],  # (2)
```

1. See [:material-code-brackets: MemberStatusType](./literals.md#memberstatustype) 
2. See [:material-code-braces: DataEncryptionMetadataTypeDef](./type_defs.md#dataencryptionmetadatatypedef) 
3. See [:material-code-brackets: CollaborationQueryLogStatusType](./literals.md#collaborationquerylogstatustype) 
## SchemaTypeDef

```python
# SchemaTypeDef definition

class SchemaTypeDef(TypedDict):
    columns: List[ColumnTypeDef],  # (1)
    partitionKeys: List[ColumnTypeDef],  # (1)
    analysisRuleTypes: List[AnalysisRuleTypeType],  # (3)
    creatorAccountId: str,
    name: str,
    collaborationId: str,
    collaborationArn: str,
    description: str,
    createTime: datetime,
    updateTime: datetime,
    type: SchemaTypeType,  # (5)
    analysisMethod: NotRequired[AnalysisMethodType],  # (4)
```

1. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
2. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
3. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
4. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
5. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype) 
## ListConfiguredTableAssociationsOutputTypeDef

```python
# ListConfiguredTableAssociationsOutputTypeDef definition

class ListConfiguredTableAssociationsOutputTypeDef(TypedDict):
    configuredTableAssociationSummaries: List[ConfiguredTableAssociationSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationSummaryTypeDef](./type_defs.md#configuredtableassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredTableAssociationOutputTypeDef

```python
# CreateConfiguredTableAssociationOutputTypeDef definition

class CreateConfiguredTableAssociationOutputTypeDef(TypedDict):
    configuredTableAssociation: ConfiguredTableAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationTypeDef](./type_defs.md#configuredtableassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredTableAssociationOutputTypeDef

```python
# GetConfiguredTableAssociationOutputTypeDef definition

class GetConfiguredTableAssociationOutputTypeDef(TypedDict):
    configuredTableAssociation: ConfiguredTableAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationTypeDef](./type_defs.md#configuredtableassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredTableAssociationOutputTypeDef

```python
# UpdateConfiguredTableAssociationOutputTypeDef definition

class UpdateConfiguredTableAssociationOutputTypeDef(TypedDict):
    configuredTableAssociation: ConfiguredTableAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationTypeDef](./type_defs.md#configuredtableassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfiguredTablesOutputTypeDef

```python
# ListConfiguredTablesOutputTypeDef definition

class ListConfiguredTablesOutputTypeDef(TypedDict):
    configuredTableSummaries: List[ConfiguredTableSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableSummaryTypeDef](./type_defs.md#configuredtablesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCollaborationInputRequestTypeDef

```python
# CreateCollaborationInputRequestTypeDef definition

class CreateCollaborationInputRequestTypeDef(TypedDict):
    members: Sequence[MemberSpecificationTypeDef],  # (1)
    name: str,
    description: str,
    creatorMemberAbilities: Sequence[MemberAbilityType],  # (2)
    creatorDisplayName: str,
    queryLogStatus: CollaborationQueryLogStatusType,  # (3)
    dataEncryptionMetadata: NotRequired[DataEncryptionMetadataTypeDef],  # (4)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: MemberSpecificationTypeDef](./type_defs.md#memberspecificationtypedef) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
3. See [:material-code-brackets: CollaborationQueryLogStatusType](./literals.md#collaborationquerylogstatustype) 
4. See [:material-code-braces: DataEncryptionMetadataTypeDef](./type_defs.md#dataencryptionmetadatatypedef) 
## CreateMembershipOutputTypeDef

```python
# CreateMembershipOutputTypeDef definition

class CreateMembershipOutputTypeDef(TypedDict):
    membership: MembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MembershipTypeDef](./type_defs.md#membershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMembershipOutputTypeDef

```python
# GetMembershipOutputTypeDef definition

class GetMembershipOutputTypeDef(TypedDict):
    membership: MembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MembershipTypeDef](./type_defs.md#membershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMembershipOutputTypeDef

```python
# UpdateMembershipOutputTypeDef definition

class UpdateMembershipOutputTypeDef(TypedDict):
    membership: MembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MembershipTypeDef](./type_defs.md#membershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TableReferenceTypeDef

```python
# TableReferenceTypeDef definition

class TableReferenceTypeDef(TypedDict):
    glue: NotRequired[GlueTableReferenceTypeDef],  # (1)
```

1. See [:material-code-braces: GlueTableReferenceTypeDef](./type_defs.md#gluetablereferencetypedef) 
## ListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef

```python
# ListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef definition

class ListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef

```python
# ListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef definition

class ListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationsInputListCollaborationsPaginateTypeDef

```python
# ListCollaborationsInputListCollaborationsPaginateTypeDef definition

class ListCollaborationsInputListCollaborationsPaginateTypeDef(TypedDict):
    memberStatus: NotRequired[FilterableMemberStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FilterableMemberStatusType](./literals.md#filterablememberstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef

```python
# ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef definition

class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef

```python
# ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef definition

class ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembersInputListMembersPaginateTypeDef

```python
# ListMembersInputListMembersPaginateTypeDef definition

class ListMembersInputListMembersPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembershipsInputListMembershipsPaginateTypeDef

```python
# ListMembershipsInputListMembershipsPaginateTypeDef definition

class ListMembershipsInputListMembershipsPaginateTypeDef(TypedDict):
    status: NotRequired[MembershipStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef

```python
# ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef definition

class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    status: NotRequired[ProtectedQueryStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchemasInputListSchemasPaginateTypeDef

```python
# ListSchemasInputListSchemasPaginateTypeDef definition

class ListSchemasInputListSchemasPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    schemaType: NotRequired[SchemaTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembersOutputTypeDef

```python
# ListMembersOutputTypeDef definition

class ListMembersOutputTypeDef(TypedDict):
    nextToken: str,
    memberSummaries: List[MemberSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberSummaryTypeDef](./type_defs.md#membersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMembershipsOutputTypeDef

```python
# ListMembershipsOutputTypeDef definition

class ListMembershipsOutputTypeDef(TypedDict):
    nextToken: str,
    membershipSummaries: List[MembershipSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MembershipSummaryTypeDef](./type_defs.md#membershipsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProtectedQueriesOutputTypeDef

```python
# ListProtectedQueriesOutputTypeDef definition

class ListProtectedQueriesOutputTypeDef(TypedDict):
    nextToken: str,
    protectedQueries: List[ProtectedQuerySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectedQuerySummaryTypeDef](./type_defs.md#protectedquerysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSchemasOutputTypeDef

```python
# ListSchemasOutputTypeDef definition

class ListSchemasOutputTypeDef(TypedDict):
    schemaSummaries: List[SchemaSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaSummaryTypeDef](./type_defs.md#schemasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProtectedQueryOutputConfigurationTypeDef

```python
# ProtectedQueryOutputConfigurationTypeDef definition

class ProtectedQueryOutputConfigurationTypeDef(TypedDict):
    s3: NotRequired[ProtectedQueryS3OutputConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ProtectedQueryS3OutputConfigurationTypeDef](./type_defs.md#protectedquerys3outputconfigurationtypedef) 
## ProtectedQueryOutputTypeDef

```python
# ProtectedQueryOutputTypeDef definition

class ProtectedQueryOutputTypeDef(TypedDict):
    s3: NotRequired[ProtectedQueryS3OutputTypeDef],  # (1)
```

1. See [:material-code-braces: ProtectedQueryS3OutputTypeDef](./type_defs.md#protectedquerys3outputtypedef) 
## AnalysisRulePolicyV1TypeDef

```python
# AnalysisRulePolicyV1TypeDef definition

class AnalysisRulePolicyV1TypeDef(TypedDict):
    list: NotRequired[AnalysisRuleListTypeDef],  # (1)
    aggregation: NotRequired[AnalysisRuleAggregationTypeDef],  # (2)
    custom: NotRequired[AnalysisRuleCustomTypeDef],  # (3)
```

1. See [:material-code-braces: AnalysisRuleListTypeDef](./type_defs.md#analysisrulelisttypedef) 
2. See [:material-code-braces: AnalysisRuleAggregationTypeDef](./type_defs.md#analysisruleaggregationtypedef) 
3. See [:material-code-braces: AnalysisRuleCustomTypeDef](./type_defs.md#analysisrulecustomtypedef) 
## ConfiguredTableAnalysisRulePolicyV1TypeDef

```python
# ConfiguredTableAnalysisRulePolicyV1TypeDef definition

class ConfiguredTableAnalysisRulePolicyV1TypeDef(TypedDict):
    list: NotRequired[AnalysisRuleListTypeDef],  # (1)
    aggregation: NotRequired[AnalysisRuleAggregationTypeDef],  # (2)
    custom: NotRequired[AnalysisRuleCustomTypeDef],  # (3)
```

1. See [:material-code-braces: AnalysisRuleListTypeDef](./type_defs.md#analysisrulelisttypedef) 
2. See [:material-code-braces: AnalysisRuleAggregationTypeDef](./type_defs.md#analysisruleaggregationtypedef) 
3. See [:material-code-braces: AnalysisRuleCustomTypeDef](./type_defs.md#analysisrulecustomtypedef) 
## CreateAnalysisTemplateOutputTypeDef

```python
# CreateAnalysisTemplateOutputTypeDef definition

class CreateAnalysisTemplateOutputTypeDef(TypedDict):
    analysisTemplate: AnalysisTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisTemplateTypeDef](./type_defs.md#analysistemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAnalysisTemplateOutputTypeDef

```python
# GetAnalysisTemplateOutputTypeDef definition

class GetAnalysisTemplateOutputTypeDef(TypedDict):
    analysisTemplate: AnalysisTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisTemplateTypeDef](./type_defs.md#analysistemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAnalysisTemplateOutputTypeDef

```python
# UpdateAnalysisTemplateOutputTypeDef definition

class UpdateAnalysisTemplateOutputTypeDef(TypedDict):
    analysisTemplate: AnalysisTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisTemplateTypeDef](./type_defs.md#analysistemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetCollaborationAnalysisTemplateOutputTypeDef

```python
# BatchGetCollaborationAnalysisTemplateOutputTypeDef definition

class BatchGetCollaborationAnalysisTemplateOutputTypeDef(TypedDict):
    collaborationAnalysisTemplates: List[CollaborationAnalysisTemplateTypeDef],  # (1)
    errors: List[BatchGetCollaborationAnalysisTemplateErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CollaborationAnalysisTemplateTypeDef](./type_defs.md#collaborationanalysistemplatetypedef) 
2. See [:material-code-braces: BatchGetCollaborationAnalysisTemplateErrorTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCollaborationAnalysisTemplateOutputTypeDef

```python
# GetCollaborationAnalysisTemplateOutputTypeDef definition

class GetCollaborationAnalysisTemplateOutputTypeDef(TypedDict):
    collaborationAnalysisTemplate: CollaborationAnalysisTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationAnalysisTemplateTypeDef](./type_defs.md#collaborationanalysistemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCollaborationOutputTypeDef

```python
# CreateCollaborationOutputTypeDef definition

class CreateCollaborationOutputTypeDef(TypedDict):
    collaboration: CollaborationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationTypeDef](./type_defs.md#collaborationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCollaborationOutputTypeDef

```python
# GetCollaborationOutputTypeDef definition

class GetCollaborationOutputTypeDef(TypedDict):
    collaboration: CollaborationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationTypeDef](./type_defs.md#collaborationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCollaborationOutputTypeDef

```python
# UpdateCollaborationOutputTypeDef definition

class UpdateCollaborationOutputTypeDef(TypedDict):
    collaboration: CollaborationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationTypeDef](./type_defs.md#collaborationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetSchemaOutputTypeDef

```python
# BatchGetSchemaOutputTypeDef definition

class BatchGetSchemaOutputTypeDef(TypedDict):
    schemas: List[SchemaTypeDef],  # (1)
    errors: List[BatchGetSchemaErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SchemaTypeDef](./type_defs.md#schematypedef) 
2. See [:material-code-braces: BatchGetSchemaErrorTypeDef](./type_defs.md#batchgetschemaerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaOutputTypeDef

```python
# GetSchemaOutputTypeDef definition

class GetSchemaOutputTypeDef(TypedDict):
    schema: SchemaTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaTypeDef](./type_defs.md#schematypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfiguredTableTypeDef

```python
# ConfiguredTableTypeDef definition

class ConfiguredTableTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    tableReference: TableReferenceTypeDef,  # (1)
    createTime: datetime,
    updateTime: datetime,
    analysisRuleTypes: List[ConfiguredTableAnalysisRuleTypeType],  # (2)
    analysisMethod: AnalysisMethodType,  # (3)
    allowedColumns: List[str],
    description: NotRequired[str],
```

1. See [:material-code-braces: TableReferenceTypeDef](./type_defs.md#tablereferencetypedef) 
2. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
3. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
## CreateConfiguredTableInputRequestTypeDef

```python
# CreateConfiguredTableInputRequestTypeDef definition

class CreateConfiguredTableInputRequestTypeDef(TypedDict):
    name: str,
    tableReference: TableReferenceTypeDef,  # (1)
    allowedColumns: Sequence[str],
    analysisMethod: AnalysisMethodType,  # (2)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: TableReferenceTypeDef](./type_defs.md#tablereferencetypedef) 
2. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
## ProtectedQueryResultConfigurationTypeDef

```python
# ProtectedQueryResultConfigurationTypeDef definition

class ProtectedQueryResultConfigurationTypeDef(TypedDict):
    outputConfiguration: ProtectedQueryOutputConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: ProtectedQueryOutputConfigurationTypeDef](./type_defs.md#protectedqueryoutputconfigurationtypedef) 
## ProtectedQueryResultTypeDef

```python
# ProtectedQueryResultTypeDef definition

class ProtectedQueryResultTypeDef(TypedDict):
    output: ProtectedQueryOutputTypeDef,  # (1)
```

1. See [:material-code-braces: ProtectedQueryOutputTypeDef](./type_defs.md#protectedqueryoutputtypedef) 
## AnalysisRulePolicyTypeDef

```python
# AnalysisRulePolicyTypeDef definition

class AnalysisRulePolicyTypeDef(TypedDict):
    v1: NotRequired[AnalysisRulePolicyV1TypeDef],  # (1)
```

1. See [:material-code-braces: AnalysisRulePolicyV1TypeDef](./type_defs.md#analysisrulepolicyv1typedef) 
## ConfiguredTableAnalysisRulePolicyTypeDef

```python
# ConfiguredTableAnalysisRulePolicyTypeDef definition

class ConfiguredTableAnalysisRulePolicyTypeDef(TypedDict):
    v1: NotRequired[ConfiguredTableAnalysisRulePolicyV1TypeDef],  # (1)
```

1. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyV1TypeDef](./type_defs.md#configuredtableanalysisrulepolicyv1typedef) 
## CreateConfiguredTableOutputTypeDef

```python
# CreateConfiguredTableOutputTypeDef definition

class CreateConfiguredTableOutputTypeDef(TypedDict):
    configuredTable: ConfiguredTableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableTypeDef](./type_defs.md#configuredtabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredTableOutputTypeDef

```python
# GetConfiguredTableOutputTypeDef definition

class GetConfiguredTableOutputTypeDef(TypedDict):
    configuredTable: ConfiguredTableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableTypeDef](./type_defs.md#configuredtabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredTableOutputTypeDef

```python
# UpdateConfiguredTableOutputTypeDef definition

class UpdateConfiguredTableOutputTypeDef(TypedDict):
    configuredTable: ConfiguredTableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableTypeDef](./type_defs.md#configuredtabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartProtectedQueryInputRequestTypeDef

```python
# StartProtectedQueryInputRequestTypeDef definition

class StartProtectedQueryInputRequestTypeDef(TypedDict):
    type: ProtectedQueryTypeType,  # (1)
    membershipIdentifier: str,
    sqlParameters: ProtectedQuerySQLParametersTypeDef,  # (2)
    resultConfiguration: ProtectedQueryResultConfigurationTypeDef,  # (3)
```

1. See [:material-code-brackets: ProtectedQueryTypeType](./literals.md#protectedquerytypetype) 
2. See [:material-code-braces: ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef) 
3. See [:material-code-braces: ProtectedQueryResultConfigurationTypeDef](./type_defs.md#protectedqueryresultconfigurationtypedef) 
## ProtectedQueryTypeDef

```python
# ProtectedQueryTypeDef definition

class ProtectedQueryTypeDef(TypedDict):
    id: str,
    membershipId: str,
    membershipArn: str,
    createTime: datetime,
    sqlParameters: ProtectedQuerySQLParametersTypeDef,  # (1)
    status: ProtectedQueryStatusType,  # (2)
    resultConfiguration: ProtectedQueryResultConfigurationTypeDef,  # (3)
    statistics: NotRequired[ProtectedQueryStatisticsTypeDef],  # (4)
    result: NotRequired[ProtectedQueryResultTypeDef],  # (5)
    error: NotRequired[ProtectedQueryErrorTypeDef],  # (6)
```

1. See [:material-code-braces: ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef) 
2. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype) 
3. See [:material-code-braces: ProtectedQueryResultConfigurationTypeDef](./type_defs.md#protectedqueryresultconfigurationtypedef) 
4. See [:material-code-braces: ProtectedQueryStatisticsTypeDef](./type_defs.md#protectedquerystatisticstypedef) 
5. See [:material-code-braces: ProtectedQueryResultTypeDef](./type_defs.md#protectedqueryresulttypedef) 
6. See [:material-code-braces: ProtectedQueryErrorTypeDef](./type_defs.md#protectedqueryerrortypedef) 
## AnalysisRuleTypeDef

```python
# AnalysisRuleTypeDef definition

class AnalysisRuleTypeDef(TypedDict):
    collaborationId: str,
    type: AnalysisRuleTypeType,  # (1)
    name: str,
    createTime: datetime,
    updateTime: datetime,
    policy: AnalysisRulePolicyTypeDef,  # (2)
```

1. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
2. See [:material-code-braces: AnalysisRulePolicyTypeDef](./type_defs.md#analysisrulepolicytypedef) 
## ConfiguredTableAnalysisRuleTypeDef

```python
# ConfiguredTableAnalysisRuleTypeDef definition

class ConfiguredTableAnalysisRuleTypeDef(TypedDict):
    configuredTableId: str,
    configuredTableArn: str,
    policy: ConfiguredTableAnalysisRulePolicyTypeDef,  # (1)
    type: ConfiguredTableAnalysisRuleTypeType,  # (2)
    createTime: datetime,
    updateTime: datetime,
```

1. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef) 
2. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
## CreateConfiguredTableAnalysisRuleInputRequestTypeDef

```python
# CreateConfiguredTableAnalysisRuleInputRequestTypeDef definition

class CreateConfiguredTableAnalysisRuleInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef,  # (2)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef) 
## UpdateConfiguredTableAnalysisRuleInputRequestTypeDef

```python
# UpdateConfiguredTableAnalysisRuleInputRequestTypeDef definition

class UpdateConfiguredTableAnalysisRuleInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef,  # (2)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef) 
## GetProtectedQueryOutputTypeDef

```python
# GetProtectedQueryOutputTypeDef definition

class GetProtectedQueryOutputTypeDef(TypedDict):
    protectedQuery: ProtectedQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectedQueryTypeDef](./type_defs.md#protectedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartProtectedQueryOutputTypeDef

```python
# StartProtectedQueryOutputTypeDef definition

class StartProtectedQueryOutputTypeDef(TypedDict):
    protectedQuery: ProtectedQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectedQueryTypeDef](./type_defs.md#protectedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProtectedQueryOutputTypeDef

```python
# UpdateProtectedQueryOutputTypeDef definition

class UpdateProtectedQueryOutputTypeDef(TypedDict):
    protectedQuery: ProtectedQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectedQueryTypeDef](./type_defs.md#protectedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaAnalysisRuleOutputTypeDef

```python
# GetSchemaAnalysisRuleOutputTypeDef definition

class GetSchemaAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: AnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisRuleTypeDef](./type_defs.md#analysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredTableAnalysisRuleOutputTypeDef

```python
# CreateConfiguredTableAnalysisRuleOutputTypeDef definition

class CreateConfiguredTableAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: ConfiguredTableAnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAnalysisRuleTypeDef](./type_defs.md#configuredtableanalysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredTableAnalysisRuleOutputTypeDef

```python
# GetConfiguredTableAnalysisRuleOutputTypeDef definition

class GetConfiguredTableAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: ConfiguredTableAnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAnalysisRuleTypeDef](./type_defs.md#configuredtableanalysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredTableAnalysisRuleOutputTypeDef

```python
# UpdateConfiguredTableAnalysisRuleOutputTypeDef definition

class UpdateConfiguredTableAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: ConfiguredTableAnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAnalysisRuleTypeDef](./type_defs.md#configuredtableanalysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
