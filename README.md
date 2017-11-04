# python

Microsoft Windows [Version 6.2.9200]
(c) 2012 Microsoft Corporation. All rights reserved.

C:\Users\Admin>python
Python 3.6.3 (v3.6.3:2c5fed8, Oct  3 2017, 17:26:49) [MSC v.1900 32 bit (Intel)]
 on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> import os
>>> os.path.basename(os.path.dirname(os.path.realpath(_file_)))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name '_file_' is not defined
>>> os.path.basename(os.path.dirname(os.path.realpath(__file__)))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name '__file__' is not defined
>>> 2+2
4
>>> 50-5*6
20
>>> a,b=0,1
>>> while b<10:
... print(b)
  File "<stdin>", line 2
    print(b)
        ^
IndentationError: expected an indented block
>>> while b<10:
...     print(b)
...     a,b=b, a+b
...
1
1
2
3
5
8
>>> import os
>>> print(os.getcwd())
C:\Users\Admin
>>>
KeyboardInterrupt
>>> exit
Use exit() or Ctrl-Z plus Return to exit
>>> ^Z


C:\Users\Admin>f:

F:\>python
Python 3.6.3 (v3.6.3:2c5fed8, Oct  3 2017, 17:26:49) [MSC v.1900 32 bit (Intel)]
 on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> print(os.getcwd())
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'os' is not defined
>>> import os
>>> print(os.getcwd())
F:\
>>> import os
>>> files = [f for f in os.listdir('.') if os.path.isfile(f)]
>>> for f in files:
...     print(f.name)
...
Traceback (most recent call last):
  File "<stdin>", line 2, in <module>
AttributeError: 'str' object has no attribute 'name'
>>> import os
>>> files = [f for f in os.listdir('.') if os.path.isfile(f)]
>>> for f in files:
...     print(f)
...
6215ijmpict04.pdf
Android Slide Next Ver-Jan 2016.pdf
Destop.psd
eclipse-inst-win64.exe
Firefox Setup 49.0.exe
inewsletter-sc-002.doc
Iphone-sagar-taxi-service-dfd.png
mysql-connector.jar
paresh_First.rar
raj.oxps
Ravi_NET.zip
sagar_network_sheet.xlsx
Thumbs.db
>>> import os
>>> files = [f for f in os.listdir('.') if os.path.isfile(f)]
>>> for f in files:
...     fo=open(f)
...     if fo.name == "Thumbs.db":
...         print(f)
...
Thumbs.db
>>> import os
>>> files = [f for f in os.listdir('.')]
>>> for f in files:
...     print(f)
...
$RECYCLE.BIN
6215ijmpict04.pdf
Android Slide Next Ver-Jan 2016.pdf
AnkitSodha
Backup_Tops
Destop.psd
Downloads
eclipse-inst-win64.exe
english grammer
Exam
Firefox Setup 49.0.exe
inewsletter-sc-002.doc
Iphone-sagar-taxi-service-dfd.png
MACOS
MaterialSiblingTabs
merge
MExam
MyRadioApplication
mysql-connector
mysql-connector.jar
paresh_First
paresh_First.rar
raj.oxps
Ravi_NET
Ravi_NET.zip
RecyclerViewWithPopup
RFFlow Full version
sagar_network_sheet.xlsx
Softwares
System Volume Information
Thumbs.db
ViewPagerExample
WdSoftwares
>>> fo=open("test.txt")
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
FileNotFoundError: [Errno 2] No such file or directory: 'test.txt'
>>> import os
>>> files = [f for f in os.listdir('.')]
>>> for f in files:
...     print(f)
...
$RECYCLE.BIN
6215ijmpict04.pdf
Android Slide Next Ver-Jan 2016.pdf
AnkitSodha
Backup_Tops
Destop.psd
Downloads
eclipse-inst-win64.exe
english grammer
Exam
Firefox Setup 49.0.exe
inewsletter-sc-002.doc
Iphone-sagar-taxi-service-dfd.png
MACOS
MaterialSiblingTabs
merge
MExam
MyRadioApplication
mysql-connector
mysql-connector.jar
paresh_First
paresh_First.rar
raj.oxps
Ravi_NET
Ravi_NET.zip
RecyclerViewWithPopup
RFFlow Full version
sagar_network_sheet.xlsx
Softwares
System Volume Information
test.txt.txt
Thumbs.db
ViewPagerExample
WdSoftwares
>>> fo=open('test.txt')
>>> print(fo.read())
hi
>>> fo=open('test.txt','a+')
>>> fo.write('how are you')
11
>>> fo.read()
''
>>> fo=open('test.txt','a+')
>>> fo.write("hi")
2
>>> fo=open("test.txt")
>>> print(fo.read())
hihow are youhi
>>> fo=open('test.txt','a+')
>>>
>>>
>>> print(fo)
<_io.TextIOWrapper name='test.txt' mode='a+' encoding='cp1252'>
>>> fo.close()
>>> fo=open("test.txt")
>>> for line in fo:
...     newline=str(line)
...     print(newline)
...
a, b, 10,20,30

c,d,10,20,30

e,f,10,20,30
>>> fo=open("test.txt")
>>> for line in fo:
...     newline=str(line)
...     lines=newline.split(",")
...     print(lines)
...
['a', ' b', ' 10', '20', '30\n']
['c', 'd', '10', '20', '30\n']
['e', 'f', '10', '20', '30']
>>> for line in fo:
... fo=open("test.txt")
  File "<stdin>", line 2
    fo=open("test.txt")
     ^
IndentationError: expected an indented block
>>> fo=open("test.txt")
>>> for line in fo:
...     newline=str(line)
...     lines=newline.split(",")
...     print(lines[0])
...
a
c
e
>>>
