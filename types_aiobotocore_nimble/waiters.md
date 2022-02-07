<a id="waiters-for-aiobotocore-nimblestudio-module"></a>

# Waiters for aiobotocore NimbleStudio module

> [Index](..) > [NimbleStudio](.) > Waiters

Auto-generated documentation for
[NimbleStudio](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
type annotations stubs module
[types-aiobotocore-nimble](https://pypi.org/project/types-aiobotocore-nimble/).

- [Waiters for aiobotocore NimbleStudio module](#waiters-for-aiobotocore-nimblestudio-module)
  - [LaunchProfileDeletedWaiter](#launchprofiledeletedwaiter)
  - [LaunchProfileReadyWaiter](#launchprofilereadywaiter)
  - [StreamingImageDeletedWaiter](#streamingimagedeletedwaiter)
  - [StreamingImageReadyWaiter](#streamingimagereadywaiter)
  - [StreamingSessionDeletedWaiter](#streamingsessiondeletedwaiter)
  - [StreamingSessionReadyWaiter](#streamingsessionreadywaiter)
  - [StreamingSessionStoppedWaiter](#streamingsessionstoppedwaiter)
  - [StreamingSessionStreamReadyWaiter](#streamingsessionstreamreadywaiter)
  - [StudioComponentDeletedWaiter](#studiocomponentdeletedwaiter)
  - [StudioComponentReadyWaiter](#studiocomponentreadywaiter)
  - [StudioDeletedWaiter](#studiodeletedwaiter)
  - [StudioReadyWaiter](#studioreadywaiter)

<a id="launchprofiledeletedwaiter"></a>

## LaunchProfileDeletedWaiter

Type annotations for
`session.create_client("nimble").get_waiter("launch_profile_deleted")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_nimble.waiter import LaunchProfileDeletedWaiter

def get_launch_profile_deleted_waiter() -> LaunchProfileDeletedWaiter:
    return Session().client("nimble").get_waiter("launch_profile_deleted")
```

Boto3 documentation:
[NimbleStudio.Waiter.launch_profile_deleted](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.LaunchProfileDeleted)

Arguments for `LaunchProfileDeletedWaiter.wait` method:

- `launchProfileId`: `str` *(required)*
- `studioId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="launchprofilereadywaiter"></a>

## LaunchProfileReadyWaiter

Type annotations for
`session.create_client("nimble").get_waiter("launch_profile_ready")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_nimble.waiter import LaunchProfileReadyWaiter

def get_launch_profile_ready_waiter() -> LaunchProfileReadyWaiter:
    return Session().client("nimble").get_waiter("launch_profile_ready")
```

Boto3 documentation:
[NimbleStudio.Waiter.launch_profile_ready](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.LaunchProfileReady)

Arguments for `LaunchProfileReadyWaiter.wait` method:

- `launchProfileId`: `str` *(required)*
- `studioId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="streamingimagedeletedwaiter"></a>

## StreamingImageDeletedWaiter

Type annotations for
`session.create_client("nimble").get_waiter("streaming_image_deleted")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_nimble.waiter import StreamingImageDeletedWaiter

def get_streaming_image_deleted_waiter() -> StreamingImageDeletedWaiter:
    return Session().client("nimble").get_waiter("streaming_image_deleted")
```

Boto3 documentation:
[NimbleStudio.Waiter.streaming_image_deleted](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.StreamingImageDeleted)

Arguments for `StreamingImageDeletedWaiter.wait` method:

- `streamingImageId`: `str` *(required)*
- `studioId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="streamingimagereadywaiter"></a>

## StreamingImageReadyWaiter

Type annotations for
`session.create_client("nimble").get_waiter("streaming_image_ready")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_nimble.waiter import StreamingImageReadyWaiter

def get_streaming_image_ready_waiter() -> StreamingImageReadyWaiter:
    return Session().client("nimble").get_waiter("streaming_image_ready")
```

Boto3 documentation:
[NimbleStudio.Waiter.streaming_image_ready](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.StreamingImageReady)

Arguments for `StreamingImageReadyWaiter.wait` method:

- `streamingImageId`: `str` *(required)*
- `studioId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="streamingsessiondeletedwaiter"></a>

## StreamingSessionDeletedWaiter

Type annotations for
`session.create_client("nimble").get_waiter("streaming_session_deleted")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_nimble.waiter import StreamingSessionDeletedWaiter

def get_streaming_session_deleted_waiter() -> StreamingSessionDeletedWaiter:
    return Session().client("nimble").get_waiter("streaming_session_deleted")
```

Boto3 documentation:
[NimbleStudio.Waiter.streaming_session_deleted](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.StreamingSessionDeleted)

Arguments for `StreamingSessionDeletedWaiter.wait` method:

- `sessionId`: `str` *(required)*
- `studioId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="streamingsessionreadywaiter"></a>

## StreamingSessionReadyWaiter

Type annotations for
`session.create_client("nimble").get_waiter("streaming_session_ready")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_nimble.waiter import StreamingSessionReadyWaiter

def get_streaming_session_ready_waiter() -> StreamingSessionReadyWaiter:
    return Session().client("nimble").get_waiter("streaming_session_ready")
```

Boto3 documentation:
[NimbleStudio.Waiter.streaming_session_ready](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.StreamingSessionReady)

Arguments for `StreamingSessionReadyWaiter.wait` method:

- `sessionId`: `str` *(required)*
- `studioId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="streamingsessionstoppedwaiter"></a>

## StreamingSessionStoppedWaiter

Type annotations for
`session.create_client("nimble").get_waiter("streaming_session_stopped")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_nimble.waiter import StreamingSessionStoppedWaiter

def get_streaming_session_stopped_waiter() -> StreamingSessionStoppedWaiter:
    return Session().client("nimble").get_waiter("streaming_session_stopped")
```

Boto3 documentation:
[NimbleStudio.Waiter.streaming_session_stopped](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.StreamingSessionStopped)

Arguments for `StreamingSessionStoppedWaiter.wait` method:

- `sessionId`: `str` *(required)*
- `studioId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="streamingsessionstreamreadywaiter"></a>

## StreamingSessionStreamReadyWaiter

Type annotations for
`session.create_client("nimble").get_waiter("streaming_session_stream_ready")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_nimble.waiter import StreamingSessionStreamReadyWaiter

def get_streaming_session_stream_ready_waiter() -> StreamingSessionStreamReadyWaiter:
    return Session().client("nimble").get_waiter("streaming_session_stream_ready")
```

Boto3 documentation:
[NimbleStudio.Waiter.streaming_session_stream_ready](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.StreamingSessionStreamReady)

Arguments for `StreamingSessionStreamReadyWaiter.wait` method:

- `sessionId`: `str` *(required)*
- `streamId`: `str` *(required)*
- `studioId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="studiocomponentdeletedwaiter"></a>

## StudioComponentDeletedWaiter

Type annotations for
`session.create_client("nimble").get_waiter("studio_component_deleted")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_nimble.waiter import StudioComponentDeletedWaiter

def get_studio_component_deleted_waiter() -> StudioComponentDeletedWaiter:
    return Session().client("nimble").get_waiter("studio_component_deleted")
```

Boto3 documentation:
[NimbleStudio.Waiter.studio_component_deleted](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.StudioComponentDeleted)

Arguments for `StudioComponentDeletedWaiter.wait` method:

- `studioComponentId`: `str` *(required)*
- `studioId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="studiocomponentreadywaiter"></a>

## StudioComponentReadyWaiter

Type annotations for
`session.create_client("nimble").get_waiter("studio_component_ready")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_nimble.waiter import StudioComponentReadyWaiter

def get_studio_component_ready_waiter() -> StudioComponentReadyWaiter:
    return Session().client("nimble").get_waiter("studio_component_ready")
```

Boto3 documentation:
[NimbleStudio.Waiter.studio_component_ready](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.StudioComponentReady)

Arguments for `StudioComponentReadyWaiter.wait` method:

- `studioComponentId`: `str` *(required)*
- `studioId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="studiodeletedwaiter"></a>

## StudioDeletedWaiter

Type annotations for
`session.create_client("nimble").get_waiter("studio_deleted")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_nimble.waiter import StudioDeletedWaiter

def get_studio_deleted_waiter() -> StudioDeletedWaiter:
    return Session().client("nimble").get_waiter("studio_deleted")
```

Boto3 documentation:
[NimbleStudio.Waiter.studio_deleted](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.StudioDeleted)

Arguments for `StudioDeletedWaiter.wait` method:

- `studioId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="studioreadywaiter"></a>

## StudioReadyWaiter

Type annotations for
`session.create_client("nimble").get_waiter("studio_ready")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_nimble.waiter import StudioReadyWaiter

def get_studio_ready_waiter() -> StudioReadyWaiter:
    return Session().client("nimble").get_waiter("studio_ready")
```

Boto3 documentation:
[NimbleStudio.Waiter.studio_ready](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.StudioReady)

Arguments for `StudioReadyWaiter.wait` method:

- `studioId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
