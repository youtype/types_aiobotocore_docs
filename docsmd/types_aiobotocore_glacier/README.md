# Glacier module

> [Index](../README.md) > Glacier


!!! note ""

    Auto-generated documentation for [Glacier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#glacier)
    type annotations stubs module [types-aiobotocore-glacier](https://pypi.org/project/types-aiobotocore-glacier/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Glacier` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Glacier` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[glacier]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[glacier]'

# standalone installation
python -m pip install types-aiobotocore-glacier
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-glacier
```

## Usage

Code samples can be found in [Examples](./usage.md).

## GlacierClient

Type annotations and code completion for  `#!python session.create_client("glacier")` as [GlacierClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client)

```python
# GlacierClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_glacier.client import GlacierClient


session = get_session()
async with session.create_client("glacier") as client:
    client: GlacierClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("glacier").get_paginator("...")`.

```python
# ListJobsPaginator usage example

from types_aiobotocore_glacier.paginator import ListJobsPaginator

def get_list_jobs_paginator() -> ListJobsPaginator:
    return client.get_paginator("list_jobs"))
```

- [ListJobsPaginator](./paginators.md#listjobspaginator)
- [ListMultipartUploadsPaginator](./paginators.md#listmultipartuploadspaginator)
- [ListPartsPaginator](./paginators.md#listpartspaginator)
- [ListVaultsPaginator](./paginators.md#listvaultspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("glacier").get_waiter("...")`.

```python
# VaultExistsWaiter usage example

from types_aiobotocore_glacier.waiter import VaultExistsWaiter

def get_vault_exists_waiter() -> VaultExistsWaiter:
    return Session().client("glacier").get_waiter("vault_exists")
```

- [VaultExistsWaiter](./waiters.md#vaultexistswaiter)
- [VaultNotExistsWaiter](./waiters.md#vaultnotexistswaiter)




## GlacierServiceResource

Type annotations and code completion for `#!python session.resource("glacier")` as
[GlacierServiceResource](./service_resource.md#glacierserviceresource)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/service-resource/index.html)

```python
# GlacierServiceResource usage example

from types_aiobotocore_glacier.service_resource import GlacierServiceResource
```


### Collections

Type annotations and code completion for collections
from `#!python session.resource("glacier").*`.

```python
# ServiceResourceVaultsCollection usage example

from types_aiobotocore_glacier.service_resource import ServiceResourceVaultsCollection

def get_collection() -> ServiceResourceVaultsCollection:
    return resource.vaults
```

- [ServiceResourceVaultsCollection](./service_resource.md#serviceresourcevaultscollection)





### Resources

Type annotations and code completion for additional resources
from `#!python session.resource("glacier").*`.

```python
# Account usage example

from types_aiobotocore_glacier.service_resource import Account

def get_resource() -> Account:
    return resource.Account(...)
```

- [Account](./service_resource.md#account)
- [Archive](./service_resource.md#archive)
- [Job](./service_resource.md#job)
- [MultipartUpload](./service_resource.md#multipartupload)
- [Notification](./service_resource.md#notification)
- [Vault](./service_resource.md#vault)





## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionCodeType usage example

from types_aiobotocore_glacier.literals import ActionCodeType

def get_value() -> ActionCodeType:
    return "ArchiveRetrieval"
```

- [ActionCodeType](./literals.md#actioncodetype)
- [CannedACLType](./literals.md#cannedacltype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [ExpressionTypeType](./literals.md#expressiontypetype)
- [FileHeaderInfoType](./literals.md#fileheaderinfotype)
- [ListJobsPaginatorName](./literals.md#listjobspaginatorname)
- [ListMultipartUploadsPaginatorName](./literals.md#listmultipartuploadspaginatorname)
- [ListPartsPaginatorName](./literals.md#listpartspaginatorname)
- [ListVaultsPaginatorName](./literals.md#listvaultspaginatorname)
- [PermissionType](./literals.md#permissiontype)
- [QuoteFieldsType](./literals.md#quotefieldstype)
- [StatusCodeType](./literals.md#statuscodetype)
- [StorageClassType](./literals.md#storageclasstype)
- [TypeType](./literals.md#typetype)
- [VaultExistsWaiterName](./literals.md#vaultexistswaitername)
- [VaultNotExistsWaiterName](./literals.md#vaultnotexistswaitername)
- [GlacierServiceName](./literals.md#glacierservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AbortMultipartUploadInputRequestTypeDef](./type_defs.md#abortmultipartuploadinputrequesttypedef)
- [AbortVaultLockInputRequestTypeDef](./type_defs.md#abortvaultlockinputrequesttypedef)
- [AddTagsToVaultInputRequestTypeDef](./type_defs.md#addtagstovaultinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CSVInputTypeDef](./type_defs.md#csvinputtypedef)
- [CSVOutputTypeDef](./type_defs.md#csvoutputtypedef)
- [CompleteMultipartUploadInputMultipartUploadCompleteTypeDef](./type_defs.md#completemultipartuploadinputmultipartuploadcompletetypedef)
- [CompleteMultipartUploadInputRequestTypeDef](./type_defs.md#completemultipartuploadinputrequesttypedef)
- [CompleteVaultLockInputRequestTypeDef](./type_defs.md#completevaultlockinputrequesttypedef)
- [CreateVaultInputAccountCreateVaultTypeDef](./type_defs.md#createvaultinputaccountcreatevaulttypedef)
- [CreateVaultInputRequestTypeDef](./type_defs.md#createvaultinputrequesttypedef)
- [CreateVaultInputServiceResourceCreateVaultTypeDef](./type_defs.md#createvaultinputserviceresourcecreatevaulttypedef)
- [DataRetrievalRuleTypeDef](./type_defs.md#dataretrievalruletypedef)
- [DeleteArchiveInputRequestTypeDef](./type_defs.md#deletearchiveinputrequesttypedef)
- [DeleteVaultAccessPolicyInputRequestTypeDef](./type_defs.md#deletevaultaccesspolicyinputrequesttypedef)
- [DeleteVaultInputRequestTypeDef](./type_defs.md#deletevaultinputrequesttypedef)
- [DeleteVaultNotificationsInputRequestTypeDef](./type_defs.md#deletevaultnotificationsinputrequesttypedef)
- [DescribeJobInputRequestTypeDef](./type_defs.md#describejobinputrequesttypedef)
- [DescribeVaultInputRequestTypeDef](./type_defs.md#describevaultinputrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeVaultOutputTypeDef](./type_defs.md#describevaultoutputtypedef)
- [EncryptionTypeDef](./type_defs.md#encryptiontypedef)
- [GetDataRetrievalPolicyInputRequestTypeDef](./type_defs.md#getdataretrievalpolicyinputrequesttypedef)
- [GetJobOutputInputJobGetOutputTypeDef](./type_defs.md#getjoboutputinputjobgetoutputtypedef)
- [GetJobOutputInputRequestTypeDef](./type_defs.md#getjoboutputinputrequesttypedef)
- [GetVaultAccessPolicyInputRequestTypeDef](./type_defs.md#getvaultaccesspolicyinputrequesttypedef)
- [VaultAccessPolicyTypeDef](./type_defs.md#vaultaccesspolicytypedef)
- [GetVaultLockInputRequestTypeDef](./type_defs.md#getvaultlockinputrequesttypedef)
- [GetVaultNotificationsInputRequestTypeDef](./type_defs.md#getvaultnotificationsinputrequesttypedef)
- [VaultNotificationConfigOutputTypeDef](./type_defs.md#vaultnotificationconfigoutputtypedef)
- [InventoryRetrievalJobDescriptionTypeDef](./type_defs.md#inventoryretrievaljobdescriptiontypedef)
- [GranteeTypeDef](./type_defs.md#granteetypedef)
- [InitiateMultipartUploadInputRequestTypeDef](./type_defs.md#initiatemultipartuploadinputrequesttypedef)
- [InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef](./type_defs.md#initiatemultipartuploadinputvaultinitiatemultipartuploadtypedef)
- [VaultLockPolicyTypeDef](./type_defs.md#vaultlockpolicytypedef)
- [InventoryRetrievalJobInputTypeDef](./type_defs.md#inventoryretrievaljobinputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListJobsInputRequestTypeDef](./type_defs.md#listjobsinputrequesttypedef)
- [ListMultipartUploadsInputRequestTypeDef](./type_defs.md#listmultipartuploadsinputrequesttypedef)
- [UploadListElementTypeDef](./type_defs.md#uploadlistelementtypedef)
- [ListPartsInputMultipartUploadPartsTypeDef](./type_defs.md#listpartsinputmultipartuploadpartstypedef)
- [ListPartsInputRequestTypeDef](./type_defs.md#listpartsinputrequesttypedef)
- [PartListElementTypeDef](./type_defs.md#partlistelementtypedef)
- [ListProvisionedCapacityInputRequestTypeDef](./type_defs.md#listprovisionedcapacityinputrequesttypedef)
- [ProvisionedCapacityDescriptionTypeDef](./type_defs.md#provisionedcapacitydescriptiontypedef)
- [ListTagsForVaultInputRequestTypeDef](./type_defs.md#listtagsforvaultinputrequesttypedef)
- [ListVaultsInputRequestTypeDef](./type_defs.md#listvaultsinputrequesttypedef)
- [PurchaseProvisionedCapacityInputRequestTypeDef](./type_defs.md#purchaseprovisionedcapacityinputrequesttypedef)
- [RemoveTagsFromVaultInputRequestTypeDef](./type_defs.md#removetagsfromvaultinputrequesttypedef)
- [VaultNotificationConfigTypeDef](./type_defs.md#vaultnotificationconfigtypedef)
- [ArchiveCreationOutputTypeDef](./type_defs.md#archivecreationoutputtypedef)
- [CreateVaultOutputTypeDef](./type_defs.md#createvaultoutputtypedef)
- [DescribeVaultResponseTypeDef](./type_defs.md#describevaultresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetJobOutputOutputTypeDef](./type_defs.md#getjoboutputoutputtypedef)
- [GetVaultLockOutputTypeDef](./type_defs.md#getvaultlockoutputtypedef)
- [InitiateJobOutputTypeDef](./type_defs.md#initiatejoboutputtypedef)
- [InitiateMultipartUploadOutputTypeDef](./type_defs.md#initiatemultipartuploadoutputtypedef)
- [InitiateVaultLockOutputTypeDef](./type_defs.md#initiatevaultlockoutputtypedef)
- [ListTagsForVaultOutputTypeDef](./type_defs.md#listtagsforvaultoutputtypedef)
- [PurchaseProvisionedCapacityOutputTypeDef](./type_defs.md#purchaseprovisionedcapacityoutputtypedef)
- [UploadMultipartPartOutputTypeDef](./type_defs.md#uploadmultipartpartoutputtypedef)
- [UploadArchiveInputRequestTypeDef](./type_defs.md#uploadarchiveinputrequesttypedef)
- [UploadArchiveInputVaultUploadArchiveTypeDef](./type_defs.md#uploadarchiveinputvaultuploadarchivetypedef)
- [UploadMultipartPartInputMultipartUploadUploadPartTypeDef](./type_defs.md#uploadmultipartpartinputmultipartuploaduploadparttypedef)
- [UploadMultipartPartInputRequestTypeDef](./type_defs.md#uploadmultipartpartinputrequesttypedef)
- [InputSerializationTypeDef](./type_defs.md#inputserializationtypedef)
- [OutputSerializationTypeDef](./type_defs.md#outputserializationtypedef)
- [DataRetrievalPolicyOutputTypeDef](./type_defs.md#dataretrievalpolicyoutputtypedef)
- [DataRetrievalPolicyTypeDef](./type_defs.md#dataretrievalpolicytypedef)
- [DescribeVaultInputWaitTypeDef](./type_defs.md#describevaultinputwaittypedef)
- [ListVaultsOutputTypeDef](./type_defs.md#listvaultsoutputtypedef)
- [GetVaultAccessPolicyOutputTypeDef](./type_defs.md#getvaultaccesspolicyoutputtypedef)
- [SetVaultAccessPolicyInputRequestTypeDef](./type_defs.md#setvaultaccesspolicyinputrequesttypedef)
- [GetVaultNotificationsOutputTypeDef](./type_defs.md#getvaultnotificationsoutputtypedef)
- [GrantTypeDef](./type_defs.md#granttypedef)
- [InitiateVaultLockInputRequestTypeDef](./type_defs.md#initiatevaultlockinputrequesttypedef)
- [ListJobsInputPaginateTypeDef](./type_defs.md#listjobsinputpaginatetypedef)
- [ListMultipartUploadsInputPaginateTypeDef](./type_defs.md#listmultipartuploadsinputpaginatetypedef)
- [ListPartsInputPaginateTypeDef](./type_defs.md#listpartsinputpaginatetypedef)
- [ListVaultsInputPaginateTypeDef](./type_defs.md#listvaultsinputpaginatetypedef)
- [ListMultipartUploadsOutputTypeDef](./type_defs.md#listmultipartuploadsoutputtypedef)
- [ListPartsOutputTypeDef](./type_defs.md#listpartsoutputtypedef)
- [ListProvisionedCapacityOutputTypeDef](./type_defs.md#listprovisionedcapacityoutputtypedef)
- [SetVaultNotificationsInputNotificationSetTypeDef](./type_defs.md#setvaultnotificationsinputnotificationsettypedef)
- [SetVaultNotificationsInputRequestTypeDef](./type_defs.md#setvaultnotificationsinputrequesttypedef)
- [SelectParametersTypeDef](./type_defs.md#selectparameterstypedef)
- [GetDataRetrievalPolicyOutputTypeDef](./type_defs.md#getdataretrievalpolicyoutputtypedef)
- [SetDataRetrievalPolicyInputRequestTypeDef](./type_defs.md#setdataretrievalpolicyinputrequesttypedef)
- [S3LocationOutputTypeDef](./type_defs.md#s3locationoutputtypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [OutputLocationOutputTypeDef](./type_defs.md#outputlocationoutputtypedef)
- [S3LocationUnionTypeDef](./type_defs.md#s3locationuniontypedef)
- [GlacierJobDescriptionResponseTypeDef](./type_defs.md#glacierjobdescriptionresponsetypedef)
- [GlacierJobDescriptionTypeDef](./type_defs.md#glacierjobdescriptiontypedef)
- [OutputLocationTypeDef](./type_defs.md#outputlocationtypedef)
- [ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef)
- [OutputLocationUnionTypeDef](./type_defs.md#outputlocationuniontypedef)
- [JobParametersTypeDef](./type_defs.md#jobparameterstypedef)
- [InitiateJobInputRequestTypeDef](./type_defs.md#initiatejobinputrequesttypedef)

