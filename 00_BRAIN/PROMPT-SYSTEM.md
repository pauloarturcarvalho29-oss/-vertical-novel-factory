# Prompt System

Prompts are generated from structured specifications rather than written as isolated one-off prompts.

## Prompt layers
1. Global visual identity
2. Character identity
3. Location identity
4. Scene intent
5. Shot composition
6. Action and emotion
7. Camera and lighting
8. Model-specific parameters
9. Negative constraints

## Consistency rule
Character references, wardrobe, locations, and canonical visual traits must be injected from structured project records whenever the target model supports reference conditioning.

## Model adapter principle
A model adapter translates the common Shot Spec into the syntax and capabilities of a specific image or video model. The common creative specification must remain model-agnostic.
