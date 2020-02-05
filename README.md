# Ansible Search Container

This role will build a container using Ansible, install multiple search servers, commit the container image and then remove the running container. This is an alternative way of building containers described [here](https://github.com/geerlingguy/ansible-role-docker). This image is meant to be used to easily compare multiple search servers on specific configurations.

Supported search providers:

- [Elasticsearch](https://www.elastic.co/)
- [Redisearch](https://oss.redislabs.com/redisearch/index.html)
- [Searchlight](https://docs.openstack.org/searchlight/latest/)
- [Solr](https://lucene.apache.org/solr/)


## Use

Assumes Docker CE, Ansible and [Docker python](https://github.com/docker/docker-py) installed.

### Build

Within this dir, install remote dependencies with:

    ansible-galaxy install -r requirements.yml

Run the playbook:

    ansible-playbook -i inventory main.yml

### Tests

TK
