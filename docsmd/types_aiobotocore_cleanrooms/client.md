# CleanRoomsServiceClient

> [Index](../README.md) > [CleanRoomsService](./README.md) > CleanRoomsServiceClient

!!! note ""

    Auto-generated documentation for [CleanRoomsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
    type annotations stubs module [types-aiobotocore-cleanrooms](https://pypi.org/project/types-aiobotocore-cleanrooms/).

## CleanRoomsServiceClient

Type annotations and code completion for `#!python session.create_client("cleanrooms")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client)

```python
CleanRoomsServiceClient usage example

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
CleanRoomsServiceClient.exceptions usage example

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
CleanRoomsServiceClient usage type checking example

from types_aiobotocore_cleanrooms.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### batch\_get\_collaboration\_analysis\_template

Retrieves multiple analysis templates within a collaboration by their Amazon
Resource Names (ARNs).

Type annotations and code completion for `#!python session.create_client("cleanrooms").batch_get_collaboration_analysis_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.batch_get_collaboration_analysis_template)

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

kwargs: BatchGetCollaborationAnalysisTemplateInputRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "analysisTemplateArns": ...,
}

parent.batch_get_collaboration_analysis_template(**kwargs)
```

1. See [:material-code-braces: BatchGetCollaborationAnalysisTemplateInputRequestTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateinputrequesttypedef) 

### batch\_get\_schema

Retrieves multiple schemas by their identifiers.

Type annotations and code completion for `#!python session.create_client("cleanrooms").batch_get_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.batch_get_schema)

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

kwargs: BatchGetSchemaInputRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "names": ...,
}

parent.batch_get_schema(**kwargs)
```

1. See [:material-code-braces: BatchGetSchemaInputRequestTypeDef](./type_defs.md#batchgetschemainputrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("cleanrooms").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("cleanrooms").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_analysis\_template

Creates a new analysis template.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_analysis_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_analysis_template)

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

kwargs: CreateAnalysisTemplateInputRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "name": ...,
    "format": ...,
    "source": ...,
}

parent.create_analysis_template(**kwargs)
```

1. See [:material-code-braces: CreateAnalysisTemplateInputRequestTypeDef](./type_defs.md#createanalysistemplateinputrequesttypedef) 

### create\_collaboration

Creates a new collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_collaboration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_collaboration)

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
    dataEncryptionMetadata: DataEncryptionMetadataTypeDef = ...,  # (4)
    tags: Mapping[str, str] = ...,
) -> CreateCollaborationOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: MemberSpecificationTypeDef](./type_defs.md#memberspecificationtypedef) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
3. See [:material-code-brackets: CollaborationQueryLogStatusType](./literals.md#collaborationquerylogstatustype) 
4. See [:material-code-braces: DataEncryptionMetadataTypeDef](./type_defs.md#dataencryptionmetadatatypedef) 
5. See [:material-code-braces: CreateCollaborationOutputTypeDef](./type_defs.md#createcollaborationoutputtypedef) 


```python
# create_collaboration method usage example with argument unpacking

kwargs: CreateCollaborationInputRequestTypeDef = {  # (1)
    "members": ...,
    "name": ...,
    "description": ...,
    "creatorMemberAbilities": ...,
    "creatorDisplayName": ...,
    "queryLogStatus": ...,
}

parent.create_collaboration(**kwargs)
```

1. See [:material-code-braces: CreateCollaborationInputRequestTypeDef](./type_defs.md#createcollaborationinputrequesttypedef) 

### create\_configured\_table

Creates a new configured table resource.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_configured_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table)

```python
# create_configured_table method definition

await def create_configured_table(
    self,
    *,
    name: str,
    tableReference: TableReferenceTypeDef,  # (1)
    allowedColumns: Sequence[str],
    analysisMethod: AnalysisMethodType,  # (2)
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateConfiguredTableOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TableReferenceTypeDef](./type_defs.md#tablereferencetypedef) 
2. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
3. See [:material-code-braces: CreateConfiguredTableOutputTypeDef](./type_defs.md#createconfiguredtableoutputtypedef) 


```python
# create_configured_table method usage example with argument unpacking

kwargs: CreateConfiguredTableInputRequestTypeDef = {  # (1)
    "name": ...,
    "tableReference": ...,
    "allowedColumns": ...,
    "analysisMethod": ...,
}

parent.create_configured_table(**kwargs)
```

1. See [:material-code-braces: CreateConfiguredTableInputRequestTypeDef](./type_defs.md#createconfiguredtableinputrequesttypedef) 

### create\_configured\_table\_analysis\_rule

Creates a new analysis rule for a configured table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_configured_table_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_analysis_rule)

```python
# create_configured_table_analysis_rule method definition

await def create_configured_table_analysis_rule(
    self,
    *,
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef,  # (2)
) -> CreateConfiguredTableAnalysisRuleOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef) 
3. See [:material-code-braces: CreateConfiguredTableAnalysisRuleOutputTypeDef](./type_defs.md#createconfiguredtableanalysisruleoutputtypedef) 


```python
# create_configured_table_analysis_rule method usage example with argument unpacking

kwargs: CreateConfiguredTableAnalysisRuleInputRequestTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
    "analysisRuleType": ...,
    "analysisRulePolicy": ...,
}

parent.create_configured_table_analysis_rule(**kwargs)
```

1. See [:material-code-braces: CreateConfiguredTableAnalysisRuleInputRequestTypeDef](./type_defs.md#createconfiguredtableanalysisruleinputrequesttypedef) 

### create\_configured\_table\_association

Creates a configured table association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_configured_table_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_association)

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

kwargs: CreateConfiguredTableAssociationInputRequestTypeDef = {  # (1)
    "name": ...,
    "membershipIdentifier": ...,
    "configuredTableIdentifier": ...,
    "roleArn": ...,
}

parent.create_configured_table_association(**kwargs)
```

1. See [:material-code-braces: CreateConfiguredTableAssociationInputRequestTypeDef](./type_defs.md#createconfiguredtableassociationinputrequesttypedef) 

### create\_membership

Creates a membership for a specific collaboration identifier and joins the
collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").create_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_membership)

```python
# create_membership method definition

await def create_membership(
    self,
    *,
    collaborationIdentifier: str,
    queryLogStatus: MembershipQueryLogStatusType,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateMembershipOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype) 
2. See [:material-code-braces: CreateMembershipOutputTypeDef](./type_defs.md#createmembershipoutputtypedef) 


```python
# create_membership method usage example with argument unpacking

kwargs: CreateMembershipInputRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "queryLogStatus": ...,
}

parent.create_membership(**kwargs)
```

1. See [:material-code-braces: CreateMembershipInputRequestTypeDef](./type_defs.md#createmembershipinputrequesttypedef) 

### delete\_analysis\_template

Deletes an analysis template.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_analysis_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_analysis_template)

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

kwargs: DeleteAnalysisTemplateInputRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "analysisTemplateIdentifier": ...,
}

parent.delete_analysis_template(**kwargs)
```

1. See [:material-code-braces: DeleteAnalysisTemplateInputRequestTypeDef](./type_defs.md#deleteanalysistemplateinputrequesttypedef) 

### delete\_collaboration

Deletes a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_collaboration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_collaboration)

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

kwargs: DeleteCollaborationInputRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.delete_collaboration(**kwargs)
```

1. See [:material-code-braces: DeleteCollaborationInputRequestTypeDef](./type_defs.md#deletecollaborationinputrequesttypedef) 

### delete\_configured\_table

Deletes a configured table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_configured_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_configured_table)

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

kwargs: DeleteConfiguredTableInputRequestTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
}

parent.delete_configured_table(**kwargs)
```

1. See [:material-code-braces: DeleteConfiguredTableInputRequestTypeDef](./type_defs.md#deleteconfiguredtableinputrequesttypedef) 

### delete\_configured\_table\_analysis\_rule

Deletes a configured table analysis rule.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_configured_table_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_configured_table_analysis_rule)

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

kwargs: DeleteConfiguredTableAnalysisRuleInputRequestTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
    "analysisRuleType": ...,
}

parent.delete_configured_table_analysis_rule(**kwargs)
```

1. See [:material-code-braces: DeleteConfiguredTableAnalysisRuleInputRequestTypeDef](./type_defs.md#deleteconfiguredtableanalysisruleinputrequesttypedef) 

### delete\_configured\_table\_association

Deletes a configured table association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_configured_table_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_configured_table_association)

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

kwargs: DeleteConfiguredTableAssociationInputRequestTypeDef = {  # (1)
    "configuredTableAssociationIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.delete_configured_table_association(**kwargs)
```

1. See [:material-code-braces: DeleteConfiguredTableAssociationInputRequestTypeDef](./type_defs.md#deleteconfiguredtableassociationinputrequesttypedef) 

### delete\_member

Removes the specified member from a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_member` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_member)

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

kwargs: DeleteMemberInputRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "accountId": ...,
}

parent.delete_member(**kwargs)
```

1. See [:material-code-braces: DeleteMemberInputRequestTypeDef](./type_defs.md#deletememberinputrequesttypedef) 

### delete\_membership

Deletes a specified membership.

Type annotations and code completion for `#!python session.create_client("cleanrooms").delete_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_membership)

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

kwargs: DeleteMembershipInputRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.delete_membership(**kwargs)
```

1. See [:material-code-braces: DeleteMembershipInputRequestTypeDef](./type_defs.md#deletemembershipinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("cleanrooms").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.generate_presigned_url)

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


### get\_analysis\_template

Retrieves an analysis template.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_analysis_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_analysis_template)

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

kwargs: GetAnalysisTemplateInputRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "analysisTemplateIdentifier": ...,
}

parent.get_analysis_template(**kwargs)
```

1. See [:material-code-braces: GetAnalysisTemplateInputRequestTypeDef](./type_defs.md#getanalysistemplateinputrequesttypedef) 

### get\_collaboration

Returns metadata about a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_collaboration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_collaboration)

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

kwargs: GetCollaborationInputRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.get_collaboration(**kwargs)
```

1. See [:material-code-braces: GetCollaborationInputRequestTypeDef](./type_defs.md#getcollaborationinputrequesttypedef) 

### get\_collaboration\_analysis\_template

Retrieves an analysis template within a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_collaboration_analysis_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_collaboration_analysis_template)

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

kwargs: GetCollaborationAnalysisTemplateInputRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "analysisTemplateArn": ...,
}

parent.get_collaboration_analysis_template(**kwargs)
```

1. See [:material-code-braces: GetCollaborationAnalysisTemplateInputRequestTypeDef](./type_defs.md#getcollaborationanalysistemplateinputrequesttypedef) 

### get\_configured\_table

Retrieves a configured table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_configured_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_configured_table)

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

kwargs: GetConfiguredTableInputRequestTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
}

parent.get_configured_table(**kwargs)
```

1. See [:material-code-braces: GetConfiguredTableInputRequestTypeDef](./type_defs.md#getconfiguredtableinputrequesttypedef) 

### get\_configured\_table\_analysis\_rule

Retrieves a configured table analysis rule.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_configured_table_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_configured_table_analysis_rule)

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

kwargs: GetConfiguredTableAnalysisRuleInputRequestTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
    "analysisRuleType": ...,
}

parent.get_configured_table_analysis_rule(**kwargs)
```

1. See [:material-code-braces: GetConfiguredTableAnalysisRuleInputRequestTypeDef](./type_defs.md#getconfiguredtableanalysisruleinputrequesttypedef) 

### get\_configured\_table\_association

Retrieves a configured table association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_configured_table_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_configured_table_association)

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

kwargs: GetConfiguredTableAssociationInputRequestTypeDef = {  # (1)
    "configuredTableAssociationIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.get_configured_table_association(**kwargs)
```

1. See [:material-code-braces: GetConfiguredTableAssociationInputRequestTypeDef](./type_defs.md#getconfiguredtableassociationinputrequesttypedef) 

### get\_membership

Retrieves a specified membership for an identifier.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_membership)

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

kwargs: GetMembershipInputRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.get_membership(**kwargs)
```

1. See [:material-code-braces: GetMembershipInputRequestTypeDef](./type_defs.md#getmembershipinputrequesttypedef) 

### get\_protected\_query

Returns query processing metadata.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_protected_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_protected_query)

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

kwargs: GetProtectedQueryInputRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "protectedQueryIdentifier": ...,
}

parent.get_protected_query(**kwargs)
```

1. See [:material-code-braces: GetProtectedQueryInputRequestTypeDef](./type_defs.md#getprotectedqueryinputrequesttypedef) 

### get\_schema

Retrieves the schema for a relation within a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_schema)

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

kwargs: GetSchemaInputRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "name": ...,
}

parent.get_schema(**kwargs)
```

1. See [:material-code-braces: GetSchemaInputRequestTypeDef](./type_defs.md#getschemainputrequesttypedef) 

### get\_schema\_analysis\_rule

Retrieves a schema analysis rule.

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_schema_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_schema_analysis_rule)

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

kwargs: GetSchemaAnalysisRuleInputRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "name": ...,
    "type": ...,
}

parent.get_schema_analysis_rule(**kwargs)
```

1. See [:material-code-braces: GetSchemaAnalysisRuleInputRequestTypeDef](./type_defs.md#getschemaanalysisruleinputrequesttypedef) 

### list\_analysis\_templates

Lists analysis templates that the caller owns.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_analysis_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_analysis_templates)

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

kwargs: ListAnalysisTemplatesInputRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_analysis_templates(**kwargs)
```

1. See [:material-code-braces: ListAnalysisTemplatesInputRequestTypeDef](./type_defs.md#listanalysistemplatesinputrequesttypedef) 

### list\_collaboration\_analysis\_templates

Lists analysis templates within a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_collaboration_analysis_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_collaboration_analysis_templates)

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

kwargs: ListCollaborationAnalysisTemplatesInputRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.list_collaboration_analysis_templates(**kwargs)
```

1. See [:material-code-braces: ListCollaborationAnalysisTemplatesInputRequestTypeDef](./type_defs.md#listcollaborationanalysistemplatesinputrequesttypedef) 

### list\_collaborations

Lists collaborations the caller owns, is active in, or has been invited to.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_collaborations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_collaborations)

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

kwargs: ListCollaborationsInputRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_collaborations(**kwargs)
```

1. See [:material-code-braces: ListCollaborationsInputRequestTypeDef](./type_defs.md#listcollaborationsinputrequesttypedef) 

### list\_configured\_table\_associations

Lists configured table associations for a membership.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_configured_table_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_configured_table_associations)

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

kwargs: ListConfiguredTableAssociationsInputRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_configured_table_associations(**kwargs)
```

1. See [:material-code-braces: ListConfiguredTableAssociationsInputRequestTypeDef](./type_defs.md#listconfiguredtableassociationsinputrequesttypedef) 

### list\_configured\_tables

Lists configured tables.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_configured_tables` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_configured_tables)

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

kwargs: ListConfiguredTablesInputRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_configured_tables(**kwargs)
```

1. See [:material-code-braces: ListConfiguredTablesInputRequestTypeDef](./type_defs.md#listconfiguredtablesinputrequesttypedef) 

### list\_members

Lists all members within a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_members)

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

kwargs: ListMembersInputRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.list_members(**kwargs)
```

1. See [:material-code-braces: ListMembersInputRequestTypeDef](./type_defs.md#listmembersinputrequesttypedef) 

### list\_memberships

Lists all memberships resources within the caller's account.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_memberships` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_memberships)

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

kwargs: ListMembershipsInputRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_memberships(**kwargs)
```

1. See [:material-code-braces: ListMembershipsInputRequestTypeDef](./type_defs.md#listmembershipsinputrequesttypedef) 

### list\_protected\_queries

Lists protected queries, sorted by the most recent query.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_protected_queries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_protected_queries)

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

kwargs: ListProtectedQueriesInputRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_protected_queries(**kwargs)
```

1. See [:material-code-braces: ListProtectedQueriesInputRequestTypeDef](./type_defs.md#listprotectedqueriesinputrequesttypedef) 

### list\_schemas

Lists the schemas for relations within a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_schemas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_schemas)

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

kwargs: ListSchemasInputRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.list_schemas(**kwargs)
```

1. See [:material-code-braces: ListSchemasInputRequestTypeDef](./type_defs.md#listschemasinputrequesttypedef) 

### list\_tags\_for\_resource

Lists all of the tags that have been added to a resource.

Type annotations and code completion for `#!python session.create_client("cleanrooms").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_tags_for_resource)

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

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### start\_protected\_query

Creates a protected query that is started by Clean Rooms .

Type annotations and code completion for `#!python session.create_client("cleanrooms").start_protected_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.start_protected_query)

```python
# start_protected_query method definition

await def start_protected_query(
    self,
    *,
    type: ProtectedQueryTypeType,  # (1)
    membershipIdentifier: str,
    sqlParameters: ProtectedQuerySQLParametersTypeDef,  # (2)
    resultConfiguration: ProtectedQueryResultConfigurationTypeDef,  # (3)
) -> StartProtectedQueryOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ProtectedQueryTypeType](./literals.md#protectedquerytypetype) 
2. See [:material-code-braces: ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef) 
3. See [:material-code-braces: ProtectedQueryResultConfigurationTypeDef](./type_defs.md#protectedqueryresultconfigurationtypedef) 
4. See [:material-code-braces: StartProtectedQueryOutputTypeDef](./type_defs.md#startprotectedqueryoutputtypedef) 


```python
# start_protected_query method usage example with argument unpacking

kwargs: StartProtectedQueryInputRequestTypeDef = {  # (1)
    "type": ...,
    "membershipIdentifier": ...,
    "sqlParameters": ...,
    "resultConfiguration": ...,
}

parent.start_protected_query(**kwargs)
```

1. See [:material-code-braces: StartProtectedQueryInputRequestTypeDef](./type_defs.md#startprotectedqueryinputrequesttypedef) 

### tag\_resource

Tags a resource.

Type annotations and code completion for `#!python session.create_client("cleanrooms").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.tag_resource)

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

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Removes a tag or list of tags from a resource.

Type annotations and code completion for `#!python session.create_client("cleanrooms").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.untag_resource)

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

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_analysis\_template

Updates the analysis template metadata.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_analysis_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_analysis_template)

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

kwargs: UpdateAnalysisTemplateInputRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "analysisTemplateIdentifier": ...,
}

parent.update_analysis_template(**kwargs)
```

1. See [:material-code-braces: UpdateAnalysisTemplateInputRequestTypeDef](./type_defs.md#updateanalysistemplateinputrequesttypedef) 

### update\_collaboration

Updates collaboration metadata and can only be called by the collaboration
owner.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_collaboration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_collaboration)

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

kwargs: UpdateCollaborationInputRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.update_collaboration(**kwargs)
```

1. See [:material-code-braces: UpdateCollaborationInputRequestTypeDef](./type_defs.md#updatecollaborationinputrequesttypedef) 

### update\_configured\_table

Updates a configured table.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_configured_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table)

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

kwargs: UpdateConfiguredTableInputRequestTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
}

parent.update_configured_table(**kwargs)
```

1. See [:material-code-braces: UpdateConfiguredTableInputRequestTypeDef](./type_defs.md#updateconfiguredtableinputrequesttypedef) 

### update\_configured\_table\_analysis\_rule

Updates a configured table analysis rule.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_configured_table_analysis_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_analysis_rule)

```python
# update_configured_table_analysis_rule method definition

await def update_configured_table_analysis_rule(
    self,
    *,
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef,  # (2)
) -> UpdateConfiguredTableAnalysisRuleOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef) 
3. See [:material-code-braces: UpdateConfiguredTableAnalysisRuleOutputTypeDef](./type_defs.md#updateconfiguredtableanalysisruleoutputtypedef) 


```python
# update_configured_table_analysis_rule method usage example with argument unpacking

kwargs: UpdateConfiguredTableAnalysisRuleInputRequestTypeDef = {  # (1)
    "configuredTableIdentifier": ...,
    "analysisRuleType": ...,
    "analysisRulePolicy": ...,
}

parent.update_configured_table_analysis_rule(**kwargs)
```

1. See [:material-code-braces: UpdateConfiguredTableAnalysisRuleInputRequestTypeDef](./type_defs.md#updateconfiguredtableanalysisruleinputrequesttypedef) 

### update\_configured\_table\_association

Updates a configured table association.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_configured_table_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_association)

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

kwargs: UpdateConfiguredTableAssociationInputRequestTypeDef = {  # (1)
    "configuredTableAssociationIdentifier": ...,
    "membershipIdentifier": ...,
}

parent.update_configured_table_association(**kwargs)
```

1. See [:material-code-braces: UpdateConfiguredTableAssociationInputRequestTypeDef](./type_defs.md#updateconfiguredtableassociationinputrequesttypedef) 

### update\_membership

Updates a membership.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_membership)

```python
# update_membership method definition

await def update_membership(
    self,
    *,
    membershipIdentifier: str,
    queryLogStatus: MembershipQueryLogStatusType = ...,  # (1)
) -> UpdateMembershipOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype) 
2. See [:material-code-braces: UpdateMembershipOutputTypeDef](./type_defs.md#updatemembershipoutputtypedef) 


```python
# update_membership method usage example with argument unpacking

kwargs: UpdateMembershipInputRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.update_membership(**kwargs)
```

1. See [:material-code-braces: UpdateMembershipInputRequestTypeDef](./type_defs.md#updatemembershipinputrequesttypedef) 

### update\_protected\_query

Updates the processing of a currently running query.

Type annotations and code completion for `#!python session.create_client("cleanrooms").update_protected_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_protected_query)

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

kwargs: UpdateProtectedQueryInputRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "protectedQueryIdentifier": ...,
    "targetStatus": ...,
}

parent.update_protected_query(**kwargs)
```

1. See [:material-code-braces: UpdateProtectedQueryInputRequestTypeDef](./type_defs.md#updateprotectedqueryinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cleanrooms").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> CleanRoomsServiceClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cleanrooms").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator` method with overloads.

- `client.get_paginator("list_analysis_templates")` -> [ListAnalysisTemplatesPaginator](./paginators.md#listanalysistemplatespaginator)
- `client.get_paginator("list_collaboration_analysis_templates")` -> [ListCollaborationAnalysisTemplatesPaginator](./paginators.md#listcollaborationanalysistemplatespaginator)
- `client.get_paginator("list_collaborations")` -> [ListCollaborationsPaginator](./paginators.md#listcollaborationspaginator)
- `client.get_paginator("list_configured_table_associations")` -> [ListConfiguredTableAssociationsPaginator](./paginators.md#listconfiguredtableassociationspaginator)
- `client.get_paginator("list_configured_tables")` -> [ListConfiguredTablesPaginator](./paginators.md#listconfiguredtablespaginator)
- `client.get_paginator("list_members")` -> [ListMembersPaginator](./paginators.md#listmemberspaginator)
- `client.get_paginator("list_memberships")` -> [ListMembershipsPaginator](./paginators.md#listmembershipspaginator)
- `client.get_paginator("list_protected_queries")` -> [ListProtectedQueriesPaginator](./paginators.md#listprotectedqueriespaginator)
- `client.get_paginator("list_schemas")` -> [ListSchemasPaginator](./paginators.md#listschemaspaginator)



