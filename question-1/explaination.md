# Linux Environment Verification

## Objective

The purpose of this task is to verify the basic Linux environment by checking the current user, user groups, shell, working directory, workspace contents, and network connectivity.

---

## Commands Used

### 1. Verify Current User

```bash
whoami
```

**Output**

```text
vishaan
```

This command displays the username of the currently logged-in user.

---

### 2. Verify User Groups

```bash
groups
```

**Output**

```text
vishaan users
```

This command lists the groups associated with the current user.

---

### 3. Check Current Shell

```bash
echo $SHELL
```

**Output**

```text
/bin/bash
```

This confirms that the Bash shell is being used.

---

### 4. Check Current Working Directory

```bash
pwd
```

**Output**

```text
/home/vishaan
```

This command displays the current working directory.

---

### 5. List Workspace Contents

```bash
ls -la
```

This command lists all files and directories, including hidden files such as `.bashrc`, `.profile`, `.config`, `.cache`, and `.ssh`, along with standard directories like Desktop, Documents, Downloads, Music, Pictures, Projects, Public, Templates, and Videos.

---

### 6. Verify Network Connectivity

```bash
ping -c 4 google.com
```

The successful transmission and reception of all four packets confirms that the system has an active internet connection with **0% packet loss**.

---

## Conclusion

The Linux environment was successfully verified. The current user, user groups, shell, working directory, workspace contents, and internet connectivity were confirmed using standard Linux commands. 
