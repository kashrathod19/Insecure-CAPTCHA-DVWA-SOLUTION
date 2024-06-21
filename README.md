# Insecure-CAPTCHA-DVWA-SOLUTION

Insecure CAPTCHA in DVWA Solution  This repository provides a solution to the Insecure CAPTCHA challenge in DVWA, featuring exploit scripts, detailed documentation, mitigation strategies, and test cases. It's designed for educational purposes to help understand and secure CAPTCHA implementations.

# What is Insecure CAPTCHA?

Insecure CAPTCHA refers to a CAPTCHA (Completely Automated Public Turing test to tell Computers and Humans Apart) implementation that is vulnerable to being bypassed or defeated by automated scripts or malicious users. CAPTCHAs prevent automated systems from performing actions meant for humans, such as submitting forms or creating accounts. However, if the CAPTCHA is not implemented securely, it can be easily circumvented, rendering it ineffective

![image](https://github.com/kashrathod19/Insecure-CAPTCHA-DVWA-SOLUTION/assets/54115061/2a5567ac-de89-430c-92bc-6d7a00cf99d2)

# Insecure CAPTCHA (LOW/MEDIUM)

```The Solution of low and medium level are same ```

Burp will be required for this challenges 

![image](https://github.com/kashrathod19/Insecure-CAPTCHA-DVWA-SOLUTION/assets/54115061/6567b0b6-2709-49ee-b083-1827bd1e5c7c)

Change the password and pass the CAPTCHA once the password is changed go to burp HTTP History and observe the two requests of ```POST``` of ```dvwa/vulnerabilities/captcha```Compare both the requests you can see there are changes in content length 

![image](https://github.com/kashrathod19/Insecure-CAPTCHA-DVWA-SOLUTION/assets/54115061/c5d9fc20-e74d-4b72-bf4b-59b51d9d5f7d)

We will be taking the below request in the repeater

![image](https://github.com/kashrathod19/Insecure-CAPTCHA-DVWA-SOLUTION/assets/54115061/08cdee6b-fd30-455c-9038-07158cd3570a)

Now change the password parameter and send the request check in the response whether the password is changed or not try to cross-check by logging off the ID and try login by using the password that you have used in the repeater

![image](https://github.com/kashrathod19/Insecure-CAPTCHA-DVWA-SOLUTION/assets/54115061/15438256-b92a-412e-a556-a3229da53dd5)

