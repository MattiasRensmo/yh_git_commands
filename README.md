# Gitkommandon

## Länkar till mer läsning

- [Alla git-komandon som finns](https://git-scm.com/docs/git#_git_commands)
- [De mest använda komandon](https://git-scm.com/docs)

## Vanliga arbetsflöden

### Använda terminalen

**Se till att du alltid är i rätt mapp innan du börjar använda git!**

`dir` Visar alla filer och mappar i nuvarnade mapp

`cd [mappnamn]` Gå till undermapp som heter \[mappnamn\]

`cd ..` Gå till överordnad mapp

---

### Create repositories

`git clone [url]` Hämtar lådan från länken och lägger i en undermapp

`cd [mappnamn]` Gå in i mappen du precis laddade ner

### Ladda ner ändringar

`git pull` Ladda ner ändringar från GitHub till din dator. Viktigt när det är flera som jobbar med samma kod.

### Spara ändringar till Github

`git add .` Lägger till alla filer i lådan

`git commit -m "[message]"` Ställer lådan i arkivet

`git push` Skickar lådan till GitHub

### Branches

#### Lista branches

`git branch -a` Listar alla branches

#### Skapa och byt mellan branches

`git checkout -b [branch name]` Skapa en ny branch och byt till den

`git checkout [branch name]` Byt till [branch name]

#### Samanfoga branches

1.  Byt till branchen du vill samanfoga in till
2.  `git merge [branch]` Ange branchen du vill lägg in i branchen du står i

---

## De vanligaste komandona

### Create repositories

`git init`

Turn an existing directory into a git repository

`git remote add origin [url]`

After using the git init command, link the local repository to an empty GitHub repository. Specifies the remote repository for your local repository. The url points to a repository on GitHub.

`git clone [url]`

Clone (download) a repository that already exists on GitHub, including all of the files, branches, and commits

### Make changes

`git add [file/.]`

Snapshots the file in preparation for versioning. Period (.) means all

`git commit -m "[message]"`

Records file snapshots permanently in version history

### Synchronize changes

`git fetch`

Downloads all history from the remote tracking branches

`git merge`

Combines remote tracking branches into current local branch

`git push`

Uploads all local branch commits to GitHub

`git pull`

Updates your current local working branch with all new commits from the corresponding remote branch on GitHub. git pull is a combination of `git fetch` and `git merge`
