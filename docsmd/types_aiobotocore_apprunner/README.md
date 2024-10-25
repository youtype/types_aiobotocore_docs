# AppRunner module

> [Index](../README.md) > AppRunner


!!! note ""

    Auto-generated documentation for [AppRunner](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
    type annotations stubs module [types-aiobotocore-apprunner](https://pypi.org/project/types-aiobotocore-apprunner/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `AppRunner` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[apprunner]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[apprunner]'


# standalone installation
python -m pip install types-aiobotocore-apprunner
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-apprunner
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AppRunnerClient

Type annotations and code completion for  `#!python session.create_client("apprunner")` as [AppRunnerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client)

```python
# AppRunnerClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_apprunner.client import AppRunnerClient


session = get_session()
async with session.create_client("apprunner") as client:
    client: AppRunnerClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AutoScalingConfigurationStatusType usage example

from types_aiobotocore_apprunner.literals import AutoScalingConfigurationStatusType

def get_value() -> AutoScalingConfigurationStatusType:
    return "ACTIVE"
```

- [AutoScalingConfigurationStatusType](./literals.md#autoscalingconfigurationstatustype)
- [CertificateValidationRecordStatusType](./literals.md#certificatevalidationrecordstatustype)
- [ConfigurationSourceType](./literals.md#configurationsourcetype)
- [ConnectionStatusType](./literals.md#connectionstatustype)
- [CustomDomainAssociationStatusType](./literals.md#customdomainassociationstatustype)
- [EgressTypeType](./literals.md#egresstypetype)
- [HealthCheckProtocolType](./literals.md#healthcheckprotocoltype)
- [ImageRepositoryTypeType](./literals.md#imagerepositorytypetype)
- [IpAddressTypeType](./literals.md#ipaddresstypetype)
- [ObservabilityConfigurationStatusType](./literals.md#observabilityconfigurationstatustype)
- [OperationStatusType](./literals.md#operationstatustype)
- [OperationTypeType](./literals.md#operationtypetype)
- [ProviderTypeType](./literals.md#providertypetype)
- [RuntimeType](./literals.md#runtimetype)
- [ServiceStatusType](./literals.md#servicestatustype)
- [SourceCodeVersionTypeType](./literals.md#sourcecodeversiontypetype)
- [TracingVendorType](./literals.md#tracingvendortype)
- [VpcConnectorStatusType](./literals.md#vpcconnectorstatustype)
- [VpcIngressConnectionStatusType](./literals.md#vpcingressconnectionstatustype)
- [AppRunnerServiceName](./literals.md#apprunnerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AssociateCustomDomainRequestRequestTypeDef](./type_defs.md#associatecustomdomainrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [VpcDNSTargetTypeDef](./type_defs.md#vpcdnstargettypedef)
- [AuthenticationConfigurationTypeDef](./type_defs.md#authenticationconfigurationtypedef)
- [AutoScalingConfigurationSummaryTypeDef](./type_defs.md#autoscalingconfigurationsummarytypedef)
- [AutoScalingConfigurationTypeDef](./type_defs.md#autoscalingconfigurationtypedef)
- [CertificateValidationRecordTypeDef](./type_defs.md#certificatevalidationrecordtypedef)
- [CodeConfigurationValuesOutputTypeDef](./type_defs.md#codeconfigurationvaluesoutputtypedef)
- [CodeConfigurationValuesTypeDef](./type_defs.md#codeconfigurationvaluestypedef)
- [SourceCodeVersionTypeDef](./type_defs.md#sourcecodeversiontypedef)
- [ConnectionSummaryTypeDef](./type_defs.md#connectionsummarytypedef)
- [ConnectionTypeDef](./type_defs.md#connectiontypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [TraceConfigurationTypeDef](./type_defs.md#traceconfigurationtypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [HealthCheckConfigurationTypeDef](./type_defs.md#healthcheckconfigurationtypedef)
- [InstanceConfigurationTypeDef](./type_defs.md#instanceconfigurationtypedef)
- [ServiceObservabilityConfigurationTypeDef](./type_defs.md#serviceobservabilityconfigurationtypedef)
- [VpcConnectorTypeDef](./type_defs.md#vpcconnectortypedef)
- [IngressVpcConfigurationTypeDef](./type_defs.md#ingressvpcconfigurationtypedef)
- [DeleteAutoScalingConfigurationRequestRequestTypeDef](./type_defs.md#deleteautoscalingconfigurationrequestrequesttypedef)
- [DeleteConnectionRequestRequestTypeDef](./type_defs.md#deleteconnectionrequestrequesttypedef)
- [DeleteObservabilityConfigurationRequestRequestTypeDef](./type_defs.md#deleteobservabilityconfigurationrequestrequesttypedef)
- [DeleteServiceRequestRequestTypeDef](./type_defs.md#deleteservicerequestrequesttypedef)
- [DeleteVpcConnectorRequestRequestTypeDef](./type_defs.md#deletevpcconnectorrequestrequesttypedef)
- [DeleteVpcIngressConnectionRequestRequestTypeDef](./type_defs.md#deletevpcingressconnectionrequestrequesttypedef)
- [DescribeAutoScalingConfigurationRequestRequestTypeDef](./type_defs.md#describeautoscalingconfigurationrequestrequesttypedef)
- [DescribeCustomDomainsRequestRequestTypeDef](./type_defs.md#describecustomdomainsrequestrequesttypedef)
- [DescribeObservabilityConfigurationRequestRequestTypeDef](./type_defs.md#describeobservabilityconfigurationrequestrequesttypedef)
- [DescribeServiceRequestRequestTypeDef](./type_defs.md#describeservicerequestrequesttypedef)
- [DescribeVpcConnectorRequestRequestTypeDef](./type_defs.md#describevpcconnectorrequestrequesttypedef)
- [DescribeVpcIngressConnectionRequestRequestTypeDef](./type_defs.md#describevpcingressconnectionrequestrequesttypedef)
- [DisassociateCustomDomainRequestRequestTypeDef](./type_defs.md#disassociatecustomdomainrequestrequesttypedef)
- [EgressConfigurationTypeDef](./type_defs.md#egressconfigurationtypedef)
- [ImageConfigurationOutputTypeDef](./type_defs.md#imageconfigurationoutputtypedef)
- [ImageConfigurationTypeDef](./type_defs.md#imageconfigurationtypedef)
- [IngressConfigurationTypeDef](./type_defs.md#ingressconfigurationtypedef)
- [ListAutoScalingConfigurationsRequestRequestTypeDef](./type_defs.md#listautoscalingconfigurationsrequestrequesttypedef)
- [ListConnectionsRequestRequestTypeDef](./type_defs.md#listconnectionsrequestrequesttypedef)
- [ListObservabilityConfigurationsRequestRequestTypeDef](./type_defs.md#listobservabilityconfigurationsrequestrequesttypedef)
- [ObservabilityConfigurationSummaryTypeDef](./type_defs.md#observabilityconfigurationsummarytypedef)
- [ListOperationsRequestRequestTypeDef](./type_defs.md#listoperationsrequestrequesttypedef)
- [OperationSummaryTypeDef](./type_defs.md#operationsummarytypedef)
- [ListServicesForAutoScalingConfigurationRequestRequestTypeDef](./type_defs.md#listservicesforautoscalingconfigurationrequestrequesttypedef)
- [ListServicesRequestRequestTypeDef](./type_defs.md#listservicesrequestrequesttypedef)
- [ServiceSummaryTypeDef](./type_defs.md#servicesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListVpcConnectorsRequestRequestTypeDef](./type_defs.md#listvpcconnectorsrequestrequesttypedef)
- [ListVpcIngressConnectionsFilterTypeDef](./type_defs.md#listvpcingressconnectionsfiltertypedef)
- [VpcIngressConnectionSummaryTypeDef](./type_defs.md#vpcingressconnectionsummarytypedef)
- [PauseServiceRequestRequestTypeDef](./type_defs.md#pauseservicerequestrequesttypedef)
- [ResumeServiceRequestRequestTypeDef](./type_defs.md#resumeservicerequestrequesttypedef)
- [StartDeploymentRequestRequestTypeDef](./type_defs.md#startdeploymentrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDefaultAutoScalingConfigurationRequestRequestTypeDef](./type_defs.md#updatedefaultautoscalingconfigurationrequestrequesttypedef)
- [ListServicesForAutoScalingConfigurationResponseTypeDef](./type_defs.md#listservicesforautoscalingconfigurationresponsetypedef)
- [StartDeploymentResponseTypeDef](./type_defs.md#startdeploymentresponsetypedef)
- [ListAutoScalingConfigurationsResponseTypeDef](./type_defs.md#listautoscalingconfigurationsresponsetypedef)
- [CreateAutoScalingConfigurationResponseTypeDef](./type_defs.md#createautoscalingconfigurationresponsetypedef)
- [DeleteAutoScalingConfigurationResponseTypeDef](./type_defs.md#deleteautoscalingconfigurationresponsetypedef)
- [DescribeAutoScalingConfigurationResponseTypeDef](./type_defs.md#describeautoscalingconfigurationresponsetypedef)
- [UpdateDefaultAutoScalingConfigurationResponseTypeDef](./type_defs.md#updatedefaultautoscalingconfigurationresponsetypedef)
- [CustomDomainTypeDef](./type_defs.md#customdomaintypedef)
- [CodeConfigurationOutputTypeDef](./type_defs.md#codeconfigurationoutputtypedef)
- [CodeConfigurationValuesUnionTypeDef](./type_defs.md#codeconfigurationvaluesuniontypedef)
- [ListConnectionsResponseTypeDef](./type_defs.md#listconnectionsresponsetypedef)
- [CreateConnectionResponseTypeDef](./type_defs.md#createconnectionresponsetypedef)
- [DeleteConnectionResponseTypeDef](./type_defs.md#deleteconnectionresponsetypedef)
- [CreateAutoScalingConfigurationRequestRequestTypeDef](./type_defs.md#createautoscalingconfigurationrequestrequesttypedef)
- [CreateConnectionRequestRequestTypeDef](./type_defs.md#createconnectionrequestrequesttypedef)
- [CreateVpcConnectorRequestRequestTypeDef](./type_defs.md#createvpcconnectorrequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateObservabilityConfigurationRequestRequestTypeDef](./type_defs.md#createobservabilityconfigurationrequestrequesttypedef)
- [ObservabilityConfigurationTypeDef](./type_defs.md#observabilityconfigurationtypedef)
- [CreateVpcConnectorResponseTypeDef](./type_defs.md#createvpcconnectorresponsetypedef)
- [DeleteVpcConnectorResponseTypeDef](./type_defs.md#deletevpcconnectorresponsetypedef)
- [DescribeVpcConnectorResponseTypeDef](./type_defs.md#describevpcconnectorresponsetypedef)
- [ListVpcConnectorsResponseTypeDef](./type_defs.md#listvpcconnectorsresponsetypedef)
- [CreateVpcIngressConnectionRequestRequestTypeDef](./type_defs.md#createvpcingressconnectionrequestrequesttypedef)
- [UpdateVpcIngressConnectionRequestRequestTypeDef](./type_defs.md#updatevpcingressconnectionrequestrequesttypedef)
- [VpcIngressConnectionTypeDef](./type_defs.md#vpcingressconnectiontypedef)
- [ImageRepositoryOutputTypeDef](./type_defs.md#imagerepositoryoutputtypedef)
- [ImageConfigurationUnionTypeDef](./type_defs.md#imageconfigurationuniontypedef)
- [NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef)
- [ListObservabilityConfigurationsResponseTypeDef](./type_defs.md#listobservabilityconfigurationsresponsetypedef)
- [ListOperationsResponseTypeDef](./type_defs.md#listoperationsresponsetypedef)
- [ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef)
- [ListVpcIngressConnectionsRequestRequestTypeDef](./type_defs.md#listvpcingressconnectionsrequestrequesttypedef)
- [ListVpcIngressConnectionsResponseTypeDef](./type_defs.md#listvpcingressconnectionsresponsetypedef)
- [AssociateCustomDomainResponseTypeDef](./type_defs.md#associatecustomdomainresponsetypedef)
- [DescribeCustomDomainsResponseTypeDef](./type_defs.md#describecustomdomainsresponsetypedef)
- [DisassociateCustomDomainResponseTypeDef](./type_defs.md#disassociatecustomdomainresponsetypedef)
- [CodeRepositoryOutputTypeDef](./type_defs.md#coderepositoryoutputtypedef)
- [CodeConfigurationTypeDef](./type_defs.md#codeconfigurationtypedef)
- [CreateObservabilityConfigurationResponseTypeDef](./type_defs.md#createobservabilityconfigurationresponsetypedef)
- [DeleteObservabilityConfigurationResponseTypeDef](./type_defs.md#deleteobservabilityconfigurationresponsetypedef)
- [DescribeObservabilityConfigurationResponseTypeDef](./type_defs.md#describeobservabilityconfigurationresponsetypedef)
- [CreateVpcIngressConnectionResponseTypeDef](./type_defs.md#createvpcingressconnectionresponsetypedef)
- [DeleteVpcIngressConnectionResponseTypeDef](./type_defs.md#deletevpcingressconnectionresponsetypedef)
- [DescribeVpcIngressConnectionResponseTypeDef](./type_defs.md#describevpcingressconnectionresponsetypedef)
- [UpdateVpcIngressConnectionResponseTypeDef](./type_defs.md#updatevpcingressconnectionresponsetypedef)
- [ImageRepositoryTypeDef](./type_defs.md#imagerepositorytypedef)
- [SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef)
- [CodeConfigurationUnionTypeDef](./type_defs.md#codeconfigurationuniontypedef)
- [ImageRepositoryUnionTypeDef](./type_defs.md#imagerepositoryuniontypedef)
- [ServiceTypeDef](./type_defs.md#servicetypedef)
- [CodeRepositoryTypeDef](./type_defs.md#coderepositorytypedef)
- [CreateServiceResponseTypeDef](./type_defs.md#createserviceresponsetypedef)
- [DeleteServiceResponseTypeDef](./type_defs.md#deleteserviceresponsetypedef)
- [DescribeServiceResponseTypeDef](./type_defs.md#describeserviceresponsetypedef)
- [PauseServiceResponseTypeDef](./type_defs.md#pauseserviceresponsetypedef)
- [ResumeServiceResponseTypeDef](./type_defs.md#resumeserviceresponsetypedef)
- [UpdateServiceResponseTypeDef](./type_defs.md#updateserviceresponsetypedef)
- [CodeRepositoryUnionTypeDef](./type_defs.md#coderepositoryuniontypedef)
- [SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef)
- [CreateServiceRequestRequestTypeDef](./type_defs.md#createservicerequestrequesttypedef)
- [UpdateServiceRequestRequestTypeDef](./type_defs.md#updateservicerequestrequesttypedef)

