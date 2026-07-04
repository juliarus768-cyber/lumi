# Developer Playbook

## Related Documents

- [Backend and Cloud Architecture](../05_ENGINEERING/backend-and-cloud-architecture.md)
- [TypeScript Interfaces and JSON Schemas](../05_ENGINEERING/typescript-interfaces-and-json-schemas.md)
- [Testing and Quality Assurance Manual](../07_QA/testing-and-quality-assurance-manual.md)

## Migrated Content

## Math Adventure 17 – Developer Playbook

Version 1.0 Engineering Standards & AI Development Guide

## Purpose

This playbook defines how Math Adventure should be developed, reviewed, tested and released. It ensures human developers and AI coding assistants work consistently while protecting the educational vision of the product.

## 1. Engineering Principles

- Preserve educational quality over shipping speed.

- Do not redesign approved UI without explicit approval.

- Business logic belongs in engines, not components.

- Prefer small, reviewable pull requests.

- Every change must keep children’s progress intact.

## 2. Repository Workflow

- Create a feature branch from main.

- Verify dependencies before coding.

- Implement one logical feature per branch.

- Run build and tests locally.

- Open a Pull Request.

- Do not merge until reviewed.

## 3. Pull Request Template

Every PR should include: • Goal of the change • Files modified • Screens affected • Educational impact • Testing completed • Screenshots (if UI changed) • Known limitations

## 4. Coding Standards

- Keep components small and focused.

- Extract reusable logic into engines or services.

- Avoid duplicated code.

- Use descriptive names.

- Document non-obvious algorithms.

- Keep functions pure where possible.

## 5. AI-Assisted Development Rules

- AI may generate code but not product decisions.

- AI must follow the Product Vision and PRD.

- AI should preserve existing functionality unless instructed otherwise.

- AI-generated code must be reviewed before merge.

- Never expose API keys in generated code.

## 6. Documentation Rules

- Update documentation when architecture changes.

- Version all specification documents.

- Record breaking changes in CHANGELOG.

- Keep implementation aligned with documented acceptance criteria.

## 7. Branch Naming

- feature/<feature-name>

- fix/<bug-name>

- refactor/<module>

- docs/<document>

- release/<version>

## 8. Commit Message Guidelines

- feat: add adaptive mission generator

- fix: prevent keyboard overlap

- refactor: move reward logic into engine

- docs: update AI Coach specification

- test: add adaptive engine unit tests

## 9. Definition of Ready

- User story understood.

- Acceptance criteria defined.

- Dependencies identified.

- Design approved.

- Documentation available.

## 10. Definition of Done

- Build passes.

- Tests pass.

- No regressions introduced.

- Documentation updated.

- PR reviewed.

- Acceptance criteria met.

## 11. Release Management

- Tag releases using semantic versioning.

- Maintain release notes.

- Keep migration scripts when schema changes.

- Verify backward compatibility.

## 12. Code Review Checklist

- Architecture respected.

- Educational behaviour unchanged unless intended.

- Performance acceptable.

- Accessibility maintained.

- No duplicated logic.

- Error handling included.

- Local persistence verified.

## 13. Future Team Roles

- Product Owner

- Curriculum Specialist

- UX Designer

- Frontend Engineer

- Backend Engineer

- AI Engineer

- QA Engineer

- Illustrator / Animator

## Acceptance Criteria

- The playbook provides a repeatable development process.

- AI coding assistants can follow the same workflow as human developers.

- Every release remains aligned with the Product Vision.
