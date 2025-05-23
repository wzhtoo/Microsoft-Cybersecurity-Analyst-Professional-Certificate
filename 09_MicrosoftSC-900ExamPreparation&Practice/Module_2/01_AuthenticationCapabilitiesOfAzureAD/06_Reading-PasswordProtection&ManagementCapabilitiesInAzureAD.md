# Password protection and management capabilities in Azure AD

[Password protection and management capabilities in Azure AD 🔗](https://www.coursera.org/learn/microsoft-sc-900-exam-preparation-and-practice/supplement/j0yMS/password-protection-and-management-capabilities-in-azure-ad)

# Azure AD တွင် စကားဝှက် ကာကွယ်ရေးနှင့် စီမံခန့်ခွဲမှု စွမ်းရည်များ

## Introduction (နိဒါန်း)

ယခုအချိန်အထိ၊ လုံခြုံရေး ကျွမ်းကျင်သူများသည် အတည်ပြုခြင်း၏ အဓိကနည်းလမ်းအဖြစ် စကားဝှက်များကို အသုံးပြုခြင်းမှ ရွေ့လျားခဲ့ကြောင်း သင်လေ့လာခဲ့ပြီးဖြစ်သည်။ ၎င်းတို့ကို ရှောင်ကွင်းရန်အတွက် ခေတ်မီ ဟက်ခ်များ တိုးတက်ပြောင်းလဲလာခဲ့ပြီး ၎င်းတို့၏ အသုံးပြုမှုသည် အသုံးပြုသူတစ်ဦးကို အတည်ပြုရန် အခြားနည်းလမ်းများ လိုအပ်လာစေသည်။

အသုံးပြုသူ၏ အချက်အလက်များမှ စကားဝှက်များကို ဝင်ရောက်ရန် ကြိုးစားရန် လူများက ဖိရှ်တိုက်ခိုက်မှုများကို လုပ်ဆောင်ရန် ဆိုရှယ်မီဒီယာကို မည်သို့ အသုံးပြုကြောင်းကို စဉ်းစားပါ။ ဤလမ်းကြောင်းသည် ဆက်လက်တည်ရှိနေပြီး၊ ထို့ကြောင့် စကားဝှက်များကိုသာ အားကိုးရန် မလုံခြုံပါ။ ရလဒ်အနေဖြင့်၊ အချက်အလက်ပေါင်းစုံ အတည်ပြုခြင်း (MFA) ကဲ့သို့သော လုံခြုံရေးနည်းလမ်းများစွာကို ယခုရရှိနိုင်ပြီဖြစ်ပြီး၊ ၎င်းသည် စကားဝှက်အတွက် အခြား အတည်ပြုခြင်းပုံစံတစ်ခု လိုအပ်ပါသည်။ ထို့အပြင်၊ ခိုင်မာသော စကားဝှက်များ ဖန်တီးရန်အတွက် အကောင်းဆုံး အလေ့အကျင့်များစွာလည်း ရှိပါသည်။

ဤစာဖတ်ခြင်းတွင်၊ စကားဝှက်များကို နက်ရှိုင်းစွာ လေ့လာပါမည်။ Azure AD စကားဝှက် ကာကွယ်ရေးနှင့် Azure စကားဝှက် ကာကွယ်ရေး ပရောက်စီကဲ့သို့သော တန်ဖိုးရှိသော ဝန်ဆောင်မှုများကို သင် ရှာဖွေတွေ့ရှိပါမည်။ သင်၏ စကားဝှက်သည် ရှုပ်ထွေးရန် မည်မျှ အရေးကြီးကြောင်း စကားဝှက် ဖြန်းခြင်းဆိုသည်ကိုလည်း သင်လေ့လာပါမည်။ ထို့အပြင်၊ ကမ္ဘာလုံးဆိုင်ရာနှင့် စိတ်ကြိုက် စကားဝှက်စာရင်းကို ထိန်းသိမ်းခြင်းအကြောင်းကိုလည်း သင်လေ့လာပါမည်။

## Azure AD Password Protection (Azure AD စကားဝှက် ကာကွယ်ရေး)

IT အဖွဲ့များနှင့် အချို့သော စိတ်ပါဝင်စားသည့် အဖွဲ့ဝင်များသည် စကားဝှက်ရွေးချယ်မှုတွင် အကောင်းဆုံး အလေ့အကျင့်များကို အသုံးပြုနိုင်သော်လည်း လူတိုင်းသည် ၎င်းကို လိုက်နာမည်ဟု သင် မယူဆနိုင်ပါ။ ထို့ကြောင့်၊ Azure Active Directory (AD) တွင် Azure AD စကားဝှက် ကာကွယ်ရေးဟုခေါ်သော အင်္ဂါရပ်တစ်ခုရှိပြီး၊ ၎င်းသည် ရွေးချယ်ထားသော စကားဝှက်များကို ခွဲခြမ်းစိတ်ဖြာခြင်းနှင့် စစ်ဆေးခြင်းဖြင့် ညံ့ဖျင်းသော စကားဝှက် ဖန်တီးခြင်း၏ အန္တရာယ်ကို လျှော့ချပေးပါသည်။ ၎င်းသည် သိရှိထားသော အားနည်းသော စကားဝှက်များနှင့် ၎င်းတို့၏ အမျိုးကွဲများကို ရှာဖွေတွေ့ရှိပြီး ပိတ်ဆို့သည်။ ဤနေရာတွင်၊ အားနည်းသော စကားဝှက်ကို 'စကားဝှက်' သို့မဟုတ် 'qwerty123' ကဲ့သို့သော အသုံးများသော စကားဝှက်များ သို့မဟုတ် ထုတ်ကုန် သို့မဟုတ် ဝန်ဆောင်မှု၏ အမည်ကဲ့သို့သော အဖွဲ့အစည်းဆိုင်ရာ သီးခြား စကားဝှက်များအဖြစ် သတ်မှတ်သည်။

Azure AD စကားဝှက် ကာကွယ်ရေးကို အသုံးပြုသောအခါ၊ ရွေးချယ်ထားသော မည်သည့် စကားဝှက်ကိုမဆို ပထမဦးစွာ တားမြစ်ထားသော စကားဝှက်များ၏ ကမ္ဘာလုံးဆိုင်ရာ စာရင်းနှင့် နှိုင်းယှဉ်ပါသည်။ Microsoft ၏ ခြိမ်းခြောက်မှုဆိုင်ရာ ထောက်လှမ်းရေး အချက်အလက်နှင့် လုံခြုံရေး သုတေသန အဖွဲ့များသည် တားမြစ်ထားသော စကားဝှက်များကို ဆုံးဖြတ်ရန် နည်းလမ်းများစွာကို အသုံးပြုသည့် ကမ္ဘာလုံးဆိုင်ရာ တားမြစ်ထားသော စကားဝှက်စာရင်းကို စုစည်းပါသည်။ ဤချဉ်းကပ်မှုများတွင်-

- ကြီးမားသော ချိုးဖောက်မှုများမှ စကားဝှက်များကို ထုတ်ယူသည့် လုံခြုံရေး ချိုးဖောက်မှုများ။
- လူများ ရွေးချယ်လေ့ရှိသော အသုံးများသော ပုံစံများကို ထင်ဟပ်သည့် အသုံးများသော စကားဝှက် ပုံစံများ။ ၎င်းတွင် ‘o’ အတွက် ‘0’ သို့မဟုတ် ‘i’ အတွက် ‘1’ ကဲ့သို့သော လူများ အသုံးများနိုင်သည့် အချို့သော ကွဲပြားမှုများကို ခွဲခြားသတ်မှတ်ခြင်း ပါဝင်သည်၊ ဥပမာ- passw0rd သို့မဟုတ် emp1re။
- လုံခြုံရေး အစီရင်ခံစာများနှင့် အသုံးပြုသူ အပြုအမူ အစီရင်ခံစာများ၊ လုံခြုံရေး အစီရင်ခံစာများနှင့် အသုံးပြုသူ အပြုအမူ လမ်းကြောင်းများကို ခွဲခြမ်းစိတ်ဖြာခြင်း ပါဝင်ပြီး ၎င်းတို့ကို တားမြစ်ထားသော စာရင်းထဲသို့ ထည့်သွင်းခြင်း၏ သက်သာစေသည့် အဆင့်ကို လုပ်ဆောင်သည်။

# Azure Active Directory ၏ စိတ်ကြိုက် စကားဝှက်စာရင်း

Azure AD သည် သင့်အား အဖွဲ့အစည်း သို့မဟုတ် ဒေသဆိုင်ရာ သီးခြားဖြစ်သော စိတ်ကြိုက် စကားဝှက်စာရင်းကို ဖန်တီးရန်လည်း ခွင့်ပြုပါသည်။ ဥပမာအားဖြင့်၊ အိုင်ယာလန်အခြေစိုက် အဖွဲ့အစည်းတစ်ခုသည် leprechaun၊ clover သို့မဟုတ် lucky ကဲ့သို့သော ဝေါဟာရများကို ရှောင်ရှားနိုင်ပါသည်။ ထို့နောက် ခွင့်ပြုနိုင်သော အချက်များမှာ-

- အမှတ်တံဆိပ် အမည်များ
- ထုတ်ကုန် အမည်များ
- ကုမ္ပဏီဌာနချုပ်ကဲ့သို့သော တည်နေရာများ
- ကုမ္ပဏီဆိုင်ရာ အတွင်းပိုင်း ဝေါဟာရများ
- သီးခြား ကုမ္ပဏီ အဓိပ္ပာယ်ရှိသော အတိုကောက်များ

နောက်ဆုံးတွင်၊ သင်၏ အရင်းအမြစ်များကို ဘေးကင်းစေရန်အတွက် အချက်အလက်ပေါင်းစုံ အတည်ပြုခြင်းကို အသုံးပြုရန် အကောင်းဆုံး အလေ့အကျင့်များက အမိန့်ပေးပါသည်။ တားမြစ်ထားသော စကားဝှက်များသည် Azure AD Premium 1 သို့မဟုတ် 2 လိုင်စင်များအတွက်သာ ရရှိနိုင်သော အင်္ဂါရပ်တစ်ခုဖြစ်သည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/WjQtflXuQI2p4cLiJXjWyw_9d6f256490494eb59c0b9003346c56e1_C9M2L1_item06_img01.png?expiry=1744502400000&hmac=FWUvhDEf_5_OAIJLGBMJakRLpFb1oDGhK4JKXR5s-0k">

ဤကာကွယ်ရေး အစီအမံများကို အသုံးပြုခြင်းသည် စကားဝှက် ဖြန်းခြင်းကို သက်သာစေရန် ကူညီပေးပါသည်။ ဤအသုံးချမှုသည် တရားဝင် အသုံးပြုသူ အကောင့်အမည်များဖြင့် အသုံးအများဆုံး စကားဝှက်များကို ရွေးချယ်ပြီး ကြိုးစားသည်။ တားမြစ်ထားသော စကားဝှက်စာရင်းကို ဖန်တီးခြင်းသည် ဤအသုံးချမှု ထိရောက်နိုင်ခြေကို လျှော့ချပေးသည်။ ၎င်းကို အနီးကပ် စောင့်ကြည့်ခြင်းနှင့် ပေါင်းစပ်ခြင်းဖြင့် အချိန်တိုအတွင်း များပြားလှသော ဝင်ရောက်ခြင်း ကြိုးပမ်းမှုများကဲ့သို့သော ပုံမှန်မဟုတ်သော လုပ်ဆောင်ချက်ကို ခွဲခြားသတ်မှတ်ပေးပါသည်။ မည်သို့ပင်ဆိုစေကာမူ၊ တိုက်ခိုက်သူသည် အသုံးပြုသူများ အမြဲတမ်း သတိထားရန် အရေးကြီးသောကြောင့် ထောက်လှမ်းခြင်း အနိမ့်ဆုံးအောက်တွင် ရှိနေစေရန် အဖွဲ့အစည်းရှိ အမည်များအားလုံးအတွက် အသုံးများသော စကားဝှက်များကို အကြိမ်အနည်းငယ် ကြိုးစားပါမည်။

## Azure Password Protection Proxy (Azure စကားဝှက် ကာကွယ်ရေး ပရောက်စီ)

Azure စကားဝှက် ကာကွယ်ရေးသည် cloud-based အင်္ဂါရပ်တစ်ခုဖြစ်သည်။ ၎င်းသည် on-premises ကွန်ရက်တွင် အသုံးပြုသည့် စကားဝှက် ဖြန်းခြင်းကို သက်သာစေရန် မလုပ်ဆောင်ပါ။ သို့သော် ဟိုက်ဘရစ် ပတ်ဝန်းကျင်တွင် လည်ပတ်နေသော အသုံးပြုသူများအတွက် တိုးချဲ့နိုင်သည်။ Azure စကားဝှက် ကာကွယ်ရေး၏ ဥပမာတစ်ခုကို on-premises ဆာဗာတွင် ထည့်သွင်းနိုင်သည်။ ၎င်းကို Azure စကားဝှက် ကာကွယ်ရေး ပရောက်စီဟု ရည်ညွှန်းသည်။ ၎င်း၏ အခန်းကဏ္ဍမှာ Azure AD စကားဝှက်များနှင့် on-premises AD စကားဝှက်များကြား တံတားအဖြစ် လုပ်ဆောင်ခြင်း၊ စာရင်းများသို့ ပြောင်းလဲမှုများကို ပေးပို့ခြင်းနှင့် အသုံးပြုသည့် မည်သည့် စိတ်ကြိုက် စာရင်းများကိုမဆို အကြောင်းကြားခြင်းဖြစ်သည်။ ထို့ကြောင့် ၎င်း၏ အခန်းကဏ္ဍမှာ on-premises တွင် တူညီသော စကားဝှက် လုပ်ထုံးလုပ်နည်းကို အတင်းအကြပ် လုပ်ဆောင်ရန်ဖြစ်သည်။

## Conclusion (နိဂုံး)

ဤစာဖတ်ခြင်းတွင်၊ သင်၏ ဒိုမိန်း၏ တစ်ခုတည်းသော တံခါးစောင့်အဖြစ် စကားဝှက်များကို အသုံးပြုခြင်းမှ ဖြစ်ပေါ်လာသော ပြဿနာများကို သရုပ်ဖော်ခြင်းဖြင့် စကားဝှက်မဲ့ အတည်ပြုခြင်းသို့ အဘယ်ကြောင့် ရွေ့လျားခဲ့ကြောင်း သင် နားလည်ပါပြီ။ စကားဝှက်ရွေးချယ်မှုကို စောင့်ကြည့်ခြင်း၊ စကားဝှက် ယိုစိမ့်မှုများအတွက် ဝဘ်ကို စောင့်ကြည့်ခြင်းနှင့် လုံခြုံရေး အစီရင်ခံစာများ ထုတ်ပေးရန်အတွက် အသုံးပြုသူ အပြုအမူကို ခွဲခြမ်းစိတ်ဖြာခြင်းဖြင့် Azure စကားဝှက် ကာကွယ်ရေး ဝန်ဆောင်မှုသည် အချို့သော ကာကွယ်ရေး အဆင့်ကို မည်သို့ ပေးဆောင်ကြောင်းကိုလည်း သင်လေ့လာခဲ့သည်။
