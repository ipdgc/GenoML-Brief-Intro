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
--gwas-file=[file] --cov-file=[file] --herit=[number] --addit-file=[addit] --n-cores=[number]
```
Although "herit" is not recommended if you are in a hurry due to runtime issues

#### Validate it
```
genoml-inference --valid-geno-prefix=[geno_file] --valid-pheno-file=[pheno_file] --valid-dir=[file]
```

## Depends on...
...python 3.6, R > 3.5.0 or later and pip.

## Example using data from this repository
```
pip install genoml
genoml-train --geno-prefix=./exampleData/training --pheno-file=./exampleData/training.pheno --model-file=./testTrain.zip --addit=./exampleData/training.addit --n-cores=2
genoml-inference --model-file=./testTrain.zip --valid-dir=./testValidate --valid-geno-prefix=./exampleData/validation --valid-pheno-file=./exampleData/validation.pheno --valid-addit-file=./exampleData/validation.addit
```

## For questions, comments, requests or collaborations
[Faraz Faghri](faraz.faghri@gmail.com), [Hampton Leonard](hampton.leonard@nih.gov), [Sayed Hadi Hashemi](sayedhadihashemi@gmail.com), [Juan Botia](juanbotiablaya@gmail.com), and [Mike Nalls](mike@datatecnica.com)
