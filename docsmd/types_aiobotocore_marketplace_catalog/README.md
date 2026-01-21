# MarketplaceCatalog module

> [Index](../README.md) > MarketplaceCatalog


!!! note ""

    Auto-generated documentation for [MarketplaceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#marketplacecatalog)
    type annotations stubs module [types-aiobotocore-marketplace-catalog](https://pypi.org/project/types-aiobotocore-marketplace-catalog/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `MarketplaceCatalog` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `MarketplaceCatalog` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[marketplace-catalog]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[marketplace-catalog]'

# standalone installation
python -m pip install types-aiobotocore-marketplace-catalog
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-marketplace-catalog
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MarketplaceCatalogClient

Type annotations and code completion for  `#!python session.create_client("marketplace-catalog")` as [MarketplaceCatalogClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# MarketplaceCatalogClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_catalog.client import MarketplaceCatalogClient


session = get_session()
async with session.create_client("marketplace-catalog") as client:
    client: MarketplaceCatalogClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("marketplace-catalog").get_paginator("...")`.

```python
# ListChangeSetsPaginator usage example

from types_aiobotocore_marketplace_catalog.paginator import ListChangeSetsPaginator

def get_list_change_sets_paginator() -> ListChangeSetsPaginator:
    return client.get_paginator("list_change_sets"))
```

- [ListChangeSetsPaginator](./paginators.md#listchangesetspaginator)
- [ListEntitiesPaginator](./paginators.md#listentitiespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AmiProductSortByType usage example

from types_aiobotocore_marketplace_catalog.literals import AmiProductSortByType

def get_value() -> AmiProductSortByType:
    return "EntityId"
```

- [AmiProductSortByType](./literals.md#amiproductsortbytype)
- [AmiProductVisibilityStringType](./literals.md#amiproductvisibilitystringtype)
- [ChangeStatusType](./literals.md#changestatustype)
- [ContainerProductSortByType](./literals.md#containerproductsortbytype)
- [ContainerProductVisibilityStringType](./literals.md#containerproductvisibilitystringtype)
- [DataProductSortByType](./literals.md#dataproductsortbytype)
- [DataProductVisibilityStringType](./literals.md#dataproductvisibilitystringtype)
- [FailureCodeType](./literals.md#failurecodetype)
- [IntentType](./literals.md#intenttype)
- [ListChangeSetsPaginatorName](./literals.md#listchangesetspaginatorname)
- [ListEntitiesPaginatorName](./literals.md#listentitiespaginatorname)
- [MachineLearningProductSortByType](./literals.md#machinelearningproductsortbytype)
- [MachineLearningProductVisibilityStringType](./literals.md#machinelearningproductvisibilitystringtype)
- [OfferSetSortByType](./literals.md#offersetsortbytype)
- [OfferSetStateStringType](./literals.md#offersetstatestringtype)
- [OfferSortByType](./literals.md#offersortbytype)
- [OfferStateStringType](./literals.md#offerstatestringtype)
- [OfferTargetingStringType](./literals.md#offertargetingstringtype)
- [OwnershipTypeType](./literals.md#ownershiptypetype)
- [ResaleAuthorizationSortByType](./literals.md#resaleauthorizationsortbytype)
- [ResaleAuthorizationStatusStringType](./literals.md#resaleauthorizationstatusstringtype)
- [SaaSProductSortByType](./literals.md#saasproductsortbytype)
- [SaaSProductVisibilityStringType](./literals.md#saasproductvisibilitystringtype)
- [SortOrderType](./literals.md#sortordertype)
- [MarketplaceCatalogServiceName](./literals.md#marketplacecatalogservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AmiProductEntityIdFilterTypeDef](./type_defs.md#amiproductentityidfiltertypedef)
- [AmiProductTitleFilterTypeDef](./type_defs.md#amiproducttitlefiltertypedef)
- [AmiProductVisibilityFilterTypeDef](./type_defs.md#amiproductvisibilityfiltertypedef)
- [AmiProductLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#amiproductlastmodifieddatefilterdaterangetypedef)
- [AmiProductSortTypeDef](./type_defs.md#amiproductsorttypedef)
- [AmiProductSummaryTypeDef](./type_defs.md#amiproductsummarytypedef)
- [EntityRequestTypeDef](./type_defs.md#entityrequesttypedef)
- [BatchDescribeErrorDetailTypeDef](./type_defs.md#batchdescribeerrordetailtypedef)
- [EntityDetailTypeDef](./type_defs.md#entitydetailtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CancelChangeSetRequestTypeDef](./type_defs.md#cancelchangesetrequesttypedef)
- [ChangeSetSummaryListItemTypeDef](./type_defs.md#changesetsummarylistitemtypedef)
- [EntityTypeDef](./type_defs.md#entitytypedef)
- [ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ContainerProductEntityIdFilterTypeDef](./type_defs.md#containerproductentityidfiltertypedef)
- [ContainerProductTitleFilterTypeDef](./type_defs.md#containerproducttitlefiltertypedef)
- [ContainerProductVisibilityFilterTypeDef](./type_defs.md#containerproductvisibilityfiltertypedef)
- [ContainerProductLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#containerproductlastmodifieddatefilterdaterangetypedef)
- [ContainerProductSortTypeDef](./type_defs.md#containerproductsorttypedef)
- [ContainerProductSummaryTypeDef](./type_defs.md#containerproductsummarytypedef)
- [DataProductEntityIdFilterTypeDef](./type_defs.md#dataproductentityidfiltertypedef)
- [DataProductTitleFilterTypeDef](./type_defs.md#dataproducttitlefiltertypedef)
- [DataProductVisibilityFilterTypeDef](./type_defs.md#dataproductvisibilityfiltertypedef)
- [DataProductLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#dataproductlastmodifieddatefilterdaterangetypedef)
- [DataProductSortTypeDef](./type_defs.md#dataproductsorttypedef)
- [DataProductSummaryTypeDef](./type_defs.md#dataproductsummarytypedef)
- [DeleteResourcePolicyRequestTypeDef](./type_defs.md#deleteresourcepolicyrequesttypedef)
- [DescribeChangeSetRequestTypeDef](./type_defs.md#describechangesetrequesttypedef)
- [DescribeEntityRequestTypeDef](./type_defs.md#describeentityrequesttypedef)
- [MachineLearningProductSummaryTypeDef](./type_defs.md#machinelearningproductsummarytypedef)
- [OfferSetSummaryTypeDef](./type_defs.md#offersetsummarytypedef)
- [OfferSummaryTypeDef](./type_defs.md#offersummarytypedef)
- [ResaleAuthorizationSummaryTypeDef](./type_defs.md#resaleauthorizationsummarytypedef)
- [SaaSProductSummaryTypeDef](./type_defs.md#saasproductsummarytypedef)
- [MachineLearningProductSortTypeDef](./type_defs.md#machinelearningproductsorttypedef)
- [OfferSetSortTypeDef](./type_defs.md#offersetsorttypedef)
- [OfferSortTypeDef](./type_defs.md#offersorttypedef)
- [ResaleAuthorizationSortTypeDef](./type_defs.md#resaleauthorizationsorttypedef)
- [SaaSProductSortTypeDef](./type_defs.md#saasproductsorttypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetResourcePolicyRequestTypeDef](./type_defs.md#getresourcepolicyrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [SortTypeDef](./type_defs.md#sorttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [MachineLearningProductEntityIdFilterTypeDef](./type_defs.md#machinelearningproductentityidfiltertypedef)
- [MachineLearningProductTitleFilterTypeDef](./type_defs.md#machinelearningproducttitlefiltertypedef)
- [MachineLearningProductVisibilityFilterTypeDef](./type_defs.md#machinelearningproductvisibilityfiltertypedef)
- [MachineLearningProductLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#machinelearningproductlastmodifieddatefilterdaterangetypedef)
- [OfferAvailabilityEndDateFilterDateRangeTypeDef](./type_defs.md#offeravailabilityenddatefilterdaterangetypedef)
- [OfferBuyerAccountsFilterTypeDef](./type_defs.md#offerbuyeraccountsfiltertypedef)
- [OfferEntityIdFilterTypeDef](./type_defs.md#offerentityidfiltertypedef)
- [OfferNameFilterTypeDef](./type_defs.md#offernamefiltertypedef)
- [OfferProductIdFilterTypeDef](./type_defs.md#offerproductidfiltertypedef)
- [OfferResaleAuthorizationIdFilterTypeDef](./type_defs.md#offerresaleauthorizationidfiltertypedef)
- [OfferSetIdFilterTypeDef](./type_defs.md#offersetidfiltertypedef)
- [OfferStateFilterTypeDef](./type_defs.md#offerstatefiltertypedef)
- [OfferTargetingFilterTypeDef](./type_defs.md#offertargetingfiltertypedef)
- [OfferLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#offerlastmodifieddatefilterdaterangetypedef)
- [OfferReleaseDateFilterDateRangeTypeDef](./type_defs.md#offerreleasedatefilterdaterangetypedef)
- [OfferSetAssociatedOfferIdsFilterTypeDef](./type_defs.md#offersetassociatedofferidsfiltertypedef)
- [OfferSetEntityIdFilterTypeDef](./type_defs.md#offersetentityidfiltertypedef)
- [OfferSetNameFilterTypeDef](./type_defs.md#offersetnamefiltertypedef)
- [OfferSetSolutionIdFilterTypeDef](./type_defs.md#offersetsolutionidfiltertypedef)
- [OfferSetStateFilterTypeDef](./type_defs.md#offersetstatefiltertypedef)
- [OfferSetLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#offersetlastmodifieddatefilterdaterangetypedef)
- [OfferSetReleaseDateFilterDateRangeTypeDef](./type_defs.md#offersetreleasedatefilterdaterangetypedef)
- [PutResourcePolicyRequestTypeDef](./type_defs.md#putresourcepolicyrequesttypedef)
- [ResaleAuthorizationAvailabilityEndDateFilterDateRangeTypeDef](./type_defs.md#resaleauthorizationavailabilityenddatefilterdaterangetypedef)
- [ResaleAuthorizationCreatedDateFilterDateRangeTypeDef](./type_defs.md#resaleauthorizationcreateddatefilterdaterangetypedef)
- [ResaleAuthorizationEntityIdFilterTypeDef](./type_defs.md#resaleauthorizationentityidfiltertypedef)
- [ResaleAuthorizationManufacturerAccountIdFilterTypeDef](./type_defs.md#resaleauthorizationmanufactureraccountidfiltertypedef)
- [ResaleAuthorizationManufacturerLegalNameFilterTypeDef](./type_defs.md#resaleauthorizationmanufacturerlegalnamefiltertypedef)
- [ResaleAuthorizationNameFilterTypeDef](./type_defs.md#resaleauthorizationnamefiltertypedef)
- [ResaleAuthorizationOfferExtendedStatusFilterTypeDef](./type_defs.md#resaleauthorizationofferextendedstatusfiltertypedef)
- [ResaleAuthorizationProductIdFilterTypeDef](./type_defs.md#resaleauthorizationproductidfiltertypedef)
- [ResaleAuthorizationProductNameFilterTypeDef](./type_defs.md#resaleauthorizationproductnamefiltertypedef)
- [ResaleAuthorizationResellerAccountIDFilterTypeDef](./type_defs.md#resaleauthorizationreselleraccountidfiltertypedef)
- [ResaleAuthorizationResellerLegalNameFilterTypeDef](./type_defs.md#resaleauthorizationresellerlegalnamefiltertypedef)
- [ResaleAuthorizationStatusFilterTypeDef](./type_defs.md#resaleauthorizationstatusfiltertypedef)
- [ResaleAuthorizationLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#resaleauthorizationlastmodifieddatefilterdaterangetypedef)
- [SaaSProductEntityIdFilterTypeDef](./type_defs.md#saasproductentityidfiltertypedef)
- [SaaSProductTitleFilterTypeDef](./type_defs.md#saasproducttitlefiltertypedef)
- [SaaSProductVisibilityFilterTypeDef](./type_defs.md#saasproductvisibilityfiltertypedef)
- [SaaSProductLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#saasproductlastmodifieddatefilterdaterangetypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [AmiProductLastModifiedDateFilterTypeDef](./type_defs.md#amiproductlastmodifieddatefiltertypedef)
- [BatchDescribeEntitiesRequestTypeDef](./type_defs.md#batchdescribeentitiesrequesttypedef)
- [BatchDescribeEntitiesResponseTypeDef](./type_defs.md#batchdescribeentitiesresponsetypedef)
- [CancelChangeSetResponseTypeDef](./type_defs.md#cancelchangesetresponsetypedef)
- [DescribeEntityResponseTypeDef](./type_defs.md#describeentityresponsetypedef)
- [GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef)
- [StartChangeSetResponseTypeDef](./type_defs.md#startchangesetresponsetypedef)
- [ListChangeSetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef)
- [ChangeSummaryTypeDef](./type_defs.md#changesummarytypedef)
- [ChangeTypeDef](./type_defs.md#changetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [ContainerProductLastModifiedDateFilterTypeDef](./type_defs.md#containerproductlastmodifieddatefiltertypedef)
- [DataProductLastModifiedDateFilterTypeDef](./type_defs.md#dataproductlastmodifieddatefiltertypedef)
- [EntitySummaryTypeDef](./type_defs.md#entitysummarytypedef)
- [EntityTypeSortTypeDef](./type_defs.md#entitytypesorttypedef)
- [ListChangeSetsRequestPaginateTypeDef](./type_defs.md#listchangesetsrequestpaginatetypedef)
- [ListChangeSetsRequestTypeDef](./type_defs.md#listchangesetsrequesttypedef)
- [MachineLearningProductLastModifiedDateFilterTypeDef](./type_defs.md#machinelearningproductlastmodifieddatefiltertypedef)
- [OfferAvailabilityEndDateFilterTypeDef](./type_defs.md#offeravailabilityenddatefiltertypedef)
- [OfferLastModifiedDateFilterTypeDef](./type_defs.md#offerlastmodifieddatefiltertypedef)
- [OfferReleaseDateFilterTypeDef](./type_defs.md#offerreleasedatefiltertypedef)
- [OfferSetLastModifiedDateFilterTypeDef](./type_defs.md#offersetlastmodifieddatefiltertypedef)
- [OfferSetReleaseDateFilterTypeDef](./type_defs.md#offersetreleasedatefiltertypedef)
- [ResaleAuthorizationAvailabilityEndDateFilterTypeDef](./type_defs.md#resaleauthorizationavailabilityenddatefiltertypedef)
- [ResaleAuthorizationCreatedDateFilterTypeDef](./type_defs.md#resaleauthorizationcreateddatefiltertypedef)
- [ResaleAuthorizationLastModifiedDateFilterTypeDef](./type_defs.md#resaleauthorizationlastmodifieddatefiltertypedef)
- [SaaSProductLastModifiedDateFilterTypeDef](./type_defs.md#saasproductlastmodifieddatefiltertypedef)
- [AmiProductFiltersTypeDef](./type_defs.md#amiproductfilterstypedef)
- [DescribeChangeSetResponseTypeDef](./type_defs.md#describechangesetresponsetypedef)
- [StartChangeSetRequestTypeDef](./type_defs.md#startchangesetrequesttypedef)
- [ContainerProductFiltersTypeDef](./type_defs.md#containerproductfilterstypedef)
- [DataProductFiltersTypeDef](./type_defs.md#dataproductfilterstypedef)
- [ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef)
- [MachineLearningProductFiltersTypeDef](./type_defs.md#machinelearningproductfilterstypedef)
- [OfferFiltersTypeDef](./type_defs.md#offerfilterstypedef)
- [OfferSetFiltersTypeDef](./type_defs.md#offersetfilterstypedef)
- [ResaleAuthorizationFiltersTypeDef](./type_defs.md#resaleauthorizationfilterstypedef)
- [SaaSProductFiltersTypeDef](./type_defs.md#saasproductfilterstypedef)
- [EntityTypeFiltersTypeDef](./type_defs.md#entitytypefilterstypedef)
- [ListEntitiesRequestPaginateTypeDef](./type_defs.md#listentitiesrequestpaginatetypedef)
- [ListEntitiesRequestTypeDef](./type_defs.md#listentitiesrequesttypedef)

