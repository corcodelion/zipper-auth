

# MerchantSummary


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** |  |  [optional] |
|**businessName** | **String** |  |  [optional] |
|**email** | **String** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**origin** | [**OriginEnum**](#OriginEnum) |  |  [optional] |
|**partnerId** | **UUID** |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| PENDING_ACTIVATION | &quot;PENDING_ACTIVATION&quot; |
| PENDING_PASSWORD_SETUP | &quot;PENDING_PASSWORD_SETUP&quot; |
| ACTIVE | &quot;ACTIVE&quot; |
| SUSPENDED | &quot;SUSPENDED&quot; |



## Enum: OriginEnum

| Name | Value |
|---- | -----|
| SELF | &quot;SELF&quot; |
| PARTNER_API | &quot;PARTNER_API&quot; |
| ADMIN | &quot;ADMIN&quot; |



