<br />
<br />

<p>
<img width="1431" alt="屏幕快照 2020-05-19 下午5 22 58" src="https://user-images.githubusercontent.com/2507027/82379839-97245780-99f5-11ea-902f-983d09049b9e.png">
  
<img width="1299" alt="屏幕快照 2020-05-19 下午5 23 26" src="https://user-images.githubusercontent.com/2507027/82379872-a1deec80-99f5-11ea-81b6-5b7388fc21c8.png">

</p>

<br />
<br />

Near Beauty is a roguelike game which you need a Near Protocol Account to start the game and redeem your bountry assets.

### To run on main Testnet
#### Requirements
##### IMPORTANT: Make sure you have the latest version of NEAR Shell and Node Version > 10.x 
1. node and npm
2. near shell
Install with 
```
npm i -g near-shell
```
3.(optional) install yarn to build
```
npm i -g yarn
```
#### procedure
Step 1: Create account for the contract and deploy the contract.
In the terminal
```
near login
```
click the link and create your own contract ID

Step 2:
Modify src/config.js line that sets the contractName. Set it to id from step 1.
```
const CONTRACT_NAME = "contractId"; /* TODO: fill this in! */
```

Step 3:
Finally, run the command in your terminal.
```
npm install && npm run start
```
with yarn:
```
yarn install && yarn start
```
The server that starts is for static assets and by default serves them to localhost:3000. Navigate there in your browser to see the app running!

## To Explore

- `assembly/main.ts` for the contract code
- `src/index.html` for the front-end HTML
- `src/main.js` for the JavaScript front-end code and how to integrate contracts
- `src/app.js` for the first react component

### To run on Local Node

Step 1:
Get nearcore

Step 2:
Use command ```./scripts/start_localnet.py --local``` to start the local node

Step 3:
Install serve with:
```
npm i serve
```
Use command ```serve src -p 3000``` to start on localhost:3000

Step 4:
Start frontend with command:
```
NODE_ENV=local yarn start
```
Now, open localhost:3000. Navigate there in your browser to see the app running!

Step 5:
Use wallet/login/index.html to create account and start exploring.
