---
title       : Week 2
description : Insert the chapter description here


--- type:NormalExercise lang:python xp:100 skills:2 key:6183155ad1
## String Methods


*** =instructions

* Use the string's spaces to split it up

*** =hint

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
names = "amy greg todd"


```

*** =solution
```{python}
names = "amy greg todd"

names.split(" ")
```

*** =sct
```{python}
Ex().test_function_v2('names.split')
```

--- type:NormalExercise lang:python xp:100 skills:2 key:1e0a2e80a2
## String Methods and Lists


*** =instructions

* split the variable `names` by its spaces. Assign the result to `split_names`
* add the names `"jane"` and `"pablo"` to the end of `split_names`

*** =hint

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
names = "amy greg todd"

# fill in the blank
split_names = ___

# add jane and pablo to names


```

*** =solution
```{python}
names = "amy greg todd"

# fill in the blank
split_names = names.split(" ")

split_names.append("jane")
split_names.append("pablo")
```

*** =sct
```{python}
Ex().check_object('split_names').is_instance(list)
Ex().has_equal_value("By the end, does `split_names` have 5 entries?", expr_code = "len('split_names')")
Ex().test_object('split_names')
```

--- type:NormalExercise lang:python xp:100 skills:2 key:f72ba2e93a
## Dictionaries


*** =instructions

* make a new dictionary, `d`, containing the keys `"fruit"` and `"calories"`.

(Note, they can have any corresponding values)

*** =hint

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}

```

*** =solution
```{python}
d = {
    'fruit': 'apple',
    'calories': 100
}
```

*** =sct
```{python}
Ex().check_object('d').has_key('fruit').has_key('calories')
```

--- type:NormalExercise lang:python xp:100 skills:2 key:ea5eb927a1
## Modifying a List


*** =instructions

* replace `'b'` with `'x'`, and `'c'` with `'z'`

*** =hint

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
x = ['a', 'b', 'c', 'd']
```

*** =solution
```{python}
x = ['a', 'b', 'c', 'd']
x[1] = 'x'
x[2] = 'z'
```

*** =sct
```{python}
Ex().test_object('x')
```

--- type:NormalExercise lang:python xp:100 skills:2 key:1b9bd13546
## Modifying a Dictionary


*** =instructions

*** =hint

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
d = { 'id': 0, 'name': 'jane' }
```

*** =solution
```{python}
d = { 'id': 0, 'name': 'jane' }

d['name'] = 'susan'
```

*** =sct
```{python}
Ex().test_object('d')
```
