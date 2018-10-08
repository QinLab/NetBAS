# NetBAS
Both Human and Yeast PIN are used.
R mark down examples (/MarkDown) include:

Examples: using 50 permutations from yeast PIN.
  
1. yeast.bp.matrix.Rmd
This script calculate the frequencies between each pair of BP terms from the yeast PIN (the original BioGrid PIN)
The heatmap was plotted agains log10(freq+1) (the frequencies vary from 0 to > 7000).

2. yeast.ms02.bp.matrix.Rmd
This script do the same calculations as for 1, for permutations. 50 permutations are used here.
All results are saved in the directory "/ms02.yeast/bp-bp/"

3. yeast.bp.z.heatmap.Rmd
This script calculate the Z-scores for each BP term, resulting in a n*n matrix, where n is the total number of BP terms.
Heatmap is plotted based on this matrix, positive Z-scores are in red, and negative Z-scores are in blue, respectively.

4. yeast.cm15.bp.matrix.Rmd
This script calculate the BP terms from proteins that interact with the CM15 set (225 genes).
The result is a spectrum-like, 1D array.

5. yeast.cm15.ms02.bp.matrix.Rmd
This script do the same calculations as for 4, for permutations. 50 permutations are used here.
All results are saved in the directory "/ms02.yeast/cm15/"

6. yeast.cm15.bp.z.heatmap.Rmd
This script calculate z-scores of BP terms from CM15 set.
The enriched (Z > 3) and suppressed (Z < -3) BP terms are recorded in the files yeast.cm15.bp.enriched.csv and yeast.cm15.bp.suppressed.csv, respectively.
The top 10 enriched BP terms are plotted as heatmap.
