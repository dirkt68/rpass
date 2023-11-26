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
    the username `<username>` and would begin generating cryptographically 
    secure passwords with parameters defined by the user.
  - Ex) ```rpass --show --name <account name>``` would prompt for a login 
    and try to display a login with that name by showing `username` printed 
    and by adding the password into the clipboard for a certain amount of 
    time. If no account exists, it will display no account. Adding 
    `--show-pass` would also print the password.
  - Ex) ```rpass --show --all``` would print every login and password to the 
    screen. Would like to add fuzzy searching and maybe selecting without 
    showing passwords for all.
- Add someway for username to be set like a config file, might add ability 
  to do encryption instead of passwords.
- Support TOTP generation for accounts.
- Save to a secure local database that is only accessible with credentials
- Allow the database to be output into json for transfer.
- Learn better programming skills.