# Kinesis module

> [Index](../README.md) > Kinesis


!!! note ""

    Auto-generated documentation for [Kinesis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#kinesis)
    type annotations stubs module [types-aiobotocore-kinesis](https://pypi.org/project/types-aiobotocore-kinesis/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Kinesis` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Kinesis` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[kinesis]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[kinesis]'

# standalone installation
python -m pip install types-aiobotocore-kinesis
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-kinesis
```

## Usage

Code samples can be found in [Examples](./usage.md).

## KinesisClient

Type annotations and code completion for  `#!python session.create_client("kinesis")` as [KinesisClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client)

```python
# KinesisClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_kinesis.client import KinesisClient


session = get_session()
async with session.create_client("kinesis") as client:
    client: KinesisClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("kinesis").get_paginator("...")`.

```python
# DescribeStreamPaginator usage example

from types_aiobotocore_kinesis.paginator import DescribeStreamPaginator

def get_describe_stream_paginator() -> DescribeStreamPaginator:
    return client.get_paginator("describe_stream"))
```

- [DescribeStreamPaginator](./paginators.md#describestreampaginator)
- [ListShardsPaginator](./paginators.md#listshardspaginator)
- [ListStreamConsumersPaginator](./paginators.md#liststreamconsumerspaginator)
- [ListStreamsPaginator](./paginators.md#liststreamspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("kinesis").get_waiter("...")`.

```python
# StreamExistsWaiter usage example

from types_aiobotocore_kinesis.waiter import StreamExistsWaiter

def get_stream_exists_waiter() -> StreamExistsWaiter:
    return Session().client("kinesis").get_waiter("stream_exists")
```

- [StreamExistsWaiter](./waiters.md#streamexistswaiter)
- [StreamNotExistsWaiter](./waiters.md#streamnotexistswaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ConsumerStatusType usage example

from types_aiobotocore_kinesis.literals import ConsumerStatusType

def get_value() -> ConsumerStatusType:
    return "ACTIVE"
```

- [ConsumerStatusType](./literals.md#consumerstatustype)
- [DescribeStreamPaginatorName](./literals.md#describestreampaginatorname)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [ListShardsPaginatorName](./literals.md#listshardspaginatorname)
- [ListStreamConsumersPaginatorName](./literals.md#liststreamconsumerspaginatorname)
- [ListStreamsPaginatorName](./literals.md#liststreamspaginatorname)
- [MetricsNameType](./literals.md#metricsnametype)
- [MinimumThroughputBillingCommitmentInputStatusType](./literals.md#minimumthroughputbillingcommitmentinputstatustype)
- [MinimumThroughputBillingCommitmentOutputStatusType](./literals.md#minimumthroughputbillingcommitmentoutputstatustype)
- [ScalingTypeType](./literals.md#scalingtypetype)
- [ShardFilterTypeType](./literals.md#shardfiltertypetype)
- [ShardIteratorTypeType](./literals.md#sharditeratortypetype)
- [StreamExistsWaiterName](./literals.md#streamexistswaitername)
- [StreamModeType](./literals.md#streammodetype)
- [StreamNotExistsWaiterName](./literals.md#streamnotexistswaitername)
- [StreamStatusType](./literals.md#streamstatustype)
- [KinesisServiceName](./literals.md#kinesisservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AddTagsToStreamInputTypeDef](./type_defs.md#addtagstostreaminputtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [HashKeyRangeTypeDef](./type_defs.md#hashkeyrangetypedef)
- [ConsumerDescriptionTypeDef](./type_defs.md#consumerdescriptiontypedef)
- [ConsumerTypeDef](./type_defs.md#consumertypedef)
- [StreamModeDetailsTypeDef](./type_defs.md#streammodedetailstypedef)
- [DecreaseStreamRetentionPeriodInputTypeDef](./type_defs.md#decreasestreamretentionperiodinputtypedef)
- [DeleteResourcePolicyInputTypeDef](./type_defs.md#deleteresourcepolicyinputtypedef)
- [DeleteStreamInputTypeDef](./type_defs.md#deletestreaminputtypedef)
- [DeregisterStreamConsumerInputTypeDef](./type_defs.md#deregisterstreamconsumerinputtypedef)
- [MinimumThroughputBillingCommitmentOutputTypeDef](./type_defs.md#minimumthroughputbillingcommitmentoutputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DescribeStreamConsumerInputTypeDef](./type_defs.md#describestreamconsumerinputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeStreamInputTypeDef](./type_defs.md#describestreaminputtypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeStreamSummaryInputTypeDef](./type_defs.md#describestreamsummaryinputtypedef)
- [DisableEnhancedMonitoringInputTypeDef](./type_defs.md#disableenhancedmonitoringinputtypedef)
- [EnableEnhancedMonitoringInputTypeDef](./type_defs.md#enableenhancedmonitoringinputtypedef)
- [EnhancedMetricsTypeDef](./type_defs.md#enhancedmetricstypedef)
- [GetRecordsInputTypeDef](./type_defs.md#getrecordsinputtypedef)
- [RecordTypeDef](./type_defs.md#recordtypedef)
- [GetResourcePolicyInputTypeDef](./type_defs.md#getresourcepolicyinputtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [IncreaseStreamRetentionPeriodInputTypeDef](./type_defs.md#increasestreamretentionperiodinputtypedef)
- [InternalFailureExceptionTypeDef](./type_defs.md#internalfailureexceptiontypedef)
- [KMSAccessDeniedExceptionTypeDef](./type_defs.md#kmsaccessdeniedexceptiontypedef)
- [KMSDisabledExceptionTypeDef](./type_defs.md#kmsdisabledexceptiontypedef)
- [KMSInvalidStateExceptionTypeDef](./type_defs.md#kmsinvalidstateexceptiontypedef)
- [KMSNotFoundExceptionTypeDef](./type_defs.md#kmsnotfoundexceptiontypedef)
- [KMSOptInRequiredTypeDef](./type_defs.md#kmsoptinrequiredtypedef)
- [KMSThrottlingExceptionTypeDef](./type_defs.md#kmsthrottlingexceptiontypedef)
- [ListStreamsInputTypeDef](./type_defs.md#liststreamsinputtypedef)
- [ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ListTagsForStreamInputTypeDef](./type_defs.md#listtagsforstreaminputtypedef)
- [MergeShardsInputTypeDef](./type_defs.md#mergeshardsinputtypedef)
- [MinimumThroughputBillingCommitmentInputTypeDef](./type_defs.md#minimumthroughputbillingcommitmentinputtypedef)
- [PutRecordsResultEntryTypeDef](./type_defs.md#putrecordsresultentrytypedef)
- [PutResourcePolicyInputTypeDef](./type_defs.md#putresourcepolicyinputtypedef)
- [RegisterStreamConsumerInputTypeDef](./type_defs.md#registerstreamconsumerinputtypedef)
- [RemoveTagsFromStreamInputTypeDef](./type_defs.md#removetagsfromstreaminputtypedef)
- [ResourceInUseExceptionTypeDef](./type_defs.md#resourceinuseexceptiontypedef)
- [ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef)
- [SequenceNumberRangeTypeDef](./type_defs.md#sequencenumberrangetypedef)
- [SplitShardInputTypeDef](./type_defs.md#splitshardinputtypedef)
- [StartStreamEncryptionInputTypeDef](./type_defs.md#startstreamencryptioninputtypedef)
- [StopStreamEncryptionInputTypeDef](./type_defs.md#stopstreamencryptioninputtypedef)
- [WarmThroughputObjectTypeDef](./type_defs.md#warmthroughputobjecttypedef)
- [TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)
- [UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)
- [UpdateMaxRecordSizeInputTypeDef](./type_defs.md#updatemaxrecordsizeinputtypedef)
- [UpdateShardCountInputTypeDef](./type_defs.md#updateshardcountinputtypedef)
- [UpdateStreamWarmThroughputInputTypeDef](./type_defs.md#updatestreamwarmthroughputinputtypedef)
- [PutRecordInputTypeDef](./type_defs.md#putrecordinputtypedef)
- [PutRecordsRequestEntryTypeDef](./type_defs.md#putrecordsrequestentrytypedef)
- [ChildShardTypeDef](./type_defs.md#childshardtypedef)
- [CreateStreamInputTypeDef](./type_defs.md#createstreaminputtypedef)
- [StreamSummaryTypeDef](./type_defs.md#streamsummarytypedef)
- [UpdateStreamModeInputTypeDef](./type_defs.md#updatestreammodeinputtypedef)
- [DescribeAccountSettingsOutputTypeDef](./type_defs.md#describeaccountsettingsoutputtypedef)
- [DescribeLimitsOutputTypeDef](./type_defs.md#describelimitsoutputtypedef)
- [DescribeStreamConsumerOutputTypeDef](./type_defs.md#describestreamconsumeroutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [EnhancedMonitoringOutputTypeDef](./type_defs.md#enhancedmonitoringoutputtypedef)
- [GetResourcePolicyOutputTypeDef](./type_defs.md#getresourcepolicyoutputtypedef)
- [GetShardIteratorOutputTypeDef](./type_defs.md#getsharditeratoroutputtypedef)
- [ListStreamConsumersOutputTypeDef](./type_defs.md#liststreamconsumersoutputtypedef)
- [PutRecordOutputTypeDef](./type_defs.md#putrecordoutputtypedef)
- [RegisterStreamConsumerOutputTypeDef](./type_defs.md#registerstreamconsumeroutputtypedef)
- [UpdateAccountSettingsOutputTypeDef](./type_defs.md#updateaccountsettingsoutputtypedef)
- [UpdateShardCountOutputTypeDef](./type_defs.md#updateshardcountoutputtypedef)
- [DescribeStreamInputPaginateTypeDef](./type_defs.md#describestreaminputpaginatetypedef)
- [ListStreamsInputPaginateTypeDef](./type_defs.md#liststreamsinputpaginatetypedef)
- [DescribeStreamInputWaitExtraTypeDef](./type_defs.md#describestreaminputwaitextratypedef)
- [DescribeStreamInputWaitTypeDef](./type_defs.md#describestreaminputwaittypedef)
- [GetShardIteratorInputTypeDef](./type_defs.md#getsharditeratorinputtypedef)
- [ListStreamConsumersInputPaginateTypeDef](./type_defs.md#liststreamconsumersinputpaginatetypedef)
- [ListStreamConsumersInputTypeDef](./type_defs.md#liststreamconsumersinputtypedef)
- [ShardFilterTypeDef](./type_defs.md#shardfiltertypedef)
- [StartingPositionTypeDef](./type_defs.md#startingpositiontypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [ListTagsForStreamOutputTypeDef](./type_defs.md#listtagsforstreamoutputtypedef)
- [UpdateAccountSettingsInputTypeDef](./type_defs.md#updateaccountsettingsinputtypedef)
- [PutRecordsOutputTypeDef](./type_defs.md#putrecordsoutputtypedef)
- [ShardTypeDef](./type_defs.md#shardtypedef)
- [StreamDescriptionSummaryTypeDef](./type_defs.md#streamdescriptionsummarytypedef)
- [UpdateStreamWarmThroughputOutputTypeDef](./type_defs.md#updatestreamwarmthroughputoutputtypedef)
- [PutRecordsInputTypeDef](./type_defs.md#putrecordsinputtypedef)
- [GetRecordsOutputTypeDef](./type_defs.md#getrecordsoutputtypedef)
- [SubscribeToShardEventTypeDef](./type_defs.md#subscribetoshardeventtypedef)
- [ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef)
- [ListShardsInputPaginateTypeDef](./type_defs.md#listshardsinputpaginatetypedef)
- [ListShardsInputTypeDef](./type_defs.md#listshardsinputtypedef)
- [SubscribeToShardInputTypeDef](./type_defs.md#subscribetoshardinputtypedef)
- [ListShardsOutputTypeDef](./type_defs.md#listshardsoutputtypedef)
- [StreamDescriptionTypeDef](./type_defs.md#streamdescriptiontypedef)
- [DescribeStreamSummaryOutputTypeDef](./type_defs.md#describestreamsummaryoutputtypedef)
- [SubscribeToShardEventStreamTypeDef](./type_defs.md#subscribetoshardeventstreamtypedef)
- [DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef)
- [SubscribeToShardOutputTypeDef](./type_defs.md#subscribetoshardoutputtypedef)

