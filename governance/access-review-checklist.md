# Access Review Checklist (IAM Governance)

## 1) Review Setup
- [ ] Define scope (system/app/group/role)
- [ ] Define review period (monthly/quarterly)
- [ ] Identify reviewer(s) (manager/app owner/security)
- [ ] Export current access list (users, groups, roles, privileged assignments)
- [ ] Confirm authoritative source (AD / Entra ID / app admin console)

## 2) Review Questions (Per User)
- [ ] Does the user still need access for their current role?
- [ ] Is access aligned to least privilege (no extra roles/groups)?
- [ ] Are there separation-of-duties conflicts?
- [ ] Is access granted via group/role (not direct assignment)?
- [ ] For privileged access: is it time-bound and justified?

## 3) Exceptions & Remediation
- [ ] Document exceptions with justification and owner approval
- [ ] Remove stale access (disabled users, leavers, role changes)
- [ ] Reduce over-privileged access (downgrade roles / remove groups)
- [ ] Confirm changes were applied and re-validate effective access

## 4) Evidence & Sign-Off
- [ ] Capture evidence (before/after screenshots, logs, exports)
- [ ] Record reviewer decision (approve / revoke / adjust)
- [ ] Add sign-off date + reviewer name
- [ ] Store evidence in audit-ready location (repo folder / ticket / GRC system)
