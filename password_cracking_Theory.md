# Password Attack

## 1. Password Gussing

- Password guessing is a technique used to target online protocols and services. Therefore, it's considered time-consuming and opens up the opportunity to generate logs for the failed login attempts. A password guessing attack conducted on a web-based system often requires a new request to be sent for each attempt, which can be easily detected. It may cause an account to be locked out if the system is designed and configured securely.

## 2. Password Cracking

- Password cracking is a technique performed locally or on systems controlled by the attacker.


# Password Profiling

## 1. Default password

- Manufacturers set default passwords with products and equipment such as switches, firewalls, routers.
- For example, suppose the target server is a Tomcat, a lightweight, open-source Java application server. In that case, there are a couple of possible default passwords we can try: `admin:admin` or `tomcat:admin`

#### Some Website that provide defautl password for various product

```
https://cirt.net/passwords
https://default-password.info/
https://datarecovery.com/rd/default-passwords/
```

## 2. Weak Password

#### Weak Password list

- Professionals collect and generate weak password lists over time and often combine them into one large wordlist. Lists are generated based on their experience and what they see in pentesting engagements. These lists may also contain leaked passwords that have been published publically. Here are some of the common weak passwords lists

```
https://wiki.skullsecurity.org/index.php?title=Passwords
https://github.com/danielmiessler/SecLists/tree/master/Passwords
```

## 3. Leaked Password

- Sensitive data such as passwords or hashes may be publicly disclosed or sold as a result of a breach. These public or privately available leaks are often referred to as 'dumps'. 
-  The following are some of the common password lists that have weak and leaked passwords, including `webhost`, `elitehacker`,`hak5`, `Hotmail`, `PhpBB` companies' leaks:

`https://github.com/danielmiessler/SecLists/tree/master/Passwords/Leaked-Databases`


## 4. COmbined wordlist

- Let's say that we have more than one wordlist. Then, we can combine these wordlists into one large file. This can be done as follows using `cat` :

`cat file1.txt file2.txt file3.txt > combined_list.txt`

- To clean up the generated combined list to remove duplicated words, we can use `sort` and `uniq` as follows:

`sort combined_list.txt | uniq -u > cleaned_combined_list.txt`







