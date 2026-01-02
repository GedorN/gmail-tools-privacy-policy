# Security Policy - Gmail Tools

## 1. Overview

The Gmail Helper extension has been developed with security and privacy as fundamental priorities. This document describes the security practices, data protection policies, and measures implemented to protect users.

## 2. Privacy and Data Protection

### 2.1 Data Collected

The Gmail Helper extension collects only the data **necessary** for its operation:

- **Authentication Information**: OAuth access token for Gmail (stored locally on the device)
- **Configuration Data**: User preferences and settings
- **Language Information**: User location and language preferences

### 2.2 Data Not Collected

The extension **DOES NOT**:
- Collect personally identifiable information beyond what is necessary
- Share data with third parties without consent
- Store email history on servers
- Perform user tracking
- Collect browsing information

## 3. Data Storage

### 3.1 Local Storage
- All sensitive data is stored **locally** on the user's device
- Access tokens are securely stored using the browser's native storage APIs
- Data is encrypted when possible

### 3.2 Servers
- The extension does not maintain a user database
- No personal data is synchronized with external servers
- Connections to third-party APIs (when they exist) use HTTPS

## 4. Requested Permissions

The extension requests the following browser permissions:

| Permission | Justification |
|-----------|---------------|
| `mailto:` | Gmail integration for reading and composing emails |
| `storage` | Storage of user configurations and preferences |
| `activeTab` | Detection of active Gmail tabs |
| `scripting` | Script injection for additional functionality in the Gmail interface |
| `identity` | OAuth authentication with Google for secure Gmail access |

## 5. Authentication Security

### 5.1 OAuth 2.0
- We use Google's official OAuth 2.0 flow
- Passwords are never requested or stored by the extension
- Tokens are securely stored and can be revoked at any time

### 5.2 Permission Revocation
- Users can revoke permissions at any time in the browser settings
- Access revocation is immediate and secure

## 6. Secure Communication

- All communications with external APIs use **HTTPS** (TLS 1.2 or higher)
- SSL/TLS certificates are validated
- Content Security Policy (CSP) is implemented for protection against XSS

## 7. Secure Development Practices

### 7.1 Code
- Source code is kept private until release
- Code review is mandatory before merge
- Security testing is performed regularly

### 7.2 Updates
- Security updates are released promptly
- Critical vulnerabilities are handled with maximum priority
- Detailed changelog in each version

### 7.3 Dependencies
- Dependencies are kept up to date
- Audit is regularly performed for known vulnerabilities

## 8. Compliance and Regulations

The extension complies with:

- **General Data Protection Law (LGPD)** - Brazilian regulation
- **General Data Protection Regulation (GDPR)** - European regulation
- **Chrome Web Store Policies** - Security and privacy requirements

## 9. What We Do With Your Data

### Permitted Use
- Process user requests
- Improve extension functionality
- Problem diagnosis

### NOT Permitted Use
- Sell data to third parties
- Use data for marketing
- Share with advertisers
- Share with governments without legal order

## 10. Data Retention

- Configuration data is maintained while the extension is installed
- Data is automatically deleted when the extension is uninstalled
- Users can request manual deletion at any time

## 11. Third-Party Security

### Google APIs
- The extension uses Google's official APIs
- Google is responsible for the security of its services
- See [Google's Privacy Policy](https://policies.google.com/privacy) for more information

## 12. Reporting Security Vulnerabilities

If you discover a security vulnerability:

1. **DO NOT** disclose publicly
2. Contact us through the support email
3. Provide technical details and steps to reproduce
4. Wait for confirmation before any public disclosure

## 13. Updates to This Policy

This security policy may be updated periodically. We recommend reviewing it regularly to stay informed about current security practices.

**Last Updated**: January 2026

## 14. Contact

For questions about security, privacy, or this policy:

- 📧 Email: [gedor.silvaneto@gmail.com]
<!-- - 🐛 Security Issues: [link-to-report] -->
<!-- - 💬 Support: [support-channel] -->

---

**Thank you for using Gmail Helper. Your security and privacy are our priority.**
