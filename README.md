# Password-Generator
Password Generator Using Python
import random
letters=['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z','A','B','C','D','E','F','F','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z']
numbers=['0','1','2','3','4','5','6','7','8','9']
symbols=['!','#','$','@','%','^','&','*','(',')','+','-']
print("Welcome to password Generator:")
nletters=int(input("How Many Letters you want in your password ?\n "))
nsymbols=int(input("How Many Symbols you want in your password ?\n "))
nnumbers=int(input("How Many numbers you want in your password ?\n "))

password=""
for i in range(1,nletters+1):
    char=random.choice(letters)
    password=password+char;
for i in range(1,nsymbols+1):
    char=random.choice(symbols)
    password=password+char;
for i in range(1,nnumbers+1):
    char=random.choice(numbers)
    password=password+char
print(password)
