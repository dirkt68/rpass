# rpass - a local password manager
This project is  a local password manager with a functionality similar to 
1password, written in Rust. It will support quickly viewing and creating 
logins securely on a local machine.

This is mainly to practice Rust and general programming, and is not intended 
to be a true product. Therefore, YMMV in usage.

## Goals:
- Use command line arguments to quickly create and access logins securely.
  - Ex) ```rpass --new --name <account name> --user <username> --gen-pass``` 
    would prompt for login, add a login for the account `<account name>` with 
    the username `<username>` 