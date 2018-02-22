# ibm-verse-extension-poins-example
IBM Verse Extensions Points consolidated examples

More details here:
http://ebasso.net/wiki/index.php?title=IBM_Verse:_Extension_Points_-_Examples


# Getting start

## Prerequisites

A prerequisite is to have an IBM Domino server installed and IBM Verse configured.

## Configure Ansible hosts file

First you need to clone/download my files from Git Hub https://github.com/ebasso/ibm-verse-extension-points-examples

1) Copy the **applications.json** file to the **notesdata** directory

2) Edit applications.json, and change urls to the hostname of your Domino server

3) Copy or Move the vopext directory to
```
 /domino/notesdata/domino/html/vopext
 ```

4) Set the variables in the notes.ini:
```
 VOP_EXTENSIBILITY_DATA_PROVIDER_NAME=localFileProvider
 VOP_Extensibility_Applications_Json_FilePath=/domino/notesdata/applications.json
```

5) Restart http the server

# Authors

* **Enio Basso** - *Initial work* - [My Repository](https://github.com/ebasso)


See also the list of [contributors](https://github.com/ebasso/ansible-ibm-websphere/graphs/contributors) who participated in this project.

# License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
