# LaunchWizard module

> [Index](../README.md) > LaunchWizard


!!! note ""

    Auto-generated documentation for [LaunchWizard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
    type annotations stubs module [types-aiobotocore-launch-wizard](https://pypi.org/project/types-aiobotocore-launch-wizard/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `LaunchWizard` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[launch-wizard]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[launch-wizard]'


# standalone installation
python -m pip install types-aiobotocore-launch-wizard
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-launch-wizard
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LaunchWizardClient

Type annotations and code completion for  `#!python session.create_client("launch-wizard")` as [LaunchWizardClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client)

```python
# LaunchWizardClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_launch_wizard.client import LaunchWizardClient


session = get_session()
async with session.create_client("launch-wizard") as client:
    client: LaunchWizardClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("launch-wizard").get_paginator("...")`.

```python
# ListDeploymentEventsPaginator usage example

from types_aiobotocore_launch_wizard.paginator import ListDeploymentEventsPaginator

def get_list_deployment_events_paginator() -> ListDeploymentEventsPaginator:
    return client.get_paginator("list_deployment_events"))
```

- [ListDeploymentEventsPaginator](./paginators.md#listdeploymenteventspaginator)
- [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
- [ListWorkloadDeploymentPatternsPaginator](./paginators.md#listworkloaddeploymentpatternspaginator)
- [ListWorkloadsPaginator](./paginators.md#listworkloadspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DeploymentFilterKeyType usage example

from types_aiobotocore_launch_wizard.literals import DeploymentFilterKeyType

def get_value() -> DeploymentFilterKeyType:
    return "DEPLOYMENT_STATUS"
```

- [DeploymentFilterKeyType](./literals.md#deploymentfilterkeytype)
- [DeploymentStatusType](./literals.md#deploymentstatustype)
- [EventStatusType](./literals.md#eventstatustype)
- [ListDeploymentEventsPaginatorName](./literals.md#listdeploymenteventspaginatorname)
- [ListDeploymentsPaginatorName](./literals.md#listdeploymentspaginatorname)
- [ListWorkloadDeploymentPatternsPaginatorName](./literals.md#listworkloaddeploymentpatternspaginatorname)
- [ListWorkloadsPaginatorName](./literals.md#listworkloadspaginatorname)
- [WorkloadDeploymentPatternStatusType](./literals.md#workloaddeploymentpatternstatustype)
- [WorkloadStatusType](./literals.md#workloadstatustype)
- [LaunchWizardServiceName](./literals.md#launchwizardservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CreateDeploymentInputRequestTypeDef](./type_defs.md#createdeploymentinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteDeploymentInputRequestTypeDef](./type_defs.md#deletedeploymentinputrequesttypedef)
- [DeploymentConditionalFieldTypeDef](./type_defs.md#deploymentconditionalfieldtypedef)
- [DeploymentDataSummaryTypeDef](./type_defs.md#deploymentdatasummarytypedef)
- [DeploymentDataTypeDef](./type_defs.md#deploymentdatatypedef)
- [DeploymentEventDataSummaryTypeDef](./type_defs.md#deploymenteventdatasummarytypedef)
- [DeploymentFilterTypeDef](./type_defs.md#deploymentfiltertypedef)
- [GetDeploymentInputRequestTypeDef](./type_defs.md#getdeploymentinputrequesttypedef)
- [GetWorkloadDeploymentPatternInputRequestTypeDef](./type_defs.md#getworkloaddeploymentpatterninputrequesttypedef)
- [GetWorkloadInputRequestTypeDef](./type_defs.md#getworkloadinputrequesttypedef)
- [WorkloadDataTypeDef](./type_defs.md#workloaddatatypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDeploymentEventsInputRequestTypeDef](./type_defs.md#listdeploymenteventsinputrequesttypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ListWorkloadDeploymentPatternsInputRequestTypeDef](./type_defs.md#listworkloaddeploymentpatternsinputrequesttypedef)
- [WorkloadDeploymentPatternDataSummaryTypeDef](./type_defs.md#workloaddeploymentpatterndatasummarytypedef)
- [ListWorkloadsInputRequestTypeDef](./type_defs.md#listworkloadsinputrequesttypedef)
- [WorkloadDataSummaryTypeDef](./type_defs.md#workloaddatasummarytypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [CreateDeploymentOutputTypeDef](./type_defs.md#createdeploymentoutputtypedef)
- [DeleteDeploymentOutputTypeDef](./type_defs.md#deletedeploymentoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [DeploymentSpecificationsFieldTypeDef](./type_defs.md#deploymentspecificationsfieldtypedef)
- [ListDeploymentsOutputTypeDef](./type_defs.md#listdeploymentsoutputtypedef)
- [GetDeploymentOutputTypeDef](./type_defs.md#getdeploymentoutputtypedef)
- [ListDeploymentEventsOutputTypeDef](./type_defs.md#listdeploymenteventsoutputtypedef)
- [ListDeploymentsInputRequestTypeDef](./type_defs.md#listdeploymentsinputrequesttypedef)
- [GetWorkloadOutputTypeDef](./type_defs.md#getworkloadoutputtypedef)
- [ListDeploymentEventsInputListDeploymentEventsPaginateTypeDef](./type_defs.md#listdeploymenteventsinputlistdeploymenteventspaginatetypedef)
- [ListDeploymentsInputListDeploymentsPaginateTypeDef](./type_defs.md#listdeploymentsinputlistdeploymentspaginatetypedef)
- [ListWorkloadDeploymentPatternsInputListWorkloadDeploymentPatternsPaginateTypeDef](./type_defs.md#listworkloaddeploymentpatternsinputlistworkloaddeploymentpatternspaginatetypedef)
- [ListWorkloadsInputListWorkloadsPaginateTypeDef](./type_defs.md#listworkloadsinputlistworkloadspaginatetypedef)
- [ListWorkloadDeploymentPatternsOutputTypeDef](./type_defs.md#listworkloaddeploymentpatternsoutputtypedef)
- [ListWorkloadsOutputTypeDef](./type_defs.md#listworkloadsoutputtypedef)
- [WorkloadDeploymentPatternDataTypeDef](./type_defs.md#workloaddeploymentpatterndatatypedef)
- [GetWorkloadDeploymentPatternOutputTypeDef](./type_defs.md#getworkloaddeploymentpatternoutputtypedef)

