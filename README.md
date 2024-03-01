# amaris_mlops

Worflow 

# Start with branch master in version 1.0.0
git checkout master
git pull origin master

# Create and switch to a feature branch based on master
git checkout -b feature-1
# Work on feature implementation, commit changes

# Merge feature branch into master and tag as version 1.0.1
git checkout master
git merge feature-1
git tag -a v1.0.1 -m "Release version 1.0.1"
git push origin master --tags

# Create and switch to a develop branch based on master version 1.0.1
git checkout -b develop
# Work on additional features or changes, commit changes

# Merge develop branch into master and tag as version 1.1.0
git checkout master
git merge develop
git tag -a v1.1.0 -m "Release version 1.1.0"
git push origin master --tags

# Checkout version 1.0.1
git checkout v1.0.1

# Create and switch to a feature2 branch based on master version 1.0.1
git checkout -b feature-2

# Work on another feature, commit changes

# Merge feature2 branch into master and tag as version 1.2.0
git checkout master
git merge feature-2
git tag -a v1.2.0 -m "Release version 1.2.0"
git push origin master --tags
