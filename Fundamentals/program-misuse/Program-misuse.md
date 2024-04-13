# Program Misuse Challenge: Reading root owned flag

In this challenge, participants will navigate to the `/challenge` directory and execute the `babysuid` program. This program grants the SUID (Set User ID) bit on various commands, presenting an opportunity for users to escalate privileges and gain unauthorized access. The objective is to retrieve a flag owned by the root user.

## Instructions

1. Navigate to the `/challenge` directory:
    ```bash
    cd /challenge
    ```

2. Execute the `babysuid` program:
    ```bash
    ./babysuid
    ```

3. Exploit the SUID permissions granted by `babysuid` to execute commands as the root user and locate the flag.

**Note:** Exercise caution while participating in this challenge, as it involves potentially risky actions that could compromise system integrity or security.
