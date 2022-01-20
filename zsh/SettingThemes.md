#Setting Themes
A shell that has a wide range of customization abilities is zsh. The package that we will be using is oh-my-zsh
#Installing zsh
brew install zsh
zsh --version
chsh -s /usr/local/bin/zsh
echo $SHELL # make sure this outputs zsh


#oh-my-zsh Package
Working in the terminal allows you to use some custom themes through the use of the package: oh-my-zsh
Oh-my-zsh Website: https://ohmyz.sh/#install
oh-my-zsh Github Website: https://github.com/ohmyzsh/ohmyzsh/wiki

The basic instructions for installing oh-my-zsh are:
- make sure your default shell is zsh 
- if it is not then use steps listed in Installing zsh to do so.
- use command sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
- it will automatically install oh-my-zsh and create a .zshrc file.

can change themes by looking inside of the .zshrc file and changing ZSH_THEME='ThemeToBeUsed'

#Installing Fonts

In order to have the more fancy themes to work, custom fonts are needed to be installed. 
Steps are taken from https://github.com/powerline/fonts

If on Linux (Debian or Ubuntu based): sudo apt-get install fonts-powerline

If on other linux environment, check the wiki

On other environments:
# clone
git clone https://github.com/powerline/fonts.git --depth=1
# install
cd fonts
./install.sh
# clean-up a bit
cd ..
rm -rf fonts

Once Powerline fonts are installed, open the terminal application and change the default font to something like Meslo LG S DZ for Powerline.

After the powerline font is set to default, the theme should render properly.  
