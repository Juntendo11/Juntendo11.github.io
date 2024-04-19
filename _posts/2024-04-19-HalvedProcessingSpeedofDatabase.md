# Comparing against the entire Database

Comparing an template against an entire databse found to be time consuming, and often taking two minutes or more.
This was due to repeatedly processing the template over database over and over for same template.
This was mitigated by first processing the template, and using those values for comparison against the databse.
This cut the processing time by half :D

```
f1, m1, ls1 = Analyze_fingerprint(self.myDBdest)
```

```
score comp_fin(fin1, fin2):
```
Changed to
```
score = comp_template(f, f1, m1, ls1)
```
