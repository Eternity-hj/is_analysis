## 接口：GetOneStudentResult   [返回](README.md)
用例：[批改实验](用例/批改实验.md)
-  功能：设置一个学生的实验成绩以及批语
- 权限：用于老师批改学生的实验成绩，仅限于老师可以调用此接口
- API请求地址：https://testmanage.com/v1/api/setOneStudentResult/<student_id>
- 请求方式：POST
- 请求示例
<pre>
<code>
{ "student_id": "201510315203",
 "total": 6, 
 "data": [ { "test_id":1, 
 "result": 91,
  "memo":"本实验做得好", },
   { ...其他实验 } ] }
</code>
</pre>
- 请求参数说明：

|参数名称|说明|
|------|------|
|student_id|学生的ID号，学生的学号|
|total|本次批改的所有实验的总数，小于等于全部实验的总数|
|data|实验的成绩和评语|
|test_id|实验编号|
|result|本实验成绩，可以为空，表示没有批改|
|memo|本实验老师的评价，可以为空|
- 返回实例：
<pre>
<code>
{
"status":true，
"info":null，
}
</code>
</pre>
- 返回参数说明：

|参数名称|说明|
|------|------|
|status|bool类型，true代表当前操作成功，false表示当前操作失败|
|info|返回结果说明信息|
