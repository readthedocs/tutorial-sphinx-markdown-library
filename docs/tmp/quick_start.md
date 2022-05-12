# 第1章 快速上手

## 访问用户门户

您可以使用Web浏览器访问”神工坊“高性能仿真平台V2.0用户门户。

建议您使用Google Chrome或Microsoft Edge浏览器访问。

### 登录

登录”神工坊“高性能仿真平台V2.0用户门户前应确保：您已具有含用户门户登录权限的用户账号（用户名和密码）；

*“神工坊”高性能仿真平台V2.0用户门户IP地址https://192.168.61.51:8888*，例如，在浏览器地址栏中输入192.168.61.51:8888，显示系统登录页面如下。

[![qjJG1x.png](https://s1.ax1x.com/2022/04/06/qjJG1x.png)](https://imgtu.com/i/qjJG1x)

-   输入正确的用户名及密码登录系统后，进入平台桌面。

-   用户登录后，如半小时未操作，会话即自动过期，需要重新登录。

[![qjG1Qf.png](https://s1.ax1x.com/2022/04/06/qjG1Qf.png)](https://imgtu.com/i/qjG1Qf)

### 退出

如要退出系统，请在系统右上角单击户头像图标[![qjYDZF.png](https://s1.ax1x.com/2022/04/06/qjYDZF.png)](https://imgtu.com/i/qjYDZF)，然后选择**退出**即回到系统登录页面。

[![qjGdWq.png](https://s1.ax1x.com/2022/04/06/qjGdWq.png)](https://imgtu.com/i/qjGdWq)

### 进入和退出全屏模式

登录用户门户后，在桌面上任意位置单击右键，选择**进入全屏**即可进入全屏模式；如要退出全屏模式，按**Esc**键或在桌面上任意位置单击右键后选择**退出全屏**即可。

[![qjG0S0.png](https://s1.ax1x.com/2022/04/06/qjG0S0.png)](https://imgtu.com/i/qjG0S0)

### 刷新

登录用户门户后，在桌面上任意位置单击右键，点击**刷新，**即可刷新当前页面，适用于实时刷新当前用户信息，例如用户权限被修改以及应用权限的修改。用户能通过刷新获取最新的应用权限信息。

## 快速上手示例

本节的示例将给您展示在“神工坊“高性能仿真平台V2.0上正确使用应用的**最少必要知识**。本图文教程秉承着“宁繁勿简”的原则。习惯于视频教程的用户可移步[视频教程](https://space.bilibili.com/301027927?spm_id_from=333.788.b_765f7570696e666f.2)。扫码关注“神工坊”哔哩哔哩账号，该账号将持续更新神工坊最新资料。

[![qzlOBD.jpg](https://s1.ax1x.com/2022/04/07/qzlOBD.jpg)](https://imgtu.com/i/qzlOBD)

[仿真计算](#第4章-仿真计算)[![qjYOQP.png](https://s1.ax1x.com/2022/04/06/qjYOQP.png)](https://imgtu.com/i/qjYOQP)：仿真类软件，需提交至CPU计算队列。

[图形应用](#第3章-图形应用)[![qjYjL8.png](https://s1.ax1x.com/2022/04/06/qjYjL8.png)](https://imgtu.com/i/qjYjL8)：设计类、可视化类软件，需提交至GPU渲染队列以使用GPU加速渲染功能。

**GUI作业提交方式：**

VDI：虚拟远程桌面接口（需付费开通）

VNC：虚拟网络控制台（免费使用）

仿真计算的GUI模式和图形应用均可使用上述两种方式提交。

以下展示集群用户基本队列，使用其他更多队列资源请联系管理员：

**CPU计算队列：**q_x86_sf

**GPU渲染队列：**GPU_sf

本节的仿真计算示例为：Abaqus2017，图形应用示例为Abaqus2017-CAE。

[![qz8nXV.png](https://s1.ax1x.com/2022/04/07/qz8nXV.png)](https://imgtu.com/i/qz8nXV)**警告** 请不要在使用**仿真计算**应用时提交至**GPU渲染队列**，作业将被管理员杀掉。

[![qz8nXV.png](https://s1.ax1x.com/2022/04/07/qz8nXV.png)](https://imgtu.com/i/qz8nXV)**警告** 请不要在使用**图形应用**时提交至**CPU计算队列**，作业将被管理员杀掉。

![qz8WB8.png](https://s1.ax1x.com/2022/04/07/qz8WB8.png)**注意**
**仿真计算应用也可打开图形界面**，进行简单的前后处理，只是无法使用高性能GPU渲染。当对渲染性能要求不高时，可以使用该方式。

### 仿真计算

登录用户门户后，在页面底部的菜单栏单击**仿真计算**[![qjYOQP.png](https://s1.ax1x.com/2022/04/06/qjYOQP.png)](https://imgtu.com/i/qjYOQP)，进入如下桌面。桌面上将显示您目前已经订阅的仿真应用；

![](media/647970a1c4aca5b6cd2a2696091fea90.png)

**准备工作：**

（a）**应用订阅**。若没有您需要的应用，在页面底部的菜单栏单击**应用订阅![](media/2ed952413e107b1a374e89cce848fc41.png)**，弹出如下页面。在**全部应用**中点击申请订阅，联系管理员进行审批。订阅成功后将在上方**已订阅应用**中显示该应用。

[![qjNfED.png](https://s1.ax1x.com/2022/04/06/qjNfED.png)](https://imgtu.com/i/qjNfED)

为了方便您测试，在已订阅应用的最右侧**应用文档**中可下载相应的输入文件。

（b）**上传文件**。在页面底部的菜单栏单击**数据管理**[![qjtWfs.png](https://s1.ax1x.com/2022/04/06/qjtWfs.png)](https://imgtu.com/i/qjtWfs)，弹出个人数据管理页面。在个人目录页面中，点击新建文件夹并输入名称，如abaqus。双击进入新建的目录，右击空白处，选择上传文件，选择要上传的文件或目录（多个文件或整个目录建议压缩后上传速度更快）。上传完成后的文件可进行复制、粘贴、编辑等操作。
[![qjaH78.png](https://s1.ax1x.com/2022/04/06/qjaH78.png)](https://imgtu.com/i/qjaH78)

（c）远程虚拟桌面（VDI方式）开通。在页面底部的菜单栏单击**远程桌面**[![qjNejP.png](https://s1.ax1x.com/2022/04/06/qjNejP.png)](https://imgtu.com/i/qjNejP)，选择开通远程工作站，选择虚拟机规格后点击提交。若出现资源不足请联系管理员。具体内容请参考本文档[第五章](#第5章-远程桌面)；

[![qjdV39.png](https://s1.ax1x.com/2022/04/06/qjdV39.png)](https://imgtu.com/i/qjdV39)

开通成功后，如下图所示。

[![qjdnnx.png](https://s1.ax1x.com/2022/04/06/qjdnnx.png)](https://imgtu.com/i/qjdnnx)

**（一）经典GUI界面使用方式（VDI方式）**

1.  双击应用图标，如**Abaqus2017**，弹出应用、集群参数设置页面，鼠标滚轮可上下移动页面。其中带”\*“的项目为必填参数，其余为可选参数。例如，资源池和队列为必填参数，其将决定您使用的计算资源；用户子程序为可选参数，仅当需要使用该功能时填写。各项目具体含义及注意事项请参考本文档[第四章](#441-abaqus)。将GUI开关置为是。页面如下图所示。

[![qjwUz9.png](https://s1.ax1x.com/2022/04/06/qjwUz9.png)](https://imgtu.com/i/qjwUz9)

2.  按上图所示，填写作业名称，选择资源池、图形界面、队列、CPU等参数；其中，图形应用选择VDI。

**注意**
此处CPU核数为之后提交Abaqus作业的并发最大核数

3.  点击提交，提交作业至**CPU计算节点**。弹出作业详情页面，如下图所示。

[![qjwOQs.png](https://s1.ax1x.com/2022/04/06/qjwOQs.png)](https://imgtu.com/i/qjwOQs)

4.  稍等几秒钟，在页面底部的菜单栏单击**远程桌面![](media/582c38d05eddb0417f8033f08b77b573.png)**，如下图所示，Abaqus经典界面已经在其中显示。

[![qj0EO1.png](https://s1.ax1x.com/2022/04/06/qj0EO1.png)](https://imgtu.com/i/qj0EO1)

5.  有限元模型定义。跟个人电脑没有任何区别。这里演示已经下载好的案例。File \>
    Import \> Model调出文件选择器，File Filter选择Abaqus Input
    File。选择上传的\*.inp文件，点击OK，如下图所示。

[![qj0Jmt.png](https://s1.ax1x.com/2022/04/06/qj0Jmt.png)](https://imgtu.com/i/qj0Jmt)

6.  提交计算。跟个人电脑提交作业没有任何区别。需要并行计算请在Edit Job \>
    Parallelization中设置并行核数，其余选项默认即可，如下图所示。


![qz8WB8.png](https://s1.ax1x.com/2022/04/07/qz8WB8.png)**注意**
同时运行的作业总核数不得超过提交作业时设定的值。

[![qj00pQ.png](https://s1.ax1x.com/2022/04/06/qj00pQ.png)](https://imgtu.com/i/qj00pQ)

[![qj0hp4.png](https://s1.ax1x.com/2022/04/06/qj0hp4.png)](https://imgtu.com/i/qj0hp4)

7.  后处理。跟个人电脑提交作业没有任何区别。

[![qj0OhD.png](https://s1.ax1x.com/2022/04/06/qj0OhD.png)](https://imgtu.com/i/qj0OhD)

若您最小化了界面，恢复请先点击右下方隐藏dock面板![](media/0404e94c52298d3f6f64b65428ea3e3c.png)，防止菜单栏阻挡鼠标操作。全屏以获得更好的操作体验，见[2.1.3](#213进入和退出全屏模式)。

![qz8WB8.png](https://s1.ax1x.com/2022/04/07/qz8WB8.png)**注意**
工作目录若不指定，默认为用户Home目录。指定工作目录方法:File\>Set Work Directory…

**（二）经典GUI界面使用方式（VNC方式）**

[![qjBygH.md.png](https://s1.ax1x.com/2022/04/06/qjBygH.md.png)](https://imgtu.com/i/qjBygH)

1.  按上图所示，填写作业名称，选择资源池、图形界面、队列、CPU等参数；其中，图形应用选择VNC。VNC方式无需开通远程虚拟桌面，**但性能上会比VDI方式弱**。

2.  点击提交，提交作业至**CPU计算节点**。弹出作业详情页面，如下图所示。

[![qjB458.md.png](https://s1.ax1x.com/2022/04/06/qjB458.md.png)](https://imgtu.com/i/qjB458)

3.  稍等几秒钟，点击刷新，然后点击**图形窗口**，即可进入经典GUI界面。

[![qjDnRe.md.png](https://s1.ax1x.com/2022/04/06/qjDnRe.md.png)](https://imgtu.com/i/qjDnRe)

4.  其余步骤和注意事项与VDI方式一致，这里不再赘述。

**（三）Batch模式使用方式**

**当需要进行较大规模计算时，强烈建议您使用Batch模式，以免图形界面误关闭导致计算中断。**

1.  双击应用图标，如**Abaqus2017**，弹出应用、集群参数设置页面，鼠标滚轮可上下移动页面。其中带”\*“的项目为必填参数，其余为可选参数。例如，资源池和队列为必填参数，其将决定您使用的计算资源；用户子程序为可选参数，仅当需要使用该功能时填写。各项目具体含义及注意事项请参考本文档[第四章](#441-abaqus)；

2.  填写作业名称，选择队列和CPU参数；

[![qz8WB8.png](https://s1.ax1x.com/2022/04/07/qz8WB8.png)](https://imgtu.com/i/qz8WB8)**注意**
队列请选择CPU计算队列，如q_x86_sf。

1.  一般仿真应用需要指定输入文件。点击INP文件项目后方选择文件，弹出服务器文件管理器。在管理器中选择提前上传好的文件。成功选择后如下图所示，将在文件名下方显示文件名称；

[![qjD0Ln.md.png](https://s1.ax1x.com/2022/04/06/qjD0Ln.md.png)](https://imgtu.com/i/qjD0Ln)

2.  点击“提交”，提交作业至CPU节点。在弹出的作业详情页面中，可查看作业信息，例如，作业状态，一般分为等待、运行、完成、退出（等待一般为资源不足，尝试减少CPU核数；退出一般为作业异常结束，请查看日志或求解器输出信息）；再如，作业号：10769。点击左侧刷新，可更新作业信息。此外，停止和暂停按钮分别可以杀掉和挂起作业，具体细节参考本文档[第六章](#第6章-作业管理)。

[![qjDWQJ.md.png](https://s1.ax1x.com/2022/04/06/qjDWQJ.md.png)](https://imgtu.com/i/qjDWQJ)

3.  点击查看输出，可以查看求解器的输出信息。该信息保存在与作业号同名的\*.out文件，该文件路径一般与输入文件一致。

[![Ly0RdP.png](https://s1.ax1x.com/2022/04/21/Ly0RdP.png)](https://imgtu.com/i/Ly0RdP)

4.  点击作业数据，进入工作目录，右键**刷新**。右键相关文件，即可进行在线预览、下载等操作。亦可通过数据管理器查看，见[2.2中的上传文件教程](#221仿真计算)。

[![qzuHeJ.md.png](https://s1.ax1x.com/2022/04/07/qzuHeJ.md.png)](https://imgtu.com/i/qzuHeJ)

5.  作业详情的重新打开。单击页面底部的菜单栏“作业管理“[![qzKSyD.png](https://s1.ax1x.com/2022/04/07/qzKSyD.png)](https://imgtu.com/i/qzKSyD)，单击作业号即可重新打开对应ID的作业详情页面。

[![qzK8f0.md.png](https://s1.ax1x.com/2022/04/07/qzK8f0.md.png)](https://imgtu.com/i/qzK8f0)

### 图形应用

1.  登录用户门户后，在页面底部的菜单栏单击**图形应用**[![qjYjL8.png](https://s1.ax1x.com/2022/04/06/qjYjL8.png)](https://imgtu.com/i/qjYjL8)，进入如下桌面。桌面上将显示您目前已经订阅的图形应用；

2.  编辑实例。右击应用图标后选择编辑实例，如**Abaqus2017-CAE**，弹出实例编辑页面。一般会有一个系统默认实例，点击查看可一下查看该实例参数但不能修改。

[![qzM0KS.png](https://s1.ax1x.com/2022/04/07/qzM0KS.png)](https://imgtu.com/i/qzM0KS)

3.  若系统默认实例不能满足您的使用需求，点击右上方新增实例以设置自定义实例，设置完成后保存，如下图所示。（注意：1、图形界面若选择**VDI需开通远程桌面功能**，见[2.2.1](#221仿真计算)，具体内容参考本文档[第五章](#第5章-远程桌面)；2、队列请选择**图形队列**，否则无法启动GPU渲染，队列资源参考[2.2](#22-快速上手示例)或本文档[第八章](#第8章-资源动态)）；

[![qzMsEj.png](https://s1.ax1x.com/2022/04/07/qzMsEj.png)](https://imgtu.com/i/qzMsEj)

[![qzM5b4.md.png](https://s1.ax1x.com/2022/04/07/qzM5b4.md.png)](https://imgtu.com/i/qzM5b4)

4.  设置默认实例。方法1，实例编辑完成后，在实例编辑页面的实例名称前的方框中勾选实例，点击右上方的设置为默认实例；方法2，右击应用图标，移动至设置默认实例进行设置。
[![qzMjKO.md.png](https://s1.ax1x.com/2022/04/07/qzMjKO.md.png)](https://imgtu.com/i/qzMjKO)

    [![qzQSVH.png](https://s1.ax1x.com/2022/04/07/qzQSVH.png)](https://imgtu.com/i/qzQSVH)

5.  打开图形应用。双击应用图标，等待应用程序加载。
[![qzQmZQ.png](https://s1.ax1x.com/2022/04/07/qzQmZQ.png)](https://imgtu.com/i/qzQmZQ)

6.  图形应用的重新打开。图形作业与仿真作业一样，提交后可至作业管理中查看作业信息，参考2.2.1中的5。若使用VNC方式提交，关闭VNC窗口而不关闭图形应用，图形作业任持续运行。单击页面底部的菜单栏“作业管理“[![qzKSyD.png](https://s1.ax1x.com/2022/04/07/qzKSyD.png)](https://imgtu.com/i/qzKSyD)，单击作业号即可重新打开对应ID的作业详情页面。单击右上方图形窗口，即可重新打开VNC窗口。

[![qzQQGq.png](https://s1.ax1x.com/2022/04/07/qzQQGq.png)](https://imgtu.com/i/qzQQGq)