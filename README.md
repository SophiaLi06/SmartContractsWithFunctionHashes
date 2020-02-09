# SmartContractsWithFunctionHashes
This repository includes smart contracts and (if available) their corresponding inputs for model checking. Please see follows for additional information:
## Notes for smart contracts that come with inputs for model checking
+ create-react-dapp voting.sol: I have used "PARAM" to refer to the "candidate" parameter of voteForCandidate(bytes32 candidate)
+ ethereum-dapps-examples poll.sol: This is a poll in which the users can only vote for favorable or not favorable. I think we can either consider this as a voting with no candidate, or a voting with two candidates: one being "favorable" and the other being "not favorable"
+ heiswap-dapp Heiswap.sol: I think its withdraw function is really doing a transfer instead. The withdraw function has both receiver and amount specified as parameters. I have used "PARAM1" and "PARAM2" to refer to them respectively.
+ mastering-ethereum-auction-dapp: I have used "TIMESTAMP" to refer to "block.timestamp"
+ auctionhouse: I have used "BLOCKNUMBER" to refer to "block.number"
+ DiceRoll: This is a gambling that determines whether the user gets the reward right after the user calles the "buy" function. That is, there is no "draw" nor "refund" function.
+ SimpleDice: Same as DiceRoll
+ Invest: I was having a hard time telling what model it really fits into. I think it's kind of like a wallet which possibly transfers some money back to the user when they deposit.
+ Wallet-Multi-sig: It works like a wallet which only allows users to transfer.

## Reasons of why some smart contracts are ignored
+ ethereum-dapps NoNameToken.sol: This is a simple contract for token, so I ignored it.
+ multisender UpgradebleStormSender.sol: is really just helping the users to make several transfers at once. It doesn't seem to fit in any of our models
+ note_dapp: is just a note-taking dapp. It doesn't seem to fit in any of our models.
+ react-ethereum-metacoin-master ZettaToken.sol: This is a simple contract for token, so I ignored it.
+ ownanumber: Doesn't come with a smart contract :(
