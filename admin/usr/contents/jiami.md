date: 2014-03-24 23:38:06

title:加密技术和技术 
category: 软考
 
##加密技术##
    1. 发送者生成对称密钥
    2. 将生成的对称密钥和公钥进行加密
    3. 将原文用对称密钥进行加密
    4. 将2、3的结果合并发送给接收者
    5. 接收者先用私钥对2中的文件进行解密得到对称密钥
    6. 再用5得到的对称密钥去解密3的文件得到原文

##认证技术（签名）##
    1. 原文通过Hash函数进行加密成摘要
    2. 将摘要用私钥加密（签名）
    3. 将2得到的结果和原文一起发送给接收者
    4. 接收者原文通过Hash函数进行加密成摘要
    5. 将摘要用公钥加密后跟2的结果比较