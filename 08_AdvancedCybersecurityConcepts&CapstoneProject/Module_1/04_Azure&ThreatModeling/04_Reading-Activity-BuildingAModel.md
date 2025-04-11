# Activity: Building a model

[Activity: Building a model 🔗](https://www.coursera.org/learn/advanced-cybersecurity-concepts-and-capstone-project/supplement/5JcWl/activity-building-a-model)

# Activity: Building a model (လှုပ်ရှားမှု: ပုံစံတစ်ခု တည်ဆောက်ခြင်း)

## Introduction (နိဒါန်း)

ဤလှုပ်ရှားမှုတွင် Microsoft Threat Modeling Tool ကို မည်သို့အသုံးပြုရမည်ကို သင်လေ့လာရမည်ဖြစ်သည်။ ဤကိရိယာသည် ဆော့ဖ်ဝဲလ်ပုံများ ဖန်တီးခြင်း၊ ခြိမ်းခြောက်မှုများကို ခွဲခြမ်းစိတ်ဖြာခြင်းနှင့် လျှော့ချရေးနည်းဗျူဟာများကို စီမံခန့်ခွဲခြင်းတို့တွင် ကူညီရန် ဒီဇိုင်းထုတ်ထားသည်။ ကိရိယာ၏ မျက်နှာပြင်ကို မည်သို့သွားလာရမည်နှင့် အပြန်အလှန်ဆက်သွယ်ရမည်ကို နားလည်ရန် ပေးထားသော ဖန်သားပြင်ဓာတ်ပုံများကို ကိုးကား၍ အဆင့်များစွာကို သင်လိုက်နာရမည်ဖြစ်သည်။

## Prerequisites (လိုအပ်ချက်များ)

ဤလှုပ်ရှားမှုကို မကြိုးစားမီ သင့်ကွန်ပျူတာတွင် Microsoft Threat Modeling Tool ကို ထည့်သွင်းထားပြီး နမူနာခြိမ်းခြောက်မှုပုံစံကို ဒေါင်းလုဒ်လုပ်ထားကြောင်း သေချာပါစေ။

## MacOS users (MacOS အသုံးပြုသူများ)

Microsoft Threat Modeling Tool သည် Windows လည်ပတ်မှုစနစ်များအတွက် သီးသန့်ဒီဇိုင်းထုတ်ထားကြောင်း အသိပေးအပ်ပါသည်။ MacOS အသုံးပြုသူအနေဖြင့် ဤကိရိယာကို အသုံးပြုရန် Windows 11 လည်ပတ်နေသော Azure Virtual Machine (VM) တစ်ခုကို တပ်ဆင်ရပါမည်။ တပ်ဆင်ရန် မည်သည့်ဒေသကိုမဆို ရွေးချယ်နိုင်ပြီး သင်၏နှစ်သက်မှုအပေါ်အခြေခံ၍ ရှိပြီးသား Resource Group တွင် VM ကို ထားရန် သို့မဟုတ် အသစ်တစ်ခုကို ဖန်တီးရန် ရွေးချယ်နိုင်သည်။ သင်၏ MacOS ပတ်ဝန်းကျင်တွင် Microsoft Threat Modeling Tool ကို ချောမွေ့စွာအသုံးပြုရန် ဤတပ်ဆင်မှုသည် လိုအပ်ကြောင်း သတိပြုပါ။ Threat Modeling Tool ကို အသုံးပြုပြီးသည်နှင့် ငွေတောင်းခံခြင်းကို ချက်ချင်းရပ်တန့်စေရန်နှင့် မလိုအပ်သော ကုန်ကျစရိတ်များ မဖြစ်ပေါ်စေရန် VM ကို ရပ်တန့်ပြီး ဖျက်ရန် သတိရပါ။

## Microsoft Threat Modeling Tool download (Microsoft Threat Modeling Tool ဒေါင်းလုဒ်)

Microsoft Threat Modeling Tool ကို ဒေါင်းလုဒ်လုပ်ရန် T
hreat Modeling Tool

သို့ သွားပါ။

Windows တွင် နမူနာဖိုင်ကို ဒေါင်းလုဒ်လုပ်ရန် အောက်ပါလင့်ခ်ကို ညာကလစ်နှိပ်ပြီး "Save link as" ရွေးချယ်မှုကို ရွေးချယ်ပါ။ Mac တွင် နမူနာဖိုင်ကို ဒေါင်းလုဒ်လုပ်ရန် အောက်ပါလင့်ခ်ကို Control-click နှိပ်ပြီး "Download Linked File" ရွေးချယ်မှုကို ရွေးချယ်ပါ။

Sample_Threat Model_https
TM7 File

## Steps (အဆင့်များ)

Microsoft Threat Modeling Tool ကို အသုံးပြုပါ။
Open a Model ကို ရွေးချယ်ပြီး သင်ယခင်ဒေါင်းလုဒ်လုပ်ထားသော Sample_Threat Model_https.tm7 ဖိုင်သို့ သွားပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/TUX9YixgRtyLwQdsgVfLeA_fbf5e3eed1504e7c9efc66da680c8fe1_image.png?expiry=1744416000000&hmac=v1D77sK0cj1rHdWKkZFpCqyeQtUjbD6A5oJlugG_ags">

မျက်နှာပြင်၏ ညာဘက်တွင် Stencils panel တစ်ခုရှိသည်ကို သတိပြုပါ။ Stencils များကို ပုံတွင် အစိတ်အပိုင်းများထည့်ရန် အသုံးပြုပါသည်။ ပုံကိုနားလည်ကြောင်းသေချာစေရန် မော်ဒယ်တွင်အသုံးပြုထားသော အစိတ်အပိုင်းများကို လေ့လာပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/ys9-WiNzT4iU2slZXAsHQA_2a293904620a494bb1e3807577414ce1_image.png?expiry=1744416000000&hmac=8Gqanap4_oB1_Nm_UpNRWYcXLZjlDIlba1ydfTRupcE">

မျက်နှာပြင်၏ ဘယ်ဘက်အပေါ်ထောင့်ရှိ toolbar ရှိ Switch to Analysis View ခလုတ် (မှန်ဘီလူးပုံပါသော စာမျက်နှာ) ကို ရွေးချယ်ခြင်းဖြင့် Analysis View သို့ ပြောင်းပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/BuJD1B5dRd2nz0Zh0T3Qcg_ab6e3607221b4e9db8e1b0f8be8d25e1_image.png?expiry=1744416000000&hmac=p1izICj2IJQhW_8sNJtCK_mFG18XQ2VBZe9h_AMhkzE">

Threat List panel သည် ပုံအောက်ရှိ စာရင်းတွင် ဖြစ်နိုင်ချေရှိသော ခြိမ်းခြောက်မှုများကို ယခုပြသနေသည်ကို သတိပြုပါ။ သီးခြားခြိမ်းခြောက်မှုအကြောင်း နောက်ထပ်အချက်အလက်များပါရှိသော Threat Properties panel ကိုကြည့်ရှုရန် စာရင်းရှိ ခြိမ်းခြောက်မှုတစ်ခုကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/8iSFkCHNQPux7zmnPXhFyQ_d1478ab1812b4e87a9204f7b164ac3e1_image.png?expiry=1744416000000&hmac=i_i3ocs82ceHrv6go5WUL-KDp8vEnFK3lV-qlMhZVpA">

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/XCNl70iJRAWkMUdYKNAN5A_d7a4f7f2daeb47eb8fcdaae05041f7e1_image.png?expiry=1744416000000&hmac=r4-xADbV1VQWwGXfqo94rh8fNnzWGcovnmSz8TfhX_o">

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/kexNzbfXTdGKKybp-GDCLg_b2a449cef91f467eaafc679f3d7d99e1_image.png?expiry=1744416000000&hmac=42WT1rJbDrpZMHMIKo3xyATBNcvR0pALBTY1z65kJsA">

အောက်ပါခြိမ်းခြောက်မှု ဂုဏ်သတ္တိများကို အာရုံစိုက်ပါ။

- Title, Category, and Description fields: ဤအကွက်များတွင် ခြိမ်းခြောက်မှုအကြောင်း အရေးကြီးသော အချက်အလက်များကို သင်ထည့်သွင်းနိုင်သည်။
- Justification field: ဤအကွက်တွင် သီးခြားခြိမ်းခြောက်မှုကို သင်လက်ခံရန် သို့မဟုတ် ငြင်းပယ်ရန် ရွေးချယ်ရသည့်အကြောင်းရင်းအကြောင်း အချက်အလက်များကို သင်ထည့်သွင်းနိုင်သည်။ ဤအချက်အလက်သည် ခြိမ်းခြောက်မှုပုံစံကို ပြန်လည်သုံးသပ်နေသော အခြားအဖွဲ့ဝင်များအတွက်သာမက နောင်ကိုးကားရန်အတွက်လည်း အထောက်အကူဖြစ်နိုင်သည်။
- Priority box: ဤနေရာတွင် ခြိမ်းခြောက်မှု၏ ဦးစားပေးမှုကို High, Medium သို့မဟုတ် Low ဟု သတ်မှတ်နိုင်သည်။
- Team box: ဤနေရာတွင် သီးခြားအဖွဲ့တစ်ခုသို့ ခြိမ်းခြောက်မှုကို သင်တာဝန်ပေးနိုင်သည်။
- Status box: ဤနေရာတွင် ခြိမ်းခြောက်မှုအခြေအနေကို Not Started, Needs Investigation, Not Applicable သို့မဟုတ် Mitigated ဟု သတ်မှတ်နိုင်သည်။

Export CSV ကို ရွေးချယ်ခြင်းဖြင့် ခြိမ်းခြောက်မှုစာရင်းကို CSV ဖိုင်အဖြစ် ဒေါင်းလုဒ်လုပ်နိုင်သည်။ ၎င်းသည် Microsoft Threat Modeling tool ကို ထည့်သွင်းမထားသော သက်ဆိုင်သူများနှင့် မျှဝေနိုင်သော ခွဲခြားသတ်မှတ်ထားသော ခြိမ်းခြောက်မှုများ၏ စနစ်တကျနှင့် အလွယ်တကူရယူနိုင်သော မှတ်တမ်းတစ်ခုကို သင့်အားပေးသည်။ လိုအပ်ပါက နောက်ထပ်ခွဲခြမ်းစိတ်ဖြာခြင်း၊ စီခြင်း၊ စစ်ထုတ်ခြင်း သို့မဟုတ် ဒေတာကိုင်တွယ်ခြင်းတို့ကို လုပ်ဆောင်ရန်လည်း ၎င်းကို သင်အသုံးပြုနိုင်သည်။ တင်ပို့ထားသော CSV ဖိုင်၏ နမူနာကို ဤနေရာတွင် ကြည့်ရှုပါ-

Threatlist-activity
CSV File

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/1ay5ZJgtRAep8T4mg9BDRg_1bf545d59f804e849376812b5e619fe1_image.png?expiry=1744416000000&hmac=VG1sb0Q7VGceNrhM0YG-ajlVyNWUsk_C3P2LIWd2Eiw">

ထိပ် toolbar ရှိ Reports menu ကို ရွေးချယ်ပြီး Create Full Report ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/hqSx4grrTmKRDM04JEYKAA_5c6ab9a137db4358950d14896745c5e1_image.png?expiry=1744416000000&hmac=sFK6EGc6JA1OTN4oSxAyqv9bGeR87SqfdJFyLB8gHGA">

Popup window တစ်ခုပေါ်လာလိမ့်မည်။ Countermeasure, Risk နှင့် Team options များကို ရွေးချယ်ပြီး Generate Report ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/hqSx4grrTmKRDM04JEYKAA_5c6ab9a137db4358950d14896745c5e1_image.png?expiry=1744416000000&hmac=sFK6EGc6JA1OTN4oSxAyqv9bGeR87SqfdJFyLB8gHGA">

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/FiQ056tyRf6Tco_TUqnaCg_6a256f628f504b8b962c01f4e02380e1_image.png?expiry=1744416000000&hmac=CPav_xuJ-lC2ACcFnwjlolcYsRavTYShtXTTF8RO83E">

အစီရင်ခံစာကို ပြန်လည်သုံးသပ်ပါ
Sample_Threat Model_https.tm7 b အတွက် အစီရင်ခံစာကို ဤနေရာတွင် ပြန်လည်သုံးသပ်ပါ-

Sample_Threat Model_https_Report
HTM File

Sample_Threat Model_https_Report.pdf
PDF File

## Conclusion (နိဂုံး)

ဂုဏ်ယူပါတယ်! ဤလှုပ်ရှားမှုတွင် ပံ့ပိုးပေးထားသော ဖန်သားပြင်ဓာတ်ပုံများနှင့် ညွှန်ကြားချက်များကို လိုက်နာခြင်းဖြင့် သင်သည် Microsoft Threat Modeling Tool ကို ယခုအသုံးပြုနိုင်ပြီဖြစ်သည်။ ဤကိရိယာသည် သင်၏ဆော့ဖ်ဝဲလ်စနစ်များအတွက် ခြိမ်းခြောက်မှုများကို ခွဲခြမ်းစိတ်ဖြာခြင်းနှင့် လျှော့ချခြင်းအတွက် အဖိုးတန်အရင်းအမြစ်တစ်ခုဖြစ်သည်။ ၎င်းသည် နောက်ဆက်တွဲ လေ့ကျင့်ခန်းနှင့် ကိုယ်တိုင်ပြန်လည်သုံးသပ်ခြင်းကို အောင်မြင်စွာ ပြီးမြောက်ရန် သင့်အား အဆင်သင့်ဖြစ်စေပါသည်။
