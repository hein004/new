# Guessing number

import random
a= random.randint(1,9)

count =0

invalid =True
while invalid:
    guess=input('guess an integer between 1-9')
    if guess=='exit':
        print('Better Luck Next Time')
        break
    else:
        ''
    guess=int(guess)
    if guess==a:
        count=count+1
        print('congratz! it is',a)
        print('you took only',count,'tries')
        invalid=False
    elif guess>a:
        count=count+1
        print('Too high')
    elif guess<a:
        count=count+1
        print('Too low')
    elif guess=='exit':
        break
    else:
        ''
