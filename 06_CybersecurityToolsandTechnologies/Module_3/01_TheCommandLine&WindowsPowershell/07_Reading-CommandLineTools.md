# Command Line tools

[Command Line tools 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/supplement/s7c0B/command-line-tools)

# Command Line ကိရိယာများ

## နိဒ္ဒါန်း (Introduction)

ထိုးဖောက်စမ်းသပ်ခြင်းသည် အဖွဲ့အစည်းများအတွက် မရှိမဖြစ်လိုအပ်သော လုပ်ငန်းစဉ်တစ်ခုဖြစ်ပြီး ၎င်းတို့၏ စနစ်များ၊ ကွန်ရက်များနှင့် အပလီကေးရှင်းများရှိ အားနည်းချက်များကို ခွဲခြားသတ်မှတ်ရန် ကူညီပေးသည်။ သင်ယခင်က လေ့လာခဲ့သည့်အတိုင်း၊ ပစ်မှတ်စနစ်တစ်ခု၏ လုံခြုံရေးအခြေအနေကို အကဲဖြတ်ခြင်းဖြင့် ဤလုပ်ငန်းစဉ်တွင် အမျိုးမျိုးသော command line ကိရိယာများက ကူညီပေးသည်။

ဤစာဖတ်ခြင်းတွင် Network Mapper (Nmap)၊ Metasploit နှင့် Nessus ဟူသော command line ကိရိယာသုံးခုကို သင်လေ့လာပါမည်။ တစ်ခုချင်းစီ၏ အင်္ဂါရပ်များနှင့် စွမ်းရည်များကိုလည်း သင်ရှာဖွေတွေ့ရှိပါမည်။

## Network Mapper (Nmap)

သင်ယခင်က Nmap ကို တက်ကြွသော hosts များ၊ ပွင့်နေသော ports များနှင့် network တစ်ခုရှိ ဝန်ဆောင်မှုများကို ခွဲခြားသတ်မှတ်ရန်အတွက် အသုံးပြုကြောင်း လေ့လာခဲ့ပြီးဖြစ်သည်။ Nmap သည် Transmission Control Protocol (TCP)၊ User Datagram Protocol (UDP)၊ SYN scanning (တစ်ဝက်ဖွင့် scanning ဟုလည်းသိကြသည်) အပါအဝင် scanning နည်းလမ်းများစွာကို ပေးပါသည်။ SYN scanning သည် အပြည့်အဝချိတ်ဆက်မှုမပြုလုပ်ဘဲ ဆက်သွယ်ရေး port တစ်ခု၏ အခြေအနေကို ဆုံးဖြတ်ရန်အတွက် မရိုးသားသော ဟက်ကာများအသုံးပြုသည့် နည်းဗျူဟာတစ်ခုဖြစ်သည်။ ဤနည်းစနစ်များကို ကွန်ရက်တစ်ခု၏ တိုက်ခိုက်မှုမျက်နှာပြင်ကို အကဲဖြတ်ရန်နှင့် တိုက်ခိုက်သူများအတွက် ဖြစ်နိုင်ချေရှိသော ဝင်ပေါက်များကို ရှာဖွေရန်အတွက် အများအားဖြင့်အသုံးပြုသည်။

### စွမ်းရည်များ (Capabilities)

command line အတွင်း Nmap တွင် အောက်ပါစွမ်းရည်များစွာ ပါဝင်သည်-

- `-sP`: တက်ကြွသော hosts များကို ရှာဖွေရန် ping scan လုပ်ဆောင်သည်။
- `-sS`: TCP SYN scan လုပ်ဆောင်ပြီး ပွင့်နေသော ports များကို ရှာဖွေသည်။
- `-sU`: UDP scan လုပ်ဆောင်ပြီး ပွင့်နေသော UDP ports များကို ခွဲခြားသတ်မှတ်သည်။
- `-sV`: Version detection သည် ဝန်ဆောင်မှုဗားရှင်းများကို ဆုံးဖြတ်သည်။
- `-A`: Aggressive scan mode သည် အမျိုးမျိုးသော scan အမျိုးအစားများကို ပေါင်းစပ်သည်။

### အင်္ဂါရပ်များ (Features)

open-source ကိရိယာတစ်ခုအနေဖြင့် Nmap သည် ကွန်ရက်စူးစမ်းရှာဖွေခြင်းတွင် ၎င်း၏အရေးပါမှုကို ထိန်းသိမ်းထားပြီး ဖြစ်နိုင်ချေရှိသော လုံခြုံရေးအန္တရာယ်များကို အလံပြရာတွင် မရှိမဖြစ်လိုအပ်သော ပိုင်ဆိုင်မှုတစ်ခုအဖြစ် ရပ်တည်သည်။ မရိုးသားသော လုပ်ဆောင်သူများက အသုံးချနိုင်သော အားနည်းချက်များနှင့် ဖြစ်နိုင်ချေရှိသော ဝင်ပေါက်များကို ရှာဖွေရာတွင် ကျွမ်းကျင်ပြီး Nmap သည် ပွင့်နေသော ports များကို အခြေခံထားသော ဆော့ဖ်ဝဲလ်ကို ဖော်ထုတ်သည့် version detection ကို လုပ်ဆောင်နိုင်စွမ်းတွင် ထူးချွန်သည်။

Nmap သည် လုံခြုံရေးဆိုင်ရာ အင်္ဂါရပ်များကို ရှာဖွေဖော်ထုတ်ရန်နှင့် အကဲဖြတ်ရန် အတိအကျ ဖန်တီးထားသော ကွန်ရက်များကို စကင်ဖတ်ရန်အတွက် ဘက်စုံသုံးနိုင်သော ကိရိယာတစ်ခုအဖြစ် ရပ်တည်သည်။ ၎င်း၏ command-line interface သည် ကျယ်ပြန့်သော scanning နည်းလမ်းများကို တင်ပြပြီး သုံးစွဲသူများအား ကွန်ရက်များတစ်လျှောက် တက်ကြွသော hosts များ၊ ဝင်ရောက်နိုင်သော ports များနှင့် ဝန်ဆောင်မှုများကို တိကျစွာ ဖော်ထုတ်နိုင်စေသည်။ Nmap သည် TCP၊ UDP နှင့် SYN scans များကို ကျွမ်းကျင်စွာ ထောက်ပံ့ပေးပြီး စမ်းသပ်သူများအား ပစ်မှတ်၏ အားနည်းချက်ရှုခင်းကို အကဲဖြတ်ရာတွင် အားဖြည့်ပေးသည်။ ၎င်း၏ ခိုင်မာသော aggressive scan mode သည် အမျိုးမျိုးသော scan နည်းစနစ်များကို ပေါင်းစပ်ပြီး ဘက်စုံရလဒ်များကို မြှင့်တင်ပေးသည်။

## Metasploit

နောက်တစ်ခုမှာ ထိုးဖောက်စမ်းသပ်ခြင်းအတွက် အသုံးပြုသော အခြား command-line ကိရိယာတစ်ခုဖြစ်သည့် Metasploit ဖြစ်သည်။ Metasploit သည် အဝေးမှပစ်မှတ်တစ်ခုကို အသုံးပြုရန်အတွက် exploit code ၏ ဖွံ့ဖြိုးတိုးတက်မှု၊ စမ်းသပ်မှုနှင့် လုပ်ဆောင်မှုတွင် ထိုးဖောက်စမ်းသပ်သူများကို ကူညီပေးသည့် အစွမ်းထက်သော ဘောင်တစ်ခုဖြစ်ကြောင်း သင်ယခင်က လေ့လာခဲ့ပြီးဖြစ်သည်။ ၎င်းတွင် စနစ်များကို အားနည်းစေရန်၊ စနစ်များသို့ ဝင်ရောက်ခွင့်ရရှိရန်နှင့် အချက်အလက်များကို စုဆောင်းရန်အတွက် အသုံးပြုနိုင်သော payloads နှင့် auxiliary modules များ ပါဝင်သည်။ Metasploit ကို post-exploitation လုပ်ငန်းများအတွက်လည်း အသုံးပြုနိုင်သည်။

### စွမ်းရည်များ (Capabilities)

command line အတွင်း Metasploit ၏ စွမ်းရည်များတွင်-

- `use <module>`: exploit သို့မဟုတ် module တစ်ခုကို ရွေးချယ်ပါ။
- `set <option> <value>`: ရွေးချယ်ထားသော module အတွက် ရွေးချယ်စရာများစွာကို သတ်မှတ်ပါ။
- `exploit` သို့မဟုတ် `run`: ရွေးချယ်ထားသော exploit သို့မဟုတ် module ကို လုပ်ဆောင်ပါ။
- `sessions`: တက်ကြွသော sessions များနှင့် ချိတ်ဆက်မှုများအားလုံးကို စာရင်းပြုစုပါ။
- `Post module`: အထူးအခွင့်အရေး တိုးမြှင့်ခြင်း သို့မဟုတ် ဒေတာစုဆောင်းခြင်းကဲ့သို့သော post-exploitation လုပ်ငန်းများအတွက် အသုံးပြုသည်။

### အင်္ဂါရပ်များ (Features)

Metasploit သည် ထိုးဖောက်စမ်းသပ်ခြင်းနှင့် အားနည်းချက်များကို အသုံးချခြင်း နှစ်မျိုးစလုံးအတွက် ရည်ရွယ်ထားသော အစွမ်းထက်သော ဘောင်တစ်ခုအဖြစ် ရပ်တည်သည်။ ၎င်း၏ command-line interface မှတဆင့် exploit code ၏ ဖွံ့ဖြိုးတိုးတက်မှု၊ အကဲဖြတ်မှုနှင့် လုပ်ဆောင်မှုတို့ကို ဖြည့်ဆည်းပေးသော လုပ်ဆောင်ချက်များစွာကို ပေးပါသည်။ ဘောင်တွင် exploits၊ payloads နှင့် auxiliary modules များပါဝင်သော ကျယ်ပြန့်သော သိုလှောင်ရာတစ်ခုရှိပြီး စမ်းသပ်သူများအား စနစ်များကို အားနည်းစေရန်နှင့် ဝင်ရောက်ခွင့်ရရှိရန် နည်းလမ်းများကို တပ်ဆင်ပေးထားသည်။

Metasploit အတွင်းရှိ `use` command သည် သီးခြား exploits သို့မဟုတ် modules များကို ရွေးချယ်ပြီး `set` command သည် ဖွဲ့စည်းမှုဆိုင်ရာ ချိန်ညှိမှုများကို လွယ်ကူချောမွေ့စေသည်။ ပစ်မှတ်စနစ်များအပေါ် exploits သို့မဟုတ် modules များကို စတင်ခြင်းသည် `exploit` သို့မဟုတ် `run` command ဖြင့် လွယ်ကူချောမွေ့စေသည်။ Metasploit ၏ post-exploitation စွမ်းရည်များ ထင်ရှားလာပြီး အထူးအခွင့်အရေးများ တိုးမြှင့်ခြင်းနှင့် ဒေတာစုဆောင်းခြင်းကဲ့သို့သော လုပ်ငန်းများကို လွယ်ကူချောမွေ့စေသည်။ ဘောင်၏ လိုက်လျောညီထွေရှိမှုနှင့် ကျယ်ပြန့်သော exploits သိုလှောင်ရာသည် ၎င်းအား ကျင့်ဝတ်ဆိုင်ရာ ဟက်ကာများကြားတွင် နှစ်သက်သော ရွေးချယ်မှုတစ်ခုအဖြစ် ရပ်တည်စေပြီး ၎င်းတို့အား စနစ်များကို ကျွမ်းကျင်စွာ အကဲဖြတ်ကာ ကာကွယ်ရန် ခွင့်ပြုသည်။

## Nessus

နောက်ဆုံးအနေဖြင့် Nessus ဖြစ်ပြီး ကွန်ရက်များ၊ စနစ်များနှင့် အပလီကေးရှင်းများအတွင်း လုံခြုံရေးဆိုင်ရာ ပြဿနာများကို ခွဲခြားသတ်မှတ်ရန်အတွက် ကူးသန်းရောင်းဝယ်ရေးဆိုင်ရာ အားနည်းချက်များကို စကင်ဖတ်ရန်အတွက် အသုံးပြုကြောင်း သင်ယခင်က လေ့လာခဲ့ပြီးဖြစ်သည်။ Nessus ကို အများအားဖြင့် web interface မှတဆင့် စီမံခန့်ခွဲသော်လည်း Nessus command ကို အသုံးပြု၍ CLI မှတဆင့်လည်း ထိန်းချုပ်နိုင်သည်။ Nessus သည် ကျယ်ပြန့်သော အားနည်းချက်စစ်ဆေးမှုများကို ပေးစွမ်းပြီး တိုက်ခိုက်သူများက အသုံးချနိုင်သော ဖြစ်နိုင်ချေရှိသော အားနည်းချက်များကို အစီရင်ခံသည်။

### စွမ်းရည်များ (Capabilities)

Nessus တွင် အသုံးပြုနိုင်သော အခြား command များစွာရှိသည်၊ ၎င်းတို့တွင်-

- `nessuscli scan list`: ရှိပြီးသား scan ဖွဲ့စည်းမှုများကို စာရင်းပြုစုပါ။
- `nessuscli scan new`: scan ဖွဲ့စည်းမှုအသစ်တစ်ခု ဖန်တီးပါ။
- `nessuscli scan launch`: သီးခြားဖွဲ့စည်းမှုကို အသုံးပြု၍ scan တစ်ခုကို စတင်ပါ။
- `nessuscli report list`: ရရှိနိုင်သော scan အစီရင်ခံစာအားလုံးကို စာရင်းပြုစုပါ။
- `nessuscli report export`: scan အစီရင်ခံစာကို အမျိုးမျိုးသော ဖော်မတ်များဖြင့် ထုတ်ယူပါ။

### အင်္ဂါရပ်များ (Features)

Nessus သည် လုံခြုံရေးဆိုင်ရာ ပြဿနာများကို ခွဲခြားသတ်မှတ်ရန်အတွက် အစွမ်းထက်သော စွမ်းရည်များ တပ်ဆင်ထားသော ပြည့်စုံသော ကူးသန်းရောင်းဝယ်ရေးဆိုင်ရာ အားနည်းချက် scanner တစ်ခုဖြစ်သည်။ ၎င်း၏ CLI သည် web-based interface ကို ဖြည့်စွက်ပြီး သုံးစွဲသူများအား scans များကို စီမံခန့်ခွဲကာ ထိရောက်သောနည်းလမ်းဖြင့် အစီရင်ခံရန် ခွင့်ပြုသည်။

Nessus သည် ကွန်ရက်များ၊ စနစ်များနှင့် အပလီကေးရှင်းများကို စေ့စေ့စပ်စပ် အကဲဖြတ်နိုင်စေမည့် ကြိုတင်တည်ဆောက်ထားသော အားနည်းချက်စစ်ဆေးမှုများစွာကို ပေးပါသည်။ ကိရိယာ၏ `scan list` နှင့် `scan new` command များသည် scan ဖွဲ့စည်းမှု ဖန်တီးခြင်းနှင့် စီမံခန့်ခွဲခြင်းကို လွယ်ကူချောမွေ့စေသည်။ `scan launch` command သည် scans များကို စတင်ပြီး `report list` နှင့် `report export` command များသည် scan အစီရင်ခံစာများကို ခွဲခြမ်းစိတ်ဖြာခြင်းနှင့် ထုတ်ယူခြင်းတွင် ကူညီပေးသည်။ မတူညီသော ပတ်ဝန်းကျင်များတစ်လျှောက် အားနည်းချက်များကို ရှာဖွေနိုင်စွမ်းနှင့် အမျိုးမျိုးသော အစီရင်ခံစာဖော်မတ်များကို ပံ့ပိုးပေးခြင်းတို့ကြောင့် Nessus သည် လုံခြုံရေးဆိုင်ရာ စိုးရိမ်ပူပန်မှုများကို ကြိုတင်ကိုင်တွယ်ဖြေရှင်းလိုသော အဖွဲ့အစည်းများအတွက် တန်ဖိုးရှိသော ကိရိယာတစ်ခုဖြစ်သည်။

## နိဂုံး (Conclusion)

Nmap၊ Metasploit နှင့် Nessus တို့သည် ထိုးဖောက်စမ်းသပ်ခြင်းနယ်ပယ်တွင် သီးခြားရည်ရွယ်ချက်များအတွက် အသုံးပြုသော အစွမ်းထက်သော command-line ကိရိယာများဖြစ်သည်။ Nmap သည် ကွန်ရက်စူးစမ်းရှာဖွေခြင်းတွင် ထူးချွန်ပြီး Metasploit သည် အားနည်းချက်များကို အသုံးချခြင်းအပေါ် အာရုံစိုက်ကာ Nessus သည် ပြည့်စုံသော အားနည်းချက်အကဲဖြတ်မှုစွမ်းရည်များကို ပေးဆောင်သည်။ တာဝန်သိစွာနှင့် ကျင့်ဝတ်နှင့်အညီ အသုံးပြုသောအခါ ဤကိရိယာများသည် စနစ်များနှင့် ကွန်ရက်များ၏ လုံခြုံရေးအခြေအနေကို တိုးတက်စေရန်အတွက် များစွာအထောက်အကူပြုသည်။

ဤကိရိယာများသည် ထိုးဖောက်စမ်းသပ်ခြင်းတွင် တန်ဖိုးရှိသော်လည်း ၎င်းတို့၏အသုံးပြုမှုသည် အမြဲတမ်း ကျင့်ဝတ်ဆိုင်ရာ စံနှုန်းများနှင့် ဥပဒေများကို လိုက်နာသင့်ကြောင်း မှတ်သားထားရန် အရေးကြီးပါသည်။ ခွင့်ပြုချက်မရှိဘဲ စကင်ဖတ်ခြင်းနှင့် စမ်းသပ်ခြင်းသည် တရားဥပဒေအရ အကျိုးဆက်များကို ဖြစ်ပေါ်စေနိုင်သည်။ ထို့အပြင် ထိုးဖောက်စမ်းသပ်ခြင်းကို အမြဲတမ်း သင့်လျော်သော ခွင့်ပြုချက်နှင့် စမ်းသပ်ခံရမည့် စနစ်များကို နားလည်မှုဖြင့် လုပ်ဆောင်သင့်သည်။
