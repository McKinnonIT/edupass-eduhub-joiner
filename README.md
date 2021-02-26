## eduPass & eduHub Joiner
Joins eduPass export data from the [eduSTAR MC](https://apps.edustar.vic.edu.au/edustarmc/student_passwords) (eg. login) with eduHub Student export (XXXX_8125.csv)
This allows us to map the eduPass login with CASES codes.

Only supports ACTV & LVNG students.

### Usage
```❯ python3 joiner.py --help
usage: joiner.py [-h] --eduhub EDUHUB --edupass EDUPASS --out OUT

optional arguments:
  -h, --help            show this help message and exit
  --eduhub EDUHUB, --eduhub-student-file EDUHUB
                        eduHub Student File (ST_XXXX.csv)
  --edupass EDUPASS, --edupass-student-export EDUPASS
                        eduPass Student Export from the EduSTAR MC (https://apps.edustar.vic.edu.au/edustarmc/student_passwords)
  --out OUT, --out-file OUT
                        Output file name or path
```

### Example
`python3 joiner.py --eduhub ST_8125.csv --edupass 8125_students.csv --out-file passhub.csv`
