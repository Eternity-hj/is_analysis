## 接口：GetOneStudentResult   [返回](README.md)
用例：[查看成绩](用例/查看成绩.md)，[批改实验](用例/批改实验.md)
-  功能：获得一个学生的所有实验成绩和实验评价
- 权限：用于老师和学生查看自己的信息，必须先登录，同时不能查看本人的信息
- API请求地址：https://testmanage.com/v1/api/getOneStudentResult/<student_id>
- 请求方式：GET
- 请求参数说明：

|参数名称|说明|
|------|------|
|student_id|学生的ID号，学生的学号|
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
"total":
"data": [
          {
          "test_id":1,
          "web_exists": true, 
          "result": 91, 
          "memo":"本实验做得好",
          "update_date": "2018-04-02 13:48:01"
          }, 
          {
          ...其他实验
          }
      ] 
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
