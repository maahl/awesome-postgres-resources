# Awesome PostgreSQL resources
A curated list of awesome resources to understand PostgreSQL. Inspired by [awesome-postgres](https://github.com/dhamaniasad/awesome-postgres)

This is a WIP, contributions are welcome!

## Contents

* [Administration](#administration)
* [Extensions](#extensions)
* [Internals](#internals)
* [SQL](#sql)

## Administration

* [Autovacuum, explained for engineers](http://blog.postgresql-consulting.com/2015/10/autovacuum-explained-for-engineers-new.html)  
  A presentation describing autovacuum.  
  Ilya Kosmodemiansky, 2015

* [Common misconceptions about locking in PostgreSQL](https://www.compose.com/articles/common-misconceptions-about-locking-in-postgresql/)  
  A blog post clarifying locks in PostgreSQL.  
  Robert Wysocki, 2015

* [It's a view, it's a table... no, it's a materialized view!](https://www.compose.com/articles/its-a-view-its-a-table-no-its-a-materialized-view/)  
  A fairly complete introduction to materialized views.  
  Robert Wysocki, 2015

* [Postgres autovacuum is not the enemy](https://www.citusdata.com/blog/2016/11/04/autovacuum-not-the-enemy/)  
  A blog post explaining the rationale behind autovacuum.  
  Joe Nelson, 2016

* [PostgreSQL monitoring cheatsheet](https://russ.garrett.co.uk/2015/10/02/postgres-monitoring-cheatsheet/)  
  A blog post listing some useful metrics when monitoring PostgreSQL.  
  Russ Garett, 2015

* [PostgreSQL primary key type analysis](http://gosimple.me/postgresql-primary-key-type-analysis/)  
  A blog post comparing the performance of primary keys using integer sequences
  and various UUID generation methods.  
  Adam Brusselback, 2016

## Extensions

* [Writing Postgres extensions - the basics](http://big-elephants.com/2015-10/writing-postgres-extensions-part-i/)  
  [Writing Postgres extensions - types and operators](http://big-elephants.com/2015-10/writing-postgres-extensions-part-ii/)  
  [Writing Postgres extensions - debugging](http://big-elephants.com/2015-10/writing-postgres-extensions-part-iii/)  
  [Writing Postgres extensions - testing](http://big-elephants.com/2015-11/writing-postgres-extensions-part-iv/)  
  [Writing Postgres extensions - code organization and versioning](http://big-elephants.com/2015-11/writing-postgres-extensions-part-v/)  
  A series of blog posts that explain in details how to code your own extensions  
  Manuel Kniep and adjust GmbH, 2015

## Internals

* [Access path selection in a relational database management system](https://s3.amazonaws.com/academia.edu.documents/12453180/selinger-etal-1979.pdf?AWSAccessKeyId=AKIAIWOWYYGZ2Y53UL3A&Expires=1524048486&Signature=2e%2Fpd9Wk57zalZ7lwQAixWYl%2FPg%3D&response-content-disposition=inline%3B%20filename%3DAccess_path_selection_in_a_relational_da.pdf)  
  The original article describing the query optimizer dynamic algorithm for join
  order selection, originally implemented in System R but still used in many
  DBMSs, including PostgreSQL.  
  Patricia Selinger et al., 1976

* [All you need to know about sorting in Postgres](https://madusudanan.com/blog/all-you-need-to-know-about-sorting-in-postgres/#DiskMerge)  
  An overview of the sorting algorithms used in PostgreSQL and how PostgreSQL
  chooses which one to use.  
  Madusudanan.B.N, 2016

* [A look at how postgres executes a join](http://patshaughnessy.net/2015/11/24/a-look-at-how-postgres-executes-a-tiny-join)  
  A detailed description of join execution.  
  Pat Shaughnessy, 2015

* [Backend flowchart](https://www.postgresql.org/developer/backend/)  
  A chart describing the role of each component in the backend. Don't forget to
  also check the [full
  index](https://wiki.postgresql.org/wiki/Backend_flowchart#parser) that is
  associated to it.  
  PostgreSQL, 2012

* [Buffer manager](http://www.interdb.jp/pg/pgsql08.html)  
  A detailed description of the cache handling in PostgreSQL.  
  Hironobu Suzuki, 2016

* [Explaining `CREATE INDEX CONCURRENTLY`](http://blog.2ndquadrant.com/create-index-concurrently/)  
  A blog post explaining in great detail how PostgreSQL builds an index without
  locking the table from updates.  
  Pavan Deolasee, 2017

* [Explaining the query optimizer](http://momjian.us/main/writings/pgsql/optimizer.pdf)  
  A presentation introducing the query planner.  
  Bruce Momjian, 2016

* [Explicit locking](https://www.postgresql.org/docs/current/static/explicit-locking.html)  
  The section in PostgreSQL docs that explains the various locks available and
  how they interact with each other.  
  PostgreSQL, current

* [HOT](https://git.postgresql.org/gitweb/?p=postgresql.git;a=blob;f=src/backend/access/heap/README.HOT;hb=HEAD)  
  The readme in the PostgreSQL source code that describes in great details how
  Heap-Only Tuples (HOT) work.  
  PostgreSQL, 2012

* [Index internals](https://www.pgcon.org/2016/schedule/attachments/434_Index-internals-PGCon2016.pdf)  
  A presentation ([video
  available](https://www.youtube.com/watch?v=W6B8-srOsrs)) that describes how
  the different indexes in PostgreSQL store data.  
  Heikki Linnakangas, 2016

* [Introduction to MemoryContexts](http://blog.pgaddict.com/posts/introduction-to-memory-contexts)  
  [AllocationSet internals](http://blog.pgaddict.com/posts/allocation-set-internals)  
  [Examples of palloc overhead](http://blog.pgaddict.com/posts/palloc-overhead-examples)  
  [How much benefit do we get from Allocation set?](http://blog.pgaddict.com/posts/how-much-benefit-do-we-get-from-allocation-set)  
  A series of blog posts explaining the rationale behind `palloc` (postgres'
  replacement of `malloc`), how to use it and its consequences on
  performance.  
  Tomas Vondra, 2014

* [PostgreSQL internals through pictures](https://momjian.us/main/writings/pgsql/internalpics.pdf)  
  A presentation doing a broad overview of PostgreSQL internals.  
  Bruce Momjian, 2016

* [PostgreSQL query optimization](http://jinchengli.me/post/postgres-query-opt/)  
  A blog post introducing query evaluation plans and the algorithm to generate
  them.  
  Jincheng Li, 2016

* [Query execution techniques in PostgreSQL](http://www.neilconway.org/talks/executor.pdf)  
  A presentation that describes how plan nodes are executed.  
  Neil Conway, 2007

## SQL

* [Explanation of jsonb introduced by PostgreSQL](http://stackoverflow.com/a/22910602/2451259)  
  A stackoverflow answer that explains concisely the differences between hstore,
  json and jsonb formats.  
  pozs, 2014

* [PostgreSQL cheat sheet: string functions](http://postgresql-backup.com/postgresql-blog/wp-content/uploads/2016/06/PostgreSQL-Cheat-Sheet_-String-Functions.pdf)  
  A cheat sheet for string operations in PostgreSQL.  
  PostgreSQL Backup, 2016

* [Postgres window magic](http://momjian.us/main/writings/pgsql/window.pdf)  
  A presentation detailing the possibilities of window functions.  
  Bruce Momjian, 2017

* [SQL joins visualizer](http://sql-joins.leopard.in.ua/)  
  Describe the data you want to get from a join using Venn diagrams, and the
  corresponding SQL join is generated.  
  Alexey Vasiliev, 2016
