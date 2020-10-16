## Installation Steps

### For macOS

### Method 1: Installing GitHub Desktop

GitHub Desktop simplifies the development workflow with a UI. It will install Git if your system doesn't already have it.

1. Download GitHub desktop from https://desktop.github.com/
2. Follow the instructions in the installation window. You'll need a GitHub account.
3. Once installed, check yout Git version with:
```
git --version
```

### Method 2: Using Xcode

Apple ships Git as part of their Xcode commmand-line tools.

1. Open **Terminal** and run the following command:
```
xcode-select —install
```
2. A new window will pop-up asking you if you want to install Xcode command line developer tools, select yes
3. Once the installation finishes, you can check your Git version in Terminal with:
```
git --version
```

### Method 3: Using Homebew

Homebew is a popular method for downloading software

1. Open **Terminal**
2. Run the following command:
```
brew install git
```
3. If you dont have brew already installed, you can install it with this command:
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```
4. Once Brew is installed and you run step 2, check your Git version with:
```
git --version
```
