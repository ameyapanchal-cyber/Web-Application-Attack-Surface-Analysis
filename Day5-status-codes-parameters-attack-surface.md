### Objective
- The objective of this writeup is to understand how websites behave at the HTTP level, how different status codes indicate server behavior, and how attackers analyze website structure, files, folders, and parameters to identify attack surfaces.

### HTTP Status Codes Observed
During this module, I studied the meaning and behavior of common HTTP status codes, including:
- 100 – Informational responses
- 200 / 201 – Successful request and resource creation
- 301 / 302 – Redirection behavior
- 304 – Cached response usage
- 400 – Bad request due to client-side error
- 401 / 403 – Authentication and authorization failures
- 404 / 405 – Resource not found or method not allowed
- 413 / 414 – Request size and URL length limitations
- 500 / 503 – Server-side errors and service unavailability

These status codes help attackers understand how the server processes requests and where restrictions or weaknesses may exist.

### Web Structure & Technologies
I learned how modern websites are structured and the technologies commonly used in web applications, including:
- Frontend technologies: HTML, CSS, JavaScript
- Frontend frameworks: React, Angular, Vue
- Backend technologies: PHP, Node.js, Django
- APIs: REST API, GraphQL
- Data formats: JSON, XML
- Supporting components: SQL databases, CDN, SSL/TLS

Understanding the tech stack helps attackers predict backend behavior and possible weaknesses.

### Important Files and Folders
I learned about commonly exposed or sensitive files and folders that attackers look for during enumeration, such as:
- .htaccess – Server configuration and access control
- robots.txt – Search engine crawl rules
- config.php – Configuration and credentials
- login.php – Authentication logic
- upload.php – File upload handling
- api.php – API endpoints
- backup/ – Backup files and directories
- privacy.html / terms.html – Informational pages revealing application structure

### Parameters Identified
I understood how parameters act as inputs to website functionality and how attackers focus on them instead of pages.
- URL parameters (GET)
- POST body parameters
- Hidden parameters
I also learned the flow used by attackers:
- Website → Page → Function → Parameter

### Observations
- Different website functions generate different parameters.
- Parameters control how data is retrieved, updated, or processed.
- Some parameters are visible, while others are hidden or inactive.
- Status codes reveal how the server reacts to valid and invalid inputs.
- Website behavior changes based on parameter presence and values.

### Why This Matters for Security
Attackers do not attack pages; they attack logic and parameters.
Understanding status codes, file structures, and parameters helps attackers:
- Identify authentication and authorization weaknesses
- Discover hidden functionality
- Predict backend logic behavior
- Prepare for advanced attacks like SQL injection, IDOR, and logic flaws

This highlights the importance of secure coding, proper validation, and layered defenses.

### Learning
- Before this module, I viewed websites as static pages.
Now, I understand that every website is a combination of functions, parameters, and server responses, which together form the attack surface for web application security testing.
- Status codes → behavior
- Tech stack → expected weaknesses
- Files & folders → entry points
