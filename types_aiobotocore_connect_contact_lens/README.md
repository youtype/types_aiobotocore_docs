<a id="type-annotations-for-aiobotocore-connectcontactlens-module"></a>

# Type annotations for aiobotocore ConnectContactLens module

> [Index](..) > ConnectContactLens

Auto-generated documentation for
[ConnectContactLens](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
type annotations stubs module
[types-aiobotocore-connect-contact-lens](https://pypi.org/project/types-aiobotocore-connect-contact-lens/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[connect-contact-lens]'

# install as a standalone
pip install types-aiobotocore-connect-contact-lens
```

- [Type annotations for aiobotocore ConnectContactLens module](#type-annotations-for-aiobotocore-connectcontactlens-module)
  - [ConnectContactLensClient](#connectcontactlensclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="connectcontactlensclient"></a>

## ConnectContactLensClient

Type annotations for `aiobotocore.create_client("connect-contact-lens")` as
[ConnectContactLensClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_connect_contact_lens.client import ConnectContactLensClient
```

<a id="methods"></a>

### Methods

- [can_paginate](./client.md#can_paginate)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [list_realtime_contact_analysis_segments](./client.md#list_realtime_contact_analysis_segments)

<a id="exceptions"></a>

### Exceptions

ConnectContactLensClient [exceptions](./client.md#exceptions)

- AccessDeniedException
- ClientError
- InternalServiceException
- InvalidRequestException
- ResourceNotFoundException
- ThrottlingException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_connect_contact_lens.literals import SentimentValueType, ...
```

- [SentimentValueType](./literals.md#sentimentvaluetype)
- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_connect_contact_lens.type_defs import CategoriesTypeDef, ...
```

- [CategoriesTypeDef](./type_defs.md#categoriestypedef)
- [CategoryDetailsTypeDef](./type_defs.md#categorydetailstypedef)
- [CharacterOffsetsTypeDef](./type_defs.md#characteroffsetstypedef)
- [IssueDetectedTypeDef](./type_defs.md#issuedetectedtypedef)
- [ListRealtimeContactAnalysisSegmentsRequestRequestTypeDef](./type_defs.md#listrealtimecontactanalysissegmentsrequestrequesttypedef)
- [ListRealtimeContactAnalysisSegmentsResponseTypeDef](./type_defs.md#listrealtimecontactanalysissegmentsresponsetypedef)
- [PointOfInterestTypeDef](./type_defs.md#pointofinteresttypedef)
- [RealtimeContactAnalysisSegmentTypeDef](./type_defs.md#realtimecontactanalysissegmenttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TranscriptTypeDef](./type_defs.md#transcripttypedef)
