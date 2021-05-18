# Roadmap: Formula

## Strategy

### Why are we building this?

- The PII that is submitted for employment needs to be encrypted at rest.
- Current form submission is not scalable given its resides within Google forms.

### Who are our consumers?

Consumers will be clients in need of a submittable form that can be configured to meet their specific use cases.

## Personas

- Admin
- Manager
- Applicant
- User

## Capabilities

- User can navigate to Formula UI
- User can be authenticated
- User can be created
- Admin can create a tenant
- Admin can create a manager
- Admin can add a manager to tenant
- Manager can create an application for a tenant
- Manager can create a common input for tenant
- Manager can create a custom input for a given application
- Manager can view submitted applications
- Manager can review a submitted application
- Manager can print a submitted application
- Applicant can submit an application with photo identification

## System Architecture

See diagram below

## Features

- UI
  - User will authenticate using Google OAuth 2.0
  - Admin can create a tenant
  - Admin can create a manager
  - Admin can add a manager to tenant
  - Manager can create an application for a tenant
  - Manager can create a common input for tenant
  - Manager can create a custom input for a given application
  - Applicant can submit an application with photo identification
  - Manager can view applicants
  - Manager can review an applicant
  - Manager can print PDF of applicant's application
- Middle Tier
  - Validate OAuth token
  - Create user from OAuth token
  - Create a tenant
  - Create a manager
  - Assign manager to a tenant
  - Create application
  - Create a common input at tenant level
  - Create a custom input at application level
  - Create applicant
  - Email photo identification
  - View list of applications
  - View single application
  - Review application
- Database
  - Create User
  - Create Tenant
  - Create Manager
  - Link Tenant-Manager
  - Create Application
  - Create Input:Common
  - Create Input:Custom
  - Create Applicant
  - Read Applications
  - Read Application
  - Update Application
