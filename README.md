# O.N.D.E.

O.N.D.E. - Onde is Not Developed by Experts

Inspired by the [exflickr/flamework](https://github.com/exflickr/flamework), 
Onde is a quick and dirty PHP application prototyping fLame Work.

## Automatic form CRUD (forms.php)

In its current version, it serves as the basis for an simple PHP application,
providing functions to generate HTML tables from PostgreSQL queries and also a
module to automatically generate CRUD forms for PostgreSQL tables.

The CRUD form generation tool scans the database data dictionary no
identify relations making selection boxes (or radio lists, depending of the
size of the list) for the 1:N relations and check boxes lists for the
N:N relations.

The tool handles the submited information throught a "insert" or a "save" button,
thus automaticallly generating a insert or update query statment.
There is no object relational abstration, the queries are generated directly
in the PHP functions. 

## Automatic Menus from table menu (databasemenu.php)

The framework provides a side menu (usually at left side of the window),
which is generated from table menu's data. The menu items could link
to a php script a forms.php's form ar a calendar.

## User access control

The user's access control is made through limiting the access of
user's groups. Each user is asigned to a group (or groups) and the
forms and menus are cleared for the groups.

It is possible to clear some forms to be accessible without authentication.
