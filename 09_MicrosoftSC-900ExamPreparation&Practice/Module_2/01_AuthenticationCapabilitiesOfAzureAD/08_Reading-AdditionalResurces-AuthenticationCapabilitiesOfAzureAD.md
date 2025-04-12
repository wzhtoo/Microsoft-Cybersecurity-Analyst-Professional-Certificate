# Additional resources: Authentication capabilities of Azure AD

[Additional resources: Authentication capabilities of Azure AD 🔗](https://www.coursera.org/learn/microsoft-sc-900-exam-preparation-and-practice/supplement/Qnq4d/additional-resources-authentication-capabilities-of-azure-ad)

# Additional Resources: Authentication Capabilities of Azure AD (နောက်ထပ် အရင်းအမြစ်များ- Azure AD ၏ အတည်ပြုခြင်း စွမ်းရည်များ)

အသုံးပြုသူသည် စက်ပစ္စည်း၊ အပလီကေးရှင်း သို့မဟုတ် ဝန်ဆောင်မှုတစ်ခုသို့ ဝင်ရောက်သည့်အခါ အထောက်အထားများကို အတည်ပြုခြင်း သို့မဟုတ် အတည်ပြုခြင်းသည် အိုင်ဒင်တီတီ ပလက်ဖောင်း၏ အဓိက အင်္ဂါရပ်များထဲမှ တစ်ခုဖြစ်သည်။ အတည်ပြုခြင်းတွင် အသုံးပြုသူအမည်နှင့် စကားဝှက်ကို အတည်ပြုခြင်းထက် ပိုမိုပါဝင်ပါသည်။ လုံခြုံရေးကို မြှင့်တင်ရန်အတွက်၊ အတည်ပြုခြင်းတွင် ကိုယ်တိုင်ဝန်ဆောင်မှု စကားဝှက် ပြန်လည်သတ်မှတ်ခြင်း (SSPR)၊ အချက်အလက်ပေါင်းစုံ အတည်ပြုခြင်း (MFA)၊ စကားဝှက်မဲ့နှင့် writeback ကဲ့သို့သော အစိတ်အပိုင်းများစွာ ပါဝင်ပါသည်။

အောက်ပါ နောက်ထပ် အရင်းအမြစ်များသည် အတည်ပြုခြင်းဆိုင်ရာ သင်၏ နားလည်မှုကို ကျယ်ပြန့်စေရန် ရည်ရွယ်ပါသည်။

- **Microsoft authentication overview:** [https://learn.microsoft.com/en-us/azure/active-directory/authentication/authentication-fundamentals-overview](https://learn.microsoft.com/en-us/azure/active-directory/authentication/authentication-fundamentals-overview)

  ဤ အတည်ပြုခြင်း အယူအဆများအကြောင်း ပိုမိုနက်ရှိုင်းစွာ လေ့လာရန် ဤ အရင်းအမြစ်ကို လိုက်နာပါ။

- **Passwordless authentication options:** [https://learn.microsoft.com/en-us/azure/active-directory/authentication/howto-authentication-passwordless](https://learn.microsoft.com/en-us/azure/active-directory/authentication/howto-authentication-passwordless)

  ၎င်းသည် မည်သို့ အလုပ်လုပ်သည်ကို ရှင်းလင်းသော ဖော်ပြချက် ဘာသာစကားနှင့် ရှင်းလင်းသော ပုံကားချပ်များဖြင့် စကားဝှက်မဲ့ အတည်ပြုခြင်းကို နားလည်ပါ။

- **FIDO (Fast IDentity Online):** [https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-authentication-passwordless#fido2-security-keys](https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-authentication-passwordless#fido2-security-keys)

  စကားဝှက်မဲ့သည် FIDO ၏ ခိုင်မာသော အစိတ်အပိုင်းတစ်ခုဖြစ်သည်။ ဤ အရင်းအမြစ်သည် FIDO သည် အဆင်ပြေပြီး လုံခြုံပုံနှင့် ၎င်းတွင် မည်သည့် အစိတ်အပိုင်းများ ပါဝင်ကြောင်း စူးစမ်းသည်။

- **Authentication and verification methods:** [https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-authentication-methods](https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-authentication-methods)

  အမျိုးမျိုးသော အတည်ပြုခြင်းနည်းလမ်းများ၏ ထိရောက်မှုဆိုင်ရာ အသေးစိတ် အသိပညာကို ရှာဖွေပါ။ ဤ အရင်းအမြစ်တွင် Azure AD တွင် ရရှိနိုင်သော အတည်ပြုခြင်းနည်းလမ်းများနှင့် ဆက်စပ်နေသော အမျိုးမျိုးသော ဂုဏ်ရည်များကို နှိုင်းယှဉ်သည့် အကောင်းဆုံး ဇယားအချို့ ပါရှိသည်။

- **OATH tokens:** [https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-authentication-oath-tokens](https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-authentication-oath-tokens)

  MFA ကို ပြီးမြောက်ရန် အတည်ပြုခြင်းနည်းလမ်းများစွာသည် အင်တာနက်ချိတ်ဆက်မှု လိုအပ်ပါသည်။ သို့သော် ပါဝါ လွှမ်းခြုံမှုရှိသော အသုံးပြုသူအတွက် ရွေးချယ်ထားသော အကောင်အထည်ဖော်မှုသည် အဘယ်နည်း။ ဤ အရင်းအမြစ်သည် 30-60 စက္ကန့်တိုင်း ပြန်လည်ထုတ်ပေးသည့် တည်ဆောက်ထားသော အင်္ဂါရပ်တစ်ခု အပါအဝင် Oath ၏ အားသာချက်များကို ဖော်ပြထားသည်။ ၎င်းသည် MFA ကို လုပ်ဆောင်ရန် အင်တာနက်ချိတ်ဆက်မှု မလိုအပ်ကြောင်း ဆိုလိုသည်။

- **Phone options:** [https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-authentication-phone-options](https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-authentication-phone-options)

  သင်၏ အင်တာနက်ချိတ်ဆက်မှု ညံ့ဖျင်းပါက နောက်ထပ် ဖြစ်နိုင်ချေရှိသော ကျရှုံးမှုမှာ ဖုန်းကို အသုံးပြုခြင်းဖြစ်သည်။ ဤ အရင်းအမြစ်သည် အမျိုးမျိုးသော ဖုန်းလုပ်ဆောင်နိုင်စွမ်းကို မည်သို့ အကောင်အထည်ဖော်ရမည်ကို ပိုမိုနည်းပညာပိုင်းဆိုင်ရာ ဖော်ပြချက်အချို့ကို သင့်အား ပေးပါသည်။

ဤ အရင်းအမြစ်များသည် Azure AD ၏ မတူညီသော အစိတ်အပိုင်းများနှင့် အားသာချက်များကို သင်၏ နားလည်မှုကို မြှင့်တင်ရန်အတွက် အမျိုးမျိုးသော အတည်ပြုခြင်းနည်းလမ်းများအကြောင်း အသေးစိတ် ထိုးထွင်းသိမြင်မှုများကို ပေးပါသည်။ ဤ အသိပညာ အခြေခံသည် ထိရောက်သော လုံခြုံရေး အစီအမံများကို အကောင်အထည်ဖော်ရန် သင့်အား တပ်ဆင်ပေးပါသည်။
