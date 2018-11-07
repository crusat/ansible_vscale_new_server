This ansible playbook create server with docker and docker-compose from your gitlab repository over hosting vscale.io and up it.

## Example structure in repository

    ...
    /deploy/server/docker-compose.yml
    /deploy/server/.env
    /deploy/server/...
    /deploy/...
    ...

## Example run playbook

Example of creating new server on hosting https://vscale.io.

    ansible-playbook -i <path/to/your/inventory/file> ./main.yml

## Troubleshooting

You can disable host key checking. Edit file `/etc/ansible/ansible.cfg` and uncomment next line:

    [defaults]
    host_key_checking = False

