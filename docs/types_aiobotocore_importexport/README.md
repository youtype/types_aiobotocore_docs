<a id="type-annotations-for-aiobotocore-importexport-module"></a>

# Type annotations for aiobotocore ImportExport module

> [Index](../README.md) > ImportExport

Auto-generated documentation for
[ImportExport](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
type annotations stubs module
[types-aiobotocore-importexport](https://pypi.org/project/types-aiobotocore-importexport/).

- [Type annotations for aiobotocore ImportExport module](#type-annotations-for-aiobotocore-importexport-module)
  - [How to install](#how-to-install)
    - [VSCode extension](#vscode-extension)
    - [From PyPI with pip](#from-pypi-with-pip)
  - [How to uninstall](#how-to-uninstall)
  - [Usage](#usage)
  - [ImportExportClient](#importexportclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Paginators](#paginators)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="how-to-install"></a>

## How to install

<a id="vscode-extension"></a>

### VSCode extension

Add
[AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `ImportExport`.

<a id="from-pypi-with-pip"></a>

### From PyPI with pip

Install `types-aiobotocore` for `ImportExport` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[importexport]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[importexport]'


# standalone installation
python -m pip install types-aiobotocore-importexport
```

<a id="how-to-uninstall"></a>

## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-importexport
```

<a id="usage"></a>

## Usage

Code samples can be found [here](./usage.md).

<a id="importexportclient"></a>

## ImportExportClient

Type annotations for `session.create_client("importexport")` as
[ImportExportClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_importexport.client import ImportExportClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [cancel_job](./client.md#cancel_job)
- [create_job](./client.md#create_job)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_paginator](./client.md#get_paginator)
- [get_shipping_label](./client.md#get_shipping_label)
- [get_status](./client.md#get_status)
- [list_jobs](./client.md#list_jobs)
- [update_job](./client.md#update_job)

<a id="exceptions"></a>

### Exceptions

ImportExportClient [exceptions](./client.md#exceptions)

- BucketPermissionException
- CanceledJobIdException
- ClientError
- CreateJobQuotaExceededException
- ExpiredJobIdException
- InvalidAccessKeyIdException
- InvalidAddressException
- InvalidCustomsException
- InvalidFileSystemException
- InvalidJobIdException
- InvalidManifestFieldException
- InvalidParameterException
- InvalidVersionException
- MalformedManifestException
- MissingCustomsException
- MissingManifestFieldException
- MissingParameterException
- MultipleRegionsException
- NoSuchBucketException
- UnableToCancelJobIdException
- UnableToUpdateJobIdException

<a id="paginators"></a>

## Paginators

Type annotations for [paginators](./paginators.md) from
`boto3.client("importexport").get_paginator("...")`.

Can be used directly:

```python
from types_aiobotocore_importexport.paginator import ListJobsPaginator, ...
```

- [ListJobsPaginator](./paginators.md#listjobspaginator)

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_importexport.literals import JobTypeType, ...
```

- [JobTypeType](./literals.md#jobtypetype)
- [ListJobsPaginatorName](./literals.md#listjobspaginatorname)
- [ImportExportServiceName](./literals.md#importexportservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from types_aiobotocore_importexport.type_defs import ArtifactTypeDef, ...
```

- [ArtifactTypeDef](./type_defs.md#artifacttypedef)
- [CancelJobInputRequestTypeDef](./type_defs.md#canceljobinputrequesttypedef)
- [CancelJobOutputTypeDef](./type_defs.md#canceljoboutputtypedef)
- [CreateJobInputRequestTypeDef](./type_defs.md#createjobinputrequesttypedef)
- [CreateJobOutputTypeDef](./type_defs.md#createjoboutputtypedef)
- [GetShippingLabelInputRequestTypeDef](./type_defs.md#getshippinglabelinputrequesttypedef)
- [GetShippingLabelOutputTypeDef](./type_defs.md#getshippinglabeloutputtypedef)
- [GetStatusInputRequestTypeDef](./type_defs.md#getstatusinputrequesttypedef)
- [GetStatusOutputTypeDef](./type_defs.md#getstatusoutputtypedef)
- [JobTypeDef](./type_defs.md#jobtypedef)
- [ListJobsInputRequestTypeDef](./type_defs.md#listjobsinputrequesttypedef)
- [ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [UpdateJobInputRequestTypeDef](./type_defs.md#updatejobinputrequesttypedef)
- [UpdateJobOutputTypeDef](./type_defs.md#updatejoboutputtypedef)
