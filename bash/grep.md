# Grep

`grep` is an extremely useful command to get comfortable with that will make your life a lot easier. 


Here are some grep snippets that I have used:

-----

Show 3 lines before and 2 lines after `foo`

```bash
grep -B 3 -A 2 foo README.txt
```
-----
Search all files that start with for a word:
```bash
echo file_starts_with* | xargs -d' ' -I{} zgrep "value" {}
```

or simpler:

```bash
zgrep "thing" file_starts_with*
```

----
Search multiple files for `magic`:
```bash
grep "magic" file1.txt file2.txt
```

___
Search for lines with `magic` and `potter`:
```bash
grep "magic" file1.txt | grep "potter"
```
