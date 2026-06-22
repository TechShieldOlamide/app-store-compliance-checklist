# KYC/AML App Readiness Checklist

> Created by [TrustGrid Technology Limited](https://trustgridhq.com) — App Security & Compliance Consulting.
> Use this checklist before launching a fintech, digital lending, or payment app.

---

## 1. KYC Identity Verification

- [ ] Identity document upload flow is functional end-to-end
- [ ] Accepted document types clearly communicated to user
- [ ] Document image quality validation implemented
- [ ] Liveness detection implemented for selfie verification
- [ ] Face match between selfie and ID document performed
- [ ] BVN verification integrated (Nigeria)
- [ ] NIN verification integrated where required
- [ ] Failed verification flow handled gracefully with clear user messaging
- [ ] Manual review process defined for edge cases
- [ ] KYC status tracked and visible in admin dashboard

---

## 2. KYC Data Handling

- [ ] Identity documents stored encrypted at rest
- [ ] Access to KYC documents restricted to authorised staff only
- [ ] Audit trail maintained for all KYC document access
- [ ] Document fetch API functional and tested end-to-end
- [ ] KYC documents retrievable from admin dashboard
- [ ] Document retention period defined and enforced
- [ ] Secure deletion process for documents after retention period

---

## 3. Customer Due Diligence (CDD)

- [ ] Standard CDD process documented and implemented
- [ ] Enhanced Due Diligence (EDD) process defined for high-risk customers
- [ ] PEP (Politically Exposed Person) screening integrated
- [ ] Sanctions list screening integrated (UN, OFAC, local lists)
- [ ] Customer risk scoring implemented
- [ ] High-risk customer escalation process defined
- [ ] Periodic review schedule defined for existing customers

---

## 4. AML Transaction Monitoring

- [ ] Transaction monitoring system integrated
- [ ] Threshold alerts configured for large transactions
- [ ] Structuring detection implemented (multiple transactions below threshold)
- [ ] Unusual pattern detection configured
- [ ] High-risk geography flags implemented
- [ ] Alert review workflow defined and staffed
- [ ] False positive management process in place

---

## 5. Suspicious Activity Reporting

- [ ] Internal SAR form and process defined
- [ ] MLRO (Money Laundering Reporting Officer) designated
- [ ] External STR filing process to NFIU documented
- [ ] Tipping-off prevention controls in place
- [ ] SAR records retention policy defined (minimum 7 years)
- [ ] Staff trained on suspicious activity identification and reporting

---

## 6. Regulatory Compliance

- [ ] CBN licence or exemption confirmed before launch
- [ ] NDPC registration completed (Nigeria)
- [ ] Applicable CBN circulars reviewed and implemented
- [ ] KYC tier limits configured per CBN guidelines
  - [ ] Tier 1: No BVN, max balance NGN 50,000, daily transaction NGN 50,000
  - [ ] Tier 2: BVN + basic KYC, max balance NGN 300,000
  - [ ] Tier 3: Full KYC, higher limits
- [ ] Currency Transaction Report (CTR) process for transactions above NGN 5M
- [ ] Legal counsel reviewed compliance posture before launch

---

## 7. Staff Training & Governance

- [ ] All customer-facing staff trained on KYC procedures
- [ ] All staff trained on AML red flags and reporting obligations
- [ ] Training records maintained
- [ ] Compliance Officer designated
- [ ] AML/KYC policy approved by senior management
- [ ] Annual policy review scheduled

---

## 8. Third-Party KYC Providers

- [ ] KYC provider due diligence completed
- [ ] Data Processing Agreement (DPA) signed with KYC provider
- [ ] Provider's data handling practices reviewed
- [ ] Fallback process defined if provider is unavailable
- [ ] Provider integration tested end-to-end including failure scenarios

---

## 9. App Store Specific (KYC Apps)

- [ ] Data Safety / Privacy Label accurately reflects KYC data collection
- [ ] Biometric data handling disclosed in privacy label
- [ ] Government ID handling disclosed in privacy label
- [ ] Financial information handling disclosed in privacy label
- [ ] Purpose of data collection clearly explained in privacy policy

---

## 10. Pre-Launch Final Check

- [ ] KYC flow tested with real documents (not test data only)
- [ ] Admin dashboard KYC review functionality tested
- [ ] Rejection and retry flows tested
- [ ] Data storage and retrieval tested end-to-end
- [ ] Regulatory review completed or legal sign-off obtained
- [ ] Incident response plan updated to cover KYC data breach scenarios

---

## Readiness Summary

| Area | Status | Notes |
|------|--------|-------|
| KYC Identity Verification | | |
| KYC Data Handling | | |
| Customer Due Diligence | | |
| AML Transaction Monitoring | | |
| Suspicious Activity Reporting | | |
| Regulatory Compliance | | |
| Staff Training | | |

---

*Created by [TrustGrid Technology Limited](https://trustgridhq.com). For KYC/AML compliance setup and audit, visit our [Fiverr service page](https://www.fiverr.com/s/m54N7ZV).*
