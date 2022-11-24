# CSRF
# What is CSRF? 
CSRF stands for Cross Site Request Foregery. Also known as XSRF. IT is an attack vector that tricks a web browser into executing an unwanted action in an application to which a user is logged in. CSRFs are typically conducted using malicious social engineering, such as an email or link that tricks the victim into sending a forged request to a server. As the unsuspecting user is authenticated by their application at the time of the attack, it’s impossible to distinguish a legitimate request from a forged one.  
![form-handling-with-anti-csrf-protection](https://user-images.githubusercontent.com/115407638/203840620-18971121-a48d-4260-8c17-62a76e2abe54.png)

# BUG
Takes user to a forged/faked generated URL. 

# Steps to perform CSRF 
1) URL is being created from the desired website to perform attack. 
2) Hyperlink of that URL is sent to the attacker who is logged in that website. 
3) The attacker clicks to the link and the request is sent. 
4) Website fulfills the request and the authetication is sent to the attacker.  

# Forged URL used 
1) http://magnus.jalatechnologies.com//Account/Login/acct=AttackerA&password=$100  
2) http://magnus.jalatechnologies.com/Account/AdminLogin/acct=AttackerA&password=$100 


