# Exercise: Configure identity and access policies

[Exercise: Configure identity and access policies 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/supplement/ArDqa/exercise-configure-identity-and-access-policies)

## Exercise: Configure Identity and Access Policies (လေ့ကျင့်ခန်း- အထောက်အထားနှင့် ဝင်ရောက်ခွင့် မူဝါဒများ ဖွဲ့စည်းပုံပြင်ဆင်ခြင်း)

### Introduction (မိတ်ဆက်)

ဤလေ့ကျင့်ခန်းတွင်၊ သင်သည် ယခုအချိန်အထိ သင်ယူခဲ့သော ကျွမ်းကျင်မှုအားလုံးကို အသုံးပြု၍ Microsoft Entra ID တွင် အလုပ်လုပ်နိုင်သော အခြေခံအဆောက်အအုံတစ်ခု စီစဉ်သတ်မှတ်ရမည်။ ကုမ္ပဏီတစ်ခု၏ အုပ်ချုပ်သူတစ်ဦးအနေဖြင့်၊ သင်၏ တာဝန်မှာ တူညီသော အခန်းကဏ္ဍများရှိသော အသုံးပြုသူများကို စုစည်းထားသည့် ညီညွတ်သော အထောက်အထား ဖွဲ့စည်းပုံတစ်ခု ဖန်တီးရန်ဖြစ်သည်။ ထို့နောက် ၎င်းတို့ကို သတ်မှတ်ထားသော အုပ်ချုပ်ရေး အသုံးပြုသူတစ်ဦးထံ သတ်မှတ်ပေးရမည်။

### Objective (ရည်မှန်းချက်)

ဤတာဝန်ကို အောင်မြင်ရန်၊ သင်သည် အသုံးပြုသူတစ်ဦး ဖန်တီးရမည်၊ အထူး အုပ်စုတစ်ခု စီစဉ်သတ်မှတ်ရမည်၊ ကိုယ်တိုင်ဝန်ဆောင်မှု စကားဝှက် ပြန်လည်သတ်မှတ်ခြင်း (SSPR) ကို ဖြစ်နိုင်စေရမည်၊ အခန်းကဏ္ဍတစ်ခု သတ်မှတ်ပေးရမည်၊ နှင့် စကားဝှက် အခန်းကဏ္ဍများ သတ်မှတ်ပေးထားသော အုပ်ချုပ်ရေး အုပ်စုတစ်ခု ဖန်တီးရမည်ဖြစ်ပြီး၊ ၎င်းကို အသုံးပြုသူသစ်ထံ သတ်မှတ်ပေးရမည်။ ၎င်းသည် Microsoft Entra ID နှင့် ၎င်း၏ မရှိမဖြစ် အစိတ်အပိုင်းများကို သင်၏ နားလည်မှုကို အားဖြည့်ပေးမည်ဖြစ်သည်။

### Step 1: Create a User (အဆင့် ၁- အသုံးပြုသူတစ်ဦး ဖန်တီးခြင်း)

Azure ပေါ်တယ် (https://portal.azure.com/) သို့ ဝင်ရောက်ပြီး ခြုံငုံသုံးသပ်ချက် (Overview) အပိုင်းသို့ သွားပါ။

မျက်နှာပြင် အောက်ခြေရှိ အမြန် လုပ်ဆောင်ချက် (Quick Actions) မီနူးတွင်၊ အသုံးပြုသူ ထည့်သွင်းခြင်း (Add User) ကို ရွေးချယ်ပါ။

အသုံးပြုသူ ဖန်တီးခြင်း (Create User) ကို ရွေးချယ်ပြီး အထောက်အထား အသေးစိတ်အချက်အလက်များကို ဖြည့်စွက်ပါ။

Microsoft Entra ID မှ စကားဝှက်ကို အလိုအလျောက် ဖန်တီးစေရန် ခွင့်ပြုပါ သို့မဟုတ် စကားဝှက်ကို ကိုယ်တိုင် သတ်မှတ်ပါ။

ရွေးချယ်ခွင့်အနေဖြင့်၊ အသုံးပြုသူအတွက် အခန်းကဏ္ဍတစ်ခု ရွေးချယ်ပါ။

ရာထူးနှင့် သက်ဆိုင်သော အလုပ်အချက်အလက်များကို ဖြည့်စွက်ပါ။ ၎င်းတွင် အလုပ်ခေါင်းစဉ် (User Administrator - အသုံးပြုသူ အုပ်ချုပ်သူ)၊ ဌာန (IT Department - အိုင်တီ ဌာန)၊ နှင့် ကုမ္ပဏီအမည် (Sam's Scoops) တို့ ပါဝင်သည်။

ယခု၊ အသုံးပြုသူသစ် ပရိုဖိုင်သို့ သွားပြီး ဖန်တီးထားသော အသုံးပြုသူ၏ စခရင်ရှော့ကို ရိုက်ယူပါ။

### Step 2: Create a Group (အဆင့် ၂- အုပ်စုတစ်ခု ဖန်တီးခြင်း)

Azure ပေါ်တယ်ရှိ စီမံခန့်ခွဲမှု (Manage) တက်ဘ်မှ၊ အုပ်စုများ (Groups) ကို ရွေးချယ်ပါ။

အုပ်စုသစ် (New Group) ကို ရွေးချယ်ပြီး ၎င်းကို "End_Project_Group" ဟု အမည်ပေးပါ။

အုပ်စုအတွက် သင့်လျော်သော အသေးစိတ်အချက်အလက်များကို ဖြည့်စွက်ပါ။

### Step 3: Enable SSPR (Self-Service Password Reset) (အဆင့် ၃- SSPR (ကိုယ်တိုင်ဝန်ဆောင်မှု စကားဝှက် ပြန်လည်သတ်မှတ်ခြင်း) ဖြစ်နိုင်စေခြင်း)

Microsoft Entra ID ခြုံငုံသုံးသပ်ချက် (Overview) မီနူးရှိ စကားဝှက် ပြန်လည်သတ်မှတ်ခြင်း (Password Reset) တက်ဘ်သို့ ဝင်ရောက်ပါ။

SSPR ကို ဖြစ်နိုင်စေရန်၊ ရွေးချယ်ထားသော (Selected) ရွေးချယ်မှုအတွက် ခလုတ်ကို ရွေးပါ။

End_Project_Group ကို SSPR ဖွဲ့စည်းပုံသို့ ထည့်သွင်းပါ။

ပြောင်းလဲမှုများကို သိမ်းဆည်းပါ။

### Step 4: Assign a Role (အဆင့် ၄- အခန်းကဏ္ဍတစ်ခု သတ်မှတ်ပေးခြင်း)

ဒါရိုက်ထရီအတွက် Privileged Role Administrator (အခွင့်ထူး အခန်းကဏ္ဍ အုပ်ချုပ်သူ) အခန်းကဏ္ဍကို အသုံးပြု၍ Azure ပေါ်တယ်သို့ ဝင်ရောက်ပါ။

Microsoft Entra ID သို့ သွားပြီး၊ ထို့နောက် အသုံးပြုသူများ (Users) ကို ရွေးချယ်ပါ။

အခန်းကဏ္ဍ သတ်မှတ်ပေးမှု လက်ခံရရှိမည့် အသုံးပြုသူကို ရှာဖွေပြီး ၎င်းကို ရွေးချယ်ပါ။

ဘေးဘက် မီနူးမှ၊ သတ်မှတ်ပေးထားသော အခန်းကဏ္ဍများ (Assigned Roles) ကို ရွေးချယ်ပြီး ထို့နောက် တာဝန်ပေးအပ်မှုများ ထည့်သွင်းခြင်း (Add Assignments) ကို ရွေးပါ။

ဒရော့ပ်ဒေါင်း စာရင်းမှ အခန်းကဏ္ဍတစ်ခု ရွေးချယ်ပြီး နောက်တစ်ဆင့် (Next) ကို ရွေးပါ။

### Step 5: Create an Administrative Group and Assign Password Roles (အဆင့် ၅- အုပ်ချုပ်ရေး အုပ်စုတစ်ခု ဖန်တီးပြီး စကားဝှက် အခန်းကဏ္ဍများ သတ်မှတ်ပေးခြင်း)

Azure ပေါ်တယ်သို့ ဝင်ရောက်ပါ။

ထပ်မံ၍ Microsoft Entra ID သို့ သွားပြီး အုပ်ချုပ်ရေး ယူနစ်များ (Administrative Units) ကို ရွေးချယ်ပါ။

အုပ်ချုပ်ရေး ယူနစ်သစ်တစ်ခု ဖန်တီးရန် ထည့်သွင်းခြင်း (Add) ကို ရွေးချယ်ပါ။

အုပ်ချုပ်ရေး ယူနစ်၏ အမည်နှင့် ဖော်ပြချက်ကို ထည့်သွင်းပါ။

ရွေးချယ်ခွင့်အနေဖြင့်၊ အခန်းကဏ္ဍများ သတ်မှတ်ပေးပြီး ဤအုပ်ချုပ်ရေး ယူနစ် အတိုင်းအတာအတွင်း အခန်းကဏ္ဍများ သတ်မှတ်ပေးမည့် အသုံးပြုသူများကို ရွေးချယ်ပါ။

အုပ်ချုပ်ရေး ယူနစ်နှင့် မည်သည့် အခန်းကဏ္ဍ သတ်မှတ်ပေးမှုများကို ပြန်လည်သုံးသပ်ပါ။

နောက်ဆုံးတွင်၊ စီစဉ်သတ်မှတ်မှုကို အပြီးသတ်ရန် ဖန်တီးခြင်း (Create) ကို ရွေးချယ်ပါ။

### Step 6: Add a Group to the Administrative Unit (အဆင့် ၆- အုပ်စုတစ်ခုကို အုပ်ချုပ်ရေး ယူနစ်သို့ ထည့်သွင်းခြင်း)

1. စီမံခန့်ခွဲမှု (Manage) တက်ဘ်သို့ သွားပြီး၊ အုပ်ချုပ်ရေး ယူနစ်များ (Administrative Units) ကို ရွေးချယ်ပါ။
2. အသစ်ဖန်တီးထားသော အုပ်ချုပ်ရေး ယူနစ်ကို ရွေးချယ်ပါ။
3. ဘေးဘက် မီနူးဘားမှ အုပ်စုများ (Groups) ကို ရွေးချယ်ပါ။
4. ထည့်သွင်းခြင်း (Add) ကို ရွေးချယ်ပြီး End_Project_Group ကို ဆက်လက် ထည့်သွင်းပါ။

### Conclusion (နိဂုံးချုပ်)

ဤလေ့ကျင့်ခန်းတွင်၊ သင်သည် Microsoft Entra ID တွင် အလုပ်လုပ်နိုင်သော အခြေခံအဆောက်အအုံတစ်ခု စီစဉ်သတ်မှတ်ခြင်းဖြင့် Azure အထောက်အထားဆိုင်ရာ သင်၏ အသိပညာကို စုစည်းခဲ့သည်။ သင်သည် အသုံးပြုသူတစ်ဦး ဖန်တီးခဲ့သည်၊ အထူး အုပ်စုတစ်ခု ဖွဲ့စည်းပုံပြင်ဆင်ခဲ့သည်၊ SSPR ကို ဖြစ်နိုင်စေခဲ့သည်၊ အခန်းကဏ္ဍတစ်ခု သတ်မှတ်ပေးခဲ့သည်၊ နှင့် စကားဝှက် အခန်းကဏ္ဍများ ပါဝင်သော အုပ်ချုပ်ရေး အုပ်စုတစ်ခု ဖန်တီးခဲ့သည်။ သင်သည် Microsoft Entra ID ၏ အရေးပါသော အစိတ်အပိုင်းများကို အကောင်အထည်ဖော်ရာတွင် လက်တွေ့ အတွေ့အကြုံကို ရရှိခဲ့သည်။
