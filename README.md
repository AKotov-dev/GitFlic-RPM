# GitFlic-RPM
`python3-gitflic` - python library to use the GitFlic API v3 + `gitswitch` - a tool for transferring repositories from GitHub to GitFlic rpm packages for Mageia-8/9.

**Installation:** The package `python3-gitflic` is installed first, then `gitswitch`.
```
> gitswitch --help

Options:
--gf_token TEXT        Your GitFlic token.  [required]
--gh_token TEXT        Your GitHub token.  [required]
--clone_folder PATH    Directory where to download repositories.
--apply_private        Need to copy private repositories?
--apply_organisations  Need to copy organisations repositories?
--use_ssh              Use SSH mode to upload repositories.
--help                 Show this message and exit.
```
Get GitHub token from: https://github.com/settings/tokens  
Get GitFlic token from: https://gitflic.ru/settings/oauth/token  
  
If you are using 2AF into GitFlic select ssh connection using the key: `--use_ssh`  
  
The script will copy all the necessary repositories to `./cloned-repos/<login>/<repo_name>`, then push it to GitFlic
  
gitflic: https://pypi.org/project/gitflic/  
GitSwitch: https://gitflic.ru/project/dbi471/git-switch
