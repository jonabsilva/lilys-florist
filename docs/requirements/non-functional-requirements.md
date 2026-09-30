# Non-Functional Requirements

The following non-functional requirements define the constraints under which the system must operate. They share the same derivation as the functional requirements.

## NFR-01 — Page Performance

The system shall load normal customer-facing pages in approximately 2 seconds under expected operating conditions.

## NFR-02 — Checkout Performance

The system shall complete checkout actions in approximately 3 seconds under expected operating conditions.

## NFR-03 — Peak-Period Reliability

The system shall support peak periods of 100+ orders per day without timeouts or failed orders.

## NFR-04 — Payment and Order Consistency

The system shall not confirm an order unless payment succeeds and shall not charge a customer without a corresponding confirmed transaction.

## NFR-05 — Security and Role-Based Access

The system shall provide secure authentication, temporary lockout after several failed login attempts, secure password reset through the registered email address, and role-limited access to staff, manager, and owner/admin information and settings.

## NFR-06 — Privacy and Data Protection

The system shall protect customer personal data in accordance with applicable Irish/EU privacy requirements and support appropriate requests for access to or deletion of personal information.

## NFR-07 — Accessibility and Responsive Use

The system shall provide readable content, appropriate contrast, image descriptions, simple navigation, assistive-technology-friendly forms, and a usable experience across mobile, tablet, and desktop devices.

## NFR-08 — Maintainability, Hosting, and Backups

The system shall use a dependable hosted service that supports reliable operation during high-demand periods and regular backups, and shall allow Lily and authorized managers to manage relevant business content without technical assistance. Exact backup frequency, retention, and recovery targets remain open questions.
