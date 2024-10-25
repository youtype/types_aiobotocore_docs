# CodeArtifact module

> [Index](../README.md) > CodeArtifact


!!! note ""

    Auto-generated documentation for [CodeArtifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
    type annotations stubs module [types-aiobotocore-codeartifact](https://pypi.org/project/types-aiobotocore-codeartifact/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `CodeArtifact` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[codeartifact]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[codeartifact]'


# standalone installation
python -m pip install types-aiobotocore-codeartifact
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-codeartifact
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CodeArtifactClient

Type annotations and code completion for  `#!python session.create_client("codeartifact")` as [CodeArtifactClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client)

```python
# CodeArtifactClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.client import CodeArtifactClient


session = get_session()
async with session.create_client("codeartifact") as client:
    client: CodeArtifactClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("codeartifact").get_paginator("...")`.

```python
# ListAllowedRepositoriesForGroupPaginator usage example

from types_aiobotocore_codeartifact.paginator import ListAllowedRepositoriesForGroupPaginator

def get_list_allowed_repositories_for_group_paginator() -> ListAllowedRepositoriesForGroupPaginator:
    return client.get_paginator("list_allowed_repositories_for_group"))
```

- [ListAllowedRepositoriesForGroupPaginator](./paginators.md#listallowedrepositoriesforgrouppaginator)
- [ListAssociatedPackagesPaginator](./paginators.md#listassociatedpackagespaginator)
- [ListDomainsPaginator](./paginators.md#listdomainspaginator)
- [ListPackageGroupsPaginator](./paginators.md#listpackagegroupspaginator)
- [ListPackageVersionAssetsPaginator](./paginators.md#listpackageversionassetspaginator)
- [ListPackageVersionsPaginator](./paginators.md#listpackageversionspaginator)
- [ListPackagesPaginator](./paginators.md#listpackagespaginator)
- [ListRepositoriesPaginator](./paginators.md#listrepositoriespaginator)
- [ListRepositoriesInDomainPaginator](./paginators.md#listrepositoriesindomainpaginator)
- [ListSubPackageGroupsPaginator](./paginators.md#listsubpackagegroupspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AllowPublishType usage example

from types_aiobotocore_codeartifact.literals import AllowPublishType

def get_value() -> AllowPublishType:
    return "ALLOW"
```

- [AllowPublishType](./literals.md#allowpublishtype)
- [AllowUpstreamType](./literals.md#allowupstreamtype)
- [DomainStatusType](./literals.md#domainstatustype)
- [EndpointTypeType](./literals.md#endpointtypetype)
- [ExternalConnectionStatusType](./literals.md#externalconnectionstatustype)
- [HashAlgorithmType](./literals.md#hashalgorithmtype)
- [ListAllowedRepositoriesForGroupPaginatorName](./literals.md#listallowedrepositoriesforgrouppaginatorname)
- [ListAssociatedPackagesPaginatorName](./literals.md#listassociatedpackagespaginatorname)
- [ListDomainsPaginatorName](./literals.md#listdomainspaginatorname)
- [ListPackageGroupsPaginatorName](./literals.md#listpackagegroupspaginatorname)
- [ListPackageVersionAssetsPaginatorName](./literals.md#listpackageversionassetspaginatorname)
- [ListPackageVersionsPaginatorName](./literals.md#listpackageversionspaginatorname)
- [ListPackagesPaginatorName](./literals.md#listpackagespaginatorname)
- [ListRepositoriesInDomainPaginatorName](./literals.md#listrepositoriesindomainpaginatorname)
- [ListRepositoriesPaginatorName](./literals.md#listrepositoriespaginatorname)
- [ListSubPackageGroupsPaginatorName](./literals.md#listsubpackagegroupspaginatorname)
- [PackageFormatType](./literals.md#packageformattype)
- [PackageGroupAllowedRepositoryUpdateTypeType](./literals.md#packagegroupallowedrepositoryupdatetypetype)
- [PackageGroupAssociationTypeType](./literals.md#packagegroupassociationtypetype)
- [PackageGroupOriginRestrictionModeType](./literals.md#packagegrouporiginrestrictionmodetype)
- [PackageGroupOriginRestrictionTypeType](./literals.md#packagegrouporiginrestrictiontypetype)
- [PackageVersionErrorCodeType](./literals.md#packageversionerrorcodetype)
- [PackageVersionOriginTypeType](./literals.md#packageversionorigintypetype)
- [PackageVersionSortTypeType](./literals.md#packageversionsorttypetype)
- [PackageVersionStatusType](./literals.md#packageversionstatustype)
- [CodeArtifactServiceName](./literals.md#codeartifactservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AssetSummaryTypeDef](./type_defs.md#assetsummarytypedef)
- [AssociateExternalConnectionRequestRequestTypeDef](./type_defs.md#associateexternalconnectionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AssociatedPackageTypeDef](./type_defs.md#associatedpackagetypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CopyPackageVersionsRequestRequestTypeDef](./type_defs.md#copypackageversionsrequestrequesttypedef)
- [PackageVersionErrorTypeDef](./type_defs.md#packageversionerrortypedef)
- [SuccessfulPackageVersionInfoTypeDef](./type_defs.md#successfulpackageversioninfotypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DomainDescriptionTypeDef](./type_defs.md#domaindescriptiontypedef)
- [UpstreamRepositoryTypeDef](./type_defs.md#upstreamrepositorytypedef)
- [DeleteDomainPermissionsPolicyRequestRequestTypeDef](./type_defs.md#deletedomainpermissionspolicyrequestrequesttypedef)
- [ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef)
- [DeleteDomainRequestRequestTypeDef](./type_defs.md#deletedomainrequestrequesttypedef)
- [DeletePackageGroupRequestRequestTypeDef](./type_defs.md#deletepackagegrouprequestrequesttypedef)
- [DeletePackageRequestRequestTypeDef](./type_defs.md#deletepackagerequestrequesttypedef)
- [DeletePackageVersionsRequestRequestTypeDef](./type_defs.md#deletepackageversionsrequestrequesttypedef)
- [DeleteRepositoryPermissionsPolicyRequestRequestTypeDef](./type_defs.md#deleterepositorypermissionspolicyrequestrequesttypedef)
- [DeleteRepositoryRequestRequestTypeDef](./type_defs.md#deleterepositoryrequestrequesttypedef)
- [DescribeDomainRequestRequestTypeDef](./type_defs.md#describedomainrequestrequesttypedef)
- [DescribePackageGroupRequestRequestTypeDef](./type_defs.md#describepackagegrouprequestrequesttypedef)
- [DescribePackageRequestRequestTypeDef](./type_defs.md#describepackagerequestrequesttypedef)
- [DescribePackageVersionRequestRequestTypeDef](./type_defs.md#describepackageversionrequestrequesttypedef)
- [DescribeRepositoryRequestRequestTypeDef](./type_defs.md#describerepositoryrequestrequesttypedef)
- [DisassociateExternalConnectionRequestRequestTypeDef](./type_defs.md#disassociateexternalconnectionrequestrequesttypedef)
- [DisposePackageVersionsRequestRequestTypeDef](./type_defs.md#disposepackageversionsrequestrequesttypedef)
- [DomainEntryPointTypeDef](./type_defs.md#domainentrypointtypedef)
- [DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef)
- [GetAssociatedPackageGroupRequestRequestTypeDef](./type_defs.md#getassociatedpackagegrouprequestrequesttypedef)
- [GetAuthorizationTokenRequestRequestTypeDef](./type_defs.md#getauthorizationtokenrequestrequesttypedef)
- [GetDomainPermissionsPolicyRequestRequestTypeDef](./type_defs.md#getdomainpermissionspolicyrequestrequesttypedef)
- [GetPackageVersionAssetRequestRequestTypeDef](./type_defs.md#getpackageversionassetrequestrequesttypedef)
- [GetPackageVersionReadmeRequestRequestTypeDef](./type_defs.md#getpackageversionreadmerequestrequesttypedef)
- [GetRepositoryEndpointRequestRequestTypeDef](./type_defs.md#getrepositoryendpointrequestrequesttypedef)
- [GetRepositoryPermissionsPolicyRequestRequestTypeDef](./type_defs.md#getrepositorypermissionspolicyrequestrequesttypedef)
- [LicenseInfoTypeDef](./type_defs.md#licenseinfotypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAllowedRepositoriesForGroupRequestRequestTypeDef](./type_defs.md#listallowedrepositoriesforgrouprequestrequesttypedef)
- [ListAssociatedPackagesRequestRequestTypeDef](./type_defs.md#listassociatedpackagesrequestrequesttypedef)
- [ListDomainsRequestRequestTypeDef](./type_defs.md#listdomainsrequestrequesttypedef)
- [ListPackageGroupsRequestRequestTypeDef](./type_defs.md#listpackagegroupsrequestrequesttypedef)
- [ListPackageVersionAssetsRequestRequestTypeDef](./type_defs.md#listpackageversionassetsrequestrequesttypedef)
- [ListPackageVersionDependenciesRequestRequestTypeDef](./type_defs.md#listpackageversiondependenciesrequestrequesttypedef)
- [PackageDependencyTypeDef](./type_defs.md#packagedependencytypedef)
- [ListPackageVersionsRequestRequestTypeDef](./type_defs.md#listpackageversionsrequestrequesttypedef)
- [ListPackagesRequestRequestTypeDef](./type_defs.md#listpackagesrequestrequesttypedef)
- [ListRepositoriesInDomainRequestRequestTypeDef](./type_defs.md#listrepositoriesindomainrequestrequesttypedef)
- [RepositorySummaryTypeDef](./type_defs.md#repositorysummarytypedef)
- [ListRepositoriesRequestRequestTypeDef](./type_defs.md#listrepositoriesrequestrequesttypedef)
- [ListSubPackageGroupsRequestRequestTypeDef](./type_defs.md#listsubpackagegroupsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [PackageGroupAllowedRepositoryTypeDef](./type_defs.md#packagegroupallowedrepositorytypedef)
- [PackageGroupReferenceTypeDef](./type_defs.md#packagegroupreferencetypedef)
- [PackageOriginRestrictionsTypeDef](./type_defs.md#packageoriginrestrictionstypedef)
- [PutDomainPermissionsPolicyRequestRequestTypeDef](./type_defs.md#putdomainpermissionspolicyrequestrequesttypedef)
- [PutRepositoryPermissionsPolicyRequestRequestTypeDef](./type_defs.md#putrepositorypermissionspolicyrequestrequesttypedef)
- [RepositoryExternalConnectionInfoTypeDef](./type_defs.md#repositoryexternalconnectioninfotypedef)
- [UpstreamRepositoryInfoTypeDef](./type_defs.md#upstreamrepositoryinfotypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdatePackageGroupRequestRequestTypeDef](./type_defs.md#updatepackagegrouprequestrequesttypedef)
- [UpdatePackageVersionsStatusRequestRequestTypeDef](./type_defs.md#updatepackageversionsstatusrequestrequesttypedef)
- [GetAuthorizationTokenResultTypeDef](./type_defs.md#getauthorizationtokenresulttypedef)
- [GetPackageVersionAssetResultTypeDef](./type_defs.md#getpackageversionassetresulttypedef)
- [GetPackageVersionReadmeResultTypeDef](./type_defs.md#getpackageversionreadmeresulttypedef)
- [GetRepositoryEndpointResultTypeDef](./type_defs.md#getrepositoryendpointresulttypedef)
- [ListAllowedRepositoriesForGroupResultTypeDef](./type_defs.md#listallowedrepositoriesforgroupresulttypedef)
- [ListPackageVersionAssetsResultTypeDef](./type_defs.md#listpackageversionassetsresulttypedef)
- [PublishPackageVersionResultTypeDef](./type_defs.md#publishpackageversionresulttypedef)
- [ListAssociatedPackagesResultTypeDef](./type_defs.md#listassociatedpackagesresulttypedef)
- [PublishPackageVersionRequestRequestTypeDef](./type_defs.md#publishpackageversionrequestrequesttypedef)
- [CopyPackageVersionsResultTypeDef](./type_defs.md#copypackageversionsresulttypedef)
- [DeletePackageVersionsResultTypeDef](./type_defs.md#deletepackageversionsresulttypedef)
- [DisposePackageVersionsResultTypeDef](./type_defs.md#disposepackageversionsresulttypedef)
- [UpdatePackageVersionsStatusResultTypeDef](./type_defs.md#updatepackageversionsstatusresulttypedef)
- [CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef)
- [CreatePackageGroupRequestRequestTypeDef](./type_defs.md#createpackagegrouprequestrequesttypedef)
- [ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateDomainResultTypeDef](./type_defs.md#createdomainresulttypedef)
- [DeleteDomainResultTypeDef](./type_defs.md#deletedomainresulttypedef)
- [DescribeDomainResultTypeDef](./type_defs.md#describedomainresulttypedef)
- [CreateRepositoryRequestRequestTypeDef](./type_defs.md#createrepositoryrequestrequesttypedef)
- [UpdateRepositoryRequestRequestTypeDef](./type_defs.md#updaterepositoryrequestrequesttypedef)
- [DeleteDomainPermissionsPolicyResultTypeDef](./type_defs.md#deletedomainpermissionspolicyresulttypedef)
- [DeleteRepositoryPermissionsPolicyResultTypeDef](./type_defs.md#deleterepositorypermissionspolicyresulttypedef)
- [GetDomainPermissionsPolicyResultTypeDef](./type_defs.md#getdomainpermissionspolicyresulttypedef)
- [GetRepositoryPermissionsPolicyResultTypeDef](./type_defs.md#getrepositorypermissionspolicyresulttypedef)
- [PutDomainPermissionsPolicyResultTypeDef](./type_defs.md#putdomainpermissionspolicyresulttypedef)
- [PutRepositoryPermissionsPolicyResultTypeDef](./type_defs.md#putrepositorypermissionspolicyresulttypedef)
- [PackageVersionOriginTypeDef](./type_defs.md#packageversionorigintypedef)
- [ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef)
- [ListAllowedRepositoriesForGroupRequestListAllowedRepositoriesForGroupPaginateTypeDef](./type_defs.md#listallowedrepositoriesforgrouprequestlistallowedrepositoriesforgrouppaginatetypedef)
- [ListAssociatedPackagesRequestListAssociatedPackagesPaginateTypeDef](./type_defs.md#listassociatedpackagesrequestlistassociatedpackagespaginatetypedef)
- [ListDomainsRequestListDomainsPaginateTypeDef](./type_defs.md#listdomainsrequestlistdomainspaginatetypedef)
- [ListPackageGroupsRequestListPackageGroupsPaginateTypeDef](./type_defs.md#listpackagegroupsrequestlistpackagegroupspaginatetypedef)
- [ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef](./type_defs.md#listpackageversionassetsrequestlistpackageversionassetspaginatetypedef)
- [ListPackageVersionsRequestListPackageVersionsPaginateTypeDef](./type_defs.md#listpackageversionsrequestlistpackageversionspaginatetypedef)
- [ListPackagesRequestListPackagesPaginateTypeDef](./type_defs.md#listpackagesrequestlistpackagespaginatetypedef)
- [ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef](./type_defs.md#listrepositoriesindomainrequestlistrepositoriesindomainpaginatetypedef)
- [ListRepositoriesRequestListRepositoriesPaginateTypeDef](./type_defs.md#listrepositoriesrequestlistrepositoriespaginatetypedef)
- [ListSubPackageGroupsRequestListSubPackageGroupsPaginateTypeDef](./type_defs.md#listsubpackagegroupsrequestlistsubpackagegroupspaginatetypedef)
- [ListPackageVersionDependenciesResultTypeDef](./type_defs.md#listpackageversiondependenciesresulttypedef)
- [ListRepositoriesInDomainResultTypeDef](./type_defs.md#listrepositoriesindomainresulttypedef)
- [ListRepositoriesResultTypeDef](./type_defs.md#listrepositoriesresulttypedef)
- [UpdatePackageGroupOriginConfigurationRequestRequestTypeDef](./type_defs.md#updatepackagegrouporiginconfigurationrequestrequesttypedef)
- [PackageGroupOriginRestrictionTypeDef](./type_defs.md#packagegrouporiginrestrictiontypedef)
- [PackageOriginConfigurationTypeDef](./type_defs.md#packageoriginconfigurationtypedef)
- [PutPackageOriginConfigurationRequestRequestTypeDef](./type_defs.md#putpackageoriginconfigurationrequestrequesttypedef)
- [RepositoryDescriptionTypeDef](./type_defs.md#repositorydescriptiontypedef)
- [PackageVersionDescriptionTypeDef](./type_defs.md#packageversiondescriptiontypedef)
- [PackageVersionSummaryTypeDef](./type_defs.md#packageversionsummarytypedef)
- [PackageGroupOriginConfigurationTypeDef](./type_defs.md#packagegrouporiginconfigurationtypedef)
- [PackageDescriptionTypeDef](./type_defs.md#packagedescriptiontypedef)
- [PackageSummaryTypeDef](./type_defs.md#packagesummarytypedef)
- [PutPackageOriginConfigurationResultTypeDef](./type_defs.md#putpackageoriginconfigurationresulttypedef)
- [AssociateExternalConnectionResultTypeDef](./type_defs.md#associateexternalconnectionresulttypedef)
- [CreateRepositoryResultTypeDef](./type_defs.md#createrepositoryresulttypedef)
- [DeleteRepositoryResultTypeDef](./type_defs.md#deleterepositoryresulttypedef)
- [DescribeRepositoryResultTypeDef](./type_defs.md#describerepositoryresulttypedef)
- [DisassociateExternalConnectionResultTypeDef](./type_defs.md#disassociateexternalconnectionresulttypedef)
- [UpdateRepositoryResultTypeDef](./type_defs.md#updaterepositoryresulttypedef)
- [DescribePackageVersionResultTypeDef](./type_defs.md#describepackageversionresulttypedef)
- [ListPackageVersionsResultTypeDef](./type_defs.md#listpackageversionsresulttypedef)
- [PackageGroupDescriptionTypeDef](./type_defs.md#packagegroupdescriptiontypedef)
- [PackageGroupSummaryTypeDef](./type_defs.md#packagegroupsummarytypedef)
- [DescribePackageResultTypeDef](./type_defs.md#describepackageresulttypedef)
- [DeletePackageResultTypeDef](./type_defs.md#deletepackageresulttypedef)
- [ListPackagesResultTypeDef](./type_defs.md#listpackagesresulttypedef)
- [CreatePackageGroupResultTypeDef](./type_defs.md#createpackagegroupresulttypedef)
- [DeletePackageGroupResultTypeDef](./type_defs.md#deletepackagegroupresulttypedef)
- [DescribePackageGroupResultTypeDef](./type_defs.md#describepackagegroupresulttypedef)
- [GetAssociatedPackageGroupResultTypeDef](./type_defs.md#getassociatedpackagegroupresulttypedef)
- [UpdatePackageGroupOriginConfigurationResultTypeDef](./type_defs.md#updatepackagegrouporiginconfigurationresulttypedef)
- [UpdatePackageGroupResultTypeDef](./type_defs.md#updatepackagegroupresulttypedef)
- [ListPackageGroupsResultTypeDef](./type_defs.md#listpackagegroupsresulttypedef)
- [ListSubPackageGroupsResultTypeDef](./type_defs.md#listsubpackagegroupsresulttypedef)

