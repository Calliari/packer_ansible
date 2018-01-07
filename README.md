# packer_ansible_terraform


Instructions

Install packer on MAC
```
brew install packer

```

replace the "********" with the AWS credentials

`web-server.json` and `db-server.json`

"aws_access_key": "********",
"aws_secret_key": "**********",


change directory to "packer_projects/packer" run;
```
packer build web-server.json # for the web-server
packer build db-server.json # for the db-server
```

The images will be built based on the the ansible playbook `db_provision.yml` and `web_provision.yml"`
