# Group Management-
- Group is collection of user accounts that share set of permissions.
- Primary Group- Every user acc associated with primary group.
- Specified in /etc/gpasswd
- Secondary group- any additional group
- Specified in /etc/group
### groupadd –
- ‘groupadd’ command is use to add secondary or supplementary group in system. Group information are stored in /etc/group file. 
* Syntax- 
- groupadd [groupname]
### usermod to add user in group-
- usermod option groupname username
### option-
- -G -groupname
- -a - append
### groupmod -
- Modify existing group with customize setting,
* Syntax-
- groupmod option parameter groupname
# Options, 
* -g :- Group id
- sudo groupmod -g new_gid groupname
* -n :- Group Name
- sudo groupmod -n new_groupname old_groupname
 
### groupdel-
- groupdel [groupname]

# Password Management-
## gpasswd –
- ‘gpasswd’ command is use to give password to group.
- It also can be used to add members and assign admin to the group.
- Specified in /etc/gshadow
* gpasswd <option> <parameter> <groupname> 
### Options:
- -a :- Add members in group
#### Syntax-
- gpasswd -a username groupname

- -M :- Set list of members in group
#### Syntax-
- gpasswd -M username1,username2,...,usernameN groupname

- -A :- Assign user as group admin
#### Syntax-
- gpasswd -A username groupname
  
- -d :- To remove user from group
#### Syntax-
- gpasswd -d username groupname







