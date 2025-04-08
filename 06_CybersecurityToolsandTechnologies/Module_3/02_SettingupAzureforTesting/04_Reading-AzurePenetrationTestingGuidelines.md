# Azure penetration testing guidelines

[Azure penetration testing guidelines 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/supplement/wuSRe/azure-penetration-testing-guidelines)

# Azure Penetration Testing Guidelines (Azure ထိုးဖောက်စမ်းသပ်မှု လမ်းညွှန်ချက်များ)

## Introduction (နိဒ္ဒါန်း)

In cloud environments like Microsoft Azure, the importance of penetration testing is amplified, serving as a barrier to the security of cloud-based resources and data repositories. Penetration testing is a critical security practice that involves assessing the security posture of an information system by simulating cyberattacks to identify vulnerabilities and weaknesses.

ဤစာဖတ်ခြင်းတွင် Microsoft Azure တွင် ထိုးဖောက်စမ်းသပ်မှုတစ်ခု လုပ်ဆောင်ရန်အတွက် အဓိကအဆင့်များနှင့် ထည့်သွင်းစဉ်းစားရမည့်အချက်များကို သင်လေ့လာပါမည်။

## Guidelines to performing Azure penetration testing (Azure ထိုးဖောက်စမ်းသပ်မှု လုပ်ဆောင်ရန် လမ်းညွှန်ချက်များ)

### Planning and preparation (စီမံကိန်းရေးဆွဲခြင်းနှင့် ပြင်ဆင်ခြင်း)

The first step in conducting a penetration test on Azure is planning and preparation. It is essential to carefully plan and prepare to ensure the safety of both your assets and the Azure environment itself.

Azure တွင် ထိုးဖောက်စမ်းသပ်မှုတစ်ခု လုပ်ဆောင်ရာတွင် ပထမအဆင့်မှာ စီမံကိန်းရေးဆွဲခြင်းနှင့် ပြင်ဆင်ခြင်းဖြစ်သည်။ သင်၏ပိုင်ဆိုင်မှုများနှင့် Azure ပတ်ဝန်းကျင်ကိုယ်တိုင်၏ ဘေးကင်းမှုကို သေချာစေရန်အတွက် ဂရုတစိုက် စီမံကိန်းရေးဆွဲခြင်းနှင့် ပြင်ဆင်ခြင်းသည် မရှိမဖြစ်လိုအပ်ပါသည်။

- **Scope definition (နယ်ပယ်သတ်မှတ်ခြင်း)**: Clearly define the scope of the penetration test. Identify the specific Azure resources, services, and applications in scope for testing.

  ထိုးဖောက်စမ်းသပ်မှု၏ နယ်ပယ်ကို ရှင်းလင်းစွာ သတ်မှတ်ပါ။ စမ်းသပ်ရန်အတွက် အကျုံးဝင်သော သီးခြား Azure အရင်းအမြစ်များ၊ ဝန်ဆောင်မှုများနှင့် အပလီကေးရှင်းများကို ခွဲခြားသတ်မှတ်ပါ။

- **Permission and notification (ခွင့်ပြုချက်နှင့် အသိပေးခြင်း)**: Obtain proper authorization from Azure administrators and Microsoft Azure's support team before starting the test. Unauthorized penetration testing can result in account suspension.

  စမ်းသပ်မှုမစတင်မီ Azure စီမံခန့်ခွဲသူများနှင့် Microsoft Azure ၏ ပံ့ပိုးကူညီရေးအဖွဲ့ထံမှ သင့်လျော်သော ခွင့်ပြုချက်ရယူပါ။ ခွင့်ပြုချက်မရှိဘဲ ထိုးဖောက်စမ်းသပ်ခြင်းသည် အကောင့်ရပ်ဆိုင်းခြင်းကို ဖြစ်ပေါ်စေနိုင်သည်။

- **Rules of engagement (ပါဝင်မှုစည်းမျဉ်းများ)**: Define the rules of engagement that outline the testing methods, target assets, testing hours, and expected outcomes. Ensure that all stakeholders understand and agree to these rules.

  စမ်းသပ်မှုနည်းလမ်းများ၊ ပစ်မှတ်ပိုင်ဆိုင်မှုများ၊ စမ်းသပ်မှုအချိန်များနှင့် မျှော်လင့်ထားသော ရလဒ်များကို ဖော်ပြသည့် ပါဝင်မှုစည်းမျဉ်းများကို သတ်မှတ်ပါ။ သက်ဆိုင်သူအားလုံးသည် ဤစည်းမျဉ်းများကို နားလည်ပြီး သဘောတူကြောင်း သေချာပါစေ။

- **Legal and compliance (တရားဥပဒေနှင့် လိုက်နာမှု)**: Ensure that the penetration test complies with legal and regulatory requirements in your jurisdiction.

  သင်၏တရားစီရင်ပိုင်ခွင့်ရှိ တရားဥပဒေနှင့် စည်းမျဉ်းစည်းကမ်းများ၏ လိုအပ်ချက်များနှင့် ထိုးဖောက်စမ်းသပ်မှုသည် ကိုက်ညီကြောင်း သေချာပါစေ။

### Understanding the Azure environment (Azure ပတ်ဝန်းကျင်ကို နားလည်ခြင်း)

It is crucial to understand the Azure environment to effectively plan and conduct a penetration test.

ထိုးဖောက်စမ်းသပ်မှုကို ထိရောက်စွာ စီမံကိန်းရေးဆွဲရန်နှင့် လုပ်ဆောင်ရန်အတွက် Azure ပတ်ဝန်းကျင်ကို နားလည်ရန် အလွန်အရေးကြီးပါသည်။

- **Azure architecture (Azure ဗိသုကာ)**: Familiarize yourself with Azure's architecture, including regions, availability zones, and networking components such as virtual networks, subnets, and firewalls.

  ဒေသများ၊ ရရှိနိုင်မှုဇုန်များနှင့် virtual networks၊ subnets နှင့် firewalls ကဲ့သို့သော ကွန်ရက်အစိတ်အပိုင်းများအပါအဝင် Azure ၏ ဗိသုကာနှင့် ရင်းနှီးကျွမ်းဝင်ပါ။

- **Azure services (Azure ဝန်ဆောင်မှုများ)**: Identify the Azure services in use, such as virtual machines, databases, storage accounts, and containers.

  virtual machines၊ databases၊ storage accounts နှင့် containers ကဲ့သို့သော အသုံးပြုနေသော Azure ဝန်ဆောင်မှုများကို ခွဲခြားသတ်မှတ်ပါ။

- **Identity and access management (အထောက်အထားနှင့် ဝင်ရောက်ခွင့် စီမံခန့်ခွဲမှု)**: Understand Azure Active Directory (AD), role-based access control (RBAC), and identity management mechanisms.

  Azure Active Directory (AD)၊ အခန်းကဏ္ဍအခြေပြု ဝင်ရောက်ခွင့် ထိန်းချုပ်မှု (RBAC) နှင့် အထောက်အထားစီမံခန့်ခွဲမှု ယန္တရားများကို နားလည်ပါ။

### Threat modeling (ခြိမ်းခြောက်မှုပုံစံဖော်ခြင်း)

Conduct a threat modeling exercise to identify potential attack vectors and prioritize them based on risk.

ဖြစ်နိုင်ချေရှိသော တိုက်ခိုက်မှုလမ်းကြောင်းများကို ခွဲခြားသတ်မှတ်ရန်နှင့် အန္တရာယ်အပေါ် အခြေခံ၍ ၎င်းတို့ကို ဦးစားပေးရန် ခြိမ်းခြောက်မှုပုံစံဖော်ခြင်း လေ့ကျင့်ခန်းတစ်ခုကို လုပ်ဆောင်ပါ။

- **Asset identification (ပိုင်ဆိုင်မှု ခွဲခြားသတ်မှတ်ခြင်း)**: Identify the most critical assets in your Azure environment, such as sensitive data, applications, and services.

  အရေးကြီးသော ဒေတာ၊ အပလီကေးရှင်းများနှင့် ဝန်ဆောင်မှုများကဲ့သို့ သင်၏ Azure ပတ်ဝန်းကျင်ရှိ အရေးအကြီးဆုံး ပိုင်ဆိုင်မှုများကို ခွဲခြားသတ်မှတ်ပါ။

- **Vulnerability assessment (အားနည်းချက် အကဲဖြတ်ခြင်း)**: Use tools and manual analysis to identify potential vulnerabilities in Azure resources.

  Azure အရင်းအမြစ်များရှိ ဖြစ်နိုင်ချေရှိသော အားနည်းချက်များကို ခွဲခြားသတ်မှတ်ရန် ကိရိယာများနှင့် လက်ဖြင့်ခွဲခြမ်းစိတ်ဖြာခြင်းကို အသုံးပြုပါ။

- **Attack surface mapping (တိုက်ခိုက်မှုမျက်နှာပြင် မြေပုံဆွဲခြင်း)**: Determine how attackers could move laterally within the Azure environment and escalate privileges.

  တိုက်ခိုက်သူများသည် Azure ပတ်ဝန်းကျင်အတွင်း ဘေးတိုက်ရွေ့လျားပြီး အခွင့်အရေးများကို မည်သို့တိုးမြှင့်နိုင်သည်ကို ဆုံးဖြတ်ပါ။

### Penetration testing (ထိုးဖောက်စမ်းသပ်ခြင်း)

Execute the penetration tests based on the predefined rules of engagement.

ကြိုတင်သတ်မှတ်ထားသော ပါဝင်မှုစည်းမျဉ်းများအပေါ် အခြေခံ၍ ထိုးဖောက်စမ်းသပ်မှုများကို လုပ်ဆောင်ပါ။

- **Network security testing (ကွန်ရက်လုံခြုံရေး စမ်းသပ်ခြင်း)**: Test the security of Azure networking components, including firewalls, network security groups (NSGs), and virtual network configurations.

  firewalls၊ network security groups (NSGs) နှင့် virtual network ဖွဲ့စည်းမှုများအပါအဝင် Azure ကွန်ရက်အစိတ်အပိုင်းများ၏ လုံခြုံရေးကို စမ်းသပ်ပါ။

- **Web application testing (ဝဘ်အပလီကေးရှင်း စမ်းသပ်ခြင်း)**: Assess the security of web applications hosted in Azure, including APIs, websites, and microservices.

  APIs၊ ဝဘ်ဆိုဒ်များနှင့် microservices များအပါအဝင် Azure တွင် လက်ခံထားသော ဝဘ်အပလီကေးရှင်းများ၏ လုံခြုံရေးကို အကဲဖြတ်ပါ။

- **Database security testing (ဒေတာဘေ့စ်လုံခြုံရေး စမ်းသပ်ခြင်း)**: Test the security of Azure databases, ensuring that they are properly configured and protected.

  Azure ဒေတာဘေ့စ်များ၏ လုံခြုံရေးကို စမ်းသပ်ပြီး ၎င်းတို့ကို သင့်လျော်စွာ ဖွဲ့စည်းပြီး ကာကွယ်ထားကြောင်း သေချာပါစေ။

- **Identity and access testing (အထောက်အထားနှင့် ဝင်ရောက်ခွင့် စမ်းသပ်ခြင်း)**: Evaluate Azure AD and RBAC configurations to identify misconfigurations or weaknesses in identity and access management.

  အထောက်အထားနှင့် ဝင်ရောက်ခွင့် စီမံခန့်ခွဲမှုတွင် မှားယွင်းသော ဖွဲ့စည်းမှုများ သို့မဟုတ် အားနည်းချက်များကို ခွဲခြားသတ်မှတ်ရန် Azure AD နှင့် RBAC ဖွဲ့စည်းမှုများကို အကဲဖြတ်ပါ။

### Exploitation and post-exploitation (အသုံးချခြင်းနှင့် အသုံးချပြီးနောက် လုပ်ဆောင်ချက်များ)

When discovering and exploiting vulnerabilities, you must perform some controlled actions to demonstrate potential impact.

အားနည်းချက်များကို ရှာဖွေတွေ့ရှိပြီး အသုံးချသည့်အခါ ဖြစ်နိုင်ချေရှိသော သက်ရောက်မှုကို သရုပ်ပြရန်အတွက် ထိန်းချုပ်ထားသော လုပ်ဆောင်ချက်အချို့ကို သင်လုပ်ဆောင်ရမည်ဖြစ်သည်။

- **Privilege escalation (အခွင့်အရေး တိုးမြှင့်ခြင်း)**: Test for privilege escalation within the Azure environment to understand the extent of potential compromise.

  ဖြစ်နိုင်ချေရှိသော အားနည်းချက်၏ အတိုင်းအတာကို နားလည်ရန်အတွက် Azure ပတ်ဝန်းကျင်အတွင်း အခွင့်အရေး တိုးမြှင့်ခြင်းကို စမ်းသပ်ပါ။

- **Data exposure (ဒေတာ ထိတွေ့မှု)**: Demonstrate how an attacker could access or exfiltrate sensitive data if vulnerabilities are successfully exploited.

  အားနည်းချက်များကို အောင်မြင်စွာ အသုံးချပါက တိုက်ခိုက်သူသည် အရေးကြီးသော ဒေတာကို မည်သို့ဝင်ရောက်နိုင်သည် သို့မဟုတ် ထုတ်ယူနိုင်သည်ကို သရုပ်ပြပါ။

- **Maintaining access (ဝင်ရောက်ခွင့် ထိန်းသိမ်းခြင်း)**: Illustrate the persistence an attacker could achieve by maintaining unauthorized access to Azure resources.

  Azure အရင်းအမြစ်များသို့ ခွင့်ပြုချက်မရှိဘဲ ဝင်ရောက်ခွင့်ကို ထိန်းသိမ်းခြင်းဖြင့် တိုက်ခိုက်သူသည် မည်သို့သော ခိုင်မာမှုကို ရရှိနိုင်သည်ကို သရုပ်ပြပါ။

### Documentation (မှတ်တမ်းတင်ခြင်း)

Thorough documentation is crucial to provide a clear understanding of the findings and their potential impact.

တွေ့ရှိချက်များနှင့် ၎င်းတို့၏ ဖြစ်နိုင်ချေရှိသော သက်ရောက်မှုကို ရှင်းလင်းစွာ နားလည်စေရန်အတွက် စေ့စပ်သေချာသော မှတ်တမ်းတင်ခြင်းသည် အလွန်အရေးကြီးပါသည်။

- **Vulnerability reports (အားနည်းချက် အစီရင်ခံစာများ)**: Create detailed reports for each identified vulnerability, including their descriptions, steps to reproduce, potential impact, and remediation recommendations.

  ၎င်းတို့၏ ဖော်ပြချက်များ၊ ပြန်လည်ထုတ်လုပ်ရန် အဆင့်များ၊ ဖြစ်နိုင်ချေရှိသော သက်ရောက်မှုနှင့် ပြုပြင်ရန် အကြံပြုချက်များအပါအဝင် ခွဲခြားသတ်မှတ်ထားသော အားနည်းချက်တစ်ခုစီအတွက် အသေးစိတ်အစီရင်ခံစာများ ဖန်တီးပါ။

- **Evidence collection (သက်သေခံ အထောက်အထား စုဆောင်းခြင်း)**: Gather evidence of successful exploitation, such as screenshots, logs, and any other relevant data.

  အောင်မြင်စွာ အသုံးချခြင်း၏ သက်သေခံ အထောက်အထားများ (စခရင်ပုံများ၊ မှတ်တမ်းများနှင့် အခြားသက်ဆိုင်ရာ ဒေတာများ) ကို စုဆောင်းပါ။

### Remediation and reporting (ပြုပြင်ခြင်းနှင့် အစီရင်ခံခြင်း)

Collaborate with Azure administrators to address the identified vulnerabilities and weaknesses.

ခွဲခြားသတ်မှတ်ထားသော အားနည်းချက်များနှင့် ချို့ယွင်းချက်များကို ကိုင်တွယ်ဖြေရှင်းရန် Azure စီမံခန့်ခွဲသူများနှင့် ပူးပေါင်းဆောင်ရွက်ပါ။

- **Prioritization (ဦးစားပေးသတ်မှတ်ခြင်း)**: Work with Azure administrators to prioritize and address vulnerabilities based on their potential impact.

  ၎င်းတို့၏ ဖြစ်နိုင်ချေရှိသော သက်ရောက်မှုအပေါ် အခြေခံ၍ အားနည်းချက်များကို ဦးစားပေးသတ်မှတ်ရန်နှင့် ကိုင်တွယ်ဖြေရှင်းရန် Azure စီမံခန့်ခွဲသူများနှင့် ပူးပေါင်းဆောင်ရွက်ပါ။

- **Remediation (ပြုပြင်ခြင်း)**: Provide clear guidance on how to remediate each vulnerability and secure the Azure environment.

  အားနည်းချက်တစ်ခုစီကို မည်သို့ပြုပြင်ရမည်နှင့် Azure ပတ်ဝန်းကျင်ကို လုံခြုံစေရမည်ကို ရှင်းလင်းသော လမ်းညွှန်ချက်ပေးပါ။

- **Post-test review (စမ်းသပ်ပြီးနောက် ပြန်လည်သုံးသပ်ခြင်း)**: Conduct a post-test review meeting to discuss findings, remediation efforts, and lessons learned.

  တွေ့ရှိချက်များ၊ ပြုပြင်မှုကြိုးပမ်းမှုများနှင့် သင်ခန်းစာများကို ဆွေးနွေးရန် စမ်းသပ်ပြီးနောက် ပြန်လည်သုံးသပ်ခြင်း အစည်းအဝေးတစ်ခုကို လုပ်ဆောင်ပါ။

## Steps to perform a penetration test in Azure (Azure တွင် ထိုးဖောက်စမ်းသပ်မှုတစ်ခု လုပ်ဆောင်ရန် အဆင့်များ)

To conduct a penetration test in a Microsoft Azure environment, perform the following steps:

Microsoft Azure ပတ်ဝန်းကျင်တွင် ထိုးဖောက်စမ်းသပ်မှုတစ်ခု လုပ်ဆောင်ရန် အောက်ပါအဆင့်များကို လုပ်ဆောင်ပါ။

1.  Identify attack surfaces. (တိုက်ခိုက်ခံရနိုင်သော မျက်နှာပြင်များကို ခွဲခြားသတ်မှတ်ပါ။)
2.  Collect data for security reviews using Azure Security Center. (Azure Security Center ကို အသုံးပြု၍ လုံခြုံရေးသုံးသပ်မှုများအတွက် ဒေတာစုဆောင်းပါ။)
3.  Scan for vulnerabilities using the Azure Portal. (Azure Portal ကို အသုံးပြု၍ အားနည်းချက်များကို စကင်ဖတ်ပါ။)
4.  Collect evidence and indications of compromise (IoC). (ချိုးဖောက်ခံရကြောင်း အထောက်အထားများနှင့် လက္ခဏာများ (IoC) ကို စုဆောင်းပါ။)
5.  Notify engineering and operations teams. (အင်ဂျင်နီယာနှင့် လုပ်ငန်းလည်ပတ်ရေးအဖွဲ့များကို အသိပေးပါ။)

### Identify attack surfaces (တိုက်ခိုက်ခံရနိုင်သော မျက်နှာပြင်များကို ခွဲခြားသတ်မှတ်ခြင်း)

Attack path analysis helps you to identify the security issues in the cloud environment that pose the most risk. It also enables you to prioritize their remediation by detecting exploitable paths attackers can use in the environment.

တိုက်ခိုက်မှုလမ်းကြောင်းခွဲခြမ်းစိတ်ဖြာခြင်းသည် cloud ပတ်ဝန်းကျင်တွင် အန္တရာယ်အများဆုံးဖြစ်စေသော လုံခြုံရေးဆိုင်ရာ ပြဿနာများကို ခွဲခြားသတ်မှတ်ရန် ကူညီပေးပါသည်။ ၎င်းသည် တိုက်ခိုက်သူများ ပတ်ဝန်းကျင်တွင် အသုံးချနိုင်သော လမ်းကြောင်းများကို ရှာဖွေခြင်းဖြင့် ၎င်းတို့၏ ပြုပြင်မှုကို ဦးစားပေးရန်လည်း လုပ်ဆောင်ပေးပါသည်။

To investigate and remediate an attack surface or an attack path, perform the following steps:

တိုက်ခိုက်ခံရနိုင်သော မျက်နှာပြင် သို့မဟုတ် တိုက်ခိုက်မှုလမ်းကြောင်းတစ်ခုကို စုံစမ်းစစ်ဆေးပြီး ပြုပြင်ရန် အောက်ပါအဆင့်များကို လုပ်ဆောင်ပါ။

1.  Sign in to portal.azure.com. (portal.azure.com သို့ လက်မှတ်ထိုးဝင်ပါ။)
2.  Navigate to **Microsoft Defender for Cloud > Attack path analysis**. (**Microsoft Defender for Cloud > Attack path analysis** သို့ သွားပါ။)

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/NfMDU-LFTp6my5r7T0AANg_64259328375f4baa88d00941e52617e1_image.png?expiry=1744243200000&hmac=hXj7lSk-6Px0Np8UHUeCfrhQosQTVEzWgJOTm-DTpi0">

3.  Select an attack path. (တိုက်ခိုက်မှုလမ်းကြောင်းတစ်ခုကို ရွေးချယ်ပါ။)

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/-4SuazI-QUigaNBKMWRkYA_a72199f6dd9c4510b5943967620d1de1_image.png?expiry=1744243200000&hmac=advHpwzMmTinIOm_9Gzf78EMsUauwpZTGfkhUYe_F0E">

4.  Select a node. (node တစ်ခုကို ရွေးချယ်ပါ။)

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/J9pbKphNQKSO-oNSZnn-Iw_0e26e22450174f6d9121eac0e2c054e1_image.png?expiry=1744243200000&hmac=X4iqz8FwsPtqGyjr8ec62w56u-25WI0SznjGu01J0kM">

5.  Select **Insights** to view the associated insights for that node. (ထို node အတွက် ဆက်စပ်အချက်အလက်များကို ကြည့်ရှုရန် **Insights** ကို ရွေးချယ်ပါ။)

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/EIO4_rsfQR6yYwuhJDInTw_ebcdd11b79fe44adad9fc7eb4b23a1e1_image.png?expiry=1744243200000&hmac=rX8pmhnGVPAwAJNLD-hzh44IwOdxgU2EFAlcRLL9Cv8">

6.  Select **Recommendations**. (**Recommendations** ကို ရွေးချယ်ပါ။)
7.  Select a recommendation. (အကြံပြုချက်တစ်ခုကို ရွေးချယ်ပါ။)
8.  Follow the remediation steps to remediate the recommendation. (အကြံပြုချက်ကို ပြုပြင်ရန် ပြုပြင်ရေးအဆင့်များကို လိုက်နာပါ။)
9.  Select other nodes as necessary and view their insights and recommendations, as required. (လိုအပ်သလို အခြား nodes များကို ရွေးချယ်ပြီး ၎င်းတို့၏ အချက်အလက်များနှင့် အကြံပြုချက်များကို ကြည့်ရှုပါ။)

Once an attack path is resolved, it can take up to 24 hours for an attack path to be removed from the list.

တိုက်ခိုက်မှုလမ်းကြောင်းတစ်ခု ဖြေရှင်းပြီးပါက စာရင်းမှ ဖယ်ရှားရန် ၂၄ နာရီအထိ ကြာနိုင်သည်။

## Collect data for security reviews using Azure Security Center (Azure Security Center ကို အသုံးပြု၍ လုံခြုံရေးသုံးသပ်မှုများအတွက် ဒေတာစုဆောင်းခြင်း)

Azure Security Benchmark တွင် Azure ရှိ သင်၏အပလီကေးရှင်းများနှင့် ဒေတာများ၏ လုံခြုံရေးကို မြှင့်တင်ရန် ကူညီနိုင်သည့် အကြံပြုချက်များ ပါဝင်သည်။ သင်၏လုံခြုံရေးမူဝါဒများနှင့် ယန္တရားများရှိ ချို့ယွင်းချက်များကို ခွဲခြားသတ်မှတ်ရန် ကူညီရန်အတွက် Azure သည် ဖွဲ့စည်းနိုင်သော လုံခြုံရေးစစ်ဆေးခြင်းနှင့် မှတ်တမ်းတင်ခြင်း ရွေးချယ်စရာများစွာကို ပေးပါသည်။ ကွန်ပျူတာအရင်းအမြစ်ကို Microsoft က ပိုင်ဆိုင်ပါက Microsoft သည် ၎င်းကို စောင့်ကြည့်ရန် တာဝန်ရှိသည်။ သို့သော် ကွန်ပျူတာအရင်းအမြစ်ကို သင်၏အဖွဲ့အစည်းက ပိုင်ဆိုင်ပါက ၎င်းကို စောင့်ကြည့်ရန် သင်၏တာဝန်ဖြစ်သည်။ လည်ပတ်မှုစနစ် (OS) ကို စောင့်ကြည့်ရန် Azure Security Center ကို အသုံးပြုနိုင်သည်။

Security Center မှ OS မှ စုဆောင်းထားသော ဒေတာတွင် OS အမျိုးအစားနှင့် ဗားရှင်း၊ OS (Windows Event Logs)၊ လည်ပတ်နေသော လုပ်ငန်းစဉ်များ၊ စက်အမည်၊ IP လိပ်စာများနှင့် လက်မှတ်ထိုးဝင်ထားသော အသုံးပြုသူတို့ ပါဝင်သည်။
Microsoft Defender for Cloud ကို log analytics tool၊ Virtual Machine Scale Sets၊ Infrastructure as a service (IaaS) containers နှင့် လုံခြုံရေးဆိုင်ရာ အားနည်းချက်များနှင့် ခြိမ်းခြောက်မှုများကို စောင့်ကြည့်ရန်အတွက် non-Azure (on-premises အပါအဝင်) စက်များမှ ဒေတာစုဆောင်းရန်အတွက် အသုံးပြုနိုင်သည်။ Defender အစီအစဉ်အချို့သည် သင်၏လုပ်ငန်းဝန်များမှ ဒေတာစုဆောင်းရန် စောင့်ကြည့်ရေးအစိတ်အပိုင်းများ လိုအပ်သည်။
ပျောက်ဆုံးနေသော အပ်ဒိတ်များ၊ မှားယွင်းစွာ ဖွဲ့စည်းထားသော OS လုံခြုံရေးဆက်တင်များ၊ endpoint ကာကွယ်မှုအခြေအနေနှင့် ကျန်းမာရေးနှင့် ခြိမ်းခြောက်မှုကာကွယ်မှုတို့ကို မြင်နိုင်စွမ်းပေးရန် ဒေတာစုဆောင်းခြင်း လိုအပ်သည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/sc2foZgmQei7pEnSZkKteA_0ad2bf13f4b142759c81f1f1633674e1__v6JUOjEEoyt8aZanraUz9y6G_ojUHaHJK6GMn2YBxG45foh40K3W2LCrC00MeoHmDzHqLtLAh2Usm4ToKquX6BU5DwV5Ql-r2eF0diCeiK1uk3S5lHoRITom30VAwn92Rp2cYpcbsgZAEfyio9JrUU?expiry=1744243200000&hmac=N7yjkn2JA6BA_KGWuB_1ydhv7hNp8VDwlHL0EsAbQT4">

## Scan for vulnerabilities using the Azure Portal (Azure Portal ကို အသုံးပြု၍ အားနည်းချက်များကို စကင်ဖတ်ခြင်း)

ပေါင်းစည်းထားသော Qualys scanner ဖြင့် အားနည်းချက်စကင်ဖတ်ခြင်းကို ဖွင့်ခြင်းဖြင့် Azure Portal ကို အသုံးပြု၍ အားနည်းချက်များကို စကင်ဖတ်နိုင်သည်။
ဆိုက်ဘာအန္တရာယ်နှင့် လုံခြုံရေးအစီအစဉ်တိုင်း၏ အဓိကအစိတ်အပိုင်းတစ်ခုမှာ အားနည်းချက်များကို ခွဲခြားသတ်မှတ်ခြင်းနှင့် ခွဲခြမ်းစိတ်ဖြာခြင်းဖြစ်သည်။ Defender for Cloud သည် သင်၏ချိတ်ဆက်ထားသော စက်များကို ပုံမှန်စစ်ဆေးပြီး ၎င်းတို့တွင် အားနည်းချက်အကဲဖြတ်ကိရိယာများ လည်ပတ်နေကြောင်း သေချာစေသည်။
အားနည်းချက်အကဲဖြတ်မှုဖြေရှင်းချက်ကို တပ်ဆင်ထားခြင်းမရှိသော စက်တစ်ခုကို တွေ့ရှိသောအခါ Defender for Cloud သည် လုံခြုံရေးဆိုင်ရာ အကြံပြုချက်ကို ထုတ်ပေးသည်- စက်များတွင် အားနည်းချက်အကဲဖြတ်မှုဖြေရှင်းချက် ရှိသင့်သည်။ ဤအကြံပြုချက်ကို အသုံးပြု၍ သင်၏ Azure virtual machines များနှင့် သင်၏ Azure Arc-enabled hybrid machines များတွင် အားနည်းချက်အကဲဖြတ်မှုဖြေရှင်းချက်ကို ဖြန့်ကျက်ပါ။
Defender for Cloud တွင် သင်၏စက်များအတွက် အားနည်းချက်စကင်ဖတ်ခြင်း ပါဝင်သည်။ Qualys လိုင်စင် သို့မဟုတ် Qualys အကောင့်ပင် မလိုအပ်ပါ - အရာအားလုံးကို Defender for Cloud အတွင်း ချောမွေ့စွာ ကိုင်တွယ်ဆောင်ရွက်ပါသည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/-sKxwHhdRveG_iRHWhehbw_bdc45f88f1a74756ac7b484ee7760fe1_zUpMXRv-dDf-gzGm0Z3aYTs4Jc81FRC3uBPGa0Lu5C8aKQheXHXZTAD3RChYb6PtCafe0tFf829WCNrUbMJZrFEVShYWqoGiPLXBSeQh9P89rwrq13luX-GYsRd92mP7KlOmF6IqreeDXCUc6Z-hB3s?expiry=1744243200000&hmac=PSQsJxsZounXeXBLkRtVcLoEEy8h2xZEKgJbP4551P0">

## Collect evidence and indicators of compromise (IoC) (ချိုးဖောက်ခံရကြောင်း အထောက်အထားများနှင့် လက္ခဏာများ (IoC) ကို စုဆောင်းခြင်း)

ချိုးဖောက်ခံရကြောင်း လက္ခဏာ (IoC) သည် ကွန်ရက် သို့မဟုတ် host တွင် တွေ့ရှိရသော forensic artifact တစ်ခုဖြစ်သည်။ IoC သည် ကွန်ပျူတာ သို့မဟုတ် ကွန်ရက်အတွင်းသို့ ကျူးကျော်ဝင်ရောက်မှုတစ်ခု ဖြစ်ပွားခဲ့ကြောင်း အလွန်ယုံကြည်စိတ်ချစွာ ညွှန်ပြသည်။ IoCs များသည် တိုင်းတာနိုင်သော ဖြစ်ရပ်များနှင့် တိုက်ရိုက်ချိတ်ဆက်ထားသောကြောင့် လေ့လာတွေ့ရှိနိုင်ပါသည်။ IoC ဥပမာအချို့တွင်-

- သိရှိထားသော malware ၏ hashes များ
- မရိုးသားသော ကွန်ရက် traffic ၏ လက်မှတ်များ
- သိရှိထားသော malware ဖြန့်ဖြူးသူများ၏ URL များ သို့မဟုတ် domains များ
  နောက်ထပ် အားနည်းချက်ကို ရပ်တန့်ရန် သို့မဟုတ် သိရှိထားသော IoCs များကို ချိုးဖောက်ခြင်းမှ ကာကွယ်ရန်အတွက် အောင်မြင်သော IoC ကိရိယာများသည် ကိရိယာ၏ စည်းမျဉ်းအစုဖြင့် စာရင်းပြုစုထားသော မရိုးသားသော ဒေတာအားလုံးကို ရှာဖွေနိုင်ရမည်ဖြစ်သည်။ IoC ကိုက်ညီမှုသည် endpoint ကာကွယ်မှုဖြေရှင်းချက်တိုင်းတွင် မရှိမဖြစ်လိုအပ်သော လုပ်ဆောင်ချက်တစ်ခုဖြစ်သည်။ ဤစွမ်းရည်သည် Security Operations (SecOps) အား ရှာဖွေခြင်းနှင့် ပိတ်ဆို့ခြင်း (ကာကွယ်ခြင်းနှင့် တုံ့ပြန်ခြင်း) အတွက် ညွှန်ကိန်းများစာရင်းကို သတ်မှတ်နိုင်သည့် စွမ်းရည်ကို ပေးပါသည်။
  အဖွဲ့အစည်းများသည် IoC entities များကို ရှာဖွေခြင်း၊ ကာကွယ်ခြင်းနှင့် ချန်လှပ်ခြင်းတို့ကို သတ်မှတ်သည့် ညွှန်ကိန်းများကို ဖန်တီးနိုင်သည်။ လုပ်ဆောင်ရမည့် လုပ်ဆောင်ချက်အပြင် လုပ်ဆောင်ချက်ကို အသုံးပြုရမည့် ကြာချိန်နှင့် ၎င်းကို အသုံးပြုရမည့် စက်အုပ်စု၏ နယ်ပယ်ကို သင်သတ်မှတ်နိုင်သည်။
  Microsoft 365 defender portal မှ ညွှန်ကိန်းများကို ဖန်တီးနိုင်သည်။

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/JPHCqnSGTVK0VZ-myh8lsg_0444103317e844e08a1f7bb2f03062e1_d46HCyeamUDyjKAQhZwC_KiJXP9e51j36u4b9Ht6q88JqDpXCQ0cd-oIk3BQorMEoMryO6k27nnXf1UGDdokBHV0eAz4PdcOQeSJWNeokr6C2G8L4gwkajYojEkjf-TIoO4Kj0PMjn3wiAuQfa5nZfI?expiry=1744243200000&hmac=4gSN3YPt_nh8zFubBzS7soWBjujPWA32s4NNwECgK7I">

## Notify engineering and operations teams (အင်ဂျင်နီယာနှင့် လုပ်ငန်းလည်ပတ်ရေးအဖွဲ့များကို အသိပေးခြင်း)

Microsoft Azure ပတ်ဝန်းကျင်တွင် ထိုးဖောက်စမ်းသပ်မှုအစီအစဉ်တစ်ခုကို စတင်သောအခါ အခြေခံအကျဆုံးအဆင့်များထဲမှတစ်ခုမှာ အင်ဂျင်နီယာနှင့် လုပ်ငန်းလည်ပတ်ရေးအဖွဲ့များကို အသိပေးခြင်းဖြစ်သည်။ ဤကြိုတင်ဆက်သွယ်မှုသည် စမ်းသပ်မှုကာလအတွင်း ဖြစ်နိုင်ချေရှိသော အနှောင့်အယှက်များနှင့် မှားယွင်းစွာ အဓိပ္ပာယ်ဖွင့်ဆိုမှုများကို လျှော့ချနေစဉ် စမ်းသပ်မှု၏ ချောမွေ့စွာ လုပ်ဆောင်မှုကို သေချာစေရန်အတွက် အရေးကြီးပါသည်။ ၎င်းသည် အင်ဂျင်နီယာနှင့် လုပ်ငန်းလည်ပတ်ရေးအဖွဲ့များအား လာမည့်လုပ်ဆောင်ချက်များအတွက် ပြင်ဆင်ခွင့်ပြုပြီး စမ်းသပ်မှုပတ်ဝန်းကျင်၏ တည်ငြိမ်မှုကို ထိခိုက်စေနိုင်သည့် မလိုလားအပ်သော တုံ့ပြန်မှုများကို ကာကွယ်ပေးပါသည်။

## Conclusion (နိဂုံး)

ဤစာဖတ်ခြင်းတွင် Microsoft Azure ပတ်ဝန်းကျင်တွင် ထိုးဖောက်စမ်းသပ်မှုတစ်ခု လုပ်ဆောင်ရန် cloud နည်းပညာများနှင့် ဆိုက်ဘာလုံခြုံရေးနှစ်ခုလုံးတွင် ကျွမ်းကျင်မှုလိုအပ်ကြောင်း သင်လေ့လာခဲ့သည်။ ကျင့်ဝတ်ဆိုင်ရာ လမ်းညွှန်ချက်များကို လိုက်နာရန်၊ သက်ဆိုင်သူအားလုံးနှင့် ထိရောက်စွာ ဆက်သွယ်ရန်နှင့် Azure ပတ်ဝန်းကျင်နှင့် စမ်းသပ်ထားသော ပိုင်ဆိုင်မှုများ၏ လုံခြုံရေးကို ဦးစားပေးရန် အရေးကြီးပါသည်။ ပုံမှန်ထိုးဖောက်စမ်းသပ်ခြင်းသည် သင်၏ Azure အခြေခံအဆောက်အအုံ၏ လုံခြုံရေးအခြေအနေကို သိသိသာသာ မြှင့်တင်နိုင်ပြီး ပြောင်းလဲနေသော ဆိုက်ဘာခြိမ်းခြောက်မှုများမှ သင်၏ဒေတာနှင့် အပလီကေးရှင်းများကို ကာကွယ်ရန် ကူညီပေးနိုင်ပါသည်။
