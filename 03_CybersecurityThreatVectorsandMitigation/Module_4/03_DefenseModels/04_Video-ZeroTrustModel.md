# Zero Trust Model

[Zero Trust Model 🔗](https://www.coursera.org/learn/cybersecurity-threat-vectors-and-mitigation/lecture/HFpTH/zero-trust-model)

### Zero Trust Model (သုညယုံကြည်မှု ပုံစံ)

#### Introduction (နိဒါန်း)

လုံခြုံရေး ချိုးဖောက်မှုများ မကြာခဏ ဖြစ်ပွားနေသည့် ခေတ်တွင်၊ သင်၏ ဒေတာကို မည်သူ့ကို အမှန်တကယ် ယုံကြည်နိုင်မည်နည်း။ တစ်ချိန်က ကာကွယ်မှုကို အာမခံခဲ့သော ရိုးရာ ပုံစံများသည် ထိရောက်မှု မရှိကြောင်း သက်သေပြခဲ့ပြီးဖြစ်သည်။ ယခုအခါ ယုံကြည်မှု၏ သဘောတရားကို စိန်ခေါ်သည့် ပုံစံတစ်ခုသို့ အပြောင်းအလဲတစ်ခု လိုအပ်လာပြီဖြစ်သည်။ ဤဗီဒီယိုတွင်၊ သင်သည် သုညယုံကြည်မှု ပုံစံ (Zero Trust Model) ကို ရှာဖွေတွေ့ရှိမည်ဖြစ်သည်။ ၎င်းသည် "အတိအလင်း စစ်ဆေးအတည်ပြုခြင်း"၊ "အနည်းဆုံး ခွင့်ပြုချက် ဝင်ရောက်မှု အသုံးပြုခြင်း" နှင့် "ချိုးဖောက်မှုကို ယူဆခြင်း" ဟူသော မူများပေါ်တွင် တည်ဆောက်ထားသော ထုတ်ကုန်များနှင့် ဝန်ဆောင်မှုများထက် ကျော်လွန်သည့် ဒေတာ လုံခြုံရေးအတွက် ချဉ်းကပ်မှုအသစ်တစ်ခုဖြစ်သည်။ ဤပုံစံသည် လုံခြုံရေး အလေ့အကျင့်များတွင် အခြေခံကျသော အသွင်ပြောင်းမှုကို ဖော်ညွှန်းသည်။ ယုံကြည်မှု၏ သဘောတရားကို ပြန်လည်သတ်မှတ်ပေးသော ဤပုံစံအကြောင်း လေ့လာကြည့်ကြပါစို့။

- **ပထမမူ - အတိအလင်း စစ်ဆေးအတည်ပြုခြင်း (Verify Explicitly)**  
  ၎င်းသည် စဉ်ဆက်မပြတ် အထောက်အထားစစ်ဆေးခြင်း (authentication) နှင့် ခွင့်ပြုချက် (authorization) ၏ အရေးပါမှုကို အလေးပေးသည်။ ၎င်းသည် ရရှိနိုင်သော ဒေတာအချက်အားလုံးကို အခြေခံထားသည်။ သင့်ကွန်ရက်ကို ဝင်ရောက်ရန် ကြိုးစားနေသူကို သိရှိရုံဖြင့် မလုံလောက်ပါ။ ၎င်းတို့၏ စက်ပစ္စည်း၊ ၎င်းတို့၏ တည်နေရာ၊ နှင့် အခြားအရာများကိုလည်း သိရှိရန် လိုအပ်သည်။

- **ဒုတိယမူ - အနည်းဆုံး ခွင့်ပြုချက် ဝင်ရောက်မှု (Use Least Privilege Access)**  
  ၎င်းသည် အချိန်နှင့်တပြေးညီ လုံလောက်သော ဝင်ရောက်မှု မူဝါဒများဖြင့် အသုံးပြုသူ၏ ဝင်ရောက်မှုကို ကန့်သတ်ခြင်းကို ဆိုလိုသည်။ ဤမူဝါဒများသည် သတ်မှတ်ထားသော အလုပ်တစ်ခုအတွက် လိုအပ်သည်များကိုသာ ဝင်ရောက်ခွင့်ပြုပြီး၊ ချိုးဖောက်မှု၏ ဖြစ်နိုင်ချေရှိသော သက်ရောက်မှုကို လျှော့ချပေးသည်။

- **နောက်ဆုံးမူ - ချိုးဖောက်မှုကို ယူဆခြင်း (Assume Breach)**  
  ၎င်းသည် သက်ရောက်မှု ဧရိယာကို လျှော့ချခြင်း၊ ဝင်ရောက်မှုကို ခွဲခြမ်းခြင်း (segmenting access)၊ အဆုံးမှအဆုံး စာဝှက်ပြုလုပ်ခြင်း (end-to-end encryption) ကို စစ်ဆေးအတည်ပြုခြင်း၊ နှင့် ခြိမ်းခြောက်မှု သိရှိခြင်းနှင့် ကာကွယ်မှု တိုးတက်စေရန် ခွဲခြမ်းစိတ်ဖြာမှု (analytics) ကို အသုံးပြုခြင်းဖြင့် ခုခံကာကွယ်သည့် အသွင်ကို ယူဆခြင်းပါဝင်သည်။

ခိုင်မာသော သုညယုံကြည်မှု ပုံစံကို သေချာစေရန် လုံခြုံစေရမည့် အဓိက အစိတ်အပိုင်း ခြောက်ခုကို စူးစမ်းကြည့်ကြပါစို့ - အထောက်အထားများ (Identities)၊ စက်ပစ္စည်းများ (Devices)၊ အပ္ပလီကေးရှင်းများ (Applications)၊ ဒေတာ (Data)၊ အခြေခံအဆောက်အအုံ (Infrastructure)၊ နှင့် ကွန်ရက်များ (Networks)။

**[ဗီဒီယို 1:31 မှ စတင်ဖွင့်ပြီး စာသားကို လိုက်နာပါ]**

- **အထောက်အထားများ (Identities)**  
  အရင်းအမြစ်များကို ဝင်ရောက်ရန် ကြိုးစားသူများ၏ အထောက်အထားကို အတည်ပြုရန် ခိုင်မာသော အထောက်အထားစစ်ဆေးခြင်း (strong authentication) သည် မရှိမဖြစ် လိုအပ်သည်။

- **စက်ပစ္စည်းများ (Devices)**  
  IoT စက်ပစ္စည်းများနှင့် အဆုံးသတ် စက်ပစ္စည်းများ (endpoints) အပါအဝင် စက်ပစ္စည်းအားလုံးကို စောင့်ကြည့်ပြီး ကာကွယ်ရန် လိုအပ်ပြီး၊ ဖြစ်နိုင်ချေရှိသော တိုက်ခိုက်မှု မျက်နှာပြင်များကို လျှော့ချရန် လိုအပ်သည်။

- **အပ္ပလီကေးရှင်းများ (Applications)**  
  အပ္ပလီကေးရှင်းများနှင့် API များသည် ကော်ပိုရိတ် စက်ပစ္စည်းများပေါ်ရှိ ခွင့်မပြုထားသော အက်ပ်များကဲ့သို့သော Shadow IT လုပ်ဆောင်ချက်များကို ရှာဖွေရန် လုံခြုံရေး ထိန်းချုပ်မှုများ လိုအပ်သည်။ ပုံမှန်မဟုတ်သော အပြုအမူများကို စောင့်ကြည့်ပြီး လုံခြုံသော ဖွဲ့စည်းပုံ ရွေးချယ်မှုများကို အတည်ပြုပါ။

- **ဒေတာ (Data)**  
  ဒေတာများကို ခွဲခြားသတ်မှတ်ခြင်း (classify)၊ တံဆိပ်တပ်ခြင်း (label)၊ စာဝှက်ပြုလုပ်ခြင်း (encrypt)၊ နှင့် ဤဂုဏ်ရည်များအပေါ် အခြေခံ၍ ဝင်ရောက်မှုကို ကန့်သတ်ခြင်းဖြင့် အဖွဲ့အစည်း၏ ထိန်းချုပ်မှု အပြင်ဘက်တွင်ပင် ဒေတာများ လုံခြုံမှု ရှိနေစေရန် သေချာစေပါ။

- **အခြေခံအဆောက်အအုံ (Infrastructure)**  
  အဆောက်အဦအတွင်း ဆာဗာများမှ ကလောက်အခြေခံ ဗာ့ချွယ် စက်များ (cloud-based virtual machines) အထိ၊ အခြေခံအဆောက်အအုံသည် အရေးကြီးသော ခြိမ်းခြောက်မှု အကြောင်းရင်းတစ်ခု ဖြစ်သည်။ တိုက်ခိုက်မှုများနှင့် ပုံမှန်မဟုတ်မှုများကို သိရှိရန် အကဲဖြတ်မှု (assessment) နှင့် တိုင်းတာမှု (telemetry) ဖြင့် ခိုင်မာသော ကာကွယ်မှုကို ထားရှိပြီး၊ အလိုအလျောက် ကာကွယ်မှု အရေးယူမှုများ လုပ်ဆောင်ပါ။

- **ကွန်ရက်များ (Networks)**  
  ကွန်ရက်ခွဲခြမ်းမှု (network segmentation)၊ အချိန်နှင့်တပြေးညီ ခြိမ်းခြောက်မှု ကာကွယ်မှု (real-time threat protection)၊ နှင့် အဆုံးမှအဆုံး စာဝှက်ပြုလုပ်ခြင်း (end-to-end encryption) တို့သည် ကွန်ရက်အတွင်း တိုက်ခိုက်သူများ၏ ဘေးတိုက်ရွှေ့လျားမှုကို တားဆီးရန် အရေးကြီးသော ထိန်းချုပ်မှုများ ပေးရန် လိုအပ်သည်။

- **အားလုံးသော မဏ္ဍိုင်များနှင့် သက်ဆိုင်သော အစိတ်အပိုင်း**  
  မြင်နိုင်မှု (visibility)၊ အလိုအလျောက်လုပ်ဆောင်မှု (automation)၊ နှင့် ညှိနှိုင်းမှု (orchestration) ၏ မူသည် မတူညီသော နယ်ပယ်များမှ ဒေတာနှင့် သတိပေးချက်များ၏ ဝင်ရောက်မှုကို စီမံခန့်ခွဲရာတွင် အထောက်အကူဖြစ်ပြီး၊ ခြိမ်းခြောက်မှုများကို ပိုမိုကောင်းမွန်စွာ ကာကွယ်ရန်နှင့် ယုံကြည်မှုကို အတည်ပြုရန် ခွင့်ပြုသည်။

#### Zero Trust Model in Practice (သုညယုံကြည်မှု ပုံစံကို လက်တွေ့အသုံးချခြင်း)

ယခု သင်သည် သုညယုံကြည်မှု ပုံစံ၏ အဓိက မူများနှင့် မဏ္ဍိုင်များကို နားလည်ပြီးဖြစ်သည်၊ ၎င်းသည် Sam Scoops ကဲ့သို့သော ကုမ္ပဏီတစ်ခုတွင် မည်သို့ ကွဲပြားမှုတစ်ခု ဖြစ်စေနိုင်သည်ကို စူးစမ်းကြည့်ကြပါစို့။  
ရိုးရာအရ Sam သည် စတိုးဆိုင်အတွင်းရှိ ဝန်ထမ်းများကို ယုံကြည်မည်ဖြစ်ပြီး၊ ၎င်းတို့သည် ၎င်းတို့လိုအပ်သော အရင်းအမြစ်များနှင့် စက်ပစ္စည်းများကိုသာ ဝင်ရောက်အသုံးပြုမည်ဟု ယူဆသည်။ သို့သော် ဝန်ထမ်းတစ်ဦးသည် ထိုယုံကြည်မှုကို ချိုးဖောက်ပါက ဘာဖြစ်မည်နည်း။ ၎င်းတို့ မဝင်ရောက်သင့်သော အရင်းအမြစ်များကို ပြုပြင်မွမ်းမံခြင်းဖြင့် အရင်းအမြစ်များကို ပျက်စီးစေခြင်း သို့မဟုတ် ဒေတာ ချိုးဖောက်မှု ဖြစ်စေခြင်း ဖြစ်နိုင်သည်။ ၎င်းသည် ကွန်ရက်အတွင်းသို့ ဝင်ရောက်ပြီးသည်နှင့် ယုံကြည်မှုကို ယူဆထားသော ရိုးရာ ကွန်ရက် လုံခြုံရေး ပုံစံများနှင့် လက်တွေ့ကမ္ဘာ့ အပြိုင်ဖြစ်သည်။  
သုညယုံကြည်မှု ပုံစံသည် အခြားတစ်ဖက်တွင်၊ "ဘယ်တော့မှ မယုံကြည်ပါ၊ အမြဲတမ်း စစ်ဆေးအတည်ပြုပါ" ဟူသော စကားကို ပြသည့် စဉ်ဆက်မပြတ် အတည်ပြုခြင်း၏ တင်းကျပ်သော ချဉ်းကပ်မှုကို လက်ခံသည်။ Sam Scoops အတွက်၊ သုညယုံကြည်မှု ပုံစံကို လက်ခံခြင်းသည် ဒေတာ လုံခြုံရေးနှင့် ကာကွယ်မှု၏ အဆင့်သစ်တစ်ခုကို ယူဆောင်လာမည်ဖြစ်သည်။  
ဥပမာအားဖြင့်၊ Sam သည် ခွင့်ပြုထားသော ဝန်ထမ်းများသာ အတည်ပြုထားသော စက်ပစ္စည်းများဖြင့် ကွန်ရက်နှင့် အရေးကြီး ဒေတာများကို ဝင်ရောက်နိုင်ကြောင်း သေချာစေရန် အချက်ပေါင်းများစွာ အထောက်အထားစစ်ဆေးခြင်း (multi-factor authentication) ကို အကောင်အထည်ဖော်နိုင်သည်။ ၎င်းသည် ၎င်းတို့၏ ကိုယ်ပိုင် စက်ပစ္စည်းများကို အသုံးပြုသည့် သို့မဟုတ် ရိုးရာ ဖိုင်းဝေါလ် (firewalls) ၏ အကန့်အသတ်များအပြင်ဘက်တွင် အလုပ်လုပ်သော ဝန်ထမ်းများအတွက် အထူးသဖြင့် အရေးကြီးသည်။  
သုညယုံကြည်မှု ချဉ်းကပ်မှုတွင်၊ အရင်းအမြစ်များကို ဝင်ရောက်ရန် ကြိုးစားမှု အားလုံးကို ကွန်ရက်အတွင်းမှ သို့မဟုတ် အပြင်မှ ဖြစ်စေ၊ ဂရုတစိုက် စစ်ဆေးသည်။ "အနည်းဆုံး ခွင့်ပြုချက်" မူကို လိုက်နာပြီး၊ Sam သည် ဝန်ထမ်းများအား ၎င်းတို့၏ အခန်းကဏ္ဍအတွက် လိုအပ်သော သတ်မှတ်ထားသော စနစ်များနှင့် ဒေတာများသို့သာ ဝင်ရောက်ခွင့် ပေးနိုင်သည်။ ဥပမာ၊ ငွေကိုင်သမားသည် အရောင်းစနစ် (point of sale system) ကို ဝင်ရောက်နိုင်သော်လည်း၊ စာရင်းစီမံခန့်ခွဲမှု စနစ် (inventory management system) ကို ဝင်ရောက်ခွင့် မရှိပါ။  
နောက်ဆုံးအနေဖြင့်၊ Sam သည် ဖြစ်နိုင်ချေရှိသော ချိုးဖောက်မှု၏ သက်ရောက်မှုကို လျှော့ချရန် တက်ကြွသော ချဉ်းကပ်မှုကို လက်ခံနိုင်ပြီး၊ စနစ်များနှင့် ဒေတာများကို သီးခြားအပိုင်းများ သို့မဟုတ် ဇုန်များအဖြစ် ပိုင်းခြားနိုင်သည်။ သူမသည် စတိုးဆိုင် နေရာကို အပြည့်အဝ မြင်နိုင်မှုနှင့် စောင့်ကြည့်မှု သေချာစေရန် လုံခြုံရေး ကင်မရာများကဲ့သို့သော ရုပ်ပိုင်းဆိုင်ရာ ဟာ့ဒ်ဝဲများကိုလည်း အသုံးပြုနိုင်သည်။

#### Conclusion (နိဂုံး)

သုညယုံကြည်မှု ပုံစံသည် အလွှာပေါင်းစုံ လုံခြုံရေး မဟာဗျူဟာကို ပေးစွမ်းသည်။ ၎င်းသည် အသုံးပြုသူ၏ အထောက်အထား၊ စက်ပစ္စည်း၏ လုံခြုံရေး အခြေအနေ၊ နှင့် ကွန်ရက် လုံခြုံရေး အနေအထားကို စစ်ဆေးအတည်ပြုသည်။ ငွေပေးငွေယူ၊ အစိတ်အပိုင်းများ၊ နှင့် ဝင်ရောက်မှု တောင်းဆိုမှု အားလုံးကို ဝင်ရောက်ခွင့် မပေးမီ အထောက်အထားစစ်ဆေးခြင်း (authenticated)၊ ခွင့်ပြုခြင်း (authorized)၊ နှင့် စာဝှက်ပြုလုပ်ခြင်း (encrypted) ပြုလုပ်သည်။  
သုညယုံကြည်မှု ပုံစံသည် ဆက်လက်မြင့်တက်လာသော ဆိုက်ဘာ ခြိမ်းခြောက်မှုများကို ရင်ဆိုင်ရာတွင် ကွန်ရက် လုံခြုံရေး ချဉ်းကပ်မှုကို တော်လှန်ပြောင်းလဲပေးသည်။ "အတိအလင်း စစ်ဆေးအတည်ပြုခြင်း"၊ "အနည်းဆုံး ခွင့်ပြုချက် ဝင်ရောက်မှု အသုံးပြုခြင်း"၊ နှင့် "ချိုးဖောက်မှုကို ယူဆခြင်း" ကဲ့သို့သော မူများကို ပေါင်းစပ်ခြင်းဖြင့်၊ Sam Scoops ကဲ့သို့သော အဖွဲ့အစည်းများသည် ဒေတာ လုံခြုံရေးနှင့် ကာကွယ်မှုကို သေချာစေနိုင်သည်။ ဤပုံစံသည် အရေးကြီး သတင်းအချက်အလက်များကို ကာကွယ်ရန် ပြည့်စုံသော မူဘောင်တစ်ခုကို ပံ့ပိုးပေးပြီး၊ ကွန်ရက် လုံခြုံရေး အလေ့အကျင့်များတွင် အခြေခံကျသော ပြောင်းလဲမှုကို ကိုယ်စားပြုသည်။
