# Week 3: Linux Find Command Lab

## Date Completed
January 17, 2026

## Objectives
- Master basic find command syntax
- Use wildcards for pattern matching
- Search by file size
- Search by modification time
- Combine multiple search criteria

## Key Commands Learned

### Find by Name
- `find . -name "filename"` - Case-sensitive exact match
- `find . -iname "filename"` - Case-insensitive match
- `find . -name "*.ext"` - Wildcard pattern matching

### Find by Size
- `find . -size +100c` - Files larger than 100 bytes
- `find . -size -100c` - Files smaller than 100 bytes
- `find . -size 0c` - Empty files

### Find by Time
- `find . -mmin -60` - Modified in last 60 minutes
- `find . -mtime -1` - Modified in last day
- `find . -mtime +30` - Modified more than 30 days ago

### Combine Criteria
- `find . -name "*.log" -size +1000c -ls` - Multiple conditions together
- `find . -type f -name "*.conf"` - File type + name pattern

### Useful Options
- `-ls` - Show detailed info (like ls -l)
- `-type f` - Files only
- `-type d` - Directories only

## Real-World Applications
1. **Finding configuration files** - Locate all .conf files across system directories
2. **Disk space management** - Identify large files consuming storage
3. **Log rotation** - Find old log files for archival/deletion
4. **File organization** - Search for files by naming patterns

## Lab Results
Successfully practiced all find command variations including:
- Case-sensitive and case-insensitive searches
- Wildcard pattern matching with * 
- Size-based file searches (bytes, KB, MB)
- Time-based searches (minutes and days)
- Combined multiple search criteria for complex queries

## Key Takeaways
- `-name` is case-sensitive, `-iname` is case-insensitive
- Size suffixes: `c`=bytes, `k`=KB, `M`=MB, `G`=GB
- Time options: `-mmin` for minutes, `-mtime` for days
- `-ls` flag provides detailed output similar to ls -l
- Multiple criteria can be combined in single find command
- Find is essential for navigating large file systems efficiently

## Next Steps
Continue to Week 4 of Zero To Linux course and practice find command regularly in daily Linux work.
