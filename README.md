# C#  Naming Conventions

In short examples that do not include using directives, use namespace qualifications. If you know that a namespace is imported by default in a project, you do not have to fully qualify the names from that namespace. Qualified names can be broken after a dot (.) if they are too long for a single line, as shown in the following example.

Write only one statement per line.

Write only one declaration per line.

If continuation lines are not indented automatically, indent them one tab stop (four spaces).

Add at least one blank line between method definitions and property definitions.

Use parentheses to make clauses in an expression apparent, as shown in the following code.


| Subject                   |Case                   |
| ------------------------- | --------------------- |
| Class name                | PascalCase            | 
| Constructor name          | PascalCase            | 
| Method name               | PascalCase            | 
| Method arguments          | camelCase             | 
| Local variables           | camelCase             | 
| Constants name            | PascalCase            | 
| Field name                |(Underscore) camelCase | 
| Properties name           | PascalCase            | 
| Delegate name             | PascalCase            | 
| Enum type name            | PascalCase            | 

Method Names
Methods should have verb or verb phrase names like postPayment, deletePage, or save.
Use one word per concept

| like :                 |
| -----------------------|
| verb + name + Name     |
| CreateCartForCustomer()|

REST API Naming 
resource (controller) can be a singleton or a collection
| like :             |
| -------------------|
| User / users       |
| product / products |

resource may contain sub-collection resources
like:
/customers/{customerId}/accounts

Use nouns to represent resources
do not use Get / Create / Update RESTful URI should refer to a resource that is a thing (noun) instead of referring to an action (verb)
| like :                                 |
| ---------------------------------------|
| api/users//user-management             |
| api/device-management/managed-devices  | 

In functions  resources are like executable functions, with parameters and return values; inputs and outputs use verb
like : checkout or play 
| api//cart-management/users/{id}/cart/checkout |

in api do not use underscores 

Argument objects
When a function seems to need more than two or three arguments, it is likely that some of those arguments can be wrapped into a class of their own. Consider, for example, the difference between the two following declarations:














