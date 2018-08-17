---
  title: "Hello World"
  description: "Python cơ bản"
---

## Giao diện Python trên Data Camp

```yaml
type: NormalExercise 
lang: python
xp: 100 
skills: 2
key: bdc52f0e19   
```


Trong khung script python bên phải, bạn có thể gõ code Python để làm bài tập. Khi bạn nhấn _Run Code_ hoặc _Submit Answer_, script python (`script.py`) sẽ được thực thi và kết quả sẽ được hiện thị ở khung IPython Shell(Khung phía dưới). _Submit Answer_ kiểm tra bài làm của bạn có đúng không và thông báo kết quả.

 Nếu cảm thấy yêu cầu của bài hơi khó, bạn có thể click vào _Take Hint_ hoặc  _Take Solution_ . Dĩ nhiên bạn sẽ bị mất đi 1 phần Xp khi click vào các nút này.

Bạn có thể sử dụng  IPython Shell  để gõ các câu lệnh python sau đó nhấn Enter.  Sử dụng nó để kiểm tra lỗi cú pháp hoặc kết quả.


`@instructions`
- Trong khung  IPython Shell; gõ `5 / 8`.
- Trong khung Python script, gõ : `print(7 + 10)`.
-  Nhấn _Submit Answer_.

`@hint`
Bạn đã gõ `print(7 + 10)`  vào khung Python Script chưa?

`@sample_code`

```{python}
# Ví dụ
print(5 / 8)

# Gõ code vào đây
```

`@solution`

```{python}
# Ví dụ
print(5 / 8)

# Gõ code vào đây
print(7 + 10)
```

`@sct`

```{python}
Ex().has_printout(1, not_printed_msg = "__JINJA__: Bạn đã sử dụng `{{sol_call}}` để in tổng của 7 và 10 chưa?")
success_msg("Tuyệt! Đến bài tiếp theo nào")
```

---

## Bạn sử dụng Python khi nào?

```yaml
type: MultipleChoiceExercise 
lang: python
xp: 50 
skills: 2
key: 9703b117fb   
```


Python là một ngôn ngữ đa năng. Bạn có thể dùng python khi?


`@instructions`
- Thực hiện một số tính toán một cách nhanh chóng .
- Xây dựng một database-driven website.
- Làm sạch dữ liệu và phân tích các bảng khảo sát.
- Tất cả các phương án trên.

`@hint`
Bạn có thể tra google...

`@sct`

```{python}
msg1 = "Chưa chính xác. Python có thể làm được nhiều hơn thế!"
msg2 = "Chưa chính xác. Framework phổ biến để xây dựng database-driven websites là Django, Nhưng Python còn có thể làm nhiều hơn vậy."
msg3 = "Chưa chính xác. Python là một công cụ rất mạnh cho việc xử lý và phân tích dữ liệu. Ngoài ra nó còn làm được các việc khác"
msg4 = "Chính xác! Python là một ngôn ngữ rất đa năng."
Ex().has_chosen(4, [msg1, msg2, msg3, msg4])
```

---

## Thêm chú thích vào Python script

```yaml
type: NormalExercise 
lang: python
xp: 100 
skills: 2
key: 7c4a738a13   
```


Bạn có thể thêm vào dòng chú thích (**comments**) trong file Python scripts. Dòng chú thích giúp người khác đọc lại code của bạn dễ dàng hơn, và cũng để bạn nhớ ra bạn code cái quái gì vào tuần trước.

Để thêm **comments** vào  Python script ,sử dụng `#` tag. Những **comment** này sẽ không được tính là một dòng  code Python, và nó sẽ không ảnh hưởng tới kết quả tính toán.   Trong vị dụ bên phải, mình đã thêm comment : `# Division`


`@instructions`
Thêm chú thích ` # Addition ` phía trên dòng `print(7 + 10)`.

`@hint`
Bạn đã thêm chú thích đúng chỗ chưa

`@sample_code`

```{python}
# Division
print(5 / 8)


print(7 + 10)
```

`@solution`

```{python}
# Division
print(5 / 8)

# Addition
print(7 + 10)
```

`@sct`

```{python}
Ex().has_code("#\s*(\w+)[\s.!?]*print\s*\(\s*7", not_typed_msg = "Hãy chắc chắn rằng bạn đã thêm phần comment phía trên phần `print(7 + 10)`.")
success_msg("Tuyệt!")
```

---

## Tính toán đơn giản bằng Python

```yaml
type: NormalExercise 
lang: python
xp: 100 
skills: 2
key: 0f7c039428   
```


Python phù hợp cho các tính toán cơ bản bao gồm cộng trừ nhân chia, ngoài ra nó còn hỗ trợ các phép tính khác
- Phép lũy thừa: `**`.  Ví dụ `4**2` sẽ cho kết quả là `16`.
- Modulo: `%`. Cho kết quả là modulo. Ví dụ  `18 % 7` có kết quả là  `4`.

Dưới đây là một ví dụ.


`@instructions`
Giả sử bạn có $100, Bạn có thể gửi ngân hàng với lãi suất  là 10% Mỗi năm. Năm đầu tiên bạn sẽ có  $100 \times 1.1 = 110$ , sau năm thứ hai nó sẽ là  $100 \times 1.1 \times 1.1 = 121$. 
Hãy viết đoạn code tính tổng tiền bạn có sau 7 năm.

`@hint`
Sau năm thứ 2 bạn có $100 \times 1.1 \times 1.1 = 100 \times 1.1^2$. Sau 7 năm bạn sẽ có bao nhiêu? Sử dụng  `*` và`**`.

`@pre_exercise_code`

```{python}

```


`@sample_code`

```{python}
# Cộng, trừ
print(5 + 5)
print(5 - 5)

# Nhân, Chia, Modulo, Lũy thừa
print(3 * 5)
print(10 / 2)
print(18 % 7)
print(4 ** 2)

# Số tiền bạn có được sau 7 năm?
```

`@solution`

```{python}
# Cộng, trừ
print(5 + 5)
print(5 - 5)

# Nhân, Chia, Modulo, Lũy thừa
print(3 * 5)
print(10 / 2)
print(18 % 7)
print(4 ** 2)

# Số tiền bạn có được sau 7 năm?
print(100 * 1.1 ** 7)
```

`@sct`

```{python}
Ex().has_printout(6, not_printed_msg = "Bạn đã thử `print(100 * 1.1 ** 7)` chưa?")
success_msg("Tuyệt!")
```

---

## Gán giá trị

```yaml
type: NormalExercise 
lang: python
xp: 100 
skills: 2
key: 4bf65ad83e   
```


Để khai báo biến và gán giá trị cho python sử dụng ``` Tên biến = Tên giá trị``
Ví dụ
```
x = 5
```

Nhớ răng, `=` trong Python có nghĩa là   _phép gán_,  Không phải so sánh bằng~~


`@instructions`
- Create a variable `savings` with the value 100.
- Check out this variable by typing `print(savings)` in the script.

`@hint`
- Type `savings = 100` to create the variable `savings`.
- After creating the variable `savings`, you can type `print(savings)`.

`@pre_exercise_code`

```{python}

```


`@sample_code`

```{python}
# Create a variable savings


# Print out savings
```

`@solution`

```{python}
# Create a variable savings
savings = 100

# Print out savings
print(savings)
```

`@sct`

```{python}
Ex().check_object("savings").has_equal_value(incorrect_msg="Assign `100` to the variable `savings`.")
Ex().has_printout(0, not_printed_msg = "Print out `savings`, the variable you created, with `print(savings)`.")
success_msg("Great! Let's try to do some calculations with this variable now!")
```

---

## Calculations with variables

```yaml
type: NormalExercise 
lang: python
xp: 100 
skills: 2
key: ff06cedeb4   
```


Remember how you calculated the money you ended up with after 7 years of investing $100? You did something like this:

```
100 * 1.10 ** 7
```

Instead of calculating with the actual values, you can use variables instead. The `savings` variable you've created in the previous exercise represents the $100 you started with. It's up to you to create a new variable to represent `1.10` and then redo the calculations!


`@instructions`
- Create a variable `factor`, equal to `1.10`.
- Use `savings` and `factor` to calculate the amount of money you end up with after 7 years. Store the result in a new variable, `result`.
- Print out the value of `result`.

`@hint`
- To create the variable `factor`, use `factor = 1.10`.
- In the example code block of the assignment, replace `100` with `savings` and `1.10` with `factor`: `savings * factor ** 7`.
- Use the [`print()`](https://docs.python.org/3/library/functions.html#print) function to print the value of a variable.

`@sample_code`

```{python}
# Create a variable savings
savings = 100

# Create a variable factor


# Calculate result


# Print out result
```

`@solution`

```{python}
# Create a variable savings
savings = 100

# Create a variable factor
factor = 1.1

# Calculate result
result = savings * factor ** 7

# Print out result
print(result)
```

`@sct`

```{python}
Ex().check_correct(
  check_object("result").has_equal_value(incorrect_msg="Have you used `*` and `**` to calculate `result`?"),
  multi(
    check_object("savings", missing_msg="The variable `savings` was defined for you, don't remove it!").has_equal_value(incorrect_msg="The variable `savings` should be `100`, like it was defined for you."),
    check_object("factor").has_equal_value(incorrect_msg="The value of `factor` should be `1.1`.")
  )
)
Ex().has_printout(0, not_printed_msg="Don't forget to print out `result` at the end of your script.")
success_msg("Great!")
```

---

## Other variable types

```yaml
type: NormalExercise 
lang: python
xp: 100 
skills: 2
key: 006b48561f   
```


In the previous exercise, you worked with two Python data types:

- `int`, or integer: a number without a fractional part. `savings`, with the value `100`, is an example of an integer.
- `float`, or floating point: a number that has both an integer and fractional part, separated by a point. `factor`, with the value `1.10`, is an example of a float.

Next to numerical data types, there are two other very common data types:

- `str`, or string: a type to represent text. You can use single or double quotes to build a string.
- `bool`, or boolean: a type to represent logical values. Can only be `True` or `False` (the capitalization is important!).


`@instructions`
- Create a new string, `desc`, with the value `"compound interest"`.
- Create a new boolean, `profitable`, with the value `True`.

`@hint`
- To create a variable in Python, use `=`. Make sure to wrap your string in single or double quotes.
- Only two boolean values exist in Python: `True` and `False`. `TRUE`, `true`, `FALSE`, `false` and other versions will not be accepted.

`@sample_code`

```{python}
# Create a variable desc


# Create a variable profitable
```

`@solution`

```{python}
# Create a variable desc
desc = "compound interest"

# Create a variable profitable
profitable = True
```

`@sct`

```{python}
Ex().check_object("desc").has_equal_value()
Ex().check_object("profitable").has_equal_value()
success_msg("Nice!")
```

---

## Guess the type

```yaml
type: MultipleChoiceExercise 
lang: python
xp: 50 
skills: 2
key: b35f67514c   
```


To find out the type of a value or a variable that refers to that value, you can use the [`type()`](https://docs.python.org/3/library/functions.html#type) function. Suppose you've defined a variable `a`, but you forgot the type of this variable. To determine the type of `a`, simply execute:

```
type(a)
```

We already went ahead and created three variables: `a`, `b` and `c`. You can use the IPython shell on the right to discover their type. Which of the following options is correct?


`@instructions`
- `a` is of type `int`, `b` is of type `str`, `c` is of type `bool`
- `a` is of type `float`, `b` is of type `bool`, `c` is of type `str`
- `a` is of type `float`, `b` is of type `str`, `c` is of type `bool`
- `a` is of type `int`, `b` is of type `bool`, `c` is of type `str`

`@hint`
Use `type(a)`, `type(b)` and `type(c)` inside the IPython Shell to find out about the variables' types.

`@pre_exercise_code`

```{python}
a = 100*1.1**7
b = "True"
c = False
```

`@sct`

```{python}
msg1 = "The type of `a` is not `int`. Try out `type(a)` and see for yourself."
msg2 = "`b` is not a `bool`, it's a `str`! The fact that `True` is wrapped in double quotes makes it a string."
msg3 = "Correcto perfecto!"
msg4 = "None of the variable's types is correct here. Try `type(a)` and see what type this variable is."
Ex().has_chosen(3,[msg1, msg2, msg3, msg4])
```

---

## Operations with other types

```yaml
type: NormalExercise 
lang: python
xp: 100 
skills: 2
key: 4d0d83cc02   
```


Filip mentioned that different types behave differently in Python.

When you sum two strings, for example, you'll get different behavior than when you sum two integers or two booleans.

In the script some variables with different types have already been created. It's up to you to use them.


`@instructions`
- Calculate the product of `savings` and `factor`. Store the result in `year1`.
- What do you think the resulting type will be? Find out by printing out the type of `year1`.
- Calculate the sum of `desc` and `desc` and store the result in a new variable `doubledesc`.
- Print out `doubledesc`. Did you expect this?

`@hint`
- Assign `factor * savings` to a new variable, `year1`.
- To print the type of a variable `x`, use `print(type(x))`.
- Assign `desc + desc` to a new variable, `doubledesc`.
- To print a variable `x`, write `print(x)` in the script.

`@sample_code`

```{python}
savings = 100
factor = 1.1
desc = "compound interest"

# Assign product of factor and savings to year1


# Print the type of year1


# Assign sum of desc and desc to doubledesc


# Print out doubledesc
```

`@solution`

```{python}
savings = 100
factor = 1.1
desc = "compound interest"

# Assign product of savings and factor to year1
year1 = savings * factor

# Print the type of year1
print(type(year1))

# Assign sum of desc and desc to doubledesc
doubledesc = desc + desc

# Print out doubledesc
print(doubledesc)
```

`@sct`

```{python}
# predefined
msg = "You don't have to change or remove the predefined variables."
objs = ["savings", "factor", "desc", "year1"]
Ex().multi(
    check_object('savings', missing_msg=msg).has_equal_value(incorrect_msg=msg),
    check_object('factor', missing_msg=msg).has_equal_value(incorrect_msg=msg),
    check_object('desc', missing_msg=msg).has_equal_value(incorrect_msg=msg),
    check_object('year1', missing_msg=msg).has_equal_value(incorrect_msg=msg)
)

# check year1 and printout
Ex().multi(
    check_object("year1").has_equal_value(incorrect_msg="Multiply `savings` and `factor` to create the `year1` variable."),
    has_printout(0, not_printed_msg = "__JINJA__:Use `{{sol_call}}` to print out the type of `year1`.")
)

# check doubledesc and prinout
Ex().multi(
    check_object("doubledesc").has_equal_value(incorrect_msg  = "Have you stored the result of `desc + desc` in `doubledesc`?"),
    has_printout(1, not_printed_msg = "Don't forget to print out `doubledesc`.")
)

success_msg("Nice. Notice how `desc + desc` causes `\"compound interest\"` and `\"compound interest\"` to be pasted together.")
```

---

## Type conversion

```yaml
type: NormalExercise 
lang: python
xp: 100 
skills: 2
key: 085bb602b9   
```


Using the `+` operator to paste together two strings can be very useful in building custom messages.

Suppose, for example, that you've calculated the return of your investment and want to summarize the results in a string. Assuming the floats `savings` and `result` are defined, you can try something like this:

```
print("I started with $" + savings + " and now have $" + result + ". Awesome!")
```

This will not work, though, as you cannot simply sum strings and floats.

To fix the error, you'll need to explicitly convert the types of your variables. More specifically, you'll need [`str()`](https://docs.python.org/3/library/functions.html#func-str), to convert a value into a string. `str(savings)`, for example, will convert the float `savings` to a string.

Similar functions such as [`int()`](https://docs.python.org/3/library/functions.html#int), [`float()`](https://docs.python.org/3/library/functions.html#float) and [`bool()`](https://docs.python.org/3/library/functions.html#bool) will help you convert Python values into any type.


`@instructions`
- Hit _Run Code_ to run the code on the right. Try to understand the error message.
- Fix the code on the right such that the printout runs without errors; use the function [`str()`](https://docs.python.org/3/library/functions.html#func-str) to convert the variables to strings.
- Convert the variable `pi_string` to a float and store this float as a new variable, `pi_float`.

`@hint`
- You should use [`str()`](https://docs.python.org/3/library/functions.html#func-str) twice!
- Use [`float()`](https://docs.python.org/3/library/functions.html#float) on `pi_string` and store the result in `pi_float`.

`@sample_code`

```{python}
# Definition of savings and result
savings = 100
result = 100 * 1.10 ** 7

# Fix the printout
print("I started with $" + savings + " and now have $" + result + ". Awesome!")

# Definition of pi_string
pi_string = "3.1415926"

# Convert pi_string into float: pi_float
```

`@solution`

```{python}
# Definition of savings and result
savings = 100
result = 100 * 1.10 ** 7

# Fix the printout
print("I started with $" + str(savings) + " and now have $" + str(result) + ". Awesome!")

# Definition of pi_string
pi_string = "3.1415926"

# Convert pi_string into float: pi_float
pi_float = float(pi_string)
```

`@sct`

```{python}
# ensure predefined values are unmodified
msg = "You don't have to change or remove the predefined variables."
Ex().multi(
    check_object("savings", missing_msg=msg).has_equal_ast(incorrect_msg=msg),
    check_object("result", missing_msg=msg).has_equal_ast(incorrect_msg=msg)
)

Ex().check_correct(
    has_printout(0),
    multi(
        check_function("str", 0).check_args(0).has_equal_value(incorrect_msg="Inside the `print()` command, make sure to convert `savings` into a string with `str(savings)`."),
        check_function("str", 1).check_args(0).has_equal_value(incorrect_msg="Inside the `print()` command, make sure to convert `result` into a string `str(result)`.")
    )
)

# check pi_float
Ex().check_correct(
    check_object("pi_float").has_equal_value(),
    multi(
        check_object("pi_string").has_equal_value(),
        check_function("float", missing_msg = "In order to convert `pi_string` to a float, be sure to use the `float()` function.").has_equal_value(incorrect_msg="Use `float(pi_string) to create the variable `pi_float`.")
    )
)

success_msg("Great! You have a profit of around $95; that's pretty awesome indeed!")
```

---

## Can Python handle everything?

```yaml
type: MultipleChoiceExercise 
lang: python
xp: 50 
skills: 2
key: 3e5f0bdf3a   
```


Now that you know something more about combining different sources of information, have a look at the four Python expressions below.
Which one of these will throw an error? You can always copy and paste this code in the IPython Shell to find out!


`@instructions`
- `"I can add integers, like "  + str(5) + " to strings."`
- `"I said " + ("Hey " * 2) + "Hey!"`
- `"The correct answer to this multiple choice exercise is answer number " + 2`
- `True + False`

`@hint`
Copy and paste the different expressions into the IPython Shell and try to figure out which one throws an error.
