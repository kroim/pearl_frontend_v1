

npm install

npm start

So this repo is cloned originally from pig-defi.

You can find their repo here:

https://github.com/Pig-Finance

The Pearl token is a clone of Pantherswap Token. 

The masterchef is a clone of Void.Farm (now defunct), with additional features taken form the Pantherswap Masterchef. 

Their website color scheme was atrocious and the logo was horrendous. But I used this because I am entirely self-taught and don't know how to initialize Storybook. This repo seems to work fine using the above commands and configuring storybook wasn't needeed.


Note: Please see pearl_frontend_V1/contracts to see the codes for Pearl and Masterchef.

1. Deposit and withdraw works on the masterchef, but upon users depositing a second time, withdraws create a safemath error: subtraction overflow

Note: all contracts on the frontend have not been updated and are using old contracts. 

Current Frontend issues:

1. Wallets sync with certain contract functions, correctly showing the amount of Pearl in wallet for example, but currently cannot sync after calling approval functions in the pool.
 
2. Some stats are not displaying correctly on the home screen. Total supply works but 'burned amount' doesn't work.  



Additional Questions:

1. When adding an adddiitonal native token (PEARL) farm pool to the UI, how does the app differentiate between PEARL and non-PEARL LP pools? In order that the farm card correctly shows the gradient animaiton. 

2. I want to activate the 'Souschef'/Syrup page. I tried to do this but got errors. The code is already there on src/views/pools/Syrup.tsx. I just need it activated and able to be navigated by the menu. I plan to use this page for users to stake PEARL and receive BUSD through a separate souschef contract.

3. Instructions for how to delpoy the final app on a VPS server.

4. Whatever else needs to be done in order to make this production ready and go live.

5. Are there any special things to keep in mind for the PEARL smart contract regarding the contract's automated liquidity function? I have tested it an it works fine so far. 

Optional:

1. Lottery (code is already there, just not sure how to activate it)

****


Notes to self:

to differentiate between single staking and LP, simply include 'isTokenOnly: true,' beneath the 'risk' label
