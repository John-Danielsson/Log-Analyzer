# Log-Analyzer
Log analyzer for SIEM.

## Example bash commands to run

```
# Basic
python log_analyzer.py example.log
python3 log_analyzer.py example.log

# Filter by keyword and show top 5
python log_analyzer.py example.log --keyword "User" --ignore-case --top 5
python3 log_analyzer.py example.log --keyword "User" --ignore-case --top 5

# Filter by level (WARN will also match WARNING)
python log_analyzer.py example.log --level WARN
python3 log_analyzer.py example.log --level WARN

# Count IPs too, save report to a file
python log_analyzer.py example.log --ips --out reports/summary.txt
python3 log_analyzer.py example.log --ips --out reports/summary.txt

# Multiple files
python log_analyzer.py logs/app1.log logs/app2.log --ips --top 20
python3 log_analyzer.py logs/app1.log logs/app2.log --ips --top 20
```
