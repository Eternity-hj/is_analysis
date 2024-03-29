## 读者参与者用例规约表
### 1.登录用例规约表
| 用例名称| 登录系统 |
| ------ | :------|
| 用例ID | US1 | 
|角色|读者，系统管理员，系统管理员|
| 用例说明 | 读者通过自己已有的账号和密码登录进入图书管理系统 |
| 前置条件 | 输入正确的用户名和密码 |
| 基本事件流 | 打开系统首页，输入正确的账号密码，点击登录按钮 |
| 其他事件流 | 无 |
| 异常事件流 | 账号密码不正确 |
|后置条件|登录成功|
### 2.查询书籍信息用例规约表
| 用例名称| 查询书籍信息 |
| ------ | ------ |
| 用例ID | US2| 
|角色|读者，系统管理员，系统管理员|
| 用例说明 | 无论是读者，还是系统管理员还是图书管理员都应该可以查询书籍的信息，查询书籍是否可借，库存等信息 |
| 前置条件 | 登录系统成功 |
| 基本事件流 | 搜索要查询的书籍，点击查询状态 |
| 其他事件流 | 无 |
| 异常事件流 | 搜索书籍不存在或者书名错误，返回错误信息 |
|后置条件|书籍预定|
### 3.书籍预定用例规约表
| 用例名称| 书籍预定 |
| ------ | ------ |
| 用例ID | US3| 
|角色|读者|
| 用例说明 | 读者在查询了书籍信息之后可以预定图书，这样就不会出现借不到书的情况|
| 前置条件 | 书籍信息查询结果显示为可借 |
| 基本事件流 | 登录系统，查找要借的书，点击预定 |
| 其他事件流 | 无 |
| 异常事件流 | 无|
|后置条件|借书|
### 4.查询借阅信息用例规约表
| 用例名称| 查询借阅信息 |
| ------ | ------ |
| 用例ID | US4| 
|角色|读者|
| 用例说明 | 读者可以登录系统，查看自己的借阅信息|
| 前置条件 | 正确登录系统 |
| 基本事件流 | 登录系统，点击个人中心，查看借阅信息 |
| 其他事件流 | 无 |
| 异常事件流 | 无|
|后置条件|还书|
### 5.借书用例规约表
| 用例名称| 借书 |
| ------ | ------ |
| 用例ID | US5| 
|角色|读者|
| 用例说明 | 读者可以借阅系统内显示还有余量的书籍|
| 前置条件 | 正确登录系统，同时书记显示为可以借阅 |
| 基本事件流 | 登录系统，书籍信息显示为可以借阅，点击借阅，系统内该书的余量减一|
| 其他事件流 | 如果借书量超过上限，则显示无法借阅 |
| 异常事件流 | 该书为不可借图书|
|后置条件|续借|
### 6.续借用例规约表
| 用例名称| 续借 |
| ------ | ------ |
| 用例ID | US6| 
|角色|读者|
| 用例说明 | 借阅期未满，但是在书籍并未完全看完的情况下可以续借|
| 前置条件 | 正确登录系统，并且已有相关的借书信息|
| 基本事件流 | 登录系统，查看自己的借阅信息，在相关的书籍信息后面点击续借 |
| 其他事件流 | 已超过借阅时间，点击续借，无法继续续借 |
| 异常事件流 | 无|
|后置条件|还书|
### 7.还书用例规约表
| 用例名称| 还书 |
| ------ | ------ |
| 用例ID | US7| 
|角色|读者|
| 用例说明 | 读者登录系统，进入个人中心后，在相应的书后点击归还，即可还书，待还书成功后，系统余量加一|
| 前置条件 | 正确登录系统，已经借阅相关书籍 |
| 基本事件流 | 登录系统，点击个人中心，点击还书，未超出借阅期，即可顺利还书 |
| 其他事件流 | 如超过借阅期则不能还书成功，同时须在管理员出缴纳罚款后，方可还书成功|
| 异常事件流 | 无|
|后置条件|无|

