# 🧩 Autonomy Engine – Compliance & Security Roadmap

> A living checklist for building AE’s security, privacy, and compliance posture.
> Update quarterly or after any major architectural change.

---

## 📘 Phase 0 – Foundation (Month 0 → 1)

- [ ] Create `/docs/compliance/README.md` as master index.
- [ ] Write **Access Control Policy** (1 page).
- [ ] Write **Data Retention & Redaction Policy** (1 page).
- [ ] Write **Incident Response Plan** (1 page).
- [ ] Write **Vendor / Sub-processor Register** (table of APIs, PHI status, BAA status).
- [ ] Enforce **2FA** on all services (GitHub, npm, cloud console).
- [ ] Enable **branch protection** on `main`.
- [ ] Add **npm audit + Dependabot** to CI pipeline.
- [ ] Confirm **secrets are encrypted** (no `.env` in repo).
- [ ] Verify **TLS 1.2+** enforced on all endpoints.

---

## 🧠 Phase 1 – Proof-of-Concept Compliance (Month 1 → 3)

- [ ] Restrict all data in dev/prod to **de-identified or synthetic** PHI.
- [ ] Implement **IAEL export** (JSON hash-chained logs).
- [ ] Write & attach **One-Page Security & Compliance Summary** (PDF/Markdown).
- [ ] Maintain **Risk Log** (`risk | likelihood | mitigation | owner`).
- [ ] Enable **cost / governance approvals** for all paid API calls.
- [ ] Run **quarterly vulnerability review** (npm audit + manual).
- [ ] Store policy docs in private repo folder with version history.

---

## 🧱 Phase 2 – BAA-Ready Stack (Month 3 → 6)

- [ ] Choose HIPAA-eligible cloud region (AWS HealthLake / Azure Health / GCP Healthcare).
- [ ] Draft **base BAA template** (lawyer review later).
- [ ] Sign BAAs with:
  - [ ] Cloud provider  
  - [ ] Notion Enterprise (BAA tier)  
  - [ ] Analytics provider (Power BI Premium / Tableau Cloud)  
- [ ] Verify **disk encryption** + **KMS key management** active.
- [ ] Contract **external security reviewer** for quick audit.
- [ ] Document **data-flow diagram** (where PHI / metadata / audit logs live).

---

## 🧭 Phase 3 – Mature Posture (Month 6 → 12)

- [ ] Separate **Ops / Dev** roles + service accounts.
- [ ] Run **external penetration test**.
- [ ] Add **SOC 2 / ISO 27001** alignment note (“in progress” ok).
- [ ] Obtain **business liability / cyber insurance**.
- [ ] Hire or contract **legal counsel** for HIPAA / BAA negotiations.
- [ ] Update marketing / docs with **security overview** section.

---

## 🔁 Phase 4 – Ongoing Maintenance

- [ ] **Rotate API keys** quarterly; update in Secrets Manager.
- [ ] **Review & re-sign BAAs** annually.
- [ ] **Review policies** quarterly.
- [ ] **Verify audit log integrity** monthly.
- [ ] **Backup & restore test** quarterly.
- [ ] **Review vendor list** yearly.
- [ ] **Refresh staff training / self-review** yearly.

---

## ✅ Quick Status Summary

| Area | Status | Notes |
|------|--------|-------|
| Governance & Policies | ☐ |  |
| Identity & Access | ☐ |  |
| Data Security | ☐ |  |
| Vendor BAAs | ☐ |  |
| Audit & Logging | ☐ |  |
| External Review | ☐ |  |

---

> **Reminder:**  
> “Compliance” is a living habit, not a finish line.  
> Keep the stack documented, automate checks where possible, and re-evaluate risks after every new integration.
