# updatePersonalSql


## 描述
更新收藏sql

## 请求方式
POST

## 请求地址
https://dms.jdcloud-api.com/v1/regions/{regionId}/personalSql:update

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**regionId**|String|True| |地域代码，取值范围参见[《各地域及可用区对照表》](../Enum-Definitions/Regions-AZ.md)|

## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**id**|Integer|True| |主键id|
|**hint**|String|True| |sql备注|
|**sqlStr**|String|True| |sql内容|


## 返回参数
无


## 返回码
|返回码|描述|
|---|---|
|**200**|OK|
