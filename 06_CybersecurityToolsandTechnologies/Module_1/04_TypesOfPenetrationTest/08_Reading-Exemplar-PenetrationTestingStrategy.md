# Exemplar: Penetration testing strategy

[Exemplar: Penetration testing strategy 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/supplement/lEw0I/exemplar-penetration-testing-strategy)

# ထိုးဖောက်စမ်းသပ်ခြင်း မဟာဗျူဟာ နမူနာ (Exemplar: Penetration Testing Strategy)

**နိဒါန်း (Introduction)**

လေ့ကျင့်ခန်းတွင် သင့်လုပ်ငန်းမှာ Sam's Scoops ၏ အခြေအနေလေ့လာမှုနှင့် ကိုက်ညီသော မတူညီသော အဆင့်များနှင့် လုပ်ငန်းများကို လွှမ်းခြုံသည့် ထိုးဖောက်စမ်းသပ်ခြင်း မဟာဗျူဟာကို တည်ဆောက်ရန်ဖြစ်သည်။

ယခု လေ့ကျင့်ခန်း၏ တွေ့ရှိချက်များနှင့် အကြံပြုချက်များအပေါ် အခြေခံ၍ ဖြစ်နိုင်ချေရှိသော ထိုးဖောက်စမ်းသပ်ခြင်း အစီအစဉ်ကို တင်ပြသည့် နမူနာတစ်ခုကို လေ့လာကြည့်ကြပါစို့။

မှတ်သားရန်- သင့်လေ့ကျင့်ခန်း၏ ရလဒ်သည် ကွဲပြားပါက စိတ်မပူပါနှင့်၊ နမူနာသည် သင့်အလုပ်ကို နှိုင်းယှဉ်ရန်အတွက် ရည်ညွှန်းလမ်းညွှန်အဖြစ် လုပ်ဆောင်ပါသည်။

**ထိုးဖောက်စမ်းသပ်ခြင်း မဟာဗျူဟာ (Penetration Testing Strategy)**

**အဆင့် ၁ - စူးစမ်းရှာဖွေခြင်း (Stage 1 - Reconnaissance)**

- လူမှုမီဒီယာ၊ ရှာဖွေရေးအင်ဂျင်များနှင့် ၎င်းတို့၏ ဝဘ်ဆိုက်ကဲ့သို့သော အများပြည်သူ ရရှိနိုင်သော အရင်းအမြစ်များမှ Sam's Scoops နှင့် ၎င်းတို့၏ အခြေခံအဆောက်အအုံအကြောင်း သတင်းအချက်အလက်များကို စုဆောင်းပါ။
- Sam's Scoops၊ ၎င်းတို့၏ ဝန်ထမ်းများနှင့် ဖြစ်နိုင်ချေရှိသော ဆက်သွယ်မှုများအကြောင်း သတင်းအချက်အလက်များကို စုဆောင်းရန်အတွက် ရှာဖွေရေးအင်ဂျင်များနှင့် လူမှုမီဒီယာ ပလက်ဖောင်းများကို အသုံးပြုပါ။
- စနစ် ဗိသုကာ၊ အီးမေးလ် လိပ်စာများနှင့် အခြားတန်ဖိုးရှိသော အသေးစိတ်အချက်အလက်များအကြောင်း ဒေတာ စုဆောင်းရန် Sam's Scoops ဝဘ်ဆိုက်ကို စူးစမ်းပါ။

**အဆင့် ၂ - ရေတွက်ခြင်း (Stage 2 - Enumeration)**

- ပစ်မှတ် VMs များကို စကင်ဖတ်ရန်နှင့် ဖွင့်ထားသော port များ၊ ဝန်ဆောင်မှုများနှင့် ဗားရှင်းများကို ခွဲခြားသိရှိရန် Nmap ကို အသုံးပြုပါ။
- ပစ်မှတ် VMs များရှိ ဖွင့်ထားသော port အားလုံးကို ခွဲခြားသိရှိရန် Nmap ကို အသုံးပြု၍ ပြည့်စုံသော port စကင်ဖတ်ခြင်းကို လုပ်ဆောင်ပါ။
- လုပ်ဆောင်နေသော ဝန်ဆောင်မှုများနှင့် ၎င်းတို့၏ ဆက်စပ် port များကို ဆုံးဖြတ်ရန် စကင်ဖတ်ခြင်း ရလဒ်များကို ခွဲခြမ်းစိတ်ဖြာပါ။
- ပစ်မှတ် VMs များတွင် လုပ်ဆောင်နေသော လည်ပတ်မှုစနစ်ကို ခွဲခြားသိရှိရန် Nmap ၏ လည်ပတ်မှုစနစ် ရှာဖွေခြင်း အင်္ဂါရပ်ကို အသုံးပြုပါ။
- ပစ်မှတ် VMs များတွင် အားနည်းချက် စကင်ဖတ်ခြင်းများကို လုပ်ဆောင်ရန် Nessus ကို အသုံးပြုပါ။
- ၎င်းတို့၏ ဝန်ဆောင်မှုများနှင့် ဗားရှင်းများအပေါ် အခြေခံ၍ သိထားသော အားနည်းချက်များအတွက် ပစ်မှတ် VMs များကို စကင်ဖတ်ရန် Nessus ကို ဖွဲ့စည်းပါ။
- ဖြစ်နိုင်ချေရှိသော အားနည်းချက်များကို ခွဲခြားသိရှိရန်နှင့် ၎င်းတို့၏ ပြင်းထန်မှုအပေါ် အခြေခံ၍ ဦးစားပေးရန် စကင်ဖတ်ခြင်း ရလဒ်များကို ခွဲခြမ်းစိတ်ဖြာပါ။
- ပစ်မှတ် VMs များတွင် လုပ်ဆောင်နေသော ဝန်ဆောင်မှုများအကြောင်း သတင်းအချက်အလက် စုဆောင်းရန် ဘန်နာ ဖမ်းယူခြင်းကို လုပ်ဆောင်ပါ။
- ပစ်မှတ် ဝန်ဆောင်မှုများမှ ဘန်နာများကို ပြန်လည်ရယူရန် netcat သို့မဟုတ် telnet ကဲ့သို့သော ကိရိယာများနှင့်အတူ ဘန်နာ ဖမ်းယူခြင်း နည်းပညာများကို အသုံးပြုပါ။
- ဝန်ဆောင်မှု အမည်များ၊ ဗားရှင်းများနှင့် ရောင်းချသူ သတင်းအချက်အလက်များကို ဆုံးဖြတ်ရန် ရရှိထားသော ဘန်နာများကို ခွဲခြမ်းစိတ်ဖြာပါ။
- ကွန်ရက် အသွားအလာကို ဖမ်းယူပြီး ခွဲခြမ်းစိတ်ဖြာရန် ကွန်ရက် sniffing ကို လုပ်ဆောင်ပါ (ခွင့်ပြုချက်ရှိလျှင်)။
- ပစ်မှတ် VMs များနှင့် အခြား စက်များကြား ကွန်ရက် အသွားအလာကို ဖမ်းယူပြီး ခွဲခြမ်းစိတ်ဖြာရန် Wireshark ကဲ့သို့သော ခွင့်ပြုထားသော ကွန်ရက် sniffing ကိရိယာများကို အသုံးပြုပါ။
- ဖြစ်နိုင်ချေရှိသော လုံခြုံရေး အားနည်းချက်များ သို့မဟုတ် အရေးကြီးသော သတင်းအချက်အလက်များကို ခွဲခြားသိရှိရန် ဖမ်းယူထားသော ကွန်ရက် packets များကို ခွဲခြမ်းစိတ်ဖြာပါ။

**အဆင့် ၃ - အသုံးချခြင်း (Stage 3 - Exploitation)**

- brute-force နည်းပညာများကို အသုံးပြု၍ အားနည်းသော စကားဝှက်များကို အသုံးချရန် ကြိုးစားပါ။
- အမျိုးမျိုးသော စကားဝှက် ပေါင်းစပ်မှုများကို ကြိုးစား၍ ခွဲခြားသိရှိထားသော သုံးစွဲသူ အကောင့်များအပေါ် brute-force တိုက်ခိုက်မှုများကို အသုံးပြုပါ။
- သိထားသော အကောင့် သတင်းအချက်အလက် သို့မဟုတ် အသုံးများသော စကားဝှက် ပုံစံများအပေါ် အခြေခံ၍ တိုက်ခိုက်မှု parameter များကို ချိန်ညှိပါ။
- သင့်လျော်သော နည်းလမ်းများနှင့် နည်းပညာများကို အသုံးပြု၍ eCommerce ပလက်ဖောင်း သို့မဟုတ် SQL Server တွင် သိထားသော အားနည်းချက်များကို အသုံးချပါ။
- အားနည်းချက် စကင်ဖတ်ခြင်းများမှ ရလဒ်များအပေါ် အခြေခံ၍ ပစ်မှတ် စနစ်များတွင် သိထားသော အားနည်းချက်များကို ခွဲခြားသိရှိပြီး အသုံးချပါ။
- ခွဲခြားသိရှိထားသော အားနည်းချက်များကို အသုံးချရန် သင့်လျော်သော နည်းလမ်းများနှင့် နည်းပညာများကို အသုံးပြုပါ။
- သုံးစွဲသူများအား အထောက်အထားများ ထုတ်ဖော်ရန် လှည့်စားရန်အတွက် phishing အီးမေးလ်များ ဖန်တီးခြင်းနှင့် ပေးပို့ခြင်းကဲ့သို့သော လူမှုအင်ဂျင်နီယာ တိုက်ခိုက်မှုများကို အတုယူပါ။
- ယုံကြည်ရသော အဖွဲ့အစည်းများအဖြစ် ဟန်ဆောင်ရန် ယုံကြည်နိုင်လောက်သော phishing အီးမေးလ်များကို ဖန်တီးပါ။
- လူမှုအင်ဂျင်နီယာ နည်းပညာများ၏ ထိရောက်မှုကို အကဲဖြတ်ရန် အတုယူထားသော phishing တိုက်ခိုက်မှုများကို လုပ်ဆောင်ပြီး တုံ့ပြန်မှုများကို စောင့်ကြည့်ပါ။

**အဆင့် ၄ - မြှင့်တင်ခြင်း (Stage 4 - Escalation)**

- VMs များတွင် အခွင့်ထူးများ မြှင့်တင်ရန်အတွက် patch မလုပ်ထားသော ဆော့ဖ်ဝဲ အားနည်းချက်များ သို့မဟုတ် အားနည်းသော ဝင်ရောက်ခွင့် ထိန်းချုပ်မှုများကို အသုံးချပါ။
- ပစ်မှတ် VMs များ၏ လည်ပတ်မှုစနစ်များ၊ အပလီကေးရှင်းများ သို့မဟုတ် ဝန်ဆောင်မှုများတွင် patch မလုပ်ထားသော ဆော့ဖ်ဝဲ အားနည်းချက်များကို ခွဲခြားသိရှိပါ။
- ပိုမိုမြင့်မားသော ဝင်ရောက်ခွင့် အဆင့်များကို ရယူရန် ဤအားနည်းချက်များကို အသုံးချပါ။
- ပိုမိုမြင့်မားသော ဝင်ရောက်ခွင့် အဆင့်များကို ရယူရန်အတွက် firewall များ သို့မဟုတ် ကွန်ရက် စက်များတွင် ဖွဲ့စည်းပုံအမှားများကို အလွဲသုံးစားလုပ်ပါ။
- ပစ်မှတ် VMs များကို ကာကွယ်သည့် Azure Firewall သို့မဟုတ် အခြား ကွန်ရက် စက်များတွင် ဖွဲ့စည်းပုံအမှားများကို ခွဲခြားသိရှိပါ။
- ဝင်ရောက်ခွင့် ထိန်းချုပ်မှုများကို ကျော်လွှားရန် သို့မဟုတ် ပစ်မှတ် စနစ်များသို့ ခွင့်ပြုချက်မရှိဘဲ ဝင်ရောက်ခွင့် ရယူရန် ဤဖွဲ့စည်းပုံအမှားများကို အသုံးချပါ။
- အုပ်ချုပ်သူ သို့မဟုတ် root ဝင်ရောက်ခွင့် ရယူရန်အတွက် အခွင့်ထူး မြှင့်တင်ခြင်း နည်းပညာများကို ကြိုးစားပါ။
- ပစ်မှတ် လည်ပတ်မှုစနစ်များ သို့မဟုတ် အပလီကေးရှင်းများအတွက် သီးခြား သင့်လျော်သော နည်းပညာများကို အသုံးပြုပါ။
- ဖွဲ့စည်းပုံအမှားရှိသော ဖိုင် ခွင့်ပြုချက်များ သို့မဟုတ် အားနည်းသော စနစ် ဝန်ဆောင်မှုများကဲ့သို့သော အသုံးများသော အခွင့်ထူး မြှင့်တင်ခြင်း လမ်းကြောင်းများကို စူးစမ်းပါ။

**စမ်းသပ်ခြင်း အမျိုးအစား အမျိုးအစားခွဲခြားခြင်း (Classification of Testing Type)**

ပေးထားသော အခြေအနေအပေါ် အခြေခံ၍ ပါဝင်သည့် စမ်းသပ်ခြင်း အမျိုးအစားသည် white box စမ်းသပ်ခြင်း ဖြစ်သည်။ ထိုးဖောက်စမ်းသပ်သူအနေဖြင့် စနစ်၏ ဗိသုကာ၊ အစိတ်အပိုင်းများနှင့် အခြေခံအဆောက်အအုံအကြောင်း အသေးစိတ် သတင်းအချက်အလက်များကို ဝင်ရောက်ခွင့်ရှိသည်။ သင့်တွင် အတွင်းလူ သို့မဟုတ် ခွင့်ပြုထားသော သုံးစွဲသူနှင့် ဆင်တူသော မြင့်မားသော အသိပညာ အဆင့်ရှိပြီး၊ ၎င်းသည် သင့်အား ပိုမို နက်ရှိုင်းသော ခွဲခြမ်းစိတ်ဖြာမှုကို လုပ်ဆောင်ရန်နှင့် ဖြစ်နိုင်ချေရှိသော အားနည်းချက်များနှင့် အားနည်းချက်များကို ခွဲခြားသိရှိနိုင်စေပါသည်။
