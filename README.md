import random
import string

def generate_password(num_letters, num_symbols, num_numbers):
     letters = string.ascii_letters
    symbols = string.punctuation
    numbers = string.digits

 password_list = []

 for _ in range(num_letters):
 password_list.append(random.choice(letters))

   for _ in range(num_symbols)
   password_list.append(random.choice(symbols))

for _ in range(num_numbers):
password_list.append(random.choice(numbers))

random.shuffle(password_list)

password = ''.join(password_list)

return password

 num_letters = int(input("Enter the number of letters in the password: "))
 num_symbols = int(input("Enter the number of symbols in the password: "))
 num_numbers = int(input("Enter the number of numbers in the password: "))

 password = generate_password(num_letters, num_symbols, num_numbers)
 print("Generated Password:", password)
