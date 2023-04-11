# rHFA
Home field advantage (hfa) analysis of local adaptation in crop populations. Input should be breeding variety trials (ex. multi environment trials)

Largely works on R 4.1, though not compiled (yet... very much in progress!). For now, you'll have to source(). 

Brief how-to:

1. id_home() to identify home site (optional)
2. permute_hfa() to run hfa analysis. This will work at the population and genotype level and may work across years (for populations).
You'll need to manually calculate p-values for genotypes from the permutations (first column is observed; try .two-tailed()). If really slow, try setting BLUP=FALSE. 
3. temporal_hfa() for calculationg hfa across years at the population level. 

All functions are relatively documented in source code. See also [analysis code](https://github.com/Alice-MacQueen/cdbn-home-away) for:

  MacQueen, Alice H., et al. "Local to continental‐scale variation in fitness and heritability in common bean." Crop Science 62.2 (2022): 767-779. [[Link]](https://acsess.onlinelibrary.wiley.com/doi/full/10.1002/csc2.20694)
  
And, of course, message with questions. 
