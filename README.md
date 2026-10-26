My Contribution: SARIF Validation & Error Handling

As part of the ReleaseShield AI project under the EPAM CoE program, I worked on SARIF 2.1.0 Validation and Error Handling (Role 9).

My responsibility was to develop a Python validator that checks scanner reports before they are passed to the SARIF merger. The validator uses the project's existing SARIF 2.1.0 JSON Schema to identify invalid reports and provide clear, actionable error messages.

Key Responsibilities

- JSON Parsing: Detect malformed JSON and report parsing errors with line and column information.
- Schema Validation: Validate scanner reports against the existing SARIF 2.1.0 schema using Python's "jsonschema" library.
- Version Checking: Reject reports that use unsupported SARIF versions.
- Structural Validation: Detect invalid report structures and missing required fields.
- Input Error Handling: Handle missing files, unreadable files, and invalid input paths.
- Automated Testing: Write pytest tests covering valid and invalid reports, schema violations, and input errors.
- Integration Readiness: Provide a validation interface that the merger can call before processing scanner findings.

Implementation

File| Responsibility
"src/validator.py"| SARIF report validation and error handling
"tests/test_validator.py"| Automated tests for validation behavior
"schemas/sarif-schema-2.1.0.json"| Existing schema used by the validator
"fixtures/"| Existing valid and invalid sample reports

The schema and original fixtures were prepared as part of the project's SARIF schema and test-fixture work. My contribution builds on that foundation by implementing the validation logic and its dedicated tests.

Technology Stack

- Python
- JSON
- JSON Schema
- "jsonschema"
- "pytest"
- Git and GitHub

Testing Results

The combined local test suite completed successfully:

12 tests passed

- 4 existing schema-fixture tests
- 8 validator tests

The tests were run against the project's checked-out schema and fixtures. They cover valid reports, unsupported versions, incorrect structures, malformed JSON, missing required fields, and file-access errors.

Scope of My Contribution

My component is responsible for validating scanner reports before they enter the merger.

It does not perform finding deduplication, merge multiple reports, or execute the security scanners. Those responsibilities belong to other components of ReleaseShield AI.

Project Impact

This component establishes a validation boundary between scanner output and downstream processing. It helps prevent malformed or structurally invalid reports from reaching the merger, improves debugging through understandable errors, and makes the input-processing pipeline more reliable.

Contribution: SARIF 2.1.0 Validation & Error Handling — Role 9, ReleaseShield AI / EPAM CoE Project.
