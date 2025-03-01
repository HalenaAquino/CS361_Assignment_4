Environment Setup Documentation:

1. Download a virtual OS system (I chose VirtualBox)
2. Download preferred OS (I chose Ubuntu)
3. Start up OS system and create new VM with preferred settings; I chose 4000MB memory and 2 processors
4. Follow OS setup instructions
5. Install OWASP Juice Shop using Docker
     Run these commands on the VM terminal:
      - sudo apt update && sudo apt upgrade -y
      - sudo apt install docker.io -y
      - sudo systemctl start docker
      - sudo systemctl enable docker
      - sudo docker run -d -p 3000:3000 bkimminich/juice-shop
6. Go to "http://localhost:3000" to verify that Juice Shop is running
7. Download Wireshark and Burp Suite Community onto the VM
