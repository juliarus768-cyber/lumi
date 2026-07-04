# TypeScript Interfaces and JSON Schemas

## Related Documents

- [Backend and Cloud Architecture](../05_ENGINEERING/backend-and-cloud-architecture.md)
- [Developer Playbook](../05_ENGINEERING/developer-playbook.md)
- [Ontario Math Knowledge Base and Question Bank Specification](../02_EDUCATION/ontario-math-knowledge-base-and-question-bank-specification.md)

## Migrated Content

## Math Adventure 14 – TypeScript Interfaces & JSON Schemas

Version 1.0 Implementation Data Contracts

## Purpose

This document defines the canonical data contracts for Math Adventure. These interfaces should become the single source of truth for the frontend, future backend, storage layer, AI services, and cloud synchronization.

### AppState

Contains the complete persisted application state including schemaVersion, active profile, child profiles, rewards, missions, badges, purchases, calendar and settings.

Example TypeScript interface AppState { id: string; // Additional properties defined by the Technical Architecture document. }

### ChildProfile

Stores learner identity, grade, companion, balances, streak, goals and LearningProfile.

Example TypeScript interface ChildProfile { id: string; // Additional properties defined by the Technical Architecture document. }

### LearningProfile

Stores mastery by skill, learning style, misconceptions, review queue and adaptive settings.

Example TypeScript interface LearningProfile { id: string; // Additional properties defined by the Technical Architecture document. }

### SkillRecord

Tracks attempts, accuracy, mastery level, confidence, review dates and Tutor Mode usage.

Example TypeScript interface SkillRecord { id: string; // Additional properties defined by the Technical Architecture document. }

### Mission

Represents a generated required, bonus or challenge mission with four stages.

Example TypeScript interface Mission { id: string; // Additional properties defined by the Technical Architecture document. }

### MissionResult

Stores completed answers, Tutor Mode events, rewards earned and mastery updates.

Example TypeScript interface MissionResult { id: string; // Additional properties defined by the Technical Architecture document. }

### Question

Curriculum-tagged learning object with hints, explanation, misconception tags and metadata.

Example TypeScript interface Question { id: string; // Additional properties defined by the Technical Architecture document. }

### Reward

Represents a purchasable reward or unlockable family activity.

Example TypeScript interface Reward { id: string; // Additional properties defined by the Technical Architecture document. }

### Purchase

Tracks reward request, approval workflow and redemption history.

Example TypeScript interface Purchase { id: string; // Additional properties defined by the Technical Architecture document. }

### Badge

Achievement metadata and earned status.

Example TypeScript interface Badge { id: string; // Additional properties defined by the Technical Architecture document. }

### CalendarDay

Daily completion, streak and effort information.

Example TypeScript interface CalendarDay { id: string; // Additional properties defined by the Technical Architecture document. }

### AdventureProgress

Current world, unlocked regions and collectibles.

Example TypeScript interface AdventureProgress { id: string; // Additional properties defined by the Technical Architecture document. }

### ParentSettings

Reward rules, curriculum settings, vacation mode and advanced options.

Example TypeScript interface ParentSettings { id: string; // Additional properties defined by the Technical Architecture document. }

## JSON Schema Guidelines

- Every persisted object contains an id where appropriate.

- Dates use ISO-8601 strings.

- Enums are preferred over free-form strings.

- Unknown fields should be ignored to support forward compatibility.

- schemaVersion is mandatory for migration.

## API Contracts (Future)

All server communication should use versioned REST or RPC endpoints.

| Endpoint | Request | Response |
| --- | --- | --- |
| /missions/generate | Child profile + date | Mission |
| /tutor/explain | Question + misconception | Tutor response |
| /reports/weekly | Child ID | Weekly coaching report |
| /sync | AppState delta | Updated AppState |
| /worksheet/analyze | Worksheet metadata | Detected skills + study plan |

## Validation Rules

- Reject invalid schemaVersion.

- Validate required fields before persistence.

- Prevent negative coin balances.

- Mission must contain exactly 20 required questions.

- Reward purchase requires sufficient balance.

- Child grade must match supported curriculum.

## Migration Strategy

Each storage version should include migration functions. Example: v1 -> v2 : Add LearningDNA v2 -> v3 : Add CloudSync metadata v3 -> v4 : Add Multi-subject progress Older data should migrate automatically without loss.

## Developer Checklist

- Implement interfaces before business logic.

- Keep interfaces synchronized with PRD updates.

- Generate JSON validation from interfaces where possible.

- Never duplicate model definitions across modules.

- Document breaking changes in CHANGELOG.

## Acceptance Criteria

- Every major entity has a documented interface.

- Future backend can consume the same contracts.

- Codex can scaffold models directly from this document.

- Schema supports future AI, cloud sync and additional subjects.
