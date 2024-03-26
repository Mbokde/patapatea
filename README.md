
👨‍💻sudo su
👨‍💻curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash - &&sudo apt-get install -y nodejs
👨‍💻npm install
👨‍💻curl -L https://foundry.paradigm.xyz | bash
👨‍💻source /root/.bashrc
👨‍💻foundryup
👨‍💻wget -qO - 'https://proget.makedeb.org/debian-feeds/prebuilt-mpr.pub' | gpg --dearmor | sudo tee /usr/share/keyrings/prebuilt-mpr-archive-keyring.gpg 1> /dev/null
👨‍💻echo "deb [arch=all,$(dpkg --print-architecture) signed-by=/usr/share/keyrings/prebuilt-mpr-archive-keyring.gpg] https://proget.makedeb.org prebuilt-mpr $(lsb_release -cs)" | sudo tee /etc/apt/sources.list.d/prebuilt-mpr.list
👨‍💻apt update
👨‍💻apt install just
👨‍💻just install
