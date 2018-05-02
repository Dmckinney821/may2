# may2

Online presence
Do's and Don'ts
Slack channels that can help with job search
LinkedIN work
Stack Overflow
class Cart(object):
    def __init__(self):
        print('New shopping cart created')
        self.items = []

    def add(self,product):
        self.items.append

    def total(self):
        amount = 0
        for product in self.items:
            amount = amount + product.price()

        return amount

    def description(self):
        final_description = ''
    
        for product in self.items:
            final_description = final_description + product.price()
        return final_description
class Product(object):
    def __init__(self, price, name):
        self.price = price
        self.name = name
        
    def description(self):
        return '%s: %d' % (self.name, self.price)
Last login: Tue May  1 11:37:08 on ttys000
$ ipython
Python 2.7.14 |Anaconda, Inc.| (default, Dec  7 2017, 11:07:58) 
Type "copyright", "credits" or "license" for more information.

IPython 5.4.1 -- An enhanced Interactive Python.
?         -> Introduction and overview of IPython's features.
%quickref -> Quick reference.
help      -> Python's own help system.
object?   -> Details about 'object', use 'object??' for extra details.

In [1]: my_file = open('lalallalalalla.dat', 'ab+') 

In [2]: my_file
Out[2]: <open file 'lalallalalalla.dat', mode 'ab+' at 0x1068688a0>

In [3]: pickle.dump(my_character, my_file)
---------------------------------------------------------------------------
NameError                                 Traceback (most recent call last)
<ipython-input-3-e12affe341dc> in <module>()
----> 1 pickle.dump(my_character, my_file)

NameError: name 'pickle' is not defined

In [4]: import pickle

In [5]: pickle.dump(my_character, my_file)
---------------------------------------------------------------------------
NameError                                 Traceback (most recent call last)
<ipython-input-5-e12affe341dc> in <module>()
----> 1 pickle.dump(my_character, my_file)

NameError: name 'my_character' is not defined

In [6]: my_character = my_file

In [7]: pickle.dump(my_character, my_file)
---------------------------------------------------------------------------
TypeError                                 Traceback (most recent call last)
<ipython-input-7-e12affe341dc> in <module>()
----> 1 pickle.dump(my_character, my_file)

/Users/danielmckinney/anaconda2/lib/python2.7/pickle.pyc in dump(obj, file, protocol)
   1374 
   1375 def dump(obj, file, protocol=None):
-> 1376     Pickler(file, protocol).dump(obj)
   1377 
   1378 def dumps(obj, protocol=None):

/Users/danielmckinney/anaconda2/lib/python2.7/pickle.pyc in dump(self, obj)
    222         if self.proto >= 2:
    223             self.write(PROTO + chr(self.proto))
--> 224         self.save(obj)
    225         self.write(STOP)
    226 

/Users/danielmckinney/anaconda2/lib/python2.7/pickle.pyc in save(self, obj)
    304             reduce = getattr(obj, "__reduce_ex__", None)
    305             if reduce:
--> 306                 rv = reduce(self.proto)
    307             else:
    308                 reduce = getattr(obj, "__reduce__", None)

/Users/danielmckinney/anaconda2/lib/python2.7/copy_reg.pyc in _reduce_ex(self, proto)
     68     else:
     69         if base is self.__class__:
---> 70             raise TypeError, "can't pickle %s objects" % base.__name__
     71         state = base(self)
     72     args = (self.__class__, base, state)

TypeError: can't pickle file objects

In [8]: exit
$ pwd
/Users/danielmckinney
$ ls
99bottle.py		Public			lalallalalalla.dat
Applications		README.md		lpthw
Dan			ReduxSimpleStarter	manual
Desktop			SubmitAlerter		missing
DigitalCrafts-04-2018	WebstormProjects	n
Documents		anaconda2		p
Downloads		cc_validator		playground
Library			css			src
Movies			directory_1		temp
Music			github			the
Pictures		hello			uninstall-node.sh
$ import piclkle
-bash: import: command not found
$ import pickle
-bash: import: command not found
$ import pickle
-bash: import: command not found
$ ipython
Python 2.7.14 |Anaconda, Inc.| (default, Dec  7 2017, 11:07:58) 
Type "copyright", "credits" or "license" for more information.

IPython 5.4.1 -- An enhanced Interactive Python.
?         -> Introduction and overview of IPython's features.
%quickref -> Quick reference.
help      -> Python's own help system.
object?   -> Details about 'object', use 'object??' for extra details.

In [1]: import pickle

In [2]: my_char_file = open('lalalalall.dat', 'rb')
---------------------------------------------------------------------------
IOError                                   Traceback (most recent call last)
<ipython-input-2-658b317064c4> in <module>()
----> 1 my_char_file = open('lalalalall.dat', 'rb')

IOError: [Errno 2] No such file or directory: 'lalalalall.dat'

In [3]: my_char_file = open('lalallalalalla.dat', 'rb')

In [4]: taserface = pickle.load(my_char_file)
---------------------------------------------------------------------------
EOFError                                  Traceback (most recent call last)
<ipython-input-4-905e49a5f9a6> in <module>()
----> 1 taserface = pickle.load(my_char_file)

/Users/danielmckinney/anaconda2/lib/python2.7/pickle.pyc in load(file)
   1382 
   1383 def load(file):
-> 1384     return Unpickler(file).load()
   1385 
   1386 def loads(str):

/Users/danielmckinney/anaconda2/lib/python2.7/pickle.pyc in load(self)
    862             while 1:
    863                 key = read(1)
--> 864                 dispatch[key](self)
    865         except _Stop, stopinst:
    866             return stopinst.value

/Users/danielmckinney/anaconda2/lib/python2.7/pickle.pyc in load_eof(self)
    884 
    885     def load_eof(self):
--> 886         raise EOFError
    887     dispatch[''] = load_eof
    888 

EOFError: 

In [5]: taserface
---------------------------------------------------------------------------
NameError                                 Traceback (most recent call last)
<ipython-input-5-e2c79c8e1f8b> in <module>()
----> 1 taserface

NameError: name 'taserface' is not defined

In [6]: cart = {}

In [7]: shoes = {}

In [8]: shoes['name'] = 'adidas'

In [9]: shoes
Out[9]: {'name': 'adidas'}

In [10]: shoes['size'] = 10

In [11]: shoes
Out[11]: {'name': 'adidas', 'size': 10}

In [12]: cart['items'] = []

In [13]: cart['items']
Out[13]: []

In [14]: cart['items'].append(shoes)

In [15]: shoes
Out[15]: {'name': 'adidas', 'size': 10}

In [16]: pants = {
    ...: 'brnad
  File "<ipython-input-16-bdc1676d8ff8>", line 2
    'brnad
         ^
SyntaxError: EOL while scanning string literal


In [17]: pants = {
    ...: 'brnad
  File "<ipython-input-17-bdc1676d8ff8>", line 2
    'brnad
         ^
SyntaxError: EOL while scanning string literal


In [18]: pants = {
    ...: 'brand' : 'lucky',
    ...: 'size' : 'wider than i want to admit'
    ...: }

In [19]: cart
Out[19]: {'items': [{'name': 'adidas', 'size': 10}]}

In [20]: cart['items'].append(pants)

In [21]: cart
Out[21]: 
{'items': [{'name': 'adidas', 'size': 10},
  {'brand': 'lucky', 'size': 'wider than i want to admit'}]}

In [22]: class Cart(object):
    ...:     def __init__(self):
    ...:         print('New shopping cart created')
    ...:         

In [23]: my_shopping_cart = Cart()
New shopping cart created

In [24]: my_shopping_cart
Out[24]: <__main__.Cart at 0x10b33ddd0>

In [25]: class Cart(object):
    ...:     def __init__(self):
    ...:         print('New shopping cart created')
    ...:         self.items = []
    ...:         

In [26]: my_shopping_cart = Cart()
New shopping cart created

In [27]: my_shopping_cart.items
Out[27]: []

In [28]: my_shopping_cart.items.append(shoes)

In [29]: my_shopping_cart.items.append(pants)

In [30]: my_shopping_cart.items
Out[30]: 
[{'name': 'adidas', 'size': 10},
 {'brand': 'lucky', 'size': 'wider than i want to admit'}]

In [31]: class Cart(object):
    ...:     def __init__(self):
    ...:         print('New shopping cart created')
    ...:         self.items = []
    ...:     def add(self, product)
  File "<ipython-input-31-39c3ed80a49d>", line 5
    def add(self, product)
                          ^
SyntaxError: invalid syntax


In [32]: class Cart(object):
    ...:     def __init__(self):
    ...:         print('New shopping cart created')
    ...:         self.items = []
    ...:     def add(self, product):
    ...:         self.items.append(product)
    ...:         

In [33]: my_shopping_cart = Cart()
New shopping cart created

In [34]: my_shopping_cart.items
Out[34]: []

In [35]: my_shopping_cart.add(shoes)

In [36]: my_shopping_cart.add(pants)

In [37]: my_shopping_cart.items
Out[37]: 
[{'name': 'adidas', 'size': 10},
 {'brand': 'lucky', 'size': 'wider than i want to admit'}]

In [38]: 
