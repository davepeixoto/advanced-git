# Commands #
- git flow init
- git flow feature start name
- git flow featuer finish name
- git flow release start 0.1.0 **version**
- git flow release finish 0.1.0 **version**

# signatures #
- GPG Gnu Privacy Guide
- gpg --list-secret-key --keyid-form LONG
- gpg --full-generate-key
    1
    4096
    1y
    name
    email
    o
- gpg --armor --export id
- git config --global user.signingkey id
- export GPG_TTY=$(tty)
- git config commit.gpgsign true **for each repository**
- git config --global commit.gpgsign true **as default**
- git config tag.gpgsign true **for each repository**
- git config --global tag.gpgsign true **as default**
- git log --show-signature -1
- vim ~/.gnupg/gpg.conf
- gpgconf --launch gpg-agent
- gpg --edit-key id
- adduid
- uid 2
- trust
- save

# SEMVER #
MAJOR version when you make incompatible API changes,
MINOR version when you add functionality in a backwards compatible manner, and
PATCH version when you make backwards compatible bug fixes.

https://semver.org/lang/pt-BR/

# Conventional Commits #
https://www.conventionalcommits.org/pt-br/v1.0.0/

# Commitlint #
https://commitlint.js.org/#/


# Commitsar #
https://commitsar.aevea.ee/usage/docker/
docker run --rm --name="commitsar" -w /src -v "$(pwd)":/src aevea/commitsar commitsar . 

# Commitzen #
https://commitizen-tools.github.io/commitizen/
https://github.com/commitizen/cz-cli
    
    npm install -g commitizen
    commitizen init cz-conventional-changelog --save-dev --save-exact
    git cz




