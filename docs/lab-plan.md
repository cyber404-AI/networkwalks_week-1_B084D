# Week 1 Lab Plan

## Purpose

Prepare a Kali Linux virtual machine for the NetworkWalks Academy Week 1 lab assignment and document the actual configuration with reproducible evidence.

## Existing setup

- Host: Windows 11
- Hypervisor: VMware
- Guest: Kali Linux
- Kali is already installed; reinstalling it is not part of this plan.

## Important hypervisor distinction

The assignment reference describes Oracle VirtualBox and a NAT Network. My existing Kali VM is in VMware. VMware and VirtualBox have different network and shared-folder configuration interfaces. I will document the hypervisor I actually use and will not label VMware screenshots as VirtualBox evidence.

If VirtualBox is mandatory for assessment, I must complete that requirement in VirtualBox separately. A VMware configuration alone should not be described as proof of a VirtualBox requirement.

## Assignment reference values

| Item | Reference value |
|---|---|
| Network type | NAT Network |
| Network range | 10.0.0.0/24 |
| Kali address | 10.0.0.2/24 |
| Shared folder path | /downloads |

These values are copied as requirements from the assignment context. They are not verified settings for my current VM.

## Verification procedure

1. Record the VMware product/version and VM hardware allocation.
2. Start Kali and identify the active network interface using `ip -br addr`.
3. Record the default route using `ip route`.
4. Record DNS configuration using `resolvectl status` or the resolver configuration available on the guest.
5. Test the configured gateway and a permitted external destination.
6. Test DNS resolution separately from basic IP connectivity.
7. Inspect the configured shared folder and confirm read/write access without exposing personal files.
8. Capture screenshots that show my own VM and the relevant settings.
9. Add the raw command output and screenshots to this repository, removing sensitive information first.

## Evidence rules

- Include the date and command used for each verification.
- Preserve actual output; do not manufacture terminal output.
- Distinguish a setting being configured from a feature being functionally tested.
- Do not claim a snapshot restore, file transfer, or network test unless it was performed.
- Do not include another person's screenshots, usernames, paths, or machine identifiers.
