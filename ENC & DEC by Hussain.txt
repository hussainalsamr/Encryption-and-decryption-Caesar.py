import string
arr=string.ascii_letters
pl=input("please enter Encryption message :")
key=input('please enter key 0 into 9 :')
iq=""

for item in pl:
    if item.isalpha():
        iq+=arr[(arr.index(item)+int(key))%26]
    else :
       iq+=item
print(iq)
pli=input("please enter Decryption message :")
key=input('please enter key 0 into 9 :')
iqe=""
for item in pli:
    if item.isalpha():
        iqe+=arr[(arr.index(item)-int(key))%26]
    else :
       iqe+=item
print(iqe)
