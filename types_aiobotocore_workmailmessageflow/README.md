<a id="type-annotations-for-aiobotocore-workmailmessageflow-module"></a>

# Type annotations for aiobotocore WorkMailMessageFlow module

> [Index](..) > WorkMailMessageFlow

Auto-generated documentation for
[WorkMailMessageFlow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow)
type annotations stubs module
[types-aiobotocore-workmailmessageflow](https://pypi.org/project/types-aiobotocore-workmailmessageflow/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[workmailmessageflow]'

# install as a standalone
pip install types-aiobotocore-workmailmessageflow
```

- [Type annotations for aiobotocore WorkMailMessageFlow module](#type-annotations-for-aiobotocore-workmailmessageflow-module)
  - [WorkMailMessageFlowClient](#workmailmessageflowclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="workmailmessageflowclient"></a>

## WorkMailMessageFlowClient

Type annotations for `aiobotocore.create_client("workmailmessageflow")` as
[WorkMailMessageFlowClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_workmailmessageflow.client import WorkMailMessageFlowClient
```

<a id="methods"></a>

### Methods

- [can_paginate](./client.md#can_paginate)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_raw_message_content](./client.md#get_raw_message_content)
- [put_raw_message_content](./client.md#put_raw_message_content)

<a id="exceptions"></a>

### Exceptions

WorkMailMessageFlowClient [exceptions](./client.md#exceptions)

- ClientError
- InvalidContentLocation
- MessageFrozen
- MessageRejected
- ResourceNotFoundException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_workmailmessageflow.literals import ServiceName, ...
```

- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_workmailmessageflow.type_defs import GetRawMessageContentRequestRequestTypeDef, ...
```

- [GetRawMessageContentRequestRequestTypeDef](./type_defs.md#getrawmessagecontentrequestrequesttypedef)
- [GetRawMessageContentResponseTypeDef](./type_defs.md#getrawmessagecontentresponsetypedef)
- [PutRawMessageContentRequestRequestTypeDef](./type_defs.md#putrawmessagecontentrequestrequesttypedef)
- [RawMessageContentTypeDef](./type_defs.md#rawmessagecontenttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [S3ReferenceTypeDef](./type_defs.md#s3referencetypedef)
