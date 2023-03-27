# 學習JIEBA筆記
## 我猜要先熟悉PYTHON的字串方法
* <span style="color:red">capitalize()</span>第1個字母轉成大寫
```
    >>> saying = 'you can\'t be perfect but you can be unique.'
    >>> saying.capitalize()
    "You can't be perfect but you can be unique."
    >>>
```
* casefold()轉換成小寫，與lower()有些差異，略
* center()	Returns a centered string
```
    >>> saying = 'I come, I see, I conquer.'
    >>> saying.center(40,'-')
    '-------I come, I see, I conquer.--------'
    >>>
```
* count()	Returns the number of times a specified value occurs in a string
```
    >>> saying = 'I come, I see, I conquer.'
    >>> saying.count('I')                   
    3
    >>> saying.count('i')
    0
    >>>
```
* encode()	Returns an encoded version of the string
* endswith()	Returns true if the string ends with the specified value
```
    >>> saying = 'YOU CAN\'T BE PERFECT BUT YOU CAN BE UNIQUE.'
    >>> saying.endswith('que')
    False
    >>> saying.endswith('QUE') 
    False
    >>> saying.endswith('.')   
    True
    >>>
```
* expandtabs()	Sets the tab size of the string
* find()	Searches the string for a specified value and returns the position of where it was found
* format()	Formats specified values in a string
* format_map()	Formats specified values in a string
* index()	Searches the string for a specified value and returns the position of where it was found
* isalnum()判斷字母或數字傳回真假
```
    >>> emailaccount = 'david@greatking.com'
    >>> emailaccount.isalnum()
    False
    >>> emailaccount.isalpha() 
    False
    >>> emailaccount.islower() 
    True
    >>> emailaccount.isupper()
    False
    >>>
```
* isalpha()判斷字母傳回真假
* isascii()	Returns True if all characters in the string are ascii characters
* isdecimal()	Returns True if all characters in the string are decimals
* isdigit()	Returns True if all characters in the string are digits
* isidentifier()	Returns True if the string is an identifier
* islower()	Returns True if all characters in the string are lower case
* isnumeric()判斷數字
```
    >>> X = 123
    >>> S = '123'
    >>> X.isnumeric()
    Traceback (most recent call last):
      File "<stdin>", line 1, in <module>
    AttributeError: 'int' object has no attribute 'isnumeric'
    >>> S.isnumeric()
    True
    >>>
```
* isprintable()	Returns True if all characters in the string are printable
* isspace()	Returns True if all characters in the string are whitespaces
* istitle()	Returns True if the string follows the rules of a title
* isupper()	Returns True if all characters in the string are upper case
* join()	Converts the elements of an iterable into a string
* ljust()	Returns a left justified version of the string
* lower() 轉換成小寫
```
    >>> saying = 'YOU CAN\'T BE PERFECT BUT YOU CAN BE UNIQUE.'
    >>> saying.lower()
    "you can't be perfect but you can be unique."
    >>>
```
* lstrip()將字串左邊的指定字串消除
```
    >>> saying = ' You can\'t be perfect but you can be unique.'
    >>> print(saying.lstrip()) 
    You can't be perfect but you can be unique.
    >>> print(saying.lstrip('You'))
     You can't be perfect but you can be unique.
    >>> print(saying.lstrip(' You'))
    can't be perfect but you can be unique.
    >>>
```
* maketrans()	Returns a translation table to be used in translations
* partition()	Returns a tuple where the string is parted into three parts
* replace()	Returns a string where a specified value is replaced with a specified value
* rfind()	Searches the string for a specified value and returns the last position of where it was found
* rindex()	Searches the string for a specified value and returns the last position of where it was found
* rjust()	Returns a right justified version of the string
* rpartition()	Returns a tuple where the string is parted into three parts
* rsplit()	Splits the string at the specified separator, and returns a list
* rstrip()	Returns a right trim version of the string
* split()斷開字串變成串列，有進階用法
```
    >>> saying = 'I come, I see, I conquer.'                                    
    >>> print(saying.split())
    ['I', 'come,', 'I', 'see,', 'I', 'conquer.']
    >>> print(saying.split(','))
    ['I come', ' I see', ' I conquer.']
    >>> print(saying.split(',',1))
    ['I come', ' I see, I conquer.']
    >>>
```
* splitlines()	Splits the string at line breaks and returns a list
* startswith()判斷字串開始是否為某字串
```
    >>> saying = 'I come, I see, I conquer.'
    >>> print(saying.startswith('i come'))
    False
    >>> print(saying.startswith('I come')) 
    True
    >>> print(saying.startswith('come'))   
    False
    >>>
```
* strip()	Returns a trimmed version of the string
* swapcase()大寫變小寫，小寫變大寫
```
    >>> saying = 'I come, I see, I conquer.'
    >>> print(saying.swapcase())
    i COME, i SEE, i CONQUER.
    >>>
```
* title()字串標題化，每個單字首字母大寫
```
    >>> saying = 'I come, I see, I conquer.'
    >>> print(saying.title())
    I Come, I See, I Conquer.
    >>>
```
* translate()	Returns a translated string
* upper()	轉換成大寫
```
    >>> saying = 'you can\'t be perfect but you can be unique.'
    >>> saying.upper()
    "YOU CAN'T BE PERFECT BUT YOU CAN BE UNIQUE."
    >>>
```
* zfill()	Fills the string with a specified number of 0 values at the beginning
