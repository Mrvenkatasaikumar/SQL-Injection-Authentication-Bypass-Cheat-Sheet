# SQL Injection – Authentication Bypass

## 1. Introduction

SQL Injection (SQLi) is a web application vulnerability that occurs when user input is improperly included in SQL queries. An attacker may manipulate the query to access unauthorized data or bypass login authentication.

Authentication bypass through SQL Injection occurs when a vulnerable login page accepts manipulated input and incorrectly authenticates a user without valid credentials.

## 2. Objective

- Understand SQL Injection.
- Learn how authentication bypass occurs.
- Identify vulnerable login forms.
- Practice testing in an authorized lab environment.
- Understand prevention techniques.

## 3. Authentication Bypass Test Payload

' OR '1'='1' -- 
Attempts to bypass login by making the SQL condition always true
## 4. Impact

- Unauthorized access to user accounts.
- Exposure of sensitive database information.
- Unauthorized access to application features.
- Potential data modification or deletion, depending on database permissions and query design.

## 5. Prevention and Mitigation

1. **Use parameterized queries:** Keep SQL commands separate from user-supplied values.
2. **Use prepared statements:** Prevent input from being interpreted as SQL syntax.
3. **Avoid dynamic SQL:** Do not concatenate untrusted input into queries.
4. **Use least-privilege database accounts:** Limit the application's database permissions.
5. **Apply secure error handling:** Do not expose database errors to users.
6. **Perform security testing:** Regularly assess applications in authorized environments.

## 6. Disclaimer

This documentation is for educational purposes and authorized security testing only. Do not attempt authentication bypass on systems without permission.
