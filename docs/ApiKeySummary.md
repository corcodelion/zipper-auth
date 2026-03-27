

# ApiKeySummary


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** |  |  [optional] |
|**apiKeyPrefix** | **String** |  |  [optional] |
|**label** | **String** |  |  [optional] |
|**scopes** | **Set&lt;String&gt;** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |
|**lastUsedAt** | **OffsetDateTime** |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| ACTIVE | &quot;ACTIVE&quot; |
| REVOKED | &quot;REVOKED&quot; |



