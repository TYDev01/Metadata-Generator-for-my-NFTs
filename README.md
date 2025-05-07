# NFT Metadata Generator

A Python script for batch-generating OpenSea-compatible NFT metadata with dynamic traits and royalties.

![NFT Example](https://via.placeholder.com/600x200?text=NFT+Metadata+Generator)

## Features

- 🎨 Dynamic trait generation with rarity
- 💰 Built-in royalty configuration
- 🌐 IPFS media linking support
- 🔄 Bulk file renaming
- 📁 Organized folder structure
- 📈 OpenSea standards compliant

## Prerequisites

- Python 3.8+
- `python-dotenv` package

## Installation

1. Clone the repository:
```bash
git clone https://github.com/TYDev01/Metadata-Generator-for-my-NFTs
cd Metadata-Generator-for-my-NFTs

pip install -r requirements.txt
```
## Create .env file
```bash
touch .env
```

### Edit .env file
BASE_IPFS_IMAGE_URL="ipfs://YOUR_CID"

### Folder Structure
.
├── .env
├── images/
├── metadata/
├── main.py
└── README.md


## Usage

```bash
python main.py
```

## Example Metadata Output
{
  "name": "Collection Name #42",
  "description": "A unique NFT featuring Thunder God Zenitsu.",
  "image": "ipfs://QmX.../42.jpeg",
  "external_url": "https://yourwebsite.com",
  "attributes": [
    {"trait_type": "Background", "value": "Stormy"},
    {"trait_type": "Eyes", "value": "Thunder God Red"},
    {"trait_type": "Rarity", "value": "Legendary"}
  ],
  "seller_fee_basis_points": 750
}