const NFTs = []

function mintNFT(name,age,favAnimal,favColor){
    const NFT = {
        "name": name,
        "age": age,
        "favAnimal": favAnimal,
        "favColor": favColor,
    }
    NFTs.push(NFT);
}

function listNFTs(){
    for(let i = 0; i < NFTs.length; i++){
        console.log("\nName: " + NFTs[i].name)
        console.log("Age: " + NFTs[i].age)
        console.log("Favorite Animal: " + NFTs[i].favAnimal)
        console.log("Favorite Color: " + NFTs[i].favColor)
    }
}

function getTotalSupply(){
    console.log("\n" + NFTs.length)
}

mintNFT("Sharon", "22 years old", "Penguin", "Purple")
mintNFT("Momo", "25 years old", "Cat", "Pink")
mintNFT("Jackson", "30 years old", "Tiger", "Blue")
listNFTs()
getTotalSupply()
