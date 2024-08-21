---
x-trestle-comp-def-rules:
  appid-D:
    - name: appid_redirect_uris_no_localhost_or_127001
      description: Ensure App ID redirect URIs are not using localhost or 127.0.0.1
    - name: appid_redirect_uris_no_wildcards
      description: Ensure App ID redirect URIs are not using wildcards (*)
x-trestle-param-values:
  sc-07_odp:
x-trestle-global:
  profile:
    title: NIST Special Publication 800-53 Revision 5 HIGH IMPACT BASELINE
    href: profiles/acme-profile-nist-800-53/profile.json
  sort-id: sc-07
---

# sc-7 - \[System and Communications Protection\] Boundary Protection

## Control Statement

- \[a.\] Monitor and control communications at the external managed interfaces to the system and at key internal managed interfaces within the system;

- \[b.\] Implement subnetworks for publicly accessible system components that are {{ insert: param, sc-07_odp }} separated from internal organizational networks; and

- \[c.\] Connect to external networks or systems only through managed interfaces consisting of boundary protection devices arranged in accordance with an organizational security and privacy architecture.

## Control Assessment Objective

- \[SC-07a.\]

  - \[SC-07a.[01]\] communications at external managed interfaces to the system are monitored;
  - \[SC-07a.[02]\] communications at external managed interfaces to the system are controlled;
  - \[SC-07a.[03]\] communications at key internal managed interfaces within the system are monitored;
  - \[SC-07a.[04]\] communications at key internal managed interfaces within the system are controlled;

- \[SC-07b.\] subnetworks for publicly accessible system components are {{ insert: param, sc-07_odp }} separated from internal organizational networks;

- \[SC-07c.\] external networks or systems are only connected to through managed interfaces consisting of boundary protection devices arranged in accordance with an organizational security and privacy architecture.

## Control guidance

Managed interfaces include gateways, routers, firewalls, guards, network-based malicious code analysis, virtualization systems, or encrypted tunnels implemented within a security architecture. Subnetworks that are physically or logically separated from internal networks are referred to as demilitarized zones or DMZs. Restricting or prohibiting interfaces within organizational systems includes restricting external web traffic to designated web servers within managed interfaces, prohibiting external traffic that appears to be spoofing internal addresses, and prohibiting internal traffic that appears to be spoofing external addresses. [SP 800-189](#f5edfe51-d1f2-422e-9b27-5d0e90b49c72) provides additional information on source address validation techniques to prevent ingress and egress of traffic with spoofed addresses. Commercial telecommunications services are provided by network components and consolidated management systems shared by customers. These services may also include third party-provided access lines and other service elements. Such services may represent sources of increased risk despite contract security provisions. Boundary protection may be implemented as a common control for all or part of an organizational network such that the boundary to be protected is greater than a system-specific boundary (i.e., an authorization boundary).

______________________________________________________________________

## What is the solution and how is it implemented?

<!-- For implementation status enter one of: implemented, partial, planned, alternative, not-applicable -->

<!-- Note that the list of rules under ### Rules: is read-only and changes will not be captured after assembly to JSON -->

<!-- Add control implementation description here for control: sc-7 -->

### Implementation Status: operational

______________________________________________________________________

## Implementation for part a.

<!-- Add control implementation description here for item a. -->

### Rules:

  - appid_redirect_uris_no_localhost_or_127001
  - appid_redirect_uris_no_wildcards

### Implementation Status: planned

______________________________________________________________________

## Implementation for part b.

<!-- Add control implementation description here for item b. -->

### Rules:

  - appid_redirect_uris_no_localhost_or_127001
  - appid_redirect_uris_no_wildcards

### Implementation Status: planned

______________________________________________________________________
