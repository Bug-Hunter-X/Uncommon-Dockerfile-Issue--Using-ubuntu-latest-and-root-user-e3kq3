This repository demonstrates a common but often overlooked issue in Dockerfiles: the use of `ubuntu:latest` and running commands as root.  `ubuntu:latest` is huge and frequently updated, causing unpredictable build times and potential security risks. Running commands as root introduces unnecessary privilege escalation.  The solution demonstrates best practices, including using a slimmer base image and a non-root user.

**Problem:**
* Insecure use of `ubuntu:latest` as a base image
* Running commands as the root user