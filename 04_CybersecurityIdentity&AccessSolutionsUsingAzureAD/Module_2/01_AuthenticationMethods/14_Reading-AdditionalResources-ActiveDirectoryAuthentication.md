# Additional resources: Active Directory authentication

[Additional resources: Active Directory authentication 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/supplement/wfh3x/additional-resources-active-directory-authentication)

## Additional Resources: Active Directory Authentication (အပိုဆောင်း အရင်းအမြစ်များ- Active Directory စစ်မှန်ကြောင်းအထောက်အထားပြခြင်း)

### Overview (ခြုံငုံသုံးသပ်ချက်)

ယခုအခါ၊ သင်သည် စစ်မှန်ကြောင်းအထောက်အထားပြခြင်း (authentication) ဆိုသည်မှာ အဘယ်နည်းနှင့် သင်နှင့် သင့်အဖွဲ့အစည်းအတွက် ရနိုင်သော စစ်မှန်ကြောင်းအထောက်အထားပြမှု နည်းလမ်းအမျိုးမျိုးကို ကောင်းစွာ နားလည်ထားပါပြီ။ အောက်ပါ အပိုဆောင်း အရင်းအမြစ်များကို စူးစမ်းလေ့လာခြင်းသည် စစ်မှန်ကြောင်းအထောက်အထားပြမှု နည်းလမ်းများအကြောင်း သင့်နားလည်မှုကို ပိုမိုမြှင့်တင်ပေးပါသည်။

### Single Sign-On (SSO) (တစ်ကြိမ်ဝင်ရောက်မှု - SSO)

SSO နှင့်ပတ်သက်၍ ပိုမိုနက်ရှိုင်းသော ထိုးထွင်းသိမြင်မှုများအတွက်၊ [SSO in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/what-is-single-sign-on) သို့ ဝင်ရောက်ကြည့်ရှုပါ။ SSO သည် လက်တွင်းရှိ (on-premises) သို့မဟုတ် ကလောက်အခြေခံ (cloud-based) Active Directory များသို့ ဝင်ရောက်ရာတွင် အသုံးပြုသူ၏ ပင်ပန်းမှုကို လျှော့ချရာတွင် အလွန်အထောက်အကူဖြစ်နိုင်ပါသည်။ ဤနေရာတွင်၊ Azure AD ဖြင့် အလိုအလျောက် ပြင်ဆင်သတ်မှတ်ထားသော အက်ပ်လီကေးရှင်းများကို စူးစမ်းနိုင်ပြီး၊ SSO က ၎င်းတို့ကို အကောင်အထည်ဖော်သည့် မတူညီသော နည်းလမ်းများကို လေ့လာနိုင်ပါသည်။

### Hybrid Identity with Azure Active Directory (Azure Active Directory ဖြင့် ပေါင်းစပ်အထောက်အထား)

လက်တွင်းရှိ နှင့် ကလောက်အခြေခံ Active Directory နှစ်ခုလုံးကို ပေါင်းစပ်အသုံးပြုခြင်းကို ပေါင်းစပ်စနစ် (hybrid system) ဟု ခေါ်သည်ကို ပြန်လည်သတိရပါ။ [Hybrid Identities in Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-hybrid-identity) အကြောင်း ပိုမိုလေ့လာပါ၊ ထိုသို့သော စနစ်တစ်ခု ဖန်တီးရာတွင် အရေးကြီးသော အစိတ်အပိုင်းနှစ်ခုဖြစ်သည့် ပြင်ဆင်ပေးခြင်း (provisioning) နှင့် ထပ်တူပြုခြင်း (synchronizing) တို့ကို လေ့လာနိုင်ပါသည်။

### Password Hash Synchronization (စကားဝှက် ဟက်ရှ် ထပ်တူပြုခြင်း)

ပေါင်းစပ်ပတ်ဝန်းကျင်ကို ပိုမိုနားလည်လာသည်နှင့်အမျှ၊ အထောက်အထားများကို ထပ်တူကျစေပြီး လုံခြုံအောင် ထားရှိနည်းကို သင်စဉ်းစားလိုပေမည်။ Microsoft တွင် AAD နှင့် AD ကို ထပ်တူကျစေရန် [Password Hash Synchronization](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-password-hash-synchronization) ကို စီမံခန့်ခွဲပေးသော ဝန်ဆောင်မှု နှစ်ခု ရှိပါသည်။ ဤဝန်ဆောင်မှုများမှာ Azure AD Connect နှင့် ပေါ့ပါးသော Azure AD Connect Sync တို့ဖြစ်သည်။ ဤအရင်းအမြစ်သည် Azure AD Connect Sync ဖြင့် စကားဝှက် ထပ်တူပြုခြင်းကို အကောင်အထည်ဖော်သည့် နည်းလမ်းများကို စူးစမ်းပေးပါသည်။

### Passwordless Authentication (စကားဝှက်မဲ့ စစ်မှန်ကြောင်းအထောက်အထားပြခြင်း)

ယခုအခါ၊ သင့်အတွက် ရနိုင်သော စစ်မှန်ကြောင်းအထောက်အထားပြမှု နည်းလမ်းအမျိုးမျိုးရှိကြောင်း သင်သိပါသည်။ ဤနည်းလမ်းများသည် ပိုမိုမြှင့်တင်ထားသော လုံခြုံရေးနှင့် အသုံးပြုသူများအတွက် အဆင်ပြေမှုကို ပေးစွမ်းပါသည်။ ပိုမိုလေ့လာရန် အောက်ပါ အရင်းအမြစ်များကို စူးစမ်းပါ-

#### Passwordless Authentication Options for Azure Active Directory (Azure Active Directory အတွက် စကားဝှက်မဲ့ စစ်မှန်ကြောင်းအထောက်အထားပြမှု ရွေးချယ်စရာများ)

[Passwordless Authentication Options for Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/authentication/concept-authentication-passwordless): စကားဝှက်များသည် စနစ်တစ်ခုကို လုံခြုံစေရန် အချိန်ကြာရှည် အသုံးပြုလာခဲ့သော ချဉ်းကပ်မှုတစ်ခုဖြစ်သော်လည်း၊ ခေတ်မီလုံခြုံရေး အစီအမံများတွင် အပိုဆောင်း အင်္ဂါရပ်အချို့ ပါဝင်ပါသည်။ ဤအရင်းအမြစ်သည် လုံခြုံသော စနစ်တစ်ခုကို ထိန်းသိမ်းရမှုနှင့် အသုံးပြုသူအတွက် အသုံးပြုရလွယ်ကူမှု အကြား ဖြစ်ပေါ်လာသော အပေးအယူများကို စူးစမ်းပေးပါသည်။ ၎င်းတို့သည် မကြာခဏ တစ်ခုနှင့်တစ်ခု ဆန့်ကျင်ဘက် ဖြစ်တတ်ပါသည်။

#### Microsoft Authenticator App (Microsoft Authenticator အက်ပ်)

[Microsoft Authenticator App](https://docs.microsoft.com/en-us/azure/active-directory/user-help/user-help-auth-app-overview): ဤနည်းလမ်းသည် Azure AD တွင် အလုပ်လုပ်သည့်အခါ သင့်အတွက် အပိုဆောင်း လုံခြုံရေးအလွှာတစ်ခု ဖြစ်ပါသည်။ ဝင်ရောက်သည့်အခါ စကားဝှက်မဲ့ နည်းလမ်းဖြင့် စစ်မှန်ကြောင်းအထောက်အထားပြခြင်းအကြောင်း ပိုမိုလေ့လာပါ။

### Conclusion (နိဂုံး)

ဤအပိုဆောင်း အရင်းအမြစ်များကို အသုံးပြုခြင်းဖြင့်၊ သင်သည် စစ်မှန်ကြောင်းအထောက်အထားပြမှု နည်းလမ်းများအကြောင်း သင့်နားလည်မှုကို ပိုမိုနက်ရှိုင်းစေပြီး၊ သင့်လိုအပ်ချက်များအတွက် အသင့်လျော်ဆုံး ရွေးချယ်စရာ(များ)ကို အကောင်အထည်ဖော်နိုင်ပါသည်။ သင်သည် AD နှင့် Azure AD အကြား သင့်စကားဝှက်များနှင့် အခြားဒေတာများကို ထပ်တူပြုရန် ရနိုင်သော ကိရိယာများအကြောင်း ထပ်မံလေ့လာခဲ့ပြီး၊ SSO မှတစ်ဆင့် တစ်ကြိမ်တည်း ဝင်ရောက်မှုဖြင့် ဝန်ဆောင်မှုများစွာသို့ ဝင်ရောက်နိုင်မှု၏ အဆင်ပြေမှုနှင့် လုံခြုံရေးမှ အကျိုးခံစားခဲ့ရသည်။
