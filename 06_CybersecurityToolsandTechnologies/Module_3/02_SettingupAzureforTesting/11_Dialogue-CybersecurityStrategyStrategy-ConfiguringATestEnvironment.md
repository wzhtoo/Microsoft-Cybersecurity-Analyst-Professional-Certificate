# Cybersecurity Strategy: Configuring a Test Environment

[Cybersecurity Strategy: Configuring a Test Environment 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/ungradedWidget/FW8x8/cybersecurity-strategy-configuring-a-test-environment)

# Cybersecurity Strategy: Configuring a Test Environment (ဆိုက်ဘာလုံခြုံရေး မဟာဗျူဟာ- စမ်းသပ်မှု ပတ်ဝန်းကျင်ကို ဖွဲ့စည်းခြင်း)

## Introduction (နိဒ္ဒါန်း)

စမ်းသပ်မှု ပတ်ဝန်းကျင်များသည် အဖွဲ့အစည်းများအား တကယ့်ကမ္ဘာ့အခြေအနေများကို အတုယူရန်၊ ဖွဲ့စည်းမှုဆိုင်ရာ ပြဿနာများကို ဖြေရှင်းရန်နှင့် တိုက်ရိုက်ပတ်ဝန်းကျင်ကို အန္တရာယ်မပြုဘဲ စနစ်များ မျှော်လင့်ထားသည့်အတိုင်း လုပ်ဆောင်ကြောင်း သေချာစေရန် ခွင့်ပြုပါသည်။

သင်သည် ၎င်း၏အတွင်းပိုင်း အခြေခံအဆောက်အအုံတွင် ထိုးဖောက်စမ်းသပ်မှုအတွက် ပြင်ဆင်နေသော ကုမ္ပဏီတစ်ခုဖြစ်သည့် CyberDefend Corp တွင် လုံခြုံရေး အင်ဂျင်နီယာတစ်ဦးဖြစ်သည်ဟု မြင်ယောင်ကြည့်ပါ။ သင်၏တာဝန်မှာ ထိန်းချုပ်ထားသော ဆက်တင်တွင် ဖြစ်နိုင်ချေရှိသော အားနည်းချက်များကို အကဲဖြတ်ရန် စမ်းသပ်မှု ပတ်ဝန်းကျင်တစ်ခုကို ဖန်တီးရန်ဖြစ်သည်။ ဤပတ်ဝန်းကျင်တွင် စမ်းသပ်မှု၏ လိုအပ်ချက်များနှင့်အညီ ပြုပြင်ထားသော virtual machines များ၊ ကွန်ရက်များနှင့် လုံခြုံရေး ထိန်းချုပ်မှုများ ပါဝင်မည်ဖြစ်သည်။

ခိုင်မာသော စမ်းသပ်မှု ပတ်ဝန်းကျင်တစ်ခုကို တည်ဆောက်ကြပါစို့။

[Testing and Dialog 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/ungradedWidget/FW8x8/cybersecurity-strategy-configuring-a-test-environment)

# Azure Penetration Testing Environment Setup

**Coach:** Hello! I am your Coursera Coach for this activity. Today, we will be setting up a penetration testing environment in Azure. We'll be focusing on configuring the network, virtual machines, and security controls.
To achieve our objective, we will be working through these checkpoints:
Networking Setup: Design a secure network topology for penetration testing. (Weight = 30%)
Virtual Machine Configuration: Choose and configure VMs for the test environment. (Weight = 40%)
Security Controls Implementation: Set up and configure security controls for the test. (Weight = 30%)
You can pause at any time during our session to review the material. Let me know when you are ready to begin our discussion!

**Win:** Let's get started

**Coach:** Great! Let's imagine CyberDefend Corp. wants to test their network against attackers who typically target web applications. How would you design the virtual network topology in Azure to simulate this scenario, and what considerations would you make for network security?

**Win:** Okay! We need to make a pretend computer network in the cloud for CyberDefend. It should have different rooms, like a house! One room for the website and another for the attackers, so they don't mess with the real stuff. We need to put strong doors between them to keep things safe!

**Coach:** You're thinking along the right lines! It's like having separate rooms in a house. In Azure, we call these rooms 'subnets' within a 'virtual network'.
So, we'll have one subnet for the web application, acting as our 'public-facing' area. Then, another subnet will house the attacker's virtual machines, completely isolated.
Tell me, how would you control the traffic or 'doors' between these subnets to make sure the attackers can't just walk into the web application's subnet? What tools in Azure can help us with that?

**Win:** We need special guards for the doors between the rooms! In Azure, these guards are called "Network Security Groups" or NSGs. They are like lists that say who can go in and out of each room and what they can carry. We can tell the NSG for the website room to only let people who want to see the website come in, but not the attackers' machines!

**Coach:** That's exactly right! Network Security Groups (NSGs) are the guards of our Azure network. We can configure strict rules for each subnet, controlling inbound and outbound traffic based on IP addresses, ports, and protocols.
You've clearly grasped the core concepts of using subnets and NSGs to design a secure network topology for penetration testing. You've earned 30 points for completing this checkpoint!
You are 30% complete.
Now, let's move on to setting up the virtual machines themselves. Are you ready to proceed to the next checkpoint?

**Win:** Yay!

**Coach:** That's great to hear! Let's move on to the next checkpoint: Virtual Machine Configuration.
CyberDefend Corp. uses a mix of Windows and Linux servers for their web application. Considering this, what operating systems would you choose for the attacker and target virtual machines in our test environment, and why? What factors would you consider when making this decision?

**Win:** Hmm, for the pretend computers, we should have one that looks like CyberDefend's computers, so maybe a Windows one and a Linux one for the website stuff. And for the attacker computer, maybe another Linux one because I think hackers use those sometimes for testing! We need to pick computers that can do the testing jobs well!

**Coach:** You've got the right idea! It's smart to mimic CyberDefend Corp.'s environment closely. So, for our target subnet, we'll have one Windows VM and one Linux VM, representing their web server and database server, respectively.
And you're spot on about attackers often using Linux. A Kali Linux VM in the attacker subnet would provide a wide range of penetration testing tools.
By mirroring their real-world setup, we create a more realistic and effective testing environment.
Now, tell me, what are some basic security configurations you would apply to ALL these virtual machines, regardless of their operating system, to ensure they are secure during our test? Think about the essential steps you'd take to harden any computer before exposing it to potential attacks.

**Win:** Okay! For all the pretend computers, we should:
Give them strong secret words to log in! Not easy-peasy ones!
Make sure only the right people can get in, like with a special key!
Keep them updated with the newest fixes so bad things can't sneak in!
Maybe turn off extra things they don't need so there are fewer doors for trouble!

**Coach:** You've outlined some crucial security hardening steps! Let's translate those into specific actions for our VMs:
Strong Passwords: We'll enforce complex passwords for all user accounts, making them difficult to crack.
Access Control: We'll use Azure Role-Based Access Control (RBAC) to grant only necessary permissions to specific users or groups.
Updates: We'll ensure all VMs are updated with the latest security patches to fix known vulnerabilities.
Disable Unnecessary Services: We'll disable any services or features not required for the test, reducing the attack surface.
You've demonstrated a good understanding of basic VM security configuration. You've earned 40 points for completing this checkpoint!
You are 70% complete.
Ready to move on to the final checkpoint: Security Controls Implementation?

**Win:** Yes! Let's put up even more shields to keep our pretend computers safe during the testing! What cool security things can we add?

**Coach:** Excellent! You're eager to fortify our testing environment even further! Now that we have our network and VMs set up, let's focus on implementing security controls to make our test as realistic as possible.
Think about CyberDefend Corp.'s web application. They likely have firewalls to control traffic. How would you configure the Azure Firewall in our test environment to simulate real-world traffic patterns and challenges for the attackers? What specific rules or configurations would you consider?

**Win:** Okay! For the Azure Firewall, we can pretend it's the bouncer for our website room! We should tell it:
Only let people who want to see the website (like regular visitors) come in through the special website door (port 80 and 443).
Don't let the attacker computers talk to the website computers unless we say it's okay for the test.
Maybe we can even watch what the traffic looks like to see if the attackers are trying sneaky things!

**Coach:** You're thinking like a security pro! Those are excellent points to consider for our Azure Firewall configuration:
Website Access: We'll allow inbound traffic on ports 80 (HTTP) and 443 (HTTPS) to simulate regular user access to the web application.
Controlled Communication: We'll block direct communication between the attacker subnet and the web application subnet by default. This forces attackers to find ways to bypass our defenses, just like in a real-world scenario.
Traffic Monitoring: You're absolutely right! We need to watch for suspicious activity. We'll enable logging and monitoring on the Azure Firewall to capture traffic details and analyze them for any malicious attempts or successful breaches.
You've successfully identified key considerations for configuring Azure Firewall in a penetration testing environment. You've earned 30 points for completing this final checkpoint!
Congratulations! You are 100% complete.
You've demonstrated a solid understanding of setting up a penetration testing environment in Azure. You're well on your way to becoming a skilled cybersecurity professional!
Keep up the good work! If you want to continue practicing, start a new chat.

**Coach:** During today's session covering Networking Setup, Virtual Machine Configuration, and Security Controls Implementation, our goal was to set up a penetration testing environment in Azure. Your responses show an Advanced level.
The strengths I saw in your responses are:
You grasp core concepts like subnets, NSGs, and security hardening.
You can apply those concepts to a realistic scenario and suggest practical configurations.
Keep up the good work! If you want to continue practicing, start a new chat.
