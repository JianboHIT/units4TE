### Part IV: 数据模板

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;这里展示了一个按列排放的数据模板（示例文件：
*[DataTemplate.txt](DataTemplate.txt)*
）。文件中每列数据对应一个物理量，具有相同的物理单位，而且每列的数据个数是一样的。
数据的分隔符可以是空格或者制表符，文件名以 .txt 为扩展名。
文件中以 "#" 号开头的行通常用来表示注解信息，比如日期，每列的变量名称、单位，
个人的备注信息等。这种格式的文件可以被绝大多数文本编辑器处理，而且可读性较好。

```
# Here are some comments. 
# Multiple lines of comments are allowed, but they must 
# all begin with the "#" character.
# Blank lines will be ignored (as shown below).

# property1   property2   property3   property4
300      0.0236       -51.33     9.3760e+01
323      0.0214       -40.33     9.9980e+01
373      0.0227       -8.53      9.6227e+01
423      0.0218        3.11      1.0170e+02
473      0.0228        18.29     9.7098e+01
523      0.0220        24.54     9.6694e+01
573      0.0217        54.92     1.0055e+02
623      0.0232        39.55     9.3134e+01
# Comments are also allowed to be inserted inside data blocks,
# as long as they start with a "#" sign as such.
673      0.0215        23.34     9.4004e+01
723      0.0235        0.13      8.3193e+01
773      0.0220       -16.76     9.7579e+01
823      0.0216       -48.61     9.9000e+01
873      0.0218       -93.34     1.0131e+02

# Here is a comment at the end of the file.
```


### Part IV: Data Template

&nbsp;&nbsp;&nbsp;&nbsp;Here is a recommended template file to save 
column-indexed block-datas (see a example 
*[DataTemplate.txt](DataTemplate.txt)*
). Each column of data in the file corresponds to a property, 
they share the same unit, and the number of data samples in each column 
is the same. The file is delimited by spaces or tabs in the data block, 
and the filename has .txt as its extension. Lines starting with "#" in 
the file are usually interpreted as some comment information, such as date, 
author, variable name of each column, unit, personal comment information, etc. 
Data files in this format are highly readable and can be processed by most text editors.

```
# Here are some comments.
# Multiple lines of comments are allowed, but they must
# all begin with the "#" character.
# Blank lines will be ignored (as shown below).

# property1   property2   property3   property4
300      0.0236       -51.33     9.3760e+01
323      0.0214       -40.33     9.9980e+01
373      0.0227       -8.53      9.6227e+01
423      0.0218        3.11      1.0170e+02
473      0.0228        18.29     9.7098e+01
523      0.0220        24.54     9.6694e+01
573      0.0217        54.92     1.0055e+02
623      0.0232        39.55     9.3134e+01
# Comments are also allowed to be inserted inside data blocks,
# as long as they start with a "#" sign as such.
673      0.0215        23.34     9.4004e+01
723      0.0235        0.13      8.3193e+01
773      0.0220       -16.76     9.7579e+01
823      0.0216       -48.61     9.9000e+01
873      0.0218       -93.34     1.0131e+02

# Here is a comment at the end of the file.
```
