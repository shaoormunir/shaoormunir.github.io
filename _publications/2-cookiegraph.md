---
title: "COOKIEGRAPH: Measuring and Countering First-Party Tracking Cookies"
classes: wide
---
[arXiv preprint](https://arxiv.org/abs/2208.12370), **(2022)**

***Shaoor Munir**, Sandra Siby, Umar Iqbal, Steven Englehardt, Zubair Shafiq, Carmela Troncoso*
# Abstract
Recent privacy protections by browser vendors aim to limit the abuse of third-party cookies for cross-site tracking. While these countermeasures against third-party cookies are widely welcome, there are concerns that they will result in advertisers and trackers abusing first-party cookies instead. We provide the first empirical evidence of how first-party cookies are abused by advertisers and trackers by conducting a differential measurement study on 10K websites with third-party cookies allowed and blocked. We find that advertisers and trackers implement cross-site tracking despite third-party cookie blocking by storing identifiers, based on probabilistic and deterministic attributes, in first-party cookies. As opposed to third-party cookies, outright first-party cookie blocking is not practical because it would result in major breakage of legitimate website functionality.

We propose CookieGraph, a machine learning approach that can accurately and robustly detect first-party tracking cookies. CookieGraph detects first-party tracking cookies with 91.06% accuracy, outperforming the state-of-the-art CookieBlock approach by 10.28%. We show that CookieGraph is fully robust against cookie name manipulation while CookieBlock's accuracy drops by 15.68%. We also show that CookieGraph does not cause any major breakage while CookieBlock causes major breakage on 8% of the websites with SSO logins. Our deployment of CookieGraph shows that first-party tracking cookies are used on 93.43% of the 10K websites. We also find that the most prevalent first-party tracking cookies are set by major advertising entities such as Google as well as many specialized entities such as Criteo.