## Solana Candy Machine NFT Mint UI

Here is the demo Mint UI URL : https://final-aim-mint-ui.vercel.app/

## Candy Machine Mint UI local deployment
- Clone repository `git clone https://github.com/ernitingarg09/solana-metaplex.git`
- Checkout branch `mint-ui`
- Go to folder `js/packages/candy-machine-ui`
- Find file with extension `*.env` and rename it to just with `.env`
- `.env` file should have below contents
  ```env
  REACT_APP_CANDY_MACHINE_ID=J4hFeorEW8TVyvJbt2cM1Jaz1Q3ChsQVWBoCikd8hFoJ
  REACT_APP_SOLANA_NETWORK=devnet
  REACT_APP_SOLANA_RPC_HOST=https://metaplex.devnet.rpcpool.com/
  SKIP_PREFLIGHT_CHECK=true
  ``` 
- Replace `REACT_APP_CANDY_MACHINE_ID` with candy machine address which is generated during nft upload.
- You can also find candy machine address in file `.cache/devnet-example.json`
- Now, run below commands to launch mint UI
  ```
  cd js/packages/candy-machine-ui
  yarn install && yarn start
  ```

### Candy Machine Mint UI vercel deployment
- In Visual Studio code, open folder `metaplex\js\packages\candy-machine-ui`
- Open new terminal and run `yarn build`
- The above command will create a new deployment folder `build`
- Copy this folder and paster it somewhere else (eg: desktop)
- In open visual studio code, open this build folder
- Publish this folder in github (same as this current repository has been published)
- In `vercel`, import your repository and deploy. 

### Document

I have written a document explaining each steps, please refer [this](https://github.com/ernitingarg09/documents/blob/master/solana/metaplex.md).
