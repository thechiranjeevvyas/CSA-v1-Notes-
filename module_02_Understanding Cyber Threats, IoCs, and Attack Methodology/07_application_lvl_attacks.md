## ⚠️ 7. Application-Level Attacks

### 🛠️ 7.1. SQL Injection Attacks

SQL injection attacks use a series of malicious SQL queries or SQL statements to directly manipulate the database. These attacks occur when an application does not properly validate input before passing it to a SQL statement.

```sql
SELECT * FROM tablename WHERE UserID= 2302
```

can be altered by an attacker to:

```sql
SELECT * FROM tablename WHERE UserID= 2302 OR 1=1
```

#### 🧨 SQL Injection Can Allow Attackers To:

- Log into the application without valid credentials.
- Access or manipulate restricted data.
- Drop or modify databases.
- Use trusted app components to reach other databases.

---

### 🧪 7.2. Cross-site Scripting (XSS) Attacks

XSS attacks exploit dynamically generated web pages by injecting malicious client-side scripts into them.

#### 🧨 XSS Can Lead To:

- Execution of malicious scripts
- Session hijacking
- Data theft and manipulation
- Brute-force attacks, keylogging
- Intranet probing

#### 🧵 XSS Attack Scenario (Email Example):

```html
<a
  href="http://bank.com/registration.cgi?clientprofile=<SCRIPT>maliciouscode</SCRIPT>"
>
  Click here</a
>
```

The victim unknowingly executes the malicious script, compromising sensitive data.

---

### ⚙️ 7.3. Parameter Tampering

Involves manipulating parameters exchanged between server and client to alter data like prices, access rights, and credentials.

#### 🧪 Examples:

- **Query String Tampering**: Changing visible URL parameters.
- **HTTP Header Tampering**: Modifying headers like `Referer`.
- **Cookie Parameter Tampering**: Altering cookie data to escalate privileges.

---

### 📂 7.4. Directory Traversal

Also known as path traversal, this attack accesses unintended files/directories via unsanitized input.

#### 🧨 Impacts:

- Exposes file structures
- Accesses protected pages
- Leaks sensitive credentials
- Retrieves source code

#### 🌐 Example URL:

```
http://www.example.com/../.././../some_dir/some_file
```

---

### 🔁 7.5. Cross-site Request Forgery (CSRF) Attack

Also called XSRF, this attack forces a logged-in user to perform unintended actions. Severity depends on the user's role.

#### 🧪 Attack Flow:

1. Victim logs into a trusted site (e.g., bank).
2. Visits a malicious site.
3. Malicious site injects a request to the trusted site using the user's session.

This exploits the fact that the web application fully trusts the user post-authentication.

---

### 💥 7.6. Application-level DoS Attack

Targets app-layer availability by exploiting flaws like poor input validation or resource exhaustion.

#### 🧨 Examples:

- **User Registration DoS**: Submitting forms repeatedly.
- **User Enumeration**: Automating username discovery.
- **Login Flooding**: Spamming login attempts.
- **Account Lock Out**: Causing user account lockouts via invalid attempts.

---

### 🍪 7.7. Cookie Poisoning Attacks

This attack involves tampering with cookie contents to impersonate users or gain unauthorized access.

Cookies store session data. If manipulated, attackers can:

- Hijack sessions
- Bypass authentication
- Inject malicious content

---

### 🔒 7.8. Session Fixation

Here, the attacker sets a known session ID and tricks the user into using it. Once the victim logs in, the attacker hijacks the session using the fixed ID.

#### 🔐 Example Attack Flow:

1. Attacker creates a session ID.
2. Victim logs in using this ID.
3. Attacker now has access to the authenticated session.

---
