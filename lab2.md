# Дорогие друзья,
'''
#1
def convert_types(data):
	for i in range(len(data), 1):
		pass

#2		
def swap_values(a, b):
	a, b = b, a
	return (a, b)
	
#3
def bool_transform(value = False):
	if value:
		return True
	else: return False

#4
def compound_operations(a, b):
	add = a+b
	subtr = a-b
	mult = a*b
	divide = a/b
	whole = a//b
	remainder = a%b
	power = a**b
	return [add, subtr, mult, divide, whole, remainder, power]

#5
def check_type(value, expected_type):
	if type(value).__name__ == type(expected_type).__name__:
		return True
	else: return False

#6
def logical_and(a, b, c):
	if a:
		if b:
			if c:
				return True
			else: return False
		else: return False
	else: return False

#7
def logical_or(a, b, c):
	if a:
		return True
	else:
		if b:
			return True
		else:
			if c:
				return True
			else: return False

#8
def is_between(value, low, high):
			if value>low and value<high:
				return True
			else: return False

#9
def print_even_numbers(n):
	for i in range(1, n+1, 1):
		if i % 2 == 0:
			print (i)

#10
def countdown_while(n):
	while n > 1:
		print(n)
		n -=1
		if n == 1:
			print(n)
			break

#11
def skip_multiples(n, multiple):
	for i in range(1, n+1, 1):
			if i%multiple == 0: continue
			print(i)

#12
def if_elif_else_chain(x):
	if x > 0: return "positive"
	elif x < 0: return "negative"
	else: return "zero"

#13
def abs_value(x):
	if x >= 0: return x
	else: return x * -1
	
#14
def binary_representation(x):
	pass

#15
def custom_round(num, ndigits):
	return int(num * 10**ndigits) / 10**ndigits

#16
def find_max_min(num):
	for i in num:
		pass
		
#17
def all_true(iterable):
	for i in iterable:
		if i:
			return False
			break


#18
def any_true(iterable):
	for i in iterable:
		if i:
			return True
			break

#19
def custom_enumerate(seq, start = 0):
	arr = []
	for i in seq:
		arr.append((start+1, i))
		start += 1
	return arr
	
#25
def sum_digits(n):
	s = 0
	while n // 10 > 0:
		s += n%10
		n // 10
	return s
	
#30
def fibonacci(n):
	a = 0
	b = 1
	c = 0
	while c < n-1:
		s = a + b
		a = b
		b = s
		c += 1
	return b
  '''
  # Спасибо за внимание.
