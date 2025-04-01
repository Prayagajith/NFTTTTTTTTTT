# NFTTTTTTTTTT

Overview

NFT Trading Post is a smart contract written in Solidity that facilitates seamless NFT exchanges on-chain. It allows users to list their NFTs for trade and execute trades in a decentralized manner.

Features

List NFTs for trade.

Execute trades between users.

Secure on-chain ownership transfer.

Contract Address

0x81aE1129974d5f8CbE546c364bA58d13D42cF2a4

How It Works

Listing an NFT for Trade:

The owner of an NFT calls listTrade(nftContract, tokenId), transferring the NFT to the smart contract.

Executing a Trade:

A user calls executeTrade(tradeId, newOwner) to transfer the NFT to the predefined new owner.

Smart Contract Functions

listTrade(address nftContract, uint256 tokenId)

Transfers the specified NFT from the caller to the smart contract.

Stores trade details in the contract.

executeTrade(uint256 tradeId, address newOwner)

Transfers the NFT from the contract to the specified new owner.

Marks the trade as completed.

Dependencies

This contract interacts with ERC-721 NFTs but does not import any external libraries. It assumes standard ERC-721 compliance.

Notes

Ensure the contract has the correct permissions to transfer NFTs.

This contract does not handle pricing or payments, only NFT transfers.

External validation is needed before executing trades.

License

This project is open-source and available under the MIT License.

