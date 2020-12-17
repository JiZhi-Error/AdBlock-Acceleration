![Anurag’s github stats](https://github-readme-stats.vercel.app/api?username=Silentely&show_icons=true&theme=merko)

# AdBlock-Acceleration

International/China accelerated ad filtering rules subscription（[中文说明](https://github.com/Silentely/AdBlock-Acceleration/blob/master/README_CN.md)）

## 🔖 Filter Tool Recommendations 

Filtering tools：
* 🌍 browser plug-in
  * [AdGuard](https://adguard.com)
  * [uBlock Origin](https://github.com/gorhill/uBlock)
  * [AdBlock Plus](https://adblockplus.org)
  * [Adblock](https://getadblock.com)
* 📺 router terminal
  * [AdGuard Home](https://adguard.com/zh_cn/adguard-home/overview.html)
  * [KoolProxyR](https://github.com/user1121114685/koolproxyR)
  * [Adbyby](http://www.adbyby.com/)
  * [admflt](http://www.admflt.com)
* 📱 mobile 
  * [AdGuard for Android](https://adguard.com/zh_cn/adguard-android/overview.html)
  * [AdGuard for iOS](https://adguard.com/zh_cn/adguard-ios/overview.html)
* 💻 Desktop (global de-advertising)）
  * [AdGuard for Windows](https://adguard.com/zh_cn/adguard-windows/overview.html)
  * [AdGuard for macOS](https://adguard.com/zh_cn/adguard-mac/overview.html)
  
🙅‍♂️However, there is a pain point with all of these tools, as the rules are largely hosted on offshore servers, making updates extremely slow or even impossible to successfully update.

😫 A very common scenario: you've configured de-advertising tools for the elders and elderly in your family to prevent them from being phished, scammed or infected with viruses while browsing the web. But the fact is that often, many rules are carefully chosen, but in fact most of them are in the state of failure to update, and then a pop-up box appears, and the elder clicks randomly, but not necessarily what happens after ...... may say that the computer is broken, the update failed....

💥 This project is designed to solve this problem by updating the rules at light speed without going through any agents.

## 🕹 Project rationale
The project uses GitHub Actions to download the latest rules every 4 hours every day at UTC time, and then pushes them to GitHub Repo.
This works in conjunction with the [jsDelivr](https://www.jsdelivr.com) and [staticdn](https://raw.staticdn.net) global acceleration CDNs to distribute the rules.
The result is a second-by-second update of all de-advertising rules.

## 🧪 personal test
Under normal network environment (without any proxies, in mainland China network environment)
* Before using accelerated links: It can take up to 5 minutes and 12 seconds to update up to 13 rules, and 4 updates have failed.
* When accelerated links are used: all rules are updated within 15 seconds.

## 🚛 Refinement projects
I'd like you to submit an Issue or Request to help me improve the rules.

Submit the rules that you think you need to update for acceleration. The following points should be noted.

1. the rules need to be on an offshore server, difficult to successfully update or slow to update.
2. indicate the name, source, and function of the rule.
3. If the rule you want to speed up is a file in a GitHub project, just use the jsDelivr syntax to speed up the project file **without submitting a request**.
`https://cdn.jsdelivr.net/gh/username/project name@version/accelerate files`.

## 🍔 Usage
⚠️ Note: This rule is not for web proxy tools, don't give it to Surge, ShadowRocket, Quantumult(X), Clash(X/A) and similar tools!
Just copy the table below and use the accelerated address of the corresponding rule as a link to the subscription rule for the de-advertising tool.

## 📃 List of rules

|  🥑 Rule Name   |    original address  | 🚀 accelerated address（China） | 🚀 accelerated address（International）  |
|  :----:  | :----:  | :----:  | :----:  |
| AdGuard DNS filter | [original](https://adguardteam.github.io/AdGuardSDNSFilter/Filters/filter.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/AdGuard_Simplified_Domain_Names_Filter.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/AdGuard_Simplified_Domain_Names_Filter.txt) |
| Anti-AD | [original](https://anti-ad.net/easylist.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/Anti_AD_Easylist.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/Anti_AD_Easylist.txt) |
| EasyList China | [original](https://easylist-downloads.adblockplus.org/easylistchina.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/EasyList_China.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/EasyList_China.txt) |
| EasyPrivacy | [original](https://easylist-downloads.adblockplus.org/easyprivacy.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/EasyPrivacy.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/EasyPrivacy.txt) |
| I Don't Care About Cookies | [original](https://www.i-dont-care-about-cookies.eu/abp) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/I_dont_care_about_cookies.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/I_dont_care_about_cookies.txt) |
| HalfLife | [original](https://raw.githubusercontent.com/o0HalfLife0o/list/master/ad.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/HalfLife.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/HalfLife.txt ) |
| CJX's EasyList Lite | [original](https://raw.githubusercontent.com/cjx82630/cjxlist/master/cjxlist.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/CJX's_EasyList_Lite.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/CJX's_EasyList_Lite.txt) |
| CJX's Annoyance List | [original](https://raw.githubusercontent.com/cjx82630/cjxlist/master/cjx-annoyance.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/CJX's_Annoyance_List.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/CJX's_Annoyance_List.txt) |
| 乘风广告过滤 | [original](https://gitee.com/xinggsf/Adblock-Rule/raw/master/rule.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/Xinggsf_rule.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/Xinggsf_rule.txt) |
| 乘风视频过滤 | [original](https://gitee.com/xinggsf/Adblock-Rule/raw/master/mv.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/Xinggsf_mv.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/Xinggsf_mv.txt) |
| ADgk | [original](https://gitee.com/banbendalao/adguard/raw/master/ADgk.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/ADgk.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/ADgk.txt) |
| 大圣净化 | [original](https://raw.githubusercontent.com/jdlingyu/ad-wars/master/hosts) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/ds_hosts.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/ds_hosts.txt) |
| 1024 hosts | [original](https://raw.githubusercontent.com/Goooler/1024_hosts/master/hosts) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/1024_hosts.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/1024_hosts.txt) |
| iOSAdblockList | [original](https://raw.githubusercontent.com/BlackJack8/iOSAdblockList/master/iPv4Hosts.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/iPv4_hosts.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/iPv4_hosts.txt) |
| StevenBlack | [original](https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/Steven_hosts) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/Steven_hosts) |
| Hblock | [original](https://hblock.molinero.dev/hosts) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/Hblock_hosts) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/Hblock_hosts) |
| Malware Domain List | [original](https://www.malwaredomainlist.com/hostslist/hosts.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/Malware_host.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/Malware_hosts.txt) |
| Adblock Warning Removal List | [original](https://easylist-downloads.adblockplus.org/antiadblockfilters.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/antiadblockfilters.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/antiadblockfilters.txt) |
| Fanboy’s Annoyances List | [original](https://easylist-downloads.adblockplus.org/fanboy-annoyance.txt) | [accelerated](https://raw.staticdn.net/Silentely/AdBlock-Acceleration/master/fanboy-annoyance.txt) | [accelerated](https://cdn.jsdelivr.net/gh/Silentely/AdBlock-Acceleration/fanboy-annoyance.txt) |


##    Special thanks

* [@Hackl0us](https://github.com/Hackl0us)






