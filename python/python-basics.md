# Basic Syntax

```py
def main():
    for n in primes():
        if n > 100: 
            break
        print(n)


def isprime(n):
    if n == 1:
        return False
    for x in range(2, n):
        if n % x == 0:
            return False
    else:
        return True


def primes(n=1):
    while (True):
        if isprime(n): 
            yield n
        n += 1


if __name__ == "__main__": main()
```

The first function is `main`.  This is used to denote where the program should start execution.  By default, a function needs to be defined before it can be used.  By using `main`, the function execution is deferred until the program is loaded.

The last line of code tells the compiler that if this program is being included in another module, do not execute `main`.

There are two uses of the equals operator.  The first, when used by itself, is to create an assignment.  `y = 1` means that the variable y will hold the value 1.  The double equals operator means is equal to.  `y == 1` means "Is y equal to the value 1".  It's a common programming error to use a single equals sign instead of a double equals sign.

The style guide follows `PEP-8`, a common Python styling guide.

The function `primes` has a default argument, `n=1`.  The `while(True)` creates an infinite loop.  If this isn't exited via a `break` statement, it will execute forever and crash the Python interpreter.

The `n +=1` means "Take the current value of n and add one to it.".  You will see the post-increment operator in several other languages look like this `++` and has the same meaning.

The function `isprime` takes an argument of `n`, used to denote number.  If the number is 1, it returns false.  The `for in range` loop generates a range of numbers, the min number on the left hand side and the max number on the right hand side.  The value of x on each iteration of the loop will be the next number in the range.

```
for x in range(2, 5):
    if n % 2 == 0: return False
    if n % 3 == 0: return False
    if n % 4 == 0: return False
    if n % 5 == 0: return False
```

The `%` operator means "modulus" and it's used when dividing integers to see if there is a remainder.  If a value can divide into the prime number and not leave a remainder, then it is not a prime number.

