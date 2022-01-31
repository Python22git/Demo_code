class PowTwo:
   """Class to implement an iterator
   of powers of two"""

   def __init__(self, max=0):
      self.max = max

   def __iter__(self):
      self.n = 0
      return self

   def __next__(self):
      if self.n <= self.max:
         result = 2 ** self.n
         self.n += 1
         return result
      else:
         raise StopIteration


# create an object
numbers = PowTwo(3)

# create an iterable from the object
i = iter(numbers)

# Using next to get to the next iterator element
print(next(i))
print(next(i))
print(next(i))
print(next(i))
print(next(i))

import  sys
sys.exit(0)


import random

while True:
   input("Press enter to roll the dice")

   # get a number between 1 to 6
   num = random.randint(1,6)
   print("You got",num)
   option = input("Roll again?(y/n) ")

   # condition
   if option == 'n':
       break

import sys
sys.exit(0)


vowels = "aeiouAEIOU"
while True:
   v = input("Enter a vowel: ")
   # condition in the middle
   if v in vowels:                       #if the entered letter is match with vowels then print thank you
       break                             # if entered value is notin vowels then print That is not a vowel. Try again!
   print("That is not a vowel. Try again!")

print("Thank you!")


import sys
sys.exit(0)


n = 10
sum = 0
i = 1
while i <= n:
   sum = sum + i
   i = i+1

print("The sum is",sum)