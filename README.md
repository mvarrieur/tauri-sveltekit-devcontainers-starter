# Tauri + SvelteKit + Devcontainers starter

This template should help get you started developing with Tauri and Svelte-Kit inside of a dev container for an out of the box cross platform development experience.

## Getting Started
`npx degit mvarrieur/tauri-sveltekit-devcontainers-starter my-new-project`

## Using the dev container
You will need to be running a docker daemon on your local machine for the dev container to start. [Docker Desktop](https://www.docker.com/products/docker-desktop/) is the easiest way to get started if you don't have Docker setup already

Using the devcontainer provided is not required, but it is an easy way to avoid having to install all of the necessary Rust + Node requirements this project has, as well as installing of all the associated VSCode extensions.

When using VSCode you should be prompted to run this project in a devcontainer which will have all of the necessary system requirements setup for you.

## Running the app
1) Run `npm install`
1) Run `npm run tauri dev`
1) Open a browser to http://localhost:6080/ which will you show you the desktop environment running inside the container. The default password is `vscode` (This can be changed in the [.devcontainer/devcontainer.json](./.devcontainer/devcontainer.json) file)
    * Note: You can also use VNC to view the desktop environment running inside of the container, point your VNC viewer to `localhost:5901`
1) Start developing!


## Suggested VSCode extensions
If you run in the dev container these will be installed for you, but otherwise you should probably install them for the best development experience.

* [Svelte](https://marketplace.visualstudio.com/items?itemName=svelte.svelte-vscode)
* [Tauri](https://marketplace.visualstudio.com/items?itemName=tauri-apps.tauri-vscode)
* [rust-analyzer](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer)

## Packaging
Instructions coming soon

## Known Issues
* Rust/Tauri fails compilation on MacOS Docker when using the VirtioFS file sharing implementation (PRs welcome if you know a solution to this)

