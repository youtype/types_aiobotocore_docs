# SecurityAgent module

> [Index](../README.md) > SecurityAgent


!!! note ""

    Auto-generated documentation for [SecurityAgent](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent.html#securityagent)
    type annotations stubs module [types-aiobotocore-securityagent](https://pypi.org/project/types-aiobotocore-securityagent/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.7.0' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SecurityAgent` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SecurityAgent` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[securityagent]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[securityagent]'

# standalone installation
python -m pip install types-aiobotocore-securityagent
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-securityagent
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SecurityAgentClient

Type annotations and code completion for  `#!python session.create_client("securityagent")` as [SecurityAgentClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent.html#SecurityAgent.Client)

```python
# SecurityAgentClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityagent.client import SecurityAgentClient


session = get_session()
async with session.create_client("securityagent") as client:
    client: SecurityAgentClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("securityagent").get_paginator("...")`.

```python
# ListAgentSpacesPaginator usage example

from types_aiobotocore_securityagent.paginator import ListAgentSpacesPaginator

def get_list_agent_spaces_paginator() -> ListAgentSpacesPaginator:
    return client.get_paginator("list_agent_spaces"))
```

- [ListAgentSpacesPaginator](./paginators.md#listagentspacespaginator)
- [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- [ListArtifactsPaginator](./paginators.md#listartifactspaginator)
- [ListDiscoveredEndpointsPaginator](./paginators.md#listdiscoveredendpointspaginator)
- [ListFindingsPaginator](./paginators.md#listfindingspaginator)
- [ListIntegratedResourcesPaginator](./paginators.md#listintegratedresourcespaginator)
- [ListIntegrationsPaginator](./paginators.md#listintegrationspaginator)
- [ListMembershipsPaginator](./paginators.md#listmembershipspaginator)
- [ListPentestJobTasksPaginator](./paginators.md#listpentestjobtaskspaginator)
- [ListPentestJobsForPentestPaginator](./paginators.md#listpentestjobsforpentestpaginator)
- [ListPentestsPaginator](./paginators.md#listpentestspaginator)
- [ListTargetDomainsPaginator](./paginators.md#listtargetdomainspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccessTypeType usage example

from types_aiobotocore_securityagent.literals import AccessTypeType

def get_value() -> AccessTypeType:
    return "PRIVATE"
```

- [AccessTypeType](./literals.md#accesstypetype)
- [ArtifactTypeType](./literals.md#artifacttypetype)
- [AuthenticationProviderTypeType](./literals.md#authenticationprovidertypetype)
- [CodeRemediationStrategyType](./literals.md#coderemediationstrategytype)
- [CodeRemediationTaskStatusType](./literals.md#coderemediationtaskstatustype)
- [ConfidenceLevelType](./literals.md#confidenceleveltype)
- [ContextTypeType](./literals.md#contexttypetype)
- [DNSRecordTypeType](./literals.md#dnsrecordtypetype)
- [DomainVerificationMethodType](./literals.md#domainverificationmethodtype)
- [ErrorCodeType](./literals.md#errorcodetype)
- [FindingStatusType](./literals.md#findingstatustype)
- [JobStatusType](./literals.md#jobstatustype)
- [ListAgentSpacesPaginatorName](./literals.md#listagentspacespaginatorname)
- [ListApplicationsPaginatorName](./literals.md#listapplicationspaginatorname)
- [ListArtifactsPaginatorName](./literals.md#listartifactspaginatorname)
- [ListDiscoveredEndpointsPaginatorName](./literals.md#listdiscoveredendpointspaginatorname)
- [ListFindingsPaginatorName](./literals.md#listfindingspaginatorname)
- [ListIntegratedResourcesPaginatorName](./literals.md#listintegratedresourcespaginatorname)
- [ListIntegrationsPaginatorName](./literals.md#listintegrationspaginatorname)
- [ListMembershipsPaginatorName](./literals.md#listmembershipspaginatorname)
- [ListPentestJobTasksPaginatorName](./literals.md#listpentestjobtaskspaginatorname)
- [ListPentestJobsForPentestPaginatorName](./literals.md#listpentestjobsforpentestpaginatorname)
- [ListPentestsPaginatorName](./literals.md#listpentestspaginatorname)
- [ListTargetDomainsPaginatorName](./literals.md#listtargetdomainspaginatorname)
- [LogTypeType](./literals.md#logtypetype)
- [MembershipTypeFilterType](./literals.md#membershiptypefiltertype)
- [MembershipTypeType](./literals.md#membershiptypetype)
- [NetworkTrafficRuleEffectType](./literals.md#networktrafficruleeffecttype)
- [NetworkTrafficRuleTypeType](./literals.md#networktrafficruletypetype)
- [ProviderType](./literals.md#providertype)
- [ProviderTypeType](./literals.md#providertypetype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [RiskLevelType](./literals.md#riskleveltype)
- [RiskTypeType](./literals.md#risktypetype)
- [StepNameType](./literals.md#stepnametype)
- [StepStatusType](./literals.md#stepstatustype)
- [TargetDomainStatusType](./literals.md#targetdomainstatustype)
- [TaskExecutionStatusType](./literals.md#taskexecutionstatustype)
- [UserRoleType](./literals.md#userroletype)
- [SecurityAgentServiceName](./literals.md#securityagentservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
- [VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- [AuthenticationTypeDef](./type_defs.md#authenticationtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AgentSpaceSummaryTypeDef](./type_defs.md#agentspacesummarytypedef)
- [CodeReviewSettingsTypeDef](./type_defs.md#codereviewsettingstypedef)
- [ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef)
- [ArtifactMetadataItemTypeDef](./type_defs.md#artifactmetadataitemtypedef)
- [ArtifactSummaryTypeDef](./type_defs.md#artifactsummarytypedef)
- [ArtifactTypeDef](./type_defs.md#artifacttypedef)
- [DocumentInfoTypeDef](./type_defs.md#documentinfotypedef)
- [EndpointTypeDef](./type_defs.md#endpointtypedef)
- [IntegratedRepositoryTypeDef](./type_defs.md#integratedrepositorytypedef)
- [SourceCodeRepositoryTypeDef](./type_defs.md#sourcecoderepositorytypedef)
- [BatchDeletePentestsInputTypeDef](./type_defs.md#batchdeletepentestsinputtypedef)
- [DeletePentestFailureTypeDef](./type_defs.md#deletepentestfailuretypedef)
- [BatchGetAgentSpacesInputTypeDef](./type_defs.md#batchgetagentspacesinputtypedef)
- [BatchGetArtifactMetadataInputTypeDef](./type_defs.md#batchgetartifactmetadatainputtypedef)
- [BatchGetFindingsInputTypeDef](./type_defs.md#batchgetfindingsinputtypedef)
- [BatchGetPentestJobTasksInputTypeDef](./type_defs.md#batchgetpentestjobtasksinputtypedef)
- [BatchGetPentestJobsInputTypeDef](./type_defs.md#batchgetpentestjobsinputtypedef)
- [BatchGetPentestsInputTypeDef](./type_defs.md#batchgetpentestsinputtypedef)
- [BatchGetTargetDomainsInputTypeDef](./type_defs.md#batchgettargetdomainsinputtypedef)
- [CategoryTypeDef](./type_defs.md#categorytypedef)
- [CloudWatchLogTypeDef](./type_defs.md#cloudwatchlogtypedef)
- [CodeRemediationTaskDetailsTypeDef](./type_defs.md#coderemediationtaskdetailstypedef)
- [CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef)
- [CreateTargetDomainInputTypeDef](./type_defs.md#createtargetdomaininputtypedef)
- [CustomHeaderTypeDef](./type_defs.md#customheadertypedef)
- [DeleteAgentSpaceInputTypeDef](./type_defs.md#deleteagentspaceinputtypedef)
- [DeleteApplicationRequestTypeDef](./type_defs.md#deleteapplicationrequesttypedef)
- [DeleteArtifactInputTypeDef](./type_defs.md#deleteartifactinputtypedef)
- [DeleteIntegrationInputTypeDef](./type_defs.md#deleteintegrationinputtypedef)
- [DeleteMembershipRequestTypeDef](./type_defs.md#deletemembershiprequesttypedef)
- [DeleteTargetDomainInputTypeDef](./type_defs.md#deletetargetdomaininputtypedef)
- [DiscoveredEndpointTypeDef](./type_defs.md#discoveredendpointtypedef)
- [DnsVerificationTypeDef](./type_defs.md#dnsverificationtypedef)
- [ErrorInformationTypeDef](./type_defs.md#errorinformationtypedef)
- [ExecutionContextTypeDef](./type_defs.md#executioncontexttypedef)
- [FindingSummaryTypeDef](./type_defs.md#findingsummarytypedef)
- [GetApplicationRequestTypeDef](./type_defs.md#getapplicationrequesttypedef)
- [IdCConfigurationTypeDef](./type_defs.md#idcconfigurationtypedef)
- [GetArtifactInputTypeDef](./type_defs.md#getartifactinputtypedef)
- [GetIntegrationInputTypeDef](./type_defs.md#getintegrationinputtypedef)
- [GitHubIntegrationInputTypeDef](./type_defs.md#githubintegrationinputtypedef)
- [GitHubRepositoryMetadataTypeDef](./type_defs.md#githubrepositorymetadatatypedef)
- [GitHubRepositoryResourceTypeDef](./type_defs.md#githubrepositoryresourcetypedef)
- [GitHubResourceCapabilitiesTypeDef](./type_defs.md#githubresourcecapabilitiestypedef)
- [HttpVerificationTypeDef](./type_defs.md#httpverificationtypedef)
- [InitiateProviderRegistrationInputTypeDef](./type_defs.md#initiateproviderregistrationinputtypedef)
- [IntegrationFilterTypeDef](./type_defs.md#integrationfiltertypedef)
- [IntegrationSummaryTypeDef](./type_defs.md#integrationsummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAgentSpacesInputTypeDef](./type_defs.md#listagentspacesinputtypedef)
- [ListApplicationsRequestTypeDef](./type_defs.md#listapplicationsrequesttypedef)
- [ListArtifactsInputTypeDef](./type_defs.md#listartifactsinputtypedef)
- [ListDiscoveredEndpointsInputTypeDef](./type_defs.md#listdiscoveredendpointsinputtypedef)
- [ListFindingsInputTypeDef](./type_defs.md#listfindingsinputtypedef)
- [ListIntegratedResourcesInputTypeDef](./type_defs.md#listintegratedresourcesinputtypedef)
- [ListMembershipsRequestTypeDef](./type_defs.md#listmembershipsrequesttypedef)
- [ListPentestJobTasksInputTypeDef](./type_defs.md#listpentestjobtasksinputtypedef)
- [TaskSummaryTypeDef](./type_defs.md#tasksummarytypedef)
- [ListPentestJobsForPentestInputTypeDef](./type_defs.md#listpentestjobsforpentestinputtypedef)
- [PentestJobSummaryTypeDef](./type_defs.md#pentestjobsummarytypedef)
- [ListPentestsInputTypeDef](./type_defs.md#listpentestsinputtypedef)
- [PentestSummaryTypeDef](./type_defs.md#pentestsummarytypedef)
- [ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)
- [ListTargetDomainsInputTypeDef](./type_defs.md#listtargetdomainsinputtypedef)
- [TargetDomainSummaryTypeDef](./type_defs.md#targetdomainsummarytypedef)
- [UserMetadataTypeDef](./type_defs.md#usermetadatatypedef)
- [UserConfigTypeDef](./type_defs.md#userconfigtypedef)
- [NetworkTrafficRuleTypeDef](./type_defs.md#networktrafficruletypedef)
- [StepTypeDef](./type_defs.md#steptypedef)
- [StartCodeRemediationInputTypeDef](./type_defs.md#startcoderemediationinputtypedef)
- [StartPentestJobInputTypeDef](./type_defs.md#startpentestjobinputtypedef)
- [StopPentestJobInputTypeDef](./type_defs.md#stoppentestjobinputtypedef)
- [TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)
- [UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)
- [UpdateApplicationRequestTypeDef](./type_defs.md#updateapplicationrequesttypedef)
- [UpdateFindingInputTypeDef](./type_defs.md#updatefindinginputtypedef)
- [UpdateTargetDomainInputTypeDef](./type_defs.md#updatetargetdomaininputtypedef)
- [VerifyTargetDomainInputTypeDef](./type_defs.md#verifytargetdomaininputtypedef)
- [AWSResourcesOutputTypeDef](./type_defs.md#awsresourcesoutputtypedef)
- [AWSResourcesTypeDef](./type_defs.md#awsresourcestypedef)
- [VpcConfigUnionTypeDef](./type_defs.md#vpcconfiguniontypedef)
- [ActorOutputTypeDef](./type_defs.md#actoroutputtypedef)
- [ActorTypeDef](./type_defs.md#actortypedef)
- [AddArtifactInputTypeDef](./type_defs.md#addartifactinputtypedef)
- [AddArtifactOutputTypeDef](./type_defs.md#addartifactoutputtypedef)
- [CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef)
- [CreateIntegrationOutputTypeDef](./type_defs.md#createintegrationoutputtypedef)
- [DeleteAgentSpaceOutputTypeDef](./type_defs.md#deleteagentspaceoutputtypedef)
- [DeleteTargetDomainOutputTypeDef](./type_defs.md#deletetargetdomainoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetIntegrationOutputTypeDef](./type_defs.md#getintegrationoutputtypedef)
- [InitiateProviderRegistrationOutputTypeDef](./type_defs.md#initiateproviderregistrationoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [StartPentestJobOutputTypeDef](./type_defs.md#startpentestjoboutputtypedef)
- [UpdateApplicationResponseTypeDef](./type_defs.md#updateapplicationresponsetypedef)
- [VerifyTargetDomainOutputTypeDef](./type_defs.md#verifytargetdomainoutputtypedef)
- [ListAgentSpacesOutputTypeDef](./type_defs.md#listagentspacesoutputtypedef)
- [ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)
- [BatchGetArtifactMetadataOutputTypeDef](./type_defs.md#batchgetartifactmetadataoutputtypedef)
- [ListArtifactsOutputTypeDef](./type_defs.md#listartifactsoutputtypedef)
- [GetArtifactOutputTypeDef](./type_defs.md#getartifactoutputtypedef)
- [LogLocationTypeDef](./type_defs.md#loglocationtypedef)
- [CodeRemediationTaskTypeDef](./type_defs.md#coderemediationtasktypedef)
- [ListDiscoveredEndpointsOutputTypeDef](./type_defs.md#listdiscoveredendpointsoutputtypedef)
- [ListFindingsOutputTypeDef](./type_defs.md#listfindingsoutputtypedef)
- [GetApplicationResponseTypeDef](./type_defs.md#getapplicationresponsetypedef)
- [ProviderInputTypeDef](./type_defs.md#providerinputtypedef)
- [IntegratedResourceMetadataTypeDef](./type_defs.md#integratedresourcemetadatatypedef)
- [IntegratedResourceTypeDef](./type_defs.md#integratedresourcetypedef)
- [ProviderResourceCapabilitiesTypeDef](./type_defs.md#providerresourcecapabilitiestypedef)
- [VerificationDetailsTypeDef](./type_defs.md#verificationdetailstypedef)
- [ListIntegrationsInputTypeDef](./type_defs.md#listintegrationsinputtypedef)
- [ListIntegrationsOutputTypeDef](./type_defs.md#listintegrationsoutputtypedef)
- [ListAgentSpacesInputPaginateTypeDef](./type_defs.md#listagentspacesinputpaginatetypedef)
- [ListApplicationsRequestPaginateTypeDef](./type_defs.md#listapplicationsrequestpaginatetypedef)
- [ListArtifactsInputPaginateTypeDef](./type_defs.md#listartifactsinputpaginatetypedef)
- [ListDiscoveredEndpointsInputPaginateTypeDef](./type_defs.md#listdiscoveredendpointsinputpaginatetypedef)
- [ListFindingsInputPaginateTypeDef](./type_defs.md#listfindingsinputpaginatetypedef)
- [ListIntegratedResourcesInputPaginateTypeDef](./type_defs.md#listintegratedresourcesinputpaginatetypedef)
- [ListIntegrationsInputPaginateTypeDef](./type_defs.md#listintegrationsinputpaginatetypedef)
- [ListMembershipsRequestPaginateTypeDef](./type_defs.md#listmembershipsrequestpaginatetypedef)
- [ListPentestJobTasksInputPaginateTypeDef](./type_defs.md#listpentestjobtasksinputpaginatetypedef)
- [ListPentestJobsForPentestInputPaginateTypeDef](./type_defs.md#listpentestjobsforpentestinputpaginatetypedef)
- [ListPentestsInputPaginateTypeDef](./type_defs.md#listpentestsinputpaginatetypedef)
- [ListTargetDomainsInputPaginateTypeDef](./type_defs.md#listtargetdomainsinputpaginatetypedef)
- [ListPentestJobTasksOutputTypeDef](./type_defs.md#listpentestjobtasksoutputtypedef)
- [ListPentestJobsForPentestOutputTypeDef](./type_defs.md#listpentestjobsforpentestoutputtypedef)
- [ListPentestsOutputTypeDef](./type_defs.md#listpentestsoutputtypedef)
- [ListTargetDomainsOutputTypeDef](./type_defs.md#listtargetdomainsoutputtypedef)
- [MemberMetadataTypeDef](./type_defs.md#membermetadatatypedef)
- [MembershipConfigTypeDef](./type_defs.md#membershipconfigtypedef)
- [NetworkTrafficConfigOutputTypeDef](./type_defs.md#networktrafficconfigoutputtypedef)
- [NetworkTrafficConfigTypeDef](./type_defs.md#networktrafficconfigtypedef)
- [AgentSpaceTypeDef](./type_defs.md#agentspacetypedef)
- [CreateAgentSpaceOutputTypeDef](./type_defs.md#createagentspaceoutputtypedef)
- [UpdateAgentSpaceOutputTypeDef](./type_defs.md#updateagentspaceoutputtypedef)
- [AWSResourcesUnionTypeDef](./type_defs.md#awsresourcesuniontypedef)
- [AssetsOutputTypeDef](./type_defs.md#assetsoutputtypedef)
- [AssetsTypeDef](./type_defs.md#assetstypedef)
- [TaskTypeDef](./type_defs.md#tasktypedef)
- [FindingTypeDef](./type_defs.md#findingtypedef)
- [CreateIntegrationInputTypeDef](./type_defs.md#createintegrationinputtypedef)
- [IntegratedResourceInputItemTypeDef](./type_defs.md#integratedresourceinputitemtypedef)
- [IntegratedResourceSummaryTypeDef](./type_defs.md#integratedresourcesummarytypedef)
- [CreateTargetDomainOutputTypeDef](./type_defs.md#createtargetdomainoutputtypedef)
- [TargetDomainTypeDef](./type_defs.md#targetdomaintypedef)
- [UpdateTargetDomainOutputTypeDef](./type_defs.md#updatetargetdomainoutputtypedef)
- [CreateMembershipRequestTypeDef](./type_defs.md#createmembershiprequesttypedef)
- [MembershipSummaryTypeDef](./type_defs.md#membershipsummarytypedef)
- [PentestJobTypeDef](./type_defs.md#pentestjobtypedef)
- [NetworkTrafficConfigUnionTypeDef](./type_defs.md#networktrafficconfiguniontypedef)
- [BatchGetAgentSpacesOutputTypeDef](./type_defs.md#batchgetagentspacesoutputtypedef)
- [CreateAgentSpaceInputTypeDef](./type_defs.md#createagentspaceinputtypedef)
- [UpdateAgentSpaceInputTypeDef](./type_defs.md#updateagentspaceinputtypedef)
- [CreatePentestOutputTypeDef](./type_defs.md#createpentestoutputtypedef)
- [PentestTypeDef](./type_defs.md#pentesttypedef)
- [UpdatePentestOutputTypeDef](./type_defs.md#updatepentestoutputtypedef)
- [AssetsUnionTypeDef](./type_defs.md#assetsuniontypedef)
- [BatchGetPentestJobTasksOutputTypeDef](./type_defs.md#batchgetpentestjobtasksoutputtypedef)
- [BatchGetFindingsOutputTypeDef](./type_defs.md#batchgetfindingsoutputtypedef)
- [UpdateIntegratedResourcesInputTypeDef](./type_defs.md#updateintegratedresourcesinputtypedef)
- [ListIntegratedResourcesOutputTypeDef](./type_defs.md#listintegratedresourcesoutputtypedef)
- [BatchGetTargetDomainsOutputTypeDef](./type_defs.md#batchgettargetdomainsoutputtypedef)
- [ListMembershipsResponseTypeDef](./type_defs.md#listmembershipsresponsetypedef)
- [BatchGetPentestJobsOutputTypeDef](./type_defs.md#batchgetpentestjobsoutputtypedef)
- [BatchDeletePentestsOutputTypeDef](./type_defs.md#batchdeletepentestsoutputtypedef)
- [BatchGetPentestsOutputTypeDef](./type_defs.md#batchgetpentestsoutputtypedef)
- [CreatePentestInputTypeDef](./type_defs.md#createpentestinputtypedef)
- [UpdatePentestInputTypeDef](./type_defs.md#updatepentestinputtypedef)

