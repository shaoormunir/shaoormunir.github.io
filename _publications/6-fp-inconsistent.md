---
title: "FP-Inconsistent: Detecting Evasive Bots using Browser Fingerprint Inconsistencies"
classes: wide
---
[arXiv Preprint](https://arxiv.org/abs/2406.07647), **(arXiv 2024)**

*Hari Venugopalan, **Shaoor Munir**, Shuaib Ahmed, Tangbaihe Wang, Samuel T. King, Zubair Shafiq*

# Abstract
As browser fingerprinting is increasingly being used for bot detection, bots have started altering their fingerprints for evasion. We conduct the first large-scale evaluation of evasive bots to investigate whether and how altering fingerprints helps bots evade detection. To systematically investigate evasive bots, we deploy a honey site incorporating two anti-bot services (DataDome and BotD) and solicit bot traffic from 20 different bot services that purport to sell "realistic and undetectable traffic". Across half a million requests from 20 different bot services on our honey site, we find an average evasion rate of 52.93% against DataDome and 44.56% evasion rate against BotD. Our comparison of fingerprint attributes from bot services that evade each anti-bot service individually as well as bot services that evade both shows that bot services indeed alter different browser fingerprint attributes for evasion. Further, our analysis reveals the presence of inconsistent fingerprint attributes in evasive bots. Given evasive bots seem to have difficulty in ensuring consistency in their fingerprint attributes, we propose a data-driven approach to discover rules to detect such inconsistencies across space (two attributes in a given browser fingerprint) and time (a single attribute at two different points in time). These rules, which can be readily deployed by anti-bot services, reduce the evasion rate of evasive bots against DataDome and BotD by 48.11% and 44.95% respectively.