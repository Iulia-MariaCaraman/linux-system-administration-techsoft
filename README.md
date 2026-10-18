# Linux Server Administration: Multi-Department Access and Security

Operating systems coursework project configuring a secured multi-tenant Ubuntu server for an enterprise environment.

## Overview
This project establishes a secured directory structure, access control policy, and user hierarchy on Ubuntu Linux based on the principle of least privilege.

The implementation secures departmental workspaces across software development, design, DevOps, and corporate management teams.

## Key Configuration Highlights
* User and Group Management: Provisioned system accounts with dedicated GIDs, secondary group memberships, and password aging policies.
* Directory Architecture: Structured the `/srv/techsoft` hierarchy enforcing strict ownership boundaries.
* Special Permission Bits:
  * SetGID: Preserves consistent group ownership on shared developer directories.
  * Sticky Bit: Prevents cross-user deletion in collaborative public directories.
  * SUID: Configured on deployment scripts to permit controlled execution under elevated ownership.
* Security Audit: Verified access control lists through simulated multi-user test cases and terminal logging.

## Repository Contents
* raport_proiect.pdf: Technical report detailing project requirements, permission tables, security tests, and configuration reflections.
* sesiune_terminal.txt: Complete bash shell command session history and execution audit logs.
