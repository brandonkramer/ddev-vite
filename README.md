<div align="center">
  <a href="https://vitejs.dev/">
    <img width="200" height="200" hspace="10" src="https://vitejs.dev/logo.svg" alt="vite logo" />
  </a>
  <h1>What is ddev-vite?</h1>
  <p>
This add-on simply adds a yaml config that exposes and routes the ports necessary to load up the Vite dev server ande make use of their HMR features inside DDEV.

You can read more about ViteJS on [vitejs.dev](https://vitejs.dev)
</p>
</div>

## Getting started

Install the DDEV add-on and restart the server:

```shell
ddev get wp-strap/ddev-vite
ddev restart
```
Or simply bootstrap a new WP project with these combined commands using this add-on: (make sure to change title & URL inside `wp core install` command accordingly)

```shell
mkdir wordpress 
ddev config --docroot=wordpress --project-type=wordpress
ddev get wp-strap/ddev-vite
ddev start
ddev exec wp core download --path="wordpress"
ddev exec wp core install --path="wordpress" --title="WPVitePlayground" --admin_name="admin" --admin_password="password" --admin_email="admin@local.ddev" --url="https://wp-vite-playground.ddev.site"
```

## Project Example

You can find more info and a project example that works with it here: https://github.com/wp-strap/wp-vite-starter
