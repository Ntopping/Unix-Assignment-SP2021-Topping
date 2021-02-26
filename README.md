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
$head -n 1 fang_et_al_genotypes.txt
Sample_ID	JG_OTU	Group	abph1.20	abph1.22	ae1.3	ae1.4	ae1.5	an1.4	ba1.6	ba1.9	bt2.5	bt2.7	bt2.8	Fea2.1	Fea2.5	id1.3	lg2.11	lg2.2	pbf1.1	pbf1.2	pbf1.3	pbf1.5	pbf1.6	pbf1.7	pbf1.8	PZA00003.11	PZA00004.2	PZA00005.8	PZA00005.9..... etc.
$ awk -F "\t" '{print NF; exit}' fang_et_al_genotypes.txt
986
$ tail -n +6 fang_et_al_genotypes.txt | awk -F "\t" '{print NF; exit}'
986
```
By inspecting this file I learned that:
1. This file has 2783 lines, 2744038 words, and 11051939 bytes
2. The size of the data file is 11M
4. There is also a header in the data
5. There are 986 columns in the dataset

###Attributes of `snp_position.txt`

# Data Inspection
```
$ wc snp_position.txt
  984 13198 82763 snp_position.txt
$ du -h snp_position.txt
  38K	snp_position.txt
$ head -n 1 snp_position.txt
SNP_ID	cdv_marker_id	Chromosome	Position	alt_pos	mult_positions	amplicon	cdv_map_feature.name	gene	candidate/random	Genaissance_daa_id	Sequenom_daa_id	count_amplicons	count_cmf	count_gen
$ awk -F "\t" '{print NF; exit}' snp_position.txt
15
$ tail -n +6 snp_position.txt | awk -F "\t" '{print NF; exit}'
15


  By inspecting this file i learned that:
  1. This file has 084 lines, 13198 words and 82763 bytes
  2. The size of this file is 38K
  3. There is a header in this dat set
  4. There are 15 columns in this data set
