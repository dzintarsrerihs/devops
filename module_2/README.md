# devops

## module_1 un module_2 attelu failu salīdzinājums

Pašiem failiem hash neatškiras. Atškiras komita hash.
> PS C:\lukursi\devops> git ls-files -s
- 100644 b9fa884f0b5d494a29a729861e5478095afb84b5 0       README.md
- 100644 007ad7b4e200383e2ae117fbf4e3d66640b41bd2 0       module_1/README.md
- 100644 5802fe3e4bcb4d484967c2abf1696254e60c1290 0       module_1/git.png
- 100644 6260185d252485eb1719f1770f992830db716163 0       module_1/php-helloworld.png
- 100644 5802fe3e4bcb4d484967c2abf1696254e60c1290 0       module_2/git.png
- 100644 6260185d252485eb1719f1770f992830db716163 0       module_2/php-helloworld.png

## [Terraform](https://github.com/hashicorp/terraform)

Divi veidi kā pārskatīt konkrēta perioda vēsturi. Principā atškiras tikai parametru nosaukums:

16. Pārbaudīt kādas izmaiņas tika veiktas iepriekšējās nedēļas laikā. Atrast vismaz divus veidus kā to izdarīt.  -__Jā ir veiktas izmaiņas.__
> C:\lukursi\terraform>git log --since="2022-04-18" --until="2022-04-245"

> C:\lukursi\terraform>git log --after="2022-04-18" --before="2022-04-25"

17. Atrast commit kurus veica autors - “Laura Pacilio”

> git log --author="Laura Pacilio"

18. Atrast vai Laura ir veikusi commit pagājušā gada septembrī? -__Jā ir__
> git log --author="Laura Pacilio" --since="2021-09-01" --until="2021-10-01"

> commit 8f09e27597c9e792d7d9acea158429f10269572d
Merge: 5386d6c5b c8e2be76d
Author: Laura Pacilio <83350965+laurapacilio@users.noreply.github.com>
Date:   Mon Sep 20 17:24:31 2021 -0400

19. Vai Laura ir veikusi commit vakar (25.04.2022? -__Nē. Pēdējais komits ir veikts 20. aprīlī 2022. gadā__

> git log --author="Laura Pacilio" --since="2022-04-26" --until="2022-04-26"
