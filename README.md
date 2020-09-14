# python-stack-xray
Small tool to extract all greenlets' stack traces from a greenlet-enabled CPython process

To use:
 1. Copy the file in this repo the server in question (e.g. using `scp`)
 1. Ensure the copied file is mode `0755` and readable and executable by the node user, `swift`
 1. Make sure `gdb` is installed on the node
 1. Run the file with a single supplied argument on the command-line, which is the PID of the hung eventlet process (i.e. a swift wsgi server worker).
