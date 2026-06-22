# iOS App Store Compliance Checklist

> Created by [TrustGrid Technology Limited](https://trustgridhq.com) — App Security & Compliance Consulting.
> Use this checklist before submitting your app to the Apple App Store.

---

## 1. App Privacy Label (Required)

- [ ] Privacy Nutrition Label completed accurately in App Store Connect
- [ ] All data types collected are declared (including third-party SDK data)
- [ ] Data linked to identity correctly identified
- [ ] Data used for tracking declared and ATT prompt implemented
- [ ] Privacy policy URL added to App Store listing
- [ ] Privacy policy is publicly accessible (not behind login)
- [ ] Privacy policy covers all data types declared in the label

---

## 2. App Tracking Transparency (ATT)

- [ ] ATT permission prompt implemented before any tracking begins
- [ ] ATT usage description is clear and honest
- [ ] App functions properly if user denies tracking permission
- [ ] No tracking occurs before ATT permission is granted

---

## 3. Data Collection & Handling

- [ ] App only requests permissions it actually needs
- [ ] Each permission has a clear, honest usage description
- [ ] App functions with minimum permissions if user denies optional ones
- [ ] No sensitive data stored in plain text on device
- [ ] No sensitive data logged to console in production build
- [ ] Data transmitted over HTTPS only (no HTTP)
- [ ] Certificate pinning implemented for sensitive API calls
- [ ] No hardcoded credentials, API keys, or secrets in codebase

---

## 4. Authentication & Account Management

- [ ] Secure authentication implemented (OAuth 2.0 / OIDC recommended)
- [ ] Password requirements meet minimum security standards
- [ ] Account deletion option available in-app (Apple requirement since 2022)
- [ ] Account deletion actually deletes user data (not just deactivates)
- [ ] Sign in with Apple implemented if any third-party login is offered
- [ ] Biometric authentication implemented securely if used

---

## 5. KYC/AML Requirements (Fintech/Lending Apps)

- [ ] Identity verification flow is functional end-to-end
- [ ] KYC document upload and storage is secure
- [ ] Document verification results are handled correctly
- [ ] Failed verification flows are handled gracefully
- [ ] AML screening integrated where required
- [ ] Regulatory compliance statements included where required
- [ ] Age verification implemented if required by jurisdiction

---

## 6. In-App Purchases & Payments

- [ ] All paid features use Apple's in-app purchase system (where required)
- [ ] Subscription terms clearly disclosed before purchase
- [ ] Refund policy accessible from within the app
- [ ] Payment processor integration is PCI DSS compliant
- [ ] No external payment links that bypass Apple IAP (where prohibited)

---

## 7. Content & Legal

- [ ] App does not contain prohibited content (Apple Review Guidelines Section 1)
- [ ] Intellectual property rights cleared for all content used
- [ ] No misleading descriptions in App Store listing
- [ ] Age rating selected accurately reflects app content
- [ ] Terms of Service accessible from within the app
- [ ] Support URL is active and responsive

---

## 8. Technical Requirements

- [ ] App built with current minimum iOS SDK target
- [ ] No use of private or undocumented Apple APIs
- [ ] App tested on multiple device sizes and iOS versions
- [ ] App does not crash on launch on any supported device
- [ ] All external URLs in the app are active and correct
- [ ] Push notification permissions requested appropriately

---

## 9. Privacy Manifest (Required from May 2024)

- [ ] Privacy manifest file (PrivacyInfo.xcprivacy) included
- [ ] All required reason APIs declared in privacy manifest
- [ ] Third-party SDK privacy manifests included
- [ ] Privacy manifest accurately reflects app's data practices

---

## 10. Pre-Submission Final Check

- [ ] App tested thoroughly on physical device (not just simulator)
- [ ] All placeholder content removed
- [ ] All test accounts and debug features removed from production build
- [ ] App Store screenshots are accurate and up to date
- [ ] App description matches actual app functionality
- [ ] Keywords do not include competitor names or prohibited terms
- [ ] Support email is monitored and responsive

---

## Risk Summary

After completing this checklist, classify your submission readiness:

| Status | Description |
|--------|-------------|
| ✅ Ready | All items checked — proceed to submission |
| ⚠️ At Risk | 1-3 items unchecked — address before submitting |
| ❌ Not Ready | 4+ items unchecked — significant rejection risk |

---

*Created by [TrustGrid Technology Limited](https://trustgridhq.com). For a full App Store compliance audit, visit our [Fiverr service page](https://www.fiverr.com/s/WE5jVGR).*
