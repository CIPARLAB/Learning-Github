# CIPAR LAB
**Welcome to the CIPAR LAB**.

This is the official repository of the CIPAR LAB. Here you can find the code and the data of the experiments conducted in the lab. The repository is organized in the following way:

![test_logo](/Photos/logo_2.png)




Link to our website: [website](https://sites.google.com/uniroma1.it/cipar-labs/home)
## GitHub Tutorial 

###
`**Clone**` the repository means to download the repository to your local machine. Literally, you are making a copy of the repository in your local machine.  
To clone the repository you have to use the command `**git clone**` followed by the URL of the repository. 
```bash
git clone URL
```

While if you already have a copy of the repository in your local machine in order to synchronize the information that is on GitHub with the information that is on your local machine you have to use the
command `**fetch**`. `**fetch**` is used to download the information from the repository to your local machine.
```bash
git fetch
```

**pull** command is the combination of `**fetch**` and `**merge**`. It is used to download the information from the repository to your local machine and to merge the information that is on the repository with the information that is on your local machine.
```bash
git pull
```
However, you have to specify the branch that you want to merge in the case of lack of tracking information for the current branch. In this case, you have to use the following command:
```bash 
git pull origin branch_name
```
or alternatively, you can use the following command:
```bash
git branch --set-upstream-to=origin/branch_name
```

Finally, `**push**` command is used to upload the information that is on your local machine to the repository. 
```bash
git push
```
This command pushes to the main branch of the repository. If you want to push to a different branch you have to use the following command:
```bash
git push -all
```