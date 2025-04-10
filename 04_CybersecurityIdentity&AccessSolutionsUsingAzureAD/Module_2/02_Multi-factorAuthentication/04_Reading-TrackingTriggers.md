# Tracking triggers

[Tracking triggers 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/supplement/4XcM5/tracking-triggers)

# အစပျိုးမှုများကို ခြေရာခံခြင်း

## နိဒါန်း

ယခင်က၊ ဘက်ပေါင်းစုံ အထောက်အထားစိစစ်ခြင်း (MFA) သည် လုံခြုံရေးကို အားကောင်းစေပြီး ဟက်ကာများအတွက် ဝင်ရောက်မှုကို ခက်ခဲစေနိုင်ပုံကို သင်စူးစမ်းလေ့လာခဲ့သည်။ ၎င်းသည် ဝင်ရောက်မှုအချက်များကို စောင့်ကြပ်ခြင်းမှ အာရုံပြောင်းကာ ကွန်ရက်ကို မည်သူဝင်ရောက်နေသည်ကို ဆုံးဖြတ်ခြင်းအပေါ် အာရုံစိုက်သည့် ပြောင်းလဲမှုကိုလည်း ထင်ဟပ်စေသည်။

ဤစာဖတ်ခြင်းသည် အခြေအနေအလိုက် ဝင်ရောက်ခွင့်နှင့် အထောက်အထားကာကွယ်မှုတို့ မည်သို့အလုပ်လုပ်သည်ကို သင်သင်ယူခဲ့သည့်အရာများကို ချဲ့ထွင်ပြီး၊ ဤမူဝါဒများအောက်တွင် MFA ကို အစပျိုးစေနိုင်သည့် အကြောင်းအချက်အချို့ကို တင်ပြထားသည်။ ထို့ပြင်၊ ဤအရာများကို အစားထိုးနိုင်သည့် စိတ်ကြိုက်မူဝါဒများကို မည်သို့သတ်မှတ်နိုင်သည်နှင့် အက်မင်များက MFA ကို အသုံးပြုသူများမှ မည်သည့်အချိန်၊ မည်သို့ အစပျိုးခံရသည်ကို မည်သို့ခြေရာခံနိုင်သည်ကိုလည်း သင်ရှာဖွေတွေ့ရှိမည်ဖြစ်သည်။

## လှုပ်ရှားမှုနှင့်ဆိုင်သော MFA အစပျိုးမှုများ

ကုမ္ပဏီတစ်ခု၏ အကောင့်များနှင့် အပလီကေးရှင်းများသို့ ခွင့်ပြုချက်မရှိသော ဝင်ရောက်မှုသည် ပျက်စီးမှုများနှင့် ကုန်ကျစရိတ်များစွာသော အကျိုးဆက်များကို ဖြစ်ပေါ်စေနိုင်သည်။ MFA သည် အသုံးပြုသူအမည်နှင့် စကားဝှက်အသုံးပြုမှုထက် ထပ်လောင်းစိစစ်ရန်ပုံစံတစ်ခု လိုအပ်ခြင်းဖြင့် ခွင့်ပြုချက်မရှိသော ဝင်ရောက်မှုကို တားဆီးပေးသည်။ ၎င်းသည် ခွင့်ပြုချက်မရှိသော အကောင့်အသုံးပြုမှုနှင့် ဆိုက်ဘာတိုက်ခိုက်မှုများကို ထိရောက်စွာ ကာကွယ်ပေးနိုင်ကြောင်း သက်သေပြခဲ့သည်။

ဒါဆိုရင် Azure AD တွင် MFA ကို ဖြစ်ပေါ်စေသော အစပျိုးမှုများက ဘာတွေလဲ။ အနီးကပ်စောင့်ကြည့်ထားသော နယ်ပယ်တစ်ခုမှာ ဝင်ရောက်ခြင်းနှင့် သက်ဆိုင်သည်။ ဤသည်မှာ MFA ကို ဖြစ်ပေါ်စေနိုင်သည့် ဝင်ရောက်လှုပ်ရှားမှုအချို့ဖြစ်သည်။

- စက်ကိရိယာအသစ်မှ ဝင်ရောက်ခြင်း
- အမည်မသိ IP လိပ်စာမှ ဝင်ရောက်ခြင်း
- ထူးခြားလှုပ်ရှားမှုရှိသော တည်နေရာမှ ဝင်ရောက်ခြင်း
- အန္တရာယ်များသော နိုင်ငံ/ဒေသမှ ဝင်ရောက်ခြင်း
- အချိန်ကြာရှည် မလှုပ်ရှားပြီးနောက် ဝင်ရောက်ခြင်း
- ပုံမှန်လုပ်ငန်းချိန်ပြင်ပမှ ဝင်ရောက်ခြင်း
- သံသယဖြစ်ဖွယ်လှုပ်ရှားမှုရှိသော IP လိပ်စာမှ ဝင်ရောက်ခြင်း

## အခြေအနေအလိုက် ဝင်ရောက်ခွင့်တွင် MFA အကျဉ်းချုပ်

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/vxegjQfST6eWY-SAFx2BYQ_754817d9f2cb484483a153c128e8c4e1_C4M2L2_Item4_Img1_conditional_access_overview.png?expiry=1742947200000&hmac=of50wKs_GqET2AioFbxO-bV-37dNERF3kdXvPdsBIew">

Azure AD ၏ ရှုထောင့်မှ ဤအပြုအမူတစ်ခုချင်းစီသည် သံသယဖြစ်ဖွယ်ဟု မည်ကဲ့သို့ ခံစားရပြီး ၎င်းကို မည်သို့တုံ့ပြန်မည်ကို ဆင်ခြင်ကြည့်ကြပါစို့။

- **စက်ကိရိယာအသစ်မှ ဝင်ရောက်ခြင်း**  
  ကွန်ရက်သို့ စက်ကိရိယာအသစ်ဖြင့် ဝင်ရောက်ခြင်းသည် ဒုတိယအထောက်အထားစိစစ်မှု တောင်းဆိုမှုကို အမြဲဖြစ်ပေါ်စေသည်။ သိထားသော စက်ကိရိယာသည် ဟက်ကာတစ်ဦးမှ အသုံးပြုနိုင်ဖွယ်နည်းပြီး သိထားသော အသုံးပြုသူနှင့် ဆက်စပ်နိုင်ဖွယ်ပိုများသည်။

- **အမည်မသိ IP လိပ်စာမှ ဝင်ရောက်ခြင်း**  
  အမည်မသိ IP လိပ်စာသည် သိထားသော ကုမ္ပဏီ သို့မဟုတ် အဖွဲ့အစည်းနှင့် မသက်ဆိုင်သော လိပ်စာတစ်ခုဖြစ်သည်။ ပုံမှန်အားဖြင့် ဟက်ကာများသည် ကုမ္ပဏီနှင့် ဆက်စပ်မှုလိုအပ်သော ကုမ္ပဏီလိပ်စာများကို အသုံးပြုမည်မဟုတ်ဘဲ၊ ၎င်းသည် ခြေရာခံနိုင်သည့် မှတ်တမ်းတစ်ခု ချန်ထားနိုင်သည်။ ထိုအစား၊ ဟက်ကာတစ်ဦးသည် အမည်မသိလိပ်စာကို အသုံးပြုနိုင်ဖွယ်ပိုများသည်။ ၎င်းကို Azure က အန္တရာယ်ရှိသော ဝင်ရောက်မှုအဖြစ် အမှတ်အသားပြုပြီး MFA တောင်းဆိုမှုကို ဖြစ်ပေါ်စေသည်။

- **ထူးခြားလှုပ်ရှားမှုရှိသော တည်နေရာမှ ဝင်ရောက်ခြင်း**  
  သင့်ယခင်ဝင်ရောက်မှု မှတ်တမ်းအပေါ် အခြေခံ၍ ထူးခြားသော သို့မဟုတ် မမျှော်လင့်ထားသော တည်နေရာမှ ဝင်ရောက်ပါက၊ Azure AD က ၎င်းကို အန္တရာယ်ရှိသော ဝင်ရောက်မှုအဖြစ် အမှတ်အသားပြုပြီး MFA တောင်းဆိုမှုကို ဖြစ်ပေါ်စေသည်။

- **အန္တရာယ်များသော နိုင်ငံ/ဒေသမှ ဝင်ရောက်ခြင်း**  
  AAD သို့ ဝင်ရောက်သောအခါ၊ သင်မည်သည့်နေရာမှ ဝင်ရောက်နေသည်၊ ဘာကို ဝင်ရောက်ရန် ကြိုးစားနေသည်၊ သင့်စက်ကိရိယာ ID၊ သို့မဟုတ် နေ့၏အချိန်ကဲ့သို့ အသုံးပြုသူအသေးစိတ်အချက်များကို မှတ်တမ်းတင်သည်။ ၎င်းက AAD အား ဆိုက်ဘာတိုက်ခိုက်မှု ပြုလုပ်ရန် အန္တရာယ်များ သို့မဟုတ် နည်းသော ဒေသများစာရင်းကို စုစည်းစေခဲ့သည်။ အန္တရာယ်များသော နေရာမှ ဝင်ရောက်ခြင်းသည် MFA တောင်းဆိုမှုကို ဖြစ်ပေါ်စေနိုင်သည်။

- **အချိန်ကြာရှည် မလှုပ်ရှားပြီးနောက် ဝင်ရောက်ခြင်း**  
  အချိန်ကြာရှည် အသုံးမပြုထားသော စက်ကိရိယာတစ်ခုသည် ဆုံးရှုံးသွားသော စက်ကိရိယာ သို့မဟုတ် မသုံးတော့သော စက်ကိရိယာကဲ့သို့ အကြောင်းအမျိုးမျိုးကြောင့် ဖြစ်နိုင်သည်။ ထိုသို့သော စက်ကိရိယာမှ ဝင်ရောက်ကြိုးစားမှုသည် MFA ကို ဖြစ်ပေါ်စေသည်။

- **ပုံမှန်လုပ်ငန်းချိန်ပြင်ပမှ ဝင်ရောက်ခြင်း**  
  ပုံမှန်ဝင်ရောက်မှု အပြုအမူသည် အလုပ်ချိန်အတွင်း ဖြစ်ပွားသည်။ ဝန်ထမ်းတစ်ဦးသည် အလုပ်ချိန်ပြင်ပ ဝင်ရောက်ခြင်းသည် မထူးဆန်းသော်လည်း၊ ၎င်းသည် ပြဿနာတစ်ခု၏ သေးငယ်သော အရိပ်အယောင်တစ်ခု ဖြစ်နိုင်သည်။ Azure အထောက်အထားကာကွယ်မှု၏ စက်သင်ယူမှု စွမ်းရည်များသည် အသုံးပြုသူ၏ အလုပ်ပုံစံကို လိုက်လျောညီထွေ သင်ယူနိုင်သည်။ သို့သော်၊ ၎င်းသည် AAD လိုင်စင်အားလုံးနှင့် မသက်ဆိုင်ဘဲ၊ အသုံးပြုသူ၏ ပုံစံကို ရင်းနှီးလာရန် အချိန်ယူရသည်။

- **သံသယဖြစ်ဖွယ်လှုပ်ရှားမှုရှိသော IP လိပ်စာမှ ဝင်ရောက်ခြင်း**  
  သံသယဖြစ်ဖွယ်လှုပ်ရှားမှုသည် ဟက်ကင်းသို့ ဦးတည်သည့် လှုပ်ရှားမှုကို မဆိုလိုပါ။ အထက်တွင် ဖော်ပြထားသည့်အတိုင်း သတိပေးအချက်များ ဖြစ်ပေါ်စေနိုင်သည့် လုပ်ဆောင်ချက်များကို ရည်ညွှန်းသည်။ ဥပမာ၊ သင်သည် စကားဝှက်များကို မှတ်မိရန် ညံ့ဖျင်းပြီး မမှန်ကန်သော စကားဝှက်ကို ထည့်သွင်းနိုင်သည်၊ သို့မဟုတ် သင်သည် ဟက်ကာတစ်ဦးဖြစ်ပြီး အကြမ်းဖက်တိုက်ခိုက်မှုကို အသုံးပြုနေနိုင်သည်။ AAD သည် အသုံးပြုသူလှုပ်ရှားမှုကို သိမ်းဆည်းထားပြီး MFA ကို မည်သည့်အချိန်တွင် တောင်းဆိုရမည်ကို ဆုံးဖြတ်ရန် အသုံးပြုသည်။

ယခင်ဖော်ပြခဲ့သည့်အတိုင်း၊ Azure AD ၏ အထောက်အထားကာကွယ်မှုနှင့် အခြေအနေအလိုက် ဝင်ရောက်ခွင့်သည် ဤသတ်မှတ်ချက်များကို ဆုံးဖြတ်သည့် နည်းလမ်းများဖြစ်သည်။ အထောက်အထားကာကွယ်မှုကို အသုံးပြု၍ မူဝါဒများကို သတ်မှတ်ထားပြီး၊ အန္တရာယ်အချက်များ ဖြစ်ပေါ်လာသောအခါ MFA ကို အလိုအလျောက် အစပျိုးနိုင်သည်။ အခြေအနေအလိုက် ဝင်ရောက်ခွင့်၏ အဓိပ္ပါယ်ဖွင့်ဆိုချက်သည် တည်နေရာ သို့မဟုတ် စက်ကိရိယာနှင့်ဆိုင်သော အချက်အလက်ကဲ့သို့ သတ်မှတ်ထားသော အချက်ပြမှုတစ်ခုကို ပေးရန် MFA လိုအပ်သော မူဝါဒများကို ဖန်တီးသည်။

## MFA လုပ်ငန်းစဉ်

MFA ကို အစပျိုးစေသော ဝင်ရောက်လှုပ်ရှားမှုများကို သတ်မှတ်ပြီးသည်နှင့်၊ အသုံးပြုသူဘက်မှ မည်သည့်အတွေ့အကြုံကို ဖန်တီးနိုင်မည်နည်း။ ရှာဖွေရန် ဝင်ရောက်မှုလုပ်ထုံးလုပ်နည်းတစ်ခု၏ ဥပမာကို ဖြတ်သန်းကြည့်ကြပါစို့။

အသုံးပြုသူအမည်နှင့် စကားဝှက်ကို တင်သွင်းပြီးနောက်၊ အသုံးပြုသူသည် ဆက်လက်မလုပ်ဆောင်မီ နောက်ထပ်အချက်အလက် လိုအပ်ကြောင်း အသိပေးချက်တစ်ခု ရရှိသည်။

- **ဝင်ရောက်ရန် ကြိုးစားမှုကြောင့် နောက်ထပ်အချက်အလက် လိုအပ်ကြောင်း အသိပေးချက်**

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/hM03XTI9TpeXdLes-qWjZw_1c42009e59964e2a9fbb994d346b3ee1_C4M2L2_item04_img02.png?expiry=1742947200000&hmac=9RATgsnGoY9Mbcjk6DGphPiCH2lLuAjtyw3D-hGZ1KA">

နောက်တစ်ဆင့်* ကို ရွေးချယ်ပြီးနောက်၊ အသုံးပြုသူသည် ခွင့်ပြုထားသော စိစစ်ရန်နည်းလမ်းတစ်ခု ထည့်သွင်းရန် တောင်းဆိုခံရသည်။ ဤကိစ္စတွင်၊ *မိုဘိုင်းအက်ပ်\_ ကို ရွေးချယ်ထားပြီး၊ ၎င်းသည် Microsoft Authenticator အက်ပ်သို့ အသိပေးချက် သို့မဟုတ် စိစစ်ရန်ကုဒ်တစ်ခု ပေးပို့မည်ဖြစ်သည်။

- **ဝင်ရောက်ရန်အတွက် ထပ်လောင်းလုံခြုံရေး စိစစ်ရန်နည်းလမ်းကို ရွေးချယ်ပြီး ပြင်ဆင်သတ်မှတ်ရန် တောင်းဆိုချက်**

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/VYZBHG7nSCODFitgTdvX0A_9b03242098364f10a51b2efab05555e1_C4M2L2_item04_img03.png?expiry=1742947200000&hmac=4Cj_Y_jp3lmZh6WGqJBhP_YlHH7OU7VYhEymH02_FwU">

အသုံးပြုသူသည် ပြင်ဆင်သတ်မှတ်မှုကို ပြီးမြောက်သည်နှင့်၊ ထပ်မံဝင်ရောက်ရန် တောင်းဆိုခံရမည်ဖြစ်သည်။ ဤအကြိမ်တွင်၊ အသုံးပြုသူသည် ရွေးချယ်ထားသော အထောက်အထားစိစစ်မှုနည်းလမ်းအတွက် တောင်းဆိုချက်တစ်ခု ရရှိမည်ဖြစ်သည်။

- **Microsoft Authenticator အက်ပ်တွင် လုပ်ဆောင်ရန် လိုအပ်သည့် ဝင်ရောက်ခွင့်ပြုမှု တောင်းဆိုချက်ကို ပေးပို့ပြီးကြောင်း ဖော်ပြသည့် မက်ဆေ့ချ်**

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/AmD_jWmdSnqbL2Y0Tad6nQ_0b14f30c5a9643129485ffab0c667fe1_C4M2L2_item04_img04.png?expiry=1742947200000&hmac=ilq6QKJ-phinYygiKWJx_nx6pOuv8zSOW6671Z7vwWs">

## မူဝါဒနှင့်ဆိုင်သော MFA အစပျိုးမှုများ

MFA သည် ကမ္ဘာလုံးဆိုင်ရာအဆင့်တွင် အစပျိုးနိုင်ပြီး အကောင့်တစ်ခုလုံးကို ထိခိုက်စေနိုင်သည်။ Azure Active Directory ကို ဖန်တီးသောအခါ၊ အရာအားလုံးကို သက်ရောက်မည့် မူလသတ်မှတ်ချက်အချို့ ရှိမည်ဖြစ်သည်။ ဥပမာ၊ အသုံးပြုသူအားလုံးအတွက် MFA ကို မှတ်ပုံတင်ရန် ကမ္ဘာလုံးဆိုင်ရာ လိုအပ်ချက်တစ်ခု ရှိသည်။

သို့သော်၊ ဤအပြုအမူကို အစားထိုးနိုင်ပြီး၊ MFA ကို သတ်မှတ်ထားသော ဖြစ်ရပ်များအတွက် သတ်မှတ်ပေးနိုင်သည်။ MFA ၏ ဒေသဆိုင်ရာ ဥပမာတစ်ခု ဖန်တီးခြင်းကို မူဝါဒအသစ်တစ်ခု ဖန်တီးခြင်းဟု ခေါ်သည်။ ၎င်းက မည်သို့အသုံးဝင်နိုင်သည်ကို နားလည်ရန်၊ သင်ကာကွယ်လိုသော အထိခိုက်မခံသော ဒေတာများသို့ ဝင်ရောက်ခွင့်ရှိသည့် အပလီကေးရှင်းတစ်ခု ရှိသည်ဟု စိတ်ကူးကြည့်ပါ။ ဝင်ရောက်မှုကို လုံခြုံစွာ ပြုလုပ်ကြောင်း သေချာစေရန်၊ စက်ကိရိယာအသစ် သို့မဟုတ် မသိသော စက်ကိရိယာမှ ဤအပလီကေးရှင်းသို့ ဝင်ရောက်ရန် ကြိုးစားမှုတိုင်းသည် MFA ကို အစပျိုးစေမည်ဟု မူဝါဒတစ်ခု ဖန်တီးနိုင်သည်။ ၎င်းသည် အခြားဝန်ဆောင်မှုများသို့ ဝင်ရောက်မှု သို့မဟုတ် မှတ်ပုံတင်ထားသော စက်ကိရိယာများဖြင့် ဤအပလီကေးရှင်းသို့ ဝင်ရောက်မှုကို ထိခိုက်မည်မဟုတ်ပါ။

မူဝါဒတစ်ခု ပြင်ဆင်သတ်မှတ်သောအခါ၊ အက်မင်များသည် MFA ၏ အသုံးပြုမည့်နည်းလမ်းကို ဆုံးဖြတ်နိုင်ပြီး အသုံးပြုသူတစ်ဦးမှ မှတ်ပုံတင်ထားသော MFA ပုံစံများကို ကြည့်ရှုနိုင်သည်။ အက်မင်တစ်ဦးသည် MFA သို့မဟုတ် ကိုယ်တိုင်ဝန်ဆောင်မှု စကားဝှက်ပြန်လည်သတ်မှတ်ခြင်း (SSPR) ကို အစပျိုးခံရသောအခါ အသုံးပြုသူ၏ အကောင့်သို့ အီးမေးလ်တစ်စောင် ပေးပို့ရန် ပြင်ဆင်သတ်မှတ်နိုင်သည်။ ထို့ပြင်၊ အက်မင်များသည် အသုံးပြုသူတစ်ဦးစီမှ စနစ်နှင့် ဆက်သွယ်မှုများကို ကြည့်ရှုရန် လှုပ်ရှားမှုမှတ်တမ်းများကို ပြန်လည်သုံးသပ်နိုင်သည်။

## နိဂုံးချုပ်

ဤစာဖတ်ခြင်းတွင်၊ အထောက်အထားနှင့် အခြေအနေအလိုက် ဝင်ရောက်ခွင့်နှင့် ဆက်စပ်နေသော ဝင်ရောက်မှု အပြုအမူများစွာကို သင်သတိပြုမိခဲ့ပြီး၊ ၎င်းတို့သည် MFA တောင်းဆိုမှုကို ဖြစ်ပေါ်စေမည်ဖြစ်သည်။ ဤအပြုအမူများသည် ဟက်ကင်းဖြစ်နိုင်ခြေ၏ လက္ခဏာများ မဟုတ်သော်လည်း၊ ၎င်းတို့သည် ယခင်ဟက်ကင်းများမှ ဖော်ထုတ်ခံရသော ဟက်ကင်းဖြစ်နိုင်ခြေ၏ အရိပ်အယောင်များဖြစ်သည်။ ထို့ကြောင့်၊ ၎င်းတို့ကို ဖော်ထုတ်တွေ့ရှိသောအခါ MFA ကို ထပ်လောင်းအတားအဆီးအဖြစ် ထည့်သွင်းရန် အကျိုးရှိသည်။ ထို့ပြင်၊ အက်မင်များသည် လိုအပ်သည့်နေရာတွင် ဤစည်းမျဉ်းများကို အစားထိုးနိုင်သည့် မူဝါဒများကို သတ်မှတ်နိုင်ပြီး အသုံးပြုသူများမှ အစပျိုးခံရသော MFA နည်းလမ်းများကို စောင့်ကြည့်နိုင်ကြောင်းလည်း သင်သင်ယူခဲ့သည်။
