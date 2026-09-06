# On-Device Movement Analysis

## Overview

A privacy-first mobile application concept for analyzing movement videos locally on the user's device.

## Engineering focus

- On-device video processing
- Skeleton and keypoint-based analysis
- Mobile-first architecture
- Offline-capable workflows
- Shared domain logic across platforms
- Explicit confidence and inconclusive-result handling
- Local persistence with user-controlled retention

## Architecture

The application is organized into four main layers:

1. Capture or import video
2. Extract movement data locally
3. Apply exercise-specific evaluation rules
4. Present results and preserve selected history locally

The design minimizes data transmission and keeps raw media under the user's control.

## Engineering considerations

- Platform-specific camera and vision APIs
- Shared domain models and validation rules
- Incremental processing for longer videos
- Graceful handling of missing or low-confidence keypoints
- Clear separation between detection, scoring and presentation
- Automated tests for domain rules and temporal calculations

## Scope

This case study presents architectural principles and engineering decisions in generalized form. It does not contain proprietary code, datasets, model weights or production configuration.
