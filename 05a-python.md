# Learn Python

Read Allen Downey's [Think Python](http://www.greenteapress.com/thinkpython/) for getting up to speed with Python 2.7 and computer science topics. It's completely available online, or you can buy a physical copy if you would like.

<a href="http://www.greenteapress.com/thinkpython/"><img src="img/think_python.png" style="width: 100px;" target="_blank"></a>

For quick and easy interactive practice with Python, many people enjoy [Codecademy's Python track](http://www.codecademy.com/en/tracks/python). There's also [Learn Python The Hard Way](http://learnpythonthehardway.org/book/) and [The Python Tutorial](https://docs.python.org/2/tutorial/).

---

###Q1. Lists &amp; Tuples

How are Python lists and tuples similar and different? Which will work as keys in dictionaries? Why?

>> Lists and Tuples are both data types which contain a series of values. Lists and Tuples differ in the fact that lists are mutable (the values can be changed) and tuples are immutable (values in the tuple cannot be changed). Tuples would work as keys in dictionaries because the keys should be immutable.

---

###Q2. Lists &amp; Sets

How are Python lists and sets similar and different? Give examples of using both. How does performance compare between lists and sets for finding an element. Why?


>> Sets and Lists are both data types which are comprises of a series of values. Lists and Sets differ in the fact that sets can't contain duplicate values, are unordered and can contain only hashable items, as opposed to lists which can have duplicate values, are ordered and can contain non hashable items.
---

###Q3. Lambda Function

Describe Python's `lambda`. What is it, and what is it used for? Give at least one example, including an example of using a `lambda` in the `key` argument to `sorted`.

>> The python's lambda function is used to create anonymous functions with no name. It is used when we require a nameless function for a short period of time and is generally used often as an argument to a higher order function and takes only a single parameter as an argument. They key parameter in the sorted function is used to specify a function to be called on each element prior to making comparisons. The value of the  key parameter should be a function that takes a single argument and returns a key to use for sorting purposes and hence a lamba function is used along with they key parameter.

Example: A common example is to sort complex objects using some of the objects indices as a key:
  >>> student_tuples = [('john','A',15), ('jane','B',12), ('dave','B',10)]
  >>> sorted(student_tuples, key = lambda student: student[2])  # sort by age
  [('dave','B',10),('jane','B',12),('john','A',15)]
  

---

###Q4. List Comprehension, Map &amp; Filter

Explain list comprehensions. Give examples and show equivalents with `map` and `filter`. How do their capabilities compare? Also demonstrate set comprehensions and dictionary comprehensions.

>> List comprehension is an elegant way to define and create lists in python. Essentially it is Python's way of implementing a well-known notation for sets as used by mathematicians. List comprehension is a complete substitute for the lambda function as well as the functions map(), filter() and reduce(). The syntax of list comprehensions is easier to comprehend than map() and filter() functions. Set comprehensions and dictionary comprehensions are similar but returns a set and dictionary respectively and not a list.
Example for list comprehension:
numbersone = [ i for i in range(10) if i%2 ==0]
Equivalent form with map()
nos = [0:9]
def funcc(i):
    if i%2 == 0:
         return i 
    return none
numbersone = map(funcc,nos)
Example for filter() function:
nos = [0:9]
def funcc(i):
    if i%2==0:
        return True
    return False
numbersone = filter(funcc,nos)




---

###Complete the following problems by editing the files below:

###Q5. Datetime
Use Python to compute days between start and stop date.   
a.  

```
date_start = '01-02-2013'    
date_stop = '07-28-2015'
```

>> 937

b.  
```
date_start = '12312013'  
date_stop = '05282015'  
```

>> 513

c.  
```
date_start = '15-Jan-1994'      
date_stop = '14-Jul-2015'  
```

>> 7850

Place code in this file: [q5_datetime.py](python/q5_datetime.py)

---

###Q6. Strings
Edit the 7 functions in [q6_strings.py](python/q6_strings.py)

---

###Q7. Lists
Edit the 5 functions in [q7_lists.py](python/q7_lists.py)

---

###Q8. Parsing
Edit the 3 functions in [q8_parsing.py](python/q8_parsing.py)





