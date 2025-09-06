# CloudWatchObservabilityAdminService module

> [Index](../README.md) > CloudWatchObservabilityAdminService


!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAdminService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#cloudwatchobservabilityadminservice)
    type annotations stubs module [types-aiobotocore-observabilityadmin](https://pypi.org/project/types-aiobotocore-observabilityadmin/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudWatchObservabilityAdminService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CloudWatchObservabilityAdminService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[observabilityadmin]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[observabilityadmin]'

# standalone installation
python -m pip install types-aiobotocore-observabilityadmin
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-observabilityadmin
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudWatchObservabilityAdminServiceClient

Type annotations and code completion for  `#!python session.create_client("observabilityadmin")` as [CloudWatchObservabilityAdminServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#CloudWatchObservabilityAdminService.Client)

```python
# CloudWatchObservabilityAdminServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_observabilityadmin.client import CloudWatchObservabilityAdminServiceClient


session = get_session()
async with session.create_client("observabilityadmin") as client:
    client: CloudWatchObservabilityAdminServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("observabilityadmin").get_paginator("...")`.

```python
# ListResourceTelemetryForOrganizationPaginator usage example

from types_aiobotocore_observabilityadmin.paginator import ListResourceTelemetryForOrganizationPaginator

def get_list_resource_telemetry_for_organization_paginator() -> ListResourceTelemetryForOrganizationPaginator:
    return client.get_paginator("list_resource_telemetry_for_organization"))
```

- [ListResourceTelemetryForOrganizationPaginator](./paginators.md#listresourcetelemetryfororganizationpaginator)
- [ListResourceTelemetryPaginator](./paginators.md#listresourcetelemetrypaginator)
- [ListTelemetryRulesForOrganizationPaginator](./paginators.md#listtelemetryrulesfororganizationpaginator)
- [ListTelemetryRulesPaginator](./paginators.md#listtelemetryrulespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DestinationTypeType usage example

from types_aiobotocore_observabilityadmin.literals import DestinationTypeType

def get_value() -> DestinationTypeType:
    return "cloud-watch-logs"
```

- [DestinationTypeType](./literals.md#destinationtypetype)
- [ListResourceTelemetryForOrganizationPaginatorName](./literals.md#listresourcetelemetryfororganizationpaginatorname)
- [ListResourceTelemetryPaginatorName](./literals.md#listresourcetelemetrypaginatorname)
- [ListTelemetryRulesForOrganizationPaginatorName](./literals.md#listtelemetryrulesfororganizationpaginatorname)
- [ListTelemetryRulesPaginatorName](./literals.md#listtelemetryrulespaginatorname)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [StatusType](./literals.md#statustype)
- [TelemetryStateType](./literals.md#telemetrystatetype)
- [TelemetryTypeType](./literals.md#telemetrytypetype)
- [CloudWatchObservabilityAdminServiceServiceName](./literals.md#cloudwatchobservabilityadminserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteTelemetryRuleForOrganizationInputTypeDef](./type_defs.md#deletetelemetryrulefororganizationinputtypedef)
- [DeleteTelemetryRuleInputTypeDef](./type_defs.md#deletetelemetryruleinputtypedef)
- [GetTelemetryRuleForOrganizationInputTypeDef](./type_defs.md#gettelemetryrulefororganizationinputtypedef)
- [GetTelemetryRuleInputTypeDef](./type_defs.md#gettelemetryruleinputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListResourceTelemetryForOrganizationInputTypeDef](./type_defs.md#listresourcetelemetryfororganizationinputtypedef)
- [TelemetryConfigurationTypeDef](./type_defs.md#telemetryconfigurationtypedef)
- [ListResourceTelemetryInputTypeDef](./type_defs.md#listresourcetelemetryinputtypedef)
- [ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)
- [ListTelemetryRulesForOrganizationInputTypeDef](./type_defs.md#listtelemetryrulesfororganizationinputtypedef)
- [TelemetryRuleSummaryTypeDef](./type_defs.md#telemetryrulesummarytypedef)
- [ListTelemetryRulesInputTypeDef](./type_defs.md#listtelemetryrulesinputtypedef)
- [TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)
- [VPCFlowLogParametersTypeDef](./type_defs.md#vpcflowlogparameterstypedef)
- [UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)
- [CreateTelemetryRuleForOrganizationOutputTypeDef](./type_defs.md#createtelemetryrulefororganizationoutputtypedef)
- [CreateTelemetryRuleOutputTypeDef](./type_defs.md#createtelemetryruleoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetTelemetryEvaluationStatusForOrganizationOutputTypeDef](./type_defs.md#gettelemetryevaluationstatusfororganizationoutputtypedef)
- [GetTelemetryEvaluationStatusOutputTypeDef](./type_defs.md#gettelemetryevaluationstatusoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [UpdateTelemetryRuleForOrganizationOutputTypeDef](./type_defs.md#updatetelemetryrulefororganizationoutputtypedef)
- [UpdateTelemetryRuleOutputTypeDef](./type_defs.md#updatetelemetryruleoutputtypedef)
- [ListResourceTelemetryForOrganizationInputPaginateTypeDef](./type_defs.md#listresourcetelemetryfororganizationinputpaginatetypedef)
- [ListResourceTelemetryInputPaginateTypeDef](./type_defs.md#listresourcetelemetryinputpaginatetypedef)
- [ListTelemetryRulesForOrganizationInputPaginateTypeDef](./type_defs.md#listtelemetryrulesfororganizationinputpaginatetypedef)
- [ListTelemetryRulesInputPaginateTypeDef](./type_defs.md#listtelemetryrulesinputpaginatetypedef)
- [ListResourceTelemetryForOrganizationOutputTypeDef](./type_defs.md#listresourcetelemetryfororganizationoutputtypedef)
- [ListResourceTelemetryOutputTypeDef](./type_defs.md#listresourcetelemetryoutputtypedef)
- [ListTelemetryRulesForOrganizationOutputTypeDef](./type_defs.md#listtelemetryrulesfororganizationoutputtypedef)
- [ListTelemetryRulesOutputTypeDef](./type_defs.md#listtelemetryrulesoutputtypedef)
- [TelemetryDestinationConfigurationTypeDef](./type_defs.md#telemetrydestinationconfigurationtypedef)
- [TelemetryRuleTypeDef](./type_defs.md#telemetryruletypedef)
- [CreateTelemetryRuleForOrganizationInputTypeDef](./type_defs.md#createtelemetryrulefororganizationinputtypedef)
- [CreateTelemetryRuleInputTypeDef](./type_defs.md#createtelemetryruleinputtypedef)
- [GetTelemetryRuleForOrganizationOutputTypeDef](./type_defs.md#gettelemetryrulefororganizationoutputtypedef)
- [GetTelemetryRuleOutputTypeDef](./type_defs.md#gettelemetryruleoutputtypedef)
- [UpdateTelemetryRuleForOrganizationInputTypeDef](./type_defs.md#updatetelemetryrulefororganizationinputtypedef)
- [UpdateTelemetryRuleInputTypeDef](./type_defs.md#updatetelemetryruleinputtypedef)

