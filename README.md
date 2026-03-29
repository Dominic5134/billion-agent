# billion-agent
Update
sudo apt-get update && sudo apt-get upgrade -y
Cài Node.js & npm
sudo apt install -y nodejs npm
Cài đặt git
sudo apt install -y git
Clone source repository
git clone https://github.com/BillionsNetwork/verified-agent-identity
cd verified-agent-identity
Cài đặt package
npm install shell-quote @iden3/js-iden3-auth @0xpolygonid/js-sdk ethers uuid cross-fetch
Cài skill qua ClawHub
npx clawhub@latest install verified-agent-identity
Tạo Billion identity
node scripts/createNewEthereumIdentity.js
Tạo billion verify link
node scripts/manualLinkHumanToAgent.js --challenge '{"name":"TênAgen","description":"mô tả"}'
