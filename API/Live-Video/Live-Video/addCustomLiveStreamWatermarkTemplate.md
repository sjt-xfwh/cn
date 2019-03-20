# addCustomLiveStreamWatermarkTemplate


## 描述
添加直播水印模板

## 请求方式
POST

## 请求地址
https://live.jdcloud-api.com/v1/watermarkCustoms:template


## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**offsetX**|Integer|True| |x轴偏移量:<br>  - 单位：像素<br>|
|**offsetY**|Integer|True| |y轴偏移量:<br>  - 单位：像素<br>|
|**width**|Integer|True| |水印宽度:<br>  - 取值: [0,1920]<br>|
|**height**|Integer|True| |水印高度:<br>  - 取值: [0,1920]<br>|
|**template**|String|True| |水印模板自定义名称:<br>  - 标准质量模板：sd、hd、hsd<br>  - 自定义模板: 枚举类型校验，忽略大小写，自动删除空格,<br>              取值要求：数字、大小写字母或短横线("-"),<br>              首尾不能有特殊字符("-")<br>  - <b>注意: 不能与标准的转码模板和已定义命名重复</b><br>|
|**url**|String|True| |水印地址:<br>  - 以 http开头，可访问地址<br>|


## 返回参数
|名称|类型|描述|
|---|---|---|
|**requestId**|String|ruquestId|


## 返回码
|返回码|描述|
|---|---|
|**200**|OK|
|**400**|Invalid parameter|
|**401**|Authentication failed|
|**404**|Not found|
|**500**|Internal server error|
|**503**|Service unavailable|