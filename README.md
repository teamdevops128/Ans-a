Description

We need to enable execution of Ansible playbooks on Windows machines to automate configuration management and operational tasks. This includes validating connectivity, ensuring required prerequisites (WinRM/SSH) are configured, and confirming that network-related changes (e.g., firewall rules, routes, NIC configuration, DNS updates) are captured and documented during execution. The solution should allow us to track any network changes applied to Windows machines via Ansible for auditing and rollback purposes.

Acceptance Criteria

Connectivity & Setup

Ansible control node can connect to Windows hosts using WinRM (or SSH if configured).

Necessary Python/PowerShell dependencies for Windows automation are in place.

Inventory file includes Windows hosts with correct connection variables.

Playbook Execution

Ansible playbooks can be successfully executed on Windows hosts without manual intervention.

Tasks can run with appropriate privileges (Administrator access).

Execution logs are captured and stored.

Network Change Tracking

Any playbook that modifies network configurations (e.g., IP, DNS, routing, firewall) logs changes to a centralized location.

Reports include before/after state for each change.

Rollback instructions or playbooks exist to revert changes if needed.

Validation

Test playbook demonstrates successful execution on a Windows host.

Logs confirm detection and capture of network-related changes.

Documentation updated with steps to run Windows playbooks and interpret change reports.
