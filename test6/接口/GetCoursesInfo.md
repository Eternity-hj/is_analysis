## 接口：getCoursesInfo   [返回](README.md)
用例：[选择课程](用例/选择课程.md)
- 功能：获取老师开设的课程信息
- 权限：老师和学生
- API请求地址：https://testmanage.com/v1/api/getCoursesInfo/<user_id>
- 请求方式：GET
- 请求实例：
<pre>
<code>
{
"teacher_id":"201710414204",
"name":"李四"
"github_username":"lisi"
date:[
{"courses":"Linux"
"time":"1-12周"
"address":"10517"
"credit":"3分"
"faceto":"17软件工程"}
{其他课程信息......}
]
}
</code>
</pre>
- 请求参数说明：

|参数名称|说明|
|-------|------|
|teacher_id|老师的工号。|
|github_username|用户的GitHub注册名|
|name|老师的真实姓名|
|courses|老师所要新开设的课程名称|
|time|该课程的上课周数|
|address|该门课的上课地点|
|credit|该门课的学分|
|faceto|该门课的面向的专业学生|
- 返回实例：
<pre>
<code>
{
"status":"true",
"info": null
}
</code>
</pre>
- 返回参数说明：

|参数名称|说明|
|-------|------|
|status|boolean类型，true表示修改操作正确，false表示修改操作错误|
|info|返回结果说明信息|