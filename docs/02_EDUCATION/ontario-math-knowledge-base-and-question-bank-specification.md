# Ontario Math Knowledge Base and Question Bank Specification

## Related Documents

- [Ontario Curriculum Framework and Learning Progression](../02_EDUCATION/ontario-curriculum-framework-and-learning-progression.md)
- [Curriculum Authoring Guide](../06_CONTENT/curriculum-authoring-guide.md)
- [TypeScript Interfaces and JSON Schemas](../05_ENGINEERING/typescript-interfaces-and-json-schemas.md)

## Migrated Content

## Math Adventure 12 – Ontario Math Knowledge Base & Question Bank Specification

Version 1.0 Educational Content Architecture

## Purpose

This document defines how mathematical knowledge is organized inside Math Adventure. It specifies curriculum structure, skill decomposition, metadata, question templates, mastery rules, misconceptions, and adaptive review logic. It serves as the educational content blueprint for developers, curriculum designers, and AI systems.

## 1. Content Design Principles

- Ontario curriculum is the single source of truth.

- Track skills, not worksheets.

- Every concept is broken into teachable micro-skills.

- Questions teach understanding before speed.

- Every question supports Tutor Mode.

- Every skill has measurable mastery criteria.

## 2. Curriculum Structure

| Level | Example | Purpose |
| --- | --- | --- |
| Grade | Grade 4 | School year |
| Strand | Number | Ontario curriculum strand |
| Topic | Fractions | Major concept |
| Skill | Equivalent Fractions | Adaptive tracking unit |
| Micro-skill | Recognize 1/2 = 2/4 | Question generation unit |

## Grades 1-3

- Counting

- Addition

- Subtraction

- Shapes

- Measurement

- Time

- Money

## Grades 4-5

- Multiplication

- Division

- Fractions

- Decimals

- Area & Perimeter

- Patterns

- Data

- Word Problems

## Grades 6-8

- Integers

- Ratios

- Percent

- Algebra

- Geometry

- Probability

- Surface Area & Volume

- Multi-step Problems

## 3. Skill Specification Template

Every skill in the database should contain: • Skill ID • Grade • Strand • Topic • Learning objective • Prerequisites • Common misconceptions • Difficulty progression (1-5) • Tutor strategies • Mastery criteria • Review schedule • Linked next skills

## 4. Question Metadata

- Question ID

- Grade

- Curriculum expectation

- Strand

- Topic

- Skill IDs

- Difficulty

- Estimated solving time

- Question type (numeric, MCQ, drag-and-drop, visual, word problem)

- Correct answer(s)

- Hint sequence

- Tutor Mode steps

- Explanation

- Misconception tags

- Accessibility notes

## 5. Difficulty Levels

- Level 1 – Confidence builder

- Level 2 – Standard practice

- Level 3 – Mixed application

- Level 4 – Multi-step reasoning

- Level 5 – Challenge / enrichment

## 6. Tutor Content Requirements

- Every question has at least two hints.

- Every question has a child-friendly explanation.

- Every concept includes a worked example.

- Every misconception has a recovery strategy.

- Every explanation uses age-appropriate language.

## 7. Mastery Rules

- Mastery requires repeated success across multiple missions.

- Mastered skills continue to appear using spaced repetition.

- Weak skills are revisited in different contexts.

- Mastery can decay after long periods without practice.

- Promotion depends on demonstrated understanding, not time.

## 8. Question Bank Targets

| Category | Recommended Initial Quantity |
| --- | --- |
| Each micro-skill | 20–50 questions |
| Challenge questions | 10+ |
| Word problems | 15+ |
| Visual models | 10+ |
| Tutor examples | 5+ |
| Review questions | 10+ |

## 9. AI Content Rules

- AI may generate additional practice questions but must follow curriculum metadata.

- AI explanations must align with approved learning objectives.

- AI cannot skip prerequisite skills.

- Generated content should be reviewed through automated validation before use.

## 10. Future Expansion

- Reading Adventure content repository

- Science knowledge base

- Financial literacy curriculum

- Teacher-imported curriculum maps

- Worksheet parsing and automatic skill extraction

## Acceptance Criteria

- Every curriculum expectation maps to measurable skills.

- Every skill maps to reusable question templates.

- Every question supports Tutor Mode.

- The adaptive engine can select questions using metadata alone.

- Content can expand without changing application architecture.
