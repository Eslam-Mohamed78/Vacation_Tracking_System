# Vacation Tracking System (VTS)

## Table of content

- [Vision](#vision)
- [Functional Requirements](#functional-requirements)
- [Non-Functional Requirements](#non-functional-requirements)
- [Constraints](#constraints)
- [Top Level Use Case Model](#use-case-model)
- [Use case [Manage-time]](#mange-time-use-case)

---

## Vision

The main goal of this application is to improve the internal business processes of the organization by reducing the time it takes to manage vacation time, sick leave, and personal time off,
Without having to be an expert in company policy.


---

## Functional Requirements

- **Rules-based system**: For validating and verifying leave time requests.
- **Enables manager approval (optional)**: To the vacation requests by the employees
- **Requests Access**: Providing access to requests for the previous calender year, and allows requests to be made up to a year and half in the future.
- **Email notifications**: For
  - Manager: To approve the request.
  - Employee: To give update with the request status changes.
- **Single sign-on mechanism (SSO)** For authentication using existing intranet portal system.
- **Activity logs** for all transactions (auditing).
- **Override restricted rules**: By the HR and system administration personnel to override all actions restricted by rules, with logging of those overrides.
- **Personal leave time**: Allows managers to directly award personal leave time.
- **Integration services**: For
  - Employee's vacation requests summary: System should provide Web service inteface for other inernal systems to query any given employee's vacation request summary.
  - HR department: To enable legacy systems to retrieve required employee information and changes.

---

## Non-Functional Requirements

- Emphasis on user experience to match existing organization systems.
- The system must be user-friendly and intuitive

---

## Constraints

- Integrations with legacy systems.
- Support for single sign-on.
- Uses existing hardware and middleware

---

## Top Level Use Case Model

![Use Case Model](./use_cases/top_level_use_case_model.png)

---

## Use case [Manage-time]

- **Actor**: Employee
- **Goal**: Employee wishes to submit new vacation time request.
- **Preconditions**:
  - Employee is authenticated by portal system.
  - To be identified as Employee of the company with privileges to manage his own vacation time.
- **Flow chart**: ![Manage time use case](./use_cases/manage_time/flow_chart.png)

---