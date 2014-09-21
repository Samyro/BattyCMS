Setup:

#install homebrew
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)”

#install pyenv
brew install pyenv

#install python 2.7.6
pyenv install 2.7.6

#install virtualenv
pyenv global 2.7.6
pip install virtualenv

# clone project from github
cd …/projectfolder


# Create a virtualenv to isolate our package dependencies locally
virtualenv env
source env/bin/activate  # On Windows use `env\Scripts\activate`

# Install Django and Django REST framework into the virtualenv
pip install -r requirements.txt

