 # Project Workspace and Permission Management

This task demonstrates directory creation, file management, permission control, and ownership verification in Linux.

## Commands Used

### 1. Check Default Umask

```bash
umask
```

**Output**

```text
0002
```

Displays the default permission mask used when creating new files and directories.

---

### 2. Create Project Structure

```bash
mkdir -p project_workspace/docs project_workspace/code
```

Creates the project workspace with separate directories for documentation and source code.

---

### 3. Create Documentation File

```bash
touch project_workspace/docs/design.txt
```

Creates an empty documentation file inside the docs directory.

---

### 4. Verify File Permissions

```bash
ls -l project_workspace/docs/design.txt
```

**Output**

```text
-rw-rw-r-- 1 vishaan vishaan ...
```

Shows that the file was created with permissions based on the current umask value.

---

### 5. Secure the Code Directory

```bash
chmod 700 project_workspace/code
```

Grants full access to the owner while denying access to group members and others.

---

### 6. Verify Ownership

```bash
chown $USER:$USER project_workspace/docs/design.txt
```

Ensures the file ownership belongs to the current user and group.

---

## Conclusion

The project workspace was successfully created. File permissions, ownership, and directory security were configured according to Linux permission management principles.
