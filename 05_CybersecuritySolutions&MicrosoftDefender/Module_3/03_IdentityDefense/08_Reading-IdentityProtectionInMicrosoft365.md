# Identity Protection in Microsoft 365

[Identity Protection in Microsoft 365 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/supplement/kR5T6/identity-protection-in-microsoft-365)

# Microsoft 365 တွင် သက်သေခံ ကာကွယ်ရေး (Identity Protection in Microsoft 365)

## မိတ်ဆက် (Introduction)

လက်ရှိ ဒစ်ဂျစ်တယ် အခြေအနေတွင် ဒစ်ဂျစ်တယ် သက်သေခံများကို ကာကွယ်ခြင်းသည် ဦးစားပေးရုံသာမက မဖြစ်မနေ လိုအပ်ပါသည်။ ဆိုက်ဘာ ခြိမ်းခြောက်မှုများနှင့် တိုက်ခိုက်မှုများ တိုးပွားလာခြင်းနှင့်အတူ လုပ်ငန်းများသည် ၎င်းတို့၏ ဒစ်ဂျစ်တယ် ပိုင်ဆိုင်မှုများကို ကာကွယ်ရန် ပြည့်စုံသော ကိရိယာများ လိုအပ်ပါသည်။ ယခုအချိန်အထိ Microsoft 365 သည် သက်သေခံ ကာကွယ်ရေးကို အဓိကထားသည့် ခိုင်မာသော ဝန်ဆောင်မှုများ စုစည်းမှုကို ပေးဆောင်ကြောင်း သင်လေ့လာခဲ့ပြီးဖြစ်သည်။ အထူးသဖြင့် Azure AD Identity Protection, Azure AD Privileged Identity Management နှင့် Azure AD Identity Governance တို့ဖြစ်သည်။ ဤစာဖတ်ခြင်းသည် ဤ အပြန်အလှန်ချိတ်ဆက်ထားသော ဝန်ဆောင်မှုများ၏ အကျဉ်းချုပ်ကို ပေးဆောင်ပြီး ၎င်းတို့သည် သက်သေခံ အခြေခံ ခြိမ်းခြောက်မှုများမှ ကာကွယ်ရန် မည်သို့ အတူတကွ လုပ်ဆောင်ကြောင်းကို ဖော်ပြပေးပါသည်။ Microsoft 365 ပတ်ဝန်းကျင်တွင် သက်သေခံ ကာကွယ်ရေးကို အကောင်အထည်ဖော်ရန်အတွက် အကောင်းဆုံး အလေ့အကျင့်များဆိုင်ရာ တန်ဖိုးရှိသော လမ်းညွှန်ချက်များကိုလည်း သင် ရရှိပါမည်။

## Azure AD Identity Protection

ယခင်က Azure AD Identity Protection သည် အသုံးပြုသူ သက်သေခံများနှင့် ဆက်စပ်နေသော သံသယဖြစ်ဖွယ် လုပ်ဆောင်ချက်များကို ထောက်လှမ်းရန် စက်သင်ယူခြင်းနှင့် heuristic စည်းမျဉ်းများကို အသုံးပြုသည့် အဆင့်မြင့် ခြိမ်းခြောက်မှု ကာကွယ်ရေး ကိရိယာတစ်ခုဖြစ်ကြောင်း သင်လေ့လာခဲ့ပြီးဖြစ်သည်။ ၎င်းသည် အသုံးပြုသူ အန္တရာယ်နှင့် ဝင်ရောက်ခြင်း အန္တရာယ် မူဝါဒ နှစ်ခုလုံးကို ပေးဆောင်ခြင်းဖြင့် ဖြစ်နိုင်ချေရှိသော အားနည်းချက်များကို ဖော်ထုတ်ကာ လျှော့ချပေးပါသည်။

အသုံးပြုသူ အန္တရာယ် မူဝါဒသည် အန္တရာယ်ရှိနိုင်သော အသုံးပြုသူများကို ဖော်ထုတ်ပြီး စကားဝှက် ပြန်လည် သတ်မှတ်ခြင်း သို့မဟုတ် multi-factor authentication စိန်ခေါ်မှုများကဲ့သို့ လိုက်လျောညီထွေဖြစ်သော ပြန်လည် ကုစားခြင်း လုပ်ဆောင်ချက်များကို အသုံးပြုပါသည်။ ဝင်ရောက်ခြင်း အန္တရာယ် မူဝါဒသည် ဝင်ရောက်ခြင်းအတွင်း မူမမှန်မှုများကို ထောက်လှမ်းပြီး ဝင်ရောက်ခွင့် အမှတ်တွင် အန္တရာယ် လျှော့ချခြင်း အဆင့်များကို အသုံးပြုပါသည်။

အောက်ပါပုံသည် Azure AD Identity Protection တွင် အသုံးပြုသူ အန္တရာယ်နှင့် ဝင်ရောက်ခြင်း မူဝါဒများကို မည်သို့ အသုံးပြုကြောင်းကို ညွှန်ပြပါသည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/sogcqxfSRnWv8-eU7jtHcA_ef3f3301291e48c49ebf49228c02dce1_image.png?expiry=1744070400000&hmac=xGKN-IFXtKNOrTZZe_9fgu2YdDJno1kmE-DbHMKSAbU">

## Azure AD Privileged Identity Management

အခွင့်ထူးခံ အကောင့်များနှင့် ဆက်စပ်နေသော ခြိမ်းခြောက်မှုများကို လျှော့ချရန် ရည်ရွယ်သည့် Azure AD Privileged Identity Management (PIM) အကြောင်း သင်လေ့လာခဲ့ပြီးဖြစ်သည်။ ဤ အကောင့်များသည် ၎င်းတို့၏ မြင့်မားသော ခွင့်ပြုချက်များကြောင့် အန္တရာယ်ရှိပါက သိသာထင်ရှားသော လုံခြုံရေး အန္တရာယ်များကို ဖြစ်ပေါ်စေနိုင်သည်။

PIM သည် အမြဲတမ်း စီမံအုပ်ချုပ်ရေး အခွင့်ထူးများကို ထိန်းသိမ်းမည့်အစား အချိန်နှင့်တပြေးညီ အခွင့်ထူးခံ ဝင်ရောက်ခွင့်ကို ပေးဆောင်ပြီး အသုံးပြုသူ အခွင့်အရေးများ ယာယီ မြှင့်တင်ခြင်းကို လုပ်ဆောင်စေပါသည်။ ဤ ချဉ်းကပ်မှုသည် တိုက်ခိုက်မှုများအတွက် မျက်နှာပြင်ဧရိယာကို လျှော့ချပေးပါသည်။

ထို့အပြင် PIM သည် အတည်ပြုခြင်း လုပ်ငန်းစဉ်များ၊ ဝင်ရောက်ခွင့် ပြန်လည်သုံးသပ်ခြင်းများနှင့် စစ်ဆေးခြင်း သမိုင်းကြောင်းမှတစ်ဆင့် ပြည့်စုံသော ကြီးကြပ်မှုကို သေချာစေပါသည်။ ၎င်းသည် အဖွဲ့အစည်းများအား မည်သူက ဝင်ရောက်ခွင့် ရှိသည်၊ အဘယ်ကြောင့်၊ အချိန်နှင့် ၎င်းတို့ လုပ်ဆောင်သည့် လုပ်ဆောင်ချက်များကို ထိန်းချုပ်ရန် ကူညီပေးပါသည်။

## Azure AD Identity Governance

Azure AD Identity Governance သည် အဖွဲ့အစည်းတစ်လျှောက် သက်သေခံ သက်တမ်းနှင့် ဝင်ရောက်ခွင့်ကို စီမံခန့်ခွဲရာတွင် အထောက်အကူပြုပါသည်။ ၎င်းသည် ဝင်ရောက်ခွင့် ပြန်လည်သုံးသပ်ခြင်းများ၊ ဝင်ရောက်ခွင့် ပက်ကေ့ခ်ျများ၊ အခွင့်ထူးခံ ဝင်ရောက်ခွင့်နှင့် ခံစားခွင့် စီမံခန့်ခွဲမှုအတွက် ပြည့်စုံသော ဖြေရှင်းချက်များကို ပေးဆောင်ပါသည်။

ဝင်ရောက်ခွင့် ပြန်လည်သုံးသပ်ခြင်းများသည် သင့်လျော်သော လူများသာ အရင်းအမြစ်များကို သင့်လျော်သော ဝင်ရောက်ခွင့် ရှိကြောင်း သေချာစေပါသည်။ ဝင်ရောက်ခွင့် ပက်ကေ့ခ်ျများသည် အဖွဲ့များ၊ အက်ပ်များနှင့် ဆိုက်များသို့ ဝင်ရောက်ခွင့် တောင်းဆိုခြင်း၊ အတည်ပြုခြင်းနှင့် စီမံခန့်ခွဲခြင်း လုပ်ငန်းစဉ်ကို ရိုးရှင်းစေပါသည်။ အခွင့်ထူးခံ ဝင်ရောက်ခွင့်သည် အခန်းကဏ္ဍများကို သီးခြား ကာလတစ်ခုအတွက်သာ ပေးအပ်ကြောင်းနှင့် အတည်ပြုခြင်း လိုအပ်ကြောင်း သေချာစေပါသည်။ ခံစားခွင့် စီမံခန့်ခွဲမှုသည် ဝင်ရောက်ခွင့် တောင်းဆိုမှု လုပ်ငန်းစဉ်များကို အလိုအလျောက် လုပ်ဆောင်ပြီး လက်ဖြင့် လုပ်ဆောင်ရမည့် ဝန်ထုပ်ဝန်ပိုးကို အနည်းဆုံးဖြစ်အောင် လုပ်ဆောင်ကာ တသမတ်တည်း ဆုံးဖြတ်ချက်ချခြင်းကို သေချာစေပါသည်။

## ဝန်ဆောင်မှုများ ပေါင်းစည်းခြင်း (Integration of services)

Microsoft 365 ရှိ ဤ ဝန်ဆောင်မှုများသည် သီးခြား အဖွဲ့အစည်းများ မဟုတ်ဘဲ ခိုင်မာစွာ ပေါင်းစည်းထားသော နည်းလမ်းဖြင့် လုပ်ဆောင်ပါသည်။ Azure AD Identity Protection သည် ဖြစ်နိုင်ချေရှိသော သက်သေခံ ခြိမ်းခြောက်မှုများကို ထောက်လှမ်းကာ လျှော့ချသည့် ပထမဆုံး ကာကွယ်ရေးလိုင်းဖြစ်သည်။ ၎င်းသည် ဖော်ထုတ်ထားသော အန္တရာယ်များအပေါ် အခြေခံ၍ အခွင့်ထူးခံ ဝင်ရောက်ခွင့်ကို စီမံခန့်ခွဲကာ စစ်ဆေးသည့် Azure AD Privileged Identity Management သို့ အန္တရာယ် အချက်အလက်ကို ပေးပို့ပါသည်။ Azure AD Identity Governance သည် ဝင်ရောက်ခွင့် အခွင့်အရေးများကို စီမံခန့်ခွဲကာ ထိန်းညှိရန် ဤဒေတာကို အသုံးပြုပြီး သက်သေခံနှင့် ဝင်ရောက်ခွင့် စီမံခန့်ခွဲမှုအတွက် ပိတ်ထားသော ကွင်းဆက် စနစ်ကို သေချာစေပါသည်။

## သက်သေခံ ကာကွယ်ရေး အကောင်အထည်ဖော်ရန် အကောင်းဆုံး အလေ့အကျင့်များ (Best practices for implementing Identity Protection)

Microsoft 365 ပတ်ဝန်းကျင်တွင် ဤ ဝန်ဆောင်မှုများကို အကောင်းဆုံးဖြစ်အောင် လုပ်ဆောင်ရန် အောက်ပါ အကောင်းဆုံး အလေ့အကျင့်များကို ထည့်သွင်းစဉ်းစားပါ။

- ပြည့်စုံသော အန္တရာယ် မူဝါဒများကို အကောင်အထည်ဖော်ပါ- ဖြစ်နိုင်ချေရှိသော အန္တရာယ် အခြေအနေအားလုံးကို အကျုံးဝင်စေရန် Azure AD Identity Protection တွင် အသုံးပြုသူနှင့် ဝင်ရောက်ခြင်း အန္တရာယ် မူဝါဒ နှစ်ခုလုံးကို လုပ်ဆောင်ပါ။
- အနည်းဆုံး အခွင့်ထူး၏ အခြေခံမူ (PoLP) ကို အသုံးပြုပါ- အချိန်နှင့်တပြေးညီနှင့် လိုအပ်သလောက်သာ ဝင်ရောက်ခွင့် အခြေခံမူကို အကောင်အထည်ဖော်ရန် Azure AD PIM ကို အသုံးပြုပါ။ လိုအပ်သည့်အခါနှင့် လိုအပ်သော ကြာချိန်နှင့် ဝင်ရောက်ခွင့် အဆင့်အတွက်သာ စီမံအုပ်ချုပ်ရေး အခွင့်ထူးများကို ပေးအပ်ပါ။
- ပုံမှန် ဝင်ရောက်ခွင့် ပြန်လည်သုံးသပ်ခြင်းများကို လုပ်ဆောင်ပါ- ပုံမှန် ဝင်ရောက်ခွင့် ပြန်လည်သုံးသပ်ခြင်းများကို လုပ်ဆောင်ကာ မလိုအပ်သော ခံစားခွင့်များကို ချက်ချင်း ဖယ်ရှားရန် Azure AD Identity Governance ကို အသုံးပြုပါ။
- multi-factor authentication ကို လုပ်ဆောင်ပါ- သက်သေခံ အန္တရာယ်မှ ကာကွယ်မှုကို မြှင့်တင်ရန် သင့်အဖွဲ့အစည်းတစ်လျှောက်လုံး multi-factor authentication ကို အတည်ပြုကြောင်း သေချာပါစေ။
- အသုံးပြုသူများကို ပညာပေးပါ- လူသားတို့၏ အမှားသည် သက်သေခံ အန္တရာယ်ကို မကြာခဏ ဖြစ်ပေါ်စေနိုင်သောကြောင့် သင်၏ အသုံးပြုသူများကို လုံခြုံရေး အသိပညာပေးခြင်းဆိုင်ရာ ပုံမှန် လေ့ကျင့်ပေးပါ။
- စောင့်ကြည့်ပြီး လုပ်ဆောင်ပါ- စစ်ဆေးခြင်း မှတ်တမ်းများနှင့် အန္တရာယ် ဖြစ်ရပ်များကို ပုံမှန် ပြန်လည်သုံးသပ်ပါ။ သံသယဖြစ်ဖွယ် လုပ်ဆောင်ချက်များအပေါ် လျင်မြန်စွာ လုပ်ဆောင်ပါ။

## နိဂုံး (Conclusion)

Microsoft 365 သည် Azure AD Identity Protection, Azure AD Privileged Identity Management နှင့် Azure AD Identity Governance တို့ဖြင့် သက်သေခံ ကာကွယ်ရေးအတွက် ပြည့်စုံသော၊ ပေါင်းစည်းထားသော ဖြေရှင်းချက်ကို ပေးဆောင်ပါသည်။ ဤ ကိရိယာများကို နားလည်ခြင်း၊ ၎င်းတို့ကို ထိရောက်စွာ အကောင်အထည်ဖော်ခြင်းနှင့် အကောင်းဆုံး အလေ့အကျင့်များကို လိုက်နာခြင်းဖြင့် အဖွဲ့အစည်းများသည် သက်သေခံ အခြေခံ ခြိမ်းခြောက်မှုများနှင့် တိုက်ခိုက်မှုများမှ ၎င်းတို့၏ ကာကွယ်ရေးကို သိသိသာသာ မြှင့်တင်နိုင်ပြီး လုံခြုံသော ဒစ်ဂျစ်တယ် ပတ်ဝန်းကျင်ကို သေချာစေပါသည်။
