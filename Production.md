(SingIn)[https://docs.docker.com/desktop/setup/sign-in/#credentials-management-for-linux-users]

Generate a GPG key. You can initialize pass by using a gpg key. To generate a gpg key, run:
```
gpg --generate-key
```

Copy the GPG ID and use it to initialize pass
```
 pass init D68F91E1C54E2BC3A28A1B7E937CB9EB0D2CEFBA

```
output 
```
mkdir: created directory '/home/mamun/.password-store/'
Password store initialized for D68F91E1C54E2BC3A28A1B7E937CB9EB0D2CEFBA

```
Then You have to login from Docker Desktop Gui