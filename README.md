# acme-expect
An expect script to automate diafygi's [acme-nosudo](https://github.com/diafygi/acme-nosudo)

# Compatibilty
The script has to disable port 80 on your webserver. The provided disableport80/enabledport80 script works only for Apache HTTPD on Debian (other distros may have different configuration schemes), but you can easily write your own for other distros or for nginx.

# Prerequesits
 * acme-nosudo's sign_csr.py
 * your letsencrypt user's private/public key pair
 * your server's private/public key pair


# How to use
 - Add the provided files to the directory containing your sign_csr.py script
 - You need to change 3 variables in regenrate.expect : 
   -  user_account_public_key -> this is your letsencrypt account's public key
   -  certificate_request_csr -> this is your SSL's Certificate Signing Request file.
   -  email		      -> a contact e-mail.


