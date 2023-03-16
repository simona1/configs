# Chrome Extension Development

Create a new direcory for the new Chrome extension files.


### [Getting started documentation](https://developer.chrome.com/docs/extensions/mv3/getstarted/development-basics/)

Add a `manifest.json` file that describes configuration of the extension. The example below was taken from the documentation listed above. 

```json
{
  "manifest_version": 3,
  "name": "Hello Extensions",
  "description": "Base Level Extension",
  "version": "1.0",
  "action": {
    "default_popup": "hello.html",
    "default_icon": "hello_extensions.png"
  }
}

```

to be continued