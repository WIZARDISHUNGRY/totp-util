# totp-util 

Generate TOTP 2-Factor Authentication secrets and QR codes for Google Authenticator on the command-line.

```
$ totp-util ~jellob/.totp-key "Holiday Inn" jellob@travel.kh
/Users/jellob/.totp-key read
```
<pre>
░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
░███████░░█░░░█░░█░░█░███░░░██░███████░
░█░░░░░█░██░██░██░█░░█░░░░░░█░░█░░░░░█░
░█░███░█░░███░░░░█░░░░█░██░░░█░█░███░█░
░█░███░█░██░█░██░░░░░█░█░███░░░█░███░█░
░█░███░█░░░█░██░░░░█░██░█░░█░█░█░███░█░
░█░░░░░█░█░█░░███░██░░██░░░░██░█░░░░░█░
░███████░█░█░█░█░█░█░█░█░█░█░█░███████░
░░░░░░░░░░░░░█░███░░█░██░░░░░█░░░░░░░░░
░█████░█████░████░███░░█░███░░█░█░█░█░░
░░███░░░░░█░░░░░░█░█░████░██░█░░█░░░█░░
░░█░░░███░░████░███░░███░░░░█░░█░██░██░
░░░█░██░░█░██░░██░░████░██░█░░██░░░░██░
░███████░████░██░░█░█░░░░░██░░████████░
░█░░█░█░░░░█░█░░░███░█░██░░█░█░░█░███░░
░█░█░█░█░░░█░░░░██░█░███░░█░█░█░█░█░██░
░░░█░██░░░██░█░███░░█░███░░░░░██░██░██░
░░░░████░░██░███░░█░█░███░██░█████░█░█░
░█░█░░░░░░██░░█░░█░░░█░░██░░░░░░█░██░░░
░███░█░██░░███░█████░█░█░█░░█░░░░░████░
░██░█░█░███░█░░░█░░░███░░░░█████░░█░░█░
░░░█░░░██░░░█░░░█░█░░███████░░██████░█░
░░█░░░░░░██░░██░░█░░█░░██░█░░█░░█░░██░░
░█░█░██████░░░███░██░░█░░░░███████░███░
░█░█░█░░░░█░░██░░░░░█░██░█░██░░████░░█░
░███░███░██░░█░████░█░██░████░░█░█████░
░█░░░░░░█░█░░░░░░█░░░██░█░█░░█░░░░░██░░
░█░░██░█░░█░██░░██░░░█░█░░░░███░░░░███░
░█░░██░░█░░██░░██░░░░░████░█░░░░░░░░█░░
░█░░░░░██████░░░░██░██░░░█████████░██░░
░░░░░░░░░█░░░███░█░█░████░░░██░░░█░░░░░
░███████░█░█░░███░░░░███░░░█░█░█░██░██░
░█░░░░░█░░░█░██░█░░░░░█░█░░░░█░░░█░░█░░
░█░███░█░█░░░█░████░█░█████░████████░░░
░█░███░█░█░░░░░░░█░░░█░░█░█░░█████░███░
░█░███░█░█░███░░████░█░░░███░█░░█░░███░
░█░░░░░█░█░░█░░███░█░░██░░░░███░░░░░░█░
░███████░█░██░░░░███░███████░░░██░░███░
░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
</pre>
```
otpauth://totp/Holiday%20Inn:jellob@travel.kh?secret=NYG4KQIYJ7KOJQ7C&issuer=Holiday%20Inn
```

## Install
```
npm install -g https://github.com/WIZARDISHUNGRY/totp-util
```

## Usage
```
$ totp-util --help

Usage: totp-util [file] [issuer] [user@host]

Options:
  -h, --help           output usage information
  -v, --version        output version number

Examples:

  $ totp-util
  $ totp-util ~mojonixon/.totp-key
  $ totp-util ~al/.totp-key "Wax Trax"
  $ totp-util ~jellob/.totp-key "Holiday Inn" jellob@travel.kh
```

## Additional Docs
- [Configuring OpenSSH with OATH and public keys (2 factor authentication)](https://www.insecure.ws/linux/openssh_oath.html)
- [Using google authenticator with OpenBSD SSH logins](http://blog.asleson.org/index.php/2014/04/11/using-google-authenticator-with-openbsd-ssh-logins/)
