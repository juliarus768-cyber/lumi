# Product Architecture and User Flows

## Related Documents

- [Math Adventure PRD](../01_PRODUCT/math-adventure-prd.md)
- [Parent Mission Control](../01_PRODUCT/parent-mission-control.md)
- [Screen-by-Screen Functional Specification](../01_PRODUCT/screen-by-screen-functional-specification.md)

## Migrated Content

## Math Adventure Product Architecture & User Flows

Version 1.0 Functional Architecture Specification

## Purpose

This document defines every major screen, navigation flow, and interaction in Math Adventure. It should allow a developer or AI coding assistant to understand how users move through the product before implementation.

## 1. User Roles

- Child (Learner)

- Parent / Guardian

- Future Family Members (multiple profiles)

## 2. Information Architecture

- Landing Screen

- Profile Selection

- Child Home

- Daily Adventure

- Tutor Mode

- Adventure Map

- Treasure Store

- Pet & Companion

- Achievements

- Summer Calendar

- Mission Control (Parent)

- Settings

## 3. Child Journey

1. Open app

2. Choose profile

3. Receive pet greeting and daily surprise

4. View today's mission

5. Complete 4 learning stages

6. Receive celebration and rewards

7. Visit Adventure Map or Store

8. Optionally complete Bonus Mission

9. Return tomorrow to maintain streak

## 4. Screen Specifications

### Landing Screen

Simple welcoming screen with logo, animated background, Play button and parent access.

- Primary purpose

- Key UI components

- Entry points

- Exit points

- Success state

- Error/empty states

### Profile Selection

Large profile cards. Alex (cat), Katya (dog). Future: unlimited profiles.

- Primary purpose

- Key UI components

- Entry points

- Exit points

- Success state

- Error/empty states

### Child Home

Hero screen with streak, pet, today's adventure, coins, XP and quick access to map and store.

- Primary purpose

- Key UI components

- Entry points

- Exit points

- Success state

- Error/empty states

### Daily Adventure

20 adaptive questions split into four stages. Progress shown as a journey rather than a checklist.

- Primary purpose

- Key UI components

- Entry points

- Exit points

- Success state

- Error/empty states

### Tutor Mode

Full-screen guided learning experience that explains concepts step-by-step without failure.

- Primary purpose

- Key UI components

- Entry points

- Exit points

- Success state

- Error/empty states

### Adventure Map

Visual progression across themed locations unlocked through consistent learning.

- Primary purpose

- Key UI components

- Entry points

- Exit points

- Success state

- Error/empty states

### Treasure Store

Reward redemption, purchase history, pending approvals and balance.

- Primary purpose

- Key UI components

- Entry points

- Exit points

- Success state

- Error/empty states

### Summer Calendar

Visual calendar showing completed, restored and perfect days.

- Primary purpose

- Key UI components

- Entry points

- Exit points

- Success state

- Error/empty states

### Mission Control

Parent dashboard with insights, approvals, reports and settings.

- Primary purpose

- Key UI components

- Entry points

- Exit points

- Success state

- Error/empty states

## 5. Navigation Principles

- One primary action per screen.

- Large touch-friendly controls.

- Minimal text on child screens.

- Consistent bottom navigation.

- No dead ends; every screen has a clear way back.

## 6. Animation Guidelines

- Screen transitions under 300 ms.

- Celebrate mission completion with confetti and pet animation.

- Smooth progress animations.

- Subtle idle animations for pets.

- Respect reduced-motion accessibility settings.

## 7. Offline Behaviour

- Daily missions available offline once generated.

- Progress saved locally.

- Automatic sync in future cloud version.

## 8. Acceptance Criteria

- Every screen has a defined purpose.

- All major user journeys are documented.

- Children can complete a full learning session without parent assistance.

- Parent can manage rewards and review progress without entering child mode.
