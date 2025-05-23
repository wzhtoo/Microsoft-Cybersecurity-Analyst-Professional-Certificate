# Azure AD role-based access control

[Azure AD role-based access control 🔗](https://www.coursera.org/learn/microsoft-sc-900-exam-preparation-and-practice/supplement/qqjmr/azure-ad-role-based-access-control)

# Azure AD Role-Based Access Control (Azure AD အခန်းကဏ္ဍ အခြေခံ ဝင်ရောက်ခွင့် ထိန်းချုပ်ခြင်း)

## Introduction (နိဒါန်း)

ယခင်က၊ Azure Active Directory (AD) ရှိ အမျိုးမျိုးသော အခန်းကဏ္ဍများအကြောင်း သင် လေ့လာခဲ့သည်။ Azure AD အတွင်း၊ အခန်းကဏ္ဍများသည် အသုံးပြုသူများအား အမျိုးမျိုးသော လုပ်ငန်းများကို လုပ်ဆောင်ရန် ခွင့်ပြုပါသည်။ ကမ္ဘာလုံးဆိုင်ရာ စီမံခန့်ခွဲသူကဲ့သို့သော အချို့သော အခန်းကဏ္ဍများသည် စီမံခန့်ခွဲခြင်း သို့မဟုတ် သတ်မှတ်ထားသော စက်ပစ္စည်းများ၊ အပလီကေးရှင်းများနှင့် ငွေတောင်းခံခြင်းကို ကြီးကြပ်ရန်အတွက် ဒိုမိန်းအားလုံးတွင် ပုံမှန်ဖြစ်သည်။ အလားတူပင်၊ ဤအခန်းကဏ္ဍအတွက် လုပ်ငန်းများနှင့် ခွင့်ပြုချက်များသည် အလားတူ တင်းပလိတ်ကို လိုက်နာသည်။ Azure AD သည် ဤကမ္ဘာလုံးဆိုင်ရာ အခန်းကဏ္ဍများအတွက် ကြိုတင်သတ်မှတ်ထားသော တင်းပလိတ်တစ်ခုကို ပေးဆောင်ခြင်းဖြင့် စီမံခန့်ခွဲရေး လုပ်ငန်းများတွင် သင့်အား အချိန်ကုန်သက်သာစေရန် ကူညီပေးနိုင်သည်။

ရှင်းလင်းပြတ်သားသော ခွင့်ပြုချက်များနှင့် တာဝန်များ အစုအဝေးကို ဖန်တီးခြင်း၏ အယူအဆသည် Microsoft ၏ ခေတ်မီ အတည်ပြုခြင်း ချဉ်းကပ်မှုအသစ်ကို ညွှန်ပြသည်။ ဤစာဖတ်ခြင်းတွင်၊ အခန်းကဏ္ဍ အခြေခံ ဝင်ရောက်ခွင့် ထိန်းချုပ်ခြင်း (RBAC) ဟုခေါ်သော အခန်းကဏ္ဍများကို အသုံးပြု၍ ဤနည်းလမ်း၏ အုပ်ချုပ်မှုကို သင် လေ့လာပါမည်။

## Custom Roles (စိတ်ကြိုက် အခန်းကဏ္ဍများ)

Azure AD သည် သင့်အဖွဲ့အစည်းအတွင်း ထူးခြားသော လုပ်ဆောင်ချက်များကို လုပ်ဆောင်နိုင်သည့် စိတ်ကြိုက် အခန်းကဏ္ဍများကို ဖန်တီးရန် သင့်အား ခွင့်ပြုပါသည်။ ၎င်းသည် သင့်လိုအပ်ချက်နှင့် ကိုက်ညီသော စိတ်ကြိုက် ပတ်ဝန်းကျင်တစ်ခုကို ဖန်တီးရန် သင့်အား ပိုမိုပြောင်းလွယ်ပြင်လွယ်မှု ပေးပါသည်။ စိတ်ကြိုက် အခန်းကဏ္ဍတစ်ခုကို ဖန်တီးရန်အတွက်၊ ကြိုတင်စုစည်းထားသော စာရင်းမှ ခွင့်ပြုချက်များကို သင် ရွေးချယ်ပါသည်။ ခွင့်ပြုချက်များသည် တည်ဆောက်ထားသော အခန်းကဏ္ဍ၏ စွမ်းရည်များတွင် ထင်ဟပ်ပါသည်။ စိတ်ကြိုက်ပြုလုပ်ခြင်းမှတစ်ဆင့်၊ အခန်းကဏ္ဍကို ဒီဇိုင်းဆွဲသည့်အခါ ဂုဏ်ရည်တစ်ခုကို ရွေးချယ်ခြင်း သို့မဟုတ် ချန်လှပ်ခြင်းဖြင့် သီးခြား အခန်းကဏ္ဍတစ်ခု၏ အတိုင်းအတာကို သင် ချဲ့ထွင်နိုင်သည် သို့မဟုတ် လျှော့ချနိုင်သည်။ စိတ်ကြိုက် အခန်းကဏ္ဍတစ်ခုကို ဖန်တီးပြီးနောက်၊ ၎င်းကို အသုံးပြုသူ သို့မဟုတ် အသုံးပြုသူများ အဖွဲ့သို့ သတ်မှတ်ပေးနိုင်သည်။ အခန်းကဏ္ဍသည် အသုံးပြုသူ၏ စွမ်းရည်များနှင့် ဤခွင့်ပြုချက်များ၏ အတိုင်းအတာကို ဖော်ပြသည်။ အတိုင်းအတာသည် ခွင့်ပြုချက်များ တိုးချဲ့သည့် အရင်းအမြစ်များကို ရည်ညွှန်းသည်။ အပလီကေးရှင်းများကို ဖန်တီး/ဖျက်ခြင်းနှင့် အပ်ဒိတ်လုပ်ခြင်း စွမ်းအားရှိသော စိတ်ကြိုက် အပလီကေးရှင်းများ စီမံခန့်ခွဲသူကို ဖန်တီးခြင်း၏ ကွာခြားချက်ကို စဉ်းစားပါ။ ဖျက်ခြင်းနှင့် အပ်ဒိတ်လုပ်ခြင်း ခွင့်ပြုချက်များ၏ အတိုင်းအတာကို အပလီကေးရှင်းများသို့သာ ကန့်သတ်ထားသည်။ ဤအခန်းကဏ္ဍရှိ အသုံးပြုသူသည် အခြား အသုံးပြုသူများ သို့မဟုတ် ဝန်ဆောင်မှုများကို အပ်ဒိတ်လုပ်ခြင်း သို့မဟုတ် ဖျက်ခြင်း မပြုလုပ်နိုင်ပါ။

ပရီမီယံ လိုင်စင်ဖြင့် အတိုင်းအတာ၏ အသေးစိတ်အချက်အလက်များကို ချဲ့ထွင်နိုင်သည် သို့မဟုတ် ကျုံ့နိုင်သည်။ ကုမ္ပဏီတစ်ဝှမ်းရှိ အရင်းအမြစ်များအားလုံးတွင် မည်သည့် လုပ်ဆောင်ချက်ကိုမဆို လုပ်ဆောင်ရန် စွမ်းအားရှိသော စိတ်ကြိုက် အခန်းကဏ္ဍကို စဉ်းစားပါ။ ဥပမာအားဖြင့်၊ သီးခြား အပလီကေးရှင်း သို့မဟုတ် virtual machine ကဲ့သို့သော အရင်းအမြစ်တစ်ခုအတွက်သာ ခွင့်ပြုချက်များ သက်ရောက်ကြောင်း အပ်ဒိတ် ပြဋ္ဌာန်းချက်ဖြင့် ဤအခန်းကဏ္ဍကို အသုံးပြုသူအသစ်သို့ သတ်မှတ်ပေးနိုင်သည်။ အတိုင်းအတာ၏ ဤစိတ်ကြိုက်ပြင်ဆင်နိုင်သော ပြင်ဆင်ဖွဲ့စည်းမှုသည် ကုမ္ပဏီတစ်ခုသည် ၎င်း၏ ပတ်ဝန်းကျင်တွင် Azure AD ကို အသုံးပြုရန် ရွေးချယ်နိုင်သည့် အကြောင်းရင်းများထဲမှ တစ်ခုဖြစ်သည်။ ပေးထားသော ရည်မှန်းချက်တစ်ခုကို ရရှိရန် လုံလောက်သော ခွင့်ပြုချက်များကို ပေးဆောင်ရန်နှင့် ထို့ထက်ပို၍ မပေးဆောင်ရန် အကောင်းဆုံး အလေ့အကျင့်အဖြစ် သတ်မှတ်သည်။ ၎င်းကို အနည်းဆုံး အထူးအခွင့်အရေး၏ အလေ့အကျင့်ဟုခေါ်ပြီး၊ ပေးထားသော လုပ်ငန်း/တစ်ဦးချင်းစီအတွက် ပေးထားသော ထိတွေ့မှုပမာဏကို ကန့်သတ်ခြင်းဖြင့် အဖွဲ့အစည်းတစ်ခုကို ကာကွယ်ရန် ကူညီပေးသည်။ ၎င်းသည် တစ်စုံတစ်ခု မှားယွင်းသွားပါက နောက်ဆက်တွဲ ပြဿနာများကို ကန့်သတ်သည့် အသားတင် ရလဒ် ရှိပါသည်။

## Roles in Microsoft Services (Microsoft ဝန်ဆောင်မှုများရှိ အခန်းကဏ္ဍများ)

ဤအချက်တွင် Azure AD သည် ဖြန့်ဝေထားသော လုပ်ငန်းပတ်ဝန်းကျင်အတွက် အိုင်ဒင်တီတီအပေါ် အခြေခံသည့် ဝင်ရောက်ခွင့်သည် အကောင်းဆုံး ဖြေရှင်းချက်ဖြစ်သည်ဟု ယူဆသည့် အတွေးအခေါ်ကို အသုံးပြုသည့် cloud-based အိုင်ဒင်တီတီနှင့် ဝင်ရောက်ခွင့် စီမံခန့်ခွဲရေး စနစ်တစ်ခုဖြစ်ကြောင်း ထင်ဟပ်ရန် ထိုက်တန်ပါသည်။ သင်သည် မည်သည့် Microsoft ဝန်ဆောင်မှုများကိုမဆို စာရင်းသွင်းသောအခါ ၎င်းသည် ရောက်လာပါသည်။ သို့သော်၊ အချိန်ကြာလာသည်နှင့်အမျှ၊ ဤဝန်ဆောင်မှုအချို့သည် သီးခြား လုပ်ဆောင်နိုင်စွမ်းကို စီမံခန့်ခွဲရန် ၎င်းတို့၏ အခန်းကဏ္ဍများကို တီထွင်ခဲ့သည်။ အတွင်းပိုင်း အခန်းကဏ္ဍများရှိသော Microsoft ဝန်ဆောင်မှုအချို့နှင့် Azure AD အခန်းကဏ္ဍများကို အားကိုးသည့် ဝန်ဆောင်မှုများကို စစ်ဆေးကြပါစို့။

**အတွင်းပိုင်း အခန်းကဏ္ဍများရှိသော ဝန်ဆောင်မှုများ:**

- **Microsoft Exchange Server:** Exchange အင်္ဂါရပ်များနှင့် မေးလ်ဘောက် စီမံခန့်ခွဲမှုအပေါ် အသေးစိတ် ထိန်းချုပ်မှုကို ဖွင့်ပေးသည့် Exchange Server စီမံခန့်ခွဲသူ၊ မေးလ်ဘောက် စီမံခန့်ခွဲသူနှင့် လက်ခံသူ စီမံခန့်ခွဲသူကဲ့သို့သော ၎င်း၏ အတွင်းပိုင်း အခန်းကဏ္ဍများ ရှိသည်။
- **Microsoft SharePoint Server:** SharePoint ဆိုက်များနှင့် အကြောင်းအရာများကို စီမံခန့်ခွဲခြင်းကို ဖွင့်ပေးသည့် SharePoint Farm စီမံခန့်ခွဲသူ၊ ဆိုက် စုစည်းမှု စီမံခန့်ခွဲသူနှင့် ဆိုက် ပိုင်ရှင်ကဲ့သို့သော အတွင်းပိုင်း အခန်းကဏ္ဍများကို ပေးဆောင်သည်။
- **Microsoft SQL Server:** SQL ဆာဗာ အဖြစ်အပျက်များနှင့် ဒေတာဘေ့စ်များအပေါ် ထိန်းချုပ်မှုကို ဖွင့်ပေးသည့် SQL ဆာဗာ စီမံခန့်ခွဲသူ၊ ဒေတာဘေ့စ် ပိုင်ရှင်နှင့် ဒေတာဘေ့စ် အသုံးပြုသူကဲ့သို့သော အတွင်းပိုင်း အခန်းကဏ္ဍများကို ပေးဆောင်သည်။
- **Microsoft Teams:** Teams နှင့် ၎င်းတို့၏ အဖွဲ့ဝင်ခြင်းကို စီမံခန့်ခွဲခြင်းကို ဖွင့်ပေးသည့် အဖွဲ့ ပိုင်ရှင်၊ အဖွဲ့ အဖွဲ့ဝင်နှင့် ဧည့်သည်ကဲ့သို့သော အတွင်းပိုင်း အခန်းကဏ္ဍများကို ပေးဆောင်သည်။

**Azure AD အခန်းကဏ္ဍများကို အားကိုးသည့် ဝန်ဆောင်မှုများ:**

- **Microsoft 365 (ယခင်က Office 365):** Microsoft 365 အစုအဝေးတွင် အမျိုးမျိုးသော စီမံခန့်ခွဲရေး အင်္ဂါရပ်များသို့ ဝင်ရောက်ခွင့် ပေးသည့် ကမ္ဘာလုံးဆိုင်ရာ စီမံခန့်ခွဲသူ၊ အသုံးပြုသူ စီမံခန့်ခွဲသူနှင့် Exchange စီမံခန့်ခွဲသူကဲ့သို့သော Azure AD အခန်းကဏ္ဍများကို အားကိုးသည်။
- **Azure Portal:** မတူညီသော ဝင်ရောက်ခွင့် အဆင့်များဖြင့် Azure အရင်းအမြစ်များကို စီမံခန့်ခွဲရန် အသုံးပြုသူများကို ဖွင့်ပေးသည့် ပိုင်ရှင်၊ ပံ့ပိုးသူနှင့် ဖတ်ရှုသူကဲ့သို့သော Azure AD အခန်းကဏ္ဍများကို အားကိုးသည်။
- **Microsoft Intune:** မိုဘိုင်းလ် စက်ပစ္စည်းများနှင့် အပလီကေးရှင်း ဖြန့်ကျက်မှုများကို စီမံခန့်ခွဲခြင်းကို ဖွင့်ပေးသည့် Intune စီမံခန့်ခွဲသူကဲ့သို့သော Azure AD အခန်းကဏ္ဍများကို အားကိုးသည်။
- **Microsoft Power BI:** Power BI လုပ်ငန်းခွင်များနှင့် ဒေတာအစုများကို ထိန်းချုပ်ခြင်းကို ဖွင့်ပေးသည့် Power BI စီမံခန့်ခွဲသူကဲ့သို့သော Azure AD အခန်းကဏ္ဍများကို အားကိုးသည်။
- **Microsoft Azure DevOps (ယခင်က Visual Studio Team ဝန်ဆောင်မှုများ):** ပရောဂျက်များနှင့် သိုလှောင်ရုံများကို စီမံခန့်ခွဲခြင်းကို ဖွင့်ပေးသည့် ပရောဂျက် စီမံခန့်ခွဲသူကဲ့သို့သော Azure AD အခန်းကဏ္ဍများကို အားကိုးသည်။

ထို့ကြောင့်၊ ပေးထားသော Azure AD အခန်းကဏ္ဍအတွက် ရရှိနိုင်သည့် လုပ်ဆောင်နိုင်စွမ်းတွင် အောက်ပါအတိုင်း ကွာခြားမှု ရှိသည်-

- **Azure AD-specific roles:** Azure AD ရှိ အခန်းကဏ္ဍများကို ရည်ညွှန်းသည်။ ၎င်းသည် ဤအတိုင်းအတာအတွက် ကန့်သတ်ထားပြီး၊ ဤအခန်းကဏ္ဍများကို အခြား Microsoft 365 ဝန်ဆောင်မှုများကို ဝင်ရောက်ရန် တိုးချဲ့၍မရပါ။ Azure-specific အခန်းကဏ္ဍများ၏ ဥပမာများတွင် အသုံးပြုသူ စီမံခန့်ခွဲသူနှင့် အပလီကေးရှင်းများ စီမံခန့်ခွဲသူတို့ ပါဝင်သည်။
- **Service-specific roles:** ဤအခန်းကဏ္ဍများသည် Microsoft ၏ ပိုမိုကျယ်ပြန့်သော ဝန်ဆောင်မှုအချို့ကို စီမံခန့်ခွဲရန် Azure AD တွင် ဖန်တီးထားသည့် ဝန်ဆောင်မှု-သီးခြား အခန်းကဏ္ဍများနှင့် သက်ဆိုင်သည်။ ဥပမာများတွင် Exchange စီမံခန့်ခွဲသူ၊ Intune စီမံခန့်ခွဲသူ၊ Teams စီမံခန့်ခွဲသူ စသည်တို့ ပါဝင်သည်။ ဤအခန်းကဏ္ဍတစ်ခုစီအတွက် ခွင့်ပြုချက်ရှိသော ဝန်ဆောင်မှုကို စီမံခန့်ခွဲသူရှေ့တွင် အမည်တွင် ထည့်သွင်းထားသည်။
- **Cross-service roles:** မတူညီသော အဖွဲ့အစည်းများအတွက် နေ့စဉ် လုပ်ငန်းများ ရှိပါသည်။ လိုက်နာမှု သို့မဟုတ် လုံခြုံရေးကဲ့သို့သော အသုံးများသော စိုးရိမ်ပူပန်မှုများလည်း ရှိပါသည်။ Cross-service အခန်းကဏ္ဍများသည် မတူညီသော ဝန်ဆောင်မှုများကို ဝင်ရောက်ရန် အခန်းကဏ္ဍ ခွင့်ပြုချက်များ ပေးခြင်းဖြင့် ဤလိုအပ်ချက်ကို ဖြေရှင်းပေးပါသည်။ ထို့ကြောင့်၊ လိုက်နာမှု စီမံခန့်ခွဲသူသည် Teams လဲလှယ်မှုများတွင် လိုက်နာမှုကို စီမံခန့်ခွဲနိုင်သည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/jWAAxPV3RiK8OtcmqZ0vZA_767258b836fb4352999e816606a377e1_C9M2L2_item03_img01.png?expiry=1744502400000&hmac=Euv5wr5cHllNOytzkArP3dE61M7yv7eUj-vkqmf-K20">

အတိုင်းအတာတွင် ခွဲခြားမှုကြောင့် မတူညီသော အခန်းကဏ္ဍများကြားတွင် ခွဲခြားရန် အကျိုးရှိသည်။ Azure AD RBAC သည် Azure AD အရင်းအမြစ်များကို စီမံခန့်ခွဲရန် အထူးဖန်တီးထားသော အခန်းကဏ္ဍများကို ရည်ညွှန်းသည်။ Azure အရင်းအမြစ်များကို ဝင်ရောက်ခွင့် ပေးသည့် အခန်းကဏ္ဍများကို Azure RBAC ဟု လူသိများသည်။ သို့သော်၊ အခန်းကဏ္ဍများကို အသုံးပြု၍ ထိန်းချုပ်သည့် အယူအဆကို RBAC ဟု ရည်ညွှန်းသည်။

## Conclusion (နိဂုံး)

ဤစာဖတ်ခြင်းတွင်၊ အခန်းကဏ္ဍများနှင့် အခန်းကဏ္ဍ အခြေခံ ဝင်ရောက်ခွင့်အကြောင်း သင် လေ့လာခဲ့သည်။ အခန်းကဏ္ဍများ၊ ၎င်းတို့သည် ပိုမိုကြီးမားသော ကွန်ရက်အတွင်း မည်သို့ ကိုက်ညီသည်နှင့် မည်သည့် ဒိုမိန်းနှင့် မည်သည့် အခန်းကဏ္ဍများ ဆက်စပ်နေသည်ကို သင် ထိုးထွင်းသိမြင်ခဲ့သည်။ အနည်းဆုံး အထူးအခွင့်အရေးများ၏ အတွေးအခေါ်ကို လိုက်နာရန် ခွင့်ပြုချက်များ၏ အပိုင်းအခြားကို ကျဉ်းမြောင်းစေရန် သင့်အား ဖွင့်ပေးသည့် အတိုင်းအတာသည် ပရီမီယံ အင်္ဂါရပ်တစ်ခုဖြစ်ကြောင်းကိုလည်း သင် လေ့လာခဲ့သည်။
