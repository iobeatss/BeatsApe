# 📝 BeatsApe NFT — Contract Information

**Network**: Ethereum Mainnet  
**Standard**: ERC-721 (OpenZeppelin)  
**Token Name**: BeatsApe  
**Symbol**: BAPE  
**Max Supply**: 10,000

## 🔗 Contract Address
`0x1234567890abcdef1234567890abcdef12345678`

## 📦 Features
- EIP-2981 Royalties (marketplace-compatible)
- Verified on Etherscan
- Metadata on IPFS (image + animation_url)
- OpenSea/LooksRare compatible
- Pausable & Ownable (admin) — optional

## 🧰 Admin / Minting
- **Base URI**: `ipfs://QmYourBaseCID/` (each token adds `<id>.json`)
- **Mint Types**: allowlist / public / airdrop (selon ton implémentation)
- **Start/Stop**: via `pause()` / `unpause()` si nécessaire

## 🪙 Royalties
- **Recipient**: `0x1234567890abcdef1234567890abcdef12345678`
- **Fee**: 5% (example)

## 📚 Notes
- Replace all CIDs after deploying files to IPFS.
- `background_color` must be hex without `#` (OpenSea).
- `attributes` support `display_type`: `number`, `boost_percentage`, `boost_number`, `date`.
- For animated NFTs, prefer `animation_url` (mp4/gif/html) + a static `image`.
