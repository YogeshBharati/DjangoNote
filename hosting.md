### Host Django Website On VPS Using DigitalOcean. Website Include Django With Sqlite3 Database.

### Step 1: Create Droplet on DigitalOcean
### Step 2: Connect to Droplet using SSH
```
ssh root@your_droplet_ip
```
### Step 3: Generate SSH key
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```
### Step 4: Show the pubic key for connect github
```
cat  your_server_publickey(which key add in github setting)
```

### Step 5: Update and Upgrade Packages
```bash
sudo apt update && sudo apt upgrade -y
```

### Step 6: Install Python, Pip, and Virtual Environment
```bash
sudo apt install python3-pip python3-dev libpq-dev nginx curl -y
sudo apt install python3-virtualenv -y
```

### Step 7: Create a New Directory for Django Project
```bash
mkdir django_project
cd django_project
```

### Step 8: Clone Django Project from GitHub
```bash
git clone your_project_url
```

### Step 9: Create Virtual Environment
```bash
python3 -m virtualenv venv
source venv/bin/activate
```

### Step 10: Update Django Settings
```python
ALLOWED_HOSTS = ['132.168.1.231','your_domain.com', 'www.your_domain.com']
```


