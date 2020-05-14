## 接口：GetNextPrevStudent   [返回](README.md)
用例：[批改实验](用例/批改实验.md)
-  功能：返回当前学生的前一个或者后一个学生的学号
- 权限：仅限于教师角色调用此接口
- API请求地址：https://testmanage.com/v1/api/getNextPrevStudent/<student_id>
- 请求方式：GET
- 请求参数说明：

|参数名称|说明|
|------|------|
|is_next|bool类型的值，取1表示下一个，取0表示上一个|
|student_id|学生的ID号，学生的学号|
- 返回实例：
<pre>
<code>
{
"status":true，
"info":null，
"ID":"201710414204"
}
</code>
</pre>
- 返回参数说明：

|参数名称|说明|
|------|------|
|status|bool类型，true代表当前操作成功，false表示当前操作失败|
|info|返回结果说明信息|
|student_id|学生学号或者教师工号|

