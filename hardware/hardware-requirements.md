# Hardware requirements

**Some notes before we begin:**

 
· The ideal set up, and best practice is to have a dedicated computer for staking. Try to limit additional processes running on your staking box. Especially if it is something that is connecting to the outside world. Every extra process and every file being downloaded is another opportunity for an exploit.
 
· At the time of writing, you are locking up at least 130,000 dollars in this endeavor. Your ETH will be locked in to the beaconchain until at earliest mid 2022, maybe later. It makes sense to buy some good hardware. This isn’t like mining with razor thin margins, it will pay for itself quickly. An anecdote: my server paid for itself after 3 days.
 
· Use Linux! It's easy, I promise. For the foreseeable future Linux will receive better support from both the client teams and the community at large. If you choose Linux you will have access to more guides and more technical support from the community at large. Linux is light weight, stable, secure, and it doesn't force you to restart for updates every other day.
 
· Use a minority client! It is both good for the health of Ethereum, and it is good for the health of your money. [You can read more about my thoughts on this here.]( https://old.reddit.com/r/ethstaker/comments/ptm04i/the_financial_incentive_to_run_a_minority_client/)

· A [battery back up]( https://www.newegg.com/apc-bx1500m-5-x-nema-5-15r-5-x-nema-5-15r/p/N82E16842301561?Description=battery%20back%20up&cm_re=battery_back%20up-_-42-301-561-_-Product&quicklink=true) is **strongly** recommended! Plug your modem and router in to it also. My ISP has generators to support emergency services communications, meaning the internet continues to work during a power outage as long as my equipment is powered. Your ISP may be the same. Aside from black-outs, not having your computer shut down on every momentary power flicker is a nice quality of life improvement from the admin’s (you) perspective.
 
· We have a few Rocket Pool fans hanging around here. Everything here applies to both solo staking and being a 16 ETH minipool node operator. 
 
[**Raspberry Pi 4 8GB**](https://www.pishop.us/product/raspberry-pi-4-model-b-8gb/?src=raspberrypi)
 
Price: $104.80 (including case, power supply, SD card, and heat sinks).
 
Performance: Running an execution and consensus node on a Raspberry Pi 4 is possible. Specifically Nimbus which was designed to run on devices like a Raspberry Pi. Being able to run Ethereum nodes on low powered hardware is great for decentralization and an honourable goal. However, running a validator is different. I maintain that the Pi’s lack of processing power and memory is a risk in some situations such as a period with no finalization. The reward of saving a few hundred dollars vs more powerful hardware does not even come close to outweighing the risk of extended downtime due to a lack of processing power or memory.
 
Power Usage: Approximately 8 watts. This would cost about 76 cents a month to run at 13c/kwh.
 
My opinion: I would not recommend purchasing a RPI4 for staking. (Sorry Joe!)
 
**Old laptop/desktop**
 
Price: Free! Well, kind of anyway.
 
CPU: For staking on mainnet, I would strongly recommend a CPU that scores at least 6000 or better on Passmark. For initial sync times single thread performance is better than having many cores.
 
Memory: Unless you go with an extremely bare bones OS, 16gb is the minimum amount of RAM I would recommend for mainnet. My staking machine typically sits at about 7.5-7.9gb used total which is too close for comfort to 8gb in my opinion.
 
Storage: An SSD is required. You do not need to worry about SATA vs NVMe, either will be fast enough. Buying one with a high terabytes written spec will help with longevity. The Ethereum execution and consensus layer (ETH1+2 if you ask Ben) are approaching 1TB in size so a 2TB or bigger drive is recommended.
 
Caveats: Stability and uptime are essential to maximize your profits. If you are using an older desktop consider replacing the PSU and the fans. Buying a titanium or platinum rated PSU will help save on the monthly power bill as well.
 
If you are planning on staking with an older laptop, consider that they have reduced capacity to deal with heat due to their form factor, and in rare cases, running while plugged in 24/7 can cause issues with the battery. If you do choose to stake with a laptop, I would recommend using one that far exceeds the CPU requirements as running a laptop at nearly full load 24/7 is not advisable. You will probably be fine, but generally speaking laptops are not designed with that in mind.
 
**New laptop**
 
If you are buying brand new, I do not see any value in paying the price premium for a portable form factor, screen, keyboard, and trackpad. Once you get your staking machine set up, you do not need any of these features. You can just remote into the staking machine from your daily driver computer. The low profile form factor will actually be a downside when taking thermal performance into account. Laptops typically do not include an ethernet port now, which means you will be relying on WiFi. WiFi is very reliable now, but you can't beat the simplicity and reliability of a cable.
 
[**New pre-built desktop**](https://www.newegg.com/p/1VK-0001-5YY35?quicklink=true)
 
Price: Around 700-900 dollars. There are likely better deals out there than the one I linked, that is just an example.
 
Performance: This will reliably and competently run any amount of validators. The CPU scores 17,149 on passmark. It has a 2TB SSD, and 16GB of ram. Any other prebuilt desktop with similar specs will work just as well. Shop around for one you like.
 
Power Usage: Probably around 30 watts. That is $2.85 per month at 13c/kwh.
 
My opinion: This is a great option. This is likely the simplest option and it will be easy to upgrade and service in the future
 
**Custom built desktop**
 
I won't go too in-depth here because this is essentially the same as using a prebuilt desktop. However, building your own gives you the option of choosing a case you like the look of, and buying higher quality parts. For those of you who have never built a computer, I assure you it is easier than Lego because they only go together one way. Also, you won’t get any weird proprietary parts that will be difficult to replace should they ever fail. Unfortunately with prebuilt computers, concessions are sometimes made with components like the PSU to assuage the accountants and boost margins.
 
Style points for adding a RAID card!
 
[**Intel NUC**](https://www.newegg.com/intel-nuc10i7fnh/p/1VK-004K-016A1?quicklink=true)
 
Price: About 1000 dollars. Note that it is possible to buy a barebones NUC with no storage or memory. You can sometimes find a better overall deal buying RAM and storage separately then assembling it yourself.
 
Performance: The one I linked weighs in at a mighty 10,077 passmark score, pair that up with 16GB of memory and it will run a node and more validators than Vitalik could spin up without breaking a sweat.
 
Power usage: 20-25ish watts. Around 2 dollars a month.
 
My opinion: NUCs are super cute, and their small form factor gives them a very high significant-other approval factor. Unfortunately that does come with a bit of a price premium and slightly less performance than the larger desktop option. However, these are minor drawbacks. This is probably the best option for most people.
 
**Server**
 
Price: You really need to look around for deals when it comes to this. Usedservers.com is one option but they charge a premium for the convenience and customization they offer. If you search through ebay, or even better your local classifieds you can often find a lightly used one for a few hundred bucks.
 
Performance: The 6000 passmark score is still in play here, but you should think about single thread performance as well. If it is a 24 core CPU that scores 6000, it will be worse than a 4 core CPU that also scores 6000.
 
Power Usage: [It's bad.](https://i.imgur.com/mliCfYr.png) My server runs around 100 watts, but it is pretty modern. If you get an older one, expect to be up around 150 watts. That's 10-14 dollars a month.
 
My opinion: This is my favorite option. Enterprise servers are jam packed with features, and are specifically designed to do exactly what we are trying to do. Run 24/7/365. They have redundant power supplies in case one breaks, they mostly have 2 CPUs, so in the unlikely event of one going bad, you can pop it out and restart with just one. They have built in RAID cards so you can have redundant storage. They have hot swappable drive trays, so if one of your drives goes bad, you don't even need to shut down. All of the components are high quality and built to last. You also get monitoring and maintenance tools that are not included in consumer gear like iDRAC and iLo. That's where that power usage graph I linked above came from. Neat right? I would definitely caution that while servers are great for staking, you probably want to be the type of person who is willing to go into the weeds a bit and geek out. There is some research required to know what you are looking for before you go out and buy a server and there is a possibility you run into a weird technical issue that you will have to troubleshoot.
 
[**DAppNode**](https://dappnode.io/)
 
Price: 1155€ (1300 USD)
 
Performance: The same as the NUC above, except you get 4TB of storage which somewhat justifies the bump in price. The DAppNodeXtreme is a good option if you are looking for a custom built OS with an easy UX. A DAppNode box is just a NUC pre configured with their software. If you are confident enough to install an OS by yourself, you can save a bit of money by purchasing a normal NUC and installing DAppNode yourself. You can also install the DAppNode OS on any computer. If you don’t want to mess around with installing operating systems and want an easy UX, buying a DAppNode box is a convenient and simple way to get started.
 
Power Usage: The same as the NUC above
 
My opinion: The DAppNode OS is very nice and easy to use. Unfortunately they (at the time of writing, they are working on fixing this) only support Prysm. While I love Prysm and their whole team, please read my “run a minority client” note above to understand why this is temporarily an issue that makes a DAppNode something I would not recommend. When support for Lighthouse, Teku, Nimbus, and Lodestar is added I would definitely recommend purchasing a DAppNode box.
 
[**Avado**](https://ava.do/shop)
 
A competitor to the DAppNode machines above. Their OS is not open source and they are more expensive than DAppNodes. Perhaps their OS has amazing UX and performance which justifies this price. I am not sure, I have not used it.
 
My Opinion: The closed source OS, high price, and only supporting Prysm lead me to not recommend the Avado for staking.
 
[**M1 Mac Mini**]( https://www.apple.com/shop/buy-mac/mac-mini)
 
Price: $899 for 16GB of memory + the cost of external 2TB of storage or $1699 for the 2TB version


Performance: Definitely upgrade to 16GB of memory. The CPU will be more than fast enough with a 15,108 passmark score. Make sure you have a plan to get up to 2TB or more of storage, the internal memory and storage is integrated into the motherboard and requires soldering and advanced technical knowledge to upgrade.
 
Power Usage: Slightly less than the NUC, but not enough to make any real difference.
 
My opinion: I still recommend people run Linux, and that is not possible with the new ARM architecture this uses. I think this loses out to the NUC in terms of price, support, upgradability, and ease of service, but for the Mac OS fans out there this is a great option that will work very well.
 
**Asus PN50/PN51**
 
As far as I can tell these are out of stock everywhere except for a few resellers who are charging a lot of money for them. They might be discontinued, or maybe just pandemic stuff. If you know, let me know.

 If you do manage to find one, it is Asus’ version of the NUC but it is built with AMD silicon. I know a few people that are currently staking on these and have heard nothing but great reviews. If you can find one do not hesitate to use this for staking, they are great.  
 

**Virtual Private Server**
 
Price: I looked over the different provider's websites and it looks to be anywhere from 20-40 dollars a month.
 
Performance: You can buy as much as you can afford.
 
My opinion: If you live somewhere that is prone to natural disaster or has an unstable power grid or internet connection but still want to solo stake, this is a good option. If you do have stable power and internet, running your own hardware will be a cheaper/more profitable solution long term. You need to evaluate the pros/cons of this for your own situation. Remember that if one of the VPS providers goes down, it will mean all of the people using that VPS service to host will also go down, and the inactivity penalties will be much larger than if you have uncorrelated down time yourself.
 
Simply using a decentralized staking service such as Rocket Pool will likely end up being more profitable unless you are staking a very large amount of ETH.
