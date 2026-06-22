# Google Play Store Compliance Checklist

> Created by [TrustGrid Technology Limited](https://trustgridhq.com) — App Security & Compliance Consulting.
> Use this checklist before submitting your app to the Google Play Store.

---

## 1. Data Safety Form (Required)

- [ ] Data Safety section completed accurately in Play Console
- [ ] All data types collected declared including third-party SDK data
- [ ] Data sharing with third parties accurately disclosed
- [ ] Security practices section completed (encryption, deletion on request)
- [ ] Privacy policy URL added to Play Store listing
- [ ] Privacy policy is publicly accessible without login
- [ ] Privacy policy matches what is declared in Data Safety form

---

## 2. Permissions

- [ ] App only requests permissions actually needed for core functionality
- [ ] Each permission has a clear rationale
- [ ] Dangerous permissions justified and documented
- [ ] App functions correctly if user denies optional permissions
- [ ] No permissions requested at app launch without context
- [ ] Background location permission only requested if genuinely needed

---

## 3. Data Collection & Security

- [ ] All data transmitted over HTTPS only
- [ ] No sensitive data stored in plain text on device
- [ ] No sensitive data written to external storage without encryption
- [ ] No hardcoded credentials, API keys, or secrets in codebase
- [ ] No sensitive data logged in production build
- [ ] Certificate pinning implemented for sensitive API endpoints
- [ ] WebViews do not load arbitrary URLs or execute arbitrary JavaScript

---

## 4. Authentication & Account Management

- [ ] Secure authentication implemented
- [ ] Account deletion option available in-app (Google Play requirement)
- [ ] Account deletion removes user data from servers
- [ ] Password reset flow is functional
- [ ] Session tokens expire appropriately
- [ ] Biometric authentication implemented securely if used

---

## 5. KYC/AML Requirements (Fintech/Lending Apps)

- [ ] Identity verification flow functional end-to-end
- [ ] KYC document handling is secure
- [ ] Failed verification flows handled gracefully
- [ ] AML screening integrated where required by regulation
- [ ] Financial product terms clearly disclosed
- [ ] Cooling-off period implemented where required by law
- [ ] CBN/regulatory licence number displayed where required

---

## 6. Financial Features & Payments

- [ ] Payment processor integration is PCI DSS compliant
- [ ] In-app purchase items accurately described
- [ ] Subscription cancellation process is straightforward
- [ ] Refund policy clearly accessible
- [ ] Loan terms and APR clearly disclosed for lending apps
- [ ] No predatory lending practices that violate Play Store policies

---

## 7. Target API Level

- [ ] App targets current required Android API level
- [ ] App tested on minimum supported Android version
- [ ] 64-bit architecture supported
- [ ] App bundle (AAB) used instead of APK for new submissions

---

## 8. Content Policy

- [ ] App does not contain prohibited content per Google Play policies
- [ ] No misleading functionality or descriptions
- [ ] Age rating accurately reflects app content
- [ ] Content rating questionnaire completed accurately
- [ ] No deceptive design patterns (dark patterns)
- [ ] All intellectual property rights cleared

---

## 9. Ads & Monetisation

- [ ] Ads do not interfere with app functionality
- [ ] No ads shown to users identified as minors
- [ ] Interstitial ads appear at natural transition points only
- [ ] Ad network SDKs declared in Data Safety form

---

## 10. Pre-Submission Final Check

- [ ] App tested on multiple Android devices and versions
- [ ] All placeholder content removed
- [ ] All test/debug features removed from production build
- [ ] Store listing screenshots accurate and up to date
- [ ] Short and full descriptions accurate and keyword-appropriate
- [ ] Contact email monitored and responsive
- [ ] App signing configured correctly in Play Console

---

## Risk Summary

| Status | Description |
|--------|-------------|
| ✅ Ready | All items checked — proceed to submission |
| ⚠️ At Risk | 1-3 items unchecked — address before submitting |
| ❌ Not Ready | 4+ items unchecked — significant rejection risk |

---

*Created by [TrustGrid Technology Limited](https://trustgridhq.com). For a full Play Store compliance audit, visit our [Fiverr service page](https://www.fiverr.com/s/WE5jVGR).*
