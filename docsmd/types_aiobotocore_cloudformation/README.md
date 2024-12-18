# CloudFormation module

> [Index](../README.md) > CloudFormation


!!! note ""

    Auto-generated documentation for [CloudFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#cloudformation)
    type annotations stubs module [types-aiobotocore-cloudformation](https://pypi.org/project/types-aiobotocore-cloudformation/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudFormation` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CloudFormation` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cloudformation]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cloudformation]'

# standalone installation
python -m pip install types-aiobotocore-cloudformation
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cloudformation
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudFormationClient

Type annotations and code completion for  `#!python session.create_client("cloudformation")` as [CloudFormationClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client)

```python
# CloudFormationClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.client import CloudFormationClient


session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("cloudformation").get_paginator("...")`.

```python
# DescribeAccountLimitsPaginator usage example

from types_aiobotocore_cloudformation.paginator import DescribeAccountLimitsPaginator

def get_describe_account_limits_paginator() -> DescribeAccountLimitsPaginator:
    return client.get_paginator("describe_account_limits"))
```

- [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
- [DescribeChangeSetPaginator](./paginators.md#describechangesetpaginator)
- [DescribeStackEventsPaginator](./paginators.md#describestackeventspaginator)
- [DescribeStacksPaginator](./paginators.md#describestackspaginator)
- [ListChangeSetsPaginator](./paginators.md#listchangesetspaginator)
- [ListExportsPaginator](./paginators.md#listexportspaginator)
- [ListGeneratedTemplatesPaginator](./paginators.md#listgeneratedtemplatespaginator)
- [ListImportsPaginator](./paginators.md#listimportspaginator)
- [ListResourceScanRelatedResourcesPaginator](./paginators.md#listresourcescanrelatedresourcespaginator)
- [ListResourceScanResourcesPaginator](./paginators.md#listresourcescanresourcespaginator)
- [ListResourceScansPaginator](./paginators.md#listresourcescanspaginator)
- [ListStackInstancesPaginator](./paginators.md#liststackinstancespaginator)
- [ListStackResourcesPaginator](./paginators.md#liststackresourcespaginator)
- [ListStackSetOperationResultsPaginator](./paginators.md#liststacksetoperationresultspaginator)
- [ListStackSetOperationsPaginator](./paginators.md#liststacksetoperationspaginator)
- [ListStackSetsPaginator](./paginators.md#liststacksetspaginator)
- [ListStacksPaginator](./paginators.md#liststackspaginator)
- [ListTypesPaginator](./paginators.md#listtypespaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("cloudformation").get_waiter("...")`.

```python
# ChangeSetCreateCompleteWaiter usage example

from types_aiobotocore_cloudformation.waiter import ChangeSetCreateCompleteWaiter

def get_change_set_create_complete_waiter() -> ChangeSetCreateCompleteWaiter:
    return Session().client("cloudformation").get_waiter("change_set_create_complete")
```

- [ChangeSetCreateCompleteWaiter](./waiters.md#changesetcreatecompletewaiter)
- [StackCreateCompleteWaiter](./waiters.md#stackcreatecompletewaiter)
- [StackDeleteCompleteWaiter](./waiters.md#stackdeletecompletewaiter)
- [StackExistsWaiter](./waiters.md#stackexistswaiter)
- [StackImportCompleteWaiter](./waiters.md#stackimportcompletewaiter)
- [StackRollbackCompleteWaiter](./waiters.md#stackrollbackcompletewaiter)
- [StackUpdateCompleteWaiter](./waiters.md#stackupdatecompletewaiter)
- [TypeRegistrationCompleteWaiter](./waiters.md#typeregistrationcompletewaiter)




## CloudFormationServiceResource

Type annotations and code completion for `#!python session.resource("cloudformation")` as
[CloudFormationServiceResource](./service_resource.md#cloudformationserviceresource)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/service-resource/index.html)

```python
# CloudFormationServiceResource usage example

from types_aiobotocore_cloudformation.service_resource import CloudFormationServiceResource
```


### Collections

Type annotations and code completion for collections
from `#!python session.resource("cloudformation").*`.

```python
# ServiceResourceStacksCollection usage example

from types_aiobotocore_cloudformation.service_resource import ServiceResourceStacksCollection

def get_collection() -> ServiceResourceStacksCollection:
    return resource.stacks
```

- [ServiceResourceStacksCollection](./service_resource.md#serviceresourcestackscollection)





### Resources

Type annotations and code completion for additional resources
from `#!python session.resource("cloudformation").*`.

```python
# Event usage example

from types_aiobotocore_cloudformation.service_resource import Event

def get_resource() -> Event:
    return resource.Event(...)
```

- [Event](./service_resource.md#event)
- [Stack](./service_resource.md#stack)
- [StackResource](./service_resource.md#stackresource)
- [StackResourceSummary](./service_resource.md#stackresourcesummary)





## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccountFilterTypeType usage example

from types_aiobotocore_cloudformation.literals import AccountFilterTypeType

def get_value() -> AccountFilterTypeType:
    return "DIFFERENCE"
```

- [AccountFilterTypeType](./literals.md#accountfiltertypetype)
- [AccountGateStatusType](./literals.md#accountgatestatustype)
- [AttributeChangeTypeType](./literals.md#attributechangetypetype)
- [CallAsType](./literals.md#callastype)
- [CapabilityType](./literals.md#capabilitytype)
- [CategoryType](./literals.md#categorytype)
- [ChangeActionType](./literals.md#changeactiontype)
- [ChangeSetCreateCompleteWaiterName](./literals.md#changesetcreatecompletewaitername)
- [ChangeSetHooksStatusType](./literals.md#changesethooksstatustype)
- [ChangeSetStatusType](./literals.md#changesetstatustype)
- [ChangeSetTypeType](./literals.md#changesettypetype)
- [ChangeSourceType](./literals.md#changesourcetype)
- [ChangeTypeType](./literals.md#changetypetype)
- [ConcurrencyModeType](./literals.md#concurrencymodetype)
- [DeletionModeType](./literals.md#deletionmodetype)
- [DeprecatedStatusType](./literals.md#deprecatedstatustype)
- [DescribeAccountLimitsPaginatorName](./literals.md#describeaccountlimitspaginatorname)
- [DescribeChangeSetPaginatorName](./literals.md#describechangesetpaginatorname)
- [DescribeStackEventsPaginatorName](./literals.md#describestackeventspaginatorname)
- [DescribeStacksPaginatorName](./literals.md#describestackspaginatorname)
- [DetailedStatusType](./literals.md#detailedstatustype)
- [DifferenceTypeType](./literals.md#differencetypetype)
- [EvaluationTypeType](./literals.md#evaluationtypetype)
- [ExecutionStatusType](./literals.md#executionstatustype)
- [GeneratedTemplateDeletionPolicyType](./literals.md#generatedtemplatedeletionpolicytype)
- [GeneratedTemplateResourceStatusType](./literals.md#generatedtemplateresourcestatustype)
- [GeneratedTemplateStatusType](./literals.md#generatedtemplatestatustype)
- [GeneratedTemplateUpdateReplacePolicyType](./literals.md#generatedtemplateupdatereplacepolicytype)
- [HandlerErrorCodeType](./literals.md#handlererrorcodetype)
- [HookFailureModeType](./literals.md#hookfailuremodetype)
- [HookInvocationPointType](./literals.md#hookinvocationpointtype)
- [HookStatusType](./literals.md#hookstatustype)
- [HookTargetTypeType](./literals.md#hooktargettypetype)
- [IdentityProviderType](./literals.md#identityprovidertype)
- [ListChangeSetsPaginatorName](./literals.md#listchangesetspaginatorname)
- [ListExportsPaginatorName](./literals.md#listexportspaginatorname)
- [ListGeneratedTemplatesPaginatorName](./literals.md#listgeneratedtemplatespaginatorname)
- [ListHookResultsTargetTypeType](./literals.md#listhookresultstargettypetype)
- [ListImportsPaginatorName](./literals.md#listimportspaginatorname)
- [ListResourceScanRelatedResourcesPaginatorName](./literals.md#listresourcescanrelatedresourcespaginatorname)
- [ListResourceScanResourcesPaginatorName](./literals.md#listresourcescanresourcespaginatorname)
- [ListResourceScansPaginatorName](./literals.md#listresourcescanspaginatorname)
- [ListStackInstancesPaginatorName](./literals.md#liststackinstancespaginatorname)
- [ListStackResourcesPaginatorName](./literals.md#liststackresourcespaginatorname)
- [ListStackSetOperationResultsPaginatorName](./literals.md#liststacksetoperationresultspaginatorname)
- [ListStackSetOperationsPaginatorName](./literals.md#liststacksetoperationspaginatorname)
- [ListStackSetsPaginatorName](./literals.md#liststacksetspaginatorname)
- [ListStacksPaginatorName](./literals.md#liststackspaginatorname)
- [ListTypesPaginatorName](./literals.md#listtypespaginatorname)
- [OnFailureType](./literals.md#onfailuretype)
- [OnStackFailureType](./literals.md#onstackfailuretype)
- [OperationResultFilterNameType](./literals.md#operationresultfilternametype)
- [OperationStatusType](./literals.md#operationstatustype)
- [OrganizationStatusType](./literals.md#organizationstatustype)
- [PermissionModelsType](./literals.md#permissionmodelstype)
- [PolicyActionType](./literals.md#policyactiontype)
- [ProvisioningTypeType](./literals.md#provisioningtypetype)
- [PublisherStatusType](./literals.md#publisherstatustype)
- [RegionConcurrencyTypeType](./literals.md#regionconcurrencytypetype)
- [RegistrationStatusType](./literals.md#registrationstatustype)
- [RegistryTypeType](./literals.md#registrytypetype)
- [ReplacementType](./literals.md#replacementtype)
- [RequiresRecreationType](./literals.md#requiresrecreationtype)
- [ResourceAttributeType](./literals.md#resourceattributetype)
- [ResourceScanStatusType](./literals.md#resourcescanstatustype)
- [ResourceSignalStatusType](./literals.md#resourcesignalstatustype)
- [ResourceStatusType](./literals.md#resourcestatustype)
- [StackCreateCompleteWaiterName](./literals.md#stackcreatecompletewaitername)
- [StackDeleteCompleteWaiterName](./literals.md#stackdeletecompletewaitername)
- [StackDriftDetectionStatusType](./literals.md#stackdriftdetectionstatustype)
- [StackDriftStatusType](./literals.md#stackdriftstatustype)
- [StackExistsWaiterName](./literals.md#stackexistswaitername)
- [StackImportCompleteWaiterName](./literals.md#stackimportcompletewaitername)
- [StackInstanceDetailedStatusType](./literals.md#stackinstancedetailedstatustype)
- [StackInstanceFilterNameType](./literals.md#stackinstancefilternametype)
- [StackInstanceStatusType](./literals.md#stackinstancestatustype)
- [StackResourceDriftStatusType](./literals.md#stackresourcedriftstatustype)
- [StackRollbackCompleteWaiterName](./literals.md#stackrollbackcompletewaitername)
- [StackSetDriftDetectionStatusType](./literals.md#stacksetdriftdetectionstatustype)
- [StackSetDriftStatusType](./literals.md#stacksetdriftstatustype)
- [StackSetOperationActionType](./literals.md#stacksetoperationactiontype)
- [StackSetOperationResultStatusType](./literals.md#stacksetoperationresultstatustype)
- [StackSetOperationStatusType](./literals.md#stacksetoperationstatustype)
- [StackSetStatusType](./literals.md#stacksetstatustype)
- [StackStatusType](./literals.md#stackstatustype)
- [StackUpdateCompleteWaiterName](./literals.md#stackupdatecompletewaitername)
- [TemplateFormatType](./literals.md#templateformattype)
- [TemplateStageType](./literals.md#templatestagetype)
- [ThirdPartyTypeType](./literals.md#thirdpartytypetype)
- [TypeRegistrationCompleteWaiterName](./literals.md#typeregistrationcompletewaitername)
- [TypeTestsStatusType](./literals.md#typetestsstatustype)
- [VersionBumpType](./literals.md#versionbumptype)
- [VisibilityType](./literals.md#visibilitytype)
- [WarningTypeType](./literals.md#warningtypetype)
- [CloudFormationServiceName](./literals.md#cloudformationservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountGateResultTypeDef](./type_defs.md#accountgateresulttypedef)
- [AccountLimitTypeDef](./type_defs.md#accountlimittypedef)
- [LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AutoDeploymentTypeDef](./type_defs.md#autodeploymenttypedef)
- [TypeConfigurationIdentifierTypeDef](./type_defs.md#typeconfigurationidentifiertypedef)
- [TypeConfigurationDetailsTypeDef](./type_defs.md#typeconfigurationdetailstypedef)
- [CancelUpdateStackInputRequestTypeDef](./type_defs.md#cancelupdatestackinputrequesttypedef)
- [CancelUpdateStackInputStackCancelUpdateTypeDef](./type_defs.md#cancelupdatestackinputstackcancelupdatetypedef)
- [ChangeSetHookResourceTargetDetailsTypeDef](./type_defs.md#changesethookresourcetargetdetailstypedef)
- [ChangeSetSummaryTypeDef](./type_defs.md#changesetsummarytypedef)
- [ContinueUpdateRollbackInputRequestTypeDef](./type_defs.md#continueupdaterollbackinputrequesttypedef)
- [ParameterTypeDef](./type_defs.md#parametertypedef)
- [ResourceToImportTypeDef](./type_defs.md#resourcetoimporttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResourceDefinitionTypeDef](./type_defs.md#resourcedefinitiontypedef)
- [TemplateConfigurationTypeDef](./type_defs.md#templateconfigurationtypedef)
- [DeploymentTargetsTypeDef](./type_defs.md#deploymenttargetstypedef)
- [StackSetOperationPreferencesTypeDef](./type_defs.md#stacksetoperationpreferencestypedef)
- [ManagedExecutionTypeDef](./type_defs.md#managedexecutiontypedef)
- [DeactivateTypeInputRequestTypeDef](./type_defs.md#deactivatetypeinputrequesttypedef)
- [DeleteChangeSetInputRequestTypeDef](./type_defs.md#deletechangesetinputrequesttypedef)
- [DeleteGeneratedTemplateInputRequestTypeDef](./type_defs.md#deletegeneratedtemplateinputrequesttypedef)
- [DeleteStackInputRequestTypeDef](./type_defs.md#deletestackinputrequesttypedef)
- [DeleteStackInputStackDeleteTypeDef](./type_defs.md#deletestackinputstackdeletetypedef)
- [DeleteStackSetInputRequestTypeDef](./type_defs.md#deletestacksetinputrequesttypedef)
- [DeploymentTargetsOutputTypeDef](./type_defs.md#deploymenttargetsoutputtypedef)
- [DeregisterTypeInputRequestTypeDef](./type_defs.md#deregistertypeinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeAccountLimitsInputRequestTypeDef](./type_defs.md#describeaccountlimitsinputrequesttypedef)
- [DescribeChangeSetHooksInputRequestTypeDef](./type_defs.md#describechangesethooksinputrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeChangeSetInputRequestTypeDef](./type_defs.md#describechangesetinputrequesttypedef)
- [DescribeGeneratedTemplateInputRequestTypeDef](./type_defs.md#describegeneratedtemplateinputrequesttypedef)
- [TemplateProgressTypeDef](./type_defs.md#templateprogresstypedef)
- [DescribeOrganizationsAccessInputRequestTypeDef](./type_defs.md#describeorganizationsaccessinputrequesttypedef)
- [DescribePublisherInputRequestTypeDef](./type_defs.md#describepublisherinputrequesttypedef)
- [DescribeResourceScanInputRequestTypeDef](./type_defs.md#describeresourcescaninputrequesttypedef)
- [DescribeStackDriftDetectionStatusInputRequestTypeDef](./type_defs.md#describestackdriftdetectionstatusinputrequesttypedef)
- [DescribeStackEventsInputRequestTypeDef](./type_defs.md#describestackeventsinputrequesttypedef)
- [StackEventTypeDef](./type_defs.md#stackeventtypedef)
- [DescribeStackInstanceInputRequestTypeDef](./type_defs.md#describestackinstanceinputrequesttypedef)
- [DescribeStackResourceDriftsInputRequestTypeDef](./type_defs.md#describestackresourcedriftsinputrequesttypedef)
- [DescribeStackResourceInputRequestTypeDef](./type_defs.md#describestackresourceinputrequesttypedef)
- [DescribeStackResourcesInputRequestTypeDef](./type_defs.md#describestackresourcesinputrequesttypedef)
- [DescribeStackSetInputRequestTypeDef](./type_defs.md#describestacksetinputrequesttypedef)
- [DescribeStackSetOperationInputRequestTypeDef](./type_defs.md#describestacksetoperationinputrequesttypedef)
- [DescribeStacksInputRequestTypeDef](./type_defs.md#describestacksinputrequesttypedef)
- [DescribeTypeInputRequestTypeDef](./type_defs.md#describetypeinputrequesttypedef)
- [RequiredActivatedTypeTypeDef](./type_defs.md#requiredactivatedtypetypedef)
- [DescribeTypeRegistrationInputRequestTypeDef](./type_defs.md#describetyperegistrationinputrequesttypedef)
- [DetectStackDriftInputRequestTypeDef](./type_defs.md#detectstackdriftinputrequesttypedef)
- [DetectStackResourceDriftInputRequestTypeDef](./type_defs.md#detectstackresourcedriftinputrequesttypedef)
- [ExecuteChangeSetInputRequestTypeDef](./type_defs.md#executechangesetinputrequesttypedef)
- [ExportTypeDef](./type_defs.md#exporttypedef)
- [GetGeneratedTemplateInputRequestTypeDef](./type_defs.md#getgeneratedtemplateinputrequesttypedef)
- [GetStackPolicyInputRequestTypeDef](./type_defs.md#getstackpolicyinputrequesttypedef)
- [GetTemplateInputRequestTypeDef](./type_defs.md#gettemplateinputrequesttypedef)
- [TemplateSummaryConfigTypeDef](./type_defs.md#templatesummaryconfigtypedef)
- [ResourceIdentifierSummaryTypeDef](./type_defs.md#resourceidentifiersummarytypedef)
- [WarningsTypeDef](./type_defs.md#warningstypedef)
- [HookResultSummaryTypeDef](./type_defs.md#hookresultsummarytypedef)
- [ListChangeSetsInputRequestTypeDef](./type_defs.md#listchangesetsinputrequesttypedef)
- [ListExportsInputRequestTypeDef](./type_defs.md#listexportsinputrequesttypedef)
- [ListGeneratedTemplatesInputRequestTypeDef](./type_defs.md#listgeneratedtemplatesinputrequesttypedef)
- [TemplateSummaryTypeDef](./type_defs.md#templatesummarytypedef)
- [ListHookResultsInputRequestTypeDef](./type_defs.md#listhookresultsinputrequesttypedef)
- [ListImportsInputRequestTypeDef](./type_defs.md#listimportsinputrequesttypedef)
- [ScannedResourceIdentifierTypeDef](./type_defs.md#scannedresourceidentifiertypedef)
- [ScannedResourceTypeDef](./type_defs.md#scannedresourcetypedef)
- [ListResourceScanResourcesInputRequestTypeDef](./type_defs.md#listresourcescanresourcesinputrequesttypedef)
- [ListResourceScansInputRequestTypeDef](./type_defs.md#listresourcescansinputrequesttypedef)
- [ResourceScanSummaryTypeDef](./type_defs.md#resourcescansummarytypedef)
- [ListStackInstanceResourceDriftsInputRequestTypeDef](./type_defs.md#liststackinstanceresourcedriftsinputrequesttypedef)
- [StackInstanceFilterTypeDef](./type_defs.md#stackinstancefiltertypedef)
- [ListStackResourcesInputRequestTypeDef](./type_defs.md#liststackresourcesinputrequesttypedef)
- [ListStackSetAutoDeploymentTargetsInputRequestTypeDef](./type_defs.md#liststacksetautodeploymenttargetsinputrequesttypedef)
- [StackSetAutoDeploymentTargetSummaryTypeDef](./type_defs.md#stacksetautodeploymenttargetsummarytypedef)
- [OperationResultFilterTypeDef](./type_defs.md#operationresultfiltertypedef)
- [ListStackSetOperationsInputRequestTypeDef](./type_defs.md#liststacksetoperationsinputrequesttypedef)
- [ListStackSetsInputRequestTypeDef](./type_defs.md#liststacksetsinputrequesttypedef)
- [ListStacksInputRequestTypeDef](./type_defs.md#liststacksinputrequesttypedef)
- [ListTypeRegistrationsInputRequestTypeDef](./type_defs.md#listtyperegistrationsinputrequesttypedef)
- [ListTypeVersionsInputRequestTypeDef](./type_defs.md#listtypeversionsinputrequesttypedef)
- [TypeVersionSummaryTypeDef](./type_defs.md#typeversionsummarytypedef)
- [TypeFiltersTypeDef](./type_defs.md#typefilterstypedef)
- [TypeSummaryTypeDef](./type_defs.md#typesummarytypedef)
- [ModuleInfoTypeDef](./type_defs.md#moduleinfotypedef)
- [OutputTypeDef](./type_defs.md#outputtypedef)
- [ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef)
- [PhysicalResourceIdContextKeyValuePairTypeDef](./type_defs.md#physicalresourceidcontextkeyvaluepairtypedef)
- [PropertyDifferenceTypeDef](./type_defs.md#propertydifferencetypedef)
- [PublishTypeInputRequestTypeDef](./type_defs.md#publishtypeinputrequesttypedef)
- [RecordHandlerProgressInputRequestTypeDef](./type_defs.md#recordhandlerprogressinputrequesttypedef)
- [RegisterPublisherInputRequestTypeDef](./type_defs.md#registerpublisherinputrequesttypedef)
- [ResourceTargetDefinitionTypeDef](./type_defs.md#resourcetargetdefinitiontypedef)
- [RollbackTriggerTypeDef](./type_defs.md#rollbacktriggertypedef)
- [RollbackStackInputRequestTypeDef](./type_defs.md#rollbackstackinputrequesttypedef)
- [SetStackPolicyInputRequestTypeDef](./type_defs.md#setstackpolicyinputrequesttypedef)
- [SetTypeConfigurationInputRequestTypeDef](./type_defs.md#settypeconfigurationinputrequesttypedef)
- [SetTypeDefaultVersionInputRequestTypeDef](./type_defs.md#settypedefaultversioninputrequesttypedef)
- [SignalResourceInputRequestTypeDef](./type_defs.md#signalresourceinputrequesttypedef)
- [StackDriftInformationSummaryTypeDef](./type_defs.md#stackdriftinformationsummarytypedef)
- [StackDriftInformationTypeDef](./type_defs.md#stackdriftinformationtypedef)
- [StackInstanceComprehensiveStatusTypeDef](./type_defs.md#stackinstancecomprehensivestatustypedef)
- [StackResourceDriftInformationTypeDef](./type_defs.md#stackresourcedriftinformationtypedef)
- [StackResourceDriftInformationSummaryTypeDef](./type_defs.md#stackresourcedriftinformationsummarytypedef)
- [StackSetDriftDetectionDetailsTypeDef](./type_defs.md#stacksetdriftdetectiondetailstypedef)
- [StackSetOperationPreferencesOutputTypeDef](./type_defs.md#stacksetoperationpreferencesoutputtypedef)
- [StackSetOperationStatusDetailsTypeDef](./type_defs.md#stacksetoperationstatusdetailstypedef)
- [StartResourceScanInputRequestTypeDef](./type_defs.md#startresourcescaninputrequesttypedef)
- [StopStackSetOperationInputRequestTypeDef](./type_defs.md#stopstacksetoperationinputrequesttypedef)
- [TemplateParameterTypeDef](./type_defs.md#templateparametertypedef)
- [TestTypeInputRequestTypeDef](./type_defs.md#testtypeinputrequesttypedef)
- [UpdateTerminationProtectionInputRequestTypeDef](./type_defs.md#updateterminationprotectioninputrequesttypedef)
- [ValidateTemplateInputRequestTypeDef](./type_defs.md#validatetemplateinputrequesttypedef)
- [WarningPropertyTypeDef](./type_defs.md#warningpropertytypedef)
- [StackSetOperationResultSummaryTypeDef](./type_defs.md#stacksetoperationresultsummarytypedef)
- [ActivateTypeInputRequestTypeDef](./type_defs.md#activatetypeinputrequesttypedef)
- [RegisterTypeInputRequestTypeDef](./type_defs.md#registertypeinputrequesttypedef)
- [ActivateTypeOutputTypeDef](./type_defs.md#activatetypeoutputtypedef)
- [CreateChangeSetOutputTypeDef](./type_defs.md#createchangesetoutputtypedef)
- [CreateGeneratedTemplateOutputTypeDef](./type_defs.md#creategeneratedtemplateoutputtypedef)
- [CreateStackInstancesOutputTypeDef](./type_defs.md#createstackinstancesoutputtypedef)
- [CreateStackOutputTypeDef](./type_defs.md#createstackoutputtypedef)
- [CreateStackSetOutputTypeDef](./type_defs.md#createstacksetoutputtypedef)
- [DeleteStackInstancesOutputTypeDef](./type_defs.md#deletestackinstancesoutputtypedef)
- [DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef)
- [DescribeOrganizationsAccessOutputTypeDef](./type_defs.md#describeorganizationsaccessoutputtypedef)
- [DescribePublisherOutputTypeDef](./type_defs.md#describepublisheroutputtypedef)
- [DescribeResourceScanOutputTypeDef](./type_defs.md#describeresourcescanoutputtypedef)
- [DescribeStackDriftDetectionStatusOutputTypeDef](./type_defs.md#describestackdriftdetectionstatusoutputtypedef)
- [DescribeTypeRegistrationOutputTypeDef](./type_defs.md#describetyperegistrationoutputtypedef)
- [DetectStackDriftOutputTypeDef](./type_defs.md#detectstackdriftoutputtypedef)
- [DetectStackSetDriftOutputTypeDef](./type_defs.md#detectstacksetdriftoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [EstimateTemplateCostOutputTypeDef](./type_defs.md#estimatetemplatecostoutputtypedef)
- [GetGeneratedTemplateOutputTypeDef](./type_defs.md#getgeneratedtemplateoutputtypedef)
- [GetStackPolicyOutputTypeDef](./type_defs.md#getstackpolicyoutputtypedef)
- [GetTemplateOutputTypeDef](./type_defs.md#gettemplateoutputtypedef)
- [ImportStacksToStackSetOutputTypeDef](./type_defs.md#importstackstostacksetoutputtypedef)
- [ListImportsOutputTypeDef](./type_defs.md#listimportsoutputtypedef)
- [ListTypeRegistrationsOutputTypeDef](./type_defs.md#listtyperegistrationsoutputtypedef)
- [PublishTypeOutputTypeDef](./type_defs.md#publishtypeoutputtypedef)
- [RegisterPublisherOutputTypeDef](./type_defs.md#registerpublisheroutputtypedef)
- [RegisterTypeOutputTypeDef](./type_defs.md#registertypeoutputtypedef)
- [RollbackStackOutputTypeDef](./type_defs.md#rollbackstackoutputtypedef)
- [SetTypeConfigurationOutputTypeDef](./type_defs.md#settypeconfigurationoutputtypedef)
- [StartResourceScanOutputTypeDef](./type_defs.md#startresourcescanoutputtypedef)
- [TestTypeOutputTypeDef](./type_defs.md#testtypeoutputtypedef)
- [UpdateGeneratedTemplateOutputTypeDef](./type_defs.md#updategeneratedtemplateoutputtypedef)
- [UpdateStackInstancesOutputTypeDef](./type_defs.md#updatestackinstancesoutputtypedef)
- [UpdateStackOutputTypeDef](./type_defs.md#updatestackoutputtypedef)
- [UpdateStackSetOutputTypeDef](./type_defs.md#updatestacksetoutputtypedef)
- [UpdateTerminationProtectionOutputTypeDef](./type_defs.md#updateterminationprotectionoutputtypedef)
- [BatchDescribeTypeConfigurationsErrorTypeDef](./type_defs.md#batchdescribetypeconfigurationserrortypedef)
- [BatchDescribeTypeConfigurationsInputRequestTypeDef](./type_defs.md#batchdescribetypeconfigurationsinputrequesttypedef)
- [ChangeSetHookTargetDetailsTypeDef](./type_defs.md#changesethooktargetdetailstypedef)
- [ListChangeSetsOutputTypeDef](./type_defs.md#listchangesetsoutputtypedef)
- [EstimateTemplateCostInputRequestTypeDef](./type_defs.md#estimatetemplatecostinputrequesttypedef)
- [CreateGeneratedTemplateInputRequestTypeDef](./type_defs.md#creategeneratedtemplateinputrequesttypedef)
- [UpdateGeneratedTemplateInputRequestTypeDef](./type_defs.md#updategeneratedtemplateinputrequesttypedef)
- [CreateStackInstancesInputRequestTypeDef](./type_defs.md#createstackinstancesinputrequesttypedef)
- [DeleteStackInstancesInputRequestTypeDef](./type_defs.md#deletestackinstancesinputrequesttypedef)
- [DetectStackSetDriftInputRequestTypeDef](./type_defs.md#detectstacksetdriftinputrequesttypedef)
- [ImportStacksToStackSetInputRequestTypeDef](./type_defs.md#importstackstostacksetinputrequesttypedef)
- [UpdateStackInstancesInputRequestTypeDef](./type_defs.md#updatestackinstancesinputrequesttypedef)
- [CreateStackSetInputRequestTypeDef](./type_defs.md#createstacksetinputrequesttypedef)
- [StackSetSummaryTypeDef](./type_defs.md#stacksetsummarytypedef)
- [UpdateStackSetInputRequestTypeDef](./type_defs.md#updatestacksetinputrequesttypedef)
- [DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef](./type_defs.md#describeaccountlimitsinputdescribeaccountlimitspaginatetypedef)
- [DescribeChangeSetInputDescribeChangeSetPaginateTypeDef](./type_defs.md#describechangesetinputdescribechangesetpaginatetypedef)
- [DescribeStackEventsInputDescribeStackEventsPaginateTypeDef](./type_defs.md#describestackeventsinputdescribestackeventspaginatetypedef)
- [DescribeStacksInputDescribeStacksPaginateTypeDef](./type_defs.md#describestacksinputdescribestackspaginatetypedef)
- [ListChangeSetsInputListChangeSetsPaginateTypeDef](./type_defs.md#listchangesetsinputlistchangesetspaginatetypedef)
- [ListExportsInputListExportsPaginateTypeDef](./type_defs.md#listexportsinputlistexportspaginatetypedef)
- [ListGeneratedTemplatesInputListGeneratedTemplatesPaginateTypeDef](./type_defs.md#listgeneratedtemplatesinputlistgeneratedtemplatespaginatetypedef)
- [ListImportsInputListImportsPaginateTypeDef](./type_defs.md#listimportsinputlistimportspaginatetypedef)
- [ListResourceScanResourcesInputListResourceScanResourcesPaginateTypeDef](./type_defs.md#listresourcescanresourcesinputlistresourcescanresourcespaginatetypedef)
- [ListResourceScansInputListResourceScansPaginateTypeDef](./type_defs.md#listresourcescansinputlistresourcescanspaginatetypedef)
- [ListStackResourcesInputListStackResourcesPaginateTypeDef](./type_defs.md#liststackresourcesinputliststackresourcespaginatetypedef)
- [ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef](./type_defs.md#liststacksetoperationsinputliststacksetoperationspaginatetypedef)
- [ListStackSetsInputListStackSetsPaginateTypeDef](./type_defs.md#liststacksetsinputliststacksetspaginatetypedef)
- [ListStacksInputListStacksPaginateTypeDef](./type_defs.md#liststacksinputliststackspaginatetypedef)
- [DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef](./type_defs.md#describechangesetinputchangesetcreatecompletewaittypedef)
- [DescribeStacksInputStackCreateCompleteWaitTypeDef](./type_defs.md#describestacksinputstackcreatecompletewaittypedef)
- [DescribeStacksInputStackDeleteCompleteWaitTypeDef](./type_defs.md#describestacksinputstackdeletecompletewaittypedef)
- [DescribeStacksInputStackExistsWaitTypeDef](./type_defs.md#describestacksinputstackexistswaittypedef)
- [DescribeStacksInputStackImportCompleteWaitTypeDef](./type_defs.md#describestacksinputstackimportcompletewaittypedef)
- [DescribeStacksInputStackRollbackCompleteWaitTypeDef](./type_defs.md#describestacksinputstackrollbackcompletewaittypedef)
- [DescribeStacksInputStackUpdateCompleteWaitTypeDef](./type_defs.md#describestacksinputstackupdatecompletewaittypedef)
- [DescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef](./type_defs.md#describetyperegistrationinputtyperegistrationcompletewaittypedef)
- [DescribeStackEventsOutputTypeDef](./type_defs.md#describestackeventsoutputtypedef)
- [DescribeTypeOutputTypeDef](./type_defs.md#describetypeoutputtypedef)
- [ListExportsOutputTypeDef](./type_defs.md#listexportsoutputtypedef)
- [GetTemplateSummaryInputRequestTypeDef](./type_defs.md#gettemplatesummaryinputrequesttypedef)
- [ListHookResultsOutputTypeDef](./type_defs.md#listhookresultsoutputtypedef)
- [ListGeneratedTemplatesOutputTypeDef](./type_defs.md#listgeneratedtemplatesoutputtypedef)
- [ListResourceScanRelatedResourcesInputListResourceScanRelatedResourcesPaginateTypeDef](./type_defs.md#listresourcescanrelatedresourcesinputlistresourcescanrelatedresourcespaginatetypedef)
- [ListResourceScanRelatedResourcesInputRequestTypeDef](./type_defs.md#listresourcescanrelatedresourcesinputrequesttypedef)
- [ListResourceScanRelatedResourcesOutputTypeDef](./type_defs.md#listresourcescanrelatedresourcesoutputtypedef)
- [ListResourceScanResourcesOutputTypeDef](./type_defs.md#listresourcescanresourcesoutputtypedef)
- [ListResourceScansOutputTypeDef](./type_defs.md#listresourcescansoutputtypedef)
- [ListStackInstancesInputListStackInstancesPaginateTypeDef](./type_defs.md#liststackinstancesinputliststackinstancespaginatetypedef)
- [ListStackInstancesInputRequestTypeDef](./type_defs.md#liststackinstancesinputrequesttypedef)
- [ListStackSetAutoDeploymentTargetsOutputTypeDef](./type_defs.md#liststacksetautodeploymenttargetsoutputtypedef)
- [ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef](./type_defs.md#liststacksetoperationresultsinputliststacksetoperationresultspaginatetypedef)
- [ListStackSetOperationResultsInputRequestTypeDef](./type_defs.md#liststacksetoperationresultsinputrequesttypedef)
- [ListTypeVersionsOutputTypeDef](./type_defs.md#listtypeversionsoutputtypedef)
- [ListTypesInputListTypesPaginateTypeDef](./type_defs.md#listtypesinputlisttypespaginatetypedef)
- [ListTypesInputRequestTypeDef](./type_defs.md#listtypesinputrequesttypedef)
- [ListTypesOutputTypeDef](./type_defs.md#listtypesoutputtypedef)
- [ParameterDeclarationTypeDef](./type_defs.md#parameterdeclarationtypedef)
- [StackInstanceResourceDriftsSummaryTypeDef](./type_defs.md#stackinstanceresourcedriftssummarytypedef)
- [StackResourceDriftTypeDef](./type_defs.md#stackresourcedrifttypedef)
- [ResourceChangeDetailTypeDef](./type_defs.md#resourcechangedetailtypedef)
- [RollbackConfigurationOutputTypeDef](./type_defs.md#rollbackconfigurationoutputtypedef)
- [RollbackConfigurationTypeDef](./type_defs.md#rollbackconfigurationtypedef)
- [StackSummaryTypeDef](./type_defs.md#stacksummarytypedef)
- [StackInstanceSummaryTypeDef](./type_defs.md#stackinstancesummarytypedef)
- [StackInstanceTypeDef](./type_defs.md#stackinstancetypedef)
- [StackResourceDetailTypeDef](./type_defs.md#stackresourcedetailtypedef)
- [StackResourceTypeDef](./type_defs.md#stackresourcetypedef)
- [StackResourceSummaryTypeDef](./type_defs.md#stackresourcesummarytypedef)
- [StackSetTypeDef](./type_defs.md#stacksettypedef)
- [StackSetOperationSummaryTypeDef](./type_defs.md#stacksetoperationsummarytypedef)
- [StackSetOperationTypeDef](./type_defs.md#stacksetoperationtypedef)
- [ValidateTemplateOutputTypeDef](./type_defs.md#validatetemplateoutputtypedef)
- [WarningDetailTypeDef](./type_defs.md#warningdetailtypedef)
- [ListStackSetOperationResultsOutputTypeDef](./type_defs.md#liststacksetoperationresultsoutputtypedef)
- [BatchDescribeTypeConfigurationsOutputTypeDef](./type_defs.md#batchdescribetypeconfigurationsoutputtypedef)
- [ChangeSetHookTypeDef](./type_defs.md#changesethooktypedef)
- [ListStackSetsOutputTypeDef](./type_defs.md#liststacksetsoutputtypedef)
- [GetTemplateSummaryOutputTypeDef](./type_defs.md#gettemplatesummaryoutputtypedef)
- [ListStackInstanceResourceDriftsOutputTypeDef](./type_defs.md#liststackinstanceresourcedriftsoutputtypedef)
- [DescribeStackResourceDriftsOutputTypeDef](./type_defs.md#describestackresourcedriftsoutputtypedef)
- [DetectStackResourceDriftOutputTypeDef](./type_defs.md#detectstackresourcedriftoutputtypedef)
- [ResourceChangeTypeDef](./type_defs.md#resourcechangetypedef)
- [StackTypeDef](./type_defs.md#stacktypedef)
- [CreateChangeSetInputRequestTypeDef](./type_defs.md#createchangesetinputrequesttypedef)
- [CreateStackInputRequestTypeDef](./type_defs.md#createstackinputrequesttypedef)
- [CreateStackInputServiceResourceCreateStackTypeDef](./type_defs.md#createstackinputserviceresourcecreatestacktypedef)
- [UpdateStackInputRequestTypeDef](./type_defs.md#updatestackinputrequesttypedef)
- [UpdateStackInputStackUpdateTypeDef](./type_defs.md#updatestackinputstackupdatetypedef)
- [ListStacksOutputTypeDef](./type_defs.md#liststacksoutputtypedef)
- [ListStackInstancesOutputTypeDef](./type_defs.md#liststackinstancesoutputtypedef)
- [DescribeStackInstanceOutputTypeDef](./type_defs.md#describestackinstanceoutputtypedef)
- [DescribeStackResourceOutputTypeDef](./type_defs.md#describestackresourceoutputtypedef)
- [DescribeStackResourcesOutputTypeDef](./type_defs.md#describestackresourcesoutputtypedef)
- [ListStackResourcesOutputTypeDef](./type_defs.md#liststackresourcesoutputtypedef)
- [DescribeStackSetOutputTypeDef](./type_defs.md#describestacksetoutputtypedef)
- [ListStackSetOperationsOutputTypeDef](./type_defs.md#liststacksetoperationsoutputtypedef)
- [DescribeStackSetOperationOutputTypeDef](./type_defs.md#describestacksetoperationoutputtypedef)
- [ResourceDetailTypeDef](./type_defs.md#resourcedetailtypedef)
- [DescribeChangeSetHooksOutputTypeDef](./type_defs.md#describechangesethooksoutputtypedef)
- [ChangeTypeDef](./type_defs.md#changetypedef)
- [DescribeStacksOutputTypeDef](./type_defs.md#describestacksoutputtypedef)
- [DescribeGeneratedTemplateOutputTypeDef](./type_defs.md#describegeneratedtemplateoutputtypedef)
- [DescribeChangeSetOutputTypeDef](./type_defs.md#describechangesetoutputtypedef)

