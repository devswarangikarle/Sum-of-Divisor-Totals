# Sum-of-Divisor-Totals

Ethan is exploring numbers and their divisors. Given a positive integer N, he wants to calculate the total sum of divisors for every number from 1 to N. For each number i, he defines F(i) as the sum of all divisors of i. Ethan’s goal is to find the combined value of F(i) for all numbers from 1 to N. Can you help him compute this total sum?

def sum_of_divisor_totals(n):
    total_sum = 0
    for d in range(1, n + 1):
        total_sum += d * (n // d)
    return total_sum

# Input
n = int(input().strip())

# Output
print(sum_of_divisor_totals(n))
