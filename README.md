
# Blackhat Patterns Repository

This repository contains a collection of JSON files used for security testing, vulnerability scanning, and pattern matching. These patterns can be used with tools like `gf` (Gf-Patterns) for fast and accurate reconnaissance and exploitation.
```markdown
## 📂 **File Structure**
| File Name | Description |
|-----------|-------------|
| `api-keys.json` | Patterns for identifying API keys. |
| `asymmetric-keys_secrets.json` | Patterns for asymmetric key secrets. |
| `auth.json` | Authentication-related patterns. |
| `aws-keys.json` | AWS key patterns. |
| `aws-mws-key.json` | AWS Marketplace Web Service key patterns. |
| `badwords.json` | List of banned or sensitive words. |
| `base64.json` | Base64-encoded strings and patterns. |
| `bufferoverflow.json` | Patterns related to buffer overflow vulnerabilities. |
| `cdn.json` | Patterns related to CDN (Content Delivery Network). |
| `cors.json` | CORS-related patterns. |
| `crypto.json` | Cryptography-related patterns. |
| `debug-pages.json` | Debugging page patterns. |
| `debug_logic.json` | Debug logic-related patterns. |
| `domxss.json` | Patterns for detecting DOM-based XSS vulnerabilities. |
| `endpoints.json` | API endpoint patterns. |
| `environment-configuration.json` | Environment configuration file patterns. |
| `execs.json` | Patterns for identifying executable files. |
| `framework.json` | Patterns related to specific frameworks. |
| `github.json` | GitHub-related patterns. |
| `google-keys_secrets.json` | Google service key patterns. |
| `idor.json` | Patterns for Insecure Direct Object References (IDOR). |
| `interestingparams.json` | Interesting URL or API parameters. |
| `ip.json` | Patterns related to IP addresses. |
| `jsfiles.json` | JavaScript file patterns. |
| `jwt.json` | JSON Web Token (JWT) patterns. |
| `lfi.json` | Local File Inclusion (LFI) vulnerability patterns. |
| `php-callbacks.json` | PHP callback function patterns. |
| `php-codeexec.json` | PHP code execution patterns. |
| `php-errors.json` | PHP error message patterns. |
| `php-informationdisclosure.json` | PHP information disclosure patterns. |
| `php-sinks.json` | PHP sink function patterns. |
| `php-sources.json` | PHP source function patterns. |
| `rce.json` | Remote Code Execution (RCE) patterns. |
| `redirect.json` | URL redirection patterns. |
| `s3-buckets.json` | Amazon S3 bucket patterns. |
| `sqli.json` | SQL Injection patterns. |
| `ssrf.json` | Server-Side Request Forgery (SSRF) patterns. |
| `ssti.json` | Server-Side Template Injection (SSTI) patterns. |
| `takeovers.json` | Subdomain takeover patterns. |
| `truffle.json` | TruffleHog-related patterns. |
| `urls.json` | Common URL patterns. |
| `version-files.json` | Versioning and cache-busting file patterns. |
| `WebSocket.json` | WebSocket call patterns. |
| `xpath.json` | XPath injection patterns. |
| `xss.json` | Cross-Site Scripting (XSS) patterns. |
| `xxe.json` | XML External Entity (XXE) patterns. |

---

## 🛠️ **How to Install and Use with `gf`**
Follow these steps to add these patterns to `gf`:

### ✅ **1. Clone the repository**  
```sh
git clone https://github.com/NightfallSecDev/blackhat-patterns.git
```

### ✅ **2. Create the `.gf` directory (if it doesn't exist):**  
```sh
mkdir ~/.gf
```

### ✅ **3. Copy the patterns to the `.gf` directory:**  
```sh
cp blackhat-patterns/*.json ~/.gf/
```

### ✅ **4. Test the Patterns in `gf`:**  
You can now use the patterns with `gf`. For example:

- To use the `xss` pattern:
```sh
gf xss target.txt
```

- To list all available patterns:
```sh
gf -list
```

### ✅ **5. Example Output:**  
```sh
cat target.txt | gf xss
```
This will filter out any possible XSS vulnerabilities from `target.txt`.


## 🚀 **Contributing**
- If you want to add more patterns or improve existing ones, feel free to submit a pull request.
- Ensure that new patterns are tested before submitting.



## 📄 **License**
This repository is open-source under the [MIT License](LICENSE).



**Happy Hacking! 🐱‍💻**
