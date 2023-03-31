#!/usr/bin/python3
""" Factorise number in a file into a product of two prime number """
import sys

def factorize():
    """
    A function to search file and factirize the given set of numbers
    """
    try:
        file = sys.argv[1]
        with open(file) as f:
            for line_number in f:
                line_number = int(line_number)
                if line_number % 2 == 0:
                    print("{}={}*{}".format(line_number, line_number // 2, 2))
                    continue
                i = 3
                while i < line_number // 2:
                    if line_number % i == 0:
                        print("{}={}*{}".format(line_number, line_number // i, i))
                        break
                i = i + 2
                if i == (line_number // 2) + 1:
                    print("{}={}*{}".format(line_number, line_number, 1))
    except (IndexError):
        pass

factorize()
