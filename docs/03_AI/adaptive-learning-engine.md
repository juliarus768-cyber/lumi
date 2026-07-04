# Adaptive Learning Engine

## Related Documents

- [AI Coach Specification](../03_AI/ai-coach-specification.md)
- [AI Prompt Engineering Manual](../03_AI/ai-prompt-engineering-manual.md)
- [Ontario Curriculum Framework and Learning Progression](../02_EDUCATION/ontario-curriculum-framework-and-learning-progression.md)

## Migrated Content

## Math Adventure Adaptive Learning Engine Specification

Version 1.0 Core Intelligence of Math Adventure

## Purpose

This document defines the adaptive learning engine that powers Math Adventure. It explains how the application determines what each child should learn next, how it adapts to strengths and weaknesses, how Tutor Mode behaves, and how progress is measured. This engine is the core intellectual property of the product and should remain consistent even as the visual design evolves.

## 1. Design Principles

- Every child can succeed.

- Understanding is more important than speed.

- The app adapts to the learner, not the learner to the app.

- Children are never punished for mistakes.

- Mastery is earned through practice over time.

- The experience should feel like an adventure, not a worksheet.

## 2. Student Learning Profile

Each child has a persistent learning profile stored locally (future cloud sync).

- Current grade and next grade

- Learning goals

- Skill mastery profile

- Learning style profile

- Confidence level

- Persistence indicators

- Preferred explanation style

- History of misconceptions

- Mission history

- Streak history

## 3. Skill-Based Learning Model

The engine tracks skills rather than individual questions. Every question is tagged with one or more curriculum skills.

- Multiplication facts

- Division

- Long division

- Fractions

- Equivalent fractions

- Decimals

- Percents

- Integers

- BEDMAS

- Geometry

- Measurement

- Money

- Time

- Patterns

- Word problems

- Data and graphs

- Algebra foundations

## 4. Mastery Levels

- Beginning

- Developing

- Practicing

- Confident

- Mastered

Mastery is determined using multiple successful demonstrations over time rather than a single correct answer.

## 5. Daily Mission Generator

Every weekday the engine creates one required mission containing 20 questions divided into four stages.

- Warm-Up (5)

- Skill Builder (5)

- Adventure Round (5)

- Boss Round (5)

Question distribution:

- 30% weak skills

- 25% current grade review

- 20% previously missed concepts

- 15% next-grade preparation

- 10% challenge questions

## 6. Adaptive Strategy

The adaptive engine uses a hybrid strategy (approved product decision).

The curriculum continues to progress normally while quietly increasing the frequency of weak skills. Weak concepts are revisited over several days using spaced repetition and different contexts rather than replacing the entire mission.

- Maintain balanced curriculum coverage.

- Increase practice for weak skills.

- Mix review naturally into future missions.

- Reduce frequency after consistent mastery.

- Re-check mastered skills periodically.

## 7. Tutor Mode

Tutor Mode activates automatically after an incorrect answer. There is no mission failure.

- Pet offers encouragement.

- Break the problem into smaller steps.

- Ask scaffolded multiple-choice questions.

- Provide hints instead of answers first.

- Allow another attempt.

- Explain the concept if still incorrect.

- Schedule similar practice later in the mission or future missions.

## 8. Learning Style Adaptation

The engine gradually learns how each child learns best.

- Independent problem solver

- Visual learner

- Needs worked examples

- Benefits from encouragement

- Rushing tendencies

- Confidence level

- Preferred pacing

Future AI will personalize explanations using this profile.

## 9. Misconception Tracking

Incorrect answers are classified whenever possible.

- Calculation error

- Concept misunderstanding

- Fact recall issue

- Misread question

- Place value confusion

- Fraction misconception

- Rushing

- Confidence issue

Different misconceptions trigger different tutoring strategies.

## 10. Progress Metrics

- Knowledge XP

- Courage XP

- Coins

- Badges

- Skill mastery

- Longest streak

- Weekly growth

- Monthly growth

## 11. Parent Insights

- Strongest skills

- Skills needing attention

- Recent improvements

- Tutor Mode usage

- Recommended home activities

- Weekly coaching summary

## 12. AI Integration Roadmap

OpenAI or another LLM will enhance the engine but will not replace deterministic curriculum sequencing.

- Generate personalized explanations.

- Adjust tutoring style.

- Generate additional practice.

- Summarize learning progress.

- Recommend real-life activities.

- Analyze uploaded worksheets in future versions.

## 13. Acceptance Criteria

- Every mission is personalized.

- Questions are selected by skill mastery.

- Weak skills receive additional practice without dominating the curriculum.

- Tutor Mode always supports the learner until understanding improves.

- Progress persists between sessions.

- Parent dashboard reflects learning insights generated by the engine.

## Future Expansion

The adaptive engine is designed to support additional subjects such as Reading Adventure, Science Adventure, Financial Literacy Adventure, and Homework Adventure without redesigning the underlying architecture.
