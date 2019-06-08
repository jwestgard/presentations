---
title: Tools and Techniques for a Repository-Centric Architecture with Fedora
subtitle: Open Repositories 2019
revealjs-url: lib/reveal
theme: inst326
transition: slide
---

# 

::: {.left}
Python is an [imperative] programming language. Your programs are a series
of **Statements** that are executed in order.

Each **Statement** can be made up of
**Variables** and **Expressions**.

**Conditional Statements** change the execution
of your program depending on the state of **Variables** and **Expressions**.
:::

::: fragment

---
*This is a lot, so let's unpack it.*

:::

# What are Variables?

<p class="left">
Variables are *names* that can be attached to *data*. Each variable has a *type*:
</p>

::: incremental

* Integer: x = 1
* Float: x = 1.5
* String: x = "umd"
* Boolean: x = True

:::

<p class="left fragment">
We'll be talking about more complex types (e.g. *lists*, *dictionaries*, *sets*) and 
even how to create your own over the course of the semester.
</p>

# Working with Variables

There are two main actions we take with variables:

* *assignment*: attach a name to some data
* *evaluation*: lookup the data by its name

# Practice with Variables

~~~~ {.python .numberLines}
# assignment
x = "Hello World"

# evaluation
print(x) 
~~~~

::: fragment
Notice the use of comments on lines 1 and 4?
:::

# What are Expressions?

Expressions are pieces of Python that get *evaluated*, and are often 
created with *operators*: 

::: columns 

:::: column

- addition (+)
- subtraction (-)
- multiplication (\*)
- division (/)

::::

- integer division (//)
- modulo (%)
- exponentiation (**)
- equality (==)

:::

Remember order of operations: [PEMDAS](https://www.mathsisfun.com/operation-order-pemdas.html)

# Practice with Expressions

# 

~~~ {.python .numberLines}
x = 2 
x * x
~~~

::: fragment
**4**
:::

# 

~~~ {.python .numberLines}
x = 2
x ** 3
~~~ 

::: fragment
**8**
:::

#

~~~ {.python .numberLines}
x = 2 
y = 3
x == y
~~~

::: fragment
**False**
:::

# 

~~~ {.python .numberLines}
x = 80
y = 30
x - y
~~~

::: fragment
**50**
:::

#

~~~ {.python .numberLines}
x = 2
y = 3
y - x + 4
~~~

::: fragment
**5**
:::

# 

~~~ {.python .numberLines}
x = 2
2 + x ** 3
~~~

::: fragment
**10**
:::

# 

Operators behave differently depending on the *type*:

``` python
"u" + "m" + "d"
```

::: {.fragment}
**umd**
:::

::: fragment
```python
"umd " * 5
```
:::

::: fragment
**umd umd umd umd umd**
:::

# What are Statements?

* Statements are the most basic units of executable Python code.
* A Python program is a series of statements executed in order.

#

Try these statements to input and print a variable:

~~~~ {.python .numberLines}
username = input("Enter your name: ")
print("Hello", username)
~~~~

# What are Conditionals?

* In practice, you often do not want every *statement* in a program to be executed every time.
* Instead, you want your program to execute depending on the logical state of data or input when your program is running.
* The basic building blocks for this logic are conditionals, which are constructed with the keywords *if*, *else* and *elif*.

# Structure of Conditionals

``` {.python .numberLines}
if 1 > 0:
    print("yes")
else:
    print("no")
```

::: fragment
**yes**
:::

::: notes
* Conditionals are different from statements in that they are multi-statement structures of code
* The fist line of a conditional block begins with one of the if/elif/else keywords followed by an expression
* The first line ends with a colon
* This first line is followed by an indented block of one or more lines of code
* The indented block is only executed if the expression in the first line evaluates as "True"

:::


# Practice with Conditionals

~~~~ {.python .numberLines}
order = input("What can I get you? ")

if order == "burger":
    side = input("Would you like fries? ")
elif order == "salad':
    side = input("What kind of dressing? ")
else:
    print("We only sell burgers and salads.")

print("You ordered:", order, side)

~~~~

# So ...

<p class="left">
We've covered a lot but now you know the basic buiding blocks of all Python
programs, and [imperative] programming languages in general:
</p>

* Statements
* Variables
* Types
* Operators 
* Expressions
* Conditionals

[imperative]: https://en.wikipedia.org/wiki/Imperative_programming
