# Pgcli

## Documentaiton

[Documentation](https://www.pgcli.com/)

## Commands

### Fuzzy Search Commands Executed

`<Ctrl> + r`: enter text and search latest command  with arrows or `<Ctrl> + r`

### Named Queries (alias queries)

1. `\n`: list all named queries.
2. `\n <name>`: Invoke a named query by its name.
3. `\n <name> <query>`: Saved a new named query called `name`
4. `\nd <name>`: Delete an axisting named query by its name.

### Positional Parameters

Named queries support shell-style parameter substitution. Save your named query with parameters as placeholders (e.g. $1, $2, $3, etc.)

**Example**

`\ns user_by_name select * from users where name = '$1'`

When you call a named query with parameters, just add the parameters after the query's name. You can put quotes around arguments that include spaces.

`\n user_by_name "Skelly McDermott"\n`

### Clear Screen

`Ctrl + L`

### Formating output to column_name-value

1. `\x`: Set formatting output
2. `SELECT ...`: Execute any queries and ger formating results
3. `\x`: Disable formating output




