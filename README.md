# Banking Workflow System

A mini project implementing banking workflow system using Spring Boot, PostgreSQL, Golang, and gRPC.

## Project Overview

This project implements a banking workflow system with features including:
- Limit checking
- Financial matrix checking
- User authentication & authorization
- Role-based access control
- Workflow management using Camunda BPM

## Technology Stack

### Core Technologies
- Java 17
- Spring Boot 3.x
- PostgreSQL
- Golang
- gRPC
- Camunda BPM
- Docker

### Additional Tools
- Maven
- Git
- Docker Compose

## Project Phases

### Phase 1: Project Setup and Basic Infrastructure

#### 1. Initial Setup
- [ ] Set up Spring Boot project with dependencies
  - Camunda BPM
  - Spring Security
  - PostgreSQL
  - gRPC
- [ ] Configure PostgreSQL database
- [ ] Set up basic project structure
- [ ] Configure application properties

#### 2. Authentication & Authorization
- [ ] Implement custom authentication service
- [ ] Integrate with KMS (Key Management System)
- [ ] Set up role-based access control (RBAC)
- [ ] Create user management APIs
- [ ] Implement token-based authentication

### Phase 2: Core Banking Workflow Components

#### 3. Design Basic Workflow
- [ ] Create BPMN workflow diagrams using Camunda Modeler
- [ ] Implement basic workflow steps:
  - User request initiation
  - Basic validation
  - Approval process
- [ ] Test workflow execution

#### 4. Implement Core Services
- [ ] Create service layer for:
  - Limit checking service
  - Financial matrix validation
  - Transaction processing
- [ ] Implement error handling
- [ ] Add logging and monitoring

### Phase 3: Advanced Features and Integration

#### 5. Golang Service Integration
- [ ] Set up Golang project structure
- [ ] Implement gRPC services
- [ ] Create Proto definitions
- [ ] Implement business logic services
- [ ] Set up Java-Golang communication

#### 6. Advanced Workflow Features
- [ ] Implement approval matrices
- [ ] Add dynamic routing
- [ ] Implement timeout handling
- [ ] Add workflow versioning

### Phase 4: Security and Validation

#### 7. Enhanced Security
- [ ] Implement additional security layers
- [ ] Add input validation
- [ ] Implement audit logging
- [ ] Add transaction signing

#### 8. Business Rules Implementation
- [ ] Create business rule engine
- [ ] Implement validation rules
- [ ] Add limit checking rules
- [ ] Implement matrix approval rules

### Phase 5: Testing and Documentation

#### 9. Testing
- [ ] Unit tests
- [ ] Integration tests
- [ ] Performance tests
- [ ] Security tests

#### 10. Documentation
- [ ] API documentation
- [ ] Workflow documentation
- [ ] Setup guide
- [ ] User guide

banking-workflow/
├── workflow-service (Java)
│   ├── src/main/java
│   │   ├── config
│   │   ├── controller
│   │   ├── model
│   │   ├── repository
│   │   ├── service
│   │   └── security
│   ├── src/main/resources
│   │   ├── bpmn
│   │   └── application.yml
│   └── src/test
│
├── business-service (Golang)
│   ├── cmd
│   ├── internal
│   │   ├── service
│   │   ├── repository
│   │   └── model
│   └── pkg
│
├── proto
│   └── banking
│       └── v1
│
└── docker
    ├── docker-compose.yml
    └── Dockerfile

## Setup Instructions

### Prerequisites
1. Java 17
2. Go 1.19+
3. PostgreSQL
4. Docker & Docker Compose
5. Maven
