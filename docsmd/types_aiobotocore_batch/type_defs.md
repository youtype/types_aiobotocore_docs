# Type definitions

> [Index](../README.md) > [Batch](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Batch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
    type annotations stubs module [types-aiobotocore-batch](https://pypi.org/project/types-aiobotocore-batch/).



## ArrayPropertiesDetailTypeDef

```python
# ArrayPropertiesDetailTypeDef definition

class ArrayPropertiesDetailTypeDef(TypedDict):
    statusSummary: NotRequired[Dict[str, int]],
    size: NotRequired[int],
    index: NotRequired[int],
```

## ArrayPropertiesSummaryTypeDef

```python
# ArrayPropertiesSummaryTypeDef definition

class ArrayPropertiesSummaryTypeDef(TypedDict):
    size: NotRequired[int],
    index: NotRequired[int],
```

## ArrayPropertiesTypeDef

```python
# ArrayPropertiesTypeDef definition

class ArrayPropertiesTypeDef(TypedDict):
    size: NotRequired[int],
```

## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    attachmentId: NotRequired[str],
    ipv6Address: NotRequired[str],
    privateIpv4Address: NotRequired[str],
```

## CancelJobRequestRequestTypeDef

```python
# CancelJobRequestRequestTypeDef definition

class CancelJobRequestRequestTypeDef(TypedDict):
    jobId: str,
    reason: str,
```

## EksConfigurationTypeDef

```python
# EksConfigurationTypeDef definition

class EksConfigurationTypeDef(TypedDict):
    eksClusterArn: str,
    kubernetesNamespace: str,
```

## UpdatePolicyTypeDef

```python
# UpdatePolicyTypeDef definition

class UpdatePolicyTypeDef(TypedDict):
    terminateJobsOnUpdate: NotRequired[bool],
    jobExecutionTimeoutMinutes: NotRequired[int],
```

## ComputeEnvironmentOrderTypeDef

```python
# ComputeEnvironmentOrderTypeDef definition

class ComputeEnvironmentOrderTypeDef(TypedDict):
    order: int,
    computeEnvironment: str,
```

## Ec2ConfigurationTypeDef

```python
# Ec2ConfigurationTypeDef definition

class Ec2ConfigurationTypeDef(TypedDict):
    imageType: str,
    imageIdOverride: NotRequired[str],
    imageKubernetesVersion: NotRequired[str],
```

## LaunchTemplateSpecificationTypeDef

```python
# LaunchTemplateSpecificationTypeDef definition

class LaunchTemplateSpecificationTypeDef(TypedDict):
    launchTemplateId: NotRequired[str],
    launchTemplateName: NotRequired[str],
    version: NotRequired[str],
```

## EphemeralStorageTypeDef

```python
# EphemeralStorageTypeDef definition

class EphemeralStorageTypeDef(TypedDict):
    sizeInGiB: int,
```

## FargatePlatformConfigurationTypeDef

```python
# FargatePlatformConfigurationTypeDef definition

class FargatePlatformConfigurationTypeDef(TypedDict):
    platformVersion: NotRequired[str],
```

## KeyValuePairTypeDef

```python
# KeyValuePairTypeDef definition

class KeyValuePairTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[str],
```

## MountPointTypeDef

```python
# MountPointTypeDef definition

class MountPointTypeDef(TypedDict):
    containerPath: NotRequired[str],
    readOnly: NotRequired[bool],
    sourceVolume: NotRequired[str],
```

## NetworkConfigurationTypeDef

```python
# NetworkConfigurationTypeDef definition

class NetworkConfigurationTypeDef(TypedDict):
    assignPublicIp: NotRequired[AssignPublicIpType],  # (1)
```

1. See [:material-code-brackets: AssignPublicIpType](./literals.md#assignpubliciptype) 
## ResourceRequirementTypeDef

```python
# ResourceRequirementTypeDef definition

class ResourceRequirementTypeDef(TypedDict):
    value: str,
    type: ResourceTypeType,  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## RuntimePlatformTypeDef

```python
# RuntimePlatformTypeDef definition

class RuntimePlatformTypeDef(TypedDict):
    operatingSystemFamily: NotRequired[str],
    cpuArchitecture: NotRequired[str],
```

## SecretTypeDef

```python
# SecretTypeDef definition

class SecretTypeDef(TypedDict):
    name: str,
    valueFrom: str,
```

## UlimitTypeDef

```python
# UlimitTypeDef definition

class UlimitTypeDef(TypedDict):
    hardLimit: int,
    name: str,
    softLimit: int,
```

## ContainerSummaryTypeDef

```python
# ContainerSummaryTypeDef definition

class ContainerSummaryTypeDef(TypedDict):
    exitCode: NotRequired[int],
    reason: NotRequired[str],
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

## DeleteComputeEnvironmentRequestRequestTypeDef

```python
# DeleteComputeEnvironmentRequestRequestTypeDef definition

class DeleteComputeEnvironmentRequestRequestTypeDef(TypedDict):
    computeEnvironment: str,
```

## DeleteJobQueueRequestRequestTypeDef

```python
# DeleteJobQueueRequestRequestTypeDef definition

class DeleteJobQueueRequestRequestTypeDef(TypedDict):
    jobQueue: str,
```

## DeleteSchedulingPolicyRequestRequestTypeDef

```python
# DeleteSchedulingPolicyRequestRequestTypeDef definition

class DeleteSchedulingPolicyRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeregisterJobDefinitionRequestRequestTypeDef

```python
# DeregisterJobDefinitionRequestRequestTypeDef definition

class DeregisterJobDefinitionRequestRequestTypeDef(TypedDict):
    jobDefinition: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeComputeEnvironmentsRequestRequestTypeDef

```python
# DescribeComputeEnvironmentsRequestRequestTypeDef definition

class DescribeComputeEnvironmentsRequestRequestTypeDef(TypedDict):
    computeEnvironments: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## DescribeJobDefinitionsRequestRequestTypeDef

```python
# DescribeJobDefinitionsRequestRequestTypeDef definition

class DescribeJobDefinitionsRequestRequestTypeDef(TypedDict):
    jobDefinitions: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    jobDefinitionName: NotRequired[str],
    status: NotRequired[str],
    nextToken: NotRequired[str],
```

## DescribeJobQueuesRequestRequestTypeDef

```python
# DescribeJobQueuesRequestRequestTypeDef definition

class DescribeJobQueuesRequestRequestTypeDef(TypedDict):
    jobQueues: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## DescribeJobsRequestRequestTypeDef

```python
# DescribeJobsRequestRequestTypeDef definition

class DescribeJobsRequestRequestTypeDef(TypedDict):
    jobs: Sequence[str],
```

## DescribeSchedulingPoliciesRequestRequestTypeDef

```python
# DescribeSchedulingPoliciesRequestRequestTypeDef definition

class DescribeSchedulingPoliciesRequestRequestTypeDef(TypedDict):
    arns: Sequence[str],
```

## DeviceTypeDef

```python
# DeviceTypeDef definition

class DeviceTypeDef(TypedDict):
    hostPath: str,
    containerPath: NotRequired[str],
    permissions: NotRequired[List[DeviceCgroupPermissionType]],  # (1)
```

1. See [:material-code-brackets: DeviceCgroupPermissionType](./literals.md#devicecgrouppermissiontype) 
## EFSAuthorizationConfigTypeDef

```python
# EFSAuthorizationConfigTypeDef definition

class EFSAuthorizationConfigTypeDef(TypedDict):
    accessPointId: NotRequired[str],
    iam: NotRequired[EFSAuthorizationConfigIAMType],  # (1)
```

1. See [:material-code-brackets: EFSAuthorizationConfigIAMType](./literals.md#efsauthorizationconfigiamtype) 
## EksAttemptContainerDetailTypeDef

```python
# EksAttemptContainerDetailTypeDef definition

class EksAttemptContainerDetailTypeDef(TypedDict):
    exitCode: NotRequired[int],
    reason: NotRequired[str],
```

## EksContainerEnvironmentVariableTypeDef

```python
# EksContainerEnvironmentVariableTypeDef definition

class EksContainerEnvironmentVariableTypeDef(TypedDict):
    name: str,
    value: NotRequired[str],
```

## EksContainerResourceRequirementsTypeDef

```python
# EksContainerResourceRequirementsTypeDef definition

class EksContainerResourceRequirementsTypeDef(TypedDict):
    limits: NotRequired[Dict[str, str]],
    requests: NotRequired[Dict[str, str]],
```

## EksContainerSecurityContextTypeDef

```python
# EksContainerSecurityContextTypeDef definition

class EksContainerSecurityContextTypeDef(TypedDict):
    runAsUser: NotRequired[int],
    runAsGroup: NotRequired[int],
    privileged: NotRequired[bool],
    readOnlyRootFilesystem: NotRequired[bool],
    runAsNonRoot: NotRequired[bool],
```

## EksContainerVolumeMountTypeDef

```python
# EksContainerVolumeMountTypeDef definition

class EksContainerVolumeMountTypeDef(TypedDict):
    name: NotRequired[str],
    mountPath: NotRequired[str],
    readOnly: NotRequired[bool],
```

## EksEmptyDirTypeDef

```python
# EksEmptyDirTypeDef definition

class EksEmptyDirTypeDef(TypedDict):
    medium: NotRequired[str],
    sizeLimit: NotRequired[str],
```

## EksHostPathTypeDef

```python
# EksHostPathTypeDef definition

class EksHostPathTypeDef(TypedDict):
    path: NotRequired[str],
```

## EksMetadataTypeDef

```python
# EksMetadataTypeDef definition

class EksMetadataTypeDef(TypedDict):
    labels: NotRequired[Dict[str, str]],
```

## EksSecretTypeDef

```python
# EksSecretTypeDef definition

class EksSecretTypeDef(TypedDict):
    secretName: str,
    optional: NotRequired[bool],
```

## EvaluateOnExitTypeDef

```python
# EvaluateOnExitTypeDef definition

class EvaluateOnExitTypeDef(TypedDict):
    action: RetryActionType,  # (1)
    onStatusReason: NotRequired[str],
    onReason: NotRequired[str],
    onExitCode: NotRequired[str],
```

1. See [:material-code-brackets: RetryActionType](./literals.md#retryactiontype) 
## ShareAttributesTypeDef

```python
# ShareAttributesTypeDef definition

class ShareAttributesTypeDef(TypedDict):
    shareIdentifier: str,
    weightFactor: NotRequired[float],
```

## HostTypeDef

```python
# HostTypeDef definition

class HostTypeDef(TypedDict):
    sourcePath: NotRequired[str],
```

## JobTimeoutTypeDef

```python
# JobTimeoutTypeDef definition

class JobTimeoutTypeDef(TypedDict):
    attemptDurationSeconds: NotRequired[int],
```

## JobDependencyTypeDef

```python
# JobDependencyTypeDef definition

class JobDependencyTypeDef(TypedDict):
    jobId: NotRequired[str],
    type: NotRequired[ArrayJobDependencyType],  # (1)
```

1. See [:material-code-brackets: ArrayJobDependencyType](./literals.md#arrayjobdependencytype) 
## NodeDetailsTypeDef

```python
# NodeDetailsTypeDef definition

class NodeDetailsTypeDef(TypedDict):
    nodeIndex: NotRequired[int],
    isMainNode: NotRequired[bool],
```

## NodePropertiesSummaryTypeDef

```python
# NodePropertiesSummaryTypeDef definition

class NodePropertiesSummaryTypeDef(TypedDict):
    isMainNode: NotRequired[bool],
    numNodes: NotRequired[int],
    nodeIndex: NotRequired[int],
```

## KeyValuesPairTypeDef

```python
# KeyValuesPairTypeDef definition

class KeyValuesPairTypeDef(TypedDict):
    name: NotRequired[str],
    values: NotRequired[Sequence[str]],
```

## TmpfsTypeDef

```python
# TmpfsTypeDef definition

class TmpfsTypeDef(TypedDict):
    containerPath: str,
    size: int,
    mountOptions: NotRequired[List[str]],
```

## ListSchedulingPoliciesRequestRequestTypeDef

```python
# ListSchedulingPoliciesRequestRequestTypeDef definition

class ListSchedulingPoliciesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## SchedulingPolicyListingDetailTypeDef

```python
# SchedulingPolicyListingDetailTypeDef definition

class SchedulingPolicyListingDetailTypeDef(TypedDict):
    arn: str,
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TerminateJobRequestRequestTypeDef

```python
# TerminateJobRequestRequestTypeDef definition

class TerminateJobRequestRequestTypeDef(TypedDict):
    jobId: str,
    reason: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## AttemptContainerDetailTypeDef

```python
# AttemptContainerDetailTypeDef definition

class AttemptContainerDetailTypeDef(TypedDict):
    containerInstanceArn: NotRequired[str],
    taskArn: NotRequired[str],
    exitCode: NotRequired[int],
    reason: NotRequired[str],
    logStreamName: NotRequired[str],
    networkInterfaces: NotRequired[List[NetworkInterfaceTypeDef]],  # (1)
```

1. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
## CreateJobQueueRequestRequestTypeDef

```python
# CreateJobQueueRequestRequestTypeDef definition

class CreateJobQueueRequestRequestTypeDef(TypedDict):
    jobQueueName: str,
    priority: int,
    computeEnvironmentOrder: Sequence[ComputeEnvironmentOrderTypeDef],  # (1)
    state: NotRequired[JQStateType],  # (2)
    schedulingPolicyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ComputeEnvironmentOrderTypeDef](./type_defs.md#computeenvironmentordertypedef) 
2. See [:material-code-brackets: JQStateType](./literals.md#jqstatetype) 
## JobQueueDetailTypeDef

```python
# JobQueueDetailTypeDef definition

class JobQueueDetailTypeDef(TypedDict):
    jobQueueName: str,
    jobQueueArn: str,
    state: JQStateType,  # (1)
    priority: int,
    computeEnvironmentOrder: List[ComputeEnvironmentOrderTypeDef],  # (3)
    schedulingPolicyArn: NotRequired[str],
    status: NotRequired[JQStatusType],  # (2)
    statusReason: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: JQStateType](./literals.md#jqstatetype) 
2. See [:material-code-brackets: JQStatusType](./literals.md#jqstatustype) 
3. See [:material-code-braces: ComputeEnvironmentOrderTypeDef](./type_defs.md#computeenvironmentordertypedef) 
## UpdateJobQueueRequestRequestTypeDef

```python
# UpdateJobQueueRequestRequestTypeDef definition

class UpdateJobQueueRequestRequestTypeDef(TypedDict):
    jobQueue: str,
    state: NotRequired[JQStateType],  # (1)
    schedulingPolicyArn: NotRequired[str],
    priority: NotRequired[int],
    computeEnvironmentOrder: NotRequired[Sequence[ComputeEnvironmentOrderTypeDef]],  # (2)
```

1. See [:material-code-brackets: JQStateType](./literals.md#jqstatetype) 
2. See [:material-code-braces: ComputeEnvironmentOrderTypeDef](./type_defs.md#computeenvironmentordertypedef) 
## ComputeResourceTypeDef

```python
# ComputeResourceTypeDef definition

class ComputeResourceTypeDef(TypedDict):
    type: CRTypeType,  # (1)
    maxvCpus: int,
    subnets: Sequence[str],
    allocationStrategy: NotRequired[CRAllocationStrategyType],  # (2)
    minvCpus: NotRequired[int],
    desiredvCpus: NotRequired[int],
    instanceTypes: NotRequired[Sequence[str]],
    imageId: NotRequired[str],
    securityGroupIds: NotRequired[Sequence[str]],
    ec2KeyPair: NotRequired[str],
    instanceRole: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    placementGroup: NotRequired[str],
    bidPercentage: NotRequired[int],
    spotIamFleetRole: NotRequired[str],
    launchTemplate: NotRequired[LaunchTemplateSpecificationTypeDef],  # (3)
    ec2Configuration: NotRequired[Sequence[Ec2ConfigurationTypeDef]],  # (4)
```

1. See [:material-code-brackets: CRTypeType](./literals.md#crtypetype) 
2. See [:material-code-brackets: CRAllocationStrategyType](./literals.md#crallocationstrategytype) 
3. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
4. See [:material-code-braces: Ec2ConfigurationTypeDef](./type_defs.md#ec2configurationtypedef) 
## ComputeResourceUpdateTypeDef

```python
# ComputeResourceUpdateTypeDef definition

class ComputeResourceUpdateTypeDef(TypedDict):
    minvCpus: NotRequired[int],
    maxvCpus: NotRequired[int],
    desiredvCpus: NotRequired[int],
    subnets: NotRequired[Sequence[str]],
    securityGroupIds: NotRequired[Sequence[str]],
    allocationStrategy: NotRequired[CRUpdateAllocationStrategyType],  # (1)
    instanceTypes: NotRequired[Sequence[str]],
    ec2KeyPair: NotRequired[str],
    instanceRole: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    placementGroup: NotRequired[str],
    bidPercentage: NotRequired[int],
    launchTemplate: NotRequired[LaunchTemplateSpecificationTypeDef],  # (2)
    ec2Configuration: NotRequired[Sequence[Ec2ConfigurationTypeDef]],  # (3)
    updateToLatestImageVersion: NotRequired[bool],
    type: NotRequired[CRTypeType],  # (4)
    imageId: NotRequired[str],
```

1. See [:material-code-brackets: CRUpdateAllocationStrategyType](./literals.md#crupdateallocationstrategytype) 
2. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
3. See [:material-code-braces: Ec2ConfigurationTypeDef](./type_defs.md#ec2configurationtypedef) 
4. See [:material-code-brackets: CRTypeType](./literals.md#crtypetype) 
## ContainerOverridesTypeDef

```python
# ContainerOverridesTypeDef definition

class ContainerOverridesTypeDef(TypedDict):
    vcpus: NotRequired[int],
    memory: NotRequired[int],
    command: NotRequired[Sequence[str]],
    instanceType: NotRequired[str],
    environment: NotRequired[Sequence[KeyValuePairTypeDef]],  # (1)
    resourceRequirements: NotRequired[Sequence[ResourceRequirementTypeDef]],  # (2)
```

1. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
2. See [:material-code-braces: ResourceRequirementTypeDef](./type_defs.md#resourcerequirementtypedef) 
## LogConfigurationTypeDef

```python
# LogConfigurationTypeDef definition

class LogConfigurationTypeDef(TypedDict):
    logDriver: LogDriverType,  # (1)
    options: NotRequired[Dict[str, str]],
    secretOptions: NotRequired[List[SecretTypeDef]],  # (2)
```

1. See [:material-code-brackets: LogDriverType](./literals.md#logdrivertype) 
2. See [:material-code-braces: SecretTypeDef](./type_defs.md#secrettypedef) 
## CreateComputeEnvironmentResponseTypeDef

```python
# CreateComputeEnvironmentResponseTypeDef definition

class CreateComputeEnvironmentResponseTypeDef(TypedDict):
    computeEnvironmentName: str,
    computeEnvironmentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobQueueResponseTypeDef

```python
# CreateJobQueueResponseTypeDef definition

class CreateJobQueueResponseTypeDef(TypedDict):
    jobQueueName: str,
    jobQueueArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSchedulingPolicyResponseTypeDef

```python
# CreateSchedulingPolicyResponseTypeDef definition

class CreateSchedulingPolicyResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterJobDefinitionResponseTypeDef

```python
# RegisterJobDefinitionResponseTypeDef definition

class RegisterJobDefinitionResponseTypeDef(TypedDict):
    jobDefinitionName: str,
    jobDefinitionArn: str,
    revision: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubmitJobResponseTypeDef

```python
# SubmitJobResponseTypeDef definition

class SubmitJobResponseTypeDef(TypedDict):
    jobArn: str,
    jobName: str,
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateComputeEnvironmentResponseTypeDef

```python
# UpdateComputeEnvironmentResponseTypeDef definition

class UpdateComputeEnvironmentResponseTypeDef(TypedDict):
    computeEnvironmentName: str,
    computeEnvironmentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateJobQueueResponseTypeDef

```python
# UpdateJobQueueResponseTypeDef definition

class UpdateJobQueueResponseTypeDef(TypedDict):
    jobQueueName: str,
    jobQueueArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef

```python
# DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef definition

class DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef(TypedDict):
    computeEnvironments: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef

```python
# DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef definition

class DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef(TypedDict):
    jobDefinitions: NotRequired[Sequence[str]],
    jobDefinitionName: NotRequired[str],
    status: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef

```python
# DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef definition

class DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef(TypedDict):
    jobQueues: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef

```python
# ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef definition

class ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## EFSVolumeConfigurationTypeDef

```python
# EFSVolumeConfigurationTypeDef definition

class EFSVolumeConfigurationTypeDef(TypedDict):
    fileSystemId: str,
    rootDirectory: NotRequired[str],
    transitEncryption: NotRequired[EFSTransitEncryptionType],  # (1)
    transitEncryptionPort: NotRequired[int],
    authorizationConfig: NotRequired[EFSAuthorizationConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: EFSTransitEncryptionType](./literals.md#efstransitencryptiontype) 
2. See [:material-code-braces: EFSAuthorizationConfigTypeDef](./type_defs.md#efsauthorizationconfigtypedef) 
## EksAttemptDetailTypeDef

```python
# EksAttemptDetailTypeDef definition

class EksAttemptDetailTypeDef(TypedDict):
    containers: NotRequired[List[EksAttemptContainerDetailTypeDef]],  # (1)
    podName: NotRequired[str],
    nodeName: NotRequired[str],
    startedAt: NotRequired[int],
    stoppedAt: NotRequired[int],
    statusReason: NotRequired[str],
```

1. See [:material-code-braces: EksAttemptContainerDetailTypeDef](./type_defs.md#eksattemptcontainerdetailtypedef) 
## EksContainerOverrideTypeDef

```python
# EksContainerOverrideTypeDef definition

class EksContainerOverrideTypeDef(TypedDict):
    image: NotRequired[str],
    command: NotRequired[Sequence[str]],
    args: NotRequired[Sequence[str]],
    env: NotRequired[Sequence[EksContainerEnvironmentVariableTypeDef]],  # (1)
    resources: NotRequired[EksContainerResourceRequirementsTypeDef],  # (2)
```

1. See [:material-code-braces: EksContainerEnvironmentVariableTypeDef](./type_defs.md#ekscontainerenvironmentvariabletypedef) 
2. See [:material-code-braces: EksContainerResourceRequirementsTypeDef](./type_defs.md#ekscontainerresourcerequirementstypedef) 
## EksContainerDetailTypeDef

```python
# EksContainerDetailTypeDef definition

class EksContainerDetailTypeDef(TypedDict):
    name: NotRequired[str],
    image: NotRequired[str],
    imagePullPolicy: NotRequired[str],
    command: NotRequired[List[str]],
    args: NotRequired[List[str]],
    env: NotRequired[List[EksContainerEnvironmentVariableTypeDef]],  # (1)
    resources: NotRequired[EksContainerResourceRequirementsTypeDef],  # (2)
    exitCode: NotRequired[int],
    reason: NotRequired[str],
    volumeMounts: NotRequired[List[EksContainerVolumeMountTypeDef]],  # (3)
    securityContext: NotRequired[EksContainerSecurityContextTypeDef],  # (4)
```

1. See [:material-code-braces: EksContainerEnvironmentVariableTypeDef](./type_defs.md#ekscontainerenvironmentvariabletypedef) 
2. See [:material-code-braces: EksContainerResourceRequirementsTypeDef](./type_defs.md#ekscontainerresourcerequirementstypedef) 
3. See [:material-code-braces: EksContainerVolumeMountTypeDef](./type_defs.md#ekscontainervolumemounttypedef) 
4. See [:material-code-braces: EksContainerSecurityContextTypeDef](./type_defs.md#ekscontainersecuritycontexttypedef) 
## EksContainerTypeDef

```python
# EksContainerTypeDef definition

class EksContainerTypeDef(TypedDict):
    image: str,
    name: NotRequired[str],
    imagePullPolicy: NotRequired[str],
    command: NotRequired[List[str]],
    args: NotRequired[List[str]],
    env: NotRequired[List[EksContainerEnvironmentVariableTypeDef]],  # (1)
    resources: NotRequired[EksContainerResourceRequirementsTypeDef],  # (2)
    volumeMounts: NotRequired[List[EksContainerVolumeMountTypeDef]],  # (3)
    securityContext: NotRequired[EksContainerSecurityContextTypeDef],  # (4)
```

1. See [:material-code-braces: EksContainerEnvironmentVariableTypeDef](./type_defs.md#ekscontainerenvironmentvariabletypedef) 
2. See [:material-code-braces: EksContainerResourceRequirementsTypeDef](./type_defs.md#ekscontainerresourcerequirementstypedef) 
3. See [:material-code-braces: EksContainerVolumeMountTypeDef](./type_defs.md#ekscontainervolumemounttypedef) 
4. See [:material-code-braces: EksContainerSecurityContextTypeDef](./type_defs.md#ekscontainersecuritycontexttypedef) 
## EksVolumeTypeDef

```python
# EksVolumeTypeDef definition

class EksVolumeTypeDef(TypedDict):
    name: str,
    hostPath: NotRequired[EksHostPathTypeDef],  # (1)
    emptyDir: NotRequired[EksEmptyDirTypeDef],  # (2)
    secret: NotRequired[EksSecretTypeDef],  # (3)
```

1. See [:material-code-braces: EksHostPathTypeDef](./type_defs.md#ekshostpathtypedef) 
2. See [:material-code-braces: EksEmptyDirTypeDef](./type_defs.md#eksemptydirtypedef) 
3. See [:material-code-braces: EksSecretTypeDef](./type_defs.md#ekssecrettypedef) 
## RetryStrategyTypeDef

```python
# RetryStrategyTypeDef definition

class RetryStrategyTypeDef(TypedDict):
    attempts: NotRequired[int],
    evaluateOnExit: NotRequired[List[EvaluateOnExitTypeDef]],  # (1)
```

1. See [:material-code-braces: EvaluateOnExitTypeDef](./type_defs.md#evaluateonexittypedef) 
## FairsharePolicyTypeDef

```python
# FairsharePolicyTypeDef definition

class FairsharePolicyTypeDef(TypedDict):
    shareDecaySeconds: NotRequired[int],
    computeReservation: NotRequired[int],
    shareDistribution: NotRequired[Sequence[ShareAttributesTypeDef]],  # (1)
```

1. See [:material-code-braces: ShareAttributesTypeDef](./type_defs.md#shareattributestypedef) 
## JobSummaryTypeDef

```python
# JobSummaryTypeDef definition

class JobSummaryTypeDef(TypedDict):
    jobId: str,
    jobName: str,
    jobArn: NotRequired[str],
    createdAt: NotRequired[int],
    status: NotRequired[JobStatusType],  # (1)
    statusReason: NotRequired[str],
    startedAt: NotRequired[int],
    stoppedAt: NotRequired[int],
    container: NotRequired[ContainerSummaryTypeDef],  # (2)
    arrayProperties: NotRequired[ArrayPropertiesSummaryTypeDef],  # (3)
    nodeProperties: NotRequired[NodePropertiesSummaryTypeDef],  # (4)
    jobDefinition: NotRequired[str],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ContainerSummaryTypeDef](./type_defs.md#containersummarytypedef) 
3. See [:material-code-braces: ArrayPropertiesSummaryTypeDef](./type_defs.md#arraypropertiessummarytypedef) 
4. See [:material-code-braces: NodePropertiesSummaryTypeDef](./type_defs.md#nodepropertiessummarytypedef) 
## ListJobsRequestListJobsPaginateTypeDef

```python
# ListJobsRequestListJobsPaginateTypeDef definition

class ListJobsRequestListJobsPaginateTypeDef(TypedDict):
    jobQueue: NotRequired[str],
    arrayJobId: NotRequired[str],
    multiNodeJobId: NotRequired[str],
    jobStatus: NotRequired[JobStatusType],  # (1)
    filters: NotRequired[Sequence[KeyValuesPairTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: KeyValuesPairTypeDef](./type_defs.md#keyvaluespairtypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsRequestRequestTypeDef

```python
# ListJobsRequestRequestTypeDef definition

class ListJobsRequestRequestTypeDef(TypedDict):
    jobQueue: NotRequired[str],
    arrayJobId: NotRequired[str],
    multiNodeJobId: NotRequired[str],
    jobStatus: NotRequired[JobStatusType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filters: NotRequired[Sequence[KeyValuesPairTypeDef]],  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: KeyValuesPairTypeDef](./type_defs.md#keyvaluespairtypedef) 
## LinuxParametersTypeDef

```python
# LinuxParametersTypeDef definition

class LinuxParametersTypeDef(TypedDict):
    devices: NotRequired[List[DeviceTypeDef]],  # (1)
    initProcessEnabled: NotRequired[bool],
    sharedMemorySize: NotRequired[int],
    tmpfs: NotRequired[List[TmpfsTypeDef]],  # (2)
    maxSwap: NotRequired[int],
    swappiness: NotRequired[int],
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
2. See [:material-code-braces: TmpfsTypeDef](./type_defs.md#tmpfstypedef) 
## ListSchedulingPoliciesResponseTypeDef

```python
# ListSchedulingPoliciesResponseTypeDef definition

class ListSchedulingPoliciesResponseTypeDef(TypedDict):
    schedulingPolicies: List[SchedulingPolicyListingDetailTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchedulingPolicyListingDetailTypeDef](./type_defs.md#schedulingpolicylistingdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttemptDetailTypeDef

```python
# AttemptDetailTypeDef definition

class AttemptDetailTypeDef(TypedDict):
    container: NotRequired[AttemptContainerDetailTypeDef],  # (1)
    startedAt: NotRequired[int],
    stoppedAt: NotRequired[int],
    statusReason: NotRequired[str],
```

1. See [:material-code-braces: AttemptContainerDetailTypeDef](./type_defs.md#attemptcontainerdetailtypedef) 
## DescribeJobQueuesResponseTypeDef

```python
# DescribeJobQueuesResponseTypeDef definition

class DescribeJobQueuesResponseTypeDef(TypedDict):
    jobQueues: List[JobQueueDetailTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobQueueDetailTypeDef](./type_defs.md#jobqueuedetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ComputeEnvironmentDetailTypeDef

```python
# ComputeEnvironmentDetailTypeDef definition

class ComputeEnvironmentDetailTypeDef(TypedDict):
    computeEnvironmentName: str,
    computeEnvironmentArn: str,
    unmanagedvCpus: NotRequired[int],
    ecsClusterArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    type: NotRequired[CETypeType],  # (1)
    state: NotRequired[CEStateType],  # (2)
    status: NotRequired[CEStatusType],  # (3)
    statusReason: NotRequired[str],
    computeResources: NotRequired[ComputeResourceTypeDef],  # (4)
    serviceRole: NotRequired[str],
    updatePolicy: NotRequired[UpdatePolicyTypeDef],  # (5)
    eksConfiguration: NotRequired[EksConfigurationTypeDef],  # (6)
    containerOrchestrationType: NotRequired[OrchestrationTypeType],  # (7)
    uuid: NotRequired[str],
```

1. See [:material-code-brackets: CETypeType](./literals.md#cetypetype) 
2. See [:material-code-brackets: CEStateType](./literals.md#cestatetype) 
3. See [:material-code-brackets: CEStatusType](./literals.md#cestatustype) 
4. See [:material-code-braces: ComputeResourceTypeDef](./type_defs.md#computeresourcetypedef) 
5. See [:material-code-braces: UpdatePolicyTypeDef](./type_defs.md#updatepolicytypedef) 
6. See [:material-code-braces: EksConfigurationTypeDef](./type_defs.md#eksconfigurationtypedef) 
7. See [:material-code-brackets: OrchestrationTypeType](./literals.md#orchestrationtypetype) 
## CreateComputeEnvironmentRequestRequestTypeDef

```python
# CreateComputeEnvironmentRequestRequestTypeDef definition

class CreateComputeEnvironmentRequestRequestTypeDef(TypedDict):
    computeEnvironmentName: str,
    type: CETypeType,  # (1)
    state: NotRequired[CEStateType],  # (2)
    unmanagedvCpus: NotRequired[int],
    computeResources: NotRequired[ComputeResourceTypeDef],  # (3)
    serviceRole: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    eksConfiguration: NotRequired[EksConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: CETypeType](./literals.md#cetypetype) 
2. See [:material-code-brackets: CEStateType](./literals.md#cestatetype) 
3. See [:material-code-braces: ComputeResourceTypeDef](./type_defs.md#computeresourcetypedef) 
4. See [:material-code-braces: EksConfigurationTypeDef](./type_defs.md#eksconfigurationtypedef) 
## UpdateComputeEnvironmentRequestRequestTypeDef

```python
# UpdateComputeEnvironmentRequestRequestTypeDef definition

class UpdateComputeEnvironmentRequestRequestTypeDef(TypedDict):
    computeEnvironment: str,
    state: NotRequired[CEStateType],  # (1)
    unmanagedvCpus: NotRequired[int],
    computeResources: NotRequired[ComputeResourceUpdateTypeDef],  # (2)
    serviceRole: NotRequired[str],
    updatePolicy: NotRequired[UpdatePolicyTypeDef],  # (3)
```

1. See [:material-code-brackets: CEStateType](./literals.md#cestatetype) 
2. See [:material-code-braces: ComputeResourceUpdateTypeDef](./type_defs.md#computeresourceupdatetypedef) 
3. See [:material-code-braces: UpdatePolicyTypeDef](./type_defs.md#updatepolicytypedef) 
## NodePropertyOverrideTypeDef

```python
# NodePropertyOverrideTypeDef definition

class NodePropertyOverrideTypeDef(TypedDict):
    targetNodes: str,
    containerOverrides: NotRequired[ContainerOverridesTypeDef],  # (1)
```

1. See [:material-code-braces: ContainerOverridesTypeDef](./type_defs.md#containeroverridestypedef) 
## VolumeTypeDef

```python
# VolumeTypeDef definition

class VolumeTypeDef(TypedDict):
    host: NotRequired[HostTypeDef],  # (1)
    name: NotRequired[str],
    efsVolumeConfiguration: NotRequired[EFSVolumeConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: HostTypeDef](./type_defs.md#hosttypedef) 
2. See [:material-code-braces: EFSVolumeConfigurationTypeDef](./type_defs.md#efsvolumeconfigurationtypedef) 
## EksPodPropertiesOverrideTypeDef

```python
# EksPodPropertiesOverrideTypeDef definition

class EksPodPropertiesOverrideTypeDef(TypedDict):
    containers: NotRequired[Sequence[EksContainerOverrideTypeDef]],  # (1)
    metadata: NotRequired[EksMetadataTypeDef],  # (2)
```

1. See [:material-code-braces: EksContainerOverrideTypeDef](./type_defs.md#ekscontaineroverridetypedef) 
2. See [:material-code-braces: EksMetadataTypeDef](./type_defs.md#eksmetadatatypedef) 
## EksPodPropertiesDetailTypeDef

```python
# EksPodPropertiesDetailTypeDef definition

class EksPodPropertiesDetailTypeDef(TypedDict):
    serviceAccountName: NotRequired[str],
    hostNetwork: NotRequired[bool],
    dnsPolicy: NotRequired[str],
    containers: NotRequired[List[EksContainerDetailTypeDef]],  # (1)
    volumes: NotRequired[List[EksVolumeTypeDef]],  # (2)
    podName: NotRequired[str],
    nodeName: NotRequired[str],
    metadata: NotRequired[EksMetadataTypeDef],  # (3)
```

1. See [:material-code-braces: EksContainerDetailTypeDef](./type_defs.md#ekscontainerdetailtypedef) 
2. See [:material-code-braces: EksVolumeTypeDef](./type_defs.md#eksvolumetypedef) 
3. See [:material-code-braces: EksMetadataTypeDef](./type_defs.md#eksmetadatatypedef) 
## EksPodPropertiesTypeDef

```python
# EksPodPropertiesTypeDef definition

class EksPodPropertiesTypeDef(TypedDict):
    serviceAccountName: NotRequired[str],
    hostNetwork: NotRequired[bool],
    dnsPolicy: NotRequired[str],
    containers: NotRequired[List[EksContainerTypeDef]],  # (1)
    volumes: NotRequired[List[EksVolumeTypeDef]],  # (2)
    metadata: NotRequired[EksMetadataTypeDef],  # (3)
```

1. See [:material-code-braces: EksContainerTypeDef](./type_defs.md#ekscontainertypedef) 
2. See [:material-code-braces: EksVolumeTypeDef](./type_defs.md#eksvolumetypedef) 
3. See [:material-code-braces: EksMetadataTypeDef](./type_defs.md#eksmetadatatypedef) 
## CreateSchedulingPolicyRequestRequestTypeDef

```python
# CreateSchedulingPolicyRequestRequestTypeDef definition

class CreateSchedulingPolicyRequestRequestTypeDef(TypedDict):
    name: str,
    fairsharePolicy: NotRequired[FairsharePolicyTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FairsharePolicyTypeDef](./type_defs.md#fairsharepolicytypedef) 
## SchedulingPolicyDetailTypeDef

```python
# SchedulingPolicyDetailTypeDef definition

class SchedulingPolicyDetailTypeDef(TypedDict):
    name: str,
    arn: str,
    fairsharePolicy: NotRequired[FairsharePolicyTypeDef],  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: FairsharePolicyTypeDef](./type_defs.md#fairsharepolicytypedef) 
## UpdateSchedulingPolicyRequestRequestTypeDef

```python
# UpdateSchedulingPolicyRequestRequestTypeDef definition

class UpdateSchedulingPolicyRequestRequestTypeDef(TypedDict):
    arn: str,
    fairsharePolicy: NotRequired[FairsharePolicyTypeDef],  # (1)
```

1. See [:material-code-braces: FairsharePolicyTypeDef](./type_defs.md#fairsharepolicytypedef) 
## ListJobsResponseTypeDef

```python
# ListJobsResponseTypeDef definition

class ListJobsResponseTypeDef(TypedDict):
    jobSummaryList: List[JobSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeComputeEnvironmentsResponseTypeDef

```python
# DescribeComputeEnvironmentsResponseTypeDef definition

class DescribeComputeEnvironmentsResponseTypeDef(TypedDict):
    computeEnvironments: List[ComputeEnvironmentDetailTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComputeEnvironmentDetailTypeDef](./type_defs.md#computeenvironmentdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NodeOverridesTypeDef

```python
# NodeOverridesTypeDef definition

class NodeOverridesTypeDef(TypedDict):
    numNodes: NotRequired[int],
    nodePropertyOverrides: NotRequired[Sequence[NodePropertyOverrideTypeDef]],  # (1)
```

1. See [:material-code-braces: NodePropertyOverrideTypeDef](./type_defs.md#nodepropertyoverridetypedef) 
## ContainerDetailTypeDef

```python
# ContainerDetailTypeDef definition

class ContainerDetailTypeDef(TypedDict):
    image: NotRequired[str],
    vcpus: NotRequired[int],
    memory: NotRequired[int],
    command: NotRequired[List[str]],
    jobRoleArn: NotRequired[str],
    executionRoleArn: NotRequired[str],
    volumes: NotRequired[List[VolumeTypeDef]],  # (1)
    environment: NotRequired[List[KeyValuePairTypeDef]],  # (2)
    mountPoints: NotRequired[List[MountPointTypeDef]],  # (3)
    readonlyRootFilesystem: NotRequired[bool],
    ulimits: NotRequired[List[UlimitTypeDef]],  # (4)
    privileged: NotRequired[bool],
    user: NotRequired[str],
    exitCode: NotRequired[int],
    reason: NotRequired[str],
    containerInstanceArn: NotRequired[str],
    taskArn: NotRequired[str],
    logStreamName: NotRequired[str],
    instanceType: NotRequired[str],
    networkInterfaces: NotRequired[List[NetworkInterfaceTypeDef]],  # (5)
    resourceRequirements: NotRequired[List[ResourceRequirementTypeDef]],  # (6)
    linuxParameters: NotRequired[LinuxParametersTypeDef],  # (7)
    logConfiguration: NotRequired[LogConfigurationTypeDef],  # (8)
    secrets: NotRequired[List[SecretTypeDef]],  # (9)
    networkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (10)
    fargatePlatformConfiguration: NotRequired[FargatePlatformConfigurationTypeDef],  # (11)
    ephemeralStorage: NotRequired[EphemeralStorageTypeDef],  # (12)
    runtimePlatform: NotRequired[RuntimePlatformTypeDef],  # (13)
```

1. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
2. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
3. See [:material-code-braces: MountPointTypeDef](./type_defs.md#mountpointtypedef) 
4. See [:material-code-braces: UlimitTypeDef](./type_defs.md#ulimittypedef) 
5. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
6. See [:material-code-braces: ResourceRequirementTypeDef](./type_defs.md#resourcerequirementtypedef) 
7. See [:material-code-braces: LinuxParametersTypeDef](./type_defs.md#linuxparameterstypedef) 
8. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
9. See [:material-code-braces: SecretTypeDef](./type_defs.md#secrettypedef) 
10. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
11. See [:material-code-braces: FargatePlatformConfigurationTypeDef](./type_defs.md#fargateplatformconfigurationtypedef) 
12. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
13. See [:material-code-braces: RuntimePlatformTypeDef](./type_defs.md#runtimeplatformtypedef) 
## ContainerPropertiesTypeDef

```python
# ContainerPropertiesTypeDef definition

class ContainerPropertiesTypeDef(TypedDict):
    image: NotRequired[str],
    vcpus: NotRequired[int],
    memory: NotRequired[int],
    command: NotRequired[List[str]],
    jobRoleArn: NotRequired[str],
    executionRoleArn: NotRequired[str],
    volumes: NotRequired[List[VolumeTypeDef]],  # (1)
    environment: NotRequired[List[KeyValuePairTypeDef]],  # (2)
    mountPoints: NotRequired[List[MountPointTypeDef]],  # (3)
    readonlyRootFilesystem: NotRequired[bool],
    privileged: NotRequired[bool],
    ulimits: NotRequired[List[UlimitTypeDef]],  # (4)
    user: NotRequired[str],
    instanceType: NotRequired[str],
    resourceRequirements: NotRequired[List[ResourceRequirementTypeDef]],  # (5)
    linuxParameters: NotRequired[LinuxParametersTypeDef],  # (6)
    logConfiguration: NotRequired[LogConfigurationTypeDef],  # (7)
    secrets: NotRequired[List[SecretTypeDef]],  # (8)
    networkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (9)
    fargatePlatformConfiguration: NotRequired[FargatePlatformConfigurationTypeDef],  # (10)
    ephemeralStorage: NotRequired[EphemeralStorageTypeDef],  # (11)
    runtimePlatform: NotRequired[RuntimePlatformTypeDef],  # (12)
```

1. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
2. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
3. See [:material-code-braces: MountPointTypeDef](./type_defs.md#mountpointtypedef) 
4. See [:material-code-braces: UlimitTypeDef](./type_defs.md#ulimittypedef) 
5. See [:material-code-braces: ResourceRequirementTypeDef](./type_defs.md#resourcerequirementtypedef) 
6. See [:material-code-braces: LinuxParametersTypeDef](./type_defs.md#linuxparameterstypedef) 
7. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
8. See [:material-code-braces: SecretTypeDef](./type_defs.md#secrettypedef) 
9. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
10. See [:material-code-braces: FargatePlatformConfigurationTypeDef](./type_defs.md#fargateplatformconfigurationtypedef) 
11. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
12. See [:material-code-braces: RuntimePlatformTypeDef](./type_defs.md#runtimeplatformtypedef) 
## EksPropertiesOverrideTypeDef

```python
# EksPropertiesOverrideTypeDef definition

class EksPropertiesOverrideTypeDef(TypedDict):
    podProperties: NotRequired[EksPodPropertiesOverrideTypeDef],  # (1)
```

1. See [:material-code-braces: EksPodPropertiesOverrideTypeDef](./type_defs.md#ekspodpropertiesoverridetypedef) 
## EksPropertiesDetailTypeDef

```python
# EksPropertiesDetailTypeDef definition

class EksPropertiesDetailTypeDef(TypedDict):
    podProperties: NotRequired[EksPodPropertiesDetailTypeDef],  # (1)
```

1. See [:material-code-braces: EksPodPropertiesDetailTypeDef](./type_defs.md#ekspodpropertiesdetailtypedef) 
## EksPropertiesTypeDef

```python
# EksPropertiesTypeDef definition

class EksPropertiesTypeDef(TypedDict):
    podProperties: NotRequired[EksPodPropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: EksPodPropertiesTypeDef](./type_defs.md#ekspodpropertiestypedef) 
## DescribeSchedulingPoliciesResponseTypeDef

```python
# DescribeSchedulingPoliciesResponseTypeDef definition

class DescribeSchedulingPoliciesResponseTypeDef(TypedDict):
    schedulingPolicies: List[SchedulingPolicyDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchedulingPolicyDetailTypeDef](./type_defs.md#schedulingpolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NodeRangePropertyTypeDef

```python
# NodeRangePropertyTypeDef definition

class NodeRangePropertyTypeDef(TypedDict):
    targetNodes: str,
    container: NotRequired[ContainerPropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: ContainerPropertiesTypeDef](./type_defs.md#containerpropertiestypedef) 
## SubmitJobRequestRequestTypeDef

```python
# SubmitJobRequestRequestTypeDef definition

class SubmitJobRequestRequestTypeDef(TypedDict):
    jobName: str,
    jobQueue: str,
    jobDefinition: str,
    shareIdentifier: NotRequired[str],
    schedulingPriorityOverride: NotRequired[int],
    arrayProperties: NotRequired[ArrayPropertiesTypeDef],  # (1)
    dependsOn: NotRequired[Sequence[JobDependencyTypeDef]],  # (2)
    parameters: NotRequired[Mapping[str, str]],
    containerOverrides: NotRequired[ContainerOverridesTypeDef],  # (3)
    nodeOverrides: NotRequired[NodeOverridesTypeDef],  # (4)
    retryStrategy: NotRequired[RetryStrategyTypeDef],  # (5)
    propagateTags: NotRequired[bool],
    timeout: NotRequired[JobTimeoutTypeDef],  # (6)
    tags: NotRequired[Mapping[str, str]],
    eksPropertiesOverride: NotRequired[EksPropertiesOverrideTypeDef],  # (7)
```

1. See [:material-code-braces: ArrayPropertiesTypeDef](./type_defs.md#arraypropertiestypedef) 
2. See [:material-code-braces: JobDependencyTypeDef](./type_defs.md#jobdependencytypedef) 
3. See [:material-code-braces: ContainerOverridesTypeDef](./type_defs.md#containeroverridestypedef) 
4. See [:material-code-braces: NodeOverridesTypeDef](./type_defs.md#nodeoverridestypedef) 
5. See [:material-code-braces: RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef) 
6. See [:material-code-braces: JobTimeoutTypeDef](./type_defs.md#jobtimeouttypedef) 
7. See [:material-code-braces: EksPropertiesOverrideTypeDef](./type_defs.md#ekspropertiesoverridetypedef) 
## NodePropertiesTypeDef

```python
# NodePropertiesTypeDef definition

class NodePropertiesTypeDef(TypedDict):
    numNodes: int,
    mainNode: int,
    nodeRangeProperties: List[NodeRangePropertyTypeDef],  # (1)
```

1. See [:material-code-braces: NodeRangePropertyTypeDef](./type_defs.md#noderangepropertytypedef) 
## JobDefinitionTypeDef

```python
# JobDefinitionTypeDef definition

class JobDefinitionTypeDef(TypedDict):
    jobDefinitionName: str,
    jobDefinitionArn: str,
    revision: int,
    type: str,
    status: NotRequired[str],
    schedulingPriority: NotRequired[int],
    parameters: NotRequired[Dict[str, str]],
    retryStrategy: NotRequired[RetryStrategyTypeDef],  # (1)
    containerProperties: NotRequired[ContainerPropertiesTypeDef],  # (2)
    timeout: NotRequired[JobTimeoutTypeDef],  # (3)
    nodeProperties: NotRequired[NodePropertiesTypeDef],  # (4)
    tags: NotRequired[Dict[str, str]],
    propagateTags: NotRequired[bool],
    platformCapabilities: NotRequired[List[PlatformCapabilityType]],  # (5)
    eksProperties: NotRequired[EksPropertiesTypeDef],  # (6)
    containerOrchestrationType: NotRequired[OrchestrationTypeType],  # (7)
```

1. See [:material-code-braces: RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef) 
2. See [:material-code-braces: ContainerPropertiesTypeDef](./type_defs.md#containerpropertiestypedef) 
3. See [:material-code-braces: JobTimeoutTypeDef](./type_defs.md#jobtimeouttypedef) 
4. See [:material-code-braces: NodePropertiesTypeDef](./type_defs.md#nodepropertiestypedef) 
5. See [:material-code-brackets: PlatformCapabilityType](./literals.md#platformcapabilitytype) 
6. See [:material-code-braces: EksPropertiesTypeDef](./type_defs.md#ekspropertiestypedef) 
7. See [:material-code-brackets: OrchestrationTypeType](./literals.md#orchestrationtypetype) 
## JobDetailTypeDef

```python
# JobDetailTypeDef definition

class JobDetailTypeDef(TypedDict):
    jobName: str,
    jobId: str,
    jobQueue: str,
    status: JobStatusType,  # (1)
    startedAt: int,
    jobDefinition: str,
    jobArn: NotRequired[str],
    shareIdentifier: NotRequired[str],
    schedulingPriority: NotRequired[int],
    attempts: NotRequired[List[AttemptDetailTypeDef]],  # (2)
    statusReason: NotRequired[str],
    createdAt: NotRequired[int],
    retryStrategy: NotRequired[RetryStrategyTypeDef],  # (3)
    stoppedAt: NotRequired[int],
    dependsOn: NotRequired[List[JobDependencyTypeDef]],  # (4)
    parameters: NotRequired[Dict[str, str]],
    container: NotRequired[ContainerDetailTypeDef],  # (5)
    nodeDetails: NotRequired[NodeDetailsTypeDef],  # (6)
    nodeProperties: NotRequired[NodePropertiesTypeDef],  # (7)
    arrayProperties: NotRequired[ArrayPropertiesDetailTypeDef],  # (8)
    timeout: NotRequired[JobTimeoutTypeDef],  # (9)
    tags: NotRequired[Dict[str, str]],
    propagateTags: NotRequired[bool],
    platformCapabilities: NotRequired[List[PlatformCapabilityType]],  # (10)
    eksProperties: NotRequired[EksPropertiesDetailTypeDef],  # (11)
    eksAttempts: NotRequired[List[EksAttemptDetailTypeDef]],  # (12)
    isCancelled: NotRequired[bool],
    isTerminated: NotRequired[bool],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: AttemptDetailTypeDef](./type_defs.md#attemptdetailtypedef) 
3. See [:material-code-braces: RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef) 
4. See [:material-code-braces: JobDependencyTypeDef](./type_defs.md#jobdependencytypedef) 
5. See [:material-code-braces: ContainerDetailTypeDef](./type_defs.md#containerdetailtypedef) 
6. See [:material-code-braces: NodeDetailsTypeDef](./type_defs.md#nodedetailstypedef) 
7. See [:material-code-braces: NodePropertiesTypeDef](./type_defs.md#nodepropertiestypedef) 
8. See [:material-code-braces: ArrayPropertiesDetailTypeDef](./type_defs.md#arraypropertiesdetailtypedef) 
9. See [:material-code-braces: JobTimeoutTypeDef](./type_defs.md#jobtimeouttypedef) 
10. See [:material-code-brackets: PlatformCapabilityType](./literals.md#platformcapabilitytype) 
11. See [:material-code-braces: EksPropertiesDetailTypeDef](./type_defs.md#ekspropertiesdetailtypedef) 
12. See [:material-code-braces: EksAttemptDetailTypeDef](./type_defs.md#eksattemptdetailtypedef) 
## RegisterJobDefinitionRequestRequestTypeDef

```python
# RegisterJobDefinitionRequestRequestTypeDef definition

class RegisterJobDefinitionRequestRequestTypeDef(TypedDict):
    jobDefinitionName: str,
    type: JobDefinitionTypeType,  # (1)
    parameters: NotRequired[Mapping[str, str]],
    schedulingPriority: NotRequired[int],
    containerProperties: NotRequired[ContainerPropertiesTypeDef],  # (2)
    nodeProperties: NotRequired[NodePropertiesTypeDef],  # (3)
    retryStrategy: NotRequired[RetryStrategyTypeDef],  # (4)
    propagateTags: NotRequired[bool],
    timeout: NotRequired[JobTimeoutTypeDef],  # (5)
    tags: NotRequired[Mapping[str, str]],
    platformCapabilities: NotRequired[Sequence[PlatformCapabilityType]],  # (6)
    eksProperties: NotRequired[EksPropertiesTypeDef],  # (7)
```

1. See [:material-code-brackets: JobDefinitionTypeType](./literals.md#jobdefinitiontypetype) 
2. See [:material-code-braces: ContainerPropertiesTypeDef](./type_defs.md#containerpropertiestypedef) 
3. See [:material-code-braces: NodePropertiesTypeDef](./type_defs.md#nodepropertiestypedef) 
4. See [:material-code-braces: RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef) 
5. See [:material-code-braces: JobTimeoutTypeDef](./type_defs.md#jobtimeouttypedef) 
6. See [:material-code-brackets: PlatformCapabilityType](./literals.md#platformcapabilitytype) 
7. See [:material-code-braces: EksPropertiesTypeDef](./type_defs.md#ekspropertiestypedef) 
## DescribeJobDefinitionsResponseTypeDef

```python
# DescribeJobDefinitionsResponseTypeDef definition

class DescribeJobDefinitionsResponseTypeDef(TypedDict):
    jobDefinitions: List[JobDefinitionTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobDefinitionTypeDef](./type_defs.md#jobdefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeJobsResponseTypeDef

```python
# DescribeJobsResponseTypeDef definition

class DescribeJobsResponseTypeDef(TypedDict):
    jobs: List[JobDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobDetailTypeDef](./type_defs.md#jobdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
