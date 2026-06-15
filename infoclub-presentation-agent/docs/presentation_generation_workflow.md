# Presentation Generation Workflow Specification

This workflow defines the ordered presentation generation process for the InfoClub Presentation Agent.
Each stage must complete before the next stage begins.

## Workflow

Request
↓
Audience Analysis
↓
Knowledge Selection
↓
Presentation Planning
↓
Slide Generation
↓
Brand Enforcement
↓
Presentation Artifact

## Stages

### 1. Request

Read the presentation request contract and identify the requested presentation type, audience, goal, tone, duration, language, and additional context.

### 2. Audience Analysis

Match the request audience to the operational audience profiles in the knowledge layer.
If audience data is unknown, keep it marked as unknown instead of inventing audience needs.

### 3. Knowledge Selection

Select only relevant knowledge sources for the requested audience and goal.
Apply claims and constraints before using any factual statement.

### 4. Presentation Planning

Create a slide-level plan that matches the presentation type, goal, audience, duration, tone, and language.

### 5. Slide Generation

Generate slide titles and content from the approved plan and selected knowledge sources.
Do not introduce unsupported facts during slide generation.

### 6. Brand Enforcement

Apply brand guide, color, typography, and presentation rules before producing the final draft.

### 7. Presentation Artifact

Produce the final structured presentation draft as the presentation artifact.
