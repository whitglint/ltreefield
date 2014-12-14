ltreefield
==========

Django Field class for PostgreSQL ltree data type.

Class
-----
LtreeField

Lookups
-------
* aore
  * ltree @> ltree
  * is left argument an ancestor of right (or equal)?
* dore
  * ltree <@ ltree
  * is left argument a descendant of right (or equal)?
* match
  * ltree ~ lquery
  * does ltree match lquery?

Usage
-----
```python
path__aore='Top.Science' # path @> 'Top.Science'
path__dore='Top.Science' # path <@ 'Top.Science'
path__match='*.Astronomy.*' # path ~ '*.Astronomy.*'
```

Reference
---------
[PostgreSQL: Documentation: 9.3: ltree](http://www.postgresql.org/docs/9.3/static/ltree.html)
