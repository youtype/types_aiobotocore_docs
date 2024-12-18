# AppStream module

> [Index](../README.md) > AppStream


!!! note ""

    Auto-generated documentation for [AppStream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#appstream)
    type annotations stubs module [types-aiobotocore-appstream](https://pypi.org/project/types-aiobotocore-appstream/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `AppStream` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `AppStream` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[appstream]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[appstream]'

# standalone installation
python -m pip install types-aiobotocore-appstream
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-appstream
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AppStreamClient

Type annotations and code completion for  `#!python session.create_client("appstream")` as [AppStreamClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client)

```python
# AppStreamClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_appstream.client import AppStreamClient


session = get_session()
async with session.create_client("appstream") as client:
    client: AppStreamClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("appstream").get_paginator("...")`.

```python
# DescribeDirectoryConfigsPaginator usage example

from types_aiobotocore_appstream.paginator import DescribeDirectoryConfigsPaginator

def get_describe_directory_configs_paginator() -> DescribeDirectoryConfigsPaginator:
    return client.get_paginator("describe_directory_configs"))
```

- [DescribeDirectoryConfigsPaginator](./paginators.md#describedirectoryconfigspaginator)
- [DescribeFleetsPaginator](./paginators.md#describefleetspaginator)
- [DescribeImageBuildersPaginator](./paginators.md#describeimagebuilderspaginator)
- [DescribeImagesPaginator](./paginators.md#describeimagespaginator)
- [DescribeSessionsPaginator](./paginators.md#describesessionspaginator)
- [DescribeStacksPaginator](./paginators.md#describestackspaginator)
- [DescribeUserStackAssociationsPaginator](./paginators.md#describeuserstackassociationspaginator)
- [DescribeUsersPaginator](./paginators.md#describeuserspaginator)
- [ListAssociatedFleetsPaginator](./paginators.md#listassociatedfleetspaginator)
- [ListAssociatedStacksPaginator](./paginators.md#listassociatedstackspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("appstream").get_waiter("...")`.

```python
# FleetStartedWaiter usage example

from types_aiobotocore_appstream.waiter import FleetStartedWaiter

def get_fleet_started_waiter() -> FleetStartedWaiter:
    return Session().client("appstream").get_waiter("fleet_started")
```

- [FleetStartedWaiter](./waiters.md#fleetstartedwaiter)
- [FleetStoppedWaiter](./waiters.md#fleetstoppedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccessEndpointTypeType usage example

from types_aiobotocore_appstream.literals import AccessEndpointTypeType

def get_value() -> AccessEndpointTypeType:
    return "STREAMING"
```

- [AccessEndpointTypeType](./literals.md#accessendpointtypetype)
- [ActionType](./literals.md#actiontype)
- [AppBlockBuilderAttributeType](./literals.md#appblockbuilderattributetype)
- [AppBlockBuilderPlatformTypeType](./literals.md#appblockbuilderplatformtypetype)
- [AppBlockBuilderStateChangeReasonCodeType](./literals.md#appblockbuilderstatechangereasoncodetype)
- [AppBlockBuilderStateType](./literals.md#appblockbuilderstatetype)
- [AppBlockStateType](./literals.md#appblockstatetype)
- [AppVisibilityType](./literals.md#appvisibilitytype)
- [ApplicationAttributeType](./literals.md#applicationattributetype)
- [AuthenticationTypeType](./literals.md#authenticationtypetype)
- [CertificateBasedAuthStatusType](./literals.md#certificatebasedauthstatustype)
- [DescribeDirectoryConfigsPaginatorName](./literals.md#describedirectoryconfigspaginatorname)
- [DescribeFleetsPaginatorName](./literals.md#describefleetspaginatorname)
- [DescribeImageBuildersPaginatorName](./literals.md#describeimagebuilderspaginatorname)
- [DescribeImagesPaginatorName](./literals.md#describeimagespaginatorname)
- [DescribeSessionsPaginatorName](./literals.md#describesessionspaginatorname)
- [DescribeStacksPaginatorName](./literals.md#describestackspaginatorname)
- [DescribeUserStackAssociationsPaginatorName](./literals.md#describeuserstackassociationspaginatorname)
- [DescribeUsersPaginatorName](./literals.md#describeuserspaginatorname)
- [DynamicAppProvidersEnabledType](./literals.md#dynamicappprovidersenabledtype)
- [FleetAttributeType](./literals.md#fleetattributetype)
- [FleetErrorCodeType](./literals.md#fleeterrorcodetype)
- [FleetStartedWaiterName](./literals.md#fleetstartedwaitername)
- [FleetStateType](./literals.md#fleetstatetype)
- [FleetStoppedWaiterName](./literals.md#fleetstoppedwaitername)
- [FleetTypeType](./literals.md#fleettypetype)
- [ImageBuilderStateChangeReasonCodeType](./literals.md#imagebuilderstatechangereasoncodetype)
- [ImageBuilderStateType](./literals.md#imagebuilderstatetype)
- [ImageSharedWithOthersType](./literals.md#imagesharedwithotherstype)
- [ImageStateChangeReasonCodeType](./literals.md#imagestatechangereasoncodetype)
- [ImageStateType](./literals.md#imagestatetype)
- [LatestAppstreamAgentVersionType](./literals.md#latestappstreamagentversiontype)
- [ListAssociatedFleetsPaginatorName](./literals.md#listassociatedfleetspaginatorname)
- [ListAssociatedStacksPaginatorName](./literals.md#listassociatedstackspaginatorname)
- [MessageActionType](./literals.md#messageactiontype)
- [PackagingTypeType](./literals.md#packagingtypetype)
- [PermissionType](./literals.md#permissiontype)
- [PlatformTypeType](./literals.md#platformtypetype)
- [PreferredProtocolType](./literals.md#preferredprotocoltype)
- [SessionConnectionStateType](./literals.md#sessionconnectionstatetype)
- [SessionStateType](./literals.md#sessionstatetype)
- [StackAttributeType](./literals.md#stackattributetype)
- [StackErrorCodeType](./literals.md#stackerrorcodetype)
- [StorageConnectorTypeType](./literals.md#storageconnectortypetype)
- [StreamViewType](./literals.md#streamviewtype)
- [ThemeAttributeType](./literals.md#themeattributetype)
- [ThemeStateType](./literals.md#themestatetype)
- [ThemeStylingType](./literals.md#themestylingtype)
- [UsageReportExecutionErrorCodeType](./literals.md#usagereportexecutionerrorcodetype)
- [UsageReportScheduleType](./literals.md#usagereportscheduletype)
- [UserStackAssociationErrorCodeType](./literals.md#userstackassociationerrorcodetype)
- [VisibilityTypeType](./literals.md#visibilitytypetype)
- [AppStreamServiceName](./literals.md#appstreamservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessEndpointTypeDef](./type_defs.md#accessendpointtypedef)
- [AppBlockBuilderAppBlockAssociationTypeDef](./type_defs.md#appblockbuilderappblockassociationtypedef)
- [AppBlockBuilderStateChangeReasonTypeDef](./type_defs.md#appblockbuilderstatechangereasontypedef)
- [ResourceErrorTypeDef](./type_defs.md#resourceerrortypedef)
- [VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
- [ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [ApplicationFleetAssociationTypeDef](./type_defs.md#applicationfleetassociationtypedef)
- [ApplicationSettingsResponseTypeDef](./type_defs.md#applicationsettingsresponsetypedef)
- [ApplicationSettingsTypeDef](./type_defs.md#applicationsettingstypedef)
- [AssociateAppBlockBuilderAppBlockRequestRequestTypeDef](./type_defs.md#associateappblockbuilderappblockrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AssociateApplicationFleetRequestRequestTypeDef](./type_defs.md#associateapplicationfleetrequestrequesttypedef)
- [AssociateApplicationToEntitlementRequestRequestTypeDef](./type_defs.md#associateapplicationtoentitlementrequestrequesttypedef)
- [AssociateFleetRequestRequestTypeDef](./type_defs.md#associatefleetrequestrequesttypedef)
- [UserStackAssociationTypeDef](./type_defs.md#userstackassociationtypedef)
- [CertificateBasedAuthPropertiesTypeDef](./type_defs.md#certificatebasedauthpropertiestypedef)
- [ComputeCapacityStatusTypeDef](./type_defs.md#computecapacitystatustypedef)
- [ComputeCapacityTypeDef](./type_defs.md#computecapacitytypedef)
- [CopyImageRequestRequestTypeDef](./type_defs.md#copyimagerequestrequesttypedef)
- [VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- [CreateAppBlockBuilderStreamingURLRequestRequestTypeDef](./type_defs.md#createappblockbuilderstreamingurlrequestrequesttypedef)
- [ServiceAccountCredentialsTypeDef](./type_defs.md#serviceaccountcredentialstypedef)
- [EntitlementAttributeTypeDef](./type_defs.md#entitlementattributetypedef)
- [DomainJoinInfoTypeDef](./type_defs.md#domainjoininfotypedef)
- [CreateImageBuilderStreamingURLRequestRequestTypeDef](./type_defs.md#createimagebuilderstreamingurlrequestrequesttypedef)
- [StreamingExperienceSettingsTypeDef](./type_defs.md#streamingexperiencesettingstypedef)
- [UserSettingTypeDef](./type_defs.md#usersettingtypedef)
- [CreateStreamingURLRequestRequestTypeDef](./type_defs.md#createstreamingurlrequestrequesttypedef)
- [ThemeFooterLinkTypeDef](./type_defs.md#themefooterlinktypedef)
- [CreateUpdatedImageRequestRequestTypeDef](./type_defs.md#createupdatedimagerequestrequesttypedef)
- [CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef)
- [DeleteAppBlockBuilderRequestRequestTypeDef](./type_defs.md#deleteappblockbuilderrequestrequesttypedef)
- [DeleteAppBlockRequestRequestTypeDef](./type_defs.md#deleteappblockrequestrequesttypedef)
- [DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef)
- [DeleteDirectoryConfigRequestRequestTypeDef](./type_defs.md#deletedirectoryconfigrequestrequesttypedef)
- [DeleteEntitlementRequestRequestTypeDef](./type_defs.md#deleteentitlementrequestrequesttypedef)
- [DeleteFleetRequestRequestTypeDef](./type_defs.md#deletefleetrequestrequesttypedef)
- [DeleteImageBuilderRequestRequestTypeDef](./type_defs.md#deleteimagebuilderrequestrequesttypedef)
- [DeleteImagePermissionsRequestRequestTypeDef](./type_defs.md#deleteimagepermissionsrequestrequesttypedef)
- [DeleteImageRequestRequestTypeDef](./type_defs.md#deleteimagerequestrequesttypedef)
- [DeleteStackRequestRequestTypeDef](./type_defs.md#deletestackrequestrequesttypedef)
- [DeleteThemeForStackRequestRequestTypeDef](./type_defs.md#deletethemeforstackrequestrequesttypedef)
- [DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef)
- [DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef](./type_defs.md#describeappblockbuilderappblockassociationsrequestrequesttypedef)
- [DescribeAppBlockBuildersRequestRequestTypeDef](./type_defs.md#describeappblockbuildersrequestrequesttypedef)
- [DescribeAppBlocksRequestRequestTypeDef](./type_defs.md#describeappblocksrequestrequesttypedef)
- [DescribeApplicationFleetAssociationsRequestRequestTypeDef](./type_defs.md#describeapplicationfleetassociationsrequestrequesttypedef)
- [DescribeApplicationsRequestRequestTypeDef](./type_defs.md#describeapplicationsrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeDirectoryConfigsRequestRequestTypeDef](./type_defs.md#describedirectoryconfigsrequestrequesttypedef)
- [DescribeEntitlementsRequestRequestTypeDef](./type_defs.md#describeentitlementsrequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeFleetsRequestRequestTypeDef](./type_defs.md#describefleetsrequestrequesttypedef)
- [DescribeImageBuildersRequestRequestTypeDef](./type_defs.md#describeimagebuildersrequestrequesttypedef)
- [DescribeImagePermissionsRequestRequestTypeDef](./type_defs.md#describeimagepermissionsrequestrequesttypedef)
- [DescribeImagesRequestRequestTypeDef](./type_defs.md#describeimagesrequestrequesttypedef)
- [DescribeSessionsRequestRequestTypeDef](./type_defs.md#describesessionsrequestrequesttypedef)
- [DescribeStacksRequestRequestTypeDef](./type_defs.md#describestacksrequestrequesttypedef)
- [DescribeThemeForStackRequestRequestTypeDef](./type_defs.md#describethemeforstackrequestrequesttypedef)
- [DescribeUsageReportSubscriptionsRequestRequestTypeDef](./type_defs.md#describeusagereportsubscriptionsrequestrequesttypedef)
- [DescribeUserStackAssociationsRequestRequestTypeDef](./type_defs.md#describeuserstackassociationsrequestrequesttypedef)
- [DescribeUsersRequestRequestTypeDef](./type_defs.md#describeusersrequestrequesttypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
- [DisableUserRequestRequestTypeDef](./type_defs.md#disableuserrequestrequesttypedef)
- [DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef](./type_defs.md#disassociateappblockbuilderappblockrequestrequesttypedef)
- [DisassociateApplicationFleetRequestRequestTypeDef](./type_defs.md#disassociateapplicationfleetrequestrequesttypedef)
- [DisassociateApplicationFromEntitlementRequestRequestTypeDef](./type_defs.md#disassociateapplicationfromentitlementrequestrequesttypedef)
- [DisassociateFleetRequestRequestTypeDef](./type_defs.md#disassociatefleetrequestrequesttypedef)
- [EnableUserRequestRequestTypeDef](./type_defs.md#enableuserrequestrequesttypedef)
- [EntitledApplicationTypeDef](./type_defs.md#entitledapplicationtypedef)
- [ExpireSessionRequestRequestTypeDef](./type_defs.md#expiresessionrequestrequesttypedef)
- [FleetErrorTypeDef](./type_defs.md#fleeterrortypedef)
- [ImageBuilderStateChangeReasonTypeDef](./type_defs.md#imagebuilderstatechangereasontypedef)
- [NetworkAccessConfigurationTypeDef](./type_defs.md#networkaccessconfigurationtypedef)
- [ImagePermissionsTypeDef](./type_defs.md#imagepermissionstypedef)
- [ImageStateChangeReasonTypeDef](./type_defs.md#imagestatechangereasontypedef)
- [LastReportGenerationExecutionErrorTypeDef](./type_defs.md#lastreportgenerationexecutionerrortypedef)
- [ListAssociatedFleetsRequestRequestTypeDef](./type_defs.md#listassociatedfleetsrequestrequesttypedef)
- [ListAssociatedStacksRequestRequestTypeDef](./type_defs.md#listassociatedstacksrequestrequesttypedef)
- [ListEntitledApplicationsRequestRequestTypeDef](./type_defs.md#listentitledapplicationsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [StackErrorTypeDef](./type_defs.md#stackerrortypedef)
- [StorageConnectorOutputTypeDef](./type_defs.md#storageconnectoroutputtypedef)
- [StartAppBlockBuilderRequestRequestTypeDef](./type_defs.md#startappblockbuilderrequestrequesttypedef)
- [StartFleetRequestRequestTypeDef](./type_defs.md#startfleetrequestrequesttypedef)
- [StartImageBuilderRequestRequestTypeDef](./type_defs.md#startimagebuilderrequestrequesttypedef)
- [StopAppBlockBuilderRequestRequestTypeDef](./type_defs.md#stopappblockbuilderrequestrequesttypedef)
- [StopFleetRequestRequestTypeDef](./type_defs.md#stopfleetrequestrequesttypedef)
- [StopImageBuilderRequestRequestTypeDef](./type_defs.md#stopimagebuilderrequestrequesttypedef)
- [StorageConnectorTypeDef](./type_defs.md#storageconnectortypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AppBlockBuilderTypeDef](./type_defs.md#appblockbuildertypedef)
- [ApplicationTypeDef](./type_defs.md#applicationtypedef)
- [CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef)
- [ScriptDetailsTypeDef](./type_defs.md#scriptdetailstypedef)
- [UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef)
- [AssociateAppBlockBuilderAppBlockResultTypeDef](./type_defs.md#associateappblockbuilderappblockresulttypedef)
- [AssociateApplicationFleetResultTypeDef](./type_defs.md#associateapplicationfleetresulttypedef)
- [CopyImageResponseTypeDef](./type_defs.md#copyimageresponsetypedef)
- [CreateAppBlockBuilderStreamingURLResultTypeDef](./type_defs.md#createappblockbuilderstreamingurlresulttypedef)
- [CreateImageBuilderStreamingURLResultTypeDef](./type_defs.md#createimagebuilderstreamingurlresulttypedef)
- [CreateStreamingURLResultTypeDef](./type_defs.md#createstreamingurlresulttypedef)
- [CreateUsageReportSubscriptionResultTypeDef](./type_defs.md#createusagereportsubscriptionresulttypedef)
- [DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef](./type_defs.md#describeappblockbuilderappblockassociationsresulttypedef)
- [DescribeApplicationFleetAssociationsResultTypeDef](./type_defs.md#describeapplicationfleetassociationsresulttypedef)
- [ListAssociatedFleetsResultTypeDef](./type_defs.md#listassociatedfleetsresulttypedef)
- [ListAssociatedStacksResultTypeDef](./type_defs.md#listassociatedstacksresulttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [BatchAssociateUserStackRequestRequestTypeDef](./type_defs.md#batchassociateuserstackrequestrequesttypedef)
- [BatchDisassociateUserStackRequestRequestTypeDef](./type_defs.md#batchdisassociateuserstackrequestrequesttypedef)
- [DescribeUserStackAssociationsResultTypeDef](./type_defs.md#describeuserstackassociationsresulttypedef)
- [UserStackAssociationErrorTypeDef](./type_defs.md#userstackassociationerrortypedef)
- [CreateAppBlockBuilderRequestRequestTypeDef](./type_defs.md#createappblockbuilderrequestrequesttypedef)
- [UpdateAppBlockBuilderRequestRequestTypeDef](./type_defs.md#updateappblockbuilderrequestrequesttypedef)
- [CreateDirectoryConfigRequestRequestTypeDef](./type_defs.md#createdirectoryconfigrequestrequesttypedef)
- [DirectoryConfigTypeDef](./type_defs.md#directoryconfigtypedef)
- [UpdateDirectoryConfigRequestRequestTypeDef](./type_defs.md#updatedirectoryconfigrequestrequesttypedef)
- [CreateEntitlementRequestRequestTypeDef](./type_defs.md#createentitlementrequestrequesttypedef)
- [EntitlementTypeDef](./type_defs.md#entitlementtypedef)
- [UpdateEntitlementRequestRequestTypeDef](./type_defs.md#updateentitlementrequestrequesttypedef)
- [CreateFleetRequestRequestTypeDef](./type_defs.md#createfleetrequestrequesttypedef)
- [CreateImageBuilderRequestRequestTypeDef](./type_defs.md#createimagebuilderrequestrequesttypedef)
- [UpdateFleetRequestRequestTypeDef](./type_defs.md#updatefleetrequestrequesttypedef)
- [CreateThemeForStackRequestRequestTypeDef](./type_defs.md#createthemeforstackrequestrequesttypedef)
- [ThemeTypeDef](./type_defs.md#themetypedef)
- [UpdateThemeForStackRequestRequestTypeDef](./type_defs.md#updatethemeforstackrequestrequesttypedef)
- [DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef](./type_defs.md#describedirectoryconfigsrequestdescribedirectoryconfigspaginatetypedef)
- [DescribeFleetsRequestDescribeFleetsPaginateTypeDef](./type_defs.md#describefleetsrequestdescribefleetspaginatetypedef)
- [DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef](./type_defs.md#describeimagebuildersrequestdescribeimagebuilderspaginatetypedef)
- [DescribeImagesRequestDescribeImagesPaginateTypeDef](./type_defs.md#describeimagesrequestdescribeimagespaginatetypedef)
- [DescribeSessionsRequestDescribeSessionsPaginateTypeDef](./type_defs.md#describesessionsrequestdescribesessionspaginatetypedef)
- [DescribeStacksRequestDescribeStacksPaginateTypeDef](./type_defs.md#describestacksrequestdescribestackspaginatetypedef)
- [DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef](./type_defs.md#describeuserstackassociationsrequestdescribeuserstackassociationspaginatetypedef)
- [DescribeUsersRequestDescribeUsersPaginateTypeDef](./type_defs.md#describeusersrequestdescribeuserspaginatetypedef)
- [ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef](./type_defs.md#listassociatedfleetsrequestlistassociatedfleetspaginatetypedef)
- [ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef](./type_defs.md#listassociatedstacksrequestlistassociatedstackspaginatetypedef)
- [DescribeFleetsRequestFleetStartedWaitTypeDef](./type_defs.md#describefleetsrequestfleetstartedwaittypedef)
- [DescribeFleetsRequestFleetStoppedWaitTypeDef](./type_defs.md#describefleetsrequestfleetstoppedwaittypedef)
- [DescribeUsersResultTypeDef](./type_defs.md#describeusersresulttypedef)
- [ListEntitledApplicationsResultTypeDef](./type_defs.md#listentitledapplicationsresulttypedef)
- [FleetTypeDef](./type_defs.md#fleettypedef)
- [ImageBuilderTypeDef](./type_defs.md#imagebuildertypedef)
- [SessionTypeDef](./type_defs.md#sessiontypedef)
- [SharedImagePermissionsTypeDef](./type_defs.md#sharedimagepermissionstypedef)
- [UpdateImagePermissionsRequestRequestTypeDef](./type_defs.md#updateimagepermissionsrequestrequesttypedef)
- [UsageReportSubscriptionTypeDef](./type_defs.md#usagereportsubscriptiontypedef)
- [StackTypeDef](./type_defs.md#stacktypedef)
- [StorageConnectorUnionTypeDef](./type_defs.md#storageconnectoruniontypedef)
- [UpdateStackRequestRequestTypeDef](./type_defs.md#updatestackrequestrequesttypedef)
- [CreateAppBlockBuilderResultTypeDef](./type_defs.md#createappblockbuilderresulttypedef)
- [DescribeAppBlockBuildersResultTypeDef](./type_defs.md#describeappblockbuildersresulttypedef)
- [StartAppBlockBuilderResultTypeDef](./type_defs.md#startappblockbuilderresulttypedef)
- [StopAppBlockBuilderResultTypeDef](./type_defs.md#stopappblockbuilderresulttypedef)
- [UpdateAppBlockBuilderResultTypeDef](./type_defs.md#updateappblockbuilderresulttypedef)
- [CreateApplicationResultTypeDef](./type_defs.md#createapplicationresulttypedef)
- [DescribeApplicationsResultTypeDef](./type_defs.md#describeapplicationsresulttypedef)
- [ImageTypeDef](./type_defs.md#imagetypedef)
- [UpdateApplicationResultTypeDef](./type_defs.md#updateapplicationresulttypedef)
- [AppBlockTypeDef](./type_defs.md#appblocktypedef)
- [CreateAppBlockRequestRequestTypeDef](./type_defs.md#createappblockrequestrequesttypedef)
- [BatchAssociateUserStackResultTypeDef](./type_defs.md#batchassociateuserstackresulttypedef)
- [BatchDisassociateUserStackResultTypeDef](./type_defs.md#batchdisassociateuserstackresulttypedef)
- [CreateDirectoryConfigResultTypeDef](./type_defs.md#createdirectoryconfigresulttypedef)
- [DescribeDirectoryConfigsResultTypeDef](./type_defs.md#describedirectoryconfigsresulttypedef)
- [UpdateDirectoryConfigResultTypeDef](./type_defs.md#updatedirectoryconfigresulttypedef)
- [CreateEntitlementResultTypeDef](./type_defs.md#createentitlementresulttypedef)
- [DescribeEntitlementsResultTypeDef](./type_defs.md#describeentitlementsresulttypedef)
- [UpdateEntitlementResultTypeDef](./type_defs.md#updateentitlementresulttypedef)
- [CreateThemeForStackResultTypeDef](./type_defs.md#createthemeforstackresulttypedef)
- [DescribeThemeForStackResultTypeDef](./type_defs.md#describethemeforstackresulttypedef)
- [UpdateThemeForStackResultTypeDef](./type_defs.md#updatethemeforstackresulttypedef)
- [CreateFleetResultTypeDef](./type_defs.md#createfleetresulttypedef)
- [DescribeFleetsResultTypeDef](./type_defs.md#describefleetsresulttypedef)
- [UpdateFleetResultTypeDef](./type_defs.md#updatefleetresulttypedef)
- [CreateImageBuilderResultTypeDef](./type_defs.md#createimagebuilderresulttypedef)
- [DeleteImageBuilderResultTypeDef](./type_defs.md#deleteimagebuilderresulttypedef)
- [DescribeImageBuildersResultTypeDef](./type_defs.md#describeimagebuildersresulttypedef)
- [StartImageBuilderResultTypeDef](./type_defs.md#startimagebuilderresulttypedef)
- [StopImageBuilderResultTypeDef](./type_defs.md#stopimagebuilderresulttypedef)
- [DescribeSessionsResultTypeDef](./type_defs.md#describesessionsresulttypedef)
- [DescribeImagePermissionsResultTypeDef](./type_defs.md#describeimagepermissionsresulttypedef)
- [DescribeUsageReportSubscriptionsResultTypeDef](./type_defs.md#describeusagereportsubscriptionsresulttypedef)
- [CreateStackResultTypeDef](./type_defs.md#createstackresulttypedef)
- [DescribeStacksResultTypeDef](./type_defs.md#describestacksresulttypedef)
- [UpdateStackResultTypeDef](./type_defs.md#updatestackresulttypedef)
- [CreateStackRequestRequestTypeDef](./type_defs.md#createstackrequestrequesttypedef)
- [CreateUpdatedImageResultTypeDef](./type_defs.md#createupdatedimageresulttypedef)
- [DeleteImageResultTypeDef](./type_defs.md#deleteimageresulttypedef)
- [DescribeImagesResultTypeDef](./type_defs.md#describeimagesresulttypedef)
- [CreateAppBlockResultTypeDef](./type_defs.md#createappblockresulttypedef)
- [DescribeAppBlocksResultTypeDef](./type_defs.md#describeappblocksresulttypedef)

