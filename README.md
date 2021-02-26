# Unix-Assignment-SP2021-Topping
#### Start by creating a data repository on GitHub
#### Navigate to the top right corner of the GitHub webpage and click on "New Repository"
#### Name the repository, make it public, and hit create
#### Copy the link to the repository and open your Unix program (Terminal for me)
#### Make a clone to your local machine
#### `Git Clone https://github.com/Ntopping/Unix-Assignment-SP2021-Topping.git`
#### This will also allow you to access the repository on GitHub from your local machine
#### List all files in the repository
`ls -a`
#### This should be empty
#### Locate the downloaded .txt files for the assignment from the BCB546-Spring2021 repository
#### Move the files into Unix-Assignment-SP2021-Topping.git
`mv "file name" Unix-Assignment-SP2021-Topping`
#### Now, all of the files needed for the assignment are within the repository
# Data Inspection

#### To check the number of lines, words, and bytes respectively run this line of code
```
$wc fang_et_al_genotypes.txt`
2783 2744038 11051939 fang_et_al_genotypes.txt
```
To check the file size, run this line of code
```
du -h fang_et_al_genotypes.txt
 11M	fang_et_al_genotypes.txt
 ```
 To inspect the number of columns, use the awk command
```
awk -F "\t" '{print NF; exit}' fang_et_al_genotypes.txt
986
```
