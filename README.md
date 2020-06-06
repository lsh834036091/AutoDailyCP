# AutoDailyCP
使用GitHub ACTIONS自动进行今日校园打卡

Fork后在你的项目下点击Settings增加`SCHOOL_NAME`、`ACCOUNT`、`PASSWORD`、`ADDRESS` 4个Secrets，分别对应你的学校名称、账号、密码、定位地址。<br>
![Secrets](https://github.com/lemofire/AutoDailyCP/blob/master/Secrets.png)

### ACTIONS运行方式：
* 1.push
* 2.自己给自己star
* 3.每日9点自动运行

第一次使用需要根据Actions的`Run program`中的提示修改`.github/workflows/AutoDailyCP.yml`文件中的`cat>formdb/36.json<<EOF`。<br>
~~当然你也可以使用[旧版](https://github.com/lemofire/DailyCP)就不用修改了~~<br>
栗子：<br>
* 提示：`请手动填写./formdb/41.json，之后重新运行脚本`<br>
* 修改后：`cat>formdb/41.json<<EOF`<br>
每次运行action后会自动打包formdb，可以根据里面的内容修改`cat>formdb/36.json<<EOF`下的代码

### Credits
* [Finch/FuckDailyCP](https://gitee.com/Finch1/FuckDailyCP)
