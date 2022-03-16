# [インストール方法](https://github.com/pyenv/pyenv#installation)

## [Ubuntu/Debian (bash)](https://github.com/pyenv/pyenv#basic-github-checkout)

1. [事前準備](https://github.com/pyenv/pyenv/wiki#suggested-build-environment)として、次のコマンドをターミナルで実行

```shell
sudo apt update
sudo apt install make build-essential libssl-dev zlib1g-dev \
libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm \
libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
```

2. pyenvのリポジトリをクローン

```shell
git clone https://github.com/pyenv/pyenv.git ~/.pyenv
```

3. （Option）適用するrelease version（例：v2.2.3）にリポジトリを変更

```shell
cd ~/.pyenv
git checkout v2.2.3
```

4. 次のコマンドを実行し、`pyenv`コマンドのパスを通す

```shell
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(pyenv init --path)"' >> ~/.bashrc
source ~/.bashrc
```

5. ターミナルで`pyenv`コマンドが実行できれば、インストール完了

```code
pyenv 2.2.3
Usage: pyenv <command> [<args>]

Some useful pyenv commands are:
   --version   Display the version of pyenv
   commands    List all available pyenv commands
   exec        Run an executable with the selected Python version
   global      Set or show the global Python version(s)
   help        Display help for a command
   hooks       List hook scripts for a given pyenv command
   init        Configure the shell environment for pyenv
   install     Install a Python version using python-build
   local       Set or show the local application-specific Python version(s)
   prefix      Display prefix for a Python version
   rehash      Rehash pyenv shims (run this after installing executables)
   root        Display the root directory where versions and shims are kept
   shell       Set or show the shell-specific Python version
   shims       List existing pyenv shims
   uninstall   Uninstall a specific Python version
   version     Show the current Python version(s) and its origin
   version-file   Detect the file that sets the current pyenv version
   version-name   Show the current Python version
   version-origin   Explain how the current Python version is set
   versions    List all Python versions available to pyenv
   whence      List all Python versions that contain the given executable
   which       Display the full path to an executable

See `pyenv help <command>' for information on a specific command.
For full documentation, see: https://github.com/pyenv/pyenv#readme
```

## [Windows](https://github.com/pyenv/pyenv#windows)

非対応
