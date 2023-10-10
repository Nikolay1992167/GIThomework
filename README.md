# Description of creating a structure git flow
* The project will figuratively describe an example of home renovation.
* $ git init. Files created house.txt.
* $ git add . - I use this command everywhere because of the simplicity of the content.
* $ git commit -m "feat: start of home renovation" 
* $ git tag "v.0.1" - assign tag.
* $ git checkout -b develop - create new branch 'develop'
* Add line '1. We are repairing the roof.' in house.txt.
* $ git add .
* $ git commit -m "feat: task to repair the roof"
* Add line '2. We are repairing the walls.' in house.txt.
* $ git add .
* $ git commit -m "feat: task to repair the walls"
* Add line '3. Yard landscaping.' in house.txt.
* $ git add .
* $ git commit -m "feat: task of landscaping the yard"
* $ git checkout -b feature/garden
* Create garden.txt and add line '1. Plant fruit trees.'
* $ git add .
* $ git commit -m "feat: task to plant fruit trees"
* Add line '2. Plant berry bushes.' in garden.txt
* $ git add .
* $ git commit -m "feat: task to plant berry bushes"
* Add line '3. Plant strawberries.' in garden.txt
* $ git add .
* $ git commit -m "feat: task to plant strawberries"
* Add line '4. Plant raspberries.' in garden.txt
* $ git add .
* $ git commit -m "feat: task to plant raspberries"
* Select branch 'develop' 
* $ git checkout develop
* $ git checkout -b feature/pool - create new branch 'feature/poll'
* File created pool.txt and added line '1. Install a swimming pool.'
* $ git add .
* $ git commit -m "feat: task to install a swimming pool" 
* Add line '2. Install an umbrella.' in pool.txt.
* $ git add .
* $ git commit -m "feat: task to install an umbrella"
* Add line '3. Install sunloungers.' in pool.txt.
* $ git add .
* $ git commit -m "feat: task to install sunloungers"
* Select branch 'develop'
* $ git checkout develop 
* Add line '4. We are repairing the floor.' in house.txt.
* $ git add .
* $ git commit -m "feat: task to repair the floor"
* Select a branch 'master'
* $ git checkout master
* $ git checkout -b hotfixes - create new branch 'hotfixes'
* Add line 'We bought a house and will be renovating it.' in house.txt
* $ git add .
* $ git commit -m "fix: severe bug fixed for production"
* Select branch 'master'
* $ git checkout master
* Merge branch 'hotfixes' into branch 'master'
* $ git merge --no-ff hotfixes and add commit message "Merge branch 'hotfixes' into 'master'"
* $ git tag "v.0.2" - assign tag.
* Select branch 'develop'
* $ git checkout develop
* Merge branch 'hotfixes' into branch 'develop'
* $ git merge --no-ff hotfixes and eliminate the conflict in house.txt
* $ git add .
* $ git commit -m "Merge branch 'hotfixes' into 'develop'"
* $ git branch -d hotfixes - delete branch 'hotfixes'
* Merge branch 'feature/pool' into branch 'develop'
* $ git merge --no-ff feature/pool and add commit message "Merge branch 'feature/pool' into 'develop'
* $ git branch -d feature/pool - delete branch 'feature/pool'
* $ git checkout -b release - create new branch 'release' 
* File created address.txt and add line 'Republic of Belarus'
* $ git add .
* $ git commit -m "feat: add address"
* Add line 'Mozyr, Geologov street, 15' in address.txt
* $ git add .
* $ git commit -m "fix: updated address"
* Select branch develop
* $ git checkout develop
* Merge branch 'release' into branch 'develop'
* $ git merge --no-ff release add commit message "Merge branch 'release' into 'develop'"
* $ git checkout -b feature/pool - create branch 'feature/pool'
* Add line '4. Install a descent into the pool.' in pool.txt.
* $ git add .
* $ git commit -m "feat: task to install a descent into the pool"
* Add line '5. Place air mattresses and circles.' in pool.txt.
* $ git add .
* $ git commit -m "feat: task to place air mattresses and circles"
* Add line '6. Place a bar.'
* $ git add .
* git commit -m "feat: task to place a bar."
* Select branch 'release'
* $ git checkout release
* Add line 'Postcode: 247795' in address.txt.
* $ git add .
* $ git commit -m "fix: fixed address add postcode"
* Add line 'Gomel region' in address.txt.
* $ git add .
* $ git commit -m "fix: fixed address add region'
* Select branch 'master'
* $ git checkout master
* Merge branch 'release' into branch 'master'
* $ git merge --no-ff release and add commit message "Merge branch 'release' into 'master'"
* $ git tag "v.1.0" - assign tag.
* Select branch 'develop'
* $ git checkout develop
* Merge branch 'release' into branch 'develop'
* $ git merge --no-ff release and add commit message "Merge branch 'release' into 'develop'"
* $ git branch -d release - delete branch 'release'
* Merge branches 'feature/garden' and 'feature/pool' into branch 'develop'
* $ git merge --no-ff feature/garden feature/pool and add commit message "Merge branches 'feature/garden' and 'feature/pool' into 'develop'"
* $ git branch -d feature/garden - delete branch 'feature/garden'
* $ git branch -d feature/pool - delete branch 'feature/pool'
* $ git checkout -b release - create branch 'release'
* Add file README.md
* $ git add .
* $ git commit -m "docs: add README.md"
* Select branch 'master'
* $ git checkout master
* Merge branch 'release' into branch 'master'
* $ git merge --no-ff release and add commit message "Merge branch 'release' into 'master'
* Select branch 'develop'
* $ git checkout develop
* Merge branch 'release' into branch 'develop'
* $ git merge --no-ff release and add commit message "Merge branch 'release' into 'develop'"
* $ git branch -d release