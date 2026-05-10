# Linux Ticket: User Management & File Permissions

## Ticket Summary
Add two new users to an Ubuntu Linux host, expire their passwords, create a confidential directory with proper group ownership and permissions.

## Environment
- OS: Ubuntu Linux
- Host: brady@UbuntuHomeLab

## Tasks Completed

### 1. Created Users
- Added users `bertram` and `erlich`
- Left additional details blank as specified in ticket

### 2. Expired Passwords
- Forced both users to create a new password on first login using `passwd --expire`

### 3. Created Confidential Directory
- Created `/Confidential` in the root directory

### 4. Created Group and Added Users
- Created group `confidential`
- Added both `bertram` and `erlich` to the group

### 5. Set Ownership and Permissions
- Set owner to `root`, group to `confidential`
- Permissions: full access for root and group, no access for others (`770`)

## Commands Used
```bash
sudo adduser bertram
sudo adduser erlich
sudo passwd --expire bertram
sudo passwd --expire erlich
sudo mkdir /Confidential
sudo groupadd confidential
sudo usermod -aG confidential bertram
sudo usermod -aG confidential erlich
sudo chown root:confidential /Confidential
sudo chmod 770 /Confidential
ls -la /
```

## Verification
Confirmed correct permissions with `ls -la /` showing:
`drwxrwx--- root confidential /Confidential`

## Screenshots
See screenshots folder for full documentation.
