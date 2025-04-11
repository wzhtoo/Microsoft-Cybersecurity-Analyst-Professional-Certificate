# Exemplar: Web application threat modeling

[Exemplar: Web application threat modeling 🔗](https://www.coursera.org/learn/advanced-cybersecurity-concepts-and-capstone-project/supplement/lgog2/exemplar-web-application-threat-modeling)

# Exemplar: Web application threat modeling (နမူနာ: ဝဘ်အပလီကေးရှင်း ခြိမ်းခြောက်မှုပုံစံဖော်ခြင်း)

C8M1L4 Item 08

## Introduction (နိဒါန်း)

ဝဘ်အပလီကေးရှင်း ခြိမ်းခြောက်မှုပုံစံဖော်ခြင်း

လေ့ကျင့်ခန်းတွင် ဝဘ်အက်ပ် ဗိသုကာလက်ရာအတွက် ပြည့်စုံသော ခြိမ်းခြောက်မှုပုံစံတစ်ခုကို သင်ဖန်တီးခဲ့သည်။
ဖြစ်နိုင်ချေရှိသော ခြိမ်းခြောက်မှုများနှင့် ၎င်းတို့၏ သက်ဆိုင်ရာ လျှော့ချမှုများကို မှတ်တမ်းတင်ရန် အစွမ်းထက်သော Microsoft Threat Modeling Tool ကို အသုံးပြု၍ လုံခြုံရေးဆိုင်ရာ ထည့်သွင်းစဉ်းစားမှုများကို မြှင့်တင်ခြင်းသည် သင်၏ အဓိကအာရုံစိုက်မှုဖြစ်သည်။ ဤနမူနာသည် လုပ်ငန်းအတွက် ဖြစ်နိုင်ချေရှိသော အဖြေတစ်ခုအဖြစ် လုပ်ဆောင်သည်။ သင်၏လုပ်ငန်းစဉ်ကို ဤနေရာတွင် ဖော်ပြထားသော လုပ်ငန်းစဉ်နှင့် နှိုင်းယှဉ်ရန် အဆင့်များအတိုင်း လိုက်နာပါ။

## Instructions (ညွှန်ကြားချက်များ)

ဝဘ်အပလီကေးရှင်းပုံကို ပြန်လည်သုံးသပ်ပါ။ "Targeted Web App Architecture Threat Model" ဟု အမည်ပေးထားသော မော်ဒယ်အသစ်တစ်ခုကို ဖန်တီးရန် Microsoft Threat Model Tool ကို ဖွင့်ပါ။
Stencils panel မှ ၎င်းတို့ကို ဆွဲယူ၍ ချခြင်းဖြင့် သင်၏ပုံအတွက် အစိတ်အပိုင်းများကို ထည့်ပါ။ စနစ်၏ ရှင်းလင်းသော ကိုယ်စားပြုမှုအတွက် ဤအစိတ်အပိုင်းများကို ချိတ်ဆက်ထားသင့်သည်။ အောက်ပါနမူနာပုံတွင် ဖော်ပြထားသည့်အတိုင်း ရှင်းလင်းမှုကို မြှင့်တင်ရန် စာသားအညွှန်းများနှင့် ဖော်ပြချက်များလည်း ရှိသင့်သည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/oNGLNRFYS1aFzdKfJu4cBg_03b4a692ed8c4cf391adc5e9249a14e1_image.png?expiry=1744416000000&hmac=LWJS5LRmuT2EkoZhN9ykWTFTknBjBV0CC_EULfaLT_c">

မျက်နှာပြင်၏ ဘယ်ဘက်အပေါ်ထောင့်ရှိ toolbar ရှိ စာမျက်နှာနှင့် မှန်ဘီလူးပုံသင်္ကေတကို ရွေးချယ်ခြင်းဖြင့် ခြိမ်းခြောက်မှုပုံစံကို ခွဲခြမ်းစိတ်ဖြာရန် Analysis View သို့ ပြောင်းပါ။ သင်ချဲ့ထွင်နိုင်သော Threat List panel သည် အောက်ပါဖန်သားပြင်ဓာတ်ပုံတွင် မြင်တွေ့နိုင်သည့်အတိုင်း ဖြစ်နိုင်ချေရှိသော ခြိမ်းခြောက်မှုများကို အလွယ်တကူ ပြသထားသည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/b6XNkPPKQJWd1lTubC6mTg_ffad57f78c3c40d98551c1db8d37efe1_image.png?expiry=1744416000000&hmac=P7ptaoFMV9I9UdFtRhwnL98bOOUWTx42y6-RQnqr09Q">

CSV ဖိုင်ပုံစံဖြင့် ခြိမ်းခြောက်မှုများ၏ အသေးစိတ်အချက်အလက်အားလုံးကို လေ့လာရန် ပိုမိုလွယ်ကူသည်။ အောက်ပါလင့်ခ်မှတစ်ဆင့် CSV ဖိုင်ကို ဖွင့်ပါ-

Threats List
CSV File

စာရင်းမှ ခြိမ်းခြောက်မှုများကို ရွေးချယ်ခြင်းဖြင့် Threat Properties panel ကို စစ်ဆေးပါ။ ဤနေရာတွင် ခြိမ်းခြောက်မှုအခြေအနေ၊ ဦးစားပေးမှုနှင့် အဖွဲ့တာဝန်ပေးအပ်မှုများကဲ့သို့သော ခြိမ်းခြောက်မှုအသေးစိတ်အချက်အလက်များကို သင်ရယူနိုင်ပြီး သတင်းအချက်အလက်အပေါ် အခြေခံ၍ ဆုံးဖြတ်ချက်များချမှတ်နိုင်စေပါသည်။ Threats Properties panel သည် သင့်အား ပိုမိုနက်ရှိုင်းသော ထိုးထွင်းသိမြင်မှုများကို ပေးပါသည်။ ဥပမာအားဖြင့် စုံစမ်းစစ်ဆေးရန် လိုအပ်သော ခြိမ်းခြောက်မှုများကို သင့်အာရုံစိုက်ရန် မီးမောင်းထိုးပြထားသည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/jwZgUVWpQii4VsGu3SYEAQ_ebcf7ed52ee747ceb0b5cce2b4f126e1_image.png?expiry=1744416000000&hmac=af_M3oLlfkKOTjACtgP9WsdhUr_L1IobLNFdfwVECIg">

ထိပ် toolbar ရှိ Reports menu ကို ရွေးချယ်ပြီး Create Full Report ကို ရွေးချယ်ခြင်းဖြင့် ခြိမ်းခြောက်မှုပုံစံ၏ ရှုထောင့်အားလုံးကို လွှမ်းခြုံသော အပြည့်အစုံ အစီရင်ခံစာကို ထုတ်လုပ်ပါ။ Popup window တစ်ခုပေါ်လာလိမ့်မည်။ Countermeasure, Risk နှင့် Team options များကို ရွေးချယ်ပြီး Generate Report ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/O-91Scm9S7i1XOgpwhdOuQ_5825d7b1ae114b84aff473d832e68ee1_image.png?expiry=1744416000000&hmac=DAfduoL30XM2FFINP-XL5zpdFcCPGuCtHZZ7UWbkVj0">

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/MavgGSI8TxmSiciNpW30EQ_4ce758f0804f4cbaac11e59decafe3e1_image.png?expiry=1744416000000&hmac=FtFfE9UdSdX0ZcgnR-pgFqV1oTKrGH8ARwuV9ssSihU">

သင်၏အစီရင်ခံစာကို နမူနာအစီရင်ခံစာနှင့် နှိုင်းယှဉ်ပါ-

Web Application Threat Modeling
HTM File

နမူနာပုံစံကို ပိုမိုစစ်ဆေးရန် Microsoft Threat Modeling Tool တွင် TM7 ဖိုင်ကို ဖွင့်ပါ-

Web Application Threat Modeling
TM7 File

## Conclusion (နိဂုံး)

ဤလေ့ကျင့်ခန်းသည် စနစ်၏လုံခြုံရေးကို ကာကွယ်ရန် အရေးကြီးသောအဆင့်ဖြစ်သော ခိုင်မာသော ခြိမ်းခြောက်မှုပုံစံတစ်ခုကို ဖန်တီးခြင်းဖြင့် အထွတ်အထိပ်သို့ ရောက်ရှိခဲ့သည်။ Microsoft Threat Model Tool ကို အသုံးပြုခြင်းဖြင့် ဖြစ်နိုင်ချေရှိသော လုံခြုံရေးဆိုင်ရာ အန္တရာယ်များကို စနစ်တကျ ခွဲခြားသတ်မှတ်ပြီး ကိုင်တွယ်ဖြေရှင်းကာ ဝဘ်အပလီကေးရှင်းနှင့် ၎င်းနှင့်ဆက်စပ်သော အစိတ်အပိုင်းများကို ခြိမ်းခြောက်မှုများနှင့် အားနည်းချက်များမှ ကာကွယ်နိုင်ခဲ့သည်။
