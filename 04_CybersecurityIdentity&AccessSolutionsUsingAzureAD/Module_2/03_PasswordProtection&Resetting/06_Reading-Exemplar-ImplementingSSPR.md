# Exemplar: Implementing SSPR

[Exemplar: Implementing SSPR 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/supplement/4mqKj/exemplar-implementing-sspr)

# Exemplar: Implementing SSPR (နမူနာ: SSPR အကောင်အထည်ဖော်ခြင်း)

## Overview (ခြုံငုံသုံးသပ်ချက်)

ယခင်လေ့ကျင့်ခန်းတွင်၊ သင်သည် ကိုယ်တိုင်ဝန်ဆောင်မှု စကားဝှက်ပြန်လည်သတ်မှတ်ခြင်း (SSPR) ကို ပိုမိုနက်ရှိုင်းစွာ စူးစမ်းခဲ့သည်။ သင်သည် အဖွဲ့နှစ်ဖွဲ့ ဖန်တီးရန် တာဝန်ပေးခံခဲ့ရသည်။ ပထမအဖွဲ့သည် SSPR ဖွင့်ထားပြီး ပြဿနာရှိပါက ၎င်းတို့၏ စကားဝှက်များကို ပြန်လည်သတ်မှတ်နိုင်ပြီး၊ နောက်အဖွဲ့တစ်ဖွဲ့သည် ဤအခွင့်အာဏာကို ရယူနိုင်မီ အက်မင်မှတစ်ဆင့် ဖြတ်သန်းရမည်။ ထို့ပြင်၊ သင်၏ လုပ်ငန်းစဉ်ကို တူညီသော ခေါင်းစဉ်များအောက်တွင် စာရင်းပြုစုပြီး သင့်ရလဒ်များကို သင့်လျော်သော စခရင်ရှော့များဖြင့် ပံ့ပိုးရန် တောင်းဆိုခံခဲ့ရသည်။  
အောက်တွင်၊ ဖော်ပြသင့်သော အချက်အလက်များ၏ နမူနာတစ်ခုကို သင်တွေ့ရမည်ဖြစ်သည်။

## Exemplar: Implementing SSPR (နမူနာ: SSPR အကောင်အထည်ဖော်ခြင်း)

## Step 1: Create the first group (အဆင့် ၁: ပထမအဖွဲ့ကို ဖန်တီးခြင်း)

_Manage_ တဘ်မှ _Groups_ ကို ရွေးချယ်ပါ။  
ထို့နောက် _New group_ ကို ရွေးချယ်ပါ။  
"SSPR*Enabled" ဟု အမည်ပေးထားသော အဖွဲ့တစ်ဖွဲ့ကို ဖန်တီးပါ။  
\_SSPR အဖွဲ့အသစ် စခရင်မှ ခြုံငုံသုံးသပ်ချက်သို့ အဖွဲ့တစ်ဖွဲ့ ဖန်တီးခြင်း*

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/KgFOAxBBTDGL7D8MFcy0nA_ac6c76a36362454390eb63356ba97ce1_C4M2L3_Itm6_Img1.png?expiry=1743033600000&hmac=WZcgOSXbeCiprMtX1MrBRwNAojW1YSe6FvS7HCh0vNM">

## Step 2: Fill in the group details (အဆင့် ၂: အဖွဲ့အသေးစိတ်အချက်အလက်များ ဖြည့်သွင်းခြင်း)

ဤနေရာတွင်၊ ပထမအဖွဲ့နှင့် ပတ်သက်သော အောက်ပါ အသေးစိတ်အချက်အလက်များကို ထည့်သွင်းသင့်သည်။

- အဖွဲ့၏ အမည်မှာ "SSPR_Enabled" ဖြစ်သည်။
- သင့်လျော်သော ဖော်ပြချက်။
- အခန်းကဏ္ဍများသည် _Unassigned_ အဖြစ် ကျန်ရှိနေသည်။
- _Membership type_ ကို _Assigned_ သို့ ပြောင်းထားသည်။
- အဖွဲ့သို့ နမူနာအသုံးပြုသူတစ်ဦးကို သတ်မှတ်ထားသည်။  
  _SSPR အဖွဲ့အသစ် စခရင်မှ အဖွဲ့အသေးစိတ်အချက်အလက်များ ဖြည့်သွင်းခြင်း_

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/o_llCnngSTSeX7_Upx37_g_b46bad958ec94799b9af5268fe4394e1_C4M2L3_Itm6_Img2.png?expiry=1743033600000&hmac=4M3VRFIx0C46xMR71xGAac7o1ofy-tiHNrseatVn2pQ">

## Step 3: Enable SSPR (အဆင့် ၃: SSPR ဖွင့်ခြင်း)

ဤအဆင့်တွင်၊ _Overview_ မီနူးမှ _Password reset_ တဘ်သို့ သွားခြင်းဖြင့် SSPR ကို ဖွင့်ထားသည်။  
ထို့နောက် _Selected_ ဟု ခေါ်သော ရွေးချယ်မှုအတွက် ဖွင့်/ပိတ် ခလုတ်ကို ရွေးချယ်သင့်သည်။  
"SSPR*Enabled Group" ကို ထည့်သွင်းပြီး၊ ထို့နောက် \_Save* ခလုတ်ကို ရွေးချယ်ပါ။  
*ကိုယ်တိုင်ဝန်ဆောင်မှု စကားဝှက်ပြန်လည်သတ်မှတ်ခြင်းကို *Selected* ဆက်တင်သို့ ဖွင့်ထားခြင်း*

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/3GOytR4-R1WHmbnCvIA7vA_013a2d598c3c419fbfd830f5a86c6ee1_C4M2L3_Itm6_Img3.png?expiry=1743033600000&hmac=XvgX_AWAFN5TDedIlAHqrX5s46_ECXrOerJ18eNnv_M">

## Step 4: Register a user (အဆင့် ၄: အသုံးပြုသူတစ်ဦးကို မှတ်ပုံတင်ခြင်း)

သင်သည် အသုံးပြုသူသည် SSPR ကို ဝင်ရောက်၍မရသည်ကို အတည်ပြုခဲ့သည်။  
ထို့ကြောင့် အပလီကေးရှင်း ဝက်ဘ်ဆိုက်သို့ သွားပြီး ဆိုက်ပေါ်တွင် အသုံးပြုသူတစ်ဦးကို မှတ်ပုံတင်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/QoA6CLinS5SNgVD4nQuOcQ_1f0b6c75dfe5422f8837622969ab88e1_C4M2L3_Itm6_Img4.png?expiry=1743033600000&hmac=tMZrAOpe09-4LK5ytIKtVvpBd4nSwm0XIKEuD9fFq7A">

## Step 5: Verify user access to Password reset (အဆင့် ၅: စကားဝှက်ပြန်လည်သတ်မှတ်ခြင်းသို့ အသုံးပြုသူ၏ ဝင်ရောက်ခွင့်ကို အတည်ပြုခြင်း)

SSPR ပေါ်တယ်သို့ ဝင်ရောက်ပါ။ စမ်းသပ်မှု ပြီးမြောက်ပြီး အသုံးပြုသူသည် _Password reset_ ကို ဝင်ရောက်နိုင်ကြောင်း သရုပ်ပြသည်။  
_အဆင့် ၁ အတည်ပြုခြင်းတွင် အကောင့်သို့ ပြန်ဝင်ရန် မိုဘိုင်းရွေးချယ်မှုဖြင့် စာသား_

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/QoA6CLinS5SNgVD4nQuOcQ_1f0b6c75dfe5422f8837622969ab88e1_C4M2L3_Itm6_Img4.png?expiry=1743033600000&hmac=tMZrAOpe09-4LK5ytIKtVvpBd4nSwm0XIKEuD9fFq7A">

## Step 6: Create the second group (အဆင့် ၆: ဒုတိယအဖွဲ့ကို ဖန်တီးခြင်း)

ဒုတိယအဖွဲ့ကို ဖန်တီးရာတွင် အဆင့် ၂ နှင့် ၃ ကို ထပ်လုပ်ပါ။  
ဤအဖွဲ့ကို "SSPR*not_Enabled" ဟု အမည်ပေးထားသည်။  
ဤနေရာတွင် SSPR ကို ပြင်ဆင်သတ်မှတ်မထားပါ။  
အဖွဲ့ဝင်တစ်ဦးကို သတ်မှတ်ပေးထားသည်။  
\_SSPR ကို ထိုအဖွဲ့အတွက် ဖွင့်မထားသည့် အဖွဲ့စခရင်*

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Scm0QWylQoqpciCjZ4hjAg_80d0f3810bf34f09b3f1a98ed046e3e1_C4M2L3_Itm6_Img5.png?expiry=1743033600000&hmac=1Fmg1pkIh8Oj1VdmT6VD8WzwgDt1IamWqnXY2CwnXp4">

## Step 7: Demonstrate non-SSPR availability (အဆင့် ၇: SSPR မရရှိနိုင်မှုကို သရုပ်ပြခြင်း)

ပုံသည် "SSPR*not_Enabled" အဖွဲ့မှ အဖွဲ့ဝင်တစ်ဦးသည် SSPR လုပ်ဆောင်ချက်ကို ဖွင့်ရန် ကြိုးစားသော်လည်း မအောင်မြင်ကြောင်း အတည်ပြုသည်။  
\_SSPR ဖွင့်မထားသည့်ကြောင့် အကောင့်ဝင်ရောက်မှု ငြင်းပယ်ခံရခြင်း*

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/7Zu4O6ZnTvStPDUZPfl5OQ_c28c19adcd464943a7a57c9cd974b7e1_C4M2L3_Itm6_Img6.png?expiry=1743033600000&hmac=CLxnNf7ISsoA_OEIVJEbtvuSCunF0N79gWugILSZ1Zg">

## Conclusion (နိဂုံးချုပ်)

ဤလေ့ကျင့်ခန်းတွင်၊ အဖွဲ့များကို SSPR နှင့် ပေါင်းစပ်၍ အလုပ်သမား၏ အတိုင်းအတာကို ကန့်သတ်နိုင်ပုံကို သင်သရုပ်ပြခဲ့သည်။ သင်သည် အဖွဲ့နှစ်ဖွဲ့ ဖန်တီးခဲ့ပြီး၊ ပထမအဖွဲ့သည် SSPR ကို အသုံးပြု၍ စနစ်သို့ ဝင်ရောက်ခဲ့ပြီး၊ ဒုတိယအဖွဲ့သည် SSPR မရှိပါ။ ယင်းအစား၊ သင်၊ အက်မင်အနေဖြင့် "SSPR_not_Enabled" အဖွဲ့သို့ ဝင်ရောက်ခွင့် အခွင့်အာဏာများကို ကူညီဆောင်ရွက်ပေးရမည်။
