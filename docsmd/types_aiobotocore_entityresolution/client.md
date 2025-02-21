# EntityResolutionClient

> [Index](../README.md) > [EntityResolution](./README.md) > EntityResolutionClient

!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#entityresolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## EntityResolutionClient

Type annotations and code completion for `#!python session.create_client("entityresolution")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client)

```python
# EntityResolutionClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_entityresolution.client import EntityResolutionClient

session = get_session()
async with session.create_client("entityresolution") as client:
    client: EntityResolutionClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("entityresolution").exceptions` structure.

```python
# EntityResolutionClient.exceptions usage example

async with session.create_client("entityresolution") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.ExceedsLimitException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# EntityResolutionClient usage type checking example

from types_aiobotocore_entityresolution.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("entityresolution").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("entityresolution").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/generate_presigned_url.html)

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


### add\_policy\_statement

Adds a policy statement object.

Type annotations and code completion for `#!python session.create_client("entityresolution").add_policy_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/add_policy_statement.html)

```python
# add_policy_statement method definition

await def add_policy_statement(
    self,
    *,
    action: Sequence[str],
    arn: str,
    effect: StatementEffectType,  # (1)
    principal: Sequence[str],
    statementId: str,
    condition: str = ...,
) -> AddPolicyStatementOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StatementEffectType](./literals.md#statementeffecttype) 
2. See [:material-code-braces: AddPolicyStatementOutputTypeDef](./type_defs.md#addpolicystatementoutputtypedef) 


```python
# add_policy_statement method usage example with argument unpacking

kwargs: AddPolicyStatementInputTypeDef = {  # (1)
    "action": ...,
    "arn": ...,
    "effect": ...,
    "principal": ...,
    "statementId": ...,
}

parent.add_policy_statement(**kwargs)
```

1. See [:material-code-braces: AddPolicyStatementInputTypeDef](./type_defs.md#addpolicystatementinputtypedef) 

### batch\_delete\_unique\_id

Deletes multiple unique IDs in a matching workflow.

Type annotations and code completion for `#!python session.create_client("entityresolution").batch_delete_unique_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/batch_delete_unique_id.html)

```python
# batch_delete_unique_id method definition

await def batch_delete_unique_id(
    self,
    *,
    uniqueIds: Sequence[str],
    workflowName: str,
    inputSource: str = ...,
) -> BatchDeleteUniqueIdOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteUniqueIdOutputTypeDef](./type_defs.md#batchdeleteuniqueidoutputtypedef) 


```python
# batch_delete_unique_id method usage example with argument unpacking

kwargs: BatchDeleteUniqueIdInputTypeDef = {  # (1)
    "uniqueIds": ...,
    "workflowName": ...,
}

parent.batch_delete_unique_id(**kwargs)
```

1. See [:material-code-braces: BatchDeleteUniqueIdInputTypeDef](./type_defs.md#batchdeleteuniqueidinputtypedef) 

### create\_id\_mapping\_workflow

Creates an <code>IdMappingWorkflow</code> object which stores the configuration
of the data processing job to be run.

Type annotations and code completion for `#!python session.create_client("entityresolution").create_id_mapping_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/create_id_mapping_workflow.html)

```python
# create_id_mapping_workflow method definition

await def create_id_mapping_workflow(
    self,
    *,
    idMappingTechniques: IdMappingTechniquesUnionTypeDef,  # (1)
    inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],  # (2)
    workflowName: str,
    description: str = ...,
    outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef] = ...,  # (3)
    roleArn: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateIdMappingWorkflowOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) [:material-code-braces: IdMappingTechniquesOutputTypeDef](./type_defs.md#idmappingtechniquesoutputtypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
4. See [:material-code-braces: CreateIdMappingWorkflowOutputTypeDef](./type_defs.md#createidmappingworkflowoutputtypedef) 


```python
# create_id_mapping_workflow method usage example with argument unpacking

kwargs: CreateIdMappingWorkflowInputTypeDef = {  # (1)
    "idMappingTechniques": ...,
    "inputSourceConfig": ...,
    "workflowName": ...,
}

parent.create_id_mapping_workflow(**kwargs)
```

1. See [:material-code-braces: CreateIdMappingWorkflowInputTypeDef](./type_defs.md#createidmappingworkflowinputtypedef) 

### create\_id\_namespace

Creates an ID namespace object which will help customers provide metadata
explaining their dataset and how to use it.

Type annotations and code completion for `#!python session.create_client("entityresolution").create_id_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/create_id_namespace.html)

```python
# create_id_namespace method definition

await def create_id_namespace(
    self,
    *,
    idNamespaceName: str,
    type: IdNamespaceTypeType,  # (1)
    description: str = ...,
    idMappingWorkflowProperties: Sequence[IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef] = ...,  # (2)
    inputSourceConfig: Sequence[IdNamespaceInputSourceTypeDef] = ...,  # (3)
    roleArn: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateIdNamespaceOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: IdNamespaceTypeType](./literals.md#idnamespacetypetype) 
2. See [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiestypedef) [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiesoutputtypedef) 
3. See [:material-code-braces: IdNamespaceInputSourceTypeDef](./type_defs.md#idnamespaceinputsourcetypedef) 
4. See [:material-code-braces: CreateIdNamespaceOutputTypeDef](./type_defs.md#createidnamespaceoutputtypedef) 


```python
# create_id_namespace method usage example with argument unpacking

kwargs: CreateIdNamespaceInputTypeDef = {  # (1)
    "idNamespaceName": ...,
    "type": ...,
}

parent.create_id_namespace(**kwargs)
```

1. See [:material-code-braces: CreateIdNamespaceInputTypeDef](./type_defs.md#createidnamespaceinputtypedef) 

### create\_matching\_workflow

Creates a <code>MatchingWorkflow</code> object which stores the configuration
of the data processing job to be run.

Type annotations and code completion for `#!python session.create_client("entityresolution").create_matching_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/create_matching_workflow.html)

```python
# create_matching_workflow method definition

await def create_matching_workflow(
    self,
    *,
    inputSourceConfig: Sequence[InputSourceTypeDef],  # (1)
    outputSourceConfig: Sequence[OutputSourceUnionTypeDef],  # (2)
    resolutionTechniques: ResolutionTechniquesUnionTypeDef,  # (3)
    roleArn: str,
    workflowName: str,
    description: str = ...,
    incrementalRunConfig: IncrementalRunConfigTypeDef = ...,  # (4)
    tags: Mapping[str, str] = ...,
) -> CreateMatchingWorkflowOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
2. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) [:material-code-braces: OutputSourceOutputTypeDef](./type_defs.md#outputsourceoutputtypedef) 
3. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) [:material-code-braces: ResolutionTechniquesOutputTypeDef](./type_defs.md#resolutiontechniquesoutputtypedef) 
4. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
5. See [:material-code-braces: CreateMatchingWorkflowOutputTypeDef](./type_defs.md#creatematchingworkflowoutputtypedef) 


```python
# create_matching_workflow method usage example with argument unpacking

kwargs: CreateMatchingWorkflowInputTypeDef = {  # (1)
    "inputSourceConfig": ...,
    "outputSourceConfig": ...,
    "resolutionTechniques": ...,
    "roleArn": ...,
    "workflowName": ...,
}

parent.create_matching_workflow(**kwargs)
```

1. See [:material-code-braces: CreateMatchingWorkflowInputTypeDef](./type_defs.md#creatematchingworkflowinputtypedef) 

### create\_schema\_mapping

Creates a schema mapping, which defines the schema of the input customer
records table.

Type annotations and code completion for `#!python session.create_client("entityresolution").create_schema_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/create_schema_mapping.html)

```python
# create_schema_mapping method definition

await def create_schema_mapping(
    self,
    *,
    mappedInputFields: Sequence[SchemaInputAttributeTypeDef],  # (1)
    schemaName: str,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateSchemaMappingOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
2. See [:material-code-braces: CreateSchemaMappingOutputTypeDef](./type_defs.md#createschemamappingoutputtypedef) 


```python
# create_schema_mapping method usage example with argument unpacking

kwargs: CreateSchemaMappingInputTypeDef = {  # (1)
    "mappedInputFields": ...,
    "schemaName": ...,
}

parent.create_schema_mapping(**kwargs)
```

1. See [:material-code-braces: CreateSchemaMappingInputTypeDef](./type_defs.md#createschemamappinginputtypedef) 

### delete\_id\_mapping\_workflow

Deletes the <code>IdMappingWorkflow</code> with a given name.

Type annotations and code completion for `#!python session.create_client("entityresolution").delete_id_mapping_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/delete_id_mapping_workflow.html)

```python
# delete_id_mapping_workflow method definition

await def delete_id_mapping_workflow(
    self,
    *,
    workflowName: str,
) -> DeleteIdMappingWorkflowOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteIdMappingWorkflowOutputTypeDef](./type_defs.md#deleteidmappingworkflowoutputtypedef) 


```python
# delete_id_mapping_workflow method usage example with argument unpacking

kwargs: DeleteIdMappingWorkflowInputTypeDef = {  # (1)
    "workflowName": ...,
}

parent.delete_id_mapping_workflow(**kwargs)
```

1. See [:material-code-braces: DeleteIdMappingWorkflowInputTypeDef](./type_defs.md#deleteidmappingworkflowinputtypedef) 

### delete\_id\_namespace

Deletes the <code>IdNamespace</code> with a given name.

Type annotations and code completion for `#!python session.create_client("entityresolution").delete_id_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/delete_id_namespace.html)

```python
# delete_id_namespace method definition

await def delete_id_namespace(
    self,
    *,
    idNamespaceName: str,
) -> DeleteIdNamespaceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteIdNamespaceOutputTypeDef](./type_defs.md#deleteidnamespaceoutputtypedef) 


```python
# delete_id_namespace method usage example with argument unpacking

kwargs: DeleteIdNamespaceInputTypeDef = {  # (1)
    "idNamespaceName": ...,
}

parent.delete_id_namespace(**kwargs)
```

1. See [:material-code-braces: DeleteIdNamespaceInputTypeDef](./type_defs.md#deleteidnamespaceinputtypedef) 

### delete\_matching\_workflow

Deletes the <code>MatchingWorkflow</code> with a given name.

Type annotations and code completion for `#!python session.create_client("entityresolution").delete_matching_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/delete_matching_workflow.html)

```python
# delete_matching_workflow method definition

await def delete_matching_workflow(
    self,
    *,
    workflowName: str,
) -> DeleteMatchingWorkflowOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMatchingWorkflowOutputTypeDef](./type_defs.md#deletematchingworkflowoutputtypedef) 


```python
# delete_matching_workflow method usage example with argument unpacking

kwargs: DeleteMatchingWorkflowInputTypeDef = {  # (1)
    "workflowName": ...,
}

parent.delete_matching_workflow(**kwargs)
```

1. See [:material-code-braces: DeleteMatchingWorkflowInputTypeDef](./type_defs.md#deletematchingworkflowinputtypedef) 

### delete\_policy\_statement

Deletes the policy statement.

Type annotations and code completion for `#!python session.create_client("entityresolution").delete_policy_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/delete_policy_statement.html)

```python
# delete_policy_statement method definition

await def delete_policy_statement(
    self,
    *,
    arn: str,
    statementId: str,
) -> DeletePolicyStatementOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePolicyStatementOutputTypeDef](./type_defs.md#deletepolicystatementoutputtypedef) 


```python
# delete_policy_statement method usage example with argument unpacking

kwargs: DeletePolicyStatementInputTypeDef = {  # (1)
    "arn": ...,
    "statementId": ...,
}

parent.delete_policy_statement(**kwargs)
```

1. See [:material-code-braces: DeletePolicyStatementInputTypeDef](./type_defs.md#deletepolicystatementinputtypedef) 

### delete\_schema\_mapping

Deletes the <code>SchemaMapping</code> with a given name.

Type annotations and code completion for `#!python session.create_client("entityresolution").delete_schema_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/delete_schema_mapping.html)

```python
# delete_schema_mapping method definition

await def delete_schema_mapping(
    self,
    *,
    schemaName: str,
) -> DeleteSchemaMappingOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSchemaMappingOutputTypeDef](./type_defs.md#deleteschemamappingoutputtypedef) 


```python
# delete_schema_mapping method usage example with argument unpacking

kwargs: DeleteSchemaMappingInputTypeDef = {  # (1)
    "schemaName": ...,
}

parent.delete_schema_mapping(**kwargs)
```

1. See [:material-code-braces: DeleteSchemaMappingInputTypeDef](./type_defs.md#deleteschemamappinginputtypedef) 

### get\_id\_mapping\_job

Gets the status, metrics, and errors (if there are any) that are associated
with a job.

Type annotations and code completion for `#!python session.create_client("entityresolution").get_id_mapping_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/get_id_mapping_job.html)

```python
# get_id_mapping_job method definition

await def get_id_mapping_job(
    self,
    *,
    jobId: str,
    workflowName: str,
) -> GetIdMappingJobOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdMappingJobOutputTypeDef](./type_defs.md#getidmappingjoboutputtypedef) 


```python
# get_id_mapping_job method usage example with argument unpacking

kwargs: GetIdMappingJobInputTypeDef = {  # (1)
    "jobId": ...,
    "workflowName": ...,
}

parent.get_id_mapping_job(**kwargs)
```

1. See [:material-code-braces: GetIdMappingJobInputTypeDef](./type_defs.md#getidmappingjobinputtypedef) 

### get\_id\_mapping\_workflow

Returns the <code>IdMappingWorkflow</code> with a given name, if it exists.

Type annotations and code completion for `#!python session.create_client("entityresolution").get_id_mapping_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/get_id_mapping_workflow.html)

```python
# get_id_mapping_workflow method definition

await def get_id_mapping_workflow(
    self,
    *,
    workflowName: str,
) -> GetIdMappingWorkflowOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdMappingWorkflowOutputTypeDef](./type_defs.md#getidmappingworkflowoutputtypedef) 


```python
# get_id_mapping_workflow method usage example with argument unpacking

kwargs: GetIdMappingWorkflowInputTypeDef = {  # (1)
    "workflowName": ...,
}

parent.get_id_mapping_workflow(**kwargs)
```

1. See [:material-code-braces: GetIdMappingWorkflowInputTypeDef](./type_defs.md#getidmappingworkflowinputtypedef) 

### get\_id\_namespace

Returns the <code>IdNamespace</code> with a given name, if it exists.

Type annotations and code completion for `#!python session.create_client("entityresolution").get_id_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/get_id_namespace.html)

```python
# get_id_namespace method definition

await def get_id_namespace(
    self,
    *,
    idNamespaceName: str,
) -> GetIdNamespaceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdNamespaceOutputTypeDef](./type_defs.md#getidnamespaceoutputtypedef) 


```python
# get_id_namespace method usage example with argument unpacking

kwargs: GetIdNamespaceInputTypeDef = {  # (1)
    "idNamespaceName": ...,
}

parent.get_id_namespace(**kwargs)
```

1. See [:material-code-braces: GetIdNamespaceInputTypeDef](./type_defs.md#getidnamespaceinputtypedef) 

### get\_match\_id

Returns the corresponding Match ID of a customer record if the record has been
processed.

Type annotations and code completion for `#!python session.create_client("entityresolution").get_match_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/get_match_id.html)

```python
# get_match_id method definition

await def get_match_id(
    self,
    *,
    record: Mapping[str, str],
    workflowName: str,
    applyNormalization: bool = ...,
) -> GetMatchIdOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMatchIdOutputTypeDef](./type_defs.md#getmatchidoutputtypedef) 


```python
# get_match_id method usage example with argument unpacking

kwargs: GetMatchIdInputTypeDef = {  # (1)
    "record": ...,
    "workflowName": ...,
}

parent.get_match_id(**kwargs)
```

1. See [:material-code-braces: GetMatchIdInputTypeDef](./type_defs.md#getmatchidinputtypedef) 

### get\_matching\_job

Gets the status, metrics, and errors (if there are any) that are associated
with a job.

Type annotations and code completion for `#!python session.create_client("entityresolution").get_matching_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/get_matching_job.html)

```python
# get_matching_job method definition

await def get_matching_job(
    self,
    *,
    jobId: str,
    workflowName: str,
) -> GetMatchingJobOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMatchingJobOutputTypeDef](./type_defs.md#getmatchingjoboutputtypedef) 


```python
# get_matching_job method usage example with argument unpacking

kwargs: GetMatchingJobInputTypeDef = {  # (1)
    "jobId": ...,
    "workflowName": ...,
}

parent.get_matching_job(**kwargs)
```

1. See [:material-code-braces: GetMatchingJobInputTypeDef](./type_defs.md#getmatchingjobinputtypedef) 

### get\_matching\_workflow

Returns the <code>MatchingWorkflow</code> with a given name, if it exists.

Type annotations and code completion for `#!python session.create_client("entityresolution").get_matching_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/get_matching_workflow.html)

```python
# get_matching_workflow method definition

await def get_matching_workflow(
    self,
    *,
    workflowName: str,
) -> GetMatchingWorkflowOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMatchingWorkflowOutputTypeDef](./type_defs.md#getmatchingworkflowoutputtypedef) 


```python
# get_matching_workflow method usage example with argument unpacking

kwargs: GetMatchingWorkflowInputTypeDef = {  # (1)
    "workflowName": ...,
}

parent.get_matching_workflow(**kwargs)
```

1. See [:material-code-braces: GetMatchingWorkflowInputTypeDef](./type_defs.md#getmatchingworkflowinputtypedef) 

### get\_policy

Returns the resource-based policy.

Type annotations and code completion for `#!python session.create_client("entityresolution").get_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/get_policy.html)

```python
# get_policy method definition

await def get_policy(
    self,
    *,
    arn: str,
) -> GetPolicyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyOutputTypeDef](./type_defs.md#getpolicyoutputtypedef) 


```python
# get_policy method usage example with argument unpacking

kwargs: GetPolicyInputTypeDef = {  # (1)
    "arn": ...,
}

parent.get_policy(**kwargs)
```

1. See [:material-code-braces: GetPolicyInputTypeDef](./type_defs.md#getpolicyinputtypedef) 

### get\_provider\_service

Returns the <code>ProviderService</code> of a given name.

Type annotations and code completion for `#!python session.create_client("entityresolution").get_provider_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/get_provider_service.html)

```python
# get_provider_service method definition

await def get_provider_service(
    self,
    *,
    providerName: str,
    providerServiceName: str,
) -> GetProviderServiceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProviderServiceOutputTypeDef](./type_defs.md#getproviderserviceoutputtypedef) 


```python
# get_provider_service method usage example with argument unpacking

kwargs: GetProviderServiceInputTypeDef = {  # (1)
    "providerName": ...,
    "providerServiceName": ...,
}

parent.get_provider_service(**kwargs)
```

1. See [:material-code-braces: GetProviderServiceInputTypeDef](./type_defs.md#getproviderserviceinputtypedef) 

### get\_schema\_mapping

Returns the SchemaMapping of a given name.

Type annotations and code completion for `#!python session.create_client("entityresolution").get_schema_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/get_schema_mapping.html)

```python
# get_schema_mapping method definition

await def get_schema_mapping(
    self,
    *,
    schemaName: str,
) -> GetSchemaMappingOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSchemaMappingOutputTypeDef](./type_defs.md#getschemamappingoutputtypedef) 


```python
# get_schema_mapping method usage example with argument unpacking

kwargs: GetSchemaMappingInputTypeDef = {  # (1)
    "schemaName": ...,
}

parent.get_schema_mapping(**kwargs)
```

1. See [:material-code-braces: GetSchemaMappingInputTypeDef](./type_defs.md#getschemamappinginputtypedef) 

### list\_id\_mapping\_jobs

Lists all ID mapping jobs for a given workflow.

Type annotations and code completion for `#!python session.create_client("entityresolution").list_id_mapping_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/list_id_mapping_jobs.html)

```python
# list_id_mapping_jobs method definition

await def list_id_mapping_jobs(
    self,
    *,
    workflowName: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListIdMappingJobsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdMappingJobsOutputTypeDef](./type_defs.md#listidmappingjobsoutputtypedef) 


```python
# list_id_mapping_jobs method usage example with argument unpacking

kwargs: ListIdMappingJobsInputTypeDef = {  # (1)
    "workflowName": ...,
}

parent.list_id_mapping_jobs(**kwargs)
```

1. See [:material-code-braces: ListIdMappingJobsInputTypeDef](./type_defs.md#listidmappingjobsinputtypedef) 

### list\_id\_mapping\_workflows

Returns a list of all the <code>IdMappingWorkflows</code> that have been
created for an Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("entityresolution").list_id_mapping_workflows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/list_id_mapping_workflows.html)

```python
# list_id_mapping_workflows method definition

await def list_id_mapping_workflows(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListIdMappingWorkflowsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdMappingWorkflowsOutputTypeDef](./type_defs.md#listidmappingworkflowsoutputtypedef) 


```python
# list_id_mapping_workflows method usage example with argument unpacking

kwargs: ListIdMappingWorkflowsInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_id_mapping_workflows(**kwargs)
```

1. See [:material-code-braces: ListIdMappingWorkflowsInputTypeDef](./type_defs.md#listidmappingworkflowsinputtypedef) 

### list\_id\_namespaces

Returns a list of all ID namespaces.

Type annotations and code completion for `#!python session.create_client("entityresolution").list_id_namespaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/list_id_namespaces.html)

```python
# list_id_namespaces method definition

await def list_id_namespaces(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListIdNamespacesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdNamespacesOutputTypeDef](./type_defs.md#listidnamespacesoutputtypedef) 


```python
# list_id_namespaces method usage example with argument unpacking

kwargs: ListIdNamespacesInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_id_namespaces(**kwargs)
```

1. See [:material-code-braces: ListIdNamespacesInputTypeDef](./type_defs.md#listidnamespacesinputtypedef) 

### list\_matching\_jobs

Lists all jobs for a given workflow.

Type annotations and code completion for `#!python session.create_client("entityresolution").list_matching_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/list_matching_jobs.html)

```python
# list_matching_jobs method definition

await def list_matching_jobs(
    self,
    *,
    workflowName: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMatchingJobsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMatchingJobsOutputTypeDef](./type_defs.md#listmatchingjobsoutputtypedef) 


```python
# list_matching_jobs method usage example with argument unpacking

kwargs: ListMatchingJobsInputTypeDef = {  # (1)
    "workflowName": ...,
}

parent.list_matching_jobs(**kwargs)
```

1. See [:material-code-braces: ListMatchingJobsInputTypeDef](./type_defs.md#listmatchingjobsinputtypedef) 

### list\_matching\_workflows

Returns a list of all the <code>MatchingWorkflows</code> that have been created
for an Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("entityresolution").list_matching_workflows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/list_matching_workflows.html)

```python
# list_matching_workflows method definition

await def list_matching_workflows(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMatchingWorkflowsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMatchingWorkflowsOutputTypeDef](./type_defs.md#listmatchingworkflowsoutputtypedef) 


```python
# list_matching_workflows method usage example with argument unpacking

kwargs: ListMatchingWorkflowsInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_matching_workflows(**kwargs)
```

1. See [:material-code-braces: ListMatchingWorkflowsInputTypeDef](./type_defs.md#listmatchingworkflowsinputtypedef) 

### list\_provider\_services

Returns a list of all the <code>ProviderServices</code> that are available in
this Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("entityresolution").list_provider_services` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/list_provider_services.html)

```python
# list_provider_services method definition

await def list_provider_services(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    providerName: str = ...,
) -> ListProviderServicesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProviderServicesOutputTypeDef](./type_defs.md#listproviderservicesoutputtypedef) 


```python
# list_provider_services method usage example with argument unpacking

kwargs: ListProviderServicesInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_provider_services(**kwargs)
```

1. See [:material-code-braces: ListProviderServicesInputTypeDef](./type_defs.md#listproviderservicesinputtypedef) 

### list\_schema\_mappings

Returns a list of all the <code>SchemaMappings</code> that have been created
for an Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("entityresolution").list_schema_mappings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/list_schema_mappings.html)

```python
# list_schema_mappings method definition

await def list_schema_mappings(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSchemaMappingsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSchemaMappingsOutputTypeDef](./type_defs.md#listschemamappingsoutputtypedef) 


```python
# list_schema_mappings method usage example with argument unpacking

kwargs: ListSchemaMappingsInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_schema_mappings(**kwargs)
```

1. See [:material-code-braces: ListSchemaMappingsInputTypeDef](./type_defs.md#listschemamappingsinputtypedef) 

### list\_tags\_for\_resource

Displays the tags associated with an Entity Resolution resource.

Type annotations and code completion for `#!python session.create_client("entityresolution").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/list_tags_for_resource.html)

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

### put\_policy

Updates the resource-based policy.

Type annotations and code completion for `#!python session.create_client("entityresolution").put_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/put_policy.html)

```python
# put_policy method definition

await def put_policy(
    self,
    *,
    arn: str,
    policy: str,
    token: str = ...,
) -> PutPolicyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutPolicyOutputTypeDef](./type_defs.md#putpolicyoutputtypedef) 


```python
# put_policy method usage example with argument unpacking

kwargs: PutPolicyInputTypeDef = {  # (1)
    "arn": ...,
    "policy": ...,
}

parent.put_policy(**kwargs)
```

1. See [:material-code-braces: PutPolicyInputTypeDef](./type_defs.md#putpolicyinputtypedef) 

### start\_id\_mapping\_job

Starts the <code>IdMappingJob</code> of a workflow.

Type annotations and code completion for `#!python session.create_client("entityresolution").start_id_mapping_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/start_id_mapping_job.html)

```python
# start_id_mapping_job method definition

await def start_id_mapping_job(
    self,
    *,
    workflowName: str,
    outputSourceConfig: Sequence[IdMappingJobOutputSourceTypeDef] = ...,  # (1)
) -> StartIdMappingJobOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IdMappingJobOutputSourceTypeDef](./type_defs.md#idmappingjoboutputsourcetypedef) 
2. See [:material-code-braces: StartIdMappingJobOutputTypeDef](./type_defs.md#startidmappingjoboutputtypedef) 


```python
# start_id_mapping_job method usage example with argument unpacking

kwargs: StartIdMappingJobInputTypeDef = {  # (1)
    "workflowName": ...,
}

parent.start_id_mapping_job(**kwargs)
```

1. See [:material-code-braces: StartIdMappingJobInputTypeDef](./type_defs.md#startidmappingjobinputtypedef) 

### start\_matching\_job

Starts the <code>MatchingJob</code> of a workflow.

Type annotations and code completion for `#!python session.create_client("entityresolution").start_matching_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/start_matching_job.html)

```python
# start_matching_job method definition

await def start_matching_job(
    self,
    *,
    workflowName: str,
) -> StartMatchingJobOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMatchingJobOutputTypeDef](./type_defs.md#startmatchingjoboutputtypedef) 


```python
# start_matching_job method usage example with argument unpacking

kwargs: StartMatchingJobInputTypeDef = {  # (1)
    "workflowName": ...,
}

parent.start_matching_job(**kwargs)
```

1. See [:material-code-braces: StartMatchingJobInputTypeDef](./type_defs.md#startmatchingjobinputtypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified Entity Resolution
resource.

Type annotations and code completion for `#!python session.create_client("entityresolution").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/tag_resource.html)

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

Removes one or more tags from the specified Entity Resolution resource.

Type annotations and code completion for `#!python session.create_client("entityresolution").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/untag_resource.html)

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

### update\_id\_mapping\_workflow

Updates an existing <code>IdMappingWorkflow</code>.

Type annotations and code completion for `#!python session.create_client("entityresolution").update_id_mapping_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/update_id_mapping_workflow.html)

```python
# update_id_mapping_workflow method definition

await def update_id_mapping_workflow(
    self,
    *,
    idMappingTechniques: IdMappingTechniquesUnionTypeDef,  # (1)
    inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],  # (2)
    workflowName: str,
    description: str = ...,
    outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef] = ...,  # (3)
    roleArn: str = ...,
) -> UpdateIdMappingWorkflowOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) [:material-code-braces: IdMappingTechniquesOutputTypeDef](./type_defs.md#idmappingtechniquesoutputtypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
4. See [:material-code-braces: UpdateIdMappingWorkflowOutputTypeDef](./type_defs.md#updateidmappingworkflowoutputtypedef) 


```python
# update_id_mapping_workflow method usage example with argument unpacking

kwargs: UpdateIdMappingWorkflowInputTypeDef = {  # (1)
    "idMappingTechniques": ...,
    "inputSourceConfig": ...,
    "workflowName": ...,
}

parent.update_id_mapping_workflow(**kwargs)
```

1. See [:material-code-braces: UpdateIdMappingWorkflowInputTypeDef](./type_defs.md#updateidmappingworkflowinputtypedef) 

### update\_id\_namespace

Updates an existing ID namespace.

Type annotations and code completion for `#!python session.create_client("entityresolution").update_id_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/update_id_namespace.html)

```python
# update_id_namespace method definition

await def update_id_namespace(
    self,
    *,
    idNamespaceName: str,
    description: str = ...,
    idMappingWorkflowProperties: Sequence[IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef] = ...,  # (1)
    inputSourceConfig: Sequence[IdNamespaceInputSourceTypeDef] = ...,  # (2)
    roleArn: str = ...,
) -> UpdateIdNamespaceOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiestypedef) [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiesoutputtypedef) 
2. See [:material-code-braces: IdNamespaceInputSourceTypeDef](./type_defs.md#idnamespaceinputsourcetypedef) 
3. See [:material-code-braces: UpdateIdNamespaceOutputTypeDef](./type_defs.md#updateidnamespaceoutputtypedef) 


```python
# update_id_namespace method usage example with argument unpacking

kwargs: UpdateIdNamespaceInputTypeDef = {  # (1)
    "idNamespaceName": ...,
}

parent.update_id_namespace(**kwargs)
```

1. See [:material-code-braces: UpdateIdNamespaceInputTypeDef](./type_defs.md#updateidnamespaceinputtypedef) 

### update\_matching\_workflow

Updates an existing <code>MatchingWorkflow</code>.

Type annotations and code completion for `#!python session.create_client("entityresolution").update_matching_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/update_matching_workflow.html)

```python
# update_matching_workflow method definition

await def update_matching_workflow(
    self,
    *,
    inputSourceConfig: Sequence[InputSourceTypeDef],  # (1)
    outputSourceConfig: Sequence[OutputSourceUnionTypeDef],  # (2)
    resolutionTechniques: ResolutionTechniquesUnionTypeDef,  # (3)
    roleArn: str,
    workflowName: str,
    description: str = ...,
    incrementalRunConfig: IncrementalRunConfigTypeDef = ...,  # (4)
) -> UpdateMatchingWorkflowOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
2. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) [:material-code-braces: OutputSourceOutputTypeDef](./type_defs.md#outputsourceoutputtypedef) 
3. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) [:material-code-braces: ResolutionTechniquesOutputTypeDef](./type_defs.md#resolutiontechniquesoutputtypedef) 
4. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
5. See [:material-code-braces: UpdateMatchingWorkflowOutputTypeDef](./type_defs.md#updatematchingworkflowoutputtypedef) 


```python
# update_matching_workflow method usage example with argument unpacking

kwargs: UpdateMatchingWorkflowInputTypeDef = {  # (1)
    "inputSourceConfig": ...,
    "outputSourceConfig": ...,
    "resolutionTechniques": ...,
    "roleArn": ...,
    "workflowName": ...,
}

parent.update_matching_workflow(**kwargs)
```

1. See [:material-code-braces: UpdateMatchingWorkflowInputTypeDef](./type_defs.md#updatematchingworkflowinputtypedef) 

### update\_schema\_mapping

Updates a schema mapping.

Type annotations and code completion for `#!python session.create_client("entityresolution").update_schema_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/client/update_schema_mapping.html)

```python
# update_schema_mapping method definition

await def update_schema_mapping(
    self,
    *,
    mappedInputFields: Sequence[SchemaInputAttributeTypeDef],  # (1)
    schemaName: str,
    description: str = ...,
) -> UpdateSchemaMappingOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
2. See [:material-code-braces: UpdateSchemaMappingOutputTypeDef](./type_defs.md#updateschemamappingoutputtypedef) 


```python
# update_schema_mapping method usage example with argument unpacking

kwargs: UpdateSchemaMappingInputTypeDef = {  # (1)
    "mappedInputFields": ...,
    "schemaName": ...,
}

parent.update_schema_mapping(**kwargs)
```

1. See [:material-code-braces: UpdateSchemaMappingInputTypeDef](./type_defs.md#updateschemamappinginputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("entityresolution").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("entityresolution").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client)

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

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator` method with overloads.

- `client.get_paginator("list_id_mapping_jobs")` -> [ListIdMappingJobsPaginator](./paginators.md#listidmappingjobspaginator)
- `client.get_paginator("list_id_mapping_workflows")` -> [ListIdMappingWorkflowsPaginator](./paginators.md#listidmappingworkflowspaginator)
- `client.get_paginator("list_id_namespaces")` -> [ListIdNamespacesPaginator](./paginators.md#listidnamespacespaginator)
- `client.get_paginator("list_matching_jobs")` -> [ListMatchingJobsPaginator](./paginators.md#listmatchingjobspaginator)
- `client.get_paginator("list_matching_workflows")` -> [ListMatchingWorkflowsPaginator](./paginators.md#listmatchingworkflowspaginator)
- `client.get_paginator("list_provider_services")` -> [ListProviderServicesPaginator](./paginators.md#listproviderservicespaginator)
- `client.get_paginator("list_schema_mappings")` -> [ListSchemaMappingsPaginator](./paginators.md#listschemamappingspaginator)



