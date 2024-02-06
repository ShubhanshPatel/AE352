# [AE352] Changing passwords

The use case allows you to change the password, as desired:
- an account defined on a machine list,
- an account defined on an inventory,
- all accounts expiring on a machine list,
- of all accounts expiring on an inventory.

## Prerequisites and dependencies

The custom keepass module (in the mod-isim2-keepass repo) must be present in venv/EE.

## Use

Input variables:
- (optional) ansible_limit: must be defined to limit execution to a list of machines rather than the general inventory.
- (optional) change_mdp_user_to_update: must be defined to limit execution to a defined account rather than all expiring accounts.
- use_case_environment: (DEV|PRD) use case execution environment.
- use_case_report_email: list of emails (comma separated) which will receive the execution report.