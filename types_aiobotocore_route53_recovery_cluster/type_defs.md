<a id="typed-dictionaries-for-aiobotocore-route53recoverycluster-module"></a>

# Typed dictionaries for aiobotocore Route53RecoveryCluster module

> [Index](..) > [Route53RecoveryCluster](.) > Typed dictionaries

Auto-generated documentation for
[Route53RecoveryCluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
type annotations stubs module
[types-aiobotocore-route53-recovery-cluster](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster/).

- [Typed dictionaries for aiobotocore Route53RecoveryCluster module](#typed-dictionaries-for-aiobotocore-route53recoverycluster-module)
  - [GetRoutingControlStateRequestRequestTypeDef](#getroutingcontrolstaterequestrequesttypedef)
  - [GetRoutingControlStateResponseTypeDef](#getroutingcontrolstateresponsetypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [UpdateRoutingControlStateEntryTypeDef](#updateroutingcontrolstateentrytypedef)
  - [UpdateRoutingControlStateRequestRequestTypeDef](#updateroutingcontrolstaterequestrequesttypedef)
  - [UpdateRoutingControlStatesRequestRequestTypeDef](#updateroutingcontrolstatesrequestrequesttypedef)

<a id="getroutingcontrolstaterequestrequesttypedef"></a>

## GetRoutingControlStateRequestRequestTypeDef

```python
from types_aiobotocore_route53_recovery_cluster.type_defs import GetRoutingControlStateRequestRequestTypeDef
```

Required fields:

- `RoutingControlArn`: `str`

<a id="getroutingcontrolstateresponsetypedef"></a>

## GetRoutingControlStateResponseTypeDef

```python
from types_aiobotocore_route53_recovery_cluster.type_defs import GetRoutingControlStateResponseTypeDef
```

Required fields:

- `RoutingControlArn`: `str`
- `RoutingControlState`:
  [RoutingControlStateType](./literals.md#routingcontrolstatetype)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_route53_recovery_cluster.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="updateroutingcontrolstateentrytypedef"></a>

## UpdateRoutingControlStateEntryTypeDef

```python
from types_aiobotocore_route53_recovery_cluster.type_defs import UpdateRoutingControlStateEntryTypeDef
```

Required fields:

- `RoutingControlArn`: `str`
- `RoutingControlState`:
  [RoutingControlStateType](./literals.md#routingcontrolstatetype)

<a id="updateroutingcontrolstaterequestrequesttypedef"></a>

## UpdateRoutingControlStateRequestRequestTypeDef

```python
from types_aiobotocore_route53_recovery_cluster.type_defs import UpdateRoutingControlStateRequestRequestTypeDef
```

Required fields:

- `RoutingControlArn`: `str`
- `RoutingControlState`:
  [RoutingControlStateType](./literals.md#routingcontrolstatetype)

<a id="updateroutingcontrolstatesrequestrequesttypedef"></a>

## UpdateRoutingControlStatesRequestRequestTypeDef

```python
from types_aiobotocore_route53_recovery_cluster.type_defs import UpdateRoutingControlStatesRequestRequestTypeDef
```

Required fields:

- `UpdateRoutingControlStateEntries`:
  `Sequence`\[[UpdateRoutingControlStateEntryTypeDef](./type_defs.md#updateroutingcontrolstateentrytypedef)\]
