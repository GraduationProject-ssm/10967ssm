# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# 10967ssm家教平台系统

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1Sh44eDEx6?p=66)


# 系统概述
进过系统的分析后，就开始记性系统的设计，系统设计包含总体设计和详细设计。总体设计只是一个大体的设计，经过了总体设计，我们能够划分出系统的一些东西，例如文件、文档、数据等。而且我们通过总体设计，大致可以划分出了程序的模块，以及功能。但是只是一个初步的分类，并没有真正的实现。

整体设计，只是一个初步设计，而且，对于一个项目，我们可以进行多个整体设计，通过对比，包括性能的对比、成本的对比、效益的对比，来最终确定一个最优的设计方案，选择优秀的整体设计可以降低开发成本，增加公司效益，从这一点来讲，整体设计还是非常重要的。

家教平台系统工作原理图如图4-1所示：

![](/md/blog.013.png)

图4-1 系统工作原理图
## 4.2 系统结构设计
系统架构图属于系统设计阶段，系统架构图只是这个阶段一个产物，系统的总体架构决定了整个系统的模式，是系统的基础。家教平台系统的整体结构设计如图4-2所示。

![](/md/blog.014.png)

图4-2 系统结构图
## 4.3数据库设计
数据库是计算机信息系统的基础。目前，电脑系统的关键与核心部分就是数据库。数据库开发的优劣对整个系统的质量和速度有着直接影响。
### 4.3.1 数据库设计原则
数据库的概念结构设计采用实体—联系（E-R）模型设计方法。E-R模型法的组成元素有：实体、属性、联系，E-R模型用E-R图表示，是提示用户工作环境中所涉及的事物，属性则是对实体特性的描述。在系统设计当中数据库起着决定性的因素。下面设计出这几个关键实体的实体—关系图。
### 4.3.2 数据库实体
数据模型中的实体（Entity），也称为实例，对应现实世界中可区别于其他对象的“事件”或“事物”。例如，公司中的每个用户，家里中的每个家具。

本系统的E-R图如下图所示：

1、用户信息：账号、姓名、性别、手机、邮箱、照片、地址，实体图如图4-3所示：

![](/md/blog.015.png)

图4-3用户信息实体图

2、教师信息：教师工号、密码、教师姓名、年龄、性别、学院、学历、手机、邮箱、照片，实体图如图4-4所示：

![](/md/blog.016.png)

`  `图4-4教师信息实体图

3、教师申请信息：账号、姓名、标题、申请原因、申请日期实体图如图4-5所示：

![](/md/blog.017.png)

图4-5教师申请信息实体图

#########

### 4.3.3 数据库表设计
数据库的表信息属于设计的一部分，下面介绍数据库中的各个表的详细信息。

表4-1 allusers表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|NOT NULL|
|username|varchar|50|` `default NULL|
|pwd|varchar|50|` `default NULL|
|cx|varchar|50|` `default NULL|


表4-2 jiaoshi表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|jiaoshigonghao|varchar|50|default NULL|
|mima|varchar|50|default NULL|
|jiaoshixingming|varchar|50|default NULL|
|nianling|varchar|50|default NULL|
|xingbie|varchar|50|default NULL|
|zhuanye|varchar|50|default NULL|
|xueli|varchar|50|default NULL|
|shouji|varchar|50|default NULL|
|youxiang|varchar|50|default NULL|
|zhaopian|varchar|50|default NULL|

表4-3：jiaoshijianli表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|` `int|11|NOT NULL |
|addtime|varchar|50|default NULL|
|jiaoshigonghao|varchar|50|default NULL|
|jiaoshixingming|varchar|50|default NULL|
|zhuanye|varchar|50|default NULL|
|xueli|varchar|50|default NULL|
|xingbie|varchar|50|default NULL|
|zhaopian|varchar|50|default NULL|
|chushengriqi|varchar|50|default NULL|
|gongzuojingli|varchar|50|default NULL|
|gerentezhang|varchar|50|default NULL|
|qiwangxinzi|varchar|50|default NULL|
|jiaoyubeijing|varchar|50|default NULL|
|huojiangzhengshu|varchar|50|default NULL|
|biyexuexiao|varchar|50|default NULL|
|xiangxineirong|varchar|50|default NULL|


表4-4：jiaoshishenqing表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|` `int|11|NOT NULL |
|addtime|varchar|50|default NULL|
|zhanghao|varchar|50|default NULL|
|xingming|varchar|50|default NULL|
|biaoti|varchar|50|default NULL|
|neirong|varchar|50|default NULL|
|shenqingyuanyin|varchar|50|default NULL|
|shenqingriqi|varchar|50|default NULL|
|sfsh|varchar|50|default NULL|
|shhf|varchar|50|default NULL|

表4-5：yonghu表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|` `int|11|NOT NULL |
|addtime|varchar|50|default NULL|
|zhanghao|varchar|50|default NULL|
|mima|varchar|50|default NULL|
|xingming|varchar|50|default NULL|
|xingbie|varchar|50|default NULL|
|shouji|varchar|50|default NULL|
|youxiang|varchar|50|default NULL|
|zhaopian|varchar|50|default NULL|
|dizhi|varchar|50|default NULL|





# 5统详细设计
## 5.1前台首页功能模块
家教平台系统，用户在系统首页可以查看首页、教师简历、课程信息、招聘教师、通知公告、个人中心、后台管理等内容，如图5-1所示。

![](/md/blog.018.png)

图5-1前台首页功能界面图



`    `用户注册，在用户注册页面用户填写账号、密码、姓名、手机、邮箱、地址等详细信息进行注册，如图5-2所示。

![](/md/blog.019.png)

图5-2用户注册界面图

登录，用户在登录页面通过填写账号、密码信息完成登录，如图5-3所示。

![](/md/blog.020.png)

图5-3登录界面图



课程信息，用户进入到课程信息界面，通过界面进行查看，也可根据需要课程信息名称进行搜索操作，如图5-4所示。 

![](/md/blog.021.png)

图5-4课程信息界面图

招聘教师，用户进入到招聘教师界面，通过界面进行查看，也可根据需要招聘教师搜索操作，点击应聘页面查看名称、职位、账号、姓名、应聘时间、教师工号、教师姓名、手机等操作，如图5-5所示。 

![](/md/blog.022.png)

![](/md/blog.023.png)

图5-5招聘教师界面图

个人中心，用户在个人信息页面中可以查看账号、姓名、性别、手机、邮箱、照片、地址等信息，并可根据需要对已有个人信息修改或删除等操作，如图5-6所示。

![](/md/blog.024.png)

图5-8个人信息界面图


## 5.2管理员功能模块
管理员登录，管理员通过填写用户名、密码进行登录，如图5-7所示。

![](/md/blog.025.png)

图5-7管理员登录界面图

管理员登录进入家教平台系统可以查看首页、个人中心、用户管理、教师管理、教师简历管理、教师申请管理、课程信息管理、招聘教师管理、应聘职位管理、用户评价管理、系统管理等信息。如图5-7所示。

用户管理，管理员在用户管理页面中可以查看账号、姓名、性别、手机、邮箱、照片、地址等内容进行查看详情、删除、修改，如图5-8所示。

![](/md/blog.026.png)

图5-7首页界面图

![](/md/blog.027.png)

图5-8用户界面图

教师管理，管理员在教师管理页面中可以查看教师工号、密码、教师姓名、年龄、性别、学院、学历、手机、邮箱、照片等信息，并可根据需要对已有教师进行详情、修改或删除等操作，如图5-9所示。

![](/md/blog.028.png)

图5-9教师管理界面图

教师简历管理，管理员在教师简历管理页面中可以查看详情、修改或删除等详细操作，如图5-10所示。

![](/md/blog.029.png)

图5-10教师简历管理界面图

课程信息管理，管理员在课程信息页面中可以查看详情、添加，修改或删除等详细操作，如图5-11所示。

![](/md/blog.030.png)

图5-11课程信息管理界面图

系统管理；该页面为通知公告、轮播图管理界面。管理员可以在此页面进行公告发布、首页轮播图上传，通过新建操作可在轮播图中加入新的图片，还可以对以上传的图片进行修改操作，以及图片的删除操作，如图5-12所示。

![](/md/blog.031.png)

![](/md/blog.032.png)

图5-12系统管理管理界面图



## 5.3用户功能模块
登陆，用户进入登录页面进行填写用户名、密码进行登陆操作。如图5-13所示。

![](/md/blog.033.png)

图5-13登陆界面图

首页，用户在首页页面中进行查看首页、个人中心、教师申请管理、招聘教师管理、应聘职位管理、用户评价管理等信息，如图5-14所示。

![](/md/blog.034.png)

图5-14首页界面图

个人信息，用户在个人信息页面中进行填写账号、密码、姓名、性别、手机、邮箱、照片、地址，并进行详情、删除、修改操作，如图5-15所示。

![](/md/blog.035.png)

图5-15个人信息界面图

应聘职位管理，用户在应聘职位管理页面中进行查看，并对应聘教师进行审核，如图5-16所示。

![](/md/blog.036.png)

![](/md/blog.037.png)

图5-16应聘职位管理界面图

## 5.4 教师功能模块
教师通过登录界面填写教师工号、密码进行登陆。如图5-17所示。

首页，教师在首页页面查看首页、个人中心、教师简历管理、课程信息管理、应聘职位管理、用户评价管理等信息，如图5-18所示。

![](/md/blog.038.png)

图5-15教师管理界面图

首页，教师在首页页面中查看首页、个人中心、教师简历管理、课程信息管理、应聘职位管理、用户评价管理等信息，如图5-16所示。

![](/md/blog.039.png)

图5-16教师首页界面图

个人信息，教师在个人信息页面中编辑教师工号、密码、教师姓名、年龄、性别、学院、学历、手机、邮箱、照片等信息，并进行详情、删除、修改、提交操作，如图5-17所示。

![](/md/blog.040.png)

图5-17个人信息界面图

教师简历管理，教师在教师简历页面可进行新增、删除、修改操作，如图5-18所示。

![](/md/blog.041.png)

图5-18教师简历管理界面图


应聘职位管理，教师在应聘职位管理页面中可以查看名称、职位、账号、账号、应聘时间、教师工号、教师姓名、手机等信息，并且根据需要对已有应聘职位管理进行详情查看，如图5-19所示。

![](/md/blog.042.png)

图5-19应聘职位管理界面图















