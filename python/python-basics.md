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

The first function is main.  This is used to denote where the program should start execution.  By default, a function needs to be defined before it can be used.  By using main, the function execution is deferred until the program is loaded.  

The last line of code tells the compiler that if this program is being included in another module, do not execute main.

The style guide follows PEP-8, a common Python styling guide.  

The function primes has a default argument, n=1.  The while\(True\) creates an infinite loop.  If 

