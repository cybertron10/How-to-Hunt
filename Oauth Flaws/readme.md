
![Image of Yaktocat](https://camo.githubusercontent.com/4c062366ebe04d5161079ed0665c6a43fd2e32d3466cfd7bc2a49d016f2c69a8/68747470733a2f2f7062732e7477696d672e636f6d2f6d656469612f455a3157716d6358594141717753483f666f726d61743d6a7067266e616d653d39303078393030)



**Oauth token Leaks flaws**

1. Token leak through postMessage Vulnerability https://hackerone.com/reports/314814
2. Token steal by changing redirect_uri param https://hackerone.com/reports/665651
3. Token Steal usin IDN Homograph attack https://hackerone.com/reports/861940


**Oauth CSRF**
It can be Login CSRF or it also can be Oauth CSRF on account connect/link fucntion.
Login CSRF sometimes accepted by program. CSRF on oauth connect leads to account takeover.

Things need to check while hunting:
1. State Parameter is missing.
2. State Parameter is there but not validated at server side same as using another user's state parameter.
3. State Parameter is Predictable.

**Race Condition on Oauth**

1. https://pandaonair.com/2020/06/11/race-conditions-exploring-the-possibilities.html

**Oauth Cookie Injection to DoS**

https://hackerone.com/reports/1005421
