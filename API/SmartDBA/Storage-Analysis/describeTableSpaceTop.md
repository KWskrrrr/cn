# describeTableSpaceTop


## 描述
表空间Top 10

## 请求方式
GET

## 请求地址
https://smartdba.jdcloud-api.com/v2/regions/{regionId}/instance/{instanceGid}/tableSpaceTop

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**regionId**|String|True| |地域代码，取值范围参见[《各地域及可用区对照表》](../Enum-Definitions/Regions-AZ.md)|
|**instanceGid**|String|True| |RDS 实例ID，唯一标识一个RDS实例。|

## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**sortField**|String|False| |排序字段：表空间(totalSize)、表数据空间(dataSize)、索引空间(idxSize)、碎片率(fragment)、行数(dataRows)|
|**sortType**|String|False| |排序类型，desc 降序、asc 升序，默认降序|


## 返回参数
|名称|类型|描述|
|---|---|---|
|**result**|[Result](#result)| |
|**requestId**|String|请求id|
|**error**|[Error](#error)|Error信息|

### <div id="Error">Error</div>
|名称|类型|描述|
|---|---|---|
|**errorInfo**|[ErrorInfo](#errorinfo)| |
### <div id="ErrorInfo">ErrorInfo</div>
|名称|类型|描述|
|---|---|---|
|**code**|Integer|错误码，默认正确为0|
|**message**|String|错误信息，默认为""|
|**status**|String|错误状态信息，默认为""|
### <div id="Result">Result</div>
|名称|类型|描述|
|---|---|---|
|**data**|[TableStorageInfo[]](#tablestorageinfo)|表空间信息Top 列表|
### <div id="TableStorageInfo">TableStorageInfo</div>
|名称|类型|描述|
|---|---|---|
|**tableName**|String|表名|
|**dbName**|String|数据库名|
|**engine**|String|引擎|
|**totalSize**|String|表空间大小|
|**percentage**|String|表空间占比|
|**dataSize**|String|数据空间|
|**idxSize**|String|索引空间|
|**fragment**|String|碎片率|
|**dataRows**|Integer|表行数|

## 返回码
|返回码|描述|
|---|---|
|**200**|OK|
