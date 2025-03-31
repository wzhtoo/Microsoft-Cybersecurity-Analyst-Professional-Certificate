# Exemplar: Set up a SSO in the free Azure portal

[Exemplar: Set up a SSO in the free Azure portal 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/supplement/UHAEo/exemplar-set-up-a-sso-in-the-free-azure-portal)

## Exemplar: Set Up SSO in the Free Azure Portal (နမူနာ- Azure အခမဲ့ပေါ်တယ်တွင် SSO ထည့်သွင်းခြင်း)

### Overview (ခြုံငုံသုံးသပ်ချက်)

ယခင်လေ့ကျင့်ခန်းတွင်၊ သင်သည် Sam’s Scoops ၏ Azure Active Directory ကို SAML Toolkit ဟုခေါ်သော နမူနာအက်ပ်လီကေးရှင်းတစ်ခုနှင့် ပြင်ဆင်သတ်မှတ်ရန် တာဝန်ပေးအပ်ခံခဲ့ရသည်။ ထို့နောက်၊ ဤအက်ပ်လီကေးရှင်းကို Single Sign-On (SSO) အတွက် ပြင်ဆင်သတ်မှတ်ရန် တောင်းဆိုခံခဲ့ရပြီး၊ ၎င်းကို အသုံးပြုသူ အသေးစိတ်အချက်များကို ပြန်လည်ထည့်သွင်းရန်မလိုဘဲ ဝင်ရောက်နိုင်ရန် ပြုလုပ်ခဲ့သည်။ ဤနေရာတွင်၊ ဖော်မတ်သည် အဆင့်တစ်ခုစီကို ထောက်ပံ့ပေးထားသော မျက်နှာပြင်ဓာတ်ပုံ (screenshot) နှင့် အဆင့်ဖော်ပြချက် အကျဉ်းချုပ်ဖြင့် ဖော်ပြထားသည်။

အောက်တွင်၊ ဤလေ့ကျင့်ခန်းကို ချဉ်းကပ်ရန် နည်းလမ်းတစ်ခု၏ ရလဒ်ဥပမာကို သင်တွေ့ရပါမည်။

### Exemplar Steps (နမူနာ အဆင့်များ)

#### Create the SAML Toolkit (SAML Toolkit ဖန်တီးခြင်း)

ပထမဦးစွာ၊ သင်၏ Azure ပေါ်တယ်၏ **Overview** အပိုင်းသို့ သွားရောက်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/GdtQKKo5RrCbUThYx3E8pQ_fadfc806a7d14a43b13b194b1da922e1_C4M12L1_Itm09_Img1.png?expiry=1742774400000&hmac=h6cdq9h1go3ueQXwfsHaQRGSOquzTQAqh4EKAjCgVq4">

**Manage** အပိုင်းမှ **Enterprise Applications** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Ble0-S7RSU-HAbvCvjGJuQ_90b88808ffbf43d4a2ab0661df2698e1_C4M12L1_Itm09_Img2.png?expiry=1742774400000&hmac=jelYnJumcPbMBQgKUWpdn9mC1ZGmDGvHOxp5DMKy6m8">

#### Set Up Single Sign-On (Single Sign-On ထည့်သွင်းခြင်း)

**Enterprise Applications** အတွင်း၊ SSO ကို သရုပ်ပြရန် အက်ပ်လီကေးရှင်းသစ်တစ်ခု ဖန်တီးရန် **New Application** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/_i56-HA5T7OJnskLGB9BKg_278cac5921e64d4cbeade19be53902e1_C4M12L1_Itm09_Img3.png?expiry=1742774400000&hmac=QD90hg8giVBPkrKLvwFe6tgrLVyO47B1MBm8HtwgWmE">

Microsoft ၏ **Azure AD SAML Toolkit** ကို ရှာဖွေပါ။ ၎င်းကို ရွေးချယ်ပြီး **Create** ကို နှိပ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/z0kgqAjPRdiwO9k2yqNWiw_aeb93baf130e49ed8e8032151f9034e1_C4M12L1_Itm09_Img4.png?expiry=1742774400000&hmac=pHHPOjHgWlz8-aCPnXgEKQb9SKSLBNwxgyLbzhSwk3c">

#### Create a New User (အသုံးပြုသူသစ်တစ်ဦး ဖန်တီးခြင်း)

အက်ပ်လီကေးရှင်းကို အောင်မြင်စွာ ဖန်တီးပြီးသည်နှင့်၊ သင်၏ Azure AD ပင်မစာမျက်နှာသို့ သွားရောက်ပါ။

**Users** ကို ရွေးချယ်ပါ။

ထို့နောက် **Create New User** ကို ရွေးချယ်ပါ။

အသုံးပြုသူအား သင့်လျော်သော အမည်တစ်ခု ပေးပါ။

သင့်အတွက် အလိုအလျောက် ထုတ်ပေးထားသော စကားဝှက်ကို မှတ်သားထားပါ။

သင်၏ ဆက်တင်များကို ကျေနပ်သည်နှင့် **Create** ကို နှိပ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Wg84xosFRveJvLaXFurYIA_aaa013f629b4489eb2396dfc5d7a89e1_C4M12L1_Itm09_Img5.png?expiry=1742774400000&hmac=eLbJ4mSGOkqETgEJ751wtjgksgzrOQN324TNvQSQyOg">

#### Register a User with the Application (အက်ပ်လီကေးရှင်းတွင် အသုံးပြုသူတစ်ဦးကို မှတ်ပုံတင်ခြင်း)

ဤအသုံးပြုသူအား Azure Overview မှ အက်ပ်လီကေးရှင်းသို့ ဝင်ရောက်ခွင့် ပေးပါ။

**Users and Groups** အပိုင်းတွင်၊ **Add User/Group** ကို ရွေးချယ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/DZlJAUgJRMCKsKx97Q9AZg_267e9d4bd675485bbe3e7b8c54b2bbe1_C4M12L1_Itm09_Img6.png?expiry=1742774400000&hmac=mT9bTnC-uMfXi0ZsFGIkhjM-Ha3Dulx5ZHX5KyR1heE">

SSO ပေးလိုသော အသုံးပြုသူကို ရှာဖွေပါ။ အသုံးပြုသူ၏ အမည်ကို ရွေးချယ်ပြီး၊ **Assign** ခလုတ်ကို နှိပ်ပါ။

ထို့နောက်၊ အက်ပ်လီကေးရှင်း၏ တည်နေရာသို့ သွားရောက်ပါ- `https://samltoolkit.azurewebsites.net/`

**Register** ကို ရွေးချယ်ပြီး SSO အတွက် သင်ပြင်ဆင်ပေးနေသော အသုံးပြုသူနှင့် ဆက်စပ်နေသော အီးမေးလ်လိပ်စာကို ထည့်သွင်းပါ။ အသုံးပြုမည့် စကားဝှက်သည် သင်္ကေတတစ်ခု၊ စာလုံးသေး၊ နှင့် စာလုံးကြီးများ ပေါင်းစပ်ထားရမည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/EDmG3BeIQ62HKrTya6cC2g_02b3488779f04e19bd27b5faa13287e1_C4M12L1_Itm09_Img7.png?expiry=1742774400000&hmac=3i3EK_HGhBkkDis8D4tCMcSL5dyUewrIaoSr92lvX48">

အောင်မြင်စွာ မှတ်ပုံတင်ပြီးသည်နှင့်၊ သင်သည် ပင်မစာမျက်နှာသို့ ပြန်လည်ညွှန်းခံရမည်ဖြစ်သည်။

**SAML Configuration** သို့ သွားရောက်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/XPvVY4jwSTmNrdsHuKzIAg_daa55392137a4ad488e32c85b1bf6ce1_C4M12L1_Itm09_Img8.png?expiry=1742774400000&hmac=W9vQ8B4squFxm3Y8SBejw5otmUzn2NoUrVZO5pFMAcE">

#### Configure SAML (SAML ပြင်ဆင်သတ်မှတ်ခြင်း)

သင်၏ အက်ပ်လီကေးရှင်းကို ပြင်ဆင်သတ်မှတ်ရန် **Create** ရွေးချယ်မှုကို နှိပ်ပါ။ သင့်အက်ပ်လီကေးရှင်းကို ပြင်ဆင်သတ်မှတ်ရန် အချက်လေးခုကို ထည့်သွင်းရန် အခွင့်အရေး ပေးထားပါသည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/F2QtlbH3R0m_bxaXgLWIrA_8d36bdeb261542d587db564b180547e1_C4M12L1_Itm09_Img9.png?expiry=1742774400000&hmac=CXhKQUaRAn1q9s8YK1fbRgw2KPDw5jyN6zTZVql8BOU">

**Enterprise Applications** စာမျက်နှာသို့ ပြန်သွားပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/lEboLl00S52ZYEKgKqcrsQ_8966da840b3d4230b3337cbffba7d4e1_C4M12L1_Itm09_Img11.png?expiry=1742774400000&hmac=uMgwmn6bkMydB4RCpO5QOeIf8XrFQoG987GX10QLIss">

**Set Up Single Sign-On** ကို ရွေးချယ်ပါ။

![Set up single sign on tab](setup_sso_tab.png)

#### Update Azure AD Configuration (Azure AD ပြင်ဆင်သတ်မှတ်မှုကို အဆင့်မြှင့်တင်ခြင်း)

**SAML** ရွေးချယ်မှုကို ရွေးပါ။

**Basic SAML Configuration** အောက်တွင် **Edit** ကို နှိပ်ပါ။

ဤအပိုင်းအတွင်း ပြင်ဆင်သတ်မှတ်ရန် အချက်သုံးခု ရှိပါသည်-

- **Identifier (Entity ID)**: အကယ်၍ ၎င်းကို သတ်မှတ်မထားပါက `"https://samltoolkit.azurewebsites.net"` ကို ရိုက်ထည့်ပါ။
- **Reply URL**: `"https://samltoolkit.azurewebsites.net/SAML/Consume"` ကို ရိုက်ထည့်ပါ။
- **Sign on URL**: `"https://samltoolkit.azurewebsites.net/"` ကို ရိုက်ထည့်ပါ။

ထို့နောက် **Save** ကို နှိပ်ပါ။

**SAML Certificate** ဒေါင်းလုဒ်အတွင်း၊ စစ်မှန်သော လက်မှတ် (raw certificate) တစ်ခု ရှိပါသည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/xgnQxPyoS96ROn4FJ8hcJQ_64d9b6fee3cd49ef9e50569b422b17e1_C4M12L1_Itm09_Img12.png?expiry=1742774400000&hmac=l-HyPiw0tTlNlJtjA6ApPnNET5KfmVmInatEe5UVAV0">

**URL Identifiers for Azure AD SAML Toolkit setup** ကို ကြည့်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/m7CQhh-iRD-NFN92b3rWTw_f1599e06e62d4c9a85a3972ecac9f0e1_C4M12L1_Itm09_Img13.png?expiry=1742774400000&hmac=HDhRdbIO0UIzci7_Eaxc9fX6wsHADCZzztPDp1_Qm-k">

Azure AD SAML Toolkit ၏ ပြင်ဆင်သတ်မှတ်မှုသို့ ပြန်သွားပြီး၊ ကူးယူထားသော **Login URL**၊ **Azure AD Identifier**၊ နှင့် **Logout URL** တို့ကို အက်ပ်လီကေးရှင်း၏ ဆက်တင်များတွင် ထည့်သွင်းပါ။

ထို့ပြင်၊ အဆင့် ၅ တွင် ဒေါင်းလုဒ်လုပ်ထားသော စစ်မှန်သော လက်မှတ်ကို အပ်လုဒ်လုပ်ပြီး **Create** ကို နှိပ်ပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/eEoiC0_9Tuy_Agb9z-Gb5Q_2a387091aa1b4383b7a2dee342e70ee1_C4M12L1_Itm09_Img14.png?expiry=1742774400000&hmac=Bx263ecY6S3qM3sWbwHiINgwak28NkoY8z6S6NcJ3aA">

၎င်းသည် SAML 2.0 Single Sign-On Configuration လက်မှတ်တစ်ခု ဖန်တီးပေးပါလိမ့်မည်။

**Details** ကို နှိပ်ပြီး **Azure ID Identifier** ကို ထုတ်ယူပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/z_3Oo1drTl6eUCbKI7aSGw_025471951322437689e23d015c1047e1_C4M12L1_Itm09_Img15.png?expiry=1742774400000&hmac=vvSgoAngUhHpqv7b8YTs2KEy4cFo_q9VwnqYlKfbeiM">

Azure AD ပေါ်တယ်ရှိ SAML Toolkit ၏ **Basic SAML Configuration** ကို **Azure ID Identifier** ဖြင့် အဆင့်မြှင့်တင်ပါ။

ထို့ပြင်၊ **SP Initiated Login URL** မှ URL ကို ထုတ်ယူပါ။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/vzq3HLJRQYmXKo2eML3r6g_60dda2793da84263b14b185cf9dcbbe1_C4M12L1_Itm09_Img16.png?expiry=1742774400000&hmac=Ph_NcJTSzgCVHYdrXv8ZRNW6JaDi-ZiQ1EbnLBZTZU0">

**Sign On URL** နှင့် **Relay State** ကို အဆင့်မြှင့်တင်ပါ။

#### Test Your Implementation (သင်၏ အကောင်အထည်ဖော်မှုကို စမ်းသပ်ခြင်း)

သင်၏ ပြင်ဆင်သတ်မှတ်မှုကို စမ်းသပ်ရန် အခွင့်အရေးပေးသော ပေါ်လာသော ဝင်းဒိုးတစ်ခု ထွက်ပေါ်လာပါလိမ့်မည်။ ဆက်လက်၍ စမ်းသပ်ပါ။

အောင်မြင်သော စမ်းသပ်မှုတစ်ခုသည် သင့်ဝင်ရောက်မှု အသေးစိတ်အချက်များကို ထည့်သွင်းရန်မလိုဘဲ ဝင်ရောက်ခွင့်ပြုပါလိမ့်မည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/6Y0A94j8TOuKr9hGpW6sqQ_dbb0a96a8c424c74863a9fd0d14877e1_C4M12L1_Itm09_Img17.png?expiry=1742774400000&hmac=n4vx3jAqATSezWLxHdTLqyFHpTt4h1NK95Fb2xfYhsg">

### Conclusion (နိဂုံး)

ဤဖတ်ရှုမှုတွင်၊ သင်သည် Sam’s Scoops ၏ Azure Active Directory ကို SAML Toolkit ဖြင့် မည်သို့ပြင်ဆင်သတ်မှတ်ရမည်ကို ဥပမာတစ်ခု ကြည့်ရှုခဲ့သည်။ ထို့နောက်၊ ဤအက်ပ်လီကေးရှင်းကို SSO လုပ်ဆောင်နိုင်မှုမှတစ်ဆင့် အသုံးပြုသူ အသေးစိတ်အချက်များကို ပြန်လည်ထည့်သွင်းရန်မလိုဘဲ ဝင်ရောက်နိုင်ရန် ပြင်ဆင်သတ်မှတ်ခဲ့သည်။
