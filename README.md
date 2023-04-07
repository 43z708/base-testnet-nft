# Base Goerli Testnet NFT deploy

1. src 直下に.env ファイルを作成し、WALLET_KEY=private key

2. docker compose up -d

3. docker compose exec base bash で docker コンテナ内にログインする（src 直下にいることを確認する）

4. package のインストール

```
npm install
```

5. コンパイル

```
npx hardhat compile
```

6. deploy

```
npx hardhat run scripts/deploy.ts --network base-goerli
```

7. deploy したコントラクトアドレスを控えておき、NFT の claim
   https://quests.base.org/

- Docs https://docs.base.org/guides/deploy-smart-contracts/#prerequisites
