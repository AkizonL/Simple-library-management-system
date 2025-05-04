毕设来的，到了反哺开源社区的时候了:-)
1，python 3.11+MySql
2，venv 为虚拟环境，您可以直接指定环境运行，或者安装 requirements.txt 文件
3，v1，v2 文件夹为不同的版本，可按需选择，复制所有文件到根目录，删除原有根目录中所有的.py 文件即可
4，librarydatabase.sql 为数据库文件，可以直接在 Navicat 里面导入
5，connector.py 和 connector_pymysql.py 是用不同的数据库驱动第三方库写的，运行时用的后者
6，main.py 是控制台程序，UI_main 带有 GUI 页面
7，connector.py 和 connector_pymysql.py 里面最后面的
db_config = {
"host": "localhost",
"database": "librarydatabase", # 自动转换为 pymysql 的 db 参数
"user": "root",
"password": "114514"
}中的"password"字段值改为您自己的数据库密码

ps.因为使用的 qfluentwidgets（https://qfluentwidgets.com/）为GPL开源协议，所以您更改后开源的时候，请同样使用GPL协议，并禁止商用（虽然不可能就是了）
