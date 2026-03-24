# Formato de usb:

1. diskpart
2. list disk
3. select disk x
4. clean
5. create partition primary
6. active
7. select partition 1
8. format fs=fat32 quick
9. exit

# Formato para instalar OS en disco duro:

0. Shift + F10: open CMD.
1. diskpart
2. list disk
3. select disk x
4. clean
5. convert gpt
6. exit
