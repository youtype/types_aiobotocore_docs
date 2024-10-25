# OpenSearchService module

> [Index](../README.md) > OpenSearchService


!!! note ""

    Auto-generated documentation for [OpenSearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
    type annotations stubs module [types-aiobotocore-opensearch](https://pypi.org/project/types-aiobotocore-opensearch/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `OpenSearchService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[opensearch]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[opensearch]'


# standalone installation
python -m pip install types-aiobotocore-opensearch
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-opensearch
```

## Usage

Code samples can be found in [Examples](./usage.md).

## OpenSearchServiceClient

Type annotations and code completion for  `#!python session.create_client("opensearch")` as [OpenSearchServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client)

```python
# OpenSearchServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_opensearch.client import OpenSearchServiceClient


session = get_session()
async with session.create_client("opensearch") as client:
    client: OpenSearchServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionSeverityType usage example

from types_aiobotocore_opensearch.literals import ActionSeverityType

def get_value() -> ActionSeverityType:
    return "HIGH"
```

- [ActionSeverityType](./literals.md#actionseveritytype)
- [ActionStatusType](./literals.md#actionstatustype)
- [ActionTypeType](./literals.md#actiontypetype)
- [AutoTuneDesiredStateType](./literals.md#autotunedesiredstatetype)
- [AutoTuneStateType](./literals.md#autotunestatetype)
- [AutoTuneTypeType](./literals.md#autotunetypetype)
- [ConfigChangeStatusType](./literals.md#configchangestatustype)
- [ConnectionModeType](./literals.md#connectionmodetype)
- [DataSourceStatusType](./literals.md#datasourcestatustype)
- [DeploymentStatusType](./literals.md#deploymentstatustype)
- [DescribePackagesFilterNameType](./literals.md#describepackagesfilternametype)
- [DomainHealthType](./literals.md#domainhealthtype)
- [DomainPackageStatusType](./literals.md#domainpackagestatustype)
- [DomainProcessingStatusTypeType](./literals.md#domainprocessingstatustypetype)
- [DomainStateType](./literals.md#domainstatetype)
- [DryRunModeType](./literals.md#dryrunmodetype)
- [EngineTypeType](./literals.md#enginetypetype)
- [IPAddressTypeType](./literals.md#ipaddresstypetype)
- [InboundConnectionStatusCodeType](./literals.md#inboundconnectionstatuscodetype)
- [InitiatedByType](./literals.md#initiatedbytype)
- [LogTypeType](./literals.md#logtypetype)
- [MaintenanceStatusType](./literals.md#maintenancestatustype)
- [MaintenanceTypeType](./literals.md#maintenancetypetype)
- [MasterNodeStatusType](./literals.md#masternodestatustype)
- [NaturalLanguageQueryGenerationCurrentStateType](./literals.md#naturallanguagequerygenerationcurrentstatetype)
- [NaturalLanguageQueryGenerationDesiredStateType](./literals.md#naturallanguagequerygenerationdesiredstatetype)
- [NodeStatusType](./literals.md#nodestatustype)
- [NodeTypeType](./literals.md#nodetypetype)
- [OpenSearchPartitionInstanceTypeType](./literals.md#opensearchpartitioninstancetypetype)
- [OpenSearchWarmPartitionInstanceTypeType](./literals.md#opensearchwarmpartitioninstancetypetype)
- [OptionStateType](./literals.md#optionstatetype)
- [OutboundConnectionStatusCodeType](./literals.md#outboundconnectionstatuscodetype)
- [OverallChangeStatusType](./literals.md#overallchangestatustype)
- [PackageStatusType](./literals.md#packagestatustype)
- [PackageTypeType](./literals.md#packagetypetype)
- [PrincipalTypeType](./literals.md#principaltypetype)
- [PropertyValueTypeType](./literals.md#propertyvaluetypetype)
- [ReservedInstancePaymentOptionType](./literals.md#reservedinstancepaymentoptiontype)
- [RollbackOnDisableType](./literals.md#rollbackondisabletype)
- [ScheduleAtType](./literals.md#scheduleattype)
- [ScheduledAutoTuneActionTypeType](./literals.md#scheduledautotuneactiontypetype)
- [ScheduledAutoTuneSeverityTypeType](./literals.md#scheduledautotuneseveritytypetype)
- [ScheduledByType](./literals.md#scheduledbytype)
- [SkipUnavailableStatusType](./literals.md#skipunavailablestatustype)
- [TLSSecurityPolicyType](./literals.md#tlssecuritypolicytype)
- [TimeUnitType](./literals.md#timeunittype)
- [UpgradeStatusType](./literals.md#upgradestatustype)
- [UpgradeStepType](./literals.md#upgradesteptype)
- [VolumeTypeType](./literals.md#volumetypetype)
- [VpcEndpointErrorCodeType](./literals.md#vpcendpointerrorcodetype)
- [VpcEndpointStatusType](./literals.md#vpcendpointstatustype)
- [ZoneStatusType](./literals.md#zonestatustype)
- [OpenSearchServiceServiceName](./literals.md#opensearchserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [NaturalLanguageQueryGenerationOptionsInputTypeDef](./type_defs.md#naturallanguagequerygenerationoptionsinputtypedef)
- [NaturalLanguageQueryGenerationOptionsOutputTypeDef](./type_defs.md#naturallanguagequerygenerationoptionsoutputtypedef)
- [OptionStatusTypeDef](./type_defs.md#optionstatustypedef)
- [AWSDomainInformationTypeDef](./type_defs.md#awsdomaininformationtypedef)
- [AcceptInboundConnectionRequestRequestTypeDef](./type_defs.md#acceptinboundconnectionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [AdditionalLimitTypeDef](./type_defs.md#additionallimittypedef)
- [JWTOptionsInputTypeDef](./type_defs.md#jwtoptionsinputtypedef)
- [MasterUserOptionsTypeDef](./type_defs.md#masteruseroptionstypedef)
- [JWTOptionsOutputTypeDef](./type_defs.md#jwtoptionsoutputtypedef)
- [AssociatePackageRequestRequestTypeDef](./type_defs.md#associatepackagerequestrequesttypedef)
- [AuthorizeVpcEndpointAccessRequestRequestTypeDef](./type_defs.md#authorizevpcendpointaccessrequestrequesttypedef)
- [AuthorizedPrincipalTypeDef](./type_defs.md#authorizedprincipaltypedef)
- [ScheduledAutoTuneDetailsTypeDef](./type_defs.md#scheduledautotunedetailstypedef)
- [DurationTypeDef](./type_defs.md#durationtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [AutoTuneOptionsOutputTypeDef](./type_defs.md#autotuneoptionsoutputtypedef)
- [AutoTuneStatusTypeDef](./type_defs.md#autotunestatustypedef)
- [AvailabilityZoneInfoTypeDef](./type_defs.md#availabilityzoneinfotypedef)
- [CancelDomainConfigChangeRequestRequestTypeDef](./type_defs.md#canceldomainconfigchangerequestrequesttypedef)
- [CancelledChangePropertyTypeDef](./type_defs.md#cancelledchangepropertytypedef)
- [CancelServiceSoftwareUpdateRequestRequestTypeDef](./type_defs.md#cancelservicesoftwareupdaterequestrequesttypedef)
- [ServiceSoftwareOptionsTypeDef](./type_defs.md#servicesoftwareoptionstypedef)
- [ChangeProgressDetailsTypeDef](./type_defs.md#changeprogressdetailstypedef)
- [ChangeProgressStageTypeDef](./type_defs.md#changeprogressstagetypedef)
- [ColdStorageOptionsTypeDef](./type_defs.md#coldstorageoptionstypedef)
- [ZoneAwarenessConfigTypeDef](./type_defs.md#zoneawarenessconfigtypedef)
- [CognitoOptionsTypeDef](./type_defs.md#cognitooptionstypedef)
- [CompatibleVersionsMapTypeDef](./type_defs.md#compatibleversionsmaptypedef)
- [CrossClusterSearchConnectionPropertiesTypeDef](./type_defs.md#crossclustersearchconnectionpropertiestypedef)
- [DomainEndpointOptionsTypeDef](./type_defs.md#domainendpointoptionstypedef)
- [EBSOptionsTypeDef](./type_defs.md#ebsoptionstypedef)
- [EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef)
- [LogPublishingOptionTypeDef](./type_defs.md#logpublishingoptiontypedef)
- [NodeToNodeEncryptionOptionsTypeDef](./type_defs.md#nodetonodeencryptionoptionstypedef)
- [SnapshotOptionsTypeDef](./type_defs.md#snapshotoptionstypedef)
- [SoftwareUpdateOptionsTypeDef](./type_defs.md#softwareupdateoptionstypedef)
- [VPCOptionsTypeDef](./type_defs.md#vpcoptionstypedef)
- [OutboundConnectionStatusTypeDef](./type_defs.md#outboundconnectionstatustypedef)
- [PackageSourceTypeDef](./type_defs.md#packagesourcetypedef)
- [S3GlueDataCatalogTypeDef](./type_defs.md#s3gluedatacatalogtypedef)
- [DeleteDataSourceRequestRequestTypeDef](./type_defs.md#deletedatasourcerequestrequesttypedef)
- [DeleteDomainRequestRequestTypeDef](./type_defs.md#deletedomainrequestrequesttypedef)
- [DeleteInboundConnectionRequestRequestTypeDef](./type_defs.md#deleteinboundconnectionrequestrequesttypedef)
- [DeleteOutboundConnectionRequestRequestTypeDef](./type_defs.md#deleteoutboundconnectionrequestrequesttypedef)
- [DeletePackageRequestRequestTypeDef](./type_defs.md#deletepackagerequestrequesttypedef)
- [DeleteVpcEndpointRequestRequestTypeDef](./type_defs.md#deletevpcendpointrequestrequesttypedef)
- [VpcEndpointSummaryTypeDef](./type_defs.md#vpcendpointsummarytypedef)
- [DescribeDomainAutoTunesRequestRequestTypeDef](./type_defs.md#describedomainautotunesrequestrequesttypedef)
- [DescribeDomainChangeProgressRequestRequestTypeDef](./type_defs.md#describedomainchangeprogressrequestrequesttypedef)
- [DescribeDomainConfigRequestRequestTypeDef](./type_defs.md#describedomainconfigrequestrequesttypedef)
- [DescribeDomainHealthRequestRequestTypeDef](./type_defs.md#describedomainhealthrequestrequesttypedef)
- [DescribeDomainNodesRequestRequestTypeDef](./type_defs.md#describedomainnodesrequestrequesttypedef)
- [DomainNodesStatusTypeDef](./type_defs.md#domainnodesstatustypedef)
- [DescribeDomainRequestRequestTypeDef](./type_defs.md#describedomainrequestrequesttypedef)
- [DescribeDomainsRequestRequestTypeDef](./type_defs.md#describedomainsrequestrequesttypedef)
- [DescribeDryRunProgressRequestRequestTypeDef](./type_defs.md#describedryrunprogressrequestrequesttypedef)
- [DryRunResultsTypeDef](./type_defs.md#dryrunresultstypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [DescribeInstanceTypeLimitsRequestRequestTypeDef](./type_defs.md#describeinstancetypelimitsrequestrequesttypedef)
- [DescribePackagesFilterTypeDef](./type_defs.md#describepackagesfiltertypedef)
- [DescribeReservedInstanceOfferingsRequestRequestTypeDef](./type_defs.md#describereservedinstanceofferingsrequestrequesttypedef)
- [DescribeReservedInstancesRequestRequestTypeDef](./type_defs.md#describereservedinstancesrequestrequesttypedef)
- [DescribeVpcEndpointsRequestRequestTypeDef](./type_defs.md#describevpcendpointsrequestrequesttypedef)
- [VpcEndpointErrorTypeDef](./type_defs.md#vpcendpointerrortypedef)
- [DissociatePackageRequestRequestTypeDef](./type_defs.md#dissociatepackagerequestrequesttypedef)
- [ModifyingPropertiesTypeDef](./type_defs.md#modifyingpropertiestypedef)
- [DomainInfoTypeDef](./type_defs.md#domaininfotypedef)
- [DomainMaintenanceDetailsTypeDef](./type_defs.md#domainmaintenancedetailstypedef)
- [ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef)
- [VPCDerivedInfoTypeDef](./type_defs.md#vpcderivedinfotypedef)
- [ValidationFailureTypeDef](./type_defs.md#validationfailuretypedef)
- [GetCompatibleVersionsRequestRequestTypeDef](./type_defs.md#getcompatibleversionsrequestrequesttypedef)
- [GetDataSourceRequestRequestTypeDef](./type_defs.md#getdatasourcerequestrequesttypedef)
- [GetDomainMaintenanceStatusRequestRequestTypeDef](./type_defs.md#getdomainmaintenancestatusrequestrequesttypedef)
- [GetPackageVersionHistoryRequestRequestTypeDef](./type_defs.md#getpackageversionhistoryrequestrequesttypedef)
- [GetUpgradeHistoryRequestRequestTypeDef](./type_defs.md#getupgradehistoryrequestrequesttypedef)
- [GetUpgradeStatusRequestRequestTypeDef](./type_defs.md#getupgradestatusrequestrequesttypedef)
- [InboundConnectionStatusTypeDef](./type_defs.md#inboundconnectionstatustypedef)
- [InstanceCountLimitsTypeDef](./type_defs.md#instancecountlimitstypedef)
- [InstanceTypeDetailsTypeDef](./type_defs.md#instancetypedetailstypedef)
- [ListDataSourcesRequestRequestTypeDef](./type_defs.md#listdatasourcesrequestrequesttypedef)
- [ListDomainMaintenancesRequestRequestTypeDef](./type_defs.md#listdomainmaintenancesrequestrequesttypedef)
- [ListDomainNamesRequestRequestTypeDef](./type_defs.md#listdomainnamesrequestrequesttypedef)
- [ListDomainsForPackageRequestRequestTypeDef](./type_defs.md#listdomainsforpackagerequestrequesttypedef)
- [ListInstanceTypeDetailsRequestRequestTypeDef](./type_defs.md#listinstancetypedetailsrequestrequesttypedef)
- [ListPackagesForDomainRequestRequestTypeDef](./type_defs.md#listpackagesfordomainrequestrequesttypedef)
- [ListScheduledActionsRequestRequestTypeDef](./type_defs.md#listscheduledactionsrequestrequesttypedef)
- [ScheduledActionTypeDef](./type_defs.md#scheduledactiontypedef)
- [ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef)
- [ListVersionsRequestRequestTypeDef](./type_defs.md#listversionsrequestrequesttypedef)
- [ListVpcEndpointAccessRequestRequestTypeDef](./type_defs.md#listvpcendpointaccessrequestrequesttypedef)
- [ListVpcEndpointsForDomainRequestRequestTypeDef](./type_defs.md#listvpcendpointsfordomainrequestrequesttypedef)
- [ListVpcEndpointsRequestRequestTypeDef](./type_defs.md#listvpcendpointsrequestrequesttypedef)
- [WindowStartTimeTypeDef](./type_defs.md#windowstarttimetypedef)
- [PluginPropertiesTypeDef](./type_defs.md#pluginpropertiestypedef)
- [PurchaseReservedInstanceOfferingRequestRequestTypeDef](./type_defs.md#purchasereservedinstanceofferingrequestrequesttypedef)
- [RecurringChargeTypeDef](./type_defs.md#recurringchargetypedef)
- [RejectInboundConnectionRequestRequestTypeDef](./type_defs.md#rejectinboundconnectionrequestrequesttypedef)
- [RemoveTagsRequestRequestTypeDef](./type_defs.md#removetagsrequestrequesttypedef)
- [RevokeVpcEndpointAccessRequestRequestTypeDef](./type_defs.md#revokevpcendpointaccessrequestrequesttypedef)
- [SAMLIdpTypeDef](./type_defs.md#samlidptypedef)
- [StartDomainMaintenanceRequestRequestTypeDef](./type_defs.md#startdomainmaintenancerequestrequesttypedef)
- [StartServiceSoftwareUpdateRequestRequestTypeDef](./type_defs.md#startservicesoftwareupdaterequestrequesttypedef)
- [StorageTypeLimitTypeDef](./type_defs.md#storagetypelimittypedef)
- [UpdateScheduledActionRequestRequestTypeDef](./type_defs.md#updatescheduledactionrequestrequesttypedef)
- [UpgradeDomainRequestRequestTypeDef](./type_defs.md#upgradedomainrequestrequesttypedef)
- [UpgradeStepItemTypeDef](./type_defs.md#upgradestepitemtypedef)
- [AIMLOptionsInputTypeDef](./type_defs.md#aimloptionsinputtypedef)
- [AIMLOptionsOutputTypeDef](./type_defs.md#aimloptionsoutputtypedef)
- [AccessPoliciesStatusTypeDef](./type_defs.md#accesspoliciesstatustypedef)
- [AdvancedOptionsStatusTypeDef](./type_defs.md#advancedoptionsstatustypedef)
- [IPAddressTypeStatusTypeDef](./type_defs.md#ipaddresstypestatustypedef)
- [VersionStatusTypeDef](./type_defs.md#versionstatustypedef)
- [DomainInformationContainerTypeDef](./type_defs.md#domaininformationcontainertypedef)
- [AddDataSourceResponseTypeDef](./type_defs.md#adddatasourceresponsetypedef)
- [DeleteDataSourceResponseTypeDef](./type_defs.md#deletedatasourceresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetDomainMaintenanceStatusResponseTypeDef](./type_defs.md#getdomainmaintenancestatusresponsetypedef)
- [GetUpgradeStatusResponseTypeDef](./type_defs.md#getupgradestatusresponsetypedef)
- [ListVersionsResponseTypeDef](./type_defs.md#listversionsresponsetypedef)
- [PurchaseReservedInstanceOfferingResponseTypeDef](./type_defs.md#purchasereservedinstanceofferingresponsetypedef)
- [StartDomainMaintenanceResponseTypeDef](./type_defs.md#startdomainmaintenanceresponsetypedef)
- [UpdateDataSourceResponseTypeDef](./type_defs.md#updatedatasourceresponsetypedef)
- [AddTagsRequestRequestTypeDef](./type_defs.md#addtagsrequestrequesttypedef)
- [ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef)
- [AuthorizeVpcEndpointAccessResponseTypeDef](./type_defs.md#authorizevpcendpointaccessresponsetypedef)
- [ListVpcEndpointAccessResponseTypeDef](./type_defs.md#listvpcendpointaccessresponsetypedef)
- [AutoTuneDetailsTypeDef](./type_defs.md#autotunedetailstypedef)
- [AutoTuneMaintenanceScheduleOutputTypeDef](./type_defs.md#autotunemaintenancescheduleoutputtypedef)
- [AutoTuneMaintenanceScheduleTypeDef](./type_defs.md#autotunemaintenancescheduletypedef)
- [EnvironmentInfoTypeDef](./type_defs.md#environmentinfotypedef)
- [CancelDomainConfigChangeResponseTypeDef](./type_defs.md#canceldomainconfigchangeresponsetypedef)
- [CancelServiceSoftwareUpdateResponseTypeDef](./type_defs.md#cancelservicesoftwareupdateresponsetypedef)
- [StartServiceSoftwareUpdateResponseTypeDef](./type_defs.md#startservicesoftwareupdateresponsetypedef)
- [UpgradeDomainResponseTypeDef](./type_defs.md#upgradedomainresponsetypedef)
- [ChangeProgressStatusDetailsTypeDef](./type_defs.md#changeprogressstatusdetailstypedef)
- [ClusterConfigTypeDef](./type_defs.md#clusterconfigtypedef)
- [CognitoOptionsStatusTypeDef](./type_defs.md#cognitooptionsstatustypedef)
- [GetCompatibleVersionsResponseTypeDef](./type_defs.md#getcompatibleversionsresponsetypedef)
- [ConnectionPropertiesTypeDef](./type_defs.md#connectionpropertiestypedef)
- [DomainEndpointOptionsStatusTypeDef](./type_defs.md#domainendpointoptionsstatustypedef)
- [EBSOptionsStatusTypeDef](./type_defs.md#ebsoptionsstatustypedef)
- [EncryptionAtRestOptionsStatusTypeDef](./type_defs.md#encryptionatrestoptionsstatustypedef)
- [LogPublishingOptionsStatusTypeDef](./type_defs.md#logpublishingoptionsstatustypedef)
- [NodeToNodeEncryptionOptionsStatusTypeDef](./type_defs.md#nodetonodeencryptionoptionsstatustypedef)
- [SnapshotOptionsStatusTypeDef](./type_defs.md#snapshotoptionsstatustypedef)
- [SoftwareUpdateOptionsStatusTypeDef](./type_defs.md#softwareupdateoptionsstatustypedef)
- [CreateVpcEndpointRequestRequestTypeDef](./type_defs.md#createvpcendpointrequestrequesttypedef)
- [UpdateVpcEndpointRequestRequestTypeDef](./type_defs.md#updatevpcendpointrequestrequesttypedef)
- [CreatePackageRequestRequestTypeDef](./type_defs.md#createpackagerequestrequesttypedef)
- [UpdatePackageRequestRequestTypeDef](./type_defs.md#updatepackagerequestrequesttypedef)
- [DataSourceTypeTypeDef](./type_defs.md#datasourcetypetypedef)
- [DeleteVpcEndpointResponseTypeDef](./type_defs.md#deletevpcendpointresponsetypedef)
- [ListVpcEndpointsForDomainResponseTypeDef](./type_defs.md#listvpcendpointsfordomainresponsetypedef)
- [ListVpcEndpointsResponseTypeDef](./type_defs.md#listvpcendpointsresponsetypedef)
- [DescribeDomainNodesResponseTypeDef](./type_defs.md#describedomainnodesresponsetypedef)
- [DescribeInboundConnectionsRequestRequestTypeDef](./type_defs.md#describeinboundconnectionsrequestrequesttypedef)
- [DescribeOutboundConnectionsRequestRequestTypeDef](./type_defs.md#describeoutboundconnectionsrequestrequesttypedef)
- [DescribePackagesRequestRequestTypeDef](./type_defs.md#describepackagesrequestrequesttypedef)
- [ListDomainNamesResponseTypeDef](./type_defs.md#listdomainnamesresponsetypedef)
- [ListDomainMaintenancesResponseTypeDef](./type_defs.md#listdomainmaintenancesresponsetypedef)
- [DomainPackageDetailsTypeDef](./type_defs.md#domainpackagedetailstypedef)
- [VPCDerivedInfoStatusTypeDef](./type_defs.md#vpcderivedinfostatustypedef)
- [VpcEndpointTypeDef](./type_defs.md#vpcendpointtypedef)
- [DryRunProgressStatusTypeDef](./type_defs.md#dryrunprogressstatustypedef)
- [InstanceLimitsTypeDef](./type_defs.md#instancelimitstypedef)
- [ListInstanceTypeDetailsResponseTypeDef](./type_defs.md#listinstancetypedetailsresponsetypedef)
- [ListScheduledActionsResponseTypeDef](./type_defs.md#listscheduledactionsresponsetypedef)
- [UpdateScheduledActionResponseTypeDef](./type_defs.md#updatescheduledactionresponsetypedef)
- [OffPeakWindowTypeDef](./type_defs.md#offpeakwindowtypedef)
- [PackageDetailsTypeDef](./type_defs.md#packagedetailstypedef)
- [PackageVersionHistoryTypeDef](./type_defs.md#packageversionhistorytypedef)
- [ReservedInstanceOfferingTypeDef](./type_defs.md#reservedinstanceofferingtypedef)
- [ReservedInstanceTypeDef](./type_defs.md#reservedinstancetypedef)
- [SAMLOptionsInputTypeDef](./type_defs.md#samloptionsinputtypedef)
- [SAMLOptionsOutputTypeDef](./type_defs.md#samloptionsoutputtypedef)
- [StorageTypeTypeDef](./type_defs.md#storagetypetypedef)
- [UpgradeHistoryTypeDef](./type_defs.md#upgradehistorytypedef)
- [AIMLOptionsStatusTypeDef](./type_defs.md#aimloptionsstatustypedef)
- [InboundConnectionTypeDef](./type_defs.md#inboundconnectiontypedef)
- [AutoTuneTypeDef](./type_defs.md#autotunetypedef)
- [AutoTuneOptionsExtraOutputTypeDef](./type_defs.md#autotuneoptionsextraoutputtypedef)
- [AutoTuneMaintenanceScheduleUnionTypeDef](./type_defs.md#autotunemaintenancescheduleuniontypedef)
- [DescribeDomainHealthResponseTypeDef](./type_defs.md#describedomainhealthresponsetypedef)
- [DescribeDomainChangeProgressResponseTypeDef](./type_defs.md#describedomainchangeprogressresponsetypedef)
- [ClusterConfigStatusTypeDef](./type_defs.md#clusterconfigstatustypedef)
- [CreateOutboundConnectionRequestRequestTypeDef](./type_defs.md#createoutboundconnectionrequestrequesttypedef)
- [CreateOutboundConnectionResponseTypeDef](./type_defs.md#createoutboundconnectionresponsetypedef)
- [OutboundConnectionTypeDef](./type_defs.md#outboundconnectiontypedef)
- [AddDataSourceRequestRequestTypeDef](./type_defs.md#adddatasourcerequestrequesttypedef)
- [DataSourceDetailsTypeDef](./type_defs.md#datasourcedetailstypedef)
- [GetDataSourceResponseTypeDef](./type_defs.md#getdatasourceresponsetypedef)
- [UpdateDataSourceRequestRequestTypeDef](./type_defs.md#updatedatasourcerequestrequesttypedef)
- [AssociatePackageResponseTypeDef](./type_defs.md#associatepackageresponsetypedef)
- [DissociatePackageResponseTypeDef](./type_defs.md#dissociatepackageresponsetypedef)
- [ListDomainsForPackageResponseTypeDef](./type_defs.md#listdomainsforpackageresponsetypedef)
- [ListPackagesForDomainResponseTypeDef](./type_defs.md#listpackagesfordomainresponsetypedef)
- [CreateVpcEndpointResponseTypeDef](./type_defs.md#createvpcendpointresponsetypedef)
- [DescribeVpcEndpointsResponseTypeDef](./type_defs.md#describevpcendpointsresponsetypedef)
- [UpdateVpcEndpointResponseTypeDef](./type_defs.md#updatevpcendpointresponsetypedef)
- [OffPeakWindowOptionsTypeDef](./type_defs.md#offpeakwindowoptionstypedef)
- [CreatePackageResponseTypeDef](./type_defs.md#createpackageresponsetypedef)
- [DeletePackageResponseTypeDef](./type_defs.md#deletepackageresponsetypedef)
- [DescribePackagesResponseTypeDef](./type_defs.md#describepackagesresponsetypedef)
- [UpdatePackageResponseTypeDef](./type_defs.md#updatepackageresponsetypedef)
- [GetPackageVersionHistoryResponseTypeDef](./type_defs.md#getpackageversionhistoryresponsetypedef)
- [DescribeReservedInstanceOfferingsResponseTypeDef](./type_defs.md#describereservedinstanceofferingsresponsetypedef)
- [DescribeReservedInstancesResponseTypeDef](./type_defs.md#describereservedinstancesresponsetypedef)
- [AdvancedSecurityOptionsInputTypeDef](./type_defs.md#advancedsecurityoptionsinputtypedef)
- [AdvancedSecurityOptionsTypeDef](./type_defs.md#advancedsecurityoptionstypedef)
- [LimitsTypeDef](./type_defs.md#limitstypedef)
- [GetUpgradeHistoryResponseTypeDef](./type_defs.md#getupgradehistoryresponsetypedef)
- [AcceptInboundConnectionResponseTypeDef](./type_defs.md#acceptinboundconnectionresponsetypedef)
- [DeleteInboundConnectionResponseTypeDef](./type_defs.md#deleteinboundconnectionresponsetypedef)
- [DescribeInboundConnectionsResponseTypeDef](./type_defs.md#describeinboundconnectionsresponsetypedef)
- [RejectInboundConnectionResponseTypeDef](./type_defs.md#rejectinboundconnectionresponsetypedef)
- [DescribeDomainAutoTunesResponseTypeDef](./type_defs.md#describedomainautotunesresponsetypedef)
- [AutoTuneOptionsStatusTypeDef](./type_defs.md#autotuneoptionsstatustypedef)
- [AutoTuneOptionsInputTypeDef](./type_defs.md#autotuneoptionsinputtypedef)
- [AutoTuneOptionsTypeDef](./type_defs.md#autotuneoptionstypedef)
- [DeleteOutboundConnectionResponseTypeDef](./type_defs.md#deleteoutboundconnectionresponsetypedef)
- [DescribeOutboundConnectionsResponseTypeDef](./type_defs.md#describeoutboundconnectionsresponsetypedef)
- [ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef)
- [OffPeakWindowOptionsStatusTypeDef](./type_defs.md#offpeakwindowoptionsstatustypedef)
- [AdvancedSecurityOptionsStatusTypeDef](./type_defs.md#advancedsecurityoptionsstatustypedef)
- [DomainStatusTypeDef](./type_defs.md#domainstatustypedef)
- [DescribeInstanceTypeLimitsResponseTypeDef](./type_defs.md#describeinstancetypelimitsresponsetypedef)
- [CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef)
- [UpdateDomainConfigRequestRequestTypeDef](./type_defs.md#updatedomainconfigrequestrequesttypedef)
- [DomainConfigTypeDef](./type_defs.md#domainconfigtypedef)
- [CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef)
- [DeleteDomainResponseTypeDef](./type_defs.md#deletedomainresponsetypedef)
- [DescribeDomainResponseTypeDef](./type_defs.md#describedomainresponsetypedef)
- [DescribeDomainsResponseTypeDef](./type_defs.md#describedomainsresponsetypedef)
- [DescribeDryRunProgressResponseTypeDef](./type_defs.md#describedryrunprogressresponsetypedef)
- [DescribeDomainConfigResponseTypeDef](./type_defs.md#describedomainconfigresponsetypedef)
- [UpdateDomainConfigResponseTypeDef](./type_defs.md#updatedomainconfigresponsetypedef)

