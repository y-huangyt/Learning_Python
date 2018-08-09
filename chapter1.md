---
title: 'Load Data'
description: 'Load Data'
---

## Đọc file

```yaml
type: NormalExercise 
lang: python
xp: 100 
skills: 2
key: 5cced56cca   
```


Dữ liệu về thông tin thành viên được lưu dưới dạng `.csv`.
Bài tập này giúp hiểu được các đọc file `.csv`


`@instructions`
- Tên file đã được lưu với biến `member_file`. Đọc dữ liệu với `pd.read_csv`
- In ra 10 dòng đầu tiên. Sử dụng hàm `head()'
- Xem tên các cột. Sử dụng thuộc tính `columns`

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
member = pd.read_csv(__)
# xuất ra 10 dòng đầu tiên
print(member.__(10))
# xuất ra tên các cột
print(member.__)
```
`@solution`
```{python}
# Import pandas as pd
import pandas as pd
# Đọc file csv
member = pd.read_csv(member_file)
# xuất ra 10 dòng đầu tiên
print(member.head(10))
# xuất ra tên các cột
print(member.columns)
```
`@sct`
```{python}
# Update this to something more informative.
success_msg("Some praise! Then reinforce a learning objective from the exercise.")
```