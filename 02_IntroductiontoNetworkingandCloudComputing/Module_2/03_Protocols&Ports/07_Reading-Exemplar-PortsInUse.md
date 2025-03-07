# Exemplar: Ports in use

[Exemplar: Ports in use 🔗](https://www.coursera.org/learn/introduction-to-networking-and-Cloud-computing/supplement/DfiZt/exemplar-ports-in-use)

# နမူနာ - အသုံးပြုနေသော ပို့တ်များ

## Introduction နိဒါန်း

ဒီနမူနာက သင့်ကိရိယာမှာ လက်ရှိ အသုံးပြုနေတဲ့ ပရိုတိုကောတွေနဲ့ ပို့တ်တွေကို ဘယ်လို ဖော်ထုတ်နိုင်သလဲဆိုတာကို သရုပ်ပြပါတယ်။ အောက်မှာ Windows နဲ့ Mac ကိရိယာ နှစ်ခုလုံးအတွက် အဆင့်တွေကို ပြန်သုံးသပ်ပါ။ အနာဂတ်မှာ ကွန်ရက်ပေါ်မှာ ဒီစက်နှစ်မျိုးလုံးကို သင်ကြုံတွေ့ဖွယ် ရှိလို့ပါ။

## Identifying Protocols and Sessions on a Windows Machine Windows စက်ပေါ်မှာ ပရိုတိုကောများနှင့် ဆက်ရှင်များ ဖော်ထုတ်ခြင်း

### အဆင့် ၁ - တက်စဘားပေါ်က Windows ခလုတ်ကို နှိပ်ပါ။

_Windows စတင်မီနူး ပုံ_

<img src="https://d3c33hcgiwev3.Cloudfront.net/imageAssetProxy.v1/2SZVH8LxT7e3U55ks7aCXQ_7c376537e3984befa0e2e3f2e3cf8fe1_image.jpeg?expiry=1740873600000&hmac=azKC3ANwRyuWBmgXuZnsbDSxzH45QWHktRy_htYVF2g">

### အဆင့် ၂ - ရှာဖွေဘားမှာ "cmd" လို့ ရိုက်ပါ။ မီနူးမှာ ကွန်မန်း ပရော့ပ်အတွက် သေးပုံ (thumbnail) ပေါ်လာသင့်ပါတယ်။

_မီနူးမှာ ကွန်မန်း ပရော့ပ်အတွက် သေးပုံ_

<img src="https://d3c33hcgiwev3.Cloudfront.net/imageAssetProxy.v1/ekeiciAZRSGudL6jj8w0Hg_1310f5428d244712b472a80321916ae1_image.jpeg?expiry=1740873600000&hmac=EuelWTVaY6V25AaC-VBjz-gYd6jWUPT4vKCFfJQFPHk">

### အဆင့် ၃ - ကွန်မန်း ပရော့ပ်ကို ဖွင့်ဖို့ သေးပုံကို နှိပ်ပါ။ အနက်ရောင် နောက်ခံနဲ့ ဝင်းဒိုးတစ်ခု ဖွင့်လာပါလိမ့်မယ်။

_C2M2L3 Item07_img1 ကွန်မန်း ပရော့ပ် ဝင်းဒိုး_

<img src = "https://d3c33hcgiwev3.Cloudfront.net/imageAssetProxy.v1/A5YWbnnmTlCknhD6Dr3Rpw_7cb2d14a2bf64ba18cba3ff160a74ee1_CMD.png?expiry=1740873600000&hmac=Q-WwiLXJ9FOFkam4IYcBv6WIpTJJek0eAbvIz2nSqsc">

### အဆင့် ၄ - အနက်ရောင် နေရာမှာ "netstat -a" လို့ ရိုက်ပြီး Enter ကို နှိပ်ပါ။

_C2M2L3_Item 07_img2 ကွန်မန်း ပရော့ပ်မှာ netstat ရိုက်ထည့်ထားပုံ_

<img src = "https://d3c33hcgiwev3.Cloudfront.net/imageAssetProxy.v1/9L1IJB9XSf6JX_U7AhZMiQ_4225fc65b76242f39791d870cc53f5e1_netstat.png?expiry=1740873600000&hmac=fZZEIxmd08ewSFc89BGtBDrW0BnzeBgYrY4U58RMRfQ">

### အဆင့် ၅ - လက်ရှိ ဆက်ရှင်တွေ ဖွင့်လာဖို့ ၃၀ စက္ကန့် စောင့်ပါ�।

_C2M2L3_Item07_img3 ကွန်မန်း ပရော့ပ်မှာ ဖွင့်လာတဲ့ လက်ရှိ netstat ဆက်ရှင်_

<img src = "https://d3c33hcgiwev3.Cloudfront.net/imageAssetProxy.v1/j0nZYPioQFOnb4lM1_EZkA_5bba6320821f4dfdba68c9e4efd7ffe1_netstat-2.png?expiry=1740873600000&hmac=TQkWxTvwj9Vs_NejP7N0UcaNIv9COtAStVR1tvYhEZ4">

ဝင်းဒိုးထဲမှာ၊ သင့် PC ပေါ်မှာ ဖွင့်ထားတဲ့ ဆက်ရှင်တွေကို အခု ပြန်သုံးသပ်နိုင်သင့်ပါတယ်။

## Identifying Protocols and Sessions on a Mac Mac ပေါ်မှာ ပရိုတိုကောများနှင့် ဆက်ရှင်များ ဖော်ထုတ်ခြင်း

### အဆင့် ၁ - Spotlight ရှာဖွေမှု ဒါမှမဟုတ် Go > Utilities ကနေ Mac တာမီနယ်ကို ဖွင့်ပါ။ တာမီနယ် အပလီကေးရှင်း ဖွင့်လာပါလိမ့်မယ်။

_Spotlight ရှာဖွေဘား ပုံ_

<img src = "https://d3c33hcgiwev3.Cloudfront.net/imageAssetProxy.v1/3HVarNr4STS3oGI6WaeNOQ_5243201c6eff472a85fba057508e00e1_dHwWPcfwT86EtDFfmMLj_w_26f941ce038b4023929aa98012de06e1_image.png?expiry=1740873600000&hmac=WpEL6OG52SK-zXqZ7slVWfayla3McyQahLb7IrPjY3Y">

_MacOS တာမီနယ် ဝင်းဒိုး ပုံ_

<img src = "https://d3c33hcgiwev3.Cloudfront.net/imageAssetProxy.v1/MEdGk4aOSCSt7bKGb3HV6A_185fc60bae0d4776bb1b3936b9eb50e1_Terminal.png?expiry=1740873600000&hmac=twSSBLIvzJ2eHBPfTe0mzvZVVyTq4MZF4cTMHnIJECo">

### အဆင့် ၂ - အဖြူရောင် နေရာမှာ "netstat -a" လို့ ရိုက်ပါ။

_MacOS တာမီနယ်မှာ netstat -a ကွန်မန်း ရိုက်ထည့်ထားပုံ_

<img src="https://d3c33hcgiwev3.Cloudfront.net/imageAssetProxy.v1/mD17k01UR5CyPb7wg-VBnA_687507e9e2f74f0585408f6fa358dde1_Mac-netstat1.png?expiry=1740873600000&hmac=qtdf1spRPW0toJiZWPW9pNFVCdsqclJLiAJmDqzJjpU">

### အဆင့် ၃ - Mac က အထွက် (output) အများကြီး ထုတ်ပေးနိုင်တာမို့၊ သင် netstat ကွန်မန်း ရိုက်ထည့်တဲ့ နေရာဆီ ပြန်လှိမ့်ကြည့်ပါ။ ဒီကွန်မန်းရဲ့ အောက်မှာ လက်ရှိ ဆက်ရှင်တွေ ရှိပါလိမ့်မယ်။

_လက်ရှိ ဆက်ရှင် အားလုံးကို ပြသထားတဲ့ တာမီနယ် ပုံ_

<img src = "https://d3c33hcgiwev3.Cloudfront.net/imageAssetProxy.v1/ucqX_QtfT4KlTzdgmSz55A_490f1c10c71e49ba9cb704a62b6b16e1_Mac-netstat2.png?expiry=1740873600000&hmac=RmcrCouDlQikKLDmpDZ2rYo6PVhMzb7KUrRiq_NFZAw">

## Conclusion နိဂုံး

သင်ဟာ အခု Windows နဲ့ Mac တွေပေါ်မှာ လည်ပတ်နေတဲ့ မတူညီတဲ့ ဆက်ရှင်တွေနဲ့ ပရိုတိုကောတွေကို ဖော်ထုတ်နိုင်သင့်ပါပြီ။ ဒီဗဟုသုတက သင့်စက်ပေါ်မှာ ဘယ်ပရိုတိုကောတွေ လည်ပတ်နေသလဲ၊ ၎င်းတို့က ပရိုတိုကောရဲ့ လုံခြုံတဲ့ ဗားရှင်း ဟုတ်၊ မဟုတ်ဆိုတာကို စစ်ဆေးနိုင်စေပါတယ်။ ဘာတွေ အသုံးပြုနေလဲဆိုတာကို ကြည့်ဖို့ အပလီကေးရှင်း ပိုများများ ဖွင့်ကြည့်ပါ။
