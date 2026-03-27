# 🔐 Website Security Analysis Project



## 📌 Objective

The objective of this project is to assess the security posture of a target website by identifying potential vulnerabilities, evaluating their risk levels, and recommending practical fixes. This project aims to provide actionable insights for improving website security and raising awareness about common web security threats.  



## 🛠 Tools Used

The following tools were used to perform the assessment:

- **Postman**  
  Used to test API endpoints, analyze response codes, and check for insecure responses.  

- **Browser Developer Tools (Network Tab)**  
  Used to inspect network requests, capture HTTP status codes, and identify potential issues such as redirects and missing headers.  


## 🔍 Methodology / Analysis Approach

The website security assessment was carried out in a step-by-step manner:

1. **Scope Definition**  
   Defined the parts of the website in scope, including publicly accessible pages, forms, and API endpoints.  

2. **Information Gathering**  
   Collected relevant information such as network responses, URLs, and HTTP headers for analysis.  

3. **Vulnerability Identification**  
   Analyzed collected data for potential security issues such as open redirects, missing security headers, and exposed sensitive information.  

4. **Risk Classification**  
   Each finding was assigned a risk level: Low / Medium / High / Critical, based on its potential impact.  

5. **Documentation**  
   Findings, screenshots, and tool outputs were documented in a structured report.  



## ⚠️ Identified Security Findings

The following issues were observed during the assessment:

- **Open Redirects**  
  Certain URLs can redirect users without proper validation, which may be exploited for phishing or malicious purposes.  

- **Exposed Sensitive Data**  
  Some API responses revealed sensitive information such as user IDs or internal tokens.  

- **HTTP Status Codes (302 Redirects)**  
  Unintended redirects were observed, requiring validation to ensure correct behavior.  

- **Missing Security Headers**  
  Headers like `Content-Security-Policy`, `X-Frame-Options`, and `Strict-Transport-Security` were missing, increasing exposure to common attacks.  

- **Improper Input Validation**  
  Some input fields were not properly sanitized, which could lead to injection attacks.  



## 🚨 Risk Classification

| Finding | Risk Level |
|---------|------------|
| Open Redirects | Medium |
| Exposed Sensitive Data | High |
| HTTP 302 Redirect | Low |
| Missing Security Headers | Medium |
| Improper Input Validation | High |

> Risk levels are based on potential impact on confidentiality, integrity, and availability.  



## 📊 Results / Outcome

The assessment confirmed that the target website has multiple security issues that require attention.  
- Some vulnerabilities could allow attackers to steal sensitive data or manipulate web traffic.  
- Missing security headers increase susceptibility to browser-based attacks.  
- Open redirects and input validation issues could be exploited for phishing or injection attacks.  

The findings provide actionable guidance to improve the website’s security posture.  



## 🛡 Recommendations & Best Practices

✅ Do’s:  

- Validate all redirects and URLs  
- Implement proper input validation and sanitization  
- Add missing security headers (`CSP`, `X-Frame-Options`, `HSTS`)  
- Use HTTPS and secure cookies  
- Regularly scan APIs and endpoints for vulnerabilities  

❌ Don’ts:

- Do not ignore low-risk issues—they can be chained for higher impact attacks  
- Do not expose sensitive data in API responses  
- Do not leave unvalidated input fields accessible to public users  



 📢 Conclusion

This project highlights the importance of **proactive website security assessments**. By identifying vulnerabilities, classifying risks, and implementing recommended fixes, website owners can significantly reduce the likelihood of cyberattacks and protect user data.  
