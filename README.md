# Overview
As a penetration tester, I assessed the client-side security of a web application with a focus on JavaScript behavior and third-party library integration. During testing, I identified a client-side prototype pollution vulnerability that could be exploited through a gadget in a third-party library. By polluting the global object prototype via a URL fragment, I was able to trigger a DOM-based XSS sink and execute arbitrary JavaScript in the victim’s browser. This project demonstrates how unsafe object handling and vulnerable library gadgets can be chained to achieve high-impact client-side exploitation.

# Steps Undertaken

Step 1: Analyzed client-side JavaScript execution paths using Burp Suite’s DOM Invader.

Step 2: Identified a prototype pollution source in user-controlled input and traced it to a gadget in a third-party library.

Step 3: Confirmed execution by reaching a DOM XSS sink and triggering JavaScript payloads.

Step 4: Delivered a malicious URL to demonstrate real-world exploitation without additional user interaction.

# Conclusion

This assessment confirmed a high-severity client-side vulnerability where prototype pollution could be abused to achieve DOM-based XSS. The findings highlight the risks of unvalidated client-side input and implicit trust in third-party JavaScript libraries, emphasizing the need for strict input handling and proactive dependency security.
