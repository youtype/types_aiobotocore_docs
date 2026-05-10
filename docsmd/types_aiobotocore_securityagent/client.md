# SecurityAgentClient

> [Index](../README.md) > [SecurityAgent](./README.md) > SecurityAgentClient

!!! note ""

    Auto-generated documentation for [SecurityAgent](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent.html#securityagent)
    type annotations stubs module [types-aiobotocore-securityagent](https://pypi.org/project/types-aiobotocore-securityagent/).

## SecurityAgentClient

Type annotations and code completion for `#!python session.create_client("securityagent")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent.html#SecurityAgent.Client)

```python
# SecurityAgentClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_securityagent.client import SecurityAgentClient

session = get_session()
async with session.create_client("securityagent") as client:
    client: SecurityAgentClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("securityagent").exceptions` structure.

```python
# SecurityAgentClient.exceptions usage example

async with session.create_client("securityagent") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# SecurityAgentClient usage type checking example

from types_aiobotocore_securityagent.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("securityagent").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("securityagent").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/generate_presigned_url.html)

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


### add\_artifact

Uploads an artifact to an agent space.

Type annotations and code completion for `#!python session.create_client("securityagent").add_artifact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/add_artifact.html)

```python
# add_artifact method definition

await def add_artifact(
    self,
    *,
    agentSpaceId: str,
    artifactContent: BlobTypeDef,
    artifactType: ArtifactTypeType,  # (1)
    fileName: str,
) -> AddArtifactOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ArtifactTypeType](./literals.md#artifacttypetype)
2. See [:material-code-braces: AddArtifactOutputTypeDef](./type_defs.md#addartifactoutputtypedef)


```python
# add_artifact method usage example with argument unpacking

kwargs: AddArtifactInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "artifactContent": ...,
    "artifactType": ...,
    "fileName": ...,
}

parent.add_artifact(**kwargs)
```

1. See [:material-code-braces: AddArtifactInputTypeDef](./type_defs.md#addartifactinputtypedef)

### batch\_delete\_pentests

Deletes one or more pentests from an agent space.

Type annotations and code completion for `#!python session.create_client("securityagent").batch_delete_pentests` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/batch_delete_pentests.html)

```python
# batch_delete_pentests method definition

await def batch_delete_pentests(
    self,
    *,
    pentestIds: Sequence[str],
    agentSpaceId: str,
) -> BatchDeletePentestsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeletePentestsOutputTypeDef](./type_defs.md#batchdeletepentestsoutputtypedef)


```python
# batch_delete_pentests method usage example with argument unpacking

kwargs: BatchDeletePentestsInputTypeDef = {  # (1)
    "pentestIds": ...,
    "agentSpaceId": ...,
}

parent.batch_delete_pentests(**kwargs)
```

1. See [:material-code-braces: BatchDeletePentestsInputTypeDef](./type_defs.md#batchdeletepentestsinputtypedef)

### batch\_get\_agent\_spaces

Retrieves information about one or more agent spaces.

Type annotations and code completion for `#!python session.create_client("securityagent").batch_get_agent_spaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/batch_get_agent_spaces.html)

```python
# batch_get_agent_spaces method definition

await def batch_get_agent_spaces(
    self,
    *,
    agentSpaceIds: Sequence[str],
) -> BatchGetAgentSpacesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetAgentSpacesOutputTypeDef](./type_defs.md#batchgetagentspacesoutputtypedef)


```python
# batch_get_agent_spaces method usage example with argument unpacking

kwargs: BatchGetAgentSpacesInputTypeDef = {  # (1)
    "agentSpaceIds": ...,
}

parent.batch_get_agent_spaces(**kwargs)
```

1. See [:material-code-braces: BatchGetAgentSpacesInputTypeDef](./type_defs.md#batchgetagentspacesinputtypedef)

### batch\_get\_artifact\_metadata

Retrieves metadata for one or more artifacts in an agent space.

Type annotations and code completion for `#!python session.create_client("securityagent").batch_get_artifact_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/batch_get_artifact_metadata.html)

```python
# batch_get_artifact_metadata method definition

await def batch_get_artifact_metadata(
    self,
    *,
    agentSpaceId: str,
    artifactIds: Sequence[str],
) -> BatchGetArtifactMetadataOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetArtifactMetadataOutputTypeDef](./type_defs.md#batchgetartifactmetadataoutputtypedef)


```python
# batch_get_artifact_metadata method usage example with argument unpacking

kwargs: BatchGetArtifactMetadataInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "artifactIds": ...,
}

parent.batch_get_artifact_metadata(**kwargs)
```

1. See [:material-code-braces: BatchGetArtifactMetadataInputTypeDef](./type_defs.md#batchgetartifactmetadatainputtypedef)

### batch\_get\_findings

Retrieves information about one or more security findings in an agent space.

Type annotations and code completion for `#!python session.create_client("securityagent").batch_get_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/batch_get_findings.html)

```python
# batch_get_findings method definition

await def batch_get_findings(
    self,
    *,
    findingIds: Sequence[str],
    agentSpaceId: str,
) -> BatchGetFindingsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetFindingsOutputTypeDef](./type_defs.md#batchgetfindingsoutputtypedef)


```python
# batch_get_findings method usage example with argument unpacking

kwargs: BatchGetFindingsInputTypeDef = {  # (1)
    "findingIds": ...,
    "agentSpaceId": ...,
}

parent.batch_get_findings(**kwargs)
```

1. See [:material-code-braces: BatchGetFindingsInputTypeDef](./type_defs.md#batchgetfindingsinputtypedef)

### batch\_get\_pentest\_job\_tasks

Retrieves information about one or more tasks within a pentest job.

Type annotations and code completion for `#!python session.create_client("securityagent").batch_get_pentest_job_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/batch_get_pentest_job_tasks.html)

```python
# batch_get_pentest_job_tasks method definition

await def batch_get_pentest_job_tasks(
    self,
    *,
    agentSpaceId: str,
    taskIds: Sequence[str],
) -> BatchGetPentestJobTasksOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetPentestJobTasksOutputTypeDef](./type_defs.md#batchgetpentestjobtasksoutputtypedef)


```python
# batch_get_pentest_job_tasks method usage example with argument unpacking

kwargs: BatchGetPentestJobTasksInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "taskIds": ...,
}

parent.batch_get_pentest_job_tasks(**kwargs)
```

1. See [:material-code-braces: BatchGetPentestJobTasksInputTypeDef](./type_defs.md#batchgetpentestjobtasksinputtypedef)

### batch\_get\_pentest\_jobs

Retrieves information about one or more pentest jobs in an agent space.

Type annotations and code completion for `#!python session.create_client("securityagent").batch_get_pentest_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/batch_get_pentest_jobs.html)

```python
# batch_get_pentest_jobs method definition

await def batch_get_pentest_jobs(
    self,
    *,
    pentestJobIds: Sequence[str],
    agentSpaceId: str,
) -> BatchGetPentestJobsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetPentestJobsOutputTypeDef](./type_defs.md#batchgetpentestjobsoutputtypedef)


```python
# batch_get_pentest_jobs method usage example with argument unpacking

kwargs: BatchGetPentestJobsInputTypeDef = {  # (1)
    "pentestJobIds": ...,
    "agentSpaceId": ...,
}

parent.batch_get_pentest_jobs(**kwargs)
```

1. See [:material-code-braces: BatchGetPentestJobsInputTypeDef](./type_defs.md#batchgetpentestjobsinputtypedef)

### batch\_get\_pentests

Retrieves information about one or more pentests in an agent space.

Type annotations and code completion for `#!python session.create_client("securityagent").batch_get_pentests` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/batch_get_pentests.html)

```python
# batch_get_pentests method definition

await def batch_get_pentests(
    self,
    *,
    pentestIds: Sequence[str],
    agentSpaceId: str,
) -> BatchGetPentestsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetPentestsOutputTypeDef](./type_defs.md#batchgetpentestsoutputtypedef)


```python
# batch_get_pentests method usage example with argument unpacking

kwargs: BatchGetPentestsInputTypeDef = {  # (1)
    "pentestIds": ...,
    "agentSpaceId": ...,
}

parent.batch_get_pentests(**kwargs)
```

1. See [:material-code-braces: BatchGetPentestsInputTypeDef](./type_defs.md#batchgetpentestsinputtypedef)

### batch\_get\_target\_domains

Retrieves information about one or more target domains.

Type annotations and code completion for `#!python session.create_client("securityagent").batch_get_target_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/batch_get_target_domains.html)

```python
# batch_get_target_domains method definition

await def batch_get_target_domains(
    self,
    *,
    targetDomainIds: Sequence[str],
) -> BatchGetTargetDomainsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetTargetDomainsOutputTypeDef](./type_defs.md#batchgettargetdomainsoutputtypedef)


```python
# batch_get_target_domains method usage example with argument unpacking

kwargs: BatchGetTargetDomainsInputTypeDef = {  # (1)
    "targetDomainIds": ...,
}

parent.batch_get_target_domains(**kwargs)
```

1. See [:material-code-braces: BatchGetTargetDomainsInputTypeDef](./type_defs.md#batchgettargetdomainsinputtypedef)

### create\_agent\_space

Creates a new agent space.

Type annotations and code completion for `#!python session.create_client("securityagent").create_agent_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/create_agent_space.html)

```python
# create_agent_space method definition

await def create_agent_space(
    self,
    *,
    name: str,
    description: str = ...,
    awsResources: AWSResourcesUnionTypeDef = ...,  # (1)
    targetDomainIds: Sequence[str] = ...,
    codeReviewSettings: CodeReviewSettingsTypeDef = ...,  # (2)
    kmsKeyId: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateAgentSpaceOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AWSResourcesUnionTypeDef](#awsresourcesuniontypedef)
2. See [:material-code-braces: CodeReviewSettingsTypeDef](./type_defs.md#codereviewsettingstypedef)
3. See [:material-code-braces: CreateAgentSpaceOutputTypeDef](./type_defs.md#createagentspaceoutputtypedef)


```python
# create_agent_space method usage example with argument unpacking

kwargs: CreateAgentSpaceInputTypeDef = {  # (1)
    "name": ...,
}

parent.create_agent_space(**kwargs)
```

1. See [:material-code-braces: CreateAgentSpaceInputTypeDef](./type_defs.md#createagentspaceinputtypedef)

### create\_application

Creates a new application.

Type annotations and code completion for `#!python session.create_client("securityagent").create_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/create_application.html)

```python
# create_application method definition

await def create_application(
    self,
    *,
    idcInstanceArn: str = ...,
    roleArn: str = ...,
    defaultKmsKeyId: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef)


```python
# create_application method usage example with argument unpacking

kwargs: CreateApplicationRequestTypeDef = {  # (1)
    "idcInstanceArn": ...,
}

parent.create_application(**kwargs)
```

1. See [:material-code-braces: CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef)

### create\_integration

Creates a new integration with a third-party provider, such as GitHub, for code
review and remediation.

Type annotations and code completion for `#!python session.create_client("securityagent").create_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/create_integration.html)

```python
# create_integration method definition

await def create_integration(
    self,
    *,
    provider: ProviderType,  # (1)
    input: ProviderInputTypeDef,  # (2)
    integrationDisplayName: str,
    kmsKeyId: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateIntegrationOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ProviderType](./literals.md#providertype)
2. See [:material-code-braces: ProviderInputTypeDef](./type_defs.md#providerinputtypedef)
3. See [:material-code-braces: CreateIntegrationOutputTypeDef](./type_defs.md#createintegrationoutputtypedef)


```python
# create_integration method usage example with argument unpacking

kwargs: CreateIntegrationInputTypeDef = {  # (1)
    "provider": ...,
    "input": ...,
    "integrationDisplayName": ...,
}

parent.create_integration(**kwargs)
```

1. See [:material-code-braces: CreateIntegrationInputTypeDef](./type_defs.md#createintegrationinputtypedef)

### create\_membership

Creates a new membership, granting a user access to an agent space within an
application.

Type annotations and code completion for `#!python session.create_client("securityagent").create_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/create_membership.html)

```python
# create_membership method definition

await def create_membership(
    self,
    *,
    applicationId: str,
    agentSpaceId: str,
    membershipId: str,
    memberType: MembershipTypeType,  # (1)
    config: MembershipConfigTypeDef = ...,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype)
2. See [:material-code-braces: MembershipConfigTypeDef](./type_defs.md#membershipconfigtypedef)


```python
# create_membership method usage example with argument unpacking

kwargs: CreateMembershipRequestTypeDef = {  # (1)
    "applicationId": ...,
    "agentSpaceId": ...,
    "membershipId": ...,
    "memberType": ...,
}

parent.create_membership(**kwargs)
```

1. See [:material-code-braces: CreateMembershipRequestTypeDef](./type_defs.md#createmembershiprequesttypedef)

### create\_pentest

Creates a new pentest configuration in an agent space.

Type annotations and code completion for `#!python session.create_client("securityagent").create_pentest` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/create_pentest.html)

```python
# create_pentest method definition

await def create_pentest(
    self,
    *,
    title: str,
    agentSpaceId: str,
    assets: AssetsUnionTypeDef = ...,  # (1)
    excludeRiskTypes: Sequence[RiskTypeType] = ...,  # (2)
    serviceRole: str = ...,
    logConfig: CloudWatchLogTypeDef = ...,  # (3)
    vpcConfig: VpcConfigUnionTypeDef = ...,  # (4)
    networkTrafficConfig: NetworkTrafficConfigUnionTypeDef = ...,  # (5)
    codeRemediationStrategy: CodeRemediationStrategyType = ...,  # (6)
) -> CreatePentestOutputTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: AssetsUnionTypeDef](#assetsuniontypedef)
2. See `Sequence[RiskTypeType]`
3. See [:material-code-braces: CloudWatchLogTypeDef](./type_defs.md#cloudwatchlogtypedef)
4. See [:material-code-braces: VpcConfigUnionTypeDef](#vpcconfiguniontypedef)
5. See [:material-code-braces: NetworkTrafficConfigUnionTypeDef](#networktrafficconfiguniontypedef)
6. See [:material-code-brackets: CodeRemediationStrategyType](./literals.md#coderemediationstrategytype)
7. See [:material-code-braces: CreatePentestOutputTypeDef](./type_defs.md#createpentestoutputtypedef)


```python
# create_pentest method usage example with argument unpacking

kwargs: CreatePentestInputTypeDef = {  # (1)
    "title": ...,
    "agentSpaceId": ...,
}

parent.create_pentest(**kwargs)
```

1. See [:material-code-braces: CreatePentestInputTypeDef](./type_defs.md#createpentestinputtypedef)

### create\_target\_domain

Creates a new target domain for penetration testing.

Type annotations and code completion for `#!python session.create_client("securityagent").create_target_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/create_target_domain.html)

```python
# create_target_domain method definition

await def create_target_domain(
    self,
    *,
    targetDomainName: str,
    verificationMethod: DomainVerificationMethodType,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateTargetDomainOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DomainVerificationMethodType](./literals.md#domainverificationmethodtype)
2. See [:material-code-braces: CreateTargetDomainOutputTypeDef](./type_defs.md#createtargetdomainoutputtypedef)


```python
# create_target_domain method usage example with argument unpacking

kwargs: CreateTargetDomainInputTypeDef = {  # (1)
    "targetDomainName": ...,
    "verificationMethod": ...,
}

parent.create_target_domain(**kwargs)
```

1. See [:material-code-braces: CreateTargetDomainInputTypeDef](./type_defs.md#createtargetdomaininputtypedef)

### delete\_agent\_space

Deletes an agent space and all of its associated resources, including pentests,
findings, and artifacts.

Type annotations and code completion for `#!python session.create_client("securityagent").delete_agent_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/delete_agent_space.html)

```python
# delete_agent_space method definition

await def delete_agent_space(
    self,
    *,
    agentSpaceId: str,
) -> DeleteAgentSpaceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAgentSpaceOutputTypeDef](./type_defs.md#deleteagentspaceoutputtypedef)


```python
# delete_agent_space method usage example with argument unpacking

kwargs: DeleteAgentSpaceInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.delete_agent_space(**kwargs)
```

1. See [:material-code-braces: DeleteAgentSpaceInputTypeDef](./type_defs.md#deleteagentspaceinputtypedef)

### delete\_application

Deletes an application and its associated configuration, including IAM Identity
Center settings.

Type annotations and code completion for `#!python session.create_client("securityagent").delete_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/delete_application.html)

```python
# delete_application method definition

await def delete_application(
    self,
    *,
    applicationId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_application method usage example with argument unpacking

kwargs: DeleteApplicationRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.delete_application(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationRequestTypeDef](./type_defs.md#deleteapplicationrequesttypedef)

### delete\_artifact

Deletes an artifact from an agent space.

Type annotations and code completion for `#!python session.create_client("securityagent").delete_artifact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/delete_artifact.html)

```python
# delete_artifact method definition

await def delete_artifact(
    self,
    *,
    agentSpaceId: str,
    artifactId: str,
) -> dict[str, Any]:
    ...
```

```python
# delete_artifact method usage example with argument unpacking

kwargs: DeleteArtifactInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "artifactId": ...,
}

parent.delete_artifact(**kwargs)
```

1. See [:material-code-braces: DeleteArtifactInputTypeDef](./type_defs.md#deleteartifactinputtypedef)

### delete\_integration

Deletes an integration with a third-party provider.

Type annotations and code completion for `#!python session.create_client("securityagent").delete_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/delete_integration.html)

```python
# delete_integration method definition

await def delete_integration(
    self,
    *,
    integrationId: str,
) -> dict[str, Any]:
    ...
```

```python
# delete_integration method usage example with argument unpacking

kwargs: DeleteIntegrationInputTypeDef = {  # (1)
    "integrationId": ...,
}

parent.delete_integration(**kwargs)
```

1. See [:material-code-braces: DeleteIntegrationInputTypeDef](./type_defs.md#deleteintegrationinputtypedef)

### delete\_membership

Deletes a membership, revoking a user's access to an agent space.

Type annotations and code completion for `#!python session.create_client("securityagent").delete_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/delete_membership.html)

```python
# delete_membership method definition

await def delete_membership(
    self,
    *,
    applicationId: str,
    agentSpaceId: str,
    membershipId: str,
    memberType: MembershipTypeType = ...,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype)


```python
# delete_membership method usage example with argument unpacking

kwargs: DeleteMembershipRequestTypeDef = {  # (1)
    "applicationId": ...,
    "agentSpaceId": ...,
    "membershipId": ...,
}

parent.delete_membership(**kwargs)
```

1. See [:material-code-braces: DeleteMembershipRequestTypeDef](./type_defs.md#deletemembershiprequesttypedef)

### delete\_target\_domain

Deletes a target domain registration.

Type annotations and code completion for `#!python session.create_client("securityagent").delete_target_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/delete_target_domain.html)

```python
# delete_target_domain method definition

await def delete_target_domain(
    self,
    *,
    targetDomainId: str,
) -> DeleteTargetDomainOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTargetDomainOutputTypeDef](./type_defs.md#deletetargetdomainoutputtypedef)


```python
# delete_target_domain method usage example with argument unpacking

kwargs: DeleteTargetDomainInputTypeDef = {  # (1)
    "targetDomainId": ...,
}

parent.delete_target_domain(**kwargs)
```

1. See [:material-code-braces: DeleteTargetDomainInputTypeDef](./type_defs.md#deletetargetdomaininputtypedef)

### get\_application

Retrieves information about an application.

Type annotations and code completion for `#!python session.create_client("securityagent").get_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/get_application.html)

```python
# get_application method definition

await def get_application(
    self,
    *,
    applicationId: str,
) -> GetApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApplicationResponseTypeDef](./type_defs.md#getapplicationresponsetypedef)


```python
# get_application method usage example with argument unpacking

kwargs: GetApplicationRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.get_application(**kwargs)
```

1. See [:material-code-braces: GetApplicationRequestTypeDef](./type_defs.md#getapplicationrequesttypedef)

### get\_artifact

Retrieves an artifact from an agent space.

Type annotations and code completion for `#!python session.create_client("securityagent").get_artifact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/get_artifact.html)

```python
# get_artifact method definition

await def get_artifact(
    self,
    *,
    agentSpaceId: str,
    artifactId: str,
) -> GetArtifactOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetArtifactOutputTypeDef](./type_defs.md#getartifactoutputtypedef)


```python
# get_artifact method usage example with argument unpacking

kwargs: GetArtifactInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "artifactId": ...,
}

parent.get_artifact(**kwargs)
```

1. See [:material-code-braces: GetArtifactInputTypeDef](./type_defs.md#getartifactinputtypedef)

### get\_integration

Retrieves information about an integration.

Type annotations and code completion for `#!python session.create_client("securityagent").get_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/get_integration.html)

```python
# get_integration method definition

await def get_integration(
    self,
    *,
    integrationId: str,
) -> GetIntegrationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIntegrationOutputTypeDef](./type_defs.md#getintegrationoutputtypedef)


```python
# get_integration method usage example with argument unpacking

kwargs: GetIntegrationInputTypeDef = {  # (1)
    "integrationId": ...,
}

parent.get_integration(**kwargs)
```

1. See [:material-code-braces: GetIntegrationInputTypeDef](./type_defs.md#getintegrationinputtypedef)

### initiate\_provider\_registration

Initiates the OAuth registration flow with a third-party provider.

Type annotations and code completion for `#!python session.create_client("securityagent").initiate_provider_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/initiate_provider_registration.html)

```python
# initiate_provider_registration method definition

await def initiate_provider_registration(
    self,
    *,
    provider: ProviderType,  # (1)
) -> InitiateProviderRegistrationOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ProviderType](./literals.md#providertype)
2. See [:material-code-braces: InitiateProviderRegistrationOutputTypeDef](./type_defs.md#initiateproviderregistrationoutputtypedef)


```python
# initiate_provider_registration method usage example with argument unpacking

kwargs: InitiateProviderRegistrationInputTypeDef = {  # (1)
    "provider": ...,
}

parent.initiate_provider_registration(**kwargs)
```

1. See [:material-code-braces: InitiateProviderRegistrationInputTypeDef](./type_defs.md#initiateproviderregistrationinputtypedef)

### list\_agent\_spaces

Returns a paginated list of agent space summaries in your account.

Type annotations and code completion for `#!python session.create_client("securityagent").list_agent_spaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/list_agent_spaces.html)

```python
# list_agent_spaces method definition

await def list_agent_spaces(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAgentSpacesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentSpacesOutputTypeDef](./type_defs.md#listagentspacesoutputtypedef)


```python
# list_agent_spaces method usage example with argument unpacking

kwargs: ListAgentSpacesInputTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_agent_spaces(**kwargs)
```

1. See [:material-code-braces: ListAgentSpacesInputTypeDef](./type_defs.md#listagentspacesinputtypedef)

### list\_applications

Returns a paginated list of application summaries in your account.

Type annotations and code completion for `#!python session.create_client("securityagent").list_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/list_applications.html)

```python
# list_applications method definition

await def list_applications(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListApplicationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)


```python
# list_applications method usage example with argument unpacking

kwargs: ListApplicationsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_applications(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestTypeDef](./type_defs.md#listapplicationsrequesttypedef)

### list\_artifacts

Returns a paginated list of artifact summaries for the specified agent space.

Type annotations and code completion for `#!python session.create_client("securityagent").list_artifacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/list_artifacts.html)

```python
# list_artifacts method definition

await def list_artifacts(
    self,
    *,
    agentSpaceId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListArtifactsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListArtifactsOutputTypeDef](./type_defs.md#listartifactsoutputtypedef)


```python
# list_artifacts method usage example with argument unpacking

kwargs: ListArtifactsInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.list_artifacts(**kwargs)
```

1. See [:material-code-braces: ListArtifactsInputTypeDef](./type_defs.md#listartifactsinputtypedef)

### list\_discovered\_endpoints

Returns a paginated list of endpoints discovered during a pentest job execution.

Type annotations and code completion for `#!python session.create_client("securityagent").list_discovered_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/list_discovered_endpoints.html)

```python
# list_discovered_endpoints method definition

await def list_discovered_endpoints(
    self,
    *,
    pentestJobId: str,
    agentSpaceId: str,
    maxResults: int = ...,
    prefix: str = ...,
    nextToken: str = ...,
) -> ListDiscoveredEndpointsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDiscoveredEndpointsOutputTypeDef](./type_defs.md#listdiscoveredendpointsoutputtypedef)


```python
# list_discovered_endpoints method usage example with argument unpacking

kwargs: ListDiscoveredEndpointsInputTypeDef = {  # (1)
    "pentestJobId": ...,
    "agentSpaceId": ...,
}

parent.list_discovered_endpoints(**kwargs)
```

1. See [:material-code-braces: ListDiscoveredEndpointsInputTypeDef](./type_defs.md#listdiscoveredendpointsinputtypedef)

### list\_findings

Lists the security findings for a pentest job.

Type annotations and code completion for `#!python session.create_client("securityagent").list_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/list_findings.html)

```python
# list_findings method definition

await def list_findings(
    self,
    *,
    pentestJobId: str,
    agentSpaceId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    riskType: str = ...,
    riskLevel: RiskLevelType = ...,  # (1)
    status: FindingStatusType = ...,  # (2)
    confidence: ConfidenceLevelType = ...,  # (3)
    name: str = ...,
) -> ListFindingsOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: RiskLevelType](./literals.md#riskleveltype)
2. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype)
3. See [:material-code-brackets: ConfidenceLevelType](./literals.md#confidenceleveltype)
4. See [:material-code-braces: ListFindingsOutputTypeDef](./type_defs.md#listfindingsoutputtypedef)


```python
# list_findings method usage example with argument unpacking

kwargs: ListFindingsInputTypeDef = {  # (1)
    "pentestJobId": ...,
    "agentSpaceId": ...,
}

parent.list_findings(**kwargs)
```

1. See [:material-code-braces: ListFindingsInputTypeDef](./type_defs.md#listfindingsinputtypedef)

### list\_integrated\_resources

Lists the integrated resources for an agent space, optionally filtered by
integration or resource type.

Type annotations and code completion for `#!python session.create_client("securityagent").list_integrated_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/list_integrated_resources.html)

```python
# list_integrated_resources method definition

await def list_integrated_resources(
    self,
    *,
    agentSpaceId: str,
    integrationId: str = ...,
    resourceType: ResourceTypeType = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListIntegratedResourcesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype)
2. See [:material-code-braces: ListIntegratedResourcesOutputTypeDef](./type_defs.md#listintegratedresourcesoutputtypedef)


```python
# list_integrated_resources method usage example with argument unpacking

kwargs: ListIntegratedResourcesInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.list_integrated_resources(**kwargs)
```

1. See [:material-code-braces: ListIntegratedResourcesInputTypeDef](./type_defs.md#listintegratedresourcesinputtypedef)

### list\_integrations

Lists the integrations in your account, optionally filtered by provider or
provider type.

Type annotations and code completion for `#!python session.create_client("securityagent").list_integrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/list_integrations.html)

```python
# list_integrations method definition

await def list_integrations(
    self,
    *,
    filter: IntegrationFilterTypeDef = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListIntegrationsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IntegrationFilterTypeDef](./type_defs.md#integrationfiltertypedef)
2. See [:material-code-braces: ListIntegrationsOutputTypeDef](./type_defs.md#listintegrationsoutputtypedef)


```python
# list_integrations method usage example with argument unpacking

kwargs: ListIntegrationsInputTypeDef = {  # (1)
    "filter": ...,
}

parent.list_integrations(**kwargs)
```

1. See [:material-code-braces: ListIntegrationsInputTypeDef](./type_defs.md#listintegrationsinputtypedef)

### list\_memberships

Returns a paginated list of membership summaries for the specified agent space
within an application.

Type annotations and code completion for `#!python session.create_client("securityagent").list_memberships` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/list_memberships.html)

```python
# list_memberships method definition

await def list_memberships(
    self,
    *,
    applicationId: str,
    agentSpaceId: str,
    memberType: MembershipTypeFilterType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMembershipsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MembershipTypeFilterType](./literals.md#membershiptypefiltertype)
2. See [:material-code-braces: ListMembershipsResponseTypeDef](./type_defs.md#listmembershipsresponsetypedef)


```python
# list_memberships method usage example with argument unpacking

kwargs: ListMembershipsRequestTypeDef = {  # (1)
    "applicationId": ...,
    "agentSpaceId": ...,
}

parent.list_memberships(**kwargs)
```

1. See [:material-code-braces: ListMembershipsRequestTypeDef](./type_defs.md#listmembershipsrequesttypedef)

### list\_pentest\_job\_tasks

Returns a paginated list of task summaries for the specified pentest job,
optionally filtered by step name or category.

Type annotations and code completion for `#!python session.create_client("securityagent").list_pentest_job_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/list_pentest_job_tasks.html)

```python
# list_pentest_job_tasks method definition

await def list_pentest_job_tasks(
    self,
    *,
    agentSpaceId: str,
    maxResults: int = ...,
    pentestJobId: str = ...,
    stepName: StepNameType = ...,  # (1)
    categoryName: str = ...,
    nextToken: str = ...,
) -> ListPentestJobTasksOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StepNameType](./literals.md#stepnametype)
2. See [:material-code-braces: ListPentestJobTasksOutputTypeDef](./type_defs.md#listpentestjobtasksoutputtypedef)


```python
# list_pentest_job_tasks method usage example with argument unpacking

kwargs: ListPentestJobTasksInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.list_pentest_job_tasks(**kwargs)
```

1. See [:material-code-braces: ListPentestJobTasksInputTypeDef](./type_defs.md#listpentestjobtasksinputtypedef)

### list\_pentest\_jobs\_for\_pentest

Returns a paginated list of pentest job summaries for the specified pentest
configuration.

Type annotations and code completion for `#!python session.create_client("securityagent").list_pentest_jobs_for_pentest` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/list_pentest_jobs_for_pentest.html)

```python
# list_pentest_jobs_for_pentest method definition

await def list_pentest_jobs_for_pentest(
    self,
    *,
    pentestId: str,
    agentSpaceId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListPentestJobsForPentestOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPentestJobsForPentestOutputTypeDef](./type_defs.md#listpentestjobsforpentestoutputtypedef)


```python
# list_pentest_jobs_for_pentest method usage example with argument unpacking

kwargs: ListPentestJobsForPentestInputTypeDef = {  # (1)
    "pentestId": ...,
    "agentSpaceId": ...,
}

parent.list_pentest_jobs_for_pentest(**kwargs)
```

1. See [:material-code-braces: ListPentestJobsForPentestInputTypeDef](./type_defs.md#listpentestjobsforpentestinputtypedef)

### list\_pentests

Returns a paginated list of pentest summaries for the specified agent space.

Type annotations and code completion for `#!python session.create_client("securityagent").list_pentests` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/list_pentests.html)

```python
# list_pentests method definition

await def list_pentests(
    self,
    *,
    agentSpaceId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListPentestsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPentestsOutputTypeDef](./type_defs.md#listpentestsoutputtypedef)


```python
# list_pentests method usage example with argument unpacking

kwargs: ListPentestsInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.list_pentests(**kwargs)
```

1. See [:material-code-braces: ListPentestsInputTypeDef](./type_defs.md#listpentestsinputtypedef)

### list\_tags\_for\_resource

Returns the tags associated with the specified resource.

Type annotations and code completion for `#!python session.create_client("securityagent").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/list_tags_for_resource.html)

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

### list\_target\_domains

Returns a paginated list of target domain summaries in your account.

Type annotations and code completion for `#!python session.create_client("securityagent").list_target_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/list_target_domains.html)

```python
# list_target_domains method definition

await def list_target_domains(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTargetDomainsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTargetDomainsOutputTypeDef](./type_defs.md#listtargetdomainsoutputtypedef)


```python
# list_target_domains method usage example with argument unpacking

kwargs: ListTargetDomainsInputTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_target_domains(**kwargs)
```

1. See [:material-code-braces: ListTargetDomainsInputTypeDef](./type_defs.md#listtargetdomainsinputtypedef)

### start\_code\_remediation

Initiates code remediation for one or more security findings.

Type annotations and code completion for `#!python session.create_client("securityagent").start_code_remediation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/start_code_remediation.html)

```python
# start_code_remediation method definition

await def start_code_remediation(
    self,
    *,
    agentSpaceId: str,
    pentestJobId: str,
    findingIds: Sequence[str],
) -> dict[str, Any]:
    ...
```

```python
# start_code_remediation method usage example with argument unpacking

kwargs: StartCodeRemediationInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "pentestJobId": ...,
    "findingIds": ...,
}

parent.start_code_remediation(**kwargs)
```

1. See [:material-code-braces: StartCodeRemediationInputTypeDef](./type_defs.md#startcoderemediationinputtypedef)

### start\_pentest\_job

Starts a new pentest job for a pentest configuration.

Type annotations and code completion for `#!python session.create_client("securityagent").start_pentest_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/start_pentest_job.html)

```python
# start_pentest_job method definition

await def start_pentest_job(
    self,
    *,
    agentSpaceId: str,
    pentestId: str,
) -> StartPentestJobOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartPentestJobOutputTypeDef](./type_defs.md#startpentestjoboutputtypedef)


```python
# start_pentest_job method usage example with argument unpacking

kwargs: StartPentestJobInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "pentestId": ...,
}

parent.start_pentest_job(**kwargs)
```

1. See [:material-code-braces: StartPentestJobInputTypeDef](./type_defs.md#startpentestjobinputtypedef)

### stop\_pentest\_job

Stops a running pentest job.

Type annotations and code completion for `#!python session.create_client("securityagent").stop_pentest_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/stop_pentest_job.html)

```python
# stop_pentest_job method definition

await def stop_pentest_job(
    self,
    *,
    agentSpaceId: str,
    pentestJobId: str,
) -> dict[str, Any]:
    ...
```

```python
# stop_pentest_job method usage example with argument unpacking

kwargs: StopPentestJobInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "pentestJobId": ...,
}

parent.stop_pentest_job(**kwargs)
```

1. See [:material-code-braces: StopPentestJobInputTypeDef](./type_defs.md#stoppentestjobinputtypedef)

### tag\_resource

Adds tags to a resource.

Type annotations and code completion for `#!python session.create_client("securityagent").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> dict[str, Any]:
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

Removes tags from a resource.

Type annotations and code completion for `#!python session.create_client("securityagent").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> dict[str, Any]:
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

### update\_agent\_space

Updates the configuration of an existing agent space, including its name,
description, AWS resources, target domains, and code review settings.

Type annotations and code completion for `#!python session.create_client("securityagent").update_agent_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/update_agent_space.html)

```python
# update_agent_space method definition

await def update_agent_space(
    self,
    *,
    agentSpaceId: str,
    name: str = ...,
    description: str = ...,
    awsResources: AWSResourcesUnionTypeDef = ...,  # (1)
    targetDomainIds: Sequence[str] = ...,
    codeReviewSettings: CodeReviewSettingsTypeDef = ...,  # (2)
) -> UpdateAgentSpaceOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AWSResourcesUnionTypeDef](#awsresourcesuniontypedef)
2. See [:material-code-braces: CodeReviewSettingsTypeDef](./type_defs.md#codereviewsettingstypedef)
3. See [:material-code-braces: UpdateAgentSpaceOutputTypeDef](./type_defs.md#updateagentspaceoutputtypedef)


```python
# update_agent_space method usage example with argument unpacking

kwargs: UpdateAgentSpaceInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.update_agent_space(**kwargs)
```

1. See [:material-code-braces: UpdateAgentSpaceInputTypeDef](./type_defs.md#updateagentspaceinputtypedef)

### update\_application

Updates the configuration of an existing application, including the IAM role
and default KMS key.

Type annotations and code completion for `#!python session.create_client("securityagent").update_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/update_application.html)

```python
# update_application method definition

await def update_application(
    self,
    *,
    applicationId: str,
    roleArn: str = ...,
    defaultKmsKeyId: str = ...,
) -> UpdateApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateApplicationResponseTypeDef](./type_defs.md#updateapplicationresponsetypedef)


```python
# update_application method usage example with argument unpacking

kwargs: UpdateApplicationRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.update_application(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationRequestTypeDef](./type_defs.md#updateapplicationrequesttypedef)

### update\_finding

Updates the status or risk level of a security finding.

Type annotations and code completion for `#!python session.create_client("securityagent").update_finding` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/update_finding.html)

```python
# update_finding method definition

await def update_finding(
    self,
    *,
    findingId: str,
    agentSpaceId: str,
    riskLevel: RiskLevelType = ...,  # (1)
    status: FindingStatusType = ...,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: RiskLevelType](./literals.md#riskleveltype)
2. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype)


```python
# update_finding method usage example with argument unpacking

kwargs: UpdateFindingInputTypeDef = {  # (1)
    "findingId": ...,
    "agentSpaceId": ...,
}

parent.update_finding(**kwargs)
```

1. See [:material-code-braces: UpdateFindingInputTypeDef](./type_defs.md#updatefindinginputtypedef)

### update\_integrated\_resources

Updates the integrated resources for an agent space, including their
capabilities.

Type annotations and code completion for `#!python session.create_client("securityagent").update_integrated_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/update_integrated_resources.html)

```python
# update_integrated_resources method definition

await def update_integrated_resources(
    self,
    *,
    agentSpaceId: str,
    integrationId: str,
    items: Sequence[IntegratedResourceInputItemTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See `Sequence[IntegratedResourceInputItemTypeDef]`


```python
# update_integrated_resources method usage example with argument unpacking

kwargs: UpdateIntegratedResourcesInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "integrationId": ...,
    "items": ...,
}

parent.update_integrated_resources(**kwargs)
```

1. See [:material-code-braces: UpdateIntegratedResourcesInputTypeDef](./type_defs.md#updateintegratedresourcesinputtypedef)

### update\_pentest

Updates an existing pentest configuration.

Type annotations and code completion for `#!python session.create_client("securityagent").update_pentest` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/update_pentest.html)

```python
# update_pentest method definition

await def update_pentest(
    self,
    *,
    pentestId: str,
    agentSpaceId: str,
    title: str = ...,
    assets: AssetsUnionTypeDef = ...,  # (1)
    excludeRiskTypes: Sequence[RiskTypeType] = ...,  # (2)
    serviceRole: str = ...,
    logConfig: CloudWatchLogTypeDef = ...,  # (3)
    vpcConfig: VpcConfigUnionTypeDef = ...,  # (4)
    networkTrafficConfig: NetworkTrafficConfigUnionTypeDef = ...,  # (5)
    codeRemediationStrategy: CodeRemediationStrategyType = ...,  # (6)
) -> UpdatePentestOutputTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: AssetsUnionTypeDef](#assetsuniontypedef)
2. See `Sequence[RiskTypeType]`
3. See [:material-code-braces: CloudWatchLogTypeDef](./type_defs.md#cloudwatchlogtypedef)
4. See [:material-code-braces: VpcConfigUnionTypeDef](#vpcconfiguniontypedef)
5. See [:material-code-braces: NetworkTrafficConfigUnionTypeDef](#networktrafficconfiguniontypedef)
6. See [:material-code-brackets: CodeRemediationStrategyType](./literals.md#coderemediationstrategytype)
7. See [:material-code-braces: UpdatePentestOutputTypeDef](./type_defs.md#updatepentestoutputtypedef)


```python
# update_pentest method usage example with argument unpacking

kwargs: UpdatePentestInputTypeDef = {  # (1)
    "pentestId": ...,
    "agentSpaceId": ...,
}

parent.update_pentest(**kwargs)
```

1. See [:material-code-braces: UpdatePentestInputTypeDef](./type_defs.md#updatepentestinputtypedef)

### update\_target\_domain

Updates the verification method for a target domain.

Type annotations and code completion for `#!python session.create_client("securityagent").update_target_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/update_target_domain.html)

```python
# update_target_domain method definition

await def update_target_domain(
    self,
    *,
    targetDomainId: str,
    verificationMethod: DomainVerificationMethodType,  # (1)
) -> UpdateTargetDomainOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DomainVerificationMethodType](./literals.md#domainverificationmethodtype)
2. See [:material-code-braces: UpdateTargetDomainOutputTypeDef](./type_defs.md#updatetargetdomainoutputtypedef)


```python
# update_target_domain method usage example with argument unpacking

kwargs: UpdateTargetDomainInputTypeDef = {  # (1)
    "targetDomainId": ...,
    "verificationMethod": ...,
}

parent.update_target_domain(**kwargs)
```

1. See [:material-code-braces: UpdateTargetDomainInputTypeDef](./type_defs.md#updatetargetdomaininputtypedef)

### verify\_target\_domain

Initiates verification of a target domain.

Type annotations and code completion for `#!python session.create_client("securityagent").verify_target_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent/client/verify_target_domain.html)

```python
# verify_target_domain method definition

await def verify_target_domain(
    self,
    *,
    targetDomainId: str,
) -> VerifyTargetDomainOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: VerifyTargetDomainOutputTypeDef](./type_defs.md#verifytargetdomainoutputtypedef)


```python
# verify_target_domain method usage example with argument unpacking

kwargs: VerifyTargetDomainInputTypeDef = {  # (1)
    "targetDomainId": ...,
}

parent.verify_target_domain(**kwargs)
```

1. See [:material-code-braces: VerifyTargetDomainInputTypeDef](./type_defs.md#verifytargetdomaininputtypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("securityagent").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent.html#SecurityAgent.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("securityagent").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent.html#SecurityAgent.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("securityagent").get_paginator` method with overloads.

- `client.get_paginator("list_agent_spaces")` -> [ListAgentSpacesPaginator](./paginators.md#listagentspacespaginator)
- `client.get_paginator("list_applications")` -> [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- `client.get_paginator("list_artifacts")` -> [ListArtifactsPaginator](./paginators.md#listartifactspaginator)
- `client.get_paginator("list_discovered_endpoints")` -> [ListDiscoveredEndpointsPaginator](./paginators.md#listdiscoveredendpointspaginator)
- `client.get_paginator("list_findings")` -> [ListFindingsPaginator](./paginators.md#listfindingspaginator)
- `client.get_paginator("list_integrated_resources")` -> [ListIntegratedResourcesPaginator](./paginators.md#listintegratedresourcespaginator)
- `client.get_paginator("list_integrations")` -> [ListIntegrationsPaginator](./paginators.md#listintegrationspaginator)
- `client.get_paginator("list_memberships")` -> [ListMembershipsPaginator](./paginators.md#listmembershipspaginator)
- `client.get_paginator("list_pentest_job_tasks")` -> [ListPentestJobTasksPaginator](./paginators.md#listpentestjobtaskspaginator)
- `client.get_paginator("list_pentest_jobs_for_pentest")` -> [ListPentestJobsForPentestPaginator](./paginators.md#listpentestjobsforpentestpaginator)
- `client.get_paginator("list_pentests")` -> [ListPentestsPaginator](./paginators.md#listpentestspaginator)
- `client.get_paginator("list_target_domains")` -> [ListTargetDomainsPaginator](./paginators.md#listtargetdomainspaginator)



