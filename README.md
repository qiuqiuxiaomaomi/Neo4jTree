# Neo4jTree
图数据库

![](https://i.imgur.com/Z9ject0.png)

<pre>
CREATE 
 (p1:Person {name:'胡兴炯', born:1991, interest:'mac,ios,旅游', goodat:'java,swift,objectiveC'}),
 (p2:Person {name:'张勇', born:1990,  interest:'android', goodat:'java,android'}),
 (p3:Person {name:'成文龙', born:1990, interest:'linux,hadoop', goodat:'linux,java,android'}),
 (p4:Person {name:'王昕', born:1978, interest:'wpf,noSQL,旅游', goodat:'java,c#'}),
 (p5:Person {name:'周开琪', born:1977 , interest:'管理', goodat:'管理,'}),
 (p6:Person {name:'徐锦亮', born:1985,  interest:'前端', goodat:'前端，html5,hadoop'}),
 (p7:Person {name:'张三', born:1993,  interest:'大数据', goodat:'hadoop，html5,java,lucene,elasticsearch,solr'}),
 (p8:Person {name:'徐辉霞', born:1990,  interest:'管理,旅游', goodat:'管理,采购'}),
 (p9:Person {name:'黄廷鹏', born:1992,  interest:'OA', goodat:'java'}),
 (p10:Person {name:'史乐乐', born:1991,  interest:'OA,旅游', goodat:'管理'}),
 (p1)-[:认识]->(p2),
 (p1)-[:认识]->(p3),
 (p1)-[:认识]->(p4),
 (p1)-[:认识]->(p5),
 (p1)-[:认识]->(p9),
 (p2)-[:认识]->(p1),
 (p2)-[:认识]->(p3),
 (p2)-[:认识]->(p4),
 (p2)-[:认识]->(p5),
 (p2)-[:认识]->(p9),
 (p3)-[:认识]->(p1),
 (p3)-[:认识]->(p2),
 (p3)-[:认识]->(p4),
 (p3)-[:认识]->(p5),
 (p3)-[:认识]->(p7),
 (p4)-[:认识]->(p1),
 (p4)-[:认识]->(p2),
 (p4)-[:认识]->(p3),
 (p4)-[:认识]->(p5),
 (p4)-[:认识]->(p9),
 (p5)-[:认识]->(p1),
 (p5)-[:认识]->(p2),
 (p5)-[:认识]->(p3),
 (p5)-[:认识]->(p4),
 (p5)-[:认识]->(p6),
 (p5)-[:认识]->(p8),
 (p5)-[:管理]->(p1),
 (p5)-[:管理]->(p2),
 (p5)-[:管理]->(p3),
 (p5)-[:管理]->(p4),
 (p5)-[:管理]->(p6),
 (p6)-[:认识]->(p5),
 (p6)-[:认识]->(p4),
 (p6)-[:夫妻]->(p8),
 (p9)-[:认识]->(p1),
 (p9)-[:认识]->(p2),
 (p9)-[:认识]->(p3),
 (p9)-[:认识]->(p10),
 (p9)-[:喜欢]->(p10),
 (p10)-[:认识]->(p9),
 (p10)-[:同事]->(p7)
</pre>

![](https://i.imgur.com/ZdQ1Pu0.png)

<pre>
CREATE
(p112:Artist {name:'周杰伦',nation:'中国台湾'}),
(p208:Artist {name:'王菲',nation:'中国'}),
(p263:Artist {name:'刘若英',nation:'中国台湾'}),
(p292:Artist {name:'谢霆锋',nation:'中国香港'}),
(p529:Artist {name:'五月天',nation:'中国台湾'}),
(p581:Artist {name:'孙俪',nation:'中国'}),
(p621:Artist {name:'窦唯',nation:'中国'}),
(p1590:Artist {name:'戚薇',nation:'中国'}),
(p1719:Artist {name:'黄家强',nation:'中国香港'}),
(p5787:Artist {name:'Jay-Z',nation:'美国'}),
(p17796:Artist {name:'邓超',nation:'中国'}),
(p24680:Artist {name:'GALA3',nation:'中国'}),
(p27039:Artist {name:'黄秋生',nation:'中国香港'}),
(p29774:Artist {name:'Beyonce',nation:'美国'}),
(p31323:Artist {name:'Louis Armstrong',nation:'美国'}),
(p51584:Artist {name:'Toshiko Akiyoshi',nation:''}),
(p63216:Artist {name:'陈建州',nation:'中国台湾'}),
(p314315:Artist {name:'Steve Howe',nation:'英国'}),
(p692280:Artist {name:'泰歌',nation:'中国'}),
(p1000000391:Artist {name:'黄家驹',nation:'中国香港'}),
(p1000000461:Artist {name:'李宗盛',nation:'中国台湾'}),
(p1000004479:Artist {name:'秋元康',nation:'日本'}),
(p1000055076:Artist {name:'初音未来',nation:'日本'}),
(p1000089993:Artist {name:'小花',nation:'中国'}),
(p1000093632:Artist {name:'李承铉',nation:'美国'}),
(p1000099804:Artist {name:'AKB48',nation:'日本'}),
(p1000596481:Artist {name:'窦靖童',nation:'中国'}),
(p1000601602:Artist {name:'小臭臭',nation:'中国'}),
(p1001205604:Artist {name:'NMB48',nation:'日本'}),
(p1001215412:Artist {name:'Blue Ivy',nation:'美国'}),
(p1001485615:Artist {name:'侯佩岑',nation:'中国台湾'}),
(p1001640975:Artist {name:'Way Out West',nation:'英国'}),
(p1001658350:Artist {name:'Charlie Mariano',nation:'美国'}),
(p1002146850:Artist {name:'昆凌',nation:'中国台湾'}),
(p1003058140:Artist {name:'Velma Middleton',nation:'美国'}),
(p1003175970:Artist {name:'刘耕宏',nation:''}),
(p1004640626:Artist {name:'Nick Warren',nation:'英国'}),
(p1104958835:Artist {name:'DECO*27',nation:'日本'}),
(p1104992642:Artist {name:'doriko',nation:'日本'}),
(p1106590248:Artist {name:'藤田咲 ',nation:'日本'}),
(p1106931509:Artist {name:'等等',nation:'中国'}),
(p1107088425:Artist {name:'Virgil Howe',nation:'英国'}),
(p1109265737:Artist {name:'Afilia Saga',nation:'日本'}),
(p29774)-[:母女]->(p1001215412),
(p5787)-[:父女]->(p1001215412),
(p17796)-[:父子]->(p1106931509),
(p581)-[:母子]->(p1106931509),
(p314315)-[:父子]->(p1107088425),
(p17796)-[:父女]->(p1000089993),
(p581)-[:母女]->(p1000089993),
(p1106590248)-[:中之人]->(p1000055076),
(p1104958835)-[:制作人]->(p1000055076),
(p1104992642)-[:制作人]->(p1000055076),
(p1000004479)-[:制作人]->(p1000099804),
(p51584)-[:妻子]->(p1001658350),
(p292)-[:男朋友]->(p208),
(p621)-[:前夫]->(p208),
(p1000596481)-[:女儿]->(p208),
(p1000000461)-[:老师]->(p529),
(p24680)-[:好友]->(p529),
(p263)-[:好友]->(p529),
(p692280)-[:父女]->(p1000601602),
(p1109938911)-[:制作人]->(p1109265737),
(p1000093632)-[:夫妻]->(p1590),
(p1000004479)-[:制作人]->(p1001205604),
(p208)-[:母女]->(p1000596481),
(p621)-[:父女]->(p1000596481),
(p1002146850)-[:妻子]->(p112),
(p1001485615)-[:前女友]->(p112),
(p27039)-[:义父]->(p112),
(p1003175970)-[:好友]->(p112),
(p63216)-[:好友]->(p112),
(p1719)-[:弟弟]->(p1000000391)
</pre>

Neo4j的关系存储示意图

![](https://i.imgur.com/pPNI06e.png)

从一个节点开始遍历它的所有关系

<pre>
Neo4j是一个高性能的NoSQL图形数据库，它将结构化数据存储在网络上而不是表中，Neo4j也可以被
看做是一个高性能的图引擎，该引擎具有成熟数据库的所有特性，程序员工作在一个面向对象的，灵活
的网络结构下而不是严格的，静态的表中----但是他们可以享受到具备完全的事务特性，企业级的数据
库的所有好处。

Neo4j因其嵌入式，高性能，轻量级等优势，备受关注

图形数据库
       在一个图中包含两种基本的数据类型: Nodes（节点）, RelationShips（关系）
       Nodes和RelationShips包含key/value形式的属性，Nodes通过RelationShips所定义的
    关系相连起来，形成关系型网络结构。
    从这几个方面来说，	Neo4j是一个合适的选择
        1) 自带一套易于学习的查询语言
        2）不使用schema，因此可以满足你任何形式的需求
        3）与关系型数据库相比，对于高度关联的数据（图形数据）的查询速度要快上许多
        5）它的实体与关系结构非常自然的契合人类的直观感受
        6）支持兼容的ACID的事务模型
        7）提供了一个高可用性模型，以支持大规模数据量的查询，支持备份，数据局部性以及冗余
        8）提供了一个可视化的查询控制台

</pre>
