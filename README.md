
def fibonacci_generator(n):
    a, b = 0, 1
    count = 0

    while count < n:
        yield a
        a, b = b, a + b
        count += 1

# Example: Generate the first 10 Fibonacci numbers
n = 10
fibonacci_sequence = list(fibonacci_generator(n))
print(f"The first {n} Fibonacci numbers are: {fibonacci_sequence}")
