---
title: Hacking the free ANZ fitness band
layout: post
categories: [Project, ANZ, Fitnessband ,Nordic, nrf5283x]
image: /assets/img/2021-07-08/ANZ-Support-Band-Image.png
description: "Updating to commercial H707 firmware on ANZ free fitness band to use its full functionality"
---

![Fitness band photo](/assets/img/2021-07-08/ANZ-Support-Band-Image.png)
Some of you guys probably heard of and ordered the free ANZ Olympic support bands few weeks ago.
<https://supportband.anz.co.nz/registration-closed>
Like everyone else, I was excited and ordered two for me and my wife.
When it showed up, I was really disappointed. The only functionality the band has was literally show time and send vibration.
As a ANZ customer, thinking that my money has been spent on this thing just wouldn't let me through. So, I decided to have some fun with it.

Upon looking at some post on Choice Cheapies and searching for similar band, I figured out that these band were actually named H707.
I have confirmed this again, by checking the Bluetooth broadcast name of the band, which was "H707"

This band was based on Nordic Semiconductor's famous NRF5283X chipset, which I had some experience with.
Through this helpful post on Choice Cheapie, I have gotten hold of the firmware distribution package zip file.
<https://www.cheapies.nz/node/28151>

So, here is the step by step guide to update your fitness band.
Hope this finds more use.

*DISCLAIMER* I AM NOT LIABLE FOR ANY DAMAGE THAT THIS MAY CAUSE. IF YOU DO IT, IT'S YOUR RESPONSIBILITY.

1. Download the NRF Toolbox app from the Google Play store. (For iphone users check if it is there, I don't own an iPhone)
<https://play.google.com/store/apps/details?id=no.nordicsemi.android.nrftoolbox>

2. Download the firmware zip file on your phone from here <https://easyupload.io/6mea18>

3. Open NRF Toolbox and go to DFU (device firmware update) mode.
![Select DFU](/assets/img/2021-07-08/step1.jpg)

4. When selecting file check the "Distribution packet (ZIP)" and pick the file downloaded from above.
![Select Distribution Packet when selecting file](/assets/img/2021-07-08/step2.jpg)

5. Select "All" as the scope.
![Select all as scope](/assets/img/2021-07-08/step3.jpg)

6. Check if the status is "OK"
![Check status OK](/assets/img/2021-07-08/step4.jpg)

7. Go to Select Device and select your "H707" band
![Select H707](/assets/img/2021-07-08/step5.jpg)

8. Start upload, and once you finish you will see a toast that it is finished.
![Start Upload](/assets/img/2021-07-08/step6.jpg)

9. End of the firmware update. Download the fitness band software, "Fitpolo" from the Google Play Store.
<https://play.google.com/store/apps/details?id=com.moko.fitpolo>
![Finish uploading](/assets/img/2021-07-08/step7.jpg)