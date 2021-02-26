# Unix Assignment
## Data Inspection

### Attributes of `fang_et_al_genotypes.txt`

# Data Inspection
```
$wc fang_et_al_genotypes.txt`
2783 2744038 11051939 fang_et_al_genotypes.txt
$du -h fang_et_al_genotypes.txt
 11M	fang_et_al_genotypes.txt
$awk -F "\t" '{print NF; exit}' fang_et_al_genotypes.txt
986
```
By inspecting this file I learned that:
1. This file has 2783 lines, 2744038 words, and 11051939 bytes
2. The size of the data file is 11M
3. 
