# ResilienceHubClient

> [Index](../README.md) > [ResilienceHub](./README.md) > ResilienceHubClient

!!! note ""

    Auto-generated documentation for [ResilienceHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
    type annotations stubs module [types-aiobotocore-resiliencehub](https://pypi.org/project/types-aiobotocore-resiliencehub/).

## ResilienceHubClient

Type annotations and code completion for `#!python session.create_client("resiliencehub")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client)

```python
# ResilienceHubClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_resiliencehub.client import ResilienceHubClient

session = get_session()
async with session.create_client("resiliencehub") as client:
    client: ResilienceHubClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("resiliencehub").exceptions` structure.

```python
# ResilienceHubClient.exceptions usage example

async with session.create_client("resiliencehub") as client:
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
# ResilienceHubClient usage type checking example

from types_aiobotocore_resiliencehub.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### accept\_resource\_grouping\_recommendations

Accepts the resource grouping recommendations suggested by Resilience Hub for
your
application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").accept_resource_grouping_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.accept_resource_grouping_recommendations)

```python
# accept_resource_grouping_recommendations method definition

await def accept_resource_grouping_recommendations(
    self,
    *,
    appArn: str,
    entries: Sequence[AcceptGroupingRecommendationEntryTypeDef],  # (1)
) -> AcceptResourceGroupingRecommendationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AcceptGroupingRecommendationEntryTypeDef](./type_defs.md#acceptgroupingrecommendationentrytypedef) 
2. See [:material-code-braces: AcceptResourceGroupingRecommendationsResponseTypeDef](./type_defs.md#acceptresourcegroupingrecommendationsresponsetypedef) 


```python
# accept_resource_grouping_recommendations method usage example with argument unpacking

kwargs: AcceptResourceGroupingRecommendationsRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "entries": ...,
}

parent.accept_resource_grouping_recommendations(**kwargs)
```

1. See [:material-code-braces: AcceptResourceGroupingRecommendationsRequestRequestTypeDef](./type_defs.md#acceptresourcegroupingrecommendationsrequestrequesttypedef) 

### add\_draft\_app\_version\_resource\_mappings

Adds the source of resource-maps to the draft version of an application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").add_draft_app_version_resource_mappings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.add_draft_app_version_resource_mappings)

```python
# add_draft_app_version_resource_mappings method definition

await def add_draft_app_version_resource_mappings(
    self,
    *,
    appArn: str,
    resourceMappings: Sequence[ResourceMappingTypeDef],  # (1)
) -> AddDraftAppVersionResourceMappingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceMappingTypeDef](./type_defs.md#resourcemappingtypedef) 
2. See [:material-code-braces: AddDraftAppVersionResourceMappingsResponseTypeDef](./type_defs.md#adddraftappversionresourcemappingsresponsetypedef) 


```python
# add_draft_app_version_resource_mappings method usage example with argument unpacking

kwargs: AddDraftAppVersionResourceMappingsRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "resourceMappings": ...,
}

parent.add_draft_app_version_resource_mappings(**kwargs)
```

1. See [:material-code-braces: AddDraftAppVersionResourceMappingsRequestRequestTypeDef](./type_defs.md#adddraftappversionresourcemappingsrequestrequesttypedef) 

### batch\_update\_recommendation\_status

Enables you to include or exclude one or more operational recommendations.

Type annotations and code completion for `#!python session.create_client("resiliencehub").batch_update_recommendation_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.batch_update_recommendation_status)

```python
# batch_update_recommendation_status method definition

await def batch_update_recommendation_status(
    self,
    *,
    appArn: str,
    requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef],  # (1)
) -> BatchUpdateRecommendationStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateRecommendationStatusRequestEntryTypeDef](./type_defs.md#updaterecommendationstatusrequestentrytypedef) 
2. See [:material-code-braces: BatchUpdateRecommendationStatusResponseTypeDef](./type_defs.md#batchupdaterecommendationstatusresponsetypedef) 


```python
# batch_update_recommendation_status method usage example with argument unpacking

kwargs: BatchUpdateRecommendationStatusRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "requestEntries": ...,
}

parent.batch_update_recommendation_status(**kwargs)
```

1. See [:material-code-braces: BatchUpdateRecommendationStatusRequestRequestTypeDef](./type_defs.md#batchupdaterecommendationstatusrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("resiliencehub").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("resiliencehub").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_app

Creates an Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").create_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app)

```python
# create_app method definition

await def create_app(
    self,
    *,
    name: str,
    assessmentSchedule: AppAssessmentScheduleTypeType = ...,  # (1)
    awsApplicationArn: str = ...,
    clientToken: str = ...,
    description: str = ...,
    eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,  # (2)
    permissionModel: PermissionModelTypeDef = ...,  # (3)
    policyArn: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateAppResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AppAssessmentScheduleTypeType](./literals.md#appassessmentscheduletypetype) 
2. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
3. See [:material-code-braces: PermissionModelTypeDef](./type_defs.md#permissionmodeltypedef) 
4. See [:material-code-braces: CreateAppResponseTypeDef](./type_defs.md#createappresponsetypedef) 


```python
# create_app method usage example with argument unpacking

kwargs: CreateAppRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_app(**kwargs)
```

1. See [:material-code-braces: CreateAppRequestRequestTypeDef](./type_defs.md#createapprequestrequesttypedef) 

### create\_app\_version\_app\_component

Creates a new Application Component in the Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").create_app_version_app_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_app_component)

```python
# create_app_version_app_component method definition

await def create_app_version_app_component(
    self,
    *,
    appArn: str,
    name: str,
    type: str,
    additionalInfo: Mapping[str, Sequence[str]] = ...,
    clientToken: str = ...,
    id: str = ...,
) -> CreateAppVersionAppComponentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAppVersionAppComponentResponseTypeDef](./type_defs.md#createappversionappcomponentresponsetypedef) 


```python
# create_app_version_app_component method usage example with argument unpacking

kwargs: CreateAppVersionAppComponentRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "name": ...,
    "type": ...,
}

parent.create_app_version_app_component(**kwargs)
```

1. See [:material-code-braces: CreateAppVersionAppComponentRequestRequestTypeDef](./type_defs.md#createappversionappcomponentrequestrequesttypedef) 

### create\_app\_version\_resource

Adds a resource to the Resilience Hub application and assigns it to the
specified Application
Components.

Type annotations and code completion for `#!python session.create_client("resiliencehub").create_app_version_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_resource)

```python
# create_app_version_resource method definition

await def create_app_version_resource(
    self,
    *,
    appArn: str,
    appComponents: Sequence[str],
    logicalResourceId: LogicalResourceIdTypeDef,  # (1)
    physicalResourceId: str,
    resourceType: str,
    additionalInfo: Mapping[str, Sequence[str]] = ...,
    awsAccountId: str = ...,
    awsRegion: str = ...,
    clientToken: str = ...,
    resourceName: str = ...,
) -> CreateAppVersionResourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LogicalResourceIdTypeDef](./type_defs.md#logicalresourceidtypedef) 
2. See [:material-code-braces: CreateAppVersionResourceResponseTypeDef](./type_defs.md#createappversionresourceresponsetypedef) 


```python
# create_app_version_resource method usage example with argument unpacking

kwargs: CreateAppVersionResourceRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appComponents": ...,
    "logicalResourceId": ...,
    "physicalResourceId": ...,
    "resourceType": ...,
}

parent.create_app_version_resource(**kwargs)
```

1. See [:material-code-braces: CreateAppVersionResourceRequestRequestTypeDef](./type_defs.md#createappversionresourcerequestrequesttypedef) 

### create\_recommendation\_template

Creates a new recommendation template for the Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").create_recommendation_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_recommendation_template)

```python
# create_recommendation_template method definition

await def create_recommendation_template(
    self,
    *,
    assessmentArn: str,
    name: str,
    bucketName: str = ...,
    clientToken: str = ...,
    format: TemplateFormatType = ...,  # (1)
    recommendationIds: Sequence[str] = ...,
    recommendationTypes: Sequence[RenderRecommendationTypeType] = ...,  # (2)
    tags: Mapping[str, str] = ...,
) -> CreateRecommendationTemplateResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TemplateFormatType](./literals.md#templateformattype) 
2. See [:material-code-brackets: RenderRecommendationTypeType](./literals.md#renderrecommendationtypetype) 
3. See [:material-code-braces: CreateRecommendationTemplateResponseTypeDef](./type_defs.md#createrecommendationtemplateresponsetypedef) 


```python
# create_recommendation_template method usage example with argument unpacking

kwargs: CreateRecommendationTemplateRequestRequestTypeDef = {  # (1)
    "assessmentArn": ...,
    "name": ...,
}

parent.create_recommendation_template(**kwargs)
```

1. See [:material-code-braces: CreateRecommendationTemplateRequestRequestTypeDef](./type_defs.md#createrecommendationtemplaterequestrequesttypedef) 

### create\_resiliency\_policy

Creates a resiliency policy for an application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").create_resiliency_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_resiliency_policy)

```python
# create_resiliency_policy method definition

await def create_resiliency_policy(
    self,
    *,
    policy: Mapping[DisruptionTypeType, FailurePolicyTypeDef],  # (1)
    policyName: str,
    tier: ResiliencyPolicyTierType,  # (2)
    clientToken: str = ...,
    dataLocationConstraint: DataLocationConstraintType = ...,  # (3)
    policyDescription: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateResiliencyPolicyResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: DisruptionTypeType](./literals.md#disruptiontypetype) [:material-code-braces: FailurePolicyTypeDef](./type_defs.md#failurepolicytypedef) 
2. See [:material-code-brackets: ResiliencyPolicyTierType](./literals.md#resiliencypolicytiertype) 
3. See [:material-code-brackets: DataLocationConstraintType](./literals.md#datalocationconstrainttype) 
4. See [:material-code-braces: CreateResiliencyPolicyResponseTypeDef](./type_defs.md#createresiliencypolicyresponsetypedef) 


```python
# create_resiliency_policy method usage example with argument unpacking

kwargs: CreateResiliencyPolicyRequestRequestTypeDef = {  # (1)
    "policy": ...,
    "policyName": ...,
    "tier": ...,
}

parent.create_resiliency_policy(**kwargs)
```

1. See [:material-code-braces: CreateResiliencyPolicyRequestRequestTypeDef](./type_defs.md#createresiliencypolicyrequestrequesttypedef) 

### delete\_app

Deletes an Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").delete_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app)

```python
# delete_app method definition

await def delete_app(
    self,
    *,
    appArn: str,
    clientToken: str = ...,
    forceDelete: bool = ...,
) -> DeleteAppResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAppResponseTypeDef](./type_defs.md#deleteappresponsetypedef) 


```python
# delete_app method usage example with argument unpacking

kwargs: DeleteAppRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.delete_app(**kwargs)
```

1. See [:material-code-braces: DeleteAppRequestRequestTypeDef](./type_defs.md#deleteapprequestrequesttypedef) 

### delete\_app\_assessment

Deletes an Resilience Hub application assessment.

Type annotations and code completion for `#!python session.create_client("resiliencehub").delete_app_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_assessment)

```python
# delete_app_assessment method definition

await def delete_app_assessment(
    self,
    *,
    assessmentArn: str,
    clientToken: str = ...,
) -> DeleteAppAssessmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAppAssessmentResponseTypeDef](./type_defs.md#deleteappassessmentresponsetypedef) 


```python
# delete_app_assessment method usage example with argument unpacking

kwargs: DeleteAppAssessmentRequestRequestTypeDef = {  # (1)
    "assessmentArn": ...,
}

parent.delete_app_assessment(**kwargs)
```

1. See [:material-code-braces: DeleteAppAssessmentRequestRequestTypeDef](./type_defs.md#deleteappassessmentrequestrequesttypedef) 

### delete\_app\_input\_source

Deletes the input source and all of its imported resources from the Resilience
Hub
application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").delete_app_input_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_input_source)

```python
# delete_app_input_source method definition

await def delete_app_input_source(
    self,
    *,
    appArn: str,
    clientToken: str = ...,
    eksSourceClusterNamespace: EksSourceClusterNamespaceTypeDef = ...,  # (1)
    sourceArn: str = ...,
    terraformSource: TerraformSourceTypeDef = ...,  # (2)
) -> DeleteAppInputSourceResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EksSourceClusterNamespaceTypeDef](./type_defs.md#ekssourceclusternamespacetypedef) 
2. See [:material-code-braces: TerraformSourceTypeDef](./type_defs.md#terraformsourcetypedef) 
3. See [:material-code-braces: DeleteAppInputSourceResponseTypeDef](./type_defs.md#deleteappinputsourceresponsetypedef) 


```python
# delete_app_input_source method usage example with argument unpacking

kwargs: DeleteAppInputSourceRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.delete_app_input_source(**kwargs)
```

1. See [:material-code-braces: DeleteAppInputSourceRequestRequestTypeDef](./type_defs.md#deleteappinputsourcerequestrequesttypedef) 

### delete\_app\_version\_app\_component

Deletes an Application Component from the Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").delete_app_version_app_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_version_app_component)

```python
# delete_app_version_app_component method definition

await def delete_app_version_app_component(
    self,
    *,
    appArn: str,
    id: str,
    clientToken: str = ...,
) -> DeleteAppVersionAppComponentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAppVersionAppComponentResponseTypeDef](./type_defs.md#deleteappversionappcomponentresponsetypedef) 


```python
# delete_app_version_app_component method usage example with argument unpacking

kwargs: DeleteAppVersionAppComponentRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "id": ...,
}

parent.delete_app_version_app_component(**kwargs)
```

1. See [:material-code-braces: DeleteAppVersionAppComponentRequestRequestTypeDef](./type_defs.md#deleteappversionappcomponentrequestrequesttypedef) 

### delete\_app\_version\_resource

Deletes a resource from the Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").delete_app_version_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_version_resource)

```python
# delete_app_version_resource method definition

await def delete_app_version_resource(
    self,
    *,
    appArn: str,
    awsAccountId: str = ...,
    awsRegion: str = ...,
    clientToken: str = ...,
    logicalResourceId: LogicalResourceIdTypeDef = ...,  # (1)
    physicalResourceId: str = ...,
    resourceName: str = ...,
) -> DeleteAppVersionResourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LogicalResourceIdTypeDef](./type_defs.md#logicalresourceidtypedef) 
2. See [:material-code-braces: DeleteAppVersionResourceResponseTypeDef](./type_defs.md#deleteappversionresourceresponsetypedef) 


```python
# delete_app_version_resource method usage example with argument unpacking

kwargs: DeleteAppVersionResourceRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.delete_app_version_resource(**kwargs)
```

1. See [:material-code-braces: DeleteAppVersionResourceRequestRequestTypeDef](./type_defs.md#deleteappversionresourcerequestrequesttypedef) 

### delete\_recommendation\_template

Deletes a recommendation template.

Type annotations and code completion for `#!python session.create_client("resiliencehub").delete_recommendation_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_recommendation_template)

```python
# delete_recommendation_template method definition

await def delete_recommendation_template(
    self,
    *,
    recommendationTemplateArn: str,
    clientToken: str = ...,
) -> DeleteRecommendationTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteRecommendationTemplateResponseTypeDef](./type_defs.md#deleterecommendationtemplateresponsetypedef) 


```python
# delete_recommendation_template method usage example with argument unpacking

kwargs: DeleteRecommendationTemplateRequestRequestTypeDef = {  # (1)
    "recommendationTemplateArn": ...,
}

parent.delete_recommendation_template(**kwargs)
```

1. See [:material-code-braces: DeleteRecommendationTemplateRequestRequestTypeDef](./type_defs.md#deleterecommendationtemplaterequestrequesttypedef) 

### delete\_resiliency\_policy

Deletes a resiliency policy.

Type annotations and code completion for `#!python session.create_client("resiliencehub").delete_resiliency_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_resiliency_policy)

```python
# delete_resiliency_policy method definition

await def delete_resiliency_policy(
    self,
    *,
    policyArn: str,
    clientToken: str = ...,
) -> DeleteResiliencyPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteResiliencyPolicyResponseTypeDef](./type_defs.md#deleteresiliencypolicyresponsetypedef) 


```python
# delete_resiliency_policy method usage example with argument unpacking

kwargs: DeleteResiliencyPolicyRequestRequestTypeDef = {  # (1)
    "policyArn": ...,
}

parent.delete_resiliency_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResiliencyPolicyRequestRequestTypeDef](./type_defs.md#deleteresiliencypolicyrequestrequesttypedef) 

### describe\_app

Describes an Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").describe_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app)

```python
# describe_app method definition

await def describe_app(
    self,
    *,
    appArn: str,
) -> DescribeAppResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAppResponseTypeDef](./type_defs.md#describeappresponsetypedef) 


```python
# describe_app method usage example with argument unpacking

kwargs: DescribeAppRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.describe_app(**kwargs)
```

1. See [:material-code-braces: DescribeAppRequestRequestTypeDef](./type_defs.md#describeapprequestrequesttypedef) 

### describe\_app\_assessment

Describes an assessment for an Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").describe_app_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_assessment)

```python
# describe_app_assessment method definition

await def describe_app_assessment(
    self,
    *,
    assessmentArn: str,
) -> DescribeAppAssessmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAppAssessmentResponseTypeDef](./type_defs.md#describeappassessmentresponsetypedef) 


```python
# describe_app_assessment method usage example with argument unpacking

kwargs: DescribeAppAssessmentRequestRequestTypeDef = {  # (1)
    "assessmentArn": ...,
}

parent.describe_app_assessment(**kwargs)
```

1. See [:material-code-braces: DescribeAppAssessmentRequestRequestTypeDef](./type_defs.md#describeappassessmentrequestrequesttypedef) 

### describe\_app\_version

Describes the Resilience Hub application version.

Type annotations and code completion for `#!python session.create_client("resiliencehub").describe_app_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version)

```python
# describe_app_version method definition

await def describe_app_version(
    self,
    *,
    appArn: str,
    appVersion: str,
) -> DescribeAppVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAppVersionResponseTypeDef](./type_defs.md#describeappversionresponsetypedef) 


```python
# describe_app_version method usage example with argument unpacking

kwargs: DescribeAppVersionRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appVersion": ...,
}

parent.describe_app_version(**kwargs)
```

1. See [:material-code-braces: DescribeAppVersionRequestRequestTypeDef](./type_defs.md#describeappversionrequestrequesttypedef) 

### describe\_app\_version\_app\_component

Describes an Application Component in the Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").describe_app_version_app_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_app_component)

```python
# describe_app_version_app_component method definition

await def describe_app_version_app_component(
    self,
    *,
    appArn: str,
    appVersion: str,
    id: str,
) -> DescribeAppVersionAppComponentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAppVersionAppComponentResponseTypeDef](./type_defs.md#describeappversionappcomponentresponsetypedef) 


```python
# describe_app_version_app_component method usage example with argument unpacking

kwargs: DescribeAppVersionAppComponentRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appVersion": ...,
    "id": ...,
}

parent.describe_app_version_app_component(**kwargs)
```

1. See [:material-code-braces: DescribeAppVersionAppComponentRequestRequestTypeDef](./type_defs.md#describeappversionappcomponentrequestrequesttypedef) 

### describe\_app\_version\_resource

Describes a resource of the Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").describe_app_version_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_resource)

```python
# describe_app_version_resource method definition

await def describe_app_version_resource(
    self,
    *,
    appArn: str,
    appVersion: str,
    awsAccountId: str = ...,
    awsRegion: str = ...,
    logicalResourceId: LogicalResourceIdTypeDef = ...,  # (1)
    physicalResourceId: str = ...,
    resourceName: str = ...,
) -> DescribeAppVersionResourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LogicalResourceIdTypeDef](./type_defs.md#logicalresourceidtypedef) 
2. See [:material-code-braces: DescribeAppVersionResourceResponseTypeDef](./type_defs.md#describeappversionresourceresponsetypedef) 


```python
# describe_app_version_resource method usage example with argument unpacking

kwargs: DescribeAppVersionResourceRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appVersion": ...,
}

parent.describe_app_version_resource(**kwargs)
```

1. See [:material-code-braces: DescribeAppVersionResourceRequestRequestTypeDef](./type_defs.md#describeappversionresourcerequestrequesttypedef) 

### describe\_app\_version\_resources\_resolution\_status

Returns the resolution status for the specified resolution identifier for an
application
version.

Type annotations and code completion for `#!python session.create_client("resiliencehub").describe_app_version_resources_resolution_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_resources_resolution_status)

```python
# describe_app_version_resources_resolution_status method definition

await def describe_app_version_resources_resolution_status(
    self,
    *,
    appArn: str,
    appVersion: str,
    resolutionId: str = ...,
) -> DescribeAppVersionResourcesResolutionStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAppVersionResourcesResolutionStatusResponseTypeDef](./type_defs.md#describeappversionresourcesresolutionstatusresponsetypedef) 


```python
# describe_app_version_resources_resolution_status method usage example with argument unpacking

kwargs: DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appVersion": ...,
}

parent.describe_app_version_resources_resolution_status(**kwargs)
```

1. See [:material-code-braces: DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef](./type_defs.md#describeappversionresourcesresolutionstatusrequestrequesttypedef) 

### describe\_app\_version\_template

Describes details about an Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").describe_app_version_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_template)

```python
# describe_app_version_template method definition

await def describe_app_version_template(
    self,
    *,
    appArn: str,
    appVersion: str,
) -> DescribeAppVersionTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAppVersionTemplateResponseTypeDef](./type_defs.md#describeappversiontemplateresponsetypedef) 


```python
# describe_app_version_template method usage example with argument unpacking

kwargs: DescribeAppVersionTemplateRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appVersion": ...,
}

parent.describe_app_version_template(**kwargs)
```

1. See [:material-code-braces: DescribeAppVersionTemplateRequestRequestTypeDef](./type_defs.md#describeappversiontemplaterequestrequesttypedef) 

### describe\_draft\_app\_version\_resources\_import\_status

Describes the status of importing resources to an application version.

Type annotations and code completion for `#!python session.create_client("resiliencehub").describe_draft_app_version_resources_import_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_draft_app_version_resources_import_status)

```python
# describe_draft_app_version_resources_import_status method definition

await def describe_draft_app_version_resources_import_status(
    self,
    *,
    appArn: str,
) -> DescribeDraftAppVersionResourcesImportStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDraftAppVersionResourcesImportStatusResponseTypeDef](./type_defs.md#describedraftappversionresourcesimportstatusresponsetypedef) 


```python
# describe_draft_app_version_resources_import_status method usage example with argument unpacking

kwargs: DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.describe_draft_app_version_resources_import_status(**kwargs)
```

1. See [:material-code-braces: DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef](./type_defs.md#describedraftappversionresourcesimportstatusrequestrequesttypedef) 

### describe\_resiliency\_policy

Describes a specified resiliency policy for an Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").describe_resiliency_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_resiliency_policy)

```python
# describe_resiliency_policy method definition

await def describe_resiliency_policy(
    self,
    *,
    policyArn: str,
) -> DescribeResiliencyPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeResiliencyPolicyResponseTypeDef](./type_defs.md#describeresiliencypolicyresponsetypedef) 


```python
# describe_resiliency_policy method usage example with argument unpacking

kwargs: DescribeResiliencyPolicyRequestRequestTypeDef = {  # (1)
    "policyArn": ...,
}

parent.describe_resiliency_policy(**kwargs)
```

1. See [:material-code-braces: DescribeResiliencyPolicyRequestRequestTypeDef](./type_defs.md#describeresiliencypolicyrequestrequesttypedef) 

### describe\_resource\_grouping\_recommendation\_task

Describes the resource grouping recommendation tasks run by Resilience Hub for
your
application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").describe_resource_grouping_recommendation_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_resource_grouping_recommendation_task)

```python
# describe_resource_grouping_recommendation_task method definition

await def describe_resource_grouping_recommendation_task(
    self,
    *,
    appArn: str,
    groupingId: str = ...,
) -> DescribeResourceGroupingRecommendationTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeResourceGroupingRecommendationTaskResponseTypeDef](./type_defs.md#describeresourcegroupingrecommendationtaskresponsetypedef) 


```python
# describe_resource_grouping_recommendation_task method usage example with argument unpacking

kwargs: DescribeResourceGroupingRecommendationTaskRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.describe_resource_grouping_recommendation_task(**kwargs)
```

1. See [:material-code-braces: DescribeResourceGroupingRecommendationTaskRequestRequestTypeDef](./type_defs.md#describeresourcegroupingrecommendationtaskrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("resiliencehub").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.generate_presigned_url)

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


### import\_resources\_to\_draft\_app\_version

Imports resources to Resilience Hub application draft version from different
input
sources.

Type annotations and code completion for `#!python session.create_client("resiliencehub").import_resources_to_draft_app_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.import_resources_to_draft_app_version)

```python
# import_resources_to_draft_app_version method definition

await def import_resources_to_draft_app_version(
    self,
    *,
    appArn: str,
    eksSources: Sequence[EksSourceUnionTypeDef] = ...,  # (1)
    importStrategy: ResourceImportStrategyTypeType = ...,  # (2)
    sourceArns: Sequence[str] = ...,
    terraformSources: Sequence[TerraformSourceTypeDef] = ...,  # (3)
) -> ImportResourcesToDraftAppVersionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: EksSourceTypeDef](./type_defs.md#ekssourcetypedef) [:material-code-braces: EksSourceOutputTypeDef](./type_defs.md#ekssourceoutputtypedef) 
2. See [:material-code-brackets: ResourceImportStrategyTypeType](./literals.md#resourceimportstrategytypetype) 
3. See [:material-code-braces: TerraformSourceTypeDef](./type_defs.md#terraformsourcetypedef) 
4. See [:material-code-braces: ImportResourcesToDraftAppVersionResponseTypeDef](./type_defs.md#importresourcestodraftappversionresponsetypedef) 


```python
# import_resources_to_draft_app_version method usage example with argument unpacking

kwargs: ImportResourcesToDraftAppVersionRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.import_resources_to_draft_app_version(**kwargs)
```

1. See [:material-code-braces: ImportResourcesToDraftAppVersionRequestRequestTypeDef](./type_defs.md#importresourcestodraftappversionrequestrequesttypedef) 

### list\_alarm\_recommendations

Lists the alarm recommendations for an Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_alarm_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_alarm_recommendations)

```python
# list_alarm_recommendations method definition

await def list_alarm_recommendations(
    self,
    *,
    assessmentArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAlarmRecommendationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAlarmRecommendationsResponseTypeDef](./type_defs.md#listalarmrecommendationsresponsetypedef) 


```python
# list_alarm_recommendations method usage example with argument unpacking

kwargs: ListAlarmRecommendationsRequestRequestTypeDef = {  # (1)
    "assessmentArn": ...,
}

parent.list_alarm_recommendations(**kwargs)
```

1. See [:material-code-braces: ListAlarmRecommendationsRequestRequestTypeDef](./type_defs.md#listalarmrecommendationsrequestrequesttypedef) 

### list\_app\_assessment\_compliance\_drifts

Indicates the list of compliance drifts that were detected while running an
assessment.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_app_assessment_compliance_drifts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessment_compliance_drifts)

```python
# list_app_assessment_compliance_drifts method definition

await def list_app_assessment_compliance_drifts(
    self,
    *,
    assessmentArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAppAssessmentComplianceDriftsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppAssessmentComplianceDriftsResponseTypeDef](./type_defs.md#listappassessmentcompliancedriftsresponsetypedef) 


```python
# list_app_assessment_compliance_drifts method usage example with argument unpacking

kwargs: ListAppAssessmentComplianceDriftsRequestRequestTypeDef = {  # (1)
    "assessmentArn": ...,
}

parent.list_app_assessment_compliance_drifts(**kwargs)
```

1. See [:material-code-braces: ListAppAssessmentComplianceDriftsRequestRequestTypeDef](./type_defs.md#listappassessmentcompliancedriftsrequestrequesttypedef) 

### list\_app\_assessment\_resource\_drifts

Indicates the list of resource drifts that were detected while running an
assessment.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_app_assessment_resource_drifts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessment_resource_drifts)

```python
# list_app_assessment_resource_drifts method definition

await def list_app_assessment_resource_drifts(
    self,
    *,
    assessmentArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAppAssessmentResourceDriftsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppAssessmentResourceDriftsResponseTypeDef](./type_defs.md#listappassessmentresourcedriftsresponsetypedef) 


```python
# list_app_assessment_resource_drifts method usage example with argument unpacking

kwargs: ListAppAssessmentResourceDriftsRequestRequestTypeDef = {  # (1)
    "assessmentArn": ...,
}

parent.list_app_assessment_resource_drifts(**kwargs)
```

1. See [:material-code-braces: ListAppAssessmentResourceDriftsRequestRequestTypeDef](./type_defs.md#listappassessmentresourcedriftsrequestrequesttypedef) 

### list\_app\_assessments

Lists the assessments for an Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_app_assessments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessments)

```python
# list_app_assessments method definition

await def list_app_assessments(
    self,
    *,
    appArn: str = ...,
    assessmentName: str = ...,
    assessmentStatus: Sequence[AssessmentStatusType] = ...,  # (1)
    complianceStatus: ComplianceStatusType = ...,  # (2)
    invoker: AssessmentInvokerType = ...,  # (3)
    maxResults: int = ...,
    nextToken: str = ...,
    reverseOrder: bool = ...,
) -> ListAppAssessmentsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AssessmentStatusType](./literals.md#assessmentstatustype) 
2. See [:material-code-brackets: ComplianceStatusType](./literals.md#compliancestatustype) 
3. See [:material-code-brackets: AssessmentInvokerType](./literals.md#assessmentinvokertype) 
4. See [:material-code-braces: ListAppAssessmentsResponseTypeDef](./type_defs.md#listappassessmentsresponsetypedef) 


```python
# list_app_assessments method usage example with argument unpacking

kwargs: ListAppAssessmentsRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.list_app_assessments(**kwargs)
```

1. See [:material-code-braces: ListAppAssessmentsRequestRequestTypeDef](./type_defs.md#listappassessmentsrequestrequesttypedef) 

### list\_app\_component\_compliances

Lists the compliances for an Resilience Hub Application Component.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_app_component_compliances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_component_compliances)

```python
# list_app_component_compliances method definition

await def list_app_component_compliances(
    self,
    *,
    assessmentArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAppComponentCompliancesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppComponentCompliancesResponseTypeDef](./type_defs.md#listappcomponentcompliancesresponsetypedef) 


```python
# list_app_component_compliances method usage example with argument unpacking

kwargs: ListAppComponentCompliancesRequestRequestTypeDef = {  # (1)
    "assessmentArn": ...,
}

parent.list_app_component_compliances(**kwargs)
```

1. See [:material-code-braces: ListAppComponentCompliancesRequestRequestTypeDef](./type_defs.md#listappcomponentcompliancesrequestrequesttypedef) 

### list\_app\_component\_recommendations

Lists the recommendations for an Resilience Hub Application Component.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_app_component_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_component_recommendations)

```python
# list_app_component_recommendations method definition

await def list_app_component_recommendations(
    self,
    *,
    assessmentArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAppComponentRecommendationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppComponentRecommendationsResponseTypeDef](./type_defs.md#listappcomponentrecommendationsresponsetypedef) 


```python
# list_app_component_recommendations method usage example with argument unpacking

kwargs: ListAppComponentRecommendationsRequestRequestTypeDef = {  # (1)
    "assessmentArn": ...,
}

parent.list_app_component_recommendations(**kwargs)
```

1. See [:material-code-braces: ListAppComponentRecommendationsRequestRequestTypeDef](./type_defs.md#listappcomponentrecommendationsrequestrequesttypedef) 

### list\_app\_input\_sources

Lists all the input sources of the Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_app_input_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_input_sources)

```python
# list_app_input_sources method definition

await def list_app_input_sources(
    self,
    *,
    appArn: str,
    appVersion: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAppInputSourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppInputSourcesResponseTypeDef](./type_defs.md#listappinputsourcesresponsetypedef) 


```python
# list_app_input_sources method usage example with argument unpacking

kwargs: ListAppInputSourcesRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appVersion": ...,
}

parent.list_app_input_sources(**kwargs)
```

1. See [:material-code-braces: ListAppInputSourcesRequestRequestTypeDef](./type_defs.md#listappinputsourcesrequestrequesttypedef) 

### list\_app\_version\_app\_components

Lists all the Application Components in the Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_app_version_app_components` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_app_components)

```python
# list_app_version_app_components method definition

await def list_app_version_app_components(
    self,
    *,
    appArn: str,
    appVersion: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAppVersionAppComponentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppVersionAppComponentsResponseTypeDef](./type_defs.md#listappversionappcomponentsresponsetypedef) 


```python
# list_app_version_app_components method usage example with argument unpacking

kwargs: ListAppVersionAppComponentsRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appVersion": ...,
}

parent.list_app_version_app_components(**kwargs)
```

1. See [:material-code-braces: ListAppVersionAppComponentsRequestRequestTypeDef](./type_defs.md#listappversionappcomponentsrequestrequesttypedef) 

### list\_app\_version\_resource\_mappings

Lists how the resources in an application version are mapped/sourced from.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_app_version_resource_mappings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resource_mappings)

```python
# list_app_version_resource_mappings method definition

await def list_app_version_resource_mappings(
    self,
    *,
    appArn: str,
    appVersion: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAppVersionResourceMappingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppVersionResourceMappingsResponseTypeDef](./type_defs.md#listappversionresourcemappingsresponsetypedef) 


```python
# list_app_version_resource_mappings method usage example with argument unpacking

kwargs: ListAppVersionResourceMappingsRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appVersion": ...,
}

parent.list_app_version_resource_mappings(**kwargs)
```

1. See [:material-code-braces: ListAppVersionResourceMappingsRequestRequestTypeDef](./type_defs.md#listappversionresourcemappingsrequestrequesttypedef) 

### list\_app\_version\_resources

Lists all the resources in an Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_app_version_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resources)

```python
# list_app_version_resources method definition

await def list_app_version_resources(
    self,
    *,
    appArn: str,
    appVersion: str,
    maxResults: int = ...,
    nextToken: str = ...,
    resolutionId: str = ...,
) -> ListAppVersionResourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppVersionResourcesResponseTypeDef](./type_defs.md#listappversionresourcesresponsetypedef) 


```python
# list_app_version_resources method usage example with argument unpacking

kwargs: ListAppVersionResourcesRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appVersion": ...,
}

parent.list_app_version_resources(**kwargs)
```

1. See [:material-code-braces: ListAppVersionResourcesRequestRequestTypeDef](./type_defs.md#listappversionresourcesrequestrequesttypedef) 

### list\_app\_versions

Lists the different versions for the Resilience Hub applications.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_app_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_versions)

```python
# list_app_versions method definition

await def list_app_versions(
    self,
    *,
    appArn: str,
    endTime: TimestampTypeDef = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    startTime: TimestampTypeDef = ...,
) -> ListAppVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppVersionsResponseTypeDef](./type_defs.md#listappversionsresponsetypedef) 


```python
# list_app_versions method usage example with argument unpacking

kwargs: ListAppVersionsRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.list_app_versions(**kwargs)
```

1. See [:material-code-braces: ListAppVersionsRequestRequestTypeDef](./type_defs.md#listappversionsrequestrequesttypedef) 

### list\_apps

Lists your Resilience Hub applications.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_apps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_apps)

```python
# list_apps method definition

await def list_apps(
    self,
    *,
    appArn: str = ...,
    awsApplicationArn: str = ...,
    fromLastAssessmentTime: TimestampTypeDef = ...,
    maxResults: int = ...,
    name: str = ...,
    nextToken: str = ...,
    reverseOrder: bool = ...,
    toLastAssessmentTime: TimestampTypeDef = ...,
) -> ListAppsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppsResponseTypeDef](./type_defs.md#listappsresponsetypedef) 


```python
# list_apps method usage example with argument unpacking

kwargs: ListAppsRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.list_apps(**kwargs)
```

1. See [:material-code-braces: ListAppsRequestRequestTypeDef](./type_defs.md#listappsrequestrequesttypedef) 

### list\_recommendation\_templates

Lists the recommendation templates for the Resilience Hub applications.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_recommendation_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_recommendation_templates)

```python
# list_recommendation_templates method definition

await def list_recommendation_templates(
    self,
    *,
    assessmentArn: str = ...,
    maxResults: int = ...,
    name: str = ...,
    nextToken: str = ...,
    recommendationTemplateArn: str = ...,
    reverseOrder: bool = ...,
    status: Sequence[RecommendationTemplateStatusType] = ...,  # (1)
) -> ListRecommendationTemplatesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RecommendationTemplateStatusType](./literals.md#recommendationtemplatestatustype) 
2. See [:material-code-braces: ListRecommendationTemplatesResponseTypeDef](./type_defs.md#listrecommendationtemplatesresponsetypedef) 


```python
# list_recommendation_templates method usage example with argument unpacking

kwargs: ListRecommendationTemplatesRequestRequestTypeDef = {  # (1)
    "assessmentArn": ...,
}

parent.list_recommendation_templates(**kwargs)
```

1. See [:material-code-braces: ListRecommendationTemplatesRequestRequestTypeDef](./type_defs.md#listrecommendationtemplatesrequestrequesttypedef) 

### list\_resiliency\_policies

Lists the resiliency policies for the Resilience Hub applications.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_resiliency_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_resiliency_policies)

```python
# list_resiliency_policies method definition

await def list_resiliency_policies(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    policyName: str = ...,
) -> ListResiliencyPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResiliencyPoliciesResponseTypeDef](./type_defs.md#listresiliencypoliciesresponsetypedef) 


```python
# list_resiliency_policies method usage example with argument unpacking

kwargs: ListResiliencyPoliciesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_resiliency_policies(**kwargs)
```

1. See [:material-code-braces: ListResiliencyPoliciesRequestRequestTypeDef](./type_defs.md#listresiliencypoliciesrequestrequesttypedef) 

### list\_resource\_grouping\_recommendations

Lists the resource grouping recommendations suggested by Resilience Hub for
your
application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_resource_grouping_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_resource_grouping_recommendations)

```python
# list_resource_grouping_recommendations method definition

await def list_resource_grouping_recommendations(
    self,
    *,
    appArn: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListResourceGroupingRecommendationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResourceGroupingRecommendationsResponseTypeDef](./type_defs.md#listresourcegroupingrecommendationsresponsetypedef) 


```python
# list_resource_grouping_recommendations method usage example with argument unpacking

kwargs: ListResourceGroupingRecommendationsRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.list_resource_grouping_recommendations(**kwargs)
```

1. See [:material-code-braces: ListResourceGroupingRecommendationsRequestRequestTypeDef](./type_defs.md#listresourcegroupingrecommendationsrequestrequesttypedef) 

### list\_sop\_recommendations

Lists the standard operating procedure (SOP) recommendations for the Resilience
Hub
applications.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_sop_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_sop_recommendations)

```python
# list_sop_recommendations method definition

await def list_sop_recommendations(
    self,
    *,
    assessmentArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSopRecommendationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSopRecommendationsResponseTypeDef](./type_defs.md#listsoprecommendationsresponsetypedef) 


```python
# list_sop_recommendations method usage example with argument unpacking

kwargs: ListSopRecommendationsRequestRequestTypeDef = {  # (1)
    "assessmentArn": ...,
}

parent.list_sop_recommendations(**kwargs)
```

1. See [:material-code-braces: ListSopRecommendationsRequestRequestTypeDef](./type_defs.md#listsoprecommendationsrequestrequesttypedef) 

### list\_suggested\_resiliency\_policies

Lists the suggested resiliency policies for the Resilience Hub applications.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_suggested_resiliency_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_suggested_resiliency_policies)

```python
# list_suggested_resiliency_policies method definition

await def list_suggested_resiliency_policies(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSuggestedResiliencyPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSuggestedResiliencyPoliciesResponseTypeDef](./type_defs.md#listsuggestedresiliencypoliciesresponsetypedef) 


```python
# list_suggested_resiliency_policies method usage example with argument unpacking

kwargs: ListSuggestedResiliencyPoliciesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_suggested_resiliency_policies(**kwargs)
```

1. See [:material-code-braces: ListSuggestedResiliencyPoliciesRequestRequestTypeDef](./type_defs.md#listsuggestedresiliencypoliciesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for your resources in your Resilience Hub applications.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_test\_recommendations

Lists the test recommendations for the Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_test_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_test_recommendations)

```python
# list_test_recommendations method definition

await def list_test_recommendations(
    self,
    *,
    assessmentArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTestRecommendationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTestRecommendationsResponseTypeDef](./type_defs.md#listtestrecommendationsresponsetypedef) 


```python
# list_test_recommendations method usage example with argument unpacking

kwargs: ListTestRecommendationsRequestRequestTypeDef = {  # (1)
    "assessmentArn": ...,
}

parent.list_test_recommendations(**kwargs)
```

1. See [:material-code-braces: ListTestRecommendationsRequestRequestTypeDef](./type_defs.md#listtestrecommendationsrequestrequesttypedef) 

### list\_unsupported\_app\_version\_resources

Lists the resources that are not currently supported in Resilience Hub.

Type annotations and code completion for `#!python session.create_client("resiliencehub").list_unsupported_app_version_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_unsupported_app_version_resources)

```python
# list_unsupported_app_version_resources method definition

await def list_unsupported_app_version_resources(
    self,
    *,
    appArn: str,
    appVersion: str,
    maxResults: int = ...,
    nextToken: str = ...,
    resolutionId: str = ...,
) -> ListUnsupportedAppVersionResourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUnsupportedAppVersionResourcesResponseTypeDef](./type_defs.md#listunsupportedappversionresourcesresponsetypedef) 


```python
# list_unsupported_app_version_resources method usage example with argument unpacking

kwargs: ListUnsupportedAppVersionResourcesRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appVersion": ...,
}

parent.list_unsupported_app_version_resources(**kwargs)
```

1. See [:material-code-braces: ListUnsupportedAppVersionResourcesRequestRequestTypeDef](./type_defs.md#listunsupportedappversionresourcesrequestrequesttypedef) 

### publish\_app\_version

Publishes a new version of a specific Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").publish_app_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.publish_app_version)

```python
# publish_app_version method definition

await def publish_app_version(
    self,
    *,
    appArn: str,
    versionName: str = ...,
) -> PublishAppVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PublishAppVersionResponseTypeDef](./type_defs.md#publishappversionresponsetypedef) 


```python
# publish_app_version method usage example with argument unpacking

kwargs: PublishAppVersionRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.publish_app_version(**kwargs)
```

1. See [:material-code-braces: PublishAppVersionRequestRequestTypeDef](./type_defs.md#publishappversionrequestrequesttypedef) 

### put\_draft\_app\_version\_template

Adds or updates the app template for an Resilience Hub application draft
version.

Type annotations and code completion for `#!python session.create_client("resiliencehub").put_draft_app_version_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.put_draft_app_version_template)

```python
# put_draft_app_version_template method definition

await def put_draft_app_version_template(
    self,
    *,
    appArn: str,
    appTemplateBody: str,
) -> PutDraftAppVersionTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutDraftAppVersionTemplateResponseTypeDef](./type_defs.md#putdraftappversiontemplateresponsetypedef) 


```python
# put_draft_app_version_template method usage example with argument unpacking

kwargs: PutDraftAppVersionTemplateRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appTemplateBody": ...,
}

parent.put_draft_app_version_template(**kwargs)
```

1. See [:material-code-braces: PutDraftAppVersionTemplateRequestRequestTypeDef](./type_defs.md#putdraftappversiontemplaterequestrequesttypedef) 

### reject\_resource\_grouping\_recommendations

Rejects resource grouping recommendations.

Type annotations and code completion for `#!python session.create_client("resiliencehub").reject_resource_grouping_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.reject_resource_grouping_recommendations)

```python
# reject_resource_grouping_recommendations method definition

await def reject_resource_grouping_recommendations(
    self,
    *,
    appArn: str,
    entries: Sequence[RejectGroupingRecommendationEntryTypeDef],  # (1)
) -> RejectResourceGroupingRecommendationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RejectGroupingRecommendationEntryTypeDef](./type_defs.md#rejectgroupingrecommendationentrytypedef) 
2. See [:material-code-braces: RejectResourceGroupingRecommendationsResponseTypeDef](./type_defs.md#rejectresourcegroupingrecommendationsresponsetypedef) 


```python
# reject_resource_grouping_recommendations method usage example with argument unpacking

kwargs: RejectResourceGroupingRecommendationsRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "entries": ...,
}

parent.reject_resource_grouping_recommendations(**kwargs)
```

1. See [:material-code-braces: RejectResourceGroupingRecommendationsRequestRequestTypeDef](./type_defs.md#rejectresourcegroupingrecommendationsrequestrequesttypedef) 

### remove\_draft\_app\_version\_resource\_mappings

Removes resource mappings from a draft application version.

Type annotations and code completion for `#!python session.create_client("resiliencehub").remove_draft_app_version_resource_mappings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.remove_draft_app_version_resource_mappings)

```python
# remove_draft_app_version_resource_mappings method definition

await def remove_draft_app_version_resource_mappings(
    self,
    *,
    appArn: str,
    appRegistryAppNames: Sequence[str] = ...,
    eksSourceNames: Sequence[str] = ...,
    logicalStackNames: Sequence[str] = ...,
    resourceGroupNames: Sequence[str] = ...,
    resourceNames: Sequence[str] = ...,
    terraformSourceNames: Sequence[str] = ...,
) -> RemoveDraftAppVersionResourceMappingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RemoveDraftAppVersionResourceMappingsResponseTypeDef](./type_defs.md#removedraftappversionresourcemappingsresponsetypedef) 


```python
# remove_draft_app_version_resource_mappings method usage example with argument unpacking

kwargs: RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.remove_draft_app_version_resource_mappings(**kwargs)
```

1. See [:material-code-braces: RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef](./type_defs.md#removedraftappversionresourcemappingsrequestrequesttypedef) 

### resolve\_app\_version\_resources

Resolves the resources for an application version.

Type annotations and code completion for `#!python session.create_client("resiliencehub").resolve_app_version_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.resolve_app_version_resources)

```python
# resolve_app_version_resources method definition

await def resolve_app_version_resources(
    self,
    *,
    appArn: str,
    appVersion: str,
) -> ResolveAppVersionResourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResolveAppVersionResourcesResponseTypeDef](./type_defs.md#resolveappversionresourcesresponsetypedef) 


```python
# resolve_app_version_resources method usage example with argument unpacking

kwargs: ResolveAppVersionResourcesRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appVersion": ...,
}

parent.resolve_app_version_resources(**kwargs)
```

1. See [:material-code-braces: ResolveAppVersionResourcesRequestRequestTypeDef](./type_defs.md#resolveappversionresourcesrequestrequesttypedef) 

### start\_app\_assessment

Creates a new application assessment for an application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").start_app_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.start_app_assessment)

```python
# start_app_assessment method definition

await def start_app_assessment(
    self,
    *,
    appArn: str,
    appVersion: str,
    assessmentName: str,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> StartAppAssessmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartAppAssessmentResponseTypeDef](./type_defs.md#startappassessmentresponsetypedef) 


```python
# start_app_assessment method usage example with argument unpacking

kwargs: StartAppAssessmentRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "appVersion": ...,
    "assessmentName": ...,
}

parent.start_app_assessment(**kwargs)
```

1. See [:material-code-braces: StartAppAssessmentRequestRequestTypeDef](./type_defs.md#startappassessmentrequestrequesttypedef) 

### start\_resource\_grouping\_recommendation\_task

Starts grouping recommendation task.

Type annotations and code completion for `#!python session.create_client("resiliencehub").start_resource_grouping_recommendation_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.start_resource_grouping_recommendation_task)

```python
# start_resource_grouping_recommendation_task method definition

await def start_resource_grouping_recommendation_task(
    self,
    *,
    appArn: str,
) -> StartResourceGroupingRecommendationTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartResourceGroupingRecommendationTaskResponseTypeDef](./type_defs.md#startresourcegroupingrecommendationtaskresponsetypedef) 


```python
# start_resource_grouping_recommendation_task method usage example with argument unpacking

kwargs: StartResourceGroupingRecommendationTaskRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.start_resource_grouping_recommendation_task(**kwargs)
```

1. See [:material-code-braces: StartResourceGroupingRecommendationTaskRequestRequestTypeDef](./type_defs.md#startresourcegroupingrecommendationtaskrequestrequesttypedef) 

### tag\_resource

Applies one or more tags to a resource.

Type annotations and code completion for `#!python session.create_client("resiliencehub").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.tag_resource)

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

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes one or more tags from a resource.

Type annotations and code completion for `#!python session.create_client("resiliencehub").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.untag_resource)

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

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_app

Updates an application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").update_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app)

```python
# update_app method definition

await def update_app(
    self,
    *,
    appArn: str,
    assessmentSchedule: AppAssessmentScheduleTypeType = ...,  # (1)
    clearResiliencyPolicyArn: bool = ...,
    description: str = ...,
    eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,  # (2)
    permissionModel: PermissionModelTypeDef = ...,  # (3)
    policyArn: str = ...,
) -> UpdateAppResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AppAssessmentScheduleTypeType](./literals.md#appassessmentscheduletypetype) 
2. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
3. See [:material-code-braces: PermissionModelTypeDef](./type_defs.md#permissionmodeltypedef) 
4. See [:material-code-braces: UpdateAppResponseTypeDef](./type_defs.md#updateappresponsetypedef) 


```python
# update_app method usage example with argument unpacking

kwargs: UpdateAppRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.update_app(**kwargs)
```

1. See [:material-code-braces: UpdateAppRequestRequestTypeDef](./type_defs.md#updateapprequestrequesttypedef) 

### update\_app\_version

Updates the Resilience Hub application version.

Type annotations and code completion for `#!python session.create_client("resiliencehub").update_app_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version)

```python
# update_app_version method definition

await def update_app_version(
    self,
    *,
    appArn: str,
    additionalInfo: Mapping[str, Sequence[str]] = ...,
) -> UpdateAppVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAppVersionResponseTypeDef](./type_defs.md#updateappversionresponsetypedef) 


```python
# update_app_version method usage example with argument unpacking

kwargs: UpdateAppVersionRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.update_app_version(**kwargs)
```

1. See [:material-code-braces: UpdateAppVersionRequestRequestTypeDef](./type_defs.md#updateappversionrequestrequesttypedef) 

### update\_app\_version\_app\_component

Updates an existing Application Component in the Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").update_app_version_app_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_app_component)

```python
# update_app_version_app_component method definition

await def update_app_version_app_component(
    self,
    *,
    appArn: str,
    id: str,
    additionalInfo: Mapping[str, Sequence[str]] = ...,
    name: str = ...,
    type: str = ...,
) -> UpdateAppVersionAppComponentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAppVersionAppComponentResponseTypeDef](./type_defs.md#updateappversionappcomponentresponsetypedef) 


```python
# update_app_version_app_component method usage example with argument unpacking

kwargs: UpdateAppVersionAppComponentRequestRequestTypeDef = {  # (1)
    "appArn": ...,
    "id": ...,
}

parent.update_app_version_app_component(**kwargs)
```

1. See [:material-code-braces: UpdateAppVersionAppComponentRequestRequestTypeDef](./type_defs.md#updateappversionappcomponentrequestrequesttypedef) 

### update\_app\_version\_resource

Updates the resource details in the Resilience Hub application.

Type annotations and code completion for `#!python session.create_client("resiliencehub").update_app_version_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_resource)

```python
# update_app_version_resource method definition

await def update_app_version_resource(
    self,
    *,
    appArn: str,
    additionalInfo: Mapping[str, Sequence[str]] = ...,
    appComponents: Sequence[str] = ...,
    awsAccountId: str = ...,
    awsRegion: str = ...,
    excluded: bool = ...,
    logicalResourceId: LogicalResourceIdTypeDef = ...,  # (1)
    physicalResourceId: str = ...,
    resourceName: str = ...,
    resourceType: str = ...,
) -> UpdateAppVersionResourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LogicalResourceIdTypeDef](./type_defs.md#logicalresourceidtypedef) 
2. See [:material-code-braces: UpdateAppVersionResourceResponseTypeDef](./type_defs.md#updateappversionresourceresponsetypedef) 


```python
# update_app_version_resource method usage example with argument unpacking

kwargs: UpdateAppVersionResourceRequestRequestTypeDef = {  # (1)
    "appArn": ...,
}

parent.update_app_version_resource(**kwargs)
```

1. See [:material-code-braces: UpdateAppVersionResourceRequestRequestTypeDef](./type_defs.md#updateappversionresourcerequestrequesttypedef) 

### update\_resiliency\_policy

Updates a resiliency policy.

Type annotations and code completion for `#!python session.create_client("resiliencehub").update_resiliency_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_resiliency_policy)

```python
# update_resiliency_policy method definition

await def update_resiliency_policy(
    self,
    *,
    policyArn: str,
    dataLocationConstraint: DataLocationConstraintType = ...,  # (1)
    policy: Mapping[DisruptionTypeType, FailurePolicyTypeDef] = ...,  # (2)
    policyDescription: str = ...,
    policyName: str = ...,
    tier: ResiliencyPolicyTierType = ...,  # (3)
) -> UpdateResiliencyPolicyResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: DataLocationConstraintType](./literals.md#datalocationconstrainttype) 
2. See [:material-code-brackets: DisruptionTypeType](./literals.md#disruptiontypetype) [:material-code-braces: FailurePolicyTypeDef](./type_defs.md#failurepolicytypedef) 
3. See [:material-code-brackets: ResiliencyPolicyTierType](./literals.md#resiliencypolicytiertype) 
4. See [:material-code-braces: UpdateResiliencyPolicyResponseTypeDef](./type_defs.md#updateresiliencypolicyresponsetypedef) 


```python
# update_resiliency_policy method usage example with argument unpacking

kwargs: UpdateResiliencyPolicyRequestRequestTypeDef = {  # (1)
    "policyArn": ...,
}

parent.update_resiliency_policy(**kwargs)
```

1. See [:material-code-braces: UpdateResiliencyPolicyRequestRequestTypeDef](./type_defs.md#updateresiliencypolicyrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("resiliencehub").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "ResilienceHubClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("resiliencehub").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("resiliencehub").get_paginator` method with overloads.

- `client.get_paginator("list_app_assessment_resource_drifts")` -> [ListAppAssessmentResourceDriftsPaginator](./paginators.md#listappassessmentresourcedriftspaginator)
- `client.get_paginator("list_resource_grouping_recommendations")` -> [ListResourceGroupingRecommendationsPaginator](./paginators.md#listresourcegroupingrecommendationspaginator)



