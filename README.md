### 解密

```
import sm2 from '@/static/js/index.js'; // index.js 就是压缩包中index.js

let a = '04123456' // 这个是后端返回的加密字符串
let b = sm2.doDecrypt(a.substr(2, a.length), config.privateKey); // 此处b是解密后数据，privateKey这个是私钥常量
```

### 加密

```
import sm2 from '@/static/js/index.js'; // index.js 就是压缩包中index.js

let a = "15555555555" // 这个是需要加密的字符串
let b = '04' + sm2.doEncrypt(a, config.publicKey); // publicKey这个是公钥常量，b是加密后的字符串
```

### sm 工具类地址
使用sm2
