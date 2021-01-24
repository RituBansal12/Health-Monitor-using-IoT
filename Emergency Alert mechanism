import smtplib 
def email_alert(examp_str=""): 
server = smtplib.SMTP_SSL('smtp.gmail.com', port=465) 
print("Server Started...") 
server.login('test_email@gmail.com','pwd123') 
48
print("Server Login Successful") 
msg="""From:test_email@gmail.com\nTo:recipient_email@gmail.com\nSubject: Testing Email\n 
""" 
msg = msg+"Number = "+examp_str 
try: 
server.sendmail('test_email@gmail.com','recipient_email@gmail.com',msg) except: 
return server 
print("Sending Message...") 
server.quit() 
print("Quit Server") 
for ii in range(0,50): 
if ii==35: 
server=email_alert(str(ii)) 
else: 
continue
