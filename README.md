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

## How to

### Start the development server

```
# Inside /benbankes.com
hugo serve
```

### Create a new page

```
# Inside /benbankes.com
hugo new posts/my-first-post.md
```

This will create a new markdown file under the posts folder, based on the `default.md` template/archetype

### Deploy

```
# Inside /benbankes.com
hugo && ./deploy.sh "Your optional commit message"
# Inside /pencilinthehand.com
rm -Rf public && hugo && npx netlify-cli deploy --prod
```

## Notes

- I think I should have run `git submodule add` for benbankes.com from the root folder.  Maybe I will get around to changing that.
- pencilinthehand.com uses the "go modules" way of adding a theme.  This seems best.
- I might want to eventually split sites and the hugo install into separate repositories.
