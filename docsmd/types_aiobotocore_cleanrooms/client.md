# CleanRoomsServiceClient

> [Index](../README.md) > [CleanRoomsService](./README.md) > CleanRoomsServiceClient

!!! note ""

    Auto-generated documentation for [CleanRoomsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#cleanroomsservice)
    type annotations stubs module [types-aiobotocore-cleanrooms](https://pypi.org/project/types-aiobotocore-cleanrooms/).

## CleanRoomsServiceClient

Type annotations and code completion for `#!python session.create_client("cleanrooms")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client)

```python
# CleanRoomsServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_cleanrooms.client import CleanRoomsServiceClient

session = get_session()
async with session.create_client("cleanrooms") as client:
    client: CleanRoomsServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cleanrooms").exceptions` structure.

```python
# CleanRoomsServiceClient.exceptions usage example

async with session.create_client("cleanrooms") as client:
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
# CleanRoomsServiceClient usage type checking example

from types_aiobotocore_cleanrooms.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("cleanrooms").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("cleanrooms").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/generate_presigned_url.html)

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


### batch\_get\_collaboration\_analysis\_template

Retrieves multiple analysis templates within a collaboration by their Amazon
Resource Names (ARNs).

Type annotations and code completion for `#!python session.create_client("cleanrooms").batch_get_collaboration_analysis_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/batch_get_collaboration_analysis_template.html)

```python
# batch_get_collaboration_analysis_template method definition

await def batch_get_collaboration_analysis_template(
    self,
    *,
    collaborationIdentifier: str,
    analysisTemplateArns: Sequence[str],
) -> BatchGetCollaborationAnalysisTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetCollaborationAnalysisTemplateOutputTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateoutputtypedef) 


```python
# batch_get_collaboration_analysis_template method usage example with argument unpacking

kwargs: BatchGetCollaborationAnalysisTemplateInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "analysisTemplateArns": ...,
}

parent.batch_get_collaboration_analysis_template(**kwargs)
```

1. See [:material-code-braces: BatchGetCollaborationAnalysisTemplateInputTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateinputtypedef) 

### batch\_get\_schema

Retrieves multiple schemas by their identifiers.

Type annotations and code completion for `#!python session.create_client("cleanrooms").batch_get_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/batch_get_schema.html)

```python
# batch_get_schema method definition

await def batch_get_schema(
    self,
    *,
    collaborationIdentifier: str,
    names: Sequence[str],
) -> BatchGetSchemaOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetSchemaOutputTypeDef](./type_defs.md#batchgetschemaoutputtypedef) 


```python
# batch_get_schema method usage example with argument unpacking

kwargs: BatchGetSchemaInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "names": ...,
}

parent.batch_get_schema(**kwargs)
```

1. See [:material-code-braces: BatchGetSchemaInputTypeDef](./type_defs.md#batchgetschemainputtypedef) 

### batch\_get\_schema\_analysis\_rule

Retrieves multiple analysis rule schemas.

Type annotations and code completion for `#!python session.create_client("cleanrooms").batch_get_schema_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/batch_get_schema_analysis_rule.html)

```python
# batch_get_schema_analysis_rule method definition

await def batch_get_schema_analysis_rule(
    self,
    *,
    collaborationIdentifier: str,
    schemaAnalysisRuleRequests: Sequence[SchemaAnalysisRuleRequestTypeDef],  # (1)
) -> BatchGetSchemaAnalysisRuleOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SchemaAnalysisRuleRequestTypeDef](./type_defs.md#schemaanalysisrulerequesttypedef) 
2. See [:material-code-braces: BatchGetSchemaAnalysisRuleOutputTypeDef](./type_defs.md#batchgetschemaanalysisruleoutputtypedef) 


```python
# batch_get_schema_analysis_rule method usage example with argument unpacking

kwargs: BatchGetSchemaAnalysisRuleInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "schemaAnalysisRuleRequests": ...,
}

parent.batch_get_schema_analysis_rule(**kwargs)
```

1. See [:material-code-braces: BatchGetSchemaAnalysisRuleInputTypeDef](./type_defs.md#batchgetschemaanalysisruleinputtypedef) 

### create\_analysis\_template

Creates a new analysis template.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_analysis_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/create_analysis_template.html)

```python
# create_analysis_template method definition

await def create_analysis_template(
    self,
    *,
    membershipIdentifier: str,
    name: str,
    format: AnalysisFormatType,  # (1)
    source: AnalysisSourceTypeDef,  # (2)
    description: str = ...,
    tags: Mapping[str, str] = ...,
    analysisParameters: Sequence[AnalysisParameterTypeDef] = ...,  # (3)
) -> CreateAnalysisTemplateOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AnalysisFormatType](./literals.md#analysisformattype) 
2. See [:material-code-braces: AnalysisSourceTypeDef](./type_defs.md#analysissourcetypedef) 
3. See [:material-code-braces: AnalysisParameterTypeDef](./type_defs.md#analysisparametertypedef) 
4. See [:material-code-braces: CreateAnalysisTemplateOutputTypeDef](./type_defs.md#createanalysistemplateoutputtypedef) 


```python
# create_analysis_template method usage example with argument unpacking

kwargs: CreateAnalysisTemplateInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "name": ...,
    "format": ...,
    "source": ...,
}

parent.create_analysis_template(**kwargs)
```

1. See [:material-code-braces: CreateAnalysisTemplateInputTypeDef](./type_defs.md#createanalysistemplateinputtypedef) 

### create\_collaboration

Creates a new collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_collaboration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/create_collaboration.html)

```python
# create_collaboration method definition

await def create_collaboration(
    self,
    *,
    members: Sequence[MemberSpecificationTypeDef],  # (1)
    name: str,
    description: str,
    creatorMemberAbilities: Sequence[MemberAbilityType],  # (2)
    creatorDisplayName: str,
    queryLogStatus: CollaborationQueryLogStatusType,  # (3)
    creatorMLMemberAbilities: MLMemberAbilitiesUnionTypeDef = ...,  # (4)
    dataEncryptionMetadata: DataEncryptionMetadataTypeDef = ...,  # (5)
    tags: Mapping[str, str] = ...,
    creatorPaymentConfiguration: PaymentConfigurationTypeDef = ...,  # (6)
    analyticsEngine: AnalyticsEngineType = ...,  # (7)
) -> CreateCollaborationOutputTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: MemberSpecificationTypeDef](./type_defs.md#memberspecificationtypedef) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
3. See [:material-code-brackets: CollaborationQueryLogStatusType](./literals.md#collaborationquerylogstatustype) 
4. See [:material-code-braces: MLMemberAbilitiesTypeDef](./type_defs.md#mlmemberabilitiestypedef) [:material-code-braces: MLMemberAbilitiesOutputTypeDef](./type_defs.md#mlmemberabilitiesoutputtypedef) 
5. See [:material-code-braces: DataEncryptionMetadataTypeDef](./type_defs.md#dataencryptionmetadatatypedef) 
6. See [:material-code-braces: PaymentConfigurationTypeDef](./type_defs.md#paymentconfigurationtypedef) 
7. See [:material-code-brackets: AnalyticsEngineType](./literals.md#analyticsenginetype) 
8. See [:material-code-braces: CreateCollaborationOutputTypeDef](./type_defs.md#createcollaborationoutputtypedef) 


```python
# create_collaboration method usage example with argument unpacking

kwargs: CreateCollaborationInputTypeDef = {  # (1)
    "members": ...,
    "name": ...,
    "description": ...,
    "creatorMemberAbilities": ...,
    "creatorDisplayName": ...,
    "queryLogStatus": ...,
}

parent.create_collaboration(**kwargs)
```

1. See [:material-code-braces: CreateCollaborationInputTypeDef](./type_defs.md#createcollaborationinputtypedef) 

### create\_configured\_audience\_model\_association

Provides the details necessary to create a configured audience model
association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_configured_audience_model_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/create_configured_audience_model_association.html)

```python
# create_configured_audience_model_association method definition

await def create_configured_audience_model_association(
    self,
    *,
    membershipIdentifier: str,
    configuredAudienceModelArn: str,
    configuredAudienceModelAssociationName: str,
    manageResourcePolicies: bool,
    tags: Mapping[str, str] = ...,
    description: str = ...,
) -> CreateConfiguredAudienceModelAssociationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateConfiguredAudienceModelAssociationOutputTypeDef](./type_defs.md#createconfiguredaudiencemodelassociationoutputtypedef) 


```python
# create_configured_audience_model_association method usage example with argument unpacking

kwargs: CreateConfiguredAudienceModelAssociationInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "configuredAudienceModelArn": ...,
    "configuredAudienceModelAssociationName": ...,
    "manageResourcePolicies": ...,
}

parent.create_configured_audience_model_association(**kwargs)
```

1. See [:material-code-braces: CreateConfiguredAudienceModelAssociationInputTypeDef](./type_defs.md#createconfiguredaudiencemodelassociationinputtypedef) 

### create\_configured\_table

Creates a new configured table resource.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_configured_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/create_configured_table.html)

```python
# create_configured_table method definition

await def create_configured_table(
    self,
    *,
    name: str,
    tableReference: TableReferenceUnionTypeDef,  # (1)
    allowedColumns: Sequence[str],
    analysisMethod: AnalysisMethodType,  # (2)
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateConfiguredTableOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TableReferenceTypeDef](./type_defs.md#tablereferencetypedef) [:material-code-braces: TableReferenceOutputTypeDef](./type_defs.md#tablereferenceoutputtypedef) 
2. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
3. See [:material-code-braces: CreateConfiguredTableOutputTypeDef](./type_defs.md#createconfiguredtableoutputtypedef) 


```python
# create_configured_table method usage example with argument unpacking

kwargs: CreateConfiguredTableInputTypeDef = {  # (1)
    "name": ...,
    "tableReference": ...,
    "allowedColumns": ...,
    "analysisMethod": ...,
}

parent.create_configured_table(**kwargs)
```

1. See [:material-code-braces: CreateConfiguredTableInputTypeDef](./type_defs.md#createconfiguredtableinputtypedef) 

### create\_configured\_table\_analysis\_rule

Creates a new analysis rule for a configured table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_configured_table_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/create_configured_table_analysis_rule.html)

```python
# create_configured_table_analysis_rule method definition

await def create_configured_table_analysis_rule(
    self,
    *,
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAnalysisRulePolicyUnionTypeDef,  # (2)
) -> CreateConfiguredTableAnalysisRuleOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef) [:material-code-braces: ConfiguredTableAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableanalysisrulepolicyoutputtypedef) 
3. See [:material-code-braces: CreateConfiguredTableAnalysisRuleOutputTypeDef](./type_defs.md#createconfiguredtableanalysisruleoutputtypedef) 


```python
# create_configured_table_analysis_rule method usage example with argument unpacking

kwargs: CreateConfiguredTableAnalysisRuleInputTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
    "analysisRuleType": ...,
    "analysisRulePolicy": ...,
}

parent.create_configured_table_analysis_rule(**kwargs)
```

1. See [:material-code-braces: CreateConfiguredTableAnalysisRuleInputTypeDef](./type_defs.md#createconfiguredtableanalysisruleinputtypedef) 

### create\_configured\_table\_association

Creates a configured table association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_configured_table_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/create_configured_table_association.html)

```python
# create_configured_table_association method definition

await def create_configured_table_association(
    self,
    *,
    name: str,
    membershipIdentifier: str,
    configuredTableIdentifier: str,
    roleArn: str,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateConfiguredTableAssociationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateConfiguredTableAssociationOutputTypeDef](./type_defs.md#createconfiguredtableassociationoutputtypedef) 


```python
# create_configured_table_association method usage example with argument unpacking

kwargs: CreateConfiguredTableAssociationInputTypeDef = {  # (1)
    "name": ...,
    "membershipIdentifier": ...,
    "configuredTableIdentifier": ...,
    "roleArn": ...,
}

parent.create_configured_table_association(**kwargs)
```

1. See [:material-code-braces: CreateConfiguredTableAssociationInputTypeDef](./type_defs.md#createconfiguredtableassociationinputtypedef) 

### create\_configured\_table\_association\_analysis\_rule

Creates a new analysis rule for an associated configured table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_configured_table_association_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/create_configured_table_association_analysis_rule.html)

```python
# create_configured_table_association_analysis_rule method definition

await def create_configured_table_association_analysis_rule(
    self,
    *,
    membershipIdentifier: str,
    configuredTableAssociationIdentifier: str,
    analysisRuleType: ConfiguredTableAssociationAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAssociationAnalysisRulePolicyUnionTypeDef,  # (2)
) -> CreateConfiguredTableAssociationAnalysisRuleOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ConfiguredTableAssociationAnalysisRuleTypeType](./literals.md#configuredtableassociationanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAssociationAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicytypedef) [:material-code-braces: ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicyoutputtypedef) 
3. See [:material-code-braces: CreateConfiguredTableAssociationAnalysisRuleOutputTypeDef](./type_defs.md#createconfiguredtableassociationanalysisruleoutputtypedef) 


```python
# create_configured_table_association_analysis_rule method usage example with argument unpacking

kwargs: CreateConfiguredTableAssociationAnalysisRuleInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "configuredTableAssociationIdentifier": ...,
    "analysisRuleType": ...,
    "analysisRulePolicy": ...,
}

parent.create_configured_table_association_analysis_rule(**kwargs)
```

1. See [:material-code-braces: CreateConfiguredTableAssociationAnalysisRuleInputTypeDef](./type_defs.md#createconfiguredtableassociationanalysisruleinputtypedef) 

### create\_id\_mapping\_table

Creates an ID mapping table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_id_mapping_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/create_id_mapping_table.html)

```python
# create_id_mapping_table method definition

await def create_id_mapping_table(
    self,
    *,
    membershipIdentifier: str,
    name: str,
    inputReferenceConfig: IdMappingTableInputReferenceConfigTypeDef,  # (1)
    description: str = ...,
    tags: Mapping[str, str] = ...,
    kmsKeyArn: str = ...,
) -> CreateIdMappingTableOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IdMappingTableInputReferenceConfigTypeDef](./type_defs.md#idmappingtableinputreferenceconfigtypedef) 
2. See [:material-code-braces: CreateIdMappingTableOutputTypeDef](./type_defs.md#createidmappingtableoutputtypedef) 


```python
# create_id_mapping_table method usage example with argument unpacking

kwargs: CreateIdMappingTableInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "name": ...,
    "inputReferenceConfig": ...,
}

parent.create_id_mapping_table(**kwargs)
```

1. See [:material-code-braces: CreateIdMappingTableInputTypeDef](./type_defs.md#createidmappingtableinputtypedef) 

### create\_id\_namespace\_association

Creates an ID namespace association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_id_namespace_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/create_id_namespace_association.html)

```python
# create_id_namespace_association method definition

await def create_id_namespace_association(
    self,
    *,
    membershipIdentifier: str,
    inputReferenceConfig: IdNamespaceAssociationInputReferenceConfigTypeDef,  # (1)
    name: str,
    tags: Mapping[str, str] = ...,
    description: str = ...,
    idMappingConfig: IdMappingConfigTypeDef = ...,  # (2)
) -> CreateIdNamespaceAssociationOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IdNamespaceAssociationInputReferenceConfigTypeDef](./type_defs.md#idnamespaceassociationinputreferenceconfigtypedef) 
2. See [:material-code-braces: IdMappingConfigTypeDef](./type_defs.md#idmappingconfigtypedef) 
3. See [:material-code-braces: CreateIdNamespaceAssociationOutputTypeDef](./type_defs.md#createidnamespaceassociationoutputtypedef) 


```python
# create_id_namespace_association method usage example with argument unpacking

kwargs: CreateIdNamespaceAssociationInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "inputReferenceConfig": ...,
    "name": ...,
}

parent.create_id_namespace_association(**kwargs)
```

1. See [:material-code-braces: CreateIdNamespaceAssociationInputTypeDef](./type_defs.md#createidnamespaceassociationinputtypedef) 

### create\_membership

Creates a membership for a specific collaboration identifier and joins the
collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/create_membership.html)

```python
# create_membership method definition

await def create_membership(
    self,
    *,
    collaborationIdentifier: str,
    queryLogStatus: MembershipQueryLogStatusType,  # (1)
    tags: Mapping[str, str] = ...,
    defaultResultConfiguration: MembershipProtectedQueryResultConfigurationTypeDef = ...,  # (2)
    paymentConfiguration: MembershipPaymentConfigurationTypeDef = ...,  # (3)
) -> CreateMembershipOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype) 
2. See [:material-code-braces: MembershipProtectedQueryResultConfigurationTypeDef](./type_defs.md#membershipprotectedqueryresultconfigurationtypedef) 
3. See [:material-code-braces: MembershipPaymentConfigurationTypeDef](./type_defs.md#membershippaymentconfigurationtypedef) 
4. See [:material-code-braces: CreateMembershipOutputTypeDef](./type_defs.md#createmembershipoutputtypedef) 


```python
# create_membership method usage example with argument unpacking

kwargs: CreateMembershipInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "queryLogStatus": ...,
}

parent.create_membership(**kwargs)
```

1. See [:material-code-braces: CreateMembershipInputTypeDef](./type_defs.md#createmembershipinputtypedef) 

### create\_privacy\_budget\_template

Creates a privacy budget template for a specified membership.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_privacy_budget_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/create_privacy_budget_template.html)

```python
# create_privacy_budget_template method definition

await def create_privacy_budget_template(
    self,
    *,
    membershipIdentifier: str,
    autoRefresh: PrivacyBudgetTemplateAutoRefreshType,  # (1)
    privacyBudgetType: PrivacyBudgetTypeType,  # (2)
    parameters: PrivacyBudgetTemplateParametersInputTypeDef,  # (3)
    tags: Mapping[str, str] = ...,
) -> CreatePrivacyBudgetTemplateOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: PrivacyBudgetTemplateAutoRefreshType](./literals.md#privacybudgettemplateautorefreshtype) 
2. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
3. See [:material-code-braces: PrivacyBudgetTemplateParametersInputTypeDef](./type_defs.md#privacybudgettemplateparametersinputtypedef) 
4. See [:material-code-braces: CreatePrivacyBudgetTemplateOutputTypeDef](./type_defs.md#createprivacybudgettemplateoutputtypedef) 


```python
# create_privacy_budget_template method usage example with argument unpacking

kwargs: CreatePrivacyBudgetTemplateInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "autoRefresh": ...,
    "privacyBudgetType": ...,
    "parameters": ...,
}

parent.create_privacy_budget_template(**kwargs)
```

1. See [:material-code-braces: CreatePrivacyBudgetTemplateInputTypeDef](./type_defs.md#createprivacybudgettemplateinputtypedef) 

### delete\_analysis\_template

Deletes an analysis template.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_analysis_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/delete_analysis_template.html)

```python
# delete_analysis_template method definition

await def delete_analysis_template(
    self,
    *,
    membershipIdentifier: str,
    analysisTemplateIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_analysis_template method usage example with argument unpacking

kwargs: DeleteAnalysisTemplateInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "analysisTemplateIdentifier": ...,
}

parent.delete_analysis_template(**kwargs)
```

1. See [:material-code-braces: DeleteAnalysisTemplateInputTypeDef](./type_defs.md#deleteanalysistemplateinputtypedef) 

### delete\_collaboration

Deletes a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_collaboration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/delete_collaboration.html)

```python
# delete_collaboration method definition

await def delete_collaboration(
    self,
    *,
    collaborationIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_collaboration method usage example with argument unpacking

kwargs: DeleteCollaborationInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.delete_collaboration(**kwargs)
```

1. See [:material-code-braces: DeleteCollaborationInputTypeDef](./type_defs.md#deletecollaborationinputtypedef) 

### delete\_configured\_audience\_model\_association

Provides the information necessary to delete a configured audience model
association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_configured_audience_model_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/delete_configured_audience_model_association.html)

```python
# delete_configured_audience_model_association method definition

await def delete_configured_audience_model_association(
    self,
    *,
    configuredAudienceModelAssociationIdentifier: str,
    membershipIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_configured_audience_model_association method usage example with argument unpacking

kwargs: DeleteConfiguredAudienceModelAssociationInputTypeDef = {  # (1)
    "configuredAudienceModelAssociationIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.delete_configured_audience_model_association(**kwargs)
```

1. See [:material-code-braces: DeleteConfiguredAudienceModelAssociationInputTypeDef](./type_defs.md#deleteconfiguredaudiencemodelassociationinputtypedef) 

### delete\_configured\_table

Deletes a configured table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_configured_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/delete_configured_table.html)

```python
# delete_configured_table method definition

await def delete_configured_table(
    self,
    *,
    configuredTableIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_configured_table method usage example with argument unpacking

kwargs: DeleteConfiguredTableInputTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
}

parent.delete_configured_table(**kwargs)
```

1. See [:material-code-braces: DeleteConfiguredTableInputTypeDef](./type_defs.md#deleteconfiguredtableinputtypedef) 

### delete\_configured\_table\_analysis\_rule

Deletes a configured table analysis rule.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_configured_table_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/delete_configured_table_analysis_rule.html)

```python
# delete_configured_table_analysis_rule method definition

await def delete_configured_table_analysis_rule(
    self,
    *,
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 


```python
# delete_configured_table_analysis_rule method usage example with argument unpacking

kwargs: DeleteConfiguredTableAnalysisRuleInputTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
    "analysisRuleType": ...,
}

parent.delete_configured_table_analysis_rule(**kwargs)
```

1. See [:material-code-braces: DeleteConfiguredTableAnalysisRuleInputTypeDef](./type_defs.md#deleteconfiguredtableanalysisruleinputtypedef) 

### delete\_configured\_table\_association

Deletes a configured table association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_configured_table_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/delete_configured_table_association.html)

```python
# delete_configured_table_association method definition

await def delete_configured_table_association(
    self,
    *,
    configuredTableAssociationIdentifier: str,
    membershipIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_configured_table_association method usage example with argument unpacking

kwargs: DeleteConfiguredTableAssociationInputTypeDef = {  # (1)
    "configuredTableAssociationIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.delete_configured_table_association(**kwargs)
```

1. See [:material-code-braces: DeleteConfiguredTableAssociationInputTypeDef](./type_defs.md#deleteconfiguredtableassociationinputtypedef) 

### delete\_configured\_table\_association\_analysis\_rule

Deletes an analysis rule for a configured table association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_configured_table_association_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/delete_configured_table_association_analysis_rule.html)

```python
# delete_configured_table_association_analysis_rule method definition

await def delete_configured_table_association_analysis_rule(
    self,
    *,
    membershipIdentifier: str,
    configuredTableAssociationIdentifier: str,
    analysisRuleType: ConfiguredTableAssociationAnalysisRuleTypeType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ConfiguredTableAssociationAnalysisRuleTypeType](./literals.md#configuredtableassociationanalysisruletypetype) 


```python
# delete_configured_table_association_analysis_rule method usage example with argument unpacking

kwargs: DeleteConfiguredTableAssociationAnalysisRuleInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "configuredTableAssociationIdentifier": ...,
    "analysisRuleType": ...,
}

parent.delete_configured_table_association_analysis_rule(**kwargs)
```

1. See [:material-code-braces: DeleteConfiguredTableAssociationAnalysisRuleInputTypeDef](./type_defs.md#deleteconfiguredtableassociationanalysisruleinputtypedef) 

### delete\_id\_mapping\_table

Deletes an ID mapping table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_id_mapping_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/delete_id_mapping_table.html)

```python
# delete_id_mapping_table method definition

await def delete_id_mapping_table(
    self,
    *,
    idMappingTableIdentifier: str,
    membershipIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_id_mapping_table method usage example with argument unpacking

kwargs: DeleteIdMappingTableInputTypeDef = {  # (1)
    "idMappingTableIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.delete_id_mapping_table(**kwargs)
```

1. See [:material-code-braces: DeleteIdMappingTableInputTypeDef](./type_defs.md#deleteidmappingtableinputtypedef) 

### delete\_id\_namespace\_association

Deletes an ID namespace association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_id_namespace_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/delete_id_namespace_association.html)

```python
# delete_id_namespace_association method definition

await def delete_id_namespace_association(
    self,
    *,
    idNamespaceAssociationIdentifier: str,
    membershipIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_id_namespace_association method usage example with argument unpacking

kwargs: DeleteIdNamespaceAssociationInputTypeDef = {  # (1)
    "idNamespaceAssociationIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.delete_id_namespace_association(**kwargs)
```

1. See [:material-code-braces: DeleteIdNamespaceAssociationInputTypeDef](./type_defs.md#deleteidnamespaceassociationinputtypedef) 

### delete\_member

Removes the specified member from a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_member` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/delete_member.html)

```python
# delete_member method definition

await def delete_member(
    self,
    *,
    collaborationIdentifier: str,
    accountId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_member method usage example with argument unpacking

kwargs: DeleteMemberInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "accountId": ...,
}

parent.delete_member(**kwargs)
```

1. See [:material-code-braces: DeleteMemberInputTypeDef](./type_defs.md#deletememberinputtypedef) 

### delete\_membership

Deletes a specified membership.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/delete_membership.html)

```python
# delete_membership method definition

await def delete_membership(
    self,
    *,
    membershipIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_membership method usage example with argument unpacking

kwargs: DeleteMembershipInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.delete_membership(**kwargs)
```

1. See [:material-code-braces: DeleteMembershipInputTypeDef](./type_defs.md#deletemembershipinputtypedef) 

### delete\_privacy\_budget\_template

Deletes a privacy budget template for a specified membership.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_privacy_budget_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/delete_privacy_budget_template.html)

```python
# delete_privacy_budget_template method definition

await def delete_privacy_budget_template(
    self,
    *,
    membershipIdentifier: str,
    privacyBudgetTemplateIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_privacy_budget_template method usage example with argument unpacking

kwargs: DeletePrivacyBudgetTemplateInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "privacyBudgetTemplateIdentifier": ...,
}

parent.delete_privacy_budget_template(**kwargs)
```

1. See [:material-code-braces: DeletePrivacyBudgetTemplateInputTypeDef](./type_defs.md#deleteprivacybudgettemplateinputtypedef) 

### get\_analysis\_template

Retrieves an analysis template.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_analysis_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_analysis_template.html)

```python
# get_analysis_template method definition

await def get_analysis_template(
    self,
    *,
    membershipIdentifier: str,
    analysisTemplateIdentifier: str,
) -> GetAnalysisTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAnalysisTemplateOutputTypeDef](./type_defs.md#getanalysistemplateoutputtypedef) 


```python
# get_analysis_template method usage example with argument unpacking

kwargs: GetAnalysisTemplateInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "analysisTemplateIdentifier": ...,
}

parent.get_analysis_template(**kwargs)
```

1. See [:material-code-braces: GetAnalysisTemplateInputTypeDef](./type_defs.md#getanalysistemplateinputtypedef) 

### get\_collaboration

Returns metadata about a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_collaboration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_collaboration.html)

```python
# get_collaboration method definition

await def get_collaboration(
    self,
    *,
    collaborationIdentifier: str,
) -> GetCollaborationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCollaborationOutputTypeDef](./type_defs.md#getcollaborationoutputtypedef) 


```python
# get_collaboration method usage example with argument unpacking

kwargs: GetCollaborationInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.get_collaboration(**kwargs)
```

1. See [:material-code-braces: GetCollaborationInputTypeDef](./type_defs.md#getcollaborationinputtypedef) 

### get\_collaboration\_analysis\_template

Retrieves an analysis template within a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_collaboration_analysis_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_collaboration_analysis_template.html)

```python
# get_collaboration_analysis_template method definition

await def get_collaboration_analysis_template(
    self,
    *,
    collaborationIdentifier: str,
    analysisTemplateArn: str,
) -> GetCollaborationAnalysisTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCollaborationAnalysisTemplateOutputTypeDef](./type_defs.md#getcollaborationanalysistemplateoutputtypedef) 


```python
# get_collaboration_analysis_template method usage example with argument unpacking

kwargs: GetCollaborationAnalysisTemplateInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "analysisTemplateArn": ...,
}

parent.get_collaboration_analysis_template(**kwargs)
```

1. See [:material-code-braces: GetCollaborationAnalysisTemplateInputTypeDef](./type_defs.md#getcollaborationanalysistemplateinputtypedef) 

### get\_collaboration\_configured\_audience\_model\_association

Retrieves a configured audience model association within a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_collaboration_configured_audience_model_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_collaboration_configured_audience_model_association.html)

```python
# get_collaboration_configured_audience_model_association method definition

await def get_collaboration_configured_audience_model_association(
    self,
    *,
    collaborationIdentifier: str,
    configuredAudienceModelAssociationIdentifier: str,
) -> GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef](./type_defs.md#getcollaborationconfiguredaudiencemodelassociationoutputtypedef) 


```python
# get_collaboration_configured_audience_model_association method usage example with argument unpacking

kwargs: GetCollaborationConfiguredAudienceModelAssociationInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "configuredAudienceModelAssociationIdentifier": ...,
}

parent.get_collaboration_configured_audience_model_association(**kwargs)
```

1. See [:material-code-braces: GetCollaborationConfiguredAudienceModelAssociationInputTypeDef](./type_defs.md#getcollaborationconfiguredaudiencemodelassociationinputtypedef) 

### get\_collaboration\_id\_namespace\_association

Retrieves an ID namespace association from a specific collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_collaboration_id_namespace_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_collaboration_id_namespace_association.html)

```python
# get_collaboration_id_namespace_association method definition

await def get_collaboration_id_namespace_association(
    self,
    *,
    collaborationIdentifier: str,
    idNamespaceAssociationIdentifier: str,
) -> GetCollaborationIdNamespaceAssociationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCollaborationIdNamespaceAssociationOutputTypeDef](./type_defs.md#getcollaborationidnamespaceassociationoutputtypedef) 


```python
# get_collaboration_id_namespace_association method usage example with argument unpacking

kwargs: GetCollaborationIdNamespaceAssociationInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "idNamespaceAssociationIdentifier": ...,
}

parent.get_collaboration_id_namespace_association(**kwargs)
```

1. See [:material-code-braces: GetCollaborationIdNamespaceAssociationInputTypeDef](./type_defs.md#getcollaborationidnamespaceassociationinputtypedef) 

### get\_collaboration\_privacy\_budget\_template

Returns details about a specified privacy budget template.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_collaboration_privacy_budget_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_collaboration_privacy_budget_template.html)

```python
# get_collaboration_privacy_budget_template method definition

await def get_collaboration_privacy_budget_template(
    self,
    *,
    collaborationIdentifier: str,
    privacyBudgetTemplateIdentifier: str,
) -> GetCollaborationPrivacyBudgetTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCollaborationPrivacyBudgetTemplateOutputTypeDef](./type_defs.md#getcollaborationprivacybudgettemplateoutputtypedef) 


```python
# get_collaboration_privacy_budget_template method usage example with argument unpacking

kwargs: GetCollaborationPrivacyBudgetTemplateInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "privacyBudgetTemplateIdentifier": ...,
}

parent.get_collaboration_privacy_budget_template(**kwargs)
```

1. See [:material-code-braces: GetCollaborationPrivacyBudgetTemplateInputTypeDef](./type_defs.md#getcollaborationprivacybudgettemplateinputtypedef) 

### get\_configured\_audience\_model\_association

Returns information about a configured audience model association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_configured_audience_model_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_configured_audience_model_association.html)

```python
# get_configured_audience_model_association method definition

await def get_configured_audience_model_association(
    self,
    *,
    configuredAudienceModelAssociationIdentifier: str,
    membershipIdentifier: str,
) -> GetConfiguredAudienceModelAssociationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfiguredAudienceModelAssociationOutputTypeDef](./type_defs.md#getconfiguredaudiencemodelassociationoutputtypedef) 


```python
# get_configured_audience_model_association method usage example with argument unpacking

kwargs: GetConfiguredAudienceModelAssociationInputTypeDef = {  # (1)
    "configuredAudienceModelAssociationIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.get_configured_audience_model_association(**kwargs)
```

1. See [:material-code-braces: GetConfiguredAudienceModelAssociationInputTypeDef](./type_defs.md#getconfiguredaudiencemodelassociationinputtypedef) 

### get\_configured\_table

Retrieves a configured table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_configured_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_configured_table.html)

```python
# get_configured_table method definition

await def get_configured_table(
    self,
    *,
    configuredTableIdentifier: str,
) -> GetConfiguredTableOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfiguredTableOutputTypeDef](./type_defs.md#getconfiguredtableoutputtypedef) 


```python
# get_configured_table method usage example with argument unpacking

kwargs: GetConfiguredTableInputTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
}

parent.get_configured_table(**kwargs)
```

1. See [:material-code-braces: GetConfiguredTableInputTypeDef](./type_defs.md#getconfiguredtableinputtypedef) 

### get\_configured\_table\_analysis\_rule

Retrieves a configured table analysis rule.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_configured_table_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_configured_table_analysis_rule.html)

```python
# get_configured_table_analysis_rule method definition

await def get_configured_table_analysis_rule(
    self,
    *,
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
) -> GetConfiguredTableAnalysisRuleOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-braces: GetConfiguredTableAnalysisRuleOutputTypeDef](./type_defs.md#getconfiguredtableanalysisruleoutputtypedef) 


```python
# get_configured_table_analysis_rule method usage example with argument unpacking

kwargs: GetConfiguredTableAnalysisRuleInputTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
    "analysisRuleType": ...,
}

parent.get_configured_table_analysis_rule(**kwargs)
```

1. See [:material-code-braces: GetConfiguredTableAnalysisRuleInputTypeDef](./type_defs.md#getconfiguredtableanalysisruleinputtypedef) 

### get\_configured\_table\_association

Retrieves a configured table association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_configured_table_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_configured_table_association.html)

```python
# get_configured_table_association method definition

await def get_configured_table_association(
    self,
    *,
    configuredTableAssociationIdentifier: str,
    membershipIdentifier: str,
) -> GetConfiguredTableAssociationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfiguredTableAssociationOutputTypeDef](./type_defs.md#getconfiguredtableassociationoutputtypedef) 


```python
# get_configured_table_association method usage example with argument unpacking

kwargs: GetConfiguredTableAssociationInputTypeDef = {  # (1)
    "configuredTableAssociationIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.get_configured_table_association(**kwargs)
```

1. See [:material-code-braces: GetConfiguredTableAssociationInputTypeDef](./type_defs.md#getconfiguredtableassociationinputtypedef) 

### get\_configured\_table\_association\_analysis\_rule

Retrieves the analysis rule for a configured table association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_configured_table_association_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_configured_table_association_analysis_rule.html)

```python
# get_configured_table_association_analysis_rule method definition

await def get_configured_table_association_analysis_rule(
    self,
    *,
    membershipIdentifier: str,
    configuredTableAssociationIdentifier: str,
    analysisRuleType: ConfiguredTableAssociationAnalysisRuleTypeType,  # (1)
) -> GetConfiguredTableAssociationAnalysisRuleOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConfiguredTableAssociationAnalysisRuleTypeType](./literals.md#configuredtableassociationanalysisruletypetype) 
2. See [:material-code-braces: GetConfiguredTableAssociationAnalysisRuleOutputTypeDef](./type_defs.md#getconfiguredtableassociationanalysisruleoutputtypedef) 


```python
# get_configured_table_association_analysis_rule method usage example with argument unpacking

kwargs: GetConfiguredTableAssociationAnalysisRuleInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "configuredTableAssociationIdentifier": ...,
    "analysisRuleType": ...,
}

parent.get_configured_table_association_analysis_rule(**kwargs)
```

1. See [:material-code-braces: GetConfiguredTableAssociationAnalysisRuleInputTypeDef](./type_defs.md#getconfiguredtableassociationanalysisruleinputtypedef) 

### get\_id\_mapping\_table

Retrieves an ID mapping table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_id_mapping_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_id_mapping_table.html)

```python
# get_id_mapping_table method definition

await def get_id_mapping_table(
    self,
    *,
    idMappingTableIdentifier: str,
    membershipIdentifier: str,
) -> GetIdMappingTableOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdMappingTableOutputTypeDef](./type_defs.md#getidmappingtableoutputtypedef) 


```python
# get_id_mapping_table method usage example with argument unpacking

kwargs: GetIdMappingTableInputTypeDef = {  # (1)
    "idMappingTableIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.get_id_mapping_table(**kwargs)
```

1. See [:material-code-braces: GetIdMappingTableInputTypeDef](./type_defs.md#getidmappingtableinputtypedef) 

### get\_id\_namespace\_association

Retrieves an ID namespace association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_id_namespace_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_id_namespace_association.html)

```python
# get_id_namespace_association method definition

await def get_id_namespace_association(
    self,
    *,
    idNamespaceAssociationIdentifier: str,
    membershipIdentifier: str,
) -> GetIdNamespaceAssociationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdNamespaceAssociationOutputTypeDef](./type_defs.md#getidnamespaceassociationoutputtypedef) 


```python
# get_id_namespace_association method usage example with argument unpacking

kwargs: GetIdNamespaceAssociationInputTypeDef = {  # (1)
    "idNamespaceAssociationIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.get_id_namespace_association(**kwargs)
```

1. See [:material-code-braces: GetIdNamespaceAssociationInputTypeDef](./type_defs.md#getidnamespaceassociationinputtypedef) 

### get\_membership

Retrieves a specified membership for an identifier.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_membership.html)

```python
# get_membership method definition

await def get_membership(
    self,
    *,
    membershipIdentifier: str,
) -> GetMembershipOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMembershipOutputTypeDef](./type_defs.md#getmembershipoutputtypedef) 


```python
# get_membership method usage example with argument unpacking

kwargs: GetMembershipInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.get_membership(**kwargs)
```

1. See [:material-code-braces: GetMembershipInputTypeDef](./type_defs.md#getmembershipinputtypedef) 

### get\_privacy\_budget\_template

Returns details for a specified privacy budget template.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_privacy_budget_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_privacy_budget_template.html)

```python
# get_privacy_budget_template method definition

await def get_privacy_budget_template(
    self,
    *,
    membershipIdentifier: str,
    privacyBudgetTemplateIdentifier: str,
) -> GetPrivacyBudgetTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPrivacyBudgetTemplateOutputTypeDef](./type_defs.md#getprivacybudgettemplateoutputtypedef) 


```python
# get_privacy_budget_template method usage example with argument unpacking

kwargs: GetPrivacyBudgetTemplateInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "privacyBudgetTemplateIdentifier": ...,
}

parent.get_privacy_budget_template(**kwargs)
```

1. See [:material-code-braces: GetPrivacyBudgetTemplateInputTypeDef](./type_defs.md#getprivacybudgettemplateinputtypedef) 

### get\_protected\_query

Returns query processing metadata.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_protected_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_protected_query.html)

```python
# get_protected_query method definition

await def get_protected_query(
    self,
    *,
    membershipIdentifier: str,
    protectedQueryIdentifier: str,
) -> GetProtectedQueryOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProtectedQueryOutputTypeDef](./type_defs.md#getprotectedqueryoutputtypedef) 


```python
# get_protected_query method usage example with argument unpacking

kwargs: GetProtectedQueryInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "protectedQueryIdentifier": ...,
}

parent.get_protected_query(**kwargs)
```

1. See [:material-code-braces: GetProtectedQueryInputTypeDef](./type_defs.md#getprotectedqueryinputtypedef) 

### get\_schema

Retrieves the schema for a relation within a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_schema.html)

```python
# get_schema method definition

await def get_schema(
    self,
    *,
    collaborationIdentifier: str,
    name: str,
) -> GetSchemaOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSchemaOutputTypeDef](./type_defs.md#getschemaoutputtypedef) 


```python
# get_schema method usage example with argument unpacking

kwargs: GetSchemaInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "name": ...,
}

parent.get_schema(**kwargs)
```

1. See [:material-code-braces: GetSchemaInputTypeDef](./type_defs.md#getschemainputtypedef) 

### get\_schema\_analysis\_rule

Retrieves a schema analysis rule.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_schema_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/get_schema_analysis_rule.html)

```python
# get_schema_analysis_rule method definition

await def get_schema_analysis_rule(
    self,
    *,
    collaborationIdentifier: str,
    name: str,
    type: AnalysisRuleTypeType,  # (1)
) -> GetSchemaAnalysisRuleOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
2. See [:material-code-braces: GetSchemaAnalysisRuleOutputTypeDef](./type_defs.md#getschemaanalysisruleoutputtypedef) 


```python
# get_schema_analysis_rule method usage example with argument unpacking

kwargs: GetSchemaAnalysisRuleInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "name": ...,
    "type": ...,
}

parent.get_schema_analysis_rule(**kwargs)
```

1. See [:material-code-braces: GetSchemaAnalysisRuleInputTypeDef](./type_defs.md#getschemaanalysisruleinputtypedef) 

### list\_analysis\_templates

Lists analysis templates that the caller owns.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_analysis_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_analysis_templates.html)

```python
# list_analysis_templates method definition

await def list_analysis_templates(
    self,
    *,
    membershipIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAnalysisTemplatesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAnalysisTemplatesOutputTypeDef](./type_defs.md#listanalysistemplatesoutputtypedef) 


```python
# list_analysis_templates method usage example with argument unpacking

kwargs: ListAnalysisTemplatesInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_analysis_templates(**kwargs)
```

1. See [:material-code-braces: ListAnalysisTemplatesInputTypeDef](./type_defs.md#listanalysistemplatesinputtypedef) 

### list\_collaboration\_analysis\_templates

Lists analysis templates within a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_collaboration_analysis_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_collaboration_analysis_templates.html)

```python
# list_collaboration_analysis_templates method definition

await def list_collaboration_analysis_templates(
    self,
    *,
    collaborationIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCollaborationAnalysisTemplatesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCollaborationAnalysisTemplatesOutputTypeDef](./type_defs.md#listcollaborationanalysistemplatesoutputtypedef) 


```python
# list_collaboration_analysis_templates method usage example with argument unpacking

kwargs: ListCollaborationAnalysisTemplatesInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.list_collaboration_analysis_templates(**kwargs)
```

1. See [:material-code-braces: ListCollaborationAnalysisTemplatesInputTypeDef](./type_defs.md#listcollaborationanalysistemplatesinputtypedef) 

### list\_collaboration\_configured\_audience\_model\_associations

Lists configured audience model associations within a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_collaboration_configured_audience_model_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_collaboration_configured_audience_model_associations.html)

```python
# list_collaboration_configured_audience_model_associations method definition

await def list_collaboration_configured_audience_model_associations(
    self,
    *,
    collaborationIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef](./type_defs.md#listcollaborationconfiguredaudiencemodelassociationsoutputtypedef) 


```python
# list_collaboration_configured_audience_model_associations method usage example with argument unpacking

kwargs: ListCollaborationConfiguredAudienceModelAssociationsInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.list_collaboration_configured_audience_model_associations(**kwargs)
```

1. See [:material-code-braces: ListCollaborationConfiguredAudienceModelAssociationsInputTypeDef](./type_defs.md#listcollaborationconfiguredaudiencemodelassociationsinputtypedef) 

### list\_collaboration\_id\_namespace\_associations

Returns a list of the ID namespace associations in a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_collaboration_id_namespace_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_collaboration_id_namespace_associations.html)

```python
# list_collaboration_id_namespace_associations method definition

await def list_collaboration_id_namespace_associations(
    self,
    *,
    collaborationIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCollaborationIdNamespaceAssociationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCollaborationIdNamespaceAssociationsOutputTypeDef](./type_defs.md#listcollaborationidnamespaceassociationsoutputtypedef) 


```python
# list_collaboration_id_namespace_associations method usage example with argument unpacking

kwargs: ListCollaborationIdNamespaceAssociationsInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.list_collaboration_id_namespace_associations(**kwargs)
```

1. See [:material-code-braces: ListCollaborationIdNamespaceAssociationsInputTypeDef](./type_defs.md#listcollaborationidnamespaceassociationsinputtypedef) 

### list\_collaboration\_privacy\_budget\_templates

Returns an array that summarizes each privacy budget template in a specified
collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_collaboration_privacy_budget_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_collaboration_privacy_budget_templates.html)

```python
# list_collaboration_privacy_budget_templates method definition

await def list_collaboration_privacy_budget_templates(
    self,
    *,
    collaborationIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCollaborationPrivacyBudgetTemplatesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCollaborationPrivacyBudgetTemplatesOutputTypeDef](./type_defs.md#listcollaborationprivacybudgettemplatesoutputtypedef) 


```python
# list_collaboration_privacy_budget_templates method usage example with argument unpacking

kwargs: ListCollaborationPrivacyBudgetTemplatesInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.list_collaboration_privacy_budget_templates(**kwargs)
```

1. See [:material-code-braces: ListCollaborationPrivacyBudgetTemplatesInputTypeDef](./type_defs.md#listcollaborationprivacybudgettemplatesinputtypedef) 

### list\_collaboration\_privacy\_budgets

Returns an array that summarizes each privacy budget in a specified
collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_collaboration_privacy_budgets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_collaboration_privacy_budgets.html)

```python
# list_collaboration_privacy_budgets method definition

await def list_collaboration_privacy_budgets(
    self,
    *,
    collaborationIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListCollaborationPrivacyBudgetsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-braces: ListCollaborationPrivacyBudgetsOutputTypeDef](./type_defs.md#listcollaborationprivacybudgetsoutputtypedef) 


```python
# list_collaboration_privacy_budgets method usage example with argument unpacking

kwargs: ListCollaborationPrivacyBudgetsInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "privacyBudgetType": ...,
}

parent.list_collaboration_privacy_budgets(**kwargs)
```

1. See [:material-code-braces: ListCollaborationPrivacyBudgetsInputTypeDef](./type_defs.md#listcollaborationprivacybudgetsinputtypedef) 

### list\_collaborations

Lists collaborations the caller owns, is active in, or has been invited to.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_collaborations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_collaborations.html)

```python
# list_collaborations method definition

await def list_collaborations(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    memberStatus: FilterableMemberStatusType = ...,  # (1)
) -> ListCollaborationsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FilterableMemberStatusType](./literals.md#filterablememberstatustype) 
2. See [:material-code-braces: ListCollaborationsOutputTypeDef](./type_defs.md#listcollaborationsoutputtypedef) 


```python
# list_collaborations method usage example with argument unpacking

kwargs: ListCollaborationsInputTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_collaborations(**kwargs)
```

1. See [:material-code-braces: ListCollaborationsInputTypeDef](./type_defs.md#listcollaborationsinputtypedef) 

### list\_configured\_audience\_model\_associations

Lists information about requested configured audience model associations.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_configured_audience_model_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_configured_audience_model_associations.html)

```python
# list_configured_audience_model_associations method definition

await def list_configured_audience_model_associations(
    self,
    *,
    membershipIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListConfiguredAudienceModelAssociationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConfiguredAudienceModelAssociationsOutputTypeDef](./type_defs.md#listconfiguredaudiencemodelassociationsoutputtypedef) 


```python
# list_configured_audience_model_associations method usage example with argument unpacking

kwargs: ListConfiguredAudienceModelAssociationsInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_configured_audience_model_associations(**kwargs)
```

1. See [:material-code-braces: ListConfiguredAudienceModelAssociationsInputTypeDef](./type_defs.md#listconfiguredaudiencemodelassociationsinputtypedef) 

### list\_configured\_table\_associations

Lists configured table associations for a membership.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_configured_table_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_configured_table_associations.html)

```python
# list_configured_table_associations method definition

await def list_configured_table_associations(
    self,
    *,
    membershipIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListConfiguredTableAssociationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConfiguredTableAssociationsOutputTypeDef](./type_defs.md#listconfiguredtableassociationsoutputtypedef) 


```python
# list_configured_table_associations method usage example with argument unpacking

kwargs: ListConfiguredTableAssociationsInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_configured_table_associations(**kwargs)
```

1. See [:material-code-braces: ListConfiguredTableAssociationsInputTypeDef](./type_defs.md#listconfiguredtableassociationsinputtypedef) 

### list\_configured\_tables

Lists configured tables.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_configured_tables` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_configured_tables.html)

```python
# list_configured_tables method definition

await def list_configured_tables(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListConfiguredTablesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConfiguredTablesOutputTypeDef](./type_defs.md#listconfiguredtablesoutputtypedef) 


```python
# list_configured_tables method usage example with argument unpacking

kwargs: ListConfiguredTablesInputTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_configured_tables(**kwargs)
```

1. See [:material-code-braces: ListConfiguredTablesInputTypeDef](./type_defs.md#listconfiguredtablesinputtypedef) 

### list\_id\_mapping\_tables

Returns a list of ID mapping tables.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_id_mapping_tables` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_id_mapping_tables.html)

```python
# list_id_mapping_tables method definition

await def list_id_mapping_tables(
    self,
    *,
    membershipIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListIdMappingTablesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdMappingTablesOutputTypeDef](./type_defs.md#listidmappingtablesoutputtypedef) 


```python
# list_id_mapping_tables method usage example with argument unpacking

kwargs: ListIdMappingTablesInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_id_mapping_tables(**kwargs)
```

1. See [:material-code-braces: ListIdMappingTablesInputTypeDef](./type_defs.md#listidmappingtablesinputtypedef) 

### list\_id\_namespace\_associations

Returns a list of ID namespace associations.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_id_namespace_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_id_namespace_associations.html)

```python
# list_id_namespace_associations method definition

await def list_id_namespace_associations(
    self,
    *,
    membershipIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListIdNamespaceAssociationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdNamespaceAssociationsOutputTypeDef](./type_defs.md#listidnamespaceassociationsoutputtypedef) 


```python
# list_id_namespace_associations method usage example with argument unpacking

kwargs: ListIdNamespaceAssociationsInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_id_namespace_associations(**kwargs)
```

1. See [:material-code-braces: ListIdNamespaceAssociationsInputTypeDef](./type_defs.md#listidnamespaceassociationsinputtypedef) 

### list\_members

Lists all members within a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_members.html)

```python
# list_members method definition

await def list_members(
    self,
    *,
    collaborationIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListMembersOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMembersOutputTypeDef](./type_defs.md#listmembersoutputtypedef) 


```python
# list_members method usage example with argument unpacking

kwargs: ListMembersInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.list_members(**kwargs)
```

1. See [:material-code-braces: ListMembersInputTypeDef](./type_defs.md#listmembersinputtypedef) 

### list\_memberships

Lists all memberships resources within the caller's account.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_memberships` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_memberships.html)

```python
# list_memberships method definition

await def list_memberships(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    status: MembershipStatusType = ...,  # (1)
) -> ListMembershipsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
2. See [:material-code-braces: ListMembershipsOutputTypeDef](./type_defs.md#listmembershipsoutputtypedef) 


```python
# list_memberships method usage example with argument unpacking

kwargs: ListMembershipsInputTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_memberships(**kwargs)
```

1. See [:material-code-braces: ListMembershipsInputTypeDef](./type_defs.md#listmembershipsinputtypedef) 

### list\_privacy\_budget\_templates

Returns detailed information about the privacy budget templates in a specified
membership.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_privacy_budget_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_privacy_budget_templates.html)

```python
# list_privacy_budget_templates method definition

await def list_privacy_budget_templates(
    self,
    *,
    membershipIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPrivacyBudgetTemplatesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPrivacyBudgetTemplatesOutputTypeDef](./type_defs.md#listprivacybudgettemplatesoutputtypedef) 


```python
# list_privacy_budget_templates method usage example with argument unpacking

kwargs: ListPrivacyBudgetTemplatesInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_privacy_budget_templates(**kwargs)
```

1. See [:material-code-braces: ListPrivacyBudgetTemplatesInputTypeDef](./type_defs.md#listprivacybudgettemplatesinputtypedef) 

### list\_privacy\_budgets

Returns detailed information about the privacy budgets in a specified
membership.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_privacy_budgets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_privacy_budgets.html)

```python
# list_privacy_budgets method definition

await def list_privacy_budgets(
    self,
    *,
    membershipIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPrivacyBudgetsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-braces: ListPrivacyBudgetsOutputTypeDef](./type_defs.md#listprivacybudgetsoutputtypedef) 


```python
# list_privacy_budgets method usage example with argument unpacking

kwargs: ListPrivacyBudgetsInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "privacyBudgetType": ...,
}

parent.list_privacy_budgets(**kwargs)
```

1. See [:material-code-braces: ListPrivacyBudgetsInputTypeDef](./type_defs.md#listprivacybudgetsinputtypedef) 

### list\_protected\_queries

Lists protected queries, sorted by the most recent query.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_protected_queries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_protected_queries.html)

```python
# list_protected_queries method definition

await def list_protected_queries(
    self,
    *,
    membershipIdentifier: str,
    status: ProtectedQueryStatusType = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListProtectedQueriesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype) 
2. See [:material-code-braces: ListProtectedQueriesOutputTypeDef](./type_defs.md#listprotectedqueriesoutputtypedef) 


```python
# list_protected_queries method usage example with argument unpacking

kwargs: ListProtectedQueriesInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_protected_queries(**kwargs)
```

1. See [:material-code-braces: ListProtectedQueriesInputTypeDef](./type_defs.md#listprotectedqueriesinputtypedef) 

### list\_schemas

Lists the schemas for relations within a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_schemas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_schemas.html)

```python
# list_schemas method definition

await def list_schemas(
    self,
    *,
    collaborationIdentifier: str,
    schemaType: SchemaTypeType = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListSchemasOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype) 
2. See [:material-code-braces: ListSchemasOutputTypeDef](./type_defs.md#listschemasoutputtypedef) 


```python
# list_schemas method usage example with argument unpacking

kwargs: ListSchemasInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.list_schemas(**kwargs)
```

1. See [:material-code-braces: ListSchemasInputTypeDef](./type_defs.md#listschemasinputtypedef) 

### list\_tags\_for\_resource

Lists all of the tags that have been added to a resource.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef) 

### populate\_id\_mapping\_table

Defines the information that's necessary to populate an ID mapping table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").populate_id_mapping_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/populate_id_mapping_table.html)

```python
# populate_id_mapping_table method definition

await def populate_id_mapping_table(
    self,
    *,
    idMappingTableIdentifier: str,
    membershipIdentifier: str,
) -> PopulateIdMappingTableOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PopulateIdMappingTableOutputTypeDef](./type_defs.md#populateidmappingtableoutputtypedef) 


```python
# populate_id_mapping_table method usage example with argument unpacking

kwargs: PopulateIdMappingTableInputTypeDef = {  # (1)
    "idMappingTableIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.populate_id_mapping_table(**kwargs)
```

1. See [:material-code-braces: PopulateIdMappingTableInputTypeDef](./type_defs.md#populateidmappingtableinputtypedef) 

### preview\_privacy\_impact

An estimate of the number of aggregation functions that the member who can
query can run given epsilon and noise parameters.

Type annotations and code completion for `#!python session.create_client("cleanrooms").preview_privacy_impact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/preview_privacy_impact.html)

```python
# preview_privacy_impact method definition

await def preview_privacy_impact(
    self,
    *,
    membershipIdentifier: str,
    parameters: PreviewPrivacyImpactParametersInputTypeDef,  # (1)
) -> PreviewPrivacyImpactOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PreviewPrivacyImpactParametersInputTypeDef](./type_defs.md#previewprivacyimpactparametersinputtypedef) 
2. See [:material-code-braces: PreviewPrivacyImpactOutputTypeDef](./type_defs.md#previewprivacyimpactoutputtypedef) 


```python
# preview_privacy_impact method usage example with argument unpacking

kwargs: PreviewPrivacyImpactInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "parameters": ...,
}

parent.preview_privacy_impact(**kwargs)
```

1. See [:material-code-braces: PreviewPrivacyImpactInputTypeDef](./type_defs.md#previewprivacyimpactinputtypedef) 

### start\_protected\_query

Creates a protected query that is started by Clean Rooms.

Type annotations and code completion for `#!python session.create_client("cleanrooms").start_protected_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/start_protected_query.html)

```python
# start_protected_query method definition

await def start_protected_query(
    self,
    *,
    type: ProtectedQueryTypeType,  # (1)
    membershipIdentifier: str,
    sqlParameters: ProtectedQuerySQLParametersUnionTypeDef,  # (2)
    resultConfiguration: ProtectedQueryResultConfigurationTypeDef = ...,  # (3)
    computeConfiguration: ComputeConfigurationTypeDef = ...,  # (4)
) -> StartProtectedQueryOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ProtectedQueryTypeType](./literals.md#protectedquerytypetype) 
2. See [:material-code-braces: ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef) [:material-code-braces: ProtectedQuerySQLParametersOutputTypeDef](./type_defs.md#protectedquerysqlparametersoutputtypedef) 
3. See [:material-code-braces: ProtectedQueryResultConfigurationTypeDef](./type_defs.md#protectedqueryresultconfigurationtypedef) 
4. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
5. See [:material-code-braces: StartProtectedQueryOutputTypeDef](./type_defs.md#startprotectedqueryoutputtypedef) 


```python
# start_protected_query method usage example with argument unpacking

kwargs: StartProtectedQueryInputTypeDef = {  # (1)
    "type": ...,
    "membershipIdentifier": ...,
    "sqlParameters": ...,
}

parent.start_protected_query(**kwargs)
```

1. See [:material-code-braces: StartProtectedQueryInputTypeDef](./type_defs.md#startprotectedqueryinputtypedef) 

### tag\_resource

Tags a resource.

Type annotations and code completion for `#!python session.create_client("cleanrooms").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef) 

### untag\_resource

Removes a tag or list of tags from a resource.

Type annotations and code completion for `#!python session.create_client("cleanrooms").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef) 

### update\_analysis\_template

Updates the analysis template metadata.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_analysis_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/update_analysis_template.html)

```python
# update_analysis_template method definition

await def update_analysis_template(
    self,
    *,
    membershipIdentifier: str,
    analysisTemplateIdentifier: str,
    description: str = ...,
) -> UpdateAnalysisTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAnalysisTemplateOutputTypeDef](./type_defs.md#updateanalysistemplateoutputtypedef) 


```python
# update_analysis_template method usage example with argument unpacking

kwargs: UpdateAnalysisTemplateInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "analysisTemplateIdentifier": ...,
}

parent.update_analysis_template(**kwargs)
```

1. See [:material-code-braces: UpdateAnalysisTemplateInputTypeDef](./type_defs.md#updateanalysistemplateinputtypedef) 

### update\_collaboration

Updates collaboration metadata and can only be called by the collaboration
owner.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_collaboration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/update_collaboration.html)

```python
# update_collaboration method definition

await def update_collaboration(
    self,
    *,
    collaborationIdentifier: str,
    name: str = ...,
    description: str = ...,
) -> UpdateCollaborationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateCollaborationOutputTypeDef](./type_defs.md#updatecollaborationoutputtypedef) 


```python
# update_collaboration method usage example with argument unpacking

kwargs: UpdateCollaborationInputTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.update_collaboration(**kwargs)
```

1. See [:material-code-braces: UpdateCollaborationInputTypeDef](./type_defs.md#updatecollaborationinputtypedef) 

### update\_configured\_audience\_model\_association

Provides the details necessary to update a configured audience model
association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_configured_audience_model_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/update_configured_audience_model_association.html)

```python
# update_configured_audience_model_association method definition

await def update_configured_audience_model_association(
    self,
    *,
    configuredAudienceModelAssociationIdentifier: str,
    membershipIdentifier: str,
    description: str = ...,
    name: str = ...,
) -> UpdateConfiguredAudienceModelAssociationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateConfiguredAudienceModelAssociationOutputTypeDef](./type_defs.md#updateconfiguredaudiencemodelassociationoutputtypedef) 


```python
# update_configured_audience_model_association method usage example with argument unpacking

kwargs: UpdateConfiguredAudienceModelAssociationInputTypeDef = {  # (1)
    "configuredAudienceModelAssociationIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.update_configured_audience_model_association(**kwargs)
```

1. See [:material-code-braces: UpdateConfiguredAudienceModelAssociationInputTypeDef](./type_defs.md#updateconfiguredaudiencemodelassociationinputtypedef) 

### update\_configured\_table

Updates a configured table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_configured_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/update_configured_table.html)

```python
# update_configured_table method definition

await def update_configured_table(
    self,
    *,
    configuredTableIdentifier: str,
    name: str = ...,
    description: str = ...,
) -> UpdateConfiguredTableOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateConfiguredTableOutputTypeDef](./type_defs.md#updateconfiguredtableoutputtypedef) 


```python
# update_configured_table method usage example with argument unpacking

kwargs: UpdateConfiguredTableInputTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
}

parent.update_configured_table(**kwargs)
```

1. See [:material-code-braces: UpdateConfiguredTableInputTypeDef](./type_defs.md#updateconfiguredtableinputtypedef) 

### update\_configured\_table\_analysis\_rule

Updates a configured table analysis rule.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_configured_table_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/update_configured_table_analysis_rule.html)

```python
# update_configured_table_analysis_rule method definition

await def update_configured_table_analysis_rule(
    self,
    *,
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAnalysisRulePolicyUnionTypeDef,  # (2)
) -> UpdateConfiguredTableAnalysisRuleOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef) [:material-code-braces: ConfiguredTableAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableanalysisrulepolicyoutputtypedef) 
3. See [:material-code-braces: UpdateConfiguredTableAnalysisRuleOutputTypeDef](./type_defs.md#updateconfiguredtableanalysisruleoutputtypedef) 


```python
# update_configured_table_analysis_rule method usage example with argument unpacking

kwargs: UpdateConfiguredTableAnalysisRuleInputTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
    "analysisRuleType": ...,
    "analysisRulePolicy": ...,
}

parent.update_configured_table_analysis_rule(**kwargs)
```

1. See [:material-code-braces: UpdateConfiguredTableAnalysisRuleInputTypeDef](./type_defs.md#updateconfiguredtableanalysisruleinputtypedef) 

### update\_configured\_table\_association

Updates a configured table association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_configured_table_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/update_configured_table_association.html)

```python
# update_configured_table_association method definition

await def update_configured_table_association(
    self,
    *,
    configuredTableAssociationIdentifier: str,
    membershipIdentifier: str,
    description: str = ...,
    roleArn: str = ...,
) -> UpdateConfiguredTableAssociationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateConfiguredTableAssociationOutputTypeDef](./type_defs.md#updateconfiguredtableassociationoutputtypedef) 


```python
# update_configured_table_association method usage example with argument unpacking

kwargs: UpdateConfiguredTableAssociationInputTypeDef = {  # (1)
    "configuredTableAssociationIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.update_configured_table_association(**kwargs)
```

1. See [:material-code-braces: UpdateConfiguredTableAssociationInputTypeDef](./type_defs.md#updateconfiguredtableassociationinputtypedef) 

### update\_configured\_table\_association\_analysis\_rule

Updates the analysis rule for a configured table association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_configured_table_association_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/update_configured_table_association_analysis_rule.html)

```python
# update_configured_table_association_analysis_rule method definition

await def update_configured_table_association_analysis_rule(
    self,
    *,
    membershipIdentifier: str,
    configuredTableAssociationIdentifier: str,
    analysisRuleType: ConfiguredTableAssociationAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAssociationAnalysisRulePolicyUnionTypeDef,  # (2)
) -> UpdateConfiguredTableAssociationAnalysisRuleOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ConfiguredTableAssociationAnalysisRuleTypeType](./literals.md#configuredtableassociationanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAssociationAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicytypedef) [:material-code-braces: ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicyoutputtypedef) 
3. See [:material-code-braces: UpdateConfiguredTableAssociationAnalysisRuleOutputTypeDef](./type_defs.md#updateconfiguredtableassociationanalysisruleoutputtypedef) 


```python
# update_configured_table_association_analysis_rule method usage example with argument unpacking

kwargs: UpdateConfiguredTableAssociationAnalysisRuleInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "configuredTableAssociationIdentifier": ...,
    "analysisRuleType": ...,
    "analysisRulePolicy": ...,
}

parent.update_configured_table_association_analysis_rule(**kwargs)
```

1. See [:material-code-braces: UpdateConfiguredTableAssociationAnalysisRuleInputTypeDef](./type_defs.md#updateconfiguredtableassociationanalysisruleinputtypedef) 

### update\_id\_mapping\_table

Provides the details that are necessary to update an ID mapping table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_id_mapping_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/update_id_mapping_table.html)

```python
# update_id_mapping_table method definition

await def update_id_mapping_table(
    self,
    *,
    idMappingTableIdentifier: str,
    membershipIdentifier: str,
    description: str = ...,
    kmsKeyArn: str = ...,
) -> UpdateIdMappingTableOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateIdMappingTableOutputTypeDef](./type_defs.md#updateidmappingtableoutputtypedef) 


```python
# update_id_mapping_table method usage example with argument unpacking

kwargs: UpdateIdMappingTableInputTypeDef = {  # (1)
    "idMappingTableIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.update_id_mapping_table(**kwargs)
```

1. See [:material-code-braces: UpdateIdMappingTableInputTypeDef](./type_defs.md#updateidmappingtableinputtypedef) 

### update\_id\_namespace\_association

Provides the details that are necessary to update an ID namespace association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_id_namespace_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/update_id_namespace_association.html)

```python
# update_id_namespace_association method definition

await def update_id_namespace_association(
    self,
    *,
    idNamespaceAssociationIdentifier: str,
    membershipIdentifier: str,
    name: str = ...,
    description: str = ...,
    idMappingConfig: IdMappingConfigTypeDef = ...,  # (1)
) -> UpdateIdNamespaceAssociationOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IdMappingConfigTypeDef](./type_defs.md#idmappingconfigtypedef) 
2. See [:material-code-braces: UpdateIdNamespaceAssociationOutputTypeDef](./type_defs.md#updateidnamespaceassociationoutputtypedef) 


```python
# update_id_namespace_association method usage example with argument unpacking

kwargs: UpdateIdNamespaceAssociationInputTypeDef = {  # (1)
    "idNamespaceAssociationIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.update_id_namespace_association(**kwargs)
```

1. See [:material-code-braces: UpdateIdNamespaceAssociationInputTypeDef](./type_defs.md#updateidnamespaceassociationinputtypedef) 

### update\_membership

Updates a membership.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/update_membership.html)

```python
# update_membership method definition

await def update_membership(
    self,
    *,
    membershipIdentifier: str,
    queryLogStatus: MembershipQueryLogStatusType = ...,  # (1)
    defaultResultConfiguration: MembershipProtectedQueryResultConfigurationTypeDef = ...,  # (2)
) -> UpdateMembershipOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype) 
2. See [:material-code-braces: MembershipProtectedQueryResultConfigurationTypeDef](./type_defs.md#membershipprotectedqueryresultconfigurationtypedef) 
3. See [:material-code-braces: UpdateMembershipOutputTypeDef](./type_defs.md#updatemembershipoutputtypedef) 


```python
# update_membership method usage example with argument unpacking

kwargs: UpdateMembershipInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.update_membership(**kwargs)
```

1. See [:material-code-braces: UpdateMembershipInputTypeDef](./type_defs.md#updatemembershipinputtypedef) 

### update\_privacy\_budget\_template

Updates the privacy budget template for the specified membership.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_privacy_budget_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/update_privacy_budget_template.html)

```python
# update_privacy_budget_template method definition

await def update_privacy_budget_template(
    self,
    *,
    membershipIdentifier: str,
    privacyBudgetTemplateIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    parameters: PrivacyBudgetTemplateUpdateParametersTypeDef = ...,  # (2)
) -> UpdatePrivacyBudgetTemplateOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-braces: PrivacyBudgetTemplateUpdateParametersTypeDef](./type_defs.md#privacybudgettemplateupdateparameterstypedef) 
3. See [:material-code-braces: UpdatePrivacyBudgetTemplateOutputTypeDef](./type_defs.md#updateprivacybudgettemplateoutputtypedef) 


```python
# update_privacy_budget_template method usage example with argument unpacking

kwargs: UpdatePrivacyBudgetTemplateInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "privacyBudgetTemplateIdentifier": ...,
    "privacyBudgetType": ...,
}

parent.update_privacy_budget_template(**kwargs)
```

1. See [:material-code-braces: UpdatePrivacyBudgetTemplateInputTypeDef](./type_defs.md#updateprivacybudgettemplateinputtypedef) 

### update\_protected\_query

Updates the processing of a currently running query.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_protected_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/client/update_protected_query.html)

```python
# update_protected_query method definition

await def update_protected_query(
    self,
    *,
    membershipIdentifier: str,
    protectedQueryIdentifier: str,
    targetStatus: TargetProtectedQueryStatusType,  # (1)
) -> UpdateProtectedQueryOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TargetProtectedQueryStatusType](./literals.md#targetprotectedquerystatustype) 
2. See [:material-code-braces: UpdateProtectedQueryOutputTypeDef](./type_defs.md#updateprotectedqueryoutputtypedef) 


```python
# update_protected_query method usage example with argument unpacking

kwargs: UpdateProtectedQueryInputTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "protectedQueryIdentifier": ...,
    "targetStatus": ...,
}

parent.update_protected_query(**kwargs)
```

1. See [:material-code-braces: UpdateProtectedQueryInputTypeDef](./type_defs.md#updateprotectedqueryinputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cleanrooms").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cleanrooms").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client)

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

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator` method with overloads.

- `client.get_paginator("list_analysis_templates")` -> [ListAnalysisTemplatesPaginator](./paginators.md#listanalysistemplatespaginator)
- `client.get_paginator("list_collaboration_analysis_templates")` -> [ListCollaborationAnalysisTemplatesPaginator](./paginators.md#listcollaborationanalysistemplatespaginator)
- `client.get_paginator("list_collaboration_configured_audience_model_associations")` -> [ListCollaborationConfiguredAudienceModelAssociationsPaginator](./paginators.md#listcollaborationconfiguredaudiencemodelassociationspaginator)
- `client.get_paginator("list_collaboration_id_namespace_associations")` -> [ListCollaborationIdNamespaceAssociationsPaginator](./paginators.md#listcollaborationidnamespaceassociationspaginator)
- `client.get_paginator("list_collaboration_privacy_budget_templates")` -> [ListCollaborationPrivacyBudgetTemplatesPaginator](./paginators.md#listcollaborationprivacybudgettemplatespaginator)
- `client.get_paginator("list_collaboration_privacy_budgets")` -> [ListCollaborationPrivacyBudgetsPaginator](./paginators.md#listcollaborationprivacybudgetspaginator)
- `client.get_paginator("list_collaborations")` -> [ListCollaborationsPaginator](./paginators.md#listcollaborationspaginator)
- `client.get_paginator("list_configured_audience_model_associations")` -> [ListConfiguredAudienceModelAssociationsPaginator](./paginators.md#listconfiguredaudiencemodelassociationspaginator)
- `client.get_paginator("list_configured_table_associations")` -> [ListConfiguredTableAssociationsPaginator](./paginators.md#listconfiguredtableassociationspaginator)
- `client.get_paginator("list_configured_tables")` -> [ListConfiguredTablesPaginator](./paginators.md#listconfiguredtablespaginator)
- `client.get_paginator("list_id_mapping_tables")` -> [ListIdMappingTablesPaginator](./paginators.md#listidmappingtablespaginator)
- `client.get_paginator("list_id_namespace_associations")` -> [ListIdNamespaceAssociationsPaginator](./paginators.md#listidnamespaceassociationspaginator)
- `client.get_paginator("list_members")` -> [ListMembersPaginator](./paginators.md#listmemberspaginator)
- `client.get_paginator("list_memberships")` -> [ListMembershipsPaginator](./paginators.md#listmembershipspaginator)
- `client.get_paginator("list_privacy_budget_templates")` -> [ListPrivacyBudgetTemplatesPaginator](./paginators.md#listprivacybudgettemplatespaginator)
- `client.get_paginator("list_privacy_budgets")` -> [ListPrivacyBudgetsPaginator](./paginators.md#listprivacybudgetspaginator)
- `client.get_paginator("list_protected_queries")` -> [ListProtectedQueriesPaginator](./paginators.md#listprotectedqueriespaginator)
- `client.get_paginator("list_schemas")` -> [ListSchemasPaginator](./paginators.md#listschemaspaginator)



