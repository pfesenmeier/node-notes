# exiting node

*ending a process that will not end.*

ungraceful | `process.exit(1) || process.kill()`
graceful | handler for 'SIGTERM' calls 'close'
`process.on('SIGTERM', () => {
  server.close(() => {
    console.log('Process terminated')
  })
})`
