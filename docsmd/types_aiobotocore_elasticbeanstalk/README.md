# ElasticBeanstalk module

> [Index](../README.md) > ElasticBeanstalk


!!! note ""

    Auto-generated documentation for [ElasticBeanstalk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#elasticbeanstalk)
    type annotations stubs module [types-aiobotocore-elasticbeanstalk](https://pypi.org/project/types-aiobotocore-elasticbeanstalk/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ElasticBeanstalk` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ElasticBeanstalk` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[elasticbeanstalk]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[elasticbeanstalk]'

# standalone installation
python -m pip install types-aiobotocore-elasticbeanstalk
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-elasticbeanstalk
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ElasticBeanstalkClient

Type annotations and code completion for  `#!python session.create_client("elasticbeanstalk")` as [ElasticBeanstalkClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client)

```python
# ElasticBeanstalkClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticbeanstalk.client import ElasticBeanstalkClient


session = get_session()
async with session.create_client("elasticbeanstalk") as client:
    client: ElasticBeanstalkClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("elasticbeanstalk").get_paginator("...")`.

```python
# DescribeApplicationVersionsPaginator usage example

from types_aiobotocore_elasticbeanstalk.paginator import DescribeApplicationVersionsPaginator

def get_describe_application_versions_paginator() -> DescribeApplicationVersionsPaginator:
    return client.get_paginator("describe_application_versions"))
```

- [DescribeApplicationVersionsPaginator](./paginators.md#describeapplicationversionspaginator)
- [DescribeEnvironmentManagedActionHistoryPaginator](./paginators.md#describeenvironmentmanagedactionhistorypaginator)
- [DescribeEnvironmentsPaginator](./paginators.md#describeenvironmentspaginator)
- [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
- [ListPlatformVersionsPaginator](./paginators.md#listplatformversionspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("elasticbeanstalk").get_waiter("...")`.

```python
# EnvironmentExistsWaiter usage example

from types_aiobotocore_elasticbeanstalk.waiter import EnvironmentExistsWaiter

def get_environment_exists_waiter() -> EnvironmentExistsWaiter:
    return Session().client("elasticbeanstalk").get_waiter("environment_exists")
```

- [EnvironmentExistsWaiter](./waiters.md#environmentexistswaiter)
- [EnvironmentTerminatedWaiter](./waiters.md#environmentterminatedwaiter)
- [EnvironmentUpdatedWaiter](./waiters.md#environmentupdatedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionHistoryStatusType usage example

from types_aiobotocore_elasticbeanstalk.literals import ActionHistoryStatusType

def get_value() -> ActionHistoryStatusType:
    return "Completed"
```

- [ActionHistoryStatusType](./literals.md#actionhistorystatustype)
- [ActionStatusType](./literals.md#actionstatustype)
- [ActionTypeType](./literals.md#actiontypetype)
- [ApplicationVersionStatusType](./literals.md#applicationversionstatustype)
- [ComputeTypeType](./literals.md#computetypetype)
- [ConfigurationDeploymentStatusType](./literals.md#configurationdeploymentstatustype)
- [ConfigurationOptionValueTypeType](./literals.md#configurationoptionvaluetypetype)
- [DescribeApplicationVersionsPaginatorName](./literals.md#describeapplicationversionspaginatorname)
- [DescribeEnvironmentManagedActionHistoryPaginatorName](./literals.md#describeenvironmentmanagedactionhistorypaginatorname)
- [DescribeEnvironmentsPaginatorName](./literals.md#describeenvironmentspaginatorname)
- [DescribeEventsPaginatorName](./literals.md#describeeventspaginatorname)
- [EnvironmentExistsWaiterName](./literals.md#environmentexistswaitername)
- [EnvironmentHealthAttributeType](./literals.md#environmenthealthattributetype)
- [EnvironmentHealthStatusType](./literals.md#environmenthealthstatustype)
- [EnvironmentHealthType](./literals.md#environmenthealthtype)
- [EnvironmentInfoTypeType](./literals.md#environmentinfotypetype)
- [EnvironmentStatusType](./literals.md#environmentstatustype)
- [EnvironmentTerminatedWaiterName](./literals.md#environmentterminatedwaitername)
- [EnvironmentUpdatedWaiterName](./literals.md#environmentupdatedwaitername)
- [EventSeverityType](./literals.md#eventseveritytype)
- [FailureTypeType](./literals.md#failuretypetype)
- [InstancesHealthAttributeType](./literals.md#instanceshealthattributetype)
- [ListPlatformVersionsPaginatorName](./literals.md#listplatformversionspaginatorname)
- [PlatformStatusType](./literals.md#platformstatustype)
- [SourceRepositoryType](./literals.md#sourcerepositorytype)
- [SourceTypeType](./literals.md#sourcetypetype)
- [ValidationSeverityType](./literals.md#validationseveritytype)
- [ElasticBeanstalkServiceName](./literals.md#elasticbeanstalkservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AbortEnvironmentUpdateMessageRequestTypeDef](./type_defs.md#abortenvironmentupdatemessagerequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [LatencyTypeDef](./type_defs.md#latencytypedef)
- [StatusCodesTypeDef](./type_defs.md#statuscodestypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [SourceBuildInformationTypeDef](./type_defs.md#sourcebuildinformationtypedef)
- [MaxAgeRuleTypeDef](./type_defs.md#maxageruletypedef)
- [MaxCountRuleTypeDef](./type_defs.md#maxcountruletypedef)
- [ApplyEnvironmentManagedActionRequestRequestTypeDef](./type_defs.md#applyenvironmentmanagedactionrequestrequesttypedef)
- [AssociateEnvironmentOperationsRoleMessageRequestTypeDef](./type_defs.md#associateenvironmentoperationsrolemessagerequesttypedef)
- [AutoScalingGroupTypeDef](./type_defs.md#autoscalinggrouptypedef)
- [BuildConfigurationTypeDef](./type_defs.md#buildconfigurationtypedef)
- [BuilderTypeDef](./type_defs.md#buildertypedef)
- [CPUUtilizationTypeDef](./type_defs.md#cpuutilizationtypedef)
- [CheckDNSAvailabilityMessageRequestTypeDef](./type_defs.md#checkdnsavailabilitymessagerequesttypedef)
- [ComposeEnvironmentsMessageRequestTypeDef](./type_defs.md#composeenvironmentsmessagerequesttypedef)
- [OptionRestrictionRegexTypeDef](./type_defs.md#optionrestrictionregextypedef)
- [ConfigurationOptionSettingTypeDef](./type_defs.md#configurationoptionsettingtypedef)
- [ValidationMessageTypeDef](./type_defs.md#validationmessagetypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef)
- [EnvironmentTierTypeDef](./type_defs.md#environmenttiertypedef)
- [OptionSpecificationTypeDef](./type_defs.md#optionspecificationtypedef)
- [PlatformSummaryTypeDef](./type_defs.md#platformsummarytypedef)
- [CustomAmiTypeDef](./type_defs.md#customamitypedef)
- [DeleteApplicationMessageRequestTypeDef](./type_defs.md#deleteapplicationmessagerequesttypedef)
- [DeleteApplicationVersionMessageRequestTypeDef](./type_defs.md#deleteapplicationversionmessagerequesttypedef)
- [DeleteConfigurationTemplateMessageRequestTypeDef](./type_defs.md#deleteconfigurationtemplatemessagerequesttypedef)
- [DeleteEnvironmentConfigurationMessageRequestTypeDef](./type_defs.md#deleteenvironmentconfigurationmessagerequesttypedef)
- [DeletePlatformVersionRequestRequestTypeDef](./type_defs.md#deleteplatformversionrequestrequesttypedef)
- [DeploymentTypeDef](./type_defs.md#deploymenttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeApplicationVersionsMessageRequestTypeDef](./type_defs.md#describeapplicationversionsmessagerequesttypedef)
- [DescribeApplicationsMessageRequestTypeDef](./type_defs.md#describeapplicationsmessagerequesttypedef)
- [DescribeConfigurationSettingsMessageRequestTypeDef](./type_defs.md#describeconfigurationsettingsmessagerequesttypedef)
- [DescribeEnvironmentHealthRequestRequestTypeDef](./type_defs.md#describeenvironmenthealthrequestrequesttypedef)
- [InstanceHealthSummaryTypeDef](./type_defs.md#instancehealthsummarytypedef)
- [DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef](./type_defs.md#describeenvironmentmanagedactionhistoryrequestrequesttypedef)
- [ManagedActionHistoryItemTypeDef](./type_defs.md#managedactionhistoryitemtypedef)
- [DescribeEnvironmentManagedActionsRequestRequestTypeDef](./type_defs.md#describeenvironmentmanagedactionsrequestrequesttypedef)
- [ManagedActionTypeDef](./type_defs.md#managedactiontypedef)
- [DescribeEnvironmentResourcesMessageRequestTypeDef](./type_defs.md#describeenvironmentresourcesmessagerequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeInstancesHealthRequestRequestTypeDef](./type_defs.md#describeinstanceshealthrequestrequesttypedef)
- [DescribePlatformVersionRequestRequestTypeDef](./type_defs.md#describeplatformversionrequestrequesttypedef)
- [DisassociateEnvironmentOperationsRoleMessageRequestTypeDef](./type_defs.md#disassociateenvironmentoperationsrolemessagerequesttypedef)
- [EnvironmentLinkTypeDef](./type_defs.md#environmentlinktypedef)
- [EnvironmentInfoDescriptionTypeDef](./type_defs.md#environmentinfodescriptiontypedef)
- [InstanceTypeDef](./type_defs.md#instancetypedef)
- [LaunchConfigurationTypeDef](./type_defs.md#launchconfigurationtypedef)
- [LaunchTemplateTypeDef](./type_defs.md#launchtemplatetypedef)
- [LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef)
- [QueueTypeDef](./type_defs.md#queuetypedef)
- [TriggerTypeDef](./type_defs.md#triggertypedef)
- [EventDescriptionTypeDef](./type_defs.md#eventdescriptiontypedef)
- [SolutionStackDescriptionTypeDef](./type_defs.md#solutionstackdescriptiontypedef)
- [SearchFilterTypeDef](./type_defs.md#searchfiltertypedef)
- [PlatformBranchSummaryTypeDef](./type_defs.md#platformbranchsummarytypedef)
- [PlatformFilterTypeDef](./type_defs.md#platformfiltertypedef)
- [ListTagsForResourceMessageRequestTypeDef](./type_defs.md#listtagsforresourcemessagerequesttypedef)
- [ListenerTypeDef](./type_defs.md#listenertypedef)
- [PlatformFrameworkTypeDef](./type_defs.md#platformframeworktypedef)
- [PlatformProgrammingLanguageTypeDef](./type_defs.md#platformprogramminglanguagetypedef)
- [RebuildEnvironmentMessageRequestTypeDef](./type_defs.md#rebuildenvironmentmessagerequesttypedef)
- [RequestEnvironmentInfoMessageRequestTypeDef](./type_defs.md#requestenvironmentinfomessagerequesttypedef)
- [ResourceQuotaTypeDef](./type_defs.md#resourcequotatypedef)
- [RestartAppServerMessageRequestTypeDef](./type_defs.md#restartappservermessagerequesttypedef)
- [RetrieveEnvironmentInfoMessageRequestTypeDef](./type_defs.md#retrieveenvironmentinfomessagerequesttypedef)
- [SwapEnvironmentCNAMEsMessageRequestTypeDef](./type_defs.md#swapenvironmentcnamesmessagerequesttypedef)
- [TerminateEnvironmentMessageRequestTypeDef](./type_defs.md#terminateenvironmentmessagerequesttypedef)
- [UpdateApplicationMessageRequestTypeDef](./type_defs.md#updateapplicationmessagerequesttypedef)
- [UpdateApplicationVersionMessageRequestTypeDef](./type_defs.md#updateapplicationversionmessagerequesttypedef)
- [ApplyEnvironmentManagedActionResultTypeDef](./type_defs.md#applyenvironmentmanagedactionresulttypedef)
- [CheckDNSAvailabilityResultMessageTypeDef](./type_defs.md#checkdnsavailabilityresultmessagetypedef)
- [CreateStorageLocationResultMessageTypeDef](./type_defs.md#createstoragelocationresultmessagetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ApplicationMetricsTypeDef](./type_defs.md#applicationmetricstypedef)
- [ApplicationVersionDescriptionTypeDef](./type_defs.md#applicationversiondescriptiontypedef)
- [ApplicationVersionLifecycleConfigTypeDef](./type_defs.md#applicationversionlifecycleconfigtypedef)
- [SystemStatusTypeDef](./type_defs.md#systemstatustypedef)
- [ConfigurationOptionDescriptionTypeDef](./type_defs.md#configurationoptiondescriptiontypedef)
- [ConfigurationSettingsDescriptionResponseTypeDef](./type_defs.md#configurationsettingsdescriptionresponsetypedef)
- [ConfigurationSettingsDescriptionTypeDef](./type_defs.md#configurationsettingsdescriptiontypedef)
- [ValidateConfigurationSettingsMessageRequestTypeDef](./type_defs.md#validateconfigurationsettingsmessagerequesttypedef)
- [ConfigurationSettingsValidationMessagesTypeDef](./type_defs.md#configurationsettingsvalidationmessagestypedef)
- [CreateApplicationVersionMessageRequestTypeDef](./type_defs.md#createapplicationversionmessagerequesttypedef)
- [CreatePlatformVersionRequestRequestTypeDef](./type_defs.md#createplatformversionrequestrequesttypedef)
- [ResourceTagsDescriptionMessageTypeDef](./type_defs.md#resourcetagsdescriptionmessagetypedef)
- [UpdateTagsForResourceMessageRequestTypeDef](./type_defs.md#updatetagsforresourcemessagerequesttypedef)
- [CreateConfigurationTemplateMessageRequestTypeDef](./type_defs.md#createconfigurationtemplatemessagerequesttypedef)
- [CreateEnvironmentMessageRequestTypeDef](./type_defs.md#createenvironmentmessagerequesttypedef)
- [DescribeConfigurationOptionsMessageRequestTypeDef](./type_defs.md#describeconfigurationoptionsmessagerequesttypedef)
- [UpdateConfigurationTemplateMessageRequestTypeDef](./type_defs.md#updateconfigurationtemplatemessagerequesttypedef)
- [UpdateEnvironmentMessageRequestTypeDef](./type_defs.md#updateenvironmentmessagerequesttypedef)
- [CreatePlatformVersionResultTypeDef](./type_defs.md#createplatformversionresulttypedef)
- [DeletePlatformVersionResultTypeDef](./type_defs.md#deleteplatformversionresulttypedef)
- [ListPlatformVersionsResultTypeDef](./type_defs.md#listplatformversionsresulttypedef)
- [DescribeApplicationVersionsMessagePaginateTypeDef](./type_defs.md#describeapplicationversionsmessagepaginatetypedef)
- [DescribeEnvironmentManagedActionHistoryRequestPaginateTypeDef](./type_defs.md#describeenvironmentmanagedactionhistoryrequestpaginatetypedef)
- [DescribeEnvironmentManagedActionHistoryResultTypeDef](./type_defs.md#describeenvironmentmanagedactionhistoryresulttypedef)
- [DescribeEnvironmentManagedActionsResultTypeDef](./type_defs.md#describeenvironmentmanagedactionsresulttypedef)
- [DescribeEnvironmentsMessagePaginateTypeDef](./type_defs.md#describeenvironmentsmessagepaginatetypedef)
- [DescribeEnvironmentsMessageRequestTypeDef](./type_defs.md#describeenvironmentsmessagerequesttypedef)
- [DescribeEventsMessagePaginateTypeDef](./type_defs.md#describeeventsmessagepaginatetypedef)
- [DescribeEventsMessageRequestTypeDef](./type_defs.md#describeeventsmessagerequesttypedef)
- [DescribeEnvironmentsMessageWaitTypeDef](./type_defs.md#describeenvironmentsmessagewaittypedef)
- [RetrieveEnvironmentInfoResultMessageTypeDef](./type_defs.md#retrieveenvironmentinforesultmessagetypedef)
- [EnvironmentResourceDescriptionTypeDef](./type_defs.md#environmentresourcedescriptiontypedef)
- [EventDescriptionsMessageTypeDef](./type_defs.md#eventdescriptionsmessagetypedef)
- [ListAvailableSolutionStacksResultMessageTypeDef](./type_defs.md#listavailablesolutionstacksresultmessagetypedef)
- [ListPlatformBranchesRequestRequestTypeDef](./type_defs.md#listplatformbranchesrequestrequesttypedef)
- [ListPlatformBranchesResultTypeDef](./type_defs.md#listplatformbranchesresulttypedef)
- [ListPlatformVersionsRequestPaginateTypeDef](./type_defs.md#listplatformversionsrequestpaginatetypedef)
- [ListPlatformVersionsRequestRequestTypeDef](./type_defs.md#listplatformversionsrequestrequesttypedef)
- [LoadBalancerDescriptionTypeDef](./type_defs.md#loadbalancerdescriptiontypedef)
- [PlatformDescriptionTypeDef](./type_defs.md#platformdescriptiontypedef)
- [ResourceQuotasTypeDef](./type_defs.md#resourcequotastypedef)
- [DescribeEnvironmentHealthResultTypeDef](./type_defs.md#describeenvironmenthealthresulttypedef)
- [ApplicationVersionDescriptionMessageTypeDef](./type_defs.md#applicationversiondescriptionmessagetypedef)
- [ApplicationVersionDescriptionsMessageTypeDef](./type_defs.md#applicationversiondescriptionsmessagetypedef)
- [ApplicationResourceLifecycleConfigTypeDef](./type_defs.md#applicationresourcelifecycleconfigtypedef)
- [SingleInstanceHealthTypeDef](./type_defs.md#singleinstancehealthtypedef)
- [ConfigurationOptionsDescriptionTypeDef](./type_defs.md#configurationoptionsdescriptiontypedef)
- [ConfigurationSettingsDescriptionsTypeDef](./type_defs.md#configurationsettingsdescriptionstypedef)
- [EnvironmentResourceDescriptionsMessageTypeDef](./type_defs.md#environmentresourcedescriptionsmessagetypedef)
- [EnvironmentResourcesDescriptionTypeDef](./type_defs.md#environmentresourcesdescriptiontypedef)
- [DescribePlatformVersionResultTypeDef](./type_defs.md#describeplatformversionresulttypedef)
- [DescribeAccountAttributesResultTypeDef](./type_defs.md#describeaccountattributesresulttypedef)
- [ApplicationDescriptionTypeDef](./type_defs.md#applicationdescriptiontypedef)
- [ApplicationResourceLifecycleDescriptionMessageTypeDef](./type_defs.md#applicationresourcelifecycledescriptionmessagetypedef)
- [CreateApplicationMessageRequestTypeDef](./type_defs.md#createapplicationmessagerequesttypedef)
- [UpdateApplicationResourceLifecycleMessageRequestTypeDef](./type_defs.md#updateapplicationresourcelifecyclemessagerequesttypedef)
- [DescribeInstancesHealthResultTypeDef](./type_defs.md#describeinstanceshealthresulttypedef)
- [EnvironmentDescriptionResponseTypeDef](./type_defs.md#environmentdescriptionresponsetypedef)
- [EnvironmentDescriptionTypeDef](./type_defs.md#environmentdescriptiontypedef)
- [ApplicationDescriptionMessageTypeDef](./type_defs.md#applicationdescriptionmessagetypedef)
- [ApplicationDescriptionsMessageTypeDef](./type_defs.md#applicationdescriptionsmessagetypedef)
- [EnvironmentDescriptionsMessageTypeDef](./type_defs.md#environmentdescriptionsmessagetypedef)

