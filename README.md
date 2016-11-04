# Awesome PostgreSQL resources
A curated list of awesome PostgreSQL resources to understand PostgreSQL. Inspired by [awesome-postgres](https://github.com/dhamaniasad/awesome-postgres)

This is a WIP, contributions are welcome!

## Contents
* [Administration](#administration)
* [Internals](#internals)
* [SQL](#sql)

## Administration
* [Autovacuum, explained for engineers](http://blog.postgresql-consulting.com/2015/10/autovacuum-explained-for-engineers-new.html) - A presentation describing autovacuum. Ilya Kosmodemiansky, 2015
* [PostgreSQL monitoring cheatsheet](https://russ.garrett.co.uk/2015/10/02/postgres-monitoring-cheatsheet/) - A blog post listing some useful metrics when monitoring PostgreSQL. Russ Garett, 2015

## Internals
* [Backend flowchart](https://www.postgresql.org/developer/backend/) - A chart describing the role of each component in the backend. Don't forget to also check the [full index](https://wiki.postgresql.org/wiki/Backend_flowchart#parser) that is associated to it. PostgreSQL, 2012
* [Explaining the query optimizer](http://momjian.us/main/writings/pgsql/optimizer.pdf) - A presentation introducing the query planner. Bruce Momjian, 2016
* [HOT](https://git.postgresql.org/gitweb/?p=postgresql.git;a=blob;f=src/backend/access/heap/README.HOT;hb=HEAD) - The readme in the PostgreSQL source code that describes in great details how Heap-Only Tuples (HOT) work. PostgreSQL, 2012
* [Index internals](https://www.pgcon.org/2016/schedule/attachments/434_Index-internals-PGCon2016.pdf) - A presentation ([video available](https://www.youtube.com/watch?v=W6B8-srOsrs)) that describes how the different indexes in PostgreSQL store data. Heikki Linnakangas, 2016
* [PostgreSQL internals through pictures](https://momjian.us/main/writings/pgsql/internalpics.pdf) - A presentation doing a broad overview of PostgreSQL internals. Bruce Momjian, 2016
* [PostgreSQL query optimization](http://jinchengli.me/post/postgres-query-opt/) - A blog post introducing query evaluation plans and the algorithm to generate them. Jincheng Li, 2016
* [Query execution techniques in PostgreSQL](http://www.neilconway.org/talks/executor.pdf) - A presentation that describes how plan nodes are executed. Neil Conway, 2007

## SQL
* [SQL joins visualizer](http://sql-joins.leopard.in.ua/) - Describe the data you want to get from a join using Venn diagrams, and the corresponding SQL join is generated. Alexey Vasiliev, 2016
