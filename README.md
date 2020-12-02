# F5 Cipher version 2020 - December

I use the following cipher ECDHE:RSA:ECDHE_ECDSA:!SSLV3:!RC4:!EXP:!DES:!3DES:TLSV1_3:!TLSv1:!TLSv1_1

TMSH Commands 

Create a cipher rule "custom-secure"
```
create ltm cipher group custom-secure-rule cipher 'ECDHE:RSA:ECDHE_ECDSA:!SSLV3:!RC4:!EXP:!DES:!3DES:TLSV1_3:!TLSv1:!TLSv1_1'
```

Create a cipher Group "custom-secure"

```
create ltm cipher group custom-secure-group allow add { custom-secure-rule }

```



F5 How to article : https://support.f5.com/csp/article/K10866411

