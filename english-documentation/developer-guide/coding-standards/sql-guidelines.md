# SQL Guidelines

## Table names <a href="#sqlguidelines-tablenames" id="sqlguidelines-tablenames"></a>

1.  Table names must begin with the PrestaShop "`_DB_PREFIX_`" prefix.

    ```
    ... FROM `'. _DB_PREFIX_.'customer` ...
    ```
2. Table names must have the same name as the object they reflect: "`ps_cart`".
3. Table names have to stay singular: "`ps_order`".
4. Language data have to be stored in a table named exactly like the object's table, and with the "`_lang`" suffix: "`ps_product_lang`".

## SQL query <a href="#sqlguidelines-sqlquery" id="sqlguidelines-sqlquery"></a>

1.  Keywords must be written in uppercase.

    ```
    SELECT `firstname`
    FROM `'._DB_PREFIX_.'customer`
    ```
2.  Back quotes ("`` ` ``") must be used around SQL field names and table names.

    ```
    SELECT p.`foo`, c.`bar`
    FROM `'._DB_PREFIX_.'product` p, `'._DB_PREFIX_.'customer` c
    ```
3.  Table aliases have to be named by taking the first letter of each word, and must be lowercase.

    ```
    SELECT p.`id_product`, pl.`name`
    FROM `'._DB_PREFIX_.'product` p
    NATURAL JOIN `'._DB_PREFIX_.'product_lang` pl
    ```
4.  When conflicts between table aliases occur, the second character has to be also used in the name.

    ```
    SELECT ca.`id_product`, cu.`firstname`
    FROM `'._DB_PREFIX_.'cart` ca, `'._DB_PREFIX_.'customer` cu
    ```
5.  A new line has to be created for each clause.

    ```
    $query = 'SELECT pl.`name`
    FROM `'._DB_PREFIX_.'product_lang` pl
    WHERE pl.`id_product` = 17';
    ```
6. It is forbidden to make a `JOIN` in a `WHERE` clause.
