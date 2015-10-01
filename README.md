# 快乐学习营成员管理系统

> 给补习班做的一个成员管理系统,旨在帮助管理者更方便的管理补习班的成员,让工作变得更有效率和轻松.

> 此程序为 [Hardi](http://weibo.com/hardi/) 的第二个php项目, 此版本 core/ 和 lib/ 下的文件依然使用了上一个程序 [自画像](https://github.com/huanghao521/zihuaxiang) 的大部分代码. 下一个版本会使用面向对象思想和MVC框架进行改良. 
(---2015.10.1) 

## 功能

* 按照年级和激活状态 **分类显示** 所有成员;
* 添加成员信息,包括基本信息,交费信息,加减分,成绩统计 **四个类型**;
* 修改成员基本信息;
* 删除用户*(需管理员密码);
* 消息提醒, **5天之内** 将要到期的成员,**当天** 该交费的成员,已经 **超过** 交费期的成员 将会用不同的颜色显示在"消息"页面中
* 使用 ChartJs 显示 **统计图表** *(未完成)

## 截图

![登陆页面](https://raw.githubusercontent.com/huanghao521/happyhome/master/screenshot/1.png)
![成员列表页面](https://raw.githubusercontent.com/huanghao521/happyhome/master/screenshot/2.png)

## 使用方法

1. 导入 *happyhome_db.sql* 到数据库;
2. 打开 *configs.php* 页面,填入你的数据库地址、用户名、密码以及数据库名;
2. 在 *configs.php* 页面设置你的程序入口密码以及删除用户密码;

## 备注
* 为了使用方便, 程序登陆没有设置用户名要求,并且输入4位密码后js代码会自动提交表格,若感觉不方便请酌情调整login.php页面最下方的js代码;
* 第一版没有实现给用户添加多个电话的功能,但已把电话从用户的 member 表中分离出来了到了 phone 表中,下一版会实现这个功能;
* Hardi 使用了sublime text的 plainTasks 插件,将制作程序的过程都记录在了 TODO 文件里;