# 2.1 资源管理

资源管理负责管理集成环境的各节点（ESB服务器或运行实例），提供了新增实例、注册节点、实例资源管理、修改环境配置等功能。

## 2.1.1 资源列表

### 2.1.1.1 功能介绍

资源列表主要负责管理实例，显示管理实例基本信息、当前运行状态、资源状态及相关操作；节点的注册，包括新增、删除、修改节点注册信息。

### 2.1.1.2 界面说明

单击【资源管理】→【资源列表】进入资源列表界面。用户当前已创建实例的基本信息，呈卡片样式显示。

![](/articles/cesb/2-/images/image13.png)

图2.1‑1资源列表

实例卡片，显示该实例基本信息，可刷新启动、释放及资源状态。

![](/articles/cesb/2-/images/image14.png)


图2.1‑2实例基本信息

### 2.1.1.3 操作流程

**创建实例**

单击〖创建实例〗按钮，从右侧滑出窗口，填写相应内容（*表示必填项）后，单击〖确定〗按钮，完成管理服务器的注册。

**实例名称**：填写实例的名称；

**主机名**：填写主机名；

**主机IP**：主机的IP；

**管理端口**：管理端口；

**颜色标记**：选择颜色标记。

![](/articles/cesb/2-/images/image15.png)



图2.1‑3创建实例

**实例管理**

**刷新**

选择一个实例，单击开启状态中〖刷新〗按钮 ![](/articles/cesb/2-/images/image16.png)，刷新实例实时状态。

创建实例，首次启动时，点击〖刷新〗按钮![](/articles/cesb/2-/images/image16.png)。

![](/articles/cesb/2-/images/image17.png)


图2.1‑4刷新开启状态

**释放**

选择一个实例，单击〖释放〗按钮![](/articles/cesb/2-/images/image18.png)，弹出一个窗口，可释放该实例下所有节点资源。

![](/articles/cesb/2-/images/image19.png)


图2.1‑5释放节点

**资源状态**

选择一个实例，单击〖资源状态〗按钮 ![](/articles/cesb/2-/images/image20.png)，弹出一个窗口，可查看该实例cpu及内存的实时使用状况。

![](/articles/cesb/2-/images/image21.png)



图2.1‑6实例—CPU信息

![](/articles/cesb/2-/images/image22.png)



图2.1‑7实例—内存信息

**实例管理**

选择一个实例进行操作，单击〖实例管理〗按钮，进入该实例资源管理界面。可新增节点、添加已有节点、配置节点、查看节点日志、释放节点等操作。

![](/articles/cesb/2-/images/image23.png)



图2.1‑8实例管理

**修改实例名称**

单击“修改”按钮 ![](/articles/cesb/2-/images/image24.png)，修改当前实例名称。

![](/articles/cesb/2-/images/image25.png)



图2.1‑9修改实例名称


**新建节点**

单击〖新建节点〗按钮，弹出一个窗口，填写相应内容（*表示必填项）后，单击〖确定〗，完成服务器节点的注册。

![](/articles/cesb/2-/images/image26.png)



图2.1‑10新增节点

**配置**

选择一个服务器节点，单击当前状态中“配置”按钮![](/articles/cesb/2-/images/image27.png)，会弹出“修改配置信息”对话框。该对话框以页签形式显示出选择的服务器上的配置信息，包括启动配置、消息中间件、数据源配置、调试端口、HTTP启动配置、启动设置、日志配置、邮箱配置。详细界面如下：

![](/articles/cesb/2-/images/image28.png)



图2.1‑11配置信息窗口

**启动配置**

显示启动Server时的配置参数，启动配置各参数项默认设置，包括JAVA_HOME、Jvm参数、失败重试开关、重试次数、使用数据库开关、新增配置项。

用户可以〖重置〗或〖新增配置项〗。点击〖确定〗完成配置的修改操作。

<table>

<tr>

<td>参数项</td>

<td>默认值</td>

<td>含义</td>

</tr>

<tr>

<td>JAVA_HOME</td>

<td></td>

<td>JDK路径</td>

</tr>

<tr>

<td>Jvm参数</td>

<td></td>

<td></td>

</tr>

<tr>

<td>失败重试</td>

<td>开</td>

<td>启动组件失败时，是否重新启动</td>

</tr>

<tr>

<td>重试次数</td>

<td>3次</td>

<td></td>

</tr>

<tr>

<td>是否使用数据库</td>

<td>开</td>

<td>服务部署过程中，检查更新系统数据库配置信息</td>

</tr>
</table>

![](/articles/cesb/2-/images/image29.png)



图2.1‑12 启动配置


**消息中间件**

显示选择的服务器上的消息中间件配置信息。

![](/articles/cesb/2-/images/image30.png)



图2.1-13消息中间件配置

**数据源配置**

显示选择的服务器上的第三方数据源配置信息，用户可以勾选配置第三方数据源。

![](/articles/cesb/2-/images/image31.png)



图2.1‑14 数据源配置

**调试端口**

显示选择的服务器上的调试端口号，包括OSGI端口和JMX端口，并能选择启动特定端口。点击〖确定〗完成配置的修改操作。

![](/articles/cesb/2-/images/image32.png)



图2.1‑15 调试端口

**HTTP启动配置**

可以编辑、删除端口和空闲时间，或者点击〖新增HTTP启动〗新增启动。点击〖确定〗完成配置的修改操作。

![](/articles/cesb/2-/images/image33.png)



图2.1-16 HTTP启动配置


**启动设置**

显示当前服务器下的OSGi Bundle组件信息，可以进行启动、不启动、设置启动级别及删除组件等操作，点击〖确定〗完成配置的修改操作。

![](/articles/cesb/2-/images/image34.png)



图2.1‑17 启动设置

**日志配置**

显示选择的服务器上的日志配置信息，用户可以直接修改服务器上组件的Java包的日志，日志级别配置，配置日志输出规则。点击〖确定〗完成配置的修改操作。

![](/articles/cesb/2-/images/image35.png)



图2.1‑18 日志配置

新增日志：配置包路径、日志输出规则及启动级别，新增一条日志配置。

<table>

<tr>

<td>日志级别配置</td>

</tr>

<tr>

<td>Debug</td>

</tr>

<tr>

<td>INFO</td>

</tr>

<tr>

<td>Warn</td>

</tr>

<tr>

<td>Error</td>

</tr>

<tr>

<td>Off</td>

</tr>

<tr>

<td>All</td>

</tr>

</table>

![](/articles/cesb/2-/images/image36.png)



图2.1‑19 输出规则管理

新增输出规则：配置日志输出类型及名称，新增一条输出规则。

<table>

<tr>

<td>输出规则类型</td>

</tr>

<tr>

<td>ConsoleAppender</td>

</tr>

<tr>

<td>RollingFileAppender</td>

</tr>

<tr>

<td>DailyRollingAppender</td>

</tr>

</table>



**邮箱配置**

显示邮箱的配置参数，可以进行修改。点击〖确定〗完成配置的修改操作。

![](/articles/cesb/2-/images/image37.png)



图2.1‑20 邮箱配置


**日志**

选择一个服务器节点，单击当前状态中“日志”按钮![](/articles/cesb/2-/images/image38.png)，查看该服务器节点的控制台日志。

![](/articles/cesb/2-/images/image39.png)



图2.1‑21 控制台日志

**JVM**

选择一个服务器节点，单击当前状态中“JVM”按钮 ![](/articles/cesb/2-/images/image40.png)，查看该服务器节点的JVM状态。

![](/articles/cesb/2-/images/image41.png)



图2.1‑22 JVM内存

** 释放**

选择一个服务器节点，单击当前状态中“删除”按钮![](/articles/cesb/2-/images/image42.png)，弹出确认提示框，单击〖确定〗，完成释放节点，界面如下：

![](/articles/cesb/2-/images/image43.png)





图2.1‑23 释放节点

各字段校验规则如下：

<table>

<tr>

<td></td>

<td>名称</td>

<td>必输项</td>

<td>是否为数字</td>

<td>唯一</td>

<td>其他</td>

</tr>

<tr>

<td>“资源管理”字段设置</td>

<td>主机名</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td></td>

<td>管理服务器名</td>

<td>是</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td></td>

<td>路径</td>

<td>是</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td></td>

<td>主机ip</td>

<td>是</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td></td>

<td>管理端口号</td>

<td></td>

<td>是</td>

<td></td>

<td>【主机IP+管理端口】必须唯一</td>

</tr>

<tr>

<td></td>

<td>http端口号</td>

<td></td>

<td>是</td>

<td></td>

<td>【主机IP+HTTP端口】必须唯一</td>

</tr>

<tr>

<td></td>

<td>JVMID</td>

<td></td>

<td></td>

<td>是</td>

<td></td>

</tr>

<tr>

<td></td>

<td>是否为前置机</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td></td>

<td>热备组号</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td></td>

<td>代理端口</td>

<td>是</td>

<td>是</td>

<td></td>

<td></td>

</tr>

<tr>

<td></td>

<td>JMX端口</td>

<td></td>

<td>是</td>

<td></td>

<td>【主机IP+JMX端口】必须唯一</td>

</tr>

</table>

## 2.1.2 环境部署

### 2.1.2.1 功能介绍

环境部署主要负责部署节点环境，显示管理服务器环境下运行的节点。

### 2.1.2.2 界面说明

单击【资源管理】→【环境部署】进入环境部署界面。用户当前管理的环境的基本信息。

![](/articles/cesb/2-/images/image44.png)





图2.1‑24 环境部署

### 2.1.2.3 操作流程

**新增环境**

单击〖新增环境〗按钮，从右侧滑出窗口，填写相应内容（*表示必填项）后，单击〖确定〗，完成新环境的注册。

![](/articles/cesb/2-/images/image45.png)





图2.1‑25 新增环境

**编辑**

选择一个环境，单击〖编辑〗，从右侧滑出窗口，可修改相应内容（*表示必填项）后，单击〖确定〗，完成修改。

可管理已配置/未配置节点，分配节点权重。

![](/articles/cesb/2-/images/image46.png)





图2.1‑26 编辑环境

**删除**

选择一个环境，单击![](/articles/cesb/2-/images/image47.png)按钮，滑出提示窗口，单击〖确定〗，删除该环境。

![](/articles/cesb/2-/images/image48.png)





图2.1‑27 删除环境























































































