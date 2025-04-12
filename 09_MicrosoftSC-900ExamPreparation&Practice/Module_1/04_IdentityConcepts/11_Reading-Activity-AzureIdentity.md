# Activity: Azure Identity

[Activity: Azure Identity 🔗](https://www.coursera.org/learn/microsoft-sc-900-exam-preparation-and-practice/supplement/enlas/activity-azure-identity)

# Activity: Azure Identity (လှုပ်ရှားမှု- Azure အထောက်အထား)

## Introduction (နိဒါန်း)

ဤလှုပ်ရှားမှုတွင်၊ Azure AD B2C ကို အသုံးပြု၍ ပြင်ပ အထောက်အထားတစ်ခု ဖန်တီးခြင်း လုပ်ငန်းစဉ်ကို လိုက်နာခြင်းဖြင့် အထောက်အထားဆိုင်ရာ သင့်နားလည်မှုကို တိုးချဲ့ပါမည်။ ဤဝန်ဆောင်မှုသည် Azure AD ၏ တည်ဆောက်ပုံနှင့် လုပ်ဆောင်နိုင်စွမ်းကို ထင်ဟပ်စေပြီး ၎င်းသည် ဖောက်သည်နှင့် ဆက်သွယ်ရသောကြောင့် ဖြစ်သည်။ အခြားနည်းအားဖြင့်၊ ဆက်စပ်အင်္ဂါရပ်များကို စီးပွားရေးတစ်ခုသည် ထုတ်ကုန် သို့မဟုတ် ဝန်ဆောင်မှုတစ်ခုနှင့် ဖောက်သည် မည်သို့ အပြန်အလှန် တုံ့ပြန်နိုင်သည်ကို ထိန်းချုပ်နိုင်စေရန် စီစဉ်ထားပါသည်။

## Authentication in Azure AD B2C (Azure AD B2C တွင် စစ်မှန်ကြောင်း အတည်ပြုခြင်း)

ယခု သင်သည် စစ်မှန်ကြောင်း အတည်ပြုခြင်းသည် အသုံးပြုသူ သို့မဟုတ် အရာဝတ္ထုတစ်ခု၏ အထောက်အထားကို အတည်ပြုခြင်း လုပ်ငန်းစဉ်ဖြစ်ကြောင်း သိရှိပြီဖြစ်သည်။ Azure AD B2C သည် အမျိုးမျိုးသော စစ်မှန်ကြောင်း အတည်ပြုခြင်း ရွေးချယ်စရာများကို ပေးဆောင်ပါသည်။ ၎င်းတို့တွင် Google နှင့် Facebook ကဲ့သို့သော လူမှုရေး အထောက်အထား ပံ့ပိုးပေးသူများသာမက ဒေသဆိုင်ရာ အကောင့်များနှင့် SAML ကဲ့သို့သော ပရိုတိုကောများကို အသုံးပြု၍ စိတ်ကြိုက် အထောက်အထား ပံ့ပိုးပေးသူများလည်း ပါဝင်ပါသည်။ တစ်ကြိမ်တည်း ဝင်ရောက်ခြင်း (SSO) သည် ဖောက်သည်များအား ထပ်ခါထပ်ခါ ဝင်ရောက်ခြင်းမရှိဘဲ အပလီကေးရှင်း အများအပြားကို ဝင်ရောက်ခွင့်ပေးခြင်းဖြင့် အသုံးပြုသူ အတွေ့အကြုံကို မည်သို့ တိုးတက်စေနိုင်ကြောင်းလည်း သင်သိရှိပြီဖြစ်သည်။

## Authorization in Azure AD B2C (Azure AD B2C တွင် ခွင့်ပြုချက် ပေးခြင်း)

ထို့နောက် သင်သည် စစ်မှန်ကြောင်း အတည်ပြုပြီးနောက် အပလီကေးရှင်းတစ်ခုအတွင်း အသုံးပြုသူ၏ လုပ်ဆောင်ချက်များကို ဆုံးဖြတ်ပေးသည့် ခွင့်ပြုချက် ပေးခြင်းကို လေ့လာခဲ့သည်။ သင်သည် အခန်းကဏ္ဍများနှင့် တာဝန်များအပေါ် အခြေခံ၍ မတူညီသော အသုံးပြုသူများအား မှန်ကန်သော ဝင်ရောက်ခွင့် အဆင့်ကို ပေးအပ်ခြင်း၏ အရေးပါမှုကို အလေးပေး၍ အနည်းဆုံး ခွင့်ပြုချက်ရ ဝင်ရောက်ခွင့်၊ အခြေအနေအရ ဝင်ရောက်ခွင့်နှင့် သုည-ယုံကြည်မှု အယူအဆများကို လေ့လာခဲ့သည်။

ပြင်ပ အထောက်အထားများကို သိမ်းဆည်းနိုင်သည့် Azure AD B2C ငှားရမ်းသူ ဖန်တီးခြင်း၏ လက်တွေ့ အစိတ်အပိုင်းကို လေ့လာကြပါစို့။

## Steps to configure Azure AD B2C (Azure AD B2C ဖွဲ့စည်းရန် အဆင့်များ)

1.  သင်၏ Azure Portal သို့ ဝင်ရောက်ပါ။
2.  သင်၏ Azure AD B2C ငှားရမ်းသူကို ချိတ်ဆက်ခြင်းမပြုမီ သင်သည် ငှားရမ်းသူ ၂၀ သာ ဖန်တီးနိုင်ကြောင်း သတိပြုသင့်သည်။ B2C အင်္ဂါရပ်သည် သီးခြား အခန်းကဏ္ဍ အဆင့်များအတွက်သာ ရရှိနိုင်ပါသည်။ ဤအင်္ဂါရပ်ကို ဝင်ရောက်ရန် သင်အသုံးပြုနိုင်သည့် အနိမ့်ဆုံး အခန်းကဏ္ဍမှာ Contributor အခန်းကဏ္ဍ ဖြစ်ပါသည်။ ဤအောက်ရှိ မည်သည့် အခန်းကဏ္ဍမဆို သင့်လျော်သော ခွင့်ပြုချက်များ ရှိမည် မဟုတ်ပါ။
3.  အောက်ပါ ဖန်သားပြင်ဓာတ်ပုံတွင် ပြထားသည့်အတိုင်း ဂီယာ အိုင်ကွန်ကို ရွေးချယ်ခြင်းဖြင့် Portal ဆက်တင်များကို ဝင်ရောက်ပါ။
    (မှတ်ချက်- ပုံများကို ပြသ၍ မရသောကြောင့် ဂီယာ အိုင်ကွန်အတွက် Azure Portal UI ကို ကိုးကားပါ)

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/jWrBD8J9QEOrfxg-mYgMFg_d01559dfa2334510a3938613a48034e1_MSCSA_C9M1L4_Item-10_img1.PNG?expiry=1744502400000&hmac=cYMSCfvbTtx0JIwLHfhxmjCK2gvCw6vDHnFcO7slOYk">

4.  ရှာဖွေရေးဘားတွင် ဝန်ဆောင်မှုများ ကဏ္ဍမှ **Subscriptions** ကို ရှာဖွေပြီး ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/tAtQ29q3Sq2lfRmpBzRyhg_96a49e546fe346beb2d14e0b733108e1_MSCSA_C9M1L4_Item-10_img2.PNG?expiry=1744502400000&hmac=_IOq80tsbjLczR4h24ZFJTqS2v24JoBciuvIoBhKoNk">

5.  ထိုမှ ဘယ်ဘက်အကန့်တွင် **Resource Providers** ကို ရွေးချယ်ပြီး **Microsoft.AzureActiveDirectory** ကို ရှာဖွေပါ။ အခြေအနေကို မှတ်ပုံတင်ထားကြောင်း သေချာပါစေ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/nnO16ujfSyGCrN6xAH1P4A_dd01a544dc9b42238a4680c83e79c2e1_MSCSA_C9M1L4_Item-10_img3.PNG?expiry=1744502400000&hmac=xYngMT-KaBJ-E-WiUvxrNFFuUlb-P6MqWF_cNa3-8xQ">

6.  Azure Active Directory ကို မှတ်ပုံတင်ပြီးနောက် ပင်မ မီနူးသို့ ပြန်သွားပြီး ဘယ်ဘက်အပေါ်ထောင့်ရှိ **Create a resource** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/yLbxqY6PQTKudNvaZNoF5A_144af86ec551483bb530a33c586941e1_MSCSA_C9M1L4_Item-10_img04_V2.PNG?expiry=1744502400000&hmac=FS8zDgOkWZsX9s3Ur9mu0bkQBfSXQkZUWL66g46ihak">

7.  နောက်စာမျက်နှာတွင် **Azure Active Directory B2C** သို့ သွားပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/zh9kAfu4Sza0wYBwx_i8Fg_62de6be70d524610bfd2bcfafe700fe1_MSCSA_C9M1L4_Item-10_img05_V2.PNG?expiry=1744502400000&hmac=0xe2dYwK-XDFDXNW9WsEaQr2UXBNSRVhROPugs1dzmw">

8.  နောက်မျက်နှာပြင်မှ **Create** ကို ရွေးချယ်ပါ။
    <img src = "https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/uY5lg6vTR9mKJ54692m7YQ_54ff71f67d504838a61a3c9100a753e1_MSCSA_C9M1L4_Item-10_img06_V2.PNG?expiry=1744502400000&hmac=4eTBI39VUdiCfttaWgaIVKRBWEB8lQdNqkjWhqlPIHk">

9.  နောက်တွင် ငှားရမ်းသူကို ဖန်တီးခြင်း သို့မဟုတ် ချိတ်ဆက်ခြင်း၏ ရွေးချယ်မှုကို သင်အား ပေးပါလိမ့်မည်။ **Create new tenant** ကို ရွေးချယ်ခြင်းဖြင့် အသစ်တစ်ခုကို ဖန်တီးပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/EGgRSffiRB2uGJG72VaypQ_3bd8414520364645920344e70a7795e1_MSCSA_C9M1L4_Item-10_img07_V2.PNG?expiry=1744502400000&hmac=JA9NJQYSq-ojWeyDqs6v0Jl0s8-80vuXauYo_iW8g-k">

10. တောင်းဆိုထားသော သတင်းအချက်အလက်ကို ဖြည့်ပါ။
    - “Customer Organization” ကို ထည့်ပါ။
    - “SamsScoopsCustomerOrg” ကို ရိုက်ထည့်ပါ။
    - United States ကို ရွေးချယ်ပါ။
    - သင်၏ စာရင်းသွင်းမှုကို ရွေးချယ်ပါ။
    - သင်၏ Resource group ကို ရွေးချယ်ပါ။
    - သင့်လျော်သော တည်နေရာကို ခွဲဝေပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/rGE93qkPTGWlMU2jtqonig_d776a55330a94e1ea1f6166fe360e7e1_MSCSA_C9M1L4_Item-10_img08_V2.PNG?expiry=1744502400000&hmac=Gp9WMydn_8TI3iEu_tNrzyFPy6EOwZW0S5KlxpAn0Yg">

11. ထို့နောက် **Review + create** ကို ရွေးချယ်ပါ။ သင်သည် ငှားရမ်းသူကို အောင်မြင်စွာ ဖန်တီးကြောင်း ညွှန်ပြသည့် “validation passed” ဟု ပြောသော အကြောင်းကြားချက်ကို ရရှိသင့်ပါသည်။
12. နောက်ဆုံးတွင် အောက်ပါ မျက်နှာပြင်ကို သင်အား တင်ပြသင့်ပါသည်။
    (မှတ်ချက်- ပုံများကို ပြသ၍ မရသောကြောင့် အတည်ပြုခြင်း မျက်နှာပြင်အတွက် Azure Portal UI ကို ကိုးကားပါ)

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/kJktfeAAQYSPPsuFkYDF2w_09c935806f0a4cc089d2713acce422e1_MSCSA_C9M1L4_Item-10_img11.PNG?expiry=1744502400000&hmac=TA7ses5azPEaHM9jFVW9VBeUhTfhQkZcBfrZ5zdo6iw">

## Conclusion (နိဂုံး)

ဤလှုပ်ရှားမှုတွင် သင်သည် ပြင်ပ အထောက်အထားများကို ပေါင်းစည်းနိုင်စေသည့် Azure AD ဖြင့် သင်၏ Azure AD B2C ကို ဖွဲ့စည်းပြီး ဖြစ်ပါသည်။
