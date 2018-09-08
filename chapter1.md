---
title: 'Hello World'
description: 'Python cơ bản'
---

## Giao diện Python trên Data Camp

```yaml
type: NormalExercise
key: bdc52f0e19
lang: python
xp: 100
skills: 2
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
key: 9703b117fb
lang: python
xp: 50
skills: 2
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
key: 7c4a738a13
lang: python
xp: 100
skills: 2
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
key: 0f7c039428
lang: python
xp: 100
skills: 2
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
key: 4bf65ad83e
lang: python
xp: 100
skills: 2
```

Để khai báo biến và gán giá trị cho python sử dụng ``` Tên biến = giá trị``
Ví dụ
```
x = 5
```

Nhớ rằng, `=` trong Python có nghĩa là   _phép gán_,  Không phải so sánh bằng~~

`@instructions`
- Tạo biến `savings` Với giá trị 100.
- Xuất ra giá trị của biến với cú pháp  `print(savings)` .

`@hint`
- Cái này dễ mà, thử lại nào!!!!!!!!!!!!!!!!!!!!!!!!!!!

`@sample_code`
```{python}
# Tạo biến savings

# In ra giá trị savings
```

`@solution`
```{python}
# Tạo biến savings
savings = 100
# In ra giá trị savings
print(savings)
```

`@sct`
```{python}
Ex().check_object("savings").has_equal_value(incorrect_msg="Gán `100` Cho biến `savings`.")
Ex().has_printout(0, not_printed_msg = "In ra giá trị `savings`, sử dụng `print(savings)`.")
success_msg("Tuyệt!")
```

---

## Tính toán với các biến

```yaml
type: NormalExercise
key: ff06cedeb4
lang: python
xp: 100
skills: 2
```

Hãy nhớ lại bài trước đó, dưới đây là kết quả số tiền bạn có được sau 7 năm.
```
100 * 1.10 ** 7
```

`@instructions`
- Tạo biến hệ số : `factor`và gán giá trị `1.10`.
- Sử dụng 2 biến `savings` và `factor` để tính số tiền bạn thu được, và lưu kết quả vào biến `result`.
- In ra giá trị của biến `result`.

`@hint`
- Tạo biến `factor`, dùng lệnh `factor = 1.10`.
- Thay  `100` bằng `savings` và `1.10` bằng  `factor`: `savings * factor ** 7`.

`@sample_code`
```{python}
# Khai báo biến savings
savings = 100
# Khai báo biến factor

# Tính kết quả và lưu vào biến: result

# In kết quả
```

`@solution`
```{python}
# Khai báo biến savings
savings = 100
# Khai báo biến factor
factor = 1.1
# Tính kết quả và lưu vào biến: result
result = savings * factor ** 7
# In kết quả 
print(result)
```

`@sct`
```{python}
Ex().check_correct(
  check_object("result").has_equal_value(incorrect_msg="Bạn đã sử dụng `*` and `**` để tính kết quả và lưu vào `result` chưa?"),
  multi(
    check_object("savings", missing_msg=" Vui lòng đừng xóa biến `savings`!").has_equal_value(incorrect_msg="Biến `savings` nên để giá trị `100`, Vui lòng đừng thay đổi."),
    check_object("factor").has_equal_value(incorrect_msg="Biến `factor` nên có giá trị `1.1`.")
  )
)
Ex().has_printout(0, not_printed_msg="Đừng quên in giá trị của `result`.")
success_msg("Tuyệt!")
```

---

## Các kiểu biến trong Python

```yaml
type: NormalExercise
key: 006b48561f
lang: python
xp: 100
skills: 2
```

Trong bài tập trước, chúng ta đã làm quen với 2 kiểu biến trong Python
- `int` : kiểu số nguyên
- `float` : kiểu thập phân.

Ngoài kiểu số còn có 2 kiểu dữ liệu rất phổ biến:

- `str`, : Kiểu chuỗi, được đặt trong nháy đơn `'` hoặc nháy kép `"`.
- `bool`: Kiểu logic, chỉ mang giá trị `True` hoặc `False`(Lưu ý là viết Hoa chữ cái đầu).

`@instructions`
- Khai báo biến kiểu string , `msg` với giá trị `"Hello World!"`.
- Khai báo biến kiểu boolean, `newbie`, với giá trị `True`.

`@hint`
- Hãy chắc rằng chuỗi bạn truyền vào nằm trong `'` hoặc `"`.
- `True` chỉ viết hoa chữ cái đầu

`@sample_code`
```{python}
# Khai báo biến msg

# Khai báo biến newbie
```

`@solution`
```{python}
# Khai báo biến msg
msg = "Hello World!"
# Khai báo biến newbie
newbie = True
```

`@sct`
```{python}
Ex().check_object("msg").has_equal_value()
Ex().check_object("newbie").has_equal_value()
success_msg("Xong!")
```

---

## Kiểm tra kiểu dữ liệu

```yaml
type: MultipleChoiceExercise
key: b35f67514c
lang: python
xp: 50
skills: 2
```

Để kiểm tra kiểu dữ liệu của một biến hoặc một giá trị, ta dùng hàm  [`type()`](https://docs.python.org/3/library/functions.html#type) function. Để kiểm tra kiểu dữ liệu của biến `a` ta chỉ cần gọi `type(a)`:

```
type(a)
```

Chúng tôi đã khai báo sẵn ba biến `a`, `b` and `c`. Bằng cách sử dụng `type()` trong khung _IPython shell_ hãy đánh dấu vào câu trả lời đúng?

`@instructions`
- `a` thuộc kiểu `int`, `b` thuộc kiểu  `str`, `c` thuộc kiểu `bool`
- `a` thuộc kiểu `float`, `b` thuộc kiểu `bool`, `c` thuộc kiểu `str`
- `a` thuộc kiểu `float`, `b` thuộc kiểu `str`, `c` thuộc kiểu `bool`
- `a` thuộc kiểu `int`, `b` thuộc kiểu `bool`, `c`thuộc kiểu `str`

`@hint`
Sử dụng `type(a)`, `type(b)`, `type(c)`  để kiểm tra.

`@pre_exercise_code`
```{python}
a = 100*1.1**7
b = "True"
c = False
```

`@sct`
```{python}
msg1 = "`a` Không phải kiểu `int`."
msg2 = "`b` Không phải kiểu `bool`, nó là kiểu `str`! Vì True nằm trong nháy kép "
msg3 = "Chính xác!"
msg4 = "Không có khẳng định nào là đúng trong câu này."
Ex().has_chosen(3,[msg1, msg2, msg3, msg4])
```

---

## Một số thao tác trên chuỗi

```yaml
type: NormalExercise
key: 4d0d83cc02
lang: python
xp: 100
skills: 2
```

Thao tác cộng chuỗi khác với cộng trên số. Thao tác này sẽ làm chuỗi của bạn được thêm vào 1 chuỗi giống hệt chuỗi trước đó.
Tương tự với thao tác nhân.

`@instructions`
-  Sử dụng thao tác cộng `msg` và `msg` và lưu giá trị vào `double_msg`
- In ra kiểu của biến `double_msg`, sử dụng `type()`
- Sử dụng thao tác nhân `msg` với `3`  và lưu giá trị vào `triple_msg`
- Xuất ra giá trị của `triple_msg`

`@hint`
- `double_msg  = msg + msg`.
- Để in ra kiểu của biến  `x`, sử dụng `print(type(x))`.
-  `triple_msg = msg * 3`.
- Để in ra giá trị của biến `x`, sử dụng `print(x)`.

`@sample_code`
```{python}
msg = "Hello World!"

# Sử dụng thao tác cộng msg và msg và lưu giá trị vào double_msg

# In ra kiểu của biến double_msg

# Sử dụng thao tác nhân msg với 3  và lưu giá trị vào triple_msg

# Xuất ra giá trị của triple_msg
```

`@solution`
```{python}
msg = "Hello World!"
# Sử dụng thao tác cộng msg và msg và lưu giá trị vào double_msg
double_msg = msg + msg
# In ra kiểu của biến double_msg
print(type(double_msg))
# Sử dụng thao tác nhân msg với 3 và lưu giá trị vào triple_msg
triple_msg = msg * 3
# Xuất ra giá trị của triple_msg
print(triple_msg)
```

`@sct`
```{python}
# predefined
msg = "Vui lòng đừng xóa biến msg."
Ex().check_object('msg', missing_msg=msg).has_equal_value(incorrect_msg=msg)
# check year1 and printout
msg2 = "Bạn đã thực hiện thao tác cộng chưa"
Ex().multi(
    check_object("double_msg").has_equal_value(incorrect_msg=msg2),
    has_printout(0, not_printed_msg = "__JINJA__:Sử dụng `{{sol_call}}` Xuất ra kiểu của `double_msg`.")
)
msg3 = "Bạn đã thực hiện thao tác nhân chưa"
# check doubledesc and prinout
Ex().multi(
    check_object("triple_msg").has_equal_value(incorrect_msg = msg3),
    has_printout(1, not_printed_msg = "Đừng quên xuất giá trị của `triple_msg`.")
)

success_msg("Tốt.")
```

---

## Ép kiểu

```yaml
type: NormalExercise
key: 085bb602b9
lang: python
xp: 100
skills: 2
```

Ở bài học 6, từ số tiền `savings` ta tính được số tiền sở hữu sau `year` năm được lưu vào biến `result` và chỉ xuất ra được con số duy nhất. Vậy để in ra một kết quả có kèm theo chuỗi thông báo là :  

> "sau `year` năm từ số tiền `savings` ban đầu, chúng ta có thể kiếm được  `result`$ "

Bằng cách sử dụng toán tử `+` giữa các chuỗi, ta có thể xuất ra một câu tùy chỉnh:

```
print("sau" + year + "năm từ số tiền " + savings +"$ ban đầu, chúng ta có thể kiếm được " + result + "$")
```

Câu lệnh trên sẽ báo sai bởi vì chúng ta không thể cộng một chuỗi và 1 số .

Để sửa lỗi này bạn chỉ cần ép kiểu số về kiểu chuỗi [`str()`](https://docs.python.org/3/library/functions.html#func-str).
Ví dụ `str(year)` sẽ ép kiểu số của biến `year` về kiểu chuỗi.

Tương tự ta cũng có các hàm [`int()`](https://docs.python.org/3/library/functions.html#int), [`float()`](https://docs.python.org/3/library/functions.html#float) và [`bool()`](https://docs.python.org/3/library/functions.html#bool) để ép kiểu dữ liệu.

`@instructions`
- Nhấn _Run Code_ để xem thông báo lỗi 
- sửa code bằng cách sử dụng hàm [`str()`](https://docs.python.org/3/library/functions.html#func-str) để ép kiểu số sang chuỗi.
- ép kiểu của biến `pi_string` từ chuỗi sang số và gán vào biến `pi_float`.

`@hint`
- Bạn nên sử dụng [`str()`](https://docs.python.org/3/library/functions.html#func-str)!
- Bạn nên sử dụng [`float()`](https://docs.python.org/3/library/functions.html#float) để ép kiểu cho  `pi_string` và lưu nó vào `pi_float`.

`@sample_code`
```{python}
# Cho trước các biến
savings = 100
year = 7
result = 100 * 1.10 ** 7
# Sửa code cho đúng 
print("sau " + year + " năm từ số tiền " + savings +"$ ban đầu, chúng ta có thể kiếm được " + result + "$")
# Khởi tạo biến pi_string
pi_string = "3.1415926"
# Ép kiểu của pi_string về float: pi_float
```

`@solution`
```{python}
# Cho trước các biến
savings = 100
year = 7
result = 100 * 1.10 ** 7
# Sửa code cho đúng 
print("sau " + str(year) + " năm từ số tiền " + str(savings) +"$ ban đầu, chúng ta có thể kiếm được " + str(result) + "$")
# Khởi tạo biến pi_string
pi_string = "3.1415926"
# Ép kiểu của pi_string về float: pi_float
pi_float = float(pi_string)
```

`@sct`
```{python}
# ensure predefined values are unmodified
msg = "Không nên xóa các biến đã được tạo sẵn."
Ex().multi(
    check_object("savings", missing_msg=msg).has_equal_ast(incorrect_msg=msg),
  	check_object("year", missing_msg=msg).has_equal_ast(incorrect_msg=msg),
    check_object("result", missing_msg=msg).has_equal_ast(incorrect_msg=msg)
)

Ex().check_correct(
    has_printout(0),
    multi(
      	check_function("str", 0).check_args(0).has_equal_value(incorrect_msg="Hãy chắc chắn rằng bạn đã ép kiểu của biến `year` về kiểu chuỗi bằng `str(year)`."),
        check_function("str", 1).check_args(0).has_equal_value(incorrect_msg="Hãy chắc chắn rằng bạn đã ép kiểu của biến `savings` về kiểu chuỗi bằng `str(savings)`."),
        check_function("str", 2).check_args(0).has_equal_value(incorrect_msg="Hãy chắc chắn rằng bạn đã ép kiểu của biến `result` về kiểu chuỗi bằng `str(result)`."),
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

success_msg("Tuyệt")
```

---

## Tổng kết chương 1

```yaml
type: MultipleChoiceExercise
key: 3e5f0bdf3a
lang: python
xp: 50
skills: 2
```

Câu hỏi trắc nghiệm cuối chương. Đáp án nào là  không chính xác

Bạn có thể copy các dòng lệnh và chạy nó trong khung _IPython Shell_ để kiểm tra kết quả

`@instructions`
- `"Có thể ép kiểu của số "  + str(5) + " sang string."`
- `"Có một con muỗi kêu " + ("vove " * 3) + "love"+ ("vove " * 5)`
- `"Câu trả lời đúng là câu số " + 2`
- `True + False`

`@hint`
Bạn có thể copy các dòng lệnh và chạy nó trong khung _IPython Shell_ để kiểm tra kết quả

`@pre_exercise_code`
```{python}

```

`@sct`
```{python}
msg1 = "Chưa chính xác, Câu lệnh này hoàn toàn hợp lệ."
msg2 = "Chưa chính xác, Câu lệnh này hoàn toàn hợp lệ."
msg3 = "Chính xác! bởi vì bạn chưa ép kiểu số `2` sang string sử dụng [`str()`](https://docs.python.org/3/library/functions.html#func-str), this will give an error."
msg4 = "`True + False` Không sai. Khi thực hiện phép `+` các giá trị boolean, Python sẽ tự động ép về kiểu số "
Ex().has_chosen(3, [msg1, msg2, msg3, msg4])
```
