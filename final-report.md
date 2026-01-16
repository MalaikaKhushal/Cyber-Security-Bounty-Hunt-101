# Final Vulnerability Report

## Vulnerability Name
Reflected Cross-Site Scripting (XSS)

## Target Environment
PortSwigger Web Security Academy (Lab Environment)

## Description
A reflected cross-site scripting vulnerability was identified
where user-supplied input was reflected back in the response
without proper validation.

## Steps to Reproduce
1. Open the vulnerable lab page.
2. Locate the search or input field.
3. Enter the following payload:
   <script>alert(1)</script>
4. Submit the input.
5. An alert popup appears on the screen.

## Proof of Concept (PoC)
Payload Used:
<script>alert(1)</script>

## Impact
This vulnerability allows execution of arbitrary JavaScript
in the victim’s browser and may lead to session hijacking
or phishing attacks.

## Conclusion
The vulnerability was successfully identified and documented
as part of a beginner bug bounty project.

