# cop_ansible

### Requirements
1. credentials.yml file like:
    ```
    auth_url: http://AUTH_URL:15000/v3/
    username: USER
    password: PASSS
    tenant_name: TENANT
    user_domain_name: DOMAIN
    project_id: XXXXXXXXXXXXXXXXXXX
    ```
2. testkeypair.pem file created and stored in openstack keypairs

## USE

For deploy use: 
```
ansible-playbook cop.yml -e 'deploy_action=DEPLOY'
```
For destroy use: 
```
ansible-playbook cop.yml -e 'deploy_action=DESTROY'
```