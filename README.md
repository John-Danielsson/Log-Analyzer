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


### Screenshot of terminal showing a basic run
<img width="599" height="208" alt="Screenshot 2026-01-07 at 15 02 56" src="https://github.com/user-attachments/assets/72233a64-33a4-4a36-9bd1-ca8011ea1217" />

### Screenshot of a run with --ips and the resulting “Top IPs” section, saving the report to a file
<img width="808" height="50" alt="Screenshot 2026-01-07 at 15 04 58" src="https://github.com/user-attachments/assets/6a1d4d37-b04b-4e1b-b8bc-795cdba7ae67" />

### Screenshot of the saved report file
<img width="537" height="495" alt="Screenshot 2026-01-07 at 15 05 51" src="https://github.com/user-attachments/assets/025488de-05b0-4189-b216-9702b13af36c" />

