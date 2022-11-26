# Uploading and retrieving file IPFS/FileCoin in Next.Js

#### ~> Deependu Jha
---

### Install the package
``` shell
npx create-next-app myapp
npm i web3.storage
```

---
### Import Web3.Storage package
``` js
import { Web3Storage } from 'web3.storage'
```
---

### Upload to the web3.storage

``` js
const storage = new Web3Storage({ YOUR_WEB3_STORAGE_TOKEN });

const CID = await storage.put(FILES); // setFiles(e.target.files)
console.log('Content added with CID:', CID);

``` 

### Get the files
visit the url:
``` js
https://CID.ipfs.w3s.link/FILENAME.EXTENSION
```

---


### Reference:
Docs: https://web3.storage/docs/intro/
Examples: https://github.com/web3-storage/web3.storage/tree/main/packages/client/examples