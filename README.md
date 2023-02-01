# Senior Frontend Engineer Take Home Assessment

## Overview

Thanks for taking the time to interview with the Gradio team, the next step in the process includes completing a take-home assessment. 

The format of the assessment will consist of:
1. A quick call to help you get setup with your local development environment and answer any questions around the assessment.
2. Time on your own to complete the assessment. (You can always ask us clarifying questions during this process)
3. A final call to explain your submission and approach.

The purpose of this assessment is to create a custom dropdown menu. The dropdown component is an important input component within the Gradio library. It allows developers to enable users to select from a list of options within their demos. This repository currently implements a standard dropdown menu using the html `select` element:

![dropdown_standard](https://user-images.githubusercontent.com/12725292/215598524-f4a628a4-13ca-4d9a-a2c3-9c0c0fc5b938.gif)



As shown above, the current dropdown is limited in its capabilities and very simplistic design. Your job will be to replace this dropdown with your own custom implementation and add more features, requested by our developers. Use the current dropdown component implementation as a starting point and build a completely custom dropdown within a fork of this repository. Below is an example of a custom dropdown with extra functionality, don't feel the need to mimic this exact dropdown, we want to see your own unique approach:

![210434026-737809ed-5e6c-4b10-97ff-e489bbfe72e4_AdobeExpress_AdobeExpress](https://user-images.githubusercontent.com/12725292/215605827-a20fda39-0dec-4bb8-8928-8118695489bc.gif)


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
