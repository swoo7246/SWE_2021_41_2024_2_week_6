# SWE_2021_41_2024_2_week6
---

## Week 4 Assignment
- [Link of repository](https://github.com/swoo7246/SWE_2021_41_2024_2_week_4)

### MY_CODE
```python
def isHappy(n):
  li = []
  while n != 1 and n not in li:
    li.append(n)
    a = 0
    for i in str(n):
      a += int(i)**2
    n = a
  return n == 1
```
- This function determines whether the input number n is a "happy number" by continuously calculating the sum of the squares of its digits until it either equals 1 or falls into a repetitive cycle.
---
## Week 5 Assignment
> docker exec <container_name> cat /etc/os-release
> - This prints the operating system information by reading /etc/os-release file.
> - C:\Users\swoo7\docker_practice>docker exec ossp-container cat /etc/os-release\
PRETTY_NAME="Ubuntu 24.04.1 LTS"\
NAME="Ubuntu"\
VERSION_ID="24.04"\
VERSION="24.04.1 LTS (Noble Numbat)"\
VERSION_CODENAME=noble\
ID=ubuntu\
ID_LIKE=debian\
HOME_URL="https://www.ubuntu.com/"\
SUPPORT_URL="https://help.ubuntu.com/"\
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"\
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"\
UBUNTU_CODENAME=noble\
LOGO=ubuntu-logo

> docker exec <container_name> git --version
> - This checks the version of Git.
> - git version 2.43.0

> docker exec <container_name> python3 --version
> - This checks the version of Python.
> - Python 3.12.3

> docker inspect --format="{{ .HostConfig.Binds }}" <container_name>
> - This examines the container's configuration and prints the bind mounts.
> - [C:\Users\swoo7\docker_practice\ossp_host_dir:/mnt/ossp_container_dir]
