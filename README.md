# terraform
test repository to play around with terraform

```
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt 
# pip3 freeze > requirements.txt
```

Installation:

```
wget -O- https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install terraform
```

## Docker

```
terraform init
terraform apply
terraform destroy
```

## AWS

```
bash credentials.sh
terraform init
terraform fmt
terraform validate # check if configuration is valid
terraform apply
terraform show
```
