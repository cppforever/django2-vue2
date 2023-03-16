# django2-vue2（基于django-vue-admin的二次开发，感谢作者袁小天）
一个后台django2.xx版本，前台vue2版本制作的后台管理系统
环境需求：python3.8或3.9版本、node.js版本16、Mysql >= 5.7.0 (可选，默认数据库sqlite3，推荐8.0版本)、Redis(可选，最新版)
本地下载及运行：          
git clone https://gitee.com/liqianglog/django-vue-admin.git #下载
#后端运行
1、进入后端项目目录:cd backend
2、在项目根目录中，复制 ./conf/env.example.py 文件为一份新的到 ./conf/env.py 下，并重命名为env.py
3、在 env.py 中配置数据库信息(默认数据库为sqlite3，测试演示可忽略此步骤)
4、安装依赖环境: pip3 install -r requirements.txt -i https://mirrors.aliyun.com/pypi/simple
5、执行迁移命令: python3 manage.py makemigrations python3 manage.py migrate
6、初始化数据: python3 manage.py init
7、初始化省市县数据: python3 manage.py init_area
8、启动项目: python3 manage.py runserver 0.0.0.0:8000     
#前端运行
1、进入前端项目目录 cd web
2、安装依赖 npm install --registry=https://registry.npm.taobao.org
3、启动服务 npm run dev
#访问项目
访问地址：http://localhost:8080 (opens new window)(默认为此地址，如有修改请按照配置文件)
账号：superadmin 密码：admin123456
