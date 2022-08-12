# Data-Structure-and-Algorithms

Data Structure and Algorithms Implementation with different languages

<!-- ## Started CP: `12/05/2021` -->

## Notes

- Language
  - `int` capacity: `-2 * 10^9` to `2 * 10^9`
  - `long long int` capacity: `-9 * 10^18` to `9 * 10^18`
  - Global Array Size: `10^7`
  - Local Array Size: `10^5`
  - `typeid` operator in c++
- OJ Time Limits
  - Number of iterations in 1 second is : `10^7 to 10^8`
  - `10^8` operation -> `1second`
  - `10^9 -> 10 seconds`
  - `10^10` operation -> `10^10/10^8` or `100seconds`
  - `10^11 -> 1000 seconds`
- Primes and Divisors
  - `log(a^b) = b log(a)`
  - `n << k` -> `n * 2^k`
  - `n >> k` -> `n / 2^k`
  - 2'complement of `~N` = `-((~(~N))+1)` = `-(N+1)`
  - positive integers: `>= 1` and non-negative integers: `>=0`
  - `log6(x) = log_e(x) / log_e(6)`
  - builtin functions
    - `__builtin_popcount(x)`
    - `__builtin_clz(x)`
    - `__builtin_ctz(x)`
  - xor Trick
    - `n ^ (n + 1) == 1 // if n is even`
    - `x ^ 0 == x`
    - `x ^ y == 0 // x == y`
    - `x ^ x ^ x = x // len even`
    - `x ^ x ^ x ^ x = 0 // len odd`
  - BIT LOW: Think about each bit separately. That's it. It will make your life real comfy.
  - The complexity of bitwise operations in bitset of size is O(size/32) or O(size/64)
- Modular Arithmetic
  - Notation:
    - expr1 ≡ expr2(mod m). This is read as "expr1 is congruent to expr2 modulo m", and is shorthand for expr1 mod m=expr2 mod m.
  - Basic arithmetics:
    - `-b % m` = `(m - b) % m`
      - `-4 % 6` = `(6 - 4) % 6`
      - `-49 % 6` = `((-47 % 6) + 6) % 6`
      - finally `-b % m` = `((-b % m) + m) % m`
    - `a % b` = `a - (floor(a/b) * b)`
    - `(a + b) % m` = `(a % m + b % m) % m`
    - `(a - b) % m` = `(a % m - b % m) % m`
    - `(a * b) % m` = `(a % m * b % m) % m`
    - `25 ^ 4 % 10` = `(25 % 10 * 25 % 10 * 25 % 10 * 25 % 10) % 10` = `(5 * 5 * 5 * 5) % 10` = `(5 % 10 * 5 % 10 * 5 % 10 * 5 % 10) % 10`
  - modulo `2^32` and `2^64`
    - `x % 10^k` got last k digit
    - `x % 2^k` got last k bit
    - `x % 2^k` = `x & (2^k - 1)`
    - Note that `x % 2^k` = `x & (2^k - 1)`. So `unsigned int x, y, z; z = x * y` is the same as `z = 1LL * x * y % 2^32`. Similarly `unsigned long long` will automatically take modulo by `2^64`.
  - modular multiplicative inverse
    - mmi defined when `a` and `m` is coprime
    - if `gcd(a, m) == 1` then `a` and `m` is coprime
    - `(a / b) % m` => `(a * b^-1) % m` => `(a % m) * (b^-1 % m) % m`
    - `b^-1 % m` - modular multiplicative inverse of `b`
    - `(a * b) % m = 1` - `b` is mmi of `a` => `((a % m) * (b % m)) % m = 1`
  - fermat's little theorem
    - `a ^ m-1 = 1 % m` -> fermat's little theorem, here `m` is prime and `a` is not multiple of `m`
    - `a^-1 % m = a^m-2` => `a^-1 = a^m-2 % m`
    - `a / b % m` = `a * b^m-2 % m` if `m` is prime
  - intuitive mod
    - x mod m < m / 2 when x >= m.

# Path

## Complexity

- [x] Time complexity
- [x] Space complexity
- [x] O(1)
- [x] O(n)
- [x] O(n^2)
- [x] O(n^3)
- [x] O(sqrt(n))
- [x] O(log(n))
- [x] Logarithm

## Recursion

- [x] print 1 to n
- [x] print n to 1
- [x] sum of array
- [x] sum of n number
- [x] digit sum
- [x] fibonacci
- [x] gcd with recursion
- [x] calculate x of the power y
- [x] reverse string

## Cpp STL

- [x] pair
- [x] vector
- [x] iterator
- [x] string, stringstream
- [x] map, unordered_map
- [x] set, unordered_set, multiset
- [x] bitset
- [x] math.h
- [x] algorithms
- [x] stack
- [x] queue, deque, priority_queue

## Sorting

- [x] selection sort
- [x] bubble sort
- [x] insertion sort
- [x] counting sort
- [x] merge sort
- [x] lexicographical sorting
- [x] std::sort()
- [x] comparator function
- quick sort

## Searching

- [x] linear search
- [x] binary search
- [x] lower bound
- [x] upper bound
- [x] peak element
- [x] first last occurrence
- [x] rotated array
- [x] max in a hill
- [x] square root

## Primes and Divisors

- [x] divisors
- [x] gcd lcm
- [x] primality test
- [x] prime factors
- [x] sieve of eratosthenes
- [x] string multiplication

## Binary Numbers

- [x] base conversion
- [x] bitwise operators
- [x] k-th bit on/off and set/unset
- [x] bit masking
- [x] builtin functions
- [x] xor trick
- [x] bitset
- [x] contribution technique

## Modular Arithmetic

- [x] notation
- [x] basic arithmetics
- [x] binary exponentiation (bigmod)
- [x] modulo `2^32` and `2^64`
- [x] modular multiplicative inverse (modular inverse)
- [x] fermat's little theorem
- [x] mulmod
- [x] \_\_int128
- [x] intuitive mod
- [x] assert function

## Data Structure

- [x] stack
- [x] queue, circular queue

<!-- ## Greedy

## Dynamic programming

- Fibonacci, Shortest path, LIS and Path Printing,
- Longest common subsequence, Coin Change / 0-1 Napsack
- Subset Sam, Combinatorics, Decision Problem
- Matrix Chain Multiplication

## Trees

- Segment Tree 1
- Segment Tree 2
- Binary Indexed Tree

## Graph theory

- Basic of Graph
- Adjacency matrix
- Adjacency list
- Breadth-first search
- Depth First Search
- Topological Sort
- Dijkstra
- Bellman–Ford
- Floyd Warshall
- Minimum Spanning Tree 1, 2
- Maximum flow 1, 2
- Longest path problem
- Strongly connected component

## String

- Rabin-karp string matching
- Knuth–Morris–Pratt (KMP)
- Meet in the middle Technique -->
