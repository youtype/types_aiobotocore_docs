# EMRContainers module

> [Index](../README.md) > EMRContainers


!!! note ""

    Auto-generated documentation for [EMRContainers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#emrcontainers)
    type annotations stubs module [types-aiobotocore-emr-containers](https://pypi.org/project/types-aiobotocore-emr-containers/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `EMRContainers` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `EMRContainers` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[emr-containers]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[emr-containers]'

# standalone installation
python -m pip install types-aiobotocore-emr-containers
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-emr-containers
```

## Usage

Code samples can be found in [Examples](./usage.md).

## EMRContainersClient

Type annotations and code completion for  `#!python session.create_client("emr-containers")` as [EMRContainersClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client)

```python
# EMRContainersClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.client import EMRContainersClient


session = get_session()
async with session.create_client("emr-containers") as client:
    client: EMRContainersClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("emr-containers").get_paginator("...")`.

```python
# ListJobRunsPaginator usage example

from types_aiobotocore_emr_containers.paginator import ListJobRunsPaginator

def get_list_job_runs_paginator() -> ListJobRunsPaginator:
    return client.get_paginator("list_job_runs"))
```

- [ListJobRunsPaginator](./paginators.md#listjobrunspaginator)
- [ListJobTemplatesPaginator](./paginators.md#listjobtemplatespaginator)
- [ListManagedEndpointsPaginator](./paginators.md#listmanagedendpointspaginator)
- [ListSecurityConfigurationsPaginator](./paginators.md#listsecurityconfigurationspaginator)
- [ListVirtualClustersPaginator](./paginators.md#listvirtualclusterspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CertificateProviderTypeType usage example

from types_aiobotocore_emr_containers.literals import CertificateProviderTypeType

def get_value() -> CertificateProviderTypeType:
    return "PEM"
```

- [CertificateProviderTypeType](./literals.md#certificateprovidertypetype)
- [ContainerProviderTypeType](./literals.md#containerprovidertypetype)
- [EndpointStateType](./literals.md#endpointstatetype)
- [FailureReasonType](./literals.md#failurereasontype)
- [JobRunStateType](./literals.md#jobrunstatetype)
- [ListJobRunsPaginatorName](./literals.md#listjobrunspaginatorname)
- [ListJobTemplatesPaginatorName](./literals.md#listjobtemplatespaginatorname)
- [ListManagedEndpointsPaginatorName](./literals.md#listmanagedendpointspaginatorname)
- [ListSecurityConfigurationsPaginatorName](./literals.md#listsecurityconfigurationspaginatorname)
- [ListVirtualClustersPaginatorName](./literals.md#listvirtualclusterspaginatorname)
- [PersistentAppUIType](./literals.md#persistentappuitype)
- [TemplateParameterDataTypeType](./literals.md#templateparameterdatatypetype)
- [VirtualClusterStateType](./literals.md#virtualclusterstatetype)
- [EMRContainersServiceName](./literals.md#emrcontainersservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CancelJobRunRequestRequestTypeDef](./type_defs.md#canceljobrunrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CertificateTypeDef](./type_defs.md#certificatetypedef)
- [CloudWatchMonitoringConfigurationTypeDef](./type_defs.md#cloudwatchmonitoringconfigurationtypedef)
- [ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef)
- [ConfigurationPaginatorTypeDef](./type_defs.md#configurationpaginatortypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [EksInfoTypeDef](./type_defs.md#eksinfotypedef)
- [ContainerLogRotationConfigurationTypeDef](./type_defs.md#containerlogrotationconfigurationtypedef)
- [CredentialsTypeDef](./type_defs.md#credentialstypedef)
- [DeleteJobTemplateRequestRequestTypeDef](./type_defs.md#deletejobtemplaterequestrequesttypedef)
- [DeleteManagedEndpointRequestRequestTypeDef](./type_defs.md#deletemanagedendpointrequestrequesttypedef)
- [DeleteVirtualClusterRequestRequestTypeDef](./type_defs.md#deletevirtualclusterrequestrequesttypedef)
- [DescribeJobRunRequestRequestTypeDef](./type_defs.md#describejobrunrequestrequesttypedef)
- [DescribeJobTemplateRequestRequestTypeDef](./type_defs.md#describejobtemplaterequestrequesttypedef)
- [DescribeManagedEndpointRequestRequestTypeDef](./type_defs.md#describemanagedendpointrequestrequesttypedef)
- [DescribeSecurityConfigurationRequestRequestTypeDef](./type_defs.md#describesecurityconfigurationrequestrequesttypedef)
- [DescribeVirtualClusterRequestRequestTypeDef](./type_defs.md#describevirtualclusterrequestrequesttypedef)
- [GetManagedEndpointSessionCredentialsRequestRequestTypeDef](./type_defs.md#getmanagedendpointsessioncredentialsrequestrequesttypedef)
- [TLSCertificateConfigurationTypeDef](./type_defs.md#tlscertificateconfigurationtypedef)
- [SparkSqlJobDriverTypeDef](./type_defs.md#sparksqljobdrivertypedef)
- [SparkSubmitJobDriverOutputTypeDef](./type_defs.md#sparksubmitjobdriveroutputtypedef)
- [RetryPolicyConfigurationTypeDef](./type_defs.md#retrypolicyconfigurationtypedef)
- [RetryPolicyExecutionTypeDef](./type_defs.md#retrypolicyexecutiontypedef)
- [TemplateParameterConfigurationTypeDef](./type_defs.md#templateparameterconfigurationtypedef)
- [SecureNamespaceInfoTypeDef](./type_defs.md#securenamespaceinfotypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [S3MonitoringConfigurationTypeDef](./type_defs.md#s3monitoringconfigurationtypedef)
- [ParametricCloudWatchMonitoringConfigurationTypeDef](./type_defs.md#parametriccloudwatchmonitoringconfigurationtypedef)
- [ParametricS3MonitoringConfigurationTypeDef](./type_defs.md#parametrics3monitoringconfigurationtypedef)
- [SparkSubmitJobDriverTypeDef](./type_defs.md#sparksubmitjobdrivertypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [CancelJobRunResponseTypeDef](./type_defs.md#canceljobrunresponsetypedef)
- [CreateJobTemplateResponseTypeDef](./type_defs.md#createjobtemplateresponsetypedef)
- [CreateManagedEndpointResponseTypeDef](./type_defs.md#createmanagedendpointresponsetypedef)
- [CreateSecurityConfigurationResponseTypeDef](./type_defs.md#createsecurityconfigurationresponsetypedef)
- [CreateVirtualClusterResponseTypeDef](./type_defs.md#createvirtualclusterresponsetypedef)
- [DeleteJobTemplateResponseTypeDef](./type_defs.md#deletejobtemplateresponsetypedef)
- [DeleteManagedEndpointResponseTypeDef](./type_defs.md#deletemanagedendpointresponsetypedef)
- [DeleteVirtualClusterResponseTypeDef](./type_defs.md#deletevirtualclusterresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartJobRunResponseTypeDef](./type_defs.md#startjobrunresponsetypedef)
- [ConfigurationUnionTypeDef](./type_defs.md#configurationuniontypedef)
- [ContainerInfoTypeDef](./type_defs.md#containerinfotypedef)
- [GetManagedEndpointSessionCredentialsResponseTypeDef](./type_defs.md#getmanagedendpointsessioncredentialsresponsetypedef)
- [InTransitEncryptionConfigurationTypeDef](./type_defs.md#intransitencryptionconfigurationtypedef)
- [JobDriverOutputTypeDef](./type_defs.md#jobdriveroutputtypedef)
- [LakeFormationConfigurationTypeDef](./type_defs.md#lakeformationconfigurationtypedef)
- [ListJobRunsRequestListJobRunsPaginateTypeDef](./type_defs.md#listjobrunsrequestlistjobrunspaginatetypedef)
- [ListJobRunsRequestRequestTypeDef](./type_defs.md#listjobrunsrequestrequesttypedef)
- [ListJobTemplatesRequestListJobTemplatesPaginateTypeDef](./type_defs.md#listjobtemplatesrequestlistjobtemplatespaginatetypedef)
- [ListJobTemplatesRequestRequestTypeDef](./type_defs.md#listjobtemplatesrequestrequesttypedef)
- [ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef](./type_defs.md#listmanagedendpointsrequestlistmanagedendpointspaginatetypedef)
- [ListManagedEndpointsRequestRequestTypeDef](./type_defs.md#listmanagedendpointsrequestrequesttypedef)
- [ListSecurityConfigurationsRequestListSecurityConfigurationsPaginateTypeDef](./type_defs.md#listsecurityconfigurationsrequestlistsecurityconfigurationspaginatetypedef)
- [ListSecurityConfigurationsRequestRequestTypeDef](./type_defs.md#listsecurityconfigurationsrequestrequesttypedef)
- [ListVirtualClustersRequestListVirtualClustersPaginateTypeDef](./type_defs.md#listvirtualclustersrequestlistvirtualclusterspaginatetypedef)
- [ListVirtualClustersRequestRequestTypeDef](./type_defs.md#listvirtualclustersrequestrequesttypedef)
- [MonitoringConfigurationTypeDef](./type_defs.md#monitoringconfigurationtypedef)
- [ParametricMonitoringConfigurationTypeDef](./type_defs.md#parametricmonitoringconfigurationtypedef)
- [SparkSubmitJobDriverUnionTypeDef](./type_defs.md#sparksubmitjobdriveruniontypedef)
- [ContainerProviderTypeDef](./type_defs.md#containerprovidertypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [ConfigurationOverridesOutputTypeDef](./type_defs.md#configurationoverridesoutputtypedef)
- [ConfigurationOverridesPaginatorTypeDef](./type_defs.md#configurationoverridespaginatortypedef)
- [ConfigurationOverridesTypeDef](./type_defs.md#configurationoverridestypedef)
- [ParametricConfigurationOverridesOutputTypeDef](./type_defs.md#parametricconfigurationoverridesoutputtypedef)
- [ParametricConfigurationOverridesPaginatorTypeDef](./type_defs.md#parametricconfigurationoverridespaginatortypedef)
- [ParametricConfigurationOverridesTypeDef](./type_defs.md#parametricconfigurationoverridestypedef)
- [JobDriverTypeDef](./type_defs.md#jobdrivertypedef)
- [CreateVirtualClusterRequestRequestTypeDef](./type_defs.md#createvirtualclusterrequestrequesttypedef)
- [VirtualClusterTypeDef](./type_defs.md#virtualclustertypedef)
- [AuthorizationConfigurationTypeDef](./type_defs.md#authorizationconfigurationtypedef)
- [EndpointTypeDef](./type_defs.md#endpointtypedef)
- [JobRunTypeDef](./type_defs.md#jobruntypedef)
- [EndpointPaginatorTypeDef](./type_defs.md#endpointpaginatortypedef)
- [JobRunPaginatorTypeDef](./type_defs.md#jobrunpaginatortypedef)
- [CreateManagedEndpointRequestRequestTypeDef](./type_defs.md#createmanagedendpointrequestrequesttypedef)
- [JobTemplateDataOutputTypeDef](./type_defs.md#jobtemplatedataoutputtypedef)
- [JobTemplateDataPaginatorTypeDef](./type_defs.md#jobtemplatedatapaginatortypedef)
- [ParametricConfigurationOverridesUnionTypeDef](./type_defs.md#parametricconfigurationoverridesuniontypedef)
- [JobDriverUnionTypeDef](./type_defs.md#jobdriveruniontypedef)
- [StartJobRunRequestRequestTypeDef](./type_defs.md#startjobrunrequestrequesttypedef)
- [DescribeVirtualClusterResponseTypeDef](./type_defs.md#describevirtualclusterresponsetypedef)
- [ListVirtualClustersResponseTypeDef](./type_defs.md#listvirtualclustersresponsetypedef)
- [SecurityConfigurationDataTypeDef](./type_defs.md#securityconfigurationdatatypedef)
- [DescribeManagedEndpointResponseTypeDef](./type_defs.md#describemanagedendpointresponsetypedef)
- [ListManagedEndpointsResponseTypeDef](./type_defs.md#listmanagedendpointsresponsetypedef)
- [DescribeJobRunResponseTypeDef](./type_defs.md#describejobrunresponsetypedef)
- [ListJobRunsResponseTypeDef](./type_defs.md#listjobrunsresponsetypedef)
- [ListManagedEndpointsResponsePaginatorTypeDef](./type_defs.md#listmanagedendpointsresponsepaginatortypedef)
- [ListJobRunsResponsePaginatorTypeDef](./type_defs.md#listjobrunsresponsepaginatortypedef)
- [JobTemplateTypeDef](./type_defs.md#jobtemplatetypedef)
- [JobTemplatePaginatorTypeDef](./type_defs.md#jobtemplatepaginatortypedef)
- [JobTemplateDataTypeDef](./type_defs.md#jobtemplatedatatypedef)
- [CreateSecurityConfigurationRequestRequestTypeDef](./type_defs.md#createsecurityconfigurationrequestrequesttypedef)
- [SecurityConfigurationTypeDef](./type_defs.md#securityconfigurationtypedef)
- [DescribeJobTemplateResponseTypeDef](./type_defs.md#describejobtemplateresponsetypedef)
- [ListJobTemplatesResponseTypeDef](./type_defs.md#listjobtemplatesresponsetypedef)
- [ListJobTemplatesResponsePaginatorTypeDef](./type_defs.md#listjobtemplatesresponsepaginatortypedef)
- [CreateJobTemplateRequestRequestTypeDef](./type_defs.md#createjobtemplaterequestrequesttypedef)
- [DescribeSecurityConfigurationResponseTypeDef](./type_defs.md#describesecurityconfigurationresponsetypedef)
- [ListSecurityConfigurationsResponseTypeDef](./type_defs.md#listsecurityconfigurationsresponsetypedef)

