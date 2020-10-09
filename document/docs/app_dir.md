# 应用程序基本目录结构



## 目录

[TOC]

## 一、概述

本文介绍应用程序的目录、文件结构规划及命名推荐方案。

- 目录命名

- 目录结构

- 文件命名

## 二、详细

1. 目录命名

应用程序目录命名采用`apache`项目命名规则。应用程序名分为两部分，用横杠分隔，左侧为主项目名称，右侧为模块名称。鉴于目前项目团队的规模和人数，认为项目分两层即可，更多的层次可以在下层自行建立和管理。

例如: 

- `common-io`

- `common-collection`

- `common-net`

对应的命名空间为: 

- `com.winning.dcs.common.io`

- `com.winning.dcs.common.collection`

- `com.winning.dcs.common.net`

2. 目录结构

主目录结构大致如下: 

~~~dir
└─sql-backup
    ├─bin
    │      sql-backup-csv-reset.sh
    │      sql-backup-csv.sh
    |      datax.sh
    ├─config
    │      SQL_BACKUP.csv
    │      application-prod.yml
    ├─lib
    |       sql-backup.jar
    | 		log4j.jar
    ├─ data
    |      CLINICAL_SERVICE_MEDICATION.json   
    |      DMH_EMPLOYEE.json                   
    |      DMH_RIS_REPORT_RESULT.json
    |      ... ...
    └─
~~~

3. 命名规则

	- 目录及可执行文件: 这类文件经常需要用户通过键盘访问或执行。应尽量采用`小写字母`，`横杠`分隔，这样降低了敲击难度。这些文件命名应采用一定的规律性，便于用户记忆和识别。
	- 数据文件: 用户通常不会通过命令访问，而主要编辑内容。这类可以`大写字母`加`下划线`分隔，增加明显可辨识性，且不易输入，避免误操作。
	- 框架要求的文件: 例如`application-prod.yml`这类框架要求在固定的目录和命名，应`遵循框架约定`。

4. 目录解释

    - `sql-backup:` 为项目名，其下包含: 
        - `bin`: 可执行目录，放二进制文件或脚本
            - `sql-backup-csv-reset.sh` 需要用户来执行脚本，因此命名遵循某种一致性规则
            - `sql-backup-csv.sh` 需要用户来执行的脚本，因此命名遵循某种一致性规则
            - `datax.sh` 涉及第三方的工具脚本，被脚本调用，保持原有的命名和含义
        - `config`: 配置目录，放置配置文件
            - `SQL_BACKUP.csv` 数据文件，采用大写加下划线
            - `applicaiton-prod.yml` 配置文件，遵循框架的写法
        - lib: 类库目录，放置类库
            - `sql-backup.jar` 主程序，与项目名保持一致便于辨识
            - `log4j.jar` 第三方类库
        - data: 数据目录，放置数据
            - `CLINICAL_SERVICE_MEDICATION.jso` 数据文件，采用大写字母，下划线分隔

## 三、关于

- 撰写: tlw
- 日志: 
	- 20200825： 创建


