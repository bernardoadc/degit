1) run

action = bootstrap
type = shell/other
cmd = git init etc/node bootstrap.js/
args?

[
    {
        "action": "shell",
        "shell": "git init"
    },
    {
        "action": "shell",
        "shell": "npm init -y"
    },
    {
        "action": "shell",
        "shell": "npm install --save-dev eslint ..."
    },
      {
      "action": "script/run/node",
      "script": "bootstrap.js",
      "args": ""
  }
]

2) confirm
exibe script interno e pede confirmaçao

3) specify
degit xxx --scripts "rename,xxx" --dont-confirm

@opensas neat names, but unfortunately they're both taken..
--scripts "rename,xxx"
--dont-confirm

4) se é do tipo node, tem q ver se tem node. se é python, etc.. shell, ok, batch nao tanto