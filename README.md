# hello-world
**dd~~粗体+删除线~~cc**
__~~粗体+删除线~~__
*~~斜体+删除线~~*
_~~斜体+删除线~~_
***~~粗斜体+删除线~~***
___~~粗斜体+删除线~~___
**~粗体+删除线~**
__~粗体+删除线~__
*~斜体+删除线~*
_~斜体+删除线~_
***~粗斜体+删除线~***
___~粗斜体+删除线~___
~~**删除线+粗体**~~
~~__删除线+粗体__~~
~~*删除线+斜体*~~
~~_删除线+斜体_~~
~~***删除线+粗斜体***~~
~~___删除线+粗斜体___~~
~**删除线+粗体**~
~__删除线+粗体__~
~*删除线+斜体*~
~_删除线+斜体_~
~***删除线+粗斜体***~
~___删除线+粗斜体___~
**粗体**
__粗体__
*斜体*
_斜体_
***粗斜体***
___粗斜体___
~删除线~
~~删除线~~
**[粗体](https://www.baidu.com/)**
__[粗体](https://www.baidu.com/)__
*[斜体](https://www.baidu.com/)*
_[斜体](https://www.baidu.com/)_
***[粗斜体](https://www.baidu.com/)***
___[粗斜体](https://www.baidu.com/)___
~[删除线](https://www.baidu.com/)~
~~[删除线](https://www.baidu.com/)~~
**`inline code`**
__`inline code`__
*`inline code`*
_`inline code`_
***`inline code`***
___`inline code`___
~`inline code`~
~~`inline code`~~
[**百度**](https://www.baidu.com/)
[__百度__](https://www.baidu.com/)
[*百度*](https://www.baidu.com/)
[_百度_](https://www.baidu.com/)
[***百度***](https://www.baidu.com/)
[___百度___](https://www.baidu.com/)
[~百度~](https://www.baidu.com/)
[~~百度~~](https://www.baidu.com/)
[`inline code`](https://www.baidu.com/)
[**`inline code`**](https://www.baidu.com/)

[__`inline code`__](https://www.baidu.com/)

[*`inline code`*](https://www.baidu.com/)

[_`inline code`_](https://www.baidu.com/)

[***`inline code`***](https://www.baidu.com/)

[___`inline code`___](https://www.baidu.com/)

[~`inline code`~](https://www.baidu.com/)

[`~~inline code~~`](https://www.baidu.com/)

[`**百度**`](https://www.baidu.com/)
[`__百度__`](https://www.baidu.com/)
[`*百度*`](https://www.baidu.com/)
[`_百度_`](https://www.baidu.com/)
[`***百度***`](https://www.baidu.com/)
[`___百度___`](https://www.baidu.com/)
[`~百度~`](https://www.baidu.com/)
[`~~百度~~`](https://www.baidu.com/)
`**[百度](https://www.baidu.com/)**`
`__[百度](https://www.baidu.com/)__`
`*[百度](https://www.baidu.com/)*`
`_[百度](https://www.baidu.com/)*`
`***[百度](https://www.baidu.com/)***`
`___[百度](https://www.baidu.com/)***`
`~~[百度](https://www.baidu.com/)~~`
`~[百度](https://www.baidu.com/)~`
# mdH1
## mdH2
### mdH3
####mdH4
**粗体** or __粗体__ 
*斜体* or _斜体_ 
***粗体+斜体*** 
~下划线~ 2没有通用的下划线语法，编辑器只是手动自定义的
~~删除线~~ 
# H2
`行内代码` 
[] 待办不是通用的，是自定义的
[x] 完成待办
***123123
```css
123
```
3. 有序
    9. 123123
1. 123123123123
- 无序1
+ 无序3
	+ 无序123123123
* 无序2
	* 1231123123
```go
hello world
```
# 123123
1. 123
a. 123
Q. 123123
[] 待办
[x] 完成待办
1. 指定语言的代码块

```go
hello world
```

2. 指定语言的代码块，并且语言后面有空格

```go   
hello world
```

3. 不指定语言的代码块，创建为Plain Text类型代码块

```
hello world
```

4. 无闭合标签的代码块

```go
hello world

5. 行内代
`code`
> 引用
---

11分割线
Ph-f7-179
- - -
* * *
***
*****
----- 
-----------------------------
# H1💰222
```
1. 123
23
```bash
123123
```
代码块123123()
2. 12323
# 12123
   ```shell
	##2222

	222
   ```
3. 12323
1. keymapcase相关

   ``` shell
   ## 读取验证
   ./bin/keymap_case -c -filter_time 3 -start_time 2021-06-22T15:47:00Z -end_time 2021-06-22T15:49:30Z &run.log &
   
   ## 删除旧数据
   ./bin/keymap_case -d -old_del_ratio 100 -c -filter_time 3 -start_time 2021-01-01T12:00:00Z -end_time 2021-01-10T17:00:00Z
   ```

2. 生成fstab

   ``` shell
   for disk in {b..s}; do tune2fs -l /dev/sd${disk}1 | grep UUID | awk '{print "UUID="$3}'; done | awk 'BEGIN{i=0}{printf "%s\t/home/disk%d\text4\tnoatime\t0\t0\n",$0,i;i+=1}'
   ```

3. 生成drop_space语句

   ``` shell
   ./bin/aries_cli -op list_space -print_json=true | jq '.space_list[]|"./bin/aries_cli -op drop_space -space_name="+(.space_name|tostring)+" -space_id="+(.space_id|tostring)' | tr -d \" 
   ```

4. 发送邮件

   ``` shell
   echo -e "To: zhengchenyang@baidu.com\nCC: zhengchenyang@baidu.com\nFrom: test<zhengchenyang@baidu.com>\nSubject: test\n\nhello world" | sendmail -t
   ```

5. 安全漏洞处理方法

   ``` shell
   如果该帐号(例: testuser)不需要密码登录，则使用如下命令删除密码。
   参考方法：passwd -d testuser
   如果该帐号(例: testuser)为部署服务使用的账号，建议将其login shell修改为nologin，
   参考方法：usermod -s /sbin/nologin testuser
   
   根据《百度Linux主机安全配置规范》中物理机账号权限管理部分："uid为0的均为root权限帐户，系统中应该有且只有1个。IDC服务器只允许root、work、rd账号可shell登录"
   ```

   ```Java
2222
	```
3.3333
# 123
[eeeeeeeeeee](https://www.baidu.com)
![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)
![t2](https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=2771978851,2906984932&fm=26&gp=0.jp)

[eeeeeeeeeee](https://www.baidu.com)
| 1123123 | 1222222 | 
| :------ | :-----: |
| vvvvvq2 | 11fff32 |
