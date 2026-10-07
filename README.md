# IntelliAttend

## Multimodal AI Attendance and Authentication System

IntelliAttend is a multimodal AI-based attendance and authentication system that combines face recognition and voice recognition to verify user identity and automate attendance recording.

The application provides separate workflows for students and teachers, with database-backed attendance management and role-based access to application functionality.

The project demonstrates the integration of computer vision, speech processing, machine learning, authentication, database management, and web application development.

---

## Problem Statement

Traditional attendance systems often rely on manual verification, identity cards, or single-factor authentication. These approaches can increase administrative effort and may be vulnerable to proxy attendance and unauthorized access.

IntelliAttend explores a multimodal biometric approach where facial and voice characteristics are used to verify user identity before recording an attendance event.

The goal is to build an automated attendance workflow that integrates AI-based identity verification with secure application and database components.

---

## Objectives

- Automate attendance recording using AI-based identity verification.
- Implement face-based user recognition.
- Implement voice-based user recognition.
- Provide separate student and teacher workflows.
- Maintain attendance records using a database.
- Implement role-based access to application functionality.
- Integrate AI inference with a web-based application.
- Provide a foundation for multimodal biometric authentication.

---

## Key Features

### Face Recognition

The system processes facial input to identify registered users and support identity verification.

### Voice Recognition

The system processes voice input to provide an additional biometric authentication signal.

### Multimodal Authentication

Face and voice recognition can be used as complementary authentication signals for identity verification.

### Student Portal

Authenticated students can access functionality related to:

- Attendance
- Attendance history
- Profile information
- Authentication

### Teacher Portal

Authenticated teachers can access functionality related to:

- Student records
- Attendance records
- Attendance monitoring
- Dashboard-based management

### Database-Backed Attendance

Verified attendance events are stored in a structured database for subsequent retrieval and monitoring.

### Role-Based Access

Application functionality is separated based on the authenticated user's role.

---

## System Architecture

```text
                         User
                           |
                           v
                  Web Application
                           |
              +------------+------------+
              |                         |
              v                         v
       Student Portal             Teacher Portal
              |                         |
              +------------+------------+
                           |
                           v
                    Authentication
                           |
              +------------+------------+
              |                         |
              v                         v
       Face Recognition          Voice Recognition
              |                         |
              +------------+------------+
                           |
                           v
                  Identity Verification
                           |
                           v
                   Attendance Service
                           |
                           v
                       Database



                       
