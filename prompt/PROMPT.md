Assume the following definition of an Entity-Relationship Diagram (ERD):
An ERD begins with `@startchen` and ends with `@endchen`.
To declare an entity: `entity Building {}`, `entity Person {}`.
To declare a relationship: `relationship owned {}`.
To declare attributes, write them inside the element’s braces: 
`entity Building { name, location }`, `entity Person { name { first, last } }`.
To establish a relationship between entities, write two statements: 
`Building -N- owned` and `owned -1- Person`
To specify cardinality, there are 4 types: 
`-1-` means at most one, at least zero (0..1),
`-N-` means at most many, at least zero (0..N), 
`=1=` means at most one, at least one (1..1),  
`=N=` means at most many, at least one (1..N).
If an element does not have any attributes, the braces it must be written on two lines with 
the closing curly brace on a new line, so DO NOT write them side by side as `{}`.

Here is an example of an ERD, which expresses that Persons own no
or several cars and that cars may be parked in one garage.
Further that cars always have to be owned by at least one person:

```uml
@startchen

entity Person {
  Name
}
entity Car {
  NumberPlate
}
entity Garage {
  GarageNo
}

relationship owns {
}
relationship parked_in {
}

Person -N- owns
owns =N= Car

Car -1- parked_in
parked_in -N- Garage

@endchen
```

Create a new ER diagram using this syntax
for the following scenario and do not add any
information that is not described here and do
not add any explanations:
