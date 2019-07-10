# Azkaban
> Open-source Workflow Manager

## 概述
**`批处理工作流`**  **`用户界面`**  
> Azkaban is a batch workflow job scheduler created at LinkedIn to run Hadoop jobs. Azkaban resolves the ordering through job dependencies and provides an easy to use web user interface to maintain and track your workflows.

## 架构

### Relational Database(MySQL)

### AzkabanWebServer

### AzkabanExecutorServer

## 运行模式

### solo-server
> In solo server mode, the DB is embedded H2 and both web server and executor server run in the same process. 
### multiple-executor
> The multiple executor mode is for most serious production environment. Its DB should be backed by MySQL instances with master-slave set up. The web server and executor servers should ideally run in different hosts so that upgrading and maintenance shouldn’t affect users. This multiple host setup brings in robust and scalable aspect to Azkaban.

## Azkaban实战