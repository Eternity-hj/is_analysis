## 接口：getUserInfo   [返回](README.md)
用例：[修改用户信息](用例/修改个人信息.md)
- 功能：获取用户的所有信息
- 权限：用于老师和学生查看自己的信息，必须先登录，同时不能查看本人的信息
- API请求地址：https://testmanage.com/v1/api/setUserInfo/<user_id>
- 请求方式：POST
- 请求实例：
<pre>
<code>
{
"id":"201710414204",
"github_username":"honora"
}
</code>
</pre>
- 请求参数说明：

|参数名称|说明|
|-------|------|
|user_id|用户的ID号，对应表USER.USER_ID的值，学生的学号，老师工号。|
|github_username|用户的GitHub注册名|
- 返回实例：
<pre>
<code>
{
"status":"true",
"info": "修改成功"
}
</code>
</pre>
- 返回参数说明：

|参数名称|说明|
|-------|------|
|status|boolean类型，true表示修改操作正确，false表示修改操作错误|
|info|返回结果说明信息|