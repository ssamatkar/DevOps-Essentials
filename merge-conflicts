
# Git Merge Conflict Resolution

## 1. Initialize a New Git Repository:

```bash
mkdir merge-conflict-demo
cd merge-conflict-demo
git init .
```

## 2. Create a Sample File:

```bash
echo "Line 1" > example.txt
echo "Line 2" >> example.txt
echo "Line 3" >> example.txt
```

## 3. Commit this file to the main branch:

```bash
git add example.txt
git commit -m "Initial commit with example.txt"
```

## 4. Create a New Branch and Make Changes:

```bash
git checkout -b feature-branch

echo "Line 4 from feature-branch" >> example.txt
git add example.txt
git commit -m "Added line 4 in feature-branch"
```

## 5. Switch Back to main Branch:

```bash
git checkout main
```

## 6. Modify the Same File in main:

```bash
echo "Line 4 from main" >> example.txt
git add example.txt
git commit -m "Added line 4 in main"
```

## 7. Attempt to Merge `feature-branch` into `main`:

```bash
git merge feature-branch
```

## 8. Git will output a message indicating there is a conflict:

```plaintext
Auto-merging example.txt
CONFLICT (content): Merge conflict in example.txt
Automatic merge failed; fix conflicts and then commit the result.
```

## 9. Open `example.txt` to see the conflict markers:

```plaintext
Line 1
Line 2
Line 3
Line 4 from feature-branch
```

## 10. Edit the file to resolve the conflict. Choose which lines to keep or combine them:

```plaintext
Line 1
Line 2
Line 3
Line 4 (merged from both branches)
```

## 11. Add and commit the resolved file:

```bash
git add example.txt
git commit -m "Resolved merge conflict between main and feature-branch"
```

## 12. Once everything is resolved and merged, you can delete the `feature-branch` locally:

```bash
git branch -d feature-branch
```
```
