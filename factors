#!/usr/bin/python3
import sys
def facto(number):
    factors = []
    for i in range(2, number // 2 + 1):
        if number % i == 0:
            factors.append((i, number // i))
            break
    return factors

def main(input_file):
    with open(input_file, 'r') as file:
        for line in file:
            number = int(line.strip())
            factors = facto(number)
            if factors:
                p, q = factors[0]
                print(f"{number}={p}*{q}")

if __name__ == "__main__":
    if len(sys.argv) != 2:
        print("Usage: python factors.py <file>")
        sys.exit(1)

    input_file = sys.argv[1]
    main(input_file)
