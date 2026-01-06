# Log-Analyzer
Log analyzer for SIEM.

## Example bash commands to run

```
# Basic
python log_analyzer.py sample.log

# Filter by keyword and show top 5
python log_analyzer.py sample.log --keyword "User" --ignore-case --top 5

# Filter by level (WARN will also match WARNING)
python log_analyzer.py sample.log --level WARN

# Count IPs too, save report to a file
python log_analyzer.py sample.log --ips --out reports/summary.txt

# Multiple files
python log_analyzer.py logs/app1.log logs/app2.log --ips --top 20
```
