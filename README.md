# Senior Frontend Engineer Take Home Assessment

## Overview

The purpose of this assessment is to create a custom dropdown menu. This repository currently implements a standard dropdown menu using the html `select` element:

![dropdown_standard](https://user-images.githubusercontent.com/12725292/215598524-f4a628a4-13ca-4d9a-a2c3-9c0c0fc5b938.gif)



Use the current dropdown component implementation as a starting point and build a completely custom dropdown within this repo. Here's an example of a custom dropdown with extra functionality below:

![dropdown_custom](https://user-images.githubusercontent.com/12725292/215598540-7ece725b-0bb8-4fca-84cd-126fbffc8198.gif)


## Prerequisites

* First, you will fork this repository and follow the [CONTRIBUTING.md](https://github.com/gradio-app/gradio/blob/main/CONTRIBUTING.md) guide in order to setup your local development environment (both client and server side).

  - We will setup an initial call to help with any issues when setting up your local environment. Try to see how far you can get on your own by following the guide. But we expect there to be some hurdles, so don't stress, we'll help get it sorted!

* Next, follow [Creating a new component guide](https://github.com/gradio-app/gradio/blob/main/CONTRIBUTING.md) to understand which specific files in the repository you will have to change to customize the dropdown component. You will mainly be working with:
  - `gradio/ui/packages/form/src/Dropdown.svelte`
  - `gradio/ui/packages/app/src/components/Dropdown/Dropdown.svelte`
  - `gradio/gradio/components.py` (to change the python api and add any additional developer facing parameters for the dropdown component)


## What we're looking for

Please don't feel the need to spend too much time on this assessment! You can always discuss your approach and how you would've implemented something you didn't have the time for. We're mainly looking for how you work and communicate.

Overall:

* A basic working custom dropdown component
* Code quality and organization
* Documentation of how the component works and in-code documentation for any areas of code that may be hard to understand
* Good design eye
* Basic unit tests
* Ability to talk through your implementation
* Willingness to ask us questions if you reach any issues or have trouble understanding anything

Dropdown Features:

* Nice design and UX/UI
* Ability to type and search through dropdown options
* Clear selected option
* Keyboard functionality: enter key to select an option, and arrow key support for navigating options

Extra Dropdown Features (Optional):
* Ability to select multiple dropdown options
* Section headers in the dropdown to organize options
* Filter dropdown options by typing in section header name
* Ability to clear all options and individual options
* [A11Y (accessiblity)](https://developer.mozilla.org/en-US/docs/Web/Accessibility) adherence 
