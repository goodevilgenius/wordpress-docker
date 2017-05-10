# Wordpress Docker Boilerplate

This is a boilerplate site for Wordpress, with Docker built-in. This will allow you to easily build a Wordpress site with a local environment in Docker.

## Setup

0. Install and setup `docker` and `docker-compose`.
1. [Download](https://github.com/goodevilgenius/wordpress-docker/archive/master.zip) a copy of this repo.
2. Set up your `PATH` variable to include `./bin`. This will allow you to use the built-in scripts to easily interact with your docker instance.
   You can do this by adding this to your `.bashrc` (or similar file for other shells): `export PATH="./bin:$PATH"`.
3. `cp .env.example .env`, and then edit the `.env` as you see fit.
4. `dc build` will run `docker-compose build` to build your images.
5. `dc up` to start your containers.

## Usage

Open up your browser to <http://localhost:7373> and set up Wordpress.

After this, you can also use [wp-cli](http://wp-cli.org/) from the root directory. E.g., to install the [WooCommerce](https://woocommerce.com) plugin, you can run `wp plugin install woocommerce`, and `wp plugin activate woocommerce` to activate the plugin.

## Notes

I'll try to keep this repo up-to-date with the most recent version of Wordpress.

Feel free to submit an issue for any bugs/improvements, or even better, fork the repo, fix the bug, and open a PR.
