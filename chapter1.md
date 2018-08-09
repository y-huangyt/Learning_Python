---
title: 'Load Data'
description: 'Load Data'
---

## An exercise title written in sentence case

```yaml
type: NormalExercise 
lang: python
xp: 100 
skills: 2
key: 5cced56cca   
```


Xử lý dữ liệu


`@instructions`
- Tên file đã được lưu với biến `member_file`
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
member_file = 'https://assets.datacamp.com/production/repositories/3358/datasets/0dfd9cf73134137fc9e7abcbdce4a3d8af269ae9/member.csv'
```
`@sample_code`
```{python}
# Import pandas as pd
import pandas as pd
# Đọc file csv
member = pd.read_csv(__,__)
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