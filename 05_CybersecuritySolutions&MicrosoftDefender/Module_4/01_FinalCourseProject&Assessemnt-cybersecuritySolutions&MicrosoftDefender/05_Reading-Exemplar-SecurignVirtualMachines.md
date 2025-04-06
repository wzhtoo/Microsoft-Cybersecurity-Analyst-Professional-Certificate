# Exemplar: Securing virtual machines

[Exemplar: Securing virtual machines 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/supplement/my0PK/exemplar-securing-virtual-machines)

# နမူနာ- Virtual Machines များကို လုံခြုံစေခြင်း (Exemplar: Securing virtual machines)

## နိဒါန်း (Introduction)

Virtual Machines များကို လုံခြုံစေခြင်း လေ့ကျင့်ခန်းတွင်၊ အခြားကုမ္ပဏီများသို့ IT ဝန်ဆောင်မှုများ ပေးဆောင်သည့် အသေးစားလုပ်ငန်းတစ်ခုအတွက် စမ်းသပ်ပတ်ဝန်းကျင်တစ်ခု ဖန်တီးရန် virtual machine တစ်ခုကို တည်ဆောက်ကာ ကာကွယ်ရန် တာဝန်ပေးအပ်ခြင်းခံရပါသည်။ ၎င်းကိုပြုလုပ်ရန် JIT၊ Azure Bastion နှင့် Azure Standard Firewall တို့ကို အသုံးပြုခဲ့ပါသည်။ စမ်းသပ်ပတ်ဝန်းကျင်ကို စောင့်ကြည့်ရန် Microsoft Sentinel ကိုလည်း တည်ဆောက်ခဲ့ပါသည်။ ဤနမူနာသည် လေ့ကျင့်ခန်းအတွက် ဖြေရှင်းချက်အဖြစ် ဆောင်ရွက်ပြီး သင်လိုက်နာရမည့် အဆင့်များကို သရုပ်ပြသည့် ဖန်သားပြင်ဓာတ်ပုံများ ပါဝင်ပါသည်။ အောက်ပါပုံသည် သင်ဖန်တီးရန် လိုအပ်သည့် ကွန်ရက်ဖွဲ့စည်းပုံ၏ အယူအဆဆိုင်ရာ ကိုယ်စားပြုမှုတစ်ခုဖြစ်သည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/nzxCiliRRsaTwk96ogqIPA_a37519f257874eeb8115c3a3596fdae1_C5M4L1_Item-05_Exemplar_final-project-diagram_new2.png?expiry=1744070400000&hmac=rk95vgfWPFhsZsF7jdbEMGw_kLmwsZtm8MyJY2HCV00">

## ဖြစ်ရပ်လေ့လာမှု (Case study)

IT ဝန်ဆောင်မှုများ ပေးဆောင်သည့် အသေးစားလုပ်ငန်းတစ်ခုတွင် Microsoft Azure တွင် လက်ခံထားသည့် စနစ်များစွာ ရှိပါသည်။ backend စနစ်များကို Azure virtual machines များတွင် လက်ခံထားပြီး ၎င်းတို့ကို လုံခြုံစွာ ဖွဲ့စည်းကာ ခြိမ်းခြောက်မှုများမှ ကာကွယ်ရန် လိုအပ်ပါသည်။

Microsoft လုံခြုံရေး ဝန်ဆောင်မှုများစွာကို အသုံးပြု၍ စမ်းသပ်ပတ်ဝန်းကျင်တစ်ခု တည်ဆောက်ရန် လုံခြုံရေး အင်ဂျင်နီယာအဖြစ် သင်ငှားရမ်းခြင်းခံရပါသည်။ ဤစမ်းသပ်ပတ်ဝန်းကျင်သည် ဤ IT ဝန်ဆောင်မှုပေးသူအတွက် အနာဂတ်တွင် ထုတ်လုပ်ရေး VMs များကို မည်သို့ ကာကွယ်မည်ကို အခြေခံမည်ဖြစ်သည်။

သင်၏ အလုပ်ရှင်သည် JIT၊ Azure Bastion နှင့် Azure Standard Firewall တို့ကို အသုံးပြု၍ Azure ရှိ virtual machine တစ်ခုအတွက် ကာကွယ်ရေးကို တည်ဆောက်ရန် သင့်အား လိုအပ်ပါသည်။ ၎င်းကို တည်ဆောက်ပြီးသည်နှင့် ထုတ်လုပ်ရေး ကွန်ရက်တွင် မဖြန့်ချိမီ စမ်းသပ်ပတ်ဝန်းကျင်ကို စောင့်ကြည့်ရန် Microsoft Sentinel ကို ဖွဲ့စည်းရန်လည်း လိုအပ်ပါသည်။

## ညွှန်ကြားချက်များ (Instructions)

### အဆင့် ၁- Virtual Machine တည်ဆောက်ခြင်း (Step 1: Virtual machine setup)

စမ်းသပ်ပတ်ဝန်းကျင်တစ်ခု တည်ဆောက်ရန် virtual machine တစ်ခုကို ဦးစွာ လိုအပ်ပါသည်။ အရင်းအမြစ်အုပ်စုအသစ်တွင် virtual machine တစ်ခုကို ဖြန့်ချိပါ။ Azure Bastion ကို အဝေးမှ ဝင်ရောက်ရန် အသုံးပြုမည်ဖြစ်သောကြောင့် ဤ VM အတွက် အများသုံး IP မလိုအပ်ပါ။ virtual machines များကို မည်သို့ ဖန်တီးရမည်ကို သတိရစေရန် [Virtual Machine တစ်ခုကို စတင်ခြင်း](link_to_spinning_up_vm_video) ဗီဒီယိုကို ပြန်လည်ကြည့်ရှုပါ။

1.  သင်၏ အထောက်အထားများဖြင့် [Azure portal](https://portal.azure.com/) သို့ ဝင်ရောက်ပါ။
2.  Azure portal မီနူးတွင်၊ မျက်နှာပြင်၏ ဘယ်ဘက်ခြမ်းတွင် တည်ရှိသော **အရင်းအမြစ်တစ်ခု ဖန်တီးပါ** ခလုတ်ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/SB5-t45tTCa5PXHhgLSRhA_6fe55861dcfe495397236a7610c86ce1_image.png?expiry=1744070400000&hmac=sgj2MmTqL1esFjfY1NixMegvjO-Bam2hi79AtpX32DA">

3.  နောက်တွင်၊ ရှာဖွေရေးဘားတွင် “virtual network” ကို ရှာဖွေပါ၊ ရလဒ်များမှ **Virtual machine** ကို ရွေးချယ်ပြီး **ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/XbNxVPrLSsCnfNqAJuaA5g_5d56a8d1254f472a977cdae3947991e1_image.png?expiry=1744070400000&hmac=jTnFrWdfCA7Ft77x1kdaw9bVtIy2KWgeVah3LqNQw9U">

4.  Virtual Machine ဖန်တီးခြင်း wizard ၏ **အခြေခံများ** တက်ဘ်တွင်၊ အောက်ပါ အချက်အလက်များကို ဖြည့်စွက်ပါ-
    _ Subscription: သင်၏ subscription ကို ရွေးချယ်ပါ။
    _ Resource group: **အသစ် ဖန်တီးပါ** နှင့် အရင်းအမြစ်အုပ်စုအသစ်၏ အမည်အဖြစ် "Services\*Test" ကို ထည့်ပါ။

    - အမည်- virtual machine ၏ အမည်အဖြစ် "ServicesVM" ကို ထည့်ပါ။
      \_ ဒေသ- သင့်နှင့် အနီးဆုံး ဒေသကို ရွေးချယ်ပါ။ \* ပုံရိပ်- Windows Server 2022 Datacenter: Azure Edition။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/aocB0CIGQbCLM5Ev6wabLg_7688cfe452b3488d89daa722892c8ce1_image.png?expiry=1744070400000&hmac=jh-oBndlg-ms0s8dhDs7hM46Hq7jvfTBm4hYKqhQmcY">

အောက်သို့ ဆင်းပြီး ကျန်အသေးစိတ်များကို ဖြည့်စွက်ပါ။

- အရွယ်အစား- Standard_DS1_v2
- Username: AzAdmin
- Password: P@<span class="math-block">@1234567
- Password အတည်ပြုပါ\- P@</span>@1234567

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/-b4UFqjISTOKrlG286PH9w_dbc87b946c8c4bf8b52134045ebe28e1_image.png?expiry=1744070400000&hmac=rtjjBSZfomKvZyIeQGh0GD1-AD2doP0A83HL-QT08h8">

5.  **နောက်တစ်ခု- Disks** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Gy3dOKdsTjKoH2DZ1Ij2Gw_aa82742114e04d7fa706170b1b459de1_image.png?expiry=1744070400000&hmac=jq-J4oY8h4y0rgAKpgd5e0OUnioZpfhuupTHXCqcF0M">

6.  **နောက်တစ်ခု- Networking** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/ZnOkQGrSQCKPefQFAtHA5g_c216b808cbac4bc88112deba253d8be1_image.png?expiry=1744070400000&hmac=Yh4q3hTZfE6YAzp4V4nHmfTpdGXZ4Y_Gdwobhe8U0S4">

7.  virtual network အတွက် **အသစ် ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/F1JGJmApSAuttHp3ennTAw_581c62007a17417b8e9ac521ba5ea4e1_image.png?expiry=1744070400000&hmac=MZ7BvdF8DvFjwrkY4PHIi-5RCQjDbIYQ5PyhVPIao58">

8.  Virtual network ဖန်တီးခြင်း စာမျက်နှာတွင် အောက်ပါ အသေးစိတ်များကို ဖြည့်စွက်ပါ-

    - အမည်- "Services_Test_Network"
    - Address space address range: 172.16.0.0/16
    - Subnets Subnet အမည်- "VMs"
    - Subnets Address range: 172.16.1.0/24

9.  **OK** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/nKMegL9tSMOR65jiqGy-6Q_9748c065192a450cb54f668261b536e1_image.png?expiry=1744070400000&hmac=-vt-Fhn16ldyaZPLAXMkBPza9oLdp6gMe0CdSFjXwVY">

10. အများသုံး IP အတွက် **None** ကို ရွေးချယ်ပါ။
11. ဆက်တင်များကို ပြန်လည်သုံးသပ်ရန် **ပြန်လည်သုံးသပ်ပြီး ဖန်တီးပါ** ခလုတ်ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/FvQF0hfHSOKqdyCx4LNJ1Q_1883a8323257440894c626cae38e8be1_image.png?expiry=1744070400000&hmac=IFjYf8uOh_K1FBgEPwz_MoixpFj4jsRdCmoL1XaOzq0">

12. virtual network ကို ဖန်တီးရန် **ဖန်တီးပါ** ခလုတ်ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/E41ViewFT363Tz5nivgO4w_ffee0818149f4d38ae77cddefaa720e1_image.png?expiry=1744070400000&hmac=Xkie_fQGJuQU4xhWWzMSNNpV4-sPk2jCxVKj39RpzUU">

13. virtual machine သည် ယခု ဖြန့်ချိပါမည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Tk41KFAJSTS6QQvs2ezw0A_b1de676e831b411998cb1ca741a7f0e1_image.png?expiry=1744070400000&hmac=fgUOgOn4y0qFfgBCRQ75G9DEiwD_izBejDbfyLZNq1k">

### အဆင့် ၂- VNet peering ပါသော Hub Network (Step 2: Hub Network with VNet peering.)

Azure Standard firewall ဖြန့်ချိရန် အဆင်သင့်ဖြစ်သည့် အရင်းအမြစ်အုပ်စုအသစ်အတွင်းရှိ Service_Test_Network သို့ VNet peering ပါသော hub network တစ်ခုကို ဖန်တီးပါ။ hub တစ်ခုကို မည်သို့ ဖန်တီးပြီး VNet peering ကို မည်သို့ လုပ်ဆောင်ရမည်ကို သတိရစေရန် [အရင်းအမြစ်အုပ်စုနှင့် VNet ဖန်တီးခြင်း](link_to_vnet_creation_activity) လုပ်ဆောင်ချက်သည် သင့်အား ကူညီပေးပါမည်။

1.  Azure ပင်မစာမျက်နှာတွင်၊ အရင်းအမြစ်အုပ်စုများ ဝန်ဆောင်မှုကို ရှာဖွေပြီး ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/OQ9iGoLwTBK_vVkSqoCY7w_567c6e7289c947d191e8df30473cb7e1_image.png?expiry=1744070400000&hmac=lomt4Wm3K_OQi8FLW6ESixYIbcgFLkuzmpmsJtR1Mkg">

2.  **ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/VXB4qQ1qT_K4uV_6xw9Awg_eb7a5012d17e4643b9c306c31a17e6e1_image.png?expiry=1744070400000&hmac=bl9w7_TAkila_ABv2KAH9eXo_0urvMu8LnJsNKCw1sY">

3.  အောက်ပါ အသေးစိတ်များကို ရွေးချယ်ပါ-
    - အရင်းအမြစ်အုပ်စု- "Service_Security"
    - Virtual network အမည်- "Services_Hub"
4.  **ပြန်လည်သုံးသပ်ပြီး ဖန်တီးပါ** ကို ရွေးချယ်ပြီးနောက် **ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/DktAu4VLTHKBr8QmmoJrlA_60a9f23a14cf4d2d8245acad8ece26e1_image.png?expiry=1744070400000&hmac=1PtMxHczeZk-N9oiptGSFlz3s58DlfplVUEY8rTV_-U">

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/_dYe176IRCOFvoLSCSSz0w_35d2c563c6034b18ba1991eebf4454e1_image.png?expiry=1744070400000&hmac=ueZBnrAPA3oxguqUrd_AGxuz4dmz2w5F8b86Ug3RTUo">

5.  ဘယ်ဘက်အပေါ်ထောင့်ရှိ **ပင်မ** ကို ရွေးချယ်ခြင်းဖြင့် Azure ပင်မစာမျက်နှာသို့ ပြန်သွားပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/r7gFY-K2Q1e-h36aUv5xrA_037f6e7c6e5d463289f57f6396aef2e1_image.png?expiry=1744070400000&hmac=Na_OKJ5gZcUNuyj85KeyXRU9zLSqAJQDvQr7H2bnjko">

6.  Azure ပင်မစာမျက်နှာတွင် Virtual networks ကို ရှာဖွေပြီး Virtual networks ဝန်ဆောင်မှုကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/ZHv5NJHJT6OxPJsCdNclAQ_f52388b389fb436dbe7ad6c9040cc2e1_image.png?expiry=1744070400000&hmac=1Mp8Zl4xXhlQ608_oRk4u6IE95stb6Db33oa5Ep-NiI">

7.  **ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/muxu_GqzRfqsID09Rk74MA_fe5731d797574cbc98e328b291fc3be1_image.png?expiry=1744070400000&hmac=F1gXmnTb41COjUp7v1_nZimBAduWBMd__jzysQH8KQ4">

8.  သင်၏ subscription နှင့် အရင်းအမြစ်အုပ်စု Services_Security ကို ရွေးချယ်ပါ။
9.  **နောက်တစ်ခု** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Q97oC7-iQsCND9TkLE3L_g_f558bfbccfbb4e178c0c4cc63b538ee1_image.png?expiry=1744070400000&hmac=YQ08kcQnMaRj38nY9Ug7fPlKRkNfSKFTSLs9ca_wh64">

10. **နောက်တစ်ခု** ကို ထပ်မံရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/YIQEGnG0T6OHxNnshgSjgA_3d270c543d784144a327adb49b9299e1_image.png?expiry=1744070400000&hmac=ZpyzPzmE9pIMBFP1eZDmeD_TvTw5dkrKvpzCXbyLKfU">

11. 192.168.1.0 ကို ထည့်သွင်းခြင်းဖြင့် IP လိပ်စာ နေရာကို တည်းဖြတ်ပြီး လိပ်စာ နေရာ အရွယ်အစားအတွက် /24 ကို ထည့်သွင်းပါ။
12. Subnets အောက်တွင် default ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Tu_jg64gRhK9PAL325nbhA_a763c2e19523487093072746e347dfe1_image.png?expiry=1744070400000&hmac=Cvl0ej6DqjTh0xYo0N6Y5aNjn4Lziwoc4YzbXfx4Fzo">

13. subnet template ကို ဖြည့်စွက်ပါ- Azure Firewall။
14. လိပ်စာအသစ် စတင်ခြင်း- 192.168.1.0 ကို ဖြည့်စွက်ပါ။
15. **သိမ်းဆည်းပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/LFrFtyHGRqOXLavD5wrFIQ_a1c0b49bd45a49058c5030c84df203e1_image.png?expiry=1744070400000&hmac=Fcm6CZ0NX7g_33CRNiYL4_blkwWhlKcIXIJbrxoZRG0">

16. **ပြန်လည်သုံးသပ်ပြီး ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/yghu13zkSmS-LOSKiZtrdA_185c954ba37544e686675fa59396d0e1_image.png?expiry=1744070400000&hmac=aYj8OQ67Ns3BXDUSHvhwYbB0nT3GepQt-vfsGdQA4go">

17. **ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/u8dtuN3-S7yaJS-Q4kEp3g_18a34ed4aa8a4a7a939c08a45cf11ce1_image.png?expiry=1744070400000&hmac=i-ACIvaykXxrx6I4nyBz_38WbzuXV4oLxaFrC_75w-s">

18. **အရင်းအမြစ်သို့ သွားပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/pmLW1pTiRmibbq6vKPKHLw_8cf3ebaa25c54c11b33ae602f38b3fe1_image.png?expiry=1744070400000&hmac=iqzkVSxQAYvRqwzObK_l5p4o8xTuicr_ilhJ89k7NXY">

19. စာမျက်နှာ၏ ဘယ်ဘက် သို့မဟုတ် ညာဘက်ခြမ်းတွင် **Peerings** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/W_k2N3sNSFuXBP_GUAUPxg_05c8285decf24eef8811bb0272fe83e1_image.png?expiry=1744070400000&hmac=WYcwdvAQBmZ8G7FPhImQVLFcRzNQo6qbhfKav1dubXw">

20. peering အသစ်တစ်ခု ထည့်ရန် **ထည့်ပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/nJs4MPdAQdmy4UMa-5BuVA_a40a1f67891540b29d108ba40aae29e1_image.png?expiry=1744070400000&hmac=nG89yWEqCZQ3oAVHuPVAQwcaha4jCemPkN1pNFRe0s4">

21. peering ကို "Hub_Test" ဟု အမည်ပေးပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/gkw0IV1hTVWlNl1qjc-Phg_0f51e5fdab0448c6857d18a7ad8421e1_image.png?expiry=1744070400000&hmac=HABkRudwZtjCL5ehJKGjIsmS9sqxrw0y5gxqMnfraUo">

22. အောက်သို့ ဆင်းပါ၊ ပုံသေဆက်တင်များကို ထားခဲ့ပြီး Peering link အမည်အောက်တွင် "Test_Hub" ဟု ရိုက်ထည့်ပါ။
23. Virtual network dropdown အောက်တွင် Services_Test_Network ကို ရွေးချယ်ပါ။
24. **ထည့်ပါ** ကို ရွေးချယ်ပြီး ကွန်ရက် peering ကို တည်ဆောက်ပါမည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/jqTy0ZStRMu0WeSztDIJaw_527449eabde544ecba4ce101c21bfce1_image.png?expiry=1744070400000&hmac=v-FrMtsBhI_d3xElwhKpIwMr3aBuL1878BEiytX507c">

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/hadqQNFQSvSGInrX-eg0Vw_218e4ea7337049d089a6d732e3c178e1_image.png?expiry=1744070400000&hmac=Dx-4s4Yxu8pPWRHd4pBWKP6E1Br8M9vj4DORnjNaGWk">

### အဆင့် ၃- Azure Standard Firewall ဖြန့်ချိခြင်း (Step 3: Azure Standard Firewall deployment)

hub network အတွင်း Azure Standard Firewall တစ်ခုကို ဖြန့်ချိပါ။ firewall တစ်ခု ဖြန့်ချိသည့်အခါ လုပ်ဆောင်ရန် လိုအပ်သည့် အဆင့်များအားလုံးကို သင့်အား သတိရစေရန် [Azure Firewall ဖြန့်ချိခြင်း](link_to_firewall_deployment_video) ဗီဒီယိုကို ပြန်လည်ကြည့်ရှုပါ။

1.  firewalls များကို ရှာဖွေပြီး **Firewalls** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/VQZImzRgTY66Cmvj5v5Qfg_a5925386ce1e41199006f44ab84883e1_image.png?expiry=1744070400000&hmac=RS30aAaUH2GbPzKYwg5bNeWfnYOmcKsW19t3JWOCemM">

2.  **Firewall ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/tVs3NraNTXGkTxn0AjK9Sw_a7ba4965433e452293d4393c04ba95e1_image.png?expiry=1744070400000&hmac=FyUWQ5iMdVPw7bq-v6s86oB39OX2WEv73iB6g2-X27E">

3.  အောက်ပါ အသေးစိတ်များကို ဖြည့်စွက်ပါ-

    - Subscription: သင်၏ subscription ကို ရွေးချယ်ပါ။
    - အရင်းအမြစ်အုပ်စု- Services_Security
    - firewall instance ကို "ServicesFirewall" ဟု အမည်ပေးပါ။
    - ဒေသ- သင် ယခင်က အသုံးပြုခဲ့သည့် တည်နေရာကို ရွေးချယ်ပါ။
    - <img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/tXsDSHKuSLKbBrDEgAuAHA_7060023fcdef4ba7b504d0eabec35ee1_image.png?expiry=1744070400000&hmac=INdsTfM2gW-45JtUS9qImoyxGBukFhM8LUd-iiyAR30">
    - Firewall SKU: Standard ကို ရွေးချယ်ပါ။
    - Firewall စီမံခန့်ခွဲမှု- ဤ firewall ကို စီမံခန့်ခွဲရန် Firewall စည်းမျဉ်းများ (ဂန္ထဝင်) ကို အသုံးပြုပါ။
    - Virtual network: ရှိပြီးသားကို အသုံးပြုပါ ကို ရွေးချယ်ပြီး Services_Security_Network ကို ရွေးချယ်ပါ။
    - အများသုံး IP လိပ်စာအတွက် အသစ် ထည့်ပါ ကို ရွေးချယ်ပြီး "Services" ဟု အမည်ပေးပါ။

4.  **ပြန်လည်သုံးသပ်ပြီး ဖန်တီးပါ** ကို နှိပ်ပြီးနောက် **ဖန်တီးပါ** ကို နှိပ်ပါက firewall ကို ဖြန့်ချိပါမည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/N_du23zsQZmvJbWKkvy4Tg_537535b30f21442d920317636c9a0de1_image.png?expiry=1744070400000&hmac=uWg-0teg5Q1O6bRHhQbsC15u78xbaGJb7ZV365eJmMc">

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/wMShQ4S3QAGXTJs0Wwyjig_62b10e6f4c5d43b3b970e0cde9ab9ce1_image.png?expiry=1744070400000&hmac=iuUyRrJfBZd2uMdfx54Xr9vrlr31NS0FladkiAvXwXI">

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/DDwF4odqTNKvvSVQy5WVdQ_4ae37768674a4e36b47d2179e7acaae1_image.png?expiry=1744070400000&hmac=qdoz6ctvyieXoSAOQB1WHeNwL0D_ukYmG_K14tDw8uQ">

### အဆင့် ၄- Just-in-time access (JIT) တည်ဆောက်ခြင်း (Step 4: Just-in-time access (JIT) setup)

Services_VM တွင် JIT access ကို ဖွင့်ပါ။ RDP access ကို ပုံသေအားဖြင့် ဖွင့်ထားပါသည်။ JIT access ကို ဖွင့်ရန် အဆင့်များကို သင့်အား သတိရစေရန် [Just-in-time access အကောင်အထည်ဖော်ခြင်း](link_to_jit_video) ဗီဒီယိုကို ပြန်လည်ကြည့်ရှုပါ။

1.  **Virtual machines** ကို ရှာဖွေပြီး ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/gD3BhO5bTvutp1qJOFOxuw_3f5bfee746a642149e0def22935c7ae1_image.png?expiry=1744070400000&hmac=SC-JnZlNQG7UjaOiThctzpd8lFZQ6LrbTszp_g7g3aY">

2.  Services_VM virtual machine ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/vuECjiBXRYKOXZ5Kohgtsw_d3623e85cce443e2a3f1d0ce48bcaee1_image.png?expiry=1744070400000&hmac=Zuey_Oux5GoAj6mxYDc0hK4c44D2USfBfb30rephGyc">

3.  ဘယ်ဘက်ခြမ်း မီနူးမှ **ဖွဲ့စည်းပုံ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/IJ2_2C8zRwuE4yhW_ZMyHA_b243b11617954e79acf555271e3d67e1_image.png?expiry=1744070400000&hmac=XawHt_ReD8DlsDZ2AHC_mqs5NbI5bkkHIL5r-v2MWKo">

4.  **Just-in-time ဖွင့်ပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/SKE7X5IJTtaBIPo0MiWkPw_072b60ca867d4a4e808d017d0186fbe1_image.png?expiry=1744070400000&hmac=Wkd0DXnotxjhm32GvRT4zIJh93CPOzWHyHhHLwdtZg0">

### အဆင့် ၅- Azure Bastion ဖွဲ့စည်းပုံ (Step 5: Azure Bastion configuration)

ServicesVM အတွက် Azure Bastion ကို ဖွဲ့စည်းပါ။ အဆင့်များကို သင့်အား သတိရစေရန် [Bastion နှင့် virtual machines](link_to_bastion_video) ဗီဒီယိုကို ပြန်လည်ကြည့်ရှုပါ။

1.  ရှာဖွေရေးဘားကို အသုံးပြုပြီး **Virtual networks** ကို ရှာဖွေပြီး **Virtual networks** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/TLJUU3ldSaSPXCxSLSsVNw_085ab34d866b4edd9e6e6b0611eb66e1_image.png?expiry=1744070400000&hmac=fccSyYn__EIwWn3ACA7OJdpEgry0Fxajqo51kZwdhMY">

2.  Services_Test_Network network ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/XnrjLOLZRdWpW88e7VQGMg_75b242017b4c4fd194cf30ebe14fe0e1_image.png?expiry=1744070400000&hmac=i3evKZNRLZXqdsEp6KZwunZ5Gos1LsHkEvj5Y5kC-mM">

3.  virtual network အတွက် စာမျက်နှာတွင်၊ Bastion စာမျက်နှာကို ဖွင့်ရန် ဘယ်ဘက်အကန့်တွင် **Bastion** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/T1EQRbIDTUKdpEB0tqxbcg_10f1d8f2604f4da1a3f978dca8085be1_image.png?expiry=1744070400000&hmac=bpNB_NIpCYdhPJCibU7VEwcwMnuxMGXo7lEGFPtIvic">

4.  Bastion စာမျက်နှာတွင် **ကိုယ်တိုင် ဖွဲ့စည်းပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/6TcbDCmnTKqLwPCD51CGsw_aac1e2bcd0fe4327ad77082de74820e1_image.png?expiry=1744070400000&hmac=AYUmQ63LPTt_cMRCgO3sf0vSwmHx7Up4D_yX9CprsVs">

5.  Bastion ဖန်တီးခြင်း စာမျက်နှာတွင် အောက်ပါ ဆက်တင်များကို အသုံးပြုပါ-

    - Instance အမည်- "Services_Bastion"။
    - Virtual network: "Services_Test_Network".

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/pFUephj9R2aR79tTHjQ5rw_f746c28a9ef64a1993edd3e5934656e1_image.png?expiry=1744070400000&hmac=KxXN3Thc1fuXN96aqqqTj9HDThoFEOJG-VzVy1eeQF4">

6.  အောက်သို့ ဆင်းပြီး AzureBastionSubnet ကို ဖွဲ့စည်းရန် **Subnet ဖွဲ့စည်းပုံကို စီမံပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/a0JnSNc_TsyOhrKbCqKQ7A_251ede39b95f4eec90103dd396c94ce1_image.png?expiry=1744070400000&hmac=JZC8EKCpgk4Ksi6SC3CW1aoVto6JP5TSsJOXY3xIYfk">

7.  subnets စာမျက်နှာတွင် **+ Subnet** ကို ရွေးချယ်ပါ။

<img src="![Subnet ထည့်ပါ](add_subnet.png) _(add_subnet.png ကို သင်၏ တကယ့် ဖန်သားပြင်ဓာတ်ပုံ သို့မဟုတ် နေရာပြပုံဖြင့် အစားထိုးပါ)_">

8.  အောက်ပါ တန်ဖိုးများကို အသုံးပြု၍ AzureBastionSubnet subnet ကို ဖန်တီးပါ။

    - Subnet အမည်- "AzureBastionSubnet"။
    - Subnet လိပ်စာ နေရာ- 172.16.2.0/24။
    - သင်၏ တန်ဖိုးများကို သိမ်းဆည်းရန် စာမျက်နှာ၏ အောက်ခြေရှိ **သိမ်းဆည်းပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/IcGBKO24T7OlUwI7EUasQg_ef570bcacf0b4902adcee72686d8f5e1_image.png?expiry=1744070400000&hmac=SbbOQ-4xc3imsmG6jMpFoTBu9NfSqN3mbUDQ5zwC9RY">

9.  Subnets စာမျက်နှာ၏ အပေါ်ဆုံးတွင် Bastion ဖွဲ့စည်းပုံ စာမျက်နှာသို့ ပြန်သွားရန် **Bastion ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/PYJti3N1SO6FI1Agt6PcUg_401a4220bff24c6685e64d5c96bb55e1_image.png?expiry=1744070400000&hmac=8rbZxDA7ACdAuEkco7cH9wUlI_SG99bDcj471GBzTuw">

10. အများသုံး IP လိပ်စာအောက်တွင် **အသစ် ဖန်တီးပါ** ကို ရွေးချယ်ပါ။ ပုံသေ အမည်ပေးခြင်း အကြံပြုချက်ကို ထားခဲ့ပါ။ **ပြန်လည်သုံးသပ်ပြီး ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/ssgswyCESmOvifbTsgLnUQ_6e09a81dd5c644fdb820e0148fdd07e1_image.png?expiry=1744070400000&hmac=fRPOui4CrL3UQx-kkmgvqarhNqFeoAoybuPekIdu4Xk">

11. **ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/jmg3kcVAT_iWXzNRY4p1Cg_be823c6ab1b34784b3efc5b18f0ae6e1_image.png?expiry=1744070400000&hmac=sYnaeKYD296mkRfarIS0tRsrXPI3H7a4CSxIEzYhDJY">

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/F9sdEELnQOCMdogFZ6J3iA_fc911a9ba6eb4ef6a41d77d834df71e1_image.png?expiry=1744070400000&hmac=c2ik9U1xKbdF5eaAiHLS1KIAz34vrwKZliwQfRLP23s">

### အဆင့် ၆- အဝေးမှ ချိတ်ဆက်မှုကို စမ်းသပ်ခြင်း (Step 6: Testing remote connectivity)

ဖြန့်ချိမှု အလုပ်လုပ်ကြောင်း အတည်ပြုရန် JIT ပါသော Azure Bastion ကို အသုံးပြုပြီး RDP ကို အသုံးပြု၍ Services VM သို့ ချိတ်ဆက်ပါ။ အဆင့်များကို သင့်အား သတိရစေရန် [Bastion နှင့် virtual machines](link_to_bastion_video) ဗီဒီယိုကို ပြန်လည်ကြည့်ရှုပါ။

1.  **Virtual machines** ကို ရှာဖွေပြီး ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/AiDjSEEPSH6lXpd93sDG2w_21237d7dd9f4450c9f444bb7f24e5ce1_image.png?expiry=1744070400000&hmac=J0c-H4OzDnCZ_OCjHjNRNCfxRmMc-Y-cUeNMZvQNZvs">

2.  Services_VM ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/40UkvAojTb6TJFiXaUOGMw_57a85800f1954c31bba37d84ede55de1_image.png?expiry=1744070400000&hmac=B6T46k1KAG4KfjG1zsHopVBn6L-2Qk3F-xkE81-24Vk">

3.  စာမျက်နှာ၏ အပေါ်ဆုံးတွင် **ချိတ်ဆက်ပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/bd3ZftftQBa3YQc1BRKooQ_79375bc94d66437e9eaecddc58ca97e1_image.png?expiry=1744070400000&hmac=zl93g3EDyA6igK6P8Y5ujDP12hdNpfvXQ35lpbS4cUo">

4.  ညာဘက် scroll bar တွင် အောက်သို့ ဆင်းပြီး **access တောင်းဆိုပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/1w7UoJztTG6IxAM8s85dGQ_347658b493e740d68407d6b0336ae1e1_image.png?expiry=1744070400000&hmac=hKt6Oc1db12pNQIEPeXe6LQX49pR6YAgR9g7xxoxJ0A">

5.  စာမျက်နှာ၏ အပေါ်ဆုံးတွင် Bastion စာမျက်နှာသို့ သွားရန် **Bastion** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/WsHzKZ3BQ2i-7MnAMlz1oA_3fb126afe9cd40ceac7e4b97e7e841e1_image.png?expiry=1744070400000&hmac=K8IToq8mwSe3P4wyXgSgiaVskyT-TBdhK0SU8NAS_Xg">

6.  **Bastion ကို အသုံးပြုပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/h2zdzUjuQDq2QVAlvEq-hA_4258269376d54d8aba8388fe5f748ce1_image.png?expiry=1744070400000&hmac=qqwTGQrQvImePVKMSPu0pH4XNhBUeQ5kY8DjfMvh-MM">

7.  Services_VM အတွက် လိုအပ်သော အထောက်အထား တန်ဖိုးများကို ဖြည့်စွက်ပါ-
    - Username AzAdmin
    - Password P@$$@1234567
8.  VM သို့ ချိတ်ဆက်ရန် **ချိတ်ဆက်ပါ** ကို နှိပ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/T_KaYR02Rn6mxEgzW_uw6g_43b4dbf2bc2b4ed4be5a7b62d5f4fae1_image.png?expiry=1744070400000&hmac=39ovUWDxJpJJPHOS5ybWa_M9ijbeo_J6mAKBVo8jIO0">

Bastion မှတစ်ဆင့် ဤ virtual machine သို့ ချိတ်ဆက်မှုသည် port 443 နှင့် Bastion ဝန်ဆောင်မှုကို အသုံးပြု၍ Azure portal တွင် (HTML5 မှတစ်ဆင့်) တိုက်ရိုက် ဖွင့်ပါမည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/7RTFK0PJS6mEx5petYIGgQ_02b5aca158004f9e84c2a942b16f2ae1_image.png?expiry=1744070400000&hmac=F9T52-DRPbqSWAKWs1vibf_WMNOxHFR4qLCjvpW_NOk">

### အဆင့် ၇- Microsoft Sentinel အကောင်အထည်ဖော်ခြင်း (Step 7: Implement Microsoft Sentinel)

စမ်းသပ်ခြင်းနှင့် လေ့ကျင့်ခြင်းအတွက် အဆင်သင့်ဖြစ်သည့် Microsoft Sentinel ကို အကောင်အထည်ဖော်ပါ။ အဆင့်များကို သင့်အား သတိရစေရန် [Microsoft Sentinel](link_to_sentinel_video) ဗီဒီယိုကို ပြန်လည်ကြည့်ရှုပါ။ ၎င်းကို ပြုလုပ်ရန် အဆင့်များကို သင့်အား သတိရစေရန် [Microsoft Sentinel](link_to_sentinel_video) ဗီဒီယိုကို ပြန်လည်ကြည့်ရှုပါ။

1.  Azure portal ပင်မစာမျက်နှာမှ Microsoft Sentinel ကို ရှာဖွေပြီး ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/3Yl9TCRpTNazVxOQMM-iKw_3abc6f2f9e424cc1b5822475cb108de1_image.png?expiry=1744070400000&hmac=Xub2KexqM0XsC5YpIeAzCGXKdUKxKiNVUP22sgFjc40">

2.  **Microsoft Sentinel ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/A6Sx6UZ8RHeyP_uMUauYsQ_6e0545ba83624b1080633271ec4ae5e1_image.png?expiry=1744070400000&hmac=R9lETId2vbGdBVhymJ82xW_p9QuacanfAxl0Hnxciuw">

3.  **workspace အသစ် ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/qP_TBNF2R5m9C5plIsgH4w_b00e3b7383a04796b758f7bc1fee10e1_image.png?expiry=1744070400000&hmac=luEB4lrBmTZEKcHLdb_MaKcpUTd0fkbfY8OOBuSrcc0">

4.  log analytics workspace အတွက် အောက်ပါ ဖြန့်ချိမှု အသေးစိတ်များကို ဖြည့်စွက်ပါ။ သင်၏ လက်ရှိ subscription ကို ရွေးချယ်ပြီး ဖြစ်ပါမည်။
    - အရင်းအမြစ်အုပ်စု- "Services_Test"
    - Instance အမည်- "ServiceSentinel"
5.  **ပြန်လည်သုံးသပ်ပြီး ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/lIf3SsxOQxSS0lKSFA-8Jw_a06bb1bfb35d473cb328cd12b24560e1_image.png?expiry=1744070400000&hmac=sxGHvvLifQHZnE6dslhWkWFEMPRFuMoNcbeLwss31gw">

6.  **ဖန်တီးပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Uj_Y_b-7QjK4QN808F3Itw_901ee598e6094d05b70cb22c3669d4e1_image.png?expiry=1744070400000&hmac=mvuP4ySAA8-i8-WQ8hOeOl2aoLGatIU9uPwE8yG8-Cw">

7.  စက္ကန့်အနည်းငယ်ကြာပြီးနောက် workspace အသစ်တစ်ခုကို ဖန်တီးပါမည်။ Service_Sentinel ကို ရွေးချယ်ပါ။
8.  **ထည့်ပါ** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/jXAHq0jEQTShYvyHaeqMVA_04faac4045254d62936d82a6f06050e1_image.png?expiry=1744070400000&hmac=-yF8Rp581Y8WfU_Z1sBh3alISScuE2NI7VUMw380Tps">

9.  Microsoft Sentinel အခမဲ့ အစမ်းသုံးရန် **OK** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/xQUZ3eJ-R_2M1twm4iLIfA_dae19144709c42f9855fd1fbe5cdc6e1_image.png?expiry=1744070400000&hmac=kFLkVLv7VPfMwHNiIA0S9vGY1UduT7YdcNd6j2Lk0Bk">

## ရှင်းလင်းခြင်း (Clean-up)

သင်သည် သင်၏ ကိုယ်ပိုင် Azure subscription ကို အသုံးပြုနေပါက၊ သင်ခန်းစာတစ်ခုစီကို ပြီးမြောက်ပြီးနောက် compute အရင်းအမြစ်များကို ရပ်တန့်ရန် ရှင်းလင်းခြင်း ညွှန်ကြားချက်များကို လိုက်နာရန် အကြံပြုအပ်ပါသည်။ သင်သည် သင်၏ ကိုယ်ပိုင် subscription တွင် လုပ်ဆောင်နေပါက၊ ပရောဂျက်တစ်ခု၏ အဆုံးတွင် သင်ဖန်တီးထားသော အရင်းအမြစ်များကို သင် ဆက်လက်လိုအပ်သေးခြင်း ရှိမရှိကို ခွဲခြားသတ်မှတ်ရန်လည်း ကောင်းမွန်ပါသည်။ ဆက်လက်လည်ပတ်နေသည့် အရင်းအမြစ်များသည် သင့်အား ငွေကုန်ကျစေနိုင်ပါသည်။ သင်သည် အရင်းအမြစ်များကို တစ်ဦးချင်း ဖျက်နိုင်သည် သို့မဟုတ် အရင်းအမြစ် အစုံလိုက်ကို ဖျက်ရန် အရင်းအမြစ်အုပ်စုကို ဖျက်နိုင်ပါသည်။

လေ့ကျင့်ခန်းကို ပြီးမြောက်ပြီးနောက် အရင်းအမြစ်များကို မည်သို့ ဖျက်ရမည်ကို ညွှန်ကြားချက်များအတွက် [အရင်းအမြစ်များကို ရှင်းလင်းပါ](link_to_cleanup_reading) စာဖတ်ခြင်းကို ကြည့်ရှုပါ။

Standard Firewall ကိုလည်း ပါဝါပိတ်၍မရသောကြောင့် ဖျက်ရန် မမေ့ပါနှင့်။ ၎င်းသည် အသက်ဝင်နေပါက သင့်အား ဆက်လက် ကောက်ခံမည်ဖြစ်သည်။

## နိဂုံး (Conclusion)

ဤနောက်ဆုံး သင်တန်း ပရောဂျက်ကို ပြီးမြောက်ခြင်းသည် virtual machines များကို လုံခြုံစေခြင်းအကြောင်း သင်လေ့လာခဲ့သည့်အရာကို လက်တွေ့ကျင့်သုံးရန် သင့်အား ခွင့်ပြုခဲ့ပါသည်။ အသေးစားလုပ်ငန်းတစ်ခုအတွက် စမ်းသပ်ပတ်ဝန်းကျင်တစ်ခု တည်ဆောက်ခြင်းဖြင့် သင်သည် အဓိက Microsoft ဝန်ဆောင်မှုများကို မည်သို့ ဖွဲ့စည်းကာ ဖြန့်ချိရမည်ကို သင်၏ နားလည်မှုကို သရုပ်ပြခဲ့ပါသည်။ သင်သည် virtual machine တစ်ခုကို မည်သို့ ဖြန့်ချိရမည်ကို ဦးစွာ သရုပ်ပြခဲ့ပြီးနောက် Azure firewall တစ်ခု ဖြန့်ချိခြင်းဖြင့် ကွန်ရက်ကို ကာကွယ်ရန် ဆက်လက်လုပ်ဆောင်ခဲ့ပါသည်။ ထို့နောက် JIT နှင့် Azure Bastion တို့ကို ပေါင်းစပ်အသုံးပြုခြင်းဖြင့် ထို VM ရှိ စီမံခန့်ခွဲမှု port များကို မည်သို့ ကာကွယ်ရမည်ကို သရုပ်ပြခဲ့ပါသည်။ နောက်ဆုံးတွင် အနာဂတ်တွင် မတူညီသော ဒေတာ ချိတ်ဆက်ကိရိယာများကို ထည့်ရန် အဆင်သင့်ဖြစ်သည့် Microsoft Sentinel ကို မည်သို့ ဖြန့်ချိရမည်ကို သရုပ်ပြခဲ့ပါသည်။
