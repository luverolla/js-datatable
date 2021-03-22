# JS DataTable
Pure JavaScript (VanillaJS) component that transforms simple html tables, into fully-interactive and accessible datatables with sorting, searching and paging features.

## How to use
To use the datatable plugins, two main file must be included.
The stylesheet:
```html
<link rel="stylesheet" href="/js-datatable/dist/css/datatable.min.css" />
```
And the script file (inclusive of all language files)
```html
<script src="/js-datatable/dist/datatable.min.js"></script>
```
The table must be wrapped correcty as the following example
```html
<table data-replace="jtable" data-search="true" data-locale="en">
    <thead>
        <tr>
            <th>Name</th>
            <th>Surname</th>
            <th>Age</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Mario</td>
            <td>Rossi</td>
            <td>20</td>
        </tr>
    </tbody>
</table>
```

## Options
| attribute name | data type | description |
| ---- | ------ | ----------- |
| `data-locale` | `string` | lowercase two-letters ISO language code |
| `data-search` | `boolean` | tells if table should be searchable |

## Languages
At the time I'm writing this document, there are only Italian (`it`) and English (`en`) available.<br/>
I don't use automatic translators. I prefer filling only languages that I know.<br/>
Other translation can be easily added in the `/src/locales.js` file.<br/>
Remeber to use the correct ISO two-letter code. See <a href="https://www.loc.gov/standards/iso639-2/php/code_list.php">here</a>
