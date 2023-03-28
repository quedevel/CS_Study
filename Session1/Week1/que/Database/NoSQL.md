# 🎯 SQL vs NoSQL
- - -
<br>

### **_SQL(Structured Query Language)_**
- - -
SQL(Structured Query Language)은 관계형 데이터베이스에서 사용하는 쿼리 언어입니다. 
SQL을 사용하면 데이터베이스에 저장된 데이터를 검색하거나 조작하는 등의 작업을 할 수 있습니다. 
SQL은 데이터의 구조와 유형을 정의하고, 데이터를 삽입, 수정, 삭제, 검색하는데 사용됩니다. 
SQL은 데이터베이스의 스키마를 정의하는 데이터 정의 언어(DDL), 데이터를 조작하는 데이터 조작 언어(DML), 데이터를 검색하는 데이터 검색 언어(DQL), 데이터를 제어하는 데이터 제어 언어(DCL)로 구성되어 있습니다. 
SQL은 대부분의 관계형 데이터베이스 관리 시스템(RDBMS)에서 지원됩니다. <br>

<span style="font-size: 20px">**⭐️ SQL의 장점**</span> <br>

1.  관계형 데이터베이스의 가장 강력한 특징인 데이터의 일관성과 무결성을 보장합니다.
2.  데이터베이스 구조가 확실하게 정의되어 있어 데이터베이스 설계와 운영이 비교적 쉽습니다.
3.  SQL의 문법이 직관적이고 간결하기 때문에 비교적 쉽게 배울 수 있습니다.
4.  데이터 검색, 필터링, 정렬, 그룹핑 등 다양한 데이터 처리 기능을 제공합니다.

<span style="font-size: 20px">**💀️ SQL의 단점**</span> <br>
1. **고정된 스키마**
   * SQL 데이터베이스는 미리 정의된 스키마를 사용합니다. 따라서 데이터 스키마가 변경될 경우, 모든 데이터베이스 테이블을 수정해야 합니다. 이는 스키마 변경이 빈번한 경우 문제가 될 수 있습니다.
2. **수직적 확장 어려움**
   * SQL 데이터베이스는 일반적으로 단일 서버에서 작동하며, 서버 용량이 한계에 도달하면 성능이 저하됩니다. 대규모 트래픽이 발생하는 경우, 서버의 성능을 높이기 위해 비싼 하드웨어를 구입하거나, 수직적으로 확장하는 방법밖에 없습니다.
3. **높은 유지보수 비용**
   * SQL 데이터베이스의 경우, 데이터 구조와 스키마를 설계하고 유지보수하는 데 많은 시간과 비용이 들어갑니다. 따라서 작은 규모의 프로젝트나 개인적인 목적으로 사용하기에는 비용 대비 효율이 떨어질 수 있습니다.
4. **복잡한 조인 작업**
   * SQL 데이터베이스에서는 여러 테이블을 조인해야 하는 경우가 많습니다. 하지만 이러한 조인 작업은 매우 복잡하며, 처리 속도가 느릴 수 있습니다.
5. **스키마 수정이 어려움**
   * SQL 데이터베이스에서는 스키마 변경이 매우 어렵습니다. 따라서 스키마 수정을 할 때마다 대규모의 데이터를 백업하고, 다시 복원해야 하는 등 복잡한 과정을 거쳐야 합니다.

<br>

### **_NoSQL(Not Only SQL)_**
- - -
NoSQL은 "Not Only SQL"의 약어로, 관계형 데이터베이스 모델과 달리 스키마를 미리 정의하지 않는 비관계형 데이터베이스 모델을 말합니다. 
NoSQL 데이터베이스는 데이터 구조와 속성이 다양하며, 수평적으로 확장이 가능한 분산 시스템 아키텍처를 가집니다.

#### NoSQL은 크게 4가지 유형으로 분류됩니다.

1. **Key-Value Stores**
   * 각각의 아이템이 key와 value로 저장되는 데이터 모델입니다. Redis, Riak 등이 이 유형에 해당됩니다.
2. **Document Databases**
   * key-value stores와 유사하지만, value가 구조화된 문서일 수 있습니다. MongoDB, CouchDB 등이 이 유형에 해당됩니다.
3. **Column-Family Stores**
   * BigTable 데이터 모델을 기반으로 하며, 여러 개의 column으로 이루어진 레코드를 저장합니다. Cassandra, HBase 등이 이 유형에 해당됩니다.
4. **Graph Databases**
   * 데이터를 노드(node)와 엣지(edge)의 그래프 형태로 저장합니다. Neo4j, OrientDB 등이 이 유형에 해당됩니다.


<span style="font-size: 20px">**⭐️ NoSQL의 장점**</span> <br>

1. **유연성**
   * 데이터 모델이 미리 정의되어 있지 않아서 새로운 속성을 추가하거나 삭제할 때 유연합니다.
2. **확장성**
   * 수평적으로 쉽게 확장이 가능합니다.
3. **높은 가용성**
   * 분산 시스템 아키텍처를 가지고 있어서 장애가 발생해도 데이터 유실이 발생하지 않습니다.
4. **빠른 처리 속도**
   * 대부분의 NoSQL은 메모리에 데이터를 저장하기 때문에 빠른 응답 속도를 가지고 있습니다.


<span style="font-size: 20px">**💀️ NoSQL의 단점**</span> <br>

1. **한계된 기능**
   * NoSQL은 각각의 유형에 따라 특화된 기능을 가지고 있어서 특정한 작업에 적합하지만, 모든 작업에 대해서는 SQL보다 제한적인 기능을 가지고 있습니다.
2. **데이터 일관성 보장 어려움**
   * 데이터 일관성이 보장되지 않는 경우가 있습니다.
3. **학습 비용**
   * SQL보다 NoSQL을 학습하는 데 높은 비용이 필요합니다.

<br>

### **_SQL vs NoSQL_**
- - -

SQL과 NoSQL은 각각 결정할 때 몇 가지 요소를 고려해야 합니다.

1. **데이터 구조와 스키마**
   * SQL은 관계형 데이터베이스로 구조화된 데이터를 다루는 데 적합합니다. 스키마가 명확하게 정의되어 있고, 관계가 복잡한 데이터를 다루는 데 용이합니다. 반면 NoSQL은 스키마가 유연하고 자유로운 형태로 데이터를 저장할 수 있습니다. 데이터의 구조가 불명확하거나 변경 가능성이 높은 경우 NoSQL을 사용하는 것이 좋습니다.
2. **데이터 양과 처리 속도**
   * 대용량 데이터 처리와 빠른 읽기/쓰기 속도를 요구하는 경우 NoSQL이 적합합니다. NoSQL은 수평적 확장이 용이하고 분산 처리에 적합한 구조를 가지고 있습니다. SQL은 대용량 데이터 처리에도 적합하지만, NoSQL보다는 처리 속도가 느리고, 수직적 확장에 한계가 있을 수 있습니다.
3. **트랜잭션 처리와 일관성**
   * SQL은 ACID(원자성, 일관성, 고립성, 지속성) 트랜잭션을 지원하며, 데이터 일관성과 무결성을 보장합니다. 따라서 데이터의 일관성이 매우 중요한 경우 SQL을 사용하는 것이 좋습니다. NoSQL은 일관성이 보장되지 않을 수 있지만, 대신 분산 처리가 용이하고, 확장성과 가용성이 높습니다.
4. **개발자 및 인프라 역량**
   * SQL과 NoSQL은 각각 다른 개발 및 운영 방식이 필요합니다. SQL은 관계형 모델과 SQL 쿼리를 다루는 데에 높은 역량이 필요하고, 대용량 처리를 위해 복잡한 인프라를 구축해야 할 수도 있습니다. NoSQL은 각 데이터베이스마다 다른 문법과 API를 가지고 있으며, 복잡한 인프라를 구축할 필요는 없지만, 분산 처리 및 운영 경험이 필요합니다.