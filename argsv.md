# Argsv

where stored | process.argsv (array)
how stored
    argsv[0] -> full path of command
    argsv[1] -> full path of file being executed
    args[>2] -> rest of arguments

`node app.js joe`
`// process.argsv[2] == joe`

how to handle named arguments | minimist

`const args = require('minimist')(process.argv.slice(2))
args['name'] //joe`

[link](https://nodejs.dev/learn/nodejs-accept-arguments-from-the-command-line)
