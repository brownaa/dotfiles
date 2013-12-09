# Make sure we’re using the latest Homebrew
update

# Upgrade any already-installed formulae
upgrade

# Get git
install git

# Install GNU core utilities (those that come with OS X are outdated)
install coreutils
echo "Don’t forget to add $(brew --prefix coreutils)/libexec/gnubin to \$PATH."
# Install GNU `find`, `locate`, `updatedb`, and `xargs`, g-prefixed
install findutils
# Install Bash 4
install bash

# Install wget with IRI support
install wget --enable-iri

# Tap dupes and science
tap homebrew/dupes
tap homebrew/science

# Install everything else
install the_silver_searcher
install unrar
install ssh-copy-id
install tree

# Install boost, eigen, cmake
install boost --c++11
install cmake
install eigen

# Remove outdated versions from the cellar
cleanup
