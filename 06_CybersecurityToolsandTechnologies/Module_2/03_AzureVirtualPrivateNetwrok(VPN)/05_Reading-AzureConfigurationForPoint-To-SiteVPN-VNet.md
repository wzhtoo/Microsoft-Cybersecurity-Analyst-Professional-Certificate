# Azure configuration for Point-to-Site VPN: VNet

[Azure configuration for Point-to-Site VPN: VNet 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/supplement/EuNbr/azure-configuration-for-point-to-site-vpn-vnet)

# Point-to-Site VPN အတွက် Azure ဖွဲ့စည်းမှု- VNet (Azure Configuration for Point-to-Site VPN: VNet)

**နိဒါန်း (Introduction)**

သင်၏ on-premises ကွန်ရက်နှင့် virtual network (VNet) ကြား point-to-site VPN ဂိတ်ဝေး ချိတ်ဆက်မှုကို ဖန်တီးရန် Azure portal ကို မည်သို့ အသုံးပြုရမည်ကို ဖော်ပြထားသော သုံးပိုင်းပါ စာဖတ်ခြင်း၏ ပထမပိုင်းသို့ ကြိုဆိုပါသည်။

ဤစာဖတ်ခြင်းတွင် Azure တွင် လုံခြုံပြီး ယုံကြည်စိတ်ချရသော virtual network (VNet) ကို ဖန်တီးနည်းကို သင် လေ့လာပါမည်။

ဤစာဖတ်ခြင်းသည် စမ်းသပ် ပတ်ဝန်းကျင်ကို ဖန်တီးရန်အတွက် အောက်ပါ တန်ဖိုးများကို အသုံးပြုပါသည်။

- VNet အမည်: VNet1
- လိပ်စာ နေရာ: 10.1.0.0/16 ဤဥပမာတွင် လိပ်စာ နေရာ တစ်ခုသာ ရှိပါသည်။ သင်၏ VNet အတွက် လိပ်စာ နေရာ တစ်ခုထက်ပို၍ ရှိနိုင်ပါသည်။
- Subnet အမည်: FrontEnd
- Subnet လိပ်စာ အပိုင်းအခြား: 10.1.0.0/24
- စာရင်းသွင်းခြင်း: စာရင်းသွင်းခြင်း တစ်ခုထက်ပို၍ ရှိပါက သင် မှန်ကန်သော တစ်ခုကို အသုံးပြုနေကြောင်း အတည်ပြုပါ။
- အရင်းအမြစ် အုပ်စု: TestRG1
- တည်နေရာ: အရှေ့ပိုင်း US

ဤဖွဲ့စည်းမှုအတွက် အသုံးပြုရန် အကြံပြုထားသော တန်ဖိုးများအတွက် VNet ဥပမာ တန်ဖိုးများ အပိုင်းကို ရည်ညွှန်းပါ။

1.  Azure portal သို့ ဆိုင်းအင်ဝင်ပါ (Sign in to the Azure portal)။
2.  အရင်းအမြစ်များ၊ ဝန်ဆောင်မှုနှင့် စာရွက်စာတမ်းများကို ရှာဖွေပါ (G+/) တွင် virtual network ဟု ရိုက်ထည့်ပါ။
3.  Virtual network စာမျက်နှာကို ဖွင့်ရန် Marketplace ရလဒ်များမှ Virtual network ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/a3876Kg6SE2KOulUSl_nAw_d6ce420431494e53b91e317459a064e1_image.png?expiry=1744156800000&hmac=j7_lO9dAIpZHYYN3le3yp3LpsCUYUKNDXJXtMdEbydU">

4.  Virtual network စာမျက်နှာတွင် ဖန်တီးပါ (Create) ကို ရွေးချယ်ပါ။ ၎င်းသည် virtual network ဖန်တီးပါ (Create virtual network) စာမျက်နှာကို ဖွင့်ပေးပါသည်။
5.  အခြေခံများ (Basics) တက်ဘ်တွင် ပရောဂျက် အသေးစိတ်များ (Project details) နှင့် ဥပမာ အသေးစိတ်များ (Instance details) အတွက် VNet ဆက်တင်များကို ဖွဲ့စည်းပါ။ သင် ထည့်သွင်းသည့် တန်ဖိုးများကို အတည်ပြုသောအခါ အစိမ်းရောင် အမှတ်အသားကို သင် သတိပြုမိပါလိမ့်မည်။ သင် လိုအပ်သည့် ဆက်တင်များအရ တန်ဖိုးများကို ချိန်ညှိနိုင်ပါသည်။
    - စာရင်းသွင်းခြင်း (Subscription): ဖော်ပြထားသော စာရင်းသွင်းခြင်းသည် မှန်ကန်ကြောင်း အတည်ပြုပါ။ သင်သည် drop-down ကို အသုံးပြု၍ စာရင်းသွင်းခြင်းများကို ပြောင်းလဲနိုင်ပါသည်။
    - အရင်းအမြစ် အုပ်စု (Resource group): တည်ရှိနေသော အရင်းအမြစ် အုပ်စုကို ရွေးချယ်ပါ သို့မဟုတ် အသစ် ဖန်တီးရန်အတွက် အသစ် ဖန်တီးပါ (Create new) ကို ရွေးချယ်ပါ။
    - အမည် (Name): သင်၏ virtual network အတွက် အမည်ကို ရိုက်ထည့်ပါ။
    - ဒေသ (Region): သင်၏ VNet အတွက် တည်နေရာကို ရွေးချယ်ပါ။ တည်နေရာသည် ဤ VNet သို့ သင် ဖြန့်ကျက်သည့် အရင်းအမြစ်များ တည်ရှိမည့်နေရာကို ဆုံးဖြတ်ပေးပါသည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Aw1tf2p0SU6Hj8YORyq-YQ_ba2cecc2c0a14b5881a63ed0cb4f64e1_image.png?expiry=1744156800000&hmac=dvygEOACziUdfNVkkgDEPtOl_qxLpU_uhJDkP3Ca9IQ">

6.  လုံခြုံရေး (Security) ကို ရွေးချယ်၍ လုံခြုံရေး (Security) တက်ဘ်သို့ ဆက်သွားပါ။ ဤသရုပ်ပြအတွက် ဤစာမျက်နှာရှိ ဝန်ဆောင်မှုများအားလုံးအတွက် မူရင်း တန်ဖိုးများကို ထားခဲ့ပါ။
7.  IP လိပ်စာများ (IP Addresses) ကို ရွေးချယ်၍ IP လိပ်စာများ (IP Addresses) တက်ဘ်သို့ ဆက်သွားပါ။
8.  IP လိပ်စာများ (IP Addresses) တက်ဘ်တွင် ဆက်တင်များကို ဖွဲ့စည်းပါ:
    - IPv4 လိပ်စာ နေရာ (IPv4 address space): မူရင်းအားဖြင့် လိပ်စာ နေရာကို အလိုအလျောက် ဖန်တီးပါသည်။ သင်သည် လိပ်စာ နေရာကို ရွေးချယ်ပြီး သင်၏ ကိုယ်ပိုင် တန်ဖိုးများကို ထင်ဟပ်စေရန် ချိန်ညှိနိုင်ပါသည်။ သင်သည် မတူညီသော လိပ်စာ နေရာကိုလည်း ထည့်သွင်းနိုင်ပြီး အလိုအလျောက် ဖန်တီးထားသော မူရင်းကို ဖယ်ရှားနိုင်သည်။ ဥပမာအားဖြင့် သင်သည် စတင်သည့် လိပ်စာကို 10.1.0.0 ဟု သတ်မှတ်ပြီး လိပ်စာ နေရာ အရွယ်အစားကို /16 ဟု သတ်မှတ်ကာ ထို လိပ်စာ နေရာကို ထည့်ပါ (Add)။
    - - Subnet ထည့်ပါ (+ Add subnet): သင်သည် မူရင်း လိပ်စာ နေရာကို အသုံးပြုပါက မူရင်း subnet ကို အလိုအလျောက် ဖန်တီးပါသည်။ သင်သည် လိပ်စာ နေရာကို ပြောင်းလဲပါက ထို လိပ်စာ နေရာအတွင်း အသစ် subnet တစ်ခုကို ထည့်ပါ။ Subnet ထည့်ပါ (+ Add subnet) ကို ရွေးချယ်၍ Subnet ထည့်ပါ (Add subnet) ဝင်းဒိုးကို ဖွင့်ပါ။ အောက်ပါ ဆက်တင်များကို ဖွဲ့စည်းပြီး တန်ဖိုးများကို ထည့်ရန်အတွက် စာမျက်နှာ၏ အောက်ခြေရှိ ထည့်ပါ (Add) ကို ရွေးချယ်ပါ။
        - Subnet အမည် (Subnet name): ဥပမာ- FrontEnd။
        - Subnet လိပ်စာ အပိုင်းအခြား (Subnet address range): ဤ subnet အတွက် လိပ်စာ အပိုင်းအခြား။ ဥပမာ- 10.1.0.0 နှင့် /24။
9.  IP လိပ်စာများ (IP addresses) စာမျက်နှာကို ပြန်လည်သုံးသပ်ပြီး သင် မလိုအပ်သော မည်သည့် လိပ်စာ နေရာများ သို့မဟုတ် subnets များကိုမဆို ဖယ်ရှားပါ။
10. virtual network ဆက်တင်များကို အတည်ပြုရန် ပြန်လည်သုံးသပ် + ဖန်တီးပါ (Review + create) ကို ရွေးချယ်ပါ။
11. ဆက်တင်များကို အတည်ပြုပြီးနောက် virtual network ကို ဖန်တီးရန် ဖန်တီးပါ (Create) ကို ရွေးချယ်ပါ။

သင်၏ အပလီကေးရှင်းများနှင့် အရင်းအမြစ်များအတွက် လုံခြုံသော ပတ်ဝန်းကျင်ကို ထောက်ပံ့ပေးပါသည်။

<video width=100% height=100% controls>
  <source src="https://d3c33hcgiwev3.cloudfront.net/MQw5h9uRQOy2fcLzaVQIrQ_b4fdc8f527b34276a829400000f22ee1_C6M2L3-Item-06--Creating-the-VNet_V3.mp4?Expires=1744156800&Signature=NOEH0HtkVIbz-aqCd9PmyU8QtbO-6NyFoP~7T1MzKA3RjwKOmjoPTVky097PbEsPYJmGskroDEOZj07LfN~x112T5K~j7g~dRQrbOD7yobidNfDm3k97j9zxvo-ezYHRPB4g6tmpMDrdLa1ku-Qrl0JiNfm6iY43bH97kPRQjcs_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A" type="video/mp4">
</video>

**နိဂုံး (Conclusion)**

သင်သည် Azure VPN အတွက် လိုအပ်သော VNet ကို အောင်မြင်စွာ တည်ဆောက်ပြီး ဖြန့်ကျက်ပြီးဖြစ်သည်။ လုံခြုံပြီး စိတ်ကြိုက်ပြင်ဆင်နိုင်သော ကွန်ရက် ပတ်ဝန်းကျင်ကို ဖန်တီးခြင်းဖြင့် သင်သည် သင်၏ အရင်းအမြစ်များသို့ လုံခြုံသော အဝေးမှ ဝင်ရောက်ခွင့်ကို ဖွင့်ပေးရန် တစ်ဆင့် နီးစပ်လာပါပြီ။

နောက်စာဖတ်ခြင်းတွင် ဤ VNet တွင် Azure VPN ဖြန့်ကျက်ခြင်းကို သင် လေ့လာပါမည်။ သင်သည် Azure VPN ဂိတ်ဝေးကို ဖွဲ့စည်းရန်နှင့် သင်၏ ကွန်ရက်သို့ လုံခြုံသော ချိတ်ဆက်မှုများကို တည်ဆောက်ရန် လိုအပ်သော အဆင့်များကို လုပ်ဆောင်ပါမည်။
