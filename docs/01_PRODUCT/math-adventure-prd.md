# Math Adventure PRD

## Related Documents

- [Math Adventure Product Vision and Philosophy](../00_MASTER_BIBLE/math-adventure-product-vision-and-philosophy.md)
- [Product Architecture and User Flows](../01_PRODUCT/product-architecture-and-user-flows.md)
- [Screen-by-Screen Functional Specification](../01_PRODUCT/screen-by-screen-functional-specification.md)

## Migrated Content

## Math Adventure Product Requirements Document (PRD)

Version 1.0 Functional Blueprint

## Purpose

This PRD defines the functional, educational, technical and user experience requirements for Math Adventure. It is intended to serve as the single source of truth for AI coding assistants and software developers. Features should be implemented incrementally while remaining faithful to the Product Vision & Philosophy.

## 1. Product Scope

- Adaptive Ontario mathematics learning platform for Grades 1–8 (Version 1 optimized for Grade 4→5 and Grade 7→8).

- AI tutor with personalized coaching.

- Gamified adventure experience for children.

- Mission Control dashboard for parents.

- Offline-first with local storage, future cloud synchronization.

## 2. User Personas

- Child learner (Alex profile).

- Child learner (Katya profile).

- Parent / Guardian.

- Future multi-child household.

## 3. Information Architecture

- Landing/Profile Selection

- Child Home

- Daily Adventure

- Tutor Mode

- Adventure Map

- Treasure Store

- Pet

- Achievements

- Summer Calendar

- Mission Control

- Settings

## 4. Daily Adventure Flow

- Login reward.

- Pet greeting.

- Warm-Up (5 questions).

- Skill Builder (5 questions).

- Adventure Round (5 questions).

- Boss Round (5 questions).

- Celebration sequence.

- Unlock Bonus Mission.

## 5. Adaptive Learning Engine

- Track mastery by skill rather than by question.

- Maintain confidence level for each skill.

- Prioritize weak concepts.

- Introduce next-grade concepts gradually.

- Use spaced repetition.

- Maintain learning history.

## 6. Tutor Mode

- Never fail a child.

- Guide with hints.

- Ask scaffolded questions.

- Offer multiple-choice intermediate steps.

- Retry original question.

- Save unresolved skills for future missions.

## 7. AI Coach (Future API)

- Explain mistakes.

- Adapt to learning style.

- Generate personalized examples.

- Recommend home activities.

- Generate parent summaries.

- Never replace curriculum sequencing.

## 8. Companion System

- Version 1: Alex = Cat, Katya = Dog.

- Future: selectable companions.

- Companion acts as tutor and emotional guide.

## 9. Reward Economy

- Coins for completion.

- XP for learning.

- Badges for persistence.

- Store categories: Fun, Family, Savings.

- Parent approval workflow.

- Purchase history.

- Undo last purchase.

## 10. Adventure Map

- Weekly travel progression.

- Unlock regions.

- Mystery rewards.

- Seasonal events.

- Collectibles.

## 11. Summer Calendar

- Track completed days.

- Perfect days.

- Restored streak days.

- Weekly milestones.

- End-of-summer certificate.

## 12. Parent Mission Control

- Coach Insights.

- Learning strengths.

- Weak skills.

- Recommendations.

- Reward approvals.

- Monthly streak restore.

- Weekly reports.

## 13. Technical Requirements

- React + Vite.

- PWA.

- Responsive for tablets.

- Offline-first.

- localStorage abstraction.

- Future API layer.

- Modular architecture.

## 14. Data Model

- Child Profile

- Mission

- Skill

- Question

- Reward

- Purchase

- Badge

- Pet

- Calendar

- Adventure Progress

- Parent Settings

## 15. Accessibility

- Readable fonts.

- Touch-friendly controls.

- Reduced motion option.

- Future text-to-speech.

- Numeric keyboard for answers.

## 16. Acceptance Criteria

- Build passes.

- Responsive on tablet/mobile.

- Daily missions adaptive.

- Reward store functional.

- Keyboard never hides question.

- Progress persists after refresh.

## 17. Future Roadmap

- Reading Adventure.

- Science Adventure.

- Homework upload and AI lesson planning.

- Teacher worksheet analysis.

- Cloud sync.

- Voice tutor.

- Family challenges.

- Multi-curriculum support.

## Appendix A – Screen Specifications (To Be Expanded)

### A.1 Landing

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

### A.2 Profile Selection

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

### A.3 Child Dashboard

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

### A.4 Daily Adventure

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

### A.5 Tutor Mode

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

### A.6 Adventure Map

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

### A.7 Treasure Store

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

### A.8 Pet

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

### A.9 Achievements

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

### A.10 Summer Calendar

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

### A.11 Mission Control

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

### A.12 Settings

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

### A.13 Weekly Report

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

### A.14 Monthly Report

Purpose - Define primary user goal. UI Components - Layout, navigation, states, animations. Interactions - User actions and transitions. Acceptance Criteria - Functional completion requirements. Future Enhancements.

## Document Status

This is Version 1.0 of the PRD framework. Each section is intended to be expanded into detailed functional specifications during subsequent design iterations until the document becomes the complete implementation blueprint.
