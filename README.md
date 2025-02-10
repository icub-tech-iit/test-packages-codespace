Sandbox for Testing Packages
============================

A one-off disposable environment to test packages for the **`latest ubuntu`** release of our SW distros.

## 🌏  Open in the Cloud 

To get started, click any of the badges below to start a new development environment to demo or contribute to the codebase without having to install anything on your machine:

[![Open in VS Code](https://img.shields.io/badge/Open%20in-VS%20Code-blue?logo=visualstudiocode)](https://vscode.dev/github/icub-tech-iit/test-packages-sandbox)
[![Open in Glitch](https://img.shields.io/badge/Open%20in-Glitch-blue?logo=glitch)](https://glitch.com/edit/#!/import/github/icub-tech-iit/test-packages-sandbox)
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/icub-tech-iit/test-packages-sandbox)
[![Edit in Codesandbox](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/github/icub-tech-iit/test-packages-sandbox)
[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/icub-tech-iit/test-packages-sandbox)
[![Open in Repl.it](https://replit.com/badge/github/withastro/astro)](https://replit.com/github/icub-tech-iit/test-packages-sandbox)
[![Open in Codeanywhere](https://codeanywhere.com/img/open-in-codeanywhere-btn.svg)](https://app.codeanywhere.com/#https://github.com/icub-tech-iit/test-packages-sandbox)
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/icub-tech-iit/test-packages-sandbox)

> [!important]
> You need to enable the [Codespaces](https://docs.github.com/en/codespaces) feature on your account to access the sandbox.

Instead, if you aim to test against different **`distros/releases`**, do:
1. 📝 Edit the file [`Dockerfile`](/.devcontainer/Dockerfile) and create a **`new branch`**. In detail, you have to fiddle with these [sections](/.devcontainer/Dockerfile#L7-L11).
1. 🚀 Launch the corresponding GitHub Codespace from within the new branch. Don't click on the main badge but rather use the green <kbd><> Code</kbd> button up here (switch to the tab `Codespaces`).
1. 🧹 Finish up by wiping out the branch.

### ⚠ How to flush the docker cache
As Docker relies on cached sections, you may still be using an old image when you've just updated a package to test. To invalidate the cache forcing Docker to build the relevant sections entirely again, apply the following workarounds:
- If you aim to build the whole image again, increase the variable [`INVALIDATE_DOCKER_CACHE_ALL`](/.devcontainer/Dockerfile#L5).
- If you've just fixed up the packages and aim to download and install them again, increase the variable [`INVALIDATE_DOCKER_CACHE_DL`](/.devcontainer/Dockerfile#L95).

