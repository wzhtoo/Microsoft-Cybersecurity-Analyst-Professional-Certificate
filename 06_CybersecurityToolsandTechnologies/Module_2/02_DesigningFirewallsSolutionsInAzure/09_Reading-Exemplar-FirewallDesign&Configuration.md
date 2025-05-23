# Exemplar: Firewall design and configuration

[Exemplar: Firewall design and configuration 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/supplement/MRnJ3/exemplar-firewall-design-and-configuration)

# နမူနာ- Firewall ဒီဇိုင်းနှင့် ဖွဲ့စည်းမှု (Exemplar: Firewall Design and Configuration)

**နိဒါန်း (Introduction)**

Azure Firewall သည် Azure cloud တွင် လုပ်ဆောင်နေသော virtual networks များနှင့် workloads များကို ကာကွယ်ရာတွင် အရေးပါသော အခန်းကဏ္ဍမှ ပါဝင်ပါသည်။ လေ့ကျင့်ခန်းတွင် ABC Inc. ၏ သီးခြား လိုအပ်ချက်များနှင့် ကိုက်ညီစေရန်အတွက် Azure Firewall ဖြေရှင်းချက်ကို ဒီဇိုင်းဆွဲရန် သင့်အား တာဝန်ပေးထားပါသည်။ ကုမ္ပဏီသည် ၎င်း၏ virtual networks များနှင့် အင်တာနက်ကြား အသွားအလာကို ထိန်းချုပ်ပေးသည့် ဗဟိုချုပ်ကိုင်ထားသော firewall တစ်ခုကို အကောင်အထည်ဖော်ရန် ကြိုးပမ်းပြီး အရေးကြီးသော ဒေတာကို ကာကွယ်ရန်အတွက် တင်းကျပ်သော စည်းမျဉ်းများကို လိုက်နာကာ လုံခြုံသော ဆက်သွယ်ရေးကို သေချာစေပါသည်။

ဤနမူနာသည် ABC Inc. အတွက် ထိရောက်ပြီး လုံခြုံသော Azure Firewall တည်ဆောက်မှုကို ဒီဇိုင်းဆွဲရန်အတွက် လမ်းညွှန်ချက်အဖြစ် လုပ်ဆောင်ပါသည်။ ကုမ္ပဏီ၏ ထူးခြားသော လိုအပ်ချက်များနှင့် ကိုက်ညီသော ခိုင်မာပြီး သင့်လျော်သော ဖြေရှင်းချက်ကို သေချာစေရန်အတွက် သင်၏ ဒီဇိုင်းအစီအစဉ်ကို နှိုင်းယှဉ်ပြီး ချိန်ညှိရန်အတွက် ရည်ညွှန်းချက်အဖြစ် ၎င်းကို အသုံးပြုပါ။

**အဆင့် ၁- ကွန်ရက် topology ရွေးချယ်မှု (Step 1: Network Topology Selection)**

hub-and-spoke topology သည် virtual networks အားလုံးအတွက် ဗဟိုချုပ်ကိုင်ထားပြီး ထိန်းချုပ်ထားသော အသွားအလာ စီးဆင်းမှု အမှတ်ကို ပံ့ပိုးပေးပါသည်။ ဗဟို hub တစ်ခုဖြင့် ABC Inc. သည် လုံခြုံရေး မူဝါဒများကို အတင်းအကျပ် ချမှတ်နိုင်ပြီး အသွားအလာကို စစ်ဆေးနိုင်ကာ spoke virtual networks အားလုံးအတွက် တသမတ်တည်း firewall စည်းမျဉ်းများကို အသုံးပြုနိုင်ပါသည်။ ၎င်းသည် ကွန်ရက် စီမံခန့်ခွဲမှုကို ရိုးရှင်းစေပြီး တိုက်ခိုက်မှု မျက်နှာပြင်ကို လျှော့ချကာ ကုမ္ပဏီ၏ ကွန်ရက်အတွင်းနှင့် အပြင်သို့ အသွားအလာကို ပိုမို ထိရောက်စွာ စောင့်ကြည့်နိုင်စေပါသည်။

**အဆင့် ၂- Firewall စည်းမျဉ်း ခွဲခြားသတ်မှတ်ခြင်း (Step 2: Firewall Rule Identification)**

ABC Inc. ၏ လိုအပ်ချက်များနှင့် ကိုက်ညီစေရန် အကောင်အထည်ဖော်သင့်သည့် အရေးကြီးသော firewall စည်းမျဉ်းများတွင် အောက်ပါတို့ ပါဝင်သည်-

- **ဝင်လာသော အင်တာနက် စည်းမျဉ်း (Inbound Internet Rule)**: ဝဘ်ကြည့်ရှုခြင်းနှင့် အခြား အင်တာနက်အခြေခံ ဝန်ဆောင်မှုများကို ခွင့်ပြုခြင်းဖြင့် spoke ကွန်ရက်များမှ အင်တာနက်သို့ ထွက်သွားသော အသွားအလာကို ခွင့်ပြုပါ။
- **ထွက်သွားသော အင်တာနက် စည်းမျဉ်း (Outbound Internet Rule)**: spoke ကွန်ရက်များရှိ သီးခြား အရင်းအမြစ်များသို့ အင်တာနက်မှ ဝင်လာသော အသွားအလာကို ခွင့်ပြုပါ (ဥပမာ- အင်တာနက်မှ ဝင်ရောက်ကြည့်ရှုနိုင်သော ဝဘ်ဆာဗာများ)။
- **Inter-spoke စည်းမျဉ်း (Inter-Spoke Rule)**: မတူညီသော spoke virtual networks များကြား အသွားအလာကို ထိန်းချုပ်ပြီး မလိုအပ်သော အသွားအလာကို ပိတ်ဆို့နေစဉ် လိုအပ်သော ဆက်သွယ်ရေးကိုသာ ခွင့်ပြုပါ။
- **အားလုံးကို ငြင်းပယ်သည့် စည်းမျဉ်း (Deny All Rule)**: အထက်ပါ သီးခြား စည်းမျဉ်းများနှင့် မကိုက်ညီသော မည်သည့် အသွားအလာကိုမဆို ပိတ်ဆို့ရန်အတွက် အဆုံးတွင် မူရင်း အားလုံးကို ငြင်းပယ်သည့် စည်းမျဉ်းကို ထည့်ပါ။

**အဆင့် ၃- ကွန်ရက် လိပ်စာ ဘာသာပြန်ခြင်း (NAT) စည်းမျဉ်း အကဲဖြတ်ခြင်း (Step 3: Network Address Translation (NAT) Rule Assessment)**

spoke virtual networks များသည် အင်တာနက်နှင့် ဆက်သွယ်ရန်အတွက် NAT စည်းမျဉ်းများ လိုအပ်ပါသည်။ spoke တစ်ခုစီသည် ထွက်သွားသော အင်တာနက် ဝင်ရောက်ခွင့်အတွက် ၎င်း၏ကိုယ်ပိုင် အများပြည်သူ IP လိပ်စာ လိုအပ်ပါမည်။ Azure Firewall သည် အင်တာနက်နှင့် ဆက်သွယ်သောအခါ spoke ကွန်ရက်များ၏ သီးသန့် IP လိပ်စာများအတွက် NAT ဘာသာပြန်ခြင်းကို စီမံခန့်ခွဲပါမည်။

**အဆင့် ၄- အပလီကေးရှင်း စည်းမျဉ်း အကဲဖြတ်ခြင်း (Step 4: Application Rule Evaluation)**

ABC Inc. သည် virtual networks များမှ ဝင်ရောက်ကြည့်ရှုခြင်းမှ သီးခြား အပလီကေးရှင်းများ သို့မဟုတ် ဝန်ဆောင်မှုများကို ခွင့်ပြုခြင်း သို့မဟုတ် ငြင်းပယ်ခြင်း ပြုလုပ်လိုလျှင် အပလီကေးရှင်း စည်းမျဉ်းများသည် အသုံးဝင်ပါသည်။ ဥပမာအားဖြင့် ကုမ္ပဏီသည် အင်တာနက်မှ သို့မဟုတ် spoke ကွန်ရက်များကြားမှ သီးခြား ဝဘ် အပလီကေးရှင်းများ သို့မဟုတ် APIs များကိုသာ ဝင်ရောက်ကြည့်ရှုရန် ခွင့်ပြုသည့် စည်းမျဉ်းများကို ဖန်တီးနိုင်သည်။

**အဆင့် ၅- မှတ်တမ်းတင်ခြင်းနှင့် စောင့်ကြည့်ခြင်း တည်ဆောက်မှု (Step 5: Logging and Monitoring Setup)**

Azure Firewall အတွက် မှတ်တမ်းတင်ခြင်းကို ဖွင့်ခြင်းသည် လုံခြုံရေး ခွဲခြမ်းစိတ်ဖြာခြင်းနှင့် စာရင်းစစ်ခြင်းအတွက် အရေးကြီးပါသည်။ ရောဂါရှာဖွေ မှတ်တမ်းများကို ဖွင့်ခြင်းဖြင့် ABC Inc. သည် ခွင့်ပြုထားသောနှင့် ငြင်းပယ်ထားသော အသွားအလာအကြောင်း သတင်းအချက်အလက်ကို ဖမ်းယူနိုင်ပြီး ဖြစ်နိုင်ချေရှိသော ခြိမ်းခြောက်မှုများကို ခွဲခြားသတ်မှတ်ကာ ချိတ်ဆက်မှု ပြဿနာများကို ဖြေရှင်းနိုင်သည်။ မှတ်တမ်းတင်ထားသော ဒေတာကို အချိန်နှင့်တပြေးညီ စောင့်ကြည့်ခြင်းနှင့် ခွဲခြမ်းစိတ်ဖြာခြင်းအတွက် Azure Monitor၊ Log Analytics သို့မဟုတ် ပြင်ပ SIEM (လုံခြုံရေး သတင်းအချက်အလက်နှင့် ဖြစ်ရပ် စီမံခန့်ခွဲမှု) ဖြေရှင်းချက်များသို့ ပေးပို့နိုင်ပါသည်။

**အဆင့် ၆- မြင့်မားသော ရရှိနိုင်မှု ရွေးချယ်စရာများ (Step 6: High Availability Options)**

Azure Firewall အတွက် မြင့်မားသော ရရှိနိုင်မှုကို သေချာစေရန်အတွက် ABC Inc. သည် ၎င်းကို ရရှိနိုင်မှု ဇုန်တစ်ခုတွင် ဖြန့်ကျက်နိုင်သည် သို့မဟုတ် Azure ဒေသများစွာတွင် တက်ကြွ-နှေးကွေး ဖွဲ့စည်းပုံကို အသုံးပြုနိုင်သည်။ firewall ကို ဇုန်များ သို့မဟုတ် ဒေသများစွာတွင် ဖြန့်ကျက်ခြင်းဖြင့် ကုမ္ပဏီသည် ဒေတာစင်တာ ပျက်ကွက်မှုများ သို့မဟုတ် ပြတ်တောက်မှုများမှ ကာကွယ်နိုင်ပြီး ပျက်ကွက်မှုများအတွင်း၌ပင် အဆက်မပြတ် ကာကွယ်မှုကို သေချာစေနိုင်သည်။

**အဆင့် ၇- လုံခြုံရေး အကောင်းဆုံး အလေ့အကျင့်များ (Step 7: Security Best Practices)**

Azure Firewall နှင့် ၎င်း၏ ဆက်စပ် အရင်းအမြစ်များကို ထိရောက်စွာ လုံခြုံစေရန်အတွက် အောက်ပါ အကောင်းဆုံး အလေ့အကျင့်များကို အသုံးပြုနိုင်ပါသည်။

- **ကွန်ရက် လုံခြုံရေး အုပ်စုများ (NSGs) (Network Security Groups (NSGs))**: subnet အဆင့်တွင် အသွားအလာကို ထိန်းချုပ်ရန် virtual networks များသို့ NSGs များကို အသုံးပြုပြီး သီးခြား အရင်းအမြစ်များသို့ ဝင်ရောက်ခြင်းနှင့် ဝင်ရောက်ကြည့်ရှုခြင်းကို ထပ်မံ ကန့်သတ်ပါ။
- **သုံးစွဲသူ သတ်မှတ်ထားသော လမ်းကြောင်းများ (UDRs) (User-Defined Routes (UDRs))**: virtual networks များအတွင်း အသွားအလာ စီးဆင်းမှုကို ထိန်းချုပ်ရန်နှင့် စစ်ဆေးခြင်းအတွက် နောက်ခုန်အဖြစ် Azure Firewall သို့ အသွားအလာကို ညွှန်ကြားရန် UDRs များကို အသုံးပြုပါ။
- **ပုံမှန် အပ်ဒိတ်များနှင့် patch များ (Regular Updates and Patches)**: ဖြစ်နိုင်ချေရှိသော အားနည်းချက်များကို လျှော့ချရန်အတွက် နောက်ဆုံးပေါ် လုံခြုံရေး patch များနှင့်အတူ Azure Firewall ကို အပ်ဒိတ်လုပ်ထားပါ။
- **အချိန်မီ (JIT) ဝင်ရောက်ခွင့် (Just-in-Time (JIT) Access)**: လိုအပ်သည့်အခါနှင့် အကန့်အသတ်ရှိသော အချိန်အတွက်သာ အုပ်ချုပ်ရေး ဝင်ရောက်ခွင့်ကို ပေးအပ်ကာ Azure Firewall အတွက် JIT ဝင်ရောက်ခွင့်ကို အကောင်အထည်ဖော်ပါ။
- **Azure Firewall သို့ လုံခြုံသော ဝင်ရောက်ခွင့် (Secure Access to Azure Firewall)**: ယုံကြည်ရသော ကွန်ရက်များနှင့် ခွင့်ပြုထားသော စီမံခန့်ခွဲသူများမှသာ Azure Firewall ၏ စီမံခန့်ခွဲမှု ports (SSH/HTTPS) သို့ ဝင်ရောက်ခွင့်ကို ကန့်သတ်ပါ။

**နိဂုံး (Conclusion)**

ABC Inc. အတွက် ဤ Azure Firewall ဒီဇိုင်းသည် လုံခြုံပြီး ကောင်းမွန်စွာ ဖွဲ့စည်းထားသော ကွန်ရက် ပတ်ဝန်းကျင်ကို သေချာစေပါသည်။ ဗဟိုချုပ်ကိုင်ထားသော firewall သည် အင်တာနက်မှ မလိုအပ်သော ဝင်ရောက်ခွင့်ကို ကန့်သတ်နေစဉ် virtual networks များကြား လုံခြုံသော ဆက်သွယ်ရေးကို လွယ်ကူချောမွေ့စေပါသည်။ မှတ်တမ်းတင်ခြင်းနှင့် စောင့်ကြည့်ခြင်းကို ဖွင့်ခြင်းဖြင့် ကုမ္ပဏီသည် ကွန်ရက် အသွားအလာနှင့် ဖြစ်နိုင်ချေရှိသော လုံခြုံရေး ခြိမ်းခြောက်မှုများကို တွေ့မြင်နိုင်ပါသည်။ မြင့်မားသော ရရှိနိုင်မှု အတိုင်းအတာများကို အသုံးပြုခြင်းနှင့် လုံခြုံရေး အကောင်းဆုံး အလေ့အကျင့်များကို လိုက်နာခြင်းသည် အဆက်မပြတ် ကာကွယ်မှုကို သေချာစေပြီး အလုံးစုံ ကွန်ရက် ခံနိုင်ရည်ကို မြှင့်တင်ပေးပါသည်။
