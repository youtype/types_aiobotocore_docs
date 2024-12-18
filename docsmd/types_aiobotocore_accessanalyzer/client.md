# AccessAnalyzerClient

> [Index](../README.md) > [AccessAnalyzer](./README.md) > AccessAnalyzerClient

!!! note ""

    Auto-generated documentation for [AccessAnalyzer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#accessanalyzer)
    type annotations stubs module [types-aiobotocore-accessanalyzer](https://pypi.org/project/types-aiobotocore-accessanalyzer/).

## AccessAnalyzerClient

Type annotations and code completion for `#!python session.create_client("accessanalyzer")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client)

```python
# AccessAnalyzerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_accessanalyzer.client import AccessAnalyzerClient

session = get_session()
async with session.create_client("accessanalyzer") as client:
    client: AccessAnalyzerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("accessanalyzer").exceptions` structure.

```python
# AccessAnalyzerClient.exceptions usage example

async with session.create_client("accessanalyzer") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.InvalidParameterException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.UnprocessableEntityException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# AccessAnalyzerClient usage type checking example

from types_aiobotocore_accessanalyzer.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("accessanalyzer").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("accessanalyzer").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/generate_presigned_url.html)

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


### close



Type annotations and code completion for `#!python session.create_client("accessanalyzer").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### apply\_archive\_rule

Retroactively applies the archive rule to existing findings that meet the
archive rule criteria.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").apply_archive_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/apply_archive_rule.html)

```python
# apply_archive_rule method definition

await def apply_archive_rule(
    self,
    *,
    analyzerArn: str,
    ruleName: str,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# apply_archive_rule method usage example with argument unpacking

kwargs: ApplyArchiveRuleRequestRequestTypeDef = {  # (1)
    "analyzerArn": ...,
    "ruleName": ...,
}

parent.apply_archive_rule(**kwargs)
```

1. See [:material-code-braces: ApplyArchiveRuleRequestRequestTypeDef](./type_defs.md#applyarchiverulerequestrequesttypedef) 

### cancel\_policy\_generation

Cancels the requested policy generation.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").cancel_policy_generation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/cancel_policy_generation.html)

```python
# cancel_policy_generation method definition

await def cancel_policy_generation(
    self,
    *,
    jobId: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_policy_generation method usage example with argument unpacking

kwargs: CancelPolicyGenerationRequestRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.cancel_policy_generation(**kwargs)
```

1. See [:material-code-braces: CancelPolicyGenerationRequestRequestTypeDef](./type_defs.md#cancelpolicygenerationrequestrequesttypedef) 

### check\_access\_not\_granted

Checks whether the specified access isn't allowed by a policy.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").check_access_not_granted` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/check_access_not_granted.html)

```python
# check_access_not_granted method definition

await def check_access_not_granted(
    self,
    *,
    policyDocument: str,
    access: Sequence[AccessTypeDef],  # (1)
    policyType: AccessCheckPolicyTypeType,  # (2)
) -> CheckAccessNotGrantedResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AccessTypeDef](./type_defs.md#accesstypedef) 
2. See [:material-code-brackets: AccessCheckPolicyTypeType](./literals.md#accesscheckpolicytypetype) 
3. See [:material-code-braces: CheckAccessNotGrantedResponseTypeDef](./type_defs.md#checkaccessnotgrantedresponsetypedef) 


```python
# check_access_not_granted method usage example with argument unpacking

kwargs: CheckAccessNotGrantedRequestRequestTypeDef = {  # (1)
    "policyDocument": ...,
    "access": ...,
    "policyType": ...,
}

parent.check_access_not_granted(**kwargs)
```

1. See [:material-code-braces: CheckAccessNotGrantedRequestRequestTypeDef](./type_defs.md#checkaccessnotgrantedrequestrequesttypedef) 

### check\_no\_new\_access

Checks whether new access is allowed for an updated policy when compared to the
existing policy.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").check_no_new_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/check_no_new_access.html)

```python
# check_no_new_access method definition

await def check_no_new_access(
    self,
    *,
    newPolicyDocument: str,
    existingPolicyDocument: str,
    policyType: AccessCheckPolicyTypeType,  # (1)
) -> CheckNoNewAccessResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AccessCheckPolicyTypeType](./literals.md#accesscheckpolicytypetype) 
2. See [:material-code-braces: CheckNoNewAccessResponseTypeDef](./type_defs.md#checknonewaccessresponsetypedef) 


```python
# check_no_new_access method usage example with argument unpacking

kwargs: CheckNoNewAccessRequestRequestTypeDef = {  # (1)
    "newPolicyDocument": ...,
    "existingPolicyDocument": ...,
    "policyType": ...,
}

parent.check_no_new_access(**kwargs)
```

1. See [:material-code-braces: CheckNoNewAccessRequestRequestTypeDef](./type_defs.md#checknonewaccessrequestrequesttypedef) 

### check\_no\_public\_access

Checks whether a resource policy can grant public access to the specified
resource type.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").check_no_public_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/check_no_public_access.html)

```python
# check_no_public_access method definition

await def check_no_public_access(
    self,
    *,
    policyDocument: str,
    resourceType: AccessCheckResourceTypeType,  # (1)
) -> CheckNoPublicAccessResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AccessCheckResourceTypeType](./literals.md#accesscheckresourcetypetype) 
2. See [:material-code-braces: CheckNoPublicAccessResponseTypeDef](./type_defs.md#checknopublicaccessresponsetypedef) 


```python
# check_no_public_access method usage example with argument unpacking

kwargs: CheckNoPublicAccessRequestRequestTypeDef = {  # (1)
    "policyDocument": ...,
    "resourceType": ...,
}

parent.check_no_public_access(**kwargs)
```

1. See [:material-code-braces: CheckNoPublicAccessRequestRequestTypeDef](./type_defs.md#checknopublicaccessrequestrequesttypedef) 

### create\_access\_preview

Creates an access preview that allows you to preview IAM Access Analyzer
findings for your resource before deploying resource permissions.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").create_access_preview` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/create_access_preview.html)

```python
# create_access_preview method definition

await def create_access_preview(
    self,
    *,
    analyzerArn: str,
    configurations: Mapping[str, ConfigurationUnionTypeDef],  # (1)
    clientToken: str = ...,
) -> CreateAccessPreviewResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
2. See [:material-code-braces: CreateAccessPreviewResponseTypeDef](./type_defs.md#createaccesspreviewresponsetypedef) 


```python
# create_access_preview method usage example with argument unpacking

kwargs: CreateAccessPreviewRequestRequestTypeDef = {  # (1)
    "analyzerArn": ...,
    "configurations": ...,
}

parent.create_access_preview(**kwargs)
```

1. See [:material-code-braces: CreateAccessPreviewRequestRequestTypeDef](./type_defs.md#createaccesspreviewrequestrequesttypedef) 

### create\_analyzer

Creates an analyzer for your account.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").create_analyzer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/create_analyzer.html)

```python
# create_analyzer method definition

await def create_analyzer(
    self,
    *,
    analyzerName: str,
    type: TypeType,  # (1)
    archiveRules: Sequence[InlineArchiveRuleTypeDef] = ...,  # (2)
    tags: Mapping[str, str] = ...,
    clientToken: str = ...,
    configuration: AnalyzerConfigurationTypeDef = ...,  # (3)
) -> CreateAnalyzerResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-braces: InlineArchiveRuleTypeDef](./type_defs.md#inlinearchiveruletypedef) 
3. See [:material-code-braces: AnalyzerConfigurationTypeDef](./type_defs.md#analyzerconfigurationtypedef) 
4. See [:material-code-braces: CreateAnalyzerResponseTypeDef](./type_defs.md#createanalyzerresponsetypedef) 


```python
# create_analyzer method usage example with argument unpacking

kwargs: CreateAnalyzerRequestRequestTypeDef = {  # (1)
    "analyzerName": ...,
    "type": ...,
}

parent.create_analyzer(**kwargs)
```

1. See [:material-code-braces: CreateAnalyzerRequestRequestTypeDef](./type_defs.md#createanalyzerrequestrequesttypedef) 

### create\_archive\_rule

Creates an archive rule for the specified analyzer.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").create_archive_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/create_archive_rule.html)

```python
# create_archive_rule method definition

await def create_archive_rule(
    self,
    *,
    analyzerName: str,
    ruleName: str,
    filter: Mapping[str, CriterionUnionTypeDef],  # (1)
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CriterionTypeDef](./type_defs.md#criteriontypedef) [:material-code-braces: CriterionOutputTypeDef](./type_defs.md#criterionoutputtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_archive_rule method usage example with argument unpacking

kwargs: CreateArchiveRuleRequestRequestTypeDef = {  # (1)
    "analyzerName": ...,
    "ruleName": ...,
    "filter": ...,
}

parent.create_archive_rule(**kwargs)
```

1. See [:material-code-braces: CreateArchiveRuleRequestRequestTypeDef](./type_defs.md#createarchiverulerequestrequesttypedef) 

### delete\_analyzer

Deletes the specified analyzer.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").delete_analyzer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/delete_analyzer.html)

```python
# delete_analyzer method definition

await def delete_analyzer(
    self,
    *,
    analyzerName: str,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_analyzer method usage example with argument unpacking

kwargs: DeleteAnalyzerRequestRequestTypeDef = {  # (1)
    "analyzerName": ...,
}

parent.delete_analyzer(**kwargs)
```

1. See [:material-code-braces: DeleteAnalyzerRequestRequestTypeDef](./type_defs.md#deleteanalyzerrequestrequesttypedef) 

### delete\_archive\_rule

Deletes the specified archive rule.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").delete_archive_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/delete_archive_rule.html)

```python
# delete_archive_rule method definition

await def delete_archive_rule(
    self,
    *,
    analyzerName: str,
    ruleName: str,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_archive_rule method usage example with argument unpacking

kwargs: DeleteArchiveRuleRequestRequestTypeDef = {  # (1)
    "analyzerName": ...,
    "ruleName": ...,
}

parent.delete_archive_rule(**kwargs)
```

1. See [:material-code-braces: DeleteArchiveRuleRequestRequestTypeDef](./type_defs.md#deletearchiverulerequestrequesttypedef) 

### generate\_finding\_recommendation

Creates a recommendation for an unused permissions finding.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").generate_finding_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/generate_finding_recommendation.html)

```python
# generate_finding_recommendation method definition

await def generate_finding_recommendation(
    self,
    *,
    analyzerArn: str,
    id: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# generate_finding_recommendation method usage example with argument unpacking

kwargs: GenerateFindingRecommendationRequestRequestTypeDef = {  # (1)
    "analyzerArn": ...,
    "id": ...,
}

parent.generate_finding_recommendation(**kwargs)
```

1. See [:material-code-braces: GenerateFindingRecommendationRequestRequestTypeDef](./type_defs.md#generatefindingrecommendationrequestrequesttypedef) 

### get\_access\_preview

Retrieves information about an access preview for the specified analyzer.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_access_preview` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/get_access_preview.html)

```python
# get_access_preview method definition

await def get_access_preview(
    self,
    *,
    accessPreviewId: str,
    analyzerArn: str,
) -> GetAccessPreviewResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessPreviewResponseTypeDef](./type_defs.md#getaccesspreviewresponsetypedef) 


```python
# get_access_preview method usage example with argument unpacking

kwargs: GetAccessPreviewRequestRequestTypeDef = {  # (1)
    "accessPreviewId": ...,
    "analyzerArn": ...,
}

parent.get_access_preview(**kwargs)
```

1. See [:material-code-braces: GetAccessPreviewRequestRequestTypeDef](./type_defs.md#getaccesspreviewrequestrequesttypedef) 

### get\_analyzed\_resource

Retrieves information about a resource that was analyzed.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_analyzed_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/get_analyzed_resource.html)

```python
# get_analyzed_resource method definition

await def get_analyzed_resource(
    self,
    *,
    analyzerArn: str,
    resourceArn: str,
) -> GetAnalyzedResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAnalyzedResourceResponseTypeDef](./type_defs.md#getanalyzedresourceresponsetypedef) 


```python
# get_analyzed_resource method usage example with argument unpacking

kwargs: GetAnalyzedResourceRequestRequestTypeDef = {  # (1)
    "analyzerArn": ...,
    "resourceArn": ...,
}

parent.get_analyzed_resource(**kwargs)
```

1. See [:material-code-braces: GetAnalyzedResourceRequestRequestTypeDef](./type_defs.md#getanalyzedresourcerequestrequesttypedef) 

### get\_analyzer

Retrieves information about the specified analyzer.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_analyzer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/get_analyzer.html)

```python
# get_analyzer method definition

await def get_analyzer(
    self,
    *,
    analyzerName: str,
) -> GetAnalyzerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAnalyzerResponseTypeDef](./type_defs.md#getanalyzerresponsetypedef) 


```python
# get_analyzer method usage example with argument unpacking

kwargs: GetAnalyzerRequestRequestTypeDef = {  # (1)
    "analyzerName": ...,
}

parent.get_analyzer(**kwargs)
```

1. See [:material-code-braces: GetAnalyzerRequestRequestTypeDef](./type_defs.md#getanalyzerrequestrequesttypedef) 

### get\_archive\_rule

Retrieves information about an archive rule.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_archive_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/get_archive_rule.html)

```python
# get_archive_rule method definition

await def get_archive_rule(
    self,
    *,
    analyzerName: str,
    ruleName: str,
) -> GetArchiveRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetArchiveRuleResponseTypeDef](./type_defs.md#getarchiveruleresponsetypedef) 


```python
# get_archive_rule method usage example with argument unpacking

kwargs: GetArchiveRuleRequestRequestTypeDef = {  # (1)
    "analyzerName": ...,
    "ruleName": ...,
}

parent.get_archive_rule(**kwargs)
```

1. See [:material-code-braces: GetArchiveRuleRequestRequestTypeDef](./type_defs.md#getarchiverulerequestrequesttypedef) 

### get\_finding

Retrieves information about the specified finding.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_finding` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/get_finding.html)

```python
# get_finding method definition

await def get_finding(
    self,
    *,
    analyzerArn: str,
    id: str,
) -> GetFindingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFindingResponseTypeDef](./type_defs.md#getfindingresponsetypedef) 


```python
# get_finding method usage example with argument unpacking

kwargs: GetFindingRequestRequestTypeDef = {  # (1)
    "analyzerArn": ...,
    "id": ...,
}

parent.get_finding(**kwargs)
```

1. See [:material-code-braces: GetFindingRequestRequestTypeDef](./type_defs.md#getfindingrequestrequesttypedef) 

### get\_finding\_recommendation

Retrieves information about a finding recommendation for the specified analyzer.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_finding_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/get_finding_recommendation.html)

```python
# get_finding_recommendation method definition

await def get_finding_recommendation(
    self,
    *,
    analyzerArn: str,
    id: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> GetFindingRecommendationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFindingRecommendationResponseTypeDef](./type_defs.md#getfindingrecommendationresponsetypedef) 


```python
# get_finding_recommendation method usage example with argument unpacking

kwargs: GetFindingRecommendationRequestRequestTypeDef = {  # (1)
    "analyzerArn": ...,
    "id": ...,
}

parent.get_finding_recommendation(**kwargs)
```

1. See [:material-code-braces: GetFindingRecommendationRequestRequestTypeDef](./type_defs.md#getfindingrecommendationrequestrequesttypedef) 

### get\_finding\_v2

Retrieves information about the specified finding.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_finding_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/get_finding_v2.html)

```python
# get_finding_v2 method definition

await def get_finding_v2(
    self,
    *,
    analyzerArn: str,
    id: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> GetFindingV2ResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFindingV2ResponseTypeDef](./type_defs.md#getfindingv2responsetypedef) 


```python
# get_finding_v2 method usage example with argument unpacking

kwargs: GetFindingV2RequestRequestTypeDef = {  # (1)
    "analyzerArn": ...,
    "id": ...,
}

parent.get_finding_v2(**kwargs)
```

1. See [:material-code-braces: GetFindingV2RequestRequestTypeDef](./type_defs.md#getfindingv2requestrequesttypedef) 

### get\_generated\_policy

Retrieves the policy that was generated using
<code>StartPolicyGeneration</code>.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_generated_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/get_generated_policy.html)

```python
# get_generated_policy method definition

await def get_generated_policy(
    self,
    *,
    jobId: str,
    includeResourcePlaceholders: bool = ...,
    includeServiceLevelTemplate: bool = ...,
) -> GetGeneratedPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGeneratedPolicyResponseTypeDef](./type_defs.md#getgeneratedpolicyresponsetypedef) 


```python
# get_generated_policy method usage example with argument unpacking

kwargs: GetGeneratedPolicyRequestRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.get_generated_policy(**kwargs)
```

1. See [:material-code-braces: GetGeneratedPolicyRequestRequestTypeDef](./type_defs.md#getgeneratedpolicyrequestrequesttypedef) 

### list\_access\_preview\_findings

Retrieves a list of access preview findings generated by the specified access
preview.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").list_access_preview_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/list_access_preview_findings.html)

```python
# list_access_preview_findings method definition

await def list_access_preview_findings(
    self,
    *,
    accessPreviewId: str,
    analyzerArn: str,
    filter: Mapping[str, CriterionTypeDef] = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAccessPreviewFindingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CriterionTypeDef](./type_defs.md#criteriontypedef) 
2. See [:material-code-braces: ListAccessPreviewFindingsResponseTypeDef](./type_defs.md#listaccesspreviewfindingsresponsetypedef) 


```python
# list_access_preview_findings method usage example with argument unpacking

kwargs: ListAccessPreviewFindingsRequestRequestTypeDef = {  # (1)
    "accessPreviewId": ...,
    "analyzerArn": ...,
}

parent.list_access_preview_findings(**kwargs)
```

1. See [:material-code-braces: ListAccessPreviewFindingsRequestRequestTypeDef](./type_defs.md#listaccesspreviewfindingsrequestrequesttypedef) 

### list\_access\_previews

Retrieves a list of access previews for the specified analyzer.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").list_access_previews` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/list_access_previews.html)

```python
# list_access_previews method definition

await def list_access_previews(
    self,
    *,
    analyzerArn: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAccessPreviewsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccessPreviewsResponseTypeDef](./type_defs.md#listaccesspreviewsresponsetypedef) 


```python
# list_access_previews method usage example with argument unpacking

kwargs: ListAccessPreviewsRequestRequestTypeDef = {  # (1)
    "analyzerArn": ...,
}

parent.list_access_previews(**kwargs)
```

1. See [:material-code-braces: ListAccessPreviewsRequestRequestTypeDef](./type_defs.md#listaccesspreviewsrequestrequesttypedef) 

### list\_analyzed\_resources

Retrieves a list of resources of the specified type that have been analyzed by
the specified analyzer.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").list_analyzed_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/list_analyzed_resources.html)

```python
# list_analyzed_resources method definition

await def list_analyzed_resources(
    self,
    *,
    analyzerArn: str,
    resourceType: ResourceTypeType = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAnalyzedResourcesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ListAnalyzedResourcesResponseTypeDef](./type_defs.md#listanalyzedresourcesresponsetypedef) 


```python
# list_analyzed_resources method usage example with argument unpacking

kwargs: ListAnalyzedResourcesRequestRequestTypeDef = {  # (1)
    "analyzerArn": ...,
}

parent.list_analyzed_resources(**kwargs)
```

1. See [:material-code-braces: ListAnalyzedResourcesRequestRequestTypeDef](./type_defs.md#listanalyzedresourcesrequestrequesttypedef) 

### list\_analyzers

Retrieves a list of analyzers.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").list_analyzers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/list_analyzers.html)

```python
# list_analyzers method definition

await def list_analyzers(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    type: TypeType = ...,  # (1)
) -> ListAnalyzersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-braces: ListAnalyzersResponseTypeDef](./type_defs.md#listanalyzersresponsetypedef) 


```python
# list_analyzers method usage example with argument unpacking

kwargs: ListAnalyzersRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_analyzers(**kwargs)
```

1. See [:material-code-braces: ListAnalyzersRequestRequestTypeDef](./type_defs.md#listanalyzersrequestrequesttypedef) 

### list\_archive\_rules

Retrieves a list of archive rules created for the specified analyzer.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").list_archive_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/list_archive_rules.html)

```python
# list_archive_rules method definition

await def list_archive_rules(
    self,
    *,
    analyzerName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListArchiveRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListArchiveRulesResponseTypeDef](./type_defs.md#listarchiverulesresponsetypedef) 


```python
# list_archive_rules method usage example with argument unpacking

kwargs: ListArchiveRulesRequestRequestTypeDef = {  # (1)
    "analyzerName": ...,
}

parent.list_archive_rules(**kwargs)
```

1. See [:material-code-braces: ListArchiveRulesRequestRequestTypeDef](./type_defs.md#listarchiverulesrequestrequesttypedef) 

### list\_findings

Retrieves a list of findings generated by the specified analyzer.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").list_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/list_findings.html)

```python
# list_findings method definition

await def list_findings(
    self,
    *,
    analyzerArn: str,
    filter: Mapping[str, CriterionTypeDef] = ...,  # (1)
    sort: SortCriteriaTypeDef = ...,  # (2)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListFindingsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: CriterionTypeDef](./type_defs.md#criteriontypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
3. See [:material-code-braces: ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef) 


```python
# list_findings method usage example with argument unpacking

kwargs: ListFindingsRequestRequestTypeDef = {  # (1)
    "analyzerArn": ...,
}

parent.list_findings(**kwargs)
```

1. See [:material-code-braces: ListFindingsRequestRequestTypeDef](./type_defs.md#listfindingsrequestrequesttypedef) 

### list\_findings\_v2

Retrieves a list of findings generated by the specified analyzer.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").list_findings_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/list_findings_v2.html)

```python
# list_findings_v2 method definition

await def list_findings_v2(
    self,
    *,
    analyzerArn: str,
    filter: Mapping[str, CriterionTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    sort: SortCriteriaTypeDef = ...,  # (2)
) -> ListFindingsV2ResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: CriterionTypeDef](./type_defs.md#criteriontypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
3. See [:material-code-braces: ListFindingsV2ResponseTypeDef](./type_defs.md#listfindingsv2responsetypedef) 


```python
# list_findings_v2 method usage example with argument unpacking

kwargs: ListFindingsV2RequestRequestTypeDef = {  # (1)
    "analyzerArn": ...,
}

parent.list_findings_v2(**kwargs)
```

1. See [:material-code-braces: ListFindingsV2RequestRequestTypeDef](./type_defs.md#listfindingsv2requestrequesttypedef) 

### list\_policy\_generations

Lists all of the policy generations requested in the last seven days.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").list_policy_generations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/list_policy_generations.html)

```python
# list_policy_generations method definition

await def list_policy_generations(
    self,
    *,
    principalArn: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListPolicyGenerationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPolicyGenerationsResponseTypeDef](./type_defs.md#listpolicygenerationsresponsetypedef) 


```python
# list_policy_generations method usage example with argument unpacking

kwargs: ListPolicyGenerationsRequestRequestTypeDef = {  # (1)
    "principalArn": ...,
}

parent.list_policy_generations(**kwargs)
```

1. See [:material-code-braces: ListPolicyGenerationsRequestRequestTypeDef](./type_defs.md#listpolicygenerationsrequestrequesttypedef) 

### list\_tags\_for\_resource

Retrieves a list of tags applied to the specified resource.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/list_tags_for_resource.html)

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

### start\_policy\_generation

Starts the policy generation request.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").start_policy_generation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/start_policy_generation.html)

```python
# start_policy_generation method definition

await def start_policy_generation(
    self,
    *,
    policyGenerationDetails: PolicyGenerationDetailsTypeDef,  # (1)
    cloudTrailDetails: CloudTrailDetailsTypeDef = ...,  # (2)
    clientToken: str = ...,
) -> StartPolicyGenerationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: PolicyGenerationDetailsTypeDef](./type_defs.md#policygenerationdetailstypedef) 
2. See [:material-code-braces: CloudTrailDetailsTypeDef](./type_defs.md#cloudtraildetailstypedef) 
3. See [:material-code-braces: StartPolicyGenerationResponseTypeDef](./type_defs.md#startpolicygenerationresponsetypedef) 


```python
# start_policy_generation method usage example with argument unpacking

kwargs: StartPolicyGenerationRequestRequestTypeDef = {  # (1)
    "policyGenerationDetails": ...,
}

parent.start_policy_generation(**kwargs)
```

1. See [:material-code-braces: StartPolicyGenerationRequestRequestTypeDef](./type_defs.md#startpolicygenerationrequestrequesttypedef) 

### start\_resource\_scan

Immediately starts a scan of the policies applied to the specified resource.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").start_resource_scan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/start_resource_scan.html)

```python
# start_resource_scan method definition

await def start_resource_scan(
    self,
    *,
    analyzerArn: str,
    resourceArn: str,
    resourceOwnerAccount: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_resource_scan method usage example with argument unpacking

kwargs: StartResourceScanRequestRequestTypeDef = {  # (1)
    "analyzerArn": ...,
    "resourceArn": ...,
}

parent.start_resource_scan(**kwargs)
```

1. See [:material-code-braces: StartResourceScanRequestRequestTypeDef](./type_defs.md#startresourcescanrequestrequesttypedef) 

### tag\_resource

Adds a tag to the specified resource.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/tag_resource.html)

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

Removes a tag from the specified resource.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/untag_resource.html)

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

### update\_analyzer

Modifies the configuration of an existing analyzer.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").update_analyzer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/update_analyzer.html)

```python
# update_analyzer method definition

await def update_analyzer(
    self,
    *,
    analyzerName: str,
    configuration: AnalyzerConfigurationTypeDef = ...,  # (1)
) -> UpdateAnalyzerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AnalyzerConfigurationTypeDef](./type_defs.md#analyzerconfigurationtypedef) 
2. See [:material-code-braces: UpdateAnalyzerResponseTypeDef](./type_defs.md#updateanalyzerresponsetypedef) 


```python
# update_analyzer method usage example with argument unpacking

kwargs: UpdateAnalyzerRequestRequestTypeDef = {  # (1)
    "analyzerName": ...,
}

parent.update_analyzer(**kwargs)
```

1. See [:material-code-braces: UpdateAnalyzerRequestRequestTypeDef](./type_defs.md#updateanalyzerrequestrequesttypedef) 

### update\_archive\_rule

Updates the criteria and values for the specified archive rule.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").update_archive_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/update_archive_rule.html)

```python
# update_archive_rule method definition

await def update_archive_rule(
    self,
    *,
    analyzerName: str,
    ruleName: str,
    filter: Mapping[str, CriterionTypeDef],  # (1)
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CriterionTypeDef](./type_defs.md#criteriontypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_archive_rule method usage example with argument unpacking

kwargs: UpdateArchiveRuleRequestRequestTypeDef = {  # (1)
    "analyzerName": ...,
    "ruleName": ...,
    "filter": ...,
}

parent.update_archive_rule(**kwargs)
```

1. See [:material-code-braces: UpdateArchiveRuleRequestRequestTypeDef](./type_defs.md#updatearchiverulerequestrequesttypedef) 

### update\_findings

Updates the status for the specified findings.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").update_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/update_findings.html)

```python
# update_findings method definition

await def update_findings(
    self,
    *,
    analyzerArn: str,
    status: FindingStatusUpdateType,  # (1)
    ids: Sequence[str] = ...,
    resourceArn: str = ...,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FindingStatusUpdateType](./literals.md#findingstatusupdatetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_findings method usage example with argument unpacking

kwargs: UpdateFindingsRequestRequestTypeDef = {  # (1)
    "analyzerArn": ...,
    "status": ...,
}

parent.update_findings(**kwargs)
```

1. See [:material-code-braces: UpdateFindingsRequestRequestTypeDef](./type_defs.md#updatefindingsrequestrequesttypedef) 

### validate\_policy

Requests the validation of a policy and returns a list of findings.

Type annotations and code completion for `#!python session.create_client("accessanalyzer").validate_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/client/validate_policy.html)

```python
# validate_policy method definition

await def validate_policy(
    self,
    *,
    policyDocument: str,
    policyType: PolicyTypeType,  # (1)
    locale: LocaleType = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
    validatePolicyResourceType: ValidatePolicyResourceTypeType = ...,  # (3)
) -> ValidatePolicyResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
3. See [:material-code-brackets: ValidatePolicyResourceTypeType](./literals.md#validatepolicyresourcetypetype) 
4. See [:material-code-braces: ValidatePolicyResponseTypeDef](./type_defs.md#validatepolicyresponsetypedef) 


```python
# validate_policy method usage example with argument unpacking

kwargs: ValidatePolicyRequestRequestTypeDef = {  # (1)
    "policyDocument": ...,
    "policyType": ...,
}

parent.validate_policy(**kwargs)
```

1. See [:material-code-braces: ValidatePolicyRequestRequestTypeDef](./type_defs.md#validatepolicyrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("accessanalyzer").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "AccessAnalyzerClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("accessanalyzer").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client)

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

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_paginator` method with overloads.

- `client.get_paginator("get_finding_recommendation")` -> [GetFindingRecommendationPaginator](./paginators.md#getfindingrecommendationpaginator)
- `client.get_paginator("get_finding_v2")` -> [GetFindingV2Paginator](./paginators.md#getfindingv2paginator)
- `client.get_paginator("list_access_preview_findings")` -> [ListAccessPreviewFindingsPaginator](./paginators.md#listaccesspreviewfindingspaginator)
- `client.get_paginator("list_access_previews")` -> [ListAccessPreviewsPaginator](./paginators.md#listaccesspreviewspaginator)
- `client.get_paginator("list_analyzed_resources")` -> [ListAnalyzedResourcesPaginator](./paginators.md#listanalyzedresourcespaginator)
- `client.get_paginator("list_analyzers")` -> [ListAnalyzersPaginator](./paginators.md#listanalyzerspaginator)
- `client.get_paginator("list_archive_rules")` -> [ListArchiveRulesPaginator](./paginators.md#listarchiverulespaginator)
- `client.get_paginator("list_findings")` -> [ListFindingsPaginator](./paginators.md#listfindingspaginator)
- `client.get_paginator("list_findings_v2")` -> [ListFindingsV2Paginator](./paginators.md#listfindingsv2paginator)
- `client.get_paginator("list_policy_generations")` -> [ListPolicyGenerationsPaginator](./paginators.md#listpolicygenerationspaginator)
- `client.get_paginator("validate_policy")` -> [ValidatePolicyPaginator](./paginators.md#validatepolicypaginator)



