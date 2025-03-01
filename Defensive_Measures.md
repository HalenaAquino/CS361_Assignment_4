Vulnerability: SQL Injection

Countermeasures and how it'll mitigate risk: 
- Use parameterized queries and input validation: prevents direct SQL injection
- Filter database inputs: blocks malicious characters
- Restrict database code: limits SQL execution to safe queries
- Restrict database access: reduces the impact of an attack
- Maintain applications and databases: fixes known vulnerabilities before exploitation 
- Monitor application and database inputs and communications: detects SQL injection attempts in real time

---

Vulnerability: Cross-Site Scripting (XSS)

Countermeasures and how it'll mitigate risk: 
- Filter input on arrival: blocks SQL injections, XSS and command injection before it reaches the system
- Encode data on output: prevents XSS by ensuring that user input is treated as text, not as code
- Use appropriate response headers: stops Clickjacking, XSS, and MITM attacks using security headers
- Content Security Policy: blocks execution of unauthorized scripts (even if injected)

---

Vulnerability: Broken Authentication

Countermeasures and how it'll mitigate risk: 
- Control Session Length: prevents long session abuse (sessopn hijacking)
- Rotate and Invalidate Session IDs: stops session fixation and reuse of stolen sessions
- Multi-factor Authentication: blocks unauthorized access even if passwords are stolen
- Implement Brute-Force Protection: prevents automated login guessing attacks
- Avoid Showing Session IDs in URLs: protects session tokens from exposure in logs and referrers
- Create Strong Password Policies: reduces the risk of password cracking and credential surfing

---

Vulnerability: Directory Traversal

Countermeasures and how it'll mitigate risk: 
- Input validation: blocks ../, special characters, and unapproved file names
- Use of allow lists: ensures only safe files can be accessed
- Avoid using user input for file operations: prevents attackers from controlling file paths
- Use of built-in functions to normalize paths: stops traversal attempts by keeping paths within allowed directories
- Least privilege principle: limits access, reducing the impact of successful attacks
- Regular security testing: detects vulnerabilities before attackers can exploit them

---

Vulnerability: Insecure Direct Object References (IDOR)

Countermeasures and how it'll mitigate risk: 
- Implement authorization checks: ensures users can only access objects they own
- Use indirect references: prevents attackers from guessing sequential ID
- Access control mechanisms: limits access based on roles and permissions
- Validate and sanitize input: blocks malicious modifications of object references
- Secure API Design: ensures API does not expose sensitive object details
- Monitor and log access: detects unauthorized access attempts in real time
- Conduct regular security audits and penetration testing: finds and fixes IDOR vulnerabilities before attackers can exploit them
