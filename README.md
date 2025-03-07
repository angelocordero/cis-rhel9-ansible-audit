# CIS RHEL9 ANSIBLE AUDIT

Ansible playbook for the [CIS RHEL9 Benchmark](https://www.cisecurity.org/benchmark/red_hat_linux) Audits

## How to use
1. Clone the repo
2. Create an inventory file
3. Make sure the managed hosts has an `ansible` user, or change the `remote_user` property in `audit.yml`
4. Run the playbook using the command `ansible-playbook -i /path/to/your/inventory/file audit.yml -Kk`
	Note: the `-Kk` flag will ask you for the SSH password and the become password (so the playbook can be executed as root)

## Versions
This playbook was written and tested on `ansible [core 2.14.17]`

## Terms of Use
Access and utilization of this Ansible Playbook are contingent upon compliance with the [Terms of Use for Non-Member CIS Products](https://www.cisecurity.org/terms-of-use-for-non-member-cis-products)

## Disclaimer
This Ansible Playbook remains under development and does not represent a comprehensive audit. It may be subject to errors and defects. Some of the recommendations that are yet to be implemented include:
1. 5.3.6
2. 5.4
3. 5.5.1

## License
Copyright © 2025 & onwards, John Angelo Cordero <johnangelocordero.dev@gmail.com>

All work within this project and repository is subject to the terms of the MIT license, which can be found in the [LICENSE](./LICENSE) file.