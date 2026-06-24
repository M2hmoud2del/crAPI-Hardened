# crAPI-Hardened Roadmap

This roadmap outlines the planned progression for hardening the crAPI application. The goal is to incrementally secure the API while documenting each vulnerability and its remediation.

## Phase 1: Foundation and Authentication
- [x] Establish community hardening repository structure.
- [x] Implement Vulnerability Reporting Program and Hall of Fame.
- [ ] Address critical Authentication vulnerabilities.
- [ ] Remediate NoSQL injection in authentication flows.
- [ ] Implement secure password reset logic.

## Phase 2: Authorization and Data Exposure
- [ ] Remediate Broken Object Level Authorization (BOLA) in vehicle data.
- [ ] Remediate Broken Function Level Authorization (BFLA) in administrative endpoints.
- [ ] Secure endpoints against Mass Assignment.
- [ ] Implement proper data filtering to prevent excessive data exposure.

## Phase 3: Business Logic and Infrastructure
- [ ] Fix race conditions and rate limiting issues (e.g., in coupon or order processing).
- [ ] Secure the application against Server-Side Request Forgery (SSRF).
- [ ] Harden the underlying container and Vagrant configurations.

## Phase 4: Monitoring and Advanced Security
- [ ] Introduce secure logging practices.
- [ ] Implement API gateway security controls.
- [ ] Final security audit and community review.

*Note: This roadmap is subject to change based on community contributions and discovered vulnerabilities.*
