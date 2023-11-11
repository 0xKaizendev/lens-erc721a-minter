# LensNFTMinter

## Context

- Integration of Lens Protocol with ERC721A for efficient NFT minting.
- Aimed at leveraging the Lens Protocol's social media capabilities with the NFT ecosystem.
- Focus on optimizing gas costs for batch minting of NFTs.

## Goal

- Develop a smart contract that allows users to mint ERC721A NFTs directly via LensHub contracts.
- Ensure the contract is compatible with Lens Protocol's Publication Actions.
- Optimize for gas efficiency, especially for batch minting scenarios.

## Interface

LensNFTMintHelper

- Must comply with ERC721A standards for NFT minting.
- Interact seamlessly with Lens Protocol's Publication Actions.

### Fields

- `mintNFT`: Function to mint NFTs.
- `batchMintNFT`: Function for batch minting of NFTs.
- `lensPublicationId`: ID of the Lens publication associated with the minting action.

### Main Functions

- `initializePublicationAction`: Initializes the action module for a publication.
- `processPublicationAction`: Processes the minting action for a given publication.
- `mint`: Function to mint a single NFT.
- `batchMint`: Function to mint multiple NFTs in a single transaction.

### Config Functions

- `setLensHub`: Sets the LensHub address.
- `updateMintingParameters`: Updates parameters related to the minting process.

### Roles

- `admin`: Single account with the ability to update contract parameters and interact with LensHub.
- `user`: General users who can mint NFTs through the contract.


