# chappe-telegraph

This repo contains minor improvements that could potentially be made for the book [*Aeon's Surreal Renaissance*](https://surrealdb.com/learn/book) after reading it (2024/Oct/22).

## ch01
* The code block is not wrapped in the appropriate CSS class. [(Link)](https://surrealdb.com/learn/book/chapter-01#installing-starting-and-connecting-to-surrealdb)

![](./img/ch01/01-code-block.png)

## ch03
* Duplicated dot. [(Link)](https://surrealdb.com/learn/book/chapter-03#surrealdb-architecture)

![](./img/ch03/01-dup-dot.png)

* `town` field should be `population` field. [(Link)](https://surrealdb.com/learn/book/chapter-03#the-null-and-none-types)

![](./img/ch03/02-field.png)


* `WHEN` should be `WHERE`. [(Link)](https://surrealdb.com/learn/book/chapter-03#5-how-would-you-then-return-all-of-these-towns-if-their-name-is-greater-than-the-value-m)

![](./img/ch03/03-q5.png)


## ch04
* The bottom `person:7ykci42eb08vszvcur2t` is not highlighted in blue like the top one. [(Link)](https://surrealdb.com/learn/book/chapter-04#returning-before-after-and-more)

![](./img/ch04/01-color.png)


* `$town` is not highlighted. [(Link)](https://surrealdb.com/learn/book/chapter-04#for-loops)

![](./img/ch04/02-highlight.png)

* `string::is::datetime(` is not properly formatted. [(Link)](https://surrealdb.com/learn/book/chapter-04#datetimes-string-prefixes-durations-and-sleeping)

![](./img/ch04/03-fmt.png)


## ch05
* I suggest using `TABLE` consistently instead of `table` in this schema only.
[(Link)](https://surrealdb.com/learn/book/chapter-05#schema-basics)

![](./img/ch05/01-table.png)

* Using `INFO FOR TABLE` would be preferable to using `INFO FOR table`.
[(Link)](https://surrealdb.com/learn/book/chapter-05#info-for-table-and-properties-inside-arrays)

![](./img/ch05/02-table.png)

## ch06
* Query should be `UPDATE person:the_nobleman SET children = [person:wulfield];`.
[(Link)](https://surrealdb.com/learn/book/chapter-06#relate)

![](./img/ch06/01-sql.png)

## ch07
* Typo: `hearn` should be `heard`.
[(Link)](https://surrealdb.com/learn/book/chapter-07#more-advanced-relational-queries)

![](./img/ch07/01-typo.png)

## ch09
* The code block is not wrapped in the appropriate CSS class.
[(Link)](https://surrealdb.com/learn/book/chapter-09#strictness-across-the-entire-database)

![](./img/ch09/01-code-block.png)

## ch10
* Rendering issue here.
[(Link)](https://surrealdb.com/learn/book/chapter-10#geo-functions)


![](./img/ch10/01-render.png)


* `651898892358.2931f` is not highlighted.
[(Link)](https://surrealdb.com/learn/book/chapter-10#geo-functions)


![](./img/ch10/02-highlight.png)


* `..>` should be `>..`.
[(Link)](https://surrealdb.com/learn/book/chapter-10#comparing-values-and-complex-record-id-behaviour)

![](./img/ch10/03-typo.png)


## ch12
* `backticks` issue here.
[(Link)](https://surrealdb.com/learn/book/chapter-12#changefeeds-and-the-show-statement)

![](./img/ch12/01-backtick.png)

* Extra line. 
[(Link)](https://surrealdb.com/learn/book/chapter-12#3-the-following-data-is-divided-into-planet-star-and-moon-record-types-using-method-syntax-how-could-you-combine-them-into-a-single-array-of-objects-that-has-the-table-name-as-the-type-and-the-table-id-as-its-name)

![](./img/ch12/02-extra-line.png)


## ch14

* This chapter utilizes [this dataset](https://datasets.surrealdb.com/learn/book/book-part-8-dataset.surql). However, to achieve the results shown below, we need to add `DEFINE FIELD name ON TABLE building TYPE string;`.
[(Link)](https://surrealdb.com/learn/book/chapter-14#using-the-explorer-view-to-visualize-relations)

![](./img/ch14/01-define-field.png)

## ch17
* Rendering issue here. [(Link)](https://surrealdb.com/learn/book/chapter-17#viewing-external-dependencies-inside-cargotoml)

![](./img/ch17/01-render.png)

## ch18
* It appears that `RETURN (SELECT VALUE languages FROM movie).distinct().flatten();` (incorrect) is not equivalent to `RETURN (SELECT VALUE languages FROM movie).flatten().distinct();` (correct).
[(Link)](https://surrealdb.com/learn/book/chapter-18#genres-languages)

![](./img/ch18/01-sql.png)
* This chapter utilizes [this dataset](https://datasets.surrealdb.com/learn/book/book-naive-movies.surql) that contains `NONE` in the `Language` field, which is quite interesting.
```
{
		Actors: 'Charles Chaplin, Virginia Cherrill, Florence Lee',
		Awards: '3 wins & 1 nomination',
		BoxOffice: '$19,181',
		Country: 'United States',
		DVD: '23 Feb 2010',
		Director: 'Charles Chaplin',
		Genre: 'Comedy, Drama, Romance',
		Language: 'None, English',
        ...
}
```

## ch21

* Typo: duplicated `"think"`. [(Link)](https://surrealdb.com/learn/book/chapter-21#a-farewell-to-failure)

![](./img/ch21/01-typo.png)