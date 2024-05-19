---
layout: page
title: RookieDB
description: A Java-based SQL database system
img: assets/img/rookie_db.jpg
importance: 1
category: School Projects
related_publications: false
---

## Overview
[RookieDB](https://cs186.gitbook.io/project) is a bare-bones database implementation supporting the execution of simple transactions in series. Throughout this project, I added support for B+ tree indices, efficient join algorithms, query optimization, multigranularity locking to allow concurrent execution of transactions, and database recovery.

## Project Details

### 1. B+ Tree Indices
In the first part, I implemented B+ tree indices, which are crucial for efficient data retrieval. The key components include:
- **DataBox**: Represents data types (Boolean, Int, Float, Long, String) in RookieDB.
- **RecordId**: Identifies a record by its page and entry number.
- **BPlusTree, BPlusNode, LeafNode, InnerNode**: Classes to manage the structure and operations of the B+ tree.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/b_plus_tree.jpg" title="B+ Tree Structure" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### 2. Efficient Join Algorithms
Implemented join algorithms to optimize query execution:
- **Block Nested Loop Join (BNLJ)**: Efficiently joins large tables by using blocks of data pages.
- **Grace Hash Join (GHJ)**: Uses hash partitioning to manage memory efficiently during join operations.
- **Sort Merge Join (SMJ)**: Sorts and merges tables to perform joins.

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/BNLJ.gif" title="Block Nested Loop Join GIF" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### 3. Query Optimization
Developed query optimization techniques to improve the efficiency of database operations:
- **Single Table Access Selection**: Chooses the optimal way to access single tables.
- **Join Selection**: Selects the best join order and method.
- **Cost-Based Optimization**: Utilizes cost estimates to determine the most efficient query execution plan.


### 4. Multigranularity Locking
Implemented a locking mechanism to ensure transaction isolation and consistency:
- **Lock Types**: S (shared), X (exclusive), IS (intent shared), IX (intent exclusive), SIX (shared with intent exclusive).
- **Lock Manager**: Manages locks and enforces multigranularity constraints.
- **LockContext**: Represents resources in the hierarchy and handles locking at different levels.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lock_escalate.jpg" title="Multigranularity Lock Escalate" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### 5. Database Recovery
Ensured the database can recover from crashes while maintaining ACID properties:
- **Write-Ahead Logging (WAL)**: Logs changes before applying them to the database.
- **Checkpointing**: Periodically saves the state of the database to reduce recovery time.
- **ARIES Recovery Algorithm**: Utilizes analysis, redo, and undo phases to restore the database to a consistent state.


### 6. NoSQL Features
Explored NoSQL features by working with a document-based database:
- **Handling Documents**: Managed collections of documents with fields that are not primitive data types.
- **Aggregation Framework**: Used MongoDB’s aggregation framework to perform complex data queries and transformations.
- **Query Examples**: Demonstrated complex queries involving match, group, sort, limit, lookup, and project stages.


## Conclusion
RookieDB provided a comprehensive experience in building a fully functional database system. From implementing fundamental data structures like B+ trees to ensuring robust transaction management with locking and recovery mechanisms, this project encompassed a wide range of essential database concepts and techniques.


## Acknowledgments
- Project address: [https://cs186.gitbook.io/project](https://cs186.gitbook.io/project)
- Image sources: [cs186.gitbook.io/project](https://cs186.gitbook.io/project)