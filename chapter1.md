---
title: Test
description: Test
---

## An exercise title written in sentence case

```yaml
type: NormalExercise
key: b9c20640c5
lang: python
xp: 100
skills: 2
```

This is the assignment text. It should help provide students with the background information needed.
The instructions that follow should be in bullet point form with clear guidance for what is expected.

`@instructions`
- Instruction 1
- Instruction 2
- Instruction 3

`@hint`
- Here is the hint for this setup problem. 
- It should get students 50% of the way to the correct answer.
- So don't provide the answer, but don't just reiterate the instructions.
- Typically one hint per instruction is a sensible amount.

`@pre_exercise_code`
```{python}
# Load datasets and packages here.
```

`@sample_code`
```{python}
# Your
# sample
# code
# should
# be
# ideally
# 10 lines or less,
# with a max
# of 16 lines.
```

`@solution`
```{python}
# Answer goes here
# Make sure to match the comments with your sample code
# to help students see the differences from solution
# to given.
```

`@sct`
```{python}
# Update this to something more informative.
success_msg("Some praise! Then reinforce a learning objective from the exercise.")
```

---

## Lists to Tuples

```yaml
type: NormalExercise
key: a4991ac1aa
xp: 100
```

Python has lists. Python also has tuples. They are similar, yet different.

`@instructions`
- Create a list called `number_list` containing the numbers 1 through 5
- Convert the list to a tuple called `number_tuple`

`@hint`
The `tuple()` function can convert a list to a tuple.

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
# create the list here
number_list = ____

# convert it to a tuple here
number_tuple = ____
```

`@solution`
```{python}
# create the list here
number_list = [1, 2, 3, 4, 5]

# convert it to a tuple here
number_tuple = tuple(number_list)
```

`@sct`
```{python}
msg = "did you make the list?"
Ex().check_correct(
  check_object("number_list").has_equal_value(),
  check_object("number_tuple").has_equal_value()
)
```
