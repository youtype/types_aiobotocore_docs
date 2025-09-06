# Synthetics module

> [Index](../README.md) > Synthetics


!!! note ""

    Auto-generated documentation for [Synthetics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#synthetics)
    type annotations stubs module [types-aiobotocore-synthetics](https://pypi.org/project/types-aiobotocore-synthetics/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Synthetics` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Synthetics` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[synthetics]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[synthetics]'

# standalone installation
python -m pip install types-aiobotocore-synthetics
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-synthetics
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SyntheticsClient

Type annotations and code completion for  `#!python session.create_client("synthetics")` as [SyntheticsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client)

```python
# SyntheticsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_synthetics.client import SyntheticsClient


session = get_session()
async with session.create_client("synthetics") as client:
    client: SyntheticsClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BrowserTypeType usage example

from types_aiobotocore_synthetics.literals import BrowserTypeType

def get_value() -> BrowserTypeType:
    return "CHROME"
```

- [BrowserTypeType](./literals.md#browsertypetype)
- [CanaryRunStateReasonCodeType](./literals.md#canaryrunstatereasoncodetype)
- [CanaryRunStateType](./literals.md#canaryrunstatetype)
- [CanaryRunTestResultType](./literals.md#canaryruntestresulttype)
- [CanaryStateReasonCodeType](./literals.md#canarystatereasoncodetype)
- [CanaryStateType](./literals.md#canarystatetype)
- [DependencyTypeType](./literals.md#dependencytypetype)
- [EncryptionModeType](./literals.md#encryptionmodetype)
- [ProvisionedResourceCleanupSettingType](./literals.md#provisionedresourcecleanupsettingtype)
- [ResourceToTagType](./literals.md#resourcetotagtype)
- [RunTypeType](./literals.md#runtypetype)
- [SyntheticsServiceName](./literals.md#syntheticsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [S3EncryptionConfigTypeDef](./type_defs.md#s3encryptionconfigtypedef)
- [AssociateResourceRequestTypeDef](./type_defs.md#associateresourcerequesttypedef)
- [BaseScreenshotOutputTypeDef](./type_defs.md#basescreenshotoutputtypedef)
- [BaseScreenshotTypeDef](./type_defs.md#basescreenshottypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [BrowserConfigTypeDef](./type_defs.md#browserconfigtypedef)
- [DependencyTypeDef](./type_defs.md#dependencytypedef)
- [CanaryDryRunConfigOutputTypeDef](./type_defs.md#canarydryrunconfigoutputtypedef)
- [CanaryRunConfigInputTypeDef](./type_defs.md#canaryrunconfiginputtypedef)
- [CanaryRunConfigOutputTypeDef](./type_defs.md#canaryrunconfigoutputtypedef)
- [CanaryRunStatusTypeDef](./type_defs.md#canaryrunstatustypedef)
- [CanaryRunTimelineTypeDef](./type_defs.md#canaryruntimelinetypedef)
- [RetryConfigInputTypeDef](./type_defs.md#retryconfiginputtypedef)
- [RetryConfigOutputTypeDef](./type_defs.md#retryconfigoutputtypedef)
- [CanaryStatusTypeDef](./type_defs.md#canarystatustypedef)
- [CanaryTimelineTypeDef](./type_defs.md#canarytimelinetypedef)
- [DryRunConfigOutputTypeDef](./type_defs.md#dryrunconfigoutputtypedef)
- [EngineConfigTypeDef](./type_defs.md#engineconfigtypedef)
- [VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
- [VpcConfigInputTypeDef](./type_defs.md#vpcconfiginputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateGroupRequestTypeDef](./type_defs.md#creategrouprequesttypedef)
- [GroupTypeDef](./type_defs.md#grouptypedef)
- [DeleteCanaryRequestTypeDef](./type_defs.md#deletecanaryrequesttypedef)
- [DeleteGroupRequestTypeDef](./type_defs.md#deletegrouprequesttypedef)
- [DescribeCanariesLastRunRequestTypeDef](./type_defs.md#describecanarieslastrunrequesttypedef)
- [DescribeCanariesRequestTypeDef](./type_defs.md#describecanariesrequesttypedef)
- [DescribeRuntimeVersionsRequestTypeDef](./type_defs.md#describeruntimeversionsrequesttypedef)
- [RuntimeVersionTypeDef](./type_defs.md#runtimeversiontypedef)
- [DisassociateResourceRequestTypeDef](./type_defs.md#disassociateresourcerequesttypedef)
- [GetCanaryRequestTypeDef](./type_defs.md#getcanaryrequesttypedef)
- [GetCanaryRunsRequestTypeDef](./type_defs.md#getcanaryrunsrequesttypedef)
- [GetGroupRequestTypeDef](./type_defs.md#getgrouprequesttypedef)
- [GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef)
- [ListAssociatedGroupsRequestTypeDef](./type_defs.md#listassociatedgroupsrequesttypedef)
- [ListGroupResourcesRequestTypeDef](./type_defs.md#listgroupresourcesrequesttypedef)
- [ListGroupsRequestTypeDef](./type_defs.md#listgroupsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [StartCanaryRequestTypeDef](./type_defs.md#startcanaryrequesttypedef)
- [StopCanaryRequestTypeDef](./type_defs.md#stopcanaryrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [ArtifactConfigInputTypeDef](./type_defs.md#artifactconfiginputtypedef)
- [ArtifactConfigOutputTypeDef](./type_defs.md#artifactconfigoutputtypedef)
- [VisualReferenceOutputTypeDef](./type_defs.md#visualreferenceoutputtypedef)
- [BaseScreenshotUnionTypeDef](./type_defs.md#basescreenshotuniontypedef)
- [CanaryCodeInputTypeDef](./type_defs.md#canarycodeinputtypedef)
- [CanaryCodeOutputTypeDef](./type_defs.md#canarycodeoutputtypedef)
- [CanaryRunTypeDef](./type_defs.md#canaryruntypedef)
- [CanaryScheduleInputTypeDef](./type_defs.md#canaryscheduleinputtypedef)
- [CanaryScheduleOutputTypeDef](./type_defs.md#canaryscheduleoutputtypedef)
- [ListGroupResourcesResponseTypeDef](./type_defs.md#listgroupresourcesresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartCanaryDryRunResponseTypeDef](./type_defs.md#startcanarydryrunresponsetypedef)
- [CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef)
- [GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef)
- [DescribeRuntimeVersionsResponseTypeDef](./type_defs.md#describeruntimeversionsresponsetypedef)
- [ListAssociatedGroupsResponseTypeDef](./type_defs.md#listassociatedgroupsresponsetypedef)
- [ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef)
- [VisualReferenceInputTypeDef](./type_defs.md#visualreferenceinputtypedef)
- [CanaryLastRunTypeDef](./type_defs.md#canarylastruntypedef)
- [GetCanaryRunsResponseTypeDef](./type_defs.md#getcanaryrunsresponsetypedef)
- [CreateCanaryRequestTypeDef](./type_defs.md#createcanaryrequesttypedef)
- [CanaryTypeDef](./type_defs.md#canarytypedef)
- [StartCanaryDryRunRequestTypeDef](./type_defs.md#startcanarydryrunrequesttypedef)
- [UpdateCanaryRequestTypeDef](./type_defs.md#updatecanaryrequesttypedef)
- [DescribeCanariesLastRunResponseTypeDef](./type_defs.md#describecanarieslastrunresponsetypedef)
- [CreateCanaryResponseTypeDef](./type_defs.md#createcanaryresponsetypedef)
- [DescribeCanariesResponseTypeDef](./type_defs.md#describecanariesresponsetypedef)
- [GetCanaryResponseTypeDef](./type_defs.md#getcanaryresponsetypedef)

