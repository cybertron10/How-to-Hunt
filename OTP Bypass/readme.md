* Response Tampering:
```
Capture the correct otp response and replace that response with wrong otp response.

Sensitive data in response (Visible of otp in response,Password reset token in response)

```
* Default OTP like 0000,1234 etc

* Direct page request:(Forced Browsing)

* BruteForce:
```
No RateLimit

No RateLimit while generating otp Can create python script which will generate and send otp which allows bruteforcing. 

```
* Using other account valid token or otp:


* OTP Bypass using IP Rotate plugin:


* Bypass OTP using HTTP Headers while bruteforing:


* Using Burp FakeIP Plugin


* Password reset poisoning:
```
Host: target.com

X-Forwarded-Host: evil.com


Host: evil.com

X-Forwarded-Host: target.com
```

* Oauth redirection to token leakage:


* Weird Bypass:
```
Remove the country code +91 to [ ] Modify the number from +91 xxxxx-xxxxx to [] xxxxx-xxxxx
```

* Rate Limit Bypass:
```
&user%5Bemail%5D=email@here.com%00 - and keep adding %00 everytime you are rate limited. After a while you can go back to just %00 as it resets after so long.

we can use %0d%0a and achieve same results by increasing %0d%0a when we hit "Too many requests".

we can still use %09 over and over again to bypass the rate limit. Using %09 will still target the same email. %09 is a blank space.

```

* Race Condition OTP Bypass:
```
If otp is 6 digits use turbo intruder default script to bruteforce.

```

* Bypassing 2-Factor auth by Reset Password Functionality


* Bypassing 2fa Via OAuth mechanism
```

For this bypass to work the attacker must have access to the OAuth integration account to log in on behalf of the user

Mostly it will not be accepted. There are rare cases some companies may accept it.
```

* Bypassing 2fa via CSRF attack on disable 2FA:

* Bypassing 2fa using backup code request & response:

* Removing the OTP field, sometimes the OTP can be bypassed
```
In PHP, your otp is 123456 you can try replacing parameters with otp[]=12356. Another example if the backend accepts JSON: {"userid": "x123", "otp":"123456"}then we change it to {"userid": "x123", "otp":[]}

BruteForcingOTP

Otp is checked at client side and returned in response
```

# Reference

https://blog.compactbyte.com/2019/11/30/aneka-bug-bypass-otp-one-time-password/

https://link.medium.com/FIRrM4Jl05 https://link.medium.com/tKqQY1Ml05 https://link.medium.com/ne4pwoOl05 https://link.medium.com/hhdBnCPl05 https://link.medium.com/YFLGk4Ql05 https://link.medium.com/rml43ESl05 https://link.medium.com/ds1k5XTl05 https://link.medium.com/35IjaPVl05 https://link.medium.com/4l50R4Xl05
