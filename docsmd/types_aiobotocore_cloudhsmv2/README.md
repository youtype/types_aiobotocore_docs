# CloudHSMV2 module

> [Index](../README.md) > CloudHSMV2


!!! note ""

    Auto-generated documentation for [CloudHSMV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#cloudhsmv2)
    type annotations stubs module [types-aiobotocore-cloudhsmv2](https://pypi.org/project/types-aiobotocore-cloudhsmv2/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudHSMV2` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CloudHSMV2` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cloudhsmv2]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cloudhsmv2]'

# standalone installation
python -m pip install types-aiobotocore-cloudhsmv2
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cloudhsmv2
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudHSMV2Client

Type annotations and code completion for  `#!python session.create_client("cloudhsmv2")` as [CloudHSMV2Client](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client)

```python
# CloudHSMV2Client usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudhsmv2.client import CloudHSMV2Client


session = get_session()
async with session.create_client("cloudhsmv2") as client:
    client: CloudHSMV2Client
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("cloudhsmv2").get_paginator("...")`.

```python
# DescribeBackupsPaginator usage example

from types_aiobotocore_cloudhsmv2.paginator import DescribeBackupsPaginator

def get_describe_backups_paginator() -> DescribeBackupsPaginator:
    return client.get_paginator("describe_backups"))
```

- [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
- [DescribeClustersPaginator](./paginators.md#describeclusterspaginator)
- [ListTagsPaginator](./paginators.md#listtagspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BackupPolicyType usage example

from types_aiobotocore_cloudhsmv2.literals import BackupPolicyType

def get_value() -> BackupPolicyType:
    return "DEFAULT"
```

- [BackupPolicyType](./literals.md#backuppolicytype)
- [BackupRetentionTypeType](./literals.md#backupretentiontypetype)
- [BackupStateType](./literals.md#backupstatetype)
- [ClusterModeType](./literals.md#clustermodetype)
- [ClusterStateType](./literals.md#clusterstatetype)
- [DescribeBackupsPaginatorName](./literals.md#describebackupspaginatorname)
- [DescribeClustersPaginatorName](./literals.md#describeclusterspaginatorname)
- [HsmStateType](./literals.md#hsmstatetype)
- [ListTagsPaginatorName](./literals.md#listtagspaginatorname)
- [NetworkTypeType](./literals.md#networktypetype)
- [CloudHSMV2ServiceName](./literals.md#cloudhsmv2servicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BackupRetentionPolicyTypeDef](./type_defs.md#backupretentionpolicytypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CertificatesTypeDef](./type_defs.md#certificatestypedef)
- [HsmTypeDef](./type_defs.md#hsmtypedef)
- [DestinationBackupTypeDef](./type_defs.md#destinationbackuptypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateHsmRequestTypeDef](./type_defs.md#createhsmrequesttypedef)
- [DeleteBackupRequestTypeDef](./type_defs.md#deletebackuprequesttypedef)
- [DeleteClusterRequestTypeDef](./type_defs.md#deleteclusterrequesttypedef)
- [DeleteHsmRequestTypeDef](./type_defs.md#deletehsmrequesttypedef)
- [DeleteResourcePolicyRequestTypeDef](./type_defs.md#deleteresourcepolicyrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeBackupsRequestTypeDef](./type_defs.md#describebackupsrequesttypedef)
- [DescribeClustersRequestTypeDef](./type_defs.md#describeclustersrequesttypedef)
- [GetResourcePolicyRequestTypeDef](./type_defs.md#getresourcepolicyrequesttypedef)
- [InitializeClusterRequestTypeDef](./type_defs.md#initializeclusterrequesttypedef)
- [ListTagsRequestTypeDef](./type_defs.md#listtagsrequesttypedef)
- [ModifyBackupAttributesRequestTypeDef](./type_defs.md#modifybackupattributesrequesttypedef)
- [PutResourcePolicyRequestTypeDef](./type_defs.md#putresourcepolicyrequesttypedef)
- [RestoreBackupRequestTypeDef](./type_defs.md#restorebackuprequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [ModifyClusterRequestTypeDef](./type_defs.md#modifyclusterrequesttypedef)
- [BackupTypeDef](./type_defs.md#backuptypedef)
- [CopyBackupToRegionRequestTypeDef](./type_defs.md#copybackuptoregionrequesttypedef)
- [CreateClusterRequestTypeDef](./type_defs.md#createclusterrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [ClusterTypeDef](./type_defs.md#clustertypedef)
- [CopyBackupToRegionResponseTypeDef](./type_defs.md#copybackuptoregionresponsetypedef)
- [CreateHsmResponseTypeDef](./type_defs.md#createhsmresponsetypedef)
- [DeleteHsmResponseTypeDef](./type_defs.md#deletehsmresponsetypedef)
- [DeleteResourcePolicyResponseTypeDef](./type_defs.md#deleteresourcepolicyresponsetypedef)
- [GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef)
- [InitializeClusterResponseTypeDef](./type_defs.md#initializeclusterresponsetypedef)
- [ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef)
- [PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef)
- [DescribeBackupsRequestPaginateTypeDef](./type_defs.md#describebackupsrequestpaginatetypedef)
- [DescribeClustersRequestPaginateTypeDef](./type_defs.md#describeclustersrequestpaginatetypedef)
- [ListTagsRequestPaginateTypeDef](./type_defs.md#listtagsrequestpaginatetypedef)
- [DeleteBackupResponseTypeDef](./type_defs.md#deletebackupresponsetypedef)
- [DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef)
- [ModifyBackupAttributesResponseTypeDef](./type_defs.md#modifybackupattributesresponsetypedef)
- [RestoreBackupResponseTypeDef](./type_defs.md#restorebackupresponsetypedef)
- [CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)
- [DeleteClusterResponseTypeDef](./type_defs.md#deleteclusterresponsetypedef)
- [DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef)
- [ModifyClusterResponseTypeDef](./type_defs.md#modifyclusterresponsetypedef)

