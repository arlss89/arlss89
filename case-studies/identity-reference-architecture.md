# Identity and Authentication Reference Architecture

## Overview

A reference architecture for secure identity workflows in a distributed application.

## Engineering focus

- Account registration and sign-in
- Passwordless authentication
- One-time passcode verification
- Multi-factor authentication
- Contact verification
- Session and token lifecycle
- Authorization boundaries
- Event-driven integration between identity services
- Customizable authentication journeys

## Architecture

The reference solution separates:

- Identity profile management
- Contact verification
- Authentication orchestration
- Notification delivery
- Authorization and access decisions
- Integration events
- User-facing authentication screens

An Ory-based identity layer can provide a flexible foundation for customized authentication journeys, while the application controls the user-facing HTML experience and keeps identity and authorization concerns isolated from presentation details.

This approach can reduce coupling to provider-specific interfaces and allow backend and frontend components to evolve independently.

## Engineering considerations

- Secure token handling
- Replay and abuse prevention
- Rate limiting
- Idempotent verification operations
- Auditability and correlation identifiers
- Contract and integration testing
- Failure handling for external notification providers
- Safe rollout of authentication policy changes
- Secure frontend/backend integration
- Accessible and maintainable authentication interfaces

## Scope

This is an independent, generalized reference architecture. It does not reproduce any employer's policies, endpoints, claims, tenant configuration, naming conventions or implementation.
