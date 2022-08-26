# Paginators

> [Index](../README.md) > [ConfigService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ConfigService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
    type annotations stubs module [types-aiobotocore-config](https://pypi.org/project/types-aiobotocore-config/).

## DescribeAggregateComplianceByConfigRulesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_aggregate_compliance_by_config_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConfigRules)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeAggregateComplianceByConfigRulesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeAggregateComplianceByConfigRulesPaginator = client.get_paginator("describe_aggregate_compliance_by_config_rules")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAggregateComplianceByConfigRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeAggregateComplianceByConfigRulesPaginator](./paginators.md#describeaggregatecompliancebyconfigrulespaginator)
3. item: [:material-code-braces: DescribeAggregateComplianceByConfigRulesResponseTypeDef](./type_defs.md#describeaggregatecompliancebyconfigrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAggregateComplianceByConfigRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConfigurationAggregatorName: str,
    Filters: ConfigRuleComplianceFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeAggregateComplianceByConfigRulesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ConfigRuleComplianceFiltersTypeDef](./type_defs.md#configrulecompliancefilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeAggregateComplianceByConfigRulesResponseTypeDef](./type_defs.md#describeaggregatecompliancebyconfigrulesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef](./type_defs.md#describeaggregatecompliancebyconfigrulesrequestdescribeaggregatecompliancebyconfigrulespaginatetypedef) 
## DescribeAggregateComplianceByConformancePacksPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_aggregate_compliance_by_conformance_packs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConformancePacks)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeAggregateComplianceByConformancePacksPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeAggregateComplianceByConformancePacksPaginator = client.get_paginator("describe_aggregate_compliance_by_conformance_packs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAggregateComplianceByConformancePacksResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeAggregateComplianceByConformancePacksPaginator](./paginators.md#describeaggregatecompliancebyconformancepackspaginator)
3. item: [:material-code-braces: DescribeAggregateComplianceByConformancePacksResponseTypeDef](./type_defs.md#describeaggregatecompliancebyconformancepacksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAggregateComplianceByConformancePacksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConfigurationAggregatorName: str,
    Filters: AggregateConformancePackComplianceFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeAggregateComplianceByConformancePacksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AggregateConformancePackComplianceFiltersTypeDef](./type_defs.md#aggregateconformancepackcompliancefilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeAggregateComplianceByConformancePacksResponseTypeDef](./type_defs.md#describeaggregatecompliancebyconformancepacksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef](./type_defs.md#describeaggregatecompliancebyconformancepacksrequestdescribeaggregatecompliancebyconformancepackspaginatetypedef) 
## DescribeAggregationAuthorizationsPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_aggregation_authorizations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregationAuthorizations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeAggregationAuthorizationsPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeAggregationAuthorizationsPaginator = client.get_paginator("describe_aggregation_authorizations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAggregationAuthorizationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeAggregationAuthorizationsPaginator](./paginators.md#describeaggregationauthorizationspaginator)
3. item: [:material-code-braces: DescribeAggregationAuthorizationsResponseTypeDef](./type_defs.md#describeaggregationauthorizationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAggregationAuthorizationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeAggregationAuthorizationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAggregationAuthorizationsResponseTypeDef](./type_defs.md#describeaggregationauthorizationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef](./type_defs.md#describeaggregationauthorizationsrequestdescribeaggregationauthorizationspaginatetypedef) 
## DescribeComplianceByConfigRulePaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_compliance_by_config_rule")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByConfigRule)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeComplianceByConfigRulePaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeComplianceByConfigRulePaginator = client.get_paginator("describe_compliance_by_config_rule")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeComplianceByConfigRuleResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeComplianceByConfigRulePaginator](./paginators.md#describecompliancebyconfigrulepaginator)
3. item: [:material-code-braces: DescribeComplianceByConfigRuleResponseTypeDef](./type_defs.md#describecompliancebyconfigruleresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeComplianceByConfigRulePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConfigRuleNames: Sequence[str] = ...,
    ComplianceTypes: Sequence[ComplianceTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeComplianceByConfigRuleResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeComplianceByConfigRuleResponseTypeDef](./type_defs.md#describecompliancebyconfigruleresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef = {  # (1)
    "ConfigRuleNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef](./type_defs.md#describecompliancebyconfigrulerequestdescribecompliancebyconfigrulepaginatetypedef) 
## DescribeComplianceByResourcePaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_compliance_by_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByResource)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeComplianceByResourcePaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeComplianceByResourcePaginator = client.get_paginator("describe_compliance_by_resource")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeComplianceByResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeComplianceByResourcePaginator](./paginators.md#describecompliancebyresourcepaginator)
3. item: [:material-code-braces: DescribeComplianceByResourceResponseTypeDef](./type_defs.md#describecompliancebyresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeComplianceByResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceType: str = ...,
    ResourceId: str = ...,
    ComplianceTypes: Sequence[ComplianceTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeComplianceByResourceResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeComplianceByResourceResponseTypeDef](./type_defs.md#describecompliancebyresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef = {  # (1)
    "ResourceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef](./type_defs.md#describecompliancebyresourcerequestdescribecompliancebyresourcepaginatetypedef) 
## DescribeConfigRuleEvaluationStatusPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_config_rule_evaluation_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRuleEvaluationStatus)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeConfigRuleEvaluationStatusPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeConfigRuleEvaluationStatusPaginator = client.get_paginator("describe_config_rule_evaluation_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConfigRuleEvaluationStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeConfigRuleEvaluationStatusPaginator](./paginators.md#describeconfigruleevaluationstatuspaginator)
3. item: [:material-code-braces: DescribeConfigRuleEvaluationStatusResponseTypeDef](./type_defs.md#describeconfigruleevaluationstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConfigRuleEvaluationStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConfigRuleNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeConfigRuleEvaluationStatusResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeConfigRuleEvaluationStatusResponseTypeDef](./type_defs.md#describeconfigruleevaluationstatusresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef = {  # (1)
    "ConfigRuleNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef](./type_defs.md#describeconfigruleevaluationstatusrequestdescribeconfigruleevaluationstatuspaginatetypedef) 
## DescribeConfigRulesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_config_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRules)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeConfigRulesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeConfigRulesPaginator = client.get_paginator("describe_config_rules")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConfigRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeConfigRulesPaginator](./paginators.md#describeconfigrulespaginator)
3. item: [:material-code-braces: DescribeConfigRulesResponseTypeDef](./type_defs.md#describeconfigrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConfigRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConfigRuleNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeConfigRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeConfigRulesResponseTypeDef](./type_defs.md#describeconfigrulesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef = {  # (1)
    "ConfigRuleNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef](./type_defs.md#describeconfigrulesrequestdescribeconfigrulespaginatetypedef) 
## DescribeConfigurationAggregatorSourcesStatusPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_configuration_aggregator_sources_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregatorSourcesStatus)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeConfigurationAggregatorSourcesStatusPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeConfigurationAggregatorSourcesStatusPaginator = client.get_paginator("describe_configuration_aggregator_sources_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConfigurationAggregatorSourcesStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeConfigurationAggregatorSourcesStatusPaginator](./paginators.md#describeconfigurationaggregatorsourcesstatuspaginator)
3. item: [:material-code-braces: DescribeConfigurationAggregatorSourcesStatusResponseTypeDef](./type_defs.md#describeconfigurationaggregatorsourcesstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConfigurationAggregatorSourcesStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConfigurationAggregatorName: str,
    UpdateStatus: Sequence[AggregatedSourceStatusTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeConfigurationAggregatorSourcesStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AggregatedSourceStatusTypeType](./literals.md#aggregatedsourcestatustypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeConfigurationAggregatorSourcesStatusResponseTypeDef](./type_defs.md#describeconfigurationaggregatorsourcesstatusresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef](./type_defs.md#describeconfigurationaggregatorsourcesstatusrequestdescribeconfigurationaggregatorsourcesstatuspaginatetypedef) 
## DescribeConfigurationAggregatorsPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_configuration_aggregators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregators)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeConfigurationAggregatorsPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeConfigurationAggregatorsPaginator = client.get_paginator("describe_configuration_aggregators")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConfigurationAggregatorsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeConfigurationAggregatorsPaginator](./paginators.md#describeconfigurationaggregatorspaginator)
3. item: [:material-code-braces: DescribeConfigurationAggregatorsResponseTypeDef](./type_defs.md#describeconfigurationaggregatorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConfigurationAggregatorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConfigurationAggregatorNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeConfigurationAggregatorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeConfigurationAggregatorsResponseTypeDef](./type_defs.md#describeconfigurationaggregatorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef = {  # (1)
    "ConfigurationAggregatorNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef](./type_defs.md#describeconfigurationaggregatorsrequestdescribeconfigurationaggregatorspaginatetypedef) 
## DescribeConformancePackStatusPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_conformance_pack_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePackStatus)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeConformancePackStatusPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeConformancePackStatusPaginator = client.get_paginator("describe_conformance_pack_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConformancePackStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeConformancePackStatusPaginator](./paginators.md#describeconformancepackstatuspaginator)
3. item: [:material-code-braces: DescribeConformancePackStatusResponseTypeDef](./type_defs.md#describeconformancepackstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConformancePackStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConformancePackNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeConformancePackStatusResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeConformancePackStatusResponseTypeDef](./type_defs.md#describeconformancepackstatusresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef = {  # (1)
    "ConformancePackNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef](./type_defs.md#describeconformancepackstatusrequestdescribeconformancepackstatuspaginatetypedef) 
## DescribeConformancePacksPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_conformance_packs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePacks)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeConformancePacksPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeConformancePacksPaginator = client.get_paginator("describe_conformance_packs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConformancePacksResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeConformancePacksPaginator](./paginators.md#describeconformancepackspaginator)
3. item: [:material-code-braces: DescribeConformancePacksResponseTypeDef](./type_defs.md#describeconformancepacksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConformancePacksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConformancePackNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeConformancePacksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeConformancePacksResponseTypeDef](./type_defs.md#describeconformancepacksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef = {  # (1)
    "ConformancePackNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef](./type_defs.md#describeconformancepacksrequestdescribeconformancepackspaginatetypedef) 
## DescribeOrganizationConfigRuleStatusesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_organization_config_rule_statuses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRuleStatuses)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeOrganizationConfigRuleStatusesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeOrganizationConfigRuleStatusesPaginator = client.get_paginator("describe_organization_config_rule_statuses")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeOrganizationConfigRuleStatusesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeOrganizationConfigRuleStatusesPaginator](./paginators.md#describeorganizationconfigrulestatusespaginator)
3. item: [:material-code-braces: DescribeOrganizationConfigRuleStatusesResponseTypeDef](./type_defs.md#describeorganizationconfigrulestatusesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrganizationConfigRuleStatusesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationConfigRuleNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeOrganizationConfigRuleStatusesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeOrganizationConfigRuleStatusesResponseTypeDef](./type_defs.md#describeorganizationconfigrulestatusesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef = {  # (1)
    "OrganizationConfigRuleNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef](./type_defs.md#describeorganizationconfigrulestatusesrequestdescribeorganizationconfigrulestatusespaginatetypedef) 
## DescribeOrganizationConfigRulesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_organization_config_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRules)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeOrganizationConfigRulesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeOrganizationConfigRulesPaginator = client.get_paginator("describe_organization_config_rules")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeOrganizationConfigRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeOrganizationConfigRulesPaginator](./paginators.md#describeorganizationconfigrulespaginator)
3. item: [:material-code-braces: DescribeOrganizationConfigRulesResponseTypeDef](./type_defs.md#describeorganizationconfigrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrganizationConfigRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationConfigRuleNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeOrganizationConfigRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeOrganizationConfigRulesResponseTypeDef](./type_defs.md#describeorganizationconfigrulesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef = {  # (1)
    "OrganizationConfigRuleNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef](./type_defs.md#describeorganizationconfigrulesrequestdescribeorganizationconfigrulespaginatetypedef) 
## DescribeOrganizationConformancePackStatusesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_organization_conformance_pack_statuses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePackStatuses)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeOrganizationConformancePackStatusesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeOrganizationConformancePackStatusesPaginator = client.get_paginator("describe_organization_conformance_pack_statuses")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeOrganizationConformancePackStatusesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeOrganizationConformancePackStatusesPaginator](./paginators.md#describeorganizationconformancepackstatusespaginator)
3. item: [:material-code-braces: DescribeOrganizationConformancePackStatusesResponseTypeDef](./type_defs.md#describeorganizationconformancepackstatusesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrganizationConformancePackStatusesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationConformancePackNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeOrganizationConformancePackStatusesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeOrganizationConformancePackStatusesResponseTypeDef](./type_defs.md#describeorganizationconformancepackstatusesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef = {  # (1)
    "OrganizationConformancePackNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef](./type_defs.md#describeorganizationconformancepackstatusesrequestdescribeorganizationconformancepackstatusespaginatetypedef) 
## DescribeOrganizationConformancePacksPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_organization_conformance_packs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePacks)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeOrganizationConformancePacksPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeOrganizationConformancePacksPaginator = client.get_paginator("describe_organization_conformance_packs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeOrganizationConformancePacksResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeOrganizationConformancePacksPaginator](./paginators.md#describeorganizationconformancepackspaginator)
3. item: [:material-code-braces: DescribeOrganizationConformancePacksResponseTypeDef](./type_defs.md#describeorganizationconformancepacksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrganizationConformancePacksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationConformancePackNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeOrganizationConformancePacksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeOrganizationConformancePacksResponseTypeDef](./type_defs.md#describeorganizationconformancepacksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef = {  # (1)
    "OrganizationConformancePackNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef](./type_defs.md#describeorganizationconformancepacksrequestdescribeorganizationconformancepackspaginatetypedef) 
## DescribePendingAggregationRequestsPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_pending_aggregation_requests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribePendingAggregationRequests)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribePendingAggregationRequestsPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribePendingAggregationRequestsPaginator = client.get_paginator("describe_pending_aggregation_requests")  # (2)
    async for item in paginator.paginate(...):
        item: DescribePendingAggregationRequestsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribePendingAggregationRequestsPaginator](./paginators.md#describependingaggregationrequestspaginator)
3. item: [:material-code-braces: DescribePendingAggregationRequestsResponseTypeDef](./type_defs.md#describependingaggregationrequestsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribePendingAggregationRequestsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribePendingAggregationRequestsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribePendingAggregationRequestsResponseTypeDef](./type_defs.md#describependingaggregationrequestsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef](./type_defs.md#describependingaggregationrequestsrequestdescribependingaggregationrequestspaginatetypedef) 
## DescribeRemediationExecutionStatusPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_remediation_execution_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRemediationExecutionStatus)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeRemediationExecutionStatusPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeRemediationExecutionStatusPaginator = client.get_paginator("describe_remediation_execution_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRemediationExecutionStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeRemediationExecutionStatusPaginator](./paginators.md#describeremediationexecutionstatuspaginator)
3. item: [:material-code-braces: DescribeRemediationExecutionStatusResponseTypeDef](./type_defs.md#describeremediationexecutionstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRemediationExecutionStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConfigRuleName: str,
    ResourceKeys: Sequence[ResourceKeyTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeRemediationExecutionStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ResourceKeyTypeDef](./type_defs.md#resourcekeytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeRemediationExecutionStatusResponseTypeDef](./type_defs.md#describeremediationexecutionstatusresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = {  # (1)
    "ConfigRuleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef](./type_defs.md#describeremediationexecutionstatusrequestdescriberemediationexecutionstatuspaginatetypedef) 
## DescribeRetentionConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_retention_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRetentionConfigurations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeRetentionConfigurationsPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeRetentionConfigurationsPaginator = client.get_paginator("describe_retention_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRetentionConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeRetentionConfigurationsPaginator](./paginators.md#describeretentionconfigurationspaginator)
3. item: [:material-code-braces: DescribeRetentionConfigurationsResponseTypeDef](./type_defs.md#describeretentionconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRetentionConfigurationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RetentionConfigurationNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeRetentionConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRetentionConfigurationsResponseTypeDef](./type_defs.md#describeretentionconfigurationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef = {  # (1)
    "RetentionConfigurationNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef](./type_defs.md#describeretentionconfigurationsrequestdescriberetentionconfigurationspaginatetypedef) 
## GetAggregateComplianceDetailsByConfigRulePaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_aggregate_compliance_details_by_config_rule")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetAggregateComplianceDetailsByConfigRule)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetAggregateComplianceDetailsByConfigRulePaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetAggregateComplianceDetailsByConfigRulePaginator = client.get_paginator("get_aggregate_compliance_details_by_config_rule")  # (2)
    async for item in paginator.paginate(...):
        item: GetAggregateComplianceDetailsByConfigRuleResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetAggregateComplianceDetailsByConfigRulePaginator](./paginators.md#getaggregatecompliancedetailsbyconfigrulepaginator)
3. item: [:material-code-braces: GetAggregateComplianceDetailsByConfigRuleResponseTypeDef](./type_defs.md#getaggregatecompliancedetailsbyconfigruleresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetAggregateComplianceDetailsByConfigRulePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConfigurationAggregatorName: str,
    ConfigRuleName: str,
    AccountId: str,
    AwsRegion: str,
    ComplianceType: ComplianceTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetAggregateComplianceDetailsByConfigRuleResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetAggregateComplianceDetailsByConfigRuleResponseTypeDef](./type_defs.md#getaggregatecompliancedetailsbyconfigruleresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
    "ConfigRuleName": ...,
    "AccountId": ...,
    "AwsRegion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef](./type_defs.md#getaggregatecompliancedetailsbyconfigrulerequestgetaggregatecompliancedetailsbyconfigrulepaginatetypedef) 
## GetComplianceDetailsByConfigRulePaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_compliance_details_by_config_rule")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByConfigRule)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetComplianceDetailsByConfigRulePaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetComplianceDetailsByConfigRulePaginator = client.get_paginator("get_compliance_details_by_config_rule")  # (2)
    async for item in paginator.paginate(...):
        item: GetComplianceDetailsByConfigRuleResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetComplianceDetailsByConfigRulePaginator](./paginators.md#getcompliancedetailsbyconfigrulepaginator)
3. item: [:material-code-braces: GetComplianceDetailsByConfigRuleResponseTypeDef](./type_defs.md#getcompliancedetailsbyconfigruleresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetComplianceDetailsByConfigRulePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConfigRuleName: str,
    ComplianceTypes: Sequence[ComplianceTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetComplianceDetailsByConfigRuleResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetComplianceDetailsByConfigRuleResponseTypeDef](./type_defs.md#getcompliancedetailsbyconfigruleresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = {  # (1)
    "ConfigRuleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef](./type_defs.md#getcompliancedetailsbyconfigrulerequestgetcompliancedetailsbyconfigrulepaginatetypedef) 
## GetComplianceDetailsByResourcePaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_compliance_details_by_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByResource)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetComplianceDetailsByResourcePaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetComplianceDetailsByResourcePaginator = client.get_paginator("get_compliance_details_by_resource")  # (2)
    async for item in paginator.paginate(...):
        item: GetComplianceDetailsByResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetComplianceDetailsByResourcePaginator](./paginators.md#getcompliancedetailsbyresourcepaginator)
3. item: [:material-code-braces: GetComplianceDetailsByResourceResponseTypeDef](./type_defs.md#getcompliancedetailsbyresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetComplianceDetailsByResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceType: str,
    ResourceId: str,
    ComplianceTypes: Sequence[ComplianceTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetComplianceDetailsByResourceResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetComplianceDetailsByResourceResponseTypeDef](./type_defs.md#getcompliancedetailsbyresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef = {  # (1)
    "ResourceType": ...,
    "ResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef](./type_defs.md#getcompliancedetailsbyresourcerequestgetcompliancedetailsbyresourcepaginatetypedef) 
## GetConformancePackComplianceSummaryPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_conformance_pack_compliance_summary")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetConformancePackComplianceSummary)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetConformancePackComplianceSummaryPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetConformancePackComplianceSummaryPaginator = client.get_paginator("get_conformance_pack_compliance_summary")  # (2)
    async for item in paginator.paginate(...):
        item: GetConformancePackComplianceSummaryResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetConformancePackComplianceSummaryPaginator](./paginators.md#getconformancepackcompliancesummarypaginator)
3. item: [:material-code-braces: GetConformancePackComplianceSummaryResponseTypeDef](./type_defs.md#getconformancepackcompliancesummaryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetConformancePackComplianceSummaryPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConformancePackNames: Sequence[str],
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetConformancePackComplianceSummaryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetConformancePackComplianceSummaryResponseTypeDef](./type_defs.md#getconformancepackcompliancesummaryresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = {  # (1)
    "ConformancePackNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef](./type_defs.md#getconformancepackcompliancesummaryrequestgetconformancepackcompliancesummarypaginatetypedef) 
## GetOrganizationConfigRuleDetailedStatusPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_organization_config_rule_detailed_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConfigRuleDetailedStatus)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetOrganizationConfigRuleDetailedStatusPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetOrganizationConfigRuleDetailedStatusPaginator = client.get_paginator("get_organization_config_rule_detailed_status")  # (2)
    async for item in paginator.paginate(...):
        item: GetOrganizationConfigRuleDetailedStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetOrganizationConfigRuleDetailedStatusPaginator](./paginators.md#getorganizationconfigruledetailedstatuspaginator)
3. item: [:material-code-braces: GetOrganizationConfigRuleDetailedStatusResponseTypeDef](./type_defs.md#getorganizationconfigruledetailedstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetOrganizationConfigRuleDetailedStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationConfigRuleName: str,
    Filters: StatusDetailFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetOrganizationConfigRuleDetailedStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: StatusDetailFiltersTypeDef](./type_defs.md#statusdetailfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetOrganizationConfigRuleDetailedStatusResponseTypeDef](./type_defs.md#getorganizationconfigruledetailedstatusresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef = {  # (1)
    "OrganizationConfigRuleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef](./type_defs.md#getorganizationconfigruledetailedstatusrequestgetorganizationconfigruledetailedstatuspaginatetypedef) 
## GetOrganizationConformancePackDetailedStatusPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_organization_conformance_pack_detailed_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConformancePackDetailedStatus)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetOrganizationConformancePackDetailedStatusPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetOrganizationConformancePackDetailedStatusPaginator = client.get_paginator("get_organization_conformance_pack_detailed_status")  # (2)
    async for item in paginator.paginate(...):
        item: GetOrganizationConformancePackDetailedStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetOrganizationConformancePackDetailedStatusPaginator](./paginators.md#getorganizationconformancepackdetailedstatuspaginator)
3. item: [:material-code-braces: GetOrganizationConformancePackDetailedStatusResponseTypeDef](./type_defs.md#getorganizationconformancepackdetailedstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetOrganizationConformancePackDetailedStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationConformancePackName: str,
    Filters: OrganizationResourceDetailedStatusFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetOrganizationConformancePackDetailedStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: OrganizationResourceDetailedStatusFiltersTypeDef](./type_defs.md#organizationresourcedetailedstatusfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetOrganizationConformancePackDetailedStatusResponseTypeDef](./type_defs.md#getorganizationconformancepackdetailedstatusresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef = {  # (1)
    "OrganizationConformancePackName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef](./type_defs.md#getorganizationconformancepackdetailedstatusrequestgetorganizationconformancepackdetailedstatuspaginatetypedef) 
## GetResourceConfigHistoryPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_resource_config_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetResourceConfigHistory)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetResourceConfigHistoryPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetResourceConfigHistoryPaginator = client.get_paginator("get_resource_config_history")  # (2)
    async for item in paginator.paginate(...):
        item: GetResourceConfigHistoryResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetResourceConfigHistoryPaginator](./paginators.md#getresourceconfighistorypaginator)
3. item: [:material-code-braces: GetResourceConfigHistoryResponseTypeDef](./type_defs.md#getresourceconfighistoryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetResourceConfigHistoryPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    resourceType: ResourceTypeType,  # (1)
    resourceId: str,
    laterTime: Union[datetime, str] = ...,
    earlierTime: Union[datetime, str] = ...,
    chronologicalOrder: ChronologicalOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[GetResourceConfigHistoryResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ChronologicalOrderType](./literals.md#chronologicalordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetResourceConfigHistoryResponseTypeDef](./type_defs.md#getresourceconfighistoryresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = {  # (1)
    "resourceType": ...,
    "resourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef](./type_defs.md#getresourceconfighistoryrequestgetresourceconfighistorypaginatetypedef) 
## ListAggregateDiscoveredResourcesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("list_aggregate_discovered_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListAggregateDiscoveredResources)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import ListAggregateDiscoveredResourcesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: ListAggregateDiscoveredResourcesPaginator = client.get_paginator("list_aggregate_discovered_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListAggregateDiscoveredResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [ListAggregateDiscoveredResourcesPaginator](./paginators.md#listaggregatediscoveredresourcespaginator)
3. item: [:material-code-braces: ListAggregateDiscoveredResourcesResponseTypeDef](./type_defs.md#listaggregatediscoveredresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAggregateDiscoveredResourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConfigurationAggregatorName: str,
    ResourceType: ResourceTypeType,  # (1)
    Filters: ResourceFiltersTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListAggregateDiscoveredResourcesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ResourceFiltersTypeDef](./type_defs.md#resourcefilterstypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListAggregateDiscoveredResourcesResponseTypeDef](./type_defs.md#listaggregatediscoveredresourcesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
    "ResourceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef](./type_defs.md#listaggregatediscoveredresourcesrequestlistaggregatediscoveredresourcespaginatetypedef) 
## ListDiscoveredResourcesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("list_discovered_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListDiscoveredResources)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import ListDiscoveredResourcesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: ListDiscoveredResourcesPaginator = client.get_paginator("list_discovered_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListDiscoveredResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [ListDiscoveredResourcesPaginator](./paginators.md#listdiscoveredresourcespaginator)
3. item: [:material-code-braces: ListDiscoveredResourcesResponseTypeDef](./type_defs.md#listdiscoveredresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDiscoveredResourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    resourceType: ResourceTypeType,  # (1)
    resourceIds: Sequence[str] = ...,
    resourceName: str = ...,
    includeDeletedResources: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDiscoveredResourcesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDiscoveredResourcesResponseTypeDef](./type_defs.md#listdiscoveredresourcesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = {  # (1)
    "resourceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef](./type_defs.md#listdiscoveredresourcesrequestlistdiscoveredresourcespaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListTagsForResource)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourcerequestlisttagsforresourcepaginatetypedef) 
## SelectAggregateResourceConfigPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("select_aggregate_resource_config")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectAggregateResourceConfig)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import SelectAggregateResourceConfigPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: SelectAggregateResourceConfigPaginator = client.get_paginator("select_aggregate_resource_config")  # (2)
    async for item in paginator.paginate(...):
        item: SelectAggregateResourceConfigResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [SelectAggregateResourceConfigPaginator](./paginators.md#selectaggregateresourceconfigpaginator)
3. item: [:material-code-braces: SelectAggregateResourceConfigResponseTypeDef](./type_defs.md#selectaggregateresourceconfigresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SelectAggregateResourceConfigPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Expression: str,
    ConfigurationAggregatorName: str,
    MaxResults: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[SelectAggregateResourceConfigResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SelectAggregateResourceConfigResponseTypeDef](./type_defs.md#selectaggregateresourceconfigresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = {  # (1)
    "Expression": ...,
    "ConfigurationAggregatorName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef](./type_defs.md#selectaggregateresourceconfigrequestselectaggregateresourceconfigpaginatetypedef) 
## SelectResourceConfigPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("select_resource_config")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectResourceConfig)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import SelectResourceConfigPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: SelectResourceConfigPaginator = client.get_paginator("select_resource_config")  # (2)
    async for item in paginator.paginate(...):
        item: SelectResourceConfigResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [SelectResourceConfigPaginator](./paginators.md#selectresourceconfigpaginator)
3. item: [:material-code-braces: SelectResourceConfigResponseTypeDef](./type_defs.md#selectresourceconfigresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SelectResourceConfigPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Expression: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[SelectResourceConfigResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SelectResourceConfigResponseTypeDef](./type_defs.md#selectresourceconfigresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = {  # (1)
    "Expression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef](./type_defs.md#selectresourceconfigrequestselectresourceconfigpaginatetypedef) 
