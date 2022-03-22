<a id="elasticinferenceclient-for-aiobotocore-elasticinference-module"></a>

# ElasticInferenceClient for aiobotocore ElasticInference module

> [Index](../README.md) > [ElasticInference](./README.md) >
> ElasticInferenceClient

Auto-generated documentation for
[ElasticInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
type annotations stubs module
[types-aiobotocore-elastic-inference](https://pypi.org/project/types-aiobotocore-elastic-inference/).

- [ElasticInferenceClient for aiobotocore ElasticInference module](#elasticinferenceclient-for-aiobotocore-elasticinference-module)
  - [ElasticInferenceClient](#elasticinferenceclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [describe_accelerator_offerings](#describe_accelerator_offerings)
    - [describe_accelerator_types](#describe_accelerator_types)
    - [describe_accelerators](#describe_accelerators)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="elasticinferenceclient"></a>

## ElasticInferenceClient

Type annotations for `session.create_client("elastic-inference")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_elastic_inference.client import ElasticInferenceClient

session = get_session()
async with session.create_client("elastic-inference") as client:
    client: ElasticInferenceClient
```

Boto3 documentation:
[ElasticInference.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_elastic_inference.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ElasticInferenceClient exceptions.

Type annotations for `session.create_client("elastic-inference").exceptions`
method.

Boto3 documentation:
[ElasticInference.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("elastic-inference").can_paginate`
method.

Boto3 documentation:
[ElasticInference.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="describe\_accelerator\_offerings"></a>

### describe_accelerator_offerings

Describes the locations in which a given accelerator type or set of types is
present in a given region.

Type annotations for
`session.create_client("elastic-inference").describe_accelerator_offerings`
method.

Boto3 documentation:
[ElasticInference.Client.describe_accelerator_offerings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.describe_accelerator_offerings)

Asynchronous method. Use `await describe_accelerator_offerings(...)` for a
synchronous call.

Arguments mapping described in
[DescribeAcceleratorOfferingsRequestRequestTypeDef](./type_defs.md#describeacceleratorofferingsrequestrequesttypedef).

Keyword-only arguments:

- `locationType`: [LocationTypeType](./literals.md#locationtypetype)
  *(required)*
- `acceleratorTypes`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[DescribeAcceleratorOfferingsResponseTypeDef](./type_defs.md#describeacceleratorofferingsresponsetypedef).

<a id="describe\_accelerator\_types"></a>

### describe_accelerator_types

Describes the accelerator types available in a given region, as well as their
characteristics, such as memory and throughput.

Type annotations for
`session.create_client("elastic-inference").describe_accelerator_types` method.

Boto3 documentation:
[ElasticInference.Client.describe_accelerator_types](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.describe_accelerator_types)

Asynchronous method. Use `await describe_accelerator_types(...)` for a
synchronous call.

Returns a `Coroutine` for
[DescribeAcceleratorTypesResponseTypeDef](./type_defs.md#describeacceleratortypesresponsetypedef).

<a id="describe\_accelerators"></a>

### describe_accelerators

Describes information over a provided set of accelerators belonging to an
account.

Type annotations for
`session.create_client("elastic-inference").describe_accelerators` method.

Boto3 documentation:
[ElasticInference.Client.describe_accelerators](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.describe_accelerators)

Asynchronous method. Use `await describe_accelerators(...)` for a synchronous
call.

Arguments mapping described in
[DescribeAcceleratorsRequestRequestTypeDef](./type_defs.md#describeacceleratorsrequestrequesttypedef).

Keyword-only arguments:

- `acceleratorIds`: `Sequence`\[`str`\]
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[DescribeAcceleratorsResponseTypeDef](./type_defs.md#describeacceleratorsresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("elastic-inference").generate_presigned_url` method.

Boto3 documentation:
[ElasticInference.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Returns all tags of an Elastic Inference Accelerator.

Type annotations for
`session.create_client("elastic-inference").list_tags_for_resource` method.

Boto3 documentation:
[ElasticInference.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef).

<a id="tag\_resource"></a>

### tag_resource

Adds the specified tags to an Elastic Inference Accelerator.

Type annotations for `session.create_client("elastic-inference").tag_resource`
method.

Boto3 documentation:
[ElasticInference.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Removes the specified tags from an Elastic Inference Accelerator.

Type annotations for
`session.create_client("elastic-inference").untag_resource` method.

Boto3 documentation:
[ElasticInference.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("elastic-inference").__aenter__`
method.

Boto3 documentation:
[ElasticInference.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [ElasticInferenceClient](#elasticinferenceclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("elastic-inference").__aexit__`
method.

Boto3 documentation:
[ElasticInference.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("elastic-inference").get_paginator`
method with overloads.

- `client.get_paginator("describe_accelerators")` ->
  [DescribeAcceleratorsPaginator](./paginators.md#describeacceleratorspaginator)
