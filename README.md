# JS Destructuring Object And Array data
This is how you can destructor the Object and Array data. It is useful specially when you work with third party data.

DESTRUCTURING ARRAY DATA IN JS

```JS
  // Structuring Array JS
  const darray = [2, 4, 6];
  console.log(darray);

  // Destructuring Array JS
  const a = darray[0];
  const b = darray[1];
  const c = darray[2];
  console.log(a, b, c);
  // OR 
  const [x, y, n] = darray;
  console.log(x, y, n);
  
  // Nested array destructuring
  const nested = [2, 4, [5,6]];
  const [a1, , [c1,d1]] = nested;
  console.log(a1); 

  // Assigned Default Nested Value
  const [v = 8, w = 1, h = 1] = ['A'];
  console.log(v); // Result A
```

```JS
// Console.log() | Result
(3) [2, 4, 6]
2 4 6
2 4 6
2
A
```

DESTRUCTURING OBJECT DATA IN JS
```JS
  // OBJECT
  const Developer = {
      
    name: 'NielsOffice',
    skills : ['PHP','JS','C++'],
    yearExperience: 3,

    getReport : function() {
        return `${this.name} skills are ${this.skills} Years of experience ${this.yearExperience}`;
    }

  }
    
  // DESTRUCTURING OBJECT !
  const { name, skills, yearExperience } = Developer;
  // For instance ifever one of this is array you can work loop through it!
  // Selecting the property or destrucking to access the data from object!
  console.log(name, skills, yearExperience); 

  // DESTRUCTURING ASSIGNED VARIABLE ON PROPERTIES OF OBJECT !
  const {name : assignVarIsN, skills: asignVarIsS, yearExperience: assignVarIsyE} = Developer;
  console.log(assignVarIsN, asignVarIsS, assignVarIsyE); 
```

```JS
// Console.log() | Result
NielsOffice (3) ['PHP', 'JS', 'C++'] 3
NielsOffice (3) ['PHP', 'JS', 'C++'] 3
```
