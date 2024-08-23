# Mihir's First CS193 Homework

## Favorite Things About CS193
- Programming!
- Being in the physics building
- The lecturers

## Fun Code
Here's a small program I just wrote to test the Collatz Conjecture! The method below uses BigIntegers to handle much larger numbers: `((2^32)^Integer.MAX_VALUE))`. The Collatz Conjecture (or the 2n+1) is one of the most famous math problem that has never been proven yet, and you can potentially win 120 million Japanese Yen to find a number that disproves this conjecture. Essentially, you start with a number `n` and if it is even, divide by 2, and otherwise, if odd, you apply `2n+1`.
```
public static long collatzConjectureTest(BigInteger number) {
    long counter = 0L;

    for(BigInteger aNum = number; !aNum.equals(new BigInteger("1")); ++counter) {
        aNum = aNum.mod(new BigInteger("2")).equals(new BigInteger("0")) ? aNum.divide(new BigInteger("2")) : aNum.multiply(new BigInteger("3")).add(new BigInteger("1"));
    }

    return counter;
}
```
This function returns the number of steps it took to reach 1.

## Support or Contact

Reach me at [my email](mailto:chauhanm@purdue.edu)! Thanks
