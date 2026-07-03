 # System and Link Analysis

This task demonstrates the behavior of hard links and symbolic links in Linux.

## Commands Used

### 1. Create Original File

```bash
touch original_file.txt
echo "Hello Linux" > original_file.txt
```

Creates a file and stores sample content.

---

### 2. Create Hard Link

```bash
ln original_file.txt hard_link.txt
```

Creates a hard link pointing directly to the same inode as the original file.

---

### 3. Create Symbolic Link

```bash
ln -s original_file.txt sym_link.txt
```

Creates a symbolic link that references the original file path.

---

### 4. Verify Links

```bash
ls -li original_file.txt hard_link.txt sym_link.txt
```

Shows inode information and link relationships.

---

### 5. Delete Original File

```bash
rm original_file.txt
```

Removes the original file.

---

### 6. Test Link Behavior

```bash
cat hard_link.txt
cat sym_link.txt
```

The hard link continues to work because it shares the same inode. The symbolic link becomes broken because its target file no longer exists.

---

## Conclusion

Hard links remain functional after deletion of the original file, while symbolic links depend on the existence of their target path.
