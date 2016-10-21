#PRACTICAL 5 - time, math and random module with its functions
#time module
import time
t = time.localtime()
print("Local time is:" ,t)
print("time.asctime(t): %s " % time.asctime(t))
print('The time is:', time.time())
print('The clock time is:', time.clock())
print('The ctime is:', time.ctime())
print('The local time is:', time.sleep(2))

t = (2009, 2, 17, 17, 3, 38, 1, 48, 0)
t = time.mktime(t)
print(time.strftime("%b %d %Y %H:%M:%S", time.gmtime(t)))

print('The time is      :', time.ctime())
later = time.time() + 15
print( '15 secs from now :', time.ctime(later))


print( 'gmtime is %s  :', time.gmtime())
print( 'localtime:', time.localtime())
print( 'mktime   :', time.mktime(time.localtime()))

print("\n")
t = time.localtime()
print( 'Day of month:', t.tm_mday)
print( ' Day of week:', t.tm_wday)
print( ' Day of year:', t.tm_yday)

now = time.ctime()
print (now)
parsed = time.strptime(now)
print (parsed)
print (time.strftime("%a %b %d %H:%M:%S %Y", parsed))

import math 
print(round(5.67))
print(math.ceil(45.20))
print(math.sqrt(64))
print(math.pow(2,4))

import random
print(random.random() *200)
print(random.randint(1,10))
print(random.randrange(1,10,2))
print(random.choice( ['red', 'black', 'green'] ))
myList = [2, 109, False, 10, "Lorem", 482, "Ipsum"]
print(random.choice(myList))




