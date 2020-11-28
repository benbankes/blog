### Setup

To setup a development environment with ansible, run the ansible playbook.

1. Get ansible if you do not already have it

    ```
    sudo apt update
    sudo apt install ansible
    ```

1. Run the playbook

    ```
    cd ansible
    ansible-playbook setup-development-environment.yml
    ```

### Useful extensions for VSCode

Provide a bulleted list of links here, as extensions arise


### How to create a new page

```
hugo new posts/my-first-post.md
```

This will create a new markdown file under the posts folder, based on the `default.md` template/archetype
