---
title       : Week 1
description : Insert the chapter description here
attachments :
  slides_link : https://s3.amazonaws.com/assets.datacamp.com/course/teach/slides_example.pdf


---
## Basic string

```yaml
type: NormalExercise
key: e18675f236
lang: python
xp: 100
skills: 2
```


`@instructions`

`@hint`

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
"a string"
```

`@solution`
```{python}
type("a string")
```

`@sct`
```{python}
Ex().test_function_v2('type', params = ['self'])
```
---
## Defining and printing variables

```yaml
type: NormalExercise
key: d54002a0b5
lang: python
xp: 100
skills: 2
```


`@instructions`

* Add a comment to the code below
* Define a variable `x`. Set it equal to `2`
* print out x

`@hint`

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}
# Defining the variable x
x = 2

print(x)
```

`@sct`
```{python}
Ex().test_student_typed('^\S*#', not_typed_msg = "Did you add a comment by starting a line with `#`?")

Ex().test_object('x')

Ex().test_function_v2('print', params = ['value'])

```

---
## Basic operations

```yaml
type: NormalExercise
key: eb0d5ca694
lang: python
xp: 100
skills: 2
```


`@instructions`

* set `x` to be 5
* set `y` to be 2
* write in a comment what you expect x divided by y to be.
* print `x` divided by `y`

`@hint`

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}
x = 5
y = 2

# x / y will be 2, since when python divides whole numbers, it rounds down

print(x / y)
```

`@sct`
```{python}

```


---
## Lists

```yaml
type: NormalExercise
key: 8e146cf9b6
lang: python
xp: 100
skills: 2
```


`@instructions`

* define `cities` to be a list with 3 entries

`@hint`

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
cities = 
```

`@solution`
```{python}
cities = ['new york', 'princeton', 'philadelphia']
```

`@sct`
```{python}
Ex().check_object('cities').is_instance(list)
Ex().has_equal_value("Did you add three entries to `cities`?", expr_code = "len(cities)")
```


---
## List indexing

```yaml
type: NormalExercise
key: 01f9e51b07
lang: python
xp: 100
skills: 2
```


`@instructions`

* print out the first entry of `x`

`@hint`

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
x = ['a', 'b', 'c']
```

`@solution`
```{python}
x = ['a', 'b', 'c']

print(x[0])
```

`@sct`
```{python}
Ex().test_function_v2('print')
Ex().test_output_contains("'a'", no_output_message = "Did you get the first entry ('a')?")
```
---
## Importing (1)

```yaml
type: NormalExercise
key: 71cf4495b4
lang: python
xp: 100
skills: 2
```


`@instructions`

* import the `math` library
* use the `abs` function from that library (try it on a number)

`@hint`

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}
import math
abs(-2)
```

`@sct`
```{python}
Ex().test_import('math')
Ex().test_function_v2('abs')
```


---
## Importing (2)

```yaml
type: NormalExercise
key: f3c5d745cc
lang: python
xp: 100
skills: 2
```


`@instructions`

* import `glob` from the `glob` library

`@hint`

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
# import glob func from glob library

# use to see files in directory
# * is a wildcard, that matches anything
glob('*.ipynb')

```

`@solution`
```{python}
# import glob func from glob library
from glob import glob

# use to see files in directory
# * is a wildcard, that matches anything
glob('*.ipynb')
```

`@sct`
```{python}
Ex().test_import('glob')
```
