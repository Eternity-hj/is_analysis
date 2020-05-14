## 接口：setPassword   [返回](README.md)
用例：[修改密码](用例/修改密码.md)
- 功能：修改或者设置用户密码
- 权限：学生或者老师
- API请求地址：https://testmanage.com/v1/api/logout
- 请求方式：POST
- 请求实例：
<pre>
<code>
{
"id":"2017104142040",
"password":"q22323s"
}
</code>
</pre>
- 请求参数说明：

|参数名称|说明|
|-------|------|
|id|用户的ID号，学生的学号，老师工号。|
|password|用户的密码。不能为空且经过加密|

- 返回实例：
<pre>
<code>
{
"status":"true",
"info": "null"
}
</code>
</pre>
- 返回参数说明：

|参数名称|说明|
|-------|------|
|status|boolean类型，true表示修改操作正确，false表示修改操作错误|
|info|返回结果说明信息|