# 	BIT密码学研究生学习路线-AI
目前我是北京理工大学-网络空间安全学院-密码学**研0**，计划在2026年9月份开学前**系统学习密码学的核心理论**，阅读相关文献，了解行业发展现状，争取早日把本科计算机的编码能力、工程落地能力应用在密码学的项目中。

欢迎大家与我交流学习心得，愿我们都有一个美好的未来。

##  1. 基础理论  
学习数学理论基础，为理解密码学的算法奠定基础。  
1. **<span style="color:#e60000;">《初等数论》（潘承洞）</span>**  
	要求：吃透：整除、同余、CRT、欧拉函数、阶 & 原根、二次剩余。  
2. **<span style="color:#e60000;">《抽象代数》</span>**   
	要求：群、环、域、循环群、置换群、多项式环  
3. **<span style="color:#e60000;">《有限域及其应用》</span>**  
	要求：Fp、有限域扩张F2n、本原多项式、域上运算。

##  2. 入门阶段  
1. 了解密码学的基本理论，先从最简单的开始入门：**<span style="color:#e60000;">《深入浅出密码学》</span>**    
睡前读物   

2. 系统打底：**<span style="color:#e60000;">《密码学原理与实践 (第三版)》</span>（Stinson）**  
- 定位：密码学国际经典教材，也是国内很多高校的教学蓝本，覆盖对称 / 公钥 / 哈希 / 协议全体系，逻辑严谨，习题质量高。  
 - 怎么读：  
	- 先读：第 1-7 章（<span style="background-color:#ffff00;">对称密码、公钥密码基础、哈希、数字签名</span>）  
	- 重点啃：<span style="background-color:#ffff00;">RSA、离散对数、椭圆曲线、对称密码分析基础</span>
	- 跳过：太老的算法（DES 等）和你暂时用不上的协议细节，先建立完整知识框架。  
    
3.  国内高校适配版：**<span style="color:#e60000;">《现代密码学 (杨波)》</span>**    
- 定位：国内密码学入门主流教材，内容贴合国内课程体系，有国密相关内容，语言更易读。
- 怎么读：
	- 读：和 Stinson 互补的部分，比如<span style="background-color:#ffff00;">国密算法（SM2/SM3/SM4）、密码协议的简化讲解</span>
	- 重点：国密部分直接对接未来北理课程和就业需求
	- 方式：作为 Stinson 的补充，而不是从头啃一遍



同时想要进阶论文的阅读能力，可以看一些难度稍微高一点的书，我选择了《Introduction to Modern Cryptography》，这本书无论是英文写作还是理论学术都对初学者有很大帮助。配合b站上[<span style="background-color:#ffff00;">斯坦福教授Dan Boneh的密码学</span>](https://www.bilibili.com/video/BV1yx411T78i/?vd_source=1e182b13168c097b8bfb5d1ab9aea2e3)课程观看，每天花2小时的时间观看课程并做笔记，大概需要15天的时间全部看完。  

## 	3. 研究阶段  
 阅读密码学基础文献，理解<span style="background-color:#ffff00;">公钥加密、数字签名、身份加密</span>等技术实现。    
论文list:  
- 数字签名  
[1] Boneh, D., Lynn, B., Shacham, H.: Short signatures from the Weil pairing. In: C. Boyd (ed.) 
ASIACRYPT 2001, LNCS, vol. 2248, pp. 514–532. Springer (2001)   
[2] Boneh, D., Boyen, X.: Short signatures without random oracles. In: C. Cachin, J. Camenisch 
(eds.) EUROCRYPT 2004, LNCS, vol. 3027, pp. 56–73. Springer (2004)

- 公钥加密  
[1] Cramer, R., Shoup, V.: A practical public key cryptosystem provably secure against adaptive 
chosen ciphertext attack. In: H. Krawczyk (ed.) CRYPTO 1998, LNCS, vol. 1462, pp. 13–25. 
Springer (1998)   
[2] Abdalla, M., Bellare, M., Rogaway, P.: The oracle Diffifie-Hellman assumptions and an analy
sis of DHIES. In: D. Naccache (ed.) CT-RSA 2001, LNCS, vol. 2020, pp. 143–158. Springer 
(2001) Attention！This paper gave a hashed ElGamal encryption scheme. You can try to give an ElGamal encryption scheme. 

- 基于身份的加密  
[1] Boneh, D., Franklin, M.K.: Identity-based encryption from the Weil pairing. In: J. Kilian 
(ed.) CRYPTO 2001, LNCS, vol. 2139, pp. 213–229. Springer (2001)   
[2] Boneh, D., Boyen, X.: Effificient selective-ID secure identity-based encryption without ran
dom oracles. In: C. Cachin, J. Camenisch (eds.) EUROCRYPT 2004, LNCS, vol. 3027, pp. 
223–238. Springer (2004)   

要求：
1. 理清background，motivation和contribution
2. technique掌握，包括algorithm definition和construction。掌握意味着可以脱稿讲出，在适当的情况下会用
3. security model和security proof（这个可以放后面一个阶段）
4. 写个report或者summary，在meeting前发给导师，meeting在准备好之后，提前约个时间就好
5. 尽量用英文写，保持每周都有文献的输入

## 4. 开学后  
1. 进阶1：**《密码编码学与网络安全。原理与实践。第七版》（William Stallings）**
- 定位：偏应用的经典教材，覆盖密码在网络安全中的落地，适合理解 “密码怎么用”。
- 怎么读：
	- 读：和网络安全结合的部分，比如 SSL/TLS、IPsec、PGP
	- 跳过：和 Stinson 重复的理论基础部分，只补 Stinson 没讲的应用场景
	- 定位：当工具书用，遇到协议 / 应用问题时翻，不用通读  
    
2. 进阶2：**《现代密码学 - 原理和协议》（Katz & Lindell）**  
- 定位：密码学理论硬核教材，偏形式化证明和安全定义，是科研向的经典。
- 怎么读：
	- 等 Stinson 和杨波的书读完，进组做科研时，再根据课题需要翻对应章节（比如零知识证明、安全多方计算部分）。
	- 重点：理解 “可证明安全” 的思想，这对做 AI 安全 + 密码交叉的课题很重要。
