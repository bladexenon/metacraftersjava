// Array to store minted NFTs
let mintedNFTs = [];

// Function to mint an NFT with metadata
function mintNFT(name, image, description, ...otherProperties) {
  // Create an NFT object with metadata
  const nft = {
    name,
    image,
    description,
    ...otherProperties, // Include any additional properties passed
  };

  // Push the new NFT object into the storage array
  mintedNFTs.push(nft);
}

// Function to list all minted NFTs
function listNFTs() {
  console.log("**Your Epic NFTs**");
  if (mintedNFTs.length === 0) {
    console.log("No NFTs minted yet!");
  } else {
    for (const nft of mintedNFTs) {
      console.log(`\nName: ${nft.name}`);
      console.log(`Image: ${nft.image}`); // This assumes that the image is a url
      console.log(`Description: ${nft.description}`);
      // Print any additional properties if present
      for (const key in nft) {
        if (key !== 'name' && key !== 'image' && key !== 'description') {
          console.log(`${key}: ${nft[key]}`);
        }
      }
    }
  }
}

// Function to get the total number of minted NFTs
function getTotalSupply() {
  return mintedNFTs.length;
}

// Example usage (call your functions here)
mintNFT("Cool Cat", "https://catgaming.com/coolcat.png", "A very cool cat.");
mintNFT("Shining Dragon", "https://bigdraco.com/dragon.jpg", "A majestic dragon with shimmering scales.");
mintNFT("BearMofu", "https://bigbearwithmofusand.com/bearsand.jpg", "The cutest bear ever!.");

listNFTs(); // Print all minted NFTs
const totalNFTs = getTotalSupply();
console.log(`Total NFTs minted: ${totalNFTs}`);
