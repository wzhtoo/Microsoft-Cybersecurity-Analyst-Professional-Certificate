# Exemplar: Identify and respond

[Exemplar: Identify and respond 🔗](https://www.coursera.org/learn/cybersecurity-management-and-compliance/supplement/TNNUm/exemplar-identify-and-respond)

# Exemplar: Identify and respond (စံနမူနာ- ခွဲခြားသတ်မှတ်ပြီး တုံ့ပြန်ပါ)

## Overview (အကျဉ်းချုပ်)

လေ့ကျင့်ခန်းတွင်၊ သင်သည် အတွင်းလူခြိမ်းခြောက်မှုကို ရှာဖွေပြီး တားဆီးရန် တာဝန်ပေးအပ်ခံခဲ့ရသည်။ အထူးသဖြင့်၊ Azure Blob Storage မှတစ်ဆင့် အတွင်းလူခြိမ်းခြောက်မှုကို သရုပ်တူဖန်တီးခြင်းဖြင့် စတင်သည့် အဆင့်များကို သင်ပြီးမြောက်ခဲ့ပြီး၊ ထို့နောက် Azure Security Center နှင့် Azure Sentinel မှတစ်ဆင့် ခြိမ်းခြောက်မှုရှာဖွေခြင်းနှင့် ကာကွယ်ခြင်းတို့ကို အကောင်အထည်ဖော်ခဲ့သည်။

အောက်တွင်၊ Azure ၏ လုံခြုံရေးဖြေရှင်းနည်းများဖြင့် အတွင်းလူခြိမ်းခြောက်မှုများကို ရှာဖွေပြီး တားဆီးရန် ဖြစ်နိုင်ချေရှိသော ဖြေရှင်းနည်းကို သင်တွေ့လိမ့်မည်။

## Exemplar (စံနမူနာ)

**Step 1: Set up the scenario (အခြေအနေကို သတ်မှတ်ပါ)**
Azure Blob Storage အကောင့်တစ်ခု ဖန်တီးခဲ့သည်။ ဤလေ့ကျင့်ခန်းအတွက်၊ အကောင့်အမည်မှာ "internal-threat-lab" ဖြစ်သည်။
ဖိုင်အမည် "employee_data.csv" ပါရှိသော အတုအယောင် အရေးကြီးဒေတာအချို့ကို sensitive-data container သို့ အပ်လုဒ်လုပ်ခဲ့သည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/DUFd3cVaTvCGLQhPlj3oyQ_9001c292e9c3450eacfadcce9f0425e1_C7M2L2_item09_img01.png?expiry=1744329600000&hmac=bh1wB2ygxAScXCvhGVPXJymh8Xv_15Jb8OR_jOShtkY">

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/xYVQ5UDLQBeGV1M9BNhbqw_8cbd83dc425b4bfbb9e665e75c6bebe1_C7M2L2_Itm09_Img02.PNG?expiry=1744329600000&hmac=xrXgnD-sQFT0jNy0MXNoT0HqScrsDq4pf5vaA0unsWI">

**Step 2: Simulate the insider threat (အတွင်းလူခြိမ်းခြောက်မှုကို သရုပ်တူဖန်တီးပါ)**
Azure Blob Storage သို့ ဖတ်ခွင့်ရရှိထားသော သီးခြား Azure အသုံးပြုသူအကောင့်တစ်ခု ဖန်တီးခဲ့သည်။
ထို့နောက် IP လိပ်စာ 192.168.1.105 ကဲ့သို့သော IP လိပ်စာတစ်ခုမှ ဝင်ရောက်ကြည့်ရှုခြင်းကို လုပ်ဆောင်ခဲ့ပြီး၊ သင်သည် employee_data.csv ဖိုင်ကို ဝင်ရောက်ကြည့်ရှုပြီး ဒေါင်းလုဒ်လုပ်ခဲ့သည်။

**Step 3: Set up Azure Security Center (Azure Security Center ကို သတ်မှတ်ပါ)**
ထို့နောက် မြှင့်တင်ထားသော လုံခြုံရေးစွမ်းရည်များအတွက် Azure Security Center ၏ Standard အဆင့်ကို အသက်သွင်းခဲ့သည်။
လုံခြုံရေးမူဝါဒအောက်တွင်၊ Data Storage Access စောင့်ကြည့်ခြင်းသည် တက်ကြွနေကြောင်း သင်အတည်ပြုခဲ့သည်။
Blob Storage နှင့်သက်ဆိုင်သော Security Center ၏ အကြံပြုချက်များကို ပြန်လည်သုံးသပ်ခဲ့သည်။ ထို့နောက် Blob Storage ရှိ ဖြစ်နိုင်ချေရှိသော ခြိမ်းခြောက်မှုများကို ရှာဖွေရန် Azure Defender for Storage ကို အသက်သွင်းခဲ့သည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/MRNCculXQGums2b3IuMEqA_ece68f6cbd6e44c88c8c2634041632e1_C7M2L2_item09_img03.png?expiry=1744329600000&hmac=ve5kBNAWM3GZ-UkuGoZEglewWTotY2E-3d5qN7xEu24">
<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/CdNiuH0_T-ebNcUdmcewpg_f1830982e6594c0991df4db5d0f214e1_C7M2L2_Itm09_Img04.PNG?expiry=1744329600000&hmac=wBiWh9WEGJLbKKwGMlk94nEJ7Ock3l0HghIVJHYE9IE">

**Step 4: Setting up Azure Sentinel (Azure Sentinel ကို သတ်မှတ်ပါ)**
ထို့နောက် Azure Sentinel ကို အသုံးချပြီး ပေါ်တယ်တွင် ၎င်းကို အသက်သွင်းခဲ့သည်။
ဒေတာအရင်းအမြစ်များကို ချိတ်ဆက်ပြီး Azure Activity Log သည် သင်၏အရင်းအမြစ်များရှိ မည်သည့်လုပ်ဆောင်ချက်ကိုမဆို ခြေရာခံရန် အဆင်သင့်ဖြစ်ကြောင်း သေချာစေခဲ့သည်။
ပုံမှန်မဟုတ်သော ဒေတာထုတ်ယူမှုပုံစံများကို ရှာဖွေရန် Detection templates ကို အသက်သွင်းခဲ့သည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/FnGYh9uzSly5aoa5G9-0bQ_9f2018c1e71f41648f3fc72f43e39ce1_C7M2L2_Itm09_Img05.PNG?expiry=1744329600000&hmac=hKnrKoqC_T6C7Msva_nbw7Qx3cTbbLaHf_TOok1xpe4">

**Step 5: Detecting the insider threat (အတွင်းလူခြိမ်းခြောက်မှုကို ရှာဖွေခြင်း)**
ဤအဆင့်တွင်၊ Azure Security Center ၏ သတိပေးချက်များကို စစ်ဆေးခဲ့သည်။ ဒေါင်းလုဒ်လုပ်ရန် ကြိုးစားမှုကြောင့် "Access to a large amount of items" ဟု အမည်ပေးထားသော သတိပေးချက်တစ်ခု စတင်ခဲ့သည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Xzm-pb4GTgiysAGrwrb3kg_53e6a2ecb20b46b9b1d4a7e2d2da96e1_C7M2L2_Itm09_Img06.PNG?expiry=1744329600000&hmac=kY-EG7y3xwvIMOBydGO9IOAAwn-IM1l9gC-mJ7voEmE">

ထို့နောက် Azure Sentinel တွင် ဖြစ်ရပ်များကို ပြန်လည်သုံးသပ်ခဲ့သည်။ ပုံမှန်မဟုတ်သော ဒေတာဒေါင်းလုဒ်ပုံစံများကို ညွှန်ပြသော ဖြစ်ရပ်တစ်ခုကို တွေ့ရှိခဲ့ပြီး Medium severity level ဖြင့် တဂ်လုပ်ခဲ့သည်။ ဆက်စပ်အသုံးပြုသူ testuser@company.com နှင့် IP 192.168.1.105 တို့ကို ခွဲခြားသတ်မှတ်ခဲ့သည်။

[ပုံ- Azure Sentinel တွင် တွေ့ရှိခဲ့သော ပုံမှန်မဟုတ်သော ဒေတာဒေါင်းလုဒ်ပုံစံများကို ညွှန်ပြသော ဖြစ်ရပ်ကို ပြသသည့် မျက်နှာပြင်ဓာတ်ပုံ]

**Step 6: Prevention steps (ကာကွယ်ရေးအဆင့်များ)**
အသုံးပြုသူများအား အကန့်အသတ်ရှိသောအချိန်အတွက် Blob Storage သို့ ဝင်ရောက်ခွင့်တောင်းခံရန် ခွင့်ပြုရန် Just-In-Time (JIT) VM Access ကို စီစဉ်သတ်မှတ်ခဲ့သည်။ ဤကိစ္စတွင်၊ ၎င်းသည် testuser@company.com အတွက် ၁ နာရီကြာ ၀ င်ရောက်ခွင့်ကို ပေးအပ်ခြင်းဖြစ်သည်။
ထို့နောက် အသေးစိတ် Blob Storage Permissions ကို သတ်မှတ်ခဲ့သည်။ ဤနေရာတွင်၊ testuser@company.com အား public-data container သို့ ဝင်ရောက်ခွင့်ပေးပြီး sensitive-data သို့ ဝင်ရောက်ခွင့်ကို ရုပ်သိမ်းရန် ခွင့်ပြုချက်များကို ပြောင်းလဲခဲ့သည်။
ထို့နောက်၊ Blob Storage အားလုံးတွင် Azure Defender ကို ဖွင့်ထားကြောင်း သေချာစေရန် Azure Policy တစ်ခုကို ဖန်တီးပြီး အတင်းအကျပ်လုပ်ဆောင်ခဲ့သည်။

**Take time to reflect (ပြန်လည်သုံးသပ်ရန် အချိန်ယူပါ)**

1.  **Key Indicators (အဓိကညွှန်းကိန်းများ)**

    - ဒေတာကို လျင်မြန်စွာနှင့် အမြောက်အမြား ဒေါင်းလုဒ်လုပ်ခြင်းသည် သံသယဖြစ်ဖွယ်အချက်ဖြစ်သည်။
    - ဝင်ရောက်မှုပုံစံသည် ပုံမှန်အသုံးပြုသူ၏ အပြုအမူနှင့် မကိုက်ညီပါ။

2.  **Swift Detection Measures (လျင်မြန်သော ရှာဖွေတွေ့ရှိမှု အစီအမံများ)**
    - Azure Security Center နှင့် Azure Sentinel ကို ပေါင်းစည်းခြင်းဖြင့် ပုံမှန်မဟုတ်သော အပြုအမူကို ချက်ချင်း ရှာဖွေတွေ့ရှိနိုင်ခဲ့သည်။
    - လက်တွေ့ကမ္ဘာတွင်၊ အဖွဲ့အစည်းများသည် ခွင့်ပြုချက်များကို ပုံမှန်ပြန်လည်သုံးသပ်ပြီး ချိန်ညှိသင့်သည်၊ အသုံးပြုသူ၏ အပြုအမူများကို စောင့်ကြည့်သင့်ပြီး၊ လုံခြုံရေးအစီအမံများအကြောင်း ဝန်ထမ်းများကို အဆက်မပြတ် ပညာပေးသင့်သည်။

**Conclusion (နိဂုံး)**
ဤလေ့ကျင့်ခန်းတွင်၊ သရုပ်တူဖန်တီးထားသော အတွင်းလူခြိမ်းခြောက်မှုကို အောင်မြင်စွာ ရှာဖွေတွေ့ရှိခြင်းနှင့် Azure ၏ လုံခြုံရေးအင်္ဂါရပ်များကို အသုံးပြု၍ ထိုကဲ့သို့သော ပြဿနာများကို လျှော့ချရန် အဆင့်များကို သရုပ်ပြသည့် ဖြစ်နိုင်ချေရှိသော ဖြေရှင်းနည်းကို သင်ပြန်လည်သုံးသပ်ခဲ့သည်။ လုပ်ဆောင်ခဲ့သော လုပ်ဆောင်ချက်တစ်ခုစီ၏ သီးခြားအချက်အလက်များနှင့် လုပ်ဆောင်ချက်အကောင်အထည်ဖော်စဉ်အတွင်း ပေါ်ပေါက်လာနိုင်သည့် ကွဲလွဲချက်များနှင့်အညီ ဤစံနမူနာကို လိုက်လျောညီထွေဖြစ်စေရန် အရေးကြီးပါသည်။
