# Name Convention

- [Name Convention](#name-convention)
    - [*Rules*](#rules)
  - [***Classes***](#classes)
  - [***Functions***](#functions)
  - [***Variables & Paramters Functions***](#variables--paramters-functions)
  - [***Constants***](#constants)
  - [**Database Tables**](#database-tables)
    - [*Naming rules:*](#naming-rules)
  - [**Files & Folders**](#files--folders)
    - [File](#file)
    - [Folder](#folder)

### *Rules*
- Start with letters
- Remaining can be letters or numbers

---

## ***Classes***

I- Start Capital letters

II- Multi word in Class name start Capital letters


> Examples

``` Java

Class User {}

Class GroupUser {}

```
---

## ***Functions***

I- Start lower letters

II- Multi word in Class name start Capital letters

III- if add underscore to name between word must all functioins name will follow same convention (the word after underscore will start lower case)


> Examples

``` Java

// (1)
public void getName() {}

private String setName(...) {}

// (2)
public void get_name() {}

private String set_name(...) {}

```

--- 

## ***Variables & Paramters Functions***

`var` : variable

`param` : Paramters function

I- `var`, `param`: Start lower letters

param: start always with char 'p_'

II- Multi word

`var`: second word will upper case 

`param`: second word will start with underscore

III- `var` : in private start with underscore

IV- `Boolean` : It is common to use a prefix like is, are, has in the names to distinguish a boolean from other variables.


``` Java

// Variables in class

Class User {

    public int id;

    private float _salary;

    public String firstName;

}

// Variables in block

{
    int id;
    float salary;
    String firstName;
}

// Parameters in function

public void getNameUser(int p_userId, String p_conditionSting) {}

// Boolean variable

// bad
var flag = true;

// bad
var clicked = true;

// good
var isClicked = true;

```

---

## ***Constants***

- Capital Letters all the word with underscore between word

> Examples

```Java
const String KEY_AUTH_HASHING = "..."
```

--- 

## **Database Tables**

### *Naming rules:*


* Single column primary key fields should be named id.
* Foreign key fields should be a combination of the name of the referenced table
    and the name of the referenced fields. 
    
    > Ex: foo_id.


* Prefixes and Suffixes (are bad)
    > Ex: naming tables with a TB_ , etc.   prefix is a bad idea.

    > Ex: our app "Foobar" would have tables name Foobar_Users, Foobar_Teams, etc.
    Again, this is a bad idea.

    > Ex: data types to suffixes, text -> tx, date -> dt, etc. is a bad idea.


* Avoid quotes and  use Lowercase. Identifiers should be written entirely in lower case.
Ex: Avoid using names like "FirstName" or "All Employees".
    > Ex: Use first_name, not "First_Name".

* Avoid reserved words and Data types are not names. Avoid using words that are just data types such as text or timestamp.
    > Ex: Avoid using words like user, lock, or table.

* Underscores separate words. Object name that are comprised of multiple words should be
    separated by underscores (ie. snake case).
    > Ex: Use word_count or team_member_id, not wordcount or wordCount.

* Full words, not abbreviations.
    > Ex: Use middle_name, not mid_nm.

---

## **Files & Folders**

### File

You can name files by using PascalCase and kebab-case.

> Example

```
>PascalCase<

- components/
--- user/
----- UserProfile.js
----- UserList.js
----- UserItem.js
--- ui/
----- Dialog.js
----- Dropdown.js
----- Table.js

>kebab-case<

- routing/
--- user-route.js
--- messages-route.js

```

### Folder

Name of folder will be in lower case only

List of common folders name:

- libs
- utils


