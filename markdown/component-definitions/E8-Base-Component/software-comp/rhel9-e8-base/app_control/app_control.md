---
x-trestle-comp-def-rules:
  software-comp:
    - name: rule-app_control
      description: Rule for app_control
x-trestle-global:
  profile:
    title: rhel9-e8-base
    href: trestle://profiles/rhel9-e8-base/profile.json
  sort-id: app_control
---

# app_control - \[REPLACE_ME\] Application Control

## Control Statement

______________________________________________________________________

## What is the solution and how is it implemented?

Implementing application control within Linux environments can be achieved using the File Access Policy daemon (fapolicyd). The fapolicyd framework allows Linux system administrators to control which applications are allowed (or denied) execution based on either path, hash, MIME type or if they are trusted (i.e. properly installed by the system package manager and registered in the RPM database). Red Hat’s Security Hardening publication provides advice on how to configure and manage the use of the fapolicyd framework within Red Hat Enterprise Linux 9.

selinux will be enabled by default within Red Hat Enterprise Linux 9, which will ensure authorized access prior to any changes to the package manager configuration or repositories being made.

<!-- For implementation status enter one of: implemented, partial, planned, alternative, not-applicable -->

<!-- Note that the list of rules under ### Rules: is read-only and changes will not be captured after assembly to JSON -->

<!-- Add control implementation description here for control: app_control -->

### Rules:

  - rule-app_control

### Implementation Status: planned

______________________________________________________________________
