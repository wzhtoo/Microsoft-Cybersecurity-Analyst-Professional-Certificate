# JIT and encryption

[JIT and encryption 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/supplement/nqiC7/jit-and-encryption)

## JIT and Encryption (JIT နှင့် ကုဒ်ပြောင်းခြင်း)

### Introduction (မိတ်ဆက်)

ယခင်က သင်သည် Microsoft Azure အတွင်းရှိ ဒေတာသည် အခြေအနေ နှစ်မျိုး - အနားယူအခြေအနေ (at rest) နှင့် သယ်ယူအခြေအနေ (in transit) - တွင် ရှိနိုင်ကြောင်း သင်ယူခဲ့သည်။ ဤအခြေအနေ နှစ်မျိုးအတွက် Microsoft Azure သည် ဒေတာကို လုံခြုံစေရန် မတူညီသော ဖြေရှင်းချက်များနှင့် အကောင်းဆုံး အလေ့အကျင့်များကို ပေးထားသည်။ ဥပမာ၊ VPN၊ TLS၊ MACsec၊ ဆင်မီထရစ် ကုဒ်ပြောင်းခြင်း (symmetric encryption) နှင့် အခြားသော ကုဒ်ပြောင်းနည်းပညာများစွာ ပါဝင်သည်။ ဤနည်းပညာများအားလုံးတွင် ဒေတာကို ကုဒ်ပြောင်းရန် သော့ (key) သို့မဟုတ် လက်မှတ် (certificate) ကို အသုံးပြုထားပြီး၊ ထို့ကြောင့် သင်၏ သော့များကို ဂရုစိုက်ခြင်းနှင့် ကောင်းမွန်သော သော့စီမံခန့်ခွဲမှု လုပ်ငန်းစဉ်ရှိခြင်းသည် ဒေတာကို လုံခြုံစွာ ထိန်းသိမ်းရန် အရေးကြီးသည်။

Sam’s Scoops သည် ၎င်း၏ ဗာ့ချွယ် စက်များသို့ ဝင်ရောက်ခွင့်ကို ကာကွယ်ရန် JIT ကို အသုံးပြုနေသော်လည်း၊ ထိုဒေတာကို ကုဒ်ပြောင်းထားရမည်ဖြစ်ပြီး၊ လုပ်ငန်းအတွက် အက်ပလီကေးရှင်းများ လုပ်ဆောင်ရန် တတိယပုဂ္ဂိုလ် ဖန်တီးသူများ (third-party developers) အား ဝင်ရောက်ခွင့် ပေးထားရမည်။ ဤအတွက် ဖန်တီးသူများသည် သော့များသို့ ဝင်ရောက်ခွင့် လိုအပ်မည်ဖြစ်သည်။

ဤဖတ်ရှုမှုတွင်၊ Azure အတွင်း သော့စီမံခန့်ခွဲမှုအကြောင်း သင်လေ့လာရမည်ဖြစ်ပြီး၊ သော့စီမံခန့်ခွဲမှု လုပ်ငန်းစဉ်တွင် ပါဝင်သော နည်းပညာဆိုင်ရာ အဆင့်များကို ဖော်ထုတ်ရမည်။

### Azure Encryption in Transit and at Rest (Azure တွင် သယ်ယူဒေတာနှင့် အနားယူဒေတာ ကုဒ်ပြောင်းခြင်း)

Sam’s Scoops တွင် ယခုအခါ ဂိုဒေါင်တစ်ခု၊ ဝန်ထမ်းများပါဝင်သော ဆိုင်များစွာ ရှိသည်။ ဝန်ထမ်းများနှင့် ဖောက်သည်များသည် ဒေတာကို ထုတ်လုပ်ပြီး၊ ဖောက်သည် ဒေတာကို လုပ်ငန်းကို စျေးကွက်ချဲ့ထွင်ရန် အသုံးပြုသည်။ ဤဒေတာအားလုံးကို လုံခြုံသော နေရာတစ်ခုတွင် သိမ်းဆည်းထားရန် လိုအပ်သော်လည်း၊ အလွယ်တကူ ဝင်ရောက်နိုင်ရမည်။ ၎င်းကို ဒေတာ အမျိုးအစားနှင့် ဝန်ဆောင်မှုပေါ်မူတည်၍ Azure တစ်လျှောက် မတူညီသော သိုလှောင်မှု အမျိုးအစားများတွင် သိမ်းဆည်းနိုင်သည်။

ဥပမာ၊ Sam’s Scoops သည် ဖိုင်မျှဝေမှု (file share) နှင့် ဝက်ဘ်ဆာဗာကဲ့သို့သော ဗာ့ချွယ် စက်များ၏ လည်ပတ်စနစ်များအတွက် သိုလှောင်မှု လိုအပ်သည်။ ဒေတာကို Azure Disk Encryption ဖြင့် အနားယူဒေတာအဖြစ် ကုဒ်ပြောင်းပြီး လုံခြုံစေနိုင်သော်လည်း၊ ဤဖိုင်များရှိ ဒေတာကို Azure သို့ မရွှေ့မီ ကုဒ်ပြောင်းထားကြောင်း မည်သို့ သေချာစေမည်နည်း။ ဤအတွက် သင်သည် ကလိုင်းယင့်ဘက်ကုဒ်ပြောင်းခြင်း (client-side encryption) သို့မဟုတ် ဆာဗာဘက်ကုဒ်ပြောင်းခြင်း (server-side encryption) ကို အသုံးပြုနိုင်သည်။

#### Client-Side Encryption (ကလိုင်းယင့်ဘက်ကုဒ်ပြောင်းခြင်း)

ကလိုင်းယင့်ဘက်ကုဒ်ပြောင်းခြင်းကို Azure ပြင်ပတွင် လုပ်ဆောင်သည်။ ၎င်းတွင် အောက်ပါတို့ ပါဝင်သည်-

- ဖောက်သည်၏ ဒေတာစင်တာတွင် လည်ပတ်နေသော အက်ပလီကေးရှင်း သို့မဟုတ် ဝန်ဆောင်မှု အက်ပလီကေးရှင်းတစ်ခုမှ ကုဒ်ပြောင်းထားသော ဒေတာ။
- Azure မှ လက်ခံရရှိသောအခါ ကုဒ်ပြောင်းပြီးသား ဒေတာ။

ကလိုင်းယင့်ဘက်ကုဒ်ပြောင်းခြင်းဖြင့်၊ ကလောက် ဝန်ဆောင်မှု ပေးသူများသည် ကုဒ်ပြောင်းသော့များသို့ ဝင်ရောက်ခွင့် မရှိသလို ဤဒေတာကို ကုဒ်ဖြေ၍လည်း မရနိုင်ပါ။ သင်သည် သော့များကို အပြည့်အဝ ထိန်းချုပ်ထားသည်။

ကလိုင်းယင့်ဘက်ကုဒ်ပြောင်းခြင်းကို အသုံးပြု၍ ဒေတာကို ကုဒ်ပြောင်းရန်၊ ပထမဦးစွာ အကြောင်းအရာ ကုဒ်ပြောင်းသော့ (Content Encryption Key - CEK) ကို ဖန်တီးရမည်။ ကလိုင်းယင့် ကွန်ရက်ပေါ်တွင် ဒေတာကို ကုဒ်ပြောင်းရန် ဤ CEK လိုအပ်သည်။ ထို့နောက် ဤသော့ကို သော့ကုဒ်ပြောင်းသော့ (Key Encryption Key - KEK) ဖြင့် ကုဒ်ပြောင်းသည်။ နောက်ဆုံးတွင်၊ ကုဒ်ပြောင်းထားသော ဒေတာကို Azure Storage တွင် သိမ်းဆည်းနိုင်သည်။ ဤလုပ်ငန်းစဉ်ကို အင်ဗလုပ် ကုဒ်ပြောင်းခြင်း (envelope encryption) ဟု ခေါ်သည်။

##### Encryption Process Using CEK and KEK (CEK နှင့် KEK ကို အသုံးပြု၍ ကုဒ်ပြောင်းခြင်း လုပ်ငန်းစဉ်)

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/pXBchbPKRfil1bGEwW86yw_ee6a6944ab5f4f7395cac672165423e1_image.png?expiry=1743638400000&hmac=ltqyA__CFn5QoKotuSM8EeNi0sGuxD6nfmdvq0NNL_U">

ဤသည်မှာ Azure တစ်လျှောက် အသုံးပြုနိုင်သော ကုဒ်ပြောင်းခြင်း လုပ်ငန်းစဉ်များထဲမှ တစ်ခုသာဖြစ်ပြီး၊ ၎င်းသည် အတော်လေး ရှုပ်ထွေးနိုင်သည်။

#### Server-Side Encryption (ဆာဗာဘက်ကုဒ်ပြောင်းခြင်း)

ဆာဗာဘက်ကုဒ်ပြောင်းခြင်းတွင် သော့စီမံခန့်ခွဲမှု ဝိသေသလက္ခဏာများ ကွဲပြားသော မော်ဒယ် သုံးမျိုး ရှိပြီး၊ သင်၏ လိုအပ်ချက်များအလိုက် တစ်ခုကို ရွေးချယ်နိုင်သည်။ ထိုမော်ဒယ်များမှာ-

- **ဝန်ဆောင်မှုမှ စီမံခန့်ခွဲသော သော့များ (Service-Managed Keys)**: ထိန်းချုပ်မှုနှင့် အဆင်ပြေမှုကို ပေါင်းစပ်ပေးပြီး အနည်းငယ်သာ စရိတ်သက်သာသည်။
- **ဖောက်သည်မှ စီမံခန့်ခွဲသော သော့များ (Customer-Managed Keys)**: သော့များကို သင်ထိန်းချုပ်နိုင်ပြီး Bring Your Own Keys (BYOK) ကို ပံ့ပိုးပေးသည် သို့မဟုတ် အသစ်ဖန်တီးနိုင်သည်။
- **ဖောက်သည်ထိန်းချုပ်သော ဟာ့ဒ်ဝဲတွင် ဝန်ဆောင်မှုမှ စီမံခန့်ခွဲသော သော့များ (Service-Managed Keys in Customer-Controlled Hardware)**: Microsoft ၏ ထိန်းချုပ်မှု ပြင်ပရှိ သင်၏ ပိုင်ဆိုင်မှု သိုလှောင်မှုတွင် သော့များကို စီမံခန့်ခွဲနိုင်စေသည်။ ဤဝိသေသလက္ခဏာကို Host Your Own Key (HYOK) ဟု ခေါ်သည်။ သို့သော်၊ ဖွဲ့စည်းပုံသည် ရှုပ်ထွေးပြီး Azure ဝန်ဆောင်မှု အများစုက ၎င်းမော်ဒယ်ကို မပံ့ပိုးပါ။

လုပ်ငန်းများတွင် အသုံးပြုသူများစွာနှင့် ဒေတာများစွာ ရှိနိုင်သောကြောင့်၊ ဤသော့အားလုံးကို စီမံခန့်ခွဲရန် တစ်စုံတစ်ခု ရှိရန် အရေးကြီးသည်။ ဤနေရာတွင် Azure Key Vault ဝင်လာသည်။

### Azure Key Vault (Azure Key Vault)

သင်ယခင်က သင်ယူခဲ့သည့်အတိုင်း၊ Azure Key Vault သည် Azure ရှိ သော့စီမံခန့်ခွဲမှု ဖြေရှင်းချက်များထဲမှ တစ်ခုဖြစ်ပြီး အောက်ပါ ပြဿနာများကို ဖြေရှင်းရန် ကူညီပေးသည်။

- **သော့စီမံခန့်ခွဲမှု**: Azure Key Vault ကို သော့စီမံခန့်ခွဲမှု ဖြေရှင်းချက်အဖြစ် အသုံးပြုနိုင်သည်။ Azure Key Vault သည် သင်၏ ဒေတာကို ကုဒ်ပြောင်းရန် အသုံးပြုသော ကုဒ်ပြောင်းသော့များကို ဖန်တီးရန်နှင့် ထိန်းချုပ်ရန် လွယ်ကူစေသည်။
- **လျှို့ဝှက်အချက်အလက် စီမံခန့်ခွဲမှု (Secrets Management)**: Azure Key Vault ကို တိုကင်များ၊ စကားဝှက်များ၊ လက်မှတ်များ၊ API သော့များ၊ နှင့် အခြားလျှို့ဝှက်အချက်အလက်များသို့ ဝင်ရောက်ခွင့်ကို လုံခြုံစွာ သိမ်းဆည်းပြီး တင်းကြပ်စွာ ထိန်းချုပ်ရန် အသုံးပြုနိုင်သည်။

Azure Key Vault သည် လက်မှတ် စီမံခန့်ခွဲမှုတွင်လည်း ကူညီပေးသည်။ ၎င်းသည် Azure နှင့် သင်၏ အတွင်းပိုင်း ချိတ်ဆက်ထားသော အရင်းအမြစ်များနှင့် အသုံးပြုရန် အများသုံး နှင့် သီးသန့် Transport Layer Security/Secure Sockets Layer (TLS/SSL) လက်မှတ်များကို အလွယ်တကူ ပံ့ပိုးပေးခြင်း၊ စီမံခန့်ခွဲခြင်း၊ နှင့် ဖြန့်ကျက်ခြင်း ပြုလုပ်နိုင်စေသည်။ အောက်တွင် Key Vault ရှိ လက်မှတ်တစ်ခု၏ ဥပမာဖြစ်သည်။

**Key Vault တွင် လက်မှတ်၊ လက်မှတ် မက်တာဒေတာ၊ သော့၊ နှင့် လျှို့ဝှက်အချက်အလက် ပါဝင်သည်**

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/2Gsk2KakRDqswyIo7ZH5vg_dced84163b334438817fd6b437351ce1_image.png?expiry=1743638400000&hmac=kroz_QyBWnXoI9JWmb_NRaXEb8oPEluzi-NnUG5rU9Y">

Key Vault နှင့် ကလိုင်းယင့်ဘက်ကုဒ်ပြောင်းခြင်းကို အသုံးပြုသောအခါ၊ သင်၏ ဒေတာကို Azure Storage ကလိုင်းယင့် SDK မှ ဖန်တီးထားသော တစ်ကြိမ်သုံး ဆင်မီထရစ် အကြောင်းအရာ ကုဒ်ပြောင်းသော့ (CEK) ကို အသုံးပြု၍ ကုဒ်ပြောင်းသည်။ Azure Storage ကလိုင်းယင့် SDK ကို အသုံးပြုခြင်းဆိုင်ရာ နောက်ထပ် အချက်အလက်များကို ဤသင်ခန်းစာ၏ အဆုံးရှိ ထပ်ဆောင်း အရင်းအမြစ်များတွင် ရှာဖွေနိုင်သည်။ CEK ကို ဆင်မီထရစ် သော့ သို့မဟုတ် အက်ဆင်မီထရစ် သော့တစ်စုံ (asymmetric key pair) ဖြစ်နိုင်သော သော့ကုဒ်ပြောင်းသော့ (KEK) ဖြင့် ကုဒ်ပြောင်းသည်။ ၎င်းကို ဒေသတွင်း၌ စီမံခန့်ခွဲနိုင်သည် သို့မဟုတ် Key Vault တွင် သိမ်းဆည်းနိုင်သည်။ ထို့နောက် ကုဒ်ပြောင်းထားသော ဒေတာကို Azure Storage သို့ တင်ပို့သည်။

Key Vault ဖြင့် မည်သည့် လုပ်ငန်းဆောင်ရွက်မှုများ လုပ်ဆောင်ရန်မဆို၊ ပထမဦးစွာ ၎င်းကို အတည်ပြုရန် (authenticate) လိုအပ်သည်။ Key Vault နှင့် အတည်ပြုခြင်းသည် မည်သည့် လုံခြုံရေး အဓိကပုဂ္ဂိုလ် (security principal) ၏ အထောက်အထားကို အတည်ပြုရန် တာဝန်ရှိသော Azure Active Directory နှင့် အလုပ်လုပ်သည်။

Azure တွင် ဗာ့ချွယ် စက်တစ်ခုပေါ်တွင် အက်ပ်တစ်ခု ဖြန့်ကျက်သောအခါ၊ Key Vault သို့ ဝင်ရောက်ခွင့်ရှိသော အထောက်အထားတစ်ခု (identity) ကို ထိုဗာ့ချွယ် စက်သို့ သတ်မှတ်ပေးနိုင်သည်။ အခြား Azure အရင်းအမြစ်များသို့လည်း အထောက်အထားများ သတ်မှတ်ပေးနိုင်သည်။ ဤနည်းလမ်း၏ အကျိုးကျေးဇူးမှာ အက်ပ် သို့မဟုတ် ဝန်ဆောင်မှုသည် ပထမဆုံး လျှို့ဝှက်အချက်အလက်၏ လည်ပတ်မှု (rotation) ကို စီမံခန့်ခွဲရန် မလိုအပ်ခြင်းဖြစ်သည်။ Azure သည် အထောက်အထားနှင့် ဆက်စပ်နေသော ဝန်ဆောင်မှု အဓိကပုဂ္ဂိုလ် ကလိုင်းယင့် လျှို့ဝှက်အချက်အလက် (service principal client secret) ကို အလိုအလျောက် လည်ပတ်ပေးသည်။ ၎င်းသည် အကောင်းဆုံး အလေ့အကျင့်တစ်ခုအဖြစ် အကြံပြုထားသော ချဉ်းကပ်နည်းဖြစ်သည်။

##### Process of Using Azure Key Vault with Azure Active Directory (Azure Active Directory နှင့် Azure Key Vault ကို အသုံးပြုခြင်း လုပ်ငန်းစဉ်)

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/vADl9u-NR7ijxozLQlupIg_813de8706f4c4e00a8c43c05344a1ae1_image.png?expiry=1743638400000&hmac=NRnC21_gNXrA1j0XC0zbM02BjGT_MvK7exD04l1nltc">

Azure Key Vault သည် Azure Key Vault နှင့် ကလိုင်းယင့်များအကြား ဒေတာ သွားလာသည့်အခါ ၎င်းကို ကာကွယ်ရန် Transport Layer Security (TLS) ပရိုတိုကောကို အသုံးပြုသည်။ ကလိုင်းယင့်များသည် Azure Key Vault နှင့် TLS ချိတ်ဆက်မှုကို ညှိနှိုင်းသည်။

Azure စာရင်းသွင်းမှု (subscription) ရှိသူတိုင်းသည် သော့ဗော့များကို ဖန်တီးပြီး အသုံးပြုနိုင်သည်။ Key Vault သည် ဖန်တီးသူများနှင့် လုံခြုံရေး အုပ်ချုပ်သူများအတွက် အကျိုးကျေးဇူးပေးသော်လည်း၊ ၎င်းကို အခြား Azure ဝန်ဆောင်မှုများကို စီမံခန့်ခွဲသော အဖွဲ့အစည်း၏ အုပ်ချုပ်သူတစ်ဦးမှ အကောင်အထည်ဖော်၍ စီမံခန့်ခွဲနိုင်သည်။ ဥပမာ၊ အုပ်ချုပ်သူသည် Azure စာရင်းသွင်းမှုဖြင့် ဝင်ရောက်နိုင်ပြီး၊ သော့များသိမ်းဆည်းရန် အဖွဲ့အစည်းအတွက် ဗော့တစ်ခု ဖန်တီးနိုင်ကာ၊ ထို့နောက် အောက်ပါ လုပ်ငန်းဆောင်တာများအတွက် တာဝန်ယူနိုင်သည်-

- သော့ သို့မဟုတ် လျှို့ဝှက်အချက်အလက်တစ်ခု ဖန်တီးခြင်း သို့မဟုတ် တင်သွင်းခြင်း
- သော့ သို့မဟုတ် လျှို့ဝှက်အချက်အလက်တစ်ခု ပြန်လည်ရုပ်သိမ်းခြင်း သို့မဟုတ် ဖျက်ဆီးခြင်း
- အသုံးပြုသူများ သို့မဟုတ် အက်ပလီကေးရှင်းများကို သော့ဗော့သို့ ဝင်ရောက်ခွင့် ခွင့်ပြုခြင်း၊ ထို့ကြောင့် ၎င်းတို့သည် ၎င်း၏ သော့များနှင့် လျှို့ဝှက်အချက်အလက်များကို စီမံခန့်ခွဲခြင်း သို့မဟုတ် အသုံးပြုနိုင်သည်
- သော့အသုံးပြုမှု ဖွဲ့စည်းပုံပြင်ဆင်ခြင်း (ဥပမာ၊ လက်မှတ်ထိုးခြင်း သို့မဟုတ် ကုဒ်ပြောင်းခြင်း)
- သော့အသုံးပြုမှုကို စောင့်ကြည့်ခြင်း

ဖန်တီးသူများအတွက်၊ အက်ပလီကေးရှင်းများသည် URI များကို အသုံးပြု၍ ၎င်းတို့လိုအပ်သော အချက်အလက်များကို လုံခြုံစွာ ဝင်ရောက်နိုင်သည်။ URL များသည် အရင်းအမြစ်တစ်ခုကို ရှာဖွေရန် ခွင့်ပြုသော်လည်း၊ URI သည် အရင်းအမြစ်တစ်ခုကို ခွဲခြားသတ်မှတ်ရုံသာဖြစ်သည်။ ဆိုလိုသည်မှာ URI သည် အရင်းအမြစ်တစ်ခုကို ရယူရန် လိပ်စာတစ်ခုအဖြစ် ရည်ရွယ်ထားခြင်း မဟုတ်ဘဲ၊ ခွဲခြားသတ်မှတ်သူအဖြစ်သာ ရည်ရွယ်သည်။ ဤ URI များသည် အက်ပလီကေးရှင်းများအား လျှို့ဝှက်အချက်အလက်၏ သတ်မှတ်ထားသော ဗားရှင်းများကို ပြန်လည်ရယူနိုင်စေသည်။ Key Vault တွင် သိမ်းဆည်းထားသော လျှို့ဝှက်အချက်အလက်များကို ကာကွယ်ရန် စိတ်ကြိုက် ကုဒ်ရေးရန် မလိုအပ်ပါ။

အောက်ပါ ဥပမာတွင်၊ အုပ်ချုပ်သူသည် ဖန်တီးသူများအား ၎င်းတို့၏ အက်ပလီကေးရှင်းများမှ ခေါ်ဆိုရန် URI များကို ပေးထားပြီး၊ ၎င်းတို့ အသုံးပြုနိုင်သော သော့များကို ရယူနိုင်သည်။ ဤအုပ်ချုပ်သူသည် သော့အသုံးပြုမှုနှင့် မှတ်တမ်းတင်ခြင်း အချက်အလက်များသို့လည်း ဝင်ရောက်ခွင့် ရှိသည်။

##### Secure Access to Applications Ensured with URIs for Keys (သော့များအတွက် URI များဖြင့် အက်ပလီကေးရှင်းများသို့ လုံခြုံသော ဝင်ရောက်ခွင့် သေချာစေခြင်း)

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Ht6D-DM_RIuibZpUJqU53w_477c3e16c3804d7abb9546c85cc543e1_image.png?expiry=1743638400000&hmac=DlDxYa3eav1QfKSzWGaCy_hVR6Mo1X2AKYQmB5X2DAE">

ဤဖွဲ့စည်းပုံသည် Sam’s Scoops အတွက် ကောင်းမွန်စွာ အလုပ်လုပ်မည်ဖြစ်သည်။ ဝက်ဘ် ဖန်တီးသူသည် ဗာ့ချွယ် စက်သို့ ဝင်ရောက်ရန် JIT ကို အသုံးပြုနိုင်ပြီး၊ သော့ဗော့ကို အသုံးပြုရန်နှင့် လျှို့ဝှက်အချက်အလက်များ သိမ်းဆည်းရန် မှန်ကန်သော ဝင်ရောက်ခွင့် အခွင့်အာဏာများ သတ်မှတ်ပေးခံရမည်။

### Conclusion (နိဂုံးချုပ်)

Microsoft Azure ကဲ့သို့သော အများသုံး ကလောက် ဝန်ဆောင်မှုကို အသုံးပြုသောအခါ၊ ၎င်း၏ ဒေတာစင်တာများအတွင်း သိမ်းဆည်းထားသော ဒေတာများကို ကုဒ်ပြောင်းရန် အရေးကြီးသည်။ ထိုဒေတာအားလုံးကို ကလောက်သို့ မရွှေ့မီ ကုဒ်ပြောင်းရန်လည်း အလားတူ အရေးကြီးသည်။ အင်ဗလုပ် ကုဒ်ပြောင်းခြင်း လုပ်ငန်းစဉ်ကဲ့သို့သော နည်းလမ်းများစွာ ရှိသော်လည်း၊ ၎င်းတို့အားလုံးသည် ကုဒ်ပြောင်းသော့များကို ဖန်တီးပြီး လိုအပ်သည်။ စီမံခန့်ခွဲရန် သော့များစွာ ရှိသည့်အခါ သော့စီမံခန့်ခွဲမှု လုပ်ငန်းစဉ် လိုအပ်သည်။

သော့စီမံခန့်ခွဲမှုအတွက် Azure Key Vault ဝန်ဆောင်မှုကို အသုံးပြု၍ သော့အသုံးပြုမှုကို စီမံခန့်ခွဲပြီး စောင့်ကြည့်နိုင်သည်။ သော့စီမံခန့်ခွဲမှု အလုပ်လုပ်ရန်၊ အသုံးပြုသူများ၊ အက်ပလီကေးရှင်းများ၊ နှင့် စက်များအားလုံးကို ခွဲခြားသတ်မှတ်ရန် လိုအပ်ပြီး၊ Azure Active Directory ကို အသုံးပြု၍ အသုံးပြုသူများကို အတည်ပြုကာ ၎င်းတို့၏ အခန်းကဏ္ဍကို လုပ်ဆောင်ရန် လိုအပ်သော သက်ဆိုင်ရာ သော့များသို့ ဝင်ရောက်ခွင့် ပေးနိုင်သည်။ Azure Key Vault သည် Sam’s Scoops အတွက် အလုပ်လုပ်မည်ဖြစ်သည်။ အကြောင်းမှာ ဖန်တီးသူသည် စက်ဝင်ရောက်ခွင့်အတွက် JIT ကို အသုံးပြုနိုင်ပြီး၊ Azure Active Directory ကို အသုံးပြု၍ အတည်ပြုကာ Azure Key Vault အတွင်းရှိ မှန်ကန်သော ကုဒ်ပြောင်းသော့များသို့ ဝင်ရောက်ခွင့် ရယူနိုင်သောကြောင့်ဖြစ်သည်။
