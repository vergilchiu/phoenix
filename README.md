<!--
Licensed to the Apache Software Foundation (ASF) under one or more
contributor license agreements.  See the NOTICE file distributed with
this work for additional information regarding copyright ownership.
The ASF licenses this file to You under the Apache License, Version 2.0
(the "License"); you may not use this file except in compliance with
the License.  You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->

![logo](http://phoenix.apache.org/images/logo.png)

<b>[Apache Phoenix](http://phoenix.apache.org/)</b> is a SQL skin over HBase delivered as a client-embedded JDBC driver targeting low latency queries over HBase data. Visit the Apache Phoenix website <b>[here](http://phoenix.apache.org/)</b>.

Copyright ©2014 [Apache Software Foundation](http://www.apache.org/). All Rights Reserved. 

Phoenix4.11-hbase1.2 修改记录  
====================

|序号|项目|类|方法|行号|修改说明| 
|---|---|---|---|---|---|  
|201707-01|Phoenix|pom|-|73|修改hive的版本到2.3.0|
|201707-02|Phoenix-hive|IndexPredicateAnalyzer|analyzeExpr,createAnalyzer|364,523|where条件增加like表达式处理方式|
|201707-03|Phoenix-hive|PhoenixInputFormat|getSplits|108|修改老版本的序列化反序列化工具|
|201707-04|Phoenix-hive|PhoenixQueryBUilder|Expression|709|增加like表达式|
|201707-05|Phoenix-hive|PhoenixStorageHandler|getSerDeClass|233|修改老版本获取序列化方法错误问题|
|201707-06|Phoenix-hive|PhoenixInputFormat|getSplits|104|增加spark客户端判断|
|201707-07|Phoenix-core|IndexTool|run|492,528,602|修复phoenix表名为小写，批量建立索引失败|