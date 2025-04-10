# Exemplar: Evaluating threats

[Exemplar: Evaluating threats 🔗](https://www.coursera.org/learn/advanced-cybersecurity-concepts-and-capstone-project/supplement/p3FDA/exemplar-evaluating-threats)

# Exemplar: Evaluating threats (နမူနာ: ခြိမ်းခြောက်မှုများ အကဲဖြတ်ခြင်း)

## Introduction (နိဒါန်း)

လေ့ကျင့်ခန်း ခြိမ်းခြောက်မှုများ အကဲဖြတ်ခြင်း

တွင် သင်သည် Sam's Scoops firewall ရှိ စိတ်ကူးယဉ် လုံခြုံရေးဆိုင်ရာ အားနည်းချက်တစ်ခု၏ ပြင်းထန်မှုကို အကဲဖြတ်ပြီး အဆင့်သတ်မှတ်ခဲ့သည်။ ဤနမူနာသည် လုပ်ငန်းအတွက် ဖြစ်နိုင်ချေရှိသော အဖြေတစ်ခုအဖြစ် လုပ်ဆောင်သည်။ သင်၏အကဲဖြတ်မှုကို နမူနာနှင့် နှိုင်းယှဉ်ရန် အဆင့်များအတိုင်း လိုက်နာပါ။

## Instructions (ညွှန်ကြားချက်များ)

### Step 1: Access the CVSS Calculator (အဆင့် ၁: CVSS Calculator သို့ ဝင်ရောက်ပါ)

CVSS Calculator

သို့ ဝင်ရောက်ရန် NIST National Vulnerability Database (NVD) ဝဘ်ဆိုဒ်သို့ သင်သွားရောက်ခဲ့ရသည်။

### Step 2: Calculate the CVSS Score (အဆင့် ၂: CVSS အမှတ် တွက်ချက်ပါ)

CVSS အမှတ်ကို တွက်ချက်ရန် CVSS Calculator တွင် တိုင်းတာမှုများကို သင်ထည့်သွင်းခဲ့ရသည်။ တိုင်းတာမှုများနှင့် ၎င်းတို့၏ အကဲဖြတ်ချက်များမှာ အောက်ပါအတိုင်းဖြစ်သည်။

**Base Score Metrics (အခြေခံအမှတ် တိုင်းတာမှုများ)**
| Metric (တိုင်းတာမှု) | Selection (ရွေးချယ်မှု) | CVSS Calculator option (CVSS ဂဏန်းတွက်စက် ရွေးချယ်မှု) |
| ---------------------------- | --------------------- | -------------------------------------------------- |
| Attack Vector (တိုက်ခိုက်မှု လမ်းကြောင်း) | Network (ကွန်ရက်) | (AV:N) |
| Attack Complexity (တိုက်ခိုက်မှု ရှုပ်ထွေးမှု) | Low (နိမ့်) | (AC:L) |
| Privileges Required (လိုအပ်သော အခွင့်အရေးများ) | None (မရှိ) | (PR:N) |
| User Interaction (အသုံးပြုသူ အပြန်အလှန်ဆက်သွယ်မှု) | None (မရှိ) | (UI:N) |
| Scope (အတိုင်းအတာ) | Changed (ပြောင်းလဲ) | (S:C) |
| Confidentiality Impact (လျှို့ဝှက်ရေး သက်ရောက်မှု) | High (မြင့်) | (C:H) |
| Integrity Impact (သမာဓိ သက်ရောက်မှု) | High (မြင့်) | (I:H) |
| Availability Impact (ရရှိနိုင်မှု သက်ရောက်မှု) | High (မြင့်) | (A:H) |

Sam's Scoops ၏ ဖြစ်ရပ်လေ့လာမှုတွင် CVSS အခြေခံတိုင်းတာမှုများသည် ၎င်းတို့၏ firewall တွင် ခွဲခြားသတ်မှတ်ထားသော အားနည်းချက်၏ ပြင်းထန်မှုနှင့် ဖြစ်နိုင်ချေရှိသော သက်ရောက်မှုကို အလေးပေးဖော်ပြသည်။ တိုက်ခိုက်မှု လမ်းကြောင်းအတွက် အဝေးမှ အသုံးချနိုင်ခြေကို ညွှန်ပြသောကြောင့် ကွန်ရက်ရွေးချယ်မှုကို ရွေးချယ်ထားသည်။ တိုက်ခိုက်မှု ရှုပ်ထွေးမှုသည် နိမ့်ကျသည်၊ အကြောင်းမှာ ကျွမ်းကျင်မှုနည်းသော တိုက်ခိုက်သူများပင် အားနည်းချက်ကို အလွယ်တကူ အသုံးချနိုင်သောကြောင့် ပိုမိုအရေးကြီးသော စိုးရိမ်မှုတစ်ခုဖြစ်သည်။ အားနည်းချက်ကို အသုံးချရန် အထူးအခွင့်အရေးများ မလိုအပ်ပါ။ ၎င်းသည် ဖြစ်နိုင်ချေရှိသော တိုက်ခိုက်သူများ၏ အရေအတွက်ကို တိုးချဲ့စေပြီး ဦးစားပေးမှု မြင့်မားစေသည်။ အသုံးချရန်အတွက် အသုံးပြုသူအပြန်အလှန်ဆက်သွယ်မှု မလိုအပ်သောကြောင့် အသုံးပြုသူ အပြန်အလှန်ဆက်သွယ်မှုကိုလည်း မရှိဟု သတ်မှတ်ထားသည်။ ၎င်းသည် အားနည်းချက်ကို အသုံးပြုသူ၏ သတိမထားမိဘဲ အသုံးချနိုင်သောကြောင့် အထူးအန္တရာယ်များစေသည်။ တိုက်ခိုက်သူသည် firewall ချိုးဖောက်မှုမှတစ်ဆင့် ထိခိုက်ခံရသော စနစ်ကို အလုံးစုံ ထိန်းချုပ်နိုင်သောကြောင့် အတိုင်းအတာကို ပြောင်းလဲဟု သတ်မှတ်သင့်ပြီး ပြင်းထန်မှုအမြင့်ဆုံးအဆင့်ကို ညွှန်ပြသည်။ လျှို့ဝှက်ရေး သက်ရောက်မှု၊ သမာဓိ သက်ရောက်မှုနှင့် ရရှိနိုင်မှု သက်ရောက်မှုအားလုံးသည် မြင့်မားသည်၊ အကြောင်းမှာ သုံးခုစလုံးသည် ပြင်းထန်စွာ ထိခိုက်ခံရမည်ဖြစ်သည်။ Sam's Scoops ၏ ချက်ပြုတ်နည်းများ ထုတ်ဖော်ခံရနိုင်သည်၊ ဒေတာကို ပြောင်းလဲခြင်း သို့မဟုတ် ပျက်စီးစေနိုင်သည်၊ စနစ်မှ ပံ့ပိုးပေးသော ဝန်ဆောင်မှုများကို မရရှိနိုင်တော့ခြင်း သို့မဟုတ် အနှောင့်အယှက်ဖြစ်စေနိုင်သည်။

အောက်တွင် ဂဏန်းတွက်စက်တွင် ရွေးချယ်မှု မည်သို့ပုံစံဖြစ်သည်ကို ဖန်သားပြင်ဓာတ်ပုံကို ပြထားသည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/HMoToJUZS4akRtH7-fvthQ_18feade091714c38a4e7306455d33ae1_image.png?expiry=1744416000000&hmac=4ejV9LJCwRnuGJLPMxPS_gDNk8sFCukUJoA7tqHlxN8">

ရွေးချယ်နိုင်သည်မှာ အောက်ပါအတိုင်းဖြစ်သော Temporal နှင့် Environmental Score Metrics များကိုလည်း သင်ဖြည့်သွင်းနိုင်ပါသည်။

**Temporal Score Metrics (ယာယီအမှတ် တိုင်းတာမှုများ)**
| Metric (တိုင်းတာမှု) | Selection (ရွေးချယ်မှု) | CVSS Calculator option (CVSS ဂဏန်းတွက်စက် ရွေးချယ်မှု) |
| ----------------------- | --------------------- | -------------------------------------------------- |
| Exploitability (အသုံးချနိုင်မှု) | High (မြင့်) | (E:H) |
| Remediation Level (ပြုပြင်မှုအဆင့်) | Unavailable (မရနိုင်) | (RL:U) |
| Report Confidence (အစီရင်ခံစာ ယုံကြည်မှု) | Confirmed (အတည်ပြု) | (RC:C) |

Exploitability ကို မြင့်မားသည်ဟု သတ်မှတ်ထားသည်၊ အကြောင်းမှာ အများပြည်သူအတွက် ရရှိနိုင်သော အသုံးပြုရလွယ်ကူသော အသုံးချကုဒ်ကို firewall အားနည်းချက်ကို အသုံးချရန် အသုံးပြုနိုင်သောကြောင့်ဖြစ်သည်။ ထိုကဲ့သို့သော အားနည်းချက်များသည် ပစ်မှတ်ထားခံရပြီး အသုံးချခံရနိုင်ခြေ ပိုများပါသည်။ Remediation Level ကို Unavailable ဟု သတ်မှတ်ထားသည်၊ အကြောင်းမှာ လက်ရှိရရှိနိုင်သော ပြင်ဆင်မှုများ သို့မဟုတ် ရှောင်ကွင်းမှုများ မရှိသောကြောင့် အားနည်းချက်ကို လျှော့ချရန် ပိုမိုခက်ခဲပြီး ထို့ကြောင့် ပိုမိုအရေးကြီးပါသည်။ နောက်ဆုံးတွင် Report Confidence ကို Confirmed ဟု သတ်မှတ်ထားသည်၊ အကြောင်းမှာ အားနည်းချက်ကို လုံခြုံရေးအဖွဲ့ဝင် တစ်ဦးထက်ပိုသောသူများက အတည်ပြုထားသောကြောင့် ၎င်းသည် တရားဝင်စိုးရိမ်မှုတစ်ခုဖြစ်နိုင်ခြေ ပိုများပါသည်။

အောက်တွင် ဂဏန်းတွက်စက်တွင် ရွေးချယ်မှု မည်သို့ပုံစံဖြစ်သည်ကို ဖန်သားပြင်ဓာတ်ပုံကို ပြထားသည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/dPKot26pQyW8MrPQJH_wjw_33edc4b15d40457db8b8eb9f6706f1e1_image.png?expiry=1744416000000&hmac=fIZ7WMY0Vd6AyoEMdqmhBhO-NSIt-o0NtBeZIVz5jWA">

**Environmental Score Metrics (ပတ်ဝန်းကျင်ဆိုင်ရာ အမှတ် တိုင်းတာမှုများ)**
| Metric (တိုင်းတာမှု) | Selection (ရွေးချယ်မှု) | CVSS Calculator option (CVSS ဂဏန်းတွက်စက် ရွေးချယ်မှု) |
| --------------------------------------- | --------------------- | -------------------------------------------------- |
| Modified Attack Vector (ပြုပြင်ထားသော တိုက်ခိုက်မှု လမ်းကြောင်း) | Network (ကွန်ရက်) | (MAV:N) |
| Modified Attack Complexity (ပြုပြင်ထားသော တိုက်ခိုက်မှု ရှုပ်ထွေးမှု) | Low (နိမ့်) | (MAC:L) |
| Modified Privileges Required (ပြုပြင်ထားသော လိုအပ်သော အခွင့်အရေးများ) | None (မရှိ) | (MPR:N) |
| Modified User Interaction (ပြုပြင်ထားသော အသုံးပြုသူ အပြန်အလှန်ဆက်သွယ်မှု) | None (မရှိ) | (MUI:N) |
| Modified Scope (ပြုပြင်ထားသော အတိုင်းအတာ) | Changed (ပြောင်းလဲ) | (MS:C) |
| Modified Confidentiality Impact (ပြုပြင်ထားသော လျှို့ဝှက်ရေး သက်ရောက်မှု) | High (မြင့်) | (MC:H) |
| Modified Integrity Impact (ပြုပြင်ထားသော သမာဓိ သက်ရောက်မှု) | High (မြင့်) | (MI:H) |
| Modified Availability Impact (ပြုပြင်ထားသော ရရှိနိုင်မှု သက်ရောက်မှု) | High (မြင့်) | (MA:H) |
| Modified Confidentiality Requirement (ပြုပြင်ထားသော လျှို့ဝှက်ရေး လိုအပ်ချက်) | High (မြင့်) | (CR:H) |
| Modified Integrity Requirement (ပြုပြင်ထားသော သမာဓိ လိုအပ်ချက်) | High (မြင့်) | (IR:H) |
| Modified Availability Requirement (ပြုပြင်ထားသော ရရှိနိုင်မှု လိုအပ်ချက်) | High (မြင့်) | (AR:H) |

အားနည်းချက်ကို ကွန်ရက်တစ်ခုမှတဆင့် အသုံးချနိုင်သောကြောင့် Modified Attack Vector ကို Network ဟု သတ်မှတ်သင့်သည်။ အားနည်းချက်ကို အသုံးချခြင်းသည် အတော်လေးလွယ်ကူသောကြောင့် Modified Attack Complexity ကို Low ဟု သတ်မှတ်ထားသည်။ အထူးအခွင့်အရေးများ သို့မဟုတ် အသုံးပြုသူအပြန်အလှန်ဆက်သွယ်မှု မလိုအပ်သောကြောင့် ဤတိုင်းတာမှုနှစ်ခုစလုံးကို None ဟု သတ်မှတ်ထားသည်။ အားနည်းချက်သည် firewall ၏ အတိုင်းအတာထက် ကျော်လွန်သော အရင်းအမြစ်များကို ထိခိုက်စေနိုင်သောကြောင့် Modified Scope ကို Changed ဟု သတ်မှတ်ထားသည်။ ဒေတာလျှို့ဝှက်ရေး၊ ဒေတာ၏ ယုံကြည်စိတ်ချရမှုနှင့် တိကျမှုတို့သည် အန္တရာယ်ရှိပြီး ဝန်ဆောင်မှုရရှိနိုင်မှုအပေါ် သက်ရောက်မှုရှိနိုင်ခြေ မြင့်မားသောကြောင့် Modified Confidentiality Integrity Availability အားလုံးကို High ဟု သတ်မှတ်ထားသည်။ နောက်ဆုံး တိုင်းတာမှု သုံးခုဖြစ်သော Modified Confidentiality, Integrity, and Availability Requirements တို့ကို High ဟု သတ်မှတ်ထားသည်၊ အကြောင်းမှာ လျှို့ဝှက်ရေးကို ထိန်းသိမ်းရန်၊ ဒေတာသမာဓိကို ထိန်းသိမ်းရန်နှင့် ဝန်ဆောင်မှုများ၏ ရရှိနိုင်မှုကို ထိန်းသိမ်းရန် လိုအပ်ချက် မြင့်မားသောကြောင့်ဖြစ်သည်။

အောက်တွင် ဂဏန်းတွက်စက်တွင် ရွေးချယ်မှု မည်သို့ပုံစံဖြစ်သည်ကို ဖန်သားပြင်ဓာတ်ပုံကို ပြထားသည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/KjDaz_oXRmuycBTZ6zZhtg_39072584e13d448c9c5b6b22ef5511e1_image.png?expiry=1744416000000&hmac=pPPw4RwMDO6lND6BdbuQsiRiO3AEpY1eMiyWTvACFOE">

အကဲဖြတ်ထားသော တိုင်းတာမှုအားလုံးသည် အောက်ပါအမှတ်ကို ထုတ်ပေးသည်-
| Score (အမှတ်) | Numerical score (ဂဏန်းအမှတ်) |
| --------------------------- | ------------------------- |
| CVSS Base Score (CVSS အခြေခံအမှတ်) | 10.0 |
| Impact Subscore (သက်ရောက်မှု အမှတ်ခွဲ) | 6.0 |
| Exploitability Subscore (အသုံးချနိုင်မှု အမှတ်ခွဲ) | 3.9 |
| CVSS Temporal Score (CVSS ယာယီအမှတ်) | 10.0 |
| CVSS Environmental Score (CVSS ပတ်ဝန်းကျင်ဆိုင်ရာ အမှတ်) | 10.0 |
| Modified Impact Subscore (ပြုပြင်ထားသော သက်ရောက်မှု အမှတ်ခွဲ) | 6.1 |
| Overall CVSS Score (အလုံးစုံ CVSS အမှတ်) | 10.0 |

အောက်တွင် အမှတ်များ၏ ဂရပ်ဖစ်ကိုယ်စားပြုမှုကို ပြထားသည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/L4jwMA_5Rj6KfhmY-cGINQ_dca7ce35ce584bafa6c2118752cc63e1_image.png?expiry=1744416000000&hmac=A1JyVpWKfv2J7lTYwRoqwPSrs4j7wSUW-zz_sOpv94I">

### Step 3: Interpret the score (အဆင့် ၃: အမှတ်ကို အဓိပ္ပာယ်ဖွင့်ပါ)

အလုံးစုံ CVSS အမှတ် 10.0 သည် "အလွန်အန္တရာယ်များ" အမျိုးအစား (9.0-10.0) တွင် ကျရောက်သည်။ ၎င်းသည် အားနည်းချက်သည် သိသာထင်ရှားသော အန္တရာယ်ကို ဖြစ်ပေါ်စေပြီး ၎င်းကို လျှော့ချရန် ချက်ချင်းအာရုံစိုက်ကာ လုပ်ဆောင်ရန် လိုအပ်ကြောင်း ညွှန်ပြသည်။

### Step 4: Mitigation and remediation (အဆင့် ၄: လျှော့ချခြင်းနှင့် ပြုပြင်ခြင်း)

ဤအလွန်အန္တရာယ်များသော အားနည်းချက်ကို လျှော့ချရန်နှင့် ပြုပြင်ရန် အခြေခံ၊ ယာယီနှင့် ပတ်ဝန်းကျင်ဆိုင်ရာ အမှတ်များကို ထည့်သွင်းစဉ်းစား၍ အောက်ပါအဆင့်များကို စဉ်းစားပါ။

- **Apply patches (ပြင်ဆင်မှုများ အသုံးပြုခြင်း):** ထိခိုက်ခံရသော firewall အတွက် မည်သည့်ပြင်ဆင်မှုများ သို့မဟုတ် အပ်ဒိတ်များ ရရှိနိုင်သည်ကို စစ်ဆေးပါ။ အားနည်းချက်ကို ဖယ်ရှားရန် ၎င်းတို့ကို ချက်ချင်းအသုံးပြုပါ။
- **Access control (ဝင်ရောက်ခွင့် ထိန်းချုပ်ခြင်း):** ဝဘ်ဆာဗာသို့ ဝင်ရောက်ခွင့်ကို ခွင့်ပြုထားသော ဝန်ထမ်းများအတွက်သာ ကန့်သတ်ပါ။ ၎င်းသည် ခွင့်ပြုချက်မရှိဘဲ ဝင်ရောက်နိုင်ခြေကို လျှော့ချနိုင်သည်။
- **Network segmentation (ကွန်ရက်ပိုင်းခြားခြင်း):** ဝဘ်ဆာဗာကို အရေးကြီးသော စနစ်များမှ သီးခြားခွဲထုတ်ရန် ကွန်ရက်ပိုင်းခြားခြင်းကို အကောင်အထည်ဖော်ခြင်းဖြင့် ထိခိုက်နိုင်ခြေ၏ အလားအလာရှိသော အတိုင်းအတာကို လျှော့ချပါ။
- **Monitoring (စောင့်ကြည့်ခြင်း):** သံသယဖြစ်ဖွယ် လုပ်ဆောင်ချက်များကို ချက်ချင်းသိရှိနိုင်ရန် ဝဘ်ဆာဗာရှိ စောင့်ကြည့်ခြင်းနှင့် မှတ်တမ်းတင်ခြင်းကို တိုးမြှင့်ပါ။
- **Incident response plan (ဖြစ်ရပ်တုံ့ပြန်ရေးအစီအစဉ်):** ချိုးဖောက်မှုတစ်ခု ဖြစ်ပွားပါက ထိရောက်စွာ တုံ့ပြန်နိုင်ရန် ဖြစ်ရပ်တုံ့ပြန်ရေးအစီအစဉ်ကို တီထွင်ပြီး စမ်းသပ်ပါ။
- **Security awareness training (လုံခြုံရေးဆိုင်ရာ အသိအမြင်လေ့ကျင့်မှု):** လူမှုရေးအင်ဂျင်နီယာတိုက်ခိုက်မှုများကို ကာကွယ်ရန် လုံခြုံရေးဆိုင်ရာ ခြိမ်းခြောက်မှုများကို အသိအမှတ်ပြုပြီး တင်ပြရန် ဝန်ထမ်းများနှင့် အသုံးပြုသူများကို လေ့ကျင့်ပေးပါ။
- **Regular vulnerability scanning (ပုံမှန် အားနည်းချက် စကင်ဖတ်ခြင်း):** လုံခြုံရေးဆိုင်ရာ အားနည်းချက်များကို တက်ကြွစွာ ခွဲခြားသတ်မှတ်ပြီး ပြုပြင်ရန် ပုံမှန် အားနည်းချက် စကင်ဖတ်ခြင်းနှင့် ထိုးဖောက်စမ်းသပ်ခြင်းများကို လုပ်ဆောင်ပါ။

## Conclusion (နိဂုံး)

ဤနမူနာတွင် သင်သည် Sam's Scoops firewall အားနည်းချက်၏ ဖြစ်နိုင်ချေရှိသော CVSS အကဲဖြတ်ချက်ကို ပြန်လည်သုံးသပ်ခဲ့သည်။ ထိုသို့ပြုလုပ်ခြင်းဖြင့် သင်သည် အားနည်းချက်တစ်ခုကို အကဲဖြတ်ခြင်းနှင့် အဆင့်သတ်မှတ်ခြင်းဆိုင်ရာ လက်တွေ့အတွေ့အကြုံကို ရရှိခဲ့သည်။

firewall ရှိ စိတ်ကူးယဉ် လုံခြုံရေးဆိုင်ရာ အားနည်းချက်ကို အကဲဖြတ်ခြင်းသည် CVSS အမှတ် 10.0 ကို ဖြစ်ပေါ်စေခဲ့သည်။ ဤအဆင့်သတ်မှတ်ချက်သည် အားနည်းချက်သည် အဖွဲ့အစည်းနှင့် ၎င်း၏ပိုင်ဆိုင်မှုများအတွက် သိသာထင်ရှားသော အန္တရာယ်ကို ဖြစ်ပေါ်စေကြောင်း ဖော်ပြသည်။ ထိုကဲ့သို့ မြင့်မားသောအမှတ်သည် ဖြစ်နိုင်ချေရှိသော အကျိုးဆက်များကို လျှော့ချရန် ၎င်းကို ချက်ချင်းကိုင်တွယ်ဖြေရှင်းရန် အရေးတကြီး လိုအပ်ကြောင်း အလေးပေးဖော်ပြသည်။ ၎င်းတို့တွင် ခွင့်ပြုချက်မရှိဘဲ ဝင်ရောက်ခြင်း၊ တန်ဖိုးရှိသော ဒေတာကို ခိုးယူခြင်း သို့မဟုတ် ကိုင်တွယ်ဖျက်ဆီးခြင်းနှင့် Sam's Scoops ကို သိသိသာသာ ထိခိုက်စေနိုင်သော အနှောင့်အယှက်များ ပါဝင်နိုင်သည်။

နောက်ဆုံးတွင် CVSS Calculator ကဲ့သို့သော ကိရိယာများကို အသုံးပြု၍ ခြိမ်းခြောက်မှုများကို အကဲဖြတ်ခြင်းသည် တက်ကြွသော ဆိုက်ဘာလုံခြုံရေးဆိုင်ရာ နည်းဗျူဟာအတွက် အလွန်အရေးကြီးပါသည်။ ၎င်းသည် အဖွဲ့အစည်းများအား အထိခိုက်မခံသော သတင်းအချက်အလက်များကို ကာကွယ်ခြင်းနှင့် အရေးကြီးသော စနစ်များ၏ ခံနိုင်ရည်အား သေချာစေရန် အားနည်းချက်များကို ခွဲခြားသတ်မှတ်ပြီး ဦးစားပေးရန် စွမ်းဆောင်ပေးပါသည်။
