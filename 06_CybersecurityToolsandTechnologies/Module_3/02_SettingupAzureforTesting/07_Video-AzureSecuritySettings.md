# Azure security settings

[Azure security settings 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/lecture/arkdw/azure-security-settings)

# Azure security settings (Azure လုံခြုံရေး ဆက်တင်များ)

## Configuring Azure Groups for Penetration Testing (ထိုးဖောက်စမ်းသပ်မှုအတွက် Azure Groups များကို ဖွဲ့စည်းခြင်း)

Azure တွင် ထိုးဖောက်စမ်းသပ်မှုပြုလုပ်ရာတွင် စမ်းသပ်ပတ်ဝန်းကျင်များကို သင့်လျော်စွာ ခွဲခြားထားရန် အရေးကြီးပါသည်။ Role Based Access Control (RBAC) နှင့် ခွင့်ပြုချက်များမှတစ်ဆင့် ဝင်ရောက်ခွင့်ကို ထိန်းချုပ်ရန်လည်း အရေးကြီးပါသည်။ နောက်ဆုံးအနေဖြင့် ထုတ်လုပ်မှုအရင်းအမြစ်များသို့ မတော်တဆ အနှောင့်အယှက်မဖြစ်စေရန် လုံခြုံရေးဆိုင်ရာ အကောင်းဆုံးအလေ့အကျင့်များကို လိုက်နာသင့်ပါသည်။

Azure Portal ကို အသုံးပြု၍ Azure groups များကို ဖန်တီးနိုင်ပြီး global administrator၊ user administrator၊ role administrator နှင့် groups administrator အပါအဝင် အခန်းကဏ္ဍများမှ အဖွဲ့ဝင်များကို ထည့်သွင်းနိုင်သည်။ အဖွဲ့ကို အောင်မြင်စွာ ဖန်တီးပြီးပါက ဝင်ရောက်ခွင့်ကို စီမံခန့်ခွဲရန်နှင့် မည်သည့်ပစ်မှတ်အရင်းအမြစ်တွင်မဆို ထိုးဖောက်စမ်းသပ်မှုကို လုပ်ဆောင်ရန် ၎င်းကို အသုံးပြုနိုင်သည်။

### Creating an Azure Group (Azure Group တစ်ခု ဖန်တီးခြင်း)

1.  ရှာဖွေမှုအကွက်တွင် Group ဟုရိုက်ထည့်ပြီး Services အောက်တွင် Groups ကိုရွေးချယ်ပါ။
2.  Azure group အသစ်တစ်ခုဖန်တီးရန် New group ကိုရွေးချယ်ပါ။
3.  Group အတွက် dropdown menu မှ Security ကိုရွေးချယ်ပါ။
4.  Group name အတွက် Sam's scoops Group ဟုရိုက်ထည့်ပါ။
5.  Group description တစ်ခုပေးပါ၊ learning and development။
6.  အဖွဲ့သို့ ပေးအပ်နိုင်သော Azure AD roles များအတွက် Yes, you can ကိုရွေးချယ်ပါ။
7.  Owners, members နှင့် roles များကို သတ်မှတ်ရန် အောက်သို့ဆွဲချပါ။
8.  Create ကိုရွေးချယ်၍ ထိုးဖောက်စမ်းသပ်မှုအတွက် သင်၏ Azure group ကို ဖန်တီးပါ။

## Configuring Azure Firewall Settings for Penetration Testing (ထိုးဖောက်စမ်းသပ်မှုအတွက် Azure Firewall ဆက်တင်များကို ဖွဲ့စည်းခြင်း)

အလုံးစုံသော ကွန်ရက်လုံခြုံရေးအစီအစဉ်၏ အရေးကြီးသော အစိတ်အပိုင်းတစ်ခုမှာ အပြင်ထွက် ကွန်ရက်ဝင်ရောက်ခွင့်ကို ထိန်းချုပ်ခြင်းဖြစ်သည်။ Azure subnet မှ အပြင်ထွက် ကွန်ရက်ဝင်ရောက်ခွင့်ကို ထိန်းချုပ်ရန် နည်းလမ်းတစ်ခုမှာ Azure Firewall ကိုအသုံးပြုခြင်းဖြစ်သည်။ Azure Firewall ဖြင့် application rules နှင့် network rules များကို ဖွဲ့စည်းနိုင်သည်။ Application rules များသည် သတ်မှတ်ထားသော application တစ်ခုအတွက် မည်သည့် traffic အမျိုးအစားကို ခွင့်ပြုထားသည်ကို သတ်မှတ်ပြီး network rules များသည် source address၊ protocol၊ destination port နှင့် destination address တို့ကို သတ်မှတ်သည်။

### Creating and Configuring Azure Firewall (Azure Firewall ကို ဖန်တီးခြင်းနှင့် ဖွဲ့စည်းခြင်း)

1.  ရှာဖွေမှုအကွက်တွင် firewall ဟုရိုက်ထည့်ပြီး Services အောက်တွင် Firewalls ကိုရွေးချယ်ပါ။
2.  Firewall အသစ်တစ်ခုဖန်တီးရန် Create first ကိုရွေးချယ်ပါ၊ သင်၏ Azure Firewall ဆက်တင်များကို ဖြန့်ကျက်ခြင်းမပြုမီ Azure subscription ရှိကြောင်း အတည်ပြုပါ။
3.  Next select create new ကိုရွေးချယ်ပါ။
4.  Resource group အသစ်တစ်ခုဖန်တီးရန်။ Name အတွက် Sam scoops resource group ဟုရိုက်ထည့်ပြီး OK ကိုရွေးချယ်ပါ။
5.  Next for the firewall name အတွက် Sam scoops Firewall ဟုရိုက်ထည့်ပါ။
6.  Region dropdown menu မှ East US ကိုရွေးချယ်ပါ။
7.  Firewall policy အသစ်တစ်ခုဖန်တီးရန် Add New ကိုရွေးချယ်ပါ။
8.  Policy name အတွက် Sam scoop Policy ဟုရိုက်ထည့်ပါ။
9.  Region အတွက် East US ကိုရွေးချယ်ပါ။
10. အောက်သို့ဆွဲချပြီး OK ကိုရွေးချယ်ပါ။
11. Virtual Network name အကွက်တွင် Sam scoop's virtual network ဟုရိုက်ထည့်ပါ။
12. Address space အတွက် 10.0.0/16 ဟုရိုက်ထည့်ပါ။
13. Subnet address space အတွက် 10.0.0.0/24 ဟုရိုက်ထည့်ပါ။
14. Public IP address တစ်ခုထည့်ရန် Add New ကိုရွေးချယ်ပါ။
15. Name အတွက် Sam Scoops IP ဟုရိုက်ထည့်ပြီး OK ကိုရွေးချယ်ပါ။
16. လိုအပ်သောအချက်အလက်အားလုံးကို ထည့်သွင်းပြီးပါက Review plus Create ကိုရွေးချယ်ပါ။
17. Validation passed message ပေါ်လာပြီးနောက် Create ကိုရွေးချယ်ပါ။
18. သင်၏ ဖြန့်ကျက်မှု ပြီးစီးသောအခါ ဖြန့်ကျက်မှု အောင်မြင်ကြောင်း အတည်ပြုသည့် message တစ်ခု ပေါ်လာမည်ဖြစ်သည်။

## Conclusion (နိဂုံး)

ဤဗီဒီယိုတွင် ထိုးဖောက်စမ်းသပ်မှုအတွက် Azure Firewall ဆက်တင်များနှင့် groups များကို ဖွဲ့စည်းခြင်းသည် ထိန်းချုပ်ထားသော ဝင်ရောက်ခွင့်ကို ခွင့်ပြုခြင်းနှင့် လုံခြုံရေးကို ထိန်းသိမ်းခြင်းကြား မျှတမှုလိုအပ်ကြောင်း သင်လေ့လာခဲ့သည်။ လုံခြုံရေးအကဲဖြတ်မှုများသည် Azure အရင်းအမြစ်များ၏ တည်ငြိမ်မှုကို ထိန်းသိမ်းထားစဉ် အားနည်းချက်များဆိုင်ရာ တန်ဖိုးရှိသော ထိုးထွင်းသိမြင်မှုများကို ပေးဆောင်ကြောင်း သေချာစေရန်အတွက် ၎င်းသည် အရေးပါသော ကဏ္ဍတစ်ခုဖြစ်သည်။ တာဝန်သိသော စမ်းသပ်မှု၊ ကျင့်ဝတ်ဆိုင်ရာ ထည့်သွင်းစဉ်းစားမှုနှင့် သင့်လျော်သော ဖွဲ့စည်းမှုအပေါ် အာရုံစိုက်၍ ထိုးဖောက်စမ်းသပ်မှုကို ချဉ်းကပ်သော အဖွဲ့အစည်းများသည် ၎င်းတို့၏ လုံခြုံရေးအခြေအနေကို ထိရောက်စွာ မြှင့်တင်ရန် ပိုမိုကောင်းမွန်စွာ တပ်ဆင်ထားပါသည်။
