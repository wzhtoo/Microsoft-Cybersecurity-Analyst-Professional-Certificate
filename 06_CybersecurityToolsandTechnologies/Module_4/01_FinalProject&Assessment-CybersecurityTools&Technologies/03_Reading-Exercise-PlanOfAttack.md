# Exercise: Plan of attack

[Exercise: Plan of attack 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/supplement/XOMME/exercise-plan-of-attack)

# Exercise: Plan of attack (လေ့ကျင့်ခန်း- တိုက်ခိုက်မှုအစီအစဉ်)

## Introduction (နိဒါန်း)

ဤလေ့ကျင့်ခန်းသည် ဤသင်တန်းတစ်လျှောက် သင်လေ့လာခဲ့သော အသိပညာနှင့် ကျွမ်းကျင်မှုများကို အသုံးချနိုင်စေမည်ဖြစ်သည်။ သင်၏တာဝန်မှာ သရုပ်တူ Microsoft Azure ပတ်ဝန်းကျင်အတွင်း White Box ထိုးဖောက်စမ်းသပ်ခြင်းအတွက် အလုံးစုံပါဝင်သော စီစဉ်သတ်မှတ်မှုနှင့် စမ်းသပ်မှုဗျူဟာကို ရေးဆွဲရန်ဖြစ်သည်။ ထို့အပြင် ထိုးဖောက်စမ်းသပ်မှု၏ အဆင့်ငါးဆင့်ကို သရုပ်ဖော်ရန် Figma သို့မဟုတ် အလားတူ ပုံဆွဲကိရိယာကို အသုံးပြုရန်လည်း တိုက်တွန်းပါသည်။

## Scenario (အခြေအနေ)

Sam's Scoops သည် ယခုအခါ နိုင်ငံတကာအဖွဲ့အစည်းတစ်ခုဖြစ်လာပြီး နေရာအများအပြားတွင် လည်ပတ်ကာ သုံးစွဲသူများ၏ အွန်လိုင်းအမှာစာများစွာကို ကိုင်တွယ်ဆောင်ရွက်နေပါသည်။ Sam သည် သီးသန့်သုံးစွဲသူအချက်အလက်များကို သိမ်းဆည်းထားပြီး ကိုယ်ရေးကိုယ်တာနှင့် ငွေကြေးဆိုင်ရာ အချက်အလက်များစွာကို ကိုင်တွယ်ဆောင်ရွက်နေသောကြောင့် Sam သည် ၎င်းတို့၏ အခြေခံအဆောက်အအုံသည် ထိုတာဝန်အတွက် လုံလောက်သည်ဟု မည်သို့ယုံကြည်နိုင်မည်နည်း။ ဆိုက်ဘာလုံခြုံရေးသည် ယခုအခါ လူများ၏ စိတ်ထဲတွင် အဓိကနေရာယူလာသောကြောင့် ၎င်း၏လုပ်ငန်းအပေါ် ခြိမ်းခြောက်မှုများ တိုးပွားလာလျက်ရှိသည်။

ထို့ကြောင့် ဤလေ့ကျင့်ခန်း၏ အဓိကရည်ရွယ်ချက်မှာ လက်တွေ့ကမ္ဘာ့ အခြေခံအဆောက်အအုံနှင့် အက်ပ်များကို တုပရန် ရည်ရွယ်ထားသော Azure ပတ်ဝန်းကျင်အတွင်း လုပ်ဆောင်မည့် White Box ထိုးဖောက်စမ်းသပ်မှုကို ဂရုတစိုက် စီစဉ်ရန်ဖြစ်သည်။ ဤလေ့ကျင့်ခန်း၏ အဓိကရည်ရွယ်ချက်မှာ အလုံးစုံပါဝင်သော ထိုးဖောက်စမ်းသပ်မှုအစီအစဉ်တစ်ခုကို ရေးဆွဲပြီး ကွန်ရက် ဗိသုကာပုံကြမ်းတစ်ခုကို ဖန်တီးရန်ဖြစ်သည်။ ထို့အပြင် ပုံကြမ်း၏ အဓိကအစိတ်အပိုင်းများနှင့် ဖွဲ့စည်းပုံကို ရှင်းလင်းချက်ဖြင့် ပူးတွဲတင်ပြရန် အရေးကြီးပါသည်။

ဤလေ့ကျင့်ခန်းသည် စီစဉ်ရေးအဆင့်ကို အဓိကထားပြီး၊ ဤလုပ်ငန်းတာဝန်၏ တစ်စိတ်တစ်ပိုင်းအနေဖြင့် ထိုးဖောက်စကင်ကို အမှန်တကယ် လုပ်ဆောင်ရန် မလိုအပ်ကြောင်း သတိပြုပါ။ အခြေခံအဆောက်အအုံနှင့် ၎င်း၏အသုံးပြုမှုကို အောက်တွင်ဖော်ပြထားသော်လည်း အခြားအစိတ်အပိုင်းများ သို့မဟုတ် အရင်းအမြစ်များကို လွတ်လပ်စွာ ထည့်သွင်းနိုင်သည်။

## Sam's Scoops' Azure infrastructure description (Sam's Scoops ၏ Azure အခြေခံအဆောက်အအုံ ဖော်ပြချက်)

### Virtual machine (VM) (ကွန်ပျူတာသရုပ်တူစက် (VM))

ကျွန်ုပ်တို့၏ VMs များသည် ကျွန်ုပ်တို့၏ Azure အခြေခံအဆောက်အအုံ၏ အဓိကလုပ်ဆောင်သူများဖြစ်ပြီး၊ ကျွန်ုပ်တို့၏ အပလီကေးရှင်းများနှင့် ဝန်ဆောင်မှုများကို လုပ်ဆောင်ရန် အခြေခံအဖြစ် ဆောင်ရွက်ပါသည်။ VM တစ်ခုစီသည် ကျွန်ုပ်တို့၏ လုပ်ငန်းတာဝန်များကို ထိရောက်စွာ အသုံးချစီမံနိုင်စေရန် လိုက်လျောညီထွေရှိပြီး စိတ်ကြိုက်ပြင်ဆင်နိုင်သော ကွန်ပျူတာအမျိုးအစားတစ်ခုဖြစ်သည်။

VM တစ်ခုစီသည် ကျွန်ုပ်တို့၏ Virtual Network (VNet) နှင့် ချိတ်ဆက်ထားပြီး၊ လိုအပ်သော ကွန်ရက်သီးခြားထားရှိမှုနှင့် လုံခြုံရေးထိန်းချုပ်မှုများကို ပံ့ပိုးပေးပါသည်။ RBAC (အခန်းကဏ္ဍအခြေပြု ဝင်ရောက်ခွင့်ထိန်းချုပ်မှု) နှင့် Azure လုံခြုံရေးမူဝါဒများဖြင့် VM အရင်းအမြစ်များသို့ ဝင်ရောက်ခွင့်ကို ဂရုတစိုက် စီမံခန့်ခွဲပြီး ဖြစ်နိုင်ချေရှိသော လုံခြုံရေးအန္တရာယ်များကို လျှော့ချရန်အတွက် အနည်းဆုံးအခွင့်အရေးမူကို လိုက်နာပါသည်။

အချုပ်အားဖြင့် ကျွန်ုပ်တို့၏ ကွန်ပျူတာသရုပ်တူစက်များသည် ကျွန်ုပ်တို့၏ Azure စမ်းသပ်ပတ်ဝန်းကျင်၏ အဓိကအချက်ဖြစ်ပြီး၊ လုံခြုံရေးနှင့် စည်းကမ်းလိုက်နာမှု၏ အမြင့်ဆုံးစံနှုန်းများကို ထိန်းသိမ်းထားစဉ် ကျွန်ုပ်တို့၏ မတူကွဲပြားသော လုပ်ငန်းတာဝန်များကို ပံ့ပိုးရန် ဂရုတစိုက် စီစဉ်သတ်မှတ်ပြီး လုံခြုံအောင်ထားရှိပါသည်။

### Virtual network (VNet) (ကွန်ရက်သရုပ်တူ)

ကျွန်ုပ်တို့၏ Azure အခြေခံအဆောက်အအုံ၏ အခြေခံအုတ်မြစ်မှာ Virtual Network (VNet) ဖြစ်သည်။ ၎င်းသည် Azure တွင် ကွန်ရက်သရုပ်တူ ဒေတာစင်တာတစ်ခုအဖြစ် ဆောင်ရွက်ပြီး ကျွန်ုပ်တို့၏ စမ်းသပ်ပတ်ဝန်းကျင်ကို ထုတ်လုပ်မှုကွန်ရက်မှ သီးခြားထားရှိပေးပါသည်။ VNet သည် ကျွန်ုပ်တို့အား သီးသန့် IP လိပ်စာနေရာများ၊ ကွန်ရက်ငယ်များနှင့် ကွန်ရက်လုံခြုံရေးထိန်းချုပ်မှုများကို သတ်မှတ်ခွင့်ပြုပါသည်။

### Subnets (ကွန်ရက်ငယ်များ)

ကျွန်ုပ်တို့၏ VNet အတွင်းတွင် သက်ဆိုင်ရာအရင်းအမြစ်များကို ယုတ္တိနည်းကျ စုစည်းရန် ကျွန်ုပ်တို့၏ပတ်ဝန်းကျင်ကို ကွန်ရက်ငယ်များစွာအဖြစ် ခွဲခြားထားပါသည်။ ကွန်ရက်ငယ်များကို ဝဘ်ဆာဗာများ၊ အပလီကေးရှင်းဆာဗာများနှင့် ဒေတာဘေ့စ်များကဲ့သို့သော မတူညီသော အစိတ်အပိုင်းများကို ခွဲခြားရန်အတွက် အသုံးပြုပြီး လုံခြုံရေးနှင့် စနစ်တကျဖွဲ့စည်းမှုကို မြှင့်တင်ပေးပါသည်။

### Network security groups (NSG) (ကွန်ရက်လုံခြုံရေးအဖွဲ့များ)

ကျွန်ုပ်တို့၏ Azure အရင်းအမြစ်များအတွင်းနှင့် အပြင်သို့ ဒေတာစီးဆင်းမှုကို ထိန်းချုပ်ရန်အတွက် ကျွန်ုပ်တို့သည် Network Security Groups (NSGs) ကို အကောင်အထည်ဖော်ထားပါသည်။ NSGs များသည် ကွန်ရက်သရုပ်တူ Firewall များအဖြစ် ဆောင်ရွက်ပြီး IP လိပ်စာများ၊ port များနှင့် protocol များ၏ အရင်းအမြစ်နှင့် ဦးတည်ရာအပေါ် အခြေခံ၍ ကွန်ရက်ဒေတာကို ခွင့်ပြုခြင်း သို့မဟုတ် ငြင်းပယ်ခြင်းဆိုင်ရာ စည်းမျဉ်းများကို သတ်မှတ်ခွင့်ပြုပါသည်။

### Private IP range (သီးသန့် IP လိပ်စာအကွာအဝေး)

လက်တွေ့ကမ္ဘာ့ ကွန်ရက်အခြေအနေများကို တုပရန် ကျွန်ုပ်တို့သည် ကျွန်ုပ်တို့၏ VNet သို့ သီးသန့် IP လိပ်စာအကွာအဝေးတစ်ခုကို သတ်မှတ်ပေးထားပါသည်။ ဤသီးသန့် IP လိပ်စာအကွာအဝေးသည် ကျွန်ုပ်တို့၏ စမ်းသပ်ပတ်ဝန်းကျင်သည် သာမန်သီးသန့်ကွန်ရက်လိပ်စာနေရာအတွင်း လုပ်ဆောင်ကြောင်း သေချာစေပါသည်။

### Resource groups (အရင်းအမြစ်အုပ်စုများ)

ကျွန်ုပ်တို့၏ စမ်းသပ်ရင်းအမြစ်များကို ထိရောက်စွာ စီမံခန့်ခွဲရန်နှင့် သီးခြားထားရှိရန်အတွက် ၎င်းတို့ကို သီးခြားအရင်းအမြစ်အုပ်စုတစ်ခုအဖြစ် စုစည်းထားပါသည်။ ဤခွဲခြားမှုသည် ထုတ်လုပ်မှုအရင်းအမြစ်များနှင့် မရည်ရွယ်ဘဲ အနှောင့်အယှက်ဖြစ်ခြင်းကို ကာကွယ်ပြီး အရင်းအမြစ်စီမံခန့်ခွဲမှုကို ချောမွေ့စေပါသည်။

### Role-based access control (RBAC) (အခန်းကဏ္ဍအခြေပြု ဝင်ရောက်ခွင့်ထိန်းချုပ်မှု)

လုံခြုံရေးသည် ကျွန်ုပ်တို့၏ စမ်းသပ်ပတ်ဝန်းကျင်တွင် ဦးစားပေးဖြစ်သည်။ သင့်လျော်သော ဝင်ရောက်ခွင့်ထိန်းချုပ်မှုကို သေချာစေရန်အတွက် ကျွန်ုပ်တို့သည် RBAC မူများကို အကောင်အထည်ဖော်ထားပါသည်။ RBAC သည် အနည်းဆုံးအခွင့်အရေးမူ (PoLP) ကို လိုက်နာ၍ အခန်းကဏ္ဍများနှင့် ခွင့်ပြုချက်များအပေါ် အခြေခံ၍ သုံးစွဲသူဝင်ရောက်ခွင့်ကို ကန့်သတ်ထားပါသည်။

### Azure Firewall (Azure Firewall)

ကျွန်ုပ်တို့၏ ကွန်ရက်လုံခြုံရေးကို မြှင့်တင်ရန်အတွက် ကျွန်ုပ်တို့သည် Azure Firewall ကို အသုံးပြုထားပါသည်။ ဤဝန်ဆောင်မှုသည် ကျွန်ုပ်တို့၏ စမ်းသပ်ပတ်ဝန်းကျင်နှင့် အင်တာနက်ကြားရှိ ဒေတာစီးဆင်းမှုကို ထိန်းချုပ်သည့် အပြင်ဘက် Firewall အဖြစ် ဆောင်ရွက်ပါသည်။ ခွင့်ပြုချက်မရှိဘဲ ဝင်ရောက်ခြင်းနှင့် ခြိမ်းခြောက်မှုများမှ ကာကွယ်ရန်အတွက် လုံခြုံရေးမူဝါဒများကို အတင်းအကြပ် အကောင်အထည်ဖော်ပါသည်။

### Virtual private network (VPN) (ကွန်ရက်သရုပ်တူ သီးသန့်ကွန်ရက် (VPN))

ကျွန်ုပ်တို့၏ စမ်းသပ်ပတ်ဝန်းကျင်အတွက် လုံခြုံသော အဝေးမှဝင်ရောက်ခွင့်သည် အလွန်အရေးကြီးပါသည်။ ခွင့်ပြုထားသော သုံးစွဲသူများသည် အဝေးမှနေရာများမှ ကျွန်ုပ်တို့၏ Azure အရင်းအမြစ်များကို လုံခြုံစွာ ဝင်ရောက်နိုင်စေရန် VPN ချိတ်ဆက်မှုကို တည်ဆောက်ထားပါသည်။ ဤ VPN ချိတ်ဆက်မှုသည် ဒေတာလျှို့ဝှက်ချက်နှင့် တည်ကြည်မှုကို သေချာစေပါသည်။

### Azure Security Center (Defender for Cloud) (Azure လုံခြုံရေးစင်တာ (Cloud အတွက် Defender))

စဉ်ဆက်မပြတ် စောင့်ကြည့်ခြင်းနှင့် ခြိမ်းခြောက်မှုရှာဖွေခြင်းသည် ကျွန်ုပ်တို့၏ လုံခြုံရေးဗျူဟာ၏ အရေးပါသော အစိတ်အပိုင်းများဖြစ်သည်။ Azure Security Center ကို အချိန်နှင့်တပြေးညီ ခြိမ်းခြောက်မှုဆိုင်ရာ ထောက်လှမ်းရေးနှင့် ကြိုတင်ကာကွယ်သော လုံခြုံရေးဆိုင်ရာ အကြံပြုချက်များကို ပေးရန်အတွက် အသုံးပြုပါသည်။

### Microsoft Sentinel and Log Analytics (Microsoft Sentinel နှင့် Log Analytics)

သံသယဖြစ်ဖွယ် လုပ်ဆောင်ချက်များကို ရှာဖွေရန်အတွက် မှတ်တမ်းများနှင့် တယ်လီမေထရီဒေတာများကို စုဆောင်းခြင်းနှင့် ခွဲခြမ်းစိတ်ဖြာခြင်းသည် အလွန်အရေးကြီးပါသည်။ မှတ်တမ်းများကို ဗဟိုချုပ်ကိုင်ပြီး ခွဲခြမ်းစိတ်ဖြာရန် Microsoft Sentinel နှင့် Log Analytics ကို အသုံးပြုပြီး လုံခြုံရေးဖြစ်ရပ်များကို ထိရောက်စွာ ခွဲခြားသတ်မှတ်ပြီး တုံ့ပြန်နိုင်စေပါသည်။

### Azure Security Policy (Azure လုံခြုံရေးမူဝါဒ)

လုံခြုံရေးစံနှုန်းများနှင့် ကိုက်ညီမှုရှိစေရန် ကျွန်ုပ်တို့သည် Azure လုံခြုံရေးမူဝါဒများကို အကောင်အထည်ဖော်ထားပါသည်။ ဤမူဝါဒများသည် သီးခြားလုံခြုံရေးလိုအပ်ချက်များကို အတင်းအကြပ် အကောင်အထည်ဖော်ပြီး လုပ်ငန်းနယ်ပယ်၏ အကောင်းဆုံးအလေ့အကျင့်များနှင့် ကိုက်ညီရန် ကူညီပေးပါသည်။

### Azure Active Directory (Azure AD) (Azure Active Directory (Azure AD))

သင့်လျော်သော အထောက်အထားနှင့် ဝင်ရောက်ခွင့်စီမံခန့်ခွဲမှု ထိန်းချုပ်မှုများသည် အလွန်အရေးကြီးပါသည်။ Azure Active Directory (Azure AD) သည် ကျွန်ုပ်တို့၏ Azure အရင်းအမြစ်များသို့ သုံးစွဲသူအထောက်အထားများနှင့် ဝင်ရောက်ခွင့်ကို စီမံခန့်ခွဲရာတွင် အဓိကအခန်းကဏ္ဍမှ ပါဝင်ပါသည်။

ဤအခြေခံအဆောက်အအုံနှင့် ၎င်းတွင်ပေါင်းစပ်ထားသော Azure ဝန်ဆောင်မှုများကို လုံခြုံ၊ သီးခြားထားရှိပြီး လက်တွေ့ဆန်သော စမ်းသပ်ပတ်ဝန်းကျင်ကို ပံ့ပိုးရန် ဂရုတစိုက် ဒီဇိုင်းထုတ်ထားပါသည်။ ဤအစိတ်အပိုင်းများကို အခြေခံအဖြစ် အသုံးပြု၍ သင်၏ ကွန်ရက် ဗိသုကာပုံကြမ်းသည် ဤ Azure ပတ်ဝန်းကျင်ကို မြင်သာထင်သာစွာ ကိုယ်စားပြုမည်ဖြစ်ပြီး သင်၏ ထိုးဖောက်စမ်းသပ်မှုအစီအစဉ်ကို မြှင့်တင်ကာ တွေ့ရှိချက်များနှင့် အကြံပြုချက်များကို ထိရောက်စွာ ဆက်သွယ်ပြောဆိုနိုင်စေမည်ဖြစ်သည်။

## Network architecture diagram (ကွန်ရက် ဗိသုကာပုံကြမ်း)

သင်၏ ကွန်ရက် ဗိသုကာပုံကြမ်းတွင် ထည့်သွင်းသင့်သော အရာများ၏ စုစည်းထားသော စာရင်းကို ဤတွင်ဖော်ပြထားပါသည်။

- **Virtual machine (VM)**: စမ်းသပ်ပတ်ဝန်းကျင်အတွက် သီးသန့် VM ကို ကိုယ်စားပြုပါ။
- **Virtual network (VNet)**: စမ်းသပ်ပတ်ဝန်းကျင်အတွက် သီးသန့် VNet ကို ကိုယ်စားပြုပါ။
- **Subnets**: ဝဘ်ဆာဗာများ၊ အပလီကေးရှင်းဆာဗာများနှင့် ဒေတာဘေ့စ်များကဲ့သို့သော မတူညီသော အစိတ်အပိုင်းများကို ခွဲခြားရန်အတွက် အသုံးပြုသည့် ကွန်ရက်ငယ်များစွာကို သရုပ်ဖော်ပါ။
- **Network security groups (NSG)**: အဝင်နှင့် အထွက်ဒေတာကို ထိန်းချုပ်ရာတွင် NSG များ၏ အခန်းကဏ္ဍကို ကိုယ်စားပြုရန် သင်္ကေတများကို အသုံးပြုပါ။
- **Private IP range**: VNet သို့ သတ်မှတ်ထားသော သီးသန့် IP လိပ်စာအကွာအဝေးကို ညွှန်ပြပါ။
- **Resource groups**: ထုတ်လုပ်မှုအရင်းအမြစ်များနှင့် အနှောင့်အယှက်မဖြစ်စေရန် သီးခြားအရင်းအမြစ်အုပ်စုအတွင်း စမ်းသပ်အရင်းအမြစ်များကို သီးခြားထားရှိမှုကို ပြပါ။
- **Role-based access control (RBAC)**: သုံးစွဲသူများနှင့် အခန်းကဏ္ဍများအတွက် အနည်းဆုံးအခွင့်အရေးမူ (PoLP) ကို အလေးပေးရန် RBAC မူများကို ကိုယ်စားပြုပါ။
- **Azure Firewall**: ဒေတာထိန်းချုပ်ရာတွင် ၎င်း၏အခန်းကဏ္ဍကို အလေးပေးရန် Azure Firewall အတွက် သင်္ကေတတစ်ခု ထည့်သွင်းပါ။
- **Virtual private network (VPN)**: စမ်းသပ်ပတ်ဝန်းကျင်သို့ လုံခြုံစွာဝင်ရောက်ရန်အတွက် အသုံးပြုသည့် VPN ချိတ်ဆက်မှုကို သရုပ်ဖော်ပါ။
- **Azure Security Center (Defender for Cloud)**: စဉ်ဆက်မပြတ် စောင့်ကြည့်ခြင်းနှင့် ခြိမ်းခြောက်မှုရှာဖွေခြင်းအတွက် Azure Security Center ကို အသုံးပြုမှုကို ပြသပါ။
- **Microsoft Sentinel and Log Analytics**: သံသယဖြစ်ဖွယ် လုပ်ဆောင်ချက်များကို ရှာဖွေရန် မှတ်တမ်းများစုဆောင်းခြင်းနှင့် ခွဲခြမ်းစိတ်ဖြာခြင်းကို ကိုယ်စားပြုရန် အရာများ ထည့်သွင်းပါ။
- **Azure Security Policy**: စည်းကမ်းလိုက်နာမှုစံနှုန်းများကို အတင်းအကြပ်အကောင်အထည်ဖော်ရန် လုံခြုံရေးမူဝါဒများ အကောင်အထည်ဖော်မှုကို သရုပ်ဖော်ပါ။
- **Azure Active Directory (Azure AD)**: သင့်လျော်သော အထောက်အထားနှင့် ဝင်ရောက်ခွင့်စီမံခန့်ခွဲမှု ထိန်းချုပ်မှုများကို အလေးပေးရန် Azure AD ကို ကိုယ်စားပြုပါ။

ထို့အပြင် ကွန်ရက် ဗိသုကာပုံကြမ်းဖန်တီးမှုကို လွယ်ကူချောမွေ့စေရန်အတွက် လိုအပ်သော သင်္ကေတများအားလုံးကို ဤလေ့ကျင့်ခန်း၏ တစ်စိတ်တစ်ပိုင်းအဖြစ် ထည့်သွင်းထားကြောင်း သတိပြုပါ။

## Diagram assets (ပုံကြမ်းပစ္စည်းများ)

[ZIP File](link_to_diagram_assets)

## Penetration testing plan (ထိုးဖောက်စမ်းသပ်မှုအစီအစဉ်)

သင်ယခင်က တည်ဆောက်ခဲ့သော Azure ကွန်ရက်ဒီဇိုင်းအတွက် ပံ့ပိုးထားသော စမ်းသပ်မှုဗျူဟာအပေါ် အခြေခံ၍ ထိုးဖောက်စမ်းသပ်မှုအစီအစဉ်ကို ဖန်တီးပါ။ အစီအစဉ်၏ အောင်မြင်စွာ အကောင်အထည်ဖော်မှုကို အာမခံရန် အဖွဲ့အစည်းတွင် အစွမ်းထက်သော ကိရိယာများစွာရှိသည်။

### Testing Tools Available (ရရှိနိုင်သော စမ်းသပ်ကိရိယာများ)

အဖွဲ့အစည်းသည် Azure ပတ်ဝန်းကျင်ကို အသေးစိတ် အကဲဖြတ်နိုင်စေရန် စွမ်းဆောင်ရည်မြင့်မားပြီး လုပ်ငန်းနယ်ပယ်စံနှုန်းမီ ကိရိယာအမျိုးမျိုးကို အသုံးပြုခွင့်ရှိသည်။ ဤစမ်းသပ်မှုအတွက် အသုံးပြုရန် အတည်ပြုထားသော ကိရိယာများစာရင်းမှာ အောက်ပါအတိုင်းဖြစ်သည်-

- Azure CLI
- PowerShell
- Open-source intelligence (OSINT) sources
- Nmap
- OWASP ZAP
- Azure Security Center
- Metasploit
- OWASP WebGoat

### Testing plan (စမ်းသပ်မှုအစီအစဉ်)

ဤလေ့ကျင့်ခန်းအတွက် သင်သည် Sam's Scoops ၏ Microsoft Azure ပတ်ဝန်းကျင်အတွက် အလုံးစုံပါဝင်သော ထိုးဖောက်စမ်းသပ်မှုအစီအစဉ်ကို ဖန်တီးရန် တာဝန်ပေးအပ်ထားသော ဆိုက်ဘာလုံခြုံရေးကျွမ်းကျင်ပညာရှင်တစ်ဦးအဖြစ် ဆောင်ရွက်ပါ။ ထိုးဖောက်စမ်းသပ်မှုသည် အဆင့်ငါးဆင့်ဖြစ်သော- ထောက်လှမ်းခြင်း၊ စာရင်းကောက်ခြင်း၊ အသုံးချခြင်း၊ အဆင့်မြှင့်တင်ခြင်းနှင့် နောက်ဆုံးတွင် အစီရင်ခံခြင်းနှင့် ပြုပြင်ခြင်းတို့ကို လိုက်နာရမည်ဖြစ်သည်။

အလုံးစုံပါဝင်သော ထိုးဖောက်စမ်းသပ်မှုအစီအစဉ်သည် စမ်းသပ်မှုဗျူဟာတစ်ခုကို လိုက်နာရမည်ဖြစ်သည်။

### Testing strategy (စမ်းသပ်မှုဗျူဟာ)

#### Step 1: Reconnaissance (အဆင့် ၁: ထောက်လှမ်းခြင်း)

**Techniques**: Gather information about Azure resources, endpoints, and configurations. (နည်းပညာများ- Azure အရင်းအမြစ်များ၊ အဆုံးမှတ်များနှင့် စီစဉ်သတ်မှတ်မှုများအကြောင်း သတင်းအချက်အလက်များ စုဆောင်းပါ။)
**Explanation**: Describe the methods and tools that will be used to gather information about the Azure environment. Explain the importance of this step in understanding potential vulnerabilities and entry points. (ရှင်းလင်းချက်- Azure ပတ်ဝန်းကျင်အကြောင်း သတင်းအချက်အလက်များ စုဆောင်းရန် အသုံးပြုမည့် နည်းလမ်းများနှင့် ကိရိယာများကို ဖော်ပြပါ။ ဖြစ်နိုင်ချေရှိသော အားနည်းချက်များနှင့် ဝင်ရောက်နိုင်သည့်နေရာများကို နားလည်ရန် ဤအဆင့်၏ အရေးပါမှုကို ရှင်းပြပါ။)

#### Step 2: Enumeration (အဆင့် ၂: စာရင်းကောက်ခြင်း)

**Methodology**: Employ automated scanning tools. (နည်းစနစ်- အလိုအလျောက် စကင်ဖတ်စစ်ဆေးသည့် ကိရိယာများကို အသုံးပြုပါ။)
**Vulnerability scanning**: Identify vulnerabilities in Azure resources. (အားနည်းချက် စကင်ဖတ်စစ်ဆေးခြင်း- Azure အရင်းအမြစ်များရှိ အားနည်းချက်များကို ဖော်ထုတ်ပါ။)
**Manual testing**: Manually verify vulnerabilities, configurations, and access controls. (ကိုယ်တိုင်စမ်းသပ်ခြင်း- အားနည်းချက်များ၊ စီစဉ်သတ်မှတ်မှုများနှင့် ဝင်ရောက်ခွင့်ထိန်းချုပ်မှုများကို ကိုယ်တိုင်စစ်ဆေးပါ။)
**Explanation**: Detail the automated scanning tools to be used, the approach for vulnerability scanning, and the manual testing procedures. Emphasize the significance of thorough enumeration in identifying potential weaknesses. (ရှင်းလင်းချက်- အသုံးပြုမည့် အလိုအလျောက် စကင်ဖတ်စစ်ဆေးသည့် ကိရိယာများ၊ အားနည်းချက် စကင်ဖတ်စစ်ဆေးခြင်းအတွက် ချဉ်းကပ်ပုံနှင့် ကိုယ်တိုင်စမ်းသပ်ခြင်း လုပ်ငန်းစဉ်များကို အသေးစိတ်ဖော်ပြပါ။ ဖြစ်နိုင်ချေရှိသော အားနည်းချက်များကို ဖော်ထုတ်ရာတွင် စေ့စေ့စပ်စပ် စာရင်းကောက်ခြင်း၏ အရေးပါမှုကို အလေးပေးပါ။)

#### Step 3: Exploitation (အဆင့် ၃: အသုံးချခြင်း)

**Ethical approach**: Ensure all actions adhere to ethical hacking principles. (ကျင့်ဝတ်ဆိုင်ရာ ချဉ်းကပ်မှု- လုပ်ဆောင်ချက်အားလုံးသည် ကျင့်ဝတ်ဆိုင်ရာ ဟက်ကင်းမူများကို လိုက်နာကြောင်း သေချာပါစေ။)
**Proof of Concept (PoC)**: Exploit vulnerabilities to demonstrate their impact without causing harm. (သဘောတရားသက်သေ (PoC)- ထိခိုက်မှုမဖြစ်စေဘဲ ၎င်းတို့၏အကျိုးသက်ရောက်မှုကို သရုပ်ပြရန် အားနည်းချက်များကို အသုံးချပါ။)
**Exploit frameworks**: Use ethical hacking frameworks to simulate attacks. (အသုံးချမှုမူဘောင်များ- တိုက်ခိုက်မှုများကို သရုပ်တူဖန်တီးရန် ကျင့်ဝတ်ဆိုင်ရာ ဟက်ကင်းမူဘောင်များကို အသုံးပြုပါ။)
**Explanation**: Explain the ethical approach to exploitation, the purpose of PoC, and the frameworks to be utilized. Stress the importance of ethical conduct during this phase. (ရှင်းလင်းချက်- အသုံးချခြင်းအတွက် ကျင့်ဝတ်ဆိုင်ရာ ချဉ်းကပ်မှု၊ PoC ၏ ရည်ရွယ်ချက်နှင့် အသုံးပြုမည့် မူဘောင်များကို ရှင်းပြပါ။ ဤအဆင့်အတွင်း ကျင့်ဝတ်ဆိုင်ရာ လုပ်ဆောင်မှု၏ အရေးပါမှုကို အလေးပေးပါ။)

#### Step 4: Escalation (အဆင့် ၄: အဆင့်မြှင့်တင်ခြင်း)

**Privilege escalation**: Attempt to escalate privileges using known techniques. (အခွင့်အရေးမြှင့်တင်ခြင်း- သိရှိထားသော နည်းပညာများကို အသုံးပြု၍ အခွင့်အရေးများ မြှင့်တင်ရန် ကြိုးစားပါ။)
**Explanation**: Describe the techniques and methods to be employed for privilege escalation. Clarify the significance of assessing the extent to which an attacker can escalate privileges. (ရှင်းလင်းချက်- အခွင့်အရေးမြှင့်တင်ရန်အတွက် အသုံးပြုမည့် နည်းပညာများနှင့် နည်းလမ်းများကို ဖော်ပြပါ။ တိုက်ခိုက်သူတစ်ဦးသည် အခွင့်အရေးများကို မည်သည့်အထိ မြှင့်တင်နိုင်သည်ကို အကဲဖြတ်ခြင်း၏ အရေးပါမှုကို ရှင်းလင်းပါ။)

#### Step 5: Reporting and remediation (အဆင့် ၅: အစီရင်ခံခြင်းနှင့် ပြုပြင်ခြင်း)

**Documentation**: Record all findings, including vulnerabilities and exploitation methods. (မှတ်တမ်းတင်ခြင်း- အားနည်းချက်များနှင့် အသုံးချမှုနည်းလမ်းများအပါအဝင် တွေ့ရှိချက်အားလုံးကို မှတ်တမ်းတင်ပါ။)
**Prioritization**: Prioritize vulnerabilities based on their criticality. (ဦးစားပေးသတ်မှတ်ခြင်း- ၎င်းတို့၏ အရေးပါမှုအပေါ် အခြေခံ၍ အားနည်းချက်များကို ဦးစားပေးသတ်မှတ်ပါ။)
**Recommendations**: Provide recommendations for remediation. (အကြံပြုချက်များ- ပြုပြင်ရန်အတွက် အကြံပြုချက်များ ပေးပါ။)
**Collaboration**: Collaborate with stakeholders to address identified issues. (ပူးပေါင်းဆောင်ရွက်ခြင်း- ဖော်ထုတ်ထားသော ပြဿနာများကို ဖြေရှင်းရန် သက်ဆိုင်သူများနှင့် ပူးပေါင်းဆောင်ရွက်ပါ။)
**Explanation**: Outline the process of documenting findings, prioritizing vulnerabilities, and providing recommendations. Highlight the importance of collaboration with stakeholders for security enhancement. (ရှင်းလင်းချက်- တွေ့ရှိချက်များကို မှတ်တမ်းတင်ခြင်း၊ အားနည်းချက်များကို ဦးစားပေးသတ်မှတ်ခြင်းနှင့် အကြံပြုချက်များပေးခြင်း လုပ်ငန်းစဉ်ကို ဖော်ပြပါ။ လုံခြုံရေးတိုးမြှင့်ရန်အတွက် သက်ဆိုင်သူများနှင့် ပူးပေါင်းဆောင်ရွက်ခြင်း၏ အရေးပါမှုကို အလေးပေးပါ။)

## Conclusion (နိဂုံး)

ဤတာဝန်ကို ပြီးမြောက်ခြင်းဖြင့် သင်သည် ထိုးဖောက်စမ်းသပ်မှု၏ အဆင့်အမျိုးမျိုးကို ခိုင်မာစွာ နားလည်သဘောပေါက်လိမ့်မည်။ သင်၏စာရွက်စာတမ်းသည် အလုံးစုံပါဝင်ပြီး ကောင်းမွန်စွာ ဖွဲ့စည်းထားကြောင်းနှင့် ပစ်မှတ်စနစ်ရှိ အားနည်းချက်များကို ရှာဖွေရန် ယုတ္တိရှိသော လမ်းကြောင်းအတိုင်း လိုက်နာကြောင်း သေချာပါစေ။

ဤနောက်ဆုံးစီမံကိန်းနှင့် အကဲဖြတ်မှုကို ကြိုးစားအားထုတ်ပြီး တီထွင်ဖန်တီးမှုဖြင့် ချဉ်းကပ်ခြင်းဖြင့် သင်သည် ဆိုက်ဘာလုံခြုံရေးကိရိယာများနှင့် နည်းပညာများတွင် သင်၏ကျွမ်းကျင်မှုကို သရုပ်ပြရန်နှင့် White Box ထိုးဖောက်စမ်းသပ်မှုကို ဒီဇိုင်းဆွဲကာ လုပ်ဆောင်နိုင်စွမ်းကို ပြသရန် အခွင့်အရေးကောင်းတစ်ခုကို အသုံးချနိုင်မည်ဖြစ်သည်။

**Note**: It's important to note that conducting penetration testing on this type of infrastructure can lead to increased utilization of Azure resources, resulting in additional costs on your billing. (မှတ်ချက်- ဤကဲ့သို့သော အခြေခံအဆောက်အအုံတွင် ထိုးဖောက်စမ်းသပ်မှုပြုလုပ်ခြင်းသည် Azure အရင်းအမြစ်များ၏ အသုံးပြုမှုတိုးလာစေပြီး သင်၏ငွေတောင်းခံမှုတွင် အပိုကုန်ကျစရိတ်များ ဖြစ်ပေါ်စေနိုင်ကြောင်း သတိပြုရန် အရေးကြီးပါသည်။)
