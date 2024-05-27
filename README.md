const NFTarray = [];
function mintNFT(name,age,job,hobby){
    let NFT = {
        name : name,
        age : age,
        job : job,
        hobby : hobby
    };
     NFTarray.push(NFT);
}

function listNFTs(){
    for(let i=0;i<NFTarray.length;i++){
        console.log("NFT no " + (i+1));
        console.log("NAME: " + NFTarray[i].name);
        console.log("AGE: " + NFTarray[i].age);
        console.log("WORKING JOB: " + NFTarray[i].job);
        console.log("HOBBY: " + NFTarray[i].hobby);
        console.log("       ");
    }
}

function getTotalSupply(){
    return NFTarray.length;
}

mintNFT("Daniel",34,"Pilot","Football");
mintNFT("cooper",28,"HR","Chess");
mintNFT("Kevin",29,"Stuntman","Cricket");
mintNFT("Robert",40,"Actor","Golf");

console.log("List of all NFTs: ");
console.log("     ");
listNFTs();

console.log("Total no of NFTs : " + getTotalSupply());
