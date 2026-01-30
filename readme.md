````markdown
# Banking Application

Banking application with facial recognition and keystroke dynamics authentication.

## Requirements Installation

Install the required dependencies on the host machine.
```bash
sudo apt update
pip install -r requirements.txt
````

## Docker

To install the Docker package:

```bash
sudo apt update
sudo apt install -y docker.io
sudo systemctl enable docker --now
sudo usermod -aG docker $USER
```

To import the Docker image:

```bash
tar --no-same-owner -xjvf meudocker.tar.bz2
sudo docker import meudocker.tar tbmesi # sha256:388ca49fa3fac1c5a33ed5fa8ab21fc9811cab8fdb1426dfa13b085c6bb66220
sudo docker run --name dockerfinal -it tbmesi /bin/bash
```

Inside the Docker container:

```bash
service ssh restart
```

To start the application:

```bash
python3 bankApp.py
```

```

Se quiseres um tom mais “corporate”, mais técnico, ou mais simples para GitHub público, ajusto num instante.
```
