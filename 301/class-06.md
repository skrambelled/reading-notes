# node.js

## what is node.js

node.js is a runtime built on Google's V8 JavaScript engine, meaning you can run js directly on a machine or in an application using node, rather than using a browsers as your runtime.

You can install node using nvm (Node Version Manager).

To check your version of node, if installed: `node -v`

## Node is single threaded

node.js is single threaded, but also asyncronous through events. Meaning when the logic-flow runs into some sort of event like a server request, rather than stopping there and waiting for the server to process the request, it will simply register a callback function with the event to be called once it is resolved and node will continue on its merry way.

The single threaded nature of Node means that you do need to be aware of situations where you needs to hand off high CPU operations to a different thread.

## Node as your server

You can build the front end and also the backend in JavaScript when using Node so that you dont need to switch languages and your data when switcching between those two sides.

## npm (node package manager)

`node init -y` will inititalise a project, creating a package.json file where you can list any dependencies.

`npm install` will install any listed dependencies.

Dependencies will be installed to `node_modueles/`, which should not be checked into git. Those dependencies are listed in the package.json file.

[<-- Back](../README.md)