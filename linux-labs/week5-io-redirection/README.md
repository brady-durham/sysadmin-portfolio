# Week 5 Lab: Input/Output Redirection

## Scenario
Junior sysadmin at DataFlow Technologies analyzing system logs from overnight issues.

## Skills Practiced

### Output Redirection
- `>` - Redirect stdout to file (overwrites)
- `>>` - Append stdout to file
- `2>` - Redirect stderr to file

### Piping
- `|` - Send output of one command to another
- Chained multiple commands together

### Practical Applications
- Extracted ERROR and WARNING messages from logs
- Counted specific message types
- Created executive summary report
- Separated normal output from errors

## Commands Used
- grep (search text patterns)
- cat (display file contents)
- wc -l (count lines)
- sort (alphabetically order)
- echo (print text)

## Files Created
- reports/errors.txt - ERROR and WARNING messages
- reports/warning_count.txt - Count of warnings
- reports/critical_sorted.txt - Sorted critical messages
- reports/executive_summary.txt - Professional report for management

## Date Completed
February 1, 2026

## Real-World Application
As a sysadmin, I would use these skills daily to:
- Analyze log files for issues
- Create reports for management
- Filter large amounts of data
- Automate data processing tasks
