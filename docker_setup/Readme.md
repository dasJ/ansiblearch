# Docker setup

This role installs Docker on the machine, starts it up, and adds users to the Docker group.
If a user does not exist yet, it will be created.

## Variables

### Optional
- `docker_setup_group_members` - An array of users to be added to the docker group (don't forget to log out and back in)
