# OpenRAG Issue #1460 – Bug Investigation

## Project
OpenRAG – Open-source Retrieval-Augmented Generation application.

## Problem
Answers containing words like `resources` or `Ressources` may be incorrectly detected as source citation tags.

## Suspected Cause
The source filtering regex does not properly distinguish the word `Sources` from part of another word.

## Investigation Plan
1. Understand the source filtering implementation.
2. Study the `_SOURCES_LABEL` regex.
3. Reproduce the reported bug.
4. Understand the existing tests.
5. Implement and verify a fix.

## Learning Goals
- Python debugging
- Regular expressions
- Pytest
- Git and GitHub
- Open-source contribution
