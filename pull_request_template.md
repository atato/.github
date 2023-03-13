Fixes issue https://atato.atlassian.net/browse/PR-
- [ ] Has tests
- [ ] Code is easily readable
- [ ] Rapid Risk Assessment(RRA) Approval Required 

---

RRA
- [x] Are you changing the attack surface?
    - Api, Entry points, endpoints. Anything with an open port, input field, receiving data
- [x] Are you changing the tech stack?
    - Upgrade node, new js framework? New tool?
- [x] Are you changing the application security controls?
    - Password logic, authentication, authorisation, accounting, audit trail, logging
- [x] Are you adding confidential/sensitive data?
    - Personally Identifiable Information (PII) or Sensitive Personal Data (sDP)
- [x] Are you modifying high-risk code?
    - Password hashing, cryptography libraries, anything dealing with security
    - Anything listed in CODEOWNERS files in any repository

If any of the 5 questions remain checked, you must get specific approval of the RRA before the PR can be approved. To avoid delays, comment the full detail of the YES in the PR (i.e. if you answer YES to (1) then specify what port is being opened, and why it has to be open, and what security measures you have already taken if any)
