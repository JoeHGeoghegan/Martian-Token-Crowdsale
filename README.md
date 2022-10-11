# Unit 21: Martian Token Crowdsale

![alt=""](Images/application-image.png)

## Background

After waiting for years and passing several tests, the Martian Aerospace Agency selected you to become part of the first human colony on Mars. As a prominent fintech professional, they chose you to lead a project developing a monetary system for the new Mars colony. You decided to base this new system on blockchain technology and to define a new cryptocurrency named **KaseiCoin**. (Kasei means Mars in Japanese.)

KaseiCoin will be a fungible token that’s ERC-20 compliant. You’ll launch a crowdsale that will allow people who are moving to Mars to convert their earthling money to KaseiCoin.

### KaseiCoin.sol compile screenshot
![alt=""](Images/KaseiCoin.png)

### KaseiCoinCrowdsale.sol (no deployer) compile screenshot
![alt=""](Images/KaseiCoinCrowdsale.png)

### KaseiCoinCrowdsale.sol (with deployer) compile screenshot
![alt=""](Images/KaseiCoinCrowdsaleDeployer.png)

### Functionality Preview (Note: Capped, Timed, and Refundable)
Activities shown. Metamask is not shown, used primarily for accepting transactions and switching accounts.
1. Deploy the crowdsale to a local blockchain by using Remix, MetaMask, and Ganache.

![alt=""](Images/1.gif)

2. Test the functionality of the crowdsale by using test accounts to buy new tokens and then checking the balances of those accounts.

![alt=""](Images/2.gif)

3. Review the total supply of minted tokens and the amount of wei that the crowdsale contract has raised.

![alt=""](Images/3.gif)

4. Send ether to the crowdsale from a different account (that is, not the same account that’s raising funds). Then, once you confirm that the crowdsale works as expected, try to add the token to your wallet and to test a transaction.

![alt=""](Images/4.gif)

5. By setting the `close` time to a shorter crowdsale show the crowdsale expiring and refunding.

![alt=""](Images/5.png)

6. When sending ether to the contract, make sure that you meet the `goal` of the contract. Then finalize the sale by using the `finalize` function of the `Crowdsale` contract. Note that to finalize the sale, `isOpen` must return false (`isOpen` comes from `TimedCrowdsale` and checks whether the `close` time has passed). If you set the `goal` to 300 ether, for example, you might need to have multiple accounts buy tokens to meet the goal. If you run out of prefunded accounts in Ganache, you can create a new workspace.

![alt=""](Images/6.gif)

7. Review your tokens in MetaMask. To do so in MetaMask, click Add Token, click Custom Token, and then enter the address of the token contract. Make sure to buy larger amounts of tokens to get the denomination to appear in your wallet as more than a few wei worth.

![alt=""](Images/7.png)
