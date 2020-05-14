## 接口：getUserInfo   [返回](README.md)
用例：[修改用户信息](用例/修改个人信息.md)
-  功能：获取用户的所有信息
- 权限：用于老师和学生查看自己的信息，必须先登录，同时不能查看本人的信息
- API请求地址：https://testmanage.com/v1/api/getUserInfo/<user_id>
- 请求方式：GET
- 请求参数说明：

|参数名称|说明|
|------|------|
|user_id|用户的ID号，对应表的USER.USER_ID的支|
- 返回实例：
<pre>
<code>
{
"status":true，
"info":null，
"ID":"201710414204"
"name":"张三"
"class_dept":"软件工程2班"
"github_username":"honora"
"type":"学生"
}
</code>
</pre>
- 返回参数说明：

|参数名称|说明|
|------|------|
|status|bool类型，true代表当前操作成功，false表示当前操作失败|
|info|返回结果说明信息|
|ID|学生学号或者教师工号|
|name|用户的真实姓名|
|class_dept|班级或者部门名称|
|github_username|用户的GitHub注册名|
|type|用户类型：学生或者老师|
