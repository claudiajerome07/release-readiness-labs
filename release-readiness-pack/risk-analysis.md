# Risk Analysis

| Risk | Severity | Likelihood | Mitigation | Owner |
|------|----------|------------|------------|-------|
| Hardcoded secrets | High | High | Move secrets to Kubernetes Secrets or Secret Manager | DevOps Team |
| Mutable image tag | Medium | Medium | Use immutable version tags | Release Engineer |
| Rollback script incomplete | High | High | Implement and validate rollback | DevOps Team |
| Pending approvals | High | High | Obtain formal approval before deployment | Release Manager |
| Dependency version not pinned | Medium | Medium | Pin dependency versions | Development Team |

---

## Overall Risk Assessment

Current release risk is **HIGH** because:

- Sensitive credentials are committed.
- Rollback is not fully implemented.
- Required approvals are missing.
- Deployment image is not pinned.

---

## Recommendation

The release should not proceed until all High severity risks are resolved.