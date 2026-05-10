# Type definitions

> [Index](../README.md) > [SecurityAgent](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SecurityAgent](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent.html#securityagent)
    type annotations stubs module [types-aiobotocore-securityagent](https://pypi.org/project/types-aiobotocore-securityagent/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_securityagent.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    aiobotocore.response.StreamingBody,
]
```


## VpcConfigUnionTypeDef

```python
# VpcConfigUnionTypeDef Union usage example

from types_aiobotocore_securityagent.type_defs import VpcConfigUnionTypeDef


def get_value() -> VpcConfigUnionTypeDef:
    return ...


# VpcConfigUnionTypeDef definition

VpcConfigUnionTypeDef = Union[
    VpcConfigTypeDef,  # (1)
    VpcConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef)
2. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)

## AWSResourcesUnionTypeDef

```python
# AWSResourcesUnionTypeDef Union usage example

from types_aiobotocore_securityagent.type_defs import AWSResourcesUnionTypeDef


def get_value() -> AWSResourcesUnionTypeDef:
    return ...


# AWSResourcesUnionTypeDef definition

AWSResourcesUnionTypeDef = Union[
    AWSResourcesTypeDef,  # (1)
    AWSResourcesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AWSResourcesTypeDef](./type_defs.md#awsresourcestypedef)
2. See [:material-code-braces: AWSResourcesOutputTypeDef](./type_defs.md#awsresourcesoutputtypedef)

## NetworkTrafficConfigUnionTypeDef

```python
# NetworkTrafficConfigUnionTypeDef Union usage example

from types_aiobotocore_securityagent.type_defs import NetworkTrafficConfigUnionTypeDef


def get_value() -> NetworkTrafficConfigUnionTypeDef:
    return ...


# NetworkTrafficConfigUnionTypeDef definition

NetworkTrafficConfigUnionTypeDef = Union[
    NetworkTrafficConfigTypeDef,  # (1)
    NetworkTrafficConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NetworkTrafficConfigTypeDef](./type_defs.md#networktrafficconfigtypedef)
2. See [:material-code-braces: NetworkTrafficConfigOutputTypeDef](./type_defs.md#networktrafficconfigoutputtypedef)

## AssetsUnionTypeDef

```python
# AssetsUnionTypeDef Union usage example

from types_aiobotocore_securityagent.type_defs import AssetsUnionTypeDef


def get_value() -> AssetsUnionTypeDef:
    return ...


# AssetsUnionTypeDef definition

AssetsUnionTypeDef = Union[
    AssetsTypeDef,  # (1)
    AssetsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AssetsTypeDef](./type_defs.md#assetstypedef)
2. See [:material-code-braces: AssetsOutputTypeDef](./type_defs.md#assetsoutputtypedef)



## VpcConfigOutputTypeDef

```python
# VpcConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import VpcConfigOutputTypeDef


def get_value() -> VpcConfigOutputTypeDef:
    return {
        "vpcArn": ...,
    }


# VpcConfigOutputTypeDef definition

class VpcConfigOutputTypeDef(TypedDict):
    vpcArn: NotRequired[str],
    securityGroupArns: NotRequired[list[str]],
    subnetArns: NotRequired[list[str]],
```


## VpcConfigTypeDef

```python
# VpcConfigTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import VpcConfigTypeDef


def get_value() -> VpcConfigTypeDef:
    return {
        "vpcArn": ...,
    }


# VpcConfigTypeDef definition

class VpcConfigTypeDef(TypedDict):
    vpcArn: NotRequired[str],
    securityGroupArns: NotRequired[Sequence[str]],
    subnetArns: NotRequired[Sequence[str]],
```


## AuthenticationTypeDef

```python
# AuthenticationTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import AuthenticationTypeDef


def get_value() -> AuthenticationTypeDef:
    return {
        "providerType": ...,
    }


# AuthenticationTypeDef definition

class AuthenticationTypeDef(TypedDict):
    providerType: NotRequired[AuthenticationProviderTypeType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: AuthenticationProviderTypeType](./literals.md#authenticationprovidertypetype)

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```


## AgentSpaceSummaryTypeDef

```python
# AgentSpaceSummaryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import AgentSpaceSummaryTypeDef


def get_value() -> AgentSpaceSummaryTypeDef:
    return {
        "agentSpaceId": ...,
    }


# AgentSpaceSummaryTypeDef definition

class AgentSpaceSummaryTypeDef(TypedDict):
    agentSpaceId: str,
    name: str,
    createdAt: NotRequired[datetime.datetime],
    updatedAt: NotRequired[datetime.datetime],
```


## CodeReviewSettingsTypeDef

```python
# CodeReviewSettingsTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CodeReviewSettingsTypeDef


def get_value() -> CodeReviewSettingsTypeDef:
    return {
        "controlsScanning": ...,
    }


# CodeReviewSettingsTypeDef definition

class CodeReviewSettingsTypeDef(TypedDict):
    controlsScanning: bool,
    generalPurposeScanning: bool,
```


## ApplicationSummaryTypeDef

```python
# ApplicationSummaryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ApplicationSummaryTypeDef


def get_value() -> ApplicationSummaryTypeDef:
    return {
        "applicationId": ...,
    }


# ApplicationSummaryTypeDef definition

class ApplicationSummaryTypeDef(TypedDict):
    applicationId: str,
    applicationName: str,
    domain: str,
    defaultKmsKeyId: NotRequired[str],
```


## ArtifactMetadataItemTypeDef

```python
# ArtifactMetadataItemTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ArtifactMetadataItemTypeDef


def get_value() -> ArtifactMetadataItemTypeDef:
    return {
        "agentSpaceId": ...,
    }


# ArtifactMetadataItemTypeDef definition

class ArtifactMetadataItemTypeDef(TypedDict):
    agentSpaceId: str,
    artifactId: str,
    fileName: str,
    updatedAt: datetime.datetime,
```


## ArtifactSummaryTypeDef

```python
# ArtifactSummaryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ArtifactSummaryTypeDef


def get_value() -> ArtifactSummaryTypeDef:
    return {
        "artifactId": ...,
    }


# ArtifactSummaryTypeDef definition

class ArtifactSummaryTypeDef(TypedDict):
    artifactId: str,
    fileName: str,
    artifactType: ArtifactTypeType,  # (1)
```

1. See [:material-code-brackets: ArtifactTypeType](./literals.md#artifacttypetype)

## ArtifactTypeDef

```python
# ArtifactTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ArtifactTypeDef


def get_value() -> ArtifactTypeDef:
    return {
        "contents": ...,
    }


# ArtifactTypeDef definition

class ArtifactTypeDef(TypedDict):
    contents: str,
    type: ArtifactTypeType,  # (1)
```

1. See [:material-code-brackets: ArtifactTypeType](./literals.md#artifacttypetype)

## DocumentInfoTypeDef

```python
# DocumentInfoTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import DocumentInfoTypeDef


def get_value() -> DocumentInfoTypeDef:
    return {
        "s3Location": ...,
    }


# DocumentInfoTypeDef definition

class DocumentInfoTypeDef(TypedDict):
    s3Location: NotRequired[str],
    artifactId: NotRequired[str],
```


## EndpointTypeDef

```python
# EndpointTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import EndpointTypeDef


def get_value() -> EndpointTypeDef:
    return {
        "uri": ...,
    }


# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    uri: NotRequired[str],
```


## IntegratedRepositoryTypeDef

```python
# IntegratedRepositoryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import IntegratedRepositoryTypeDef


def get_value() -> IntegratedRepositoryTypeDef:
    return {
        "integrationId": ...,
    }


# IntegratedRepositoryTypeDef definition

class IntegratedRepositoryTypeDef(TypedDict):
    integrationId: str,
    providerResourceId: str,
```


## SourceCodeRepositoryTypeDef

```python
# SourceCodeRepositoryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import SourceCodeRepositoryTypeDef


def get_value() -> SourceCodeRepositoryTypeDef:
    return {
        "s3Location": ...,
    }


# SourceCodeRepositoryTypeDef definition

class SourceCodeRepositoryTypeDef(TypedDict):
    s3Location: NotRequired[str],
```


## BatchDeletePentestsInputTypeDef

```python
# BatchDeletePentestsInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchDeletePentestsInputTypeDef


def get_value() -> BatchDeletePentestsInputTypeDef:
    return {
        "pentestIds": ...,
    }


# BatchDeletePentestsInputTypeDef definition

class BatchDeletePentestsInputTypeDef(TypedDict):
    pentestIds: Sequence[str],
    agentSpaceId: str,
```


## DeletePentestFailureTypeDef

```python
# DeletePentestFailureTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import DeletePentestFailureTypeDef


def get_value() -> DeletePentestFailureTypeDef:
    return {
        "pentestId": ...,
    }


# DeletePentestFailureTypeDef definition

class DeletePentestFailureTypeDef(TypedDict):
    pentestId: NotRequired[str],
    reason: NotRequired[str],
```


## BatchGetAgentSpacesInputTypeDef

```python
# BatchGetAgentSpacesInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetAgentSpacesInputTypeDef


def get_value() -> BatchGetAgentSpacesInputTypeDef:
    return {
        "agentSpaceIds": ...,
    }


# BatchGetAgentSpacesInputTypeDef definition

class BatchGetAgentSpacesInputTypeDef(TypedDict):
    agentSpaceIds: Sequence[str],
```


## BatchGetArtifactMetadataInputTypeDef

```python
# BatchGetArtifactMetadataInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetArtifactMetadataInputTypeDef


def get_value() -> BatchGetArtifactMetadataInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# BatchGetArtifactMetadataInputTypeDef definition

class BatchGetArtifactMetadataInputTypeDef(TypedDict):
    agentSpaceId: str,
    artifactIds: Sequence[str],
```


## BatchGetFindingsInputTypeDef

```python
# BatchGetFindingsInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetFindingsInputTypeDef


def get_value() -> BatchGetFindingsInputTypeDef:
    return {
        "findingIds": ...,
    }


# BatchGetFindingsInputTypeDef definition

class BatchGetFindingsInputTypeDef(TypedDict):
    findingIds: Sequence[str],
    agentSpaceId: str,
```


## BatchGetPentestJobTasksInputTypeDef

```python
# BatchGetPentestJobTasksInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetPentestJobTasksInputTypeDef


def get_value() -> BatchGetPentestJobTasksInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# BatchGetPentestJobTasksInputTypeDef definition

class BatchGetPentestJobTasksInputTypeDef(TypedDict):
    agentSpaceId: str,
    taskIds: Sequence[str],
```


## BatchGetPentestJobsInputTypeDef

```python
# BatchGetPentestJobsInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetPentestJobsInputTypeDef


def get_value() -> BatchGetPentestJobsInputTypeDef:
    return {
        "pentestJobIds": ...,
    }


# BatchGetPentestJobsInputTypeDef definition

class BatchGetPentestJobsInputTypeDef(TypedDict):
    pentestJobIds: Sequence[str],
    agentSpaceId: str,
```


## BatchGetPentestsInputTypeDef

```python
# BatchGetPentestsInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetPentestsInputTypeDef


def get_value() -> BatchGetPentestsInputTypeDef:
    return {
        "pentestIds": ...,
    }


# BatchGetPentestsInputTypeDef definition

class BatchGetPentestsInputTypeDef(TypedDict):
    pentestIds: Sequence[str],
    agentSpaceId: str,
```


## BatchGetTargetDomainsInputTypeDef

```python
# BatchGetTargetDomainsInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetTargetDomainsInputTypeDef


def get_value() -> BatchGetTargetDomainsInputTypeDef:
    return {
        "targetDomainIds": ...,
    }


# BatchGetTargetDomainsInputTypeDef definition

class BatchGetTargetDomainsInputTypeDef(TypedDict):
    targetDomainIds: Sequence[str],
```


## CategoryTypeDef

```python
# CategoryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CategoryTypeDef


def get_value() -> CategoryTypeDef:
    return {
        "name": ...,
    }


# CategoryTypeDef definition

class CategoryTypeDef(TypedDict):
    name: NotRequired[str],
    isPrimary: NotRequired[bool],
```


## CloudWatchLogTypeDef

```python
# CloudWatchLogTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CloudWatchLogTypeDef


def get_value() -> CloudWatchLogTypeDef:
    return {
        "logGroup": ...,
    }


# CloudWatchLogTypeDef definition

class CloudWatchLogTypeDef(TypedDict):
    logGroup: NotRequired[str],
    logStream: NotRequired[str],
```


## CodeRemediationTaskDetailsTypeDef

```python
# CodeRemediationTaskDetailsTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CodeRemediationTaskDetailsTypeDef


def get_value() -> CodeRemediationTaskDetailsTypeDef:
    return {
        "repoName": ...,
    }


# CodeRemediationTaskDetailsTypeDef definition

class CodeRemediationTaskDetailsTypeDef(TypedDict):
    repoName: NotRequired[str],
    codeDiffLink: NotRequired[str],
    pullRequestLink: NotRequired[str],
```


## CreateApplicationRequestTypeDef

```python
# CreateApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CreateApplicationRequestTypeDef


def get_value() -> CreateApplicationRequestTypeDef:
    return {
        "idcInstanceArn": ...,
    }


# CreateApplicationRequestTypeDef definition

class CreateApplicationRequestTypeDef(TypedDict):
    idcInstanceArn: NotRequired[str],
    roleArn: NotRequired[str],
    defaultKmsKeyId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```


## CreateTargetDomainInputTypeDef

```python
# CreateTargetDomainInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CreateTargetDomainInputTypeDef


def get_value() -> CreateTargetDomainInputTypeDef:
    return {
        "targetDomainName": ...,
    }


# CreateTargetDomainInputTypeDef definition

class CreateTargetDomainInputTypeDef(TypedDict):
    targetDomainName: str,
    verificationMethod: DomainVerificationMethodType,  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DomainVerificationMethodType](./literals.md#domainverificationmethodtype)

## CustomHeaderTypeDef

```python
# CustomHeaderTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CustomHeaderTypeDef


def get_value() -> CustomHeaderTypeDef:
    return {
        "name": ...,
    }


# CustomHeaderTypeDef definition

class CustomHeaderTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[str],
```


## DeleteAgentSpaceInputTypeDef

```python
# DeleteAgentSpaceInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import DeleteAgentSpaceInputTypeDef


def get_value() -> DeleteAgentSpaceInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# DeleteAgentSpaceInputTypeDef definition

class DeleteAgentSpaceInputTypeDef(TypedDict):
    agentSpaceId: str,
```


## DeleteApplicationRequestTypeDef

```python
# DeleteApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import DeleteApplicationRequestTypeDef


def get_value() -> DeleteApplicationRequestTypeDef:
    return {
        "applicationId": ...,
    }


# DeleteApplicationRequestTypeDef definition

class DeleteApplicationRequestTypeDef(TypedDict):
    applicationId: str,
```


## DeleteArtifactInputTypeDef

```python
# DeleteArtifactInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import DeleteArtifactInputTypeDef


def get_value() -> DeleteArtifactInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# DeleteArtifactInputTypeDef definition

class DeleteArtifactInputTypeDef(TypedDict):
    agentSpaceId: str,
    artifactId: str,
```


## DeleteIntegrationInputTypeDef

```python
# DeleteIntegrationInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import DeleteIntegrationInputTypeDef


def get_value() -> DeleteIntegrationInputTypeDef:
    return {
        "integrationId": ...,
    }


# DeleteIntegrationInputTypeDef definition

class DeleteIntegrationInputTypeDef(TypedDict):
    integrationId: str,
```


## DeleteMembershipRequestTypeDef

```python
# DeleteMembershipRequestTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import DeleteMembershipRequestTypeDef


def get_value() -> DeleteMembershipRequestTypeDef:
    return {
        "applicationId": ...,
    }


# DeleteMembershipRequestTypeDef definition

class DeleteMembershipRequestTypeDef(TypedDict):
    applicationId: str,
    agentSpaceId: str,
    membershipId: str,
    memberType: NotRequired[MembershipTypeType],  # (1)
```

1. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype)

## DeleteTargetDomainInputTypeDef

```python
# DeleteTargetDomainInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import DeleteTargetDomainInputTypeDef


def get_value() -> DeleteTargetDomainInputTypeDef:
    return {
        "targetDomainId": ...,
    }


# DeleteTargetDomainInputTypeDef definition

class DeleteTargetDomainInputTypeDef(TypedDict):
    targetDomainId: str,
```


## DiscoveredEndpointTypeDef

```python
# DiscoveredEndpointTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import DiscoveredEndpointTypeDef


def get_value() -> DiscoveredEndpointTypeDef:
    return {
        "uri": ...,
    }


# DiscoveredEndpointTypeDef definition

class DiscoveredEndpointTypeDef(TypedDict):
    uri: str,
    pentestJobId: str,
    taskId: str,
    agentSpaceId: str,
    evidence: NotRequired[str],
    operation: NotRequired[str],
    description: NotRequired[str],
```


## DnsVerificationTypeDef

```python
# DnsVerificationTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import DnsVerificationTypeDef


def get_value() -> DnsVerificationTypeDef:
    return {
        "token": ...,
    }


# DnsVerificationTypeDef definition

class DnsVerificationTypeDef(TypedDict):
    token: NotRequired[str],
    dnsRecordName: NotRequired[str],
    dnsRecordType: NotRequired[DNSRecordTypeType],  # (1)
```

1. See [:material-code-brackets: DNSRecordTypeType](./literals.md#dnsrecordtypetype)

## ErrorInformationTypeDef

```python
# ErrorInformationTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ErrorInformationTypeDef


def get_value() -> ErrorInformationTypeDef:
    return {
        "code": ...,
    }


# ErrorInformationTypeDef definition

class ErrorInformationTypeDef(TypedDict):
    code: NotRequired[ErrorCodeType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype)

## ExecutionContextTypeDef

```python
# ExecutionContextTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ExecutionContextTypeDef


def get_value() -> ExecutionContextTypeDef:
    return {
        "contextType": ...,
    }


# ExecutionContextTypeDef definition

class ExecutionContextTypeDef(TypedDict):
    contextType: NotRequired[ContextTypeType],  # (1)
    context: NotRequired[str],
    timestamp: NotRequired[datetime.datetime],
```

1. See [:material-code-brackets: ContextTypeType](./literals.md#contexttypetype)

## FindingSummaryTypeDef

```python
# FindingSummaryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import FindingSummaryTypeDef


def get_value() -> FindingSummaryTypeDef:
    return {
        "findingId": ...,
    }


# FindingSummaryTypeDef definition

class FindingSummaryTypeDef(TypedDict):
    findingId: str,
    agentSpaceId: str,
    pentestId: NotRequired[str],
    pentestJobId: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[FindingStatusType],  # (1)
    riskType: NotRequired[str],
    riskLevel: NotRequired[RiskLevelType],  # (2)
    confidence: NotRequired[ConfidenceLevelType],  # (3)
    createdAt: NotRequired[datetime.datetime],
    updatedAt: NotRequired[datetime.datetime],
```

1. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype)
2. See [:material-code-brackets: RiskLevelType](./literals.md#riskleveltype)
3. See [:material-code-brackets: ConfidenceLevelType](./literals.md#confidenceleveltype)

## GetApplicationRequestTypeDef

```python
# GetApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import GetApplicationRequestTypeDef


def get_value() -> GetApplicationRequestTypeDef:
    return {
        "applicationId": ...,
    }


# GetApplicationRequestTypeDef definition

class GetApplicationRequestTypeDef(TypedDict):
    applicationId: str,
```


## IdCConfigurationTypeDef

```python
# IdCConfigurationTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import IdCConfigurationTypeDef


def get_value() -> IdCConfigurationTypeDef:
    return {
        "idcApplicationArn": ...,
    }


# IdCConfigurationTypeDef definition

class IdCConfigurationTypeDef(TypedDict):
    idcApplicationArn: NotRequired[str],
    idcInstanceArn: NotRequired[str],
```


## GetArtifactInputTypeDef

```python
# GetArtifactInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import GetArtifactInputTypeDef


def get_value() -> GetArtifactInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# GetArtifactInputTypeDef definition

class GetArtifactInputTypeDef(TypedDict):
    agentSpaceId: str,
    artifactId: str,
```


## GetIntegrationInputTypeDef

```python
# GetIntegrationInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import GetIntegrationInputTypeDef


def get_value() -> GetIntegrationInputTypeDef:
    return {
        "integrationId": ...,
    }


# GetIntegrationInputTypeDef definition

class GetIntegrationInputTypeDef(TypedDict):
    integrationId: str,
```


## GitHubIntegrationInputTypeDef

```python
# GitHubIntegrationInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import GitHubIntegrationInputTypeDef


def get_value() -> GitHubIntegrationInputTypeDef:
    return {
        "code": ...,
    }


# GitHubIntegrationInputTypeDef definition

class GitHubIntegrationInputTypeDef(TypedDict):
    code: str,
    state: str,
    organizationName: NotRequired[str],
```


## GitHubRepositoryMetadataTypeDef

```python
# GitHubRepositoryMetadataTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import GitHubRepositoryMetadataTypeDef


def get_value() -> GitHubRepositoryMetadataTypeDef:
    return {
        "name": ...,
    }


# GitHubRepositoryMetadataTypeDef definition

class GitHubRepositoryMetadataTypeDef(TypedDict):
    name: str,
    providerResourceId: str,
    owner: str,
    accessType: NotRequired[AccessTypeType],  # (1)
```

1. See [:material-code-brackets: AccessTypeType](./literals.md#accesstypetype)

## GitHubRepositoryResourceTypeDef

```python
# GitHubRepositoryResourceTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import GitHubRepositoryResourceTypeDef


def get_value() -> GitHubRepositoryResourceTypeDef:
    return {
        "name": ...,
    }


# GitHubRepositoryResourceTypeDef definition

class GitHubRepositoryResourceTypeDef(TypedDict):
    name: str,
    owner: str,
```


## GitHubResourceCapabilitiesTypeDef

```python
# GitHubResourceCapabilitiesTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import GitHubResourceCapabilitiesTypeDef


def get_value() -> GitHubResourceCapabilitiesTypeDef:
    return {
        "leaveComments": ...,
    }


# GitHubResourceCapabilitiesTypeDef definition

class GitHubResourceCapabilitiesTypeDef(TypedDict):
    leaveComments: NotRequired[bool],
    remediateCode: NotRequired[bool],
```


## HttpVerificationTypeDef

```python
# HttpVerificationTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import HttpVerificationTypeDef


def get_value() -> HttpVerificationTypeDef:
    return {
        "token": ...,
    }


# HttpVerificationTypeDef definition

class HttpVerificationTypeDef(TypedDict):
    token: NotRequired[str],
    routePath: NotRequired[str],
```


## InitiateProviderRegistrationInputTypeDef

```python
# InitiateProviderRegistrationInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import InitiateProviderRegistrationInputTypeDef


def get_value() -> InitiateProviderRegistrationInputTypeDef:
    return {
        "provider": ...,
    }


# InitiateProviderRegistrationInputTypeDef definition

class InitiateProviderRegistrationInputTypeDef(TypedDict):
    provider: ProviderType,  # (1)
```

1. See [:material-code-brackets: ProviderType](./literals.md#providertype)

## IntegrationFilterTypeDef

```python
# IntegrationFilterTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import IntegrationFilterTypeDef


def get_value() -> IntegrationFilterTypeDef:
    return {
        "provider": ...,
    }


# IntegrationFilterTypeDef definition

class IntegrationFilterTypeDef(TypedDict):
    provider: NotRequired[ProviderType],  # (1)
    providerType: NotRequired[ProviderTypeType],  # (2)
```

1. See [:material-code-brackets: ProviderType](./literals.md#providertype)
2. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype)

## IntegrationSummaryTypeDef

```python
# IntegrationSummaryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import IntegrationSummaryTypeDef


def get_value() -> IntegrationSummaryTypeDef:
    return {
        "integrationId": ...,
    }


# IntegrationSummaryTypeDef definition

class IntegrationSummaryTypeDef(TypedDict):
    integrationId: str,
    installationId: str,
    provider: ProviderType,  # (1)
    providerType: ProviderTypeType,  # (2)
    displayName: str,
```

1. See [:material-code-brackets: ProviderType](./literals.md#providertype)
2. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype)

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```


## ListAgentSpacesInputTypeDef

```python
# ListAgentSpacesInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListAgentSpacesInputTypeDef


def get_value() -> ListAgentSpacesInputTypeDef:
    return {
        "nextToken": ...,
    }


# ListAgentSpacesInputTypeDef definition

class ListAgentSpacesInputTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```


## ListApplicationsRequestTypeDef

```python
# ListApplicationsRequestTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListApplicationsRequestTypeDef


def get_value() -> ListApplicationsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListApplicationsRequestTypeDef definition

class ListApplicationsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```


## ListArtifactsInputTypeDef

```python
# ListArtifactsInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListArtifactsInputTypeDef


def get_value() -> ListArtifactsInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# ListArtifactsInputTypeDef definition

class ListArtifactsInputTypeDef(TypedDict):
    agentSpaceId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```


## ListDiscoveredEndpointsInputTypeDef

```python
# ListDiscoveredEndpointsInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListDiscoveredEndpointsInputTypeDef


def get_value() -> ListDiscoveredEndpointsInputTypeDef:
    return {
        "pentestJobId": ...,
    }


# ListDiscoveredEndpointsInputTypeDef definition

class ListDiscoveredEndpointsInputTypeDef(TypedDict):
    pentestJobId: str,
    agentSpaceId: str,
    maxResults: NotRequired[int],
    prefix: NotRequired[str],
    nextToken: NotRequired[str],
```


## ListFindingsInputTypeDef

```python
# ListFindingsInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListFindingsInputTypeDef


def get_value() -> ListFindingsInputTypeDef:
    return {
        "pentestJobId": ...,
    }


# ListFindingsInputTypeDef definition

class ListFindingsInputTypeDef(TypedDict):
    pentestJobId: str,
    agentSpaceId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    riskType: NotRequired[str],
    riskLevel: NotRequired[RiskLevelType],  # (1)
    status: NotRequired[FindingStatusType],  # (2)
    confidence: NotRequired[ConfidenceLevelType],  # (3)
    name: NotRequired[str],
```

1. See [:material-code-brackets: RiskLevelType](./literals.md#riskleveltype)
2. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype)
3. See [:material-code-brackets: ConfidenceLevelType](./literals.md#confidenceleveltype)

## ListIntegratedResourcesInputTypeDef

```python
# ListIntegratedResourcesInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListIntegratedResourcesInputTypeDef


def get_value() -> ListIntegratedResourcesInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# ListIntegratedResourcesInputTypeDef definition

class ListIntegratedResourcesInputTypeDef(TypedDict):
    agentSpaceId: str,
    integrationId: NotRequired[str],
    resourceType: NotRequired[ResourceTypeType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype)

## ListMembershipsRequestTypeDef

```python
# ListMembershipsRequestTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListMembershipsRequestTypeDef


def get_value() -> ListMembershipsRequestTypeDef:
    return {
        "applicationId": ...,
    }


# ListMembershipsRequestTypeDef definition

class ListMembershipsRequestTypeDef(TypedDict):
    applicationId: str,
    agentSpaceId: str,
    memberType: NotRequired[MembershipTypeFilterType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: MembershipTypeFilterType](./literals.md#membershiptypefiltertype)

## ListPentestJobTasksInputTypeDef

```python
# ListPentestJobTasksInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListPentestJobTasksInputTypeDef


def get_value() -> ListPentestJobTasksInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# ListPentestJobTasksInputTypeDef definition

class ListPentestJobTasksInputTypeDef(TypedDict):
    agentSpaceId: str,
    maxResults: NotRequired[int],
    pentestJobId: NotRequired[str],
    stepName: NotRequired[StepNameType],  # (1)
    categoryName: NotRequired[str],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: StepNameType](./literals.md#stepnametype)

## TaskSummaryTypeDef

```python
# TaskSummaryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import TaskSummaryTypeDef


def get_value() -> TaskSummaryTypeDef:
    return {
        "taskId": ...,
    }


# TaskSummaryTypeDef definition

class TaskSummaryTypeDef(TypedDict):
    taskId: str,
    pentestId: NotRequired[str],
    pentestJobId: NotRequired[str],
    agentSpaceId: NotRequired[str],
    title: NotRequired[str],
    riskType: NotRequired[RiskTypeType],  # (1)
    executionStatus: NotRequired[TaskExecutionStatusType],  # (2)
    createdAt: NotRequired[datetime.datetime],
    updatedAt: NotRequired[datetime.datetime],
```

1. See [:material-code-brackets: RiskTypeType](./literals.md#risktypetype)
2. See [:material-code-brackets: TaskExecutionStatusType](./literals.md#taskexecutionstatustype)

## ListPentestJobsForPentestInputTypeDef

```python
# ListPentestJobsForPentestInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListPentestJobsForPentestInputTypeDef


def get_value() -> ListPentestJobsForPentestInputTypeDef:
    return {
        "pentestId": ...,
    }


# ListPentestJobsForPentestInputTypeDef definition

class ListPentestJobsForPentestInputTypeDef(TypedDict):
    pentestId: str,
    agentSpaceId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## PentestJobSummaryTypeDef

```python
# PentestJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import PentestJobSummaryTypeDef


def get_value() -> PentestJobSummaryTypeDef:
    return {
        "pentestJobId": ...,
    }


# PentestJobSummaryTypeDef definition

class PentestJobSummaryTypeDef(TypedDict):
    pentestJobId: str,
    pentestId: str,
    title: NotRequired[str],
    status: NotRequired[JobStatusType],  # (1)
    createdAt: NotRequired[datetime.datetime],
    updatedAt: NotRequired[datetime.datetime],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype)

## ListPentestsInputTypeDef

```python
# ListPentestsInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListPentestsInputTypeDef


def get_value() -> ListPentestsInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# ListPentestsInputTypeDef definition

class ListPentestsInputTypeDef(TypedDict):
    agentSpaceId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## PentestSummaryTypeDef

```python
# PentestSummaryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import PentestSummaryTypeDef


def get_value() -> PentestSummaryTypeDef:
    return {
        "pentestId": ...,
    }


# PentestSummaryTypeDef definition

class PentestSummaryTypeDef(TypedDict):
    pentestId: str,
    agentSpaceId: str,
    title: str,
    createdAt: NotRequired[datetime.datetime],
    updatedAt: NotRequired[datetime.datetime],
```


## ListTagsForResourceInputTypeDef

```python
# ListTagsForResourceInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListTagsForResourceInputTypeDef


def get_value() -> ListTagsForResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceInputTypeDef definition

class ListTagsForResourceInputTypeDef(TypedDict):
    resourceArn: str,
```


## ListTargetDomainsInputTypeDef

```python
# ListTargetDomainsInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListTargetDomainsInputTypeDef


def get_value() -> ListTargetDomainsInputTypeDef:
    return {
        "nextToken": ...,
    }


# ListTargetDomainsInputTypeDef definition

class ListTargetDomainsInputTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```


## TargetDomainSummaryTypeDef

```python
# TargetDomainSummaryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import TargetDomainSummaryTypeDef


def get_value() -> TargetDomainSummaryTypeDef:
    return {
        "targetDomainId": ...,
    }


# TargetDomainSummaryTypeDef definition

class TargetDomainSummaryTypeDef(TypedDict):
    targetDomainId: str,
    domainName: str,
    verificationStatus: NotRequired[TargetDomainStatusType],  # (1)
```

1. See [:material-code-brackets: TargetDomainStatusType](./literals.md#targetdomainstatustype)

## UserMetadataTypeDef

```python
# UserMetadataTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import UserMetadataTypeDef


def get_value() -> UserMetadataTypeDef:
    return {
        "username": ...,
    }


# UserMetadataTypeDef definition

class UserMetadataTypeDef(TypedDict):
    username: str,
    email: str,
```


## UserConfigTypeDef

```python
# UserConfigTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import UserConfigTypeDef


def get_value() -> UserConfigTypeDef:
    return {
        "role": ...,
    }


# UserConfigTypeDef definition

class UserConfigTypeDef(TypedDict):
    role: NotRequired[UserRoleType],  # (1)
```

1. See [:material-code-brackets: UserRoleType](./literals.md#userroletype)

## NetworkTrafficRuleTypeDef

```python
# NetworkTrafficRuleTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import NetworkTrafficRuleTypeDef


def get_value() -> NetworkTrafficRuleTypeDef:
    return {
        "effect": ...,
    }


# NetworkTrafficRuleTypeDef definition

class NetworkTrafficRuleTypeDef(TypedDict):
    effect: NotRequired[NetworkTrafficRuleEffectType],  # (1)
    pattern: NotRequired[str],
    networkTrafficRuleType: NotRequired[NetworkTrafficRuleTypeType],  # (2)
```

1. See [:material-code-brackets: NetworkTrafficRuleEffectType](./literals.md#networktrafficruleeffecttype)
2. See [:material-code-brackets: NetworkTrafficRuleTypeType](./literals.md#networktrafficruletypetype)

## StepTypeDef

```python
# StepTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import StepTypeDef


def get_value() -> StepTypeDef:
    return {
        "name": ...,
    }


# StepTypeDef definition

class StepTypeDef(TypedDict):
    name: NotRequired[StepNameType],  # (1)
    status: NotRequired[StepStatusType],  # (2)
    createdAt: NotRequired[datetime.datetime],
    updatedAt: NotRequired[datetime.datetime],
```

1. See [:material-code-brackets: StepNameType](./literals.md#stepnametype)
2. See [:material-code-brackets: StepStatusType](./literals.md#stepstatustype)

## StartCodeRemediationInputTypeDef

```python
# StartCodeRemediationInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import StartCodeRemediationInputTypeDef


def get_value() -> StartCodeRemediationInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# StartCodeRemediationInputTypeDef definition

class StartCodeRemediationInputTypeDef(TypedDict):
    agentSpaceId: str,
    pentestJobId: str,
    findingIds: Sequence[str],
```


## StartPentestJobInputTypeDef

```python
# StartPentestJobInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import StartPentestJobInputTypeDef


def get_value() -> StartPentestJobInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# StartPentestJobInputTypeDef definition

class StartPentestJobInputTypeDef(TypedDict):
    agentSpaceId: str,
    pentestId: str,
```


## StopPentestJobInputTypeDef

```python
# StopPentestJobInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import StopPentestJobInputTypeDef


def get_value() -> StopPentestJobInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# StopPentestJobInputTypeDef definition

class StopPentestJobInputTypeDef(TypedDict):
    agentSpaceId: str,
    pentestJobId: str,
```


## TagResourceInputTypeDef

```python
# TagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import TagResourceInputTypeDef


def get_value() -> TagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceInputTypeDef definition

class TagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```


## UntagResourceInputTypeDef

```python
# UntagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import UntagResourceInputTypeDef


def get_value() -> UntagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceInputTypeDef definition

class UntagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```


## UpdateApplicationRequestTypeDef

```python
# UpdateApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import UpdateApplicationRequestTypeDef


def get_value() -> UpdateApplicationRequestTypeDef:
    return {
        "applicationId": ...,
    }


# UpdateApplicationRequestTypeDef definition

class UpdateApplicationRequestTypeDef(TypedDict):
    applicationId: str,
    roleArn: NotRequired[str],
    defaultKmsKeyId: NotRequired[str],
```


## UpdateFindingInputTypeDef

```python
# UpdateFindingInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import UpdateFindingInputTypeDef


def get_value() -> UpdateFindingInputTypeDef:
    return {
        "findingId": ...,
    }


# UpdateFindingInputTypeDef definition

class UpdateFindingInputTypeDef(TypedDict):
    findingId: str,
    agentSpaceId: str,
    riskLevel: NotRequired[RiskLevelType],  # (1)
    status: NotRequired[FindingStatusType],  # (2)
```

1. See [:material-code-brackets: RiskLevelType](./literals.md#riskleveltype)
2. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype)

## UpdateTargetDomainInputTypeDef

```python
# UpdateTargetDomainInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import UpdateTargetDomainInputTypeDef


def get_value() -> UpdateTargetDomainInputTypeDef:
    return {
        "targetDomainId": ...,
    }


# UpdateTargetDomainInputTypeDef definition

class UpdateTargetDomainInputTypeDef(TypedDict):
    targetDomainId: str,
    verificationMethod: DomainVerificationMethodType,  # (1)
```

1. See [:material-code-brackets: DomainVerificationMethodType](./literals.md#domainverificationmethodtype)

## VerifyTargetDomainInputTypeDef

```python
# VerifyTargetDomainInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import VerifyTargetDomainInputTypeDef


def get_value() -> VerifyTargetDomainInputTypeDef:
    return {
        "targetDomainId": ...,
    }


# VerifyTargetDomainInputTypeDef definition

class VerifyTargetDomainInputTypeDef(TypedDict):
    targetDomainId: str,
```


## AWSResourcesOutputTypeDef

```python
# AWSResourcesOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import AWSResourcesOutputTypeDef


def get_value() -> AWSResourcesOutputTypeDef:
    return {
        "vpcs": ...,
    }


# AWSResourcesOutputTypeDef definition

class AWSResourcesOutputTypeDef(TypedDict):
    vpcs: NotRequired[list[VpcConfigOutputTypeDef]],  # (1)
    logGroups: NotRequired[list[str]],
    s3Buckets: NotRequired[list[str]],
    secretArns: NotRequired[list[str]],
    lambdaFunctionArns: NotRequired[list[str]],
    iamRoles: NotRequired[list[str]],
```

1. See `list[VpcConfigOutputTypeDef]`

## AWSResourcesTypeDef

```python
# AWSResourcesTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import AWSResourcesTypeDef


def get_value() -> AWSResourcesTypeDef:
    return {
        "vpcs": ...,
    }


# AWSResourcesTypeDef definition

class AWSResourcesTypeDef(TypedDict):
    vpcs: NotRequired[Sequence[VpcConfigTypeDef]],  # (1)
    logGroups: NotRequired[Sequence[str]],
    s3Buckets: NotRequired[Sequence[str]],
    secretArns: NotRequired[Sequence[str]],
    lambdaFunctionArns: NotRequired[Sequence[str]],
    iamRoles: NotRequired[Sequence[str]],
```

1. See `Sequence[VpcConfigTypeDef]`

## ActorOutputTypeDef

```python
# ActorOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ActorOutputTypeDef


def get_value() -> ActorOutputTypeDef:
    return {
        "identifier": ...,
    }


# ActorOutputTypeDef definition

class ActorOutputTypeDef(TypedDict):
    identifier: NotRequired[str],
    uris: NotRequired[list[str]],
    authentication: NotRequired[AuthenticationTypeDef],  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: AuthenticationTypeDef](./type_defs.md#authenticationtypedef)

## ActorTypeDef

```python
# ActorTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ActorTypeDef


def get_value() -> ActorTypeDef:
    return {
        "identifier": ...,
    }


# ActorTypeDef definition

class ActorTypeDef(TypedDict):
    identifier: NotRequired[str],
    uris: NotRequired[Sequence[str]],
    authentication: NotRequired[AuthenticationTypeDef],  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: AuthenticationTypeDef](./type_defs.md#authenticationtypedef)

## AddArtifactInputTypeDef

```python
# AddArtifactInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import AddArtifactInputTypeDef


def get_value() -> AddArtifactInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# AddArtifactInputTypeDef definition

class AddArtifactInputTypeDef(TypedDict):
    agentSpaceId: str,
    artifactContent: BlobTypeDef,
    artifactType: ArtifactTypeType,  # (1)
    fileName: str,
```

1. See [:material-code-brackets: ArtifactTypeType](./literals.md#artifacttypetype)

## AddArtifactOutputTypeDef

```python
# AddArtifactOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import AddArtifactOutputTypeDef


def get_value() -> AddArtifactOutputTypeDef:
    return {
        "artifactId": ...,
    }


# AddArtifactOutputTypeDef definition

class AddArtifactOutputTypeDef(TypedDict):
    artifactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateApplicationResponseTypeDef

```python
# CreateApplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CreateApplicationResponseTypeDef


def get_value() -> CreateApplicationResponseTypeDef:
    return {
        "applicationId": ...,
    }


# CreateApplicationResponseTypeDef definition

class CreateApplicationResponseTypeDef(TypedDict):
    applicationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateIntegrationOutputTypeDef

```python
# CreateIntegrationOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CreateIntegrationOutputTypeDef


def get_value() -> CreateIntegrationOutputTypeDef:
    return {
        "integrationId": ...,
    }


# CreateIntegrationOutputTypeDef definition

class CreateIntegrationOutputTypeDef(TypedDict):
    integrationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteAgentSpaceOutputTypeDef

```python
# DeleteAgentSpaceOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import DeleteAgentSpaceOutputTypeDef


def get_value() -> DeleteAgentSpaceOutputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# DeleteAgentSpaceOutputTypeDef definition

class DeleteAgentSpaceOutputTypeDef(TypedDict):
    agentSpaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteTargetDomainOutputTypeDef

```python
# DeleteTargetDomainOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import DeleteTargetDomainOutputTypeDef


def get_value() -> DeleteTargetDomainOutputTypeDef:
    return {
        "targetDomainId": ...,
    }


# DeleteTargetDomainOutputTypeDef definition

class DeleteTargetDomainOutputTypeDef(TypedDict):
    targetDomainId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetIntegrationOutputTypeDef

```python
# GetIntegrationOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import GetIntegrationOutputTypeDef


def get_value() -> GetIntegrationOutputTypeDef:
    return {
        "integrationId": ...,
    }


# GetIntegrationOutputTypeDef definition

class GetIntegrationOutputTypeDef(TypedDict):
    integrationId: str,
    installationId: str,
    provider: ProviderType,  # (1)
    providerType: ProviderTypeType,  # (2)
    displayName: str,
    kmsKeyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ProviderType](./literals.md#providertype)
2. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## InitiateProviderRegistrationOutputTypeDef

```python
# InitiateProviderRegistrationOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import InitiateProviderRegistrationOutputTypeDef


def get_value() -> InitiateProviderRegistrationOutputTypeDef:
    return {
        "redirectTo": ...,
    }


# InitiateProviderRegistrationOutputTypeDef definition

class InitiateProviderRegistrationOutputTypeDef(TypedDict):
    redirectTo: str,
    csrfState: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListTagsForResourceOutputTypeDef


def get_value() -> ListTagsForResourceOutputTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StartPentestJobOutputTypeDef

```python
# StartPentestJobOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import StartPentestJobOutputTypeDef


def get_value() -> StartPentestJobOutputTypeDef:
    return {
        "title": ...,
    }


# StartPentestJobOutputTypeDef definition

class StartPentestJobOutputTypeDef(TypedDict):
    title: str,
    status: JobStatusType,  # (1)
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    pentestId: str,
    pentestJobId: str,
    agentSpaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateApplicationResponseTypeDef

```python
# UpdateApplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import UpdateApplicationResponseTypeDef


def get_value() -> UpdateApplicationResponseTypeDef:
    return {
        "applicationId": ...,
    }


# UpdateApplicationResponseTypeDef definition

class UpdateApplicationResponseTypeDef(TypedDict):
    applicationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## VerifyTargetDomainOutputTypeDef

```python
# VerifyTargetDomainOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import VerifyTargetDomainOutputTypeDef


def get_value() -> VerifyTargetDomainOutputTypeDef:
    return {
        "targetDomainId": ...,
    }


# VerifyTargetDomainOutputTypeDef definition

class VerifyTargetDomainOutputTypeDef(TypedDict):
    targetDomainId: str,
    domainName: str,
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    verifiedAt: datetime.datetime,
    status: TargetDomainStatusType,  # (1)
    verificationStatusReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TargetDomainStatusType](./literals.md#targetdomainstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListAgentSpacesOutputTypeDef

```python
# ListAgentSpacesOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListAgentSpacesOutputTypeDef


def get_value() -> ListAgentSpacesOutputTypeDef:
    return {
        "agentSpaceSummaries": ...,
    }


# ListAgentSpacesOutputTypeDef definition

class ListAgentSpacesOutputTypeDef(TypedDict):
    agentSpaceSummaries: list[AgentSpaceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[AgentSpaceSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListApplicationsResponseTypeDef

```python
# ListApplicationsResponseTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListApplicationsResponseTypeDef


def get_value() -> ListApplicationsResponseTypeDef:
    return {
        "applicationSummaries": ...,
    }


# ListApplicationsResponseTypeDef definition

class ListApplicationsResponseTypeDef(TypedDict):
    applicationSummaries: list[ApplicationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ApplicationSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## BatchGetArtifactMetadataOutputTypeDef

```python
# BatchGetArtifactMetadataOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetArtifactMetadataOutputTypeDef


def get_value() -> BatchGetArtifactMetadataOutputTypeDef:
    return {
        "artifactMetadataList": ...,
    }


# BatchGetArtifactMetadataOutputTypeDef definition

class BatchGetArtifactMetadataOutputTypeDef(TypedDict):
    artifactMetadataList: list[ArtifactMetadataItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `list[ArtifactMetadataItemTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListArtifactsOutputTypeDef

```python
# ListArtifactsOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListArtifactsOutputTypeDef


def get_value() -> ListArtifactsOutputTypeDef:
    return {
        "artifactSummaries": ...,
    }


# ListArtifactsOutputTypeDef definition

class ListArtifactsOutputTypeDef(TypedDict):
    artifactSummaries: list[ArtifactSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ArtifactSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetArtifactOutputTypeDef

```python
# GetArtifactOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import GetArtifactOutputTypeDef


def get_value() -> GetArtifactOutputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# GetArtifactOutputTypeDef definition

class GetArtifactOutputTypeDef(TypedDict):
    agentSpaceId: str,
    artifactId: str,
    artifact: ArtifactTypeDef,  # (1)
    fileName: str,
    updatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ArtifactTypeDef](./type_defs.md#artifacttypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## LogLocationTypeDef

```python
# LogLocationTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import LogLocationTypeDef


def get_value() -> LogLocationTypeDef:
    return {
        "logType": ...,
    }


# LogLocationTypeDef definition

class LogLocationTypeDef(TypedDict):
    logType: NotRequired[LogTypeType],  # (1)
    cloudWatchLog: NotRequired[CloudWatchLogTypeDef],  # (2)
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype)
2. See [:material-code-braces: CloudWatchLogTypeDef](./type_defs.md#cloudwatchlogtypedef)

## CodeRemediationTaskTypeDef

```python
# CodeRemediationTaskTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CodeRemediationTaskTypeDef


def get_value() -> CodeRemediationTaskTypeDef:
    return {
        "status": ...,
    }


# CodeRemediationTaskTypeDef definition

class CodeRemediationTaskTypeDef(TypedDict):
    status: CodeRemediationTaskStatusType,  # (1)
    statusReason: NotRequired[str],
    taskDetails: NotRequired[list[CodeRemediationTaskDetailsTypeDef]],  # (2)
```

1. See [:material-code-brackets: CodeRemediationTaskStatusType](./literals.md#coderemediationtaskstatustype)
2. See `list[CodeRemediationTaskDetailsTypeDef]`

## ListDiscoveredEndpointsOutputTypeDef

```python
# ListDiscoveredEndpointsOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListDiscoveredEndpointsOutputTypeDef


def get_value() -> ListDiscoveredEndpointsOutputTypeDef:
    return {
        "discoveredEndpoints": ...,
    }


# ListDiscoveredEndpointsOutputTypeDef definition

class ListDiscoveredEndpointsOutputTypeDef(TypedDict):
    discoveredEndpoints: list[DiscoveredEndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[DiscoveredEndpointTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListFindingsOutputTypeDef

```python
# ListFindingsOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListFindingsOutputTypeDef


def get_value() -> ListFindingsOutputTypeDef:
    return {
        "findingsSummaries": ...,
    }


# ListFindingsOutputTypeDef definition

class ListFindingsOutputTypeDef(TypedDict):
    findingsSummaries: list[FindingSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[FindingSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetApplicationResponseTypeDef

```python
# GetApplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import GetApplicationResponseTypeDef


def get_value() -> GetApplicationResponseTypeDef:
    return {
        "applicationId": ...,
    }


# GetApplicationResponseTypeDef definition

class GetApplicationResponseTypeDef(TypedDict):
    applicationId: str,
    domain: str,
    applicationName: str,
    idcConfiguration: IdCConfigurationTypeDef,  # (1)
    roleArn: str,
    defaultKmsKeyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdCConfigurationTypeDef](./type_defs.md#idcconfigurationtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ProviderInputTypeDef

```python
# ProviderInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ProviderInputTypeDef


def get_value() -> ProviderInputTypeDef:
    return {
        "github": ...,
    }


# ProviderInputTypeDef definition

class ProviderInputTypeDef(TypedDict):
    github: NotRequired[GitHubIntegrationInputTypeDef],  # (1)
```

1. See [:material-code-braces: GitHubIntegrationInputTypeDef](./type_defs.md#githubintegrationinputtypedef)

## IntegratedResourceMetadataTypeDef

```python
# IntegratedResourceMetadataTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import IntegratedResourceMetadataTypeDef


def get_value() -> IntegratedResourceMetadataTypeDef:
    return {
        "githubRepository": ...,
    }


# IntegratedResourceMetadataTypeDef definition

class IntegratedResourceMetadataTypeDef(TypedDict):
    githubRepository: NotRequired[GitHubRepositoryMetadataTypeDef],  # (1)
```

1. See [:material-code-braces: GitHubRepositoryMetadataTypeDef](./type_defs.md#githubrepositorymetadatatypedef)

## IntegratedResourceTypeDef

```python
# IntegratedResourceTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import IntegratedResourceTypeDef


def get_value() -> IntegratedResourceTypeDef:
    return {
        "githubRepository": ...,
    }


# IntegratedResourceTypeDef definition

class IntegratedResourceTypeDef(TypedDict):
    githubRepository: NotRequired[GitHubRepositoryResourceTypeDef],  # (1)
```

1. See [:material-code-braces: GitHubRepositoryResourceTypeDef](./type_defs.md#githubrepositoryresourcetypedef)

## ProviderResourceCapabilitiesTypeDef

```python
# ProviderResourceCapabilitiesTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ProviderResourceCapabilitiesTypeDef


def get_value() -> ProviderResourceCapabilitiesTypeDef:
    return {
        "github": ...,
    }


# ProviderResourceCapabilitiesTypeDef definition

class ProviderResourceCapabilitiesTypeDef(TypedDict):
    github: NotRequired[GitHubResourceCapabilitiesTypeDef],  # (1)
```

1. See [:material-code-braces: GitHubResourceCapabilitiesTypeDef](./type_defs.md#githubresourcecapabilitiestypedef)

## VerificationDetailsTypeDef

```python
# VerificationDetailsTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import VerificationDetailsTypeDef


def get_value() -> VerificationDetailsTypeDef:
    return {
        "method": ...,
    }


# VerificationDetailsTypeDef definition

class VerificationDetailsTypeDef(TypedDict):
    method: NotRequired[DomainVerificationMethodType],  # (1)
    dnsTxt: NotRequired[DnsVerificationTypeDef],  # (2)
    httpRoute: NotRequired[HttpVerificationTypeDef],  # (3)
```

1. See [:material-code-brackets: DomainVerificationMethodType](./literals.md#domainverificationmethodtype)
2. See [:material-code-braces: DnsVerificationTypeDef](./type_defs.md#dnsverificationtypedef)
3. See [:material-code-braces: HttpVerificationTypeDef](./type_defs.md#httpverificationtypedef)

## ListIntegrationsInputTypeDef

```python
# ListIntegrationsInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListIntegrationsInputTypeDef


def get_value() -> ListIntegrationsInputTypeDef:
    return {
        "filter": ...,
    }


# ListIntegrationsInputTypeDef definition

class ListIntegrationsInputTypeDef(TypedDict):
    filter: NotRequired[IntegrationFilterTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: IntegrationFilterTypeDef](./type_defs.md#integrationfiltertypedef)

## ListIntegrationsOutputTypeDef

```python
# ListIntegrationsOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListIntegrationsOutputTypeDef


def get_value() -> ListIntegrationsOutputTypeDef:
    return {
        "integrationSummaries": ...,
    }


# ListIntegrationsOutputTypeDef definition

class ListIntegrationsOutputTypeDef(TypedDict):
    integrationSummaries: list[IntegrationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[IntegrationSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListAgentSpacesInputPaginateTypeDef

```python
# ListAgentSpacesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListAgentSpacesInputPaginateTypeDef


def get_value() -> ListAgentSpacesInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListAgentSpacesInputPaginateTypeDef definition

class ListAgentSpacesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListApplicationsRequestPaginateTypeDef

```python
# ListApplicationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListApplicationsRequestPaginateTypeDef


def get_value() -> ListApplicationsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListApplicationsRequestPaginateTypeDef definition

class ListApplicationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListArtifactsInputPaginateTypeDef

```python
# ListArtifactsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListArtifactsInputPaginateTypeDef


def get_value() -> ListArtifactsInputPaginateTypeDef:
    return {
        "agentSpaceId": ...,
    }


# ListArtifactsInputPaginateTypeDef definition

class ListArtifactsInputPaginateTypeDef(TypedDict):
    agentSpaceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListDiscoveredEndpointsInputPaginateTypeDef

```python
# ListDiscoveredEndpointsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListDiscoveredEndpointsInputPaginateTypeDef


def get_value() -> ListDiscoveredEndpointsInputPaginateTypeDef:
    return {
        "pentestJobId": ...,
    }


# ListDiscoveredEndpointsInputPaginateTypeDef definition

class ListDiscoveredEndpointsInputPaginateTypeDef(TypedDict):
    pentestJobId: str,
    agentSpaceId: str,
    prefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListFindingsInputPaginateTypeDef

```python
# ListFindingsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListFindingsInputPaginateTypeDef


def get_value() -> ListFindingsInputPaginateTypeDef:
    return {
        "pentestJobId": ...,
    }


# ListFindingsInputPaginateTypeDef definition

class ListFindingsInputPaginateTypeDef(TypedDict):
    pentestJobId: str,
    agentSpaceId: str,
    riskType: NotRequired[str],
    riskLevel: NotRequired[RiskLevelType],  # (1)
    status: NotRequired[FindingStatusType],  # (2)
    confidence: NotRequired[ConfidenceLevelType],  # (3)
    name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: RiskLevelType](./literals.md#riskleveltype)
2. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype)
3. See [:material-code-brackets: ConfidenceLevelType](./literals.md#confidenceleveltype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListIntegratedResourcesInputPaginateTypeDef

```python
# ListIntegratedResourcesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListIntegratedResourcesInputPaginateTypeDef


def get_value() -> ListIntegratedResourcesInputPaginateTypeDef:
    return {
        "agentSpaceId": ...,
    }


# ListIntegratedResourcesInputPaginateTypeDef definition

class ListIntegratedResourcesInputPaginateTypeDef(TypedDict):
    agentSpaceId: str,
    integrationId: NotRequired[str],
    resourceType: NotRequired[ResourceTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListIntegrationsInputPaginateTypeDef

```python
# ListIntegrationsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListIntegrationsInputPaginateTypeDef


def get_value() -> ListIntegrationsInputPaginateTypeDef:
    return {
        "filter": ...,
    }


# ListIntegrationsInputPaginateTypeDef definition

class ListIntegrationsInputPaginateTypeDef(TypedDict):
    filter: NotRequired[IntegrationFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: IntegrationFilterTypeDef](./type_defs.md#integrationfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListMembershipsRequestPaginateTypeDef

```python
# ListMembershipsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListMembershipsRequestPaginateTypeDef


def get_value() -> ListMembershipsRequestPaginateTypeDef:
    return {
        "applicationId": ...,
    }


# ListMembershipsRequestPaginateTypeDef definition

class ListMembershipsRequestPaginateTypeDef(TypedDict):
    applicationId: str,
    agentSpaceId: str,
    memberType: NotRequired[MembershipTypeFilterType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: MembershipTypeFilterType](./literals.md#membershiptypefiltertype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListPentestJobTasksInputPaginateTypeDef

```python
# ListPentestJobTasksInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListPentestJobTasksInputPaginateTypeDef


def get_value() -> ListPentestJobTasksInputPaginateTypeDef:
    return {
        "agentSpaceId": ...,
    }


# ListPentestJobTasksInputPaginateTypeDef definition

class ListPentestJobTasksInputPaginateTypeDef(TypedDict):
    agentSpaceId: str,
    pentestJobId: NotRequired[str],
    stepName: NotRequired[StepNameType],  # (1)
    categoryName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: StepNameType](./literals.md#stepnametype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListPentestJobsForPentestInputPaginateTypeDef

```python
# ListPentestJobsForPentestInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListPentestJobsForPentestInputPaginateTypeDef


def get_value() -> ListPentestJobsForPentestInputPaginateTypeDef:
    return {
        "pentestId": ...,
    }


# ListPentestJobsForPentestInputPaginateTypeDef definition

class ListPentestJobsForPentestInputPaginateTypeDef(TypedDict):
    pentestId: str,
    agentSpaceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListPentestsInputPaginateTypeDef

```python
# ListPentestsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListPentestsInputPaginateTypeDef


def get_value() -> ListPentestsInputPaginateTypeDef:
    return {
        "agentSpaceId": ...,
    }


# ListPentestsInputPaginateTypeDef definition

class ListPentestsInputPaginateTypeDef(TypedDict):
    agentSpaceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListTargetDomainsInputPaginateTypeDef

```python
# ListTargetDomainsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListTargetDomainsInputPaginateTypeDef


def get_value() -> ListTargetDomainsInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListTargetDomainsInputPaginateTypeDef definition

class ListTargetDomainsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListPentestJobTasksOutputTypeDef

```python
# ListPentestJobTasksOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListPentestJobTasksOutputTypeDef


def get_value() -> ListPentestJobTasksOutputTypeDef:
    return {
        "taskSummaries": ...,
    }


# ListPentestJobTasksOutputTypeDef definition

class ListPentestJobTasksOutputTypeDef(TypedDict):
    taskSummaries: list[TaskSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[TaskSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListPentestJobsForPentestOutputTypeDef

```python
# ListPentestJobsForPentestOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListPentestJobsForPentestOutputTypeDef


def get_value() -> ListPentestJobsForPentestOutputTypeDef:
    return {
        "pentestJobSummaries": ...,
    }


# ListPentestJobsForPentestOutputTypeDef definition

class ListPentestJobsForPentestOutputTypeDef(TypedDict):
    pentestJobSummaries: list[PentestJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[PentestJobSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListPentestsOutputTypeDef

```python
# ListPentestsOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListPentestsOutputTypeDef


def get_value() -> ListPentestsOutputTypeDef:
    return {
        "pentestSummaries": ...,
    }


# ListPentestsOutputTypeDef definition

class ListPentestsOutputTypeDef(TypedDict):
    pentestSummaries: list[PentestSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[PentestSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListTargetDomainsOutputTypeDef

```python
# ListTargetDomainsOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListTargetDomainsOutputTypeDef


def get_value() -> ListTargetDomainsOutputTypeDef:
    return {
        "targetDomainSummaries": ...,
    }


# ListTargetDomainsOutputTypeDef definition

class ListTargetDomainsOutputTypeDef(TypedDict):
    targetDomainSummaries: list[TargetDomainSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[TargetDomainSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## MemberMetadataTypeDef

```python
# MemberMetadataTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import MemberMetadataTypeDef


def get_value() -> MemberMetadataTypeDef:
    return {
        "user": ...,
    }


# MemberMetadataTypeDef definition

class MemberMetadataTypeDef(TypedDict):
    user: NotRequired[UserMetadataTypeDef],  # (1)
```

1. See [:material-code-braces: UserMetadataTypeDef](./type_defs.md#usermetadatatypedef)

## MembershipConfigTypeDef

```python
# MembershipConfigTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import MembershipConfigTypeDef


def get_value() -> MembershipConfigTypeDef:
    return {
        "user": ...,
    }


# MembershipConfigTypeDef definition

class MembershipConfigTypeDef(TypedDict):
    user: NotRequired[UserConfigTypeDef],  # (1)
```

1. See [:material-code-braces: UserConfigTypeDef](./type_defs.md#userconfigtypedef)

## NetworkTrafficConfigOutputTypeDef

```python
# NetworkTrafficConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import NetworkTrafficConfigOutputTypeDef


def get_value() -> NetworkTrafficConfigOutputTypeDef:
    return {
        "rules": ...,
    }


# NetworkTrafficConfigOutputTypeDef definition

class NetworkTrafficConfigOutputTypeDef(TypedDict):
    rules: NotRequired[list[NetworkTrafficRuleTypeDef]],  # (1)
    customHeaders: NotRequired[list[CustomHeaderTypeDef]],  # (2)
```

1. See `list[NetworkTrafficRuleTypeDef]`
2. See `list[CustomHeaderTypeDef]`

## NetworkTrafficConfigTypeDef

```python
# NetworkTrafficConfigTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import NetworkTrafficConfigTypeDef


def get_value() -> NetworkTrafficConfigTypeDef:
    return {
        "rules": ...,
    }


# NetworkTrafficConfigTypeDef definition

class NetworkTrafficConfigTypeDef(TypedDict):
    rules: NotRequired[Sequence[NetworkTrafficRuleTypeDef]],  # (1)
    customHeaders: NotRequired[Sequence[CustomHeaderTypeDef]],  # (2)
```

1. See `Sequence[NetworkTrafficRuleTypeDef]`
2. See `Sequence[CustomHeaderTypeDef]`

## AgentSpaceTypeDef

```python
# AgentSpaceTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import AgentSpaceTypeDef


def get_value() -> AgentSpaceTypeDef:
    return {
        "agentSpaceId": ...,
    }


# AgentSpaceTypeDef definition

class AgentSpaceTypeDef(TypedDict):
    agentSpaceId: str,
    name: str,
    description: NotRequired[str],
    awsResources: NotRequired[AWSResourcesOutputTypeDef],  # (1)
    targetDomainIds: NotRequired[list[str]],
    codeReviewSettings: NotRequired[CodeReviewSettingsTypeDef],  # (2)
    kmsKeyId: NotRequired[str],
    createdAt: NotRequired[datetime.datetime],
    updatedAt: NotRequired[datetime.datetime],
```

1. See [:material-code-braces: AWSResourcesOutputTypeDef](./type_defs.md#awsresourcesoutputtypedef)
2. See [:material-code-braces: CodeReviewSettingsTypeDef](./type_defs.md#codereviewsettingstypedef)

## CreateAgentSpaceOutputTypeDef

```python
# CreateAgentSpaceOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CreateAgentSpaceOutputTypeDef


def get_value() -> CreateAgentSpaceOutputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# CreateAgentSpaceOutputTypeDef definition

class CreateAgentSpaceOutputTypeDef(TypedDict):
    agentSpaceId: str,
    name: str,
    description: str,
    awsResources: AWSResourcesOutputTypeDef,  # (1)
    targetDomainIds: list[str],
    codeReviewSettings: CodeReviewSettingsTypeDef,  # (2)
    kmsKeyId: str,
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AWSResourcesOutputTypeDef](./type_defs.md#awsresourcesoutputtypedef)
2. See [:material-code-braces: CodeReviewSettingsTypeDef](./type_defs.md#codereviewsettingstypedef)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateAgentSpaceOutputTypeDef

```python
# UpdateAgentSpaceOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import UpdateAgentSpaceOutputTypeDef


def get_value() -> UpdateAgentSpaceOutputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# UpdateAgentSpaceOutputTypeDef definition

class UpdateAgentSpaceOutputTypeDef(TypedDict):
    agentSpaceId: str,
    name: str,
    description: str,
    awsResources: AWSResourcesOutputTypeDef,  # (1)
    targetDomainIds: list[str],
    codeReviewSettings: CodeReviewSettingsTypeDef,  # (2)
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AWSResourcesOutputTypeDef](./type_defs.md#awsresourcesoutputtypedef)
2. See [:material-code-braces: CodeReviewSettingsTypeDef](./type_defs.md#codereviewsettingstypedef)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## AssetsOutputTypeDef

```python
# AssetsOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import AssetsOutputTypeDef


def get_value() -> AssetsOutputTypeDef:
    return {
        "endpoints": ...,
    }


# AssetsOutputTypeDef definition

class AssetsOutputTypeDef(TypedDict):
    endpoints: NotRequired[list[EndpointTypeDef]],  # (1)
    actors: NotRequired[list[ActorOutputTypeDef]],  # (2)
    documents: NotRequired[list[DocumentInfoTypeDef]],  # (3)
    sourceCode: NotRequired[list[SourceCodeRepositoryTypeDef]],  # (4)
    integratedRepositories: NotRequired[list[IntegratedRepositoryTypeDef]],  # (5)
```

1. See `list[EndpointTypeDef]`
2. See `list[ActorOutputTypeDef]`
3. See `list[DocumentInfoTypeDef]`
4. See `list[SourceCodeRepositoryTypeDef]`
5. See `list[IntegratedRepositoryTypeDef]`

## AssetsTypeDef

```python
# AssetsTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import AssetsTypeDef


def get_value() -> AssetsTypeDef:
    return {
        "endpoints": ...,
    }


# AssetsTypeDef definition

class AssetsTypeDef(TypedDict):
    endpoints: NotRequired[Sequence[EndpointTypeDef]],  # (1)
    actors: NotRequired[Sequence[ActorTypeDef]],  # (2)
    documents: NotRequired[Sequence[DocumentInfoTypeDef]],  # (3)
    sourceCode: NotRequired[Sequence[SourceCodeRepositoryTypeDef]],  # (4)
    integratedRepositories: NotRequired[Sequence[IntegratedRepositoryTypeDef]],  # (5)
```

1. See `Sequence[EndpointTypeDef]`
2. See `Sequence[ActorTypeDef]`
3. See `Sequence[DocumentInfoTypeDef]`
4. See `Sequence[SourceCodeRepositoryTypeDef]`
5. See `Sequence[IntegratedRepositoryTypeDef]`

## TaskTypeDef

```python
# TaskTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import TaskTypeDef


def get_value() -> TaskTypeDef:
    return {
        "taskId": ...,
    }


# TaskTypeDef definition

class TaskTypeDef(TypedDict):
    taskId: str,
    pentestId: NotRequired[str],
    pentestJobId: NotRequired[str],
    agentSpaceId: NotRequired[str],
    title: NotRequired[str],
    description: NotRequired[str],
    categories: NotRequired[list[CategoryTypeDef]],  # (1)
    riskType: NotRequired[RiskTypeType],  # (2)
    targetEndpoint: NotRequired[EndpointTypeDef],  # (3)
    executionStatus: NotRequired[TaskExecutionStatusType],  # (4)
    logsLocation: NotRequired[LogLocationTypeDef],  # (5)
    createdAt: NotRequired[datetime.datetime],
    updatedAt: NotRequired[datetime.datetime],
```

1. See `list[CategoryTypeDef]`
2. See [:material-code-brackets: RiskTypeType](./literals.md#risktypetype)
3. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef)
4. See [:material-code-brackets: TaskExecutionStatusType](./literals.md#taskexecutionstatustype)
5. See [:material-code-braces: LogLocationTypeDef](./type_defs.md#loglocationtypedef)

## FindingTypeDef

```python
# FindingTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import FindingTypeDef


def get_value() -> FindingTypeDef:
    return {
        "findingId": ...,
    }


# FindingTypeDef definition

class FindingTypeDef(TypedDict):
    findingId: str,
    agentSpaceId: str,
    pentestId: NotRequired[str],
    pentestJobId: NotRequired[str],
    taskId: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    status: NotRequired[FindingStatusType],  # (1)
    riskType: NotRequired[str],
    riskLevel: NotRequired[RiskLevelType],  # (2)
    riskScore: NotRequired[str],
    reasoning: NotRequired[str],
    confidence: NotRequired[ConfidenceLevelType],  # (3)
    attackScript: NotRequired[str],
    codeRemediationTask: NotRequired[CodeRemediationTaskTypeDef],  # (4)
    lastUpdatedBy: NotRequired[str],
    createdAt: NotRequired[datetime.datetime],
    updatedAt: NotRequired[datetime.datetime],
```

1. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype)
2. See [:material-code-brackets: RiskLevelType](./literals.md#riskleveltype)
3. See [:material-code-brackets: ConfidenceLevelType](./literals.md#confidenceleveltype)
4. See [:material-code-braces: CodeRemediationTaskTypeDef](./type_defs.md#coderemediationtasktypedef)

## CreateIntegrationInputTypeDef

```python
# CreateIntegrationInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CreateIntegrationInputTypeDef


def get_value() -> CreateIntegrationInputTypeDef:
    return {
        "provider": ...,
    }


# CreateIntegrationInputTypeDef definition

class CreateIntegrationInputTypeDef(TypedDict):
    provider: ProviderType,  # (1)
    input: ProviderInputTypeDef,  # (2)
    integrationDisplayName: str,
    kmsKeyId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ProviderType](./literals.md#providertype)
2. See [:material-code-braces: ProviderInputTypeDef](./type_defs.md#providerinputtypedef)

## IntegratedResourceInputItemTypeDef

```python
# IntegratedResourceInputItemTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import IntegratedResourceInputItemTypeDef


def get_value() -> IntegratedResourceInputItemTypeDef:
    return {
        "resource": ...,
    }


# IntegratedResourceInputItemTypeDef definition

class IntegratedResourceInputItemTypeDef(TypedDict):
    resource: IntegratedResourceTypeDef,  # (1)
    capabilities: NotRequired[ProviderResourceCapabilitiesTypeDef],  # (2)
```

1. See [:material-code-braces: IntegratedResourceTypeDef](./type_defs.md#integratedresourcetypedef)
2. See [:material-code-braces: ProviderResourceCapabilitiesTypeDef](./type_defs.md#providerresourcecapabilitiestypedef)

## IntegratedResourceSummaryTypeDef

```python
# IntegratedResourceSummaryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import IntegratedResourceSummaryTypeDef


def get_value() -> IntegratedResourceSummaryTypeDef:
    return {
        "integrationId": ...,
    }


# IntegratedResourceSummaryTypeDef definition

class IntegratedResourceSummaryTypeDef(TypedDict):
    integrationId: str,
    resource: IntegratedResourceMetadataTypeDef,  # (1)
    capabilities: NotRequired[ProviderResourceCapabilitiesTypeDef],  # (2)
```

1. See [:material-code-braces: IntegratedResourceMetadataTypeDef](./type_defs.md#integratedresourcemetadatatypedef)
2. See [:material-code-braces: ProviderResourceCapabilitiesTypeDef](./type_defs.md#providerresourcecapabilitiestypedef)

## CreateTargetDomainOutputTypeDef

```python
# CreateTargetDomainOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CreateTargetDomainOutputTypeDef


def get_value() -> CreateTargetDomainOutputTypeDef:
    return {
        "targetDomainId": ...,
    }


# CreateTargetDomainOutputTypeDef definition

class CreateTargetDomainOutputTypeDef(TypedDict):
    targetDomainId: str,
    domainName: str,
    verificationStatus: TargetDomainStatusType,  # (1)
    verificationStatusReason: str,
    verificationDetails: VerificationDetailsTypeDef,  # (2)
    createdAt: datetime.datetime,
    verifiedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TargetDomainStatusType](./literals.md#targetdomainstatustype)
2. See [:material-code-braces: VerificationDetailsTypeDef](./type_defs.md#verificationdetailstypedef)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## TargetDomainTypeDef

```python
# TargetDomainTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import TargetDomainTypeDef


def get_value() -> TargetDomainTypeDef:
    return {
        "targetDomainId": ...,
    }


# TargetDomainTypeDef definition

class TargetDomainTypeDef(TypedDict):
    targetDomainId: str,
    domainName: str,
    verificationStatus: NotRequired[TargetDomainStatusType],  # (1)
    verificationStatusReason: NotRequired[str],
    verificationDetails: NotRequired[VerificationDetailsTypeDef],  # (2)
    createdAt: NotRequired[datetime.datetime],
    verifiedAt: NotRequired[datetime.datetime],
```

1. See [:material-code-brackets: TargetDomainStatusType](./literals.md#targetdomainstatustype)
2. See [:material-code-braces: VerificationDetailsTypeDef](./type_defs.md#verificationdetailstypedef)

## UpdateTargetDomainOutputTypeDef

```python
# UpdateTargetDomainOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import UpdateTargetDomainOutputTypeDef


def get_value() -> UpdateTargetDomainOutputTypeDef:
    return {
        "targetDomainId": ...,
    }


# UpdateTargetDomainOutputTypeDef definition

class UpdateTargetDomainOutputTypeDef(TypedDict):
    targetDomainId: str,
    domainName: str,
    verificationStatus: TargetDomainStatusType,  # (1)
    verificationStatusReason: str,
    verificationDetails: VerificationDetailsTypeDef,  # (2)
    createdAt: datetime.datetime,
    verifiedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TargetDomainStatusType](./literals.md#targetdomainstatustype)
2. See [:material-code-braces: VerificationDetailsTypeDef](./type_defs.md#verificationdetailstypedef)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateMembershipRequestTypeDef

```python
# CreateMembershipRequestTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CreateMembershipRequestTypeDef


def get_value() -> CreateMembershipRequestTypeDef:
    return {
        "applicationId": ...,
    }


# CreateMembershipRequestTypeDef definition

class CreateMembershipRequestTypeDef(TypedDict):
    applicationId: str,
    agentSpaceId: str,
    membershipId: str,
    memberType: MembershipTypeType,  # (1)
    config: NotRequired[MembershipConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype)
2. See [:material-code-braces: MembershipConfigTypeDef](./type_defs.md#membershipconfigtypedef)

## MembershipSummaryTypeDef

```python
# MembershipSummaryTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import MembershipSummaryTypeDef


def get_value() -> MembershipSummaryTypeDef:
    return {
        "membershipId": ...,
    }


# MembershipSummaryTypeDef definition

class MembershipSummaryTypeDef(TypedDict):
    membershipId: str,
    applicationId: str,
    agentSpaceId: str,
    memberType: MembershipTypeType,  # (1)
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    createdBy: str,
    updatedBy: str,
    config: NotRequired[MembershipConfigTypeDef],  # (2)
    metadata: NotRequired[MemberMetadataTypeDef],  # (3)
```

1. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype)
2. See [:material-code-braces: MembershipConfigTypeDef](./type_defs.md#membershipconfigtypedef)
3. See [:material-code-braces: MemberMetadataTypeDef](./type_defs.md#membermetadatatypedef)

## PentestJobTypeDef

```python
# PentestJobTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import PentestJobTypeDef


def get_value() -> PentestJobTypeDef:
    return {
        "pentestJobId": ...,
    }


# PentestJobTypeDef definition

class PentestJobTypeDef(TypedDict):
    pentestJobId: NotRequired[str],
    pentestId: NotRequired[str],
    title: NotRequired[str],
    overview: NotRequired[str],
    status: NotRequired[JobStatusType],  # (1)
    endpoints: NotRequired[list[EndpointTypeDef]],  # (2)
    actors: NotRequired[list[ActorOutputTypeDef]],  # (3)
    documents: NotRequired[list[DocumentInfoTypeDef]],  # (4)
    sourceCode: NotRequired[list[SourceCodeRepositoryTypeDef]],  # (5)
    excludePaths: NotRequired[list[EndpointTypeDef]],  # (2)
    allowedDomains: NotRequired[list[EndpointTypeDef]],  # (2)
    excludeRiskTypes: NotRequired[list[RiskTypeType]],  # (8)
    steps: NotRequired[list[StepTypeDef]],  # (9)
    executionContext: NotRequired[list[ExecutionContextTypeDef]],  # (10)
    serviceRole: NotRequired[str],
    logConfig: NotRequired[CloudWatchLogTypeDef],  # (11)
    vpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (12)
    networkTrafficConfig: NotRequired[NetworkTrafficConfigOutputTypeDef],  # (13)
    errorInformation: NotRequired[ErrorInformationTypeDef],  # (14)
    integratedRepositories: NotRequired[list[IntegratedRepositoryTypeDef]],  # (15)
    codeRemediationStrategy: NotRequired[CodeRemediationStrategyType],  # (16)
    createdAt: NotRequired[datetime.datetime],
    updatedAt: NotRequired[datetime.datetime],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype)
2. See `list[EndpointTypeDef]`
3. See `list[ActorOutputTypeDef]`
4. See `list[DocumentInfoTypeDef]`
5. See `list[SourceCodeRepositoryTypeDef]`
6. See `list[EndpointTypeDef]`
7. See `list[EndpointTypeDef]`
8. See `list[RiskTypeType]`
9. See `list[StepTypeDef]`
10. See `list[ExecutionContextTypeDef]`
11. See [:material-code-braces: CloudWatchLogTypeDef](./type_defs.md#cloudwatchlogtypedef)
12. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
13. See [:material-code-braces: NetworkTrafficConfigOutputTypeDef](./type_defs.md#networktrafficconfigoutputtypedef)
14. See [:material-code-braces: ErrorInformationTypeDef](./type_defs.md#errorinformationtypedef)
15. See `list[IntegratedRepositoryTypeDef]`
16. See [:material-code-brackets: CodeRemediationStrategyType](./literals.md#coderemediationstrategytype)

## BatchGetAgentSpacesOutputTypeDef

```python
# BatchGetAgentSpacesOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetAgentSpacesOutputTypeDef


def get_value() -> BatchGetAgentSpacesOutputTypeDef:
    return {
        "agentSpaces": ...,
    }


# BatchGetAgentSpacesOutputTypeDef definition

class BatchGetAgentSpacesOutputTypeDef(TypedDict):
    agentSpaces: list[AgentSpaceTypeDef],  # (1)
    notFound: list[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `list[AgentSpaceTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateAgentSpaceInputTypeDef

```python
# CreateAgentSpaceInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CreateAgentSpaceInputTypeDef


def get_value() -> CreateAgentSpaceInputTypeDef:
    return {
        "name": ...,
    }


# CreateAgentSpaceInputTypeDef definition

class CreateAgentSpaceInputTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    awsResources: NotRequired[AWSResourcesUnionTypeDef],  # (1)
    targetDomainIds: NotRequired[Sequence[str]],
    codeReviewSettings: NotRequired[CodeReviewSettingsTypeDef],  # (2)
    kmsKeyId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AWSResourcesUnionTypeDef](#awsresourcesuniontypedef)
2. See [:material-code-braces: CodeReviewSettingsTypeDef](./type_defs.md#codereviewsettingstypedef)

## UpdateAgentSpaceInputTypeDef

```python
# UpdateAgentSpaceInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import UpdateAgentSpaceInputTypeDef


def get_value() -> UpdateAgentSpaceInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# UpdateAgentSpaceInputTypeDef definition

class UpdateAgentSpaceInputTypeDef(TypedDict):
    agentSpaceId: str,
    name: NotRequired[str],
    description: NotRequired[str],
    awsResources: NotRequired[AWSResourcesUnionTypeDef],  # (1)
    targetDomainIds: NotRequired[Sequence[str]],
    codeReviewSettings: NotRequired[CodeReviewSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: AWSResourcesUnionTypeDef](#awsresourcesuniontypedef)
2. See [:material-code-braces: CodeReviewSettingsTypeDef](./type_defs.md#codereviewsettingstypedef)

## CreatePentestOutputTypeDef

```python
# CreatePentestOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CreatePentestOutputTypeDef


def get_value() -> CreatePentestOutputTypeDef:
    return {
        "pentestId": ...,
    }


# CreatePentestOutputTypeDef definition

class CreatePentestOutputTypeDef(TypedDict):
    pentestId: str,
    title: str,
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    assets: AssetsOutputTypeDef,  # (1)
    excludeRiskTypes: list[RiskTypeType],  # (2)
    serviceRole: str,
    logConfig: CloudWatchLogTypeDef,  # (3)
    agentSpaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AssetsOutputTypeDef](./type_defs.md#assetsoutputtypedef)
2. See `list[RiskTypeType]`
3. See [:material-code-braces: CloudWatchLogTypeDef](./type_defs.md#cloudwatchlogtypedef)
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## PentestTypeDef

```python
# PentestTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import PentestTypeDef


def get_value() -> PentestTypeDef:
    return {
        "pentestId": ...,
    }


# PentestTypeDef definition

class PentestTypeDef(TypedDict):
    pentestId: str,
    agentSpaceId: str,
    title: str,
    assets: AssetsOutputTypeDef,  # (1)
    excludeRiskTypes: NotRequired[list[RiskTypeType]],  # (2)
    serviceRole: NotRequired[str],
    logConfig: NotRequired[CloudWatchLogTypeDef],  # (3)
    vpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (4)
    networkTrafficConfig: NotRequired[NetworkTrafficConfigOutputTypeDef],  # (5)
    codeRemediationStrategy: NotRequired[CodeRemediationStrategyType],  # (6)
    createdAt: NotRequired[datetime.datetime],
    updatedAt: NotRequired[datetime.datetime],
```

1. See [:material-code-braces: AssetsOutputTypeDef](./type_defs.md#assetsoutputtypedef)
2. See `list[RiskTypeType]`
3. See [:material-code-braces: CloudWatchLogTypeDef](./type_defs.md#cloudwatchlogtypedef)
4. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
5. See [:material-code-braces: NetworkTrafficConfigOutputTypeDef](./type_defs.md#networktrafficconfigoutputtypedef)
6. See [:material-code-brackets: CodeRemediationStrategyType](./literals.md#coderemediationstrategytype)

## UpdatePentestOutputTypeDef

```python
# UpdatePentestOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import UpdatePentestOutputTypeDef


def get_value() -> UpdatePentestOutputTypeDef:
    return {
        "pentestId": ...,
    }


# UpdatePentestOutputTypeDef definition

class UpdatePentestOutputTypeDef(TypedDict):
    pentestId: str,
    title: str,
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    assets: AssetsOutputTypeDef,  # (1)
    excludeRiskTypes: list[RiskTypeType],  # (2)
    serviceRole: str,
    logConfig: CloudWatchLogTypeDef,  # (3)
    agentSpaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AssetsOutputTypeDef](./type_defs.md#assetsoutputtypedef)
2. See `list[RiskTypeType]`
3. See [:material-code-braces: CloudWatchLogTypeDef](./type_defs.md#cloudwatchlogtypedef)
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## BatchGetPentestJobTasksOutputTypeDef

```python
# BatchGetPentestJobTasksOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetPentestJobTasksOutputTypeDef


def get_value() -> BatchGetPentestJobTasksOutputTypeDef:
    return {
        "tasks": ...,
    }


# BatchGetPentestJobTasksOutputTypeDef definition

class BatchGetPentestJobTasksOutputTypeDef(TypedDict):
    tasks: list[TaskTypeDef],  # (1)
    notFound: list[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `list[TaskTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## BatchGetFindingsOutputTypeDef

```python
# BatchGetFindingsOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetFindingsOutputTypeDef


def get_value() -> BatchGetFindingsOutputTypeDef:
    return {
        "findings": ...,
    }


# BatchGetFindingsOutputTypeDef definition

class BatchGetFindingsOutputTypeDef(TypedDict):
    findings: list[FindingTypeDef],  # (1)
    notFound: list[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `list[FindingTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateIntegratedResourcesInputTypeDef

```python
# UpdateIntegratedResourcesInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import UpdateIntegratedResourcesInputTypeDef


def get_value() -> UpdateIntegratedResourcesInputTypeDef:
    return {
        "agentSpaceId": ...,
    }


# UpdateIntegratedResourcesInputTypeDef definition

class UpdateIntegratedResourcesInputTypeDef(TypedDict):
    agentSpaceId: str,
    integrationId: str,
    items: Sequence[IntegratedResourceInputItemTypeDef],  # (1)
```

1. See `Sequence[IntegratedResourceInputItemTypeDef]`

## ListIntegratedResourcesOutputTypeDef

```python
# ListIntegratedResourcesOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListIntegratedResourcesOutputTypeDef


def get_value() -> ListIntegratedResourcesOutputTypeDef:
    return {
        "integratedResourceSummaries": ...,
    }


# ListIntegratedResourcesOutputTypeDef definition

class ListIntegratedResourcesOutputTypeDef(TypedDict):
    integratedResourceSummaries: list[IntegratedResourceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[IntegratedResourceSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## BatchGetTargetDomainsOutputTypeDef

```python
# BatchGetTargetDomainsOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetTargetDomainsOutputTypeDef


def get_value() -> BatchGetTargetDomainsOutputTypeDef:
    return {
        "targetDomains": ...,
    }


# BatchGetTargetDomainsOutputTypeDef definition

class BatchGetTargetDomainsOutputTypeDef(TypedDict):
    targetDomains: list[TargetDomainTypeDef],  # (1)
    notFound: list[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `list[TargetDomainTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListMembershipsResponseTypeDef

```python
# ListMembershipsResponseTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import ListMembershipsResponseTypeDef


def get_value() -> ListMembershipsResponseTypeDef:
    return {
        "membershipSummaries": ...,
    }


# ListMembershipsResponseTypeDef definition

class ListMembershipsResponseTypeDef(TypedDict):
    membershipSummaries: list[MembershipSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[MembershipSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## BatchGetPentestJobsOutputTypeDef

```python
# BatchGetPentestJobsOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetPentestJobsOutputTypeDef


def get_value() -> BatchGetPentestJobsOutputTypeDef:
    return {
        "pentestJobs": ...,
    }


# BatchGetPentestJobsOutputTypeDef definition

class BatchGetPentestJobsOutputTypeDef(TypedDict):
    pentestJobs: list[PentestJobTypeDef],  # (1)
    notFound: list[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `list[PentestJobTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## BatchDeletePentestsOutputTypeDef

```python
# BatchDeletePentestsOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchDeletePentestsOutputTypeDef


def get_value() -> BatchDeletePentestsOutputTypeDef:
    return {
        "deleted": ...,
    }


# BatchDeletePentestsOutputTypeDef definition

class BatchDeletePentestsOutputTypeDef(TypedDict):
    deleted: list[PentestTypeDef],  # (1)
    failed: list[DeletePentestFailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See `list[PentestTypeDef]`
2. See `list[DeletePentestFailureTypeDef]`
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## BatchGetPentestsOutputTypeDef

```python
# BatchGetPentestsOutputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import BatchGetPentestsOutputTypeDef


def get_value() -> BatchGetPentestsOutputTypeDef:
    return {
        "pentests": ...,
    }


# BatchGetPentestsOutputTypeDef definition

class BatchGetPentestsOutputTypeDef(TypedDict):
    pentests: list[PentestTypeDef],  # (1)
    notFound: list[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `list[PentestTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreatePentestInputTypeDef

```python
# CreatePentestInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import CreatePentestInputTypeDef


def get_value() -> CreatePentestInputTypeDef:
    return {
        "title": ...,
    }


# CreatePentestInputTypeDef definition

class CreatePentestInputTypeDef(TypedDict):
    title: str,
    agentSpaceId: str,
    assets: NotRequired[AssetsUnionTypeDef],  # (1)
    excludeRiskTypes: NotRequired[Sequence[RiskTypeType]],  # (2)
    serviceRole: NotRequired[str],
    logConfig: NotRequired[CloudWatchLogTypeDef],  # (3)
    vpcConfig: NotRequired[VpcConfigUnionTypeDef],  # (4)
    networkTrafficConfig: NotRequired[NetworkTrafficConfigUnionTypeDef],  # (5)
    codeRemediationStrategy: NotRequired[CodeRemediationStrategyType],  # (6)
```

1. See [:material-code-braces: AssetsUnionTypeDef](#assetsuniontypedef)
2. See `Sequence[RiskTypeType]`
3. See [:material-code-braces: CloudWatchLogTypeDef](./type_defs.md#cloudwatchlogtypedef)
4. See [:material-code-braces: VpcConfigUnionTypeDef](#vpcconfiguniontypedef)
5. See [:material-code-braces: NetworkTrafficConfigUnionTypeDef](#networktrafficconfiguniontypedef)
6. See [:material-code-brackets: CodeRemediationStrategyType](./literals.md#coderemediationstrategytype)

## UpdatePentestInputTypeDef

```python
# UpdatePentestInputTypeDef TypedDict usage example

from types_aiobotocore_securityagent.type_defs import UpdatePentestInputTypeDef


def get_value() -> UpdatePentestInputTypeDef:
    return {
        "pentestId": ...,
    }


# UpdatePentestInputTypeDef definition

class UpdatePentestInputTypeDef(TypedDict):
    pentestId: str,
    agentSpaceId: str,
    title: NotRequired[str],
    assets: NotRequired[AssetsUnionTypeDef],  # (1)
    excludeRiskTypes: NotRequired[Sequence[RiskTypeType]],  # (2)
    serviceRole: NotRequired[str],
    logConfig: NotRequired[CloudWatchLogTypeDef],  # (3)
    vpcConfig: NotRequired[VpcConfigUnionTypeDef],  # (4)
    networkTrafficConfig: NotRequired[NetworkTrafficConfigUnionTypeDef],  # (5)
    codeRemediationStrategy: NotRequired[CodeRemediationStrategyType],  # (6)
```

1. See [:material-code-braces: AssetsUnionTypeDef](#assetsuniontypedef)
2. See `Sequence[RiskTypeType]`
3. See [:material-code-braces: CloudWatchLogTypeDef](./type_defs.md#cloudwatchlogtypedef)
4. See [:material-code-braces: VpcConfigUnionTypeDef](#vpcconfiguniontypedef)
5. See [:material-code-braces: NetworkTrafficConfigUnionTypeDef](#networktrafficconfiguniontypedef)
6. See [:material-code-brackets: CodeRemediationStrategyType](./literals.md#coderemediationstrategytype)

