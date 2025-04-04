# NFTTTTTTTTTT

This is a simple on-chain NFT Trading Post written in Solidity. The smart contract allows users to list, buy, and cancel NFT listings on the blockchain.

## Contract Address
0x81aE1129974d5f8CbE546c364bA58d13D42cF2a4

## Features
- *List NFTs*: Users can list their NFTs with a specified price.
- *Buy NFTs*: Users can purchase listed NFTs by sending the required Ether.
- *Cancel Listings*: The owner of a listing can cancel it at any time.

## Smart Contract Functions

### listNFT(address _nftContract, uint256 _tokenId, uint256 _price)
Lists an NFT for sale with a given price.

### buyNFT(uint256 _listingId)
Allows a user to buy an NFT by sending the required Ether.

### cancelListing(uint256 _listingId)
Cancels a listing, making it inactive.

## Notes
- The contract does not include imports or constructors.
- Transactions are handled using payable to transfer funds.
- The contract does not directly handle NFT transfers; external NFT contracts should be used for that purpose.

## License
This project is open-source and available for use under the MIT license.
