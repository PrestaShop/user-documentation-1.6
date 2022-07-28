# Cheat-sheet: Concepts outlined in this tutorial

## Summary of the available methods in the library <a href="#cheat-sheet-conceptsoutlinedinthistutorial-summaryoftheavailablemethodsinthelibrary" id="cheat-sheet-conceptsoutlinedinthistutorial-summaryoftheavailablemethodsinthelibrary"></a>

To help you get started with web service, here's a little memo of techniques used in this tutorial.

|       |        |        | Method parameters |          |    |     |
| ----- | ------ | ------ | ----------------- | -------- | -- | --- |
|       | REST   | Method | url               | resource | id | xml |
| **C** | POST   | add    | X                 | X        |    | X   |
| **R** | GET    | get    | X                 | X        | X  |     |
| **U** | UPDATE | edit   | X                 | X        | X  | X   |
| **D** | DELETE | delete | X                 | X        | X  |     |

If the URL parameter is specified, no other setting can be used and vice versa.

## Options <a href="#cheat-sheet-conceptsoutlinedinthistutorial-options" id="cheat-sheet-conceptsoutlinedinthistutorial-options"></a>

| Key            | Value                  | Description                                   |
| -------------- | ---------------------- | --------------------------------------------- |
| output\_format | XML, JSON              | Change the output format                      |
| ps\_method     | GET, POST, PUT, DELETE | Override the HTTP method used for the request |
| display        | \[field1,field2 …]     | Only display fields in brackets               |
| display        | full                   | Display all fields                            |

| Key    | Key suffix | prefix | Value             | Suffix    | Description                                             |
| ------ | ---------- | ------ | ----------------- | --------- | ------------------------------------------------------- |
| filter | \[field]   |        | \[value1          | \[value2] | Filter "field" with value between "value1" and "value2" |
| filter | \[field]   |        | \[value]          |           | Filter field with the value "value"                     |
| filter | \[field]   |        | \[value1,value2…] |           | Filter fields for values specified between brackets     |
| filter | \[field]   | %      | \[value]          | %         | Filter "columns" for values containing "value"          |

| Key  | Value                                   | Description                                                |
| ---- | --------------------------------------- | ---------------------------------------------------------- |
| sort | \[field1\_ASC,field2\_DESC,field3\_ASC] | Sort by field with the suffix \_ASC \_DESC or in the order |
| sort | full                                    | show all fields                                            |

| Key   | Value                  | Description                                   |
| ----- | ---------------------- | --------------------------------------------- |
| limit | Number                 | Limit the result to "Number"                  |
| limit | Starting index, Number | Limit the result to "Number" from the "Index" |

## Using the library in multistore mode <a href="#cheat-sheet-conceptsoutlinedinthistutorial-usingthelibraryinmultistoremode" id="cheat-sheet-conceptsoutlinedinthistutorial-usingthelibraryinmultistoremode"></a>

In order to use web services in when the multistore feature is enabled, you simply have to add the `id_shop` parameter.

The `shops` entity enables you to access to the list of shops as well as their associated identifiers.

| Key             | Value         | Description                                                        |
| --------------- | ------------- | ------------------------------------------------------------------ |
| id\_shop        | Shop ID       | Define the shop to be used as a context for the web service.       |
| id\_group\_shop | Group shop ID | Define the group shop to be used as a context for the web service. |
