## NFT creator

This project creates, stores, and displays unique digital collectibles, known as Non-Fungible Tokens (NFTs), each with distinct metadata properties.

## Description

This project is a simple NFT creator and manager that allows you to:

- Mint new NFTs with unique metadata (name, eye color, shirt type, and bling)
- Store and manage a collection of NFTs
- List and display the metadata of all minted NFTs
- Keep track of the total supply of NFTs created

## Getting Started

### Installing

* This program is written in a code named file in J-Anushka/JSAssessment repository on github, this can be downloaded from there

### Executing program

To run this program, I'm using Gitpod.io, which is a cloud development environment. 

Once we are on the Gitpod website, we can create a new file in the Explorer section. Save the file with a .js extension. Copy and paste the following code into the file:

// create a variable to hold your NFT's

const NFTs = [];

// this function will take in some values as parameters, create an
// NFT object using the parameters passed to it for its metadata,
// and store it in the variable above

function mintNFT (_name, _eyeColor, _shirtType, _bling) {

  const NFT = {
  
    "name": _name,
    "eyeColor": _eyeColor,
    "shirtType": _shirtType,
    "bling": _bling
    
  }
  
  NFTs.push(NFT);
  
  console.log("Minted: "+ _name);
  
}

// create a "loop" that will go through an "array" of NFT's
// and print their metadata with console.log()

function listNFTs () {

  for(let i = 0; i< NFTs.length; i++) {
  
    console.log("\nID: \t\t" + (i + 1));
    console.log("Name: \t\t" + NFTs[i].name);
    console.log("Eye Color: \t" + NFTs[i].eyeColor);
    console.log("Shirt Type: " + NFTs[i].shirtType);
    console.log("Bling: \t\t" + NFTs[i].bling);
    
  }
}

// print the total number of NFTs we have minted to the console

function getTotalSupply() {

    console.log("\nTotal Supply: " + NFTs.length);
    
  }
  
  // call your functions below this line
  
  mintNFT("Bob", "Blue", "Hoodie", "Gold Chain");
  
  mintNFT("Sue", "Blue", "Hoodie", "Gold Chain");
  
  mintNFT("Anna", "Blue", "Hoodie", "Gold Chain");
  
  mintNFT("John", "Blue", "Hoodie", "Gold Chain");
  
  listNFTs();
  
  getTotalSupply();


  

- To run the code, press Ctrl + Alt + N

## Authors

Anushka Jaiswal

anushkajais1001@gmail.com


