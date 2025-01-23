# SecretsManager module

> [Index](../README.md) > SecretsManager


!!! note ""

    Auto-generated documentation for [SecretsManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#secretsmanager)
    type annotations stubs module [types-aiobotocore-secretsmanager](https://pypi.org/project/types-aiobotocore-secretsmanager/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SecretsManager` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SecretsManager` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[secretsmanager]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[secretsmanager]'

# standalone installation
python -m pip install types-aiobotocore-secretsmanager
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-secretsmanager
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SecretsManagerClient

Type annotations and code completion for  `#!python session.create_client("secretsmanager")` as [SecretsManagerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client)

```python
# SecretsManagerClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_secretsmanager.client import SecretsManagerClient


session = get_session()
async with session.create_client("secretsmanager") as client:
    client: SecretsManagerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("secretsmanager").get_paginator("...")`.

```python
# ListSecretsPaginator usage example

from types_aiobotocore_secretsmanager.paginator import ListSecretsPaginator

def get_list_secrets_paginator() -> ListSecretsPaginator:
    return client.get_paginator("list_secrets"))
```

- [ListSecretsPaginator](./paginators.md#listsecretspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# FilterNameStringTypeType usage example

from types_aiobotocore_secretsmanager.literals import FilterNameStringTypeType

def get_value() -> FilterNameStringTypeType:
    return "all"
```

- [FilterNameStringTypeType](./literals.md#filternamestringtypetype)
- [ListSecretsPaginatorName](./literals.md#listsecretspaginatorname)
- [SortOrderTypeType](./literals.md#sortordertypetype)
- [StatusTypeType](./literals.md#statustypetype)
- [SecretsManagerServiceName](./literals.md#secretsmanagerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [APIErrorTypeTypeDef](./type_defs.md#apierrortypetypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SecretValueEntryTypeDef](./type_defs.md#secretvalueentrytypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CancelRotateSecretRequestRequestTypeDef](./type_defs.md#cancelrotatesecretrequestrequesttypedef)
- [ReplicaRegionTypeTypeDef](./type_defs.md#replicaregiontypetypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ReplicationStatusTypeTypeDef](./type_defs.md#replicationstatustypetypedef)
- [DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef)
- [DeleteSecretRequestRequestTypeDef](./type_defs.md#deletesecretrequestrequesttypedef)
- [DescribeSecretRequestRequestTypeDef](./type_defs.md#describesecretrequestrequesttypedef)
- [RotationRulesTypeTypeDef](./type_defs.md#rotationrulestypetypedef)
- [GetRandomPasswordRequestRequestTypeDef](./type_defs.md#getrandompasswordrequestrequesttypedef)
- [GetResourcePolicyRequestRequestTypeDef](./type_defs.md#getresourcepolicyrequestrequesttypedef)
- [GetSecretValueRequestRequestTypeDef](./type_defs.md#getsecretvaluerequestrequesttypedef)
- [ListSecretVersionIdsRequestRequestTypeDef](./type_defs.md#listsecretversionidsrequestrequesttypedef)
- [SecretVersionsListEntryTypeDef](./type_defs.md#secretversionslistentrytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef)
- [RemoveRegionsFromReplicationRequestRequestTypeDef](./type_defs.md#removeregionsfromreplicationrequestrequesttypedef)
- [RestoreSecretRequestRequestTypeDef](./type_defs.md#restoresecretrequestrequesttypedef)
- [StopReplicationToReplicaRequestRequestTypeDef](./type_defs.md#stopreplicationtoreplicarequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateSecretVersionStageRequestRequestTypeDef](./type_defs.md#updatesecretversionstagerequestrequesttypedef)
- [ValidateResourcePolicyRequestRequestTypeDef](./type_defs.md#validateresourcepolicyrequestrequesttypedef)
- [ValidationErrorsEntryTypeDef](./type_defs.md#validationerrorsentrytypedef)
- [BatchGetSecretValueRequestRequestTypeDef](./type_defs.md#batchgetsecretvaluerequestrequesttypedef)
- [ListSecretsRequestRequestTypeDef](./type_defs.md#listsecretsrequestrequesttypedef)
- [CancelRotateSecretResponseTypeDef](./type_defs.md#cancelrotatesecretresponsetypedef)
- [DeleteResourcePolicyResponseTypeDef](./type_defs.md#deleteresourcepolicyresponsetypedef)
- [DeleteSecretResponseTypeDef](./type_defs.md#deletesecretresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetRandomPasswordResponseTypeDef](./type_defs.md#getrandompasswordresponsetypedef)
- [GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef)
- [GetSecretValueResponseTypeDef](./type_defs.md#getsecretvalueresponsetypedef)
- [PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef)
- [PutSecretValueResponseTypeDef](./type_defs.md#putsecretvalueresponsetypedef)
- [RestoreSecretResponseTypeDef](./type_defs.md#restoresecretresponsetypedef)
- [RotateSecretResponseTypeDef](./type_defs.md#rotatesecretresponsetypedef)
- [StopReplicationToReplicaResponseTypeDef](./type_defs.md#stopreplicationtoreplicaresponsetypedef)
- [UpdateSecretResponseTypeDef](./type_defs.md#updatesecretresponsetypedef)
- [UpdateSecretVersionStageResponseTypeDef](./type_defs.md#updatesecretversionstageresponsetypedef)
- [BatchGetSecretValueResponseTypeDef](./type_defs.md#batchgetsecretvalueresponsetypedef)
- [PutSecretValueRequestRequestTypeDef](./type_defs.md#putsecretvaluerequestrequesttypedef)
- [UpdateSecretRequestRequestTypeDef](./type_defs.md#updatesecretrequestrequesttypedef)
- [ReplicateSecretToRegionsRequestRequestTypeDef](./type_defs.md#replicatesecrettoregionsrequestrequesttypedef)
- [CreateSecretRequestRequestTypeDef](./type_defs.md#createsecretrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateSecretResponseTypeDef](./type_defs.md#createsecretresponsetypedef)
- [RemoveRegionsFromReplicationResponseTypeDef](./type_defs.md#removeregionsfromreplicationresponsetypedef)
- [ReplicateSecretToRegionsResponseTypeDef](./type_defs.md#replicatesecrettoregionsresponsetypedef)
- [DescribeSecretResponseTypeDef](./type_defs.md#describesecretresponsetypedef)
- [RotateSecretRequestRequestTypeDef](./type_defs.md#rotatesecretrequestrequesttypedef)
- [SecretListEntryTypeDef](./type_defs.md#secretlistentrytypedef)
- [ListSecretVersionIdsResponseTypeDef](./type_defs.md#listsecretversionidsresponsetypedef)
- [ListSecretsRequestPaginateTypeDef](./type_defs.md#listsecretsrequestpaginatetypedef)
- [ValidateResourcePolicyResponseTypeDef](./type_defs.md#validateresourcepolicyresponsetypedef)
- [ListSecretsResponseTypeDef](./type_defs.md#listsecretsresponsetypedef)

