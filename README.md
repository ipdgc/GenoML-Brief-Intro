# GenoML Brief Intro
The briefest intro to our genomics focused automated machine learning pipeline.

## For additional details see...
... its home on [PIP](https://pypi.org/project/genoml/) or its own [website](https://genoml.github.io).

## Three lines for a quick run
#### Install it
```
pip install genoml
```

#### Train it
```
genoml-train   --geno-file=[geno_file] --pheno-file=[pheno_file] 
```
Additional possible options include: 
```
--gwas-file=[file] --cov-file=[file] --herit=[number] --addit-file=[addit]
```
Although "herit" is not recommended if you are in a hurry due to runtime issues

#### Validate it
```
genoml-inference --valid-geno-prefix=[geno_file] --valid-pheno-file=[pheno_file]
```

## Depends on...
...python 3 and pip.

## For questions, comments, requests or collaborations
[Faraz Faghri](faraz.faghri@gmail.com), [Hampton Leonard](hampton.leonard@nih.gov), [Sayed Hadi Hashemi](sayedhadihashemi@gmail.com), [Juan Botia](juanbotiablaya@gmail.com), and [Mike Nalls](mike@datatecnica.com)
