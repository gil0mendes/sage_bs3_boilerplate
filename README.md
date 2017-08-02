# Sage BS3 Boilerplate

WordPress boilerplate with modern development tools, easier configuration, and an improved folder structure.

**Includes:**
- Wordpress 4.8
- Composer
- Sage 9 Beta 3
- Bootstrap 3
- Docker compose file
- Advanced Custom Fields

**Requires:**
- Docker
- PHP + Composer
- Node
- Yarn

## Development

The following commands are used during the development process and deploy. First of all, it's necessary create a `.env` file based on the `.env.example` and copy the ACF key to there.

```bash
# Run a docker instance
$ docker-compose up

# Install composer dependencies
$ composer install

# Install Sage dependencies (read the note bellow)
$ cd ./wp-content/themes/sage
$ yarn

# Start watch deamon for theme development
$ yarn run start

# Compile and optimize assets
$ yarn run build

# Build for production
$ yarn run build:production
```

> Note: You can change the development URL after run the `yarn` command. More info [here](https://github.com/roots/sage/tree/9.0.0-beta.3#theme-development).
