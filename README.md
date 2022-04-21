![alt=“Lets build a rug pull”](https://pbs.twimg.com/media/FHFJiAvXwAQT6tP.jpg)

### Background

To automate the creation of joint savings accounts, create a Solidity smart contract that accepts two user addresses. These addresses will be able to control a joint savings account. Your smart contract will use ether management functions to implement a financial institution’s requirements for providing the features of the joint savings account. These features will consist of the ability to deposit and withdraw funds from the account.

### What You're Creating

* The completed Solidity `JointSavings` smart contract.

* A folder named `Execution_Results` contains images of smart contract executions. These images confirm that the deposit and withdrawal transactions, which are designed to test the `JointSavings` functionality in the JavaScript VM, worked as expected.

### Instructions

1. Create a Joint Savings Account Contract in Solidity

2. Compile and Deploy Your Contract in the JavaScript VM

3. Interact with Your Deployed Smart Contract

#### Step 1: Create a Joint Savings Account Contract in Solidity

1. Open the Solidity file named `joint_savings.sol` in the Remix IDE.

#### Step 2: Compile and Deploy Your Contract in the JavaScript VM

1. In the Remix IDE, navigate to the “Deploy & Run Transactions” pane, and then make sure that “JavaScript VM” is selected as the environment.

2. Click the Deploy button to deploy your smart contract, and then confirm that it successfully deployed.

#### Step 3: Interact with Your Deployed Smart Contract

Now that your contract is deployed, it’s time to test its functionality!

To interact with your deployed smart contract, complete the following steps:

1. Use the `setAccounts` function to define the authorized Ethereum address that will be able to withdraw funds from your contract.

     > **Note** You can either use the following Ethereum addresses or create new, dummy addresses on the [Vanity-ETH](https://vanity-eth.tk/) website, which includes an Ethereum vanity address generator.
    >
    > ```text
    > Dummy account1 address: 0x0c0669Cd5e60a6F4b8ce437E4a4A007093D368Cb
    > Dummy account2 address: 0x7A1f3dFAa0a4a19844B606CD6e91d693083B12c0
    > ```

2. Test the deposit functionality of your smart contract by sending the following amounts of ether. After each transaction, use the `contractBalance` function to verify that the funds were added to your contract:

    * Transaction 1: Send 1 ether as wei.

    * Transaction 2: Send 10 ether as wei.

    * Transaction 3: Send 5 ether.

    > **Note** Remembering how to convert ether to wei and vice versa can be challenging. So, you can use a website like [Ethereum Unit Converter](https://eth-converter.com/) to ease doing the conversion.

3. Once you’ve successfully deposited funds into your contract, test the contract’s withdrawal functionality by withdrawing 5 ether into `accountOne` and 10 ether into `accountTwo`. After each transaction, use the `contractBalance` function to verify that the funds were withdrawn from your contract. Also, use the `lastToWithdraw` and `lastWithdrawAmount` functions to verify that the address and amount were correct.

---

### Execution Results
Setting the accounts.
![alt=“SetAccounts”](https://github.com/DanEspin0821/Joint-Savings-Account-20/blob/main/Execution_Results/setAccounts.png)

Depositing 1 ETH in Wei.
![alt=“Deposit 1 Eth in Wei”](https://github.com/DanEspin0821/Joint-Savings-Account-20/blob/main/Execution_Results/1ETHinWei.png)

Showing balance after depositing 1 ETH in Wei.
![alt=“Balance Snap 1”](https://github.com/DanEspin0821/Joint-Savings-Account-20/blob/main/Execution_Results/1EthinWeiBal.png)

Depositing 10 Eth in Wei.
![alt=“10 Eth in Wei”](https://github.com/DanEspin0821/Joint-Savings-Account-20/blob/main/Execution_Results/10ETHinWei.png)

Showing balance after depositing 10 ETH in Wei.
![alt=“Bal Snap 2”](https://github.com/DanEspin0821/Joint-Savings-Account-20/blob/main/Execution_Results/10EthinWeiBal.png)

Depositing 5 ETH.
![alt=“”](https://github.com/DanEspin0821/Joint-Savings-Account-20/blob/main/Execution_Results/5ETH.png)

Showing balance after depositing 5 ETH.
![alt=“Snap bal 3”](https://github.com/DanEspin0821/Joint-Savings-Account-20/blob/main/Execution_Results/5EthBal.png)

Withdrawaing 5 ETH to account 1, and showing the function calls for the balance, and withdrawal functions.
![alt=“Withdraw to acct 1”](https://github.com/DanEspin0821/Joint-Savings-Account-20/blob/main/Execution_Results/withdraw5ethacct1.png)

Withdrawaing 10 ETH to account 2, and showing the function calls for the balance, and withdrawal functions.
![alt=“Withdraw to acct 2](https://github.com/DanEspin0821/Joint-Savings-Account-20/blob/main/Execution_Results/withdraw10ethacct2.png)
