# 产品优势

## 公有云Redis产品优势

* 高可用：多可用区部署，提供主从热备架构、宕机监测、自动容灾，当发生故障后访问秒级切换至备机。
* 高可靠：持久化数据，提供定时自动备份/手动备份/备份恢复，保证可靠性。
* 高性能：低延迟、高吞吐量。标准版支持8W+QPS，集群版支持千万级QPS。
* 高弹性：提供主从版、集群版实例多规格，控制台提供一键式扩缩容且过程无需停服。
* 易运维：提供托管服务、可视化操作、性能分析、监控报警、参数调优、白名单。
 

## 云Redis与开源Redis差异
相比自搭建Redis数据库，云Redis节省了开发、运维系统带来的人力和时间成本。
| 对比项 |  云缓存Redis  |   自建Redis      |
| :--- | :---  | :---  |
| 高可用	 | 双机热备，自动切换。当主节点发生故障后，从节点会被迅速提升为新的主节点，继续提供服务。	 | 自行安装、配置主从节点。 | 
| 高可靠	 | 服务数据持久化，实例跨可用区部署，保证数据的安全和业务的不间断运行。	 | 自行保障redis服务运行，依赖技术人员的数据库管理水平。 | 
| 高性能	 | 使用内存作为存储介质，利用 Redis 引擎的低延迟、高吞吐量特点，提供比关系型数据库高很多的性能；源码级护航，超高的性能可以满足您绝大部分场景需求；支持绝大多数Redis命令，轻松应对Redis大容量或高性能的业务需求；提供集群版规格扩展Redis性能，破除Redis单线程机制的性能瓶颈。	 | 需要额外自行研究核心代码、开发、维护、解决高速缓存问题。 | 
| 平滑扩容	 | 一键扩容，方便快捷。可根据使用情况弹性扩容，按需选择，按需升级，提高资源利用率，降低冗余费用；您可以登录控制台进行扩容操作，整个过程不影响您的线上业务 | 	在超出容量阈值后，需要新建足量资源、中断应用连接、迁移数据，过程影响业务正常访问。扩展周期长，资源利用率低。 | 
| 大容量	 | 海量存储，无限容量。集群版采用分布式架构，数据分布在多台物理机上，突破单机物理限制，解决海量数据存储在 Redis 上的瓶颈。 | 	受物理内存限制，需要自行解决容量以及稳定性问题。 | 
| 监控告警	 | 为用户提供多种类型的监控，包括如使用量、连接数、QPS、 Key数量等多种监控，可视化数据监控展示。全链路监控预警，帮助您提前预警提示风险、快速定位和解决问题。 | 	需自行开发监控系统，运维人员随时待命。 | 
| 低成本	 | 可轻松部署、运行和扩展缓存Redis，无需机器安装和数据库部署运维等工作；提供资源监控、稳定性维护等功能，降低日常维护工作量 | 	需要专人搭建服务，耗时耗力，人力成本高 | 
| 易运维	 | 提供了可视化易操作的控制台，方便用户快速创建和使用Redis服务，方便用户对缓存参数调优、一键备份恢复、查询大Key热Key、查看客户端IP列表等常见运维操作。提供7*24小时的人工客服和运维保障。 | 	人工运维，自行准备服务器和安装Redis服务。 | 


##  Redis与Memcached对比
目前Memcached的所有功能可视为已成为Redis的子集。二者主要有以下区别。

| 对比项 |  云缓存Redis  |   Memcached      |
| :--- | :---  | :---  |
| 适用场景	 | 数据结构复杂、需要持久化存储数据、存储大key的场景 | 数据结构模型简单，小型静态数据的缓存场景	 | 
| 对集群的支持	 | Redis已支持集群，并提供了标准版和集群版两种架构供用户选择	 | Memcached需要通过第三方集群工具进行管理	 | 
| 数据持久化 | 	支持RDB快照+AOF备份	 | 开源Memcached不支持持久化存储	 | 
| 线程/进程 | 	是单线程模型，采用IO多路复用，但其性能已足够优秀到不会成为瓶颈。	 | 支持多线程，可扩展，理论上性能更高	 | 
| 数据类型 | 支持如字符串（String）、链表（List）、集合（Set）、有序集合（SortedSet）、哈希表（Hash），充分满足业务需求	 | 支持简单的字符串	 | 
|  Lua脚本支持		 | 支持  	 |   不支持。	 | 
| 数据迁移		 | 支持 	 | 	开源Memcached不支持	 | 
| Key的Value限制		 | Key的值最大可以有1G。	 | 1M | 
| 多数据库		 | 	支持。默认0-256个DB。	 | 	不支持	 | 


## 常见问题
**Q：与Memcached相比，Redis具有何种优势？**

A：开源Redis与开源Memcached，可从以下几点来进行对比：
性能上：Memcached支持多线程模型，理论上性能更高。虽然Redis是单线程模型，但其性能已足够优秀到不会成为瓶颈。
功能上：当Redis3.0推出后，可视为Memcached的所有功能已成为Redis的子集。
对集群的支持：Redis已支持集群，并提供了标准版和集群版两种架构供用户选择。而Memcached需要通过第三方集群工具进行管理，因此Redis更具优势。
Redis还具有其它功能优势，如：具有自动淘汰功能、Redis列表类型可实现队列并支持阻塞式读取、Redis支持“发布/订阅”消息模式等。


