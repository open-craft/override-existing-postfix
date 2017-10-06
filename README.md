# override-existing-postfix

## Usage

```bash
ansible-playbook -i fq.domain.name, update_passwd.yml --extra-vars="@path_to_vars.yml"
```

## Required variables

```yaml
POSTFIX_QUEUE_HOST: "my.smtp.server"
POSTFIX_QUEUE_USERNAME: "my_username"
POSTFIX_QUEUE_PASSWORD: "my_supersecret_password"
```

## Defaults

```yaml
POSTFIX_QUEUE_PASSWORD_FILE: "/etc/postfix/sasl/passwd"
POSTFIX_PASSWORD_FILE_OWNER: "root"
POSTFIX_PASSWORD_FILE_GROUP: "root"
POSTFIX_QUEUE_PORT: 587
```
