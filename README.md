## Take Advantage of Github's verified commits using GPG keys

With signing of commits and tags, One can prove that certain commits and tags were from you.

There are number of ways in which a git repository can be compromised. For example, someone pushed to your repository with the intent of sabotaging your work and claiming it was you as shown below.


> **NOTE**: This is not a mandatory feature. You can use this as additional layer of security in your repository


## Example 1.1 : How easy it is to spoof commit
![](images/commit-history-with-spoof.png?raw=true)

To simulate a spoof commit, just change git config
```
git config user.name Spoofer Person
git config user.email spoofer@email.com
```

To generate GPG Keys, Please go to githubs tutorial in the link provided below:

[Generate GPG Key](https://help.github.com/articles/generating-a-new-gpg-key/)

---

> How do I commit a verified commit?<space><space>

You just need to add -S in git commit as shown below
```
git commit -S -m 'My Verified Commit'
```
---

>So, what does verified commits look like?<space><space>

![](images/verified-commit.png?raw=true)

Happy Coding! :smile: